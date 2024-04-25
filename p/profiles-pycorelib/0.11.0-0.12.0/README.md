# Comparing `tmp/profiles_pycorelib-0.11.0-py3-none-any.whl.zip` & `tmp/profiles_pycorelib-0.12.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 4691 bytes, number of entries: 7
--rw-r--r--  2.0 unx      208 b- defN 24-Feb-12 06:08 profiles-pycorelib/__init__.py
--rw-r--r--  2.0 unx     4143 b- defN 24-Feb-12 06:17 profiles-pycorelib/common_col_union.py
--rw-r--r--  2.0 unx     4994 b- defN 24-Feb-12 06:17 profiles-pycorelib/sample_model.py
--rw-r--r--  2.0 unx      245 b- defN 24-Feb-29 05:45 profiles_pycorelib-0.11.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-29 05:45 profiles_pycorelib-0.11.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 24-Feb-29 05:45 profiles_pycorelib-0.11.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      617 b- defN 24-Feb-29 05:45 profiles_pycorelib-0.11.0.dist-info/RECORD
-7 files, 10318 bytes uncompressed, 3581 bytes compressed:  65.3%
+Zip file size: 9410 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      306 b- defN 24-Apr-17 11:22 profiles-pycorelib/__init__.py
+-rw-r--r--  2.0 unx    16817 b- defN 24-Apr-22 06:37 profiles-pycorelib/attribution_model.py
+-rw-r--r--  2.0 unx     5532 b- defN 24-Apr-22 12:10 profiles-pycorelib/common_col_union.py
+-rw-r--r--  2.0 unx     6336 b- defN 24-Apr-17 11:22 profiles-pycorelib/sample_model.py
+-rw-r--r--  2.0 unx      378 b- defN 24-Apr-25 11:19 profiles_pycorelib-0.12.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 11:19 profiles_pycorelib-0.12.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-Apr-25 11:19 profiles_pycorelib-0.12.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      714 b- defN 24-Apr-25 11:19 profiles_pycorelib-0.12.0.dist-info/RECORD
+8 files, 30194 bytes uncompressed, 8146 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: profiles-pycorelib/__init__.py
 Comment: 
 
+Filename: profiles-pycorelib/attribution_model.py
+Comment: 
+
 Filename: profiles-pycorelib/common_col_union.py
 Comment: 
 
 Filename: profiles-pycorelib/sample_model.py
 Comment: 
 
-Filename: profiles_pycorelib-0.11.0.dist-info/METADATA
+Filename: profiles_pycorelib-0.12.0.dist-info/METADATA
 Comment: 
 
-Filename: profiles_pycorelib-0.11.0.dist-info/WHEEL
+Filename: profiles_pycorelib-0.12.0.dist-info/WHEEL
 Comment: 
 
-Filename: profiles_pycorelib-0.11.0.dist-info/top_level.txt
+Filename: profiles_pycorelib-0.12.0.dist-info/top_level.txt
 Comment: 
 
-Filename: profiles_pycorelib-0.11.0.dist-info/RECORD
+Filename: profiles_pycorelib-0.12.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## profiles-pycorelib/__init__.py

```diff
@@ -1,5 +1,7 @@
 from profiles_rudderstack.project import WhtProject
 from .common_col_union import CommonColumnUnionModel
+from .attribution_model import AttributionModel
 
 def register_extensions(project: WhtProject):
     project.register_model_type(CommonColumnUnionModel)
+    project.register_model_type(AttributionModel)
```

## profiles-pycorelib/common_col_union.py

```diff
@@ -34,15 +34,56 @@
         self.inputs = inputs
         self.logger = Logger("common_column_union_recipe")
         self.sql = ""
 
     def describe(self, this: WhtMaterial):
         return self.sql, ".sql"
 
-    def prepare(self, this: WhtMaterial):
+    def register_dependencies(self, this: WhtMaterial):
+        is_null_ctx = this.wht_ctx.is_null_ctx
+        if is_null_ctx:
+            for in_model in self.inputs:
+                this.de_ref(in_model, edge_type="optional")
+            return
+        
+        inputs = [] # enabled inputs
+        common_columns_count = {}
+        for in_model in self.inputs:
+            in_material = this.de_ref(in_model, edge_type="optional")
+            if in_material is None:
+                continue # disabled
+
+            inputs.append(in_model)
+
+        union_sql = ""
+        union_queries = []
+        for in_model in inputs:
+            union_queries.append(
+            f"""{{% with input_mat = this.DeRef('{in_model}') %}}
+                    select  <determined at runtime> from {{{{input_mat}}}}
+                {{% endwith %}}"""
+            )
+            
+        union_sql = " UNION ALL ".join(union_queries)
+        
+        
+        sql = this.execute_text_template(
+            f"""
+            {{% macro begin_block() %}}
+                {{% macro selector_sql() %}}
+                    {union_sql}
+                {{% endmacro %}}
+                {{% exec %}} {{{{warehouse.CreateReplaceTableAs(this.Name(), selector_sql())}}}} {{% endexec %}}
+            {{% endmacro %}}
+            
+            {{% exec %}} {{{{warehouse.BeginEndBlock(begin_block())}}}} {{% endexec %}}"""
+        )
+        self.sql = sql            
+
+    def execute(self, this: WhtMaterial):
         is_null_ctx = this.wht_ctx.is_null_ctx
         if is_null_ctx:
             for in_model in self.inputs:
                 this.de_ref(in_model, edge_type="optional")
             return
         
         inputs = [] # enabled inputs
@@ -94,14 +135,12 @@
                     {union_sql}
                 {{% endmacro %}}
                 {{% exec %}} {{{{warehouse.CreateReplaceTableAs(this.Name(), selector_sql())}}}} {{% endexec %}}
             {{% endmacro %}}
             
             {{% exec %}} {{{{warehouse.BeginEndBlock(begin_block())}}}} {{% endexec %}}"""
         )
-        self.sql = sql            
-
-    def execute(self, this: WhtMaterial):
+        self.sql = sql        
         if self.sql == "":
             self.logger.error("error executing common_column_union_recipe, sql is empty")
         
         this.wht_ctx.client.query_sql_without_result(self.sql)
```

## profiles-pycorelib/sample_model.py

```diff
@@ -45,15 +45,56 @@
         self.sql = "" # the sql code to be executed
 
     # describe the compile output of the recipe - the sql code and the extension of the file
     def describe(self, this: WhtMaterial):
         return self.sql, ".sql"
 
     # prepare the material for execution - de_ref the inputs and create the sql code
-    def prepare(self, this: WhtMaterial):
+    def register_dependencies(self, this: WhtMaterial):
+        is_null_ctx = this.wht_ctx.is_null_ctx
+        if is_null_ctx:
+            for in_model in self.inputs:
+                this.de_ref(in_model, edge_type="optional")
+            return
+
+        inputs = [] # enabled inputs
+        common_columns_count = {}
+        for in_model in self.inputs:
+            in_material = this.de_ref(in_model, edge_type="optional")
+            if in_material is None:
+                continue # disabled
+
+            inputs.append(in_model)
+           
+        union_sql = ""
+        union_queries = []
+        for in_model in inputs:
+            union_queries.append(
+            f"""{{% with input_mat = this.DeRef('{in_model}') %}}
+                    select <determined at runtime> from {{{{input_mat}}}}
+                {{% endwith %}}"""
+            )
+
+        union_sql = " UNION ALL ".join(union_queries)
+
+        sql = this.execute_text_template(
+            f"""
+            {{% macro begin_block() %}}
+                {{% macro selector_sql() %}}
+                    {union_sql}
+                {{% endmacro %}}
+                {{% exec %}} {{{{warehouse.CreateReplaceTableAs(this.Name(), selector_sql())}}}} {{% endexec %}}
+            {{% endmacro %}}
+
+            {{% exec %}} {{{{warehouse.BeginEndBlock(begin_block())}}}} {{% endexec %}}"""
+        )
+        self.sql = sql
+
+    # execute the material
+    def execute(self, this: WhtMaterial):
         is_null_ctx = this.wht_ctx.is_null_ctx
         if is_null_ctx:
             for in_model in self.inputs:
                 this.de_ref(in_model, edge_type="optional")
             return
 
         inputs = [] # enabled inputs
@@ -104,16 +145,13 @@
                 {{% endmacro %}}
                 {{% exec %}} {{{{warehouse.CreateReplaceTableAs(this.Name(), selector_sql())}}}} {{% endexec %}}
             {{% endmacro %}}
 
             {{% exec %}} {{{{warehouse.BeginEndBlock(begin_block())}}}} {{% endexec %}}"""
         )
         self.sql = sql
-
-    # execute the material
-    def execute(self, this: WhtMaterial):
         if self.sql == "":
             model_name = this.model.name()
             self.logger.error(f"error executing {model_name} model, compiled sql is empty")
 
         # execute the sql code
         this.wht_ctx.client.query_sql_without_result(self.sql)
```

