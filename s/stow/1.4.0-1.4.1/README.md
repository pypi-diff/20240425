# Comparing `tmp/stow-1.4.0.tar.gz` & `tmp/stow-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stow-1.4.0.tar", last modified: Tue Apr 23 10:42:57 2024, max compression
+gzip compressed data, was "stow-1.4.1.tar", last modified: Thu Apr 25 09:46:48 2024, max compression
```

## Comparing `stow-1.4.0.tar` & `stow-1.4.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 10:42:57.880548 stow-1.4.0/
--rw-rw-rw-   0        0        0    10756 2023-03-26 22:44:13.000000 stow-1.4.0/LICENSE
--rw-rw-rw-   0        0        0    21448 2024-04-23 10:42:57.880548 stow-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      410 2024-01-21 14:29:30.000000 stow-1.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 10:42:57.827375 stow-1.4.0/docs/
--rw-rw-rw-   0        0        0    19244 2023-08-04 17:54:30.000000 stow-1.4.0/docs/index.md
--rw-rw-rw-   0        0        0       86 2023-03-26 22:44:13.000000 stow-1.4.0/pyproject.toml
--rw-rw-rw-   0        0        0     1382 2024-04-23 10:42:57.886399 stow-1.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-23 10:42:57.837733 stow-1.4.0/stow/
--rw-rw-rw-   0        0        0     2022 2024-04-23 10:42:04.000000 stow-1.4.0/stow/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 10:42:57.860715 stow-1.4.0/stow/artefacts/
--rw-rw-rw-   0        0        0       86 2024-01-21 14:29:30.000000 stow-1.4.0/stow/artefacts/__init__.py
--rw-rw-rw-   0        0        0    22235 2024-04-23 10:42:04.000000 stow-1.4.0/stow/artefacts/artefacts.py
--rw-rw-rw-   0        0        0     5221 2024-04-23 10:42:04.000000 stow-1.4.0/stow/artefacts/interfaces.py
--rw-rw-rw-   0        0        0      413 2024-01-21 14:29:30.000000 stow-1.4.0/stow/artefacts/types.py
--rw-rw-rw-   0        0        0     7895 2024-04-23 10:42:04.000000 stow-1.4.0/stow/callbacks.py
--rw-rw-rw-   0        0        0    12517 2024-04-23 10:42:04.000000 stow-1.4.0/stow/cli.py
--rw-rw-rw-   0        0        0      938 2024-01-21 14:29:30.000000 stow-1.4.0/stow/exceptions.py
--rw-rw-rw-   0        0        0      517 2024-01-21 14:29:30.000000 stow-1.4.0/stow/localiser.py
-drwxrwxrwx   0        0        0        0 2024-04-23 10:42:57.866034 stow-1.4.0/stow/manager/
--rw-rw-rw-   0        0        0      130 2024-04-23 10:42:04.000000 stow-1.4.0/stow/manager/__init__.py
--rw-rw-rw-   0        0        0    15058 2024-04-23 10:42:04.000000 stow-1.4.0/stow/manager/abstract_methods.py
--rw-rw-rw-   0        0        0     7335 2024-01-21 14:29:30.000000 stow-1.4.0/stow/manager/base_managers.py
--rw-rw-rw-   0        0        0      290 2024-04-23 10:42:04.000000 stow-1.4.0/stow/manager/configs.py
--rw-rw-rw-   0        0        0    70711 2024-04-23 10:42:04.000000 stow-1.4.0/stow/manager/manager.py
-drwxrwxrwx   0        0        0        0 2024-04-23 10:42:57.872093 stow-1.4.0/stow/managers/
--rw-rw-rw-   0        0        0       26 2023-05-23 16:38:50.000000 stow-1.4.0/stow/managers/__init__.py
--rw-rw-rw-   0        0        0    52725 2024-04-23 10:42:04.000000 stow-1.4.0/stow/managers/amazon.py
--rw-rw-rw-   0        0        0    21754 2024-04-23 10:42:04.000000 stow-1.4.0/stow/managers/filesystem.py
--rw-rw-rw-   0        0        0     1775 2024-04-23 10:42:04.000000 stow-1.4.0/stow/managers/google.py
--rw-rw-rw-   0        0        0    23022 2024-04-23 10:42:04.000000 stow-1.4.0/stow/managers/kubernetes.py
--rw-rw-rw-   0        0        0    14458 2024-01-21 14:29:30.000000 stow-1.4.0/stow/managers/ssh.py
--rw-rw-rw-   0        0        0     1050 2024-01-21 14:29:30.000000 stow-1.4.0/stow/storage_classes.py
--rw-rw-rw-   0        0        0      411 2024-01-21 14:29:30.000000 stow-1.4.0/stow/types.py
--rw-rw-rw-   0        0        0     3181 2024-01-21 14:29:30.000000 stow-1.4.0/stow/utils.py
--rw-rw-rw-   0        0        0     4723 2024-04-23 10:42:04.000000 stow-1.4.0/stow/worker_config.py
-drwxrwxrwx   0        0        0        0 2024-04-23 10:42:57.878042 stow-1.4.0/stow.egg-info/
--rw-rw-rw-   0        0        0    21448 2024-04-23 10:42:57.000000 stow-1.4.0/stow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      865 2024-04-23 10:42:57.000000 stow-1.4.0/stow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 10:42:57.000000 stow-1.4.0/stow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      152 2024-04-23 10:42:57.000000 stow-1.4.0/stow.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      386 2024-04-23 10:42:57.000000 stow-1.4.0/stow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-23 10:42:57.000000 stow-1.4.0/stow.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-23 10:42:57.876774 stow-1.4.0/tests/
--rw-rw-rw-   0        0        0     1959 2024-01-21 14:29:30.000000 stow-1.4.0/tests/test_callbacks.py
--rw-rw-rw-   0        0        0    11244 2024-01-22 18:56:13.000000 stow-1.4.0/tests/test_cli.py
--rw-rw-rw-   0        0        0    34145 2024-01-22 18:55:59.000000 stow-1.4.0/tests/test_stateless.py
--rw-rw-rw-   0        0        0     2798 2024-01-21 14:29:30.000000 stow-1.4.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 09:46:48.098695 stow-1.4.1/
+-rw-rw-rw-   0        0        0    10756 2023-03-26 22:44:13.000000 stow-1.4.1/LICENSE
+-rw-rw-rw-   0        0        0    21448 2024-04-25 09:46:48.098695 stow-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2024-01-21 14:29:30.000000 stow-1.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 09:46:47.917626 stow-1.4.1/docs/
+-rw-rw-rw-   0        0        0    19244 2023-08-04 17:54:30.000000 stow-1.4.1/docs/index.md
+-rw-rw-rw-   0        0        0       86 2023-03-26 22:44:13.000000 stow-1.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1382 2024-04-25 09:46:48.100678 stow-1.4.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-25 09:46:47.967861 stow-1.4.1/stow/
+-rw-rw-rw-   0        0        0     2022 2024-04-23 10:42:04.000000 stow-1.4.1/stow/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 09:46:48.007774 stow-1.4.1/stow/artefacts/
+-rw-rw-rw-   0        0        0       86 2024-01-21 14:29:30.000000 stow-1.4.1/stow/artefacts/__init__.py
+-rw-rw-rw-   0        0        0    22308 2024-04-25 09:43:20.000000 stow-1.4.1/stow/artefacts/artefacts.py
+-rw-rw-rw-   0        0        0     5221 2024-04-23 10:42:04.000000 stow-1.4.1/stow/artefacts/interfaces.py
+-rw-rw-rw-   0        0        0      413 2024-01-21 14:29:30.000000 stow-1.4.1/stow/artefacts/types.py
+-rw-rw-rw-   0        0        0     7895 2024-04-23 10:42:04.000000 stow-1.4.1/stow/callbacks.py
+-rw-rw-rw-   0        0        0    12517 2024-04-23 10:42:04.000000 stow-1.4.1/stow/cli.py
+-rw-rw-rw-   0        0        0      938 2024-01-21 14:29:30.000000 stow-1.4.1/stow/exceptions.py
+-rw-rw-rw-   0        0        0      517 2024-01-21 14:29:30.000000 stow-1.4.1/stow/localiser.py
+drwxrwxrwx   0        0        0        0 2024-04-25 09:46:48.035100 stow-1.4.1/stow/manager/
+-rw-rw-rw-   0        0        0      130 2024-04-23 10:42:04.000000 stow-1.4.1/stow/manager/__init__.py
+-rw-rw-rw-   0        0        0    15194 2024-04-25 09:43:20.000000 stow-1.4.1/stow/manager/abstract_methods.py
+-rw-rw-rw-   0        0        0     7335 2024-01-21 14:29:30.000000 stow-1.4.1/stow/manager/base_managers.py
+-rw-rw-rw-   0        0        0      290 2024-04-23 10:42:04.000000 stow-1.4.1/stow/manager/configs.py
+-rw-rw-rw-   0        0        0    71716 2024-04-25 09:43:20.000000 stow-1.4.1/stow/manager/manager.py
+drwxrwxrwx   0        0        0        0 2024-04-25 09:46:48.069845 stow-1.4.1/stow/managers/
+-rw-rw-rw-   0        0        0       26 2023-05-23 16:38:50.000000 stow-1.4.1/stow/managers/__init__.py
+-rw-rw-rw-   0        0        0    53526 2024-04-25 09:43:20.000000 stow-1.4.1/stow/managers/amazon.py
+-rw-rw-rw-   0        0        0    21754 2024-04-23 10:42:04.000000 stow-1.4.1/stow/managers/filesystem.py
+-rw-rw-rw-   0        0        0     1775 2024-04-23 10:42:04.000000 stow-1.4.1/stow/managers/google.py
+-rw-rw-rw-   0        0        0    23022 2024-04-23 10:42:04.000000 stow-1.4.1/stow/managers/kubernetes.py
+-rw-rw-rw-   0        0        0    14458 2024-01-21 14:29:30.000000 stow-1.4.1/stow/managers/ssh.py
+-rw-rw-rw-   0        0        0     1050 2024-01-21 14:29:30.000000 stow-1.4.1/stow/storage_classes.py
+-rw-rw-rw-   0        0        0      411 2024-01-21 14:29:30.000000 stow-1.4.1/stow/types.py
+-rw-rw-rw-   0        0        0     3181 2024-01-21 14:29:30.000000 stow-1.4.1/stow/utils.py
+-rw-rw-rw-   0        0        0     4723 2024-04-23 10:42:04.000000 stow-1.4.1/stow/worker_config.py
+drwxrwxrwx   0        0        0        0 2024-04-25 09:46:48.096618 stow-1.4.1/stow.egg-info/
+-rw-rw-rw-   0        0        0    21448 2024-04-25 09:46:47.000000 stow-1.4.1/stow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      865 2024-04-25 09:46:47.000000 stow-1.4.1/stow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 09:46:47.000000 stow-1.4.1/stow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      152 2024-04-25 09:46:47.000000 stow-1.4.1/stow.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      386 2024-04-25 09:46:47.000000 stow-1.4.1/stow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-25 09:46:47.000000 stow-1.4.1/stow.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 09:46:48.094557 stow-1.4.1/tests/
+-rw-rw-rw-   0        0        0     1959 2024-01-21 14:29:30.000000 stow-1.4.1/tests/test_callbacks.py
+-rw-rw-rw-   0        0        0    11244 2024-01-22 18:56:13.000000 stow-1.4.1/tests/test_cli.py
+-rw-rw-rw-   0        0        0    34145 2024-01-22 18:55:59.000000 stow-1.4.1/tests/test_stateless.py
+-rw-rw-rw-   0        0        0     2798 2024-01-21 14:29:30.000000 stow-1.4.1/tests/test_utils.py
```

### Comparing `stow-1.4.0/LICENSE` & `stow-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stow-1.4.0/PKG-INFO` & `stow-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stow
-Version: 1.4.0
+Version: 1.4.1
 Summary: stow artefacts anywhere, with ease
 Author: Kieran Bacon
 Author-email: kieran.bacon@outlook.com
 Project-URL: Homepage, https://github.com/Kieran-Bacon/stow
 Project-URL: Documentation, https://stow.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/Kieran-Bacon/stow/issues
 Keywords: aws s3 boto3 ssh os
```

### Comparing `stow-1.4.0/docs/index.md` & `stow-1.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `stow-1.4.0/setup.cfg` & `stow-1.4.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 746f 770d 0a76 6572 7369 6f6e   = stow..version
-00000020: 203d 2031 2e34 2e30 0d0a 6175 7468 6f72   = 1.4.0..author
+00000020: 203d 2031 2e34 2e31 0d0a 6175 7468 6f72   = 1.4.1..author
 00000030: 203d 204b 6965 7261 6e20 4261 636f 6e0d   = Kieran Bacon.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 6b69 6572 616e 2e62 6163 6f6e 406f 7574  kieran.bacon@out
 00000060: 6c6f 6f6b 2e63 6f6d 0d0a 6465 7363 7269  look.com..descri
 00000070: 7074 696f 6e20 3d20 7374 6f77 2061 7274  ption = stow art
 00000080: 6566 6163 7473 2061 6e79 7768 6572 652c  efacts anywhere,
 00000090: 2077 6974 6820 6561 7365 0d0a 6c6f 6e67   with ease..long
```

### Comparing `stow-1.4.0/stow/__init__.py` & `stow-1.4.1/stow/__init__.py`

 * *Files identical despite different names*

### Comparing `stow-1.4.0/stow/artefacts/artefacts.py` & `stow-1.4.1/stow/artefacts/artefacts.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,23 +31,25 @@
         self,
         manager: ManagerInterface,
         path: str,
         *,
         createdTime: Optional[datetime.datetime] = None,
         modifiedTime: Optional[datetime.datetime] = None,
         accessedTime: Optional[datetime.datetime] = None,
+        tags: Optional[Dict[str, str]] = None,
         metadata: Optional[Dict[str, str]] = None,
         ):
 
         self._manager = manager  # Link back to the owning manager
         self._path = path  # Relative path on manager
 
         self._createdTime = createdTime
         self._modifiedTime = modifiedTime
         self._accessedTime = accessedTime
+        self._tags = tags
         self._metadata = metadata
 
     def __reduce__(self):
         return (ArtefactReloader, (self._manager.protocol, self._manager.config, self._path))
 
     def __hash__(self):
         return hash(self.abspath)
```

### Comparing `stow-1.4.0/stow/artefacts/interfaces.py` & `stow-1.4.1/stow/artefacts/interfaces.py`

 * *Files identical despite different names*

### Comparing `stow-1.4.0/stow/callbacks.py` & `stow-1.4.1/stow/callbacks.py`

 * *Files identical despite different names*

### Comparing `stow-1.4.0/stow/cli.py` & `stow-1.4.1/stow/cli.py`

 * *Files identical despite different names*

### Comparing `stow-1.4.0/stow/exceptions.py` & `stow-1.4.1/stow/exceptions.py`

 * *Files identical despite different names*

### Comparing `stow-1.4.0/stow/localiser.py` & `stow-1.4.1/stow/localiser.py`

 * *Files identical despite different names*

### Comparing `stow-1.4.0/stow/manager/abstract_methods.py` & `stow-1.4.1/stow/manager/abstract_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,14 +182,15 @@
     @abstractmethod
     def _put(
         self,
         source: Artefact,
         destination: str,
         /,
         callback: AbstractCallback,
+        tags: Optional[Metadata],
         metadata: Optional[Metadata],
         modified_time: Optional[TimestampLike],
         accessed_time: Optional[TimestampLike],
         content_type: Optional[str],
         storage_class: Optional[StorageClass],
         worker_config: WorkerPoolConfig,
         delete_source: bool = False
@@ -211,14 +212,15 @@
     @abstractmethod
     def _putBytes(
         self,
         fileBytes: bytes,
         destination: str,
         *,
         callback: AbstractCallback,
+        tags: Optional[Metadata],
         metadata: Optional[Metadata],
         modified_time: Optional[float],
         accessed_time: Optional[float],
         content_type: Optional[str],
         storage_class: Optional[StorageClass],
         ) -> File:
         """ Put the bytes of a file object onto the underlying manager implementation using the absolute path given.
@@ -239,14 +241,15 @@
     def _cp(
         self,
         source: Artefact,
         destination: str,
         /,
         callback: AbstractCallback,
         worker_config: WorkerPoolConfig,
+        tags: Optional[Metadata],
         metadata: Optional[Metadata],
         modified_time: Optional[float],
         accessed_time: Optional[float],
         content_type: Optional[str],
         storage_class: Optional[StorageClass],
         ) -> ArtefactType:
         """ Method for copying an artefact local to the manager to another location on the manager. Implementation
@@ -267,14 +270,15 @@
     def _mv(
         self,
         source: Artefact,
         destination: str,
         /,
         callback: AbstractCallback,
         worker_config: WorkerPoolConfig,
+        tags: Optional[Metadata],
         metadata: Optional[Metadata],
         modified_time: Optional[float],
         accessed_time: Optional[float],
         storage_class: Optional[StorageClass],
         content_type: Optional[str],
         ) -> ArtefactType:
         """ Move an artefact from its location to another location managed by the same manager class. This method should
```

### Comparing `stow-1.4.0/stow/manager/base_managers.py` & `stow-1.4.1/stow/manager/base_managers.py`

 * *Files identical despite different names*

### Comparing `stow-1.4.0/stow/manager/manager.py` & `stow-1.4.1/stow/manager/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1113,14 +1113,15 @@
     def put(
         self,
         source: Union[File, bytes],
         destination: ArtefactOrPathLike,
         overwrite: bool = False,
         *,
         callback: AbstractCallback = DefaultCallback(),
+        tags: Optional[Metadata] = None,
         metadata: Optional[Metadata] = None,
         modified_time: Optional[TimestampLike] = None,
         accessed_time: Optional[TimestampLike] = None,
         content_type: Optional[str] = None,
         storage_class: Optional[StorageClass] = None,
         worker_config: Optional[WorkerPoolConfig] = None,
         ) -> File:
@@ -1128,14 +1129,15 @@
     @overload
     def put(
         self,
         source: Directory,
         destination: ArtefactOrPathLike,
         overwrite: bool = False,
         *,
+        tags: Optional[Metadata] = None,
         metadata: Optional[Metadata] = None,
         callback: AbstractCallback = DefaultCallback(),
         modified_time: Optional[TimestampLike] = None,
         accessed_time: Optional[TimestampLike] = None,
         content_type: Optional[str] = None,
         storage_class: Optional[StorageClass] = None,
         worker_config: Optional[WorkerPoolConfig] = None,
@@ -1144,14 +1146,15 @@
     @overload
     def put(
         self,
         source: ArtefactOrPathLike,
         destination: ArtefactOrPathLike,
         overwrite: bool = False,
         *,
+        tags: Optional[Metadata] = None,
         metadata: Optional[Metadata] = None,
         callback: AbstractCallback = DefaultCallback(),
         modified_time: Optional[TimestampLike] = None,
         accessed_time: Optional[TimestampLike] = None,
         content_type: Optional[str] = None,
         storage_class: Optional[StorageClass] = None,
         worker_config: Optional[WorkerPoolConfig] = None,
@@ -1159,14 +1162,15 @@
         pass
     def put(
         self,
         source: Union[ArtefactOrPathLike, bytes],
         destination: ArtefactOrPathLike,
         overwrite: bool = False,
         *,
+        tags: Optional[Metadata] = None,
         metadata: Optional[Metadata] = None,
         callback: AbstractCallback = DefaultCallback(),
         modified_time: Optional[TimestampLike] = None,
         accessed_time: Optional[TimestampLike] = None,
         content_type: Optional[str] = None,
         storage_class: Optional[StorageClass] = None,
         worker_config: Optional[WorkerPoolConfig] = None,
@@ -1205,14 +1209,15 @@
                     callback=callback,
                     worker_config=worker_config
                 )
 
                 putArtefact = destinationManager._putBytes(
                     source,
                     destinationPath,
+                    tags=tags,
                     metadata=metadata,
                     callback=callback,
                     modified_time=utils.timestampToFloatOrNone(modified_time),
                     accessed_time=utils.timestampToFloatOrNone(accessed_time),
                     content_type=content_type,
                     storage_class=storage_class,
                 )
@@ -1229,14 +1234,15 @@
                     callback=callback,
                     worker_config=worker_config
                 )
 
                 putArtefact = destinationManager._put(
                     sourceObj,
                     destinationPath,
+                    tags=tags,
                     metadata=metadata,
                     callback=callback,
                     modified_time=modified_time,
                     accessed_time=accessed_time,
                     content_type=content_type,
                     storage_class=storage_class,
                     worker_config=worker_config
@@ -1250,14 +1256,15 @@
     def cp(
         self,
         source: ArtefactOrPathLike,
         destination: ArtefactOrPathLike,
         overwrite: bool = False,
         *,
         callback: AbstractCallback = DefaultCallback(),
+        tags: Optional[Metadata] = None,
         metadata: Optional[Metadata] = None,
         modified_time: Optional[datetime.datetime] = None,
         accessed_time: Optional[datetime.datetime] = None,
         storage_class: Optional[StorageClass] = None,
         content_type: Optional[str] = None,
         worker_config: Optional[WorkerPoolConfig] = None,
         ) -> ArtefactType:
@@ -1297,39 +1304,52 @@
             # TODO it may not be possible to copy from one manager of the same type to another manager of the same type
             # but be possible to copy within a manager - need more dials for this.
             if type(sourceManager) == type(destinationManager) and not sourceManager.ISOLATED:
                 copiedArtefact = destinationManager._cp(
                     sourceObj,
                     destinationPath,
                     callback=callback,
+                    tags=tags,
                     metadata=metadata,
                     modified_time=utils.timestampToFloatOrNone(modified_time),
                     accessed_time=utils.timestampToFloatOrNone(accessed_time),
                     storage_class=storage_class,
                     content_type=content_type,
                     worker_config=worker_config,
                 )
 
             else:
 
                 log.warning('Cannot perform copy on manager - defaulting to put for %s->%s', source, destination)
-                copiedArtefact = self.put(sourceObj, destination, callback=callback, worker_config=worker_config)
+                copiedArtefact = destinationManager._put(
+                    sourceObj,
+                    destinationPath,
+                    callback=callback,
+                    tags=tags,
+                    metadata=metadata,
+                    modified_time=utils.timestampToFloatOrNone(modified_time),
+                    accessed_time=utils.timestampToFloatOrNone(accessed_time),
+                    storage_class=storage_class,
+                    content_type=content_type,
+                    worker_config=worker_config,
+                )
 
             return copiedArtefact
 
         finally:
             worker_config.conclude()
 
     def mv(
         self,
         source: ArtefactOrPathLike,
         destination: ArtefactOrPathLike,
         overwrite: bool = False,
         *,
         callback: AbstractCallback = DefaultCallback(),
+        tags: Optional[Metadata] = None,
         metadata: Optional[Metadata] = None,
         content_type: Optional[str] = None,
         modified_time: Optional[datetime.datetime] = None,
         accessed_time: Optional[datetime.datetime] = None,
         storage_class: Optional[StorageClass] = None,
         worker_config: Optional[WorkerPoolConfig] = None,
         ) -> ArtefactType:
@@ -1365,14 +1385,15 @@
 
             # Check if the source and destination are from the same manager class
             if type(sourceManager) == type(destinationManager) and not sourceManager.ISOLATED:
                 movedArtefact = destinationManager._mv(
                     sourceObj,
                     destinationPath,
                     callback=callback,
+                    tags=tags,
                     metadata=metadata,
                     modified_time=utils.timestampToFloatOrNone(modified_time),
                     accessed_time=utils.timestampToFloatOrNone(accessed_time),
                     storage_class=storage_class,
                     content_type=content_type,
                     worker_config=worker_config or WorkerPoolConfig(shutdown=True),
                 )
@@ -1380,14 +1401,15 @@
             else:
 
                 # Moving between manager types - put the object and then delete the old one
                 movedArtefact = destinationManager._put(
                     sourceObj,
                     destinationPath,
                     callback=callback,
+                    tags=tags,
                     metadata=metadata,
                     modified_time=utils.timestampToFloatOrNone(modified_time),
                     accessed_time=utils.timestampToFloatOrNone(accessed_time),
                     storage_class=storage_class,
                     worker_config=worker_config,
                     content_type=content_type,
                     delete_source=True
@@ -1575,14 +1597,15 @@
         *,
         delete: bool = False,
         check_modified_times: bool = True,
         artefact_comparator: Optional[typing.Callable[[File, File], bool]] = None,
 
         content_type: Optional[str] = None,
         storage_class: Optional[StorageClass] = None,
+        tags: Optional[Metadata] = None,
         metadata: Optional[Metadata] = None,
         modified_time: Optional[datetime.datetime] = None,
         accessed_time: Optional[datetime.datetime] = None,
         overwrite: bool = False,
         worker_config: Optional[WorkerPoolConfig] = None,
         callback: AbstractCallback = DefaultCallback()
         ) -> ArtefactType:
@@ -1612,14 +1635,15 @@
         if destinationObj is None:
             log.warning("Syncing: Destination=%s doesn't exist therefore putting entire source=%s", destinationPath, sourceObj)
             return destinationManager.put(
                 source,
                 destinationPath,
                 overwrite=overwrite,
                 callback=callback,
+                tags=tags,
                 metadata=metadata,
                 modified_time=modified_time,
                 accessed_time=accessed_time,
                 storage_class=storage_class,
                 worker_config=worker_config
             )
 
@@ -1630,14 +1654,15 @@
         if type(sourceManager) == type(destinationManager) and not sourceManager.ISOLATED:
             sync_method = destinationManager._cp
 
         else:
             sync_method = destinationManager._put
 
         sync_arguments = {
+            "tags": tags,
             "metadata": metadata,
             "modified_time": utils.timestampToFloatOrNone(modified_time),
             "accessed_time": utils.timestampToFloatOrNone(accessed_time),
             "storage_class": storage_class,
             "overwrite": overwrite,
             "callback": callback,
             "content_type": content_type,
@@ -1783,14 +1808,15 @@
 
     def touch(
         self,
         relpath: ArtefactOrPathLike,
         modified_time: Optional[TimestampLike] = None,
         accessed_time: Optional[TimestampLike] = None,
         *,
+        tags: Optional[Metadata] = None,
         metadata: Optional[Metadata] = None,
         content_type: Optional[str] = None,
         storage_class: Optional[StorageClass] = None
         ) -> File:
         """ Perform the linux touch command to create a empty file at the path provided, or for existing files, update
         their modified timestamps as if there where just created.
 
@@ -1810,14 +1836,15 @@
             return artefact
 
         else:
             log.debug("creating artefact=%s with times mt=%s at=%s", path, modified_time, accessed_time, extra={'method': 'touch'})
             return manager._putBytes(
                 b'',
                 path,
+                tags=tags,
                 metadata=metadata,
                 callback=DefaultCallback(),
                 modified_time=utils.timestampToFloatOrNone(modified_time),
                 accessed_time=utils.timestampToFloatOrNone(accessed_time),
                 storage_class=storage_class,
                 content_type=content_type,
             )
```

### Comparing `stow-1.4.0/stow/managers/amazon.py` & `stow-1.4.1/stow/managers/amazon.py`

 * *Files 2% similar despite different names*

```diff
@@ -895,14 +895,15 @@
         source: ArtefactType,
         destination: str,
         *,
         callback: AbstractCallback,
         worker_config: WorkerPoolConfig,
         content_type: Optional[str],
         storage_class: Optional[StorageClass],
+        tags: Optional[Metadata] = None,
         metadata: Optional[Metadata] = None,
         delete_source: bool = False,
         delete_root: Optional[DeleteRoot] = None,
         **kwargs
         ):
 
         # Mark that we are writting this source
@@ -932,14 +933,15 @@
                     # Put the contents of the directory into the bucket
                     self._put(
                         artefact,
                         '/' + artefact.basename,
                         callback=callback,
                         worker_config=worker_config,
                         content_type=content_type,
+                        tags=tags,
                         metadata=metadata,
                         storage_class=storage_class,
                         delete_source=delete_source,
                         delete_root=delete_root
                     )
 
                 else:
@@ -983,14 +985,17 @@
 
                             file_destination = self.join(
                                 key,
                                 source.relpath(artefact, separator='/'),
                                 separator='/'
                             )
 
+                            if tags is not None:
+                                extra_args['Tagging'] = urllib.parse.urlencode(self._freezeMetadata(tags, artefact))
+
                             if metadata is not None:
                                 extra_args['Metadata'] = self._freezeMetadata(metadata, artefact)
 
                             worker_config.submit(
                                 self._localise_put_file,
                                 artefact,
                                 bucket,
@@ -1027,14 +1032,17 @@
                 if delete_root is not None and delete_root.size == 0:
                     # We moved a number of directories that didn't have any files inside them
                     # We are safe to trigger the delete in the main thread of the directory source
                     delete_root.trigger_delete()
 
             else:
 
+                if tags is not None:
+                    extra_args['Tagging'] = urllib.parse.urlencode(self._freezeMetadata(tags, source))
+
                 if metadata is not None:
                     extra_args['Metadata'] = self._freezeMetadata(metadata, source)
 
                 worker_config.submit(
                     self._localise_put_file,
                     source,
                     bucket,
@@ -1050,14 +1058,15 @@
 
     def _putBytes(
         self,
         fileBytes: bytes,
         destination: str,
         *,
         callback: AbstractCallback,
+        tags: Optional[Metadata] = None,
         metadata: Optional[Metadata] = None,
         content_type: Optional[str],
         storage_class: Optional[StorageClass],
         **kwargs
         ):
         callback.writing(1)
 
@@ -1076,14 +1085,15 @@
             self._s3.upload_fileobj(
                 io.BytesIO(fileBytes),
                 bucket,
                 key,
                 ExtraArgs={
                     "StorageClass": amazon_storage_class.value,
                     "ContentType": (content_type or mimetypes.guess_type(destination)[0] or 'application/octet-stream'),
+                    "Tagging": (urllib.parse.urlencode({str(k): str(v) for k, v in tags.items()}) if tags else ""),
                     "Metadata": ({str(k): str(v) for k, v in metadata.items()} if metadata else {})
                 },
                 Callback=callback.get_bytes_transfer(destination, len(fileBytes)),
                 Config=TransferConfig(use_threads=False)
             )
             callback.written(destination)
 
@@ -1183,15 +1193,16 @@
     def _cp(
         self,
         source: ArtefactType,
         destination: str,
         *,
         move: bool = False,
         callback: AbstractCallback,
-        metadata: Optional[Metadata] = None,
+        tags: Optional[Metadata],
+        metadata: Optional[Metadata],
         content_type: Optional[str],
         storage_class: Optional[StorageClassInterface],
         worker_config: WorkerPoolConfig,
         **kwargs
     ) -> ArtefactType:
 
         # Record that the source is being written into the target
@@ -1213,14 +1224,15 @@
 
             for bucket in sourceManager._s3.list_buckets()['Buckets']:
                 self._cp(
                     Directory(sourceManager, '/' + bucket['Name']),
                     '/'.join((destination, bucket['Name'])),
                     move=False,
                     callback=callback,
+                    tags=tags,
                     metadata=metadata,
                     content_type=content_type,
                     storage_class=storage_class,
                     worker_config=worker_config,
                 )
 
         elif destinationBucket is None:
@@ -1233,14 +1245,15 @@
                 for artefact in source.iterls():
                     if isinstance(artefact, Directory):
                         self._cp(
                             artefact,
                             '/' + artefact.basename,
                             move=False,
                             callback=callback,
+                            tags=tags,
                             metadata=metadata,
                             content_type=content_type,
                             storage_class=storage_class,
                             worker_config=worker_config,
                         )
 
                     else:
@@ -1257,14 +1270,17 @@
             if isinstance(source, Directory):
 
                 for result in sourceManager._list_objects(sourceBucket, sourceKey):
                     callback.writing(len(result))
 
                     for sourceSubKey, sourceSubFile in zip(result.keys, result.files):
 
+                        if tags is not None:
+                            copy_args['Tagging'] = urllib.parse.urlencode(self._freezeMetadata(tags, sourceSubFile))
+
                         if metadata is not None:
                             copy_args['Metadata'] = self._freezeMetadata(metadata, sourceSubFile)
 
                         # Copy the object from the source object to the relative location in the destination location
                         relpath = self.relpath(sourceSubKey, sourceKey, separator='/')
                         if sourceSubKey[-1] == '/':
                             relpath += '/'
```

### Comparing `stow-1.4.0/stow/managers/filesystem.py` & `stow-1.4.1/stow/managers/filesystem.py`

 * *Files identical despite different names*

### Comparing `stow-1.4.0/stow/managers/google.py` & `stow-1.4.1/stow/managers/google.py`

 * *Files identical despite different names*

### Comparing `stow-1.4.0/stow/managers/kubernetes.py` & `stow-1.4.1/stow/managers/kubernetes.py`

 * *Files identical despite different names*

### Comparing `stow-1.4.0/stow/managers/ssh.py` & `stow-1.4.1/stow/managers/ssh.py`

 * *Files identical despite different names*

### Comparing `stow-1.4.0/stow/storage_classes.py` & `stow-1.4.1/stow/storage_classes.py`

 * *Files identical despite different names*

### Comparing `stow-1.4.0/stow/utils.py` & `stow-1.4.1/stow/utils.py`

 * *Files identical despite different names*

### Comparing `stow-1.4.0/stow/worker_config.py` & `stow-1.4.1/stow/worker_config.py`

 * *Files identical despite different names*

### Comparing `stow-1.4.0/stow.egg-info/PKG-INFO` & `stow-1.4.1/stow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stow
-Version: 1.4.0
+Version: 1.4.1
 Summary: stow artefacts anywhere, with ease
 Author: Kieran Bacon
 Author-email: kieran.bacon@outlook.com
 Project-URL: Homepage, https://github.com/Kieran-Bacon/stow
 Project-URL: Documentation, https://stow.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/Kieran-Bacon/stow/issues
 Keywords: aws s3 boto3 ssh os
```

### Comparing `stow-1.4.0/stow.egg-info/SOURCES.txt` & `stow-1.4.1/stow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stow-1.4.0/tests/test_callbacks.py` & `stow-1.4.1/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `stow-1.4.0/tests/test_cli.py` & `stow-1.4.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `stow-1.4.0/tests/test_stateless.py` & `stow-1.4.1/tests/test_stateless.py`

 * *Files identical despite different names*

### Comparing `stow-1.4.0/tests/test_utils.py` & `stow-1.4.1/tests/test_utils.py`

 * *Files identical despite different names*

