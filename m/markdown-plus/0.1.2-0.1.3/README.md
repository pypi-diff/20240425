# Comparing `tmp/markdown_plus-0.1.2.tar.gz` & `tmp/markdown_plus-0.1.3.tar.gz`

## Comparing `markdown_plus-0.1.2.tar` & `markdown_plus-0.1.3.tar`

### file list

```diff
@@ -1,65 +1,67 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/CODEOWNERS
--rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/READMEold.md
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/docs/DevelopNewGenerators.md
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/docs/DevelopNewTemplates.md
--rw-r--r--   0        0        0     7851 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/docs/Generators.md
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/docs/README.md
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/docs/Templates.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/_version.py
--rw-r--r--   0        0        0     7352 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/cli.py
--rw-r--r--   0        0        0    13906 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/cli_old.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/config.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/core_old.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/core/__init__.py
--rw-r--r--   0        0        0     8951 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/core/generator.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/core/importer.py
--rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/core/documents/block.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/core/documents/definitions.py
--rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/core/documents/document.py
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/core/documents/structure.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/core/environments/base.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/core/environments/ros2.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/__init__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/flags.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/generate/__init__.py
--rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/generate/content.py
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/generate/installation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/generate/getting_started/__init__.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/generate/getting_started/pakk.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/include/__init__.py
--rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/include/example.py
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/include/examples.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/include/md.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/ros/__init__.py
--rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/ros/interfaces.py
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/ros/launchs.py
--rw-r--r--   0        0        0     8010 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/ros/nodes.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/Hooks.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/MDP_IGNORE
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/__init__.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/default/DOCS.md
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/default/README.md
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/init/_README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/init/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/init/docs/AUTHORS.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/init/docs/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/init/examples/__init__.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/init/examples/example1.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/init/examples/mdplus.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/util/__init__.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/util/file_utils.py
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/util/hooks.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/util/markdown.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/util/regex.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/util/parser/__init__.py
--rw-r--r--   0        0        0    15397 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/util/parser/py_parser.py
--rw-r--r--   0        0        0    20733 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/util/parser/ros2_parser.py
--rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/.gitignore
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/LICENSE
--rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/README.md
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/CODEOWNERS
+-rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/READMEold.md
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/docs/DevelopNewGenerators.md
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/docs/DevelopNewTemplates.md
+-rw-r--r--   0        0        0     7851 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/docs/Generators.md
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/docs/README.md
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/docs/Templates.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/_version.py
+-rw-r--r--   0        0        0     7812 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/cli.py
+-rw-r--r--   0        0        0    13494 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/cli_old.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/config.py
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/core_old.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/core/__init__.py
+-rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/core/generator.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/core/importer.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/core/documents/block.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/core/documents/definitions.py
+-rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/core/documents/document.py
+-rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/core/documents/structure.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/core/environments/base.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/core/environments/ros2.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/generators/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/generators/flags.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/generators/generate/__init__.py
+-rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/generators/generate/content.py
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/generators/generate/installation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/generators/generate/getting_started/__init__.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/generators/generate/getting_started/pakk.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/generators/include/__init__.py
+-rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/generators/include/example.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/generators/include/examples.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/generators/include/md.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/generators/ros/__init__.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/generators/ros/interfaces.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/generators/ros/launchs.py
+-rw-r--r--   0        0        0     8189 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/generators/ros/nodes.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/templates/Hooks.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/templates/MDP_IGNORE
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/templates/__init__.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/templates/default/DOCS.md
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/templates/default/README.md
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/templates/init/_README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/templates/init/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/templates/init/docs/AUTHORS.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/templates/init/docs/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/templates/init/examples/__init__.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/templates/init/examples/example1.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/templates/init/examples/mdplus.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/util/__init__.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/util/file_utils.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/util/hooks.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/util/markdown.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/util/regex.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/util/parser/__init__.py
+-rw-r--r--   0        0        0    15362 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/util/parser/py_parser.py
+-rw-r--r--   0        0        0    21835 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/mdplus/util/parser/ros2_parser.py
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/.gitignore
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/README.md
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 markdown_plus-0.1.3/PKG-INFO
```

### Comparing `markdown_plus-0.1.2/READMEold.md` & `markdown_plus-0.1.3/READMEold.md`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.2/.github/workflows/python-publish.yml` & `markdown_plus-0.1.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.2/docs/Generators.md` & `markdown_plus-0.1.3/docs/Generators.md`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.2/docs/README.md` & `markdown_plus-0.1.3/docs/README.md`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.2/mdplus/cli.py` & `markdown_plus-0.1.3/mdplus/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,47 +15,56 @@
 modules = dict()
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"], max_content_width=800)
 
 
 def setup_logger(**kwargs):
     global logger_initialized
-    logger.setLevel(logging.DEBUG if kwargs.get("verbose") else logging.INFO)
+    if kwargs.get("quiet"):
+        logger.setLevel(logging.ERROR)
+    elif kwargs.get("verbose"):
+        logger.setLevel(logging.DEBUG)
+    else:
+        logger.setLevel(logging.INFO)
+
     if logger_initialized:
         return
-    
+
     logger_initialized = True
     if kwargs.get("verbose"):
         # FORMAT = "%(asctime)s - %(name)s - %(message)s"
         FORMAT = "%(asctime)s %(message)s"
     else:
         FORMAT = "%(message)s"
-    
+
     # Set the format and handler for the logger
-    handler = RichHandler() 
+    handler = RichHandler()
     formatter = logging.Formatter(fmt=FORMAT, datefmt="[%X]")
     handler.setFormatter(formatter)
     logger.addHandler(handler)
 
 
-
 @click.group(cls=ClickAliasedGroup, context_settings=CONTEXT_SETTINGS)
 def execute():
     pass
 
 
 @execute.command(aliases=["c"])
 def config():
     """Configure the MD Plus settings in the current project."""
-    
+
     # GitHub / GitLab Flavored Markdown
     pass
 
+
 @execute.command(aliases=["p"])
 @click.option("--verbose", "-v", is_flag=True, help="Print more output.")
+@click.option("--quiet", "-q", is_flag=True, help="Print less output.")
+@click.option("--write-only-new-content", "-N", is_flag=True, help="Only write files with new content.")
+@click.option("--is-pre-commit-hook", is_flag=True, help="Enables output for pre-commit hook.")
 # @click.option("--recursive", "-r", is_flag=True, help="Parse all subdirectories.")
 # @click.option("--root", "-R", help="Root directory parsing the repo.")
 @click.argument(
     "root_dir",
     nargs=1,
     type=click.Path(exists=True, file_okay=True, dir_okay=False, readable=True),
     required=False,
@@ -70,19 +79,22 @@
     # print(root_dir, kwargs)
     # return
 
     root_dir = None
     # If no dirname is specified, use the current working directory
     if root_dir is None or len(root_dir) == 0:
         root_dir = os.getcwd()
-            
+
     logger.debug(f"Starting parsing of {root_dir}")
-    
+
     workspace = Workspace(root_dir)
-    workspace.process()
+    workspace.is_pre_commit_hook = kwargs.get("is_pre_commit_hook", False)
+    workspace.process(kwargs.get("write_only_new_content", False))
+
+    return 0
 
 
 @execute.command(aliases=["i"])
 @click.option("--verbose", "-v", is_flag=True, help="Print more output.")
 @click.option("--overwrite", "-O", default=False, is_flag=True, help="Overwrites existing files.")
 @click.option("--skip-existing", "-S", default=False, is_flag=True, help="Skip existing files.")
 @click.option("--include-all", "-A", default=False, is_flag=True, help="Include all files without asking.")
@@ -143,27 +155,27 @@
         *template_choices,
         Separator(),
     ]
 
     if len(template_choices) == 0:
         logger.error("No templates found")
         return
-    
+
     if len(template_choices) == 1:
         answer = list(template_workspaces.keys())[0]
     else:
         answer = inquirer.select(
             message="Select a template for initializing the project:",
             choices=choices,
         ).execute()
 
     if answer is None:
         logger.error("No template selected")
         return
-    
+
     selected_workspace = template_workspaces[answer]
 
     # Copy all documents to the target directory
     for doc in selected_workspace.documents:
         logger.debug(f"Processing {doc.file_name}")
         file_path = os.path.abspath(os.path.join(abs_path, doc.args["path"]))
         file_name = os.path.basename(file_path)
@@ -176,15 +188,14 @@
                 message=f"Create {file_name} @ {file_path}?",
                 long_instruction=doc.get_title(),
                 default=True,
             ).execute()
 
         if not proceed:
             continue
-        
 
         # Make dirs if not exists
         dir_path = os.path.dirname(file_path)
         if not os.path.isdir(dir_path):
             os.makedirs(dir_path)
 
         # Check, if file already exists
@@ -204,24 +215,23 @@
                 if not proceed:
                     continue
 
                 # Create backup
                 backup_path = f"{file_path}{datetime.now().strftime('%Y%m%d%H%M%S')}.bak"
                 logger.info(f"Creating backup of {file_path} @ {backup_path}")
                 os.rename(file_path, backup_path)
-        
+
         logger.info(f"Writing {file_name} @ {file_path}")
         with open(file_path, "w") as f:
             with open(doc.full_path, "r") as template:
                 for line in template:
                     f.write(line)
 
-
     # After template is initialized, ask if mdplus parse should be executed
     if inquirer.confirm("Do you want to parse the initialized template now?", default=True).execute():
         logger.info(f"Starting 'mdplus parse' for {abs_path}")
         ctx.invoke(parse, root_dir=abs_path, **kwargs)
         # parse(abs_path)
 
     logger.info("Initialization completed! :)")
 
-    return
+    return
```

### Comparing `markdown_plus-0.1.2/mdplus/cli_old.py` & `markdown_plus-0.1.3/mdplus/cli_old.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import importlib
 import importlib.util
 import importlib.resources
 
 # from mdplus.core import Replacement
 
 from mdplus.logger import Logger
+
 # from mdplus.util.hooks import Hooks
 # from mdplus.util.parser.py_parser import get_args
 # from mdplus.util.markdown import adapt_header_level
 
 logger = logging.getLogger(__name__)
 
 modules = dict()
@@ -26,24 +27,22 @@
 
 
 @click.group(cls=ClickAliasedGroup, context_settings=CONTEXT_SETTINGS)
 def execute():
     pass
 
 
-
-
-
 @execute.command(aliases=["c"])
 def config():
     """Configure the MD Plus settings in the current project."""
-    
+
     # GitHub / GitLab Flavored Markdown
     pass
 
+
 @execute.command(aliases=["p"])
 @click.option("--verbose", "-v", is_flag=True, help="Print more output.")
 @click.argument(
     "dirname",
     nargs=1,
     type=click.Path(exists=True, file_okay=False, dir_okay=True, readable=True),
     required=False,
@@ -53,14 +52,15 @@
     nargs=-1,
     type=click.Path(exists=True, file_okay=True, dir_okay=False, readable=True),
     required=False,
 )
 def parse(dirname, files, **kwargs: str):
     print("Parsing", dirname, files)
 
+
 @execute.command(aliases=[])
 @click.argument(
     "dirname",
     nargs=1,
     type=click.Path(exists=True, file_okay=False, dir_okay=True, readable=True),
     required=False,
 )
@@ -87,17 +87,15 @@
     cfg_file = os.path.join(dirname, ".mdplus.cfg")
     if os.path.isfile(cfg_file):
         cfg.read(cfg_file)
 
     dirs = []
 
     for section in cfg.sections():
-        if (in_dir := cfg.get(section, "in", fallback=None)) and (
-            out_dir := cfg.get(section, "out", fallback=None)
-        ):
+        if (in_dir := cfg.get(section, "in", fallback=None)) and (out_dir := cfg.get(section, "out", fallback=None)):
             logger.info(f"Found {section} cfg: in='{in_dir}', out='{out_dir}'")
             dirs.append(
                 (
                     os.path.abspath(os.path.join(dirname, in_dir)),
                     os.path.abspath(os.path.join(dirname, out_dir)),
                 )
             )
@@ -111,19 +109,15 @@
     rules = [
         [lambda f: f.endswith(".md") and f.startswith("_"), lambda f: f[1:]],
         [lambda f: f.endswith("mdp.md"), lambda f: f[:-7] + ".md"],
     ]
 
     for in_dir, out_dir in dirs:
         if files is None or len(files) == 0:
-            files = [
-                f
-                for f in os.listdir(in_dir)
-                if any([r_check(f) for r_check, r_modify in rules])
-            ]
+            files = [f for f in os.listdir(in_dir) if any([r_check(f) for r_check, r_modify in rules])]
 
         logger.info(f"Parsing the following files in '{in_dir}':")
         files_str = "\n".join([f" - '{f}'" for f in files])
         logger.info(files_str)
 
         for source_file in files:
             abs_path = os.path.abspath(in_dir)
@@ -176,17 +170,15 @@
                         logger.debug(f"Text before command: '{text_before_cmd}'")
 
                         if inline:
                             # If the command is inline, count the number of # in front of the command
                             header_level = text_before_cmd.count("#") - 1
                             text_before_cmd = text_before_cmd.strip("#").strip()
                         else:
-                            header_level = (
-                                (match.group(1).count("#") - 1) if match.group(1) else 0
-                            )
+                            header_level = (match.group(1).count("#") - 1) if match.group(1) else 0
                         fun_call = match.group(2)
                         command = match.group(3)
 
                         logger.debug(
                             f"Start: {start}, end: {end}, header_level: {header_level}, fun_call: {fun_call}, command: {command}"
                         )
 
@@ -201,17 +193,15 @@
                             else:
                                 logger.warning(f"Module {module_name} not found")
                                 modules[command] = None
 
                         cmd_module = modules[command]
                         if cmd_module is not None:
                             # print(cmd_module)
-                            if not hasattr(cmd_module, "main") or not callable(
-                                cmd_module.main
-                            ):
+                            if not hasattr(cmd_module, "main") or not callable(cmd_module.main):
                                 logger.error(
                                     f"Module {cmd_module} is a package or does not have a main() function. Call with package.module!"
                                 )
                                 continue
 
                             fun = getattr(cmd_module, "main")
                             args, _kwargs = get_args(fun_call)
@@ -222,17 +212,15 @@
 
                             logger.debug(
                                 f"Running {command} @ header {header_level} with args {args} and kwargs {_kwargs}"
                             )
                             replacement = fun(*args, **_kwargs)
                             if isinstance(replacement, str):
                                 replacement = Replacement(replacement)
-                            replacement.text = adapt_header_level(
-                                replacement.text, header_level
-                            )
+                            replacement.text = adapt_header_level(replacement.text, header_level)
 
                             # If the replacement replaces the text before the command, adapt the start index
                             if replacement.replaces_text_before_cmd:
                                 start = check_index
 
                             # Replace match by fun result
                             text = text[:start] + replacement.text + text[end:]
@@ -266,20 +254,16 @@
                         text_before, link = match.groups()
                         # Check if the link is relative
                         if link.startswith("http") or os.path.isabs(link):
                             start_pos = match.end()
                             continue
 
                         destination = os.path.abspath(os.path.join(in_dir, link))
-                        new_link = os.path.join(
-                            ".", os.path.relpath(destination, out_dir)
-                        ).replace("\\", "/")
-                        logger.debug(
-                            f"Transforming relative link:\n  {link} to\n  {new_link}"
-                        )
+                        new_link = os.path.join(".", os.path.relpath(destination, out_dir)).replace("\\", "/")
+                        logger.debug(f"Transforming relative link:\n  {link} to\n  {new_link}")
 
                         text = text[: match.start(2)] + new_link + text[match.end(2) :]
                         start_pos = match.start(2) + len(new_link)
 
                 # Write the file to the output
                 logger.info(f"Writing output to {outpath}")
                 with open(outpath, "w") as f:
@@ -290,17 +274,15 @@
     splits = name.split("/")
     template = "mdplus.templates." + ".".join(splits[:-1])
     return importlib.resources.read_text(template, splits[-1])
 
 
 @execute.command(aliases=["i"])
 @click.argument("dirname")
-@click.option(
-    "--overwrite", "-O", default=False, is_flag=True, help="Overwrites existing files."
-)
+@click.option("--overwrite", "-O", default=False, is_flag=True, help="Overwrites existing files.")
 @click.option(
     "--with-examples",
     "-e",
     default=False,
     is_flag=True,
     help="Creates an examples directory.",
 )
@@ -355,17 +337,15 @@
             f.write(readme_content)
 
     # If without examples, delete the examples command
     if not with_examples:
         with open(os.path.join(abs_path, "_README.md"), "r") as f:
             readme_content = f.read()
 
-        readme_content = readme_content.replace(
-            '# #MD+:include.examples("./examples/")\n\n', ""
-        )
+        readme_content = readme_content.replace('# #MD+:include.examples("./examples/")\n\n', "")
 
         with open(os.path.join(abs_path, "_README.md"), "w") as f:
             f.write(readme_content)
 
 
 if __name__ == "__main__":
     parse()
```

### Comparing `markdown_plus-0.1.2/mdplus/config.py` & `markdown_plus-0.1.3/mdplus/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 from typing import List
 
 
-class JsonLoadable():
+class JsonLoadable:
     def assign_from_json(self, json_dict: dict):
         # Iter all keys in the json dict
         for key in json_dict:
             if hasattr(self, key):
                 if isinstance(getattr(self, key), JsonLoadable):
                     getattr(self, key).assign_from_json(json_dict[key])
                 else:
```

### Comparing `markdown_plus-0.1.2/mdplus/core_old.py` & `markdown_plus-0.1.3/mdplus/core_old.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import re
 
 pattern_headers = re.compile(r"#+ .*")
 pattern_headers_inside_code = re.compile(r"```(.|[\n\s$^])*?(# .*?\n)(.|[\n\s$^])*?```")
 
 pattern_code_block = re.compile(r"```(.|[\n\s$^])*?```")
 
+
 class Replacement:
     """Helper object for replacements of md+ commands in markdown files"""
+
     def __init__(self, text, replaces_text_before_cmd=False):
         """Craete a new Replacement object
 
         Parameters
         ----------
         text : str
             The replacement text for the original command
```

### Comparing `markdown_plus-0.1.2/mdplus/logger.py` & `markdown_plus-0.1.3/mdplus/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from rich.console import Console
 from rich.progress import Progress, TaskID
 
 console = Console()
 
 logger = logging.getLogger(__name__)
 
+
 class Logger:
     @staticmethod
     def get_console():
         global console
         return console
 
     @staticmethod
```

### Comparing `markdown_plus-0.1.2/mdplus/core/generator.py` & `markdown_plus-0.1.3/mdplus/core/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 
         Returns
         -------
         str
             The entry of the module.
         """
         if not self.is_applicable():
-            logger.info("Module %s not applicable", self.command)
+            logger.warning("Module %s not applicable", self.command)
             return self.origin_text
 
         logger.info("Generating entry for %s", self.command)
 
         # Adapt the header level
         content = self.get_content()
         content = adapt_header_level(content, self.arg_level - 1)
@@ -191,15 +191,15 @@
                 if start < len(text):
                     modules.append(NoChangeModule(document, text[start:]))
                 break
 
             # Get the mdp definition out of the regex match
             # and extract the command
             mdp_block = MdpBlock(match)
-            command = mdp_block.command            
+            command = mdp_block.command
 
             if command.upper() in MdpGenerator.IGNORED_COMMANDS:
                 module_cls = None
             else:
                 module_cls = ModuleImporter.get_module(command)
                 if ("IGNORE" in mdp_block.arguments) and (mdp_block.arguments["IGNORE"]):
                     module_cls = None
@@ -207,25 +207,29 @@
             if module_cls is not None:
                 # Add NoChangeModule for text before the command
                 if start < match.start():
                     modules.append(NoChangeModule(document, text[start : match.start()]))
 
                 # Add module defined by the command
                 module: MdpGenerator = module_cls(document, mdp_block)
-                module.origin_text = text[match.start() : match.end()]
+                tag_start = match.start()
+                tag_end = match.end()
                 modules.append(module)
 
                 # Find end tag for that module and continue search
                 start = match.end()
                 end_pattern = module.fin_pattern
                 match = end_pattern.search(text, start)
                 if match is None:
                     logger.warning(f"End tag for {command} not found")
                 else:
+                    tag_end = match.end()
                     start = match.end()
+                module.origin_text = text[tag_start:tag_end]
+
             else:
                 modules.append(NoChangeModule(document, text[start : match.end()]))
                 start = match.end()
 
         return modules
```

### Comparing `markdown_plus-0.1.2/mdplus/core/importer.py` & `markdown_plus-0.1.3/mdplus/core/importer.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.2/mdplus/core/documents/block.py` & `markdown_plus-0.1.3/mdplus/core/documents/block.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 import re
 import ast
 
 from mdplus.core.documents.definitions import CommentDefinition
 
 logger = logging.getLogger(__name__)
 
+
 class MdpBlock:
-    def __init__(self, match: re.Match):        
+    def __init__(self, match: re.Match):
         self.match = match
         self.command: str = match.group(2)
         self.arguments_str: str = match.group(3)
 
     @property
     def arguments(self) -> dict[str, str]:
-        return self.parse_arguments(self.arguments_str) 
+        return self.parse_arguments(self.arguments_str)
 
     @staticmethod
     def get_pattern(comment_definition: CommentDefinition):
         # print(comment_definition.multi_line_start)
         # print('|'.join(comment_definition.multi_line_start))
         start = f"({'|'.join(re.escape(s) for s in comment_definition.multi_line_start)})"
         end = f"({'|'.join(re.escape(s) for s in comment_definition.multi_line_end)})"
@@ -30,52 +31,52 @@
         # print(pattern_str)
 
         # Group 1: Multi line comment start
         # Group 2: Command
         # Group 3: Arguments
 
         return re.compile(pattern_str, re.MULTILINE | re.DOTALL)
-    
+
     @staticmethod
     def get_fin_pattern(command: str, comment_definition: CommentDefinition):
-        
+
         start = f"({'|'.join(re.escape(s) for s in comment_definition.multi_line_start)})"
         end = f"({'|'.join(re.escape(s) for s in comment_definition.multi_line_end)})"
         whitespace = r"[\s\n]*?"
         pattern_str = start + whitespace + r"MD\+FIN:" + command + whitespace + r"(" + end + r")"
         return re.compile(pattern_str, re.MULTILINE | re.DOTALL)
-   
+
     @staticmethod
     def parse_arguments(arguments: str) -> dict[str, str]:
         """Parse the arguments of the generator from the string representation.
 
         Parameters
         ----------
         arguments : str
             The string representation of the arguments in the markdown text.
 
         Returns
         -------
         dict[str, str]
             Dictionary containing the arguments.
         """
-        
+
         if arguments.strip() == "":
             return {}
 
         # Remove leading and trailing whitespaces from lines based on intend on the first line
         lines = arguments.split("\n")
         first_none_empty_line = next((i for i, line in enumerate(lines) if line.strip() != ""), None)
         first_none_empty_line = lines[first_none_empty_line] if first_none_empty_line is not None else None
         if first_none_empty_line is not None:
             intend = len(first_none_empty_line) - len(first_none_empty_line.lstrip())
             lines = [line[intend:] for line in lines]
             arguments = "\n".join(lines)
         # print(arguments)
-            
+
         parsed_dict = {}
         parsed_ast = ast.parse(arguments)
 
         global_vars = {}
 
         for node in parsed_ast.body:
             if isinstance(node, ast.Assign):
@@ -85,18 +86,20 @@
                         var_value = node.value
 
                         # Evaluate the expression if it's not a simple value assignment
                         if isinstance(var_value, ast.Expr):
                             var_value = ast.literal_eval(var_value.value)
                         else:
                             try:
-                                var_value = eval(compile(ast.Expression(var_value), '', 'eval'), global_vars, parsed_dict)
-                            except Exception as _:   
+                                var_value = eval(
+                                    compile(ast.Expression(var_value), "", "eval"), global_vars, parsed_dict
+                                )
+                            except Exception as _:
                                 string_of_expression = ast.get_source_segment(arguments, node.value)
                                 logger.error("Error evaluating expression '%s'", string_of_expression)
                                 var_value = None
                         parsed_dict[var_name] = var_value
                     else:
                         logger.warning("Unsupported target type %s", target)
             else:
                 logger.warning("Unsupported node type %s", node)
-        return parsed_dict
+        return parsed_dict
```

### Comparing `markdown_plus-0.1.2/mdplus/core/documents/definitions.py` & `markdown_plus-0.1.3/mdplus/core/documents/definitions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,29 @@
-
 class CommentDefinition:
-    def __init__(self, single_line: str, multi_line_start: str | list[str], multi_line_end: str | list[str] = None, multi_line_between: str | list[str] = ""):
+    def __init__(
+        self,
+        single_line: str,
+        multi_line_start: str | list[str],
+        multi_line_end: str | list[str] = None,
+        multi_line_between: str | list[str] = "",
+    ):
         multi_line_start = [multi_line_start] if isinstance(multi_line_start, str) else list(multi_line_start)
         if multi_line_end is None:
             multi_line_end = multi_line_start
         multi_line_end = [multi_line_end] if isinstance(multi_line_end, str) else list(multi_line_end)
-        
-        self.single_line = single_line 
+
+        self.single_line = single_line
         self.multi_line_start: list[str] = multi_line_start
-        self.multi_line_end: list[str] = multi_line_end 
+        self.multi_line_end: list[str] = multi_line_end
         self.multi_line_between = multi_line_between or ""
 
     @staticmethod
     def get_python_style():
         return CommentDefinition("#", ('"""', "'''"), ('"""', "'''"), "")
-    
+
     @staticmethod
     def get_cpp_style():
         return CommentDefinition("//", "/*", "*/", ("", "*"))
-    
+
     @staticmethod
     def get_markdown_style():
         return CommentDefinition(None, "<!--", "-->", "")
```

### Comparing `markdown_plus-0.1.2/mdplus/core/documents/document.py` & `markdown_plus-0.1.3/mdplus/core/documents/document.py`

 * *Files 12% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 
         for flag in flags:
             if flag in self.args:
                 return self.args[flag]
 
         return False
 
-    def process(self):
+    def process(self, check_for_new_content: bool = False):
 
         # If skip_generating is set, we do not generate the document
         if self.skip_generating:
             logger.info(f"Skipping document: {self.full_path}")
             return
 
         logger.info(f"Processing document: {self.full_path}")
@@ -171,28 +171,47 @@
         text = ""
         with open(self.full_path, "r", encoding="utf-8") as f:
             text = f.read()
 
         self.origin_text = text
         self.modules = MdpGenerator.get_all_generators(text, self)
 
-        self.write()
+        self.write(check_for_new_content=check_for_new_content)
 
     def get_generated_content(self):
         s = ""
         for module in self.modules:
             try:
                 s += module.get_entry()
             except Exception as e:
                 logger.error(f"Error in module {module.command}: {e}")
                 s += module.origin_text
                 # raise e
 
         return s
 
-    def write(self, file_path: str = None):
+    def write(self, file_path: str = None, check_for_new_content: bool = False):
         if file_path is None:
             file_path = self.full_path
 
         content = self.get_generated_content()
+
+        if check_for_new_content:
+            content_lines = content.strip().split("\n")
+            with open(file_path, "r", encoding="utf-8") as f:
+                old_content_lines = f.read().strip().split("\n")
+                no_changes = True
+                for i, line in enumerate(content_lines):
+                    if line.strip() != old_content_lines[i].strip():
+                        no_changes = False
+                        break
+
+                if no_changes and len(content_lines) == len(old_content_lines):
+                    logger.debug(f"Skipping document: {file_path}")
+                    return
+
+        logger.info(f"Writing document: {file_path}")
+        if self.workspace.is_pre_commit_hook:
+            print("Fixing", file_path)
+
         with open(file_path, "w", encoding="utf-8") as f:
             f.write(content)
```

### Comparing `markdown_plus-0.1.2/mdplus/core/documents/structure.py` & `markdown_plus-0.1.3/mdplus/core/documents/structure.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,16 @@
 
         Parameters
         ----------
         root : str
             Root path of the workspace.
         """
 
+        self.is_pre_commit_hook = False
+
         self.root_path = root
         """The root path of the workspace."""
 
         self.environments: dict[str, MdpEnvironment] = dict()
         """
         The environments of the workspace.
         You can retreive an environment by calling `get_environment(env_name, YourMdpEnvironmentClass)`.
@@ -149,12 +151,18 @@
         T
             The environment.
         """
         if name not in self.environments:
             self.environments[name] = env_class(self, name)
         return self.environments[name]
 
-    def process(self):
-        """Process all documents in the workspace."""
+    def process(self, check_for_new_content: bool = False):
+        """Process all documents in the workspace.
+
+        Parameters
+        ----------
+        check_for_new_content : bool, optional
+            If True, the workspace will check for new content in the written documents before writing them, by default False.
+        """
 
         for doc in self.generated_documents:
-            doc.process()
+            doc.process(check_for_new_content)
```

### Comparing `markdown_plus-0.1.2/mdplus/core/environments/base.py` & `markdown_plus-0.1.3/mdplus/core/environments/base.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.2/mdplus/generators/generate/content.py` & `markdown_plus-0.1.3/mdplus/generators/generate/content.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,31 +9,35 @@
 import pandas as pd
 
 
 logger = logging.getLogger(__name__)
 
 
 from typing import TYPE_CHECKING
+
 if TYPE_CHECKING:
     from mdplus.core.documents.document import Document
     from mdplus.core.documents.block import MdpBlock
 
+
 class ContentGenerator(MdpGenerator):
     """Creates a table of contents of the given directory"""
+
     def __init__(self, document: Document, mdpBlock: MdpBlock):
         super().__init__(document, mdpBlock)
 
         self.arg_header = self.get_arg("header", "# Contents of this Repository")
         self.arg_dirs = self.get_arg("dirs", True)
         self.arg_md_files = self.get_arg("md_files", False)
 
     def get_content(self) -> str:
-        
+
         content = list()
-        content.append(self.arg_header)
+        if len(self.arg_header) > 0:
+            content.append(self.arg_header)
 
         # dir_path = self.workspace.root_path
         dir_path = self.document.dir_path
 
         logger.info(f"Creating content of {dir_path}")
 
         # Check if directory exists
@@ -57,15 +61,15 @@
 
                     # Check if directory contains a MDP_IGNORE file
                     if os.path.isfile(os.path.join(dir, "MDP_IGNORE")):
                         continue
 
                     mdp_dir = self.workspace.directory_map.get(dir, None)
                     need_parse = True
-                    
+
                     # If there is a readme file in the directory, check for given args in that file
                     if mdp_dir is not None:
                         if mdp_dir.readme is not None:
                             # If title is given in the args, use this as info
                             if "title" in mdp_dir.readme.args:
                                 info = mdp_dir.readme.args["title"]
                                 need_parse = False
@@ -96,32 +100,35 @@
                                         break
 
                     file_entry = f"[`{file}`]({file})"
                     entries[file_entry] = info
                 elif self.arg_md_files and file.endswith(".md"):
 
                     path = os.path.join(dir_path, file)
-                    
+
                     # Skip the own file
                     if path == self.document.full_path:
                         continue
 
                     doc = self.workspace.document_map.get(path, None)
 
                     basename = os.path.basename(file)
                     if doc is not None:
                         info = doc.get_title() or doc.file_name
                     else:
                         info = basename
-                    
+
                     file_entry = f"[`{basename}`]({file})"
                     entries[file_entry] = info
 
-
             # Convert entries to a dataframe
-            df = pd.DataFrame(entries.items(), columns=["Dir", "Content"])
+            df = pd.DataFrame(entries.items(), columns=["Directory", "Content"])
 
             # Create a Markdown table out of the dataframe
             mkdict = df.to_dict(orient="records")
-            content.append(markdown_table(mkdict).set_params(row_sep="markdown", quote=False, padding_weight="right").get_markdown())
+            content.append(
+                markdown_table(mkdict)
+                .set_params(row_sep="markdown", quote=False, padding_weight="right")
+                .get_markdown()
+            )
 
             return "\n\n".join(content)
```

### Comparing `markdown_plus-0.1.2/mdplus/generators/generate/installation.py` & `markdown_plus-0.1.3/mdplus/generators/generate/installation.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 logger = logging.getLogger(__name__)
 
 
 def clear_git_url(url: str):
     pattern = re.compile(r"oauth2?:.*?@")
     return pattern.sub("", url)
 
+
 def create_git_instructions(git_repo_path: str, kwargs, header_level=2):
     hooks: Hooks = kwargs["hooks"]
 
     try:
         repo = git.Repo(git_repo_path)
         basename = os.path.basename(git_repo_path)
 
@@ -102,16 +103,18 @@
     logger.info(f"Creating installation instruction for {dir_path}")
 
     # Check if directory exists
     if not os.path.isdir(dir_path):
         logger.error(f"Directory {dir_path} for creating installation instruction does not exist")
         return f"# {dir_path} NOT FOUND"
 
-    instructions = [create_git_instructions(dir_path, kwargs, header_level=2),
-                    create_rosepkg_instructions(dir_path, kwargs, header_level=2)]
+    instructions = [
+        create_git_instructions(dir_path, kwargs, header_level=2),
+        create_rosepkg_instructions(dir_path, kwargs, header_level=2),
+    ]
 
     content.append("\n".join([i for i in instructions if i is not None]))
 
     return "\n\n".join(content)
 
 
 class InstallationModule(MdpGenerator):
@@ -119,8 +122,8 @@
     def __init__(self, command: str, arguments: str):
         super().__init__(command, arguments)
 
     def get_content(self):
         return "INSTALL"
 
 
-module = InstallationModule
+module = InstallationModule
```

### Comparing `markdown_plus-0.1.2/mdplus/generators/generate/getting_started/pakk.py` & `markdown_plus-0.1.3/mdplus/generators/generate/getting_started/pakk.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.2/mdplus/generators/include/example.py` & `markdown_plus-0.1.3/mdplus/generators/include/example.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
         return "\n".join(contents)
 
         return "ERROR"
 
     @staticmethod
     def remove_empty_lines(text: str):
-        return empty_lines.sub("\n\n", text)
+        return empty_lines.sub("\n\n", text.strip())
 
     @staticmethod
     def process_ignored(text: str):
         text = replace_pattern(text, ignore_line, only_first=False)
         text = replace_pattern(text, ignore_section, only_first=False)
         text = replace_pattern(text, ignore_start, only_first=False)
         return text
@@ -68,27 +68,35 @@
             input_text = self.process_ignored(input_text)
 
             comment_block_pattern = re.compile(r'"""((""?(?!")|[^"])*)"""')
 
             first_comment_block = comment_block_pattern.search(input_text)
             if first_comment_block is not None:
                 text: str = first_comment_block.group(1)
-
                 # If we do not have an explicit header starting with markdowns header-# in the example
                 if not text.strip().startswith("# "):
                     header = self.arg_header or os.path.basename(file_path)
-                    output += f"# [{header}]({relative_link})\n"
+
+                    # output += f"# [{header}]({relative_link})\n"
+                    output += f"# {header}\n"
+                    # output += f"See [{relative_link.lstrip('./')}](./" + relative_link + ").\n\n"
+
                 # If we have an explicit header in the example
                 else:
                     header_pattern = re.compile(r"# (.*?)\n\n")
                     m = header_pattern.search(text)
                     if m is not None:
                         header = self.arg_header or m.group(1)
                         start, end = m.span()
-                        text = text[:start] + f"# [{header}]({relative_link})\n" + text[end:]
+
+                        # text = text[:start] + f"# [{header}]({relative_link})\n" + text[end:]
+                        end = text[end:]
+                        text = text[:start] + f"# {header}\n"
+                        text += f"See [{relative_link.lstrip('./')}](./" + relative_link + ").\n\n"
+                        text += end
 
                     input_text = (
                         input_text[: first_comment_block.start(1)] + text + input_text[first_comment_block.end(1) :]
                     )
 
             while comment_block := comment_block_pattern.search(input_text):
                 start, end = comment_block.span()
@@ -112,8 +120,10 @@
             if len(input_text) > 0:
                 new_part = input_text.strip()
                 if len(new_part) > 0:
                     output += "```python\n"
                     output += new_part
                     output += "\n```\n\n"
 
+            output += f"Source of the above code: [{relative_link.lstrip('./')}](./" + relative_link + ").\n\n"
+
         return self.remove_empty_lines(output)
```

### Comparing `markdown_plus-0.1.2/mdplus/generators/include/examples.py` & `markdown_plus-0.1.3/mdplus/generators/include/examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from mdplus.util.markdown import adapt_header_level
 
 
 logger = logging.getLogger(__name__)
 
 ignore_line = re.compile(r".*?(" + re.escape(Flags.IGNORE_LINE) + r").*?\n")
 
+
 def main(*args, **kwargs):
     directory = args[0]
     relative_link = directory
 
     logger.info(f"Including examples from {directory}")
 
     root = kwargs["root"]
```

### Comparing `markdown_plus-0.1.2/mdplus/generators/include/md.py` & `markdown_plus-0.1.3/mdplus/generators/include/md.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.2/mdplus/generators/ros/interfaces.py` & `markdown_plus-0.1.3/mdplus/generators/ros/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,8 +85,12 @@
                         "Package": package.name,
                     }
                 )
 
         msg_data.sort(key=lambda x: x["Name"])
         srv_data.sort(key=lambda x: x["Name"])
 
-        return markdown_table(msg_data + srv_data).set_params(row_sep="markdown", quote=False, padding_weight="right").get_markdown()
+        return (
+            markdown_table(msg_data + srv_data)
+            .set_params(row_sep="markdown", quote=False, padding_weight="right")
+            .get_markdown()
+        )
```

### Comparing `markdown_plus-0.1.2/mdplus/generators/ros/launchs.py` & `markdown_plus-0.1.3/mdplus/generators/ros/launchs.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,29 +38,36 @@
         content = list()
         content.append(self.arg_header)
 
         scripts = list()
 
         for package in packages:
             if package.package_type == PackageType.PYTHON:
-                
+
                 if len(package.launch_scripts) > 0:
                     for script in package.launch_scripts:
+                        rel_path = file_utils.get_relative_path(script.launch_file_path, self.document.dir_path)
                         scripts.append(
                             {
-                                "Name": script.name,
+                                # "Name": script.name,
                                 "Info": adapt_string_for_table(script.info),
                                 "Script": get_link(
-                                    script.name,
-                                    file_utils.get_relative_path(script.launch_file_path, self.document.dir_path),
+                                    # script.name,
+                                    rel_path.lstrip("/."),
+                                    rel_path,
                                 ),
                             }
                         )
 
-        scripts.sort(key=lambda x: x["Name"])
+        # scripts.sort(key=lambda x: x["Name"])
+        scripts.sort(key=lambda x: x["Script"])
 
         if len(scripts) > 0:
-            content.append(markdown_table(scripts).set_params(row_sep="markdown", quote=False, padding_weight="right").get_markdown())
+            content.append(
+                markdown_table(scripts)
+                .set_params(row_sep="markdown", quote=False, padding_weight="right")
+                .get_markdown()
+            )
         else:
             content.append("This package has no launch scripts")
 
         return "\n\n".join(content)
```

### Comparing `markdown_plus-0.1.2/mdplus/generators/ros/nodes.py` & `markdown_plus-0.1.3/mdplus/generators/ros/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
                         has_nodes = True
 
         if not has_nodes:
             content.append("This package has no ROS nodes.")
 
         return "\n\n".join(content)
 
-    def get_node_section(self, node: Node) -> str:
+    def get_node_section(self, node: Node, comment_as_code_block=False) -> str:
         content = []
         topics = []
 
         content.append(f"## `{node.name}` Node")
         content.append(adapt_header_level(node.doc_string_without_header, 2))
 
         #################################################################################
@@ -113,15 +113,14 @@
                     {
                         "Topic": publisher.topic_name,
                         "Type": publisher.msg_type,
                         "Kind": "Publisher",
                         "Comment": publisher.comment,
                     }
                 )
-
         for subscription in node.subscriptions:
             if not self.arg_only_commented_subscriptions or len(subscription.comment) > 0:
                 if Flags.IGNORE in subscription.comment:
                     continue
                 topics.append(
                     {
                         "Topic": subscription.topic_name,
@@ -142,15 +141,18 @@
             topic["HasLink"] = True
 
             parts = [
                 f'### `{topic["Topic"]}`',
                 # f'{topic["Kind"]} of type {topic["Type"]}'
             ]
             if comment is not None and len(comment) > 0:
-                parts.extend([f"```", f"{comment}", f"```"])
+                if comment_as_code_block:
+                    parts.extend([f"```", f"{comment}", f"```"])
+                else:
+                    parts.extend([f"{comment}"])
             part = "\n".join(parts)
             content.append(part)
 
         # Adapt the topics for the Markdown table
         has_other_topics_than_not_found = False
         for topic in topics:
             if topic["HasLink"]:
@@ -169,15 +171,17 @@
         if not has_other_topics_than_not_found:
             for topic in topics:
                 del topic["Info"]
 
         if len(topics) > 0:
             topics.sort(key=lambda x: x["Topic"])
             table = (
-                markdown_table(topics).set_params(row_sep="markdown", quote=False, padding_weight="right").get_markdown()
+                markdown_table(topics)
+                .set_params(row_sep="markdown", quote=False, padding_weight="right")
+                .get_markdown()
             )
             content.insert(2, "**Publisher, Subscriber and Services of this node**")
             content.insert(3, table)
 
         #################################################################################
         ### Parameter stuff
```

### Comparing `markdown_plus-0.1.2/mdplus/templates/default/README.md` & `markdown_plus-0.1.3/mdplus/templates/default/README.md`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.2/mdplus/util/file_utils.py` & `markdown_plus-0.1.3/mdplus/util/file_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,25 +36,26 @@
 
     for f in allFiles:
         if f in files:
             existingCount += 1
 
     return existingCount == len(files)
 
-def linux_path(path):
+
+def linux_path(path) -> str:
     return os.path.normpath(path).replace("\\", "/")
 
-def get_relative_path(path, root):
+
+def get_relative_path(path, root) -> str:
     # Check if the path is a subdirectory of the root
     if path.startswith(root):
-      return linux_path(os.path.join(".", path[len(root):]))
-  
+        return linux_path(os.path.join(".", path[len(root) :]))
+
     # Otherwise, we have to go up the directory tree
-    
-    
+
     # Get the common prefix of the path and the root
     common = os.path.commonprefix([path, root])
     # Get the relative path from the common prefix to the root
     relative = os.path.relpath(common, root)
     # Get the relative path from the common prefix to the path
     p = os.path.join(relative, os.path.relpath(path, common))
     return linux_path(p)
```

### Comparing `markdown_plus-0.1.2/mdplus/util/hooks.py` & `markdown_plus-0.1.3/mdplus/util/hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import logging
 
 logger = logging.getLogger(__name__)
 
 
-class HookText():
+class HookText:
     def __init__(self, module: str, text: str):
         self.module = module
 
         text = text.strip()
         while text.startswith("\n"):
             text = text[1:]
         while text.endswith("\n"):
@@ -37,15 +37,15 @@
 
         if current_hook is not None:
             hook_texts[current_hook] = HookText(current_hook, current_text)
 
         return hook_texts
 
 
-class Hooks():
+class Hooks:
     def __init__(self, path: str):
         self.path = path
         self.file_content = ""
         self.hooks = {}
 
         self.load_hooks()
 
@@ -54,15 +54,17 @@
             with open(self.path, "r") as f:
                 self.file_content = f.read()
                 self.hooks = HookText.get_from_file_content(self.file_content)
 
     def __getitem__(self, item):
         return self.hooks[item]
 
-    def append_to_content(self, module_name: str | list[str], part_name: str | list[str], content: list[str], index=None):
+    def append_to_content(
+        self, module_name: str | list[str], part_name: str | list[str], content: list[str], index=None
+    ):
         if isinstance(module_name, str):
             module_name = [module_name]
 
         for mn in module_name:
             if isinstance(part_name, list):
                 part_name = ".".join(part_name)
             name = f"{mn}.{part_name}" if len(part_name) > 0 else mn
```

### Comparing `markdown_plus-0.1.2/mdplus/util/markdown.py` & `markdown_plus-0.1.3/mdplus/util/markdown.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 gitlab_punctuation = string.punctuation.replace("_", "")
 
 
 def get_anchor_from_header(header: str):
     """According to https://docs.gitlab.com/ee/user/markdown.html#header-ids-and-links"""
 
     # Remove all punctuation
-    anchor = header.translate(str.maketrans('', '', gitlab_punctuation))
+    anchor = header.translate(str.maketrans("", "", gitlab_punctuation))
 
     # Replace all whitespace with dashes
     splits = re.split(r"\W", anchor)
     anchor = "-".join([s.lower() for s in splits if len(s) > 0])
     return anchor
```

### Comparing `markdown_plus-0.1.2/mdplus/util/regex.py` & `markdown_plus-0.1.3/mdplus/util/regex.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import re
 from typing import List, Union
 
 
 def replace_pattern(
-    file_content: str, pattern: Union[str, re.Pattern], group: Union[int, List[int]] = 0, substitution: str = "", only_first=True
+    file_content: str,
+    pattern: Union[str, re.Pattern],
+    group: Union[int, List[int]] = 0,
+    substitution: str = "",
+    only_first=True,
 ) -> str:
     """Replaces all matches of the given pattern with the given replacement.
 
     Args:
         file_content (str): The content of the file to be modified.
         pattern (Union[str, re.Pattern]): The regex pattern to be replaced.
         group (Union[int, List[int]], optional): If != 0 just replace the specified group of the match. Defaults to 0.
```

### Comparing `markdown_plus-0.1.2/mdplus/util/parser/py_parser.py` & `markdown_plus-0.1.3/mdplus/util/parser/py_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
         end_col = ast_item.end_col_offset
         lines = script_content.splitlines()
         if line == end_line:
             return lines[line - 1][col:end_col]
         else:
             start = lines[line - 1][col:]
             end = lines[end_line - 1][:end_col]
-            middle = lines[line:end_line - 1]
+            middle = lines[line : end_line - 1]
             return "\n".join([start] + middle + [end])
 
     @staticmethod
     def get_elements_of_type(item: ast.ClassDef | ast.FunctionDef, t: Type[T]) -> list[T]:
         """Get all elements of a certain type from the body of a class or function definition"""
         res = []
         for i in item.body:
@@ -268,17 +268,15 @@
         elif isinstance(item, ast.Attribute):
             res.extend(PyParser.get_all_elements_of_type(item.value, t))
 
         return res
 
     @staticmethod
     def get_elements_where_value_is_of_type(
-            item: ast.ClassDef | ast.FunctionDef,
-            t: Type[T],
-            return_value=False
+        item: ast.ClassDef | ast.FunctionDef, t: Type[T], return_value=False
     ) -> list[T]:
         res = []
         for i in item.body:
             if hasattr(i, "value"):
                 if isinstance(i.value, t):
                     res.append(i.value if return_value else i)
 
@@ -342,16 +340,17 @@
         else:
             # compiled = compile(item, "<ast>", "eval")
             unparsed = ast.unparse(item)
             return unparsed
             # raise ValueError(f"Unknown type {type(item)}")
 
     @staticmethod
-    def get_doc_string(item: ast.ClassDef | ast.FunctionDef | ast.Expr | ast.Constant, only_first_line=False,
-                       remove_indentation=True) -> str:
+    def get_doc_string(
+        item: ast.ClassDef | ast.FunctionDef | ast.Expr | ast.Constant, only_first_line=False, remove_indentation=True
+    ) -> str:
         """Gets a doc string from a class or function or a docstring expression"""
 
         doc: str = None
         elem = item
 
         if isinstance(item, ast.ClassDef) or isinstance(item, ast.FunctionDef):
             if item.body and len(item.body) > 0:
@@ -396,15 +395,15 @@
 
 
 if __name__ == "__main__":
     import mistletoe
     from mistletoe.ast_renderer import ASTRenderer, get_ast
 
     file_path = "C:/Users/schoc/Documents/Studium/Git/ROS-E/software/ros2-packages/displays/docs/HOOKS.md"
-    with open(file_path, 'r') as fin:
+    with open(file_path, "r") as fin:
         # ast = mistletoe.ast_renderer.get_ast(fin.read())
         d = Document(fin)
         sss = str(d)
         a = get_ast(d)
         rendered = mistletoe.markdown(fin, renderer=ASTRenderer)
 
         # markdown.Markdown().
```

### Comparing `markdown_plus-0.1.2/mdplus/util/parser/ros2_parser.py` & `markdown_plus-0.1.3/mdplus/util/parser/ros2_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
         self.package = package
         self.msg_file_path = msg_file_path
         self.name = os.path.basename(self.msg_file_path).replace(".msg", "")
 
         with open(self.msg_file_path) as file:
             lines = file.readlines()
-            self.contentOriginal = "\n".join(lines)
+            self.content_original = "\n".join(lines)
             lines = [line.strip() for line in lines]
 
             splittedLines = []
 
             # Skip Copyright / Licence block
             init_comment_lines = []
             for l in lines:
@@ -68,28 +68,34 @@
                         splittedLines.append(l)
                     else:
                         splittedLines.append("# " + splits[1])
                         splittedLines.append(splits[0])
 
             self.content = "\n".join(splittedLines)
 
-    def get_wiki_entry(self, header_level: int, replace_root: str = ""):
+    def get_wiki_entry(self, header_level: int, replace_root: str = "", as_code_block=True):
         self.wikiEntry = ""
         self.wikiEntry += header_level * "#"
 
         relative_path = self.msg_file_path
         if replace_root != "":
             relative_path = file_utils.get_relative_path(relative_path, replace_root)
 
-        self.wikiEntry += f" [`{self.name}`]({relative_path})\n"
+        # self.wikiEntry += f" [`{self.name}`]({relative_path})\n"
+        self.wikiEntry += f" `{self.name}`\n"
         self.wikiEntry += "\n"
-        self.wikiEntry += "```python\n"
+        if as_code_block:
+            self.wikiEntry += "```python\n"
         self.wikiEntry += self.content
         self.wikiEntry += "\n"
-        self.wikiEntry += "```\n"
+        if as_code_block:
+            self.wikiEntry += "```\n"
+            self.wikiEntry += "\n"
+        self.wikiEntry += f"Source: [{relative_path.lstrip('./')}]({relative_path})"
+
         return self.wikiEntry
 
     def __repr__(self) -> str:
         return self.__str__()
 
     def __str__(self) -> str:
         return self.wikiEntry if self.wikiEntry is not None and len(self.wikiEntry) > 0 else self.get_wiki_entry()
@@ -100,46 +106,69 @@
 
         self.package = package
         self.srv_file_path = srv_file_path
         self.name = os.path.basename(self.srv_file_path).replace(".srv", "")
 
         with open(self.srv_file_path) as file:
             lines = file.readlines()
-            self.contentOriginal = "\n".join(lines)
+            self.content_original = "\n".join(lines)
             lines = [line.strip() for line in lines]
 
             splittedLines = []
 
+            # Skip Copyright / Licence block
+            init_comment_lines = []
+            for l in lines:
+                if l.startswith("#"):
+                    init_comment_lines.append(l)
+                else:
+                    break
+
+            if len(init_comment_lines) > 0:
+                s = "\n".join(init_comment_lines).lower()
+                if "license" in s or "copyright" in s:
+                    lines = lines[len(init_comment_lines) :]
+
+            # Skip the first lines if they are empty
+            while len(lines) > 0 and lines[0] == "":
+                lines.pop(0)
+
             for l in lines:
                 if l.startswith("#"):
                     splittedLines.append(l)
                 else:
                     splits = [a.strip() for a in l.split("#", 1)]
                     if len(splits) == 1:
                         splittedLines.append(l)
                     else:
                         splittedLines.append("# " + splits[1])
                         splittedLines.append(splits[0])
 
             self.content = "\n".join(splittedLines)
 
-    def get_wiki_entry(self, header_level, replace_root: str = ""):
+    def get_wiki_entry(self, header_level: int, replace_root: str = "", as_code_block=True):
         self.wikiEntry = ""
         self.wikiEntry += header_level * "#"
 
         relative_path = self.srv_file_path
         if replace_root != "":
             relative_path = file_utils.get_relative_path(relative_path, replace_root)
 
-        self.wikiEntry += f" [`{self.name}`]({relative_path})\n"
+        # self.wikiEntry += f" [`{self.name}`]({relative_path})\n"
+        self.wikiEntry += f" `{self.name}`\n"
         self.wikiEntry += "\n"
-        self.wikiEntry += "```python\n"
+        if as_code_block:
+            self.wikiEntry += "```python\n"
         self.wikiEntry += self.content
         self.wikiEntry += "\n"
-        self.wikiEntry += "```\n"
+        if as_code_block:
+            self.wikiEntry += "```\n"
+            self.wikiEntry += "\n"
+        self.wikiEntry += f"Source: [{relative_path.lstrip('./')}]({relative_path})"
+
         return self.wikiEntry
 
     def __repr__(self) -> str:
         return self.__str__()
 
     def __str__(self) -> str:
         return self.wikiEntry if self.wikiEntry is not None and len(self.wikiEntry) > 0 else self.get_wiki_entry()
@@ -344,15 +373,14 @@
         if m is None:
             return services
 
         calls = PyParser.get_elements_where_value_is_of_type(m, ast.Call, return_value=True)
         constants = PyParser.get_elements_where_value_is_of_type(m, ast.Constant, return_value=True)
         constants = {e.lineno: e for e in constants}
         filtered = PyParser.filter_calls(calls, "create_service")
-
         for call in filtered:
             args = PyParser.get_args(call, ["srv_type", "srv_name", "callback"])
             srv_type, srv_name, callback = args
             s_srv_type = PyParser.get_name_or_value(srv_type)
             s_srv_name = PyParser.get_name_or_value(srv_name)
             s_callback = PyParser.get_name_or_value(callback, include_origin_for_attributes=False)
 
@@ -429,15 +457,15 @@
         self.name = os.path.basename(os.path.normpath(self.path))
 
         logger.debug(f"Parsing PACKAGE at {self.path}")
 
         self.nodes: List[Node] = []
         self.launch_scripts: List[LaunchScript] = []
         self.messages: List[MessageType] = []
-        self.services: List["ServiceType"] = []
+        self.services: List[ServiceType] = []
 
         self.package_type = PackageType.NONE
 
         if Package.isPythonPackage(self.path):
             self.package_type = PackageType.PYTHON
 
             setupPath = os.path.join(self.path, "setup.py")
```

### Comparing `markdown_plus-0.1.2/.gitignore` & `markdown_plus-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.2/LICENSE` & `markdown_plus-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.2/README.md` & `markdown_plus-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.2/pyproject.toml` & `markdown_plus-0.1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "markdown-plus"
-version = "0.1.2"
+version = "0.1.3"
 authors = [{ name = "Valentin Schröter", email = "vasc9380@th-wildau.de" }]
 description = "Generator for markdown files."
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
   "click-aliases",
   "click",
```

### Comparing `markdown_plus-0.1.2/PKG-INFO` & `markdown_plus-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: markdown-plus
-Version: 0.1.2
+Version: 0.1.3
 Summary: Generator for markdown files.
 Project-URL: Homepage, https://github.com/iCampus-Wildau/markdown-plus
 Project-URL: Issues, https://github.com/iCampus-Wildau/markdown-plus/issues
 Author-email: Valentin Schröter <vasc9380@th-wildau.de>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

