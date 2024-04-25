# Comparing `tmp/xunter-0.2.1.tar.gz` & `tmp/xunter-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xunter-0.2.1.tar", last modified: Sun Apr 21 12:33:58 2024, max compression
+gzip compressed data, was "xunter-0.2.2.tar", last modified: Thu Apr 25 15:30:19 2024, max compression
```

## Comparing `xunter-0.2.1.tar` & `xunter-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:33:58.460224 xunter-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 12:33:51.000000 xunter-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-21 12:33:51.000000 xunter-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-21 12:33:58.460224 xunter-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-21 12:33:51.000000 xunter-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 12:33:58.460224 xunter-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-21 12:33:51.000000 xunter-0.2.1/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3187 2024-04-21 12:33:51.000000 xunter-0.2.1/xunter
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:33:58.460224 xunter-0.2.1/xunter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-21 12:33:58.000000 xunter-0.2.1/xunter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-21 12:33:58.000000 xunter-0.2.1/xunter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 12:33:58.000000 xunter-0.2.1/xunter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-21 12:33:58.000000 xunter-0.2.1/xunter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 12:33:58.000000 xunter-0.2.1/xunter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9937 2024-04-21 12:33:51.000000 xunter-0.2.1/xunter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      556 2024-04-21 12:33:51.000000 xunter-0.2.1/xunter2excel
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:30:19.190402 xunter-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-25 15:30:15.000000 xunter-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-25 15:30:15.000000 xunter-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-25 15:30:19.190402 xunter-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-25 15:30:15.000000 xunter-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:30:19.190402 xunter-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-25 15:30:15.000000 xunter-0.2.2/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3441 2024-04-25 15:30:15.000000 xunter-0.2.2/xunter
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:30:19.190402 xunter-0.2.2/xunter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-25 15:30:19.000000 xunter-0.2.2/xunter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-25 15:30:19.000000 xunter-0.2.2/xunter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:30:19.000000 xunter-0.2.2/xunter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 15:30:19.000000 xunter-0.2.2/xunter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 15:30:19.000000 xunter-0.2.2/xunter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9937 2024-04-25 15:30:15.000000 xunter-0.2.2/xunter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      556 2024-04-25 15:30:15.000000 xunter-0.2.2/xunter2excel
```

### Comparing `xunter-0.2.1/LICENSE` & `xunter-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xunter-0.2.1/PKG-INFO` & `xunter-0.2.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xunter
-Version: 0.2.1
+Version: 0.2.2
 Summary: Profiling for the xonsh shell based on hunter.
 Home-page: https://github.com/anki-code/xunter
 Author: anki-code
 Author-email: no@no.no
 License: MIT
 Project-URL: Documentation, https://github.com/anki-code/xunter/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xunter
@@ -58,29 +58,40 @@
 xunter --no-rc ++depth-lt 5 ++output /tmp/22.xunter
 xunter --no-rc -c '2+2' ++filter 'Q(filename_endswith="main.py")'
 ```
 To set `++filter` read about [filters](https://python-hunter.readthedocs.io/en/latest/filtering.html) 
 and take a look into the [cookbook](https://python-hunter.readthedocs.io/en/latest/cookbook.html).
 Use `./playground/trace.py` to experiment with the tracing filters and understand how it works.
 
+#### Trace xonsh in the current directory
+
+```xsh
+mkdir -p ~/git/ && cd ~/git/
+git clone git+https://github.com/xonsh/xonsh
+cd xonsh
+xunter --no-rc -c '1+1' ++cwd
+# Trace ./xonsh
+```
+
 #### Find function calls
 
 ```xsh
-xunter --no-rc -c 'echo 1' ++filter 'Q(filename_has="specs.py"),Q(function="run_subproc")'
+xunter --no-rc -c 'echo 1' ++filter 'Q(filename_has="specs.py")' ++output /tmp/specs.xunter
+cat /tmp/specs.xunter | grep run_subproc
 # [...]/site-packages/xonsh/procs/specs.py:910:run_subproc 
 #   <= xonsh/built_ins.py:206:subproc_captured_hiddenobject 
 #   <= <string>:1:<module> <= xonsh/codecache.py:64:run_compiled_code 
 #   <= xonsh/codecache.py:218:run_code_with_cache
 #   <= xonsh/main.py:519:main_xonsh 
 #   <= xonsh/main.py:470:main 
 #   <= xunter/xunter:91:<module>
 #   - time_sec=[0.1505]
 
 # Don't forget about xonsh`s awesome macro call:
-xunter --no-rc -c 'echo 1' ++filter! Q(filename_has="specs.py"),Q(function="run_subproc")
+xunter --no-rc -c 'echo 1' ++printer call ++filter! Q(filename_has="specs.py"),Q(function="run_subproc")
 ```
 
 #### Filter code from prompt-toolkit and unwanted libs
 
 ```xsh
 # These `filename` filters will be applied to the code that executed at the end.
 # i.e. `filename="a.py"` will filter `a.py:func <= b.py:func <= c.py:func`
@@ -119,8 +130,10 @@
 ## Known issues
 
 If you see the unexpected exceptions try to install xonsh from the main branch first.
 
 ## See also
 * [xonsh-cheatsheet](https://github.com/anki-code/xonsh-cheatsheet)
 * [xonsh-install](https://github.com/anki-code/xonsh-install)
+* [How to debug xonsh interactively in IDE PyCharm](https://github.com/xonsh/xonsh/issues/3090#issuecomment-2068043223)
 * By putting `import ipdb; ipdb.set_trace()` into any place of code you can investigate the environment interactively.
+* xonsh builtin [`trace`](https://xon.sh/aliases.html#trace)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xunter Version: 0.2.1 Summary: Profiling for the
+Metadata-Version: 2.1 Name: xunter Version: 0.2.2 Summary: Profiling for the
 xonsh shell based on hunter. Home-page: https://github.com/anki-code/xunter
 Author: anki-code Author-email: no@no.no License: MIT Project-URL:
 Documentation, https://github.com/anki-code/xunter/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xunter Project-URL: Issue
 tracker, https://github.com/anki-code/xunter/issues Platform: any Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -21,22 +21,25 @@
 -c "2+2" ++depth-lt 5 # ^^^^^^^^^^^^^^^^ ^^^^^^^^^^^^ # xonsh xunter ``` Simple
 examples: ```xsh xunter --no-rc -c "2+2" ++depth-lt 10 xunter --no-rc ++depth-
 lt 5 ++output /tmp/22.xunter xunter --no-rc -c '2+2' ++filter 'Q
 (filename_endswith="main.py")' ``` To set `++filter` read about [filters]
 (https://python-hunter.readthedocs.io/en/latest/filtering.html) and take a look
 into the [cookbook](https://python-hunter.readthedocs.io/en/latest/
 cookbook.html). Use `./playground/trace.py` to experiment with the tracing
-filters and understand how it works. #### Find function calls ```xsh xunter --
-no-rc -c 'echo 1' ++filter 'Q(filename_has="specs.py"),Q
-(function="run_subproc")' # [...]/site-packages/xonsh/procs/specs.py:910:
-run_subproc # <= xonsh/built_ins.py:206:subproc_captured_hiddenobject # <= :1:
-<= xonsh/codecache.py:64:run_compiled_code # <= xonsh/codecache.py:218:
+filters and understand how it works. #### Trace xonsh in the current directory
+```xsh mkdir -p ~/git/ && cd ~/git/ git clone git+https://github.com/xonsh/
+xonsh cd xonsh xunter --no-rc -c '1+1' ++cwd # Trace ./xonsh ``` #### Find
+function calls ```xsh xunter --no-rc -c 'echo 1' ++filter 'Q
+(filename_has="specs.py")' ++output /tmp/specs.xunter cat /tmp/specs.xunter |
+grep run_subproc # [...]/site-packages/xonsh/procs/specs.py:910:run_subproc #
+<= xonsh/built_ins.py:206:subproc_captured_hiddenobject # <= :1: <= xonsh/
+codecache.py:64:run_compiled_code # <= xonsh/codecache.py:218:
 run_code_with_cache # <= xonsh/main.py:519:main_xonsh # <= xonsh/main.py:470:
 main # <= xunter/xunter:91: # - time_sec=[0.1505] # Don't forget about xonsh`s
-awesome macro call: xunter --no-rc -c 'echo 1' ++filter! Q
+awesome macro call: xunter --no-rc -c 'echo 1' ++printer call ++filter! Q
 (filename_has="specs.py"),Q(function="run_subproc") ``` #### Filter code from
 prompt-toolkit and unwanted libs ```xsh # These `filename` filters will be
 applied to the code that executed at the end. # i.e. `filename="a.py"` will
 filter `a.py:func <= b.py:func <= c.py:func` # but `c.py:func <= a.py:func <=
 b.py:func` case (`a.py` in the middle) wont be filtered. filters = [ '~Q
 (filename_has="prompt_toolkit/")', '~Q(filename_has="prompt/")', '~Q
 (filename_has="ptk_shell/")', '~Q(filename_has="pygments")', '~Q
@@ -46,9 +49,12 @@
 to monitor the activity: tail -f /tmp/1.xunter # | grep -i func ``` #### Time
 profiling ```xsh xunter --no-rc -c 'echo 1' ++time-sec-gt 0.1 ++depth-lt 2 #
 ... - time_sec=[1.3710] ``` #### Convert log to table ```python xunter --no-rc
 -c "2+2" ++depth-lt 10 ++printer stack ++output /tmp/22.xunter xunter2excel /
 tmp/22.xunter ``` ## Known issues If you see the unexpected exceptions try to
 install xonsh from the main branch first. ## See also * [xonsh-cheatsheet]
 (https://github.com/anki-code/xonsh-cheatsheet) * [xonsh-install](https://
-github.com/anki-code/xonsh-install) * By putting `import ipdb; ipdb.set_trace
-()` into any place of code you can investigate the environment interactively.
+github.com/anki-code/xonsh-install) * [How to debug xonsh interactively in IDE
+PyCharm](https://github.com/xonsh/xonsh/issues/3090#issuecomment-2068043223) *
+By putting `import ipdb; ipdb.set_trace()` into any place of code you can
+investigate the environment interactively. * xonsh builtin [`trace`](https://
+xon.sh/aliases.html#trace)
```

### Comparing `xunter-0.2.1/README.md` & `xunter-0.2.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -30,29 +30,40 @@
 xunter --no-rc ++depth-lt 5 ++output /tmp/22.xunter
 xunter --no-rc -c '2+2' ++filter 'Q(filename_endswith="main.py")'
 ```
 To set `++filter` read about [filters](https://python-hunter.readthedocs.io/en/latest/filtering.html) 
 and take a look into the [cookbook](https://python-hunter.readthedocs.io/en/latest/cookbook.html).
 Use `./playground/trace.py` to experiment with the tracing filters and understand how it works.
 
+#### Trace xonsh in the current directory
+
+```xsh
+mkdir -p ~/git/ && cd ~/git/
+git clone git+https://github.com/xonsh/xonsh
+cd xonsh
+xunter --no-rc -c '1+1' ++cwd
+# Trace ./xonsh
+```
+
 #### Find function calls
 
 ```xsh
-xunter --no-rc -c 'echo 1' ++filter 'Q(filename_has="specs.py"),Q(function="run_subproc")'
+xunter --no-rc -c 'echo 1' ++filter 'Q(filename_has="specs.py")' ++output /tmp/specs.xunter
+cat /tmp/specs.xunter | grep run_subproc
 # [...]/site-packages/xonsh/procs/specs.py:910:run_subproc 
 #   <= xonsh/built_ins.py:206:subproc_captured_hiddenobject 
 #   <= <string>:1:<module> <= xonsh/codecache.py:64:run_compiled_code 
 #   <= xonsh/codecache.py:218:run_code_with_cache
 #   <= xonsh/main.py:519:main_xonsh 
 #   <= xonsh/main.py:470:main 
 #   <= xunter/xunter:91:<module>
 #   - time_sec=[0.1505]
 
 # Don't forget about xonsh`s awesome macro call:
-xunter --no-rc -c 'echo 1' ++filter! Q(filename_has="specs.py"),Q(function="run_subproc")
+xunter --no-rc -c 'echo 1' ++printer call ++filter! Q(filename_has="specs.py"),Q(function="run_subproc")
 ```
 
 #### Filter code from prompt-toolkit and unwanted libs
 
 ```xsh
 # These `filename` filters will be applied to the code that executed at the end.
 # i.e. `filename="a.py"` will filter `a.py:func <= b.py:func <= c.py:func`
@@ -91,8 +102,10 @@
 ## Known issues
 
 If you see the unexpected exceptions try to install xonsh from the main branch first.
 
 ## See also
 * [xonsh-cheatsheet](https://github.com/anki-code/xonsh-cheatsheet)
 * [xonsh-install](https://github.com/anki-code/xonsh-install)
+* [How to debug xonsh interactively in IDE PyCharm](https://github.com/xonsh/xonsh/issues/3090#issuecomment-2068043223)
 * By putting `import ipdb; ipdb.set_trace()` into any place of code you can investigate the environment interactively.
+* xonsh builtin [`trace`](https://xon.sh/aliases.html#trace)
```

#### html2text {}

```diff
@@ -7,22 +7,25 @@
 -c "2+2" ++depth-lt 5 # ^^^^^^^^^^^^^^^^ ^^^^^^^^^^^^ # xonsh xunter ``` Simple
 examples: ```xsh xunter --no-rc -c "2+2" ++depth-lt 10 xunter --no-rc ++depth-
 lt 5 ++output /tmp/22.xunter xunter --no-rc -c '2+2' ++filter 'Q
 (filename_endswith="main.py")' ``` To set `++filter` read about [filters]
 (https://python-hunter.readthedocs.io/en/latest/filtering.html) and take a look
 into the [cookbook](https://python-hunter.readthedocs.io/en/latest/
 cookbook.html). Use `./playground/trace.py` to experiment with the tracing
-filters and understand how it works. #### Find function calls ```xsh xunter --
-no-rc -c 'echo 1' ++filter 'Q(filename_has="specs.py"),Q
-(function="run_subproc")' # [...]/site-packages/xonsh/procs/specs.py:910:
-run_subproc # <= xonsh/built_ins.py:206:subproc_captured_hiddenobject # <= :1:
-<= xonsh/codecache.py:64:run_compiled_code # <= xonsh/codecache.py:218:
+filters and understand how it works. #### Trace xonsh in the current directory
+```xsh mkdir -p ~/git/ && cd ~/git/ git clone git+https://github.com/xonsh/
+xonsh cd xonsh xunter --no-rc -c '1+1' ++cwd # Trace ./xonsh ``` #### Find
+function calls ```xsh xunter --no-rc -c 'echo 1' ++filter 'Q
+(filename_has="specs.py")' ++output /tmp/specs.xunter cat /tmp/specs.xunter |
+grep run_subproc # [...]/site-packages/xonsh/procs/specs.py:910:run_subproc #
+<= xonsh/built_ins.py:206:subproc_captured_hiddenobject # <= :1: <= xonsh/
+codecache.py:64:run_compiled_code # <= xonsh/codecache.py:218:
 run_code_with_cache # <= xonsh/main.py:519:main_xonsh # <= xonsh/main.py:470:
 main # <= xunter/xunter:91: # - time_sec=[0.1505] # Don't forget about xonsh`s
-awesome macro call: xunter --no-rc -c 'echo 1' ++filter! Q
+awesome macro call: xunter --no-rc -c 'echo 1' ++printer call ++filter! Q
 (filename_has="specs.py"),Q(function="run_subproc") ``` #### Filter code from
 prompt-toolkit and unwanted libs ```xsh # These `filename` filters will be
 applied to the code that executed at the end. # i.e. `filename="a.py"` will
 filter `a.py:func <= b.py:func <= c.py:func` # but `c.py:func <= a.py:func <=
 b.py:func` case (`a.py` in the middle) wont be filtered. filters = [ '~Q
 (filename_has="prompt_toolkit/")', '~Q(filename_has="prompt/")', '~Q
 (filename_has="ptk_shell/")', '~Q(filename_has="pygments")', '~Q
@@ -32,9 +35,12 @@
 to monitor the activity: tail -f /tmp/1.xunter # | grep -i func ``` #### Time
 profiling ```xsh xunter --no-rc -c 'echo 1' ++time-sec-gt 0.1 ++depth-lt 2 #
 ... - time_sec=[1.3710] ``` #### Convert log to table ```python xunter --no-rc
 -c "2+2" ++depth-lt 10 ++printer stack ++output /tmp/22.xunter xunter2excel /
 tmp/22.xunter ``` ## Known issues If you see the unexpected exceptions try to
 install xonsh from the main branch first. ## See also * [xonsh-cheatsheet]
 (https://github.com/anki-code/xonsh-cheatsheet) * [xonsh-install](https://
-github.com/anki-code/xonsh-install) * By putting `import ipdb; ipdb.set_trace
-()` into any place of code you can investigate the environment interactively.
+github.com/anki-code/xonsh-install) * [How to debug xonsh interactively in IDE
+PyCharm](https://github.com/xonsh/xonsh/issues/3090#issuecomment-2068043223) *
+By putting `import ipdb; ipdb.set_trace()` into any place of code you can
+investigate the environment interactively. * xonsh builtin [`trace`](https://
+xon.sh/aliases.html#trace)
```

### Comparing `xunter-0.2.1/setup.py` & `xunter-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.md', 'r', encoding='utf-8') as fh:
         long_description = fh.read()
 except (IOError, OSError):
     long_description = ''
 
 setuptools.setup(
     name='xunter',
-    version='0.2.1',
+    version='0.2.2',
     license='MIT',
     author='anki-code',
     author_email='no@no.no',
     description="Profiling for the xonsh shell based on hunter.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.6',
```

### Comparing `xunter-0.2.1/xunter` & `xunter-0.2.2/xunter`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 #!/usr/bin/env python
 
+import os
 import sys
 import argparse
 from hunter import trace, Q
 from xunter import CallPrinterProfile, StackPrinterProfile
 
 def xunter_help():
     print('Xunter was made for tracing xonsh via python-hunter.')
     print("Example: xunter --no-rc -c '2+2' ++depth-lt 10")
+    print("Example: git clone xonsh; cd xonsh; xunter --no-rc -c '2+2' ++depth-lt 10 ++cwd")
     print("Example: xunter --no-rc -c '2+2' ++depth-lt 10 ++output /tmp/22.xunter")
     print("Example: xunter --no-rc -c '2+2' ++depth-lt 10 ++filter 'Q(filename_has=\"main.py\")'")
     print()
 
 
 def argparse_xunter():
     parser = argparse.ArgumentParser(prefix_chars='-+')
+    parser.add_argument('++cwd', action='store_true', help='Append current working directory to PATH.')
     parser.add_argument('++time-sec-gt', help="Show rows with time in seconds greater than.")
     parser.add_argument('++depth-lt', help="Trace depth. The same as `++filter 'Q(depth_lt=5)'`.")
     parser.add_argument('++printer', default='stack', help="Printer: `stack` or `call`. Default: `stack`.")
     parser.add_argument('++stdlib', action='store_true', help='Trace stdlib. Default: no.')
     parser.add_argument('++output', default='stderr', help='Output: `stdout`, `stderr` or filepath. Default: `stderr`.')
     parser.add_argument('++filter', default='()', help='Hunter filters: https://python-hunter.readthedocs.io/en/latest/filtering.html')
     parser.add_argument('++debug', action='store_true', help='Debug mode for xunter.')
@@ -48,14 +51,17 @@
 
 if x := argparse_xunter():
     for a in sys.argv:
         if a[:2] == '++':
             print(f'Unknown xunter argument: {a}')
             sys.exit(1)
 
+    if x.cwd:
+        sys.path.insert(0, os.getcwd())
+
     if x.printer == 'call':
         printer = CallPrinterProfile
     elif x.printer == 'stack':
         printer = StackPrinterProfile
     else:
         raise Exception('Unknown printer')
 
@@ -82,15 +88,15 @@
         print('Filters:', filters, file=sys.stderr)
 
     trace(
         *filters,
         action=printer,
         stdlib=x.stdlib
     )
-# exit()
+
 # From `cat @$(which xonsh)`:
 import re
 import sys
 from xonsh.main import main
 if __name__ == '__main__':
     sys.argv[0] = re.sub(r'(-script\.pyw|\.exe)?$', '', sys.argv[0])
     sys.exit(main())
```

### Comparing `xunter-0.2.1/xunter.egg-info/PKG-INFO` & `xunter-0.2.2/xunter.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xunter
-Version: 0.2.1
+Version: 0.2.2
 Summary: Profiling for the xonsh shell based on hunter.
 Home-page: https://github.com/anki-code/xunter
 Author: anki-code
 Author-email: no@no.no
 License: MIT
 Project-URL: Documentation, https://github.com/anki-code/xunter/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xunter
@@ -58,29 +58,40 @@
 xunter --no-rc ++depth-lt 5 ++output /tmp/22.xunter
 xunter --no-rc -c '2+2' ++filter 'Q(filename_endswith="main.py")'
 ```
 To set `++filter` read about [filters](https://python-hunter.readthedocs.io/en/latest/filtering.html) 
 and take a look into the [cookbook](https://python-hunter.readthedocs.io/en/latest/cookbook.html).
 Use `./playground/trace.py` to experiment with the tracing filters and understand how it works.
 
+#### Trace xonsh in the current directory
+
+```xsh
+mkdir -p ~/git/ && cd ~/git/
+git clone git+https://github.com/xonsh/xonsh
+cd xonsh
+xunter --no-rc -c '1+1' ++cwd
+# Trace ./xonsh
+```
+
 #### Find function calls
 
 ```xsh
-xunter --no-rc -c 'echo 1' ++filter 'Q(filename_has="specs.py"),Q(function="run_subproc")'
+xunter --no-rc -c 'echo 1' ++filter 'Q(filename_has="specs.py")' ++output /tmp/specs.xunter
+cat /tmp/specs.xunter | grep run_subproc
 # [...]/site-packages/xonsh/procs/specs.py:910:run_subproc 
 #   <= xonsh/built_ins.py:206:subproc_captured_hiddenobject 
 #   <= <string>:1:<module> <= xonsh/codecache.py:64:run_compiled_code 
 #   <= xonsh/codecache.py:218:run_code_with_cache
 #   <= xonsh/main.py:519:main_xonsh 
 #   <= xonsh/main.py:470:main 
 #   <= xunter/xunter:91:<module>
 #   - time_sec=[0.1505]
 
 # Don't forget about xonsh`s awesome macro call:
-xunter --no-rc -c 'echo 1' ++filter! Q(filename_has="specs.py"),Q(function="run_subproc")
+xunter --no-rc -c 'echo 1' ++printer call ++filter! Q(filename_has="specs.py"),Q(function="run_subproc")
 ```
 
 #### Filter code from prompt-toolkit and unwanted libs
 
 ```xsh
 # These `filename` filters will be applied to the code that executed at the end.
 # i.e. `filename="a.py"` will filter `a.py:func <= b.py:func <= c.py:func`
@@ -119,8 +130,10 @@
 ## Known issues
 
 If you see the unexpected exceptions try to install xonsh from the main branch first.
 
 ## See also
 * [xonsh-cheatsheet](https://github.com/anki-code/xonsh-cheatsheet)
 * [xonsh-install](https://github.com/anki-code/xonsh-install)
+* [How to debug xonsh interactively in IDE PyCharm](https://github.com/xonsh/xonsh/issues/3090#issuecomment-2068043223)
 * By putting `import ipdb; ipdb.set_trace()` into any place of code you can investigate the environment interactively.
+* xonsh builtin [`trace`](https://xon.sh/aliases.html#trace)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xunter Version: 0.2.1 Summary: Profiling for the
+Metadata-Version: 2.1 Name: xunter Version: 0.2.2 Summary: Profiling for the
 xonsh shell based on hunter. Home-page: https://github.com/anki-code/xunter
 Author: anki-code Author-email: no@no.no License: MIT Project-URL:
 Documentation, https://github.com/anki-code/xunter/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xunter Project-URL: Issue
 tracker, https://github.com/anki-code/xunter/issues Platform: any Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -21,22 +21,25 @@
 -c "2+2" ++depth-lt 5 # ^^^^^^^^^^^^^^^^ ^^^^^^^^^^^^ # xonsh xunter ``` Simple
 examples: ```xsh xunter --no-rc -c "2+2" ++depth-lt 10 xunter --no-rc ++depth-
 lt 5 ++output /tmp/22.xunter xunter --no-rc -c '2+2' ++filter 'Q
 (filename_endswith="main.py")' ``` To set `++filter` read about [filters]
 (https://python-hunter.readthedocs.io/en/latest/filtering.html) and take a look
 into the [cookbook](https://python-hunter.readthedocs.io/en/latest/
 cookbook.html). Use `./playground/trace.py` to experiment with the tracing
-filters and understand how it works. #### Find function calls ```xsh xunter --
-no-rc -c 'echo 1' ++filter 'Q(filename_has="specs.py"),Q
-(function="run_subproc")' # [...]/site-packages/xonsh/procs/specs.py:910:
-run_subproc # <= xonsh/built_ins.py:206:subproc_captured_hiddenobject # <= :1:
-<= xonsh/codecache.py:64:run_compiled_code # <= xonsh/codecache.py:218:
+filters and understand how it works. #### Trace xonsh in the current directory
+```xsh mkdir -p ~/git/ && cd ~/git/ git clone git+https://github.com/xonsh/
+xonsh cd xonsh xunter --no-rc -c '1+1' ++cwd # Trace ./xonsh ``` #### Find
+function calls ```xsh xunter --no-rc -c 'echo 1' ++filter 'Q
+(filename_has="specs.py")' ++output /tmp/specs.xunter cat /tmp/specs.xunter |
+grep run_subproc # [...]/site-packages/xonsh/procs/specs.py:910:run_subproc #
+<= xonsh/built_ins.py:206:subproc_captured_hiddenobject # <= :1: <= xonsh/
+codecache.py:64:run_compiled_code # <= xonsh/codecache.py:218:
 run_code_with_cache # <= xonsh/main.py:519:main_xonsh # <= xonsh/main.py:470:
 main # <= xunter/xunter:91: # - time_sec=[0.1505] # Don't forget about xonsh`s
-awesome macro call: xunter --no-rc -c 'echo 1' ++filter! Q
+awesome macro call: xunter --no-rc -c 'echo 1' ++printer call ++filter! Q
 (filename_has="specs.py"),Q(function="run_subproc") ``` #### Filter code from
 prompt-toolkit and unwanted libs ```xsh # These `filename` filters will be
 applied to the code that executed at the end. # i.e. `filename="a.py"` will
 filter `a.py:func <= b.py:func <= c.py:func` # but `c.py:func <= a.py:func <=
 b.py:func` case (`a.py` in the middle) wont be filtered. filters = [ '~Q
 (filename_has="prompt_toolkit/")', '~Q(filename_has="prompt/")', '~Q
 (filename_has="ptk_shell/")', '~Q(filename_has="pygments")', '~Q
@@ -46,9 +49,12 @@
 to monitor the activity: tail -f /tmp/1.xunter # | grep -i func ``` #### Time
 profiling ```xsh xunter --no-rc -c 'echo 1' ++time-sec-gt 0.1 ++depth-lt 2 #
 ... - time_sec=[1.3710] ``` #### Convert log to table ```python xunter --no-rc
 -c "2+2" ++depth-lt 10 ++printer stack ++output /tmp/22.xunter xunter2excel /
 tmp/22.xunter ``` ## Known issues If you see the unexpected exceptions try to
 install xonsh from the main branch first. ## See also * [xonsh-cheatsheet]
 (https://github.com/anki-code/xonsh-cheatsheet) * [xonsh-install](https://
-github.com/anki-code/xonsh-install) * By putting `import ipdb; ipdb.set_trace
-()` into any place of code you can investigate the environment interactively.
+github.com/anki-code/xonsh-install) * [How to debug xonsh interactively in IDE
+PyCharm](https://github.com/xonsh/xonsh/issues/3090#issuecomment-2068043223) *
+By putting `import ipdb; ipdb.set_trace()` into any place of code you can
+investigate the environment interactively. * xonsh builtin [`trace`](https://
+xon.sh/aliases.html#trace)
```

### Comparing `xunter-0.2.1/xunter.py` & `xunter-0.2.2/xunter.py`

 * *Files identical despite different names*

### Comparing `xunter-0.2.1/xunter2excel` & `xunter-0.2.2/xunter2excel`

 * *Files identical despite different names*

