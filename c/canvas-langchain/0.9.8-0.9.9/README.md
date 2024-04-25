# Comparing `tmp/canvas_langchain-0.9.8.tar.gz` & `tmp/canvas_langchain-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canvas_langchain-0.9.8.tar", last modified: Sat Jan 27 13:01:15 2024, max compression
+gzip compressed data, was "canvas_langchain-0.9.9.tar", last modified: Wed Jan 31 18:02:07 2024, max compression
```

## Comparing `canvas_langchain-0.9.8.tar` & `canvas_langchain-0.9.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jparisea   (501) staff       (20)        0 2024-01-27 13:01:15.387978 canvas_langchain-0.9.8/
--rw-r--r--   0 jparisea   (501) staff       (20)    35148 2023-07-31 20:28:17.000000 canvas_langchain-0.9.8/LICENSE.txt
--rw-r--r--   0 jparisea   (501) staff       (20)     2411 2024-01-27 13:01:15.387774 canvas_langchain-0.9.8/PKG-INFO
--rw-r--r--   0 jparisea   (501) staff       (20)     1590 2024-01-27 12:17:35.000000 canvas_langchain-0.9.8/README.md
-drwxr-xr-x   0 jparisea   (501) staff       (20)        0 2024-01-27 13:01:15.386704 canvas_langchain-0.9.8/canvas_langchain/
--rw-r--r--   0 jparisea   (501) staff       (20)        0 2023-07-31 15:52:56.000000 canvas_langchain-0.9.8/canvas_langchain/__init__.py
--rw-r--r--   0 jparisea   (501) staff       (20)    25675 2024-01-27 09:39:58.000000 canvas_langchain-0.9.8/canvas_langchain/canvas.py
-drwxr-xr-x   0 jparisea   (501) staff       (20)        0 2024-01-27 13:01:15.387558 canvas_langchain-0.9.8/canvas_langchain.egg-info/
--rw-r--r--   0 jparisea   (501) staff       (20)     2411 2024-01-27 13:01:15.000000 canvas_langchain-0.9.8/canvas_langchain.egg-info/PKG-INFO
--rw-r--r--   0 jparisea   (501) staff       (20)      285 2024-01-27 13:01:15.000000 canvas_langchain-0.9.8/canvas_langchain.egg-info/SOURCES.txt
--rw-r--r--   0 jparisea   (501) staff       (20)        1 2024-01-27 13:01:15.000000 canvas_langchain-0.9.8/canvas_langchain.egg-info/dependency_links.txt
--rw-r--r--   0 jparisea   (501) staff       (20)      161 2024-01-27 13:01:15.000000 canvas_langchain-0.9.8/canvas_langchain.egg-info/requires.txt
--rw-r--r--   0 jparisea   (501) staff       (20)       17 2024-01-27 13:01:15.000000 canvas_langchain-0.9.8/canvas_langchain.egg-info/top_level.txt
--rw-r--r--   0 jparisea   (501) staff       (20)       38 2024-01-27 13:01:15.388026 canvas_langchain-0.9.8/setup.cfg
--rw-r--r--   0 jparisea   (501) staff       (20)      945 2024-01-27 05:08:46.000000 canvas_langchain-0.9.8/setup.py
+drwxr-xr-x   0 jparisea   (501) staff       (20)        0 2024-01-31 18:02:07.818277 canvas_langchain-0.9.9/
+-rw-r--r--   0 jparisea   (501) staff       (20)    35148 2023-07-31 20:28:17.000000 canvas_langchain-0.9.9/LICENSE.txt
+-rw-r--r--   0 jparisea   (501) staff       (20)     2411 2024-01-31 18:02:07.818044 canvas_langchain-0.9.9/PKG-INFO
+-rw-r--r--   0 jparisea   (501) staff       (20)     1590 2024-01-27 12:17:35.000000 canvas_langchain-0.9.9/README.md
+drwxr-xr-x   0 jparisea   (501) staff       (20)        0 2024-01-31 18:02:07.816826 canvas_langchain-0.9.9/canvas_langchain/
+-rw-r--r--   0 jparisea   (501) staff       (20)        0 2023-07-31 15:52:56.000000 canvas_langchain-0.9.9/canvas_langchain/__init__.py
+-rw-r--r--   0 jparisea   (501) staff       (20)    26055 2024-01-31 15:25:29.000000 canvas_langchain-0.9.9/canvas_langchain/canvas.py
+drwxr-xr-x   0 jparisea   (501) staff       (20)        0 2024-01-31 18:02:07.817813 canvas_langchain-0.9.9/canvas_langchain.egg-info/
+-rw-r--r--   0 jparisea   (501) staff       (20)     2411 2024-01-31 18:02:07.000000 canvas_langchain-0.9.9/canvas_langchain.egg-info/PKG-INFO
+-rw-r--r--   0 jparisea   (501) staff       (20)      285 2024-01-31 18:02:07.000000 canvas_langchain-0.9.9/canvas_langchain.egg-info/SOURCES.txt
+-rw-r--r--   0 jparisea   (501) staff       (20)        1 2024-01-31 18:02:07.000000 canvas_langchain-0.9.9/canvas_langchain.egg-info/dependency_links.txt
+-rw-r--r--   0 jparisea   (501) staff       (20)      161 2024-01-31 18:02:07.000000 canvas_langchain-0.9.9/canvas_langchain.egg-info/requires.txt
+-rw-r--r--   0 jparisea   (501) staff       (20)       17 2024-01-31 18:02:07.000000 canvas_langchain-0.9.9/canvas_langchain.egg-info/top_level.txt
+-rw-r--r--   0 jparisea   (501) staff       (20)       38 2024-01-31 18:02:07.818326 canvas_langchain-0.9.9/setup.cfg
+-rw-r--r--   0 jparisea   (501) staff       (20)      945 2024-01-31 18:01:20.000000 canvas_langchain-0.9.9/setup.py
```

### Comparing `canvas_langchain-0.9.8/LICENSE.txt` & `canvas_langchain-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `canvas_langchain-0.9.8/PKG-INFO` & `canvas_langchain-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvas_langchain
-Version: 0.9.8
+Version: 0.9.9
 Summary: A canvas langchain integration
 Home-page: https://github.com/umich-its-ai/langchain-doc-canvas
 Author: University of Michigan
 Author-email: noreply@umich.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.8.1
```

### Comparing `canvas_langchain-0.9.8/README.md` & `canvas_langchain-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `canvas_langchain-0.9.8/canvas_langchain/canvas.py` & `canvas_langchain-0.9.9/canvas_langchain/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,34 +39,14 @@
             'message': self.message,
             'level': self.level,
         }
 
 class CanvasLoader(BaseLoader):
     """Loading logic for Canvas Pages, Announcements, Assignments and Files."""
 
-    def logMessage(self, message, level):
-        print(message)
-
-        if level == 'INFO':
-            logger.info(message)
-        if level == 'DEBUG':
-            logger.debug(message)
-        if level == 'WARNING':
-            logger.warning(message)
-
-            self.errors.append(LogStatement(
-                message = message,
-                level = level
-            ))
-
-        self.progress.append(LogStatement(
-            message = message,
-            level = level
-        ))
-
     def __init__(self, api_url: str, api_key: str = "", course_id: int = 0, index_external_urls: bool = False):
         """Initialize with API URL and api_key.
 
         Args:
             api_url: The canvas API URL endpoint.
             api_key: API Key or token.
             course_id: Course ID we want to return documents from
@@ -110,14 +90,32 @@
                     page_documents = page_documents + self.load_page(page)
                     self.indexed_items.append(f"Page:{page.page_id}")
         except CanvasException as error:
             self._error_logger(error=error, action="get_pages", entity_type="page", entity_id=page.page_id)
 
         return page_documents
 
+    def logMessage(self, message, level):
+        if level == 'INFO':
+            logger.info(message)
+        if level == 'DEBUG':
+            logger.debug(message)
+        if level == 'WARNING':
+            logger.warning(message)
+
+            self.errors.append(LogStatement(
+                message = message,
+                level = level
+            ))
+
+        self.progress.append(LogStatement(
+            message = message,
+            level = level
+        ))
+
     def load_page(self, page) -> List[Document]:
         """Load a specific page."""
         try:
             page_body_text = self._get_html_as_string(page.body)
 
             return [Document(
                 page_content=page_body_text.strip(),
@@ -245,18 +243,21 @@
             for i, page in enumerate(pdf_reader.pages):
                 docs.append(Document(
                     page_content=page.extract_text(),
                     metadata={ "filename": file.filename, "source": self._get_file_url(file.id), "kind": "file", "file_id": file.id, "page": i+1 }
                 ))
         except errors.FileNotDecryptedError:
             self._error_logger(error=f"PyPDF2.errors.FileNotDecryptedError: File has not been decrypted ({file.filename})", action="read_pdf", entity_type="file", entity_id=file.id)
+            self.logMessage(message = { "message": { 'filename': f"{file.filename}", 'reason': 'not_indexed' } }, level = 'INFO')
         except binasciiError as err:
             self._error_logger(error=f"{str(err)} ({file.filename})", action="read_pdf", entity_type="file", entity_id=file.id)
+            self.logMessage(message = { "message": { 'filename': f"{file.filename}", 'reason': 'not_indexed' } }, level = 'INFO')
         except Exception as err:
             self._error_logger(error=f"{str(err)} ({file.filename})", action="read_pdf", entity_type="file", entity_id=file.id)
+            self.logMessage(message = { "message": { 'filename': f"{file.filename}", 'reason': 'not_indexed' } }, level = 'INFO')
 
         return docs
 
     def _load_docx_file(self, file) -> List[Document]:
         file_contents = file.get_contents(binary=True)
 
         with tempfile.TemporaryDirectory() as temp_dir:
@@ -541,15 +542,15 @@
         try:
             # Initialize a new Canvas object
             canvas = Canvas(self.api_url, self.api_key)
 
             course = canvas.get_course(self.course_id, include=[ "syllabus_body" ])
 
             # Access the course's name
-            self.logMessage(message=f"Indexing: {course.name}", level="INFO")
+            self.logMessage(message=f"Indexing: {course.name} ({course.id})", level="INFO")
 
             self.returned_course_id = course.id
 
             # add syllabus
             self.logMessage(message="Load syllabus", level="DEBUG")
             docs = docs + self.load_syllabus(course=course)
```

### Comparing `canvas_langchain-0.9.8/canvas_langchain.egg-info/PKG-INFO` & `canvas_langchain-0.9.9/canvas_langchain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvas_langchain
-Version: 0.9.8
+Version: 0.9.9
 Summary: A canvas langchain integration
 Home-page: https://github.com/umich-its-ai/langchain-doc-canvas
 Author: University of Michigan
 Author-email: noreply@umich.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.8.1
```

### Comparing `canvas_langchain-0.9.8/setup.py` & `canvas_langchain-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='canvas_langchain',
-    version='0.9.8',
+    version='0.9.9',
     description='A canvas langchain integration',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='University of Michigan',
     author_email='noreply@umich.edu',
     url='https://github.com/umich-its-ai/langchain-doc-canvas',
     packages=find_packages(),
```

