# Comparing `tmp/prefect-sqlalchemy-0.4.0.tar.gz` & `tmp/prefect_sqlalchemy-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect-sqlalchemy-0.4.0.tar", last modified: Mon Jan 22 14:26:45 2024, max compression
+gzip compressed data, was "prefect_sqlalchemy-0.4.1.tar", last modified: Thu Apr 25 16:19:29 2024, max compression
```

## Comparing `prefect-sqlalchemy-0.4.0.tar` & `prefect_sqlalchemy-0.4.1.tar`

### file list

```diff
@@ -1,26 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:26:45.042980 prefect-sqlalchemy-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-01-22 14:25:55.000000 prefect-sqlalchemy-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-01-22 14:25:55.000000 prefect-sqlalchemy-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-01-22 14:26:45.042980 prefect-sqlalchemy-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-01-22 14:25:55.000000 prefect-sqlalchemy-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:26:45.042980 prefect-sqlalchemy-0.4.0/prefect_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-01-22 14:25:55.000000 prefect-sqlalchemy-0.4.0/prefect_sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-01-22 14:26:45.042980 prefect-sqlalchemy-0.4.0/prefect_sqlalchemy/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    15376 2024-01-22 14:25:55.000000 prefect-sqlalchemy-0.4.0/prefect_sqlalchemy/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    35913 2024-01-22 14:25:55.000000 prefect-sqlalchemy-0.4.0/prefect_sqlalchemy/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:26:45.042980 prefect-sqlalchemy-0.4.0/prefect_sqlalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-01-22 14:26:45.000000 prefect-sqlalchemy-0.4.0/prefect_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-01-22 14:26:45.000000 prefect-sqlalchemy-0.4.0/prefect_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 14:26:45.000000 prefect-sqlalchemy-0.4.0/prefect_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-22 14:26:45.000000 prefect-sqlalchemy-0.4.0/prefect_sqlalchemy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-01-22 14:26:45.000000 prefect-sqlalchemy-0.4.0/prefect_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-22 14:26:45.000000 prefect-sqlalchemy-0.4.0/prefect_sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-01-22 14:25:55.000000 prefect-sqlalchemy-0.4.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 14:25:55.000000 prefect-sqlalchemy-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-01-22 14:26:45.042980 prefect-sqlalchemy-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-01-22 14:25:55.000000 prefect-sqlalchemy-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:26:45.042980 prefect-sqlalchemy-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-01-22 14:25:55.000000 prefect-sqlalchemy-0.4.0/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-01-22 14:25:55.000000 prefect-sqlalchemy-0.4.0/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    23374 2024-01-22 14:25:55.000000 prefect-sqlalchemy-0.4.0/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    80049 2024-01-22 14:25:55.000000 prefect-sqlalchemy-0.4.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:19:29.052434 prefect_sqlalchemy-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-04-25 16:19:29.052434 prefect_sqlalchemy-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8826 2024-04-25 16:19:16.000000 prefect_sqlalchemy-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:19:29.044434 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-25 16:19:16.000000 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 16:19:28.000000 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15377 2024-04-25 16:19:16.000000 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35914 2024-04-25 16:19:16.000000 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:19:29.048434 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-04-25 16:19:28.000000 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-25 16:19:29.000000 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:19:28.000000 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 16:19:28.000000 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-25 16:19:28.000000 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 16:19:28.000000 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-25 16:19:16.000000 prefect_sqlalchemy-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:19:29.052434 prefect_sqlalchemy-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:19:29.048434 prefect_sqlalchemy-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-25 16:19:16.000000 prefect_sqlalchemy-0.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-25 16:19:16.000000 prefect_sqlalchemy-0.4.1/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-25 16:19:16.000000 prefect_sqlalchemy-0.4.1/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23372 2024-04-25 16:19:16.000000 prefect_sqlalchemy-0.4.1/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-25 16:19:16.000000 prefect_sqlalchemy-0.4.1/tests/test_version.py
```

### Comparing `prefect-sqlalchemy-0.4.0/PKG-INFO` & `prefect_sqlalchemy-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,90 +1,77 @@
 Metadata-Version: 2.1
 Name: prefect-sqlalchemy
-Version: 0.4.0
-Summary: Prefect integrations for interacting with SQLAlchemy.
-Home-page: https://github.com/PrefectHQ/prefect-sqlalchemy
-Author: Prefect Technologies, Inc.
-Author-email: help@prefect.io
+Version: 0.4.1
+Summary: Prefect integrations for working with databases
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-sqlalchemy
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: prefect>=2.13.5
 Requires-Dist: sqlalchemy<3,>=1.4.31
+Requires-Dist: prefect>=2.13.5
 Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: mkdocs; extra == "dev"
+Requires-Dist: aiosqlite; extra == "dev"
+Requires-Dist: asyncpg; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: interrogate; extra == "dev"
+Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: mock; python_version < "3.8" and extra == "dev"
-Requires-Dist: mkdocs-gen-files; extra == "dev"
-Requires-Dist: interrogate; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
-Requires-Dist: psycopg2; extra == "dev"
-Requires-Dist: asyncpg; extra == "dev"
-Requires-Dist: aiosqlite; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: psycopg2; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 
 # prefect-sqlalchemy
 
 <p align="center">
-    <img src="https://user-images.githubusercontent.com/15331990/217670791-ecce97ef-8f14-4519-85b7-40cd28ac2325.png">
-    <br>
     <a href="https://pypi.python.org/pypi/prefect-sqlalchemy/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-sqlalchemy?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-sqlalchemy/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-sqlalchemy?color=0052FF&labelColor=090422" /></a>
     <a href="https://pepy.tech/badge/prefect-sqlalchemy/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-sqlalchemy?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-sqlalchemy/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-sqlalchemy?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
 </p>
 
 Visit the full docs [here](https://PrefectHQ.github.io/prefect-sqlalchemy) to see additional examples and the API reference.
 
 The prefect-sqlalchemy collection makes it easy to connect to a database in your Prefect flows. Check out the examples below to get started!
 
-## Getting Started
+## Getting started
 
 ### Integrate with Prefect flows
 
-Prefect and SQLAlchemy are a data powerhouse duo. With Prefect, your data pipelines are always on track, and with SQLAlchemy, your databases are a snap to handle! Get ready to experience the ultimate data "flow-chemistry"!
+Prefect and SQLAlchemy are a data powerhouse duo. With Prefect, your workflows are orchestratable and observable, and with SQLAlchemy, your databases are a snap to handle! Get ready to experience the ultimate data "flow-chemistry"!
 
 To set up a table, use the `execute` and `execute_many` methods. Then, use the `fetch_many` method to retrieve data in a stream until there's no more data.
 
 By using the `SqlAlchemyConnector` as a context manager, you can make sure that the SQLAlchemy engine and any connected resources are closed properly after you're done with them.
 
-Be sure to install [prefect-sqlalchemy](#installation) and [save to block](#saving-credentials-to-block) to run the examples below!
+Be sure to install [prefect-sqlalchemy](#installation) and [save your credentials to a Prefect block](#saving-credentials-to-block) to run the examples below!
 
 !!! note "Async support"
 
-    `SqlAlchemyConnector` also supports async workflows! Just be sure to save, load, and use an async driver.
+    `SqlAlchemyConnector` also supports async workflows! Just be sure to save, load, and use an async driver as in the example below.
+
     ```python
     from prefect_sqlalchemy import SqlAlchemyConnector, ConnectionComponents, AsyncDriver
 
     connector = SqlAlchemyConnector(
         connection_info=ConnectionComponents(
             driver=AsyncDriver.SQLITE_AIOSQLITE,
             database="DATABASE-PLACEHOLDER.db"
@@ -166,15 +153,15 @@
                     {"name": "Unknown", "address": "Highway 42"},
                 ],
             )
 
     @task
     async def fetch_data(block_name: str) -> list:
         all_rows = []
-        async with SqlAlchemyConnector.load(block_name) as connector:
+        async with await SqlAlchemyConnector.load(block_name) as connector:
             while True:
                 # Repeated fetch* calls using the same operation will
                 # skip re-executing and instead return the next set of results
                 new_rows = await connector.fetch_many("SELECT * FROM customers", size=2)
                 if len(new_rows) == 0:
                     break
                 all_rows.append(new_rows)
@@ -188,35 +175,35 @@
 
 
     asyncio.run(sqlalchemy_flow("BLOCK-NAME-PLACEHOLDER"))
     ```
 
 ## Resources
 
-For more tips on how to use tasks and flows in a Collection, check out [Using Collections](https://orion-docs.prefect.io/collections/usage/)!
+For more tips on how to use tasks and flows provided in a Prefect integration library, check out the [Prefect docs on using integrations](https://docs.prefect.io/integrations/usage/).
 
 ### Installation
 
 Install `prefect-sqlalchemy` with `pip`:
 
 ```bash
 pip install prefect-sqlalchemy
 ```
 
-Requires an installation of Python 3.7+.
+Requires an installation of Python 3.8 or higher.
 
-We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
+We recommend using a Python virtual environment manager such as pipenv, conda, or virtualenv.
 
-These tasks are designed to work with Prefect 2.0. For more information about how to use Prefect, please refer to the [Prefect documentation](https://orion-docs.prefect.io/).
+The tasks in this library are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
-### Saving Credentials to Block
+### Saving credentials to a block
 
-To use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
+To use the `load` method on Blocks, you must have a block document [saved through code](https://docs.prefect.io/concepts/blocks/#saving-blocks) or saved through the UI.
 
-Below is a walkthrough on saving block documents through code; simply create a short script, replacing the placeholders. 
+Below is a walkthrough on saving block documents through code; simply create a short script, replacing the placeholders.
 
 ```python
 from prefect_sqlalchemy import SqlAlchemyConnector, ConnectionComponents, SyncDriver
 
 connector = SqlAlchemyConnector(
     connection_info=ConnectionComponents(
         driver=SyncDriver.POSTGRESQL_PSYCOPG2,
@@ -235,15 +222,15 @@
 
 ```python
 from prefect_sqlalchemy import SqlAlchemyConnector
 
 SqlAlchemyConnector.load("BLOCK_NAME-PLACEHOLDER")
 ```
 
-The required keywords depend on the desired `driver`. For example, sqlite only requires driver and database specified:
+The required keywords depend upon the desired driver. For example, SQLite requires only the `driver` and `database` arguments:
 
 ```python
 from prefect_sqlalchemy import SqlAlchemyConnector, ConnectionComponents, SyncDriver
 
 connector = SqlAlchemyConnector(
     connection_info=ConnectionComponents(
         driver=SyncDriver.SQLITE_PYSQLITE,
@@ -260,23 +247,20 @@
     [view and edit them](https://orion-docs.prefect.io/ui/blocks/)
     on Prefect Cloud:
 
     ```bash
     prefect block register -m prefect_sqlalchemy
     ```
 
-A list of available blocks in `prefect-sqlalchemy` and their setup instructions can be found [here](https://PrefectHQ.github.io/prefect-sqlalchemy/blocks_catalog).
-
 ### Feedback
 
-If you encounter any bugs while using `prefect-sqlalchemy`, feel free to open an issue in the [prefect-sqlalchemy](https://github.com/PrefectHQ/prefect-sqlalchemy) repository.
+If you encounter any bugs while using `prefect-sqlalchemy`, please open an issue in the [prefect](https://github.com/PrefectHQ/prefect) repository.
 
-If you have any questions or issues while using `prefect-sqlalchemy`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
+If you have any questions or issues while using `prefect-sqlalchemy`, you can find help in the [Prefect Community Slack ](https://prefect.io/slack).
 
-Feel free to star or watch [`prefect-sqlalchemy`](https://github.com/PrefectHQ/prefect-sqlalchemy) for updates too!
 
 ### Contributing
 
 If you'd like to help contribute to fix an issue or add a feature to `prefect-sqlalchemy`, please [propose changes through a pull request from a fork of the repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
 
 Here are the steps:
 
@@ -284,13 +268,12 @@
 2. [Clone the forked repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)
 3. Install the repository and its dependencies:
 ```
 pip install -e ".[dev]"
 ```
 4. Make desired changes
 5. Add tests
-6. Insert an entry to [CHANGELOG.md](https://github.com/PrefectHQ/prefect-sqlalchemy/blob/main/CHANGELOG.md)
-7. Install `pre-commit` to perform quality checks prior to commit:
+6. Install `pre-commit` to perform quality checks prior to commit:
 ```
 pre-commit install
 ```
-8. `git commit`, `git push`, and create a pull request
+7. `git commit`, `git push`, and create a pull request
```

#### html2text {}

```diff
@@ -1,58 +1,50 @@
-Metadata-Version: 2.1 Name: prefect-sqlalchemy Version: 0.4.0 Summary: Prefect
-integrations for interacting with SQLAlchemy. Home-page: https://github.com/
-PrefectHQ/prefect-sqlalchemy Author: Prefect Technologies, Inc. Author-email:
-help@prefect.io License: Apache License 2.0 Keywords: prefect Classifier:
-Natural Language :: English Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators Classifier: License ::
-OSI Approved :: Apache Software License Classifier: Programming Language ::
-Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries Requires-Python: >=3.7
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-prefect>=2.13.5 Requires-Dist: sqlalchemy<3,>=1.4.31 Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev" Requires-Dist: black; extra == "dev"
-Requires-Dist: flake8; extra == "dev" Requires-Dist: mypy; extra == "dev"
-Requires-Dist: mkdocs; extra == "dev" Requires-Dist: mkdocs-material; extra ==
-"dev" Requires-Dist: mkdocstrings[python]; extra == "dev" Requires-Dist: isort;
-extra == "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist: pytest-
-asyncio; extra == "dev" Requires-Dist: mock; python_version < "3.8" and extra
-== "dev" Requires-Dist: mkdocs-gen-files; extra == "dev" Requires-Dist:
-interrogate; extra == "dev" Requires-Dist: coverage; extra == "dev" Requires-
-Dist: psycopg2; extra == "dev" Requires-Dist: asyncpg; extra == "dev" Requires-
-Dist: aiosqlite; extra == "dev" Requires-Dist: pillow; extra == "dev" #
-prefect-sqlalchemy
- [https://user-images.githubusercontent.com/15331990/217670791-ecce97ef-8f14-
-                          4519-85b7-40cd28ac2325.png]
-         _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_P_r_e_f_e_c_t_H_Q_/_p_r_e_f_e_c_t_-
-  _s_q_l_a_l_c_h_e_m_y_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/
-  _p_r_e_f_e_c_t_-_s_q_l_a_l_c_h_e_m_y_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-                  _g_i_t_h_u_b_/_c_o_m_m_i_t_-_a_c_t_i_v_i_t_y_/_m_/_P_r_e_f_e_c_t_H_Q_/_p_r_e_f_e_c_t_-
+Metadata-Version: 2.1 Name: prefect-sqlalchemy Version: 0.4.1 Summary: Prefect
+integrations for working with databases Author-email: "Prefect Technologies,
+Inc."
+prefect.io> License: Apache License 2.0 Project-URL: Homepage, https://
+github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-sqlalchemy
+Keywords: prefect Classifier: Natural Language :: English Classifier: Intended
+Audience :: Developers Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Topic :: Software Development :: Libraries Requires-Python: >=3.8 Description-
+Content-Type: text/markdown Requires-Dist: sqlalchemy<3,>=1.4.31 Requires-Dist:
+prefect>=2.13.5 Provides-Extra: dev Requires-Dist: aiosqlite; extra == "dev"
+Requires-Dist: asyncpg; extra == "dev" Requires-Dist: coverage; extra == "dev"
+Requires-Dist: interrogate; extra == "dev" Requires-Dist: mkdocs-gen-files;
+extra == "dev" Requires-Dist: mkdocs-material; extra == "dev" Requires-Dist:
+mkdocs; extra == "dev" Requires-Dist: mkdocstrings[python]; extra == "dev"
+Requires-Dist: mock; python_version < "3.8" and extra == "dev" Requires-Dist:
+mypy; extra == "dev" Requires-Dist: pillow; extra == "dev" Requires-Dist: pre-
+commit; extra == "dev" Requires-Dist: psycopg2; extra == "dev" Requires-Dist:
+pytest-asyncio; extra == "dev" Requires-Dist: pytest-xdist; extra == "dev"
+Requires-Dist: pytest; extra == "dev" # prefect-sqlalchemy
+                _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_p_r_e_f_e_c_t_-
                   _s_q_l_a_l_c_h_e_m_y_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]
-              _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_s_l_a_c_k_-_j_o_i_n___c_o_m_m_u_n_i_t_y_-
-  _r_e_d_._s_v_g_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_&_l_o_g_o_=_s_l_a_c_k_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-                         _b_a_d_g_e_/_d_i_s_c_o_u_r_s_e_-_b_r_o_w_s_e___f_o_r_u_m_-
-            _r_e_d_._s_v_g_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_&_l_o_g_o_=_d_i_s_c_o_u_r_s_e_]
 Visit the full docs [here](https://PrefectHQ.github.io/prefect-sqlalchemy) to
 see additional examples and the API reference. The prefect-sqlalchemy
 collection makes it easy to connect to a database in your Prefect flows. Check
-out the examples below to get started! ## Getting Started ### Integrate with
+out the examples below to get started! ## Getting started ### Integrate with
 Prefect flows Prefect and SQLAlchemy are a data powerhouse duo. With Prefect,
-your data pipelines are always on track, and with SQLAlchemy, your databases
-are a snap to handle! Get ready to experience the ultimate data "flow-
-chemistry"! To set up a table, use the `execute` and `execute_many` methods.
-Then, use the `fetch_many` method to retrieve data in a stream until there's no
-more data. By using the `SqlAlchemyConnector` as a context manager, you can
-make sure that the SQLAlchemy engine and any connected resources are closed
-properly after you're done with them. Be sure to install [prefect-sqlalchemy]
-(#installation) and [save to block](#saving-credentials-to-block) to run the
-examples below! !!! note "Async support" `SqlAlchemyConnector` also supports
-async workflows! Just be sure to save, load, and use an async driver. ```python
-from prefect_sqlalchemy import SqlAlchemyConnector, ConnectionComponents,
+your workflows are orchestratable and observable, and with SQLAlchemy, your
+databases are a snap to handle! Get ready to experience the ultimate data
+"flow-chemistry"! To set up a table, use the `execute` and `execute_many`
+methods. Then, use the `fetch_many` method to retrieve data in a stream until
+there's no more data. By using the `SqlAlchemyConnector` as a context manager,
+you can make sure that the SQLAlchemy engine and any connected resources are
+closed properly after you're done with them. Be sure to install [prefect-
+sqlalchemy](#installation) and [save your credentials to a Prefect block]
+(#saving-credentials-to-block) to run the examples below! !!! note "Async
+support" `SqlAlchemyConnector` also supports async workflows! Just be sure to
+save, load, and use an async driver as in the example below. ```python from
+prefect_sqlalchemy import SqlAlchemyConnector, ConnectionComponents,
 AsyncDriver connector = SqlAlchemyConnector
 ( connection_info=ConnectionComponents( driver=AsyncDriver.SQLITE_AIOSQLITE,
 database="DATABASE-PLACEHOLDER.db" ) ) connector.save("BLOCK_NAME-PLACEHOLDER")
 ``` === "Sync" ```python from prefect import flow, task from prefect_sqlalchemy
 import SqlAlchemyConnector @task def setup_table(block_name: str) -> None: with
 SqlAlchemyConnector.load(block_name) as connector: connector.execute( "CREATE
 TABLE IF NOT EXISTS customers (name varchar, address varchar);" )
@@ -74,66 +66,59 @@
 (block_name) as connector: await connector.execute( "CREATE TABLE IF NOT EXISTS
 customers (name varchar, address varchar);" ) await connector.execute( "INSERT
 INTO customers (name, address) VALUES (:name, :address);", parameters={"name":
 "Marvin", "address": "Highway 42"}, ) await connector.execute_many( "INSERT
 INTO customers (name, address) VALUES (:name, :address);", seq_of_parameters=[
 {"name": "Ford", "address": "Highway 42"}, {"name": "Unknown", "address":
 "Highway 42"}, ], ) @task async def fetch_data(block_name: str) -> list:
-all_rows = [] async with SqlAlchemyConnector.load(block_name) as connector:
-while True: # Repeated fetch* calls using the same operation will # skip re-
-executing and instead return the next set of results new_rows = await
+all_rows = [] async with await SqlAlchemyConnector.load(block_name) as
+connector: while True: # Repeated fetch* calls using the same operation will #
+skip re-executing and instead return the next set of results new_rows = await
 connector.fetch_many("SELECT * FROM customers", size=2) if len(new_rows) == 0:
 break all_rows.append(new_rows) return all_rows @flow async def sqlalchemy_flow
 (block_name: str) -> list: await setup_table(block_name) all_rows = await
 fetch_data(block_name) return all_rows asyncio.run(sqlalchemy_flow("BLOCK-NAME-
-PLACEHOLDER")) ``` ## Resources For more tips on how to use tasks and flows in
-a Collection, check out [Using Collections](https://orion-docs.prefect.io/
-collections/usage/)! ### Installation Install `prefect-sqlalchemy` with `pip`:
-```bash pip install prefect-sqlalchemy ``` Requires an installation of Python
-3.7+. We recommend using a Python virtual environment manager such as pipenv,
-conda or virtualenv. These tasks are designed to work with Prefect 2.0. For
-more information about how to use Prefect, please refer to the [Prefect
-documentation](https://orion-docs.prefect.io/). ### Saving Credentials to Block
-To use the `load` method on Blocks, you must already have a block document
-[saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-
-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
-Below is a walkthrough on saving block documents through code; simply create a
-short script, replacing the placeholders. ```python from prefect_sqlalchemy
-import SqlAlchemyConnector, ConnectionComponents, SyncDriver connector =
+PLACEHOLDER")) ``` ## Resources For more tips on how to use tasks and flows
+provided in a Prefect integration library, check out the [Prefect docs on using
+integrations](https://docs.prefect.io/integrations/usage/). ### Installation
+Install `prefect-sqlalchemy` with `pip`: ```bash pip install prefect-sqlalchemy
+``` Requires an installation of Python 3.8 or higher. We recommend using a
+Python virtual environment manager such as pipenv, conda, or virtualenv. The
+tasks in this library are designed to work with Prefect 2. For more information
+about how to use Prefect, please refer to the [Prefect documentation](https://
+docs.prefect.io/). ### Saving credentials to a block To use the `load` method
+on Blocks, you must have a block document [saved through code](https://
+docs.prefect.io/concepts/blocks/#saving-blocks) or saved through the UI. Below
+is a walkthrough on saving block documents through code; simply create a short
+script, replacing the placeholders. ```python from prefect_sqlalchemy import
+SqlAlchemyConnector, ConnectionComponents, SyncDriver connector =
 SqlAlchemyConnector( connection_info=ConnectionComponents
 ( driver=SyncDriver.POSTGRESQL_PSYCOPG2, username="USERNAME-PLACEHOLDER",
 password="PASSWORD-PLACEHOLDER", host="localhost", port=5432,
 database="DATABASE-PLACEHOLDER", ) ) connector.save("BLOCK_NAME-PLACEHOLDER")
 ``` Congrats! You can now easily load the saved block, which holds your
 credentials: ```python from prefect_sqlalchemy import SqlAlchemyConnector
 SqlAlchemyConnector.load("BLOCK_NAME-PLACEHOLDER") ``` The required keywords
-depend on the desired `driver`. For example, sqlite only requires driver and
-database specified: ```python from prefect_sqlalchemy import
+depend upon the desired driver. For example, SQLite requires only the `driver`
+and `database` arguments: ```python from prefect_sqlalchemy import
 SqlAlchemyConnector, ConnectionComponents, SyncDriver connector =
 SqlAlchemyConnector( connection_info=ConnectionComponents
 ( driver=SyncDriver.SQLITE_PYSQLITE, database="DATABASE-PLACEHOLDER.db" ) )
 connector.save("BLOCK_NAME-PLACEHOLDER") ``` !!! info "Registering blocks"
 Register blocks in this module to [view and edit them](https://orion-
 docs.prefect.io/ui/blocks/) on Prefect Cloud: ```bash prefect block register -
-m prefect_sqlalchemy ``` A list of available blocks in `prefect-sqlalchemy` and
-their setup instructions can be found [here](https://PrefectHQ.github.io/
-prefect-sqlalchemy/blocks_catalog). ### Feedback If you encounter any bugs
-while using `prefect-sqlalchemy`, feel free to open an issue in the [prefect-
-sqlalchemy](https://github.com/PrefectHQ/prefect-sqlalchemy) repository. If you
-have any questions or issues while using `prefect-sqlalchemy`, you can find
-help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or
-the [Prefect Slack community](https://prefect.io/slack). Feel free to star or
-watch [`prefect-sqlalchemy`](https://github.com/PrefectHQ/prefect-sqlalchemy)
-for updates too! ### Contributing If you'd like to help contribute to fix an
-issue or add a feature to `prefect-sqlalchemy`, please [propose changes through
-a pull request from a fork of the repository](https://docs.github.com/en/pull-
-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-
-pull-requests/creating-a-pull-request-from-a-fork). Here are the steps: 1.
-[Fork the repository](https://docs.github.com/en/get-started/quickstart/fork-a-
-repo#forking-a-repository) 2. [Clone the forked repository](https://
-docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-
-repository) 3. Install the repository and its dependencies: ``` pip install -
-e ".[dev]" ``` 4. Make desired changes 5. Add tests 6. Insert an entry to
-[CHANGELOG.md](https://github.com/PrefectHQ/prefect-sqlalchemy/blob/main/
-CHANGELOG.md) 7. Install `pre-commit` to perform quality checks prior to
-commit: ``` pre-commit install ``` 8. `git commit`, `git push`, and create a
-pull request
+m prefect_sqlalchemy ``` ### Feedback If you encounter any bugs while using
+`prefect-sqlalchemy`, please open an issue in the [prefect](https://github.com/
+PrefectHQ/prefect) repository. If you have any questions or issues while using
+`prefect-sqlalchemy`, you can find help in the [Prefect Community Slack ]
+(https://prefect.io/slack). ### Contributing If you'd like to help contribute
+to fix an issue or add a feature to `prefect-sqlalchemy`, please [propose
+changes through a pull request from a fork of the repository](https://
+docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-
+changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
+Here are the steps: 1. [Fork the repository](https://docs.github.com/en/get-
+started/quickstart/fork-a-repo#forking-a-repository) 2. [Clone the forked
+repository](https://docs.github.com/en/get-started/quickstart/fork-a-
+repo#cloning-your-forked-repository) 3. Install the repository and its
+dependencies: ``` pip install -e ".[dev]" ``` 4. Make desired changes 5. Add
+tests 6. Install `pre-commit` to perform quality checks prior to commit: ```
+pre-commit install ``` 7. `git commit`, `git push`, and create a pull request
```

### Comparing `prefect-sqlalchemy-0.4.0/README.md` & `prefect_sqlalchemy-0.4.1/prefect_sqlalchemy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,77 @@
+Metadata-Version: 2.1
+Name: prefect-sqlalchemy
+Version: 0.4.1
+Summary: Prefect integrations for working with databases
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
+License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-sqlalchemy
+Keywords: prefect
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Requires-Dist: sqlalchemy<3,>=1.4.31
+Requires-Dist: prefect>=2.13.5
+Provides-Extra: dev
+Requires-Dist: aiosqlite; extra == "dev"
+Requires-Dist: asyncpg; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: interrogate; extra == "dev"
+Requires-Dist: mkdocs-gen-files; extra == "dev"
+Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
+Requires-Dist: mkdocstrings[python]; extra == "dev"
+Requires-Dist: mock; python_version < "3.8" and extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pillow; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: psycopg2; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+
 # prefect-sqlalchemy
 
 <p align="center">
-    <img src="https://user-images.githubusercontent.com/15331990/217670791-ecce97ef-8f14-4519-85b7-40cd28ac2325.png">
-    <br>
     <a href="https://pypi.python.org/pypi/prefect-sqlalchemy/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-sqlalchemy?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-sqlalchemy/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-sqlalchemy?color=0052FF&labelColor=090422" /></a>
     <a href="https://pepy.tech/badge/prefect-sqlalchemy/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-sqlalchemy?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-sqlalchemy/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-sqlalchemy?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
 </p>
 
 Visit the full docs [here](https://PrefectHQ.github.io/prefect-sqlalchemy) to see additional examples and the API reference.
 
 The prefect-sqlalchemy collection makes it easy to connect to a database in your Prefect flows. Check out the examples below to get started!
 
-## Getting Started
+## Getting started
 
 ### Integrate with Prefect flows
 
-Prefect and SQLAlchemy are a data powerhouse duo. With Prefect, your data pipelines are always on track, and with SQLAlchemy, your databases are a snap to handle! Get ready to experience the ultimate data "flow-chemistry"!
+Prefect and SQLAlchemy are a data powerhouse duo. With Prefect, your workflows are orchestratable and observable, and with SQLAlchemy, your databases are a snap to handle! Get ready to experience the ultimate data "flow-chemistry"!
 
 To set up a table, use the `execute` and `execute_many` methods. Then, use the `fetch_many` method to retrieve data in a stream until there's no more data.
 
 By using the `SqlAlchemyConnector` as a context manager, you can make sure that the SQLAlchemy engine and any connected resources are closed properly after you're done with them.
 
-Be sure to install [prefect-sqlalchemy](#installation) and [save to block](#saving-credentials-to-block) to run the examples below!
+Be sure to install [prefect-sqlalchemy](#installation) and [save your credentials to a Prefect block](#saving-credentials-to-block) to run the examples below!
 
 !!! note "Async support"
 
-    `SqlAlchemyConnector` also supports async workflows! Just be sure to save, load, and use an async driver.
+    `SqlAlchemyConnector` also supports async workflows! Just be sure to save, load, and use an async driver as in the example below.
+
     ```python
     from prefect_sqlalchemy import SqlAlchemyConnector, ConnectionComponents, AsyncDriver
 
     connector = SqlAlchemyConnector(
         connection_info=ConnectionComponents(
             driver=AsyncDriver.SQLITE_AIOSQLITE,
             database="DATABASE-PLACEHOLDER.db"
@@ -122,15 +153,15 @@
                     {"name": "Unknown", "address": "Highway 42"},
                 ],
             )
 
     @task
     async def fetch_data(block_name: str) -> list:
         all_rows = []
-        async with SqlAlchemyConnector.load(block_name) as connector:
+        async with await SqlAlchemyConnector.load(block_name) as connector:
             while True:
                 # Repeated fetch* calls using the same operation will
                 # skip re-executing and instead return the next set of results
                 new_rows = await connector.fetch_many("SELECT * FROM customers", size=2)
                 if len(new_rows) == 0:
                     break
                 all_rows.append(new_rows)
@@ -144,35 +175,35 @@
 
 
     asyncio.run(sqlalchemy_flow("BLOCK-NAME-PLACEHOLDER"))
     ```
 
 ## Resources
 
-For more tips on how to use tasks and flows in a Collection, check out [Using Collections](https://orion-docs.prefect.io/collections/usage/)!
+For more tips on how to use tasks and flows provided in a Prefect integration library, check out the [Prefect docs on using integrations](https://docs.prefect.io/integrations/usage/).
 
 ### Installation
 
 Install `prefect-sqlalchemy` with `pip`:
 
 ```bash
 pip install prefect-sqlalchemy
 ```
 
-Requires an installation of Python 3.7+.
+Requires an installation of Python 3.8 or higher.
 
-We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
+We recommend using a Python virtual environment manager such as pipenv, conda, or virtualenv.
 
-These tasks are designed to work with Prefect 2.0. For more information about how to use Prefect, please refer to the [Prefect documentation](https://orion-docs.prefect.io/).
+The tasks in this library are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
-### Saving Credentials to Block
+### Saving credentials to a block
 
-To use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
+To use the `load` method on Blocks, you must have a block document [saved through code](https://docs.prefect.io/concepts/blocks/#saving-blocks) or saved through the UI.
 
-Below is a walkthrough on saving block documents through code; simply create a short script, replacing the placeholders. 
+Below is a walkthrough on saving block documents through code; simply create a short script, replacing the placeholders.
 
 ```python
 from prefect_sqlalchemy import SqlAlchemyConnector, ConnectionComponents, SyncDriver
 
 connector = SqlAlchemyConnector(
     connection_info=ConnectionComponents(
         driver=SyncDriver.POSTGRESQL_PSYCOPG2,
@@ -191,15 +222,15 @@
 
 ```python
 from prefect_sqlalchemy import SqlAlchemyConnector
 
 SqlAlchemyConnector.load("BLOCK_NAME-PLACEHOLDER")
 ```
 
-The required keywords depend on the desired `driver`. For example, sqlite only requires driver and database specified:
+The required keywords depend upon the desired driver. For example, SQLite requires only the `driver` and `database` arguments:
 
 ```python
 from prefect_sqlalchemy import SqlAlchemyConnector, ConnectionComponents, SyncDriver
 
 connector = SqlAlchemyConnector(
     connection_info=ConnectionComponents(
         driver=SyncDriver.SQLITE_PYSQLITE,
@@ -216,23 +247,20 @@
     [view and edit them](https://orion-docs.prefect.io/ui/blocks/)
     on Prefect Cloud:
 
     ```bash
     prefect block register -m prefect_sqlalchemy
     ```
 
-A list of available blocks in `prefect-sqlalchemy` and their setup instructions can be found [here](https://PrefectHQ.github.io/prefect-sqlalchemy/blocks_catalog).
-
 ### Feedback
 
-If you encounter any bugs while using `prefect-sqlalchemy`, feel free to open an issue in the [prefect-sqlalchemy](https://github.com/PrefectHQ/prefect-sqlalchemy) repository.
+If you encounter any bugs while using `prefect-sqlalchemy`, please open an issue in the [prefect](https://github.com/PrefectHQ/prefect) repository.
 
-If you have any questions or issues while using `prefect-sqlalchemy`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
+If you have any questions or issues while using `prefect-sqlalchemy`, you can find help in the [Prefect Community Slack ](https://prefect.io/slack).
 
-Feel free to star or watch [`prefect-sqlalchemy`](https://github.com/PrefectHQ/prefect-sqlalchemy) for updates too!
 
 ### Contributing
 
 If you'd like to help contribute to fix an issue or add a feature to `prefect-sqlalchemy`, please [propose changes through a pull request from a fork of the repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
 
 Here are the steps:
 
@@ -240,13 +268,12 @@
 2. [Clone the forked repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)
 3. Install the repository and its dependencies:
 ```
 pip install -e ".[dev]"
 ```
 4. Make desired changes
 5. Add tests
-6. Insert an entry to [CHANGELOG.md](https://github.com/PrefectHQ/prefect-sqlalchemy/blob/main/CHANGELOG.md)
-7. Install `pre-commit` to perform quality checks prior to commit:
+6. Install `pre-commit` to perform quality checks prior to commit:
 ```
 pre-commit install
 ```
-8. `git commit`, `git push`, and create a pull request
+7. `git commit`, `git push`, and create a pull request
```

#### html2text {}

```diff
@@ -1,35 +1,50 @@
-# prefect-sqlalchemy
- [https://user-images.githubusercontent.com/15331990/217670791-ecce97ef-8f14-
-                          4519-85b7-40cd28ac2325.png]
-         _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_P_r_e_f_e_c_t_H_Q_/_p_r_e_f_e_c_t_-
-  _s_q_l_a_l_c_h_e_m_y_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/
-  _p_r_e_f_e_c_t_-_s_q_l_a_l_c_h_e_m_y_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-                  _g_i_t_h_u_b_/_c_o_m_m_i_t_-_a_c_t_i_v_i_t_y_/_m_/_P_r_e_f_e_c_t_H_Q_/_p_r_e_f_e_c_t_-
+Metadata-Version: 2.1 Name: prefect-sqlalchemy Version: 0.4.1 Summary: Prefect
+integrations for working with databases Author-email: "Prefect Technologies,
+Inc."
+prefect.io> License: Apache License 2.0 Project-URL: Homepage, https://
+github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-sqlalchemy
+Keywords: prefect Classifier: Natural Language :: English Classifier: Intended
+Audience :: Developers Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Topic :: Software Development :: Libraries Requires-Python: >=3.8 Description-
+Content-Type: text/markdown Requires-Dist: sqlalchemy<3,>=1.4.31 Requires-Dist:
+prefect>=2.13.5 Provides-Extra: dev Requires-Dist: aiosqlite; extra == "dev"
+Requires-Dist: asyncpg; extra == "dev" Requires-Dist: coverage; extra == "dev"
+Requires-Dist: interrogate; extra == "dev" Requires-Dist: mkdocs-gen-files;
+extra == "dev" Requires-Dist: mkdocs-material; extra == "dev" Requires-Dist:
+mkdocs; extra == "dev" Requires-Dist: mkdocstrings[python]; extra == "dev"
+Requires-Dist: mock; python_version < "3.8" and extra == "dev" Requires-Dist:
+mypy; extra == "dev" Requires-Dist: pillow; extra == "dev" Requires-Dist: pre-
+commit; extra == "dev" Requires-Dist: psycopg2; extra == "dev" Requires-Dist:
+pytest-asyncio; extra == "dev" Requires-Dist: pytest-xdist; extra == "dev"
+Requires-Dist: pytest; extra == "dev" # prefect-sqlalchemy
+                _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_p_r_e_f_e_c_t_-
                   _s_q_l_a_l_c_h_e_m_y_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]
-              _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_s_l_a_c_k_-_j_o_i_n___c_o_m_m_u_n_i_t_y_-
-  _r_e_d_._s_v_g_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_&_l_o_g_o_=_s_l_a_c_k_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-                         _b_a_d_g_e_/_d_i_s_c_o_u_r_s_e_-_b_r_o_w_s_e___f_o_r_u_m_-
-            _r_e_d_._s_v_g_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_&_l_o_g_o_=_d_i_s_c_o_u_r_s_e_]
 Visit the full docs [here](https://PrefectHQ.github.io/prefect-sqlalchemy) to
 see additional examples and the API reference. The prefect-sqlalchemy
 collection makes it easy to connect to a database in your Prefect flows. Check
-out the examples below to get started! ## Getting Started ### Integrate with
+out the examples below to get started! ## Getting started ### Integrate with
 Prefect flows Prefect and SQLAlchemy are a data powerhouse duo. With Prefect,
-your data pipelines are always on track, and with SQLAlchemy, your databases
-are a snap to handle! Get ready to experience the ultimate data "flow-
-chemistry"! To set up a table, use the `execute` and `execute_many` methods.
-Then, use the `fetch_many` method to retrieve data in a stream until there's no
-more data. By using the `SqlAlchemyConnector` as a context manager, you can
-make sure that the SQLAlchemy engine and any connected resources are closed
-properly after you're done with them. Be sure to install [prefect-sqlalchemy]
-(#installation) and [save to block](#saving-credentials-to-block) to run the
-examples below! !!! note "Async support" `SqlAlchemyConnector` also supports
-async workflows! Just be sure to save, load, and use an async driver. ```python
-from prefect_sqlalchemy import SqlAlchemyConnector, ConnectionComponents,
+your workflows are orchestratable and observable, and with SQLAlchemy, your
+databases are a snap to handle! Get ready to experience the ultimate data
+"flow-chemistry"! To set up a table, use the `execute` and `execute_many`
+methods. Then, use the `fetch_many` method to retrieve data in a stream until
+there's no more data. By using the `SqlAlchemyConnector` as a context manager,
+you can make sure that the SQLAlchemy engine and any connected resources are
+closed properly after you're done with them. Be sure to install [prefect-
+sqlalchemy](#installation) and [save your credentials to a Prefect block]
+(#saving-credentials-to-block) to run the examples below! !!! note "Async
+support" `SqlAlchemyConnector` also supports async workflows! Just be sure to
+save, load, and use an async driver as in the example below. ```python from
+prefect_sqlalchemy import SqlAlchemyConnector, ConnectionComponents,
 AsyncDriver connector = SqlAlchemyConnector
 ( connection_info=ConnectionComponents( driver=AsyncDriver.SQLITE_AIOSQLITE,
 database="DATABASE-PLACEHOLDER.db" ) ) connector.save("BLOCK_NAME-PLACEHOLDER")
 ``` === "Sync" ```python from prefect import flow, task from prefect_sqlalchemy
 import SqlAlchemyConnector @task def setup_table(block_name: str) -> None: with
 SqlAlchemyConnector.load(block_name) as connector: connector.execute( "CREATE
 TABLE IF NOT EXISTS customers (name varchar, address varchar);" )
@@ -51,66 +66,59 @@
 (block_name) as connector: await connector.execute( "CREATE TABLE IF NOT EXISTS
 customers (name varchar, address varchar);" ) await connector.execute( "INSERT
 INTO customers (name, address) VALUES (:name, :address);", parameters={"name":
 "Marvin", "address": "Highway 42"}, ) await connector.execute_many( "INSERT
 INTO customers (name, address) VALUES (:name, :address);", seq_of_parameters=[
 {"name": "Ford", "address": "Highway 42"}, {"name": "Unknown", "address":
 "Highway 42"}, ], ) @task async def fetch_data(block_name: str) -> list:
-all_rows = [] async with SqlAlchemyConnector.load(block_name) as connector:
-while True: # Repeated fetch* calls using the same operation will # skip re-
-executing and instead return the next set of results new_rows = await
+all_rows = [] async with await SqlAlchemyConnector.load(block_name) as
+connector: while True: # Repeated fetch* calls using the same operation will #
+skip re-executing and instead return the next set of results new_rows = await
 connector.fetch_many("SELECT * FROM customers", size=2) if len(new_rows) == 0:
 break all_rows.append(new_rows) return all_rows @flow async def sqlalchemy_flow
 (block_name: str) -> list: await setup_table(block_name) all_rows = await
 fetch_data(block_name) return all_rows asyncio.run(sqlalchemy_flow("BLOCK-NAME-
-PLACEHOLDER")) ``` ## Resources For more tips on how to use tasks and flows in
-a Collection, check out [Using Collections](https://orion-docs.prefect.io/
-collections/usage/)! ### Installation Install `prefect-sqlalchemy` with `pip`:
-```bash pip install prefect-sqlalchemy ``` Requires an installation of Python
-3.7+. We recommend using a Python virtual environment manager such as pipenv,
-conda or virtualenv. These tasks are designed to work with Prefect 2.0. For
-more information about how to use Prefect, please refer to the [Prefect
-documentation](https://orion-docs.prefect.io/). ### Saving Credentials to Block
-To use the `load` method on Blocks, you must already have a block document
-[saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-
-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
-Below is a walkthrough on saving block documents through code; simply create a
-short script, replacing the placeholders. ```python from prefect_sqlalchemy
-import SqlAlchemyConnector, ConnectionComponents, SyncDriver connector =
+PLACEHOLDER")) ``` ## Resources For more tips on how to use tasks and flows
+provided in a Prefect integration library, check out the [Prefect docs on using
+integrations](https://docs.prefect.io/integrations/usage/). ### Installation
+Install `prefect-sqlalchemy` with `pip`: ```bash pip install prefect-sqlalchemy
+``` Requires an installation of Python 3.8 or higher. We recommend using a
+Python virtual environment manager such as pipenv, conda, or virtualenv. The
+tasks in this library are designed to work with Prefect 2. For more information
+about how to use Prefect, please refer to the [Prefect documentation](https://
+docs.prefect.io/). ### Saving credentials to a block To use the `load` method
+on Blocks, you must have a block document [saved through code](https://
+docs.prefect.io/concepts/blocks/#saving-blocks) or saved through the UI. Below
+is a walkthrough on saving block documents through code; simply create a short
+script, replacing the placeholders. ```python from prefect_sqlalchemy import
+SqlAlchemyConnector, ConnectionComponents, SyncDriver connector =
 SqlAlchemyConnector( connection_info=ConnectionComponents
 ( driver=SyncDriver.POSTGRESQL_PSYCOPG2, username="USERNAME-PLACEHOLDER",
 password="PASSWORD-PLACEHOLDER", host="localhost", port=5432,
 database="DATABASE-PLACEHOLDER", ) ) connector.save("BLOCK_NAME-PLACEHOLDER")
 ``` Congrats! You can now easily load the saved block, which holds your
 credentials: ```python from prefect_sqlalchemy import SqlAlchemyConnector
 SqlAlchemyConnector.load("BLOCK_NAME-PLACEHOLDER") ``` The required keywords
-depend on the desired `driver`. For example, sqlite only requires driver and
-database specified: ```python from prefect_sqlalchemy import
+depend upon the desired driver. For example, SQLite requires only the `driver`
+and `database` arguments: ```python from prefect_sqlalchemy import
 SqlAlchemyConnector, ConnectionComponents, SyncDriver connector =
 SqlAlchemyConnector( connection_info=ConnectionComponents
 ( driver=SyncDriver.SQLITE_PYSQLITE, database="DATABASE-PLACEHOLDER.db" ) )
 connector.save("BLOCK_NAME-PLACEHOLDER") ``` !!! info "Registering blocks"
 Register blocks in this module to [view and edit them](https://orion-
 docs.prefect.io/ui/blocks/) on Prefect Cloud: ```bash prefect block register -
-m prefect_sqlalchemy ``` A list of available blocks in `prefect-sqlalchemy` and
-their setup instructions can be found [here](https://PrefectHQ.github.io/
-prefect-sqlalchemy/blocks_catalog). ### Feedback If you encounter any bugs
-while using `prefect-sqlalchemy`, feel free to open an issue in the [prefect-
-sqlalchemy](https://github.com/PrefectHQ/prefect-sqlalchemy) repository. If you
-have any questions or issues while using `prefect-sqlalchemy`, you can find
-help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or
-the [Prefect Slack community](https://prefect.io/slack). Feel free to star or
-watch [`prefect-sqlalchemy`](https://github.com/PrefectHQ/prefect-sqlalchemy)
-for updates too! ### Contributing If you'd like to help contribute to fix an
-issue or add a feature to `prefect-sqlalchemy`, please [propose changes through
-a pull request from a fork of the repository](https://docs.github.com/en/pull-
-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-
-pull-requests/creating-a-pull-request-from-a-fork). Here are the steps: 1.
-[Fork the repository](https://docs.github.com/en/get-started/quickstart/fork-a-
-repo#forking-a-repository) 2. [Clone the forked repository](https://
-docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-
-repository) 3. Install the repository and its dependencies: ``` pip install -
-e ".[dev]" ``` 4. Make desired changes 5. Add tests 6. Insert an entry to
-[CHANGELOG.md](https://github.com/PrefectHQ/prefect-sqlalchemy/blob/main/
-CHANGELOG.md) 7. Install `pre-commit` to perform quality checks prior to
-commit: ``` pre-commit install ``` 8. `git commit`, `git push`, and create a
-pull request
+m prefect_sqlalchemy ``` ### Feedback If you encounter any bugs while using
+`prefect-sqlalchemy`, please open an issue in the [prefect](https://github.com/
+PrefectHQ/prefect) repository. If you have any questions or issues while using
+`prefect-sqlalchemy`, you can find help in the [Prefect Community Slack ]
+(https://prefect.io/slack). ### Contributing If you'd like to help contribute
+to fix an issue or add a feature to `prefect-sqlalchemy`, please [propose
+changes through a pull request from a fork of the repository](https://
+docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-
+changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
+Here are the steps: 1. [Fork the repository](https://docs.github.com/en/get-
+started/quickstart/fork-a-repo#forking-a-repository) 2. [Clone the forked
+repository](https://docs.github.com/en/get-started/quickstart/fork-a-
+repo#cloning-your-forked-repository) 3. Install the repository and its
+dependencies: ``` pip install -e ".[dev]" ``` 4. Make desired changes 5. Add
+tests 6. Install `pre-commit` to perform quality checks prior to commit: ```
+pre-commit install ``` 7. `git commit`, `git push`, and create a pull request
```

### Comparing `prefect-sqlalchemy-0.4.0/prefect_sqlalchemy/credentials.py` & `prefect_sqlalchemy-0.4.1/prefect_sqlalchemy/credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Credential classes used to perform authenticated interactions with SQLAlchemy"""
 
 import warnings
 from enum import Enum
 from typing import Any, Dict, Optional, Union
 
-from prefect.blocks.core import Block
 from pydantic import VERSION as PYDANTIC_VERSION
 
+from prefect.blocks.core import Block
+
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import AnyUrl, BaseModel, Field, SecretStr
 else:
     from pydantic import AnyUrl, BaseModel, Field, SecretStr
 
 from sqlalchemy.engine import Connection, create_engine
 from sqlalchemy.engine.url import URL, make_url
```

### Comparing `prefect-sqlalchemy-0.4.0/prefect_sqlalchemy/database.py` & `prefect_sqlalchemy-0.4.1/prefect_sqlalchemy/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Tasks for querying a database with SQLAlchemy"""
 
 import contextlib
 import warnings
 from contextlib import AsyncExitStack, ExitStack, asynccontextmanager
 from typing import Any, Dict, List, Optional, Tuple, Union
 
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect import task
 from prefect.blocks.abstract import CredentialsBlock, DatabaseBlock
 from prefect.utilities.asyncutils import sync_compatible
 from prefect.utilities.hashing import hash_objects
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import AnyUrl, Field, SecretStr
 else:
     from pydantic import AnyUrl, Field, SecretStr
 
 from sqlalchemy import __version__ as SQLALCHEMY_VERSION
```

### Comparing `prefect-sqlalchemy-0.4.0/prefect_sqlalchemy.egg-info/PKG-INFO` & `prefect_sqlalchemy-0.4.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,36 @@
-Metadata-Version: 2.1
-Name: prefect-sqlalchemy
-Version: 0.4.0
-Summary: Prefect integrations for interacting with SQLAlchemy.
-Home-page: https://github.com/PrefectHQ/prefect-sqlalchemy
-Author: Prefect Technologies, Inc.
-Author-email: help@prefect.io
-License: Apache License 2.0
-Keywords: prefect
-Classifier: Natural Language :: English
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: prefect>=2.13.5
-Requires-Dist: sqlalchemy<3,>=1.4.31
-Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: mkdocs; extra == "dev"
-Requires-Dist: mkdocs-material; extra == "dev"
-Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pytest-asyncio; extra == "dev"
-Requires-Dist: mock; python_version < "3.8" and extra == "dev"
-Requires-Dist: mkdocs-gen-files; extra == "dev"
-Requires-Dist: interrogate; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
-Requires-Dist: psycopg2; extra == "dev"
-Requires-Dist: asyncpg; extra == "dev"
-Requires-Dist: aiosqlite; extra == "dev"
-Requires-Dist: pillow; extra == "dev"
-
 # prefect-sqlalchemy
 
 <p align="center">
-    <img src="https://user-images.githubusercontent.com/15331990/217670791-ecce97ef-8f14-4519-85b7-40cd28ac2325.png">
-    <br>
     <a href="https://pypi.python.org/pypi/prefect-sqlalchemy/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-sqlalchemy?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-sqlalchemy/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-sqlalchemy?color=0052FF&labelColor=090422" /></a>
     <a href="https://pepy.tech/badge/prefect-sqlalchemy/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-sqlalchemy?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-sqlalchemy/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-sqlalchemy?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
 </p>
 
 Visit the full docs [here](https://PrefectHQ.github.io/prefect-sqlalchemy) to see additional examples and the API reference.
 
 The prefect-sqlalchemy collection makes it easy to connect to a database in your Prefect flows. Check out the examples below to get started!
 
-## Getting Started
+## Getting started
 
 ### Integrate with Prefect flows
 
-Prefect and SQLAlchemy are a data powerhouse duo. With Prefect, your data pipelines are always on track, and with SQLAlchemy, your databases are a snap to handle! Get ready to experience the ultimate data "flow-chemistry"!
+Prefect and SQLAlchemy are a data powerhouse duo. With Prefect, your workflows are orchestratable and observable, and with SQLAlchemy, your databases are a snap to handle! Get ready to experience the ultimate data "flow-chemistry"!
 
 To set up a table, use the `execute` and `execute_many` methods. Then, use the `fetch_many` method to retrieve data in a stream until there's no more data.
 
 By using the `SqlAlchemyConnector` as a context manager, you can make sure that the SQLAlchemy engine and any connected resources are closed properly after you're done with them.
 
-Be sure to install [prefect-sqlalchemy](#installation) and [save to block](#saving-credentials-to-block) to run the examples below!
+Be sure to install [prefect-sqlalchemy](#installation) and [save your credentials to a Prefect block](#saving-credentials-to-block) to run the examples below!
 
 !!! note "Async support"
 
-    `SqlAlchemyConnector` also supports async workflows! Just be sure to save, load, and use an async driver.
+    `SqlAlchemyConnector` also supports async workflows! Just be sure to save, load, and use an async driver as in the example below.
+
     ```python
     from prefect_sqlalchemy import SqlAlchemyConnector, ConnectionComponents, AsyncDriver
 
     connector = SqlAlchemyConnector(
         connection_info=ConnectionComponents(
             driver=AsyncDriver.SQLITE_AIOSQLITE,
             database="DATABASE-PLACEHOLDER.db"
@@ -166,15 +112,15 @@
                     {"name": "Unknown", "address": "Highway 42"},
                 ],
             )
 
     @task
     async def fetch_data(block_name: str) -> list:
         all_rows = []
-        async with SqlAlchemyConnector.load(block_name) as connector:
+        async with await SqlAlchemyConnector.load(block_name) as connector:
             while True:
                 # Repeated fetch* calls using the same operation will
                 # skip re-executing and instead return the next set of results
                 new_rows = await connector.fetch_many("SELECT * FROM customers", size=2)
                 if len(new_rows) == 0:
                     break
                 all_rows.append(new_rows)
@@ -188,35 +134,35 @@
 
 
     asyncio.run(sqlalchemy_flow("BLOCK-NAME-PLACEHOLDER"))
     ```
 
 ## Resources
 
-For more tips on how to use tasks and flows in a Collection, check out [Using Collections](https://orion-docs.prefect.io/collections/usage/)!
+For more tips on how to use tasks and flows provided in a Prefect integration library, check out the [Prefect docs on using integrations](https://docs.prefect.io/integrations/usage/).
 
 ### Installation
 
 Install `prefect-sqlalchemy` with `pip`:
 
 ```bash
 pip install prefect-sqlalchemy
 ```
 
-Requires an installation of Python 3.7+.
+Requires an installation of Python 3.8 or higher.
 
-We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
+We recommend using a Python virtual environment manager such as pipenv, conda, or virtualenv.
 
-These tasks are designed to work with Prefect 2.0. For more information about how to use Prefect, please refer to the [Prefect documentation](https://orion-docs.prefect.io/).
+The tasks in this library are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
-### Saving Credentials to Block
+### Saving credentials to a block
 
-To use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
+To use the `load` method on Blocks, you must have a block document [saved through code](https://docs.prefect.io/concepts/blocks/#saving-blocks) or saved through the UI.
 
-Below is a walkthrough on saving block documents through code; simply create a short script, replacing the placeholders. 
+Below is a walkthrough on saving block documents through code; simply create a short script, replacing the placeholders.
 
 ```python
 from prefect_sqlalchemy import SqlAlchemyConnector, ConnectionComponents, SyncDriver
 
 connector = SqlAlchemyConnector(
     connection_info=ConnectionComponents(
         driver=SyncDriver.POSTGRESQL_PSYCOPG2,
@@ -235,15 +181,15 @@
 
 ```python
 from prefect_sqlalchemy import SqlAlchemyConnector
 
 SqlAlchemyConnector.load("BLOCK_NAME-PLACEHOLDER")
 ```
 
-The required keywords depend on the desired `driver`. For example, sqlite only requires driver and database specified:
+The required keywords depend upon the desired driver. For example, SQLite requires only the `driver` and `database` arguments:
 
 ```python
 from prefect_sqlalchemy import SqlAlchemyConnector, ConnectionComponents, SyncDriver
 
 connector = SqlAlchemyConnector(
     connection_info=ConnectionComponents(
         driver=SyncDriver.SQLITE_PYSQLITE,
@@ -260,23 +206,20 @@
     [view and edit them](https://orion-docs.prefect.io/ui/blocks/)
     on Prefect Cloud:
 
     ```bash
     prefect block register -m prefect_sqlalchemy
     ```
 
-A list of available blocks in `prefect-sqlalchemy` and their setup instructions can be found [here](https://PrefectHQ.github.io/prefect-sqlalchemy/blocks_catalog).
-
 ### Feedback
 
-If you encounter any bugs while using `prefect-sqlalchemy`, feel free to open an issue in the [prefect-sqlalchemy](https://github.com/PrefectHQ/prefect-sqlalchemy) repository.
+If you encounter any bugs while using `prefect-sqlalchemy`, please open an issue in the [prefect](https://github.com/PrefectHQ/prefect) repository.
 
-If you have any questions or issues while using `prefect-sqlalchemy`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
+If you have any questions or issues while using `prefect-sqlalchemy`, you can find help in the [Prefect Community Slack ](https://prefect.io/slack).
 
-Feel free to star or watch [`prefect-sqlalchemy`](https://github.com/PrefectHQ/prefect-sqlalchemy) for updates too!
 
 ### Contributing
 
 If you'd like to help contribute to fix an issue or add a feature to `prefect-sqlalchemy`, please [propose changes through a pull request from a fork of the repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
 
 Here are the steps:
 
@@ -284,13 +227,12 @@
 2. [Clone the forked repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)
 3. Install the repository and its dependencies:
 ```
 pip install -e ".[dev]"
 ```
 4. Make desired changes
 5. Add tests
-6. Insert an entry to [CHANGELOG.md](https://github.com/PrefectHQ/prefect-sqlalchemy/blob/main/CHANGELOG.md)
-7. Install `pre-commit` to perform quality checks prior to commit:
+6. Install `pre-commit` to perform quality checks prior to commit:
 ```
 pre-commit install
 ```
-8. `git commit`, `git push`, and create a pull request
+7. `git commit`, `git push`, and create a pull request
```

#### html2text {}

```diff
@@ -1,58 +1,27 @@
-Metadata-Version: 2.1 Name: prefect-sqlalchemy Version: 0.4.0 Summary: Prefect
-integrations for interacting with SQLAlchemy. Home-page: https://github.com/
-PrefectHQ/prefect-sqlalchemy Author: Prefect Technologies, Inc. Author-email:
-help@prefect.io License: Apache License 2.0 Keywords: prefect Classifier:
-Natural Language :: English Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators Classifier: License ::
-OSI Approved :: Apache Software License Classifier: Programming Language ::
-Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries Requires-Python: >=3.7
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-prefect>=2.13.5 Requires-Dist: sqlalchemy<3,>=1.4.31 Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev" Requires-Dist: black; extra == "dev"
-Requires-Dist: flake8; extra == "dev" Requires-Dist: mypy; extra == "dev"
-Requires-Dist: mkdocs; extra == "dev" Requires-Dist: mkdocs-material; extra ==
-"dev" Requires-Dist: mkdocstrings[python]; extra == "dev" Requires-Dist: isort;
-extra == "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist: pytest-
-asyncio; extra == "dev" Requires-Dist: mock; python_version < "3.8" and extra
-== "dev" Requires-Dist: mkdocs-gen-files; extra == "dev" Requires-Dist:
-interrogate; extra == "dev" Requires-Dist: coverage; extra == "dev" Requires-
-Dist: psycopg2; extra == "dev" Requires-Dist: asyncpg; extra == "dev" Requires-
-Dist: aiosqlite; extra == "dev" Requires-Dist: pillow; extra == "dev" #
-prefect-sqlalchemy
- [https://user-images.githubusercontent.com/15331990/217670791-ecce97ef-8f14-
-                          4519-85b7-40cd28ac2325.png]
-         _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_P_r_e_f_e_c_t_H_Q_/_p_r_e_f_e_c_t_-
-  _s_q_l_a_l_c_h_e_m_y_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/
-  _p_r_e_f_e_c_t_-_s_q_l_a_l_c_h_e_m_y_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-                  _g_i_t_h_u_b_/_c_o_m_m_i_t_-_a_c_t_i_v_i_t_y_/_m_/_P_r_e_f_e_c_t_H_Q_/_p_r_e_f_e_c_t_-
+# prefect-sqlalchemy
+                _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_p_r_e_f_e_c_t_-
                   _s_q_l_a_l_c_h_e_m_y_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]
-              _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_s_l_a_c_k_-_j_o_i_n___c_o_m_m_u_n_i_t_y_-
-  _r_e_d_._s_v_g_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_&_l_o_g_o_=_s_l_a_c_k_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-                         _b_a_d_g_e_/_d_i_s_c_o_u_r_s_e_-_b_r_o_w_s_e___f_o_r_u_m_-
-            _r_e_d_._s_v_g_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_&_l_o_g_o_=_d_i_s_c_o_u_r_s_e_]
 Visit the full docs [here](https://PrefectHQ.github.io/prefect-sqlalchemy) to
 see additional examples and the API reference. The prefect-sqlalchemy
 collection makes it easy to connect to a database in your Prefect flows. Check
-out the examples below to get started! ## Getting Started ### Integrate with
+out the examples below to get started! ## Getting started ### Integrate with
 Prefect flows Prefect and SQLAlchemy are a data powerhouse duo. With Prefect,
-your data pipelines are always on track, and with SQLAlchemy, your databases
-are a snap to handle! Get ready to experience the ultimate data "flow-
-chemistry"! To set up a table, use the `execute` and `execute_many` methods.
-Then, use the `fetch_many` method to retrieve data in a stream until there's no
-more data. By using the `SqlAlchemyConnector` as a context manager, you can
-make sure that the SQLAlchemy engine and any connected resources are closed
-properly after you're done with them. Be sure to install [prefect-sqlalchemy]
-(#installation) and [save to block](#saving-credentials-to-block) to run the
-examples below! !!! note "Async support" `SqlAlchemyConnector` also supports
-async workflows! Just be sure to save, load, and use an async driver. ```python
-from prefect_sqlalchemy import SqlAlchemyConnector, ConnectionComponents,
+your workflows are orchestratable and observable, and with SQLAlchemy, your
+databases are a snap to handle! Get ready to experience the ultimate data
+"flow-chemistry"! To set up a table, use the `execute` and `execute_many`
+methods. Then, use the `fetch_many` method to retrieve data in a stream until
+there's no more data. By using the `SqlAlchemyConnector` as a context manager,
+you can make sure that the SQLAlchemy engine and any connected resources are
+closed properly after you're done with them. Be sure to install [prefect-
+sqlalchemy](#installation) and [save your credentials to a Prefect block]
+(#saving-credentials-to-block) to run the examples below! !!! note "Async
+support" `SqlAlchemyConnector` also supports async workflows! Just be sure to
+save, load, and use an async driver as in the example below. ```python from
+prefect_sqlalchemy import SqlAlchemyConnector, ConnectionComponents,
 AsyncDriver connector = SqlAlchemyConnector
 ( connection_info=ConnectionComponents( driver=AsyncDriver.SQLITE_AIOSQLITE,
 database="DATABASE-PLACEHOLDER.db" ) ) connector.save("BLOCK_NAME-PLACEHOLDER")
 ``` === "Sync" ```python from prefect import flow, task from prefect_sqlalchemy
 import SqlAlchemyConnector @task def setup_table(block_name: str) -> None: with
 SqlAlchemyConnector.load(block_name) as connector: connector.execute( "CREATE
 TABLE IF NOT EXISTS customers (name varchar, address varchar);" )
@@ -74,66 +43,59 @@
 (block_name) as connector: await connector.execute( "CREATE TABLE IF NOT EXISTS
 customers (name varchar, address varchar);" ) await connector.execute( "INSERT
 INTO customers (name, address) VALUES (:name, :address);", parameters={"name":
 "Marvin", "address": "Highway 42"}, ) await connector.execute_many( "INSERT
 INTO customers (name, address) VALUES (:name, :address);", seq_of_parameters=[
 {"name": "Ford", "address": "Highway 42"}, {"name": "Unknown", "address":
 "Highway 42"}, ], ) @task async def fetch_data(block_name: str) -> list:
-all_rows = [] async with SqlAlchemyConnector.load(block_name) as connector:
-while True: # Repeated fetch* calls using the same operation will # skip re-
-executing and instead return the next set of results new_rows = await
+all_rows = [] async with await SqlAlchemyConnector.load(block_name) as
+connector: while True: # Repeated fetch* calls using the same operation will #
+skip re-executing and instead return the next set of results new_rows = await
 connector.fetch_many("SELECT * FROM customers", size=2) if len(new_rows) == 0:
 break all_rows.append(new_rows) return all_rows @flow async def sqlalchemy_flow
 (block_name: str) -> list: await setup_table(block_name) all_rows = await
 fetch_data(block_name) return all_rows asyncio.run(sqlalchemy_flow("BLOCK-NAME-
-PLACEHOLDER")) ``` ## Resources For more tips on how to use tasks and flows in
-a Collection, check out [Using Collections](https://orion-docs.prefect.io/
-collections/usage/)! ### Installation Install `prefect-sqlalchemy` with `pip`:
-```bash pip install prefect-sqlalchemy ``` Requires an installation of Python
-3.7+. We recommend using a Python virtual environment manager such as pipenv,
-conda or virtualenv. These tasks are designed to work with Prefect 2.0. For
-more information about how to use Prefect, please refer to the [Prefect
-documentation](https://orion-docs.prefect.io/). ### Saving Credentials to Block
-To use the `load` method on Blocks, you must already have a block document
-[saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-
-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
-Below is a walkthrough on saving block documents through code; simply create a
-short script, replacing the placeholders. ```python from prefect_sqlalchemy
-import SqlAlchemyConnector, ConnectionComponents, SyncDriver connector =
+PLACEHOLDER")) ``` ## Resources For more tips on how to use tasks and flows
+provided in a Prefect integration library, check out the [Prefect docs on using
+integrations](https://docs.prefect.io/integrations/usage/). ### Installation
+Install `prefect-sqlalchemy` with `pip`: ```bash pip install prefect-sqlalchemy
+``` Requires an installation of Python 3.8 or higher. We recommend using a
+Python virtual environment manager such as pipenv, conda, or virtualenv. The
+tasks in this library are designed to work with Prefect 2. For more information
+about how to use Prefect, please refer to the [Prefect documentation](https://
+docs.prefect.io/). ### Saving credentials to a block To use the `load` method
+on Blocks, you must have a block document [saved through code](https://
+docs.prefect.io/concepts/blocks/#saving-blocks) or saved through the UI. Below
+is a walkthrough on saving block documents through code; simply create a short
+script, replacing the placeholders. ```python from prefect_sqlalchemy import
+SqlAlchemyConnector, ConnectionComponents, SyncDriver connector =
 SqlAlchemyConnector( connection_info=ConnectionComponents
 ( driver=SyncDriver.POSTGRESQL_PSYCOPG2, username="USERNAME-PLACEHOLDER",
 password="PASSWORD-PLACEHOLDER", host="localhost", port=5432,
 database="DATABASE-PLACEHOLDER", ) ) connector.save("BLOCK_NAME-PLACEHOLDER")
 ``` Congrats! You can now easily load the saved block, which holds your
 credentials: ```python from prefect_sqlalchemy import SqlAlchemyConnector
 SqlAlchemyConnector.load("BLOCK_NAME-PLACEHOLDER") ``` The required keywords
-depend on the desired `driver`. For example, sqlite only requires driver and
-database specified: ```python from prefect_sqlalchemy import
+depend upon the desired driver. For example, SQLite requires only the `driver`
+and `database` arguments: ```python from prefect_sqlalchemy import
 SqlAlchemyConnector, ConnectionComponents, SyncDriver connector =
 SqlAlchemyConnector( connection_info=ConnectionComponents
 ( driver=SyncDriver.SQLITE_PYSQLITE, database="DATABASE-PLACEHOLDER.db" ) )
 connector.save("BLOCK_NAME-PLACEHOLDER") ``` !!! info "Registering blocks"
 Register blocks in this module to [view and edit them](https://orion-
 docs.prefect.io/ui/blocks/) on Prefect Cloud: ```bash prefect block register -
-m prefect_sqlalchemy ``` A list of available blocks in `prefect-sqlalchemy` and
-their setup instructions can be found [here](https://PrefectHQ.github.io/
-prefect-sqlalchemy/blocks_catalog). ### Feedback If you encounter any bugs
-while using `prefect-sqlalchemy`, feel free to open an issue in the [prefect-
-sqlalchemy](https://github.com/PrefectHQ/prefect-sqlalchemy) repository. If you
-have any questions or issues while using `prefect-sqlalchemy`, you can find
-help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or
-the [Prefect Slack community](https://prefect.io/slack). Feel free to star or
-watch [`prefect-sqlalchemy`](https://github.com/PrefectHQ/prefect-sqlalchemy)
-for updates too! ### Contributing If you'd like to help contribute to fix an
-issue or add a feature to `prefect-sqlalchemy`, please [propose changes through
-a pull request from a fork of the repository](https://docs.github.com/en/pull-
-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-
-pull-requests/creating-a-pull-request-from-a-fork). Here are the steps: 1.
-[Fork the repository](https://docs.github.com/en/get-started/quickstart/fork-a-
-repo#forking-a-repository) 2. [Clone the forked repository](https://
-docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-
-repository) 3. Install the repository and its dependencies: ``` pip install -
-e ".[dev]" ``` 4. Make desired changes 5. Add tests 6. Insert an entry to
-[CHANGELOG.md](https://github.com/PrefectHQ/prefect-sqlalchemy/blob/main/
-CHANGELOG.md) 7. Install `pre-commit` to perform quality checks prior to
-commit: ``` pre-commit install ``` 8. `git commit`, `git push`, and create a
-pull request
+m prefect_sqlalchemy ``` ### Feedback If you encounter any bugs while using
+`prefect-sqlalchemy`, please open an issue in the [prefect](https://github.com/
+PrefectHQ/prefect) repository. If you have any questions or issues while using
+`prefect-sqlalchemy`, you can find help in the [Prefect Community Slack ]
+(https://prefect.io/slack). ### Contributing If you'd like to help contribute
+to fix an issue or add a feature to `prefect-sqlalchemy`, please [propose
+changes through a pull request from a fork of the repository](https://
+docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-
+changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
+Here are the steps: 1. [Fork the repository](https://docs.github.com/en/get-
+started/quickstart/fork-a-repo#forking-a-repository) 2. [Clone the forked
+repository](https://docs.github.com/en/get-started/quickstart/fork-a-
+repo#cloning-your-forked-repository) 3. Install the repository and its
+dependencies: ``` pip install -e ".[dev]" ``` 4. Make desired changes 5. Add
+tests 6. Install `pre-commit` to perform quality checks prior to commit: ```
+pre-commit install ``` 7. `git commit`, `git push`, and create a pull request
```

### Comparing `prefect-sqlalchemy-0.4.0/prefect_sqlalchemy.egg-info/SOURCES.txt` & `prefect_sqlalchemy-0.4.1/prefect_sqlalchemy.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-LICENSE
-MANIFEST.in
 README.md
-requirements-dev.txt
-requirements.txt
-setup.cfg
-setup.py
-versioneer.py
+pyproject.toml
 prefect_sqlalchemy/__init__.py
 prefect_sqlalchemy/_version.py
 prefect_sqlalchemy/credentials.py
 prefect_sqlalchemy/database.py
 prefect_sqlalchemy.egg-info/PKG-INFO
 prefect_sqlalchemy.egg-info/SOURCES.txt
 prefect_sqlalchemy.egg-info/dependency_links.txt
 prefect_sqlalchemy.egg-info/entry_points.txt
 prefect_sqlalchemy.egg-info/requires.txt
 prefect_sqlalchemy.egg-info/top_level.txt
+tests/conftest.py
 tests/test_block_standards.py
 tests/test_credentials.py
-tests/test_database.py
+tests/test_database.py
+tests/test_version.py
```

### Comparing `prefect-sqlalchemy-0.4.0/tests/test_block_standards.py` & `prefect_sqlalchemy-0.4.1/tests/test_block_standards.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from prefect.blocks.core import Block
 from prefect.testing.standard_test_suites import BlockStandardTestSuite
 from prefect.utilities.dispatch import get_registry_for_type
 from prefect.utilities.importtools import to_qualified_name
 
 
 def find_module_blocks():
```

### Comparing `prefect-sqlalchemy-0.4.0/tests/test_credentials.py` & `prefect_sqlalchemy-0.4.1/tests/test_credentials.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pytest
-from prefect import flow
-from sqlalchemy.engine import URL, Engine
-from sqlalchemy.engine.url import make_url
-from sqlalchemy.ext.asyncio import AsyncEngine
-
 from prefect_sqlalchemy.credentials import (
     AsyncDriver,
     ConnectionComponents,
     DatabaseCredentials,
     SyncDriver,
 )
+from sqlalchemy.engine import URL, Engine
+from sqlalchemy.engine.url import make_url
+from sqlalchemy.ext.asyncio import AsyncEngine
+
+from prefect import flow
 
 
 @pytest.mark.parametrize(
     "url_param", ["driver", "username", "password", "database", "host", "port", "query"]
 )
 def test_sqlalchemy_credentials_post_init_url_param_conflict(url_param):
     @flow
```

### Comparing `prefect-sqlalchemy-0.4.0/tests/test_database.py` & `prefect_sqlalchemy-0.4.1/tests/test_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from contextlib import ExitStack, asynccontextmanager, contextmanager
 from unittest.mock import MagicMock
 
 import cloudpickle
 import pytest
-from prefect import flow, task
-from sqlalchemy import __version__ as SQLALCHEMY_VERSION
-from sqlalchemy.engine import Connection, Engine
-from sqlalchemy.ext.asyncio import AsyncConnection, AsyncEngine
-
 from prefect_sqlalchemy.credentials import (
     AsyncDriver,
     ConnectionComponents,
     DatabaseCredentials,
     SyncDriver,
 )
 from prefect_sqlalchemy.database import (
     SqlAlchemyConnector,
     sqlalchemy_execute,
     sqlalchemy_query,
 )
+from sqlalchemy import __version__ as SQLALCHEMY_VERSION
+from sqlalchemy.engine import Connection, Engine
+from sqlalchemy.ext.asyncio import AsyncConnection, AsyncEngine
+
+from prefect import flow, task
 
 
 class SQLAlchemyAsyncEngineMock:
     async def dispose(self):
         return True
 
     @asynccontextmanager
@@ -150,15 +150,15 @@
     async def test_flow():
         result = await sqlalchemy_execute.submit(
             "statement", sqlalchemy_credentials_async
         )
         return result
 
     result = await test_flow()
-    assert await (result.result()) is None
+    assert await result.result() is None
 
 
 def test_sqlalchemy_execute_sync(sqlalchemy_credentials_sync):
     @flow
     def test_flow():
         result = sqlalchemy_execute.submit("statement", sqlalchemy_credentials_sync)
         return result
```

