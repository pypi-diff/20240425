# Comparing `tmp/nakivo_prometheus_exporter-0.2.3.tar.gz` & `tmp/nakivo_prometheus_exporter-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nakivo_prometheus_exporter-0.2.3.tar", last modified: Tue Apr 16 13:22:56 2024, max compression
+gzip compressed data, was "nakivo_prometheus_exporter-0.3.0.tar", last modified: Thu Apr 25 11:09:45 2024, max compression
```

## Comparing `nakivo_prometheus_exporter-0.2.3.tar` & `nakivo_prometheus_exporter-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 13:22:56.646417 nakivo_prometheus_exporter-0.2.3/
--rw-rw-rw-   0        0        0     5878 2024-04-16 13:22:56.644405 nakivo_prometheus_exporter-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     4011 2024-04-05 14:17:03.000000 nakivo_prometheus_exporter-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 13:22:56.594307 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/
--rw-rw-rw-   0        0        0     1651 2024-04-05 13:26:41.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/__debug__.py
--rw-rw-rw-   0        0        0      104 2024-03-26 13:49:20.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/__init__.py
--rw-rw-rw-   0        0        0      440 2024-04-16 13:21:46.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/__version__.py
--rw-rw-rw-   0        0        0     3382 2024-04-05 13:24:38.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/metrics.py
--rw-rw-rw-   0        0        0     4088 2024-04-05 13:24:38.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/nakivo_api.py
--rw-rw-rw-   0        0        0    11041 2024-04-16 13:21:36.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/prom_parser.py
--rw-rw-rw-   0        0        0     4715 2024-04-05 13:54:13.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/server.py
-drwxrwxrwx   0        0        0        0 2024-04-16 13:22:56.635268 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter.egg-info/
--rw-rw-rw-   0        0        0     5878 2024-04-16 13:22:56.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      599 2024-04-16 13:22:56.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 13:22:56.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2024-04-16 13:22:56.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      169 2024-04-16 13:22:56.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-04-16 13:22:56.000000 nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 13:22:56.646417 nakivo_prometheus_exporter-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     5248 2024-03-26 16:09:56.000000 nakivo_prometheus_exporter-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:09:45.823846 nakivo_prometheus_exporter-0.3.0/
+-rw-rw-rw-   0        0        0     5971 2024-04-25 11:09:45.823846 nakivo_prometheus_exporter-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4104 2024-04-25 10:59:55.000000 nakivo_prometheus_exporter-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 11:09:45.776964 nakivo_prometheus_exporter-0.3.0/nakivo_prometheus_exporter/
+-rw-rw-rw-   0        0        0     1651 2024-04-05 13:26:41.000000 nakivo_prometheus_exporter-0.3.0/nakivo_prometheus_exporter/__debug__.py
+-rw-rw-rw-   0        0        0      104 2024-03-26 13:49:20.000000 nakivo_prometheus_exporter-0.3.0/nakivo_prometheus_exporter/__init__.py
+-rw-rw-rw-   0        0        0      440 2024-04-25 11:07:57.000000 nakivo_prometheus_exporter-0.3.0/nakivo_prometheus_exporter/__version__.py
+-rw-rw-rw-   0        0        0     3382 2024-04-05 13:24:38.000000 nakivo_prometheus_exporter-0.3.0/nakivo_prometheus_exporter/metrics.py
+-rw-rw-rw-   0        0        0     4088 2024-04-05 13:24:38.000000 nakivo_prometheus_exporter-0.3.0/nakivo_prometheus_exporter/nakivo_api.py
+-rw-rw-rw-   0        0        0    11634 2024-04-25 11:08:16.000000 nakivo_prometheus_exporter-0.3.0/nakivo_prometheus_exporter/prom_parser.py
+-rw-rw-rw-   0        0        0     4715 2024-04-05 13:54:13.000000 nakivo_prometheus_exporter-0.3.0/nakivo_prometheus_exporter/server.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:09:45.823846 nakivo_prometheus_exporter-0.3.0/nakivo_prometheus_exporter.egg-info/
+-rw-rw-rw-   0        0        0     5971 2024-04-25 11:09:45.000000 nakivo_prometheus_exporter-0.3.0/nakivo_prometheus_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      599 2024-04-25 11:09:45.000000 nakivo_prometheus_exporter-0.3.0/nakivo_prometheus_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 11:09:45.000000 nakivo_prometheus_exporter-0.3.0/nakivo_prometheus_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2024-04-25 11:09:45.000000 nakivo_prometheus_exporter-0.3.0/nakivo_prometheus_exporter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      169 2024-04-25 11:09:45.000000 nakivo_prometheus_exporter-0.3.0/nakivo_prometheus_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-04-25 11:09:45.000000 nakivo_prometheus_exporter-0.3.0/nakivo_prometheus_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 11:09:45.823846 nakivo_prometheus_exporter-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     5264 2024-04-25 11:08:16.000000 nakivo_prometheus_exporter-0.3.0/setup.py
```

### Comparing `nakivo_prometheus_exporter-0.2.3/PKG-INFO` & `nakivo_prometheus_exporter-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nakivo_prometheus_exporter
-Version: 0.2.3
+Version: 0.3.0
 Summary: Connecto to Nakivo API and export metrics to Prometheus
 Home-page: https://github.com/netinvent/nakivo_prometheus_exporter
 Author: NetInvent - Orsiris de Jong
 Author-email: contact@netinvent.fr
 License: GPLv3
 Keywords: shell,backup,prometheus,linux,cli
 Classifier: Development Status :: 5 - Production/Stable
@@ -116,15 +116,15 @@
 If everything works, you can use the provided systemd service file from the systemd directory, copy it into `/etc/systemd/system` and run the service with
 ```
 systemctl enable --now nakivo_prometheus_exporter
 ```
 
 ## Caveats
 
-Since on every scraping, the exporter connects to *ALL* Nakivo API endpoints defined in the host section, you should set the scraper interval to something reasonable like 1 hour.
+Since on every scraping, the exporter connects to *ALL* Nakivo API endpoints defined in the host section, you should set the scraper interval to something reasonable like 1 hour, and increase the scrape timeout value to one minute (see the `prometheus.yml` example file).
 
 ## Other caveats
 
 This is a quick and dirty proof of concept, only fetching  backup states/duration/sizes and licensing state.  
 There's still quiescing information missing (didn't find it in the (Nakivo API)[https://helpcenter.nakivo.com/api-reference/Content/API-Reference-Overview.htm])
 
 If some traction is obersved for the project, we might add missing or interesting metrics.
```

### Comparing `nakivo_prometheus_exporter-0.2.3/README.md` & `nakivo_prometheus_exporter-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 If everything works, you can use the provided systemd service file from the systemd directory, copy it into `/etc/systemd/system` and run the service with
 ```
 systemctl enable --now nakivo_prometheus_exporter
 ```
 
 ## Caveats
 
-Since on every scraping, the exporter connects to *ALL* Nakivo API endpoints defined in the host section, you should set the scraper interval to something reasonable like 1 hour.
+Since on every scraping, the exporter connects to *ALL* Nakivo API endpoints defined in the host section, you should set the scraper interval to something reasonable like 1 hour, and increase the scrape timeout value to one minute (see the `prometheus.yml` example file).
 
 ## Other caveats
 
 This is a quick and dirty proof of concept, only fetching  backup states/duration/sizes and licensing state.  
 There's still quiescing information missing (didn't find it in the (Nakivo API)[https://helpcenter.nakivo.com/api-reference/Content/API-Reference-Overview.htm])
 
 If some traction is obersved for the project, we might add missing or interesting metrics.
```

### Comparing `nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/__debug__.py` & `nakivo_prometheus_exporter-0.3.0/nakivo_prometheus_exporter/__debug__.py`

 * *Files identical despite different names*

### Comparing `nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/metrics.py` & `nakivo_prometheus_exporter-0.3.0/nakivo_prometheus_exporter/metrics.py`

 * *Files identical despite different names*

### Comparing `nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/nakivo_api.py` & `nakivo_prometheus_exporter-0.3.0/nakivo_prometheus_exporter/nakivo_api.py`

 * *Files identical despite different names*

### Comparing `nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/prom_parser.py` & `nakivo_prometheus_exporter-0.3.0/nakivo_prometheus_exporter/prom_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 __appname__ = "nakivo_prometheus_exporter"
 __author__ = "Orsiris de Jong"
 __site__ = "https://www.github.com/netinvent/nakivo_prometheus_exporter"
 __description__ = "Naviko API Prometheus data exporter"
 __copyright__ = "Copyright (C) 2024 NetInvent"
 __license__ = "GPL-3.0-only"
-__build__ = "2024041601"
+__build__ = "2024042501"
 
 
 import sys
 from argparse import ArgumentParser
 from typing import Union
 from ruamel.yaml import YAML
 from pathlib import Path
@@ -47,33 +47,39 @@
                 return False
             return full_config
     except OSError:
         logger.critical(f"Cannot load configuration file from {config_file}")
         return False
 
 
-def intercept_api_errors(api_return: dict, host: str):
+def intercept_api_errors(api_return: dict, host: str) -> tuple[bool, str]:
     """
     Intercept API return and check for errors
     """
     try:
         if api_return["type"] == "exception":
             logger.error(f"API replied: {api_return['message']}")
             logger.debug(f"Full API return: {api_return}")
-            return True
+
+            prom_data = "# HELP nakivo_api_error\n\
+# TYPE nakivo_api_error gauge\n"
+            prom_data += f'nakivo_api_error{{host="{host}"}} 1\n'
+            return True, prom_data
     except (IndexError, KeyError, TypeError, AttributeError):
         pass
+    return False, None
 
 
 def license_to_prometheus(license_data: dict, host: str):
     """
     Extract Nakivo license status from Job result
     """
-    if intercept_api_errors(license_data, host):
-        return False
+    has_errors, prom_data = intercept_api_errors(license_data, host)
+    if has_errors:
+        return prom_data
 
     try:
         installed = 1 if license_data["data"]["installed"] else 0
     except (IndexError, KeyError, TypeError, AttributeError):
         installed = 0
     try:
         client = license_data["data"]["client"]
@@ -151,24 +157,25 @@
     return prom_data
 
 
 def get_vm_backup_result(job_result: dict, host: str, filter_active_only: bool = True):
     """
     Extract VM backup status from Nakvio Job result
     """
-    if intercept_api_errors(job_result, host):
-        return False
+    has_errors, prom_data = intercept_api_errors(job_result, host)
+    if has_errors:
+        return prom_data
 
     vm_job_state = []
-    prom_data = "# HELP nakivo_backup_state When will the license expire (seconds)\n\
+    prom_data = "# HELP nakivo_backup_state backup okay (0), warnings (1), failed (2)\n\
 # TYPE nakivo_backup_state gauge\n\
-# HELP nakivo_backup_state Backup duration (seconds)\n\
-# TYPE nakivo_backup_state gauge\n\
-# HELP nakivo_backup_state Backup size (bytes)\n\
-# TYPE nakivo_backup_state gauge\n"
+# HELP nakivo_backup_duration Backup duration (seconds)\n\
+# TYPE nakivo_backup_duration gauge\n\
+# HELP nakivo_backup_size Backup size (bytes)\n\
+# TYPE nakivo_backup_size gauge\n"
     for job in job_result["data"]["children"]:
         if filter_active_only:
             if job["status"] in ("GRAY"):
                 continue
         job_name = job["name"]
         for vm in job["objects"]:
             name = vm["sourceName"]
@@ -205,27 +212,32 @@
         try:
             # pylint: disable=used-before-assignment
             logger.error(f"Bogus host config for {host}")
         except NameError:
             logger.error("Bogus host config")
         return False
 
+    prom_data = "# HELP nakivo_api_authentication Do we have an API auth error\n\
+# TYPE nakivo_api_authentication_error gauge\n"
+
     api = NakivoAPI(host, username, password, cert_verify)
     if not api.authenticate():
         logger.error(f"Authentication failure for {host} as {username}")
-        return False
+        prom_data += f'nakivo_api_authentication_error{{host="{host}"}} 1\n'
+        return prom_data
+    else:
+        prom_data += f'nakivo_api_authentication_error{{host="{host}"}} 0\n'
 
-    prom_data = ""
     try:
         license = api.get_license_info()
         if not license:
             logger.error(f"Cannot get license data for {host}")
-            prom_data = f'nakivo_license_installed{{host="{host}"}} 0'
+            prom_data += f'nakivo_license_installed{{host="{host}"}} 0'
         else:
-            prom_data = license_to_prometheus(license, host)
+            prom_data += license_to_prometheus(license, host)
     except Exception as exc:
         logger.error(f"Cannot retrieve license data for {host}: {exc}")
         logger.debug("Trace", exc_info=True)
 
     try:
         jobs = api.get_jobs()
         if not jobs:
```

### Comparing `nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter/server.py` & `nakivo_prometheus_exporter-0.3.0/nakivo_prometheus_exporter/server.py`

 * *Files identical despite different names*

### Comparing `nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter.egg-info/PKG-INFO` & `nakivo_prometheus_exporter-0.3.0/nakivo_prometheus_exporter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nakivo_prometheus_exporter
-Version: 0.2.3
+Version: 0.3.0
 Summary: Connecto to Nakivo API and export metrics to Prometheus
 Home-page: https://github.com/netinvent/nakivo_prometheus_exporter
 Author: NetInvent - Orsiris de Jong
 Author-email: contact@netinvent.fr
 License: GPLv3
 Keywords: shell,backup,prometheus,linux,cli
 Classifier: Development Status :: 5 - Production/Stable
@@ -116,15 +116,15 @@
 If everything works, you can use the provided systemd service file from the systemd directory, copy it into `/etc/systemd/system` and run the service with
 ```
 systemctl enable --now nakivo_prometheus_exporter
 ```
 
 ## Caveats
 
-Since on every scraping, the exporter connects to *ALL* Nakivo API endpoints defined in the host section, you should set the scraper interval to something reasonable like 1 hour.
+Since on every scraping, the exporter connects to *ALL* Nakivo API endpoints defined in the host section, you should set the scraper interval to something reasonable like 1 hour, and increase the scrape timeout value to one minute (see the `prometheus.yml` example file).
 
 ## Other caveats
 
 This is a quick and dirty proof of concept, only fetching  backup states/duration/sizes and licensing state.  
 There's still quiescing information missing (didn't find it in the (Nakivo API)[https://helpcenter.nakivo.com/api-reference/Content/API-Reference-Overview.htm])
 
 If some traction is obersved for the project, we might add missing or interesting metrics.
```

### Comparing `nakivo_prometheus_exporter-0.2.3/nakivo_prometheus_exporter.egg-info/SOURCES.txt` & `nakivo_prometheus_exporter-0.3.0/nakivo_prometheus_exporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nakivo_prometheus_exporter-0.2.3/setup.py` & `nakivo_prometheus_exporter-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,19 +89,23 @@
 
 package_path = os.path.abspath(PACKAGE_NAME)
 for path in ["__main__.py", PACKAGE_NAME + ".py"]:
     package_file = os.path.join(package_path, "__version__.py")
     if os.path.isfile(package_file):
         break
 metadata = get_metadata(package_file)
-requirements = parse_requirements(os.path.join(package_path, os.pardir, "requirements.txt"))
+requirements = parse_requirements(
+    os.path.join(package_path, os.pardir, "requirements.txt")
+)
 long_description = _read_file("README.md")
 
 
-console_scripts = ["nakivo_prometheus_exporter = nakivo_prometheus_exporter.server:main"]
+console_scripts = [
+    "nakivo_prometheus_exporter = nakivo_prometheus_exporter.server:main"
+]
 setuptools.setup(
     name=PACKAGE_NAME,
     # We may use find_packages in order to not specify each package manually
     # packages = ['command_runner'],
     packages=setuptools.find_packages(),
     version=metadata["version"],
     install_requires=requirements,
```

