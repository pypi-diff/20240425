# Comparing `tmp/atksh-utils-0.8.4.tar.gz` & `tmp/atksh_utils-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atksh-utils-0.8.4.tar", last modified: Fri Apr 12 03:34:23 2024, max compression
+gzip compressed data, was "atksh_utils-0.8.5.tar", last modified: Thu Apr 25 04:54:49 2024, max compression
```

## Comparing `atksh-utils-0.8.4.tar` & `atksh_utils-0.8.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:23.411105 atksh-utils-0.8.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:23.403105 atksh-utils-0.8.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:23.403105 atksh-utils-0.8.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/.github/workflows/publish_to_pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-12 03:34:23.411105 atksh-utils-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-12 03:34:23.411105 atksh-utils-0.8.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:23.403105 atksh-utils-0.8.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:23.403105 atksh-utils-0.8.4/src/atksh_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:23.407105 atksh-utils-0.8.4/src/atksh_utils/basic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/basic/functools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:23.407105 atksh-utils-0.8.4/src/atksh_utils/nlp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/nlp/str_kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:23.407105 atksh-utils-0.8.4/src/atksh_utils/openai/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25737 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/openai/api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6309 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/openai/askgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/openai/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/openai/history.py
--rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/openai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/openai/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    21358 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/openai/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 03:34:23.000000 atksh-utils-0.8.4/src/atksh_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:23.411105 atksh-utils-0.8.4/src/atksh_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-12 03:34:23.000000 atksh-utils-0.8.4/src/atksh_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-12 03:34:23.000000 atksh-utils-0.8.4/src/atksh_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:34:23.000000 atksh-utils-0.8.4/src/atksh_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-12 03:34:23.000000 atksh-utils-0.8.4/src/atksh_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-12 03:34:23.000000 atksh-utils-0.8.4/src/atksh_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 03:34:23.000000 atksh-utils-0.8.4/src/atksh_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:23.411105 atksh-utils-0.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:49.417315 atksh_utils-0.8.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:49.409314 atksh_utils-0.8.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:49.413315 atksh_utils-0.8.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/.github/workflows/publish_to_pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-25 04:54:49.417315 atksh_utils-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-25 04:54:49.417315 atksh_utils-0.8.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:49.409314 atksh_utils-0.8.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:49.413315 atksh_utils-0.8.5/src/atksh_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:49.413315 atksh_utils-0.8.5/src/atksh_utils/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/basic/functools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:49.413315 atksh_utils-0.8.5/src/atksh_utils/nlp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/nlp/str_kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:49.417315 atksh_utils-0.8.5/src/atksh_utils/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25773 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/openai/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6309 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/openai/askgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/openai/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/openai/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/openai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/openai/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21407 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/src/atksh_utils/openai/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 04:54:49.000000 atksh_utils-0.8.5/src/atksh_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:49.417315 atksh_utils-0.8.5/src/atksh_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-25 04:54:49.000000 atksh_utils-0.8.5/src/atksh_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-25 04:54:49.000000 atksh_utils-0.8.5/src/atksh_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 04:54:49.000000 atksh_utils-0.8.5/src/atksh_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-25 04:54:49.000000 atksh_utils-0.8.5/src/atksh_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-25 04:54:49.000000 atksh_utils-0.8.5/src/atksh_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 04:54:49.000000 atksh_utils-0.8.5/src/atksh_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:49.417315 atksh_utils-0.8.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:54:41.000000 atksh_utils-0.8.5/tests/__init__.py
```

### Comparing `atksh-utils-0.8.4/.github/workflows/publish_to_pypi.yaml` & `atksh_utils-0.8.5/.github/workflows/publish_to_pypi.yaml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.8.4/.gitignore` & `atksh_utils-0.8.5/.gitignore`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.8.4/LICENSE` & `atksh_utils-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.8.4/PKG-INFO` & `atksh_utils-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.8.4
+Version: 0.8.5
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
         
@@ -25,15 +25,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai~=1.14.2
+Requires-Dist: openai~=1.23.6
 Requires-Dist: beautifulsoup4<5.0.0,>=4.11.1
 Requires-Dist: requests<3.0.0,>=2.0.0
 Requires-Dist: duckduckgo_search~=4.1.1
 Requires-Dist: dill<0.4.0,>=0.3.7
 Requires-Dist: numba<0.59.0,>=0.56.4
 Requires-Dist: pylatexenc==2.10
 Requires-Dist: scipy<2.0.0,>=1.9.0
```

### Comparing `atksh-utils-0.8.4/README.md` & `atksh_utils-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.8.4/pyproject.toml` & `atksh_utils-0.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=62.6", "setuptools_scm[toml]>=6.2", "wheel"]
 
 [project]
 dependencies = [
-  "openai~=1.14.2",
+  "openai~=1.23.6",
   "beautifulsoup4>=4.11.1,<5.0.0",
   "requests>=2.0.0,<3.0.0",
   "duckduckgo_search~=4.1.1",
   "dill>=0.3.7,<0.4.0",
   "numba>=0.56.4,<0.59.0",
   "pylatexenc==2.10",
   "scipy>=1.9.0,<2.0.0",
```

### Comparing `atksh-utils-0.8.4/src/atksh_utils/basic/functools.py` & `atksh_utils-0.8.5/src/atksh_utils/basic/functools.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.8.4/src/atksh_utils/nlp/str_kernel.py` & `atksh_utils-0.8.5/src/atksh_utils/nlp/str_kernel.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.8.4/src/atksh_utils/openai/api.py` & `atksh_utils-0.8.5/src/atksh_utils/openai/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         self.model_name = model_name
         self.temperature = temperature
         self.top_p = top_p
         self._functions: list[FunctionWrapper] = []
         self.max_num_messages = max_num_messages
         if max_num_input_tokens > 0:
             self.max_num_input_tokens = max_num_input_tokens
-        elif "gpt-4-0125-preview" in self.model_name:
+        elif "gpt-4-0125-preview" in self.model_name or "gpt-4-turbo" in self.model_name:
             self.max_num_input_tokens = 120000
         elif "gpt-4-32k-0613" in self.model_name:
             self.max_num_input_tokens = 28000
         else:
             self.max_num_input_tokens = 15000
         self.is_child = is_child
```

### Comparing `atksh-utils-0.8.4/src/atksh_utils/openai/askgpt.py` & `atksh_utils-0.8.5/src/atksh_utils/openai/askgpt.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.8.4/src/atksh_utils/openai/functional.py` & `atksh_utils-0.8.5/src/atksh_utils/openai/functional.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.8.4/src/atksh_utils/openai/prompt.py` & `atksh_utils-0.8.5/src/atksh_utils/openai/prompt.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.8.4/src/atksh_utils/openai/token.py` & `atksh_utils-0.8.5/src/atksh_utils/openai/token.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.8.4/src/atksh_utils/openai/tool.py` & `atksh_utils-0.8.5/src/atksh_utils/openai/tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,16 +32,15 @@
 )
 from .token import clean_text, count_token, sub_tokenize
 
 urllib3.disable_warnings(InsecureRequestWarning)
 
 # Create a temporary directory for storing files to $HOME/.cache/askgpt/ or OPENAI_TOOLS_PYTHON_CACHE_DIR
 CACHE_DIR = os.getenv(
-    "OPENAI_TOOLS_PYTHON_CACHE_DIR",
-    os.path.join(os.path.expanduser("~"), ".cache", "askgpt")
+    "OPENAI_TOOLS_PYTHON_CACHE_DIR", os.path.join(os.path.expanduser("~"), ".cache", "askgpt")
 )
 os.makedirs(CACHE_DIR, exist_ok=True)
 SESSION_PATH = os.path.join(CACHE_DIR, "session.pkl")
 
 Print_LOCK = Lock()
 DDGS_LOCK = Lock()
 API_LOCK = Semaphore(16)
@@ -253,15 +252,17 @@
 
     return translate
 
 
 def get_browser_functions(ai: "OpenAI"):
     visit_page_model_name = ai.model_name
     visit_page_max_context_length = (
-        100000 if "gpt-4-0125-preview" in visit_page_model_name else 10000
+        100000
+        if "gpt-4-preview" in visit_page_model_name or "gpt-4-turbo" in visit_page_model_name
+        else 10000
     )
     visit_page_max_context_length -= count_token(VISIT_PAGE_SUMMARIZE_PROMPT)
 
     def _search_summarize(query_text: str, results: str) -> str:
         """Summarizes the query text and results."""
         search_result_child = ai.make_child(ai.model_name, temperature=0.2, top_p=0.8)
         search_result_child.set_system_prompt(SEARCH_RESULT_SUMMARIZE_PROMPT)
```

### Comparing `atksh-utils-0.8.4/src/atksh_utils.egg-info/PKG-INFO` & `atksh_utils-0.8.5/src/atksh_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.8.4
+Version: 0.8.5
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
         
@@ -25,15 +25,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai~=1.14.2
+Requires-Dist: openai~=1.23.6
 Requires-Dist: beautifulsoup4<5.0.0,>=4.11.1
 Requires-Dist: requests<3.0.0,>=2.0.0
 Requires-Dist: duckduckgo_search~=4.1.1
 Requires-Dist: dill<0.4.0,>=0.3.7
 Requires-Dist: numba<0.59.0,>=0.56.4
 Requires-Dist: pylatexenc==2.10
 Requires-Dist: scipy<2.0.0,>=1.9.0
```

### Comparing `atksh-utils-0.8.4/src/atksh_utils.egg-info/SOURCES.txt` & `atksh_utils-0.8.5/src/atksh_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

