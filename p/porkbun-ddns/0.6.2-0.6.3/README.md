# Comparing `tmp/porkbun_ddns-0.6.2-py3-none-any.whl.zip` & `tmp/porkbun_ddns-0.6.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9190 bytes, number of entries: 10
--rw-r--r--  2.0 unx       82 b- defN 24-Apr-15 06:10 porkbun_ddns/__init__.py
--rw-r--r--  2.0 unx     3254 b- defN 24-Apr-15 06:10 porkbun_ddns/cli.py
--rw-r--r--  2.0 unx     1475 b- defN 24-Apr-15 06:10 porkbun_ddns/helpers.py
--rw-r--r--  2.0 unx    10256 b- defN 24-Apr-15 06:10 porkbun_ddns/porkbun_ddns.py
--rw-r--r--  2.0 unx     1061 b- defN 24-Apr-15 06:10 porkbun_ddns-0.6.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     5532 b- defN 24-Apr-15 06:10 porkbun_ddns-0.6.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-15 06:10 porkbun_ddns-0.6.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 24-Apr-15 06:10 porkbun_ddns-0.6.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 24-Apr-15 06:10 porkbun_ddns-0.6.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      832 b- defN 24-Apr-15 06:10 porkbun_ddns-0.6.2.dist-info/RECORD
-10 files, 22652 bytes uncompressed, 7762 bytes compressed:  65.7%
+Zip file size: 9170 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       82 b- defN 24-Apr-25 12:44 porkbun_ddns/__init__.py
+-rw-r--r--  2.0 unx     3254 b- defN 24-Apr-25 12:44 porkbun_ddns/cli.py
+-rw-r--r--  2.0 unx     1475 b- defN 24-Apr-25 12:44 porkbun_ddns/helpers.py
+-rw-r--r--  2.0 unx    10274 b- defN 24-Apr-25 12:44 porkbun_ddns/porkbun_ddns.py
+-rw-r--r--  2.0 unx     1061 b- defN 24-Apr-25 12:44 porkbun_ddns-0.6.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5532 b- defN 24-Apr-25 12:44 porkbun_ddns-0.6.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 12:44 porkbun_ddns-0.6.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 24-Apr-25 12:44 porkbun_ddns-0.6.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-25 12:44 porkbun_ddns-0.6.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      832 b- defN 24-Apr-25 12:44 porkbun_ddns-0.6.3.dist-info/RECORD
+10 files, 22670 bytes uncompressed, 7742 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: porkbun_ddns/helpers.py
 Comment: 
 
 Filename: porkbun_ddns/porkbun_ddns.py
 Comment: 
 
-Filename: porkbun_ddns-0.6.2.dist-info/LICENSE
+Filename: porkbun_ddns-0.6.3.dist-info/LICENSE
 Comment: 
 
-Filename: porkbun_ddns-0.6.2.dist-info/METADATA
+Filename: porkbun_ddns-0.6.3.dist-info/METADATA
 Comment: 
 
-Filename: porkbun_ddns-0.6.2.dist-info/WHEEL
+Filename: porkbun_ddns-0.6.3.dist-info/WHEEL
 Comment: 
 
-Filename: porkbun_ddns-0.6.2.dist-info/entry_points.txt
+Filename: porkbun_ddns-0.6.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: porkbun_ddns-0.6.2.dist-info/top_level.txt
+Filename: porkbun_ddns-0.6.3.dist-info/top_level.txt
 Comment: 
 
-Filename: porkbun_ddns-0.6.2.dist-info/RECORD
+Filename: porkbun_ddns-0.6.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## porkbun_ddns/porkbun_ddns.py

```diff
@@ -85,36 +85,36 @@
                     public_ips.append(
                         get_ips_from_fritzbox(self.fritzbox_ip))
             else:
                 if self.ipv4:
                     urls = ['https://v4.ident.me',
                     'https://api.ipify.org',
                     'https://ipv4.icanhazip.com']
-                    try:
-                        for url in urls:
+                    for url in urls:
+                        try:
                             with urllib.request.urlopen(url) as response:
                                 if response.getcode() == 200:
                                     public_ips.append(response.read().decode('utf-8'))
                                     break
                                 logger.warning("Failed to retrieve IPv4 Address from %s! HTTP status code: %s", url, str(response.code()))
-                    except URLError:
-                        logger.warning("Can't reach IPv4 Address! Check IPv4 connectivity!")
+                        except URLError as err:
+                            logger.warning("Error reaching %s! Error: %s", url, repr(err))
                 if self.ipv6:
                     urls = ['https://v6.ident.me',
                     'https://api6.ipify.org',
                     'https://ipv6.icanhazip.com']
-                    try:
-                        for url in urls:
+                    for url in urls:
+                        try:
                             with urllib.request.urlopen(url) as response:
                                 if response.getcode() == 200:
                                     public_ips.append(response.read().decode('utf-8'))
                                     break
                                 logger.warning("Failed to retrieve IPv6 Address from %s! HTTP status code: %s", url, str(response.code()))
-                    except URLError:
-                        logger.warning("Can't reach IPv6 Address! Check IPv6 connectivity!")
+                        except URLError as err:
+                            logger.warning("Error reaching %s! Error: %s", url, repr(err))
 
             public_ips = set(public_ips)
 
         if not public_ips:
             raise PorkbunDDNS_Error('Failed to obtain IP Addresses!')
 
         return [ipaddress.ip_address(x) for x in public_ips if not ipaddress.ip_address(x).is_unspecified]
```

## Comparing `porkbun_ddns-0.6.2.dist-info/LICENSE` & `porkbun_ddns-0.6.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `porkbun_ddns-0.6.2.dist-info/METADATA` & `porkbun_ddns-0.6.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: porkbun-ddns
-Version: 0.6.2
+Version: 0.6.3
 Summary: A unofficial DDNS-Client for Porkbun domains
 Home-page: https://github.com/mietzen/porkbun-ddns
 Author: Nils Stein
 Author-email: github.nstein@mailbox.org
 License: MIT
 Keywords: porkbun ddns
 Classifier: Development Status :: 4 - Beta
```

## Comparing `porkbun_ddns-0.6.2.dist-info/RECORD` & `porkbun_ddns-0.6.3.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 porkbun_ddns/__init__.py,sha256=4E9knps0KH0NhbKGNNEeixpexHTNnxHbfUvhJD7rOUU,82
 porkbun_ddns/cli.py,sha256=WQJEcM4qsmpODHd83X_gA9fDJ-OTNbjzceZlO4EpL24,3254
 porkbun_ddns/helpers.py,sha256=i3OPqrDzMJTuhuGC18V2qerYI_i77dSF-nFIQMBcSEM,1475
-porkbun_ddns/porkbun_ddns.py,sha256=B6P0kSVEG_E6AsyQXOWIctd1sFznWCs8WIVZr8r4dZU,10256
-porkbun_ddns-0.6.2.dist-info/LICENSE,sha256=WbmjIVUkxwQ1vDNiEe2eMKL3-6nYRBN1qUv7rdvvSvY,1061
-porkbun_ddns-0.6.2.dist-info/METADATA,sha256=kF_KNairMrlu-UJbMeu8xD9yCTu2u4gH5DP0K7LYe0Y,5532
-porkbun_ddns-0.6.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-porkbun_ddns-0.6.2.dist-info/entry_points.txt,sha256=Ux4_6ekA_PZiOxw-7MbJOvQVo_7IJQzaYS24EzSjwbg,55
-porkbun_ddns-0.6.2.dist-info/top_level.txt,sha256=8hi5L7CGOlYLIOlnnPPToRxZqnZ1UkpUmCYbgYZO2JA,13
-porkbun_ddns-0.6.2.dist-info/RECORD,,
+porkbun_ddns/porkbun_ddns.py,sha256=RwhP3CRGSTRHxtgYrLhHaF1tzDCTncNaJWFDQfuZeNU,10274
+porkbun_ddns-0.6.3.dist-info/LICENSE,sha256=WbmjIVUkxwQ1vDNiEe2eMKL3-6nYRBN1qUv7rdvvSvY,1061
+porkbun_ddns-0.6.3.dist-info/METADATA,sha256=rJyI6UUe0rHD9KbJbn0mXqfNbWqpr-GKOKYTCr-DcTs,5532
+porkbun_ddns-0.6.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+porkbun_ddns-0.6.3.dist-info/entry_points.txt,sha256=Ux4_6ekA_PZiOxw-7MbJOvQVo_7IJQzaYS24EzSjwbg,55
+porkbun_ddns-0.6.3.dist-info/top_level.txt,sha256=8hi5L7CGOlYLIOlnnPPToRxZqnZ1UkpUmCYbgYZO2JA,13
+porkbun_ddns-0.6.3.dist-info/RECORD,,
```

