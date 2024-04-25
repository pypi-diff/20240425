# Comparing `tmp/mimllearning-0.1.9.tar.gz` & `tmp/mimllearning-0.2.0.tar.gz`

## Comparing `mimllearning-0.1.9.tar` & `mimllearning-0.2.0.tar`

### file list

```diff
@@ -1,48 +1,45 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 mimllearning-0.1.9/.gitattributes
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 mimllearning-0.1.9/readme.md
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 mimllearning-0.1.9/todo.md
--rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 mimllearning-0.1.9/update.bat
--rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.1.9/documentation/AnteproyectoDamianTFG.pdf
--rw-r--r--   0        0        0    83682 2020-02-02 00:00:00.000000 mimllearning-0.1.9/documentation/Formato datos tfg.png
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/__init__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/classifier/__init__.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/classifier/miml_classifier.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/classifier/mi/__init__.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/classifier/mi/all_positive_apr_classifier.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/classifier/mi/apr_classifier.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/classifier/mi/iterated_discrim_apr_classifier.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/classifier/mi/miles_classifier.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/classifier/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/classifier/mimlTOml/__init__.py
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/data/__init__.py
--rw-r--r--   0        0        0     9087 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/data/bag.py
--rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/data/instance.py
--rw-r--r--   0        0        0    15284 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/data/miml_dataset.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/datasets/__init__.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/datasets/arff_to_csv.py
--rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/datasets/load_dataset.py
--rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/datasets/miml_birds.arff
--rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/datasets/miml_birds.csv
--rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/datasets/miml_birds_random_20test.arff
--rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/datasets/miml_birds_random_80train.arff
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/datasets/toy.arff
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/datasets/toy.csv
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/test/data_test.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/transformation/__init__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/transformation/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/transformation/mimlTOml/__init__.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/transformation/mimlTOml/arithmetic.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/transformation/mimlTOml/geometric.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/transformation/mimlTOml/minmax.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/tutorial/classifiers_tutorial.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/tutorial/datasets_tutorial.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 mimllearning-0.1.9/src/miml/tutorial/transformation_tutorial.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 mimllearning-0.1.9/.gitignore
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 mimllearning-0.1.9/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 mimllearning-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 mimllearning-0.2.0/.gitattributes
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mimllearning-0.2.0/readme.md
+-rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.2.0/documentation/AnteproyectoDamianTFG.pdf
+-rw-r--r--   0        0        0    83682 2020-02-02 00:00:00.000000 mimllearning-0.2.0/documentation/Formato datos tfg.png
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/__init__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/classifier/__init__.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/classifier/miml_classifier.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/classifier/mi/__init__.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/classifier/mi/all_positive_apr_classifier.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/classifier/mi/apr_classifier.py
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/classifier/mi/iterated_discrim_apr_classifier.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/classifier/mi/miles_classifier.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/classifier/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/classifier/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/data/__init__.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/data/arff_to_csv.py
+-rw-r--r--   0        0        0     9089 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/data/bag.py
+-rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/data/instance.py
+-rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/data/load_datasets.py
+-rw-r--r--   0        0        0    15276 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/data/miml_dataset.py
+-rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/datasets/miml_birds.arff
+-rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/datasets/miml_birds.csv
+-rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/datasets/miml_birds_random_20test.arff
+-rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/datasets/miml_birds_random_80train.arff
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/datasets/toy.arff
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/datasets/toy.csv
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/test/data_test.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/transformation/__init__.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/transformation/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/transformation/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/transformation/mimlTOml/arithmetic.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/transformation/mimlTOml/geometric.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/transformation/mimlTOml/minmax.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/tutorial/classifiers_tutorial.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/tutorial/datasets_tutorial.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mimllearning-0.2.0/src/miml/tutorial/transformation_tutorial.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 mimllearning-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mimllearning-0.2.0/README.md
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 mimllearning-0.2.0/PKG-INFO
```

### Comparing `mimllearning-0.1.9/readme.md` & `mimllearning-0.2.0/readme.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install miml.
 
 ```bash
 $ pip install mimllearning
 ```
 #### Requirements
-The requirement packages for miml library are: numpy, scikit-learn, scipy, tensorflow or tensorflow-gpu.
+The requirement packages for miml library are: numpy, scikit-learn, scipy, mil, tensorflow and keras.
 Installing miml with the package manager does not install the package dependencies.
 So install them with the package manager manually if not already downloaded.
 
     $ pip install numpy
     $ pip install scikit-learn
     $ pip install scipy
+    $ pip install mil
     $ pip install tensorflow
+    $ pip install keras==2.12.0
 
 ### License
 [![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)
 - **[MIT license](http://opensource.org/licenses/mit-license.php)**
```

### Comparing `mimllearning-0.1.9/documentation/AnteproyectoDamianTFG.pdf` & `mimllearning-0.2.0/documentation/AnteproyectoDamianTFG.pdf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.9/documentation/Formato datos tfg.png` & `mimllearning-0.2.0/documentation/Formato datos tfg.png`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.9/src/miml/classifier/miml_classifier.py` & `mimllearning-0.2.0/src/miml/classifier/miml_classifier.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+import importlib
+import numpy as np
+
 from abc import ABC, abstractmethod
 
-import numpy as np
 
-from data.bag import Bag
-from data.miml_dataset import MIMLDataset
-from sklearn.metrics import classification_report, hamming_loss
+Bag = importlib.import_module(".bag", package="miml.data").Bag
+MIMLDataset = importlib.import_module(".miml_dataset", package="miml.data").MIMLDataset
 
 
 class MIMLClassifier(ABC):
     """
     Class to represent a MIMLClassifier
     """
 
@@ -20,16 +21,16 @@
     def fit(self, dataset_train: MIMLDataset) -> None:
         """
 
         Parameters
         ----------
         dataset_train
         """
-        if not isinstance(dataset_train, MIMLDataset):
-            raise Exception("Fit function should receive a MIMLDataset as parameter")
+        # if not isinstance(dataset_train, MIMLDataset):
+        #    raise Exception("Fit function should receive a MIMLDataset as parameter")
 
         self.fit_internal(dataset_train)
 
     @abstractmethod
     def fit_internal(self, dataset_train: MIMLDataset):
         pass
 
@@ -60,9 +61,9 @@
     def evaluate(self, dataset_test: MIMLDataset):
         """
 
         Parameters
         ----------
         dataset_test
         """
-        if not isinstance(dataset_test, MIMLDataset):
-            raise Exception("Evaluate function should receive a MIMLDataset as parameter")
+        # if not isinstance(dataset_test, MIMLDataset):
+        #    raise Exception("Evaluate function should receive a MIMLDataset as parameter")
```

### Comparing `mimllearning-0.1.9/src/miml/classifier/mi/all_positive_apr_classifier.py` & `mimllearning-0.2.0/src/miml/classifier/mi/all_positive_apr_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.9/src/miml/classifier/mi/iterated_discrim_apr_classifier.py` & `mimllearning-0.2.0/src/miml/classifier/mi/iterated_discrim_apr_classifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import numpy as np
 
 
 class IteratedDiscrimAPRClassifier:
 
     def __init__(self):
         """
@@ -76,15 +75,14 @@
                     not_positives_bag_in_apr.append(bag_index)
 
         # calculate new apr with not_positive_bag_in_apr and compare size
         new_aprs = []
         new_aprs_size = []
         apr_min, apr_max = None, None
         for bag_index in not_positives_bag_in_apr:
-            apr = None
             for instance in self.x_train[bag_index]:
                 apr_min = np.minimum(self.apr[0], instance)
                 apr_max = np.maximum(self.apr[1], instance)
             apr = (apr_min, apr_max)
             new_aprs.append(apr)
             new_aprs_size.append(self.size(apr))
```

### Comparing `mimllearning-0.1.9/src/miml/classifier/mi/miles_classifier.py` & `mimllearning-0.2.0/src/miml/classifier/mi/miles_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.9/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py` & `mimllearning-0.2.0/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,54 @@
-from copy import deepcopy
+import importlib
+from abc import abstractmethod
 
-from classifier.mimlTOmi.miml_to_mi_classifier import MIMLtoMIClassifier
-from classifier.miml_classifier import *
-from data.miml_dataset import MIMLDataset
-from transformation.mimlTOmi.binary_relevance_transformation import BinaryRelevanceTransformation
+import numpy as np
 
+from ..miml_classifier import MIMLClassifier
 
-class MIMLtoMIBRClassifier(MIMLtoMIClassifier):
+Bag = importlib.import_module(".bag", package="miml.data").Bag
+MIMLDataset = importlib.import_module(".miml_dataset", package="miml.data").MIMLDataset
+
+
+class MIMLtoMIClassifier(MIMLClassifier):
     """
     Class to represent a multiinstance classifier
     """
 
-    def __init__(self, classifier) -> None:
+    def __init__(self, mi_classifier):
         """
-        Constructor of the class MIMLtoMIBRClassifier
+        Constructor of the class MIMLtoMIClassifier
 
         Parameters
         ----------
-        classifier
+        mi_classifier
             Specific classifier to be used
         """
-        super().__init__(classifier)
-        self.transformation = BinaryRelevanceTransformation()
-        self.classifiers = []
+        super().__init__()
+        self.classifier = mi_classifier
 
-    def fit_internal(self, dataset_train: MIMLDataset) -> None:
-        """
-        Training the classifier
+    @abstractmethod
+    def fit_internal(self, dataset_train: MIMLDataset):
+        pass
 
-        Parameters
-        ----------
-        dataset_train: MIMLDataset
-            Dataset to train the classifier
-        """
-        for x in range(dataset_train.get_number_labels()):
-            classifier = deepcopy(self.classifier)
-            self.classifiers.append(classifier)
-
-        datasets = self.transformation.transform_dataset(dataset_train)
-        for i in range(len(datasets)):
-            self.classifiers[i].fit(datasets[i][0], datasets[i][1])
-
-    def predict(self, x):
-        results = np.zeros((len(self.classifiers)))
-        # Prediction of each label
-        for i in range(len(self.classifiers)):
-            results[i] = self.classifiers[i].predict(x)
-        return results
+    def predict(self, x: np.ndarray):
+        return self.classifier.predict(x)
 
     def predict_bag(self, bag: Bag):
         """
         Predict labels of given data
 
         Parameters
         ----------
         bag : Bag
             Bag to predict their classes
         """
         super().predict_bag(bag)
-        bags = self.transformation.transform_bag(bag)
-
-        return self.predict(bags[0][0])
 
     def evaluate(self, dataset_test: MIMLDataset):
         """
 
         Parameters
         ----------
         dataset_test
         """
         super().evaluate(dataset_test)
-
-        datasets = self.transformation.transform_dataset(dataset_test)
-
-        results = np.zeros((dataset_test.get_number_bags(), dataset_test.get_number_labels()))
-        for i, bag in enumerate(datasets[0][0]):
-            results[i] = self.predict(bag)
-
-        print(classification_report(dataset_test.get_labels_by_bag(), results))
-        print("Hamming Loss: ", hamming_loss(dataset_test.get_labels_by_bag(), results))
```

### Comparing `mimllearning-0.1.9/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py` & `mimllearning-0.2.0/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+import importlib
+import numpy as np
 
+from sklearn.metrics import classification_report, hamming_loss
+from ..miml_classifier import MIMLClassifier
 
-from classifier.miml_classifier import *
-
-from transformation.mimlTOml.miml_to_ml_transformation import MIMLtoMLTransformation
+MIMLtoMLTransformation = importlib.import_module(".miml_to_ml_transformation", package="miml.transformation.mimlTOml")
+Bag = importlib.import_module(".bag", package="miml.data").Bag
+MIMLDataset = importlib.import_module(".miml_dataset", package="miml.data").MIMLDataset
 
 
 class MIMLtoMLClassifier(MIMLClassifier):
 
     def __init__(self, ml_classifier, transformation: MIMLtoMLTransformation) -> None:
         """
         Constructor of the class MIMLtoMIClassifier
@@ -59,8 +63,11 @@
         super().evaluate(dataset_test)
         x_test, y_test = self.transformation.transform_dataset(dataset_test)
         results = self.predict(x_test)
 
         print(classification_report(dataset_test.get_labels_by_bag(), results))
         print("Hamming Loss: ", hamming_loss(dataset_test.get_labels_by_bag(), results))
 
-
+        # TODO: To Csv file
+        # report = classification_report(y_test, y_pred, output_dict=True)
+        # df = pandas.DataFrame(report).transpose()
+        # df.to_csv
```

### Comparing `mimllearning-0.1.9/src/miml/data/bag.py` & `mimllearning-0.2.0/src/miml/data/bag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
-from tabulate import tabulate
 
-from data.instance import Instance
+from tabulate import tabulate
+from .instance import Instance
 
 
 class Bag:
     """
     Class to manage MIML Bag data representation
     """
 
@@ -253,15 +253,15 @@
         values: array-like of shape (n_attributes)
             Values for the new attribute. If not provided, new values would be zero
         """
         if self.dataset is None:
             if position is None:
                 position = len(self.data)
             if values is None:
-                values = np.array([0]*self.get_number_instances())
+                values = np.array([0] * self.get_number_instances())
             elif len(values) != self.get_number_instances():
                 raise Exception("Incorrect number of values for the new attribute. Should be the same as number of "
                                 "instances of the bag")
             self.data = np.insert(self.data, position, values, axis=1)
         else:
             raise Exception("Can't add an attribute to a bag assigned to a dataset")
 
@@ -291,13 +291,13 @@
         self.dataset = dataset
 
     def show_bag(self) -> None:
         """
         Show bag info in table format
         """
         if self.dataset is None:
-            table = [[self.key]+[""]*self.get_number_attributes()]
+            table = [[self.key] + [""] * self.get_number_attributes()]
         else:
             table = [[self.key] + self.get_features_name() + self.get_labels_name()]
         for index_instance in range(self.get_number_instances()):
             table.append([index_instance] + list(self.get_instance(index_instance).get_attributes()))
         print(tabulate(table, headers='firstrow', tablefmt="grid", numalign="center"))
```

### Comparing `mimllearning-0.1.9/src/miml/data/instance.py` & `mimllearning-0.2.0/src/miml/data/instance.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.9/src/miml/data/miml_dataset.py` & `mimllearning-0.2.0/src/miml/data/miml_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 
-from data.bag import Bag
-from data.instance import Instance
+from .bag import Bag
+from .instance import Instance
 
 
 class MIMLDataset:
     """
     Class to manage MIML data obtained from datasets
     """
```

### Comparing `mimllearning-0.1.9/src/miml/datasets/arff_to_csv.py` & `mimllearning-0.2.0/src/miml/data/arff_to_csv.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.9/src/miml/datasets/load_dataset.py` & `mimllearning-0.2.0/src/miml/data/load_datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import os
-
 import numpy as np
+import os
 
-from data.bag import Bag
-from data.instance import Instance
-from data.miml_dataset import MIMLDataset
+from .bag import Bag
+from .instance import Instance
+from .miml_dataset import MIMLDataset
 
 
 def load_dataset(file, delimiter="\""):
     """
     Function to load a dataset
 
     Parameters
```

### Comparing `mimllearning-0.1.9/src/miml/datasets/miml_birds.arff` & `mimllearning-0.2.0/src/miml/datasets/miml_birds.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.9/src/miml/datasets/miml_birds.csv` & `mimllearning-0.2.0/src/miml/datasets/miml_birds.csv`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.9/src/miml/datasets/miml_birds_random_20test.arff` & `mimllearning-0.2.0/src/miml/datasets/miml_birds_random_20test.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.9/src/miml/datasets/miml_birds_random_80train.arff` & `mimllearning-0.2.0/src/miml/datasets/miml_birds_random_80train.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.9/src/miml/test/data_test.py` & `mimllearning-0.2.0/src/miml/test/data_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,16 +27,15 @@
         bag = Bag("1")
         bag.add_instance(instance)
         self.assertEqual(bag.get_number_instances(), 1)
         self.assertEqual(list(bag.get_instance(0).get_attributes()), list(instance.get_attributes()))
         self.assertEqual(bag.get_number_attributes(), 5)
         instance.set_attribute(1, 1)
         self.assertEqual(list(bag.get_instance(0).get_attributes()), list(instance.get_attributes()))
-        #bag.add_instance(instance)
-
+        # bag.add_instance(instance)
 
     def test_mimldataset(self):
         # TODO:
         pass
 
     def test_final(self):
         # TODO:
@@ -46,14 +45,14 @@
         bag = Bag("bag1")
         bag.add_instance(instance1)
         bag.add_instance(instance2)
 
         dataset = MIMLDataset()
         dataset.set_features_name(["attr1", "attr2", "attr3"])
         dataset.set_labels_name(["label1", "label2"])
-        #instance1.show_instance()
+        # instance1.show_instance()
         dataset.add_bag(bag)
-        #instance1.show_instance()
+        # instance1.show_instance()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `mimllearning-0.1.9/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py` & `mimllearning-0.2.0/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from data.bag import Bag
-from data.miml_dataset import MIMLDataset
+import importlib
+
+Bag = importlib.import_module(".bag", package="miml.data").Bag
+MIMLDataset = importlib.import_module(".miml_dataset", package="miml.data").MIMLDataset
 
 
 class BinaryRelevanceTransformation:
     """
     Class that performs a binary relevance transformation to convert a MIMLDataset class to numpy ndarrays.
     """
 
@@ -44,9 +46,7 @@
         -------
         bags : list[ndarray]
         Tuple of numpy ndarray with attribute values and labels
 
         """
         bags = [[bag.get_features(), label] for label in bag.get_labels()[0]]
         return bags
-
-
```

### Comparing `mimllearning-0.1.9/src/miml/transformation/mimlTOml/arithmetic.py` & `mimllearning-0.2.0/src/miml/transformation/mimlTOml/arithmetic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+import importlib
+
 import numpy as np
 
-from data.bag import Bag
-from data.miml_dataset import MIMLDataset
-from transformation.mimlTOml.miml_to_ml_transformation import MIMLtoMLTransformation
+from .miml_to_ml_transformation import MIMLtoMLTransformation
+
+Bag = importlib.import_module(".bag", package="miml.data").Bag
+MIMLDataset = importlib.import_module(".miml_dataset", package="miml.data").MIMLDataset
 
 
 class ArithmeticTransformation(MIMLtoMLTransformation):
     """
     Class that performs an arithmetic transformation to convert a MIMLDataset class to numpy ndarrays.
     """
```

### Comparing `mimllearning-0.1.9/src/miml/transformation/mimlTOml/geometric.py` & `mimllearning-0.2.0/src/miml/transformation/mimlTOml/geometric.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+import importlib
+
 import numpy as np
 
-from data.bag import Bag
-from data.miml_dataset import MIMLDataset
-from transformation.mimlTOml.miml_to_ml_transformation import MIMLtoMLTransformation
+from .miml_to_ml_transformation import MIMLtoMLTransformation
+
+Bag = importlib.import_module(".bag", package="miml.data").Bag
+MIMLDataset = importlib.import_module(".miml_dataset", package="miml.data").MIMLDataset
 
 
 class GeometricTransformation(MIMLtoMLTransformation):
     """
     Class that performs a geometric transformation to convert a MIMLDataset class to numpy ndarrays.
     """
 
     def __init__(self):
         super().__init__()
 
-    def transform_dataset(self, dataset):
+    def transform_dataset(self, dataset: MIMLDataset):
         """
         Transform the dataset to multilabel dataset converting each bag into a single instance being the value of each
         attribute the geometric center of the instances in the bag.
 
         Returns
         -------
 
@@ -59,8 +62,8 @@
         # TODO: Test
 
         features = bag.get_features()
         labels = bag.get_labels()[0]
         min_values = np.min(features, axis=0)
         max_values = np.max(features, axis=0)
         features = (min_values + max_values) / 2
-        return features, labels
+        return features, labels
```

### Comparing `mimllearning-0.1.9/src/miml/transformation/mimlTOml/minmax.py` & `mimllearning-0.2.0/src/miml/transformation/mimlTOml/minmax.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+import importlib
+
 import numpy as np
 
-from data.bag import Bag
-from data.miml_dataset import MIMLDataset
-from transformation.mimlTOml.miml_to_ml_transformation import MIMLtoMLTransformation
+from .miml_to_ml_transformation import MIMLtoMLTransformation
+
+Bag = importlib.import_module(".bag", package="miml.data").Bag
+MIMLDataset = importlib.import_module(".miml_dataset", package="miml.data").MIMLDataset
 
 
 class MinMaxTransformation(MIMLtoMLTransformation):
     """
     Class that performs a minmax transformation to convert a MIMLDataset class to numpy ndarrays.
     """
```

### Comparing `mimllearning-0.1.9/README.md` & `mimllearning-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install miml.
 
 ```bash
 $ pip install mimllearning
 ```
 #### Requirements
-The requirement packages for miml library are: numpy, scikit-learn, scipy, tensorflow or tensorflow-gpu.
+The requirement packages for miml library are: numpy, scikit-learn, scipy, mil, tensorflow and keras.
 Installing miml with the package manager does not install the package dependencies.
 So install them with the package manager manually if not already downloaded.
 
     $ pip install numpy
     $ pip install scikit-learn
     $ pip install scipy
+    $ pip install mil
     $ pip install tensorflow
+    $ pip install keras==2.12.0
 
 ### License
 [![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)
 - **[MIT license](http://opensource.org/licenses/mit-license.php)**
```

### Comparing `mimllearning-0.1.9/pyproject.toml` & `mimllearning-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 requires = ["hatchling", "pkginfo >= 1.10"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/miml", "src/miml/*"]
 
 [metadata]
-version = "0.1.9"
+version = "0.2.0"
 name = "mimllearning"
 
 [project]
 name = "mimllearning"
-version = "0.1.9"
+version = "0.2.0"
 authors = [
   { name="Damian Martinez", email="damianmartinezavila@gmail.com" },
 ]
 description = "MIML Learning Library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mimllearning-0.1.9/PKG-INFO` & `mimllearning-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mimllearning
-Version: 0.1.9
+Version: 0.2.0
 Summary: MIML Learning Library
 Project-URL: Homepage, https://github.com/p82maavd/miml
 Author-email: Damian Martinez <damianmartinezavila@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -22,19 +22,21 @@
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install miml.
 
 ```bash
 $ pip install mimllearning
 ```
 #### Requirements
-The requirement packages for miml library are: numpy, scikit-learn, scipy, tensorflow or tensorflow-gpu.
+The requirement packages for miml library are: numpy, scikit-learn, scipy, mil, tensorflow and keras.
 Installing miml with the package manager does not install the package dependencies.
 So install them with the package manager manually if not already downloaded.
 
     $ pip install numpy
     $ pip install scikit-learn
     $ pip install scipy
+    $ pip install mil
     $ pip install tensorflow
+    $ pip install keras==2.12.0
 
 ### License
 [![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)
 - **[MIT license](http://opensource.org/licenses/mit-license.php)**
```

