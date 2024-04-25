# Comparing `tmp/lazy_injector-0.0.1.tar.gz` & `tmp/lazy_injector-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_injector-0.0.1.tar", last modified: Mon Apr 22 18:52:33 2024, max compression
+gzip compressed data, was "lazy_injector-0.0.2.tar", last modified: Thu Apr 25 17:02:29 2024, max compression
```

## Comparing `lazy_injector-0.0.1.tar` & `lazy_injector-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 petmoe     (501) staff       (20)        0 2024-04-22 18:52:33.066541 lazy_injector-0.0.1/
--rw-r--r--   0 petmoe     (501) staff       (20)      240 2024-04-22 18:52:33.066279 lazy_injector-0.0.1/PKG-INFO
--rw-r--r--   0 petmoe     (501) staff       (20)     1103 2024-04-22 12:28:08.000000 lazy_injector-0.0.1/README.md
-drwxr-xr-x   0 petmoe     (501) staff       (20)        0 2024-04-22 18:52:33.064760 lazy_injector-0.0.1/lazy_injector/
--rw-r--r--   0 petmoe     (501) staff       (20)       50 2024-04-22 12:28:08.000000 lazy_injector-0.0.1/lazy_injector/__init__.py
--rw-r--r--   0 petmoe     (501) staff       (20)      655 2024-04-22 12:28:08.000000 lazy_injector-0.0.1/lazy_injector/dependency.py
--rw-r--r--   0 petmoe     (501) staff       (20)      220 2024-04-22 12:28:08.000000 lazy_injector-0.0.1/lazy_injector/exceptions.py
--rw-r--r--   0 petmoe     (501) staff       (20)     2902 2024-04-22 16:40:00.000000 lazy_injector-0.0.1/lazy_injector/provider.py
-drwxr-xr-x   0 petmoe     (501) staff       (20)        0 2024-04-22 18:52:33.065967 lazy_injector-0.0.1/lazy_injector.egg-info/
--rw-r--r--   0 petmoe     (501) staff       (20)      240 2024-04-22 18:52:33.000000 lazy_injector-0.0.1/lazy_injector.egg-info/PKG-INFO
--rw-r--r--   0 petmoe     (501) staff       (20)      302 2024-04-22 18:52:33.000000 lazy_injector-0.0.1/lazy_injector.egg-info/SOURCES.txt
--rw-r--r--   0 petmoe     (501) staff       (20)        1 2024-04-22 18:52:33.000000 lazy_injector-0.0.1/lazy_injector.egg-info/dependency_links.txt
--rw-r--r--   0 petmoe     (501) staff       (20)       14 2024-04-22 18:52:33.000000 lazy_injector-0.0.1/lazy_injector.egg-info/top_level.txt
--rw-r--r--   0 petmoe     (501) staff       (20)       38 2024-04-22 18:52:33.066592 lazy_injector-0.0.1/setup.cfg
--rw-r--r--   0 petmoe     (501) staff       (20)      435 2024-04-22 18:51:12.000000 lazy_injector-0.0.1/setup.py
-drwxr-xr-x   0 petmoe     (501) staff       (20)        0 2024-04-22 18:52:33.065512 lazy_injector-0.0.1/tests/
--rw-r--r--   0 petmoe     (501) staff       (20)     5758 2024-04-22 16:35:51.000000 lazy_injector-0.0.1/tests/test_lazy_injector.py
+drwxr-xr-x   0 petmoe     (501) staff       (20)        0 2024-04-25 17:02:29.134635 lazy_injector-0.0.2/
+-rw-r--r--   0 petmoe     (501) staff       (20)      240 2024-04-25 17:02:29.134407 lazy_injector-0.0.2/PKG-INFO
+-rw-r--r--   0 petmoe     (501) staff       (20)     1024 2024-04-22 18:55:11.000000 lazy_injector-0.0.2/README.md
+drwxr-xr-x   0 petmoe     (501) staff       (20)        0 2024-04-25 17:02:29.132641 lazy_injector-0.0.2/lazy_injector/
+-rw-r--r--   0 petmoe     (501) staff       (20)       75 2024-04-25 16:54:01.000000 lazy_injector-0.0.2/lazy_injector/__init__.py
+-rw-r--r--   0 petmoe     (501) staff       (20)      661 2024-04-25 16:48:03.000000 lazy_injector-0.0.2/lazy_injector/dependency.py
+-rw-r--r--   0 petmoe     (501) staff       (20)      220 2024-04-22 12:28:08.000000 lazy_injector-0.0.2/lazy_injector/exceptions.py
+-rw-r--r--   0 petmoe     (501) staff       (20)     2880 2024-04-23 14:44:31.000000 lazy_injector-0.0.2/lazy_injector/provider.py
+-rw-r--r--   0 petmoe     (501) staff       (20)     1468 2024-04-25 16:49:01.000000 lazy_injector-0.0.2/lazy_injector/singleton.py
+drwxr-xr-x   0 petmoe     (501) staff       (20)        0 2024-04-25 17:02:29.134197 lazy_injector-0.0.2/lazy_injector.egg-info/
+-rw-r--r--   0 petmoe     (501) staff       (20)      240 2024-04-25 17:02:29.000000 lazy_injector-0.0.2/lazy_injector.egg-info/PKG-INFO
+-rw-r--r--   0 petmoe     (501) staff       (20)      377 2024-04-25 17:02:29.000000 lazy_injector-0.0.2/lazy_injector.egg-info/SOURCES.txt
+-rw-r--r--   0 petmoe     (501) staff       (20)        1 2024-04-25 17:02:29.000000 lazy_injector-0.0.2/lazy_injector.egg-info/dependency_links.txt
+-rw-r--r--   0 petmoe     (501) staff       (20)       14 2024-04-25 17:02:29.000000 lazy_injector-0.0.2/lazy_injector.egg-info/top_level.txt
+-rw-r--r--   0 petmoe     (501) staff       (20)       38 2024-04-25 17:02:29.134681 lazy_injector-0.0.2/setup.cfg
+-rw-r--r--   0 petmoe     (501) staff       (20)      435 2024-04-25 16:59:44.000000 lazy_injector-0.0.2/setup.py
+drwxr-xr-x   0 petmoe     (501) staff       (20)        0 2024-04-25 17:02:29.133915 lazy_injector-0.0.2/tests/
+-rw-r--r--   0 petmoe     (501) staff       (20)      819 2024-04-23 14:36:39.000000 lazy_injector-0.0.2/tests/test_flask_app.py
+-rw-r--r--   0 petmoe     (501) staff       (20)     5664 2024-04-25 16:52:18.000000 lazy_injector-0.0.2/tests/test_lazy_injector.py
+-rw-r--r--   0 petmoe     (501) staff       (20)      596 2024-04-25 16:58:12.000000 lazy_injector-0.0.2/tests/test_singleton.py
```

### Comparing `lazy_injector-0.0.1/README.md` & `lazy_injector-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Introduction
 Simple dependency injection framework for python
 
 # Installation
-Can be installed from source using the `pip install -e` command
+Can be installed from pypi:
 ```sh
-> pip install -e https://github.com/pettermoe95/python-lazy-injector
+> pip install lazy-injector
 ```
 # Usage
-#### Registering dependencies
+### Registering dependencies
 
 ```python
 from lazy_injector import register, Dependency
 
 class Foo:
     ...
 
@@ -20,15 +20,15 @@
 
 
 register(
     Dependency(lambda: "dependency", str),
     Dependency(sample_provider, Foo)
 )
 ```
-#### Injecting dependencies
+### Injecting dependencies
 There are two functions to use, the `inject` and the `lazy`. The lazy must we used to get the dependency as a
 default argument inside a function. I.e. `lazy(str)` will produce a placeholder default value that the laze_injector
 can look for. The function needs to have the `@inject` set as a decorator, so that the lazy_injector
 will replace the placeholder value with the actual dependency.
 
 Here is an example:
 ```python
```

### Comparing `lazy_injector-0.0.1/lazy_injector/dependency.py` & `lazy_injector-0.0.2/lazy_injector/dependency.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable, Type, Any
+from typing import Callable, Dict, Type, Any
 from inspect import isclass
 
 
 def get_class_name(obj: Any) -> str:
     if not isclass(obj):
         class_name = str(obj.__class__.__name__)
     else:
```

### Comparing `lazy_injector-0.0.1/lazy_injector/provider.py` & `lazy_injector-0.0.2/lazy_injector/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .dependency import Dependency, Lazy, get_class_name
 from .exceptions import DuplicateDependencyError
 from typing import Any, Dict, Type, List, Union
-from inspect import FullArgSpec, getfullargspec, isfunction, ismethod
+from inspect import FullArgSpec, getfullargspec
 import logging
 
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
```

### Comparing `lazy_injector-0.0.1/tests/test_lazy_injector.py` & `lazy_injector-0.0.2/tests/test_lazy_injector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from typing import Tuple
-from lazy_injector import Dependency, reset, register, find_dependency, lazy, inject, get_class_name
+from lazy_injector import Dependency, register, find_dependency, lazy, inject, get_class_name
 from lazy_injector.exceptions import DuplicateDependencyError
+from tests.utils import set_up
 from pytest import raises
 
-def set_up(func):
-    def wrapper(*args, **kwargs):
-        reset()
-        return func(*args, **kwargs)
-    return wrapper
 
 
 def dependency_provider():
     return "it works"
 
 
 @inject
@@ -217,7 +213,9 @@
 
     a, my_str, b, my_int = init_inject.before_and_after(a="a", b="b")
     assert a == "a"
     assert b == "b"
     assert my_str == dependency_provider()
     assert my_int == 7
 
+
+
```

