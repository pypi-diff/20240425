# Comparing `tmp/git_smudge-0.0.8.tar.gz` & `tmp/git_smudge-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_smudge-0.0.8.tar", last modified: Mon Nov 14 00:19:00 2022, max compression
+gzip compressed data, was "git_smudge-0.0.9.tar", last modified: Mon Nov 14 07:00:41 2022, max compression
```

## Comparing `git_smudge-0.0.8.tar` & `git_smudge-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 ktpanda   (1000) ktpanda   (1000)        0 2022-11-14 00:19:00.028113 git_smudge-0.0.8/
--rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)     3834 2022-11-14 00:18:58.000000 git_smudge-0.0.8/CHANGELOG.md
--rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)     1074 2022-11-12 19:10:30.000000 git_smudge-0.0.8/LICENSE
--rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)       56 2022-11-12 19:10:30.000000 git_smudge-0.0.8/MANIFEST.in
--rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)     3027 2022-11-14 00:19:00.028113 git_smudge-0.0.8/PKG-INFO
--rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)     3887 2022-11-14 00:16:43.000000 git_smudge-0.0.8/README.html
--rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)     2496 2022-11-14 00:16:34.000000 git_smudge-0.0.8/README.md
--rwxrwxr-x   0 ktpanda   (1000) ktpanda   (1000)      952 2022-11-12 19:10:30.000000 git_smudge-0.0.8/gendoc
-drwxrwxr-x   0 ktpanda   (1000) ktpanda   (1000)        0 2022-11-14 00:19:00.024113 git_smudge-0.0.8/git_smudge/
--rw-------   0 ktpanda   (1000) ktpanda   (1000)    17129 2022-11-14 00:18:57.000000 git_smudge-0.0.8/git_smudge/__init__.py
--rwx------   0 ktpanda   (1000) ktpanda   (1000)     7261 2022-11-14 00:17:56.000000 git_smudge-0.0.8/git_smudge/__main__.py
--rw-------   0 ktpanda   (1000) ktpanda   (1000)    17818 2022-11-13 23:34:30.000000 git_smudge-0.0.8/git_smudge/config.py
--rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)     6911 2022-11-13 23:44:32.000000 git_smudge-0.0.8/git_smudge/filters.py
--rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)      386 2022-11-13 09:09:51.000000 git_smudge-0.0.8/git_smudge/runfilter.py
--rwxrwxr-x   0 ktpanda   (1000) ktpanda   (1000)    10879 2022-11-14 00:18:46.000000 git_smudge-0.0.8/git_smudge/tests.py
-drwxrwxr-x   0 ktpanda   (1000) ktpanda   (1000)        0 2022-11-14 00:19:00.028113 git_smudge-0.0.8/git_smudge.egg-info/
--rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)     3027 2022-11-14 00:19:00.000000 git_smudge-0.0.8/git_smudge.egg-info/PKG-INFO
--rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)      425 2022-11-14 00:19:00.000000 git_smudge-0.0.8/git_smudge.egg-info/SOURCES.txt
--rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)        1 2022-11-14 00:19:00.000000 git_smudge-0.0.8/git_smudge.egg-info/dependency_links.txt
--rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)       56 2022-11-14 00:19:00.000000 git_smudge-0.0.8/git_smudge.egg-info/entry_points.txt
--rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)       84 2022-11-14 00:19:00.000000 git_smudge-0.0.8/git_smudge.egg-info/requires.txt
--rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)       11 2022-11-14 00:19:00.000000 git_smudge-0.0.8/git_smudge.egg-info/top_level.txt
--rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)       94 2022-11-12 19:10:30.000000 git_smudge-0.0.8/pyproject.toml
--rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)      801 2022-11-14 00:19:00.028113 git_smudge-0.0.8/setup.cfg
+drwxrwxr-x   0 ktpanda   (1000) ktpanda   (1000)        0 2022-11-14 07:00:41.841548 git_smudge-0.0.9/
+-rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)     5037 2022-11-14 07:00:38.000000 git_smudge-0.0.9/CHANGELOG.md
+-rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)     1074 2022-11-12 19:10:30.000000 git_smudge-0.0.9/LICENSE
+-rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)       56 2022-11-12 19:10:30.000000 git_smudge-0.0.9/MANIFEST.in
+-rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)     3027 2022-11-14 07:00:41.841548 git_smudge-0.0.9/PKG-INFO
+-rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)     3887 2022-11-14 00:16:43.000000 git_smudge-0.0.9/README.html
+-rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)     2496 2022-11-14 00:16:34.000000 git_smudge-0.0.9/README.md
+-rwxrwxr-x   0 ktpanda   (1000) ktpanda   (1000)      952 2022-11-12 19:10:30.000000 git_smudge-0.0.9/gendoc
+drwxrwxr-x   0 ktpanda   (1000) ktpanda   (1000)        0 2022-11-14 07:00:41.841548 git_smudge-0.0.9/git_smudge/
+-rw-------   0 ktpanda   (1000) ktpanda   (1000)    17550 2022-11-14 07:00:23.000000 git_smudge-0.0.9/git_smudge/__init__.py
+-rwx------   0 ktpanda   (1000) ktpanda   (1000)     7261 2022-11-14 00:17:56.000000 git_smudge-0.0.9/git_smudge/__main__.py
+-rw-------   0 ktpanda   (1000) ktpanda   (1000)    18450 2022-11-14 06:23:09.000000 git_smudge-0.0.9/git_smudge/config.py
+-rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)     6983 2022-11-14 04:02:42.000000 git_smudge-0.0.9/git_smudge/filters.py
+-rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)      386 2022-11-13 09:09:51.000000 git_smudge-0.0.9/git_smudge/runfilter.py
+-rwxrwxr-x   0 ktpanda   (1000) ktpanda   (1000)    17248 2022-11-14 06:57:17.000000 git_smudge-0.0.9/git_smudge/tests.py
+drwxrwxr-x   0 ktpanda   (1000) ktpanda   (1000)        0 2022-11-14 07:00:41.841548 git_smudge-0.0.9/git_smudge.egg-info/
+-rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)     3027 2022-11-14 07:00:41.000000 git_smudge-0.0.9/git_smudge.egg-info/PKG-INFO
+-rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)      425 2022-11-14 07:00:41.000000 git_smudge-0.0.9/git_smudge.egg-info/SOURCES.txt
+-rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)        1 2022-11-14 07:00:41.000000 git_smudge-0.0.9/git_smudge.egg-info/dependency_links.txt
+-rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)       56 2022-11-14 07:00:41.000000 git_smudge-0.0.9/git_smudge.egg-info/entry_points.txt
+-rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)       84 2022-11-14 07:00:41.000000 git_smudge-0.0.9/git_smudge.egg-info/requires.txt
+-rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)       11 2022-11-14 07:00:41.000000 git_smudge-0.0.9/git_smudge.egg-info/top_level.txt
+-rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)       94 2022-11-12 19:10:30.000000 git_smudge-0.0.9/pyproject.toml
+-rw-rw-r--   0 ktpanda   (1000) ktpanda   (1000)      801 2022-11-14 07:00:41.841548 git_smudge-0.0.9/setup.cfg
```

### Comparing `git_smudge-0.0.8/CHANGELOG.md` & `git_smudge-0.0.9/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+[Version 0.0.9 (2022-11-14)](https://pypi.org/project/git_smudge/0.0.9/)
+============================
+
+* Add integration test which creates actual repository ([ece41c7](https://gitlab.com/ktpanda/git_smudge/-/commit/ece41c723be9a7c8fa76fdadf82fe1c4f633e326))
+* Add filter name and index to marker text ([7141f06](https://gitlab.com/ktpanda/git_smudge/-/commit/7141f06ff679d2d57d3743e5b8e85c64620202cb))
+* Do more preprocessing when loading TOML config ([8e3dabd](https://gitlab.com/ktpanda/git_smudge/-/commit/8e3dabd2eea62f94155cc07b49834151a12f0b0e))
+* Run `git update-index` on changed files after running `git smudge clean` or `git smudge apply` ([0ab492c](https://gitlab.com/ktpanda/git_smudge/-/commit/0ab492c91bab730f11f9f1c9c9e3c3beda2983d6))
+* Don't warn of changed config unless config file is at least 2 seconds newer than the working config ([ec13858](https://gitlab.com/ktpanda/git_smudge/-/commit/ec13858b0e0c5c04c46a9369d6cd1d5d8d207b8d))
+  * This mitigates the issue where it would warn right after doing `git smudge setup`
+* Restore behavior of running `clean` on idempotent filters ([308a06a](https://gitlab.com/ktpanda/git_smudge/-/commit/308a06a4132ee7c183cf5740e4ee80caac8f0a2c))
+
+
 [Version 0.0.8 (2022-11-13)](https://pypi.org/project/git_smudge/0.0.8/)
 ============================
 
 * Add auto-installation of bash completion scripts ([1fa8b20](https://gitlab.com/ktpanda/git_smudge/-/commit/1fa8b20174a75710f77311e89859403d422cfc38))
 * Fix bug with clean and apply not using new checked methods ([8e5c39a](https://gitlab.com/ktpanda/git_smudge/-/commit/8e5c39a198d2eeab9641e205fde3fa9034116a5d))
```

### Comparing `git_smudge-0.0.8/LICENSE` & `git_smudge-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `git_smudge-0.0.8/PKG-INFO` & `git_smudge-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git_smudge
-Version: 0.0.8
+Version: 0.0.9
 Summary: A powerful filter driver for Git which can automatically apply local changes to the working tree of a repository
 Home-page: https://ktpanda.org/software/git_smudge
 Author: Katie Rust
 Author-email: katie@ktpanda.org
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `git_smudge-0.0.8/README.html` & `git_smudge-0.0.9/README.html`

 * *Files identical despite different names*

### Comparing `git_smudge-0.0.8/README.md` & `git_smudge-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `git_smudge-0.0.8/gendoc` & `git_smudge-0.0.9/gendoc`

 * *Files identical despite different names*

### Comparing `git_smudge-0.0.8/git_smudge/__init__.py` & `git_smudge-0.0.9/git_smudge/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from pathlib import Path
 
 import argcomplete
 
 proc_log = logging.getLogger('git-process')
 filt_log = logging.getLogger('filters')
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 
 MAX_PACKET_CONTENT_SIZE = 65516
 BOM = '\ufeff'
 DEBUG = False
 
 # Line comments
 COMMENT_HASH = '# ', ''
@@ -306,48 +306,61 @@
             self.changed = True
             return True
         return False
 
     def _smudge_check(self, filter):
         '''Run `smudge`, checking that `clean` properly restores the content'''
         if not filter.config.get('smudge_check_clean', True):
-            filter.smudge(content)
+            filter.smudge(self)
             return
 
         new_content = self.copy()
         filter.smudge(new_content)
 
         check_content = new_content.copy()
         check_content.is_smudged = True
         filter.clean(check_content)
+        #filt_log.debug('orig:  %r', self.text_data)
+        #filt_log.debug('new:   %r', new_content.text_data)
+        #filt_log.debug('clean: %r', check_content.text_data)
         if check_content == self:
             self.set_from(new_content)
             self.changed |= new_content.changed
         else:
             filt_log.warning(
                 '%s: applying filter %r results in text that '
                 'does not restore properly',
                 self.path, filter)
 
     def smudge(self, filters):
+        # Reverse any idempotent filters
+        self.is_smudged = False
+
+        for filter in reversed(filters):
+            filter.clean(self)
+
         for filter in filters:
             self._smudge_check(filter)
 
         self.is_smudged = True
 
     def clean(self, filters):
+        self.is_smudged = True
+
         for filter in reversed(filters):
             filter.clean(self)
 
         self.is_smudged = False
 
 class GitFilter:
     args = None
 
-    def __init__(self, config=None, **kw):
+    def __init__(self, config=None, name='', index=0, **kw):
+        self.name = name
+        self.index = index
         if config is None:
             config = {}
         self.config = config
         if kw:
             config.update(kw)
 
     def _set_from_config(self, **kw):
```

### Comparing `git_smudge-0.0.8/git_smudge/__main__.py` & `git_smudge-0.0.9/git_smudge/__main__.py`

 * *Files identical despite different names*

### Comparing `git_smudge-0.0.8/git_smudge/config.py` & `git_smudge-0.0.9/git_smudge/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,56 +98,87 @@
         super().__init__()
         self.factory = factory
 
     def __missing__(self, key):
         r = self[key] = self.factory(key)
         return r
 
-def run_git(cmd, check=True):
+def run_git(cmd, check=True, **kw):
     return subprocess.run(
         ['git'] + cmd, stdout=subprocess.PIPE, check=check,
-        encoding='utf8', errors='surrogateescape')
+        encoding='utf8', errors='surrogateescape', **kw)
 
 def git_path(relpath) -> Path:
     '''Return a `Path` object pointing to a file within the .git directory'''
     return Path(run_git(['rev-parse', '--git-path', relpath]).stdout.rstrip('\n'))
 
-def _filter_list_json(lst):
-    rtn = [(filt if isinstance(filt, str) else filt.config) for filt in lst]
-    return rtn[0] if len(rtn) == 1 else rtn
-
 def item_or_list(val):
     return val if isinstance(val, list) else [val]
 
+def _build_filter_list(filter_list, obj):
+    if isinstance(obj, dict):
+        sub_filters = obj.get('filters')
+        if sub_filters:
+            _build_filter_list(filter_list, sub_filters)
+
+        if obj.get('type'):
+            filter_list.append(obj)
+
+    elif isinstance(obj, list):
+        for part in obj:
+            _build_filter_list(filter_list, part)
+
+    elif isinstance(obj, str):
+        filter_list.append(obj)
+    else:
+        raise TypeError(f'Invalid value in filter list: {obj!r}')
+
+def _resolve_references(named_filters, input_list, output_list):
+    for val in input_list:
+        if isinstance(val, str):
+            sub_list = named_filters[val]
+            if sub_list is None:
+                raise ValueError(f'Reference loop detected in filters: {val}')
+
+            # Temporarily remove the referenced list to detect loops
+            named_filters[val] = None
+            _resolve_references(named_filters, sub_list, output_list)
+            named_filters[val] = sub_list
+        else:
+            output_list.append(val)
+
 class Pattern:
     def __init__(self, pat):
         self.dir_pattern, self.file_pattern = pat
         self.include_rules = []
         self.exclude_rules = []
 
 class FilterConfig:
     def __init__(self, root):
         self.root = root
         self.filter_classes = {}
         self.named_filters = {}
-        self.rule_patterns = {}
+        self.patterns = []
 
     @classmethod
     def load_toml(cls, tomlpath, worktree, gitdir):
         try:
             with tomlpath.open('rb') as fp:
                 root = tomllib.load(fp)
         except FileNotFoundError:
             root = {}
 
         plugin_content = []
+        patterns = CacheDict(lambda k: [[], []])
+        filters = {}
+
         new_root = {
             'plugins': plugin_content,
-            'filters': root.get('filters', {}),
-            'rule': root.get('rule', [])
+            'filters': filters,
+            'patterns': patterns
         }
 
         for obj in root.get('plugins', ()):
             # support both `plugins = [ ... ]` and [[plugins]] path = ...
             if isinstance(obj, str):
                 obj = { 'path': obj }
             path = obj['path']
@@ -162,14 +193,52 @@
             else:
                 script_path = worktree / path
 
             log.debug('Loading plugin %s', script_path)
             content = FileContent(script_path, script_path.read_bytes())
             plugin_content.append({'path': str(script_path), 'content': content.get_text().split('\n')})
 
+        filter_rules = CacheDict(lambda k: [])
+        for rule in root.get('rule', ()):
+            files = item_or_list(rule.get('files', []))
+            for filter in item_or_list(rule.get('filters', [])):
+                filter_rules[filter].extend(files)
+
+        for name, obj in root.get('filters', {}).items():
+            filter_list = []
+            _build_filter_list(filter_list, obj)
+            filters[name] = filter_list
+
+
+            files = item_or_list(obj.get('files', []))
+            files.extend(filter_rules[name])
+
+            for pattern in files:
+                if exclude := pattern.startswith('!'):
+                    pattern = pattern[1:]
+
+                # If there is no '/' in the rule, then it applies to the filename only
+                dirpart, sep, filepart = pattern.rpartition('/')
+                if sep:
+                    dirpart = dirpart.lstrip('/')
+                else:
+                    dirpart = '*'
+
+                key = dirpart + '/' + filepart
+                if exclude:
+                    patterns[key][1].append(name)
+                else:
+                    patterns[key][0].append(name)
+
+        for name, obj in filters.items():
+            filters[name] = None
+            output_list = []
+            _resolve_references(filters, obj, output_list)
+            filters[name] = output_list
+
         return cls(new_root)
 
     @classmethod
     def load_json(cls, jsonpath):
         root = load_json(jsonpath)
         if root is None:
             return cls({})
@@ -194,128 +263,62 @@
                         and issubclass(value, GitFilter)
                         and value is not GitFilter):
                         log.debug('Adding filter class %s', value)
                         self.add_filter_class(value)
             except Exception as ex:
                 raise ValueError(f'Failed to load plugin {obj["path"]} (see attached exception)') from ex
 
-        filter_rules = CacheDict(lambda k: [])
-        for rule in self.root.get('rule', ()):
-            files = item_or_list(rule.get('files', []))
-            for filter in item_or_list(rule.get('filters', [])):
-                filter_rules[filter].extend(files)
-
-        patterns = self.rule_patterns = CacheDict(Pattern)
-        filters = self.named_filters = {}
-        for name, obj in self.root.get('filters', {}).items():
-            filters[name] = self.build_filter_list(obj)
-
-            files = item_or_list(obj.get('files', []))
-            files.extend(filter_rules[name])
-            for pattern in files:
-                if exclude := pattern.startswith('!'):
-                    pattern = pattern[1:]
-
-                # If there is no '/' in the rule, then it applies to the filename only
-                dirpart, sep, filepart = pattern.rpartition('/')
-                if sep:
-                    dirpart = dirpart.lstrip('/')
-                else:
-                    dirpart = '*'
-
-                if exclude:
-                    patterns[dirpart, filepart].exclude_rules.append(name)
-                else:
-                    patterns[dirpart, filepart].include_rules.append(name)
-
-        for name, filter_list in filters.items():
-            self._resolve_references(filter_list)
+        self.named_filters = filters = {}
+        for name, filter_list in self.root.get('filters', {}).items():
+            filters[name] = new_filter_list = []
+            for index, obj in enumerate(filter_list):
+                filter_type = obj['type']
+                cls = self.filter_classes[filter_type.lower()]
+                filter = cls(obj, name, index)
+                filter.update_config()
+                new_filter_list.append(filter)
+
+        patterns = self.patterns = []
+        for key, (include, exclude) in self.root.get('patterns', {}).items():
+            dirpart, _, filepart = key.rpartition('/')
+            patterns.append((dirpart, filepart, include, exclude))
 
     def add_filter_class(self, cls):
         name = cls.__name__
         if name.endswith('Filter'):
             name = name[:-6]
         #log.debug('Adding filter class %s as %s', cls, name.lower())
         self.filter_classes[name.lower()] = cls
 
     def get_filters_for_path(self, path):
-        # Make sure path starts with exactly one slash
         dirpart, _, filepart = path.rpartition('/')
 
-        include_rules = set()
-        exclude_rules = set()
-        for pat in self.rule_patterns.values():
-            if (fnmatch.fnmatch(dirpart, pat.dir_pattern) and
-                fnmatch.fnmatch(filepart, pat.file_pattern)):
-                log.debug('%s: matches %s/%s', path, pat.dir_pattern, pat.file_pattern)
-                include_rules.update(pat.include_rules)
-                exclude_rules.update(pat.exclude_rules)
+        include_filters = set()
+        exclude_filters = set()
+        for dir_pattern, file_pattern, include, exclude in self.patterns:
+            if (fnmatch.fnmatch(dirpart, dir_pattern) and
+                fnmatch.fnmatch(filepart, file_pattern)):
+
+                log.debug('%s: matches %s/%s', path, dir_pattern, file_pattern)
+                include_filters.update(include)
+                exclude_filters.update(exclude)
 
-        include_rules -= exclude_rules
-        if not include_rules:
+        include_filters -= exclude_filters
+        if not include_filters:
             log.debug('%s: no filters matched', path)
             return []
 
         rtnlist = []
         for name, filter_list in self.named_filters.items():
-            if name in include_rules:
+            if name in include_filters:
                 rtnlist.extend(filter_list)
 
         log.debug('Filters for %s: %r', path, rtnlist)
         return rtnlist
 
-    def _resolve_references(self, filter_list):
-        while True:
-            next_filters = []
-            have_references = False
-            for filt in filter_list:
-                if isinstance(filt, str):
-                    next_filters.extend(self.named_filters[filt])
-                    have_references = True
-                else:
-                    next_filters.append(filt)
-
-                if len(next_filters) > MAX_FILTER_LIST:
-                    raise ValueError(f'Too many filters in list ({len(next_filters)})')
-
-            if not have_references:
-                return
-
-            filter_list[:] = next_filters
-
-    def build_filter(self, obj):
-        type = obj['type']
-        cls = self.filter_classes[type.lower()]
-        filter = cls(obj)
-        filter.update_config()
-        return filter
-
-    def _build_filter_list(self, filter_list, obj):
-        if isinstance(obj, dict):
-            sub_filters = obj.get('filters')
-            if sub_filters:
-                self._build_filter_list(filter_list, sub_filters)
-
-            if obj.get('type'):
-                filter_list.append(self.build_filter(obj))
-
-        elif isinstance(obj, list):
-            for part in obj:
-                self._build_filter_list(filter_list, part)
-
-        elif isinstance(obj, str):
-            filter_list.append(obj)
-        else:
-            raise TypeError(f'Invalid value in filter list: {obj!r}')
-
-    def build_filter_list(self, obj):
-        filter_list = []
-        self._build_filter_list(filter_list, obj)
-        return filter_list
-
 class Config:
     def __init__(self, worktree, git_dir, git_common_dir=None, config_path=None):
         self.worktree = worktree
         self.git_dir = git_dir
         self.git_common_dir = git_common_dir or git_dir
 
         self.working_config = None
@@ -343,15 +346,15 @@
         try:
             wt_mtime = self.working_config_path.stat().st_mtime
         except FileNotFoundError:
             wt_mtime = 0
 
         try:
             config_mtime = self.config_path.stat().st_mtime
-            if config_mtime > wt_mtime:
+            if (config_mtime - wt_mtime) > 2:
                 return True
         except FileNotFoundError:
             pass
 
         return False
 
     def warn_config_newer(self):
@@ -368,15 +371,15 @@
         new_root = {
             'note': [
                 "DO NOT EDIT THIS FILE. EDIT git-smudge.toml, THEN RUN",
                 "`git smudge apply` TO APPLY CONFIGURATION CHANGES"
             ],
             'plugins': root.get('plugins', []),
             'filters': root.get('filters', {}),
-            'rule': root.get('rule', [])
+            'patterns': root.get('patterns', {})
         }
         save_json(self.working_config_path, new_root)
 
     def load_new(self):
         self.new_config = FilterConfig.load_toml(
             self.config_path, self.worktree, self.git_common_dir)
         self.new_config.load()
@@ -393,25 +396,29 @@
 
         if not update_files:
             self.save_json(self.new_config.root)
             return
 
         # Get a list of all files tracked in the repository. `git ls-files -z` will spit
         # out a NUL-separated list.
-        repo_files = run_git(['ls-files', '-z']).stdout.split('\0')
+        repo_files = run_git(['ls-files', '--stage', '-z']).stdout.split('\0')
 
         # If there are no files, or there was a terminating NUL, there will be a blank
         # item at the end
         if repo_files[-1] == '':
             repo_files.pop()
 
+        update_index_data = []
+
         change_count = 0
         written_files = []
         try:
-            for path in repo_files:
+            for entry in repo_files:
+                path = entry.split('\t', 1)[-1]
+
                 # Run the file through the `clean` method of the old filters, then the
                 # `smudge` method of the new filters.
                 old_filters = self.working_config.get_filters_for_path(path)
                 new_filters = self.new_config.get_filters_for_path(path)
                 if old_filters or new_filters:
                     fpath = self.worktree / path
 
@@ -423,14 +430,15 @@
                     content.smudge(new_filters)
 
                     if content.changed:
                         new_data = content.get_binary()
                         if new_data != prev_data:
                             change_count += 1
                             log.info('apply: Content of %s has changed', path)
+                            update_index_data.append(entry + '\0')
                             tf = tempfile.NamedTemporaryFile(
                                 dir=str(fpath.parent), prefix=fpath.name,
                                 suffix='.smudge-apply-temp', delete=False, mode='wb')
                             written_files.append((fpath, tf.name))
                             with tf:
                                 tf.write(new_data)
 
@@ -453,14 +461,19 @@
             for path, temppath in to_replace:
                 try:
                     os.replace(temppath, path)
                 except OSError as e:
                     log.error('Could not apply new content to %s: %s', path, e)
                     log.error('Keeping temporary file %s.', temppath)
 
+            # Have git stat() all the files we've changed so it doesn't automatically
+            # assume they have been "modified" just because th
+            if update_index_data:
+                run_git(['update-index', '-z', '--index-info'], input=''.join(update_index_data))
+
             log.info('git-smudge configuration updated for %s, %d files changed',
                      self.worktree, change_count)
 
         finally:
             for path, temppath in written_files:
                 try:
                     os.unlink(temppath)
@@ -474,14 +487,17 @@
         entry to `.git/info/attributes, and create an empty '''
         if not self.config_path.exists():
             self.config_path.write_text(CONFIG_TEMPLATE, encoding='ascii')
             print(f'Created template configuration in {self.config_path.absolute()}')
         else:
             print(f'Configuration {self.config_path.absolute()} already exists')
 
+        if not self.working_config_path.exists():
+            self.save_json({})
+
         exe_esc = sys.executable.replace("'", r"'\''")
         cmd = f"'{exe_esc}' -m git_smudge.runfilter"
         run_git(['config', 'filter.git-smudge.process', cmd])
 
         attributes = git_path('info/attributes')
         try:
             attribute_data = attributes.read_bytes()
```

### Comparing `git_smudge-0.0.8/git_smudge/filters.py` & `git_smudge-0.0.9/git_smudge/filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,16 +74,16 @@
             if insert[-1] == '':
                 insert.pop()
 
         self.lines = insert
 
         self.comment_style = comment_style
         self.block = block if block is not None else len(self.lines) > 1
-        self.marker_text = marker_text
-        self.marker_esc = re.escape(marker_text)
+        self.marker_text = f'{marker_text}.{self.name}[{self.index}]'
+        self.marker_esc = re.escape(self.marker_text)
 
         if isinstance(after, str):
             after = re.compile(after)
 
         self.insert_after = after
 
     def clean(self, content):
@@ -130,16 +130,16 @@
         new_text.append(post_text)
         content.set_text(''.join(new_text))
 
 class CommentOutFilter(GitFilter):
     def _set_from_config(self, /, match, marker_text='SMUDGE CommentOutFilter',
                         comment_style='auto', count=None, **kw):
         super()._set_from_config(**kw)
-        self.marker_text = marker_text
-        self.marker_esc = re.escape(marker_text)
+        self.marker_text = f'{marker_text}.{self.name}[{self.index}]'
+        self.marker_esc = re.escape(self.marker_text)
         self.count = count
         self.comment_style = comment_style
 
         if isinstance(match, str):
             match = re.compile(match, re.S)
 
         self.match = match
```

### Comparing `git_smudge-0.0.8/git_smudge/tests.py` & `git_smudge-0.0.9/git_smudge/tests.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 #!/usr/bin/python3
+import sys
 import re
+import os
 import argparse
 import unittest
 import tempfile
 import shutil
+import subprocess
 import logging
 from pathlib import Path
 
 import git_smudge
 import git_smudge.__main__
 from git_smudge import config, filters
 
@@ -15,31 +18,31 @@
 
 def build_clean_text(pre_text, indent, match_part, post_text, **kw):
     return pre_text + indent + match_part + post_text
 
 def build_insert_test_smudge_block(pre_text, indent, match_part, post_text, lines, comment, **kw):
     return (
         f'{pre_text}{indent}{match_part}'
-        f'\n{indent}{comment[0]}BEGIN SMUDGE InsertLineFilter{comment[1]}'
+        f'\n{indent}{comment[0]}BEGIN SMUDGE InsertLineFilter.test[0]{comment[1]}'
         + ''.join(f'\n{indent}{line}' for line in lines) +
-        f'\n{indent}{comment[0]}END SMUDGE InsertLineFilter{comment[1]}'
+        f'\n{indent}{comment[0]}END SMUDGE InsertLineFilter.test[0]{comment[1]}'
         f'{post_text}'
     )
 def build_insert_test_smudge_line(pre_text, indent, match_part, post_text, lines, comment, **kw):
     return (
         f'{pre_text}{indent}{match_part}'
-        + ''.join(f'\n{indent}{line} {comment[0]}LINE SMUDGE InsertLineFilter{comment[1]}' for line in lines) +
+        + ''.join(f'\n{indent}{line} {comment[0]}LINE SMUDGE InsertLineFilter.test[0]{comment[1]}' for line in lines) +
         f'{post_text}'
     )
 
 def build_comment_out_text(pre_text, indent, match_part, post_text, comment, **kw):
     text = []
     for line in (indent + match_part).split('\n'):
         split_pos = len(indent) if line.startswith(indent) else 0
-        text.append(f'{line[:split_pos]}{comment[0]}SMUDGE CommentOutFilter [{line[split_pos:]}]{comment[1]}')
+        text.append(f'{line[:split_pos]}{comment[0]}SMUDGE CommentOutFilter.test[0] [{line[split_pos:]}]{comment[1]}')
     return pre_text + '\n'.join(text) + post_text
 
 
 TEST_LINES = [
     'insert test line 1',
     '    insert test with leading space',
     'insert test with trailing space ',
@@ -62,74 +65,196 @@
                 INSERT_TESTS.append({
                     'pre_text': pre_text,
                     'indent': indent,
                     'match_part': match_part,
                     'post_text': post_text,
                 })
 
+TEST_CONTENT_C = '''
+void test() {
+\tfilter1();
+
+\tprintf("filter2\\n");
+
+\ttest("filter3");
+}
+'''
+
+TEST_CONTENT_PY = r'''
+def root():
+    filter1()
+
+    print("filter2")
+
+    test_comment("filter3")
+'''
+
+TEST_CONTENT_TXT = r'''
+test filter1
+
+test filter2
+
+test filter3
+'''
+
+SMUDGE_CONTENT_C_1 = '''
+void test() {
+\tfilter1();
+\t// BEGIN SMUDGE InsertLineFilter.filter1[0]
+\txfilt1_1
+\txfilt1_2
+\t// END SMUDGE InsertLineFilter.filter1[0]
+
+\tprintf("filter2\\n");
+
+\ttest("filter3");
+}
+'''
+
+SMUDGE_CONTENT_C_2 = '''\
+test smudge
+
+void test() {
+\tfilter1();
+
+\tprintf("filter2\\n");
+
+\ttest("filter3");
+}
+'''
+
+SMUDGE_CONTENT_C_3 = '''
+void test() {
+\tfilter1();
+\t// SMUDGE CommentOutFilter.filter2[2] [// BEGIN SMUDGE InsertLineFilter.filter2[1]]
+\txfilt1_1
+\txfilt1_2
+\t// SMUDGE CommentOutFilter.filter2[2] [// END SMUDGE InsertLineFilter.filter2[1]]
+\t// BEGIN SMUDGE InsertLineFilter.filter1[0]
+\txfilt1_1
+\txfilt1_2
+\t// END SMUDGE InsertLineFilter.filter1[0]
+
+\t// SMUDGE CommentOutFilter.filter2[2] [printf("filter2\\n");]
+
+\ttest("xfilt3");
+}
+'''
+
+SMUDGE_CONTENT_C_4 = '''\
+test smudge
+
+void test() {
+\tfilter1();
+\t// SMUDGE CommentOutFilter.filter2[2] [// BEGIN SMUDGE InsertLineFilter.filter2[1]]
+\txfilt1_1
+\txfilt1_2
+\t// SMUDGE CommentOutFilter.filter2[2] [// END SMUDGE InsertLineFilter.filter2[1]]
+
+\t// SMUDGE CommentOutFilter.filter2[2] [printf("filter2\\n");]
+
+\ttest("xfilt3");
+}
+'''
+
+SMUDGE_CONTENT_C_5 = '''
+void test() {
+\tfilter1();
+\t// BEGIN SMUDGE InsertLineFilter.filter3[1]
+\txfilt1_1
+\txfilt1_2
+\t// END SMUDGE InsertLineFilter.filter3[1]
+
+\tprintf("filter2\\n");
+
+\ttest("xfilt3");
+}
+'''
+
+SMUDGE_CONTENT_PY_1 = '''
+def boot():
+    filter1()
+
+    print("filter2")
+
+    test_comment("filter3")
+'''
+
+SMUDGE_CONTENT_PY_2 = '''
+def root():
+    filter1()
+    # SMUDGE CommentOutFilter.filter2[2] [# BEGIN SMUDGE InsertLineFilter.filter2[1]]
+    xfilt1_1
+    xfilt1_2
+    # SMUDGE CommentOutFilter.filter2[2] [# END SMUDGE InsertLineFilter.filter2[1]]
+
+    # SMUDGE CommentOutFilter.filter2[2] [print("filter2")]
+
+    test_comment("xfilt3")
+'''
+
 CONFIG_TEST_PATHS = [
-    ('root.txt', []),
-    ('root.c', [
-        ('SimpleFilter', 'search', 'filter1')
+    ('root.txt', TEST_CONTENT_TXT, TEST_CONTENT_TXT, []),
+    ('root.c', TEST_CONTENT_C, SMUDGE_CONTENT_C_1, [
+        ('InsertLineFilter', 'after', 'filter1'),
     ]),
-    ('foo.c', [
+    ('foo.c', TEST_CONTENT_C, SMUDGE_CONTENT_C_2, [
         ('TestFilter', 'test', '1234')
     ]),
-    ('root.py', [
+    ('root.py', TEST_CONTENT_PY, SMUDGE_CONTENT_PY_1, [
         ('SimpleFilter', 'search', 'root')
     ]),
-    ('subdir/test.c', [
-        ('SimpleFilter', 'search', 'filter1'),
-        ('CommentOutFilter', 'match', 'filter3'),
-        ('SimpleFilter', 'search', 'filter1'),
-        ('InsertLineFilter', 'after', 'filter2')
+    ('subdir/test.c', TEST_CONTENT_C, SMUDGE_CONTENT_C_3, [
+        ('InsertLineFilter', 'after', 'filter1'),
+        ('SimpleFilter', 'search', 'filter3'),
+        ('InsertLineFilter', 'after', 'filter1'),
+        ('CommentOutFilter', 'after', 'filter2'),
     ]),
-    ('subdir/foo.c', [
-        ('CommentOutFilter', 'match', 'filter3'),
-        ('SimpleFilter', 'search', 'filter1'),
-        ('InsertLineFilter', 'after', 'filter2'),
+    ('subdir/foo.c', TEST_CONTENT_C, SMUDGE_CONTENT_C_4, [
+        ('SimpleFilter', 'search', 'filter3'),
+        ('InsertLineFilter', 'after', 'filter1'),
+        ('CommentOutFilter', 'after', 'filter2'),
         ('TestFilter', 'test', '1234')
     ]),
-    ('subdir/foo.txt', []),
-    ('subdir/notroot.py', [
-        ('CommentOutFilter', 'match', 'filter3'),
-        ('SimpleFilter', 'search', 'filter1'),
-        ('InsertLineFilter', 'after', 'filter2')
+    ('subdir/foo.txt', TEST_CONTENT_TXT, TEST_CONTENT_TXT, []),
+    ('subdir/notroot.py', TEST_CONTENT_PY, SMUDGE_CONTENT_PY_2, [
+        ('SimpleFilter', 'search', 'filter3'),
+        ('InsertLineFilter', 'after', 'filter1'),
+        ('CommentOutFilter', 'after', 'filter2'),
     ]),
-    ('subdir/special.c', [
-        ('CommentOutFilter', 'match', 'filter3'),
-        ('SimpleFilter', 'search', 'filter1'),
+    ('subdir/special.c', TEST_CONTENT_C, SMUDGE_CONTENT_C_5, [
+        ('SimpleFilter', 'search', 'filter3'),
+        ('InsertLineFilter', 'after', 'filter1'),
     ]),
-    ('subdir2/special.c', [
-        ('CommentOutFilter', 'match', 'filter3'),
-        ('SimpleFilter', 'search', 'filter1'),
+    ('subdir2/special.c', TEST_CONTENT_C, SMUDGE_CONTENT_C_5, [
+        ('SimpleFilter', 'search', 'filter3'),
+        ('InsertLineFilter', 'after', 'filter1'),
     ]),
 ]
 
 CONFIG_TOML = '''
 plugins = [
-    "plugin-test.py"
+    ".git/plugin-test.py"
 ]
 
 [filters.filter1]
-type = "simple"
-search = "filter1"
-replace = "qwer"
+type = "InsertLine"
+after = "filter1"
+insert = ['xfilt1_1', 'xfilt1_2']
 files = ["*.c", "!foo.c" ]
 
 [filters.filter2]
 filters = "filter3"
-type = "InsertLine"
-after = 'filter2'
-insert = [ "test1", "test2" ]
+type = "CommentOut"
+match = 'filter2'
 files = [ "subdir/*", "!*.txt" ]
 
 [filters.filter3]
 filters = [
-   { type = 'CommentOut', match = 'filter3' },
+   { type = 'simple', search = 'filter3', replace = 'xfilt3' },
    "filter1"
 ]
 
 [[rule]]
 filters = [ "filter1", "filter2" ]
 files = "!special.c"
 
@@ -146,25 +271,27 @@
 type = "Simple"
 search = "root"
 replace = "boot"
 files = "/*.py"
 '''
 
 PLUGIN_TEST = r'''
+import sys
 class TestFilter(GitFilter):
     def smudge(self, content):
-        content.set_text('test smudge\n' + content.get_text)
+        content.set_text('test smudge\n' + content.get_text())
 
     def clean(self, content):
         text = content.get_text()
-        if text.startswith('test smudge\n'):
-            content.set_text(text[11:])
+        needclean = text.startswith('test smudge\n')
+        if needclean:
+            content.set_text(text[12:])
 '''
 
-class TestCase(unittest.TestCase):
+class BasicTests(unittest.TestCase):
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def do_test_filter(self, filter, kw, path, expect):
@@ -184,15 +311,15 @@
 
     def do_test_inserts(self, comment_style, path, comments, block):
         filter = filters.InsertLineFilter({
             'after': r'(?s)im_start.*im_end',
             'insert': '\n'.join(TEST_LINES),
             'comment_style': comment_style,
             'block': block
-        })
+        }, 'test', 0)
         filter.update_config()
         f = build_insert_test_smudge_block if block else build_insert_test_smudge_line
         for kw in INSERT_TESTS:
             smudge_expect = f(**kw, lines=TEST_LINES, comment=comments)
             self.do_test_filter(filter, kw, path, smudge_expect)
 
     def test_insert_block_c(self):
@@ -206,15 +333,15 @@
 
     def test_insert_line_cpp(self):
         self.do_test_inserts('auto', Path('test.cpp'), git_smudge.COMMENT_DSLASH, True)
 
     def test_comment_out(self):
         filter = filters.CommentOutFilter({
             'match': '(?s)im_start.*im_end'
-        })
+        }, 'test', 0)
         filter.update_config()
         comment_styles = [
             ('test.py', git_smudge.COMMENT_HASH),
             ('test.xml', git_smudge.COMMENT_SGML),
             ('test.css', git_smudge.COMMENT_C),
         ]
         for i, kw in enumerate(INSERT_TESTS):
@@ -282,15 +409,15 @@
         self.tempdir = Path(tempfile.mkdtemp(prefix='git_smudge_unittest'))
         self.gitdir = self.tempdir / 'gitdir'
         self.gitdir.mkdir()
 
         self.config_path = self.gitdir / 'git-smudge.toml'
         self.config_path.write_text(CONFIG_TOML, encoding='ascii')
 
-        (self.tempdir / 'plugin-test.py').write_text(PLUGIN_TEST)
+        (self.gitdir / 'plugin-test.py').write_text(PLUGIN_TEST)
 
     def tearDown(self):
         shutil.rmtree(self.tempdir)
 
     def test_config_1(self):
         cfg = config.Config(self.tempdir, self.gitdir)
         self.assertEqual(self.config_path, cfg.config_path)
@@ -303,34 +430,131 @@
         })
 
         nf = filter_conf.named_filters
         self.assertSetEqual(set(nf), {'filter1', 'filter2', 'filter3', 'foo', 'rootpy'})
 
         filter_list = nf['filter1']
         self.assertEqual(len(filter_list), 1)
-        self.assertIsInstance(filter_list[0], filters.SimpleFilter)
+        self.assertIsInstance(filter_list[0], filters.InsertLineFilter)
 
         filter_list = nf['filter2']
         self.assertEqual(len(filter_list), 3)
-        self.assertIsInstance(filter_list[0], filters.CommentOutFilter)
-        self.assertIsInstance(filter_list[1], filters.SimpleFilter)
-        self.assertIsInstance(filter_list[2], filters.InsertLineFilter)
+        self.assertIsInstance(filter_list[0], filters.SimpleFilter)
+        self.assertIsInstance(filter_list[1], filters.InsertLineFilter)
+        self.assertIsInstance(filter_list[2], filters.CommentOutFilter)
 
         filter_list = nf['filter3']
         self.assertEqual(len(filter_list), 2)
-        self.assertIsInstance(filter_list[0], filters.CommentOutFilter)
-        self.assertIsInstance(filter_list[1], filters.SimpleFilter)
+        self.assertIsInstance(filter_list[0], filters.SimpleFilter)
+        self.assertIsInstance(filter_list[1], filters.InsertLineFilter)
 
-        pats = filter_conf.rule_patterns
-        self.assertSetEqual(set(pats), {
+        pats = filter_conf.patterns
+        self.assertSetEqual(set(pat[:2] for pat in pats), {
             ('*', '*.c'), ('*', 'foo.c'), ('subdir', '*'), ('*', '*.txt'),
             ('*', 'special.c'), ('', '*.py')
         })
 
-        for path, expect_filters in CONFIG_TEST_PATHS:
+        for path, clean_content, smudge_content, expect_filters in CONFIG_TEST_PATHS:
             with self.subTest(path=path):
                 filter_list = filter_conf.get_filters_for_path(path)
                 self.assertEqual([type(f).__name__ for f in filter_list], [f[0] for f in expect_filters])
 
+class IntegrationTests(unittest.TestCase):
+    def setUp(self):
+        self.tempdir = Path(tempfile.mkdtemp(prefix='git_smudge_unittest'))
+        self.gitdir = self.tempdir / '.git'
+
+        # Make sure that running python -m git_smudge is actually testing the code where
+        # we are located.
+        self.env = dict(os.environ)
+        self.env['PYTHONPATH'] = str(Path(__file__).absolute().parent.parent)
+        #self.env['GIT_SMUDGE_DEBUG'] = '1'
+
+        # This will exit with 0 if importing git_smudge.tests imports this file
+        p = subprocess.run([
+            sys.executable, '-c',
+            'import sys;'
+            'from git_smudge import tests;'
+            'sys.exit(0 if tests.__file__ == sys.argv[1] else 1)',
+            __file__
+        ], env=self.env, cwd=self.tempdir, check=False)
+        if p.returncode != 0:
+            self.skipTest(
+                "Importing git_smudge.tests from temporary directory "
+                "imports a different module")
+
+        try:
+            self.run_git(['init'])
+        except (OSError, subprocess.CalledProcessError):
+            # If we can't run `git`, skip this test
+            self.skipTest("Cannot run `git`")
+
+        self.config_path = self.gitdir / 'git-smudge.toml'
+
+        (self.gitdir / 'plugin-test.py').write_text(PLUGIN_TEST)
+        for path, clean_content, smudge_content, expect_filters in CONFIG_TEST_PATHS:
+            fpath = self.tempdir / path
+            fpath.parent.mkdir(parents=True, exist_ok=True)
+            fpath.write_text(clean_content)
+
+        self.run_git(['add', '.'])
+        self.run_git(['commit', '-m', 'Initial commit'])
+
+    def tearDown(self):
+        shutil.rmtree(self.tempdir)
+
+    def run_smudge(self, args, **kw):
+        cmd = [sys.executable, '-m', 'git_smudge'] + args
+        return subprocess.run(
+            cmd, env=self.env, cwd=self.tempdir,
+            encoding='utf8',
+            stdout=subprocess.PIPE, **kw)
+
+    def run_git(self, args, **kw):
+        return config.run_git(args, cwd=self.tempdir, env=self.env)
+
+    def run_apply(self, cmd, expect_changed):
+        p = self.run_smudge([cmd], stderr=subprocess.PIPE)
+        self.assertRegex(p.stderr, f'{expect_changed} files changed')
+        self.assertNotRegex(p.stderr, 'text that does not restore properly')
+
+        p = self.run_git(['status', '--porcelain', '-uall'])
+        self.assertEqual(p.stdout, '', "git status should indicate no changed files")
+
+        p = self.run_git(['diff'])
+        self.assertEqual(p.stdout, '', "git diff should indicate no changed files")
+
+        for path, clean_content, smudge_content, expect_filters in CONFIG_TEST_PATHS:
+            with self.subTest(cmd=cmd, path=path):
+                fpath = self.tempdir / path
+                content = fpath.read_text(encoding='utf8')
+                if cmd == 'clean':
+                    self.assertEqual(
+                        content, clean_content,
+                        "content should match clean content")
+                else:
+                    self.assertEqual(
+                        content, smudge_content,
+                        "content should match smudged content")
+
+
+    def test_git(self):
+        p = self.run_smudge(['setup'])
+        self.assertRegex(p.stdout, 'set up for git-smudge')
+
+        self.config_path.write_text(CONFIG_TOML, encoding='ascii')
+
+        p = self.run_git(['status', '--porcelain', '-uall'])
+        self.assertEqual(p.stdout, '', "git status should indicate no changed files")
+
+        self.run_apply('apply', 8)
+
+        # Make sure that running `apply` again doesn't change files
+        self.run_apply('apply', 0)
+
+        self.run_apply('clean', 8)
+
+        self.run_apply('clean', 0)
+
 if __name__ == '__main__':
     git_smudge.__main__.setup_logging(False)
     unittest.main()
```

### Comparing `git_smudge-0.0.8/git_smudge.egg-info/PKG-INFO` & `git_smudge-0.0.9/git_smudge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-smudge
-Version: 0.0.8
+Version: 0.0.9
 Summary: A powerful filter driver for Git which can automatically apply local changes to the working tree of a repository
 Home-page: https://ktpanda.org/software/git_smudge
 Author: Katie Rust
 Author-email: katie@ktpanda.org
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `git_smudge-0.0.8/setup.cfg` & `git_smudge-0.0.9/setup.cfg`

 * *Files identical despite different names*

