# Comparing `tmp/govee-ble-0.9.0.tar.gz` & `tmp/govee-ble-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govee-ble-0.9.0.tar", max compression
+gzip compressed data, was "govee-ble-0.9.1.tar", max compression
```

## Comparing `govee-ble-0.9.0.tar` & `govee-ble-0.9.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11345 2022-07-19 07:07:42.456266 govee-ble-0.9.0/LICENSE
--rw-r--r--   0        0        0     3487 2022-07-19 07:07:42.456266 govee-ble-0.9.0/README.md
--rw-r--r--   0        0        0     2375 2022-07-19 07:07:43.308275 govee-ble-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      383 2022-07-19 07:07:43.256274 govee-ble-0.9.0/src/govee_ble/__init__.py
--rw-r--r--   0        0        0     9701 2022-07-19 07:07:42.456266 govee-ble-0.9.0/src/govee_ble/parser.py
--rw-r--r--   0        0        0        0 2022-07-19 07:07:42.456266 govee-ble-0.9.0/src/govee_ble/py.typed
--rw-r--r--   0        0        0     4503 2022-07-19 07:07:53.447293 govee-ble-0.9.0/setup.py
--rw-r--r--   0        0        0     4871 2022-07-19 07:07:53.447640 govee-ble-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11345 2022-07-19 14:35:37.564102 govee-ble-0.9.1/LICENSE
+-rw-r--r--   0        0        0     3487 2022-07-19 14:35:37.564102 govee-ble-0.9.1/README.md
+-rw-r--r--   0        0        0     2375 2022-07-19 14:35:38.604138 govee-ble-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      383 2022-07-19 14:35:38.564136 govee-ble-0.9.1/src/govee_ble/__init__.py
+-rw-r--r--   0        0        0     8410 2022-07-19 14:35:37.564102 govee-ble-0.9.1/src/govee_ble/parser.py
+-rw-r--r--   0        0        0        0 2022-07-19 14:35:37.564102 govee-ble-0.9.1/src/govee_ble/py.typed
+-rw-r--r--   0        0        0     4503 2022-07-19 14:35:48.704172 govee-ble-0.9.1/setup.py
+-rw-r--r--   0        0        0     4871 2022-07-19 14:35:48.704517 govee-ble-0.9.1/PKG-INFO
```

### Comparing `govee-ble-0.9.0/LICENSE` & `govee-ble-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `govee-ble-0.9.0/README.md` & `govee-ble-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `govee-ble-0.9.0/pyproject.toml` & `govee-ble-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "govee-ble"
-version = "0.9.0"
+version = "0.9.1"
 description = "Manage Govee BLE devices"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/bluetooth-devices/govee-ble"
 documentation = "https://govee-ble.readthedocs.io"
 classifiers = [
@@ -26,15 +26,15 @@
 python = "^3.9"
 
 # Documentation Dependencies
 Sphinx = {version = "^5.0", optional = true}
 sphinx-rtd-theme = {version = "^1.0", optional = true}
 myst-parser = {version = "^0.18", optional = true}
 home-assistant-bluetooth = ">=1.3.0"
-sensor-state-data = ">=1.7.0"
+sensor-state-data = ">=1.9.0"
 bluetooth-sensor-state-data = ">=1.4.1"
 
 [tool.poetry.extras]
 docs = [
     "myst-parser",
     "sphinx",
     "sphinx-rtd-theme",
```

### Comparing `govee-ble-0.9.0/setup.py` & `govee-ble-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['bluetooth-sensor-state-data>=1.4.1',
  'home-assistant-bluetooth>=1.3.0',
- 'sensor-state-data>=1.7.0']
+ 'sensor-state-data>=1.9.0']
 
 extras_require = \
 {'docs': ['Sphinx>=5.0,<6.0',
           'sphinx-rtd-theme>=1.0,<2.0',
           'myst-parser>=0.18,<0.19']}
 
 setup_kwargs = {
     'name': 'govee-ble',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'Manage Govee BLE devices',
     'long_description': '# Govee BLE\n\n<p align="center">\n  <a href="https://github.com/bluetooth-devices/govee-ble/actions?query=workflow%3ACI">\n    <img src="https://img.shields.io/github/workflow/status/bluetooth-devices/govee-ble/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://govee-ble.readthedocs.io">\n    <img src="https://img.shields.io/readthedocs/govee-ble.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">\n  </a>\n  <a href="https://codecov.io/gh/bluetooth-devices/govee-ble">\n    <img src="https://img.shields.io/codecov/c/github/bluetooth-devices/govee-ble.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/govee-ble/">\n    <img src="https://img.shields.io/pypi/v/govee-ble.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/govee-ble.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/govee-ble.svg?style=flat-square" alt="License">\n</p>\n\nManage Govee BLE devices\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install govee-ble`\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Cookiecutter](https://github.com/audreyr/cookiecutter) and the\n[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)\nproject template.\n',
     'author': 'J. Nick Koston',
     'author_email': 'nick@koston.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/bluetooth-devices/govee-ble',
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['govee_ble'] package_data = \ {'': ['*']} install_requires
 = \ ['bluetooth-sensor-state-data>=1.4.1', 'home-assistant-bluetooth>=1.3.0',
-'sensor-state-data>=1.7.0'] extras_require = \ {'docs': ['Sphinx>=5.0,<6.0',
+'sensor-state-data>=1.9.0'] extras_require = \ {'docs': ['Sphinx>=5.0,<6.0',
 'sphinx-rtd-theme>=1.0,<2.0', 'myst-parser>=0.18,<0.19']} setup_kwargs =
-{ 'name': 'govee-ble', 'version': '0.9.0', 'description': 'Manage Govee BLE
+{ 'name': 'govee-ble', 'version': '0.9.1', 'description': 'Manage Govee BLE
 devices', 'long_description': '# Govee BLE\n\n
     \n _\_n_ _[_C_I_ _S_t_a_t_u_s_]_\_n_ \n _\_n_ _[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_\_n_ \n _\_n_ _[_T_e_s_t_ _c_o_v_e_r_a_g_e
                                _p_e_r_c_e_n_t_a_g_e_]_\_n_ \n
 \n
            \n _\_n_ _[_P_o_e_t_r_y_]_\_n_ \n _\_n_ _[_b_l_a_c_k_]_\_n_ \n _\_n_ _[_p_r_e_-_c_o_m_m_i_t_]_\_n_ \n
 \n
       \n _\_n_ _[_P_y_P_I_ _V_e_r_s_i_o_n_]_\_n_ \n [Supported Python versions]\n [License]\n
```

### Comparing `govee-ble-0.9.0/PKG-INFO` & `govee-ble-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: govee-ble
-Version: 0.9.0
+Version: 0.9.1
 Summary: Manage Govee BLE devices
 Home-page: https://github.com/bluetooth-devices/govee-ble
 License: Apache Software License 2.0
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=5.0,<6.0); extra == "docs"
 Requires-Dist: bluetooth-sensor-state-data (>=1.4.1)
 Requires-Dist: home-assistant-bluetooth (>=1.3.0)
 Requires-Dist: myst-parser (>=0.18,<0.19); extra == "docs"
-Requires-Dist: sensor-state-data (>=1.7.0)
+Requires-Dist: sensor-state-data (>=1.9.0)
 Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0); extra == "docs"
 Project-URL: Bug Tracker, https://github.com/bluetooth-devices/govee-ble/issues
 Project-URL: Changelog, https://github.com/bluetooth-devices/govee-ble/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://govee-ble.readthedocs.io
 Project-URL: Repository, https://github.com/bluetooth-devices/govee-ble
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: govee-ble Version: 0.9.0 Summary: Manage Govee BLE
+Metadata-Version: 2.1 Name: govee-ble Version: 0.9.1 Summary: Manage Govee BLE
 devices Home-page: https://github.com/bluetooth-devices/govee-ble License:
 Apache Software License 2.0 Author: J. Nick Koston Author-email:
 nick@koston.org Requires-Python: >=3.9,<4.0 Classifier: Development Status :: 2
 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier: License ::
 Other/Proprietary License Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Topic :: Software Development ::
 Libraries Provides-Extra: docs Requires-Dist: Sphinx (>=5.0,<6.0); extra ==
 "docs" Requires-Dist: bluetooth-sensor-state-data (>=1.4.1) Requires-Dist:
 home-assistant-bluetooth (>=1.3.0) Requires-Dist: myst-parser (>=0.18,<0.19);
-extra == "docs" Requires-Dist: sensor-state-data (>=1.7.0) Requires-Dist:
+extra == "docs" Requires-Dist: sensor-state-data (>=1.9.0) Requires-Dist:
 sphinx-rtd-theme (>=1.0,<2.0); extra == "docs" Project-URL: Bug Tracker, https:
 //github.com/bluetooth-devices/govee-ble/issues Project-URL: Changelog, https:/
 /github.com/bluetooth-devices/govee-ble/blob/main/CHANGELOG.md Project-URL:
 Documentation, https://govee-ble.readthedocs.io Project-URL: Repository, https:
 //github.com/bluetooth-devices/govee-ble Description-Content-Type: text/
 markdown # Govee BLE
           _[_C_I_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _p_e_r_c_e_n_t_a_g_e_]
```

