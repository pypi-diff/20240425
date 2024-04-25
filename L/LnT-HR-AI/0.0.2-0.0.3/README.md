# Comparing `tmp/lnt_hr_ai-0.0.2.tar.gz` & `tmp/lnt_hr_ai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnt_hr_ai-0.0.2.tar", last modified: Wed Apr 24 08:58:06 2024, max compression
+gzip compressed data, was "lnt_hr_ai-0.0.3.tar", last modified: Wed Apr 24 09:09:43 2024, max compression
```

## Comparing `lnt_hr_ai-0.0.2.tar` & `lnt_hr_ai-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 08:58:06.614781 lnt_hr_ai-0.0.2/
-drwxrwxrwx   0        0        0        0 2024-04-24 08:58:06.609743 lnt_hr_ai-0.0.2/DataAnalysis_Package/
--rw-rw-rw-   0        0        0      574 2024-04-23 04:46:31.000000 lnt_hr_ai-0.0.2/DataAnalysis_Package/Address_Finder.py
--rw-rw-rw-   0        0        0     7068 2024-04-23 05:10:11.000000 lnt_hr_ai-0.0.2/DataAnalysis_Package/Data_PreProcessing.py
--rw-rw-rw-   0        0        0    45765 2024-04-24 08:56:59.000000 lnt_hr_ai-0.0.2/DataAnalysis_Package/Data_Visualization.py
--rw-rw-rw-   0        0        0    17815 2024-04-24 08:47:30.000000 lnt_hr_ai-0.0.2/DataAnalysis_Package/ML_MODELS.py
--rw-rw-rw-   0        0        0     4005 2024-04-24 07:46:51.000000 lnt_hr_ai-0.0.2/DataAnalysis_Package/Statistical_Analysis.py
--rw-rw-rw-   0        0        0      182 2024-04-23 08:32:50.000000 lnt_hr_ai-0.0.2/DataAnalysis_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 08:58:06.613779 lnt_hr_ai-0.0.2/LnT_HR_AI.egg-info/
--rw-rw-rw-   0        0        0      737 2024-04-24 08:58:06.000000 lnt_hr_ai-0.0.2/LnT_HR_AI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2024-04-24 08:58:06.000000 lnt_hr_ai-0.0.2/LnT_HR_AI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 08:58:06.000000 lnt_hr_ai-0.0.2/LnT_HR_AI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2024-04-24 08:58:06.000000 lnt_hr_ai-0.0.2/LnT_HR_AI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-04-24 08:58:06.000000 lnt_hr_ai-0.0.2/LnT_HR_AI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      737 2024-04-24 08:58:06.613779 lnt_hr_ai-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-23 09:03:04.000000 lnt_hr_ai-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-24 08:58:06.614781 lnt_hr_ai-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1037 2024-04-24 08:57:19.000000 lnt_hr_ai-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:09:43.189857 lnt_hr_ai-0.0.3/
+drwxrwxrwx   0        0        0        0 2024-04-24 09:09:43.183710 lnt_hr_ai-0.0.3/DataAnalysis_Package/
+-rw-rw-rw-   0        0        0      574 2024-04-23 04:46:31.000000 lnt_hr_ai-0.0.3/DataAnalysis_Package/Address_Finder.py
+-rw-rw-rw-   0        0        0     7047 2024-04-24 09:02:09.000000 lnt_hr_ai-0.0.3/DataAnalysis_Package/Data_PreProcessing.py
+-rw-rw-rw-   0        0        0    45765 2024-04-24 08:56:59.000000 lnt_hr_ai-0.0.3/DataAnalysis_Package/Data_Visualization.py
+-rw-rw-rw-   0        0        0    17801 2024-04-24 09:02:12.000000 lnt_hr_ai-0.0.3/DataAnalysis_Package/ML_MODELS.py
+-rw-rw-rw-   0        0        0     4005 2024-04-24 07:46:51.000000 lnt_hr_ai-0.0.3/DataAnalysis_Package/Statistical_Analysis.py
+-rw-rw-rw-   0        0        0      182 2024-04-23 08:32:50.000000 lnt_hr_ai-0.0.3/DataAnalysis_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:09:43.188853 lnt_hr_ai-0.0.3/LnT_HR_AI.egg-info/
+-rw-rw-rw-   0        0        0      749 2024-04-24 09:09:43.000000 lnt_hr_ai-0.0.3/LnT_HR_AI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2024-04-24 09:09:43.000000 lnt_hr_ai-0.0.3/LnT_HR_AI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 09:09:43.000000 lnt_hr_ai-0.0.3/LnT_HR_AI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2024-04-24 09:09:43.000000 lnt_hr_ai-0.0.3/LnT_HR_AI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-24 09:09:43.000000 lnt_hr_ai-0.0.3/LnT_HR_AI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      749 2024-04-24 09:09:43.188853 lnt_hr_ai-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-23 09:03:04.000000 lnt_hr_ai-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 09:09:43.189857 lnt_hr_ai-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1042 2024-04-24 09:08:43.000000 lnt_hr_ai-0.0.3/setup.py
```

### Comparing `lnt_hr_ai-0.0.2/DataAnalysis_Package/Address_Finder.py` & `lnt_hr_ai-0.0.3/DataAnalysis_Package/Address_Finder.py`

 * *Files identical despite different names*

### Comparing `lnt_hr_ai-0.0.2/DataAnalysis_Package/Data_PreProcessing.py` & `lnt_hr_ai-0.0.3/DataAnalysis_Package/Data_PreProcessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,14 @@
 
     # Get the absolute path of the file
     full_path = os.path.abspath(file_path)
 
     # Print the full path
     print(full_path)
 
-DataPreProcessing()
```

### Comparing `lnt_hr_ai-0.0.2/DataAnalysis_Package/Data_Visualization.py` & `lnt_hr_ai-0.0.3/DataAnalysis_Package/Data_Visualization.py`

 * *Files identical despite different names*

### Comparing `lnt_hr_ai-0.0.2/DataAnalysis_Package/ML_MODELS.py` & `lnt_hr_ai-0.0.3/DataAnalysis_Package/ML_MODELS.py`

 * *Files 0% similar despite different names*

```diff
@@ -1106,9 +1106,8 @@
 00004510: 6379 272c 2027 524f 4327 2c20 2741 5543  cy', 'ROC', 'AUC
 00004520: 275d 0d0a 2020 2020 6466 2e69 6e73 6572  ']..    df.inser
 00004530: 7428 6c6f 633d 302c 2063 6f6c 756d 6e3d  t(loc=0, column=
 00004540: 272f 2f27 2c20 7661 6c75 653d 6e65 775f  '//', value=new_
 00004550: 6461 7461 290d 0a0d 0a20 2020 2064 662e  data)....    df.
 00004560: 746f 5f63 7376 2866 227b 6164 6472 6573  to_csv(f"{addres
 00004570: 737d 2f52 6573 756c 742e 6373 7622 290d  s}/Result.csv").
-00004580: 0a0d 0a0d 0a0d 0a0d 0a52 756e 5f4d 4c4d  .........Run_MLM
-00004590: 6f64 656c 7328 29                        odels()
+00004580: 0a0d 0a0d 0a0d 0a0d 0a                   .........
```

### Comparing `lnt_hr_ai-0.0.2/DataAnalysis_Package/Statistical_Analysis.py` & `lnt_hr_ai-0.0.3/DataAnalysis_Package/Statistical_Analysis.py`

 * *Files identical despite different names*

### Comparing `lnt_hr_ai-0.0.2/LnT_HR_AI.egg-info/PKG-INFO` & `lnt_hr_ai-0.0.3/LnT_HR_AI.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: LnT_HR_AI
-Version: 0.0.2
+Version: 0.0.3
 Summary: Data analysis for Attrition predictions
 Author: Radeesh
 Author-email: <vpsrad2002@gmail.com>
-Keywords: python,video,stream,video stream,camera stream,sockets
+Keywords: python,Machine Learning,Data Analysis,Data Science,Data processing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: scipy
```

### Comparing `lnt_hr_ai-0.0.2/PKG-INFO` & `lnt_hr_ai-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: LnT_HR_AI
-Version: 0.0.2
+Version: 0.0.3
 Summary: Data analysis for Attrition predictions
 Author: Radeesh
 Author-email: <vpsrad2002@gmail.com>
-Keywords: python,video,stream,video stream,camera stream,sockets
+Keywords: python,Machine Learning,Data Analysis,Data Science,Data processing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: scipy
```

### Comparing `lnt_hr_ai-0.0.2/setup.py` & `lnt_hr_ai-0.0.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Data analysis for Attrition predictions'
 # Setting up
 setup(
     name="LnT_HR_AI",
     version=VERSION,
     author="Radeesh",
     author_email="<vpsrad2002@gmail.com>",
     description=DESCRIPTION,
     packages=find_packages(),
     install_requires=['scipy','catboost','lightgbm','xgboost','matplotlib','seaborn','scikit-learn', 'pyautogui', 'pyaudio'],
-    keywords=['python', 'video', 'stream', 'video stream', 'camera stream', 'sockets'],
+    keywords=['python','Machine Learning','Data Analysis','Data Science','Data processing'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

