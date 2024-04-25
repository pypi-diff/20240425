# Comparing `tmp/alana-0.0.7.tar.gz` & `tmp/alana-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alana-0.0.7.tar", last modified: Wed Apr 24 15:30:17 2024, max compression
+gzip compressed data, was "alana-0.0.8.tar", last modified: Thu Apr 25 12:06:23 2024, max compression
```

## Comparing `alana-0.0.7.tar` & `alana-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:30:17.394670 alana-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-24 15:30:13.000000 alana-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-24 15:30:17.394670 alana-0.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:30:17.394670 alana-0.0.7/alana/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-24 15:30:13.000000 alana-0.0.7/alana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-24 15:30:13.000000 alana-0.0.7/alana/aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-24 15:30:13.000000 alana-0.0.7/alana/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-04-24 15:30:13.000000 alana-0.0.7/alana/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)    23882 2024-04-24 15:30:13.000000 alana-0.0.7/alana/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-24 15:30:13.000000 alana-0.0.7/alana/prompt_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:30:17.394670 alana-0.0.7/alana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-24 15:30:17.000000 alana-0.0.7/alana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-24 15:30:17.000000 alana-0.0.7/alana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:30:17.000000 alana-0.0.7/alana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 15:30:17.000000 alana-0.0.7/alana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 15:30:17.000000 alana-0.0.7/alana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:30:17.394670 alana-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-24 15:30:13.000000 alana-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:23.685408 alana-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-25 12:06:19.000000 alana-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-25 12:06:23.685408 alana-0.0.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:23.685408 alana-0.0.8/alana/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-25 12:06:19.000000 alana-0.0.8/alana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-25 12:06:19.000000 alana-0.0.8/alana/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-25 12:06:19.000000 alana-0.0.8/alana/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-04-25 12:06:19.000000 alana-0.0.8/alana/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23737 2024-04-25 12:06:19.000000 alana-0.0.8/alana/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-25 12:06:19.000000 alana-0.0.8/alana/prompt_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:23.685408 alana-0.0.8/alana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-25 12:06:23.000000 alana-0.0.8/alana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-25 12:06:23.000000 alana-0.0.8/alana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 12:06:23.000000 alana-0.0.8/alana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 12:06:23.000000 alana-0.0.8/alana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 12:06:23.000000 alana-0.0.8/alana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 12:06:23.685408 alana-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-25 12:06:19.000000 alana-0.0.8/setup.py
```

### Comparing `alana-0.0.7/LICENSE` & `alana-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alana-0.0.7/PKG-INFO` & `alana-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alana
-Version: 0.0.7
+Version: 0.0.8
 Summary: Utilities for Alana, and maybe you too. Mostly geared toward LLM-heavy workflows.
 Home-page: https://github.com/alat-rights/alana-utilities
 Author: Alana
 Author-email: hi@alana.computer
 Keywords: LLM,utilities
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `alana-0.0.7/alana/__init__.py` & `alana-0.0.8/alana/__init__.py`

 * *Files identical despite different names*

### Comparing `alana-0.0.7/alana/aliases.py` & `alana-0.0.8/alana/aliases.py`

 * *Files identical despite different names*

### Comparing `alana-0.0.7/alana/color.py` & `alana-0.0.8/alana/color.py`

 * *Files identical despite different names*

### Comparing `alana-0.0.7/alana/globals.py` & `alana-0.0.8/alana/globals.py`

 * *Files identical despite different names*

### Comparing `alana-0.0.7/alana/prompt.py` & `alana-0.0.8/alana/prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import re
 import os
-from typing import List, Dict, Optional, Union, Literal, Any, TypedDict, Unpack, Tuple
+from typing import List, Dict, Optional, Union, Literal, Any
 from anthropic import Anthropic
-from anthropic._types import Headers, Query, Body, NotGiven
 from anthropic.types import Message, MessageParam
-from anthropic.types.message_create_params import Metadata
 
 from alana.color import red, yellow
 from alana import globals
 
 """
 class RequestParams(TypedDict, total=False):
     metadata: Metadata | NotGiven
```

### Comparing `alana-0.0.7/alana/prompt_async.py` & `alana-0.0.8/alana/prompt_async.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,21 @@
-import asyncio
 from anthropic import AsyncAnthropic
 import os
 from alana import yellow, red
 from alana import globals
 from alana.prompt import _append_assistant_message, _construct_messages
 from typing import List, Optional, Callable, Any
 from anthropic.types import Message, MessageParam
 
 client = AsyncAnthropic(
     # This is the default and can be omitted
     api_key=os.environ.get("ANTHROPIC_API_KEY"),
 )
 
 
-async def main() -> None:
-    message = await client.messages.create(
-        max_tokens=1024,
-        messages=[
-            {
-                "role": "user",
-                "content": "Hello, Claude",
-            }
-        ],
-        model="claude-3-opus-20240229",
-    )
-    print(message.content)
-
-
-asyncio.run(main())
-
-
 async def agen_msg(
     messages: List[MessageParam],
     system: str = "",
     model: str = globals.DEFAULT_MODEL,
     api_key: Optional[str] = None,
     max_tokens=1024,
     temperature=1.0,
```

### Comparing `alana-0.0.7/alana.egg-info/PKG-INFO` & `alana-0.0.8/alana.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alana
-Version: 0.0.7
+Version: 0.0.8
 Summary: Utilities for Alana, and maybe you too. Mostly geared toward LLM-heavy workflows.
 Home-page: https://github.com/alat-rights/alana-utilities
 Author: Alana
 Author-email: hi@alana.computer
 Keywords: LLM,utilities
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `alana-0.0.7/setup.py` & `alana-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 
 setup(
    name='alana',
-   version='0.0.7',  # Update the version number as needed
+   version='0.0.8',  # Update the version number as needed
    author='Alana',
    author_email='hi@alana.computer',
    description='Utilities for Alana, and maybe you too. Mostly geared toward LLM-heavy workflows.',
    long_description="""
 🎵 Note: I have been making new releases frequently. Make sure your package is up-to-date!
 
 ⚠️ Warning: This library is in active early development! No guarantees are made for backward compatibility. The library is NOT production-ready.
```

