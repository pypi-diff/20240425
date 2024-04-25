# Comparing `tmp/poetry_plugin_lambda_build-0.3.0.tar.gz` & `tmp/poetry_plugin_lambda_build-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_lambda_build-0.3.0.tar", max compression
+gzip compressed data, was "poetry_plugin_lambda_build-0.4.1.tar", max compression
```

## Comparing `poetry_plugin_lambda_build-0.3.0.tar` & `poetry_plugin_lambda_build-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2024-04-24 17:32:04.499768 poetry_plugin_lambda_build-0.3.0/LICENSE
--rw-r--r--   0        0        0     5785 2024-04-24 17:32:04.499768 poetry_plugin_lambda_build-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-04-24 17:32:04.499768 poetry_plugin_lambda_build-0.3.0/poetry_plugin_lambda_build/__init__.py
--rw-r--r--   0        0        0     2134 2024-04-24 17:32:04.499768 poetry_plugin_lambda_build-0.3.0/poetry_plugin_lambda_build/docker.py
--rw-r--r--   0        0        0     7165 2024-04-24 17:32:04.499768 poetry_plugin_lambda_build-0.3.0/poetry_plugin_lambda_build/plugin.py
--rw-r--r--   0        0        0     6724 2024-04-24 17:32:04.499768 poetry_plugin_lambda_build-0.3.0/poetry_plugin_lambda_build/recipes.py
--rw-r--r--   0        0        0      257 2024-04-24 17:32:04.499768 poetry_plugin_lambda_build-0.3.0/poetry_plugin_lambda_build/utils.py
--rw-r--r--   0        0        0      652 2024-04-24 17:32:04.499768 poetry_plugin_lambda_build-0.3.0/poetry_plugin_lambda_build/zip.py
--rw-r--r--   0        0        0      707 2024-04-24 17:32:04.499768 poetry_plugin_lambda_build-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6496 1970-01-01 00:00:00.000000 poetry_plugin_lambda_build-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-25 09:58:26.300745 poetry_plugin_lambda_build-0.4.1/LICENSE
+-rw-r--r--   0        0        0     5598 2024-04-25 09:58:26.300745 poetry_plugin_lambda_build-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-25 09:58:26.300745 poetry_plugin_lambda_build-0.4.1/poetry_plugin_lambda_build/__init__.py
+-rw-r--r--   0        0        0     2134 2024-04-25 09:58:26.300745 poetry_plugin_lambda_build-0.4.1/poetry_plugin_lambda_build/docker.py
+-rw-r--r--   0        0        0     6613 2024-04-25 09:58:26.300745 poetry_plugin_lambda_build-0.4.1/poetry_plugin_lambda_build/plugin.py
+-rw-r--r--   0        0        0     7660 2024-04-25 09:58:26.300745 poetry_plugin_lambda_build-0.4.1/poetry_plugin_lambda_build/recipes.py
+-rw-r--r--   0        0        0      257 2024-04-25 09:58:26.300745 poetry_plugin_lambda_build-0.4.1/poetry_plugin_lambda_build/utils.py
+-rw-r--r--   0        0        0      652 2024-04-25 09:58:26.300745 poetry_plugin_lambda_build-0.4.1/poetry_plugin_lambda_build/zip.py
+-rw-r--r--   0        0        0      707 2024-04-25 09:58:26.300745 poetry_plugin_lambda_build-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6309 1970-01-01 00:00:00.000000 poetry_plugin_lambda_build-0.4.1/PKG-INFO
```

### Comparing `poetry_plugin_lambda_build-0.3.0/LICENSE` & `poetry_plugin_lambda_build-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.3.0/README.md` & `poetry_plugin_lambda_build-0.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -79,37 +79,37 @@
 ```
 
 ```
 Description:
   Execute to build lambda lambda artifacts
 
 Usage:
-  build-lambda [options] [--] [<docker_image> [<docker_entrypoint> [<docker_environment> [<docker_dns> [<docker_network> [<docker_network_disabled> [<docker_network_mode> [<package_install_dir> [<layer_install_dir> [<function_install_dir> [<package_artifact_path> [<layer_artifact_path> [<function_artifact_path> [<only> [<without> [<with> [<install_deps_cmd> [<install_no_deps_cmd> [<install_package_cmd>]]]]]]]]]]]]]]]]]]]
+  build-lambda [options] [--] [<docker_image> [<docker_entrypoint> [<docker_environment> [<docker_dns> [<docker_network> [<docker_network_disabled> [<docker_network_mode> [<docker_platform> [<package_install_dir> [<layer_install_dir> [<function_install_dir> [<install_dir> [<package_artifact_path> [<layer_artifact_path> [<function_artifact_path> [<only> [<without> [<with> [<install_deps_cmd> [<install_no_deps_cmd>]]]]]]]]]]]]]]]]]]]]
 
 Arguments:
   docker_image               The image to run
   docker_entrypoint          The entrypoint for the container (comma separated string)
   docker_environment         Environment variables to set inside the container (comma separated string) ex. VAR_1=VALUE_1,VAR_2=VALUE_2
   docker_dns                 Set custom DNS servers (comma separated string)
   docker_network             The name of the network this container will be connected to at creation time
   docker_network_disabled    Disable networking ex. docker_network_disabled=0
   docker_network_mode        Network_mode
   docker_platform            Platform in the format os[/arch[/variant]]. Only used if the method needs to pull the requested image.
   package_install_dir        Installation directory inside zip artifact for single zip package
   layer_install_dir          Installation directory inside zip artifact for layer zip package
   function_install_dir       Installation directory inside zip artifact for function zip package
+  install_dir                Installation directory inside zip artifact for zip package (not function layer separation)
   package_artifact_path      Output package path
   layer_artifact_path        Output layer package path
   function_artifact_path     Output function package path
   only                       The only dependency groups to include
   without                    The dependency groups to ignore
   with                       The optional dependency groups to include
   install_deps_cmd           Install dependencies command. Executed during installation of dependencies layer, by default: mkdir -p {container_cache_dir} && pip install -q --upgrade pip && pip install -q -t {container_cache_dir} --no-cache-dir -r {requirements}
   install_no_deps_cmd        Install without dependencies command. Executed during installation of function, by default: mkdir -p {package_dir} && poetry run pip install --quiet -t {package_dir} --no-cache-dir --no-deps . --upgrade
-  install_package_cmd        Install package command. Executed during installation of package without function-layer separation, by default: mkdir -p {package_dir} && pip install poetry --quiet --upgrade pip && poetry build --quiet && poetry run pip install --quiet -t {package_dir} --no-cache-dir dist/*.whl --upgrade
 
 Options:
   -h, --help                 Display help for the given command. When no command is given display help for the list command.
   -q, --quiet                Do not output any message.
   -V, --version              Display this application version.
       --ansi                 Force ANSI output.
       --no-ansi              Disable ANSI output.
```

### Comparing `poetry_plugin_lambda_build-0.3.0/poetry_plugin_lambda_build/docker.py` & `poetry_plugin_lambda_build-0.4.1/poetry_plugin_lambda_build/docker.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.3.0/poetry_plugin_lambda_build/plugin.py` & `poetry_plugin_lambda_build-0.4.1/poetry_plugin_lambda_build/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,33 +17,24 @@
 )
 
 INSTALL_NO_DEPS_CMD = (
     "mkdir -p {package_dir} && poetry run pip install"
     " --quiet -t {package_dir} --no-cache-dir --no-deps . --upgrade"
 )
 
-INSTALL_PACKAGE_CMD = (
-    "mkdir -p {package_dir} && "
-    "pip install poetry --quiet --upgrade pip && "
-    "poetry build --quiet && "
-    "poetry run pip install --quiet -t {package_dir} --no-cache-dir dist/*.whl --upgrade"
-)
-
 DEFAULT_PARAMETERS = {
     "docker_entrypoint": "/bin/sh",
     "docker_network": "host",
     "docker_options": [],
     "artifact_path": "package.zip",
-    "install_package_cmd": INSTALL_PACKAGE_CMD,
     "install_no_deps_cmd": INSTALL_NO_DEPS_CMD,
     "install_deps_cmd": INSTALL_DEPS_CMD,
     "without": None,
     "only": None,
     "with": None,
-    "config": [],
 }
 
 
 class BuildType(enum.Enum):
     IN_CONTAINER_MERGED = enum.auto()
     IN_CONTAINER_SEPARATED = enum.auto()
     MERGED = enum.auto()
@@ -83,16 +74,14 @@
     "layer_artifact_path": ("Output layer package path", True, False, None),
     "function_artifact_path": ("Output function package path", True, False, None),
     "only": ("The only dependency groups to include", True, False, None),
     "without": ("The dependency groups to ignore", True, False, None),
     "with": ("The optional dependency groups to include", True, False, None),
     "install_deps_cmd": (f"Install dependencies command. Executed during installation of dependencies layer, by default: {INSTALL_DEPS_CMD}", True, False, None),
     "install_no_deps_cmd": (f"Install without dependencies command. Executed during installation of function, by default: {INSTALL_NO_DEPS_CMD}", True, False, None),
-    "install_package_cmd": (f"Install package command. Executed during installation of package without function-layer separation, by default: {INSTALL_PACKAGE_CMD}", True, False, None),
-    "config": ("Manages configuration settings.", True, True, None)
 }
 
 ARGS_SECTIONS = ("layer", "function", "docker", "artifacts")
 
 
 class ParametersContainer(dict):
     args = ARGS
```

### Comparing `poetry_plugin_lambda_build-0.3.0/poetry_plugin_lambda_build/recipes.py` & `poetry_plugin_lambda_build-0.4.1/poetry_plugin_lambda_build/recipes.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,68 +24,67 @@
         shell=True,
         stdin=None,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     )
     output, err = process.communicate()
     if process.returncode == 0:
-        self.line_error(err.decode("utf-8"), style="warning")
-        return output
+        self.line_error(err.decode(), style="warning")
+        return output.decode()
     elif process.returncode == 1:
-        self.line_error(err.decode("utf-8"), style="error")
+        self.line_error(err.decode(), style="error")
 
-    raise BuildLambdaPluginError(output.decode("utf-8"))
+    raise BuildLambdaPluginError(output.decode())
+
+
+def _parse_poetry_export_cmd(parameters: dict) -> str:
+    poetry_export_cmd = "poetry export --format=requirements.txt --with-credentials"
+    if parameters["without"]:
+        poetry_export_cmd += f" --without={parameters['without']}"
+    if parameters["with"]:
+        poetry_export_cmd += f" --with={parameters['with']}"
+    if parameters["only"]:
+        poetry_export_cmd += f" --only={parameters['only']}"
+    return poetry_export_cmd
 
 
 def create_separate_layer_package(
     self: EnvCommand, parameters: dict, in_container: bool = True
 ):
     with TemporaryDirectory() as tmp_dir:
         install_dir = parameters.get("layer_install_dir", "")
         layer_output_dir = os.path.join(tmp_dir, "layer_output")
 
         target = os.path.join(
             CURRENT_WORK_DIR, parameters.get("layer_artifact_path", "")
         )
         requirements_path = os.path.join(tmp_dir, "requirements.txt")
-
-        poetry_export_cmd = "poetry export --format=requirements.txt"
-
-        if parameters["without"]:
-            poetry_export_cmd += f" --without={parameters['without']}"
-
-        if parameters["with"]:
-            poetry_export_cmd += f" --with={parameters['with']}"
-
-        if parameters["only"]:
-            poetry_export_cmd += f" --only={parameters['only']}"
-
-        if install_dir:
-            layer_output_dir = os.path.join(layer_output_dir, install_dir)
+        poetry_export_cmd = _parse_poetry_export_cmd(parameters)
+        layer_output_dir = os.path.join(layer_output_dir, install_dir)
 
         self.line("Generating requirements file...", style="info")
         self.line(f"Executing: {poetry_export_cmd}", style="debug")
 
         output = _run_process(self, poetry_export_cmd)
 
         with open(requirements_path, "w") as f:
-            f.write(output.decode("utf-8"))
+            f.write(output)
 
         if in_container:
             with run_container(self, **parameters.get_section("docker")) as container:
                 copy_to(requirements_path, f"{container.id}:/requirements.txt")
                 self.line("Installing requirements", style="info")
                 install_deps_cmd = parameters["install_deps_cmd"].format(
                     container_cache_dir=CONTAINER_CACHE_DIR,
                     requirements="/requirements.txt",
                 )
                 result = container.exec_run(
                     f'sh -c "{install_deps_cmd}"', stream=True)
                 for line in result.output:
-                    self.line(line.strip().decode("utf-8"), style="info")
+                    self.line(line.strip().decode(), style="info")
                 self.line(f"Coping output to {layer_output_dir}", style="info")
                 os.makedirs(layer_output_dir, exist_ok=True)
                 copy_from(f"{container.id}:{CONTAINER_CACHE_DIR}/.",
                           layer_output_dir)
         else:
             install_deps_cmd = parameters["install_deps_cmd"].format(
                 container_cache_dir=layer_output_dir, requirements=requirements_path
@@ -94,18 +93,17 @@
             self.line("Installing requirements", style="info")
             self.line(f"Executing: {install_deps_cmd}", style="debug")
             _run_process(self, install_deps_cmd)
 
         self.line(f"Building {target}...", style="info")
         os.makedirs(os.path.dirname(target), exist_ok=True)
         create_zip_package(
-            remove_suffix(layer_output_dir, install_dir)
-            if install_dir
-            else layer_output_dir,
-            target,
+            dir=remove_suffix(layer_output_dir, install_dir),
+            output=target,
+            exclude=["*.pyc", "*__pycache__/*", requirements_path]
         )
         self.line(f"target successfully built: {target}...", style="info")
 
 
 def create_separated_function_package(self: EnvCommand, parameters: dict):
     with TemporaryDirectory() as tmp_dir:
         install_dir = parameters.get("function_install_dir", "")
@@ -123,57 +121,72 @@
         self.line(f"Executing: {install_cmd}", style="debug")
 
         _run_process(self, install_cmd)
 
         self.line(f"Building target: {target}", style="info")
         os.makedirs(os.path.dirname(target), exist_ok=True)
         create_zip_package(
-            remove_suffix(package_dir, install_dir),
-            target,
+            dir=remove_suffix(package_dir, install_dir),
+            output=target,
         )
         self.line(f"target successfully built: {target}...", style="info")
 
 
 def create_package(self: EnvCommand, parameters: dict, in_container: bool = True):
-    current_working_directory = os.getcwd()
     with TemporaryDirectory() as package_dir:
         install_dir = parameters.get("install_dir", "")
-
-        if install_dir:
-            package_dir = os.path.join(package_dir, install_dir)
-
+        package_dir = os.path.join(package_dir, install_dir)
+        os.makedirs(package_dir, exist_ok=True)
         target = os.path.join(
-            current_working_directory, parameters.get("artifact_path", "")
+            CURRENT_WORK_DIR, parameters.get("artifact_path", "")
         )
+        requirements_path = os.path.join(package_dir, "requirements.txt")
+        poetry_export_cmd = _parse_poetry_export_cmd(parameters)
+        self.line("Generating requirements file...", style="info")
+        self.line(f"Executing: {poetry_export_cmd}", style="debug")
+        output = _run_process(self, poetry_export_cmd)
+
+        with open(requirements_path, "w") as f:
+            f.write(output)
+
         if in_container:
-            self.line("Building package in container", style="info")
             with run_container(self, **parameters.get_section("docker")) as container:
+                copy_to(requirements_path, f"{container.id}:/requirements.txt")
+                self.line("Installing requirements", style="info")
+                install_deps_cmd = parameters["install_deps_cmd"].format(
+                    container_cache_dir=CONTAINER_CACHE_DIR,
+                    requirements="/requirements.txt",
+                )
+                self.line(f"Executing: {install_deps_cmd}", style="debug")
 
-                for config in parameters["config"]:
-                    result = container.exec_run(
-                        f'poetry config {config}', stream=True)
-                    for line in result.output:
-                        self.line(line.strip().decode("utf-8"), style="info")
-
-                cmd = parameters["install_package_cmd"].format(
-                    package_dir=package_dir)
-                self.line(f"Executing: {cmd}", style="debug")
-                result = container.exec_run(f'sh -c "{cmd}"', stream=True)
-
+                result = container.exec_run(
+                    f'sh -c "{install_deps_cmd}"', stream=True
+                )
                 for line in result.output:
-                    self.line(line.strip().decode("utf-8"), style="info")
-
-                copy_from(f"{container.id}:{package_dir}/.", package_dir)
+                    self.line(line.strip().decode(), style="info")
+                self.line(f"Coping output to {package_dir}", style="info")
+                copy_from(
+                    src=f"{container.id}:{CONTAINER_CACHE_DIR}/.",
+                    dst=package_dir
+                )
         else:
+            install_deps_cmd = parameters["install_deps_cmd"].format(
+                container_cache_dir=package_dir,
+                requirements=requirements_path
+            )
             self.line("Building package on local", style="info")
-            cmd = parameters["install_package_cmd"].format(
-                package_dir=package_dir)
-            self.line(f"Executing: {cmd}", style="debug")
-            _run_process(self, cmd)
+            self.line(f"Executing: {install_deps_cmd}", style="debug")
+            _run_process(self, install_deps_cmd)
 
+        install_cmd = parameters["install_no_deps_cmd"].format(
+            package_dir=package_dir)
+
+        os.chdir(CURRENT_WORK_DIR)
+        self.line(f"Executing: {install_cmd}", style="debug")
+        _run_process(self, install_cmd)
         os.makedirs(os.path.dirname(target), exist_ok=True)
         create_zip_package(
-            remove_suffix(
-                package_dir, install_dir) if install_dir else package_dir,
-            target,
+            dir=remove_suffix(package_dir, install_dir),
+            output=target,
+            exclude=["*.pyc", "*__pycache__/*", requirements_path]
         )
         self.line(f"target successfully built: {target}...", style="info")
```

### Comparing `poetry_plugin_lambda_build-0.3.0/poetry_plugin_lambda_build/zip.py` & `poetry_plugin_lambda_build-0.4.1/poetry_plugin_lambda_build/zip.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.3.0/pyproject.toml` & `poetry_plugin_lambda_build-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-lambda-build"
-version = "0.3.0"
+version = "0.4.1"
 description = "The plugin for poetry that allows you to build zip packages suited for serverless deployment like AWS Lambda, Google App Engine, Azure App Service, and more..."
 authors = ["Michał Murawski <mmurawski777@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 docker = "^7.0.0"
```

### Comparing `poetry_plugin_lambda_build-0.3.0/PKG-INFO` & `poetry_plugin_lambda_build-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-lambda-build
-Version: 0.3.0
+Version: 0.4.1
 Summary: The plugin for poetry that allows you to build zip packages suited for serverless deployment like AWS Lambda, Google App Engine, Azure App Service, and more...
 Author: Michał Murawski
 Author-email: mmurawski777@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -95,37 +95,37 @@
 ```
 
 ```
 Description:
   Execute to build lambda lambda artifacts
 
 Usage:
-  build-lambda [options] [--] [<docker_image> [<docker_entrypoint> [<docker_environment> [<docker_dns> [<docker_network> [<docker_network_disabled> [<docker_network_mode> [<package_install_dir> [<layer_install_dir> [<function_install_dir> [<package_artifact_path> [<layer_artifact_path> [<function_artifact_path> [<only> [<without> [<with> [<install_deps_cmd> [<install_no_deps_cmd> [<install_package_cmd>]]]]]]]]]]]]]]]]]]]
+  build-lambda [options] [--] [<docker_image> [<docker_entrypoint> [<docker_environment> [<docker_dns> [<docker_network> [<docker_network_disabled> [<docker_network_mode> [<docker_platform> [<package_install_dir> [<layer_install_dir> [<function_install_dir> [<install_dir> [<package_artifact_path> [<layer_artifact_path> [<function_artifact_path> [<only> [<without> [<with> [<install_deps_cmd> [<install_no_deps_cmd>]]]]]]]]]]]]]]]]]]]]
 
 Arguments:
   docker_image               The image to run
   docker_entrypoint          The entrypoint for the container (comma separated string)
   docker_environment         Environment variables to set inside the container (comma separated string) ex. VAR_1=VALUE_1,VAR_2=VALUE_2
   docker_dns                 Set custom DNS servers (comma separated string)
   docker_network             The name of the network this container will be connected to at creation time
   docker_network_disabled    Disable networking ex. docker_network_disabled=0
   docker_network_mode        Network_mode
   docker_platform            Platform in the format os[/arch[/variant]]. Only used if the method needs to pull the requested image.
   package_install_dir        Installation directory inside zip artifact for single zip package
   layer_install_dir          Installation directory inside zip artifact for layer zip package
   function_install_dir       Installation directory inside zip artifact for function zip package
+  install_dir                Installation directory inside zip artifact for zip package (not function layer separation)
   package_artifact_path      Output package path
   layer_artifact_path        Output layer package path
   function_artifact_path     Output function package path
   only                       The only dependency groups to include
   without                    The dependency groups to ignore
   with                       The optional dependency groups to include
   install_deps_cmd           Install dependencies command. Executed during installation of dependencies layer, by default: mkdir -p {container_cache_dir} && pip install -q --upgrade pip && pip install -q -t {container_cache_dir} --no-cache-dir -r {requirements}
   install_no_deps_cmd        Install without dependencies command. Executed during installation of function, by default: mkdir -p {package_dir} && poetry run pip install --quiet -t {package_dir} --no-cache-dir --no-deps . --upgrade
-  install_package_cmd        Install package command. Executed during installation of package without function-layer separation, by default: mkdir -p {package_dir} && pip install poetry --quiet --upgrade pip && poetry build --quiet && poetry run pip install --quiet -t {package_dir} --no-cache-dir dist/*.whl --upgrade
 
 Options:
   -h, --help                 Display help for the given command. When no command is given display help for the list command.
   -q, --quiet                Do not output any message.
   -V, --version              Display this application version.
       --ansi                 Force ANSI output.
       --no-ansi              Disable ANSI output.
```

