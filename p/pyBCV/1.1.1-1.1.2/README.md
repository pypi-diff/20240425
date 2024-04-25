# Comparing `tmp/pyBCV-1.1.1.tar.gz` & `tmp/pybcv-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyBCV-1.1.1.tar", last modified: Mon Jan  1 09:07:39 2024, max compression
+gzip compressed data, was "pybcv-1.1.2.tar", last modified: Thu Apr 25 16:40:23 2024, max compression
```

## Comparing `pyBCV-1.1.1.tar` & `pybcv-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-01-01 09:07:39.409867 pyBCV-1.1.1/
--rw-rw-rw-   0        0        0     1094 2023-12-30 18:06:11.000000 pyBCV-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     4990 2024-01-01 09:07:39.405869 pyBCV-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2779 2024-01-01 08:28:54.000000 pyBCV-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-01-01 09:07:39.370621 pyBCV-1.1.1/pyBCV/
--rw-rw-rw-   0        0        0       74 2024-01-01 08:23:09.000000 pyBCV-1.1.1/pyBCV/__init__.py
--rw-rw-rw-   0        0        0      227 2024-01-01 09:05:53.000000 pyBCV-1.1.1/pyBCV/_requests.py
--rw-rw-rw-   0        0        0     2907 2024-01-01 08:42:10.000000 pyBCV-1.1.1/pyBCV/sistema_bancario.py
--rw-rw-rw-   0        0        0     2258 2024-01-01 08:21:16.000000 pyBCV-1.1.1/pyBCV/tasas_de_cambios.py
--rw-rw-rw-   0        0        0      135 2023-12-30 18:06:11.000000 pyBCV-1.1.1/pyBCV/util.py
-drwxrwxrwx   0        0        0        0 2024-01-01 09:07:39.402871 pyBCV-1.1.1/pyBCV.egg-info/
--rw-rw-rw-   0        0        0     4990 2024-01-01 09:07:39.000000 pyBCV-1.1.1/pyBCV.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2024-01-01 09:07:39.000000 pyBCV-1.1.1/pyBCV.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-01 09:07:39.000000 pyBCV-1.1.1/pyBCV.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-01-01 09:07:39.000000 pyBCV-1.1.1/pyBCV.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-01-01 09:07:39.000000 pyBCV-1.1.1/pyBCV.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      910 2024-01-01 09:06:58.000000 pyBCV-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-01 09:07:39.410867 pyBCV-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1389 2024-01-01 09:06:54.000000 pyBCV-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:40:23.129091 pybcv-1.1.2/
+-rw-rw-rw-   0        0        0     1094 2024-04-25 16:33:04.000000 pybcv-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     4990 2024-04-25 16:40:23.125090 pybcv-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2779 2024-04-25 16:33:04.000000 pybcv-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 16:40:22.962994 pybcv-1.1.2/pyBCV/
+-rw-rw-rw-   0        0        0       74 2024-04-25 16:33:04.000000 pybcv-1.1.2/pyBCV/__init__.py
+-rw-rw-rw-   0        0        0      227 2024-04-25 16:33:04.000000 pybcv-1.1.2/pyBCV/_requests.py
+-rw-rw-rw-   0        0        0     2954 2024-04-25 16:35:13.000000 pybcv-1.1.2/pyBCV/sistema_bancario.py
+-rw-rw-rw-   0        0        0     2290 2024-04-25 16:34:07.000000 pybcv-1.1.2/pyBCV/tasas_de_cambios.py
+-rw-rw-rw-   0        0        0      135 2024-04-25 16:33:04.000000 pybcv-1.1.2/pyBCV/util.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:40:23.121089 pybcv-1.1.2/pyBCV.egg-info/
+-rw-rw-rw-   0        0        0     4990 2024-04-25 16:40:22.000000 pybcv-1.1.2/pyBCV.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2024-04-25 16:40:22.000000 pybcv-1.1.2/pyBCV.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 16:40:22.000000 pybcv-1.1.2/pyBCV.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-04-25 16:40:22.000000 pybcv-1.1.2/pyBCV.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-25 16:40:22.000000 pybcv-1.1.2/pyBCV.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      910 2024-04-25 16:39:43.000000 pybcv-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-25 16:40:23.129091 pybcv-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1389 2024-04-25 16:39:46.000000 pybcv-1.1.2/setup.py
```

### Comparing `pyBCV-1.1.1/LICENSE` & `pybcv-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyBCV-1.1.1/PKG-INFO` & `pybcv-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBCV
-Version: 1.1.1
+Version: 1.1.2
 Summary: PyBCV es una librería desarrollada en el lenguaje de programación Python que se utiliza para recopilar los precios de los tipos de cambio y las tasas informativas proporcionados por el Banco Central de Venezuela (BCV).
 Home-page: https://github.com/fcoagz/pyBCV
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
```

### Comparing `pyBCV-1.1.1/README.md` & `pybcv-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyBCV-1.1.1/pyBCV/sistema_bancario.py` & `pybcv-1.1.2/pyBCV/sistema_bancario.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Union
 from bs4 import BeautifulSoup
 from datetime import datetime
 
 from ._requests import _ensure_200_response
 
 class Bank:
     """
@@ -48,15 +49,15 @@
                 data[fecha_str].append(rate)
 
         for fecha_str in data:
             fecha = datetime.strptime(fecha_str, "%d-%m-%Y")
             if self.start_date <= fecha <= self.final_date:
                 self.result.append({fecha_str: data[fecha_str]})
     
-    def get_by_bank(self, bank_code: str = None):
+    def get_by_bank(self, bank_code: str = None) -> Union[list, dict]:
         """
         Devuelve los tipos de cambio para un banco específico.
         """
         self._load()
 
         if not bank_code:
             return self.result
```

### Comparing `pyBCV-1.1.1/pyBCV/tasas_de_cambios.py` & `pybcv-1.1.2/pyBCV/tasas_de_cambios.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Union
 from bs4 import BeautifulSoup
 from babel import dates
 
 from ._requests import _ensure_200_response
 
 def _get_time(soup: BeautifulSoup) -> str:
     date = soup.find("span", "date-display-single").get('content')
@@ -29,15 +30,15 @@
             "CNY": _get_rate_by_id("yuan", section_tipo_de_cambio_oficial),
             "TRY": _get_rate_by_id("lira", section_tipo_de_cambio_oficial),
             "RUB": _get_rate_by_id("rublo", section_tipo_de_cambio_oficial),
             "USD": _get_rate_by_id("dolar", section_tipo_de_cambio_oficial)
         }
         self.rates['Fecha'] = _get_time(section_tipo_de_cambio_oficial)
 
-    def get_rate(self, currency_code: str = None, prettify: bool = False) -> dict[str, str] | str:
+    def get_rate(self, currency_code: str = None, prettify: bool = False) -> Union[dict[str, str], str]:
         """
         :currency_code: Especifica una tasa de cambio en especifico de obtener su valor. (`EUR`, `CNY`, `TRY`, `RUB`, `USD`, `Fecha`)
         :prettify: True si desea que el valor tenga el simbolo de la moneda en bolivares.
         """
         self._load()
 
         if not currency_code:
```

### Comparing `pyBCV-1.1.1/pyBCV.egg-info/PKG-INFO` & `pybcv-1.1.2/pyBCV.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBCV
-Version: 1.1.1
+Version: 1.1.2
 Summary: PyBCV es una librería desarrollada en el lenguaje de programación Python que se utiliza para recopilar los precios de los tipos de cambio y las tasas informativas proporcionados por el Banco Central de Venezuela (BCV).
 Home-page: https://github.com/fcoagz/pyBCV
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
```

### Comparing `pyBCV-1.1.1/pyproject.toml` & `pybcv-1.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyBCV"
-version = "1.1.1"
+version = "1.1.2"
 dependencies = [
   "requests",
   "bs4",
   "beautifulsoup4",
   "babel"
 ]
 requires-python = ">=3.9"
```

### Comparing `pyBCV-1.1.1/setup.py` & `pybcv-1.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.1.1'
+VERSION = '1.1.2'
 PACKAGE_NAME = 'pyBCV' 
 AUTHOR = 'Francisco Griman'
 AUTHOR_EMAIL = 'grihardware@gmail.com'
 URL = 'https://github.com/fcoagz/pyBCV'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'PyBCV es una librería desarrollada en el lenguaje de programación Python que se utiliza para recopilar los precios de los tipos de cambio y las tasas informativas proporcionados por el Banco Central de Venezuela (BCV).'
```

