# Comparing `tmp/streamlit_chat_handler-0.0.2.tar.gz` & `tmp/streamlit_chat_handler-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_chat_handler-0.0.2.tar", last modified: Tue Apr 23 14:16:45 2024, max compression
+gzip compressed data, was "streamlit_chat_handler-0.0.3.tar", last modified: Thu Apr 25 02:28:49 2024, max compression
```

## Comparing `streamlit_chat_handler-0.0.2.tar` & `streamlit_chat_handler-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-23 14:16:45.109085 streamlit_chat_handler-0.0.2/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1083 2024-04-23 04:06:28.000000 streamlit_chat_handler-0.0.2/LICENSE
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3710 2024-04-23 14:16:45.109085 streamlit_chat_handler-0.0.2/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2780 2024-04-23 04:03:07.000000 streamlit_chat_handler-0.0.2/README.md
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-23 14:16:45.105085 streamlit_chat_handler-0.0.2/examples/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      690 2024-04-23 03:41:26.000000 streamlit_chat_handler-0.0.2/examples/template.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1308 2024-04-23 14:16:01.000000 streamlit_chat_handler-0.0.2/pyproject.toml
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      356 2024-04-23 01:52:45.000000 streamlit_chat_handler-0.0.2/requirements.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2024-04-23 14:16:45.109085 streamlit_chat_handler-0.0.2/setup.cfg
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-23 14:16:45.105085 streamlit_chat_handler-0.0.2/streamlit_chat_handler/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      110 2024-04-23 00:45:47.000000 streamlit_chat_handler-0.0.2/streamlit_chat_handler/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7414 2024-04-23 14:15:01.000000 streamlit_chat_handler-0.0.2/streamlit_chat_handler/_handler.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2056 2024-04-23 03:47:04.000000 streamlit_chat_handler-0.0.2/streamlit_chat_handler/types.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-23 14:16:45.105085 streamlit_chat_handler-0.0.2/streamlit_chat_handler.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3710 2024-04-23 14:16:45.000000 streamlit_chat_handler-0.0.2/streamlit_chat_handler.egg-info/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      401 2024-04-23 14:16:45.000000 streamlit_chat_handler-0.0.2/streamlit_chat_handler.egg-info/SOURCES.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2024-04-23 14:16:45.000000 streamlit_chat_handler-0.0.2/streamlit_chat_handler.egg-info/dependency_links.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      272 2024-04-23 14:16:45.000000 streamlit_chat_handler-0.0.2/streamlit_chat_handler.egg-info/requires.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       42 2024-04-23 14:16:45.000000 streamlit_chat_handler-0.0.2/streamlit_chat_handler.egg-info/top_level.txt
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-25 02:28:49.027790 streamlit_chat_handler-0.0.3/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1083 2024-04-23 04:06:28.000000 streamlit_chat_handler-0.0.3/LICENSE
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3710 2024-04-25 02:28:49.027790 streamlit_chat_handler-0.0.3/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2780 2024-04-23 04:03:07.000000 streamlit_chat_handler-0.0.3/README.md
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-25 02:28:49.027790 streamlit_chat_handler-0.0.3/examples/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      690 2024-04-23 03:41:26.000000 streamlit_chat_handler-0.0.3/examples/template.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1308 2024-04-25 02:27:43.000000 streamlit_chat_handler-0.0.3/pyproject.toml
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      356 2024-04-23 01:52:45.000000 streamlit_chat_handler-0.0.3/requirements.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2024-04-25 02:28:49.027790 streamlit_chat_handler-0.0.3/setup.cfg
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-25 02:28:49.027790 streamlit_chat_handler-0.0.3/streamlit_chat_handler/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      110 2024-04-23 00:45:47.000000 streamlit_chat_handler-0.0.3/streamlit_chat_handler/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7434 2024-04-25 02:27:16.000000 streamlit_chat_handler-0.0.3/streamlit_chat_handler/_handler.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2056 2024-04-23 03:47:04.000000 streamlit_chat_handler-0.0.3/streamlit_chat_handler/types.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-25 02:28:49.027790 streamlit_chat_handler-0.0.3/streamlit_chat_handler.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3710 2024-04-25 02:28:49.000000 streamlit_chat_handler-0.0.3/streamlit_chat_handler.egg-info/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      401 2024-04-25 02:28:49.000000 streamlit_chat_handler-0.0.3/streamlit_chat_handler.egg-info/SOURCES.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2024-04-25 02:28:49.000000 streamlit_chat_handler-0.0.3/streamlit_chat_handler.egg-info/dependency_links.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      272 2024-04-25 02:28:49.000000 streamlit_chat_handler-0.0.3/streamlit_chat_handler.egg-info/requires.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       42 2024-04-25 02:28:49.000000 streamlit_chat_handler-0.0.3/streamlit_chat_handler.egg-info/top_level.txt
```

### Comparing `streamlit_chat_handler-0.0.2/LICENSE` & `streamlit_chat_handler-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.0.2/PKG-INFO` & `streamlit_chat_handler-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_chat_handler
-Version: 0.0.2
+Version: 0.0.3
 Summary: ...
 Author-email: Eduardo Messias de Morais <emdemor415@gmail.com>
 Keywords: sample,setuptools,development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit==1.33.0
```

### Comparing `streamlit_chat_handler-0.0.2/README.md` & `streamlit_chat_handler-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.0.2/examples/template.py` & `streamlit_chat_handler-0.0.3/examples/template.py`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.0.2/pyproject.toml` & `streamlit_chat_handler-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
 keywords = ["sample", "setuptools", "development"]
 authors = [
   {name = "Eduardo Messias de Morais", email = "emdemor415@gmail.com" },
 ]
-version = "0.0.2"
+version = "0.0.3"
 dynamic = ["dependencies"]
 
 [project.optional-dependencies]
 lint = [
     "black==23.7.0",
     "flake8==6.1.0",
     "Flake8-pyproject==1.2.3",
```

### Comparing `streamlit_chat_handler-0.0.2/streamlit_chat_handler/_handler.py` & `streamlit_chat_handler-0.0.3/streamlit_chat_handler/_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,15 @@
             kwargs=kwargs,
         )
 
         self.session_state[self.elements_label][index] = chat_element
 
         if render:
             return chat_element.render()
+        return self
 
     def render_last(self) -> None:
         """Render the last added chat element."""
         last_key, last_element = _get_last_item(self.session_state[self.elements_label])
         self.rendered_elements[last_key] = last_element.render()
 
     def render(self) -> "StreamlitChatHandler":
```

### Comparing `streamlit_chat_handler-0.0.2/streamlit_chat_handler/types.py` & `streamlit_chat_handler-0.0.3/streamlit_chat_handler/types.py`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.0.2/streamlit_chat_handler.egg-info/PKG-INFO` & `streamlit_chat_handler-0.0.3/streamlit_chat_handler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_chat_handler
-Version: 0.0.2
+Version: 0.0.3
 Summary: ...
 Author-email: Eduardo Messias de Morais <emdemor415@gmail.com>
 Keywords: sample,setuptools,development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit==1.33.0
```

