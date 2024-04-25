# Comparing `tmp/rajo-0.2.5.tar.gz` & `tmp/rajo-0.2.6.tar.gz`

## Comparing `rajo-0.2.5.tar` & `rajo-0.2.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rajo-0.2.5/examples/__init__.py
--rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 rajo-0.2.5/examples/cifar10.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 rajo-0.2.5/examples/gan.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/__init__.py
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/_foreach.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/_lazy.py
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/_trainer.py
--rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/amp.py
--rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/distributed.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/driver.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/infer.py
--rw-r--r--   0        0        0    11893 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/optim.py
--rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/plot.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/py.typed
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/sched.py
--rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/util.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/data/__init__.py
--rw-r--r--   0        0        0    11608 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/data/_loader.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/data/_sampler.py
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/data/_serialization.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/metrics/__init__.py
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/metrics/base.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/metrics/confusion.py
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/metrics/func.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/metrics/raw.py
--rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/metrics/roc.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/nn/__init__.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/nn/functional.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/nn/ops.py
--rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/nn/proto.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/nn/modules/__init__.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/nn/modules/aggregates.py
--rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/nn/modules/context.py
--rw-r--r--   0        0        0    11598 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/nn/modules/conv.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/nn/modules/head.py
--rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/nn/modules/lazy.py
--rw-r--r--   0        0        0     8315 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/nn/modules/loss.py
--rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/nn/modules/primitive.py
--rw-r--r--   0        0        0     9973 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/nn/modules/transformer.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/nn/modules/util.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/nn/modules/vision.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/transforms/__init__.py
--rw-r--r--   0        0        0    10922 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/transforms/classes.py
--rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/transforms/core.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/transforms/functional/__init__.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/transforms/functional/core.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 rajo-0.2.5/src/rajo/transforms/functional/numba.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rajo-0.2.5/test/__init__.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 rajo-0.2.5/test/run_metrics.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 rajo-0.2.5/test/test_loader.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 rajo-0.2.5/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 rajo-0.2.5/LICENSE
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 rajo-0.2.5/README.md
--rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 rajo-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 rajo-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rajo-0.2.6/examples/__init__.py
+-rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 rajo-0.2.6/examples/cifar10.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 rajo-0.2.6/examples/gan.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/__init__.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/_foreach.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/_lazy.py
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/_trainer.py
+-rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/amp.py
+-rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/distributed.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/driver.py
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/infer.py
+-rw-r--r--   0        0        0    11893 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/optim.py
+-rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/plot.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/py.typed
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/sched.py
+-rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/util.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/data/__init__.py
+-rw-r--r--   0        0        0    11608 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/data/_loader.py
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/data/_sampler.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/data/_serialization.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/metrics/__init__.py
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/metrics/base.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/metrics/confusion.py
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/metrics/func.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/metrics/raw.py
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/metrics/roc.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/nn/__init__.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/nn/functional.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/nn/ops.py
+-rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/nn/proto.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/nn/modules/__init__.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/nn/modules/aggregates.py
+-rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/nn/modules/context.py
+-rw-r--r--   0        0        0    11598 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/nn/modules/conv.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/nn/modules/head.py
+-rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/nn/modules/lazy.py
+-rw-r--r--   0        0        0     8315 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/nn/modules/loss.py
+-rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/nn/modules/primitive.py
+-rw-r--r--   0        0        0     9973 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/nn/modules/transformer.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/nn/modules/util.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/nn/modules/vision.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/transforms/__init__.py
+-rw-r--r--   0        0        0    10922 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/transforms/classes.py
+-rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/transforms/core.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/transforms/functional/__init__.py
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/transforms/functional/core.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 rajo-0.2.6/src/rajo/transforms/functional/numba.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rajo-0.2.6/test/__init__.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 rajo-0.2.6/test/run_metrics.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 rajo-0.2.6/test/test_loader.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 rajo-0.2.6/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 rajo-0.2.6/LICENSE
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 rajo-0.2.6/README.md
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 rajo-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 rajo-0.2.6/PKG-INFO
```

### Comparing `rajo-0.2.5/examples/cifar10.py` & `rajo-0.2.6/examples/cifar10.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/__init__.py` & `rajo-0.2.6/src/rajo/__init__.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/_foreach.py` & `rajo-0.2.6/src/rajo/_foreach.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/_lazy.py` & `rajo-0.2.6/src/rajo/_lazy.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/_trainer.py` & `rajo-0.2.6/src/rajo/_trainer.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/amp.py` & `rajo-0.2.6/src/rajo/amp.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/distributed.py` & `rajo-0.2.6/src/rajo/distributed.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/driver.py` & `rajo-0.2.6/src/rajo/driver.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/optim.py` & `rajo-0.2.6/src/rajo/optim.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/plot.py` & `rajo-0.2.6/src/rajo/plot.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/sched.py` & `rajo-0.2.6/src/rajo/sched.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/util.py` & `rajo-0.2.6/src/rajo/util.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/data/_loader.py` & `rajo-0.2.6/src/rajo/data/_loader.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/data/_sampler.py` & `rajo-0.2.6/src/rajo/data/_sampler.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/data/_serialization.py` & `rajo-0.2.6/src/rajo/data/_serialization.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/metrics/__init__.py` & `rajo-0.2.6/src/rajo/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/metrics/base.py` & `rajo-0.2.6/src/rajo/metrics/base.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/metrics/confusion.py` & `rajo-0.2.6/src/rajo/metrics/confusion.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/metrics/func.py` & `rajo-0.2.6/src/rajo/metrics/func.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/metrics/raw.py` & `rajo-0.2.6/src/rajo/metrics/raw.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/metrics/roc.py` & `rajo-0.2.6/src/rajo/metrics/roc.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/nn/__init__.py` & `rajo-0.2.6/src/rajo/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/nn/functional.py` & `rajo-0.2.6/src/rajo/nn/functional.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/nn/ops.py` & `rajo-0.2.6/src/rajo/nn/ops.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/nn/proto.py` & `rajo-0.2.6/src/rajo/nn/proto.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/nn/modules/__init__.py` & `rajo-0.2.6/src/rajo/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/nn/modules/aggregates.py` & `rajo-0.2.6/src/rajo/nn/modules/aggregates.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/nn/modules/context.py` & `rajo-0.2.6/src/rajo/nn/modules/context.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/nn/modules/conv.py` & `rajo-0.2.6/src/rajo/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/nn/modules/head.py` & `rajo-0.2.6/src/rajo/nn/modules/head.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/nn/modules/lazy.py` & `rajo-0.2.6/src/rajo/nn/modules/lazy.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/nn/modules/loss.py` & `rajo-0.2.6/src/rajo/nn/modules/loss.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/nn/modules/primitive.py` & `rajo-0.2.6/src/rajo/nn/modules/primitive.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/nn/modules/transformer.py` & `rajo-0.2.6/src/rajo/nn/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/nn/modules/util.py` & `rajo-0.2.6/src/rajo/nn/modules/util.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/nn/modules/vision.py` & `rajo-0.2.6/src/rajo/nn/modules/vision.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/transforms/__init__.py` & `rajo-0.2.6/src/rajo/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/transforms/classes.py` & `rajo-0.2.6/src/rajo/transforms/classes.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/transforms/core.py` & `rajo-0.2.6/src/rajo/transforms/core.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/transforms/functional/core.py` & `rajo-0.2.6/src/rajo/transforms/functional/core.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/src/rajo/transforms/functional/numba.py` & `rajo-0.2.6/src/rajo/transforms/functional/numba.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/test/run_metrics.py` & `rajo-0.2.6/test/run_metrics.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/test/test_loader.py` & `rajo-0.2.6/test/test_loader.py`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/LICENSE` & `rajo-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rajo-0.2.5/pyproject.toml` & `rajo-0.2.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 only-packages = true
 
 [project]
 name = "rajo"
-version = "0.2.5"
+version = "0.2.6"
 description = "Pytorch training utilities and models"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = []
 authors = [
     {name = "Paul Maevskikh", email = "arquolo@gmail.com"},
@@ -26,21 +26,20 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "packaging",
-    "glow~=0.13.0",
+    "glow~=0.13.6",
     "numpy~=1.21",
     "scipy",
     "opencv-python-headless~=4.0",
     "einops",
     "pynvml~=11.4",
-    # --extra-index-url https://download.pytorch.org/whl/cu118
     "torch~=2.0",
     "torchvision~=0.15",
     "tqdm",
 ]
 
 [project.urls]
 homepage = "https://github.com/arquolo/rajo"
@@ -51,23 +50,23 @@
 all = ["rajo[graph]", "matplotlib"]
 trt = [
     # TODO: upd for torch 2.x
     "torch-tensorrt~=1.3; platform_system=='Linux'",
     # -f https://github.com/NVIDIA/Torch-TensorRT/releases
 ]
 dev-core = [
-    "flake8~=6.1",
+    "flake8~=7.0",
     "flake8-pie",
     "flake8-pyi",
     "flake8-pyproject",
     "flake8-simplify",
     "isort",
     "mypy~=1.7",
-    "pytest~=7.4",
-    "ruff~=0.1.7",
+    "pytest~=8.0",
+    "ruff~=0.2.2",
     "yapf~=0.40.2",
 ]
 dev = [
     "rajo[dev-core]",
     "flake8-alphabetize",
     # "flake8-class-attributes-order",
     # "flake8-newspaper-style",
@@ -77,33 +76,35 @@
     "rajo[dev-core]",
     "wemake-python-styleguide~=0.15.0",
 ]
 
 # Lint
 
 [tool.ruff]
+line-length = 79
+target-version = "py310"
+
+[tool.ruff.lint]
 select = [
     "A", "B", "C4", "C9", "D", "E", "F", "N", "PT", "Q0", "RET", "S", "SIM", "UP", "W",
     "BLE", "COM", "ICN", "INP", "PL", "RSE", "RUF",
     # "FBT", "SLF", "TCH",
     "TRY",
 ]
 ignore = [
     "A003", "B008", "B905", "D1", "D2", "D4", "N812", "S1", "S3",
     "COM812", "COM818", "PLR0913", "PLR2004", "PT011", "RET504", "TRY003", "SIM105",
 ]
 exclude = [".eggs", ".git", "__pycache__", "build", "dist"]
-line-length = 79
-target-version = "py310"
 unfixable = ["I001"]
 
-[tool.ruff.flake8-quotes]
+[tool.ruff.lint.flake8-quotes]
 inline-quotes = "single"
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 10
 
 [tool.flake8]
 select = [
     # pyflakes,pycodestyle: n/a in ruff
     "E", "F703", "F721", "F723", "F831", "W",
     # flake8-alphabetize
```

