# Comparing `tmp/airlift-0.3.1.tar.gz` & `tmp/airlift-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airlift-0.3.1.tar", max compression
+gzip compressed data, was "airlift-0.4.0.tar", max compression
```

## Comparing `airlift-0.3.1.tar` & `airlift-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1062 2024-03-13 15:41:02.081869 airlift-0.3.1/LICENSE
--rw-r--r--   0        0        0     7842 2024-03-13 15:41:02.081869 airlift-0.3.1/README.md
--rw-r--r--   0        0        0      708 2024-03-13 15:41:02.093870 airlift-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/commands/__init__.py
--rw-r--r--   0        0        0     1364 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/commands/check.py
--rw-r--r--   0        0        0     1033 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/commands/import_variables.py
--rw-r--r--   0        0        0     1527 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/commands/logs.py
--rw-r--r--   0        0        0      939 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/commands/pause.py
--rw-r--r--   0        0        0     1161 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/commands/remove.py
--rw-r--r--   0        0        0     1144 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/commands/run_dag.py
--rw-r--r--   0        0        0     7714 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/commands/start.py
--rw-r--r--   0        0        0     1177 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/commands/status.py
--rw-r--r--   0        0        0        0 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/config/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/config/airlift/config.yaml
--rw-r--r--   0        0        0       71 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/config/airlift/required_software.yaml
--rw-r--r--   0        0        0      928 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/config/config.py
--rw-r--r--   0        0        0      176 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/config/docker/Dockerfile
--rw-r--r--   0        0        0        0 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/config/docker/final/.gitkeep
--rw-r--r--   0        0        0     1836 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/config/helm/values.yaml
--rw-r--r--   0        0        0      975 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/config/kind/cluster.yaml
--rw-r--r--   0        0        0     4121 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/main.py
--rw-r--r--   0        0        0        0 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/utils/__init__.py
--rw-r--r--   0        0        0     3676 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/utils/airflow.py
--rw-r--r--   0        0        0      767 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/utils/airlift.py
--rw-r--r--   0        0        0     1898 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/utils/command.py
--rw-r--r--   0        0        0     1989 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/utils/docker.py
--rw-r--r--   0        0        0     3186 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/utils/file.py
--rw-r--r--   0        0        0     1606 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/utils/helm.py
--rw-r--r--   0        0        0     3507 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/utils/kind.py
--rw-r--r--   0        0        0     3235 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/utils/kubernetes.py
--rw-r--r--   0        0        0    10067 2024-03-13 15:41:02.093870 airlift-0.3.1/src/airlift/utils/parser.py
--rw-r--r--   0        0        0     8585 1970-01-01 00:00:00.000000 airlift-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-25 16:38:13.628801 airlift-0.4.0/LICENSE
+-rw-r--r--   0        0        0     7842 2024-04-25 16:38:13.628801 airlift-0.4.0/README.md
+-rw-r--r--   0        0        0      717 2024-04-25 16:38:13.636801 airlift-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-25 16:38:13.636801 airlift-0.4.0/src/airlift/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/commands/__init__.py
+-rw-r--r--   0        0        0     1364 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/commands/check.py
+-rw-r--r--   0        0        0     1033 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/commands/import_variables.py
+-rw-r--r--   0        0        0     1527 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/commands/logs.py
+-rw-r--r--   0        0        0      939 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/commands/pause.py
+-rw-r--r--   0        0        0     1161 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/commands/remove.py
+-rw-r--r--   0        0        0     1144 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/commands/run_dag.py
+-rw-r--r--   0        0        0     7714 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/commands/start.py
+-rw-r--r--   0        0        0     1177 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/commands/status.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/config/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/config/airlift/config.yaml
+-rw-r--r--   0        0        0       71 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/config/airlift/required_software.yaml
+-rw-r--r--   0        0        0      928 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/config/config.py
+-rw-r--r--   0        0        0      176 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/config/docker/Dockerfile
+-rw-r--r--   0        0        0        0 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/config/docker/final/.gitkeep
+-rw-r--r--   0        0        0     2127 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/config/helm/values.yaml
+-rw-r--r--   0        0        0      975 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/config/kind/cluster.yaml
+-rw-r--r--   0        0        0     4121 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/main.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/utils/__init__.py
+-rw-r--r--   0        0        0     3676 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/utils/airflow.py
+-rw-r--r--   0        0        0      767 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/utils/airlift.py
+-rw-r--r--   0        0        0     1898 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/utils/command.py
+-rw-r--r--   0        0        0     1989 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/utils/docker.py
+-rw-r--r--   0        0        0     3186 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/utils/file.py
+-rw-r--r--   0        0        0     1606 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/utils/helm.py
+-rw-r--r--   0        0        0     3507 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/utils/kind.py
+-rw-r--r--   0        0        0     3235 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/utils/kubernetes.py
+-rw-r--r--   0        0        0    10067 2024-04-25 16:38:13.640801 airlift-0.4.0/src/airlift/utils/parser.py
+-rw-r--r--   0        0        0     8585 1970-01-01 00:00:00.000000 airlift-0.4.0/PKG-INFO
```

### Comparing `airlift-0.3.1/LICENSE` & `airlift-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airlift-0.3.1/README.md` & `airlift-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `airlift-0.3.1/pyproject.toml` & `airlift-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airlift"
-version = "0.3.1"
+version = "0.4.0"
 description = "A CLI for creating a flexible Apache Airflow local development environment"
 authors = ["jered.little <jeredlittle1996@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "airlift", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -17,15 +17,15 @@
 requests = "^2.30.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 coverage = "^7.2.5"
 mock = "^5.0.2"
-black = "^23.10.1"
+black = ">=23.10.1,<25.0.0"
 ruff = "^0.1.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
```

### Comparing `airlift-0.3.1/src/airlift/commands/check.py` & `airlift-0.4.0/src/airlift/commands/check.py`

 * *Files identical despite different names*

### Comparing `airlift-0.3.1/src/airlift/commands/import_variables.py` & `airlift-0.4.0/src/airlift/commands/import_variables.py`

 * *Files identical despite different names*

### Comparing `airlift-0.3.1/src/airlift/commands/logs.py` & `airlift-0.4.0/src/airlift/commands/logs.py`

 * *Files identical despite different names*

### Comparing `airlift-0.3.1/src/airlift/commands/pause.py` & `airlift-0.4.0/src/airlift/commands/pause.py`

 * *Files identical despite different names*

### Comparing `airlift-0.3.1/src/airlift/commands/remove.py` & `airlift-0.4.0/src/airlift/commands/remove.py`

 * *Files identical despite different names*

### Comparing `airlift-0.3.1/src/airlift/commands/run_dag.py` & `airlift-0.4.0/src/airlift/commands/run_dag.py`

 * *Files identical despite different names*

### Comparing `airlift-0.3.1/src/airlift/commands/start.py` & `airlift-0.4.0/src/airlift/commands/start.py`

 * *Files identical despite different names*

### Comparing `airlift-0.3.1/src/airlift/commands/status.py` & `airlift-0.4.0/src/airlift/commands/status.py`

 * *Files identical despite different names*

### Comparing `airlift-0.3.1/src/airlift/config/config.py` & `airlift-0.4.0/src/airlift/config/config.py`

 * *Files identical despite different names*

### Comparing `airlift-0.3.1/src/airlift/config/helm/values.yaml` & `airlift-0.4.0/src/airlift/config/helm/values.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -77,7 +77,19 @@
 webserver:
   service:
     type: NodePort
     ports:
       - name: airflow-ui
         nodePort: 30080
         port: 8080
+  extraVolumes:
+    {% if plugin_path != None  %}
+    - name: plugins
+      hostPath:
+        path: /mnt/airflow/plugins
+        type: Directory
+    {% endif %}
+  extraVolumeMounts:
+    {% if plugin_path != None  %}
+    - name: plugins
+      mountPath: /opt/airflow/plugins
+    {% endif %}
```

### Comparing `airlift-0.3.1/src/airlift/config/kind/cluster.yaml` & `airlift-0.4.0/src/airlift/config/kind/cluster.yaml`

 * *Files identical despite different names*

### Comparing `airlift-0.3.1/src/airlift/main.py` & `airlift-0.4.0/src/airlift/main.py`

 * *Files identical despite different names*

### Comparing `airlift-0.3.1/src/airlift/utils/airflow.py` & `airlift-0.4.0/src/airlift/utils/airflow.py`

 * *Files identical despite different names*

### Comparing `airlift-0.3.1/src/airlift/utils/airlift.py` & `airlift-0.4.0/src/airlift/utils/airlift.py`

 * *Files identical despite different names*

### Comparing `airlift-0.3.1/src/airlift/utils/command.py` & `airlift-0.4.0/src/airlift/utils/command.py`

 * *Files identical despite different names*

### Comparing `airlift-0.3.1/src/airlift/utils/docker.py` & `airlift-0.4.0/src/airlift/utils/docker.py`

 * *Files identical despite different names*

### Comparing `airlift-0.3.1/src/airlift/utils/file.py` & `airlift-0.4.0/src/airlift/utils/file.py`

 * *Files identical despite different names*

### Comparing `airlift-0.3.1/src/airlift/utils/helm.py` & `airlift-0.4.0/src/airlift/utils/helm.py`

 * *Files identical despite different names*

### Comparing `airlift-0.3.1/src/airlift/utils/kind.py` & `airlift-0.4.0/src/airlift/utils/kind.py`

 * *Files identical despite different names*

### Comparing `airlift-0.3.1/src/airlift/utils/kubernetes.py` & `airlift-0.4.0/src/airlift/utils/kubernetes.py`

 * *Files identical despite different names*

### Comparing `airlift-0.3.1/src/airlift/utils/parser.py` & `airlift-0.4.0/src/airlift/utils/parser.py`

 * *Files identical despite different names*

### Comparing `airlift-0.3.1/PKG-INFO` & `airlift-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airlift
-Version: 0.3.1
+Version: 0.4.0
 Summary: A CLI for creating a flexible Apache Airflow local development environment
 Author: jered.little
 Author-email: jeredlittle1996@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: airlift Version: 0.3.1 Summary: A CLI for creating
+Metadata-Version: 2.1 Name: airlift Version: 0.4.0 Summary: A CLI for creating
 a flexible Apache Airflow local development environment Author: jered.little
 Author-email: jeredlittle1996@gmail.com Requires-Python: >=3.9,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: argparse (>=1.4.0,<2.0.0)
 Requires-Dist: dotmap (>=1.3.30,<2.0.0) Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: hiyapyco (>=0.5.1,<0.6.0) Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
```

