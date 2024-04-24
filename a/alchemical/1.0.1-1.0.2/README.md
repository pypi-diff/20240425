# Comparing `tmp/alchemical-1.0.1.tar.gz` & `tmp/alchemical-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchemical-1.0.1.tar", last modified: Sat Oct 28 23:01:43 2023, max compression
+gzip compressed data, was "alchemical-1.0.2.tar", last modified: Wed Apr 24 23:21:52 2024, max compression
```

## Comparing `alchemical-1.0.1.tar` & `alchemical-1.0.2.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-10-28 23:01:43.388603 alchemical-1.0.1/
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     1072 2023-06-20 11:45:14.000000 alchemical-1.0.1/LICENSE
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      185 2023-10-15 12:08:35.000000 alchemical-1.0.1/MANIFEST.in
--rw-r--r--   0 miguel    (1000) miguel    (1000)     1204 2023-10-28 23:01:43.388603 alchemical-1.0.1/PKG-INFO
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      538 2023-10-28 19:11:03.000000 alchemical-1.0.1/README.md
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-10-28 23:01:43.384603 alchemical-1.0.1/docs/
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      634 2023-06-20 11:45:14.000000 alchemical-1.0.1/docs/Makefile
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-10-28 23:01:43.384603 alchemical-1.0.1/docs/_static/
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-10-28 23:01:43.384603 alchemical-1.0.1/docs/_static/css/
--rw-rw-r--   0 miguel    (1000) miguel    (1000)       63 2023-06-20 11:45:14.000000 alchemical-1.0.1/docs/_static/css/custom.css
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      483 2023-06-20 11:45:14.000000 alchemical-1.0.1/docs/api.rst
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     2174 2023-06-20 11:45:14.000000 alchemical-1.0.1/docs/conf.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     8554 2023-10-28 16:50:05.000000 alchemical-1.0.1/docs/howdoi.rst
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      344 2023-06-20 11:45:14.000000 alchemical-1.0.1/docs/index.rst
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     2096 2023-10-28 16:52:09.000000 alchemical-1.0.1/docs/intro.rst
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      795 2023-06-20 11:45:14.000000 alchemical-1.0.1/docs/make.bat
--rw-rw-r--   0 miguel    (1000) miguel    (1000)       53 2023-06-20 11:45:14.000000 alchemical-1.0.1/docs/requirements.txt
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    12498 2023-10-28 16:57:22.000000 alchemical-1.0.1/docs/usage.rst
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     1062 2023-10-28 23:01:39.000000 alchemical-1.0.1/pyproject.toml
--rw-rw-r--   0 miguel    (1000) miguel    (1000)       38 2023-10-28 23:01:43.388603 alchemical-1.0.1/setup.cfg
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-10-28 23:01:43.384603 alchemical-1.0.1/src/
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-10-28 23:01:43.384603 alchemical-1.0.1/src/alchemical/
--rw-rw-r--   0 miguel    (1000) miguel    (1000)       85 2023-10-20 22:06:24.000000 alchemical-1.0.1/src/alchemical/__init__.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     6487 2023-10-28 18:27:52.000000 alchemical-1.0.1/src/alchemical/aio.py
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-10-28 23:01:43.388603 alchemical-1.0.1/src/alchemical/alembic/
--rw-rw-r--   0 miguel    (1000) miguel    (1000)        0 2023-06-20 11:45:14.000000 alchemical-1.0.1/src/alchemical/alembic/__init__.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     1154 2023-06-20 11:45:14.000000 alchemical-1.0.1/src/alchemical/alembic/cli.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     4742 2023-06-20 11:45:14.000000 alchemical-1.0.1/src/alchemical/alembic/env.py
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-10-28 23:01:43.384603 alchemical-1.0.1/src/alchemical/alembic/templates/
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-10-28 23:01:43.388603 alchemical-1.0.1/src/alchemical/alembic/templates/generic/
--rw-rw-r--   0 miguel    (1000) miguel    (1000)       37 2023-06-20 11:45:14.000000 alchemical-1.0.1/src/alchemical/alembic/templates/generic/README
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     3478 2023-06-20 11:45:14.000000 alchemical-1.0.1/src/alchemical/alembic/templates/generic/alembic.ini.mako
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      967 2023-06-25 19:13:33.000000 alchemical-1.0.1/src/alchemical/alembic/templates/generic/env.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      965 2023-06-20 11:45:14.000000 alchemical-1.0.1/src/alchemical/alembic/templates/generic/script.py.mako
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    10799 2023-10-28 22:58:01.000000 alchemical-1.0.1/src/alchemical/core.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     2747 2023-10-20 22:08:31.000000 alchemical-1.0.1/src/alchemical/flask.py
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-10-28 23:01:43.388603 alchemical-1.0.1/src/alchemical.egg-info/
--rw-r--r--   0 miguel    (1000) miguel    (1000)     1204 2023-10-28 23:01:43.000000 alchemical-1.0.1/src/alchemical.egg-info/PKG-INFO
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      985 2023-10-28 23:01:43.000000 alchemical-1.0.1/src/alchemical.egg-info/SOURCES.txt
--rw-rw-r--   0 miguel    (1000) miguel    (1000)        1 2023-10-28 23:01:43.000000 alchemical-1.0.1/src/alchemical.egg-info/dependency_links.txt
--rw-rw-r--   0 miguel    (1000) miguel    (1000)        1 2023-06-25 15:00:38.000000 alchemical-1.0.1/src/alchemical.egg-info/not-zip-safe
--rw-rw-r--   0 miguel    (1000) miguel    (1000)       34 2023-10-28 23:01:43.000000 alchemical-1.0.1/src/alchemical.egg-info/requires.txt
--rw-rw-r--   0 miguel    (1000) miguel    (1000)       11 2023-10-28 23:01:43.000000 alchemical-1.0.1/src/alchemical.egg-info/top_level.txt
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-10-28 23:01:43.388603 alchemical-1.0.1/tests/
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      576 2023-10-28 16:45:40.000000 alchemical-1.0.1/tests/aioapp1.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      635 2023-10-28 16:46:14.000000 alchemical-1.0.1/tests/aioapp2.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      572 2023-10-28 16:47:05.000000 alchemical-1.0.1/tests/app1.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      631 2023-10-28 16:47:51.000000 alchemical-1.0.1/tests/app2.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     7161 2023-10-28 22:58:26.000000 alchemical-1.0.1/tests/test_aio.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     6597 2023-06-20 11:45:14.000000 alchemical-1.0.1/tests/test_alembic.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     7457 2023-10-28 22:58:37.000000 alchemical-1.0.1/tests/test_core.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     5946 2023-10-28 22:59:01.000000 alchemical-1.0.1/tests/test_flask.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      917 2023-10-28 15:48:45.000000 alchemical-1.0.1/tox.ini
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-04-24 23:21:52.164958 alchemical-1.0.2/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1072 2023-06-20 11:45:14.000000 alchemical-1.0.2/LICENSE
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      185 2023-10-15 12:08:35.000000 alchemical-1.0.2/MANIFEST.in
+-rw-r--r--   0 miguel    (1000) miguel    (1000)     1204 2024-04-24 23:21:52.164958 alchemical-1.0.2/PKG-INFO
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      538 2023-10-28 19:11:03.000000 alchemical-1.0.2/README.md
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-04-24 23:21:52.164958 alchemical-1.0.2/docs/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      634 2023-06-20 11:45:14.000000 alchemical-1.0.2/docs/Makefile
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-04-24 23:21:52.164958 alchemical-1.0.2/docs/_static/
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-04-24 23:21:52.164958 alchemical-1.0.2/docs/_static/css/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       63 2023-06-20 11:45:14.000000 alchemical-1.0.2/docs/_static/css/custom.css
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      483 2023-06-20 11:45:14.000000 alchemical-1.0.2/docs/api.rst
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     2174 2023-06-20 11:45:14.000000 alchemical-1.0.2/docs/conf.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     8554 2023-10-28 16:50:05.000000 alchemical-1.0.2/docs/howdoi.rst
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      344 2023-06-20 11:45:14.000000 alchemical-1.0.2/docs/index.rst
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     2098 2024-04-24 22:22:36.000000 alchemical-1.0.2/docs/intro.rst
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      795 2023-06-20 11:45:14.000000 alchemical-1.0.2/docs/make.bat
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       53 2023-06-20 11:45:14.000000 alchemical-1.0.2/docs/requirements.txt
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    12490 2024-04-24 22:22:36.000000 alchemical-1.0.2/docs/usage.rst
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1062 2024-04-24 23:21:50.000000 alchemical-1.0.2/pyproject.toml
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       38 2024-04-24 23:21:52.164958 alchemical-1.0.2/setup.cfg
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-04-24 23:21:52.164958 alchemical-1.0.2/src/
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-04-24 23:21:52.164958 alchemical-1.0.2/src/alchemical/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       85 2023-10-20 22:06:24.000000 alchemical-1.0.2/src/alchemical/__init__.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     7576 2024-04-24 23:02:08.000000 alchemical-1.0.2/src/alchemical/aio.py
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-04-24 23:21:52.164958 alchemical-1.0.2/src/alchemical/alembic/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)        0 2023-06-20 11:45:14.000000 alchemical-1.0.2/src/alchemical/alembic/__init__.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1154 2023-06-20 11:45:14.000000 alchemical-1.0.2/src/alchemical/alembic/cli.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     4742 2023-06-20 11:45:14.000000 alchemical-1.0.2/src/alchemical/alembic/env.py
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-04-24 23:21:52.164958 alchemical-1.0.2/src/alchemical/alembic/templates/
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-04-24 23:21:52.164958 alchemical-1.0.2/src/alchemical/alembic/templates/generic/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       37 2023-06-20 11:45:14.000000 alchemical-1.0.2/src/alchemical/alembic/templates/generic/README
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     3478 2023-06-20 11:45:14.000000 alchemical-1.0.2/src/alchemical/alembic/templates/generic/alembic.ini.mako
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      967 2023-06-25 19:13:33.000000 alchemical-1.0.2/src/alchemical/alembic/templates/generic/env.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      965 2023-06-20 11:45:14.000000 alchemical-1.0.2/src/alchemical/alembic/templates/generic/script.py.mako
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    10893 2024-04-24 23:11:05.000000 alchemical-1.0.2/src/alchemical/core.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     2747 2023-10-20 22:08:31.000000 alchemical-1.0.2/src/alchemical/flask.py
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-04-24 23:21:52.164958 alchemical-1.0.2/src/alchemical.egg-info/
+-rw-r--r--   0 miguel    (1000) miguel    (1000)     1204 2024-04-24 23:21:52.000000 alchemical-1.0.2/src/alchemical.egg-info/PKG-INFO
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1000 2024-04-24 23:21:52.000000 alchemical-1.0.2/src/alchemical.egg-info/SOURCES.txt
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)        1 2024-04-24 23:21:52.000000 alchemical-1.0.2/src/alchemical.egg-info/dependency_links.txt
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)        1 2023-06-25 15:00:38.000000 alchemical-1.0.2/src/alchemical.egg-info/not-zip-safe
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       34 2024-04-24 23:21:52.000000 alchemical-1.0.2/src/alchemical.egg-info/requires.txt
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       11 2024-04-24 23:21:52.000000 alchemical-1.0.2/src/alchemical.egg-info/top_level.txt
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-04-24 23:21:52.164958 alchemical-1.0.2/tests/
+-rw-r--r--   0 miguel    (1000) miguel    (1000)        0 2024-04-24 22:47:01.000000 alchemical-1.0.2/tests/_temp.db
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      576 2023-10-28 16:45:40.000000 alchemical-1.0.2/tests/aioapp1.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      635 2023-10-28 16:46:14.000000 alchemical-1.0.2/tests/aioapp2.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      572 2023-10-28 16:47:05.000000 alchemical-1.0.2/tests/app1.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      631 2023-10-28 16:47:51.000000 alchemical-1.0.2/tests/app2.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     7757 2024-04-24 23:10:41.000000 alchemical-1.0.2/tests/test_aio.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     6597 2023-06-20 11:45:14.000000 alchemical-1.0.2/tests/test_alembic.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     8011 2024-04-24 22:47:55.000000 alchemical-1.0.2/tests/test_core.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     6536 2024-04-24 23:09:00.000000 alchemical-1.0.2/tests/test_flask.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      917 2023-10-28 15:48:45.000000 alchemical-1.0.2/tox.ini
```

### Comparing `alchemical-1.0.1/LICENSE` & `alchemical-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alchemical-1.0.1/PKG-INFO` & `alchemical-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemical
-Version: 1.0.1
+Version: 1.0.2
 Summary: Modern SQLAlchemy simplified
 Author-email: Miguel Grinberg <miguel.grinberg@gmail.com>
 Project-URL: Homepage, https://github.com/miguelgrinberg/alchemical
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/alchemical/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alchemical-1.0.1/README.md` & `alchemical-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alchemical-1.0.1/docs/Makefile` & `alchemical-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `alchemical-1.0.1/docs/conf.py` & `alchemical-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `alchemical-1.0.1/docs/howdoi.rst` & `alchemical-1.0.2/docs/howdoi.rst`

 * *Files identical despite different names*

### Comparing `alchemical-1.0.1/docs/intro.rst` & `alchemical-1.0.2/docs/intro.rst`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     from alchemical import Alchemical, Model
 
     class User(Model):
         id: Mapped[int] = mapped_column(primary_key=True)
         name: Mapped[str] = mapped_column(String(128))
 
         def __repr__(self):
-            return f'<User {self.name}'
+            return f'<User {self.name}>'
 
     db = Alchemical('sqlite:///users.sqlite')
     db.drop_all()
     db.create_all()
 
     with db.begin() as session:
         for name in ['mary', 'joe', 'susan']:
@@ -48,15 +48,15 @@
     from alchemical.aio import Alchemical, Model
 
     class User(Model):
         id: Mapped[int] = mapped_column(primary_key=True)
         name: Mapped[str] = mapped_column(String(128))
 
         def __repr__(self):
-            return f'<User {self.name}'
+            return f'<User {self.name}>'
 
     async def main():
         db = Alchemical('sqlite:///users.sqlite')
         await db.drop_all()
         await db.create_all()
 
         async with db.begin() as session:
```

### Comparing `alchemical-1.0.1/docs/make.bat` & `alchemical-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `alchemical-1.0.1/docs/usage.rst` & `alchemical-1.0.2/docs/usage.rst`

 * *Files 2% similar despite different names*

```diff
@@ -34,31 +34,31 @@
 
     from sqlalchemy.orm import Mapped, mapped_column
     from alchemical import Model
 
     class User(Model):
         id: Mapped[int] = mapped_column(primary_key=True)
         name: Mapped[str]
-        fullname = Mapped[str]
-        nickname = Mapped[str]
+        fullname: Mapped[str]
+        nickname: Mapped[str]
 
 See `Declarative Mapping <https://docs.sqlalchemy.org/en/14/orm/mapping_styles.html#declarative-mapping>`_
 in the SQLAlchemy documentation.
 
 Alchemical automatically names each database table with the name of its
 corresponding  model class converted to snake case. To override the automatic
 naming, a ``__tablename__`` attribute can be added to the model class::
 
     class User(Model):
         __tablename__ = 'users'
 
         id: Mapped[int] = mapped_column(primary_key=True)
         name: Mapped[str]
-        fullname = Mapped[str]
-        nickname = Mapped[str]
+        fullname: Mapped[str]
+        nickname: Mapped[str]
 
 Creating and Destroying Database Tables
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Alchemical can create all the tables referenced by models with a single call::
 
     db.create_all()
@@ -128,29 +128,29 @@
 to with the ``__bind_key__`` attribute::
 
     class User(Model):
         __bind_key__ = 'users'
 
         id: Mapped[int] = mapped_column(primary_key=True)
         name: Mapped[str]
-        fullname = Mapped[str]
-        nickname = Mapped[str]
+        fullname: Mapped[str]
+        nickname: Mapped[str]
 
 To avoid duplicating the ``__bind_key__`` attribute in many model classes, you
 can create an abstract parent class for each bind::
 
     class UsersBind(Model):
         __abstract__ = True
         __bind_key__ = 'users'
 
     class User(UsersBind):
         id: Mapped[int] = mapped_column(primary_key=True)
         name: Mapped[str]
-        fullname = Mapped[str]
-        nickname = Mapped[str]
+        fullname: Mapped[str]
+        nickname: Mapped[str]
 
 The ``Alchemical`` instance can also be configured to combine the use of a main
 database and binds. The following example connects to a MySQL database as the
 main database, plus the Postgres and SQLite databases of the previous example::
 
     db = Alchemical('mysqldb://user:password@localhost/db', binds={
         'users': 'postgresql://user:password@localhost/mydb',
```

### Comparing `alchemical-1.0.1/pyproject.toml` & `alchemical-1.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=61.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alchemical"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     { name = "Miguel Grinberg", email = "miguel.grinberg@gmail.com" },
 ]
 description = "Modern SQLAlchemy simplified"
 classifiers = [
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
```

### Comparing `alchemical-1.0.1/src/alchemical/aio.py` & `alchemical-1.0.2/src/alchemical/aio.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,14 +46,35 @@
                  naming_convention=None):
         super().__init__(url=url, binds=binds, engine_options=engine_options,
                          session_options=session_options,
                          model_class=model_class,
                          naming_convention=naming_convention)
         self._sync = None
 
+    def initialize(self, url=None, binds=None, engine_options=None,
+                   session_options=None):
+        """Initialize the database instance.
+
+        :param url: the database URL.
+        :param binds: a dictionary with additional databases to manage with
+                      this instance. The keys are the names, and the values are
+                      the database URLs. A model is then assigned to a specific
+                      bind with the `__bind_key__` class attribute.
+        :param engine_options: a dictionary with additional engine options to
+                               pass to SQLAlchemy.
+        :param session_options: a dictionary with additional session options to
+                                use when creating sessions.
+
+        This method must be called explicitly to complete the initialization of
+        the instance the two-phase initialization method is used.
+        """
+        super().initialize(url, binds=binds, engine_options=engine_options,
+                           session_options=session_options)
+        self._sync = None
+
     def _create_engine(self, url, *args, **kwargs):
         return create_async_engine(url, *args, **kwargs)
 
     async def create_all(self):
         """Create the database tables.
 
         Only tables that do not already exist are created. Existing tables are
```

### Comparing `alchemical-1.0.1/src/alchemical/alembic/cli.py` & `alchemical-1.0.2/src/alchemical/alembic/cli.py`

 * *Files identical despite different names*

### Comparing `alchemical-1.0.1/src/alchemical/alembic/env.py` & `alchemical-1.0.2/src/alchemical/alembic/env.py`

 * *Files identical despite different names*

### Comparing `alchemical-1.0.1/src/alchemical/alembic/templates/generic/alembic.ini.mako` & `alchemical-1.0.2/src/alchemical/alembic/templates/generic/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `alchemical-1.0.1/src/alchemical/alembic/templates/generic/env.py` & `alchemical-1.0.2/src/alchemical/alembic/templates/generic/env.py`

 * *Files identical despite different names*

### Comparing `alchemical-1.0.1/src/alchemical/alembic/templates/generic/script.py.mako` & `alchemical-1.0.2/src/alchemical/alembic/templates/generic/script.py.mako`

 * *Files identical despite different names*

### Comparing `alchemical-1.0.1/src/alchemical/core.py` & `alchemical-1.0.2/src/alchemical/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,17 @@
         if url is None and binds is None:
             raise ValueError('"url" and/or "binds" must be set')
 
         self.url = url or self.url
         self.binds = binds or self.binds
         self.engine_options = engine_options or self.engine_options
         self.session_options = session_options or self.session_options
+        self.session_class = None
+        self.engines = None
+        self.table_binds = None
 
     def _get_declarative_base(self, model_class):
         if model_class is None:
             return Model
 
         if not issubclass(model_class, BaseModel):
             # if the given model class does not have the Alchemical additions
```

### Comparing `alchemical-1.0.1/src/alchemical/flask.py` & `alchemical-1.0.2/src/alchemical/flask.py`

 * *Files identical despite different names*

### Comparing `alchemical-1.0.1/src/alchemical.egg-info/PKG-INFO` & `alchemical-1.0.2/src/alchemical.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemical
-Version: 1.0.1
+Version: 1.0.2
 Summary: Modern SQLAlchemy simplified
 Author-email: Miguel Grinberg <miguel.grinberg@gmail.com>
 Project-URL: Homepage, https://github.com/miguelgrinberg/alchemical
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/alchemical/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alchemical-1.0.1/src/alchemical.egg-info/SOURCES.txt` & `alchemical-1.0.2/src/alchemical.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 src/alchemical/alembic/__init__.py
 src/alchemical/alembic/cli.py
 src/alchemical/alembic/env.py
 src/alchemical/alembic/templates/generic/README
 src/alchemical/alembic/templates/generic/alembic.ini.mako
 src/alchemical/alembic/templates/generic/env.py
 src/alchemical/alembic/templates/generic/script.py.mako
+tests/_temp.db
 tests/aioapp1.py
 tests/aioapp2.py
 tests/app1.py
 tests/app2.py
 tests/test_aio.py
 tests/test_alembic.py
 tests/test_core.py
```

### Comparing `alchemical-1.0.1/tests/aioapp1.py` & `alchemical-1.0.2/tests/aioapp1.py`

 * *Files identical despite different names*

### Comparing `alchemical-1.0.1/tests/aioapp2.py` & `alchemical-1.0.2/tests/aioapp2.py`

 * *Files identical despite different names*

### Comparing `alchemical-1.0.1/tests/app1.py` & `alchemical-1.0.2/tests/app1.py`

 * *Files identical despite different names*

### Comparing `alchemical-1.0.1/tests/app2.py` & `alchemical-1.0.2/tests/app2.py`

 * *Files identical despite different names*

### Comparing `alchemical-1.0.1/tests/test_aio.py` & `alchemical-1.0.2/tests/test_aio.py`

 * *Files 4% similar despite different names*

```diff
@@ -195,7 +195,26 @@
     def test_two_phase(self):
         db = Alchemical(engine_options={'foo': 'bar'},
                         session_options={'bar': 'foo'})
         db.initialize('sqlite://', engine_options={'foo': 'baz'},
                       session_options={'baz': 'foo'})
         assert db.engine_options == {'foo': 'baz'}
         assert db.session_options == {'baz': 'foo'}
+
+    @async_test
+    async def test_reinitialize(self):
+        db = Alchemical('sqlite://')
+
+        class User(db.Model):
+            id: Mapped[int] = mapped_column(primary_key=True)
+            name: Mapped[str]
+
+        await db.create_all()
+        async with db.begin() as session:
+            for name in ['mary', 'joe', 'susan']:
+                session.add(User(name=name))
+
+        db.initialize('sqlite://')
+        await db.create_all()
+        async with db.Session() as session:
+            all = (await session.execute(User.select())).scalars().all()
+        assert len(all) == 0
```

### Comparing `alchemical-1.0.1/tests/test_alembic.py` & `alchemical-1.0.2/tests/test_alembic.py`

 * *Files identical despite different names*

### Comparing `alchemical-1.0.1/tests/test_core.py` & `alchemical-1.0.2/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,14 +182,32 @@
         db = Alchemical(engine_options={'foo': 'bar'},
                         session_options={'bar': 'foo'})
         db.initialize('sqlite://', engine_options={'foo': 'baz'},
                       session_options={'baz': 'foo'})
         assert db.engine_options == {'foo': 'baz'}
         assert db.session_options == {'baz': 'foo'}
 
+    def test_reinitialize(self):
+        db = self.create_alchemical('sqlite://')
+
+        class User(db.Model):
+            id: Mapped[int] = mapped_column(primary_key=True)
+            name: Mapped[str]
+
+        db.create_all()
+        with db.begin() as session:
+            for name in ['mary', 'joe', 'susan']:
+                session.add(User(name=name))
+
+        db.initialize('sqlite://')
+        db.create_all()
+        with db.Session() as session:
+            all = session.execute(User.select()).scalars().all()
+        assert len(all) == 0
+
 
 class TestCoreWithCustomBase(TestCore):
     def create_alchemical(self, url=None, binds=None):
         class CustomModel:
             def foo(self):
                 return 42
```

### Comparing `alchemical-1.0.1/tests/test_flask.py` & `alchemical-1.0.2/tests/test_flask.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,14 @@
 
 class TestFlask(unittest.TestCase):
     def setUp(self):
         Model.metadata.clear()
         Model.__metadatas__.clear()
         clear_mappers()
 
-    def create_db(self):
-        db = Alchemical()
-        return db
-
     def test_read_write(self):
         db = Alchemical()
 
         class User(db.Model):
             id: Mapped[int] = mapped_column(primary_key=True)
             name: Mapped[str]
 
@@ -135,15 +131,14 @@
     def test_db_session(self):
         db = Alchemical()
 
         class User(db.Model):
             id: Mapped[int] = mapped_column(primary_key=True)
             name: Mapped[str]
 
-        db = self.create_db()
         app = Flask(__name__)
         app.config['ALCHEMICAL_DATABASE_URL'] = 'sqlite://'
         db.init_app(app)
 
         db.drop_all()
         db.create_all()
 
@@ -165,15 +160,14 @@
     def test_db_session_autocommit(self):
         db = Alchemical()
 
         class User(db.Model):
             id: Mapped[int] = mapped_column(primary_key=True)
             name: Mapped[str]
 
-        db = self.create_db()
         app = Flask(__name__)
         app.config['ALCHEMICAL_DATABASE_URL'] = 'sqlite://'
         app.config['ALCHEMICAL_AUTOCOMMIT'] = True
         db.init_app(app)
 
         db.drop_all()
         db.create_all()
@@ -182,14 +176,37 @@
             for name in ['mary', 'joe', 'susan']:
                 db.session.add(User(name=name))
 
         with db.Session() as session:
             all = session.execute(User.select()).scalars().all()
         assert len(all) == 3
 
+    def test_reinit(self):
+        db = Alchemical()
+
+        class User(db.Model):
+            id: Mapped[int] = mapped_column(primary_key=True)
+            name: Mapped[str]
+
+        app = Flask(__name__)
+        app.config['ALCHEMICAL_DATABASE_URL'] = 'sqlite://'
+        db.init_app(app)
+        db.create_all()
+        with db.begin() as session:
+            for name in ['mary', 'joe', 'susan']:
+                session.add(User(name=name))
+
+        app = Flask(__name__)
+        app.config['ALCHEMICAL_DATABASE_URL'] = 'sqlite://'
+        db.init_app(app)
+        db.create_all()
+        with db.Session() as session:
+            all = session.execute(User.select()).scalars().all()
+        assert len(all) == 0
+
     def test_bad_config(self):
         db = Alchemical()
         app = Flask(__name__)
         with pytest.raises(ValueError):
             db.init_app(app)
 
     def test_alternate_config(self):
```

### Comparing `alchemical-1.0.1/tox.ini` & `alchemical-1.0.2/tox.ini`

 * *Files identical despite different names*

