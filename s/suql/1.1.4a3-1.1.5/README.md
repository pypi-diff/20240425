# Comparing `tmp/suql-1.1.4a3.tar.gz` & `tmp/suql-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suql-1.1.4a3.tar", last modified: Wed Apr 17 08:35:23 2024, max compression
+gzip compressed data, was "suql-1.1.5.tar", last modified: Thu Apr 25 17:52:14 2024, max compression
```

## Comparing `suql-1.1.4a3.tar` & `suql-1.1.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwx------   0 oval      (1000) users      (100)        0 2024-04-17 08:35:23.062679 suql-1.1.4a3/
--rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.1.4a3/LICENSE
--rw-------   0 oval      (1000) users      (100)     4884 2024-04-17 08:35:23.062679 suql-1.1.4a3/PKG-INFO
--rw-------   0 oval      (1000) users      (100)     4278 2024-04-15 19:06:57.000000 suql-1.1.4a3/README.md
--rw-------   0 oval      (1000) users      (100)       38 2024-04-17 08:35:23.062679 suql-1.1.4a3/setup.cfg
--rw-------   0 oval      (1000) users      (100)     1514 2024-04-17 08:34:48.000000 suql-1.1.4a3/setup.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-17 08:35:23.058679 suql-1.1.4a3/src/
-drwx------   0 oval      (1000) users      (100)        0 2024-04-17 08:35:23.058679 suql-1.1.4a3/src/suql/
--rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.1.4a3/src/suql/__init__.py
--rw-------   0 oval      (1000) users      (100)    17354 2024-04-07 06:37:06.000000 suql-1.1.4a3/src/suql/agent.py
--rw-------   0 oval      (1000) users      (100)    16980 2024-04-17 07:37:16.000000 suql-1.1.4a3/src/suql/faiss_embedding.py
--rw-------   0 oval      (1000) users      (100)     8792 2024-04-17 07:27:02.000000 suql-1.1.4a3/src/suql/free_text_fcns_server.py
--rw-------   0 oval      (1000) users      (100)     3591 2024-04-12 01:45:49.000000 suql-1.1.4a3/src/suql/postgresql_connection.py
--rw-------   0 oval      (1000) users      (100)     9612 2024-04-17 08:33:05.000000 suql-1.1.4a3/src/suql/prompt_continuation.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-17 08:35:23.062679 suql-1.1.4a3/src/suql/prompts/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.1.4a3/src/suql/prompts/__init__.py
--rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.1.4a3/src/suql/prompts/answer_qa.prompt
--rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.1.4a3/src/suql/prompts/field_classification.prompt
--rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.1.4a3/src/suql/prompts/if_db_classification.prompt
--rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.1.4a3/src/suql/prompts/opening_hours.prompt
--rw-------   0 oval      (1000) users      (100)     5574 2024-04-03 06:02:28.000000 suql-1.1.4a3/src/suql/prompts/parser_suql.prompt
--rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.1.4a3/src/suql/prompts/verification.prompt
--rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.1.4a3/src/suql/prompts/yelp_response_SQL.prompt
--rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.1.4a3/src/suql/prompts/yelp_response_no_results.prompt
-drwx------   0 oval      (1000) users      (100)        0 2024-04-17 08:35:23.062679 suql-1.1.4a3/src/suql/sql_free_text_support/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.1.4a3/src/suql/sql_free_text_support/__init__.py
--rw-------   0 oval      (1000) users      (100)    65217 2024-04-17 08:34:40.000000 suql-1.1.4a3/src/suql/sql_free_text_support/execute_free_text_sql.py
--rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.1.4a3/src/suql/utils.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-17 08:35:23.058679 suql-1.1.4a3/src/suql.egg-info/
--rw-r--r--   0 oval      (1000) users      (100)     4884 2024-04-17 08:35:22.000000 suql-1.1.4a3/src/suql.egg-info/PKG-INFO
--rw-------   0 oval      (1000) users      (100)      824 2024-04-17 08:35:23.000000 suql-1.1.4a3/src/suql.egg-info/SOURCES.txt
--rw-------   0 oval      (1000) users      (100)        1 2024-04-17 08:35:22.000000 suql-1.1.4a3/src/suql.egg-info/dependency_links.txt
--rw-------   0 oval      (1000) users      (100)      186 2024-04-17 08:35:22.000000 suql-1.1.4a3/src/suql.egg-info/requires.txt
--rw-------   0 oval      (1000) users      (100)        5 2024-04-17 08:35:22.000000 suql-1.1.4a3/src/suql.egg-info/top_level.txt
+drwx------   0 oval      (1000) users      (100)        0 2024-04-25 17:52:14.590216 suql-1.1.5/
+-rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.1.5/LICENSE
+-rw-------   0 oval      (1000) users      (100)     4882 2024-04-25 17:52:14.590216 suql-1.1.5/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)     4278 2024-04-15 19:06:57.000000 suql-1.1.5/README.md
+-rw-------   0 oval      (1000) users      (100)       38 2024-04-25 17:52:14.590216 suql-1.1.5/setup.cfg
+-rw-------   0 oval      (1000) users      (100)     1512 2024-04-25 17:52:02.000000 suql-1.1.5/setup.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-25 17:52:14.586217 suql-1.1.5/src/
+drwx------   0 oval      (1000) users      (100)        0 2024-04-25 17:52:14.590216 suql-1.1.5/src/suql/
+-rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.1.5/src/suql/__init__.py
+-rw-------   0 oval      (1000) users      (100)    17393 2024-04-25 17:52:02.000000 suql-1.1.5/src/suql/agent.py
+-rw-------   0 oval      (1000) users      (100)    16980 2024-04-25 17:38:32.000000 suql-1.1.5/src/suql/faiss_embedding.py
+-rw-------   0 oval      (1000) users      (100)     8792 2024-04-17 07:27:02.000000 suql-1.1.5/src/suql/free_text_fcns_server.py
+-rw-------   0 oval      (1000) users      (100)     3563 2024-04-25 17:52:02.000000 suql-1.1.5/src/suql/postgresql_connection.py
+-rw-------   0 oval      (1000) users      (100)     9612 2024-04-17 08:33:05.000000 suql-1.1.5/src/suql/prompt_continuation.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-25 17:52:14.590216 suql-1.1.5/src/suql/prompts/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.1.5/src/suql/prompts/__init__.py
+-rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.1.5/src/suql/prompts/answer_qa.prompt
+-rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.1.5/src/suql/prompts/field_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.1.5/src/suql/prompts/if_db_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.1.5/src/suql/prompts/opening_hours.prompt
+-rw-------   0 oval      (1000) users      (100)     5574 2024-04-03 06:02:28.000000 suql-1.1.5/src/suql/prompts/parser_suql.prompt
+-rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.1.5/src/suql/prompts/verification.prompt
+-rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.1.5/src/suql/prompts/yelp_response_SQL.prompt
+-rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.1.5/src/suql/prompts/yelp_response_no_results.prompt
+drwx------   0 oval      (1000) users      (100)        0 2024-04-25 17:52:14.590216 suql-1.1.5/src/suql/sql_free_text_support/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.1.5/src/suql/sql_free_text_support/__init__.py
+-rw-------   0 oval      (1000) users      (100)    66566 2024-04-25 17:52:02.000000 suql-1.1.5/src/suql/sql_free_text_support/execute_free_text_sql.py
+-rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.1.5/src/suql/utils.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-25 17:52:14.590216 suql-1.1.5/src/suql.egg-info/
+-rw-r--r--   0 oval      (1000) users      (100)     4882 2024-04-25 17:52:14.000000 suql-1.1.5/src/suql.egg-info/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)      824 2024-04-25 17:52:14.000000 suql-1.1.5/src/suql.egg-info/SOURCES.txt
+-rw-------   0 oval      (1000) users      (100)        1 2024-04-25 17:52:14.000000 suql-1.1.5/src/suql.egg-info/dependency_links.txt
+-rw-------   0 oval      (1000) users      (100)      186 2024-04-25 17:52:14.000000 suql-1.1.5/src/suql.egg-info/requires.txt
+-rw-------   0 oval      (1000) users      (100)        5 2024-04-25 17:52:14.000000 suql-1.1.5/src/suql.egg-info/top_level.txt
```

### Comparing `suql-1.1.4a3/LICENSE` & `suql-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a3/PKG-INFO` & `suql-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.1.4a3
+Version: 1.1.5
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.1.4a3 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.5 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `suql-1.1.4a3/README.md` & `suql-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a3/setup.py` & `suql-1.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 # Package metadata
 name = "suql"
-version = "1.1.4a3"
+version = "1.1.5"
 description = "Structured and Unstructured Query Language (SUQL) Python API"
 author = "Shicheng Liu"
 author_email = "shicheng@cs.stanford.edu"
 url = "https://github.com/stanford-oval/suql"
 
 # Specify the packages to include. You can use `find_packages` to automatically discover them.
 packages = find_packages(where="src")
```

### Comparing `suql-1.1.4a3/src/suql/agent.py` & `suql-1.1.5/src/suql/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,18 @@
         postprocess=False,
     )
     print("directly generated SUQL query: {}".format(generated_suql))
     postprocessed_suql = postprocess_suql(generated_suql)
 
     suql_execute_start_time = time.time()
     final_res, column_names, cache = suql_execute(
-        postprocessed_suql, {"restaurants": "_id"}, fts_fields=[("restaurants", "name")]
+        postprocessed_suql,
+        {"restaurants": "_id"},
+        "restaurants",
+        fts_fields=[("restaurants", "name")]
     )
     suql_execute_end_time = time.time()
 
     results_for_ned = extract_id_name(final_res, column_names)
     final_res = clean_up_response(final_res, column_names)
 
     return (
```

### Comparing `suql-1.1.4a3/src/suql/faiss_embedding.py` & `suql-1.1.5/src/suql/faiss_embedding.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a3/src/suql/free_text_fcns_server.py` & `suql-1.1.5/src/suql/free_text_fcns_server.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a3/src/suql/postgresql_connection.py` & `suql-1.1.5/src/suql/postgresql_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import time
 
 import psycopg2
 
 
 def execute_sql(
     sql_query,
-    database="restaurants",
+    database,
     user="select_user",
     password="select_user",
     data=None,
     commit_in_lieu_fetch=False,
     no_print=False,
 ):
     start_time = time.time()
@@ -68,15 +68,15 @@
     end_time = time.time()
     elapsed_time = end_time - start_time
     return list(results), column_names, elapsed_time
 
 
 def execute_sql_with_column_info(
     sql_query,
-    database="restaurants",
+    database,
     user="select_user",
     password="select_user",
     unprotected=False,
 ):
     # Establish a connection to the PostgreSQL database
     conn = psycopg2.connect(
         database=database,
```

### Comparing `suql-1.1.4a3/src/suql/prompt_continuation.py` & `suql-1.1.5/src/suql/prompt_continuation.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a3/src/suql/prompts/if_db_classification.prompt` & `suql-1.1.5/src/suql/prompts/if_db_classification.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a3/src/suql/prompts/opening_hours.prompt` & `suql-1.1.5/src/suql/prompts/opening_hours.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a3/src/suql/prompts/parser_suql.prompt` & `suql-1.1.5/src/suql/prompts/parser_suql.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a3/src/suql/prompts/yelp_response_SQL.prompt` & `suql-1.1.5/src/suql/prompts/yelp_response_SQL.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a3/src/suql/prompts/yelp_response_no_results.prompt` & `suql-1.1.5/src/suql/prompts/yelp_response_no_results.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a3/src/suql/sql_free_text_support/execute_free_text_sql.py` & `suql-1.1.5/src/suql/sql_free_text_support/execute_free_text_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,14 +192,15 @@
     return visitor.res
 
 
 class _SelectVisitor(Visitor):
     def __init__(
         self,
         fts_fields,
+        database,
         embedding_server_address,
         select_username,
         select_userpswd,
         create_username,
         create_userpswd,
         table_w_ids,
         llm_model_name,
@@ -222,14 +223,17 @@
         self.table_w_ids = table_w_ids
         
         # store default LLM
         self.llm_model_name = llm_model_name
         
         # store max verify param
         self.max_verify = max_verify
+        
+        # store database
+        self.database = database
 
     def __call__(self, node):
         super().__call__(node)
 
     def visit_SelectStmt(self, ancestors, node: SelectStmt):
         type_cast_answer_visitor = _TypeCastAnswer()
         type_cast_answer_visitor(node)
@@ -251,14 +255,15 @@
         if freeTextFcnVisitor.res:
             tmp_table_name = "temp_table_{}".format(_generate_random_string())
             self.tmp_tables.append(tmp_table_name)
 
             # main entry point for SUQL compiler optimization
             results, column_info = _analyze_SelectStmt(
                 node,
+                self.database,
                 self.cache,
                 self.fts_fields,
                 self.embedding_server_address,
                 self.select_username,
                 self.select_userpswd,
                 self.table_w_ids,
                 self.llm_model_name,
@@ -269,14 +274,15 @@
             column_create_stmt = ",\n".join(
                 list(map(lambda x: f'"{x[0]}" {x[1]}', column_info))
             )
             create_stmt = f"CREATE TABLE {tmp_table_name} (\n{column_create_stmt}\n); GRANT SELECT ON {tmp_table_name} TO {self.select_username};"
             logging.info("created table {}".format(tmp_table_name))
             execute_sql(
                 create_stmt,
+                self.database,
                 user=self.create_username,
                 password=self.create_userpswd,
                 commit_in_lieu_fetch=True,
                 no_print=True,
             )
 
             if results:
@@ -292,14 +298,15 @@
                         [
                             json.dumps(element) if index in json_indices else element
                             for index, element in enumerate(result)
                         ]
                     )
                     execute_sql(
                         f"INSERT INTO {tmp_table_name} VALUES ({placeholder_str})",
+                        self.database,
                         data=updated_results,
                         user=self.create_username,
                         password=self.create_userpswd,
                         commit_in_lieu_fetch=True,
                         no_print=True
                     )
 
@@ -307,14 +314,15 @@
             node.fromClause = (
                 RangeVar(relname=tmp_table_name, inh=True, relpersistence="p"),
             )
             node.whereClause = None
         else:
             _classify_db_fields(
                 node,
+                self.database,
                 self.cache,
                 self.fts_fields,
                 self.select_username,
                 self.select_userpswd,
                 self.llm_model_name
             )
 
@@ -343,14 +351,15 @@
         return dict(res)
 
     def drop_tmp_tables(self):
         for tmp_table_name in self.tmp_tables:
             drop_stmt = f"DROP TABLE {tmp_table_name}"
             execute_sql(
                 drop_stmt,
+                self.database,
                 user=self.create_username,
                 password=self.create_userpswd,
                 commit_in_lieu_fetch=True,
                 no_print=True
             )
 
 
@@ -836,18 +845,26 @@
     except ValueError:
         # If a ValueError is raised, it means at least one value is not a valid number, so return False
         return False
 
 
 class _StructuralClassification(Visitor):
     def __init__(
-        self, node: SelectStmt, cache, fts_fields, select_username, select_userpswd, llm_model_name
+        self,
+        node: SelectStmt,
+        database,
+        cache,
+        fts_fields,
+        select_username,
+        select_userpswd,
+        llm_model_name
     ) -> None:
         super().__init__()
         self.node = node
+        self.database = database
         self.cache = cache
         self.fts_fields = fts_fields
         self.select_username = select_username
         self.select_userpswd = select_userpswd
         self.llm_model_name = llm_model_name
 
     def __call__(self, node):
@@ -929,26 +946,28 @@
         to_execute_node.groupClause = None
         # reset sorting
         to_execute_node.sortClause = None
 
         try:
             res, column_infos = execute_sql_with_column_info(
                 RawStream()(to_execute_node),
+                self.database,
                 unprotected=True,
                 user=self.select_username,
                 password=self.select_userpswd,
             )
             # it is possible if there is a type error
             # e.g. "Passengers ( 2017 )" = '490,000', but "Passengers ( 2017 )" is actually of type int
             # in such cases, the `column_infos` variable would not capture the actual type and instead stores an empty list
             # thus execute an empty query just to find out the type
             if column_infos == []:
                 to_execute_node.whereClause = None
                 _, column_infos = execute_sql_with_column_info(
                     RawStream()(to_execute_node),
+                    self.database,
                     user=self.select_username,
                     password=self.select_userpswd,
                 )
         except psyconpg2Error:
             logging.info(
                 "above error happens during ENUM classification attempts. Marking this predicate as returning answer."
             )
@@ -1022,14 +1041,15 @@
                     )
 
                 to_execute_node.sortClause = None
                 to_execute_node.whereClause = None
                 to_execute_node.limitCount = None  # find all entries
                 field_value_choices, _ = execute_sql_with_column_info(
                     RawStream()(to_execute_node),
+                    self.database,
                     user=self.select_username,
                     password=self.select_userpswd,
                 )
                 # TODO deal with list problems?
                 field_value_choices = list(map(lambda x: x[0], field_value_choices))
                 field_value_choices.sort()
 
@@ -1062,26 +1082,33 @@
                             )
                             _replace_a_expr_field(node, ancestors, parsed_res)
                             self.cache[column_name][value_res_clear] = parsed_res
 
 
 def _classify_db_fields(
     node: SelectStmt,
+    database: str,
     cache: dict,
     fts_fields: List,
     select_username: str,
     select_userpswd: str,
     llm_model_name: str
 ):
     # we expect all atomic predicates under `predicate` to only involve stru fields
     # (no `answer` function)
     # the goal of this function is to determine which predicate leads to no results
     # for a field without results, try to classify into one of the existing fields
     visitor = _StructuralClassification(
-        node, cache, fts_fields, select_username, select_userpswd, llm_model_name
+        node,
+        database,
+        cache,
+        fts_fields,
+        select_username,
+        select_userpswd,
+        llm_model_name
     )
     visitor(node)
 
 
 class _Replace_Original_Target_Visitor(Visitor):
     def __init__(self, table_column_mapping={}) -> None:
         super().__init__()
@@ -1103,14 +1130,15 @@
                         break
                     res = (String(sval=f"{table_name}^{node.fields[0].sval}"),)
             node.fields = res
 
 
 def _execute_structural_sql(
     original_node: SelectStmt,
+    database: str,
     predicate: BoolExpr,
     cache: dict,
     fts_fields: List,
     select_username: str,
     select_userpswd: str,
     llm_model_name: str
 ):
@@ -1124,14 +1152,15 @@
     elif len(node.fromClause) == 1 and isinstance(node.fromClause[0], JoinExpr):
         all_projection_fields = []
         table_column_mapping = {}
         for table in [node.fromClause[0].larg, node.fromClause[0].rarg]:
             # find out what columns this table has
             _, columns = _execute_structural_sql(
                 SelectStmt(fromClause=(table,)),
+                database,
                 None,
                 cache,
                 fts_fields,
                 select_username,
                 select_userpswd,
                 llm_model_name
             )
@@ -1164,14 +1193,15 @@
     # next, there are tuple joins (self joins)
     elif len(node.fromClause) > 1 and isinstance(node.fromClause, tuple):
         all_projection_fields = []
         for table in node.fromClause:
             # find out what columns this table has
             _, columns = _execute_structural_sql(
                 SelectStmt(fromClause=(table,)),
+                database,
                 None,
                 cache,
                 fts_fields,
                 select_username,
                 select_userpswd,
                 llm_model_name
             )
@@ -1210,19 +1240,30 @@
     node.groupClause = None
     node.havingClause = None
 
     # only queries that involve only structural parts can be executed
     assert _if_all_structural(node)
 
     # deal with sturctural field classification
-    _classify_db_fields(node, cache, fts_fields, select_username, select_userpswd, llm_model_name)
+    _classify_db_fields(
+        node,
+        database,
+        cache,
+        fts_fields,
+        select_username,
+        select_userpswd,
+        llm_model_name
+    )
 
     sql = RawStream()(node)
     return execute_sql_with_column_info(
-        sql, user=select_username, password=select_userpswd
+        sql, 
+        database,
+        user=select_username,
+        password=select_userpswd
     )
 
 
 def _execute_free_text_queries(
     node,
     predicate: BoolExpr,
     existing_results,
@@ -1373,14 +1414,15 @@
                 RawStream()(predicate)
             )
         )
 
 
 def _execute_and(
     sql_dnf_predicates,
+    database: str,
     node: SelectStmt,
     limit,
     cache: dict,
     fts_fields: List,
     embedding_server_address,
     select_username,
     select_userpswd,
@@ -1406,14 +1448,15 @@
             structural_predicates = BoolExpr(
                 boolop=BoolExprType.AND_EXPR, args=structural_predicates
             )
 
         # execute structural part
         structural_res, column_info = _execute_structural_sql(
             node,
+            database,
             structural_predicates,
             cache,
             fts_fields,
             select_username,
             select_userpswd,
             llm_model_name
         )
@@ -1443,24 +1486,32 @@
     elif isinstance(sql_dnf_predicates, A_Expr) or (
         isinstance(sql_dnf_predicates, BoolExpr)
         and sql_dnf_predicates.boolop == BoolExprType.NOT_EXPR
     ):
         if _if_all_structural(sql_dnf_predicates):
             return _execute_structural_sql(
                 node,
+                database,
                 sql_dnf_predicates,
                 cache,
                 fts_fields,
                 select_username,
                 select_userpswd,
                 llm_model_name
             )
         else:
             all_results, column_info = _execute_structural_sql(
-                node, None, cache, fts_fields, select_username, select_userpswd, llm_model_name
+                node,
+                database,
+                None,
+                cache,
+                fts_fields,
+                select_username,
+                select_userpswd,
+                llm_model_name
             )
             return _execute_free_text_queries(
                 node,
                 sql_dnf_predicates,
                 all_results,
                 column_info,
                 limit,
@@ -1469,14 +1520,15 @@
                 llm_model_name,
                 max_verify
             )
 
 
 def _analyze_SelectStmt(
     node: SelectStmt,
+    database: str,
     cache: dict,
     fts_fields: List,
     embedding_server_address: str,
     select_username: str,
     select_userpswd: str,
     table_w_ids: dict,
     llm_model_name: str,
@@ -1494,14 +1546,15 @@
         choices = sorted(
             sql_dnf_predicates.args, key=lambda x: _if_all_structural(x), reverse=True
         )
         res = []
         for choice in choices:
             choice_res, column_info = _execute_and(
                 choice,
+                database,
                 node,
                 limit - len(res),
                 cache,
                 fts_fields,
                 embedding_server_address,
                 select_username,
                 select_userpswd,
@@ -1519,14 +1572,15 @@
 
     elif (
         isinstance(sql_dnf_predicates, BoolExpr)
         and sql_dnf_predicates.boolop == BoolExprType.AND_EXPR
     ):
         return _execute_and(
             sql_dnf_predicates,
+            database,
             node,
             limit,
             cache,
             fts_fields,
             embedding_server_address,
             select_username,
             select_userpswd,
@@ -1537,14 +1591,15 @@
 
     elif isinstance(sql_dnf_predicates, A_Expr) or (
         isinstance(sql_dnf_predicates, BoolExpr)
         and sql_dnf_predicates.boolop == BoolExprType.NOT_EXPR
     ):
         return _execute_and(
             sql_dnf_predicates,
+            database,
             node,
             limit,
             cache,
             fts_fields,
             embedding_server_address,
             select_username,
             select_userpswd,
@@ -1584,14 +1639,15 @@
     
     return _answer(source_content, query)
     
 
 def suql_execute(
     suql,
     table_w_ids,
+    database,
     fts_fields=[],
     llm_model_name="gpt-3.5-turbo-0125",
     max_verify=20,
     loggings="",
     log_filename=None,
     disable_try_catch=False,
     embedding_server_address="http://127.0.0.1:8501",
@@ -1606,15 +1662,17 @@
 
     # Parameters:
     `suql` (str): The to-be-executed suql query.
     
     `table_w_ids` (dict): A dictionary where each key is a table name, and each value is the corresponding
         unique ID column name in this table, e.g., `table_w_ids = {"restaurants": "_id"}`, meaning that the
         relevant tables to the SUQL compiler include only the `restaurants` table, which has unique ID column `_id`.
-        
+    
+    `database` (str): The name of the PostgreSQL database to execute the query.
+    
     `fts_fields` (List[str], optional): Fields that should use PostgreSQL's Full Text Search (FTS) operators;
         The SUQL compiler would change certain string operators like "=" to use PostgreSQL's FTS operators.
         It uses `websearch_to_tsquery` and the `@@` operator to match against these fields.
         
     `llm_model_name` (str, optional): The LLM to be used by the SUQL compiler.
         Defaults to `gpt-3.5-turbo-0125`.
         
@@ -1681,14 +1739,15 @@
 
     if _parse_standalone_answer(suql) is not None:
         return _execute_standalone_answer(suql, source_file_mapping), [], {}
 
     results, column_names, cache = _suql_execute_single(
         suql,
         table_w_ids,
+        database,
         fts_fields,
         llm_model_name,
         max_verify,
         embedding_server_address,
         loggings,
         disable_try_catch,
         select_username,
@@ -1713,14 +1772,15 @@
     # TODO: handle cases to go to multiple projection fields, from hybridQA
     return results, column_names, cache
 
 
 def _suql_execute_single(
     suql,
     table_w_ids,
+    database,
     fts_fields,
     llm_model_name,
     max_verify,
     embedding_server_address,
     loggings,
     disable_try_catch,
     select_username,
@@ -1731,33 +1791,41 @@
     results = []
     column_names = []
     cache = {}
 
     if disable_try_catch:
         visitor = _SelectVisitor(
             fts_fields,
+            database,
             embedding_server_address,
             select_username,
             select_userpswd,
             create_username,
             create_userpswd,
             table_w_ids,
             llm_model_name,
             max_verify
         )
         root = parse_sql(suql)
         visitor(root)
         second_sql = RawStream()(root)
         cache = visitor.serialize_cache()
 
-        return execute_sql(second_sql, user=select_username, password=select_userpswd, no_print=True)
+        return execute_sql(
+            second_sql,
+            database,
+            user=select_username,
+            password=select_userpswd,
+            no_print=True
+        )
     else:
         try:
             visitor = _SelectVisitor(
                 fts_fields,
+                database,
                 embedding_server_address,
                 select_username,
                 select_userpswd,
                 create_username,
                 create_userpswd,
                 table_w_ids,
                 llm_model_name,
@@ -1765,15 +1833,19 @@
             )
             root = parse_sql(suql)
             visitor(root)
             second_sql = RawStream()(root)
             cache = visitor.serialize_cache()
 
             results, column_names, cache = execute_sql(
-                second_sql, user=select_username, password=select_userpswd, no_print=True
+                second_sql,
+                database,
+                user=select_username,
+                password=select_userpswd,
+                no_print=True
             )
         except Exception as err:
             with open("_suql_error_log.txt", "a") as file:
                 file.write(f"==============\n")
                 file.write(f"{loggings}\n")
                 file.write(f"{suql}\n")
                 file.write(f"{str(err)}\n")
@@ -1781,18 +1853,19 @@
         finally:
             visitor.drop_tmp_tables()
             return results, column_names, cache
 
 
 if __name__ == "__main__":
     # print(suql_execute(sql, disable_try_catch=True, fts_fields=[("restaurants", "name")] )[0])
+    database = "restaurants"
     with open("sql_free_text_support/test_cases.txt", "r") as fd:
         test_cases = fd.readlines()
     res = []
     for sql in test_cases:
         sql = sql.strip()
-        i_res = suql_execute(sql, disable_try_catch=True)[0]
+        i_res = suql_execute(sql, database, disable_try_catch=True)[0]
         res.append(i_res)
         with open("sql_free_text_support/test_cases_res.txt", "w") as fd:
             for i_res in res:
                 fd.write(str(i_res))
                 fd.write("\n")
```

### Comparing `suql-1.1.4a3/src/suql/utils.py` & `suql-1.1.5/src/suql/utils.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a3/src/suql.egg-info/PKG-INFO` & `suql-1.1.5/src/suql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.1.4a3
+Version: 1.1.5
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.1.4a3 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.5 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `suql-1.1.4a3/src/suql.egg-info/SOURCES.txt` & `suql-1.1.5/src/suql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

