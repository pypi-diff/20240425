# Comparing `tmp/ms2rescore-3.1.0.dev5.tar.gz` & `tmp/ms2rescore-3.1.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms2rescore-3.1.0.dev5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ms2rescore-3.1.0.dev6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ms2rescore-3.1.0.dev5.tar` & `ms2rescore-3.1.0.dev6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0    11357 2024-04-18 09:22:19.784489 ms2rescore-3.1.0.dev5/LICENSE
--rw-r--r--   0        0        0     6477 2024-04-18 09:22:19.784489 ms2rescore-3.1.0.dev5/README.md
--rw-r--r--   0        0        0      458 2024-04-18 09:22:19.836490 ms2rescore-3.1.0.dev5/ms2rescore/__init__.py
--rw-r--r--   0        0        0     6608 2024-04-18 09:22:19.836490 ms2rescore-3.1.0.dev5/ms2rescore/__main__.py
--rw-r--r--   0        0        0     5957 2024-04-18 09:22:19.836490 ms2rescore-3.1.0.dev5/ms2rescore/config_parser.py
--rw-r--r--   0        0        0     9229 2024-04-18 09:22:19.836490 ms2rescore-3.1.0.dev5/ms2rescore/core.py
--rw-r--r--   0        0        0      633 2024-04-18 09:22:19.836490 ms2rescore-3.1.0.dev5/ms2rescore/exceptions.py
--rw-r--r--   0        0        0      803 2024-04-18 09:22:19.836490 ms2rescore-3.1.0.dev5/ms2rescore/feature_generators/__init__.py
--rw-r--r--   0        0        0      522 2024-04-18 09:22:19.836490 ms2rescore-3.1.0.dev5/ms2rescore/feature_generators/base.py
--rw-r--r--   0        0        0     3436 2024-04-18 09:22:19.836490 ms2rescore-3.1.0.dev5/ms2rescore/feature_generators/basic.py
--rw-r--r--   0        0        0    10496 2024-04-18 09:22:19.836490 ms2rescore-3.1.0.dev5/ms2rescore/feature_generators/deeplc.py
--rw-r--r--   0        0        0     6261 2024-04-18 09:22:19.836490 ms2rescore-3.1.0.dev5/ms2rescore/feature_generators/im2deep.py
--rw-r--r--   0        0        0    10740 2024-04-18 09:22:19.836490 ms2rescore-3.1.0.dev5/ms2rescore/feature_generators/ionmob.py
--rw-r--r--   0        0        0     7069 2024-04-18 09:22:19.836490 ms2rescore-3.1.0.dev5/ms2rescore/feature_generators/maxquant.py
--rw-r--r--   0        0        0    17272 2024-04-18 09:22:19.836490 ms2rescore-3.1.0.dev5/ms2rescore/feature_generators/ms2pip.py
--rw-r--r--   0        0        0        0 2024-04-18 09:22:19.840490 ms2rescore-3.1.0.dev5/ms2rescore/gui/__init__.py
--rw-r--r--   0        0        0      419 2024-04-18 09:22:19.840490 ms2rescore-3.1.0.dev5/ms2rescore/gui/__main__.py
--rw-r--r--   0        0        0    25980 2024-04-18 09:22:19.840490 ms2rescore-3.1.0.dev5/ms2rescore/gui/app.py
--rw-r--r--   0        0        0    11797 2024-04-18 09:22:19.840490 ms2rescore-3.1.0.dev5/ms2rescore/gui/function2ctk.py
--rw-r--r--   0        0        0    14890 2024-04-18 09:22:19.840490 ms2rescore-3.1.0.dev5/ms2rescore/gui/widgets.py
--rw-r--r--   0        0        0        0 2024-04-18 09:22:19.840490 ms2rescore-3.1.0.dev5/ms2rescore/package_data/__init__.py
--rw-r--r--   0        0        0     1154 2024-04-18 09:22:19.840490 ms2rescore-3.1.0.dev5/ms2rescore/package_data/config_default.json
--rw-r--r--   0        0        0      601 2024-04-18 09:22:19.840490 ms2rescore-3.1.0.dev5/ms2rescore/package_data/config_default_tims.json
--rw-r--r--   0        0        0    12615 2024-04-18 09:22:19.840490 ms2rescore-3.1.0.dev5/ms2rescore/package_data/config_schema.json
--rw-r--r--   0        0        0        0 2024-04-18 09:22:19.840490 ms2rescore-3.1.0.dev5/ms2rescore/package_data/img/__init__.py
--rw-r--r--   0        0        0 44669194 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/package_data/img/config_icon.png
--rw-r--r--   0        0        0     4837 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/package_data/img/github-mark-white.png
--rw-r--r--   0        0        0     5557 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/package_data/img/github-mark.png
--rw-r--r--   0        0        0    52066 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/package_data/img/ms2rescore_logo.png
--rw-r--r--   0        0        0    43034 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/package_data/img/program_icon.ico
--rw-r--r--   0        0        0     5068 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/package_data/ms2rescore-gui-theme.json
--rw-r--r--   0        0        0     7974 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/parse_psms.py
--rw-r--r--   0        0        0     1935 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/parse_spectra.py
--rw-r--r--   0        0        0      138 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/report/__init__.py
--rw-r--r--   0        0        0      614 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/report/__main__.py
--rw-r--r--   0        0        0    18673 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/report/charts.py
--rw-r--r--   0        0        0    14790 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/report/generate.py
--rw-r--r--   0        0        0        0 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/report/templates/__init__.py
--rw-r--r--   0        0        0     1677 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/report/templates/about.html
--rw-r--r--   0        0        0     3182 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/report/templates/base.html
--rw-r--r--   0        0        0      107 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/report/templates/config.html
--rw-r--r--   0        0        0      138 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/report/templates/features.html
--rw-r--r--   0        0        0       22 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/report/templates/log.html
--rw-r--r--   0        0        0      559 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/report/templates/metadata.html
--rw-r--r--   0        0        0      341 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/report/templates/overview.html
--rw-r--r--   0        0        0      831 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/report/templates/stats-card.html
--rw-r--r--   0        0        0     1904 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/report/templates/style.html
--rw-r--r--   0        0        0      138 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/report/templates/target-decoy.html
--rw-r--r--   0        0        0     5189 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/report/templates/texts.toml
--rw-r--r--   0        0        0     2804 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/report/utils.py
--rw-r--r--   0        0        0      302 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/rescoring_engines/__init__.py
--rw-r--r--   0        0        0     9727 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/rescoring_engines/mokapot.py
--rw-r--r--   0        0        0     8207 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/rescoring_engines/percolator.py
--rw-r--r--   0        0        0     3717 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/ms2rescore/utils.py
--rw-r--r--   0        0        0     2680 2024-04-18 09:22:19.992493 ms2rescore-3.1.0.dev5/pyproject.toml
--rw-r--r--   0        0        0     9028 1970-01-01 00:00:00.000000 ms2rescore-3.1.0.dev5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-25 11:51:40.315643 ms2rescore-3.1.0.dev6/LICENSE
+-rw-r--r--   0        0        0     6477 2024-04-25 11:51:40.315643 ms2rescore-3.1.0.dev6/README.md
+-rw-r--r--   0        0        0      458 2024-04-25 11:51:40.367643 ms2rescore-3.1.0.dev6/ms2rescore/__init__.py
+-rw-r--r--   0        0        0     6608 2024-04-25 11:51:40.367643 ms2rescore-3.1.0.dev6/ms2rescore/__main__.py
+-rw-r--r--   0        0        0     5957 2024-04-25 11:51:40.367643 ms2rescore-3.1.0.dev6/ms2rescore/config_parser.py
+-rw-r--r--   0        0        0     9229 2024-04-25 11:51:40.367643 ms2rescore-3.1.0.dev6/ms2rescore/core.py
+-rw-r--r--   0        0        0      633 2024-04-25 11:51:40.367643 ms2rescore-3.1.0.dev6/ms2rescore/exceptions.py
+-rw-r--r--   0        0        0      803 2024-04-25 11:51:40.367643 ms2rescore-3.1.0.dev6/ms2rescore/feature_generators/__init__.py
+-rw-r--r--   0        0        0      522 2024-04-25 11:51:40.367643 ms2rescore-3.1.0.dev6/ms2rescore/feature_generators/base.py
+-rw-r--r--   0        0        0     3436 2024-04-25 11:51:40.367643 ms2rescore-3.1.0.dev6/ms2rescore/feature_generators/basic.py
+-rw-r--r--   0        0        0    10496 2024-04-25 11:51:40.367643 ms2rescore-3.1.0.dev6/ms2rescore/feature_generators/deeplc.py
+-rw-r--r--   0        0        0     6261 2024-04-25 11:51:40.367643 ms2rescore-3.1.0.dev6/ms2rescore/feature_generators/im2deep.py
+-rw-r--r--   0        0        0    10740 2024-04-25 11:51:40.367643 ms2rescore-3.1.0.dev6/ms2rescore/feature_generators/ionmob.py
+-rw-r--r--   0        0        0     7069 2024-04-25 11:51:40.367643 ms2rescore-3.1.0.dev6/ms2rescore/feature_generators/maxquant.py
+-rw-r--r--   0        0        0    17272 2024-04-25 11:51:40.367643 ms2rescore-3.1.0.dev6/ms2rescore/feature_generators/ms2pip.py
+-rw-r--r--   0        0        0        0 2024-04-25 11:51:40.367643 ms2rescore-3.1.0.dev6/ms2rescore/gui/__init__.py
+-rw-r--r--   0        0        0      419 2024-04-25 11:51:40.367643 ms2rescore-3.1.0.dev6/ms2rescore/gui/__main__.py
+-rw-r--r--   0        0        0    25980 2024-04-25 11:51:40.367643 ms2rescore-3.1.0.dev6/ms2rescore/gui/app.py
+-rw-r--r--   0        0        0    11797 2024-04-25 11:51:40.367643 ms2rescore-3.1.0.dev6/ms2rescore/gui/function2ctk.py
+-rw-r--r--   0        0        0    14890 2024-04-25 11:51:40.367643 ms2rescore-3.1.0.dev6/ms2rescore/gui/widgets.py
+-rw-r--r--   0        0        0        0 2024-04-25 11:51:40.367643 ms2rescore-3.1.0.dev6/ms2rescore/package_data/__init__.py
+-rw-r--r--   0        0        0     1154 2024-04-25 11:51:40.367643 ms2rescore-3.1.0.dev6/ms2rescore/package_data/config_default.json
+-rw-r--r--   0        0        0      601 2024-04-25 11:51:40.367643 ms2rescore-3.1.0.dev6/ms2rescore/package_data/config_default_tims.json
+-rw-r--r--   0        0        0    12615 2024-04-25 11:51:40.367643 ms2rescore-3.1.0.dev6/ms2rescore/package_data/config_schema.json
+-rw-r--r--   0        0        0        0 2024-04-25 11:51:40.367643 ms2rescore-3.1.0.dev6/ms2rescore/package_data/img/__init__.py
+-rw-r--r--   0        0        0 44669194 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/package_data/img/config_icon.png
+-rw-r--r--   0        0        0     4837 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/package_data/img/github-mark-white.png
+-rw-r--r--   0        0        0     5557 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/package_data/img/github-mark.png
+-rw-r--r--   0        0        0    52066 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/package_data/img/ms2rescore_logo.png
+-rw-r--r--   0        0        0    43034 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/package_data/img/program_icon.ico
+-rw-r--r--   0        0        0     5068 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/package_data/ms2rescore-gui-theme.json
+-rw-r--r--   0        0        0     7974 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/parse_psms.py
+-rw-r--r--   0        0        0     1935 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/parse_spectra.py
+-rw-r--r--   0        0        0      138 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/report/__init__.py
+-rw-r--r--   0        0        0      614 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/report/__main__.py
+-rw-r--r--   0        0        0    18673 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/report/charts.py
+-rw-r--r--   0        0        0    14790 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/report/generate.py
+-rw-r--r--   0        0        0        0 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/report/templates/__init__.py
+-rw-r--r--   0        0        0     1677 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/report/templates/about.html
+-rw-r--r--   0        0        0     3182 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/report/templates/base.html
+-rw-r--r--   0        0        0      107 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/report/templates/config.html
+-rw-r--r--   0        0        0      138 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/report/templates/features.html
+-rw-r--r--   0        0        0       22 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/report/templates/log.html
+-rw-r--r--   0        0        0      559 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/report/templates/metadata.html
+-rw-r--r--   0        0        0      341 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/report/templates/overview.html
+-rw-r--r--   0        0        0      831 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/report/templates/stats-card.html
+-rw-r--r--   0        0        0     1904 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/report/templates/style.html
+-rw-r--r--   0        0        0      138 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/report/templates/target-decoy.html
+-rw-r--r--   0        0        0     5189 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/report/templates/texts.toml
+-rw-r--r--   0        0        0     2804 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/report/utils.py
+-rw-r--r--   0        0        0      302 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/rescoring_engines/__init__.py
+-rw-r--r--   0        0        0     9673 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/rescoring_engines/mokapot.py
+-rw-r--r--   0        0        0     8207 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/rescoring_engines/percolator.py
+-rw-r--r--   0        0        0     3717 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/ms2rescore/utils.py
+-rw-r--r--   0        0        0     2680 2024-04-25 11:51:40.523643 ms2rescore-3.1.0.dev6/pyproject.toml
+-rw-r--r--   0        0        0     9028 1970-01-01 00:00:00.000000 ms2rescore-3.1.0.dev6/PKG-INFO
```

### Comparing `ms2rescore-3.1.0.dev5/LICENSE` & `ms2rescore-3.1.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/README.md` & `ms2rescore-3.1.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/__main__.py` & `ms2rescore-3.1.0.dev6/ms2rescore/__main__.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/config_parser.py` & `ms2rescore-3.1.0.dev6/ms2rescore/config_parser.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/core.py` & `ms2rescore-3.1.0.dev6/ms2rescore/core.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/exceptions.py` & `ms2rescore-3.1.0.dev6/ms2rescore/exceptions.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/feature_generators/__init__.py` & `ms2rescore-3.1.0.dev6/ms2rescore/feature_generators/__init__.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/feature_generators/base.py` & `ms2rescore-3.1.0.dev6/ms2rescore/feature_generators/base.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/feature_generators/basic.py` & `ms2rescore-3.1.0.dev6/ms2rescore/feature_generators/basic.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/feature_generators/deeplc.py` & `ms2rescore-3.1.0.dev6/ms2rescore/feature_generators/deeplc.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/feature_generators/im2deep.py` & `ms2rescore-3.1.0.dev6/ms2rescore/feature_generators/im2deep.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/feature_generators/ionmob.py` & `ms2rescore-3.1.0.dev6/ms2rescore/feature_generators/ionmob.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/feature_generators/maxquant.py` & `ms2rescore-3.1.0.dev6/ms2rescore/feature_generators/maxquant.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/feature_generators/ms2pip.py` & `ms2rescore-3.1.0.dev6/ms2rescore/feature_generators/ms2pip.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/gui/app.py` & `ms2rescore-3.1.0.dev6/ms2rescore/gui/app.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/gui/function2ctk.py` & `ms2rescore-3.1.0.dev6/ms2rescore/gui/function2ctk.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/gui/widgets.py` & `ms2rescore-3.1.0.dev6/ms2rescore/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/package_data/config_default.json` & `ms2rescore-3.1.0.dev6/ms2rescore/package_data/config_default.json`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/package_data/config_default_tims.json` & `ms2rescore-3.1.0.dev6/ms2rescore/package_data/config_default_tims.json`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/package_data/config_schema.json` & `ms2rescore-3.1.0.dev6/ms2rescore/package_data/config_schema.json`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/package_data/img/config_icon.png` & `ms2rescore-3.1.0.dev6/ms2rescore/package_data/img/config_icon.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/package_data/img/github-mark-white.png` & `ms2rescore-3.1.0.dev6/ms2rescore/package_data/img/github-mark-white.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/package_data/img/github-mark.png` & `ms2rescore-3.1.0.dev6/ms2rescore/package_data/img/github-mark.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/package_data/img/ms2rescore_logo.png` & `ms2rescore-3.1.0.dev6/ms2rescore/package_data/img/ms2rescore_logo.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/package_data/img/program_icon.ico` & `ms2rescore-3.1.0.dev6/ms2rescore/package_data/img/program_icon.ico`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/package_data/ms2rescore-gui-theme.json` & `ms2rescore-3.1.0.dev6/ms2rescore/package_data/ms2rescore-gui-theme.json`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/parse_psms.py` & `ms2rescore-3.1.0.dev6/ms2rescore/parse_psms.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/parse_spectra.py` & `ms2rescore-3.1.0.dev6/ms2rescore/parse_spectra.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/report/__main__.py` & `ms2rescore-3.1.0.dev6/ms2rescore/report/__main__.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/report/charts.py` & `ms2rescore-3.1.0.dev6/ms2rescore/report/charts.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/report/generate.py` & `ms2rescore-3.1.0.dev6/ms2rescore/report/generate.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/report/templates/about.html` & `ms2rescore-3.1.0.dev6/ms2rescore/report/templates/about.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/report/templates/base.html` & `ms2rescore-3.1.0.dev6/ms2rescore/report/templates/base.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/report/templates/metadata.html` & `ms2rescore-3.1.0.dev6/ms2rescore/report/templates/metadata.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/report/templates/stats-card.html` & `ms2rescore-3.1.0.dev6/ms2rescore/report/templates/stats-card.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/report/templates/style.html` & `ms2rescore-3.1.0.dev6/ms2rescore/report/templates/style.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/report/templates/texts.toml` & `ms2rescore-3.1.0.dev6/ms2rescore/report/templates/texts.toml`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/report/utils.py` & `ms2rescore-3.1.0.dev6/ms2rescore/report/utils.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/rescoring_engines/mokapot.py` & `ms2rescore-3.1.0.dev6/ms2rescore/rescoring_engines/mokapot.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,29 +107,27 @@
 
     # Add Mokapot results to PSMList
     psm_list["score"] = q[:, 0]
     psm_list["qvalue"] = q[:, 1]
     psm_list["pep"] = q[:, 2]
 
     # Repeat for peptide-level scores
-    peptides_targets = confidence_results.confidence_estimates["peptides"].set_index(
-        ["peptide", "run"]
-    )[keys]
+    peptides_targets = confidence_results.confidence_estimates["peptides"].set_index(["peptide"])[
+        keys
+    ]
     peptides_decoys = confidence_results.decoy_confidence_estimates["peptides"].set_index(
-        ["peptide", "run"]
+        ["peptide"]
     )[keys]
     peptide_info = pd.concat([peptides_targets, peptides_decoys], axis=0).to_dict(orient="index")
 
     # Add peptide-level scores to PSM metadata
-    run_key = "na" if not all(psm.run for psm in psm_list) else None
+    # run_key = "na" if not all(psm.run for psm in psm_list) else None
     no_charge_pattern = re.compile(r"(/\d+$)")
     for psm in psm_list:
-        peptide_scores = peptide_info[
-            (no_charge_pattern.sub("", str(psm.peptidoform), 1), run_key or psm.run)
-        ]
+        peptide_scores = peptide_info[(no_charge_pattern.sub("", str(psm.peptidoform), 1))]
         psm.metadata.update(
             {
                 "peptide_score": peptide_scores["mokapot score"],
                 "peptide_qvalue": peptide_scores["mokapot q-value"],
                 "peptide_pep": peptide_scores["mokapot PEP"],
             }
         )
```

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/rescoring_engines/percolator.py` & `ms2rescore-3.1.0.dev6/ms2rescore/rescoring_engines/percolator.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/ms2rescore/utils.py` & `ms2rescore-3.1.0.dev6/ms2rescore/utils.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/pyproject.toml` & `ms2rescore-3.1.0.dev6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev5/PKG-INFO` & `ms2rescore-3.1.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms2rescore
-Version: 3.1.0.dev5
+Version: 3.1.0.dev6
 Summary: MS²Rescore: Sensitive PSM rescoring with predicted MS² peak intensities and retention times.
 Keywords: MS2Rescore,MS2PIP,DeepLC,Percolator,proteomics,mass spectrometry,peptide identification,rescoring,machine learning
 Author: Ana Sílvia C. Silva, Robbin Bouwmeester, Louise Buur
 Author-email: Ralf Gabriels <ralf@gabriels.dev>, Arthur Declercq <arthur.declercq@ugent.be>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
```

