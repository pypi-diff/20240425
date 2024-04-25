# Comparing `tmp/treeview_karjakak-1.8.5.tar.gz` & `tmp/treeview-karjakak-1.8.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treeview_karjakak-1.8.5.tar", last modified: Thu Apr 25 06:55:15 2024, max compression
+gzip compressed data, was "treeview-karjakak-1.8.5rc1.tar", last modified: Tue Oct 10 08:28:30 2023, max compression
```

## Comparing `treeview_karjakak-1.8.5.tar` & `treeview-karjakak-1.8.5rc1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 06:55:15.354821 treeview_karjakak-1.8.5/
--rw-rw-rw-   0        0        0     6952 2024-04-25 06:55:15.353880 treeview_karjakak-1.8.5/PKG-INFO
--rw-rw-rw-   0        0        0     6019 2021-08-24 02:06:04.000000 treeview_karjakak-1.8.5/README.md
--rw-rw-rw-   0        0        0      115 2022-01-24 09:33:35.000000 treeview_karjakak-1.8.5/pyproject.toml
--rw-rw-rw-   0        0        0      701 2024-04-25 06:55:15.355870 treeview_karjakak-1.8.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-25 06:55:15.147673 treeview_karjakak-1.8.5/treeview/
--rw-rw-rw-   0        0        0       38 2022-09-22 05:02:49.000000 treeview_karjakak-1.8.5/treeview/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 06:55:15.225670 treeview_karjakak-1.8.5/treeview/dbase/
--rw-rw-rw-   0        0        0       34 2021-08-30 06:01:18.000000 treeview_karjakak-1.8.5/treeview/dbase/__init__.py
--rw-rw-rw-   0        0        0     5899 2022-11-02 14:55:48.000000 treeview_karjakak-1.8.5/treeview/dbase/datab.py
--rw-rw-rw-   0        0        0    22136 2024-03-26 12:44:19.000000 treeview_karjakak-1.8.5/treeview/treeview.py
-drwxrwxrwx   0        0        0        0 2024-04-25 06:55:15.307433 treeview_karjakak-1.8.5/treeview/tvdescript/
--rw-rw-rw-   0        0        0       63 2021-08-27 03:00:48.000000 treeview_karjakak-1.8.5/treeview/tvdescript/__init__.py
--rw-rw-rw-   0        0        0     3002 2022-11-02 14:56:17.000000 treeview_karjakak-1.8.5/treeview/tvdescript/tvdescript.py
-drwxrwxrwx   0        0        0        0 2024-04-25 06:55:15.352511 treeview_karjakak-1.8.5/treeview_karjakak.egg-info/
--rw-rw-rw-   0        0        0     6952 2024-04-25 06:55:15.000000 treeview_karjakak-1.8.5/treeview_karjakak.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2024-04-25 06:55:15.000000 treeview_karjakak-1.8.5/treeview_karjakak.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 06:55:15.000000 treeview_karjakak-1.8.5/treeview_karjakak.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-25 06:55:15.000000 treeview_karjakak-1.8.5/treeview_karjakak.egg-info/top_level.txt
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-10-10 08:28:30.290210 treeview-karjakak-1.8.5rc1/
+-rw-r--r--   0 karja      (501) staff       (20)     6648 2023-10-10 08:28:30.290127 treeview-karjakak-1.8.5rc1/PKG-INFO
+-rw-r--r--   0 karja      (501) staff       (20)     6019 2021-08-24 02:06:04.000000 treeview-karjakak-1.8.5rc1/README.md
+-rw-r--r--   0 karja      (501) staff       (20)      115 2022-01-24 09:33:35.000000 treeview-karjakak-1.8.5rc1/pyproject.toml
+-rw-r--r--   0 karja      (501) staff       (20)      679 2023-10-10 08:28:30.290479 treeview-karjakak-1.8.5rc1/setup.cfg
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-10-10 08:28:30.288634 treeview-karjakak-1.8.5rc1/treeview/
+-rw-r--r--   0 karja      (501) staff       (20)       38 2022-09-22 05:02:49.000000 treeview-karjakak-1.8.5rc1/treeview/__init__.py
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-10-10 08:28:30.289148 treeview-karjakak-1.8.5rc1/treeview/dbase/
+-rw-r--r--   0 karja      (501) staff       (20)       34 2021-08-30 06:01:18.000000 treeview-karjakak-1.8.5rc1/treeview/dbase/__init__.py
+-rw-r--r--   0 karja      (501) staff       (20)     5899 2022-11-02 14:55:48.000000 treeview-karjakak-1.8.5rc1/treeview/dbase/datab.py
+-rw-r--r--   0 karja      (501) staff       (20)    22056 2023-10-10 02:54:45.000000 treeview-karjakak-1.8.5rc1/treeview/treeview.py
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-10-10 08:28:30.289364 treeview-karjakak-1.8.5rc1/treeview/tvdescript/
+-rw-r--r--   0 karja      (501) staff       (20)       63 2021-08-27 03:00:48.000000 treeview-karjakak-1.8.5rc1/treeview/tvdescript/__init__.py
+-rw-r--r--   0 karja      (501) staff       (20)     3002 2022-11-02 14:56:17.000000 treeview-karjakak-1.8.5rc1/treeview/tvdescript/tvdescript.py
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-10-10 08:28:30.289799 treeview-karjakak-1.8.5rc1/treeview_karjakak.egg-info/
+-rw-r--r--   0 karja      (501) staff       (20)     6648 2023-10-10 08:28:30.000000 treeview-karjakak-1.8.5rc1/treeview_karjakak.egg-info/PKG-INFO
+-rw-r--r--   0 karja      (501) staff       (20)      357 2023-10-10 08:28:30.000000 treeview-karjakak-1.8.5rc1/treeview_karjakak.egg-info/SOURCES.txt
+-rw-r--r--   0 karja      (501) staff       (20)        1 2023-10-10 08:28:30.000000 treeview-karjakak-1.8.5rc1/treeview_karjakak.egg-info/dependency_links.txt
+-rw-r--r--   0 karja      (501) staff       (20)        9 2023-10-10 08:28:30.000000 treeview-karjakak-1.8.5rc1/treeview_karjakak.egg-info/top_level.txt
```

### Comparing `treeview_karjakak-1.8.5/PKG-INFO` & `treeview-karjakak-1.8.5rc1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,308 +1,308 @@
-Metadata-Version: 2.1
-Name: treeview-karjakak
-Version: 1.8.5
-Summary: TreeView is a note taking that written to text file and view in tree-view outline.
-Home-page: https://github.com/kakkarja/TV
-Author: karjakak
-Author-email: kakkarja.github@gmail.com
-License: BSD3 License
-Classifier: Environment :: Win32 (MS Windows)
-Classifier: Environment :: MacOS X
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Topic :: Text Editors :: Text Processing
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
-# TreeView
-## Writing an outline note with tree-view look.
-
-## Installation
-```
-pip install treeview-karjakak
-```
-## Usage
-```Python
-from treeview import TreeView, conftv
-
-# To configure the childs (by default 50 childs, and 4 spaces)
-TreeView = conftv(TreeView, 5, 1)
-print(dict(TreeView.childs))
-
-w = 'Amazing Grace'
-with TreeView('test') as tv:
-
-    # First time write on note as parent
-    tv.writetree(w)
-
-    # Write it with loop in childs 
-    for i in range(5):
-        tv.quickchild(w, child = f'child{i+1}')
-        
-    # Edit the parent
-    tv.edittree('Amazing Grace, how sweet the sound')
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    
-    # Edit again in row 4 to child2
-    tv.edittree('Mantaaaaaaap!', row = 4, child = 'child2')
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    
-    # Write new parent
-    tv.addparent('Wow good job')
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    
-    # Edit again in row 6 to child5
-    tv.edittree('Wow good job buddy', row = 6, child = 'child5')
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    
-    # Write again new childs
-    tv.quickchild('Totally awesome', child = 'child1')
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    tv.quickchild('This is quick child edit', child = 'child2')
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    tv.quickchild('Thank You', child = 'child1')
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    
-    # Delete row 10
-    tv.delrow(10)
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    
-    # Insert to row 8 as child1
-    tv.insertrow('God bless you', row = 8, child = 'child1' )
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    
-    # Moving position from row 6 to row 4
-    tv.movetree(6, 4)
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    
-    # Moving position of child in row 6 as child1
-    tv.movechild(6, child = 'child1')
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    
-    # Print an iterator to dict
-    pprint(dict(tv.insighttree()))
-    
-    # Create spaces between rows
-    for i in range(1, tv.getdatanum()+4, 2):
-        if i == 15:
-            break
-        tv.insertspace(i)
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    pprint(dict(tv.insighttree()))
-    
-    # Backup note as json file
-    tv.backuptv()
-    del tv, w, i
-```
-**Result:**
-```Python
-{'child1': 1, 'child2': 2, 'child3': 3, 'child4': 4, 'child5': 5}
-------------
-Amazing Grace, how sweet the sound:
- -Amazing Grace
-  -Amazing Grace
-   -Amazing Grace
-    -Amazing Grace
-     -Amazing Grace
-------------
-------------
-Amazing Grace, how sweet the sound:
- -Amazing Grace
-  -Amazing Grace
-   -Amazing Grace
-  -Mantaaaaaaap!
-     -Amazing Grace
-------------
-------------
-Amazing Grace, how sweet the sound:
- -Amazing Grace
-  -Amazing Grace
-   -Amazing Grace
-  -Mantaaaaaaap!
-     -Amazing Grace
-
-Wow good job:
-------------
-------------
-Amazing Grace, how sweet the sound:
- -Amazing Grace
-  -Amazing Grace
-   -Amazing Grace
-  -Mantaaaaaaap!
-     -Amazing Grace
-     -Wow good job buddy
-
-Wow good job:
-------------
-------------
-Amazing Grace, how sweet the sound:
- -Amazing Grace
-  -Amazing Grace
-   -Amazing Grace
-  -Mantaaaaaaap!
-     -Amazing Grace
-     -Wow good job buddy
-
-Wow good job:
- -Totally awesome
-------------
-------------
-Amazing Grace, how sweet the sound:
- -Amazing Grace
-  -Amazing Grace
-   -Amazing Grace
-  -Mantaaaaaaap!
-     -Amazing Grace
-     -Wow good job buddy
-
-Wow good job:
- -Totally awesome
-  -This is quick child edit
-------------
-------------
-Amazing Grace, how sweet the sound:
- -Amazing Grace
-  -Amazing Grace
-   -Amazing Grace
-  -Mantaaaaaaap!
-     -Amazing Grace
-     -Wow good job buddy
-
-Wow good job:
- -Totally awesome
-  -This is quick child edit
- -Thank You
-------------
-------------
-Amazing Grace, how sweet the sound:
- -Amazing Grace
-  -Amazing Grace
-   -Amazing Grace
-  -Mantaaaaaaap!
-     -Amazing Grace
-     -Wow good job buddy
-
-Wow good job:
- -Totally awesome
- -Thank You
-------------
-------------
-Amazing Grace, how sweet the sound:
- -Amazing Grace
-  -Amazing Grace
-   -Amazing Grace
-  -Mantaaaaaaap!
-     -Amazing Grace
-     -Wow good job buddy
- -God bless you
-
-Wow good job:
- -Totally awesome
- -Thank You
-------------
-------------
-Amazing Grace, how sweet the sound:
- -Amazing Grace
-  -Amazing Grace
-   -Amazing Grace
-     -Wow good job buddy
-  -Mantaaaaaaap!
-     -Amazing Grace
- -God bless you
-
-Wow good job:
- -Totally awesome
- -Thank You
-------------
-------------
-Amazing Grace, how sweet the sound:
- -Amazing Grace
-  -Amazing Grace
-   -Amazing Grace
-     -Wow good job buddy
-  -Mantaaaaaaap!
- -Amazing Grace
- -God bless you
-
-Wow good job:
- -Totally awesome
- -Thank You
-------------
-{0: ('parent', 'Amazing Grace, how sweet the sound:\n'),
- 1: ('child1', '-Amazing Grace\n'),
- 2: ('child2', '-Amazing Grace\n'),
- 3: ('child3', '-Amazing Grace\n'),
- 4: ('child5', '-Wow good job buddy\n'),
- 5: ('child2', '-Mantaaaaaaap!\n'),
- 6: ('child1', '-Amazing Grace\n'),
- 7: ('child1', '-God bless you\n'),
- 8: ('space', '\n'),
- 9: ('parent', 'Wow good job:\n'),
- 10: ('child1', '-Totally awesome\n'),
- 11: ('child1', '-Thank You\n')}
-------------
-Amazing Grace, how sweet the sound:
-
- -Amazing Grace
-
-  -Amazing Grace
-
-   -Amazing Grace
-
-     -Wow good job buddy
-
-  -Mantaaaaaaap!
-
- -Amazing Grace
-
- -God bless you
-
-Wow good job:
- -Totally awesome
- -Thank You
-------------
-{0: ('parent', 'Amazing Grace, how sweet the sound:\n'),
- 1: ('space', '\n'),
- 2: ('child1', '-Amazing Grace\n'),
- 3: ('space', '\n'),
- 4: ('child2', '-Amazing Grace\n'),
- 5: ('space', '\n'),
- 6: ('child3', '-Amazing Grace\n'),
- 7: ('space', '\n'),
- 8: ('child5', '-Wow good job buddy\n'),
- 9: ('space', '\n'),
- 10: ('child2', '-Mantaaaaaaap!\n'),
- 11: ('space', '\n'),
- 12: ('child1', '-Amazing Grace\n'),
- 13: ('space', '\n'),
- 14: ('child1', '-God bless you\n'),
- 15: ('space', '\n'),
- 16: ('parent', 'Wow good job:\n'),
- 17: ('child1', '-Totally awesome\n'),
- 18: ('child1', '-Thank You\n')}
-```
+Metadata-Version: 2.1
+Name: treeview-karjakak
+Version: 1.8.5rc1
+Summary: TreeView is a note taking that written to text file and view in tree-view outline.
+Home-page: https://github.com/kakkarja/TV
+Author: karjakak
+Author-email: kakkarja.github@gmail.com
+License: BSD3 License
+Classifier: Environment :: Win32 (MS Windows)
+Classifier: Environment :: MacOS X
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Topic :: Text Editors :: Text Processing
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+
+# TreeView
+## Writing an outline note with tree-view look.
+
+## Installation
+```
+pip install treeview-karjakak
+```
+## Usage
+```Python
+from treeview import TreeView, conftv
+
+# To configure the childs (by default 50 childs, and 4 spaces)
+TreeView = conftv(TreeView, 5, 1)
+print(dict(TreeView.childs))
+
+w = 'Amazing Grace'
+with TreeView('test') as tv:
+
+    # First time write on note as parent
+    tv.writetree(w)
+
+    # Write it with loop in childs 
+    for i in range(5):
+        tv.quickchild(w, child = f'child{i+1}')
+        
+    # Edit the parent
+    tv.edittree('Amazing Grace, how sweet the sound')
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    
+    # Edit again in row 4 to child2
+    tv.edittree('Mantaaaaaaap!', row = 4, child = 'child2')
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    
+    # Write new parent
+    tv.addparent('Wow good job')
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    
+    # Edit again in row 6 to child5
+    tv.edittree('Wow good job buddy', row = 6, child = 'child5')
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    
+    # Write again new childs
+    tv.quickchild('Totally awesome', child = 'child1')
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    tv.quickchild('This is quick child edit', child = 'child2')
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    tv.quickchild('Thank You', child = 'child1')
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    
+    # Delete row 10
+    tv.delrow(10)
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    
+    # Insert to row 8 as child1
+    tv.insertrow('God bless you', row = 8, child = 'child1' )
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    
+    # Moving position from row 6 to row 4
+    tv.movetree(6, 4)
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    
+    # Moving position of child in row 6 as child1
+    tv.movechild(6, child = 'child1')
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    
+    # Print an iterator to dict
+    pprint(dict(tv.insighttree()))
+    
+    # Create spaces between rows
+    for i in range(1, tv.getdatanum()+4, 2):
+        if i == 15:
+            break
+        tv.insertspace(i)
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    pprint(dict(tv.insighttree()))
+    
+    # Backup note as json file
+    tv.backuptv()
+    del tv, w, i
+```
+**Result:**
+```Python
+{'child1': 1, 'child2': 2, 'child3': 3, 'child4': 4, 'child5': 5}
+------------
+Amazing Grace, how sweet the sound:
+ -Amazing Grace
+  -Amazing Grace
+   -Amazing Grace
+    -Amazing Grace
+     -Amazing Grace
+------------
+------------
+Amazing Grace, how sweet the sound:
+ -Amazing Grace
+  -Amazing Grace
+   -Amazing Grace
+  -Mantaaaaaaap!
+     -Amazing Grace
+------------
+------------
+Amazing Grace, how sweet the sound:
+ -Amazing Grace
+  -Amazing Grace
+   -Amazing Grace
+  -Mantaaaaaaap!
+     -Amazing Grace
+
+Wow good job:
+------------
+------------
+Amazing Grace, how sweet the sound:
+ -Amazing Grace
+  -Amazing Grace
+   -Amazing Grace
+  -Mantaaaaaaap!
+     -Amazing Grace
+     -Wow good job buddy
+
+Wow good job:
+------------
+------------
+Amazing Grace, how sweet the sound:
+ -Amazing Grace
+  -Amazing Grace
+   -Amazing Grace
+  -Mantaaaaaaap!
+     -Amazing Grace
+     -Wow good job buddy
+
+Wow good job:
+ -Totally awesome
+------------
+------------
+Amazing Grace, how sweet the sound:
+ -Amazing Grace
+  -Amazing Grace
+   -Amazing Grace
+  -Mantaaaaaaap!
+     -Amazing Grace
+     -Wow good job buddy
+
+Wow good job:
+ -Totally awesome
+  -This is quick child edit
+------------
+------------
+Amazing Grace, how sweet the sound:
+ -Amazing Grace
+  -Amazing Grace
+   -Amazing Grace
+  -Mantaaaaaaap!
+     -Amazing Grace
+     -Wow good job buddy
+
+Wow good job:
+ -Totally awesome
+  -This is quick child edit
+ -Thank You
+------------
+------------
+Amazing Grace, how sweet the sound:
+ -Amazing Grace
+  -Amazing Grace
+   -Amazing Grace
+  -Mantaaaaaaap!
+     -Amazing Grace
+     -Wow good job buddy
+
+Wow good job:
+ -Totally awesome
+ -Thank You
+------------
+------------
+Amazing Grace, how sweet the sound:
+ -Amazing Grace
+  -Amazing Grace
+   -Amazing Grace
+  -Mantaaaaaaap!
+     -Amazing Grace
+     -Wow good job buddy
+ -God bless you
+
+Wow good job:
+ -Totally awesome
+ -Thank You
+------------
+------------
+Amazing Grace, how sweet the sound:
+ -Amazing Grace
+  -Amazing Grace
+   -Amazing Grace
+     -Wow good job buddy
+  -Mantaaaaaaap!
+     -Amazing Grace
+ -God bless you
+
+Wow good job:
+ -Totally awesome
+ -Thank You
+------------
+------------
+Amazing Grace, how sweet the sound:
+ -Amazing Grace
+  -Amazing Grace
+   -Amazing Grace
+     -Wow good job buddy
+  -Mantaaaaaaap!
+ -Amazing Grace
+ -God bless you
+
+Wow good job:
+ -Totally awesome
+ -Thank You
+------------
+{0: ('parent', 'Amazing Grace, how sweet the sound:\n'),
+ 1: ('child1', '-Amazing Grace\n'),
+ 2: ('child2', '-Amazing Grace\n'),
+ 3: ('child3', '-Amazing Grace\n'),
+ 4: ('child5', '-Wow good job buddy\n'),
+ 5: ('child2', '-Mantaaaaaaap!\n'),
+ 6: ('child1', '-Amazing Grace\n'),
+ 7: ('child1', '-God bless you\n'),
+ 8: ('space', '\n'),
+ 9: ('parent', 'Wow good job:\n'),
+ 10: ('child1', '-Totally awesome\n'),
+ 11: ('child1', '-Thank You\n')}
+------------
+Amazing Grace, how sweet the sound:
+
+ -Amazing Grace
+
+  -Amazing Grace
+
+   -Amazing Grace
+
+     -Wow good job buddy
+
+  -Mantaaaaaaap!
+
+ -Amazing Grace
+
+ -God bless you
+
+Wow good job:
+ -Totally awesome
+ -Thank You
+------------
+{0: ('parent', 'Amazing Grace, how sweet the sound:\n'),
+ 1: ('space', '\n'),
+ 2: ('child1', '-Amazing Grace\n'),
+ 3: ('space', '\n'),
+ 4: ('child2', '-Amazing Grace\n'),
+ 5: ('space', '\n'),
+ 6: ('child3', '-Amazing Grace\n'),
+ 7: ('space', '\n'),
+ 8: ('child5', '-Wow good job buddy\n'),
+ 9: ('space', '\n'),
+ 10: ('child2', '-Mantaaaaaaap!\n'),
+ 11: ('space', '\n'),
+ 12: ('child1', '-Amazing Grace\n'),
+ 13: ('space', '\n'),
+ 14: ('child1', '-God bless you\n'),
+ 15: ('space', '\n'),
+ 16: ('parent', 'Wow good job:\n'),
+ 17: ('child1', '-Totally awesome\n'),
+ 18: ('child1', '-Thank You\n')}
+```
```

### Comparing `treeview_karjakak-1.8.5/README.md` & `treeview-karjakak-1.8.5rc1/README.md`

 * *Files identical despite different names*

### Comparing `treeview_karjakak-1.8.5/setup.cfg` & `treeview-karjakak-1.8.5rc1/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,43 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2074 7265 6576 6965 772d 6b61 726a   = treeview-karj
-00000020: 616b 616b 0d0a 7665 7273 696f 6e20 3d20  akak..version = 
-00000030: 312e 382e 350d 0a61 7574 686f 7220 3d20  1.8.5..author = 
-00000040: 6b61 726a 616b 616b 0d0a 6175 7468 6f72  karjakak..author
-00000050: 5f65 6d61 696c 203d 206b 616b 6b61 726a  _email = kakkarj
-00000060: 612e 6769 7468 7562 4067 6d61 696c 2e63  a.github@gmail.c
-00000070: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
-00000080: 3d20 5472 6565 5669 6577 2069 7320 6120  = TreeView is a 
-00000090: 6e6f 7465 2074 616b 696e 6720 7468 6174  note taking that
-000000a0: 2077 7269 7474 656e 2074 6f20 7465 7874   written to text
-000000b0: 2066 696c 6520 616e 6420 7669 6577 2069   file and view i
-000000c0: 6e20 7472 6565 2d76 6965 7720 6f75 746c  n tree-view outl
-000000d0: 696e 652e 0d0a 6c6f 6e67 5f64 6573 6372  ine...long_descr
-000000e0: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
-000000f0: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
-00000100: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
-00000110: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
-00000120: 6172 6b64 6f77 6e0d 0a75 726c 203d 2068  arkdown..url = h
-00000130: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000140: 6d2f 6b61 6b6b 6172 6a61 2f54 560d 0a6c  m/kakkarja/TV..l
-00000150: 6963 656e 7365 203d 2042 5344 3320 4c69  icense = BSD3 Li
-00000160: 6365 6e73 650d 0a63 6c61 7373 6966 6965  cense..classifie
-00000170: 7273 203d 200d 0a09 456e 7669 726f 6e6d  rs = ...Environm
-00000180: 656e 7420 3a3a 2057 696e 3332 2028 4d53  ent :: Win32 (MS
-00000190: 2057 696e 646f 7773 290d 0a09 456e 7669   Windows)...Envi
-000001a0: 726f 6e6d 656e 7420 3a3a 204d 6163 4f53  ronment :: MacOS
-000001b0: 2058 0d0a 0949 6e74 656e 6465 6420 4175   X...Intended Au
-000001c0: 6469 656e 6365 203a 3a20 456e 6420 5573  dience :: End Us
-000001d0: 6572 732f 4465 736b 746f 700d 0a09 546f  ers/Desktop...To
-000001e0: 7069 6320 3a3a 2054 6578 7420 4564 6974  pic :: Text Edit
-000001f0: 6f72 7320 3a3a 2054 6578 7420 5072 6f63  ors :: Text Proc
-00000200: 6573 7369 6e67 0d0a 0950 726f 6772 616d  essing...Program
-00000210: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000220: 2050 7974 686f 6e20 3a3a 2033 2e39 0d0a   Python :: 3.9..
-00000230: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
-00000240: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
-00000250: 4c69 6365 6e73 650d 0a0d 0a5b 6f70 7469  License....[opti
-00000260: 6f6e 735d 0d0a 7061 636b 6167 6573 203d  ons]..packages =
-00000270: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
-00000280: 6571 7569 7265 7320 3d20 3e3d 332e 390d  equires = >=3.9.
-00000290: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-000002a0: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-000002b0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 7472 6565 7669 6577 2d6b 6172 6a61  = treeview-karja
+00000020: 6b61 6b0a 7665 7273 696f 6e20 3d20 312e  kak.version = 1.
+00000030: 382e 3572 6331 0a61 7574 686f 7220 3d20  8.5rc1.author = 
+00000040: 6b61 726a 616b 616b 0a61 7574 686f 725f  karjakak.author_
+00000050: 656d 6169 6c20 3d20 6b61 6b6b 6172 6a61  email = kakkarja
+00000060: 2e67 6974 6875 6240 676d 6169 6c2e 636f  .github@gmail.co
+00000070: 6d0a 6465 7363 7269 7074 696f 6e20 3d20  m.description = 
+00000080: 5472 6565 5669 6577 2069 7320 6120 6e6f  TreeView is a no
+00000090: 7465 2074 616b 696e 6720 7468 6174 2077  te taking that w
+000000a0: 7269 7474 656e 2074 6f20 7465 7874 2066  ritten to text f
+000000b0: 696c 6520 616e 6420 7669 6577 2069 6e20  ile and view in 
+000000c0: 7472 6565 2d76 6965 7720 6f75 746c 696e  tree-view outlin
+000000d0: 652e 0a6c 6f6e 675f 6465 7363 7269 7074  e..long_descript
+000000e0: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
+000000f0: 4d45 2e6d 640a 6c6f 6e67 5f64 6573 6372  ME.md.long_descr
+00000100: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
+00000110: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
+00000120: 6f77 6e0a 7572 6c20 3d20 6874 7470 733a  own.url = https:
+00000130: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 616b  //github.com/kak
+00000140: 6b61 726a 612f 5456 0a6c 6963 656e 7365  karja/TV.license
+00000150: 203d 2042 5344 3320 4c69 6365 6e73 650a   = BSD3 License.
+00000160: 636c 6173 7369 6669 6572 7320 3d20 0a09  classifiers = ..
+00000170: 456e 7669 726f 6e6d 656e 7420 3a3a 2057  Environment :: W
+00000180: 696e 3332 2028 4d53 2057 696e 646f 7773  in32 (MS Windows
+00000190: 290a 0945 6e76 6972 6f6e 6d65 6e74 203a  )..Environment :
+000001a0: 3a20 4d61 634f 5320 580a 0949 6e74 656e  : MacOS X..Inten
+000001b0: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
+000001c0: 456e 6420 5573 6572 732f 4465 736b 746f  End Users/Deskto
+000001d0: 700a 0954 6f70 6963 203a 3a20 5465 7874  p..Topic :: Text
+000001e0: 2045 6469 746f 7273 203a 3a20 5465 7874   Editors :: Text
+000001f0: 2050 726f 6365 7373 696e 670a 0950 726f   Processing..Pro
+00000200: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000210: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000220: 2e39 0a09 4c69 6365 6e73 6520 3a3a 204f  .9..License :: O
+00000230: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
+00000240: 4954 204c 6963 656e 7365 0a0a 5b6f 7074  IT License..[opt
+00000250: 696f 6e73 5d0a 7061 636b 6167 6573 203d  ions].packages =
+00000260: 2066 696e 643a 0a70 7974 686f 6e5f 7265   find:.python_re
+00000270: 7175 6972 6573 203d 203e 3d33 2e31 300a  quires = >=3.10.
+00000280: 0a5b 6567 675f 696e 666f 5d0a 7461 675f  .[egg_info].tag_
+00000290: 6275 696c 6420 3d20 0a74 6167 5f64 6174  build = .tag_dat
+000002a0: 6520 3d20 300a 0a                        e = 0..
```

### Comparing `treeview_karjakak-1.8.5/treeview/dbase/datab.py` & `treeview-karjakak-1.8.5rc1/treeview/dbase/datab.py`

 * *Files identical despite different names*

### Comparing `treeview_karjakak-1.8.5/treeview/treeview.py` & `treeview-karjakak-1.8.5rc1/treeview/treeview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # -*- coding: utf-8 -*-
 # Copyright © kakkarja (K A K)
 
 import datetime
-import locale
 import os
 import re
-from collections.abc import Iterator
+from .dbase import Datab as db, primer
 from itertools import islice
+from typing import Union
 from types import GeneratorType
-from typing import Any, Generator, Union
+import locale
+from collections.abc import Iterator
+from .tvdescript import Parent, ChildsNum, FileName
 
-from .dbase import Datab as db
-from .dbase import primer
-from .tvdescript import ChildsNum, FileName, Parent
 
 __all__ = ("conftv", "TreeView")
 
 
 def conftv(cls, childs=50, space=4):
     """
     Configure Childs with spaces limited from 1 to 10
@@ -72,30 +71,30 @@
     def __exit__(self, type_, value, trace):
         """When exit, all TreeView class properties is cleared."""
 
         if TreeView.filename.store1:
             TreeView.filename.finalize(self.__weakref__)
         return False
 
-    def getdata(self) -> Generator[tuple[int, str], Any, None]:
+    def getdata(self) -> GeneratorType:
         """Get file datas"""
 
         if os.path.exists(f"{self.filename}.txt"):
             with open(f"{self.filename}.txt") as rd:
                 yield from enumerate(rd)
         else:
             raise FileNotFoundError(f"{self.filename}.txt not exist!")
 
     def getdatanum(self) -> int:
         """Len of data"""
 
         return tuple(self.getdata())[-1][0] + 1
 
     @primer
-    def satofi(self, wr: bool = True) -> Generator[None, Any, None]:
+    def satofi(self, wr: bool = True) -> None:
         """Generator writer to file"""
 
         caperr = None
         file = open(f"{self.filename}_", "wb")
         try:
             while True:
                 try:
```

### Comparing `treeview_karjakak-1.8.5/treeview/tvdescript/tvdescript.py` & `treeview-karjakak-1.8.5rc1/treeview/tvdescript/tvdescript.py`

 * *Files identical despite different names*

### Comparing `treeview_karjakak-1.8.5/treeview_karjakak.egg-info/PKG-INFO` & `treeview-karjakak-1.8.5rc1/treeview_karjakak.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,308 +1,308 @@
-Metadata-Version: 2.1
-Name: treeview-karjakak
-Version: 1.8.5
-Summary: TreeView is a note taking that written to text file and view in tree-view outline.
-Home-page: https://github.com/kakkarja/TV
-Author: karjakak
-Author-email: kakkarja.github@gmail.com
-License: BSD3 License
-Classifier: Environment :: Win32 (MS Windows)
-Classifier: Environment :: MacOS X
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Topic :: Text Editors :: Text Processing
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
-# TreeView
-## Writing an outline note with tree-view look.
-
-## Installation
-```
-pip install treeview-karjakak
-```
-## Usage
-```Python
-from treeview import TreeView, conftv
-
-# To configure the childs (by default 50 childs, and 4 spaces)
-TreeView = conftv(TreeView, 5, 1)
-print(dict(TreeView.childs))
-
-w = 'Amazing Grace'
-with TreeView('test') as tv:
-
-    # First time write on note as parent
-    tv.writetree(w)
-
-    # Write it with loop in childs 
-    for i in range(5):
-        tv.quickchild(w, child = f'child{i+1}')
-        
-    # Edit the parent
-    tv.edittree('Amazing Grace, how sweet the sound')
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    
-    # Edit again in row 4 to child2
-    tv.edittree('Mantaaaaaaap!', row = 4, child = 'child2')
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    
-    # Write new parent
-    tv.addparent('Wow good job')
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    
-    # Edit again in row 6 to child5
-    tv.edittree('Wow good job buddy', row = 6, child = 'child5')
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    
-    # Write again new childs
-    tv.quickchild('Totally awesome', child = 'child1')
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    tv.quickchild('This is quick child edit', child = 'child2')
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    tv.quickchild('Thank You', child = 'child1')
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    
-    # Delete row 10
-    tv.delrow(10)
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    
-    # Insert to row 8 as child1
-    tv.insertrow('God bless you', row = 8, child = 'child1' )
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    
-    # Moving position from row 6 to row 4
-    tv.movetree(6, 4)
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    
-    # Moving position of child in row 6 as child1
-    tv.movechild(6, child = 'child1')
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    
-    # Print an iterator to dict
-    pprint(dict(tv.insighttree()))
-    
-    # Create spaces between rows
-    for i in range(1, tv.getdatanum()+4, 2):
-        if i == 15:
-            break
-        tv.insertspace(i)
-    print('-'* 12)
-    tv.readtree()
-    print('-'* 12)
-    pprint(dict(tv.insighttree()))
-    
-    # Backup note as json file
-    tv.backuptv()
-    del tv, w, i
-```
-**Result:**
-```Python
-{'child1': 1, 'child2': 2, 'child3': 3, 'child4': 4, 'child5': 5}
-------------
-Amazing Grace, how sweet the sound:
- -Amazing Grace
-  -Amazing Grace
-   -Amazing Grace
-    -Amazing Grace
-     -Amazing Grace
-------------
-------------
-Amazing Grace, how sweet the sound:
- -Amazing Grace
-  -Amazing Grace
-   -Amazing Grace
-  -Mantaaaaaaap!
-     -Amazing Grace
-------------
-------------
-Amazing Grace, how sweet the sound:
- -Amazing Grace
-  -Amazing Grace
-   -Amazing Grace
-  -Mantaaaaaaap!
-     -Amazing Grace
-
-Wow good job:
-------------
-------------
-Amazing Grace, how sweet the sound:
- -Amazing Grace
-  -Amazing Grace
-   -Amazing Grace
-  -Mantaaaaaaap!
-     -Amazing Grace
-     -Wow good job buddy
-
-Wow good job:
-------------
-------------
-Amazing Grace, how sweet the sound:
- -Amazing Grace
-  -Amazing Grace
-   -Amazing Grace
-  -Mantaaaaaaap!
-     -Amazing Grace
-     -Wow good job buddy
-
-Wow good job:
- -Totally awesome
-------------
-------------
-Amazing Grace, how sweet the sound:
- -Amazing Grace
-  -Amazing Grace
-   -Amazing Grace
-  -Mantaaaaaaap!
-     -Amazing Grace
-     -Wow good job buddy
-
-Wow good job:
- -Totally awesome
-  -This is quick child edit
-------------
-------------
-Amazing Grace, how sweet the sound:
- -Amazing Grace
-  -Amazing Grace
-   -Amazing Grace
-  -Mantaaaaaaap!
-     -Amazing Grace
-     -Wow good job buddy
-
-Wow good job:
- -Totally awesome
-  -This is quick child edit
- -Thank You
-------------
-------------
-Amazing Grace, how sweet the sound:
- -Amazing Grace
-  -Amazing Grace
-   -Amazing Grace
-  -Mantaaaaaaap!
-     -Amazing Grace
-     -Wow good job buddy
-
-Wow good job:
- -Totally awesome
- -Thank You
-------------
-------------
-Amazing Grace, how sweet the sound:
- -Amazing Grace
-  -Amazing Grace
-   -Amazing Grace
-  -Mantaaaaaaap!
-     -Amazing Grace
-     -Wow good job buddy
- -God bless you
-
-Wow good job:
- -Totally awesome
- -Thank You
-------------
-------------
-Amazing Grace, how sweet the sound:
- -Amazing Grace
-  -Amazing Grace
-   -Amazing Grace
-     -Wow good job buddy
-  -Mantaaaaaaap!
-     -Amazing Grace
- -God bless you
-
-Wow good job:
- -Totally awesome
- -Thank You
-------------
-------------
-Amazing Grace, how sweet the sound:
- -Amazing Grace
-  -Amazing Grace
-   -Amazing Grace
-     -Wow good job buddy
-  -Mantaaaaaaap!
- -Amazing Grace
- -God bless you
-
-Wow good job:
- -Totally awesome
- -Thank You
-------------
-{0: ('parent', 'Amazing Grace, how sweet the sound:\n'),
- 1: ('child1', '-Amazing Grace\n'),
- 2: ('child2', '-Amazing Grace\n'),
- 3: ('child3', '-Amazing Grace\n'),
- 4: ('child5', '-Wow good job buddy\n'),
- 5: ('child2', '-Mantaaaaaaap!\n'),
- 6: ('child1', '-Amazing Grace\n'),
- 7: ('child1', '-God bless you\n'),
- 8: ('space', '\n'),
- 9: ('parent', 'Wow good job:\n'),
- 10: ('child1', '-Totally awesome\n'),
- 11: ('child1', '-Thank You\n')}
-------------
-Amazing Grace, how sweet the sound:
-
- -Amazing Grace
-
-  -Amazing Grace
-
-   -Amazing Grace
-
-     -Wow good job buddy
-
-  -Mantaaaaaaap!
-
- -Amazing Grace
-
- -God bless you
-
-Wow good job:
- -Totally awesome
- -Thank You
-------------
-{0: ('parent', 'Amazing Grace, how sweet the sound:\n'),
- 1: ('space', '\n'),
- 2: ('child1', '-Amazing Grace\n'),
- 3: ('space', '\n'),
- 4: ('child2', '-Amazing Grace\n'),
- 5: ('space', '\n'),
- 6: ('child3', '-Amazing Grace\n'),
- 7: ('space', '\n'),
- 8: ('child5', '-Wow good job buddy\n'),
- 9: ('space', '\n'),
- 10: ('child2', '-Mantaaaaaaap!\n'),
- 11: ('space', '\n'),
- 12: ('child1', '-Amazing Grace\n'),
- 13: ('space', '\n'),
- 14: ('child1', '-God bless you\n'),
- 15: ('space', '\n'),
- 16: ('parent', 'Wow good job:\n'),
- 17: ('child1', '-Totally awesome\n'),
- 18: ('child1', '-Thank You\n')}
-```
+Metadata-Version: 2.1
+Name: treeview-karjakak
+Version: 1.8.5rc1
+Summary: TreeView is a note taking that written to text file and view in tree-view outline.
+Home-page: https://github.com/kakkarja/TV
+Author: karjakak
+Author-email: kakkarja.github@gmail.com
+License: BSD3 License
+Classifier: Environment :: Win32 (MS Windows)
+Classifier: Environment :: MacOS X
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Topic :: Text Editors :: Text Processing
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+
+# TreeView
+## Writing an outline note with tree-view look.
+
+## Installation
+```
+pip install treeview-karjakak
+```
+## Usage
+```Python
+from treeview import TreeView, conftv
+
+# To configure the childs (by default 50 childs, and 4 spaces)
+TreeView = conftv(TreeView, 5, 1)
+print(dict(TreeView.childs))
+
+w = 'Amazing Grace'
+with TreeView('test') as tv:
+
+    # First time write on note as parent
+    tv.writetree(w)
+
+    # Write it with loop in childs 
+    for i in range(5):
+        tv.quickchild(w, child = f'child{i+1}')
+        
+    # Edit the parent
+    tv.edittree('Amazing Grace, how sweet the sound')
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    
+    # Edit again in row 4 to child2
+    tv.edittree('Mantaaaaaaap!', row = 4, child = 'child2')
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    
+    # Write new parent
+    tv.addparent('Wow good job')
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    
+    # Edit again in row 6 to child5
+    tv.edittree('Wow good job buddy', row = 6, child = 'child5')
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    
+    # Write again new childs
+    tv.quickchild('Totally awesome', child = 'child1')
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    tv.quickchild('This is quick child edit', child = 'child2')
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    tv.quickchild('Thank You', child = 'child1')
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    
+    # Delete row 10
+    tv.delrow(10)
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    
+    # Insert to row 8 as child1
+    tv.insertrow('God bless you', row = 8, child = 'child1' )
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    
+    # Moving position from row 6 to row 4
+    tv.movetree(6, 4)
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    
+    # Moving position of child in row 6 as child1
+    tv.movechild(6, child = 'child1')
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    
+    # Print an iterator to dict
+    pprint(dict(tv.insighttree()))
+    
+    # Create spaces between rows
+    for i in range(1, tv.getdatanum()+4, 2):
+        if i == 15:
+            break
+        tv.insertspace(i)
+    print('-'* 12)
+    tv.readtree()
+    print('-'* 12)
+    pprint(dict(tv.insighttree()))
+    
+    # Backup note as json file
+    tv.backuptv()
+    del tv, w, i
+```
+**Result:**
+```Python
+{'child1': 1, 'child2': 2, 'child3': 3, 'child4': 4, 'child5': 5}
+------------
+Amazing Grace, how sweet the sound:
+ -Amazing Grace
+  -Amazing Grace
+   -Amazing Grace
+    -Amazing Grace
+     -Amazing Grace
+------------
+------------
+Amazing Grace, how sweet the sound:
+ -Amazing Grace
+  -Amazing Grace
+   -Amazing Grace
+  -Mantaaaaaaap!
+     -Amazing Grace
+------------
+------------
+Amazing Grace, how sweet the sound:
+ -Amazing Grace
+  -Amazing Grace
+   -Amazing Grace
+  -Mantaaaaaaap!
+     -Amazing Grace
+
+Wow good job:
+------------
+------------
+Amazing Grace, how sweet the sound:
+ -Amazing Grace
+  -Amazing Grace
+   -Amazing Grace
+  -Mantaaaaaaap!
+     -Amazing Grace
+     -Wow good job buddy
+
+Wow good job:
+------------
+------------
+Amazing Grace, how sweet the sound:
+ -Amazing Grace
+  -Amazing Grace
+   -Amazing Grace
+  -Mantaaaaaaap!
+     -Amazing Grace
+     -Wow good job buddy
+
+Wow good job:
+ -Totally awesome
+------------
+------------
+Amazing Grace, how sweet the sound:
+ -Amazing Grace
+  -Amazing Grace
+   -Amazing Grace
+  -Mantaaaaaaap!
+     -Amazing Grace
+     -Wow good job buddy
+
+Wow good job:
+ -Totally awesome
+  -This is quick child edit
+------------
+------------
+Amazing Grace, how sweet the sound:
+ -Amazing Grace
+  -Amazing Grace
+   -Amazing Grace
+  -Mantaaaaaaap!
+     -Amazing Grace
+     -Wow good job buddy
+
+Wow good job:
+ -Totally awesome
+  -This is quick child edit
+ -Thank You
+------------
+------------
+Amazing Grace, how sweet the sound:
+ -Amazing Grace
+  -Amazing Grace
+   -Amazing Grace
+  -Mantaaaaaaap!
+     -Amazing Grace
+     -Wow good job buddy
+
+Wow good job:
+ -Totally awesome
+ -Thank You
+------------
+------------
+Amazing Grace, how sweet the sound:
+ -Amazing Grace
+  -Amazing Grace
+   -Amazing Grace
+  -Mantaaaaaaap!
+     -Amazing Grace
+     -Wow good job buddy
+ -God bless you
+
+Wow good job:
+ -Totally awesome
+ -Thank You
+------------
+------------
+Amazing Grace, how sweet the sound:
+ -Amazing Grace
+  -Amazing Grace
+   -Amazing Grace
+     -Wow good job buddy
+  -Mantaaaaaaap!
+     -Amazing Grace
+ -God bless you
+
+Wow good job:
+ -Totally awesome
+ -Thank You
+------------
+------------
+Amazing Grace, how sweet the sound:
+ -Amazing Grace
+  -Amazing Grace
+   -Amazing Grace
+     -Wow good job buddy
+  -Mantaaaaaaap!
+ -Amazing Grace
+ -God bless you
+
+Wow good job:
+ -Totally awesome
+ -Thank You
+------------
+{0: ('parent', 'Amazing Grace, how sweet the sound:\n'),
+ 1: ('child1', '-Amazing Grace\n'),
+ 2: ('child2', '-Amazing Grace\n'),
+ 3: ('child3', '-Amazing Grace\n'),
+ 4: ('child5', '-Wow good job buddy\n'),
+ 5: ('child2', '-Mantaaaaaaap!\n'),
+ 6: ('child1', '-Amazing Grace\n'),
+ 7: ('child1', '-God bless you\n'),
+ 8: ('space', '\n'),
+ 9: ('parent', 'Wow good job:\n'),
+ 10: ('child1', '-Totally awesome\n'),
+ 11: ('child1', '-Thank You\n')}
+------------
+Amazing Grace, how sweet the sound:
+
+ -Amazing Grace
+
+  -Amazing Grace
+
+   -Amazing Grace
+
+     -Wow good job buddy
+
+  -Mantaaaaaaap!
+
+ -Amazing Grace
+
+ -God bless you
+
+Wow good job:
+ -Totally awesome
+ -Thank You
+------------
+{0: ('parent', 'Amazing Grace, how sweet the sound:\n'),
+ 1: ('space', '\n'),
+ 2: ('child1', '-Amazing Grace\n'),
+ 3: ('space', '\n'),
+ 4: ('child2', '-Amazing Grace\n'),
+ 5: ('space', '\n'),
+ 6: ('child3', '-Amazing Grace\n'),
+ 7: ('space', '\n'),
+ 8: ('child5', '-Wow good job buddy\n'),
+ 9: ('space', '\n'),
+ 10: ('child2', '-Mantaaaaaaap!\n'),
+ 11: ('space', '\n'),
+ 12: ('child1', '-Amazing Grace\n'),
+ 13: ('space', '\n'),
+ 14: ('child1', '-God bless you\n'),
+ 15: ('space', '\n'),
+ 16: ('parent', 'Wow good job:\n'),
+ 17: ('child1', '-Totally awesome\n'),
+ 18: ('child1', '-Thank You\n')}
+```
```

