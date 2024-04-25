# Comparing `tmp/dscim-0.5.0.tar.gz` & `tmp/dscim-0.6.0.tar.gz`

## Comparing `dscim-0.5.0.tar` & `dscim-0.6.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 dscim-0.5.0/CHANGELOG.md
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 dscim-0.5.0/requirements.txt
--rw-r--r--   0        0        0     8559 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/_version.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/descriptors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/menu/__init__.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/menu/baseline.py
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/menu/decorators.py
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/menu/equity.py
--rw-r--r--   0        0        0    50103 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/menu/main_recipe.py
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/menu/risk_aversion.py
--rw-r--r--   0        0        0    13741 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/menu/simple_storage.py
--rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/preprocessing/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/preprocessing/__init__.py
--rw-r--r--   0        0        0    27393 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/preprocessing/input_damages.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/preprocessing/midprocessing.py
--rw-r--r--   0        0        0    12594 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/preprocessing/preprocessing.py
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/preprocessing/climate/all_masks_rff.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/preprocessing/climate/ssp_clipped_rff.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/preprocessing/climate/stack_iterations.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/preprocessing/climate/stack_masks.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/preprocessing/misc/bottom_code_econ_zarr.py
--rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/preprocessing/misc/check_nans.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/preprocessing/misc/convert_float32.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/utils/__init__.py
--rw-r--r--   0        0        0     7768 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/utils/functions.py
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/utils/generate_yaml.py
--rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/utils/menu_runs.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/utils/plotting_utils.py
--rw-r--r--   0        0        0    16504 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/utils/rff.py
--rw-r--r--   0        0        0    21040 2020-02-02 00:00:00.000000 dscim-0.5.0/src/dscim/utils/utils.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dscim-0.5.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dscim-0.5.0/LICENSE
--rw-r--r--   0        0        0     5436 2020-02-02 00:00:00.000000 dscim-0.5.0/README.md
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 dscim-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     6489 2020-02-02 00:00:00.000000 dscim-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     9966 2020-02-02 00:00:00.000000 dscim-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 dscim-0.6.0/requirements.txt
+-rw-r--r--   0        0        0     8559 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/_version.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/descriptors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/menu/__init__.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/menu/baseline.py
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/menu/decorators.py
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/menu/equity.py
+-rw-r--r--   0        0        0    50633 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/menu/main_recipe.py
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/menu/risk_aversion.py
+-rw-r--r--   0        0        0    13741 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/menu/simple_storage.py
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/preprocessing/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/preprocessing/__init__.py
+-rw-r--r--   0        0        0    27523 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/preprocessing/input_damages.py
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/preprocessing/midprocessing.py
+-rw-r--r--   0        0        0    12594 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/preprocessing/preprocessing.py
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/preprocessing/climate/all_masks_rff.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/preprocessing/climate/ssp_clipped_rff.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/preprocessing/climate/stack_iterations.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/preprocessing/climate/stack_masks.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/preprocessing/misc/bottom_code_econ_zarr.py
+-rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/preprocessing/misc/check_nans.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/preprocessing/misc/convert_float32.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/utils/__init__.py
+-rw-r--r--   0        0        0     7770 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/utils/functions.py
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/utils/generate_yaml.py
+-rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/utils/menu_runs.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/utils/plotting_utils.py
+-rw-r--r--   0        0        0    16504 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/utils/rff.py
+-rw-r--r--   0        0        0    21273 2020-02-02 00:00:00.000000 dscim-0.6.0/src/dscim/utils/utils.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dscim-0.6.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dscim-0.6.0/LICENSE
+-rw-r--r--   0        0        0     5436 2020-02-02 00:00:00.000000 dscim-0.6.0/README.md
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 dscim-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6489 2020-02-02 00:00:00.000000 dscim-0.6.0/PKG-INFO
```

### Comparing `dscim-0.5.0/CHANGELOG.md` & `dscim-0.6.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,29 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.6.0] - 2024-04-24
+
 ### Added
+
+- Add an option for producing SCC ranges that account for only statistical uncertainty. ([PR #143](https://github.com/ClimateImpactLab/dscim/pull/143), [@davidrzhdu](https://github.com/davidrzhdu))
+
+### Fixed
+
+- Fix concatenate_energy_damages netcdf saving functionality which was not clearing data encoding causing some coordinates to be truncated. ([PR #229](https://github.com/ClimateImpactLab/dscim/pull/229), [@JMGilbert](https://github.com/JMGilbert))
+- Fix tests broken by sorting update in pandas v2.2.1 ([PR #216] (https://github.com/ClimateImpactLab/dscim/pull/216), [@JMGilbert](https://github.com/JMGilbert))
+
+## [0.5.0] - 2023-11-17
+
+### Added
+
 - Add naive list of package dependencies to pyproject.toml.([PR #123](https://github.com/ClimateImpactLab/dscim/pull/123), [@brews](https://github.com/brews))
 - CI, coverage, DOI badges on README. ([PR #134](https://github.com/ClimateImpactLab/dscim/pull/134), [@brews](https://github.com/brews))
 
 ### Changed
 
 - Dropped optional/unused dependencies `click`, `dask-jobqueue`, `geopandas`, `gurobipy`, `ipywidgets`, `seaborn`. ([PR #99](https://github.com/ClimateImpactLab/dscim/pull/99), [@brews](https://github.com/brews))
 - Switch build system from `setuptools` to `hatchling`. ([PR #128](https://github.com/ClimateImpactLab/dscim/pull/128), [@brews](https://github.com/brews))
@@ -98,13 +112,15 @@
 
 - Add missing `self` arg to `global_consumption_calculation` abstract method. ([PR #43](https://github.com/ClimateImpactLab/dscim/pull/43), [@brews](https://github.com/brews))
 
 ## [0.1.0] - 2022-08-30
 
 - Initial release.
 
-[unreleased]: https://github.com/climateimpactlab/dscim/compare/v0.4.0...HEAD
+[unreleased]: https://github.com/climateimpactlab/dscim/compare/v0.6.0...HEAD
+[0.6.0]: https://github.com/climateimpactlab/dscim/compare/v0.5.0...v0.6.0
+[0.5.0]: https://github.com/climateimpactlab/dscim/compare/v0.4.0...v0.5.0
 [0.4.0]: https://github.com/climateimpactlab/dscim/compare/v0.3.0...v0.4.0
 [0.3.0]: https://github.com/climateimpactlab/dscim/compare/v0.2.1...v0.3.0
 [0.2.1]: https://github.com/climateimpactlab/dscim/compare/v0.2.0...v0.2.1
 [0.2.0]: https://github.com/climateimpactlab/dscim/compare/v0.1.0...v0.2.0
 [0.1.0]: https://github.com/climateimpactlab/dscim/releases/tag/v0.1.0
```

### Comparing `dscim-0.5.0/src/dscim/__init__.py` & `dscim-0.6.0/src/dscim/__init__.py`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/src/dscim/descriptors.py` & `dscim-0.6.0/src/dscim/descriptors.py`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/src/dscim/menu/baseline.py` & `dscim-0.6.0/src/dscim/menu/baseline.py`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/src/dscim/menu/decorators.py` & `dscim-0.6.0/src/dscim/menu/decorators.py`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/src/dscim/menu/equity.py` & `dscim-0.6.0/src/dscim/menu/equity.py`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/src/dscim/menu/main_recipe.py` & `dscim-0.6.0/src/dscim/menu/main_recipe.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,14 +314,16 @@
         def scc():
             damage_function()
             self.global_consumption
             self.global_consumption_no_pulse
             self.logger.info("Processing SCC calculation ...")
             if self.fit_type == "quantreg":
                 self.full_uncertainty_iqr
+                self.calculate_scc
+                self.stat_uncertainty_iqr
             else:
                 if len(self.fair_aggregation) > 0:
                     self.stream_discount_factors
                     self.calculate_scc
                 self.uncollapsed_sccs
                 self.uncollapsed_marginal_damages
                 self.uncollapsed_discount_factors
@@ -1117,40 +1119,52 @@
         return pvd_damages
 
     @cachedproperty
     @save(name="uncollapsed_sccs")
     def uncollapsed_sccs(self):
         """Calculate full distribution of SCCs without FAIR aggregation"""
 
-        md = self.global_consumption_no_pulse - self.global_consumption_pulse
+        md = (
+            self.global_consumption_no_pulse - self.global_consumption_pulse
+        )  # this is for full uncertainty
 
         # convert to the marginal damages from a single pulse
         md = md * self.climate.conversion
 
         md = md.expand_dims({"fair_aggregation": ["uncollapsed"]})
 
         sccs = self.discounted_damages(
             damages=md,
             discrate=self.discounting_type,
         ).sum(dim="year")
 
         return sccs
 
-    # @cachedproperty
-    # def quantiles_sccs(self):
-    #     return self.uncollapsed_sccs.quantile(self.scc_quantiles, dim=self.fair_dims)
+    @cachedproperty
+    @save(name="stat_uncertainty_iqr")
+    def stat_uncertainty_iqr(self):
+        """Calculate the distribution of quantile-weighted SCCs produced from
+        quantile regressions that have already been collapsed across other dimensions to give statistical-only uncertainty.
+        """
+        return quantile_weight_quantilereg(
+            self.calculate_scc,
+            fair_dims=self.fair_dims,
+            quantiles=self.full_uncertainty_quantiles,
+        )
 
     @cachedproperty
     @save(name="full_uncertainty_iqr")
     def full_uncertainty_iqr(self):
         """Calculate the distribution of quantile-weighted SCCs produced from
         quantile regressions.
         """
         return quantile_weight_quantilereg(
-            self.uncollapsed_sccs, quantiles=self.full_uncertainty_quantiles
+            self.uncollapsed_sccs,
+            fair_dims=self.fair_dims,
+            quantiles=self.full_uncertainty_quantiles,
         )
 
     def calculate_discount_factors(self, cons_pc):
         """Calculates the stream of discount factors based on the Euler equation that defines an optimal
         intertemporal consumption allocation. Rearranging that equation shows that an outcome that will occur at the
         period t will be converted into today's, period 0 value, the following way :
```

### Comparing `dscim-0.5.0/src/dscim/menu/risk_aversion.py` & `dscim-0.6.0/src/dscim/menu/risk_aversion.py`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/src/dscim/menu/simple_storage.py` & `dscim-0.6.0/src/dscim/menu/simple_storage.py`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/src/dscim/preprocessing/README.md` & `dscim-0.6.0/src/dscim/preprocessing/README.md`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/src/dscim/preprocessing/input_damages.py` & `dscim-0.6.0/src/dscim/preprocessing/input_damages.py`

 * *Files 1% similar despite different names*

```diff
@@ -645,15 +645,19 @@
         if format_file == "zarr":
             to_store = concat_ds.copy()
             for var in to_store.variables:
                 to_store[var].encoding.clear()
 
             to_store.to_zarr(f"{path_to_file}.zarr", mode="w", consolidated=True)
         elif format_file == "netcdf":
-            concat_ds.to_netcdf(f"{path_to_file}.nc4")
+            to_store = concat_ds.copy()
+            for var in to_store.variables:
+                to_store[var].encoding.clear()
+
+            to_store.to_netcdf(f"{path_to_file}.nc4")
 
     return concat_ds
 
 
 def calculate_energy_batch_damages(batch, ec, input_path, save_path):
     print(f"Processing batch={batch} damages in {os.getpid()}")
     concatenate_energy_damages(
```

### Comparing `dscim-0.5.0/src/dscim/preprocessing/midprocessing.py` & `dscim-0.6.0/src/dscim/preprocessing/midprocessing.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,17 +41,17 @@
 ):
     print(f"Creating {recipe} {disc} for {CAMEL}...")
     os.makedirs(f"{input_dir}/{CAMEL}/{pulse_year}/{mask}", exist_ok=True)
 
     coefs, fit = {}, {}
 
     for sector in [coastal, AMEL]:
-        coefs[
-            sector
-        ] = f"{input_dir}/{sector}/{pulse_year}/{mask}/{recipe}_{disc}_eta{eta}_rho{rho}_damage_function_coefficients.nc4"
+        coefs[sector] = (
+            f"{input_dir}/{sector}/{pulse_year}/{mask}/{recipe}_{disc}_eta{eta}_rho{rho}_damage_function_coefficients.nc4"
+        )
 
     coefs["combined"] = xr.combine_by_coords(
         [
             xr.open_dataset(coefs[AMEL]),
             xr.open_dataset(coefs[coastal]),
         ],
         combine_attrs="drop",
@@ -67,17 +67,17 @@
 
     coefs["combined"].to_netcdf(
         f"{input_dir}/{CAMEL}/{pulse_year}/{mask}/{recipe}_{disc}_eta{eta}_rho{rho}_damage_function_coefficients.nc4"
     )
 
     if fit:
         for sector in [coastal, AMEL]:
-            fit[
-                sector
-            ] = f"{input_dir}/{sector}/{pulse_year}/{mask}/{recipe}_{disc}_eta{eta}_rho{rho}_damage_function_fit.nc4"
+            fit[sector] = (
+                f"{input_dir}/{sector}/{pulse_year}/{mask}/{recipe}_{disc}_eta{eta}_rho{rho}_damage_function_fit.nc4"
+            )
 
         fit["combined"] = xr.open_dataset(fit[coastal]) + xr.open_dataset(fit[AMEL])
 
         fit["combined"].attrs = {
             "sector": CAMEL,
             "Run type": recipe,
             "Discount type": disc,
```

### Comparing `dscim-0.5.0/src/dscim/preprocessing/preprocessing.py` & `dscim-0.6.0/src/dscim/preprocessing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/src/dscim/preprocessing/climate/all_masks_rff.py` & `dscim-0.6.0/src/dscim/preprocessing/climate/all_masks_rff.py`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/src/dscim/preprocessing/climate/ssp_clipped_rff.py` & `dscim-0.6.0/src/dscim/preprocessing/climate/ssp_clipped_rff.py`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/src/dscim/preprocessing/climate/stack_iterations.py` & `dscim-0.6.0/src/dscim/preprocessing/climate/stack_iterations.py`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/src/dscim/preprocessing/climate/stack_masks.py` & `dscim-0.6.0/src/dscim/preprocessing/climate/stack_masks.py`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/src/dscim/preprocessing/misc/bottom_code_econ_zarr.py` & `dscim-0.6.0/src/dscim/preprocessing/misc/bottom_code_econ_zarr.py`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/src/dscim/preprocessing/misc/check_nans.py` & `dscim-0.6.0/src/dscim/preprocessing/misc/check_nans.py`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/src/dscim/preprocessing/misc/convert_float32.py` & `dscim-0.6.0/src/dscim/preprocessing/misc/convert_float32.py`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/src/dscim/utils/functions.py` & `dscim-0.6.0/src/dscim/utils/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,17 +202,17 @@
         "mri-cgcm3": "MRI-CGCM3",
         "noresm1-m": "NorESM1-M",
     }
 
     [v.update(common) for k, v in name_dict.items()]
 
     for old, new in name_dict[rcp].items():
-        weights.loc[
-            weights.model.str.contains(f"{old}"), "model"
-        ] = weights.model.apply(lambda x: x.replace(x, new))
+        weights.loc[weights.model.str.contains(f"{old}"), "model"] = (
+            weights.model.apply(lambda x: x.replace(x, new))
+        )
     weights.model = weights.model.apply(lambda x: x.replace("*", ""))
     weights = weights.rename(columns={"model": "gcm"}).set_index("gcm").to_xarray()
     weights = weights.assign_coords({"rcp": rcp})
 
     return weights.weight
```

### Comparing `dscim-0.5.0/src/dscim/utils/generate_yaml.py` & `dscim-0.6.0/src/dscim/utils/generate_yaml.py`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/src/dscim/utils/menu_runs.py` & `dscim-0.6.0/src/dscim/utils/menu_runs.py`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/src/dscim/utils/plotting_utils.py` & `dscim-0.6.0/src/dscim/utils/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/src/dscim/utils/rff.py` & `dscim-0.6.0/src/dscim/utils/rff.py`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/src/dscim/utils/utils.py` & `dscim-0.6.0/src/dscim/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,32 +95,39 @@
     if np.any(np.logical_or(quantiles > 1, quantiles < 0)):
         raise RuntimeError("quantiles must be between 0-1")
     bounds = np.array([0] + ((quantiles[:-1] + quantiles[1:]) / 2).tolist() + [1])
     weights = np.diff(bounds)
     return weights
 
 
-def quantile_weight_quantilereg(array, quantiles=None):
+def quantile_weight_quantilereg(array, fair_dims, quantiles=None):
     """Produce quantile weights of the quantile regression damages.
 
     Parameters
     ----------
     qr_quantiles: the quantile regression quantiles for damages. (Must be 0-1!)
     quantiles : sequence or None, optional
         Quantiles to compute. Default is (0.01, 0.05, 0.167, 0.25, 0.5, 0.75,
         0.833, 0.95, 0.99).
     """
     if quantiles is None:
         quantiles = [0.01, 0.05, 0.167, 0.25, 0.5, 0.75, 0.833, 0.95, 0.99]
 
     qr_quantiles = array.q.values
+
+    to_stack = ["q"] + list(set(fair_dims).intersection(set(array.coords)))
     weights = xr.DataArray(get_weights(qr_quantiles), dims=["q"], coords=[qr_quantiles])
 
-    ds_stacked = array.stack(obs=("simulation", "q"))
-    weights_by_obs = weights.sel(q=ds_stacked.obs.q)
+    if len(to_stack) > 1:
+        ds_stacked = array.stack(obs=to_stack)
+        weights_by_obs = weights.sel(q=ds_stacked.obs.q)
+    else:
+        ds_stacked = array.rename({to_stack[0]: "obs"})
+        weights_by_obs = weights.sel(q=ds_stacked.obs)
+
     dim = "obs"
 
     # these are quantiles of the statistical or full uncertainty, weighted by the quantile regression quantiles
     ds_quantiles = impactlab_tools.utils.weighting.weighted_quantile_xr(
         ds_stacked, quantiles, sample_weight=weights_by_obs.values, dim=dim
     )
```

### Comparing `dscim-0.5.0/.gitignore` & `dscim-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/LICENSE` & `dscim-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/README.md` & `dscim-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/pyproject.toml` & `dscim-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dscim-0.5.0/PKG-INFO` & `dscim-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: dscim
-Version: 0.5.0
+Version: 0.6.0
 Summary: Data-Driven Spatial Climate Impact Model core component code
 Project-URL: Homepage, https://github.com/ClimateImpactLab/dscim
 Project-URL: Documentation, https://github.com/ClimateImpactLab/dscim
 Project-URL: Source, https://github.com/ClimateImpactLab/dscim
 Project-URL: Bug Tracker, https://github.com/ClimateImpactLab/dscim/issues
 License-File: LICENSE
 Classifier: Intended Audience :: Science/Research
```

