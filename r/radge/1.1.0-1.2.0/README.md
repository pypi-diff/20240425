# Comparing `tmp/radge-1.1.0.tar.gz` & `tmp/radge-1.2.0.tar.gz`

## Comparing `radge-1.1.0.tar` & `radge-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 radge-1.1.0/requirements.txt
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 radge-1.1.0/radge/__init__.py
--rw-r--r--   0        0        0     8580 2020-02-02 00:00:00.000000 radge-1.1.0/radge/graph.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 radge-1.1.0/radge/numbers.py
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 radge-1.1.0/radge/polygon.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 radge-1.1.0/radge/sequences.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 radge-1.1.0/radge/string.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 radge-1.1.0/radge/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 radge-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 radge-1.1.0/tests/test_graph.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 radge-1.1.0/tests/test_numbers.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 radge-1.1.0/tests/test_polygon.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 radge-1.1.0/tests/test_sequences.py
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 radge-1.1.0/tests/test_string.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 radge-1.1.0/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 radge-1.1.0/LICENSE
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 radge-1.1.0/README.md
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 radge-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 radge-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 radge-1.2.0/requirements.txt
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 radge-1.2.0/radge/__init__.py
+-rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 radge-1.2.0/radge/graph.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 radge-1.2.0/radge/numbers.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 radge-1.2.0/radge/polygon.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 radge-1.2.0/radge/sequences.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 radge-1.2.0/radge/string.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 radge-1.2.0/radge/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 radge-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 radge-1.2.0/tests/test_graph.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 radge-1.2.0/tests/test_numbers.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 radge-1.2.0/tests/test_polygon.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 radge-1.2.0/tests/test_seed.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 radge-1.2.0/tests/test_sequences.py
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 radge-1.2.0/tests/test_string.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 radge-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 radge-1.2.0/LICENSE
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 radge-1.2.0/README.md
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 radge-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 radge-1.2.0/PKG-INFO
```

### Comparing `radge-1.1.0/radge/graph.py` & `radge-1.2.0/radge/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 Generate graphs with various properties, including trees.
 """
 
 import math
 import random
 from typing import Callable, Optional
 
-from .utils import NOISE
-
+import radge.utils as utils
 
 class Edge:
     """Edge between two vertices."""
 
-    def __init__(self, u: int, v: int, w: Optional[int] = None):
+    def __init__(self, u: int, v: int, w: Optional[int] = None) -> None:
         self.u = u
         self.v = v
         self.w = w
 
     def __str__(self) -> str:
         """Return the edge as a string."""
         return f"{self.u} {self.v}" + (f" {self.w}" if self.w else "")
@@ -26,23 +25,24 @@
     """Vertices connected by edges."""
 
     def __init__(
         self,
         vertex_cnt: int,
         weight_func: Optional[Callable[[], int]] = None,
         directed: bool = False,
-    ):
+    ) -> None:
         """Initialize a graph."""
         self.vertex_cnt = vertex_cnt
         self.weight_func = weight_func
         self.directed = directed
 
         self.edge_cnt = 0
         self.edges = [[] for _ in range(vertex_cnt + 1)]
         perm = list(range(1, vertex_cnt + 1))
+        random.seed(utils.SEED)
         random.shuffle(perm)
         self.perm = [0] + perm
 
     def permute_edge(self, edge: Edge) -> str:
         """Return the edge with vertices permuted."""
         split = str(edge).split()
         coin = random.randint(0, 1) if not self.directed else 1
@@ -61,15 +61,15 @@
                 # to avoid duplicates in undirected graphs
                 if self.directed or (not self.directed and edge.u <= edge.v):
                     ret.append(self.permute_edge(edge))
         random.shuffle(ret)
 
         return "\n".join(ret)
 
-    def add_edge(self, u: int, v: int):
+    def add_edge(self, u: int, v: int) -> None:
         """Add an edge u-v (and v-u if the graph is undirected)."""
         self.edge_cnt += 1
         w = self.weight_func() if self.weight_func else None
         self.edges[u].append(Edge(u, v, w))
         if not self.directed:
             self.edges[v].append(Edge(v, u, w))
 
@@ -156,16 +156,16 @@
 def comb_tree(
     vertex_cnt: int, weight_func: Optional[Callable[[], int]] = None
 ) -> Graph:
     """Return a 'comb' tree (trunk with ~sqrt(n) vertices, of which each one has a ~sqrt(n)-long branch) with vertex_cnt vertices."""
 
     def approx_sqrt(n: int) -> int:
         s = int(math.sqrt(n))
-        if s > NOISE and s < n - NOISE:
-            return s + random.randint(-NOISE, NOISE)
+        if s > utils.NOISE and s < n - utils.NOISE:
+            return s + random.randint(-utils.NOISE, utils.NOISE)
 
         return s
 
     tree = Graph(vertex_cnt, weight_func=weight_func)
     trunk_len = approx_sqrt(vertex_cnt)
     for i in range(2, trunk_len + 1):
         tree.add_edge(i, i - 1)
```

### Comparing `radge-1.1.0/radge/numbers.py` & `radge-1.2.0/radge/numbers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,64 @@
 """
 Generate numbers with desired properties
 """
 
 import math
 import random
+import radge.utils as utils
 
 
-class Numbers:
-    """Numbers: a class handling the generation of numbers."""
-
-    def __init__(self, max_n: int):
-        """Initialize the generator."""
-        self.max_n = max_n
-
-    def random_prime(self) -> int:
-        """Generate a random prime number not greater than max_n using the Miller-Rabin primality test."""
-
-        def mpow(a: int, b: int, m: int) -> int:
-            """Modular exponentiation."""
-            res = 1
-            while b > 0:
-                if b % 2 == 1:
-                    res = (res * a) % m
-                a = (a * a) % m
-                b //= 2
-
-            return res
-
-        def miller_rabin(n: int) -> bool:
-            """Miller-Rabin primality test."""
-
-            def is_composite(n: int, a: int, q: int, s: int) -> bool:
-                x = mpow(a, q, n)
-                if x == 1 or x == n - 1:
+def mpow(a: int, b: int, m: int) -> int:
+    """Modular exponentiation."""
+    res = 1
+    while b > 0:
+        if b % 2 == 1:
+            res = (res * a) % m
+        a = (a * a) % m
+        b //= 2
+
+    return res
+
+
+def random_prime(max_n: int) -> int:
+    """Generate a random prime number not greater than max_n."""
+
+    def miller_rabin(n: int) -> bool:
+        """Miller-Rabin primality test."""
+
+        def is_composite(n: int, a: int, q: int, s: int) -> bool:
+            x = mpow(a, q, n)
+            if x == 1 or x == n - 1:
+                return False
+            for _ in range(1, s):
+                x = (x * x) % n
+                if x == n - 1:
                     return False
-                for _ in range(1, s):
-                    x = (x * x) % n
-                    if x == n - 1:
-                        return False
 
-                return True
+            return True
 
-            if n == 2 or n == 3:
-                return True
+        if n == 2 or n == 3:
+            return True
 
-            s = 0
-            q = n - 1
-            while q % 2 == 0:
-                q //= 2
-                s += 1
-
-            for a in [2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37]:
-                if n == a:
-                    return True
-                if is_composite(n, a, q, s):
-                    return False
+        s = 0
+        q = n - 1
+        while q % 2 == 0:
+            q //= 2
+            s += 1
 
-            return True
+        for a in [2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37]:
+            if n == a:
+                return True
+            if is_composite(n, a, q, s):
+                return False
+
+        return True
 
-        bound, iters = 10 * int(math.log(self.max_n)), 0
-        while iters < bound:
-            n = random.randint(2, self.max_n)
-            if miller_rabin(n):
-                return n
-            iters += 1
+    random.seed(utils.SEED)
+    bound, iters = 10 * int(math.log(max_n)), 0
+    while iters < bound:
+        n = random.randint(2, max_n)
+        if miller_rabin(n):
+            return n
+        iters += 1
 
-        return 2
+    return 2
```

### Comparing `radge-1.1.0/radge/polygon.py` & `radge-1.2.0/radge/polygon.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 Generate convex polygons.
 """
 
 import math
 import random
 from typing import List
 
-from .utils import PI, EXP, NOISE
-
+import radge.utils as utils
 
 class Vector:
     """Vector in the cartesian plane."""
 
     def __init__(self, x: int, y: int):
         self.x = x
         self.y = y
@@ -44,20 +43,21 @@
         """Return the norm of the vector."""
         return math.sqrt(self.x**2 + self.y**2)
 
     def angle(self) -> float:
         """Return the directed angle (in radians) that the vector makes with the X-axis."""
         return math.atan2(self.y, self.x)
 
-
+# TODO: change this to finding the convex hull of a random set of points.
 def random_convex(n: int, max_coord: int = 1000) -> List[Vector]:
     """Return a random convex polygon with n >= 3 vertices, such that none of its vertices have a coordinate bigger than max_coord."""
     # note: degenerate polygons are possible (for example a "triangle" with 3 colinear points)
     if n < 3:
         raise ValueError("n must be at least 3")
+    random.seed(utils.SEED)
     max_r = random.randint(2, 2 + max_coord // n)
 
     vecs = []
     cur = Vector(0, 0)
     for _ in range(n - 1):
         new_p = cur
         while new_p == cur:
@@ -66,14 +66,14 @@
                 random.randint(cur.y - max_r, cur.y + max_r),
             )
         vecs.append(new_p - cur)
         cur = new_p
     vecs.append(-cur)
     vecs.sort(key=lambda v: v.angle())
 
-    start = Vector(random.randint(-NOISE, NOISE), random.randint(-NOISE, NOISE))
+    start = Vector(random.randint(-utils.NOISE, utils.NOISE), random.randint(-utils.NOISE, utils.NOISE))
     points = [start]
     for vec in vecs:
         points.append(points[-1] + vec)
     points.pop()
 
     return points
```

### Comparing `radge-1.1.0/radge/sequences.py` & `radge-1.2.0/radge/sequences.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
 Sequences, permutations and so on.
 """
 
 import random
 from typing import Any, Callable, Optional
+import radge.utils as utils
 
 
 def seq(n: int, a: range, key: Optional[Callable[[int], Any]] = None) -> list:
     """Pick n random items from range a (possibly with repetitions).
     Optionally sort the resulting sequence using the key(x) function
     (takes in x, and returns the value that x should be compared by)."""
+    random.seed(utils.SEED)
     ret = [random.choice(a) for _ in range(n)]
     random.shuffle(ret)
     if key:
         ret.sort(key=key)
     return ret
 
 
@@ -21,23 +23,25 @@
     """Pick n unique random items from range a.
     Optionally sort the resulting sequence using the key(x) function
     (takes in x, and returns the value that x should be compared by)."""
     if len(a) < n:
         raise IndexError(
             f"Can't pick {n} distinct elements from a range of length {len(a)}."
         )
+    random.seed(utils.SEED)
     ret = random.sample(a, n)
     if key:
         ret.sort(key=key)
     return ret
 
 
 def perm(n: int, key: Optional[Callable[[int], Any]] = None) -> list:
     """Return a random permutatation of the set {1,2,...,n}.
     Optionally sort the resulting sequence using the key(x) function
     (takes in x, and returns the value that x should be compared by)."""
+    random.seed(utils.SEED)
     ret = list(range(1, n + 1))
     if key:
         ret.sort(key=key)
     else:
         random.shuffle(ret)
     return ret
```

### Comparing `radge-1.1.0/radge/string.py` & `radge-1.2.0/radge/string.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 Generate various types of strings.
 """
 
 import random
 
-from .utils import ALPHA_LOWER, ALPHA_UPPER
+import radge.utils as utils
 
 
 class String:
     """A string made using characters from the given alphabet."""
 
-    def __init__(self, len: int, alpha: str = ALPHA_LOWER + ALPHA_UPPER):
+    def __init__(self, len: int, alpha: str = utils.ALPHA_LOWER + utils.ALPHA_UPPER) -> None:
+        random.seed(utils.SEED)
         self.len = len
         self.alpha = alpha
         self.s = "".join(random.choice(alpha) for _ in range(len))
 
     def __str__(self) -> str:
         """Return the string."""
         return self.s
```

### Comparing `radge-1.1.0/tests/test_graph.py` & `radge-1.2.0/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `radge-1.1.0/tests/test_numbers.py` & `radge-1.2.0/tests/test_polygon.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-import math
+import random
 import unittest
 
-from radge.numbers import *
+from radge.polygon import *
 
-TESTS = 1000
-MAX_N = 1_000_000_000
 
+def is_convex_angle(v: Vector, w: Vector) -> bool:
+    return v.x * w.y - v.y * w.x >= 0
 
-class TestNumbers(unittest.TestCase):
-    def test_random_prime(self):
-        """Test if the generated number is a prime."""
-        num_gen = Numbers(MAX_N)
-        for i in range(TESTS):
-            random.seed(i)
-            p = num_gen.random_prime()
-            self.assertTrue(p > 1)
-            self.assertTrue(p < MAX_N)
-            self.assertTrue(all(p % i != 0 for i in range(2, math.isqrt(p) + 1)))
 
-
-if __name__ == "__main__":
-    unittest.main(failfast=True)
+class TestPolygon(unittest.TestCase):
+    def test_convex(self):
+        """Test if the generated polygon is convex."""
+        TESTS = 1000
+        MAX_N = 1000
+
+        for test in range(TESTS):
+            random.seed(test)
+            n = random.randint(3, MAX_N)
+            poly = random_convex(n)
+            v = poly[1] - poly[0]
+            for i in range(2, n):
+                w = poly[i] - poly[i - 1]
+                self.assertTrue(is_convex_angle(v, w))
+                v = w
```

### Comparing `radge-1.1.0/tests/test_sequences.py` & `radge-1.2.0/tests/test_sequences.py`

 * *Files identical despite different names*

### Comparing `radge-1.1.0/tests/test_string.py` & `radge-1.2.0/tests/test_string.py`

 * *Files identical despite different names*

### Comparing `radge-1.1.0/.gitignore` & `radge-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `radge-1.1.0/LICENSE` & `radge-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `radge-1.1.0/README.md` & `radge-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `radge-1.1.0/PKG-INFO` & `radge-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: radge
-Version: 1.1.0
+Version: 1.2.0
 Summary: A random algorithmic data generator
 Author-email: Antoni Zasada <zsd.antoni@gmail.com>
 License-File: LICENSE
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Radge - Random algorithmic data generator
```

