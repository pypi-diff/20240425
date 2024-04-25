# Comparing `tmp/ALLMDEV-1.2.2-py3-none-any.whl.zip` & `tmp/ALLMDEV-1.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,14 @@
-Zip file size: 6787 bytes, number of entries: 10
+Zip file size: 9781 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat       39 b- defN 24-Apr-17 06:01 ALLMDEV/__init__.py
--rw-rw-rw-  2.0 fat     1904 b- defN 24-Apr-20 05:31 ALLMDEV/api.py
 -rw-rw-rw-  2.0 fat      757 b- defN 24-Apr-17 06:35 ALLMDEV/cli.py
 -rw-rw-rw-  2.0 fat     2579 b- defN 24-Apr-20 10:27 ALLMDEV/generate.py
 -rw-rw-rw-  2.0 fat    10334 b- defN 24-Apr-19 14:10 ALLMDEV/instruct.py
--rw-rw-rw-  2.0 fat     2366 b- defN 24-Apr-20 10:27 ALLMDEV-1.2.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-20 10:27 ALLMDEV-1.2.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       81 b- defN 24-Apr-20 10:27 ALLMDEV-1.2.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-20 10:27 ALLMDEV-1.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      760 b- defN 24-Apr-20 10:27 ALLMDEV-1.2.2.dist-info/RECORD
-10 files, 18920 bytes uncompressed, 5499 bytes compressed:  70.9%
+-rw-rw-rw-  2.0 fat     1985 b- defN 24-Apr-25 11:09 ALLMDEV/rag.py
+-rw-rw-rw-  2.0 fat     3016 b- defN 24-Apr-25 07:21 ALLMDEV/ragrun.py
+-rw-rw-rw-  2.0 fat     3144 b- defN 24-Apr-25 07:25 ALLMDEV/ragserve.py
+-rw-rw-rw-  2.0 fat     3227 b- defN 24-Apr-25 12:35 ALLMDEV-1.2.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-25 12:35 ALLMDEV-1.2.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      192 b- defN 24-Apr-25 12:35 ALLMDEV-1.2.4.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-25 12:35 ALLMDEV-1.2.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      911 b- defN 24-Apr-25 12:35 ALLMDEV-1.2.4.dist-info/RECORD
+12 files, 26284 bytes uncompressed, 8269 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -1,31 +1,37 @@
 Filename: ALLMDEV/__init__.py
 Comment: 
 
-Filename: ALLMDEV/api.py
-Comment: 
-
 Filename: ALLMDEV/cli.py
 Comment: 
 
 Filename: ALLMDEV/generate.py
 Comment: 
 
 Filename: ALLMDEV/instruct.py
 Comment: 
 
-Filename: ALLMDEV-1.2.2.dist-info/METADATA
+Filename: ALLMDEV/rag.py
+Comment: 
+
+Filename: ALLMDEV/ragrun.py
+Comment: 
+
+Filename: ALLMDEV/ragserve.py
+Comment: 
+
+Filename: ALLMDEV-1.2.4.dist-info/METADATA
 Comment: 
 
-Filename: ALLMDEV-1.2.2.dist-info/WHEEL
+Filename: ALLMDEV-1.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: ALLMDEV-1.2.2.dist-info/entry_points.txt
+Filename: ALLMDEV-1.2.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: ALLMDEV-1.2.2.dist-info/top_level.txt
+Filename: ALLMDEV-1.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: ALLMDEV-1.2.2.dist-info/RECORD
+Filename: ALLMDEV-1.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ALLMDEV/api.py` & `ALLMDEV/ragserve.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,88 @@
 from flask import Flask, request, jsonify
-from .instruct import load_model
 from llama_index.llms.llama_cpp import LlamaCPP
+from .instruct import load_model
 import os
-import argparse
+from langchain.embeddings import SentenceTransformerEmbeddings
+from langchain.vectorstores import Chroma
+
+
+persist_directory = 'db'
+embeddings = SentenceTransformerEmbeddings(model_name="all-MiniLM-L6-v2")
 
-parser = argparse.ArgumentParser()
-parser.add_argument("--host", type=str, default="127.0.0.1", help="Host on which you wish to run the API server")
-parser.add_argument("--port", type=str, default='5000', help="Host on which you wish to run the API server")
+db = Chroma(embedding_function=embeddings, persist_directory=persist_directory)
 
 app = Flask(__name__)
-app.config['DEBUG'] = False
+
+# Check if apiconfig.txt exists in the model folder
+config_file_path = os.path.join('model', 'apiconfig.txt')
+if not os.path.exists(config_file_path):
+    # Create apiconfig.txt with default values
+    with open(config_file_path, 'w') as file:
+       file.write('Host=127.0.0.1\n')
+       file.write('Port=5000\n')
+       file.write('CertFile=""\n')
+       file.write('CertKey=""\n')
+
+# Read host and port from apiconfig.txt
+if os.path.exists(config_file_path):
+    with open(config_file_path, 'r') as file:
+        for line in file:
+            key, value = line.strip().split('=')
+            if key == 'Host':
+                host = value
+            elif key == 'Port':
+                port = int(value)
+            elif key == 'CertFile':
+                cert_file = value.strip('"')
+            elif key == 'CertKey':
+                cert_key = value.strip('"')
+else:
+    print("File doesn't exist.")
+    host = '127.0.0.1'
+    port = 5000
+    cert_file = ""
+    cert_key = ""
+
+print("Host:", host)
+print("Port:", port)
+print("CertFile:", cert_file)
+print("CertKey:", cert_key)
 
 model_files = [f for f in os.listdir('model') if f.endswith('.gguf')]
 model_path = load_model(model_files[0]) if model_files else None
 
-def generate(model):
-    llm = LlamaCPP(
-            model_path=model,
-            temperature=0.5,
-            max_new_tokens=512,
-            context_window=3900,
-            verbose=False,
-        )
-    return llm
-
-def infer(llm, prompt):
-    if prompt.lower() == "exit":
-        return "Exiting chat."
+llm = LlamaCPP(
+    model_path=model_path,
+    temperature=0.1,
+    max_new_tokens=512,
+    context_window=3900,
+    model_kwargs={"n_gpu_layers": 0},
+    verbose=False,
+)
+
+@app.route('/v1/chat/completions', methods=['POST'])
+def chat():
+    user_input = request.json.get("input")
+
+    if user_input.lower() == "exit":
+        return jsonify({"response": "Exiting chat."})
+
+    prompt_template = "You are a friendly assistant, who gives context aware responses on user query. Kindly analyse the provided context and give proper response\n   Context: {context}\n query:<s>[INST] {prompt} [/INST]"
+    docs = db.similarity_search(user_input,k=1)
+    context=docs[0].page_content
+    prompt = prompt_template.format(context=context,prompt=user_input)
+
     response_iter = llm.stream_complete(prompt)
     response_text = ''.join(response.delta for response in response_iter)
-    return response_text
 
-@app.route('/')
-def index():
-    return "Welcome to the allmdev API!"
-
-@app.route('/v1/chat/completions', methods=['POST'])
-def infer_text():
-    user_input = request.data.decode('utf-8')
-    print("Received input:", user_input)  # Debug statement
-
-    if model_path is None:
-        return "Model is not loaded or initialized. Kindly run 'allm-run --name model_name_or_path' to initialize the model"
-
-    llm = generate(model_path)
-    response = infer(llm, user_input)
-    print("Generated response:", response)  # Debug statement
-    return response
+    return jsonify({"response": response_text})
 
 def main():
-    args = parser.parse_args()
-    host = args.host
-    port = args.port
-    print(f"Inference is working on http://{host}:{port}/v1/chat/completions")
-    app.run(host=host, port=port)
-    
-if __name__ == '__main__':
+        print(f"Inference is working on http://{host}:{port}/v1/chat/completions. You can configure custom host IP and port, and ssl certificate via the apiconfig.txt file available at {config_file_path}")
+        if cert_file is not "" and cert_key is not "":
+            app.run(host=host, port=port, debug=False, ssl_context=[cert_file,cert_key])
+        else:
+            app.run(host=host, port=port, debug=False)
+
+if __name__ == "__main__":
     main()
```

## Comparing `ALLMDEV-1.2.2.dist-info/RECORD` & `ALLMDEV-1.2.4.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 ALLMDEV/__init__.py,sha256=8XSO2SVH9cZ_Iut8rNwcDxtEaBp4LIdXP6hAKGRgeaI,39
-ALLMDEV/api.py,sha256=Y69wMrLgODKsoiWQRH9CCVLU4IA8QYO9rX3C0fciEGI,1904
 ALLMDEV/cli.py,sha256=wWOt7Uv_DmQKT821rEIaEVh9MFJVz0n19BXgwTHsdDY,757
 ALLMDEV/generate.py,sha256=bjvXRrlHpe_-TsWDAL-OoivuTO9225gOK15FKRlBvIg,2579
 ALLMDEV/instruct.py,sha256=9cjx7CnIc-C-LXxVl2THdlrNX3WXcZ0rXKXWVpZ0BXY,10334
-ALLMDEV-1.2.2.dist-info/METADATA,sha256=BLX5if4AII5rc4TX3sCjgRb-5ZAWmZ-WUzLNyelhJbk,2366
-ALLMDEV-1.2.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ALLMDEV-1.2.2.dist-info/entry_points.txt,sha256=Vg1PNkMT6_InD8pcRNpouHe5eJ-VSb9lWSb7XeeJr1o,81
-ALLMDEV-1.2.2.dist-info/top_level.txt,sha256=zQYMpzphh7BJt_BseuV6ImX-bYvNZcuXsmNLbIr57Ts,8
-ALLMDEV-1.2.2.dist-info/RECORD,,
+ALLMDEV/rag.py,sha256=jpb_cbv9GqhAJC3Ju3yJEqhWUXmKaKPkPBBTODXfwz0,1985
+ALLMDEV/ragrun.py,sha256=4mThVEP---UPQn-5zFwGkg202A7U1PNn_yZTQElaFsc,3016
+ALLMDEV/ragserve.py,sha256=WqmwVnlEbmc712GLuaEMAXBWB4U_6Wf8RbWNY2TgJcg,3144
+ALLMDEV-1.2.4.dist-info/METADATA,sha256=qM54Hvixes_kii9in2O9fyYfQjOWHQYGWYwyjVQM95E,3227
+ALLMDEV-1.2.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ALLMDEV-1.2.4.dist-info/entry_points.txt,sha256=TidmTXG14j0DW0hCJrqDCYZNY4SBrBdcyJ6pNIr9X70,192
+ALLMDEV-1.2.4.dist-info/top_level.txt,sha256=zQYMpzphh7BJt_BseuV6ImX-bYvNZcuXsmNLbIr57Ts,8
+ALLMDEV-1.2.4.dist-info/RECORD,,
```

