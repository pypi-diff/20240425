# Comparing `tmp/LiveTune-0.0.7.tar.gz` & `tmp/LiveTune-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LiveTune-0.0.7.tar", last modified: Wed Nov 15 23:15:11 2023, max compression
+gzip compressed data, was "LiveTune-0.0.8.tar", last modified: Thu Apr 25 18:03:08 2024, max compression
```

## Comparing `LiveTune-0.0.7.tar` & `LiveTune-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 soheilxi   (501) staff       (20)        0 2023-11-15 23:15:11.439221 LiveTune-0.0.7/
--rw-r--r--   0 soheilxi   (501) staff       (20)     1808 2023-11-02 17:56:15.000000 LiveTune-0.0.7/LICENSE
--rw-r--r--   0 soheilxi   (501) staff       (20)     7101 2023-11-15 23:15:11.439060 LiveTune-0.0.7/PKG-INFO
--rw-r--r--   0 soheilxi   (501) staff       (20)     6392 2023-11-15 23:03:09.000000 LiveTune-0.0.7/README.md
--rw-r--r--   0 soheilxi   (501) staff       (20)       38 2023-11-15 23:15:11.439265 LiveTune-0.0.7/setup.cfg
--rw-r--r--   0 soheilxi   (501) staff       (20)     1049 2023-11-15 23:15:00.000000 LiveTune-0.0.7/setup.py
-drwxr-xr-x   0 soheilxi   (501) staff       (20)        0 2023-11-15 23:15:11.435407 LiveTune-0.0.7/src/
-drwxr-xr-x   0 soheilxi   (501) staff       (20)        0 2023-11-15 23:15:11.437118 LiveTune-0.0.7/src/LiveTune/
--rw-r--r--   0 soheilxi   (501) staff       (20)     5659 2023-11-02 17:56:15.000000 LiveTune-0.0.7/src/LiveTune/LiveVariableBase.py
--rw-r--r--   0 soheilxi   (501) staff       (20)      190 2023-09-11 17:39:09.000000 LiveTune-0.0.7/src/LiveTune/__init__.py
--rw-r--r--   0 soheilxi   (501) staff       (20)     1689 2023-10-04 03:16:42.000000 LiveTune-0.0.7/src/LiveTune/liveTrigger.py
--rwxr-xr-x   0 soheilxi   (501) staff       (20)     7152 2023-10-04 03:20:14.000000 LiveTune-0.0.7/src/LiveTune/liveVar.py
-drwxr-xr-x   0 soheilxi   (501) staff       (20)        0 2023-11-15 23:15:11.438295 LiveTune-0.0.7/src/LiveTune/tools/
--rw-r--r--   0 soheilxi   (501) staff       (20)       42 2023-09-11 17:39:40.000000 LiveTune-0.0.7/src/LiveTune/tools/__init__.py
--rw-r--r--   0 soheilxi   (501) staff       (20)     4060 2023-11-15 21:59:10.000000 LiveTune-0.0.7/src/LiveTune/tools/tune.py
-drwxr-xr-x   0 soheilxi   (501) staff       (20)        0 2023-11-15 23:15:11.437916 LiveTune-0.0.7/src/LiveTune.egg-info/
--rw-r--r--   0 soheilxi   (501) staff       (20)     7101 2023-11-15 23:15:11.000000 LiveTune-0.0.7/src/LiveTune.egg-info/PKG-INFO
--rw-r--r--   0 soheilxi   (501) staff       (20)      392 2023-11-15 23:15:11.000000 LiveTune-0.0.7/src/LiveTune.egg-info/SOURCES.txt
--rw-r--r--   0 soheilxi   (501) staff       (20)        1 2023-11-15 23:15:11.000000 LiveTune-0.0.7/src/LiveTune.egg-info/dependency_links.txt
--rw-r--r--   0 soheilxi   (501) staff       (20)       50 2023-11-15 23:15:11.000000 LiveTune-0.0.7/src/LiveTune.egg-info/entry_points.txt
--rw-r--r--   0 soheilxi   (501) staff       (20)        9 2023-11-15 23:15:11.000000 LiveTune-0.0.7/src/LiveTune.egg-info/top_level.txt
-drwxr-xr-x   0 soheilxi   (501) staff       (20)        0 2023-11-15 23:15:11.438632 LiveTune-0.0.7/tests/
--rw-r--r--   0 soheilxi   (501) staff       (20)    11225 2023-11-15 21:59:10.000000 LiveTune-0.0.7/tests/tests.py
+drwxr-xr-x   0 soheilxi   (501) staff       (20)        0 2024-04-25 18:03:08.466261 LiveTune-0.0.8/
+-rw-r--r--   0 soheilxi   (501) staff       (20)     1808 2023-11-02 17:56:15.000000 LiveTune-0.0.8/LICENSE
+-rw-r--r--   0 soheilxi   (501) staff       (20)     7442 2024-04-25 18:03:08.466094 LiveTune-0.0.8/PKG-INFO
+-rw-r--r--   0 soheilxi   (501) staff       (20)     6733 2024-04-25 17:54:07.000000 LiveTune-0.0.8/README.md
+-rw-r--r--   0 soheilxi   (501) staff       (20)       38 2024-04-25 18:03:08.466312 LiveTune-0.0.8/setup.cfg
+-rw-r--r--   0 soheilxi   (501) staff       (20)     1049 2024-04-24 23:26:58.000000 LiveTune-0.0.8/setup.py
+drwxr-xr-x   0 soheilxi   (501) staff       (20)        0 2024-04-25 18:03:08.462659 LiveTune-0.0.8/src/
+drwxr-xr-x   0 soheilxi   (501) staff       (20)        0 2024-04-25 18:03:08.464157 LiveTune-0.0.8/src/LiveTune/
+-rw-r--r--   0 soheilxi   (501) staff       (20)     5995 2024-04-25 17:54:50.000000 LiveTune-0.0.8/src/LiveTune/LiveVariableBase.py
+-rw-r--r--   0 soheilxi   (501) staff       (20)      190 2023-09-11 17:39:09.000000 LiveTune-0.0.8/src/LiveTune/__init__.py
+-rw-r--r--   0 soheilxi   (501) staff       (20)     1689 2023-10-04 03:16:42.000000 LiveTune-0.0.8/src/LiveTune/liveTrigger.py
+-rwxr-xr-x   0 soheilxi   (501) staff       (20)     7152 2023-10-04 03:20:14.000000 LiveTune-0.0.8/src/LiveTune/liveVar.py
+drwxr-xr-x   0 soheilxi   (501) staff       (20)        0 2024-04-25 18:03:08.465411 LiveTune-0.0.8/src/LiveTune/tools/
+-rw-r--r--   0 soheilxi   (501) staff       (20)       42 2023-09-11 17:39:40.000000 LiveTune-0.0.8/src/LiveTune/tools/__init__.py
+-rw-r--r--   0 soheilxi   (501) staff       (20)     4062 2024-04-25 17:48:38.000000 LiveTune-0.0.8/src/LiveTune/tools/tune.py
+drwxr-xr-x   0 soheilxi   (501) staff       (20)        0 2024-04-25 18:03:08.464980 LiveTune-0.0.8/src/LiveTune.egg-info/
+-rw-r--r--   0 soheilxi   (501) staff       (20)     7442 2024-04-25 18:03:08.000000 LiveTune-0.0.8/src/LiveTune.egg-info/PKG-INFO
+-rw-r--r--   0 soheilxi   (501) staff       (20)      392 2024-04-25 18:03:08.000000 LiveTune-0.0.8/src/LiveTune.egg-info/SOURCES.txt
+-rw-r--r--   0 soheilxi   (501) staff       (20)        1 2024-04-25 18:03:08.000000 LiveTune-0.0.8/src/LiveTune.egg-info/dependency_links.txt
+-rw-r--r--   0 soheilxi   (501) staff       (20)       50 2024-04-25 18:03:08.000000 LiveTune-0.0.8/src/LiveTune.egg-info/entry_points.txt
+-rw-r--r--   0 soheilxi   (501) staff       (20)        9 2024-04-25 18:03:08.000000 LiveTune-0.0.8/src/LiveTune.egg-info/top_level.txt
+drwxr-xr-x   0 soheilxi   (501) staff       (20)        0 2024-04-25 18:03:08.465657 LiveTune-0.0.8/tests/
+-rw-r--r--   0 soheilxi   (501) staff       (20)    11225 2023-11-15 21:59:10.000000 LiveTune-0.0.8/tests/tests.py
```

### Comparing `LiveTune-0.0.7/LICENSE` & `LiveTune-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `LiveTune-0.0.7/PKG-INFO` & `LiveTune-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: LiveTune
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python package for ML developers and researchers to change certain variables while their code is executing to make the task of training a ML project easier. This package will allow you to tune some parameters while your code is live from outside of the program.
 Home-page: https://github.com/soheilzi/LiveTune
 Author: Soheil Zibakhsh Shabgahi, Aiden Tabrizi
 Author-email: szibakhshshabgahi@ucsd.edu, atabrizi@ucsd.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# LiveTune: Dynamic Parameter Tuning 🎶
+![LiveTune(Github)](https://github.com/soheilzi/LiveTune/assets/33820269/e87062c0-2d1c-4b23-a3a5-6eed7d07fa18)
+## Dynamic Parameter Tuning 🎶
 
 LiveTune is a cutting-edge Python package that empowers Machine Learning developers and researchers to adjust parameters in real-time while their program is running. Seamlessly modify variables, data, or hyperparameters, such as learning rate and regularizer, without interrupting your code execution. Experience the freedom to fine-tune your ML projects on-the-fly.
 
 ## Installation
 
 ### Platform Compatibility
 
@@ -27,15 +28,15 @@
 | Windows 🪟 | Not Yet Tested |
 
 ### Installation Guide
 
 1. Ensure you have PyPi installed. If not, [follow these instructions](https://packaging.python.org/en/latest/tutorials/installing-packages/).
 2. Execute the following command in your terminal:
 ```bash
-pip install -i https://test.pypi.org/simple/ LiveTune==0.0.7
+pip install LiveTune
 ```
 
 ## Key Features
 
 LiveTune offers two primary features: **Live Variables** and **Live Triggers**. Both are managed using our intuitive **tag system**.
 
 Upon starting a program that integrates LiveTune, the terminal will display the port number associated with that program instance.
@@ -179,8 +180,16 @@
 
 ### Contact
 If you are interested in using the code for commercial use, please contact [innovation@ucsd.edu](mailto:innovation@ucsd.edu)
 
 ## Thank you for using LiveTune!
 We're still early in testing, so please [fill out the feedback form if you find any bugs or have feature requests.](https://docs.google.com/forms/d/e/1FAIpQLSfHbM8Jy8w8EDZu_mEV0pH2qtqn3jplsB45KlmVsj6LORrBQQ/viewform?usp=sf_link)
 
-Thank you for using LiveTune! If it's been beneficial to your work, please consider citing our package in your publications. Your support helps us continue our efforts and assists others in discovering LiveTune. We appreciate your acknowledgment.
+Thank you for using LiveTune! If it's been beneficial to your work, please consider citing our paper in your publications. 
+```@article{shabgahi2023livetune,
+  title={LiveTune: Dynamic Parameter Tuning for Training Deep Neural Networks},
+  author={Shabgahi, Soheil Zibakhsh and Sheybani, Nojan and Tabrizi, Aiden and Koushanfar, Farinaz},
+  journal={arXiv preprint arXiv:2311.17279},
+  year={2023}
+}
+```
+Your support helps us continue our efforts and assists others in discovering LiveTune. We appreciate your acknowledgment.
```

### Comparing `LiveTune-0.0.7/README.md` & `LiveTune-0.0.8/src/LiveTune.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,23 @@
-# LiveTune: Dynamic Parameter Tuning 🎶
+Metadata-Version: 2.1
+Name: LiveTune
+Version: 0.0.8
+Summary: Python package for ML developers and researchers to change certain variables while their code is executing to make the task of training a ML project easier. This package will allow you to tune some parameters while your code is live from outside of the program.
+Home-page: https://github.com/soheilzi/LiveTune
+Author: Soheil Zibakhsh Shabgahi, Aiden Tabrizi
+Author-email: szibakhshshabgahi@ucsd.edu, atabrizi@ucsd.edu
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![LiveTune(Github)](https://github.com/soheilzi/LiveTune/assets/33820269/e87062c0-2d1c-4b23-a3a5-6eed7d07fa18)
+## Dynamic Parameter Tuning 🎶
 
 LiveTune is a cutting-edge Python package that empowers Machine Learning developers and researchers to adjust parameters in real-time while their program is running. Seamlessly modify variables, data, or hyperparameters, such as learning rate and regularizer, without interrupting your code execution. Experience the freedom to fine-tune your ML projects on-the-fly.
 
 ## Installation
 
 ### Platform Compatibility
 
@@ -13,15 +28,15 @@
 | Windows 🪟 | Not Yet Tested |
 
 ### Installation Guide
 
 1. Ensure you have PyPi installed. If not, [follow these instructions](https://packaging.python.org/en/latest/tutorials/installing-packages/).
 2. Execute the following command in your terminal:
 ```bash
-pip install -i https://test.pypi.org/simple/ LiveTune==0.0.7
+pip install LiveTune
 ```
 
 ## Key Features
 
 LiveTune offers two primary features: **Live Variables** and **Live Triggers**. Both are managed using our intuitive **tag system**.
 
 Upon starting a program that integrates LiveTune, the terminal will display the port number associated with that program instance.
@@ -165,8 +180,16 @@
 
 ### Contact
 If you are interested in using the code for commercial use, please contact [innovation@ucsd.edu](mailto:innovation@ucsd.edu)
 
 ## Thank you for using LiveTune!
 We're still early in testing, so please [fill out the feedback form if you find any bugs or have feature requests.](https://docs.google.com/forms/d/e/1FAIpQLSfHbM8Jy8w8EDZu_mEV0pH2qtqn3jplsB45KlmVsj6LORrBQQ/viewform?usp=sf_link)
 
-Thank you for using LiveTune! If it's been beneficial to your work, please consider citing our package in your publications. Your support helps us continue our efforts and assists others in discovering LiveTune. We appreciate your acknowledgment.
+Thank you for using LiveTune! If it's been beneficial to your work, please consider citing our paper in your publications. 
+```@article{shabgahi2023livetune,
+  title={LiveTune: Dynamic Parameter Tuning for Training Deep Neural Networks},
+  author={Shabgahi, Soheil Zibakhsh and Sheybani, Nojan and Tabrizi, Aiden and Koushanfar, Farinaz},
+  journal={arXiv preprint arXiv:2311.17279},
+  year={2023}
+}
+```
+Your support helps us continue our efforts and assists others in discovering LiveTune. We appreciate your acknowledgment.
```

### Comparing `LiveTune-0.0.7/setup.py` & `LiveTune-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="LiveTune",
-    version="0.0.7",
+    version="0.0.8",
     author="Soheil Zibakhsh Shabgahi, Aiden Tabrizi",
     author_email="szibakhshshabgahi@ucsd.edu, atabrizi@ucsd.edu",
     description="Python package for ML developers and researchers to change certain variables while their code is executing to make the task of training a ML project easier. This package will allow you to tune some parameters while your code is live from outside of the program.",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
```

### Comparing `LiveTune-0.0.7/src/LiveTune/LiveVariableBase.py` & `LiveTune-0.0.8/src/LiveTune/LiveVariableBase.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,17 +15,21 @@
     dictionary_port = []
     preferred_port = []
 
     def __init__(self, tag: str):
         if not isinstance(tag, str):
             raise TypeError("Tag must be a string.")
         
-        for instance in self.instances:
+        for i, instance in enumerate(self.instances):
             if instance.tag == tag:
-                raise Warning(f"{Color.RED}[WARN]{Color.END} {Color.YELLOW}{tag} already exists. Reusing tag names may have unintended consequences.{Color.END}")
+                # raise Warning(f"{Color.RED}[WARN]{Color.END} {Color.YELLOW}{tag} already exists. Reusing tag names may have unintended consequences.{Color.END}")
+                print(f"{Color.RED}[WARN]{Color.END} {Color.YELLOW}{tag} already exists. Reusing tag names may have unintended consequences.{Color.END}")
+                # del instance
+                self.instances.pop(i)
+                break
 
         if self.dictionary_port == []:
             sock = socket.socket()
             try:
                 sock.bind(('', 0 if self.preferred_port == [] else self.preferred_port[0]))
                 self.dictionary_port.append(sock.getsockname()[1])
                 print(f"{Color.BLUE}[LiveTune] {Color.GREEN}Port number for the LiveTune dictionary: {Color.YELLOW}{self.dictionary_port[0]}{Color.END}")
@@ -146,8 +150,11 @@
             while True:
                 connection, address = listenerSocket.accept()
 
                 client_thread = threading.Thread(target=self.handleClient, args=(connection,))
                 client_thread.daemon = True
                 client_thread.start()
         finally:
-            listenerSocket.close()
+            listenerSocket.close()
+
+    def get_dictionary_port(self):
+        return self.dictionary_port[0]
```

### Comparing `LiveTune-0.0.7/src/LiveTune/liveTrigger.py` & `LiveTune-0.0.8/src/LiveTune/liveTrigger.py`

 * *Files identical despite different names*

### Comparing `LiveTune-0.0.7/src/LiveTune/liveVar.py` & `LiveTune-0.0.8/src/LiveTune/liveVar.py`

 * *Files identical despite different names*

### Comparing `LiveTune-0.0.7/src/LiveTune/tools/tune.py` & `LiveTune-0.0.8/src/LiveTune/tools/tune.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
     try:
         client_socket.connect(('localhost', port))
         client_socket.send(f"request_type: dictionary_entry - {tag}".encode())
         response = client_socket.recv(1024).decode()
     except:
         print(f"{Color.RED}[ERROR]{Color.END} {Color.YELLOW}Failed to connect to the LiveTune dictionary. This is most likely because of an incorrect port.{Color.END}")
-        raise
+        exit(1)
     finally:
         client_socket.close()
 
     return int(response)
```

### Comparing `LiveTune-0.0.7/src/LiveTune.egg-info/PKG-INFO` & `LiveTune-0.0.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,9 @@
-Metadata-Version: 2.1
-Name: LiveTune
-Version: 0.0.7
-Summary: Python package for ML developers and researchers to change certain variables while their code is executing to make the task of training a ML project easier. This package will allow you to tune some parameters while your code is live from outside of the program.
-Home-page: https://github.com/soheilzi/LiveTune
-Author: Soheil Zibakhsh Shabgahi, Aiden Tabrizi
-Author-email: szibakhshshabgahi@ucsd.edu, atabrizi@ucsd.edu
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# LiveTune: Dynamic Parameter Tuning 🎶
+![LiveTune(Github)](https://github.com/soheilzi/LiveTune/assets/33820269/e87062c0-2d1c-4b23-a3a5-6eed7d07fa18)
+## Dynamic Parameter Tuning 🎶
 
 LiveTune is a cutting-edge Python package that empowers Machine Learning developers and researchers to adjust parameters in real-time while their program is running. Seamlessly modify variables, data, or hyperparameters, such as learning rate and regularizer, without interrupting your code execution. Experience the freedom to fine-tune your ML projects on-the-fly.
 
 ## Installation
 
 ### Platform Compatibility
 
@@ -27,15 +14,15 @@
 | Windows 🪟 | Not Yet Tested |
 
 ### Installation Guide
 
 1. Ensure you have PyPi installed. If not, [follow these instructions](https://packaging.python.org/en/latest/tutorials/installing-packages/).
 2. Execute the following command in your terminal:
 ```bash
-pip install -i https://test.pypi.org/simple/ LiveTune==0.0.7
+pip install LiveTune
 ```
 
 ## Key Features
 
 LiveTune offers two primary features: **Live Variables** and **Live Triggers**. Both are managed using our intuitive **tag system**.
 
 Upon starting a program that integrates LiveTune, the terminal will display the port number associated with that program instance.
@@ -179,8 +166,16 @@
 
 ### Contact
 If you are interested in using the code for commercial use, please contact [innovation@ucsd.edu](mailto:innovation@ucsd.edu)
 
 ## Thank you for using LiveTune!
 We're still early in testing, so please [fill out the feedback form if you find any bugs or have feature requests.](https://docs.google.com/forms/d/e/1FAIpQLSfHbM8Jy8w8EDZu_mEV0pH2qtqn3jplsB45KlmVsj6LORrBQQ/viewform?usp=sf_link)
 
-Thank you for using LiveTune! If it's been beneficial to your work, please consider citing our package in your publications. Your support helps us continue our efforts and assists others in discovering LiveTune. We appreciate your acknowledgment.
+Thank you for using LiveTune! If it's been beneficial to your work, please consider citing our paper in your publications. 
+```@article{shabgahi2023livetune,
+  title={LiveTune: Dynamic Parameter Tuning for Training Deep Neural Networks},
+  author={Shabgahi, Soheil Zibakhsh and Sheybani, Nojan and Tabrizi, Aiden and Koushanfar, Farinaz},
+  journal={arXiv preprint arXiv:2311.17279},
+  year={2023}
+}
+```
+Your support helps us continue our efforts and assists others in discovering LiveTune. We appreciate your acknowledgment.
```

### Comparing `LiveTune-0.0.7/tests/tests.py` & `LiveTune-0.0.8/tests/tests.py`

 * *Files identical despite different names*

