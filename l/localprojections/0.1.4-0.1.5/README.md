# Comparing `tmp/localprojections-0.1.4.tar.gz` & `tmp/localprojections-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localprojections-0.1.4.tar", last modified: Mon Apr  1 06:52:12 2024, max compression
+gzip compressed data, was "localprojections-0.1.5.tar", last modified: Thu Apr 25 05:27:08 2024, max compression
```

## Comparing `localprojections-0.1.4.tar` & `localprojections-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 06:52:12.887005 localprojections-0.1.4/
--rw-rw-rw-   0        0        0     1090 2024-04-01 06:48:44.000000 localprojections-0.1.4/LICENSE
--rw-rw-rw-   0        0        0    17277 2024-04-01 06:52:12.884469 localprojections-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    15132 2024-04-01 06:48:44.000000 localprojections-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 06:52:12.867540 localprojections-0.1.4/localprojections/
--rw-rw-rw-   0        0        0      501 2024-04-01 06:48:44.000000 localprojections-0.1.4/localprojections/__init__.py
--rw-rw-rw-   0        0        0      126 2024-04-01 06:48:44.000000 localprojections-0.1.4/localprojections/__main__.py
--rw-rw-rw-   0        0        0    70380 2024-04-01 06:48:44.000000 localprojections-0.1.4/localprojections/lp.py
-drwxrwxrwx   0        0        0        0 2024-04-01 06:52:12.883000 localprojections-0.1.4/localprojections.egg-info/
--rw-rw-rw-   0        0        0    17277 2024-04-01 06:52:12.000000 localprojections-0.1.4/localprojections.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2024-04-01 06:52:12.000000 localprojections-0.1.4/localprojections.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 06:52:12.000000 localprojections-0.1.4/localprojections.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-04-01 06:52:12.000000 localprojections-0.1.4/localprojections.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       88 2024-04-01 06:52:12.000000 localprojections-0.1.4/localprojections.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-01 06:52:12.000000 localprojections-0.1.4/localprojections.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1111 2024-04-01 06:48:44.000000 localprojections-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-01 06:52:12.887005 localprojections-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-25 05:27:08.009297 localprojections-0.1.5/
+-rw-rw-rw-   0        0        0     1090 2024-04-01 06:48:44.000000 localprojections-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0    17277 2024-04-25 05:27:08.005828 localprojections-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    15132 2024-04-01 06:48:44.000000 localprojections-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 05:27:07.989399 localprojections-0.1.5/localprojections/
+-rw-rw-rw-   0        0        0      533 2024-04-25 05:25:18.000000 localprojections-0.1.5/localprojections/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-04-01 06:48:44.000000 localprojections-0.1.5/localprojections/__main__.py
+-rw-rw-rw-   0        0        0    81506 2024-04-25 05:25:18.000000 localprojections-0.1.5/localprojections/lp.py
+drwxrwxrwx   0        0        0        0 2024-04-25 05:27:08.003843 localprojections-0.1.5/localprojections.egg-info/
+-rw-rw-rw-   0        0        0    17277 2024-04-25 05:27:07.000000 localprojections-0.1.5/localprojections.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2024-04-25 05:27:07.000000 localprojections-0.1.5/localprojections.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 05:27:07.000000 localprojections-0.1.5/localprojections.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-04-25 05:27:07.000000 localprojections-0.1.5/localprojections.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       88 2024-04-25 05:27:07.000000 localprojections-0.1.5/localprojections.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-25 05:27:07.000000 localprojections-0.1.5/localprojections.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1111 2024-04-25 05:26:11.000000 localprojections-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-25 05:27:08.011319 localprojections-0.1.5/setup.cfg
```

### Comparing `localprojections-0.1.4/LICENSE` & `localprojections-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `localprojections-0.1.4/PKG-INFO` & `localprojections-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localprojections
-Version: 0.1.4
+Version: 0.1.5
 Summary: This module implements the local projections models for single entity time series and panel / longitudinal data, as well as threshold versions.
 Author-email: Jing Lian Suah <suahjinglian@bnm.gov.my>
 License: MIT License
         
         Copyright (c) 2024 Jing Lian Suah
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `localprojections-0.1.4/README.md` & `localprojections-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `localprojections-0.1.4/localprojections/lp.py` & `localprojections-0.1.5/localprojections/lp.py`

 * *Files 10% similar despite different names*

```diff
@@ -959,15 +959,15 @@
     # reference for LP regressions
     col_entity = Entity
     # Column names of the output dataframe
     col_output = [
         "Shock",
         "Response",
         "Horizon",
-        "Point",
+        "Mean",
         "LB",
         "UB",
     ]  
     # Empty output dataframe to be filled over every iteration
     irf_full = pd.DataFrame(
         columns=col_output
     ) 
@@ -1051,29 +1051,263 @@
                 irf = pd.DataFrame(
                     [[1] * len(col_output)], columns=col_output
                 )  # double list = single row
                 irf["Response"] = r
                 irf["Horizon"] = h
                 if z == r:  # shock = response
                     irf["Shock"] = r
-                    irf["Point"] = beta_ownshock[z]
+                    irf["Mean"] = beta_ownshock[z]
                     irf["LB"] = beta_ownshock[z] - z_val * se_ownshock[z]
                     irf["UB"] = beta_ownshock[z] + z_val * se_ownshock[z]
                 else:  # shock =/= response
                     irf["Shock"] = z
-                    irf["Point"] = beta[z]
+                    irf["Mean"] = beta[z]
                     irf["LB"] = beta[z] - z_val * se[z]
                     irf["UB"] = beta[z] + z_val * se[z]
                 irf_full = pd.concat([irf_full, irf], axis=0)  # top to bottom concat
     ## Sort by response, shock, horizon
     irf_full = irf_full.sort_values(
         by=["Response", "Shock", "Horizon"], axis=0, ascending=[True, True, True]
     )
     return irf_full
 
+### ThresholdPanelQuantileLPX
+## Input attributes
+# This is almost identical procedurally with the Panel version
+# data = pandas dataframe (each row = 1 period)
+# Y = list of variables, cholesky ordered (last = contemporaneous shock from all previous variables)
+# X = list of exogenous variables, to be entered contemporaneously into the model; must not overlap with elements of Y
+# threshold_var = dummy variable to be interacted with endogenous and exogenous variables on the RHS; see Goncalves et al (2022) for more info at https://www.dallasfed.org/~/media/documents/research/papers/2022/wp2205.pdf
+# response = list of variables contained in Y to be shocked
+# horizon = integer indicating estimation horizon for the IRFs (e.g., input 8 for 8 quarters ahead)
+# lags = integer indicating number of lags to be used in the estimation models (e.g., 4 for 4 lags)
+# newey_lags = max lags for Newey-West HAC SEs
+# ci_width = float within (0, 1) indicating the width of the confidence band (e.g., 0.95 for 95% CI)
+def ThresholdPanelQuantileLPX(
+    data, 
+    Y, 
+    X, 
+    Entity,
+    threshold_var, 
+    response, 
+    horizon, 
+    lags, 
+    varcov="robust", 
+    kernel="epa", 
+    bandwidth="hsheather", 
+    ci_width=0.95, 
+    quantile=0.5
+):
+    ## Illegal inputs
+    if (ci_width >= 1) | (ci_width <= 0):
+        raise NotImplementedError("CI Width must be within (0, 1), non-inclusive!")
+    if horizon < 1:
+        raise NotImplementedError("Estimation horizon for IRFs must be at least 1")
+    if lags < 1:
+        raise NotImplementedError("Number of lags in the model must be at least 1")
+    if any(col in X for col in Y):
+        raise NotImplementedError(
+            "Exogenous and endogenous blocks overlap! Please ensure they are mutually exclusive"
+        )
+    if any(threshold_var in col for col in Y):
+        raise NotImplementedError(
+            "Threshold variable and endogenous block overlap! Please ensure they are mutually exclusive"
+        )
+    if any(threshold_var in col for col in X):
+        raise NotImplementedError(
+            "Threshold variable and exogenous block overlap! Please ensure they are mutually exclusive"
+        )
+    ## Preliminaries
+    # deep copy
+    df = data.copy()
+    # fixed effects dummies
+    cols_entity_dummies = []
+    for entity in list(df[Entity].unique()):
+        df.loc[df[Entity] == entity, entity] = 1
+        df.loc[df[entity].isna(), entity] = 0
+        df[entity] = df[entity].astype("int")
+        cols_entity_dummies += [entity]
+    # reference for LP regressions
+    col_entity = Entity
+    # Column names of the output dataframe
+    col_output = [
+        "Shock",
+        "Response",
+        "Horizon",
+        "Mean",
+        "LB",
+        "UB",
+    ]  
+    # Empty output dataframe to be filled over every iteration (for H = 1)
+    irf_on_full = pd.DataFrame(
+        columns=col_output
+    )  
+    # Empty output dataframe to be filled over every iteration (for H = 0)
+    irf_off_full = pd.DataFrame(
+        columns=col_output
+    )  
+    # Determines what multiplier to use when calculating UB & LB from SE
+    z_val = NormalDist().inv_cdf(
+        (1 + ci_width) / 2
+    )  
+
+    for r in response:
+        ## Check ordering of response variable in the full list of Y
+        r_loc = Y.index(r)
+        ## Generate copy of data for horizon h + first difference RHS variables + transform response variable to desired horizon
+        for h in range(horizon + 1):
+            d = df.copy()
+            d[r + "forward"] = d.groupby(col_entity)[r].shift(
+                -h
+            )  # forward; equivalent to F`h'. in Stata
+            ## Generate lags of RHS variables (only the first, either l0 or l1 will be used in the IRFs)
+            list_RHS_forReg = []
+            list_RHS_forIRF = []
+            for y in Y:
+                d[y] = d[y] - d.groupby(col_entity)[y].shift(1)  # first difference
+                if Y.index(y) == r_loc:  # include lagged response variables on the RHS
+                    for l in range(1, lags + 1):
+                        d[y + str(l) + "lag"] = d.groupby(col_entity)[y].shift(
+                            l
+                        )  # for lagged dependent variable, we will use _l1 to generate the IRF
+                        list_RHS_forReg = list_RHS_forReg + [y + str(l) + "lag"]
+                    list_RHS_forIRF = list_RHS_forIRF + [
+                        y
+                    ]  # to figure out if the own-shock model should be used
+                if Y.index(y) < r_loc:  # y affects r contemporaneously
+                    list_RHS_forReg = list_RHS_forReg + [y]
+                    list_RHS_forIRF = list_RHS_forIRF + [y]
+                    for l in range(1, lags + 1):
+                        d[y + str(l) + "lag"] = d.groupby(col_entity)[y].shift(
+                            l
+                        )  # keep original name for convenience (d[y] = _l0 will be used for IRF)
+                        list_RHS_forReg = list_RHS_forReg + [y + str(l) + "lag"]
+                elif Y.index(y) > r_loc:  # y affects r with a lag
+                    list_RHS_forReg = list_RHS_forReg + [y]
+                    list_RHS_forIRF = list_RHS_forIRF + [y]
+                    for l in range(2, lags + 1):
+                        d[y + str(l) + "lag"] = d.groupby(col_entity)[y].shift(l)
+                        list_RHS_forReg = list_RHS_forReg + [y + str(l) + "lag"]
+                    d[y] = d[y].shift(
+                        1
+                    )  # replace original with first lag (d[y] = _l1 will be used for IRF)
+            d = d.dropna(
+                axis=0
+            )  # clear all rows with NAs from the lag / forward transformations
+            # Now add the threshold interactions (X_{t-k} * H_{t-1} for k = 0,1,2,3, ..., h)
+            # first generate lagged threshold indicator
+            d[threshold_var] = d.groupby(col_entity)[threshold_var].shift(1)
+            d["threshold_on"] = d[threshold_var].copy()
+            d["threshold_off"] = 1 - d[threshold_var]
+            # split RHS lists into "regime on", and "regime off"
+            # regime on
+            list_RHS_forReg_On = list_RHS_forReg.copy()
+            list_RHS_forIRF_On = list_RHS_forIRF.copy()
+            list_RHS_forReg_On = [i + ":" + "threshold_on" for i in list_RHS_forReg_On]
+            list_RHS_forIRF_On = [i + ":" + "threshold_on" for i in list_RHS_forIRF_On]
+            # regime off
+            list_RHS_forReg_Off = list_RHS_forReg.copy()
+            list_RHS_forIRF_Off = list_RHS_forIRF.copy()
+            list_RHS_forReg_Off = [
+                i + ":" + "threshold_off" for i in list_RHS_forReg_Off
+            ]
+            list_RHS_forIRF_Off = [
+                i + ":" + "threshold_off" for i in list_RHS_forIRF_Off
+            ]
+            # iInteract threshold indicator with exog variables too
+            X_On = [i + ":" + "threshold_on" for i in X]
+            X_Off = [i + ":" + "threshold_off" for i in X]
+            # Estimate the model
+            eqn = (
+                r
+                + "forward"
+                + "~"
+                + "+".join(cols_entity_dummies)
+                + "+"
+                + "+".join(list_RHS_forReg_On)
+                + "+"
+                + "+".join(list_RHS_forReg_Off)
+                + "+"
+                + "+".join(X_On)
+                + "+"
+                + "+".join(X_Off)
+                + "+threshold_on+threshold_off"
+            )
+            eqn_ownshock = (
+                r
+                + "forward"
+                + "~"
+                + "+".join(cols_entity_dummies)
+                + "+"
+                + "+".join([r + ":threshold_on"] + list_RHS_forReg_On)
+                + "+"
+                + "+".join([r + ":threshold_off"] + list_RHS_forReg_Off)
+                + "+"
+                + "+".join(X_On)
+                + "+"
+                + "+".join(X_Off)
+                + "+threshold_on +threshold_off"
+            )  # own-shock model includes contemp first diff dependent
+            mod = smf.quantreg(formula=eqn, data=d)
+            mod_ownshock = smf.quantreg(formula=eqn_ownshock, data=d)  # own-shock model
+            est = mod.fit(q=quantile, vcov=varcov, kernel=kernel, bandwidth=bandwidth)
+            est_ownshock = mod_ownshock.fit(q=quantile, vcov=varcov, kernel=kernel, bandwidth=bandwidth)  # own-shock mode
+            beta = est.params
+            beta_ownshock = est_ownshock.params  # own-shock model
+            se = est.bse
+            se_ownshock = est_ownshock.bse  # own-shock model
+            # IRF for H = 1
+            for z, znice in zip(list_RHS_forIRF_On, list_RHS_forIRF):
+                irf = pd.DataFrame(
+                    [[1] * len(col_output)], columns=col_output
+                )  # double list = single row
+                irf["Response"] = r
+                irf["Horizon"] = h
+                if r in znice:  # shock = response (diff from other functions)
+                    irf["Shock"] = r
+                    irf["Mean"] = beta_ownshock[z]
+                    irf["LB"] = beta_ownshock[z] - z_val * se_ownshock[z]
+                    irf["UB"] = beta_ownshock[z] + z_val * se_ownshock[z]
+                else:  # shock =/= response
+                    irf["Shock"] = znice
+                    irf["Mean"] = beta[z]
+                    irf["LB"] = beta[z] - z_val * se[z]
+                    irf["UB"] = beta[z] + z_val * se[z]
+                irf_on_full = pd.concat(
+                    [irf_on_full, irf], axis=0
+                )  # top to bottom concat
+            # IRF for H = 0
+            for z, znice in zip(list_RHS_forIRF_Off, list_RHS_forIRF):
+                irf = pd.DataFrame(
+                    [[1] * len(col_output)], columns=col_output
+                )  # double list = single row
+                irf["Response"] = r
+                irf["Horizon"] = h
+                if r in znice:  # shock = response (diff from other functions)
+                    irf["Shock"] = r
+                    irf["Mean"] = beta_ownshock[z]
+                    irf["LB"] = beta_ownshock[z] - z_val * se_ownshock[z]
+                    irf["UB"] = beta_ownshock[z] + z_val * se_ownshock[z]
+                else:  # shock =/= response
+                    irf["Shock"] = znice
+                    irf["Mean"] = beta[z]
+                    irf["LB"] = beta[z] - z_val * se[z]
+                    irf["UB"] = beta[z] + z_val * se[z]
+                irf_off_full = pd.concat(
+                    [irf_off_full, irf], axis=0
+                )  # top to bottom concat
+    ## Sort by response, shock, horizon
+    irf_on_full = irf_on_full.sort_values(
+        by=["Response", "Shock", "Horizon"], axis=0, ascending=[True, True, True]
+    )
+    irf_off_full = irf_off_full.sort_values(
+        by=["Response", "Shock", "Horizon"], axis=0, ascending=[True, True, True]
+    )
+    return irf_on_full, irf_off_full
+
 
 
 ### PanelQuantileLP
 ## Input attributes
 # Implements panel quantile regression using statsmodels and entity dummies (rather than "de-mean" fixed effects) without exogenous block
 # data = pandas dataframe (each row = 1 period)
 # Y = list of variables, cholesky ordered (last = contemporaneous shock from all previous variables)
@@ -1117,15 +1351,15 @@
     # reference for LP regressions
     col_entity = Entity
     # Column names of the output dataframe
     col_output = [
         "Shock",
         "Response",
         "Horizon",
-        "Point",
+        "Mean",
         "LB",
         "UB",
     ]  
     # Empty output dataframe to be filled over every iteration
     irf_full = pd.DataFrame(
         columns=col_output
     ) 
@@ -1205,20 +1439,20 @@
                 irf = pd.DataFrame(
                     [[1] * len(col_output)], columns=col_output
                 )  # double list = single row
                 irf["Response"] = r
                 irf["Horizon"] = h
                 if z == r:  # shock = response
                     irf["Shock"] = r
-                    irf["Point"] = beta_ownshock[z]
+                    irf["Mean"] = beta_ownshock[z]
                     irf["LB"] = beta_ownshock[z] - z_val * se_ownshock[z]
                     irf["UB"] = beta_ownshock[z] + z_val * se_ownshock[z]
                 else:  # shock =/= response
                     irf["Shock"] = z
-                    irf["Point"] = beta[z]
+                    irf["Mean"] = beta[z]
                     irf["LB"] = beta[z] - z_val * se[z]
                     irf["UB"] = beta[z] + z_val * se[z]
                 irf_full = pd.concat([irf_full, irf], axis=0)  # top to bottom concat
     ## Sort by response, shock, horizon
     irf_full = irf_full.sort_values(
         by=["Response", "Shock", "Horizon"], axis=0, ascending=[True, True, True]
     )
```

### Comparing `localprojections-0.1.4/localprojections.egg-info/PKG-INFO` & `localprojections-0.1.5/localprojections.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localprojections
-Version: 0.1.4
+Version: 0.1.5
 Summary: This module implements the local projections models for single entity time series and panel / longitudinal data, as well as threshold versions.
 Author-email: Jing Lian Suah <suahjinglian@bnm.gov.my>
 License: MIT License
         
         Copyright (c) 2024 Jing Lian Suah
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `localprojections-0.1.4/pyproject.toml` & `localprojections-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "localprojections"
-version = "0.1.4"
+version = "0.1.5"
 description = "This module implements the local projections models for single entity time series and panel / longitudinal data, as well as threshold versions."
 readme = "README.md"
 authors = [{ name = "Jing Lian Suah", email = "suahjinglian@bnm.gov.my" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

