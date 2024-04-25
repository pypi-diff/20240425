# Comparing `tmp/modulos_client-0.5.6.tar.gz` & `tmp/modulos_client-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modulos_client-0.5.6.tar", last modified: Fri Feb  9 11:59:57 2024, max compression
+gzip compressed data, was "modulos_client-0.5.7.tar", last modified: Thu Apr 25 16:55:18 2024, max compression
```

## Comparing `modulos_client-0.5.6.tar` & `modulos_client-0.5.7.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:59:57.076541 modulos_client-0.5.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:59:57.068541 modulos_client-0.5.6/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-02-09 11:59:44.000000 modulos_client-0.5.6/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-02-09 11:59:44.000000 modulos_client-0.5.6/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:59:57.068541 modulos_client-0.5.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-02-09 11:59:44.000000 modulos_client-0.5.6/.github/workflows/pr-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-02-09 11:59:44.000000 modulos_client-0.5.6/.github/workflows/publish_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-02-09 11:59:44.000000 modulos_client-0.5.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-09 11:59:44.000000 modulos_client-0.5.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-02-09 11:59:57.076541 modulos_client-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-02-09 11:59:44.000000 modulos_client-0.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-09 11:59:44.000000 modulos_client-0.5.6/dev_README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:59:57.072541 modulos_client-0.5.6/modulos_client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 11:59:44.000000 modulos_client-0.5.6/modulos_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-09 11:59:56.000000 modulos_client-0.5.6/modulos_client/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-02-09 11:59:44.000000 modulos_client-0.5.6/modulos_client/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-02-09 11:59:44.000000 modulos_client-0.5.6/modulos_client/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-02-09 11:59:44.000000 modulos_client-0.5.6/modulos_client/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-02-09 11:59:44.000000 modulos_client-0.5.6/modulos_client/profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-02-09 11:59:44.000000 modulos_client-0.5.6/modulos_client/projects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:59:57.072541 modulos_client-0.5.6/modulos_client/registering/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-02-09 11:59:44.000000 modulos_client-0.5.6/modulos_client/registering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-02-09 11:59:44.000000 modulos_client-0.5.6/modulos_client/registering/register_on_modulos_platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:59:57.072541 modulos_client-0.5.6/modulos_client/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 11:59:44.000000 modulos_client-0.5.6/modulos_client/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-09 11:59:44.000000 modulos_client-0.5.6/modulos_client/services/users_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-02-09 11:59:44.000000 modulos_client-0.5.6/modulos_client/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-02-09 11:59:44.000000 modulos_client-0.5.6/modulos_client/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:59:57.072541 modulos_client-0.5.6/modulos_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-02-09 11:59:57.000000 modulos_client-0.5.6/modulos_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-02-09 11:59:57.000000 modulos_client-0.5.6/modulos_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 11:59:57.000000 modulos_client-0.5.6/modulos_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-09 11:59:57.000000 modulos_client-0.5.6/modulos_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-09 11:59:57.000000 modulos_client-0.5.6/modulos_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-09 11:59:57.000000 modulos_client-0.5.6/modulos_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-02-09 11:59:44.000000 modulos_client-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 11:59:57.076541 modulos_client-0.5.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:59:57.072541 modulos_client-0.5.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-02-09 11:59:44.000000 modulos_client-0.5.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-02-09 11:59:44.000000 modulos_client-0.5.6/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9577 2024-02-09 11:59:44.000000 modulos_client-0.5.6/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-02-09 11:59:44.000000 modulos_client-0.5.6/tests/test_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-02-09 11:59:44.000000 modulos_client-0.5.6/tests/test_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-02-09 11:59:44.000000 modulos_client-0.5.6/tests/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-02-09 11:59:44.000000 modulos_client-0.5.6/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-02-09 11:59:44.000000 modulos_client-0.5.6/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    23892 2024-02-09 11:59:44.000000 modulos_client-0.5.6/tests/test_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-02-09 11:59:44.000000 modulos_client-0.5.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:55:18.395778 modulos_client-0.5.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:55:18.387778 modulos_client-0.5.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-25 16:55:11.000000 modulos_client-0.5.7/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-25 16:55:11.000000 modulos_client-0.5.7/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:55:18.387778 modulos_client-0.5.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-25 16:55:11.000000 modulos_client-0.5.7/.github/workflows/pr-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-25 16:55:11.000000 modulos_client-0.5.7/.github/workflows/publish_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-25 16:55:11.000000 modulos_client-0.5.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-25 16:55:11.000000 modulos_client-0.5.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-25 16:55:18.395778 modulos_client-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-25 16:55:11.000000 modulos_client-0.5.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-25 16:55:11.000000 modulos_client-0.5.7/dev_README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:55:18.391778 modulos_client-0.5.7/modulos_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 16:55:18.000000 modulos_client-0.5.7/modulos_client/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/projects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:55:18.391778 modulos_client-0.5.7/modulos_client/registering/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/registering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/registering/register_on_modulos_platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:55:18.391778 modulos_client-0.5.7/modulos_client/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/services/users_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-04-25 16:55:11.000000 modulos_client-0.5.7/modulos_client/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:55:18.395778 modulos_client-0.5.7/modulos_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-25 16:55:18.000000 modulos_client-0.5.7/modulos_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-25 16:55:18.000000 modulos_client-0.5.7/modulos_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:55:18.000000 modulos_client-0.5.7/modulos_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 16:55:18.000000 modulos_client-0.5.7/modulos_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-25 16:55:18.000000 modulos_client-0.5.7/modulos_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 16:55:18.000000 modulos_client-0.5.7/modulos_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-25 16:55:11.000000 modulos_client-0.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:55:18.395778 modulos_client-0.5.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:55:18.395778 modulos_client-0.5.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-25 16:55:11.000000 modulos_client-0.5.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-25 16:55:11.000000 modulos_client-0.5.7/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9577 2024-04-25 16:55:11.000000 modulos_client-0.5.7/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-25 16:55:11.000000 modulos_client-0.5.7/tests/test_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-25 16:55:11.000000 modulos_client-0.5.7/tests/test_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-04-25 16:55:11.000000 modulos_client-0.5.7/tests/test_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-25 16:55:11.000000 modulos_client-0.5.7/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-25 16:55:11.000000 modulos_client-0.5.7/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-25 16:55:11.000000 modulos_client-0.5.7/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23892 2024-04-25 16:55:11.000000 modulos_client-0.5.7/tests/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-25 16:55:11.000000 modulos_client-0.5.7/tox.ini
```

### Comparing `modulos_client-0.5.6/.github/workflows/pr-test.yml` & `modulos_client-0.5.7/.github/workflows/pr-test.yml`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.6/.github/workflows/publish_pypi.yml` & `modulos_client-0.5.7/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.6/.gitignore` & `modulos_client-0.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.6/Makefile` & `modulos_client-0.5.7/Makefile`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.6/PKG-INFO` & `modulos_client-0.5.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: modulos_client
-Version: 0.5.6
+Version: 0.5.7
 Summary: Package to interact with the Modulos Platform
 Author-email: Modulos AG <contact@modulos.ai>
 Project-URL: Homepage, https://github.com/Modulos/modulos_client
 Project-URL: Bug Reports, https://github.com/Modulos/modulos_client/issues
 Project-URL: Source, https://github.com/Modulos/modulos_client
 Keywords: modulos_client
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: click<=8.1.7,>=8.1.7
-Requires-Dist: pandas<=2.1.4,>=1.5.3
-Requires-Dist: pydantic<=2.5.3,>=2.4.2
+Requires-Dist: pandas<=2.2.1,>=1.5.3
+Requires-Dist: pydantic<=2.6.3,>=2.4.2
 Requires-Dist: pyYAML<=6.0.1,>=6.0.1
 Requires-Dist: requests<=2.31.0,>=2.0.0
 Requires-Dist: tabulate<=0.9.0,>=0.9.0
 Provides-Extra: dev
-Requires-Dist: coverage<=7.4.0,>=7.2.7; extra == "dev"
-Requires-Dist: pytest<=7.4.4,>=7.3.1; extra == "dev"
-Requires-Dist: tox<=4.12.0,>=4.11.4; extra == "dev"
+Requires-Dist: coverage<=7.4.3,>=7.2.7; extra == "dev"
+Requires-Dist: pytest<=8.0.2,>=7.3.1; extra == "dev"
+Requires-Dist: tox<=4.13.0,>=4.11.4; extra == "dev"
 
 ## Modulos Client Tool
 
 This tool provides a command-line interface to interact with the Modulos platform.
 
 ### Prerequisites
 
@@ -109,32 +109,52 @@
 
 Create a new organization:
 
 ```bash
 modulos orgs create --name [ORG_NAME]
 ```
 
+#### Managing Organization Configurations
+
+In order to use the `modulos config-organizations` commands, you need to have superadmin permissions.
+
+Obtain the configuration of an organisation.
+
+```bash
+modulos config-organizations get [--organization-id [ORGANIZATION_ID]]
+```
+
+> There is an optional `--organization-id` parameter to specify the organization you want to get.
+> If you do not specify it, the organization you are currently logged into will be returned.
+> If you want to get the configuration for a different organization, you need to have super administrator permissions.
+
+Update configurations for an organization.
+
+```bash
+modulos config-organizations update --organization-id [ORGANIZATION_ID] --quota-projects [NUMBER_OF_PROJECTS_ALLOWED]
+```
+
 #### Managing Users
 
 List all users:
 
 ```bash
 modulos users list
 ```
 
 Create a new user:
 
 ```bash
 modulos users create --firstname [FIRST_NAME] --lastname [LAST_NAME] --email [EMAIL] --is-active [IS_ACTIVE] --is-org-admin [IS_ORG_ADMIN]
 ```
 
-There is an optional `--organization-id` parameter to specify the organization the user should be created for.
-If you don't specify it, the user will be created for the organization you are currently logged in to.
-If the user should be created for a different organization, you need to have superadmin permissions.
-For a user in the same organization, you need to have org admin permissions.
+> There is an optional `--organization-id` parameter to specify the organization the user should be created for.
+> If you don't specify it, the user will be created for the organization you are currently logged in to.
+> If the user should be created for a different organization, you need to have superadmin permissions.
+> For a user in the same organization, you need to have org admin permissions.
 
 Add organization admin privileges to a user:
 
 ```bash
 modulos users add-org-admin --user-id [USER_ID]
 ```
 
@@ -170,17 +190,17 @@
 
 Upload templates for your organization:
 
 ```bash
 modulos templates upload --file [FILE_PATH]
 ```
 
-There is an optional `--organization-id` parameter to specify the organization the template should be uploaded for.
-If you don't specify it, the template will be uploaded for the organization you are currently logged in to.
-If the template should be uploaded for a different organization, you need to have superadmin permissions.
+> There is an optional `--organization-id` parameter to specify the organization the template should be uploaded for.
+> If you don't specify it, the template will be uploaded for the organization you are currently logged in to.
+> If the template should be uploaded for a different organization, you need to have superadmin permissions.
 
 ---
 
 For a detailed list of available commands and their options, run:
 
 ```bash
 modulos --help
```

### Comparing `modulos_client-0.5.6/README.md` & `modulos_client-0.5.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -83,32 +83,52 @@
 
 Create a new organization:
 
 ```bash
 modulos orgs create --name [ORG_NAME]
 ```
 
+#### Managing Organization Configurations
+
+In order to use the `modulos config-organizations` commands, you need to have superadmin permissions.
+
+Obtain the configuration of an organisation.
+
+```bash
+modulos config-organizations get [--organization-id [ORGANIZATION_ID]]
+```
+
+> There is an optional `--organization-id` parameter to specify the organization you want to get.
+> If you do not specify it, the organization you are currently logged into will be returned.
+> If you want to get the configuration for a different organization, you need to have super administrator permissions.
+
+Update configurations for an organization.
+
+```bash
+modulos config-organizations update --organization-id [ORGANIZATION_ID] --quota-projects [NUMBER_OF_PROJECTS_ALLOWED]
+```
+
 #### Managing Users
 
 List all users:
 
 ```bash
 modulos users list
 ```
 
 Create a new user:
 
 ```bash
 modulos users create --firstname [FIRST_NAME] --lastname [LAST_NAME] --email [EMAIL] --is-active [IS_ACTIVE] --is-org-admin [IS_ORG_ADMIN]
 ```
 
-There is an optional `--organization-id` parameter to specify the organization the user should be created for.
-If you don't specify it, the user will be created for the organization you are currently logged in to.
-If the user should be created for a different organization, you need to have superadmin permissions.
-For a user in the same organization, you need to have org admin permissions.
+> There is an optional `--organization-id` parameter to specify the organization the user should be created for.
+> If you don't specify it, the user will be created for the organization you are currently logged in to.
+> If the user should be created for a different organization, you need to have superadmin permissions.
+> For a user in the same organization, you need to have org admin permissions.
 
 Add organization admin privileges to a user:
 
 ```bash
 modulos users add-org-admin --user-id [USER_ID]
 ```
 
@@ -144,17 +164,17 @@
 
 Upload templates for your organization:
 
 ```bash
 modulos templates upload --file [FILE_PATH]
 ```
 
-There is an optional `--organization-id` parameter to specify the organization the template should be uploaded for.
-If you don't specify it, the template will be uploaded for the organization you are currently logged in to.
-If the template should be uploaded for a different organization, you need to have superadmin permissions.
+> There is an optional `--organization-id` parameter to specify the organization the template should be uploaded for.
+> If you don't specify it, the template will be uploaded for the organization you are currently logged in to.
+> If the template should be uploaded for a different organization, you need to have superadmin permissions.
 
 ---
 
 For a detailed list of available commands and their options, run:
 
 ```bash
 modulos --help
```

### Comparing `modulos_client-0.5.6/dev_README.md` & `modulos_client-0.5.7/dev_README.md`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.6/modulos_client/cli.py` & `modulos_client-0.5.7/modulos_client/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 # --------------------------------------------------- #
 # Copyright (C) 2023 Modulos AG. All rights reserved. #
 # --------------------------------------------------- #
 import click
 
 from modulos_client import config as config_utils
-from modulos_client import organizations, profiles, projects, users, templates
+from modulos_client import (
+    organizations,
+    profiles,
+    projects,
+    users,
+    templates,
+    configurations,
+)
 
 
 @click.group()
 def main():
     pass
 
 
 main.add_command(profiles.profiles)
 main.add_command(organizations.orgs)
+main.add_command(configurations.config_organizations)
 main.add_command(users.users)
 main.add_command(projects.projects)
 main.add_command(templates.templates)
 
 
 @main.command(
     help=(
```

### Comparing `modulos_client-0.5.6/modulos_client/config.py` & `modulos_client-0.5.7/modulos_client/config.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.6/modulos_client/organizations.py` & `modulos_client-0.5.7/modulos_client/organizations.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.6/modulos_client/profiles.py` & `modulos_client-0.5.7/modulos_client/profiles.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.6/modulos_client/projects.py` & `modulos_client-0.5.7/modulos_client/projects.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.6/modulos_client/registering/register_on_modulos_platform.py` & `modulos_client-0.5.7/modulos_client/registering/register_on_modulos_platform.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.6/modulos_client/services/users_services.py` & `modulos_client-0.5.7/modulos_client/services/users_services.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.6/modulos_client/templates.py` & `modulos_client-0.5.7/modulos_client/templates.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.6/modulos_client/users.py` & `modulos_client-0.5.7/modulos_client/users.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.6/modulos_client.egg-info/PKG-INFO` & `modulos_client-0.5.7/modulos_client.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: modulos_client
-Version: 0.5.6
+Version: 0.5.7
 Summary: Package to interact with the Modulos Platform
 Author-email: Modulos AG <contact@modulos.ai>
 Project-URL: Homepage, https://github.com/Modulos/modulos_client
 Project-URL: Bug Reports, https://github.com/Modulos/modulos_client/issues
 Project-URL: Source, https://github.com/Modulos/modulos_client
 Keywords: modulos_client
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: click<=8.1.7,>=8.1.7
-Requires-Dist: pandas<=2.1.4,>=1.5.3
-Requires-Dist: pydantic<=2.5.3,>=2.4.2
+Requires-Dist: pandas<=2.2.1,>=1.5.3
+Requires-Dist: pydantic<=2.6.3,>=2.4.2
 Requires-Dist: pyYAML<=6.0.1,>=6.0.1
 Requires-Dist: requests<=2.31.0,>=2.0.0
 Requires-Dist: tabulate<=0.9.0,>=0.9.0
 Provides-Extra: dev
-Requires-Dist: coverage<=7.4.0,>=7.2.7; extra == "dev"
-Requires-Dist: pytest<=7.4.4,>=7.3.1; extra == "dev"
-Requires-Dist: tox<=4.12.0,>=4.11.4; extra == "dev"
+Requires-Dist: coverage<=7.4.3,>=7.2.7; extra == "dev"
+Requires-Dist: pytest<=8.0.2,>=7.3.1; extra == "dev"
+Requires-Dist: tox<=4.13.0,>=4.11.4; extra == "dev"
 
 ## Modulos Client Tool
 
 This tool provides a command-line interface to interact with the Modulos platform.
 
 ### Prerequisites
 
@@ -109,32 +109,52 @@
 
 Create a new organization:
 
 ```bash
 modulos orgs create --name [ORG_NAME]
 ```
 
+#### Managing Organization Configurations
+
+In order to use the `modulos config-organizations` commands, you need to have superadmin permissions.
+
+Obtain the configuration of an organisation.
+
+```bash
+modulos config-organizations get [--organization-id [ORGANIZATION_ID]]
+```
+
+> There is an optional `--organization-id` parameter to specify the organization you want to get.
+> If you do not specify it, the organization you are currently logged into will be returned.
+> If you want to get the configuration for a different organization, you need to have super administrator permissions.
+
+Update configurations for an organization.
+
+```bash
+modulos config-organizations update --organization-id [ORGANIZATION_ID] --quota-projects [NUMBER_OF_PROJECTS_ALLOWED]
+```
+
 #### Managing Users
 
 List all users:
 
 ```bash
 modulos users list
 ```
 
 Create a new user:
 
 ```bash
 modulos users create --firstname [FIRST_NAME] --lastname [LAST_NAME] --email [EMAIL] --is-active [IS_ACTIVE] --is-org-admin [IS_ORG_ADMIN]
 ```
 
-There is an optional `--organization-id` parameter to specify the organization the user should be created for.
-If you don't specify it, the user will be created for the organization you are currently logged in to.
-If the user should be created for a different organization, you need to have superadmin permissions.
-For a user in the same organization, you need to have org admin permissions.
+> There is an optional `--organization-id` parameter to specify the organization the user should be created for.
+> If you don't specify it, the user will be created for the organization you are currently logged in to.
+> If the user should be created for a different organization, you need to have superadmin permissions.
+> For a user in the same organization, you need to have org admin permissions.
 
 Add organization admin privileges to a user:
 
 ```bash
 modulos users add-org-admin --user-id [USER_ID]
 ```
 
@@ -170,17 +190,17 @@
 
 Upload templates for your organization:
 
 ```bash
 modulos templates upload --file [FILE_PATH]
 ```
 
-There is an optional `--organization-id` parameter to specify the organization the template should be uploaded for.
-If you don't specify it, the template will be uploaded for the organization you are currently logged in to.
-If the template should be uploaded for a different organization, you need to have superadmin permissions.
+> There is an optional `--organization-id` parameter to specify the organization the template should be uploaded for.
+> If you don't specify it, the template will be uploaded for the organization you are currently logged in to.
+> If the template should be uploaded for a different organization, you need to have superadmin permissions.
 
 ---
 
 For a detailed list of available commands and their options, run:
 
 ```bash
 modulos --help
```

### Comparing `modulos_client-0.5.6/modulos_client.egg-info/SOURCES.txt` & `modulos_client-0.5.7/modulos_client.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 .github/pull_request_template.md
 .github/workflows/pr-test.yml
 .github/workflows/publish_pypi.yml
 modulos_client/__init__.py
 modulos_client/_version.py
 modulos_client/cli.py
 modulos_client/config.py
+modulos_client/configurations.py
 modulos_client/organizations.py
 modulos_client/profiles.py
 modulos_client/projects.py
 modulos_client/templates.py
 modulos_client/users.py
 modulos_client.egg-info/PKG-INFO
 modulos_client.egg-info/SOURCES.txt
@@ -26,13 +27,14 @@
 modulos_client/registering/__init__.py
 modulos_client/registering/register_on_modulos_platform.py
 modulos_client/services/__init__.py
 modulos_client/services/users_services.py
 tests/conftest.py
 tests/test_cli.py
 tests/test_config.py
+tests/test_configurations.py
 tests/test_organization.py
 tests/test_profiles.py
 tests/test_projects.py
 tests/test_services.py
 tests/test_templates.py
 tests/test_users.py
```

### Comparing `modulos_client-0.5.6/pyproject.toml` & `modulos_client-0.5.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -17,31 +17,31 @@
   "Natural Language :: English",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version"]
 dependencies = [
     "click >= 8.1.7, <= 8.1.7",
-    "pandas >= 1.5.3, <= 2.1.4",
-    "pydantic >= 2.4.2, <= 2.5.3",
+    "pandas >= 1.5.3, <= 2.2.1",
+    "pydantic >= 2.4.2, <= 2.6.3",
     "pyYAML >= 6.0.1, <= 6.0.1",
     "requests >= 2.0.0, <= 2.31.0",
     "tabulate >= 0.9.0, <= 0.9.0",
 ]
 
 # List additional groups of dependencies here (e.g. development
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
 #   $ pip install modulos_client[dev]
 [project.optional-dependencies]
 dev = [
-    'coverage>= 7.2.7, <= 7.4.0',
-    'pytest >= 7.3.1, <= 7.4.4',
-    'tox >= 4.11.4, <= 4.12.0',
+    'coverage>= 7.2.7, <= 7.4.3',
+    'pytest >= 7.3.1, <= 8.0.2',
+    'tox >= 4.11.4, <= 4.13.0',
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Modulos/modulos_client"
 "Bug Reports" = "https://github.com/Modulos/modulos_client/issues"
 "Source" = "https://github.com/Modulos/modulos_client"
```

### Comparing `modulos_client-0.5.6/tests/conftest.py` & `modulos_client-0.5.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.6/tests/test_cli.py` & `modulos_client-0.5.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.6/tests/test_config.py` & `modulos_client-0.5.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.6/tests/test_organization.py` & `modulos_client-0.5.7/tests/test_organization.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.6/tests/test_profiles.py` & `modulos_client-0.5.7/tests/test_profiles.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.6/tests/test_projects.py` & `modulos_client-0.5.7/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.6/tests/test_services.py` & `modulos_client-0.5.7/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.6/tests/test_templates.py` & `modulos_client-0.5.7/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.6/tests/test_users.py` & `modulos_client-0.5.7/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `modulos_client-0.5.6/tox.ini` & `modulos_client-0.5.7/tox.ini`

 * *Files identical despite different names*

