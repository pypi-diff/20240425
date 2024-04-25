# Comparing `tmp/proxygen_cli-2.1.8.tar.gz` & `tmp/proxygen_cli-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxygen_cli-2.1.8.tar", max compression
+gzip compressed data, was "proxygen_cli-2.1.9.tar", max compression
```

## Comparing `proxygen_cli-2.1.8.tar` & `proxygen_cli-2.1.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     3336 2024-04-23 08:24:49.628867 proxygen_cli-2.1.8/README.md
--rw-r--r--   0        0        0      248 2024-04-23 08:24:49.628867 proxygen_cli-2.1.8/proxygen_cli/__init__.py
--rw-r--r--   0        0        0     3268 2024-04-23 08:24:49.628867 proxygen_cli-2.1.8/proxygen_cli/cli/command_credentials.py
--rw-r--r--   0        0        0     1167 2024-04-23 08:24:49.628867 proxygen_cli-2.1.8/proxygen_cli/cli/command_docker.py
--rw-r--r--   0        0        0     4603 2024-04-23 08:24:49.628867 proxygen_cli-2.1.8/proxygen_cli/cli/command_instance.py
--rw-r--r--   0        0        0      951 2024-04-23 08:24:49.628867 proxygen_cli-2.1.8/proxygen_cli/cli/command_main.py
--rw-r--r--   0        0        0      861 2024-04-23 08:24:49.628867 proxygen_cli-2.1.8/proxygen_cli/cli/command_pytest_nhsd_apim_token.py
--rw-r--r--   0        0        0     6548 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/cli/command_secret.py
--rw-r--r--   0        0        0     1781 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/cli/command_settings.py
--rw-r--r--   0        0        0     3697 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/cli/command_spec.py
--rw-r--r--   0        0        0     5722 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/lib/auth.py
--rw-r--r--   0        0        0      268 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/lib/constants.py
--rw-r--r--   0        0        0     4170 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/lib/credentials.py
--rw-r--r--   0        0        0     1018 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/lib/dot_proxygen.py
--rw-r--r--   0        0        0     1562 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/lib/output.py
--rw-r--r--   0        0        0     5880 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/lib/proxygen_api.py
--rw-r--r--   0        0        0      865 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/lib/settings.py
--rw-r--r--   0        0        0     3037 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/lib/spec.py
--rw-r--r--   0        0        0     1042 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/lib/spec_server.py
--rw-r--r--   0        0        0      520 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/lib/version.py
--rw-r--r--   0        0        0        0 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/test/__init__.py
--rw-r--r--   0        0        0     6555 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/test/command_credentials_test.py
--rw-r--r--   0        0        0    13013 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/test/command_instance_test.py
--rw-r--r--   0        0        0      752 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/test/command_main_test.py
--rw-r--r--   0        0        0      688 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/test/command_pytest_nhsd_apim_token_test.py
--rw-r--r--   0        0        0     7005 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/test/command_secret_test.py
--rw-r--r--   0        0        0     3591 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/test/command_settings_test.py
--rw-r--r--   0        0        0     4263 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/test/command_spec_test.py
--rw-r--r--   0        0        0     6678 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/test/conftest.py
--rw-r--r--   0        0        0     3272 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/test/fixtures/client.key
--rw-r--r--   0        0        0     1952 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/test/fixtures/client.pem
--rw-r--r--   0        0        0       30 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/test/fixtures/secret.txt
--rw-r--r--   0        0        0      570 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/test/mock_private_key.py
--rw-r--r--   0        0        0      786 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/proxygen_cli/test/validate_cli_version_test.py
--rw-r--r--   0        0        0      760 2024-04-23 08:24:49.632867 proxygen_cli-2.1.8/pyproject.toml
--rw-r--r--   0        0        0     4306 1970-01-01 00:00:00.000000 proxygen_cli-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0     3354 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/README.md
+-rw-r--r--   0        0        0      248 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/__init__.py
+-rw-r--r--   0        0        0     2988 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/cli/command_credentials.py
+-rw-r--r--   0        0        0     1167 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/cli/command_docker.py
+-rw-r--r--   0        0        0     4603 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/cli/command_instance.py
+-rw-r--r--   0        0        0      951 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/cli/command_main.py
+-rw-r--r--   0        0        0      861 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/cli/command_pytest_nhsd_apim_token.py
+-rw-r--r--   0        0        0     6548 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/cli/command_secret.py
+-rw-r--r--   0        0        0     1781 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/cli/command_settings.py
+-rw-r--r--   0        0        0     3697 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/cli/command_spec.py
+-rw-r--r--   0        0        0     5722 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/lib/auth.py
+-rw-r--r--   0        0        0      268 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/lib/constants.py
+-rw-r--r--   0        0        0     4375 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/lib/credentials.py
+-rw-r--r--   0        0        0     1018 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/lib/dot_proxygen.py
+-rw-r--r--   0        0        0     1562 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/lib/output.py
+-rw-r--r--   0        0        0     5880 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/lib/proxygen_api.py
+-rw-r--r--   0        0        0      865 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/lib/settings.py
+-rw-r--r--   0        0        0     3037 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/lib/spec.py
+-rw-r--r--   0        0        0     1042 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/lib/spec_server.py
+-rw-r--r--   0        0        0      520 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/lib/version.py
+-rw-r--r--   0        0        0        0 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/test/__init__.py
+-rw-r--r--   0        0        0    10697 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/test/command_credentials_test.py
+-rw-r--r--   0        0        0    13013 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/test/command_instance_test.py
+-rw-r--r--   0        0        0      752 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/test/command_main_test.py
+-rw-r--r--   0        0        0      688 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/test/command_pytest_nhsd_apim_token_test.py
+-rw-r--r--   0        0        0     7005 2024-04-23 14:46:26.853902 proxygen_cli-2.1.9/proxygen_cli/test/command_secret_test.py
+-rw-r--r--   0        0        0     3591 2024-04-23 14:46:26.857902 proxygen_cli-2.1.9/proxygen_cli/test/command_settings_test.py
+-rw-r--r--   0        0        0     4263 2024-04-23 14:46:26.857902 proxygen_cli-2.1.9/proxygen_cli/test/command_spec_test.py
+-rw-r--r--   0        0        0     6678 2024-04-23 14:46:26.857902 proxygen_cli-2.1.9/proxygen_cli/test/conftest.py
+-rw-r--r--   0        0        0     3272 2024-04-23 14:46:26.857902 proxygen_cli-2.1.9/proxygen_cli/test/fixtures/client.key
+-rw-r--r--   0        0        0     1952 2024-04-23 14:46:26.857902 proxygen_cli-2.1.9/proxygen_cli/test/fixtures/client.pem
+-rw-r--r--   0        0        0       30 2024-04-23 14:46:26.857902 proxygen_cli-2.1.9/proxygen_cli/test/fixtures/secret.txt
+-rw-r--r--   0        0        0      570 2024-04-23 14:46:26.857902 proxygen_cli-2.1.9/proxygen_cli/test/mock_private_key.py
+-rw-r--r--   0        0        0      786 2024-04-23 14:46:26.857902 proxygen_cli-2.1.9/proxygen_cli/test/validate_cli_version_test.py
+-rw-r--r--   0        0        0      760 2024-04-23 14:46:26.857902 proxygen_cli-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4324 1970-01-01 00:00:00.000000 proxygen_cli-2.1.9/PKG-INFO
```

### Comparing `proxygen_cli-2.1.8/README.md` & `proxygen_cli-2.1.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 After installation, the `proxygen` executable is available. Typing `proxygen` displays a list of available commands.
 
 
 ## Configuration
 
 ### Credentials
 
-The CLI requires client credentials, which can be obtained from the `platforms-api-producer-support` Slack channel.
+The Proxygen CLI client credentials `client_id`, `client_secret` are setup as part of proxygen CLI package.
 
-All users should also have individual credentials. `proxygen-cli` needs to know about them.
-You can setup the credentials in `proxygen-cli` using:
+All users should have individual credentials. `proxygen-cli` needs to know about them. You can setup your user credentials in proxygen-cli using:
 ```
 proxygen credentials set
 ```
-This command prompts you to enter your `client_id`, `client_secret`, `username`, and `password`. 
-To update credentials in the future, use:
+This command prompts you to enter your `username`, and `password`.
+
+To update any credentials `client_id`/ `client_secret`/ `username`/ `password` in the future, use:
 ```
 proxygen credentials set <KEY> <VALUE>
 ```
 
 
 ### Settings
 To specify the API you are developing for, use:
```

### Comparing `proxygen_cli-2.1.8/proxygen_cli/cli/command_credentials.py` & `proxygen_cli-2.1.9/proxygen_cli/cli/command_credentials.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import json
 import click
 import yaml
 import pydantic
+import os
 
 from proxygen_cli.lib import output
 from proxygen_cli.lib.credentials import (
     Credentials, get_credentials, _yaml_credentials_file_source, create_yaml_credentials_file, initialise_credentials)
 from proxygen_cli.lib.dot_proxygen import credentials_file
 
 CHOICE_OF_CREDENTIAL_KEYS = click.Choice(Credentials.__fields__.keys())
 
-
 @click.group()
 def credentials():
     """Get/set credentials."""
 
 
 @credentials.command()
 def list():
@@ -51,28 +51,24 @@
     Write a value to your credentials.
     """
     if not _yaml_credentials_file_source(None):
         create_yaml_credentials_file()
 
     current_credentials = _yaml_credentials_file_source(None)
 
-    # Check if base credentials are set
+    # Check if user credentials are set
     base_credentials_set = all(
         current_credentials.get(field) is not None
-        for field in ["client_id", "client_secret", "username", "password"]
+        for field in ["username", "password"]
     )
 
     if not base_credentials_set or force:
-        client_id = click.prompt("Enter client_id")
-        client_secret = click.prompt("Enter client_secret", default="", show_default=False)
         username = click.prompt("Enter username", default="", show_default=False)
         password = click.prompt("Enter password", default="", show_default=False)
 
-        current_credentials["client_id"] = client_id
-        current_credentials["client_secret"] = client_secret
         current_credentials["username"] = username
         current_credentials["password"] = password
 
     # Prompt for individual custom key-value pairs
     for i in range(0, len(custom_pairs), 2):
         key, value = custom_pairs[i:i + 2]
         current_credentials[key] = value
@@ -94,8 +90,8 @@
 def rm(key):
     """
     Delete a value from your credentials.
     """
     current_credentials = _yaml_credentials_file_source(None)
     current_credentials.pop(key, None)
     with credentials_file().open("w") as f:
-        yaml.safe_dump(current_credentials, f)
+        yaml.safe_dump(current_credentials, f)
```

### Comparing `proxygen_cli-2.1.8/proxygen_cli/cli/command_docker.py` & `proxygen_cli-2.1.9/proxygen_cli/cli/command_docker.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/cli/command_instance.py` & `proxygen_cli-2.1.9/proxygen_cli/cli/command_instance.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/cli/command_main.py` & `proxygen_cli-2.1.9/proxygen_cli/cli/command_main.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/cli/command_pytest_nhsd_apim_token.py` & `proxygen_cli-2.1.9/proxygen_cli/cli/command_pytest_nhsd_apim_token.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/cli/command_secret.py` & `proxygen_cli-2.1.9/proxygen_cli/cli/command_secret.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/cli/command_settings.py` & `proxygen_cli-2.1.9/proxygen_cli/cli/command_settings.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/cli/command_spec.py` & `proxygen_cli-2.1.9/proxygen_cli/cli/command_spec.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/lib/auth.py` & `proxygen_cli-2.1.9/proxygen_cli/lib/auth.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/lib/credentials.py` & `proxygen_cli-2.1.9/proxygen_cli/lib/credentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,26 +11,32 @@
     validator,
     AnyHttpUrl,
     ValidationError,
 )
 
 from . import dot_proxygen
 
+CLIENT_ID = os.environ["proxygen_client_id"]
+CLIENT_SECRET = os.environ["proxygen_client_secret"]
+
+data = {"client_id": CLIENT_ID, "client_secret": CLIENT_SECRET}
+
 
 def _yaml_credentials_file_source(_):
     with dot_proxygen.credentials_file().open() as yaml_file:
         credentials = yaml.safe_load(yaml_file)
         return credentials or {}
 
 
 def create_yaml_credentials_file():
     file_path = os.path.expanduser("~/.proxygen/credentials.yaml")
 
     if not os.path.exists(file_path):
-        with open(file_path, 'w'):
+        with open(file_path, "w"):
+            yaml.dump(data, file_path)
             pass
 
 
 class Credentials(BaseSettings):
     base_url: AnyHttpUrl = (
         "https://identity.prod.api.platform.nhs.uk/realms/api-producers"
     )
@@ -109,14 +115,16 @@
                 init_settings,
                 env_settings,
                 _yaml_credentials_file_source,
             )
 
 
 _CREDENTIALS = None
+
+
 def initialise_credentials():
     global _CREDENTIALS
     try:
         _CREDENTIALS = Credentials()
     except ValidationError as e:
         errors = json.loads(e.json())
         print("*" * 100, file=sys.stderr)
```

### Comparing `proxygen_cli-2.1.8/proxygen_cli/lib/dot_proxygen.py` & `proxygen_cli-2.1.9/proxygen_cli/lib/dot_proxygen.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/lib/output.py` & `proxygen_cli-2.1.9/proxygen_cli/lib/output.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/lib/proxygen_api.py` & `proxygen_cli-2.1.9/proxygen_cli/lib/proxygen_api.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/lib/settings.py` & `proxygen_cli-2.1.9/proxygen_cli/lib/settings.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/lib/spec.py` & `proxygen_cli-2.1.9/proxygen_cli/lib/spec.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/lib/spec_server.py` & `proxygen_cli-2.1.9/proxygen_cli/lib/spec_server.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/lib/version.py` & `proxygen_cli-2.1.9/proxygen_cli/lib/version.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/test/command_instance_test.py` & `proxygen_cli-2.1.9/proxygen_cli/test/command_instance_test.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/test/command_main_test.py` & `proxygen_cli-2.1.9/proxygen_cli/test/command_main_test.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/test/command_pytest_nhsd_apim_token_test.py` & `proxygen_cli-2.1.9/proxygen_cli/test/command_pytest_nhsd_apim_token_test.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/test/command_secret_test.py` & `proxygen_cli-2.1.9/proxygen_cli/test/command_secret_test.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/test/command_settings_test.py` & `proxygen_cli-2.1.9/proxygen_cli/test/command_settings_test.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/test/command_spec_test.py` & `proxygen_cli-2.1.9/proxygen_cli/test/command_spec_test.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/test/conftest.py` & `proxygen_cli-2.1.9/proxygen_cli/test/conftest.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/test/fixtures/client.key` & `proxygen_cli-2.1.9/proxygen_cli/test/fixtures/client.key`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/test/fixtures/client.pem` & `proxygen_cli-2.1.9/proxygen_cli/test/fixtures/client.pem`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/test/mock_private_key.py` & `proxygen_cli-2.1.9/proxygen_cli/test/mock_private_key.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/proxygen_cli/test/validate_cli_version_test.py` & `proxygen_cli-2.1.9/proxygen_cli/test/validate_cli_version_test.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.8/pyproject.toml` & `proxygen_cli-2.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proxygen-cli"
-version = "2.1.8"
+version = "2.1.9"
 description = "CLI for interacting with NHSD APIM's proxygen service"
 authors = ["Ben Strutt <ben.strutt1@nhs.net>"]
 readme = "README.md"
 packages = [{include = "proxygen_cli"}]
 repository = "https://github.com/NHSDigital/proxygen-cli"
 
 [tool.poetry.scripts]
```

### Comparing `proxygen_cli-2.1.8/PKG-INFO` & `proxygen_cli-2.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxygen-cli
-Version: 2.1.8
+Version: 2.1.9
 Summary: CLI for interacting with NHSD APIM's proxygen service
 Home-page: https://github.com/NHSDigital/proxygen-cli
 Author: Ben Strutt
 Author-email: ben.strutt1@nhs.net
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -34,23 +34,23 @@
 After installation, the `proxygen` executable is available. Typing `proxygen` displays a list of available commands.
 
 
 ## Configuration
 
 ### Credentials
 
-The CLI requires client credentials, which can be obtained from the `platforms-api-producer-support` Slack channel.
+The Proxygen CLI client credentials `client_id`, `client_secret` are setup as part of proxygen CLI package.
 
-All users should also have individual credentials. `proxygen-cli` needs to know about them.
-You can setup the credentials in `proxygen-cli` using:
+All users should have individual credentials. `proxygen-cli` needs to know about them. You can setup your user credentials in proxygen-cli using:
 ```
 proxygen credentials set
 ```
-This command prompts you to enter your `client_id`, `client_secret`, `username`, and `password`. 
-To update credentials in the future, use:
+This command prompts you to enter your `username`, and `password`.
+
+To update any credentials `client_id`/ `client_secret`/ `username`/ `password` in the future, use:
 ```
 proxygen credentials set <KEY> <VALUE>
 ```
 
 
 ### Settings
 To specify the API you are developing for, use:
```

