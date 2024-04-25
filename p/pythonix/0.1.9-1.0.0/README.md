# Comparing `tmp/pythonix-0.1.9.tar.gz` & `tmp/pythonix-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonix-0.1.9.tar", max compression
+gzip compressed data, was "pythonix-1.0.0.tar", max compression
```

## Comparing `pythonix-0.1.9.tar` & `pythonix-1.0.0.tar`

### file list

```diff
@@ -1,51 +1,32 @@
--rwxr-xr-x   0        0        0      296 2024-01-26 16:30:26.709984 pythonix-0.1.9/pyproject.toml
--rwxr-xr-x   0        0        0        0 2024-01-24 16:26:09.556393 pythonix-0.1.9/pythonix/__init__.py
--rwxr-xr-x   0        0        0        0 2024-01-24 16:25:23.590016 pythonix-0.1.9/pythonix/result/__init__.py
--rwxr-xr-x   0        0        0      144 2024-01-24 16:25:23.678120 pythonix-0.1.9/pythonix/result/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      168 2024-01-24 17:00:06.039380 pythonix-0.1.9/pythonix/result/__pycache__/__init__.cpython-312.pyc
--rwxr-xr-x   0        0        0     5627 2024-01-24 16:25:23.704839 pythonix-0.1.9/pythonix/result/__pycache__/containers.cpython-310.pyc
--rwxr-xr-x   0        0        0     9049 2024-01-25 15:40:51.485350 pythonix-0.1.9/pythonix/result/__pycache__/containers.cpython-312.pyc
--rwxr-xr-x   0        0        0     2234 2024-01-25 15:40:51.438010 pythonix-0.1.9/pythonix/result/__pycache__/decorators.cpython-312.pyc
--rwxr-xr-x   0        0        0     1050 2024-01-24 16:25:23.788808 pythonix-0.1.9/pythonix/result/__pycache__/errors.cpython-310.pyc
--rwxr-xr-x   0        0        0     1325 2024-01-24 17:00:06.176217 pythonix-0.1.9/pythonix/result/__pycache__/errors.cpython-312.pyc
--rwxr-xr-x   0        0        0     3246 2024-01-24 16:25:23.754076 pythonix-0.1.9/pythonix/result/__pycache__/funcs.cpython-310.pyc
--rwxr-xr-x   0        0        0     5615 2024-01-25 15:40:51.729272 pythonix-0.1.9/pythonix/result/__pycache__/funcs.cpython-312.pyc
--rwxr-xr-x   0        0        0     1512 2024-01-24 17:00:06.226250 pythonix-0.1.9/pythonix/result/__pycache__/suffixes.cpython-312.pyc
--rwxr-xr-x   0        0        0     4481 2024-01-25 15:39:50.755008 pythonix-0.1.9/pythonix/result/containers.py
--rwxr-xr-x   0        0        0      943 2024-01-25 15:39:50.541925 pythonix-0.1.9/pythonix/result/decorators.py
--rwxr-xr-x   0        0        0      316 2024-01-24 16:25:23.576010 pythonix-0.1.9/pythonix/result/errors.py
--rwxr-xr-x   0        0        0     2313 2024-01-25 15:39:50.655022 pythonix-0.1.9/pythonix/result/funcs.py
--rwxr-xr-x   0        0        0      810 2024-01-24 16:30:13.437044 pythonix-0.1.9/pythonix/result/suffixes.py
--rwxr-xr-x   0        0        0     1891 2024-01-26 16:30:10.713544 pythonix-0.1.9/pythonix/suffix_types.py
--rwxr-xr-x   0        0        0        0 2024-01-24 16:25:24.360304 pythonix-0.1.9/pythonix/suffixes/__init__.py
--rwxr-xr-x   0        0        0      170 2024-01-24 17:00:06.369640 pythonix-0.1.9/pythonix/suffixes/__pycache__/__init__.cpython-312.pyc
--rwxr-xr-x   0        0        0      151 2024-01-24 16:25:24.281154 pythonix-0.1.9/pythonix/suffixes/__pycache__/functools.cpython-312.pyc
--rwxr-xr-x   0        0        0      806 2024-01-24 16:25:24.329218 pythonix-0.1.9/pythonix/suffixes/__pycache__/itertools.cpython-312.pyc
--rwxr-xr-x   0        0        0     1894 2024-01-24 16:25:24.305176 pythonix-0.1.9/pythonix/suffixes/__pycache__/operators.cpython-312.pyc
--rwxr-xr-x   0        0        0        0 2024-01-24 16:25:24.504115 pythonix-0.1.9/pythonix/suffixes/builtins/__init__.py
--rwxr-xr-x   0        0        0      179 2024-01-24 17:00:06.863214 pythonix-0.1.9/pythonix/suffixes/builtins/__pycache__/__init__.cpython-312.pyc
--rwxr-xr-x   0        0        0      942 2024-01-25 15:40:51.886839 pythonix-0.1.9/pythonix/suffixes/builtins/__pycache__/conversion.cpython-312.pyc
--rwxr-xr-x   0        0        0     1758 2024-01-24 20:41:45.512810 pythonix-0.1.9/pythonix/suffixes/builtins/__pycache__/io.cpython-312.pyc
--rwxr-xr-x   0        0        0      537 2024-01-24 20:47:45.261074 pythonix-0.1.9/pythonix/suffixes/builtins/__pycache__/mathematical.cpython-312.pyc
--rwxr-xr-x   0        0        0      533 2024-01-25 15:40:49.936779 pythonix-0.1.9/pythonix/suffixes/builtins/conversion.py
--rwxr-xr-x   0        0        0      417 2024-01-26 16:04:35.411688 pythonix-0.1.9/pythonix/suffixes/builtins/iterable.py
--rwxr-xr-x   0        0        0      258 2024-01-24 20:47:43.195828 pythonix-0.1.9/pythonix/suffixes/builtins/mathematical.py
--rwxr-xr-x   0        0        0     1542 2024-01-26 16:27:11.916051 pythonix-0.1.9/pythonix/suffixes/itertools/__pycache__/combinatoric.cpython-312.pyc
--rwxr-xr-x   0        0        0     1366 2024-01-26 16:06:53.659554 pythonix-0.1.9/pythonix/suffixes/itertools/__pycache__/infinite.cpython-312.pyc
--rwxr-xr-x   0        0        0     5138 2024-01-26 16:27:11.997102 pythonix-0.1.9/pythonix/suffixes/itertools/__pycache__/terminating.cpython-312.pyc
--rwxr-xr-x   0        0        0      681 2024-01-26 16:16:37.321812 pythonix-0.1.9/pythonix/suffixes/itertools/combinatoric.py
--rwxr-xr-x   0        0        0      610 2024-01-26 16:06:51.651105 pythonix-0.1.9/pythonix/suffixes/itertools/infinite.py
--rwxr-xr-x   0        0        0     2390 2024-01-26 16:16:37.376284 pythonix-0.1.9/pythonix/suffixes/itertools/terminating.py
--rwxr-xr-x   0        0        0        0 2024-01-24 16:25:24.052685 pythonix-0.1.9/pythonix/suffixes/operators/__init__.py
--rwxr-xr-x   0        0        0      180 2024-01-24 17:00:06.594874 pythonix-0.1.9/pythonix/suffixes/operators/__pycache__/__init__.cpython-312.pyc
--rwxr-xr-x   0        0        0     2144 2024-01-25 15:40:51.611092 pythonix-0.1.9/pythonix/suffixes/operators/__pycache__/class_utils.cpython-312.pyc
--rwxr-xr-x   0        0        0     1581 2024-01-25 15:40:51.571337 pythonix-0.1.9/pythonix/suffixes/operators/__pycache__/comparison.cpython-312.pyc
--rwxr-xr-x   0        0        0     1612 2024-01-25 15:40:51.529358 pythonix-0.1.9/pythonix/suffixes/operators/__pycache__/logical.cpython-312.pyc
--rwxr-xr-x   0        0        0     8176 2024-01-26 16:11:44.040334 pythonix-0.1.9/pythonix/suffixes/operators/__pycache__/mathematical.cpython-312.pyc
--rwxr-xr-x   0        0        0     3947 2024-01-25 15:40:51.650290 pythonix-0.1.9/pythonix/suffixes/operators/__pycache__/sequence.cpython-312.pyc
--rwxr-xr-x   0        0        0     1001 2024-01-25 15:39:50.591321 pythonix-0.1.9/pythonix/suffixes/operators/class_utils.py
--rwxr-xr-x   0        0        0      627 2024-01-25 15:39:50.565198 pythonix-0.1.9/pythonix/suffixes/operators/comparison.py
--rwxr-xr-x   0        0        0      695 2024-01-25 15:39:50.595857 pythonix-0.1.9/pythonix/suffixes/operators/logical.py
--rwxr-xr-x   0        0        0     3665 2024-01-26 16:11:42.354222 pythonix-0.1.9/pythonix/suffixes/operators/mathematical.py
--rwxr-xr-x   0        0        0     1980 2024-01-25 15:39:50.732233 pythonix-0.1.9/pythonix/suffixes/operators/sequence.py
--rw-r--r--   0        0        0      342 1970-01-01 00:00:00.000000 pythonix-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-13 01:39:00.350000 pythonix-1.0.0/README.md
+-rw-r--r--   0        0        0      284 2024-04-25 18:09:22.814118 pythonix-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-13 01:39:00.350000 pythonix-1.0.0/pythonix/__init__.py
+-rw-r--r--   0        0        0     5348 2024-04-25 15:52:31.904118 pythonix-1.0.0/pythonix/internals/__pycache__/op.cpython-312.pyc
+-rw-r--r--   0        0        0     2421 2024-04-18 01:37:05.054118 pythonix-1.0.0/pythonix/internals/__pycache__/ops.cpython-312.pyc
+-rw-r--r--   0        0        0     4967 2024-04-25 15:54:40.194118 pythonix-1.0.0/pythonix/internals/__pycache__/pair.cpython-312.pyc
+-rw-r--r--   0        0        0     7799 2024-04-22 17:28:53.444118 pythonix-1.0.0/pythonix/internals/__pycache__/pipe.cpython-312.pyc
+-rw-r--r--   0        0        0     7141 2024-04-18 01:37:05.044118 pythonix-1.0.0/pythonix/internals/__pycache__/pipes.cpython-312.pyc
+-rw-r--r--   0        0        0    13646 2024-04-25 15:46:38.174118 pythonix-1.0.0/pythonix/internals/__pycache__/req.cpython-312.pyc
+-rw-r--r--   0        0        0    10297 2024-04-23 19:30:10.434118 pythonix-1.0.0/pythonix/internals/__pycache__/request.cpython-312.pyc
+-rw-r--r--   0        0        0    22954 2024-04-25 16:07:26.584118 pythonix-1.0.0/pythonix/internals/__pycache__/res.cpython-312.pyc
+-rw-r--r--   0        0        0     7175 2024-04-25 16:23:02.564118 pythonix-1.0.0/pythonix/internals/__pycache__/trail.cpython-312.pyc
+-rw-r--r--   0        0        0      817 2024-04-25 17:35:02.224118 pythonix-1.0.0/pythonix/internals/__pycache__/types.cpython-312.pyc
+-rw-r--r--   0        0        0     4377 2024-04-25 15:52:22.614118 pythonix-1.0.0/pythonix/internals/mdeq.py
+-rw-r--r--   0        0        0     2447 2024-04-25 15:52:31.424118 pythonix-1.0.0/pythonix/internals/op.py
+-rw-r--r--   0        0        0     1368 2024-04-25 15:54:39.704118 pythonix-1.0.0/pythonix/internals/pair.py
+-rw-r--r--   0        0        0     4045 2024-04-22 17:28:24.824118 pythonix-1.0.0/pythonix/internals/pipe.py
+-rw-r--r--   0        0        0     7316 2024-04-25 15:46:37.674118 pythonix-1.0.0/pythonix/internals/req.py
+-rw-r--r--   0        0        0    10908 2024-04-25 16:07:26.104118 pythonix-1.0.0/pythonix/internals/res.py
+-rw-r--r--   0        0        0     2183 2024-04-25 16:23:02.094118 pythonix-1.0.0/pythonix/internals/trail.py
+-rw-r--r--   0        0        0     2780 2024-04-25 18:04:02.194118 pythonix-1.0.0/pythonix/internals/tuple.py
+-rw-r--r--   0        0        0       95 2024-04-25 17:35:01.674118 pythonix-1.0.0/pythonix/internals/types.py
+-rw-r--r--   0        0        0      206 2024-04-23 18:09:04.734118 pythonix-1.0.0/pythonix/mdeq.py
+-rw-r--r--   0        0        0       69 2024-04-22 17:26:16.504118 pythonix-1.0.0/pythonix/op.py
+-rw-r--r--   0        0        0      133 2024-04-23 19:02:18.274118 pythonix-1.0.0/pythonix/pair.py
+-rw-r--r--   0        0        0      886 2024-04-18 16:47:23.234118 pythonix-1.0.0/pythonix/pipe.py
+-rw-r--r--   0        0        0      216 2024-04-25 15:14:51.934118 pythonix-1.0.0/pythonix/prelude.py
+-rw-r--r--   0        0        0      644 2024-04-25 15:40:16.334118 pythonix-1.0.0/pythonix/req.py
+-rw-r--r--   0        0        0      425 2024-04-22 18:27:24.324118 pythonix-1.0.0/pythonix/res.py
+-rw-r--r--   0        0        0      183 2024-04-25 18:08:10.144118 pythonix-1.0.0/pythonix/trail.py
+-rw-r--r--   0        0        0      181 2024-04-22 17:55:20.064118 pythonix-1.0.0/pythonix/tuple.py
+-rw-r--r--   0        0        0      324 1970-01-01 00:00:00.000000 pythonix-1.0.0/PKG-INFO
```

