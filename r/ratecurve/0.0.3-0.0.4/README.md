# Comparing `tmp/ratecurve-0.0.3.tar.gz` & `tmp/ratecurve-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratecurve-0.0.3.tar", last modified: Mon Apr 22 23:51:40 2024, max compression
+gzip compressed data, was "ratecurve-0.0.4.tar", last modified: Thu Apr 25 14:45:40 2024, max compression
```

## Comparing `ratecurve-0.0.3.tar` & `ratecurve-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 disent    (1000) disent    (1000)        0 2024-04-22 23:51:40.965411 ratecurve-0.0.3/
--rw-r--r--   0 disent    (1000) disent    (1000)    11357 2024-04-11 17:03:55.000000 ratecurve-0.0.3/LICENSE
--rw-r--r--   0 disent    (1000) disent    (1000)       49 2024-04-17 21:48:00.000000 ratecurve-0.0.3/MANIFEST.in
--rw-r--r--   0 disent    (1000) disent    (1000)     1019 2024-04-22 23:51:40.965411 ratecurve-0.0.3/PKG-INFO
--rw-r--r--   0 disent    (1000) disent    (1000)     2283 2024-04-22 23:34:39.000000 ratecurve-0.0.3/README.md
-drwxr-xr-x   0 disent    (1000) disent    (1000)        0 2024-04-22 23:51:40.965411 ratecurve-0.0.3/ratecurve/
--rw-r--r--   0 disent    (1000) disent    (1000)       47 2024-04-22 20:10:42.000000 ratecurve-0.0.3/ratecurve/__init__.py
--rw-r--r--   0 disent    (1000) disent    (1000)        0 2024-04-17 21:10:09.000000 ratecurve-0.0.3/ratecurve/__main__.py
--rw-r--r--   0 disent    (1000) disent    (1000)     1555 2024-04-22 23:39:48.000000 ratecurve-0.0.3/ratecurve/equations.py
--rw-r--r--   0 disent    (1000) disent    (1000)     9485 2024-04-22 23:45:06.000000 ratecurve-0.0.3/ratecurve/ratecurve.py
--rw-r--r--   0 disent    (1000) disent    (1000)     3167 2024-04-22 22:15:19.000000 ratecurve-0.0.3/ratecurve/utils.py
-drwxr-xr-x   0 disent    (1000) disent    (1000)        0 2024-04-22 23:51:40.965411 ratecurve-0.0.3/ratecurve.egg-info/
--rw-r--r--   0 disent    (1000) disent    (1000)     1019 2024-04-22 23:51:40.000000 ratecurve-0.0.3/ratecurve.egg-info/PKG-INFO
--rw-r--r--   0 disent    (1000) disent    (1000)      447 2024-04-22 23:51:40.000000 ratecurve-0.0.3/ratecurve.egg-info/SOURCES.txt
--rw-r--r--   0 disent    (1000) disent    (1000)        1 2024-04-22 23:51:40.000000 ratecurve-0.0.3/ratecurve.egg-info/dependency_links.txt
--rw-r--r--   0 disent    (1000) disent    (1000)        1 2024-04-18 15:56:39.000000 ratecurve-0.0.3/ratecurve.egg-info/not-zip-safe
--rw-r--r--   0 disent    (1000) disent    (1000)       28 2024-04-22 23:51:40.000000 ratecurve-0.0.3/ratecurve.egg-info/requires.txt
--rw-r--r--   0 disent    (1000) disent    (1000)       10 2024-04-22 23:51:40.000000 ratecurve-0.0.3/ratecurve.egg-info/top_level.txt
--rw-r--r--   0 disent    (1000) disent    (1000)       38 2024-04-22 23:51:40.965411 ratecurve-0.0.3/setup.cfg
--rw-r--r--   0 disent    (1000) disent    (1000)     1173 2024-04-22 23:50:56.000000 ratecurve-0.0.3/setup.py
-drwxr-xr-x   0 disent    (1000) disent    (1000)        0 2024-04-22 23:51:40.965411 ratecurve-0.0.3/tests/
--rw-r--r--   0 disent    (1000) disent    (1000)     4174 2024-04-22 15:31:54.000000 ratecurve-0.0.3/tests/test_curve.py
--rw-r--r--   0 disent    (1000) disent    (1000)     2482 2024-04-22 15:31:54.000000 ratecurve-0.0.3/tests/test_equations.py
--rw-r--r--   0 disent    (1000) disent    (1000)      711 2024-04-22 22:26:14.000000 ratecurve-0.0.3/tests/test_suite.py
--rw-r--r--   0 disent    (1000) disent    (1000)     1222 2024-04-22 23:45:59.000000 ratecurve-0.0.3/tests/test_usage.py
--rw-r--r--   0 disent    (1000) disent    (1000)     3071 2024-04-22 15:31:54.000000 ratecurve-0.0.3/tests/test_utils.py
+drwxr-xr-x   0 disent    (1000) disent    (1000)        0 2024-04-25 14:45:40.276218 ratecurve-0.0.4/
+-rw-r--r--   0 disent    (1000) disent    (1000)    11357 2024-04-11 17:03:55.000000 ratecurve-0.0.4/LICENSE
+-rw-r--r--   0 disent    (1000) disent    (1000)       49 2024-04-17 21:48:00.000000 ratecurve-0.0.4/MANIFEST.in
+-rw-r--r--   0 disent    (1000) disent    (1000)     1019 2024-04-25 14:45:40.276218 ratecurve-0.0.4/PKG-INFO
+-rw-r--r--   0 disent    (1000) disent    (1000)     2283 2024-04-22 23:34:39.000000 ratecurve-0.0.4/README.md
+drwxr-xr-x   0 disent    (1000) disent    (1000)        0 2024-04-25 14:45:40.276218 ratecurve-0.0.4/ratecurve/
+-rw-r--r--   0 disent    (1000) disent    (1000)       47 2024-04-22 20:10:42.000000 ratecurve-0.0.4/ratecurve/__init__.py
+-rw-r--r--   0 disent    (1000) disent    (1000)        0 2024-04-17 21:10:09.000000 ratecurve-0.0.4/ratecurve/__main__.py
+-rw-r--r--   0 disent    (1000) disent    (1000)     1569 2024-04-25 14:23:55.000000 ratecurve-0.0.4/ratecurve/equations.py
+-rw-r--r--   0 disent    (1000) disent    (1000)    15571 2024-04-25 14:33:51.000000 ratecurve-0.0.4/ratecurve/ratecurve.py
+-rw-r--r--   0 disent    (1000) disent    (1000)     3352 2024-04-24 20:32:23.000000 ratecurve-0.0.4/ratecurve/utils.py
+drwxr-xr-x   0 disent    (1000) disent    (1000)        0 2024-04-25 14:45:40.276218 ratecurve-0.0.4/ratecurve.egg-info/
+-rw-r--r--   0 disent    (1000) disent    (1000)     1019 2024-04-25 14:45:40.000000 ratecurve-0.0.4/ratecurve.egg-info/PKG-INFO
+-rw-r--r--   0 disent    (1000) disent    (1000)      447 2024-04-25 14:45:40.000000 ratecurve-0.0.4/ratecurve.egg-info/SOURCES.txt
+-rw-r--r--   0 disent    (1000) disent    (1000)        1 2024-04-25 14:45:40.000000 ratecurve-0.0.4/ratecurve.egg-info/dependency_links.txt
+-rw-r--r--   0 disent    (1000) disent    (1000)        1 2024-04-18 15:56:39.000000 ratecurve-0.0.4/ratecurve.egg-info/not-zip-safe
+-rw-r--r--   0 disent    (1000) disent    (1000)       28 2024-04-25 14:45:40.000000 ratecurve-0.0.4/ratecurve.egg-info/requires.txt
+-rw-r--r--   0 disent    (1000) disent    (1000)       10 2024-04-25 14:45:40.000000 ratecurve-0.0.4/ratecurve.egg-info/top_level.txt
+-rw-r--r--   0 disent    (1000) disent    (1000)       38 2024-04-25 14:45:40.276218 ratecurve-0.0.4/setup.cfg
+-rw-r--r--   0 disent    (1000) disent    (1000)     1173 2024-04-25 14:44:57.000000 ratecurve-0.0.4/setup.py
+drwxr-xr-x   0 disent    (1000) disent    (1000)        0 2024-04-25 14:45:40.276218 ratecurve-0.0.4/tests/
+-rw-r--r--   0 disent    (1000) disent    (1000)     9133 2024-04-25 14:30:35.000000 ratecurve-0.0.4/tests/test_curve.py
+-rw-r--r--   0 disent    (1000) disent    (1000)     2544 2024-04-25 14:28:30.000000 ratecurve-0.0.4/tests/test_equations.py
+-rw-r--r--   0 disent    (1000) disent    (1000)      711 2024-04-22 22:26:14.000000 ratecurve-0.0.4/tests/test_suite.py
+-rw-r--r--   0 disent    (1000) disent    (1000)     2067 2024-04-24 19:09:55.000000 ratecurve-0.0.4/tests/test_usage.py
+-rw-r--r--   0 disent    (1000) disent    (1000)     3071 2024-04-22 15:31:54.000000 ratecurve-0.0.4/tests/test_utils.py
```

### Comparing `ratecurve-0.0.3/LICENSE` & `ratecurve-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ratecurve-0.0.3/PKG-INFO` & `ratecurve-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratecurve
-Version: 0.0.3
+Version: 0.0.4
 Summary: simple utility for curve interpolation
 Home-page: https://github.com/disentcorp/ratecurve
 Author: Disent
 Author-email: chris@disent.com
 License: Apache Software License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ratecurve-0.0.3/README.md` & `ratecurve-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ratecurve-0.0.3/ratecurve/equations.py` & `ratecurve-0.0.4/ratecurve/equations.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,19 +32,18 @@
     """
     return 1 / cap_factor(r, t, method)
 
 
 def convert_cap_factor_to_rate(cf, t, method, default=None):
     """
     Converts cap_factor to rate. If default provided, will serve as default answer
-    when t = 0.
+    when t = 0 or cf = 1.
     """
-    if t == 0:
-        return np.inf if default is None else default
-    
+    if t == 0 or cf==1:
+        return np.nan if default is None else default
     if method == "EXP":
         r = ln(cf) / t
     elif method == "YLD":
         r = (cf ** (1 / t)) - 1
     elif method == "LIN":
         r = (cf - 1) / t
     else:
```

### Comparing `ratecurve-0.0.3/ratecurve/ratecurve.py` & `ratecurve-0.0.4/ratecurve/ratecurve.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import numpy as np
 import pandas as pd
 from dateroll import Duration, ddh
 from scipy import interpolate
 
 from ratecurve import equations, utils
 
 # Standin for upcoming dateroll features
@@ -28,14 +29,15 @@
         self,
         d,
         dc="ACT/365",
         cal="ALL",
         method="EXP",
         interp_on="ln(df)",
         interp_method="linear",
+        extrap_method='flat',
         base="t",
     ):
         """
         Parameters
         -----------
         d
             Dict or dict-like raw rate data to construct curve.  Given in form {[tenor/date]:[rate]}.
@@ -46,26 +48,31 @@
             Holiday calendar used in day count calculations. Only "ALL" supported for right now.
         method
             Compounding method for discount and cap factors. Supports 'EXP', 'LIN', and 'YLD'.
         interp_on
             Y-transformation performed on rates before interpolating. Support for 'ln(df)', 'r*t' and 'r'.
         interp_method
             Kind of interpolation performed on data. See scipy.interp1d documentation for details.
+        extrap_method
+            Kind of extrapolation performed on dates outside of date bounds given. Can be either 'flat' or 'extrapolate'.
+            'flat' will return earliest value given for all dates prior. 'extrapolate' will extrapolate from interpolated
+            curve. See scipy.interp1d documentation for details.      
         base
             Date at head of curve. Default is current date.
         """
         self.base = ddh(base)  # Base is always in date form
         self.dc = dc
         self.method = method
         self.interp_on = interp_on
         self.cal = cal
         self.interp_method = interp_method
+        self.extrap_method = extrap_method
         # Transformations for input and outputs to interpolation
         self.to_x = lambda x: self.make_date_a_number(x)
-        self.to_y, self.from_y = self.get_y_transformers(interp_on, method)
+        self.to_y, self.from_y, = self.get_y_transformers(interp_on, method)
 
         # Data processing and validation will parse and store dates and rates
         if isinstance(d, dict):
             self.dates, self.rates = self.validate_data(d)
         elif isinstance(d, pd.Series):
             data = d.to_dict()
             self.dates, self.rates = self.validate_data(data)
@@ -93,36 +100,96 @@
     def validate_data(self, data):
         """
         Validates input data is of type {[date-like]:rate} and returns list of dates and
         a list of rates for interpolation.
         """
         x = []
         y = []
-        base_rate = None  # Rate associated with earliest date
+        earliest_date = None
+        latest_date = None
+        earliest_rate = None 
+        latest_rate = None
         for i in data.items():
             key = i[0]
             val = i[1]
             try:
                 # Convert key to date
                 key_as_date = self.to_date(key)
                 if not isinstance(val, float):
                     raise
                 x.append(key_as_date)
                 y.append(val)
-                if key_as_date == self.base:  
-                    # Case where rate data contains a 0-tenor. Will need the rate at base_date
-                    # to avoid complications from calling self.spot(base_date)
-                    base_rate = val
+                if earliest_date is None or key_as_date < earliest_date:
+                    earliest_date = key_as_date 
+                    earliest_rate = val
+                if latest_date is None or key_as_date > latest_date:
+                    latest_date = key_as_date 
+                    latest_rate = val           
+            
             except Exception:
                 raise ValueError(
                     "Invalid data. Data must be of form {[date-like object]:float}"
                 )
+        # ###WHEREDOESTHISGO    
+        # if self.interp_on == "ln(df)":
+        #     # Will not interpolate properly on ln(df) if x = 0 is not provided
+        #     x.append(self.base)
+        #     y.append(None)
+
         self.raw_data = data
-        self.base_rate = base_rate
+        self.earliest_date = earliest_date
+        self.earliest_rate = earliest_rate
+        self.latest_date = latest_date
+        self.latest_rate = latest_rate
         return x, y
+    
+    def get_y_transformers(self, interp_on, method):
+        """
+        Returns 2 functions:
+            1. Convert raw rates into interpolated form
+            2. Convert interpolated form to raw_rates
+        """
+        def to_y(t, rate):
+            # From rate to interpolated form
+            r = rate
+            if interp_on == "r":
+                return r
+            elif interp_on in ("rt", "r*t"):
+                return r * t
+            elif interp_on == "ln(df)":
+                ###WHEREDOESTHISGO
+                if t == 0:
+                    return 0
+                else:
+                    df = equations.disc_factor(r, t, method)
+                    return equations.ln(df)
+            else:
+                raise ValueError(f"Unknown interp_on {interp_on}")
+
+        def from_y(t, y):
+            # From interpolated form to cap factor
+            if t <= 0:
+                return 1
+            # Perform time adjustment for flat extrapolation
+            if self.extrap_method == 'flat':
+                if t < self._t(self.earliest_date):
+                    t = self._t(self.earliest_date)
+                elif t > self._t(self.latest_date):
+                    t = self._t(self.latest_date)
+            # Return cap factors based on interp_on
+            if interp_on == "r":
+                return equations.cap_factor(y, t, self.method)
+            elif interp_on in ("rt", "r*t"):
+                return equations.cap_factor(y / t, t, self.method)
+            elif interp_on == "ln(df)":
+                df = equations.e**y     
+                return 1 / df
+
+        return to_y, from_y, 
+    
 
     def to_date(self, datelike):
         """
         Converts tenors to dates relative to Curve.base date.
         """
         return utils.to_dateroll_date(datelike, self.base)
 
@@ -133,73 +200,57 @@
         return utils.delta_t(date1, date2, self.dc, self.cal)
 
     def _t(self, date):
         """
         Coverts date to year fraction.
         """
         return self._dt(self.base, date)
+    
+    def _is_extrapolated_date(self, date):
+        '''
+        Returns whether given date is outside bounds of interpolation.
+        '''
+        return not utils.date_within_bounds(date, self.earliest_date, self.latest_date)
 
     def cap_factor(self, date1, date2):
         """
         Interpolated cap factor of curve between two dates. See docs for
         ratecurve.equations.cap_factor for more details.
         """
         # Validate dates
         validated_date1 = utils.to_dateroll_date(date1, base=self.base)
         validated_date2 = utils.to_dateroll_date(date2, base=date1)
-        # Get interpolated cap factor
-        cf01 = self.interpolate_cap_factor(validated_date1)
-        cf02 = self.interpolate_cap_factor(validated_date2)
+        # Get cap factor
+        cf01 = self.extrapolate_cap_factor(validated_date1) if self._is_extrapolated_date(validated_date1) else self.interpolate_cap_factor(validated_date1)
+        cf02 = self.extrapolate_cap_factor(validated_date2) if self._is_extrapolated_date(validated_date2) else self.interpolate_cap_factor(validated_date2)
         # Compute forward cap factor
         cf12 = cf02 / cf01
         return cf12
     
-    def convert_cap_factor_to_rate(self, cf, dt):
-        return equations.convert_cap_factor_to_rate(cf, dt, self.method, default=self.base_rate)
+    def convert_cap_factor_to_rate(self, cf, date1, date2):
+        '''
+        Converts cap factor to rate.
+        '''
+        validated_date1 = utils.to_dateroll_date(date1, base=self.base)
+        validated_date2 = utils.to_dateroll_date(date2, base=date1)
+        dt = self._dt(validated_date1, validated_date2)
+        hasExtrapolatedDate = self._is_extrapolated_date(validated_date1) or self._is_extrapolated_date(validated_date2)
+        if hasExtrapolatedDate:
+            return self.extrapolated_rate_from_cf(cf, validated_date1, validated_date2)        
+        else:
+            default_rate = self.interpolate_r0() if self.extrap_method == 'extrapolate' else self.earliest_rate    
+            return equations.convert_cap_factor_to_rate(cf, dt, self.method, default=default_rate)
 
     def disc_factor(self, date1, date2):
         """
         Interpolated discount factor of curve between two dates. See docs for
         ratecurve.equations.disc_factor for more details.
         """
         return 1 / self.cap_factor(date1, date2)
 
-    def get_y_transformers(self, interp_on, method):
-        """
-        Returns 2 functions:
-            1. Convert raw rates into interpolated form
-            2. Convert interpolated form to raw_rates
-        """
-
-        def to_y(t, rate):
-            # From rate to interpolated form
-            r = rate
-            if interp_on == "r":
-                return r
-            elif interp_on in ("rt", "r*t"):
-                return r * t
-            elif interp_on == "ln(df)":
-                df = equations.disc_factor(r, t, method)
-                return equations.ln(df)
-            else:
-                raise ValueError(f"Unknown interp_on {interp_on}")
-
-        def from_y(t, y):
-            # From interpolated form to cap factor
-            if interp_on == "r":
-                return equations.cap_factor(y, t, self.method)
-            elif interp_on in ("rt", "r*t"):
-                # Cannot divide by 0, cap_factor at t = 0 is 1.
-                return equations.cap_factor(y / t, t, self.method) if t > 0 else 1
-            elif interp_on == "ln(df)":
-                df = equations.e**y
-                return 1 / df
-
-        return to_y, from_y
-
     def make_date_a_number(self, date):
         """
         Converts date or list of dates to a number(s) for interpolation. Number is
         days since root date (originally set to 1/1/2000).
         """
         return utils.from_date_to_number(
             date, INTERPOLATION_ROOT_DATE, self.dc, self.cal
@@ -208,26 +259,99 @@
     def make_number_a_date(self, number):
         """
         Convers interpolation number to date.
         """
         return utils.from_number_to_date(
             number, INTERPOLATION_ROOT_DATE, self.dc, self.cal
         )
-
+    
+    def interpolate_r0(self):
+        """
+        Interpolates r0 for returning on convert_cap_factor_to_rate when self.extrap_method = 'extrapolate'.
+        Raw interpolation of rate data. Interpolates by method specified for general interpolation.
+        """
+        dates = self.dates
+        rates = self.rates
+        processed_x = [self.to_x(date) for date in dates]
+        transformed_y = [self.to_y(self._t(dates[i]), rates[i]) for i in range(len(self.rates))]
+        cf_y = [self.from_y(self._t(dates[i]),transformed_y[i]) for i in range(len(transformed_y))]
+        r_y = [equations.convert_cap_factor_to_rate(cf_y[i], self._dt(self.base, dates[i]), self.method) for i in range(len(cf_y))]
+        sorted_points = sorted(list(zip(processed_x,r_y)), key=lambda x:x[0])
+        front_x = [sorted_points[i][0] for i in range(2)]
+        front_y = [sorted_points[i][1] for i in range(2)]
+        rate_interpolation = interpolate.interp1d(
+            front_x, front_y, kind=self.interp_method, bounds_error=False, fill_value='extrapolate'
+        )
+        d0 = self.to_x(self.base)
+        rate = rate_interpolation(d0)
+        return float(rate)
+        
     def fit(self):
         """
         Fits interpolation and sets self.f
         """
         dates = self.dates
         rates = self.rates
         x = [self.to_x(date) for date in dates]
         y = [self.to_y(self._t(dates[i]), rates[i]) for i in range(len(self.rates))]
+        # Inteprolator
         self.interpolator_unadjusted = interpolate.interp1d(
-            x, y, kind=self.interp_method
+            x, y, kind=self.interp_method,
+        )        
+        # Extrapolators
+        sorted_points = sorted(list(zip(x,y)), key=lambda x:x[0])
+        front_extrap_value =  sorted_points[0][1]
+        back_extrap_value = sorted_points[-1][1]
+        if self.extrap_method == 'extrapolate':
+            front_x = [sorted_points[i][0] for i in range(2)]
+            front_y = [sorted_points[i][1] for i in range(2)]
+            self.front_extrapolator_undajusted = interpolate.interp1d(
+            front_x, front_y, kind=self.interp_method, bounds_error=False, fill_value='extrapolate'
         )
+            
+            back_x = [sorted_points[-(i + 1)][0] for i in range(2)]
+            back_y = [sorted_points[-(i+1)][1] for i in range(2)]            
+            self.back_extrapolator_unadjusted = interpolate.interp1d(
+            back_x, back_y, kind=self.interp_method, bounds_error=False, fill_value='extrapolate'
+        ) 
+        elif self.extrap_method == 'flat':
+            self.front_extrapolator_undajusted = lambda date: front_extrap_value
+            self.back_extrapolator_unadjusted = lambda date: back_extrap_value
+        else:
+            raise ValueError("Extrapolation methods must be either 'extrapolate' or 'flat'")
+
+    def extrapolate_cap_factor(self, date):
+        '''
+        Returns cap_factor for dates that are outside of provided data.
+        '''
+        if date <= self.earliest_date:
+            extrapolator =  self.front_extrapolator_undajusted
+        elif date >= self.latest_date:
+            extrapolator = self.back_extrapolator_unadjusted
+        validated_t = self._t(date)
+        x = self.to_x(date)
+        unadjusted_interpolation = extrapolator(x)
+        cf = self.from_y(validated_t, unadjusted_interpolation)
+        return cf       
+
+    def extrapolated_rate_from_cf(self, cf, date1, date2):
+        '''
+        Returns rates given cap factor on dates that are outside of provided data.
+        '''
+        dt = self._dt(date1, date2)
+        if self.extrap_method=='flat':
+            if date2 < self.earliest_date:
+                rate = self.earliest_rate 
+            elif date2 > self.latest_date and (date1 == self.base or date1 > self.latest_date):
+                rate = self.latest_rate
+            else:
+                rate = equations.convert_cap_factor_to_rate(cf, dt, self.method, default=self.earliest_rate)
+        else:
+            rate = equations.convert_cap_factor_to_rate(cf, dt, self.method, default=self.interpolate_r0())
+        return rate
 
     def interpolate_cap_factor(self, date):
         """
         Adjusts raw interpolation to return cap factor for given date.
         """
         validated_t = self._t(date)
         x = self.to_x(date)
@@ -248,16 +372,15 @@
             raise TypeError("Curve instance call takes 1 or 2 positional arguments")
 
     def fwd(self, date1, date2):
         """
         Computes forward rate between date a and date b.
         """
         cf12 = self.cap_factor(date1, date2)
-        dt = self._dt(date1, date2)
-        r12 = self.convert_cap_factor_to_rate(cf12, dt)
+        r12 = self.convert_cap_factor_to_rate(cf12, date1, date2)
         return r12
 
     def spot(self, date):
         """
         Computes spot rate at date a. Can return as either rate or discount factor.
         """
         # Convert to dates
```

### Comparing `ratecurve-0.0.3/ratecurve/utils.py` & `ratecurve-0.0.4/ratecurve/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -96,7 +96,13 @@
     """
     Calculate year fraction between two dates (date2 after date1)
     """
     # Validate and convert to appropriate dates
     validated_date1 = to_dateroll_date(date1)
     validated_date2 = to_dateroll_date(date2, base=validated_date1)
     return (validated_date2 - validated_date1).yf(cal, dc)
+
+def date_within_bounds(date, lower_bound, upper_bound):
+    '''
+    Returns whether given date is within bounds provided.
+    '''
+    return lower_bound <= date and date <= upper_bound
```

### Comparing `ratecurve-0.0.3/ratecurve.egg-info/PKG-INFO` & `ratecurve-0.0.4/ratecurve.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratecurve
-Version: 0.0.3
+Version: 0.0.4
 Summary: simple utility for curve interpolation
 Home-page: https://github.com/disentcorp/ratecurve
 Author: Disent
 Author-email: chris@disent.com
 License: Apache Software License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ratecurve-0.0.3/setup.py` & `ratecurve-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="ratecurve",
-    version="0.0.3",
+    version="0.0.4",
     description="""simple utility for curve interpolation""",
     author="Disent",
     author_email="chris@disent.com",
     license="Apache Software License",
     url="https://github.com/disentcorp/ratecurve",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `ratecurve-0.0.3/tests/test_equations.py` & `ratecurve-0.0.4/tests/test_equations.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         """
         r = 0.05
         dc = "ACT/365"
         cal = "ALL"
         d1 = ddh("t")
         d2 = ddh("t+1y")
         t = utils.delta_t(d1, d2, dc, cal)
-
+        self.assertEqual(equations.cap_factor(r, 0, "EXP"), 1)
         self.assertEqual(equations.cap_factor(r, t, "EXP"), e ** (r * t))
         self.assertEqual(equations.cap_factor(r, t, "LIN"), 1 + r * t)
         self.assertEqual(equations.cap_factor(r, t, "YLD"), (1 + r) ** t)
         with self.assertRaises(Exception):
             equations.cap_factor(r, t, "apple")
 
     def test_disc_factor(self):
```

### Comparing `ratecurve-0.0.3/tests/test_suite.py` & `ratecurve-0.0.4/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `ratecurve-0.0.3/tests/test_utils.py` & `ratecurve-0.0.4/tests/test_utils.py`

 * *Files identical despite different names*

