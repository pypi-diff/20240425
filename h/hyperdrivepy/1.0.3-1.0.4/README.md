# Comparing `tmp/hyperdrivepy-1.0.3.tar.gz` & `tmp/hyperdrivepy-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperdrivepy-1.0.3.tar", last modified: Fri Apr 19 21:07:14 2024, max compression
+gzip compressed data, was "hyperdrivepy-1.0.4.tar", last modified: Thu Apr 25 19:27:17 2024, max compression
```

## Comparing `hyperdrivepy-1.0.3.tar` & `hyperdrivepy-1.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:07:14.324319 hyperdrivepy-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-19 21:07:14.324319 hyperdrivepy-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:07:14.320318 hyperdrivepy-1.0.3/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:07:14.320318 hyperdrivepy-1.0.3/python/hyperdrivepy/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/python/hyperdrivepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20357 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/python/hyperdrivepy/hyperdrive_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/python/hyperdrivepy/hyperdrive_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:07:14.324319 hyperdrivepy-1.0.3/python/hyperdrivepy/pypechain_types/
--rw-r--r--   0 runner    (1001) docker     (127)   255141 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/python/hyperdrivepy/pypechain_types/IHyperdriveContract.py
--rw-r--r--   0 runner    (1001) docker     (127)    16836 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/python/hyperdrivepy/pypechain_types/IHyperdriveTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/python/hyperdrivepy/pypechain_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/python/hyperdrivepy/pypechain_types/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/python/hyperdrivepy/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/python/hyperdrivepy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:07:14.324319 hyperdrivepy-1.0.3/python/hyperdrivepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-19 21:07:14.000000 hyperdrivepy-1.0.3/python/hyperdrivepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-19 21:07:14.000000 hyperdrivepy-1.0.3/python/hyperdrivepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:07:14.000000 hyperdrivepy-1.0.3/python/hyperdrivepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:07:14.000000 hyperdrivepy-1.0.3/python/hyperdrivepy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 21:07:14.000000 hyperdrivepy-1.0.3/python/hyperdrivepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:07:14.324319 hyperdrivepy-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:07:14.324319 hyperdrivepy-1.0.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/src/hyperdrive_state.rs
--rw-r--r--   0 runner    (1001) docker     (127)    16359 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/src/hyperdrive_state_methods.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/src/hyperdrive_utils.rs
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/src/pool_config.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/src/pool_info.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/src/utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:27:17.898141 hyperdrivepy-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-25 19:27:12.000000 hyperdrivepy-1.0.4/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 19:27:12.000000 hyperdrivepy-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 19:27:12.000000 hyperdrivepy-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-25 19:27:17.898141 hyperdrivepy-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-25 19:27:12.000000 hyperdrivepy-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-25 19:27:12.000000 hyperdrivepy-1.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:27:17.890141 hyperdrivepy-1.0.4/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:27:17.894141 hyperdrivepy-1.0.4/python/hyperdrivepy/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-25 19:27:12.000000 hyperdrivepy-1.0.4/python/hyperdrivepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20247 2024-04-25 19:27:12.000000 hyperdrivepy-1.0.4/python/hyperdrivepy/hyperdrive_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-25 19:27:12.000000 hyperdrivepy-1.0.4/python/hyperdrivepy/hyperdrive_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:27:17.894141 hyperdrivepy-1.0.4/python/hyperdrivepy/pypechain_types/
+-rw-r--r--   0 runner    (1001) docker     (127)   255141 2024-04-25 19:27:12.000000 hyperdrivepy-1.0.4/python/hyperdrivepy/pypechain_types/IHyperdriveContract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16836 2024-04-25 19:27:12.000000 hyperdrivepy-1.0.4/python/hyperdrivepy/pypechain_types/IHyperdriveTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 19:27:12.000000 hyperdrivepy-1.0.4/python/hyperdrivepy/pypechain_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-25 19:27:12.000000 hyperdrivepy-1.0.4/python/hyperdrivepy/pypechain_types/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-25 19:27:12.000000 hyperdrivepy-1.0.4/python/hyperdrivepy/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-25 19:27:12.000000 hyperdrivepy-1.0.4/python/hyperdrivepy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:27:17.898141 hyperdrivepy-1.0.4/python/hyperdrivepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-25 19:27:17.000000 hyperdrivepy-1.0.4/python/hyperdrivepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-25 19:27:17.000000 hyperdrivepy-1.0.4/python/hyperdrivepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:27:17.000000 hyperdrivepy-1.0.4/python/hyperdrivepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:27:17.000000 hyperdrivepy-1.0.4/python/hyperdrivepy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 19:27:17.000000 hyperdrivepy-1.0.4/python/hyperdrivepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:27:17.898141 hyperdrivepy-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-25 19:27:12.000000 hyperdrivepy-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:27:17.894141 hyperdrivepy-1.0.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-25 19:27:12.000000 hyperdrivepy-1.0.4/src/hyperdrive_state.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    16125 2024-04-25 19:27:12.000000 hyperdrivepy-1.0.4/src/hyperdrive_state_methods.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-25 19:27:12.000000 hyperdrivepy-1.0.4/src/hyperdrive_utils.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-25 19:27:12.000000 hyperdrivepy-1.0.4/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-25 19:27:12.000000 hyperdrivepy-1.0.4/src/pool_config.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-25 19:27:12.000000 hyperdrivepy-1.0.4/src/pool_info.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-25 19:27:12.000000 hyperdrivepy-1.0.4/src/utils.rs
```

### Comparing `hyperdrivepy-1.0.3/Cargo.toml` & `hyperdrivepy-1.0.4/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "hyperdrivepy"
 edition = "2021"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
     "Dylan Paiton",
     "Matt Brown",
     "Sheng Lundquist",
 ]
 description = "Python wrappers for the Hyperdrive AMM"
```

### Comparing `hyperdrivepy-1.0.3/LICENSE` & `hyperdrivepy-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.3/PKG-INFO` & `hyperdrivepy-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperdrivepy
-Version: 1.0.3
+Version: 1.0.4
 Project-URL: Homepage, https://github.com/delvtech/hyperdrive-bindings
 Project-URL: Issues, https://github.com/delvtech/hyperdrive-bindings/issues
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `hyperdrivepy-1.0.3/pyproject.toml` & `hyperdrivepy-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hyperdrivepy"
-version = "1.0.3"
+version = "1.0.4"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Rust",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 readme = "README.md"
```

### Comparing `hyperdrivepy-1.0.3/python/hyperdrivepy/hyperdrive_state.py` & `hyperdrivepy-1.0.4/python/hyperdrivepy/hyperdrive_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,45 +249,42 @@
     return _get_interface(pool_config, pool_info).calculate_close_long(bond_amount, maturity_time, current_time)
 
 
 def calculate_open_short(
     pool_config: types.PoolConfigType,
     pool_info: types.PoolInfoType,
     short_amount: str,
-    spot_price: str,
     open_vault_share_price: str | None = None,
 ) -> str:
     """Gets the amount of base the trader will need to deposit for a short of a given size.
 
     Arguments
     ---------
     pool_config: PoolConfig
         Static configuration for the hyperdrive contract.
         Set at deploy time.
     pool_info: PoolInfo
         Current state information of the hyperdrive contract.
         Includes attributes like reserve levels and share prices.
     short_amount: str (FixedPoint)
         The amount to of bonds to short.
-    spot_price: str (FixedPoint)
-        The pool's current price for bonds.
     open_vault_share_price: str (FixedPoint) | None, optional
         Optionally provide the open share price for the short.
         If this is not provided or is None, then we will use the pool's current share price.
 
     Returns
     -------
     str (FixedPoint)
         The amount of base required to short the bonds (aka the "max loss").
     """
     if open_vault_share_price is None:
         # the underlying rust code uses current market share price if this is 0
         # zero value is used because the smart contract will return 0 if the checkpoint hasn't been minted
         open_vault_share_price = "0"
-    return _get_interface(pool_config, pool_info).calculate_open_short(short_amount, spot_price, open_vault_share_price)
+    return _get_interface(pool_config, pool_info).calculate_open_short(short_amount, open_vault_share_price)
 
 
 def calculate_close_short(
     pool_config: types.PoolConfigType,
     pool_info: types.PoolInfoType,
     bond_amount: str,
     open_vault_share_price: str,
```

### Comparing `hyperdrivepy-1.0.3/python/hyperdrivepy/hyperdrive_utils.py` & `hyperdrivepy-1.0.4/python/hyperdrivepy/hyperdrive_utils.py`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.3/python/hyperdrivepy/pypechain_types/IHyperdriveContract.py` & `hyperdrivepy-1.0.4/python/hyperdrivepy/pypechain_types/IHyperdriveContract.py`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.3/python/hyperdrivepy/pypechain_types/IHyperdriveTypes.py` & `hyperdrivepy-1.0.4/python/hyperdrivepy/pypechain_types/IHyperdriveTypes.py`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.3/python/hyperdrivepy/pypechain_types/utilities.py` & `hyperdrivepy-1.0.4/python/hyperdrivepy/pypechain_types/utilities.py`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.3/python/hyperdrivepy/types.py` & `hyperdrivepy-1.0.4/python/hyperdrivepy/types.py`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.3/python/hyperdrivepy/utils.py` & `hyperdrivepy-1.0.4/python/hyperdrivepy/utils.py`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.3/python/hyperdrivepy.egg-info/PKG-INFO` & `hyperdrivepy-1.0.4/python/hyperdrivepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperdrivepy
-Version: 1.0.3
+Version: 1.0.4
 Project-URL: Homepage, https://github.com/delvtech/hyperdrive-bindings
 Project-URL: Issues, https://github.com/delvtech/hyperdrive-bindings/issues
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `hyperdrivepy-1.0.3/python/hyperdrivepy.egg-info/SOURCES.txt` & `hyperdrivepy-1.0.4/python/hyperdrivepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.3/src/hyperdrive_state.rs` & `hyperdrivepy-1.0.4/src/hyperdrive_state.rs`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.3/src/hyperdrive_state_methods.rs` & `hyperdrivepy-1.0.4/src/hyperdrive_state_methods.rs`

 * *Files 1% similar despite different names*

```diff
@@ -151,32 +151,28 @@
         let result = U256::from(result_fp).to_string();
         return Ok(result);
     }
 
     pub fn calculate_open_short(
         &self,
         short_amount: &str,
-        spot_price: &str,
         open_vault_share_price: &str,
     ) -> PyResult<String> {
         let short_amount_fp = FixedPoint::from(U256::from_dec_str(short_amount).map_err(|_| {
             PyErr::new::<PyValueError, _>("Failed to convert short_amount string to U256")
         })?);
-        let spot_price_fp = FixedPoint::from(U256::from_dec_str(spot_price).map_err(|_| {
-            PyErr::new::<PyValueError, _>("Failed to convert spot_price string to U256")
-        })?);
         let open_vault_share_price_fp =
             FixedPoint::from(U256::from_dec_str(open_vault_share_price).map_err(|_| {
                 PyErr::new::<PyValueError, _>(
                     "Failed to convert open_vault_share_price string to U256",
                 )
             })?);
         let result_fp = self
             .state
-            .calculate_open_short(short_amount_fp, spot_price_fp, open_vault_share_price_fp)
+            .calculate_open_short(short_amount_fp, open_vault_share_price_fp)
             .unwrap();
         let result = U256::from(result_fp).to_string();
         return Ok(result);
     }
 
     pub fn calculate_close_short(
         &self,
```

### Comparing `hyperdrivepy-1.0.3/src/hyperdrive_utils.rs` & `hyperdrivepy-1.0.4/src/hyperdrive_utils.rs`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.3/src/lib.rs` & `hyperdrivepy-1.0.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.3/src/pool_config.rs` & `hyperdrivepy-1.0.4/src/pool_config.rs`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.3/src/pool_info.rs` & `hyperdrivepy-1.0.4/src/pool_info.rs`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.3/src/utils.rs` & `hyperdrivepy-1.0.4/src/utils.rs`

 * *Files identical despite different names*

