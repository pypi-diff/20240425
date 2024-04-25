# Comparing `tmp/sphinxcontrib-getstart-sphinx-1.1.0.tar.gz` & `tmp/sphinxcontrib-getstart-sphinx-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-getstart-sphinx-1.1.0.tar", last modified: Sat May  1 08:51:49 2021, max compression
+gzip compressed data, was "sphinxcontrib-getstart-sphinx-1.2.0.tar", last modified: Thu Apr 25 08:14:11 2024, max compression
```

## Comparing `sphinxcontrib-getstart-sphinx-1.1.0.tar` & `sphinxcontrib-getstart-sphinx-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-01 08:51:49.979219 sphinxcontrib-getstart-sphinx-1.1.0/
--rw-r--r--   0 tkomiya    (502) staff       (20)     4239 2021-05-01 08:51:49.979507 sphinxcontrib-getstart-sphinx-1.1.0/PKG-INFO
--rw-r--r--   0 tkomiya    (502) staff       (20)     2729 2021-05-01 08:40:43.000000 sphinxcontrib-getstart-sphinx-1.1.0/README.rst
--rw-r--r--   0 tkomiya    (502) staff       (20)      266 2021-05-01 08:51:49.980225 sphinxcontrib-getstart-sphinx-1.1.0/setup.cfg
--rw-r--r--   0 tkomiya    (502) staff       (20)     1201 2021-05-01 08:51:01.000000 sphinxcontrib-getstart-sphinx-1.1.0/setup.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-01 08:51:49.975380 sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib/
--rw-r--r--   0 tkomiya    (502) staff       (20)       80 2021-05-01 08:40:43.000000 sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib/__init__.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-01 08:51:49.977096 sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib/getstart_sphinx/
--rw-r--r--   0 tkomiya    (502) staff       (20)      508 2021-05-01 08:40:43.000000 sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib/getstart_sphinx/__init__.py
--rw-r--r--   0 tkomiya    (502) staff       (20)     3927 2021-05-01 08:40:43.000000 sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib/getstart_sphinx/better_docref.py
--rw-r--r--   0 tkomiya    (502) staff       (20)     2166 2021-05-01 08:40:43.000000 sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib/getstart_sphinx/column.py
--rw-r--r--   0 tkomiya    (502) staff       (20)     1191 2021-05-01 08:40:43.000000 sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib/getstart_sphinx/footnote_relocator.py
--rw-r--r--   0 tkomiya    (502) staff       (20)      722 2021-05-01 08:40:43.000000 sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib/getstart_sphinx/glossary_decorator.py
--rw-r--r--   0 tkomiya    (502) staff       (20)      783 2021-05-01 08:38:20.000000 sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib/getstart_sphinx/oreilly_review_table.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-01 08:51:49.978921 sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib_getstart_sphinx.egg-info/
--rw-r--r--   0 tkomiya    (502) staff       (20)     4239 2021-05-01 08:51:49.000000 sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib_getstart_sphinx.egg-info/PKG-INFO
--rw-r--r--   0 tkomiya    (502) staff       (20)      720 2021-05-01 08:51:49.000000 sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib_getstart_sphinx.egg-info/SOURCES.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)        1 2021-05-01 08:51:49.000000 sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib_getstart_sphinx.egg-info/dependency_links.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)       14 2021-05-01 08:51:49.000000 sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib_getstart_sphinx.egg-info/namespace_packages.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)        1 2021-05-01 08:51:49.000000 sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib_getstart_sphinx.egg-info/not-zip-safe
--rw-r--r--   0 tkomiya    (502) staff       (20)       47 2021-05-01 08:51:49.000000 sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib_getstart_sphinx.egg-info/requires.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)       14 2021-05-01 08:51:49.000000 sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib_getstart_sphinx.egg-info/top_level.txt
+drwxr-xr-x   0 tkomiya    (501) staff       (20)        0 2024-04-25 08:14:11.165734 sphinxcontrib-getstart-sphinx-1.2.0/
+-rw-r--r--   0 tkomiya    (501) staff       (20)     3599 2024-04-25 08:14:11.165372 sphinxcontrib-getstart-sphinx-1.2.0/PKG-INFO
+-rw-r--r--   0 tkomiya    (501) staff       (20)     2729 2024-04-20 07:07:49.000000 sphinxcontrib-getstart-sphinx-1.2.0/README.rst
+-rw-r--r--   0 tkomiya    (501) staff       (20)      266 2024-04-25 08:14:11.168252 sphinxcontrib-getstart-sphinx-1.2.0/setup.cfg
+-rw-r--r--   0 tkomiya    (501) staff       (20)     1201 2024-04-25 08:12:53.000000 sphinxcontrib-getstart-sphinx-1.2.0/setup.py
+drwxr-xr-x   0 tkomiya    (501) staff       (20)        0 2024-04-25 08:14:11.138471 sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib/
+-rw-r--r--   0 tkomiya    (501) staff       (20)       80 2024-04-20 07:07:49.000000 sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib/__init__.py
+drwxr-xr-x   0 tkomiya    (501) staff       (20)        0 2024-04-25 08:14:11.150653 sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib/getstart_sphinx/
+-rw-r--r--   0 tkomiya    (501) staff       (20)      508 2024-04-20 07:07:49.000000 sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib/getstart_sphinx/__init__.py
+-rw-r--r--   0 tkomiya    (501) staff       (20)     3927 2024-04-20 07:07:49.000000 sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib/getstart_sphinx/better_docref.py
+-rw-r--r--   0 tkomiya    (501) staff       (20)     2833 2024-04-25 08:12:39.000000 sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib/getstart_sphinx/column.py
+-rw-r--r--   0 tkomiya    (501) staff       (20)     1191 2024-04-20 07:07:49.000000 sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib/getstart_sphinx/footnote_relocator.py
+-rw-r--r--   0 tkomiya    (501) staff       (20)      722 2024-04-20 07:07:49.000000 sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib/getstart_sphinx/glossary_decorator.py
+-rw-r--r--   0 tkomiya    (501) staff       (20)      783 2024-04-20 07:07:49.000000 sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib/getstart_sphinx/oreilly_review_table.py
+drwxr-xr-x   0 tkomiya    (501) staff       (20)        0 2024-04-25 08:14:11.164180 sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib_getstart_sphinx.egg-info/
+-rw-r--r--   0 tkomiya    (501) staff       (20)     3599 2024-04-25 08:14:11.000000 sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib_getstart_sphinx.egg-info/PKG-INFO
+-rw-r--r--   0 tkomiya    (501) staff       (20)      720 2024-04-25 08:14:11.000000 sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib_getstart_sphinx.egg-info/SOURCES.txt
+-rw-r--r--   0 tkomiya    (501) staff       (20)        1 2024-04-25 08:14:11.000000 sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib_getstart_sphinx.egg-info/dependency_links.txt
+-rw-r--r--   0 tkomiya    (501) staff       (20)       14 2024-04-25 08:14:11.000000 sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib_getstart_sphinx.egg-info/namespace_packages.txt
+-rw-r--r--   0 tkomiya    (501) staff       (20)        1 2024-04-25 08:14:11.000000 sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib_getstart_sphinx.egg-info/not-zip-safe
+-rw-r--r--   0 tkomiya    (501) staff       (20)       47 2024-04-25 08:14:11.000000 sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib_getstart_sphinx.egg-info/requires.txt
+-rw-r--r--   0 tkomiya    (501) staff       (20)       14 2024-04-25 08:14:11.000000 sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib_getstart_sphinx.egg-info/top_level.txt
```

### Comparing `sphinxcontrib-getstart-sphinx-1.1.0/PKG-INFO` & `sphinxcontrib-getstart-sphinx-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,109 +1,111 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: sphinxcontrib-getstart-sphinx
-Version: 1.1.0
+Version: 1.2.0
 Summary: Sphinx extensions for "Getting Started with Sphinx 2nd Edition"
 Home-page: https://github.com/getstart-sphinx/sphinxcontrib-getstart-sphinx
 Author: Takeshi KOMIYA
 Author-email: i.tkomiya@gmail.com
 License: BSD
-Description: sphinxcontrib-getstart-sphinx
-        =============================
-        
-        ``sphinxcontrib-getstart-sphinx`` is a collection of Sphinx extensions to
-        build `Sphinxをはじめよう 第2版 (Getting Started with Sphinx 2nd Edition)`__.
-        
-        __ https://www.oreilly.co.jp/books/9784873118192/
-        
-        
-        This package provides following extensions:
-        
-        ``sphinxcontrib.getstart_sphinx.better_docref``
-            Append section numbers to each ``:doc:`` references.
-        
-        ``sphinxcontrib.getstart_sphinx.column``
-            Add ``column`` directive to note columns.
-        
-        ``sphinxcontrib.getstart_sphinx.footnote_relocator``
-            Move footnote definitions to the bottom of each sections.
-        
-        ``sphinxcontrib.getstart_sphinx.glossary_decorator``
-            Make terms of glossaries bold.
-        
-        ``sphinxcontrib.getstart_sphinx.oreilly_review_table``
-            Convert tables in Re:VIEW output to original notation for
-            O'Reilly Japan internal tools.
-        
-        
-        Usage
-        -----
-        
-        To enable all extensions in this package, please add
-        ``sphinxcontrib.getstart_sphinx`` to your ``extensions`` list in conf.py::
-        
-            extensions = ['sphinxcontrib.getstart_sphinx']
-        
-        If you want to enable specific extensions individually, please add its
-        name to the list like bollow::
-        
-            extensions = ['sphinxcontrib.getstart_sphinx.better_docref',
-                          'sphinxcontrib.getstart_sphinx.footnote_relocator']
-        
-        Directives
-        ----------
-        
-        You can use following directives:
-        
-        ``column``
-            A directive to note a column.  It takes a title of column as an argument,
-            and also takes body of column as content block.
-        
-            Example::
-        
-                .. column:: SphinxとPythonのバージョンの関係
-        
-                   バージョン1.5以降、Sphinxを動作させるには2.7もしくは3.4以上の
-                   Pythonが必要です。
-                   そのため、古いPythonがインストールされるCentOS 6.x系などのディスト
-                   リビューションでは、最新のSphinxが利用できません。
-        
-        
-        Settings
-        --------
-        
-        You can configure following settings to arrange the behavior of the extension.
-        
-        ``section_numbers``:
-            A dict for mapping docname to section number text.
-            This is used by ``better_docref`` extension to build a link title
-            for document reference.
-        
-            Example::
-        
-                section_numbers = {
-                    'ch01': '第1章',
-                    'ch02': '第2章',
-                    'ch03': '第3章',
-                    'ch04': '第4章',
-                    'ch05': '第5章',
-                    'ch06': '第6章',
-                    'appendix/references': '付録A',
-                    'appendix/builders': '付録B',
-                    'appendix/quickstart': '付録C',
-                    'appendix/texlive': '付録D',
-                    'appendix/make_sh': '付録E',
-                    'appendix/markdown': '付録F',
-                    'appendix/community': '付録G',
-                }
-        
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
+Requires-Dist: Sphinx>=2.0
+Requires-Dist: sphinxcontrib-reviewbuilder>=0.0.8
+
+sphinxcontrib-getstart-sphinx
+=============================
+
+``sphinxcontrib-getstart-sphinx`` is a collection of Sphinx extensions to
+build `Sphinxをはじめよう 第2版 (Getting Started with Sphinx 2nd Edition)`__.
+
+__ https://www.oreilly.co.jp/books/9784873118192/
+
+
+This package provides following extensions:
+
+``sphinxcontrib.getstart_sphinx.better_docref``
+    Append section numbers to each ``:doc:`` references.
+
+``sphinxcontrib.getstart_sphinx.column``
+    Add ``column`` directive to note columns.
+
+``sphinxcontrib.getstart_sphinx.footnote_relocator``
+    Move footnote definitions to the bottom of each sections.
+
+``sphinxcontrib.getstart_sphinx.glossary_decorator``
+    Make terms of glossaries bold.
+
+``sphinxcontrib.getstart_sphinx.oreilly_review_table``
+    Convert tables in Re:VIEW output to original notation for
+    O'Reilly Japan internal tools.
+
+
+Usage
+-----
+
+To enable all extensions in this package, please add
+``sphinxcontrib.getstart_sphinx`` to your ``extensions`` list in conf.py::
+
+    extensions = ['sphinxcontrib.getstart_sphinx']
+
+If you want to enable specific extensions individually, please add its
+name to the list like bollow::
+
+    extensions = ['sphinxcontrib.getstart_sphinx.better_docref',
+                  'sphinxcontrib.getstart_sphinx.footnote_relocator']
+
+Directives
+----------
+
+You can use following directives:
+
+``column``
+    A directive to note a column.  It takes a title of column as an argument,
+    and also takes body of column as content block.
+
+    Example::
+
+        .. column:: SphinxとPythonのバージョンの関係
+
+           バージョン1.5以降、Sphinxを動作させるには2.7もしくは3.4以上の
+           Pythonが必要です。
+           そのため、古いPythonがインストールされるCentOS 6.x系などのディスト
+           リビューションでは、最新のSphinxが利用できません。
+
+
+Settings
+--------
+
+You can configure following settings to arrange the behavior of the extension.
+
+``section_numbers``:
+    A dict for mapping docname to section number text.
+    This is used by ``better_docref`` extension to build a link title
+    for document reference.
+
+    Example::
+
+        section_numbers = {
+            'ch01': '第1章',
+            'ch02': '第2章',
+            'ch03': '第3章',
+            'ch04': '第4章',
+            'ch05': '第5章',
+            'ch06': '第6章',
+            'appendix/references': '付録A',
+            'appendix/builders': '付録B',
+            'appendix/quickstart': '付録C',
+            'appendix/texlive': '付録D',
+            'appendix/make_sh': '付録E',
+            'appendix/markdown': '付録F',
+            'appendix/community': '付録G',
+        }
```

### Comparing `sphinxcontrib-getstart-sphinx-1.1.0/README.rst` & `sphinxcontrib-getstart-sphinx-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-getstart-sphinx-1.1.0/setup.py` & `sphinxcontrib-getstart-sphinx-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 long_desc = open('README.rst').read()
 
 requires = ['Sphinx>=2.0', 'sphinxcontrib-reviewbuilder>=0.0.8']
 
 setup(
     name='sphinxcontrib-getstart-sphinx',
-    version='1.1.0',
+    version='1.2.0',
     url='https://github.com/getstart-sphinx/sphinxcontrib-getstart-sphinx',
     license='BSD',
     author='Takeshi KOMIYA',
     author_email='i.tkomiya@gmail.com',
     description='Sphinx extensions for "Getting Started with Sphinx 2nd Edition"',
     long_description=long_desc,
     zip_safe=False,
```

### Comparing `sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib/getstart_sphinx/better_docref.py` & `sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib/getstart_sphinx/better_docref.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib/getstart_sphinx/column.py` & `sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib/getstart_sphinx/column.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 
 from docutils import nodes
 from docutils.parsers.rst.directives.admonitions import Admonition
+from sphinx.transforms import SphinxTransform
 
 
 BLOCK_LEVEL_NODES = (
     nodes.literal_block,
     nodes.table,
 )
 
@@ -36,14 +37,16 @@
         r[0]['title'] = self.arguments[0]
         r[0]['name'] = self.name
         return r
 
 
 
 def visit_column(self, node):
+    if node['title']:
+        node.insert(0, nodes.title(node['title'], node['title']))
     self.visit_admonition(node)
 
 
 def depart_column(self, node):
     self.depart_admonition(node)
 
 
@@ -63,13 +66,26 @@
 def review_depart_column(self, node):
     if any(node.traverse(lambda n: isinstance(n, BLOCK_LEVEL_NODES))):
         self.add_text('//raw[|html|</div>]\n\n')
     else:
         self.add_text('=====[/column]\n\n')
 
 
+class ColumnTitleCollector(SphinxTransform):
+    default_priority = 900  # after processing documents by Sphinx Domains
+
+    def apply(self, **kwargs):
+        std_domain = self.env.get_domain('std')
+        for node in self.document.findall(column):
+            for name in node['names']:
+                if name not in std_domain.labels:
+                    node_id = self.document.nameids[name]
+                    std_domain.labels[name] = (self.env.docname, node_id, node['title'])
+
+
 def setup(app):
     app.add_node(column,
                  html=(visit_column, depart_column),
                  latex=(visit_column, depart_column),
                  text=(review_visit_column, review_depart_column))
     app.add_directive('column', ColumnDirective)
+    app.add_transform(ColumnTitleCollector)
```

### Comparing `sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib/getstart_sphinx/footnote_relocator.py` & `sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib/getstart_sphinx/footnote_relocator.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib/getstart_sphinx/glossary_decorator.py` & `sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib/getstart_sphinx/glossary_decorator.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib/getstart_sphinx/oreilly_review_table.py` & `sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib/getstart_sphinx/oreilly_review_table.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib_getstart_sphinx.egg-info/PKG-INFO` & `sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib_getstart_sphinx.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,109 +1,111 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: sphinxcontrib-getstart-sphinx
-Version: 1.1.0
+Version: 1.2.0
 Summary: Sphinx extensions for "Getting Started with Sphinx 2nd Edition"
 Home-page: https://github.com/getstart-sphinx/sphinxcontrib-getstart-sphinx
 Author: Takeshi KOMIYA
 Author-email: i.tkomiya@gmail.com
 License: BSD
-Description: sphinxcontrib-getstart-sphinx
-        =============================
-        
-        ``sphinxcontrib-getstart-sphinx`` is a collection of Sphinx extensions to
-        build `Sphinxをはじめよう 第2版 (Getting Started with Sphinx 2nd Edition)`__.
-        
-        __ https://www.oreilly.co.jp/books/9784873118192/
-        
-        
-        This package provides following extensions:
-        
-        ``sphinxcontrib.getstart_sphinx.better_docref``
-            Append section numbers to each ``:doc:`` references.
-        
-        ``sphinxcontrib.getstart_sphinx.column``
-            Add ``column`` directive to note columns.
-        
-        ``sphinxcontrib.getstart_sphinx.footnote_relocator``
-            Move footnote definitions to the bottom of each sections.
-        
-        ``sphinxcontrib.getstart_sphinx.glossary_decorator``
-            Make terms of glossaries bold.
-        
-        ``sphinxcontrib.getstart_sphinx.oreilly_review_table``
-            Convert tables in Re:VIEW output to original notation for
-            O'Reilly Japan internal tools.
-        
-        
-        Usage
-        -----
-        
-        To enable all extensions in this package, please add
-        ``sphinxcontrib.getstart_sphinx`` to your ``extensions`` list in conf.py::
-        
-            extensions = ['sphinxcontrib.getstart_sphinx']
-        
-        If you want to enable specific extensions individually, please add its
-        name to the list like bollow::
-        
-            extensions = ['sphinxcontrib.getstart_sphinx.better_docref',
-                          'sphinxcontrib.getstart_sphinx.footnote_relocator']
-        
-        Directives
-        ----------
-        
-        You can use following directives:
-        
-        ``column``
-            A directive to note a column.  It takes a title of column as an argument,
-            and also takes body of column as content block.
-        
-            Example::
-        
-                .. column:: SphinxとPythonのバージョンの関係
-        
-                   バージョン1.5以降、Sphinxを動作させるには2.7もしくは3.4以上の
-                   Pythonが必要です。
-                   そのため、古いPythonがインストールされるCentOS 6.x系などのディスト
-                   リビューションでは、最新のSphinxが利用できません。
-        
-        
-        Settings
-        --------
-        
-        You can configure following settings to arrange the behavior of the extension.
-        
-        ``section_numbers``:
-            A dict for mapping docname to section number text.
-            This is used by ``better_docref`` extension to build a link title
-            for document reference.
-        
-            Example::
-        
-                section_numbers = {
-                    'ch01': '第1章',
-                    'ch02': '第2章',
-                    'ch03': '第3章',
-                    'ch04': '第4章',
-                    'ch05': '第5章',
-                    'ch06': '第6章',
-                    'appendix/references': '付録A',
-                    'appendix/builders': '付録B',
-                    'appendix/quickstart': '付録C',
-                    'appendix/texlive': '付録D',
-                    'appendix/make_sh': '付録E',
-                    'appendix/markdown': '付録F',
-                    'appendix/community': '付録G',
-                }
-        
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
+Requires-Dist: Sphinx>=2.0
+Requires-Dist: sphinxcontrib-reviewbuilder>=0.0.8
+
+sphinxcontrib-getstart-sphinx
+=============================
+
+``sphinxcontrib-getstart-sphinx`` is a collection of Sphinx extensions to
+build `Sphinxをはじめよう 第2版 (Getting Started with Sphinx 2nd Edition)`__.
+
+__ https://www.oreilly.co.jp/books/9784873118192/
+
+
+This package provides following extensions:
+
+``sphinxcontrib.getstart_sphinx.better_docref``
+    Append section numbers to each ``:doc:`` references.
+
+``sphinxcontrib.getstart_sphinx.column``
+    Add ``column`` directive to note columns.
+
+``sphinxcontrib.getstart_sphinx.footnote_relocator``
+    Move footnote definitions to the bottom of each sections.
+
+``sphinxcontrib.getstart_sphinx.glossary_decorator``
+    Make terms of glossaries bold.
+
+``sphinxcontrib.getstart_sphinx.oreilly_review_table``
+    Convert tables in Re:VIEW output to original notation for
+    O'Reilly Japan internal tools.
+
+
+Usage
+-----
+
+To enable all extensions in this package, please add
+``sphinxcontrib.getstart_sphinx`` to your ``extensions`` list in conf.py::
+
+    extensions = ['sphinxcontrib.getstart_sphinx']
+
+If you want to enable specific extensions individually, please add its
+name to the list like bollow::
+
+    extensions = ['sphinxcontrib.getstart_sphinx.better_docref',
+                  'sphinxcontrib.getstart_sphinx.footnote_relocator']
+
+Directives
+----------
+
+You can use following directives:
+
+``column``
+    A directive to note a column.  It takes a title of column as an argument,
+    and also takes body of column as content block.
+
+    Example::
+
+        .. column:: SphinxとPythonのバージョンの関係
+
+           バージョン1.5以降、Sphinxを動作させるには2.7もしくは3.4以上の
+           Pythonが必要です。
+           そのため、古いPythonがインストールされるCentOS 6.x系などのディスト
+           リビューションでは、最新のSphinxが利用できません。
+
+
+Settings
+--------
+
+You can configure following settings to arrange the behavior of the extension.
+
+``section_numbers``:
+    A dict for mapping docname to section number text.
+    This is used by ``better_docref`` extension to build a link title
+    for document reference.
+
+    Example::
+
+        section_numbers = {
+            'ch01': '第1章',
+            'ch02': '第2章',
+            'ch03': '第3章',
+            'ch04': '第4章',
+            'ch05': '第5章',
+            'ch06': '第6章',
+            'appendix/references': '付録A',
+            'appendix/builders': '付録B',
+            'appendix/quickstart': '付録C',
+            'appendix/texlive': '付録D',
+            'appendix/make_sh': '付録E',
+            'appendix/markdown': '付録F',
+            'appendix/community': '付録G',
+        }
```

### Comparing `sphinxcontrib-getstart-sphinx-1.1.0/sphinxcontrib_getstart_sphinx.egg-info/SOURCES.txt` & `sphinxcontrib-getstart-sphinx-1.2.0/sphinxcontrib_getstart_sphinx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

