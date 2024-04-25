# Comparing `tmp/wkregister-0.0.6.tar.gz` & `tmp/wkregister-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wkregister-0.0.6.tar", last modified: Thu Apr 18 18:39:30 2024, max compression
+gzip compressed data, was "wkregister-0.0.7.tar", last modified: Thu Apr 25 16:59:25 2024, max compression
```

## Comparing `wkregister-0.0.6.tar` & `wkregister-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 18:39:30.855525 wkregister-0.0.6/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1073 2023-11-28 19:55:03.000000 wkregister-0.0.6/LICENSE
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     3722 2024-04-18 18:39:30.855175 wkregister-0.0.6/PKG-INFO
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     3246 2024-04-17 16:54:30.000000 wkregister-0.0.6/README.md
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      539 2024-04-18 18:39:23.000000 wkregister-0.0.6/pyproject.toml
--rw-r--r--   0 gustavogordillo   (501) staff       (20)       38 2024-04-18 18:39:30.855634 wkregister-0.0.6/setup.cfg
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 18:39:30.853201 wkregister-0.0.6/src/
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 18:39:30.853443 wkregister-0.0.6/src/test/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2024-04-15 18:05:55.000000 wkregister-0.0.6/src/test/__init__.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      668 2024-04-18 17:44:42.000000 wkregister-0.0.6/src/test/test_logs.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      417 2024-04-18 17:44:39.000000 wkregister-0.0.6/src/test.py
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 18:39:30.854074 wkregister-0.0.6/src/wkregister/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2024-04-15 16:15:44.000000 wkregister-0.0.6/src/wkregister/__init__.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1825 2024-04-18 18:39:14.000000 wkregister-0.0.6/src/wkregister/decorator.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      561 2024-04-18 17:43:57.000000 wkregister-0.0.6/src/wkregister/models.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1394 2024-04-18 17:39:56.000000 wkregister-0.0.6/src/wkregister/producer.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      702 2024-04-18 17:45:49.000000 wkregister-0.0.6/src/wkregister/util.py
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 18:39:30.854909 wkregister-0.0.6/src/wkregister.egg-info/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     3722 2024-04-18 18:39:30.000000 wkregister-0.0.6/src/wkregister.egg-info/PKG-INFO
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      406 2024-04-18 18:39:30.000000 wkregister-0.0.6/src/wkregister.egg-info/SOURCES.txt
--rw-r--r--   0 gustavogordillo   (501) staff       (20)        1 2024-04-18 18:39:30.000000 wkregister-0.0.6/src/wkregister.egg-info/dependency_links.txt
--rw-r--r--   0 gustavogordillo   (501) staff       (20)       16 2024-04-18 18:39:30.000000 wkregister-0.0.6/src/wkregister.egg-info/requires.txt
--rw-r--r--   0 gustavogordillo   (501) staff       (20)       16 2024-04-18 18:39:30.000000 wkregister-0.0.6/src/wkregister.egg-info/top_level.txt
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-25 16:59:25.531007 wkregister-0.0.7/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1073 2023-11-28 19:55:03.000000 wkregister-0.0.7/LICENSE
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     5153 2024-04-25 16:59:25.530723 wkregister-0.0.7/PKG-INFO
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     4677 2024-04-25 16:58:53.000000 wkregister-0.0.7/README.md
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      539 2024-04-25 16:59:09.000000 wkregister-0.0.7/pyproject.toml
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)       38 2024-04-25 16:59:25.531061 wkregister-0.0.7/setup.cfg
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-25 16:59:25.527479 wkregister-0.0.7/src/
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-25 16:59:25.527877 wkregister-0.0.7/src/test/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2024-04-15 18:05:55.000000 wkregister-0.0.7/src/test/__init__.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1479 2024-04-25 16:51:51.000000 wkregister-0.0.7/src/test/test_logs.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      417 2024-04-18 17:44:39.000000 wkregister-0.0.7/src/test.py
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-25 16:59:25.529163 wkregister-0.0.7/src/wkregister/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2024-04-15 16:15:44.000000 wkregister-0.0.7/src/wkregister/__init__.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1427 2024-04-25 16:42:46.000000 wkregister-0.0.7/src/wkregister/decorator.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1753 2024-04-25 16:49:44.000000 wkregister-0.0.7/src/wkregister/models.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1802 2024-04-25 16:43:08.000000 wkregister-0.0.7/src/wkregister/producer.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      769 2024-04-25 16:42:02.000000 wkregister-0.0.7/src/wkregister/util.py
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-25 16:59:25.530352 wkregister-0.0.7/src/wkregister.egg-info/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     5153 2024-04-25 16:59:25.000000 wkregister-0.0.7/src/wkregister.egg-info/PKG-INFO
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      406 2024-04-25 16:59:25.000000 wkregister-0.0.7/src/wkregister.egg-info/SOURCES.txt
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)        1 2024-04-25 16:59:25.000000 wkregister-0.0.7/src/wkregister.egg-info/dependency_links.txt
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)       16 2024-04-25 16:59:25.000000 wkregister-0.0.7/src/wkregister.egg-info/requires.txt
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)       16 2024-04-25 16:59:25.000000 wkregister-0.0.7/src/wkregister.egg-info/top_level.txt
```

### Comparing `wkregister-0.0.6/LICENSE` & `wkregister-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wkregister-0.0.6/PKG-INFO` & `wkregister-0.0.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkregister
-Version: 0.0.6
+Version: 0.0.7
 Summary: A wk register library for python
 Author-email: Gustavo <gustavo.gordillo.giron@gmail.com>
 Project-URL: Homepage, https://github.com/gtavo95/wknmi.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -154,7 +154,40 @@
         status="success",
         errorMessage=None,
         service="pay-service",
     )
     # The record is returned for demonstration purposes
     return {"result": "ok", "record": record}
 ```
+
+### Utilize the Built-In Send Method
+
+he send method is designed to forward records to a Kafka topic without requiring additional decorators. Below is an example that demonstrates how to use the send method with the Records model from the wkregister.models module. This example involves sending a record asynchronously:
+
+```python
+from wkregister.models import Records
+import asyncio
+
+async def sendRecord():
+    """
+    This asynchronous function creates and sends a record to a Kafka topic.
+    It constructs an instance of the Records class with predefined attributes and
+    sends the instance using its built-in asynchronous send method.
+    """
+    # Creating an instance of the Records class
+    record = Records(
+        org="testorg",           # Organization identifier
+        key="your-key",          # Unique key for the record
+        userId="1",              # User ID associated with the record
+        actionType="update",     # Type of action performed
+        status="success",        # Status of the action
+        errorMessage=None,       # Error message, if any (None if no errors)
+        service="pay-service",   # Service associated with the record
+        payload={"hola": "mundo"}  # Payload of the record (example data)
+    )
+    # Sending the record asynchronously to a Kafka topic
+    await record.send()
+
+# Running the asynchronous function using asyncio's event loop
+asyncio.run(sendRecord())
+
+```
```

### Comparing `wkregister-0.0.6/README.md` & `wkregister-0.0.7/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -140,7 +140,40 @@
         status="success",
         errorMessage=None,
         service="pay-service",
     )
     # The record is returned for demonstration purposes
     return {"result": "ok", "record": record}
 ```
+
+### Utilize the Built-In Send Method
+
+he send method is designed to forward records to a Kafka topic without requiring additional decorators. Below is an example that demonstrates how to use the send method with the Records model from the wkregister.models module. This example involves sending a record asynchronously:
+
+```python
+from wkregister.models import Records
+import asyncio
+
+async def sendRecord():
+    """
+    This asynchronous function creates and sends a record to a Kafka topic.
+    It constructs an instance of the Records class with predefined attributes and
+    sends the instance using its built-in asynchronous send method.
+    """
+    # Creating an instance of the Records class
+    record = Records(
+        org="testorg",           # Organization identifier
+        key="your-key",          # Unique key for the record
+        userId="1",              # User ID associated with the record
+        actionType="update",     # Type of action performed
+        status="success",        # Status of the action
+        errorMessage=None,       # Error message, if any (None if no errors)
+        service="pay-service",   # Service associated with the record
+        payload={"hola": "mundo"}  # Payload of the record (example data)
+    )
+    # Sending the record asynchronously to a Kafka topic
+    await record.send()
+
+# Running the asynchronous function using asyncio's event loop
+asyncio.run(sendRecord())
+
+```
```

### Comparing `wkregister-0.0.6/pyproject.toml` & `wkregister-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "wkregister"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Gustavo", email="gustavo.gordillo.giron@gmail.com" },
 ]
 description = "A wk register library for python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `wkregister-0.0.6/src/wkregister/decorator.py` & `wkregister-0.0.7/src/wkregister/producer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,59 @@
-from wkregister.producer import KafkaProducerWrapper, KafkaMessageSender
-from wkregister.models import Records
-from wkregister.util import kafkaParams
-from typing import Callable, Any, Dict
-from functools import wraps
-import inspect
-import asyncio
+import os
+from confluent_kafka import Producer, KafkaException
+from dotenv import load_dotenv
+from typing import Dict
 import json
-import time
 
-
-async def record2Kafka(org: str, key: str, value: Dict) -> None:
-    producer_wrapper = KafkaProducerWrapper()
-    # Crear el enviador de mensajes
-    message_sender = KafkaMessageSender(producer_wrapper)
-    # Enviar un mensaje
-    topic = f"{org}_logs"
-    key = f"{key}"
-    value = json.dumps(value)
-    await message_sender.send(topic, key, value)
-
-    return None
+load_dotenv()
 
 
-# Decorator for logging
-def record():
-    def decorator_log(func: Callable):
-        @wraps(func)
-        async def wrapper(*args, **kwargs):
-            input = func(*args, **kwargs)
+producerconf = {
+    "bootstrap.servers": os.getenv("BOOTSTRAP_SERVER"),
+    "security.protocol": os.getenv("SECURITY_PROTOCOL"),
+    "sasl.mechanisms": os.getenv("SASL_MECHANISM"),
+    "sasl.username": os.getenv("SASL_USERNAME"),
+    "sasl.password": os.getenv("SAS_PASSWORD"),
+}
 
-            if inspect.iscoroutine(input):
-                result = await input
-            else:
-                result = input
 
-            org, key, log = kafkaParams(result)
+class KafkaProducerWrapper:
+    def __init__(self):
+        self.producer = Producer(producerconf)
 
-            start_time = time.time()  # Capture the start time
+    def get_producer(self):
+        return self.producer
 
-            # Log after function execution, you can adjust what you log as needed
-            asyncio.create_task(record2Kafka(org, key, log.dict()))
 
-            end_time = time.time()  # Capture the end time
+class KafkaMessageSender:
+    def __init__(self, producer_wrapper):
+        self.producer = producer_wrapper.get_producer()
 
-            elapsed_time = end_time - start_time  # Calculate elapsed time
-            # print(f"The function took {elapsed_time} seconds to complete.")
-
-            output = {}
-            for key, value in result.items():
-                if not key == "record" or not key == "log":
-                    output[key] = value
+    async def send(self, topic, key, value):
+        def delivery_report(err, msg):
+            if err is not None:
+                print(f"Message not sent: {err}")
+            else:
+                # print(f'Message sent: {msg.value()}')
+                print(f"Message sent")
 
-            if "record" in output:
-                del output["record"]
-            if "log" in output:
-                del output["log"]
+        try:
+            # Intenta enviar el mensaje
+            self.producer.produce(topic, key=key, value=value, callback=delivery_report)
+            self.producer.flush()  # Espera a que el mensaje se entregue
+            return True  # Retorna True si se entregó exitosamente
+        except KafkaException as e:
+            print(f"Error sending to Kafka: {e}")
+            return False  # Retorna False si ocurrió algún error
 
-            return output
 
-        return wrapper
+async def record2Kafka(org: str, key: str, value: Dict) -> None:
+    producer_wrapper = KafkaProducerWrapper()
+    # Crear el enviador de mensajes
+    message_sender = KafkaMessageSender(producer_wrapper)
+    # Enviar un mensaje
+    topic = f"{org}_logs"
+    key = f"{key}"
+    value = json.dumps(value)
+    await message_sender.send(topic, key, value)
 
-    return decorator_log
+    return None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wkregister-0.0.6/src/wkregister/util.py` & `wkregister-0.0.7/src/wkregister/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+# from wkregister.producer import KafkaProducerWrapper, KafkaMessageSender
 from wkregister.models import Records
-from typing import Callable, Any
-import json
+from typing import Any
 
+# import json
 
-def kafkaParams(result: Any):
 
+def kafkaParams(result: Any):
     # Retrieve 'record' or 'log', defaulting to None if neither is found
     log: Records = (result).get("record") or (result).get("log")
     # Check if 'log' was not retrieved and inform the user
     if not log:
         print("No record/log was set")
 
     # Extract 'org' and 'key' from the log, defaulting to None if not found
```

### Comparing `wkregister-0.0.6/src/wkregister.egg-info/PKG-INFO` & `wkregister-0.0.7/src/wkregister.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkregister
-Version: 0.0.6
+Version: 0.0.7
 Summary: A wk register library for python
 Author-email: Gustavo <gustavo.gordillo.giron@gmail.com>
 Project-URL: Homepage, https://github.com/gtavo95/wknmi.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -154,7 +154,40 @@
         status="success",
         errorMessage=None,
         service="pay-service",
     )
     # The record is returned for demonstration purposes
     return {"result": "ok", "record": record}
 ```
+
+### Utilize the Built-In Send Method
+
+he send method is designed to forward records to a Kafka topic without requiring additional decorators. Below is an example that demonstrates how to use the send method with the Records model from the wkregister.models module. This example involves sending a record asynchronously:
+
+```python
+from wkregister.models import Records
+import asyncio
+
+async def sendRecord():
+    """
+    This asynchronous function creates and sends a record to a Kafka topic.
+    It constructs an instance of the Records class with predefined attributes and
+    sends the instance using its built-in asynchronous send method.
+    """
+    # Creating an instance of the Records class
+    record = Records(
+        org="testorg",           # Organization identifier
+        key="your-key",          # Unique key for the record
+        userId="1",              # User ID associated with the record
+        actionType="update",     # Type of action performed
+        status="success",        # Status of the action
+        errorMessage=None,       # Error message, if any (None if no errors)
+        service="pay-service",   # Service associated with the record
+        payload={"hola": "mundo"}  # Payload of the record (example data)
+    )
+    # Sending the record asynchronously to a Kafka topic
+    await record.send()
+
+# Running the asynchronous function using asyncio's event loop
+asyncio.run(sendRecord())
+
+```
```

