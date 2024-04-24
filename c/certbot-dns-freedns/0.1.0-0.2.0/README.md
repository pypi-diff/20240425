# Comparing `tmp/certbot-dns-freedns-0.1.0.tar.gz` & `tmp/certbot_dns_freedns-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-dns-freedns-0.1.0.tar", last modified: Wed Nov 16 18:35:54 2022, max compression
+gzip compressed data, was "certbot_dns_freedns-0.2.0.tar", last modified: Wed Apr 24 23:36:20 2024, max compression
```

## Comparing `certbot-dns-freedns-0.1.0.tar` & `certbot_dns_freedns-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2022-11-16 18:35:54.235760 certbot-dns-freedns-0.1.0/
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     1022 2022-11-16 17:57:28.000000 certbot-dns-freedns-0.1.0/LICENSE.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     6130 2022-11-16 18:35:54.235760 certbot-dns-freedns-0.1.0/PKG-INFO
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     4388 2022-11-16 18:35:49.000000 certbot-dns-freedns-0.1.0/README.rst
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2022-11-16 18:35:54.235760 certbot-dns-freedns-0.1.0/certbot_dns_freedns/
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     3101 2022-11-16 17:43:53.000000 certbot-dns-freedns-0.1.0/certbot_dns_freedns/__init__.py
--rw-rw-r--   0 rafael    (1000) rafael    (1000)    11791 2022-11-16 17:43:53.000000 certbot-dns-freedns-0.1.0/certbot_dns_freedns/dns_freedns.py
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2022-11-16 18:35:54.235760 certbot-dns-freedns-0.1.0/certbot_dns_freedns.egg-info/
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     6130 2022-11-16 18:35:54.000000 certbot-dns-freedns-0.1.0/certbot_dns_freedns.egg-info/PKG-INFO
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      383 2022-11-16 18:35:54.000000 certbot-dns-freedns-0.1.0/certbot_dns_freedns.egg-info/SOURCES.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)        1 2022-11-16 18:35:54.000000 certbot-dns-freedns-0.1.0/certbot_dns_freedns.egg-info/dependency_links.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       78 2022-11-16 18:35:54.000000 certbot-dns-freedns-0.1.0/certbot_dns_freedns.egg-info/entry_points.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       68 2022-11-16 18:35:54.000000 certbot-dns-freedns-0.1.0/certbot_dns_freedns.egg-info/requires.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       20 2022-11-16 18:35:54.000000 certbot-dns-freedns-0.1.0/certbot_dns_freedns.egg-info/top_level.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      737 2022-11-16 18:26:52.000000 certbot-dns-freedns-0.1.0/pyproject.toml
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       67 2022-11-16 18:35:54.235760 certbot-dns-freedns-0.1.0/setup.cfg
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     1849 2022-11-16 17:43:53.000000 certbot-dns-freedns-0.1.0/setup.py
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-04-24 23:36:20.161605 certbot_dns_freedns-0.2.0/
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     1022 2022-11-16 17:57:28.000000 certbot_dns_freedns-0.2.0/LICENSE.txt
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     6273 2024-04-24 23:36:20.161605 certbot_dns_freedns-0.2.0/PKG-INFO
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     4388 2022-11-16 18:35:49.000000 certbot_dns_freedns-0.2.0/README.rst
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-04-24 23:36:20.161605 certbot_dns_freedns-0.2.0/certbot_dns_freedns/
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     3101 2022-11-16 17:43:53.000000 certbot_dns_freedns-0.2.0/certbot_dns_freedns/__init__.py
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)    11444 2024-04-24 23:27:25.000000 certbot_dns_freedns-0.2.0/certbot_dns_freedns/dns_freedns.py
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-04-24 23:36:20.161605 certbot_dns_freedns-0.2.0/certbot_dns_freedns.egg-info/
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     6273 2024-04-24 23:36:20.000000 certbot_dns_freedns-0.2.0/certbot_dns_freedns.egg-info/PKG-INFO
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)      383 2024-04-24 23:36:20.000000 certbot_dns_freedns-0.2.0/certbot_dns_freedns.egg-info/SOURCES.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)        1 2024-04-24 23:36:20.000000 certbot_dns_freedns-0.2.0/certbot_dns_freedns.egg-info/dependency_links.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       78 2024-04-24 23:36:20.000000 certbot_dns_freedns-0.2.0/certbot_dns_freedns.egg-info/entry_points.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       68 2024-04-24 23:36:20.000000 certbot_dns_freedns-0.2.0/certbot_dns_freedns.egg-info/requires.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       20 2024-04-24 23:36:20.000000 certbot_dns_freedns-0.2.0/certbot_dns_freedns.egg-info/top_level.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     1230 2024-04-24 23:35:13.000000 certbot_dns_freedns-0.2.0/pyproject.toml
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       67 2024-04-24 23:36:20.161605 certbot_dns_freedns-0.2.0/setup.cfg
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     1849 2024-04-24 23:25:57.000000 certbot_dns_freedns-0.2.0/setup.py
```

### Comparing `certbot-dns-freedns-0.1.0/LICENSE.txt` & `certbot_dns_freedns-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-freedns-0.1.0/PKG-INFO` & `certbot_dns_freedns-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-freedns
-Version: 0.1.0
+Version: 0.2.0
 Summary: FreeDNS Authenticator plugin for Certbot
 Home-page: https://github.com/schleuss/certbot-dns-freedns
 Author: Rafael Schleuss
 Author-email: Rafael Schleuss <rschleuss@gmail.com>
 License: Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
@@ -27,14 +27,19 @@
 Keywords: FreeDNS,Certbot
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: acme>=1.22.0
+Requires-Dist: certbot>=1.22.0
+Requires-Dist: setuptools
+Requires-Dist: requests>=2.26.0
+Requires-Dist: bs4>=0.0.1
 
 certbot-dns-freedns
 ===================
 
 FreeDNS - DNS Authenticator plugin for Certbot
 
 This plugin automates the process of completing a ``dns-01`` challenge
```

### Comparing `certbot-dns-freedns-0.1.0/README.rst` & `certbot_dns_freedns-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `certbot-dns-freedns-0.1.0/certbot_dns_freedns/__init__.py` & `certbot_dns_freedns-0.2.0/certbot_dns_freedns/__init__.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-freedns-0.1.0/certbot_dns_freedns/dns_freedns.py` & `certbot_dns_freedns-0.2.0/certbot_dns_freedns/dns_freedns.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 class Authenticator(dns_common.DNSAuthenticator):
     """DNS Authenticator for FreeDNS
 
     This Authenticator uses the FreeDNS Remote REST API to fulfill a dns-01 challenge.
     """
 
     description = "Obtain certificates using a DNS TXT record (if you are using FreeDNS for DNS)."
-    ttl = 60
 
     def __init__(self, *args, **kwargs):
         super(Authenticator, self).__init__(*args, **kwargs)
         self.credentials = None
 
     @classmethod
     def add_parser_arguments(cls, add):  # pylint: disable=arguments-differ
@@ -50,20 +49,20 @@
                 "username": "Username for FreeDNS Remote API.",
                 "password": "Password for FreeDNS Remote API.",
             },
         )
 
     def _perform(self, domain, validation_name, validation):
         self._get_freedns_client().add_txt_record(
-            domain, validation_name, validation, self.ttl
+            domain, validation_name, validation
         )
 
     def _cleanup(self, domain, validation_name, validation):
         self._get_freedns_client().del_txt_record(
-            domain, validation_name, validation, self.ttl
+            domain, validation_name, validation
         )
 
     def _get_freedns_client(self):
         return _FreeDNSClient(
             self.credentials.conf("username"),
             self.credentials.conf("password"),
         )
@@ -95,15 +94,15 @@
         if response.status_code == 200:
             return True
         return False
 
     def _get_url(self, path):
         return "{0}{1}".format(self.endpoint, path)
 
-    def add_txt_record(self, domain, record_name, record_content, record_ttl):
+    def add_txt_record(self, domain, record_name, record_content):
         self._login()
         zone_id, zone_name = self._find_managed_zone_id(domain)
         if zone_id is None:
             raise errors.PluginError("Domain not known")
         logger.debug("domain found: %s with id: %s", zone_name, zone_id)
 
         o_record_name = record_name
@@ -117,21 +116,21 @@
         if record is not None:
             if record["data"] == record_content:
                 logger.info("already there, id {0}".format(record["id"]))
                 return
             else:
                 logger.info("update {0}".format(record["id"]))
                 self._update_txt_record(
-                    zone_id, record["id"], record_name, record_content, record_ttl
+                    zone_id, record["id"], record_name, record_content
                 )
         else:
             logger.info("insert new txt record")
-            self._insert_txt_record(zone_id, record_name, record_content, record_ttl)
+            self._insert_txt_record(zone_id, record_name, record_content)
 
-    def del_txt_record(self, domain, record_name, record_content, record_ttl):
+    def del_txt_record(self, domain, record_name, record_content):
         self._login()
         zone_id, zone_name = self._find_managed_zone_id(domain)
         
         if zone_id is None:
             raise errors.PluginError("Domain not known")
 
         logger.debug("domain found: %s with id: %s", zone_name, zone_id)
@@ -150,36 +149,33 @@
     def _del_txt_record(self, record_id):
         if record_id is not None:
             response = self.session.post("{}/subdomain/delete2.php?data_id%5B%5D={}&submit=delete+selected".format(self.endpoint, record_id))
             if response.status_code == 200:
                     return True
         return False
 
-    def _insert_txt_record(self, zone_id, record_name, record_content, record_ttl):
-        logger.debug("insert with data: %s", (zone_id, record_name, record_content, record_ttl))
-        return self._edit_txt_record(zone_id, None, record_name, record_content, record_ttl)
-
-    def _update_txt_record(self, zone_id, primary_id, record_name, record_content, record_ttl):
-        logger.debug("update with data: %s", (zone_id, primary_id, record_name, record_content, record_ttl))
-        return self._edit_txt_record(zone_id, primary_id, record_name, record_content, record_ttl)
+    def _insert_txt_record(self, zone_id, record_name, record_content):
+        logger.debug("insert with data: %s", (zone_id, record_name, record_content))
+        return self._edit_txt_record(zone_id, None, record_name, record_content)
+
+    def _update_txt_record(self, zone_id, primary_id, record_name, record_content):
+        logger.debug("update with data: %s", (zone_id, primary_id, record_name, record_content))
+        return self._edit_txt_record(zone_id, primary_id, record_name, record_content)
 
-    def _edit_txt_record(self, zone_id, primary_id, record_name, record_content, record_ttl):
+    def _edit_txt_record(self, zone_id, primary_id, record_name, record_content):
         # Valid types: A, AAAA, CNAME, CAA, NS, MX, TXT, SPF, LOC, HINFO, RP, SRV, SSHFP, 
         txt_data = '"{}"'.format(record_content)
         params = {"type": "TXT", 
                 "subdomain": record_name, 
                 "domain_id": zone_id,
                 "address": txt_data, 
                 "send": "Save%21"}
 
         if primary_id is not None:
             params["data_id"] = primary_id
-    
-        if record_ttl is not None:
-            params["ttl"] = record_ttl    
 
         response = self.session.post(self.endpoint+"/subdomain/save.php?step=2", data=params)
         if response.status_code == 200:
             soup = BeautifulSoup(response.text, "html.parser")
             title = soup.find("title")
             if "Problems" not in title.text:
                 return True
@@ -279,15 +275,14 @@
         response = self.session.get("{}/subdomain/edit.php?data_id={}".format(self.endpoint, freedns_record_id))
         if response.status_code == 200:
             soup = BeautifulSoup(response.text, "html.parser")
             form = soup.find("form", action="save.php?step=2")
 
             if form is not None:
                 input_wildcard = soup.find("input", recursive=True, attrs={"name": "wildcard"}).get("value")
-                input_ttl = soup.find("input", recursive=True, attrs={"name": "ttl"}).get("value")
                 input_address = soup.find("input", recursive=True, attrs={"name": "address"}).get("value")
                 input_subdomain = soup.find("input", recursive=True, attrs={"name": "subdomain"}).get("value")
 
                 record_data = {}
                 record_data["id"] = freedns_record_id
                 record_data["domain_id"] = freedns_domain_id
                 record_data["wildcard"] = input_wildcard
```

### Comparing `certbot-dns-freedns-0.1.0/certbot_dns_freedns.egg-info/PKG-INFO` & `certbot_dns_freedns-0.2.0/certbot_dns_freedns.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-freedns
-Version: 0.1.0
+Version: 0.2.0
 Summary: FreeDNS Authenticator plugin for Certbot
 Home-page: https://github.com/schleuss/certbot-dns-freedns
 Author: Rafael Schleuss
 Author-email: Rafael Schleuss <rschleuss@gmail.com>
 License: Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
@@ -27,14 +27,19 @@
 Keywords: FreeDNS,Certbot
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: acme>=1.22.0
+Requires-Dist: certbot>=1.22.0
+Requires-Dist: setuptools
+Requires-Dist: requests>=2.26.0
+Requires-Dist: bs4>=0.0.1
 
 certbot-dns-freedns
 ===================
 
 FreeDNS - DNS Authenticator plugin for Certbot
 
 This plugin automates the process of completing a ``dns-01`` challenge
```

### Comparing `certbot-dns-freedns-0.1.0/setup.py` & `certbot_dns_freedns-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 from setuptools import find_packages
 
-version = "0.1.0"
+version = "0.2.0"
 
 install_requires = [
     "acme>=1.22.0",
     "certbot>=1.22.0",
     "setuptools",
     "requests>=2.26.0",
     "bs4>=0.0.1",
```

