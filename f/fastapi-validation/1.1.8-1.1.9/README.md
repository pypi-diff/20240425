# Comparing `tmp/fastapi_validation-1.1.8.tar.gz` & `tmp/fastapi_validation-1.1.9.tar.gz`

## Comparing `fastapi_validation-1.1.8.tar` & `fastapi_validation-1.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/build_and_publish.sh
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/build_and_test.sh
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/requirements.txt
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/tox.ini
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/fastapi_validation/__init__.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/fastapi_validation/constants/validator_constant.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/fastapi_validation/custom_errors/value_error.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/fastapi_validation/enums/database_type_enum.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/fastapi_validation/helpers/list_init_enum_query_param.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/fastapi_validation/models/projection_model.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/fastapi_validation/types/custom_condition_type.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/fastapi_validation/validators/base.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/fastapi_validation/validators/base_exist_validator.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/fastapi_validation/validators/exist.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/fastapi_validation/validators/field_validator.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/fastapi_validation/validators/model_validator.py
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/fastapi_validation/validators/nosql_exists.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/fastapi_validation/validators/password.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/fastapi_validation/validators/query_list_integer_enum.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/fastapi_validation/validators/sql_exist.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/fastapi_validation/validators/unique.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/tests/application/config/i18n.py
--rw-r--r--   0        0        0     8329 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/tests/application/i18n/validation.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/tests/application/src/main.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/LICENSE
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/README.md
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 fastapi_validation-1.1.8/PKG-INFO
+-rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/build_and_publish.sh
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/build_and_test.sh
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/requirements.txt
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/tox.ini
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/fastapi_validation/__init__.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/fastapi_validation/constants/validator_constant.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/fastapi_validation/custom_errors/value_error.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/fastapi_validation/enums/database_type_enum.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/fastapi_validation/helpers/list_init_enum_query_param.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/fastapi_validation/models/projection_model.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/fastapi_validation/types/custom_condition_type.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/fastapi_validation/validators/base.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/fastapi_validation/validators/base_exist_validator.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/fastapi_validation/validators/exist.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/fastapi_validation/validators/field_validator.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/fastapi_validation/validators/model_validator.py
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/fastapi_validation/validators/nosql_exists.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/fastapi_validation/validators/password.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/fastapi_validation/validators/query_list_integer_enum.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/fastapi_validation/validators/sql_exist.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/fastapi_validation/validators/unique.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/tests/application/config/i18n.py
+-rw-r--r--   0        0        0     8329 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/tests/application/i18n/validation.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/tests/application/src/main.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/LICENSE
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/README.md
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 fastapi_validation-1.1.9/PKG-INFO
```

### Comparing `fastapi_validation-1.1.8/.github/workflows/publish.yaml` & `fastapi_validation-1.1.9/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `fastapi_validation-1.1.8/fastapi_validation/__init__.py` & `fastapi_validation-1.1.9/fastapi_validation/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_validation-1.1.8/fastapi_validation/validators/base_exist_validator.py` & `fastapi_validation-1.1.9/fastapi_validation/validators/base_exist_validator.py`

 * *Files identical despite different names*

### Comparing `fastapi_validation-1.1.8/fastapi_validation/validators/exist.py` & `fastapi_validation-1.1.9/fastapi_validation/validators/exist.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 		custom_error: Optional[Callable] | None = EntityNotFoundException
     ):
         self.table = table
         self.column = column
         self.case_insensitive = case_insensitive
         self.customs = customs
         self.exist_validator = self.get_exist_validator()
-		self.custom_error = custom_error
+        self.custom_error = custom_error
 
     def get_exist_validator(self):
         if GlobalVariable.get('database_type') == DatabaseTypeEnum.SQL:
             return SqlExists(self.table, self.column, self.case_insensitive, self.customs)
 
         return NosqlExists(self.table, self.column, self.case_insensitive, self.customs)
```

### Comparing `fastapi_validation-1.1.8/fastapi_validation/validators/field_validator.py` & `fastapi_validation-1.1.9/fastapi_validation/validators/field_validator.py`

 * *Files identical despite different names*

### Comparing `fastapi_validation-1.1.8/fastapi_validation/validators/nosql_exists.py` & `fastapi_validation-1.1.9/fastapi_validation/validators/nosql_exists.py`

 * *Files identical despite different names*

### Comparing `fastapi_validation-1.1.8/fastapi_validation/validators/password.py` & `fastapi_validation-1.1.9/fastapi_validation/validators/password.py`

 * *Files identical despite different names*

### Comparing `fastapi_validation-1.1.8/fastapi_validation/validators/query_list_integer_enum.py` & `fastapi_validation-1.1.9/fastapi_validation/validators/query_list_integer_enum.py`

 * *Files identical despite different names*

### Comparing `fastapi_validation-1.1.8/fastapi_validation/validators/sql_exist.py` & `fastapi_validation-1.1.9/fastapi_validation/validators/sql_exist.py`

 * *Files identical despite different names*

### Comparing `fastapi_validation-1.1.8/fastapi_validation/validators/unique.py` & `fastapi_validation-1.1.9/fastapi_validation/validators/unique.py`

 * *Files identical despite different names*

### Comparing `fastapi_validation-1.1.8/tests/application/config/i18n.py` & `fastapi_validation-1.1.9/tests/application/config/i18n.py`

 * *Files identical despite different names*

### Comparing `fastapi_validation-1.1.8/tests/application/i18n/validation.json` & `fastapi_validation-1.1.9/tests/application/i18n/validation.json`

 * *Files identical despite different names*

### Comparing `fastapi_validation-1.1.8/tests/application/src/main.py` & `fastapi_validation-1.1.9/tests/application/src/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_validation-1.1.8/.gitignore` & `fastapi_validation-1.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_validation-1.1.8/LICENSE` & `fastapi_validation-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_validation-1.1.8/README.md` & `fastapi_validation-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_validation-1.1.8/pyproject.toml` & `fastapi_validation-1.1.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastapi_validation"
-version = "1.1.8"
+version = "1.1.9"
 authors = [
   { name="Dzung Nguyen", email="dung@megatron-solutions.com" },
   { name="Harry Dang", email="harrydang.tech@gmail.com" },
 ]
 description = "FastAPI Event"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `fastapi_validation-1.1.8/PKG-INFO` & `fastapi_validation-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_validation
-Version: 1.1.8
+Version: 1.1.9
 Summary: FastAPI Event
 Project-URL: Homepage, https://github.com/megatron-global/fastapi-validation
 Project-URL: Bug Tracker, https://github.com/megatron-global/fastapi-validation/issues
 Author-email: Dzung Nguyen <dung@megatron-solutions.com>, Harry Dang <harrydang.tech@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

