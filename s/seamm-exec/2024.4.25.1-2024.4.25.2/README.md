# Comparing `tmp/seamm_exec-2024.4.25.1.tar.gz` & `tmp/seamm_exec-2024.4.25.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seamm_exec-2024.4.25.1.tar", last modified: Thu Apr 25 18:25:27 2024, max compression
+gzip compressed data, was "seamm_exec-2024.4.25.2.tar", last modified: Thu Apr 25 18:52:08 2024, max compression
```

## Comparing `seamm_exec-2024.4.25.1.tar` & `seamm_exec-2024.4.25.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:25:27.303436 seamm_exec-2024.4.25.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-25 18:25:09.000000 seamm_exec-2024.4.25.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-25 18:25:09.000000 seamm_exec-2024.4.25.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 18:25:09.000000 seamm_exec-2024.4.25.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-25 18:25:27.303436 seamm_exec-2024.4.25.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-25 18:25:09.000000 seamm_exec-2024.4.25.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-25 18:25:09.000000 seamm_exec-2024.4.25.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:25:27.303436 seamm_exec-2024.4.25.1/seamm_exec/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-25 18:25:09.000000 seamm_exec-2024.4.25.1/seamm_exec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 18:25:27.000000 seamm_exec-2024.4.25.1/seamm_exec/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-04-25 18:25:09.000000 seamm_exec-2024.4.25.1/seamm_exec/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-25 18:25:09.000000 seamm_exec-2024.4.25.1/seamm_exec/computational_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-04-25 18:25:09.000000 seamm_exec-2024.4.25.1/seamm_exec/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)    27614 2024-04-25 18:25:09.000000 seamm_exec-2024.4.25.1/seamm_exec/exec_flowchart.py
--rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-04-25 18:25:09.000000 seamm_exec-2024.4.25.1/seamm_exec/local.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-25 18:25:09.000000 seamm_exec-2024.4.25.1/seamm_exec/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-25 18:25:09.000000 seamm_exec-2024.4.25.1/seamm_exec/seamm_exec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:25:27.303436 seamm_exec-2024.4.25.1/seamm_exec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-25 18:25:27.000000 seamm_exec-2024.4.25.1/seamm_exec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-25 18:25:27.000000 seamm_exec-2024.4.25.1/seamm_exec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:25:27.000000 seamm_exec-2024.4.25.1/seamm_exec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-25 18:25:27.000000 seamm_exec-2024.4.25.1/seamm_exec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:25:13.000000 seamm_exec-2024.4.25.1/seamm_exec.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-25 18:25:27.000000 seamm_exec-2024.4.25.1/seamm_exec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 18:25:27.000000 seamm_exec-2024.4.25.1/seamm_exec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-25 18:25:27.303436 seamm_exec-2024.4.25.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:25:27.303436 seamm_exec-2024.4.25.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-25 18:25:09.000000 seamm_exec-2024.4.25.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-25 18:25:09.000000 seamm_exec-2024.4.25.1/tests/test_seamm_exec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:08.588481 seamm_exec-2024.4.25.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-25 18:52:00.000000 seamm_exec-2024.4.25.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-25 18:52:00.000000 seamm_exec-2024.4.25.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 18:52:00.000000 seamm_exec-2024.4.25.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-25 18:52:08.588481 seamm_exec-2024.4.25.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-25 18:52:00.000000 seamm_exec-2024.4.25.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-25 18:52:00.000000 seamm_exec-2024.4.25.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:08.584481 seamm_exec-2024.4.25.2/seamm_exec/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-25 18:52:00.000000 seamm_exec-2024.4.25.2/seamm_exec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 18:52:08.000000 seamm_exec-2024.4.25.2/seamm_exec/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-04-25 18:52:00.000000 seamm_exec-2024.4.25.2/seamm_exec/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-25 18:52:00.000000 seamm_exec-2024.4.25.2/seamm_exec/computational_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-25 18:52:00.000000 seamm_exec-2024.4.25.2/seamm_exec/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27614 2024-04-25 18:52:00.000000 seamm_exec-2024.4.25.2/seamm_exec/exec_flowchart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-04-25 18:52:00.000000 seamm_exec-2024.4.25.2/seamm_exec/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-25 18:52:00.000000 seamm_exec-2024.4.25.2/seamm_exec/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-25 18:52:00.000000 seamm_exec-2024.4.25.2/seamm_exec/seamm_exec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:08.588481 seamm_exec-2024.4.25.2/seamm_exec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-25 18:52:08.000000 seamm_exec-2024.4.25.2/seamm_exec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-25 18:52:08.000000 seamm_exec-2024.4.25.2/seamm_exec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:52:08.000000 seamm_exec-2024.4.25.2/seamm_exec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-25 18:52:08.000000 seamm_exec-2024.4.25.2/seamm_exec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:52:03.000000 seamm_exec-2024.4.25.2/seamm_exec.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-25 18:52:08.000000 seamm_exec-2024.4.25.2/seamm_exec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 18:52:08.000000 seamm_exec-2024.4.25.2/seamm_exec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-25 18:52:08.588481 seamm_exec-2024.4.25.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:08.584481 seamm_exec-2024.4.25.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-25 18:52:00.000000 seamm_exec-2024.4.25.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-25 18:52:00.000000 seamm_exec-2024.4.25.2/tests/test_seamm_exec.py
```

### Comparing `seamm_exec-2024.4.25.1/CODE_OF_CONDUCT.md` & `seamm_exec-2024.4.25.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.25.1/LICENSE` & `seamm_exec-2024.4.25.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.25.1/PKG-INFO` & `seamm_exec-2024.4.25.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seamm_exec
-Version: 2024.4.25.1
+Version: 2024.4.25.2
 Summary: Classes to execute background codes for SEAMM
 Author-email: Paul Saxe <psaxe@molssi.org>
 License: MIT
 Project-URL: Source, https://github.com/molssi-seamm/seamm_exec/
 Project-URL: Documentation, https://molssi-seamm.github.io/
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seamm_exec-2024.4.25.1/README.md` & `seamm_exec-2024.4.25.2/README.md`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.25.1/pyproject.toml` & `seamm_exec-2024.4.25.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.25.1/seamm_exec/__init__.py` & `seamm_exec-2024.4.25.2/seamm_exec/__init__.py`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.25.1/seamm_exec/base.py` & `seamm_exec-2024.4.25.2/seamm_exec/base.py`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.25.1/seamm_exec/computational_environment.py` & `seamm_exec-2024.4.25.2/seamm_exec/computational_environment.py`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.25.1/seamm_exec/docker.py` & `seamm_exec-2024.4.25.2/seamm_exec/docker.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,17 +70,15 @@
         The equivalent commandline commmand is::
 
             docker run --rm -v $PWD:/home -w /home psaxe/mopac [mopac input_file]
 
         For this container the input filename defaults to "mopac.dat" so we do not need
         to add it.
         """
-        if "SEAMM_DEBUG_DOCKER" in os.environ:
-            log_level = self.logger.level
-            self.logger.setLevel(logging.DEBUG)
+        # self.logger.setLevel(logging.DEBUG)
 
         client = docker.from_env()
 
         # See if this is running in Docker and adjust the path accordingly
         if (
             "SEAMM_ENVIRONMENT" in os.environ
             and os.environ["SEAMM_ENVIRONMENT"] == "docker"
@@ -130,25 +128,44 @@
             tmp = command
             while True:
                 command = tmp.format(**config, **ce)
                 if tmp == command:
                     break
                 tmp = command
 
+            if "SEAMM_DEBUG_DOCKER" in os.environ:
+                with open(directory / "docker.txt", "a") as fd:
+                    print(
+                        f"""
+                        result = client.containers.run(
+                            command={command},
+                            environment={env},
+                            image={container},
+                            platform={platform},
+                            remove=True,
+                            stderr=True,
+                            stdout=True,
+                            volumes={paths},
+                            working_dir="/home",
+                        )
+                        """,
+                        file=fd,
+                        flush=True,
+                    )
             self.logger.debug(
                 f"""
                 result = client.containers.run(
                     command={command},
                     environment={env},
                     image={container},
                     platform={platform},
                     remove=True,
                     stderr=True,
                     stdout=True,
-                    volumes=paths,
+                    volumes={paths},
                     working_dir="/home",
                 )
                 """
             )
 
             result = client.containers.run(
                 command=command,
@@ -167,15 +184,15 @@
                 result = client.containers.run(
                     environment={env},
                     image={container},
                     platform={platform},
                     remove=True,
                     stderr=True,
                     stdout=True,
-                    volumes=paths,
+                    volumes={paths},
                     working_dir="/home",
                 )
                 """
             )
 
             result = client.containers.run(
                 environment=env,
@@ -186,11 +203,8 @@
                 stdout=True,
                 volumes=paths,
                 working_dir="/home",
             )
 
         self.logger.debug("\n" + pprint.pformat(result))
 
-        if "SEAMM_DEBUG_DOCKER" in os.environ:
-            self.logger.setLevel(log_level)
-
         return {}
```

### Comparing `seamm_exec-2024.4.25.1/seamm_exec/exec_flowchart.py` & `seamm_exec-2024.4.25.2/seamm_exec/exec_flowchart.py`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.25.1/seamm_exec/local.py` & `seamm_exec-2024.4.25.2/seamm_exec/local.py`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.25.1/seamm_exec/seamm_exec.py` & `seamm_exec-2024.4.25.2/seamm_exec/seamm_exec.py`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.25.1/seamm_exec.egg-info/PKG-INFO` & `seamm_exec-2024.4.25.2/seamm_exec.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seamm_exec
-Version: 2024.4.25.1
+Version: 2024.4.25.2
 Summary: Classes to execute background codes for SEAMM
 Author-email: Paul Saxe <psaxe@molssi.org>
 License: MIT
 Project-URL: Source, https://github.com/molssi-seamm/seamm_exec/
 Project-URL: Documentation, https://molssi-seamm.github.io/
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seamm_exec-2024.4.25.1/seamm_exec.egg-info/SOURCES.txt` & `seamm_exec-2024.4.25.2/seamm_exec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

