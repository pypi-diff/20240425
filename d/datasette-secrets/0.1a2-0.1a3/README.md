# Comparing `tmp/datasette_secrets-0.1a2.tar.gz` & `tmp/datasette_secrets-0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette_secrets-0.1a2.tar", last modified: Wed Apr 24 22:20:58 2024, max compression
+gzip compressed data, was "datasette_secrets-0.1a3.tar", last modified: Wed Apr 24 23:30:56 2024, max compression
```

## Comparing `datasette_secrets-0.1a2.tar` & `datasette_secrets-0.1a3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:20:58.792120 datasette_secrets-0.1a2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 22:20:52.000000 datasette_secrets-0.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-24 22:20:58.792120 datasette_secrets-0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-24 22:20:52.000000 datasette_secrets-0.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:20:58.788120 datasette_secrets-0.1a2/datasette_secrets/
--rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-04-24 22:20:52.000000 datasette_secrets-0.1a2/datasette_secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-24 22:20:52.000000 datasette_secrets-0.1a2/datasette_secrets/hookspecs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:20:58.792120 datasette_secrets-0.1a2/datasette_secrets/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-24 22:20:52.000000 datasette_secrets-0.1a2/datasette_secrets/templates/secrets_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-24 22:20:52.000000 datasette_secrets-0.1a2/datasette_secrets/templates/secrets_update.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:20:58.792120 datasette_secrets-0.1a2/datasette_secrets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-24 22:20:58.000000 datasette_secrets-0.1a2/datasette_secrets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-24 22:20:58.000000 datasette_secrets-0.1a2/datasette_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 22:20:58.000000 datasette_secrets-0.1a2/datasette_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 22:20:58.000000 datasette_secrets-0.1a2/datasette_secrets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-24 22:20:58.000000 datasette_secrets-0.1a2/datasette_secrets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 22:20:58.000000 datasette_secrets-0.1a2/datasette_secrets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-24 22:20:52.000000 datasette_secrets-0.1a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 22:20:58.792120 datasette_secrets-0.1a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:20:58.792120 datasette_secrets-0.1a2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-04-24 22:20:52.000000 datasette_secrets-0.1a2/tests/test_secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:30:56.783430 datasette_secrets-0.1a3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 23:30:49.000000 datasette_secrets-0.1a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-24 23:30:56.783430 datasette_secrets-0.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-24 23:30:49.000000 datasette_secrets-0.1a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:30:56.779430 datasette_secrets-0.1a3/datasette_secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)    10508 2024-04-24 23:30:49.000000 datasette_secrets-0.1a3/datasette_secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-24 23:30:49.000000 datasette_secrets-0.1a3/datasette_secrets/hookspecs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:30:56.783430 datasette_secrets-0.1a3/datasette_secrets/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-24 23:30:49.000000 datasette_secrets-0.1a3/datasette_secrets/templates/secrets_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-24 23:30:49.000000 datasette_secrets-0.1a3/datasette_secrets/templates/secrets_update.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:30:56.783430 datasette_secrets-0.1a3/datasette_secrets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-24 23:30:56.000000 datasette_secrets-0.1a3/datasette_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-24 23:30:56.000000 datasette_secrets-0.1a3/datasette_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 23:30:56.000000 datasette_secrets-0.1a3/datasette_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 23:30:56.000000 datasette_secrets-0.1a3/datasette_secrets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-24 23:30:56.000000 datasette_secrets-0.1a3/datasette_secrets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 23:30:56.000000 datasette_secrets-0.1a3/datasette_secrets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-24 23:30:49.000000 datasette_secrets-0.1a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 23:30:56.783430 datasette_secrets-0.1a3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:30:56.783430 datasette_secrets-0.1a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-04-24 23:30:49.000000 datasette_secrets-0.1a3/tests/test_secrets.py
```

### Comparing `datasette_secrets-0.1a2/LICENSE` & `datasette_secrets-0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette_secrets-0.1a2/PKG-INFO` & `datasette_secrets-0.1a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-secrets
-Version: 0.1a2
+Version: 0.1a3
 Summary: Manage secrets such as API keys for use with other Datasette plugins
 Author: Datasette
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-secrets
 Project-URL: Changelog, https://github.com/datasette/datasette-secrets/releases
 Project-URL: Issues, https://github.com/datasette/datasette-secrets/issues
 Project-URL: CI, https://github.com/datasette/datasette-secrets/actions
```

### Comparing `datasette_secrets-0.1a2/README.md` & `datasette_secrets-0.1a3/README.md`

 * *Files identical despite different names*

### Comparing `datasette_secrets-0.1a2/datasette_secrets/__init__.py` & `datasette_secrets-0.1a3/datasette_secrets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import click
 from cryptography.fernet import Fernet
 import dataclasses
 from datasette import hookimpl, Forbidden, Permission, Response
 from datasette.plugins import pm
-from datasette.utils import await_me_maybe
+from datasette.utils import await_me_maybe, sqlite3
 import os
 from typing import Optional
 from . import hookspecs
 
 MAX_NOTE_LENGTH = 100
 
 pm.add_hookspecs(hookspecs)
@@ -20,20 +20,23 @@
     # Is it an environment secret?
     env_var = "DATASETTE_SECRETS_{}".format(secret_name)
     if os.environ.get(env_var):
         return os.environ[env_var]
     # Now look it up in the database
     config = get_config(datasette)
     db = get_database(datasette)
-    db_secret = (
-        await db.execute(
-            "select id, encrypted from datasette_secrets where name = ? order by version desc limit 1",
-            (secret_name,),
-        )
-    ).first()
+    try:
+        db_secret = (
+            await db.execute(
+                "select id, encrypted from datasette_secrets where name = ? order by version desc limit 1",
+                (secret_name,),
+            )
+        ).first()
+    except sqlite3.OperationalError:
+        return None
     if not db_secret:
         return None
     key = Fernet(config["encryption_key"].encode("utf-8"))
     decrypted = key.decrypt(db_secret["encrypted"])
     # Update the last used timestamp and actor_id
     params = (actor_id, db_secret["id"])
     if not actor_id:
```

### Comparing `datasette_secrets-0.1a2/datasette_secrets/templates/secrets_index.html` & `datasette_secrets-0.1a3/datasette_secrets/templates/secrets_index.html`

 * *Files identical despite different names*

### Comparing `datasette_secrets-0.1a2/datasette_secrets/templates/secrets_update.html` & `datasette_secrets-0.1a3/datasette_secrets/templates/secrets_update.html`

 * *Files identical despite different names*

### Comparing `datasette_secrets-0.1a2/datasette_secrets.egg-info/PKG-INFO` & `datasette_secrets-0.1a3/datasette_secrets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-secrets
-Version: 0.1a2
+Version: 0.1a3
 Summary: Manage secrets such as API keys for use with other Datasette plugins
 Author: Datasette
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-secrets
 Project-URL: Changelog, https://github.com/datasette/datasette-secrets/releases
 Project-URL: Issues, https://github.com/datasette/datasette-secrets/issues
 Project-URL: CI, https://github.com/datasette/datasette-secrets/actions
```

### Comparing `datasette_secrets-0.1a2/pyproject.toml` & `datasette_secrets-0.1a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "datasette-secrets"
-version = "0.1a2"
+version = "0.1a3"
 description = "Manage secrets such as API keys for use with other Datasette plugins"
 readme = "README.md"
 authors = [{name = "Datasette"}]
 license = {text = "Apache-2.0"}
 classifiers=[
     "Framework :: Datasette",
     "License :: OSI Approved :: Apache Software License"
```

### Comparing `datasette_secrets-0.1a2/tests/test_secrets.py` & `datasette_secrets-0.1a3/tests/test_secrets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from click.testing import CliRunner
 from cryptography.fernet import Fernet
 from datasette import hookimpl
 from datasette.app import Datasette
 from datasette.cli import cli
 from datasette.plugins import pm
-from datasette_secrets import get_secret, Secret
+from datasette_secrets import get_secret, Secret, startup
 import pytest
 from unittest.mock import ANY
 
 TEST_ENCRYPTION_KEY = "-LujHtwFWGaBpznrV1zduoZBmCnMOW7J0H5hmeXgAVo="
 
 
 def test_generate_command():
@@ -265,14 +265,19 @@
     assert response.status_code == 200
     expected_html = """
     <li><strong>EXAMPLE_SECRET</a></strong> - An example secret<br>
       <span style="font-size: 0.8 em">Set by <code>DATASETTE_SECRETS_EXAMPLE_SECRET</code></span></li>
     """
     assert remove_whitespace(expected_html) in remove_whitespace(response.text)
 
+    # Finally it should still work even if the datasette_secrets table is missing
+    await db.execute_write("drop table datasette_secrets")
+    monkeypatch.delenv("DATASETTE_SECRETS_EXAMPLE_SECRET")
+    assert await get_secret(ds, "EXAMPLE_SECRET") is None
+
 
 @pytest.mark.asyncio
 async def test_secret_index_page(ds, register_multiple_secrets):
     response = await ds.client.get(
         "/-/secrets",
         cookies={
             "ds_actor": ds.client.actor_cookie({"id": "admin"}),
```

