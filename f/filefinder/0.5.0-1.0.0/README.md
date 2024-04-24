# Comparing `tmp/filefinder-0.5.0.tar.gz` & `tmp/filefinder-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filefinder-0.5.0.tar", last modified: Wed Aug 24 17:46:43 2022, max compression
+gzip compressed data, was "filefinder-1.0.0.tar", last modified: Wed Apr 24 22:54:59 2024, max compression
```

## Comparing `filefinder-0.5.0.tar` & `filefinder-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 17:46:43.851844 filefinder-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-08-24 17:46:33.000000 filefinder-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-08-24 17:46:33.000000 filefinder-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2825 2022-08-24 17:46:43.851844 filefinder-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1876 2022-08-24 17:46:33.000000 filefinder-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-08-24 17:46:33.000000 filefinder-0.5.0/changelog.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-24 17:46:43.851844 filefinder-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1765 2022-08-24 17:46:33.000000 filefinder-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 17:46:43.847845 filefinder-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 17:46:43.847845 filefinder-0.5.0/src/filefinder/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-24 17:46:33.000000 filefinder-0.5.0/src/filefinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19726 2022-08-24 17:46:33.000000 filefinder-0.5.0/src/filefinder/finder.py
--rw-r--r--   0 runner    (1001) docker     (121)     7175 2022-08-24 17:46:33.000000 filefinder-0.5.0/src/filefinder/format.py
--rw-r--r--   0 runner    (1001) docker     (121)     3877 2022-08-24 17:46:33.000000 filefinder-0.5.0/src/filefinder/library.py
--rw-r--r--   0 runner    (1001) docker     (121)    10116 2022-08-24 17:46:33.000000 filefinder-0.5.0/src/filefinder/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 17:46:43.851844 filefinder-0.5.0/src/filefinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2825 2022-08-24 17:46:43.000000 filefinder-0.5.0/src/filefinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-08-24 17:46:43.000000 filefinder-0.5.0/src/filefinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-24 17:46:43.000000 filefinder-0.5.0/src/filefinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-08-24 17:46:43.000000 filefinder-0.5.0/src/filefinder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:54:59.274006 filefinder-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-24 22:54:55.000000 filefinder-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-24 22:54:55.000000 filefinder-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-24 22:54:59.274006 filefinder-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-24 22:54:55.000000 filefinder-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-24 22:54:55.000000 filefinder-1.0.0/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-24 22:54:55.000000 filefinder-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 22:54:59.274006 filefinder-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:54:59.270006 filefinder-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:54:59.270006 filefinder-1.0.0/src/filefinder/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-24 22:54:55.000000 filefinder-1.0.0/src/filefinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19135 2024-04-24 22:54:55.000000 filefinder-1.0.0/src/filefinder/finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-04-24 22:54:55.000000 filefinder-1.0.0/src/filefinder/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-04-24 22:54:55.000000 filefinder-1.0.0/src/filefinder/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-24 22:54:55.000000 filefinder-1.0.0/src/filefinder/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-04-24 22:54:55.000000 filefinder-1.0.0/src/filefinder/matches.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:54:55.000000 filefinder-1.0.0/src/filefinder/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:54:59.274006 filefinder-1.0.0/src/filefinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-24 22:54:59.000000 filefinder-1.0.0/src/filefinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-24 22:54:59.000000 filefinder-1.0.0/src/filefinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 22:54:59.000000 filefinder-1.0.0/src/filefinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 22:54:59.000000 filefinder-1.0.0/src/filefinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 22:54:59.000000 filefinder-1.0.0/src/filefinder.egg-info/top_level.txt
```

### Comparing `filefinder-0.5.0/LICENSE` & `filefinder-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `filefinder-0.5.0/PKG-INFO` & `filefinder-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,103 @@
 Metadata-Version: 2.1
 Name: filefinder
-Version: 0.5.0
+Version: 1.0.0
 Summary: Find files using a simple syntax.
-Home-page: https://github.com/Descanonge/filefinder
-Author: Clément Haëck
-Author-email: clement.haeck@posteo.net
+Author-email: Clément Haëck <clement.haeck@locean.ipsl.fr>
 Project-URL: Source, https://github.com/Descanonge/filefinder
 Project-URL: Documentation, https://filefinder.readthedocs.io
-Keywords: find files filename regular expression regex xarray
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: sphinx==6.2.1; extra == "dev"
+Requires-Dist: sphinx-book-theme==1.0.1; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: mypy>=1.5; extra == "dev"
+Requires-Dist: pytest>=7.4; extra == "dev"
+Requires-Dist: pyfakefs; extra == "dev"
+Requires-Dist: hypothesis; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
 
 
 # FileFinder
 
 > Find files using a simple syntax.
 
 <div align="left">
 
 [![PyPI](https://img.shields.io/pypi/v/filefinder)](https://pypi.org/project/filefinder)
 [![GitHub release](https://img.shields.io/github/v/release/Descanonge/filefinder)](https://github.com/Descanonge/filefinder/releases)
+[![codecov](https://codecov.io/github/Descanonge/filefinder/branch/master/graph/badge.svg?token=D5OBXX61HM)](https://codecov.io/github/Descanonge/filefinder)
+![test status](https://github.com/Descanonge/filefinder/actions/workflows/tests.yml/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/filefinder/badge/?version=latest)](https://filefinder.readthedocs.io/en/latest/?badge=latest)
 
 </div>
 
-To find files, FileFinder allows to specify the structure of filenames with a simple syntax.
-Parts of the file structure varying from file to file can be indicated with format strings
-or regular expressions, or with pre-defined defaults (mainly for dates).
-Once setup, it can:
+FileFinder allows to specify the structure of filenames using a simple syntax.
+Parts of the file structure varying from file to file are indicated within named
+groups, either with format strings or regular expressions (with some pre-defined
+values for some names). Once setup, it can:
 
-- Find corresponding files in a directory
-- Parse information from the filenames
+- Find corresponding files in a directory (and sub-directories)
+- Parse values from the filenames
 - Select only filenames with specific values
 - Generate filenames
 
-The package also interface easily with `xarray.open_mfdataset`.
-
 ## Quick examples
 
-The following example will find all files with the structure ``Data/[month]/Temperature_[depth]_[date].nc``:
+The following example will find all files with the structure ``Data/param_[parameter]/Temperature_[date].nc``:
 ``` python
-finder = Finder('/.../Data', '%(m)/Temperature_%(depth:fmt=03d)_%(Y)%(m)%(d).nc')
+finder = Finder('/.../Data', 'param_%(parameter:fmt=.1f)/%(Y)/Temperature_%(Y)%(m)%(d).nc')
 files = finder.get_files()
 ```
 
-We can also select only some files, for instance the first day of each month:
+We can also select only some files, for instance only in january:
 ``` python
-finder.fix_matcher('d', 1)
-files = finder.get_files()
+    finder.fix_group('m', 1)
+    files = finder.get_files()
 ```
 
 We can retrieve values from found files:
 ``` python
-filename, matches = finder.files[0]
-depth = matches['depth'].get_match()
-date = filefinder.library.get_date(matches)
+    filename, matches = finder.files[0]
+    parameter = matches["parameter"]
+    # the date as a datetime object
+    date = filefinder.library.get_date(matches)
 ```
 
 And we can generate a filename with a set of parameters:
 ``` python
-finder.get_filename(depth=100, Y=2000, m=1, d=1)
-# Specifying the day is optional since we already fixed it to 1.
+    finder.make_filename(parameter=0.5, Y=2000, m=1, d=1)
+    # Specifying the month is optional since we already fixed it to 1.
 ```
 
-
 ## Requirements
 
-Python >= 3.7.
+Python >= 3.10
 
 ## Installation
 
 From pip:
 ``` sh
 pip install filefinder
 ```
 
 From source:
 ``` sh
-git clone https://github.com/Descanonge/filefinder.git
-cd filefinder
-pip install -e .
+pip install -e https://github.com/Descanonge/filefinder.git#egg=filefinder
 ```
 
 ## Documentation
 
 Documentation is available at [filefinder.readthedocs.io](https://filefinder.readthedocs.io).
```

### Comparing `filefinder-0.5.0/src/filefinder/finder.py` & `filefinder-1.0.0/src/filefinder/finder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,576 +1,561 @@
 """Main class."""
 
 # This file is part of the 'filefinder' project
 # (http://github.com/Descanonge/filefinder) and subject
 # to the MIT License as defined in the file 'LICENSE',
 # at the root of this project. © 2021 Clément Haëck
 
-from __future__ import annotations
-import os
+import itertools
 import logging
+import os
 import re
+from collections.abc import Sequence
+from copy import copy
+from typing import Any
 
-from typing import Any, Callable, Dict, List, Tuple
+from filefinder.group import Group, GroupKey
+from filefinder.matches import Matches, get_groups_indices
 
-from filefinder.matcher import (Matcher, Matches,
-                                get_matchers_indices,
-                                InvalidMatcher)
+logger = logging.getLogger(__name__)
 
-log = logging.getLogger(__name__)
 
+class Finder:
+    """Find files using a filename pattern.
 
-class Finder():
-    """Find files using a pre-regex.
+    The Finder object is the main entrance point to this library.
+    Given a root directory and a filename pattern, it can search for all
+    corresponding files.
 
     Parameters
     ----------
-    root: str
-        The root directory of a filetree where all files can be found.
-    pregex: str
-        The pre-regex. A regular expression with added 'Matchers'.
-        Only the matchers vary from file to file. See documentation
-        for details.
-    use_regex: bool
-        Characters outside of matchers are considered as valid regex (and not
-        escaped) if True. Default is False.
-    replacements: str, optional
-        Matchers to replace by a string:
-        `'matcher name' = 'replacement string'`.
-
-    Attributes
-    ----------
-    root: str
-        The root directory of the finder.
-    use_regex: bool
-        Characters outside of matchers are considered as valid regex (and not
-        escaped) if true.
+    root:
+        The root directory of the filetree where all files can be found.
+    pattern:
+        A regular expression with the addition of 'groups'. See :ref:`find-files` for
+        details.
+    use_regex:
+        If True, characters outside of groups are considered as valid regex (and
+        not escaped). Default is False.
+    scan_everything
+        If true, look into all sub-directories up to a depth of :attr:`max_scan_depth` .
+        This is appropriate if the pattern contains optional sub-directories. If false
+        (default), check that every sub-directory matches its part of the regular
+        expression, thus avoiding some work.
     """
 
-    def __init__(self, root: str, pregex: str, use_regex: bool = False,
-                 **replacements: str):
+    max_scan_depth: int = 32
+    """Maximum sub-directory depth to scan when :attr:`scan_everything` is True."""
 
-        if isinstance(root, (list, tuple)):
-            root = os.path.join(*root)
+    def __init__(
+        self,
+        root: str,
+        pattern: str,
+        use_regex: bool = False,
+        scan_everything: bool = False,
+    ):
         self.root: str = root
+        """The root directory of the finder."""
         self.use_regex: bool = use_regex
+        """If True, characters outside of groups are considered as valid regex
+        (and not escaped). Default is False."""
 
-        self._pregex: str = ''
-        self._regex: str = ''
+        self.scan_everything: bool = scan_everything
+        """Whether to scan all subdirectories."""
 
-        self._pattern: re.Pattern | None = None
-        self._matchers: List[Matcher] = []
-        self._segments: List[str] = []
-        """Segments of the pre-regex. Used to replace specific matchers.
-        `['text before matcher 1', 'matcher 1',
-        'text before matcher 2, 'matcher 2', ...]`
-        """
-        self._fixed_matchers: Dict[str, str] = dict()
-        self._files: List[Tuple[str, Matcher]] = []
-        self._scanned: bool = False
+        self._pattern: str
 
-        self.set_pregex(pregex, **replacements)
-        self._update_regex()
+        self.groups: list[Group] = []
+        self._segments: list[str] = []
+        """Segments of the pattern. Used to replace specific groups.
+        `['text before group 1', 'group 1',
+        'text before group 2, 'group 2', ...]`
+        """
+        self._files: list[tuple[str, Matches]] = []
+        self.scanned: bool = False
+        """True if files have been scanned with current parameters.
 
-    @property
-    def n_matchers(self) -> int:
-        """Number of matchers in pre-regex."""
-        return len(self._matchers)
+        Is reset to False if the cache (of scanned files) is voided, for instance by
+        operation like changing fixed values of groups.
+        """
+
+        self.set_pattern(pattern)
 
     @property
-    def scanned(self) -> bool:
-        """If files have been scanned."""
-        return self._scanned
+    def n_groups(self) -> int:
+        """Number of groups in pre-regex."""
+        return len(self.groups)
 
     @property
-    def files(self) -> List[Tuple[str, Matches]]:
+    def files(self) -> list[tuple[str, Matches]]:
         """List of filenames and their matches.
 
-        Will scan files if not already done.
+        Will scan files when accessed and cache the result, if it has not
+        already been done.
         """
-        if not self._scanned:
+        if not self.scanned:
             self.find_files()
         return self._files
 
-    def __repr__(self):
-        return '\n'.join([super().__repr__(), self.__str__()])
+    def __repr__(self) -> str:
+        """Human readable information."""
+        return "\n".join([super().__repr__(), self.__str__()])
+
+    def __str__(self) -> str:
+        """Human readable information."""
+        s = [
+            f"root: {self.root}",
+            f"pattern: {self._pattern}",
+            f"regex: {self.get_regex()}",
+        ]
+
+        fixed_groups = [
+            (i, g.fixed_value)
+            for i, g in enumerate(self.groups)
+            if g.fixed_value is not None
+        ]
+        if fixed_groups:
+            s.append("fixed groups:")
+            s += [f"\t fixed #{i} to {v}" for i, v in fixed_groups]
 
-    def __str__(self):
-        s = ['root: {}'.format(self.root)]
-        s += ["pre-regex: {}".format(self._pregex)]
-        if self._regex is not None:
-            s += ["regex: {}".format(self._regex)]
-        else:
-            s += ["regex not created"]
-        if self._fixed_matchers:
-            s += ["fixed matchers:"]
-            s += ["\t fixed #{} to {}".format(i, v)
-                  for i, v in self._fixed_matchers.items()]
-        if not self._scanned:
-            s += ["not scanned"]
+        if not self.scanned:
+            s.append("not scanned")
         else:
-            s += ["scanned: found {} files".format(len(self._files))]
-        return '\n'.join(s)
+            s.append(f"scanned: found {len(self._files)} files")
+        return "\n".join(s)
+
+    def set_scan_everything(self, scan_everything: bool, /) -> None:
+        """Set value for attribute :attr:`scan_everything`.
 
-    def get_files(self, relative: bool = False,
-                  nested: List[str] | None = None) -> List[str]:
+        Void cache if necessary.
+        """
+        if scan_everything != self.scan_everything:
+            self.scan_everything = scan_everything
+            self._void_cache()
+
+    def set_use_regex(self, use_regex: bool, /) -> None:
+        """Set value for attribute :attr:`use_regex`."""
+        self.use_regex = use_regex
+
+    def get_files(
+        self,
+        relative: bool = False,
+        nested: Sequence[str | Sequence[str]] | None = None,
+    ) -> list:
         """Return files that matches the regex.
 
         Lazily scan files: if files were already scanned, just return
         the stored list of files.
-        Scanned files are flushed if the regex is changed (by fixing matcher
+        Scanned files are flushed if the regex is changed (by fixing group
         for instance).
 
         Parameters
         ----------
-        relative: bool
+        relative:
             If True, filenames are returned relative to the finder
             root directory. If not, paths are absolute (default).
-        nested: list of str
+        nested:
             If not None, return nested list of filenames with each level
-            corresponding to a group in this argument. Last group in the list
-            is at the innermost level. A level specified as None refer to
-            matchers without a group.
+            corresponding to a group, or set of group. Last set in the list
+            is at the innermost level.
 
         Raises
         ------
-        KeyError
-            A level in `nested` is not in the pre-regex groups.
+        KeyError: A group name in `nested` is not found in the pattern.
         """
-        def _get_files(files_matches):
+
+        def get_files(files_matches):
             if relative:
                 return [f for f, _ in files_matches]
             return [self.get_absolute(f) for f, _ in files_matches]
 
-        def get_match(m, group):
-            return ''.join([m_.get_match(parsed=False) for m_ in m
-                            if m_.matcher.group == group])
-
-        def nest(files_matches, groups, relative):
-            if len(groups) == 0:
-                return _get_files(files_matches)
+        def get_key(matches: Matches, level: list[str]) -> str:
+            return ":".join(
+                [
+                    match.get_match(parse=False)
+                    for match in matches
+                    if match.group.name in level
+                ]
+            )
+
+        def nest(files_matches, levels, relative):
+            if len(levels) == 0:
+                return get_files(files_matches)
 
-            group = groups[0]
+            level = levels[0]
             files_grouped = []
-            matches = {}
+            matches: dict[str, int] = {}
+            # We need to sort files by their value.
+            # We use all unparsed matches joined in a single string as a key
+            # (using get_key). We store it in a dictionnary, the value being
+            # the corresponding index
             for f, m in files_matches:
-                match = get_match(m, group)
-                if match not in matches:
-                    matches[match] = len(matches)
+                key = get_key(m, level)
+                if key not in matches:
+                    matches[key] = len(matches)
                     files_grouped.append([])
-                files_grouped[matches[match]].append((f, m))
+                files_grouped[matches[key]].append((f, m))
 
-            return [nest(grp, groups[1:], relative) for grp in files_grouped]
+            return [nest(grp, levels[1:], relative) for grp in files_grouped]
 
         if not self.scanned:
             self.find_files()
 
         if nested is None:
-            files = _get_files(self._files)
+            files = get_files(self._files)
         else:
-            groups = [m.group for m in self._matchers]
-            for g in nested:
-                if g not in groups:
-                    raise KeyError(f'{g} is not in Finder groups.')
+            names = set(g.name for g in self.groups)
+            nested = [[name] if isinstance(name, str) else name for name in nested]
+            for name in itertools.chain(*nested):
+                if name not in names:
+                    raise KeyError(f"{name} is not in Finder groups.")
             files = nest(self._files, nested, relative)
 
         return files
 
     def get_relative(self, filename: str) -> str:
         """Get filename path relative to root."""
         return os.path.relpath(filename, self.root)
 
     def get_absolute(self, filename: str) -> str:
         """Get absolute path to filename."""
         return os.path.join(self.root, filename)
 
-    def fix_matcher(
-            self, key: int | str | Tuple[str],
-            value: Any,
-            fix_discard: bool = False
-    ):
-        """Fix a matcher to a string.
+    def fix_group(self, key: GroupKey, value: str | Any, fix_discard: bool = False):
+        """Fix a group to a string.
 
         Parameters
         ----------
-        key: int, or str, or tuple of str of length 2.
-            If int, is matcher index, starts at 0.
-            If str, can be matcher name, or a group and name combination with
-            the syntax 'group:name'.
-            When using strings, if multiple matchers are found with the same
-            name or group/name combination, all are fixed to the same value.
-        value: str or value, or list of
+        key:
+            Can be the index of a group in the pattern (starts at 0), or the
+            name of a group. If multiple groups share the same name, they are
+            all fixed to the same value.
+        value:
             Will replace the match for all files. Can be a string, or a value
-            that will be formatted using the matcher format string.
+            that will be formatted using the group format string.
             A list of values will be joined by the regex '|' OR.
-            Special characters should be properly escaped in strings.
-        fix_discard: bool
-            If True, matchers with the 'discard' option will still be fixed.
+            A string will be interpreted as a regular expression, so all special
+            characters should be properly escaped.
+        fix_discard:
+            If True, groups with the 'discard' option will still be fixed.
             Default is False.
         """
-        self._fix_matcher_no_update(key, value, fix_discard)
-        self._update_regex()
-
-    def _fix_matcher_no_update(self, key, value, fix_discard):
-        for m in self.get_matchers(key):
+        for m in self.get_groups(key):
             if not fix_discard and m.discard:
                 continue
-            self._fixed_matchers[m.idx] = value
+            m.fix_value(value)
+        self._void_cache()
 
-    def fix_matchers(
-            self, fixes: Dict[int | str | Tuple[str], Any] = None,
-            fix_discard: bool = False,
-            **fixes_kw
+    def fix_groups(
+        self,
+        fixes: dict[Any, str | Any] | None = None,
+        fix_discard: bool = False,
+        **fixes_kw: str | Any,
     ):
-        """Fix multiple values at once.
+        """Fix multiple groups at once.
 
         Parameters
         ----------
-        fixes: dict
-            Dictionnary of matcher key: value. See :func:`fix_matcher` for
-            details. If None, no matcher will be fixed.
-        fix_discard: bool
-            If True, matchers with the 'discard' option will still be fixed.
+        fixes:
+            Dictionnary of `{group key: value}`. See :func:`fix_group` for
+            details.
+        fix_discard:
+            If True, groups with the 'discard' option will still be fixed.
             Default is False.
         fixes_kw:
             Same as `fixes`. Takes precedence.
         """
         if fixes is None:
             fixes = {}
-        fixes.update(fixes_kw)
+        fixes.update(**fixes_kw)
         for f in fixes.items():
-            self._fix_matcher_no_update(*f, fix_discard=fix_discard)
-        self._update_regex()
+            self.fix_group(*f, fix_discard=fix_discard)
 
-    def unfix_matchers(self, *keys: str):
-        """Unfix matchers.
+    def unfix_groups(self, *keys: str):
+        """Unfix groups.
 
         Parameters
         ----------
-        keys: str
-           Keys to find matchers to unfix. See :func:`get_matchers`.
-           If no key is provided, all matchers will be unfixed.
+        keys:
+           Keys to find groups to unfix. See :func:`get_groups`.
+           If no key is provided, all groups will be unfixed.
         """
         if not keys:
-            self._fixed_matchers = {}
+            for g in self.groups:
+                g.unfix()
         else:
             for key in keys:
-                matchers = self.get_matchers(key)
-                for m in matchers:
-                    self._fixed_matchers.pop(m.idx, None)
-        self._update_regex()
-
-    def get_matches(self, filename: str,
-                    relative: bool = True) -> Matches:
-        """Get matches for a given filename.
+                groups = self.get_groups(key)
+                for g in groups:
+                    g.unfix()
+        self._void_cache()
+
+    def find_matches(self, filename: str, relative: bool = True) -> Matches | None:
+        """Find matches for a given filename.
 
-        Apply regex to `filename` and return the results as a
-        :class:`Matches<filefinder.matcher.Matches>` object.
+        Apply regex to `filename` and return the results as a :class:`~.matches.Matches`
+        object. Fixed values are applied as normal.
 
         Parameters
         ----------
-        filename: str
+        filename:
             Filename to retrieve matches from.
-        relative: bool
+        relative:
             True if the filename is relative to the finder root directory
             (default). If False, the filename is made relative before being
             matched.
 
-        Raises
-        ------
-        AttributeError
-            The regex is empty.
-        ValueError
-            The filename did not match the pattern.
-        IndexError
-            Not as many matches as matchers.
+        Returns
+        -------
+        matches
+            A :class:`~.matches.Matches` object, or None if the filename did not match.
         """
-        if not self._regex:
-            raise AttributeError("Finder is missing a regex.")
-
         if not relative:
             filename = self.get_relative(filename)
 
-        return Matches(self._matchers, filename, re.compile(self._regex))
+        return Matches.from_filename(filename, self.get_regex(), self.groups)
 
-    def get_filename(self, fixes: Dict | None = None, relative: bool = False,
-                     **kw_fixes: Any) -> str:
+    def make_filename(
+        self,
+        fixes: dict | None = None,
+        relative: bool = False,
+        **kw_fixes: Any,
+    ) -> str:
         """Return a filename.
 
-        Replace matchers with provided values.
-        All matchers must be fixed prior, or with `fixes` argument.
+        Replace groups with provided values.
+        All groups must be fixed prior, or with `fixes` argument.
 
         Parameters
         ----------
-        fixes: dict
-            Dictionnary of fixes (matcher key: value). For details, see
-            :func:`fix_matcher`. Will (temporarily) supplant matcher fixed
+        fixes:
+            Dictionnary of fixes (group name or index: value). For details, see
+            :func:`fix_group`. Will (temporarily) supplant group fixed
             prior. If prior fix is a list, first item will be used.
-        relative: bool
+        relative:
             If the filename should be relative to the finder root directory.
             Default is False.
         kw_fixes:
             Same as `fixes`. Takes precedence.
 
         Raises
         ------
-        ValueError
-            `use_regex` is activated.
+        ValueError: `use_regex` is activated.
         """
         if self.use_regex:
-            raise ValueError("Cannot generate a valid filename if regex "
-                             "is present outside matchers.")
+            raise ValueError(
+                "Cannot generate a valid filename if regex "
+                "is present outside groups (`use_regex=True`)."
+            )
 
-        fixed_matchers = self._fixed_matchers.copy()
         if fixes is None:
             fixes = {}
-        fixes.update(kw_fixes)
-        for key, value in fixes.items():
-            for m in self.get_matchers(key):
-                fixed_matchers[m.idx] = value
-
-        non_fixed = [i for i in range(self.n_matchers)
-                     if i not in fixed_matchers]
-        if any(non_fixed):
-            log.error("Matchers not fixed: %s",
-                      ', '.join([str(self._matchers[i]) for i in non_fixed]))
-            raise TypeError("Not all matchers were fixed.")
+        fixes.update(**kw_fixes)
 
         segments = self._segments.copy()
+        groups = [copy(g) for g in self.groups]  # shallow copy (no reparsing of def)
 
-        for idx, value in fixed_matchers.items():
-            if isinstance(value, bool):
-                value = self._matchers[idx].opt[value]
-            if isinstance(value, (list, tuple)):
-                value = value[0]
-            if not isinstance(value, str):
-                value = self._matchers[idx].format(value)
-            segments[2*idx+1] = value
+        for i, g in enumerate(groups):
+            if g.name in fixes:
+                g.fix_value(fixes[g.name])
+            if i in fixes:
+                g.fix_value(fixes[i])
+
+            if g.fixed_string is not None:
+                segments[2 * i + 1] = g.fixed_string
+            else:
+                raise ValueError(f"Group '{g!s}' has no fixed value.")
 
-        filename = ''.join(segments)
+        filename = "".join(segments).replace("/", os.sep)
 
         if not relative:
             filename = self.get_absolute(filename)
 
         return filename
 
-    def get_func_process_filename(self, func: Callable, relative: bool = True,
-                                  *args, **kwargs) -> Callable:
-        r"""Get a function that can preprocess a dataset.
-
-        Written to be used as the 'process' argument of
-        `xarray.open_mfdataset`. Allows to use a function with additional
-        arguments, that can retrieve information from the filename.
-
-        Parameters
-        ----------
-        func: Callable
-            Input arguments (`xarray.Dataset`, filename: `str`,
-            `Finder`, \*args, \*\*kwargs)
-            Should return a Dataset.
-            Filename is retrieved from the dataset encoding attribute.
-        relative: If True (default), `filename` is made relative to the finder
-            root. This is necessary to match the filename against the finder
-            regex.
-        args: optional
-            Passed to `func` when called.
-        kwargs: optional
-            Passed to `func` when called.
-
-        Returns
-        -------
-        Callable
-             Function with the signature of the 'process' argument of
-             `xarray.open_mfdataset`.
-
-        Examples
-        --------
-        This retrieve the date from the filename, and add a time dimensions
-        to the dataset with the corresponding value.
-        >>> from filefinder import library
-        ... def process(ds, filename, finder, default_date=None):
-        ...     matches = finder.get_matches(filename)
-        ...     date = library.get_date(matches, default_date=default_date)
-        ...     ds = ds.assign_coords(time=[date])
-        ...     return ds
-        ...
-        ... ds = xr.open_mfdataset(finder.get_files(),
-        ...                        preprocess=finder.get_func_process_filename(
-        ...     process, default_date={'hour': 12}))
-        """
-        def f(ds):
-            filename = ds.encoding['source']
-            if relative:
-                filename = self.get_relative(filename)
-            return func(ds, filename, self, *args, **kwargs)
-        return f
-
-    def set_pregex(self, pregex: str, **replacements: str):
-        """Set pre-regex.
-
-        Apply replacements.
-        """
-        pregex = pregex.strip()
-        for k, z in replacements.items():
-            pregex = pregex.replace("%({:s})".format(k), z)
-        self._pregex = pregex
-        self._scan_pregex()
-        self._update_regex()
-
-    def _scan_pregex(self):
-        """Scan pregex for matchers.
-
-        Add matchers objects to self.
-        Set segments attribute.
-        """
-        matchers_starts = [m.start()+1
-                           for m in re.finditer(r'%\(', self._pregex)]
-
-        self._matchers = []
-        splits = [0]
-        for idx, start in enumerate(matchers_starts):
+    def get_pattern(self) -> str:
+        """Get filename pattern."""
+        return self._pattern
+
+    def set_pattern(self, pattern: str):
+        """Set pattern and parse for group objects."""
+        self._void_cache()
+        self._pattern = pattern
+        groups_starts = [m.start() + 1 for m in re.finditer(r"%\(", pattern)]
+
+        # This finds the matching end parenthesis for each group start
+        self.groups = []
+        splits = [0]  # separation between groups
+        for idx, start in enumerate(groups_starts):
             end = None
             level = 1
-            for i, c in enumerate(self._pregex[start+1:]):
+            for i, c in enumerate(pattern[start + 1 :]):
                 if c == "(":
                     level += 1
                 elif c == ")":
                     level -= 1
-                    if level == 0:
-                        end = start+i+1
+                    if level == 0:  # matching parenthesis
+                        end = start + i + 1
                         break
 
-            if end is None:
-                end = start+6
-                substr = self._pregex[start-1:end]
-                if end < len(self._pregex):
-                    substr += '...'
-                raise ValueError("No matcher end found for '{}'"
-                                 .format(substr))
-
-            try:
-                self._matchers.append(Matcher(self._pregex[start+1:end], idx))
-                splits += [start-1, end+1]  # -1 removes the %
-            except InvalidMatcher:
-                pass
-
-        self._segments = [self._pregex[i:j]
-                          for i, j in zip(splits, splits[1:]+[None])]
-
-        # Replace matcher by its regex
-        for idx, m in enumerate(self._matchers):
-            self._segments[2*idx+1] = m.get_regex()
+            if end is None:  # did not find matching parenthesis :(
+                end = start + 6
+                substr = pattern[start - 1 : end]
+                if end < len(self._pattern):
+                    substr += "..."
+                raise ValueError(f"No group end found for '{substr}'")
 
-    def _update_regex(self):
-        """Update regex.
+            self.groups.append(Group(pattern[start + 1 : end], idx))
+            splits += [start - 1, end + 1]  # -1 removes the %
 
-        Set fixed matchers. Compute regex. Scrap previous scanning.
-        """
+        self._segments = [pattern[i:j] for i, j in zip(splits, splits[1:] + [None])]
+
+    def _get_regex(self) -> str:
         segments = self._segments.copy()
         if not self.use_regex:
-            for i, s in enumerate(segments):
-                # Escape outside matchers
-                segments[i] = s if i % 2 == 1 else re.escape(s)
-
-        for idx, value in self._fixed_matchers.items():
-            if isinstance(value, bool):
-                if isinstance(self._matchers[idx].opt, tuple):
-                    value = self._matchers[idx].opt[value]
-            if not isinstance(value, (list, tuple)):
-                value = [value]
-            value = [v if isinstance(v, str)
-                     else re.escape(self._matchers[idx].format(v))
-                     for v in value]
-            segments[2*idx+1] = '({})'.format('|'.join(value))
-
-        self._regex = ''.join(segments)
-        self._scanned = False
-        self._files = []
+            # escape regex outside groups
+            segments = [
+                s if (i % 2 == 1) else re.escape(s) for i, s in enumerate(segments)
+            ]
+
+        for idx, group in enumerate(self.groups):
+            segments[2 * idx + 1] = group.get_regex()
+
+        return "".join(segments)
+
+    def get_regex(self) -> str:
+        """Return regex."""
+        return self._get_regex().replace("/", re.escape(os.sep))
+
+    def get_regex_subdirs(self) -> list[str]:
+        """Return regexes for each sub-directory."""
+        return self._get_regex().split("/")
 
     def find_files(self):
         """Find files to scan and store them.
 
-        Is automatically called when accessing :attr:`files` or
-        :func:`get_files`.
-        Sort files alphabetically.
+        Is automatically called when accessing :attr:`files` or :func:`get_files`. Sort
+        files alphabetically.
+        """
+        if self.scan_everything:
+            self._find_files_scan_everything()
+        else:
+            self._find_files_subdirectories()
 
-        Raises
-        ------
-        AttributeError
-            If no regex is set.
-        IndexError
-            If no files are found in the filetree.
-        """
-        if self._regex is None:
-            self.create_regex()
-        if self._regex == '':
-            raise AttributeError("Finder is missing a regex.")
+        self._files.sort(key=lambda x: x[0])
+
+    def _find_files_scan_everything(self) -> None:
+        """Find files checking every sub-directory.
+
+        Because having to check if a sub-directory matches the pattern is difficult,
+        this allows for more exotic patterns where a folder separator can appear in a
+        capturing group, by example for optional sub-directories.
+
+        This will the whole filetree under :attr:`root_directory` and check every file
+        found, which can be significant work in some cases.
+        """
+        pattern = re.compile(self.get_regex())
+        files_matched = []
+
+        for dirpath, dirnames, filenames in os.walk(self.root):
+            depth = dirpath.rstrip(os.sep).count(os.sep) - self.root.rstrip(
+                os.sep
+            ).count(os.sep)
+            if depth > self.max_scan_depth:
+                dirnames.clear()
+
+            for f in filenames:
+                to_root = self.get_relative(os.path.join(dirpath, f))
+                matches = Matches.from_filename(to_root, pattern, self.groups)
+                if matches is not None:
+                    files_matched.append((to_root, matches))
+
+        self.scanned = True
+        self._files = files_matched
+
+    def _find_files_subdirectories(self) -> None:
+        """Find files checking sub-directories along the way.
 
-        subpatterns = [re.compile(rgx)
-                       for rgx in self._regex.split(os.path.sep)]
+        Each sub-directory must match against its corresponding part of the generated
+        regular expression. This is ill suited if any group contains a folder
+        separator. But it will limit the number of sub-directories to explore and
+        thus the number of files to check.
+        """
+        max_log_lines = 3
+
+        subpatterns = [re.compile(rgx) for rgx in self.get_regex_subdirs()]
         files = []
         for dirpath, dirnames, filenames in os.walk(self.root):
-            # Feels hacky, better way ?
-            depth = dirpath.count(os.sep) - self.root.count(os.sep)
+            depth = dirpath.rstrip(os.sep).count(os.sep) - self.root.rstrip(
+                os.sep
+            ).count(os.sep)
             pattern = subpatterns[depth]
 
-            if depth == len(subpatterns)-1:
-                dirnames.clear()  # Look no deeper
-                files += [self.get_relative(os.path.join(dirpath, f))
-                          for f in filenames]
-            else:
-                dirlogs = dirnames[:3]
-                if len(dirnames) > 3:
-                    dirlogs += ['...']
-                log.debug('depth: %d, pattern: %s, folders:\n\t%s',
-                          depth, pattern.pattern, '\n\t'.join(dirlogs))
+            if depth == len(subpatterns) - 1:
+                dirnames.clear()  # look no deeper
+                files += [
+                    self.get_relative(os.path.join(dirpath, f)) for f in filenames
+                ]
+            elif logger.isEnabledFor(logging.DEBUG):
+                dirlogs = dirnames[:max_log_lines]
+                if len(dirnames) > max_log_lines:
+                    dirlogs += ["..."]
+                logger.debug(
+                    "depth: %d, pattern: %s, folders:\n\t%s",
+                    depth,
+                    pattern.pattern,
+                    "\n\t".join(dirlogs),
+                )
 
             # Removes directories not matching regex
-            # We do double regex on directories, good enough
             to_remove = [d for d in dirnames if not pattern.fullmatch(d)]
             for d in to_remove:
                 dirnames.remove(d)
 
-        files.sort()
+        logger.debug("Found %s files in sub-directories", len(files))
 
+        # Now only retain files that match the full pattern
+        pattern = re.compile(self.get_regex())
         files_matched = []
+
         for f in files:
-            try:
-                matches = self.get_matches(f, relative=True)
-            except ValueError:  # Filename did not match pattern
-                pass
-            else:
+            matches = Matches.from_filename(f, pattern, self.groups)
+            if matches is not None:
                 files_matched.append((f, matches))
 
-        filelogs = files[:3]
-        if len(files) > 3:
-            filelogs += ['...']
-        log.debug("regex: %s, files:\n\t%s", self._regex, '\n\t'.join(filelogs))
-        log.debug("Found %s matching files in %s",
-                  len(files_matched), self.root)
+        if logger.isEnabledFor(logging.DEBUG):
+            filelogs = files[:max_log_lines]
+            if len(files) > max_log_lines:
+                filelogs += ["..."]
+            logger.debug(
+                "regex: %s, files:\n\t%s", pattern.pattern, "\n\t".join(filelogs)
+            )
+            logger.debug("Found %s matching files in %s", len(files_matched), self.root)
 
-        self._scanned = True
+        self.scanned = True
         self._files = files_matched
 
-    def get_matchers(self, key: int | str) -> List[Matcher]:
-        """Return list of matchers corresponding to key.
+    def _void_cache(self) -> None:
+        self.scanned = False
+        self._files.clear()
+
+    def get_groups(self, key: GroupKey) -> list[Group]:
+        """Return list of groups corresponding to key.
 
         Parameters
         ----------
         key: int, str, or list of int
-            Can be matcher index, name, or group+name combination with the
+            Can be group index, name, or group+name combination with the
             syntax: 'group:name'.
 
         Returns
         -------
-        List of matchers corresponding to key.
+        List of groups corresponding to key.
 
         Raises
         ------
-        KeyError
-            No matcher found.
-        TypeError
-            Key type is not valid.
-        """
-        selected = get_matchers_indices(self._matchers, key)
-        matchers = [self._matchers[i] for i in selected]
-        return matchers
+        KeyError: No group found.
+        TypeError: Key type is not valid.
+        """
+        selected = get_groups_indices(self.groups, key)
+        groups = [self.groups[i] for i in selected]
+        return groups
```

### Comparing `filefinder-0.5.0/src/filefinder/library.py` & `filefinder-1.0.0/src/filefinder/library.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,88 +1,78 @@
 """Functions to retrieve values from filename."""
 
 # This file is part of the 'filefinder' project
 # (http://github.com/Descanonge/filefinder) and subject
 # to the MIT License as defined in the file 'LICENSE',
 # at the root of this project. © 2021 Clément Haëck
 
-from datetime import datetime, timedelta
 import logging
-from typing import Dict
+from collections.abc import Callable
+from datetime import datetime, timedelta
 
-from filefinder.matcher import Matches
+from .matches import Matches
 
-log = logging.getLogger(__name__)
+logger = logging.getLogger(__name__)
 
 
-def get_date(matches: Matches, default_date: Dict = None,
-             group: str = None) -> datetime:
+def get_date(matches: Matches, default_date: dict | None = None) -> datetime:
     """Retrieve date from matched elements.
 
     If a matcher is *not* found in the filename, it will be replaced by the
     element of the default date argument.
     Matchers that can be used are (in order of increasing priority):
     YBmdjHMSFxX. If two matchers have the same name, the last one in the
     pre-regex will get priority.
 
     Parameters
     ----------
-    matches: :class:`Matches<filefinder.matcher.Matches>`
+    matches:
         Matches obtained from a filename.
-    group: str
-        If not None, restrict matchers to this group.
-    default_date: dict, optional
+    default_date:
         Default date. Dictionnary with keys: year, month, day, hour, minute,
         and second. Defaults to 1970-01-01 00:00:00
-
-    Raises
-    ------
-    KeyError
-        If no matchers are found to create a date from.
     """
-    NAME_TO_DATETIME = dict(
-        Y='year', m='month', d='day', H='hour', M='minute', S='second')
+    name_to_datetime = dict(
+        Y="year", m="month", d="day", H="hour", M="minute", S="second"
+    )
 
-    def get_elts(names: str, callback):
+    def get_elts(elts: dict[str, str], names: str, callback: Callable):
         for name in names:
             elt = elts.pop(name, None)
             if elt is not None:
                 date.update(callback(elt, name))
 
-    def process_int(elt, name):
-        return {NAME_TO_DATETIME[name]: int(elt)}
+    def process_int(elt: str, name: str) -> dict[str, int]:
+        return {name_to_datetime[name]: int(elt)}
+
+    def process_month_name(elt: str, name: str) -> dict[str, int]:
+        return dict(month=_find_month_number(elt))
 
-    def process_month_name(elt, name):
-        elt = _find_month_number(elt)
-        if elt is not None:
-            return dict(month=elt)
-        return {}
-
-    def process_doy(elt, name):
-        elt = datetime(date["year"], 1, 1) + timedelta(days=int(elt)-1)
-        return dict(month=elt.month, day=elt.day)
+    def process_doy(elt: str, name: str) -> dict[str, int]:
+        d = datetime(date["year"], 1, 1) + timedelta(days=int(elt) - 1)
+        return dict(month=d.month, day=d.day)
 
-    date = {"year": 1970, "month": 1, "day": 1,
-            "hour": 0, "minute": 0, "second": 0}
+    date = {"year": 1970, "month": 1, "day": 1, "hour": 0, "minute": 0, "second": 0}
 
     if default_date is None:
         default_date = {}
     date.update(default_date)
 
-    elts = {m.matcher.name: m.get_match(parsed=False) for m in matches
-            if (not m.matcher.discard
-                and (group is None or m.matcher.group == group))}
+    elts = {
+        m.group.name: m.get_match(parse=False) for m in matches if not m.group.discard
+    }
 
-    elts_needed = set('xXYmdBjHMSF')
+    elts_needed = set("xXYmdBjHMSF")
     if len(set(elts.keys()) & elts_needed) == 0:
-        log.warning("No matchers to retrieve a date from."
-                    " Returning default date.")
+        logger.warning(
+            "No matchers to retrieve a date from." " Returning default date."
+        )
 
     # Process month name first to keep element priorities simples
-    get_elts('B', process_month_name)
+    get_elts(elts, "B", process_month_name)
 
     # Decompose elements
     elt = elts.pop("F", None)
     if elt is not None:
         elts["Y"] = elt[:4]
         elts["m"] = elt[5:7]
         elts["d"] = elt[8:10]
@@ -93,36 +83,47 @@
         elts["m"] = elt[4:6]
         elts["d"] = elt[6:8]
 
     elt = elts.pop("X", None)
     if elt is not None:
         elts["H"] = elt[:2]
         elts["M"] = elt[2:4]
-        if len(elt) > 4:
+        if len(elt) > 4:  # noqa: PLR2004
             elts["S"] = elt[4:6]
 
     # Process elements
-    get_elts('Ymd', process_int)
-    get_elts('j', process_doy)
-    get_elts('HMS', process_int)
+    get_elts(elts, "Ymd", process_int)
+    get_elts(elts, "j", process_doy)
+    get_elts(elts, "HMS", process_int)
 
-    return datetime(**date)
+    return datetime(**date)  # type: ignore
 
 
 def _find_month_number(name: str) -> int:
     """Find a month number from its name.
 
     Name can be the full name (January) or its three letter abbreviation (jan).
     The casing does not matter.
     """
-    names = ['january', 'february', 'march', 'april',
-             'may', 'june', 'july', 'august', 'september',
-             'october', 'november', 'december']
+    names = [
+        "january",
+        "february",
+        "march",
+        "april",
+        "may",
+        "june",
+        "july",
+        "august",
+        "september",
+        "october",
+        "november",
+        "december",
+    ]
     names_abbr = [c[:3] for c in names]
 
     name = name.lower()
     if name in names:
         return names.index(name) + 1
     if name in names_abbr:
         return names_abbr.index(name) + 1
 
-    return None
+    raise ValueError(f"Could not interpret month name '{name}'")
```

### Comparing `filefinder-0.5.0/src/filefinder/matcher.py` & `filefinder-1.0.0/src/filefinder/matches.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,346 +1,269 @@
 """Matches management."""
 
 # This file is part of the 'filefinder' project
 # (http://github.com/Descanonge/filefinder) and subject
 # to the MIT License as defined in the file 'LICENSE',
 # at the root of this project. © 2021 Clément Haëck
 
-import re
 import logging
-from typing import Any, List, Union
-
-from .format import Format
-
-
-log = logging.getLogger(__name__)
+import re
+import typing as t
+from collections import abc
 
+from .group import Group, GroupKey
 
-class InvalidMatcher(ValueError):
-    """No valid matcher could be found in pre-regex substring."""
-    pass
+logger = logging.getLogger(__name__)
 
 
-class Matcher():
-    """Manage a matcher inside the pre-regex.
+class Match:
+    """Match extract from a filename.
 
     Parameters
     ----------
-    m: re.Match
-        Match object obtained to find matchers in the pre-regex.
-    idx: int
-        Index inside the pre-regex.
-
-    Attributes
-    ----------
-    idx: int
-        Index inside the pre-regex.
-    group: str
-        Group name.
-    name: str
-        Matcher name.
-    rgx: str
-        Regex.
-    discard: bool
-        If the matcher should not be used when retrieving values from matches.
-    fmt: :class:`Format<filefinder.format.Format>`
-        Format string object.
-    match: str
-        The string that created the matcher `%(match)`.
-    """
-
-    DEFAULT_ELTS = {
-        "I": [r"\d+", 'd'],
-        "Y": [r"\d{4}", '04d'],
-        "m": [r"\d\d", '02d'],
-        "d": [r"\d\d", '02d'],
-        "j": [r"\d{3}", '03d'],
-        "H": [r"\d\d", '02d'],
-        "M": [r"\d\d", '02d'],
-        "S": [r"\d\d", '02d'],
-        "x": [r"%Y%m%d", '08d'],
-        "X": [r"%H%M%S", '06d'],
-        "F": [r"%Y-%m-%d", 's'],
-        "B": [r"[a-zA-Z]*", 's'],
-        "text": [r'\w', 's'],
-        "char": [r"\S*", 's']
-    }
-    """Regex str for each type of element."""
-
-    REGEX = (r"^(?:(?P<group>\w*):)??"
-             r"(?P<name>\w*)"
-             r"(:fmt=(?P<fmt>.*?))?"
-             r"(?P<opt>:opt(?:=(?P<optA>.*?):(?P<optB>.*?))?)?"
-             r"(:rgx=(?P<rgx>.*?))?"
-             r"(?P<discard>:discard)?")
-    """Regex to find matcher properties from pre-regex substring."""
-
-    def __init__(self, matcher: str, idx: int):
-        self.idx = idx
-        self.group = None
-        self.name = None
-        self.rgx = None
-        self.discard = False
-        self.fmt = None
-        self.opt = None
-        self.match = ''
-
-        self.set_matcher(matcher)
-
-    def __repr__(self):
-        return '\n'.join([super().__repr__(), self.__str__()])
-
-    def __str__(self):
-        s = ''
-        if self.group:
-            s += self.group + ':'
-        s += '{}:{:d}'.format(self.name, self.idx)
-        return s
-
-    def set_matcher(self, matcher: str):
-        """Find attributes from match.
-
-        Raises
-        ------
-        NameError
-            No name.
-        ValueError
-            Empty custom regex or format.
-        KeyError
-            No regex could be produced (name is not in defaults, and no regex
-            was specified).
-        InvalidMatcher
-            Pre-regex substring contains no valid matcher.
-        """
-        m = re.fullmatch(self.REGEX, matcher)
-        if m is None:
-            log.warning("No matcher found in sub-string %s", matcher)
-            raise InvalidMatcher("No matcher found in sub-string")
-
-        self.match = matcher
-        self.group = m.group('group')
-        self.name = m.group('name')
-        self.discard = m.group('discard') is not None
-
-        rgx = m.group('rgx')
-        fmt = m.group('fmt')
-
-        if self.name is None:
-            raise NameError("Matcher name cannot be empty.")
-        if rgx is not None and rgx == '':
-            raise ValueError("Matcher custom regex cannot be empty.")
-        if fmt is not None and fmt == '':
-            raise ValueError("Matcher custom format cannot be empty.")
-
-        # Set defaults if name is known
-        if self.name in self.DEFAULT_ELTS:
-            self.rgx, fmt_def = self.DEFAULT_ELTS[self.name]
-            self.fmt = Format(fmt_def)
-
-        # Override default format
-        if fmt:
-            self.fmt = Format(fmt)
-            if not rgx:  # No need to generate rgx if it is provided
-                self.rgx = self.fmt.generate_expression()
-
-        if m.group('opt') is not None:
-            optA, optB = m.group('optA'), m.group('optB')
-            if optA is not None or optB is not None:
-                optA = '' if optA is None else optA
-                optB = '' if optB is None else optB
-                self.opt = (optA, optB)
-                self.rgx = '{}|{}'.format(optA, optB)
-            else:
-                self.opt = True
-
-        # Override regex
-        if rgx:
-            self.rgx = rgx
-
-        if self.rgx is None:
-            raise KeyError("No regex could have been produced for "
-                           "matcher '{}'.".format(matcher))
-
-    def format(self, value: Any):
-        return self.fmt.format(value)
-
-    def get_regex(self) -> str:
-        """Get matcher regex.
-
-        Replace the matchers name by regex from `Matcher.NAME_RGX`. If there is
-        a custom regex, recursively replace '%' followed by a single letter by
-        the corresponding regex from `NAME_RGX`. '%%' is replaced by a single
-        percentage character.
-
-        Raises
-        ------
-        KeyError
-            Unknown replacement.
-        """
-        def replace(match):
-            group = match.group(1)
-            if group == '%':
-                return '%'
-            if group in self.DEFAULT_ELTS:
-                replacement = self.DEFAULT_ELTS[group][0]
-                if '%' in replacement:
-                    return self.get_regex(replacement)
-                return replacement
-            raise KeyError("Unknown replacement '{}'.".format(match.group(0)))
-
-        rgx = re.sub("%([a-zA-Z%])", replace, self.rgx)
-
-        # Make it matching
-        rgx = '({})'.format(rgx)
-
-        if self.opt is True:
-            rgx += '?'
-
-        return rgx
-
-
-class Match:
-    """Match extract from a filename.
+    group
+        Group used to get this match.
+    match
+        Match object for the complete filename.
+    idx
+        Index of the group in the match object.
 
     Attributes
     ----------
-    matcher: Matcher
-        Matcher used to get this match.
-    match_str: str
+    group:
+        Group used to get this match.
+    match_str:
         String matched in the filename.
-    start: int
+    start:
         Start index of match in the filename.
-    end: int
+    end:
         End index of match in the filename.
-    match_parsed: any
+    match_parsed:
         Parsed value. None if parsing was not successful.
     """
 
-    def __init__(self, matcher: Matcher, match: re.Match, group: int):
-        self.matcher = matcher
-        self.match_str = match.group(group+1)
-        self.start = match.start(group+1)
-        self.end = match.end(group+1)
-
-        self.match_parsed = None
-        if matcher.fmt is not None:
-            try:
-                self.match_parsed = matcher.fmt.parse(self.match_str)
-            except Exception:
-                log.warning('Failed to parse for matcher %s', str(matcher))
+    def __init__(self, group: Group, match: re.Match, idx: int):
+        self.group: Group = group
+        self.match_str: str = match.group(idx + 1)
+        self.start: int = match.start(idx + 1)
+        self.end: int = match.end(idx + 1)
+
+        self.match_parsed: t.Any = None
+        try:
+            self.match_parsed = group.parse(self.match_str)
+        except Exception:
+            logger.debug("Failed to parse for group %s", str(group))
 
     def __repr__(self):
-        return '\n'.join([super().__repr__(), self.__str__()])
+        """Human readable information."""
+        return "\n".join([super().__repr__(), self.__str__()])
 
     def __str__(self):
-        return str(self.matcher) + ' = {}'.format(self.match_str)
+        """Human readable information."""
+        return f"{self.group!s} = {self.match_str}"
 
-    def get_match(self, parsed: bool = True):
+    def get_match(self, parse: bool = True) -> str | t.Any:
         """Get match string or value.
 
-        If `parsed` is true, and the parsing was successful, return the
-        parsed value instead of the matched string.
+        Parameters
+        ----------
+        parse:
+            If True (default), and the parsing was successful, return the
+            parsed value instead of the matched string.
+
+        Raises
+        ------
+        ValueError: Could not parse the match.
         """
-        if parsed and self.match_parsed is not None:
+        if parse:
+            if self.match_parsed is None:
+                raise ValueError(
+                    f"Failed to parse value '{self.match_str}' "
+                    f"for group '{self.group!s}'."
+                )
             return self.match_parsed
         return self.match_str
 
 
 class Matches:
-    """Store multiples matches.
+    """Scan an input file and store the results.
 
-    Attributes
+    Parameters
     ----------
-    matches: list of :class:`Match`
-        Matches for a single filename.
-    matchers: list of :class:`Matcher`
-        Matchers used.
+    match
+        Match object obtained from a filename. It should have as much capturing groups
+        as the pattern.
+    groups
+        Sequence of Groups objects present in the pattern.
 
-    Raises
-    ------
-    ValueError
-        Filename did not match pattern.
-    IndexError
-        Not as many matches as matchers.
     """
 
-    def __init__(self, matchers: List[Matcher], filename: str,
-                 pattern: re.Pattern):
-        self.matches = []
-        self.matchers = matchers
+    @classmethod
+    def from_filename(
+        cls, filename: str, pattern: re.Pattern | str, groups: abc.Sequence[Group]
+    ) -> "Matches | None":
+        """Find matches for a given filename.
+
+        Parameters
+        ----------
+        filename:
+            Filename to retrieve matches from.
+        pattern
+            Compiled match pattern to use. If left to None, we generate the current
+            regex.
+
+        Returns
+        -------
+        matches
+            A :class:`Matches` object, or None if the filename did not match.
 
+        Raises
+        ------
+        IndexError
+            Not as many matches as groups. Maybe one of the group regex contains an
+            additional (unwanted) capturing group ?
+        """
+        if isinstance(pattern, str):
+            pattern = re.compile(pattern)
         m = pattern.fullmatch(filename)
         if m is None:
-            raise ValueError("Filename did not match pattern.")
-        if len(m.groups()) != len(matchers):
-            raise IndexError("Not as many matches as matchers.")
+            return None
 
-        for i in range(len(matchers)):
-            self.matches.append(Match(matchers[i], m, i))
+        if len(groups) != len(m.groups()):
+            raise IndexError(
+                "Not as many captured matches as pattern groups. "
+                "Does one of the group regex contains a capturing group ?"
+            )
 
-    def __repr__(self):
-        return '\n'.join([super().__repr__(), self.__str__()])
+        return cls(m, groups)
 
-    def __str__(self):
-        return '\n'.join([str(m) for m in self.matches])
+    def __init__(self, match: re.Match, groups: abc.Sequence[Group]):
+        self.matches: list[Match] = []
+        """Matches for a single filename."""
+        self.groups = list(groups)
+        """Groups used."""
+
+        assert len(match.groups()) == len(groups)
+
+        for i in range(len(groups)):
+            self.matches.append(Match(groups[i], match, i))
+
+    def __repr__(self) -> str:
+        """Human readable information."""
+        return "\n".join([super().__repr__(), self.__str__()])
 
-    def __getitem__(self, key: Union[int, str]):
-        return self.get_matches(key)
+    def __str__(self) -> str:
+        """Human readable information."""
+        return "\n".join([str(m) for m in self.matches])
 
-    def __iter__(self):
+    def __getitem__(self, key: GroupKey) -> t.Any:
+        """Get first parsed value corresponding to key.
+
+        Ignore groups with the 'discard' option.
+        """
+        return self.get_value(key, parse=True, keep_discard=False)
+
+    def __iter__(self) -> abc.Iterator[Match]:
+        """Iterate over matches."""
         return iter(self.matches)
 
-    def __len__(self):
+    def __len__(self) -> int:
+        """Return number of matches."""
         return len(self.matches)
 
-    def get_matches(self, key: Union[int, str]) -> Union[Match, List[Match]]:
-        """Get matches corresponding to key.
+    def get_values(
+        self, key: GroupKey, parse: bool = True, keep_discard: bool = False
+    ) -> list[str | t.Any]:
+        """Get matched values corresponding to key.
+
+        Return a list of values, even if only one group is selected.
+
+        Parameters
+        ----------
+        key:
+            Group(s) to select, either by index or name.
+        parse:
+            If True (default), return the parsed value. If False return the
+            matched string.
+        keep_discard:
+            If true groups with the 'discard' option are kept. Defauult is false.
+        """
+        matches = self.get_matches(key, keep_discard=keep_discard)
+        values = [m.get_match(parse=parse) for m in matches]
+        return values
+
+    def get_value(
+        self, key: GroupKey, parse: bool = True, keep_discard: bool = False
+    ) -> str | t.Any:
+        """Get matched value corresponding to key.
+
+        Return a single value. If multiple groups correspond to ``key``,
+        the value of the first one to appear in the pattern is returned.
+
+        Parameters
+        ----------
+        key:
+            Group(s) to select, either by index or name.
+        parse:
+            If True (default), return the parsed value. If False return the
+            matched string.
+        keep_discard:
+            If true groups with the 'discard' option are kept. Defauult is false.
 
-        See :func:`Finder.get_matchers
-        <filefinder.finder.Finder.get_matchers>` for details on
-        `key` argument.
-        :func:`__getitem__` wraps around this method.
+        Raises
+        ------
+        KeyError: No group with no 'discard' option was found.
+        """
+        values = self.get_values(key, parse=parse, keep_discard=keep_discard)
+        if len(values) == 0:
+            raise KeyError(
+                "No group was found " f"(key: {key}, keep_discard: {keep_discard})"
+            )
+        if len(values) > 1:
+            if any(v != values[0] for v in values[1:]):
+                logger.warning(
+                    "Different parsed values for key %s (%s)", str(key), repr(values)
+                )
+        return values[0]
+
+    def get_matches(self, key: GroupKey, keep_discard: bool = False) -> list[Match]:
+        """Get Match objects corresponding to key.
+
+        Parameters
+        ----------
+        key:
+            Group(s) to select, either by index or name.
+        keep_discard:
+            If true groups with the 'discard' option are kept. Defauult is false.
 
         Returns
         -------
-        List of Match corresponding to the key. If only one Match corresponds,
-        return it directly.
+        List of Match corresponding to the key.
         """
-        selected = get_matchers_indices(self.matchers, key)
+        selected = get_groups_indices(self.groups, key)
         matches = [self.matches[k] for k in selected]
-        if len(matches) == 1:
-            return matches[0]
+        if not keep_discard:
+            matches = [m for m in matches if not m.group.discard]
         return matches
 
 
-def get_matchers_indices(matchers: List[Matcher],
-                         key: Union[int, str]) -> List[int]:
-    """Get list of matchers indices corresponding to key.
+def get_groups_indices(groups: list[Group], key: GroupKey) -> list[int]:
+    """Get sorted list of groups indices corresponding to key.
 
-    Key can be an integer index, or a string of the name, or a combination
-    of the group and the name with the syntax 'group:name'
+    Key can be an integer index, or a string of a group name. Since multiple
+    groups can share the same name, multiple indices can be returned (sorted).
 
     Raises
     ------
-    IndexError
-        No matcher found corresponding to the key
-    TypeError
-        Key is not int or str
+    IndexError: No group found corresponding to the key
+    TypeError: Key is not int or str
     """
     if isinstance(key, int):
         return [key]
     if isinstance(key, str):
-        k = key.split(':')
-        if len(k) == 1:
-            name, group = k[0], None
-        else:
-            group, name = k[:2]
-        selected = []
-        for i, m in enumerate(matchers):
-            if m.name == name and (group is None or group == m.group):
-                selected.append(i)
+        selected = [i for i, group in enumerate(groups) if group.name == key]
 
         if len(selected) == 0:
-            raise IndexError(f"No matcher found for key '{key}'")
+            raise IndexError(f"No group found for key '{key}'")
         return selected
 
     raise TypeError("Key must be int or str.")
```

### Comparing `filefinder-0.5.0/src/filefinder.egg-info/PKG-INFO` & `filefinder-1.0.0/src/filefinder.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,103 @@
 Metadata-Version: 2.1
 Name: filefinder
-Version: 0.5.0
+Version: 1.0.0
 Summary: Find files using a simple syntax.
-Home-page: https://github.com/Descanonge/filefinder
-Author: Clément Haëck
-Author-email: clement.haeck@posteo.net
+Author-email: Clément Haëck <clement.haeck@locean.ipsl.fr>
 Project-URL: Source, https://github.com/Descanonge/filefinder
 Project-URL: Documentation, https://filefinder.readthedocs.io
-Keywords: find files filename regular expression regex xarray
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: sphinx==6.2.1; extra == "dev"
+Requires-Dist: sphinx-book-theme==1.0.1; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: mypy>=1.5; extra == "dev"
+Requires-Dist: pytest>=7.4; extra == "dev"
+Requires-Dist: pyfakefs; extra == "dev"
+Requires-Dist: hypothesis; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
 
 
 # FileFinder
 
 > Find files using a simple syntax.
 
 <div align="left">
 
 [![PyPI](https://img.shields.io/pypi/v/filefinder)](https://pypi.org/project/filefinder)
 [![GitHub release](https://img.shields.io/github/v/release/Descanonge/filefinder)](https://github.com/Descanonge/filefinder/releases)
+[![codecov](https://codecov.io/github/Descanonge/filefinder/branch/master/graph/badge.svg?token=D5OBXX61HM)](https://codecov.io/github/Descanonge/filefinder)
+![test status](https://github.com/Descanonge/filefinder/actions/workflows/tests.yml/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/filefinder/badge/?version=latest)](https://filefinder.readthedocs.io/en/latest/?badge=latest)
 
 </div>
 
-To find files, FileFinder allows to specify the structure of filenames with a simple syntax.
-Parts of the file structure varying from file to file can be indicated with format strings
-or regular expressions, or with pre-defined defaults (mainly for dates).
-Once setup, it can:
+FileFinder allows to specify the structure of filenames using a simple syntax.
+Parts of the file structure varying from file to file are indicated within named
+groups, either with format strings or regular expressions (with some pre-defined
+values for some names). Once setup, it can:
 
-- Find corresponding files in a directory
-- Parse information from the filenames
+- Find corresponding files in a directory (and sub-directories)
+- Parse values from the filenames
 - Select only filenames with specific values
 - Generate filenames
 
-The package also interface easily with `xarray.open_mfdataset`.
-
 ## Quick examples
 
-The following example will find all files with the structure ``Data/[month]/Temperature_[depth]_[date].nc``:
+The following example will find all files with the structure ``Data/param_[parameter]/Temperature_[date].nc``:
 ``` python
-finder = Finder('/.../Data', '%(m)/Temperature_%(depth:fmt=03d)_%(Y)%(m)%(d).nc')
+finder = Finder('/.../Data', 'param_%(parameter:fmt=.1f)/%(Y)/Temperature_%(Y)%(m)%(d).nc')
 files = finder.get_files()
 ```
 
-We can also select only some files, for instance the first day of each month:
+We can also select only some files, for instance only in january:
 ``` python
-finder.fix_matcher('d', 1)
-files = finder.get_files()
+    finder.fix_group('m', 1)
+    files = finder.get_files()
 ```
 
 We can retrieve values from found files:
 ``` python
-filename, matches = finder.files[0]
-depth = matches['depth'].get_match()
-date = filefinder.library.get_date(matches)
+    filename, matches = finder.files[0]
+    parameter = matches["parameter"]
+    # the date as a datetime object
+    date = filefinder.library.get_date(matches)
 ```
 
 And we can generate a filename with a set of parameters:
 ``` python
-finder.get_filename(depth=100, Y=2000, m=1, d=1)
-# Specifying the day is optional since we already fixed it to 1.
+    finder.make_filename(parameter=0.5, Y=2000, m=1, d=1)
+    # Specifying the month is optional since we already fixed it to 1.
 ```
 
-
 ## Requirements
 
-Python >= 3.7.
+Python >= 3.10
 
 ## Installation
 
 From pip:
 ``` sh
 pip install filefinder
 ```
 
 From source:
 ``` sh
-git clone https://github.com/Descanonge/filefinder.git
-cd filefinder
-pip install -e .
+pip install -e https://github.com/Descanonge/filefinder.git#egg=filefinder
 ```
 
 ## Documentation
 
 Documentation is available at [filefinder.readthedocs.io](https://filefinder.readthedocs.io).
```

