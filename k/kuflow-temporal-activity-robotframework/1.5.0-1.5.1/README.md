# Comparing `tmp/kuflow_temporal_activity_robotframework-1.5.0.tar.gz` & `tmp/kuflow_temporal_activity_robotframework-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuflow_temporal_activity_robotframework-1.5.0.tar", max compression
+gzip compressed data, was "kuflow_temporal_activity_robotframework-1.5.1.tar", max compression
```

## Comparing `kuflow_temporal_activity_robotframework-1.5.0.tar` & `kuflow_temporal_activity_robotframework-1.5.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      921 2024-04-09 11:44:28.833042 kuflow_temporal_activity_robotframework-1.5.0/README.md
--rw-r--r--   0        0        0        6 2024-04-09 11:44:28.833042 kuflow_temporal_activity_robotframework-1.5.0/VERSION
--rw-r--r--   0        0        0     1235 2024-04-09 11:44:28.833042 kuflow_temporal_activity_robotframework-1.5.0/kuflow_temporal_activity_robotframework/__init__.py
--rw-r--r--   0        0        0     5990 2024-04-09 11:44:28.833042 kuflow_temporal_activity_robotframework-1.5.0/kuflow_temporal_activity_robotframework/robot_framework_activities.py
--rw-r--r--   0        0        0     1006 2024-04-09 11:50:40.137394 kuflow_temporal_activity_robotframework-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     1713 1970-01-01 00:00:00.000000 kuflow_temporal_activity_robotframework-1.5.0/setup.py
--rw-r--r--   0        0        0     1767 1970-01-01 00:00:00.000000 kuflow_temporal_activity_robotframework-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      921 2024-04-25 11:49:37.329017 kuflow_temporal_activity_robotframework-1.5.1/README.md
+-rw-r--r--   0        0        0        6 2024-04-25 11:49:37.329017 kuflow_temporal_activity_robotframework-1.5.1/VERSION
+-rw-r--r--   0        0        0     1235 2024-04-25 11:49:37.329017 kuflow_temporal_activity_robotframework-1.5.1/kuflow_temporal_activity_robotframework/__init__.py
+-rw-r--r--   0        0        0     5990 2024-04-25 11:49:37.329017 kuflow_temporal_activity_robotframework-1.5.1/kuflow_temporal_activity_robotframework/robot_framework_activities.py
+-rw-r--r--   0        0        0     1006 2024-04-25 11:57:00.292206 kuflow_temporal_activity_robotframework-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1713 1970-01-01 00:00:00.000000 kuflow_temporal_activity_robotframework-1.5.1/setup.py
+-rw-r--r--   0        0        0     1767 1970-01-01 00:00:00.000000 kuflow_temporal_activity_robotframework-1.5.1/PKG-INFO
```

### Comparing `kuflow_temporal_activity_robotframework-1.5.0/README.md` & `kuflow_temporal_activity_robotframework-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_robotframework-1.5.0/kuflow_temporal_activity_robotframework/__init__.py` & `kuflow_temporal_activity_robotframework-1.5.1/kuflow_temporal_activity_robotframework/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 #
 
 from .robot_framework_activities import RobotFrameworkActivities
 
 
 __all__ = ["RobotFrameworkActivities"]
 
-__version__ = "1.5.0"
+__version__ = "1.5.1"
```

### Comparing `kuflow_temporal_activity_robotframework-1.5.0/kuflow_temporal_activity_robotframework/robot_framework_activities.py` & `kuflow_temporal_activity_robotframework-1.5.1/kuflow_temporal_activity_robotframework/robot_framework_activities.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_robotframework-1.5.0/pyproject.toml` & `kuflow_temporal_activity_robotframework-1.5.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuflow-temporal-activity-robotframework"
-version = "1.5.0"
+version = "1.5.1"
 description = "KuFlow SDK :: Temporal.io activities to execute Robot Frameworks tasks"
 license = "MIT"
 authors = ["KuFlow S.L. <kuflow@kuflow.com>"]
 homepage = "https://kuflow.com/"
 documentation = "https://docs.kuflow.com/"
 repository = "https://github.com/kuflow/kuflow-sdk-python"
 readme = "README.md"
@@ -13,15 +13,15 @@
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-kuflow-temporal-common = "^1.5.0"
+kuflow-temporal-common = "^1.5.1"
 robotframework = ">5.0.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.3.0"
 ruff = ">=0.1.8,<1.0.0"
 pytest = "^7.3.1"
 robotframework-tidy = "^3.3.3"
```

### Comparing `kuflow_temporal_activity_robotframework-1.5.0/setup.py` & `kuflow_temporal_activity_robotframework-1.5.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['kuflow_temporal_activity_robotframework']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['kuflow-temporal-common>=1.5.0,<2.0.0', 'robotframework>5.0.0']
+['kuflow-temporal-common>=1.5.1,<2.0.0', 'robotframework>5.0.0']
 
 setup_kwargs = {
     'name': 'kuflow-temporal-activity-robotframework',
-    'version': '1.5.0',
+    'version': '1.5.1',
     'description': 'KuFlow SDK :: Temporal.io activities to execute Robot Frameworks tasks',
     'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n[![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-robotframework)\n[![PyPI](https://img.shields.io/pypi/v/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-robotframework)\n\n# KuFlow Temporal Activities Robot Framework\n\nTemporal.io activities to execute Robot Framework tasks, aka RPA\n\n## Documentation\n\nMore detailed docs are available in the [documentation pages](https://docs.kuflow.com/developers/).\n\n## Contributing\n\nWe are happy to receive your help and comments, together we will dance a wonderful KuFlow. Please review our [contribution guide](CONTRIBUTING.md).\n\n## License\n\n[MIT License](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n',
     'author': 'KuFlow S.L.',
     'author_email': 'kuflow@kuflow.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kuflow.com/',
```

### Comparing `kuflow_temporal_activity_robotframework-1.5.0/PKG-INFO` & `kuflow_temporal_activity_robotframework-1.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kuflow-temporal-activity-robotframework
-Version: 1.5.0
+Version: 1.5.1
 Summary: KuFlow SDK :: Temporal.io activities to execute Robot Frameworks tasks
 Home-page: https://kuflow.com/
 License: MIT
 Author: KuFlow S.L.
 Author-email: kuflow@kuflow.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: kuflow-temporal-common (>=1.5.0,<2.0.0)
+Requires-Dist: kuflow-temporal-common (>=1.5.1,<2.0.0)
 Requires-Dist: robotframework (>5.0.0)
 Project-URL: Documentation, https://docs.kuflow.com/
 Project-URL: Repository, https://github.com/kuflow/kuflow-sdk-python
 Description-Content-Type: text/markdown
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)
 [![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-robotframework)
```

