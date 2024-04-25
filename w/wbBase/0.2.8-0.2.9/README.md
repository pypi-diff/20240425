# Comparing `tmp/wbBase-0.2.8.tar.gz` & `tmp/wbbase-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbBase-0.2.8.tar", last modified: Wed Feb 14 15:16:20 2024, max compression
+gzip compressed data, was "wbbase-0.2.9.tar", last modified: Thu Apr 25 15:45:28 2024, max compression
```

## Comparing `wbBase-0.2.8.tar` & `wbbase-0.2.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 15:16:20.454690 wbBase-0.2.8/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2024-02-14 15:16:19.000000 wbBase-0.2.8/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 15:16:20.444690 wbBase-0.2.8/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 15:16:20.449690 wbBase-0.2.8/Lib/wbBase/
--rw-rw-rw-   0 root         (0) root         (0)      152 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26135 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/application.py
--rw-rw-rw-   0 root         (0) root         (0)     2377 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/applicationInfo.py
--rw-rw-rw-   0 root         (0) root         (0)    20860 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/applicationWindow.py
--rw-rw-rw-   0 root         (0) root         (0)   312891 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/artprovider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 15:16:20.451690 wbBase-0.2.8/Lib/wbBase/control/
--rw-rw-rw-   0 root         (0) root         (0)     1118 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/control/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4414 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/control/externalToolConfig.py
--rw-rw-rw-   0 root         (0) root         (0)     5891 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/control/externalToolConfigUI.py
--rw-rw-rw-   0 root         (0) root         (0)     2666 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/control/filling.py
--rw-rw-rw-   0 root         (0) root         (0)     1670 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/control/iePanel.py
--rw-rw-rw-   0 root         (0) root         (0)     8569 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/control/propgrid.py
--rw-rw-rw-   0 root         (0) root         (0)    47198 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/control/textEditControl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 15:16:20.452690 wbBase-0.2.8/Lib/wbBase/dialog/
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/dialog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2342 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/dialog/multiSaveModifiedDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     3293 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)    20923 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/dialog/preferences.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 15:16:20.453690 wbBase-0.2.8/Lib/wbBase/document/
--rw-rw-rw-   0 root         (0) root         (0)    23535 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/document/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    36849 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/document/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4743 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/document/notebook.py
--rw-rw-rw-   0 root         (0) root         (0)     8099 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/document/template.py
--rw-rw-rw-   0 root         (0) root         (0)     8265 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/document/view.py
--rw-rw-rw-   0 root         (0) root         (0)    22086 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/panelManager.py
--rw-rw-rw-   0 root         (0) root         (0)     3362 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/pluginManager.py
--rw-rw-rw-   0 root         (0) root         (0)     2942 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/pluginManager_old.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     8940 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/scripting.py
--rw-rw-rw-   0 root         (0) root         (0)     9858 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/shortcut.py
--rw-rw-rw-   0 root         (0) root         (0)      929 2024-02-14 15:16:19.000000 wbBase-0.2.8/Lib/wbBase/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 15:16:20.454690 wbBase-0.2.8/Lib/wbBase.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3046 2024-02-14 15:16:20.000000 wbBase-0.2.8/Lib/wbBase.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1088 2024-02-14 15:16:20.000000 wbBase-0.2.8/Lib/wbBase.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 15:16:20.000000 wbBase-0.2.8/Lib/wbBase.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2024-02-14 15:16:20.000000 wbBase-0.2.8/Lib/wbBase.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-02-14 15:16:20.000000 wbBase-0.2.8/Lib/wbBase.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3046 2024-02-14 15:16:20.454690 wbBase-0.2.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1444 2024-02-14 15:16:19.000000 wbBase-0.2.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2080 2024-02-14 15:16:20.455690 wbBase-0.2.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-02-14 15:16:19.000000 wbBase-0.2.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 15:16:20.454690 wbBase-0.2.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)      515 2024-02-14 15:16:19.000000 wbBase-0.2.8/tests/test_app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 15:45:28.872872 wbbase-0.2.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-04-25 15:45:27.000000 wbbase-0.2.9/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 15:45:28.861872 wbbase-0.2.9/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 15:45:28.866872 wbbase-0.2.9/Lib/wbBase/
+-rw-rw-rw-   0 root         (0) root         (0)      152 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26135 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/application.py
+-rw-rw-rw-   0 root         (0) root         (0)     2377 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/applicationInfo.py
+-rw-rw-rw-   0 root         (0) root         (0)    20860 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/applicationWindow.py
+-rw-rw-rw-   0 root         (0) root         (0)   312891 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/artprovider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 15:45:28.869872 wbbase-0.2.9/Lib/wbBase/control/
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/control/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4414 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/control/externalToolConfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     5891 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/control/externalToolConfigUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/control/filling.py
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/control/iePanel.py
+-rw-rw-rw-   0 root         (0) root         (0)     8569 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/control/propgrid.py
+-rw-rw-rw-   0 root         (0) root         (0)    47198 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/control/textEditControl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 15:45:28.870872 wbbase-0.2.9/Lib/wbBase/dialog/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/dialog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2342 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/dialog/multiSaveModifiedDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     3293 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)    20923 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/dialog/preferences.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 15:45:28.871872 wbbase-0.2.9/Lib/wbBase/document/
+-rw-rw-rw-   0 root         (0) root         (0)    23535 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/document/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    38237 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/document/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4743 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/document/notebook.py
+-rw-rw-rw-   0 root         (0) root         (0)     8099 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/document/template.py
+-rw-rw-rw-   0 root         (0) root         (0)     8265 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/document/view.py
+-rw-rw-rw-   0 root         (0) root         (0)    22086 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/panelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3362 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/pluginManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2942 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/pluginManager_old.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     8940 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/scripting.py
+-rw-rw-rw-   0 root         (0) root         (0)     9858 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/shortcut.py
+-rw-rw-rw-   0 root         (0) root         (0)      929 2024-04-25 15:45:27.000000 wbbase-0.2.9/Lib/wbBase/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 15:45:28.871872 wbbase-0.2.9/Lib/wbBase.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3046 2024-04-25 15:45:28.000000 wbbase-0.2.9/Lib/wbBase.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1088 2024-04-25 15:45:28.000000 wbbase-0.2.9/Lib/wbBase.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 15:45:28.000000 wbbase-0.2.9/Lib/wbBase.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2024-04-25 15:45:28.000000 wbbase-0.2.9/Lib/wbBase.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-25 15:45:28.000000 wbbase-0.2.9/Lib/wbBase.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3046 2024-04-25 15:45:28.872872 wbbase-0.2.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1444 2024-04-25 15:45:27.000000 wbbase-0.2.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2024-04-25 15:45:28.873872 wbbase-0.2.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-25 15:45:27.000000 wbbase-0.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 15:45:28.871872 wbbase-0.2.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      515 2024-04-25 15:45:27.000000 wbbase-0.2.9/tests/test_app.py
```

### Comparing `wbBase-0.2.8/LICENSE` & `wbbase-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/application.py` & `wbbase-0.2.9/Lib/wbBase/application.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/applicationInfo.py` & `wbbase-0.2.9/Lib/wbBase/applicationInfo.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/applicationWindow.py` & `wbbase-0.2.9/Lib/wbBase/applicationWindow.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/artprovider.py` & `wbbase-0.2.9/Lib/wbBase/artprovider.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/control/__init__.py` & `wbbase-0.2.9/Lib/wbBase/control/__init__.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/control/externalToolConfig.py` & `wbbase-0.2.9/Lib/wbBase/control/externalToolConfig.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/control/externalToolConfigUI.py` & `wbbase-0.2.9/Lib/wbBase/control/externalToolConfigUI.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/control/filling.py` & `wbbase-0.2.9/Lib/wbBase/control/filling.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/control/iePanel.py` & `wbbase-0.2.9/Lib/wbBase/control/iePanel.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/control/propgrid.py` & `wbbase-0.2.9/Lib/wbBase/control/propgrid.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/control/textEditControl.py` & `wbbase-0.2.9/Lib/wbBase/control/textEditControl.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/dialog/multiSaveModifiedDialog.py` & `wbbase-0.2.9/Lib/wbBase/dialog/multiSaveModifiedDialog.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py` & `wbbase-0.2.9/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/dialog/preferences.py` & `wbbase-0.2.9/Lib/wbBase/dialog/preferences.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/document/__init__.py` & `wbbase-0.2.9/Lib/wbBase/document/__init__.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/document/manager.py` & `wbbase-0.2.9/Lib/wbBase/document/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -465,15 +465,15 @@
         """
         dbg("DocumentManager.RemoveDocument()")
         if document in self._docs:
             docPath = document.path
             self._docs.remove(document)
             self.log.info("document closed: %s", docPath)
 
-    def CreateDocument(self, path: Optional[str], flags: int = 0) -> Optional[Document]:
+    def CreateDocument(self, path: str = "", flags: int = 0) -> Optional[Document]:
         """
         Creates a new document in a manner determined by the flags parameter,
         which can be:
 
         * DOC_NEW Creates a fresh document.
         * DOC_SILENT Silently loads the given document file.
 
@@ -593,17 +593,36 @@
         dbg("DocumentManager.CreateDocument() -> done NO DOC", indent=0)
         return None
 
     def openDocuments(self, filenames: Sequence[str]):
         """
         Opens Documents by calling :meth:`CreateDocument` for every filename.
         """
-        for name in filenames:
-            self.CreateDocument(name, DOC_SILENT)
-            self.app.Yield(True)
+        fileCount = len(filenames)
+        if fileCount == 1:
+            self.CreateDocument(filenames[0], DOC_SILENT)
+            return
+        with wx.ProgressDialog(
+            "Open Documents",
+            f"Opening {fileCount} Documents",
+            fileCount,
+            self.app.TopWindow,
+            wx.PD_APP_MODAL
+            | wx.PD_ESTIMATED_TIME
+            | wx.PD_ELAPSED_TIME
+            | wx.PD_REMAINING_TIME
+            | wx.PD_SMOOTH
+            | wx.PD_AUTO_HIDE,
+        ) as progress:
+            progress: wx.ProgressDialog
+            for name in filenames:
+                progress.Update(progress.Value, os.path.basename(name))
+                self.CreateDocument(name, DOC_SILENT)
+                progress.Update(progress.Value + 1)
+                self.app.Yield(True)
 
     def SelectDocumentPath(
         self, templates: Sequence[DocumentTemplate], flags: int
     ) -> Union[Tuple[DocumentTemplate, str], Tuple[None, None]]:
         """
         Under Windows, pops up a file selector with a list of filters
         corresponding to document templates. The wxDocTemplate corresponding
@@ -921,16 +940,35 @@
         """
         Event handler for menu :menuselection:`File --> Save All`
 
         Saves all documents by calling :meth:`.Document.Save` method
         of every open document.
         """
         dbg("DocumentManager.on_file_saveall()")
-        for document in self.documents:
-            document.Save()
+        if self.documentCount == 1:
+            self.documents[0].Save()
+            return
+        with wx.ProgressDialog(
+            "Save Documents",
+            f"Saving {self.documentCount} Documents",
+            self.documentCount,
+            self.app.TopWindow,
+            wx.PD_APP_MODAL
+            | wx.PD_ESTIMATED_TIME
+            | wx.PD_ELAPSED_TIME
+            | wx.PD_REMAINING_TIME
+            | wx.PD_SMOOTH
+            | wx.PD_AUTO_HIDE,
+        ) as progress:
+            progress: wx.ProgressDialog
+            for document in self.documents:
+                progress.Update(progress.Value, os.path.basename(document.title))
+                document.Save()
+                progress.Update(progress.Value + 1)
+                self.app.Yield(True)
             # event.Skip()
 
     def on_file_saveas(self, event: wx.CommandEvent) -> None:
         doc = self.currentDocument
         if doc:
             doc.SaveAs()
```

### Comparing `wbBase-0.2.8/Lib/wbBase/document/notebook.py` & `wbbase-0.2.9/Lib/wbBase/document/notebook.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/document/template.py` & `wbbase-0.2.9/Lib/wbBase/document/template.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/document/view.py` & `wbbase-0.2.9/Lib/wbBase/document/view.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/panelManager.py` & `wbbase-0.2.9/Lib/wbBase/panelManager.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/pluginManager.py` & `wbbase-0.2.9/Lib/wbBase/pluginManager.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/pluginManager_old.py` & `wbbase-0.2.9/Lib/wbBase/pluginManager_old.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/scripting.py` & `wbbase-0.2.9/Lib/wbBase/scripting.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/shortcut.py` & `wbbase-0.2.9/Lib/wbBase/shortcut.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase/tools.py` & `wbbase-0.2.9/Lib/wbBase/tools.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/Lib/wbBase.egg-info/PKG-INFO` & `wbbase-0.2.9/Lib/wbBase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbBase
-Version: 0.2.8
+Version: 0.2.9
 Summary: Base package for WorkBench applications.
 Home-page: https://gitlab.com/workbench2/wbbase
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/wbbase
 Project-URL: Documentation, https://workbench2.gitlab.io/wbbase
 Project-URL: Tracker, https://gitlab.com/workbench2/wbbase/-/issues
```

### Comparing `wbBase-0.2.8/Lib/wbBase.egg-info/SOURCES.txt` & `wbbase-0.2.9/Lib/wbBase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/PKG-INFO` & `wbbase-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbBase
-Version: 0.2.8
+Version: 0.2.9
 Summary: Base package for WorkBench applications.
 Home-page: https://gitlab.com/workbench2/wbbase
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/wbbase
 Project-URL: Documentation, https://workbench2.gitlab.io/wbbase
 Project-URL: Tracker, https://gitlab.com/workbench2/wbbase/-/issues
```

### Comparing `wbBase-0.2.8/README.md` & `wbbase-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `wbBase-0.2.8/setup.cfg` & `wbbase-0.2.9/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.8
+current_version = 0.2.9
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
```

### Comparing `wbBase-0.2.8/tests/test_app.py` & `wbbase-0.2.9/tests/test_app.py`

 * *Files identical despite different names*

