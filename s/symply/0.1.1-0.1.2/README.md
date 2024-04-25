# Comparing `tmp/symply-0.1.1.tar.gz` & `tmp/symply-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symply-0.1.1.tar", max compression
+gzip compressed data, was "symply-0.1.2.tar", max compression
```

## Comparing `symply-0.1.1.tar` & `symply-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2024-04-16 00:37:19.582472 symply-0.1.1/LICENSE
--rw-r--r--   0        0        0     2328 2024-04-16 04:44:56.171036 symply-0.1.1/README.md
--rw-r--r--   0        0        0      503 2024-04-21 06:40:14.122415 symply-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      202 2024-04-16 21:57:45.430130 symply-0.1.1/symply/__init__.py
--rw-r--r--   0        0        0     3930 2024-04-21 06:20:40.692633 symply-0.1.1/symply/symply.py
--rw-r--r--   0        0        0     4885 2024-04-21 06:22:15.562616 symply-0.1.1/symply/watcher.py
--rw-r--r--   0        0        0     2816 1970-01-01 00:00:00.000000 symply-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-16 00:37:19.582472 symply-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2328 2024-04-16 04:44:56.171036 symply-0.1.2/README.md
+-rw-r--r--   0        0        0      503 2024-04-25 11:05:51.820948 symply-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      202 2024-04-16 21:57:45.430130 symply-0.1.2/symply/__init__.py
+-rw-r--r--   0        0        0     4167 2024-04-25 11:04:49.340959 symply-0.1.2/symply/symply.py
+-rw-r--r--   0        0        0     4885 2024-04-21 06:22:15.562616 symply-0.1.2/symply/watcher.py
+-rw-r--r--   0        0        0     2816 1970-01-01 00:00:00.000000 symply-0.1.2/PKG-INFO
```

### Comparing `symply-0.1.1/LICENSE` & `symply-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `symply-0.1.1/README.md` & `symply-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `symply-0.1.1/symply/symply.py` & `symply-0.1.2/symply/symply.py`

 * *Files 19% similar despite different names*

```diff
@@ -22,86 +22,87 @@
 """
 import logging
 import os
 
 logger = logging.getLogger(__name__)
 
 
-def symlink(source: str, target: str, force: bool = False) -> None:
+def symlink(source: str, target: str, force: bool = False) -> bool:
     """
     Create a symlink from source to target. Optionally, overwrite any existing symlink if `force` is True.
 
     Args:
         source (str): The path to the source file.
         target (str): The path where the symlink will be created.
         force (bool): If True, overwrite an existing symlink if it exists.
 
     Raises:
         TypeError: If any of the parameters are not of the expected type.
         ValueError: If source or target is an empty string.
-        FileNotFoundError: If the source file or target directory does not exist.
-        FileExistsError: If the symlink already exists and points to a different source, and force is False.
+        FileNotFoundError: If the source file does not exist.
+        FileExistsError: If the target already exists and force is not True.
         Exception: If the symlink creation fails for other reasons.
 
     Returns:
-        None: A successful operation is indicated by the function completing without raising an exception.
+        bool: True if the symlink was created successfully, otherwise False.
     """
-    if not isinstance(source, str) or not isinstance(target, str):
+    if not (isinstance(source, str) and isinstance(target, str)):
         raise TypeError("Source and target must be strings")
     if not isinstance(force, bool):
         raise TypeError("Force must be a boolean")
-
     if not source or not target:
         raise ValueError("Source and target must be non-empty strings")
 
-    source: str = os.path.abspath(source)
-    target: str = os.path.abspath(target)
+    source = os.path.abspath(source)
+    target = os.path.abspath(target)
 
     if not os.path.exists(source):
-        raise FileNotFoundError(f"Source file does not exist: {source}")
+        raise FileNotFoundError(f"Source file or directory does not exist: {source}")
 
-    target_dir: str = os.path.dirname(target)
+    target_dir = os.path.dirname(target)
     if not os.path.exists(target_dir):
         os.makedirs(target_dir)
         logger.info(f"Created missing directory: {target_dir}")
 
     if os.path.lexists(target):
-        current_target: str | None = os.readlink(target) if os.path.islink(target) else None
-        if current_target != source:
-            if force:
-                os.unlink(target)
-                logger.info(f"Removed existing link: {target}")
+        if os.path.islink(target):
+            current_target = os.path.realpath(target)
+            if current_target != source:
+                if force:
+                    os.unlink(target)
+                    logger.info(f"Removed existing link: {target}")
+                else:
+                    raise FileExistsError(f"Symlink exists and points to a different source: {current_target}")
+        elif force:
+            if os.path.isfile(target) or os.path.isdir(target):
+                os.remove(target)
+                logger.info(f"Removed existing file or directory: {target}")
             else:
-                raise FileExistsError(
-                    f"Symlink already exists and points to a different source: {current_target}"
-                )
-
-    if not os.path.exists(target):
-        os.symlink(source, target)
-        logger.info(f"Symlink created: {target} -> {source}")
-    else:
-        logger.info(f"Symlink points correctly: {target} -> {source}")
+                raise FileExistsError(f"File or directory exists and is not a symlink: {target}")
+        else:
+            raise FileExistsError(f"File or directory exists and is not a symlink: {target}")
 
-    if not os.path.islink(target) or os.readlink(target) != source:
+    os.symlink(source, target)
+    if not os.path.islink(target) or os.path.realpath(target) != source:
         raise Exception("Failed to create or validate the symlink")
 
+    logger.info(f"Symlink created: {target} -> {source}")
+    return True
 
-def delete_symlink(target):
-    """Deletes a symlink if it exists.
-
-    Args:
-        target (str): The path to the symlink to delete.
 
-    Returns:
-        bool: True if the symlink was successfully deleted, False otherwise.
-    """
-    try:
-        if os.path.islink(target):
-            os.unlink(target)
-            logger.info(f"Symlink deleted: {target}")
-            return True
-        else:
-            logger.error(f"No symlink found at {target}")
-            return False
-    except OSError as e:
-        logger.error(f"Failed to delete symlink: {e}")
+def delete_symlink(target, remove_source=False) -> bool:
+    """Remove a symlink at the specified target path and optionally remove the source file or directory."""
+    if not os.path.islink(target):
         return False
+
+    source = os.path.realpath(target)
+    os.unlink(target)
+    logger.info(f"Deleted symlink: {target}")
+
+    if remove_source:
+        if os.path.isfile(source):
+            os.remove(source)
+            logger.info(f"Deleted source file: {source}")
+        elif os.path.isdir(source):
+            os.rmdir(source)
+            logger.info(f"Deleted source directory: {source}")
+    return True
```

### Comparing `symply-0.1.1/symply/watcher.py` & `symply-0.1.2/symply/watcher.py`

 * *Files identical despite different names*

### Comparing `symply-0.1.1/PKG-INFO` & `symply-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symply
-Version: 0.1.1
+Version: 0.1.2
 Summary: Effortless Symlink Management as a Python Package!
 License: MIT
 Author: Spoked
 Author-email: dreu.lavelle@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

