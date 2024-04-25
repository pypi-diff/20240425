# Comparing `tmp/morast-0.3.1.tar.gz` & `tmp/morast-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morast-0.3.1.tar", last modified: Sat Mar 16 20:03:05 2024, max compression
+gzip compressed data, was "morast-0.3.3.tar", last modified: Thu Apr 25 17:01:15 2024, max compression
```

## Comparing `morast-0.3.1.tar` & `morast-0.3.3.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-16 20:03:05.336845 morast-0.3.1/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2024-03-16 20:02:55.000000 morast-0.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4064 2024-03-16 20:03:05.335845 morast-0.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1342 2024-03-16 20:02:55.000000 morast-0.3.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1595 2024-03-16 20:02:55.000000 morast-0.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-16 20:03:05.336845 morast-0.3.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-16 20:03:05.328845 morast-0.3.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-16 20:03:05.332845 morast-0.3.1/src/morast/
--rw-rw-rw-   0 root         (0) root         (0)      546 2024-03-16 20:02:55.000000 morast-0.3.1/src/morast/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      933 2024-03-16 20:02:55.000000 morast-0.3.1/src/morast/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    12849 2024-03-16 20:02:55.000000 morast-0.3.1/src/morast/commandline.py
--rw-rw-rw-   0 root         (0) root         (0)      850 2024-03-16 20:02:55.000000 morast-0.3.1/src/morast/commons.py
--rw-rw-rw-   0 root         (0) root         (0)     7342 2024-03-16 20:02:55.000000 morast-0.3.1/src/morast/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)    39887 2024-03-16 20:02:55.000000 morast-0.3.1/src/morast/core.py
--rw-rw-rw-   0 root         (0) root         (0)    39816 2024-03-16 20:02:55.000000 morast-0.3.1/src/morast/nodes.py
--rw-rw-rw-   0 root         (0) root         (0)    14736 2024-03-16 20:02:55.000000 morast-0.3.1/src/morast/overrides.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-16 20:02:55.000000 morast-0.3.1/src/morast/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-16 20:03:05.335845 morast-0.3.1/src/morast.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4064 2024-03-16 20:03:05.000000 morast-0.3.1/src/morast.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      490 2024-03-16 20:03:05.000000 morast-0.3.1/src/morast.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-16 20:03:05.000000 morast-0.3.1/src/morast.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-03-16 20:03:05.000000 morast-0.3.1/src/morast.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-03-16 20:03:05.000000 morast-0.3.1/src/morast.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-16 20:03:05.335845 morast-0.3.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2014 2024-03-16 20:02:55.000000 morast-0.3.1/tests/test_commandline.py
--rw-rw-rw-   0 root         (0) root         (0)    12816 2024-03-16 20:02:55.000000 morast-0.3.1/tests/test_core.py
--rw-rw-rw-   0 root         (0) root         (0)     1779 2024-03-16 20:02:55.000000 morast-0.3.1/tests/test_main.py
--rw-rw-rw-   0 root         (0) root         (0)    19370 2024-03-16 20:02:55.000000 morast-0.3.1/tests/test_nodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:01:15.704330 morast-0.3.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2024-04-25 17:01:04.000000 morast-0.3.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4064 2024-04-25 17:01:15.704330 morast-0.3.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1342 2024-04-25 17:01:04.000000 morast-0.3.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1625 2024-04-25 17:01:04.000000 morast-0.3.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 17:01:15.705330 morast-0.3.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:01:15.695330 morast-0.3.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:01:15.699330 morast-0.3.3/src/morast/
+-rw-rw-rw-   0 root         (0) root         (0)      545 2024-04-25 17:01:04.000000 morast-0.3.3/src/morast/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2024-04-25 17:01:04.000000 morast-0.3.3/src/morast/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18476 2024-04-25 17:01:04.000000 morast-0.3.3/src/morast/capabilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    12771 2024-04-25 17:01:04.000000 morast-0.3.3/src/morast/commandline.py
+-rw-rw-rw-   0 root         (0) root         (0)      849 2024-04-25 17:01:04.000000 morast-0.3.3/src/morast/commons.py
+-rw-rw-rw-   0 root         (0) root         (0)     7399 2024-04-25 17:01:04.000000 morast-0.3.3/src/morast/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)    46853 2024-04-25 17:01:04.000000 morast-0.3.3/src/morast/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    40546 2024-04-25 17:01:04.000000 morast-0.3.3/src/morast/nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)    14699 2024-04-25 17:01:04.000000 morast-0.3.3/src/morast/overrides.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 17:01:04.000000 morast-0.3.3/src/morast/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:01:15.703330 morast-0.3.3/src/morast.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4064 2024-04-25 17:01:15.000000 morast-0.3.3/src/morast.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      544 2024-04-25 17:01:15.000000 morast-0.3.3/src/morast.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 17:01:15.000000 morast-0.3.3/src/morast.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-25 17:01:15.000000 morast-0.3.3/src/morast.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-25 17:01:15.000000 morast-0.3.3/src/morast.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:01:15.702330 morast-0.3.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    13096 2024-04-25 17:01:04.000000 morast-0.3.3/tests/test_capabilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2013 2024-04-25 17:01:04.000000 morast-0.3.3/tests/test_commandline.py
+-rw-rw-rw-   0 root         (0) root         (0)    14131 2024-04-25 17:01:04.000000 morast-0.3.3/tests/test_core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1778 2024-04-25 17:01:04.000000 morast-0.3.3/tests/test_main.py
+-rw-rw-rw-   0 root         (0) root         (0)    19369 2024-04-25 17:01:04.000000 morast-0.3.3/tests/test_nodes.py
```

### Comparing `morast-0.3.1/LICENSE` & `morast-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `morast-0.3.1/PKG-INFO` & `morast-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morast
-Version: 0.3.1
+Version: 0.3.3
 Summary: MOdule Reference by Analyzing the Syntax Tree
 Author-email: Rainer Schwarzbach <rainer@blackstream.de>
 License: MIT License
         
         Copyright (c) 2023 Rainer Schwarzbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `morast-0.3.1/README.md` & `morast-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `morast-0.3.1/pyproject.toml` & `morast-0.3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -42,13 +42,16 @@
 [project.urls]
 Homepage = "https://gitlab.com/blackstream-x/morast"
 Documentation = "https://blackstream-x.gitlab.io/morast"
 CI = "https://gitlab.com/blackstream-x/morast/-/pipelines"
 "Bug Tracker" = "https://gitlab.com/blackstream-x/morast/-/issues"
 Repository = "https://gitlab.com/blackstream-x/morast.git"
 
+[tool.ruff]
+line-length = 79
+
 [tool.setuptools.dynamic]
 version = {attr = "morast.__version__"}
 
 [tool.setuptools.package-data]
 "morast" = ["py.typed"]
```

### Comparing `morast-0.3.1/src/morast/__init__.py` & `morast-0.3.3/src/morast/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,12 +17,11 @@
 morast is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
-
-__version__ = "0.3.1"
+__version__ = "0.3.3"
 
 
 # vim: fileencoding=utf-8 ts=4 sts=4 sw=4 autoindent expandtab syntax=python:
```

### Comparing `morast-0.3.1/src/morast/__main__.py` & `morast-0.3.3/src/morast/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 morast is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
-
 import sys
 
 from morast import commandline
 
 
 #
 # Functions
```

### Comparing `morast-0.3.1/src/morast/commandline.py` & `morast-0.3.3/src/morast/commandline.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 morast is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
-
 import argparse
 import ast
 import fnmatch
 import logging
 import pathlib
 
 from typing import Dict, Iterator, Tuple
@@ -62,41 +61,38 @@
 class Program:
     """Command line program"""
 
     name: str = "morast"
     description: str = "Create reference documentation from sources using AST"
 
     def __init__(self, *args: str) -> None:
-        """Parse command line arguments and initialize the logger
+        r"""Parses command line arguments and initializes the logger
+
+        Initialization arguments:
 
-        :param args: a list of command line arguments
+        *   _\*args_: the command line arguments to parse, provided
+            as individual strings
         """
         logging.basicConfig(
             format="%(levelname)-8s | %(message)s",
             level=logging.WARNING,
         )
         self.config = configuration.GlobalOptions.from_file()
         self.__arguments = self._parse_args(*args)
         logging.getLogger().setLevel(self.arguments.loglevel)
 
     @property
     def arguments(self) -> argparse.Namespace:
-        """Property: command line arguments
-
-        :returns: the parsed command line arguments
-        """
+        """The parsed command line arguments"""
         return self.__arguments
 
     def _parse_args(self, *args: str) -> argparse.Namespace:
-        """Parse command line arguments using argparse
-        and return the arguments namespace.
-
-        :param args: the command line arguments
-        :returns: the parsed command line arguments as returned
-            by argparse.ArgumentParser().parse_args()
+        r"""Internal method to parse the command line arguments
+        provided through _\*args_ using argparse,
+        returning the parsed arguments namespace.
         """
         main_parser = argparse.ArgumentParser(
             prog=self.name,
             description=self.description,
         )
         main_parser.set_defaults(loglevel=logging.WARNING)
         main_parser.add_argument(
```

### Comparing `morast-0.3.1/src/morast/commons.py` & `morast-0.3.3/src/morast/commons.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 """
 
 
 #
 # Module constants
 #
 
-
 BLANK = " "
 DOT = "."
 EMPTY = ""
 LF = "\n"
 POUND = "#"
 UNDERSCORE = "_"
```

### Comparing `morast-0.3.1/src/morast/configuration.py` & `morast-0.3.3/src/morast/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 morast is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
-
 import dataclasses
 import logging
 import pathlib
 import unicodedata
 
 from typing import Any, Dict, List
 
@@ -86,14 +85,15 @@
     missing_documentation_prefix: str = unicodedata.lookup("CONSTRUCTION SIGN")
     #
     # alternative prefix for inheritance: SEEDLING
     inheritance_prefix: str = unicodedata.lookup("HATCHING CHICK")
     signature_prefix: str = unicodedata.lookup("OPEN BOOK")
     class_attributes_prefix: str = unicodedata.lookup("ROUND PUSHPIN")
     instance_attributes_prefix: str = unicodedata.lookup("PAPERCLIP")
+    property_prefix: str = unicodedata.lookup("CLIPBOARD")
     advertisement_prefix: str = unicodedata.lookup(
         "PUBLIC ADDRESS LOUDSPEAKER"
     )
 
     def get_serializable(self) -> Dict[str, Any]:
         """Return a serializable variant
         as a dict having the characters replaced by ther unicode names
@@ -193,15 +193,14 @@
                 except KeyError:
                     logging.info(
                         "Keyword %r missing in configuration file"
                         " – using hardcoded preset",
                         key,
                     )
                 else:
-
                     pre_config[key] = pathlib.Path(value)
                 #
             elif key == KW_EMOJI:
                 emoji_collect: Dict[str, Any] = {}
                 if isinstance(value, dict):
                     for subkey, subvalue in value.items():
                         if subkey == KW_ENABLED:
```

### Comparing `morast-0.3.1/src/morast/core.py` & `morast-0.3.3/src/morast/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,27 +18,27 @@
 morast is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
-
 import ast
 import collections
 import logging
 import pathlib
 import re
 
 from threading import Lock
 from typing import Any, Dict, Iterator, List, Optional, Set, Tuple, Union
 
 from smdg import elements as mde
 from smdg import strings as mds
 
+from morast import capabilities
 from morast import configuration
 from morast import commons
 from morast import nodes
 from morast import overrides
 
 
 #
@@ -106,36 +106,38 @@
 
 
 #
 # Classes
 #
 
 
-class IgnoredItem(Exception):
-    """Exception to be raised when an item is ignored.
-
-    Initialized with the error message given as _message_
-    """
+class IgnoredItemError(Exception):
+    """Exception to be raised when an item is ignored."""
 
     def __init__(self, message: str) -> None:
-        """Store the message"""
+        r"""Initialization arguments:
+
+        *   _message_: the detailed message"""
         self.message = message
 
 
-class EmojiProxy:
-    """Object providing emoji if enabled.
+class IsAPropertyError(Exception):
+    """Exception to be raised when a method has a "property" decorator"""
 
-    Initialization argument:
 
-    *   _emoji_: a configuration.[EmojiConfiguration]
-        instance
-    """
+class EmojiProxy:
+    """Object providing emoji if enabled."""
 
     def __init__(self, emoji: configuration.EmojiConfiguration) -> None:
-        """Store _emoji_ internally"""
+        r"""
+        Initialization argument:
+
+        *   _emoji_: a configuration.[EmojiConfiguration]
+            instance
+        """
         self.__emoji = emoji
         self.__cache: Dict[str, str] = {}
         self.__provide_preset(
             "todo_prefix", "missing_documentation_prefix", "TODO:"
         )
 
     def __provide_preset(
@@ -173,28 +175,26 @@
         #
 
 
 class SuperConfig:
     r"""Object holding a part of the configuration,
     existing overrides and an OrderedDict of
     extracted OverridesSection objects.
-
-    Initialization arguments:
-
-    *   _module\_overrides_: an overrides.[ModuleOverrides] instance
-    *   _options_: a configuration.[GlobalOptions] instance
     """
 
     def __init__(
         self,
         module_overrides=overrides.DUMMY_MOD_OVERRIDES,
         options=configuration.DUMMY_OPTIONS,
     ) -> None:
-        """Initialize by storing the overrides
-        and building a text module proxy
+        r"""
+        Initialization arguments:
+
+        *   _module\_overrides_: an overrides.[ModuleOverrides] instance
+        *   _options_: a configuration.[GlobalOptions] instance
         """
         self.mor = module_overrides
         self.emoji = EmojiProxy(options.emoji)
         self.advertise = options.advertise
         self._extracted_sections: collections.OrderedDict[
             Tuple[str, ...],
             Tuple[MorastDocumentableItem, overrides.OverridesSection],
@@ -253,37 +253,34 @@
 DUMMY_SUPERCONFIG = SuperConfig()
 
 
 # pylint: disable=too-many-instance-attributes
 
 
 class MorastDocumentableItem:
-    """A single documentable item (base class)
-
-    Initialization arguments:
-
-    *   _name_: the name of the item (public attribute)
-    *   _namespace_: the namespaced name of the containing
-        [MorastSection] instance
-    *   _scope_: the scope
-    *   _superconfig_: the [SuperConfig] instance passed from the
-        containing [MorastSection] instance
-    """
+    """A single documentable item (base class)"""
 
     kind = overrides.KIND_UNSPECIFIED
 
     def __init__(
         self,
         name: str,
         namespace: str = "",
         scope: str = SCOPE_MODULE,
         superconfig=DUMMY_SUPERCONFIG,
     ) -> None:
-        """Store the attributes and initialize
-        the internal collection of contained items.
+        r"""
+        Initialization arguments:
+
+        *   _name_: the name of the item (public attribute)
+        *   _namespace_: the namespaced name of the containing
+            [MorastSection] instance
+        *   _scope_: the scope
+        *   _superconfig_: the [SuperConfig] instance passed from the
+            containing [MorastSection] instance
         """
         self.name = name
         self.namespace = namespace
         if namespace:
             self.namespaced_name = f"{namespace}.{name}"
         else:
             self.namespaced_name = name
@@ -293,35 +290,35 @@
         self._original_docstring = True
         self.docstring: str = commons.EMPTY
         self.is_ignored = False
 
     def check_private(self) -> None:
         """Check if this is a private member"""
         if self.name.startswith(commons.UNDERSCORE):
-            raise IgnoredItem(
+            raise IgnoredItemError(
                 f"{self.namespace}: ignored private member {self.name!r}"
             )
         #
 
     def check_ignored(self) -> bool:
         """Check for self.is_ignored"""
         if self.is_ignored:
-            raise IgnoredItem(
+            raise IgnoredItemError(
                 f"{self.namespace}: ignored {self.name!r} as specified"
                 " through override"
             )
         #
         return False
 
     def set_docstring_from_override(self) -> None:
-        """Set the final docstring,
+        r"""Set the final docstring,
         either from the override if set there,
         or from its former value.
 
-        This method also sets the _is\\_ignored_ flag.
+        This method also sets the _is\_ignored_ flag.
         """
         override_section = self.sc.mor.setdefault(
             self.namespaced_name,
             kind=self.kind,
             namespace=self.namespace,
         )
         if override_section.is_ignored:
@@ -363,45 +360,93 @@
             yield from self.markdown_elements()
         #
 
 
 # pylint: enable=too-many-instance-attributes
 
 
-class MorastAttribute(MorastDocumentableItem):
-    r"""A (module, class, or instance) attribute
+class MorastBaseAttribute(MorastDocumentableItem):
+    """Base class for attributes and properties"""
 
-    Initialization arguments:
+    # pylint: disable=too-many-arguments
 
-    *   _element_: the ast element thi instance is built from
-    *   _namespace_: the namespaced name of the containing
-        [MorastSection] instance
-    *   _scope_: the scope (one of the allowed scopes defined
-        in the supported\_scopes class attribute)
-    *   _superconfig_: the [SuperConfig] instance passed from the
-        containing [MorastSection] instance
-    *   _check\_self_: a flag determining whether to ckeck for
-        a `self.` prefix (suitable for instance attributes only).
-        If this is `True`, the leading `self.` is stripped from the name
-    """
+    def __init__(
+        self,
+        name: str,
+        namespace: str = "",
+        scope: str = SCOPE_MODULE,
+        superconfig=DUMMY_SUPERCONFIG,
+        kind: str = overrides.KIND_INSTANCE_ATTRIBUTE,
+    ) -> None:
+        r"""
+        Initialization arguments:
+
+        *   _name_: the name of the attribute (public attribute)
+        *   _namespace_: the namespaced name of the containing
+            [MorastSection] instance
+        *   _scope_: the scope (one of the allowed scopes defined
+            in the supported\_scopes class attribute)
+        *   _superconfig_: the [SuperConfig] instance passed from the
+            containing [MorastSection] instance
+        *   _kind_: the item kind (one of KIND\_CONSTANT,
+            KIND\_CLASS\_ATTRIBUTE, KIND\_INSTANCE\_ATTRIBUTE
+            or KIND\_PROPERTY, all of which are defined
+            in the **[overrides]** module)
+        """
+        super().__init__(
+            name,
+            namespace=namespace,
+            scope=scope,
+            superconfig=superconfig,
+        )
+        logging.debug("ATTRIBUTE NAME: %s", name)
+        logging.debug("ATTRIBUTE SCOPE: %s", scope)
+        logging.debug("ATTRIBUTE KIND: %s", kind)
+        self.check_private()
+        self.kind = kind
+
+    def markdown_elements(self) -> Iterator[mde.BaseElement]:
+        """Return an iterator over MarkDown elements
+        if the item is not ignored
+        """
+        raise NotImplementedError
+
+    def as_md_list_item(self) -> mde.ListItem:
+        """Return aa a MarkDown list item"""
+        return mde.ListItem(*self.markdown_elements())
+
+
+class MorastAttribute(MorastBaseAttribute):
+    """A (module, class, or instance) attribute"""
 
     supported_scopes = (SCOPE_CLASS, SCOPE_INSTANCE, SCOPE_MODULE)
 
     # pylint: disable=too-many-arguments
 
     def __init__(
         self,
         element: Union[ast.Assign, ast.AnnAssign, ast.AugAssign],
         namespace: str = "",
         scope: str = SCOPE_MODULE,
         superconfig=DUMMY_SUPERCONFIG,
         check_self: bool = False,
     ) -> None:
-        """Store the attributes and initialize
-        the internal collection of contained items.
+        r"""
+        Initialization arguments:
+
+        *   _element_: the ast element this instance is built from
+        *   _namespace_: the namespaced name of the containing
+            [MorastSection] instance
+        *   _scope_: the scope (one of the allowed scopes defined
+            in the supported\_scopes class attribute)
+        *   _superconfig_: the [SuperConfig] instance passed from the
+            containing [MorastSection] instance
+        *   _check\_self_: a flag determining whether to ckeck for
+            a `self.` prefix (suitable for instance attributes only).
+            If this is `True`, the leading `self.` is stripped from the name
         """
         if scope not in self.supported_scopes:
             raise ValueError(f"scope must be one of {self.supported_scopes!r}")
         #
         prefix_by_scope: Dict[str, str] = {
             SCOPE_CLASS: f"{superconfig.emoji.class_attributes_prefix}"
             f" {namespace}",
@@ -418,69 +463,115 @@
         if scope == SCOPE_INSTANCE:
             kind = overrides.KIND_INSTANCE_ATTRIBUTE
             if check_self:
                 if name.startswith("self."):
                     assignment.strip_first()
                     name = str(assignment.target)
                 else:
-                    raise IgnoredItem(f"{name}: no instance attribute")
+                    raise IgnoredItemError(f"{name}: no instance attribute")
                 #
             #
         elif scope == SCOPE_CLASS:
             kind = overrides.KIND_CLASS_ATTRIBUTE
         #
         if commons.DOT in name:
-            raise IgnoredItem(f"{name}: ignored namespaced assignment")
+            raise IgnoredItemError(f"{name}: ignored namespaced assignment")
         #
         super().__init__(
             name,
             namespace=namespace,
             scope=scope,
             superconfig=superconfig,
+            kind=kind,
         )
-        logging.debug("ATTRIBUTE NAME: %s", name)
-        logging.debug("ATTRIBUTE SCOPE: %s", scope)
-        logging.debug("ATTRIBUTE KIND: %s", kind)
-        self.check_private()
-        self.kind = kind
         self.set_docstring_from_override()
         self.check_ignored()
         self.assignment = assignment
         if self.sc.mor[self.namespaced_name].value_is_stripped:
             self.assignment.operator = None
         #
 
     def markdown_elements(self) -> Iterator[mde.BaseElement]:
         """Return an iterator over MarkDown elements
         if the item is not ignored
         """
         yield mde.Paragraph(self.assignment.as_markdown())
         yield nodes.DocString(self.docstring).as_markdown()
 
-    def as_md_list_item(self) -> mde.ListItem:
-        """Return aa a MarkDown list item"""
-        return mde.ListItem(*self.markdown_elements())
+
+class MorastProperty(MorastBaseAttribute):
+    """An instance property"""
+
+    # pylint: disable=too-many-arguments
+
+    def __init__(
+        self,
+        element: ast.FunctionDef,
+        namespace: str = "",
+        superconfig=DUMMY_SUPERCONFIG,
+    ) -> None:
+        r"""
+        Initialization arguments:
+
+        *   _element_: the ast.FunctionDef instance of the property
+        *   _namespace_: the namespaced name of the containing
+            [MorastSection] instance
+        *   _superconfig_: the [SuperConfig] instance passed from the
+            containing [MorastSection] instance
+        *   _docstring_: the docstring from the property method
+        *   _type\_annotation_: the type annotation
+        """
+        super().__init__(
+            element.name,
+            namespace=namespace,
+            scope=SCOPE_INSTANCE,
+            superconfig=superconfig,
+            kind=overrides.KIND_PROPERTY,
+        )
+        self.type_annotation: str = commons.EMPTY
+        if isinstance(element.returns, (ast.AST, str)):
+            self.type_annotation = str(nodes.get_node(element.returns))
+        #
+        # docstring: str = commons.EMPTY
+        for sub_element in element.body:
+            if isinstance(sub_element, ast.Expr):
+                if isinstance(sub_element.value, ast.Constant):
+                    self.docstring = nodes.remove_hanging_indent(
+                        sub_element.value.value.strip(),
+                        level=2,
+                    )
+                    break
+                #
+            #
+        #
+        self.set_docstring_from_override()
+        self.check_ignored()
+
+    def markdown_elements(self) -> Iterator[mde.BaseElement]:
+        """Return an iterator over MarkDown elements
+        if the item is not ignored
+        """
+        signature_elements: List[mde.BaseElement] = [
+            mde.ItalicText("readonly property"),
+            mde.InlineElement(f" {self.sc.emoji.property_prefix} "),
+            mde.BoldText(f".{self.name}"),
+        ]
+        if self.type_annotation:
+            signature_elements.append(
+                mde.InlineElement(f": {self.type_annotation}")
+            )
+        #
+        yield mde.Paragraph(mde.CompoundInlineElement(*signature_elements))
+        yield nodes.DocString(self.docstring, level=0).as_markdown()
 
 
 class MorastSection(MorastDocumentableItem):
     """Documentation section with a headline and other nodes.
     May also contain other sections.
 
-    Initialization arguments:
-
-    *   _name_: the name of the section (public attribute)
-    *   _namespace_: the namespaced name of the containing
-        [MorastSection] instance
-    *   _scope_: the scope
-    *   _superconfig_: the [SuperConfig] instance passed from the
-        containing [MorastSection] instance
-    *   _level_: section level in the document hierarchy
-    *   _headline_: deviant headline if provided
-        (else, the headline will just be _name_)
-
     Keeps an internal collection of contained
     MorastBaseNode and [MorastSection] instances.
     """
 
     # pylint: disable=too-many-arguments
 
     def __init__(
@@ -488,16 +579,26 @@
         name: str,
         namespace: str = "",
         scope=SCOPE_MODULE,
         superconfig=DUMMY_SUPERCONFIG,
         level: int = 1,
         headline: Optional[str] = None,
     ) -> None:
-        """Store the attributes and initialize
-        the internal collection of contained items.
+        r"""
+        Initialization arguments:
+
+        *   _name_: the name of the section (public attribute)
+        *   _namespace_: the namespaced name of the containing
+            [MorastSection] instance
+        *   _scope_: the scope
+        *   _superconfig_: the [SuperConfig] instance passed from the
+            containing [MorastSection] instance
+        *   _level_: section level in the document hierarchy
+        *   _headline_: deviant headline if provided
+            (else, the headline will just be _name_)
         """
         super().__init__(
             name, namespace=namespace, scope=scope, superconfig=superconfig
         )
         if isinstance(headline, str):
             self._headline = headline
         else:
@@ -512,14 +613,21 @@
     def __getitem__(
         self,
         name: str,
     ) -> Union[nodes.MorastBaseNode, MorastDocumentableItem]:
         """Directly return the item stored as _name_"""
         return self._contents[name]
 
+    def __delitem__(
+        self,
+        name: str,
+    ) -> None:
+        """Delete the item stored as _name_"""
+        del self._contents[name]
+
     def __len__(self) -> int:
         """Total number of contained nodes and subsections"""
         return len(self._contents)
 
     def items(
         self,
     ) -> Iterator[
@@ -540,16 +648,15 @@
             #
         #
 
     def adjust_level(self, new_level: int) -> None:
         r"""Change the level to _new\_level_,
         recurse into all subsections and
         propagate the change.
-        If a docstring is present,
-        adjust its level as well.
+        If a docstring is present, adjust its level as well.
         """
         self._level = new_level
         for _, child_section in self.subsections():
             child_section.adjust_level(new_level + 1)
         #
         try:
             docstring = self[_MORAST_DOCSTRING]
@@ -625,61 +732,100 @@
                 yield from sub_element.markdown_elements()
             else:
                 yield sub_element.as_markdown()
             #
         #
 
 
-class MorastAttributesList(MorastSection):
-    r"""Attributes List,
-    container for several [MorastAttribute] instances
+class ImplementedCapabilities(MorastSection):
+    """Implemente capabilities section"""
+
+    supported_scopes = (SCOPE_CLASS, SCOPE_MODULE)
+
+    def __init__(
+        self,
+        implemented_capabilities: capabilities.Collector,
+    ) -> None:
+        r"""
+        Initialization argument:
+
+        *   _implemented\_capabilities_: a capabilities.Collector instance
+        """
+        super().__init__(
+            "implemented_capabilities",
+            namespace="",
+            scope=SCOPE_CLASS,
+            superconfig=DUMMY_SUPERCONFIG,
+            level=4,
+            headline="Implemented capabilities",
+        )
+        self._implemented_capabilities = implemented_capabilities
+
+    def markdown_elements(self) -> Iterator[mde.BaseElement]:
+        """Yield markdown elements"""
+        yield mde.Header(self._level, self._headline)
+        md_list_items: List[mde.ListItem] = []
+        for (
+            implemented_md_item
+        ) in self._implemented_capabilities.as_markdown():
+            md_list_items.append(implemented_md_item)
+        #
+        yield mde.UnorderedList(*md_list_items)
 
-    Initialization arguments:
 
-    *   _name_: the name of the attributes list
-    *   _scope_: the scope (one of the allowed scopes defined
-        in the supported\_scopes class attribute)
-    *   _superconfig_: the [SuperConfig] instance passed from the
-        containing [MorastModule] or [MorastClassDef] instance
-    *   _headline_: the headline if different from the name
+class MorastAttributesList(MorastSection):
+    """Attributes List,
+    container for several [MorastBaseAttribute] instances
     """
 
     supported_scopes = (SCOPE_CLASS, SCOPE_MODULE)
 
     def __init__(
         self,
         name: str,
         scope: str = SCOPE_MODULE,
         superconfig=DUMMY_SUPERCONFIG,
         headline: Optional[str] = None,
     ) -> None:
-        """Store the attributes and initialize
-        the internal collection of contained items.
+        r"""
+        Initialization arguments:
+
+        *   _name_: the name of the attributes list
+        *   _scope_: the scope (one of the allowed scopes defined
+            in the supported\_scopes class attribute)
+        *   _superconfig_: the [SuperConfig] instance passed from the
+            containing [MorastModule] or [MorastClassDef] instance
+        *   _headline_: the headline if different from the name
         """
+
         level = 2 if scope == SCOPE_MODULE else 4
         super().__init__(
             name,
             namespace="",
             scope=scope,
             superconfig=superconfig,
             level=level,
             headline=headline,
         )
-        self._attributes: collections.OrderedDict[str, MorastAttribute] = (
+        self._attributes: collections.OrderedDict[str, MorastBaseAttribute] = (
             collections.OrderedDict()
         )
 
-    def add(self, mor_attr: MorastAttribute) -> None:
+    def add(self, mor_attr: MorastBaseAttribute) -> None:
         """Store _mor_attr_ under its name"""
         self._attributes[mor_attr.name] = mor_attr
 
-    def remove(self, attr_name) -> None:
+    def remove(self, attr_name: str) -> None:
         """Remove the attribute named _attr_name_ if it exists"""
         self._attributes.pop(attr_name, None)
 
+    def __getitem__(self, attr_name: str) -> MorastBaseAttribute:
+        """Attribute access via name"""
+        return self._attributes[attr_name]
+
     def __len__(self) -> int:
         """Total number of contained nodes and subsections"""
         return len(self._attributes)
 
     def markdown_elements(self) -> Iterator[mde.BaseElement]:
         """Yield markdown elements"""
         yield mde.Header(self._level, self._headline)
@@ -687,49 +833,52 @@
         for mor_attr in self._attributes.values():
             md_list_items.append(mor_attr.as_md_list_item())
         #
         yield mde.UnorderedList(*md_list_items)
 
 
 class MorastFunctionDef(MorastSection):
-    r"""Represents a module-level function,
+    """Represents a module-level function,
     or a class, static, or instance method.
-
-    Initialization arguments:
-
-    *   _element_: the ast.FunctionDef instance from which
-        the function name, signature and docstring are determined
-    *   _namespace_: the namespaced name of the class
-        if the function is a method
-    *   _scope_: the scope (one of the allowed scopes defined
-        in the supported\_scopes class attribute)
-    *   _superconfig_: the [SuperConfig] instance passed from the
-        containing [MorastModule] or [MorastClassDef] instance
     """
 
     supported_scopes = (SCOPE_CLASS, SCOPE_INSTANCE, SCOPE_MODULE)
 
     # pylint: disable=too-many-branches
 
     def __init__(
         self,
         element: ast.FunctionDef,
         namespace: str = "",
         scope: str = SCOPE_MODULE,
         superconfig=DUMMY_SUPERCONFIG,
     ) -> None:
-        """Determine and store attributes"""
+        r"""
+        Initialization arguments:
+
+        *   _element_: the ast.FunctionDef instance from which
+            the function name, signature and docstring are determined
+        *   _namespace_: the namespaced name of the class
+            if the function is a method
+        *   _scope_: the scope (one of the allowed scopes defined
+            in the supported\_scopes class attribute)
+        *   _superconfig_: the [SuperConfig] instance passed from the
+            containing [MorastModule] or [MorastClassDef] instance
+        """
         parent_name = namespace.split(commons.DOT)[-1]
         self.function_type = MODULE_LEVEL_FUNCTION
         level = 3
         if scope != SCOPE_MODULE:
             level = 4
             self.function_type = INSTANCE_METHOD
             for dec in element.decorator_list:
                 if isinstance(dec, ast.Name):
+                    if dec.id == "property":
+                        raise IsAPropertyError
+                    #
                     try:
                         self.function_type = TYPES_BY_DECORATOR[dec.id]
                     except KeyError:
                         continue
                     #
                     break
                 #
@@ -797,40 +946,40 @@
         self.check_ignored()
         self.add_subnode(
             _MORAST_DOCSTRING,
             nodes.DocString(self.docstring, level=ds_level),
         )
 
 
+# pylint: disable=too-many-instance-attributes
 class MorastClassDef(MorastSection):
-    """Represents a class.
-
-    Initialization arguments:
-
-    * _element_: the ast.ClassDef instance from which
-      the class name, signature, docstring, attributes
-      and methods are determined
-    * ...
-    * _namespace_: the namespace of the class
-    * _superconfig_: the [SuperConfig] instance passed from the
-      containing [MorastModule] instance
-    """
+    """Represents a class."""
 
     kind = overrides.KIND_CLASS
 
     # pylint: disable=too-many-branches
     # pylint: disable=too-many-locals
+    # pylint: disable=too-many-statements
 
     def __init__(
         self,
         element: ast.ClassDef,
         namespace: str = "",
         superconfig=DUMMY_SUPERCONFIG,
     ) -> None:
-        """Determine and store attributes"""
+        r"""
+        Initialization arguments:
+
+        * _element_: the ast.ClassDef instance from which
+          the class name, signature, docstring, attributes
+          and methods are determined
+        * _namespace_: the namespace of the class
+        * _superconfig_: the [SuperConfig] instance passed from the
+          containing [MorastModule] instance
+        """
         name = element.name
         decorators: List[nodes.MorastBaseNode] = [
             nodes.get_node(single_dec) for single_dec in element.decorator_list
         ]
         class_prefix = "Class"
         self.is_a_dataclass = False
         for item in decorators:
@@ -850,14 +999,17 @@
             superconfig=superconfig,
             level=3,
             headline=f"{class_prefix} {name}()",
         )
         self.check_private()
         inheritance_prefix = self.sc.emoji.inheritance_prefix
         self._init_method: Optional[ast.FunctionDef] = None
+        self._implemented_specials = capabilities.Collector(
+            f"{camel_to_snake_case(self.name)}_instance"
+        )
         self.existing_attributes: Dict[str, Set[str]] = {
             SCOPE_CLASS: set(),
             SCOPE_INSTANCE: set(),
         }
         self.attribute_lists: Dict[str, MorastAttributesList] = {}
         self.methods: Dict[str, MorastSection] = {}
         for scope in (SCOPE_CLASS, SCOPE_INSTANCE):
@@ -866,20 +1018,22 @@
                 superconfig=superconfig,
                 scope=scope,
             )
             self.methods[scope] = MorastSection(
                 f"{scope} methods", superconfig=superconfig, level=self._level
             )
         #
-        ds_level = 1
+        self._init_docstring: str = commons.EMPTY
         for sub_element in element.body:
             if isinstance(sub_element, ast.Expr):
                 if isinstance(sub_element.value, ast.Constant):
-                    self.docstring = sub_element.value.value
-                    ds_level = self._level
+                    self.docstring = nodes.remove_hanging_indent(
+                        sub_element.value.value.strip(),
+                        level=1,
+                    )
                     continue
                 #
             elif isinstance(sub_element, (ast.Assign, ast.AnnAssign)):
                 if self.is_a_dataclass:
                     self._add_instance_attribute(sub_element, check_self=False)
                     continue
                 self._add_class_attribute(sub_element)
@@ -896,20 +1050,32 @@
                     *bases, prefix=f"{inheritance_prefix} "
                 ),
             )
         #
         if isinstance(self._init_method, ast.FunctionDef):
             self._add_signature(self._init_method)
         #
+        if self.docstring:
+            if self._init_docstring:
+                self.docstring = f"{self.docstring}\n\n{self._init_docstring}"
+            #
+        else:
+            self.docstring = self._init_docstring
+        #
         self.set_docstring_from_override()
         self.check_ignored()
         self.add_subnode(
             _MORAST_DOCSTRING,
-            nodes.DocString(self.docstring, level=ds_level),
+            nodes.DocString(self.docstring, level=0),
         )
+        if self._implemented_specials:
+            self.add_subsection(
+                subsection=ImplementedCapabilities(self._implemented_specials)
+            )
+        #
         for scope in (SCOPE_CLASS, SCOPE_INSTANCE):
             if len(self.attribute_lists[scope]):
                 self.add_subsection(subsection=self.attribute_lists[scope])
             #
         #
         for scope in (SCOPE_CLASS, SCOPE_INSTANCE):
             for method_name, method_sect in self.methods[scope].subsections():
@@ -919,30 +1085,61 @@
 
     def _add_method(self, element: ast.FunctionDef) -> None:
         """Add method"""
         method_name = str(element.name)
         if method_name == "__init__":
             self._init_method = element
             for init_statement in self._init_method.body:
+                if not self._init_docstring and isinstance(
+                    init_statement, ast.Expr
+                ):
+                    if isinstance(init_statement.value, ast.Constant):
+                        self._init_docstring = nodes.remove_hanging_indent(
+                            init_statement.value.value.strip(),
+                            level=2,
+                        )
+                        continue
+                    #
+                #
                 if isinstance(init_statement, (ast.Assign, ast.AnnAssign)):
                     self._add_instance_attribute(init_statement)
                 #
             #
             return
         #
         try:
+            self._implemented_specials.add_method(element)
+        except (
+            capabilities.NoSpecialMethodError,
+            capabilities.UnsupportedMethodError,
+        ):
+            pass
+        else:
+            return
+        #
+        try:
             method = MorastFunctionDef(
                 element,
                 namespace=self.namespaced_name,
                 superconfig=self.sc,
                 scope=SCOPE_CLASS,
             )
-        except IgnoredItem as ignored:
+        except IgnoredItemError as ignored:
             logging.info(ignored.message)
             return
+        except IsAPropertyError:
+            # self._add_property(element)
+            self.attribute_lists[SCOPE_INSTANCE].add(
+                MorastProperty(
+                    element,
+                    namespace=self.namespaced_name,
+                    superconfig=self.sc,
+                )
+            )
+            return
         #
         self.methods[METHOD_TARGETS[method.function_type]].add_subsection(
             subsection=method
         )
 
     def _add_attribute(
         self,
@@ -958,15 +1155,15 @@
             new_attribute = MorastAttribute(
                 element,
                 namespace=self.namespaced_name,
                 superconfig=self.sc,
                 scope=scope,
                 check_self=check_self,
             )
-        except IgnoredItem as ignored:
+        except IgnoredItemError as ignored:
             logging.info(ignored.message)
             return
         #
         if new_attribute.name in self.existing_attributes[scope]:
             return
         #
         self.attribute_lists[scope].add(new_attribute)
@@ -1018,40 +1215,41 @@
             ),
         )
 
 
 class MorastModule(MorastSection):
     """Represents a module in the document tree
 
-    Initialization arguments:
+    Internally stroes a sequence of MorastSection instances
+    in the following order:
 
-    *   _module_: an ast.Module instance from which this instance is built
-    *   _name_: the module name (public attribute, set in the ancestor class)
-    *   _namespace_: the (external) module namespace,
-         only used in the headline
-    *   _superconfig_: a [SuperConfig] instance that is also passed through
-        to to all contained [MorastDocumentableItem] subclass instances
+    1.  module contents
+    2.  module-level functions
+    3.  classes
     """
 
     kind = overrides.KIND_MODULE
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         module: ast.Module,
         name: str,
         namespace: str = "",
         superconfig=DUMMY_SUPERCONFIG,
     ) -> None:
-        """Store the attributes and build a sequence of
-        MorastSection instances:
+        r"""
+        Initialization arguments:
 
-        *   module contents
-        *   module-level functions
-        *   classes
+        *   _module_: an ast.Module instance from which this instance is built
+        *   _name_: the module name (public attribute)
+        *   _namespace_: the (external) module namespace,
+             only used in the headline
+        *   _superconfig_: a [SuperConfig] instance that is also passed through
+            to to all contained [MorastDocumentableItem] subclass instances
         """
         namespace_prefix = f"{namespace}." if namespace else ""
         headline_prefix = superconfig.emoji.module_prefix or "Module"
         super().__init__(
             name,
             superconfig=superconfig,
             headline=f"{headline_prefix} {namespace_prefix}{name}",
@@ -1109,40 +1307,40 @@
             try:
                 module_constant = MorastAttribute(
                     element,
                     namespace=self.name,
                     scope=SCOPE_MODULE,
                     superconfig=self.sc,
                 )
-            except IgnoredItem as ignored:
+            except IgnoredItemError as ignored:
                 logging.info(ignored.message)
                 return
             #
             self.module_contents.add(module_constant)
         elif isinstance(element, ast.ClassDef):
             try:
                 class_sub = MorastClassDef(
                     element,
                     namespace=self.name,
                     superconfig=self.sc,
                 )
-            except IgnoredItem as ignored:
+            except IgnoredItemError as ignored:
                 logging.info(ignored.message)
                 return
             #
             self.classes.add_subsection(subsection=class_sub)
         elif isinstance(element, ast.FunctionDef):
             try:
                 func_sub = MorastFunctionDef(
                     element,
                     namespace=self.name,
                     scope=SCOPE_MODULE,
                     superconfig=self.sc,
                 )
-            except IgnoredItem as ignored:
+            except IgnoredItemError as ignored:
                 logging.info(ignored.message)
                 return
             #
             self.functions.add_subsection(subsection=func_sub)
         else:
             raise TypeError(
                 f"{ast.dump(element)} (line {element.lineno})"
```

### Comparing `morast-0.3.1/src/morast/nodes.py` & `morast-0.3.3/src/morast/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 morast is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
-
 import ast
 import datetime
 import logging
 import re
 
 from typing import Any, Dict, List, Optional, Type, Union
 
@@ -278,15 +277,15 @@
     """
     if level < 1:
         return text
     #
     prx_hanging_indent = re.compile(f"^(    |\\t){{{level}}}")
     fixed_lines: List[str] = []
     for index, line in enumerate(text.splitlines(keepends=True)):
-        if index is None:
+        if not index:
             fixed_lines.append(line)
             continue
         #
         fixed_lines.append(prx_hanging_indent.sub(commons.EMPTY, line))
     #
     return commons.EMPTY.join(fixed_lines)
 
@@ -1079,38 +1078,54 @@
 
     def __init__(
         self,
         expression: Union[ast.Expr, str],
         level: int = 1,
         sanitize: bool = False,
     ) -> None:
-        """Store the content"""
+        """Initialization arguments:
+
+        *   _expression_: source ast.Expr or string
+        *   _level_: the docstring level, one of:
+            *   `0`: preformatted docstring,
+                no hanging index correction necessary, immutable level
+            *   `1`: usually module-level docstring,
+                no hanging index correction necessary,
+                but level is changeable
+            *   `3`: module-level function or class docstring,
+                hanging index correction by one level
+            *   `4`: class or instance method,
+                hanging index correction by two levels
+        *   _sanitize_: Flag determining if sanitization is required
+        """
         if isinstance(expression, str):
             content = expression
         elif isinstance(expression.value, ast.Constant):
             content = expression.value.value
         else:
             raise ValueError("Must be a constant expression!")
         #
-        if level < 1:
-            raise ValueError("level must be 1 or greater")
+        if level < 0:
+            raise ValueError("level must be 0 or greater")
         #
         self._level = level
         if sanitize:
             self._sane_content = mds.sanitize(content)
         else:
             self._sane_content = mds.declare_as_safe(content)
         #
 
     def adjust_level(self, new_level: int) -> None:
-        """Change the level to _new\\_level_"""
+        r"""Change the level to _new\_level_ if it may be changed"""
         if new_level < 1:
             raise ValueError("level must be 1 or greater")
         #
-        self._level = new_level
+        if self._level > 0:
+            self._level = new_level
+        #
 
     def as_markdown(self) -> mde.BaseElement:
         """Return a MarkDown representation"""
         content = remove_hanging_indent(
             str(self._sane_content), self._level - 2
         )
         return mde.BlockQuote(mds.declare_as_safe(content))
```

### Comparing `morast-0.3.1/src/morast/overrides.py` & `morast-0.3.3/src/morast/overrides.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 morast is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
-
 import collections
 import logging
 import pathlib
 import re
 
 from typing import Iterator, List, Optional, Tuple
 
@@ -36,17 +35,17 @@
 #
 # Module constants
 #
 
 
 __all__ = ["OverridesSection", "ModuleOverrides"]
 
-_KW_ADDITIONS = "additions"
-_KW_IGNORE = "ignore"
-_KW_STRIP_VALUE = "strip-value"
+ADDITIONS = "additions"
+IGNORE = "ignore"
+STRIP_VALUE = "strip-value"
 
 KIND_CLASS_ATTRIBUTE = "class attribute"
 KIND_CLASS_METHOD = "class method"
 KIND_CLASS = "class"
 KIND_CONSTANT = "module-level constant"
 KIND_FUNCTION = "module-level function"
 KIND_INSTANCE_ATTRIBUTE = "instance attribute"
@@ -119,22 +118,22 @@
         name_parts = self.name.split(commons.DOT)
         level = len(name_parts)
         headline = f"{commons.POUND * level} {name_parts[-1]} {self.kind}"
         if self.kind in CLASS_CONTEXT_KINDS:
             headline = f"{headline} of {self.namespace}"
         #
         if self.__is_ignored:
-            headline = f"{headline} | {_KW_IGNORE}"
+            headline = f"{headline} | {IGNORE}"
         #
         if self.__value_is_stripped:
-            headline = f"{headline} | {_KW_STRIP_VALUE}"
+            headline = f"{headline} | {STRIP_VALUE}"
         #
         contents = self.docstring
         if self.__additions:
-            headline = f"{headline} | {_KW_ADDITIONS}"
+            headline = f"{headline} | {ADDITIONS}"
             contents = self.additions
         #
         return commons.LF.join((headline, commons.EMPTY, contents))
 
     def __bool__(self) -> bool:
         """Return `True` if this section has any contents,
         or is ignored, or its value is stripped
@@ -392,19 +391,19 @@
                     #
                 #
                 current_section = mod_overrides.setdefault(
                     namespaced_name,
                     kind=kind,
                     namespace=namespace,
                 )
-                write_to_additions = _KW_ADDITIONS in remaining_headline
-                if _KW_IGNORE in remaining_headline:
+                write_to_additions = ADDITIONS in remaining_headline
+                if IGNORE in remaining_headline:
                     current_section.ignore()
                 #
-                if _KW_STRIP_VALUE in remaining_headline:
+                if STRIP_VALUE in remaining_headline:
                     current_section.strip_value()
                 #
                 continue
             #
             if not internal_namespace:
                 continue
             #
```

### Comparing `morast-0.3.1/src/morast.egg-info/PKG-INFO` & `morast-0.3.3/src/morast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morast
-Version: 0.3.1
+Version: 0.3.3
 Summary: MOdule Reference by Analyzing the Syntax Tree
 Author-email: Rainer Schwarzbach <rainer@blackstream.de>
 License: MIT License
         
         Copyright (c) 2023 Rainer Schwarzbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `morast-0.3.1/tests/test_commandline.py` & `morast-0.3.3/tests/test_commandline.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 morast is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
-
 import io
 import sys
 
 from unittest import TestCase
 
 from unittest.mock import patch
```

### Comparing `morast-0.3.1/tests/test_core.py` & `morast-0.3.3/tests/test_core.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,28 +17,25 @@
 morast is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
-
 import ast
 
-from typing import Iterator
 from unittest import TestCase
 
 from smdg import elements as mde
 from smdg import strings as mds
 
 from morast import core
 from morast import overrides
 
-
-# from morast import nodes
+from . import commons as tcom
 
 
 EXPECTED_MBN_REPR = "<MorastBaseNode instance>"
 
 PAPERCLIP_EMOJI = "\N{PAPERCLIP}"
 CONSTRUCTION_SIGN_EMOJI = "\N{CONSTRUCTION SIGN}"
 
@@ -75,41 +72,49 @@
     )
 )
 
 EXAMPLE_ASSIGNMENT_1 = f"{C1}: str = 'abcd'"
 EXAMPLE_ASSIGNMENT_3 = f"{C3}: List[str] = [{EXAMPLE_MOD_NAME}.{C2}]"
 
 
-SIMPLE_DATACLASS = '''
+SDC_NAME = "DataStorage"
+SIMPLE_DATACLASS = f'''
 @dataclasses.dataclass
-class DataStorage:
+class {SDC_NAME}:
     """class docstring"""
 
     number: int
     flag: bool = False
     identifier: str = "dummy"
 '''
 
-FROZEN_DATACLASS = '''
+FDC_NAME = "EmojiConfiguration"
+FROZEN_DATACLASS = f'''
 @dataclasses.dataclass(frozen=True)
-class EmojiConfiguration:
+class {FDC_NAME}:
     """Configuration of emoji for …"""
 
     enabled: bool = True
 '''
 
+PROP_NAME = "readonly_prop"
+PROPERTY = f'''
+@property
+def {PROP_NAME}(self) -> str:
+    """Readonly string property"""
+    return self.__hidden_attr
+'''
+
 
-def parsed_body(source: str) -> Iterator[ast.AST]:
-    """Return the body od a parsed module"""
-    parsed_module = ast.parse(source)
-    for item in parsed_module.body:
-        if isinstance(item, ast.AST):
-            yield item
-        #
-    #
+def safe_missing_docstring(class_name: str, attr_name: str) -> mds.SafeString:
+    """Return an expected  placeholder docstring for an attribute"""
+    return mds.declare_as_safe(
+        f"{CONSTRUCTION_SIGN_EMOJI}"
+        f" **{class_name}.{attr_name}** documentation _to be added_"
+    )
 
 
 class Functions(TestCase):
     """Module-level functions"""
 
 
 class MorastDocumentableItem(TestCase):
@@ -138,15 +143,15 @@
             item.set_docstring_from_override()
             with self.subTest(name, ignored=ignored):
                 self.assertEqual(item.is_ignored, ignored)
             #
             with self.subTest(f"{name} raises exception"):
                 if ignored:
                     self.assertRaisesRegex(
-                        core.IgnoredItem,
+                        core.IgnoredItemError,
                         f"\\A{EXAMPLE_MOD_NAME}: ignored {name!r} as specified"
                         " through override",
                         item.check_ignored,
                     )
                 else:
                     self.assertFalse(item.check_ignored())
                 #
@@ -157,15 +162,15 @@
         """.check_private() method"""
         item = core.MorastDocumentableItem(
             C4,
             namespace=EXAMPLE_MOD_NAME,
             superconfig=EXAMPLE_SUPERCONFIG,
         )
         self.assertRaisesRegex(
-            core.IgnoredItem,
+            core.IgnoredItemError,
             f"\\A{EXAMPLE_MOD_NAME}: ignored private member {C4!r}",
             item.check_private,
         )
 
     def test_markdown_elements(self) -> None:
         """.markdown_elements() method"""
         item = core.MorastDocumentableItem(
@@ -186,29 +191,29 @@
 class MorastAttribute(TestCase):
     """MorastAttribute class"""
 
     maxDiff = None
 
     def test_simple_docstring(self) -> None:
         """initialization and docstring of a simple item"""
-        element = list(parsed_body(EXAMPLE_ASSIGNMENT_1))[0]
+        element = tcom.first_parsed_body_element(EXAMPLE_ASSIGNMENT_1)
         if not isinstance(element, (ast.AnnAssign, ast.AugAssign, ast.Assign)):
             self.skipTest("wrong type")
             return
         #
         item = core.MorastAttribute(
             element,
             namespace=EXAMPLE_MOD_NAME,
             superconfig=EXAMPLE_SUPERCONFIG,
         )
         self.assertEqual(item.docstring, C1_DOC)
 
     def test_stripped_value_as_markdown(self) -> None:
         """docstring of a simple item"""
-        element = list(parsed_body(EXAMPLE_ASSIGNMENT_3))[0]
+        element = tcom.first_parsed_body_element(EXAMPLE_ASSIGNMENT_3)
         if not isinstance(element, (ast.AnnAssign, ast.AugAssign, ast.Assign)):
             self.skipTest("wrong type")
             return
         #
         item = core.MorastAttribute(
             element,
             namespace=EXAMPLE_MOD_NAME,
@@ -234,152 +239,184 @@
                     ),
                 ),
                 mde.BlockQuote(mds.SafeString(C3_DOC)),
             ],
         )
 
 
+class MorastProperty(TestCase):
+    """MorastProperty class"""
+
+    maxDiff = None
+
+    def test_attributes(self) -> None:
+        """attributes of the element"""
+        element = tcom.first_parsed_body_element(PROPERTY)
+        if not isinstance(element, ast.FunctionDef):
+            self.skipTest("wrong type")
+            return
+        #
+        item = core.MorastProperty(
+            element,
+            namespace="DummyClass",
+            superconfig=EXAMPLE_SUPERCONFIG,
+        )
+        for attr_name, expexted_value in (
+            ("name", PROP_NAME),
+            ("docstring", "Readonly string property"),
+            ("type_annotation", "str"),
+        ):
+            with self.subTest(
+                attr_name=attr_name, expexted_value=expexted_value
+            ):
+                self.assertEqual(getattr(item, attr_name), expexted_value)
+            #
+        #
+
+
 class MorastClassDef(TestCase):
     """MorastClassDef class"""
 
     maxDiff = None
 
-    def rest_simple_dataclass(self) -> None:
+    def test_simple_dataclass(self) -> None:
         """test initialization of a simple data class"""
-        ast_class_def = list(parsed_body(SIMPLE_DATACLASS))[0]
+        ast_class_def = tcom.first_parsed_body_element(SIMPLE_DATACLASS)
         if isinstance(ast_class_def, ast.ClassDef):
             class_def = core.MorastClassDef(ast_class_def)
         else:
             raise ValueError("Excpected a class definition")
         #
         with self.subTest("name"):
-            self.assertEqual(class_def.name, "DataStorage")
+            self.assertEqual(class_def.name, SDC_NAME)
         #
         with self.subTest("is a dataclass"):
             self.assertTrue(class_def.is_a_dataclass)
         #
-        # =============================================================================
-        #         for item in ("number", "flag", "identifier"):
-        #             with self.subTest("instance_attribute", item=item):
-        #                 current_node = class_def.instance_attrs[item]
-        #                 if isinstance(current_node, nodes.Assignment):
-        #                     self.assertEqual(
-        #                         str(nodes.MorastName(item)),
-        #                         str(current_node.target),
-        #                     )
-        #                 else:
-        #                     raise ValueError("expected an Assignment")
-        #                 #
-        #             #
-        # =============================================================================
+        for item in ("number", "flag", "identifier"):
+            with self.subTest("instance_attribute", item=item):
+                current_attr = class_def.attribute_lists[core.SCOPE_INSTANCE][
+                    item
+                ]
+                if isinstance(current_attr, core.MorastAttribute):
+                    self.assertEqual(current_attr.name, item)
+                    self.assertEqual(current_attr.scope, core.SCOPE_INSTANCE)
+                else:
+                    raise ValueError("expected an Attribute")
+                #
+            #
         #
         with self.subTest("MarkDown elements"):
             self.assertEqual(
                 list(class_def.markdown_elements()),
                 [
                     mde.HorizontalRule(20),
                     mde.Header(3, "Dataclass DataStorage()"),
                     mde.BlockQuote(mds.sanitize("class docstring")),
-                    mde.HorizontalRule(20),
+                    # mde.HorizontalRule(20),
                     mde.Header(4, "instance attributes"),
-                    mde.CompoundInlineElement(
-                        mde.InlineElement(f"{PAPERCLIP_EMOJI} ."),
-                        mde.BoldText(mde.InlineElement("number")),
-                        mde.InlineElement(": "),
-                        mde.InlineElement("int"),
-                    ),
-                    mde.BlockQuote(
-                        mds.sanitize(
-                            f"{CONSTRUCTION_SIGN_EMOJI}"
-                            " write number documentation"
-                        )
-                    ),
-                    mde.CompoundInlineElement(
-                        mde.InlineElement(f"{PAPERCLIP_EMOJI} ."),
-                        mde.BoldText(mde.InlineElement("flag")),
-                        mde.InlineElement(": "),
-                        mde.InlineElement("bool"),
-                        mde.InlineElement(" = "),
-                        mde.CodeSpan("False"),
-                    ),
-                    mde.BlockQuote(
-                        mds.sanitize(
-                            f"{CONSTRUCTION_SIGN_EMOJI}"
-                            " write flag documentation"
-                        )
-                    ),
-                    mde.CompoundInlineElement(
-                        mde.InlineElement(f"{PAPERCLIP_EMOJI} ."),
-                        mde.BoldText(mde.InlineElement("identifier")),
-                        mde.InlineElement(": "),
-                        mde.InlineElement("str"),
-                        mde.InlineElement(" = "),
-                        mde.CodeSpan("'dummy'"),
-                    ),
-                    mde.BlockQuote(
-                        mds.sanitize(
-                            f"{CONSTRUCTION_SIGN_EMOJI}"
-                            " write identifier documentation"
-                        )
+                    mde.UnorderedList(
+                        mde.ListItem(
+                            mde.Paragraph(
+                                mde.CompoundInlineElement(
+                                    mde.InlineElement(f"{PAPERCLIP_EMOJI} ."),
+                                    mde.BoldText(mde.InlineElement("number")),
+                                    mde.InlineElement(": "),
+                                    mde.InlineElement("int"),
+                                ),
+                            ),
+                            mde.BlockQuote(
+                                safe_missing_docstring(SDC_NAME, "number")
+                            ),
+                        ),
+                        mde.ListItem(
+                            mde.Paragraph(
+                                mde.CompoundInlineElement(
+                                    mde.InlineElement(f"{PAPERCLIP_EMOJI} ."),
+                                    mde.BoldText(mde.InlineElement("flag")),
+                                    mde.InlineElement(": "),
+                                    mde.InlineElement("bool"),
+                                    mde.InlineElement(" = "),
+                                    mde.CodeSpan("False"),
+                                ),
+                            ),
+                            mde.BlockQuote(
+                                safe_missing_docstring(SDC_NAME, "flag")
+                            ),
+                        ),
+                        mde.ListItem(
+                            mde.Paragraph(
+                                mde.CompoundInlineElement(
+                                    mde.InlineElement(f"{PAPERCLIP_EMOJI} ."),
+                                    mde.BoldText(
+                                        mde.InlineElement("identifier")
+                                    ),
+                                    mde.InlineElement(": "),
+                                    mde.InlineElement("str"),
+                                    mde.InlineElement(" = "),
+                                    mde.CodeSpan("'dummy'"),
+                                ),
+                            ),
+                            mde.BlockQuote(
+                                safe_missing_docstring(SDC_NAME, "identifier")
+                            ),
+                        ),
                     ),
                 ],
             )
 
-    def rest_frozen_dataclass(self) -> None:
+    def test_frozen_dataclass(self) -> None:
         """test initialization of a frozen data class"""
-        ast_class_def = list(parsed_body(FROZEN_DATACLASS))[0]
+        ast_class_def = tcom.first_parsed_body_element(FROZEN_DATACLASS)
         if isinstance(ast_class_def, ast.ClassDef):
             class_def = core.MorastClassDef(ast_class_def)
         else:
             raise ValueError("Excpected a class definition")
         #
         with self.subTest("name"):
-            self.assertEqual(class_def.name, "EmojiConfiguration")
+            self.assertEqual(class_def.name, FDC_NAME)
         #
         with self.subTest("is a dataclass"):
             self.assertTrue(class_def.is_a_dataclass)
         #
-        # =============================================================================
-        #         item = "enabled"
-        #         with self.subTest("instance_attribute", item=item):
-        #             current_node = class_def.instance_attrs[item]
-        #             if isinstance(current_node, nodes.Assignment):
-        #                 self.assertEqual(
-        #                     str(nodes.MorastName(item)),
-        #                     str(current_node.target),
-        #                 )
-        #             else:
-        #                 raise ValueError("expected an Assignment")
-        #             #
-        #         #
-        # =============================================================================
+        item = "enabled"
+        with self.subTest("instance_attribute", item=item):
+            current_attr = class_def.attribute_lists[core.SCOPE_INSTANCE][item]
+            if isinstance(current_attr, core.MorastAttribute):
+                self.assertEqual(current_attr.name, item)
+                self.assertEqual(current_attr.scope, core.SCOPE_INSTANCE)
+            else:
+                raise ValueError("expected an Attribute")
+            #
         #
         with self.subTest("MarkDown elements"):
             self.assertEqual(
                 list(class_def.markdown_elements()),
                 [
                     mde.HorizontalRule(20),
                     mde.Header(3, "Frozen dataclass EmojiConfiguration()"),
                     mde.BlockQuote(
                         mds.sanitize("Configuration of emoji for …")
                     ),
-                    mde.HorizontalRule(20),
                     mde.Header(4, "instance attributes"),
-                    mde.CompoundInlineElement(
-                        mde.InlineElement(f"{PAPERCLIP_EMOJI} ."),
-                        mde.BoldText(mde.InlineElement("enabled")),
-                        mde.InlineElement(": "),
-                        mde.InlineElement("bool"),
-                        mde.InlineElement(" = "),
-                        mde.CodeSpan("True"),
-                    ),
-                    mde.BlockQuote(
-                        mds.sanitize(
-                            f"{CONSTRUCTION_SIGN_EMOJI}"
-                            " write enabled documentation"
-                        )
+                    mde.UnorderedList(
+                        mde.ListItem(
+                            mde.Paragraph(
+                                mde.CompoundInlineElement(
+                                    mde.InlineElement(f"{PAPERCLIP_EMOJI} ."),
+                                    mde.BoldText(mde.InlineElement("enabled")),
+                                    mde.InlineElement(": "),
+                                    mde.InlineElement("bool"),
+                                    mde.InlineElement(" = "),
+                                    mde.CodeSpan("True"),
+                                ),
+                            ),
+                            mde.BlockQuote(
+                                safe_missing_docstring(FDC_NAME, "enabled")
+                            ),
+                        ),
                     ),
                 ],
             )
 
 
 # vim: fileencoding=utf-8 ts=4 sts=4 sw=4 autoindent expandtab syntax=python:
```

### Comparing `morast-0.3.1/tests/test_main.py` & `morast-0.3.3/tests/test_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 morast is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
-
 import io
 import sys
 
 from unittest import TestCase
 
 from unittest.mock import patch
```

### Comparing `morast-0.3.1/tests/test_nodes.py` & `morast-0.3.3/tests/test_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 morast is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
-
 import ast
 import logging
 
 from unittest import TestCase
 
 from smdg import elements as mde
```

