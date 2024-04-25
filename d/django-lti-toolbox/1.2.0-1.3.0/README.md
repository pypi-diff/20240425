# Comparing `tmp/django-lti-toolbox-1.2.0.tar.gz` & `tmp/django-lti-toolbox-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-lti-toolbox-1.2.0.tar", last modified: Wed Sep 13 16:46:29 2023, max compression
+gzip compressed data, was "django-lti-toolbox-1.3.0.tar", last modified: Thu Apr 25 14:51:22 2024, max compression
```

## Comparing `django-lti-toolbox-1.2.0.tar` & `django-lti-toolbox-1.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-09-13 16:46:29.013951 django-lti-toolbox-1.2.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1078 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2229 2023-09-13 16:46:29.013951 django-lti-toolbox-1.2.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1470 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1782 2023-09-13 16:46:29.013951 django-lti-toolbox-1.2.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)       85 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-09-13 16:46:29.009950 django-lti-toolbox-1.2.0/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-09-13 16:46:29.009950 django-lti-toolbox-1.2.0/src/django_lti_toolbox.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2229 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/src/django_lti_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      775 2023-09-13 16:46:29.000000 django-lti-toolbox-1.2.0/src/django_lti_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/src/django_lti_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      374 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/src/django_lti_toolbox.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/src/django_lti_toolbox.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/src/django_lti_toolbox.egg-info/zip-safe
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-09-13 16:46:29.013951 django-lti-toolbox-1.2.0/src/lti_toolbox/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      236 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/src/lti_toolbox/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      612 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/src/lti_toolbox/admin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      278 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/src/lti_toolbox/apps.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2608 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/src/lti_toolbox/backend.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1110 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/src/lti_toolbox/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      839 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/src/lti_toolbox/factories.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7094 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/src/lti_toolbox/launch_params.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6412 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/src/lti_toolbox/lti.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-09-13 16:46:29.013951 django-lti-toolbox-1.2.0/src/lti_toolbox/migrations/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3388 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/src/lti_toolbox/migrations/0001_initial.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      550 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/src/lti_toolbox/migrations/0002_lticonsumer_url.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/src/lti_toolbox/migrations/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4001 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/src/lti_toolbox/models.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1536 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/src/lti_toolbox/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6837 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/src/lti_toolbox/validator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3614 2023-09-13 16:46:28.000000 django-lti-toolbox-1.2.0/src/lti_toolbox/views.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-25 14:51:22.200917 django-lti-toolbox-1.3.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1078 2024-04-25 14:51:21.000000 django-lti-toolbox-1.3.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2024-04-25 14:51:21.000000 django-lti-toolbox-1.3.0/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2229 2024-04-25 14:51:22.200917 django-lti-toolbox-1.3.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1470 2024-04-25 14:51:21.000000 django-lti-toolbox-1.3.0/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1782 2024-04-25 14:51:22.200917 django-lti-toolbox-1.3.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       85 2024-04-25 14:51:21.000000 django-lti-toolbox-1.3.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-25 14:51:22.196917 django-lti-toolbox-1.3.0/src/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-25 14:51:22.200917 django-lti-toolbox-1.3.0/src/django_lti_toolbox.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2229 2024-04-25 14:51:22.000000 django-lti-toolbox-1.3.0/src/django_lti_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      775 2024-04-25 14:51:22.000000 django-lti-toolbox-1.3.0/src/django_lti_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-04-25 14:51:22.000000 django-lti-toolbox-1.3.0/src/django_lti_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      374 2024-04-25 14:51:22.000000 django-lti-toolbox-1.3.0/src/django_lti_toolbox.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2024-04-25 14:51:22.000000 django-lti-toolbox-1.3.0/src/django_lti_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-04-25 14:51:22.000000 django-lti-toolbox-1.3.0/src/django_lti_toolbox.egg-info/zip-safe
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-25 14:51:22.200917 django-lti-toolbox-1.3.0/src/lti_toolbox/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      236 2024-04-25 14:51:21.000000 django-lti-toolbox-1.3.0/src/lti_toolbox/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      612 2024-04-25 14:51:21.000000 django-lti-toolbox-1.3.0/src/lti_toolbox/admin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      278 2024-04-25 14:51:21.000000 django-lti-toolbox-1.3.0/src/lti_toolbox/apps.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2608 2024-04-25 14:51:21.000000 django-lti-toolbox-1.3.0/src/lti_toolbox/backend.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1110 2024-04-25 14:51:21.000000 django-lti-toolbox-1.3.0/src/lti_toolbox/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      839 2024-04-25 14:51:21.000000 django-lti-toolbox-1.3.0/src/lti_toolbox/factories.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7094 2024-04-25 14:51:21.000000 django-lti-toolbox-1.3.0/src/lti_toolbox/launch_params.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7255 2024-04-25 14:51:21.000000 django-lti-toolbox-1.3.0/src/lti_toolbox/lti.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-25 14:51:22.200917 django-lti-toolbox-1.3.0/src/lti_toolbox/migrations/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3388 2024-04-25 14:51:21.000000 django-lti-toolbox-1.3.0/src/lti_toolbox/migrations/0001_initial.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      550 2024-04-25 14:51:21.000000 django-lti-toolbox-1.3.0/src/lti_toolbox/migrations/0002_lticonsumer_url.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-04-25 14:51:21.000000 django-lti-toolbox-1.3.0/src/lti_toolbox/migrations/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4001 2024-04-25 14:51:21.000000 django-lti-toolbox-1.3.0/src/lti_toolbox/models.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1536 2024-04-25 14:51:21.000000 django-lti-toolbox-1.3.0/src/lti_toolbox/utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6837 2024-04-25 14:51:21.000000 django-lti-toolbox-1.3.0/src/lti_toolbox/validator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3614 2024-04-25 14:51:21.000000 django-lti-toolbox-1.3.0/src/lti_toolbox/views.py
```

### Comparing `django-lti-toolbox-1.2.0/LICENSE` & `django-lti-toolbox-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-lti-toolbox-1.2.0/PKG-INFO` & `django-lti-toolbox-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-lti-toolbox
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Django application to build LTI Tool Providers
 Home-page: https://github.com/openfun/django-lti-toolbox
 Author: Open FUN (France Universite Numerique)
 Author-email: fun.dev@fun-mooc.fr
 License: MIT
 Keywords: Django,LTI
 Platform: UNKNOWN
```

### Comparing `django-lti-toolbox-1.2.0/README.md` & `django-lti-toolbox-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `django-lti-toolbox-1.2.0/setup.cfg` & `django-lti-toolbox-1.3.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-lti-toolbox
-version = 1.2.0
+version = 1.3.0
 description = A Django application to build LTI Tool Providers
 long_description = file:README.md
 long_description_content_type = text/markdown
 author = Open FUN (France Universite Numerique)
 author_email = fun.dev@fun-mooc.fr
 url = https://github.com/openfun/django-lti-toolbox
 license = MIT
```

### Comparing `django-lti-toolbox-1.2.0/src/django_lti_toolbox.egg-info/PKG-INFO` & `django-lti-toolbox-1.3.0/src/django_lti_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-lti-toolbox
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Django application to build LTI Tool Providers
 Home-page: https://github.com/openfun/django-lti-toolbox
 Author: Open FUN (France Universite Numerique)
 Author-email: fun.dev@fun-mooc.fr
 License: MIT
 Keywords: Django,LTI
 Platform: UNKNOWN
```

### Comparing `django-lti-toolbox-1.2.0/src/django_lti_toolbox.egg-info/SOURCES.txt` & `django-lti-toolbox-1.3.0/src/django_lti_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-lti-toolbox-1.2.0/src/lti_toolbox/admin.py` & `django-lti-toolbox-1.3.0/src/lti_toolbox/admin.py`

 * *Files identical despite different names*

### Comparing `django-lti-toolbox-1.2.0/src/lti_toolbox/backend.py` & `django-lti-toolbox-1.3.0/src/lti_toolbox/backend.py`

 * *Files identical despite different names*

### Comparing `django-lti-toolbox-1.2.0/src/lti_toolbox/exceptions.py` & `django-lti-toolbox-1.3.0/src/lti_toolbox/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-lti-toolbox-1.2.0/src/lti_toolbox/factories.py` & `django-lti-toolbox-1.3.0/src/lti_toolbox/factories.py`

 * *Files identical despite different names*

### Comparing `django-lti-toolbox-1.2.0/src/lti_toolbox/launch_params.py` & `django-lti-toolbox-1.3.0/src/lti_toolbox/launch_params.py`

 * *Files identical despite different names*

### Comparing `django-lti-toolbox-1.2.0/src/lti_toolbox/lti.py` & `django-lti-toolbox-1.3.0/src/lti_toolbox/lti.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """LTI module that supports LTI 1.0.
 """
 import re
 from typing import Any, Optional, Set
+from urllib.parse import urljoin
 
 from oauthlib.oauth1 import SignatureOnlyEndpoint
 
 from .exceptions import LTIException, LTIRequestNotVerifiedException, ParamException
 from .launch_params import (
     LaunchParams,
     LTIMessageType,
@@ -131,19 +132,35 @@
                     "school_name": part[0] if length >= 1 else None,
                     "course_name": part[1] if length >= 2 else None,
                     "course_run": part[2] if length >= 3 else None,
                 }
 
         return {
             "school_name": self.get_param("tool_consumer_instance_name", None),
-            "course_name": self.get_param("context_title"),
+            "course_name": self.context_title,
             "course_run": None,
         }
 
     @property
+    def origin_url(self):
+        """Try to recreate the URL that was used to launch the LTI request."""
+        base_url = self.request.META.get("HTTP_REFERER")
+        if not base_url:
+            return None
+        context_id = self.get_param("context_id")
+
+        url = None
+        if self.is_edx_format:
+            url = urljoin(base_url, f"/course/{context_id}")
+        elif self.is_moodle_format:
+            url = urljoin(base_url, f"/course/view.php?id={context_id}")
+
+        return url
+
+    @property
     def resource_link_title(self) -> Optional[str]:
         """Return the resource link id as default for its title."""
         return self.get_param("resource_link_title", self.get_param("resource_link_id"))
 
     @property
     def context_title(self) -> Optional[str]:
         """Return the context id as default for its title."""
@@ -165,14 +182,26 @@
 
         Returns:
             boolean: True if the LTI request is sent by Open edX
 
         """
         return re.search(r"^course-v[0-9]:.*$", self.get_param("context_id"))
 
+    @property
+    def is_moodle_format(self):
+        """Check if the LTI request comes from Moodle.
+
+        Returns
+        -------
+        boolean
+            True if the LTI request is sent by Moodle
+
+        """
+        return self.get_param("tool_consumer_info_product_family_code", "") == "moodle"
+
     def _has_any_of_roles(self, roles: Set[str]):
         """Check if the LTI user has any of the provided roles."""
         return not roles.isdisjoint(self.roles)
 
     @property
     def is_student(self):
         """Check if the LTI user is a student.
```

### Comparing `django-lti-toolbox-1.2.0/src/lti_toolbox/migrations/0001_initial.py` & `django-lti-toolbox-1.3.0/src/lti_toolbox/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-lti-toolbox-1.2.0/src/lti_toolbox/migrations/0002_lticonsumer_url.py` & `django-lti-toolbox-1.3.0/src/lti_toolbox/migrations/0002_lticonsumer_url.py`

 * *Files identical despite different names*

### Comparing `django-lti-toolbox-1.2.0/src/lti_toolbox/models.py` & `django-lti-toolbox-1.3.0/src/lti_toolbox/models.py`

 * *Files identical despite different names*

### Comparing `django-lti-toolbox-1.2.0/src/lti_toolbox/utils.py` & `django-lti-toolbox-1.3.0/src/lti_toolbox/utils.py`

 * *Files identical despite different names*

### Comparing `django-lti-toolbox-1.2.0/src/lti_toolbox/validator.py` & `django-lti-toolbox-1.3.0/src/lti_toolbox/validator.py`

 * *Files identical despite different names*

### Comparing `django-lti-toolbox-1.2.0/src/lti_toolbox/views.py` & `django-lti-toolbox-1.3.0/src/lti_toolbox/views.py`

 * *Files identical despite different names*

