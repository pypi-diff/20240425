# Comparing `tmp/algophon-0.0.7.tar.gz` & `tmp/algophon-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algophon-0.0.7.tar", last modified: Fri Apr 19 17:55:21 2024, max compression
+gzip compressed data, was "algophon-0.0.8.tar", last modified: Wed Apr 24 23:35:16 2024, max compression
```

## Comparing `algophon-0.0.7.tar` & `algophon-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-19 17:55:21.845556 algophon-0.0.7/
--rw-r--r--   0 u6052607   (503) staff       (20)    11357 2024-04-18 14:18:03.000000 algophon-0.0.7/LICENSE
--rw-r--r--   0 u6052607   (503) staff       (20)     9611 2024-04-19 17:55:21.845037 algophon-0.0.7/PKG-INFO
--rw-r--r--   0 u6052607   (503) staff       (20)     9006 2024-04-19 00:09:14.000000 algophon-0.0.7/README.md
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-19 17:55:21.823849 algophon-0.0.7/algophon/
--rw-r--r--   0 u6052607   (503) staff       (20)      168 2024-04-18 16:51:58.000000 algophon-0.0.7/algophon/__init__.py
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-19 17:55:21.833758 algophon-0.0.7/algophon/dist/
--rw-r--r--   0 u6052607   (503) staff       (20)     4045 2024-04-19 14:52:46.000000 algophon-0.0.7/algophon/dist/edit_distance.py
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-19 17:55:21.839194 algophon-0.0.7/algophon/ipa/
--rw-r--r--   0 u6052607   (503) staff       (20)       32 2024-04-19 13:49:06.000000 algophon-0.0.7/algophon/ipa/__init__.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1347 2024-04-19 14:16:56.000000 algophon-0.0.7/algophon/ipa/convert.py
--rw-r--r--   0 u6052607   (503) staff       (20)   350526 2024-04-18 15:23:33.000000 algophon-0.0.7/algophon/ipa.txt
--rw-r--r--   0 u6052607   (503) staff       (20)     1006 2024-04-19 00:08:37.000000 algophon-0.0.7/algophon/natclass.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1173 2024-04-18 18:31:25.000000 algophon-0.0.7/algophon/seg.py
--rw-r--r--   0 u6052607   (503) staff       (20)     4745 2024-04-19 14:22:59.000000 algophon-0.0.7/algophon/seginv.py
--rw-r--r--   0 u6052607   (503) staff       (20)     5660 2024-04-19 17:53:50.000000 algophon-0.0.7/algophon/segstr.py
--rw-r--r--   0 u6052607   (503) staff       (20)      166 2024-04-18 18:39:21.000000 algophon-0.0.7/algophon/symbols.py
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-19 17:55:21.844452 algophon-0.0.7/algophon.egg-info/
--rw-r--r--   0 u6052607   (503) staff       (20)     9611 2024-04-19 17:55:21.000000 algophon-0.0.7/algophon.egg-info/PKG-INFO
--rw-r--r--   0 u6052607   (503) staff       (20)      472 2024-04-19 17:55:21.000000 algophon-0.0.7/algophon.egg-info/SOURCES.txt
--rw-r--r--   0 u6052607   (503) staff       (20)        1 2024-04-19 17:55:21.000000 algophon-0.0.7/algophon.egg-info/dependency_links.txt
--rw-r--r--   0 u6052607   (503) staff       (20)        9 2024-04-19 17:55:21.000000 algophon-0.0.7/algophon.egg-info/top_level.txt
--rw-r--r--   0 u6052607   (503) staff       (20)      789 2024-04-19 17:55:15.000000 algophon-0.0.7/pyproject.toml
--rw-r--r--   0 u6052607   (503) staff       (20)       38 2024-04-19 17:55:21.845614 algophon-0.0.7/setup.cfg
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-19 17:55:21.843870 algophon-0.0.7/tests/
--rw-r--r--   0 u6052607   (503) staff       (20)      860 2024-04-19 00:19:07.000000 algophon-0.0.7/tests/test_natclass.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1273 2024-04-18 23:49:35.000000 algophon-0.0.7/tests/test_seg.py
--rw-r--r--   0 u6052607   (503) staff       (20)     2132 2024-04-19 00:05:44.000000 algophon-0.0.7/tests/test_seginv.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1696 2024-04-19 17:54:23.000000 algophon-0.0.7/tests/test_segstr.py
--rw-r--r--   0 u6052607   (503) staff       (20)      740 2024-04-18 23:42:58.000000 algophon-0.0.7/tests/tester.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-24 23:35:16.081493 algophon-0.0.8/
+-rw-r--r--   0 u6052607   (503) staff       (20)    11357 2024-04-18 14:18:03.000000 algophon-0.0.8/LICENSE
+-rw-r--r--   0 u6052607   (503) staff       (20)     9611 2024-04-24 23:35:16.080694 algophon-0.0.8/PKG-INFO
+-rw-r--r--   0 u6052607   (503) staff       (20)     9006 2024-04-19 00:09:14.000000 algophon-0.0.8/README.md
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-24 23:35:16.066433 algophon-0.0.8/algophon/
+-rw-r--r--   0 u6052607   (503) staff       (20)      168 2024-04-18 16:51:58.000000 algophon-0.0.8/algophon/__init__.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-24 23:35:16.074730 algophon-0.0.8/algophon/dist/
+-rw-r--r--   0 u6052607   (503) staff       (20)     4045 2024-04-19 14:52:46.000000 algophon-0.0.8/algophon/dist/edit_distance.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-24 23:35:16.075919 algophon-0.0.8/algophon/ipa/
+-rw-r--r--   0 u6052607   (503) staff       (20)       32 2024-04-19 13:49:06.000000 algophon-0.0.8/algophon/ipa/__init__.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1347 2024-04-19 14:16:56.000000 algophon-0.0.8/algophon/ipa/convert.py
+-rw-r--r--   0 u6052607   (503) staff       (20)   350526 2024-04-18 15:23:33.000000 algophon-0.0.8/algophon/ipa.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)     1006 2024-04-19 00:08:37.000000 algophon-0.0.8/algophon/natclass.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1173 2024-04-18 18:31:25.000000 algophon-0.0.8/algophon/seg.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     5834 2024-04-24 23:33:05.000000 algophon-0.0.8/algophon/seginv.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     5780 2024-04-24 23:29:56.000000 algophon-0.0.8/algophon/segstr.py
+-rw-r--r--   0 u6052607   (503) staff       (20)      166 2024-04-18 18:39:21.000000 algophon-0.0.8/algophon/symbols.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-24 23:35:16.080019 algophon-0.0.8/algophon.egg-info/
+-rw-r--r--   0 u6052607   (503) staff       (20)     9611 2024-04-24 23:35:16.000000 algophon-0.0.8/algophon.egg-info/PKG-INFO
+-rw-r--r--   0 u6052607   (503) staff       (20)      472 2024-04-24 23:35:16.000000 algophon-0.0.8/algophon.egg-info/SOURCES.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)        1 2024-04-24 23:35:16.000000 algophon-0.0.8/algophon.egg-info/dependency_links.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)        9 2024-04-24 23:35:16.000000 algophon-0.0.8/algophon.egg-info/top_level.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)      789 2024-04-24 23:34:44.000000 algophon-0.0.8/pyproject.toml
+-rw-r--r--   0 u6052607   (503) staff       (20)       38 2024-04-24 23:35:16.081566 algophon-0.0.8/setup.cfg
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-24 23:35:16.079156 algophon-0.0.8/tests/
+-rw-r--r--   0 u6052607   (503) staff       (20)      860 2024-04-19 00:19:07.000000 algophon-0.0.8/tests/test_natclass.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1273 2024-04-18 23:49:35.000000 algophon-0.0.8/tests/test_seg.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     2746 2024-04-24 23:34:28.000000 algophon-0.0.8/tests/test_seginv.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1941 2024-04-24 23:29:27.000000 algophon-0.0.8/tests/test_segstr.py
+-rw-r--r--   0 u6052607   (503) staff       (20)      740 2024-04-18 23:42:58.000000 algophon-0.0.8/tests/tester.py
```

### Comparing `algophon-0.0.7/LICENSE` & `algophon-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `algophon-0.0.7/PKG-INFO` & `algophon-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algophon
-Version: 0.0.7
+Version: 0.0.8
 Summary: Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)
 Author: Caleb Belth
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/cbelth/algophon
 Keywords: computational linguistics,phonology,morphology,natural language processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `algophon-0.0.7/README.md` & `algophon-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `algophon-0.0.7/algophon/dist/edit_distance.py` & `algophon-0.0.8/algophon/dist/edit_distance.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.7/algophon/ipa/convert.py` & `algophon-0.0.8/algophon/ipa/convert.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.7/algophon/ipa.txt` & `algophon-0.0.8/algophon/ipa.txt`

 * *Files identical despite different names*

### Comparing `algophon-0.0.7/algophon/natclass.py` & `algophon-0.0.8/algophon/natclass.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.7/algophon/seg.py` & `algophon-0.0.8/algophon/seg.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.7/algophon/seginv.py` & `algophon-0.0.8/algophon/seginv.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from algophon.seg import Seg
 from algophon.natclass import NatClass
+from algophon.symbols import UNDERSPECIFIED
 
 import pkgutil
 
 class SegInv:
     '''
     A class representing an inventory of phonological segments (Seg objects).
     '''
@@ -135,8 +136,33 @@
     
     def extension_complement(self, nat_class) -> set:
         '''
         :nat_class: a set of features or a NatClass object
 
         :return: the extensional complement of :nat_class: relative to :self: SegInv \ NatClass
         '''
-        return self.segs.difference(self.extension(nat_class=nat_class))
+        return self.segs.difference(self.extension(nat_class=nat_class))
+    
+    def feature_intersection(self, segs, exclude_underspecified: bool=True) -> set:
+        '''
+        :segs: an iterable of phonological segments
+        :exclude_underspecified: if True (default), excludes features that all the segments are underspecified for
+
+        :return: the features shared by all the :segs: (excludes features where all segs are underspecified)
+        '''
+        segs = set(self[seg] for seg in segs)
+        return set.intersection(*list(set(f'{val}{feat}' for feat, val in seg.features.items() if val != UNDERSPECIFIED or not exclude_underspecified) for seg in segs))
+    
+    def feature_diff(self, seg1, seg2) -> set:
+        '''
+        :seg1: phonological segment
+        :seg2: phonological segment
+
+        :return: the features that differ between :seg1: and :seg2:
+        '''
+        seg1 = self[seg1]
+        seg2 = self[seg2]
+        diff = set()
+        for feat in self.feature_space:
+            if seg1.features[feat] != seg2.features[feat]:
+                diff.add(feat)
+        return diff
```

### Comparing `algophon-0.0.7/algophon/segstr.py` & `algophon-0.0.8/algophon/segstr.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,16 @@
             - a list of Seg objects
             - a SegStr object
         '''
         if isinstance(other, str):
             other = other.split()
         elif not isinstance(other, list) and not isinstance(other, SegStr):
             raise ValueError(f'Cannot compare a SegStr object with an object of type {type(other)}')
+        if len(other) > len(self):
+            return False
         for idx in range(len(other)):
             if self._segs[idx] != other[idx]:
                 return False
         return True
     
     def endswith(self, other: object) -> bool:
         '''
@@ -133,14 +135,16 @@
             - a list of Seg objects
             - a SegStr object
         '''
         if isinstance(other, str):
             other = other.split()
         elif not isinstance(other, list) and not isinstance(other, SegStr):
             raise ValueError(f'Cannot compare a SegStr object with an object of type {type(other)}')
+        if len(other) > len(self):
+            return False
         idx = -1
         for offset in range(len(other)):
             if self._segs[idx - offset] != other[idx - offset]:
                 return False
         return True
 
     def count(self, item: object) -> int:
```

### Comparing `algophon-0.0.7/algophon.egg-info/PKG-INFO` & `algophon-0.0.8/algophon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algophon
-Version: 0.0.7
+Version: 0.0.8
 Summary: Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)
 Author: Caleb Belth
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/cbelth/algophon
 Keywords: computational linguistics,phonology,morphology,natural language processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `algophon-0.0.7/pyproject.toml` & `algophon-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "algophon"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
     { name = "Caleb Belth" },
 ]
 description = "Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "Apache 2.0" }
```

### Comparing `algophon-0.0.7/tests/test_natclass.py` & `algophon-0.0.8/tests/test_natclass.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.7/tests/test_seg.py` & `algophon-0.0.8/tests/test_seg.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.7/tests/test_seginv.py` & `algophon-0.0.8/tests/test_seginv.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,9 +41,24 @@
     def test_extension_complement(self):
         seginv = SegInv()
         seginv.add_segs({'a', 'e', 'i', 'o', 'u', 'p', 'b', 't', 'd', 'k', 'g', 's', 'm', 'n'})
         assert(seginv.extension_complement({'+syl'}) == {'p', 'b', 't', 'd', 'k', 'g', 's', 'm', 'n'})
         assert(seginv.extension_complement({'+cons'}) == {'a', 'e', 'i', 'o', 'u'})
         assert(seginv.extension_complement({'-syl', '+voi'}) == {'a', 'e', 'i', 'o', 'u', 'p', 't', 'k', 's'})
 
+    def test_feature_intersection(self):
+        seginv = SegInv()
+        vs = {'a', 'e', 'i', 'o', 'u'}
+        seginv.add_segs(vs)
+        assert(seginv.feature_intersection(vs) == {'+cont', '-sg', '-delrel', '+tense', '-long', '-cons', '-velaric',
+                                                   '-nas', '+syl', '-cg', '+voi', '-lat', '+son', '-cor'})
+        
+    def test_feature_diff(self):
+        seginv = SegInv()
+        seginv.add_segs({'t', 'd'})
+        assert(seginv.feature_diff('t', 'd') == {'voi'})
+
+        seginv.add_segs({'i', 'e'})
+        assert(seginv.feature_diff('i', 'e') == {'hi'})
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `algophon-0.0.7/tests/test_segstr.py` & `algophon-0.0.8/tests/test_segstr.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,20 +21,29 @@
         assert(x[0] == 'eː')
         assert(x[-2:] == 'j ə')
         assert(x[-2:] != 'ə n')
         assert(isinstance(x[0], Seg))
         assert(isinstance(x[-2:], SegStr))
 
     def test_endswith_startswith(self):
-        x = SegStr('eː n t j ə', seginv=SegInv())
+        seginv = SegInv()
+        x = SegStr('eː n t j ə', seginv=seginv)
         assert(x.endswith('j ə'))
         sufx = x[-2:]
         assert(x.endswith(sufx))
         assert(x.startswith(x[:-2]))
 
+        y = SegStr('eː n t', seginv=seginv)
+        assert(x.startswith(y))
+        assert(not y.startswith(x))
+
+        z = SegStr('j ə', seginv=seginv)
+        assert(x.endswith(z))
+        assert(not z.endswith(x))
+
     def test_hash(self):
         x = SegStr('eː n t j ə', seginv=SegInv())
         assert(len({x, 'eː n t j ə'}))
         assert(x in {'eː n t j ə'})
         assert('eː n t j ə' in {x})
         assert(len({x, 'eː n t j ə', SegStr('eː n t j ə', seginv=SegInv())}) == 1)
```

### Comparing `algophon-0.0.7/tests/tester.py` & `algophon-0.0.8/tests/tester.py`

 * *Files identical despite different names*

