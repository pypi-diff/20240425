# Comparing `tmp/fild-0.0.8.tar.gz` & `tmp/fild-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fild-0.0.8.tar", last modified: Mon Oct 16 10:01:51 2023, max compression
+gzip compressed data, was "fild-0.0.9.tar", last modified: Thu Apr 25 19:06:06 2024, max compression
```

## Comparing `fild-0.0.8.tar` & `fild-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 10:01:51.542244 fild-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-10-16 10:01:36.000000 fild-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2023-10-16 10:01:51.542244 fild-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2023-10-16 10:01:36.000000 fild-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-10-16 10:01:36.000000 fild-0.0.8/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      699 2023-10-16 10:01:51.542244 fild-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 10:01:51.534243 fild-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 10:01:51.534243 fild-0.0.8/src/fild/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 10:01:36.000000 fild-0.0.8/src/fild/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 10:01:51.538243 fild-0.0.8/src/fild/process/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 10:01:36.000000 fild-0.0.8/src/fild/process/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2568 2023-10-16 10:01:36.000000 fild-0.0.8/src/fild/process/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11304 2023-10-16 10:01:36.000000 fild-0.0.8/src/fild/process/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 10:01:51.542244 fild-0.0.8/src/fild/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2023-10-16 10:01:36.000000 fild-0.0.8/src/fild/sdk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2610 2023-10-16 10:01:36.000000 fild-0.0.8/src/fild/sdk/array.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1206 2023-10-16 10:01:36.000000 fild-0.0.8/src/fild/sdk/dates.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5247 2023-10-16 10:01:36.000000 fild-0.0.8/src/fild/sdk/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2023-10-16 10:01:36.000000 fild-0.0.8/src/fild/sdk/fakeable.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2205 2023-10-16 10:01:36.000000 fild-0.0.8/src/fild/sdk/field.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5118 2023-10-16 10:01:36.000000 fild-0.0.8/src/fild/sdk/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 10:01:51.538243 fild-0.0.8/src/fild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2023-10-16 10:01:51.000000 fild-0.0.8/src/fild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      474 2023-10-16 10:01:51.000000 fild-0.0.8/src/fild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-16 10:01:51.000000 fild-0.0.8/src/fild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-10-16 10:01:51.000000 fild-0.0.8/src/fild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-16 10:01:51.000000 fild-0.0.8/src/fild.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:06:06.733978 fild-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-25 19:05:59.000000 fild-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-25 19:06:06.733978 fild-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-25 19:05:59.000000 fild-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-25 19:05:59.000000 fild-0.0.9/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      699 2024-04-25 19:06:06.733978 fild-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:06:06.729978 fild-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:06:06.729978 fild-0.0.9/src/fild/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:05:59.000000 fild-0.0.9/src/fild/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:06:06.733978 fild-0.0.9/src/fild/process/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:05:59.000000 fild-0.0.9/src/fild/process/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2966 2024-04-25 19:05:59.000000 fild-0.0.9/src/fild/process/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11233 2024-04-25 19:05:59.000000 fild-0.0.9/src/fild/process/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:06:06.733978 fild-0.0.9/src/fild/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-25 19:05:59.000000 fild-0.0.9/src/fild/sdk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3027 2024-04-25 19:05:59.000000 fild-0.0.9/src/fild/sdk/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-25 19:05:59.000000 fild-0.0.9/src/fild/sdk/base_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1206 2024-04-25 19:05:59.000000 fild-0.0.9/src/fild/sdk/dates.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5247 2024-04-25 19:05:59.000000 fild-0.0.9/src/fild/sdk/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-04-25 19:05:59.000000 fild-0.0.9/src/fild/sdk/fakeable.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2205 2024-04-25 19:05:59.000000 fild-0.0.9/src/fild/sdk/field.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4296 2024-04-25 19:05:59.000000 fild-0.0.9/src/fild/sdk/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:06:06.733978 fild-0.0.9/src/fild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-25 19:06:06.000000 fild-0.0.9/src/fild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-25 19:06:06.000000 fild-0.0.9/src/fild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:06:06.000000 fild-0.0.9/src/fild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-25 19:06:06.000000 fild-0.0.9/src/fild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 19:06:06.000000 fild-0.0.9/src/fild.egg-info/top_level.txt
```

### Comparing `fild-0.0.8/LICENSE` & `fild-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fild-0.0.8/PKG-INFO` & `fild-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fild
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library to describe contracts and generate data
 Home-page: https://github.com/elenakulgavaya/fild
 Author: Elena Kulgavaya
 Author-email: elena.kulgavaya@gmail.com
 Project-URL: Bug Tracker, https://github.com/elenakulgavaya/fild/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fild-0.0.8/README.md` & `fild-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fild-0.0.8/setup.cfg` & `fild-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fild
-version = 0.0.8
+version = 0.0.9
 author = Elena Kulgavaya
 author_email = elena.kulgavaya@gmail.com
 description = Library to describe contracts and generate data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/elenakulgavaya/fild
 project_urls =
```

### Comparing `fild-0.0.8/src/fild/process/dictionary.py` & `fild-0.0.9/src/fild/process/dictionary.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,13 +363,7 @@
 
     elif isinstance(initial, dict):
         for key, value in initial.items():
             if expected:
                 initial[key] = normalize(value, expected.get(key), keys=keys)
 
     return initial
-
-
-if __name__ == '__main__':
-    import doctest
-
-    doctest.testmod()
```

### Comparing `fild-0.0.8/src/fild/sdk/array.py` & `fild-0.0.9/src/fild/sdk/array.py`

 * *Files 7% similar despite different names*

```diff
@@ -79,14 +79,28 @@
 
             return self
 
         return super().with_values(values)
 
 
 class Set(Array):
+    def with_values(self, values):
+        if isinstance(values, (set, list)):
+            _values = set()
+
+            for value in values:
+                if not isinstance(value, self.field.__class__):
+                    value = self.field(is_full=False).with_values(value)
+                _values.add(value)
+            self._value = _values
+
+            return self
+
+        return super().with_values(values)
+
     @property
     def value(self):
         if self._value is None:
             return None
 
         return {field.value for field in self._value}
```

### Comparing `fild-0.0.8/src/fild/sdk/dates.py` & `fild-0.0.9/src/fild/sdk/dates.py`

 * *Files identical despite different names*

### Comparing `fild-0.0.8/src/fild/sdk/dictionary.py` & `fild-0.0.9/src/fild/sdk/dictionary.py`

 * *Files identical despite different names*

### Comparing `fild-0.0.8/src/fild/sdk/fakeable.py` & `fild-0.0.9/src/fild/sdk/fakeable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import decimal
 import random
 
 from faker import Faker
 
+from fild.sdk.base_enum import BaseEnum
 
-class Fakeable:
+
+class Fakeable(BaseEnum):
     Address = 'address'
     AmPm = 'am_pm'
     AndroidToken = 'android_platform_token'
     BankCountry = 'bank_country'
     Boolean = 'boolean'
     BuildingNumber = 'building_number'
     City = 'city'
```

### Comparing `fild-0.0.8/src/fild/sdk/field.py` & `fild-0.0.9/src/fild/sdk/field.py`

 * *Files identical despite different names*

### Comparing `fild-0.0.8/src/fild/sdk/types.py` & `fild-0.0.9/src/fild/sdk/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import decimal
 import random
 
 
 from fild.sdk import fakeable, dates
+from fild.sdk.base_enum import BaseEnum
 from fild.sdk.field import Field
 from fild.process import dictionary
 
 
 class Bool(Field):
     def generate_value(self):
         return fakeable.FAKER.boolean()
@@ -98,54 +99,24 @@
         return fakeable.fake_string_attr(
             self.fake_as or self.name,
             min_len=self.min_len,
             max_len=self.max_len
         )
 
 
-class Enum(Field):
+class Enum(Field, BaseEnum):
     def __init__(self, name=None, required=True, allow_none=False,
                  default=None, exclude=None):
         self.save_kwargs(locals())
         self.exclude = exclude or ()
         super().__init__(
             name=name, required=required, allow_none=allow_none,
             default=default
         )
 
-    @classmethod
-    def _attr_values_as_list(cls):
-        result = []
-
-        for attr_name in dir(cls):
-            if not attr_name.startswith('_'):
-                attr_value = getattr(cls, attr_name)
-
-                if (not callable(attr_value) and
-                        not isinstance(attr_value, property)):
-                    result.append(attr_value)
-
-        return result
-
-    @classmethod
-    def to_list(cls, exclude=()):
-        """
-        :param exclude: list of values to be excluded from result; if
-          not existent value passed, ValueError exception will be thrown
-        :return: list of all fields of class A(Enum) and its parents
-        """
-        result = cls._attr_values_as_list()
-        if type(exclude) not in (list, tuple):
-            exclude = (exclude,)
-
-        for item in exclude:
-            result.remove(item)
-
-        return result
-
     def generate_value(self):
         return random.choice(self.__class__.to_list(
             exclude=self.exclude
         ))
 
 
 class Raw(String):
@@ -154,15 +125,15 @@
         self.overrided_values = False
         self._value = None
         super().__init__(
             name=name, required=required, allow_none=allow_none
         )
 
     def generate_value(self):
-        return fakeable.FAKER.pydict(10, True, str)
+        return fakeable.FAKER.pydict(10, True, value_types=(str,))
 
     def with_values(self, values):
         if self.overrided_values and isinstance(self._value, dict):
             self._value = dictionary.merge_with_updates(self._value, values)
         else:
             self._value = values
```

### Comparing `fild-0.0.8/src/fild.egg-info/PKG-INFO` & `fild-0.0.9/src/fild.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fild
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library to describe contracts and generate data
 Home-page: https://github.com/elenakulgavaya/fild
 Author: Elena Kulgavaya
 Author-email: elena.kulgavaya@gmail.com
 Project-URL: Bug Tracker, https://github.com/elenakulgavaya/fild/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

