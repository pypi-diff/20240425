# Comparing `tmp/android-cli-1.0.8.tar.gz` & `tmp/android-cli-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "android-cli-1.0.8.tar", last modified: Mon Mar 18 12:50:10 2024, max compression
+gzip compressed data, was "android-cli-1.0.9.tar", last modified: Thu Apr 25 12:25:16 2024, max compression
```

## Comparing `android-cli-1.0.8.tar` & `android-cli-1.0.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-03-18 12:50:10.996668 android-cli-1.0.8/
--rw-r--r--   0 juan       (501) staff       (20)      236 2024-03-18 12:50:10.996416 android-cli-1.0.8/PKG-INFO
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-03-18 12:50:10.981082 android-cli-1.0.8/android_cli.egg-info/
--rw-r--r--   0 juan       (501) staff       (20)      236 2024-03-18 12:50:10.000000 android-cli-1.0.8/android_cli.egg-info/PKG-INFO
--rw-r--r--   0 juan       (501) staff       (20)     1963 2024-03-18 12:50:10.000000 android-cli-1.0.8/android_cli.egg-info/SOURCES.txt
--rw-r--r--   0 juan       (501) staff       (20)        1 2024-03-18 12:50:10.000000 android-cli-1.0.8/android_cli.egg-info/dependency_links.txt
--rw-r--r--   0 juan       (501) staff       (20)       51 2024-03-18 12:50:10.000000 android-cli-1.0.8/android_cli.egg-info/entry_points.txt
--rw-r--r--   0 juan       (501) staff       (20)       91 2024-03-18 12:50:10.000000 android-cli-1.0.8/android_cli.egg-info/requires.txt
--rw-r--r--   0 juan       (501) staff       (20)        4 2024-03-18 12:50:10.000000 android-cli-1.0.8/android_cli.egg-info/top_level.txt
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-03-18 12:50:10.981804 android-cli-1.0.8/cli/
--rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-14 02:14:42.000000 android-cli-1.0.8/cli/__init__.py
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-03-18 12:50:10.984590 android-cli-1.0.8/cli/entities/
--rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-14 02:21:04.000000 android-cli-1.0.8/cli/entities/__init__.py
--rw-r--r--   0 juan       (501) staff       (20)     6252 2024-03-18 12:41:51.000000 android-cli-1.0.8/cli/entities/app.py
--rw-r--r--   0 juan       (501) staff       (20)     2954 2024-03-08 20:33:40.000000 android-cli-1.0.8/cli/entities/aws.py
--rw-r--r--   0 juan       (501) staff       (20)     5858 2024-03-05 20:01:57.000000 android-cli-1.0.8/cli/entities/bitrise.py
--rw-r--r--   0 juan       (501) staff       (20)     2090 2024-03-05 20:01:57.000000 android-cli-1.0.8/cli/entities/fcm.py
--rw-r--r--   0 juan       (501) staff       (20)     2600 2024-01-24 19:37:08.000000 android-cli-1.0.8/cli/entities/git.py
--rw-r--r--   0 juan       (501) staff       (20)    13647 2024-03-04 20:18:55.000000 android-cli-1.0.8/cli/entities/jira.py
--rw-r--r--   0 juan       (501) staff       (20)     8102 2024-03-18 12:31:54.000000 android-cli-1.0.8/cli/entities/lokalise.py
--rw-r--r--   0 juan       (501) staff       (20)     9699 2024-03-18 12:31:54.000000 android-cli-1.0.8/cli/entities/menu.py
--rw-r--r--   0 juan       (501) staff       (20)     6495 2024-03-05 20:01:57.000000 android-cli-1.0.8/cli/entities/setting.py
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-03-18 12:50:10.984968 android-cli-1.0.8/cli/form/
--rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-14 22:20:43.000000 android-cli-1.0.8/cli/form/__init__.py
--rw-r--r--   0 juan       (501) staff       (20)      682 2024-01-24 18:46:20.000000 android-cli-1.0.8/cli/form/_form_confirm.py
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-03-18 12:50:10.986681 android-cli-1.0.8/cli/form/bitrise/
--rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-20 15:13:23.000000 android-cli-1.0.8/cli/form/bitrise/__init__.py
--rw-r--r--   0 juan       (501) staff       (20)     2258 2024-01-24 14:18:20.000000 android-cli-1.0.8/cli/form/bitrise/branch_form.py
--rw-r--r--   0 juan       (501) staff       (20)      676 2024-01-24 14:18:20.000000 android-cli-1.0.8/cli/form/bitrise/build_type_form.py
--rw-r--r--   0 juan       (501) staff       (20)     1489 2024-02-09 17:02:00.000000 android-cli-1.0.8/cli/form/bitrise/release_notes_form.py
--rw-r--r--   0 juan       (501) staff       (20)     2542 2024-01-29 12:48:34.000000 android-cli-1.0.8/cli/form/bitrise/version_code_form.py
--rw-r--r--   0 juan       (501) staff       (20)     2368 2024-01-24 14:18:20.000000 android-cli-1.0.8/cli/form/bitrise/version_name_form.py
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-03-18 12:50:10.987264 android-cli-1.0.8/cli/form/code_gen/
--rw-r--r--   0 juan       (501) staff       (20)        0 2024-03-04 16:53:48.000000 android-cli-1.0.8/cli/form/code_gen/__init__.py
--rw-r--r--   0 juan       (501) staff       (20)      657 2024-03-04 16:53:48.000000 android-cli-1.0.8/cli/form/code_gen/code_gen_form.py
--rw-r--r--   0 juan       (501) staff       (20)     3505 2024-03-15 19:00:19.000000 android-cli-1.0.8/cli/form/code_gen/create_new_screen.py
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-03-18 12:50:10.988584 android-cli-1.0.8/cli/form/fcm/
--rw-r--r--   0 juan       (501) staff       (20)        0 2024-03-05 20:01:57.000000 android-cli-1.0.8/cli/form/fcm/__init__.py
--rw-r--r--   0 juan       (501) staff       (20)     1194 2024-03-05 20:01:57.000000 android-cli-1.0.8/cli/form/fcm/fcm_firebase_id_form.py
--rw-r--r--   0 juan       (501) staff       (20)      456 2024-03-05 20:01:57.000000 android-cli-1.0.8/cli/form/fcm/fcm_notification_body_form.py
--rw-r--r--   0 juan       (501) staff       (20)      514 2024-03-05 20:01:57.000000 android-cli-1.0.8/cli/form/fcm/fcm_notification_deeplink_form.py
--rw-r--r--   0 juan       (501) staff       (20)      460 2024-03-05 20:01:57.000000 android-cli-1.0.8/cli/form/fcm/fcm_notification_title_form.py
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-03-18 12:50:10.989932 android-cli-1.0.8/cli/form/git/
--rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-24 12:50:52.000000 android-cli-1.0.8/cli/form/git/__init__.py
--rw-r--r--   0 juan       (501) staff       (20)     3035 2024-01-24 18:46:20.000000 android-cli-1.0.8/cli/form/git/_new_branch_form.py
--rw-r--r--   0 juan       (501) staff       (20)     4193 2024-01-24 20:09:48.000000 android-cli-1.0.8/cli/form/git/_pull_request_form.py
--rw-r--r--   0 juan       (501) staff       (20)     2242 2024-01-24 19:15:46.000000 android-cli-1.0.8/cli/form/git/create_new_branch.py
--rw-r--r--   0 juan       (501) staff       (20)     4012 2024-02-01 20:35:53.000000 android-cli-1.0.8/cli/form/git/create_new_pull_request.py
--rw-r--r--   0 juan       (501) staff       (20)      673 2024-01-24 19:45:29.000000 android-cli-1.0.8/cli/form/git/git_form.py
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-03-18 12:50:10.991648 android-cli-1.0.8/cli/form/jira/
--rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-23 15:51:10.000000 android-cli-1.0.8/cli/form/jira/__init__.py
--rw-r--r--   0 juan       (501) staff       (20)      458 2024-02-01 18:44:37.000000 android-cli-1.0.8/cli/form/jira/jira_description_form.py
--rw-r--r--   0 juan       (501) staff       (20)      611 2024-03-05 20:02:08.000000 android-cli-1.0.8/cli/form/jira/jira_issue_form.py
--rw-r--r--   0 juan       (501) staff       (20)      791 2024-02-14 12:28:45.000000 android-cli-1.0.8/cli/form/jira/jira_release_start_date_form.py
--rw-r--r--   0 juan       (501) staff       (20)      749 2024-02-14 12:27:50.000000 android-cli-1.0.8/cli/form/jira/jira_release_version_form.py
--rw-r--r--   0 juan       (501) staff       (20)      640 2024-02-01 20:23:20.000000 android-cli-1.0.8/cli/form/jira/jira_title_form.py
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-03-18 12:50:10.992872 android-cli-1.0.8/cli/form/lokalise/
--rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-20 15:15:41.000000 android-cli-1.0.8/cli/form/lokalise/__init__.py
--rw-r--r--   0 juan       (501) staff       (20)      638 2024-03-18 12:31:54.000000 android-cli-1.0.8/cli/form/lokalise/lokalise_add_strings_form.py
--rw-r--r--   0 juan       (501) staff       (20)      625 2024-01-24 14:20:55.000000 android-cli-1.0.8/cli/form/lokalise/lokalise_get_strings_form.py
--rw-r--r--   0 juan       (501) staff       (20)      859 2024-01-24 14:20:55.000000 android-cli-1.0.8/cli/form/lokalise/lokalise_menu_form.py
--rw-r--r--   0 juan       (501) staff       (20)      349 2024-03-05 14:11:11.000000 android-cli-1.0.8/cli/main.py
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-03-18 12:50:10.994563 android-cli-1.0.8/cli/utils/
--rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-14 01:48:56.000000 android-cli-1.0.8/cli/utils/__init__.py
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-03-18 12:50:10.996037 android-cli-1.0.8/cli/utils/code_templates/
--rw-r--r--   0 juan       (501) staff       (20)        0 2024-03-04 16:53:48.000000 android-cli-1.0.8/cli/utils/code_templates/__init__.py
--rw-r--r--   0 juan       (501) staff       (20)     4141 2024-03-15 19:00:19.000000 android-cli-1.0.8/cli/utils/code_templates/fragment_template.py
--rw-r--r--   0 juan       (501) staff       (20)      768 2024-03-15 19:00:19.000000 android-cli-1.0.8/cli/utils/code_templates/mock_preview_template.py
--rw-r--r--   0 juan       (501) staff       (20)      879 2024-03-04 16:53:48.000000 android-cli-1.0.8/cli/utils/code_templates/update_di.py
--rw-r--r--   0 juan       (501) staff       (20)     3204 2024-03-15 19:00:19.000000 android-cli-1.0.8/cli/utils/code_templates/viewmodel_template.py
--rw-r--r--   0 juan       (501) staff       (20)      950 2024-01-24 14:46:30.000000 android-cli-1.0.8/cli/utils/configs.py
--rw-r--r--   0 juan       (501) staff       (20)      598 2024-01-24 19:37:08.000000 android-cli-1.0.8/cli/utils/editor.py
--rw-r--r--   0 juan       (501) staff       (20)     1637 2024-01-20 02:02:53.000000 android-cli-1.0.8/cli/utils/shell.py
--rw-r--r--   0 juan       (501) staff       (20)      217 2024-01-14 01:53:54.000000 android-cli-1.0.8/cli/utils/singleton.py
--rw-r--r--   0 juan       (501) staff       (20)     4891 2024-02-20 19:19:46.000000 android-cli-1.0.8/cli/utils/ui.py
--rw-r--r--   0 juan       (501) staff       (20)     1652 2024-02-19 18:53:53.000000 android-cli-1.0.8/cli/utils/ui_menu.py
--rw-r--r--   0 juan       (501) staff       (20)       38 2024-03-18 12:50:10.996736 android-cli-1.0.8/setup.cfg
--rw-r--r--   0 juan       (501) staff       (20)      445 2024-03-18 12:48:42.000000 android-cli-1.0.8/setup.py
+drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.745930 android-cli-1.0.9/
+-rw-r--r--   0 juan       (501) staff       (20)      236 2024-04-25 12:25:16.745703 android-cli-1.0.9/PKG-INFO
+drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.731128 android-cli-1.0.9/android_cli.egg-info/
+-rw-r--r--   0 juan       (501) staff       (20)      236 2024-04-25 12:25:16.000000 android-cli-1.0.9/android_cli.egg-info/PKG-INFO
+-rw-r--r--   0 juan       (501) staff       (20)     1963 2024-04-25 12:25:16.000000 android-cli-1.0.9/android_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 juan       (501) staff       (20)        1 2024-04-25 12:25:16.000000 android-cli-1.0.9/android_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 juan       (501) staff       (20)       51 2024-04-25 12:25:16.000000 android-cli-1.0.9/android_cli.egg-info/entry_points.txt
+-rw-r--r--   0 juan       (501) staff       (20)       91 2024-04-25 12:25:16.000000 android-cli-1.0.9/android_cli.egg-info/requires.txt
+-rw-r--r--   0 juan       (501) staff       (20)        4 2024-04-25 12:25:16.000000 android-cli-1.0.9/android_cli.egg-info/top_level.txt
+drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.731381 android-cli-1.0.9/cli/
+-rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-14 02:14:42.000000 android-cli-1.0.9/cli/__init__.py
+drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.734681 android-cli-1.0.9/cli/entities/
+-rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-14 02:21:04.000000 android-cli-1.0.9/cli/entities/__init__.py
+-rw-r--r--   0 juan       (501) staff       (20)     6252 2024-04-25 12:24:19.000000 android-cli-1.0.9/cli/entities/app.py
+-rw-r--r--   0 juan       (501) staff       (20)     2954 2024-03-08 20:33:40.000000 android-cli-1.0.9/cli/entities/aws.py
+-rw-r--r--   0 juan       (501) staff       (20)     5858 2024-03-05 20:01:57.000000 android-cli-1.0.9/cli/entities/bitrise.py
+-rw-r--r--   0 juan       (501) staff       (20)     2090 2024-03-05 20:01:57.000000 android-cli-1.0.9/cli/entities/fcm.py
+-rw-r--r--   0 juan       (501) staff       (20)     2600 2024-01-24 19:37:08.000000 android-cli-1.0.9/cli/entities/git.py
+-rw-r--r--   0 juan       (501) staff       (20)    13647 2024-03-04 20:18:55.000000 android-cli-1.0.9/cli/entities/jira.py
+-rw-r--r--   0 juan       (501) staff       (20)     8314 2024-04-25 12:24:19.000000 android-cli-1.0.9/cli/entities/lokalise.py
+-rw-r--r--   0 juan       (501) staff       (20)     9699 2024-03-18 12:31:54.000000 android-cli-1.0.9/cli/entities/menu.py
+-rw-r--r--   0 juan       (501) staff       (20)     6495 2024-03-05 20:01:57.000000 android-cli-1.0.9/cli/entities/setting.py
+drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.735052 android-cli-1.0.9/cli/form/
+-rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-14 22:20:43.000000 android-cli-1.0.9/cli/form/__init__.py
+-rw-r--r--   0 juan       (501) staff       (20)      682 2024-01-24 18:46:20.000000 android-cli-1.0.9/cli/form/_form_confirm.py
+drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.736474 android-cli-1.0.9/cli/form/bitrise/
+-rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-20 15:13:23.000000 android-cli-1.0.9/cli/form/bitrise/__init__.py
+-rw-r--r--   0 juan       (501) staff       (20)     2258 2024-01-24 14:18:20.000000 android-cli-1.0.9/cli/form/bitrise/branch_form.py
+-rw-r--r--   0 juan       (501) staff       (20)      676 2024-01-24 14:18:20.000000 android-cli-1.0.9/cli/form/bitrise/build_type_form.py
+-rw-r--r--   0 juan       (501) staff       (20)     1489 2024-02-09 17:02:00.000000 android-cli-1.0.9/cli/form/bitrise/release_notes_form.py
+-rw-r--r--   0 juan       (501) staff       (20)     2542 2024-01-29 12:48:34.000000 android-cli-1.0.9/cli/form/bitrise/version_code_form.py
+-rw-r--r--   0 juan       (501) staff       (20)     2368 2024-01-24 14:18:20.000000 android-cli-1.0.9/cli/form/bitrise/version_name_form.py
+drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.737023 android-cli-1.0.9/cli/form/code_gen/
+-rw-r--r--   0 juan       (501) staff       (20)        0 2024-03-04 16:53:48.000000 android-cli-1.0.9/cli/form/code_gen/__init__.py
+-rw-r--r--   0 juan       (501) staff       (20)      657 2024-03-04 16:53:48.000000 android-cli-1.0.9/cli/form/code_gen/code_gen_form.py
+-rw-r--r--   0 juan       (501) staff       (20)     3698 2024-04-25 12:24:19.000000 android-cli-1.0.9/cli/form/code_gen/create_new_screen.py
+drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.738021 android-cli-1.0.9/cli/form/fcm/
+-rw-r--r--   0 juan       (501) staff       (20)        0 2024-03-05 20:01:57.000000 android-cli-1.0.9/cli/form/fcm/__init__.py
+-rw-r--r--   0 juan       (501) staff       (20)     1194 2024-03-05 20:01:57.000000 android-cli-1.0.9/cli/form/fcm/fcm_firebase_id_form.py
+-rw-r--r--   0 juan       (501) staff       (20)      456 2024-03-05 20:01:57.000000 android-cli-1.0.9/cli/form/fcm/fcm_notification_body_form.py
+-rw-r--r--   0 juan       (501) staff       (20)      514 2024-03-05 20:01:57.000000 android-cli-1.0.9/cli/form/fcm/fcm_notification_deeplink_form.py
+-rw-r--r--   0 juan       (501) staff       (20)      460 2024-03-05 20:01:57.000000 android-cli-1.0.9/cli/form/fcm/fcm_notification_title_form.py
+drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.740012 android-cli-1.0.9/cli/form/git/
+-rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-24 12:50:52.000000 android-cli-1.0.9/cli/form/git/__init__.py
+-rw-r--r--   0 juan       (501) staff       (20)     3035 2024-01-24 18:46:20.000000 android-cli-1.0.9/cli/form/git/_new_branch_form.py
+-rw-r--r--   0 juan       (501) staff       (20)     4193 2024-01-24 20:09:48.000000 android-cli-1.0.9/cli/form/git/_pull_request_form.py
+-rw-r--r--   0 juan       (501) staff       (20)     2242 2024-01-24 19:15:46.000000 android-cli-1.0.9/cli/form/git/create_new_branch.py
+-rw-r--r--   0 juan       (501) staff       (20)     4012 2024-02-01 20:35:53.000000 android-cli-1.0.9/cli/form/git/create_new_pull_request.py
+-rw-r--r--   0 juan       (501) staff       (20)      673 2024-01-24 19:45:29.000000 android-cli-1.0.9/cli/form/git/git_form.py
+drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.741778 android-cli-1.0.9/cli/form/jira/
+-rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-23 15:51:10.000000 android-cli-1.0.9/cli/form/jira/__init__.py
+-rw-r--r--   0 juan       (501) staff       (20)      458 2024-02-01 18:44:37.000000 android-cli-1.0.9/cli/form/jira/jira_description_form.py
+-rw-r--r--   0 juan       (501) staff       (20)      611 2024-03-05 20:02:08.000000 android-cli-1.0.9/cli/form/jira/jira_issue_form.py
+-rw-r--r--   0 juan       (501) staff       (20)      791 2024-02-14 12:28:45.000000 android-cli-1.0.9/cli/form/jira/jira_release_start_date_form.py
+-rw-r--r--   0 juan       (501) staff       (20)      749 2024-02-14 12:27:50.000000 android-cli-1.0.9/cli/form/jira/jira_release_version_form.py
+-rw-r--r--   0 juan       (501) staff       (20)      640 2024-02-01 20:23:20.000000 android-cli-1.0.9/cli/form/jira/jira_title_form.py
+drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.742857 android-cli-1.0.9/cli/form/lokalise/
+-rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-20 15:15:41.000000 android-cli-1.0.9/cli/form/lokalise/__init__.py
+-rw-r--r--   0 juan       (501) staff       (20)      638 2024-03-18 12:31:54.000000 android-cli-1.0.9/cli/form/lokalise/lokalise_add_strings_form.py
+-rw-r--r--   0 juan       (501) staff       (20)      625 2024-01-24 14:20:55.000000 android-cli-1.0.9/cli/form/lokalise/lokalise_get_strings_form.py
+-rw-r--r--   0 juan       (501) staff       (20)      859 2024-01-24 14:20:55.000000 android-cli-1.0.9/cli/form/lokalise/lokalise_menu_form.py
+-rw-r--r--   0 juan       (501) staff       (20)      349 2024-03-05 14:11:11.000000 android-cli-1.0.9/cli/main.py
+drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.744311 android-cli-1.0.9/cli/utils/
+-rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-14 01:48:56.000000 android-cli-1.0.9/cli/utils/__init__.py
+drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.745372 android-cli-1.0.9/cli/utils/code_templates/
+-rw-r--r--   0 juan       (501) staff       (20)        0 2024-03-04 16:53:48.000000 android-cli-1.0.9/cli/utils/code_templates/__init__.py
+-rw-r--r--   0 juan       (501) staff       (20)     4141 2024-03-15 19:00:19.000000 android-cli-1.0.9/cli/utils/code_templates/fragment_template.py
+-rw-r--r--   0 juan       (501) staff       (20)      768 2024-03-15 19:00:19.000000 android-cli-1.0.9/cli/utils/code_templates/mock_preview_template.py
+-rw-r--r--   0 juan       (501) staff       (20)      879 2024-03-04 16:53:48.000000 android-cli-1.0.9/cli/utils/code_templates/update_di.py
+-rw-r--r--   0 juan       (501) staff       (20)     3204 2024-03-15 19:00:19.000000 android-cli-1.0.9/cli/utils/code_templates/viewmodel_template.py
+-rw-r--r--   0 juan       (501) staff       (20)      950 2024-01-24 14:46:30.000000 android-cli-1.0.9/cli/utils/configs.py
+-rw-r--r--   0 juan       (501) staff       (20)      598 2024-01-24 19:37:08.000000 android-cli-1.0.9/cli/utils/editor.py
+-rw-r--r--   0 juan       (501) staff       (20)     1637 2024-01-20 02:02:53.000000 android-cli-1.0.9/cli/utils/shell.py
+-rw-r--r--   0 juan       (501) staff       (20)      217 2024-01-14 01:53:54.000000 android-cli-1.0.9/cli/utils/singleton.py
+-rw-r--r--   0 juan       (501) staff       (20)     4891 2024-02-20 19:19:46.000000 android-cli-1.0.9/cli/utils/ui.py
+-rw-r--r--   0 juan       (501) staff       (20)     1652 2024-02-19 18:53:53.000000 android-cli-1.0.9/cli/utils/ui_menu.py
+-rw-r--r--   0 juan       (501) staff       (20)       38 2024-04-25 12:25:16.745976 android-cli-1.0.9/setup.cfg
+-rw-r--r--   0 juan       (501) staff       (20)      445 2024-04-25 12:24:19.000000 android-cli-1.0.9/setup.py
```

### Comparing `android-cli-1.0.8/android_cli.egg-info/SOURCES.txt` & `android-cli-1.0.9/android_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/entities/app.py` & `android-cli-1.0.9/cli/entities/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from cli.entities.setting import Settings
 from cli.utils.singleton import singleton
 import questionary
 
 
 @singleton
 class App:
-    version: str = "1.0.8"
+    version: str = "1.0.9"
 
     def init(self):
         os.system('printf "\033c"')
         os.system('cls' if os.name == 'nt' else 'clear')
 
         print(f"Press [enter] to start GIT-CLI {self.version}")
```

### Comparing `android-cli-1.0.8/cli/entities/aws.py` & `android-cli-1.0.9/cli/entities/aws.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/entities/bitrise.py` & `android-cli-1.0.9/cli/entities/bitrise.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/entities/fcm.py` & `android-cli-1.0.9/cli/entities/fcm.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/entities/git.py` & `android-cli-1.0.9/cli/entities/git.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/entities/jira.py` & `android-cli-1.0.9/cli/entities/jira.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/entities/lokalise.py` & `android-cli-1.0.9/cli/entities/lokalise.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         spinner_thread.start()
 
         try:
             files = self.client.download_files(self.credentials['project_id'], {
                 "format": "xml",
                 "original_filenames": True,
                 "replace_breaks": False,
-                "export_empty_as": "base"
+                "export_empty_as": "skip"
             })
         finally:
             is_loading.clear()
             spinner_thread.join()
 
         return files
 
@@ -175,14 +175,18 @@
                     zip_info.filename = "values-ja/strings.xml"
                     zip_file.extract(zip_info, 'core/common/src/main/res')
 
                 if zip_info.filename == "values-pt-rBR/pt-rBR.xml":
                     zip_info.filename = "values-pt-rBR/strings.xml"
                     zip_file.extract(zip_info, 'core/common/src/main/res')
 
+                if zip_info.filename == "values-es-rAR/es-rAR.xml":
+                    zip_info.filename = "values-es-rAR/strings.xml"
+                    zip_file.extract(zip_info, 'core/common/src/main/res')
+
                 if zip_info.filename == "values-ru/ru.xml":
                     zip_info.filename = "values-ru/strings.xml"
                     zip_file.extract(zip_info, 'core/common/src/main/res')
 
                 if zip_info.filename == "values-ko/ko.xml":
                     zip_info.filename = "values-ko-rKR/strings.xml"
                     zip_file.extract(zip_info, 'core/common/src/main/res')
```

### Comparing `android-cli-1.0.8/cli/entities/menu.py` & `android-cli-1.0.9/cli/entities/menu.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/entities/setting.py` & `android-cli-1.0.9/cli/entities/setting.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/form/_form_confirm.py` & `android-cli-1.0.9/cli/form/_form_confirm.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/form/bitrise/branch_form.py` & `android-cli-1.0.9/cli/form/bitrise/branch_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/form/bitrise/build_type_form.py` & `android-cli-1.0.9/cli/form/bitrise/build_type_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/form/bitrise/release_notes_form.py` & `android-cli-1.0.9/cli/form/bitrise/release_notes_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/form/bitrise/version_code_form.py` & `android-cli-1.0.9/cli/form/bitrise/version_code_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/form/bitrise/version_name_form.py` & `android-cli-1.0.9/cli/form/bitrise/version_name_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/form/code_gen/code_gen_form.py` & `android-cli-1.0.9/cli/form/code_gen/code_gen_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/form/code_gen/create_new_screen.py` & `android-cli-1.0.9/cli/form/code_gen/create_new_screen.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 from cli.utils.code_templates.viewmodel_template import create_viewmodel
 import questionary
 from cli.form._form_confirm import confirm_question
 from cli.utils.shell import Shell
 from cli.utils.ui import UI
 from cli.utils.configs import custom_style
 
+def _adjust_path_to_os(path):
+    return path.replace("/", os.sep)
+
 def _get_directories():
     list = os.listdir(".")
     filtered = []
     for item in list:
         if os.path.isdir(item):
             filtered.append(item)
     filtered.sort()
@@ -36,16 +39,18 @@
                 'name': 'module',
                 'message': 'Module?',
                 'choices': list,
                 'style': custom_style
             }
         )
     os.chdir(result['module'])
-    feature_name = os.getcwd().split("/")[-1].replace("-", "_")
-    os.chdir("src/main/kotlin/com/astropaycard/android/feature/" + feature_name)
+    feature_name = os.getcwd().split(os.sep)[-1].replace("-", "_")
+    new_path = _adjust_path_to_os("src/main/kotlin/com/astropaycard/android/feature/" + feature_name)
+    os.chdir(new_path)
+
 
 def _package_form():
     list = _get_directories()
     list.insert(0, "[CREATE HERE]")
 
     UI().ptext('<g>Picking directory</g>')
     result = questionary.unsafe_prompt(
@@ -81,15 +86,15 @@
                         'type': 'input',
                         'name': 'name',
                         'message': f'Enter screen name',
                         'validate': lambda val: 'Title cannot be empty' if not val else True
                     }])["name"]
 
 def create_new_screen():
-    di_path = os.getcwd() + "/app/src/main/kotlin/com/astropaycard/android/di"
+    di_path = _adjust_path_to_os(os.getcwd() + "/app/src/main/kotlin/com/astropaycard/android/di")
     os.chdir("feature")
 
     UI().clear()
     _print_header()
     _module_form()
 
     package = "-"
@@ -104,14 +109,15 @@
     _print_header()
     _new_package_form()
 
     UI().clear()
     _print_header()
     screen_name = _new_screen_form()
 
-    package_to_import = os.getcwd().split("src/main/kotlin/")[1].replace("/",".")
+    adjusted_path = _adjust_path_to_os("src/main/kotlin/")
+    package_to_import = os.getcwd().split(adjusted_path)[1].replace(os.sep,".")
     create_fragment(screen_name, package_to_import)
     create_viewmodel(screen_name, package_to_import)
     create_mock_preview(screen_name, package_to_import)
     update_di(di_path, screen_name, package_to_import)
     UI().psuccess()
```

### Comparing `android-cli-1.0.8/cli/form/fcm/fcm_firebase_id_form.py` & `android-cli-1.0.9/cli/form/fcm/fcm_firebase_id_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/form/fcm/fcm_notification_deeplink_form.py` & `android-cli-1.0.9/cli/form/fcm/fcm_notification_deeplink_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/form/git/_new_branch_form.py` & `android-cli-1.0.9/cli/form/git/_new_branch_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/form/git/_pull_request_form.py` & `android-cli-1.0.9/cli/form/git/_pull_request_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/form/git/create_new_branch.py` & `android-cli-1.0.9/cli/form/git/create_new_branch.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/form/git/create_new_pull_request.py` & `android-cli-1.0.9/cli/form/git/create_new_pull_request.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/form/git/git_form.py` & `android-cli-1.0.9/cli/form/git/git_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/form/jira/jira_issue_form.py` & `android-cli-1.0.9/cli/form/jira/jira_issue_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/form/jira/jira_release_start_date_form.py` & `android-cli-1.0.9/cli/form/jira/jira_release_start_date_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/form/jira/jira_release_version_form.py` & `android-cli-1.0.9/cli/form/jira/jira_release_version_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/form/jira/jira_title_form.py` & `android-cli-1.0.9/cli/form/jira/jira_title_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/form/lokalise/lokalise_add_strings_form.py` & `android-cli-1.0.9/cli/form/lokalise/lokalise_add_strings_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/form/lokalise/lokalise_get_strings_form.py` & `android-cli-1.0.9/cli/form/lokalise/lokalise_get_strings_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/form/lokalise/lokalise_menu_form.py` & `android-cli-1.0.9/cli/form/lokalise/lokalise_menu_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/utils/code_templates/fragment_template.py` & `android-cli-1.0.9/cli/utils/code_templates/fragment_template.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/utils/code_templates/mock_preview_template.py` & `android-cli-1.0.9/cli/utils/code_templates/mock_preview_template.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/utils/code_templates/update_di.py` & `android-cli-1.0.9/cli/utils/code_templates/update_di.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/utils/code_templates/viewmodel_template.py` & `android-cli-1.0.9/cli/utils/code_templates/viewmodel_template.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/utils/configs.py` & `android-cli-1.0.9/cli/utils/configs.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/utils/editor.py` & `android-cli-1.0.9/cli/utils/editor.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/utils/shell.py` & `android-cli-1.0.9/cli/utils/shell.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/utils/ui.py` & `android-cli-1.0.9/cli/utils/ui.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.8/cli/utils/ui_menu.py` & `android-cli-1.0.9/cli/utils/ui_menu.py`

 * *Files identical despite different names*

