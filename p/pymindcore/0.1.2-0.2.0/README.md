# Comparing `tmp/pymindcore-0.1.2.tar.gz` & `tmp/pymindcore-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymindcore-0.1.2.tar", last modified: Fri Feb  9 05:58:19 2024, max compression
+gzip compressed data, was "pymindcore-0.2.0.tar", last modified: Thu Apr 25 02:53:04 2024, max compression
```

## Comparing `pymindcore-0.1.2.tar` & `pymindcore-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-02-09 05:58:19.103968 pymindcore-0.1.2/
--rw-rw-rw-   0        0        0      520 2023-11-17 04:55:51.000000 pymindcore-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     3080 2024-02-09 05:58:19.102966 pymindcore-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2511 2024-02-09 05:48:36.000000 pymindcore-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-02-09 05:58:19.095460 pymindcore-0.1.2/pymindcore/
--rw-rw-rw-   0        0        0       63 2023-11-17 05:24:52.000000 pymindcore-0.1.2/pymindcore/__init__.py
--rw-rw-rw-   0        0        0    34955 2024-02-09 05:56:40.000000 pymindcore-0.1.2/pymindcore/core.py
-drwxrwxrwx   0        0        0        0 2024-02-09 05:58:19.101464 pymindcore-0.1.2/pymindcore.egg-info/
--rw-rw-rw-   0        0        0     3080 2024-02-09 05:58:18.000000 pymindcore-0.1.2/pymindcore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-02-09 05:58:19.000000 pymindcore-0.1.2/pymindcore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-09 05:58:18.000000 pymindcore-0.1.2/pymindcore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-02-09 05:58:18.000000 pymindcore-0.1.2/pymindcore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-09 05:58:18.000000 pymindcore-0.1.2/pymindcore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-09 05:58:19.104467 pymindcore-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      817 2024-02-09 05:49:01.000000 pymindcore-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 02:53:04.345626 pymindcore-0.2.0/
+-rw-rw-rw-   0        0        0      520 2023-11-17 04:55:51.000000 pymindcore-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3187 2024-04-25 02:53:04.344125 pymindcore-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2598 2024-04-25 02:48:39.000000 pymindcore-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 02:53:04.335618 pymindcore-0.2.0/pymindcore/
+-rw-rw-rw-   0        0        0    44585 2024-04-25 02:43:15.000000 pymindcore-0.2.0/pymindcore/core.py
+drwxrwxrwx   0        0        0        0 2024-04-25 02:53:04.342124 pymindcore-0.2.0/pymindcore.egg-info/
+-rw-rw-rw-   0        0        0     3187 2024-04-25 02:53:04.000000 pymindcore-0.2.0/pymindcore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2024-04-25 02:53:04.000000 pymindcore-0.2.0/pymindcore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 02:53:04.000000 pymindcore-0.2.0/pymindcore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-25 02:53:04.000000 pymindcore-0.2.0/pymindcore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 02:53:04.000000 pymindcore-0.2.0/pymindcore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 02:53:04.345626 pymindcore-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      766 2024-04-25 02:39:26.000000 pymindcore-0.2.0/setup.py
```

### Comparing `pymindcore-0.1.2/LICENSE` & `pymindcore-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymindcore-0.1.2/PKG-INFO` & `pymindcore-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: pymindcore
-Version: 0.1.2
+Version: 0.2.0
 Summary: A Python library for AI, easy to use, freely available for any use
 Home-page: https://github.com/Dogz-R-Godz/Pymind
 Author: Dogz R Godz
 Author-email: doggocam01@gmail.com
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: Pillow
-Requires-Dist: idx2numpy
+Requires-Dist: numexpr
+Requires-Dist: numba
 
-# Pymind
+# Pymindcore
 
 Pymind is a Python library for AI, supporting Numpy.
 
 ## Installation
 
-You can install Pymind using pip: pip install pymind.
+You can install Pymind using pip: pip install pymindcore.
 
 ## Usage
 
 You import it, you call the class with your neural network size, and you're away! There will be actual test files in the future, but for the meantime,
 
 ## License
 
@@ -48,7 +49,11 @@
     1: Go into the game you want to train an AI for, and think what points you would punish the AI for getting wrong. eg: dying, losing, etc.
     2: Play a game, and do one of each of those things yourself, screenshotting the whole screen each time you do one.
     3: Go into the screenshot in an app like ms paint, and find a pixel that is a certain colour when you did each of the bad things. (must be unique, and not trigger when either of the others happen)
     4: Go into line 199 of VideoGameAI.py, and add in your coordinates and the pixel colour of that coordinate (in RGB). I'd recommend using Gimp for it. It should extend down to line 207. Only change the rewards if you know what you are doing.
     4.5: If you have more than 3 punishment options, then you should copy one of them, and paste it below it, copy the __Coords, __RGB, and __Punishment, and paste them below as well.
     5: Figure out what keybinds your AI will need to have for the game. The ones set up for Minecraft should cover most bases, but to be safe, double check. If you want to, remove all the keybinds that your AI will not need, so it can learn easier.
     6: Run it and it should work!
+
+## Discord server
+
+Join the discord server https://discord.gg/MSMzmJ6ffj!
```

### Comparing `pymindcore-0.1.2/README.md` & `pymindcore-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# Pymind
+# Pymindcore
 
 Pymind is a Python library for AI, supporting Numpy.
 
 ## Installation
 
-You can install Pymind using pip: pip install pymind.
+You can install Pymind using pip: pip install pymindcore.
 
 ## Usage
 
 You import it, you call the class with your neural network size, and you're away! There will be actual test files in the future, but for the meantime,
 
 ## License
 
@@ -31,8 +31,12 @@
 To make it work on a different game:
     1: Go into the game you want to train an AI for, and think what points you would punish the AI for getting wrong. eg: dying, losing, etc.
     2: Play a game, and do one of each of those things yourself, screenshotting the whole screen each time you do one.
     3: Go into the screenshot in an app like ms paint, and find a pixel that is a certain colour when you did each of the bad things. (must be unique, and not trigger when either of the others happen)
     4: Go into line 199 of VideoGameAI.py, and add in your coordinates and the pixel colour of that coordinate (in RGB). I'd recommend using Gimp for it. It should extend down to line 207. Only change the rewards if you know what you are doing.
     4.5: If you have more than 3 punishment options, then you should copy one of them, and paste it below it, copy the __Coords, __RGB, and __Punishment, and paste them below as well.
     5: Figure out what keybinds your AI will need to have for the game. The ones set up for Minecraft should cover most bases, but to be safe, double check. If you want to, remove all the keybinds that your AI will not need, so it can learn easier.
-    6: Run it and it should work!
+    6: Run it and it should work!
+
+## Discord server
+
+Join the discord server https://discord.gg/MSMzmJ6ffj!
```

### Comparing `pymindcore-0.1.2/pymindcore/core.py` & `pymindcore-0.2.0/pymindcore/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,279 +1,505 @@
 import numpy as np
 import time 
 import math as maths
-import math
-import time
-import numpy as np2
 from time import perf_counter
-#from discord_webhook import DiscordWebhook
+import numexpr as ne
+from numba import jit
+from .errors import *
 
-class Optomised_neural_network:
-    def __init__(self, input_neurons, hidden_layers, output_neurons, activation="relu",random_init=True,tanh_output=False,clip_amount=1,float_type=np.float64):
-        ###random_init can be "Mean", True, or False
+
+
+@jit(nopython=True)
+def relu(x, speedy=True):
+    if speedy: pass#return ne.evaluate("where(x > 0, x, 0.01 * x)")
+    return np.maximum(0.01*x, x)
+@jit(nopython=True)
+def relu_prime(x, speedy=True):
+    if speedy: pass#return ne.evaluate("where(x > 0, 1, 0.01)")
+    return np.where(x > 0, 1, 0.01)
+@jit(nopython=True)
+def inv_relu(x, speedy=True):
+    if speedy: pass#return ne.evaluate("where(x > 0, x, 100 * x)")
+    return x #np.where(x > 0, x, 100 * x)
+@jit(nopython=True)
+def sigmoid(x, speedy=True):
+    if speedy: pass#return ne.evaluate("(1 / (1 + exp(-x)))")
+    return (1 / (1 + np.exp(-x)))
+@jit(nopython=True)
+def sigmoid_prime(x, speedy=True):
+    if speedy: pass#return ne.evaluate("(x * (1 - x))")
+    return x * (1 - x)
+@jit(nopython=True)
+def inv_sigmoid(x, speedy=True):
+    x=np.clip(x, 0.0001, 0.9999)
+    if speedy: pass#return ne.evaluate("log(x/(1 - x))")
+    return np.log(x/(1-x))
+@jit(nopython=True)
+def tanh(x, speedy=True):
+    if speedy: pass#return ne.evaluate("tanh(x)")
+    return np.tanh(x)
+@jit(nopython=True)
+def tanh_prime(x, speedy=True):
+    if speedy: pass#return ne.evaluate("(1 - tanh(x)**2)")
+    return (1 - np.tanh(x)**2)
+@jit(nopython=True)
+def inv_tanh(x, speedy=True):
+    x=np.clip(x, -0.9999, 0.9999)
+    if speedy: pass#return ne.evaluate("arctanh(x)")
+    return np.arctanh(x)
+
+@jit(nopython=True)
+def matrixMultiply(aNegative1:np.ndarray, weightsI:np.ndarray):
+    return aNegative1 @ weightsI
+
+@jit(nopython=True)
+def matrixMultiplyWithB(aNegative1:np.ndarray, weightsI:np.ndarray, biasesI:np.ndarray):
+    return aNegative1 @ weightsI + biasesI
+
+class Optomised_neural_network: 
+    def __init__(self, input_neurons, hidden_layers, output_neurons, activation="relu", output_activation="sig",random_init=True,clip_amount=1, usingPlugin=False, **pluginSettings):
+        
         self.layers = [input_neurons] + hidden_layers + [output_neurons]
         self.weights = []
         self.biases = []
-        self.tanh_output=tanh_output
         self.clip_amount=clip_amount
-        self.float_type=float_type
+        self.float_type=np.float64
+        self.pluginSettings=pluginSettings
+        self.activationName=activation
+        self.outputActivationName=output_activation
+        self.version=2.0
+        self.usingPlugin=usingPlugin
+        
+        
+        self.matrixMultiply=self.matrixMultiplyf
+
+        
+        self.init_weights=self.init_weightsf
+        self.relu2=self.reluf
+        self.relu_prime2=self.relu_primef
+        self.inv_relu2=self.inv_reluf
+        self.sigmoid2=self.sigmoidf
+        self.sigmoid_prime2=self.sigmoid_primef
+        self.inv_sigmoid2=self.inv_sigmoidf
+        self.tanh2=self.tanhf
+        self.tanh_prime2=self.tanh_primef
+        self.inv_tanh2=self.inv_tanhf
+
+
+        self.save_to_file=self.save_to_filef
+        self.save_to_array=self.save_to_arrayf
+        self.load_from_file=self.load_from_filef
+        self.load_from_array=self.load_from_arrayf
+        self.forward=self.forwardf
+        self.compute_loss=self.compute_lossf
+        self.find_error=self.find_errorf
+        self.backward=self.backwardf
+        self.train=self.trainf    
+
+        self.init_weights(random_init)
+        self.setActivFunctions=self.setActivFunctionsf
+        self.setActivFunctions()
+
+        self.idfkanymore=False
+
+        
+    def setActivFunctionsf(self):
+        # Set activation function
+        if self.activationName == "relu":
+            self.activation = self.relu2
+            self.activation_prime = self.relu_prime2
+        elif self.activationName == "sig":
+            self.activation = self.sigmoid2
+            self.activation_prime = self.sigmoid_prime2
+        elif self.activationName == "tanh":
+            self.activation = self.tanh2
+            self.activation_prime = self.tanh_prime2
+        else:
+            if not self.usingPlugin:
+                raise invalidActivationError(self.activationName)
         
-        if random_init == "Mean":
+        if self.outputActivationName == "relu":
+            self.output_activation = self.relu2
+            self.inv_output_activation = self.inv_relu2
+        elif self.outputActivationName == "sig":
+            self.output_activation = self.sigmoid2
+            self.inv_output_activation = self.inv_sigmoid2
+        elif self.outputActivationName == "tanh":
+            self.output_activation = self.tanh2
+            self.inv_output_activation = self.inv_tanh2
+        else:
+            if not self.usingPlugin:
+                raise invalidOutputActivationError(self.outputActivationName)
+            
+        
+    
+
+
+
+    def reluf(self, x, speedy=True):
+        return relu(x, speedy)
+    
+    def relu_primef(self, x, speedy=True):
+        return relu_prime(x, speedy)
+    
+    def inv_reluf(self, x, speedy=True):
+        return inv_relu(x, speedy)
+    
+    def sigmoidf(self, x, speedy=True):
+        return sigmoid(x, speedy)
+    
+    def sigmoid_primef(self, x, speedy=True):
+        return sigmoid_prime(x, speedy)
+    
+    def inv_sigmoidf(self, x, speedy=True):
+        return inv_sigmoid(x, speedy)
+    
+    def tanhf(self, x, speedy=True):
+        return tanh(x, speedy)
+    
+    def tanh_primef(self, x, speedy=True):
+        return tanh_prime(x, speedy)
+    
+    def inv_tanhf(self, x, speedy=True):
+        return inv_tanh(x, speedy)
+
+    def matrixMultiplyf(self, a, w):
+        return matrixMultiply(a, w)
+    
+
+    def init_weightsf(self,random_init="mean"):
+        if random_init == "mean":
             for i in range(len(self.layers) - 1):
-                self.weights.append(np.random.randn(self.layers[i], self.layers[i + 1]).astype(float_type))
-                self.biases.append(np.random.randn(self.layers[i + 1]).astype(float_type))
+                print(f"Starting layer {i}")
+                self.weights.append(np.random.randn(self.layers[i], self.layers[i + 1]).astype(self.float_type)*self.clip_amount)
+                print("Make weights, doing biases now")
+                self.biases.append(np.random.randn(self.layers[i + 1]).astype(self.float_type)*self.clip_amount)
+                print(f"Done layer {i}")
             
         elif random_init:
             for i in range(len(self.layers) - 1):
-                self.weights.append(np.random.uniform(-1,1,(self.layers[i], self.layers[i + 1])).astype(float_type))
-                self.biases.append(np.random.uniform(-1,1,self.layers[i + 1]).astype(float_type))
+                self.weights.append(np.random.uniform(-1,1,(self.layers[i], self.layers[i + 1])).astype(self.float_type)*self.clip_amount)
+                self.biases.append(np.random.uniform(-1,1,self.layers[i + 1]).astype(self.float_type)*self.clip_amount)
         else:
             for i in range(len(self.layers) - 1):
-                self.weights.append(np.zeros((self.layers[i], self.layers[i + 1])).astype(float_type))
-                self.biases.append(np.zeros(self.layers[i + 1]).astype(float_type))
-        
-        
-        # Set activation function
-        if activation == "relu":
-            self.activation = self.relu
-            self.activation_prime = self.relu_prime
-        elif activation == "sig":
-            self.activation = self.sigmoid
-            self.activation_prime = self.sigmoid_prime
-        elif activation == "tanh":
-            self.activation = self.tanh
-            self.activation_prime = self.tanh_prime
-
-    def relu(self, x):
-        return np.maximum(0.01*x, x)
-    
-    def relu_prime(self, x):
-        return np.where(x > 0, 1, 0.01)
-    
-    def sigmoid(self, x):
-        return 1 / (1 + np.exp(-x))
-    
-    def sigmoid_prime(self, x):
-        return x * (1 - x)
-
-    def tanh(self, x):
-        return np.tanh(x)
-    def tanh_prime(self, x):
-        return 1 - np.tanh(x)**2
-
-    def save_to_file(self, filename):
-        # Check if self.weights and self.biases are already numpy arrays or lists of arrays
-
-        # Ensure weights and biases are lists of arrays
-        weights_list = [self.weights] if isinstance(self.weights, np.ndarray) else [np.array(w) for w in self.weights]
-        biases_list = [self.biases] if isinstance(self.biases, np.ndarray) else [np.array(b) for b in self.biases]
-
-
-        # Convert the lists to an object array
+                self.weights.append(np.zeros((self.layers[i], self.layers[i + 1])).astype(self.float_type)*self.clip_amount)
+                self.biases.append(np.zeros(self.layers[i + 1]).astype(self.float_type)*self.clip_amount)
+    
+     
+    def save_to_filef(self, filename):
         try:
-            weights_numpy = np.array(weights_list, dtype=object)
-            biases_numpy = np.array(biases_list, dtype=object)
-        except Exception as e:
-            print("Error in creating object arrays:", e)
-            raise
+            try:
+                weights_numpy = np.array(self.weights,dtype=object) #np.array([self.weights[i].T for i in range(len(self.weights))],dtype=object)
+                biases_numpy = np.array(self.biases,dtype=object)
+                
 
-        # Print shapes and contents of the object arrays
+                # Now create the NumPy array to bundle the data
+                wShape=np.array([self.weights[w].shape for w in range(len(self.weights))])
+                bShape=np.array([self.biases[b].shape for b in range(len(self.biases))])
+                data = np.array([weights_numpy, biases_numpy, np.array([1]), wShape, bShape, self.activationName, self.outputActivationName, self.clip_amount], dtype=object)
+
+                # Save the data using NumPy's save method
+                #np.save(f"{filename}_weights", weights_numpy)
+                #np.save(f"{filename}_biases",biases_numpy)
+                np.save(filename,data)
+            except:
+                weights_numpy = np.array([self.weights[i].T for i in range(len(self.weights))],dtype=object)
+                biases_numpy = np.array(self.biases,dtype=object)
+
+                # Now create the NumPy array to bundle the data
+                wShape=np.array([self.weights[w].shape for w in range(len(self.weights))])
+                bShape=np.array([self.biases[b].shape for b in range(len(self.biases))])
+                data = np.array([weights_numpy, biases_numpy, np.array([0]), wShape, bShape, self.activationName, self.outputActivationName, self.clip_amount], dtype=object)
+
+                # Save the data using NumPy's save method
+                #np.save(f"{filename}_weights", weights_numpy)
+                #np.save(f"{filename}_biases",biases_numpy)
+                np.save(filename,data)
+        except:
+            raise howDoYouFuckUpSavingError
 
-        # Bundle the data
+    def save_to_arrayf(self):
         try:
-            # Directly create an array of objects, each being a list containing one array
-            data = np.array([weights_numpy.tolist(), biases_numpy.tolist()], dtype=object)
-        except Exception as e:
-            print("Error in bundling data without broadcasting:", e)
-            raise
-
-        # Print final data array shape and contents
-
-        # Save the data
-        np.save(filename, data)
-        print("Saved the data")
+            try:
+                weights_numpy = np.array(self.weights,dtype=object) #np.array([self.weights[i].T for i in range(len(self.weights))],dtype=object)
+                biases_numpy = np.array(self.biases,dtype=object)
+                
+
+                # Now create the NumPy array to bundle the data
+                wShape=np.array([self.weights[w].shape for w in range(len(self.weights))])
+                bShape=np.array([self.biases[b].shape for b in range(len(self.biases))])
+                data = np.array([weights_numpy, biases_numpy, np.array([1]), wShape, bShape, self.activationName, self.outputActivationName, self.clip_amount], dtype=object)
+
+                # Save the data using NumPy's save method
+                #np.save(f"{filename}_weights", weights_numpy)
+                #np.save(f"{filename}_biases",biases_numpy)
+            except:
+                weights_numpy = np.array([self.weights[i].T for i in range(len(self.weights))],dtype=object)
+                biases_numpy = np.array(self.biases,dtype=object)
+
+                # Now create the NumPy array to bundle the data
+                wShape=np.array([self.weights[w].shape for w in range(len(self.weights))])
+                bShape=np.array([self.biases[b].shape for b in range(len(self.biases))])
+                data = np.array([weights_numpy, biases_numpy, np.array([0]), wShape, bShape, self.activationName, self.outputActivationName, self.clip_amount], dtype=object)
+
+                # Save the data using NumPy's save method
+                #np.save(f"{filename}_weights", weights_numpy)
+                #np.save(f"{filename}_biases",biases_numpy)
+        except:
+            raise howDoYouFuckUpSavingError
+        return data
     
-    def load_from_file(self, filename):
+    def load_from_filef(self, filename):
         # Load the data using NumPy's load method
         data = np.load(filename, allow_pickle=True)
 
         # Convert the loaded NumPy arrays back to CuPy arrays and set to self.weights and self.biases
-        self.weights = [np.array(arr) for arr in data[0]]
+        try:
+            if data[2]==0:
+                self.weights = [np.array(arr.T) for arr in data[0]]
+            else:
+                self.weights = [np.array(arr) for arr in data[0]]
+
+            weightShape=data[3]
+            biasShape=data[4]
+        except KeyError:
+            raise corruptedOrOldSaveFileError
+
+
+            
         self.biases = [np.array(arr) for arr in data[1]]
+        self.activationName=data[5]
+        self.outputActivationName=data[6]
+        self.clip_amount=data[7]
+
+
+        wShape=np.array([self.weights[w].shape for w in range(len(self.weights))], dtype=object)
+        bShape=np.array([self.biases[b].shape for b in range(len(self.biases))], dtype=object)
+
+        if (wShape != weightShape).any() or (bShape != biasShape).any():
+            raise invalidSaveNetworkShapeError
+
+        print("Successfully loaded from file")
     
-    def forward(self, x, tanh_output=False, verbose=False):
-        #self.a = [x]
-        for i in range(len(self.weights) - 1):
-            #curr_weights=self.weights[i].copy()
-            #curr_weights=np.stack(curr_weights,self.a[-1].size)
+    def load_from_arrayf(self, data):
+        try:
+            if data[2]==0:
+                self.weights = [np.array(arr.T) for arr in data[0]]
+            else:
+                self.weights = [np.array(arr) for arr in data[0]]
+
+            weightShape=data[3]
+            biasShape=data[4]
+        except KeyError:
+            raise corruptedOrOldSaveFileError
+
+
+            
+        self.biases = [np.array(arr) for arr in data[1]]
+        self.activationName=data[5]
+        self.outputActivationName=data[6]
+        self.clip_amount=data[7]
 
-            z = self.a[-1] @ self.weights[i] + self.biases[i]
+
+        wShape=np.array([self.weights[w].shape for w in range(len(self.weights))], dtype=object)
+        bShape=np.array([self.biases[b].shape for b in range(len(self.biases))], dtype=object)
+
+        if (wShape != weightShape).any() or (bShape != biasShape).any():
+            raise invalidSaveNetworkShapeError
+
+        print("Successfully loaded from file")
+        
+     
+    def forwardf(self, x, verbose=False, memory_efficent=False):
+        
+        """memory_efficent makes it delete the inputs layer from RAM after its finished with it."""
+        if type(x)==np.ndarray:
+            self.a = [x]
+        #if verbose:print("Made self.a [x]")
+        for i in range(len(self.weights) - 1):
+            z = self.matrixMultiply(self.a[-1], self.weights[i]) + self.biases[i]
+            #z = self.a[-1] @ self.weights[i] + self.biases[i]
+            #z = ne.evaluate("z + b", {'z': self.a[-1] @ self.weights[i], 'b': self.biases[i]})
             if verbose:print("Calculated the stuff")
-            self.a.append(self.activation(z))
+            #self.a[-1].
+            self.a.append(self.activation(z)) #activation is faster with Evaluate
             if verbose:print(f"Done layer {i} out of {len(self.weights) - 1}")
-        z_out = self.a[-1] @ self.weights[-1] + self.biases[-1]
-        if tanh_output:self.a.append(self.tanh(z_out))
-        else:self.a.append(self.sigmoid(z_out))
-        
-        return self.a[-1]
-    
-    def compute_loss(self, y):
+            if i == 0:
+                if memory_efficent:del self.a[0]
+        #z_out = self.a[-1] @ self.weights[-1] + self.biases[-1]
+        #z_out = matrixMultiply(self.a[-1], self.weights[-1], self.biases[-1])
+        z_out = self.matrixMultiply(self.a[-1], self.weights[-1]) + self.biases[-1]
+        #print("Mat Mulled")
+        #z_out = ne.evaluate("z + b", {'z': self.a[-1] @ self.weights[-1], 'b': self.biases[-1]})
+        #self.pll=self.a[-1].shape[1]
+        self.a.append(self.output_activation(z_out))
+        return self.a[-1] 
+    def compute_lossf(self, y):
         m = y.shape[0]
-        eachStateError=(self.a[-1] - y) ** 2
+        eachStateError=ne.evaluate("(a - y) ** 2", {'a': self.a[-1], 'y': y})
         return np.sum(eachStateError)/m #(1 / (2 * m)) * 
-
-    def find_error(self, x, y, verbose=False):
+    def find_errorf(self, x, y, verbose=False):
         # Compute predictions for the given input states
         self.a=[x]
-        predictions = self.forward(None,self.tanh_output,verbose) #x
-        if verbose:
-            print("Done forward pass")
+        predictions = self.forward(None,verbose) #x
+        if verbose:print("Done forward pass")
         # Compute the error for each sample and sum them up
         differences=(predictions - y)
         if verbose:print("Found differences")
         squared=np.sum(differences ** 2)
         if verbose:print("Squared all the differences")
         total_error = squared/len(x)
         if verbose:print("Found total error")
         return total_error
-    
-    def backward(self, x, y, learning_rate=0.1, reduceDeriv=False):
+    def backwardf(self, x, y, learning_rate=0.1, reduceDeriv=False, verbose=False):
         m = self.a[0].shape[0]
-        self.dz = [-(y - self.a[-1]) / m]
+        self.pll=self.a[0].shape[1]
+        y2=self.inv_output_activation(y)
+        self.dz = [ne.evaluate("-(y - a) / m", {'y': self.inv_output_activation(y), 'a': self.inv_output_activation(self.a[-1]), 'm': m})]
+
+        if 1 in np.isinf(y2):
+            raise asianParentsExpectationsError
+
         for i in reversed(range(len(self.weights))):
+            if verbose: print(f"Doing the funny on layer {i}")
 
-            dw = self.a[i].T @ self.dz[-1]
+            #self.dw = self.a[i].T @ self.dz[-1]
+            self.dw = self.matrixMultiply(self.a[i].T, self.dz[-1]) #.T
             #print("Matrixed the shit out of these weights")
             db = np.sum(self.dz[-1], axis=0)
             #print("About to do funny things to the weights")
-            self.weights[i] -= learning_rate * dw
-            self.biases[i] -= learning_rate * db
+
+            #weights2 = ne.evaluate("w - lr * dw", {'w': self.weights[i], 'lr': learning_rate, 'dw': self.dw})
+            #biases2 = ne.evaluate("b - lr * db2", {'b': self.biases[i], 'lr': learning_rate, 'db2': db})
+
+
+            self.weights[i] = self.weights[i] - learning_rate * self.dw
+            self.biases[i] = self.biases[i] - learning_rate * db
+
+
+
+            self.pll=self.a[i].shape[1]
             #print("About to do funny things to the derivs")
             if i != 0:
                 if reduceDeriv:
-                    act=self.activation_prime(self.a[i])
-                    dz_next = ((self.dz[-1] @ self.weights[i].T)/(0.5*(10**i))) * act
+                    if self.idfkanymore:
+                        weightsNew=self.weights[i].T # self.weights[i].T.reshape(self.weights[i].T.shape[0]*self.weights[i].T.shape[1], self.weights[i].T.shape[2])
+                    else:
+                        weightsNew=self.weights[i].T
+                    #dz_next = ne.evaluate("(d/(0.5*(10**i2))) * act2", {'d': self.dz[-1] @ self.weights[i].T, 'i2': i, 'act2': self.activation_prime(self.a[i])})
+                    dz_next = ((self.dz[-1] @ weightsNew)/(0.5*(10**i))) * self.activation_prime(self.a[i])
                     self.dz.append(dz_next)
                 else:
-                    dz_next = self.dz[-1] @ self.weights[i].T * self.activation_prime(self.a[i])
+                    #dz_next = ne.evaluate("d * a", {'d': self.dz[-1] @ self.weights[i].T, 'a': self.activation_prime(self.a[i])})
+                    dz_next = (self.dz[-1] @ self.weights[i].T) * self.activation_prime(self.a[i])
                     self.dz.append(dz_next)
-            #print(f"Derived layer {i}/{len(self.weights)}")
-                
-    def train(self, x, y, epochs=10000, learning_rate=0.01, optimizer=None, beta1=0.9, beta2=0.999, epsilon=1e-8, print_=False): #ping_webhook_URL=None,
-        if optimizer == "ADAM":
+        #pr.disable()
+        #pr.print_stats()
+            #print(f"Derived layer {i}/{len(self.weights)}") 
+     
+    def ADAM(self, verbose=False):
+        for i in range(len(self.weights)):
+            if verbose:print(f"Gradienting layer {i}")
+            # Compute gradients for weights and biases
+            grad_w = self.matrixMultiply(self.a[i].T, self.dz[-(i+1)])
+            #grad_w = self.a[i].T @ self.dz[-(i+1)]
+            grad_b = np.sum(self.dz[-(i+1)], axis=0)
+            
+            # Update first moment for weights and biases
+            self.m_weights[i] = self.beta1 * self.m_weights[i] + (1 - self.beta1) * grad_w
+            self.m_biases[i] = self.beta1 * self.m_biases[i] + (1 - self.beta1) * grad_b
+            
+            # Update second moment for weights and biases
+            self.v_weights[i] = self.beta2 * self.v_weights[i] + (1 - self.beta2) * grad_w ** 2
+            self.v_biases[i] = self.beta2 * self.v_biases[i] + (1 - self.beta2) * grad_b ** 2
+            
+            # Bias-corrected moments
+            m_weights_corr = self.m_weights[i] / (1 - self.beta1**self.t)
+            m_biases_corr = self.m_biases[i] / (1 - self.beta1**self.t)
+            v_weights_corr = self.v_weights[i] / (1 - self.beta2**self.t)
+            v_biases_corr = self.v_biases[i] / (1 - self.beta2**self.t)
+            
+            # Update weights and biases
+            self.weights[i] -= self.learning_rate * m_weights_corr / (np.sqrt(v_weights_corr) + self.epsilon)
+            self.biases[i] -= self.learning_rate * m_biases_corr / (np.sqrt(v_biases_corr) + self.epsilon)
+
+        # Fix the clipping issue by iterating through each array in the lists
+        for i in range(len(self.weights)):
+            if verbose:print(f"Clipping layer {i}")
+            self.weights[i] = np.clip(self.weights[i], -self.clip_amount, self.clip_amount)
+            self.biases[i] = np.clip(self.biases[i], -self.clip_amount, self.clip_amount)
+
+
+
+    def trainf(self, x, y, epochs=10000, learning_rate=0.01, optimizer=None, beta1=0.9, beta2=0.999, epsilon=1e-8, print_=False, resetADAMVars=True): #ping_webhook_URL=None,
+        if optimizer == "ADAM" and resetADAMVars:
             # Initialize Adam-specific variables
-            m_weights = [np.zeros_like(w) for w in self.weights]
-            v_weights = [np.zeros_like(w) for w in self.weights]
-            m_biases = [np.zeros_like(b) for b in self.biases]
-            v_biases = [np.zeros_like(b) for b in self.biases]
-            t = 0
+            self.m_weights = [np.zeros_like(w) for w in self.weights]
+            self.v_weights = [np.zeros_like(w) for w in self.weights]
+            self.m_biases = [np.zeros_like(b) for b in self.biases]
+            self.v_biases = [np.zeros_like(b) for b in self.biases]
+            self.t = 0
+        self.beta1=beta1
+        self.beta2=beta2
+        self.epsilon=epsilon
+        self.learning_rate=learning_rate
         totalTime=0
-        prevError=99999999
+        #self.a=[x]
+        #print("Doing first forward")
+        #self.forward(None)
+        #print("Done")
+        #error=self.compute_loss(y)
+        prevError=9999
+        #print(f"Starting error is {error}")
         for epoch in range(epochs):
-            startingTime=time.time()
             self.a=[x]
-            #print("Starting forward")
-            #start = perf_counter()
-            self.forward(None,self.tanh_output)
+            if print_:print("Starting forward")
+            self.forward(None, print_)
             #end = perf_counter()
             #print(f"Computed forward in {end-start} seconds")
             #start = perf_counter()
-            self.backward(None, y, learning_rate)
-            #end = perf_counter()
-            #print(f"Computed backward in {end-start} seconds")
+            if print_:print("Starting backward")
+            self.backward(None, y, learning_rate,True, print_)
             
+            if print_:print("Starting the gradienting")
             if optimizer == "ADAM":
-                t += 1
-                for i in range(len(self.weights)):
-                    # Compute gradients for weights and biases
-                    grad_w = self.a[i].T @ self.dz[-(i+1)]
-                    grad_b = np.sum(self.dz[-(i+1)], axis=0)
-                    
-                    # Update first moment for weights and biases
-                    m_weights[i] = beta1 * m_weights[i] + (1 - beta1) * grad_w
-                    m_biases[i] = beta1 * m_biases[i] + (1 - beta1) * grad_b
-                    
-                    # Update second moment for weights and biases
-                    v_weights[i] = beta2 * v_weights[i] + (1 - beta2) * grad_w ** 2
-                    v_biases[i] = beta2 * v_biases[i] + (1 - beta2) * grad_b ** 2
-                    
-                    # Bias-corrected moments
-                    m_weights_corr = m_weights[i] / (1 - beta1**t)
-                    m_biases_corr = m_biases[i] / (1 - beta1**t)
-                    v_weights_corr = v_weights[i] / (1 - beta2**t)
-                    v_biases_corr = v_biases[i] / (1 - beta2**t)
-                    
-                    # Update weights and biases
-                    self.weights[i] -= learning_rate * m_weights_corr / (np.sqrt(v_weights_corr) + epsilon)
-                    self.biases[i] -= learning_rate * m_biases_corr / (np.sqrt(v_biases_corr) + epsilon)
-
-                # Fix the clipping issue by iterating through each array in the lists
-                for i in range(len(self.weights)):
-                    self.weights[i] = np.clip(self.weights[i], -self.clip_amount, self.clip_amount)
-                    self.biases[i] = np.clip(self.biases[i], -self.clip_amount, self.clip_amount)
+                self.t += 1
+                self.ADAM(print_)
+                
             else:
                 #print("Gradient decenting")
                 # Standard gradient descent
                 for i in range(len(self.weights)):
-                    self.weights[i] -= learning_rate * self.a[i].T @ self.dz[-(i+1)]
-                    self.biases[i] -= learning_rate * np.sum(self.dz[-(i+1)], axis=0)
+                    self.weights[i] = ne.evaluate("w - lr * adz", {'w': self.weights[i], 'lr': learning_rate, 'adz': self.matrixMultiply(self.a[i].T, self.dz[-(i+1)])})
+                    self.biases[i] = ne.evaluate("b - lr * sumdz", {'b': self.biases[i], 'lr': learning_rate, 'sumdz': np.sum(self.dz[-(i+1)], axis=0)})
                 for i in range(len(self.weights)):
                     self.weights[i] = np.clip(self.weights[i], -self.clip_amount, self.clip_amount)
                     self.biases[i] = np.clip(self.biases[i], -self.clip_amount, self.clip_amount)
             
-            if epoch % math.ceil(epochs/100) == 0:
-                #self.a=[x]
-                #self.forward(None,verbose=True)
-                #error=self.compute_loss(y)
-                #print(f"Epoch {epoch}/{epochs}. Error change: {prevError-error:.6f}. New error is {error:.6f}")
-                #prevError=error
-                
-                #if ping_webhook_URL != None:
-
-                '''original_noise=np.random.uniform(0,255,self.layers[0])
+            if epoch % maths.ceil(epochs/50) == 0 and epoch != 0:
+                for layer in range(len(self.weights)):
+                    x
+            if True: #print_
+                if epoch % maths.ceil(epochs/50) == 0 and epoch != 0:end = perf_counter()
+                if epoch % maths.ceil(epochs/50) == 0 and epoch != 0:print(f"Computed everything in {end-start} seconds. Epoch number {epoch}")
+                if epoch % maths.ceil(epochs/50) == 0:
+                    self.a=[x]
+                    self.forward(None)
+                    error=self.compute_loss(y)
+                    print(f"Epoch {epoch}/{epochs}. Error change: {prevError-error:.10f}. New error is {error:.10f}")
+                    prevError=error
+                    start = perf_counter()
                     
-                    noise=original_noise.copy()
-                    noise3=original_noise.copy()
-                    noise3=noise3.reshape(50,50,3)
-                    noise3=noise3.get()
-                    original_noise=original_noise.get()
-                    img = Image.fromarray(noise3.astype('uint8'), "RGB")  # Ensure the data type is uint8 for image
-                    img.save("Trained_Images/starting_noise.png")
-                    print(self.weights)
-                    print(self.dz)
-                    
-                    for _ in range(500):
-                        outputs=self.forward(noise/255)
-                        
-                        noise+=outputs
-                        noise=np.clip(noise,0,255)
-                        noise2=noise.reshape(50,50,3)
-
-                        noise2_numpy = noise2.get()
-                    img = Image.fromarray(noise2_numpy.astype('uint8'), "RGB")  # Ensure the data type is uint8 for image
-
-                    img.save(f"Trained_Images/Epoch_{epoch}.png")'''
-
-                    #webhook = DiscordWebhook(url=ping_webhook_URL, content=f'Done Milestone! {(epoch/epochs)*100}% done')
-                '''with open(f"Trained_Images/Epoch_{epoch}.png", 'rb') as f:
-                        webhook.add_file(file=f.read(), filename=f'Milestone_{epoch}_out_of_{epochs}.png')
-                    with open(f"Trained_Images/starting_noise.png", 'rb') as f:
-                        webhook.add_file(file=f.read(), filename=f'Starting Noise.png')'''
-                    #response = webhook.execute()
-                    
-            #if epochs>0:
-                #if epoch % math.ceil(epochs/5) == 0:
-                    #self.save_to_file("Thing.npy")
+            if epochs>0:
+                if epoch % maths.ceil(epochs/5) == 0:
+                    self.save_to_file("Thing.npy")
             
             
-            endingTime=time.time()
-            totalTime+=endingTime-startingTime
-            timeTaken=(totalTime/(epoch+1))*epochs
-            #print(f"Done epoch {epoch}/{epochs}. It will be done in {timeTaken-totalTime:.1f} seconds, or {(timeTaken-totalTime)/60:.1f} minutes, or {((timeTaken-totalTime)/60)/60:.2f} hours.")
-            
+
+
             
 
 
 
 
 
 
@@ -389,15 +615,15 @@
             layer_sum = biases[layer] + np.sum(layer_output,axis=0)
             last_vals = self.activate(layer_sum,activation)
             all_vals.append(last_vals)
             unactivated_vals.append(layer_sum)
         output = last_vals
         return output, [all_vals,unactivated_vals]
     
-    def chat_gippity_output(self, inputs, activation):
+    def get_output_3(self, inputs, activation):
         try:weights=self.weight_matrices
         except:raise Exception("Weight Matrix Initialisation error: Please initialise the weight matrix with initialise_matrices(weights), or if you're not a developer, dm dogzrgodz or That Guy#6482 on discord. ")
         try:biases = self.network[1]
         except:raise Exception("Biases Initialisation error: Network biases are not defined, to define biases load or randomise the neural network, or if you're not a developer, dm dogzrgodz or That Guy#6482 on discord. ")
 
         last_vals = inputs
         all_vals = [inputs]
@@ -415,15 +641,15 @@
         output = last_vals
         return output, [all_vals, unactivated_vals]
 
     def find_error(self,expected_outputs,states,activation):
         total_error=0
         startingTime=time.time()
         for state in range(len(states)):
-            output=self.chat_gippity_output(states[state],activation)
+            output=self.get_output_3(states[state],activation)
             total_error+=np.sum((output[0]-expected_outputs[state])**2)
             if time.time()-startingTime>=5:
                 print(f"5 seconds have gone by, we are at state {state}")
                 startingTime=time.time()
         return total_error/len(states)
     def error_deriv(self,outputs,expected_outputs):
         return 2*(outputs-expected_outputs)
@@ -443,15 +669,15 @@
         weight_derivs_2=weights
         
         bias_derivs_2=biases
         state_time=time.time()
         for state in range(len(states)): 
             
             curr_state_error=self.find_error([expected_outputs[state]],[states[state]],activation)
-            outputs,status=self.chat_gippity_output(states[state],activation)
+            outputs,status=self.get_output_3(states[state],activation)
             last_layer_error_derivs=self.error_deriv(outputs,expected_outputs[state])
             bias_derivs=[]
             weight_derivs=[]
             for layer in range(len(status[1])-1): 
                 curr_layer=status[1][-(layer+1)]
                 prevous_layer=status[1][-(layer+2)]
                 curr_layer_weights=self.weight_matrices[-(layer+1)]
@@ -497,15 +723,15 @@
         biases = np.zeros_like(biases)
         weight_derivs_2=weights
         
         bias_derivs_2=biases
         for state in range(len(states)): 
             
             curr_state_error=self.find_error([expected_outputs[state]],[states[state]],activation)
-            outputs,status=self.chat_gippity_output(states[state],activation)
+            outputs,status=self.get_output_3(states[state],activation)
             last_layer_error_derivs=self.error_deriv(outputs,expected_outputs[state])
             bias_derivs=[]
             weight_derivs=[]
             for layer in range(len(status[1])-1): 
                 curr_layer=status[1][-(layer+1)]
                 prevous_layer=status[1][-(layer+2)]
                 curr_layer_weights=self.weight_matrices[-(layer+1)]
@@ -623,14 +849,15 @@
                         prevous_error=recent_error_2
                         self.network=new_network_2
                         self.initialise_matrices()
                         
 
 class DQL:
     def __init__(self,inputs,middle,outputs,activation,learning_rate):
+        print("This is depreciated. Please use Optomised_Neural_Network")
         self.inputs=inputs
         self.middle=middle
         self.outputs=outputs
         self.activation=activation
         self.learning_rate=learning_rate
         self.replay_buffer=[] #[state, action, outputs, reward, terminal]
         self.nn=neural_network(inputs,middle,outputs)
@@ -643,15 +870,15 @@
         self.nn.randomise_network()
     def get_next_frame(self,state):
         #add to replay buffer
         output=self.nn.get_output(state,self.activation)
         first_index = int(np.where(output[0] == output[0].max())[0][0])
         return first_index, output
     def better_get_next_frame(self, state):
-        output = self.nn.chat_gippity_output(state, self.activation)
+        output = self.nn.get_output_3(state, self.activation)
         first_index = int(np.where(output[0] == output[0].max())[0][0])
         return first_index, output
     def replay_buffer_adder(self,state,action,outputs,reward,terminal):
         self.replay_buffer.append([state,action,outputs,reward,terminal])
     def prepare_for_backprop(self,reward_decay=0.99,randomise=True):
         expected_outputs=[]
         states=[]
```

### Comparing `pymindcore-0.1.2/pymindcore.egg-info/PKG-INFO` & `pymindcore-0.2.0/pymindcore.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: pymindcore
-Version: 0.1.2
+Version: 0.2.0
 Summary: A Python library for AI, easy to use, freely available for any use
 Home-page: https://github.com/Dogz-R-Godz/Pymind
 Author: Dogz R Godz
 Author-email: doggocam01@gmail.com
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: Pillow
-Requires-Dist: idx2numpy
+Requires-Dist: numexpr
+Requires-Dist: numba
 
-# Pymind
+# Pymindcore
 
 Pymind is a Python library for AI, supporting Numpy.
 
 ## Installation
 
-You can install Pymind using pip: pip install pymind.
+You can install Pymind using pip: pip install pymindcore.
 
 ## Usage
 
 You import it, you call the class with your neural network size, and you're away! There will be actual test files in the future, but for the meantime,
 
 ## License
 
@@ -48,7 +49,11 @@
     1: Go into the game you want to train an AI for, and think what points you would punish the AI for getting wrong. eg: dying, losing, etc.
     2: Play a game, and do one of each of those things yourself, screenshotting the whole screen each time you do one.
     3: Go into the screenshot in an app like ms paint, and find a pixel that is a certain colour when you did each of the bad things. (must be unique, and not trigger when either of the others happen)
     4: Go into line 199 of VideoGameAI.py, and add in your coordinates and the pixel colour of that coordinate (in RGB). I'd recommend using Gimp for it. It should extend down to line 207. Only change the rewards if you know what you are doing.
     4.5: If you have more than 3 punishment options, then you should copy one of them, and paste it below it, copy the __Coords, __RGB, and __Punishment, and paste them below as well.
     5: Figure out what keybinds your AI will need to have for the game. The ones set up for Minecraft should cover most bases, but to be safe, double check. If you want to, remove all the keybinds that your AI will not need, so it can learn easier.
     6: Run it and it should work!
+
+## Discord server
+
+Join the discord server https://discord.gg/MSMzmJ6ffj!
```

### Comparing `pymindcore-0.1.2/setup.py` & `pymindcore-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pymindcore',
-    version='0.1.2',
+    version='0.2.0',
     packages=find_packages(),
     description='A Python library for AI, easy to use, freely available for any use',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Dogz-R-Godz/Pymind',
     author='Dogz R Godz',
     author_email='doggocam01@gmail.com',
     license='CC0 1.0 Universal (CC0 1.0) Public Domain Dedication',
     install_requires=[
         'numpy',
         'Pillow',
-	    'idx2numpy'
-        # Include 'cupy' if you're making a version with CuPy support
+        'numexpr', 
+        'numba'
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication',
     ],
 )
```

