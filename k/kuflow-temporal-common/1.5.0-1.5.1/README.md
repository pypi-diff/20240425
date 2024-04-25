# Comparing `tmp/kuflow_temporal_common-1.5.0.tar.gz` & `tmp/kuflow_temporal_common-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuflow_temporal_common-1.5.0.tar", max compression
+gzip compressed data, was "kuflow_temporal_common-1.5.1.tar", max compression
```

## Comparing `kuflow_temporal_common-1.5.0.tar` & `kuflow_temporal_common-1.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      789 2024-04-09 11:44:28.833042 kuflow_temporal_common-1.5.0/README.md
--rw-r--r--   0        0        0        6 2024-04-09 11:44:28.833042 kuflow_temporal_common-1.5.0/VERSION
--rw-r--r--   0        0        0     1128 2024-04-09 11:44:28.833042 kuflow_temporal_common-1.5.0/kuflow_temporal_common/__init__.py
--rw-r--r--   0        0        0    12231 2024-04-09 11:44:28.833042 kuflow_temporal_common-1.5.0/kuflow_temporal_common/_connection_config.py
--rw-r--r--   0        0        0     2453 2024-04-09 11:44:28.833042 kuflow_temporal_common-1.5.0/kuflow_temporal_common/activity_utils.py
--rw-r--r--   0        0        0     1592 2024-04-09 11:44:28.833042 kuflow_temporal_common-1.5.0/kuflow_temporal_common/attributes.py
--rw-r--r--   0        0        0     4992 2024-04-09 11:44:28.833042 kuflow_temporal_common-1.5.0/kuflow_temporal_common/authentication.py
--rw-r--r--   0        0        0     9144 2024-04-09 11:44:28.833042 kuflow_temporal_common-1.5.0/kuflow_temporal_common/connection.py
--rw-r--r--   0        0        0     2488 2024-04-09 11:44:28.837042 kuflow_temporal_common-1.5.0/kuflow_temporal_common/converter.py
--rw-r--r--   0        0        0     1826 2024-04-09 11:44:28.837042 kuflow_temporal_common-1.5.0/kuflow_temporal_common/exceptions.py
--rw-r--r--   0        0        0     6306 2024-04-09 11:44:28.837042 kuflow_temporal_common-1.5.0/kuflow_temporal_common/worker_information_notifier.py
--rw-r--r--   0        0        0      933 2024-04-09 11:50:38.237372 kuflow_temporal_common-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     1562 1970-01-01 00:00:00.000000 kuflow_temporal_common-1.5.0/setup.py
--rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 kuflow_temporal_common-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      789 2024-04-25 11:49:37.329017 kuflow_temporal_common-1.5.1/README.md
+-rw-r--r--   0        0        0        6 2024-04-25 11:49:37.329017 kuflow_temporal_common-1.5.1/VERSION
+-rw-r--r--   0        0        0     1128 2024-04-25 11:49:37.329017 kuflow_temporal_common-1.5.1/kuflow_temporal_common/__init__.py
+-rw-r--r--   0        0        0    12231 2024-04-25 11:49:37.329017 kuflow_temporal_common-1.5.1/kuflow_temporal_common/_connection_config.py
+-rw-r--r--   0        0        0     2453 2024-04-25 11:49:37.329017 kuflow_temporal_common-1.5.1/kuflow_temporal_common/activity_utils.py
+-rw-r--r--   0        0        0     1592 2024-04-25 11:49:37.329017 kuflow_temporal_common-1.5.1/kuflow_temporal_common/attributes.py
+-rw-r--r--   0        0        0     4992 2024-04-25 11:49:37.329017 kuflow_temporal_common-1.5.1/kuflow_temporal_common/authentication.py
+-rw-r--r--   0        0        0     9144 2024-04-25 11:49:37.329017 kuflow_temporal_common-1.5.1/kuflow_temporal_common/connection.py
+-rw-r--r--   0        0        0     2488 2024-04-25 11:49:37.329017 kuflow_temporal_common-1.5.1/kuflow_temporal_common/converter.py
+-rw-r--r--   0        0        0     1826 2024-04-25 11:49:37.329017 kuflow_temporal_common-1.5.1/kuflow_temporal_common/exceptions.py
+-rw-r--r--   0        0        0     6306 2024-04-25 11:49:37.329017 kuflow_temporal_common-1.5.1/kuflow_temporal_common/worker_information_notifier.py
+-rw-r--r--   0        0        0      933 2024-04-25 11:56:58.484193 kuflow_temporal_common-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1562 1970-01-01 00:00:00.000000 kuflow_temporal_common-1.5.1/setup.py
+-rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 kuflow_temporal_common-1.5.1/PKG-INFO
```

### Comparing `kuflow_temporal_common-1.5.0/README.md` & `kuflow_temporal_common-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_common-1.5.0/kuflow_temporal_common/__init__.py` & `kuflow_temporal_common-1.5.1/kuflow_temporal_common/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
-__version__ = "1.5.0"
+__version__ = "1.5.1"
```

### Comparing `kuflow_temporal_common-1.5.0/kuflow_temporal_common/_connection_config.py` & `kuflow_temporal_common-1.5.1/kuflow_temporal_common/_connection_config.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_common-1.5.0/kuflow_temporal_common/activity_utils.py` & `kuflow_temporal_common-1.5.1/kuflow_temporal_common/activity_utils.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_common-1.5.0/kuflow_temporal_common/attributes.py` & `kuflow_temporal_common-1.5.1/kuflow_temporal_common/attributes.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_common-1.5.0/kuflow_temporal_common/authentication.py` & `kuflow_temporal_common-1.5.1/kuflow_temporal_common/authentication.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_common-1.5.0/kuflow_temporal_common/connection.py` & `kuflow_temporal_common-1.5.1/kuflow_temporal_common/connection.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_common-1.5.0/kuflow_temporal_common/converter.py` & `kuflow_temporal_common-1.5.1/kuflow_temporal_common/converter.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_common-1.5.0/kuflow_temporal_common/exceptions.py` & `kuflow_temporal_common-1.5.1/kuflow_temporal_common/exceptions.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_common-1.5.0/kuflow_temporal_common/worker_information_notifier.py` & `kuflow_temporal_common-1.5.1/kuflow_temporal_common/worker_information_notifier.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_common-1.5.0/pyproject.toml` & `kuflow_temporal_common-1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuflow-temporal-common"
-version = "1.5.0"
+version = "1.5.1"
 description = "KuFlow utilities to use Temporal.io"
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
 azure-core = "^1.26.4"
 isodate = "^0.6.1"
 temporalio = "~1.5.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.3.0"
 ruff = ">=0.1.8,<1.0.0"
```

### Comparing `kuflow_temporal_common-1.5.0/setup.py` & `kuflow_temporal_common-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['azure-core>=1.26.4,<2.0.0',
  'isodate>=0.6.1,<0.7.0',
- 'kuflow-rest>=1.5.0,<2.0.0',
+ 'kuflow-rest>=1.5.1,<2.0.0',
  'temporalio>=1.5.0,<1.6.0']
 
 setup_kwargs = {
     'name': 'kuflow-temporal-common',
-    'version': '1.5.0',
+    'version': '1.5.1',
     'description': 'KuFlow utilities to use Temporal.io',
     'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n[![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-common.svg)](https://pypi.org/project/kuflow-temporal-common)\n[![PyPI](https://img.shields.io/pypi/v/kuflow-temporal-common.svg)](https://pypi.org/project/kuflow-temporal-common)\n\n# KuFlow Temporal Common\n\nTODO\n\n## Documentation\n\nMore detailed docs are available in the [documentation pages](https://docs.kuflow.com/developers/).\n\n## Contributing\n\nWe are happy to receive your help and comments, together we will dance a wonderful KuFlow. Please review our [contribution guide](CONTRIBUTING.md).\n\n## License\n\n[MIT License](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n',
     'author': 'KuFlow S.L.',
     'author_email': 'kuflow@kuflow.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kuflow.com/',
```

### Comparing `kuflow_temporal_common-1.5.0/PKG-INFO` & `kuflow_temporal_common-1.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: kuflow-temporal-common
-Version: 1.5.0
+Version: 1.5.1
 Summary: KuFlow utilities to use Temporal.io
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
 Requires-Dist: azure-core (>=1.26.4,<2.0.0)
 Requires-Dist: isodate (>=0.6.1,<0.7.0)
-Requires-Dist: kuflow-rest (>=1.5.0,<2.0.0)
+Requires-Dist: kuflow-rest (>=1.5.1,<2.0.0)
 Requires-Dist: temporalio (>=1.5.0,<1.6.0)
 Project-URL: Documentation, https://docs.kuflow.com/
 Project-URL: Repository, https://github.com/kuflow/kuflow-sdk-python
 Description-Content-Type: text/markdown
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)
 [![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-common.svg)](https://pypi.org/project/kuflow-temporal-common)
```

