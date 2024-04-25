# Comparing `tmp/cdk-opinionated-constructs-3.7.0.tar.gz` & `tmp/cdk_opinionated_constructs-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-opinionated-constructs-3.7.0.tar", last modified: Mon Apr  8 20:47:38 2024, max compression
+gzip compressed data, was "cdk_opinionated_constructs-3.7.1.tar", last modified: Thu Apr 25 10:33:28 2024, max compression
```

## Comparing `cdk-opinionated-constructs-3.7.0.tar` & `cdk_opinionated_constructs-3.7.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-08 20:47:38.447295 cdk-opinionated-constructs-3.7.0/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1071 2022-11-05 20:03:58.000000 cdk-opinionated-constructs-3.7.0/LICENSE
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      555 2024-04-08 20:47:38.447029 cdk-opinionated-constructs-3.7.0/PKG-INFO
--rw-r--r--   0 tomaszszuster   (501) staff       (20)    27598 2024-02-26 09:49:43.000000 cdk-opinionated-constructs-3.7.0/README.md
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-08 20:47:38.382575 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     5852 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/alb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2817 2024-01-24 11:50:26.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/ecr.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)    10448 2024-01-24 12:01:51.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/lmb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     6821 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/nlb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     4710 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/rds_instance.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2933 2024-02-26 09:49:43.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/s3.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-08 20:47:38.384522 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/schemas/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/schemas/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3702 2024-03-06 09:09:15.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/schemas/configuration_vars.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1272 2024-02-26 09:49:43.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/sns.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-08 20:47:38.414843 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     8283 2024-03-21 08:42:47.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2261 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/code_quality_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     6602 2024-02-06 00:49:23.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/governance_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2101 2024-03-21 08:42:47.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/infrastructure_tests_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1852 2024-03-21 08:42:47.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/integration_tests_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     7239 2024-04-08 20:45:23.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/notifications_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1872 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/pipeline_plugins_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3644 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/pipeline_trigger_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2077 2024-03-21 08:42:47.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/services_tests_stack.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-08 20:47:38.417587 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1103 2024-03-04 14:20:14.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/code_quality_stage.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      958 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/infrastructure_tests_stage.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      934 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/integration_tests_stage.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1045 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/notifications_stage.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1494 2024-02-05 18:17:09.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/plugins_stage.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      915 2024-03-04 14:20:14.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/services_tests_stage.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-08 20:47:38.418087 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/utils/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2880 2024-02-05 22:11:31.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/utils/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)    15910 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/wafv2.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-08 20:47:38.446365 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs.egg-info/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      555 2024-04-08 20:47:38.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs.egg-info/PKG-INFO
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2380 2024-04-08 20:47:38.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        1 2024-04-08 20:47:38.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      125 2024-04-08 20:47:38.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs.egg-info/requires.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       32 2024-04-08 20:47:38.000000 cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs.egg-info/top_level.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3649 2024-04-08 20:47:38.448045 cdk-opinionated-constructs-3.7.0/setup.cfg
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      806 2024-04-08 20:47:06.000000 cdk-opinionated-constructs-3.7.0/setup.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-08 20:47:38.419117 cdk-opinionated-constructs-3.7.0/test/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-3.7.0/test/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1758 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/app.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-08 20:47:38.421429 cdk-opinionated-constructs-3.7.0/test/infrastucture/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/infrastucture/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2036 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/infrastucture/test_alb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1173 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/infrastucture/test_ecr_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1851 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/infrastucture/test_lmb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1516 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/infrastucture/test_s3_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1148 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/infrastucture/test_sns_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3739 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/infrastucture/test_wafv2_stack.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-08 20:47:38.444028 cdk-opinionated-constructs-3.7.0/test/stacks/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-3.7.0/test/stacks/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3435 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/stacks/alb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1384 2024-01-24 11:27:38.000000 cdk-opinionated-constructs-3.7.0/test/stacks/ecr_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     4412 2024-01-24 11:50:26.000000 cdk-opinionated-constructs-3.7.0/test/stacks/lmb_docker_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3591 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/stacks/lmb_monitoring_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2719 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/stacks/lmb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2152 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/stacks/nlb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3293 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/stacks/rds_mysql_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3308 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/stacks/rds_postgresql_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1619 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/stacks/s3_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1067 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/stacks/sns_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2567 2024-01-17 10:21:03.000000 cdk-opinionated-constructs-3.7.0/test/stacks/wafv2_stack.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-25 10:33:28.580649 cdk_opinionated_constructs-3.7.1/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1071 2022-11-05 20:03:58.000000 cdk_opinionated_constructs-3.7.1/LICENSE
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      555 2024-04-25 10:33:28.580584 cdk_opinionated_constructs-3.7.1/PKG-INFO
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)    27598 2024-02-26 09:49:43.000000 cdk_opinionated_constructs-3.7.1/README.md
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-25 10:33:28.564378 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     5852 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/alb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2817 2024-01-24 11:50:26.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/ecr.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)    10448 2024-01-24 12:01:51.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/lmb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     6821 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/nlb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     4710 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/rds_instance.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2933 2024-02-26 09:49:43.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/s3.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-25 10:33:28.564670 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/schemas/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/schemas/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3702 2024-03-06 09:09:15.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/schemas/configuration_vars.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1272 2024-02-26 09:49:43.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/sns.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-25 10:33:28.566076 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stacks/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     8721 2024-04-25 10:31:45.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stacks/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2261 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stacks/code_quality_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     6602 2024-02-06 00:49:23.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stacks/governance_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2101 2024-03-21 08:42:47.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stacks/infrastructure_tests_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1852 2024-03-21 08:42:47.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stacks/integration_tests_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     7239 2024-04-08 20:49:10.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stacks/notifications_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1872 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stacks/pipeline_plugins_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3644 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stacks/pipeline_trigger_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2077 2024-03-21 08:42:47.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stacks/services_tests_stack.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-25 10:33:28.566805 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stages/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stages/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1103 2024-03-04 14:20:14.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stages/code_quality_stage.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      958 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stages/infrastructure_tests_stage.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      934 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stages/integration_tests_stage.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1045 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stages/notifications_stage.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1494 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stages/plugins_stage.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      915 2024-03-04 14:20:14.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stages/services_tests_stage.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-25 10:33:28.566916 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/utils/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2880 2024-02-05 22:11:31.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/utils/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)    15910 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/wafv2.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-25 10:33:28.580335 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs.egg-info/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      555 2024-04-25 10:33:28.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2380 2024-04-25 10:33:28.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        1 2024-04-25 10:33:28.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      125 2024-04-25 10:33:28.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs.egg-info/requires.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       32 2024-04-25 10:33:28.000000 cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs.egg-info/top_level.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3649 2024-04-25 10:33:28.581137 cdk_opinionated_constructs-3.7.1/setup.cfg
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      806 2024-04-25 10:29:14.000000 cdk_opinionated_constructs-3.7.1/setup.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-25 10:33:28.567108 cdk_opinionated_constructs-3.7.1/test/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk_opinionated_constructs-3.7.1/test/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1758 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.1/test/app.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-25 10:33:28.567845 cdk_opinionated_constructs-3.7.1/test/infrastucture/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.1/test/infrastucture/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2036 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.1/test/infrastucture/test_alb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1173 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.1/test/infrastucture/test_ecr_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1851 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.1/test/infrastucture/test_lmb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1516 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.1/test/infrastucture/test_s3_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1148 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.1/test/infrastucture/test_sns_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3739 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.1/test/infrastucture/test_wafv2_stack.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-25 10:33:28.569136 cdk_opinionated_constructs-3.7.1/test/stacks/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk_opinionated_constructs-3.7.1/test/stacks/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3435 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.1/test/stacks/alb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1384 2024-01-24 11:27:38.000000 cdk_opinionated_constructs-3.7.1/test/stacks/ecr_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     4412 2024-01-24 11:50:26.000000 cdk_opinionated_constructs-3.7.1/test/stacks/lmb_docker_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3591 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.1/test/stacks/lmb_monitoring_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2719 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.1/test/stacks/lmb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2152 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.1/test/stacks/nlb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3293 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.1/test/stacks/rds_mysql_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3308 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.1/test/stacks/rds_postgresql_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1619 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.1/test/stacks/s3_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1067 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.1/test/stacks/sns_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2567 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.1/test/stacks/wafv2_stack.py
```

### Comparing `cdk-opinionated-constructs-3.7.0/LICENSE` & `cdk_opinionated_constructs-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/PKG-INFO` & `cdk_opinionated_constructs-3.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-opinionated-constructs
-Version: 3.7.0
+Version: 3.7.1
 Summary: AWS CDK constructs come without added security configurations.
 License: MIT
 Requires-Python: >=3.11
 License-File: LICENSE
 Requires-Dist: aws-cdk-lib>=2.98.0
 Requires-Dist: constructs>=10.2.69
 Requires-Dist: cdk-monitoring-constructs>=6.0.0
```

### Comparing `cdk-opinionated-constructs-3.7.0/README.md` & `cdk_opinionated_constructs-3.7.1/README.md`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/alb.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/alb.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/ecr.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/ecr.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/lmb.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/lmb.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/nlb.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/nlb.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/rds_instance.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/rds_instance.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/s3.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/s3.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/schemas/configuration_vars.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/schemas/configuration_vars.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/sns.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/sns.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/__init__.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stacks/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -200,42 +200,45 @@
         rule_name=f"{pipeline_vars.project}-scheduled-release",
         schedule=schedule,
     )
     trigger.add_target(events_targets.CodePipeline(self.codepipeline.pipeline))  # type: ignore
     apply_tags(props=props, resource=trigger)  # type: ignore
 
 
-def create_pipeline_notifications(self, notifications_sns_topic: sns.Topic | sns.ITopic, pipeline_vars: PipelineVars):
-    """Creates notifications for the pipeline.
-
+def create_pipeline_notifications(
+    self,
+    notifications_sns_topic: sns.Topic | sns.ITopic,
+    pipeline_vars: PipelineVars,
+    use_chatbot: bool = True,  # noqa: FBT001, FBT002
+):
+    """
     Parameters:
-
-    notifications_sns_topic (sns.Topic | sns.ITopic): The SNS topic to publish notifications to.
-
-    pipeline_vars (PipelineVars): A Pydantic model containing pipeline configuration values like
-    notification email, Slack workspace ID, etc.
+        notifications_sns_topic (sns.Topic | sns.ITopic): The SNS topic for pipeline notifications.
+        pipeline_vars (PipelineVars): A model containing pipeline configuration values.
+        use_chatbot (bool, optional): Flag to enable or disable Slack notifications using Chatbot. Defaults to True.
 
     Functionality:
-
-    1. if a notification email address is provided in pipeline_vars, enable email notifications by calling
-    pipeline_email_notifications()
-
-    2. enable default pipeline notifications by calling pipeline_notifications()
-
-    3. if Slack workspace ID and channel ID are provided in pipeline_vars, enable Slack notifications by
-    creating a SlackChannelConfiguration construct
+        1. Enables SNS notifications if the recipient email address is provided in `pipeline_vars`.
+        2. Enables pipeline notifications if the Slack CI/CD channel ID is provided in `pipeline_vars`.
+        3. Enables Slack notifications using AWS Chatbot if the Slack workspace ID, CI/CD channel ID,
+        and `use_chatbot` flag are provided.
+
+        The function configures notifications based on the provided configuration values in `pipeline_vars`.
+        It uses the `notifications_sns_topic` to send notifications via email or Slack.
+        If `use_chatbot` is set to True and the required Slack configuration values are provided,
+        it creates a Slack channel configuration using AWS Chatbot.
     """
-
     # Enable SNS notifications if the recipient email address was provided
     if pipeline_vars.ci_cd_notification_email:
         pipeline_email_notifications(sns_topic=notifications_sns_topic)
     if pipeline_vars.slack_ci_cd_channel_id:
         pipeline_notifications(self, sns_topic=notifications_sns_topic)
+
     # Enable Slack notifications if recipient workspace and channel slack were provided.
-    if pipeline_vars.slack_workspace_id and pipeline_vars.slack_ci_cd_channel_id:
+    if pipeline_vars.slack_workspace_id and pipeline_vars.slack_ci_cd_channel_id and use_chatbot:
         chatbot.SlackChannelConfiguration(
             self,
             "chatbot",
             slack_channel_configuration_name=pipeline_vars.project,
             notification_topics=[notifications_sns_topic],
             slack_workspace_id=pipeline_vars.slack_workspace_id,
             slack_channel_id=pipeline_vars.slack_ci_cd_channel_id,
```

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/code_quality_stack.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stacks/code_quality_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/governance_stack.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stacks/governance_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/infrastructure_tests_stack.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stacks/infrastructure_tests_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/integration_tests_stack.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stacks/integration_tests_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/notifications_stack.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stacks/notifications_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/pipeline_plugins_stack.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stacks/pipeline_plugins_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/pipeline_trigger_stack.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stacks/pipeline_trigger_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stacks/services_tests_stack.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stacks/services_tests_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/code_quality_stage.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stages/code_quality_stage.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/infrastructure_tests_stage.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stages/infrastructure_tests_stage.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/integration_tests_stage.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stages/integration_tests_stage.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/notifications_stage.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stages/notifications_stage.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/plugins_stage.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stages/plugins_stage.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/stages/services_tests_stage.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/stages/services_tests_stage.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/utils/__init__.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs/wafv2.py` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs/wafv2.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs.egg-info/PKG-INFO` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-opinionated-constructs
-Version: 3.7.0
+Version: 3.7.1
 Summary: AWS CDK constructs come without added security configurations.
 License: MIT
 Requires-Python: >=3.11
 License-File: LICENSE
 Requires-Dist: aws-cdk-lib>=2.98.0
 Requires-Dist: constructs>=10.2.69
 Requires-Dist: cdk-monitoring-constructs>=6.0.0
```

### Comparing `cdk-opinionated-constructs-3.7.0/cdk_opinionated_constructs.egg-info/SOURCES.txt` & `cdk_opinionated_constructs-3.7.1/cdk_opinionated_constructs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/setup.cfg` & `cdk_opinionated_constructs-3.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/setup.py` & `cdk_opinionated_constructs-3.7.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 https://packaging.python.org/en/latest/distributing.html
 """
 
 from setuptools import find_packages, setup
 
 setup(
     name="cdk-opinionated-constructs",
-    version="3.7.0",
+    version="3.7.1",
     description="AWS CDK constructs come without added security configurations.",
     long_description="The idea behind this project is to create secured constructs from the start. \n"
     "Supported constructs: ALB, ECR, LMB, NLB, S3, SNS, WAF, RDS",
     license="MIT",
     package_dir={"": "."},
     packages=find_packages(where="."),
     install_requires=[
```

### Comparing `cdk-opinionated-constructs-3.7.0/test/app.py` & `cdk_opinionated_constructs-3.7.1/test/app.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/test/infrastucture/test_alb_stack.py` & `cdk_opinionated_constructs-3.7.1/test/infrastucture/test_alb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/test/infrastucture/test_ecr_stack.py` & `cdk_opinionated_constructs-3.7.1/test/infrastucture/test_ecr_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/test/infrastucture/test_lmb_stack.py` & `cdk_opinionated_constructs-3.7.1/test/infrastucture/test_lmb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/test/infrastucture/test_s3_stack.py` & `cdk_opinionated_constructs-3.7.1/test/infrastucture/test_s3_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/test/infrastucture/test_sns_stack.py` & `cdk_opinionated_constructs-3.7.1/test/infrastucture/test_sns_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/test/infrastucture/test_wafv2_stack.py` & `cdk_opinionated_constructs-3.7.1/test/infrastucture/test_wafv2_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/test/stacks/alb_stack.py` & `cdk_opinionated_constructs-3.7.1/test/stacks/alb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/test/stacks/ecr_stack.py` & `cdk_opinionated_constructs-3.7.1/test/stacks/ecr_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/test/stacks/lmb_docker_stack.py` & `cdk_opinionated_constructs-3.7.1/test/stacks/lmb_docker_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/test/stacks/lmb_monitoring_stack.py` & `cdk_opinionated_constructs-3.7.1/test/stacks/lmb_monitoring_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/test/stacks/lmb_stack.py` & `cdk_opinionated_constructs-3.7.1/test/stacks/lmb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/test/stacks/nlb_stack.py` & `cdk_opinionated_constructs-3.7.1/test/stacks/nlb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/test/stacks/rds_mysql_stack.py` & `cdk_opinionated_constructs-3.7.1/test/stacks/rds_mysql_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/test/stacks/rds_postgresql_stack.py` & `cdk_opinionated_constructs-3.7.1/test/stacks/rds_postgresql_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/test/stacks/s3_stack.py` & `cdk_opinionated_constructs-3.7.1/test/stacks/s3_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/test/stacks/sns_stack.py` & `cdk_opinionated_constructs-3.7.1/test/stacks/sns_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-3.7.0/test/stacks/wafv2_stack.py` & `cdk_opinionated_constructs-3.7.1/test/stacks/wafv2_stack.py`

 * *Files identical despite different names*

