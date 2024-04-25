# Comparing `tmp/Quanthon-0.3.6.tar.gz` & `tmp/quanthon-0.3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Quanthon-0.3.6.tar", last modified: Wed Apr 24 11:09:56 2024, max compression
+gzip compressed data, was "quanthon-0.3.6.1.tar", last modified: Wed Apr 24 11:31:25 2024, max compression
```

## Comparing `Quanthon-0.3.6.tar` & `quanthon-0.3.6.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-24 11:09:56.460278 Quanthon-0.3.6/
--rw-r--r--   0 bukser     (501) staff       (20)        0 2023-09-14 17:15:45.000000 Quanthon-0.3.6/LICENSE
--rw-r--r--   0 bukser     (501) staff       (20)     2519 2024-04-24 11:09:56.460089 Quanthon-0.3.6/PKG-INFO
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-24 11:09:56.457578 Quanthon-0.3.6/Quanthon/
--rw-r--r--   0 bukser     (501) staff       (20)     3709 2024-03-04 09:48:46.000000 Quanthon-0.3.6/Quanthon/Models.py
--rw-r--r--   0 bukser     (501) staff       (20)      340 2024-04-22 07:48:46.000000 Quanthon-0.3.6/Quanthon/__init__.py
--rw-r--r--   0 bukser     (501) staff       (20)     6876 2024-04-10 00:56:44.000000 Quanthon-0.3.6/Quanthon/algorithms.py
--rw-r--r--   0 bukser     (501) staff       (20)     4727 2024-04-10 00:49:28.000000 Quanthon-0.3.6/Quanthon/ansatzs.py
--rw-r--r--   0 bukser     (501) staff       (20)    12033 2024-04-10 00:38:34.000000 Quanthon-0.3.6/Quanthon/base.py
--rw-r--r--   0 bukser     (501) staff       (20)     5974 2024-04-03 18:36:12.000000 Quanthon-0.3.6/Quanthon/expectation.py
--rw-r--r--   0 bukser     (501) staff       (20)     4796 2024-04-24 11:09:30.000000 Quanthon-0.3.6/Quanthon/mappers.py
--rw-r--r--   0 bukser     (501) staff       (20)     6714 2024-04-24 11:09:39.000000 Quanthon-0.3.6/Quanthon/mappers_utils.py
--rw-r--r--   0 bukser     (501) staff       (20)      455 2024-04-18 10:41:02.000000 Quanthon-0.3.6/Quanthon/physics.py
--rw-r--r--   0 bukser     (501) staff       (20)     2302 2024-03-13 12:44:21.000000 Quanthon-0.3.6/Quanthon/ut_pyscf_mel.py
--rw-r--r--   0 bukser     (501) staff       (20)     1714 2024-03-18 22:32:17.000000 Quanthon-0.3.6/Quanthon/ut_qiskit_hamiltonian.py
--rw-r--r--   0 bukser     (501) staff       (20)     5299 2024-03-21 16:15:37.000000 Quanthon-0.3.6/Quanthon/ut_test_jw.py
--rw-r--r--   0 bukser     (501) staff       (20)     6569 2024-04-18 11:08:36.000000 Quanthon-0.3.6/Quanthon/utils.py
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-24 11:09:56.459907 Quanthon-0.3.6/Quanthon.egg-info/
--rw-r--r--   0 bukser     (501) staff       (20)     2519 2024-04-24 11:09:56.000000 Quanthon-0.3.6/Quanthon.egg-info/PKG-INFO
--rw-r--r--   0 bukser     (501) staff       (20)      581 2024-04-24 11:09:56.000000 Quanthon-0.3.6/Quanthon.egg-info/SOURCES.txt
--rw-r--r--   0 bukser     (501) staff       (20)        1 2024-04-24 11:09:56.000000 Quanthon-0.3.6/Quanthon.egg-info/dependency_links.txt
--rw-r--r--   0 bukser     (501) staff       (20)        6 2024-04-24 11:09:56.000000 Quanthon-0.3.6/Quanthon.egg-info/requires.txt
--rw-r--r--   0 bukser     (501) staff       (20)        9 2024-04-24 11:09:56.000000 Quanthon-0.3.6/Quanthon.egg-info/top_level.txt
--rw-r--r--   0 bukser     (501) staff       (20)     1656 2024-04-22 07:53:30.000000 Quanthon-0.3.6/README.md
--rw-r--r--   0 bukser     (501) staff       (20)       38 2024-04-24 11:09:56.460316 Quanthon-0.3.6/setup.cfg
--rw-r--r--   0 bukser     (501) staff       (20)     1509 2024-04-22 07:50:01.000000 Quanthon-0.3.6/setup.py
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-24 11:09:56.459439 Quanthon-0.3.6/tests/
--rw-r--r--   0 bukser     (501) staff       (20)     4052 2024-04-09 23:49:00.000000 Quanthon-0.3.6/tests/test_cmp_qk.py
--rw-r--r--   0 bukser     (501) staff       (20)      626 2024-04-18 11:24:53.000000 Quanthon-0.3.6/tests/test_mappers.py
--rw-r--r--   0 bukser     (501) staff       (20)      173 2024-04-18 11:07:53.000000 Quanthon-0.3.6/tests/test_utils.py
--rw-r--r--   0 bukser     (501) staff       (20)     3784 2024-04-10 00:22:16.000000 Quanthon-0.3.6/tests/test_vqes.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-24 11:31:25.758010 quanthon-0.3.6.1/
+-rw-r--r--   0 bukser     (501) staff       (20)        0 2023-09-14 17:15:45.000000 quanthon-0.3.6.1/LICENSE
+-rw-r--r--   0 bukser     (501) staff       (20)     2521 2024-04-24 11:31:25.757793 quanthon-0.3.6.1/PKG-INFO
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-24 11:31:25.756160 quanthon-0.3.6.1/Quanthon/
+-rw-r--r--   0 bukser     (501) staff       (20)     3709 2024-03-04 09:48:46.000000 quanthon-0.3.6.1/Quanthon/Models.py
+-rw-r--r--   0 bukser     (501) staff       (20)      340 2024-04-22 07:48:46.000000 quanthon-0.3.6.1/Quanthon/__init__.py
+-rw-r--r--   0 bukser     (501) staff       (20)     6876 2024-04-10 00:56:44.000000 quanthon-0.3.6.1/Quanthon/algorithms.py
+-rw-r--r--   0 bukser     (501) staff       (20)     4727 2024-04-10 00:49:28.000000 quanthon-0.3.6.1/Quanthon/ansatzs.py
+-rw-r--r--   0 bukser     (501) staff       (20)    12033 2024-04-10 00:38:34.000000 quanthon-0.3.6.1/Quanthon/base.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5974 2024-04-03 18:36:12.000000 quanthon-0.3.6.1/Quanthon/expectation.py
+-rw-r--r--   0 bukser     (501) staff       (20)     4775 2024-04-24 11:29:34.000000 quanthon-0.3.6.1/Quanthon/mappers.py
+-rw-r--r--   0 bukser     (501) staff       (20)     6714 2024-04-24 11:09:39.000000 quanthon-0.3.6.1/Quanthon/mappers_utils.py
+-rw-r--r--   0 bukser     (501) staff       (20)      455 2024-04-18 10:41:02.000000 quanthon-0.3.6.1/Quanthon/physics.py
+-rw-r--r--   0 bukser     (501) staff       (20)     2302 2024-03-13 12:44:21.000000 quanthon-0.3.6.1/Quanthon/ut_pyscf_mel.py
+-rw-r--r--   0 bukser     (501) staff       (20)     1714 2024-03-18 22:32:17.000000 quanthon-0.3.6.1/Quanthon/ut_qiskit_hamiltonian.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5299 2024-03-21 16:15:37.000000 quanthon-0.3.6.1/Quanthon/ut_test_jw.py
+-rw-r--r--   0 bukser     (501) staff       (20)     6569 2024-04-18 11:08:36.000000 quanthon-0.3.6.1/Quanthon/utils.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-24 11:31:25.757545 quanthon-0.3.6.1/Quanthon.egg-info/
+-rw-r--r--   0 bukser     (501) staff       (20)     2521 2024-04-24 11:31:25.000000 quanthon-0.3.6.1/Quanthon.egg-info/PKG-INFO
+-rw-r--r--   0 bukser     (501) staff       (20)      557 2024-04-24 11:31:25.000000 quanthon-0.3.6.1/Quanthon.egg-info/SOURCES.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        1 2024-04-24 11:31:25.000000 quanthon-0.3.6.1/Quanthon.egg-info/dependency_links.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        6 2024-04-24 11:31:25.000000 quanthon-0.3.6.1/Quanthon.egg-info/requires.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        9 2024-04-24 11:31:25.000000 quanthon-0.3.6.1/Quanthon.egg-info/top_level.txt
+-rw-r--r--   0 bukser     (501) staff       (20)     1656 2024-04-22 07:53:30.000000 quanthon-0.3.6.1/README.md
+-rw-r--r--   0 bukser     (501) staff       (20)       38 2024-04-24 11:31:25.758051 quanthon-0.3.6.1/setup.cfg
+-rw-r--r--   0 bukser     (501) staff       (20)     1511 2024-04-24 11:30:56.000000 quanthon-0.3.6.1/setup.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-24 11:31:25.757378 quanthon-0.3.6.1/tests/
+-rw-r--r--   0 bukser     (501) staff       (20)     4052 2024-04-09 23:49:00.000000 quanthon-0.3.6.1/tests/test_cmp_qk.py
+-rw-r--r--   0 bukser     (501) staff       (20)      626 2024-04-18 11:24:53.000000 quanthon-0.3.6.1/tests/test_mappers.py
+-rw-r--r--   0 bukser     (501) staff       (20)      173 2024-04-18 11:07:53.000000 quanthon-0.3.6.1/tests/test_utils.py
+-rw-r--r--   0 bukser     (501) staff       (20)     3784 2024-04-10 00:22:16.000000 quanthon-0.3.6.1/tests/test_vqes.py
```

### Comparing `Quanthon-0.3.6/PKG-INFO` & `quanthon-0.3.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quanthon
-Version: 0.3.6
+Version: 0.3.6.1
 Summary: A quantum computing library
 Home-page: https://quanthon.readthedocs.io/
 Author: Keran Chen
 Author-email: keranc@uio.no
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Quanthon-0.3.6/Quanthon/Models.py` & `quanthon-0.3.6.1/Quanthon/Models.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.6/Quanthon/algorithms.py` & `quanthon-0.3.6.1/Quanthon/algorithms.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.6/Quanthon/ansatzs.py` & `quanthon-0.3.6.1/Quanthon/ansatzs.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.6/Quanthon/base.py` & `quanthon-0.3.6.1/Quanthon/base.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.6/Quanthon/expectation.py` & `quanthon-0.3.6.1/Quanthon/expectation.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.6/Quanthon/mappers.py` & `quanthon-0.3.6.1/Quanthon/mappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,14 @@
     if not is_hermitian(h_mat):
         raise ValueError("The Hamiltonian matrix is not Hermitian.")
     
     h_pauli = []
     
     if not is_power_of_two(h_mat.shape[0]):
         h_mat = expand_h_mat(h_mat)
-        print(h_mat)
         
     n = int(np.log2(h_mat.shape[0]))
     all_paulis = get_all_paulis(n)
     
     for paulis in all_paulis:
         coeff = (1/2**n) * np.trace(get_pauli(paulis) @ h_mat)
         if coeff != 0:
```

### Comparing `Quanthon-0.3.6/Quanthon/mappers_utils.py` & `quanthon-0.3.6.1/Quanthon/mappers_utils.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.6/Quanthon/ut_pyscf_mel.py` & `quanthon-0.3.6.1/Quanthon/ut_pyscf_mel.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.6/Quanthon/ut_qiskit_hamiltonian.py` & `quanthon-0.3.6.1/Quanthon/ut_qiskit_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.6/Quanthon/ut_test_jw.py` & `quanthon-0.3.6.1/Quanthon/ut_test_jw.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.6/Quanthon/utils.py` & `quanthon-0.3.6.1/Quanthon/utils.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.6/Quanthon.egg-info/PKG-INFO` & `quanthon-0.3.6.1/Quanthon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quanthon
-Version: 0.3.6
+Version: 0.3.6.1
 Summary: A quantum computing library
 Home-page: https://quanthon.readthedocs.io/
 Author: Keran Chen
 Author-email: keranc@uio.no
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Quanthon-0.3.6/Quanthon.egg-info/SOURCES.txt` & `quanthon-0.3.6.1/Quanthon.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 setup.py
-Quanthon/Expectation.py
 Quanthon/Models.py
 Quanthon/__init__.py
 Quanthon/algorithms.py
 Quanthon/ansatzs.py
 Quanthon/base.py
 Quanthon/expectation.py
 Quanthon/mappers.py
```

### Comparing `Quanthon-0.3.6/README.md` & `quanthon-0.3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.6/setup.py` & `quanthon-0.3.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
     
 #### VERSION HERE #####
-version = "0.3.6" #####
+version = "0.3.6.1" #####
 #######################    
 
 setup(
     name="Quanthon",
     version=version,
     description="A quantum computing library",
     long_description=long_description,
```

### Comparing `Quanthon-0.3.6/tests/test_cmp_qk.py` & `quanthon-0.3.6.1/tests/test_cmp_qk.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.6/tests/test_mappers.py` & `quanthon-0.3.6.1/tests/test_mappers.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.6/tests/test_vqes.py` & `quanthon-0.3.6.1/tests/test_vqes.py`

 * *Files identical despite different names*

