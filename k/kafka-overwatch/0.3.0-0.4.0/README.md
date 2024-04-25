# Comparing `tmp/kafka_overwatch-0.3.0.tar.gz` & `tmp/kafka_overwatch-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka_overwatch-0.3.0.tar", max compression
+gzip compressed data, was "kafka_overwatch-0.4.0.tar", max compression
```

## Comparing `kafka_overwatch-0.3.0.tar` & `kafka_overwatch-0.4.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
--rw-r--r--   0        0        0    16725 2023-12-13 12:48:29.115693 kafka_overwatch-0.3.0/LICENSE
--rw-r--r--   0        0        0     3130 2024-02-14 21:24:07.217496 kafka_overwatch-0.3.0/README.rst
--rw-r--r--   0        0        0      176 2024-04-18 23:11:15.932008 kafka_overwatch-0.3.0/kafka_overwatch/__init__.py
--rw-r--r--   0        0        0     1300 2024-02-15 16:51:43.978241 kafka_overwatch-0.3.0/kafka_overwatch/aws_helpers/__init__.py
--rw-r--r--   0        0        0     2372 2024-03-12 06:50:39.512258 kafka_overwatch-0.3.0/kafka_overwatch/aws_helpers/kafka_client_secrets.py
--rw-r--r--   0        0        0     2862 2024-04-07 20:43:52.705782 kafka_overwatch-0.3.0/kafka_overwatch/aws_helpers/s3.py
--rw-r--r--   0        0        0     2626 2024-02-07 21:36:59.982077 kafka_overwatch-0.3.0/kafka_overwatch/cli/__init__.py
--rw-r--r--   0        0        0     1342 2024-04-17 05:19:40.739040 kafka_overwatch-0.3.0/kafka_overwatch/cli/schema_registry_restore.py
--rw-r--r--   0        0        0     1175 2024-04-07 20:43:52.705782 kafka_overwatch-0.3.0/kafka_overwatch/common/__init__.py
--rw-r--r--   0        0        0      970 2024-01-04 01:27:32.802689 kafka_overwatch-0.3.0/kafka_overwatch/config/__init__.py
--rw-r--r--   0        0        0     3228 2024-04-07 20:43:52.705782 kafka_overwatch-0.3.0/kafka_overwatch/config/config.py
--rw-r--r--   0        0        0     3229 2024-01-01 08:48:18.162847 kafka_overwatch-0.3.0/kafka_overwatch/config/logging.py
--rw-r--r--   0        0        0      250 2024-04-06 19:12:23.350109 kafka_overwatch-0.3.0/kafka_overwatch/config/threads_settings.py
--rw-r--r--   0        0        0     1542 2024-04-07 20:43:52.706782 kafka_overwatch-0.3.0/kafka_overwatch/kafka_resources/__init__.py
--rw-r--r--   0        0        0     7948 2024-04-07 20:43:52.706782 kafka_overwatch-0.3.0/kafka_overwatch/kafka_resources/groups.py
--rw-r--r--   0        0        0     8939 2024-04-07 20:43:52.706782 kafka_overwatch-0.3.0/kafka_overwatch/kafka_resources/topics.py
--rw-r--r--   0        0        0       88 2024-01-02 07:32:22.087588 kafka_overwatch-0.3.0/kafka_overwatch/monitoring/__init__.py
--rw-r--r--   0        0        0     2513 2024-04-07 20:43:52.706782 kafka_overwatch-0.3.0/kafka_overwatch/monitoring/prometheus.py
--rw-r--r--   0        0        0      176 2024-03-11 21:31:12.971386 kafka_overwatch-0.3.0/kafka_overwatch/notifications/__init__.py
--rw-r--r--   0        0        0     5230 2024-04-07 20:43:52.706782 kafka_overwatch-0.3.0/kafka_overwatch/notifications/aws_sns/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 21:31:12.972386 kafka_overwatch-0.3.0/kafka_overwatch/notifications/aws_sns/usage_report/__init__.py
--rw-r--r--   0        0        0       83 2024-03-11 21:31:12.972386 kafka_overwatch-0.3.0/kafka_overwatch/notifications/aws_sns/usage_report/default.j2
--rw-r--r--   0        0        0      484 2024-03-11 21:31:12.972386 kafka_overwatch-0.3.0/kafka_overwatch/notifications/aws_sns/usage_report/email.j2
--rw-r--r--   0        0        0     3496 2024-04-07 20:43:52.706782 kafka_overwatch-0.3.0/kafka_overwatch/overwatch.py
--rw-r--r--   0        0        0       86 2024-01-02 07:32:22.104588 kafka_overwatch-0.3.0/kafka_overwatch/overwatch_resources/__init__.py
--rw-r--r--   0        0        0    14000 2024-04-07 20:43:52.706782 kafka_overwatch-0.3.0/kafka_overwatch/overwatch_resources/clusters.py
--rw-r--r--   0        0        0     5026 2024-03-11 06:55:53.345126 kafka_overwatch-0.3.0/kafka_overwatch/overwatch_resources/groups.py
--rw-r--r--   0        0        0     5171 2024-04-17 05:16:00.917189 kafka_overwatch-0.3.0/kafka_overwatch/overwatch_resources/schema_registry/__init__.py
--rw-r--r--   0        0        0     2412 2024-04-07 20:43:52.707782 kafka_overwatch-0.3.0/kafka_overwatch/overwatch_resources/schema_registry/schema.py
--rw-r--r--   0        0        0     3135 2024-04-18 23:09:58.482167 kafka_overwatch-0.3.0/kafka_overwatch/overwatch_resources/schema_registry/schemas_restore.py
--rw-r--r--   0        0        0      801 2024-04-07 20:43:52.707782 kafka_overwatch-0.3.0/kafka_overwatch/overwatch_resources/schema_registry/subject.py
--rw-r--r--   0        0        0     7286 2024-04-07 20:43:52.707782 kafka_overwatch-0.3.0/kafka_overwatch/overwatch_resources/topics.py
--rw-r--r--   0        0        0     1089 2024-04-07 20:43:52.707782 kafka_overwatch-0.3.0/kafka_overwatch/processing/__init__.py
--rw-r--r--   0        0        0     5893 2024-04-07 20:43:52.707782 kafka_overwatch-0.3.0/kafka_overwatch/processing/clusters.py
--rw-r--r--   0        0        0     9011 2024-04-07 20:43:52.707782 kafka_overwatch-0.3.0/kafka_overwatch/processing/schema_registries.py
--rw-r--r--   0        0        0     4793 2024-04-07 20:43:52.707782 kafka_overwatch-0.3.0/kafka_overwatch/reporting/__init__.py
--rw-r--r--   0        0        0       88 2024-02-14 21:24:07.217496 kafka_overwatch-0.3.0/kafka_overwatch/reporting/governance/__init__.py
--rw-r--r--   0        0        0     1364 2024-03-11 06:55:53.346126 kafka_overwatch-0.3.0/kafka_overwatch/reporting/governance/consumer_groups_naming_convention.py
--rw-r--r--   0        0        0     1355 2024-02-14 21:24:07.217496 kafka_overwatch-0.3.0/kafka_overwatch/reporting/governance/topic_naming_convention.py
--rw-r--r--   0        0        0     1128 2024-04-07 20:43:52.707782 kafka_overwatch-0.3.0/kafka_overwatch/reporting/schema_registry.py
--rw-r--r--   0        0        0     1963 2024-03-11 06:55:53.346126 kafka_overwatch-0.3.0/kafka_overwatch/reporting/tools.py
--rw-r--r--   0        0        0     3967 2024-04-07 20:43:52.707782 kafka_overwatch-0.3.0/kafka_overwatch/reporting/topics.py
--rw-r--r--   0        0        0       86 2024-01-02 07:32:22.103588 kafka_overwatch-0.3.0/kafka_overwatch/specs/__init__.py
--rw-r--r--   0        0        0    21799 2024-04-18 23:11:16.225004 kafka_overwatch-0.3.0/kafka_overwatch/specs/config.json
--rw-r--r--   0        0        0    11668 2024-04-07 20:43:52.708782 kafka_overwatch-0.3.0/kafka_overwatch/specs/config.py
--rw-r--r--   0        0        0     6716 2024-04-18 23:11:16.225004 kafka_overwatch-0.3.0/kafka_overwatch/specs/report.json
--rw-r--r--   0        0        0     3249 2024-04-07 20:43:52.708782 kafka_overwatch-0.3.0/kafka_overwatch/specs/report.py
--rw-r--r--   0        0        0     2889 2024-04-18 23:11:15.932008 kafka_overwatch-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 kafka_overwatch-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      281 2024-02-14 21:24:07.216496 kafka_overwatch-0.4.0/AUTHORS.rst
+-rw-r--r--   0        0        0    16725 2023-12-13 12:48:29.115693 kafka_overwatch-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3130 2024-02-14 21:24:07.217496 kafka_overwatch-0.4.0/README.rst
+-rw-r--r--   0        0        0      176 2024-04-25 16:37:05.337066 kafka_overwatch-0.4.0/kafka_overwatch/__init__.py
+-rw-r--r--   0        0        0     1300 2024-02-15 16:51:43.978241 kafka_overwatch-0.4.0/kafka_overwatch/aws_helpers/__init__.py
+-rw-r--r--   0        0        0     2372 2024-03-12 06:50:39.512258 kafka_overwatch-0.4.0/kafka_overwatch/aws_helpers/kafka_client_secrets.py
+-rw-r--r--   0        0        0     2862 2024-04-07 20:43:52.705782 kafka_overwatch-0.4.0/kafka_overwatch/aws_helpers/s3.py
+-rw-r--r--   0        0        0     2626 2024-02-07 21:36:59.982077 kafka_overwatch-0.4.0/kafka_overwatch/cli/__init__.py
+-rw-r--r--   0        0        0     1342 2024-04-17 05:19:40.739040 kafka_overwatch-0.4.0/kafka_overwatch/cli/schema_registry_restore.py
+-rw-r--r--   0        0        0     1175 2024-04-07 20:43:52.705782 kafka_overwatch-0.4.0/kafka_overwatch/common/__init__.py
+-rw-r--r--   0        0        0      970 2024-01-04 01:27:32.802689 kafka_overwatch-0.4.0/kafka_overwatch/config/__init__.py
+-rw-r--r--   0        0        0     3228 2024-04-07 20:43:52.705782 kafka_overwatch-0.4.0/kafka_overwatch/config/config.py
+-rw-r--r--   0        0        0     3229 2024-01-01 08:48:18.162847 kafka_overwatch-0.4.0/kafka_overwatch/config/logging.py
+-rw-r--r--   0        0        0      250 2024-04-06 19:12:23.350109 kafka_overwatch-0.4.0/kafka_overwatch/config/threads_settings.py
+-rw-r--r--   0        0        0     1542 2024-04-07 20:43:52.706782 kafka_overwatch-0.4.0/kafka_overwatch/kafka_resources/__init__.py
+-rw-r--r--   0        0        0     7948 2024-04-07 20:43:52.706782 kafka_overwatch-0.4.0/kafka_overwatch/kafka_resources/groups.py
+-rw-r--r--   0        0        0     8939 2024-04-07 20:43:52.706782 kafka_overwatch-0.4.0/kafka_overwatch/kafka_resources/topics.py
+-rw-r--r--   0        0        0       88 2024-01-02 07:32:22.087588 kafka_overwatch-0.4.0/kafka_overwatch/monitoring/__init__.py
+-rw-r--r--   0        0        0     2513 2024-04-07 20:43:52.706782 kafka_overwatch-0.4.0/kafka_overwatch/monitoring/prometheus.py
+-rw-r--r--   0        0        0      176 2024-03-11 21:31:12.971386 kafka_overwatch-0.4.0/kafka_overwatch/notifications/__init__.py
+-rw-r--r--   0        0        0     5230 2024-04-07 20:43:52.706782 kafka_overwatch-0.4.0/kafka_overwatch/notifications/aws_sns/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-11 21:31:12.972386 kafka_overwatch-0.4.0/kafka_overwatch/notifications/aws_sns/usage_report/__init__.py
+-rw-r--r--   0        0        0       83 2024-03-11 21:31:12.972386 kafka_overwatch-0.4.0/kafka_overwatch/notifications/aws_sns/usage_report/default.j2
+-rw-r--r--   0        0        0      484 2024-03-11 21:31:12.972386 kafka_overwatch-0.4.0/kafka_overwatch/notifications/aws_sns/usage_report/email.j2
+-rw-r--r--   0        0        0     3496 2024-04-07 20:43:52.706782 kafka_overwatch-0.4.0/kafka_overwatch/overwatch.py
+-rw-r--r--   0        0        0       86 2024-01-02 07:32:22.104588 kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/__init__.py
+-rw-r--r--   0        0        0    14000 2024-04-07 20:43:52.706782 kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/clusters.py
+-rw-r--r--   0        0        0     5026 2024-03-11 06:55:53.345126 kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/groups.py
+-rw-r--r--   0        0        0     5171 2024-04-17 05:16:00.917189 kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/schema_registry/__init__.py
+-rw-r--r--   0        0        0     2412 2024-04-07 20:43:52.707782 kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/schema_registry/schema.py
+-rw-r--r--   0        0        0     3135 2024-04-18 23:09:58.482167 kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/schema_registry/schemas_restore.py
+-rw-r--r--   0        0        0      801 2024-04-07 20:43:52.707782 kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/schema_registry/subject.py
+-rw-r--r--   0        0        0     7286 2024-04-07 20:43:52.707782 kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/topics.py
+-rw-r--r--   0        0        0     1089 2024-04-07 20:43:52.707782 kafka_overwatch-0.4.0/kafka_overwatch/processing/__init__.py
+-rw-r--r--   0        0        0     5893 2024-04-07 20:43:52.707782 kafka_overwatch-0.4.0/kafka_overwatch/processing/clusters.py
+-rw-r--r--   0        0        0     9011 2024-04-07 20:43:52.707782 kafka_overwatch-0.4.0/kafka_overwatch/processing/schema_registries.py
+-rw-r--r--   0        0        0     4793 2024-04-07 20:43:52.707782 kafka_overwatch-0.4.0/kafka_overwatch/reporting/__init__.py
+-rw-r--r--   0        0        0       88 2024-02-14 21:24:07.217496 kafka_overwatch-0.4.0/kafka_overwatch/reporting/governance/__init__.py
+-rw-r--r--   0        0        0     1364 2024-03-11 06:55:53.346126 kafka_overwatch-0.4.0/kafka_overwatch/reporting/governance/consumer_groups_naming_convention.py
+-rw-r--r--   0        0        0     1355 2024-02-14 21:24:07.217496 kafka_overwatch-0.4.0/kafka_overwatch/reporting/governance/topic_naming_convention.py
+-rw-r--r--   0        0        0     1128 2024-04-07 20:43:52.707782 kafka_overwatch-0.4.0/kafka_overwatch/reporting/schema_registry.py
+-rw-r--r--   0        0        0     1963 2024-03-11 06:55:53.346126 kafka_overwatch-0.4.0/kafka_overwatch/reporting/tools.py
+-rw-r--r--   0        0        0     3967 2024-04-07 20:43:52.707782 kafka_overwatch-0.4.0/kafka_overwatch/reporting/topics.py
+-rw-r--r--   0        0        0       86 2024-01-02 07:32:22.103588 kafka_overwatch-0.4.0/kafka_overwatch/specs/__init__.py
+-rw-r--r--   0        0        0    21799 2024-04-25 16:37:05.671059 kafka_overwatch-0.4.0/kafka_overwatch/specs/config.json
+-rw-r--r--   0        0        0    11668 2024-04-07 20:43:52.708782 kafka_overwatch-0.4.0/kafka_overwatch/specs/config.py
+-rw-r--r--   0        0        0     6716 2024-04-25 16:37:05.671059 kafka_overwatch-0.4.0/kafka_overwatch/specs/report.json
+-rw-r--r--   0        0        0     3249 2024-04-07 20:43:52.708782 kafka_overwatch-0.4.0/kafka_overwatch/specs/report.py
+-rw-r--r--   0        0        0     2889 2024-04-25 16:37:05.337066 kafka_overwatch-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4989 1970-01-01 00:00:00.000000 kafka_overwatch-0.4.0/PKG-INFO
```

### Comparing `kafka_overwatch-0.3.0/LICENSE` & `kafka_overwatch-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/README.rst` & `kafka_overwatch-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/aws_helpers/__init__.py` & `kafka_overwatch-0.4.0/kafka_overwatch/aws_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/aws_helpers/kafka_client_secrets.py` & `kafka_overwatch-0.4.0/kafka_overwatch/aws_helpers/kafka_client_secrets.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/aws_helpers/s3.py` & `kafka_overwatch-0.4.0/kafka_overwatch/aws_helpers/s3.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/cli/__init__.py` & `kafka_overwatch-0.4.0/kafka_overwatch/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/cli/schema_registry_restore.py` & `kafka_overwatch-0.4.0/kafka_overwatch/cli/schema_registry_restore.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/common/__init__.py` & `kafka_overwatch-0.4.0/kafka_overwatch/common/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/config/__init__.py` & `kafka_overwatch-0.4.0/kafka_overwatch/config/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/config/config.py` & `kafka_overwatch-0.4.0/kafka_overwatch/config/config.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/config/logging.py` & `kafka_overwatch-0.4.0/kafka_overwatch/config/logging.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/kafka_resources/__init__.py` & `kafka_overwatch-0.4.0/kafka_overwatch/kafka_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/kafka_resources/groups.py` & `kafka_overwatch-0.4.0/kafka_overwatch/kafka_resources/groups.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/kafka_resources/topics.py` & `kafka_overwatch-0.4.0/kafka_overwatch/kafka_resources/topics.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/monitoring/prometheus.py` & `kafka_overwatch-0.4.0/kafka_overwatch/monitoring/prometheus.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/notifications/aws_sns/__init__.py` & `kafka_overwatch-0.4.0/kafka_overwatch/notifications/aws_sns/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/overwatch.py` & `kafka_overwatch-0.4.0/kafka_overwatch/overwatch.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/overwatch_resources/clusters.py` & `kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/clusters.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/overwatch_resources/groups.py` & `kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/groups.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/overwatch_resources/schema_registry/__init__.py` & `kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/schema_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/overwatch_resources/schema_registry/schema.py` & `kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/schema_registry/schema.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/overwatch_resources/schema_registry/schemas_restore.py` & `kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/schema_registry/schemas_restore.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/overwatch_resources/schema_registry/subject.py` & `kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/schema_registry/subject.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/overwatch_resources/topics.py` & `kafka_overwatch-0.4.0/kafka_overwatch/overwatch_resources/topics.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/processing/__init__.py` & `kafka_overwatch-0.4.0/kafka_overwatch/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/processing/clusters.py` & `kafka_overwatch-0.4.0/kafka_overwatch/processing/clusters.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/processing/schema_registries.py` & `kafka_overwatch-0.4.0/kafka_overwatch/processing/schema_registries.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/reporting/__init__.py` & `kafka_overwatch-0.4.0/kafka_overwatch/reporting/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/reporting/governance/consumer_groups_naming_convention.py` & `kafka_overwatch-0.4.0/kafka_overwatch/reporting/governance/consumer_groups_naming_convention.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/reporting/governance/topic_naming_convention.py` & `kafka_overwatch-0.4.0/kafka_overwatch/reporting/governance/topic_naming_convention.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/reporting/schema_registry.py` & `kafka_overwatch-0.4.0/kafka_overwatch/reporting/schema_registry.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/reporting/tools.py` & `kafka_overwatch-0.4.0/kafka_overwatch/reporting/tools.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/reporting/topics.py` & `kafka_overwatch-0.4.0/kafka_overwatch/reporting/topics.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/specs/config.json` & `kafka_overwatch-0.4.0/kafka_overwatch/specs/config.json`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/specs/config.py` & `kafka_overwatch-0.4.0/kafka_overwatch/specs/config.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/specs/report.json` & `kafka_overwatch-0.4.0/kafka_overwatch/specs/report.json`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/kafka_overwatch/specs/report.py` & `kafka_overwatch-0.4.0/kafka_overwatch/specs/report.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.3.0/pyproject.toml` & `kafka_overwatch-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kafka-overwatch"
-version = "0.3.0"
+version = "0.4.0"
 description = "Continuously monitors Kafka cluster topics & consumer groups"
 authors = ["John \"Preston\" Mille <john@ews-network.net>"]
 maintainers = ["John \"Preston\" Mille <john@ews-network.net>"]
 readme = "README.rst"
 license = "MPL-2.0"
 keywords = ["kafka", "monitoring", "reporting", "usage-analysis", "cost-savings"]
 
@@ -88,15 +88,15 @@
   "*/cli.py"
 ]
 
 [tool.tbump]
 github_url = "https://github.com/johnpreston/kafka-overwatch"
 
 [tool.tbump.version]
-current = "0.3.0"
+current = "0.4.0"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?:(?P<rc>[\S]+))?
```

### Comparing `kafka_overwatch-0.3.0/PKG-INFO` & `kafka_overwatch-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-overwatch
-Version: 0.3.0
+Version: 0.4.0
 Summary: Continuously monitors Kafka cluster topics & consumer groups
 License: MPL-2.0
 Keywords: kafka,monitoring,reporting,usage-analysis,cost-savings
 Author: John "Preston" Mille
 Author-email: john@ews-network.net
 Maintainer: John "Preston" Mille
 Maintainer-email: john@ews-network.net
@@ -15,14 +15,15 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aws-cfn-custom-resource-resolve-parser (>=0.3,<0.4)
 Requires-Dist: aws-embedded-metrics (>=3.2.0,<4.0.0)
 Requires-Dist: aws-msk-iam-sasl-signer-python (>=1.0.0,<2.0.0)
 Requires-Dist: boto3 (>=1.26,<2.0)
 Requires-Dist: codeguru-profiler-agent (>=1.2.4,<2.0.0)
 Requires-Dist: compose-x-common (>=1.4.4,<2.0.0)
 Requires-Dist: confluent-kafka (>=2.3.0,<3.0.0)
```

