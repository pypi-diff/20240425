# Comparing `tmp/pyhidra-1.0.2.tar.gz` & `tmp/pyhidra-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhidra-1.0.2.tar", last modified: Fri Feb 16 19:06:28 2024, max compression
+gzip compressed data, was "pyhidra-1.1.0.tar", last modified: Wed Apr 24 23:28:12 2024, max compression
```

## Comparing `pyhidra-1.0.2.tar` & `pyhidra-1.1.0.tar`

### file list

```diff
@@ -1,63 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:06:28.830531 pyhidra-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-02-16 19:06:14.000000 pyhidra-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-16 19:06:14.000000 pyhidra-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-02-16 19:06:28.830531 pyhidra-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-02-16 19:06:14.000000 pyhidra-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:06:28.806530 pyhidra-1.0.2/pyhidra/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11946 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/install_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:06:28.810531 pyhidra-1.0.2/pyhidra/java/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:06:28.814530 pyhidra-1.0.2/pyhidra/java/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/plugin/PyScriptProvider.java
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/plugin/PyhidraPlugin.java
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/plugin/PythonFieldExposer.java
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/plugin/completions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:06:28.814530 pyhidra-1.0.2/pyhidra/java/plugin/ghidra_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/plugin/ghidra_scripts/PyhidraBasics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:06:28.818531 pyhidra-1.0.2/pyhidra/java/plugin/interpreter/
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/plugin/interpreter/CancelAction.java
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/plugin/interpreter/InterpreterGhidraScript.java
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/plugin/interpreter/InterpreterTaskMonitor.java
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/plugin/interpreter/PyhidraInterpreterConnection.java
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/plugin/interpreter/RestartAction.java
--rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:06:28.826531 pyhidra-1.0.2/pyhidra/java/property/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/property/AbstractJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/property/BooleanJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/property/ByteJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/property/CharacterJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/property/DoubleJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/property/FloatJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/property/IntegerJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/property/JavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/property/JavaPropertyFactory.java
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/property/LongJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/property/ObjectJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/property/PropertyUtils.java
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/java/property/ShortJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/javac.py
--rw-r--r--   0 runner    (1001) docker     (127)    20900 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     8028 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/uninstall_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-02-16 19:06:14.000000 pyhidra-1.0.2/pyhidra/win_shortcut.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:06:28.830531 pyhidra-1.0.2/pyhidra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-02-16 19:06:28.000000 pyhidra-1.0.2/pyhidra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-02-16 19:06:28.000000 pyhidra-1.0.2/pyhidra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 19:06:28.000000 pyhidra-1.0.2/pyhidra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-16 19:06:28.000000 pyhidra-1.0.2/pyhidra.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 19:06:28.000000 pyhidra-1.0.2/pyhidra.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-16 19:06:28.000000 pyhidra-1.0.2/pyhidra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-16 19:06:28.000000 pyhidra-1.0.2/pyhidra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-02-16 19:06:28.830531 pyhidra-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-16 19:06:14.000000 pyhidra-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:06:28.830531 pyhidra-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-02-16 19:06:14.000000 pyhidra-1.0.2/tests/test_argparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-02-16 19:06:14.000000 pyhidra-1.0.2/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:28:12.428518 pyhidra-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-24 23:27:58.000000 pyhidra-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 23:27:58.000000 pyhidra-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9354 2024-04-24 23:28:12.428518 pyhidra-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-04-24 23:27:58.000000 pyhidra-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:28:12.420518 pyhidra-1.1.0/pyhidra/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7261 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13977 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/install_desktop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/install_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:28:12.420518 pyhidra-1.1.0/pyhidra/java/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:28:12.424518 pyhidra-1.1.0/pyhidra/java/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/PyScriptProvider.java
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/PyhidraPlugin.java
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/PythonFieldExposer.java
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/completions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:28:12.424518 pyhidra-1.1.0/pyhidra/java/plugin/ghidra_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/ghidra_scripts/PyhidraBasics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:28:12.424518 pyhidra-1.1.0/pyhidra/java/plugin/interpreter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/interpreter/CancelAction.java
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/interpreter/InterpreterGhidraScript.java
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/interpreter/InterpreterTaskMonitor.java
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/interpreter/PyhidraInterpreterConnection.java
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/interpreter/RestartAction.java
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:28:12.428518 pyhidra-1.1.0/pyhidra/java/property/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/AbstractJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/BooleanJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/ByteJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/CharacterJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/DoubleJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/FloatJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/IntegerJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/JavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/JavaPropertyFactory.java
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/LongJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/ObjectJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/PropertyUtils.java
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/ShortJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/javac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20899 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/linux_shortcut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8028 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/uninstall_desktop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/uninstall_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/win_shortcut.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:28:12.428518 pyhidra-1.1.0/pyhidra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9354 2024-04-24 23:28:12.000000 pyhidra-1.1.0/pyhidra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-24 23:28:12.000000 pyhidra-1.1.0/pyhidra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 23:28:12.000000 pyhidra-1.1.0/pyhidra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 23:28:12.000000 pyhidra-1.1.0/pyhidra.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 23:28:12.000000 pyhidra-1.1.0/pyhidra.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-24 23:28:12.000000 pyhidra-1.1.0/pyhidra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 23:28:12.000000 pyhidra-1.1.0/pyhidra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-24 23:28:12.428518 pyhidra-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 23:27:58.000000 pyhidra-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:28:12.428518 pyhidra-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-04-24 23:27:58.000000 pyhidra-1.1.0/tests/test_argparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-04-24 23:27:58.000000 pyhidra-1.1.0/tests/test_core.py
```

### Comparing `pyhidra-1.0.2/LICENSE` & `pyhidra-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhidra-1.0.2/PKG-INFO` & `pyhidra-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhidra
-Version: 1.0.2
+Version: 1.1.0
 Summary: Native CPython for Ghidra
 Home-page: https://github.com/Defense-Cyber-Crime-Center/pyhidra
 Author: DC3
 Author-email: dcci@dc3.mil
 License: MIT
 Keywords: ghidra
 Platform: any
@@ -39,26 +39,44 @@
 1. Download and install [Ghidra](https://github.com/NationalSecurityAgency/ghidra/releases) to a desired location.
 
 1. Set the `GHIDRA_INSTALL_DIR` environment variable to point to the directory where Ghidra is installed.
 
 1. Install pyhidra.
 
 ```console
-> pip install pyhidra
+pip install pyhidra
 ```
 ### Enabling the Ghidra User Interface Plugin
 
 1. Run `pyhidraw` from a terminal of your choice.
 2. Open the Code Browser Tool.
 3. From the `File` toolbar menu, select `Configure...`.
 4. From the menu in the image below select `configure` under `Experimental`.
  ![](https://raw.githubusercontent.com/Defense-Cyber-Crime-Center/pyhidra/master/images/image-20220111154029764.png)
 5. Check and enable Pyhidra as seen in the image below.
  ![](https://raw.githubusercontent.com/Defense-Cyber-Crime-Center/pyhidra/master/images/image-20220111154120531.png)
 
+### Desktop Entry
+
+If on linux or windows, a desktop entry can be created to launch an instance of Ghidra with pyhidra attached.
+
+```console
+python -m pyhidra.install_desktop
+```
+
+On windows, this will install a shortcut file on the user's desktop. On linux, this will create an entry 
+that can be found in the applications launcher.
+
+
+To remove, run the following:
+
+```console
+python -m pyhidra.uninstall_desktop
+```
+
 ### Manual Plugin Installation
 
 If pyhidra is planned to be used in a multiprocessing deployed server, the following must be run to allow the Ghidra plugins to be compiled and installed before use.
 
 ```console
 python -m pyhidra.install_plugins
 ```
```

### Comparing `pyhidra-1.0.2/README.md` & `pyhidra-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,44 @@
 1. Download and install [Ghidra](https://github.com/NationalSecurityAgency/ghidra/releases) to a desired location.
 
 1. Set the `GHIDRA_INSTALL_DIR` environment variable to point to the directory where Ghidra is installed.
 
 1. Install pyhidra.
 
 ```console
-> pip install pyhidra
+pip install pyhidra
 ```
 ### Enabling the Ghidra User Interface Plugin
 
 1. Run `pyhidraw` from a terminal of your choice.
 2. Open the Code Browser Tool.
 3. From the `File` toolbar menu, select `Configure...`.
 4. From the menu in the image below select `configure` under `Experimental`.
  ![](https://raw.githubusercontent.com/Defense-Cyber-Crime-Center/pyhidra/master/images/image-20220111154029764.png)
 5. Check and enable Pyhidra as seen in the image below.
  ![](https://raw.githubusercontent.com/Defense-Cyber-Crime-Center/pyhidra/master/images/image-20220111154120531.png)
 
+### Desktop Entry
+
+If on linux or windows, a desktop entry can be created to launch an instance of Ghidra with pyhidra attached.
+
+```console
+python -m pyhidra.install_desktop
+```
+
+On windows, this will install a shortcut file on the user's desktop. On linux, this will create an entry 
+that can be found in the applications launcher.
+
+
+To remove, run the following:
+
+```console
+python -m pyhidra.uninstall_desktop
+```
+
 ### Manual Plugin Installation
 
 If pyhidra is planned to be used in a multiprocessing deployed server, the following must be run to allow the Ghidra plugins to be compiled and installed before use.
 
 ```console
 python -m pyhidra.install_plugins
 ```
```

### Comparing `pyhidra-1.0.2/pyhidra/__main__.py` & `pyhidra-1.1.0/pyhidra/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,19 +10,14 @@
 import pyhidra.gui
 
 
 # NOTE: this must be "pyhidra" and not __name__
 logger = logging.getLogger("pyhidra")
 
 
-def _create_shortcut():
-    from pyhidra.win_shortcut import create_shortcut
-    create_shortcut(Path(sys.argv[-1]))
-
-
 def _interpreter(interpreter_globals: dict):
     from ghidra.framework import Application
     version = Application.getApplicationVersion()
     name = Application.getApplicationReleaseName()
     banner = f"Python Interpreter for Ghidra {version} {name}\n"
     banner += f"Python {sys.version} on {sys.platform}"
     code.interact(banner=banner, local=interpreter_globals, exitmsg='')
@@ -178,23 +173,14 @@
     parser.add_argument(
         "-g",
         "--gui",
         action="store_true",
         dest="gui",
         help="Start Ghidra GUI"
     )
-    if is_win32:
-        parser.add_argument(
-            "-s",
-            "--shortcut",
-            action="store_const",
-            dest="func",
-            const=_create_shortcut,
-            help="Creates a shortcut that can be pinned to the taskbar (Windows only)"
-        )
     parser.add_argument(
         "--install-dir",
         type=Path,
         default=None,
         dest="install_dir",
         metavar="",
         help="Path to Ghidra installation. "
```

### Comparing `pyhidra-1.0.2/pyhidra/core.py` & `pyhidra-1.1.0/pyhidra/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,48 +61,72 @@
 
 
 def _setup_project(
         binary_path: Union[str, Path],
         project_location: Union[str, Path] = None,
         project_name: str = None,
         language: str = None,
-        compiler: str = None
+        compiler: str = None,
+        loader: Union[str, JClass] = None
 ) -> Tuple["GhidraProject", "Program"]:
     from ghidra.base.project import GhidraProject
+    from java.lang import ClassLoader
     from java.io import IOException
     if binary_path is not None:
         binary_path = Path(binary_path)
     if project_location:
         project_location = Path(project_location)
     else:
         project_location = binary_path.parent
     if not project_name:
         project_name = f"{binary_path.name}_ghidra"
     project_location /= project_name
     project_location.mkdir(exist_ok=True, parents=True)
 
+    if isinstance(loader, str):
+        from java.lang import ClassNotFoundException
+        try:
+            gcl = ClassLoader.getSystemClassLoader()
+            loader = JClass(loader, gcl)
+        except (TypeError, ClassNotFoundException) as e:
+            raise ValueError from e
+
+    if isinstance(loader, JClass):
+        from ghidra.app.util.opinion import Loader
+        if not Loader.class_.isAssignableFrom(loader):
+            raise TypeError(f"{loader} does not implement ghidra.app.util.opinion.Loader")
+
     # Open/Create project
     program: "Program" = None
     try:
         project = GhidraProject.openProject(project_location, project_name, True)
         if binary_path is not None:
             if project.getRootFolder().getFile(binary_path.name):
                 program = project.openProgram("/", binary_path.name, False)
     except IOException:
         project = GhidraProject.createProject(project_location, project_name, False)
 
+    # NOTE: GhidraProject.importProgram behaves differently when a loader is provided
+    # loaderClass may not be null so we must use the correct method override
+
     if binary_path is not None and program is None:
         if language is None:
-            program = project.importProgram(binary_path)
+            if loader is None:
+                program = project.importProgram(binary_path)
+            else:
+                program = project.importProgram(binary_path, loader)
             if program is None:
                 raise RuntimeError(f"Ghidra failed to import '{binary_path}'. Try providing a language manually.")
         else:
             lang = _get_language(language)
             comp = _get_compiler_spec(lang, compiler)
-            program = project.importProgram(binary_path, lang, comp)
+            if loader is None:
+                program = project.importProgram(binary_path, lang, comp)
+            else:
+                program = project.importProgram(binary_path, loader, lang, comp)
             if program is None:
                 message = f"Ghidra failed to import '{binary_path}'. "
                 if compiler:
                     message += f"The provided language/compiler pair ({language} / {compiler}) may be invalid."
                 else:
                     message += f"The provided language ({language}) may be invalid."
                 raise ValueError(message)
@@ -154,30 +178,34 @@
 def open_program(
         binary_path: Union[str, Path],
         project_location: Union[str, Path] = None,
         project_name: str = None,
         analyze=True,
         language: str = None,
         compiler: str = None,
-) -> ContextManager["FlatProgramAPI"]:
+        loader: Union[str, JClass] = None
+) -> ContextManager["FlatProgramAPI"]: # type: ignore
     """
     Opens given binary path in Ghidra and returns FlatProgramAPI object.
 
     :param binary_path: Path to binary file, may be None.
     :param project_location: Location of Ghidra project to open/create.
         (Defaults to same directory as binary file)
     :param project_name: Name of Ghidra project to open/create.
         (Defaults to name of binary file suffixed with "_ghidra")
     :param analyze: Whether to run analysis before returning.
     :param language: The LanguageID to use for the program.
         (Defaults to Ghidra's detected LanguageID)
     :param compiler: The CompilerSpecID to use for the program. Requires a provided language.
         (Defaults to the Language's default compiler)
+    :param loader: The `ghidra.app.util.opinion.Loader` class to use when importing the program.
+        This may be either a Java class or its path. (Defaults to None)
     :return: A Ghidra FlatProgramAPI object.
-    :raises ValueError: If the provided language or compiler is invalid.
+    :raises ValueError: If the provided language, compiler or loader is invalid.
+    :raises TypeError: If the provided loader does not implement `ghidra.app.util.opinion.Loader`.
     """
 
     from pyhidra.launcher import PyhidraLauncher, HeadlessPyhidraLauncher
 
     if not PyhidraLauncher.has_launched():
         HeadlessPyhidraLauncher().start()
 
@@ -185,15 +213,16 @@
     from ghidra.program.flatapi import FlatProgramAPI
 
     project, program = _setup_project(
         binary_path,
         project_location,
         project_name,
         language,
-        compiler
+        compiler,
+        loader
     )
     GhidraScriptUtil.acquireBundleHostReference()
 
     try:
         flat_api = FlatProgramAPI(program)
 
         if analyze:
@@ -211,14 +240,15 @@
         binary_path: Union[str, Path] = None,
         project_location: Union[str, Path] = None,
         project_name: str = None,
         verbose=False,
         analyze=True,
         language: str = None,
         compiler: str = None,
+        loader: Union[str, JClass] = None,
         *,
         install_dir: Path = None
 ):
     """
     Runs a given script on a given binary path.
 
     :param binary_path: Path to binary file, may be None.
@@ -230,32 +260,36 @@
     :param script_args: Command line arguments to pass to script.
     :param verbose: Enable verbose output during Ghidra initialization.
     :param analyze: Whether to run analysis, if a binary_path is provided, before returning.
     :param language: The LanguageID to use for the program.
         (Defaults to Ghidra's detected LanguageID)
     :param compiler: The CompilerSpecID to use for the program. Requires a provided language.
         (Defaults to the Language's default compiler)
+    :param loader: The `ghidra.app.util.opinion.Loader` class to use when importing the program.
+        This may be either a Java class or its path. (Defaults to None)
     :param install_dir: The path to the Ghidra installation directory. This parameter is only
         used if Ghidra has not been started yet.
         (Defaults to the GHIDRA_INSTALL_DIR environment variable)
-    :raises ValueError: If the provided language or compiler is invalid.
+    :raises ValueError: If the provided language, compiler or loader is invalid.
+    :raises TypeError: If the provided loader does not implement `ghidra.app.util.opinion.Loader`.
     """
     from pyhidra.launcher import PyhidraLauncher, HeadlessPyhidraLauncher
 
     if not PyhidraLauncher.has_launched():
         HeadlessPyhidraLauncher(verbose=verbose, install_dir=install_dir).start()
 
     project, program = None, None
     if binary_path or project_location:
         project, program = _setup_project(
             binary_path,
             project_location,
             project_name,
             language,
-            compiler
+            compiler,
+            loader
         )
 
     from ghidra.app.script import GhidraScriptUtil
 
     # always aquire a bundle reference to avoid a NPE when attempting to run any Java scripts
     GhidraScriptUtil.acquireBundleHostReference()
     try:
@@ -278,14 +312,15 @@
     project_location: Union[str, Path] = None,
     project_name: str = None,
     script_args: List[str] = None,
     verbose=False,
     analyze=True,
     lang: str = None,
     compiler: str = None,
+    loader: Union[str, JClass] = None,
     *,
     install_dir: Path = None
 ):
     """
     Runs a given script on a given binary path.
 
     :param binary_path: Path to binary file, may be None.
@@ -297,16 +332,19 @@
     :param script_args: Command line arguments to pass to script.
     :param verbose: Enable verbose output during Ghidra initialization.
     :param analyze: Whether to run analysis, if a binary_path is provided, before running the script.
     :param lang: The LanguageID to use for the program.
         (Defaults to Ghidra's detected LanguageID)
     :param compiler: The CompilerSpecID to use for the program. Requires a provided language.
         (Defaults to the Language's default compiler)
+    :param loader: The `ghidra.app.util.opinion.Loader` class to use when importing the program.
+        This may be either a Java class or its path. (Defaults to None)
     :param install_dir: The path to the Ghidra installation directory. This parameter is only
         used if Ghidra has not been started yet.
         (Defaults to the GHIDRA_INSTALL_DIR environment variable)
-    :raises ValueError: If the provided language or compiler is invalid.
+    :raises ValueError: If the provided language, compiler or loader is invalid.
+    :raises TypeError: If the provided loader does not implement `ghidra.app.util.opinion.Loader`.
     """
     script_path = str(script_path)
-    args = binary_path, project_location, project_name, verbose, analyze, lang, compiler
+    args = binary_path, project_location, project_name, verbose, analyze, lang, compiler, loader
     with _flat_api(*args, install_dir=install_dir) as script:
         script.run(script_path, script_args)
```

### Comparing `pyhidra-1.0.2/pyhidra/gui.py` & `pyhidra-1.1.0/pyhidra/gui.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import argparse
 import io
 import os
 from pathlib import Path
 import platform
 import sys
 import traceback
+from typing import NoReturn
 import warnings
 
 import pyhidra
 
 
 class _GuiOutput(io.StringIO):
 
@@ -33,75 +34,99 @@
 
     def print_help(self, file=None):
         if file is None:
             file = _GuiOutput("Help")
         self._print_message(self.format_help(), file)
 
 
+def _gui_mac() -> NoReturn:
+    args = _parse_args()
+    install_dir = args.install_dir
+    path = Path(sys.base_exec_prefix) / "Resources/Python.app/Contents/MacOS/Python"
+    if path.exists():
+        # the python launcher app will correctly start the venv if sys.executable is in a venv
+        argv = [sys.executable, "-m", "pyhidra", "-g"]
+        if install_dir is not None:
+            argv += ["--install-dir", str(install_dir)]
+        actions = ((os.POSIX_SPAWN_CLOSE, 0), (os.POSIX_SPAWN_CLOSE, 1), (os.POSIX_SPAWN_CLOSE, 2))
+        os.posix_spawn(str(path), argv, os.environ, file_actions=actions)
+    else:
+        print("could not find the Python.app path, launch failed")
+    sys.exit(0)
+
+
+def _parse_args():
+    parser = _GuiArgumentParser(prog="pyhidraw")
+    parser.add_argument(
+        "--install-dir",
+        type=Path,
+        default=None,
+        dest="install_dir",
+        metavar="",
+        help="Path to Ghidra installation. "\
+            "(defaults to the GHIDRA_INSTALL_DIR environment variable)"
+    )
+    return parser.parse_args()
+
+
+def _gui_default(install_dir: Path):
+    pid = os.fork()
+    if pid != 0:
+        # original process can exit
+        return
+
+    fd = os.open(os.devnull, os.O_RDWR)
+    # redirect stdin, stdout and stderr to /dev/null so the jvm can't use the terminal
+    # this also prevents errors from attempting to write to a closed sys.stdout #21
+    os.dup2(fd, sys.stdin.fileno(), inheritable=False)
+    os.dup2(fd, sys.stdout.fileno(), inheritable=False)
+    os.dup2(fd, sys.stderr.fileno(), inheritable=False)
+
+    # run the application
+    gui(install_dir)
+
+
 def _gui():
     # this is the entry from the gui script
     # there may or may not be an attached terminal
     # depending on the current operating system
 
+    if platform.system() == "Darwin":
+        _gui_mac()
+
     # This check handles the edge case of having a corrupt Python installation
     # where tkinter can't be imported. Since there may not be an attached
     # terminal, the problem still needs to be reported somehow.
     try:
-        # This import creates problems for macOS
-        if platform.system() != 'Darwin':
-            import tkinter.messagebox as _
+        import tkinter.messagebox as _
     except ImportError as e:
-        if platform.system() == 'Windows':
+        if platform.system() == "Windows":
             # there is no console/terminal to report the error
             import ctypes
             MessageBox = ctypes.windll.user32.MessageBoxW
             MessageBox(None, str(e), "Import Error", 0)
             sys.exit(1)
         # report this before detaching from the console or no
         # errors will be reported if they occur
         raise
 
     try:
-        parser = _GuiArgumentParser(prog="pyhidraw")
-        parser.add_argument(
-            "--install-dir",
-            type=Path,
-            default=None,
-            dest="install_dir",
-            metavar="",
-            help="Path to Ghidra installation. "\
-                "(defaults to the GHIDRA_INSTALL_DIR environment variable)"
-        )
-        args = parser.parse_args()
+        args = _parse_args()
         install_dir = args.install_dir
     except Exception as e:
         import tkinter.messagebox
         msg = "".join(traceback.format_exception(type(e), value=e, tb=e.__traceback__))
         tkinter.messagebox.showerror(type(e), msg)
         sys.exit(1)
 
     if platform.system() == 'Windows':
         # gui_script works like it is supposed to on windows
         gui(install_dir)
-        return
-
-    pid = os.fork()
-    if pid != 0:
-        # original process can exit
-        return
-
-    fd = os.open(os.devnull, os.O_RDWR)
-    # redirect stdin, stdout and stderr to /dev/null so the jvm can't use the terminal
-    # this also prevents errors from attempting to write to a closed sys.stdout #21
-    os.dup2(fd, sys.stdin.fileno(), inheritable=False)
-    os.dup2(fd, sys.stdout.fileno(), inheritable=False)
-    os.dup2(fd, sys.stderr.fileno(), inheritable=False)
-
-    # run the application
-    gui(install_dir)
+    else:
+        _gui_default(install_dir)
 
 
 def gui(install_dir: Path = None):
     """
     Starts the Ghidra GUI
 
     :param install_dir: The path to the Ghidra installation directory.
```

### Comparing `pyhidra-1.0.2/pyhidra/install_plugins.py` & `pyhidra-1.1.0/pyhidra/install_plugins.py`

 * *Files identical despite different names*

### Comparing `pyhidra-1.0.2/pyhidra/java/plugin/PyScriptProvider.java` & `pyhidra-1.1.0/pyhidra/java/plugin/PyScriptProvider.java`

 * *Files identical despite different names*

### Comparing `pyhidra-1.0.2/pyhidra/java/plugin/PyhidraPlugin.java` & `pyhidra-1.1.0/pyhidra/java/plugin/PyhidraPlugin.java`

 * *Files identical despite different names*

### Comparing `pyhidra-1.0.2/pyhidra/java/plugin/PythonFieldExposer.java` & `pyhidra-1.1.0/pyhidra/java/plugin/PythonFieldExposer.java`

 * *Files identical despite different names*

### Comparing `pyhidra-1.0.2/pyhidra/java/plugin/completions.py` & `pyhidra-1.1.0/pyhidra/java/plugin/completions.py`

 * *Files identical despite different names*

### Comparing `pyhidra-1.0.2/pyhidra/java/plugin/ghidra_scripts/PyhidraBasics.py` & `pyhidra-1.1.0/pyhidra/java/plugin/ghidra_scripts/PyhidraBasics.py`

 * *Files identical despite different names*

### Comparing `pyhidra-1.0.2/pyhidra/java/plugin/interpreter/CancelAction.java` & `pyhidra-1.1.0/pyhidra/java/plugin/interpreter/CancelAction.java`

 * *Files identical despite different names*

### Comparing `pyhidra-1.0.2/pyhidra/java/plugin/interpreter/InterpreterGhidraScript.java` & `pyhidra-1.1.0/pyhidra/java/plugin/interpreter/InterpreterGhidraScript.java`

 * *Files identical despite different names*

### Comparing `pyhidra-1.0.2/pyhidra/java/plugin/interpreter/InterpreterTaskMonitor.java` & `pyhidra-1.1.0/pyhidra/java/plugin/interpreter/InterpreterTaskMonitor.java`

 * *Files identical despite different names*

### Comparing `pyhidra-1.0.2/pyhidra/java/plugin/interpreter/PyhidraInterpreterConnection.java` & `pyhidra-1.1.0/pyhidra/java/plugin/interpreter/PyhidraInterpreterConnection.java`

 * *Files identical despite different names*

### Comparing `pyhidra-1.0.2/pyhidra/java/plugin/interpreter/RestartAction.java` & `pyhidra-1.1.0/pyhidra/java/plugin/interpreter/RestartAction.java`

 * *Files identical despite different names*

### Comparing `pyhidra-1.0.2/pyhidra/java/plugin/plugin.py` & `pyhidra-1.1.0/pyhidra/java/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `pyhidra-1.0.2/pyhidra/java/property/AbstractJavaProperty.java` & `pyhidra-1.1.0/pyhidra/java/property/AbstractJavaProperty.java`

 * *Files identical despite different names*

### Comparing `pyhidra-1.0.2/pyhidra/java/property/JavaPropertyFactory.java` & `pyhidra-1.1.0/pyhidra/java/property/JavaPropertyFactory.java`

 * *Files identical despite different names*

### Comparing `pyhidra-1.0.2/pyhidra/java/property/PropertyUtils.java` & `pyhidra-1.1.0/pyhidra/java/property/PropertyUtils.java`

 * *Files identical despite different names*

### Comparing `pyhidra-1.0.2/pyhidra/javac.py` & `pyhidra-1.1.0/pyhidra/javac.py`

 * *Files identical despite different names*

### Comparing `pyhidra-1.0.2/pyhidra/launcher.py` & `pyhidra-1.1.0/pyhidra/launcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -551,24 +551,24 @@
         for t in Thread.getAllStackTraces().keySet():
             if t.getName() == name:
                 return t
         return None
 
     def _launch(self):
         import ctypes
-        from ghidra import GhidraRun
+        from ghidra import Ghidra
         from java.lang import Runtime, Thread
 
         if sys.platform == "win32":
             appid = ctypes.c_wchar_p(self.app_info.name)
             ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(appid)
 
         stdout = _PyhidraStdOut(sys.stdout)
         stderr = _PyhidraStdOut(sys.stderr)
         with contextlib.redirect_stdout(stdout), contextlib.redirect_stderr(stderr):
-            jpype.setupGuiEnvironment(lambda: GhidraRun().launch(self._layout, self.args))
+            jpype.setupGuiEnvironment(lambda: Ghidra.main(["ghidra.GhidraRun", *self.args]))
             is_exiting = threading.Event()
             Runtime.getRuntime().addShutdownHook(Thread(is_exiting.set))
             try:
                 is_exiting.wait()
             finally:
                 jpype.shutdownGuiEnvironment()
```

### Comparing `pyhidra-1.0.2/pyhidra/properties.py` & `pyhidra-1.1.0/pyhidra/properties.py`

 * *Files identical despite different names*

### Comparing `pyhidra-1.0.2/pyhidra/script.py` & `pyhidra-1.1.0/pyhidra/script.py`

 * *Files identical despite different names*

### Comparing `pyhidra-1.0.2/pyhidra/uninstall_plugin.py` & `pyhidra-1.1.0/pyhidra/uninstall_plugin.py`

 * *Files identical despite different names*

### Comparing `pyhidra-1.0.2/pyhidra/version.py` & `pyhidra-1.1.0/pyhidra/version.py`

 * *Files identical despite different names*

### Comparing `pyhidra-1.0.2/pyhidra/win_shortcut.py` & `pyhidra-1.1.0/pyhidra/win_shortcut.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 from pathlib import Path
 from pyhidra import DeferredPyhidraLauncher
 
 
 # creating a shortcut with the winapi to have a set app id is trivial right?
 
 
-def create_shortcut(link: Path):
-    if not link.is_absolute():
-        link = link.absolute()
-    link = link.with_suffix(".lnk")
+
+
+def create_shortcut(install_dir: Path = None):
+    """Creates a shortcut to Ghidra (with pyhidra) on the desktop."""
+
+    link = Path("~/Desktop/Ghidra (pyhidra).lnk").expanduser()
     if link.exists():
         sys.exit(f"{link} already exists")
 
     import ctypes
     import ctypes.wintypes
 
     class _GUID(ctypes.wintypes.DWORD * 4):
@@ -23,15 +25,15 @@
             ctypes.oledll.ole32.CLSIDFromString(guid, ctypes.byref(self))
 
     class _PROPERTYKEY(ctypes.wintypes.DWORD * 5):
         def __init__(self, key: str, pid: int) -> None:
             ctypes.oledll.ole32.IIDFromString(key, ctypes.byref(self))
             self[-1] = pid
 
-    launcher = DeferredPyhidraLauncher()
+    launcher = DeferredPyhidraLauncher(install_dir=install_dir)
 
     _PropertyVariant = struct.Struct(f"B7xP{ctypes.sizeof(ctypes.c_void_p())}x")
     _AppUserModelId = _PROPERTYKEY("{9F4C2855-9F79-4B39-A8D0-E1D42DE1D5F3}", 5)
     _CLSID_ShellLink = _GUID("{00021401-0000-0000-C000-000000000046}")
     _IID_IShellLinkW = _GUID("{000214F9-0000-0000-C000-000000000046}")
     _IID_IPersistFile = _GUID("{0000010B-0000-0000-C000-000000000046}")
     _IID_IPropertyStore = _GUID("{886d8eeb-8cf2-4446-8d02-cdba1dbdcf99}")
@@ -76,7 +78,16 @@
         if p_file:
             _Release(p_file)
         if p_link:
             _Release(p_link)
         if p_store:
             _Release(p_store)
         ctypes.oledll.ole32.CoUninitialize()
+
+    print(f"Installed {link}")
+
+
+def remove_shortcut():
+    link = Path("~/Desktop/Ghidra (pyhidra).lnk").expanduser()
+    if link.exists():
+        link.unlink()
+        print(f"Removed {link}")
```

### Comparing `pyhidra-1.0.2/pyhidra.egg-info/PKG-INFO` & `pyhidra-1.1.0/pyhidra.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhidra
-Version: 1.0.2
+Version: 1.1.0
 Summary: Native CPython for Ghidra
 Home-page: https://github.com/Defense-Cyber-Crime-Center/pyhidra
 Author: DC3
 Author-email: dcci@dc3.mil
 License: MIT
 Keywords: ghidra
 Platform: any
@@ -39,26 +39,44 @@
 1. Download and install [Ghidra](https://github.com/NationalSecurityAgency/ghidra/releases) to a desired location.
 
 1. Set the `GHIDRA_INSTALL_DIR` environment variable to point to the directory where Ghidra is installed.
 
 1. Install pyhidra.
 
 ```console
-> pip install pyhidra
+pip install pyhidra
 ```
 ### Enabling the Ghidra User Interface Plugin
 
 1. Run `pyhidraw` from a terminal of your choice.
 2. Open the Code Browser Tool.
 3. From the `File` toolbar menu, select `Configure...`.
 4. From the menu in the image below select `configure` under `Experimental`.
  ![](https://raw.githubusercontent.com/Defense-Cyber-Crime-Center/pyhidra/master/images/image-20220111154029764.png)
 5. Check and enable Pyhidra as seen in the image below.
  ![](https://raw.githubusercontent.com/Defense-Cyber-Crime-Center/pyhidra/master/images/image-20220111154120531.png)
 
+### Desktop Entry
+
+If on linux or windows, a desktop entry can be created to launch an instance of Ghidra with pyhidra attached.
+
+```console
+python -m pyhidra.install_desktop
+```
+
+On windows, this will install a shortcut file on the user's desktop. On linux, this will create an entry 
+that can be found in the applications launcher.
+
+
+To remove, run the following:
+
+```console
+python -m pyhidra.uninstall_desktop
+```
+
 ### Manual Plugin Installation
 
 If pyhidra is planned to be used in a multiprocessing deployed server, the following must be run to allow the Ghidra plugins to be compiled and installed before use.
 
 ```console
 python -m pyhidra.install_plugins
 ```
```

### Comparing `pyhidra-1.0.2/pyhidra.egg-info/SOURCES.txt` & `pyhidra-1.1.0/pyhidra.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 setup.cfg
 setup.py
 pyhidra/__init__.py
 pyhidra/__main__.py
 pyhidra/converters.py
 pyhidra/core.py
 pyhidra/gui.py
+pyhidra/install_desktop.py
 pyhidra/install_plugins.py
 pyhidra/javac.py
 pyhidra/launcher.py
+pyhidra/linux_shortcut.py
 pyhidra/properties.py
 pyhidra/script.py
+pyhidra/uninstall_desktop.py
 pyhidra/uninstall_plugin.py
 pyhidra/version.py
 pyhidra/win_shortcut.py
 pyhidra.egg-info/PKG-INFO
 pyhidra.egg-info/SOURCES.txt
 pyhidra.egg-info/dependency_links.txt
 pyhidra.egg-info/entry_points.txt
```

### Comparing `pyhidra-1.0.2/setup.cfg` & `pyhidra-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyhidra-1.0.2/tests/test_argparser.py` & `pyhidra-1.1.0/tests/test_argparser.py`

 * *Files identical despite different names*

