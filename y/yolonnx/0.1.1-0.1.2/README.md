# Comparing `tmp/yolonnx-0.1.1.tar.gz` & `tmp/yolonnx-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolonnx-0.1.1.tar", last modified: Tue Apr 23 09:29:04 2024, max compression
+gzip compressed data, was "yolonnx-0.1.2.tar", last modified: Thu Apr 25 11:27:33 2024, max compression
```

## Comparing `yolonnx-0.1.1.tar` & `yolonnx-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1099 2024-04-19 12:11:03.505690 yolonnx-0.1.1/LICENSE
--rw-r--r--   0        0        0     1282 2024-04-22 14:07:07.942295 yolonnx-0.1.1/README.md
--rw-r--r--   0        0        0      664 2024-04-23 09:29:04.199304 yolonnx-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-22 12:05:13.818667 yolonnx-0.1.1/src/yolonnx/__init__.py
--rw-r--r--   0        0        0      428 2024-04-23 07:40:59.649339 yolonnx-0.1.1/src/yolonnx/model.py
--rw-r--r--   0        0        0     1377 2024-04-22 13:45:27.021530 yolonnx-0.1.1/src/yolonnx/protocols.py
--rw-r--r--   0        0        0      108 2024-04-22 12:06:52.774186 yolonnx-0.1.1/src/yolonnx/services/__init__.py
--rw-r--r--   0        0        0     2186 2024-04-23 09:27:43.862303 yolonnx-0.1.1/src/yolonnx/services/classifier.py
--rw-r--r--   0        0        0     2988 2024-04-23 07:39:11.587139 yolonnx-0.1.1/src/yolonnx/services/detector.py
--rw-r--r--   0        0        0     1364 2024-04-22 13:50:09.339584 yolonnx-0.1.1/src/yolonnx/to_tensor_strategies.py
--rw-r--r--   0        0        0     1569 2024-04-22 12:31:23.751245 yolonnx-0.1.1/src/yolonnx/utils.py
--rw-r--r--   0        0        0        0 2024-04-23 08:14:27.133123 yolonnx-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1689 1970-01-01 00:00:00.000000 yolonnx-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1099 2024-04-19 12:11:03.505690 yolonnx-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1282 2024-04-22 14:07:07.942295 yolonnx-0.1.2/README.md
+-rw-r--r--   0        0        0      664 2024-04-25 11:27:33.072537 yolonnx-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-22 12:05:13.818667 yolonnx-0.1.2/src/yolonnx/__init__.py
+-rw-r--r--   0        0        0      428 2024-04-23 07:40:59.649339 yolonnx-0.1.2/src/yolonnx/model.py
+-rw-r--r--   0        0        0     1377 2024-04-22 13:45:27.021530 yolonnx-0.1.2/src/yolonnx/protocols.py
+-rw-r--r--   0        0        0      108 2024-04-22 12:06:52.774186 yolonnx-0.1.2/src/yolonnx/services/__init__.py
+-rw-r--r--   0        0        0     2327 2024-04-25 11:25:19.964794 yolonnx-0.1.2/src/yolonnx/services/classifier.py
+-rw-r--r--   0        0        0     2988 2024-04-23 07:39:11.587139 yolonnx-0.1.2/src/yolonnx/services/detector.py
+-rw-r--r--   0        0        0     1364 2024-04-22 13:50:09.339584 yolonnx-0.1.2/src/yolonnx/to_tensor_strategies.py
+-rw-r--r--   0        0        0     1569 2024-04-22 12:31:23.751245 yolonnx-0.1.2/src/yolonnx/utils.py
+-rw-r--r--   0        0        0        0 2024-04-23 08:14:27.133123 yolonnx-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     1689 1970-01-01 00:00:00.000000 yolonnx-0.1.2/PKG-INFO
```

### Comparing `yolonnx-0.1.1/LICENSE` & `yolonnx-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yolonnx-0.1.1/README.md` & `yolonnx-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `yolonnx-0.1.1/pyproject.toml` & `yolonnx-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "yolonnx"
-version = "0.1.1"
+version = "0.1.2"
 description = "You Only Look ONNX"
 authors = [
     { name = "Kasper Fromm Pedersen", email = "kasperf@cs.aau.dk" },
 ]
 dependencies = [
     "numpy==1.26.*",
     "aau-label==0.2.*",
```

### Comparing `yolonnx-0.1.1/src/yolonnx/protocols.py` & `yolonnx-0.1.2/src/yolonnx/protocols.py`

 * *Files identical despite different names*

### Comparing `yolonnx-0.1.1/src/yolonnx/services/classifier.py` & `yolonnx-0.1.2/src/yolonnx/services/classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,20 @@
 
 
 class Classifier(Generic[T]):
     def __init__(
         self,
         session: InferenceSessionProtocol,
         to_tensor_strategy: ToTensorStrategyProtocol[T],
+        none_cls_name: str = "none",
         threshold: float = 0.1,
     ) -> None:
         self.__session = session
         self.__to_tensor_strategy = to_tensor_strategy
+        self.__non_cls_name = none_cls_name
         self.__threshold = threshold
         meta = self.__session.get_modelmeta()
         self.__names: dict[int, str] = ast.literal_eval(
             meta.custom_metadata_map["names"]
         )
 
     @property
@@ -52,15 +54,16 @@
         labels_idx = numpy.argwhere(results > self.threshold)
         scores: NDArray[float32] = results[labels_idx]
 
         rv: list[ClassifierResult] = []
         for i in range(len(labels_idx)):
             id = labels_idx[i][0]
             label_name = self.names[id]
-            rv.append(ClassifierResult(name=label_name, score=scores[i]))
+            if label_name != self.__non_cls_name:
+                rv.append(ClassifierResult(name=label_name, score=scores[i][0]))
 
         rv.sort(key=lambda x: x.score, reverse=True)
         return rv
 
     def run(self, img: T) -> Sequence[ClassifierResult]:
         tensor = self.__to_tensor_strategy(img, *self.shape)
         results = self.__session.run(None, {"images": tensor.data})[0]
```

### Comparing `yolonnx-0.1.1/src/yolonnx/services/detector.py` & `yolonnx-0.1.2/src/yolonnx/services/detector.py`

 * *Files identical despite different names*

### Comparing `yolonnx-0.1.1/src/yolonnx/to_tensor_strategies.py` & `yolonnx-0.1.2/src/yolonnx/to_tensor_strategies.py`

 * *Files identical despite different names*

### Comparing `yolonnx-0.1.1/src/yolonnx/utils.py` & `yolonnx-0.1.2/src/yolonnx/utils.py`

 * *Files identical despite different names*

### Comparing `yolonnx-0.1.1/PKG-INFO` & `yolonnx-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolonnx
-Version: 0.1.1
+Version: 0.1.2
 Summary: You Only Look ONNX
 Keywords: ONNX,YOLOv8,onnxruntime,vision
 Home-page: https://www.cs.aau.dk/
 Author-Email: Kasper Fromm Pedersen <kasperf@cs.aau.dk>
 License: MIT
 Project-URL: Homepage, https://www.cs.aau.dk/
 Project-URL: Repository, https://github.com/fromm1990/yolonnx
```

