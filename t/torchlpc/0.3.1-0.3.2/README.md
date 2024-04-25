# Comparing `tmp/torchlpc-0.3.1.tar.gz` & `tmp/torchlpc-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchlpc-0.3.1.tar", last modified: Mon Jan  1 00:20:18 2024, max compression
+gzip compressed data, was "torchlpc-0.3.2.tar", last modified: Thu Apr 25 10:53:04 2024, max compression
```

## Comparing `torchlpc-0.3.1.tar` & `torchlpc-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 00:20:18.497894 torchlpc-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-01-01 00:20:03.000000 torchlpc-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-01-01 00:20:18.497894 torchlpc-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-01-01 00:20:03.000000 torchlpc-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-01 00:20:18.497894 torchlpc-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-01-01 00:20:03.000000 torchlpc-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 00:20:18.497894 torchlpc-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-01-01 00:20:03.000000 torchlpc-0.3.1/tests/test_grad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 00:20:18.497894 torchlpc-0.3.1/torchlpc/
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-01-01 00:20:03.000000 torchlpc-0.3.1/torchlpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-01-01 00:20:03.000000 torchlpc-0.3.1/torchlpc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 00:20:18.497894 torchlpc-0.3.1/torchlpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-01-01 00:20:18.000000 torchlpc-0.3.1/torchlpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-01 00:20:18.000000 torchlpc-0.3.1/torchlpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-01 00:20:18.000000 torchlpc-0.3.1/torchlpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-01 00:20:18.000000 torchlpc-0.3.1/torchlpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-01 00:20:18.000000 torchlpc-0.3.1/torchlpc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:53:04.293304 torchlpc-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-25 10:53:00.000000 torchlpc-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-25 10:53:04.293304 torchlpc-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-25 10:53:00.000000 torchlpc-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 10:53:04.293304 torchlpc-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-25 10:53:00.000000 torchlpc-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:53:04.289304 torchlpc-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-25 10:53:00.000000 torchlpc-0.3.2/tests/test_grad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:53:04.289304 torchlpc-0.3.2/torchlpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-25 10:53:00.000000 torchlpc-0.3.2/torchlpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-04-25 10:53:00.000000 torchlpc-0.3.2/torchlpc/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:53:04.293304 torchlpc-0.3.2/torchlpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-25 10:53:04.000000 torchlpc-0.3.2/torchlpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-25 10:53:04.000000 torchlpc-0.3.2/torchlpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 10:53:04.000000 torchlpc-0.3.2/torchlpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 10:53:04.000000 torchlpc-0.3.2/torchlpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 10:53:04.000000 torchlpc-0.3.2/torchlpc.egg-info/top_level.txt
```

### Comparing `torchlpc-0.3.1/LICENSE` & `torchlpc-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torchlpc-0.3.1/setup.py` & `torchlpc-0.3.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 NAME = "torchlpc"
-VERSION = "0.3.1"
+VERSION = "0.3.2"
 MAINTAINER = "Chin-Yun Yu"
 EMAIL = "chin-yun.yu@qmul.ac.uk"
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
```

### Comparing `torchlpc-0.3.1/tests/test_grad.py` & `torchlpc-0.3.2/tests/test_grad.py`

 * *Files identical despite different names*

### Comparing `torchlpc-0.3.1/torchlpc/__init__.py` & `torchlpc-0.3.2/torchlpc/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlpc-0.3.1/torchlpc/core.py` & `torchlpc-0.3.2/torchlpc/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -176,14 +176,20 @@
         if ctx.needs_input_grad[1]:
             valid_y = y[:, :-1]
             padded_y = torch.cat([zi.flip(1), valid_y], dim=1)
 
             unfolded_y = padded_y.unfold(1, order, 1).flip(2)
             grad_A = unfolded_y * -flipped_grad_x.flip(1).unsqueeze(2)
 
+        if hasattr(ctx, "y"):
+            del ctx.y
+        if hasattr(ctx, "A"):
+            del ctx.A
+        if hasattr(ctx, "zi"):
+            del ctx.zi
         return grad_x, grad_A, grad_zi
 
     @staticmethod
     def jvp(
         ctx: Any, grad_x: torch.Tensor, grad_A: torch.Tensor, grad_zi: torch.Tensor
     ) -> torch.Tensor:
         A, y, zi = ctx.A, ctx.y, ctx.zi
@@ -195,8 +201,9 @@
         if grad_A is not None:
             unfolded_y = (
                 torch.cat([zi.flip(1), y[:, :-1]], dim=1).unfold(1, order, 1).flip(2)
             )
             fwd_A = -torch.sum(unfolded_y * grad_A, dim=2)
             fwd_x = fwd_x + fwd_A
 
+        del ctx.y, ctx.A, ctx.zi
         return LPC.apply(fwd_x, A, fwd_zi)
```

