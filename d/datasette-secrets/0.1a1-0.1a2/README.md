# Comparing `tmp/datasette_secrets-0.1a1.tar.gz` & `tmp/datasette_secrets-0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette_secrets-0.1a1.tar", last modified: Tue Apr 23 05:35:10 2024, max compression
+gzip compressed data, was "datasette_secrets-0.1a2.tar", last modified: Wed Apr 24 22:20:58 2024, max compression
```

## Comparing `datasette_secrets-0.1a1.tar` & `datasette_secrets-0.1a2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:35:10.920139 datasette_secrets-0.1a1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 05:35:03.000000 datasette_secrets-0.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-04-23 05:35:10.920139 datasette_secrets-0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-23 05:35:03.000000 datasette_secrets-0.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:35:10.916139 datasette_secrets-0.1a1/datasette_secrets/
--rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-04-23 05:35:03.000000 datasette_secrets-0.1a1/datasette_secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-23 05:35:03.000000 datasette_secrets-0.1a1/datasette_secrets/hookspecs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:35:10.916139 datasette_secrets-0.1a1/datasette_secrets/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-23 05:35:03.000000 datasette_secrets-0.1a1/datasette_secrets/templates/secrets_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-23 05:35:03.000000 datasette_secrets-0.1a1/datasette_secrets/templates/secrets_update.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:35:10.920139 datasette_secrets-0.1a1/datasette_secrets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-04-23 05:35:10.000000 datasette_secrets-0.1a1/datasette_secrets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-23 05:35:10.000000 datasette_secrets-0.1a1/datasette_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 05:35:10.000000 datasette_secrets-0.1a1/datasette_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-23 05:35:10.000000 datasette_secrets-0.1a1/datasette_secrets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-23 05:35:10.000000 datasette_secrets-0.1a1/datasette_secrets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 05:35:10.000000 datasette_secrets-0.1a1/datasette_secrets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-23 05:35:03.000000 datasette_secrets-0.1a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 05:35:10.920139 datasette_secrets-0.1a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:35:10.920139 datasette_secrets-0.1a1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-04-23 05:35:03.000000 datasette_secrets-0.1a1/tests/test_secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:20:58.792120 datasette_secrets-0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 22:20:52.000000 datasette_secrets-0.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-24 22:20:58.792120 datasette_secrets-0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-24 22:20:52.000000 datasette_secrets-0.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:20:58.788120 datasette_secrets-0.1a2/datasette_secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-04-24 22:20:52.000000 datasette_secrets-0.1a2/datasette_secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-24 22:20:52.000000 datasette_secrets-0.1a2/datasette_secrets/hookspecs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:20:58.792120 datasette_secrets-0.1a2/datasette_secrets/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-24 22:20:52.000000 datasette_secrets-0.1a2/datasette_secrets/templates/secrets_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-24 22:20:52.000000 datasette_secrets-0.1a2/datasette_secrets/templates/secrets_update.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:20:58.792120 datasette_secrets-0.1a2/datasette_secrets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-24 22:20:58.000000 datasette_secrets-0.1a2/datasette_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-24 22:20:58.000000 datasette_secrets-0.1a2/datasette_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 22:20:58.000000 datasette_secrets-0.1a2/datasette_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 22:20:58.000000 datasette_secrets-0.1a2/datasette_secrets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-24 22:20:58.000000 datasette_secrets-0.1a2/datasette_secrets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 22:20:58.000000 datasette_secrets-0.1a2/datasette_secrets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-24 22:20:52.000000 datasette_secrets-0.1a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 22:20:58.792120 datasette_secrets-0.1a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:20:58.792120 datasette_secrets-0.1a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-04-24 22:20:52.000000 datasette_secrets-0.1a2/tests/test_secrets.py
```

### Comparing `datasette_secrets-0.1a1/LICENSE` & `datasette_secrets-0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette_secrets-0.1a1/PKG-INFO` & `datasette_secrets-0.1a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-secrets
-Version: 0.1a1
+Version: 0.1a2
 Summary: Manage secrets such as API keys for use with other Datasette plugins
 Author: Datasette
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-secrets
 Project-URL: Changelog, https://github.com/datasette/datasette-secrets/releases
 Project-URL: Issues, https://github.com/datasette/datasette-secrets/issues
 Project-URL: CI, https://github.com/datasette/datasette-secrets/actions
@@ -101,14 +101,16 @@
   --root
 ```
 
 ## Usage
 
 users with the `manage-secrets` permission will see a new "Manage secrets" link in the Datasette navigation menu. This interface can also be accessed at `/-/secrets`.
 
+The page with the list of secrets will show the user who last updated each secret. This will use the [actors_from_ids()](https://docs.datasette.io/en/latest/plugin_hooks.html#actors-from-ids-datasette-actor-ids) mechanism, displaying the actor's `username` if available, otherwise the `name`, otherwise the `id`.
+
 ## For plugin authors
 
 Plugins can depend on this plugin if they want to implement secrets.
 
 `datasette-secrets` to the `dependencies` list in `pyproject.toml`.
 
 Then declare the name and description of any secrets you need using the `register_secrets()` plugin hook:
@@ -117,19 +119,32 @@
 from datasette import hookimpl
 from datasette_secrets import Secret
 
 @hookimpl
 def register_secrets():
     return [
         Secret(
-            "OPENAI_API_KEY",
-            'An OpenAI API key. Get them from <a href="https://platform.openai.com/api-keys">here</a>.',
+            name="OPENAI_API_KEY",
+            description="An OpenAI API key"
+        ),
+    ]
+```
+You can also provide optional `obtain_url` and `obtain_label` fields to link to a page where a user can obtain an API key:
+```python
+@hookimpl
+def register_secrets():
+    return [
+        Secret(
+            name="OPENAI_API_KEY",
+            obtain_url="https://platform.openai.com/api-keys",
+            obtain_label="Get an OpenAI API key"
         ),
     ]
 ```
+
 The hook can take an optional `datasette` argument. It can return a list or an `async def` function that, when awaited, returns a list.
 
 The list should consist of `Secret()` instances, each with a name and an optional description. The description can contain HTML.
 
 To obtain the current value of the secret, use the `await get_secret()` method:
 
 ```python
```

### Comparing `datasette_secrets-0.1a1/README.md` & `datasette_secrets-0.1a2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -80,14 +80,16 @@
   --root
 ```
 
 ## Usage
 
 users with the `manage-secrets` permission will see a new "Manage secrets" link in the Datasette navigation menu. This interface can also be accessed at `/-/secrets`.
 
+The page with the list of secrets will show the user who last updated each secret. This will use the [actors_from_ids()](https://docs.datasette.io/en/latest/plugin_hooks.html#actors-from-ids-datasette-actor-ids) mechanism, displaying the actor's `username` if available, otherwise the `name`, otherwise the `id`.
+
 ## For plugin authors
 
 Plugins can depend on this plugin if they want to implement secrets.
 
 `datasette-secrets` to the `dependencies` list in `pyproject.toml`.
 
 Then declare the name and description of any secrets you need using the `register_secrets()` plugin hook:
@@ -96,19 +98,32 @@
 from datasette import hookimpl
 from datasette_secrets import Secret
 
 @hookimpl
 def register_secrets():
     return [
         Secret(
-            "OPENAI_API_KEY",
-            'An OpenAI API key. Get them from <a href="https://platform.openai.com/api-keys">here</a>.',
+            name="OPENAI_API_KEY",
+            description="An OpenAI API key"
+        ),
+    ]
+```
+You can also provide optional `obtain_url` and `obtain_label` fields to link to a page where a user can obtain an API key:
+```python
+@hookimpl
+def register_secrets():
+    return [
+        Secret(
+            name="OPENAI_API_KEY",
+            obtain_url="https://platform.openai.com/api-keys",
+            obtain_label="Get an OpenAI API key"
         ),
     ]
 ```
+
 The hook can take an optional `datasette` argument. It can return a list or an `async def` function that, when awaited, returns a list.
 
 The list should consist of `Secret()` instances, each with a name and an optional description. The description can contain HTML.
 
 To obtain the current value of the secret, use the `await get_secret()` method:
 
 ```python
```

### Comparing `datasette_secrets-0.1a1/datasette_secrets/__init__.py` & `datasette_secrets-0.1a2/datasette_secrets/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,17 @@
     )
     return decrypted.decode("utf-8")
 
 
 @dataclasses.dataclass
 class Secret:
     name: str
-    description_html: Optional[str] = None
+    description: Optional[str] = None
+    obtain_url: Optional[str] = None
+    obtain_label: Optional[str] = None
 
 
 SCHEMA = """
 create table if not exists datasette_secrets (
     id integer primary key,
     name text not null,
     note text,
@@ -110,34 +112,29 @@
             default=False,
         )
     ]
 
 
 async def get_secrets(datasette):
     secrets = []
+    seen = set()
     for result in pm.hook.register_secrets(datasette=datasette):
         result = await await_me_maybe(result)
-        secrets.extend(result)
+        for secret in result:
+            if secret.name in seen:
+                continue  # Skip duplicates
+            seen.add(secret.name)
+            secrets.append(secret)
     # if not secrets:
     secrets.append(Secret("EXAMPLE_SECRET", "An example secret"))
 
     return secrets
 
 
 @hookimpl
-def register_secrets():
-    return [
-        Secret(
-            "OPENAI_API_KEY",
-            'An OpenAI API key. Get them from <a href="https://platform.openai.com/api-keys">here</a>.',
-        ),
-    ]
-
-
-@hookimpl
 def register_commands(cli):
     @cli.group()
     def secrets():
         "Commands for managing datasette-secrets"
 
     @secrets.command()
     def generate_encryption_key():
@@ -179,14 +176,24 @@
         group by name
         """.format(
             ", ".join("?" for _ in environment_secrets_names)
         ),
         list(environment_secrets_names),
     )
     existing_secrets = {row["name"]: dict(row) for row in existing_secrets_result.rows}
+    # Try to turn updated_by into actors
+    actors = await datasette.actors_from_ids(
+        {row["updated_by"] for row in existing_secrets.values() if row["updated_by"]}
+    )
+    for secret in existing_secrets.values():
+        if secret["updated_by"]:
+            actor = actors.get(secret["updated_by"])
+            if actor:
+                display = actor.get("username") or actor.get("name") or actor.get("id")
+                secret["updated_by"] = display
     unset_secrets = [
         secret
         for secret in all_secrets
         if secret.name not in existing_secrets
         and secret.name not in environment_secrets_names
     ]
     return Response.html(
```

### Comparing `datasette_secrets-0.1a1/datasette_secrets/templates/secrets_index.html` & `datasette_secrets-0.1a2/datasette_secrets/templates/secrets_update.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 {% extends "base.html" %}
 
-{% block title %}Manage secrets{% endblock %}
+{% block title %}{% if current_secret %}Update{% else %}Add{% endif %} secret: {{ secret_name }}{% endblock %}
+
+{% block crumbs %}
+<p class="crumbs"><a href="{{ urls.path("/") }}">home</a> / <a href="{{ urls.path("/-/secrets") }}">secrets</a></p>
+{% endblock %}
 
 {% block content %}
-<h1>Manage secrets</h1>
+<h1>{% if current_secret %}Update{% else %}Add{% endif %} secret: {{ secret_name }}</h1>
 
-{% if existing_secrets %}
-<table>
-  <tr><th>Secret</th><th>Note</th><th>Version</th><th>Last updated</th><th>Updated by</th></tr>
-  {% for secret in existing_secrets %}
-    <tr>
-      <td><strong><a href="{{ urls.path("/-/secrets/") }}{{ secret.name }}">{{ secret.name }}</a></strong></td>
-      <td>{{ secret.note }}</td>
-      <td>{{ secret.version }}</td>
-      <td>{{ secret.updated_at or "" }}</td>
-      <td>{{ secret.updated_by or "" }}</td>
-    </tr>
-  {% endfor %}
-</table>
+{% if secret_details.description or secret_details.obtain_label %}
+  <p>{{ secret_details.description or "" }}{% if secret_details.description and secret_details.obtain_label %}. {% endif %}
+  {% if secret_details.obtain_label %}<a href="{{ secret_details.obtain_url }}">{{ secret_details.obtain_label }}</a>{% endif %}
+  </p>
 {% endif %}
 
-{% if unset_secrets %}
-<p style="margin-top: 2em">The following secret{% if unset_secrets|length == 1 %} has{% else %}s have{% endif %} not been set:</p>
-<ul>
-  {% for secret in unset_secrets %}
-    <li><strong><a href="{{ urls.path("/-/secrets/") }}{{ secret.name }}">{{ secret.name }}</a></strong>
-    {% if secret.description_html %} - {{ secret.description_html|safe }}{% endif %}</li>
-  {% endfor %}
-</ul>
+{% if error %}
+  <p class="message-error">{{ error }}</p>
 {% endif %}
 
-{% if environment_secrets %}
-<p style="margin-top: 2em">The following secret{% if environment_secrets|length == 1 %} is{% else %}s are{% endif %} set using environment variables:</p>
-<ul>
-  {% for secret in environment_secrets %}
-    <li><strong>{{ secret.name }}</a></strong>- {{ secret.description_html|safe }}<br>
-      <span style="font-size: 0.8 em">Set by <code>DATASETTE_SECRETS_{{ secret.name }}</code></span></li>
-  {% endfor %}
-</ul>
-{% endif %}
+<form action="{{ request.path }}" method="post">
+  <p>
+    <label for="secret">Secret:</label>
+  </p>
+  <p>
+    <textarea name="secret" style="width: 80%; height: 5em" id="secret"{% if not current_secret %} required{% endif %}
+      placeholder="{% if current_secret %}Leave this blank to leave the stored secret unchanged{% else %}Enter the secret here{% endif %}"
+    ></textarea>
+  </p>
+  <p>
+    <label for="note">Note (optional):</label>
+  </p>
+  <p>
+    <input type="text" name="note" id="note" maxlength="{{ max_note_length}}"
+      placeholder="{% if current_secret %}Add a note to the secret{% else %}Optional note{% endif %}"
+      value="{% if current_secret %}{{ current_secret.note }}{% endif %}"
+  </p>
+  <p>
+    <input type="submit" value="Add secret">
+    <input type="hidden" name="csrftoken" value="{{ csrftoken() }}">
+  </p>
+</form>
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,28 +1,23 @@
-{% extends "base.html" %} {% block title %}Manage secrets{% endblock %} {%
-block content %}
-************ MMaannaaggee sseeccrreettss ************
-{% if existing_secrets %}
-SSeeccrreett        NNoottee           VVeerrssiioonn        LLaasstt uuppddaatteedd      UUppddaatteedd bbyy
-/secrets/")
-}}{                          {              {                 {
-{ secret.name {{ secret.note {              {                 {
-}}">{         }}             secret.version secret.updated_at secret.updated_by
-{ secret.name                }}             or "" }}          or "" }}
-}}
-{% endif %} {% if unset_secrets %}
-The following secret{% if unset_secrets|length == 1 %} has{% else %}s have{%
-endif %} not been set:
-    * {% for secret in unset_secrets %}
-    * /secrets/") }}{{ secret.name }}">{{ secret.name }}
- {% if secret.description_html %} - {{ secret.description_html|safe }}{% endif
-%}
-{% endfor %}
-{% endif %} {% if environment_secrets %}
-The following secret{% if environment_secrets|length == 1 %} is{% else %}s are
-{% endif %} set using environment variables:
-    * {% for secret in environment_secrets %}
-    * {{{{ sseeccrreett..nnaammee }}}}
-- {{ secret.description_html|safe }}
-Set by DATASETTE_SECRETS_{{ secret.name }}
-{% endfor %}
-{% endif %} {% endblock %}
+{% extends "base.html" %} {% block title %}{% if current_secret %}Update{% else
+%}Add{% endif %} secret: {{ secret_name }}{% endblock %} {% block crumbs %}
+) }}">home
+ /
+/secrets") }}">secrets
+{% endblock %} {% block content %}
+************ {{%% iiff ccuurrrreenntt__sseeccrreett %%}}UUppddaattee{{%% eellssee %%}}AAdddd{{%% eennddiiff %%}} sseeccrreett:: {{
+{{ sseeccrreett__nnaammee }}}} ************
+{% if secret_details.description or secret_details.obtain_label %}
+{{ secret_details.description or "" }}{% if secret_details.description and
+secret_details.obtain_label %}. {% endif %} {% if secret_details.obtain_label
+%}_{_{_ _s_e_c_r_e_t___d_e_t_a_i_l_s_._o_b_t_a_i_n___l_a_b_e_l_ _}_}{% endif %}
+{% endif %} {% if error %}
+{{ error }}
+{% endif %}
+Secret:
+% if not current_secret %} required{% endif %} placeholder="{% if
+current_secret %}Leave this blank to leave the stored secret unchanged{% else
+%}Enter the secret here{% endif %}" >
+Note (optional):
+/p>
+[Add secret]
+{% endblock %}
```

### Comparing `datasette_secrets-0.1a1/datasette_secrets.egg-info/PKG-INFO` & `datasette_secrets-0.1a2/datasette_secrets.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-secrets
-Version: 0.1a1
+Version: 0.1a2
 Summary: Manage secrets such as API keys for use with other Datasette plugins
 Author: Datasette
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-secrets
 Project-URL: Changelog, https://github.com/datasette/datasette-secrets/releases
 Project-URL: Issues, https://github.com/datasette/datasette-secrets/issues
 Project-URL: CI, https://github.com/datasette/datasette-secrets/actions
@@ -101,14 +101,16 @@
   --root
 ```
 
 ## Usage
 
 users with the `manage-secrets` permission will see a new "Manage secrets" link in the Datasette navigation menu. This interface can also be accessed at `/-/secrets`.
 
+The page with the list of secrets will show the user who last updated each secret. This will use the [actors_from_ids()](https://docs.datasette.io/en/latest/plugin_hooks.html#actors-from-ids-datasette-actor-ids) mechanism, displaying the actor's `username` if available, otherwise the `name`, otherwise the `id`.
+
 ## For plugin authors
 
 Plugins can depend on this plugin if they want to implement secrets.
 
 `datasette-secrets` to the `dependencies` list in `pyproject.toml`.
 
 Then declare the name and description of any secrets you need using the `register_secrets()` plugin hook:
@@ -117,19 +119,32 @@
 from datasette import hookimpl
 from datasette_secrets import Secret
 
 @hookimpl
 def register_secrets():
     return [
         Secret(
-            "OPENAI_API_KEY",
-            'An OpenAI API key. Get them from <a href="https://platform.openai.com/api-keys">here</a>.',
+            name="OPENAI_API_KEY",
+            description="An OpenAI API key"
+        ),
+    ]
+```
+You can also provide optional `obtain_url` and `obtain_label` fields to link to a page where a user can obtain an API key:
+```python
+@hookimpl
+def register_secrets():
+    return [
+        Secret(
+            name="OPENAI_API_KEY",
+            obtain_url="https://platform.openai.com/api-keys",
+            obtain_label="Get an OpenAI API key"
         ),
     ]
 ```
+
 The hook can take an optional `datasette` argument. It can return a list or an `async def` function that, when awaited, returns a list.
 
 The list should consist of `Secret()` instances, each with a name and an optional description. The description can contain HTML.
 
 To obtain the current value of the secret, use the `await get_secret()` method:
 
 ```python
```

### Comparing `datasette_secrets-0.1a1/pyproject.toml` & `datasette_secrets-0.1a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "datasette-secrets"
-version = "0.1a1"
+version = "0.1a2"
 description = "Manage secrets such as API keys for use with other Datasette plugins"
 readme = "README.md"
 authors = [{name = "Datasette"}]
 license = {text = "Apache-2.0"}
 classifiers=[
     "Framework :: Datasette",
     "License :: OSI Approved :: Apache Software License"
```

