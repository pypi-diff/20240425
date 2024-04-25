# Comparing `tmp/eam_b2c_helper-0.1.1.tar.gz` & `tmp/eam_b2c_helper-0.1.2.tar.gz`

## Comparing `eam_b2c_helper-0.1.1.tar` & `eam_b2c_helper-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.1/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.1/src/eam_b2c_helper/__init__.py
--rw-r--r--   0        0        0     9590 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.1/src/eam_b2c_helper/b2c.py
--rw-r--r--   0        0        0    16487 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.1/tests/test_b2c.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.1/LICENSE
--rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.1/README.md
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.2/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.2/src/eam_b2c_helper/__init__.py
+-rw-r--r--   0        0        0     9731 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.2/src/eam_b2c_helper/b2c.py
+-rw-r--r--   0        0        0    16487 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.2/tests/test_b2c.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.2/README.md
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.2/PKG-INFO
```

### Comparing `eam_b2c_helper-0.1.1/src/eam_b2c_helper/b2c.py` & `eam_b2c_helper-0.1.2/src/eam_b2c_helper/b2c.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,18 @@
 def build_federated_user_object(user_details: dict, extension_id: str) -> dict:
     """Builds a federated user object to be used in the creation or update of a user in Azure AD B2C"""
     return {
         "accountEnabled": True,
         "displayName": f"{user_details['firstName']} {user_details['lastName']}",
         "mailNickname": user_details['firstName'],
         "otherMails": [user_details['email']],
+        "passwordProfile": {
+            "forceChangePasswordNextSignIn": False,
+            "password": user_details['password']
+        },
         "mobilePhone": user_details['phone'],
         f"extension_{extension_id}_OrganizationID": user_details['company_id'],
         f"extension_{extension_id}_SignUpCode": user_details['sign_up_code'],
         f"extension_{extension_id}_UserRoles": user_details['role'],
         f"extension_{extension_id}_mustResetPassword": user_details['reset_password']
     }
```

### Comparing `eam_b2c_helper-0.1.1/tests/test_b2c.py` & `eam_b2c_helper-0.1.2/tests/test_b2c.py`

 * *Files identical despite different names*

### Comparing `eam_b2c_helper-0.1.1/LICENSE` & `eam_b2c_helper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eam_b2c_helper-0.1.1/README.md` & `eam_b2c_helper-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `eam_b2c_helper-0.1.1/PKG-INFO` & `eam_b2c_helper-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: eam_b2c_helper
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package to interact with ms graph /users functionality
 Author-email: Dave Gunn <daveg@8amsolutions.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

