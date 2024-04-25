# Comparing `tmp/monit-agd-1.3.0.tar.gz` & `tmp/monit-agd-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monit-agd-1.3.0.tar", last modified: Mon Apr 22 23:31:20 2024, max compression
+gzip compressed data, was "monit-agd-1.3.1.tar", last modified: Thu Apr 25 17:27:35 2024, max compression
```

## Comparing `monit-agd-1.3.0.tar` & `monit-agd-1.3.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 23:31:20.809165 monit-agd-1.3.0/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 monit-agd-1.3.0/LICENSE
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1806 2024-04-22 23:31:20.809165 monit-agd-1.3.0/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1169 2024-04-22 23:27:01.000000 monit-agd-1.3.0/README.md
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 23:31:20.805831 monit-agd-1.3.0/monit/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 monit-agd-1.3.0/monit/__init__.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      734 2024-04-22 22:32:32.000000 monit-agd-1.3.0/monit/config.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1434 2024-04-22 17:50:32.000000 monit-agd-1.3.0/monit/core.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1334 2024-04-22 17:43:41.000000 monit-agd-1.3.0/monit/database.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      158 2024-04-22 01:06:10.000000 monit-agd-1.3.0/monit/error.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     3145 2024-04-22 21:01:19.000000 monit-agd-1.3.0/monit/func.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1831 2024-04-22 23:15:08.000000 monit-agd-1.3.0/monit/log2file.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2569 2024-04-22 23:04:24.000000 monit-agd-1.3.0/monit/logger.py
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 23:31:20.809165 monit-agd-1.3.0/monit_agd.egg-info/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1806 2024-04-22 23:31:20.000000 monit-agd-1.3.0/monit_agd.egg-info/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      319 2024-04-22 23:31:20.000000 monit-agd-1.3.0/monit_agd.egg-info/SOURCES.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-04-22 23:31:20.000000 monit-agd-1.3.0/monit_agd.egg-info/dependency_links.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-04-22 23:31:20.000000 monit-agd-1.3.0/monit_agd.egg-info/requires.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-04-22 23:31:20.000000 monit-agd-1.3.0/monit_agd.egg-info/top_level.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-04-22 23:31:20.809165 monit-agd-1.3.0/setup.cfg
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      867 2024-04-22 23:30:24.000000 monit-agd-1.3.0/setup.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-25 17:27:35.271824 monit-agd-1.3.1/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 monit-agd-1.3.1/LICENSE
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2235 2024-04-25 17:27:35.268491 monit-agd-1.3.1/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1598 2024-04-25 17:01:33.000000 monit-agd-1.3.1/README.md
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-25 17:27:35.268491 monit-agd-1.3.1/monit/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 monit-agd-1.3.1/monit/__init__.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      799 2024-04-25 16:26:23.000000 monit-agd-1.3.1/monit/config.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      860 2024-04-25 17:07:54.000000 monit-agd-1.3.1/monit/core.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1592 2024-04-25 16:30:27.000000 monit-agd-1.3.1/monit/database.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      158 2024-04-22 01:06:10.000000 monit-agd-1.3.1/monit/error.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     3145 2024-04-22 21:01:19.000000 monit-agd-1.3.1/monit/func.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1831 2024-04-22 23:15:08.000000 monit-agd-1.3.1/monit/log2file.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2569 2024-04-22 23:04:24.000000 monit-agd-1.3.1/monit/logger.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      254 2024-04-25 16:25:13.000000 monit-agd-1.3.1/monit/verify_env.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-25 17:27:35.268491 monit-agd-1.3.1/monit_agd.egg-info/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2235 2024-04-25 17:27:35.000000 monit-agd-1.3.1/monit_agd.egg-info/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      339 2024-04-25 17:27:35.000000 monit-agd-1.3.1/monit_agd.egg-info/SOURCES.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-04-25 17:27:35.000000 monit-agd-1.3.1/monit_agd.egg-info/dependency_links.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-04-25 17:27:35.000000 monit-agd-1.3.1/monit_agd.egg-info/requires.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-04-25 17:27:35.000000 monit-agd-1.3.1/monit_agd.egg-info/top_level.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-04-25 17:27:35.271824 monit-agd-1.3.1/setup.cfg
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      867 2024-04-25 17:27:24.000000 monit-agd-1.3.1/setup.py
```

### Comparing `monit-agd-1.3.0/LICENSE` & `monit-agd-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.0/PKG-INFO` & `monit-agd-1.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monit-agd
-Version: 1.3.0
+Version: 1.3.1
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -41,14 +41,38 @@
 
 # Email info
 # Deixe em branco para desativar o envio de e-mails
 EMAIL=
 EMAIL_PASSWORD=
 ```
 **Exemplo de Uso:**
+
+Maneira mais simples de usar o Monit
+```python
+import time
+
+from monit.core import Monitor as monit
+from monit.error import SetupError
+
+def main():
+
+    try:
+        time.sleep(5)
+        raise ValueError("This is a sample error.")
+
+    except Exception as e:
+        print("Erro: Ocorreu um erro inesperado.")
+        monit.notify_and_exit(SetupError, e)
+
+
+if __name__ == "__main__":
+    main()
+```
+
+Registrar múltiplos erros
 ```Python
 # sample.py
 import time
 
 from monit.core import Monitor
 from monit.error import SetupError
 # from monit.logger import Logger
```

### Comparing `monit-agd-1.3.0/README.md` & `monit-agd-1.3.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -22,14 +22,38 @@
 
 # Email info
 # Deixe em branco para desativar o envio de e-mails
 EMAIL=
 EMAIL_PASSWORD=
 ```
 **Exemplo de Uso:**
+
+Maneira mais simples de usar o Monit
+```python
+import time
+
+from monit.core import Monitor as monit
+from monit.error import SetupError
+
+def main():
+
+    try:
+        time.sleep(5)
+        raise ValueError("This is a sample error.")
+
+    except Exception as e:
+        print("Erro: Ocorreu um erro inesperado.")
+        monit.notify_and_exit(SetupError, e)
+
+
+if __name__ == "__main__":
+    main()
+```
+
+Registrar múltiplos erros
 ```Python
 # sample.py
 import time
 
 from monit.core import Monitor
 from monit.error import SetupError
 # from monit.logger import Logger
```

### Comparing `monit-agd-1.3.0/monit/config.py` & `monit-agd-1.3.1/monit/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 # Database info
 user = os.getenv('DB_USER')
 password = os.getenv('DB_PASSWORD')
 host = os.getenv('DB_HOST')
 database = os.getenv('DB_DATABASE')
 
+db_url = f'mysql+pymysql://{user}:{password}@{host}/{database}'
+
 # Email info
 email = os.getenv('EMAIL')
 email_password = os.getenv('EMAIL_PASSWORD')
 
 if not project or not company or not location or not dev:
     raise Exception("Por favor, as informações do código não podem ficar em branco.")
```

### Comparing `monit-agd-1.3.0/monit/func.py` & `monit-agd-1.3.1/monit/func.py`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.0/monit/log2file.py` & `monit-agd-1.3.1/monit/log2file.py`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.0/monit/logger.py` & `monit-agd-1.3.1/monit/logger.py`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.0/monit_agd.egg-info/PKG-INFO` & `monit-agd-1.3.1/monit_agd.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monit-agd
-Version: 1.3.0
+Version: 1.3.1
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -41,14 +41,38 @@
 
 # Email info
 # Deixe em branco para desativar o envio de e-mails
 EMAIL=
 EMAIL_PASSWORD=
 ```
 **Exemplo de Uso:**
+
+Maneira mais simples de usar o Monit
+```python
+import time
+
+from monit.core import Monitor as monit
+from monit.error import SetupError
+
+def main():
+
+    try:
+        time.sleep(5)
+        raise ValueError("This is a sample error.")
+
+    except Exception as e:
+        print("Erro: Ocorreu um erro inesperado.")
+        monit.notify_and_exit(SetupError, e)
+
+
+if __name__ == "__main__":
+    main()
+```
+
+Registrar múltiplos erros
 ```Python
 # sample.py
 import time
 
 from monit.core import Monitor
 from monit.error import SetupError
 # from monit.logger import Logger
```

### Comparing `monit-agd-1.3.0/setup.py` & `monit-agd-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import pathlib
 
 setup(
     name='monit-agd',
-    version='1.3.0',
+    version='1.3.1',
     description='Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     author='arktnld',
     author_email='arktnld@gmail.com',
     url='https://github.com/arktnld/monit',
     license='MIT',
```

