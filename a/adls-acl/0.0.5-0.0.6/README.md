# Comparing `tmp/adls_acl-0.0.5.tar.gz` & `tmp/adls_acl-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adls_acl-0.0.5.tar", last modified: Sat Apr 13 23:56:24 2024, max compression
+gzip compressed data, was "adls_acl-0.0.6.tar", last modified: Wed Apr 24 22:10:15 2024, max compression
```

## Comparing `adls_acl-0.0.5.tar` & `adls_acl-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:56:24.867834 adls_acl-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-13 23:56:19.000000 adls_acl-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 23:56:19.000000 adls_acl-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-04-13 23:56:24.867834 adls_acl-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-04-13 23:56:19.000000 adls_acl-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-13 23:56:19.000000 adls_acl-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 23:56:24.867834 adls_acl-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-13 23:56:19.000000 adls_acl-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:56:24.863834 adls_acl-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:56:24.863834 adls_acl-0.0.5/src/adls_acl/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-13 23:56:19.000000 adls_acl-0.0.5/src/adls_acl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-13 23:56:19.000000 adls_acl-0.0.5/src/adls_acl/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-13 23:56:19.000000 adls_acl-0.0.5/src/adls_acl/input_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-13 23:56:19.000000 adls_acl-0.0.5/src/adls_acl/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-04-13 23:56:19.000000 adls_acl-0.0.5/src/adls_acl/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-04-13 23:56:19.000000 adls_acl-0.0.5/src/adls_acl/orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:56:24.867834 adls_acl-0.0.5/src/adls_acl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-04-13 23:56:24.000000 adls_acl-0.0.5/src/adls_acl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-13 23:56:24.000000 adls_acl-0.0.5/src/adls_acl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 23:56:24.000000 adls_acl-0.0.5/src/adls_acl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-13 23:56:24.000000 adls_acl-0.0.5/src/adls_acl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-13 23:56:24.000000 adls_acl-0.0.5/src/adls_acl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 23:56:24.000000 adls_acl-0.0.5/src/adls_acl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:56:24.867834 adls_acl-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-04-13 23:56:19.000000 adls_acl-0.0.5/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-13 23:56:19.000000 adls_acl-0.0.5/tests/test_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:10:15.950793 adls_acl-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-24 22:10:10.000000 adls_acl-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 22:10:10.000000 adls_acl-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-04-24 22:10:15.950793 adls_acl-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-04-24 22:10:10.000000 adls_acl-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-24 22:10:10.000000 adls_acl-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 22:10:15.950793 adls_acl-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-24 22:10:10.000000 adls_acl-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:10:15.946793 adls_acl-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:10:15.946793 adls_acl-0.0.6/src/adls_acl/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 22:10:10.000000 adls_acl-0.0.6/src/adls_acl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-24 22:10:10.000000 adls_acl-0.0.6/src/adls_acl/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-24 22:10:10.000000 adls_acl-0.0.6/src/adls_acl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-24 22:10:10.000000 adls_acl-0.0.6/src/adls_acl/input_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-24 22:10:10.000000 adls_acl-0.0.6/src/adls_acl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-04-24 22:10:10.000000 adls_acl-0.0.6/src/adls_acl/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-04-24 22:10:10.000000 adls_acl-0.0.6/src/adls_acl/orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:10:15.946793 adls_acl-0.0.6/src/adls_acl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-04-24 22:10:15.000000 adls_acl-0.0.6/src/adls_acl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-24 22:10:15.000000 adls_acl-0.0.6/src/adls_acl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 22:10:15.000000 adls_acl-0.0.6/src/adls_acl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-24 22:10:15.000000 adls_acl-0.0.6/src/adls_acl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-24 22:10:15.000000 adls_acl-0.0.6/src/adls_acl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 22:10:15.000000 adls_acl-0.0.6/src/adls_acl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:10:15.946793 adls_acl-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-24 22:10:10.000000 adls_acl-0.0.6/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-04-24 22:10:10.000000 adls_acl-0.0.6/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-24 22:10:10.000000 adls_acl-0.0.6/tests/test_orchestrator.py
```

### Comparing `adls_acl-0.0.5/LICENSE` & `adls_acl-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.5/PKG-INFO` & `adls_acl-0.0.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adls_acl
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small tool for managing Azure DataLake Store (ADLS) Access Control Lists (ACLs).
 Home-page: https://github.com/karolusz/adls-acl
 Author: Karol Luszczek
 Author-email: karol.luszczek@reinsight.se
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -70,43 +70,62 @@
   --log-file TEXT  Redirect logs to a file.
   --help           Show this message and exit.
 
 Commands:
   get-acl  Read the current fs and acls on dirs.
   set-acl  Read and set direcotry structure and ACLs from a YAML file.
 ```
+Options:
+* `--debug` log levels for the adls-acl and Azure SDK libraries will be set to `DEBUG`
+* `--silent` nothing gets printed to stdout.
+* `--log-file` a copy of log messages will be printed to that file
 
 #### `set-acl` command
 ```
 Usage: adls-acl set-acl [OPTIONS] FILE
 
   Read and set direcotry structure and ACLs from a YAML file.
 
 Options:
-  --help  Show this message and exit.
+  --auth-method [default|environment|workload|managedid|azurecli|azureps|azuredevcli]
+                                  Azure AD Authentication method
+  --auth-opt <TEXT TEXT>...       Keyword arguments to pass to Azure SDK
+                                  credential constructor
+  --help                          Show this message and exit.
 ```
+Options:
+ * `--auth-method` allows the user to choose from a Azure Python SDK [Authentication methods](#authentication-methods)
+ * `--auth-opt` keyword arguments to be passed to the Azure Python SDK authentication constructors. Can be used multiple times in a call.
 
 To set acls from an input file `test.yml` the shell command would look like:
 ```bash
 adls-acl set-acl test.yml
 ```
 
 #### `get-acl` command
 ```
 Usage: adls-acl get-acl [OPTIONS] ACCOUNT_NAME OUTFILE
 
   Read the current fs and acls on dirs.
 
 Options:
-  --omit-special        Omit special ACLs when reading the account.
-  --help                Show this message and exit.
+  --omit-special                  Omit special ACLs when reading the account.
+  --auth-method [default|environment|workload|managedid|azurecli|azureps|azuredevcli]
+                                  Azure AD Authentication method
+  --auth-opt <TEXT TEXT>...       Keyword arguments to pass to Azure SDK
+                                  credential constructor
+  --help                          Show this message and exit.
 ```
 
 This will print the current filesystem of an account (directories only, no files) and their ACLs to a file on a path pass as `OUTFILE` argument.
-[Special ACLs](#special-acls) can be omitted with a flag `--omit-special`
+Options:
+ * `--omit-special` [Special ACLs](#special-acls) can be omitted and not printed to the output file 
+ * `--auth-method` allows the user to choose from a Azure Python SDK [Authentication methods](#authentication-methods)
+ * `--auth-opt` keyword arguments to be passed to the Azure Python SDK authentication constructors. Can be used multiple times in a call. 
+
 
 To read ACLs of a ADLS storage account named `testaccount` to file `dump.yml`:
 ```bash
 adls-acl get-acl testaccount dump.yml
 ```
 
 ### Input file
@@ -248,7 +267,26 @@
 
 The default ACLs defined or set on the higher level directories are pushed down to subdirectories specified in the input file.
 They will not be set on any files that had existed in the directories prior to the execution of `adls-acl`.
 Moreover, any subdirectories that exist in the account but are not specified in the input file remain untouched by `adls-acl`.
 
 Future releases will allow for more control over this behaviour (i.e, updating default ACLs on all files created prior to the change of ACLs).
 
+### Authentication Methods
+
+The Azure Python SDK authentication is by default handled with [`DefaultAzureCredenial`](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.defaultazurecredential?view=azure-python).
+
+In addition, a user can target one of the supported Azure Python SDK, by using `--auth-method` option:
+
+- [`EnvironmentCredential`](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.defaultazurecredential?view=azure-python)
+- [`WorkloadIdentityCredential`](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.workloadidentitycredential?view=azure-python)
+- [`ManagedIdentityCredential`](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.managedidentitycredential?view=azure-python)
+- [`AzureCliCrendtial`](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.azureclicredential?view=azure-python)
+- [`AzurePowerShellCrendeital`](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.azurepowershellcredential?view=azure-python)
+- [`AzureDevleoperCliCredential`](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.azurepowershellcredential?view=azure-python)
+
+To pass keyword arguments to the credential constructs use `--auth-opt` option. This option can be used multiple times, one instance per keyword argument. 
+
+e.g. to pass `managed_identity_client_id` and `exclude_cli_credential` to `DefaultAzureCredental`:
+```
+--auth-method default --auth-opt managed_identity_client_id xxxx-xxxx-xxxxx --auth-opt exlcude_cli_credential False
+```
```

### Comparing `adls_acl-0.0.5/pyproject.toml` & `adls_acl-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.bumpver]
-current_version = "0.0.5"
+current_version = "0.0.6"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `adls_acl-0.0.5/setup.py` & `adls_acl-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 readme = open("README.md", encoding="utf-8").read()
 
 setup(
     name="adls_acl",
-    version="0.0.5",
+    version="0.0.6",
     url="https://github.com/karolusz/adls-acl",
     author="Karol Luszczek",
     author_email="karol.luszczek@reinsight.se",
     description="A small tool for managing Azure DataLake Store (ADLS) Access Control Lists (ACLs).",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `adls_acl-0.0.5/src/adls_acl/cli.py` & `adls_acl-0.0.6/src/adls_acl/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,60 +2,94 @@
 # References:
 # https://learn.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-acl-python#update-acls-recursively
 #
 #
 # https://learn.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-access-control#permissions-inheritance
 # default permissions have been set on the parent items before the child items have been created.
 #
-import click, logging, yaml
-from .logger import configure_logger
-from .orchestrator import Orchestrator
+import logging
+
+import click
+import yaml
+
 from .input_parser import config_from_yaml
+from .logger import configure_logger
 from .nodes import container_config_to_tree
+from .orchestrator import Orchestrator
+from .auth import AUTH_SUPPORTED_OPTIONS
 
 root_logger = logging.getLogger()  # Root Logger
 
 
 @click.group()
 @click.option("--debug", is_flag=True, help="Enable debug messages.")
 @click.option("--silent", is_flag=True, help="Suppress logs to stdout.")
 @click.option("--log-file", "log_file", default=None, help="Redirect logs to a file.")
-def cli(debug, silent, log_file):
-    global root_logger
+def cli(debug, silent, log_file, root_logger=root_logger):
     root_logger = configure_logger(root_logger, debug, silent, log_file)
 
 
 @cli.command()
 @click.argument(
     "file",
     type=click.File(mode="r", encoding="utf-8", lazy=True),
 )
-def set_acl(file):
+@click.option(
+    "--auth-method",
+    type=click.Choice(AUTH_SUPPORTED_OPTIONS, case_sensitive=False),
+    default="default",
+    help="Azure AD Authentication method",
+)
+@click.option(
+    "--auth-opt",
+    type=click.Tuple([str, str]),
+    multiple=True,
+    help="Keyword arguments to pass to Azure SDK credential constructor",
+)
+def set_acl(file, auth_method, auth_opt):
     """Read and set direcotry structure and ACLs from a YAML file."""
+    auth_opt = {x[0]: x[1] for x in auth_opt}
     config_str = file.read()
     acls_config = config_from_yaml(config_str)
+    o = Orchestrator(
+        acls_config["account"], auth_method=auth_method, auth_kwargs=auth_opt
+    )
 
     for container in acls_config["containers"]:
         tree_root = container_config_to_tree(container)
-        Orchestrator(tree_root, acls_config["account"]).process_tree()
+        o.process_tree(tree_root)
 
 
 @cli.command()
 @click.argument("account_name", type=str)
 @click.argument(
     "outfile",
     type=click.File("w", encoding="utf-8", lazy=True),
 )
 @click.option(
     "--omit-special",
     "omit_special",
     is_flag=True,
     help="Omit special ACLs when reading the account.",
 )
-def get_acl(account_name, outfile, omit_special):
+@click.option(
+    "--auth-method",
+    type=click.Choice(AUTH_SUPPORTED_OPTIONS, case_sensitive=False),
+    default="default",
+    help="Azure AD Authentication method",
+)
+@click.option(
+    "--auth-opt",
+    type=click.Tuple([str, str]),
+    multiple=True,
+    help="Keyword arguments to pass to Azure SDK credential constructor",
+)
+def get_acl(account_name, outfile, omit_special, auth_method, auth_opt):
     """Read the current fs and acls on dirs."""
-    data = Orchestrator(None, account_name).read_account(omit_special=omit_special)
+    data = Orchestrator(
+        account_name, auth_method=auth_method, auth_kwargs=auth_opt
+    ).read_account(omit_special=omit_special)
     yaml.dump(data, outfile, sort_keys=False, indent=2)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `adls_acl-0.0.5/src/adls_acl/input_parser.py` & `adls_acl-0.0.6/src/adls_acl/input_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import yamale
-import pkgutil
 import logging
+import pkgutil
 from typing import Dict
 
+import yamale
+
 log = logging.getLogger(__name__)
 
 
 def config_from_yaml(config_str: str) -> Dict:
     """Reads a yaml file into dictionary and validates."""
     schema = pkgutil.get_data(__name__, "schema.yml").decode("utf-8")
     config_schema = yamale.make_schema(None, parser="PyYAML", content=schema)
```

### Comparing `adls_acl-0.0.5/src/adls_acl/logger.py` & `adls_acl-0.0.6/src/adls_acl/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,31 +26,31 @@
     silent: bool = False,
     log_file: str = None,
 ):
     # Determine logging level, formatter, and filters
     filters = []
     if debug:
         logger.setLevel(logging.NOTSET)
-        format = logging.Formatter(FormatterStyleEnum.debug.value)
+        fromatter = logging.Formatter(FormatterStyleEnum.debug.value)
     else:
         logger.setLevel(logging.INFO)
-        format = logging.Formatter(FormatterStyleEnum.simple.value)
+        fromatter = logging.Formatter(FormatterStyleEnum.simple.value)
         filters.append(
             lambda record: "azure" not in record.name
         )  # Filters out logging from azure packages
 
     # Determine handlers
     handlers = []
     if not silent:
         handlers.append(HandlerEnum.stream(stdout))
     if log_file:
         handlers.append(HandlerEnum.file(filename=log_file, mode="w", encoding="utf-8"))
 
     # Apply formatters, filters and register handlers
     for handler in handlers:
-        handler.setFormatter(format)
+        handler.setFormatter(fromatter)
         for filter in filters:
             handler.addFilter(filter)
 
         logger.addHandler(handler)
 
     return logger
```

### Comparing `adls_acl-0.0.5/src/adls_acl/nodes.py` & `adls_acl-0.0.6/src/adls_acl/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import Self, Optional, Dict
 from dataclasses import dataclass
+from typing import Dict, Optional, Self
 
 
 @dataclass
 class Acl:
     p_type: str
     oid: str
     permissions: str
@@ -105,15 +105,15 @@
         self.parent = parent
         self.acls = set()
 
     def __str__(self):
         """Print node nicely"""
         s = f"Path to node: {self.path}"
 
-        s += f"\nAcls from input:"
+        s += "\nAcls from input:"
         for acl in self.acls:
             s += f"\n\t{str(acl)}"
 
         return s
 
     @property
     def path_in_file_system(self):
@@ -170,15 +170,15 @@
         data = {"name": self.name, "acls": [acl.to_yaml() for acl in self.acls]}
         if len(self.children) > 0:
             data["folders"] = [child.to_yaml() for child in self.children]
 
         return data
 
 
-def _add_folder_nodes(parent_node: Node, folder: Dict):
+def _add_folder_nodes(parent_node: Node | None, folder: Dict):
     node = Node(folder["name"], parent=parent_node)
     for acl in folder["acls"]:
         node.add_acl(Acl.from_dict(acl))
 
     if "folders" in folder:
         for subfolder in folder["folders"]:
             _ = _add_folder_nodes(node, subfolder)
```

### Comparing `adls_acl-0.0.5/src/adls_acl/orchestrator.py` & `adls_acl-0.0.6/src/adls_acl/orchestrator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,105 +1,97 @@
 import logging
 from azure.storage.filedatalake import (
     DataLakeServiceClient,
     DataLakeDirectoryClient,
 )
-from azure.identity import DefaultAzureCredential, AzureCliCredential
 from azure.core.exceptions import ResourceExistsError
 from abc import ABC, abstractmethod
-from typing import Set, Dict
+from typing import Set, Dict, Any
 
 from .nodes import Node, bfs, Acl, find_node_by_name
+from .auth import get_service_client
 
 log = logging.getLogger(__name__)
 
 
 class Orchestrator:
-    def __init__(self, root: Node, account_name: str):
-        self.root = root
-        self.sc = _get_service_client_token_credential(account_name)
+    def __init__(
+        self, account_name: str, auth_method: str = "default", **auth_kwargs: Any
+    ):
+        self.sc = get_service_client(account_name, auth_method, **auth_kwargs)
         self.account_name = account_name
 
-    def process_tree(self):
-        for node in bfs(self.root):
+    def process_tree(self, root):
+        for node in bfs(root):
             processor = processor_selector(node)
             dc = processor.get_dir_client(node, self.sc)
             processor.set_acls(node, dc)
 
     def read_account(self, omit_special: bool = False) -> Dict:
         data = {}
         data["account"] = self.account_name
         data["containers"] = []
         for container in self.sc.list_file_systems():
+            # Create a root node
             fc = self.sc.get_file_system_client(container)
             dc = fc._get_root_directory_client()
-
             root_node = Node(name=fc.file_system_name)
+            for acl in _get_current_acls(dc, omit_special):
+                root_node.add_acl(acl)
 
-            for acl in dc.get_access_control()["acl"].split(","):
-                acl = Acl.from_str(acl)
-                if omit_special and acl.is_special():
-                    pass
-                else:
-                    root_node.add_acl(acl)
-
+            # Add nodes to the tree
             path_list = fc.get_paths(recursive=True)
             for path in filter(lambda x: x.is_directory == True, path_list):
                 dc = fc.get_directory_client(path.name)
                 parent_name = ("/").join(path.name.split("/")[:-1])
                 parent_node = find_node_by_name(root_node, parent_name)
                 node_name = path.name.split("/")[-1]
                 node = Node(name=node_name, parent=parent_node)
-                for acl in dc.get_access_control()["acl"].split(","):
-                    acl = Acl.from_str(acl)
-                    if omit_special and acl.is_special():
-                        pass
-                    else:
-                        node.add_acl(acl)
+                for acl in _get_current_acls(dc, omit_special):
+                    node.add_acl(acl)
 
             data["containers"].append(root_node.to_yaml())
 
             return data
 
 
 class ClientWithACLSupport(ABC):
+    @staticmethod
     @abstractmethod
     def get_access_control(): ...
 
+    @staticmethod
     @abstractmethod
     def set_access_control(): ...
 
     # Not needed until update mode is implemented
     # @abstractmethod
     # def update_permissions_recursively(): ...
 
 
-def _get_service_client_token_credential(account_name: str) -> DataLakeServiceClient:
-    account_url = f"https://{account_name}.dfs.core.windows.net"
-    token_credential = DefaultAzureCredential()
-    service_client = DataLakeServiceClient(account_url, credential=token_credential)
-
-    return service_client
-
-
 def _filter_acls_to_preserve(current_acls: Set[Acl]) -> Set[Acl]:
     """Determines which ACLs in the current Node should be preserved in the update"""
     acls_to_preserve = set()
 
     for acl in current_acls:
         if any([acl.is_mask(), acl.is_other(), acl.is_owner(), acl.is_owner_group()]):
             acls_to_preserve.update((acl,))
 
     return acls_to_preserve
 
 
-def _get_current_acls(client: DataLakeDirectoryClient) -> Set[Acl]:
+def _get_current_acls(
+    client: DataLakeDirectoryClient, omit_special: bool = False
+) -> Set[Acl]:
     """Returns a set of ACLs currently set on the directory."""
     current_acls_str = client.get_access_control()["acl"]
-    return set([Acl.from_str(acl_str) for acl_str in current_acls_str.split(",")])
+    acls = set([Acl.from_str(acl_str) for acl_str in current_acls_str.split(",")])
+    if omit_special:
+        acls = set([acl for acl in acls if not acl.is_special()])
+    return acls
 
 
 def _set_acls(client: DataLakeDirectoryClient, acls: Set[Acl]) -> None:
     """Set ACLs from the set on the node"""
     log.info("Setting new acls:")
     for acl in acls:
         log.info(f"\t{str(acl)}")
@@ -109,84 +101,90 @@
 def _pushdown_acls(node: Node, acls: Set[Acl]) -> None:
     """Pushdown selected ACLs to the children of the node"""
     for child_node in node.children:
         child_node.acls.update(acls)
 
 
 class Processor(ABC):
+    @staticmethod
     @abstractmethod
-    def set_acls(self, node: Node, client: DataLakeDirectoryClient):
+    def set_acls(node: Node, client: DataLakeDirectoryClient):
         # Get current ACLs to preseve ACLs for
-        # Owner, Owner Group, mask, and other (unless specified in input)
+        # Owner, Owner Group, mask, and other
+        # they will only change if specifie in input
         current_acls = _get_current_acls(client)
         acls_to_preserve = _filter_acls_to_preserve(current_acls)
         acls_to_pushdown = set([acl for acl in node.acls if acl.is_default()])
 
         # Collect ACLs to set
         new_acls = node.acls
         new_acls.update(acls_to_preserve)
 
         _set_acls(client, new_acls)
         _pushdown_acls(node, acls_to_pushdown)
 
+    @staticmethod
     @abstractmethod
     def get_dir_client() -> ClientWithACLSupport: ...
 
-    @abstractmethod
-    def update_acls(): ...
+    # @staticmethod
+    # @abstractmethod
+    # def update_acls(): ...
 
 
 class ProcessorRoot(Processor):
-    def __init__(self):
-        pass
 
-    def get_dir_client(self, node: Node, client: DataLakeServiceClient):
+    @staticmethod
+    def get_dir_client(node: Node, client: DataLakeServiceClient):
         """Creates a container if it doesn't exist and returns a file clietn
         to its root directory."""
         log.info("PROCESSING NODE ===========")
         log.info(node)
         if node.is_root == False:
-            raise ValueError(f"Node is not the root!")
+            raise ValueError("Node is not the root!")
 
         try:
             fs_client = client.create_file_system(node.name)
         except ResourceExistsError:
             fs_client = client.get_file_system_client(file_system=node.name)
 
         return fs_client._get_root_directory_client()
 
-    def set_acls(self, node: Node, client: DataLakeDirectoryClient):
-        super().set_acls(node, client)
+    @staticmethod
+    def set_acls(node: Node, client: DataLakeDirectoryClient):
+        super(ProcessorRoot, ProcessorRoot).set_acls(node, client)
         client.close()
 
-    def update_acls():
-        pass
+    # @staticmethod
+    # def update_acls():
+    #    pass
 
 
 class ProcessorDir(Processor):
-    def __init__(self):
-        pass
 
-    def get_dir_client(self, node: Node, client: DataLakeServiceClient):
+    @staticmethod
+    def get_dir_client(node: Node, client: DataLakeServiceClient):
         """Creates a directory, if it doesn't exist and returns a directory
         client."""
         log.info("PROCESSING NODE ===========")
         log.info(node)
 
         folder_client = client.get_file_system_client(file_system=node.get_root().name)
         dir_client = folder_client.get_directory_client(node.path_in_file_system)
         dir_client.create_directory()
 
         return dir_client
 
-    def set_acls(self, node: Node, client: DataLakeDirectoryClient):
-        super().set_acls(node, client)
-
-    def update_acls():
-        pass
+    @staticmethod
+    def set_acls(node: Node, client: DataLakeDirectoryClient):
+        super(ProcessorDir, ProcessorDir).set_acls(node, client)
+
+    # @staticmethod
+    # def update_acls():
+    #    pass
 
 
 def processor_selector(node):
     if node.is_root:
         return ProcessorRoot()
     else:
         return ProcessorDir()
```

### Comparing `adls_acl-0.0.5/src/adls_acl.egg-info/PKG-INFO` & `adls_acl-0.0.6/src/adls_acl.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adls_acl
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small tool for managing Azure DataLake Store (ADLS) Access Control Lists (ACLs).
 Home-page: https://github.com/karolusz/adls-acl
 Author: Karol Luszczek
 Author-email: karol.luszczek@reinsight.se
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -70,43 +70,62 @@
   --log-file TEXT  Redirect logs to a file.
   --help           Show this message and exit.
 
 Commands:
   get-acl  Read the current fs and acls on dirs.
   set-acl  Read and set direcotry structure and ACLs from a YAML file.
 ```
+Options:
+* `--debug` log levels for the adls-acl and Azure SDK libraries will be set to `DEBUG`
+* `--silent` nothing gets printed to stdout.
+* `--log-file` a copy of log messages will be printed to that file
 
 #### `set-acl` command
 ```
 Usage: adls-acl set-acl [OPTIONS] FILE
 
   Read and set direcotry structure and ACLs from a YAML file.
 
 Options:
-  --help  Show this message and exit.
+  --auth-method [default|environment|workload|managedid|azurecli|azureps|azuredevcli]
+                                  Azure AD Authentication method
+  --auth-opt <TEXT TEXT>...       Keyword arguments to pass to Azure SDK
+                                  credential constructor
+  --help                          Show this message and exit.
 ```
+Options:
+ * `--auth-method` allows the user to choose from a Azure Python SDK [Authentication methods](#authentication-methods)
+ * `--auth-opt` keyword arguments to be passed to the Azure Python SDK authentication constructors. Can be used multiple times in a call.
 
 To set acls from an input file `test.yml` the shell command would look like:
 ```bash
 adls-acl set-acl test.yml
 ```
 
 #### `get-acl` command
 ```
 Usage: adls-acl get-acl [OPTIONS] ACCOUNT_NAME OUTFILE
 
   Read the current fs and acls on dirs.
 
 Options:
-  --omit-special        Omit special ACLs when reading the account.
-  --help                Show this message and exit.
+  --omit-special                  Omit special ACLs when reading the account.
+  --auth-method [default|environment|workload|managedid|azurecli|azureps|azuredevcli]
+                                  Azure AD Authentication method
+  --auth-opt <TEXT TEXT>...       Keyword arguments to pass to Azure SDK
+                                  credential constructor
+  --help                          Show this message and exit.
 ```
 
 This will print the current filesystem of an account (directories only, no files) and their ACLs to a file on a path pass as `OUTFILE` argument.
-[Special ACLs](#special-acls) can be omitted with a flag `--omit-special`
+Options:
+ * `--omit-special` [Special ACLs](#special-acls) can be omitted and not printed to the output file 
+ * `--auth-method` allows the user to choose from a Azure Python SDK [Authentication methods](#authentication-methods)
+ * `--auth-opt` keyword arguments to be passed to the Azure Python SDK authentication constructors. Can be used multiple times in a call. 
+
 
 To read ACLs of a ADLS storage account named `testaccount` to file `dump.yml`:
 ```bash
 adls-acl get-acl testaccount dump.yml
 ```
 
 ### Input file
@@ -248,7 +267,26 @@
 
 The default ACLs defined or set on the higher level directories are pushed down to subdirectories specified in the input file.
 They will not be set on any files that had existed in the directories prior to the execution of `adls-acl`.
 Moreover, any subdirectories that exist in the account but are not specified in the input file remain untouched by `adls-acl`.
 
 Future releases will allow for more control over this behaviour (i.e, updating default ACLs on all files created prior to the change of ACLs).
 
+### Authentication Methods
+
+The Azure Python SDK authentication is by default handled with [`DefaultAzureCredenial`](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.defaultazurecredential?view=azure-python).
+
+In addition, a user can target one of the supported Azure Python SDK, by using `--auth-method` option:
+
+- [`EnvironmentCredential`](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.defaultazurecredential?view=azure-python)
+- [`WorkloadIdentityCredential`](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.workloadidentitycredential?view=azure-python)
+- [`ManagedIdentityCredential`](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.managedidentitycredential?view=azure-python)
+- [`AzureCliCrendtial`](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.azureclicredential?view=azure-python)
+- [`AzurePowerShellCrendeital`](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.azurepowershellcredential?view=azure-python)
+- [`AzureDevleoperCliCredential`](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.azurepowershellcredential?view=azure-python)
+
+To pass keyword arguments to the credential constructs use `--auth-opt` option. This option can be used multiple times, one instance per keyword argument. 
+
+e.g. to pass `managed_identity_client_id` and `exclude_cli_credential` to `DefaultAzureCredental`:
+```
+--auth-method default --auth-opt managed_identity_client_id xxxx-xxxx-xxxxx --auth-opt exlcude_cli_credential False
+```
```

### Comparing `adls_acl-0.0.5/tests/test_nodes.py` & `adls_acl-0.0.6/tests/test_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-import pytest, copy
+import copy
+
+import pytest
+
 from adls_acl import nodes
 
 
 @pytest.fixture(scope="module")
 def container_dict():
     return {
         "name": "test_container",
```

### Comparing `adls_acl-0.0.5/tests/test_orchestrator.py` & `adls_acl-0.0.6/tests/test_orchestrator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,21 @@
+from unittest.mock import call
+
+import azure.identity
+import azure.storage.filedatalake
 import pytest
+
 from adls_acl import orchestrator as o
 from adls_acl.nodes import Acl, Node
-import azure.storage.filedatalake
-import azure.identity
-from unittest.mock import call
 
 
 def test_processor_selector():
     pass
 
 
-def test__get_service_client_token_credential():
-    sc = o._get_service_client_token_credential("test")
-
-    assert isinstance(
-        sc, azure.storage.filedatalake._data_lake_service_client.DataLakeServiceClient
-    )
-    assert sc.account_name == "test"
-
-
 @pytest.fixture
 def mock_client(mocker):
     """Mock DataLakeDirectoryClient"""
     mock_client = mocker.patch(
         "azure.storage.filedatalake.DataLakeDirectoryClient",
         autospec=True,
     )
@@ -47,14 +40,19 @@
 
 def test__get_current_acls(mock_client):
     current_acls = o._get_current_acls(mock_client)
 
     assert len(current_acls) == 2
 
 
+def test__get_current_acl_no_special(mock_client):
+    curent_acls = o._get_current_acls(mock_client, True)
+    assert len(curent_acls) == 1
+
+
 def test__filter_acls_to_preserve(test_acl_set):
     acls_to_preserve = o._filter_acls_to_preserve(test_acl_set)
 
     assert len(acls_to_preserve) == 1
 
 
 def test__set_acls(mock_client, test_acl_set):
```

