# Comparing `tmp/caluxPy_fi-0.1.44.tar.gz` & `tmp/caluxpy_fi-0.1.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caluxPy_fi-0.1.44.tar", last modified: Thu Mar 21 21:19:31 2024, max compression
+gzip compressed data, was "caluxpy_fi-0.1.45.tar", last modified: Thu Apr 25 14:36:19 2024, max compression
```

## Comparing `caluxPy_fi-0.1.44.tar` & `caluxpy_fi-0.1.45.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 21:19:31.770882 caluxPy_fi-0.1.44/
--rw-rw-rw-   0        0        0     1106 2024-03-18 20:26:44.000000 caluxPy_fi-0.1.44/LICENSE.txt
--rw-rw-rw-   0        0        0     4738 2024-03-21 21:19:31.761877 caluxPy_fi-0.1.44/PKG-INFO
--rw-rw-rw-   0        0        0     2724 2024-01-12 17:32:24.000000 caluxPy_fi-0.1.44/README.md
--rw-rw-rw-   0        0        0      824 2024-03-21 21:18:07.000000 caluxPy_fi-0.1.44/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-21 21:19:31.771520 caluxPy_fi-0.1.44/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-21 21:19:31.692268 caluxPy_fi-0.1.44/src/
-drwxrwxrwx   0        0        0        0 2024-03-21 21:19:31.753499 caluxPy_fi-0.1.44/src/caluxPy_fi/
--rw-rw-rw-   0        0        0    15447 2024-03-15 20:06:16.000000 caluxPy_fi-0.1.44/src/caluxPy_fi/Convexity.py
--rw-rw-rw-   0        0        0     1189 2024-01-19 17:22:58.000000 caluxPy_fi-0.1.44/src/caluxPy_fi/DataBase.py
--rw-rw-rw-   0        0        0     4225 2024-03-18 22:03:06.000000 caluxPy_fi-0.1.44/src/caluxPy_fi/ExternalImport.py
--rw-rw-rw-   0        0        0    10561 2024-03-19 16:45:38.000000 caluxPy_fi-0.1.44/src/caluxPy_fi/ExternalImport2.py
--rw-rw-rw-   0        0        0    56627 2024-03-21 21:12:46.000000 caluxPy_fi-0.1.44/src/caluxPy_fi/FixedIncome.py
--rw-rw-rw-   0        0        0     5926 2024-03-21 21:15:39.000000 caluxPy_fi-0.1.44/src/caluxPy_fi/Multiple.py
--rw-rw-rw-   0        0        0    13098 2024-03-14 14:13:38.000000 caluxPy_fi-0.1.44/src/caluxPy_fi/Portfolio.py
--rw-rw-rw-   0        0        0    12223 2024-03-21 21:17:02.000000 caluxPy_fi-0.1.44/src/caluxPy_fi/Support.py
--rw-rw-rw-   0        0        0     5887 2024-03-14 13:56:00.000000 caluxPy_fi-0.1.44/src/caluxPy_fi/UserInputs.py
--rw-rw-rw-   0        0        0       28 2024-01-11 15:43:14.000000 caluxPy_fi-0.1.44/src/caluxPy_fi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 21:19:31.761877 caluxPy_fi-0.1.44/src/caluxPy_fi.egg-info/
--rw-rw-rw-   0        0        0     4738 2024-03-21 21:19:31.000000 caluxPy_fi-0.1.44/src/caluxPy_fi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2024-03-21 21:19:31.000000 caluxPy_fi-0.1.44/src/caluxPy_fi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 21:19:31.000000 caluxPy_fi-0.1.44/src/caluxPy_fi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2024-03-21 21:19:31.000000 caluxPy_fi-0.1.44/src/caluxPy_fi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-21 21:19:31.000000 caluxPy_fi-0.1.44/src/caluxPy_fi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 14:36:19.204762 caluxpy_fi-0.1.45/
+-rw-rw-rw-   0        0        0     1106 2024-03-18 20:26:44.000000 caluxpy_fi-0.1.45/LICENSE.txt
+-rw-rw-rw-   0        0        0     4738 2024-04-25 14:36:19.204762 caluxpy_fi-0.1.45/PKG-INFO
+-rw-rw-rw-   0        0        0     2724 2024-01-12 17:32:24.000000 caluxpy_fi-0.1.45/README.md
+-rw-rw-rw-   0        0        0      824 2024-04-25 14:35:28.000000 caluxpy_fi-0.1.45/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-25 14:36:19.204762 caluxpy_fi-0.1.45/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-25 14:36:19.059256 caluxpy_fi-0.1.45/src/
+drwxrwxrwx   0        0        0        0 2024-04-25 14:36:19.186465 caluxpy_fi-0.1.45/src/caluxPy_fi/
+-rw-rw-rw-   0        0        0    15447 2024-03-15 20:06:16.000000 caluxpy_fi-0.1.45/src/caluxPy_fi/Convexity.py
+-rw-rw-rw-   0        0        0     1189 2024-01-19 17:22:58.000000 caluxpy_fi-0.1.45/src/caluxPy_fi/DataBase.py
+-rw-rw-rw-   0        0        0     4225 2024-03-18 22:03:06.000000 caluxpy_fi-0.1.45/src/caluxPy_fi/ExternalImport.py
+-rw-rw-rw-   0        0        0    10561 2024-03-19 16:45:38.000000 caluxpy_fi-0.1.45/src/caluxPy_fi/ExternalImport2.py
+-rw-rw-rw-   0        0        0    56622 2024-04-25 14:35:17.000000 caluxpy_fi-0.1.45/src/caluxPy_fi/FixedIncome.py
+-rw-rw-rw-   0        0        0     5926 2024-03-21 21:15:39.000000 caluxpy_fi-0.1.45/src/caluxPy_fi/Multiple.py
+-rw-rw-rw-   0        0        0    13098 2024-03-14 14:13:38.000000 caluxpy_fi-0.1.45/src/caluxPy_fi/Portfolio.py
+-rw-rw-rw-   0        0        0    12223 2024-03-21 21:17:02.000000 caluxpy_fi-0.1.45/src/caluxPy_fi/Support.py
+-rw-rw-rw-   0        0        0     5887 2024-03-14 13:56:00.000000 caluxpy_fi-0.1.45/src/caluxPy_fi/UserInputs.py
+-rw-rw-rw-   0        0        0       28 2024-01-11 15:43:14.000000 caluxpy_fi-0.1.45/src/caluxPy_fi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:36:19.204762 caluxpy_fi-0.1.45/src/caluxPy_fi.egg-info/
+-rw-rw-rw-   0        0        0     4738 2024-04-25 14:36:19.000000 caluxpy_fi-0.1.45/src/caluxPy_fi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2024-04-25 14:36:19.000000 caluxpy_fi-0.1.45/src/caluxPy_fi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 14:36:19.000000 caluxpy_fi-0.1.45/src/caluxPy_fi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2024-04-25 14:36:19.000000 caluxpy_fi-0.1.45/src/caluxPy_fi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-25 14:36:19.000000 caluxpy_fi-0.1.45/src/caluxPy_fi.egg-info/top_level.txt
```

### Comparing `caluxPy_fi-0.1.44/LICENSE.txt` & `caluxpy_fi-0.1.45/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `caluxPy_fi-0.1.44/PKG-INFO` & `caluxpy_fi-0.1.45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluxPy_fi
-Version: 0.1.44
+Version: 0.1.45
 Summary: Fixed Income Valuation and Analysis
 Author-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 Maintainer-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luis Manuel Tavarez Valenzuela
```

### Comparing `caluxPy_fi-0.1.44/README.md` & `caluxpy_fi-0.1.45/README.md`

 * *Files identical despite different names*

### Comparing `caluxPy_fi-0.1.44/pyproject.toml` & `caluxpy_fi-0.1.45/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.2.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "caluxPy_fi"
-version = "0.1.44"
+version = "0.1.45"
 authors = [
   { name = "Luis Manuel Tavarez Valenzuela", email = "luima2494@gmail.com" }
 ]
 maintainers = [
   { name = "Luis Manuel Tavarez Valenzuela", email = "luima2494@gmail.com" }
 ]
 description = "Fixed Income Valuation and Analysis"
```

### Comparing `caluxPy_fi-0.1.44/src/caluxPy_fi/Convexity.py` & `caluxpy_fi-0.1.45/src/caluxPy_fi/Convexity.py`

 * *Files identical despite different names*

### Comparing `caluxPy_fi-0.1.44/src/caluxPy_fi/DataBase.py` & `caluxpy_fi-0.1.45/src/caluxPy_fi/DataBase.py`

 * *Files identical despite different names*

### Comparing `caluxPy_fi-0.1.44/src/caluxPy_fi/ExternalImport.py` & `caluxpy_fi-0.1.45/src/caluxPy_fi/ExternalImport.py`

 * *Files identical despite different names*

### Comparing `caluxPy_fi-0.1.44/src/caluxPy_fi/ExternalImport2.py` & `caluxpy_fi-0.1.45/src/caluxPy_fi/ExternalImport2.py`

 * *Files identical despite different names*

### Comparing `caluxPy_fi-0.1.44/src/caluxPy_fi/FixedIncome.py` & `caluxpy_fi-0.1.45/src/caluxPy_fi/FixedIncome.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,27 +39,27 @@
 
         self._start_time = time.perf_counter()
 
          #region ---> Tratamiento de las Fechas
 
         self.issuance_date = issuance_date
         try:
-            if type(self.issuance_date) == str: self.issuance_date = datetime.strptime(issuance_date, self._date_format).date()
+            if type(self.issuance_date) == str: self.issuance_date = datetime.strptime(issuance_date, self.date_format).date()
         except ValueError as e:
             self._logger.error(e)
         
         self.maturity_date = maturity_date
         try:
-            if type(self.maturity_date) == str: self.maturity_date = datetime.strptime(maturity_date, self._date_format).date()
+            if type(self.maturity_date) == str: self.maturity_date = datetime.strptime(maturity_date, self.date_format).date()
         except ValueError as e:
             self._logger.error(e)
         
         self.settlement_date = settlement_date
         try:
-            if type(self.settlement_date) == str: self.settlement_date = datetime.strptime(settlement_date, self._date_format).date()
+            if type(self.settlement_date) == str: self.settlement_date = datetime.strptime(settlement_date, self.date_format).date()
         except ValueError as e:
             self._logger.error(e)
 
         #endregion ---> Tratamiento de las Fechas
         
         self.issuer = issuer
         try:
@@ -119,15 +119,15 @@
                         self.forward_date = Support.get_date_years_ago(self.maturity_date, self._years_to_maturity)
                     except Exception as e:
                         self._logger.error(f'Error calculating a forward date => {e}')
                 else:
                     self.forward_date = forward_date
                     if self.forward_date != '': 
                         try:
-                            if type(forward_date) == str: self.forward_date = datetime.strptime(forward_date, self._date_format).date()
+                            if type(forward_date) == str: self.forward_date = datetime.strptime(forward_date, self.date_format).date()
                         except ValueError as e:
                             self._logger.error(e)    
                     else:
                         self._logger.error('Forward date not specified!') 
                         raise Exception('Forward date not specified!')
                         
                 #If the security if of bullet type then any attribute of amortizable is deleted to avoid incongruencies
@@ -138,15 +138,15 @@
                     self.amortizable_percentage = None
                 else:
                     #If not bullet then all the attributes are kept and verified
                     self.amortization_start_date = amortization_start_date
                     self._logger.info(f'Amortization Date -> {self.amortization_start_date} Type => {type(self.amortization_start_date)}')
                     if self.amortization_start_date != '':
                         try:
-                            if type(self.amortization_start_date) == str: self.amortization_start_date = datetime.strptime(self.amortization_start_date, self._date_format).date()
+                            if type(self.amortization_start_date) == str: self.amortization_start_date = datetime.strptime(self.amortization_start_date, self.date_format).date()
                             self._logger.info(f'Amortization Date -> {self.amortization_start_date} Type => {type(self.amortization_start_date)}')
                         except ValueError as e: self._logger.error(e)
                     else: 
                         self._logger.error('Amortization date not specified!') 
                         raise Exception('Amortization date not specified!')
                         
                     if amortization_periods != '':
```

### Comparing `caluxPy_fi-0.1.44/src/caluxPy_fi/Multiple.py` & `caluxpy_fi-0.1.45/src/caluxPy_fi/Multiple.py`

 * *Files identical despite different names*

### Comparing `caluxPy_fi-0.1.44/src/caluxPy_fi/Portfolio.py` & `caluxpy_fi-0.1.45/src/caluxPy_fi/Portfolio.py`

 * *Files identical despite different names*

### Comparing `caluxPy_fi-0.1.44/src/caluxPy_fi/Support.py` & `caluxpy_fi-0.1.45/src/caluxPy_fi/Support.py`

 * *Files identical despite different names*

### Comparing `caluxPy_fi-0.1.44/src/caluxPy_fi/UserInputs.py` & `caluxpy_fi-0.1.45/src/caluxPy_fi/UserInputs.py`

 * *Files identical despite different names*

### Comparing `caluxPy_fi-0.1.44/src/caluxPy_fi.egg-info/PKG-INFO` & `caluxpy_fi-0.1.45/src/caluxPy_fi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluxPy_fi
-Version: 0.1.44
+Version: 0.1.45
 Summary: Fixed Income Valuation and Analysis
 Author-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 Maintainer-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luis Manuel Tavarez Valenzuela
```

### Comparing `caluxPy_fi-0.1.44/src/caluxPy_fi.egg-info/SOURCES.txt` & `caluxpy_fi-0.1.45/src/caluxPy_fi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

