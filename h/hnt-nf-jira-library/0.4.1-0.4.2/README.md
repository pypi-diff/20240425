# Comparing `tmp/hnt_nf_jira_library-0.4.1.tar.gz` & `tmp/hnt_nf_jira_library-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnt_nf_jira_library-0.4.1.tar", last modified: Tue Apr 23 12:58:44 2024, max compression
+gzip compressed data, was "hnt_nf_jira_library-0.4.2.tar", last modified: Thu Apr 25 16:50:24 2024, max compression
```

## Comparing `hnt_nf_jira_library-0.4.1.tar` & `hnt_nf_jira_library-0.4.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 12:58:44.127407 hnt_nf_jira_library-0.4.1/
--rw-rw-rw-   0        0        0      183 2024-04-23 12:58:44.127407 hnt_nf_jira_library-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-02-23 21:17:37.000000 hnt_nf_jira_library-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 12:58:44.100893 hnt_nf_jira_library-0.4.1/hnt_nf_jira_library.egg-info/
--rw-rw-rw-   0        0        0      183 2024-04-23 12:58:43.000000 hnt_nf_jira_library-0.4.1/hnt_nf_jira_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1035 2024-04-23 12:58:44.000000 hnt_nf_jira_library-0.4.1/hnt_nf_jira_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 12:58:43.000000 hnt_nf_jira_library-0.4.1/hnt_nf_jira_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-23 12:58:43.000000 hnt_nf_jira_library-0.4.1/hnt_nf_jira_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-23 12:58:43.000000 hnt_nf_jira_library-0.4.1/hnt_nf_jira_library.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-23 12:58:44.102892 hnt_nf_jira_library-0.4.1/nf_jira/
--rw-rw-rw-   0        0        0       30 2024-02-26 12:03:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 12:58:44.121892 hnt_nf_jira_library-0.4.1/nf_jira/entities/
--rw-rw-rw-   0        0        0       92 2024-02-23 21:17:37.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/anexo.py
--rw-rw-rw-   0        0        0      131 2024-04-22 11:49:00.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/chave_acesso.py
-drwxrwxrwx   0        0        0        0 2024-04-23 12:58:44.126408 hnt_nf_jira_library-0.4.1/nf_jira/entities/classes/
--rw-rw-rw-   0        0        0     4893 2024-04-22 11:49:00.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/classes/form_jira.py
--rw-rw-rw-   0        0        0     4338 2024-04-22 11:49:00.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/classes/helper.py
--rw-rw-rw-   0        0        0     2019 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/classes/issue_fields.py
--rw-rw-rw-   0        0        0     5454 2024-04-22 11:49:00.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/classes/issue_jira.py
--rw-rw-rw-   0        0        0     1695 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/classes/n8n_domain.py
--rw-rw-rw-   0        0        0     3411 2024-04-22 11:49:00.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/constants.py
--rw-rw-rw-   0        0        0      331 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/dados_basicos_fatura.py
--rw-rw-rw-   0        0        0      145 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/dados_basicos_miro.py
--rw-rw-rw-   0        0        0      198 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/dados_nfe.py
--rw-rw-rw-   0        0        0       76 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/detalhe.py
--rw-rw-rw-   0        0        0      234 2024-04-22 11:49:00.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/fatura.py
--rw-rw-rw-   0        0        0      140 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/item.py
--rw-rw-rw-   0        0        0      224 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/itens_fatura.py
--rw-rw-rw-   0        0        0       97 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/jira_info.py
--rw-rw-rw-   0        0        0      448 2024-04-22 11:49:00.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/miro.py
--rw-rw-rw-   0        0        0      127 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/nfe_sefaz.py
--rw-rw-rw-   0        0        0      354 2024-04-22 11:49:00.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/nota_pedido.py
--rw-rw-rw-   0        0        0      169 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/pagamento.py
--rw-rw-rw-   0        0        0       92 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/referencia_pedido.py
--rw-rw-rw-   0        0        0      173 2024-02-26 12:03:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/sintese_itens.py
--rw-rw-rw-   0        0        0       78 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/sintese_miro.py
--rw-rw-rw-   0        0        0    15563 2024-04-23 12:55:45.000000 hnt_nf_jira_library-0.4.1/nf_jira/wrapper_nf_jira.py
--rw-rw-rw-   0        0        0       42 2024-04-23 12:58:44.127407 hnt_nf_jira_library-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0      510 2024-04-23 12:58:04.000000 hnt_nf_jira_library-0.4.1/setup.py
+drwxr-xr-x   0 ipepe      (501) staff       (20)        0 2024-04-25 16:50:24.185615 hnt_nf_jira_library-0.4.2/
+-rw-r--r--   0 ipepe      (501) staff       (20)      276 2024-04-25 16:50:24.185079 hnt_nf_jira_library-0.4.2/PKG-INFO
+-rw-r--r--   0 ipepe      (501) staff       (20)      381 2024-02-29 14:45:46.000000 hnt_nf_jira_library-0.4.2/README.md
+drwxr-xr-x   0 ipepe      (501) staff       (20)        0 2024-04-25 16:50:24.184325 hnt_nf_jira_library-0.4.2/hnt_nf_jira_library.egg-info/
+-rw-r--r--   0 ipepe      (501) staff       (20)      276 2024-04-25 16:50:24.000000 hnt_nf_jira_library-0.4.2/hnt_nf_jira_library.egg-info/PKG-INFO
+-rw-r--r--   0 ipepe      (501) staff       (20)     1035 2024-04-25 16:50:24.000000 hnt_nf_jira_library-0.4.2/hnt_nf_jira_library.egg-info/SOURCES.txt
+-rw-r--r--   0 ipepe      (501) staff       (20)        1 2024-04-25 16:50:24.000000 hnt_nf_jira_library-0.4.2/hnt_nf_jira_library.egg-info/dependency_links.txt
+-rw-r--r--   0 ipepe      (501) staff       (20)       55 2024-04-25 16:50:24.000000 hnt_nf_jira_library-0.4.2/hnt_nf_jira_library.egg-info/requires.txt
+-rw-r--r--   0 ipepe      (501) staff       (20)        8 2024-04-25 16:50:24.000000 hnt_nf_jira_library-0.4.2/hnt_nf_jira_library.egg-info/top_level.txt
+drwxr-xr-x   0 ipepe      (501) staff       (20)        0 2024-04-25 16:50:24.166522 hnt_nf_jira_library-0.4.2/nf_jira/
+-rw-r--r--   0 ipepe      (501) staff       (20)       30 2024-04-19 08:27:45.000000 hnt_nf_jira_library-0.4.2/nf_jira/__init__.py
+drwxr-xr-x   0 ipepe      (501) staff       (20)        0 2024-04-25 16:50:24.180642 hnt_nf_jira_library-0.4.2/nf_jira/entities/
+-rw-r--r--   0 ipepe      (501) staff       (20)       88 2024-04-19 08:27:42.000000 hnt_nf_jira_library-0.4.2/nf_jira/entities/anexo.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      126 2024-04-24 18:49:32.000000 hnt_nf_jira_library-0.4.2/nf_jira/entities/chave_acesso.py
+drwxr-xr-x   0 ipepe      (501) staff       (20)        0 2024-04-25 16:50:24.183576 hnt_nf_jira_library-0.4.2/nf_jira/entities/classes/
+-rw-r--r--   0 ipepe      (501) staff       (20)     4741 2024-04-19 08:28:17.000000 hnt_nf_jira_library-0.4.2/nf_jira/entities/classes/form_jira.py
+-rw-r--r--   0 ipepe      (501) staff       (20)     4234 2024-04-19 08:28:17.000000 hnt_nf_jira_library-0.4.2/nf_jira/entities/classes/helper.py
+-rw-r--r--   0 ipepe      (501) staff       (20)     1961 2024-04-19 08:27:45.000000 hnt_nf_jira_library-0.4.2/nf_jira/entities/classes/issue_fields.py
+-rw-r--r--   0 ipepe      (501) staff       (20)     5291 2024-04-19 08:28:17.000000 hnt_nf_jira_library-0.4.2/nf_jira/entities/classes/issue_jira.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      747 2024-04-25 13:11:39.000000 hnt_nf_jira_library-0.4.2/nf_jira/entities/classes/n8n_domain.py
+-rw-r--r--   0 ipepe      (501) staff       (20)     3305 2024-04-25 15:01:31.000000 hnt_nf_jira_library-0.4.2/nf_jira/entities/constants.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      319 2024-04-19 08:27:45.000000 hnt_nf_jira_library-0.4.2/nf_jira/entities/dados_basicos_fatura.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      139 2024-04-19 08:27:45.000000 hnt_nf_jira_library-0.4.2/nf_jira/entities/dados_basicos_miro.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      191 2024-04-19 08:27:45.000000 hnt_nf_jira_library-0.4.2/nf_jira/entities/dados_nfe.py
+-rw-r--r--   0 ipepe      (501) staff       (20)       73 2024-04-19 08:27:45.000000 hnt_nf_jira_library-0.4.2/nf_jira/entities/detalhe.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      226 2024-04-19 08:28:17.000000 hnt_nf_jira_library-0.4.2/nf_jira/entities/fatura.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      134 2024-04-19 08:27:45.000000 hnt_nf_jira_library-0.4.2/nf_jira/entities/item.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      215 2024-04-19 08:27:45.000000 hnt_nf_jira_library-0.4.2/nf_jira/entities/itens_fatura.py
+-rw-r--r--   0 ipepe      (501) staff       (20)       93 2024-04-19 08:27:45.000000 hnt_nf_jira_library-0.4.2/nf_jira/entities/jira_info.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      434 2024-04-19 08:28:17.000000 hnt_nf_jira_library-0.4.2/nf_jira/entities/miro.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      122 2024-04-19 08:27:45.000000 hnt_nf_jira_library-0.4.2/nf_jira/entities/nfe_sefaz.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      339 2024-04-19 08:28:17.000000 hnt_nf_jira_library-0.4.2/nf_jira/entities/nota_pedido.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      162 2024-04-19 08:27:45.000000 hnt_nf_jira_library-0.4.2/nf_jira/entities/pagamento.py
+-rw-r--r--   0 ipepe      (501) staff       (20)       89 2024-04-19 08:27:45.000000 hnt_nf_jira_library-0.4.2/nf_jira/entities/referencia_pedido.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      165 2024-04-19 08:27:45.000000 hnt_nf_jira_library-0.4.2/nf_jira/entities/sintese_itens.py
+-rw-r--r--   0 ipepe      (501) staff       (20)       75 2024-04-19 08:27:45.000000 hnt_nf_jira_library-0.4.2/nf_jira/entities/sintese_miro.py
+-rw-r--r--   0 ipepe      (501) staff       (20)    14692 2024-04-25 15:01:28.000000 hnt_nf_jira_library-0.4.2/nf_jira/wrapper_nf_jira.py
+-rw-r--r--   0 ipepe      (501) staff       (20)       38 2024-04-25 16:50:24.185850 hnt_nf_jira_library-0.4.2/setup.cfg
+-rw-r--r--   0 ipepe      (501) staff       (20)      493 2024-04-25 15:02:23.000000 hnt_nf_jira_library-0.4.2/setup.py
```

### Comparing `hnt_nf_jira_library-0.4.1/hnt_nf_jira_library.egg-info/SOURCES.txt` & `hnt_nf_jira_library-0.4.2/hnt_nf_jira_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.1/nf_jira/entities/classes/form_jira.py` & `hnt_nf_jira_library-0.4.2/nf_jira/entities/classes/form_jira.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-import requests
-from ..constants import *
-from .helper import JsonHelper
-# from ...wrapper_nf_jira import wrapper_jira
-
-class FormJira:
-# class FormJira(wrapper_jira):
-
-    def __init__(self) -> None:
-        pass
-
-    def get_form_fields(self, issue_key, form_template, debug=False):
-
-        form_data = self._get_form_data(issue_key, form_template)
-        form_fields = self._get_form_fields_data(form_data)
-
-        JsonHelper().save_json(f"FormFields_{issue_key}_{form_template}", form_fields) if debug else None
-
-        return form_fields
-    
-    def get_form_id(self, issue_key, form_template):
-
-        forms_from_issue = self._get_forms_from_issue(issue_key)
-        form_id = self._get_form_id_data(forms_from_issue, form_template)
-
-        return form_id
-    
-    def get_form_jira_keys(self, issue_key, form_template):
-        
-        form_data = self._get_form_data(issue_key, form_template)
-        form_keys = self._get_form_jira_keys(form_data)
-
-        return form_keys
-
-    def _get_form_data(self, issue_key, form_template):
-
-        forms_from_issue = self._get_forms_from_issue(issue_key)
-        form_id = self._get_form_id_data(forms_from_issue, form_template)
-        form_data = self._get_form(form_id, issue_key)
-
-        return form_data
-
-    def _get_forms_from_issue(self, issue_key):
-
-        try:
-            request = requests.get(
-                f"{API_FORM_URL}/{CLOUD_ID}/issue/{issue_key}/form",
-                headers=API_ATLASSIAN_HEADERS,
-                auth=JIRA_AUTH,
-            )
-            request.raise_for_status()
-            data = request.json()
-            
-            return data
-        except requests.exceptions.HTTPError as e:
-            raise Exception(f"Erro ao receber formulario da issue:\n{e}")
-        
-    def _get_form_id_data(self, data, form_template):
-        
-        for form in data:
-            if form.get("formTemplate")['id'] == form_template:
-                form_id = form.get("id")
-
-        return form_id
-    
-    def _get_form(self, form_id, issue_key):
-
-        try:
-            request = requests.get(
-                f"{API_FORM_URL}/{CLOUD_ID}/issue/{issue_key}/form/{form_id}",
-                headers=API_ATLASSIAN_HEADERS,
-                auth=JIRA_AUTH,
-            )
-            request.raise_for_status()
-            data = request.json()
-
-            return data
-        except requests.exceptions.HTTPError as e:
-            raise Exception(f"Erro ao capturar formulario:\n{e}")
-        
-    def _get_form_fields_data(self, data):
-
-        fields_json = {}
-
-        fields_values = data.get('state')['answers']
-        fields_root = data.get('design')['questions']
-        
-        for root in fields_root:
-
-            field_name = fields_root[root].get('questionKey')
-            if fields_values.get(root) is not None:
-                # field_index = list(fields_values.get(root).keys())[0]
-                if "choices" in list(fields_values.get(root).keys()):
-                    field_value = fields_values.get(root)['choices']
-                else:
-                    field_index = list(fields_values.get(root).keys())[0]
-                    field_value = fields_values.get(root)[field_index]
-            else: 
-                field_value = None
-
-            fields_json[field_name] = field_value
-
-        return fields_json
-    
-    def _get_form_jira_keys(self, data):
-        field_keys = {}
-        fields_root = data.get('design')['questions']
-
-        for root in fields_root:
-
-            field_name = fields_root[root].get('questionKey')
-            jira_key = fields_root[root].get('jiraField')
-            field_keys[field_name] = jira_key
-
-        return field_keys
-
-    def update_jira_form(self, issue, data):
-
-        answers_schema = {
-            "1":"cod_nota_pedido",
-            "4":"cod_fatura",
-            "5":"status_liberacao",
-            "6":"data_liberacao",
-            "7":"cod_miro"
-        }
-
-        answers_json = {}
-
-        for answer in answers_schema:
-            answer_label = answers_schema[answer]
-            if answer_label in data:
-                answers_json[answer] = {"text": data[answer_label]}
-
-        answers = { "answers" : answers_json }
-
-        self._save_form_answers(answers, issue["issue_id"], issue["form_id"])
-
-        pass
-    
-    def _save_form_answers(self, answers, issue_id, form_id):
-
-        try:
-            requests.put(
-                f"{API_FORM_URL}/{CLOUD_ID}/issue/{issue_id}/form/{form_id}",
-                headers = API_ATLASSIAN_HEADERS,
-                auth = JIRA_AUTH,
-                json = answers,
-            )
-
-            pass
-
-        except requests.exceptions.HTTPError as e:
+import requests
+from ..constants import *
+from .helper import JsonHelper
+# from ...wrapper_nf_jira import wrapper_jira
+
+class FormJira:
+# class FormJira(wrapper_jira):
+
+    def __init__(self) -> None:
+        pass
+
+    def get_form_fields(self, issue_key, form_template, debug=False):
+
+        form_data = self._get_form_data(issue_key, form_template)
+        form_fields = self._get_form_fields_data(form_data)
+
+        JsonHelper().save_json(f"FormFields_{issue_key}_{form_template}", form_fields) if debug else None
+
+        return form_fields
+    
+    def get_form_id(self, issue_key, form_template):
+
+        forms_from_issue = self._get_forms_from_issue(issue_key)
+        form_id = self._get_form_id_data(forms_from_issue, form_template)
+
+        return form_id
+    
+    def get_form_jira_keys(self, issue_key, form_template):
+        
+        form_data = self._get_form_data(issue_key, form_template)
+        form_keys = self._get_form_jira_keys(form_data)
+
+        return form_keys
+
+    def _get_form_data(self, issue_key, form_template):
+
+        forms_from_issue = self._get_forms_from_issue(issue_key)
+        form_id = self._get_form_id_data(forms_from_issue, form_template)
+        form_data = self._get_form(form_id, issue_key)
+
+        return form_data
+
+    def _get_forms_from_issue(self, issue_key):
+
+        try:
+            request = requests.get(
+                f"{API_FORM_URL}/{CLOUD_ID}/issue/{issue_key}/form",
+                headers=API_ATLASSIAN_HEADERS,
+                auth=JIRA_AUTH,
+            )
+            request.raise_for_status()
+            data = request.json()
+            
+            return data
+        except requests.exceptions.HTTPError as e:
+            raise Exception(f"Erro ao receber formulario da issue:\n{e}")
+        
+    def _get_form_id_data(self, data, form_template):
+        
+        for form in data:
+            if form.get("formTemplate")['id'] == form_template:
+                form_id = form.get("id")
+
+        return form_id
+    
+    def _get_form(self, form_id, issue_key):
+
+        try:
+            request = requests.get(
+                f"{API_FORM_URL}/{CLOUD_ID}/issue/{issue_key}/form/{form_id}",
+                headers=API_ATLASSIAN_HEADERS,
+                auth=JIRA_AUTH,
+            )
+            request.raise_for_status()
+            data = request.json()
+
+            return data
+        except requests.exceptions.HTTPError as e:
+            raise Exception(f"Erro ao capturar formulario:\n{e}")
+        
+    def _get_form_fields_data(self, data):
+
+        fields_json = {}
+
+        fields_values = data.get('state')['answers']
+        fields_root = data.get('design')['questions']
+        
+        for root in fields_root:
+
+            field_name = fields_root[root].get('questionKey')
+            if fields_values.get(root) is not None:
+                # field_index = list(fields_values.get(root).keys())[0]
+                if "choices" in list(fields_values.get(root).keys()):
+                    field_value = fields_values.get(root)['choices']
+                else:
+                    field_index = list(fields_values.get(root).keys())[0]
+                    field_value = fields_values.get(root)[field_index]
+            else: 
+                field_value = None
+
+            fields_json[field_name] = field_value
+
+        return fields_json
+    
+    def _get_form_jira_keys(self, data):
+        field_keys = {}
+        fields_root = data.get('design')['questions']
+
+        for root in fields_root:
+
+            field_name = fields_root[root].get('questionKey')
+            jira_key = fields_root[root].get('jiraField')
+            field_keys[field_name] = jira_key
+
+        return field_keys
+
+    def update_jira_form(self, issue, data):
+
+        answers_schema = {
+            "1":"cod_nota_pedido",
+            "4":"cod_fatura",
+            "5":"status_liberacao",
+            "6":"data_liberacao",
+            "7":"cod_miro"
+        }
+
+        answers_json = {}
+
+        for answer in answers_schema:
+            answer_label = answers_schema[answer]
+            if answer_label in data:
+                answers_json[answer] = {"text": data[answer_label]}
+
+        answers = { "answers" : answers_json }
+
+        self._save_form_answers(answers, issue["issue_id"], issue["form_id"])
+
+        pass
+    
+    def _save_form_answers(self, answers, issue_id, form_id):
+
+        try:
+            requests.put(
+                f"{API_FORM_URL}/{CLOUD_ID}/issue/{issue_id}/form/{form_id}",
+                headers = API_ATLASSIAN_HEADERS,
+                auth = JIRA_AUTH,
+                json = answers,
+            )
+
+            pass
+
+        except requests.exceptions.HTTPError as e:
             raise Exception(f"Erro ao receber anexo Jira:\n{e}")
```

### Comparing `hnt_nf_jira_library-0.4.1/nf_jira/entities/classes/helper.py` & `hnt_nf_jira_library-0.4.2/nf_jira/entities/classes/helper.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-import json
-from os import getcwd, makedirs, path
-from nf_consumo.consumo_service import ConsumoService
-from ..constants import *
-
-class BaseHelper:
-
-    def __init__(self):
-        self.ConsumoService = ConsumoService()
-
-class JsonHelper(BaseHelper):
-
-    def save_json(self, filename, json_data):
-
-        path_dir = path.join(getcwd(), 'output/json')
-        if not path.exists(path_dir):
-            makedirs(path_dir)
-
-        with open(f"./output/json/{filename}.json", "w", encoding="utf-8") as json_file:
-            json.dump( json_data, json_file, ensure_ascii=False, indent=4)
-
-class JiraFieldsHelper(BaseHelper):
-
-    def remove_null_fields(self, fields):
-        fields_data_without_nulls = {}
-
-        for key, value in fields.items():
-            if value is not None:
-                fields_data_without_nulls[key] = value
-
-        return fields_data_without_nulls
-    
-    def _rename_fields(self, fields):
-        fields = self._fields
-        new_fields_data = {}
-
-        for key, value in self._jira_fields.items():
-            if value in fields:
-                if "text" in fields[value]:
-                    new_value = fields[value].get("text")
-                elif "date" in fields[value]:
-                    new_value = fields[value].get("date")
-                elif "value" in fields[value]:
-                    new_value = fields[value].get("value")
-                else:
-                    new_value = fields[value]
-
-                new_fields_data[key] = new_value
-
-        return new_fields_data
-    
-class GuiandoHelper(BaseHelper):
-        
-        def __init__(self):
-            self._check_sefaz = lambda form_data: form_data[POSSUI_CHAVE_ACESSO][0] == "1"
-            self._check_document_type = lambda document_type: 'nota_fiscal' if document_type == "2" else 'fatura'
-            self.ConsumoService = ConsumoService()
-
-        def download_pdf_nexinvoice(self, attachment):
-            path = attachment[ARQUIVOS_DA_FATURA][0]
-            pdf = self._download_pdf(path)
-            return pdf
-
-        def _download_pdf(self, pdf_path):
-            path_dir = path.join(getcwd(), "output/pdf")
-            pdf_file = self.ConsumoService.download_pdf(pdf_path, path_dir)
-
-            return pdf_file
-
-        def include_cod_sap_miro(self, cod_sap, miro):
-
-            miro['referencia_pedido']['numero_pedido'] = cod_sap
-            return miro
-        
-        ## Validar o Form com base no Sefaz
-        def check_guiando_form(self, form_data):
-
-            check_sefaz = self._check_sefaz(form_data)
-            if check_sefaz: self._check_sefaz_form(form_data)
-            document_type = self._check_document_type(form_data['document_type'][0])
-            self._check_fiscal_form(form_data) if document_type == 'nota_fiscal' else self._check_fatura_form(form_data)
-            self._check_required_form(form_data)
-            pass
-
-        def _check_sefaz_form(self, form_data):
-            for sefaz_field in SEFAZ_FIELDS:
-                if sefaz_field not in form_data: raise KeyError(f"ERRO - O campo {sefaz_field} não foi enviado.")
-                if form_data[sefaz_field] is None or form_data[sefaz_field] == "" : raise KeyError(f"ERRO - O campo {sefaz_field} está vazio.")
-            pass
-
-        def _check_fiscal_form(self, form_data):
-            if 'nro_nota_fiscal' not in form_data: raise KeyError(f"ERRO - O Campo {'nro_nota_fiscal'} não foi enviado.")
-            if form_data['nro_nota_fiscal'] is None or form_data['nro_nota_fiscal'] == "": raise KeyError(f"ERRO - O Campo {'nro_nota_fiscal'} está vazio.")
-            pass
-
-        def _check_fatura_form(self, form_data):
-            if 'nro_fatura' not in form_data: raise KeyError(f"ERRO - O Campo {'nro_fatura'} não foi enviado.")
-            if form_data['nro_fatura'] is None or form_data['nro_fatura'] == "": raise KeyError(f"ERRO - O Campo {'nro_fatura'} está vazio.")
-            pass
-
-        def _check_required_form(self, form_data):
-            for field in form_data:
-                if field not in OPTIONAL_FIELDS and field not in SEFAZ_FIELDS:
-                    if form_data[field] is None or form_data[field] == "":raise KeyError(f"ERRO - O Campo {field} está vazio")
+import json
+from os import getcwd, makedirs, path
+from nf_consumo.consumo_service import ConsumoService
+from ..constants import *
+
+class BaseHelper:
+
+    def __init__(self):
+        self.ConsumoService = ConsumoService()
+
+class JsonHelper(BaseHelper):
+
+    def save_json(self, filename, json_data):
+
+        path_dir = path.join(getcwd(), 'output/json')
+        if not path.exists(path_dir):
+            makedirs(path_dir)
+
+        with open(f"./output/json/{filename}.json", "w", encoding="utf-8") as json_file:
+            json.dump( json_data, json_file, ensure_ascii=False, indent=4)
+
+class JiraFieldsHelper(BaseHelper):
+
+    def remove_null_fields(self, fields):
+        fields_data_without_nulls = {}
+
+        for key, value in fields.items():
+            if value is not None:
+                fields_data_without_nulls[key] = value
+
+        return fields_data_without_nulls
+    
+    def _rename_fields(self, fields):
+        fields = self._fields
+        new_fields_data = {}
+
+        for key, value in self._jira_fields.items():
+            if value in fields:
+                if "text" in fields[value]:
+                    new_value = fields[value].get("text")
+                elif "date" in fields[value]:
+                    new_value = fields[value].get("date")
+                elif "value" in fields[value]:
+                    new_value = fields[value].get("value")
+                else:
+                    new_value = fields[value]
+
+                new_fields_data[key] = new_value
+
+        return new_fields_data
+    
+class GuiandoHelper(BaseHelper):
+        
+        def __init__(self):
+            self._check_sefaz = lambda form_data: form_data[POSSUI_CHAVE_ACESSO][0] == "1"
+            self._check_document_type = lambda document_type: 'nota_fiscal' if document_type == "2" else 'fatura'
+            self.ConsumoService = ConsumoService()
+
+        def download_pdf_nexinvoice(self, attachment):
+            path = attachment[ARQUIVOS_DA_FATURA][0]
+            pdf = self._download_pdf(path)
+            return pdf
+
+        def _download_pdf(self, pdf_path):
+            path_dir = path.join(getcwd(), "output/pdf")
+            pdf_file = self.ConsumoService.download_pdf(pdf_path, path_dir)
+
+            return pdf_file
+
+        def include_cod_sap_miro(self, cod_sap, miro):
+
+            miro['referencia_pedido']['numero_pedido'] = cod_sap
+            return miro
+        
+        ## Validar o Form com base no Sefaz
+        def check_guiando_form(self, form_data):
+
+            check_sefaz = self._check_sefaz(form_data)
+            if check_sefaz: self._check_sefaz_form(form_data)
+            document_type = self._check_document_type(form_data['document_type'][0])
+            self._check_fiscal_form(form_data) if document_type == 'nota_fiscal' else self._check_fatura_form(form_data)
+            self._check_required_form(form_data)
+            pass
+
+        def _check_sefaz_form(self, form_data):
+            for sefaz_field in SEFAZ_FIELDS:
+                if sefaz_field not in form_data: raise KeyError(f"ERRO - O campo {sefaz_field} não foi enviado.")
+                if form_data[sefaz_field] is None or form_data[sefaz_field] == "" : raise KeyError(f"ERRO - O campo {sefaz_field} está vazio.")
+            pass
+
+        def _check_fiscal_form(self, form_data):
+            if 'nro_nota_fiscal' not in form_data: raise KeyError(f"ERRO - O Campo {'nro_nota_fiscal'} não foi enviado.")
+            if form_data['nro_nota_fiscal'] is None or form_data['nro_nota_fiscal'] == "": raise KeyError(f"ERRO - O Campo {'nro_nota_fiscal'} está vazio.")
+            pass
+
+        def _check_fatura_form(self, form_data):
+            if 'nro_fatura' not in form_data: raise KeyError(f"ERRO - O Campo {'nro_fatura'} não foi enviado.")
+            if form_data['nro_fatura'] is None or form_data['nro_fatura'] == "": raise KeyError(f"ERRO - O Campo {'nro_fatura'} está vazio.")
+            pass
+
+        def _check_required_form(self, form_data):
+            for field in form_data:
+                if field not in OPTIONAL_FIELDS and field not in SEFAZ_FIELDS:
+                    if form_data[field] is None or form_data[field] == "":raise KeyError(f"ERRO - O Campo {field} está vazio")
             pass
```

### Comparing `hnt_nf_jira_library-0.4.1/nf_jira/entities/classes/issue_fields.py` & `hnt_nf_jira_library-0.4.2/nf_jira/entities/classes/issue_fields.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from .helper import JsonHelper, JiraFieldsHelper
-from ..constants import *
-
-class IssueFields:
-
-    def get_fields_by_form_and_jira(self, form_jira_keys, form_fields, jira_fields, debug=False):
-
-        
-        fields = self._generate_fields(form_jira_keys)
-        fields_from_jira_keys = self._get_issue_fields_data_from_jira_keys(form_jira_keys, jira_fields)
-        JiraFieldsHelper().remove_null_fields(fields_from_jira_keys)
-        JiraFieldsHelper().remove_null_fields(form_fields)
-
-        self._append_jira_fields(fields_from_jira_keys, fields)
-        self._append_form_fields(form_fields, fields)
-
-        JsonHelper().save_json(f'Fields_From_Keys_{ISSUE_KEY}',fields) if debug else None
-        return fields
-
-    def _get_issue_fields_data_from_jira_keys(self, form_jira_keys, jira_fields):
-
-        jira_fields_from_keys = {}
-
-        for field_key in form_jira_keys:
-
-            jira_key = form_jira_keys[field_key]
-    
-            if jira_key is not None:
-                field_value = jira_fields[jira_key]
-                if 'value' in field_value:
-                    field_value = field_value['value']
-            else:
-                field_value = None
-
-            jira_fields_from_keys[field_key] = field_value if field_value else None
-
-        return jira_fields_from_keys
-    
-    def _append_jira_fields(self, jira_fields_from_keys, fields):
-
-        for jira_field in jira_fields_from_keys:
-            fields[jira_field] = jira_fields_from_keys[jira_field]  if jira_fields_from_keys[jira_field] is not None else fields[jira_field]
-
-        pass
-
-    def _append_form_fields(self, form_fields, fields):
-
-        for form_field in form_fields:
-            fields[form_field] = form_fields[form_field] if form_fields[form_field] is not None else fields[form_field]
-
-        pass
-
-    def _generate_fields(self, fields_keys):
-
-        fields = {}
-        for key in fields_keys:
-            fields[key] = None
-
+from .helper import JsonHelper, JiraFieldsHelper
+from ..constants import *
+
+class IssueFields:
+
+    def get_fields_by_form_and_jira(self, form_jira_keys, form_fields, jira_fields, debug=False):
+
+        
+        fields = self._generate_fields(form_jira_keys)
+        fields_from_jira_keys = self._get_issue_fields_data_from_jira_keys(form_jira_keys, jira_fields)
+        JiraFieldsHelper().remove_null_fields(fields_from_jira_keys)
+        JiraFieldsHelper().remove_null_fields(form_fields)
+
+        self._append_jira_fields(fields_from_jira_keys, fields)
+        self._append_form_fields(form_fields, fields)
+
+        JsonHelper().save_json(f'Fields_From_Keys_{ISSUE_KEY}',fields) if debug else None
+        return fields
+
+    def _get_issue_fields_data_from_jira_keys(self, form_jira_keys, jira_fields):
+
+        jira_fields_from_keys = {}
+
+        for field_key in form_jira_keys:
+
+            jira_key = form_jira_keys[field_key]
+    
+            if jira_key is not None:
+                field_value = jira_fields[jira_key]
+                if 'value' in field_value:
+                    field_value = field_value['value']
+            else:
+                field_value = None
+
+            jira_fields_from_keys[field_key] = field_value if field_value else None
+
+        return jira_fields_from_keys
+    
+    def _append_jira_fields(self, jira_fields_from_keys, fields):
+
+        for jira_field in jira_fields_from_keys:
+            fields[jira_field] = jira_fields_from_keys[jira_field]  if jira_fields_from_keys[jira_field] is not None else fields[jira_field]
+
+        pass
+
+    def _append_form_fields(self, form_fields, fields):
+
+        for form_field in form_fields:
+            fields[form_field] = form_fields[form_field] if form_fields[form_field] is not None else fields[form_field]
+
+        pass
+
+    def _generate_fields(self, fields_keys):
+
+        fields = {}
+        for key in fields_keys:
+            fields[key] = None
+
         return fields
```

### Comparing `hnt_nf_jira_library-0.4.1/nf_jira/wrapper_nf_jira.py` & `hnt_nf_jira_library-0.4.2/nf_jira/wrapper_nf_jira.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,358 +1,342 @@
-import json
-import requests
-import os
-from os import getcwd, path
-from datetime import datetime
-from pydantic import ValidationError
-
-from .entities.nota_pedido import NotaPedido
-from .entities.miro import Miro
-from .entities.fatura import Fatura
-from .entities.constants import *
-
-from .entities.classes.form_jira    import FormJira
-from .entities.classes.issue_jira   import IssueJira, AttachmentJira, TransitionJira, CommentJira
-from .entities.classes.issue_fields import IssueFields
-from .entities.classes.helper       import JiraFieldsHelper, JsonHelper, GuiandoHelper
-from .entities.classes.n8n_domain   import N8NDomain
-class wrapper_jira:
-
-    def __init__(self, miro_is_active=False ,debug=False):
-        
-        self._test_mode = debug
-        self._miro_is_active  = miro_is_active
-        self._instance_class()
-
-    def _instance_class(self):
-        self.FormJira         = FormJira()
-        self.IssueJira        = IssueJira()
-        self.AttachmentJira   = AttachmentJira()
-        self.TransitionJira   = TransitionJira()
-        self.CommentJira      = CommentJira()
-        self.JiraFieldsHelper = JiraFieldsHelper()
-        self.GuiandoHelper    = GuiandoHelper()
-        self.JsonHelper       = JsonHelper()
-        self.IssueFields      = IssueFields()
-        self.N8NDomain        = N8NDomain()
-
-    def get_document_by_issue(self, issue_key):
-
-        issue_sap_json = {}
-
-        issue = self._get_issue_by_key(issue_key)
-        issue_transition = issue['domain_data']['fornecedor']['transacao']
-
-        if issue_transition == 'ME21N':
-            nota_pedido_factory = self._issue_factory(issue)
-            nota_pedido_model   = NotaPedido(**nota_pedido_factory).model_dump()
-            issue_sap_json["nota_pedido"] = nota_pedido_model
-
-            if self._miro_is_active:
-                miro_factory = self._miro_factory(issue)
-                miro_model = Miro(**miro_factory).model_dump()
-                issue_sap_json["miro"] = miro_model
-
-        elif issue_transition == 'FV60':
-            fatura_factory = self._fatura_factory(issue)
-            fatura_model   = Fatura(**fatura_factory).model_dump()
-            issue_sap_json["fatura"] = fatura_model
-
-        issue_sap_json["jira_info"] = issue["jira_info"]
-
-        if self._test_mode:
-            for json in issue_sap_json:
-                self.JsonHelper.save_json(f'{json}_{issue_key}', issue_sap_json[json])
-            
-        return issue_sap_json
-
-    def _get_issue_by_key(self, issue_key):
-
-        issue_json = self._get_nf_jira(issue_key)
-
-        issue_attachment = issue_json["attachment"]
-        jira_info = issue_json["jira_info"]
-
-        fornecedor_domain = self.N8NDomain.get_nf_domain(FORNECEDOR_N8N_DOMAIN, issue_attachment[CNPJ_DO_FORNECEDOR])
-        centro_domain = self.N8NDomain.get_nf_domain(CENTRO_N8N_DOMAIN, issue_attachment[CNPJ_DO_CLIENTE])
-
-        domain = {
-            "fornecedor"    : fornecedor_domain,
-            "centro" : centro_domain
-        }
-
-        allocation = self.N8NDomain.get_allocation(
-            issue_attachment[CNPJ_DO_FORNECEDOR],
-            issue_attachment[CNPJ_DO_CLIENTE],
-            issue_attachment[NÚMERO_DO_CONTRATO]
-        )
-
-        pdf_data = self.GuiandoHelper.download_pdf_nexinvoice(issue_attachment)
-
-        issue = {
-            "issue_data": issue_json["issue_data"],
-            "json_data": issue_attachment,
-            "domain_data": domain,
-            "allocation_data": allocation,
-            "pdf_data": pdf_data,
-            "jira_info": jira_info,
-        }
-
-        if self._test_mode:
-            self.JsonHelper.save_json(f'Issue_data_{issue_key}', issue)
-
-        return issue
-
-    def _issue_factory(self, issue: dict):
-
-        sintese_itens = []
-        validTotalPercents = 0.0
-
-        if not issue["allocation_data"]:
-
-            item = {
-                "centro": issue["domain_data"]["centro"]["centro"],
-                "centro_custo": f"{issue['domain_data']['centro']['centro_custo']}",
-                "cod_imposto": "C6",
-                "valor_bruto": str(issue["json_data"][VALOR_TOTAL_DA_FATURA]),
-            }
-
-            sintese_item = {
-                "categoria_cc": "K",
-                "quantidade": 1,
-                "cod_material": issue["domain_data"]["fornecedor"]["codigo_material"],
-                "item": item,
-            }
-
-            sintese_itens.append(sintese_item)
-
-        else:
-
-            for centro_issue in issue["allocation_data"]["centro_custos"]:
-
-                validTotalPercents += float(centro_issue["porcentagem"])
-
-                item = {
-                    "centro": centro_issue["nome"].split("210")[0],
-                    "centro_custo": centro_issue["nome"],
-                    "cod_imposto": "C6",
-                    "valor_bruto": "{:.2f}".format(
-                        issue["json_data"][VALOR_TOTAL_DA_FATURA]
-                        * float(centro_issue["porcentagem"])
-                        / 100,
-                        2,
-                    ),
-                }
-
-                sintese_item = {
-                    "categoria_cc": "K",
-                    "quantidade": 1,
-                    "cod_material": issue["domain_data"]["fornecedor"][
-                        "codigo_material"
-                    ],
-                    "item": item,
-                }
-
-                sintese_itens.append(sintese_item)
-
-            if validTotalPercents != 100.0:
-                raise Exception(f"Invalid total percentage: {validTotalPercents}%")
-
-        anexo = {
-            "path": issue["pdf_data"]["path_dir"],
-            "filename": issue["pdf_data"]["filename"],
-        }
-
-        nota_pedido = {
-            "tipo": "ZCOR",
-            "org_compras": issue["domain_data"]["centro"]["org_compras"],
-            "grp_compradores": issue['json_data']['grupo_compradores'][0],
-            "empresa": "HFNT",
-            "cod_fornecedor": issue["domain_data"]["fornecedor"]["codigo_sap"],
-            "sintese_itens": sintese_itens,
-            "anexo": anexo,
-        }
-
-        return nota_pedido
-
-    def _miro_factory(self, issue: dict):
-
-        texto = self._prepare_ref(issue)
-
-        dados_basicos = {
-            "data_da_fatura": datetime.strptime(
-                issue['json_data'][DATA_DE_EMISSÃO], "%Y-%m-%d"
-            ).strftime("%d.%m.%Y"),
-            "referencia": f"{issue['json_data'][CHAVE_DE_ACESSO_DA_FATURA][25:34]}-{issue['json_data'][CHAVE_DE_ACESSO_DA_FATURA][22:25]}",
-            "montante": str(issue['json_data'][VALOR_TOTAL_DA_FATURA]),
-            "texto": texto,
-        }
-
-        detalhe = {"ctg_nf": issue["domain_data"]["fornecedor"]["categoria_nf"]}
-
-        sintese = {"CFOP": issue["domain_data"]["fornecedor"]["cfop"]}
-
-        chave_acesso = {
-            "tp_emissao":f"{issue['json_data'][CHAVE_DE_ACESSO_DA_FATURA][34]}",
-            "numero_aleatorio": f"{issue['json_data'][CHAVE_DE_ACESSO_DA_FATURA][35:43]}",
-            "dig_verif": f"{issue['json_data'][CHAVE_DE_ACESSO_DA_FATURA][43:]}",
-        }
-
-        nfe_sefaz = {
-            "numero_log": issue['json_data']["numero_log"],
-            "data_procmto": datetime.strptime(issue['json_data']["data_procmto"], "%Y-%m-%d").strftime("%d.%m.%Y"),
-            "hora_procmto": issue['json_data']["hora_procmto"],
-        }
-
-        dados_nfe = {"chave_acesso_sefaz": chave_acesso, "nfe_sefaz": nfe_sefaz}
-
-        miro_model = {
-            "dados_basicos": dados_basicos,
-            "detalhe": detalhe,
-            "sintese": sintese,
-            "dados_nfe": dados_nfe,
-        }
-
-        return miro_model
-    
-    def _fatura_factory(self, issue): 
-
-        texto = self._prepare_ref(issue)
-
-        item = {
-            "Cta_razao": issue['domain_data']['fornecedor']['razao'], #Conta Contabil SAP
-            "Montante":  str(issue['json_data'][VALOR_TOTAL_DA_FATURA]),
-            "loc_negocios": issue['domain_data']['centro']['centro'],
-            "atribuicao": datetime.strptime(issue['json_data'][DATA_DE_EMISSÃO], "%Y-%m-%d").strftime("%Y%m%d"),
-            "texto": texto,
-            "centro_custo":  f"{issue['domain_data']['centro']['centro']}210"
-        }
-
-        itens = [item]
-
-        dados_basicos = {
-            "cod_fornecedor": issue['domain_data']['fornecedor']['codigo_sap'], #ID_EXTERNO_SAP
-            "data_fatura": datetime.strptime(issue['json_data'][DATA_DE_EMISSÃO], "%Y-%m-%d").strftime("%d.%m.%Y"),
-            "referencia": issue['json_data'][NÚMERO_DA_FATURA_DO_FORNECEDOR],
-            "montante": str(issue['json_data'][VALOR_TOTAL_DA_FATURA]),
-            "bus_pl_sec_cd": itens[0]["loc_negocios"],
-            "texto": texto,
-            "itens": itens
-        }
-
-        pagamento = {
-            "data_basica": datetime.now().strftime("%d.%m.%Y"),
-            "cond_pgto": "0000" #CONSTANTE 
-        }
-
-        fatura_model = {
-            "dados_basicos": dados_basicos,
-            "pagamento":pagamento,
-        }
-
-        return fatura_model
-
-    def _get_nf_jira(self, issue_id):
-        try:
-
-            issue_data = self.IssueJira.get_issue(issue_id)
-            complement_form = self._get_issue_fields_by_keys( issue_id, FORM_TEMPLATE_COMPLEMENTO )
-            self.GuiandoHelper.check_guiando_form(complement_form)
-
-            issue_data["fields"] = self.JiraFieldsHelper.remove_null_fields(issue_data.get("fields"))
-            attachment = self.AttachmentJira.get_attachment(issue_data)
-
-            nf_type_id = complement_form["tipo_conta"]
-
-            if nf_type_id == "ÁGUA":
-                nf_type = COMPLEMENTO_DE_ÁGUA
-
-            elif nf_type_id == "ENERGIA":
-                nf_type = COMPLEMENTO_DE_ENERGIA
-
-            elif nf_type_id == "GÁS":
-                nf_type = COMPLEMENTO_DE_GÁS
-
-            else:
-                if attachment[COMPLEMENTO_DE_ÁGUA] is not None:
-                    nf_type = COMPLEMENTO_DE_ÁGUA
-                elif attachment[COMPLEMENTO_DE_ENERGIA] is not None:
-                    nf_type = COMPLEMENTO_DE_ENERGIA
-                elif attachment[COMPLEMENTO_DE_GÁS] is not None:
-                    nf_type = COMPLEMENTO_DE_GÁS
-
-            attachment[CNPJ_DO_FORNECEDOR] = complement_form['cnpj_fornecedor']
-            attachment[RAZÃO_SOCIAL_DO_FORNECEDOR] = complement_form['razao_social_fornecedor']
-
-            attachment[CNPJ_DO_CLIENTE] = complement_form['cnpj_destinatario']
-            attachment[NÚMERO_DA_FATURA] = complement_form['nro_nota_fiscal']
-            attachment[NÚMERO_DA_FATURA_DO_FORNECEDOR] = complement_form['nro_fatura']
-            attachment[DATA_DE_EMISSÃO] = complement_form['data_emissao']
-            attachment[DATA_DE_VENCIMENTO] = complement_form['data_vencimento']
-            attachment[CHAVE_DE_ACESSO_DA_FATURA] = complement_form['chave_acesso']
-            attachment[DATA_DE_REFERÊNCIA] = complement_form['periodo_referencia']
-            attachment["numero_log"] = complement_form['protocolo_autorizacao']
-            attachment["data_procmto"] = complement_form['data_autorizacao']
-            attachment["hora_procmto"] = complement_form['hora_autorizacao']
-            attachment[nf_type] = {
-                "DataLeituraAnterior" : complement_form['data_leitura_anterior'],
-                "DataLeituraAtual"    : complement_form['data_leitura_atual']
-            }
-            # attachment[nf_type]["DataLeituraAnterior"] = complement_form['data_leitura_anterior']
-            # attachment[nf_type]["DataLeituraAtual"] = complement_form['data_leitura_atual']
-            attachment["grupo_compradores"] = complement_form['grupo_compradores']
-
-            #Validação de Valor Liquido da Fatura
-            if complement_form['valor_liquido'] != "" and complement_form['valor_liquido'] != None:
-                attachment[VALOR_TOTAL_DA_FATURA] = complement_form['valor_liquido']
-            elif complement_form['valor_nota'] != None and complement_form['valor_nota'] != "":
-                attachment[VALOR_TOTAL_DA_FATURA] = complement_form['valor_nota']
-            else:
-                attachment[VALOR_TOTAL_DA_FATURA] = attachment.get(
-                    VALOR_TOTAL_DA_FATURA
-                )
-
-            automation_form_id = self.FormJira.get_form_id(issue_id, FORM_TEMPLATE_AUTOMACAO)
-
-            jira_info = {"issue_id": issue_id, "form_id": automation_form_id}
-
-            nf_jira_json = {
-                "issue_data": issue_data,
-                "attachment": attachment,
-                "jira_info": jira_info,
-            }
-
-            return nf_jira_json
-
-        except requests.exceptions.HTTPError as e:
-            raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
-
-        except Exception as e:
-            raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
-
-    def _prepare_ref(self, issue):
-
-        data_ref = datetime.strptime(issue['json_data'][DATA_DE_REFERÊNCIA], "%m/%Y").strftime("%b/%y").upper()
-
-        if issue['json_data'][COMPLEMENTO_DE_ÁGUA] is not None:
-            
-            leitura_anterior = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataLeituraAnterior'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataLeituraAnterior'] is not None else None
-            leitura_atual = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataLeituraAtual'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataLeituraAtual'] is not None else None
-        elif issue['json_data'][COMPLEMENTO_DE_ENERGIA] is not None:
-            leitura_anterior = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAnterior'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAnterior'] is not None else None
-            leitura_atual = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAtual'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAtual'] is not None else None
-        elif issue['json_data'][COMPLEMENTO_DE_GÁS] is not None:
-            leitura_anterior = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAnterior'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAnterior'] is not None else None
-            leitura_atual = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAtual'], "%Y-%m-%d").strftime("%b/%y").upper()  if issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAtual'] is not None else None
-
-        extra_ref = f"PERIODO: {leitura_anterior} A {leitura_atual}" if leitura_anterior is not None and leitura_atual is not None else None
-
-        return f"REF: {data_ref} {extra_ref}"
-
-    def _get_issue_fields_by_keys(self, issue_key, form_template):
-
-        form_jira_keys = self.FormJira.get_form_jira_keys(issue_key, form_template)
-        form_fields    = self.FormJira.get_form_fields(issue_key, form_template)
-        jira_fields    = self.IssueJira.get_issue_fields_data(issue_key)
-        fields_by_jira_and_form = self.IssueFields.get_fields_by_form_and_jira(form_jira_keys, form_fields, jira_fields)
-
+import json
+import requests
+import os
+import locale
+from os import getcwd, path
+from datetime import datetime
+from pydantic import ValidationError
+
+from .entities.nota_pedido import NotaPedido
+from .entities.miro import Miro
+from .entities.fatura import Fatura
+from .entities.constants import *
+
+from .entities.classes.form_jira    import FormJira
+from .entities.classes.issue_jira   import IssueJira, AttachmentJira, TransitionJira, CommentJira
+from .entities.classes.issue_fields import IssueFields
+from .entities.classes.helper       import JiraFieldsHelper, JsonHelper, GuiandoHelper
+from .entities.classes.n8n_domain   import N8NDomain
+class wrapper_jira:
+
+    def __init__(self, miro_is_active=False ,debug=False):
+        
+        self._test_mode = debug
+        self._miro_is_active  = miro_is_active
+        self._instance_class()
+        locale.setlocale(locale.LC_ALL, ('pt_BR.UTF-8'))
+
+    def _instance_class(self):
+        self.FormJira         = FormJira()
+        self.IssueJira        = IssueJira()
+        self.AttachmentJira   = AttachmentJira()
+        self.TransitionJira   = TransitionJira()
+        self.CommentJira      = CommentJira()
+        self.JiraFieldsHelper = JiraFieldsHelper()
+        self.GuiandoHelper    = GuiandoHelper()
+        self.JsonHelper       = JsonHelper()
+        self.IssueFields      = IssueFields()
+        self.N8NDomain        = N8NDomain()
+
+    def get_document_by_issue(self, issue_key):
+
+        issue_sap_json = {}
+
+        issue = self._get_issue_by_key(issue_key)
+        issue_transition = issue['domain_data']['fornecedor']['transacao']
+
+        if issue_transition == 'ME21N':
+            nota_pedido_factory = self._issue_factory(issue)
+            nota_pedido_model   = NotaPedido(**nota_pedido_factory).model_dump()
+            issue_sap_json["nota_pedido"] = nota_pedido_model
+
+            if self._miro_is_active:
+                miro_factory = self._miro_factory(issue)
+                miro_model = Miro(**miro_factory).model_dump()
+                issue_sap_json["miro"] = miro_model
+
+        elif issue_transition == 'FV60':
+            fatura_factory = self._fatura_factory(issue)
+            fatura_model   = Fatura(**fatura_factory).model_dump()
+            issue_sap_json["fatura"] = fatura_model
+
+        issue_sap_json["jira_info"] = issue["jira_info"]
+
+        if self._test_mode:
+            for json in issue_sap_json:
+                self.JsonHelper.save_json(f'{json}_{issue_key}', issue_sap_json[json])
+            
+        return issue_sap_json
+
+    def _get_issue_by_key(self, issue_key):
+
+        issue_json = self._get_nf_jira(issue_key)
+
+        issue_attachment = issue_json["attachment"]
+        jira_info = issue_json["jira_info"]
+
+        fornecedor_domain = self.N8NDomain.get_nf_domain(FORNECEDOR_N8N_DOMAIN, issue_attachment[CNPJ_DO_FORNECEDOR])
+        centro_domain = self.N8NDomain.get_nf_domain(CENTRO_N8N_DOMAIN, issue_attachment[CNPJ_DO_CLIENTE])
+
+        domain = {
+            "fornecedor"    : fornecedor_domain,
+            "centro" : centro_domain
+        }
+
+        pdf_data = self.GuiandoHelper.download_pdf_nexinvoice(issue_attachment)
+
+        issue = {
+            "issue_data": issue_json["issue_data"],
+            "json_data": issue_attachment,
+            "domain_data": domain,
+            "pdf_data": pdf_data,
+            "jira_info": jira_info,
+        }
+
+        if self._test_mode:
+            self.JsonHelper.save_json(f'Issue_data_{issue_key}', issue)
+
+        return issue
+
+    def _issue_factory(self, issue: dict):
+
+        sintese_itens = []
+
+        if not issue['json_data'][ALOCAÇÕES_DE_CUSTO]:
+
+            item = {
+                "centro": issue["domain_data"]["centro"]["centro"],
+                "centro_custo": f"{issue['domain_data']['centro']['centro_custo']}",
+                "cod_imposto": "C6",
+                "valor_bruto": str(issue["json_data"][VALOR_TOTAL_DA_FATURA]),
+            }
+
+            sintese_item = {
+                "categoria_cc": "K",
+                "quantidade": 1,
+                "cod_material": issue["domain_data"]["fornecedor"]["codigo_material"],
+                "item": item,
+            }
+
+            sintese_itens.append(sintese_item)
+
+        else:
+
+            for cost_allocation in issue['json_data'][ALOCAÇÕES_DE_CUSTO]:
+                
+                item = {
+                    "centro": cost_allocation['CustCenterDescription'].split(' - ')[0],
+                    "centro_custo": cost_allocation['Code'],
+                    "cod_imposto": "C6",
+                    "valor_bruto": locale.format_string("%.2f", cost_allocation['CustCenterTotalAmount']),
+                }
+
+                sintese_item = {
+                    "categoria_cc": "K",
+                    "quantidade": 1,
+                    "cod_material": issue["domain_data"]["fornecedor"][
+                        "codigo_material"
+                    ],
+                    "item": item,
+                }
+
+                sintese_itens.append(sintese_item)
+
+        anexo = {
+            "path": issue["pdf_data"]["path_dir"],
+            "filename": issue["pdf_data"]["filename"],
+        }
+
+        nota_pedido = {
+            "tipo": "ZCOR",
+            "org_compras": issue["domain_data"]["centro"]["org_compras"],
+            "grp_compradores": issue['json_data']['grupo_compradores'][0],
+            "empresa": "HFNT",
+            "cod_fornecedor": issue["domain_data"]["fornecedor"]["codigo_sap"],
+            "sintese_itens": sintese_itens,
+            "anexo": anexo,
+        }
+
+        return nota_pedido
+
+    def _miro_factory(self, issue: dict):
+
+        texto = self._prepare_ref(issue)
+
+        dados_basicos = {
+            "data_da_fatura": datetime.strptime(
+                issue['json_data'][DATA_DE_EMISSÃO], "%Y-%m-%d"
+            ).strftime("%d.%m.%Y"),
+            "referencia": f"{issue['json_data'][CHAVE_DE_ACESSO_DA_FATURA][25:34]}-{issue['json_data'][CHAVE_DE_ACESSO_DA_FATURA][22:25]}",
+            "montante": str(issue['json_data'][VALOR_TOTAL_DA_FATURA]),
+            "texto": texto,
+        }
+
+        detalhe = {"ctg_nf": issue["domain_data"]["fornecedor"]["categoria_nf"]}
+
+        sintese = {"CFOP": issue["domain_data"]["fornecedor"]["cfop"]}
+
+        chave_acesso = {
+            "tp_emissao":f"{issue['json_data'][CHAVE_DE_ACESSO_DA_FATURA][34]}",
+            "numero_aleatorio": f"{issue['json_data'][CHAVE_DE_ACESSO_DA_FATURA][35:43]}",
+            "dig_verif": f"{issue['json_data'][CHAVE_DE_ACESSO_DA_FATURA][43:]}",
+        }
+
+        nfe_sefaz = {
+            "numero_log": issue['json_data']["numero_log"],
+            "data_procmto": datetime.strptime(issue['json_data']["data_procmto"], "%Y-%m-%d").strftime("%d.%m.%Y"),
+            "hora_procmto": issue['json_data']["hora_procmto"],
+        }
+
+        dados_nfe = {"chave_acesso_sefaz": chave_acesso, "nfe_sefaz": nfe_sefaz}
+
+        miro_model = {
+            "dados_basicos": dados_basicos,
+            "detalhe": detalhe,
+            "sintese": sintese,
+            "dados_nfe": dados_nfe,
+        }
+
+        return miro_model
+    
+    def _fatura_factory(self, issue): 
+
+        texto = self._prepare_ref(issue)
+
+        item = {
+            "Cta_razao": issue['domain_data']['fornecedor']['razao'], #Conta Contabil SAP
+            "Montante":  str(issue['json_data'][VALOR_TOTAL_DA_FATURA]),
+            "loc_negocios": issue['domain_data']['centro']['centro'],
+            "atribuicao": datetime.strptime(issue['json_data'][DATA_DE_EMISSÃO], "%Y-%m-%d").strftime("%Y%m%d"),
+            "texto": texto,
+            "centro_custo":  f"{issue['domain_data']['centro']['centro']}210"
+        }
+
+        itens = [item]
+
+        dados_basicos = {
+            "cod_fornecedor": issue['domain_data']['fornecedor']['codigo_sap'], #ID_EXTERNO_SAP
+            "data_fatura": datetime.strptime(issue['json_data'][DATA_DE_EMISSÃO], "%Y-%m-%d").strftime("%d.%m.%Y"),
+            "referencia": issue['json_data'][NÚMERO_DA_FATURA_DO_FORNECEDOR],
+            "montante": str(issue['json_data'][VALOR_TOTAL_DA_FATURA]),
+            "bus_pl_sec_cd": itens[0]["loc_negocios"],
+            "texto": texto,
+            "itens": itens
+        }
+
+        pagamento = {
+            "data_basica": datetime.now().strftime("%d.%m.%Y"),
+            "cond_pgto": "0000" #CONSTANTE 
+        }
+
+        fatura_model = {
+            "dados_basicos": dados_basicos,
+            "pagamento":pagamento,
+        }
+
+        return fatura_model
+
+    def _get_nf_jira(self, issue_id):
+        try:
+
+            issue_data = self.IssueJira.get_issue(issue_id)
+            complement_form = self._get_issue_fields_by_keys( issue_id, FORM_TEMPLATE_COMPLEMENTO )
+            self.GuiandoHelper.check_guiando_form(complement_form)
+
+            issue_data["fields"] = self.JiraFieldsHelper.remove_null_fields(issue_data.get("fields"))
+            attachment = self.AttachmentJira.get_attachment(issue_data)
+
+            nf_type_id = complement_form["tipo_conta"]
+
+            if nf_type_id == "ÁGUA":
+                nf_type = COMPLEMENTO_DE_ÁGUA
+
+            elif nf_type_id == "ENERGIA":
+                nf_type = COMPLEMENTO_DE_ENERGIA
+
+            elif nf_type_id == "GÁS":
+                nf_type = COMPLEMENTO_DE_GÁS
+
+            else:
+                if attachment[COMPLEMENTO_DE_ÁGUA] is not None:
+                    nf_type = COMPLEMENTO_DE_ÁGUA
+                elif attachment[COMPLEMENTO_DE_ENERGIA] is not None:
+                    nf_type = COMPLEMENTO_DE_ENERGIA
+                elif attachment[COMPLEMENTO_DE_GÁS] is not None:
+                    nf_type = COMPLEMENTO_DE_GÁS
+
+            attachment[CNPJ_DO_FORNECEDOR] = complement_form['cnpj_fornecedor']
+            attachment[RAZÃO_SOCIAL_DO_FORNECEDOR] = complement_form['razao_social_fornecedor']
+
+            attachment[CNPJ_DO_CLIENTE] = complement_form['cnpj_destinatario']
+            attachment[NÚMERO_DA_FATURA] = complement_form['nro_nota_fiscal']
+            attachment[NÚMERO_DA_FATURA_DO_FORNECEDOR] = complement_form['nro_fatura']
+            attachment[DATA_DE_EMISSÃO] = complement_form['data_emissao']
+            attachment[DATA_DE_VENCIMENTO] = complement_form['data_vencimento']
+            attachment[CHAVE_DE_ACESSO_DA_FATURA] = complement_form['chave_acesso']
+            attachment[DATA_DE_REFERÊNCIA] = complement_form['periodo_referencia']
+            attachment["numero_log"] = complement_form['protocolo_autorizacao']
+            attachment["data_procmto"] = complement_form['data_autorizacao']
+            attachment["hora_procmto"] = complement_form['hora_autorizacao']
+            attachment[nf_type] = {
+                "DataLeituraAnterior" : complement_form['data_leitura_anterior'],
+                "DataLeituraAtual"    : complement_form['data_leitura_atual']
+            }
+            # attachment[nf_type]["DataLeituraAnterior"] = complement_form['data_leitura_anterior']
+            # attachment[nf_type]["DataLeituraAtual"] = complement_form['data_leitura_atual']
+            attachment["grupo_compradores"] = complement_form['grupo_compradores']
+
+            #Validação de Valor Liquido da Fatura
+            if complement_form['valor_liquido'] != "" and complement_form['valor_liquido'] != None:
+                attachment[VALOR_TOTAL_DA_FATURA] = complement_form['valor_liquido']
+            elif complement_form['valor_nota'] != None and complement_form['valor_nota'] != "":
+                attachment[VALOR_TOTAL_DA_FATURA] = complement_form['valor_nota']
+            else:
+                attachment[VALOR_TOTAL_DA_FATURA] = attachment.get(
+                    VALOR_TOTAL_DA_FATURA
+                )
+
+            automation_form_id = self.FormJira.get_form_id(issue_id, FORM_TEMPLATE_AUTOMACAO)
+
+            jira_info = {"issue_id": issue_id, "form_id": automation_form_id}
+
+            nf_jira_json = {
+                "issue_data": issue_data,
+                "attachment": attachment,
+                "jira_info": jira_info,
+            }
+
+            return nf_jira_json
+
+        except requests.exceptions.HTTPError as e:
+            raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
+
+        except Exception as e:
+            raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
+
+    def _prepare_ref(self, issue):
+
+        data_ref = datetime.strptime(issue['json_data'][DATA_DE_REFERÊNCIA], "%m/%Y").strftime("%b/%y").upper()
+
+        if issue['json_data'][COMPLEMENTO_DE_ÁGUA] is not None:
+            
+            leitura_anterior = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataLeituraAnterior'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataLeituraAnterior'] is not None else None
+            leitura_atual = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataLeituraAtual'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataLeituraAtual'] is not None else None
+        elif issue['json_data'][COMPLEMENTO_DE_ENERGIA] is not None:
+            leitura_anterior = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAnterior'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAnterior'] is not None else None
+            leitura_atual = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAtual'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAtual'] is not None else None
+        elif issue['json_data'][COMPLEMENTO_DE_GÁS] is not None:
+            leitura_anterior = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAnterior'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAnterior'] is not None else None
+            leitura_atual = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAtual'], "%Y-%m-%d").strftime("%b/%y").upper()  if issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAtual'] is not None else None
+
+        extra_ref = f"PERIODO: {leitura_anterior} A {leitura_atual}" if leitura_anterior is not None and leitura_atual is not None else None
+
+        return f"REF: {data_ref} {extra_ref}"
+
+    def _get_issue_fields_by_keys(self, issue_key, form_template):
+
+        form_jira_keys = self.FormJira.get_form_jira_keys(issue_key, form_template)
+        form_fields    = self.FormJira.get_form_fields(issue_key, form_template)
+        jira_fields    = self.IssueJira.get_issue_fields_data(issue_key)
+        fields_by_jira_and_form = self.IssueFields.get_fields_by_form_and_jira(form_jira_keys, form_fields, jira_fields)
+
         return fields_by_jira_and_form
```

