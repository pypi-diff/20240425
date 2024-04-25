# Comparing `tmp/scicom-0.2.5.tar.gz` & `tmp/scicom-0.3.0.tar.gz`

## Comparing `scicom-0.2.5.tar` & `scicom-0.3.0.tar`

### file list

```diff
@@ -1,59 +1,84 @@
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 scicom-0.2.5/.gitlab-ci.yml
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 scicom-0.2.5/.readthedocs.yaml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 scicom-0.2.5/MANIFEST.in
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 scicom-0.2.5/tox.ini
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/Makefile
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/authors.rst
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/conf.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/historicalletters.rst
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/index.rst
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/knowledgespread.rst
--rw-r--r--   0        0        0   272329 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/letterModel.png
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/license.rst
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/make.bat
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/randomletters.rst
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/randomlettersDoc.rst
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/readme.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/requirements.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/usingmesa.rst
--rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/_static/bmbf.png
--rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/_static/logo.png
--rw-r--r--   0        0        0    37002 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/_static/mpiwg.png
--rw-r--r--   0        0        0    50988 2020-02-02 00:00:00.000000 scicom-0.2.5/examples/RunModel.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/run.py
--rw-r--r--   0        0        0   389859 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/data/NUTS_RG_60M_2021_3857_LEVL_2.geojson
--rw-r--r--   0        0        0   327135 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/data/nuts_rg_60M_2013_lvl_2.geojson
--rw-r--r--   0        0        0     9175 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/data/pone.0162678.s003.csv
--rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/data/relPop_plosOne.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/historicalletters/__init__.py
--rw-r--r--   0        0        0    11281 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/historicalletters/agents.py
--rw-r--r--   0        0        0     9627 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/historicalletters/model.py
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/historicalletters/server.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/historicalletters/space.py
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/historicalletters/utils.py
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/knowledgespread/SimpleContinuousModule.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/knowledgespread/__init__.py
--rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/knowledgespread/agents.py
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/knowledgespread/app.py
--rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/knowledgespread/model.py
--rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/knowledgespread/server.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/knowledgespread/simple_continuous_canvas.js
--rw-r--r--   0        0        0     8659 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/knowledgespread/utils.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/randomletters/SimpleContinuousModule.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/randomletters/__init__.py
--rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/randomletters/agents.py
--rw-r--r--   0        0        0   182427 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/randomletters/map.png
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/randomletters/model.py
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/randomletters/server.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/randomletters/simple_continuous_canvas.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/utilities/__init__.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/utilities/statistics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.2.5/tests/__init__.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 scicom-0.2.5/tests/test_historicalletters.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 scicom-0.2.5/.gitignore
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 scicom-0.2.5/AUTHORS.rst
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 scicom-0.2.5/LICENSE.md
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 scicom-0.2.5/README.md
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 scicom-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 scicom-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 scicom-0.3.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 scicom-0.3.0/.readthedocs.yaml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 scicom-0.3.0/MANIFEST.in
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 scicom-0.3.0/tox.ini
+-rw-r--r--   0        0        0   822615 2020-02-02 00:00:00.000000 scicom-0.3.0/docs/HistoricalLetters.png
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scicom-0.3.0/docs/Makefile
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 scicom-0.3.0/docs/authors.rst
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 scicom-0.3.0/docs/conf.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 scicom-0.3.0/docs/index.rst
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 scicom-0.3.0/docs/license.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 scicom-0.3.0/docs/make.bat
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 scicom-0.3.0/docs/readme.rst
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 scicom-0.3.0/docs/requirements.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scicom-0.3.0/docs/usingmesa.rst
+-rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 scicom-0.3.0/docs/_static/bmbf.png
+-rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 scicom-0.3.0/docs/_static/logo.png
+-rw-r--r--   0        0        0    37002 2020-02-02 00:00:00.000000 scicom-0.3.0/docs/_static/mpiwg.png
+-rw-r--r--   0        0        0   189800 2020-02-02 00:00:00.000000 scicom-0.3.0/examples/RunModel.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.3.0/src/scicom/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 scicom-0.3.0/src/scicom/run.py
+-rw-r--r--   0        0        0   389859 2020-02-02 00:00:00.000000 scicom-0.3.0/src/scicom/data/NUTS_RG_60M_2021_3857_LEVL_2.geojson
+-rw-r--r--   0        0        0   327135 2020-02-02 00:00:00.000000 scicom-0.3.0/src/scicom/data/nuts_rg_60M_2013_lvl_2.geojson
+-rw-r--r--   0        0        0     9175 2020-02-02 00:00:00.000000 scicom-0.3.0/src/scicom/data/pone.0162678.s003.csv
+-rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 scicom-0.3.0/src/scicom/data/relPop_plosOne.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.3.0/src/scicom/historicalletters/__init__.py
+-rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 scicom-0.3.0/src/scicom/historicalletters/agents.py
+-rw-r--r--   0        0        0    10814 2020-02-02 00:00:00.000000 scicom-0.3.0/src/scicom/historicalletters/model.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 scicom-0.3.0/src/scicom/historicalletters/server.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 scicom-0.3.0/src/scicom/historicalletters/space.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 scicom-0.3.0/src/scicom/historicalletters/utils.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 scicom-0.3.0/src/scicom/knowledgespread/SimpleContinuousModule.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.3.0/src/scicom/knowledgespread/__init__.py
+-rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 scicom-0.3.0/src/scicom/knowledgespread/agents.py
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 scicom-0.3.0/src/scicom/knowledgespread/app.py
+-rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 scicom-0.3.0/src/scicom/knowledgespread/model.py
+-rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 scicom-0.3.0/src/scicom/knowledgespread/server.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 scicom-0.3.0/src/scicom/knowledgespread/simple_continuous_canvas.js
+-rw-r--r--   0        0        0     8659 2020-02-02 00:00:00.000000 scicom-0.3.0/src/scicom/knowledgespread/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.3.0/src/scicom/utilities/__init__.py
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 scicom-0.3.0/src/scicom/utilities/statistics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/.gitignore
+-rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/coverage_html.js
+-rw-r--r--   0        0        0    15089 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/d_124ad581c8e87a79_SimpleContinuousModule_py.html
+-rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/d_124ad581c8e87a79___init___py.html
+-rw-r--r--   0        0        0    52239 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/d_124ad581c8e87a79_agents_py.html
+-rw-r--r--   0        0        0    20654 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/d_124ad581c8e87a79_app_py.html
+-rw-r--r--   0        0        0    53579 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/d_124ad581c8e87a79_model_py.html
+-rw-r--r--   0        0        0    60854 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/d_124ad581c8e87a79_server_py.html
+-rw-r--r--   0        0        0    80793 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/d_124ad581c8e87a79_utils_py.html
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/d_22d2582a602e487e___init___py.html
+-rw-r--r--   0        0        0    50076 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/d_22d2582a602e487e_prune_py.html
+-rw-r--r--   0        0        0    11557 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/d_22d2582a602e487e_statistics_py.html
+-rw-r--r--   0        0        0    15405 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/d_8a73bc3a8cf0a89a_SimpleContinuousModule_py.html
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/d_8a73bc3a8cf0a89a___init___py.html
+-rw-r--r--   0        0        0    43471 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/d_8a73bc3a8cf0a89a_agents_py.html
+-rw-r--r--   0        0        0    27934 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/d_8a73bc3a8cf0a89a_model_py.html
+-rw-r--r--   0        0        0    34647 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/d_8a73bc3a8cf0a89a_server_py.html
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/d_a9eaaac38d807e21___init___py.html
+-rw-r--r--   0        0        0    80338 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/d_a9eaaac38d807e21_agents_py.html
+-rw-r--r--   0        0        0    78295 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/d_a9eaaac38d807e21_model_py.html
+-rw-r--r--   0        0        0    26934 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/d_a9eaaac38d807e21_server_py.html
+-rw-r--r--   0        0        0    19152 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/d_a9eaaac38d807e21_space_py.html
+-rw-r--r--   0        0        0    30557 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/d_a9eaaac38d807e21_utils_py.html
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/d_e85bc3a05b58e6d3___init___py.html
+-rw-r--r--   0        0        0    11246 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/d_e85bc3a05b58e6d3_run_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/favicon_32.png
+-rw-r--r--   0        0        0    11767 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/keybd_open.png
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/status.json
+-rw-r--r--   0        0        0    12394 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/reports/html/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/scicom/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/scicom/historicalletters/__init__.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/scicom/historicalletters/test_model.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/scicom/historicalletters/test_server.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/scicom/historicalletters/test_space.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 scicom-0.3.0/tests/scicom/historicalletters/test_utils.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 scicom-0.3.0/.gitignore
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 scicom-0.3.0/AUTHORS.rst
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 scicom-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 scicom-0.3.0/README.md
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 scicom-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 scicom-0.3.0/PKG-INFO
```

### Comparing `scicom-0.2.5/.gitlab-ci.yml` & `scicom-0.3.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `scicom-0.2.5/docs/Makefile` & `scicom-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scicom-0.2.5/docs/conf.py` & `scicom-0.3.0/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,44 +14,46 @@
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'Scientific Communication Models'
-copyright = '2023, Bernardo S. Buarque, Malte Vogl (ModelSEN)'
+copyright = '2022-2024, Bernardo S. Buarque, Malte Vogl (ModelSEN)'
 author = 'Bernardo S. Buarque, Malte Vogl'
 
 # The full version, including alpha/beta/rc tags
-release = '0.1.0'
+release = '0.2.5'
 
 master_doc = 'index'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc',
+    #'sphinx.ext.autodoc',
     'sphinx.ext.intersphinx',
-    'm2r2'
+    'm2r2',
+    'autoapi.extension',
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 source_suffix = [".rst", ".md"]
-
+autoapi_dirs = ['../src']
+autodoc_typehints = 'description'
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = 'sphinx_rtd_theme'
```

### Comparing `scicom-0.2.5/docs/index.rst` & `scicom-0.3.0/docs/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -4,31 +4,29 @@
    contain the root `toctree` directive.
 
 SciCom documentation
 ====================
 
 Simulating various aspects of scientific communication via Agent-based models.
 
-The development is part of the research project `ModelSEN <https://modelsen.mpiwg-berlin.mpg.de>`_
+The development was part of the research project `ModelSEN <https://modelsen.mpiwg-berlin.mpg.de>`_
 Socio-epistemic networks: Modelling Historical Knowledge Processes,
 part of Department I of the Max Planck Institute for the History of Science and
 funded by the Federal Ministry of Education and Research, Germany (Grant No. 01 UG2131).
 
+The work is continued at the department for Structural Changes of the Technosphere, Max Planck Institute of Geoanthropology, Jena.
+
 .. image:: _static/bmbf.png
 
 .. toctree::
    :maxdepth: 3
    :caption: Contents:
 
    readme
    usingmesa
-   knowledgespread
-   historicalletters
-   randomlettersDoc
-   randomletters
    authors
    license
 
 
 Indices and tables
 ==================
```

### Comparing `scicom-0.2.5/docs/make.bat` & `scicom-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scicom-0.2.5/docs/usingmesa.rst` & `scicom-0.3.0/docs/usingmesa.rst`

 * *Files identical despite different names*

### Comparing `scicom-0.2.5/docs/_static/bmbf.png` & `scicom-0.3.0/docs/_static/bmbf.png`

 * *Files identical despite different names*

### Comparing `scicom-0.2.5/docs/_static/logo.png` & `scicom-0.3.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `scicom-0.2.5/docs/_static/mpiwg.png` & `scicom-0.3.0/docs/_static/mpiwg.png`

 * *Files identical despite different names*

### Comparing `scicom-0.2.5/src/scicom/run.py` & `scicom-0.3.0/src/scicom/run.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,24 @@
+"""Run simulations."""
 import argparse
 
 parser = argparse.ArgumentParser(
-    prog='Run SciCom Simulations',
-    description='This script starts the server interfaces for the different ABM.',
-    epilog='During the running of this script, the interfaces should be reachable at http://127.0.0.1:8521'
+    prog="Run SciCom Simulations",
+    description="This script starts the server interfaces for the different ABM.",
+    epilog="During the running of this script, the interfaces should be reachable at http://127.0.0.1:8521",
 )
 
 parser.add_argument(
-    'simulation',
+    "simulation",
     choices=[
-        "randomletters", "historicalletters", "knowledgespread"
-    ]
+        "historicalletters", "knowledgespread",
+    ],
 )
 
-
 args = parser.parse_args()
 
-if args.simulation == "randomletters":
-    from randomletters.server import server
-    server.launch()
-elif args.simulation == "historicalletters":
-    from historicalletters.server import server
+if args.simulation == "historicalletters":
+    from scicom.historicalletters.server import server
     server.launch()
 elif args.simulation == "knowledgespread":
-    from knowledgespread.server import server
+    from scicom.knowledgespread.server import server
     server.launch()
```

### Comparing `scicom-0.2.5/src/scicom/data/NUTS_RG_60M_2021_3857_LEVL_2.geojson` & `scicom-0.3.0/src/scicom/data/NUTS_RG_60M_2021_3857_LEVL_2.geojson`

 * *Files identical despite different names*

### Comparing `scicom-0.2.5/src/scicom/data/nuts_rg_60M_2013_lvl_2.geojson` & `scicom-0.3.0/src/scicom/data/nuts_rg_60M_2013_lvl_2.geojson`

 * *Files identical despite different names*

### Comparing `scicom-0.2.5/src/scicom/data/pone.0162678.s003.csv` & `scicom-0.3.0/src/scicom/data/pone.0162678.s003.csv`

 * *Files identical despite different names*

### Comparing `scicom-0.2.5/src/scicom/data/relPop_plosOne.csv` & `scicom-0.3.0/src/scicom/data/relPop_plosOne.csv`

 * *Files identical despite different names*

### Comparing `scicom-0.2.5/src/scicom/historicalletters/agents.py` & `scicom-0.3.0/src/scicom/historicalletters/agents.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,59 @@
+"""The agent classes for HistoricalLetters."""
 import random
-import numpy as np
-import networkx as nx
-#from shapely.geometry import LineString
-#from sympy import Point3D, Line3D
-#from sympy.abc import t
 
 import mesa
 import mesa_geo as mg
+import numpy as np
+import shapely
 
-from scicom.historicalletters.utils import getRegion, getPositionOnLine
+from scicom.historicalletters.utils import getNewTopic, getPositionOnLine, getRegion
 
 
 class SenderAgent(mg.GeoAgent):
     """The agent sending letters.
-    
+
     On initialization an agent is places in a geographical coordinate.
     Each agent can send letters to other agents within a distance
     determined by the letterRange. Agents can also move to new positions
-    within the moveRange. 
+    within the moveRange.
 
     Agents keep track of their changing "interest" by having a vector
-    of all held positions in topic space. 
+    of all held positions in topic space.
     """
+
     def __init__(
-        self, unique_id, model, geometry, crs, updateTopic, similarityThreshold, moveRange, letterRange
-    ):
+        self,
+        unique_id:str,
+        model:mesa.Model,
+        geometry: shapely.geometry.point.Point,
+        crs:str,
+        similarityThreshold:float,
+        moveRange:float,
+        letterRange:float,
+    ) -> None:
+        """Initialize an agent.
+
+        With a model, a geometry, crs,
+        and values for updateTopic, similarityThreshold, moveRange,
+        and letterRange.
+        """
         super().__init__(unique_id, model, geometry, crs)
-        self.region_id = ''
+        self.region_id = ""
         self.activationWeight = 1
-        # Not implemented:
-        # The updating is a random walk along a line between receiver and sender.
-        # The strength of adaption is therefore random.
-        # self.updateTopic = updateTopic
         self.similarityThreshold = similarityThreshold
         self.moveRange = moveRange
         self.letterRange = letterRange
+        self.topicVec = ""
         self.topicLedger = []
         self.numLettersReceived = 0
         self.numLettersSend = 0
 
-    def move(self, neighbors):
-        """The agent can randomly move to neighboring positions."""
+    def move(self, neighbors:list) -> None:
+        """Agent can randomly move to neighboring positions."""
         if neighbors:
             # Random decision to move or not, weights are 10% moving, 90% staying.
             move = random.choices([0, 1], weights=[0.9, 0.1], k=1)
             if move[0] == 1:
                 self.model.movements += 1
                 weights = []
                 possible_steps = []
@@ -59,199 +68,188 @@
                 if possible_steps:
                     if sum(weights) > 0:
                         lineEndPoint = random.choices(possible_steps, weights, k=1)
                     else:
                         lineEndPoint = random.choices(possible_steps, k=1)
                     next_position = getPositionOnLine(self.geometry, lineEndPoint[0])
                     # Capture cases where next position has no overlap with region shapefiles.
-                    # TODO: Is there a more clever way to find nearby valid regions?
+                    # TODO(malte): Is there a more clever way to find nearby valid regions?
                     try:
                         regionID = getRegion(next_position, self.model)
                         self.model.space.move_sender(self, next_position, regionID)
                     except IndexError:
-                        if self.model.debug:
-                            print(f"No overlap for {next_position}, aborting movement.")
-                        pass
-
-
-    @property
-    def has_topic(self):
-        """Current topic of the agent."""
-        return self.topicVec
+                        text = f"No overlap for {next_position}, aborting movement."
+                        print(text)
 
-    def has_letter_contacts(self, neighbors=False):
+    def has_letter_contacts(self, *, neighbors: list = False) -> list:
         """List of already established and potential contacts.
 
         Implements the ego-reinforcing by allowing mutliple entries
         of the same agent. In neighbourhoods agents are added proportional
         to the number of letters they received, thus increasing the reinforcement.
         The range of the visible neighborhood is defined by the letterRange parameter
         during model initialization.
 
-        For neigbors in the social network (which can be long-tie), the same process 
+        For neigbors in the social network (which can be long-tie), the same process
         applies. Here, at the begining of each step a list of currently valid scalings
-        is created, see step function in model.py. This prevents updating of 
-        scales during the random activations of agents in one step. 
+        is created, see step function in model.py. This prevents updating of
+        scales during the random activations of agents in one step.
         """
         contacts = []
-        # Social contacts 
-        socialNetwork = [x for x in self.model.G.neighbors(self.unique_id)]
+        # Social contacts
+        socialNetwork = list(self.model.socialNetwork.neighbors(self.unique_id))
         scaleSocial = {}
         for x, y in self.model.scaleSendInput.items():
             if y != 0:
                 scaleSocial.update({x: y})
             else:
                 scaleSocial.update({x: 1})
-        reinforceSocial = [x for y in [[x]*scaleSocial[x] for x in socialNetwork] for x in y]
+        reinforceSocial = [x for y in [[x] * scaleSocial[x] for x in socialNetwork] for x in y]
         contacts.extend(reinforceSocial)
         # Geographical neighbors
         if neighbors:
             neighborRec = []
             for n in neighbors:
                 if n != self:
                     if n.numLettersReceived > 0:
                         nMult = [n] * n.numLettersReceived
                         neighborRec.extend(nMult)
                     else:
                         neighborRec.append(n)
             contacts.extend(neighborRec)
         return contacts
 
-    def chooses_topic(self, receiver):
+    def chooses_topic(self, receiver: mg.GeoAgent) -> tuple:
         """Choose the topic to write about in the letter.
 
         Agents can choose to write a topic from their own ledger or
         in relation to the topics of the receiver. The choice is random.
         """
         topicChoices = self.topicLedger.copy()
         topicChoices.extend(receiver.topicLedger.copy())
-        if topicChoices:
-            initTopic = random.choice(topicChoices)
-        else:
-            initTopic = self.topicVec
-        return initTopic
-
-    def sendLetter(self, neighbors):
-        """Sending a letter based on an urn model."""
-        contacts = self.has_letter_contacts(neighbors)
+        return  random.choice(topicChoices) if topicChoices else self.topicVec
+
+    def sendLetter(self, neighbors:list) -> None:
+        """Send a letter based on an urn model."""
+        contacts = self.has_letter_contacts(neighbors=neighbors)
         if contacts:
             # Randomly choose from the list of possible receivers
             receiver = random.choice(contacts)
             if isinstance(receiver, SenderAgent) and receiver != self:
                 initTopic = self.chooses_topic(receiver)
-                # Calculate distance between own chosen topic 
+                # Calculate distance between own chosen topic
                 # and current topic of receiver.
                 distance = np.linalg.norm(np.array(receiver.topicVec) - np.array(initTopic))
                 # If the calculated distance falls below a similarityThreshold,
                 # send the letter.
                 if distance < self.similarityThreshold:
                     receiver.numLettersReceived += 1
                     self.numLettersSend += 1
                     # Update model social network
-                    self.model.G.add_edge(
+                    self.model.socialNetwork.add_edge(
                         self.unique_id,
                         receiver.unique_id,
-                        step=self.model.schedule.time
+                        step=self.model.schedule.time,
                     )
-                    self.model.G.nodes()[self.unique_id]['numLettersSend'] = self.numLettersSend
-                    self.model.G.nodes()[receiver.unique_id]['numLettersReceived'] = receiver.numLettersReceived
+                    self.model.socialNetwork.nodes()[self.unique_id]["numLettersSend"] = self.numLettersSend
+                    self.model.socialNetwork.nodes()[receiver.unique_id]["numLettersReceived"] = receiver.numLettersReceived
                     # Update receivers topic vector as a random movement
                     # in 3D space on the line between receivers current topic
                     # and the senders chosen topic vectors. An amount of 1 would
                     # correspond to a complete addaption of the senders chosen topic
-                    # vector by the receiver. An amount of 0 means the 
+                    # vector by the receiver. An amount of 0 means the
                     # receiver is not influencend by the sender at all.
-                    # If both topics coincide nothing is changing. 
+                    # If both topics coincide nothing is changing.
                     start = receiver.topicVec
                     end = initTopic
-                    if not start == end:
-                        updatedTopicVec = getPositionOnLine(start, end, returnType="coords")
-                    else:
-                        updatedTopicVec = initTopic
-                    # The letter sending process is complet and the chosen topic of the letter is put into a ledger entry.
+                    updatedTopicVec = getNewTopic(start, end) if start != end else initTopic
+                    # The letter sending process is complet and
+                    # the chosen topic of the letter is put into a ledger entry.
                     self.model.letterLedger.append(
                         (
                             self.unique_id, receiver.unique_id, self.region_id, receiver.region_id,
-                            initTopic, self.model.schedule.steps
-                        )
+                            initTopic, self.model.schedule.steps,
+                        ),
                     )
-                    # Take note of the influence the letter had on the receiver. 
+                    # Take note of the influence the letter had on the receiver.
                     # This information is used in the step function to update all
-                    # agent's currently held topic positions.  
+                    # agent's currently held topic positions.
                     self.model.updatedTopicsDict.update(
-                        {receiver.unique_id: updatedTopicVec}
+                        {receiver.unique_id: updatedTopicVec},
                     )
-                    self.model.updatedTopic += 1
 
-    def step(self):
+    def step(self) -> None:
+        """Perform one simulation step."""
         self.topicVec = self.model.updatedTopicsDict[self.unique_id]
         self.topicLedger.append(
-            self.topicVec
+            self.topicVec,
         )
         currentActivation = random.choices(
             population=[0, 1],
             weights=[1 - self.activationWeight, self.activationWeight],
-            k=1  
+            k=1,
         )
         if currentActivation[0] == 1:
             neighborsMove = [
                 x for x in self.model.space.get_neighbors_within_distance(
                     self,
                     distance=self.moveRange * self.model.meandistance,
-                    center=False
+                    center=False,
                 ) if isinstance(x, SenderAgent)
             ]
             neighborsSend = [
                 x for x in self.model.space.get_neighbors_within_distance(
                     self,
                     distance=self.letterRange * self.model.meandistance,
-                    center=False
+                    center=False,
                 ) if isinstance(x, SenderAgent)
             ]
             self.sendLetter(neighborsSend)
             self.move(neighborsMove)
 
 
 class RegionAgent(mg.GeoAgent):
     """The region keeping track of contained agents.
-    
+
     This agent type is introduced for visualization purposes.
-    SenderAgents are linked to regions by calculation of a 
+    SenderAgents are linked to regions by calculation of a
     geographic overlap of the region shape with the SenderAgent
-    position. 
+    position.
     At initialization, the regions are populated with SenderAgents
     giving rise to a dictionary of the contained SenderAgent IDs and
-    their initial topic. 
-    At each movement, the SenderAgent might cross region boundaries. 
-    This reqieres a re-calculation of the potential overlap. 
+    their initial topic.
+    At each movement, the SenderAgent might cross region boundaries.
+    This reqieres a re-calculation of the potential overlap.
     """
 
-    def __init__(self, unique_id, model, geometry, crs):
+    def __init__(
+        self,
+        unique_id:str,
+        model:mesa.Model,
+        geometry: shapely.geometry.polygon.Polygon,
+        crs:str,
+    ) -> None:
+        """Initialize region with id, model, geometry and crs."""
         super().__init__(unique_id, model, geometry, crs)
-        self.senders_in_region = dict()
+        self.senders_in_region = {}
 
-    def has_main_topic(self):
+    def has_main_topic(self) -> tuple:
+        """Return weighted average topics of agents in region."""
         if len(self.senders_in_region) > 0:
-            topics = [y[0] for x,y in self.senders_in_region.items()]
-            total = [y[1] for x,y in self.senders_in_region.items()]
-            if sum(total) > 0:
-                weight = [x / sum(total) for x in total]
-            else:
-                weight = [1/len(topics)] * len(topics)
+            topics = [y[0] for x, y in self.senders_in_region.items()]
+            total = [y[1] for x, y in self.senders_in_region.items()]
+            weight = [x / sum(total) for x in total] if sum(total) > 0 else [1 / len(topics)] * len(topics)
             mixed_colors = np.sum([np.multiply(weight[i], topics[i]) for i in range(len(topics))], axis=0)
-            colors_inverse = np.subtract((1, 1, 1), mixed_colors)
-            return colors_inverse
-        else:
-            return (0.5, 0.5, 0.5)
-    
-    def add_sender(self, sender):
+            return np.subtract((1, 1, 1), mixed_colors)
+        return (0.5, 0.5, 0.5)
+
+    def add_sender(self, sender: SenderAgent) -> None:
+        """Add a sender to the region."""
         receivedLetters = sender.numLettersReceived
-        if receivedLetters > 0:
-            scale = receivedLetters
-        else: 
-            scale = 1
+        scale = receivedLetters if receivedLetters else 1
         self.senders_in_region.update(
-            {sender.unique_id: (sender.topicVec, scale)}
+            {sender.unique_id: (sender.topicVec, scale)},
         )
 
-    def remove_sender(self, sender):
+    def remove_sender(self, sender: SenderAgent) -> None:
+        """Remove a sender from the region."""
         del self.senders_in_region[sender.unique_id]
```

### Comparing `scicom-0.2.5/src/scicom/historicalletters/model.py` & `scicom-0.3.0/src/scicom/historicalletters/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,264 +1,294 @@
-
+"""The model class for HistoricalLetters."""
 import random
 from pathlib import Path
-#from statistics import mean
-from tqdm import tqdm
-from numpy import mean
 
 import mesa
-import networkx as nx
 import mesa_geo as mg
+import networkx as nx
+import pandas as pd
+from numpy import mean
 from shapely import contains
+from tqdm import tqdm
 
-from scicom.utilities.statistics import prune
-from scicom.historicalletters.utils import createData
-
-from scicom.historicalletters.agents import SenderAgent, RegionAgent
+from scicom.historicalletters.agents import RegionAgent, SenderAgent
 from scicom.historicalletters.space import Nuts2Eu
+from scicom.historicalletters.utils import createData
+from scicom.utilities.statistics import prune
 
 
-def getPrunedLedger(model):
+def getPrunedLedger(model: mesa.Model) -> pd.DataFrame:
     """Model reporter for simulation of archiving.
-    
+
     Returns statistics of ledger network of model run
-    and various iterations of statistics of pruned networks. 
+    and various iterations of statistics of pruned networks.
     """
-    # TODO: Add all model params
+    # TODO(malte): Add all model params
     if model.runPruning is True:
-        ledgerColumns = ['sender', 'receiver', 'sender_location', 'receiver_location', 'topic', 'step']
+        ledgerColumns = ["sender", "receiver", "sender_location", "receiver_location", "topic", "step"]
         modelparams = {
             "population": model.population,
             "moveRange": model.moveRange,
             "letterRange": model.letterRange,
             "useActivation": model.useActivation,
             "useSocialNetwork": model.useSocialNetwork,
         }
         result = prune(
             modelparameters=modelparams,
             network=model.letterLedger,
-            columns=ledgerColumns
+            columns=ledgerColumns,
         )
     else:
         result = model.letterLedger
     return result
 
-def getComponents(model):
+
+def getComponents(model: mesa.Model) -> int:
     """Model reporter to get number of components.
-    
-    The MultiDiGraph is converted to undirected, 
+
+    The MultiDiGraph is converted to undirected,
     considering only edges that are reciprocal, ie.
-    edges are established if sender and receiver have 
+    edges are established if sender and receiver have
     exchanged at least a letter in each direction.
     """
-    newG = model.G.to_undirected(reciprocal=True)
-    comp = nx.number_connected_components(newG)
-    return comp
+    newg = model.socialNetwork.to_undirected(reciprocal=True)
+    return nx.number_connected_components(newg)
+
+
+def getScaledLetters(model: mesa.Model) -> float:
+    """Return relative number of send letters."""
+    return len(model.letterLedger)/model.schedule.time
+
+
+def getScaledMovements(model: mesa.Model) -> float:
+    """Return relative number of movements."""
+    return model.movements/model.schedule.time
 
 
 class HistoricalLetters(mesa.Model):
     """A letter sending model with historical informed initital positions.
-    
-    Each agent has an initial topic vector, expressed as a RGB value. The 
+
+    Each agent has an initial topic vector, expressed as a RGB value. The
     initial positions of the agents is based on a weighted random draw
-    based on data from [1]
-    
-    Each step, agents generate two neighbourhoods for sending letters and 
-    potential targets to move towards. The probability to send letters is 
-    a self-reinforcing process. During each sending the internal topic of 
+    based on data from [1].
+
+    Each step, agents generate two neighbourhoods for sending letters and
+    potential targets to move towards. The probability to send letters is
+    a self-reinforcing process. During each sending the internal topic of
     the sender is updated as a random rotation towards the receivers topic.
 
     [1] J. Lobo et al, Population-Area Relationship for Medieval European Cities,
         PLoS ONE 11(10): e0162678.
     """
+
     def __init__(
         self,
         population: int = 100,
         moveRange: float = 0.05,
         letterRange: float = 0.2,
         similarityThreshold: float = 0.2,
-        updateTopic: float = 0.1,
-        useActivation=False,
-        useSocialNetwork=False,
-        longRangeNetworkFactor=0.3,
-        shortRangeNetworkFactor=0.8,
-        runPruning=False,
+        longRangeNetworkFactor: float = 0.3,
+        shortRangeNetworkFactor: float = 0.4,
         regionData: str = Path(Path(__file__).parent.parent.resolve(), "data/NUTS_RG_60M_2021_3857_LEVL_2.geojson"),
         populationDistributionData: str = Path(Path(__file__).parent.parent.resolve(), "data/pone.0162678.s003.csv"),
-        tempfolder: str = "./",
-        debug=False
-    ):
+        *,
+        useActivation: bool = False,
+        useSocialNetwork: bool = False,
+        runPruning: bool = False,
+        debug: bool = False,
+    ) -> None:
+        """Initialize a HistoricalLetters model."""
         super().__init__()
 
-        # Control variables
+        # Parameters for agents
         self.population = population
         self.moveRange = moveRange
         self.letterRange = letterRange
+        # Parameters for model
+        self.runPruning = runPruning
         self.useActivation = useActivation
-        # Initialize social network
         self.useSocialNetwork = useSocialNetwork
-        self.G = nx.MultiDiGraph()
         self.longRangeNetworkFactor = longRangeNetworkFactor
         self.shortRangeNetworkFactor = shortRangeNetworkFactor
-        # Collected output variables
+        # Initialize social network
+        self.socialNetwork = nx.MultiDiGraph()
+        # Output variables
         self.letterLedger = []
-        self.runPruning = runPruning
         self.movements = 0
-        self.updatedTopic = 0
         # Internal variables
         self.schedule = mesa.time.RandomActivation(self)
         self.scaleSendInput = {}
         self.updatedTopicsDict = {}
         self.space = Nuts2Eu()
-        self.personRegionMap = {}
-        self.tempfolder = tempfolder
         self.debug = debug
 
-        initSenderGeoDf = createData(
-            population,
-            populationDistribution=populationDistributionData
-        )
-
-        # Calculate mean of mean distances for each agent. 
-        # This is used as a measure for the range of exchanges.
-        distances = []
-        for idx, row in initSenderGeoDf.iterrows():
-            p1 = row['geometry']
-            distances.append(
-                initSenderGeoDf.geometry.apply(lambda x: p1.distance(x)).mean()
-            )
-        self.meandistance = mean(distances)
-
-        self.factors = dict(
-            updateTopic=updateTopic,
-            similarityThreshold=similarityThreshold,
-            moveRange=moveRange,
-            letterRange=letterRange,
-        )
+        #######
+        # Initialize region agents
+        #######
 
         # Set up the grid with patches for every NUTS region
+        # Create region agents
         ac = mg.AgentCreator(RegionAgent, model=self)
         self.regions = ac.from_file(
             regionData,
-            unique_id="NUTS_ID"
+            unique_id="NUTS_ID",
         )
+        # Add regions to Nuts2Eu geospace
         self.space.add_regions(self.regions)
 
+        #######
+        # Initialize sender agents
+        #######
+
+        # Draw initial geographic positions of agents
+        initSenderGeoDf = createData(
+            population,
+            populationDistribution=populationDistributionData,
+        )
+
+        # Calculate mean of mean distances for each agent.
+        # This is used as a measure for the range of exchanges.
+        meandistances = []
+        for idx in initSenderGeoDf.index.to_numpy():
+            name = initSenderGeoDf.loc[idx, "unique_id"]
+            geom = initSenderGeoDf.loc[idx, "geometry"]
+            otherAgents = initSenderGeoDf.query(f"unique_id != '{name}'").copy()
+            geometries = otherAgents.geometry.to_numpy()
+            distances = [geom.distance(othergeom) for othergeom in geometries]
+            meandistances.append(mean(distances))
+        self.meandistance = mean(meandistances)
+
+        # Populate factors dictionary
+        self.factors = {
+            "similarityThreshold": similarityThreshold,
+            "moveRange": moveRange,
+            "letterRange": letterRange,
+        }
+
         # Set up agent creator for senders
         ac_senders = mg.AgentCreator(
             SenderAgent,
             model=self,
-            agent_kwargs=self.factors
+            agent_kwargs=self.factors,
         )
 
-        # Create agents based on random coordinates generated 
+        # Create agents based on random coordinates generated
         # in the createData step above, see util.py file.
         senders = ac_senders.from_GeoDataFrame(
             initSenderGeoDf,
-            unique_id="unique_id"
+            unique_id="unique_id",
         )
 
         # Create random set of initial topic vectors.
         topics = [
             tuple(
-                [random.random() for x in range(3)]
+                [random.random() for x in range(3)],
             ) for x in range(self.population)
         ]
 
-        # Attach topic and activationWeight to each agent,
-        # connect to social network graph.
+        # Setup senders
         for idx, sender in enumerate(senders):
-            self.G.add_node(
+            # Add to social network
+            self.socialNetwork.add_node(
                 sender.unique_id,
                 numLettersSend=0,
-                numLettersReceived=0    
+                numLettersReceived=0,
             )
+            # Give sender topic
             sender.topicVec = topics[idx]
             # Add current topic to dict
             self.updatedTopicsDict.update(
-                {sender.unique_id: topics[idx]}
+                {sender.unique_id: topics[idx]},
             )
+            # Set random activation weight
             if useActivation is True:
                 sender.activationWeight = random.random()
-
-        for agent in senders:
+            # Add sender to its region
             regionID = [
-                x.unique_id for x in self.regions if contains(x.geometry, agent.geometry)
+                x.unique_id for x in self.regions if contains(x.geometry, sender.geometry)
             ]
             try:
-                self.space.add_sender(agent, regionID[0])
-            except IndexError:
-                raise IndexError(f"Problem finding region for {agent.geometry}.")
-            self.schedule.add(agent)
+                self.space.add_sender(sender, regionID[0])
+            except IndexError as exc:
+                text = f"Problem finding region for {sender.geometry}."
+                raise IndexError(text) from exc
+            # Add sender to schedule
+            self.schedule.add(sender)
 
         # Add graph to network grid for potential visualization.
-        # TODO: Not yet implemented. Maybe use Solara backend for this? 
-        self.grid = mesa.space.NetworkGrid(self.G)
+        # TODO(malte): Not yet implemented. Maybe use Solara backend for this?
+        # self.grid = mesa.space.NetworkGrid(self.socialNetwork)
 
         # Create social network
         if useSocialNetwork is True:
             for agent in self.schedule.agents:
                 if isinstance(agent, SenderAgent):
-                    self._createSocialEdges(agent, self.G)
+                    self._createSocialEdges(agent, self.socialNetwork)
 
-        # TODO: What comparitive values are useful for visualizations?
         self.datacollector = mesa.DataCollector(
             model_reporters={
                 "Ledger": getPrunedLedger,
-                "Letters": lambda x: len(self.letterLedger),
-                "Movements": lambda x: self.movements,
-                "Clusters": getComponents
+                "Letters": getScaledLetters ,
+                "Movements": getScaledMovements,
+                "Clusters": getComponents,
             },
         )
 
-    def _createSocialEdges(self, agent, graph):
+    def _createSocialEdges(self, agent: SenderAgent, graph: nx.MultiDiGraph) -> None:
         """Create social edges with the different wiring factors.
 
         Define a close range by using the moveRange parameter. Among
         these neighbors, create a connection with probability set by
-        the shortRangeNetworkFactor. 
+        the shortRangeNetworkFactor.
 
         For all other agents, that are not in this closeRange group,
         create a connection with the probability set by the longRangeNetworkFactor.
         """
         closerange = [x for x in self.space.get_neighbors_within_distance(
             agent,
             distance=self.moveRange * self.meandistance,
-            center=False
+            center=False,
         ) if isinstance(x, SenderAgent)]
         for neighbor in closerange:
             if neighbor.unique_id != agent.unique_id:
                 connect = random.choices(
                     population=[True, False],
                     weights=[self.shortRangeNetworkFactor, 1 - self.shortRangeNetworkFactor],
-                    k=1
+                    k=1,
                 )
                 if connect[0] is True:
                     graph.add_edge(agent.unique_id, neighbor.unique_id, step=0)
-                    graph.add_edge(neighbor.unique_id, agent.unique_id, step=0)
         longrange = [x for x in self.schedule.agents if x not in closerange and isinstance(x, SenderAgent)]
         for neighbor in longrange:
             if neighbor.unique_id != agent.unique_id:
                 connect = random.choices(
                     population=[True, False],
                     weights=[self.longRangeNetworkFactor, 1 - self.longRangeNetworkFactor],
-                    k=1
+                    k=1,
                 )
                 if connect[0] is True:
                     graph.add_edge(agent.unique_id, neighbor.unique_id, step=0)
-                    graph.add_edge(neighbor.unique_id, agent.unique_id, step=0)
 
-    def step(self):
+    def step(self) -> None:
+        """One simulation step."""
         self.scaleSendInput.update(
-            **{x.unique_id: x.numLettersReceived for x in self.schedule.agents}
+            **{x.unique_id: x.numLettersReceived for x in self.schedule.agents},
         )
         self.schedule.step()
         self.datacollector.collect(self)
 
-    def run(self, n):
+    def step_no_data(self) -> None:
+        """One simulation step without datacollection."""
+        self.scaleSendInput.update(
+            **{x.unique_id: x.numLettersReceived for x in self.schedule.agents},
+        )
+        self.schedule.step()
+
+    def run(self, n:int) -> None:
         """Run the model for n steps."""
         if self.debug is True:
             for _ in tqdm(range(n)):
-                self.step()
+                self.step_no_data()
         else:
             for _ in range(n):
-                self.step()
+                self.step_no_data()
+        self.datacollector.collect(self)
```

### Comparing `scicom-0.2.5/src/scicom/historicalletters/server.py` & `scicom-0.3.0/src/scicom/historicalletters/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,53 @@
-import matplotlib.colors as colors
-
+"""A visualization interface for HistoricalLetters."""
 import mesa
 import mesa_geo as mg
+from matplotlib import colors
 from mesa.visualization.modules import ChartVisualization
 
-from scicom.historicalletters.agents import SenderAgent, RegionAgent
+from scicom.historicalletters.agents import RegionAgent, SenderAgent
 from scicom.historicalletters.model import HistoricalLetters
 
 model_params = {
-    #"population": 100,
     "population": mesa.visualization.Slider(
-         "Number of persons",
-         50, 10, 100, 10,
-         description="Choose how many senders to include in the model.",
-     ),
+        "Number of persons",
+        50, 10, 100, 10,
+        description="Choose how many senders to include in the model.",
+    ),
     "useSocialNetwork": mesa.visualization.Checkbox(
         "Create initial social network of agents",
-        False
+        False,
     ),
     "useActivation": mesa.visualization.Checkbox(
         "Use heterogenous activations",
-        False
+        False,
     ),
     "similarityThreshold": mesa.visualization.Slider(
         "Similarity threshold",
         0.5, 0.0, 1.0, 0.1,
         description="Choose how similar two agents topics have to be, to send a letter.",
     ),
     "moveRange": mesa.visualization.Slider(
         "Range for moving position</br>(% of mean agent distances)",
-        0.1, 0.05, 0.75, 0.05,
+        0.01, 0.00, 0.5, 0.05,
         description="Choose the visibility range for finding potential locations to move to.",
     ),
     "letterRange": mesa.visualization.Slider(
         "Range for letter sending</br>(% of mean agent distances)",
-        0.2, 0.1,1.0, 0.1,
+        0.2, 0.1, 1.0, 0.1,
         description="Choose the visibility range for finding potential recipients.",
     ),
 }
 
 
-def topic_draw(agent):
+def topic_draw(agent:mg.GeoAgent) -> dict:
+    """Define visualization strategies for agents."""
     portrayal = {}
     if isinstance(agent, RegionAgent):
-        try:
-            color = colors.to_hex(agent.has_main_topic())
-        except: 
-            print(agent.has_main_topic())
-            raise
+        color = colors.to_hex(agent.has_main_topic())
         portrayal["color"] = color
     elif isinstance(agent, SenderAgent):
         colortuple = set(agent.topicVec)
         portrayal["radius"] = 5
         portrayal["shape"] = "circle"
         portrayal["color"] = colors.to_hex(colortuple)
         portrayal["description"] = str(agent.unique_id)
@@ -66,17 +62,17 @@
     map_height=500,
 )
 
 chart = ChartVisualization.ChartModule(
     [
         {"Label": "Movements", "Color": "red"},
         {"Label": "Clusters", "Color": "black"},
-        {'Label': "Letters", "Color": "green"}
+        {"Label": "Letters", "Color": "green"},
     ],
-    data_collector_name='datacollector',
+    data_collector_name="datacollector",
 )
 
 
 server = mesa.visualization.ModularServer(
     HistoricalLetters,
     [map_element, chart],
     "Historical Letters",
```

### Comparing `scicom-0.2.5/src/scicom/historicalletters/space.py` & `scicom-0.3.0/src/scicom/historicalletters/space.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,59 @@
-import random
-from typing import Dict, DefaultDict, Set
-from collections import defaultdict
+"""The geographical space for HistoricalLetters."""
 
 import mesa
 import mesa_geo as mg
-from shapely.geometry import Point
 
 from scicom.historicalletters.agents import RegionAgent, SenderAgent
 
 
 class Nuts2Eu(mg.GeoSpace):
     """Define regions containing senders of letters.
-    
+
+    The space model is initialized with all EU NUTS2 regions.
+    The movement of one agent during the model run consitst of
+    the removing the sender from the old region, setting the
+    new sender position and then adding the sender to the new
+    region.
+
     This is modified from a mesa-geo example, here
     https://github.com/projectmesa/mesa-examples/blob/main/gis/geo_schelling_points/geo_schelling_points/space.py
     """
-    _id_region_map: Dict[str, RegionAgent]
 
-    def __init__(self):
+    def __init__(self) -> None:
+        """Initialize space model."""
         super().__init__(warn_crs_conversion=True)
         self._id_region_map = {}
 
-    def add_regions(self, agents):
+    def add_regions(self, agents: RegionAgent) -> None:
+        """Add regions to space."""
         super().add_agents(agents)
-        total_area = 0
         for agent in agents:
             self._id_region_map[agent.unique_id] = agent
 
-    def add_sender_to_region(self, agent, region_id):
+    def add_sender_to_region(self, agent: SenderAgent, region_id: str) -> None:
+        """Add sender to region."""
         agent.region_id = region_id
         self._id_region_map[region_id].add_sender(agent)
 
-    def remove_sender_from_region(self, agent):
+    def remove_sender_from_region(self, agent: SenderAgent) -> None:
+        """Remove sender from region."""
         self._id_region_map[agent.region_id].remove_sender(agent)
         agent.region_id = None
 
     def add_sender(self, agent: SenderAgent, regionID: str) -> None:
+        """Add sender to specific region."""
         super().add_agents([agent])
         self.add_sender_to_region(agent, regionID)
-        
+
     def move_sender(
-        self, agent: SenderAgent, pos: mesa.space.FloatCoordinate, regionID: str
+        self, agent: SenderAgent, pos: mesa.space.FloatCoordinate, regionID: str,
     ) -> None:
+        """Move sender from old to new region."""
         self.__remove_sender(agent)
         agent.geometry = pos
         self.add_sender(agent, regionID)
 
     def __remove_sender(self, agent: SenderAgent) -> None:
+        """Remove sender."""
         super().remove_agent(agent)
         self.remove_sender_from_region(agent)
-
```

### Comparing `scicom-0.2.5/src/scicom/historicalletters/utils.py` & `scicom-0.3.0/src/scicom/historicalletters/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,106 +1,114 @@
+"""Utility functions for HistoricalLetters."""
 import random
-import pandas as pd
+
 import geopandas as gpd
-from shapely import contains, LineString
+import mesa
+import numpy as np
+import pandas as pd
+import shapely
+from shapely import LineString, contains
 
 
-def createData(population: int, populationDistribution: str):
+def createData(population: int, populationDistribution: str) -> gpd.GeoDataFrame:
     """Create random coordinates of historically motivated choices.
-    
+
     The routine samples a population sample based on estimated
-    population density of that coordinate. 
+    population density of that coordinate.
 
-    The original CSV dataset is retrieved from 
+    The original CSV dataset is retrieved from
     https://doi.org/10.1371/journal.pone.0162678.s003
     """
-
     initial_population_choices = pd.read_csv(
         populationDistribution,
-        encoding="latin1", index_col=0
+        encoding="latin1", index_col=0,
     )
 
     # Calculate relative population ratio to estimated settlement area.
     # This will correspont to the probabilities to draw an agent from
     # these coordinates.
     relPop = []
 
-    for idx ,row in initial_population_choices.iterrows():
+    for _, row in initial_population_choices.iterrows():
         relPop.append(
-            row["Area"]/row["Pop"]
+            row["Area"] / row["Pop"],
         )
 
-    initial_population_choices.insert(0, 'relPop', relPop)
+    initial_population_choices.insert(0, "relPop", relPop)
 
     # Four costal cities can not be considered, since the modern NUTS regions
-    # give zero overlap to their coordinates, leading to potential errors when 
+    # give zero overlap to their coordinates, leading to potential errors when
     # agents move.
-    excludeCoastal = ['Great Yarmouth', 'Kingston-upon-Hull', 'Calais', 'Toulon']
+    excludeCoastal = ["Great Yarmouth", "Kingston-upon-Hull", "Calais", "Toulon"]
     initial_population_choices = initial_population_choices.query("~Settlement.isin(@excludeCoastal)")
 
     loc_probabilities = []
     loc_values = []
-    for idx, row in initial_population_choices.iterrows():
+    for _, row in initial_population_choices.iterrows():
         loc_probabilities.append(row["relPop"])
         loc_values.append(
-            (row["longitude"], row["latitude"])
+            (row["longitude"], row["latitude"]),
         )
 
     coordinates = random.choices(
         loc_values,
         loc_probabilities,
-        k=population
+        k=population,
     )
 
     data = pd.DataFrame(
         coordinates,
-        columns=["longitude", "latitude"]
+        columns=["longitude", "latitude"],
     )
 
     data.insert(
         0,
-        'unique_id',
+        "unique_id",
         [
             "P" + str(x) for x in list(range(population))
-        ]
+        ],
     )
 
     # Read the Geodataframe with EPSG:4326 projection.
     geodf = gpd.GeoDataFrame(
         data,
         geometry=gpd.points_from_xy(data.longitude, data.latitude),
-        crs="EPSG:4326"
+        crs="EPSG:4326",
     )
 
-    # Transform to EPSG:3857, since the NUTS shape files are in 
+    # Transform to EPSG:3857, since the NUTS shape files are in
     # that projection.
-    geodf = geodf.to_crs("EPSG:3857")
-
-    return geodf
+    return geodf.to_crs("EPSG:3857")
 
 
-def getRegion(geometry, model):
+def getRegion(geometry: shapely.geometry.point.Point, model:mesa.Model) -> str:
     """Get region ID overlaping with input geometry.
-    
+
     Might e.g. fail if line of connection crosses international
     waters, since there is no NUTS region assigned then.
     """
     regionID = [
-                x.unique_id for x in model.regions if contains(x.geometry, geometry)
-            ]
+        x.unique_id for x in model.regions if contains(x.geometry, geometry)
+    ]
     if regionID:
         return regionID[0]
-    else:
-        raise IndexError(f"Can not find overlaping region to geometry {geometry}")
+    text = f"Can not find overlaping region to geometry {geometry}"
+    raise IndexError(text)
 
 
-def getPositionOnLine(start, target, returnType="point"):
+def getPositionOnLine(start:shapely.Point, target:shapely.Point) -> shapely.Point:
     """Interpolate movement along line between two given points.
-    
+
     The amount of moving from start to target is random.
     """
     segment = LineString([start, target])
-    newPos = segment.interpolate(random.random(), normalized=True)
-    if returnType == "point":
-        return newPos
-    elif returnType == "coords":
-        return [x for x in newPos.coords][0]
+    return segment.interpolate(random.uniform(0.0, 1.0), normalized=True)
+
+def getNewTopic(start: tuple, target:tuple) -> tuple:
+    """Interpolate new topic between two topics.
+
+    The amount of moving from start to target is random.
+    """
+    p1 = np.array(start)
+    p2 = np.array(target)
+    p3 = p1 + random.uniform(0, 1) * (p2 -p1)
+    return tuple(p3)
```

### Comparing `scicom-0.2.5/src/scicom/knowledgespread/SimpleContinuousModule.py` & `scicom-0.3.0/src/scicom/knowledgespread/SimpleContinuousModule.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import mesa
 
 
 class SimpleCanvas(mesa.visualization.VisualizationElement):
+    """Display agents on a map background. No coordinates."""
     local_includes = ["knowledgespread/simple_continuous_canvas.js"]
     portrayal_method = None
     canvas_height = 720
     canvas_width = 1280
 
     def __init__(self, portrayal_method, canvas_height=720, canvas_width=1280):
         """
@@ -16,14 +17,15 @@
         self.canvas_width = canvas_width
         new_element = "new Simple_Continuous_Module({}, {})".format(
             self.canvas_width, self.canvas_height
         )
         self.js_code = "elements.push(" + new_element + ");"
 
     def render(self, model):
+        """Draw agents."""
         space_state = []
         for obj in model.schedule.agents:
             portrayal = self.portrayal_method(obj)
             x, y = obj.pos
             x = (x - model.space.x_min) / (model.space.x_max - model.space.x_min)
             y = (y - model.space.y_min) / (model.space.y_max - model.space.y_min)
             portrayal["x"] = x
```

### Comparing `scicom-0.2.5/src/scicom/knowledgespread/agents.py` & `scicom-0.3.0/src/scicom/knowledgespread/agents.py`

 * *Files identical despite different names*

### Comparing `scicom-0.2.5/src/scicom/knowledgespread/app.py` & `scicom-0.3.0/src/scicom/knowledgespread/app.py`

 * *Files identical despite different names*

### Comparing `scicom-0.2.5/src/scicom/knowledgespread/model.py` & `scicom-0.3.0/src/scicom/knowledgespread/model.py`

 * *Files identical despite different names*

### Comparing `scicom-0.2.5/src/scicom/knowledgespread/server.py` & `scicom-0.3.0/src/scicom/knowledgespread/server.py`

 * *Files identical despite different names*

### Comparing `scicom-0.2.5/src/scicom/knowledgespread/simple_continuous_canvas.js` & `scicom-0.3.0/src/scicom/knowledgespread/simple_continuous_canvas.js`

 * *Files identical despite different names*

### Comparing `scicom-0.2.5/src/scicom/knowledgespread/utils.py` & `scicom-0.3.0/src/scicom/knowledgespread/utils.py`

 * *Files identical despite different names*

### Comparing `scicom-0.2.5/LICENSE.md` & `scicom-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scicom-0.2.5/README.md` & `scicom-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -26,36 +26,39 @@
 
 ## Examples
 
 You can find an example Jupyter Notebook showing the use of the LetterSpace model in the [examples folder](./examples/RunModel.ipynb). 
 
 Alternatively, you can use the mesa server framework to create an local browser interface with changeable parameters, 
 see screenshot below and [documentation on running mesa](./docs/usingmesa.rst).
-<img src="./docs/letterModel.png" alt= “MesaInterface” width="800" height="400">
+<img src="./docs/HistoricalLetters.png" alt= “MesaInterface” width="800" height="400">
 
 
 ## Testing
 
-Tests can be run by installing the _dev_ requirements and running `tox`.
+Tests can be run by installing the _test_ requirements and running `tox`.
 
 ~~~bash
-pip install scicom[dev]
+pip install scicom[test]
 tox
 ~~~
 
 ## Building documentation
 
-The documentation is build using _sphinx_. Install with the _dev_ option and run
+The documentation is build using _sphinx_. Install with the _docs_ option and run
 
 ~~~bash
-pip install scicom[dev]
+pip install scicom[docs]
 tox -e docs
 ~~~
 
 ## Funding information
 
-The development is part of the research project [ModelSEN](https://modelsen.mpiwg-berlin.mpg.de)
+The development was part of the research project [ModelSEN](https://modelsen.mpiwg-berlin.mpg.de)
 
 > Socio-epistemic networks: Modelling Historical Knowledge Processes,
 
-in Department I of the Max Planck Institute for the History of Science
+in Department I of the Max Planck Institute for the History of Science, Berlin,
 and funded by the Federal Ministry of Education and Research, Germany (Grant No. 01 UG2131).
+
+The work is continued in the department for Structural Changes of the Technosphere
+at the Max Planck Institute of Geoanthorpology, Jena.
```

### Comparing `scicom-0.2.5/pyproject.toml` & `scicom-0.3.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "SciCom"
-version = "0.2.5"
+version = "0.3.0"
 authors = [
   { name="Bernardo S. Buarque", email="bernardo.buarque@motu.org.nz"},
   { name="Malte Vogl", email="vogl@gea.mpg.de"}
 ]
 description = "Simulating various aspects of scientific communication via Agent-based models."
 readme = "README.md"
 license = {file = "LICENSE.md"}
@@ -23,27 +23,41 @@
   "mesa >= 2",
   "mesa-geo",
   "shapely >=2",
   "pandas",
   "geopandas",
   "networkx",
   "numpy",
-  "sympy",
-  "semanticlayertools",
+  "igraph",
   "solara",
   "altair",
   "nx_altair"
 ]
 
 [project.urls]
 "Project Homepage" = "https://modelsen.mpiwg-berlin.mpg.de"
 "Homepage" = "https://gitlab.gwdg.de/modelsen/sciencecommunicationmodels"
 "Issues" = "https://gitlab.gwdg.de/modelsen/sciencecommunicationmodels/-/issues"
 
 
 
 [project.optional-dependencies]
-dev = [
+test = [
   "tox",
-  "twine",
+  "flake8",
+  "pytest",
+  "pytest-cov"
+]
+docs = [
+  "sphinx_rtd_theme",
+  "m2r2",
   "sphinx",
-]
+  "sphinx-autoapi"
+]
+dev = ["twine"]
+
+[tool.ruff.lint]
+select = ["ALL"]
+
+[tool.ruff]
+line-length = 120
+ignore = ["S101", "S311", "TD003", "ANN101", "N802", "N803", "N806"]
```

### Comparing `scicom-0.2.5/PKG-INFO` & `scicom-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: SciCom
-Version: 0.2.5
+Version: 0.3.0
 Summary: Simulating various aspects of scientific communication via Agent-based models.
 Project-URL: Project Homepage, https://modelsen.mpiwg-berlin.mpg.de
 Project-URL: Homepage, https://gitlab.gwdg.de/modelsen/sciencecommunicationmodels
 Project-URL: Issues, https://gitlab.gwdg.de/modelsen/sciencecommunicationmodels/-/issues
 Author-email: "Bernardo S. Buarque" <bernardo.buarque@motu.org.nz>, Malte Vogl <vogl@gea.mpg.de>
 License: MIT License
         
@@ -31,28 +31,35 @@
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: altair
 Requires-Dist: geopandas
+Requires-Dist: igraph
 Requires-Dist: mesa-geo
 Requires-Dist: mesa>=2
 Requires-Dist: networkx
 Requires-Dist: numpy
 Requires-Dist: nx-altair
 Requires-Dist: pandas
-Requires-Dist: semanticlayertools
 Requires-Dist: shapely>=2
 Requires-Dist: solara
-Requires-Dist: sympy
 Provides-Extra: dev
-Requires-Dist: sphinx; extra == 'dev'
-Requires-Dist: tox; extra == 'dev'
 Requires-Dist: twine; extra == 'dev'
+Provides-Extra: docs
+Requires-Dist: m2r2; extra == 'docs'
+Requires-Dist: sphinx; extra == 'docs'
+Requires-Dist: sphinx-autoapi; extra == 'docs'
+Requires-Dist: sphinx-rtd-theme; extra == 'docs'
+Provides-Extra: test
+Requires-Dist: flake8; extra == 'test'
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Requires-Dist: tox; extra == 'test'
 Description-Content-Type: text/markdown
 
 ## SciCom
 
 Simulating various aspects of scientific communication via Agent-based models.
 
 In this first version, we introduce an agent-based modelling approach to reconstruct communication in
@@ -79,36 +86,39 @@
 
 ## Examples
 
 You can find an example Jupyter Notebook showing the use of the LetterSpace model in the [examples folder](./examples/RunModel.ipynb). 
 
 Alternatively, you can use the mesa server framework to create an local browser interface with changeable parameters, 
 see screenshot below and [documentation on running mesa](./docs/usingmesa.rst).
-<img src="./docs/letterModel.png" alt= “MesaInterface” width="800" height="400">
+<img src="./docs/HistoricalLetters.png" alt= “MesaInterface” width="800" height="400">
 
 
 ## Testing
 
-Tests can be run by installing the _dev_ requirements and running `tox`.
+Tests can be run by installing the _test_ requirements and running `tox`.
 
 ~~~bash
-pip install scicom[dev]
+pip install scicom[test]
 tox
 ~~~
 
 ## Building documentation
 
-The documentation is build using _sphinx_. Install with the _dev_ option and run
+The documentation is build using _sphinx_. Install with the _docs_ option and run
 
 ~~~bash
-pip install scicom[dev]
+pip install scicom[docs]
 tox -e docs
 ~~~
 
 ## Funding information
 
-The development is part of the research project [ModelSEN](https://modelsen.mpiwg-berlin.mpg.de)
+The development was part of the research project [ModelSEN](https://modelsen.mpiwg-berlin.mpg.de)
 
 > Socio-epistemic networks: Modelling Historical Knowledge Processes,
 
-in Department I of the Max Planck Institute for the History of Science
+in Department I of the Max Planck Institute for the History of Science, Berlin,
 and funded by the Federal Ministry of Education and Research, Germany (Grant No. 01 UG2131).
+
+The work is continued in the department for Structural Changes of the Technosphere
+at the Max Planck Institute of Geoanthorpology, Jena.
```

