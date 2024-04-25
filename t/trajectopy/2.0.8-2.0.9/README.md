# Comparing `tmp/trajectopy-2.0.8.tar.gz` & `tmp/trajectopy-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trajectopy-2.0.8.tar", max compression
+gzip compressed data, was "trajectopy-2.0.9.tar", max compression
```

## Comparing `trajectopy-2.0.8.tar` & `trajectopy-2.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    35790 2023-10-09 11:38:18.419402 trajectopy-2.0.8/LICENSE
--rw-r--r--   0        0        0     1000 2024-01-23 13:16:06.993704 trajectopy-2.0.8/pyproject.toml
--rw-r--r--   0        0        0    21089 2023-12-19 11:56:26.980793 trajectopy-2.0.8/README.md
--rw-r--r--   0        0        0        0 2023-10-09 11:38:18.431402 trajectopy-2.0.8/trajectopy/__init__.py
--rw-r--r--   0        0        0     2258 2023-12-06 12:09:13.292875 trajectopy-2.0.8/trajectopy/__main__.py
--rw-r--r--   0        0        0    35790 2023-10-09 11:38:18.431402 trajectopy-2.0.8/trajectopy/LICENSE
--rw-r--r--   0        0        0        0 2023-10-23 12:38:48.374045 trajectopy-2.0.8/trajectopy/managers/__init__.py
--rw-r--r--   0        0        0     5957 2023-12-04 13:35:31.207708 trajectopy-2.0.8/trajectopy/managers/file_manager.py
--rw-r--r--   0        0        0     5323 2023-12-06 10:01:05.756084 trajectopy-2.0.8/trajectopy/managers/plot_manager.py
--rw-r--r--   0        0        0     6632 2023-12-04 13:35:31.207708 trajectopy-2.0.8/trajectopy/managers/requests.py
--rw-r--r--   0        0        0     3625 2023-12-04 13:35:31.208709 trajectopy-2.0.8/trajectopy/managers/session_manager.py
--rw-r--r--   0        0        0    37958 2024-01-22 14:20:19.708191 trajectopy-2.0.8/trajectopy/managers/trajectory_manager.py
--rw-r--r--   0        0        0     9634 2023-12-04 13:35:31.209708 trajectopy-2.0.8/trajectopy/managers/ui_manager.py
--rw-r--r--   0        0        0        0 2023-10-23 12:38:48.377045 trajectopy-2.0.8/trajectopy/models/__init__.py
--rw-r--r--   0        0        0    14876 2023-12-04 13:35:31.209708 trajectopy-2.0.8/trajectopy/models/entries.py
--rw-r--r--   0        0        0     1494 2023-10-23 12:38:48.377045 trajectopy-2.0.8/trajectopy/models/property_model.py
--rw-r--r--   0        0        0     3924 2023-10-23 12:38:48.378045 trajectopy-2.0.8/trajectopy/models/result_model.py
--rw-r--r--   0        0        0      998 2023-10-23 12:38:48.378045 trajectopy-2.0.8/trajectopy/models/selection.py
--rw-r--r--   0        0        0     4215 2023-10-23 12:38:48.379044 trajectopy-2.0.8/trajectopy/models/table_model.py
--rw-r--r--   0        0        0     5314 2023-12-04 13:35:31.209708 trajectopy-2.0.8/trajectopy/models/trajectory_model.py
--rw-r--r--   0        0        0      723 2023-12-07 07:39:25.425501 trajectopy-2.0.8/trajectopy/path.py
--rw-r--r--   0        0        0   120742 2023-10-23 12:38:48.380044 trajectopy-2.0.8/trajectopy/resources/full-icon-poppins.png
--rw-r--r--   0        0        0    39912 2023-10-23 12:38:48.381190 trajectopy-2.0.8/trajectopy/resources/icon-bg.png
--rw-r--r--   0        0        0    24491 2023-10-23 12:38:48.381190 trajectopy-2.0.8/trajectopy/resources/icon.png
--rw-r--r--   0        0        0     1758 2023-10-23 12:38:48.381190 trajectopy-2.0.8/trajectopy/util.py
--rw-r--r--   0        0        0        5 2024-01-23 13:16:10.656487 trajectopy-2.0.8/trajectopy/version
--rw-r--r--   0        0        0        0 2023-10-23 12:38:48.381190 trajectopy-2.0.8/trajectopy/views/__init__.py
--rw-r--r--   0        0        0     3998 2024-01-22 14:19:05.957114 trajectopy-2.0.8/trajectopy/views/about_window.py
--rw-r--r--   0        0        0    10701 2024-01-22 14:19:05.957709 trajectopy-2.0.8/trajectopy/views/alignment_edit_window.py
--rw-r--r--   0        0        0    10398 2024-01-22 14:19:05.958244 trajectopy-2.0.8/trajectopy/views/json_settings_view.py
--rw-r--r--   0        0        0    18517 2024-01-22 14:19:05.958779 trajectopy-2.0.8/trajectopy/views/main_window.py
--rw-r--r--   0        0        0     2765 2024-01-22 14:19:05.959303 trajectopy-2.0.8/trajectopy/views/progress_window.py
--rw-r--r--   0        0        0     4133 2023-10-23 12:38:48.384195 trajectopy-2.0.8/trajectopy/views/properties_window.py
--rw-r--r--   0        0        0     6724 2023-12-04 13:35:31.211709 trajectopy-2.0.8/trajectopy/views/result_context_menu.py
--rw-r--r--   0        0        0     4798 2023-10-23 12:38:48.385195 trajectopy-2.0.8/trajectopy/views/result_selection_window.py
--rw-r--r--   0        0        0     5687 2023-10-23 12:38:48.386088 trajectopy-2.0.8/trajectopy/views/result_table_view.py
--rw-r--r--   0        0        0    24472 2023-12-04 13:35:31.211709 trajectopy-2.0.8/trajectopy/views/trajectory_context_menu.py
--rw-r--r--   0        0        0     7782 2023-10-23 12:38:48.387438 trajectopy-2.0.8/trajectopy/views/trajectory_table_view.py
--rw-r--r--   0        0        0    21651 1970-01-01 00:00:00.000000 trajectopy-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35790 2023-10-09 11:38:18.419402 trajectopy-2.0.9/LICENSE
+-rw-r--r--   0        0        0     1000 2024-01-25 13:59:39.733578 trajectopy-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0    21089 2024-01-23 13:35:40.313090 trajectopy-2.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-10-09 11:38:18.431402 trajectopy-2.0.9/trajectopy/__init__.py
+-rw-r--r--   0        0        0     2258 2023-12-06 12:09:13.292875 trajectopy-2.0.9/trajectopy/__main__.py
+-rw-r--r--   0        0        0    35790 2023-10-09 11:38:18.431402 trajectopy-2.0.9/trajectopy/LICENSE
+-rw-r--r--   0        0        0        0 2023-10-23 12:38:48.374045 trajectopy-2.0.9/trajectopy/managers/__init__.py
+-rw-r--r--   0        0        0     5957 2023-12-04 13:35:31.207708 trajectopy-2.0.9/trajectopy/managers/file_manager.py
+-rw-r--r--   0        0        0     5323 2023-12-06 10:01:05.756084 trajectopy-2.0.9/trajectopy/managers/plot_manager.py
+-rw-r--r--   0        0        0     6632 2023-12-04 13:35:31.207708 trajectopy-2.0.9/trajectopy/managers/requests.py
+-rw-r--r--   0        0        0     3625 2023-12-04 13:35:31.208709 trajectopy-2.0.9/trajectopy/managers/session_manager.py
+-rw-r--r--   0        0        0    37958 2024-01-23 13:35:40.315094 trajectopy-2.0.9/trajectopy/managers/trajectory_manager.py
+-rw-r--r--   0        0        0     9634 2023-12-04 13:35:31.209708 trajectopy-2.0.9/trajectopy/managers/ui_manager.py
+-rw-r--r--   0        0        0        0 2023-10-23 12:38:48.377045 trajectopy-2.0.9/trajectopy/models/__init__.py
+-rw-r--r--   0        0        0    14876 2023-12-04 13:35:31.209708 trajectopy-2.0.9/trajectopy/models/entries.py
+-rw-r--r--   0        0        0     1494 2023-10-23 12:38:48.377045 trajectopy-2.0.9/trajectopy/models/property_model.py
+-rw-r--r--   0        0        0     3924 2023-10-23 12:38:48.378045 trajectopy-2.0.9/trajectopy/models/result_model.py
+-rw-r--r--   0        0        0      998 2023-10-23 12:38:48.378045 trajectopy-2.0.9/trajectopy/models/selection.py
+-rw-r--r--   0        0        0     4215 2023-10-23 12:38:48.379044 trajectopy-2.0.9/trajectopy/models/table_model.py
+-rw-r--r--   0        0        0     5314 2023-12-04 13:35:31.209708 trajectopy-2.0.9/trajectopy/models/trajectory_model.py
+-rw-r--r--   0        0        0      723 2023-12-07 07:39:25.425501 trajectopy-2.0.9/trajectopy/path.py
+-rw-r--r--   0        0        0   120742 2023-10-23 12:38:48.380044 trajectopy-2.0.9/trajectopy/resources/full-icon-poppins.png
+-rw-r--r--   0        0        0    39912 2023-10-23 12:38:48.381190 trajectopy-2.0.9/trajectopy/resources/icon-bg.png
+-rw-r--r--   0        0        0    24491 2023-10-23 12:38:48.381190 trajectopy-2.0.9/trajectopy/resources/icon.png
+-rw-r--r--   0        0        0     1758 2023-10-23 12:38:48.381190 trajectopy-2.0.9/trajectopy/util.py
+-rw-r--r--   0        0        0        5 2024-01-25 14:04:56.546411 trajectopy-2.0.9/trajectopy/version
+-rw-r--r--   0        0        0        0 2023-10-23 12:38:48.381190 trajectopy-2.0.9/trajectopy/views/__init__.py
+-rw-r--r--   0        0        0     4050 2024-01-23 13:36:36.648847 trajectopy-2.0.9/trajectopy/views/about_window.py
+-rw-r--r--   0        0        0    10701 2024-01-23 13:35:40.317093 trajectopy-2.0.9/trajectopy/views/alignment_edit_window.py
+-rw-r--r--   0        0        0    10398 2024-01-23 13:35:40.317093 trajectopy-2.0.9/trajectopy/views/json_settings_view.py
+-rw-r--r--   0        0        0    18517 2024-01-23 13:35:40.318093 trajectopy-2.0.9/trajectopy/views/main_window.py
+-rw-r--r--   0        0        0     2765 2024-01-23 13:35:40.318093 trajectopy-2.0.9/trajectopy/views/progress_window.py
+-rw-r--r--   0        0        0     4133 2023-10-23 12:38:48.384195 trajectopy-2.0.9/trajectopy/views/properties_window.py
+-rw-r--r--   0        0        0     6724 2023-12-04 13:35:31.211709 trajectopy-2.0.9/trajectopy/views/result_context_menu.py
+-rw-r--r--   0        0        0     4798 2023-10-23 12:38:48.385195 trajectopy-2.0.9/trajectopy/views/result_selection_window.py
+-rw-r--r--   0        0        0     5687 2023-10-23 12:38:48.386088 trajectopy-2.0.9/trajectopy/views/result_table_view.py
+-rw-r--r--   0        0        0    24472 2023-12-04 13:35:31.211709 trajectopy-2.0.9/trajectopy/views/trajectory_context_menu.py
+-rw-r--r--   0        0        0     7782 2023-10-23 12:38:48.387438 trajectopy-2.0.9/trajectopy/views/trajectory_table_view.py
+-rw-r--r--   0        0        0    21651 1970-01-01 00:00:00.000000 trajectopy-2.0.9/PKG-INFO
```

### Comparing `trajectopy-2.0.8/LICENSE` & `trajectopy-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/pyproject.toml` & `trajectopy-2.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trajectopy"
-version = "2.0.8"
+version = "2.0.9"
 description = "Trajectory Evaluation in Python"
 authors = ["Gereon Tombrink <tombrink@igg.uni-bonn.de>"]
 maintainers = ["Gereon Tombrink <tombrink@igg.uni-bonn.de>"]
 license = "GPLv3"
 keywords = ["trajectory", "evaluation", "alignment", "similarity", "leverarm", "epsg", "robotics"]
 readme = "README.md"
 homepage = "https://github.com/gereon-t/trajectopy"
@@ -13,15 +13,15 @@
     { include = "trajectopy" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 pyqt6 = "^6.6.1"
 rich = "^13.7.0"
-trajectopy-core = "^2.5.1,<2.6.0"
+trajectopy-core = "^2.6.0,<2.7.0"
 
 [tool.poetry.scripts]
 trajectopy = "trajectopy.__main__:main"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.5.1"
 black = "^23.9.1"
```

### Comparing `trajectopy-2.0.8/README.md` & `trajectopy-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/__main__.py` & `trajectopy-2.0.9/trajectopy/__main__.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/LICENSE` & `trajectopy-2.0.9/trajectopy/LICENSE`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/managers/file_manager.py` & `trajectopy-2.0.9/trajectopy/managers/file_manager.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/managers/plot_manager.py` & `trajectopy-2.0.9/trajectopy/managers/plot_manager.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/managers/requests.py` & `trajectopy-2.0.9/trajectopy/managers/requests.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/managers/session_manager.py` & `trajectopy-2.0.9/trajectopy/managers/session_manager.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/managers/trajectory_manager.py` & `trajectopy-2.0.9/trajectopy/managers/trajectory_manager.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/managers/ui_manager.py` & `trajectopy-2.0.9/trajectopy/managers/ui_manager.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/models/entries.py` & `trajectopy-2.0.9/trajectopy/models/entries.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/models/property_model.py` & `trajectopy-2.0.9/trajectopy/models/property_model.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/models/result_model.py` & `trajectopy-2.0.9/trajectopy/models/result_model.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/models/selection.py` & `trajectopy-2.0.9/trajectopy/models/selection.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/models/table_model.py` & `trajectopy-2.0.9/trajectopy/models/table_model.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/models/trajectory_model.py` & `trajectopy-2.0.9/trajectopy/models/trajectory_model.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/path.py` & `trajectopy-2.0.9/trajectopy/path.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/resources/full-icon-poppins.png` & `trajectopy-2.0.9/trajectopy/resources/full-icon-poppins.png`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/resources/icon-bg.png` & `trajectopy-2.0.9/trajectopy/resources/icon-bg.png`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/resources/icon.png` & `trajectopy-2.0.9/trajectopy/resources/icon.png`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/util.py` & `trajectopy-2.0.9/trajectopy/util.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/views/about_window.py` & `trajectopy-2.0.9/trajectopy/views/about_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,27 @@
         super().__init__(parent=parent)
         self.setupUi()
         self.version: QtWidgets.QLabel
         self.version.setText(version_str)
 
         self.year: QtWidgets.QLabel
         self.year.setText(year_str)
-    
+
     def center(self):
         qr = self.frameGeometry()
         cp = self.screen().availableGeometry().center()
 
         qr.moveCenter(cp)
         self.move(qr.topLeft())
 
     def setupUi(self):
         self.setObjectName("MainWindow")
         self.resize(320, 270)
         self.center()
+        self.setStyleSheet("background-color: white;")
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.sizePolicy().hasHeightForWidth())
         self.setSizePolicy(sizePolicy)
         self.setMinimumSize(QtCore.QSize(320, 270))
         self.setMaximumSize(QtCore.QSize(320, 270))
@@ -82,8 +83,8 @@
     def retranslateUi(self):
         _translate = QtCore.QCoreApplication.translate
         self.setWindowTitle(_translate("MainWindow", "About Trajectopy"))
         # self.name.setText(_translate("MainWindow", "Trajectopy"))
         self.version.setText(_translate("MainWindow", "Version Number"))
         self.author.setText(_translate("MainWindow", "Gereon Tombrink"))
         self.uni.setText(_translate("MainWindow", "University of Bonn"))
-        self.year.setText(_translate("MainWindow", "2023"))
+        self.year.setText(_translate("MainWindow", "2024"))
```

### Comparing `trajectopy-2.0.8/trajectopy/views/alignment_edit_window.py` & `trajectopy-2.0.9/trajectopy/views/alignment_edit_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/views/json_settings_view.py` & `trajectopy-2.0.9/trajectopy/views/json_settings_view.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/views/main_window.py` & `trajectopy-2.0.9/trajectopy/views/main_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from trajectopy.views.about_window import AboutGUI
 from trajectopy.views.json_settings_view import JSONViewer
 from trajectopy.views.progress_window import ProgressWindow
 from trajectopy.views.result_table_view import ResultTableView
 from trajectopy.views.trajectory_table_view import TrajectoryTableView
 
 VERSION = open(VERSION_FILE_PATH, "r", encoding="utf-8").read()
-YEAR = "2023"
+YEAR = "2024"
 
 
 logger = logging.getLogger("root")
 
 
 class TrajectopyGUI(QtWidgets.QMainWindow):
     """
```

### Comparing `trajectopy-2.0.8/trajectopy/views/progress_window.py` & `trajectopy-2.0.9/trajectopy/views/progress_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/views/properties_window.py` & `trajectopy-2.0.9/trajectopy/views/properties_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/views/result_context_menu.py` & `trajectopy-2.0.9/trajectopy/views/result_context_menu.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/views/result_selection_window.py` & `trajectopy-2.0.9/trajectopy/views/result_selection_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/views/result_table_view.py` & `trajectopy-2.0.9/trajectopy/views/result_table_view.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/views/trajectory_context_menu.py` & `trajectopy-2.0.9/trajectopy/views/trajectory_context_menu.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/trajectopy/views/trajectory_table_view.py` & `trajectopy-2.0.9/trajectopy/views/trajectory_table_view.py`

 * *Files identical despite different names*

### Comparing `trajectopy-2.0.8/PKG-INFO` & `trajectopy-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trajectopy
-Version: 2.0.8
+Version: 2.0.9
 Summary: Trajectory Evaluation in Python
 Home-page: https://github.com/gereon-t/trajectopy
 License: GPLv3
 Keywords: trajectory,evaluation,alignment,similarity,leverarm,epsg,robotics
 Author: Gereon Tombrink
 Author-email: tombrink@igg.uni-bonn.de
 Maintainer: Gereon Tombrink
@@ -13,15 +13,15 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyqt6 (>=6.6.1,<7.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
-Requires-Dist: trajectopy-core (>=2.5.1,<2.6.0)
+Requires-Dist: trajectopy-core (>=2.6.0,<2.7.0)
 Project-URL: Repository, https://github.com/gereon-t/trajectopy.git
 Description-Content-Type: text/markdown
 
 <div align="center">
     <h1>Trajectopy - Trajectory Evaluation in Python</h1>
     <a href="https://github.com/gereon-t/trajectopy/releases"><img src="https://img.shields.io/github/v/release/gereon-t/trajectopy?label=version" /></a>
     <a href="https://www.python.org/downloads/"><img src="https://img.shields.io/badge/python-3.8.2+-blue.svg" /></a>
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: trajectopy Version: 2.0.8 Summary: Trajectory
+Metadata-Version: 2.1 Name: trajectopy Version: 2.0.9 Summary: Trajectory
 Evaluation in Python Home-page: https://github.com/gereon-t/trajectopy License:
 GPLv3 Keywords:
 trajectory,evaluation,alignment,similarity,leverarm,epsg,robotics Author:
 Gereon Tombrink Author-email: tombrink@igg.uni-bonn.de Maintainer: Gereon
 Tombrink Maintainer-email: tombrink@igg.uni-bonn.de Requires-Python:
 >=3.9,<3.13 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: pyqt6 (>=6.6.1,<7.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0) Requires-Dist: trajectopy-core
-(>=2.5.1,<2.6.0) Project-URL: Repository, https://github.com/gereon-t/
+(>=2.6.0,<2.7.0) Project-URL: Repository, https://github.com/gereon-t/
 trajectopy.git Description-Content-Type: text/markdown
           ************ TTrraajjeeccttooppyy -- TTrraajjeeccttoorryy EEvvaalluuaattiioonn iinn PPyytthhoonn ************
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_g_e_r_e_o_n_-_t_/_t_r_a_j_e_c_t_o_p_y_?_l_a_b_e_l_=_v_e_r_s_i_o_n_]
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._8_._2_+_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
             _g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_g_e_r_e_o_n_-_t_/_t_r_a_j_e_c_t_o_p_y_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_W_i_n_d_o_w_s_-_0_0_7_8_D_6_?_s_t_&_l_o_g_o_=_w_i_n_d_o_w_s_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_n_u_x_-_F_C_C_6_2_4_?_l_o_g_o_=_l_i_n_u_x_&_l_o_g_o_C_o_l_o_r_=_b_l_a_c_k_]_[_h_t_t_p_s_:_/_/
```

