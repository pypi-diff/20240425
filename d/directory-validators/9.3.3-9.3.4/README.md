# Comparing `tmp/directory_validators-9.3.3-py3-none-any.whl.zip` & `tmp/directory_validators-9.3.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 6529 bytes, number of entries: 10
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-20 16:29 directory_validators/__init__.py
--rw-r--r--  2.0 unx     1362 b- defN 24-Feb-20 16:29 directory_validators/file.py
--rw-r--r--  2.0 unx      959 b- defN 24-Feb-20 16:29 directory_validators/password.py
--rw-r--r--  2.0 unx     1295 b- defN 24-Feb-20 16:29 directory_validators/string.py
--rw-r--r--  2.0 unx     2247 b- defN 24-Feb-20 16:29 directory_validators/url.py
--rw-r--r--  2.0 unx     1091 b- defN 24-Feb-20 16:29 directory_validators-9.3.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     4771 b- defN 24-Feb-20 16:29 directory_validators-9.3.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-20 16:29 directory_validators-9.3.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 24-Feb-20 16:29 directory_validators-9.3.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      881 b- defN 24-Feb-20 16:29 directory_validators-9.3.3.dist-info/RECORD
-10 files, 12719 bytes uncompressed, 5001 bytes compressed:  60.7%
+Zip file size: 7053 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 10:55 directory_validators/__init__.py
+-rw-r--r--  2.0 unx     1362 b- defN 24-Apr-25 10:55 directory_validators/file.py
+-rw-r--r--  2.0 unx      723 b- defN 24-Apr-25 10:55 directory_validators/helper.py
+-rw-r--r--  2.0 unx      959 b- defN 24-Apr-25 10:55 directory_validators/password.py
+-rw-r--r--  2.0 unx     1295 b- defN 24-Apr-25 10:55 directory_validators/string.py
+-rw-r--r--  2.0 unx     2232 b- defN 24-Apr-25 10:55 directory_validators/url.py
+-rw-r--r--  2.0 unx     1091 b- defN 24-Apr-25 10:55 directory_validators-9.3.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4771 b- defN 24-Apr-25 10:55 directory_validators-9.3.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 10:55 directory_validators-9.3.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 24-Apr-25 10:55 directory_validators-9.3.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      967 b- defN 24-Apr-25 10:55 directory_validators-9.3.4.dist-info/RECORD
+11 files, 13513 bytes uncompressed, 5389 bytes compressed:  60.1%
```

## zipnote {}

```diff
@@ -1,31 +1,34 @@
 Filename: directory_validators/__init__.py
 Comment: 
 
 Filename: directory_validators/file.py
 Comment: 
 
+Filename: directory_validators/helper.py
+Comment: 
+
 Filename: directory_validators/password.py
 Comment: 
 
 Filename: directory_validators/string.py
 Comment: 
 
 Filename: directory_validators/url.py
 Comment: 
 
-Filename: directory_validators-9.3.3.dist-info/LICENSE
+Filename: directory_validators-9.3.4.dist-info/LICENSE
 Comment: 
 
-Filename: directory_validators-9.3.3.dist-info/METADATA
+Filename: directory_validators-9.3.4.dist-info/METADATA
 Comment: 
 
-Filename: directory_validators-9.3.3.dist-info/WHEEL
+Filename: directory_validators-9.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: directory_validators-9.3.3.dist-info/top_level.txt
+Filename: directory_validators-9.3.4.dist-info/top_level.txt
 Comment: 
 
-Filename: directory_validators-9.3.3.dist-info/RECORD
+Filename: directory_validators-9.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## directory_validators/url.py

```diff
@@ -1,11 +1,12 @@
 import re
-from urllib import parse
 
-from django.core.validators import RegexValidator, ValidationError
+from django.core.validators import RegexValidator
+
+from directory_validators.helper import validate_social_media_url
 
 
 MESSAGE_REMOVE_URL = 'Please remove the web or email addresses'
 MESSAGE_NOT_FACEBOOK = 'Please provide a link to Facebook.'
 MESSAGE_NOT_TWITTER = 'Please provide a link to Twitter.'
 MESSAGE_NOT_LINKEDIN = 'Please provide a link to LinkedIn.'
 
@@ -36,45 +37,39 @@
     Args:
         value (string): The url to check.
 
     Raises:
         django.forms.ValidationError
 
     """
-
-    parsed = parse.urlparse(value.lower())
-    if not parsed.netloc.endswith('facebook.com'):
-        raise ValidationError(MESSAGE_NOT_FACEBOOK)
+    allowed_list = ['facebook.com', '*.facebook.com']
+    return validate_social_media_url(value, allowed_list, MESSAGE_NOT_FACEBOOK)
 
 
 def is_twitter(value):
     """
     Confirms that the social media url is pointed at the correct domain.
 
     Args:
         value (string): The url to check.
 
     Raises:
         django.forms.ValidationError
 
     """
-
-    parsed = parse.urlparse(value.lower())
-    if not parsed.netloc.endswith('twitter.com'):
-        raise ValidationError(MESSAGE_NOT_TWITTER)
+    allowed_list = ['twitter.com', '*.twitter.com']
+    return validate_social_media_url(value, allowed_list, MESSAGE_NOT_TWITTER)
 
 
 def is_linkedin(value):
     """
     Confirms that the social media url is pointed at the correct domain.
 
     Args:
         value (string): The url to check.
 
     Raises:
         django.forms.ValidationError
 
     """
-
-    parsed = parse.urlparse(value.lower())
-    if not parsed.netloc.endswith('linkedin.com'):
-        raise ValidationError(MESSAGE_NOT_LINKEDIN)
+    allowed_list = ['linkedin.com', '*.linkedin.com']
+    return validate_social_media_url(value, allowed_list, MESSAGE_NOT_LINKEDIN)
```

## Comparing `directory_validators-9.3.3.dist-info/LICENSE` & `directory_validators-9.3.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `directory_validators-9.3.3.dist-info/METADATA` & `directory_validators-9.3.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directory-validators
-Version: 9.3.3
+Version: 9.3.4
 Summary: Django validators for GREAT.
 Home-page: https://github.com/uktrade/directory-validators
 Author: Department for International Trade
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

## Comparing `directory_validators-9.3.3.dist-info/RECORD` & `directory_validators-9.3.4.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 directory_validators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 directory_validators/file.py,sha256=V167APzkn47xleiGYZ1r8KBEJHMr1kf_8vFTaAhGDOM,1362
+directory_validators/helper.py,sha256=COVfZkx4o17I8eCUYXA91IP7ifoB7ctgRrm_h7-avYE,723
 directory_validators/password.py,sha256=J2a1glBu_cs6gJFsO-lqvxfR8R9gTtSHUfm4fDRnpJU,959
 directory_validators/string.py,sha256=hwVGMYoCRUWeCOLfaXVv81nJzFYb13vIdaxMCuE7P6o,1295
-directory_validators/url.py,sha256=PnfvDLuj8ze_jSSD4nHXyZB_-tFaqi2LWaxIhCObp1Q,2247
-directory_validators-9.3.3.dist-info/LICENSE,sha256=y-ArErAQz98OorLek2xntwEp9bo3ZcqfQMtAIcjBdvQ,1091
-directory_validators-9.3.3.dist-info/METADATA,sha256=WeXtuEtUnxA-P_BMAiDpYkGG4cUcaRpQwl0RekWT4tk,4771
-directory_validators-9.3.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-directory_validators-9.3.3.dist-info/top_level.txt,sha256=X-cd3CEWwAWY3Usg12ZBRwso59Mh8wwxBmtNjzDvnTA,21
-directory_validators-9.3.3.dist-info/RECORD,,
+directory_validators/url.py,sha256=9x7bW5pCtS3LDLPUoizQOeNOPc8VlHuwER4kgaMjztE,2232
+directory_validators-9.3.4.dist-info/LICENSE,sha256=y-ArErAQz98OorLek2xntwEp9bo3ZcqfQMtAIcjBdvQ,1091
+directory_validators-9.3.4.dist-info/METADATA,sha256=-lWgDU_ZQsEC1krR3Qoj8iUhjao8JZ32hQcKiS9ED2k,4771
+directory_validators-9.3.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+directory_validators-9.3.4.dist-info/top_level.txt,sha256=X-cd3CEWwAWY3Usg12ZBRwso59Mh8wwxBmtNjzDvnTA,21
+directory_validators-9.3.4.dist-info/RECORD,,
```

