# Comparing `tmp/gitlab_projects_settings-1.0.1.tar.gz` & `tmp/gitlab_projects_settings-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_projects_settings-1.0.1.tar", last modified: Wed Apr 24 07:19:31 2024, max compression
+gzip compressed data, was "gitlab_projects_settings-1.1.0.tar", last modified: Thu Apr 25 08:04:34 2024, max compression
```

## Comparing `gitlab_projects_settings-1.0.1.tar` & `gitlab_projects_settings-1.1.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:19:31.113362 gitlab_projects_settings-1.0.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:19:31.105362 gitlab_projects_settings-1.0.1/.chglog/
--rwxrwxrwx   0 root         (0) root         (0)      649 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/.chglog/CHANGELOG.tpl.md
--rw-rw-rw-   0 root         (0) root         (0)      759 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/.chglog/changelog.sh
--rwxrwxrwx   0 root         (0) root         (0)      703 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/.chglog/config.yml
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     6097 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/.markdownlint.json
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/.style.yapf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:19:31.106362 gitlab_projects_settings-1.0.1/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/.vscode/extensions.json
--rw-rw-rw-   0 root         (0) root         (0)     1252 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/.vscode/settings.json
--rw-rw-rw-   0 root         (0) root         (0)      329 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4924 2024-04-24 07:19:31.112362 gitlab_projects_settings-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3315 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:19:31.106362 gitlab_projects_settings-1.0.1/gitlab_projects_settings/
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/gitlab_projects_settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/gitlab_projects_settings/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:19:31.108362 gitlab_projects_settings-1.0.1/gitlab_projects_settings/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/gitlab_projects_settings/cli/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5331 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/gitlab_projects_settings/cli/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:19:31.109362 gitlab_projects_settings-1.0.1/gitlab_projects_settings/features/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/gitlab_projects_settings/features/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11344 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/gitlab_projects_settings/features/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)     7772 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/gitlab_projects_settings/features/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:19:31.110362 gitlab_projects_settings-1.0.1/gitlab_projects_settings/package/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/gitlab_projects_settings/package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/gitlab_projects_settings/package/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)     1444 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/gitlab_projects_settings/package/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:19:31.110362 gitlab_projects_settings-1.0.1/gitlab_projects_settings/prints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/gitlab_projects_settings/prints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/gitlab_projects_settings/prints/colors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:19:31.111362 gitlab_projects_settings-1.0.1/gitlab_projects_settings/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/gitlab_projects_settings/system/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/gitlab_projects_settings/system/platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:19:31.112362 gitlab_projects_settings-1.0.1/gitlab_projects_settings.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4924 2024-04-24 07:19:31.000000 gitlab_projects_settings-1.0.1/gitlab_projects_settings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1197 2024-04-24 07:19:31.000000 gitlab_projects_settings-1.0.1/gitlab_projects_settings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 07:19:31.000000 gitlab_projects_settings-1.0.1/gitlab_projects_settings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2024-04-24 07:19:31.000000 gitlab_projects_settings-1.0.1/gitlab_projects_settings.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       55 2024-04-24 07:19:31.000000 gitlab_projects_settings-1.0.1/gitlab_projects_settings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-24 07:19:31.000000 gitlab_projects_settings-1.0.1/gitlab_projects_settings.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:19:31.112362 gitlab_projects_settings-1.0.1/requirements/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/requirements/build.txt
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/requirements/deploy.txt
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/requirements/quality.txt
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/requirements/runtime.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 07:19:31.113362 gitlab_projects_settings-1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2677 2024-04-24 07:19:23.000000 gitlab_projects_settings-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 08:04:34.038734 gitlab_projects_settings-1.1.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 08:04:34.030734 gitlab_projects_settings-1.1.0/.chglog/
+-rwxrwxrwx   0 root         (0) root         (0)      649 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/.chglog/CHANGELOG.tpl.md
+-rw-rw-rw-   0 root         (0) root         (0)      759 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/.chglog/changelog.sh
+-rwxrwxrwx   0 root         (0) root         (0)      703 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/.chglog/config.yml
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     6097 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/.markdownlint.json
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/.style.yapf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 08:04:34.030734 gitlab_projects_settings-1.1.0/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/.vscode/extensions.json
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)      603 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4906 2024-04-25 08:04:34.037734 gitlab_projects_settings-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3297 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 08:04:34.031734 gitlab_projects_settings-1.1.0/gitlab_projects_settings/
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 08:04:34.033734 gitlab_projects_settings-1.1.0/gitlab_projects_settings/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/cli/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5319 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/cli/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 08:04:34.034734 gitlab_projects_settings-1.1.0/gitlab_projects_settings/features/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/features/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11344 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/features/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)     7838 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/features/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 08:04:34.034734 gitlab_projects_settings-1.1.0/gitlab_projects_settings/package/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/package/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1444 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/package/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 08:04:34.035734 gitlab_projects_settings-1.1.0/gitlab_projects_settings/prints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/prints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/prints/colors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 08:04:34.035734 gitlab_projects_settings-1.1.0/gitlab_projects_settings/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/system/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/system/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 08:04:34.037734 gitlab_projects_settings-1.1.0/gitlab_projects_settings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4906 2024-04-25 08:04:34.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-04-25 08:04:34.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 08:04:34.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2024-04-25 08:04:34.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2024-04-25 08:04:34.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-25 08:04:34.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 08:04:34.037734 gitlab_projects_settings-1.1.0/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/requirements/build.txt
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/requirements/deploy.txt
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/requirements/quality.txt
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/requirements/runtime.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 08:04:34.038734 gitlab_projects_settings-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2677 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/setup.py
```

### Comparing `gitlab_projects_settings-1.0.1/.chglog/CHANGELOG.tpl.md` & `gitlab_projects_settings-1.1.0/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-1.0.1/.chglog/changelog.sh` & `gitlab_projects_settings-1.1.0/.chglog/changelog.sh`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-1.0.1/.chglog/config.yml` & `gitlab_projects_settings-1.1.0/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-1.0.1/.gitlab-ci.yml` & `gitlab_projects_settings-1.1.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-1.0.1/.style.yapf` & `gitlab_projects_settings-1.1.0/.style.yapf`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-1.0.1/.vscode/extensions.json` & `gitlab_projects_settings-1.1.0/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-1.0.1/.vscode/settings.json` & `gitlab_projects_settings-1.1.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-1.0.1/LICENSE` & `gitlab_projects_settings-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-1.0.1/PKG-INFO` & `gitlab_projects_settings-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-settings
-Version: 1.0.1
+Version: 1.1.0
 Summary: Configure GitLab groups and projects settings automatically
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-settings
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-settings/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-settings/blob/main/CHANGELOG.md
@@ -53,16 +53,16 @@
 ---
 
 ## Usage
 
 <!-- prettier-ignore-start -->
 
 ```yaml
-usage: gitlab-projects-settings [-h] [--version] [-t TOKEN] [--dry-run] [--avoid-group]
-                                [--avoid-subgroups] [--avoid-projects] [--reset-features]
+usage: gitlab-projects-settings [-h] [--version] [-t TOKEN] [--dry-run] [--exclude-group]
+                                [--exclude-subgroups] [--exclude-projects] [--reset-features]
                                 [--reset-members] [--set-avatar FILE] [--set-description TEXT]
                                 [--update-description] [--protect-branches]
                                 [--protect-tags LEVEL]
                                 [gitlab] [path]
 
 gitlab-projects-settings: Configure GitLab groups and projects settings automatically
 
@@ -71,17 +71,17 @@
   --version             # Show the current version
 
 credentials arguments:
   -t TOKEN              # GitLab API token (default: GITLAB_TOKEN environment)
 
 common settings arguments:
   --dry-run             # Enable dry run mode to check without saving
-  --avoid-group         # Avoid affecting parent group settings
-  --avoid-subgroups     # Avoid affecting children subgroups settings
-  --avoid-projects      # Avoid affecting children projects settings
+  --exclude-group       # Exclude parent group settings
+  --exclude-subgroups   # Exclude children subgroups settings
+  --exclude-projects    # Exclude children projects settings
 
 general settings arguments:
   --reset-features      # Reset features of GitLab projects based on usage
   --reset-members       # Reset members of GitLab projects and groups
   --set-avatar FILE     # Set avatar of GitLab projects and groups
   --set-description TEXT
                         # Set description of GitLab projects and groups
```

### Comparing `gitlab_projects_settings-1.0.1/README.md` & `gitlab_projects_settings-1.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 ---
 
 ## Usage
 
 <!-- prettier-ignore-start -->
 
 ```yaml
-usage: gitlab-projects-settings [-h] [--version] [-t TOKEN] [--dry-run] [--avoid-group]
-                                [--avoid-subgroups] [--avoid-projects] [--reset-features]
+usage: gitlab-projects-settings [-h] [--version] [-t TOKEN] [--dry-run] [--exclude-group]
+                                [--exclude-subgroups] [--exclude-projects] [--reset-features]
                                 [--reset-members] [--set-avatar FILE] [--set-description TEXT]
                                 [--update-description] [--protect-branches]
                                 [--protect-tags LEVEL]
                                 [gitlab] [path]
 
 gitlab-projects-settings: Configure GitLab groups and projects settings automatically
 
@@ -37,17 +37,17 @@
   --version             # Show the current version
 
 credentials arguments:
   -t TOKEN              # GitLab API token (default: GITLAB_TOKEN environment)
 
 common settings arguments:
   --dry-run             # Enable dry run mode to check without saving
-  --avoid-group         # Avoid affecting parent group settings
-  --avoid-subgroups     # Avoid affecting children subgroups settings
-  --avoid-projects      # Avoid affecting children projects settings
+  --exclude-group       # Exclude parent group settings
+  --exclude-subgroups   # Exclude children subgroups settings
+  --exclude-projects    # Exclude children projects settings
 
 general settings arguments:
   --reset-features      # Reset features of GitLab projects based on usage
   --reset-members       # Reset members of GitLab projects and groups
   --set-avatar FILE     # Set avatar of GitLab projects and groups
   --set-description TEXT
                         # Set description of GitLab projects and groups
```

### Comparing `gitlab_projects_settings-1.0.1/gitlab_projects_settings/cli/main.py` & `gitlab_projects_settings-1.1.0/gitlab_projects_settings/cli/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,30 +57,30 @@
     group.add_argument(
         '--dry-run',
         dest='dry_run',
         action='store_true',
         help='Enable dry run mode to check without saving',
     )
     group.add_argument(
-        '--avoid-group',
-        dest='avoid_group',
+        '--exclude-group',
+        dest='exclude_group',
         action='store_true',
-        help='Avoid affecting parent group settings',
+        help='Exclude parent group settings',
     )
     group.add_argument(
-        '--avoid-subgroups',
-        dest='avoid_subgroups',
+        '--exclude-subgroups',
+        dest='exclude_subgroups',
         action='store_true',
-        help='Avoid affecting children subgroups settings',
+        help='Exclude children subgroups settings',
     )
     group.add_argument(
-        '--avoid-projects',
-        dest='avoid_projects',
+        '--exclude-projects',
+        dest='exclude_projects',
         action='store_true',
-        help='Avoid affecting children projects settings',
+        help='Exclude children projects settings',
     )
 
     # Arguments general settings definitions
     group = parser.add_argument_group('general settings arguments')
     group.add_argument(
         '--reset-features',
         dest='reset_features',
```

### Comparing `gitlab_projects_settings-1.0.1/gitlab_projects_settings/features/gitlab.py` & `gitlab_projects_settings-1.1.0/gitlab_projects_settings/features/gitlab.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-1.0.1/gitlab_projects_settings/features/settings.py` & `gitlab_projects_settings-1.1.0/gitlab_projects_settings/features/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,46 +53,105 @@
         if project:
             SettingsFeature.project(options, gitlab, project.id)
 
         # Handle group recursively
         elif group:
 
             # Handle group
-            if not options.avoid_group:
+            if not options.exclude_group:
                 SettingsFeature.group(options, gitlab, group.id)
 
             # Iterate through subgroups
-            if not options.avoid_subgroups:
+            if not options.exclude_subgroups:
                 for group_subgroup in group.descendant_groups.list(
                         get_all=True,
                         include_subgroups=True,
                         order_by='path',
                         sort='asc',
                 ):
                     SettingsFeature.group(options, gitlab, group_subgroup.id)
 
             # Iterate through projects
-            if not options.avoid_projects:
+            if not options.exclude_projects:
                 for group_project in group.projects.list(
                         get_all=True,
-                        include_subgroups=not options.avoid_subgroups,
+                        include_subgroups=not options.exclude_subgroups,
                         order_by='path',
                         sort='asc',
                 ):
                     SettingsFeature.project(options, gitlab, group_project.id)
 
         # Result
         return True
 
-    # GitLab projects settings project, pylint: disable=too-many-branches
+    # Group
     @staticmethod
-    def project(options: Namespace, gitlab: GitLabFeature, criteria: str) -> None:
+    def group(
+        options: Namespace,
+        gitlab: GitLabFeature,
+        criteria: str,
+        subgroup: bool = False,
+    ) -> None:
 
-        # Show project details
+        # Acquire group
+        group = gitlab.group(criteria)
+
+        # Show group details
+        group_type = 'subgroup' if subgroup else 'group'
+        print(f'{Colors.BOLD} - GitLab {group_type}: '
+              f'{Colors.YELLOW_LIGHT}{group.full_path} '
+              f'{Colors.CYAN}({group.description})'
+              f'{Colors.RESET}')
+
+        # Set group description
+        if options.set_description:
+            gitlab.group_set_description(criteria, options.set_description)
+            print(f'{Colors.BOLD}   - Set description: '
+                  f'{Colors.CYAN}{options.set_description}'
+                  f'{Colors.RESET}')
+
+        # Update group description
+        elif options.update_description:
+            description = f'{group.name[:1].capitalize()}{group.name[1:]}' \
+                            f' - description'
+            gitlab.group_set_description(criteria, description)
+            print(f'{Colors.BOLD}   - Updated description: '
+                  f'{Colors.CYAN}{description}'
+                  f'{Colors.RESET}')
+
+        # Reset group members
+        if options.reset_members:
+            gitlab.group_reset_members(criteria)
+            print(f'{Colors.BOLD}   - Reset members: '
+                  f'{Colors.GREEN}Success'
+                  f'{Colors.RESET}')
+
+        # Set group avatar
+        if options.set_avatar:
+            gitlab.group_set_avatar(criteria, options.set_avatar)
+            print(f'{Colors.BOLD}   - Set avatar: '
+                  f'{Colors.CYAN}{options.set_avatar}'
+                  f'{Colors.RESET}')
+
+        # Footer
+        print(' ')
+        Platform.flush()
+
+    # Project, pylint: disable=too-many-branches
+    @staticmethod
+    def project(
+        options: Namespace,
+        gitlab: GitLabFeature,
+        criteria: str,
+    ) -> None:
+
+        # Acquire project
         project = gitlab.project(criteria)
+
+        # Show project details
         print(f'{Colors.BOLD} - GitLab project: '
               f'{Colors.YELLOW_LIGHT}{project.path_with_namespace} '
               f'{Colors.CYAN}({project.description})'
               f'{Colors.RESET}')
 
         # Set project description
         if options.set_description:
@@ -160,54 +219,7 @@
                 print(f'{Colors.BOLD}   - Protecting tags: '
                       f'{Colors.GREEN}Already done'
                       f'{Colors.RESET}')
 
         # Footer
         print(' ')
         Platform.flush()
-
-    # GitLab projects settings group
-    @staticmethod
-    def group(options: Namespace, gitlab: GitLabFeature, criteria: str,
-              subgroup: bool = False) -> None:
-
-        # Show group details
-        group = gitlab.group(criteria)
-        group_type = 'subgroup' if subgroup else 'group'
-        print(f'{Colors.BOLD} - GitLab {group_type}: '
-              f'{Colors.YELLOW_LIGHT}{group.full_path} '
-              f'{Colors.CYAN}({group.description})'
-              f'{Colors.RESET}')
-
-        # Set group description
-        if options.set_description:
-            gitlab.group_set_description(criteria, options.set_description)
-            print(f'{Colors.BOLD}   - Set description: '
-                  f'{Colors.CYAN}{options.set_description}'
-                  f'{Colors.RESET}')
-
-        # Update group description
-        elif options.update_description:
-            description = f'{group.name[:1].capitalize()}{group.name[1:]}' \
-                            f' - description'
-            gitlab.group_set_description(criteria, description)
-            print(f'{Colors.BOLD}   - Updated description: '
-                  f'{Colors.CYAN}{description}'
-                  f'{Colors.RESET}')
-
-        # Reset group members
-        if options.reset_members:
-            gitlab.group_reset_members(criteria)
-            print(f'{Colors.BOLD}   - Reset members: '
-                  f'{Colors.GREEN}Success'
-                  f'{Colors.RESET}')
-
-        # Set group avatar
-        if options.set_avatar:
-            gitlab.group_set_avatar(criteria, options.set_avatar)
-            print(f'{Colors.BOLD}   - Set avatar: '
-                  f'{Colors.CYAN}{options.set_avatar}'
-                  f'{Colors.RESET}')
-
-        # Footer
-        print(' ')
-        Platform.flush()
```

### Comparing `gitlab_projects_settings-1.0.1/gitlab_projects_settings/package/version.py` & `gitlab_projects_settings-1.1.0/gitlab_projects_settings/package/version.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-1.0.1/gitlab_projects_settings/prints/colors.py` & `gitlab_projects_settings-1.1.0/gitlab_projects_settings/prints/colors.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-1.0.1/gitlab_projects_settings/system/platform.py` & `gitlab_projects_settings-1.1.0/gitlab_projects_settings/system/platform.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-1.0.1/gitlab_projects_settings.egg-info/PKG-INFO` & `gitlab_projects_settings-1.1.0/gitlab_projects_settings.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-settings
-Version: 1.0.1
+Version: 1.1.0
 Summary: Configure GitLab groups and projects settings automatically
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-settings
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-settings/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-settings/blob/main/CHANGELOG.md
@@ -53,16 +53,16 @@
 ---
 
 ## Usage
 
 <!-- prettier-ignore-start -->
 
 ```yaml
-usage: gitlab-projects-settings [-h] [--version] [-t TOKEN] [--dry-run] [--avoid-group]
-                                [--avoid-subgroups] [--avoid-projects] [--reset-features]
+usage: gitlab-projects-settings [-h] [--version] [-t TOKEN] [--dry-run] [--exclude-group]
+                                [--exclude-subgroups] [--exclude-projects] [--reset-features]
                                 [--reset-members] [--set-avatar FILE] [--set-description TEXT]
                                 [--update-description] [--protect-branches]
                                 [--protect-tags LEVEL]
                                 [gitlab] [path]
 
 gitlab-projects-settings: Configure GitLab groups and projects settings automatically
 
@@ -71,17 +71,17 @@
   --version             # Show the current version
 
 credentials arguments:
   -t TOKEN              # GitLab API token (default: GITLAB_TOKEN environment)
 
 common settings arguments:
   --dry-run             # Enable dry run mode to check without saving
-  --avoid-group         # Avoid affecting parent group settings
-  --avoid-subgroups     # Avoid affecting children subgroups settings
-  --avoid-projects      # Avoid affecting children projects settings
+  --exclude-group       # Exclude parent group settings
+  --exclude-subgroups   # Exclude children subgroups settings
+  --exclude-projects    # Exclude children projects settings
 
 general settings arguments:
   --reset-features      # Reset features of GitLab projects based on usage
   --reset-members       # Reset members of GitLab projects and groups
   --set-avatar FILE     # Set avatar of GitLab projects and groups
   --set-description TEXT
                         # Set description of GitLab projects and groups
```

### Comparing `gitlab_projects_settings-1.0.1/gitlab_projects_settings.egg-info/SOURCES.txt` & `gitlab_projects_settings-1.1.0/gitlab_projects_settings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-1.0.1/setup.py` & `gitlab_projects_settings-1.1.0/setup.py`

 * *Files identical despite different names*

