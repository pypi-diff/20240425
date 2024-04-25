# Comparing `tmp/seamm_exec-2024.4.24.tar.gz` & `tmp/seamm_exec-2024.4.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seamm_exec-2024.4.24.tar", last modified: Wed Apr 24 21:54:55 2024, max compression
+gzip compressed data, was "seamm_exec-2024.4.25.tar", last modified: Thu Apr 25 15:42:56 2024, max compression
```

## Comparing `seamm_exec-2024.4.24.tar` & `seamm_exec-2024.4.25.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:54:55.698193 seamm_exec-2024.4.24/
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-24 21:54:55.698193 seamm_exec-2024.4.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:54:55.694193 seamm_exec-2024.4.24/seamm_exec/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/seamm_exec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 21:54:55.000000 seamm_exec-2024.4.24/seamm_exec/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/seamm_exec/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/seamm_exec/computational_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/seamm_exec/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)    27614 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/seamm_exec/exec_flowchart.py
--rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/seamm_exec/local.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/seamm_exec/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/seamm_exec/seamm_exec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:54:55.694193 seamm_exec-2024.4.24/seamm_exec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-24 21:54:55.000000 seamm_exec-2024.4.24/seamm_exec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-24 21:54:55.000000 seamm_exec-2024.4.24/seamm_exec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 21:54:55.000000 seamm_exec-2024.4.24/seamm_exec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-24 21:54:55.000000 seamm_exec-2024.4.24/seamm_exec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 21:54:50.000000 seamm_exec-2024.4.24/seamm_exec.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-24 21:54:55.000000 seamm_exec-2024.4.24/seamm_exec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 21:54:55.000000 seamm_exec-2024.4.24/seamm_exec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-24 21:54:55.698193 seamm_exec-2024.4.24/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:54:55.694193 seamm_exec-2024.4.24/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/tests/test_seamm_exec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:56.369736 seamm_exec-2024.4.25/
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-25 15:42:38.000000 seamm_exec-2024.4.25/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-25 15:42:38.000000 seamm_exec-2024.4.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 15:42:38.000000 seamm_exec-2024.4.25/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-25 15:42:56.369736 seamm_exec-2024.4.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-25 15:42:38.000000 seamm_exec-2024.4.25/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-25 15:42:38.000000 seamm_exec-2024.4.25/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:56.369736 seamm_exec-2024.4.25/seamm_exec/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-25 15:42:38.000000 seamm_exec-2024.4.25/seamm_exec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 15:42:56.000000 seamm_exec-2024.4.25/seamm_exec/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-04-25 15:42:38.000000 seamm_exec-2024.4.25/seamm_exec/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-25 15:42:38.000000 seamm_exec-2024.4.25/seamm_exec/computational_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-04-25 15:42:38.000000 seamm_exec-2024.4.25/seamm_exec/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27614 2024-04-25 15:42:38.000000 seamm_exec-2024.4.25/seamm_exec/exec_flowchart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-04-25 15:42:38.000000 seamm_exec-2024.4.25/seamm_exec/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-25 15:42:38.000000 seamm_exec-2024.4.25/seamm_exec/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-25 15:42:38.000000 seamm_exec-2024.4.25/seamm_exec/seamm_exec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:56.369736 seamm_exec-2024.4.25/seamm_exec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-25 15:42:56.000000 seamm_exec-2024.4.25/seamm_exec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-25 15:42:56.000000 seamm_exec-2024.4.25/seamm_exec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:42:56.000000 seamm_exec-2024.4.25/seamm_exec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-25 15:42:56.000000 seamm_exec-2024.4.25/seamm_exec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:42:41.000000 seamm_exec-2024.4.25/seamm_exec.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-25 15:42:56.000000 seamm_exec-2024.4.25/seamm_exec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 15:42:56.000000 seamm_exec-2024.4.25/seamm_exec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-25 15:42:56.369736 seamm_exec-2024.4.25/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:56.369736 seamm_exec-2024.4.25/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-25 15:42:38.000000 seamm_exec-2024.4.25/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-25 15:42:38.000000 seamm_exec-2024.4.25/tests/test_seamm_exec.py
```

### Comparing `seamm_exec-2024.4.24/CODE_OF_CONDUCT.md` & `seamm_exec-2024.4.25/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.24/LICENSE` & `seamm_exec-2024.4.25/LICENSE`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.24/PKG-INFO` & `seamm_exec-2024.4.25/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seamm_exec
-Version: 2024.4.24
+Version: 2024.4.25
 Summary: Classes to execute background codes for SEAMM
 Author-email: Paul Saxe <psaxe@molssi.org>
 License: MIT
 Project-URL: Source, https://github.com/molssi-seamm/seamm_exec/
 Project-URL: Documentation, https://molssi-seamm.github.io/
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seamm_exec-2024.4.24/README.md` & `seamm_exec-2024.4.25/README.md`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.24/pyproject.toml` & `seamm_exec-2024.4.25/pyproject.toml`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.24/seamm_exec/__init__.py` & `seamm_exec-2024.4.25/seamm_exec/__init__.py`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.24/seamm_exec/base.py` & `seamm_exec-2024.4.25/seamm_exec/base.py`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.24/seamm_exec/computational_environment.py` & `seamm_exec-2024.4.25/seamm_exec/computational_environment.py`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.24/seamm_exec/docker.py` & `seamm_exec-2024.4.25/seamm_exec/docker.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,30 +89,31 @@
                 mounts = this_container.attrs["Mounts"]
             except Exception as e:
                 self.logger.error(
                     f"An error occurred in docker.py finding the mounts: {str(e)}"
                 )
                 raise
 
+            paths = []
             for mount in mounts:
                 self.logger.debug(f"{mount=}")
                 if mount["Destination"] == "/home":
                     path = Path(mount["Source"]).joinpath(*directory.parts[2:])
-                    break
+                    paths.append(f"{path}:/home")
                 elif mount["Destination"] == "/root/SEAMM":
                     path = Path(mount["Source"]).joinpath(*directory.parts[3:])
-                    break
-            else:
+                    paths.append(f"{path}:/root/SEAMM")
+            if len(paths) == 0:
                 raise RuntimeError(
                     "Neither /home or /root/SEAMM were in the mounts for the container!"
                     "\n{mounts=}"
                 )
         else:
             # Not in a Docker container, so use the path as is
-            path = Path(directory)
+            paths = [f"{Path(directory)}:/home"]
 
         self.logger.debug(f"path = {path}\n")
 
         self.logger.debug(pprint.pformat(config, compact=True))
 
         # Replace any variables in the container name
         container = config["container"].format(**config, **ce)
@@ -137,54 +138,54 @@
                     command={command},
                     environment={env},
                     image={container},
                     platform={platform},
                     remove=True,
                     stderr=True,
                     stdout=True,
-                    volumes=[f"{path}:/home"],
+                    volumes=paths,
                     working_dir="/home",
                 )
                 """
             )
 
             result = client.containers.run(
                 command=command,
                 environment=env,
                 image=container,
                 platform=platform,
                 remove=True,
                 stderr=True,
                 stdout=True,
-                volumes=[f"{path}:/home"],
+                volumes=paths,
                 working_dir="/home",
             )
         else:
             self.logger.debug(
                 f"""
                 result = client.containers.run(
                     environment={env},
                     image={container},
                     platform={platform},
                     remove=True,
                     stderr=True,
                     stdout=True,
-                    volumes=[f"{path}:/home"],
+                    volumes=paths,
                     working_dir="/home",
                 )
                 """
             )
 
             result = client.containers.run(
                 environment=env,
                 image=container,
                 platform=platform,
                 remove=True,
                 stderr=True,
                 stdout=True,
-                volumes=[f"{path}:/home"],
+                volumes=paths,
                 working_dir="/home",
             )
 
         self.logger.debug("\n" + pprint.pformat(result))
 
         return {}
```

### Comparing `seamm_exec-2024.4.24/seamm_exec/exec_flowchart.py` & `seamm_exec-2024.4.25/seamm_exec/exec_flowchart.py`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.24/seamm_exec/local.py` & `seamm_exec-2024.4.25/seamm_exec/local.py`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.24/seamm_exec/seamm_exec.py` & `seamm_exec-2024.4.25/seamm_exec/seamm_exec.py`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.24/seamm_exec.egg-info/PKG-INFO` & `seamm_exec-2024.4.25/seamm_exec.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seamm_exec
-Version: 2024.4.24
+Version: 2024.4.25
 Summary: Classes to execute background codes for SEAMM
 Author-email: Paul Saxe <psaxe@molssi.org>
 License: MIT
 Project-URL: Source, https://github.com/molssi-seamm/seamm_exec/
 Project-URL: Documentation, https://molssi-seamm.github.io/
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seamm_exec-2024.4.24/seamm_exec.egg-info/SOURCES.txt` & `seamm_exec-2024.4.25/seamm_exec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

