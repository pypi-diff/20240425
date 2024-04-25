# Comparing `tmp/vbao_MVVM-0.2.1.tar.gz` & `tmp/vbao_mvvm-0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbao_MVVM-0.2.1.tar", last modified: Wed Apr 10 05:19:28 2024, max compression
+gzip compressed data, was "vbao_mvvm-0.3a1.tar", last modified: Thu Apr 25 16:39:50 2024, max compression
```

## Comparing `vbao_MVVM-0.2.1.tar` & `vbao_mvvm-0.3a1.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 05:19:28.954478 vbao_MVVM-0.2.1/
--rw-rw-rw-   0        0        0    27030 2024-03-31 08:06:41.000000 vbao_MVVM-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     1417 2024-04-10 05:19:28.953478 vbao_MVVM-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      844 2024-03-31 08:06:41.000000 vbao_MVVM-0.2.1/README.md
--rw-rw-rw-   0        0        0      653 2024-04-10 05:17:11.000000 vbao_MVVM-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-10 05:19:28.954478 vbao_MVVM-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-10 05:19:28.947479 vbao_MVVM-0.2.1/vbao/
--rw-rw-rw-   0        0        0      222 2024-04-07 08:12:26.000000 vbao_MVVM-0.2.1/vbao/__init__.py
--rw-rw-rw-   0        0        0     2627 2024-04-10 05:16:32.000000 vbao_MVVM-0.2.1/vbao/base.py
--rw-rw-rw-   0        0        0     1445 2024-04-10 05:16:32.000000 vbao_MVVM-0.2.1/vbao/config.py
--rw-rw-rw-   0        0        0     3294 2024-04-10 05:16:32.000000 vbao_MVVM-0.2.1/vbao/convenient_class.py
--rw-rw-rw-   0        0        0     5604 2024-04-10 05:16:32.000000 vbao_MVVM-0.2.1/vbao/core.py
--rw-rw-rw-   0        0        0     4057 2024-04-10 05:16:32.000000 vbao_MVVM-0.2.1/vbao/mixin.py
-drwxrwxrwx   0        0        0        0 2024-04-10 05:19:28.952479 vbao_MVVM-0.2.1/vbao_MVVM.egg-info/
--rw-rw-rw-   0        0        0     1417 2024-04-10 05:19:28.000000 vbao_MVVM-0.2.1/vbao_MVVM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2024-04-10 05:19:28.000000 vbao_MVVM-0.2.1/vbao_MVVM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 05:19:28.000000 vbao_MVVM-0.2.1/vbao_MVVM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-10 05:19:28.000000 vbao_MVVM-0.2.1/vbao_MVVM.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 16:39:50.645627 vbao_mvvm-0.3a1/
+-rw-rw-rw-   0        0        0    27030 2024-03-31 08:06:41.000000 vbao_mvvm-0.3a1/LICENSE
+-rw-rw-rw-   0        0        0     1390 2024-04-25 16:39:50.644611 vbao_mvvm-0.3a1/PKG-INFO
+-rw-rw-rw-   0        0        0      844 2024-03-31 08:06:41.000000 vbao_mvvm-0.3a1/README.md
+-rw-rw-rw-   0        0        0      624 2024-04-25 16:39:23.000000 vbao_mvvm-0.3a1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-25 16:39:50.645627 vbao_mvvm-0.3a1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-25 16:39:50.637478 vbao_mvvm-0.3a1/test/
+-rw-rw-rw-   0        0        0      766 2024-04-22 08:23:43.000000 vbao_mvvm-0.3a1/test/test_util.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:39:50.639510 vbao_mvvm-0.3a1/vbao/
+-rw-rw-rw-   0        0        0      524 2024-04-22 08:02:37.000000 vbao_mvvm-0.3a1/vbao/__init__.py
+-rw-rw-rw-   0        0        0     2627 2024-04-10 05:16:32.000000 vbao_mvvm-0.3a1/vbao/base.py
+-rw-rw-rw-   0        0        0     4479 2024-04-25 15:02:50.000000 vbao_mvvm-0.3a1/vbao/config.py
+-rw-rw-rw-   0        0        0     3264 2024-04-22 05:01:18.000000 vbao_mvvm-0.3a1/vbao/convenient_class.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:39:50.641541 vbao_mvvm-0.3a1/vbao/core/
+-rw-rw-rw-   0        0        0       49 2024-04-22 05:16:27.000000 vbao_mvvm-0.3a1/vbao/core/__init__.py
+-rw-rw-rw-   0        0        0     4794 2024-04-25 14:03:21.000000 vbao_mvvm-0.3a1/vbao/core/core.py
+-rw-rw-rw-   0        0        0     8174 2024-04-25 14:47:58.000000 vbao_mvvm-0.3a1/vbao/core/mixin.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:39:50.644611 vbao_mvvm-0.3a1/vbao_MVVM.egg-info/
+-rw-rw-rw-   0        0        0     1390 2024-04-25 16:39:50.000000 vbao_mvvm-0.3a1/vbao_MVVM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2024-04-25 16:39:50.000000 vbao_mvvm-0.3a1/vbao_MVVM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 16:39:50.000000 vbao_mvvm-0.3a1/vbao_MVVM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-25 16:39:50.000000 vbao_mvvm-0.3a1/vbao_MVVM.egg-info/top_level.txt
```

### Comparing `vbao_MVVM-0.2.1/LICENSE` & `vbao_mvvm-0.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `vbao_MVVM-0.2.1/PKG-INFO` & `vbao_mvvm-0.3a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: vbao_MVVM
-Version: 0.2.1
+Version: 0.3a1
 Summary: A library aiming for building an MVVM (or MVFM) project
-Author-email: Meidozuki <author@example.com>
+Author: Meidozuki
 Project-URL: Homepage, https://github.com/Meidozuki/VBAO
 Project-URL: Bug Tracker, https://github.com/Meidozuki/VBAO/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `vbao_MVVM-0.2.1/README.md` & `vbao_mvvm-0.3a1/README.md`

 * *Files identical despite different names*

### Comparing `vbao_MVVM-0.2.1/pyproject.toml` & `vbao_mvvm-0.3a1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vbao_MVVM"
-version = "0.2.1"
+version = "0.3a1"
 authors = [
-  { name="Meidozuki", email="author@example.com" },
+  { name="Meidozuki"},
 ]
 description = "A library aiming for building an MVVM (or MVFM) project"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)",
```

### Comparing `vbao_MVVM-0.2.1/vbao/base.py` & `vbao_mvvm-0.3a1/vbao/base.py`

 * *Files identical despite different names*

### Comparing `vbao_MVVM-0.2.1/vbao/convenient_class.py` & `vbao_mvvm-0.3a1/vbao/convenient_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 from abc import ABC
 from functools import wraps
 from typing import final
 
 from .base import CommandBase, CommandListenerBase, PropertyListenerBase
-from .core import ViewModel
 
 
 @final
 class DummyPropListener(PropertyListenerBase):
     # No need to take args, except for `to_whom` to keep compatible with normal listeners
     # Throws as soon as possible
     @wraps(PropertyListenerBase.__init__)
@@ -55,17 +54,17 @@
 
 
 class CommandBaseWithOwner(CommandBase, ABC):
     """
     __init__ receives an argument and stores it in self.owner.
     """
 
-    def __init__(self, owner: ViewModel, *args, **kwargs):
+    def __init__(self, owner, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.owner: ViewModel = owner
+        self.owner: vbao.core.ViewModel = owner
 
 
 class CommandBaseWithDict(CommandBase, ABC):
     """
     __init__ receives a dict and stores it in self.dict. Allows None.
     """
```

### Comparing `vbao_MVVM-0.2.1/vbao/core.py` & `vbao_mvvm-0.3a1/vbao/core/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,27 +10,17 @@
 #
 # You should have received a copy of the GNU Lesser General Public License along with VBAO.
 # If not, see <https://www.gnu.org/licenses/>.
 
 import logging
 from typing import *
 
-from .base import *
-from .mixin import PropertyMixin, CommandMixin
-
-DictCons = dict
-
-
-def use_easydict(b=True):
-    global DictCons
-    if b:
-        from easydict import EasyDict
-        DictCons = EasyDict
-    else:
-        DictCons = dict
+from vbao.base import *
+from vbao.config import DictCons
+from .mixin import PropertyMixin, CommandMixin, PropertyCommandMixin
 
 
 class Model(PropertyMixin):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._prop_notice = PropertyNotifier()
 
@@ -44,15 +34,15 @@
             raise TypeError(f"expect PropertyListenerBase, but get {type(listener)}")
         self._prop_notice.addNotification(listener)
 
     def triggerPropertyNotifications(self, name: str):
         self._prop_notice.triggerPropertyNotifications(name)
 
 
-class ViewModel(PropertyMixin, CommandMixin):
+class ViewModel(PropertyCommandMixin):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._prop_notice = PropertyNotifier()
         self._cmd_notice = CommandNotifier()
         self._prop_listener = None
         # Viewmodel contains Model, the result of running “commands” of Model can be directly seen
         self.model = None  # lots of operations will be done with Model, model is better than _model
@@ -89,42 +79,25 @@
     @property
     def isModelSet(self):
         return self.model is not None
 
     def setListener(self, listener: PropertyListenerBase):
         self._prop_listener = listener
 
-    def runCommand(self, cmd_name: str):
-        """
-        Deprecated. Prefer to run command in View.
-        """
-        if cmd_name not in self.commands.keys():
-            raise ValueError(f"Trying to call an invalid command {cmd_name}. "
-                             f"Candidates are: {self.commands.keys()}")
-
-        self.commands.get(cmd_name).execute()
 
-
-class View(PropertyMixin, CommandMixin):
+class View(PropertyCommandMixin):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.prop_listener = None
         self.cmd_listener = None
 
         # None here means it should be set by App.bind()
         self.commands: Dict[str, CommandBase] = None
         self.properties: Dict[str, Any] = None
 
-    def runCommand(self, cmd_name: str):
-        if cmd_name not in self.commands.keys():
-            raise ValueError(f"Trying to call an invalid command {cmd_name}. "
-                             f"Candidates are: {self.commands.keys()}")
-
-        self.commands.get(cmd_name).execute()
-
 
 class App:
     @classmethod
     def bind(cls, model: Model, viewmodel: ViewModel, view: View,
              bind_vm_n_model=False, *, debug_set_vm_in_view=False):
         if bind_vm_n_model:
             viewmodel.bindModel(model)
```

### Comparing `vbao_MVVM-0.2.1/vbao_MVVM.egg-info/PKG-INFO` & `vbao_mvvm-0.3a1/vbao_MVVM.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: vbao_MVVM
-Version: 0.2.1
+Version: 0.3a1
 Summary: A library aiming for building an MVVM (or MVFM) project
-Author-email: Meidozuki <author@example.com>
+Author: Meidozuki
 Project-URL: Homepage, https://github.com/Meidozuki/VBAO
 Project-URL: Bug Tracker, https://github.com/Meidozuki/VBAO/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

