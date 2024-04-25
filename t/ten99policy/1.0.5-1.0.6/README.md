# Comparing `tmp/ten99policy-1.0.5.tar.gz` & `tmp/ten99policy-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ten99policy-1.0.5.tar", last modified: Tue Apr 16 20:16:31 2024, max compression
+gzip compressed data, was "ten99policy-1.0.6.tar", last modified: Thu Apr 25 14:16:20 2024, max compression
```

## Comparing `ten99policy-1.0.5.tar` & `ten99policy-1.0.6.tar`

### file list

```diff
@@ -1,71 +1,73 @@
-drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-16 20:16:31.163683 ten99policy-1.0.5/
-drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-16 20:16:31.149122 ten99policy-1.0.5/.circleci/
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     2971 2022-06-14 14:49:57.000000 ten99policy-1.0.5/.circleci/config.yml
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      386 2022-06-14 14:49:57.000000 ten99policy-1.0.5/.codeclimate.yml
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      252 2022-06-14 14:49:57.000000 ten99policy-1.0.5/.editorconfig
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      366 2022-06-16 06:33:50.000000 ten99policy-1.0.5/.flake8
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      667 2022-06-14 14:49:57.000000 ten99policy-1.0.5/.gitignore
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1106 2022-06-16 06:45:19.000000 ten99policy-1.0.5/LICENSE
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1584 2024-04-16 20:16:31.163595 ten99policy-1.0.5/PKG-INFO
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     3469 2022-06-16 06:46:37.000000 ten99policy-1.0.5/README.md
--rw-r--r--   0 cfkarakulak   (501) staff       (20)        6 2024-04-16 20:15:21.000000 ten99policy-1.0.5/VERSION
-drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-16 20:16:31.151175 ten99policy-1.0.5/examples/
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1640 2022-12-26 18:25:47.000000 ten99policy-1.0.5/examples/assignments.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      633 2024-04-16 12:38:39.000000 ten99policy-1.0.5/examples/contractors.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1889 2022-07-21 17:45:39.000000 ten99policy-1.0.5/examples/entities.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      673 2022-12-25 22:04:06.000000 ten99policy-1.0.5/examples/events.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1204 2022-11-02 16:58:51.000000 ten99policy-1.0.5/examples/insurance_application_sessions.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1718 2022-07-21 17:45:39.000000 ten99policy-1.0.5/examples/invoices.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1693 2023-03-26 18:07:20.000000 ten99policy-1.0.5/examples/jobs.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1576 2022-07-21 17:45:39.000000 ten99policy-1.0.5/examples/policies.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1331 2023-02-28 10:16:19.000000 ten99policy-1.0.5/examples/quotes.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1106 2024-04-16 12:23:08.000000 ten99policy-1.0.5/requirements.txt
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      102 2024-04-16 20:16:31.163970 ten99policy-1.0.5/setup.cfg
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     2060 2022-06-16 06:46:58.000000 ten99policy-1.0.5/setup.py
-drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-16 20:16:31.154145 ten99policy-1.0.5/ten99policy/
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      476 2022-12-25 22:03:41.000000 ten99policy-1.0.5/ten99policy/__init__.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)    11598 2024-04-16 12:37:14.000000 ten99policy-1.0.5/ten99policy/api_requestor.py
-drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-16 20:16:31.160902 ten99policy-1.0.5/ten99policy/api_resources/
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      788 2022-12-26 18:25:47.000000 ten99policy-1.0.5/ten99policy/api_resources/__init__.py
-drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-16 20:16:31.162540 ten99policy-1.0.5/ten99policy/api_resources/abstract/
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      799 2022-06-16 06:30:18.000000 ten99policy-1.0.5/ten99policy/api_resources/abstract/__init__.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     3093 2022-12-25 22:04:06.000000 ten99policy-1.0.5/ten99policy/api_resources/abstract/api_resource.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      869 2022-12-25 22:04:06.000000 ten99policy-1.0.5/ten99policy/api_resources/abstract/createable_api_resource.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     2081 2022-06-16 06:33:37.000000 ten99policy-1.0.5/ten99policy/api_resources/abstract/custom_method.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      634 2022-06-16 06:33:37.000000 ten99policy-1.0.5/ten99policy/api_resources/abstract/deletable_api_resource.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1062 2024-04-16 12:23:13.000000 ten99policy-1.0.5/ten99policy/api_resources/abstract/listable_api_resource.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     4418 2022-12-25 22:04:06.000000 ten99policy-1.0.5/ten99policy/api_resources/abstract/nested_resource_class_methods.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      883 2022-06-16 06:30:18.000000 ten99policy-1.0.5/ten99policy/api_resources/abstract/singleton_api_resource.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      900 2022-06-16 06:33:37.000000 ten99policy-1.0.5/ten99policy/api_resources/abstract/updateable_api_resource.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      434 2022-12-26 18:25:47.000000 ten99policy-1.0.5/ten99policy/api_resources/assignments.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      434 2022-06-16 06:30:18.000000 ten99policy-1.0.5/ten99policy/api_resources/contractors.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      428 2022-06-16 06:30:18.000000 ten99policy-1.0.5/ten99policy/api_resources/entities.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      594 2022-12-25 22:04:06.000000 ten99policy-1.0.5/ten99policy/api_resources/error_object.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      138 2022-12-25 22:04:06.000000 ten99policy-1.0.5/ten99policy/api_resources/events.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      264 2022-06-16 06:30:18.000000 ten99policy-1.0.5/ten99policy/api_resources/insurance_application_sessions.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      428 2022-06-16 06:30:18.000000 ten99policy-1.0.5/ten99policy/api_resources/invoices.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      420 2022-06-16 06:30:18.000000 ten99policy-1.0.5/ten99policy/api_resources/jobs.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     5800 2022-12-25 22:04:06.000000 ten99policy-1.0.5/ten99policy/api_resources/list_object.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      428 2022-06-16 06:30:18.000000 ten99policy-1.0.5/ten99policy/api_resources/policies.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      330 2022-06-16 06:30:18.000000 ten99policy-1.0.5/ten99policy/api_resources/quotes.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     3999 2022-06-16 06:45:08.000000 ten99policy-1.0.5/ten99policy/error.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)    24625 2022-06-16 06:45:08.000000 ten99policy-1.0.5/ten99policy/http_client.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     2775 2022-06-16 06:30:17.000000 ten99policy-1.0.5/ten99policy/multipart_data_generator.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      570 2022-06-16 06:33:37.000000 ten99policy-1.0.5/ten99policy/object_classes.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)    32463 2022-06-14 14:49:57.000000 ten99policy-1.0.5/ten99policy/six.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)    12243 2022-12-25 22:04:06.000000 ten99policy-1.0.5/ten99policy/ten99policy_object.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      998 2022-06-16 06:35:38.000000 ten99policy-1.0.5/ten99policy/ten99policy_response.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     6972 2022-12-25 22:04:06.000000 ten99policy-1.0.5/ten99policy/util.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)       18 2024-04-16 20:15:33.000000 ten99policy-1.0.5/ten99policy/version.py
-drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-16 20:16:31.163240 ten99policy-1.0.5/ten99policy.egg-info/
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1584 2024-04-16 20:16:31.000000 ten99policy-1.0.5/ten99policy.egg-info/PKG-INFO
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1946 2024-04-16 20:16:31.000000 ten99policy-1.0.5/ten99policy.egg-info/SOURCES.txt
--rw-r--r--   0 cfkarakulak   (501) staff       (20)        1 2024-04-16 20:16:31.000000 ten99policy-1.0.5/ten99policy.egg-info/dependency_links.txt
--rw-r--r--   0 cfkarakulak   (501) staff       (20)        1 2022-08-04 07:33:51.000000 ten99policy-1.0.5/ten99policy.egg-info/not-zip-safe
--rw-r--r--   0 cfkarakulak   (501) staff       (20)       95 2024-04-16 20:16:31.000000 ten99policy-1.0.5/ten99policy.egg-info/requires.txt
--rw-r--r--   0 cfkarakulak   (501) staff       (20)       12 2024-04-16 20:16:31.000000 ten99policy-1.0.5/ten99policy.egg-info/top_level.txt
-drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-16 20:16:31.162779 ten99policy-1.0.5/tests/
--rw-r--r--   0 cfkarakulak   (501) staff       (20)        0 2022-06-14 14:49:57.000000 ten99policy-1.0.5/tests/__init__.py
-drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-16 20:16:31.163018 ten99policy-1.0.5/tests/api_resources/
--rw-r--r--   0 cfkarakulak   (501) staff       (20)        0 2022-06-14 14:49:57.000000 ten99policy-1.0.5/tests/api_resources/__init__.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      404 2022-06-16 06:30:17.000000 ten99policy-1.0.5/tests/api_resources/test_customer.py
+drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-25 14:16:20.058433 ten99policy-1.0.6/
+drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-25 14:16:20.038868 ten99policy-1.0.6/.circleci/
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     2971 2022-06-14 14:49:57.000000 ten99policy-1.0.6/.circleci/config.yml
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      386 2022-06-14 14:49:57.000000 ten99policy-1.0.6/.codeclimate.yml
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      252 2022-06-14 14:49:57.000000 ten99policy-1.0.6/.editorconfig
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      366 2022-06-16 06:33:50.000000 ten99policy-1.0.6/.flake8
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      667 2022-06-14 14:49:57.000000 ten99policy-1.0.6/.gitignore
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1106 2022-06-16 06:45:19.000000 ten99policy-1.0.6/LICENSE
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1584 2024-04-25 14:16:20.058346 ten99policy-1.0.6/PKG-INFO
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     3469 2022-06-16 06:46:37.000000 ten99policy-1.0.6/README.md
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)        6 2024-04-25 14:07:19.000000 ten99policy-1.0.6/VERSION
+drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-25 14:16:20.041191 ten99policy-1.0.6/examples/
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1649 2024-04-25 14:09:18.000000 ten99policy-1.0.6/examples/assignments.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      425 2024-04-25 14:09:06.000000 ten99policy-1.0.6/examples/contractor_policies.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1928 2024-04-25 14:15:01.000000 ten99policy-1.0.6/examples/contractors.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1902 2024-04-25 14:11:30.000000 ten99policy-1.0.6/examples/entities.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      675 2024-04-25 14:09:47.000000 ten99policy-1.0.6/examples/events.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1215 2024-04-25 14:09:50.000000 ten99policy-1.0.6/examples/insurance_application_sessions.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1729 2024-04-25 14:09:55.000000 ten99policy-1.0.6/examples/invoices.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1704 2024-04-25 14:09:59.000000 ten99policy-1.0.6/examples/jobs.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1588 2024-04-25 14:10:08.000000 ten99policy-1.0.6/examples/policies.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1340 2024-04-25 14:10:11.000000 ten99policy-1.0.6/examples/quotes.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1106 2024-04-16 12:23:08.000000 ten99policy-1.0.6/requirements.txt
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      102 2024-04-25 14:16:20.058777 ten99policy-1.0.6/setup.cfg
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     2060 2022-06-16 06:46:58.000000 ten99policy-1.0.6/setup.py
+drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-25 14:16:20.044737 ten99policy-1.0.6/ten99policy/
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      481 2024-04-25 14:11:22.000000 ten99policy-1.0.6/ten99policy/__init__.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)    11598 2024-04-16 12:37:14.000000 ten99policy-1.0.6/ten99policy/api_requestor.py
+drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-25 14:16:20.048811 ten99policy-1.0.6/ten99policy/api_resources/
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      865 2024-04-25 11:31:34.000000 ten99policy-1.0.6/ten99policy/api_resources/__init__.py
+drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-25 14:16:20.057248 ten99policy-1.0.6/ten99policy/api_resources/abstract/
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      799 2022-06-16 06:30:18.000000 ten99policy-1.0.6/ten99policy/api_resources/abstract/__init__.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     3094 2024-04-25 13:26:54.000000 ten99policy-1.0.6/ten99policy/api_resources/abstract/api_resource.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      869 2022-12-25 22:04:06.000000 ten99policy-1.0.6/ten99policy/api_resources/abstract/createable_api_resource.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     2081 2022-06-16 06:33:37.000000 ten99policy-1.0.6/ten99policy/api_resources/abstract/custom_method.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      634 2022-06-16 06:33:37.000000 ten99policy-1.0.6/ten99policy/api_resources/abstract/deletable_api_resource.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1193 2024-04-25 13:27:51.000000 ten99policy-1.0.6/ten99policy/api_resources/abstract/listable_api_resource.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     4418 2022-12-25 22:04:06.000000 ten99policy-1.0.6/ten99policy/api_resources/abstract/nested_resource_class_methods.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      883 2022-06-16 06:30:18.000000 ten99policy-1.0.6/ten99policy/api_resources/abstract/singleton_api_resource.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      900 2022-06-16 06:33:37.000000 ten99policy-1.0.6/ten99policy/api_resources/abstract/updateable_api_resource.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      434 2022-12-26 18:25:47.000000 ten99policy-1.0.6/ten99policy/api_resources/assignments.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      167 2024-04-25 12:11:20.000000 ten99policy-1.0.6/ten99policy/api_resources/contractor_policies.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      434 2022-06-16 06:30:18.000000 ten99policy-1.0.6/ten99policy/api_resources/contractors.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      428 2022-06-16 06:30:18.000000 ten99policy-1.0.6/ten99policy/api_resources/entities.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      594 2022-12-25 22:04:06.000000 ten99policy-1.0.6/ten99policy/api_resources/error_object.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      138 2022-12-25 22:04:06.000000 ten99policy-1.0.6/ten99policy/api_resources/events.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      264 2022-06-16 06:30:18.000000 ten99policy-1.0.6/ten99policy/api_resources/insurance_application_sessions.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      428 2022-06-16 06:30:18.000000 ten99policy-1.0.6/ten99policy/api_resources/invoices.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      420 2022-06-16 06:30:18.000000 ten99policy-1.0.6/ten99policy/api_resources/jobs.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     5800 2022-12-25 22:04:06.000000 ten99policy-1.0.6/ten99policy/api_resources/list_object.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      428 2022-06-16 06:30:18.000000 ten99policy-1.0.6/ten99policy/api_resources/policies.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      330 2022-06-16 06:30:18.000000 ten99policy-1.0.6/ten99policy/api_resources/quotes.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     3999 2022-06-16 06:45:08.000000 ten99policy-1.0.6/ten99policy/error.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)    24625 2022-06-16 06:45:08.000000 ten99policy-1.0.6/ten99policy/http_client.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     2775 2022-06-16 06:30:17.000000 ten99policy-1.0.6/ten99policy/multipart_data_generator.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      570 2022-06-16 06:33:37.000000 ten99policy-1.0.6/ten99policy/object_classes.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)    32463 2024-04-25 12:11:53.000000 ten99policy-1.0.6/ten99policy/six.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)    12315 2024-04-25 13:23:06.000000 ten99policy-1.0.6/ten99policy/ten99policy_object.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      998 2022-06-16 06:35:38.000000 ten99policy-1.0.6/ten99policy/ten99policy_response.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     6972 2022-12-25 22:04:06.000000 ten99policy-1.0.6/ten99policy/util.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)       18 2024-04-25 14:15:58.000000 ten99policy-1.0.6/ten99policy/version.py
+drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-25 14:16:20.058026 ten99policy-1.0.6/ten99policy.egg-info/
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1584 2024-04-25 14:16:19.000000 ten99policy-1.0.6/ten99policy.egg-info/PKG-INFO
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     2027 2024-04-25 14:16:20.000000 ten99policy-1.0.6/ten99policy.egg-info/SOURCES.txt
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)        1 2024-04-25 14:16:19.000000 ten99policy-1.0.6/ten99policy.egg-info/dependency_links.txt
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)        1 2022-08-04 07:33:51.000000 ten99policy-1.0.6/ten99policy.egg-info/not-zip-safe
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)       95 2024-04-25 14:16:19.000000 ten99policy-1.0.6/ten99policy.egg-info/requires.txt
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)       12 2024-04-25 14:16:19.000000 ten99policy-1.0.6/ten99policy.egg-info/top_level.txt
+drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-25 14:16:20.057557 ten99policy-1.0.6/tests/
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)        0 2022-06-14 14:49:57.000000 ten99policy-1.0.6/tests/__init__.py
+drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-25 14:16:20.057796 ten99policy-1.0.6/tests/api_resources/
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)        0 2022-06-14 14:49:57.000000 ten99policy-1.0.6/tests/api_resources/__init__.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      404 2022-06-16 06:30:17.000000 ten99policy-1.0.6/tests/api_resources/test_customer.py
```

### Comparing `ten99policy-1.0.5/.circleci/config.yml` & `ten99policy-1.0.6/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.5/.gitignore` & `ten99policy-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.5/LICENSE` & `ten99policy-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.5/PKG-INFO` & `ten99policy-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ten99policy
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python bindings for the ten99policy API
 Home-page: https://github.com/1099policy/1099policy-client-python
 Author: Ray Ventura
 Author-email: support@1099policy.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/1099policy/1099policy-client-python/issues
 Project-URL: Documentation, https://1099policy.com/docs/api/?lang=python
```

### Comparing `ten99policy-1.0.5/README.md` & `ten99policy-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.5/examples/assignments.py` & `ten99policy-1.0.6/examples/assignments.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,30 +10,31 @@
 resource = ten99policy.Assignments.create(
     contractor="cn_kjLKMtApTv",
     job="jb_D6ZSaoa2MV",
 )
 
 # -----------------------------------------------------------------------------------*/
 # Updating an assignment (replace xxx with an existing assignment id)
-#-----------------------------------------------------------------------------------*/
+# -----------------------------------------------------------------------------------*/
 
-resource = ten99policy.Assignments.modify('an_sF3yUB3BYY',
-    contractor='cn_kjLKMtApTv',
+resource = ten99policy.Assignments.modify(
+    "an_sF3yUB3BYY",
+    contractor="cn_kjLKMtApTv",
 )
 
 # -----------------------------------------------------------------------------------*/
 # Fetching the list of Assignments
-#-----------------------------------------------------------------------------------*/
+# -----------------------------------------------------------------------------------*/
 
 resource = ten99policy.Assignments.list()
 
 # -----------------------------------------------------------------------------------*/
 # Retrieving an assignment (replace xxx with an existing assignment id)
-#-----------------------------------------------------------------------------------*/
+# -----------------------------------------------------------------------------------*/
 
-resource = ten99policy.Assignments.retrieve('en_BUcNa8jMrq')
+resource = ten99policy.Assignments.retrieve("en_BUcNa8jMrq")
 
 # -----------------------------------------------------------------------------------*/
 # Delete an assignment (replace xxx with an existing assignment id)
-#-----------------------------------------------------------------------------------*/
+# -----------------------------------------------------------------------------------*/
 
-resource = ten99policy.Assignments.delete('as_xyz')
+resource = ten99policy.Assignments.delete("as_xyz")
```

### Comparing `ten99policy-1.0.5/examples/entities.py` & `ten99policy-1.0.6/examples/entities.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 import ten99policy
 
 # You can configure the environment for 1099Policy API (sandbox|production)
 # ten99policy.environment = 'sandbox'
 
 # -----------------------------------------------------------------------------------*/
 # Creating an entity
-#-----------------------------------------------------------------------------------*/
+# -----------------------------------------------------------------------------------*/
 
 resource = ten99policy.Entities.create(
     name="Brooklyn Bowl",
     coverage_limit={
         "aggregate_limit": "200000000",
-        "occurrence_limit": "100000000"
+        "occurrence_limit": "100000000",
     },
     address={
         "line1": "3639 18th St",
         "line2": "",
         "locality": "San Francisco",
         "region": "CA",
-        "postalcode": "94110"
+        "postalcode": "94110",
     },
-    required_coverage=["general", "workers-comp"]
+    required_coverage=["general", "workers-comp"],
 )
 
 # -----------------------------------------------------------------------------------*/
 # Updating an entity (replace xxx with an existing entity id)
-#-----------------------------------------------------------------------------------*/
+# -----------------------------------------------------------------------------------*/
 
-resource = ten99policy.Entities.modify('en_C9Z2DmfHSF',
-    name='California Roll',
+resource = ten99policy.Entities.modify(
+    "en_C9Z2DmfHSF",
+    name="California Roll",
 )
 
 # -----------------------------------------------------------------------------------*/
 # Fetching the list of entities
-#-----------------------------------------------------------------------------------*/
+# -----------------------------------------------------------------------------------*/
 
 resource = ten99policy.Entities.list()
 
 # -----------------------------------------------------------------------------------*/
 # Retrieving an entity (replace xxx with an existing entity id)
-#-----------------------------------------------------------------------------------*/
+# -----------------------------------------------------------------------------------*/
 
-resource = ten99policy.Entities.retrieve('en_BUcNa8jMrq')
+resource = ten99policy.Entities.retrieve("en_BUcNa8jMrq")
 
 # -----------------------------------------------------------------------------------*/
 # Delete an entity (replace xxx with an existing entity id)
-#-----------------------------------------------------------------------------------*/
+# -----------------------------------------------------------------------------------*/
 
-resource = ten99policy.Entities.delete('en_C9Z2DmfHSF')
+resource = ten99policy.Entities.delete("en_C9Z2DmfHSF")
```

### Comparing `ten99policy-1.0.5/examples/events.py` & `ten99policy-1.0.6/examples/events.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import ten99policy
 
 # You can configure the environment for 1099Policy API (sandbox|production)
 # ten99policy.environment = 'sandbox'
 
 # -----------------------------------------------------------------------------------*/
 # Fetching the list of events
-#-----------------------------------------------------------------------------------*/
+# -----------------------------------------------------------------------------------*/
 
 resource = ten99policy.Events.list()
 
 # -----------------------------------------------------------------------------------*/
 # Retrieving an event (replace xxx with an existing event id)
-#-----------------------------------------------------------------------------------*/
+# -----------------------------------------------------------------------------------*/
 
-resource = ten99policy.Events.retrieve('wh_D1Z2DmgHSF')
+resource = ten99policy.Events.retrieve("wh_D1Z2DmgHSF")
```

### Comparing `ten99policy-1.0.5/examples/insurance_application_sessions.py` & `ten99policy-1.0.6/examples/insurance_application_sessions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import ten99policy
 
 # You can configure the environment for 1099Policy API (sandbox|production)
 # ten99policy.environment = 'sandbox'
 
 # -----------------------------------------------------------------------------------*/
 # Creating an insurance application session
-#-----------------------------------------------------------------------------------*/
+# -----------------------------------------------------------------------------------*/
 
 resource = ten99policy.InsuranceApplicationSessions.create(
     quote="qt_yVEnbNaWh6",
     success_url="http://example.com/success",
-    cancel_url="http://example.com/cancel"
+    cancel_url="http://example.com/cancel",
 )
 
 # -----------------------------------------------------------------------------------*/
 # Fetching the list of insurance application sessions
-#-----------------------------------------------------------------------------------*/
+# -----------------------------------------------------------------------------------*/
 
 resource = ten99policy.InsuranceApplicationSessions.list()
 
 # -----------------------------------------------------------------------------------*/
 # Retrieving an insurance application session (replace xxx with an existing insurance application session id)
-#-----------------------------------------------------------------------------------*/
+# -----------------------------------------------------------------------------------*/
 
-resource = ten99policy.InsuranceApplicationSessions.retrieve('ias_01G4ZVGEXG4DQHZ1TZ6ANAWPD8')
+resource = ten99policy.InsuranceApplicationSessions.retrieve(
+    "ias_01G4ZVGEXG4DQHZ1TZ6ANAWPD8"
+)
```

### Comparing `ten99policy-1.0.5/examples/invoices.py` & `ten99policy-1.0.6/examples/quotes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,35 @@
 import ten99policy
 
 # You can configure the environment for 1099Policy API (sandbox|production)
 # ten99policy.environment = 'sandbox'
 
 # -----------------------------------------------------------------------------------*/
-# Creating an invoice
-#-----------------------------------------------------------------------------------*/
+# Creating a quote
+# -----------------------------------------------------------------------------------*/
 
-resource = ten99policy.Invoices.create(
-    contractor="cn_ti8eXviE4A",
-    job="jb_rajdrwMUKi",
-    gross_pay=1000,
-    paycycle_startdate="2022-04-25T22:23:13+00:00",
-    paycycle_enddate="2022-04-28T22:23:13+00:00"
+resource = ten99policy.Quotes.create(
+    job_id="jb_jsb9KEcTpc",
+    contractor_id="cn_yJBbMeq9QA",
+    coverage_type=["general", "workers-comp"],
 )
 
-# # -----------------------------------------------------------------------------------*/
-# Updating an invoice (replace xxx with an existing invoice id)
-#-----------------------------------------------------------------------------------*/
+# -----------------------------------------------------------------------------------*/
+# Updating a quote (replace xxx with an existing quote id)
+# -----------------------------------------------------------------------------------*/
 
-resource = ten99policy.Invoices.modify('in_m47rNFQ3PS',
-    gross_pay=1500,
+resource = ten99policy.Quotes.modify(
+    "qt_C9Z2DmfHSF",
+    name="Mechanic",
 )
 
 # -----------------------------------------------------------------------------------*/
-# Fetching the list of invoices
-#-----------------------------------------------------------------------------------*/
-
-resource = ten99policy.Invoices.list()
-
+# Fetching the list of quotes
 # -----------------------------------------------------------------------------------*/
-# Retrieving an invoice (replace xxx with an existing invoice id)
-#-----------------------------------------------------------------------------------*/
 
-resource = ten99policy.Invoices.retrieve('in_tcbma8oShU')
+resource = ten99policy.Quotes.list()
 
 # -----------------------------------------------------------------------------------*/
-# Delete an invoice (replace xxx with an existing invoice id)
-#-----------------------------------------------------------------------------------*/
+# Retrieving a quote (replace xxx with an existing quote id)
+# -----------------------------------------------------------------------------------*/
 
-resource = ten99policy.Invoices.delete('in_tcbma8oShU')
+resource = ten99policy.Quotes.retrieve("qt_C9Z2DmfHSF")
```

### Comparing `ten99policy-1.0.5/examples/policies.py` & `ten99policy-1.0.6/examples/policies.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import ten99policy
 
 # You can configure the environment for 1099Policy API (sandbox|production)
 # ten99policy.environment = 'sandbox'
 
 # -----------------------------------------------------------------------------------*/
 # Creating a policy
-#-----------------------------------------------------------------------------------*/
+# -----------------------------------------------------------------------------------*/
 
 resource = ten99policy.Policies.create(
     quote_id="qt_UPmEfS6nNK",
-    is_active=True
+    is_active=True,
 )
 
 # -----------------------------------------------------------------------------------*/
 # Updating a policy (replace xxx with an existing policy id)
-#-----------------------------------------------------------------------------------*/
+# -----------------------------------------------------------------------------------*/
 
-resource = ten99policy.Policies.modify('en_C9Z2DmfHSF',
+resource = ten99policy.Policies.modify(
+    "en_C9Z2DmfHSF",
     is_active=False,
 )
 
 # -----------------------------------------------------------------------------------*/
 # Fetching the list of policies
-#-----------------------------------------------------------------------------------*/
+# -----------------------------------------------------------------------------------*/
 
 resource = ten99policy.Policies.list()
 
 # -----------------------------------------------------------------------------------*/
 # Retrieving a policy (replace xxx with an existing policy id)
-#-----------------------------------------------------------------------------------*/
+# -----------------------------------------------------------------------------------*/
 
-resource = ten99policy.Policies.retrieve('en_C9Z2DmfHSF')
+resource = ten99policy.Policies.retrieve("en_C9Z2DmfHSF")
 
 # -----------------------------------------------------------------------------------*/
 # Delete a policy (replace xxx with an existing policy id)
-#-----------------------------------------------------------------------------------*/
+# -----------------------------------------------------------------------------------*/
 
-resource = ten99policy.Policies.delete('en_C9Z2DmfHSF')
+resource = ten99policy.Policies.delete("en_C9Z2DmfHSF")
```

### Comparing `ten99policy-1.0.5/examples/quotes.py` & `ten99policy-1.0.6/examples/jobs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,46 @@
 import ten99policy
 
 # You can configure the environment for 1099Policy API (sandbox|production)
 # ten99policy.environment = 'sandbox'
 
 # -----------------------------------------------------------------------------------*/
-# Creating a quote
-#-----------------------------------------------------------------------------------*/
+# Creating a job
+# -----------------------------------------------------------------------------------*/
 
-resource = ten99policy.Quotes.create(
-    job_id="jb_jsb9KEcTpc",
-    contractor_id="cn_yJBbMeq9QA",
-    coverage_type=["general", "workers-comp"],
+resource = ten99policy.Jobs.create(
+    name="Truck driver",
+    description="Requires a truck",
+    duration_hours=20,
+    wage=100,
+    years_experience=20,
+    wage_type="flatfee",
+    entity="en_FwZfQRe4aW",
+    category_code="jc_MTqpkbkp6G",
 )
 
 # -----------------------------------------------------------------------------------*/
-# Updating a quote (replace xxx with an existing quote id)
-#-----------------------------------------------------------------------------------*/
+# Updating a job (replace xxx with an existing job id)
+# -----------------------------------------------------------------------------------*/
 
-resource = ten99policy.Quotes.modify('qt_C9Z2DmfHSF',
-    name='Mechanic',
+resource = ten99policy.Jobs.modify(
+    "jb_C9Z2DmfHSF",
+    name="Mechanic",
 )
 
 # -----------------------------------------------------------------------------------*/
-# Fetching the list of quotes
-#-----------------------------------------------------------------------------------*/
+# Fetching the list of jobs
+# -----------------------------------------------------------------------------------*/
+
+resource = ten99policy.Jobs.list()
+
+# -----------------------------------------------------------------------------------*/
+# Retrieving a job (replace xxx with an existing job id)
+# -----------------------------------------------------------------------------------*/
 
-resource = ten99policy.Quotes.list()
+resource = ten99policy.Jobs.retrieve("jb_C9Z2DmfHSF")
 
 # -----------------------------------------------------------------------------------*/
-# Retrieving a quote (replace xxx with an existing quote id)
-#-----------------------------------------------------------------------------------*/
+# Delete a job (replace xxx with an existing job id)
+# -----------------------------------------------------------------------------------*/
 
-resource = ten99policy.Quotes.retrieve('qt_C9Z2DmfHSF')
+resource = ten99policy.Jobs.delete("jb_C9Z2DmfHSF")
```

### Comparing `ten99policy-1.0.5/requirements.txt` & `ten99policy-1.0.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.5/setup.py` & `ten99policy-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.5/ten99policy/api_requestor.py` & `ten99policy-1.0.6/ten99policy/api_requestor.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.5/ten99policy/api_resources/__init__.py` & `ten99policy-1.0.6/ten99policy/api_resources/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,7 +11,8 @@
 from ten99policy.api_resources.jobs import Jobs
 from ten99policy.api_resources.policies import Policies
 from ten99policy.api_resources.quotes import Quotes
 from ten99policy.api_resources.invoices import Invoices
 from ten99policy.api_resources.insurance_application_sessions import InsuranceApplicationSessions
 from ten99policy.api_resources.events import Events
 from ten99policy.api_resources.assignments import Assignments
+from ten99policy.api_resources.contractor_policies import ContractorPolicies
```

### Comparing `ten99policy-1.0.5/ten99policy/api_resources/abstract/__init__.py` & `ten99policy-1.0.6/ten99policy/api_resources/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.5/ten99policy/api_resources/abstract/api_resource.py` & `ten99policy-1.0.6/ten99policy/api_resources/abstract/api_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
                 " `unicode`)" % (type(self).__name__, id, type(id)),
                 "id",
             )
 
         id = util.utf8(id)
         base = self.class_url()
         extn = quote_plus(id)
+
         return "%s/%s" % (base, extn)
 
     # The `method_` and `url_` arguments are suffixed with an underscore to
     # avoid conflicting with actual request parameters in `params`.
     @classmethod
     def _static_request(
         cls,
```

### Comparing `ten99policy-1.0.5/ten99policy/api_resources/abstract/createable_api_resource.py` & `ten99policy-1.0.6/ten99policy/api_resources/abstract/createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.5/ten99policy/api_resources/abstract/custom_method.py` & `ten99policy-1.0.6/ten99policy/api_resources/abstract/custom_method.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.5/ten99policy/api_resources/abstract/deletable_api_resource.py` & `ten99policy-1.0.6/ten99policy/api_resources/abstract/deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.5/ten99policy/api_resources/abstract/listable_api_resource.py` & `ten99policy-1.0.6/ten99policy/api_resources/abstract/listable_api_resource.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,23 +7,28 @@
 class ListableAPIResource(APIResource):
     @classmethod
     def auto_paging_iter(cls, *args, **params):
         return cls.list(*args, **params).auto_paging_iter()
 
     @classmethod
     def list(
-        cls, api_key=None, ten99policy_version=None, ten99policy_environment=None, **params
+        cls, id=None, api_key=None, ten99policy_version=None, ten99policy_environment=None, **params
     ):
         requestor = api_requestor.APIRequestor(
             api_key,
             api_base=cls.api_base(),
             api_version=ten99policy_version,
             environment=ten99policy_environment,
         )
         url = cls.class_url()
+
+        # supports contractors/{contractor_id}/policies
+        if id and '{}' in url:
+            url = url.format(id)
+
         response, api_key = requestor.request("get", url, params)
         ten99policy_object = util.convert_to_ten99policy_object(
             response, api_key, ten99policy_version, ten99policy_environment
         )
 
         # CFK: take a look at here
         # ten99policy_object._retrieve_params = params
```

### Comparing `ten99policy-1.0.5/ten99policy/api_resources/abstract/nested_resource_class_methods.py` & `ten99policy-1.0.6/ten99policy/api_resources/abstract/nested_resource_class_methods.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.5/ten99policy/api_resources/abstract/singleton_api_resource.py` & `ten99policy-1.0.6/ten99policy/api_resources/abstract/singleton_api_resource.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.5/ten99policy/api_resources/abstract/updateable_api_resource.py` & `ten99policy-1.0.6/ten99policy/api_resources/abstract/updateable_api_resource.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.5/ten99policy/api_resources/error_object.py` & `ten99policy-1.0.6/ten99policy/api_resources/error_object.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.5/ten99policy/api_resources/list_object.py` & `ten99policy-1.0.6/ten99policy/api_resources/list_object.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.5/ten99policy/error.py` & `ten99policy-1.0.6/ten99policy/error.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.5/ten99policy/http_client.py` & `ten99policy-1.0.6/ten99policy/http_client.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.5/ten99policy/multipart_data_generator.py` & `ten99policy-1.0.6/ten99policy/multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.5/ten99policy/object_classes.py` & `ten99policy-1.0.6/ten99policy/object_classes.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.5/ten99policy/six.py` & `ten99policy-1.0.6/ten99policy/six.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.5/ten99policy/ten99policy_object.py` & `ten99policy-1.0.6/ten99policy/ten99policy_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,14 +213,17 @@
             removed = set(self.keys()) - set(values)
             self._transient_values = self._transient_values | removed
             self._unsaved_values = set()
             self.clear()
 
         self._transient_values = self._transient_values - set(values)
 
+        # if not isinstance(values, dict):
+        #     return values
+
         for k, v in six.iteritems(values):
             super(Ten99PolicyObject, self).__setitem__(
                 k,
                 util.convert_to_ten99policy_object(
                     v, api_key, ten99policy_version, ten99policy_environment
                 ),
             )
```

### Comparing `ten99policy-1.0.5/ten99policy/ten99policy_response.py` & `ten99policy-1.0.6/ten99policy/ten99policy_response.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.5/ten99policy/util.py` & `ten99policy-1.0.6/ten99policy/util.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.5/ten99policy.egg-info/PKG-INFO` & `ten99policy-1.0.6/ten99policy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ten99policy
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python bindings for the ten99policy API
 Home-page: https://github.com/1099policy/1099policy-client-python
 Author: Ray Ventura
 Author-email: support@1099policy.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/1099policy/1099policy-client-python/issues
 Project-URL: Documentation, https://1099policy.com/docs/api/?lang=python
```

### Comparing `ten99policy-1.0.5/ten99policy.egg-info/SOURCES.txt` & `ten99policy-1.0.6/ten99policy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 README.md
 VERSION
 requirements.txt
 setup.cfg
 setup.py
 .circleci/config.yml
 examples/assignments.py
+examples/contractor_policies.py
 examples/contractors.py
 examples/entities.py
 examples/events.py
 examples/insurance_application_sessions.py
 examples/invoices.py
 examples/jobs.py
 examples/policies.py
@@ -33,14 +34,15 @@
 ten99policy.egg-info/SOURCES.txt
 ten99policy.egg-info/dependency_links.txt
 ten99policy.egg-info/not-zip-safe
 ten99policy.egg-info/requires.txt
 ten99policy.egg-info/top_level.txt
 ten99policy/api_resources/__init__.py
 ten99policy/api_resources/assignments.py
+ten99policy/api_resources/contractor_policies.py
 ten99policy/api_resources/contractors.py
 ten99policy/api_resources/entities.py
 ten99policy/api_resources/error_object.py
 ten99policy/api_resources/events.py
 ten99policy/api_resources/insurance_application_sessions.py
 ten99policy/api_resources/invoices.py
 ten99policy/api_resources/jobs.py
```

