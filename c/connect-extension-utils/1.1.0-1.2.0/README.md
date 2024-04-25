# Comparing `tmp/connect_extension_utils-1.1.0.tar.gz` & `tmp/connect_extension_utils-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connect_extension_utils-1.1.0.tar", max compression
+gzip compressed data, was "connect_extension_utils-1.2.0.tar", max compression
```

## Comparing `connect_extension_utils-1.1.0.tar` & `connect_extension_utils-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11344 2024-02-27 11:19:47.295116 connect_extension_utils-1.1.0/LICENSE
--rw-r--r--   0        0        0      301 2024-02-27 11:19:47.295116 connect_extension_utils-1.1.0/README.md
--rw-r--r--   0        0        0       86 2024-02-27 11:19:47.295116 connect_extension_utils-1.1.0/connect_extension_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-02-27 11:19:47.295116 connect_extension_utils-1.1.0/connect_extension_utils/api/__init__.py
--rw-r--r--   0        0        0     2894 2024-02-27 11:19:47.295116 connect_extension_utils-1.1.0/connect_extension_utils/api/errors.py
--rw-r--r--   0        0        0     1122 2024-02-27 11:19:47.295116 connect_extension_utils-1.1.0/connect_extension_utils/api/pagination.py
--rw-r--r--   0        0        0     1494 2024-02-27 11:19:47.295116 connect_extension_utils-1.1.0/connect_extension_utils/api/schemas.py
--rw-r--r--   0        0        0     1235 2024-02-27 11:19:47.295116 connect_extension_utils-1.1.0/connect_extension_utils/api/views.py
--rw-r--r--   0        0        0        0 2024-02-27 11:19:47.295116 connect_extension_utils-1.1.0/connect_extension_utils/connect_services/__init__.py
--rw-r--r--   0        0        0     1305 2024-02-27 11:19:47.295116 connect_extension_utils-1.1.0/connect_extension_utils/connect_services/base.py
--rw-r--r--   0        0        0        0 2024-02-27 11:19:47.295116 connect_extension_utils-1.1.0/connect_extension_utils/db/__init__.py
--rw-r--r--   0        0        0     6034 2024-02-27 11:19:47.295116 connect_extension_utils-1.1.0/connect_extension_utils/db/models.py
--rw-r--r--   0        0        0        0 2024-02-27 11:19:47.295116 connect_extension_utils-1.1.0/connect_extension_utils/testing/__init__.py
--rw-r--r--   0        0        0      190 2024-02-27 11:19:47.295116 connect_extension_utils-1.1.0/connect_extension_utils/testing/database.py
--rw-r--r--   0        0        0     2662 2024-02-27 11:19:47.295116 connect_extension_utils-1.1.0/connect_extension_utils/testing/factories.py
--rw-r--r--   0        0        0     1728 2024-02-27 11:19:47.295116 connect_extension_utils-1.1.0/connect_extension_utils/testing/fixtures.py
--rw-r--r--   0        0        0     2494 2024-02-27 11:20:11.303182 connect_extension_utils-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1311 1970-01-01 00:00:00.000000 connect_extension_utils-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11344 2024-04-25 14:34:38.207959 connect_extension_utils-1.2.0/LICENSE
+-rw-r--r--   0        0        0      301 2024-04-25 14:34:38.207959 connect_extension_utils-1.2.0/README.md
+-rw-r--r--   0        0        0       86 2024-04-25 14:34:38.207959 connect_extension_utils-1.2.0/connect_extension_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 14:34:38.207959 connect_extension_utils-1.2.0/connect_extension_utils/api/__init__.py
+-rw-r--r--   0        0        0     2894 2024-04-25 14:34:38.207959 connect_extension_utils-1.2.0/connect_extension_utils/api/errors.py
+-rw-r--r--   0        0        0     1122 2024-04-25 14:34:38.207959 connect_extension_utils-1.2.0/connect_extension_utils/api/pagination.py
+-rw-r--r--   0        0        0     1494 2024-04-25 14:34:38.207959 connect_extension_utils-1.2.0/connect_extension_utils/api/schemas.py
+-rw-r--r--   0        0        0     1235 2024-04-25 14:34:38.211959 connect_extension_utils-1.2.0/connect_extension_utils/api/views.py
+-rw-r--r--   0        0        0        0 2024-04-25 14:34:38.211959 connect_extension_utils-1.2.0/connect_extension_utils/connect_services/__init__.py
+-rw-r--r--   0        0        0     1305 2024-04-25 14:34:38.211959 connect_extension_utils-1.2.0/connect_extension_utils/connect_services/base.py
+-rw-r--r--   0        0        0        0 2024-04-25 14:34:38.211959 connect_extension_utils-1.2.0/connect_extension_utils/db/__init__.py
+-rw-r--r--   0        0        0     6039 2024-04-25 14:34:38.211959 connect_extension_utils-1.2.0/connect_extension_utils/db/models.py
+-rw-r--r--   0        0        0        0 2024-04-25 14:34:38.211959 connect_extension_utils-1.2.0/connect_extension_utils/testing/__init__.py
+-rw-r--r--   0        0        0      190 2024-04-25 14:34:38.211959 connect_extension_utils-1.2.0/connect_extension_utils/testing/database.py
+-rw-r--r--   0        0        0     2763 2024-04-25 14:34:38.211959 connect_extension_utils-1.2.0/connect_extension_utils/testing/factories.py
+-rw-r--r--   0        0        0     1728 2024-04-25 14:34:38.211959 connect_extension_utils-1.2.0/connect_extension_utils/testing/fixtures.py
+-rw-r--r--   0        0        0     2494 2024-04-25 14:35:01.879979 connect_extension_utils-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1311 1970-01-01 00:00:00.000000 connect_extension_utils-1.2.0/PKG-INFO
```

### Comparing `connect_extension_utils-1.1.0/LICENSE` & `connect_extension_utils-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connect_extension_utils-1.1.0/connect_extension_utils/api/errors.py` & `connect_extension_utils-1.2.0/connect_extension_utils/api/errors.py`

 * *Files identical despite different names*

### Comparing `connect_extension_utils-1.1.0/connect_extension_utils/api/pagination.py` & `connect_extension_utils-1.2.0/connect_extension_utils/api/pagination.py`

 * *Files identical despite different names*

### Comparing `connect_extension_utils-1.1.0/connect_extension_utils/api/schemas.py` & `connect_extension_utils-1.2.0/connect_extension_utils/api/schemas.py`

 * *Files identical despite different names*

### Comparing `connect_extension_utils-1.1.0/connect_extension_utils/api/views.py` & `connect_extension_utils-1.2.0/connect_extension_utils/api/views.py`

 * *Files identical despite different names*

### Comparing `connect_extension_utils-1.1.0/connect_extension_utils/connect_services/base.py` & `connect_extension_utils-1.2.0/connect_extension_utils/connect_services/base.py`

 * *Files identical despite different names*

### Comparing `connect_extension_utils-1.1.0/connect_extension_utils/db/models.py` & `connect_extension_utils-1.2.0/connect_extension_utils/db/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -91,65 +91,63 @@
         instances = self._set_verbose_all(instances)
         return self.add_all(instances)
 
     def add_next_with_verbose(self, instance, related_id_field):
         instance_class = instance.__class__
         new_suffix = 0
         related_id_value = getattr(instance, related_id_field)
-        if self.query(
-            self.query(instance_class)
-            .filter(instance_class.__dict__[related_id_field] == related_id_value)
-            .exists(),
-        ).scalar():
-            last_obj = (
-                self.query(instance_class)
-                .order_by(
-                    instance_class.id.desc(),
-                )
-                .first()
-            )
+        last_obj = self._get_last_obj_for_next_verbose(
+            instance_class,
+            related_id_field,
+            related_id_value,
+        )
+        if last_obj:
             _instance_id, suffix = last_obj.id.rsplit("-", 1)
             new_suffix = int(suffix) + 1
         else:
             id_body = related_id_value.split("-", 1)[-1]
             _instance_id = f"{instance_class.PREFIX}-{id_body}"
 
         instance.id = "{0}-{1}".format(_instance_id, "{0:03d}".format(new_suffix))
         return self.add(instance)
 
     def add_all_with_next_verbose(self, instances, related_id_field):
         first_item = instances[0]
         instance_class = first_item.__class__
         new_suffix = 0
         related_id_value = getattr(first_item, related_id_field)
-
-        if self.query(
-            self.query(instance_class)
-            .filter(instance_class.__dict__[related_id_field] == related_id_value)
-            .exists(),
-        ).scalar():
-            last_obj = (
-                self.query(instance_class)
-                .order_by(
-                    instance_class.id.desc(),
-                )
-                .first()
-            )
+        last_obj = self._get_last_obj_for_next_verbose(
+            instance_class,
+            related_id_field,
+            related_id_value,
+        )
+        if last_obj:
             _instance_id, suffix = last_obj.id.rsplit("-", 1)
             new_suffix = int(suffix) + 1
         else:
             id_body = related_id_value.split("-", 1)[-1]
             _instance_id = f"{instance_class.PREFIX}-{id_body}"
 
         for instance in instances:
             instance.id = "{0}-{1}".format(_instance_id, "{0:03d}".format(new_suffix))
             new_suffix += 1
 
         return self.add_all(instances)
 
+    def _get_last_obj_for_next_verbose(self, model_class, related_id_field, related_id_value):
+        base_qs = self.query(model_class).filter(
+            model_class.__dict__[related_id_field] == related_id_value,
+        )
+        last_obj = None
+        if self.query(base_qs.exists()).scalar():
+            last_obj = base_qs.order_by(
+                model_class.id.desc(),
+            ).first()
+        return last_obj
+
 
 SessionLocal = sessionmaker(autocommit=False, autoflush=False, class_=VerboseBaseSession)
 Model = declarative_base()
 
 
 def get_engine(config: dict = Depends(get_config)):
     global _ENGINE
```

### Comparing `connect_extension_utils-1.1.0/connect_extension_utils/testing/factories.py` & `connect_extension_utils-1.2.0/connect_extension_utils/testing/factories.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,40 +34,40 @@
         """Factory configuration."""
 
         sqlalchemy_session = Session
         sqlalchemy_session_persistence = 'commit'
 
     @classmethod
     def _save(cls, model_class, session, args, kwargs):
-        obj = model_class(*args, **kwargs)
+        save_method = None
         if cls._meta._is_transactional:
+            obj = model_class(*args, **kwargs)
             kwargs['id'] = cls.add_next_with_verbose(
                 model_class,
                 session,
                 obj,
                 cls._meta._related_id_field,
             )
-        return super()._save(model_class, session, args, kwargs)
+            save_method = factory.alchemy.SQLAlchemyModelFactory.__dict__['_save']
+        cls.save_method = save_method or super()._save
+        return cls.save_method(model_class, session, args, kwargs)
 
     @classmethod
     def add_next_with_verbose(cls, model_class, session, obj, related_id_field):
         new_suffix = 0
         related_id_value = getattr(obj, related_id_field)
+        base_qs = session.query(model_class).filter(
+            model_class.__dict__[related_id_field] == related_id_value,
+        )
         if session.query(
-            session.query(model_class)
-            .filter(model_class.__dict__[related_id_field] == related_id_value)
-            .exists(),
+            base_qs.exists(),
         ).scalar():
-            last_obj = (
-                session.query(model_class)
-                .order_by(
-                    model_class.id.desc(),
-                )
-                .first()
-            )
+            last_obj = base_qs.order_by(
+                model_class.id.desc(),
+            ).first()
             _instance_id, suffix = last_obj.id.rsplit("-", 1)
             new_suffix = int(suffix) + 1
         else:
             id_body = related_id_value.split("-", 1)[-1]
             _instance_id = f"{model_class.PREFIX}-{id_body}"
 
         new_id = "{0}-{1}".format(_instance_id, "{0:03d}".format(new_suffix))
```

### Comparing `connect_extension_utils-1.1.0/connect_extension_utils/testing/fixtures.py` & `connect_extension_utils-1.2.0/connect_extension_utils/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `connect_extension_utils-1.1.0/pyproject.toml` & `connect_extension_utils-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "connect-extension-utils"
-version = "v1.1.0"
+version = "v1.2.0"
 description = "This repository extend EaaS's out-of-box functionality providing a set of common utilities that can be reused between different extensions."
 authors = ["Imgram Migro"]
 license = "Apache Software License 2.0"
 packages = [
     { include = "connect_extension_utils" }
 ]
 readme = "./README.md"
```

### Comparing `connect_extension_utils-1.1.0/PKG-INFO` & `connect_extension_utils-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connect-extension-utils
-Version: 1.1.0
+Version: 1.2.0
 Summary: This repository extend EaaS's out-of-box functionality providing a set of common utilities that can be reused between different extensions.
 Home-page: https://github.com/cloudblue/connect-extension-utils
 License: Apache Software License 2.0
 Author: Imgram Migro
 Requires-Python: >=3.8,<4
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

