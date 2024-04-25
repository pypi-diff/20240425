# Comparing `tmp/bitlinear-1.0.1.tar.gz` & `tmp/bitlinear-1.1.0.tar.gz`

## Comparing `bitlinear-1.0.1.tar` & `bitlinear-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 bitlinear-1.0.1/bitlinear/__init__.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 bitlinear-1.0.1/bitlinear/bitlinear.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 bitlinear-1.0.1/bitlinear/kernels.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bitlinear-1.0.1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bitlinear-1.0.1/LICENSE
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bitlinear-1.0.1/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bitlinear-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bitlinear-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 bitlinear-1.1.0/bitlinear/__init__.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 bitlinear-1.1.0/bitlinear/bitlinear.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 bitlinear-1.1.0/bitlinear/kernels.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bitlinear-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bitlinear-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bitlinear-1.1.0/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bitlinear-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bitlinear-1.1.0/PKG-INFO
```

### Comparing `bitlinear-1.0.1/bitlinear/bitlinear.py` & `bitlinear-1.1.0/bitlinear/bitlinear.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,35 +13,37 @@
             out_features,
             bias=True,
             device=None,
             dtype=None,
             eps=1e-5,
             activation_bits=8,
             kernel=TorchLinear(),
+            measure=torch.median,
         ):
         super(BitLinear, self).__init__(
             in_features=in_features,
             out_features=out_features,
             bias=bias,
             device=device,
             dtype=dtype,
         )
         self.eps = eps
         self.activation_bits = activation_bits
         self.kernel = kernel
+        self.measure = measure
         self.Q_b = 2**(activation_bits-1)-1
 
     def __repr__(self):
         return f"BitLinear(in_features={self.in_features}, out_features={self.out_features}, bias={self.bias is not None}, eps={self.eps}, activation_bits={self.activation_bits}, kernel={self.kernel})"
 
     def forward(self, x):
         x_norm = torch.layer_norm(x, x.size()[1:])
-        x_scale = self.Q_b / x_norm.abs().max(dim=-1, keepdim=True).values.clamp_(min=self.eps)
+        x_scale = self.Q_b / x_norm.detach().abs().max(dim=-1, keepdim=True).values.clamp_(min=self.eps)
         x_quant = round_clamp(x_norm * x_scale, -self.Q_b-1, self.Q_b)
-        w_scale = 1 / self.weight.abs().mean().clamp_(min=self.eps)
+        w_scale = 1 / self.measure(self.weight.detach().abs()).clamp_(min=self.eps)
         w_quant = round_clamp(self.weight * w_scale, -1, 1)
         y_quant = self.kernel(x_quant, w_quant, self.bias)
         y = y_quant / (w_scale * x_scale)
         return y
 
 def replace_modules(model, old_class=nn.Linear, new_class=BitLinear, new_class_kwargs={}):
     for name, module in model.named_children():
```

### Comparing `bitlinear-1.0.1/bitlinear/kernels.py` & `bitlinear-1.1.0/bitlinear/kernels.py`

 * *Files identical despite different names*

### Comparing `bitlinear-1.0.1/LICENSE` & `bitlinear-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bitlinear-1.0.1/README.md` & `bitlinear-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bitlinear-1.0.1/pyproject.toml` & `bitlinear-1.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bitlinear"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
   { name = "Peter Schneider-Kamp" }
 ]
 
 description = "An production-ready implementation of 1.58 bit quantization-aware training and inference."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `bitlinear-1.0.1/PKG-INFO` & `bitlinear-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bitlinear
-Version: 1.0.1
+Version: 1.1.0
 Summary: An production-ready implementation of 1.58 bit quantization-aware training and inference.
 Project-URL: Homepage, https://github.com/schneiderkamplab/bitlinear
 Project-URL: Bug Tracker, https://github.com/schneiderkamplab/bitlinear/issues
 Author: Peter Schneider-Kamp
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

