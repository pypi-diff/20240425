# Comparing `tmp/dyff_client-0.3.1.tar.gz` & `tmp/dyff_client-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff_client-0.3.1.tar", last modified: Mon Apr 15 03:05:41 2024, max compression
+gzip compressed data, was "dyff_client-0.3.2.tar", last modified: Wed Apr 24 22:17:29 2024, max compression
```

## Comparing `dyff_client-0.3.1.tar` & `dyff_client-0.3.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:05:41.391260 dyff_client-0.3.1/
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-15 03:05:35.000000 dyff_client-0.3.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1777 2024-04-15 03:05:35.000000 dyff_client-0.3.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-15 03:05:35.000000 dyff_client-0.3.1/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-04-15 03:05:35.000000 dyff_client-0.3.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-04-15 03:05:35.000000 dyff_client-0.3.1/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     3478 2024-04-15 03:05:35.000000 dyff_client-0.3.1/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-15 03:05:35.000000 dyff_client-0.3.1/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-15 03:05:35.000000 dyff_client-0.3.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-15 03:05:35.000000 dyff_client-0.3.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4008 2024-04-15 03:05:41.390260 dyff_client-0.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2781 2024-04-15 03:05:35.000000 dyff_client-0.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:05:41.377260 dyff_client-0.3.1/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:05:41.382260 dyff_client-0.3.1/dyff/client/
--rw-rw-rw-   0 root         (0) root         (0)      221 2024-04-15 03:05:35.000000 dyff_client-0.3.1/dyff/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:05:41.383260 dyff_client-0.3.1/dyff/client/_generated/
--rw-rw-rw-   0 root         (0) root         (0)      709 2024-04-15 03:05:35.000000 dyff_client-0.3.1/dyff/client/_generated/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7058 2024-04-15 03:05:35.000000 dyff_client-0.3.1/dyff/client/_generated/_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-15 03:05:35.000000 dyff_client-0.3.1/dyff/client/_generated/_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2024-04-15 03:05:35.000000 dyff_client-0.3.1/dyff/client/_generated/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)    80932 2024-04-15 03:05:35.000000 dyff_client-0.3.1/dyff/client/_generated/_serialization.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-04-15 03:05:35.000000 dyff_client-0.3.1/dyff/client/_generated/_vendor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:05:41.384260 dyff_client-0.3.1/dyff/client/_generated/aio/
--rw-rw-rw-   0 root         (0) root         (0)      709 2024-04-15 03:05:35.000000 dyff_client-0.3.1/dyff/client/_generated/aio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7226 2024-04-15 03:05:35.000000 dyff_client-0.3.1/dyff/client/_generated/aio/_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1981 2024-04-15 03:05:35.000000 dyff_client-0.3.1/dyff/client/_generated/aio/_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-04-15 03:05:35.000000 dyff_client-0.3.1/dyff/client/_generated/aio/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-04-15 03:05:35.000000 dyff_client-0.3.1/dyff/client/_generated/aio/_vendor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:05:41.386260 dyff_client-0.3.1/dyff/client/_generated/aio/operations/
--rw-rw-rw-   0 root         (0) root         (0)     1291 2024-04-15 03:05:35.000000 dyff_client-0.3.1/dyff/client/_generated/aio/operations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   770253 2024-04-15 03:05:35.000000 dyff_client-0.3.1/dyff/client/_generated/aio/operations/_operations.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-04-15 03:05:35.000000 dyff_client-0.3.1/dyff/client/_generated/aio/operations/_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:05:41.387260 dyff_client-0.3.1/dyff/client/_generated/operations/
--rw-rw-rw-   0 root         (0) root         (0)     1291 2024-04-15 03:05:35.000000 dyff_client-0.3.1/dyff/client/_generated/operations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   821959 2024-04-15 03:05:35.000000 dyff_client-0.3.1/dyff/client/_generated/operations/_operations.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2024-04-15 03:05:35.000000 dyff_client-0.3.1/dyff/client/_generated/operations/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-04-15 03:05:35.000000 dyff_client-0.3.1/dyff/client/_generated/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    82254 2024-04-15 03:05:35.000000 dyff_client-0.3.1/dyff/client/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:05:41.390260 dyff_client-0.3.1/dyff_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4008 2024-04-15 03:05:41.000000 dyff_client-0.3.1/dyff_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1464 2024-04-15 03:05:41.000000 dyff_client-0.3.1/dyff_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 03:05:41.000000 dyff_client-0.3.1/dyff_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       83 2024-04-15 03:05:41.000000 dyff_client-0.3.1/dyff_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-15 03:05:41.000000 dyff_client-0.3.1/dyff_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1084 2024-04-15 03:05:35.000000 dyff_client-0.3.1/makefile
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-15 03:05:35.000000 dyff_client-0.3.1/package-lock.json
--rw-rw-rw-   0 root         (0) root         (0)       53 2024-04-15 03:05:35.000000 dyff_client-0.3.1/package.json
--rw-rw-rw-   0 root         (0) root         (0)     1589 2024-04-15 03:05:35.000000 dyff_client-0.3.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:05:41.378260 dyff_client-0.3.1/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:05:41.388260 dyff_client-0.3.1/scripts/inferenceservices/
--rw-rw-rw-   0 root         (0) root         (0)     2529 2024-04-15 03:05:35.000000 dyff_client-0.3.1/scripts/inferenceservices/databricks--dolly-v2-3b--default.py
--rw-rw-rw-   0 root         (0) root         (0)     2537 2024-04-15 03:05:35.000000 dyff_client-0.3.1/scripts/inferenceservices/tiiuae--falcon-7b--default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:05:41.389260 dyff_client-0.3.1/scripts/models/
--rw-rw-rw-   0 root         (0) root         (0)      420 2024-04-15 03:05:35.000000 dyff_client-0.3.1/scripts/models/databricks--dolly-v2-3b--rox.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1374 2024-04-15 03:05:35.000000 dyff_client-0.3.1/scripts/models/databricks--dolly-v2-3b.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2024-04-15 03:05:35.000000 dyff_client-0.3.1/scripts/models/tiiuae--falcon-7b--rox.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1356 2024-04-15 03:05:35.000000 dyff_client-0.3.1/scripts/models/tiiuae--falcon-7b.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 03:05:41.391260 dyff_client-0.3.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:05:41.390260 dyff_client-0.3.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1123 2024-04-15 03:05:35.000000 dyff_client-0.3.1/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.630480 dyff_client-0.3.2/
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-24 22:17:23.000000 dyff_client-0.3.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1777 2024-04-24 22:17:23.000000 dyff_client-0.3.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-24 22:17:23.000000 dyff_client-0.3.2/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-04-24 22:17:23.000000 dyff_client-0.3.2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-04-24 22:17:23.000000 dyff_client-0.3.2/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2024-04-24 22:17:23.000000 dyff_client-0.3.2/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-24 22:17:23.000000 dyff_client-0.3.2/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-24 22:17:23.000000 dyff_client-0.3.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-24 22:17:23.000000 dyff_client-0.3.2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4008 2024-04-24 22:17:29.630480 dyff_client-0.3.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2781 2024-04-24 22:17:23.000000 dyff_client-0.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.617647 dyff_client-0.3.2/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.623147 dyff_client-0.3.2/dyff/client/
+-rw-rw-rw-   0 root         (0) root         (0)      221 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.624064 dyff_client-0.3.2/dyff/client/_generated/
+-rw-rw-rw-   0 root         (0) root         (0)      709 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7058 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      752 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)    80932 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/_serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/_vendor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.624980 dyff_client-0.3.2/dyff/client/_generated/aio/
+-rw-rw-rw-   0 root         (0) root         (0)      709 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/aio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7226 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/aio/_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/aio/_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/aio/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/aio/_vendor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.625897 dyff_client-0.3.2/dyff/client/_generated/aio/operations/
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/aio/operations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   770253 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/aio/operations/_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/aio/operations/_patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.627730 dyff_client-0.3.2/dyff/client/_generated/operations/
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/operations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   821959 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/operations/_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/operations/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    82266 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.629564 dyff_client-0.3.2/dyff_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4008 2024-04-24 22:17:29.000000 dyff_client-0.3.2/dyff_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1464 2024-04-24 22:17:29.000000 dyff_client-0.3.2/dyff_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 22:17:29.000000 dyff_client-0.3.2/dyff_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2024-04-24 22:17:29.000000 dyff_client-0.3.2/dyff_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-24 22:17:29.000000 dyff_client-0.3.2/dyff_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2024-04-24 22:17:23.000000 dyff_client-0.3.2/makefile
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-24 22:17:23.000000 dyff_client-0.3.2/package-lock.json
+-rw-rw-rw-   0 root         (0) root         (0)       53 2024-04-24 22:17:23.000000 dyff_client-0.3.2/package.json
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2024-04-24 22:17:23.000000 dyff_client-0.3.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.618564 dyff_client-0.3.2/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.628647 dyff_client-0.3.2/scripts/inferenceservices/
+-rw-rw-rw-   0 root         (0) root         (0)     2529 2024-04-24 22:17:23.000000 dyff_client-0.3.2/scripts/inferenceservices/databricks--dolly-v2-3b--default.py
+-rw-rw-rw-   0 root         (0) root         (0)     2537 2024-04-24 22:17:23.000000 dyff_client-0.3.2/scripts/inferenceservices/tiiuae--falcon-7b--default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.629564 dyff_client-0.3.2/scripts/models/
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-04-24 22:17:23.000000 dyff_client-0.3.2/scripts/models/databricks--dolly-v2-3b--rox.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2024-04-24 22:17:23.000000 dyff_client-0.3.2/scripts/models/databricks--dolly-v2-3b.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-04-24 22:17:23.000000 dyff_client-0.3.2/scripts/models/tiiuae--falcon-7b--rox.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1356 2024-04-24 22:17:23.000000 dyff_client-0.3.2/scripts/models/tiiuae--falcon-7b.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 22:17:29.630480 dyff_client-0.3.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.629564 dyff_client-0.3.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1123 2024-04-24 22:17:23.000000 dyff_client-0.3.2/tests/test_import.py
```

### Comparing `dyff_client-0.3.1/.gitlab-ci.yml` & `dyff_client-0.3.2/.gitlab-ci.yml`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 include:
   - project: buildgarden/pipelines/gitlab
     ref: 0.2.2
     file:
       - gitlab-release.yml
   - project: buildgarden/pipelines/detect-secrets
-    ref: 0.1.0
+    ref: 0.2.1
     file:
       - detect-secrets.yml
   - project: buildgarden/pipelines/prettier
     ref: 0.3.2
     file:
       - prettier.yml
   - project: buildgarden/pipelines/python
```

### Comparing `dyff_client-0.3.1/.licenserc.yaml` & `dyff_client-0.3.2/.licenserc.yaml`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/.pre-commit-config.yaml` & `dyff_client-0.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/.secrets.baseline` & `dyff_client-0.3.2/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/CODE_OF_CONDUCT.md` & `dyff_client-0.3.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/LICENSE` & `dyff_client-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/PKG-INFO` & `dyff_client-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-client
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python client for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-client
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-client/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_client-0.3.1/README.md` & `dyff_client-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/dyff/client/_generated/__init__.py` & `dyff_client-0.3.2/dyff/client/_generated/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/dyff/client/_generated/_client.py` & `dyff_client-0.3.2/dyff/client/_generated/_client.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/dyff/client/_generated/_configuration.py` & `dyff_client-0.3.2/dyff/client/_generated/_configuration.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/dyff/client/_generated/_patch.py` & `dyff_client-0.3.2/dyff/client/_generated/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/dyff/client/_generated/_serialization.py` & `dyff_client-0.3.2/dyff/client/_generated/_serialization.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/dyff/client/_generated/_vendor.py` & `dyff_client-0.3.2/dyff/client/_generated/_vendor.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/dyff/client/_generated/aio/__init__.py` & `dyff_client-0.3.2/dyff/client/_generated/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/dyff/client/_generated/aio/_client.py` & `dyff_client-0.3.2/dyff/client/_generated/aio/_client.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/dyff/client/_generated/aio/_configuration.py` & `dyff_client-0.3.2/dyff/client/_generated/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/dyff/client/_generated/aio/_patch.py` & `dyff_client-0.3.2/dyff/client/_generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/dyff/client/_generated/aio/_vendor.py` & `dyff_client-0.3.2/dyff/client/_generated/aio/_vendor.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/dyff/client/_generated/aio/operations/__init__.py` & `dyff_client-0.3.2/dyff/client/_generated/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/dyff/client/_generated/aio/operations/_operations.py` & `dyff_client-0.3.2/dyff/client/_generated/aio/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/dyff/client/_generated/aio/operations/_patch.py` & `dyff_client-0.3.2/dyff/client/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/dyff/client/_generated/operations/__init__.py` & `dyff_client-0.3.2/dyff/client/_generated/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/dyff/client/_generated/operations/_operations.py` & `dyff_client-0.3.2/dyff/client/_generated/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/dyff/client/_generated/operations/_patch.py` & `dyff_client-0.3.2/dyff/client/_generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/dyff/client/client.py` & `dyff_client-0.3.2/dyff/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     # verify_ssl_certificates deprecated
     # remove after 10/2024
     return not verify_ssl_certificates or insecure
 
 
 def _retry_not_found(fn):
     def _impl(*args, **kwargs):
-        delays = [1.0, 2.0, 5.0]
+        delays = [1.0, 2.0, 5.0, 10.0, 10.0]
         retries = 0
         while True:
             try:
                 return fn(*args, **kwargs)
             except HttpResponseError as ex:
                 if ex.status_code == 404 and retries < len(delays):
                     time.sleep(delays[retries])
```

### Comparing `dyff_client-0.3.1/dyff_client.egg-info/PKG-INFO` & `dyff_client-0.3.2/dyff_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-client
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python client for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-client
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-client/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_client-0.3.1/dyff_client.egg-info/SOURCES.txt` & `dyff_client-0.3.2/dyff_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/makefile` & `dyff_client-0.3.2/makefile`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/pyproject.toml` & `dyff_client-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/scripts/inferenceservices/databricks--dolly-v2-3b--default.py` & `dyff_client-0.3.2/scripts/inferenceservices/databricks--dolly-v2-3b--default.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/scripts/inferenceservices/tiiuae--falcon-7b--default.py` & `dyff_client-0.3.2/scripts/inferenceservices/tiiuae--falcon-7b--default.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/scripts/models/databricks--dolly-v2-3b.py` & `dyff_client-0.3.2/scripts/models/databricks--dolly-v2-3b.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/scripts/models/tiiuae--falcon-7b.py` & `dyff_client-0.3.2/scripts/models/tiiuae--falcon-7b.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.1/tests/test_import.py` & `dyff_client-0.3.2/tests/test_import.py`

 * *Files identical despite different names*

