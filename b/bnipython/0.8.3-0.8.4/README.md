# Comparing `tmp/bnipython-0.8.3.tar.gz` & `tmp/bnipython-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bnipython-0.8.3.tar", last modified: Fri Mar 22 12:03:43 2024, max compression
+gzip compressed data, was "bnipython-0.8.4.tar", last modified: Thu Apr 25 06:13:49 2024, max compression
```

## Comparing `bnipython-0.8.3.tar` & `bnipython-0.8.4.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 12:03:42.999515 bnipython-0.8.3/
--rw-rw-rw-   0        0        0     1085 2023-11-02 12:35:34.000000 bnipython-0.8.3/LICENSE
--rw-rw-rw-   0        0        0    40399 2024-03-22 12:03:42.998518 bnipython-0.8.3/PKG-INFO
--rw-rw-rw-   0        0        0    39483 2024-03-22 11:34:14.000000 bnipython-0.8.3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-22 12:03:42.960215 bnipython-0.8.3/bnipython/
--rw-rw-rw-   0        0        0      478 2024-03-22 11:34:10.000000 bnipython-0.8.3/bnipython/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-22 12:03:42.979162 bnipython-0.8.3/bnipython/lib/
-drwxrwxrwx   0        0        0        0 2024-03-22 12:03:42.985148 bnipython-0.8.3/bnipython/lib/api/
--rw-rw-rw-   0        0        0     9414 2023-11-02 12:35:34.000000 bnipython-0.8.3/bnipython/lib/api/oneGatePayment.py
--rw-rw-rw-   0        0        0    21611 2023-11-02 12:35:34.000000 bnipython-0.8.3/bnipython/lib/api/rdf.py
--rw-rw-rw-   0        0        0    22000 2023-11-02 12:35:34.000000 bnipython-0.8.3/bnipython/lib/api/rdl.py
--rw-rw-rw-   0        0        0    25305 2023-11-15 02:03:49.000000 bnipython-0.8.3/bnipython/lib/api/rdn.py
--rw-rw-rw-   0        0        0    23158 2024-03-22 11:34:14.000000 bnipython-0.8.3/bnipython/lib/api/snapBI.py
--rw-rw-rw-   0        0        0     1070 2024-03-22 11:34:14.000000 bnipython-0.8.3/bnipython/lib/bniClient.py
-drwxrwxrwx   0        0        0        0 2024-03-22 12:03:42.986144 bnipython-0.8.3/bnipython/lib/net/
--rw-rw-rw-   0        0        0     4156 2024-03-22 11:34:14.000000 bnipython-0.8.3/bnipython/lib/net/httpClient.py
-drwxrwxrwx   0        0        0        0 2024-03-22 12:03:42.989136 bnipython-0.8.3/bnipython/lib/util/
--rw-rw-rw-   0        0        0      195 2024-03-22 12:00:02.000000 bnipython-0.8.3/bnipython/lib/util/constants.py
--rw-rw-rw-   0        0        0     3966 2024-03-22 11:34:14.000000 bnipython-0.8.3/bnipython/lib/util/response.py
--rw-rw-rw-   0        0        0     2707 2024-03-22 11:34:14.000000 bnipython-0.8.3/bnipython/lib/util/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-22 12:03:42.996522 bnipython-0.8.3/bnipython.egg-info/
--rw-rw-rw-   0        0        0    40399 2024-03-22 12:03:42.000000 bnipython-0.8.3/bnipython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      652 2024-03-22 12:03:42.000000 bnipython-0.8.3/bnipython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 12:03:42.000000 bnipython-0.8.3/bnipython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-03-22 12:03:42.000000 bnipython-0.8.3/bnipython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-22 12:03:42.000000 bnipython-0.8.3/bnipython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-22 12:03:42.999515 bnipython-0.8.3/setup.cfg
--rw-rw-rw-   0        0        0     1386 2024-03-22 12:01:59.000000 bnipython-0.8.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-22 12:03:42.995526 bnipython-0.8.3/tests/
--rw-rw-rw-   0        0        0     1971 2023-11-02 12:35:34.000000 bnipython-0.8.3/tests/test_bni_client.py
--rw-rw-rw-   0        0        0    10576 2023-11-02 12:35:34.000000 bnipython-0.8.3/tests/test_one_gate_payment.py
--rw-rw-rw-   0        0        0    19877 2023-11-02 12:35:34.000000 bnipython-0.8.3/tests/test_rdf.py
--rw-rw-rw-   0        0        0    19851 2023-11-02 12:35:34.000000 bnipython-0.8.3/tests/test_rdl.py
--rw-rw-rw-   0        0        0    23553 2023-11-02 12:35:34.000000 bnipython-0.8.3/tests/test_rdn.py
--rw-rw-rw-   0        0        0    35028 2024-03-22 11:34:14.000000 bnipython-0.8.3/tests/test_snap_bi.py
--rw-rw-rw-   0        0        0     1093 2023-11-02 12:35:34.000000 bnipython-0.8.3/tests/test_util.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:13:49.918058 bnipython-0.8.4/
+-rw-rw-rw-   0        0        0     1085 2023-11-02 12:35:34.000000 bnipython-0.8.4/LICENSE
+-rw-rw-rw-   0        0        0    42304 2024-04-25 06:13:49.916062 bnipython-0.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0    41388 2024-04-25 06:07:02.000000 bnipython-0.8.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 06:13:49.863372 bnipython-0.8.4/bnipython/
+-rw-rw-rw-   0        0        0      559 2024-04-25 06:07:02.000000 bnipython-0.8.4/bnipython/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:13:49.886312 bnipython-0.8.4/bnipython/lib/
+drwxrwxrwx   0        0        0        0 2024-04-25 06:13:49.894289 bnipython-0.8.4/bnipython/lib/api/
+-rw-rw-rw-   0        0        0     2455 2024-04-25 06:07:02.000000 bnipython-0.8.4/bnipython/lib/api/bniMove.py
+-rw-rw-rw-   0        0        0     9414 2023-11-02 12:35:34.000000 bnipython-0.8.4/bnipython/lib/api/oneGatePayment.py
+-rw-rw-rw-   0        0        0    21611 2023-11-02 12:35:34.000000 bnipython-0.8.4/bnipython/lib/api/rdf.py
+-rw-rw-rw-   0        0        0    22000 2023-11-02 12:35:34.000000 bnipython-0.8.4/bnipython/lib/api/rdl.py
+-rw-rw-rw-   0        0        0    25305 2023-11-15 02:03:49.000000 bnipython-0.8.4/bnipython/lib/api/rdn.py
+-rw-rw-rw-   0        0        0    23158 2024-04-17 07:27:54.000000 bnipython-0.8.4/bnipython/lib/api/snapBI.py
+-rw-rw-rw-   0        0        0     1070 2024-04-17 07:27:54.000000 bnipython-0.8.4/bnipython/lib/bniClient.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:13:49.896283 bnipython-0.8.4/bnipython/lib/net/
+-rw-rw-rw-   0        0        0     4156 2024-04-17 07:27:54.000000 bnipython-0.8.4/bnipython/lib/net/httpClient.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:13:49.900272 bnipython-0.8.4/bnipython/lib/util/
+-rw-rw-rw-   0        0        0      197 2024-04-25 06:13:04.000000 bnipython-0.8.4/bnipython/lib/util/constants.py
+-rw-rw-rw-   0        0        0     4394 2024-04-25 06:07:02.000000 bnipython-0.8.4/bnipython/lib/util/response.py
+-rw-rw-rw-   0        0        0     2840 2024-04-25 06:07:02.000000 bnipython-0.8.4/bnipython/lib/util/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:13:49.914237 bnipython-0.8.4/bnipython.egg-info/
+-rw-rw-rw-   0        0        0    42304 2024-04-25 06:13:49.000000 bnipython-0.8.4/bnipython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      704 2024-04-25 06:13:49.000000 bnipython-0.8.4/bnipython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 06:13:49.000000 bnipython-0.8.4/bnipython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-25 06:13:49.000000 bnipython-0.8.4/bnipython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-25 06:13:49.000000 bnipython-0.8.4/bnipython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 06:13:49.918058 bnipython-0.8.4/setup.cfg
+-rw-rw-rw-   0        0        0     1386 2024-04-25 06:07:02.000000 bnipython-0.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:13:49.913238 bnipython-0.8.4/tests/
+-rw-rw-rw-   0        0        0     1971 2023-11-02 12:35:34.000000 bnipython-0.8.4/tests/test_bni_client.py
+-rw-rw-rw-   0        0        0    15863 2024-04-25 06:07:02.000000 bnipython-0.8.4/tests/test_bni_move.py
+-rw-rw-rw-   0        0        0    10576 2023-11-02 12:35:34.000000 bnipython-0.8.4/tests/test_one_gate_payment.py
+-rw-rw-rw-   0        0        0    19877 2023-11-02 12:35:34.000000 bnipython-0.8.4/tests/test_rdf.py
+-rw-rw-rw-   0        0        0    19851 2023-11-02 12:35:34.000000 bnipython-0.8.4/tests/test_rdl.py
+-rw-rw-rw-   0        0        0    23553 2023-11-02 12:35:34.000000 bnipython-0.8.4/tests/test_rdn.py
+-rw-rw-rw-   0        0        0    35028 2024-04-17 07:27:54.000000 bnipython-0.8.4/tests/test_snap_bi.py
+-rw-rw-rw-   0        0        0     1093 2023-11-02 12:35:34.000000 bnipython-0.8.4/tests/test_util.py
```

### Comparing `bnipython-0.8.3/LICENSE` & `bnipython-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bnipython-0.8.3/PKG-INFO` & `bnipython-0.8.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: bnipython
-Version: 0.8.3
-Summary: Official  BNI API SDK for Python
-Home-page: https://github.com/bni-api/bni-python/
-Author: BNI API
-Author-email: 
-License: MIT
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.25.0
-Requires-Dist: pyOpenSSL>=22.0.0
-Requires-Dist: pytz>=2022.2.1
-
 
 BNI API SDK - Python
 ===============
 This is the Official Python API client / library for BNI API. 
 Please visit [Digital Services](https://digitalservices.bni.co.id/en/) for more information about our product and visit our documentation page at [API Documentation](https://digitalservices.bni.co.id/documentation/public/en) for more technical details.
 
 ## 1. Installation
@@ -391,15 +366,15 @@
     'deviceId': '09864ADCASA', # optional
     'channel': 'API' # optional
   }
 })
 
 ```
 
-### 2.3.C RDN
+### 2.2.C RDN
 Create `RDN` class object
 ```python
 from bnipython import BNIClient, RDN
 
 # Create Client instance
 client = BNIClient({
   'env': False,
@@ -643,15 +618,15 @@
   'beneficiaryAccountName': 'KEN AROK', # Get from Inquiry Interbank Account
   'beneficiaryBankCode': '014', 
   'beneficiaryBankName': 'BANK BCA',  # Get from Inquiry Interbank Account
   'amount': '15000' # Total payment/transfer
 })
 ```
 
-### 2.4.C RDL
+### 2.2.C RDL
 Create `RDL` class object
 ```python
 from bnipython import BNIClient, RDL
 
 # Create Client instance
 client = BNIClient({
   'env': False,
@@ -876,15 +851,15 @@
   'beneficiaryAccountName': 'KEN AROK', # Get from Inquiry Interbank Account
   'beneficiaryBankCode': '014', 
   'beneficiaryBankName': 'BANK BCA',  # Get from Inquiry Interbank Account
   'amount': '15000' # Total payment/transfer
 })
 ```
 
-### 2.5.E RDF
+### 2.2.E RDF
 Create `RDF` class object
 ```python
 from bnipython import BNIClient, RDF
 
 # Create Client instance
 client = BNIClient({
   'env': False,
@@ -1108,14 +1083,74 @@
   'beneficiaryAccountNumber': '3333333333', # Transfer/payment receiver account number
   'beneficiaryAccountName': 'KEN AROK', # Get from Inquiry Interbank Account
   'beneficiaryBankCode': '014', 
   'beneficiaryBankName': 'BANK BCA',  # Get from Inquiry Interbank Account
   'amount': '15000' # Total payment/transfer
 })
 ```
+### 2.2.F BNI Move / Digiloan
+Create `BNIMove` class object
+```python
+from bnipython import BNIClient, BNIMove
+
+# Create Client instance
+client = BNIClient({
+  'env': False,
+  'clientId': '{your-client-id}',
+  'clientSecret': '{your-client-secret}',
+  'apiKey': '{your-api-key}',
+  'apiSecret': '{your-api-secret}',
+  'appName': '{your-app-name}'
+})
+bniMove = BNIMove(client)
+```
+Available methods for `BNIMove` class
+
+#### Prescreening
+```python
+# return as Object
+prescreening = bniMove.prescreening({
+  "kodeMitra":"BNI", # Mitra ID / reference application from mitra
+  "npp":"", # No Refferal (optional)
+  "namaLengkapKtp":"Muhammad Haikal Madani", # Nama lengkap KTP
+  "noKtp":"3174052209980002", # Nomor KTP
+  "noHandphone":"085921658045", # No Handphone
+  "alamatUsaha":"jakarta", # Alamat Usaha
+  "provinsiUsaha":"06", # Provinsi Usaha
+  "kotaUsaha":"143", # Kota Usaha
+  "kecamatanUsaha":"1074", # Kecamatan Usaha
+  "kelurahanUsaha":"4254", # Kelurahan Usaha 
+  "kodePosUsaha":"11450", # Kode Pos Usaha
+  "sektorEkonomi":"2", # Sektor Ekonomi 
+  "totalPenjualan":50000000, # Total Penjualan per bulan
+  "jangkaWaktu":"12", # Jangka waktu / tenor
+  "jenisPinjaman":"1", # Jenis Pinjaman
+  "maximumKredit":50000000, # Maksimum kredit/plafond
+  "jenisKelamin":"1", # Jenis Kelamin
+  "tanggalLahir":"1998-10-07", # Tanggal Lahir
+  "subSektorEkonomi":"050111", # Sub-Sektor Ekonomi
+  "deskripsi":"Usaha Ternak Perikanan", # Deskripsi
+  "email":"muhammadhaikalmadani@mail.com" # Email (optional)
+})
+```
+
+#### Save Image
+```python
+# return as Object
+saveImage = bniMove.saveImage({
+  "Id": "MJO2024022000004", # Id
+  "deskripsi": "Foto Identitas KTP", # Deskripsi 
+  "jenisDokumen": "A03", # Jenis dokumen
+  "namaFile": "Foto KTP", # Nama file
+  "extensionFile": "png", # Extension File
+  "dataBase64": "" # Base64 encoded image file
+})
+```
+
+
 
 ## Get help
 
 * [Digital Services](https://digitalservices.bni.co.id/en/)
 * [API documentation](https://digitalservices.bni.co.id/documentation/public/en)
 * [Stackoverflow](https://stackoverflow.com/users/19817167/bni-api-management)
 * Can't find answer you looking for? email to [apisupport@bni.co.id](mailto:apisupport@bni.co.id)
```

### Comparing `bnipython-0.8.3/README.md` & `bnipython-0.8.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: bnipython
+Version: 0.8.4
+Summary: Official  BNI API SDK for Python
+Home-page: https://github.com/bni-api/bni-python/
+Author: BNI API
+Author-email: 
+License: MIT
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.25.0
+Requires-Dist: pyOpenSSL>=22.0.0
+Requires-Dist: pytz>=2022.2.1
+
 
 BNI API SDK - Python
 ===============
 This is the Official Python API client / library for BNI API. 
 Please visit [Digital Services](https://digitalservices.bni.co.id/en/) for more information about our product and visit our documentation page at [API Documentation](https://digitalservices.bni.co.id/documentation/public/en) for more technical details.
 
 ## 1. Installation
@@ -366,15 +391,15 @@
     'deviceId': '09864ADCASA', # optional
     'channel': 'API' # optional
   }
 })
 
 ```
 
-### 2.3.C RDN
+### 2.2.C RDN
 Create `RDN` class object
 ```python
 from bnipython import BNIClient, RDN
 
 # Create Client instance
 client = BNIClient({
   'env': False,
@@ -618,15 +643,15 @@
   'beneficiaryAccountName': 'KEN AROK', # Get from Inquiry Interbank Account
   'beneficiaryBankCode': '014', 
   'beneficiaryBankName': 'BANK BCA',  # Get from Inquiry Interbank Account
   'amount': '15000' # Total payment/transfer
 })
 ```
 
-### 2.4.C RDL
+### 2.2.C RDL
 Create `RDL` class object
 ```python
 from bnipython import BNIClient, RDL
 
 # Create Client instance
 client = BNIClient({
   'env': False,
@@ -851,15 +876,15 @@
   'beneficiaryAccountName': 'KEN AROK', # Get from Inquiry Interbank Account
   'beneficiaryBankCode': '014', 
   'beneficiaryBankName': 'BANK BCA',  # Get from Inquiry Interbank Account
   'amount': '15000' # Total payment/transfer
 })
 ```
 
-### 2.5.E RDF
+### 2.2.E RDF
 Create `RDF` class object
 ```python
 from bnipython import BNIClient, RDF
 
 # Create Client instance
 client = BNIClient({
   'env': False,
@@ -1083,14 +1108,74 @@
   'beneficiaryAccountNumber': '3333333333', # Transfer/payment receiver account number
   'beneficiaryAccountName': 'KEN AROK', # Get from Inquiry Interbank Account
   'beneficiaryBankCode': '014', 
   'beneficiaryBankName': 'BANK BCA',  # Get from Inquiry Interbank Account
   'amount': '15000' # Total payment/transfer
 })
 ```
+### 2.2.F BNI Move / Digiloan
+Create `BNIMove` class object
+```python
+from bnipython import BNIClient, BNIMove
+
+# Create Client instance
+client = BNIClient({
+  'env': False,
+  'clientId': '{your-client-id}',
+  'clientSecret': '{your-client-secret}',
+  'apiKey': '{your-api-key}',
+  'apiSecret': '{your-api-secret}',
+  'appName': '{your-app-name}'
+})
+bniMove = BNIMove(client)
+```
+Available methods for `BNIMove` class
+
+#### Prescreening
+```python
+# return as Object
+prescreening = bniMove.prescreening({
+  "kodeMitra":"BNI", # Mitra ID / reference application from mitra
+  "npp":"", # No Refferal (optional)
+  "namaLengkapKtp":"Muhammad Haikal Madani", # Nama lengkap KTP
+  "noKtp":"3174052209980002", # Nomor KTP
+  "noHandphone":"085921658045", # No Handphone
+  "alamatUsaha":"jakarta", # Alamat Usaha
+  "provinsiUsaha":"06", # Provinsi Usaha
+  "kotaUsaha":"143", # Kota Usaha
+  "kecamatanUsaha":"1074", # Kecamatan Usaha
+  "kelurahanUsaha":"4254", # Kelurahan Usaha 
+  "kodePosUsaha":"11450", # Kode Pos Usaha
+  "sektorEkonomi":"2", # Sektor Ekonomi 
+  "totalPenjualan":50000000, # Total Penjualan per bulan
+  "jangkaWaktu":"12", # Jangka waktu / tenor
+  "jenisPinjaman":"1", # Jenis Pinjaman
+  "maximumKredit":50000000, # Maksimum kredit/plafond
+  "jenisKelamin":"1", # Jenis Kelamin
+  "tanggalLahir":"1998-10-07", # Tanggal Lahir
+  "subSektorEkonomi":"050111", # Sub-Sektor Ekonomi
+  "deskripsi":"Usaha Ternak Perikanan", # Deskripsi
+  "email":"muhammadhaikalmadani@mail.com" # Email (optional)
+})
+```
+
+#### Save Image
+```python
+# return as Object
+saveImage = bniMove.saveImage({
+  "Id": "MJO2024022000004", # Id
+  "deskripsi": "Foto Identitas KTP", # Deskripsi 
+  "jenisDokumen": "A03", # Jenis dokumen
+  "namaFile": "Foto KTP", # Nama file
+  "extensionFile": "png", # Extension File
+  "dataBase64": "" # Base64 encoded image file
+})
+```
+
+
 
 ## Get help
 
 * [Digital Services](https://digitalservices.bni.co.id/en/)
 * [API documentation](https://digitalservices.bni.co.id/documentation/public/en)
 * [Stackoverflow](https://stackoverflow.com/users/19817167/bni-api-management)
 * Can't find answer you looking for? email to [apisupport@bni.co.id](mailto:apisupport@bni.co.id)
```

### Comparing `bnipython-0.8.3/bnipython/lib/api/oneGatePayment.py` & `bnipython-0.8.4/bnipython/lib/api/oneGatePayment.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.8.3/bnipython/lib/api/rdf.py` & `bnipython-0.8.4/bnipython/lib/api/rdf.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.8.3/bnipython/lib/api/rdl.py` & `bnipython-0.8.4/bnipython/lib/api/rdl.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.8.3/bnipython/lib/api/rdn.py` & `bnipython-0.8.4/bnipython/lib/api/rdn.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.8.3/bnipython/lib/api/snapBI.py` & `bnipython-0.8.4/bnipython/lib/api/snapBI.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.8.3/bnipython/lib/bniClient.py` & `bnipython-0.8.4/bnipython/lib/bniClient.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.8.3/bnipython/lib/net/httpClient.py` & `bnipython-0.8.4/bnipython/lib/net/httpClient.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.8.3/bnipython/lib/util/response.py` & `bnipython-0.8.4/bnipython/lib/util/response.py`

 * *Files 18% similar despite different names*

```diff
@@ -75,8 +75,18 @@
             errorMessage = params['res']['response']['errorMessage']
             raise ValueError(f'\033[91m errorMessage: {errorMessage}, responseMessage: {responseMessage}, code: {code} \033[0m')
         else:
             return params['res']
     except Exception as e:
         code = params['res']['Response']['parameters']['responseCode']
         message = params['res']['Response']['parameters']['responseMessage']
-        raise ValueError(f'\033[91m {code}:{message} \033[0m')
+        raise ValueError(f'\033[91m {code}:{message} \033[0m')
+    
+def responseBNIMove(params={'res'}):
+    status_code = params['res'].get('statusCode')
+    if status_code is None:
+        raise ValueError("Missing status code in response")
+    if status_code != 0:
+        status_message = params['res'].get('statusDescription', 'Unknown Error')
+        error_message = f"Error: {status_code} - {status_message}"
+        raise ValueError(error_message)
+    return params['res']
```

### Comparing `bnipython-0.8.3/bnipython/lib/util/utils.py` & `bnipython-0.8.4/bnipython/lib/util/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 
 def escape(string):
     return string.replace('+', '-').replace('/', '_').replace('=', '')
 
 def getTimestamp():
     return datetime.now(pytz.timezone('Asia/Jakarta')).strftime('%Y-%m-%dT%H:%M:%S+07:00')
 
+def getTimestampBNIMove():
+    return datetime.now(pytz.timezone('Asia/Jakarta')).strftime('%Y-%m-%dT%H:%M:%S.%f')[:-3] + '+07:00'
 
 def generateTokenSignature(params={'privateKeyPath', 'clientId', 'timeStamp'}):
     privateKeyPath = params['privateKeyPath']
     rsaPrivate = privateKeyPath.replace('./', '')
     keyFile = open(f'{rsaPrivate}', 'rb')
     key = keyFile.read()
     keyFile.close()
```

### Comparing `bnipython-0.8.3/bnipython.egg-info/PKG-INFO` & `bnipython-0.8.4/bnipython.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnipython
-Version: 0.8.3
+Version: 0.8.4
 Summary: Official  BNI API SDK for Python
 Home-page: https://github.com/bni-api/bni-python/
 Author: BNI API
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -391,15 +391,15 @@
     'deviceId': '09864ADCASA', # optional
     'channel': 'API' # optional
   }
 })
 
 ```
 
-### 2.3.C RDN
+### 2.2.C RDN
 Create `RDN` class object
 ```python
 from bnipython import BNIClient, RDN
 
 # Create Client instance
 client = BNIClient({
   'env': False,
@@ -643,15 +643,15 @@
   'beneficiaryAccountName': 'KEN AROK', # Get from Inquiry Interbank Account
   'beneficiaryBankCode': '014', 
   'beneficiaryBankName': 'BANK BCA',  # Get from Inquiry Interbank Account
   'amount': '15000' # Total payment/transfer
 })
 ```
 
-### 2.4.C RDL
+### 2.2.C RDL
 Create `RDL` class object
 ```python
 from bnipython import BNIClient, RDL
 
 # Create Client instance
 client = BNIClient({
   'env': False,
@@ -876,15 +876,15 @@
   'beneficiaryAccountName': 'KEN AROK', # Get from Inquiry Interbank Account
   'beneficiaryBankCode': '014', 
   'beneficiaryBankName': 'BANK BCA',  # Get from Inquiry Interbank Account
   'amount': '15000' # Total payment/transfer
 })
 ```
 
-### 2.5.E RDF
+### 2.2.E RDF
 Create `RDF` class object
 ```python
 from bnipython import BNIClient, RDF
 
 # Create Client instance
 client = BNIClient({
   'env': False,
@@ -1108,14 +1108,74 @@
   'beneficiaryAccountNumber': '3333333333', # Transfer/payment receiver account number
   'beneficiaryAccountName': 'KEN AROK', # Get from Inquiry Interbank Account
   'beneficiaryBankCode': '014', 
   'beneficiaryBankName': 'BANK BCA',  # Get from Inquiry Interbank Account
   'amount': '15000' # Total payment/transfer
 })
 ```
+### 2.2.F BNI Move / Digiloan
+Create `BNIMove` class object
+```python
+from bnipython import BNIClient, BNIMove
+
+# Create Client instance
+client = BNIClient({
+  'env': False,
+  'clientId': '{your-client-id}',
+  'clientSecret': '{your-client-secret}',
+  'apiKey': '{your-api-key}',
+  'apiSecret': '{your-api-secret}',
+  'appName': '{your-app-name}'
+})
+bniMove = BNIMove(client)
+```
+Available methods for `BNIMove` class
+
+#### Prescreening
+```python
+# return as Object
+prescreening = bniMove.prescreening({
+  "kodeMitra":"BNI", # Mitra ID / reference application from mitra
+  "npp":"", # No Refferal (optional)
+  "namaLengkapKtp":"Muhammad Haikal Madani", # Nama lengkap KTP
+  "noKtp":"3174052209980002", # Nomor KTP
+  "noHandphone":"085921658045", # No Handphone
+  "alamatUsaha":"jakarta", # Alamat Usaha
+  "provinsiUsaha":"06", # Provinsi Usaha
+  "kotaUsaha":"143", # Kota Usaha
+  "kecamatanUsaha":"1074", # Kecamatan Usaha
+  "kelurahanUsaha":"4254", # Kelurahan Usaha 
+  "kodePosUsaha":"11450", # Kode Pos Usaha
+  "sektorEkonomi":"2", # Sektor Ekonomi 
+  "totalPenjualan":50000000, # Total Penjualan per bulan
+  "jangkaWaktu":"12", # Jangka waktu / tenor
+  "jenisPinjaman":"1", # Jenis Pinjaman
+  "maximumKredit":50000000, # Maksimum kredit/plafond
+  "jenisKelamin":"1", # Jenis Kelamin
+  "tanggalLahir":"1998-10-07", # Tanggal Lahir
+  "subSektorEkonomi":"050111", # Sub-Sektor Ekonomi
+  "deskripsi":"Usaha Ternak Perikanan", # Deskripsi
+  "email":"muhammadhaikalmadani@mail.com" # Email (optional)
+})
+```
+
+#### Save Image
+```python
+# return as Object
+saveImage = bniMove.saveImage({
+  "Id": "MJO2024022000004", # Id
+  "deskripsi": "Foto Identitas KTP", # Deskripsi 
+  "jenisDokumen": "A03", # Jenis dokumen
+  "namaFile": "Foto KTP", # Nama file
+  "extensionFile": "png", # Extension File
+  "dataBase64": "" # Base64 encoded image file
+})
+```
+
+
 
 ## Get help
 
 * [Digital Services](https://digitalservices.bni.co.id/en/)
 * [API documentation](https://digitalservices.bni.co.id/documentation/public/en)
 * [Stackoverflow](https://stackoverflow.com/users/19817167/bni-api-management)
 * Can't find answer you looking for? email to [apisupport@bni.co.id](mailto:apisupport@bni.co.id)
```

### Comparing `bnipython-0.8.3/bnipython.egg-info/SOURCES.txt` & `bnipython-0.8.4/bnipython.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 bnipython/__init__.py
 bnipython.egg-info/PKG-INFO
 bnipython.egg-info/SOURCES.txt
 bnipython.egg-info/dependency_links.txt
 bnipython.egg-info/requires.txt
 bnipython.egg-info/top_level.txt
 bnipython/lib/bniClient.py
+bnipython/lib/api/bniMove.py
 bnipython/lib/api/oneGatePayment.py
 bnipython/lib/api/rdf.py
 bnipython/lib/api/rdl.py
 bnipython/lib/api/rdn.py
 bnipython/lib/api/snapBI.py
 bnipython/lib/net/httpClient.py
 bnipython/lib/util/constants.py
 bnipython/lib/util/response.py
 bnipython/lib/util/utils.py
 tests/test_bni_client.py
+tests/test_bni_move.py
 tests/test_one_gate_payment.py
 tests/test_rdf.py
 tests/test_rdl.py
 tests/test_rdn.py
 tests/test_snap_bi.py
 tests/test_util.py
```

### Comparing `bnipython-0.8.3/setup.py` & `bnipython-0.8.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 test_req = pkg_req + [
     'pytest>=3.0.6'
 ]
 
 setup(
     name="bnipython",
-    version="0.8.3",
+    version="0.8.4",
     author="BNI API",
     author_email="",
     license='MIT',
     description="Official  BNI API SDK for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bni-api/bni-python/",
```

### Comparing `bnipython-0.8.3/tests/test_bni_client.py` & `bnipython-0.8.4/tests/test_bni_client.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.8.3/tests/test_one_gate_payment.py` & `bnipython-0.8.4/tests/test_one_gate_payment.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.8.3/tests/test_rdf.py` & `bnipython-0.8.4/tests/test_rdf.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.8.3/tests/test_rdl.py` & `bnipython-0.8.4/tests/test_rdl.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.8.3/tests/test_rdn.py` & `bnipython-0.8.4/tests/test_rdn.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.8.3/tests/test_snap_bi.py` & `bnipython-0.8.4/tests/test_snap_bi.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.8.3/tests/test_util.py` & `bnipython-0.8.4/tests/test_util.py`

 * *Files identical despite different names*

