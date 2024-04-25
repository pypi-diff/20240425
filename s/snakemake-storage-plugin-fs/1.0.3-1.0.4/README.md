# Comparing `tmp/snakemake_storage_plugin_fs-1.0.3.tar.gz` & `tmp/snakemake_storage_plugin_fs-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_storage_plugin_fs-1.0.3.tar", max compression
+gzip compressed data, was "snakemake_storage_plugin_fs-1.0.4.tar", max compression
```

## Comparing `snakemake_storage_plugin_fs-1.0.3.tar` & `snakemake_storage_plugin_fs-1.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1066 2024-04-17 11:42:38.955679 snakemake_storage_plugin_fs-1.0.3/LICENSE
--rw-r--r--   0        0        0      139 2024-04-17 11:42:38.955679 snakemake_storage_plugin_fs-1.0.3/README.md
--rw-r--r--   0        0        0      948 2024-04-17 11:42:38.955679 snakemake_storage_plugin_fs-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     9266 2024-04-17 11:42:38.955679 snakemake_storage_plugin_fs-1.0.3/snakemake_storage_plugin_fs/__init__.py
--rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 snakemake_storage_plugin_fs-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-25 07:35:13.242998 snakemake_storage_plugin_fs-1.0.4/LICENSE
+-rw-r--r--   0        0        0      139 2024-04-25 07:35:13.242998 snakemake_storage_plugin_fs-1.0.4/README.md
+-rw-r--r--   0        0        0      948 2024-04-25 07:35:13.242998 snakemake_storage_plugin_fs-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     9422 2024-04-25 07:35:13.242998 snakemake_storage_plugin_fs-1.0.4/snakemake_storage_plugin_fs/__init__.py
+-rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 snakemake_storage_plugin_fs-1.0.4/PKG-INFO
```

### Comparing `snakemake_storage_plugin_fs-1.0.3/LICENSE` & `snakemake_storage_plugin_fs-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_storage_plugin_fs-1.0.3/pyproject.toml` & `snakemake_storage_plugin_fs-1.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snakemake-storage-plugin-fs"
-version = "1.0.3"
+version = "1.0.4"
 description = " A Snakemake storage plugin that reads and writes from a locally mounted filesystem using rsync"
 authors = ["Johannes Koester <johannes.koester@uni-due.de>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/snakemake/snakemake-storage-plugin-fs"
 documentation = "https://snakemake.github.io/snakemake-plugin-catalog/plugins/storage/fs.html"
 keywords = ["snakemake", "plugin", "storage", "filesystem", "rsync"]
```

### Comparing `snakemake_storage_plugin_fs-1.0.3/snakemake_storage_plugin_fs/__init__.py` & `snakemake_storage_plugin_fs-1.0.4/snakemake_storage_plugin_fs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,15 +208,19 @@
         # Ensure that the object is stored at the location specified by
         # self.local_path().
         self.query_path.parent.mkdir(exist_ok=True, parents=True)
         # We want to respect the permissions in the target folder, in particular the
         # setgid bit. Hence, we use --no-p to avoid preserving of permissions from the
         # source to the target.
         cmd = sysrsync.get_rsync_command(
-            str(self.local_path()), str(self.query_path), options=["-av", "--no-p"]
+            str(self.local_path()),
+            str(self.query_path),
+            # ensure that permissions and ownership are inherited from destination,
+            # e.g. setgid.
+            options=["-av", "--no-o", "--no-g", "--no-p"],
         )
         self._run_cmd(cmd)
 
     def _run_cmd(self, cmd: list[str]):
         try:
             subprocess.run(
                 cmd, check=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT
```

### Comparing `snakemake_storage_plugin_fs-1.0.3/PKG-INFO` & `snakemake_storage_plugin_fs-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake-storage-plugin-fs
-Version: 1.0.3
+Version: 1.0.4
 Summary:  A Snakemake storage plugin that reads and writes from a locally mounted filesystem using rsync
 Home-page: https://github.com/snakemake/snakemake-storage-plugin-fs
 License: MIT
 Keywords: snakemake,plugin,storage,filesystem,rsync
 Author: Johannes Koester
 Author-email: johannes.koester@uni-due.de
 Requires-Python: >=3.11,<4.0
```

