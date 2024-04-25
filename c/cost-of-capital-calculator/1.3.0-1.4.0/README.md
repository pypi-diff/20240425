# Comparing `tmp/cost-of-capital-calculator-1.3.0.tar.gz` & `tmp/cost-of-capital-calculator-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cost-of-capital-calculator-1.3.0.tar", last modified: Thu Mar 14 15:12:22 2024, max compression
+gzip compressed data, was "cost-of-capital-calculator-1.4.0.tar", last modified: Thu Apr 25 17:39:18 2024, max compression
```

## Comparing `cost-of-capital-calculator-1.3.0.tar` & `cost-of-capital-calculator-1.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:12:22.359997 cost-of-capital-calculator-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-14 15:12:15.000000 cost-of-capital-calculator-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-03-14 15:12:22.359997 cost-of-capital-calculator-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-03-14 15:12:15.000000 cost-of-capital-calculator-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:12:22.355996 cost-of-capital-calculator-1.3.0/ccc/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-14 15:12:15.000000 cost-of-capital-calculator-1.3.0/ccc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-03-14 15:12:15.000000 cost-of-capital-calculator-1.3.0/ccc/calcfunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)    87272 2024-03-14 15:12:15.000000 cost-of-capital-calculator-1.3.0/ccc/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127) 27544791 2024-03-14 15:12:15.000000 cost-of-capital-calculator-1.3.0/ccc/ccc_asset_data.csv
--rw-r--r--   0 runner    (1001) docker     (127)    16570 2024-03-14 15:12:15.000000 cost-of-capital-calculator-1.3.0/ccc/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-03-14 15:12:15.000000 cost-of-capital-calculator-1.3.0/ccc/controls_callback_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-03-14 15:12:15.000000 cost-of-capital-calculator-1.3.0/ccc/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    66894 2024-03-14 15:12:15.000000 cost-of-capital-calculator-1.3.0/ccc/default_parameters.json
--rw-r--r--   0 runner    (1001) docker     (127)     7882 2024-03-14 15:12:15.000000 cost-of-capital-calculator-1.3.0/ccc/get_taxcalc_rates.py
--rw-r--r--   0 runner    (1001) docker     (127)     9943 2024-03-14 15:12:15.000000 cost-of-capital-calculator-1.3.0/ccc/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-03-14 15:12:15.000000 cost-of-capital-calculator-1.3.0/ccc/paramfunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-14 15:12:15.000000 cost-of-capital-calculator-1.3.0/ccc/records_variables.json
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-03-14 15:12:15.000000 cost-of-capital-calculator-1.3.0/ccc/styles.py
--rw-r--r--   0 runner    (1001) docker     (127)    51310 2024-03-14 15:12:15.000000 cost-of-capital-calculator-1.3.0/ccc/tax_depreciation_rules.json
--rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-03-14 15:12:15.000000 cost-of-capital-calculator-1.3.0/ccc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:12:22.355996 cost-of-capital-calculator-1.3.0/cost_of_capital_calculator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-03-14 15:12:22.000000 cost-of-capital-calculator-1.3.0/cost_of_capital_calculator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-14 15:12:22.000000 cost-of-capital-calculator-1.3.0/cost_of_capital_calculator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 15:12:22.000000 cost-of-capital-calculator-1.3.0/cost_of_capital_calculator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 15:12:22.000000 cost-of-capital-calculator-1.3.0/cost_of_capital_calculator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-14 15:12:22.000000 cost-of-capital-calculator-1.3.0/cost_of_capital_calculator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 15:12:22.359997 cost-of-capital-calculator-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-14 15:12:15.000000 cost-of-capital-calculator-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:18.568633 cost-of-capital-calculator-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-25 17:39:16.000000 cost-of-capital-calculator-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-25 17:39:18.568633 cost-of-capital-calculator-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-25 17:39:16.000000 cost-of-capital-calculator-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:18.568633 cost-of-capital-calculator-1.4.0/ccc/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-25 17:39:16.000000 cost-of-capital-calculator-1.4.0/ccc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12670 2024-04-25 17:39:16.000000 cost-of-capital-calculator-1.4.0/ccc/calcfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87516 2024-04-25 17:39:16.000000 cost-of-capital-calculator-1.4.0/ccc/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127) 27544791 2024-04-25 17:39:16.000000 cost-of-capital-calculator-1.4.0/ccc/ccc_asset_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    16981 2024-04-25 17:39:16.000000 cost-of-capital-calculator-1.4.0/ccc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-25 17:39:16.000000 cost-of-capital-calculator-1.4.0/ccc/controls_callback_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-25 17:39:16.000000 cost-of-capital-calculator-1.4.0/ccc/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73655 2024-04-25 17:39:16.000000 cost-of-capital-calculator-1.4.0/ccc/default_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-04-25 17:39:16.000000 cost-of-capital-calculator-1.4.0/ccc/get_taxcalc_rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10551 2024-04-25 17:39:16.000000 cost-of-capital-calculator-1.4.0/ccc/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-04-25 17:39:16.000000 cost-of-capital-calculator-1.4.0/ccc/paramfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-25 17:39:16.000000 cost-of-capital-calculator-1.4.0/ccc/records_variables.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-25 17:39:16.000000 cost-of-capital-calculator-1.4.0/ccc/styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51343 2024-04-25 17:39:16.000000 cost-of-capital-calculator-1.4.0/ccc/tax_depreciation_rules.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-04-25 17:39:16.000000 cost-of-capital-calculator-1.4.0/ccc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:18.568633 cost-of-capital-calculator-1.4.0/cost_of_capital_calculator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-25 17:39:18.000000 cost-of-capital-calculator-1.4.0/cost_of_capital_calculator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-25 17:39:18.000000 cost-of-capital-calculator-1.4.0/cost_of_capital_calculator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:39:18.000000 cost-of-capital-calculator-1.4.0/cost_of_capital_calculator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 17:39:18.000000 cost-of-capital-calculator-1.4.0/cost_of_capital_calculator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-25 17:39:18.000000 cost-of-capital-calculator-1.4.0/cost_of_capital_calculator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 17:39:18.568633 cost-of-capital-calculator-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-25 17:39:16.000000 cost-of-capital-calculator-1.4.0/setup.py
```

### Comparing `cost-of-capital-calculator-1.3.0/PKG-INFO` & `cost-of-capital-calculator-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cost-of-capital-calculator
-Version: 1.3.0
+Version: 1.4.0
 Summary: CCC: A Cost of Capital Calculator
 Home-page: https://github.com/PSLmodels/Cost-of-Capital-Calculator
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Download-URL: https://github.com/PSLmodels/Cost-of-Capital-Calculator
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -70,10 +70,10 @@
 
 
 ## Disclaimer
 Results will change as the underlying models improve. A fundamental reason for adopting open source methods in this project is so that people from all backgrounds can contribute to the models that our society uses to assess economic policy; when community-contributed improvements are incorporated, the model will produce different results.
 
 
 ## Citing the Cost-of-Capital-Calculator Model
-Cost-of-Capital-Calculator (Version 1.3.0)[Source code], https://github.com/PSLmodels/Cost-of-Capital-Calculator
+Cost-of-Capital-Calculator (Version 1.4.0)[Source code], https://github.com/PSLmodels/Cost-of-Capital-Calculator
```

### Comparing `cost-of-capital-calculator-1.3.0/README.md` & `cost-of-capital-calculator-1.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -49,8 +49,8 @@
 
 
 ## Disclaimer
 Results will change as the underlying models improve. A fundamental reason for adopting open source methods in this project is so that people from all backgrounds can contribute to the models that our society uses to assess economic policy; when community-contributed improvements are incorporated, the model will produce different results.
 
 
 ## Citing the Cost-of-Capital-Calculator Model
-Cost-of-Capital-Calculator (Version 1.3.0)[Source code], https://github.com/PSLmodels/Cost-of-Capital-Calculator
+Cost-of-Capital-Calculator (Version 1.4.0)[Source code], https://github.com/PSLmodels/Cost-of-Capital-Calculator
```

### Comparing `cost-of-capital-calculator-1.3.0/ccc/calcfunctions.py` & `cost-of-capital-calculator-1.4.0/ccc/calcfunctions.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import pandas as pd
-from ccc.constants import TAX_METHODS
+from ccc.constants import TAX_METHODS, RE_ASSETS, RE_INDUSTRIES
 from ccc.utils import str_modified
 
 pd.set_option("future.no_silent_downcasting", True)
 
 ENFORCE_CHECKS = True
 
 
@@ -136,14 +136,57 @@
             $1 of investment
 
     """
     z = bonus + ((1 - bonus) * (delta / (delta + r - pi)))
     return z
 
 
+def income_forecast(Y, delta, bonus, r):
+    r"""
+    Makes the calculation for the income forecast method.
+
+    The income forecast method involved deducting expenses in relation
+    to forecasted income over the next 10 years. CCC follows the CBO
+    methodology (CBO, 2018:
+    https://www.cbo.gov/system/files/2018-11/54648-Intangible_Assets.pdf)
+    and approximate this method with the DBSL method, but with a the "b"
+    factor determined by economic depreciation rates.
+
+    .. math::
+        z = \frac{\beta}{\beta+r}\left[1-e^{-(\beta+r)Y^{*}}\right]+
+            \frac{e^{-\beta Y^{*}}}{(Y-Y^{*})r}
+            \left[e^{-rY^{*}}-e^{-rY}\right]
+
+    Args:
+        Y (array_like): asset life in years
+        delta (array_like): rate of economic depreciation
+        bonus (array_like): rate of bonus depreciation
+        r (scalar): discount rate
+
+    Returns:
+        z (array_like): net present value of depreciation deductions for
+            $1 of investment
+
+    """
+    b = 10 * delta
+    beta = b / Y
+    Y_star = Y * (1 - (1 / b))
+    z = bonus + (
+        (1 - bonus)
+        * (
+            ((beta / (beta + r)) * (1 - np.exp(-1 * (beta + r) * Y_star)))
+            + (
+                (np.exp(-1 * beta * Y_star) / ((Y - Y_star) * r))
+                * (np.exp(-1 * r * Y_star) - np.exp(-1 * r * Y))
+            )
+        )
+    )
+    return z
+
+
 def npv_tax_depr(df, r, pi, land_expensing):
     """
     Depending on the method of depreciation, makes calls to either
     the straight line or declining balance calculations.
 
     Args:
         df (Pandas DataFrame): assets by type and tax treatment
@@ -160,49 +203,111 @@
     df.loc[idx, "z"] = dbsl(
         df.loc[idx, "Y"], df.loc[idx, "b"], df.loc[idx, "bonus"], r
     )
     idx = df["method"] == "SL"
     df.loc[idx, "z"] = sl(df.loc[idx, "Y"], df.loc[idx, "bonus"], r)
     idx = df["method"] == "Economic"
     df.loc[idx, "z"] = econ(df.loc[idx, "delta"], df.loc[idx, "bonus"], r, pi)
+    idx = df["method"] == "Income Forecast"
+    df.loc[idx, "z"] = income_forecast(
+        df.loc[idx, "Y"], df.loc[idx, "delta"], df.loc[idx, "bonus"], r
+    )
     idx = df["method"] == "Expensing"
     df.loc[idx, "z"] = 1.0
     idx = df["asset_name"] == "Land"
     df.loc[idx, "z"] = np.squeeze(land_expensing)
     idx = df["asset_name"] == "Inventories"
     df.loc[idx, "z"] = 0.0  # not sure why I have to do this with changes
     z = df["z"]
 
     return z
 
 
-def eq_coc(delta, z, w, u, inv_tax_credit, pi, r):
+def eq_coc(
+    delta,
+    z,
+    w,
+    u,
+    u_d,
+    inv_tax_credit,
+    psi,
+    nu,
+    pi,
+    r,
+    re_credit=None,
+    asset_code=None,
+    ind_code=None,
+):
     r"""
     Compute the cost of capital
 
     .. math::
-        \rho = \frac{(r-\pi+\delta)}{1-u}(1-uz)+w-\delta
+        \rho = \frac{(r-\pi+\delta)}{1-u}(1-u_dz(1-\psi k) - k\nu)+w-\delta
 
     Args:
         delta (array_like): rate of economic depreciation
         z (array_like): net present value of depreciation deductions for
             $1 of investment
         w (scalar): property tax rate
-        u (scalar): statutory marginal tax rate for the first layer of
+        u (scalar): marginal tax rate for the first layer of
             income taxes
+        u_d (scalar): marginal tax rate on deductions
         inv_tax_credit (scalar): investment tax credit rate
+        psi (scalar): fraction investment tax credit that affects
+            depreciable basis of the investment
+        nu (scalar): NPV of the investment tax credit
         pi (scalar): inflation rate
         r (scalar): discount rate
+        re_credit (dict): rate of R&E credit by asset or industry
+        asset_code (array_like): asset code
+        ind_code (array_like): industry code
 
     Returns:
         rho (array_like): the cost of capital
 
     """
+    # Initialize re_credit_rate (only needed if arrays are passed in --
+    # if not, can include the R&E credit in the inv_tax_credit object)
+    if isinstance(delta, np.ndarray):
+        re_credit_rate_ind = np.zeros_like(delta)
+        re_credit_rate_asset = np.zeros_like(delta)
+        # Update by R&E credit rate amounts by industry
+        if (ind_code is not None) and (re_credit is not None):
+            idx = [
+                index
+                for index, element in enumerate(ind_code)
+                if element in re_credit["By industry"].keys()
+            ]
+            print("Keys = ", re_credit["By industry"].keys())
+            print("Ind idx = ", idx)
+            print("Dict = ", re_credit["By industry"], re_credit)
+            ind_code_idx = [ind_code[i] for i in idx]
+            re_credit_rate_ind[idx] = [
+                re_credit["By industry"][ic] for ic in ind_code_idx
+            ]
+        # Update by R&E credit rate amounts by asset
+        if (asset_code is not None) and (re_credit is not None):
+            idx = [
+                index
+                for index, element in enumerate(asset_code)
+                if element in re_credit["By asset"].keys()
+            ]
+            asset_code_idx = [asset_code[i] for i in idx]
+            re_credit_rate_asset[idx] = [
+                re_credit["By asset"][ac] for ac in asset_code_idx
+            ]
+        # take the larger of the two R&E credit rates
+        inv_tax_credit += np.maximum(re_credit_rate_asset, re_credit_rate_ind)
+        print("RE_credit object =", re_credit)
+        print("inv_tax_credit object =", inv_tax_credit)
     rho = (
-        ((r - pi + delta) / (1 - u)) * (1 - inv_tax_credit - u * z) + w - delta
+        ((r - pi + delta) / (1 - u))
+        * (1 - inv_tax_credit * nu - u_d * z * (1 - psi * inv_tax_credit))
+        + w
+        - delta
     )
 
     return rho
 
 
 def eq_coc_inventory(u, phi, Y_v, pi, r):
     r"""
```

### Comparing `cost-of-capital-calculator-1.3.0/ccc/calculator.py` & `cost-of-capital-calculator-1.4.0/ccc/calculator.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,17 +192,23 @@
                     self.__p.land_expensing,
                 )
                 dfs[t]["rho_" + str(f)] = eq_coc(
                     dfs[t]["delta"],
                     dfs[t]["z_" + str(f)],
                     self.__p.property_tax,
                     self.__p.u[t],
+                    self.__p.u_d[t],
                     self.__p.inv_tax_credit,
+                    self.__p.psi,
+                    self.__p.nu,
                     self.__p.inflation_rate,
                     self.__p.r[t][f],
+                    self.__p.re_credit,
+                    dfs[t]["bea_asset_code"],
+                    dfs[t]["bea_ind_code"],
                 )
                 if not self.__p.inventory_expensing:
                     idx = dfs[t]["asset_name"] == "Inventories"
                     dfs[t].loc[idx, "rho_" + str(f)] = np.squeeze(
                         eq_coc_inventory(
                             self.__p.u[t],
                             self.__p.phi,
@@ -1375,32 +1381,32 @@
             "positions",
             "maxes",
             color=BLUE,
             line_width=2,
             source=base_source,
         )
         # Add circles for means
-        p.circle(
+        p.scatter(
             "positions",
             "means",
             size=12,
             color=BLUE,
             source=base_source,
             legend_label="Baseline",
         )
         # Add circles for maxes and mins
-        p.circle(
+        p.scatter(
             "positions",
             "mins",
             size=12,
             color=BLUE,
             source=base_source,
             legend_label="Baseline",
         )
-        p.circle(
+        p.scatter(
             "positions",
             "maxes",
             size=12,
             color=BLUE,
             source=base_source,
             legend_label="Baseline",
         )
@@ -1412,32 +1418,32 @@
             "positions",
             "maxes",
             color=RED,
             line_width=2,
             source=reform_source,
         )
         # Add circles for means
-        p.circle(
+        p.scatter(
             "positions",
             "means",
             size=12,
             color=RED,
             source=reform_source,
             legend_label="Reform",
         )
         # Add circles for maxes and mins
-        p.circle(
+        p.scatter(
             "positions",
             "mins",
             size=12,
             color=RED,
             source=reform_source,
             legend_label="Reform",
         )
-        p.circle(
+        p.scatter(
             "positions",
             "maxes",
             size=12,
             color=RED,
             source=reform_source,
             legend_label="Reform",
         )
@@ -1740,15 +1746,15 @@
         p.xaxis.major_tick_line_width = 3
         p.xaxis.minor_tick_line_color = "orange"
 
         p.outline_line_width = 1
         p.outline_line_alpha = 1
         p.outline_line_color = "black"
 
-        p.circle(
+        p.scatter(
             x="rate",
             y="short_category",
             color=BLUE,
             size="size",
             line_color="#333333",
             fill_alpha=0.4,
             source=data_sources["equip_source"],
@@ -1804,15 +1810,15 @@
         p2.outline_line_width = 0
         p2.border_fill_alpha = 0
 
         p2.xaxis.major_tick_line_color = "firebrick"
         p2.xaxis.major_tick_line_width = 3
         p2.xaxis.minor_tick_line_color = "orange"
 
-        p2.circle(
+        p2.scatter(
             x="rate",
             y="short_category",
             color=RED,
             size="size",
             line_color="#333333",
             fill_alpha=0.4,
             source=data_sources["struc_source"],
@@ -2116,15 +2122,15 @@
         p.xaxis.major_tick_line_color = "firebrick"
         p.xaxis.major_tick_line_width = 3
         p.xaxis.minor_tick_line_color = "orange"
         p.outline_line_width = 1
         p.outline_line_alpha = 1
         p.outline_line_color = "black"
 
-        p.circle(
+        p.scatter(
             x="baseline",
             y="short_category",
             color=BLUE,
             size="size",
             line_color="#333333",
             line_alpha=0.1,
             fill_alpha=0.4,
@@ -2197,15 +2203,15 @@
         # p2.min_border_top = -13
         p2.outline_line_width = 0
         p2.border_fill_alpha = 0
         p2.xaxis.major_tick_line_color = "firebrick"
         p2.xaxis.major_tick_line_width = 3
         p2.xaxis.minor_tick_line_color = "orange"
 
-        p2.circle(
+        p2.scatter(
             x="baseline",
             y="short_category",
             color=RED,
             size="size",
             line_color="#333333",
             # line_alpha=.1,
             fill_alpha=0.4,
```

### Comparing `cost-of-capital-calculator-1.3.0/ccc/ccc_asset_data.csv` & `cost-of-capital-calculator-1.4.0/ccc/ccc_asset_data.csv`

 * *Files identical despite different names*

### Comparing `cost-of-capital-calculator-1.3.0/ccc/constants.py` & `cost-of-capital-calculator-1.4.0/ccc/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,26 @@
     "delta",
     "tax_wedge",
     "eatr",
 ]
 
 OUTPUT_DATA_FORMATS = ["csv", "tex", "excel", "json", "html", None]
 
+# TODO: perhaps make as a dict so that can vary across years?
+# And if policy variant, maybe move to default params?
+RE_ASSETS = [
+    "ENS3",  # "Credit-eligible own account software",
+    "RD70",  # "Credit-eligible research and development",
+    "SU60",  # "Wind and solar power structures",
+]
+
+RE_INDUSTRIES = [
+    "3340",  # "Computer_and_Electronic_Product_Manufacturing",
+]
+
 MAJOR_IND_ORDERED = [
     "Agriculture, forestry, fishing, and hunting",
     "Mining",
     "Utilities",
     "Construction",
     "Manufacturing",
     "Wholesale trade",
@@ -44,14 +56,15 @@
 
 TAX_METHODS = {
     "DB 200%": 2.0,
     "DB 150%": 1.5,
     "SL": 1.0,
     "Economic": 1.0,
     "Expensing": 1.0,
+    "Income Forecast": 1.0,
 }
 
 MINOR_ASSET_GROUPS = dict.fromkeys(
     [
         "Mainframes",
         "PCs",
         "DASDs",
```

### Comparing `cost-of-capital-calculator-1.3.0/ccc/controls_callback_script.py` & `cost-of-capital-calculator-1.4.0/ccc/controls_callback_script.py`

 * *Files identical despite different names*

### Comparing `cost-of-capital-calculator-1.3.0/ccc/data.py` & `cost-of-capital-calculator-1.4.0/ccc/data.py`

 * *Files identical despite different names*

### Comparing `cost-of-capital-calculator-1.3.0/ccc/default_parameters.json` & `cost-of-capital-calculator-1.4.0/ccc/default_parameters.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9085931947405829%*

 * *Differences: {"'CIT_rate_ded'": "OrderedDict([('title', 'Marginal corporate income tax rate applied to "*

 * *                   "deductions'), ('description', 'Top statutory corporate income tax rate'), "*

 * *                   "('section_1', 'Business-entity level taxes'), ('type', 'float'), ('value', "*

 * *                   "[OrderedDict([('year', 2013), ('value', 0.35)]), OrderedDict([('year', 2014), "*

 * *                   "('value', 0.35)]), OrderedDict([('year', 2015), ('value', 0.35)]), "*

 * *                   "OrderedDict([('yea […]*

```diff
@@ -588,14 +588,52 @@
             },
             {
                 "value": 0.21,
                 "year": 2018
             }
         ]
     },
+    "CIT_rate_ded": {
+        "description": "Top statutory corporate income tax rate",
+        "section_1": "Business-entity level taxes",
+        "title": "Marginal corporate income tax rate applied to deductions",
+        "type": "float",
+        "validators": {
+            "range": {
+                "max": 1.0,
+                "min": 0.0
+            }
+        },
+        "value": [
+            {
+                "value": 0.35,
+                "year": 2013
+            },
+            {
+                "value": 0.35,
+                "year": 2014
+            },
+            {
+                "value": 0.35,
+                "year": 2015
+            },
+            {
+                "value": 0.35,
+                "year": 2016
+            },
+            {
+                "value": 0.35,
+                "year": 2017
+            },
+            {
+                "value": 0.21,
+                "year": 2018
+            }
+        ]
+    },
     "E_c": {
         "description": "Expected, after-tax return on corporate equity.",
         "notes": "Expected, after-tax return on corporate equity.  Default value taken from CBO (2014): https://www.cbo.gov/sites/default/files/113th-congress-2013-2014/reports/49817-taxingcapitalincome0.pdf",
         "section_1": "Individual Level Taxes",
         "section_2": "Household Savings Behavior",
         "title": "Expected, after-tax return on corporate equity",
         "type": "float",
@@ -1316,14 +1354,33 @@
             },
             {
                 "value": 0.068,
                 "year": 2020
             }
         ]
     },
+    "nu": {
+        "description": "NPV of the investment tax credit per unit of investment",
+        "notes": "For cases when the rate of return is ntn constant and losses prevent use of ITC immediately, this parameter will reflect the lower NPV of the credit by taking a value < 1.",
+        "section_1": "Investment Tax Credits and Property Tax",
+        "title": "NPV of the investment tax credit per unit of investment",
+        "type": "float",
+        "validators": {
+            "range": {
+                "max": 1.0,
+                "min": 0.0
+            }
+        },
+        "value": [
+            {
+                "value": 1.0,
+                "year": 2013
+            }
+        ]
+    },
     "omega_lcg": {
         "description": "Fraction of capital gains that are taxed at long-term rate.",
         "notes": "Fraction of capital gains that are taxed at long-term rate.  Default value taken from CBO (2014): https://www.cbo.gov/sites/default/files/113th-congress-2013-2014/reports/49817-taxingcapitalincome0.pdf",
         "section_1": "Individual Level Taxes",
         "section_2": "Household Savings Behavior",
         "title": "Fraction of capital gains that are taxed at long-term rate",
         "type": "float",
@@ -1433,19 +1490,38 @@
         "value": [
             {
                 "value": 0.0,
                 "year": 2013
             }
         ]
     },
+    "psi": {
+        "description": "Share of investment tax credit that can't be claimed for cost recovery",
+        "notes": "This parameter gives the share of the investment tax credit that can't also be claimed for cost recovery.  Some policies allow the credit to not offset the basis of the investment (or only partially do so).  Setting this parameter to a value < 1 will do that.",
+        "section_1": "Investment Tax Credits and Property Tax",
+        "title": "Share of investment tax credit that can't be claimed for cost recovery",
+        "type": "float",
+        "validators": {
+            "range": {
+                "max": 1.0,
+                "min": 0.0
+            }
+        },
+        "value": [
+            {
+                "value": 1.0,
+                "year": 2013
+            }
+        ]
+    },
     "pt_entity_tax_ind": {
         "description": "Indicator variable indicating whether or not there is an entity-level tax on pass-through businesses. This tax is levied on entity-level profits.  Owners also pay individual income taxes on the distributions.",
         "notes": "Note that is this indicator is True, then the METR calculation for pass-through businesses will represent the effects of the entity-level tax and not the indvidiual-level tax.  This is becaue the METR represents the effective tax rate from the first layer of taxation.  The statutory rate on pass-through entities is set with the pt_entity_tax_rate parameter.",
         "section_1": "Business-entity level taxes",
-        "title": "Pass-through businss entity-level tax indicator",
+        "title": "Pass-through business entity-level tax indicator",
         "type": "bool",
         "validators": {},
         "value": [
             {
                 "value": false,
                 "year": 2013
             }
@@ -1465,53 +1541,187 @@
         "value": [
             {
                 "value": 0.0,
                 "year": 2013
             }
         ]
     },
+    "pt_scale_tax_rate_ded": {
+        "description": "Ratio of marginal tax rate on deductions by pass-through businesses to marginal tax rate on their income",
+        "section_1": "Business-entity level taxes",
+        "title": "Ratio of marginal tax rate on deductions by pass-through businesses to marginal tax rate on their income",
+        "type": "float",
+        "validators": {
+            "range": {
+                "max": 1.0,
+                "min": 0.0
+            }
+        },
+        "value": [
+            {
+                "value": 1.0,
+                "year": 2013
+            }
+        ]
+    },
+    "re_credit_asset": {
+        "description": "Effective research and experimentation tax credit rate for asset types.",
+        "notes": "This parameter captures the effective research and experimentation tax credit rate. Therefore, the value of this parameter will differ from the statutory rate based on the amount of investment that is eligible for the credit. Also note that this parameter specifies the R&E credit by eligible asset. See re_credit_industry for R&E credits assigned by industry.",
+        "section_1": "Investment Tax Credits and Property Tax",
+        "title": "Research and experimentation tax credit",
+        "type": "float",
+        "validators": {
+            "range": {
+                "max": 1.0,
+                "min": 0.0
+            }
+        },
+        "value": [
+            {
+                "bea_asset_code": "ENS3",
+                "value": 0.0851,
+                "year": 2013
+            },
+            {
+                "bea_asset_code": "RD70",
+                "value": 0.0851,
+                "year": 2013
+            },
+            {
+                "bea_asset_code": "SU60",
+                "value": 0.0,
+                "year": 2013
+            },
+            {
+                "bea_asset_code": "SU60",
+                "value": 0.3328,
+                "year": 2022
+            },
+            {
+                "bea_asset_code": "SU60",
+                "value": 0.3328,
+                "year": 2023
+            },
+            {
+                "bea_asset_code": "SU60",
+                "value": 0.3328,
+                "year": 2024
+            },
+            {
+                "bea_asset_code": "SU60",
+                "value": 0.3437,
+                "year": 2025
+            },
+            {
+                "bea_asset_code": "SU60",
+                "value": 0.3476,
+                "year": 2026
+            },
+            {
+                "bea_asset_code": "SU60",
+                "value": 0.3547,
+                "year": 2027
+            },
+            {
+                "bea_asset_code": "SU60",
+                "value": 0.3641,
+                "year": 2028
+            },
+            {
+                "bea_asset_code": "SU60",
+                "value": 0.3712,
+                "year": 2029
+            },
+            {
+                "bea_asset_code": "SU60",
+                "value": 0.3737,
+                "year": 2030
+            },
+            {
+                "bea_asset_code": "SU60",
+                "value": 0.3667,
+                "year": 2031
+            },
+            {
+                "bea_asset_code": "SU60",
+                "value": 0.3667,
+                "year": 2032
+            },
+            {
+                "bea_asset_code": "SU60",
+                "value": 0.3775,
+                "year": 2033
+            },
+            {
+                "bea_asset_code": "SU60",
+                "value": 0.3709,
+                "year": 2034
+            }
+        ]
+    },
+    "re_credit_industry": {
+        "description": "Effective research and experimentation tax credit rate for certain industries.",
+        "notes": "This parameter captures the effective research and experimentation tax credit rate. Therefore, the value of this parameter will differ from the statutory rate based on the amount of investment that is eligible for the credit.",
+        "section_1": "Investment Tax Credits and Property Tax",
+        "title": "Research and experimentation tax credit",
+        "type": "float",
+        "validators": {
+            "range": {
+                "max": 1.0,
+                "min": 0.0
+            }
+        },
+        "value": [
+            {
+                "bea_ind_code": "3340",
+                "value": 0.1175,
+                "year": 2013
+            }
+        ]
+    },
     "schema": {
         "additional_members": {
             "section_1": {
                 "type": "str"
             },
             "section_2": {
                 "type": "str"
             }
         },
         "labels": {
-            "year": {
-                "type": "int",
+            "bea_asset_code": {
+                "type": "str",
                 "validators": {
                     "choice": {
                         "choices": [
-                            2013,
-                            2014,
-                            2015,
-                            2016,
-                            2017,
-                            2018,
-                            2019,
-                            2020,
-                            2021,
-                            2022,
-                            2023,
-                            2024,
-                            2025,
-                            2026,
-                            2027,
-                            2028,
-                            2029,
-                            2030,
-                            2031,
-                            2032,
-                            2033
+                            "ENS3",
+                            "RD70",
+                            "SU60"
                         ]
                     }
                 }
+            },
+            "bea_ind_code": {
+                "type": "str",
+                "validators": {
+                    "choice": {
+                        "choices": [
+                            "3340"
+                        ]
+                    }
+                }
+            },
+            "year": {
+                "type": "int",
+                "validators": {
+                    "range": {
+                        "max": 2034,
+                        "min": 2013
+                    }
+                }
             }
         }
     },
     "tau_div": {
         "description": "Effective marginal tax rate on dividends.",
         "notes": "Effective marginal tax rate on dividends.  Computed from Tax-Calculator vX.X.X using the 2009 PUF.",
         "section_1": "Individual Level Taxes",
```

### Comparing `cost-of-capital-calculator-1.3.0/ccc/get_taxcalc_rates.py` & `cost-of-capital-calculator-1.4.0/ccc/get_taxcalc_rates.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 from taxcalc import Policy, Records, Calculator
 from ccc.utils import DEFAULT_START_YEAR, TC_LAST_YEAR, RECORDS_START_YEAR
 
 
 def get_calculator(
     baseline,
     calculator_start_year,
+    baseline_policy=None,
     reform=None,
     data="cps",
     gfactors=None,
     weights=None,
     records_start_year=RECORDS_START_YEAR,
 ):
     """
     This function creates the tax calculator object for the microsim
 
     Args:
         baseline (bool): `True` if baseline tax policy
         calculator_start_year (integer): first year of budget window
+        baseline_policy (dictionary): IIT baseline parameters
         reform (dictionary): IIT reform parameters
         data (string or Pandas DataFrame): path to file or DataFrame
             for Tax-Calculator Records object (optional)
         weights (DataFrame): weights DataFrame for Tax-Calculator
             Records object (optional)
         records_start_year (integer): the start year for the data and
             weights dfs
@@ -48,18 +50,22 @@
             weights=weights,
             start_year=records_start_year,
         )  # pragma: no cover
     else:
         records1 = Records()  # pragma: no cover
 
     if baseline:
-        # Should not be a reform if baseline is True
-        assert not reform
+        if (
+            baseline_policy
+        ):  # if something other than current law policy baseline
+            update_policy(policy1, baseline_policy)
 
     if not baseline:
+        if baseline_policy:  # update baseline policy to layer reform on top
+            update_policy(policy1, baseline_policy)
         update_policy(policy1, reform)
 
     # the default set up increments year to 2013
     calc1 = Calculator(records=records1, policy=policy1)
     print("Calculator initial year = ", calc1.current_year)
 
     # this increment_year function extrapolates all PUF variables to
@@ -69,15 +75,19 @@
     while calc1.current_year < calculator_start_year:
         calc1.increment_year()
 
     return calc1
 
 
 def get_rates(
-    baseline=False, start_year=DEFAULT_START_YEAR, reform={}, data="cps"
+    baseline=False,
+    start_year=DEFAULT_START_YEAR,
+    baseline_policy=None,
+    reform={},
+    data="cps",
 ):
     """
     This function computes weighted average marginal tax rates using
     micro data from the tax calculator
 
     Args:
         baseline (bool): `True` if baseline tax policy, `False` if reform
@@ -88,14 +98,15 @@
         individual_rates (dict): individual income (IIT+payroll)
             marginal tax rates
 
     """
     calc1 = get_calculator(
         baseline=baseline,
         calculator_start_year=start_year,
+        baseline_policy=baseline_policy,
         reform=reform,
         data=data,
     )
 
     # running all the functions and calculates taxes
     calc1.calc_all()
```

### Comparing `cost-of-capital-calculator-1.3.0/ccc/parameters.py` & `cost-of-capital-calculator-1.4.0/ccc/parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,22 +22,24 @@
 
     def __init__(
         self,
         test=False,
         baseline=False,
         year=DEFAULT_START_YEAR,
         call_tc=False,
+        baseline_policy=None,
         iit_reform={},
         data="cps",
     ):
         super().__init__()
         self.set_state(year=year)
         self.test = test
         self.baseline = baseline
         self.year = year
+        self.baseline_policy = baseline_policy
         self.iit_reform = iit_reform
         self.data = data
         # initialize parameter values from JSON
         self.ccc_initialize(call_tc=call_tc)
 
     def ccc_initialize(self, call_tc=False):
         """
@@ -51,15 +53,19 @@
         Returns:
             None
 
         """
         if call_tc:
             # Find individual income tax rates from Tax-Calculator
             indiv_rates = get_rates(
-                self.baseline, self.year, self.iit_reform, self.data
+                self.baseline,
+                self.year,
+                self.baseline_policy,
+                self.iit_reform,
+                self.data,
             )
             self.tau_pt = indiv_rates["tau_pt"]
             self.tau_div = indiv_rates["tau_div"]
             self.tau_int = indiv_rates["tau_int"]
             self.tau_scg = indiv_rates["tau_scg"]
             self.tau_lcg = indiv_rates["tau_lcg"]
             self.tau_td = indiv_rates["tau_td"]
@@ -82,23 +88,31 @@
             self.m = 1
 
         # Get after-tax return to savers
         self.s, E_pt = pf.calc_s(self)
 
         # Set rate of 1st layer of taxation on investment income
         self.u = {"c": self.CIT_rate}
+        self.u_d = {"c": self.CIT_rate_ded}
         if not self.pt_entity_tax_ind.all():
             self.u["pt"] = self.tau_pt
         else:
             self.u["pt"] = self.pt_entity_tax_rate
+        self.u_d["pt"] = self.pt_scale_tax_rate_ded * self.u["pt"]
         E_dict = {"c": self.E_c, "pt": E_pt}
 
         # Allowance for Corporate Equity
         ace_dict = {"c": self.ace_c, "pt": self.ace_pt}
 
+        # Handle R&E credits which vary by industry and asset type
+        self.re_credit = {
+            "By asset": self.re_credit_asset,
+            "By industry": self.re_credit_industry,
+        }
+
         # Limitation on interest deduction
         int_haircut_dict = {
             "c": self.interest_deduct_haircut_c,
             "pt": self.interest_deduct_haircut_pt,
         }
         # Debt financing ratios
         f_dict = {
@@ -248,15 +262,22 @@
 
 
 class DepreciationRules(ma.Schema):
     # set some field validation ranges that can't set in JSON
     life = ma.fields.Float(validate=ma.validate.Range(min=0, max=100))
     method = ma.fields.String(
         validate=ma.validate.OneOf(
-            choices=["SL", "Expensing", "DB 150%", "DB 200%", "Economic"]
+            choices=[
+                "SL",
+                "Expensing",
+                "DB 150%",
+                "DB 200%",
+                "Economic",
+                "Income Forecast",
+            ]
         )
     )
 
 
 # Register custom type defined above
 paramtools.register_custom_type(
     "depreciation_rules", ma.fields.Nested(DepreciationRules())
```

### Comparing `cost-of-capital-calculator-1.3.0/ccc/paramfunctions.py` & `cost-of-capital-calculator-1.4.0/ccc/paramfunctions.py`

 * *Files identical despite different names*

### Comparing `cost-of-capital-calculator-1.3.0/ccc/records_variables.json` & `cost-of-capital-calculator-1.4.0/ccc/records_variables.json`

 * *Files identical despite different names*

### Comparing `cost-of-capital-calculator-1.3.0/ccc/styles.py` & `cost-of-capital-calculator-1.4.0/ccc/styles.py`

 * *Files identical despite different names*

### Comparing `cost-of-capital-calculator-1.3.0/ccc/tax_depreciation_rules.json` & `cost-of-capital-calculator-1.4.0/ccc/tax_depreciation_rules.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996250208245652%*

 * *Differences: {"'asset'": "{'value': {91: {'value': {'method': 'Income Forecast'}}, 92: {'value': {'method': "*

 * *            "'Income Forecast'}}}}",*

 * * "'schema'": "{'labels': {'system': {'validators': {'choice': {'choices': {insert: [(3, 'Income "*

 * *             "Forecast')]}}}}, 'year': {'validators': {'range': {'max': 2034}}}}}"}*

```diff
@@ -1284,29 +1284,29 @@
                 "GDS_life": 15.0,
                 "asset_name": "Theatrical movies",
                 "major_asset_group": "Intellectual Property",
                 "minor_asset_group": "Intellectual Property",
                 "system": "GDS",
                 "value": {
                     "life": 15,
-                    "method": "Economic"
+                    "method": "Income Forecast"
                 },
                 "year": 2020
             },
             {
                 "ADS_life": 15.0,
                 "BEA_code": "AE20",
                 "GDS_life": 15.0,
                 "asset_name": "Long-lived television programs",
                 "major_asset_group": "Intellectual Property",
                 "minor_asset_group": "Intellectual Property",
                 "system": "GDS",
                 "value": {
                     "life": 15,
-                    "method": "Economic"
+                    "method": "Income Forecast"
                 },
                 "year": 2020
             },
             {
                 "ADS_life": 15.0,
                 "BEA_code": "AE30",
                 "GDS_life": 15.0,
@@ -1698,24 +1698,25 @@
             "system": {
                 "type": "str",
                 "validators": {
                     "choice": {
                         "choices": [
                             "ADS",
                             "GDS",
-                            "Economic"
+                            "Economic",
+                            "Income Forecast"
                         ]
                     }
                 }
             },
             "year": {
                 "type": "int",
                 "validators": {
                     "range": {
-                        "max": 2030,
+                        "max": 2034,
                         "min": 2013
                     }
                 }
             }
         }
     }
 }
```

### Comparing `cost-of-capital-calculator-1.3.0/ccc/utils.py` & `cost-of-capital-calculator-1.4.0/ccc/utils.py`

 * *Files identical despite different names*

### Comparing `cost-of-capital-calculator-1.3.0/cost_of_capital_calculator.egg-info/PKG-INFO` & `cost-of-capital-calculator-1.4.0/cost_of_capital_calculator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cost-of-capital-calculator
-Version: 1.3.0
+Version: 1.4.0
 Summary: CCC: A Cost of Capital Calculator
 Home-page: https://github.com/PSLmodels/Cost-of-Capital-Calculator
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Download-URL: https://github.com/PSLmodels/Cost-of-Capital-Calculator
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -70,10 +70,10 @@
 
 
 ## Disclaimer
 Results will change as the underlying models improve. A fundamental reason for adopting open source methods in this project is so that people from all backgrounds can contribute to the models that our society uses to assess economic policy; when community-contributed improvements are incorporated, the model will produce different results.
 
 
 ## Citing the Cost-of-Capital-Calculator Model
-Cost-of-Capital-Calculator (Version 1.3.0)[Source code], https://github.com/PSLmodels/Cost-of-Capital-Calculator
+Cost-of-Capital-Calculator (Version 1.4.0)[Source code], https://github.com/PSLmodels/Cost-of-Capital-Calculator
```

### Comparing `cost-of-capital-calculator-1.3.0/cost_of_capital_calculator.egg-info/SOURCES.txt` & `cost-of-capital-calculator-1.4.0/cost_of_capital_calculator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cost-of-capital-calculator-1.3.0/setup.py` & `cost-of-capital-calculator-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 with open("README.md") as f:
     longdesc = f.read()
 
-version = "1.3.0"
+version = "1.4.0"
 
 config = {
     "description": "CCC: A Cost of Capital Calculator",
     "url": "https://github.com/PSLmodels/Cost-of-Capital-Calculator",
     "download_url": "https://github.com/PSLmodels/Cost-of-Capital-Calculator",
     "long_description_content_type": "text/markdown",
     "long_description": longdesc,
```

