# Comparing `tmp/django_guid-3.4.0.tar.gz` & `tmp/django_guid-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_guid-3.4.0.tar", max compression
+gzip compressed data, was "django_guid-3.5.0.tar", max compression
```

## Comparing `django_guid-3.4.0.tar` & `django_guid-3.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     5976 2024-01-03 14:12:51.627221 django_guid-3.4.0/CHANGELOG.rst
--rw-r--r--   0        0        0     1107 2024-01-03 14:12:51.627221 django_guid-3.4.0/LICENSE
--rw-r--r--   0        0        0      250 2024-01-03 14:12:51.631221 django_guid-3.4.0/django_guid/__init__.py
--rw-r--r--   0        0        0      690 2024-01-03 14:12:51.631221 django_guid-3.4.0/django_guid/api.py
--rw-r--r--   0        0        0      347 2024-01-03 14:12:51.631221 django_guid-3.4.0/django_guid/apps.py
--rw-r--r--   0        0        0     5075 2024-01-03 14:12:51.631221 django_guid-3.4.0/django_guid/config.py
--rw-r--r--   0        0        0       88 2024-01-03 14:12:51.631221 django_guid-3.4.0/django_guid/context.py
--rw-r--r--   0        0        0      247 2024-01-03 14:12:51.631221 django_guid-3.4.0/django_guid/integrations/__init__.py
--rw-r--r--   0        0        0      916 2024-01-03 14:12:51.631221 django_guid-3.4.0/django_guid/integrations/base.py
--rw-r--r--   0        0        0      107 2024-01-03 14:12:51.631221 django_guid-3.4.0/django_guid/integrations/celery/__init__.py
--rw-r--r--   0        0        0     1598 2024-01-03 14:12:51.631221 django_guid-3.4.0/django_guid/integrations/celery/config.py
--rw-r--r--   0        0        0      178 2024-01-03 14:12:51.631221 django_guid-3.4.0/django_guid/integrations/celery/context.py
--rw-r--r--   0        0        0     2119 2024-01-03 14:12:51.631221 django_guid-3.4.0/django_guid/integrations/celery/integration.py
--rw-r--r--   0        0        0      913 2024-01-03 14:12:51.631221 django_guid-3.4.0/django_guid/integrations/celery/log_filters.py
--rw-r--r--   0        0        0      370 2024-01-03 14:12:51.631221 django_guid-3.4.0/django_guid/integrations/celery/logging.py
--rw-r--r--   0        0        0     3267 2024-01-03 14:12:51.631221 django_guid-3.4.0/django_guid/integrations/celery/signals.py
--rw-r--r--   0        0        0     1279 2024-01-03 14:12:51.631221 django_guid-3.4.0/django_guid/integrations/sentry.py
--rw-r--r--   0        0        0      630 2024-01-03 14:12:51.631221 django_guid-3.4.0/django_guid/log_filters.py
--rw-r--r--   0        0        0     3292 2024-01-03 14:12:51.631221 django_guid-3.4.0/django_guid/middleware.py
--rw-r--r--   0        0        0        0 2024-01-03 14:12:51.631221 django_guid-3.4.0/django_guid/py.typed
--rw-r--r--   0        0        0     1020 2024-01-03 14:12:51.631221 django_guid-3.4.0/django_guid/signals.py
--rw-r--r--   0        0        0     2970 2024-01-03 14:12:51.631221 django_guid-3.4.0/django_guid/utils.py
--rw-r--r--   0        0        0     8283 2024-01-03 14:12:51.631221 django_guid-3.4.0/docs/README_PYPI.rst
--rw-r--r--   0        0        0     3249 2024-01-03 14:12:51.635221 django_guid-3.4.0/pyproject.toml
--rw-r--r--   0        0        0    10557 1970-01-01 00:00:00.000000 django_guid-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0     5976 2024-04-25 15:48:43.270417 django_guid-3.5.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     1107 2024-04-25 15:48:43.270417 django_guid-3.5.0/LICENSE
+-rw-r--r--   0        0        0      250 2024-04-25 15:48:43.274417 django_guid-3.5.0/django_guid/__init__.py
+-rw-r--r--   0        0        0      690 2024-04-25 15:48:43.274417 django_guid-3.5.0/django_guid/api.py
+-rw-r--r--   0        0        0      347 2024-04-25 15:48:43.274417 django_guid-3.5.0/django_guid/apps.py
+-rw-r--r--   0        0        0     5075 2024-04-25 15:48:43.274417 django_guid-3.5.0/django_guid/config.py
+-rw-r--r--   0        0        0       88 2024-04-25 15:48:43.274417 django_guid-3.5.0/django_guid/context.py
+-rw-r--r--   0        0        0      247 2024-04-25 15:48:43.274417 django_guid-3.5.0/django_guid/integrations/__init__.py
+-rw-r--r--   0        0        0      916 2024-04-25 15:48:43.274417 django_guid-3.5.0/django_guid/integrations/base.py
+-rw-r--r--   0        0        0      107 2024-04-25 15:48:43.274417 django_guid-3.5.0/django_guid/integrations/celery/__init__.py
+-rw-r--r--   0        0        0     1598 2024-04-25 15:48:43.274417 django_guid-3.5.0/django_guid/integrations/celery/config.py
+-rw-r--r--   0        0        0      178 2024-04-25 15:48:43.274417 django_guid-3.5.0/django_guid/integrations/celery/context.py
+-rw-r--r--   0        0        0     2119 2024-04-25 15:48:43.274417 django_guid-3.5.0/django_guid/integrations/celery/integration.py
+-rw-r--r--   0        0        0      913 2024-04-25 15:48:43.274417 django_guid-3.5.0/django_guid/integrations/celery/log_filters.py
+-rw-r--r--   0        0        0      370 2024-04-25 15:48:43.274417 django_guid-3.5.0/django_guid/integrations/celery/logging.py
+-rw-r--r--   0        0        0     3267 2024-04-25 15:48:43.274417 django_guid-3.5.0/django_guid/integrations/celery/signals.py
+-rw-r--r--   0        0        0     1279 2024-04-25 15:48:43.274417 django_guid-3.5.0/django_guid/integrations/sentry.py
+-rw-r--r--   0        0        0      697 2024-04-25 15:48:43.274417 django_guid-3.5.0/django_guid/log_filters.py
+-rw-r--r--   0        0        0     3292 2024-04-25 15:48:43.274417 django_guid-3.5.0/django_guid/middleware.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:48:43.274417 django_guid-3.5.0/django_guid/py.typed
+-rw-r--r--   0        0        0     1020 2024-04-25 15:48:43.274417 django_guid-3.5.0/django_guid/signals.py
+-rw-r--r--   0        0        0     2970 2024-04-25 15:48:43.274417 django_guid-3.5.0/django_guid/utils.py
+-rw-r--r--   0        0        0     8283 2024-04-25 15:48:43.274417 django_guid-3.5.0/docs/README_PYPI.rst
+-rw-r--r--   0        0        0     3250 2024-04-25 15:48:43.278417 django_guid-3.5.0/pyproject.toml
+-rw-r--r--   0        0        0    10507 1970-01-01 00:00:00.000000 django_guid-3.5.0/PKG-INFO
```

### Comparing `django_guid-3.4.0/CHANGELOG.rst` & `django_guid-3.5.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `django_guid-3.4.0/LICENSE` & `django_guid-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_guid-3.4.0/django_guid/api.py` & `django_guid-3.5.0/django_guid/api.py`

 * *Files identical despite different names*

### Comparing `django_guid-3.4.0/django_guid/config.py` & `django_guid-3.5.0/django_guid/config.py`

 * *Files identical despite different names*

### Comparing `django_guid-3.4.0/django_guid/integrations/base.py` & `django_guid-3.5.0/django_guid/integrations/base.py`

 * *Files identical despite different names*

### Comparing `django_guid-3.4.0/django_guid/integrations/celery/config.py` & `django_guid-3.5.0/django_guid/integrations/celery/config.py`

 * *Files identical despite different names*

### Comparing `django_guid-3.4.0/django_guid/integrations/celery/integration.py` & `django_guid-3.5.0/django_guid/integrations/celery/integration.py`

 * *Files identical despite different names*

### Comparing `django_guid-3.4.0/django_guid/integrations/celery/log_filters.py` & `django_guid-3.5.0/django_guid/integrations/celery/log_filters.py`

 * *Files identical despite different names*

### Comparing `django_guid-3.4.0/django_guid/integrations/celery/signals.py` & `django_guid-3.5.0/django_guid/integrations/celery/signals.py`

 * *Files identical despite different names*

### Comparing `django_guid-3.4.0/django_guid/integrations/sentry.py` & `django_guid-3.5.0/django_guid/integrations/sentry.py`

 * *Files identical despite different names*

### Comparing `django_guid-3.4.0/django_guid/log_filters.py` & `django_guid-3.5.0/django_guid/log_filters.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 from django_guid.middleware import guid
 
 if TYPE_CHECKING:
     from logging import LogRecord
 
 
 class CorrelationId(Filter):
+    def __init__(self, correlation_id_field: str = 'correlation_id') -> None:
+        super().__init__()
+        self.correlation_id_field = correlation_id_field
+
     def filter(self, record: 'LogRecord') -> bool:
         """
-        Determines that the specified record is to be logged.
-
-        From the docs:
-                Is the specified record to be logged? Returns 0 for no, nonzero for
-                yes. If deemed appropriate, the record may be modified in-place.
+        Add the correlation ID to the log record.
         :param record: Log record
+        :param correlation_id_field: record field on which the correlation id is set
         :return: True
         """
-        record.correlation_id = guid.get()
+        setattr(record, self.correlation_id_field, guid.get())
         return True
```

### Comparing `django_guid-3.4.0/django_guid/middleware.py` & `django_guid-3.5.0/django_guid/middleware.py`

 * *Files identical despite different names*

### Comparing `django_guid-3.4.0/django_guid/signals.py` & `django_guid-3.5.0/django_guid/signals.py`

 * *Files identical despite different names*

### Comparing `django_guid-3.4.0/django_guid/utils.py` & `django_guid-3.5.0/django_guid/utils.py`

 * *Files identical despite different names*

### Comparing `django_guid-3.4.0/docs/README_PYPI.rst` & `django_guid-3.5.0/docs/README_PYPI.rst`

 * *Files identical despite different names*

### Comparing `django_guid-3.4.0/pyproject.toml` & `django_guid-3.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-guid"
-version = "3.4.0"  # Remember to also change __init__.py version
+version = "3.5.0"  # Remember to also change __init__.py version
 description = "Middleware that enables single request-response cycle tracing by injecting a unique ID into project logs"
 authors = ["Jonas Krüger Svensson <jonas-ks@hotmail.com>"]
 maintainers = ["Sondre Lillebø Gundersen <sondrelg@live.no>"]
 license = "MIT"
 readme = "docs/README_PYPI.rst"
 homepage = "https://github.com/snok/django-guid"
 repository = "https://github.com/snok/django-guid"
@@ -13,28 +13,28 @@
     'asgi', 'async', 'async support', 'correlation', 'correlation-id', 'django', 'guid', 'log id', 'logging',
     'logging id', 'middleware', 'request', 'request id', 'request-id', 'uuid', 'web', 'sentry', 'celery'
 ]
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Web Environment',
     'Framework :: Django',
-    'Framework :: Django :: 3.0',
-    'Framework :: Django :: 3.1',
     'Framework :: Django :: 3.2',
     'Framework :: Django :: 4.0',
     'Framework :: Django :: 4.1',
+    'Framework :: Django :: 4.2',
+    'Framework :: Django :: 5.0',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: BSD License',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
     'Topic :: Internet :: WWW/HTTP',
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     'Topic :: Internet :: WWW/HTTP :: WSGI',
     'Topic :: Software Development',
     'Topic :: Software Development :: Libraries',
     'Topic :: Software Development :: Libraries :: Application Frameworks',
     'Topic :: Software Development :: Libraries :: Python Modules',
```

### Comparing `django_guid-3.4.0/PKG-INFO` & `django_guid-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: django-guid
-Version: 3.4.0
+Version: 3.5.0
 Summary: Middleware that enables single request-response cycle tracing by injecting a unique ID into project logs
 Home-page: https://github.com/snok/django-guid
 License: MIT
 Keywords: asgi,async,async support,correlation,correlation-id,django,guid,log id,logging,logging id,middleware,request,request id,request-id,uuid,web,sentry,celery
 Author: Jonas Krüger Svensson
 Author-email: jonas-ks@hotmail.com
 Maintainer: Sondre Lillebø Gundersen
 Maintainer-email: sondrelg@live.no
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

