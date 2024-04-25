# Comparing `tmp/pypomes_store-0.2.6.tar.gz` & `tmp/pypomes_store-0.2.7.tar.gz`

## Comparing `pypomes_store-0.2.6.tar` & `pypomes_store-0.2.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_store-0.2.6/src/__init__.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 pypomes_store-0.2.6/src/pypomes_store/__init__.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 pypomes_store-0.2.6/src/pypomes_store/minio_client.py
--rw-r--r--   0        0        0    14698 2020-02-02 00:00:00.000000 pypomes_store-0.2.6/src/pypomes_store/minio_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_store-0.2.6/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_store-0.2.6/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_store-0.2.6/README.md
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 pypomes_store-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pypomes_store-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_store-0.2.7/src/__init__.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 pypomes_store-0.2.7/src/pypomes_store/__init__.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 pypomes_store-0.2.7/src/pypomes_store/minio_client.py
+-rw-r--r--   0        0        0    15337 2020-02-02 00:00:00.000000 pypomes_store-0.2.7/src/pypomes_store/minio_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_store-0.2.7/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_store-0.2.7/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_store-0.2.7/README.md
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 pypomes_store-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pypomes_store-0.2.7/PKG-INFO
```

### Comparing `pypomes_store-0.2.6/src/pypomes_store/__init__.py` & `pypomes_store-0.2.7/src/pypomes_store/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_store-0.2.6/src/pypomes_store/minio_client.py` & `pypomes_store-0.2.7/src/pypomes_store/minio_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,16 +50,18 @@
         """
         First step in providing a context-managed *MinIO* client.
 
         :return: a Minio client object
         """
         return self.minio_client
 
-    def __exit__(self, exception_type: type[BaseException],
-                 exception_value: BaseException, traceback: TracebackType) -> bool:
+    def __exit__(self,
+                 exception_type: type[BaseException],
+                 exception_value: BaseException,
+                 traceback: TracebackType) -> bool:
         """
         Last step in providing a context-managed *MinIO* client.
         """
         self.minio_client = None
 
         # make sure an eventual exception is propagated
         return exception_type is None
```

### Comparing `pypomes_store-0.2.6/src/pypomes_store/minio_pomes.py` & `pypomes_store-0.2.7/src/pypomes_store/minio_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,16 +67,20 @@
             result = True
     except Exception as e:
         errors.append(__minio_except_msg(e))
 
     return result
 
 
-def minio_file_store(errors: list[str], basepath: Path | str,
-                     identifier: str, filepath: Path | str, mimetype: str, tags: dict = None) -> None:
+def minio_file_store(errors: list[str],
+                     basepath: Path | str,
+                     identifier: str,
+                     filepath: Path | str,
+                     mimetype: str,
+                     tags: dict = None) -> None:
     """
     Store a file at the *MinIO* store.
 
     :param errors: incidental error messages
     :param basepath: the path specifying the location to store the file at
     :param identifier: the file identifier, tipically a file name
     :param filepath: the path specifying where the file is
@@ -106,25 +110,30 @@
                                      file_path=filepath,
                                      content_type=mimetype,
                                      tags=doc_tags)
     except Exception as e:
         errors.append(__minio_except_msg(e))
 
 
-def minio_file_retrieve(errors: list[str], basepath: Path | str,
-                        identifier: str, filepath: Path | str) -> any:
+def minio_file_retrieve(errors: list[str],
+                        basepath: Path | str,
+                        identifier: str,
+                        filepath: Path | str) -> any:
     """
     Retrieve a file from the *MinIO* store.
 
     :param errors: incidental error messages
     :param basepath: the path specifying the location to retrieve the file from
     :param identifier: the file identifier, tipically a file name
     :param filepath: the path to save the retrieved file at
     :return: information about the file retrieved
     """
+    # initialize the return variable
+    result: any = None
+
     # obtain the MinIO client and proceed
     try:
         with MinioCM(endpoint=MINIO_HOST,
                      access_key=MINIO_ACCESS_KEY,
                      secret_key=MINIO_SECRET_KEY,
                      secure=MINIO_SECURE_ACCESS) as minio_client:
             remotepath: Path = Path(basepath) / identifier
@@ -137,15 +146,17 @@
                     errors.append(__minio_except_msg(e))
     except Exception as e:
         errors.append(__minio_except_msg(e))
 
     return result
 
 
-def minio_object_exists(errors: list[str], basepath: Path | str, identifier: str = None) -> bool:
+def minio_object_exists(errors: list[str],
+                        basepath: Path | str,
+                        identifier: str = None) -> bool:
     """
     Determine if a given object exists in the *MinIO* store.
 
     :param errors: incidental error messages
     :param basepath: the path specifying the location to locate the object at
     :param identifier: the object identifier
     :return: True if the object was found
@@ -163,15 +174,17 @@
     # verify the status of the object
     elif minio_object_stat(errors, basepath, identifier):
         result = True
 
     return result
 
 
-def minio_object_stat(errors: list[str], basepath: Path | str, identifier: str) -> MinioObject:
+def minio_object_stat(errors: list[str],
+                      basepath: Path | str,
+                      identifier: str) -> MinioObject:
     """
     Retrieve and return the information about an object in the *MinIO* store.
 
     :param errors: incidental error messages
     :param basepath: the path specifying where to locate the object
     :param identifier: the object identifier
     :return: metadata and information about the object
@@ -194,16 +207,19 @@
                     errors.append(__minio_except_msg(e))
     except Exception as e:
         errors.append(__minio_except_msg(e))
 
     return result
 
 
-def minio_object_store(errors: list[str], basepath: Path | str,
-                       identifier: str, obj: any, tags: dict = None) -> None:
+def minio_object_store(errors: list[str],
+                       basepath: Path | str,
+                       identifier: str,
+                       obj: any,
+                       tags: dict = None) -> None:
     """
     Store an object at the *MinIO* store.
 
     :param errors: incidental error messages
     :param basepath: the path specifying the location to store the object at
     :param identifier: the object identifier
     :param obj: object to be stored
@@ -219,15 +235,17 @@
 
     # was the file stored ?
     if len(errors) == 0:
         # yes, remove it from the file system
         Path.unlink(filepath)
 
 
-def minio_object_retrieve(errors: list[str], basepath: Path, identifier: str) -> any:
+def minio_object_retrieve(errors: list[str],
+                          basepath: Path,
+                          identifier: str) -> any:
     """
     Retrieve an object from the *MinIO* store.
 
     :param errors: incidental error messages
     :param basepath: the path specifying the location to retrieve the object from
     :param identifier: the object identifier
     :return: the object retrieved
@@ -245,15 +263,17 @@
         with Path.open(filepath, "rb") as f:
             result = pickle.load(f)
         Path.unlink(filepath)
 
     return result
 
 
-def minio_object_delete(errors: list[str], basepath: str, identifier: str = None) -> None:
+def minio_object_delete(errors: list[str],
+                        basepath: str,
+                        identifier: str = None) -> None:
     """
     Remove an object from the *MinIO* store.
 
     :param errors: incidental error messages
     :param basepath: the path specifying the location to retrieve the object from
     :param identifier: the object identifier
     """
@@ -277,15 +297,17 @@
                     if not hasattr(e, "code") or e.code != "NoSuchKey":
                         errors.append(__minio_except_msg(e))
     except Exception as e:
         errors.append(__minio_except_msg(e))
 
 
 # recupera as tags do objeto
-def minio_object_tags_retrieve(errors: list[str], basepath: str, identifier: str) -> dict:
+def minio_object_tags_retrieve(errors: list[str],
+                               basepath: str,
+                               identifier: str) -> dict:
     """
     Retrieve and return the metadata information for an object in the *MinIO* store.
 
     :param errors: incidental error messages
     :param basepath: the path specifying the location to retrieve the object from
     :param identifier: the object identifier
     :return: the metadata about the object
@@ -310,15 +332,17 @@
                     errors.append(__minio_except_msg(e))
     except Exception as e:
         errors.append(__minio_except_msg(e))
 
     return result
 
 
-def minio_objects_list(errors: list[str], basepath: str, recursive: bool = False) -> Iterator:
+def minio_objects_list(errors: list[str],
+                       basepath: str,
+                       recursive: bool = False) -> Iterator:
     """
     Retrieve and return an iterator into the list of objects at *basepath*, in the *MinIO* store.
 
     :param errors: incidental error messages
     :param basepath: the path specifying the location to iterate from
     :param recursive: whether the location is iterated recursively
     :return: the iterator into the list of objects, 'None' if the folder does not exist
@@ -337,15 +361,17 @@
                                                recursive=recursive)
     except Exception as e:
         errors.append(__minio_except_msg(e))
 
     return result
 
 
-def __minio_folder_delete(errors: list[str],  minio_client: Minio, basepath: str) -> None:
+def __minio_folder_delete(errors: list[str],
+                          minio_client: Minio,
+                          basepath: str) -> None:
     """
     Traverse the folders recursively, removing its objects.
 
     :param errors: incidental error messages
     :param minio_client: the MinIO client object
     :param basepath: the path specifying the location to delete the objects at.
     """
```

### Comparing `pypomes_store-0.2.6/LICENSE` & `pypomes_store-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_store-0.2.6/pyproject.toml` & `pypomes_store-0.2.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_store"
-version = "0.2.6"
+version = "0.2.7"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (object storage modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "minio>=7.2.5",
     "pip>=24.0",
-    "pypomes_core>=0.8.4",
+    "pypomes_core>=0.8.8",
     "setuptools>=68.0.0",
     "Unidecode>=1.3.6",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-Store"
```

### Comparing `pypomes_store-0.2.6/PKG-INFO` & `pypomes_store-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.3
 Name: pypomes_store
-Version: 0.2.6
+Version: 0.2.7
 Summary: A collection of Python pomes, pennyeach (object storage modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Store
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Store/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: minio>=7.2.5
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=0.8.4
+Requires-Dist: pypomes-core>=0.8.8
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: unidecode>=1.3.6
 Requires-Dist: wheel>=0.42.0
```

