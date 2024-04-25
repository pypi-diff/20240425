# Comparing `tmp/kuflow_robotframework-1.5.0.tar.gz` & `tmp/kuflow_robotframework-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuflow_robotframework-1.5.0.tar", max compression
+gzip compressed data, was "kuflow_robotframework-1.5.1.tar", max compression
```

## Comparing `kuflow_robotframework-1.5.0.tar` & `kuflow_robotframework-1.5.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1323 2024-04-09 11:44:28.833042 kuflow_robotframework-1.5.0/KuFlow/__init__.py
--rw-r--r--   0        0        0    19124 2024-04-09 11:44:28.833042 kuflow_robotframework-1.5.0/KuFlow/keywords.py
--rw-r--r--   0        0        0     2359 2024-04-09 11:44:28.833042 kuflow_robotframework-1.5.0/README.md
--rw-r--r--   0        0        0        6 2024-04-09 11:44:28.833042 kuflow_robotframework-1.5.0/VERSION
--rw-r--r--   0        0        0     1029 2024-04-09 11:50:37.313361 kuflow_robotframework-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     3297 1970-01-01 00:00:00.000000 kuflow_robotframework-1.5.0/setup.py
--rw-r--r--   0        0        0     3288 1970-01-01 00:00:00.000000 kuflow_robotframework-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1323 2024-04-25 11:49:37.325017 kuflow_robotframework-1.5.1/KuFlow/__init__.py
+-rw-r--r--   0        0        0    19124 2024-04-25 11:49:37.325017 kuflow_robotframework-1.5.1/KuFlow/keywords.py
+-rw-r--r--   0        0        0     2359 2024-04-25 11:49:37.325017 kuflow_robotframework-1.5.1/README.md
+-rw-r--r--   0        0        0        6 2024-04-25 11:49:37.325017 kuflow_robotframework-1.5.1/VERSION
+-rw-r--r--   0        0        0     1029 2024-04-25 11:56:57.600187 kuflow_robotframework-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3297 1970-01-01 00:00:00.000000 kuflow_robotframework-1.5.1/setup.py
+-rw-r--r--   0        0        0     3288 1970-01-01 00:00:00.000000 kuflow_robotframework-1.5.1/PKG-INFO
```

### Comparing `kuflow_robotframework-1.5.0/KuFlow/__init__.py` & `kuflow_robotframework-1.5.1/KuFlow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 from .keywords import Keywords
 
 
-__version__ = "1.5.0"
+__version__ = "1.5.1"
 __all__ = ["KuFlow"]
 
 
 class KuFlow(Keywords):
     """KuFlow: Automagic Workflows."""
 
     ROBOT_LIBRARY_VERSION = __version__
```

### Comparing `kuflow_robotframework-1.5.0/KuFlow/keywords.py` & `kuflow_robotframework-1.5.1/KuFlow/keywords.py`

 * *Files identical despite different names*

### Comparing `kuflow_robotframework-1.5.0/README.md` & `kuflow_robotframework-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `kuflow_robotframework-1.5.0/pyproject.toml` & `kuflow_robotframework-1.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuflow-robotframework"
-version = "1.5.0"
+version = "1.5.1"
 description = "KuFlow library for Robot Framework"
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
-kuflow-rest = "^1.5.0"
+kuflow-rest = "^1.5.1"
 robotframework = ">5.0.0"
 python-magic = {version = "^0.4.27", platform = "!=win32"}
 python-magic-bin = {version = "^0.4.14", platform = "win32"}
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.3.0"
 ruff = ">=0.1.8,<1.0.0"
```

### Comparing `kuflow_robotframework-1.5.0/setup.py` & `kuflow_robotframework-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 packages = \
 ['KuFlow']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['kuflow-rest>=1.5.0,<2.0.0', 'robotframework>5.0.0']
+['kuflow-rest>=1.5.1,<2.0.0', 'robotframework>5.0.0']
 
 extras_require = \
 {':sys_platform != "win32"': ['python-magic>=0.4.27,<0.5.0'],
  ':sys_platform == "win32"': ['python-magic-bin>=0.4.14,<0.5.0']}
 
 setup_kwargs = {
     'name': 'kuflow-robotframework',
-    'version': '1.5.0',
+    'version': '1.5.1',
     'description': 'KuFlow library for Robot Framework',
     'long_description': "[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n[![Python](https://img.shields.io/pypi/pyversions/kuflow-robotframework.svg)](https://pypi.org/project/kuflow-robotframework)\n[![PyPI](https://img.shields.io/pypi/v/kuflow-robotframework.svg)](https://pypi.org/project/kuflow-robotframework)\n\n# KuFlow Robot Framework\n\nThis library provides keywords to interact with the KuFlow API from a Robot Framework Robot. Its purpose is to facilitate interaction from the robot logic (RPA). Its use helps to keep the manipulation of robot results by Workflow decoupled as much as possible.\n\nList of available keywords:\n\n#### Set Client Authentication\n\n> Configure the client authentication in order to execute keywords against Rest API\n\n#### Append Log Message\n\n> Add a log entry to the task\n\n#### Claim Task\n\n> Allow to claim a task\n\n#### Retrieve Process\n\n> Allow to get a process by ID\n\n#### Retrieve Task\n\n> Allow to get a task by ID\n\n#### Save Element Document\n\n> Save a element task of type document\n\n#### Delete Element Document\n\n> Allow to delete a specific document from an element of document type using its id.\n\n#### Save Element\n\n> Save a element task\n\n#### Delete Element\n\n> Allow to delete task element by specifying the item definition code.\n\n#### Convert To Principal Item\n\n> Given an Id of a Principal user, create an item that represents a reference to the Principal.\n\n#### Convert To Document Item From Uri\n\n> Given an Id of a Document or the URI reference of a Document, create an item that represents a reference to the Document elementand can be used.\n\n#### Convert JSON String To Object\n\n> Given a JSON string as argument, return new JSON object\n\n#### Save Json Forms Value Data\n\n> Allows a JSON Forms to be saved in the task.\n\n#### Upload Json Forms Value Document\n\n> Allows you to upload a document to the referenced task and then include a reference to it in the task's JSON Forms.\n\n## Documentation\n\nMore detailed docs are available in the [documentation pages](https://docs.kuflow.com/developers/).\n\n## Contributing\n\nWe are happy to receive your help and comments, together we will dance a wonderful KuFlow. Please review our [contribution guide](CONTRIBUTING.md).\n\n## License\n\n[MIT License](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n",
     'author': 'KuFlow S.L.',
     'author_email': 'kuflow@kuflow.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kuflow.com/',
```

### Comparing `kuflow_robotframework-1.5.0/PKG-INFO` & `kuflow_robotframework-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kuflow-robotframework
-Version: 1.5.0
+Version: 1.5.1
 Summary: KuFlow library for Robot Framework
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
-Requires-Dist: kuflow-rest (>=1.5.0,<2.0.0)
+Requires-Dist: kuflow-rest (>=1.5.1,<2.0.0)
 Requires-Dist: python-magic (>=0.4.27,<0.5.0) ; sys_platform != "win32"
 Requires-Dist: python-magic-bin (>=0.4.14,<0.5.0) ; sys_platform == "win32"
 Requires-Dist: robotframework (>5.0.0)
 Project-URL: Documentation, https://docs.kuflow.com/
 Project-URL: Repository, https://github.com/kuflow/kuflow-sdk-python
 Description-Content-Type: text/markdown
```

