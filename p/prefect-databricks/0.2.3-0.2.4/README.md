# Comparing `tmp/prefect-databricks-0.2.3.tar.gz` & `tmp/prefect_databricks-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect-databricks-0.2.3.tar", last modified: Wed Nov 29 19:54:19 2023, max compression
+gzip compressed data, was "prefect_databricks-0.2.4.tar", last modified: Thu Apr 25 19:20:20 2024, max compression
```

## Comparing `prefect-databricks-0.2.3.tar` & `prefect_databricks-0.2.4.tar`

### file list

```diff
@@ -1,37 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:54:19.880850 prefect-databricks-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2023-11-29 19:53:38.000000 prefect-databricks-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-11-29 19:53:38.000000 prefect-databricks-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11168 2023-11-29 19:54:19.880850 prefect-databricks-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9547 2023-11-29 19:53:38.000000 prefect-databricks-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:54:19.880850 prefect-databricks-0.2.3/prefect_databricks/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-11-29 19:53:38.000000 prefect-databricks-0.2.3/prefect_databricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-11-29 19:54:19.880850 prefect-databricks-0.2.3/prefect_databricks/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2023-11-29 19:53:38.000000 prefect-databricks-0.2.3/prefect_databricks/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    28901 2023-11-29 19:53:38.000000 prefect-databricks-0.2.3/prefect_databricks/flows.py
--rw-r--r--   0 runner    (1001) docker     (127)    81381 2023-11-29 19:53:38.000000 prefect-databricks-0.2.3/prefect_databricks/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:54:19.876850 prefect-databricks-0.2.3/prefect_databricks/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 19:53:38.000000 prefect-databricks-0.2.3/prefect_databricks/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   168971 2023-11-29 19:53:38.000000 prefect-databricks-0.2.3/prefect_databricks/models/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4762 2023-11-29 19:53:38.000000 prefect-databricks-0.2.3/prefect_databricks/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:54:19.876850 prefect-databricks-0.2.3/prefect_databricks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11168 2023-11-29 19:54:19.000000 prefect-databricks-0.2.3/prefect_databricks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      781 2023-11-29 19:54:19.000000 prefect-databricks-0.2.3/prefect_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 19:54:19.000000 prefect-databricks-0.2.3/prefect_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-11-29 19:54:19.000000 prefect-databricks-0.2.3/prefect_databricks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-11-29 19:54:19.000000 prefect-databricks-0.2.3/prefect_databricks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-11-29 19:54:19.000000 prefect-databricks-0.2.3/prefect_databricks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-11-29 19:53:38.000000 prefect-databricks-0.2.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-29 19:53:38.000000 prefect-databricks-0.2.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:54:19.876850 prefect-databricks-0.2.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 19:53:38.000000 prefect-databricks-0.2.3/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2023-11-29 19:53:38.000000 prefect-databricks-0.2.3/scripts/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2023-11-29 19:54:19.880850 prefect-databricks-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2023-11-29 19:53:38.000000 prefect-databricks-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:54:19.876850 prefect-databricks-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-11-29 19:53:38.000000 prefect-databricks-0.2.3/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2023-11-29 19:53:38.000000 prefect-databricks-0.2.3/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    24384 2023-11-29 19:53:38.000000 prefect-databricks-0.2.3/tests/test_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2023-11-29 19:53:38.000000 prefect-databricks-0.2.3/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2023-11-29 19:53:38.000000 prefect-databricks-0.2.3/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2023-11-29 19:53:38.000000 prefect-databricks-0.2.3/tests/test_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)    80049 2023-11-29 19:53:38.000000 prefect-databricks-0.2.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:20.327712 prefect_databricks-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-25 19:20:20.327712 prefect_databricks-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:20.319712 prefect_databricks-0.2.4/prefect_databricks/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/prefect_databricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 19:20:19.000000 prefect_databricks-0.2.4/prefect_databricks/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/prefect_databricks/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18357 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/prefect_databricks/flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81198 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/prefect_databricks/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:20.323712 prefect_databricks-0.2.4/prefect_databricks/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/prefect_databricks/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   168341 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/prefect_databricks/models/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/prefect_databricks/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:20.323712 prefect_databricks-0.2.4/prefect_databricks/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)   178999 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/prefect_databricks/schemas/jobs-2.1-aws.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:20.323712 prefect_databricks-0.2.4/prefect_databricks/schemas/original/
+-rw-r--r--   0 runner    (1001) docker     (127)   178843 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/prefect_databricks/schemas/original/jobs-2.1-aws.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:20.327712 prefect_databricks-0.2.4/prefect_databricks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-25 19:20:20.000000 prefect_databricks-0.2.4/prefect_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-25 19:20:20.000000 prefect_databricks-0.2.4/prefect_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:20:20.000000 prefect_databricks-0.2.4/prefect_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 19:20:20.000000 prefect_databricks-0.2.4/prefect_databricks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-25 19:20:20.000000 prefect_databricks-0.2.4/prefect_databricks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 19:20:20.000000 prefect_databricks-0.2.4/prefect_databricks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:20:20.327712 prefect_databricks-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:20.323712 prefect_databricks-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/tests/mock_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13619 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/tests/test_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/tests/test_rest.py
```

### Comparing `prefect-databricks-0.2.3/PKG-INFO` & `prefect_databricks-0.2.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,698 +1,474 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7072 6566  : 2.1.Name: pref
 00000020: 6563 742d 6461 7461 6272 6963 6b73 0a56  ect-databricks.V
-00000030: 6572 7369 6f6e 3a20 302e 322e 330a 5375  ersion: 0.2.3.Su
+00000030: 6572 7369 6f6e 3a20 302e 322e 340a 5375  ersion: 0.2.4.Su
 00000040: 6d6d 6172 793a 2050 7265 6665 6374 2069  mmary: Prefect i
-00000050: 6e74 6567 7261 7469 6f6e 7320 696e 7465  ntegrations inte
-00000060: 7261 6374 696e 6720 7769 7468 2044 6174  racting with Dat
-00000070: 6162 7269 636b 730a 486f 6d65 2d70 6167  abricks.Home-pag
-00000080: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
-00000090: 622e 636f 6d2f 5072 6566 6563 7448 512f  b.com/PrefectHQ/
-000000a0: 7072 6566 6563 742d 6461 7461 6272 6963  prefect-databric
-000000b0: 6b73 0a41 7574 686f 723a 2050 7265 6665  ks.Author: Prefe
-000000c0: 6374 2054 6563 686e 6f6c 6f67 6965 732c  ct Technologies,
-000000d0: 2049 6e63 2e0a 4175 7468 6f72 2d65 6d61   Inc..Author-ema
-000000e0: 696c 3a20 6865 6c70 4070 7265 6665 6374  il: help@prefect
-000000f0: 2e69 6f0a 4c69 6365 6e73 653a 2041 7061  .io.License: Apa
-00000100: 6368 6520 4c69 6365 6e73 6520 322e 300a  che License 2.0.
-00000110: 4b65 7977 6f72 6473 3a20 7072 6566 6563  Keywords: prefec
-00000120: 740a 436c 6173 7369 6669 6572 3a20 4e61  t.Classifier: Na
-00000130: 7475 7261 6c20 4c61 6e67 7561 6765 203a  tural Language :
-00000140: 3a20 456e 676c 6973 680a 436c 6173 7369  : English.Classi
-00000150: 6669 6572 3a20 496e 7465 6e64 6564 2041  fier: Intended A
-00000160: 7564 6965 6e63 6520 3a3a 2044 6576 656c  udience :: Devel
-00000170: 6f70 6572 730a 436c 6173 7369 6669 6572  opers.Classifier
-00000180: 3a20 496e 7465 6e64 6564 2041 7564 6965  : Intended Audie
-00000190: 6e63 6520 3a3a 2053 7973 7465 6d20 4164  nce :: System Ad
-000001a0: 6d69 6e69 7374 7261 746f 7273 0a43 6c61  ministrators.Cla
-000001b0: 7373 6966 6965 723a 204c 6963 656e 7365  ssifier: License
-000001c0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-000001d0: 203a 3a20 4170 6163 6865 2053 6f66 7477   :: Apache Softw
-000001e0: 6172 6520 4c69 6365 6e73 650a 436c 6173  are License.Clas
-000001f0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000200: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000210: 5079 7468 6f6e 203a 3a20 3320 3a3a 204f  Python :: 3 :: O
-00000220: 6e6c 790a 436c 6173 7369 6669 6572 3a20  nly.Classifier: 
-00000230: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000240: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000250: 3a20 332e 370a 436c 6173 7369 6669 6572  : 3.7.Classifier
-00000260: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000270: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000280: 203a 3a20 332e 380a 436c 6173 7369 6669   :: 3.8.Classifi
-00000290: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
-000002a0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000002b0: 6f6e 203a 3a20 332e 390a 436c 6173 7369  on :: 3.9.Classi
-000002c0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-000002d0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000002e0: 7468 6f6e 203a 3a20 332e 3130 0a43 6c61  thon :: 3.10.Cla
-000002f0: 7373 6966 6965 723a 2054 6f70 6963 203a  ssifier: Topic :
-00000300: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
-00000310: 6f70 6d65 6e74 203a 3a20 4c69 6272 6172  opment :: Librar
-00000320: 6965 730a 5265 7175 6972 6573 2d50 7974  ies.Requires-Pyt
-00000330: 686f 6e3a 203e 3d33 2e37 0a44 6573 6372  hon: >=3.7.Descr
-00000340: 6970 7469 6f6e 2d43 6f6e 7465 6e74 2d54  iption-Content-T
-00000350: 7970 653a 2074 6578 742f 6d61 726b 646f  ype: text/markdo
-00000360: 776e 0a4c 6963 656e 7365 2d46 696c 653a  wn.License-File:
-00000370: 204c 4943 454e 5345 0a52 6571 7569 7265   LICENSE.Require
-00000380: 732d 4469 7374 3a20 7072 6566 6563 743e  s-Dist: prefect>
-00000390: 3d32 2e31 332e 350a 5072 6f76 6964 6573  =2.13.5.Provides
-000003a0: 2d45 7874 7261 3a20 6465 760a 5265 7175  -Extra: dev.Requ
-000003b0: 6972 6573 2d44 6973 743a 2070 7974 6573  ires-Dist: pytes
-000003c0: 743b 2065 7874 7261 203d 3d20 2264 6576  t; extra == "dev
-000003d0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-000003e0: 2062 6c61 636b 3b20 6578 7472 6120 3d3d   black; extra ==
-000003f0: 2022 6465 7622 0a52 6571 7569 7265 732d   "dev".Requires-
-00000400: 4469 7374 3a20 666c 616b 6538 3b20 6578  Dist: flake8; ex
-00000410: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
-00000420: 7569 7265 732d 4469 7374 3a20 6d79 7079  uires-Dist: mypy
-00000430: 3b20 6578 7472 6120 3d3d 2022 6465 7622  ; extra == "dev"
-00000440: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000450: 6d6b 646f 6373 3b20 6578 7472 6120 3d3d  mkdocs; extra ==
-00000460: 2022 6465 7622 0a52 6571 7569 7265 732d   "dev".Requires-
-00000470: 4469 7374 3a20 6d6b 646f 6373 2d6d 6174  Dist: mkdocs-mat
-00000480: 6572 6961 6c3b 2065 7874 7261 203d 3d20  erial; extra == 
-00000490: 2264 6576 220a 5265 7175 6972 6573 2d44  "dev".Requires-D
-000004a0: 6973 743a 206d 6b64 6f63 7374 7269 6e67  ist: mkdocstring
-000004b0: 735b 7079 7468 6f6e 5d3b 2065 7874 7261  s[python]; extra
-000004c0: 203d 3d20 2264 6576 220a 5265 7175 6972   == "dev".Requir
-000004d0: 6573 2d44 6973 743a 2069 736f 7274 3b20  es-Dist: isort; 
-000004e0: 6578 7472 6120 3d3d 2022 6465 7622 0a52  extra == "dev".R
-000004f0: 6571 7569 7265 732d 4469 7374 3a20 7072  equires-Dist: pr
-00000500: 652d 636f 6d6d 6974 3b20 6578 7472 6120  e-commit; extra 
-00000510: 3d3d 2022 6465 7622 0a52 6571 7569 7265  == "dev".Require
-00000520: 732d 4469 7374 3a20 7079 7465 7374 2d61  s-Dist: pytest-a
-00000530: 7379 6e63 696f 3b20 6578 7472 6120 3d3d  syncio; extra ==
-00000540: 2022 6465 7622 0a52 6571 7569 7265 732d   "dev".Requires-
-00000550: 4469 7374 3a20 6d6f 636b 3b20 7079 7468  Dist: mock; pyth
-00000560: 6f6e 5f76 6572 7369 6f6e 203c 2022 332e  on_version < "3.
-00000570: 3822 2061 6e64 2065 7874 7261 203d 3d20  8" and extra == 
-00000580: 2264 6576 220a 5265 7175 6972 6573 2d44  "dev".Requires-D
-00000590: 6973 743a 206d 6b64 6f63 732d 6765 6e2d  ist: mkdocs-gen-
-000005a0: 6669 6c65 733b 2065 7874 7261 203d 3d20  files; extra == 
-000005b0: 2264 6576 220a 5265 7175 6972 6573 2d44  "dev".Requires-D
-000005c0: 6973 743a 2069 6e74 6572 726f 6761 7465  ist: interrogate
-000005d0: 3b20 6578 7472 6120 3d3d 2022 6465 7622  ; extra == "dev"
-000005e0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000005f0: 636f 7665 7261 6765 3b20 6578 7472 6120  coverage; extra 
-00000600: 3d3d 2022 6465 7622 0a52 6571 7569 7265  == "dev".Require
-00000610: 732d 4469 7374 3a20 7265 7370 783b 2065  s-Dist: respx; e
-00000620: 7874 7261 203d 3d20 2264 6576 220a 5265  xtra == "dev".Re
-00000630: 7175 6972 6573 2d44 6973 743a 2070 696c  quires-Dist: pil
-00000640: 6c6f 773b 2065 7874 7261 203d 3d20 2264  low; extra == "d
-00000650: 6576 220a 0a23 2049 6e74 6567 7261 7465  ev"..# Integrate
-00000660: 2044 6174 6162 7269 636b 7320 6a6f 6273   Databricks jobs
-00000670: 2069 6e74 6f20 796f 7572 2064 6174 6166   into your dataf
-00000680: 6c6f 7720 7769 7468 2070 7265 6665 6374  low with prefect
-00000690: 2d64 6174 6162 7269 636b 730a 200a 3c70  -databricks. .<p
-000006a0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-000006b0: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
-000006c0: 7474 7073 3a2f 2f75 7365 722d 696d 6167  ttps://user-imag
-000006d0: 6573 2e67 6974 6875 6275 7365 7263 6f6e  es.githubusercon
-000006e0: 7465 6e74 2e63 6f6d 2f31 3533 3331 3939  tent.com/1533199
-000006f0: 302f 3231 3938 3232 3433 392d 3730 6563  0/219822439-70ec
-00000700: 3832 6662 2d65 3933 612d 3439 3833 2d62  82fb-e93a-4983-b
-00000710: 6563 372d 3863 3832 3530 6662 6237 6163  ec7-8c8250fbb7ac
-00000720: 2e70 6e67 223e 0a20 2020 203c 6272 3e0a  .png">.    <br>.
-00000730: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
-00000740: 7073 3a2f 2f70 7970 692e 7079 7468 6f6e  ps://pypi.python
-00000750: 2e6f 7267 2f70 7970 692f 7072 6566 6563  .org/pypi/prefec
-00000760: 742d 6461 7461 6272 6963 6b73 2f22 2061  t-databricks/" a
-00000770: 6c74 3d22 5079 5049 2076 6572 7369 6f6e  lt="PyPI version
-00000780: 223e 0a20 2020 2020 2020 203c 696d 6720  ">.        <img 
-00000790: 616c 743d 2250 7950 4922 2073 7263 3d22  alt="PyPI" src="
-000007a0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000007b0: 6c64 732e 696f 2f70 7970 692f 762f 7072  lds.io/pypi/v/pr
-000007c0: 6566 6563 742d 6461 7461 6272 6963 6b73  efect-databricks
-000007d0: 3f63 6f6c 6f72 3d30 3035 3246 4626 6c61  ?color=0052FF&la
-000007e0: 6265 6c43 6f6c 6f72 3d30 3930 3432 3222  belColor=090422"
-000007f0: 3e3c 2f61 3e0a 2020 2020 3c61 2068 7265  ></a>.    <a hre
-00000800: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00000810: 622e 636f 6d2f 5072 6566 6563 7448 512f  b.com/PrefectHQ/
-00000820: 7072 6566 6563 742d 6461 7461 6272 6963  prefect-databric
-00000830: 6b73 2f22 2061 6c74 3d22 5374 6172 7322  ks/" alt="Stars"
-00000840: 3e0a 2020 2020 2020 2020 3c69 6d67 2073  >.        <img s
-00000850: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000860: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-00000870: 622f 7374 6172 732f 5072 6566 6563 7448  b/stars/PrefectH
-00000880: 512f 7072 6566 6563 742d 6461 7461 6272  Q/prefect-databr
-00000890: 6963 6b73 3f63 6f6c 6f72 3d30 3035 3246  icks?color=0052F
-000008a0: 4626 6c61 6265 6c43 6f6c 6f72 3d30 3930  F&labelColor=090
-000008b0: 3432 3222 202f 3e3c 2f61 3e0a 2020 2020  422" /></a>.    
-000008c0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000008d0: 2f70 6570 792e 7465 6368 2f62 6164 6765  /pepy.tech/badge
-000008e0: 2f70 7265 6665 6374 2d64 6174 6162 7269  /prefect-databri
-000008f0: 636b 732f 2220 616c 743d 2244 6f77 6e6c  cks/" alt="Downl
-00000900: 6f61 6473 223e 0a20 2020 2020 2020 203c  oads">.        <
-00000910: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00000920: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000930: 7079 7069 2f64 6d2f 7072 6566 6563 742d  pypi/dm/prefect-
-00000940: 6461 7461 6272 6963 6b73 3f63 6f6c 6f72  databricks?color
-00000950: 3d30 3035 3246 4626 6c61 6265 6c43 6f6c  =0052FF&labelCol
-00000960: 6f72 3d30 3930 3432 3222 202f 3e3c 2f61  or=090422" /></a
-00000970: 3e0a 2020 2020 3c61 2068 7265 663d 2268  >.    <a href="h
-00000980: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000990: 6d2f 5072 6566 6563 7448 512f 7072 6566  m/PrefectHQ/pref
-000009a0: 6563 742d 6461 7461 6272 6963 6b73 2f70  ect-databricks/p
-000009b0: 756c 7365 2220 616c 743d 2241 6374 6976  ulse" alt="Activ
-000009c0: 6974 7922 3e0a 2020 2020 2020 2020 3c69  ity">.        <i
-000009d0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-000009e0: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
-000009f0: 6974 6875 622f 636f 6d6d 6974 2d61 6374  ithub/commit-act
-00000a00: 6976 6974 792f 6d2f 5072 6566 6563 7448  ivity/m/PrefectH
-00000a10: 512f 7072 6566 6563 742d 6461 7461 6272  Q/prefect-databr
-00000a20: 6963 6b73 3f63 6f6c 6f72 3d30 3035 3246  icks?color=0052F
-00000a30: 4626 6c61 6265 6c43 6f6c 6f72 3d30 3930  F&labelColor=090
-00000a40: 3432 3222 202f 3e3c 2f61 3e0a 2020 2020  422" /></a>.    
-00000a50: 3c62 723e 0a20 2020 203c 6120 6872 6566  <br>.    <a href
-00000a60: 3d22 6874 7470 733a 2f2f 7072 6566 6563  ="https://prefec
-00000a70: 742d 636f 6d6d 756e 6974 792e 736c 6163  t-community.slac
-00000a80: 6b2e 636f 6d22 2061 6c74 3d22 536c 6163  k.com" alt="Slac
-00000a90: 6b22 3e0a 2020 2020 2020 2020 3c69 6d67  k">.        <img
-00000aa0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-00000ab0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00000ac0: 6765 2f73 6c61 636b 2d6a 6f69 6e5f 636f  ge/slack-join_co
-00000ad0: 6d6d 756e 6974 792d 7265 642e 7376 673f  mmunity-red.svg?
-00000ae0: 636f 6c6f 723d 3030 3532 4646 266c 6162  color=0052FF&lab
-00000af0: 656c 436f 6c6f 723d 3039 3034 3232 266c  elColor=090422&l
-00000b00: 6f67 6f3d 736c 6163 6b22 202f 3e3c 2f61  ogo=slack" /></a
-00000b10: 3e0a 2020 2020 3c61 2068 7265 663d 2268  >.    <a href="h
-00000b20: 7474 7073 3a2f 2f64 6973 636f 7572 7365  ttps://discourse
-00000b30: 2e70 7265 6665 6374 2e69 6f2f 2220 616c  .prefect.io/" al
-00000b40: 743d 2244 6973 636f 7572 7365 223e 0a20  t="Discourse">. 
-00000b50: 2020 2020 2020 203c 696d 6720 7372 633d         <img src=
-00000b60: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-00000b70: 656c 6473 2e69 6f2f 6261 6467 652f 6469  elds.io/badge/di
-00000b80: 7363 6f75 7273 652d 6272 6f77 7365 5f66  scourse-browse_f
-00000b90: 6f72 756d 2d72 6564 2e73 7667 3f63 6f6c  orum-red.svg?col
-00000ba0: 6f72 3d30 3035 3246 4626 6c61 6265 6c43  or=0052FF&labelC
-00000bb0: 6f6c 6f72 3d30 3930 3432 3226 6c6f 676f  olor=090422&logo
-00000bc0: 3d64 6973 636f 7572 7365 2220 2f3e 3c2f  =discourse" /></
-00000bd0: 613e 0a3c 2f70 3e0a 0a56 6973 6974 2074  a>.</p>..Visit t
-00000be0: 6865 2066 756c 6c20 646f 6373 205b 6865  he full docs [he
-00000bf0: 7265 5d28 6874 7470 733a 2f2f 5072 6566  re](https://Pref
-00000c00: 6563 7448 512e 6769 7468 7562 2e69 6f2f  ectHQ.github.io/
-00000c10: 7072 6566 6563 742d 6461 7461 6272 6963  prefect-databric
-00000c20: 6b73 2920 746f 2073 6565 2061 6464 6974  ks) to see addit
-00000c30: 696f 6e61 6c20 6578 616d 706c 6573 2061  ional examples a
-00000c40: 6e64 2074 6865 2041 5049 2072 6566 6572  nd the API refer
-00000c50: 656e 6365 2e0a 0a54 6865 2070 7265 6665  ence...The prefe
-00000c60: 6374 2d64 6174 6162 7269 636b 7320 636f  ct-databricks co
-00000c70: 6c6c 6563 7469 6f6e 206d 616b 6573 2069  llection makes i
-00000c80: 7420 6561 7379 2074 6f20 636f 6f72 6469  t easy to coordi
-00000c90: 616e 7465 2044 6174 6162 7269 636b 7320  ante Databricks 
-00000ca0: 6a6f 6273 2077 6974 6820 6f74 6865 7220  jobs with other 
-00000cb0: 746f 6f6c 7320 696e 2079 6f75 7220 6461  tools in your da
-00000cc0: 7461 2073 7461 636b 2075 7369 6e67 2050  ta stack using P
-00000cd0: 7265 6665 6374 2e20 4368 6563 6b20 6f75  refect. Check ou
-00000ce0: 7420 7468 6520 6578 616d 706c 6573 2062  t the examples b
-00000cf0: 656c 6f77 2074 6f20 6765 7420 7374 6172  elow to get star
-00000d00: 7465 6421 0a0a 2323 2047 6574 7469 6e67  ted!..## Getting
-00000d10: 2053 7461 7274 6564 0a0a 2323 2320 496e   Started..### In
-00000d20: 7465 6772 6174 6520 7769 7468 2050 7265  tegrate with Pre
-00000d30: 6665 6374 2066 6c6f 7773 0a0a 5573 696e  fect flows..Usin
-00000d40: 6720 5072 6566 6563 7420 7769 7468 2044  g Prefect with D
-00000d50: 6174 6162 7269 636b 7320 616c 6c6f 7773  atabricks allows
-00000d60: 2079 6f75 2074 6f20 6465 6669 6e65 2061   you to define a
-00000d70: 6e64 206f 7263 6865 7374 7261 7465 2063  nd orchestrate c
-00000d80: 6f6d 706c 6578 2064 6174 6120 776f 726b  omplex data work
-00000d90: 666c 6f77 7320 7468 6174 2074 616b 6520  flows that take 
-00000da0: 6164 7661 6e74 6167 6520 6f66 2074 6865  advantage of the
-00000db0: 2073 6361 6c61 6269 6c69 7479 2061 6e64   scalability and
-00000dc0: 2070 6572 666f 726d 616e 6365 206f 6620   performance of 
-00000dd0: 4461 7461 6272 6963 6b73 2e0a 0a54 6869  Databricks...Thi
-00000de0: 7320 6361 6e20 6265 2065 7370 6563 6961  s can be especia
-00000df0: 6c6c 7920 7573 6566 756c 2066 6f72 2064  lly useful for d
-00000e00: 6174 612d 696e 7465 6e73 6976 6520 7461  ata-intensive ta
-00000e10: 736b 7320 7375 6368 2061 7320 4554 4c20  sks such as ETL 
-00000e20: 2865 7874 7261 6374 2c20 7472 616e 7366  (extract, transf
-00000e30: 6f72 6d2c 206c 6f61 6429 2070 6970 656c  orm, load) pipel
-00000e40: 696e 6573 2c20 6d61 6368 696e 6520 6c65  ines, machine le
-00000e50: 6172 6e69 6e67 2074 7261 696e 696e 6720  arning training 
-00000e60: 616e 6420 696e 6665 7265 6e63 652c 2061  and inference, a
-00000e70: 6e64 2072 6561 6c2d 7469 6d65 2064 6174  nd real-time dat
-00000e80: 6120 7072 6f63 6573 7369 6e67 2e0a 0a42  a processing...B
-00000e90: 656c 6f77 2069 7320 616e 2065 7861 6d70  elow is an examp
-00000ea0: 6c65 206f 6620 686f 7720 796f 7520 6361  le of how you ca
-00000eb0: 6e20 696e 636f 7270 6f72 6174 6520 4461  n incorporate Da
-00000ec0: 7461 6272 6963 6b73 206e 6f74 6562 6f6f  tabricks noteboo
-00000ed0: 6b73 2077 6974 6869 6e20 796f 7572 2050  ks within your P
-00000ee0: 7265 6665 6374 2066 6c6f 7773 2e0a 0a42  refect flows...B
-00000ef0: 6520 7375 7265 2074 6f20 696e 7374 616c  e sure to instal
-00000f00: 6c20 5b70 7265 6665 6374 2d64 6174 6162  l [prefect-datab
-00000f10: 7269 636b 735d 2823 696e 7374 616c 6c61  ricks](#installa
-00000f20: 7469 6f6e 2920 616e 6420 5b73 6176 6520  tion) and [save 
-00000f30: 6120 6372 6564 656e 7469 616c 7320 626c  a credentials bl
-00000f40: 6f63 6b5d 2823 7361 7669 6e67 2d63 7265  ock](#saving-cre
-00000f50: 6465 6e74 6961 6c73 2d74 6f2d 626c 6f63  dentials-to-bloc
-00000f60: 6b29 2074 6f20 7275 6e20 7468 6520 6578  k) to run the ex
-00000f70: 616d 706c 6573 2062 656c 6f77 210a 0a49  amples below!..I
-00000f80: 6620 796f 7520 646f 6e27 7420 6861 7665  f you don't have
-00000f90: 2061 6e20 6578 6973 7469 6e67 206e 6f74   an existing not
-00000fa0: 6562 6f6f 6b20 7265 6164 7920 6f6e 2044  ebook ready on D
-00000fb0: 6174 6162 7269 636b 732c 2079 6f75 2063  atabricks, you c
-00000fc0: 616e 2063 6f70 7920 7468 6520 666f 6c6c  an copy the foll
-00000fd0: 6f77 696e 672c 2061 6e64 206e 616d 6520  owing, and name 
-00000fe0: 6974 2060 6578 616d 706c 652e 6970 796e  it `example.ipyn
-00000ff0: 6260 2e20 5468 6973 206e 6f74 6562 6f6f  b`. This noteboo
-00001000: 6b2c 2061 6363 6570 7473 2061 206e 616d  k, accepts a nam
-00001010: 6520 7061 7261 6d65 7465 7220 6672 6f6d  e parameter from
-00001020: 2074 6865 2066 6c6f 7720 616e 6420 7369   the flow and si
-00001030: 6d70 6c79 2070 7269 6e74 7320 6120 6d65  mply prints a me
-00001040: 7373 6167 652e 0a0a 6060 6070 7974 686f  ssage...```pytho
-00001050: 6e0a 6e61 6d65 203d 2064 6275 7469 6c73  n.name = dbutils
-00001060: 2e77 6964 6765 7473 2e67 6574 2822 6e61  .widgets.get("na
-00001070: 6d65 2229 0a6d 6573 7361 6765 203d 2066  me").message = f
-00001080: 2244 6f6e 2774 2077 6f72 7279 207b 6e61  "Don't worry {na
-00001090: 6d65 7d2c 2049 2067 6f74 2079 6f75 7220  me}, I got your 
-000010a0: 7265 7175 6573 7421 2057 656c 636f 6d65  request! Welcome
-000010b0: 2074 6f20 7072 6566 6563 742d 6461 7461   to prefect-data
-000010c0: 6272 6963 6b73 2122 0a70 7269 6e74 286d  bricks!".print(m
-000010d0: 6573 7361 6765 290a 6060 600a 0a48 6572  essage).```..Her
-000010e0: 652c 2074 6865 2066 6c6f 7720 6c61 756e  e, the flow laun
-000010f0: 6368 6573 2061 206e 6577 2063 6c75 7374  ches a new clust
-00001100: 6572 2074 6f20 7275 6e20 6065 7861 6d70  er to run `examp
-00001110: 6c65 2e69 7079 6e62 6020 616e 6420 7761  le.ipynb` and wa
-00001120: 6974 7320 666f 7220 7468 6520 636f 6d70  its for the comp
-00001130: 6c65 7469 6f6e 206f 6620 7468 6520 6e6f  letion of the no
-00001140: 7465 626f 6f6b 2072 756e 2e20 5265 706c  tebook run. Repl
-00001150: 6163 6520 7468 6520 706c 6163 6568 6f6c  ace the placehol
-00001160: 6465 7273 2061 6e64 2072 756e 2e0a 0a60  ders and run...`
-00001170: 6060 7079 7468 6f6e 0a66 726f 6d20 7072  ``python.from pr
-00001180: 6566 6563 7420 696d 706f 7274 2066 6c6f  efect import flo
-00001190: 770a 6672 6f6d 2070 7265 6665 6374 5f64  w.from prefect_d
-000011a0: 6174 6162 7269 636b 7320 696d 706f 7274  atabricks import
-000011b0: 2044 6174 6162 7269 636b 7343 7265 6465   DatabricksCrede
-000011c0: 6e74 6961 6c73 0a66 726f 6d20 7072 6566  ntials.from pref
-000011d0: 6563 745f 6461 7461 6272 6963 6b73 2e66  ect_databricks.f
-000011e0: 6c6f 7773 2069 6d70 6f72 7420 6a6f 6273  lows import jobs
-000011f0: 5f72 756e 735f 7375 626d 6974 5f61 6e64  _runs_submit_and
-00001200: 5f77 6169 745f 666f 725f 636f 6d70 6c65  _wait_for_comple
-00001210: 7469 6f6e 0a66 726f 6d20 7072 6566 6563  tion.from prefec
-00001220: 745f 6461 7461 6272 6963 6b73 2e6d 6f64  t_databricks.mod
-00001230: 656c 732e 6a6f 6273 2069 6d70 6f72 7420  els.jobs import 
-00001240: 280a 2020 2020 4175 746f 5363 616c 652c  (.    AutoScale,
-00001250: 0a20 2020 2041 7773 4174 7472 6962 7574  .    AwsAttribut
-00001260: 6573 2c0a 2020 2020 4a6f 6254 6173 6b53  es,.    JobTaskS
-00001270: 6574 7469 6e67 732c 0a20 2020 204e 6f74  ettings,.    Not
-00001280: 6562 6f6f 6b54 6173 6b2c 0a20 2020 204e  ebookTask,.    N
-00001290: 6577 436c 7573 7465 722c 0a29 0a0a 0a40  ewCluster,.)...@
-000012a0: 666c 6f77 0a64 6566 206a 6f62 735f 7275  flow.def jobs_ru
-000012b0: 6e73 5f73 7562 6d69 745f 666c 6f77 2862  ns_submit_flow(b
-000012c0: 6c6f 636b 5f6e 616d 653a 2073 7472 2c20  lock_name: str, 
-000012d0: 6e6f 7465 626f 6f6b 5f70 6174 683a 2073  notebook_path: s
-000012e0: 7472 2c20 2a2a 6261 7365 5f70 6172 616d  tr, **base_param
-000012f0: 6574 6572 7329 3a0a 2020 2020 6461 7461  eters):.    data
-00001300: 6272 6963 6b73 5f63 7265 6465 6e74 6961  bricks_credentia
-00001310: 6c73 203d 2044 6174 6162 7269 636b 7343  ls = DatabricksC
-00001320: 7265 6465 6e74 6961 6c73 2e6c 6f61 6428  redentials.load(
-00001330: 626c 6f63 6b5f 6e61 6d65 290a 0a20 2020  block_name)..   
-00001340: 2023 2073 7065 6369 6679 206e 6577 2063   # specify new c
-00001350: 6c75 7374 6572 2073 6574 7469 6e67 730a  luster settings.
-00001360: 2020 2020 6177 735f 6174 7472 6962 7574      aws_attribut
-00001370: 6573 203d 2041 7773 4174 7472 6962 7574  es = AwsAttribut
-00001380: 6573 280a 2020 2020 2020 2020 6176 6169  es(.        avai
-00001390: 6c61 6269 6c69 7479 3d22 5350 4f54 222c  lability="SPOT",
-000013a0: 0a20 2020 2020 2020 207a 6f6e 655f 6964  .        zone_id
-000013b0: 3d22 7573 2d77 6573 742d 3261 222c 0a20  ="us-west-2a",. 
-000013c0: 2020 2020 2020 2065 6273 5f76 6f6c 756d         ebs_volum
-000013d0: 655f 7479 7065 3d22 4745 4e45 5241 4c5f  e_type="GENERAL_
-000013e0: 5055 5250 4f53 455f 5353 4422 2c0a 2020  PURPOSE_SSD",.  
-000013f0: 2020 2020 2020 6562 735f 766f 6c75 6d65        ebs_volume
-00001400: 5f63 6f75 6e74 3d33 2c0a 2020 2020 2020  _count=3,.      
-00001410: 2020 6562 735f 766f 6c75 6d65 5f73 697a    ebs_volume_siz
-00001420: 653d 3130 302c 0a20 2020 2029 0a20 2020  e=100,.    ).   
-00001430: 2061 7574 6f5f 7363 616c 6520 3d20 4175   auto_scale = Au
-00001440: 746f 5363 616c 6528 6d69 6e5f 776f 726b  toScale(min_work
-00001450: 6572 733d 312c 206d 6178 5f77 6f72 6b65  ers=1, max_worke
-00001460: 7273 3d32 290a 2020 2020 6e65 775f 636c  rs=2).    new_cl
-00001470: 7573 7465 7220 3d20 4e65 7743 6c75 7374  uster = NewClust
-00001480: 6572 280a 2020 2020 2020 2020 6177 735f  er(.        aws_
-00001490: 6174 7472 6962 7574 6573 3d61 7773 5f61  attributes=aws_a
-000014a0: 7474 7269 6275 7465 732c 0a20 2020 2020  ttributes,.     
-000014b0: 2020 2061 7574 6f73 6361 6c65 3d61 7574     autoscale=aut
-000014c0: 6f5f 7363 616c 652c 0a20 2020 2020 2020  o_scale,.       
-000014d0: 206e 6f64 655f 7479 7065 5f69 643d 226d   node_type_id="m
-000014e0: 342e 6c61 7267 6522 2c0a 2020 2020 2020  4.large",.      
-000014f0: 2020 7370 6172 6b5f 7665 7273 696f 6e3d    spark_version=
-00001500: 2231 302e 342e 782d 7363 616c 6132 2e31  "10.4.x-scala2.1
-00001510: 3222 2c0a 2020 2020 2020 2020 7370 6172  2",.        spar
-00001520: 6b5f 636f 6e66 3d7b 2273 7061 726b 2e73  k_conf={"spark.s
-00001530: 7065 6375 6c61 7469 6f6e 223a 2054 7275  peculation": Tru
-00001540: 657d 2c0a 2020 2020 290a 0a20 2020 2023  e},.    )..    #
-00001550: 2073 7065 6369 6679 206e 6f74 6562 6f6f   specify noteboo
-00001560: 6b20 746f 2075 7365 2061 6e64 2070 6172  k to use and par
-00001570: 616d 6574 6572 7320 746f 2070 6173 730a  ameters to pass.
-00001580: 2020 2020 6e6f 7465 626f 6f6b 5f74 6173      notebook_tas
-00001590: 6b20 3d20 4e6f 7465 626f 6f6b 5461 736b  k = NotebookTask
-000015a0: 280a 2020 2020 2020 2020 6e6f 7465 626f  (.        notebo
-000015b0: 6f6b 5f70 6174 683d 6e6f 7465 626f 6f6b  ok_path=notebook
-000015c0: 5f70 6174 682c 0a20 2020 2020 2020 2062  _path,.        b
-000015d0: 6173 655f 7061 7261 6d65 7465 7273 3d62  ase_parameters=b
-000015e0: 6173 655f 7061 7261 6d65 7465 7273 2c0a  ase_parameters,.
-000015f0: 2020 2020 290a 0a20 2020 2023 2063 6f6d      )..    # com
-00001600: 7069 6c65 206a 6f62 2074 6173 6b20 7365  pile job task se
-00001610: 7474 696e 6773 0a20 2020 206a 6f62 5f74  ttings.    job_t
-00001620: 6173 6b5f 7365 7474 696e 6773 203d 204a  ask_settings = J
-00001630: 6f62 5461 736b 5365 7474 696e 6773 280a  obTaskSettings(.
-00001640: 2020 2020 2020 2020 6e65 775f 636c 7573          new_clus
-00001650: 7465 723d 6e65 775f 636c 7573 7465 722c  ter=new_cluster,
-00001660: 0a20 2020 2020 2020 206e 6f74 6562 6f6f  .        noteboo
-00001670: 6b5f 7461 736b 3d6e 6f74 6562 6f6f 6b5f  k_task=notebook_
-00001680: 7461 736b 2c0a 2020 2020 2020 2020 7461  task,.        ta
-00001690: 736b 5f6b 6579 3d22 7072 6566 6563 742d  sk_key="prefect-
-000016a0: 7461 736b 220a 2020 2020 290a 0a20 2020  task".    )..   
-000016b0: 2072 756e 203d 206a 6f62 735f 7275 6e73   run = jobs_runs
-000016c0: 5f73 7562 6d69 745f 616e 645f 7761 6974  _submit_and_wait
-000016d0: 5f66 6f72 5f63 6f6d 706c 6574 696f 6e28  _for_completion(
-000016e0: 0a20 2020 2020 2020 2064 6174 6162 7269  .        databri
-000016f0: 636b 735f 6372 6564 656e 7469 616c 733d  cks_credentials=
-00001700: 6461 7461 6272 6963 6b73 5f63 7265 6465  databricks_crede
-00001710: 6e74 6961 6c73 2c0a 2020 2020 2020 2020  ntials,.        
-00001720: 7275 6e5f 6e61 6d65 3d22 7072 6566 6563  run_name="prefec
-00001730: 742d 6a6f 6222 2c0a 2020 2020 2020 2020  t-job",.        
-00001740: 7461 736b 733d 5b6a 6f62 5f74 6173 6b5f  tasks=[job_task_
-00001750: 7365 7474 696e 6773 5d0a 2020 2020 290a  settings].    ).
-00001760: 0a20 2020 2072 6574 7572 6e20 7275 6e0a  .    return run.
-00001770: 0a0a 6a6f 6273 5f72 756e 735f 7375 626d  ..jobs_runs_subm
-00001780: 6974 5f66 6c6f 7728 0a20 2020 2062 6c6f  it_flow(.    blo
-00001790: 636b 5f6e 616d 653d 2242 4c4f 434b 2d4e  ck_name="BLOCK-N
-000017a0: 414d 452d 504c 4143 4548 4f4c 4445 5222  AME-PLACEHOLDER"
-000017b0: 0a20 2020 206e 6f74 6562 6f6f 6b5f 7061  .    notebook_pa
-000017c0: 7468 3d22 2f55 7365 7273 2f3c 454d 4149  th="/Users/<EMAI
-000017d0: 4c5f 4144 4452 4553 535f 504c 4143 4548  L_ADDRESS_PLACEH
-000017e0: 4f4c 4445 523e 2f65 7861 6d70 6c65 2e69  OLDER>/example.i
-000017f0: 7079 6e62 222c 0a20 2020 206e 616d 653d  pynb",.    name=
-00001800: 224d 6172 7669 6e22 0a29 0a60 6060 0a0a  "Marvin".).```..
-00001810: 5570 6f6e 2065 7865 6375 7469 6f6e 2c20  Upon execution, 
-00001820: 7468 6520 6e6f 7465 626f 6f6b 2072 756e  the notebook run
-00001830: 2073 686f 756c 6420 6f75 7470 7574 3a0a   should output:.
-00001840: 0a60 6060 0a44 6f6e 2774 2077 6f72 7279  .```.Don't worry
-00001850: 204d 6172 7669 6e2c 2049 2067 6f74 2079   Marvin, I got y
-00001860: 6f75 7220 7265 7175 6573 7421 2057 656c  our request! Wel
-00001870: 636f 6d65 2074 6f20 7072 6566 6563 742d  come to prefect-
-00001880: 6461 7461 6272 6963 6b73 210a 6060 600a  databricks!.```.
-00001890: 0a21 2121 2069 6e66 6f20 2249 6e70 7574  .!!! info "Input
-000018a0: 2064 6963 7469 6f6e 6172 6965 7320 696e   dictionaries in
-000018b0: 2074 6865 2070 6c61 6365 206f 6620 6d6f   the place of mo
-000018c0: 6465 6c73 220a 2020 2020 0a20 2020 2049  dels".    .    I
-000018d0: 6e73 7465 6164 206f 6620 7573 696e 6720  nstead of using 
-000018e0: 7468 6520 6275 696c 742d 696e 206d 6f64  the built-in mod
-000018f0: 656c 732c 2079 6f75 206d 6179 2061 6c73  els, you may als
-00001900: 6f20 696e 7075 7420 6120 7661 6c69 6420  o input a valid 
-00001910: 6469 6374 696f 6e61 7279 2e0a 2020 2020  dictionary..    
-00001920: 0a20 2020 2046 6f72 2065 7861 6d70 6c65  .    For example
-00001930: 2c20 7468 6520 666f 6c6c 6f77 696e 6720  , the following 
-00001940: 6172 6520 6571 7569 7661 6c65 6e74 3a0a  are equivalent:.
-00001950: 0a20 2020 2060 6060 7079 7468 6f6e 0a20  .    ```python. 
-00001960: 2020 2061 7574 6f5f 7363 616c 653d 4175     auto_scale=Au
-00001970: 746f 5363 616c 6528 6d69 6e5f 776f 726b  toScale(min_work
-00001980: 6572 733d 312c 206d 6178 5f77 6f72 6b65  ers=1, max_worke
-00001990: 7273 3d32 290a 2020 2020 6060 600a 0a20  rs=2).    ```.. 
-000019a0: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
-000019b0: 2061 7574 6f5f 7363 616c 653d 7b22 6d69   auto_scale={"mi
-000019c0: 6e5f 776f 726b 6572 7322 3a20 312c 2022  n_workers": 1, "
-000019d0: 6d61 785f 776f 726b 6572 7322 3a20 327d  max_workers": 2}
-000019e0: 0a20 2020 2060 6060 0a0a 4966 2079 6f75  .    ```..If you
-000019f0: 2068 6176 6520 616e 2065 7869 7374 696e   have an existin
-00001a00: 6720 4461 7461 6272 6963 6b73 206a 6f62  g Databricks job
-00001a10: 2c20 796f 7520 6361 6e20 7275 6e20 6974  , you can run it
-00001a20: 2075 7369 6e67 2060 6a6f 6273 5f72 756e   using `jobs_run
-00001a30: 735f 7375 626d 6974 5f62 795f 6964 5f61  s_submit_by_id_a
-00001a40: 6e64 5f77 6169 745f 666f 725f 636f 6d70  nd_wait_for_comp
-00001a50: 6c65 7469 6f6e 603a 0a0a 6060 6070 7974  letion`:..```pyt
-00001a60: 686f 6e0a 6672 6f6d 2070 7265 6665 6374  hon.from prefect
-00001a70: 2069 6d70 6f72 7420 666c 6f77 0a0a 6672   import flow..fr
-00001a80: 6f6d 2070 7265 6665 6374 5f64 6174 6162  om prefect_datab
-00001a90: 7269 636b 7320 696d 706f 7274 2044 6174  ricks import Dat
-00001aa0: 6162 7269 636b 7343 7265 6465 6e74 6961  abricksCredentia
-00001ab0: 6c73 0a66 726f 6d20 7072 6566 6563 745f  ls.from prefect_
-00001ac0: 6461 7461 6272 6963 6b73 2e66 6c6f 7773  databricks.flows
-00001ad0: 2069 6d70 6f72 7420 280a 2020 2020 6a6f   import (.    jo
-00001ae0: 6273 5f72 756e 735f 7375 626d 6974 5f62  bs_runs_submit_b
-00001af0: 795f 6964 5f61 6e64 5f77 6169 745f 666f  y_id_and_wait_fo
-00001b00: 725f 636f 6d70 6c65 7469 6f6e 2c0a 290a  r_completion,.).
-00001b10: 0a0a 4066 6c6f 770a 6465 6620 6578 6973  ..@flow.def exis
-00001b20: 7469 6e67 5f6a 6f62 5f73 7562 6d69 7428  ting_job_submit(
-00001b30: 6461 7461 6272 6963 6b73 5f63 7265 6465  databricks_crede
-00001b40: 6e74 6961 6c73 5f62 6c6f 636b 5f6e 616d  ntials_block_nam
-00001b50: 653a 2073 7472 2c20 6a6f 625f 6964 293a  e: str, job_id):
-00001b60: 0a20 2020 2064 6174 6162 7269 636b 735f  .    databricks_
-00001b70: 6372 6564 656e 7469 616c 7320 3d20 4461  credentials = Da
-00001b80: 7461 6272 6963 6b73 4372 6564 656e 7469  tabricksCredenti
-00001b90: 616c 732e 6c6f 6164 286e 616d 653d 626c  als.load(name=bl
-00001ba0: 6f63 6b5f 6e61 6d65 290a 0a20 2020 2072  ock_name)..    r
-00001bb0: 756e 203d 206a 6f62 735f 7275 6e73 5f73  un = jobs_runs_s
-00001bc0: 7562 6d69 745f 6279 5f69 645f 616e 645f  ubmit_by_id_and_
-00001bd0: 7761 6974 5f66 6f72 5f63 6f6d 706c 6574  wait_for_complet
-00001be0: 696f 6e28 0a20 2020 2020 2020 2064 6174  ion(.        dat
-00001bf0: 6162 7269 636b 735f 6372 6564 656e 7469  abricks_credenti
-00001c00: 616c 733d 6461 7461 6272 6963 6b73 5f63  als=databricks_c
-00001c10: 7265 6465 6e74 6961 6c73 2c20 6a6f 625f  redentials, job_
-00001c20: 6964 3d6a 6f62 5f69 640a 2020 2020 290a  id=job_id.    ).
-00001c30: 0a20 2020 2072 6574 7572 6e20 7275 6e0a  .    return run.
-00001c40: 0a65 7869 7374 696e 675f 6a6f 625f 7375  .existing_job_su
-00001c50: 626d 6974 2864 6174 6162 7269 636b 735f  bmit(databricks_
-00001c60: 6372 6564 656e 7469 616c 735f 626c 6f63  credentials_bloc
-00001c70: 6b5f 6e61 6d65 3d22 6462 2d63 7265 6473  k_name="db-creds
-00001c80: 222c 206a 6f62 5f69 643d 2259 4f55 522d  ", job_id="YOUR-
-00001c90: 4a4f 422d 4e41 4d45 2229 0a60 6060 0a0a  JOB-NAME").```..
-00001ca0: 2323 2052 6573 6f75 7263 6573 0a0a 466f  ## Resources..Fo
-00001cb0: 7220 6d6f 7265 2074 6970 7320 6f6e 2068  r more tips on h
-00001cc0: 6f77 2074 6f20 7573 6520 7461 736b 7320  ow to use tasks 
-00001cd0: 616e 6420 666c 6f77 7320 696e 2061 2043  and flows in a C
-00001ce0: 6f6c 6c65 6374 696f 6e2c 2063 6865 636b  ollection, check
-00001cf0: 206f 7574 205b 5573 696e 6720 436f 6c6c   out [Using Coll
-00001d00: 6563 7469 6f6e 735d 2868 7474 7073 3a2f  ections](https:/
-00001d10: 2f6f 7269 6f6e 2d64 6f63 732e 7072 6566  /orion-docs.pref
-00001d20: 6563 742e 696f 2f63 6f6c 6c65 6374 696f  ect.io/collectio
-00001d30: 6e73 2f75 7361 6765 2f29 210a 0a4e 6f74  ns/usage/)!..Not
-00001d40: 652c 2074 6865 2074 6173 6b73 2077 6974  e, the tasks wit
-00001d50: 6869 6e20 7468 6973 2063 6f6c 6c65 6374  hin this collect
-00001d60: 696f 6e20 7765 7265 2063 7265 6174 6564  ion were created
-00001d70: 2062 7920 6120 636f 6465 2067 656e 6572   by a code gener
-00001d80: 6174 6f72 2075 7369 6e67 2074 6865 2073  ator using the s
-00001d90: 6572 7669 6365 2773 204f 7065 6e41 5049  ervice's OpenAPI
-00001da0: 2073 7065 632e 0a0a 5468 6520 7365 7276   spec...The serv
-00001db0: 6963 6527 7320 5245 5354 2041 5049 2064  ice's REST API d
-00001dc0: 6f63 756d 656e 7461 7469 6f6e 2063 616e  ocumentation can
-00001dd0: 2062 6520 666f 756e 6420 5b68 6572 655d   be found [here]
-00001de0: 2868 7474 7073 3a2f 2f64 6f63 732e 6461  (https://docs.da
-00001df0: 7461 6272 6963 6b73 2e63 6f6d 2f64 6576  tabricks.com/dev
-00001e00: 2d74 6f6f 6c73 2f61 7069 2f6c 6174 6573  -tools/api/lates
-00001e10: 742f 696e 6465 782e 6874 6d6c 292e 0a0a  t/index.html)...
-00001e20: 2323 2320 496e 7374 616c 6c61 7469 6f6e  ### Installation
-00001e30: 0a0a 496e 7374 616c 6c20 6070 7265 6665  ..Install `prefe
-00001e40: 6374 2d64 6174 6162 7269 636b 7360 2077  ct-databricks` w
-00001e50: 6974 6820 6070 6970 603a 0a0a 6060 6062  ith `pip`:..```b
-00001e60: 6173 680a 7069 7020 696e 7374 616c 6c20  ash.pip install 
-00001e70: 7072 6566 6563 742d 6461 7461 6272 6963  prefect-databric
-00001e80: 6b73 0a60 6060 0a0a 5265 7175 6972 6573  ks.```..Requires
-00001e90: 2061 6e20 696e 7374 616c 6c61 7469 6f6e   an installation
-00001ea0: 206f 6620 5079 7468 6f6e 2033 2e37 2b2e   of Python 3.7+.
-00001eb0: 0a0a 5765 2072 6563 6f6d 6d65 6e64 2075  ..We recommend u
-00001ec0: 7369 6e67 2061 2050 7974 686f 6e20 7669  sing a Python vi
-00001ed0: 7274 7561 6c20 656e 7669 726f 6e6d 656e  rtual environmen
-00001ee0: 7420 6d61 6e61 6765 7220 7375 6368 2061  t manager such a
-00001ef0: 7320 7069 7065 6e76 2c20 636f 6e64 6120  s pipenv, conda 
-00001f00: 6f72 2076 6972 7475 616c 656e 762e 0a0a  or virtualenv...
-00001f10: 5468 6573 6520 7461 736b 7320 6172 6520  These tasks are 
-00001f20: 6465 7369 676e 6564 2074 6f20 776f 726b  designed to work
-00001f30: 2077 6974 6820 5072 6566 6563 7420 322e   with Prefect 2.
-00001f40: 2046 6f72 206d 6f72 6520 696e 666f 726d   For more inform
-00001f50: 6174 696f 6e20 6162 6f75 7420 686f 7720  ation about how 
-00001f60: 746f 2075 7365 2050 7265 6665 6374 2c20  to use Prefect, 
-00001f70: 706c 6561 7365 2072 6566 6572 2074 6f20  please refer to 
-00001f80: 7468 6520 5b50 7265 6665 6374 2064 6f63  the [Prefect doc
-00001f90: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
-00001fa0: 733a 2f2f 6f72 696f 6e2d 646f 6373 2e70  s://orion-docs.p
-00001fb0: 7265 6665 6374 2e69 6f2f 292e 0a0a 2323  refect.io/)...##
-00001fc0: 2320 5361 7669 6e67 2043 7265 6465 6e74  # Saving Credent
-00001fd0: 6961 6c73 2074 6f20 426c 6f63 6b0a 0a54  ials to Block..T
-00001fe0: 6f20 7573 6520 7468 6520 606c 6f61 6460  o use the `load`
-00001ff0: 206d 6574 686f 6420 6f6e 2042 6c6f 636b   method on Block
-00002000: 732c 2079 6f75 206d 7573 7420 616c 7265  s, you must alre
-00002010: 6164 7920 6861 7665 2061 2062 6c6f 636b  ady have a block
-00002020: 2064 6f63 756d 656e 7420 5b73 6176 6564   document [saved
-00002030: 2074 6872 6f75 6768 2063 6f64 655d 2868   through code](h
-00002040: 7474 7073 3a2f 2f6f 7269 6f6e 2d64 6f63  ttps://orion-doc
-00002050: 732e 7072 6566 6563 742e 696f 2f63 6f6e  s.prefect.io/con
-00002060: 6365 7074 732f 626c 6f63 6b73 2f23 7361  cepts/blocks/#sa
-00002070: 7669 6e67 2d62 6c6f 636b 7329 206f 7220  ving-blocks) or 
-00002080: 5b73 6176 6564 2074 6872 6f75 6768 2074  [saved through t
-00002090: 6865 2055 495d 2868 7474 7073 3a2f 2f6f  he UI](https://o
-000020a0: 7269 6f6e 2d64 6f63 732e 7072 6566 6563  rion-docs.prefec
-000020b0: 742e 696f 2f75 692f 626c 6f63 6b73 2f29  t.io/ui/blocks/)
-000020c0: 2e0a 0a42 656c 6f77 2069 7320 6120 7761  ...Below is a wa
-000020d0: 6c6b 7468 726f 7567 6820 6f6e 2073 6176  lkthrough on sav
-000020e0: 696e 6720 626c 6f63 6b20 646f 6375 6d65  ing block docume
-000020f0: 6e74 7320 7468 726f 7567 6820 636f 6465  nts through code
-00002100: 3b20 7369 6d70 6c79 2063 7265 6174 6520  ; simply create 
-00002110: 6120 7368 6f72 7420 7363 7269 7074 2c20  a short script, 
-00002120: 7265 706c 6163 696e 6720 7468 6520 706c  replacing the pl
-00002130: 6163 6568 6f6c 6465 7273 2e20 0a0a 312e  aceholders. ..1.
-00002140: 2048 6561 6420 6f76 6572 2074 6f20 5b44   Head over to [D
-00002150: 6174 6162 7269 636b 735d 2868 7474 7073  atabricks](https
-00002160: 3a2f 2f61 6363 6f75 6e74 732e 636c 6f75  ://accounts.clou
-00002170: 642e 6461 7461 6272 6963 6b73 2e63 6f6d  d.databricks.com
-00002180: 2f29 2e0a 322e 204c 6f67 696e 2074 6f20  /)..2. Login to 
-00002190: 796f 7572 2044 6174 6162 7269 636b 7320  your Databricks 
-000021a0: 6163 636f 756e 7420 616e 6420 7365 6c65  account and sele
-000021b0: 6374 2061 2077 6f72 6b73 7061 6365 2e0a  ct a workspace..
-000021c0: 332e 204f 6e20 7468 6520 746f 7020 7269  3. On the top ri
-000021d0: 6768 7420 7369 6465 206f 6620 7468 6520  ght side of the 
-000021e0: 6e61 7620 6261 722c 2063 6c69 636b 206f  nav bar, click o
-000021f0: 6e20 796f 7572 2061 6363 6f75 6e74 206e  n your account n
-00002200: 616d 6520 2d3e 2055 7365 7220 5365 7474  ame -> User Sett
-00002210: 696e 6773 2e0a 342e 2043 6c69 636b 2041  ings..4. Click A
-00002220: 6363 6573 7320 746f 6b65 6e73 202d 3e20  ccess tokens -> 
-00002230: 4765 6e65 7261 7465 206e 6577 2074 6f6b  Generate new tok
-00002240: 656e 202d 3e20 4765 6e65 7261 7465 2061  en -> Generate a
-00002250: 6e64 2063 6f70 7920 7468 6520 746f 6b65  nd copy the toke
-00002260: 6e2e 0a35 2e20 4e6f 7465 2064 6f77 6e20  n..5. Note down 
-00002270: 796f 7572 2044 6174 6162 7269 636b 7320  your Databricks 
-00002280: 696e 7374 616e 6365 2066 726f 6d20 7468  instance from th
-00002290: 6520 6272 6f77 7365 7220 5552 4c2c 2066  e browser URL, f
-000022a0: 6f72 6d61 7474 6564 206c 696b 6520 6068  ormatted like `h
-000022b0: 7474 7073 3a2f 2f3c 4441 5441 4252 4943  ttps://<DATABRIC
-000022c0: 4b53 2d49 4e53 5441 4e43 453e 2e63 6c6f  KS-INSTANCE>.clo
-000022d0: 7564 2e64 6174 6162 7269 636b 732e 636f  ud.databricks.co
-000022e0: 6d2f 600a 362e 2043 7265 6174 6520 6120  m/`.6. Create a 
-000022f0: 7368 6f72 7420 7363 7269 7074 2c20 7265  short script, re
-00002300: 706c 6163 696e 6720 7468 6520 706c 6163  placing the plac
-00002310: 6568 6f6c 6465 7273 2e0a 0a60 6060 7079  eholders...```py
-00002320: 7468 6f6e 0a66 726f 6d20 7072 6566 6563  thon.from prefec
-00002330: 745f 6461 7461 6272 6963 6b73 2069 6d70  t_databricks imp
-00002340: 6f72 7420 4461 7461 6272 6963 6b73 4372  ort DatabricksCr
-00002350: 6564 656e 7469 616c 730a 0a63 7265 6465  edentials..crede
-00002360: 6e74 6961 6c73 203d 2044 6174 6162 7269  ntials = Databri
-00002370: 636b 7343 7265 6465 6e74 6961 6c73 280a  cksCredentials(.
-00002380: 2020 2020 6461 7461 6272 6963 6b73 5f69      databricks_i
-00002390: 6e73 7461 6e63 653d 2244 4154 4142 5249  nstance="DATABRI
-000023a0: 434b 532d 494e 5354 414e 4345 2d50 4c41  CKS-INSTANCE-PLA
-000023b0: 4345 484f 4c44 4552 220a 2020 2020 746f  CEHOLDER".    to
-000023c0: 6b65 6e3d 2254 4f4b 454e 2d50 4c41 4345  ken="TOKEN-PLACE
-000023d0: 484f 4c44 4552 220a 290a 0a63 6f6e 6e65  HOLDER".)..conne
-000023e0: 6374 6f72 2e73 6176 6528 2242 4c4f 434b  ctor.save("BLOCK
-000023f0: 5f4e 414d 452d 504c 4143 4548 4f4c 4445  _NAME-PLACEHOLDE
-00002400: 5222 290a 6060 600a 0a43 6f6e 6772 6174  R").```..Congrat
-00002410: 7321 2059 6f75 2063 616e 206e 6f77 2065  s! You can now e
-00002420: 6173 696c 7920 6c6f 6164 2074 6865 2073  asily load the s
-00002430: 6176 6564 2062 6c6f 636b 2c20 7768 6963  aved block, whic
-00002440: 6820 686f 6c64 7320 796f 7572 2063 7265  h holds your cre
-00002450: 6465 6e74 6961 6c73 3a0a 0a60 6060 7079  dentials:..```py
-00002460: 7468 6f6e 0a66 726f 6d20 7072 6566 6563  thon.from prefec
-00002470: 745f 6461 7461 6272 6963 6b73 2069 6d70  t_databricks imp
-00002480: 6f72 7420 4461 7461 6272 6963 6b73 4372  ort DatabricksCr
-00002490: 6564 656e 7469 616c 730a 0a44 6174 6162  edentials..Datab
-000024a0: 7269 636b 7343 7265 6465 6e74 6961 6c73  ricksCredentials
-000024b0: 2e6c 6f61 6428 2242 4c4f 434b 5f4e 414d  .load("BLOCK_NAM
-000024c0: 452d 504c 4143 4548 4f4c 4445 5222 290a  E-PLACEHOLDER").
-000024d0: 6060 600a 0a21 2121 2069 6e66 6f20 2252  ```..!!! info "R
-000024e0: 6567 6973 7465 7269 6e67 2062 6c6f 636b  egistering block
-000024f0: 7322 0a0a 2020 2020 5265 6769 7374 6572  s"..    Register
-00002500: 2062 6c6f 636b 7320 696e 2074 6869 7320   blocks in this 
-00002510: 6d6f 6475 6c65 2074 6f0a 2020 2020 5b76  module to.    [v
-00002520: 6965 7720 616e 6420 6564 6974 2074 6865  iew and edit the
-00002530: 6d5d 2868 7474 7073 3a2f 2f6f 7269 6f6e  m](https://orion
-00002540: 2d64 6f63 732e 7072 6566 6563 742e 696f  -docs.prefect.io
-00002550: 2f75 692f 626c 6f63 6b73 2f29 0a20 2020  /ui/blocks/).   
-00002560: 206f 6e20 5072 6566 6563 7420 436c 6f75   on Prefect Clou
-00002570: 643a 0a0a 2020 2020 6060 6062 6173 680a  d:..    ```bash.
-00002580: 2020 2020 7072 6566 6563 7420 626c 6f63      prefect bloc
-00002590: 6b20 7265 6769 7374 6572 202d 6d20 7072  k register -m pr
-000025a0: 6566 6563 745f 6461 7461 6272 6963 6b73  efect_databricks
-000025b0: 0a20 2020 2060 6060 0a0a 2323 2320 4665  .    ```..### Fe
-000025c0: 6564 6261 636b 0a0a 4966 2079 6f75 2065  edback..If you e
-000025d0: 6e63 6f75 6e74 6572 2061 6e79 2062 7567  ncounter any bug
-000025e0: 7320 7768 696c 6520 7573 696e 6720 6070  s while using `p
-000025f0: 7265 6665 6374 2d64 6174 6162 7269 636b  refect-databrick
-00002600: 7360 2c20 6665 656c 2066 7265 6520 746f  s`, feel free to
-00002610: 206f 7065 6e20 616e 2069 7373 7565 2069   open an issue i
-00002620: 6e20 7468 6520 5b70 7265 6665 6374 2d64  n the [prefect-d
-00002630: 6174 6162 7269 636b 735d 2868 7474 7073  atabricks](https
-00002640: 3a2f 2f67 6974 6875 622e 636f 6d2f 5072  ://github.com/Pr
-00002650: 6566 6563 7448 512f 7072 6566 6563 742d  efectHQ/prefect-
-00002660: 6461 7461 6272 6963 6b73 2920 7265 706f  databricks) repo
-00002670: 7369 746f 7279 2e0a 0a49 6620 796f 7520  sitory...If you 
-00002680: 6861 7665 2061 6e79 2071 7565 7374 696f  have any questio
-00002690: 6e73 206f 7220 6973 7375 6573 2077 6869  ns or issues whi
-000026a0: 6c65 2075 7369 6e67 2060 7072 6566 6563  le using `prefec
-000026b0: 742d 6461 7461 6272 6963 6b73 602c 2079  t-databricks`, y
-000026c0: 6f75 2063 616e 2066 696e 6420 6865 6c70  ou can find help
-000026d0: 2069 6e20 6569 7468 6572 2074 6865 205b   in either the [
-000026e0: 5072 6566 6563 7420 4469 7363 6f75 7273  Prefect Discours
-000026f0: 6520 666f 7275 6d5d 2868 7474 7073 3a2f  e forum](https:/
-00002700: 2f64 6973 636f 7572 7365 2e70 7265 6665  /discourse.prefe
-00002710: 6374 2e69 6f2f 2920 6f72 2074 6865 205b  ct.io/) or the [
-00002720: 5072 6566 6563 7420 536c 6163 6b20 636f  Prefect Slack co
-00002730: 6d6d 756e 6974 795d 2868 7474 7073 3a2f  mmunity](https:/
-00002740: 2f70 7265 6665 6374 2e69 6f2f 736c 6163  /prefect.io/slac
-00002750: 6b29 2e0a 0a46 6565 6c20 6672 6565 2074  k)...Feel free t
-00002760: 6f20 7374 6172 206f 7220 7761 7463 6820  o star or watch 
-00002770: 5b60 7072 6566 6563 742d 6461 7461 6272  [`prefect-databr
-00002780: 6963 6b73 605d 2868 7474 7073 3a2f 2f67  icks`](https://g
-00002790: 6974 6875 622e 636f 6d2f 5072 6566 6563  ithub.com/Prefec
-000027a0: 7448 512f 7072 6566 6563 742d 6461 7461  tHQ/prefect-data
-000027b0: 6272 6963 6b73 2920 666f 7220 7570 6461  bricks) for upda
-000027c0: 7465 7320 746f 6f21 0a0a 2323 2320 436f  tes too!..### Co
-000027d0: 6e74 7269 6275 7469 6e67 0a0a 4966 2079  ntributing..If y
-000027e0: 6f75 2764 206c 696b 6520 746f 2068 656c  ou'd like to hel
-000027f0: 7020 636f 6e74 7269 6275 7465 2074 6f20  p contribute to 
-00002800: 6669 7820 616e 2069 7373 7565 206f 7220  fix an issue or 
-00002810: 6164 6420 6120 6665 6174 7572 6520 746f  add a feature to
-00002820: 2060 7072 6566 6563 742d 6461 7461 6272   `prefect-databr
-00002830: 6963 6b73 602c 2070 6c65 6173 6520 5b70  icks`, please [p
-00002840: 726f 706f 7365 2063 6861 6e67 6573 2074  ropose changes t
-00002850: 6872 6f75 6768 2061 2070 756c 6c20 7265  hrough a pull re
-00002860: 7175 6573 7420 6672 6f6d 2061 2066 6f72  quest from a for
-00002870: 6b20 6f66 2074 6865 2072 6570 6f73 6974  k of the reposit
-00002880: 6f72 795d 2868 7474 7073 3a2f 2f64 6f63  ory](https://doc
-00002890: 732e 6769 7468 7562 2e63 6f6d 2f65 6e2f  s.github.com/en/
-000028a0: 7075 6c6c 2d72 6571 7565 7374 732f 636f  pull-requests/co
-000028b0: 6c6c 6162 6f72 6174 696e 672d 7769 7468  llaborating-with
-000028c0: 2d70 756c 6c2d 7265 7175 6573 7473 2f70  -pull-requests/p
-000028d0: 726f 706f 7369 6e67 2d63 6861 6e67 6573  roposing-changes
-000028e0: 2d74 6f2d 796f 7572 2d77 6f72 6b2d 7769  -to-your-work-wi
-000028f0: 7468 2d70 756c 6c2d 7265 7175 6573 7473  th-pull-requests
-00002900: 2f63 7265 6174 696e 672d 612d 7075 6c6c  /creating-a-pull
-00002910: 2d72 6571 7565 7374 2d66 726f 6d2d 612d  -request-from-a-
-00002920: 666f 726b 292e 0a0a 4865 7265 2061 7265  fork)...Here are
-00002930: 2074 6865 2073 7465 7073 3a0a 0a31 2e20   the steps:..1. 
-00002940: 5b46 6f72 6b20 7468 6520 7265 706f 7369  [Fork the reposi
-00002950: 746f 7279 5d28 6874 7470 733a 2f2f 646f  tory](https://do
-00002960: 6373 2e67 6974 6875 622e 636f 6d2f 656e  cs.github.com/en
-00002970: 2f67 6574 2d73 7461 7274 6564 2f71 7569  /get-started/qui
-00002980: 636b 7374 6172 742f 666f 726b 2d61 2d72  ckstart/fork-a-r
-00002990: 6570 6f23 666f 726b 696e 672d 612d 7265  epo#forking-a-re
-000029a0: 706f 7369 746f 7279 290a 322e 205b 436c  pository).2. [Cl
-000029b0: 6f6e 6520 7468 6520 666f 726b 6564 2072  one the forked r
-000029c0: 6570 6f73 6974 6f72 795d 2868 7474 7073  epository](https
-000029d0: 3a2f 2f64 6f63 732e 6769 7468 7562 2e63  ://docs.github.c
-000029e0: 6f6d 2f65 6e2f 6765 742d 7374 6172 7465  om/en/get-starte
-000029f0: 642f 7175 6963 6b73 7461 7274 2f66 6f72  d/quickstart/for
-00002a00: 6b2d 612d 7265 706f 2363 6c6f 6e69 6e67  k-a-repo#cloning
-00002a10: 2d79 6f75 722d 666f 726b 6564 2d72 6570  -your-forked-rep
-00002a20: 6f73 6974 6f72 7929 0a33 2e20 496e 7374  ository).3. Inst
-00002a30: 616c 6c20 7468 6520 7265 706f 7369 746f  all the reposito
-00002a40: 7279 2061 6e64 2069 7473 2064 6570 656e  ry and its depen
-00002a50: 6465 6e63 6965 733a 0a60 6060 0a70 6970  dencies:.```.pip
-00002a60: 2069 6e73 7461 6c6c 202d 6520 222e 5b64   install -e ".[d
-00002a70: 6576 5d22 0a60 6060 0a34 2e20 4d61 6b65  ev]".```.4. Make
-00002a80: 2064 6573 6972 6564 2063 6861 6e67 6573   desired changes
-00002a90: 0a35 2e20 4164 6420 7465 7374 730a 362e  .5. Add tests.6.
-00002aa0: 2049 6e73 6572 7420 616e 2065 6e74 7279   Insert an entry
-00002ab0: 2074 6f20 5b43 4841 4e47 454c 4f47 2e6d   to [CHANGELOG.m
-00002ac0: 645d 2868 7474 7073 3a2f 2f67 6974 6875  d](https://githu
-00002ad0: 622e 636f 6d2f 5072 6566 6563 7448 512f  b.com/PrefectHQ/
-00002ae0: 7072 6566 6563 742d 6461 7461 6272 6963  prefect-databric
-00002af0: 6b73 2f62 6c6f 622f 6d61 696e 2f43 4841  ks/blob/main/CHA
-00002b00: 4e47 454c 4f47 2e6d 6429 0a37 2e20 496e  NGELOG.md).7. In
-00002b10: 7374 616c 6c20 6070 7265 2d63 6f6d 6d69  stall `pre-commi
-00002b20: 7460 2074 6f20 7065 7266 6f72 6d20 7175  t` to perform qu
-00002b30: 616c 6974 7920 6368 6563 6b73 2070 7269  ality checks pri
-00002b40: 6f72 2074 6f20 636f 6d6d 6974 3a0a 6060  or to commit:.``
-00002b50: 600a 7072 652d 636f 6d6d 6974 2069 6e73  `.pre-commit ins
-00002b60: 7461 6c6c 0a60 6060 0a38 2e20 6067 6974  tall.```.8. `git
-00002b70: 2063 6f6d 6d69 7460 2c20 6067 6974 2070   commit`, `git p
-00002b80: 7573 6860 2c20 616e 6420 6372 6561 7465  ush`, and create
-00002b90: 2061 2070 756c 6c20 7265 7175 6573 740a   a pull request.
+00000050: 6e74 6567 7261 7469 6f6e 7320 7769 7468  ntegrations with
+00000060: 2044 6174 6162 7269 636b 730a 4175 7468   Databricks.Auth
+00000070: 6f72 2d65 6d61 696c 3a20 2250 7265 6665  or-email: "Prefe
+00000080: 6374 2054 6563 686e 6f6c 6f67 6965 732c  ct Technologies,
+00000090: 2049 6e63 2e22 203c 6865 6c70 4070 7265   Inc." <help@pre
+000000a0: 6665 6374 2e69 6f3e 0a4c 6963 656e 7365  fect.io>.License
+000000b0: 3a20 4170 6163 6865 204c 6963 656e 7365  : Apache License
+000000c0: 2032 2e30 0a50 726f 6a65 6374 2d55 524c   2.0.Project-URL
+000000d0: 3a20 486f 6d65 7061 6765 2c20 6874 7470  : Homepage, http
+000000e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f50  s://github.com/P
+000000f0: 7265 6665 6374 4851 2f70 7265 6665 6374  refectHQ/prefect
+00000100: 2f74 7265 652f 6d61 696e 2f73 7263 2f69  /tree/main/src/i
+00000110: 6e74 6567 7261 7469 6f6e 732f 7072 6566  ntegrations/pref
+00000120: 6563 742d 6461 7461 6272 6963 6b73 0a4b  ect-databricks.K
+00000130: 6579 776f 7264 733a 2070 7265 6665 6374  eywords: prefect
+00000140: 0a43 6c61 7373 6966 6965 723a 204e 6174  .Classifier: Nat
+00000150: 7572 616c 204c 616e 6775 6167 6520 3a3a  ural Language ::
+00000160: 2045 6e67 6c69 7368 0a43 6c61 7373 6966   English.Classif
+00000170: 6965 723a 2049 6e74 656e 6465 6420 4175  ier: Intended Au
+00000180: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
+00000190: 7065 7273 0a43 6c61 7373 6966 6965 723a  pers.Classifier:
+000001a0: 2049 6e74 656e 6465 6420 4175 6469 656e   Intended Audien
+000001b0: 6365 203a 3a20 5379 7374 656d 2041 646d  ce :: System Adm
+000001c0: 696e 6973 7472 6174 6f72 730a 436c 6173  inistrators.Clas
+000001d0: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
+000001e0: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+000001f0: 3a3a 2041 7061 6368 6520 536f 6674 7761  :: Apache Softwa
+00000200: 7265 204c 6963 656e 7365 0a43 6c61 7373  re License.Class
+00000210: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000220: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000230: 7974 686f 6e20 3a3a 2033 203a 3a20 4f6e  ython :: 3 :: On
+00000240: 6c79 0a43 6c61 7373 6966 6965 723a 2050  ly.Classifier: P
+00000250: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000260: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000270: 2033 2e38 0a43 6c61 7373 6966 6965 723a   3.8.Classifier:
+00000280: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000290: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000002a0: 3a3a 2033 2e39 0a43 6c61 7373 6966 6965  :: 3.9.Classifie
+000002b0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000002c0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000002d0: 6e20 3a3a 2033 2e31 300a 436c 6173 7369  n :: 3.10.Classi
+000002e0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+000002f0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000300: 7468 6f6e 203a 3a20 332e 3131 0a43 6c61  thon :: 3.11.Cla
+00000310: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000320: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000330: 2050 7974 686f 6e20 3a3a 2033 2e31 320a   Python :: 3.12.
+00000340: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
+00000350: 6320 3a3a 2053 6f66 7477 6172 6520 4465  c :: Software De
+00000360: 7665 6c6f 706d 656e 7420 3a3a 204c 6962  velopment :: Lib
+00000370: 7261 7269 6573 0a52 6571 7569 7265 732d  raries.Requires-
+00000380: 5079 7468 6f6e 3a20 3e3d 332e 380a 4465  Python: >=3.8.De
+00000390: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
+000003a0: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
+000003b0: 6b64 6f77 6e0a 5265 7175 6972 6573 2d44  kdown.Requires-D
+000003c0: 6973 743a 2070 7265 6665 6374 3e3d 322e  ist: prefect>=2.
+000003d0: 3134 2e31 300a 5072 6f76 6964 6573 2d45  14.10.Provides-E
+000003e0: 7874 7261 3a20 6465 760a 5265 7175 6972  xtra: dev.Requir
+000003f0: 6573 2d44 6973 743a 2063 6f76 6572 6167  es-Dist: coverag
+00000400: 653b 2065 7874 7261 203d 3d20 2264 6576  e; extra == "dev
+00000410: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000420: 2069 6e74 6572 726f 6761 7465 3b20 6578   interrogate; ex
+00000430: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
+00000440: 7569 7265 732d 4469 7374 3a20 6d6b 646f  uires-Dist: mkdo
+00000450: 6373 2d67 656e 2d66 696c 6573 3b20 6578  cs-gen-files; ex
+00000460: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
+00000470: 7569 7265 732d 4469 7374 3a20 6d6b 646f  uires-Dist: mkdo
+00000480: 6373 2d6d 6174 6572 6961 6c3b 2065 7874  cs-material; ext
+00000490: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
+000004a0: 6972 6573 2d44 6973 743a 206d 6b64 6f63  ires-Dist: mkdoc
+000004b0: 733b 2065 7874 7261 203d 3d20 2264 6576  s; extra == "dev
+000004c0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+000004d0: 206d 6b64 6f63 7374 7269 6e67 735b 7079   mkdocstrings[py
+000004e0: 7468 6f6e 5d3b 2065 7874 7261 203d 3d20  thon]; extra == 
+000004f0: 2264 6576 220a 5265 7175 6972 6573 2d44  "dev".Requires-D
+00000500: 6973 743a 206d 6f63 6b3b 2070 7974 686f  ist: mock; pytho
+00000510: 6e5f 7665 7273 696f 6e20 3c20 2233 2e38  n_version < "3.8
+00000520: 2220 616e 6420 6578 7472 6120 3d3d 2022  " and extra == "
+00000530: 6465 7622 0a52 6571 7569 7265 732d 4469  dev".Requires-Di
+00000540: 7374 3a20 6d79 7079 3b20 6578 7472 6120  st: mypy; extra 
+00000550: 3d3d 2022 6465 7622 0a52 6571 7569 7265  == "dev".Require
+00000560: 732d 4469 7374 3a20 7069 6c6c 6f77 3b20  s-Dist: pillow; 
+00000570: 6578 7472 6120 3d3d 2022 6465 7622 0a52  extra == "dev".R
+00000580: 6571 7569 7265 732d 4469 7374 3a20 7072  equires-Dist: pr
+00000590: 652d 636f 6d6d 6974 3b20 6578 7472 6120  e-commit; extra 
+000005a0: 3d3d 2022 6465 7622 0a52 6571 7569 7265  == "dev".Require
+000005b0: 732d 4469 7374 3a20 7079 7465 7374 2d61  s-Dist: pytest-a
+000005c0: 7379 6e63 696f 3b20 6578 7472 6120 3d3d  syncio; extra ==
+000005d0: 2022 6465 7622 0a52 6571 7569 7265 732d   "dev".Requires-
+000005e0: 4469 7374 3a20 7079 7465 7374 3b20 6578  Dist: pytest; ex
+000005f0: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
+00000600: 7569 7265 732d 4469 7374 3a20 7079 7465  uires-Dist: pyte
+00000610: 7374 2d78 6469 7374 3b20 6578 7472 6120  st-xdist; extra 
+00000620: 3d3d 2022 6465 7622 0a52 6571 7569 7265  == "dev".Require
+00000630: 732d 4469 7374 3a20 7265 7370 783b 2065  s-Dist: respx; e
+00000640: 7874 7261 203d 3d20 2264 6576 220a 0a23  xtra == "dev"..#
+00000650: 2070 7265 6665 6374 2d64 6174 6162 7269   prefect-databri
+00000660: 636b 730a 0a56 6973 6974 2074 6865 2066  cks..Visit the f
+00000670: 756c 6c20 646f 6373 205b 6865 7265 5d28  ull docs [here](
+00000680: 6874 7470 733a 2f2f 5072 6566 6563 7448  https://PrefectH
+00000690: 512e 6769 7468 7562 2e69 6f2f 7072 6566  Q.github.io/pref
+000006a0: 6563 742d 6461 7461 6272 6963 6b73 2920  ect-databricks) 
+000006b0: 746f 2073 6565 2061 6464 6974 696f 6e61  to see additiona
+000006c0: 6c20 6578 616d 706c 6573 2061 6e64 2074  l examples and t
+000006d0: 6865 2041 5049 2072 6566 6572 656e 6365  he API reference
+000006e0: 2e0a 200a 3c70 2061 6c69 676e 3d22 6365  .. .<p align="ce
+000006f0: 6e74 6572 223e 0a20 2020 203c 6120 6872  nter">.    <a hr
+00000700: 6566 3d22 6874 7470 733a 2f2f 7079 7069  ef="https://pypi
+00000710: 2e70 7974 686f 6e2e 6f72 672f 7079 7069  .python.org/pypi
+00000720: 2f70 7265 6665 6374 2d64 6174 6162 7269  /prefect-databri
+00000730: 636b 732f 2220 616c 743d 2250 7950 4920  cks/" alt="PyPI 
+00000740: 7665 7273 696f 6e22 3e0a 2020 2020 2020  version">.      
+00000750: 2020 3c69 6d67 2061 6c74 3d22 5079 5049    <img alt="PyPI
+00000760: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
+00000770: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000780: 7069 2f76 2f70 7265 6665 6374 2d64 6174  pi/v/prefect-dat
+00000790: 6162 7269 636b 733f 636f 6c6f 723d 3030  abricks?color=00
+000007a0: 3532 4646 266c 6162 656c 436f 6c6f 723d  52FF&labelColor=
+000007b0: 3039 3034 3232 223e 3c2f 613e 0a20 2020  090422"></a>.   
+000007c0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000007d0: 2f2f 7065 7079 2e74 6563 682f 6261 6467  //pepy.tech/badg
+000007e0: 652f 7072 6566 6563 742d 6461 7461 6272  e/prefect-databr
+000007f0: 6963 6b73 2f22 2061 6c74 3d22 446f 776e  icks/" alt="Down
+00000800: 6c6f 6164 7322 3e0a 2020 2020 2020 2020  loads">.        
+00000810: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000820: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000830: 2f70 7970 692f 646d 2f70 7265 6665 6374  /pypi/dm/prefect
+00000840: 2d64 6174 6162 7269 636b 733f 636f 6c6f  -databricks?colo
+00000850: 723d 3030 3532 4646 266c 6162 656c 436f  r=0052FF&labelCo
+00000860: 6c6f 723d 3039 3034 3232 2220 2f3e 3c2f  lor=090422" /></
+00000870: 613e 0a20 2020 203c 6120 6872 6566 3d22  a>.    <a href="
+00000880: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000890: 6f6d 2f50 7265 6665 6374 4851 2f70 7265  om/PrefectHQ/pre
+000008a0: 6665 6374 2d64 6174 6162 7269 636b 732f  fect-databricks/
+000008b0: 7075 6c73 6522 2061 6c74 3d22 4163 7469  pulse" alt="Acti
+000008c0: 7669 7479 223e 0a3c 2f70 3e0a 0a23 2320  vity">.</p>..## 
+000008d0: 5765 6c63 6f6d 6521 0a0a 5072 6566 6563  Welcome!..Prefec
+000008e0: 7420 696e 7465 6772 6174 696f 6e73 2066  t integrations f
+000008f0: 6f72 2069 6e74 6572 6163 7469 6e67 2077  or interacting w
+00000900: 6974 6820 4461 7461 6272 6963 6b73 0a0a  ith Databricks..
+00000910: 5468 6520 7461 736b 7320 7769 7468 696e  The tasks within
+00000920: 2074 6869 7320 636f 6c6c 6563 7469 6f6e   this collection
+00000930: 2077 6572 6520 6372 6561 7465 6420 6279   were created by
+00000940: 2061 2063 6f64 6520 6765 6e65 7261 746f   a code generato
+00000950: 7220 7573 696e 6720 7468 6520 7365 7276  r using the serv
+00000960: 6963 6527 7320 4f70 656e 4150 4920 7370  ice's OpenAPI sp
+00000970: 6563 2e0a 0a54 6865 2073 6572 7669 6365  ec...The service
+00000980: 2773 2052 4553 5420 4150 4920 646f 6375  's REST API docu
+00000990: 6d65 6e74 6174 696f 6e20 6361 6e20 6265  mentation can be
+000009a0: 2066 6f75 6e64 205b 6865 7265 5d28 6874   found [here](ht
+000009b0: 7470 733a 2f2f 646f 6373 2e64 6174 6162  tps://docs.datab
+000009c0: 7269 636b 732e 636f 6d2f 6465 762d 746f  ricks.com/dev-to
+000009d0: 6f6c 732f 6170 692f 6c61 7465 7374 2f69  ols/api/latest/i
+000009e0: 6e64 6578 2e68 746d 6c29 2e0a 0a23 2320  ndex.html)...## 
+000009f0: 4765 7474 696e 6720 5374 6172 7465 640a  Getting Started.
+00000a00: 0a23 2323 2050 7974 686f 6e20 7365 7475  .### Python setu
+00000a10: 700a 0a52 6571 7569 7265 7320 616e 2069  p..Requires an i
+00000a20: 6e73 7461 6c6c 6174 696f 6e20 6f66 2050  nstallation of P
+00000a30: 7974 686f 6e20 332e 372b 2e0a 0a57 6520  ython 3.7+...We 
+00000a40: 7265 636f 6d6d 656e 6420 7573 696e 6720  recommend using 
+00000a50: 6120 5079 7468 6f6e 2076 6972 7475 616c  a Python virtual
+00000a60: 2065 6e76 6972 6f6e 6d65 6e74 206d 616e   environment man
+00000a70: 6167 6572 2073 7563 6820 6173 2070 6970  ager such as pip
+00000a80: 656e 762c 2063 6f6e 6461 206f 7220 7669  env, conda or vi
+00000a90: 7274 7561 6c65 6e76 2e0a 0a54 6865 7365  rtualenv...These
+00000aa0: 2074 6173 6b73 2061 7265 2064 6573 6967   tasks are desig
+00000ab0: 6e65 6420 746f 2077 6f72 6b20 7769 7468  ned to work with
+00000ac0: 2050 7265 6665 6374 2032 2e20 466f 7220   Prefect 2. For 
+00000ad0: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
+00000ae0: 2061 626f 7574 2068 6f77 2074 6f20 7573   about how to us
+00000af0: 6520 5072 6566 6563 742c 2070 6c65 6173  e Prefect, pleas
+00000b00: 6520 7265 6665 7220 746f 2074 6865 205b  e refer to the [
+00000b10: 5072 6566 6563 7420 646f 6375 6d65 6e74  Prefect document
+00000b20: 6174 696f 6e5d 2868 7474 7073 3a2f 2f6f  ation](https://o
+00000b30: 7269 6f6e 2d64 6f63 732e 7072 6566 6563  rion-docs.prefec
+00000b40: 742e 696f 2f29 2e0a 0a23 2323 2049 6e73  t.io/)...### Ins
+00000b50: 7461 6c6c 6174 696f 6e0a 0a49 6e73 7461  tallation..Insta
+00000b60: 6c6c 2060 7072 6566 6563 742d 6461 7461  ll `prefect-data
+00000b70: 6272 6963 6b73 6020 7769 7468 2060 7069  bricks` with `pi
+00000b80: 7060 3a0a 0a60 6060 6261 7368 0a70 6970  p`:..```bash.pip
+00000b90: 2069 6e73 7461 6c6c 2070 7265 6665 6374   install prefect
+00000ba0: 2d64 6174 6162 7269 636b 730a 6060 600a  -databricks.```.
+00000bb0: 0a41 206c 6973 7420 6f66 2061 7661 696c  .A list of avail
+00000bc0: 6162 6c65 2062 6c6f 636b 7320 696e 2060  able blocks in `
+00000bd0: 7072 6566 6563 742d 6461 7461 6272 6963  prefect-databric
+00000be0: 6b73 6020 616e 6420 7468 6569 7220 7365  ks` and their se
+00000bf0: 7475 7020 696e 7374 7275 6374 696f 6e73  tup instructions
+00000c00: 2063 616e 2062 6520 666f 756e 6420 5b68   can be found [h
+00000c10: 6572 655d 2868 7474 7073 3a2f 2f50 7265  ere](https://Pre
+00000c20: 6665 6374 4851 2e67 6974 6875 622e 696f  fectHQ.github.io
+00000c30: 2f70 7265 6665 6374 2d64 6174 6162 7269  /prefect-databri
+00000c40: 636b 732f 2362 6c6f 636b 732d 6361 7461  cks/#blocks-cata
+00000c50: 6c6f 6729 2e0a 0a23 2323 204c 6973 7473  log)...### Lists
+00000c60: 206a 6f62 7320 6f6e 2074 6865 2044 6174   jobs on the Dat
+00000c70: 6162 7269 636b 7320 696e 7374 616e 6365  abricks instance
+00000c80: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+00000c90: 2070 7265 6665 6374 2069 6d70 6f72 7420   prefect import 
+00000ca0: 666c 6f77 0a66 726f 6d20 7072 6566 6563  flow.from prefec
+00000cb0: 745f 6461 7461 6272 6963 6b73 2069 6d70  t_databricks imp
+00000cc0: 6f72 7420 4461 7461 6272 6963 6b73 4372  ort DatabricksCr
+00000cd0: 6564 656e 7469 616c 730a 6672 6f6d 2070  edentials.from p
+00000ce0: 7265 6665 6374 5f64 6174 6162 7269 636b  refect_databrick
+00000cf0: 732e 6a6f 6273 2069 6d70 6f72 7420 6a6f  s.jobs import jo
+00000d00: 6273 5f6c 6973 740a 0a0a 4066 6c6f 770a  bs_list...@flow.
+00000d10: 6465 6620 6578 616d 706c 655f 6578 6563  def example_exec
+00000d20: 7574 655f 656e 6470 6f69 6e74 5f66 6c6f  ute_endpoint_flo
+00000d30: 7728 293a 0a20 2020 2064 6174 6162 7269  w():.    databri
+00000d40: 636b 735f 6372 6564 656e 7469 616c 7320  cks_credentials 
+00000d50: 3d20 4461 7461 6272 6963 6b73 4372 6564  = DatabricksCred
+00000d60: 656e 7469 616c 732e 6c6f 6164 2822 6d79  entials.load("my
+00000d70: 2d62 6c6f 636b 2229 0a20 2020 206a 6f62  -block").    job
+00000d80: 7320 3d20 6a6f 6273 5f6c 6973 7428 0a20  s = jobs_list(. 
+00000d90: 2020 2020 2020 2064 6174 6162 7269 636b         databrick
+00000da0: 735f 6372 6564 656e 7469 616c 732c 0a20  s_credentials,. 
+00000db0: 2020 2020 2020 206c 696d 6974 3d35 0a20         limit=5. 
+00000dc0: 2020 2029 0a20 2020 2072 6574 7572 6e20     ).    return 
+00000dd0: 6a6f 6273 0a0a 6578 616d 706c 655f 6578  jobs..example_ex
+00000de0: 6563 7574 655f 656e 6470 6f69 6e74 5f66  ecute_endpoint_f
+00000df0: 6c6f 7728 290a 6060 600a 0a23 2323 2055  low().```..### U
+00000e00: 7365 2060 7769 7468 5f6f 7074 696f 6e73  se `with_options
+00000e10: 6020 746f 2063 7573 746f 6d69 7a65 206f  ` to customize o
+00000e20: 7074 696f 6e73 206f 6e20 616e 7920 6578  ptions on any ex
+00000e30: 6973 7469 6e67 2074 6173 6b20 6f72 2066  isting task or f
+00000e40: 6c6f 770a 0a60 6060 7079 7468 6f6e 0a63  low..```python.c
+00000e50: 7573 746f 6d5f 6578 616d 706c 655f 6578  ustom_example_ex
+00000e60: 6563 7574 655f 656e 6470 6f69 6e74 5f66  ecute_endpoint_f
+00000e70: 6c6f 7720 3d20 6578 616d 706c 655f 6578  low = example_ex
+00000e80: 6563 7574 655f 656e 6470 6f69 6e74 5f66  ecute_endpoint_f
+00000e90: 6c6f 772e 7769 7468 5f6f 7074 696f 6e73  low.with_options
+00000ea0: 280a 2020 2020 6e61 6d65 3d22 4d79 2063  (.    name="My c
+00000eb0: 7573 746f 6d20 666c 6f77 206e 616d 6522  ustom flow name"
+00000ec0: 2c0a 2020 2020 7265 7472 6965 733d 322c  ,.    retries=2,
+00000ed0: 0a20 2020 2072 6574 7279 5f64 656c 6179  .    retry_delay
+00000ee0: 5f73 6563 6f6e 6473 3d31 302c 0a29 0a60  _seconds=10,.).`
+00000ef0: 6060 0a0a 2323 2320 4c61 756e 6368 2061  ``..### Launch a
+00000f00: 206e 6577 2063 6c75 7374 6572 2061 6e64   new cluster and
+00000f10: 2072 756e 2061 2044 6174 6162 7269 636b   run a Databrick
+00000f20: 7320 6e6f 7465 626f 6f6b 0a0a 4e6f 7465  s notebook..Note
+00000f30: 626f 6f6b 206e 616d 6564 2060 6578 616d  book named `exam
+00000f40: 706c 652e 6970 796e 6260 206f 6e20 4461  ple.ipynb` on Da
+00000f50: 7461 6272 6963 6b73 2077 6869 6368 2061  tabricks which a
+00000f60: 6363 6570 7473 2061 206e 616d 6520 7061  ccepts a name pa
+00000f70: 7261 6d65 7465 723a 0a0a 6060 6070 7974  rameter:..```pyt
+00000f80: 686f 6e0a 6e61 6d65 203d 2064 6275 7469  hon.name = dbuti
+00000f90: 6c73 2e77 6964 6765 7473 2e67 6574 2822  ls.widgets.get("
+00000fa0: 6e61 6d65 2229 0a6d 6573 7361 6765 203d  name").message =
+00000fb0: 2066 2244 6f6e 2774 2077 6f72 7279 207b   f"Don't worry {
+00000fc0: 6e61 6d65 7d2c 2049 2067 6f74 2079 6f75  name}, I got you
+00000fd0: 7220 7265 7175 6573 7421 2057 656c 636f  r request! Welco
+00000fe0: 6d65 2074 6f20 7072 6566 6563 742d 6461  me to prefect-da
+00000ff0: 7461 6272 6963 6b73 2122 0a70 7269 6e74  tabricks!".print
+00001000: 286d 6573 7361 6765 290a 6060 600a 0a50  (message).```..P
+00001010: 7265 6665 6374 2066 6c6f 7720 7468 6174  refect flow that
+00001020: 206c 6175 6e63 6865 7320 6120 6e65 7720   launches a new 
+00001030: 636c 7573 7465 7220 746f 2072 756e 2060  cluster to run `
+00001040: 6578 616d 706c 652e 6970 796e 6260 3a0a  example.ipynb`:.
+00001050: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
+00001060: 7072 6566 6563 7420 696d 706f 7274 2066  prefect import f
+00001070: 6c6f 770a 6672 6f6d 2070 7265 6665 6374  low.from prefect
+00001080: 5f64 6174 6162 7269 636b 7320 696d 706f  _databricks impo
+00001090: 7274 2044 6174 6162 7269 636b 7343 7265  rt DatabricksCre
+000010a0: 6465 6e74 6961 6c73 0a66 726f 6d20 7072  dentials.from pr
+000010b0: 6566 6563 745f 6461 7461 6272 6963 6b73  efect_databricks
+000010c0: 2e6a 6f62 7320 696d 706f 7274 206a 6f62  .jobs import job
+000010d0: 735f 7275 6e73 5f73 7562 6d69 740a 6672  s_runs_submit.fr
+000010e0: 6f6d 2070 7265 6665 6374 5f64 6174 6162  om prefect_datab
+000010f0: 7269 636b 732e 6d6f 6465 6c73 2e6a 6f62  ricks.models.job
+00001100: 7320 696d 706f 7274 2028 0a20 2020 2041  s import (.    A
+00001110: 7574 6f53 6361 6c65 2c0a 2020 2020 4177  utoScale,.    Aw
+00001120: 7341 7474 7269 6275 7465 732c 0a20 2020  sAttributes,.   
+00001130: 204a 6f62 5461 736b 5365 7474 696e 6773   JobTaskSettings
+00001140: 2c0a 2020 2020 4e6f 7465 626f 6f6b 5461  ,.    NotebookTa
+00001150: 736b 2c0a 2020 2020 4e65 7743 6c75 7374  sk,.    NewClust
+00001160: 6572 2c0a 290a 0a0a 4066 6c6f 770a 6465  er,.)...@flow.de
+00001170: 6620 6a6f 6273 5f72 756e 735f 7375 626d  f jobs_runs_subm
+00001180: 6974 5f66 6c6f 7728 6e6f 7465 626f 6f6b  it_flow(notebook
+00001190: 5f70 6174 682c 202a 2a62 6173 655f 7061  _path, **base_pa
+000011a0: 7261 6d65 7465 7273 293a 0a20 2020 2064  rameters):.    d
+000011b0: 6174 6162 7269 636b 735f 6372 6564 656e  atabricks_creden
+000011c0: 7469 616c 7320 3d20 4461 7461 6272 6963  tials = Databric
+000011d0: 6b73 4372 6564 656e 7469 616c 732e 6c6f  ksCredentials.lo
+000011e0: 6164 2822 6d79 2d62 6c6f 636b 2229 0a0a  ad("my-block")..
+000011f0: 2020 2020 2320 7370 6563 6966 7920 6e65      # specify ne
+00001200: 7720 636c 7573 7465 7220 7365 7474 696e  w cluster settin
+00001210: 6773 0a20 2020 2061 7773 5f61 7474 7269  gs.    aws_attri
+00001220: 6275 7465 7320 3d20 4177 7341 7474 7269  butes = AwsAttri
+00001230: 6275 7465 7328 0a20 2020 2020 2020 2061  butes(.        a
+00001240: 7661 696c 6162 696c 6974 793d 2253 504f  vailability="SPO
+00001250: 5422 2c0a 2020 2020 2020 2020 7a6f 6e65  T",.        zone
+00001260: 5f69 643d 2275 732d 7765 7374 2d32 6122  _id="us-west-2a"
+00001270: 2c0a 2020 2020 2020 2020 6562 735f 766f  ,.        ebs_vo
+00001280: 6c75 6d65 5f74 7970 653d 2247 454e 4552  lume_type="GENER
+00001290: 414c 5f50 5552 504f 5345 5f53 5344 222c  AL_PURPOSE_SSD",
+000012a0: 0a20 2020 2020 2020 2065 6273 5f76 6f6c  .        ebs_vol
+000012b0: 756d 655f 636f 756e 743d 332c 0a20 2020  ume_count=3,.   
+000012c0: 2020 2020 2065 6273 5f76 6f6c 756d 655f       ebs_volume_
+000012d0: 7369 7a65 3d31 3030 2c0a 2020 2020 290a  size=100,.    ).
+000012e0: 2020 2020 6175 746f 5f73 6361 6c65 203d      auto_scale =
+000012f0: 2041 7574 6f53 6361 6c65 286d 696e 5f77   AutoScale(min_w
+00001300: 6f72 6b65 7273 3d31 2c20 6d61 785f 776f  orkers=1, max_wo
+00001310: 726b 6572 733d 3229 0a20 2020 206e 6577  rkers=2).    new
+00001320: 5f63 6c75 7374 6572 203d 204e 6577 436c  _cluster = NewCl
+00001330: 7573 7465 7228 0a20 2020 2020 2020 2061  uster(.        a
+00001340: 7773 5f61 7474 7269 6275 7465 733d 6177  ws_attributes=aw
+00001350: 735f 6174 7472 6962 7574 6573 2c0a 2020  s_attributes,.  
+00001360: 2020 2020 2020 6175 746f 7363 616c 653d        autoscale=
+00001370: 6175 746f 5f73 6361 6c65 2c0a 2020 2020  auto_scale,.    
+00001380: 2020 2020 6e6f 6465 5f74 7970 655f 6964      node_type_id
+00001390: 3d22 6d34 2e6c 6172 6765 222c 0a20 2020  ="m4.large",.   
+000013a0: 2020 2020 2073 7061 726b 5f76 6572 7369       spark_versi
+000013b0: 6f6e 3d22 3130 2e34 2e78 2d73 6361 6c61  on="10.4.x-scala
+000013c0: 322e 3132 222c 0a20 2020 2020 2020 2073  2.12",.        s
+000013d0: 7061 726b 5f63 6f6e 663d 7b22 7370 6172  park_conf={"spar
+000013e0: 6b2e 7370 6563 756c 6174 696f 6e22 3a20  k.speculation": 
+000013f0: 5472 7565 7d2c 0a20 2020 2029 0a0a 2020  True},.    )..  
+00001400: 2020 2320 7370 6563 6966 7920 6e6f 7465    # specify note
+00001410: 626f 6f6b 2074 6f20 7573 6520 616e 6420  book to use and 
+00001420: 7061 7261 6d65 7465 7273 2074 6f20 7061  parameters to pa
+00001430: 7373 0a20 2020 206e 6f74 6562 6f6f 6b5f  ss.    notebook_
+00001440: 7461 736b 203d 204e 6f74 6562 6f6f 6b54  task = NotebookT
+00001450: 6173 6b28 0a20 2020 2020 2020 206e 6f74  ask(.        not
+00001460: 6562 6f6f 6b5f 7061 7468 3d6e 6f74 6562  ebook_path=noteb
+00001470: 6f6f 6b5f 7061 7468 2c0a 2020 2020 2020  ook_path,.      
+00001480: 2020 6261 7365 5f70 6172 616d 6574 6572    base_parameter
+00001490: 733d 6261 7365 5f70 6172 616d 6574 6572  s=base_parameter
+000014a0: 732c 0a20 2020 2029 0a0a 2020 2020 2320  s,.    )..    # 
+000014b0: 636f 6d70 696c 6520 6a6f 6220 7461 736b  compile job task
+000014c0: 2073 6574 7469 6e67 730a 2020 2020 6a6f   settings.    jo
+000014d0: 625f 7461 736b 5f73 6574 7469 6e67 7320  b_task_settings 
+000014e0: 3d20 4a6f 6254 6173 6b53 6574 7469 6e67  = JobTaskSetting
+000014f0: 7328 0a20 2020 2020 2020 206e 6577 5f63  s(.        new_c
+00001500: 6c75 7374 6572 3d6e 6577 5f63 6c75 7374  luster=new_clust
+00001510: 6572 2c0a 2020 2020 2020 2020 6e6f 7465  er,.        note
+00001520: 626f 6f6b 5f74 6173 6b3d 6e6f 7465 626f  book_task=notebo
+00001530: 6f6b 5f74 6173 6b2c 0a20 2020 2020 2020  ok_task,.       
+00001540: 2074 6173 6b5f 6b65 793d 2270 7265 6665   task_key="prefe
+00001550: 6374 2d74 6173 6b22 0a20 2020 2029 0a0a  ct-task".    )..
+00001560: 2020 2020 7275 6e20 3d20 6a6f 6273 5f72      run = jobs_r
+00001570: 756e 735f 7375 626d 6974 280a 2020 2020  uns_submit(.    
+00001580: 2020 2020 6461 7461 6272 6963 6b73 5f63      databricks_c
+00001590: 7265 6465 6e74 6961 6c73 3d64 6174 6162  redentials=datab
+000015a0: 7269 636b 735f 6372 6564 656e 7469 616c  ricks_credential
+000015b0: 732c 0a20 2020 2020 2020 2072 756e 5f6e  s,.        run_n
+000015c0: 616d 653d 2270 7265 6665 6374 2d6a 6f62  ame="prefect-job
+000015d0: 222c 0a20 2020 2020 2020 2074 6173 6b73  ",.        tasks
+000015e0: 3d5b 6a6f 625f 7461 736b 5f73 6574 7469  =[job_task_setti
+000015f0: 6e67 735d 0a20 2020 2029 0a0a 2020 2020  ngs].    )..    
+00001600: 7265 7475 726e 2072 756e 0a0a 0a6a 6f62  return run...job
+00001610: 735f 7275 6e73 5f73 7562 6d69 745f 666c  s_runs_submit_fl
+00001620: 6f77 2822 2f55 7365 7273 2f75 7365 726e  ow("/Users/usern
+00001630: 616d 6540 676d 6169 6c2e 636f 6d2f 6578  ame@gmail.com/ex
+00001640: 616d 706c 652e 6970 796e 6222 2c20 6e61  ample.ipynb", na
+00001650: 6d65 3d22 4d61 7276 696e 2229 0a60 6060  me="Marvin").```
+00001660: 0a0a 4e6f 7465 2c20 696e 7374 6561 6420  ..Note, instead 
+00001670: 6f66 2075 7369 6e67 2074 6865 2062 7569  of using the bui
+00001680: 6c74 2d69 6e20 6d6f 6465 6c73 2c20 796f  lt-in models, yo
+00001690: 7520 6d61 7920 616c 736f 2069 6e70 7574  u may also input
+000016a0: 2076 616c 6964 204a 534f 4e2e 2046 6f72   valid JSON. For
+000016b0: 2065 7861 6d70 6c65 2c20 6041 7574 6f53   example, `AutoS
+000016c0: 6361 6c65 286d 696e 5f77 6f72 6b65 7273  cale(min_workers
+000016d0: 3d31 2c20 6d61 785f 776f 726b 6572 733d  =1, max_workers=
+000016e0: 3229 6020 6973 2065 7175 6976 616c 656e  2)` is equivalen
+000016f0: 7420 746f 2060 7b22 6d69 6e5f 776f 726b  t to `{"min_work
+00001700: 6572 7322 3a20 312c 2022 6d61 785f 776f  ers": 1, "max_wo
+00001710: 726b 6572 7322 3a20 327d 602e 0a0a 466f  rkers": 2}`...Fo
+00001720: 7220 6d6f 7265 2074 6970 7320 6f6e 2068  r more tips on h
+00001730: 6f77 2074 6f20 7573 6520 7461 736b 7320  ow to use tasks 
+00001740: 616e 6420 666c 6f77 7320 696e 2061 2043  and flows in a C
+00001750: 6f6c 6c65 6374 696f 6e2c 2063 6865 636b  ollection, check
+00001760: 206f 7574 205b 5573 696e 6720 436f 6c6c   out [Using Coll
+00001770: 6563 7469 6f6e 735d 2868 7474 7073 3a2f  ections](https:/
+00001780: 2f6f 7269 6f6e 2d64 6f63 732e 7072 6566  /orion-docs.pref
+00001790: 6563 742e 696f 2f63 6f6c 6c65 6374 696f  ect.io/collectio
+000017a0: 6e73 2f75 7361 6765 2f29 210a 0a23 2320  ns/usage/)!..## 
+000017b0: 5265 736f 7572 6365 730a 0a49 6620 796f  Resources..If yo
+000017c0: 7520 656e 636f 756e 7465 7220 616e 7920  u encounter any 
+000017d0: 6275 6773 2077 6869 6c65 2075 7369 6e67  bugs while using
+000017e0: 2060 7072 6566 6563 742d 6461 7461 6272   `prefect-databr
+000017f0: 6963 6b73 602c 2066 6565 6c20 6672 6565  icks`, feel free
+00001800: 2074 6f20 6f70 656e 2061 6e20 6973 7375   to open an issu
+00001810: 6520 696e 2074 6865 205b 7072 6566 6563  e in the [prefec
+00001820: 742d 6461 7461 6272 6963 6b73 5d28 6874  t-databricks](ht
+00001830: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001840: 2f50 7265 6665 6374 4851 2f70 7265 6665  /PrefectHQ/prefe
+00001850: 6374 2d64 6174 6162 7269 636b 7329 2072  ct-databricks) r
+00001860: 6570 6f73 6974 6f72 792e 0a0a 4966 2079  epository...If y
+00001870: 6f75 2068 6176 6520 616e 7920 7175 6573  ou have any ques
+00001880: 7469 6f6e 7320 6f72 2069 7373 7565 7320  tions or issues 
+00001890: 7768 696c 6520 7573 696e 6720 6070 7265  while using `pre
+000018a0: 6665 6374 2d64 6174 6162 7269 636b 7360  fect-databricks`
+000018b0: 2c20 796f 7520 6361 6e20 6669 6e64 2068  , you can find h
+000018c0: 656c 7020 696e 2065 6974 6865 7220 7468  elp in either th
+000018d0: 6520 5b50 7265 6665 6374 2044 6973 636f  e [Prefect Disco
+000018e0: 7572 7365 2066 6f72 756d 5d28 6874 7470  urse forum](http
+000018f0: 733a 2f2f 6469 7363 6f75 7273 652e 7072  s://discourse.pr
+00001900: 6566 6563 742e 696f 2f29 206f 7220 7468  efect.io/) or th
+00001910: 6520 5b50 7265 6665 6374 2053 6c61 636b  e [Prefect Slack
+00001920: 2063 6f6d 6d75 6e69 7479 5d28 6874 7470   community](http
+00001930: 733a 2f2f 7072 6566 6563 742e 696f 2f73  s://prefect.io/s
+00001940: 6c61 636b 292e 0a0a 4665 656c 2066 7265  lack)...Feel fre
+00001950: 6520 746f 2073 7461 7220 6f72 2077 6174  e to star or wat
+00001960: 6368 205b 6070 7265 6665 6374 2d64 6174  ch [`prefect-dat
+00001970: 6162 7269 636b 7360 5d28 6874 7470 733a  abricks`](https:
+00001980: 2f2f 6769 7468 7562 2e63 6f6d 2f50 7265  //github.com/Pre
+00001990: 6665 6374 4851 2f70 7265 6665 6374 2d64  fectHQ/prefect-d
+000019a0: 6174 6162 7269 636b 7329 2066 6f72 2075  atabricks) for u
+000019b0: 7064 6174 6573 2074 6f6f 210a 0a23 2320  pdates too!..## 
+000019c0: 436f 6e74 7269 6275 7469 6e67 0a0a 4966  Contributing..If
+000019d0: 2079 6f75 2764 206c 696b 6520 746f 2068   you'd like to h
+000019e0: 656c 7020 636f 6e74 7269 6275 7465 2074  elp contribute t
+000019f0: 6f20 6669 7820 616e 2069 7373 7565 206f  o fix an issue o
+00001a00: 7220 6164 6420 6120 6665 6174 7572 6520  r add a feature 
+00001a10: 746f 2060 7072 6566 6563 742d 6461 7461  to `prefect-data
+00001a20: 6272 6963 6b73 602c 2070 6c65 6173 6520  bricks`, please 
+00001a30: 5b70 726f 706f 7365 2063 6861 6e67 6573  [propose changes
+00001a40: 2074 6872 6f75 6768 2061 2070 756c 6c20   through a pull 
+00001a50: 7265 7175 6573 7420 6672 6f6d 2061 2066  request from a f
+00001a60: 6f72 6b20 6f66 2074 6865 2072 6570 6f73  ork of the repos
+00001a70: 6974 6f72 795d 2868 7474 7073 3a2f 2f64  itory](https://d
+00001a80: 6f63 732e 6769 7468 7562 2e63 6f6d 2f65  ocs.github.com/e
+00001a90: 6e2f 7075 6c6c 2d72 6571 7565 7374 732f  n/pull-requests/
+00001aa0: 636f 6c6c 6162 6f72 6174 696e 672d 7769  collaborating-wi
+00001ab0: 7468 2d70 756c 6c2d 7265 7175 6573 7473  th-pull-requests
+00001ac0: 2f70 726f 706f 7369 6e67 2d63 6861 6e67  /proposing-chang
+00001ad0: 6573 2d74 6f2d 796f 7572 2d77 6f72 6b2d  es-to-your-work-
+00001ae0: 7769 7468 2d70 756c 6c2d 7265 7175 6573  with-pull-reques
+00001af0: 7473 2f63 7265 6174 696e 672d 612d 7075  ts/creating-a-pu
+00001b00: 6c6c 2d72 6571 7565 7374 2d66 726f 6d2d  ll-request-from-
+00001b10: 612d 666f 726b 292e 0a0a 4865 7265 2061  a-fork)...Here a
+00001b20: 7265 2074 6865 2073 7465 7073 3a0a 312e  re the steps:.1.
+00001b30: 205b 466f 726b 2074 6865 2072 6570 6f73   [Fork the repos
+00001b40: 6974 6f72 795d 2868 7474 7073 3a2f 2f64  itory](https://d
+00001b50: 6f63 732e 6769 7468 7562 2e63 6f6d 2f65  ocs.github.com/e
+00001b60: 6e2f 6765 742d 7374 6172 7465 642f 7175  n/get-started/qu
+00001b70: 6963 6b73 7461 7274 2f66 6f72 6b2d 612d  ickstart/fork-a-
+00001b80: 7265 706f 2366 6f72 6b69 6e67 2d61 2d72  repo#forking-a-r
+00001b90: 6570 6f73 6974 6f72 7929 0a32 2e20 5b43  epository).2. [C
+00001ba0: 6c6f 6e65 2074 6865 2066 6f72 6b65 6420  lone the forked 
+00001bb0: 7265 706f 7369 746f 7279 5d28 6874 7470  repository](http
+00001bc0: 733a 2f2f 646f 6373 2e67 6974 6875 622e  s://docs.github.
+00001bd0: 636f 6d2f 656e 2f67 6574 2d73 7461 7274  com/en/get-start
+00001be0: 6564 2f71 7569 636b 7374 6172 742f 666f  ed/quickstart/fo
+00001bf0: 726b 2d61 2d72 6570 6f23 636c 6f6e 696e  rk-a-repo#clonin
+00001c00: 672d 796f 7572 2d66 6f72 6b65 642d 7265  g-your-forked-re
+00001c10: 706f 7369 746f 7279 290a 332e 2049 6e73  pository).3. Ins
+00001c20: 7461 6c6c 2074 6865 2072 6570 6f73 6974  tall the reposit
+00001c30: 6f72 7920 616e 6420 6974 7320 6465 7065  ory and its depe
+00001c40: 6e64 656e 6369 6573 3a0a 6060 600a 7069  ndencies:.```.pi
+00001c50: 7020 696e 7374 616c 6c20 2d65 2022 2e5b  p install -e ".[
+00001c60: 6465 765d 220a 6060 600a 342e 204d 616b  dev]".```.4. Mak
+00001c70: 6520 6465 7369 7265 6420 6368 616e 6765  e desired change
+00001c80: 730a 352e 2041 6464 2074 6573 7473 0a36  s.5. Add tests.6
+00001c90: 2e20 496e 7365 7274 2061 6e20 656e 7472  . Insert an entr
+00001ca0: 7920 746f 205b 4348 414e 4745 4c4f 472e  y to [CHANGELOG.
+00001cb0: 6d64 5d28 6874 7470 733a 2f2f 6769 7468  md](https://gith
+00001cc0: 7562 2e63 6f6d 2f50 7265 6665 6374 4851  ub.com/PrefectHQ
+00001cd0: 2f70 7265 6665 6374 2d64 6174 6162 7269  /prefect-databri
+00001ce0: 636b 732f 626c 6f62 2f6d 6169 6e2f 4348  cks/blob/main/CH
+00001cf0: 414e 4745 4c4f 472e 6d64 290a 372e 2049  ANGELOG.md).7. I
+00001d00: 6e73 7461 6c6c 2060 7072 652d 636f 6d6d  nstall `pre-comm
+00001d10: 6974 6020 746f 2070 6572 666f 726d 2071  it` to perform q
+00001d20: 7561 6c69 7479 2063 6865 636b 7320 7072  uality checks pr
+00001d30: 696f 7220 746f 2063 6f6d 6d69 743a 0a60  ior to commit:.`
+00001d40: 6060 0a70 7265 2d63 6f6d 6d69 7420 696e  ``.pre-commit in
+00001d50: 7374 616c 6c0a 6060 600a 382e 2060 6769  stall.```.8. `gi
+00001d60: 7420 636f 6d6d 6974 602c 2060 6769 7420  t commit`, `git 
+00001d70: 7075 7368 602c 2061 6e64 2063 7265 6174  push`, and creat
+00001d80: 6520 6120 7075 6c6c 2072 6571 7565 7374  e a pull request
+00001d90: 0a                                       .
```

### Comparing `prefect-databricks-0.2.3/prefect_databricks/credentials.py` & `prefect_databricks-0.2.4/prefect_databricks/credentials.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Credential classes used to perform authenticated interactions with Databricks"""
 
 from typing import Any, Dict, Optional
 
 from httpx import AsyncClient
-from prefect.blocks.core import Block
-from pydantic import VERSION as PYDANTIC_VERSION
 
-if PYDANTIC_VERSION.startswith("2."):
+from prefect._internal.pydantic import HAS_PYDANTIC_V2
+
+if HAS_PYDANTIC_V2:
     from pydantic.v1 import Field, SecretStr
 else:
     from pydantic import Field, SecretStr
 
+from prefect.blocks.core import Block
+
 
 class DatabricksCredentials(Block):
     """
     Block used to manage Databricks authentication.
 
     Attributes:
         databricks_instance:
@@ -27,16 +29,15 @@
         ```python
         from prefect_databricks import DatabricksCredentials
         databricks_credentials_block = DatabricksCredentials.load("BLOCK_NAME")
         ```
     """
 
     _block_type_name = "Databricks Credentials"
-    _logo_url = "https://cdn.sanity.io/images/3ugk85nk/production/ff9a2573c23954bedd27b0f420465a55b1a99dfd-250x250.png"  # noqa
-    _documentation_url = "https://prefecthq.github.io/prefect-databricks/credentials/#prefect_databricks.credentials.DatabricksCredentials"  # noqa
+    _logo_url = "https://images.ctfassets.net/gm98wzqotmnx/5GTHI1PH2dTiantfps6Fnc/1c750fab7f4c14ea1b93a62b9fea6a94/databricks_logo_icon_170295.png?h=250"  # noqa
 
     databricks_instance: str = Field(
         default=...,
         description="Databricks instance used in formatting the endpoint URL.",
     )
     token: SecretStr = Field(
         default=..., description="The token to authenticate with Databricks."
```

### Comparing `prefect-databricks-0.2.3/prefect_databricks/flows.py` & `prefect_databricks-0.2.4/prefect_databricks/flows.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """
 Module containing flows for interacting with Databricks
 """
 
 import asyncio
-import inspect
 from logging import Logger
-from typing import Any, Callable, Dict, List, Optional
+from typing import Any, Dict, List, Optional
 
 from prefect import flow, get_run_logger
-
 from prefect_databricks import DatabricksCredentials
 from prefect_databricks.jobs import (
-    jobs_run_now,
     jobs_runs_get,
     jobs_runs_get_output,
     jobs_runs_submit,
 )
 from prefect_databricks.models.jobs import (
     AccessControlRequest,
     GitSource,
@@ -64,19 +61,19 @@
     run_name: Optional[str] = None,
     max_wait_seconds: int = 900,
     poll_frequency_seconds: int = 10,
     git_source: Optional[GitSource] = None,
     timeout_seconds: Optional[int] = None,
     idempotency_token: Optional[str] = None,
     access_control_list: Optional[List[AccessControlRequest]] = None,
-    job_submission_handler: Optional[Callable] = None,
     **jobs_runs_submit_kwargs: Dict[str, Any],
 ) -> Dict:
     """
     Flow that triggers a job run and waits for the triggered run to complete.
+
     Args:
         databricks_credentials:
             Credentials to use for authentication with Databricks.
         tasks: Tasks to run, e.g.
             ```
             [
                 {
@@ -177,34 +174,37 @@
             jobs](https://kb.databricks.com/jobs/jobs-idempotency.html),
             e.g. `8f018174-4792-40d5-bcbc-3e6a527352c8`.
         access_control_list:
             List of permissions to set on the job.
         max_wait_seconds: Maximum number of seconds to wait for the entire flow to complete.
         poll_frequency_seconds: Number of seconds to wait in between checks for
             run completion.
-        job_submission_handler: An optional callable to intercept job submission
         **jobs_runs_submit_kwargs: Additional keyword arguments to pass to `jobs_runs_submit`.
+
     Returns:
         A dictionary of task keys to its corresponding notebook output.
+
     Examples:
         Submit jobs runs and wait.
         ```python
         from prefect import flow
         from prefect_databricks import DatabricksCredentials
         from prefect_databricks.flows import jobs_runs_submit_and_wait_for_completion
         from prefect_databricks.models.jobs import (
             AutoScale,
             AwsAttributes,
             JobTaskSettings,
             NotebookTask,
             NewCluster,
         )
+
         @flow
         def jobs_runs_submit_and_wait_for_completion_flow(notebook_path, **base_parameters):
             databricks_credentials = await DatabricksCredentials.load("BLOCK_NAME")
+
             # specify new cluster settings
             aws_attributes = AwsAttributes(
                 availability="SPOT",
                 zone_id="us-west-2a",
                 ebs_volume_type="GENERAL_PURPOSE_SSD",
                 ebs_volume_count=3,
                 ebs_volume_size=100,
@@ -213,30 +213,34 @@
             new_cluster = NewCluster(
                 aws_attributes=aws_attributes,
                 autoscale=auto_scale,
                 node_type_id="m4.large",
                 spark_version="10.4.x-scala2.12",
                 spark_conf={"spark.speculation": True},
             )
+
             # specify notebook to use and parameters to pass
             notebook_task = NotebookTask(
                 notebook_path=notebook_path,
                 base_parameters=base_parameters,
             )
+
             # compile job task settings
             job_task_settings = JobTaskSettings(
                 new_cluster=new_cluster,
                 notebook_task=notebook_task,
                 task_key="prefect-task"
             )
+
             multi_task_runs = jobs_runs_submit_and_wait_for_completion(
                 databricks_credentials=databricks_credentials,
                 run_name="prefect-job",
                 tasks=[job_task_settings]
             )
+
             return multi_task_runs
         ```
     """  # noqa
     logger = get_run_logger()
 
     # submit the jobs runs
     multi_task_jobs_runs_future = await jobs_runs_submit.submit(
@@ -245,20 +249,15 @@
         run_name=run_name,
         git_source=git_source,
         timeout_seconds=timeout_seconds,
         idempotency_token=idempotency_token,
         access_control_list=access_control_list,
         **jobs_runs_submit_kwargs,
     )
-
     multi_task_jobs_runs = await multi_task_jobs_runs_future.result()
-    if job_submission_handler:
-        result = job_submission_handler(multi_task_jobs_runs)
-        if inspect.isawaitable(result):
-            await result
     multi_task_jobs_runs_id = multi_task_jobs_runs["run_id"]
 
     # wait for all the jobs runs to complete in a separate flow
     # for a cleaner radar interface
     jobs_runs_state, jobs_runs_metadata = await jobs_runs_wait_for_completion(
         multi_task_jobs_runs_id=multi_task_jobs_runs_id,
         databricks_credentials=databricks_credentials,
@@ -308,228 +307,14 @@
         raise DatabricksJobInternalError(
             f"Databricks Jobs Runs Submit ({run_name} ID "
             f"{multi_task_jobs_runs_id}) "
             f"encountered an internal error: {jobs_runs_state_message}.",
         )
 
 
-@flow(
-    name="Submit existing job runs and wait for completion",
-    description=(
-        "Triggers a Databricks jobs runs and waits for the "
-        "triggered runs to complete."
-    ),
-)
-async def jobs_runs_submit_by_id_and_wait_for_completion(
-    databricks_credentials: DatabricksCredentials,
-    job_id: int,
-    idempotency_token: Optional[str] = None,
-    jar_params: Optional[List[str]] = None,
-    max_wait_seconds: int = 900,
-    poll_frequency_seconds: int = 10,
-    notebook_params: Optional[Dict] = None,
-    python_params: Optional[List[str]] = None,
-    spark_submit_params: Optional[List[str]] = None,
-    python_named_params: Optional[Dict] = None,
-    pipeline_params: Optional[str] = None,
-    sql_params: Optional[Dict] = None,
-    dbt_commands: Optional[List] = None,
-    job_submission_handler: Optional[Callable] = None,
-    **jobs_runs_submit_kwargs: Dict[str, Any],
-) -> Dict:
-    """flow that triggers an existing job and waits for its completion
-
-    Args:
-        databricks_credentials: Credentials to use for authentication with Databricks.
-        job_id: Id of the databricks job.
-        idempotency_token:
-            An optional token that can be used to guarantee the idempotency of job
-            run requests. If a run with the provided token already
-            exists, the request does not create a new run but returns
-            the ID of the existing run instead. If a run with the
-            provided token is deleted, an error is returned.  If you
-            specify the idempotency token, upon failure you can retry
-            until the request succeeds. Databricks guarantees that
-            exactly one run is launched with that idempotency token.
-            This token must have at most 64 characters.  For more
-            information, see [How to ensure idempotency for
-            jobs](https://kb.databricks.com/jobs/jobs-idempotency.html),
-            e.g. `8f018174-4792-40d5-bcbc-3e6a527352c8`.
-        jar_params:
-            A list of parameters for jobs with Spark JAR tasks, for example "jar_params"
-            : ["john doe", "35"]. The parameters are used to invoke the main function of
-            the main class specified in the Spark JAR task. If not specified upon run-
-            now, it defaults to an empty list. jar_params cannot be specified in
-            conjunction with notebook_params. The JSON representation of this field (for
-            example {"jar_params": ["john doe","35"]}) cannot exceed 10,000 bytes.
-        max_wait_seconds:
-            Maximum number of seconds to wait for the entire flow to complete.
-        poll_frequency_seconds: Number of seconds to wait in between checks for
-            run completion.
-        notebook_params:
-            A map from keys to values for jobs with notebook task, for example
-            "notebook_params": {"name": "john doe", "age": "35"}. The map is
-            passed to the notebook and is accessible through the dbutils.widgets.get
-            function. If not specified upon run-now, the triggered run uses the job’s
-            base parameters. notebook_params cannot be specified in conjunction with
-            jar_params. Use Task parameter variables to set parameters containing
-            information about job runs. The JSON representation of this field
-            (for example {"notebook_params":{"name":"john doe","age":"35"}}) cannot
-            exceed 10,000 bytes.
-        python_params:
-            A list of parameters for jobs with Python tasks, for example "python_params"
-            :["john doe", "35"]. The parameters are passed to Python file as command-
-            line parameters. If specified upon run-now, it would overwrite the
-            parameters specified in job setting. The JSON representation of this field
-            (for example {"python_params":["john doe","35"]}) cannot exceed 10,000 bytes
-            Use Task parameter variables to set parameters containing information
-            about job runs. These parameters accept only Latin characters (ASCII
-            character set). Using non-ASCII characters returns an error. Examples of
-            invalid, non-ASCII characters are Chinese, Japanese kanjis, and emojis.
-        spark_submit_params:
-            A list of parameters for jobs with spark submit task, for example
-            "spark_submit_params": ["--class", "org.apache.spark.examples.SparkPi"].
-            The parameters are passed to spark-submit script as command-line parameters.
-            If specified upon run-now, it would overwrite the parameters specified in
-            job setting. The JSON representation of this field (for example
-            {"python_params":["john doe","35"]}) cannot exceed 10,000 bytes.
-            Use Task parameter variables to set parameters containing information about
-            job runs. These parameters accept only Latin characters (ASCII character
-            set). Using non-ASCII characters returns an error. Examples of invalid,
-            non-ASCII characters are Chinese, Japanese kanjis, and emojis.
-        python_named_params:
-            A map from keys to values for jobs with Python wheel task, for example
-            "python_named_params": {"name": "task", "data": "dbfs:/path/to/data.json"}.
-        pipeline_params:
-            If `full_refresh` is set to true, trigger a full refresh on the
-            delta live table e.g.
-            ```
-                "pipeline_params": {"full_refresh": true}
-            ```
-        sql_params:
-            A map from keys to values for SQL tasks, for example "sql_params":
-            {"name": "john doe", "age": "35"}. The SQL alert task does not support
-            custom parameters.
-        dbt_commands:
-            An array of commands to execute for jobs with the dbt task,
-            for example "dbt_commands": ["dbt deps", "dbt seed", "dbt run"]
-        job_submission_handler: An optional callable to intercept job submission
-
-    Raises:
-        DatabricksJobTerminated:
-            Raised when the Databricks job run is terminated with a non-successful
-            result state.
-        DatabricksJobSkipped: Raised when the Databricks job run is skipped.
-        DatabricksJobInternalError:
-            Raised when the Databricks job run encounters an internal error.
-
-    Returns:
-        Dict: A dictionary containing information about the completed job run.
-
-    Example:
-        ```python
-        from prefect import flow
-        from prefect_databricks import DatabricksCredentials
-        from prefect_databricks.flows import (
-            jobs_runs_submit_by_id_and_wait_for_completion,
-        )
-
-
-        @flow
-        def submit_existing_job(block_name: str, job_id):
-            databricks_credentials = DatabricksCredentials.load(block_name)
-
-            run = jobs_runs_submit_by_id_and_wait_for_completion(
-                databricks_credentials=databricks_credentials, job_id=job_id
-            )
-
-            return run
-
-
-        submit_existing_job(block_name="db-creds", job_id=db_job_id)
-        ```
-    """
-    logger = get_run_logger()
-
-    # submit the jobs runs
-
-    jobs_runs_future = await jobs_run_now.submit(
-        databricks_credentials=databricks_credentials,
-        job_id=job_id,
-        idempotency_token=idempotency_token,
-        jar_params=jar_params,
-        notebook_params=notebook_params,
-        python_params=python_params,
-        spark_submit_params=spark_submit_params,
-        python_named_params=python_named_params,
-        pipeline_params=pipeline_params,
-        sql_params=sql_params,
-        dbt_commands=dbt_commands,
-        **jobs_runs_submit_kwargs,
-    )
-
-    jobs_runs = await jobs_runs_future.result()
-
-    if job_submission_handler:
-        result = job_submission_handler(jobs_runs)
-        if inspect.isawaitable(result):
-            await result
-    job_run_id = jobs_runs["run_id"]
-
-    # wait for all the jobs runs to complete in a separate flow
-    # for a cleaner radar interface
-    jobs_runs_state, jobs_runs_metadata = await jobs_runs_wait_for_completion(
-        multi_task_jobs_runs_id=job_run_id,
-        databricks_credentials=databricks_credentials,
-        max_wait_seconds=max_wait_seconds,
-        poll_frequency_seconds=poll_frequency_seconds,
-    )
-
-    # fetch the state results
-    jobs_runs_life_cycle_state = jobs_runs_state["life_cycle_state"]
-    jobs_runs_state_message = jobs_runs_state["state_message"]
-
-    # return results or raise error
-    if jobs_runs_life_cycle_state == RunLifeCycleState.terminated.value:
-        jobs_runs_result_state = jobs_runs_state.get("result_state", None)
-        if jobs_runs_result_state == RunResultState.success.value:
-            task_notebook_outputs = {}
-            for task in jobs_runs_metadata["tasks"]:
-                task_key = task["task_key"]
-                task_run_id = task["run_id"]
-                task_run_output_future = await jobs_runs_get_output.submit(
-                    run_id=task_run_id,
-                    databricks_credentials=databricks_credentials,
-                )
-                task_run_output = await task_run_output_future.result()
-                task_run_notebook_output = task_run_output.get("notebook_output", {})
-                task_notebook_outputs[task_key] = task_run_notebook_output
-            logger.info(
-                f"Databricks Jobs Runs Submit {job_id} completed successfully!",
-            )
-            return task_notebook_outputs
-        else:
-            raise DatabricksJobTerminated(
-                f"Databricks Jobs Runs Submit ID {job_id} "
-                f"terminated with result state, {jobs_runs_result_state}: "
-                f"{jobs_runs_state_message}"
-            )
-    elif jobs_runs_life_cycle_state == RunLifeCycleState.skipped.value:
-        raise DatabricksJobSkipped(
-            f"Databricks Jobs Runs Submit ID "
-            f"{job_id} was skipped: {jobs_runs_state_message}.",
-        )
-    elif jobs_runs_life_cycle_state == RunLifeCycleState.internalerror.value:
-        raise DatabricksJobInternalError(
-            f"Databricks Jobs Runs Submit ID "
-            f"{job_id} "
-            f"encountered an internal error: {jobs_runs_state_message}.",
-        )
-
-
 def _update_and_log_state_changes(
     job_or_task_states: Dict[str, Any],
     job_or_task_metadata: Dict[str, Any],
     logger: Logger,
     run_type: str = "Task",
 ) -> Dict[str, Any]:
     """
@@ -541,14 +326,15 @@
         job_or_task_metadata: Metadata object containing run, url and state
         logger: Logger instance to log with.
         run_type: String indicating if is job or task, defaults to Task
 
     Returns
         A copy of the job_or_task_states dictionary with any state updates
     """
+
     run_id = job_or_task_metadata.get("run_id", "")
     run_page_url = job_or_task_metadata.get("run_page_url", "")
     state = job_or_task_metadata.get("state", {})
 
     string_run_id = str(run_id)
 
     job_or_task_states_copy = job_or_task_states.copy()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `prefect-databricks-0.2.3/prefect_databricks/jobs.py` & `prefect_databricks-0.2.4/prefect_databricks/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -780,15 +780,15 @@
     contents = _unpack_contents(response, responses)
     return contents
 
 
 @task
 async def jobs_run_now(
     databricks_credentials: "DatabricksCredentials",
-    job_id: int,
+    job_id: Optional[int] = None,
     idempotency_token: Optional[str] = None,
     jar_params: Optional[List[str]] = None,
     notebook_params: Optional[Dict] = None,
     python_params: Optional[List[str]] = None,
     spark_submit_params: Optional[List[str]] = None,
     python_named_params: Optional[Dict] = None,
     pipeline_params: Optional[str] = None,
@@ -890,19 +890,14 @@
             A map from keys to values for jobs with Python wheel task, for example
             `'python_named_params': {'name': 'task', 'data':
             'dbfs:/path/to/data.json'}`, e.g.
             ```
             {"name": "task", "data": "dbfs:/path/to/data.json"}
             ```
         pipeline_params:
-            If `full_refresh` is set to true, trigger a full refresh on the
-            delta live table e.g.
-            ```
-                "pipeline_params": {"full_refresh": true}
-            ```
 
         sql_params:
             A map from keys to values for SQL tasks, for example `'sql_params':
             {'name': 'john doe', 'age': '35'}`. The SQL alert task does
             not support custom parameters, e.g.
             ```
             {"name": "john doe", "age": "35"}
```

### Comparing `prefect-databricks-0.2.3/prefect_databricks/models/jobs.py` & `prefect_databricks-0.2.4/prefect_databricks/models/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 #   timestamp: 2022-12-10T01:04:37+00:00
 
 from __future__ import annotations
 
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
-from pydantic import VERSION as PYDANTIC_VERSION
+from prefect._internal.pydantic import HAS_PYDANTIC_V2
 
-if PYDANTIC_VERSION.startswith("2."):
+if HAS_PYDANTIC_V2:
     from pydantic.v1 import BaseModel, Extra, Field
 else:
     from pydantic import BaseModel, Extra, Field
 
 from typing_extensions import Literal
 
 
@@ -808,23 +808,14 @@
     * `ASC`: Ascending order.
     """
 
     desc = "DESC"
     asc = "ASC"
 
 
-class RuntimeEngine(str, Enum):
-    """
-    Decides which runtime engine to be use, e.g. Standard vs. Photon. If unspecified, the runtime engine is inferred from spark_version.
-    """
-
-    standard = "STANDARD"
-    photon = "PHOTON"
-
-
 class LogSyncStatus(BaseModel):
     """
     See source code for the fields' description.
     """
 
     class Config:
         extra = Extra.allow
@@ -1490,15 +1481,15 @@
     )
 
 
 class SparkConfPair(BaseModel):
     """
     See source code for the fields' description.
 
-    An arbitrary object where the object key is a configuration propery name and the value is a configuration property value.
+    An arbitrary object where the object key is a configuration property name and the value is a configuration property value.
     """
 
     class Config:
         extra = Extra.allow
 
         allow_mutation = False
 
@@ -2467,23 +2458,14 @@
         description=(
             "The Spark version of the cluster. A list of available Spark versions can"
             " be retrieved by using the [Runtime"
             " versions](https://docs.databricks.com/dev-tools/api/latest/clusters.html#runtime-versions)"
             " API call."
         ),
     )
-    runtime_engine: Optional[RuntimeEngine] = Field(
-        None,
-        description=(
-            "Decides which runtime engine to be use, e.g. Standard vs. Photon. If "
-            "unspecified, the runtime engine is inferred from spark_version. "
-            "see https://docs.databricks.com/api-explorer/workspace/jobs/create "
-            " for more details"
-        ),
-    )
     ssh_public_keys: Optional[List[str]] = Field(
         None,
         description=(
             "SSH public key contents that are added to each Spark node in this cluster."
             " The corresponding private keys can be used to login with the user name"
             " `ubuntu` on port `2200`. Up to 10 keys can be specified."
         ),
```

### Comparing `prefect-databricks-0.2.3/prefect_databricks/rest.py` & `prefect_databricks-0.2.4/prefect_databricks/rest.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,26 @@
 # manually editing this file is not recommended.
 
 import json
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import httpx
-from prefect import task
-from pydantic import VERSION as PYDANTIC_VERSION
 
-if PYDANTIC_VERSION.startswith("2."):
+from prefect._internal.pydantic import HAS_PYDANTIC_V2
+from prefect._internal.pydantic._compat import model_dump
+
+if HAS_PYDANTIC_V2:
+    from pydantic import BaseModel as V2BaseModel
     from pydantic.v1 import BaseModel
 else:
     from pydantic import BaseModel
 
+from prefect import task
+
 if TYPE_CHECKING:
     from prefect_databricks import DatabricksCredentials
 
 
 class HTTPMethod(Enum):
     """
     Available HTTP request methods.
@@ -46,16 +50,16 @@
         Serialized version of object.
     """
     if isinstance(obj, list):
         return [serialize_model(o) for o in obj]
     elif isinstance(obj, Dict):
         return {k: serialize_model(v) for k, v in obj.items()}
 
-    if isinstance(obj, BaseModel):
-        return {k: serialize_model(v) for k, v in obj.dict().items()}
+    if isinstance(obj, (BaseModel, V2BaseModel)):
+        return model_dump(obj, mode="json")
     elif isinstance(obj, Enum):
         return obj.value
     return obj
 
 
 def strip_kwargs(**kwargs: Dict) -> Dict:
     """
```

### Comparing `prefect-databricks-0.2.3/prefect_databricks.egg-info/PKG-INFO` & `prefect_databricks-0.2.4/prefect_databricks.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,698 +1,474 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7072 6566  : 2.1.Name: pref
 00000020: 6563 742d 6461 7461 6272 6963 6b73 0a56  ect-databricks.V
-00000030: 6572 7369 6f6e 3a20 302e 322e 330a 5375  ersion: 0.2.3.Su
+00000030: 6572 7369 6f6e 3a20 302e 322e 340a 5375  ersion: 0.2.4.Su
 00000040: 6d6d 6172 793a 2050 7265 6665 6374 2069  mmary: Prefect i
-00000050: 6e74 6567 7261 7469 6f6e 7320 696e 7465  ntegrations inte
-00000060: 7261 6374 696e 6720 7769 7468 2044 6174  racting with Dat
-00000070: 6162 7269 636b 730a 486f 6d65 2d70 6167  abricks.Home-pag
-00000080: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
-00000090: 622e 636f 6d2f 5072 6566 6563 7448 512f  b.com/PrefectHQ/
-000000a0: 7072 6566 6563 742d 6461 7461 6272 6963  prefect-databric
-000000b0: 6b73 0a41 7574 686f 723a 2050 7265 6665  ks.Author: Prefe
-000000c0: 6374 2054 6563 686e 6f6c 6f67 6965 732c  ct Technologies,
-000000d0: 2049 6e63 2e0a 4175 7468 6f72 2d65 6d61   Inc..Author-ema
-000000e0: 696c 3a20 6865 6c70 4070 7265 6665 6374  il: help@prefect
-000000f0: 2e69 6f0a 4c69 6365 6e73 653a 2041 7061  .io.License: Apa
-00000100: 6368 6520 4c69 6365 6e73 6520 322e 300a  che License 2.0.
-00000110: 4b65 7977 6f72 6473 3a20 7072 6566 6563  Keywords: prefec
-00000120: 740a 436c 6173 7369 6669 6572 3a20 4e61  t.Classifier: Na
-00000130: 7475 7261 6c20 4c61 6e67 7561 6765 203a  tural Language :
-00000140: 3a20 456e 676c 6973 680a 436c 6173 7369  : English.Classi
-00000150: 6669 6572 3a20 496e 7465 6e64 6564 2041  fier: Intended A
-00000160: 7564 6965 6e63 6520 3a3a 2044 6576 656c  udience :: Devel
-00000170: 6f70 6572 730a 436c 6173 7369 6669 6572  opers.Classifier
-00000180: 3a20 496e 7465 6e64 6564 2041 7564 6965  : Intended Audie
-00000190: 6e63 6520 3a3a 2053 7973 7465 6d20 4164  nce :: System Ad
-000001a0: 6d69 6e69 7374 7261 746f 7273 0a43 6c61  ministrators.Cla
-000001b0: 7373 6966 6965 723a 204c 6963 656e 7365  ssifier: License
-000001c0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-000001d0: 203a 3a20 4170 6163 6865 2053 6f66 7477   :: Apache Softw
-000001e0: 6172 6520 4c69 6365 6e73 650a 436c 6173  are License.Clas
-000001f0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000200: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000210: 5079 7468 6f6e 203a 3a20 3320 3a3a 204f  Python :: 3 :: O
-00000220: 6e6c 790a 436c 6173 7369 6669 6572 3a20  nly.Classifier: 
-00000230: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000240: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000250: 3a20 332e 370a 436c 6173 7369 6669 6572  : 3.7.Classifier
-00000260: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000270: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000280: 203a 3a20 332e 380a 436c 6173 7369 6669   :: 3.8.Classifi
-00000290: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
-000002a0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000002b0: 6f6e 203a 3a20 332e 390a 436c 6173 7369  on :: 3.9.Classi
-000002c0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-000002d0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000002e0: 7468 6f6e 203a 3a20 332e 3130 0a43 6c61  thon :: 3.10.Cla
-000002f0: 7373 6966 6965 723a 2054 6f70 6963 203a  ssifier: Topic :
-00000300: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
-00000310: 6f70 6d65 6e74 203a 3a20 4c69 6272 6172  opment :: Librar
-00000320: 6965 730a 5265 7175 6972 6573 2d50 7974  ies.Requires-Pyt
-00000330: 686f 6e3a 203e 3d33 2e37 0a44 6573 6372  hon: >=3.7.Descr
-00000340: 6970 7469 6f6e 2d43 6f6e 7465 6e74 2d54  iption-Content-T
-00000350: 7970 653a 2074 6578 742f 6d61 726b 646f  ype: text/markdo
-00000360: 776e 0a4c 6963 656e 7365 2d46 696c 653a  wn.License-File:
-00000370: 204c 4943 454e 5345 0a52 6571 7569 7265   LICENSE.Require
-00000380: 732d 4469 7374 3a20 7072 6566 6563 743e  s-Dist: prefect>
-00000390: 3d32 2e31 332e 350a 5072 6f76 6964 6573  =2.13.5.Provides
-000003a0: 2d45 7874 7261 3a20 6465 760a 5265 7175  -Extra: dev.Requ
-000003b0: 6972 6573 2d44 6973 743a 2070 7974 6573  ires-Dist: pytes
-000003c0: 743b 2065 7874 7261 203d 3d20 2264 6576  t; extra == "dev
-000003d0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-000003e0: 2062 6c61 636b 3b20 6578 7472 6120 3d3d   black; extra ==
-000003f0: 2022 6465 7622 0a52 6571 7569 7265 732d   "dev".Requires-
-00000400: 4469 7374 3a20 666c 616b 6538 3b20 6578  Dist: flake8; ex
-00000410: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
-00000420: 7569 7265 732d 4469 7374 3a20 6d79 7079  uires-Dist: mypy
-00000430: 3b20 6578 7472 6120 3d3d 2022 6465 7622  ; extra == "dev"
-00000440: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000450: 6d6b 646f 6373 3b20 6578 7472 6120 3d3d  mkdocs; extra ==
-00000460: 2022 6465 7622 0a52 6571 7569 7265 732d   "dev".Requires-
-00000470: 4469 7374 3a20 6d6b 646f 6373 2d6d 6174  Dist: mkdocs-mat
-00000480: 6572 6961 6c3b 2065 7874 7261 203d 3d20  erial; extra == 
-00000490: 2264 6576 220a 5265 7175 6972 6573 2d44  "dev".Requires-D
-000004a0: 6973 743a 206d 6b64 6f63 7374 7269 6e67  ist: mkdocstring
-000004b0: 735b 7079 7468 6f6e 5d3b 2065 7874 7261  s[python]; extra
-000004c0: 203d 3d20 2264 6576 220a 5265 7175 6972   == "dev".Requir
-000004d0: 6573 2d44 6973 743a 2069 736f 7274 3b20  es-Dist: isort; 
-000004e0: 6578 7472 6120 3d3d 2022 6465 7622 0a52  extra == "dev".R
-000004f0: 6571 7569 7265 732d 4469 7374 3a20 7072  equires-Dist: pr
-00000500: 652d 636f 6d6d 6974 3b20 6578 7472 6120  e-commit; extra 
-00000510: 3d3d 2022 6465 7622 0a52 6571 7569 7265  == "dev".Require
-00000520: 732d 4469 7374 3a20 7079 7465 7374 2d61  s-Dist: pytest-a
-00000530: 7379 6e63 696f 3b20 6578 7472 6120 3d3d  syncio; extra ==
-00000540: 2022 6465 7622 0a52 6571 7569 7265 732d   "dev".Requires-
-00000550: 4469 7374 3a20 6d6f 636b 3b20 7079 7468  Dist: mock; pyth
-00000560: 6f6e 5f76 6572 7369 6f6e 203c 2022 332e  on_version < "3.
-00000570: 3822 2061 6e64 2065 7874 7261 203d 3d20  8" and extra == 
-00000580: 2264 6576 220a 5265 7175 6972 6573 2d44  "dev".Requires-D
-00000590: 6973 743a 206d 6b64 6f63 732d 6765 6e2d  ist: mkdocs-gen-
-000005a0: 6669 6c65 733b 2065 7874 7261 203d 3d20  files; extra == 
-000005b0: 2264 6576 220a 5265 7175 6972 6573 2d44  "dev".Requires-D
-000005c0: 6973 743a 2069 6e74 6572 726f 6761 7465  ist: interrogate
-000005d0: 3b20 6578 7472 6120 3d3d 2022 6465 7622  ; extra == "dev"
-000005e0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000005f0: 636f 7665 7261 6765 3b20 6578 7472 6120  coverage; extra 
-00000600: 3d3d 2022 6465 7622 0a52 6571 7569 7265  == "dev".Require
-00000610: 732d 4469 7374 3a20 7265 7370 783b 2065  s-Dist: respx; e
-00000620: 7874 7261 203d 3d20 2264 6576 220a 5265  xtra == "dev".Re
-00000630: 7175 6972 6573 2d44 6973 743a 2070 696c  quires-Dist: pil
-00000640: 6c6f 773b 2065 7874 7261 203d 3d20 2264  low; extra == "d
-00000650: 6576 220a 0a23 2049 6e74 6567 7261 7465  ev"..# Integrate
-00000660: 2044 6174 6162 7269 636b 7320 6a6f 6273   Databricks jobs
-00000670: 2069 6e74 6f20 796f 7572 2064 6174 6166   into your dataf
-00000680: 6c6f 7720 7769 7468 2070 7265 6665 6374  low with prefect
-00000690: 2d64 6174 6162 7269 636b 730a 200a 3c70  -databricks. .<p
-000006a0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-000006b0: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
-000006c0: 7474 7073 3a2f 2f75 7365 722d 696d 6167  ttps://user-imag
-000006d0: 6573 2e67 6974 6875 6275 7365 7263 6f6e  es.githubusercon
-000006e0: 7465 6e74 2e63 6f6d 2f31 3533 3331 3939  tent.com/1533199
-000006f0: 302f 3231 3938 3232 3433 392d 3730 6563  0/219822439-70ec
-00000700: 3832 6662 2d65 3933 612d 3439 3833 2d62  82fb-e93a-4983-b
-00000710: 6563 372d 3863 3832 3530 6662 6237 6163  ec7-8c8250fbb7ac
-00000720: 2e70 6e67 223e 0a20 2020 203c 6272 3e0a  .png">.    <br>.
-00000730: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
-00000740: 7073 3a2f 2f70 7970 692e 7079 7468 6f6e  ps://pypi.python
-00000750: 2e6f 7267 2f70 7970 692f 7072 6566 6563  .org/pypi/prefec
-00000760: 742d 6461 7461 6272 6963 6b73 2f22 2061  t-databricks/" a
-00000770: 6c74 3d22 5079 5049 2076 6572 7369 6f6e  lt="PyPI version
-00000780: 223e 0a20 2020 2020 2020 203c 696d 6720  ">.        <img 
-00000790: 616c 743d 2250 7950 4922 2073 7263 3d22  alt="PyPI" src="
-000007a0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000007b0: 6c64 732e 696f 2f70 7970 692f 762f 7072  lds.io/pypi/v/pr
-000007c0: 6566 6563 742d 6461 7461 6272 6963 6b73  efect-databricks
-000007d0: 3f63 6f6c 6f72 3d30 3035 3246 4626 6c61  ?color=0052FF&la
-000007e0: 6265 6c43 6f6c 6f72 3d30 3930 3432 3222  belColor=090422"
-000007f0: 3e3c 2f61 3e0a 2020 2020 3c61 2068 7265  ></a>.    <a hre
-00000800: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00000810: 622e 636f 6d2f 5072 6566 6563 7448 512f  b.com/PrefectHQ/
-00000820: 7072 6566 6563 742d 6461 7461 6272 6963  prefect-databric
-00000830: 6b73 2f22 2061 6c74 3d22 5374 6172 7322  ks/" alt="Stars"
-00000840: 3e0a 2020 2020 2020 2020 3c69 6d67 2073  >.        <img s
-00000850: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000860: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-00000870: 622f 7374 6172 732f 5072 6566 6563 7448  b/stars/PrefectH
-00000880: 512f 7072 6566 6563 742d 6461 7461 6272  Q/prefect-databr
-00000890: 6963 6b73 3f63 6f6c 6f72 3d30 3035 3246  icks?color=0052F
-000008a0: 4626 6c61 6265 6c43 6f6c 6f72 3d30 3930  F&labelColor=090
-000008b0: 3432 3222 202f 3e3c 2f61 3e0a 2020 2020  422" /></a>.    
-000008c0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000008d0: 2f70 6570 792e 7465 6368 2f62 6164 6765  /pepy.tech/badge
-000008e0: 2f70 7265 6665 6374 2d64 6174 6162 7269  /prefect-databri
-000008f0: 636b 732f 2220 616c 743d 2244 6f77 6e6c  cks/" alt="Downl
-00000900: 6f61 6473 223e 0a20 2020 2020 2020 203c  oads">.        <
-00000910: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00000920: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000930: 7079 7069 2f64 6d2f 7072 6566 6563 742d  pypi/dm/prefect-
-00000940: 6461 7461 6272 6963 6b73 3f63 6f6c 6f72  databricks?color
-00000950: 3d30 3035 3246 4626 6c61 6265 6c43 6f6c  =0052FF&labelCol
-00000960: 6f72 3d30 3930 3432 3222 202f 3e3c 2f61  or=090422" /></a
-00000970: 3e0a 2020 2020 3c61 2068 7265 663d 2268  >.    <a href="h
-00000980: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000990: 6d2f 5072 6566 6563 7448 512f 7072 6566  m/PrefectHQ/pref
-000009a0: 6563 742d 6461 7461 6272 6963 6b73 2f70  ect-databricks/p
-000009b0: 756c 7365 2220 616c 743d 2241 6374 6976  ulse" alt="Activ
-000009c0: 6974 7922 3e0a 2020 2020 2020 2020 3c69  ity">.        <i
-000009d0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-000009e0: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
-000009f0: 6974 6875 622f 636f 6d6d 6974 2d61 6374  ithub/commit-act
-00000a00: 6976 6974 792f 6d2f 5072 6566 6563 7448  ivity/m/PrefectH
-00000a10: 512f 7072 6566 6563 742d 6461 7461 6272  Q/prefect-databr
-00000a20: 6963 6b73 3f63 6f6c 6f72 3d30 3035 3246  icks?color=0052F
-00000a30: 4626 6c61 6265 6c43 6f6c 6f72 3d30 3930  F&labelColor=090
-00000a40: 3432 3222 202f 3e3c 2f61 3e0a 2020 2020  422" /></a>.    
-00000a50: 3c62 723e 0a20 2020 203c 6120 6872 6566  <br>.    <a href
-00000a60: 3d22 6874 7470 733a 2f2f 7072 6566 6563  ="https://prefec
-00000a70: 742d 636f 6d6d 756e 6974 792e 736c 6163  t-community.slac
-00000a80: 6b2e 636f 6d22 2061 6c74 3d22 536c 6163  k.com" alt="Slac
-00000a90: 6b22 3e0a 2020 2020 2020 2020 3c69 6d67  k">.        <img
-00000aa0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-00000ab0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00000ac0: 6765 2f73 6c61 636b 2d6a 6f69 6e5f 636f  ge/slack-join_co
-00000ad0: 6d6d 756e 6974 792d 7265 642e 7376 673f  mmunity-red.svg?
-00000ae0: 636f 6c6f 723d 3030 3532 4646 266c 6162  color=0052FF&lab
-00000af0: 656c 436f 6c6f 723d 3039 3034 3232 266c  elColor=090422&l
-00000b00: 6f67 6f3d 736c 6163 6b22 202f 3e3c 2f61  ogo=slack" /></a
-00000b10: 3e0a 2020 2020 3c61 2068 7265 663d 2268  >.    <a href="h
-00000b20: 7474 7073 3a2f 2f64 6973 636f 7572 7365  ttps://discourse
-00000b30: 2e70 7265 6665 6374 2e69 6f2f 2220 616c  .prefect.io/" al
-00000b40: 743d 2244 6973 636f 7572 7365 223e 0a20  t="Discourse">. 
-00000b50: 2020 2020 2020 203c 696d 6720 7372 633d         <img src=
-00000b60: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-00000b70: 656c 6473 2e69 6f2f 6261 6467 652f 6469  elds.io/badge/di
-00000b80: 7363 6f75 7273 652d 6272 6f77 7365 5f66  scourse-browse_f
-00000b90: 6f72 756d 2d72 6564 2e73 7667 3f63 6f6c  orum-red.svg?col
-00000ba0: 6f72 3d30 3035 3246 4626 6c61 6265 6c43  or=0052FF&labelC
-00000bb0: 6f6c 6f72 3d30 3930 3432 3226 6c6f 676f  olor=090422&logo
-00000bc0: 3d64 6973 636f 7572 7365 2220 2f3e 3c2f  =discourse" /></
-00000bd0: 613e 0a3c 2f70 3e0a 0a56 6973 6974 2074  a>.</p>..Visit t
-00000be0: 6865 2066 756c 6c20 646f 6373 205b 6865  he full docs [he
-00000bf0: 7265 5d28 6874 7470 733a 2f2f 5072 6566  re](https://Pref
-00000c00: 6563 7448 512e 6769 7468 7562 2e69 6f2f  ectHQ.github.io/
-00000c10: 7072 6566 6563 742d 6461 7461 6272 6963  prefect-databric
-00000c20: 6b73 2920 746f 2073 6565 2061 6464 6974  ks) to see addit
-00000c30: 696f 6e61 6c20 6578 616d 706c 6573 2061  ional examples a
-00000c40: 6e64 2074 6865 2041 5049 2072 6566 6572  nd the API refer
-00000c50: 656e 6365 2e0a 0a54 6865 2070 7265 6665  ence...The prefe
-00000c60: 6374 2d64 6174 6162 7269 636b 7320 636f  ct-databricks co
-00000c70: 6c6c 6563 7469 6f6e 206d 616b 6573 2069  llection makes i
-00000c80: 7420 6561 7379 2074 6f20 636f 6f72 6469  t easy to coordi
-00000c90: 616e 7465 2044 6174 6162 7269 636b 7320  ante Databricks 
-00000ca0: 6a6f 6273 2077 6974 6820 6f74 6865 7220  jobs with other 
-00000cb0: 746f 6f6c 7320 696e 2079 6f75 7220 6461  tools in your da
-00000cc0: 7461 2073 7461 636b 2075 7369 6e67 2050  ta stack using P
-00000cd0: 7265 6665 6374 2e20 4368 6563 6b20 6f75  refect. Check ou
-00000ce0: 7420 7468 6520 6578 616d 706c 6573 2062  t the examples b
-00000cf0: 656c 6f77 2074 6f20 6765 7420 7374 6172  elow to get star
-00000d00: 7465 6421 0a0a 2323 2047 6574 7469 6e67  ted!..## Getting
-00000d10: 2053 7461 7274 6564 0a0a 2323 2320 496e   Started..### In
-00000d20: 7465 6772 6174 6520 7769 7468 2050 7265  tegrate with Pre
-00000d30: 6665 6374 2066 6c6f 7773 0a0a 5573 696e  fect flows..Usin
-00000d40: 6720 5072 6566 6563 7420 7769 7468 2044  g Prefect with D
-00000d50: 6174 6162 7269 636b 7320 616c 6c6f 7773  atabricks allows
-00000d60: 2079 6f75 2074 6f20 6465 6669 6e65 2061   you to define a
-00000d70: 6e64 206f 7263 6865 7374 7261 7465 2063  nd orchestrate c
-00000d80: 6f6d 706c 6578 2064 6174 6120 776f 726b  omplex data work
-00000d90: 666c 6f77 7320 7468 6174 2074 616b 6520  flows that take 
-00000da0: 6164 7661 6e74 6167 6520 6f66 2074 6865  advantage of the
-00000db0: 2073 6361 6c61 6269 6c69 7479 2061 6e64   scalability and
-00000dc0: 2070 6572 666f 726d 616e 6365 206f 6620   performance of 
-00000dd0: 4461 7461 6272 6963 6b73 2e0a 0a54 6869  Databricks...Thi
-00000de0: 7320 6361 6e20 6265 2065 7370 6563 6961  s can be especia
-00000df0: 6c6c 7920 7573 6566 756c 2066 6f72 2064  lly useful for d
-00000e00: 6174 612d 696e 7465 6e73 6976 6520 7461  ata-intensive ta
-00000e10: 736b 7320 7375 6368 2061 7320 4554 4c20  sks such as ETL 
-00000e20: 2865 7874 7261 6374 2c20 7472 616e 7366  (extract, transf
-00000e30: 6f72 6d2c 206c 6f61 6429 2070 6970 656c  orm, load) pipel
-00000e40: 696e 6573 2c20 6d61 6368 696e 6520 6c65  ines, machine le
-00000e50: 6172 6e69 6e67 2074 7261 696e 696e 6720  arning training 
-00000e60: 616e 6420 696e 6665 7265 6e63 652c 2061  and inference, a
-00000e70: 6e64 2072 6561 6c2d 7469 6d65 2064 6174  nd real-time dat
-00000e80: 6120 7072 6f63 6573 7369 6e67 2e0a 0a42  a processing...B
-00000e90: 656c 6f77 2069 7320 616e 2065 7861 6d70  elow is an examp
-00000ea0: 6c65 206f 6620 686f 7720 796f 7520 6361  le of how you ca
-00000eb0: 6e20 696e 636f 7270 6f72 6174 6520 4461  n incorporate Da
-00000ec0: 7461 6272 6963 6b73 206e 6f74 6562 6f6f  tabricks noteboo
-00000ed0: 6b73 2077 6974 6869 6e20 796f 7572 2050  ks within your P
-00000ee0: 7265 6665 6374 2066 6c6f 7773 2e0a 0a42  refect flows...B
-00000ef0: 6520 7375 7265 2074 6f20 696e 7374 616c  e sure to instal
-00000f00: 6c20 5b70 7265 6665 6374 2d64 6174 6162  l [prefect-datab
-00000f10: 7269 636b 735d 2823 696e 7374 616c 6c61  ricks](#installa
-00000f20: 7469 6f6e 2920 616e 6420 5b73 6176 6520  tion) and [save 
-00000f30: 6120 6372 6564 656e 7469 616c 7320 626c  a credentials bl
-00000f40: 6f63 6b5d 2823 7361 7669 6e67 2d63 7265  ock](#saving-cre
-00000f50: 6465 6e74 6961 6c73 2d74 6f2d 626c 6f63  dentials-to-bloc
-00000f60: 6b29 2074 6f20 7275 6e20 7468 6520 6578  k) to run the ex
-00000f70: 616d 706c 6573 2062 656c 6f77 210a 0a49  amples below!..I
-00000f80: 6620 796f 7520 646f 6e27 7420 6861 7665  f you don't have
-00000f90: 2061 6e20 6578 6973 7469 6e67 206e 6f74   an existing not
-00000fa0: 6562 6f6f 6b20 7265 6164 7920 6f6e 2044  ebook ready on D
-00000fb0: 6174 6162 7269 636b 732c 2079 6f75 2063  atabricks, you c
-00000fc0: 616e 2063 6f70 7920 7468 6520 666f 6c6c  an copy the foll
-00000fd0: 6f77 696e 672c 2061 6e64 206e 616d 6520  owing, and name 
-00000fe0: 6974 2060 6578 616d 706c 652e 6970 796e  it `example.ipyn
-00000ff0: 6260 2e20 5468 6973 206e 6f74 6562 6f6f  b`. This noteboo
-00001000: 6b2c 2061 6363 6570 7473 2061 206e 616d  k, accepts a nam
-00001010: 6520 7061 7261 6d65 7465 7220 6672 6f6d  e parameter from
-00001020: 2074 6865 2066 6c6f 7720 616e 6420 7369   the flow and si
-00001030: 6d70 6c79 2070 7269 6e74 7320 6120 6d65  mply prints a me
-00001040: 7373 6167 652e 0a0a 6060 6070 7974 686f  ssage...```pytho
-00001050: 6e0a 6e61 6d65 203d 2064 6275 7469 6c73  n.name = dbutils
-00001060: 2e77 6964 6765 7473 2e67 6574 2822 6e61  .widgets.get("na
-00001070: 6d65 2229 0a6d 6573 7361 6765 203d 2066  me").message = f
-00001080: 2244 6f6e 2774 2077 6f72 7279 207b 6e61  "Don't worry {na
-00001090: 6d65 7d2c 2049 2067 6f74 2079 6f75 7220  me}, I got your 
-000010a0: 7265 7175 6573 7421 2057 656c 636f 6d65  request! Welcome
-000010b0: 2074 6f20 7072 6566 6563 742d 6461 7461   to prefect-data
-000010c0: 6272 6963 6b73 2122 0a70 7269 6e74 286d  bricks!".print(m
-000010d0: 6573 7361 6765 290a 6060 600a 0a48 6572  essage).```..Her
-000010e0: 652c 2074 6865 2066 6c6f 7720 6c61 756e  e, the flow laun
-000010f0: 6368 6573 2061 206e 6577 2063 6c75 7374  ches a new clust
-00001100: 6572 2074 6f20 7275 6e20 6065 7861 6d70  er to run `examp
-00001110: 6c65 2e69 7079 6e62 6020 616e 6420 7761  le.ipynb` and wa
-00001120: 6974 7320 666f 7220 7468 6520 636f 6d70  its for the comp
-00001130: 6c65 7469 6f6e 206f 6620 7468 6520 6e6f  letion of the no
-00001140: 7465 626f 6f6b 2072 756e 2e20 5265 706c  tebook run. Repl
-00001150: 6163 6520 7468 6520 706c 6163 6568 6f6c  ace the placehol
-00001160: 6465 7273 2061 6e64 2072 756e 2e0a 0a60  ders and run...`
-00001170: 6060 7079 7468 6f6e 0a66 726f 6d20 7072  ``python.from pr
-00001180: 6566 6563 7420 696d 706f 7274 2066 6c6f  efect import flo
-00001190: 770a 6672 6f6d 2070 7265 6665 6374 5f64  w.from prefect_d
-000011a0: 6174 6162 7269 636b 7320 696d 706f 7274  atabricks import
-000011b0: 2044 6174 6162 7269 636b 7343 7265 6465   DatabricksCrede
-000011c0: 6e74 6961 6c73 0a66 726f 6d20 7072 6566  ntials.from pref
-000011d0: 6563 745f 6461 7461 6272 6963 6b73 2e66  ect_databricks.f
-000011e0: 6c6f 7773 2069 6d70 6f72 7420 6a6f 6273  lows import jobs
-000011f0: 5f72 756e 735f 7375 626d 6974 5f61 6e64  _runs_submit_and
-00001200: 5f77 6169 745f 666f 725f 636f 6d70 6c65  _wait_for_comple
-00001210: 7469 6f6e 0a66 726f 6d20 7072 6566 6563  tion.from prefec
-00001220: 745f 6461 7461 6272 6963 6b73 2e6d 6f64  t_databricks.mod
-00001230: 656c 732e 6a6f 6273 2069 6d70 6f72 7420  els.jobs import 
-00001240: 280a 2020 2020 4175 746f 5363 616c 652c  (.    AutoScale,
-00001250: 0a20 2020 2041 7773 4174 7472 6962 7574  .    AwsAttribut
-00001260: 6573 2c0a 2020 2020 4a6f 6254 6173 6b53  es,.    JobTaskS
-00001270: 6574 7469 6e67 732c 0a20 2020 204e 6f74  ettings,.    Not
-00001280: 6562 6f6f 6b54 6173 6b2c 0a20 2020 204e  ebookTask,.    N
-00001290: 6577 436c 7573 7465 722c 0a29 0a0a 0a40  ewCluster,.)...@
-000012a0: 666c 6f77 0a64 6566 206a 6f62 735f 7275  flow.def jobs_ru
-000012b0: 6e73 5f73 7562 6d69 745f 666c 6f77 2862  ns_submit_flow(b
-000012c0: 6c6f 636b 5f6e 616d 653a 2073 7472 2c20  lock_name: str, 
-000012d0: 6e6f 7465 626f 6f6b 5f70 6174 683a 2073  notebook_path: s
-000012e0: 7472 2c20 2a2a 6261 7365 5f70 6172 616d  tr, **base_param
-000012f0: 6574 6572 7329 3a0a 2020 2020 6461 7461  eters):.    data
-00001300: 6272 6963 6b73 5f63 7265 6465 6e74 6961  bricks_credentia
-00001310: 6c73 203d 2044 6174 6162 7269 636b 7343  ls = DatabricksC
-00001320: 7265 6465 6e74 6961 6c73 2e6c 6f61 6428  redentials.load(
-00001330: 626c 6f63 6b5f 6e61 6d65 290a 0a20 2020  block_name)..   
-00001340: 2023 2073 7065 6369 6679 206e 6577 2063   # specify new c
-00001350: 6c75 7374 6572 2073 6574 7469 6e67 730a  luster settings.
-00001360: 2020 2020 6177 735f 6174 7472 6962 7574      aws_attribut
-00001370: 6573 203d 2041 7773 4174 7472 6962 7574  es = AwsAttribut
-00001380: 6573 280a 2020 2020 2020 2020 6176 6169  es(.        avai
-00001390: 6c61 6269 6c69 7479 3d22 5350 4f54 222c  lability="SPOT",
-000013a0: 0a20 2020 2020 2020 207a 6f6e 655f 6964  .        zone_id
-000013b0: 3d22 7573 2d77 6573 742d 3261 222c 0a20  ="us-west-2a",. 
-000013c0: 2020 2020 2020 2065 6273 5f76 6f6c 756d         ebs_volum
-000013d0: 655f 7479 7065 3d22 4745 4e45 5241 4c5f  e_type="GENERAL_
-000013e0: 5055 5250 4f53 455f 5353 4422 2c0a 2020  PURPOSE_SSD",.  
-000013f0: 2020 2020 2020 6562 735f 766f 6c75 6d65        ebs_volume
-00001400: 5f63 6f75 6e74 3d33 2c0a 2020 2020 2020  _count=3,.      
-00001410: 2020 6562 735f 766f 6c75 6d65 5f73 697a    ebs_volume_siz
-00001420: 653d 3130 302c 0a20 2020 2029 0a20 2020  e=100,.    ).   
-00001430: 2061 7574 6f5f 7363 616c 6520 3d20 4175   auto_scale = Au
-00001440: 746f 5363 616c 6528 6d69 6e5f 776f 726b  toScale(min_work
-00001450: 6572 733d 312c 206d 6178 5f77 6f72 6b65  ers=1, max_worke
-00001460: 7273 3d32 290a 2020 2020 6e65 775f 636c  rs=2).    new_cl
-00001470: 7573 7465 7220 3d20 4e65 7743 6c75 7374  uster = NewClust
-00001480: 6572 280a 2020 2020 2020 2020 6177 735f  er(.        aws_
-00001490: 6174 7472 6962 7574 6573 3d61 7773 5f61  attributes=aws_a
-000014a0: 7474 7269 6275 7465 732c 0a20 2020 2020  ttributes,.     
-000014b0: 2020 2061 7574 6f73 6361 6c65 3d61 7574     autoscale=aut
-000014c0: 6f5f 7363 616c 652c 0a20 2020 2020 2020  o_scale,.       
-000014d0: 206e 6f64 655f 7479 7065 5f69 643d 226d   node_type_id="m
-000014e0: 342e 6c61 7267 6522 2c0a 2020 2020 2020  4.large",.      
-000014f0: 2020 7370 6172 6b5f 7665 7273 696f 6e3d    spark_version=
-00001500: 2231 302e 342e 782d 7363 616c 6132 2e31  "10.4.x-scala2.1
-00001510: 3222 2c0a 2020 2020 2020 2020 7370 6172  2",.        spar
-00001520: 6b5f 636f 6e66 3d7b 2273 7061 726b 2e73  k_conf={"spark.s
-00001530: 7065 6375 6c61 7469 6f6e 223a 2054 7275  peculation": Tru
-00001540: 657d 2c0a 2020 2020 290a 0a20 2020 2023  e},.    )..    #
-00001550: 2073 7065 6369 6679 206e 6f74 6562 6f6f   specify noteboo
-00001560: 6b20 746f 2075 7365 2061 6e64 2070 6172  k to use and par
-00001570: 616d 6574 6572 7320 746f 2070 6173 730a  ameters to pass.
-00001580: 2020 2020 6e6f 7465 626f 6f6b 5f74 6173      notebook_tas
-00001590: 6b20 3d20 4e6f 7465 626f 6f6b 5461 736b  k = NotebookTask
-000015a0: 280a 2020 2020 2020 2020 6e6f 7465 626f  (.        notebo
-000015b0: 6f6b 5f70 6174 683d 6e6f 7465 626f 6f6b  ok_path=notebook
-000015c0: 5f70 6174 682c 0a20 2020 2020 2020 2062  _path,.        b
-000015d0: 6173 655f 7061 7261 6d65 7465 7273 3d62  ase_parameters=b
-000015e0: 6173 655f 7061 7261 6d65 7465 7273 2c0a  ase_parameters,.
-000015f0: 2020 2020 290a 0a20 2020 2023 2063 6f6d      )..    # com
-00001600: 7069 6c65 206a 6f62 2074 6173 6b20 7365  pile job task se
-00001610: 7474 696e 6773 0a20 2020 206a 6f62 5f74  ttings.    job_t
-00001620: 6173 6b5f 7365 7474 696e 6773 203d 204a  ask_settings = J
-00001630: 6f62 5461 736b 5365 7474 696e 6773 280a  obTaskSettings(.
-00001640: 2020 2020 2020 2020 6e65 775f 636c 7573          new_clus
-00001650: 7465 723d 6e65 775f 636c 7573 7465 722c  ter=new_cluster,
-00001660: 0a20 2020 2020 2020 206e 6f74 6562 6f6f  .        noteboo
-00001670: 6b5f 7461 736b 3d6e 6f74 6562 6f6f 6b5f  k_task=notebook_
-00001680: 7461 736b 2c0a 2020 2020 2020 2020 7461  task,.        ta
-00001690: 736b 5f6b 6579 3d22 7072 6566 6563 742d  sk_key="prefect-
-000016a0: 7461 736b 220a 2020 2020 290a 0a20 2020  task".    )..   
-000016b0: 2072 756e 203d 206a 6f62 735f 7275 6e73   run = jobs_runs
-000016c0: 5f73 7562 6d69 745f 616e 645f 7761 6974  _submit_and_wait
-000016d0: 5f66 6f72 5f63 6f6d 706c 6574 696f 6e28  _for_completion(
-000016e0: 0a20 2020 2020 2020 2064 6174 6162 7269  .        databri
-000016f0: 636b 735f 6372 6564 656e 7469 616c 733d  cks_credentials=
-00001700: 6461 7461 6272 6963 6b73 5f63 7265 6465  databricks_crede
-00001710: 6e74 6961 6c73 2c0a 2020 2020 2020 2020  ntials,.        
-00001720: 7275 6e5f 6e61 6d65 3d22 7072 6566 6563  run_name="prefec
-00001730: 742d 6a6f 6222 2c0a 2020 2020 2020 2020  t-job",.        
-00001740: 7461 736b 733d 5b6a 6f62 5f74 6173 6b5f  tasks=[job_task_
-00001750: 7365 7474 696e 6773 5d0a 2020 2020 290a  settings].    ).
-00001760: 0a20 2020 2072 6574 7572 6e20 7275 6e0a  .    return run.
-00001770: 0a0a 6a6f 6273 5f72 756e 735f 7375 626d  ..jobs_runs_subm
-00001780: 6974 5f66 6c6f 7728 0a20 2020 2062 6c6f  it_flow(.    blo
-00001790: 636b 5f6e 616d 653d 2242 4c4f 434b 2d4e  ck_name="BLOCK-N
-000017a0: 414d 452d 504c 4143 4548 4f4c 4445 5222  AME-PLACEHOLDER"
-000017b0: 0a20 2020 206e 6f74 6562 6f6f 6b5f 7061  .    notebook_pa
-000017c0: 7468 3d22 2f55 7365 7273 2f3c 454d 4149  th="/Users/<EMAI
-000017d0: 4c5f 4144 4452 4553 535f 504c 4143 4548  L_ADDRESS_PLACEH
-000017e0: 4f4c 4445 523e 2f65 7861 6d70 6c65 2e69  OLDER>/example.i
-000017f0: 7079 6e62 222c 0a20 2020 206e 616d 653d  pynb",.    name=
-00001800: 224d 6172 7669 6e22 0a29 0a60 6060 0a0a  "Marvin".).```..
-00001810: 5570 6f6e 2065 7865 6375 7469 6f6e 2c20  Upon execution, 
-00001820: 7468 6520 6e6f 7465 626f 6f6b 2072 756e  the notebook run
-00001830: 2073 686f 756c 6420 6f75 7470 7574 3a0a   should output:.
-00001840: 0a60 6060 0a44 6f6e 2774 2077 6f72 7279  .```.Don't worry
-00001850: 204d 6172 7669 6e2c 2049 2067 6f74 2079   Marvin, I got y
-00001860: 6f75 7220 7265 7175 6573 7421 2057 656c  our request! Wel
-00001870: 636f 6d65 2074 6f20 7072 6566 6563 742d  come to prefect-
-00001880: 6461 7461 6272 6963 6b73 210a 6060 600a  databricks!.```.
-00001890: 0a21 2121 2069 6e66 6f20 2249 6e70 7574  .!!! info "Input
-000018a0: 2064 6963 7469 6f6e 6172 6965 7320 696e   dictionaries in
-000018b0: 2074 6865 2070 6c61 6365 206f 6620 6d6f   the place of mo
-000018c0: 6465 6c73 220a 2020 2020 0a20 2020 2049  dels".    .    I
-000018d0: 6e73 7465 6164 206f 6620 7573 696e 6720  nstead of using 
-000018e0: 7468 6520 6275 696c 742d 696e 206d 6f64  the built-in mod
-000018f0: 656c 732c 2079 6f75 206d 6179 2061 6c73  els, you may als
-00001900: 6f20 696e 7075 7420 6120 7661 6c69 6420  o input a valid 
-00001910: 6469 6374 696f 6e61 7279 2e0a 2020 2020  dictionary..    
-00001920: 0a20 2020 2046 6f72 2065 7861 6d70 6c65  .    For example
-00001930: 2c20 7468 6520 666f 6c6c 6f77 696e 6720  , the following 
-00001940: 6172 6520 6571 7569 7661 6c65 6e74 3a0a  are equivalent:.
-00001950: 0a20 2020 2060 6060 7079 7468 6f6e 0a20  .    ```python. 
-00001960: 2020 2061 7574 6f5f 7363 616c 653d 4175     auto_scale=Au
-00001970: 746f 5363 616c 6528 6d69 6e5f 776f 726b  toScale(min_work
-00001980: 6572 733d 312c 206d 6178 5f77 6f72 6b65  ers=1, max_worke
-00001990: 7273 3d32 290a 2020 2020 6060 600a 0a20  rs=2).    ```.. 
-000019a0: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
-000019b0: 2061 7574 6f5f 7363 616c 653d 7b22 6d69   auto_scale={"mi
-000019c0: 6e5f 776f 726b 6572 7322 3a20 312c 2022  n_workers": 1, "
-000019d0: 6d61 785f 776f 726b 6572 7322 3a20 327d  max_workers": 2}
-000019e0: 0a20 2020 2060 6060 0a0a 4966 2079 6f75  .    ```..If you
-000019f0: 2068 6176 6520 616e 2065 7869 7374 696e   have an existin
-00001a00: 6720 4461 7461 6272 6963 6b73 206a 6f62  g Databricks job
-00001a10: 2c20 796f 7520 6361 6e20 7275 6e20 6974  , you can run it
-00001a20: 2075 7369 6e67 2060 6a6f 6273 5f72 756e   using `jobs_run
-00001a30: 735f 7375 626d 6974 5f62 795f 6964 5f61  s_submit_by_id_a
-00001a40: 6e64 5f77 6169 745f 666f 725f 636f 6d70  nd_wait_for_comp
-00001a50: 6c65 7469 6f6e 603a 0a0a 6060 6070 7974  letion`:..```pyt
-00001a60: 686f 6e0a 6672 6f6d 2070 7265 6665 6374  hon.from prefect
-00001a70: 2069 6d70 6f72 7420 666c 6f77 0a0a 6672   import flow..fr
-00001a80: 6f6d 2070 7265 6665 6374 5f64 6174 6162  om prefect_datab
-00001a90: 7269 636b 7320 696d 706f 7274 2044 6174  ricks import Dat
-00001aa0: 6162 7269 636b 7343 7265 6465 6e74 6961  abricksCredentia
-00001ab0: 6c73 0a66 726f 6d20 7072 6566 6563 745f  ls.from prefect_
-00001ac0: 6461 7461 6272 6963 6b73 2e66 6c6f 7773  databricks.flows
-00001ad0: 2069 6d70 6f72 7420 280a 2020 2020 6a6f   import (.    jo
-00001ae0: 6273 5f72 756e 735f 7375 626d 6974 5f62  bs_runs_submit_b
-00001af0: 795f 6964 5f61 6e64 5f77 6169 745f 666f  y_id_and_wait_fo
-00001b00: 725f 636f 6d70 6c65 7469 6f6e 2c0a 290a  r_completion,.).
-00001b10: 0a0a 4066 6c6f 770a 6465 6620 6578 6973  ..@flow.def exis
-00001b20: 7469 6e67 5f6a 6f62 5f73 7562 6d69 7428  ting_job_submit(
-00001b30: 6461 7461 6272 6963 6b73 5f63 7265 6465  databricks_crede
-00001b40: 6e74 6961 6c73 5f62 6c6f 636b 5f6e 616d  ntials_block_nam
-00001b50: 653a 2073 7472 2c20 6a6f 625f 6964 293a  e: str, job_id):
-00001b60: 0a20 2020 2064 6174 6162 7269 636b 735f  .    databricks_
-00001b70: 6372 6564 656e 7469 616c 7320 3d20 4461  credentials = Da
-00001b80: 7461 6272 6963 6b73 4372 6564 656e 7469  tabricksCredenti
-00001b90: 616c 732e 6c6f 6164 286e 616d 653d 626c  als.load(name=bl
-00001ba0: 6f63 6b5f 6e61 6d65 290a 0a20 2020 2072  ock_name)..    r
-00001bb0: 756e 203d 206a 6f62 735f 7275 6e73 5f73  un = jobs_runs_s
-00001bc0: 7562 6d69 745f 6279 5f69 645f 616e 645f  ubmit_by_id_and_
-00001bd0: 7761 6974 5f66 6f72 5f63 6f6d 706c 6574  wait_for_complet
-00001be0: 696f 6e28 0a20 2020 2020 2020 2064 6174  ion(.        dat
-00001bf0: 6162 7269 636b 735f 6372 6564 656e 7469  abricks_credenti
-00001c00: 616c 733d 6461 7461 6272 6963 6b73 5f63  als=databricks_c
-00001c10: 7265 6465 6e74 6961 6c73 2c20 6a6f 625f  redentials, job_
-00001c20: 6964 3d6a 6f62 5f69 640a 2020 2020 290a  id=job_id.    ).
-00001c30: 0a20 2020 2072 6574 7572 6e20 7275 6e0a  .    return run.
-00001c40: 0a65 7869 7374 696e 675f 6a6f 625f 7375  .existing_job_su
-00001c50: 626d 6974 2864 6174 6162 7269 636b 735f  bmit(databricks_
-00001c60: 6372 6564 656e 7469 616c 735f 626c 6f63  credentials_bloc
-00001c70: 6b5f 6e61 6d65 3d22 6462 2d63 7265 6473  k_name="db-creds
-00001c80: 222c 206a 6f62 5f69 643d 2259 4f55 522d  ", job_id="YOUR-
-00001c90: 4a4f 422d 4e41 4d45 2229 0a60 6060 0a0a  JOB-NAME").```..
-00001ca0: 2323 2052 6573 6f75 7263 6573 0a0a 466f  ## Resources..Fo
-00001cb0: 7220 6d6f 7265 2074 6970 7320 6f6e 2068  r more tips on h
-00001cc0: 6f77 2074 6f20 7573 6520 7461 736b 7320  ow to use tasks 
-00001cd0: 616e 6420 666c 6f77 7320 696e 2061 2043  and flows in a C
-00001ce0: 6f6c 6c65 6374 696f 6e2c 2063 6865 636b  ollection, check
-00001cf0: 206f 7574 205b 5573 696e 6720 436f 6c6c   out [Using Coll
-00001d00: 6563 7469 6f6e 735d 2868 7474 7073 3a2f  ections](https:/
-00001d10: 2f6f 7269 6f6e 2d64 6f63 732e 7072 6566  /orion-docs.pref
-00001d20: 6563 742e 696f 2f63 6f6c 6c65 6374 696f  ect.io/collectio
-00001d30: 6e73 2f75 7361 6765 2f29 210a 0a4e 6f74  ns/usage/)!..Not
-00001d40: 652c 2074 6865 2074 6173 6b73 2077 6974  e, the tasks wit
-00001d50: 6869 6e20 7468 6973 2063 6f6c 6c65 6374  hin this collect
-00001d60: 696f 6e20 7765 7265 2063 7265 6174 6564  ion were created
-00001d70: 2062 7920 6120 636f 6465 2067 656e 6572   by a code gener
-00001d80: 6174 6f72 2075 7369 6e67 2074 6865 2073  ator using the s
-00001d90: 6572 7669 6365 2773 204f 7065 6e41 5049  ervice's OpenAPI
-00001da0: 2073 7065 632e 0a0a 5468 6520 7365 7276   spec...The serv
-00001db0: 6963 6527 7320 5245 5354 2041 5049 2064  ice's REST API d
-00001dc0: 6f63 756d 656e 7461 7469 6f6e 2063 616e  ocumentation can
-00001dd0: 2062 6520 666f 756e 6420 5b68 6572 655d   be found [here]
-00001de0: 2868 7474 7073 3a2f 2f64 6f63 732e 6461  (https://docs.da
-00001df0: 7461 6272 6963 6b73 2e63 6f6d 2f64 6576  tabricks.com/dev
-00001e00: 2d74 6f6f 6c73 2f61 7069 2f6c 6174 6573  -tools/api/lates
-00001e10: 742f 696e 6465 782e 6874 6d6c 292e 0a0a  t/index.html)...
-00001e20: 2323 2320 496e 7374 616c 6c61 7469 6f6e  ### Installation
-00001e30: 0a0a 496e 7374 616c 6c20 6070 7265 6665  ..Install `prefe
-00001e40: 6374 2d64 6174 6162 7269 636b 7360 2077  ct-databricks` w
-00001e50: 6974 6820 6070 6970 603a 0a0a 6060 6062  ith `pip`:..```b
-00001e60: 6173 680a 7069 7020 696e 7374 616c 6c20  ash.pip install 
-00001e70: 7072 6566 6563 742d 6461 7461 6272 6963  prefect-databric
-00001e80: 6b73 0a60 6060 0a0a 5265 7175 6972 6573  ks.```..Requires
-00001e90: 2061 6e20 696e 7374 616c 6c61 7469 6f6e   an installation
-00001ea0: 206f 6620 5079 7468 6f6e 2033 2e37 2b2e   of Python 3.7+.
-00001eb0: 0a0a 5765 2072 6563 6f6d 6d65 6e64 2075  ..We recommend u
-00001ec0: 7369 6e67 2061 2050 7974 686f 6e20 7669  sing a Python vi
-00001ed0: 7274 7561 6c20 656e 7669 726f 6e6d 656e  rtual environmen
-00001ee0: 7420 6d61 6e61 6765 7220 7375 6368 2061  t manager such a
-00001ef0: 7320 7069 7065 6e76 2c20 636f 6e64 6120  s pipenv, conda 
-00001f00: 6f72 2076 6972 7475 616c 656e 762e 0a0a  or virtualenv...
-00001f10: 5468 6573 6520 7461 736b 7320 6172 6520  These tasks are 
-00001f20: 6465 7369 676e 6564 2074 6f20 776f 726b  designed to work
-00001f30: 2077 6974 6820 5072 6566 6563 7420 322e   with Prefect 2.
-00001f40: 2046 6f72 206d 6f72 6520 696e 666f 726d   For more inform
-00001f50: 6174 696f 6e20 6162 6f75 7420 686f 7720  ation about how 
-00001f60: 746f 2075 7365 2050 7265 6665 6374 2c20  to use Prefect, 
-00001f70: 706c 6561 7365 2072 6566 6572 2074 6f20  please refer to 
-00001f80: 7468 6520 5b50 7265 6665 6374 2064 6f63  the [Prefect doc
-00001f90: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
-00001fa0: 733a 2f2f 6f72 696f 6e2d 646f 6373 2e70  s://orion-docs.p
-00001fb0: 7265 6665 6374 2e69 6f2f 292e 0a0a 2323  refect.io/)...##
-00001fc0: 2320 5361 7669 6e67 2043 7265 6465 6e74  # Saving Credent
-00001fd0: 6961 6c73 2074 6f20 426c 6f63 6b0a 0a54  ials to Block..T
-00001fe0: 6f20 7573 6520 7468 6520 606c 6f61 6460  o use the `load`
-00001ff0: 206d 6574 686f 6420 6f6e 2042 6c6f 636b   method on Block
-00002000: 732c 2079 6f75 206d 7573 7420 616c 7265  s, you must alre
-00002010: 6164 7920 6861 7665 2061 2062 6c6f 636b  ady have a block
-00002020: 2064 6f63 756d 656e 7420 5b73 6176 6564   document [saved
-00002030: 2074 6872 6f75 6768 2063 6f64 655d 2868   through code](h
-00002040: 7474 7073 3a2f 2f6f 7269 6f6e 2d64 6f63  ttps://orion-doc
-00002050: 732e 7072 6566 6563 742e 696f 2f63 6f6e  s.prefect.io/con
-00002060: 6365 7074 732f 626c 6f63 6b73 2f23 7361  cepts/blocks/#sa
-00002070: 7669 6e67 2d62 6c6f 636b 7329 206f 7220  ving-blocks) or 
-00002080: 5b73 6176 6564 2074 6872 6f75 6768 2074  [saved through t
-00002090: 6865 2055 495d 2868 7474 7073 3a2f 2f6f  he UI](https://o
-000020a0: 7269 6f6e 2d64 6f63 732e 7072 6566 6563  rion-docs.prefec
-000020b0: 742e 696f 2f75 692f 626c 6f63 6b73 2f29  t.io/ui/blocks/)
-000020c0: 2e0a 0a42 656c 6f77 2069 7320 6120 7761  ...Below is a wa
-000020d0: 6c6b 7468 726f 7567 6820 6f6e 2073 6176  lkthrough on sav
-000020e0: 696e 6720 626c 6f63 6b20 646f 6375 6d65  ing block docume
-000020f0: 6e74 7320 7468 726f 7567 6820 636f 6465  nts through code
-00002100: 3b20 7369 6d70 6c79 2063 7265 6174 6520  ; simply create 
-00002110: 6120 7368 6f72 7420 7363 7269 7074 2c20  a short script, 
-00002120: 7265 706c 6163 696e 6720 7468 6520 706c  replacing the pl
-00002130: 6163 6568 6f6c 6465 7273 2e20 0a0a 312e  aceholders. ..1.
-00002140: 2048 6561 6420 6f76 6572 2074 6f20 5b44   Head over to [D
-00002150: 6174 6162 7269 636b 735d 2868 7474 7073  atabricks](https
-00002160: 3a2f 2f61 6363 6f75 6e74 732e 636c 6f75  ://accounts.clou
-00002170: 642e 6461 7461 6272 6963 6b73 2e63 6f6d  d.databricks.com
-00002180: 2f29 2e0a 322e 204c 6f67 696e 2074 6f20  /)..2. Login to 
-00002190: 796f 7572 2044 6174 6162 7269 636b 7320  your Databricks 
-000021a0: 6163 636f 756e 7420 616e 6420 7365 6c65  account and sele
-000021b0: 6374 2061 2077 6f72 6b73 7061 6365 2e0a  ct a workspace..
-000021c0: 332e 204f 6e20 7468 6520 746f 7020 7269  3. On the top ri
-000021d0: 6768 7420 7369 6465 206f 6620 7468 6520  ght side of the 
-000021e0: 6e61 7620 6261 722c 2063 6c69 636b 206f  nav bar, click o
-000021f0: 6e20 796f 7572 2061 6363 6f75 6e74 206e  n your account n
-00002200: 616d 6520 2d3e 2055 7365 7220 5365 7474  ame -> User Sett
-00002210: 696e 6773 2e0a 342e 2043 6c69 636b 2041  ings..4. Click A
-00002220: 6363 6573 7320 746f 6b65 6e73 202d 3e20  ccess tokens -> 
-00002230: 4765 6e65 7261 7465 206e 6577 2074 6f6b  Generate new tok
-00002240: 656e 202d 3e20 4765 6e65 7261 7465 2061  en -> Generate a
-00002250: 6e64 2063 6f70 7920 7468 6520 746f 6b65  nd copy the toke
-00002260: 6e2e 0a35 2e20 4e6f 7465 2064 6f77 6e20  n..5. Note down 
-00002270: 796f 7572 2044 6174 6162 7269 636b 7320  your Databricks 
-00002280: 696e 7374 616e 6365 2066 726f 6d20 7468  instance from th
-00002290: 6520 6272 6f77 7365 7220 5552 4c2c 2066  e browser URL, f
-000022a0: 6f72 6d61 7474 6564 206c 696b 6520 6068  ormatted like `h
-000022b0: 7474 7073 3a2f 2f3c 4441 5441 4252 4943  ttps://<DATABRIC
-000022c0: 4b53 2d49 4e53 5441 4e43 453e 2e63 6c6f  KS-INSTANCE>.clo
-000022d0: 7564 2e64 6174 6162 7269 636b 732e 636f  ud.databricks.co
-000022e0: 6d2f 600a 362e 2043 7265 6174 6520 6120  m/`.6. Create a 
-000022f0: 7368 6f72 7420 7363 7269 7074 2c20 7265  short script, re
-00002300: 706c 6163 696e 6720 7468 6520 706c 6163  placing the plac
-00002310: 6568 6f6c 6465 7273 2e0a 0a60 6060 7079  eholders...```py
-00002320: 7468 6f6e 0a66 726f 6d20 7072 6566 6563  thon.from prefec
-00002330: 745f 6461 7461 6272 6963 6b73 2069 6d70  t_databricks imp
-00002340: 6f72 7420 4461 7461 6272 6963 6b73 4372  ort DatabricksCr
-00002350: 6564 656e 7469 616c 730a 0a63 7265 6465  edentials..crede
-00002360: 6e74 6961 6c73 203d 2044 6174 6162 7269  ntials = Databri
-00002370: 636b 7343 7265 6465 6e74 6961 6c73 280a  cksCredentials(.
-00002380: 2020 2020 6461 7461 6272 6963 6b73 5f69      databricks_i
-00002390: 6e73 7461 6e63 653d 2244 4154 4142 5249  nstance="DATABRI
-000023a0: 434b 532d 494e 5354 414e 4345 2d50 4c41  CKS-INSTANCE-PLA
-000023b0: 4345 484f 4c44 4552 220a 2020 2020 746f  CEHOLDER".    to
-000023c0: 6b65 6e3d 2254 4f4b 454e 2d50 4c41 4345  ken="TOKEN-PLACE
-000023d0: 484f 4c44 4552 220a 290a 0a63 6f6e 6e65  HOLDER".)..conne
-000023e0: 6374 6f72 2e73 6176 6528 2242 4c4f 434b  ctor.save("BLOCK
-000023f0: 5f4e 414d 452d 504c 4143 4548 4f4c 4445  _NAME-PLACEHOLDE
-00002400: 5222 290a 6060 600a 0a43 6f6e 6772 6174  R").```..Congrat
-00002410: 7321 2059 6f75 2063 616e 206e 6f77 2065  s! You can now e
-00002420: 6173 696c 7920 6c6f 6164 2074 6865 2073  asily load the s
-00002430: 6176 6564 2062 6c6f 636b 2c20 7768 6963  aved block, whic
-00002440: 6820 686f 6c64 7320 796f 7572 2063 7265  h holds your cre
-00002450: 6465 6e74 6961 6c73 3a0a 0a60 6060 7079  dentials:..```py
-00002460: 7468 6f6e 0a66 726f 6d20 7072 6566 6563  thon.from prefec
-00002470: 745f 6461 7461 6272 6963 6b73 2069 6d70  t_databricks imp
-00002480: 6f72 7420 4461 7461 6272 6963 6b73 4372  ort DatabricksCr
-00002490: 6564 656e 7469 616c 730a 0a44 6174 6162  edentials..Datab
-000024a0: 7269 636b 7343 7265 6465 6e74 6961 6c73  ricksCredentials
-000024b0: 2e6c 6f61 6428 2242 4c4f 434b 5f4e 414d  .load("BLOCK_NAM
-000024c0: 452d 504c 4143 4548 4f4c 4445 5222 290a  E-PLACEHOLDER").
-000024d0: 6060 600a 0a21 2121 2069 6e66 6f20 2252  ```..!!! info "R
-000024e0: 6567 6973 7465 7269 6e67 2062 6c6f 636b  egistering block
-000024f0: 7322 0a0a 2020 2020 5265 6769 7374 6572  s"..    Register
-00002500: 2062 6c6f 636b 7320 696e 2074 6869 7320   blocks in this 
-00002510: 6d6f 6475 6c65 2074 6f0a 2020 2020 5b76  module to.    [v
-00002520: 6965 7720 616e 6420 6564 6974 2074 6865  iew and edit the
-00002530: 6d5d 2868 7474 7073 3a2f 2f6f 7269 6f6e  m](https://orion
-00002540: 2d64 6f63 732e 7072 6566 6563 742e 696f  -docs.prefect.io
-00002550: 2f75 692f 626c 6f63 6b73 2f29 0a20 2020  /ui/blocks/).   
-00002560: 206f 6e20 5072 6566 6563 7420 436c 6f75   on Prefect Clou
-00002570: 643a 0a0a 2020 2020 6060 6062 6173 680a  d:..    ```bash.
-00002580: 2020 2020 7072 6566 6563 7420 626c 6f63      prefect bloc
-00002590: 6b20 7265 6769 7374 6572 202d 6d20 7072  k register -m pr
-000025a0: 6566 6563 745f 6461 7461 6272 6963 6b73  efect_databricks
-000025b0: 0a20 2020 2060 6060 0a0a 2323 2320 4665  .    ```..### Fe
-000025c0: 6564 6261 636b 0a0a 4966 2079 6f75 2065  edback..If you e
-000025d0: 6e63 6f75 6e74 6572 2061 6e79 2062 7567  ncounter any bug
-000025e0: 7320 7768 696c 6520 7573 696e 6720 6070  s while using `p
-000025f0: 7265 6665 6374 2d64 6174 6162 7269 636b  refect-databrick
-00002600: 7360 2c20 6665 656c 2066 7265 6520 746f  s`, feel free to
-00002610: 206f 7065 6e20 616e 2069 7373 7565 2069   open an issue i
-00002620: 6e20 7468 6520 5b70 7265 6665 6374 2d64  n the [prefect-d
-00002630: 6174 6162 7269 636b 735d 2868 7474 7073  atabricks](https
-00002640: 3a2f 2f67 6974 6875 622e 636f 6d2f 5072  ://github.com/Pr
-00002650: 6566 6563 7448 512f 7072 6566 6563 742d  efectHQ/prefect-
-00002660: 6461 7461 6272 6963 6b73 2920 7265 706f  databricks) repo
-00002670: 7369 746f 7279 2e0a 0a49 6620 796f 7520  sitory...If you 
-00002680: 6861 7665 2061 6e79 2071 7565 7374 696f  have any questio
-00002690: 6e73 206f 7220 6973 7375 6573 2077 6869  ns or issues whi
-000026a0: 6c65 2075 7369 6e67 2060 7072 6566 6563  le using `prefec
-000026b0: 742d 6461 7461 6272 6963 6b73 602c 2079  t-databricks`, y
-000026c0: 6f75 2063 616e 2066 696e 6420 6865 6c70  ou can find help
-000026d0: 2069 6e20 6569 7468 6572 2074 6865 205b   in either the [
-000026e0: 5072 6566 6563 7420 4469 7363 6f75 7273  Prefect Discours
-000026f0: 6520 666f 7275 6d5d 2868 7474 7073 3a2f  e forum](https:/
-00002700: 2f64 6973 636f 7572 7365 2e70 7265 6665  /discourse.prefe
-00002710: 6374 2e69 6f2f 2920 6f72 2074 6865 205b  ct.io/) or the [
-00002720: 5072 6566 6563 7420 536c 6163 6b20 636f  Prefect Slack co
-00002730: 6d6d 756e 6974 795d 2868 7474 7073 3a2f  mmunity](https:/
-00002740: 2f70 7265 6665 6374 2e69 6f2f 736c 6163  /prefect.io/slac
-00002750: 6b29 2e0a 0a46 6565 6c20 6672 6565 2074  k)...Feel free t
-00002760: 6f20 7374 6172 206f 7220 7761 7463 6820  o star or watch 
-00002770: 5b60 7072 6566 6563 742d 6461 7461 6272  [`prefect-databr
-00002780: 6963 6b73 605d 2868 7474 7073 3a2f 2f67  icks`](https://g
-00002790: 6974 6875 622e 636f 6d2f 5072 6566 6563  ithub.com/Prefec
-000027a0: 7448 512f 7072 6566 6563 742d 6461 7461  tHQ/prefect-data
-000027b0: 6272 6963 6b73 2920 666f 7220 7570 6461  bricks) for upda
-000027c0: 7465 7320 746f 6f21 0a0a 2323 2320 436f  tes too!..### Co
-000027d0: 6e74 7269 6275 7469 6e67 0a0a 4966 2079  ntributing..If y
-000027e0: 6f75 2764 206c 696b 6520 746f 2068 656c  ou'd like to hel
-000027f0: 7020 636f 6e74 7269 6275 7465 2074 6f20  p contribute to 
-00002800: 6669 7820 616e 2069 7373 7565 206f 7220  fix an issue or 
-00002810: 6164 6420 6120 6665 6174 7572 6520 746f  add a feature to
-00002820: 2060 7072 6566 6563 742d 6461 7461 6272   `prefect-databr
-00002830: 6963 6b73 602c 2070 6c65 6173 6520 5b70  icks`, please [p
-00002840: 726f 706f 7365 2063 6861 6e67 6573 2074  ropose changes t
-00002850: 6872 6f75 6768 2061 2070 756c 6c20 7265  hrough a pull re
-00002860: 7175 6573 7420 6672 6f6d 2061 2066 6f72  quest from a for
-00002870: 6b20 6f66 2074 6865 2072 6570 6f73 6974  k of the reposit
-00002880: 6f72 795d 2868 7474 7073 3a2f 2f64 6f63  ory](https://doc
-00002890: 732e 6769 7468 7562 2e63 6f6d 2f65 6e2f  s.github.com/en/
-000028a0: 7075 6c6c 2d72 6571 7565 7374 732f 636f  pull-requests/co
-000028b0: 6c6c 6162 6f72 6174 696e 672d 7769 7468  llaborating-with
-000028c0: 2d70 756c 6c2d 7265 7175 6573 7473 2f70  -pull-requests/p
-000028d0: 726f 706f 7369 6e67 2d63 6861 6e67 6573  roposing-changes
-000028e0: 2d74 6f2d 796f 7572 2d77 6f72 6b2d 7769  -to-your-work-wi
-000028f0: 7468 2d70 756c 6c2d 7265 7175 6573 7473  th-pull-requests
-00002900: 2f63 7265 6174 696e 672d 612d 7075 6c6c  /creating-a-pull
-00002910: 2d72 6571 7565 7374 2d66 726f 6d2d 612d  -request-from-a-
-00002920: 666f 726b 292e 0a0a 4865 7265 2061 7265  fork)...Here are
-00002930: 2074 6865 2073 7465 7073 3a0a 0a31 2e20   the steps:..1. 
-00002940: 5b46 6f72 6b20 7468 6520 7265 706f 7369  [Fork the reposi
-00002950: 746f 7279 5d28 6874 7470 733a 2f2f 646f  tory](https://do
-00002960: 6373 2e67 6974 6875 622e 636f 6d2f 656e  cs.github.com/en
-00002970: 2f67 6574 2d73 7461 7274 6564 2f71 7569  /get-started/qui
-00002980: 636b 7374 6172 742f 666f 726b 2d61 2d72  ckstart/fork-a-r
-00002990: 6570 6f23 666f 726b 696e 672d 612d 7265  epo#forking-a-re
-000029a0: 706f 7369 746f 7279 290a 322e 205b 436c  pository).2. [Cl
-000029b0: 6f6e 6520 7468 6520 666f 726b 6564 2072  one the forked r
-000029c0: 6570 6f73 6974 6f72 795d 2868 7474 7073  epository](https
-000029d0: 3a2f 2f64 6f63 732e 6769 7468 7562 2e63  ://docs.github.c
-000029e0: 6f6d 2f65 6e2f 6765 742d 7374 6172 7465  om/en/get-starte
-000029f0: 642f 7175 6963 6b73 7461 7274 2f66 6f72  d/quickstart/for
-00002a00: 6b2d 612d 7265 706f 2363 6c6f 6e69 6e67  k-a-repo#cloning
-00002a10: 2d79 6f75 722d 666f 726b 6564 2d72 6570  -your-forked-rep
-00002a20: 6f73 6974 6f72 7929 0a33 2e20 496e 7374  ository).3. Inst
-00002a30: 616c 6c20 7468 6520 7265 706f 7369 746f  all the reposito
-00002a40: 7279 2061 6e64 2069 7473 2064 6570 656e  ry and its depen
-00002a50: 6465 6e63 6965 733a 0a60 6060 0a70 6970  dencies:.```.pip
-00002a60: 2069 6e73 7461 6c6c 202d 6520 222e 5b64   install -e ".[d
-00002a70: 6576 5d22 0a60 6060 0a34 2e20 4d61 6b65  ev]".```.4. Make
-00002a80: 2064 6573 6972 6564 2063 6861 6e67 6573   desired changes
-00002a90: 0a35 2e20 4164 6420 7465 7374 730a 362e  .5. Add tests.6.
-00002aa0: 2049 6e73 6572 7420 616e 2065 6e74 7279   Insert an entry
-00002ab0: 2074 6f20 5b43 4841 4e47 454c 4f47 2e6d   to [CHANGELOG.m
-00002ac0: 645d 2868 7474 7073 3a2f 2f67 6974 6875  d](https://githu
-00002ad0: 622e 636f 6d2f 5072 6566 6563 7448 512f  b.com/PrefectHQ/
-00002ae0: 7072 6566 6563 742d 6461 7461 6272 6963  prefect-databric
-00002af0: 6b73 2f62 6c6f 622f 6d61 696e 2f43 4841  ks/blob/main/CHA
-00002b00: 4e47 454c 4f47 2e6d 6429 0a37 2e20 496e  NGELOG.md).7. In
-00002b10: 7374 616c 6c20 6070 7265 2d63 6f6d 6d69  stall `pre-commi
-00002b20: 7460 2074 6f20 7065 7266 6f72 6d20 7175  t` to perform qu
-00002b30: 616c 6974 7920 6368 6563 6b73 2070 7269  ality checks pri
-00002b40: 6f72 2074 6f20 636f 6d6d 6974 3a0a 6060  or to commit:.``
-00002b50: 600a 7072 652d 636f 6d6d 6974 2069 6e73  `.pre-commit ins
-00002b60: 7461 6c6c 0a60 6060 0a38 2e20 6067 6974  tall.```.8. `git
-00002b70: 2063 6f6d 6d69 7460 2c20 6067 6974 2070   commit`, `git p
-00002b80: 7573 6860 2c20 616e 6420 6372 6561 7465  ush`, and create
-00002b90: 2061 2070 756c 6c20 7265 7175 6573 740a   a pull request.
+00000050: 6e74 6567 7261 7469 6f6e 7320 7769 7468  ntegrations with
+00000060: 2044 6174 6162 7269 636b 730a 4175 7468   Databricks.Auth
+00000070: 6f72 2d65 6d61 696c 3a20 2250 7265 6665  or-email: "Prefe
+00000080: 6374 2054 6563 686e 6f6c 6f67 6965 732c  ct Technologies,
+00000090: 2049 6e63 2e22 203c 6865 6c70 4070 7265   Inc." <help@pre
+000000a0: 6665 6374 2e69 6f3e 0a4c 6963 656e 7365  fect.io>.License
+000000b0: 3a20 4170 6163 6865 204c 6963 656e 7365  : Apache License
+000000c0: 2032 2e30 0a50 726f 6a65 6374 2d55 524c   2.0.Project-URL
+000000d0: 3a20 486f 6d65 7061 6765 2c20 6874 7470  : Homepage, http
+000000e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f50  s://github.com/P
+000000f0: 7265 6665 6374 4851 2f70 7265 6665 6374  refectHQ/prefect
+00000100: 2f74 7265 652f 6d61 696e 2f73 7263 2f69  /tree/main/src/i
+00000110: 6e74 6567 7261 7469 6f6e 732f 7072 6566  ntegrations/pref
+00000120: 6563 742d 6461 7461 6272 6963 6b73 0a4b  ect-databricks.K
+00000130: 6579 776f 7264 733a 2070 7265 6665 6374  eywords: prefect
+00000140: 0a43 6c61 7373 6966 6965 723a 204e 6174  .Classifier: Nat
+00000150: 7572 616c 204c 616e 6775 6167 6520 3a3a  ural Language ::
+00000160: 2045 6e67 6c69 7368 0a43 6c61 7373 6966   English.Classif
+00000170: 6965 723a 2049 6e74 656e 6465 6420 4175  ier: Intended Au
+00000180: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
+00000190: 7065 7273 0a43 6c61 7373 6966 6965 723a  pers.Classifier:
+000001a0: 2049 6e74 656e 6465 6420 4175 6469 656e   Intended Audien
+000001b0: 6365 203a 3a20 5379 7374 656d 2041 646d  ce :: System Adm
+000001c0: 696e 6973 7472 6174 6f72 730a 436c 6173  inistrators.Clas
+000001d0: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
+000001e0: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+000001f0: 3a3a 2041 7061 6368 6520 536f 6674 7761  :: Apache Softwa
+00000200: 7265 204c 6963 656e 7365 0a43 6c61 7373  re License.Class
+00000210: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000220: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000230: 7974 686f 6e20 3a3a 2033 203a 3a20 4f6e  ython :: 3 :: On
+00000240: 6c79 0a43 6c61 7373 6966 6965 723a 2050  ly.Classifier: P
+00000250: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000260: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000270: 2033 2e38 0a43 6c61 7373 6966 6965 723a   3.8.Classifier:
+00000280: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000290: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000002a0: 3a3a 2033 2e39 0a43 6c61 7373 6966 6965  :: 3.9.Classifie
+000002b0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000002c0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000002d0: 6e20 3a3a 2033 2e31 300a 436c 6173 7369  n :: 3.10.Classi
+000002e0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+000002f0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000300: 7468 6f6e 203a 3a20 332e 3131 0a43 6c61  thon :: 3.11.Cla
+00000310: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000320: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000330: 2050 7974 686f 6e20 3a3a 2033 2e31 320a   Python :: 3.12.
+00000340: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
+00000350: 6320 3a3a 2053 6f66 7477 6172 6520 4465  c :: Software De
+00000360: 7665 6c6f 706d 656e 7420 3a3a 204c 6962  velopment :: Lib
+00000370: 7261 7269 6573 0a52 6571 7569 7265 732d  raries.Requires-
+00000380: 5079 7468 6f6e 3a20 3e3d 332e 380a 4465  Python: >=3.8.De
+00000390: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
+000003a0: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
+000003b0: 6b64 6f77 6e0a 5265 7175 6972 6573 2d44  kdown.Requires-D
+000003c0: 6973 743a 2070 7265 6665 6374 3e3d 322e  ist: prefect>=2.
+000003d0: 3134 2e31 300a 5072 6f76 6964 6573 2d45  14.10.Provides-E
+000003e0: 7874 7261 3a20 6465 760a 5265 7175 6972  xtra: dev.Requir
+000003f0: 6573 2d44 6973 743a 2063 6f76 6572 6167  es-Dist: coverag
+00000400: 653b 2065 7874 7261 203d 3d20 2264 6576  e; extra == "dev
+00000410: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000420: 2069 6e74 6572 726f 6761 7465 3b20 6578   interrogate; ex
+00000430: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
+00000440: 7569 7265 732d 4469 7374 3a20 6d6b 646f  uires-Dist: mkdo
+00000450: 6373 2d67 656e 2d66 696c 6573 3b20 6578  cs-gen-files; ex
+00000460: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
+00000470: 7569 7265 732d 4469 7374 3a20 6d6b 646f  uires-Dist: mkdo
+00000480: 6373 2d6d 6174 6572 6961 6c3b 2065 7874  cs-material; ext
+00000490: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
+000004a0: 6972 6573 2d44 6973 743a 206d 6b64 6f63  ires-Dist: mkdoc
+000004b0: 733b 2065 7874 7261 203d 3d20 2264 6576  s; extra == "dev
+000004c0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+000004d0: 206d 6b64 6f63 7374 7269 6e67 735b 7079   mkdocstrings[py
+000004e0: 7468 6f6e 5d3b 2065 7874 7261 203d 3d20  thon]; extra == 
+000004f0: 2264 6576 220a 5265 7175 6972 6573 2d44  "dev".Requires-D
+00000500: 6973 743a 206d 6f63 6b3b 2070 7974 686f  ist: mock; pytho
+00000510: 6e5f 7665 7273 696f 6e20 3c20 2233 2e38  n_version < "3.8
+00000520: 2220 616e 6420 6578 7472 6120 3d3d 2022  " and extra == "
+00000530: 6465 7622 0a52 6571 7569 7265 732d 4469  dev".Requires-Di
+00000540: 7374 3a20 6d79 7079 3b20 6578 7472 6120  st: mypy; extra 
+00000550: 3d3d 2022 6465 7622 0a52 6571 7569 7265  == "dev".Require
+00000560: 732d 4469 7374 3a20 7069 6c6c 6f77 3b20  s-Dist: pillow; 
+00000570: 6578 7472 6120 3d3d 2022 6465 7622 0a52  extra == "dev".R
+00000580: 6571 7569 7265 732d 4469 7374 3a20 7072  equires-Dist: pr
+00000590: 652d 636f 6d6d 6974 3b20 6578 7472 6120  e-commit; extra 
+000005a0: 3d3d 2022 6465 7622 0a52 6571 7569 7265  == "dev".Require
+000005b0: 732d 4469 7374 3a20 7079 7465 7374 2d61  s-Dist: pytest-a
+000005c0: 7379 6e63 696f 3b20 6578 7472 6120 3d3d  syncio; extra ==
+000005d0: 2022 6465 7622 0a52 6571 7569 7265 732d   "dev".Requires-
+000005e0: 4469 7374 3a20 7079 7465 7374 3b20 6578  Dist: pytest; ex
+000005f0: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
+00000600: 7569 7265 732d 4469 7374 3a20 7079 7465  uires-Dist: pyte
+00000610: 7374 2d78 6469 7374 3b20 6578 7472 6120  st-xdist; extra 
+00000620: 3d3d 2022 6465 7622 0a52 6571 7569 7265  == "dev".Require
+00000630: 732d 4469 7374 3a20 7265 7370 783b 2065  s-Dist: respx; e
+00000640: 7874 7261 203d 3d20 2264 6576 220a 0a23  xtra == "dev"..#
+00000650: 2070 7265 6665 6374 2d64 6174 6162 7269   prefect-databri
+00000660: 636b 730a 0a56 6973 6974 2074 6865 2066  cks..Visit the f
+00000670: 756c 6c20 646f 6373 205b 6865 7265 5d28  ull docs [here](
+00000680: 6874 7470 733a 2f2f 5072 6566 6563 7448  https://PrefectH
+00000690: 512e 6769 7468 7562 2e69 6f2f 7072 6566  Q.github.io/pref
+000006a0: 6563 742d 6461 7461 6272 6963 6b73 2920  ect-databricks) 
+000006b0: 746f 2073 6565 2061 6464 6974 696f 6e61  to see additiona
+000006c0: 6c20 6578 616d 706c 6573 2061 6e64 2074  l examples and t
+000006d0: 6865 2041 5049 2072 6566 6572 656e 6365  he API reference
+000006e0: 2e0a 200a 3c70 2061 6c69 676e 3d22 6365  .. .<p align="ce
+000006f0: 6e74 6572 223e 0a20 2020 203c 6120 6872  nter">.    <a hr
+00000700: 6566 3d22 6874 7470 733a 2f2f 7079 7069  ef="https://pypi
+00000710: 2e70 7974 686f 6e2e 6f72 672f 7079 7069  .python.org/pypi
+00000720: 2f70 7265 6665 6374 2d64 6174 6162 7269  /prefect-databri
+00000730: 636b 732f 2220 616c 743d 2250 7950 4920  cks/" alt="PyPI 
+00000740: 7665 7273 696f 6e22 3e0a 2020 2020 2020  version">.      
+00000750: 2020 3c69 6d67 2061 6c74 3d22 5079 5049    <img alt="PyPI
+00000760: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
+00000770: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000780: 7069 2f76 2f70 7265 6665 6374 2d64 6174  pi/v/prefect-dat
+00000790: 6162 7269 636b 733f 636f 6c6f 723d 3030  abricks?color=00
+000007a0: 3532 4646 266c 6162 656c 436f 6c6f 723d  52FF&labelColor=
+000007b0: 3039 3034 3232 223e 3c2f 613e 0a20 2020  090422"></a>.   
+000007c0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000007d0: 2f2f 7065 7079 2e74 6563 682f 6261 6467  //pepy.tech/badg
+000007e0: 652f 7072 6566 6563 742d 6461 7461 6272  e/prefect-databr
+000007f0: 6963 6b73 2f22 2061 6c74 3d22 446f 776e  icks/" alt="Down
+00000800: 6c6f 6164 7322 3e0a 2020 2020 2020 2020  loads">.        
+00000810: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000820: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000830: 2f70 7970 692f 646d 2f70 7265 6665 6374  /pypi/dm/prefect
+00000840: 2d64 6174 6162 7269 636b 733f 636f 6c6f  -databricks?colo
+00000850: 723d 3030 3532 4646 266c 6162 656c 436f  r=0052FF&labelCo
+00000860: 6c6f 723d 3039 3034 3232 2220 2f3e 3c2f  lor=090422" /></
+00000870: 613e 0a20 2020 203c 6120 6872 6566 3d22  a>.    <a href="
+00000880: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000890: 6f6d 2f50 7265 6665 6374 4851 2f70 7265  om/PrefectHQ/pre
+000008a0: 6665 6374 2d64 6174 6162 7269 636b 732f  fect-databricks/
+000008b0: 7075 6c73 6522 2061 6c74 3d22 4163 7469  pulse" alt="Acti
+000008c0: 7669 7479 223e 0a3c 2f70 3e0a 0a23 2320  vity">.</p>..## 
+000008d0: 5765 6c63 6f6d 6521 0a0a 5072 6566 6563  Welcome!..Prefec
+000008e0: 7420 696e 7465 6772 6174 696f 6e73 2066  t integrations f
+000008f0: 6f72 2069 6e74 6572 6163 7469 6e67 2077  or interacting w
+00000900: 6974 6820 4461 7461 6272 6963 6b73 0a0a  ith Databricks..
+00000910: 5468 6520 7461 736b 7320 7769 7468 696e  The tasks within
+00000920: 2074 6869 7320 636f 6c6c 6563 7469 6f6e   this collection
+00000930: 2077 6572 6520 6372 6561 7465 6420 6279   were created by
+00000940: 2061 2063 6f64 6520 6765 6e65 7261 746f   a code generato
+00000950: 7220 7573 696e 6720 7468 6520 7365 7276  r using the serv
+00000960: 6963 6527 7320 4f70 656e 4150 4920 7370  ice's OpenAPI sp
+00000970: 6563 2e0a 0a54 6865 2073 6572 7669 6365  ec...The service
+00000980: 2773 2052 4553 5420 4150 4920 646f 6375  's REST API docu
+00000990: 6d65 6e74 6174 696f 6e20 6361 6e20 6265  mentation can be
+000009a0: 2066 6f75 6e64 205b 6865 7265 5d28 6874   found [here](ht
+000009b0: 7470 733a 2f2f 646f 6373 2e64 6174 6162  tps://docs.datab
+000009c0: 7269 636b 732e 636f 6d2f 6465 762d 746f  ricks.com/dev-to
+000009d0: 6f6c 732f 6170 692f 6c61 7465 7374 2f69  ols/api/latest/i
+000009e0: 6e64 6578 2e68 746d 6c29 2e0a 0a23 2320  ndex.html)...## 
+000009f0: 4765 7474 696e 6720 5374 6172 7465 640a  Getting Started.
+00000a00: 0a23 2323 2050 7974 686f 6e20 7365 7475  .### Python setu
+00000a10: 700a 0a52 6571 7569 7265 7320 616e 2069  p..Requires an i
+00000a20: 6e73 7461 6c6c 6174 696f 6e20 6f66 2050  nstallation of P
+00000a30: 7974 686f 6e20 332e 372b 2e0a 0a57 6520  ython 3.7+...We 
+00000a40: 7265 636f 6d6d 656e 6420 7573 696e 6720  recommend using 
+00000a50: 6120 5079 7468 6f6e 2076 6972 7475 616c  a Python virtual
+00000a60: 2065 6e76 6972 6f6e 6d65 6e74 206d 616e   environment man
+00000a70: 6167 6572 2073 7563 6820 6173 2070 6970  ager such as pip
+00000a80: 656e 762c 2063 6f6e 6461 206f 7220 7669  env, conda or vi
+00000a90: 7274 7561 6c65 6e76 2e0a 0a54 6865 7365  rtualenv...These
+00000aa0: 2074 6173 6b73 2061 7265 2064 6573 6967   tasks are desig
+00000ab0: 6e65 6420 746f 2077 6f72 6b20 7769 7468  ned to work with
+00000ac0: 2050 7265 6665 6374 2032 2e20 466f 7220   Prefect 2. For 
+00000ad0: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
+00000ae0: 2061 626f 7574 2068 6f77 2074 6f20 7573   about how to us
+00000af0: 6520 5072 6566 6563 742c 2070 6c65 6173  e Prefect, pleas
+00000b00: 6520 7265 6665 7220 746f 2074 6865 205b  e refer to the [
+00000b10: 5072 6566 6563 7420 646f 6375 6d65 6e74  Prefect document
+00000b20: 6174 696f 6e5d 2868 7474 7073 3a2f 2f6f  ation](https://o
+00000b30: 7269 6f6e 2d64 6f63 732e 7072 6566 6563  rion-docs.prefec
+00000b40: 742e 696f 2f29 2e0a 0a23 2323 2049 6e73  t.io/)...### Ins
+00000b50: 7461 6c6c 6174 696f 6e0a 0a49 6e73 7461  tallation..Insta
+00000b60: 6c6c 2060 7072 6566 6563 742d 6461 7461  ll `prefect-data
+00000b70: 6272 6963 6b73 6020 7769 7468 2060 7069  bricks` with `pi
+00000b80: 7060 3a0a 0a60 6060 6261 7368 0a70 6970  p`:..```bash.pip
+00000b90: 2069 6e73 7461 6c6c 2070 7265 6665 6374   install prefect
+00000ba0: 2d64 6174 6162 7269 636b 730a 6060 600a  -databricks.```.
+00000bb0: 0a41 206c 6973 7420 6f66 2061 7661 696c  .A list of avail
+00000bc0: 6162 6c65 2062 6c6f 636b 7320 696e 2060  able blocks in `
+00000bd0: 7072 6566 6563 742d 6461 7461 6272 6963  prefect-databric
+00000be0: 6b73 6020 616e 6420 7468 6569 7220 7365  ks` and their se
+00000bf0: 7475 7020 696e 7374 7275 6374 696f 6e73  tup instructions
+00000c00: 2063 616e 2062 6520 666f 756e 6420 5b68   can be found [h
+00000c10: 6572 655d 2868 7474 7073 3a2f 2f50 7265  ere](https://Pre
+00000c20: 6665 6374 4851 2e67 6974 6875 622e 696f  fectHQ.github.io
+00000c30: 2f70 7265 6665 6374 2d64 6174 6162 7269  /prefect-databri
+00000c40: 636b 732f 2362 6c6f 636b 732d 6361 7461  cks/#blocks-cata
+00000c50: 6c6f 6729 2e0a 0a23 2323 204c 6973 7473  log)...### Lists
+00000c60: 206a 6f62 7320 6f6e 2074 6865 2044 6174   jobs on the Dat
+00000c70: 6162 7269 636b 7320 696e 7374 616e 6365  abricks instance
+00000c80: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+00000c90: 2070 7265 6665 6374 2069 6d70 6f72 7420   prefect import 
+00000ca0: 666c 6f77 0a66 726f 6d20 7072 6566 6563  flow.from prefec
+00000cb0: 745f 6461 7461 6272 6963 6b73 2069 6d70  t_databricks imp
+00000cc0: 6f72 7420 4461 7461 6272 6963 6b73 4372  ort DatabricksCr
+00000cd0: 6564 656e 7469 616c 730a 6672 6f6d 2070  edentials.from p
+00000ce0: 7265 6665 6374 5f64 6174 6162 7269 636b  refect_databrick
+00000cf0: 732e 6a6f 6273 2069 6d70 6f72 7420 6a6f  s.jobs import jo
+00000d00: 6273 5f6c 6973 740a 0a0a 4066 6c6f 770a  bs_list...@flow.
+00000d10: 6465 6620 6578 616d 706c 655f 6578 6563  def example_exec
+00000d20: 7574 655f 656e 6470 6f69 6e74 5f66 6c6f  ute_endpoint_flo
+00000d30: 7728 293a 0a20 2020 2064 6174 6162 7269  w():.    databri
+00000d40: 636b 735f 6372 6564 656e 7469 616c 7320  cks_credentials 
+00000d50: 3d20 4461 7461 6272 6963 6b73 4372 6564  = DatabricksCred
+00000d60: 656e 7469 616c 732e 6c6f 6164 2822 6d79  entials.load("my
+00000d70: 2d62 6c6f 636b 2229 0a20 2020 206a 6f62  -block").    job
+00000d80: 7320 3d20 6a6f 6273 5f6c 6973 7428 0a20  s = jobs_list(. 
+00000d90: 2020 2020 2020 2064 6174 6162 7269 636b         databrick
+00000da0: 735f 6372 6564 656e 7469 616c 732c 0a20  s_credentials,. 
+00000db0: 2020 2020 2020 206c 696d 6974 3d35 0a20         limit=5. 
+00000dc0: 2020 2029 0a20 2020 2072 6574 7572 6e20     ).    return 
+00000dd0: 6a6f 6273 0a0a 6578 616d 706c 655f 6578  jobs..example_ex
+00000de0: 6563 7574 655f 656e 6470 6f69 6e74 5f66  ecute_endpoint_f
+00000df0: 6c6f 7728 290a 6060 600a 0a23 2323 2055  low().```..### U
+00000e00: 7365 2060 7769 7468 5f6f 7074 696f 6e73  se `with_options
+00000e10: 6020 746f 2063 7573 746f 6d69 7a65 206f  ` to customize o
+00000e20: 7074 696f 6e73 206f 6e20 616e 7920 6578  ptions on any ex
+00000e30: 6973 7469 6e67 2074 6173 6b20 6f72 2066  isting task or f
+00000e40: 6c6f 770a 0a60 6060 7079 7468 6f6e 0a63  low..```python.c
+00000e50: 7573 746f 6d5f 6578 616d 706c 655f 6578  ustom_example_ex
+00000e60: 6563 7574 655f 656e 6470 6f69 6e74 5f66  ecute_endpoint_f
+00000e70: 6c6f 7720 3d20 6578 616d 706c 655f 6578  low = example_ex
+00000e80: 6563 7574 655f 656e 6470 6f69 6e74 5f66  ecute_endpoint_f
+00000e90: 6c6f 772e 7769 7468 5f6f 7074 696f 6e73  low.with_options
+00000ea0: 280a 2020 2020 6e61 6d65 3d22 4d79 2063  (.    name="My c
+00000eb0: 7573 746f 6d20 666c 6f77 206e 616d 6522  ustom flow name"
+00000ec0: 2c0a 2020 2020 7265 7472 6965 733d 322c  ,.    retries=2,
+00000ed0: 0a20 2020 2072 6574 7279 5f64 656c 6179  .    retry_delay
+00000ee0: 5f73 6563 6f6e 6473 3d31 302c 0a29 0a60  _seconds=10,.).`
+00000ef0: 6060 0a0a 2323 2320 4c61 756e 6368 2061  ``..### Launch a
+00000f00: 206e 6577 2063 6c75 7374 6572 2061 6e64   new cluster and
+00000f10: 2072 756e 2061 2044 6174 6162 7269 636b   run a Databrick
+00000f20: 7320 6e6f 7465 626f 6f6b 0a0a 4e6f 7465  s notebook..Note
+00000f30: 626f 6f6b 206e 616d 6564 2060 6578 616d  book named `exam
+00000f40: 706c 652e 6970 796e 6260 206f 6e20 4461  ple.ipynb` on Da
+00000f50: 7461 6272 6963 6b73 2077 6869 6368 2061  tabricks which a
+00000f60: 6363 6570 7473 2061 206e 616d 6520 7061  ccepts a name pa
+00000f70: 7261 6d65 7465 723a 0a0a 6060 6070 7974  rameter:..```pyt
+00000f80: 686f 6e0a 6e61 6d65 203d 2064 6275 7469  hon.name = dbuti
+00000f90: 6c73 2e77 6964 6765 7473 2e67 6574 2822  ls.widgets.get("
+00000fa0: 6e61 6d65 2229 0a6d 6573 7361 6765 203d  name").message =
+00000fb0: 2066 2244 6f6e 2774 2077 6f72 7279 207b   f"Don't worry {
+00000fc0: 6e61 6d65 7d2c 2049 2067 6f74 2079 6f75  name}, I got you
+00000fd0: 7220 7265 7175 6573 7421 2057 656c 636f  r request! Welco
+00000fe0: 6d65 2074 6f20 7072 6566 6563 742d 6461  me to prefect-da
+00000ff0: 7461 6272 6963 6b73 2122 0a70 7269 6e74  tabricks!".print
+00001000: 286d 6573 7361 6765 290a 6060 600a 0a50  (message).```..P
+00001010: 7265 6665 6374 2066 6c6f 7720 7468 6174  refect flow that
+00001020: 206c 6175 6e63 6865 7320 6120 6e65 7720   launches a new 
+00001030: 636c 7573 7465 7220 746f 2072 756e 2060  cluster to run `
+00001040: 6578 616d 706c 652e 6970 796e 6260 3a0a  example.ipynb`:.
+00001050: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
+00001060: 7072 6566 6563 7420 696d 706f 7274 2066  prefect import f
+00001070: 6c6f 770a 6672 6f6d 2070 7265 6665 6374  low.from prefect
+00001080: 5f64 6174 6162 7269 636b 7320 696d 706f  _databricks impo
+00001090: 7274 2044 6174 6162 7269 636b 7343 7265  rt DatabricksCre
+000010a0: 6465 6e74 6961 6c73 0a66 726f 6d20 7072  dentials.from pr
+000010b0: 6566 6563 745f 6461 7461 6272 6963 6b73  efect_databricks
+000010c0: 2e6a 6f62 7320 696d 706f 7274 206a 6f62  .jobs import job
+000010d0: 735f 7275 6e73 5f73 7562 6d69 740a 6672  s_runs_submit.fr
+000010e0: 6f6d 2070 7265 6665 6374 5f64 6174 6162  om prefect_datab
+000010f0: 7269 636b 732e 6d6f 6465 6c73 2e6a 6f62  ricks.models.job
+00001100: 7320 696d 706f 7274 2028 0a20 2020 2041  s import (.    A
+00001110: 7574 6f53 6361 6c65 2c0a 2020 2020 4177  utoScale,.    Aw
+00001120: 7341 7474 7269 6275 7465 732c 0a20 2020  sAttributes,.   
+00001130: 204a 6f62 5461 736b 5365 7474 696e 6773   JobTaskSettings
+00001140: 2c0a 2020 2020 4e6f 7465 626f 6f6b 5461  ,.    NotebookTa
+00001150: 736b 2c0a 2020 2020 4e65 7743 6c75 7374  sk,.    NewClust
+00001160: 6572 2c0a 290a 0a0a 4066 6c6f 770a 6465  er,.)...@flow.de
+00001170: 6620 6a6f 6273 5f72 756e 735f 7375 626d  f jobs_runs_subm
+00001180: 6974 5f66 6c6f 7728 6e6f 7465 626f 6f6b  it_flow(notebook
+00001190: 5f70 6174 682c 202a 2a62 6173 655f 7061  _path, **base_pa
+000011a0: 7261 6d65 7465 7273 293a 0a20 2020 2064  rameters):.    d
+000011b0: 6174 6162 7269 636b 735f 6372 6564 656e  atabricks_creden
+000011c0: 7469 616c 7320 3d20 4461 7461 6272 6963  tials = Databric
+000011d0: 6b73 4372 6564 656e 7469 616c 732e 6c6f  ksCredentials.lo
+000011e0: 6164 2822 6d79 2d62 6c6f 636b 2229 0a0a  ad("my-block")..
+000011f0: 2020 2020 2320 7370 6563 6966 7920 6e65      # specify ne
+00001200: 7720 636c 7573 7465 7220 7365 7474 696e  w cluster settin
+00001210: 6773 0a20 2020 2061 7773 5f61 7474 7269  gs.    aws_attri
+00001220: 6275 7465 7320 3d20 4177 7341 7474 7269  butes = AwsAttri
+00001230: 6275 7465 7328 0a20 2020 2020 2020 2061  butes(.        a
+00001240: 7661 696c 6162 696c 6974 793d 2253 504f  vailability="SPO
+00001250: 5422 2c0a 2020 2020 2020 2020 7a6f 6e65  T",.        zone
+00001260: 5f69 643d 2275 732d 7765 7374 2d32 6122  _id="us-west-2a"
+00001270: 2c0a 2020 2020 2020 2020 6562 735f 766f  ,.        ebs_vo
+00001280: 6c75 6d65 5f74 7970 653d 2247 454e 4552  lume_type="GENER
+00001290: 414c 5f50 5552 504f 5345 5f53 5344 222c  AL_PURPOSE_SSD",
+000012a0: 0a20 2020 2020 2020 2065 6273 5f76 6f6c  .        ebs_vol
+000012b0: 756d 655f 636f 756e 743d 332c 0a20 2020  ume_count=3,.   
+000012c0: 2020 2020 2065 6273 5f76 6f6c 756d 655f       ebs_volume_
+000012d0: 7369 7a65 3d31 3030 2c0a 2020 2020 290a  size=100,.    ).
+000012e0: 2020 2020 6175 746f 5f73 6361 6c65 203d      auto_scale =
+000012f0: 2041 7574 6f53 6361 6c65 286d 696e 5f77   AutoScale(min_w
+00001300: 6f72 6b65 7273 3d31 2c20 6d61 785f 776f  orkers=1, max_wo
+00001310: 726b 6572 733d 3229 0a20 2020 206e 6577  rkers=2).    new
+00001320: 5f63 6c75 7374 6572 203d 204e 6577 436c  _cluster = NewCl
+00001330: 7573 7465 7228 0a20 2020 2020 2020 2061  uster(.        a
+00001340: 7773 5f61 7474 7269 6275 7465 733d 6177  ws_attributes=aw
+00001350: 735f 6174 7472 6962 7574 6573 2c0a 2020  s_attributes,.  
+00001360: 2020 2020 2020 6175 746f 7363 616c 653d        autoscale=
+00001370: 6175 746f 5f73 6361 6c65 2c0a 2020 2020  auto_scale,.    
+00001380: 2020 2020 6e6f 6465 5f74 7970 655f 6964      node_type_id
+00001390: 3d22 6d34 2e6c 6172 6765 222c 0a20 2020  ="m4.large",.   
+000013a0: 2020 2020 2073 7061 726b 5f76 6572 7369       spark_versi
+000013b0: 6f6e 3d22 3130 2e34 2e78 2d73 6361 6c61  on="10.4.x-scala
+000013c0: 322e 3132 222c 0a20 2020 2020 2020 2073  2.12",.        s
+000013d0: 7061 726b 5f63 6f6e 663d 7b22 7370 6172  park_conf={"spar
+000013e0: 6b2e 7370 6563 756c 6174 696f 6e22 3a20  k.speculation": 
+000013f0: 5472 7565 7d2c 0a20 2020 2029 0a0a 2020  True},.    )..  
+00001400: 2020 2320 7370 6563 6966 7920 6e6f 7465    # specify note
+00001410: 626f 6f6b 2074 6f20 7573 6520 616e 6420  book to use and 
+00001420: 7061 7261 6d65 7465 7273 2074 6f20 7061  parameters to pa
+00001430: 7373 0a20 2020 206e 6f74 6562 6f6f 6b5f  ss.    notebook_
+00001440: 7461 736b 203d 204e 6f74 6562 6f6f 6b54  task = NotebookT
+00001450: 6173 6b28 0a20 2020 2020 2020 206e 6f74  ask(.        not
+00001460: 6562 6f6f 6b5f 7061 7468 3d6e 6f74 6562  ebook_path=noteb
+00001470: 6f6f 6b5f 7061 7468 2c0a 2020 2020 2020  ook_path,.      
+00001480: 2020 6261 7365 5f70 6172 616d 6574 6572    base_parameter
+00001490: 733d 6261 7365 5f70 6172 616d 6574 6572  s=base_parameter
+000014a0: 732c 0a20 2020 2029 0a0a 2020 2020 2320  s,.    )..    # 
+000014b0: 636f 6d70 696c 6520 6a6f 6220 7461 736b  compile job task
+000014c0: 2073 6574 7469 6e67 730a 2020 2020 6a6f   settings.    jo
+000014d0: 625f 7461 736b 5f73 6574 7469 6e67 7320  b_task_settings 
+000014e0: 3d20 4a6f 6254 6173 6b53 6574 7469 6e67  = JobTaskSetting
+000014f0: 7328 0a20 2020 2020 2020 206e 6577 5f63  s(.        new_c
+00001500: 6c75 7374 6572 3d6e 6577 5f63 6c75 7374  luster=new_clust
+00001510: 6572 2c0a 2020 2020 2020 2020 6e6f 7465  er,.        note
+00001520: 626f 6f6b 5f74 6173 6b3d 6e6f 7465 626f  book_task=notebo
+00001530: 6f6b 5f74 6173 6b2c 0a20 2020 2020 2020  ok_task,.       
+00001540: 2074 6173 6b5f 6b65 793d 2270 7265 6665   task_key="prefe
+00001550: 6374 2d74 6173 6b22 0a20 2020 2029 0a0a  ct-task".    )..
+00001560: 2020 2020 7275 6e20 3d20 6a6f 6273 5f72      run = jobs_r
+00001570: 756e 735f 7375 626d 6974 280a 2020 2020  uns_submit(.    
+00001580: 2020 2020 6461 7461 6272 6963 6b73 5f63      databricks_c
+00001590: 7265 6465 6e74 6961 6c73 3d64 6174 6162  redentials=datab
+000015a0: 7269 636b 735f 6372 6564 656e 7469 616c  ricks_credential
+000015b0: 732c 0a20 2020 2020 2020 2072 756e 5f6e  s,.        run_n
+000015c0: 616d 653d 2270 7265 6665 6374 2d6a 6f62  ame="prefect-job
+000015d0: 222c 0a20 2020 2020 2020 2074 6173 6b73  ",.        tasks
+000015e0: 3d5b 6a6f 625f 7461 736b 5f73 6574 7469  =[job_task_setti
+000015f0: 6e67 735d 0a20 2020 2029 0a0a 2020 2020  ngs].    )..    
+00001600: 7265 7475 726e 2072 756e 0a0a 0a6a 6f62  return run...job
+00001610: 735f 7275 6e73 5f73 7562 6d69 745f 666c  s_runs_submit_fl
+00001620: 6f77 2822 2f55 7365 7273 2f75 7365 726e  ow("/Users/usern
+00001630: 616d 6540 676d 6169 6c2e 636f 6d2f 6578  ame@gmail.com/ex
+00001640: 616d 706c 652e 6970 796e 6222 2c20 6e61  ample.ipynb", na
+00001650: 6d65 3d22 4d61 7276 696e 2229 0a60 6060  me="Marvin").```
+00001660: 0a0a 4e6f 7465 2c20 696e 7374 6561 6420  ..Note, instead 
+00001670: 6f66 2075 7369 6e67 2074 6865 2062 7569  of using the bui
+00001680: 6c74 2d69 6e20 6d6f 6465 6c73 2c20 796f  lt-in models, yo
+00001690: 7520 6d61 7920 616c 736f 2069 6e70 7574  u may also input
+000016a0: 2076 616c 6964 204a 534f 4e2e 2046 6f72   valid JSON. For
+000016b0: 2065 7861 6d70 6c65 2c20 6041 7574 6f53   example, `AutoS
+000016c0: 6361 6c65 286d 696e 5f77 6f72 6b65 7273  cale(min_workers
+000016d0: 3d31 2c20 6d61 785f 776f 726b 6572 733d  =1, max_workers=
+000016e0: 3229 6020 6973 2065 7175 6976 616c 656e  2)` is equivalen
+000016f0: 7420 746f 2060 7b22 6d69 6e5f 776f 726b  t to `{"min_work
+00001700: 6572 7322 3a20 312c 2022 6d61 785f 776f  ers": 1, "max_wo
+00001710: 726b 6572 7322 3a20 327d 602e 0a0a 466f  rkers": 2}`...Fo
+00001720: 7220 6d6f 7265 2074 6970 7320 6f6e 2068  r more tips on h
+00001730: 6f77 2074 6f20 7573 6520 7461 736b 7320  ow to use tasks 
+00001740: 616e 6420 666c 6f77 7320 696e 2061 2043  and flows in a C
+00001750: 6f6c 6c65 6374 696f 6e2c 2063 6865 636b  ollection, check
+00001760: 206f 7574 205b 5573 696e 6720 436f 6c6c   out [Using Coll
+00001770: 6563 7469 6f6e 735d 2868 7474 7073 3a2f  ections](https:/
+00001780: 2f6f 7269 6f6e 2d64 6f63 732e 7072 6566  /orion-docs.pref
+00001790: 6563 742e 696f 2f63 6f6c 6c65 6374 696f  ect.io/collectio
+000017a0: 6e73 2f75 7361 6765 2f29 210a 0a23 2320  ns/usage/)!..## 
+000017b0: 5265 736f 7572 6365 730a 0a49 6620 796f  Resources..If yo
+000017c0: 7520 656e 636f 756e 7465 7220 616e 7920  u encounter any 
+000017d0: 6275 6773 2077 6869 6c65 2075 7369 6e67  bugs while using
+000017e0: 2060 7072 6566 6563 742d 6461 7461 6272   `prefect-databr
+000017f0: 6963 6b73 602c 2066 6565 6c20 6672 6565  icks`, feel free
+00001800: 2074 6f20 6f70 656e 2061 6e20 6973 7375   to open an issu
+00001810: 6520 696e 2074 6865 205b 7072 6566 6563  e in the [prefec
+00001820: 742d 6461 7461 6272 6963 6b73 5d28 6874  t-databricks](ht
+00001830: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001840: 2f50 7265 6665 6374 4851 2f70 7265 6665  /PrefectHQ/prefe
+00001850: 6374 2d64 6174 6162 7269 636b 7329 2072  ct-databricks) r
+00001860: 6570 6f73 6974 6f72 792e 0a0a 4966 2079  epository...If y
+00001870: 6f75 2068 6176 6520 616e 7920 7175 6573  ou have any ques
+00001880: 7469 6f6e 7320 6f72 2069 7373 7565 7320  tions or issues 
+00001890: 7768 696c 6520 7573 696e 6720 6070 7265  while using `pre
+000018a0: 6665 6374 2d64 6174 6162 7269 636b 7360  fect-databricks`
+000018b0: 2c20 796f 7520 6361 6e20 6669 6e64 2068  , you can find h
+000018c0: 656c 7020 696e 2065 6974 6865 7220 7468  elp in either th
+000018d0: 6520 5b50 7265 6665 6374 2044 6973 636f  e [Prefect Disco
+000018e0: 7572 7365 2066 6f72 756d 5d28 6874 7470  urse forum](http
+000018f0: 733a 2f2f 6469 7363 6f75 7273 652e 7072  s://discourse.pr
+00001900: 6566 6563 742e 696f 2f29 206f 7220 7468  efect.io/) or th
+00001910: 6520 5b50 7265 6665 6374 2053 6c61 636b  e [Prefect Slack
+00001920: 2063 6f6d 6d75 6e69 7479 5d28 6874 7470   community](http
+00001930: 733a 2f2f 7072 6566 6563 742e 696f 2f73  s://prefect.io/s
+00001940: 6c61 636b 292e 0a0a 4665 656c 2066 7265  lack)...Feel fre
+00001950: 6520 746f 2073 7461 7220 6f72 2077 6174  e to star or wat
+00001960: 6368 205b 6070 7265 6665 6374 2d64 6174  ch [`prefect-dat
+00001970: 6162 7269 636b 7360 5d28 6874 7470 733a  abricks`](https:
+00001980: 2f2f 6769 7468 7562 2e63 6f6d 2f50 7265  //github.com/Pre
+00001990: 6665 6374 4851 2f70 7265 6665 6374 2d64  fectHQ/prefect-d
+000019a0: 6174 6162 7269 636b 7329 2066 6f72 2075  atabricks) for u
+000019b0: 7064 6174 6573 2074 6f6f 210a 0a23 2320  pdates too!..## 
+000019c0: 436f 6e74 7269 6275 7469 6e67 0a0a 4966  Contributing..If
+000019d0: 2079 6f75 2764 206c 696b 6520 746f 2068   you'd like to h
+000019e0: 656c 7020 636f 6e74 7269 6275 7465 2074  elp contribute t
+000019f0: 6f20 6669 7820 616e 2069 7373 7565 206f  o fix an issue o
+00001a00: 7220 6164 6420 6120 6665 6174 7572 6520  r add a feature 
+00001a10: 746f 2060 7072 6566 6563 742d 6461 7461  to `prefect-data
+00001a20: 6272 6963 6b73 602c 2070 6c65 6173 6520  bricks`, please 
+00001a30: 5b70 726f 706f 7365 2063 6861 6e67 6573  [propose changes
+00001a40: 2074 6872 6f75 6768 2061 2070 756c 6c20   through a pull 
+00001a50: 7265 7175 6573 7420 6672 6f6d 2061 2066  request from a f
+00001a60: 6f72 6b20 6f66 2074 6865 2072 6570 6f73  ork of the repos
+00001a70: 6974 6f72 795d 2868 7474 7073 3a2f 2f64  itory](https://d
+00001a80: 6f63 732e 6769 7468 7562 2e63 6f6d 2f65  ocs.github.com/e
+00001a90: 6e2f 7075 6c6c 2d72 6571 7565 7374 732f  n/pull-requests/
+00001aa0: 636f 6c6c 6162 6f72 6174 696e 672d 7769  collaborating-wi
+00001ab0: 7468 2d70 756c 6c2d 7265 7175 6573 7473  th-pull-requests
+00001ac0: 2f70 726f 706f 7369 6e67 2d63 6861 6e67  /proposing-chang
+00001ad0: 6573 2d74 6f2d 796f 7572 2d77 6f72 6b2d  es-to-your-work-
+00001ae0: 7769 7468 2d70 756c 6c2d 7265 7175 6573  with-pull-reques
+00001af0: 7473 2f63 7265 6174 696e 672d 612d 7075  ts/creating-a-pu
+00001b00: 6c6c 2d72 6571 7565 7374 2d66 726f 6d2d  ll-request-from-
+00001b10: 612d 666f 726b 292e 0a0a 4865 7265 2061  a-fork)...Here a
+00001b20: 7265 2074 6865 2073 7465 7073 3a0a 312e  re the steps:.1.
+00001b30: 205b 466f 726b 2074 6865 2072 6570 6f73   [Fork the repos
+00001b40: 6974 6f72 795d 2868 7474 7073 3a2f 2f64  itory](https://d
+00001b50: 6f63 732e 6769 7468 7562 2e63 6f6d 2f65  ocs.github.com/e
+00001b60: 6e2f 6765 742d 7374 6172 7465 642f 7175  n/get-started/qu
+00001b70: 6963 6b73 7461 7274 2f66 6f72 6b2d 612d  ickstart/fork-a-
+00001b80: 7265 706f 2366 6f72 6b69 6e67 2d61 2d72  repo#forking-a-r
+00001b90: 6570 6f73 6974 6f72 7929 0a32 2e20 5b43  epository).2. [C
+00001ba0: 6c6f 6e65 2074 6865 2066 6f72 6b65 6420  lone the forked 
+00001bb0: 7265 706f 7369 746f 7279 5d28 6874 7470  repository](http
+00001bc0: 733a 2f2f 646f 6373 2e67 6974 6875 622e  s://docs.github.
+00001bd0: 636f 6d2f 656e 2f67 6574 2d73 7461 7274  com/en/get-start
+00001be0: 6564 2f71 7569 636b 7374 6172 742f 666f  ed/quickstart/fo
+00001bf0: 726b 2d61 2d72 6570 6f23 636c 6f6e 696e  rk-a-repo#clonin
+00001c00: 672d 796f 7572 2d66 6f72 6b65 642d 7265  g-your-forked-re
+00001c10: 706f 7369 746f 7279 290a 332e 2049 6e73  pository).3. Ins
+00001c20: 7461 6c6c 2074 6865 2072 6570 6f73 6974  tall the reposit
+00001c30: 6f72 7920 616e 6420 6974 7320 6465 7065  ory and its depe
+00001c40: 6e64 656e 6369 6573 3a0a 6060 600a 7069  ndencies:.```.pi
+00001c50: 7020 696e 7374 616c 6c20 2d65 2022 2e5b  p install -e ".[
+00001c60: 6465 765d 220a 6060 600a 342e 204d 616b  dev]".```.4. Mak
+00001c70: 6520 6465 7369 7265 6420 6368 616e 6765  e desired change
+00001c80: 730a 352e 2041 6464 2074 6573 7473 0a36  s.5. Add tests.6
+00001c90: 2e20 496e 7365 7274 2061 6e20 656e 7472  . Insert an entr
+00001ca0: 7920 746f 205b 4348 414e 4745 4c4f 472e  y to [CHANGELOG.
+00001cb0: 6d64 5d28 6874 7470 733a 2f2f 6769 7468  md](https://gith
+00001cc0: 7562 2e63 6f6d 2f50 7265 6665 6374 4851  ub.com/PrefectHQ
+00001cd0: 2f70 7265 6665 6374 2d64 6174 6162 7269  /prefect-databri
+00001ce0: 636b 732f 626c 6f62 2f6d 6169 6e2f 4348  cks/blob/main/CH
+00001cf0: 414e 4745 4c4f 472e 6d64 290a 372e 2049  ANGELOG.md).7. I
+00001d00: 6e73 7461 6c6c 2060 7072 652d 636f 6d6d  nstall `pre-comm
+00001d10: 6974 6020 746f 2070 6572 666f 726d 2071  it` to perform q
+00001d20: 7561 6c69 7479 2063 6865 636b 7320 7072  uality checks pr
+00001d30: 696f 7220 746f 2063 6f6d 6d69 743a 0a60  ior to commit:.`
+00001d40: 6060 0a70 7265 2d63 6f6d 6d69 7420 696e  ``.pre-commit in
+00001d50: 7374 616c 6c0a 6060 600a 382e 2060 6769  stall.```.8. `gi
+00001d60: 7420 636f 6d6d 6974 602c 2060 6769 7420  t commit`, `git 
+00001d70: 7075 7368 602c 2061 6e64 2063 7265 6174  push`, and creat
+00001d80: 6520 6120 7075 6c6c 2072 6571 7565 7374  e a pull request
+00001d90: 0a                                       .
```

### Comparing `prefect-databricks-0.2.3/prefect_databricks.egg-info/SOURCES.txt` & `prefect_databricks-0.2.4/prefect_databricks.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,26 @@
-LICENSE
-MANIFEST.in
 README.md
-requirements-dev.txt
-requirements.txt
-setup.cfg
-setup.py
-versioneer.py
+pyproject.toml
 prefect_databricks/__init__.py
 prefect_databricks/_version.py
 prefect_databricks/credentials.py
 prefect_databricks/flows.py
 prefect_databricks/jobs.py
 prefect_databricks/rest.py
 prefect_databricks.egg-info/PKG-INFO
 prefect_databricks.egg-info/SOURCES.txt
 prefect_databricks.egg-info/dependency_links.txt
 prefect_databricks.egg-info/entry_points.txt
 prefect_databricks.egg-info/requires.txt
 prefect_databricks.egg-info/top_level.txt
 prefect_databricks/models/__init__.py
 prefect_databricks/models/jobs.py
-scripts/__init__.py
-scripts/generate.py
+prefect_databricks/schemas/jobs-2.1-aws.yaml
+prefect_databricks/schemas/original/jobs-2.1-aws.yaml
+tests/conftest.py
+tests/mock_schema.yaml
 tests/test_block_standards.py
 tests/test_credentials.py
 tests/test_flows.py
 tests/test_generate.py
 tests/test_jobs.py
 tests/test_rest.py
```

### Comparing `prefect-databricks-0.2.3/tests/test_block_standards.py` & `prefect_databricks-0.2.4/tests/test_block_standards.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from prefect.blocks.core import Block
 from prefect.testing.standard_test_suites import BlockStandardTestSuite
 from prefect.utilities.dispatch import get_registry_for_type
 from prefect.utilities.importtools import to_qualified_name
 
 
 def find_module_blocks():
```

### Comparing `prefect-databricks-0.2.3/tests/test_generate.py` & `prefect_databricks-0.2.4/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `prefect-databricks-0.2.3/tests/test_jobs.py` & `prefect_databricks-0.2.4/tests/test_jobs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from prefect_databricks.models.jobs import (
     AccessControlRequest,
     AccessControlRequestForGroup,
     AccessControlRequestForUser,
     CanManage,
 )
 from prefect_databricks.rest import serialize_model
```

### Comparing `prefect-databricks-0.2.3/tests/test_rest.py` & `prefect_databricks-0.2.4/tests/test_rest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 from typing import List
 
 import httpx
 import pytest
-from pydantic import VERSION as PYDANTIC_VERSION
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import BaseModel, Extra
-else:
-    from pydantic import BaseModel, Extra
-
 from prefect_databricks import DatabricksCredentials
 from prefect_databricks.rest import (
     HTTPMethod,
     execute_endpoint,
     serialize_model,
     strip_kwargs,
 )
+from pydantic import BaseModel, Extra
 
 
 @pytest.mark.parametrize("params", [dict(a="A", b="B"), None])
 @pytest.mark.parametrize("http_method", ["get", HTTPMethod.GET, "post"])
 async def test_execute_endpoint(params, http_method, respx_mock):
     url = "https://prefect.io/"
```

