# Comparing `tmp/openshift_cluster_login-1.0.4.tar.gz` & `tmp/openshift_cluster_login-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openshift_cluster_login-1.0.4.tar", max compression
+gzip compressed data, was "openshift_cluster_login-1.0.5.tar", max compression
```

## Comparing `openshift_cluster_login-1.0.4.tar` & `openshift_cluster_login-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1073 2024-04-18 07:52:42.410214 openshift_cluster_login-1.0.4/LICENSE
--rw-r--r--   0        0        0     5190 2024-04-18 07:52:42.410214 openshift_cluster_login-1.0.4/README.md
--rw-r--r--   0        0        0        0 2024-04-18 07:52:42.418214 openshift_cluster_login-1.0.4/ocl/__init__.py
--rw-r--r--   0        0        0    14183 2024-04-18 07:52:42.418214 openshift_cluster_login-1.0.4/ocl/__main__.py
--rw-r--r--   0        0        0        0 2024-04-18 07:52:42.418214 openshift_cluster_login-1.0.4/ocl/gql_definitions/__init__.py
--rw-r--r--   0        0        0       97 2024-04-18 07:52:42.418214 openshift_cluster_login-1.0.4/ocl/gql_definitions/clusters.gql
--rw-r--r--   0        0        0     1728 2024-04-18 07:52:42.418214 openshift_cluster_login-1.0.4/ocl/gql_definitions/clusters.py
--rw-r--r--   0        0        0        0 2024-04-18 07:52:42.418214 openshift_cluster_login-1.0.4/ocl/gql_definitions/fragments/__init__.py
--rw-r--r--   0        0        0      152 2024-04-18 07:52:42.418214 openshift_cluster_login-1.0.4/ocl/gql_definitions/fragments/cluster.gql
--rw-r--r--   0        0        0     1095 2024-04-18 07:52:42.418214 openshift_cluster_login-1.0.4/ocl/gql_definitions/fragments/cluster.py
--rw-r--r--   0        0        0      145 2024-04-18 07:52:42.418214 openshift_cluster_login-1.0.4/ocl/gql_definitions/namespaces.gql
--rw-r--r--   0        0        0     1982 2024-04-18 07:52:42.418214 openshift_cluster_login-1.0.4/ocl/gql_definitions/namespaces.py
--rw-r--r--   0        0        0     2021 2024-04-18 07:52:42.418214 openshift_cluster_login-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     6273 1970-01-01 00:00:00.000000 openshift_cluster_login-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-25 08:32:45.702109 openshift_cluster_login-1.0.5/LICENSE
+-rw-r--r--   0        0        0     5120 2024-04-25 08:32:45.702109 openshift_cluster_login-1.0.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-25 08:32:45.710109 openshift_cluster_login-1.0.5/ocl/__init__.py
+-rw-r--r--   0        0        0    14243 2024-04-25 08:32:45.710109 openshift_cluster_login-1.0.5/ocl/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-25 08:32:45.710109 openshift_cluster_login-1.0.5/ocl/gql_definitions/__init__.py
+-rw-r--r--   0        0        0       97 2024-04-25 08:32:45.710109 openshift_cluster_login-1.0.5/ocl/gql_definitions/clusters.gql
+-rw-r--r--   0        0        0     1728 2024-04-25 08:32:45.710109 openshift_cluster_login-1.0.5/ocl/gql_definitions/clusters.py
+-rw-r--r--   0        0        0        0 2024-04-25 08:32:45.710109 openshift_cluster_login-1.0.5/ocl/gql_definitions/fragments/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-25 08:32:45.710109 openshift_cluster_login-1.0.5/ocl/gql_definitions/fragments/cluster.gql
+-rw-r--r--   0        0        0     1095 2024-04-25 08:32:45.710109 openshift_cluster_login-1.0.5/ocl/gql_definitions/fragments/cluster.py
+-rw-r--r--   0        0        0      145 2024-04-25 08:32:45.710109 openshift_cluster_login-1.0.5/ocl/gql_definitions/namespaces.gql
+-rw-r--r--   0        0        0     1982 2024-04-25 08:32:45.710109 openshift_cluster_login-1.0.5/ocl/gql_definitions/namespaces.py
+-rw-r--r--   0        0        0     2021 2024-04-25 08:32:45.710109 openshift_cluster_login-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6203 1970-01-01 00:00:00.000000 openshift_cluster_login-1.0.5/PKG-INFO
```

### Comparing `openshift_cluster_login-1.0.4/LICENSE` & `openshift_cluster_login-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openshift_cluster_login-1.0.4/README.md` & `openshift_cluster_login-1.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,72 @@
 ![logo](images/logo-white-bg.png)
+
 # OCL (OpenShift Login)
 
 [![PyPI](https://img.shields.io/pypi/v/openshift-cluster-login)][pypi-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 ![PyPI - License](https://img.shields.io/pypi/l/openshift-cluster-login)
 [![Release and Package Application](https://github.com/chassing/ocl/actions/workflows/release.yaml/badge.svg)](https://github.com/chassing/ocl/actions/workflows/release.yaml)
 
 OCL does an automatic login to an OpenShift cluster. It fetches cluster information from app-interface and performs a login via [Selenium](https://selenium-python.readthedocs.io).
 
 ## Installation
 
 You can install this library from [PyPI][pypi-link] with `pip`:
 
-
 ```shell
-$ python3 -m pip install openshift-cluster-login
+python3 -m pip install openshift-cluster-login
 ```
 
 or install it with `pipx`:
+
 ```shell
-$ pipx install openshift-cluster-login
+pipx install openshift-cluster-login
 ```
 
 You can also use `pipx` to run the library without installing it:
 
 ```shell
-$ pipx run openshift-cluster-login
+pipx run openshift-cluster-login
 ```
 
 ## Usage
 
 ```shell
-$ ocl
+ocl
 ```
 
 <img src="demo/quickstart.gif"/>
 
 This spawns a new shell with the following environment variables are set:
 
 * `KUBECONFIG` - path to kubeconfig file
 * `OCL_CLUSTER_NAME` - cluster name
 * `OCL_CLUSTER_CONSOLE` - url to cluster console
 
 ## Features
 
 OCL currently provides the following features (get help with `-h` or `--help`):
 
-- OpenShift console login (`oc login`) via GitHub or Red Hat authentication
-- Get cluster and namespace information from app-interface or user-defined (`OCL_USER_CLUSTERS``)
-_ Open the OpenShift `console in `the `browser`` (`--open-in-browser`)
-- Shell completion (`--install-completion`, `--show-completion`)
-- Credentials via environment variables or shell command (e.g., [1password CLI](https://developer.1password.com/docs/cli/))
-- Cache App-Interface queries (via GraphQL) for one week
-
+* OpenShift console login (`oc login`) via GitHub or Red Hat authentication
+* Get cluster and namespace information from app-interface or user-defined (`OCL_USER_CLUSTERS``)
+_ Open the OpenShift`console in `the`browser`` (`--open-in-browser`)
+* Shell completion (`--install-completion`, `--show-completion`)
+* Credentials via environment variables or shell command (e.g., [1password CLI](https://developer.1password.com/docs/cli/))
+* Cache App-Interface queries (via GraphQL) for one week
 
 ## Environment Variables
 
 | Variable Name                                       | Description                                                                                                                                 | Default |
 | --------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | ------- |
 | OCL_WAIT OCL_WAIT_COMMAND                           | Selenium webdriver wait timeout                                                                                                             | 2       |
 | OCL_APP_INTERFACE_URL OCL_APP_INTERFACE_URL_COMMAND | App-Interface URL                                                                                                                           |         |
-| OCL_APP_INT_TOKEN OCL_APP_INT_TOKEN_COMMAND         | App-Interface authentication token                                                                                                          |         |
-| USER_CLUSTERS USER_CLUSTERS_COMMAND                 | User defined clusters as json format (e.g. `[{"name": "local-kind", "serverUrl": "https://localhost:6443", "consoleUrl": "not available}]`) | "[]"    |
+| OCL_APP_INT_TOKEN OCL_APP_INT_TOKEN_COMMAND         | App-Interface authentication token [optional]                                                                                               |         |
+| OCL_USER_CLUSTERS OCL_USER_CLUSTERS_COMMAND         | User defined clusters as json format (e.g. `[{"name": "local-kind", "serverUrl": "https://localhost:6443", "consoleUrl": "not available}]`) | "[]"    |
+| OCL_CACHE_TIMEOUT_MINUTES                           | GraphQL cache timeout in minutes                                                                                                            | 1 hour  |
 
 You can either set a variable, e.g. `export OCL_GITHUB_USERNAME="mail@example.com"` or retrieve it via a command, e.g. `export OCL_GITHUB_USERNAME_COMMAND="op read op://Private/Github/username"`.
 If a variable is not set but needed, OCL will ask for it interactively.
 
 ## App-Interface
 
 OCL retrieves the cluster information from app-interface via GraphQL (`OCL_APP_INTERFACE_URL`) and caches them
@@ -78,15 +79,14 @@
 * Works only with a Red Hat associate account
 
 ## Development
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 
-
 Use [Conventional Commit messages](https://www.conventionalcommits.org).
 The most important prefixes you should have in mind are:
 
 * `fix:` which represents bug fixes, and correlates to a [SemVer](https://semver.org/)
   patch.
 * `feat:` which represents a new feature, and correlates to a SemVer minor.
 * `feat!:`,  or `fix!:`, `refactor!:`, etc., which represent a breaking change
@@ -96,17 +96,14 @@
 Consider using an empty commit:
 
 ```
 git commit --allow-empty -m "chore: release"
 ```
 
 When a commit to the main branch has `Release-As: x.x.x` (case insensitive) in the **commit body**, Release Please will open a new pull request for the specified version.
+
 ```
 git commit --allow-empty -m "chore: release 2.0.0" -m "Release-As: 2.0.0"
 ```
 
-
-[github-discussions-badge]: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
-[github-discussions-link]:  https://github.com/chassing/ocl/discussions
 [pypi-link]:                https://pypi.org/project/openshift-cluster-login/
 [pypi-platforms]:           https://img.shields.io/pypi/pyversions/openshift-cluster-login
-[pypi-version]:             https://badge.fury.io/py/openshift-cluster-login.svg
```

### Comparing `openshift_cluster_login-1.0.4/ocl/__main__.py` & `openshift_cluster_login-1.0.5/ocl/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 from ocl.gql_definitions.namespaces import query as namespaces_query
 
 appdirs = AppDirs("ocl", "ca-net")
 lock_file_name = Path(tempfile.gettempdir()) / "ocl.lock"
 lock = Lock(str(lock_file_name), lifetime=60, default_timeout=65)
 cache = Cache(directory=str(Path(appdirs.user_cache_dir) / "gql_cache"))
 
-ONE_WEEK = 7 * 24 * 60 * 60
 BANNER = """
             ';cloooolc;'            ';clloooolc;'        ':lll:'
           ;d0NWMMMMMMWN0d;        ;d0NWMMMMMMMWN0d;      oNMMMXc
          cKMMMMMMMMMMMMMMKl      cKWMMMMMMMMMMMMMWKl     oNMMMXl
         ;0MMMMXkllloONMMMMXc    ;0MMMMX0klclokNMMMMXc    oNMMMNl
         dWMMMNo      dNMMMWx'   oNMMMNo'      oNMMMWx'   oWMMMNl
        'kMMMM0;      ;KMMMMO,  'kMMMM0;       'ldddd:    dWMMMNl
@@ -134,15 +133,19 @@
             headers["Authorization"] = token
         res = requests.post(
             url=get_var("APP_INTERFACE_URL"),
             json={"query": query},
             headers=headers,
         )
         res.raise_for_status()
-        cache.set(checksum, res.json()["data"], expire=ONE_WEEK)
+        cache.set(
+            checksum,
+            res.json()["data"],
+            expire=get_var("CACHE_TIMEOUT_MINUTES", default=60) * 60,
+        )
     return cache[checksum]
 
 
 def clusters_from_app_interface() -> list[Cluster]:
     clusters = clusters_query(query_func=gql_query).clusters or []
     return [c for c in clusters if c.auth]
```

### Comparing `openshift_cluster_login-1.0.4/ocl/gql_definitions/clusters.py` & `openshift_cluster_login-1.0.5/ocl/gql_definitions/clusters.py`

 * *Files identical despite different names*

### Comparing `openshift_cluster_login-1.0.4/ocl/gql_definitions/fragments/cluster.py` & `openshift_cluster_login-1.0.5/ocl/gql_definitions/fragments/cluster.py`

 * *Files identical despite different names*

### Comparing `openshift_cluster_login-1.0.4/ocl/gql_definitions/namespaces.py` & `openshift_cluster_login-1.0.5/ocl/gql_definitions/namespaces.py`

 * *Files identical despite different names*

### Comparing `openshift_cluster_login-1.0.4/pyproject.toml` & `openshift_cluster_login-1.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openshift-cluster-login"
-version = "1.0.4"
+version = "1.0.5"
 description = "Openshift cluster login on command line"
 authors = ["Christian Assing <cassing@redhat.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "http://github.com/chassing/ocl"
 packages = [{ include = "ocl" }]
```

### Comparing `openshift_cluster_login-1.0.4/PKG-INFO` & `openshift_cluster_login-1.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-cluster-login
-Version: 1.0.4
+Version: 1.0.5
 Summary: Openshift cluster login on command line
 Home-page: http://github.com/chassing/ocl
 License: MIT
 Author: Christian Assing
 Author-email: cassing@redhat.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -23,77 +23,78 @@
 Requires-Dist: requests-kerberos (>=0.14.0,<0.15.0)
 Requires-Dist: rich (>=12.5.1,<13.0.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
 Project-URL: Repository, http://github.com/chassing/ocl
 Description-Content-Type: text/markdown
 
 ![logo](images/logo-white-bg.png)
+
 # OCL (OpenShift Login)
 
 [![PyPI](https://img.shields.io/pypi/v/openshift-cluster-login)][pypi-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 ![PyPI - License](https://img.shields.io/pypi/l/openshift-cluster-login)
 [![Release and Package Application](https://github.com/chassing/ocl/actions/workflows/release.yaml/badge.svg)](https://github.com/chassing/ocl/actions/workflows/release.yaml)
 
 OCL does an automatic login to an OpenShift cluster. It fetches cluster information from app-interface and performs a login via [Selenium](https://selenium-python.readthedocs.io).
 
 ## Installation
 
 You can install this library from [PyPI][pypi-link] with `pip`:
 
-
 ```shell
-$ python3 -m pip install openshift-cluster-login
+python3 -m pip install openshift-cluster-login
 ```
 
 or install it with `pipx`:
+
 ```shell
-$ pipx install openshift-cluster-login
+pipx install openshift-cluster-login
 ```
 
 You can also use `pipx` to run the library without installing it:
 
 ```shell
-$ pipx run openshift-cluster-login
+pipx run openshift-cluster-login
 ```
 
 ## Usage
 
 ```shell
-$ ocl
+ocl
 ```
 
 <img src="demo/quickstart.gif"/>
 
 This spawns a new shell with the following environment variables are set:
 
 * `KUBECONFIG` - path to kubeconfig file
 * `OCL_CLUSTER_NAME` - cluster name
 * `OCL_CLUSTER_CONSOLE` - url to cluster console
 
 ## Features
 
 OCL currently provides the following features (get help with `-h` or `--help`):
 
-- OpenShift console login (`oc login`) via GitHub or Red Hat authentication
-- Get cluster and namespace information from app-interface or user-defined (`OCL_USER_CLUSTERS``)
-_ Open the OpenShift `console in `the `browser`` (`--open-in-browser`)
-- Shell completion (`--install-completion`, `--show-completion`)
-- Credentials via environment variables or shell command (e.g., [1password CLI](https://developer.1password.com/docs/cli/))
-- Cache App-Interface queries (via GraphQL) for one week
-
+* OpenShift console login (`oc login`) via GitHub or Red Hat authentication
+* Get cluster and namespace information from app-interface or user-defined (`OCL_USER_CLUSTERS``)
+_ Open the OpenShift`console in `the`browser`` (`--open-in-browser`)
+* Shell completion (`--install-completion`, `--show-completion`)
+* Credentials via environment variables or shell command (e.g., [1password CLI](https://developer.1password.com/docs/cli/))
+* Cache App-Interface queries (via GraphQL) for one week
 
 ## Environment Variables
 
 | Variable Name                                       | Description                                                                                                                                 | Default |
 | --------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | ------- |
 | OCL_WAIT OCL_WAIT_COMMAND                           | Selenium webdriver wait timeout                                                                                                             | 2       |
 | OCL_APP_INTERFACE_URL OCL_APP_INTERFACE_URL_COMMAND | App-Interface URL                                                                                                                           |         |
-| OCL_APP_INT_TOKEN OCL_APP_INT_TOKEN_COMMAND         | App-Interface authentication token                                                                                                          |         |
-| USER_CLUSTERS USER_CLUSTERS_COMMAND                 | User defined clusters as json format (e.g. `[{"name": "local-kind", "serverUrl": "https://localhost:6443", "consoleUrl": "not available}]`) | "[]"    |
+| OCL_APP_INT_TOKEN OCL_APP_INT_TOKEN_COMMAND         | App-Interface authentication token [optional]                                                                                               |         |
+| OCL_USER_CLUSTERS OCL_USER_CLUSTERS_COMMAND         | User defined clusters as json format (e.g. `[{"name": "local-kind", "serverUrl": "https://localhost:6443", "consoleUrl": "not available}]`) | "[]"    |
+| OCL_CACHE_TIMEOUT_MINUTES                           | GraphQL cache timeout in minutes                                                                                                            | 1 hour  |
 
 You can either set a variable, e.g. `export OCL_GITHUB_USERNAME="mail@example.com"` or retrieve it via a command, e.g. `export OCL_GITHUB_USERNAME_COMMAND="op read op://Private/Github/username"`.
 If a variable is not set but needed, OCL will ask for it interactively.
 
 ## App-Interface
 
 OCL retrieves the cluster information from app-interface via GraphQL (`OCL_APP_INTERFACE_URL`) and caches them
@@ -106,15 +107,14 @@
 * Works only with a Red Hat associate account
 
 ## Development
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 
-
 Use [Conventional Commit messages](https://www.conventionalcommits.org).
 The most important prefixes you should have in mind are:
 
 * `fix:` which represents bug fixes, and correlates to a [SemVer](https://semver.org/)
   patch.
 * `feat:` which represents a new feature, and correlates to a SemVer minor.
 * `feat!:`,  or `fix!:`, `refactor!:`, etc., which represent a breaking change
@@ -124,18 +124,15 @@
 Consider using an empty commit:
 
 ```
 git commit --allow-empty -m "chore: release"
 ```
 
 When a commit to the main branch has `Release-As: x.x.x` (case insensitive) in the **commit body**, Release Please will open a new pull request for the specified version.
+
 ```
 git commit --allow-empty -m "chore: release 2.0.0" -m "Release-As: 2.0.0"
 ```
 
-
-[github-discussions-badge]: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
-[github-discussions-link]:  https://github.com/chassing/ocl/discussions
 [pypi-link]:                https://pypi.org/project/openshift-cluster-login/
 [pypi-platforms]:           https://img.shields.io/pypi/pyversions/openshift-cluster-login
-[pypi-version]:             https://badge.fury.io/py/openshift-cluster-login.svg
```

