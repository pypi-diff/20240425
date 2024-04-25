# Comparing `tmp/AutoZeekWatch-0.1.1.tar.gz` & `tmp/autozeekwatch-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoZeekWatch-0.1.1.tar", last modified: Thu Apr 11 20:27:14 2024, max compression
+gzip compressed data, was "autozeekwatch-0.1.3.tar", last modified: Thu Apr 25 20:14:15 2024, max compression
```

## Comparing `AutoZeekWatch-0.1.1.tar` & `autozeekwatch-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,17 @@
-drwxr-xr-x   0 zihangxia   (501) staff       (20)        0 2024-04-11 20:27:14.095740 AutoZeekWatch-0.1.1/
-drwxr-xr-x   0 zihangxia   (501) staff       (20)        0 2024-04-11 20:27:14.089242 AutoZeekWatch-0.1.1/AutoZeekWatch.egg-info/
--rw-r--r--   0 zihangxia   (501) staff       (20)     1630 2024-04-11 20:27:14.000000 AutoZeekWatch-0.1.1/AutoZeekWatch.egg-info/PKG-INFO
--rw-r--r--   0 zihangxia   (501) staff       (20)      363 2024-04-11 20:27:14.000000 AutoZeekWatch-0.1.1/AutoZeekWatch.egg-info/SOURCES.txt
--rw-r--r--   0 zihangxia   (501) staff       (20)        1 2024-04-11 20:27:14.000000 AutoZeekWatch-0.1.1/AutoZeekWatch.egg-info/dependency_links.txt
--rw-r--r--   0 zihangxia   (501) staff       (20)      162 2024-04-11 20:27:14.000000 AutoZeekWatch-0.1.1/AutoZeekWatch.egg-info/requires.txt
--rw-r--r--   0 zihangxia   (501) staff       (20)       13 2024-04-11 20:27:14.000000 AutoZeekWatch-0.1.1/AutoZeekWatch.egg-info/top_level.txt
--rw-r--r--   0 zihangxia   (501) staff       (20)     1065 2024-02-13 14:15:04.000000 AutoZeekWatch-0.1.1/LICENSE
-drwxr-xr-x   0 zihangxia   (501) staff       (20)        0 2024-04-11 20:27:14.091440 AutoZeekWatch-0.1.1/NIDS/
--rw-r--r--   0 zihangxia   (501) staff       (20)       62 2024-02-13 14:15:04.000000 AutoZeekWatch-0.1.1/NIDS/__init__.py
--rw-r--r--   0 zihangxia   (501) staff       (20)     5678 2024-04-11 19:46:37.000000 AutoZeekWatch-0.1.1/NIDS/infer.py
--rw-r--r--   0 zihangxia   (501) staff       (20)     8778 2024-04-11 19:46:37.000000 AutoZeekWatch-0.1.1/NIDS/train.py
--rw-r--r--   0 zihangxia   (501) staff       (20)    14214 2024-04-11 19:46:37.000000 AutoZeekWatch-0.1.1/NIDS/utils.py
--rw-r--r--   0 zihangxia   (501) staff       (20)     1630 2024-04-11 20:27:14.094783 AutoZeekWatch-0.1.1/PKG-INFO
--rw-r--r--   0 zihangxia   (501) staff       (20)      862 2024-02-13 14:15:04.000000 AutoZeekWatch-0.1.1/README.md
-drwxr-xr-x   0 zihangxia   (501) staff       (20)        0 2024-04-11 20:27:14.093659 AutoZeekWatch-0.1.1/package/
--rw-r--r--   0 zihangxia   (501) staff       (20)        0 2024-02-13 14:15:04.000000 AutoZeekWatch-0.1.1/package/__init__.py
--rw-r--r--   0 zihangxia   (501) staff       (20)    10086 2024-02-13 14:15:04.000000 AutoZeekWatch-0.1.1/package/data_preprocess.py
--rw-r--r--   0 zihangxia   (501) staff       (20)     4933 2024-02-13 14:15:04.000000 AutoZeekWatch-0.1.1/package/pred_kitnet.py
--rw-r--r--   0 zihangxia   (501) staff       (20)     4445 2024-02-13 14:15:04.000000 AutoZeekWatch-0.1.1/package/train_kitnet.py
--rw-r--r--   0 zihangxia   (501) staff       (20)       38 2024-04-11 20:27:14.095884 AutoZeekWatch-0.1.1/setup.cfg
--rw-r--r--   0 zihangxia   (501) staff       (20)      905 2024-04-11 20:23:49.000000 AutoZeekWatch-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:14:15.994243 autozeekwatch-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:14:15.990243 autozeekwatch-0.1.3/AutoZeekWatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-25 20:14:15.000000 autozeekwatch-0.1.3/AutoZeekWatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-25 20:14:15.000000 autozeekwatch-0.1.3/AutoZeekWatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 20:14:15.000000 autozeekwatch-0.1.3/AutoZeekWatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-25 20:14:15.000000 autozeekwatch-0.1.3/AutoZeekWatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 20:14:15.000000 autozeekwatch-0.1.3/AutoZeekWatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-25 20:14:11.000000 autozeekwatch-0.1.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:14:15.990243 autozeekwatch-0.1.3/NIDS/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 20:14:11.000000 autozeekwatch-0.1.3/NIDS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-25 20:14:11.000000 autozeekwatch-0.1.3/NIDS/infer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-04-25 20:14:11.000000 autozeekwatch-0.1.3/NIDS/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21665 2024-04-25 20:14:11.000000 autozeekwatch-0.1.3/NIDS/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-25 20:14:15.990243 autozeekwatch-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-25 20:14:11.000000 autozeekwatch-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 20:14:15.994243 autozeekwatch-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-25 20:14:13.000000 autozeekwatch-0.1.3/setup.py
```

### Comparing `AutoZeekWatch-0.1.1/LICENSE` & `autozeekwatch-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoZeekWatch-0.1.1/NIDS/infer.py` & `autozeekwatch-0.1.3/NIDS/infer.py`

 * *Files 19% similar despite different names*

```diff
@@ -40,33 +40,35 @@
 fh.setLevel(logging.INFO)
 fh.setFormatter(file_formatter)
 anomaly_logger.addHandler(fh)
 
 CONN_AD_ENABLED=False
 HTTP_AD_ENABLED=False
 DNS_AD_ENABLED=False
+SSH_AD_ENABLED=False
+SSL_AD_ENABLED=False
 
 def main():
     """
     The main control flow for the application. This script takes in as arguments the 
     location of the zeek spool directory (also found in the zeek/logs/current symlink)
     and applies the model to the conn.log stream. This expects that this stream is in JSON format, 
     which can be applied to Zeek by adding "@load policy/tuning/json-logs.zeek" to local.zeek.
     """
-    global CONN_AD_ENABLED, DNS_AD_ENABLED, HTTP_AD_ENABLED 
+    global CONN_AD_ENABLED, DNS_AD_ENABLED, HTTP_AD_ENABLED, SSL_AD_ENABLED, SSH_AD_ENABLED
     parser = argparse.ArgumentParser(
         description='Apply a KitNET model to current data and output anomaly scores. The logs MUST have been stored '
                     'in JSON format.')
     parser.add_argument('--model-path', type=str, default='kit.joblib',  
                         help='The path to the model file to load.') 
     parser.add_argument('--log-dir', type=str, required=True, 
                         help='Zeek logdir variable, where this script can find Zeek data. Please point to the logs/ '
                              'directory.')
-    parser.add_argument('--modules', nargs='+', required=True, choices=['CONN', 'DNS', 'HTTP'],
-                        help='List of modules to enable. Choose from CONN, DNS, or HTTP. At least one module is required.')
+    parser.add_argument('--modules', nargs='+', required=True, choices=['CONN', 'DNS', 'HTTP', 'SSH', 'SSL'],
+                        help='List of modules to enable. Choose from CONN, DNS, HTTP, SSL or SSH. At least one module is required.')
     args = parser.parse_args()
     log_dir = args.log_dir
     # At least 1 module must be specified
     logging.info(f"Using Modules {args.modules}")
     logging.info(f"Using logdir: {log_dir}")
     spool_path = os.path.join(log_dir, "current") 
     logging.info(f"Using spool path: {spool_path}")
@@ -103,14 +105,38 @@
             kit_http_model = load(http_model_path)
         except FileNotFoundError:
             logging.error(f"Could not find model path {http_model_path}")
             sys.exit(1)
         http_process = Process(target=follow, args=(http_log_path, kit_http_model, "http"))
         http_process.start()
         logging.info("Started HTTP Monitoring Process")
+    if 'SSL' in args.modules:
+        SSL_AD_ENABLED = True
+        ssl_log_path = os.path.join(spool_path, "ssl.log")
+        ssl_model_path = "ssl_" + args.model_path
+        try:
+            kit_ssl_model = load(ssl_model_path)
+        except FileNotFoundError:
+            logging.error(f"Could not find model path {ssl_model_path}")
+            sys.exit(1)
+        ssl_process = Process(target=follow, args=(ssl_log_path, kit_ssl_model, "ssl"))
+        ssl_process.start()
+        logging.info("Started SSL Monitoring Process")
+    if 'SSH' in args.modules:
+        SSH_AD_ENABLED = True
+        ssh_log_path = os.path.join(spool_path, "ssh.log")
+        ssh_model_path = "ssh_" + args.model_path
+        try:
+            kit_ssh_model = load(ssh_model_path)
+        except FileNotFoundError:
+            logging.error(f"Could not find model path {ssh_model_path}")
+            sys.exit(1)
+        ssh_process = Process(target=follow, args=(ssh_log_path, kit_ssh_model, "ssh"))
+        ssh_process.start()
+        logging.info("Started SSH Monitoring Process")
     logging.info("Awaiting events...")
 
 def follow(log_path, kit_model, type):
     for line in tailer.follow(open(log_path)):
         result = score_json(kit_model, line, type)
         anomaly_logger.info(result)
 
@@ -121,21 +147,25 @@
     """
     if type == "conn":
         line_processed = preprocess_json_conn(line)
     elif type == "dns":
         line_processed = preprocess_json_dns(line)
     elif type == "http":
         line_processed = preprocess_json_http(line)
+    elif type == "ssh":
+        line_processed = preprocess_json_ssh(line)
+    elif type == "ssl":
+        line_processed = preprocess_json_ssl(line)
     else:
         logging.error(f"Invalid scoring type {type}")
         sys.exit(1)
     assert len(line_processed) == 1
-    features = ['uid', "id.resp_h", "id.orig_h", "id.orig_p", "id.resp_p", "proto"]
+    features = ['uid', "id.resp_h", "id.orig_h", "id.orig_p", "id.resp_p"]
     features_obj = json.loads(line)
     features_dict = dict(zip(features, [features_obj[feature] for feature in features]))
-    assert len(features_dict) == 6
+    assert len(features_dict) == 5
     anomaly_score = kit.score_partial(line_processed[0])
     features_dict['anomaly_score'] = anomaly_score
     return features_dict
 
 if __name__ == "__main__":
     main()
```

### Comparing `AutoZeekWatch-0.1.1/NIDS/train.py` & `autozeekwatch-0.1.3/NIDS/train.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(name)s - %(levelname)s - %(message)s (%(filename)s)')
 #MODEL_PATH = 'kit.joblib'
 #LOAD_MODEL = False       
 # The different files the AD can operate on
 CONN_AD_ENABLED=False
 HTTP_AD_ENABLED=False
 DNS_AD_ENABLED=False
+SSH_AD_ENABLED=False
+SSL_AD_ENABLED=False
 
 def ungzip(file_path):
     """
     Take a file path and ungzip it
     """
     # TODO: there should probably be some error checks here
     ungzipped_file_path = file_path.removesuffix('.gz')
@@ -61,15 +63,15 @@
 
 def main():
     """
     The main control flow for the application. 
     Taking the user-provided log directory as input, recursively searches the directory 
     for all date-based subdirectories, and trains models on all `conn.log` files. 
     """
-    global CONN_AD_ENABLED, DNS_AD_ENABLED, HTTP_AD_ENABLED 
+    global CONN_AD_ENABLED, DNS_AD_ENABLED, HTTP_AD_ENABLED, SSH_AD_ENABLED, SSL_AD_ENABLED
     parser = argparse.ArgumentParser(
         description='Trains a KitNET model on the specified log directory. The logs MUST have been stored in JSON format.')
     # Eventually we will need to implement some sort of directory to house these as people will retrain
     # and will still need access to historical models
     parser.add_argument('--model-path', type=str, default='kit.joblib',  
                         help='The path to the model file to dump.') 
     parser.add_argument('--log-dir', type=str, required=True, 
@@ -80,25 +82,30 @@
                         help='The grace period for feature mapping.')     
     parser.add_argument('--grace-anomaly-detector', type=int, default=50000,    
                         help='The grace period for the anomaly detector.')  
     parser.add_argument('--learning-rate', type=float, default=0.001,    
                         help='The learning rate for the model.')
     parser.add_argument('--hidden-ratio', type=float, default=0.5,  
                         help='The hidden ratio for the model.')  
-    parser.add_argument('--modules', nargs='+', required=True, choices=['CONN', 'DNS', 'HTTP'],
-                        help='List of modules to enable. Choose from CONN, DNS, or HTTP. At least one module is required.')
+    parser.add_argument('--modules', nargs='+', required=True, choices=['CONN', 'DNS', 'HTTP', 'SSH', 'SSL'],
+                        help='List of modules to enable. Choose from CONN, DNS, HTTP, SSH, or SSL. At least one module is required.')
     args = parser.parse_args()
     log_dir = args.log_dir
     # At least 1 module must be specified
     if 'CONN' in args.modules:
         CONN_AD_ENABLED = True
     if 'DNS' in args.modules:
         DNS_AD_ENABLED = True
     if 'HTTP' in args.modules:
         HTTP_AD_ENABLED = True
+    if 'SSH' in args.modules:
+        SSH_AD_ENABLED = True
+    if 'SSL' in args.modules:
+        SSL_AD_ENABLED = True
+    
     # create kitnet model
     if CONN_AD_ENABLED:
         kit_conn_model = KitNet(
             max_size_ae=args.max_size_ae, 
             grace_feature_mapping=args.grace_feature_mapping, 
             grace_anomaly_detector=args.grace_anomaly_detector, 
             learning_rate=args.learning_rate, 
@@ -116,14 +123,30 @@
         kit_http_model = KitNet(
             max_size_ae=args.max_size_ae, 
             grace_feature_mapping=args.grace_feature_mapping, 
             grace_anomaly_detector=args.grace_anomaly_detector, 
             learning_rate=args.learning_rate, 
             hidden_ratio=args.hidden_ratio 
         )
+    if SSH_AD_ENABLED:
+        kit_ssh_model = KitNet(
+            max_size_ae=args.max_size_ae, 
+            grace_feature_mapping=args.grace_feature_mapping, 
+            grace_anomaly_detector=args.grace_anomaly_detector, 
+            learning_rate=args.learning_rate, 
+            hidden_ratio=args.hidden_ratio 
+        )
+    if SSL_AD_ENABLED:
+        kit_ssl_model = KitNet(
+            max_size_ae=args.max_size_ae, 
+            grace_feature_mapping=args.grace_feature_mapping, 
+            grace_anomaly_detector=args.grace_anomaly_detector, 
+            learning_rate=args.learning_rate, 
+            hidden_ratio=args.hidden_ratio 
+        )
     logging.info(f"Using Modules {args.modules}")
     logging.info(f"Using logdir: {log_dir}") 
     logging.info(
         f"Using Parameters - max_size_ae: {args.max_size_ae}, "
         f"grace_feature_mapping: {args.grace_feature_mapping}, "
         f"grace_anomaly_detector: {args.grace_anomaly_detector}, "
         f"learning_rate: {args.learning_rate}, "
@@ -137,15 +160,15 @@
         # `current` is a symlink for the current-day logs, we should not train on them as these files are in use. 
         if not os.path.islink(current_dir_path):
             # sub_dir is now any given historical data directory 
             logging.info(f"Checking {current_dir_path}")
             for file in os.listdir(current_dir_path):
                 # file is now any given file in the historical data directory
                 current_file_path = os.path.join(current_dir_path, file)
-                if "conn." in file or "dns." in file or "http." in file:
+                if "conn." in file or "dns." in file or "http." in file or "ssl." in file or "ssh." in file:
                     # get the whole file in memory
                     if "conn." in file and CONN_AD_ENABLED:
                         logging.info(f"Opening file {current_file_path}")
                         json_data_file = ungzip(current_file_path) 
                         try:    
                             json.loads(json_data_file.split('\n')[0])
                         except json.JSONDecodeError as e:
@@ -169,21 +192,47 @@
                         try:    
                             json.loads(json_data_file.split('\n')[0])
                         except json.JSONDecodeError as e:
                             logging.error(f"File {current_file_path} is not JSON. Skipping.")
                             continue 
                         np_arr = preprocess_json_http(json_data_file)
                         train_batch(kit_http_model, np_arr)  
+                    elif "ssh." in file and SSH_AD_ENABLED:
+                        logging.info(f"Opening file {current_file_path}")
+                        json_data_file = ungzip(current_file_path) 
+                        try:    
+                            json.loads(json_data_file.split('\n')[0])
+                        except json.JSONDecodeError as e:
+                            logging.error(f"File {current_file_path} is not JSON. Skipping.")
+                            continue 
+                        np_arr = preprocess_json_ssh(json_data_file)
+                        train_batch(kit_ssh_model, np_arr)  
+                    elif "ssl." in file and SSL_AD_ENABLED:
+                        logging.info(f"Opening file {current_file_path}")
+                        json_data_file = ungzip(current_file_path) 
+                        try:    
+                            json.loads(json_data_file.split('\n')[0])
+                        except json.JSONDecodeError as e:
+                            logging.error(f"File {current_file_path} is not JSON. Skipping.")
+                            continue 
+                        np_arr = preprocess_json_ssl(json_data_file)
+                        train_batch(kit_ssl_model, np_arr)  
 
     # TODO: Before we exit the main function, dump the trained model to disk
     if CONN_AD_ENABLED:
         dump(kit_conn_model, "conn_" + args.model_path) 
         logging.info(f"Model is saved successfully as conn_{args.model_path}.") 
     if DNS_AD_ENABLED:
-        dump(kit_conn_model, "dns_" + args.model_path) 
+        dump(kit_dns_model, "dns_" + args.model_path) 
         logging.info(f"Model is saved successfully as dns_{args.model_path}.") 
     if HTTP_AD_ENABLED:
-        dump(kit_conn_model, "http_" + args.model_path) 
+        dump(kit_http_model, "http_" + args.model_path) 
         logging.info(f"Model is saved successfully as http_{args.model_path}.") 
+    if SSH_AD_ENABLED:
+        dump(kit_ssh_model, "ssh_" + args.model_path) 
+        logging.info(f"Model is saved successfully as ssh_{args.model_path}.") 
+    if SSL_AD_ENABLED:
+        dump(kit_ssl_model, "ssl_" + args.model_path) 
+        logging.info(f"Model is saved successfully as ssl_{args.model_path}.") 
 
 if __name__ == "__main__":
     main()
```

### Comparing `AutoZeekWatch-0.1.1/NIDS/utils.py` & `autozeekwatch-0.1.3/NIDS/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,63 +26,73 @@
 def ungzip(file_path):
     """
     Take a file path and ungzip it
     """
     # TODO: there should probably be some error checks here
 
     # if the file is not a .gz file, read the content directly and return it 
-    if (not file_path.endswith('.gz')) and (file_path.endswith('.json')):
+    if (not file_path.endswith('.gz')) and (file_path.endswith('.log')):
         with open(file_path, 'rb') as f:
             return f.read().decode('utf-8') 
         
     ungzipped_file_path = file_path.removesuffix('.gz')
     with gzip.open(file_path, 'rb') as gz_file:
         file_content = gz_file.read()
     return file_content.decode('utf-8')
 
+
 def preprocess_json_conn(json_batch):
     """
     This function receives a json batch from the main control flow of the train 
     functions. It should convert the conn.log of the json_batch to a numpy 2D array, apply necessary transformations,
     then return it. 
 
     Note: the input is only one unzipped json file. 
     """
-    #TODO: 'id.orig_h' or 'id.orig_p'? 
-    features = ['id.orig_h', "id.resp_h", "proto", "conn_state", "missed_bytes",
+    # features = ['id.orig_h', "id.resp_h", "proto", "conn_state", "missed_bytes",
+    #             "orig_pkts", "orig_ip_bytes", "resp_pkts", "resp_ip_bytes"]
+    features = ["id.orig_h", "id.resp_h", "proto", "service", "duration", "conn_state", 
+                "local_orig","local_resp","missed_bytes","history", 
                 "orig_pkts", "orig_ip_bytes", "resp_pkts", "resp_ip_bytes"]
-        
+    #TODO: add features: duration, local_orig, local_resp 
     data_list = []
     for line in json_batch.splitlines():
         # log_entry is now a single json log from the file 
         log_entry = json.loads(line.strip())
-        data_list.append([log_entry[feature] for feature in features])
+        # data_list.append([log_entry[feature] for feature in features])
+        # Check if each feature is present in the log_entry
+        feature_values = [log_entry.get(feature, None) for feature in features]
+        data_list.append(feature_values)
     #Re-use the preprocess function from last sem by Zoe. 
     #TODO: optimize the code via removing pandas
     new_df = pd.DataFrame(data_list, columns=features) 
     #Fill NaNs with 0s : duration, orig_bytes resp_bytes, if there are no columns, create one and fill with 0s 
     new_df = fill_na(new_df) 
-    # Drop unnecessary columns 
-    new_df = drop_columns(new_df, ['ts','uid','local_orig', 'local_resp']) 
+    # # Drop unnecessary columns 
+    # new_df = drop_columns(new_df, ['ts','uid','local_orig', 'local_resp']) 
     # create history, broadcast, traffic_direction variables
     new_df = create_history_variable(new_df)
     new_df = create_broadcast_variable(new_df)
     new_df = create_direction_variable(new_df)
     # one hot encode categorical variables
     column_name = ['conn_state', "proto", "traffic_direction" , "service"]
     new_df = one_hot_encode(new_df, column_name)
+    # Convert the boolean values in columns "local_orig" and "local_resp" to 1 and 0s
+    new_df['local_orig'] = new_df['local_orig'].astype(int)
+    new_df['local_resp'] = new_df['local_resp'].astype(int)
     # make sure the columns are the same as the original df
     #TODO: to be confirmed once HSRN EDA is done
     cols = ['conn_state_OTH', 'conn_state_REJ','conn_state_RSTO', 'conn_state_RSTOS0', 'conn_state_RSTR','conn_state_RSTRH', 
         'conn_state_S0', 'conn_state_S1', 'conn_state_S2','conn_state_S3', 'conn_state_SF', 'conn_state_SH', 'conn_state_SHR',
-        'proto_tcp', 'proto_udp',
+        'proto_tcp', 'proto_udp', 
         'service_dhcp', 'service_dns','service_http', 'service_irc','service_ntp',
         'service_other', 'service_ssh','service_ssl',
         'traffic_direction_external','traffic_direction_incoming', 
-        'traffic_direction_internal','traffic_direction_outgoing']
+        'traffic_direction_internal','traffic_direction_outgoing',
+        "local_orig","local_resp","missed_bytes","orig_pkts","orig_ip_bytes","resp_pkts","resp_ip_bytes"]
     new_df = makedf_samecol(cols, new_df)
     # Convert DataFrame to NumPy array
     np_arr = new_df.to_numpy(dtype=np.float32)
     return np_arr
 
 
 def preprocess_json_dns(json_batch):
@@ -182,22 +192,140 @@
     #TODO: to be confirmed once EDA is done
     http_cols = ['trans_depth', 'request_body_len',
        'response_body_len', 'has_host', 'is_destination_broadcast',
        'method_CONNECT', 'method_GET', 
        'status_code_0', 'status_code_200',
        'version_0.9', 'version_1.1',
        'traffic_direction_IPv6',
-       'traffic_direction_internal', 'traffic_direction_outgoing',
-       'traffic_direction_internal','traffic_direction_outgoing']
+       'traffic_direction_external','traffic_direction_incoming', 
+        'traffic_direction_internal','traffic_direction_outgoing']
     
     df = makedf_samecol(http_cols, df)
 
     # Convert DataFrame to NumPy array
     np_arr = df.to_numpy(dtype=np.float32)
-    logging.info("Hello from preprocess_json_http. Please implement me :)")
+    return np_arr
+
+
+def preprocess_json_ssh(json_batch):
+    """
+    This function receives a json batch from the main control flow of the train 
+    functions. It should convert the dns.log of the json_batch to a numpy 2D array, apply necessary transformations,
+    then return it. 
+
+    Note: the input is only one unzipped json file. 
+    """
+    features = ['id.orig_h', 'id.resp_h','trans_depth','method','host','version',
+                'request_body_len','response_body_len','status_code']
+        
+    data_list = []
+    for line in json_batch.splitlines():
+        # log_entry is now a single json log from the file 
+        log_entry = json.loads(line.strip())
+        # Check if each feature is present in the log_entry
+        feature_values = [log_entry.get(feature, None) for feature in features]
+        data_list.append(feature_values)
+
+    df = pd.DataFrame(data_list, columns=features) 
+
+    # create broadcast, traffic_direction variables
+    df = create_broadcast_variable(df)
+    df = create_direction_variable(df)
+
+    #label encode: auth_success, direction
+    #TODO: ask Diego is it's the same as 'traffic direction'
+    df['auth_success'] = df['auth_success'].replace({False: 0, True: 1})
+    df['direction'] = df['direction'].replace({'OUTBOUND': 1, 'INBOUND': 0})
+
+    # one hot encode categorical variables: proto, qtype, qclass, rcode_name
+    column_name = ['version','traffic_direction']
+    df = one_hot_encode(df, column_name)
+
+    #TODO: to be confirmed once EDA is done
+    ssh_cols = ['auth_success', 'auth_attempts', 'direction',
+       'is_destination_broadcast', 'version_2', 
+       'traffic_direction_external','traffic_direction_incoming', 
+        'traffic_direction_internal','traffic_direction_outgoing']
+    
+    df = makedf_samecol(ssh_cols, df)
+
+    # Convert DataFrame to NumPy array
+    np_arr = df.to_numpy(dtype=np.float32)
+    return np_arr
+
+def preprocess_json_ssl(json_batch):
+    """
+    This function receives a json batch from the main control flow of the train 
+    functions. It should convert the dns.log of the json_batch to a numpy 2D array, apply necessary transformations,
+    then return it. 
+
+    Note: the input is only one unzipped json file. 
+    """
+    features = ['id.orig_h', 'id.resp_h','version','resumed','established',
+            'ssl_history','cert_chain_fps','client_cert_chain_fps','sni_matches_cert','validation_status']
+    #Ignore 'cipher','curve','server_name','next_protocol' columns for now, we can include them if they are useful later on.
+
+    data_list = []
+    for line in json_batch.splitlines():
+        # log_entry is now a single json log from the file 
+        log_entry = json.loads(line.strip())
+        # Check if each feature is present in the log_entry
+        feature_values = [log_entry.get(feature, None) for feature in features]
+        data_list.append(feature_values)
+
+    df = pd.DataFrame(data_list, columns=features) 
+
+    has_null = ['version', 'cert_chain_fps', 'client_cert_chain_fps', 'sni_matches_cert', 'validation_status']
+    # Create a variable to track if the feature contains null. Create a column "has_null_featurename"
+    for feature in has_null: 
+        df[f'has_{feature}'] = df[feature].notnull().astype(int)
+    
+
+    # create broadcast, traffic_direction variables
+    df = create_broadcast_variable(df)
+    df = create_direction_variable(df)
+
+    #fillna, considering null as False
+    df['sni_matches_cert'] = df['sni_matches_cert'].fillna(False)
+    df['cert_chain_fps'] = df['cert_chain_fps'].fillna("").apply(list)
+    df['client_cert_chain_fps'] = df['client_cert_chain_fps'].fillna("").apply(list)
+
+    #boolean to int
+    boolean_to_convert = ['resumed','established','sni_matches_cert']
+    df[boolean_to_convert] = df[boolean_to_convert].astype(int)
+    # one hot encode categorical variables: version, traffic_direction
+    column_name = ['version','traffic_direction']
+    df = one_hot_encode(df, column_name)
+
+    #Make the length of the cert_chain_fps and client_cert_chain_fps as a new feature
+    df['cert_chain_fps'] = df['cert_chain_fps'].apply(lambda x: len(x))
+    df['client_cert_chain_fps'] = df['client_cert_chain_fps'].apply(lambda x: len(x))
+
+    #create history variable
+    df = create_sslhistory_variable(df)
+
+    #TODO: to be confirmed once EDA is done
+    # List of new columns created from ssl_history
+    # Define all possible characters in 'ssl_history'
+    all_characters = set('HCSVTXKRNYGFWUABDOPMIJLQhcsvtxkrnygfwuabdopmijlq')
+    history_col = [f'ssl_history_has_{char}' for char in all_characters]
+    ssl_cols = ['resumed', 'established', 
+        'cert_chain_fps', 'client_cert_chain_fps', 'sni_matches_cert',
+        'has_version', 'has_cert_chain_fps',
+        'has_client_cert_chain_fps', 'has_sni_matches_cert',
+        'has_validation_status', 'is_destination_broadcast', 
+        'version_TLSv12','version_TLSv13', 
+        'traffic_direction_external','traffic_direction_incoming', 
+        'traffic_direction_internal','traffic_direction_outgoing']
+    ssl_cols = ssl_cols + history_col
+
+    df = makedf_samecol(ssl_cols, df)
+
+    # Convert DataFrame to NumPy array
+    np_arr = df.to_numpy(dtype=np.float32)
     return np_arr
 
 #==================================================================================
 # def is_private_ip(ip_str):
 #     """
 #     Takes an IP string and returns whether the IP is private or not per RFC 1918.
 
@@ -291,14 +419,34 @@
     new_df['history_has_d'] = new_df['history'].apply(lambda x: 1 if "d" in x else 0)
     new_df['history_has_F'] = new_df['history'].apply(lambda x: 1 if "F" in x else 0)
     new_df['history_has_f'] = new_df['history'].apply(lambda x: 1 if "f" in x else 0)
     new_df['history_has_N'] = new_df['history'].apply(lambda x: 1 if "N" in x else 0)
     new_df = new_df.drop(columns='history')
     return new_df 
 
+def create_sslhistory_variable(new_df):
+    # break out history variable
+    
+    if 'ssl_history' not in new_df.columns: 
+        new_df['ssl_history'] = ''  #TODO:?
+
+    #fill NaNs with 'N'
+    new_df['ssl_history'] = new_df['ssl_history'].fillna('') 
+    
+    # Define all possible letters in 'ssl_history'
+    all_characters = set('HCSVTXKRNYGFWUABDOPMIJLQhcsvtxkrnygfwuabdopmijlq')
+
+    # Create binary columns for each character
+    for char in all_characters:
+        new_df[f'ssl_history_has_{char}'] = new_df['ssl_history'].apply(lambda x: 1 if char in x else 0)
+
+
+    new_df = new_df.drop(columns='ssl_history')
+    return new_df 
+
 def create_broadcast_variable(new_df):
     # create broadcast variable
     # can have more than one broadcast address
     #255 is the broadcast address for ipv4 
     if 'id.resp_h' in new_df.columns:
         new_df['is_destination_broadcast'] = new_df['id.resp_h'].apply(lambda x: 1 if "255" in x[-3:] else 0) 
     return new_df
@@ -347,12 +495,33 @@
     # Ensure that all the specified columns are present even if they are not present in the original df. 
 
     for col in cols:
         if col not in new_df.columns:
             new_df[col] = 0
     return new_df[cols]
 
+def get_raw_conn(json_data_file):
+    features = ["id.orig_h", "id.resp_h", "proto", "service", "duration", "conn_state", "local_orig","local_resp",
+            "missed_bytes","history", "orig_pkts", "orig_ip_bytes", "resp_pkts", "resp_ip_bytes"]
+    data_list = []
+    for line in json_data_file.splitlines():
+        # log_entry is now a single json log from the file
+        log_entry = json.loads(line.strip())
+        
+        # Check if each feature is present in the log_entry
+        feature_values = [log_entry.get(feature, None) for feature in features]
+        data_list.append(feature_values)
+
+    df = pd.DataFrame(data_list, columns=features)
+    df = create_broadcast_variable(df)
+    df = create_direction_variable(df)
+    # Convert the boolean values in columns "local_orig" and "local_resp" to 1 and 0s
+    df['local_orig'] = df['local_orig'].astype(int)
+    df['local_resp'] = df['local_resp'].astype(int)
+    
+    return df 
+
 #------------------Online Normalization------------------#
 #TODO: def online_normalization(new_df):
 # can be skipped for now, since kitnet has its own normalization.
```

