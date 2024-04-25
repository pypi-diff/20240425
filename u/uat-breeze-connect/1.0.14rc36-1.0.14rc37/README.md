# Comparing `tmp/uat-breeze-connect-1.0.14rc36.tar.gz` & `tmp/uat_breeze_connect-1.0.14rc37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uat-breeze-connect-1.0.14rc36.tar", last modified: Fri Feb 23 09:24:12 2024, max compression
+gzip compressed data, was "uat_breeze_connect-1.0.14rc37.tar", last modified: Thu Apr 25 08:26:08 2024, max compression
```

## Comparing `uat-breeze-connect-1.0.14rc36.tar` & `uat_breeze_connect-1.0.14rc37.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-02-23 09:24:12.342670 uat-breeze-connect-1.0.14rc36/
--rw-rw-rw-   0        0        0     1100 2022-08-09 05:48:54.000000 uat-breeze-connect-1.0.14rc36/LICENSE
--rw-rw-rw-   0        0        0    19998 2024-02-23 09:24:12.342670 uat-breeze-connect-1.0.14rc36/PKG-INFO
--rw-rw-rw-   0        0        0    19463 2024-02-23 09:23:56.000000 uat-breeze-connect-1.0.14rc36/README.md
-drwxrwxrwx   0        0        0        0 2024-02-23 09:24:12.229977 uat-breeze-connect-1.0.14rc36/breeze_connect/
--rw-rw-rw-   0        0        0       55 2022-08-09 05:48:54.000000 uat-breeze-connect-1.0.14rc36/breeze_connect/__init__.py
--rw-rw-rw-   0        0        0    97980 2024-02-23 09:05:44.000000 uat-breeze-connect-1.0.14rc36/breeze_connect/breeze_connect.py
--rw-rw-rw-   0        0        0       42 2024-02-23 09:24:12.354685 uat-breeze-connect-1.0.14rc36/setup.cfg
--rw-rw-rw-   0        0        0      758 2024-02-23 09:21:17.000000 uat-breeze-connect-1.0.14rc36/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-23 09:24:12.266374 uat-breeze-connect-1.0.14rc36/uat_breeze_connect.egg-info/
--rw-rw-rw-   0        0        0    19998 2024-02-23 09:24:12.000000 uat-breeze-connect-1.0.14rc36/uat_breeze_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-02-23 09:24:12.000000 uat-breeze-connect-1.0.14rc36/uat_breeze_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-23 09:24:12.000000 uat-breeze-connect-1.0.14rc36/uat_breeze_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-02-23 09:24:12.000000 uat-breeze-connect-1.0.14rc36/uat_breeze_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-02-23 09:24:12.000000 uat-breeze-connect-1.0.14rc36/uat_breeze_connect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 08:26:08.846939 uat_breeze_connect-1.0.14rc37/
+-rw-rw-rw-   0        0        0     1100 2024-04-25 08:21:17.000000 uat_breeze_connect-1.0.14rc37/LICENSE
+-rw-rw-rw-   0        0        0    19998 2024-04-25 08:26:08.846939 uat_breeze_connect-1.0.14rc37/PKG-INFO
+-rw-rw-rw-   0        0        0    19463 2024-04-25 08:25:27.000000 uat_breeze_connect-1.0.14rc37/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 08:26:08.815024 uat_breeze_connect-1.0.14rc37/breeze_connect/
+-rw-rw-rw-   0        0        0       55 2024-04-25 08:21:17.000000 uat_breeze_connect-1.0.14rc37/breeze_connect/__init__.py
+-rw-rw-rw-   0        0        0    98442 2024-04-25 08:24:34.000000 uat_breeze_connect-1.0.14rc37/breeze_connect/breeze_connect.py
+-rw-rw-rw-   0        0        0       42 2024-04-25 08:26:08.848932 uat_breeze_connect-1.0.14rc37/setup.cfg
+-rw-rw-rw-   0        0        0      758 2024-04-25 08:25:27.000000 uat_breeze_connect-1.0.14rc37/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:26:08.844943 uat_breeze_connect-1.0.14rc37/uat_breeze_connect.egg-info/
+-rw-rw-rw-   0        0        0    19998 2024-04-25 08:26:08.000000 uat_breeze_connect-1.0.14rc37/uat_breeze_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-04-25 08:26:08.000000 uat_breeze_connect-1.0.14rc37/uat_breeze_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 08:26:08.000000 uat_breeze_connect-1.0.14rc37/uat_breeze_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-25 08:26:08.000000 uat_breeze_connect-1.0.14rc37/uat_breeze_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-25 08:26:08.000000 uat_breeze_connect-1.0.14rc37/uat_breeze_connect.egg-info/top_level.txt
```

### Comparing `uat-breeze-connect-1.0.14rc36/LICENSE` & `uat_breeze_connect-1.0.14rc37/LICENSE`

 * *Files identical despite different names*

### Comparing `uat-breeze-connect-1.0.14rc36/PKG-INFO` & `uat_breeze_connect-1.0.14rc37/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uat-breeze-connect
-Version: 1.0.14rc36
+Version: 1.0.14rc37
 Summary: UAT Breeze Connect
 Home-page: https://github.com/pypa/sampleproject
 Author: UAT Breeze Connect
 Author-email: test@mail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,15 @@
 ```
 pip install --upgrade uat-breeze-connect
 ```
 
 Or, You can also install the specific release version via pip
 
 ```
-pip install uat-breeze-connect==1.0.14rc36
+pip install uat-breeze-connect==1.0.14rc37
 ```
 
 ## Websocket Usage
 <h4 id="#Web_socket">Websocket Usage</h4>
 
 ```python
 from breeze_connect import BreezeConnect
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: uat-breeze-connect Version: 1.0.14rc36 Summary: UAT
+Metadata-Version: 2.1 Name: uat-breeze-connect Version: 1.0.14rc37 Summary: UAT
 Breeze Connect Home-page: https://github.com/pypa/sampleproject Author: UAT
 Breeze Connect Author-email: test@mail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: python-socketio
 [client] Requires-Dist: requests Requires-Dist: pandas # Index
     * _U_A_T___B_r_e_e_z_e___C_o_n_n_e_c_t___S_D_K
@@ -40,15 +40,15 @@
 You must install the virtualenv package via pip ``` pip install virtualenv ```
 You should create breeze virtual environment via virtualenv ``` virtualenv -
 p python3 breeze_venv ``` And then, You can activate virtual environment via
 source ``` source breeze_venv/bin/activate ``` ## Installing the client
 ****** IInnssttaalllliinngg tthhee cclliieenntt ******
 You can install the latest release via pip ``` pip install --upgrade uat-
 breeze-connect ``` Or, You can also install the specific release version via
-pip ``` pip install uat-breeze-connect==1.0.14rc36 ``` ## Websocket Usage
+pip ``` pip install uat-breeze-connect==1.0.14rc37 ``` ## Websocket Usage
 ****** WWeebbssoocckkeett UUssaaggee ******
 ```python from breeze_connect import BreezeConnect # Initialize SDK breeze =
 BreezeConnect(api_key="your_api_key") # Obtain your session key from https://
 uatapi.icicidirect.com/apiuser/login?api_key=YOUR_API_KEY # Incase your api-key
 has special characters(like +,=,!) then encode the api key before using in the
 url as shown below. import urllib print("https://uatapi.icicidirect.com/
 apiuser/login?api_key="+urllib.parse.quote_plus("your_api_key")) # Generate
```

### Comparing `uat-breeze-connect-1.0.14rc36/README.md` & `uat_breeze_connect-1.0.14rc37/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 ```
 pip install --upgrade uat-breeze-connect
 ```
 
 Or, You can also install the specific release version via pip
 
 ```
-pip install uat-breeze-connect==1.0.14rc36
+pip install uat-breeze-connect==1.0.14rc37
 ```
 
 ## Websocket Usage
 <h4 id="#Web_socket">Websocket Usage</h4>
 
 ```python
 from breeze_connect import BreezeConnect
```

#### html2text {}

```diff
@@ -34,15 +34,15 @@
 You must install the virtualenv package via pip ``` pip install virtualenv ```
 You should create breeze virtual environment via virtualenv ``` virtualenv -
 p python3 breeze_venv ``` And then, You can activate virtual environment via
 source ``` source breeze_venv/bin/activate ``` ## Installing the client
 ****** IInnssttaalllliinngg tthhee cclliieenntt ******
 You can install the latest release via pip ``` pip install --upgrade uat-
 breeze-connect ``` Or, You can also install the specific release version via
-pip ``` pip install uat-breeze-connect==1.0.14rc36 ``` ## Websocket Usage
+pip ``` pip install uat-breeze-connect==1.0.14rc37 ``` ## Websocket Usage
 ****** WWeebbssoocckkeett UUssaaggee ******
 ```python from breeze_connect import BreezeConnect # Initialize SDK breeze =
 BreezeConnect(api_key="your_api_key") # Obtain your session key from https://
 uatapi.icicidirect.com/apiuser/login?api_key=YOUR_API_KEY # Incase your api-key
 has special characters(like +,=,!) then encode the api key before using in the
 url as shown below. import urllib print("https://uatapi.icicidirect.com/
 apiuser/login?api_key="+urllib.parse.quote_plus("your_api_key")) # Generate
```

### Comparing `uat-breeze-connect-1.0.14rc36/breeze_connect/breeze_connect.py` & `uat_breeze_connect-1.0.14rc37/breeze_connect/breeze_connect.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,19 +257,20 @@
             exchange_code_name = ""
             exchange_code_list = {
                 "BSE": "1.",
                 "NSE": "4.",
                 "NDX": "13.",
                 "MCX": "6.",
                 "NFO": "4.",
+                "BFO": "2.",
             }
             exchange_code_name = exchange_code_list.get(exchange_code, False)
             if exchange_code_name == False:
                 raise Exception(
-                    "Exchange Code allowed are 'BSE', 'NSE', 'NDX', 'MCX' or 'NFO'."
+                    "Exchange Code allowed are 'BSE', 'NSE', 'NDX', 'MCX', 'NFO', 'BFO'."
                 )
             elif stock_code == "":
                 raise Exception("Stock-Code cannot be empty.")
             else:
                 token_value = False
                 if exchange_code.lower() == "bse":
                     token_value = self.stock_script_dict_list[0].get(stock_code, False)
@@ -316,14 +317,18 @@
                         token_value = self.stock_script_dict_list[3].get(
                             contract_detail_value, False
                         )
                     elif exchange_code.lower() == "nfo":
                         token_value = self.stock_script_dict_list[4].get(
                             contract_detail_value, False
                         )
+                    elif exchange_code.lower() == "bfo":
+                        token_value = self.stock_script_dict_list[5].get(
+                            contract_detail_value, False
+                        )
                 if token_value == False:
                     raise Exception("Stock-Code not found.")
                 exchange_quotes_token_value = False
                 if get_exchange_quotes != False:
                     exchange_quotes_token_value = (
                         exchange_code_name + "1!" + token_value
                     )
@@ -819,16 +824,16 @@
         end = time.time()
         print(f"execution time : {end - start}")
         return data
 
     def get_stock_script_list(self):
         try:
             self.load_cache()
-            self.stock_script_dict_list = [{}, {}, {}, {}, {}]
-            self.token_script_dict_list = [{}, {}, {}, {}, {}]
+            self.stock_script_dict_list = [{}, {}, {}, {}, {}, {}]
+            self.token_script_dict_list = [{}, {}, {}, {}, {}, {}]
             link = "https://traderweb.icicidirect.com/Content/File/txtFile/ScripFile/StockScriptNew.csv"
             response = self.get_response(link)
             if response is not None:
 
                 # download = s.get("https://traderweb.icicidirect.com/Content/File/txtFile/ScripFile/StockScriptNew.csv")
                 cr = csv.reader(response.text.splitlines(), delimiter=",")
                 my_list = list(cr)
@@ -844,14 +849,18 @@
                         self.token_script_dict_list[2][row[5]] = [row[7], row[1]]
                     elif row[2] == "MCX":
                         self.stock_script_dict_list[3][row[7]] = row[5]
                         self.token_script_dict_list[3][row[5]] = [row[7], row[1]]
                     elif row[2] == "NFO":
                         self.stock_script_dict_list[4][row[7]] = row[5]
                         self.token_script_dict_list[4][row[5]] = [row[7], row[1]]
+                    elif row[2] == "BFO":
+                        self.stock_script_dict_list[5][row[7]] = row[5]
+                        self.token_script_dict_list[5][row[5]] = [row[7], row[1]]
+
         except Exception as e:
             print("error", e)
             # pass
 
     def generate_session(self, api_secret, session_token):
         self.session_key = session_token
         self.secret_key = api_secret
```

### Comparing `uat-breeze-connect-1.0.14rc36/setup.py` & `uat_breeze_connect-1.0.14rc37/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="uat-breeze-connect",
-    version="1.0.14rc36",
+    version="1.0.14rc37",
     author="UAT Breeze Connect",
     author_email="test@mail.com",
     description="UAT Breeze Connect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['python-socketio[client]','requests','pandas'],
     url="https://github.com/pypa/sampleproject",
```

### Comparing `uat-breeze-connect-1.0.14rc36/uat_breeze_connect.egg-info/PKG-INFO` & `uat_breeze_connect-1.0.14rc37/uat_breeze_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uat-breeze-connect
-Version: 1.0.14rc36
+Version: 1.0.14rc37
 Summary: UAT Breeze Connect
 Home-page: https://github.com/pypa/sampleproject
 Author: UAT Breeze Connect
 Author-email: test@mail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,15 @@
 ```
 pip install --upgrade uat-breeze-connect
 ```
 
 Or, You can also install the specific release version via pip
 
 ```
-pip install uat-breeze-connect==1.0.14rc36
+pip install uat-breeze-connect==1.0.14rc37
 ```
 
 ## Websocket Usage
 <h4 id="#Web_socket">Websocket Usage</h4>
 
 ```python
 from breeze_connect import BreezeConnect
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: uat-breeze-connect Version: 1.0.14rc36 Summary: UAT
+Metadata-Version: 2.1 Name: uat-breeze-connect Version: 1.0.14rc37 Summary: UAT
 Breeze Connect Home-page: https://github.com/pypa/sampleproject Author: UAT
 Breeze Connect Author-email: test@mail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: python-socketio
 [client] Requires-Dist: requests Requires-Dist: pandas # Index
     * _U_A_T___B_r_e_e_z_e___C_o_n_n_e_c_t___S_D_K
@@ -40,15 +40,15 @@
 You must install the virtualenv package via pip ``` pip install virtualenv ```
 You should create breeze virtual environment via virtualenv ``` virtualenv -
 p python3 breeze_venv ``` And then, You can activate virtual environment via
 source ``` source breeze_venv/bin/activate ``` ## Installing the client
 ****** IInnssttaalllliinngg tthhee cclliieenntt ******
 You can install the latest release via pip ``` pip install --upgrade uat-
 breeze-connect ``` Or, You can also install the specific release version via
-pip ``` pip install uat-breeze-connect==1.0.14rc36 ``` ## Websocket Usage
+pip ``` pip install uat-breeze-connect==1.0.14rc37 ``` ## Websocket Usage
 ****** WWeebbssoocckkeett UUssaaggee ******
 ```python from breeze_connect import BreezeConnect # Initialize SDK breeze =
 BreezeConnect(api_key="your_api_key") # Obtain your session key from https://
 uatapi.icicidirect.com/apiuser/login?api_key=YOUR_API_KEY # Incase your api-key
 has special characters(like +,=,!) then encode the api key before using in the
 url as shown below. import urllib print("https://uatapi.icicidirect.com/
 apiuser/login?api_key="+urllib.parse.quote_plus("your_api_key")) # Generate
```

