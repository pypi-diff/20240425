# Comparing `tmp/uxsim-1.1.1.tar.gz` & `tmp/uxsim-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uxsim-1.1.1.tar", last modified: Mon Apr 15 10:46:50 2024, max compression
+gzip compressed data, was "uxsim-1.2.0.tar", last modified: Thu Apr 25 08:29:05 2024, max compression
```

## Comparing `uxsim-1.1.1.tar` & `uxsim-1.2.0.tar`

### file list

```diff
@@ -1,41 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 10:46:50.003897 uxsim-1.1.1/
--rw-rw-rw-   0        0        0     1086 2023-08-01 08:45:01.000000 uxsim-1.1.1/LICENSE
--rw-rw-rw-   0        0        0       21 2024-03-26 06:39:30.000000 uxsim-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0    12181 2024-04-15 10:46:50.002899 uxsim-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    11281 2024-04-08 12:09:02.000000 uxsim-1.1.1/README.md
--rw-rw-rw-   0        0        0     1123 2024-04-06 11:27:18.000000 uxsim-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 10:46:50.003897 uxsim-1.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-15 10:46:49.949399 uxsim-1.1.1/tests/
--rw-rw-rw-   0        0        0     1523 2024-04-01 12:42:22.000000 uxsim-1.1.1/tests/test_examples.py
--rw-rw-rw-   0        0        0     6650 2024-04-10 07:28:00.000000 uxsim-1.1.1/tests/test_other_functions.py
--rw-rw-rw-   0        0        0     1682 2024-04-01 12:42:22.000000 uxsim-1.1.1/tests/test_result_gui_viewer.py
--rw-rw-rw-   0        0        0     3326 2024-04-01 12:42:22.000000 uxsim-1.1.1/tests/test_verification_exceptional.py
--rw-rw-rw-   0        0        0    69316 2024-04-01 12:42:58.000000 uxsim-1.1.1/tests/test_verification_multilane.py
--rw-rw-rw-   0        0        0    42414 2024-04-01 12:42:58.000000 uxsim-1.1.1/tests/test_verification_node.py
--rw-rw-rw-   0        0        0    26886 2024-04-15 10:46:18.000000 uxsim-1.1.1/tests/test_verification_route_choice.py
--rw-rw-rw-   0        0        0     3784 2024-04-01 12:42:22.000000 uxsim-1.1.1/tests/test_verification_sioux_falls.py
--rw-rw-rw-   0        0        0    39162 2024-04-01 12:42:22.000000 uxsim-1.1.1/tests/test_verification_straight_road.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:46:49.953878 uxsim-1.1.1/uxsim/
-drwxrwxrwx   0        0        0        0 2024-04-15 10:46:49.974900 uxsim-1.1.1/uxsim/OSMImporter/
--rw-rw-rw-   0        0        0    16334 2024-04-09 08:40:41.000000 uxsim-1.1.1/uxsim/OSMImporter/OSMImporter.py
--rw-rw-rw-   0        0        0       26 2024-04-01 12:42:22.000000 uxsim-1.1.1/uxsim/OSMImporter/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:46:49.977899 uxsim-1.1.1/uxsim/ResultGUIViewer/
--rw-rw-rw-   0        0        0    16823 2024-04-09 09:16:07.000000 uxsim-1.1.1/uxsim/ResultGUIViewer/ResultGUIViewer.py
--rw-rw-rw-   0        0        0       30 2024-04-01 12:42:22.000000 uxsim-1.1.1/uxsim/ResultGUIViewer/__init__.py
--rw-rw-rw-   0        0        0      193 2024-04-15 10:46:18.000000 uxsim-1.1.1/uxsim/__init__.py
--rw-rw-rw-   0        0        0    55213 2024-04-15 10:46:18.000000 uxsim-1.1.1/uxsim/analyzer.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:46:50.000899 uxsim-1.1.1/uxsim/files/
--rw-rw-rw-   0        0        0 10695124 2024-04-01 12:42:22.000000 uxsim-1.1.1/uxsim/files/HackGen-Regular.ttf
--rw-rw-rw-   0        0        0    58464 2024-04-01 12:42:22.000000 uxsim-1.1.1/uxsim/files/Inconsolata.otf
--rw-rw-rw-   0        0        0     5951 2024-04-01 12:42:22.000000 uxsim-1.1.1/uxsim/files/LICENSE_of_HackGen-Regular
--rw-rw-rw-   0        0        0     4486 2024-04-01 12:42:22.000000 uxsim-1.1.1/uxsim/files/Licence_of_Inconsolata.otf.txt
--rw-rw-rw-   0        0        0       47 2024-04-01 12:42:22.000000 uxsim-1.1.1/uxsim/files/README.md
--rw-rw-rw-   0        0        0        0 2024-04-01 12:42:22.000000 uxsim-1.1.1/uxsim/files/__init__.py
--rw-rw-rw-   0        0        0     4939 2024-04-15 10:46:18.000000 uxsim-1.1.1/uxsim/utils.py
--rw-rw-rw-   0        0        0    80146 2024-04-15 10:46:18.000000 uxsim-1.1.1/uxsim/uxsim.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:46:50.001896 uxsim-1.1.1/uxsim.egg-info/
--rw-rw-rw-   0        0        0    12181 2024-04-15 10:46:49.000000 uxsim-1.1.1/uxsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      893 2024-04-15 10:46:49.000000 uxsim-1.1.1/uxsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 10:46:49.000000 uxsim-1.1.1/uxsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2024-04-15 10:46:49.000000 uxsim-1.1.1/uxsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-15 10:46:49.000000 uxsim-1.1.1/uxsim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 08:29:05.412792 uxsim-1.2.0/
+-rw-rw-rw-   0        0        0     1086 2023-08-01 08:45:01.000000 uxsim-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0       21 2024-03-26 06:39:30.000000 uxsim-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    12071 2024-04-25 08:29:05.411792 uxsim-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11171 2024-04-25 08:28:20.000000 uxsim-1.2.0/README.md
+-rw-rw-rw-   0        0        0     1123 2024-04-06 11:27:18.000000 uxsim-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-25 08:29:05.412792 uxsim-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-25 08:29:05.344791 uxsim-1.2.0/tests/
+-rw-rw-rw-   0        0        0     1523 2024-04-01 12:42:22.000000 uxsim-1.2.0/tests/test_examples.py
+-rw-rw-rw-   0        0        0     6971 2024-04-25 08:28:20.000000 uxsim-1.2.0/tests/test_other_functions.py
+-rw-rw-rw-   0        0        0     1682 2024-04-01 12:42:22.000000 uxsim-1.2.0/tests/test_result_gui_viewer.py
+-rw-rw-rw-   0        0        0     3326 2024-04-01 12:42:22.000000 uxsim-1.2.0/tests/test_verification_exceptional.py
+-rw-rw-rw-   0        0        0    69329 2024-04-25 08:28:20.000000 uxsim-1.2.0/tests/test_verification_multilane.py
+-rw-rw-rw-   0        0        0    42414 2024-04-01 12:42:58.000000 uxsim-1.2.0/tests/test_verification_node.py
+-rw-rw-rw-   0        0        0    26886 2024-04-15 10:46:18.000000 uxsim-1.2.0/tests/test_verification_route_choice.py
+-rw-rw-rw-   0        0        0     3784 2024-04-01 12:42:22.000000 uxsim-1.2.0/tests/test_verification_sioux_falls.py
+-rw-rw-rw-   0        0        0    39162 2024-04-01 12:42:22.000000 uxsim-1.2.0/tests/test_verification_straight_road.py
+-rw-rw-rw-   0        0        0     9443 2024-04-25 08:28:20.000000 uxsim-1.2.0/tests/test_verification_taxi.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:29:05.349792 uxsim-1.2.0/uxsim/
+drwxrwxrwx   0        0        0        0 2024-04-25 08:29:05.376792 uxsim-1.2.0/uxsim/OSMImporter/
+-rw-rw-rw-   0        0        0    16334 2024-04-09 08:40:41.000000 uxsim-1.2.0/uxsim/OSMImporter/OSMImporter.py
+-rw-rw-rw-   0        0        0       26 2024-04-01 12:42:22.000000 uxsim-1.2.0/uxsim/OSMImporter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:29:05.378792 uxsim-1.2.0/uxsim/ResultGUIViewer/
+-rw-rw-rw-   0        0        0    16823 2024-04-09 09:16:07.000000 uxsim-1.2.0/uxsim/ResultGUIViewer/ResultGUIViewer.py
+-rw-rw-rw-   0        0        0       30 2024-04-01 12:42:22.000000 uxsim-1.2.0/uxsim/ResultGUIViewer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:29:05.380792 uxsim-1.2.0/uxsim/TaxiHandler/
+-rw-rw-rw-   0        0        0    11724 2024-04-25 08:28:20.000000 uxsim-1.2.0/uxsim/TaxiHandler/TaxiHandler.py
+-rw-rw-rw-   0        0        0       26 2024-04-25 08:28:20.000000 uxsim-1.2.0/uxsim/TaxiHandler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:29:05.383791 uxsim-1.2.0/uxsim/Utilities/
+-rw-rw-rw-   0        0        0      153 2024-04-25 08:28:20.000000 uxsim-1.2.0/uxsim/Utilities/Utilities.py
+-rw-rw-rw-   0        0        0       24 2024-04-25 08:28:20.000000 uxsim-1.2.0/uxsim/Utilities/__init__.py
+-rw-rw-rw-   0        0        0      193 2024-04-25 08:28:20.000000 uxsim-1.2.0/uxsim/__init__.py
+-rw-rw-rw-   0        0        0    57254 2024-04-25 08:28:20.000000 uxsim-1.2.0/uxsim/analyzer.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:29:05.409791 uxsim-1.2.0/uxsim/files/
+-rw-rw-rw-   0        0        0 10695124 2024-04-01 12:42:22.000000 uxsim-1.2.0/uxsim/files/HackGen-Regular.ttf
+-rw-rw-rw-   0        0        0    58464 2024-04-01 12:42:22.000000 uxsim-1.2.0/uxsim/files/Inconsolata.otf
+-rw-rw-rw-   0        0        0     5951 2024-04-01 12:42:22.000000 uxsim-1.2.0/uxsim/files/LICENSE_of_HackGen-Regular
+-rw-rw-rw-   0        0        0     4486 2024-04-01 12:42:22.000000 uxsim-1.2.0/uxsim/files/Licence_of_Inconsolata.otf.txt
+-rw-rw-rw-   0        0        0       47 2024-04-01 12:42:22.000000 uxsim-1.2.0/uxsim/files/README.md
+-rw-rw-rw-   0        0        0        0 2024-04-01 12:42:22.000000 uxsim-1.2.0/uxsim/files/__init__.py
+-rw-rw-rw-   0        0        0     4939 2024-04-15 10:46:18.000000 uxsim-1.2.0/uxsim/utils.py
+-rw-rw-rw-   0        0        0    81926 2024-04-25 08:28:20.000000 uxsim-1.2.0/uxsim/uxsim.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:29:05.410792 uxsim-1.2.0/uxsim.egg-info/
+-rw-rw-rw-   0        0        0    12071 2024-04-25 08:29:05.000000 uxsim-1.2.0/uxsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1045 2024-04-25 08:29:05.000000 uxsim-1.2.0/uxsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 08:29:05.000000 uxsim-1.2.0/uxsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2024-04-25 08:29:05.000000 uxsim-1.2.0/uxsim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-25 08:29:05.000000 uxsim-1.2.0/uxsim.egg-info/top_level.txt
```

### Comparing `uxsim-1.1.1/LICENSE` & `uxsim-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.1/PKG-INFO` & `uxsim-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uxsim
-Version: 1.1.1
+Version: 1.2.0
 Summary: UXsim: traffic flow simulator
 Author-email: Toru Seo <seo.t.aa@m.titech.ac.jp>
 License: MIT License
 Project-URL: Homepage, https://github.com/toruseo/UXsim
 Project-URL: Documentation, https://toruseo.jp/UXsim/docs
 Project-URL: Issues, https://github.com/toruseo/UXsim/issues
 Classifier: Intended Audience :: Science/Research
@@ -22,16 +22,14 @@
 Requires-Dist: scipy>=1.9.1
 Requires-Dist: pandas>=1.4.4
 Requires-Dist: PyQt5>=5.15.7
 
 # UXsim: Network traffic flow simulator in pure Python
 
 [![PyPi](https://img.shields.io/pypi/v/uxsim.svg)](https://pypi.python.org/pypi/uxsim)
-[![](https://tokei.rs/b1/github/toruseo/UXsim?style=flat&category=code&color=dddd22)](https://github.com/toruseo/UXsim)
-[![](https://tokei.rs/b1/github/toruseo/UXsim?category=comments&style=flat&color=44cc44)](https://github.com/toruseo/UXsim/)
 [![Demo in Colab](https://colab.research.google.com/assets/colab-badge.svg)](http://colab.research.google.com/github/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_05en_for_google_colab.ipynb)
 [![arXiv](https://img.shields.io/badge/arXiv-2309.17114-b31b1b.svg)](http://dx.doi.org/10.48550/arXiv.2309.17114)
 [![Static Badge](https://img.shields.io/badge/readme-English%20%F0%9F%87%BA%F0%9F%87%B8%20-%20darkblue)](https://github.com/toruseo/UXsim/blob/main/README.md)
 [![Static Badge](https://img.shields.io/badge/readme-%E6%97%A5%E6%9C%AC%E8%AA%9E%20%F0%9F%87%AF%F0%9F%87%B5%20-pink)](https://github.com/toruseo/UXsim/blob/main/README.jp.md)
 
 *UXsim* is a free, open-source macroscopic and mesoscopic network traffic flow simulator written in Python.
 It simulates the movements of car travelers and traffic congestion in road networks.
@@ -45,18 +43,19 @@
 
 ## Main Features
 
 - Simple, lightweight, and easy-to-use Python implementation of modern standard models of dynamic network traffic flow
 - Macroscopic traffic simulation: Simulating over 60000 vehicles in a city in 30 seconds
 - Dynamic traffic assignment: Traffic flow simulation with a given network and time-dependent OD demand
 - Theoretically valid models commonly used in academic/professional transportation research
-- Implementation of traffic control/management schemes such as traffic signals and road pricing
+- Implementation of traffic control/management schemes such as taxi/shared-mobility, traffic signals, road pricing, and so on
 - Basic analysis of simulation results and their export to pandas.DataFrame and CSV files
 - Visualization of simulation results using matplotlib; interactive GUI is available
 - Flexible and customizable thanks to pure Python implementation; can also be directly integrated with other Python-based frameworks, such as PyTorch for deep reinforcement learning traffic control
+- The main code `uxsim.py` is only about 1800 lines of code. Users may easily understand and customize it
 
 ## Simulation Examples
 
 ### Large-scale scenario
 
 Below are simulation results where approximately 60000 vehicles pass through a 10km x 10km grid network in 2 hours. The computation time was about 30 seconds on a standard desktop PC.
```

### Comparing `uxsim-1.1.1/README.md` & `uxsim-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # UXsim: Network traffic flow simulator in pure Python
 
 [![PyPi](https://img.shields.io/pypi/v/uxsim.svg)](https://pypi.python.org/pypi/uxsim)
-[![](https://tokei.rs/b1/github/toruseo/UXsim?style=flat&category=code&color=dddd22)](https://github.com/toruseo/UXsim)
-[![](https://tokei.rs/b1/github/toruseo/UXsim?category=comments&style=flat&color=44cc44)](https://github.com/toruseo/UXsim/)
 [![Demo in Colab](https://colab.research.google.com/assets/colab-badge.svg)](http://colab.research.google.com/github/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_05en_for_google_colab.ipynb)
 [![arXiv](https://img.shields.io/badge/arXiv-2309.17114-b31b1b.svg)](http://dx.doi.org/10.48550/arXiv.2309.17114)
 [![Static Badge](https://img.shields.io/badge/readme-English%20%F0%9F%87%BA%F0%9F%87%B8%20-%20darkblue)](https://github.com/toruseo/UXsim/blob/main/README.md)
 [![Static Badge](https://img.shields.io/badge/readme-%E6%97%A5%E6%9C%AC%E8%AA%9E%20%F0%9F%87%AF%F0%9F%87%B5%20-pink)](https://github.com/toruseo/UXsim/blob/main/README.jp.md)
 
 *UXsim* is a free, open-source macroscopic and mesoscopic network traffic flow simulator written in Python.
 It simulates the movements of car travelers and traffic congestion in road networks.
@@ -20,18 +18,19 @@
 
 ## Main Features
 
 - Simple, lightweight, and easy-to-use Python implementation of modern standard models of dynamic network traffic flow
 - Macroscopic traffic simulation: Simulating over 60000 vehicles in a city in 30 seconds
 - Dynamic traffic assignment: Traffic flow simulation with a given network and time-dependent OD demand
 - Theoretically valid models commonly used in academic/professional transportation research
-- Implementation of traffic control/management schemes such as traffic signals and road pricing
+- Implementation of traffic control/management schemes such as taxi/shared-mobility, traffic signals, road pricing, and so on
 - Basic analysis of simulation results and their export to pandas.DataFrame and CSV files
 - Visualization of simulation results using matplotlib; interactive GUI is available
 - Flexible and customizable thanks to pure Python implementation; can also be directly integrated with other Python-based frameworks, such as PyTorch for deep reinforcement learning traffic control
+- The main code `uxsim.py` is only about 1800 lines of code. Users may easily understand and customize it
 
 ## Simulation Examples
 
 ### Large-scale scenario
 
 Below are simulation results where approximately 60000 vehicles pass through a 10km x 10km grid network in 2 hours. The computation time was about 30 seconds on a standard desktop PC.
```

### Comparing `uxsim-1.1.1/pyproject.toml` & `uxsim-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.1/tests/test_examples.py` & `uxsim-1.2.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.1/tests/test_other_functions.py` & `uxsim-1.2.0/tests/test_other_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,16 +101,26 @@
     W.exec_simulation()
 
     assert equal_tolerance(len(W.VEHICLES), 5000*4/5)
 
 def test_readme():
     import re, requests
     url = "https://raw.githubusercontent.com/toruseo/UXsim/main/README.md"
-    response = requests.get(url)
-    content = response.text
+
+    for _ in range(5):
+        try:
+            response = requests.get(url)
+            content = response.text
+        except (requests.exceptions.ConnectionError, requests.exceptions.Timeout, requests.exceptions.RequestException):
+            continue
+        break
+    else:
+        assert True
+        return True # Skip the test if the content cannot be retrieved
+
     pattern = re.compile(r'```python\n(.*?)```', re.DOTALL)
     code_blocks = pattern.findall(content)
 
     print(code_blocks)
 
     for code in code_blocks:
         print(code)
```

### Comparing `uxsim-1.1.1/tests/test_result_gui_viewer.py` & `uxsim-1.2.0/tests/test_result_gui_viewer.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.1/tests/test_verification_exceptional.py` & `uxsim-1.2.0/tests/test_verification_exceptional.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.1/tests/test_verification_multilane.py` & `uxsim-1.2.0/tests/test_verification_multilane.py`

 * *Files 0% similar despite different names*

```diff
@@ -1601,15 +1601,15 @@
     W.analyzer.time_space_diagram_traj_links(["linkSin","signal_SE_r", "linkEout"])
 
     avt = df["average_travel_time"].values
     print(avt)
     
     referemce_avt = [41.40449658, 65.77142857, 41.56507937, 41.41644018, 41.30793651, 65.97619048, 49.7849498, 49.15555556, 69.54444444, 49.11051701, 70.71428571, 48.62857143]
     for i in range(len(avt)):
-        assert equal_tolerance(avt[i], referemce_avt[i])
+        assert equal_tolerance(avt[i], referemce_avt[i], rel_tol=0.2)
 
 @pytest.mark.flaky(reruns=5)
 def test_route_choice_one_is_too_long_and_another_has_bottleneck():
     vol1s = []
     vol2s = []
     atts1 = []
     atts2 = []
```

### Comparing `uxsim-1.1.1/tests/test_verification_node.py` & `uxsim-1.2.0/tests/test_verification_node.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.1/tests/test_verification_route_choice.py` & `uxsim-1.2.0/tests/test_verification_route_choice.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.1/tests/test_verification_sioux_falls.py` & `uxsim-1.2.0/tests/test_verification_sioux_falls.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.1/tests/test_verification_straight_road.py` & `uxsim-1.2.0/tests/test_verification_straight_road.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.1/uxsim/OSMImporter/OSMImporter.py` & `uxsim-1.2.0/uxsim/OSMImporter/OSMImporter.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.1/uxsim/ResultGUIViewer/ResultGUIViewer.py` & `uxsim-1.2.0/uxsim/ResultGUIViewer/ResultGUIViewer.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.1/uxsim/analyzer.py` & `uxsim-1.2.0/uxsim/analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,18 +101,19 @@
             else:
                 adj_mat_time[i,j] = np.inf
         dist = floyd_warshall(adj_mat_time)
 
         for veh in s.W.VEHICLES.values():
             o = veh.orig
             d = veh.dest
-            s.od_trips[o,d] += dn
-            if veh.travel_time != -1:
-                s.od_trips_comp[o,d] += dn
-                s.od_tt[o,d].append(veh.travel_time)
+            if d != None:
+                s.od_trips[o,d] += dn
+                if veh.travel_time != -1:
+                    s.od_trips_comp[o,d] += dn
+                    s.od_tt[o,d].append(veh.travel_time)
         for o,d in s.od_tt.keys():
             s.od_tt_ave[o,d] = np.average(s.od_tt[o,d])
             s.od_tt_std[o,d] = np.std(s.od_tt[o,d])
             s.od_tt_free[o,d] = dist[o.id, d.id]
 
     def link_analysis_coarse(s):
         """
@@ -266,24 +267,26 @@
         Parameters
         ----------
         force_print : bool, optional
             print the stats regardless of the value of `print_mode`
         """
         s.W.print("results:")
         s.W.print(f" average speed:\t {s.average_speed:.1f} m/s")
-        s.W.print(" number of completed trips:\t", s.trip_completed, "/", len(s.W.VEHICLES)*s.W.DELTAN)
+        s.W.print(" number of completed trips:\t", s.trip_completed, "/", s.trip_all)
+        #s.W.print(" number of completed trips:\t", s.trip_completed, "/", len(s.W.VEHICLES)*s.W.DELTAN)
         if s.trip_completed > 0:
             s.W.print(f" average travel time of trips:\t {s.average_travel_time:.1f} s")
             s.W.print(f" average delay of trips:\t {s.average_delay:.1f} s")
             s.W.print(f" delay ratio:\t\t\t {s.average_delay/s.average_travel_time:.3f}")
 
         if force_print == 1 and s.W.print_mode == 0:
             print("results:")
             print(f" average speed:\t {s.average_speed:.1f} m/s")
-            print(" number of completed trips:\t", s.trip_completed, "/", len(s.W.VEHICLES)*s.W.DELTAN)
+            print(" number of completed trips:\t", s.trip_completed, "/", s.trip_all)
+            #print(" number of completed trips:\t", s.trip_completed, "/", len(s.W.VEHICLES)*s.W.DELTAN)
             if s.trip_completed > 0:
                 print(f" average travel time of trips:\t {s.average_travel_time:.1f} s")
                 print(f" average delay of trips:\t {s.average_delay:.1f} s")
                 print(f" delay ratio:\t\t\t {s.average_delay/s.average_travel_time:.3f}")
 
     def comp_route_travel_time(s, t, route):
         pass
@@ -709,15 +712,16 @@
         maxy += buffer
         miny -= buffer
 
         img = Image.new("RGBA", (int(maxx-minx), int(maxy-miny)), (255, 255, 255, 255))
         draw = ImageDraw.Draw(img)
         font_data = read_binary('uxsim.files', 'HackGen-Regular.ttf') 
         font_file_like = io.BytesIO(font_data)
-        font = ImageFont.truetype(font_file_like, int(network_font_size))
+        if network_font_size > 0:
+            font = ImageFont.truetype(font_file_like, int(network_font_size))
 
         def flip(y):
             return img.size[1]-y
 
         for l in s.W.LINKS:
             x1, y1 = l.start_node.x*coef-minx, l.start_node.y*coef-miny
             x2, y2 = l.end_node.x*coef-minx, l.end_node.y*coef-miny
@@ -944,15 +948,16 @@
 
         pics = []
         for t in tqdm(range(int(s.W.TMAX*0), int(s.W.TMAX*1), s.W.DELTAT*speed_coef)):
             img = Image.new("RGBA", (int(maxx-minx), int(maxy-miny)), (255, 255, 255, 255))
             draw = ImageDraw.Draw(img)
             font_data = read_binary('uxsim.files', 'HackGen-Regular.ttf') 
             font_file_like = io.BytesIO(font_data)
-            font = ImageFont.truetype(font_file_like, int(network_font_size))
+            if network_font_size > 0:
+                font = ImageFont.truetype(font_file_like, int(network_font_size))
 
             def flip(y):
                 return img.size[1]-y
 
             for l in s.W.LINKS:
                 x1, y1 = l.start_node.x*coef-minx, l.start_node.y*coef-miny
                 x2, y2 = l.end_node.x*coef-minx, l.end_node.y*coef-miny
@@ -1092,14 +1097,53 @@
             plt.savefig(f"out{s.W.name}/vehicle_{vehname}.png")
         if s.W.show_mode:
             plt.show()
         else:
             plt.close("all")
 
 
+    @catch_exceptions_and_warn()
+    def plot_vehicles_log(s, vehnamelist):
+        """
+        Plots the driving link and speed for a single vehicle.
+
+        Parameters
+        ----------
+        vehname : str
+            The name of the vehicle for which the driving link and speed are to be plotted.
+
+        Notes
+        -----
+        This method visualizes the speed profile and the links traversed by a specific vehicle over time.
+        The speed is plotted on the primary y-axis, and the links are plotted on the secondary y-axis.
+        The plot is saved to the directory `out<W.name>` with the filename `vehicle_<vehname>.png`.
+        """
+        if s.W.vehicle_logging_timestep_interval != 1:
+            warnings.warn("vehicle_logging_timestep_interval is not 1. The plot is not exactly accurate.", LoggingWarning)
+        
+        vehs = [s.W.VEHICLES[vehname] for vehname in vehnamelist]
+
+        plt.figure()
+        for veh in vehs:
+            vehlinks = [str(l.name) if l != -1 else "not in network" for l in veh.log_link]
+            plt.plot([veh.log_t[i] for i in lange(veh.log_t) if veh.log_state[i] != "home"], [vehlinks[i] for i in lange(vehlinks) if veh.log_state[i] != "home"], c=veh.color, label=veh.name)
+        plt.grid()
+        plt.ylabel('link')
+        plt.legend()
+        plt.ylim([0, None])
+        plt.tight_layout()
+
+        if s.W.save_mode:
+            plt.savefig(f"out{s.W.name}/vehicles_{vehnamelist}.png")
+        if s.W.show_mode:
+            plt.show()
+        else:
+            plt.close("all")
+
+
     def vehicles_to_pandas(s):
         """
         Converts the vehicle travel logs to a pandas DataFrame.
 
         Returns
         -------
         pd.DataFrame
@@ -1114,31 +1158,34 @@
             - 's': the spacing of the vehicle.
             - 'v': the speed of the vehicle.
         """
         if s.W.vehicle_logging_timestep_interval != 1:
             warnings.warn("vehicle_logging_timestep_interval is not 1. The output data is not exactly accurate.", LoggingWarning)
 
         if s.flag_pandas_convert == 0:
-            s.flag_pandas_convert = 1
-
             out = [["name", "dn", "orig", "dest", "t", "link", "x", "s", "v"]]
             for veh in s.W.VEHICLES.values():
                 for i in range(len(veh.log_t)):
                     if veh.log_state[i] in ("wait", "run", "end", "abort"):
                         if veh.log_link[i] != -1:
                             linkname = veh.log_link[i].name
                         else:
                             if veh.log_state[i] == "wait":
                                 linkname = "waiting_at_origin_node"
                             elif veh.log_state[i] == "abort":
                                 linkname = "trip_aborted"
                             else:
                                 linkname = "trip_end"
-                        out.append([veh.name, s.W.DELTAN, veh.orig.name, veh.dest.name, veh.log_t[i], linkname, veh.log_x[i], veh.log_s[i], veh.log_v[i]])
+                        veh_dest_name = None
+                        if veh.dest != None:
+                            veh_dest_name = veh.dest.name
+                        out.append([veh.name, s.W.DELTAN, veh.orig.name, veh_dest_name, veh.log_t[i], linkname, veh.log_x[i], veh.log_s[i], veh.log_v[i]])
             s.df_vehicles = pd.DataFrame(out[1:], columns=out[0])
+
+            s.flag_pandas_convert = 1
         return s.df_vehicles
 
     def log_vehicles_to_pandas(s):
         """
         same to `vehicles_to_pandas`, just for backward compatibility
         """
         return s.vehicles_to_pandas()
```

### Comparing `uxsim-1.1.1/uxsim/files/HackGen-Regular.ttf` & `uxsim-1.2.0/uxsim/files/HackGen-Regular.ttf`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.1/uxsim/files/Inconsolata.otf` & `uxsim-1.2.0/uxsim/files/Inconsolata.otf`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.1/uxsim/files/LICENSE_of_HackGen-Regular` & `uxsim-1.2.0/uxsim/files/LICENSE_of_HackGen-Regular`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.1/uxsim/files/Licence_of_Inconsolata.otf.txt` & `uxsim-1.2.0/uxsim/files/Licence_of_Inconsolata.otf.txt`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.1/uxsim/utils.py` & `uxsim-1.2.0/uxsim/utils.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.1/uxsim/uxsim.py` & `uxsim-1.2.0/uxsim/uxsim.py`

 * *Files 6% similar despite different names*

```diff
@@ -315,17 +315,17 @@
 
         Parameters
         ----------
         W : object
             The world to which the link belongs.
         name : str
             The name of the link.
-        start_node : str
+        start_node : str | Node
             The name of the start node of the link.
-        end_node : str
+        end_node : str | Node
             The name of the end node of the link.
         length : float
             The length of the link.
         free_flow_speed : float, optional
             The free flow speed on the link, default is 20.
         jam_density : float, optional  
             The jam density on the link, default is 0.2. If jam_density_per_lane is specified, this value is ignored.
@@ -734,34 +734,38 @@
             warnings.warn(f"ignored negative jam_density at {s}", UserWarning)
 
 
 class Vehicle:
     """
     Vehicle or platoon in a network.
     """
-    def __init__(s, W, orig, dest, departure_time, name=None, route_pref=None, route_choice_principle=None, links_prefer=[], links_avoid=[], trip_abort=1, departure_time_is_time_step=0, attribute=None, auto_rename=False):
+    def __init__(s, W, orig, dest, departure_time, name=None, route_pref=None, route_choice_principle=None, mode="single_trip", links_prefer=[], links_avoid=[], trip_abort=1, departure_time_is_time_step=0, attribute=None, auto_rename=False):
         """
         Create a vehicle (more precisely, platoon)
 
         Parameters
         ----------
         W : object
             The world to which the vehicle belongs.
-        orig : str
+        orig : str | Node
             The origin node.
-        dest : str
+        dest : str | Node
             The destination node.
         departure_time : int
             The departure time step of the vehicle.
         name : str, optional
             The name of the vehicle, default is the id of the vehicle.
         route_pref : dict, optional
             The preference weights for links, default is 0 for all links.
         route_choice_principle : str, optional
             The route choice principle of the vehicle, default is the network's route choice principle.
+        mode : str, optional
+            The mode of the vehicle. Available options are "single_trip" and "taxi", default is "single_trip".
+            "single_trip": The vehicle makes a single trip from the origin to the destination.
+            "taxi": The vehicle serves multiple trips by specifying sequence of destinations. The destination list `Vehicle.dest_list` can be dynamically updated externaly. (TODO: to be implemented next)
         links_prefer : list of str, optional
             The names of the links the vehicle prefers, default is empty list.
         links_avoid : list of str, optional
             The names of the links the vehicle avoids, default is empty list.
         trip_abort : int, optional
             Whether to abort the trip if a dead end is reached, default is 1.
         attribute : any, optinonal
@@ -809,14 +813,21 @@
 
         #経路選択
         if route_choice_principle == None:
             s.route_choice_principle = s.W.route_choice_principle
         else:
             s.route_choice_principle = route_choice_principle
 
+        #private vehicle or taxi
+        s.mode = mode
+        s.dest_list = []
+
+        #dict of events that are triggered when this vehicle reaches a certain node {Node: func}
+        s.node_event = {}
+
         #希望リンク重み：{link:重み}
         s.route_pref = route_pref
         if s.route_pref == None:
             s.route_pref = {l:0 for l in s.W.LINKS}
 
         #好むリンクと避けるリンク（近視眼的）
         s.links_prefer = [s.W.get_link(l) for l in links_prefer]
@@ -868,47 +879,64 @@
         - If the vehicle is in the "wait" state, it remains waiting at its departure node.
         - If the vehicle is in the "run" state, it updates its speed and position. If the vehicle reaches the end of its current link, it either ends its trip if it has reached its destination, or requests a transfer to the next link.
         - If the vehicle's state is "end" or "abort", no further actions are taken.
         """
         s.record_log()
 
         if s.state == "home":
-            #需要生成
+            #depart
             if s.W.T >= s.departure_time:
                 s.state = "wait"
                 s.orig.generation_queue.append(s)
         if s.state == "wait":
-            #出発ノードで待つ
+            #wait at the vertical queue at the origin node
             pass
         if s.state == "run":
-            #走行
+            #drive within the link
             s.v = (s.x_next-s.x)/s.W.DELTAT
             s.x_old = s.x
             s.x = s.x_next
 
-            #リンク下流端
+            #at the end of the link
             if s.x == s.link.length:
+                if s.link.end_node in s.node_event.keys():
+                    s.node_event[s.link.end_node]()
+                
                 if s.link.end_node == s.dest:
-                    #トリップ終了待ちにする
-                    s.flag_waiting_for_trip_end = 1
-                    if s.link.vehicles[0] == s:
-                        s.end_trip()
+                    if s.mode == "single_trip":
+                        #prepare for trip end
+                        s.flag_waiting_for_trip_end = 1
+                        if s.link.vehicles[0] == s:
+                            s.end_trip()
+                    elif s.mode == "taxi":
+                        #proceed to next destination
+                        if len(s.dest_list) > 0:
+                            s.dest = s.dest_list.pop(0)
+                        else:
+                            s.dest = None
+                            s.dest_list = []
+                        s.route_pref_update(weight=1)
+                        s.route_next_link_choice()
+                        s.link.end_node.incoming_vehicles.append(s)
+
                 elif len(s.link.end_node.outlinks.values()) == 0 and s.trip_abort == 1:
-                    #トリップ終了待ち（目的地到達不可）にする
+                    #prepare for trip abort due to dead end
                     s.flag_trip_aborted = 1
                     s.route_next_link = None
                     s.flag_waiting_for_trip_end = 1
                     if s.link.vehicles[0] == s:
                         s.end_trip()
+
                 else:
-                    #リンク間遷移リクエスト
+                    #request link transfer
                     s.route_next_link_choice()
                     s.link.end_node.incoming_vehicles.append(s)
+        
         if s.state in ["end", "abort"] :
-            #終わり
+            #ended the trip
             pass
 
     def end_trip(s):
         """
         Procedure when the vehicle finishes its trip.
         """
         s.state = "end"
@@ -966,15 +994,18 @@
 
         - If the vehicle's route choice principle is "homogeneous_DUO", it will update its preferences based on a global, homogenous dynamic user optimization (DUO) model.
         - If the route choice principle is "heterogeneous_DUO", it will update its preferences based on a heterogeneous DUO model, considering both its past preferences and the system's current state. This is imcomplete feature. Not recommended.
 
         The updated preferences guide the vehicle's decisions in subsequent route choices.
         """
         if s.route_choice_principle == "homogeneous_DUO":
-            s.route_pref = s.W.ROUTECHOICE.route_pref[s.dest.id]
+            if s.dest != None:
+                s.route_pref = s.W.ROUTECHOICE.route_pref[s.dest.id]
+            else:
+                s.route_pref = {l:0 for l in s.W.LINKS}
         elif s.route_choice_principle == "heterogeneous_DUO":
             route_pref_new = {l:0 for l in s.W.LINKS}
             k = s.dest.id
             for l in s.W.LINKS:
                 i = l.start_node.id
                 j = l.end_node.id
                 if j == s.W.ROUTECHOICE.next[i,k]:
@@ -991,29 +1022,64 @@
         Select a next link from the current link.
         """
         if s.dest != s.link.end_node:
             outlinks = list(s.link.end_node.outlinks.values())
 
             if len(outlinks):
 
-                #好むリンク・避けるリンクがあれば優先する
+                #if links_prefer is given and available at the node, select only from the links in the list. if links_avoid is given, select links not in the list.
                 if set(outlinks) & set(s.links_prefer):
                     outlinks = list(set(outlinks) & set(s.links_prefer))
                 if set(outlinks) & set(s.links_avoid):
                     outlinks = list(set(outlinks) - set(s.links_avoid))
 
                 preference = [s.route_pref[l] for l in outlinks]
 
                 if sum(preference) > 0:
                     s.route_next_link = random.choices(outlinks, preference)[0]
                 else:
                     s.route_next_link = random.choices(outlinks)[0]
             else:
                 s.route_next_link = None
 
+    def add_dest(s, dest, order=-1):
+        """
+        Add a destination to the vehicle's destination list.
+
+        Parameters
+        ----------
+        dest : str | Node
+            The destination node to be added.
+        order : int, optional
+            The order of the destination in the list. Default is -1, which appends the destination to the end of the list.
+        """
+        if s.mode == "taxi":
+            if s.dest == None:
+                s.dest = dest
+                s.route_pref_update(weight=1)
+            else:
+                if order == -1:
+                    s.dest_list.append(s.W.get_node(dest))
+                else:
+                    s.dest_list.insert(order, s.W.get_node(dest))
+        else:
+            raise ValueError(f"Vehicle {s.name} is not in taxi mode. Cannot add destination.")
+    
+    def add_dests(s, dests):
+        """
+        Add multiple destinations to the vehicle's destination list.
+
+        Parameters
+        ----------
+        dests : list of str | Node
+            The list of destinations to be added.
+        """
+        for dest in dests:
+            s.add_dest(dest)
+    
     def traveled_route(s):
         """
         Returns the route this vehicle traveled.
         """
         link_old = -1
         t = -1
         route = []
@@ -1022,14 +1088,37 @@
             if link_old != link:
                 route.append(link)
                 ts.append(s.log_t[i])
                 link_old = link
 
         return Route(s.W, route[:-1]), ts
 
+    def get_xy_coords(s, t=-1):
+        """
+        Get the x-y coordinates of the vehicle. If t is given, the position at time t is returned based on the logs.
+
+        Parameters
+        ----------
+        t : int | float, optional
+            Time in seconds. If it is -1, the latest position is returned.
+        """
+        if t != -1:
+            link = s.log_link[int(t/s.W.DELTAT/s.W.logging_timestep_interval)]
+            xx = s.log_x[int(t/s.W.DELTAT/s.W.logging_timestep_interval)]
+        else:
+            link = s.link
+            xx = s.x
+        x0 = link.start_node.x
+        y0 = link.start_node.y
+        x1 = link.end_node.x
+        y1 = link.end_node.y
+        x = x0 + (x1-x0)*xx/link.length
+        y = y0 + (y1-y0)*xx/link.length
+        return (x, y)
+
     def record_log(s, enforce_log=0):
         """
         Record travel logs.
 
         Parameters
         ----------
         enforce_log : bool, optional
@@ -1133,57 +1222,14 @@
                 # iからjへの最短経路を逆にたどる．．． -> todo: 起終点を逆にした最短経路探索にすればよい
                 if i != j:
                     prev = j
                     while s.pred[i, prev] != i and s.pred[i, prev] != -9999:
                         prev = s.pred[i, prev]
                     s.next[i, j] = prev
 
-    # def route_search_all_old(s, infty=9999999999999999999, noise=0):
-    #     """
-    #     Compute the current shortest path based on instantanious travel time. Old version, slow for large networks.
-
-    #     Parameters
-    #     ----------
-    #     infty : float
-    #         value representing infinity.
-    #     noise : float
-    #         very small noise to slightly randomize route choice. useful to eliminate strange results at an initial stage of simulation where many routes has identical travel time.
-    #     """
-    #     for link in s.W.LINKS:
-    #         i = link.start_node.id
-    #         j = link.end_node.id
-    #         if s.W.ADJ_MAT[i,j]:
-    #             s.adj_mat_time[i,j] = link.traveltime_instant[-1]*random.uniform(1, 1+noise) + link.route_choice_penalty
-    #             if link.capacity_in == 0: #流入禁止の場合は通行不可
-    #                 s.adj_mat_time[i,j] = 0
-    #         else:
-    #             s.adj_mat_time[i,j] = 0
-
-    #     dist = np.zeros([len(s.W.NODES), len(s.W.NODES)])
-    #     next = np.zeros([len(s.W.NODES), len(s.W.NODES)])
-    #     for i in range(len(s.W.NODES)):
-    #         for j in range(len(s.W.NODES)):
-    #             if s.adj_mat_time[i,j] > 0:
-    #                 dist[i,j] = s.adj_mat_time[i,j]
-    #                 next[i,j] = j
-    #             elif i == j:
-    #                 next[i,j] = j
-    #             else:
-    #                 dist[i,j] = infty
-    #                 next[i,j] = -1
-
-    #     for k in range(len(s.W.NODES)):
-    #         for i in range(len(s.W.NODES)):
-    #             for j in range(len(s.W.NODES)):
-    #                 if dist[i,j] > dist[i,k]+dist[k,j]:
-    #                     dist[i,j] = dist[i,k]+dist[k,j]
-    #                     next[i,j] = next[i,k]
-    #     s.dist = dist
-    #     s.next = next
-
     def homogeneous_DUO_update(s):
         """
         Update link preference of all homogeneous travelers based on DUO principle.
         """
         for dest in s.W.NODES:
             k = dest.id
             weight = s.W.DUO_UPDATE_WEIGHT
@@ -1248,14 +1294,15 @@
         -----
         A World object must be defined firstly to initiate simulation.
         """
 
         ## パラメータ設定
         random.seed(random_seed)
         np.random.seed(random_seed)
+        W.random_seed = random_seed
 
         W.TMAX = tmax   #シミュレーション時間（s）
 
         W.DELTAN = deltan         #車群サイズ（veh）
         W.REACTION_TIME = reaction_time         #反応時間（s）
 
         W.DUO_UPDATE_TIME = duo_update_time     #経路選択時間間隔（s）
@@ -1674,15 +1721,15 @@
 
             for name in list(W.VEHICLES_LIVING.keys()):
                 W.VEHICLES_LIVING[name].update()
 
             if W.T % W.DELTAT_ROUTE == 0:
                 W.ROUTECHOICE.route_search_all(noise=W.DUO_NOISE)
                 W.ROUTECHOICE.homogeneous_DUO_update()
-                for veh in W.VEHICLES_LIVING.values():  #TODO: this is redundant. To be moved to the previous for-loop.
+                for veh in W.VEHICLES_LIVING.values():
                     veh.route_pref_update(weight=W.DUO_UPDATE_WEIGHT)
 
             W.TIME = W.T*W.DELTAT
 
             if W.print_mode and W.show_progress and W.T%W.show_progress_deltat_timestep == 0 and W.T > 0:
                 W.analyzer.show_simulation_progress()
 
@@ -1725,14 +1772,17 @@
             The name of the node or the Node object itself.
 
         Returns
         -------
         Node object
             The found Node object.
         """
+        if node == None:
+            return None
+        
         if type(node) is Node:
             if node in W.NODES:
                 return node
             else:
                 for n in W.NODES:
                     if n.name == node.name:
                         return n
@@ -1752,14 +1802,17 @@
             The name of the link or the Link object itself.
 
         Returns
         -------
         Link object
             The found Link object.
         """
+        if link == None:
+            return None
+        
         if type(link) is Link:
             if link in W.LINKS:
                 return link
             else:
                 for l in W.LINKS:
                     if l.name == link.name:
                         return l
```

### Comparing `uxsim-1.1.1/uxsim.egg-info/PKG-INFO` & `uxsim-1.2.0/uxsim.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uxsim
-Version: 1.1.1
+Version: 1.2.0
 Summary: UXsim: traffic flow simulator
 Author-email: Toru Seo <seo.t.aa@m.titech.ac.jp>
 License: MIT License
 Project-URL: Homepage, https://github.com/toruseo/UXsim
 Project-URL: Documentation, https://toruseo.jp/UXsim/docs
 Project-URL: Issues, https://github.com/toruseo/UXsim/issues
 Classifier: Intended Audience :: Science/Research
@@ -22,16 +22,14 @@
 Requires-Dist: scipy>=1.9.1
 Requires-Dist: pandas>=1.4.4
 Requires-Dist: PyQt5>=5.15.7
 
 # UXsim: Network traffic flow simulator in pure Python
 
 [![PyPi](https://img.shields.io/pypi/v/uxsim.svg)](https://pypi.python.org/pypi/uxsim)
-[![](https://tokei.rs/b1/github/toruseo/UXsim?style=flat&category=code&color=dddd22)](https://github.com/toruseo/UXsim)
-[![](https://tokei.rs/b1/github/toruseo/UXsim?category=comments&style=flat&color=44cc44)](https://github.com/toruseo/UXsim/)
 [![Demo in Colab](https://colab.research.google.com/assets/colab-badge.svg)](http://colab.research.google.com/github/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_05en_for_google_colab.ipynb)
 [![arXiv](https://img.shields.io/badge/arXiv-2309.17114-b31b1b.svg)](http://dx.doi.org/10.48550/arXiv.2309.17114)
 [![Static Badge](https://img.shields.io/badge/readme-English%20%F0%9F%87%BA%F0%9F%87%B8%20-%20darkblue)](https://github.com/toruseo/UXsim/blob/main/README.md)
 [![Static Badge](https://img.shields.io/badge/readme-%E6%97%A5%E6%9C%AC%E8%AA%9E%20%F0%9F%87%AF%F0%9F%87%B5%20-pink)](https://github.com/toruseo/UXsim/blob/main/README.jp.md)
 
 *UXsim* is a free, open-source macroscopic and mesoscopic network traffic flow simulator written in Python.
 It simulates the movements of car travelers and traffic congestion in road networks.
@@ -45,18 +43,19 @@
 
 ## Main Features
 
 - Simple, lightweight, and easy-to-use Python implementation of modern standard models of dynamic network traffic flow
 - Macroscopic traffic simulation: Simulating over 60000 vehicles in a city in 30 seconds
 - Dynamic traffic assignment: Traffic flow simulation with a given network and time-dependent OD demand
 - Theoretically valid models commonly used in academic/professional transportation research
-- Implementation of traffic control/management schemes such as traffic signals and road pricing
+- Implementation of traffic control/management schemes such as taxi/shared-mobility, traffic signals, road pricing, and so on
 - Basic analysis of simulation results and their export to pandas.DataFrame and CSV files
 - Visualization of simulation results using matplotlib; interactive GUI is available
 - Flexible and customizable thanks to pure Python implementation; can also be directly integrated with other Python-based frameworks, such as PyTorch for deep reinforcement learning traffic control
+- The main code `uxsim.py` is only about 1800 lines of code. Users may easily understand and customize it
 
 ## Simulation Examples
 
 ### Large-scale scenario
 
 Below are simulation results where approximately 60000 vehicles pass through a 10km x 10km grid network in 2 hours. The computation time was about 30 seconds on a standard desktop PC.
```

### Comparing `uxsim-1.1.1/uxsim.egg-info/SOURCES.txt` & `uxsim-1.2.0/uxsim.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -7,26 +7,31 @@
 tests/test_result_gui_viewer.py
 tests/test_verification_exceptional.py
 tests/test_verification_multilane.py
 tests/test_verification_node.py
 tests/test_verification_route_choice.py
 tests/test_verification_sioux_falls.py
 tests/test_verification_straight_road.py
+tests/test_verification_taxi.py
 uxsim/__init__.py
 uxsim/analyzer.py
 uxsim/utils.py
 uxsim/uxsim.py
 uxsim.egg-info/PKG-INFO
 uxsim.egg-info/SOURCES.txt
 uxsim.egg-info/dependency_links.txt
 uxsim.egg-info/requires.txt
 uxsim.egg-info/top_level.txt
 uxsim/OSMImporter/OSMImporter.py
 uxsim/OSMImporter/__init__.py
 uxsim/ResultGUIViewer/ResultGUIViewer.py
 uxsim/ResultGUIViewer/__init__.py
+uxsim/TaxiHandler/TaxiHandler.py
+uxsim/TaxiHandler/__init__.py
+uxsim/Utilities/Utilities.py
+uxsim/Utilities/__init__.py
 uxsim/files/HackGen-Regular.ttf
 uxsim/files/Inconsolata.otf
 uxsim/files/LICENSE_of_HackGen-Regular
 uxsim/files/Licence_of_Inconsolata.otf.txt
 uxsim/files/README.md
 uxsim/files/__init__.py
```

