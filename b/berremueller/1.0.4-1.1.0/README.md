# Comparing `tmp/berremueller-1.0.4.tar.gz` & `tmp/berremueller-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "berremueller-1.0.4.tar", last modified: Tue Apr 23 22:25:04 2024, max compression
+gzip compressed data, was "berremueller-1.1.0.tar", last modified: Thu Apr 25 20:32:00 2024, max compression
```

## Comparing `berremueller-1.0.4.tar` & `berremueller-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 22:25:04.264253 berremueller-1.0.4/
--rw-rw-rw-   0        0        0    35823 2023-09-01 00:44:10.000000 berremueller-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1735 2024-04-23 22:25:04.262888 berremueller-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1347 2024-01-02 02:45:51.000000 berremueller-1.0.4/README.md
--rw-rw-rw-   0        0        0      475 2024-04-23 22:24:56.000000 berremueller-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-23 22:25:04.264253 berremueller-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0       41 2024-04-16 23:09:45.000000 berremueller-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 22:25:04.236427 berremueller-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-23 22:25:04.249103 berremueller-1.0.4/src/berremueller/
--rw-rw-rw-   0        0        0        2 2024-04-16 23:07:11.000000 berremueller-1.0.4/src/berremueller/__init__.py
--rw-rw-rw-   0        0        0    45413 2024-04-23 22:24:04.000000 berremueller-1.0.4/src/berremueller/berreman_mueller.py
--rw-rw-rw-   0        0        0     4818 2024-01-08 17:48:37.000000 berremueller-1.0.4/src/berremueller/cholesteric.py
--rw-rw-rw-   0        0        0    77860 2024-04-16 23:15:34.000000 berremueller-1.0.4/src/berremueller/dielectric_tensor.py
--rw-rw-rw-   0        0        0     3607 2024-01-10 20:46:11.000000 berremueller-1.0.4/src/berremueller/field_plotting.py
--rw-rw-rw-   0        0        0     3318 2023-12-13 19:38:52.000000 berremueller-1.0.4/src/berremueller/full_berreman.py
--rw-rw-rw-   0        0        0    60257 2024-04-17 20:54:46.000000 berremueller-1.0.4/src/berremueller/mueller.py
--rw-rw-rw-   0        0        0   157207 2024-04-16 23:15:34.000000 berremueller-1.0.4/src/berremueller/pyllama.py
--rw-rw-rw-   0        0        0     5071 2024-01-10 20:46:11.000000 berremueller-1.0.4/src/berremueller/python_util.py
-drwxrwxrwx   0        0        0        0 2024-04-23 22:25:04.262888 berremueller-1.0.4/src/berremueller.egg-info/
--rw-rw-rw-   0        0        0     1735 2024-04-23 22:25:04.000000 berremueller-1.0.4/src/berremueller.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      533 2024-04-23 22:25:04.000000 berremueller-1.0.4/src/berremueller.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 22:25:04.000000 berremueller-1.0.4/src/berremueller.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-23 22:25:04.000000 berremueller-1.0.4/src/berremueller.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-23 22:25:04.000000 berremueller-1.0.4/src/berremueller.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 20:32:00.041013 berremueller-1.1.0/
+-rw-rw-rw-   0        0        0    35823 2023-09-01 00:44:10.000000 berremueller-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1735 2024-04-25 20:32:00.041013 berremueller-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1347 2024-01-02 02:45:51.000000 berremueller-1.1.0/README.md
+-rw-rw-rw-   0        0        0      475 2024-04-24 21:48:26.000000 berremueller-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-25 20:32:00.042013 berremueller-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2024-04-16 23:09:45.000000 berremueller-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 20:31:59.944925 berremueller-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-25 20:32:00.022325 berremueller-1.1.0/src/berremueller/
+-rw-rw-rw-   0        0        0        2 2024-04-16 23:07:11.000000 berremueller-1.1.0/src/berremueller/__init__.py
+-rw-rw-rw-   0        0        0    45074 2024-04-24 21:52:56.000000 berremueller-1.1.0/src/berremueller/berreman_mueller.py
+-rw-rw-rw-   0        0        0     4818 2024-01-08 17:48:37.000000 berremueller-1.1.0/src/berremueller/cholesteric.py
+-rw-rw-rw-   0        0        0    77860 2024-04-16 23:15:34.000000 berremueller-1.1.0/src/berremueller/dielectric_tensor.py
+-rw-rw-rw-   0        0        0     3607 2024-01-10 20:46:11.000000 berremueller-1.1.0/src/berremueller/field_plotting.py
+-rw-rw-rw-   0        0        0     3318 2023-12-13 19:38:52.000000 berremueller-1.1.0/src/berremueller/full_berreman.py
+-rw-rw-rw-   0        0        0    64919 2024-04-25 19:46:12.000000 berremueller-1.1.0/src/berremueller/mueller.py
+-rw-rw-rw-   0        0        0   157207 2024-04-16 23:15:34.000000 berremueller-1.1.0/src/berremueller/pyllama.py
+-rw-rw-rw-   0        0        0     5071 2024-01-10 20:46:11.000000 berremueller-1.1.0/src/berremueller/python_util.py
+drwxrwxrwx   0        0        0        0 2024-04-25 20:32:00.040005 berremueller-1.1.0/src/berremueller.egg-info/
+-rw-rw-rw-   0        0        0     1735 2024-04-25 20:31:59.000000 berremueller-1.1.0/src/berremueller.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      533 2024-04-25 20:31:59.000000 berremueller-1.1.0/src/berremueller.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 20:31:59.000000 berremueller-1.1.0/src/berremueller.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-25 20:31:59.000000 berremueller-1.1.0/src/berremueller.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-25 20:31:59.000000 berremueller-1.1.0/src/berremueller.egg-info/top_level.txt
```

### Comparing `berremueller-1.0.4/LICENSE` & `berremueller-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `berremueller-1.0.4/PKG-INFO` & `berremueller-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berremueller
-Version: 1.0.4
+Version: 1.1.0
 Summary: A library for implementing the Berreman 4X4 matrix method alongside Mueller matrices
 Author-email: Andrew Salij <andrewsalij@gmail.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: scipy
```

### Comparing `berremueller-1.0.4/README.md` & `berremueller-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `berremueller-1.0.4/src/berremueller/berreman_mueller.py` & `berremueller-1.1.0/src/berremueller/berreman_mueller.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,26 +115,16 @@
     input_vector = input_vector**2 #conversion to intensity
     berre_dim = np.ndim(reflection_matrix)
     r_vec, t_vec = berre_dim_handling(berre_dim, reflection_matrix, transmission_matrix, input_vector)
     r_intensity = r_vec[0,...]+r_vec[1,...]
     t_intensity = t_vec[0,...]+t_vec[1,...]
     return r_intensity, t_intensity
 
-def kron_vectorized(a,b):
-    '''
-    kronecker product implmented so as to take advantage of numpy
-    vectorization when calculating a stack of products
-    Much faster than a for loop caclulating each stack
-    :param a: np.ndarray (shape (N,N,X))
-    :param b:  np.ndarray (shape (N,N,X))
-    :return:
-    '''
-    i,j,x = a.shape
-    k,l,y = b.shape
-    return np.einsum('ijx,klx->ikjlx',a,b).reshape(i*j,k*l,x)
+def kron_vectorized(matrix_a,matrix_b):
+    mueller.kron_vectorized(matrix_a,matrix_b)
 
 def stokes_from_jones_vector(jones_vector):
     '''
     Conversion of Jones vector to corresponding Stokes vector
     Eq. 3.30a in Ossikovski and Perez 2nd Ed, Polarized Light and the Mueller Matrix Approach
     Jones vector must be in the xy basis
     '''
```

### Comparing `berremueller-1.0.4/src/berremueller/cholesteric.py` & `berremueller-1.1.0/src/berremueller/cholesteric.py`

 * *Files identical despite different names*

### Comparing `berremueller-1.0.4/src/berremueller/dielectric_tensor.py` & `berremueller-1.1.0/src/berremueller/dielectric_tensor.py`

 * *Files identical despite different names*

### Comparing `berremueller-1.0.4/src/berremueller/field_plotting.py` & `berremueller-1.1.0/src/berremueller/field_plotting.py`

 * *Files identical despite different names*

### Comparing `berremueller-1.0.4/src/berremueller/full_berreman.py` & `berremueller-1.1.0/src/berremueller/full_berreman.py`

 * *Files identical despite different names*

### Comparing `berremueller-1.0.4/src/berremueller/mueller.py` & `berremueller-1.1.0/src/berremueller/mueller.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,30 @@
 import collections
 import warnings
 
 '''Numeric and symbolic handling of Mueller matrices with some plotting functions
 
 Andrew Salij'''
 
+def kron_vectorized(matrix_a,matrix_b):
+    '''
+    kronecker product implemented to take advantage of numpy
+    vectorization when calculating a stack of products
+    Much faster than a for loop caclulating each stack
+    :param a: np.ndarray (shape (N,N,X))
+    :param b:  np.ndarray (shape (N,N,X))
+    :return:
+    '''
+    i,j,x = matrix_a.shape
+    k,l,y = matrix_b.shape
+    return np.einsum('ijx,klx->ikjlx',matrix_a,matrix_b).reshape(i*j,k*l,x)
 def commute_matrix_stacks(matrix_a,matrix_b):
     '''
     Returns commutator of a matrix with a same shape stack of matrices
-    Designed for matrix to be magnus term after integration and stakc to be S term
+    Designed for matrix to be magnus term after integration to be S term
     :param matrix: np.ndarray (N,N) or (N,N,t)
     :param matrix_stack: np.ndarray (N,N) or (N,N,t)
     :return: np.ndarray (N,N,t)
     '''
     ab,ba = commute_handling(matrix_a,matrix_b)
     return np.squeeze(ab-ba)
 
@@ -138,22 +150,44 @@
     else:
         diff_matrix = np.array([[mean_abs,dichroism_vec[0],dichroism_vec[1],dichroism_vec[2]],
                                 [dichroism_vec[0],mean_abs,-biref_vec[2],biref_vec[1]],
                                 [dichroism_vec[1],biref_vec[2],mean_abs,-biref_vec[0]],
                                 [dichroism_vec[2],-biref_vec[1],biref_vec[0],mean_abs]])
     return diff_matrix
 
-def create_pauli_stack():
-    '''Provides stack of Pauli matrices'''
+def create_pauli_stack(convention_order = "optics"):
+    '''Provides stack of Pauli matrices
+    :param convention_order: str
+       "optics": [0, z, x, y]
+            used in optics literature such as https://doi.org/10.1117/12.202080
+       "xyz": [0, x, y, z]
+            more standard convention for quantum physics
+    return np.ndarray (2,2,4)
+    '''
     sigma_0 = np.array([[1,0],[0,1]])
     sigma_1 = np.array([[1,0],[0,-1]])
     sigma_2 = np.array([[0,1],[1,0]])
     sigma_3 = np.array([[0,-1j],[1j,0]])
-    return np.dstack((sigma_0,sigma_1,sigma_2,sigma_3))
-
+    if (convention_order == "optics"):
+        full_stack = np.dstack((sigma_0,sigma_1,sigma_2,sigma_3))
+    elif (convention_order == "xyz"):
+        full_stack = np.dstack((sigma_0,sigma_2,sigma_3,sigma_1))
+    else: raise ValueError("Invalid convention_order")
+    return full_stack
+
+def create_G_matrix_stack():
+    '''
+    Provides the stack of G matrices ((5.3) in Gil and Ossikovski, Polarized Light and the Mueller Matrix Approach)
+    :return:
+    '''
+    g_0 = np.array([[1,0,0,0],[0,1,0,0],[0,0,1,0],[0,0,0,1]])
+    g_1 = np.array([[0,1,0,0],[1,0,0,0],[0,0,0,1j],[0,0,-1j,0]])
+    g_2 = np.array([[0,0,1,0],[0,0,0,-1j],[1,0,0,0],[0,1j,0,0]])
+    g_3 = np.array([0,0,0,1],[0,0,1j,0],[0,-1j,0,0],[1,0,0,0])
+    return np.dstack((g_0,g_1,g_2,g_3))
 #b_vec and d_vec in terms of (mean,linear, linear prime, circular)
 #let b_vec and d_vec 0 components be 0 to only get polarization-dependent behavior
 class JONES_MATRIX():
     '''Handles (2 X 2) Jones matrices'''
     def __init__(self,b_vec,d_vec):
         '''
         :param b_vec: np.ndarray (LB,LBP,CB)
@@ -475,14 +509,69 @@
     :return: np.ndarray (4D) ; antisymmetric matrix, symmetric matrix stacked along final axis
     '''
     m = mueller_matrix_stack
     m_s = 0.5*(m+np.transpose(m,(1,0,2)))
     m_a = 0.5*(m-np.transpose(m,(1,0,2)))
     return np.stack((m_a,m_s),axis =-1)
 
+def mueller_from_coherency_matrix(coherency_matrix):
+    '''
+    Directly gives the analytic expression for the Mueller matrix in terms of the coherency matrix
+    5.14 in Gil and Ossikovski
+    :param coherency_matrix: np.ndarray (4,4)
+    :return:
+    '''
+    g_stack = create_G_matrix_stack()
+    mueller_matrix = np.zeros((4,4),dtype = coherency_matrix.dtype)
+    #TODO: write this in a faster way
+    for i in range(4):#there has to be a more efficient way of doing this
+        for j in range(4):
+            mueller_matrix[i,j] = np.trace((np.dot(np.conjugate(g_stack[:,:,i],
+                                                                np.dot(g_stack[:,:,j],coherency_matrix)))))
+    assert np.isclose(mueller_matrix[0,0],np.trace(coherency_matrix)), "M_00 must be equal to trace of coherency matrix"
+    return mueller_matrix
+def cloude_decompose_matrix_stack(mueller_matrix_stack):
+    '''
+    Decomposes a stack of matrices (4,4,X) into non depolarizing and depolarizing parts
+    See (17)-(19) in https://doi.org/10.1364/OL.37.000220
+    see Section 5.3 in Gil and Ossikovski, Polarized Light and the Mueller Matrix Approach, 2nd ed. 
+    :param mueller_matrix_stack:
+    :return: np.ndarray (4,4,X)
+    '''
+    matrix_shape = np.shape(mueller_matrix_stack)
+    assert matrix_shape[0] == 4 and matrix_shape[1] == 4, "Axes 0 and 1 must be (4,4)"
+    pauli_stack = create_pauli_stack(convention_order="xyz")
+    covariance_matrix = np.zeros(matrix_shape,dtype=mueller_matrix_stack.dtype)
+    for i in range(4):
+        for j in range(4):
+            covariance_term = 1/4*np.kron(pauli_stack[:,:,i],np.conjugate(pauli_stack[:,:,j]))
+            covariance_matrix = covariance_matrix+mueller_matrix_stack[i,j,:]*covariance_term
+    assert np.isclose(np.trace(covariance_matrix[:,:,0]),mueller_matrix_stack[0,0,0]), "Covariance matrix trace must equal M_00"
+    l_matrix = 1/np.sqrt(2) * \
+            np.array([[1, 0, 0, 1],
+                      [1, 0, 0, -1],
+                      [0, 1, 1, 0],
+                      [0, 1j, -1j, 0]])
+    coherency_matrix = np.einsum("ij,jkl->ikl",l_matrix, #5.13 in Gil and Ossikovski, C(M) in their notation
+                                  np.einsum("ijl,jk->ikl",covariance_matrix,np.conjugate(np.transpose(l_matrix))))
+    coherency_decomposition_matrix =  np.zeros((4,4,4,matrix_shape[2]),dtype=mueller_matrix_stack.dtype)
+    for x in range(matrix_shape[2]):
+        c_vals, c_vecs = np.linalg.eig(coherency_matrix[:,:,x])
+        idx = (-1*c_vals).argsort()
+        c_vals = c_vals[idx]
+        c_vecs = c_vecs[:,idx] #sorted greatest to least
+        for i in range(4):
+            projection_matrix = np.outer(c_vecs[:,i],np.conj(c_vecs[:,i]))
+            coherency_decomposition_matrix[:,:,i,x] = c_vals[i]*projection_matrix #sorted greatest to least
+    mueller_decomposition_matrix = np.zeros((4,4,4,matrix_shape[2]),dtype=mueller_matrix_stack.dtype)
+    for x in range(matrix_shape[2]):
+        for i in range(4):
+            mueller_decomposition_matrix[:,:,i,x] = mueller_from_coherency_matrix(coherency_decomposition_matrix[:,:,i,x])
+    return mueller_decomposition_matrix
+
 def extract_elem_mm_stack(mueller_matrix_stack,index = [0,3]):
     '''
     :param mueller_matrix_stack: np.ndarray (3D)
     :param index: MM elem index to extract--defaults to m_03 (CD)
     :return: mueller_matrix_elem
     '''
     mueller_matrix_elem = mueller_matrix_stack[index[0],index[1],:]
```

### Comparing `berremueller-1.0.4/src/berremueller/pyllama.py` & `berremueller-1.1.0/src/berremueller/pyllama.py`

 * *Files identical despite different names*

### Comparing `berremueller-1.0.4/src/berremueller/python_util.py` & `berremueller-1.1.0/src/berremueller/python_util.py`

 * *Files identical despite different names*

### Comparing `berremueller-1.0.4/src/berremueller.egg-info/PKG-INFO` & `berremueller-1.1.0/src/berremueller.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berremueller
-Version: 1.0.4
+Version: 1.1.0
 Summary: A library for implementing the Berreman 4X4 matrix method alongside Mueller matrices
 Author-email: Andrew Salij <andrewsalij@gmail.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: scipy
```

### Comparing `berremueller-1.0.4/src/berremueller.egg-info/SOURCES.txt` & `berremueller-1.1.0/src/berremueller.egg-info/SOURCES.txt`

 * *Files identical despite different names*

