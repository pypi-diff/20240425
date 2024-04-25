# Comparing `tmp/feno-0.2.1.tar.gz` & `tmp/feno-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feno-0.2.1.tar", last modified: Fri Apr 19 14:05:38 2024, max compression
+gzip compressed data, was "feno-0.2.2.tar", last modified: Thu Apr 25 14:39:42 2024, max compression
```

## Comparing `feno-0.2.1.tar` & `feno-0.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-19 14:05:38.800307 feno-0.2.1/
--rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.2.1/LICENSE
--rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.2.1/MANIFEST.in
--rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-19 14:05:38.800307 feno-0.2.1/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)     1471 2024-04-05 00:38:35.000000 feno-0.2.1/README.md
--rw-r--r--   0 lion      (1000) lion      (1000)     1300 2024-04-19 14:05:20.000000 feno-0.2.1/changelog.md
--rw-r--r--   0 lion      (1000) lion      (1000)      306 2024-04-04 23:06:44.000000 feno-0.2.1/requirements.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-19 14:05:38.800307 feno-0.2.1/setup.cfg
--rw-r--r--   0 lion      (1000) lion      (1000)     3157 2024-04-08 22:42:29.000000 feno-0.2.1/setup.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-19 14:05:38.780307 feno-0.2.1/src/
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-19 14:05:38.793640 feno-0.2.1/src/feno/
--rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-19 14:04:46.000000 feno-0.2.1/src/feno/__init__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2273 2024-04-08 17:24:02.000000 feno-0.2.1/src/feno/__main__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5271 2024-04-08 17:22:14.000000 feno-0.2.1/src/feno/actions.py
--rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.2.1/src/feno/cases.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.2.1/src/feno/check.py
--rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.2.1/src/feno/css_style.py
--rw-r--r--   0 lion      (1000) lion      (1000)     9189 2024-04-19 14:04:18.000000 feno-0.2.1/src/feno/filter.py
--rw-r--r--   0 lion      (1000) lion      (1000)     8925 2024-04-06 20:37:55.000000 feno-0.2.1/src/feno/html.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4378 2024-04-08 17:28:46.000000 feno-0.2.1/src/feno/indexer.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3503 2024-04-05 00:31:13.000000 feno-0.2.1/src/feno/jsontools.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4907 2024-04-08 23:40:15.000000 feno-0.2.1/src/feno/lock.py
--rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.2.1/src/feno/log.py
--rw-r--r--   0 lion      (1000) lion      (1000)    11894 2024-04-08 15:58:02.000000 feno-0.2.1/src/feno/mdpp.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4976 2024-04-04 23:15:36.000000 feno-0.2.1/src/feno/remote_md.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-19 14:05:38.796974 feno-0.2.1/src/feno.egg-info/
--rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-19 14:05:38.000000 feno-0.2.1/src/feno.egg-info/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)      542 2024-04-19 14:05:38.000000 feno-0.2.1/src/feno.egg-info/SOURCES.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-19 14:05:38.000000 feno-0.2.1/src/feno.egg-info/dependency_links.txt
--rw-r--r--   0 lion      (1000) lion      (1000)      192 2024-04-19 14:05:38.000000 feno-0.2.1/src/feno.egg-info/entry_points.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       51 2024-04-19 14:05:38.000000 feno-0.2.1/src/feno.egg-info/requires.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-19 14:05:38.000000 feno-0.2.1/src/feno.egg-info/top_level.txt
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-25 14:39:42.163656 feno-0.2.2/
+-rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.2.2/LICENSE
+-rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.2.2/MANIFEST.in
+-rw-r--r--   0 lion      (1000) lion      (1000)     2569 2024-04-25 14:39:42.163656 feno-0.2.2/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)     1716 2024-04-25 13:45:39.000000 feno-0.2.2/Readme.md
+-rw-r--r--   0 lion      (1000) lion      (1000)     1396 2024-04-25 13:38:45.000000 feno-0.2.2/changelog.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      305 2024-04-25 14:08:21.000000 feno-0.2.2/requirements.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-25 14:39:42.163656 feno-0.2.2/setup.cfg
+-rw-r--r--   0 lion      (1000) lion      (1000)     3157 2024-04-25 14:00:40.000000 feno-0.2.2/setup.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-25 14:39:42.150322 feno-0.2.2/src/
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-25 14:39:42.160322 feno-0.2.2/src/feno/
+-rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-25 13:23:50.000000 feno-0.2.2/src/feno/__init__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2345 2024-04-25 14:26:59.000000 feno-0.2.2/src/feno/__main__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5534 2024-04-25 14:31:38.000000 feno-0.2.2/src/feno/actions.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.2.2/src/feno/cases.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.2.2/src/feno/check.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.2.2/src/feno/css_style.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     9189 2024-04-19 14:04:18.000000 feno-0.2.2/src/feno/filter.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     8932 2024-04-25 14:27:57.000000 feno-0.2.2/src/feno/html.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4378 2024-04-08 17:28:46.000000 feno-0.2.2/src/feno/indexer.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3503 2024-04-05 00:31:13.000000 feno-0.2.2/src/feno/jsontools.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4907 2024-04-08 23:40:15.000000 feno-0.2.2/src/feno/lock.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.2.2/src/feno/log.py
+-rw-r--r--   0 lion      (1000) lion      (1000)    11894 2024-04-08 15:58:02.000000 feno-0.2.2/src/feno/mdpp.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5043 2024-04-25 14:31:56.000000 feno-0.2.2/src/feno/remote_md.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-25 14:39:42.160322 feno-0.2.2/src/feno.egg-info/
+-rw-r--r--   0 lion      (1000) lion      (1000)     2569 2024-04-25 14:39:42.000000 feno-0.2.2/src/feno.egg-info/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)      542 2024-04-25 14:39:42.000000 feno-0.2.2/src/feno.egg-info/SOURCES.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-25 14:39:42.000000 feno-0.2.2/src/feno.egg-info/dependency_links.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)      192 2024-04-25 14:39:42.000000 feno-0.2.2/src/feno.egg-info/entry_points.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       51 2024-04-25 14:39:42.000000 feno-0.2.2/src/feno.egg-info/requires.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-25 14:39:42.000000 feno-0.2.2/src/feno.egg-info/top_level.txt
```

### Comparing `feno-0.2.1/LICENSE` & `feno-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `feno-0.2.1/PKG-INFO` & `feno-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.2.1
+Version: 0.2.2
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
@@ -32,21 +32,27 @@
 - Um gerador de links absolutos para arquivos locais.
 - Uma ferramenta para filtrar rascunhos de código.
 - Um indexador de questões.
 - Um gerador de arquivos para serem utilizados no VPL do Moodle ou via tko.
 
 ## Instalação
 
+Se estiver no windows, instale o [WSL](https://docs.microsoft.com/pt-br/windows/wsl/install) e utilize o Ubuntu.
+
 ```bash
 pip install feno
 
+# ou diretamente do github
+
+pip install git+https://github.com/senapk/feno.git
+
 # tko para gerar e converter os testes e testar os códigos
 pip install tko
 
-# pandoc para gerar os htmls
+# pandoc para gerar os htmls se quiser htmls de qualidade e com suporte a latex
 sudo apt install pandoc
 ```
 
 ## Modo básico
 
 Crie um arquivo `Readme.md` com o seguinte formato:
```

### Comparing `feno-0.2.1/README.md` & `feno-0.2.2/Readme.md`

 * *Files 17% similar despite different names*

```diff
@@ -7,21 +7,27 @@
 - Um gerador de links absolutos para arquivos locais.
 - Uma ferramenta para filtrar rascunhos de código.
 - Um indexador de questões.
 - Um gerador de arquivos para serem utilizados no VPL do Moodle ou via tko.
 
 ## Instalação
 
+Se estiver no windows, instale o [WSL](https://docs.microsoft.com/pt-br/windows/wsl/install) e utilize o Ubuntu.
+
 ```bash
 pip install feno
 
+# ou diretamente do github
+
+pip install git+https://github.com/senapk/feno.git
+
 # tko para gerar e converter os testes e testar os códigos
 pip install tko
 
-# pandoc para gerar os htmls
+# pandoc para gerar os htmls se quiser htmls de qualidade e com suporte a latex
 sudo apt install pandoc
 ```
 
 ## Modo básico
 
 Crie um arquivo `Readme.md` com o seguinte formato:
```

### Comparing `feno-0.2.1/changelog.md` & `feno-0.2.2/changelog.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Changelog
 
+- 0.2.2
+  - add: python markdown instead pandoc as option
+  - fix: remote error if null content
 - 0.2.1
   - add: clear folder without removing it, changing inodes
 - 0.2.0
   - add: improved indexed checking for unused hooks
   - fix: remove extra newline in feno
   - add: ignore node_modules and .json files as feno targets
   - add: indexed needs now base folder as parameter
```

### Comparing `feno-0.2.1/setup.py` & `feno-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import pathlib
 import re
 
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 
 here = pathlib.Path(__file__).parent.resolve()  # current path
-long_description = (here / 'README.md').read_text(encoding='utf-8')  # Get the long description from the README file
+long_description = (here / 'Readme.md').read_text(encoding='utf-8')  # Get the long description from the README file
 with open(here / 'requirements.txt') as fp:  # read requirements.txt
     install_reqs = [r.rstrip() for r in fp.readlines() if not r.startswith('#')]
 
 
 def get_version():
     file = here / 'src/feno/__init__.py'
     return re.search(r'^__version__ = [\'"]([^\'"]*)[\'"]', file.read_text(), re.M).group(1)
```

### Comparing `feno-0.2.1/src/feno/__main__.py` & `feno-0.2.2/src/feno/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('targets', metavar='T', type=str, nargs='*', help='folders')
     parser.add_argument("--check", "-c", action="store_true", help="Check if the file needs to be rebuilt")
     parser.add_argument("--version", "-v", action="store_true", help="Prints the version")
-
     parser.add_argument("--brief", "-b", action="store_true", help="Brief mode")
     # add parameters to receive all target that should be ignored
     parser.add_argument("--tko", "-t", action="store_true", help="Insert tko preamble")
     parser.add_argument("--remote", "-r", action="store_true", help="Search for remote.cfg file and create absolute links")
     parser.add_argument("--erase", "-e", action="store_true", help="Erase .html and .tio temp files")
 
     parser.add_argument("--full", "-f", action="store_true", help="Full mode - equivalent to -tre")
@@ -24,36 +23,36 @@
 
     args = parser.parse_args()
     Log.set_verbose(not args.brief)
     if args.full:
         args.tko = True
         args.remote = True
         args.erase = True
-    
+
     if args.version:
         print(__version__)
         sys.exit(0)
 
     if len(args.targets) == 0:
         print("fail: No targets specified")
         exit(1)
 
     for target in args.targets:
         hook = os.path.basename(os.path.abspath(target))
 
-        actions = Actions(target, args.remote, args.tko)
+        actions = Actions(target)\
+                    .set_remote(args.remote)\
+                    .set_insert_tko_preamble(args.tko)
 
         if not actions.validate():
             continue
 
         Log.resume("- " + hook, end=": [ ")
         Log.verbose("- " + hook)
 
-
-
         actions.load_title()
         actions.create_cache()
         actions.update_markdown()
 
         if not args.check or actions.need_rebuild():
             actions.recreate_cache() # erase .cache
             actions.copy_drafts()
```

### Comparing `feno-0.2.1/src/feno/actions.py` & `feno-0.2.2/src/feno/actions.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,30 +12,39 @@
 import os
 import shutil
 
 def norm_join(*args):
     return os.path.normpath(os.path.join(*args))
 
 class Actions:
-    def __init__(self, source_dir, make_remote: bool, insert_tko_preamble: bool):
+    def __init__(self, source_dir):
         self.cache = norm_join(source_dir, ".cache")
         self.target = norm_join(self.cache, "mapi.json")
         self.source_dir = source_dir
         self.hook = os.path.basename(os.path.abspath(source_dir))
         self.source_readme = norm_join(self.source_dir, "Readme.md")
         self.remote_readme = norm_join(self.cache, "Readme.md")
         self.target_html = norm_join(self.cache, "q.html")
         self.title = ""
         self.cases = norm_join(self.cache, "q.tio")
         self.config_json = norm_join(self.source_dir, "config.json")
         self.mapi_json = norm_join(self.cache, "mapi.json")
         self.cache_src = norm_join(self.cache, "draft")
         self.vpl = None
-        self.make_remote: bool = make_remote
-        self.insert_tko_preamble: bool = insert_tko_preamble
+        self.make_remote: bool = False
+        self.insert_tko_preamble: bool = False
+        self.use_pandoc: bool = False
+
+    def set_remote(self, make_remote: bool):
+        self.make_remote = make_remote
+        return self
+
+    def set_insert_tko_preamble(self, insert_tko_preamble: bool):
+        self.insert_tko_preamble = insert_tko_preamble
+        return self
 
     def validate(self):
         if self.hook == "node_modules" or self.hook.endswith(".json"):
             return False
         if not os.path.isdir(self.source_dir):
             print(f"\n    fail: {self.source_dir} is not a directory")
             return False
@@ -61,34 +70,36 @@
         if Check.need_rebuild(self.source_dir, self.target):
             Log.resume("Changes ", end="")
             Log.verbose(f"  Changes in {self.source_dir}")
             return True
         return False
     
     def remote_md(self):
-        cfg = RemoteCfg()
+        cfg = None
         found = False
         if self.make_remote:
+            cfg = RemoteCfg()
             cfg_path = RemoteCfg.search_cfg_path(self.source_dir)
             if cfg_path is None:
+                cfg = None
                 print("\n    fail: no remote.cfg found in the parent folders")
                 print("\n    fail: proceeding without make absolute links")
             else:
                 found = True
                 Log.verbose(f"  remote.cfg: {cfg_path}")
                 cfg.read(cfg_path)
         RemoteMd.run(cfg, self.source_readme, self.remote_readme, self.hook, self.insert_tko_preamble)
         if self.make_remote and found:
             Log.resume("AbsoluteMd ", end="")
         Log.verbose(f"  RemoteFile: {self.remote_readme}")
     
     # uses pandoc to generate html from markdown
     def html(self):
         title = Title.extract_title(self.source_readme)
-        HTML.generate_html_with_pandoc(title, self.remote_readme, self.target_html, True)
+        HTML.generate_html_with_pandoc(title, self.remote_readme, self.target_html)
         Log.resume("HTML ", end="")
         Log.verbose(f"  HTML  file: {self.target_html}")
 
     # uses tko to generate cases file
     def build_cases(self):
         Cases.run(self.cases, self.source_readme, self.source_dir)
         Log.resume("Cases ", end="")
```

### Comparing `feno-0.2.1/src/feno/cases.py` & `feno-0.2.2/src/feno/cases.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.1/src/feno/check.py` & `feno-0.2.2/src/feno/check.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.1/src/feno/css_style.py` & `feno-0.2.2/src/feno/css_style.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.1/src/feno/filter.py` & `feno-0.2.2/src/feno/filter.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.1/src/feno/html.py` & `feno-0.2.2/src/feno/html.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                 output.append(line)
         with open(html_file, "w") as f:
             f.write("\n".join(output))
 
 
 
     @staticmethod
-    def generate_html_with_pandoc(title: str, input_file: str, output_file: str, enable_latex: bool):
+    def generate_html_with_pandoc(title: str, input_file: str, output_file: str, enable_latex: bool = True):
         fulltitle = title.replace('!', '\\!').replace('?', '\\?')
         cmd = ["pandoc", input_file, '--css', CssStyle.get_file(), '--metadata', 'pagetitle=' + fulltitle,
             '-s', '-o', output_file]
         if enable_latex:
             cmd.append("--mathjax")
         try:
             p = subprocess.Popen(cmd, stdout=PIPE, stderr=PIPE, universal_newlines=True)
```

### Comparing `feno-0.2.1/src/feno/indexer.py` & `feno-0.2.2/src/feno/indexer.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.1/src/feno/jsontools.py` & `feno-0.2.2/src/feno/jsontools.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.1/src/feno/lock.py` & `feno-0.2.2/src/feno/lock.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.1/src/feno/mdpp.py` & `feno-0.2.2/src/feno/mdpp.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.1/src/feno/remote_md.py` & `feno-0.2.2/src/feno/remote_md.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,16 @@
         return None
 
 class Absolute:
 
     # processa o conteúdo trocando os links locais para links absolutos utilizando a url remota
     @staticmethod
     def __replace_remote(content: str, remote_raw: str, remote_view: str, remote_folder: str) -> str:
+        if content is None or content == "":
+            return ""
         if not remote_raw.endswith("/"):
             remote_raw += "/"
         if not remote_view.endswith("/"):
             remote_view += "/"
         if not remote_folder.endswith("/"):
             remote_folder += "/"
```

### Comparing `feno-0.2.1/src/feno.egg-info/PKG-INFO` & `feno-0.2.2/src/feno.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.2.1
+Version: 0.2.2
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
@@ -32,21 +32,27 @@
 - Um gerador de links absolutos para arquivos locais.
 - Uma ferramenta para filtrar rascunhos de código.
 - Um indexador de questões.
 - Um gerador de arquivos para serem utilizados no VPL do Moodle ou via tko.
 
 ## Instalação
 
+Se estiver no windows, instale o [WSL](https://docs.microsoft.com/pt-br/windows/wsl/install) e utilize o Ubuntu.
+
 ```bash
 pip install feno
 
+# ou diretamente do github
+
+pip install git+https://github.com/senapk/feno.git
+
 # tko para gerar e converter os testes e testar os códigos
 pip install tko
 
-# pandoc para gerar os htmls
+# pandoc para gerar os htmls se quiser htmls de qualidade e com suporte a latex
 sudo apt install pandoc
 ```
 
 ## Modo básico
 
 Crie um arquivo `Readme.md` com o seguinte formato:
```

### Comparing `feno-0.2.1/src/feno.egg-info/SOURCES.txt` & `feno-0.2.2/src/feno.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE
 MANIFEST.in
-README.md
+Readme.md
 changelog.md
 requirements.txt
 setup.cfg
 setup.py
 src/feno/__init__.py
 src/feno/__main__.py
 src/feno/actions.py
```

