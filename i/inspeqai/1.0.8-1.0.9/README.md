# Comparing `tmp/inspeqai-1.0.8.tar.gz` & `tmp/inspeqai-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspeqai-1.0.8.tar", last modified: Fri Mar  8 16:34:42 2024, max compression
+gzip compressed data, was "inspeqai-1.0.9.tar", last modified: Fri Mar  8 16:49:53 2024, max compression
```

## Comparing `inspeqai-1.0.8.tar` & `inspeqai-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 socrates  (1000) socrates  (1000)        0 2024-03-08 16:34:42.096528 inspeqai-1.0.8/
--rw-rw-r--   0 socrates  (1000) socrates  (1000)    11357 2024-02-08 12:25:27.000000 inspeqai-1.0.8/LICENSE
--rw-rw-r--   0 socrates  (1000) socrates  (1000)     4578 2024-03-08 16:34:42.096528 inspeqai-1.0.8/PKG-INFO
--rw-rw-r--   0 socrates  (1000) socrates  (1000)     4281 2024-03-08 16:24:09.000000 inspeqai-1.0.8/README.md
-drwxrwxr-x   0 socrates  (1000) socrates  (1000)        0 2024-03-08 16:34:42.096528 inspeqai-1.0.8/inspeq/
--rw-rw-r--   0 socrates  (1000) socrates  (1000)        0 2024-02-08 12:25:27.000000 inspeqai-1.0.8/inspeq/__init__.py
--rw-rw-r--   0 socrates  (1000) socrates  (1000)     6960 2024-03-08 14:02:12.000000 inspeqai-1.0.8/inspeq/client.py
-drwxrwxr-x   0 socrates  (1000) socrates  (1000)        0 2024-03-08 16:34:42.096528 inspeqai-1.0.8/inspeqai.egg-info/
--rw-rw-r--   0 socrates  (1000) socrates  (1000)     4578 2024-03-08 16:34:42.000000 inspeqai-1.0.8/inspeqai.egg-info/PKG-INFO
--rw-rw-r--   0 socrates  (1000) socrates  (1000)      221 2024-03-08 16:34:42.000000 inspeqai-1.0.8/inspeqai.egg-info/SOURCES.txt
--rw-rw-r--   0 socrates  (1000) socrates  (1000)        1 2024-03-08 16:34:42.000000 inspeqai-1.0.8/inspeqai.egg-info/dependency_links.txt
--rw-rw-r--   0 socrates  (1000) socrates  (1000)        9 2024-03-08 16:34:42.000000 inspeqai-1.0.8/inspeqai.egg-info/requires.txt
--rw-rw-r--   0 socrates  (1000) socrates  (1000)        7 2024-03-08 16:34:42.000000 inspeqai-1.0.8/inspeqai.egg-info/top_level.txt
--rw-rw-r--   0 socrates  (1000) socrates  (1000)       38 2024-03-08 16:34:42.096528 inspeqai-1.0.8/setup.cfg
--rw-rw-r--   0 socrates  (1000) socrates  (1000)      725 2024-03-08 16:33:08.000000 inspeqai-1.0.8/setup.py
+drwxrwxr-x   0 socrates  (1000) socrates  (1000)        0 2024-03-08 16:49:53.579366 inspeqai-1.0.9/
+-rw-rw-r--   0 socrates  (1000) socrates  (1000)    11357 2024-02-08 12:25:27.000000 inspeqai-1.0.9/LICENSE
+-rw-rw-r--   0 socrates  (1000) socrates  (1000)     4582 2024-03-08 16:49:53.579366 inspeqai-1.0.9/PKG-INFO
+-rw-rw-r--   0 socrates  (1000) socrates  (1000)     4285 2024-03-08 16:48:30.000000 inspeqai-1.0.9/README.md
+drwxrwxr-x   0 socrates  (1000) socrates  (1000)        0 2024-03-08 16:49:53.579366 inspeqai-1.0.9/inspeq/
+-rw-rw-r--   0 socrates  (1000) socrates  (1000)        0 2024-02-08 12:25:27.000000 inspeqai-1.0.9/inspeq/__init__.py
+-rw-rw-r--   0 socrates  (1000) socrates  (1000)     6960 2024-03-08 16:38:44.000000 inspeqai-1.0.9/inspeq/client.py
+drwxrwxr-x   0 socrates  (1000) socrates  (1000)        0 2024-03-08 16:49:53.579366 inspeqai-1.0.9/inspeqai.egg-info/
+-rw-rw-r--   0 socrates  (1000) socrates  (1000)     4582 2024-03-08 16:49:53.000000 inspeqai-1.0.9/inspeqai.egg-info/PKG-INFO
+-rw-rw-r--   0 socrates  (1000) socrates  (1000)      221 2024-03-08 16:49:53.000000 inspeqai-1.0.9/inspeqai.egg-info/SOURCES.txt
+-rw-rw-r--   0 socrates  (1000) socrates  (1000)        1 2024-03-08 16:49:53.000000 inspeqai-1.0.9/inspeqai.egg-info/dependency_links.txt
+-rw-rw-r--   0 socrates  (1000) socrates  (1000)        9 2024-03-08 16:49:53.000000 inspeqai-1.0.9/inspeqai.egg-info/requires.txt
+-rw-rw-r--   0 socrates  (1000) socrates  (1000)        7 2024-03-08 16:49:53.000000 inspeqai-1.0.9/inspeqai.egg-info/top_level.txt
+-rw-rw-r--   0 socrates  (1000) socrates  (1000)       38 2024-03-08 16:49:53.579366 inspeqai-1.0.9/setup.cfg
+-rw-rw-r--   0 socrates  (1000) socrates  (1000)      725 2024-03-08 16:48:19.000000 inspeqai-1.0.9/setup.py
```

### Comparing `inspeqai-1.0.8/LICENSE` & `inspeqai-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `inspeqai-1.0.8/PKG-INFO` & `inspeqai-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspeqai
-Version: 1.0.8
+Version: 1.0.9
 Summary: Inspeq AI SDK
 Home-page: UNKNOWN
 Author: Inspeq
 License: Apache 2.0
 Project-URL: Source, https://github.com/inspeq/inspeq-py-sdk
 Platform: UNKNOWN
 Requires-Python: >=3.10
@@ -79,15 +79,15 @@
 
 '''Note : Do not change the structure of input data keep the structure as it
 is. Put your data at places of your_llm_input_context, your_llm_input_query
 and your_llm_output .
 
 '''
 print("\n   grammatical_correctness is:")
-print(inspeq_eval.grammatical_correctness(input_data))
+print(inspeq_instance.grammatical_correctness(input_data))
 #get all metrices in one function
 
 print(inspeq_instance.get_all_metrices(input_data))
 
 ```
 
 ### All Metrics provided by Inspeq sdk
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: inspeqai Version: 1.0.8 Summary: Inspeq AI SDK
+Metadata-Version: 2.1 Name: inspeqai Version: 1.0.9 Summary: Inspeq AI SDK
 Home-page: UNKNOWN Author: Inspeq License: Apache 2.0 Project-URL: Source,
 https://github.com/inspeq/inspeq-py-sdk Platform: UNKNOWN Requires-Python:
 >=3.10 Description-Content-Type: text/markdown License-File: LICENSE ## Project
 Description Inspeqai python SDK ## Inspeq ## More detail 0fficial Documentation
 Click _H_e_r_e ### Creating a Virtual Environment in Linux and Windows ### Linux OS
 / MAC OS ### Using venv (Python 3) 1. Open a terminal. 2. Navigate to the
 directory where you want to create the virtual environment. 3. Run the
@@ -17,15 +17,15 @@
 inspeq.client import Evaluator #initialization API_KEY = "your_sdk_api_key"
 inspeq_instance = Evaluator(sdk_api_key=API_KEY) # Example input data
 input_data = { "llm_input_query": "your_llm_input_query", "llm_input_context":
 "your_llm_input_context", "llm_output": "your_llm_output", } '''Note : Do not
 change the structure of input data keep the structure as it is. Put your data
 at places of your_llm_input_context, your_llm_input_query and your_llm_output .
 ''' print("\n grammatical_correctness is:") print
-(inspeq_eval.grammatical_correctness(input_data)) #get all metrices in one
+(inspeq_instance.grammatical_correctness(input_data)) #get all metrices in one
 function print(inspeq_instance.get_all_metrices(input_data)) ``` ### All
 Metrics provided by Inspeq sdk ```py print("Factual Consistency:",
 inspeq_instance.factual_consistency(input_data)) print("Answer Relevance:",
 inspeq_instance.answer_relevance(input_data)) print("Response Tone:",
 inspeq_instance.response_tone(input_data)) print("Grammatical Correctness:",
 inspeq_instance.grammatical_correctness(input_data)) print("Fluency:",
 inspeq_instance.fluency(input_data)) print("Do Not Use Keywords:",
```

### Comparing `inspeqai-1.0.8/README.md` & `inspeqai-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 '''Note : Do not change the structure of input data keep the structure as it
 is. Put your data at places of your_llm_input_context, your_llm_input_query
 and your_llm_output .
 
 '''
 print("\n   grammatical_correctness is:")
-print(inspeq_eval.grammatical_correctness(input_data))
+print(inspeq_instance.grammatical_correctness(input_data))
 #get all metrices in one function
 
 print(inspeq_instance.get_all_metrices(input_data))
 
 ```
 
 ### All Metrics provided by Inspeq sdk
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
 inspeq.client import Evaluator #initialization API_KEY = "your_sdk_api_key"
 inspeq_instance = Evaluator(sdk_api_key=API_KEY) # Example input data
 input_data = { "llm_input_query": "your_llm_input_query", "llm_input_context":
 "your_llm_input_context", "llm_output": "your_llm_output", } '''Note : Do not
 change the structure of input data keep the structure as it is. Put your data
 at places of your_llm_input_context, your_llm_input_query and your_llm_output .
 ''' print("\n grammatical_correctness is:") print
-(inspeq_eval.grammatical_correctness(input_data)) #get all metrices in one
+(inspeq_instance.grammatical_correctness(input_data)) #get all metrices in one
 function print(inspeq_instance.get_all_metrices(input_data)) ``` ### All
 Metrics provided by Inspeq sdk ```py print("Factual Consistency:",
 inspeq_instance.factual_consistency(input_data)) print("Answer Relevance:",
 inspeq_instance.answer_relevance(input_data)) print("Response Tone:",
 inspeq_instance.response_tone(input_data)) print("Grammatical Correctness:",
 inspeq_instance.grammatical_correctness(input_data)) print("Fluency:",
 inspeq_instance.fluency(input_data)) print("Do Not Use Keywords:",
```

### Comparing `inspeqai-1.0.8/inspeq/client.py` & `inspeqai-1.0.9/inspeq/client.py`

 * *Files identical despite different names*

### Comparing `inspeqai-1.0.8/inspeqai.egg-info/PKG-INFO` & `inspeqai-1.0.9/inspeqai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspeqai
-Version: 1.0.8
+Version: 1.0.9
 Summary: Inspeq AI SDK
 Home-page: UNKNOWN
 Author: Inspeq
 License: Apache 2.0
 Project-URL: Source, https://github.com/inspeq/inspeq-py-sdk
 Platform: UNKNOWN
 Requires-Python: >=3.10
@@ -79,15 +79,15 @@
 
 '''Note : Do not change the structure of input data keep the structure as it
 is. Put your data at places of your_llm_input_context, your_llm_input_query
 and your_llm_output .
 
 '''
 print("\n   grammatical_correctness is:")
-print(inspeq_eval.grammatical_correctness(input_data))
+print(inspeq_instance.grammatical_correctness(input_data))
 #get all metrices in one function
 
 print(inspeq_instance.get_all_metrices(input_data))
 
 ```
 
 ### All Metrics provided by Inspeq sdk
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: inspeqai Version: 1.0.8 Summary: Inspeq AI SDK
+Metadata-Version: 2.1 Name: inspeqai Version: 1.0.9 Summary: Inspeq AI SDK
 Home-page: UNKNOWN Author: Inspeq License: Apache 2.0 Project-URL: Source,
 https://github.com/inspeq/inspeq-py-sdk Platform: UNKNOWN Requires-Python:
 >=3.10 Description-Content-Type: text/markdown License-File: LICENSE ## Project
 Description Inspeqai python SDK ## Inspeq ## More detail 0fficial Documentation
 Click _H_e_r_e ### Creating a Virtual Environment in Linux and Windows ### Linux OS
 / MAC OS ### Using venv (Python 3) 1. Open a terminal. 2. Navigate to the
 directory where you want to create the virtual environment. 3. Run the
@@ -17,15 +17,15 @@
 inspeq.client import Evaluator #initialization API_KEY = "your_sdk_api_key"
 inspeq_instance = Evaluator(sdk_api_key=API_KEY) # Example input data
 input_data = { "llm_input_query": "your_llm_input_query", "llm_input_context":
 "your_llm_input_context", "llm_output": "your_llm_output", } '''Note : Do not
 change the structure of input data keep the structure as it is. Put your data
 at places of your_llm_input_context, your_llm_input_query and your_llm_output .
 ''' print("\n grammatical_correctness is:") print
-(inspeq_eval.grammatical_correctness(input_data)) #get all metrices in one
+(inspeq_instance.grammatical_correctness(input_data)) #get all metrices in one
 function print(inspeq_instance.get_all_metrices(input_data)) ``` ### All
 Metrics provided by Inspeq sdk ```py print("Factual Consistency:",
 inspeq_instance.factual_consistency(input_data)) print("Answer Relevance:",
 inspeq_instance.answer_relevance(input_data)) print("Response Tone:",
 inspeq_instance.response_tone(input_data)) print("Grammatical Correctness:",
 inspeq_instance.grammatical_correctness(input_data)) print("Fluency:",
 inspeq_instance.fluency(input_data)) print("Do Not Use Keywords:",
```

### Comparing `inspeqai-1.0.8/setup.py` & `inspeqai-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name="inspeqai",
-    version="1.0.8",
+    version="1.0.9",
     packages=find_packages(include=["inspeq*"]),
     license="Apache 2.0",
     author="Inspeq",
      install_requires=[
         'requests', 
             # Specify dependencies if any
     ],
```

