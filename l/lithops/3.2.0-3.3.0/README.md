# Comparing `tmp/lithops-3.2.0.tar.gz` & `tmp/lithops-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lithops-3.2.0.tar", last modified: Wed Mar 27 15:02:15 2024, max compression
+gzip compressed data, was "lithops-3.3.0.tar", last modified: Thu Apr 25 15:46:09 2024, max compression
```

## Comparing `lithops-3.2.0.tar` & `lithops-3.3.0.tar`

### file list

```diff
@@ -1,255 +1,254 @@
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:15.009384 lithops-3.2.0/
--rw-r--r--   0 josep     (1000) josep     (1000)    11357 2024-03-27 15:02:14.000000 lithops-3.2.0/LICENSE
--rw-r--r--   0 josep     (1000) josep     (1000)     1341 2024-03-27 15:02:15.009384 lithops-3.2.0/PKG-INFO
--rw-r--r--   0 josep     (1000) josep     (1000)     9405 2024-03-27 15:02:14.000000 lithops-3.2.0/README.md
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.979385 lithops-3.2.0/lithops/
--rw-r--r--   0 josep     (1000) josep     (1000)      490 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     9611 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4153 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/constants.py
--rw-r--r--   0 josep     (1000) josep     (1000)    33860 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/executors.py
--rw-r--r--   0 josep     (1000) josep     (1000)    13862 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/future.py
--rw-r--r--   0 josep     (1000) josep     (1000)    19644 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/invokers.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.979385 lithops-3.2.0/lithops/job/
--rw-r--r--   0 josep     (1000) josep     (1000)      128 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/job/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    13053 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/job/job.py
--rw-r--r--   0 josep     (1000) josep     (1000)    14699 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/job/partitioner.py
--rw-r--r--   0 josep     (1000) josep     (1000)     9589 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/job/serialize.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.979385 lithops-3.2.0/lithops/libs/
--rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/libs/__init__.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.979385 lithops-3.2.0/lithops/libs/globber/
--rw-r--r--   0 josep     (1000) josep     (1000)       72 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/libs/globber/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4385 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/libs/globber/globber.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.979385 lithops-3.2.0/lithops/libs/imp/
--rw-r--r--   0 josep     (1000) josep     (1000)      428 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/libs/imp/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2497 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/libs/imp/imp.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.979385 lithops-3.2.0/lithops/libs/multyvac/
--rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/libs/multyvac/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    14368 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/libs/multyvac/module_dependency.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.979385 lithops-3.2.0/lithops/libs/openwhisk/
--rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/libs/openwhisk/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    10745 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/libs/openwhisk/client.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.979385 lithops-3.2.0/lithops/localhost/
--rw-r--r--   0 josep     (1000) josep     (1000)      152 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/localhost/__init__.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.979385 lithops-3.2.0/lithops/localhost/v1/
--rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/localhost/v1/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    12259 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/localhost/v1/localhost.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2720 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/localhost/v1/runner.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.979385 lithops-3.2.0/lithops/localhost/v2/
--rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/localhost/v2/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    10612 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/localhost/v2/localhost.py
--rw-r--r--   0 josep     (1000) josep     (1000)     7330 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/localhost/v2/service.py
--rw-r--r--   0 josep     (1000) josep     (1000)    18089 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/monitor.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.979385 lithops-3.2.0/lithops/multiprocessing/
--rw-r--r--   0 josep     (1000) josep     (1000)     1346 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/multiprocessing/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1717 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/multiprocessing/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)    21677 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/multiprocessing/connection.py
--rw-r--r--   0 josep     (1000) josep     (1000)     5146 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/multiprocessing/context.py
--rw-r--r--   0 josep     (1000) josep     (1000)    22273 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/multiprocessing/managers.py
--rw-r--r--   0 josep     (1000) josep     (1000)     9391 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/multiprocessing/pool.py
--rw-r--r--   0 josep     (1000) josep     (1000)     7960 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/multiprocessing/process.py
--rw-r--r--   0 josep     (1000) josep     (1000)     5579 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/multiprocessing/queues.py
--rw-r--r--   0 josep     (1000) josep     (1000)     8911 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/multiprocessing/sharedctypes.py
--rw-r--r--   0 josep     (1000) josep     (1000)     9185 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/multiprocessing/synchronize.py
--rw-r--r--   0 josep     (1000) josep     (1000)     7884 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/multiprocessing/util.py
--rw-r--r--   0 josep     (1000) josep     (1000)     6323 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/plots.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.979385 lithops-3.2.0/lithops/scripts/
--rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/scripts/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     5904 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/scripts/cleaner.py
--rw-r--r--   0 josep     (1000) josep     (1000)    36090 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/scripts/cli.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.979385 lithops-3.2.0/lithops/serverless/
--rw-r--r--   0 josep     (1000) josep     (1000)       75 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/__init__.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.979385 lithops-3.2.0/lithops/serverless/backends/
--rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/__init__.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.979385 lithops-3.2.0/lithops/serverless/backends/aliyun_fc/
--rw-r--r--   0 josep     (1000) josep     (1000)      106 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/aliyun_fc/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    12637 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/aliyun_fc/aliyun_fc.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2733 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/aliyun_fc/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1606 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/aliyun_fc/entry_point.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.979385 lithops-3.2.0/lithops/serverless/backends/aws_batch/
--rw-r--r--   0 josep     (1000) josep     (1000)       93 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/aws_batch/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    26695 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/aws_batch/aws_batch.py
--rw-r--r--   0 josep     (1000) josep     (1000)     5430 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/aws_batch/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2851 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/aws_batch/entry_point.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.989385 lithops-3.2.0/lithops/serverless/backends/aws_lambda/
--rw-r--r--   0 josep     (1000) josep     (1000)       95 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/aws_lambda/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    29809 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/aws_lambda/aws_lambda.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1473 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/aws_lambda/build_layer.py
--rw-r--r--   0 josep     (1000) josep     (1000)     5753 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/aws_lambda/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1545 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/aws_lambda/entry_point.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.989385 lithops-3.2.0/lithops/serverless/backends/azure_containers/
--rw-r--r--   0 josep     (1000) josep     (1000)      109 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/azure_containers/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    13663 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/azure_containers/azure_containers.py
--rw-r--r--   0 josep     (1000) josep     (1000)     5678 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/azure_containers/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2401 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/azure_containers/entry_point.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.989385 lithops-3.2.0/lithops/serverless/backends/azure_functions/
--rw-r--r--   0 josep     (1000) josep     (1000)      107 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/azure_functions/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    15633 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/azure_functions/azure_functions.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4944 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/azure_functions/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2579 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/azure_functions/entry_point.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.989385 lithops-3.2.0/lithops/serverless/backends/code_engine/
--rw-r--r--   0 josep     (1000) josep     (1000)       97 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/code_engine/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    31342 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/code_engine/code_engine.py
--rw-r--r--   0 josep     (1000) josep     (1000)     5837 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/code_engine/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4436 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/code_engine/entry_point.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.989385 lithops-3.2.0/lithops/serverless/backends/gcp_cloudrun/
--rw-r--r--   0 josep     (1000) josep     (1000)       95 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/gcp_cloudrun/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    16890 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/gcp_cloudrun/cloudrun.py
--rw-r--r--   0 josep     (1000) josep     (1000)     5926 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/gcp_cloudrun/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2612 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/gcp_cloudrun/entry_point.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.989385 lithops-3.2.0/lithops/serverless/backends/gcp_functions/
--rw-r--r--   0 josep     (1000) josep     (1000)      101 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/gcp_functions/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     3439 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/gcp_functions/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2511 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/gcp_functions/entry_point.py
--rw-r--r--   0 josep     (1000) josep     (1000)    20582 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/gcp_functions/gcp_functions.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.989385 lithops-3.2.0/lithops/serverless/backends/ibm_cf/
--rw-r--r--   0 josep     (1000) josep     (1000)       99 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/ibm_cf/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     3378 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/ibm_cf/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1595 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/ibm_cf/entry_point.py
--rw-r--r--   0 josep     (1000) josep     (1000)    15454 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/ibm_cf/ibm_cf.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.989385 lithops-3.2.0/lithops/serverless/backends/k8s/
--rw-r--r--   0 josep     (1000) josep     (1000)       89 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/k8s/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     3792 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/k8s/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     7114 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/k8s/entry_point.py
--rw-r--r--   0 josep     (1000) josep     (1000)    30058 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/k8s/k8s.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.989385 lithops-3.2.0/lithops/serverless/backends/knative/
--rw-r--r--   0 josep     (1000) josep     (1000)       97 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/knative/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     5986 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/knative/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2614 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/knative/entry_point.py
--rw-r--r--   0 josep     (1000) josep     (1000)    30308 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/knative/knative.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.989385 lithops-3.2.0/lithops/serverless/backends/openwhisk/
--rw-r--r--   0 josep     (1000) josep     (1000)       94 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/openwhisk/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2221 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/openwhisk/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1604 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/openwhisk/entry_point.py
--rw-r--r--   0 josep     (1000) josep     (1000)     9655 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/openwhisk/openwhisk.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.989385 lithops-3.2.0/lithops/serverless/backends/oracle_f/
--rw-r--r--   0 josep     (1000) josep     (1000)      104 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/oracle_f/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     3022 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/oracle_f/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1646 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/oracle_f/entry_point.py
--rw-r--r--   0 josep     (1000) josep     (1000)    15246 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/backends/oracle_f/oracle_f.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4435 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/serverless/serverless.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.989385 lithops-3.2.0/lithops/standalone/
--rw-r--r--   0 josep     (1000) josep     (1000)      141 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/standalone/__init__.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.989385 lithops-3.2.0/lithops/standalone/backends/
--rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/standalone/backends/__init__.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.989385 lithops-3.2.0/lithops/standalone/backends/aws_ec2/
--rw-r--r--   0 josep     (1000) josep     (1000)       89 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/standalone/backends/aws_ec2/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    52469 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/standalone/backends/aws_ec2/aws_ec2.py
--rw-r--r--   0 josep     (1000) josep     (1000)     3122 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/standalone/backends/aws_ec2/config.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.989385 lithops-3.2.0/lithops/standalone/backends/azure_vms/
--rw-r--r--   0 josep     (1000) josep     (1000)       93 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/standalone/backends/azure_vms/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    36507 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/standalone/backends/azure_vms/azure_vms.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2781 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/standalone/backends/azure_vms/config.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.989385 lithops-3.2.0/lithops/standalone/backends/ibm_vpc/
--rw-r--r--   0 josep     (1000) josep     (1000)       89 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/standalone/backends/ibm_vpc/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4168 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/standalone/backends/ibm_vpc/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)    48122 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/standalone/backends/ibm_vpc/ibm_vpc.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.989385 lithops-3.2.0/lithops/standalone/backends/vm/
--rw-r--r--   0 josep     (1000) josep     (1000)       80 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/standalone/backends/vm/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1059 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/standalone/backends/vm/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     5020 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/standalone/backends/vm/vm.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4815 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/standalone/keeper.py
--rw-r--r--   0 josep     (1000) josep     (1000)    23663 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/standalone/master.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1961 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/standalone/runner.py
--rw-r--r--   0 josep     (1000) josep     (1000)    16922 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/standalone/standalone.py
--rw-r--r--   0 josep     (1000) josep     (1000)     8518 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/standalone/utils.py
--rw-r--r--   0 josep     (1000) josep     (1000)    10362 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/standalone/worker.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.989385 lithops-3.2.0/lithops/storage/
--rw-r--r--   0 josep     (1000) josep     (1000)      118 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/__init__.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.999384 lithops-3.2.0/lithops/storage/backends/
--rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/__init__.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.999384 lithops-3.2.0/lithops/storage/backends/aliyun_oss/
--rw-r--r--   0 josep     (1000) josep     (1000)      106 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/aliyun_oss/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     9359 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/aliyun_oss/aliyun_oss.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2069 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/aliyun_oss/config.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.999384 lithops-3.2.0/lithops/storage/backends/aws_s3/
--rw-r--r--   0 josep     (1000) josep     (1000)       78 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/aws_s3/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    10811 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/aws_s3/aws_s3.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1670 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/aws_s3/config.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.999384 lithops-3.2.0/lithops/storage/backends/azure_storage/
--rw-r--r--   0 josep     (1000) josep     (1000)       99 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/azure_storage/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     8780 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/azure_storage/azure_storage.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1371 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/azure_storage/config.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.999384 lithops-3.2.0/lithops/storage/backends/ceph/
--rw-r--r--   0 josep     (1000) josep     (1000)       85 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/ceph/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    11168 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/ceph/ceph.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1424 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/ceph/config.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.999384 lithops-3.2.0/lithops/storage/backends/gcp_storage/
--rw-r--r--   0 josep     (1000) josep     (1000)       91 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/gcp_storage/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1850 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/gcp_storage/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     8296 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/gcp_storage/gcp_storage.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.999384 lithops-3.2.0/lithops/storage/backends/ibm_cos/
--rw-r--r--   0 josep     (1000) josep     (1000)       98 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/ibm_cos/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4801 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/ibm_cos/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)    13502 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/ibm_cos/ibm_cos.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.999384 lithops-3.2.0/lithops/storage/backends/infinispan/
--rw-r--r--   0 josep     (1000) josep     (1000)       90 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/infinispan/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1051 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/infinispan/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)    10131 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/infinispan/infinispan.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.999384 lithops-3.2.0/lithops/storage/backends/infinispan_hotrod/
--rw-r--r--   0 josep     (1000) josep     (1000)      103 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/infinispan_hotrod/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1072 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/infinispan_hotrod/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     8918 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/infinispan_hotrod/infinispan_hotrod.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.999384 lithops-3.2.0/lithops/storage/backends/localhost/
--rw-r--r--   0 josep     (1000) josep     (1000)       95 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/localhost/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)      789 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/localhost/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     9548 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/localhost/localhost.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.999384 lithops-3.2.0/lithops/storage/backends/minio/
--rw-r--r--   0 josep     (1000) josep     (1000)       87 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/minio/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1434 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/minio/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)    11185 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/minio/minio.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.999384 lithops-3.2.0/lithops/storage/backends/oracle_oss/
--rw-r--r--   0 josep     (1000) josep     (1000)       96 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/oracle_oss/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1560 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/oracle_oss/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)    11362 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/oracle_oss/oracle_oss.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.999384 lithops-3.2.0/lithops/storage/backends/redis/
--rw-r--r--   0 josep     (1000) josep     (1000)       80 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/redis/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1007 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/redis/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     9625 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/redis/redis.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.999384 lithops-3.2.0/lithops/storage/backends/swift/
--rw-r--r--   0 josep     (1000) josep     (1000)       64 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/swift/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)      993 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/swift/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     9827 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/backends/swift/swift.py
--rw-r--r--   0 josep     (1000) josep     (1000)     7531 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/cloud_proxy.py
--rw-r--r--   0 josep     (1000) josep     (1000)    20834 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/storage.py
--rw-r--r--   0 josep     (1000) josep     (1000)     5051 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/storage/utils.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.999384 lithops-3.2.0/lithops/tests/
--rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/tests/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1361 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/tests/main_util.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2041 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/tests/test_call_async.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4708 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/tests/test_map.py
--rw-r--r--   0 josep     (1000) josep     (1000)     8466 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/tests/test_map_reduce.py
--rw-r--r--   0 josep     (1000) josep     (1000)    11815 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/tests/test_storage.py
--rw-r--r--   0 josep     (1000) josep     (1000)     3807 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/tests/test_template.py
--rw-r--r--   0 josep     (1000) josep     (1000)    10405 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/tests/tests_main.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.999384 lithops-3.2.0/lithops/tests/util_func/
--rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/tests/util_func/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)      597 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/tests/util_func/map_reduce_util.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2499 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/tests/util_func/map_util.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2324 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/tests/util_func/storage_util.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.999384 lithops-3.2.0/lithops/util/
--rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/util/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4204 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/util/ibm_token_manager.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.999384 lithops-3.2.0/lithops/util/joblib/
--rw-r--r--   0 josep     (1000) josep     (1000)      464 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/util/joblib/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     7596 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/util/joblib/lithops_backend.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1057 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/util/metrics.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4708 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/util/ssh_client.py
--rw-r--r--   0 josep     (1000) josep     (1000)    22687 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/utils.py
--rw-r--r--   0 josep     (1000) josep     (1000)       74 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/version.py
--rw-r--r--   0 josep     (1000) josep     (1000)    12264 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/wait.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:15.009384 lithops-3.2.0/lithops/worker/
--rw-r--r--   0 josep     (1000) josep     (1000)      138 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/worker/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    10174 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/worker/handler.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2888 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/worker/invoker.py
--rw-r--r--   0 josep     (1000) josep     (1000)    12891 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/worker/jobrunner.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4552 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/worker/status.py
--rw-r--r--   0 josep     (1000) josep     (1000)    11178 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops/worker/utils.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-03-27 15:02:14.979385 lithops-3.2.0/lithops.egg-info/
--rw-r--r--   0 josep     (1000) josep     (1000)     1341 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops.egg-info/PKG-INFO
--rw-r--r--   0 josep     (1000) josep     (1000)     7808 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops.egg-info/SOURCES.txt
--rw-r--r--   0 josep     (1000) josep     (1000)        1 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops.egg-info/dependency_links.txt
--rw-r--r--   0 josep     (1000) josep     (1000)       79 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops.egg-info/entry_points.txt
--rw-r--r--   0 josep     (1000) josep     (1000)      773 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops.egg-info/requires.txt
--rw-r--r--   0 josep     (1000) josep     (1000)        8 2024-03-27 15:02:14.000000 lithops-3.2.0/lithops.egg-info/top_level.txt
--rw-r--r--   0 josep     (1000) josep     (1000)       38 2024-03-27 15:02:15.009384 lithops-3.2.0/setup.cfg
--rw-r--r--   0 josep     (1000) josep     (1000)     2653 2024-03-27 15:02:14.000000 lithops-3.2.0/setup.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.742859 lithops-3.3.0/
+-rw-r--r--   0 josep     (1000) josep     (1000)    11357 2024-04-25 15:46:09.000000 lithops-3.3.0/LICENSE
+-rw-r--r--   0 josep     (1000) josep     (1000)     1363 2024-04-25 15:46:09.742859 lithops-3.3.0/PKG-INFO
+-rw-r--r--   0 josep     (1000) josep     (1000)     9399 2024-04-25 15:46:09.000000 lithops-3.3.0/README.md
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.712859 lithops-3.3.0/lithops/
+-rw-r--r--   0 josep     (1000) josep     (1000)      576 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     9545 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4153 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/constants.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    33987 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/executors.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    13862 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/future.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    19644 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/invokers.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/job/
+-rw-r--r--   0 josep     (1000) josep     (1000)      128 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/job/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    13053 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/job/job.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    14699 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/job/partitioner.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     9658 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/job/serialize.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/libs/
+-rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/libs/__init__.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/libs/globber/
+-rw-r--r--   0 josep     (1000) josep     (1000)       72 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/libs/globber/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4385 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/libs/globber/globber.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/libs/imp/
+-rw-r--r--   0 josep     (1000) josep     (1000)      428 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/libs/imp/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2497 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/libs/imp/imp.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/libs/inspect/
+-rw-r--r--   0 josep     (1000) josep     (1000)      120 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/libs/inspect/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5658 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/libs/inspect/inspect.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/libs/multyvac/
+-rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/libs/multyvac/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    14397 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/libs/multyvac/module_dependency.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/libs/openwhisk/
+-rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/libs/openwhisk/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    10745 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/libs/openwhisk/client.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/localhost/
+-rw-r--r--   0 josep     (1000) josep     (1000)      152 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/localhost/__init__.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/localhost/v1/
+-rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/localhost/v1/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    12369 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/localhost/v1/localhost.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2720 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/localhost/v1/runner.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/localhost/v2/
+-rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/localhost/v2/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    10612 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/localhost/v2/localhost.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     7330 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/localhost/v2/service.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    18089 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/monitor.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/multiprocessing/
+-rw-r--r--   0 josep     (1000) josep     (1000)     1346 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/multiprocessing/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1717 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/multiprocessing/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    21677 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/multiprocessing/connection.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5146 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/multiprocessing/context.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    22273 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/multiprocessing/managers.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     9391 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/multiprocessing/pool.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     7960 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/multiprocessing/process.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5579 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/multiprocessing/queues.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     8911 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/multiprocessing/sharedctypes.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     9185 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/multiprocessing/synchronize.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     7884 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/multiprocessing/util.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     6323 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/plots.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     7865 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/retries.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/scripts/
+-rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/scripts/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5904 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/scripts/cleaner.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    35956 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/scripts/cli.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/serverless/
+-rw-r--r--   0 josep     (1000) josep     (1000)       75 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/__init__.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/serverless/backends/
+-rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/__init__.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/serverless/backends/aliyun_fc/
+-rw-r--r--   0 josep     (1000) josep     (1000)      106 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aliyun_fc/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    12637 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aliyun_fc/aliyun_fc.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2733 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aliyun_fc/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1606 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aliyun_fc/entry_point.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/serverless/backends/aws_batch/
+-rw-r--r--   0 josep     (1000) josep     (1000)       93 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aws_batch/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    27091 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aws_batch/aws_batch.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5175 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aws_batch/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2851 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aws_batch/entry_point.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/serverless/backends/aws_lambda/
+-rw-r--r--   0 josep     (1000) josep     (1000)       95 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aws_lambda/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    29346 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aws_lambda/aws_lambda.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1473 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aws_lambda/build_layer.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5499 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aws_lambda/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1545 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aws_lambda/entry_point.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/serverless/backends/azure_containers/
+-rw-r--r--   0 josep     (1000) josep     (1000)      109 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/azure_containers/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    14266 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/azure_containers/azure_containers.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5678 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/azure_containers/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2401 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/azure_containers/entry_point.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/serverless/backends/azure_functions/
+-rw-r--r--   0 josep     (1000) josep     (1000)      107 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/azure_functions/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    15633 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/azure_functions/azure_functions.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4944 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/azure_functions/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2579 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/azure_functions/entry_point.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/serverless/backends/code_engine/
+-rw-r--r--   0 josep     (1000) josep     (1000)       97 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/code_engine/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    31342 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/code_engine/code_engine.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5837 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/code_engine/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4436 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/code_engine/entry_point.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/serverless/backends/gcp_cloudrun/
+-rw-r--r--   0 josep     (1000) josep     (1000)       95 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/gcp_cloudrun/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    16936 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/gcp_cloudrun/cloudrun.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5926 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/gcp_cloudrun/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2612 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/gcp_cloudrun/entry_point.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/serverless/backends/gcp_functions/
+-rw-r--r--   0 josep     (1000) josep     (1000)      101 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/gcp_functions/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     3439 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/gcp_functions/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2511 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/gcp_functions/entry_point.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    20582 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/gcp_functions/gcp_functions.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/serverless/backends/ibm_cf/
+-rw-r--r--   0 josep     (1000) josep     (1000)       99 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/ibm_cf/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     3378 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/ibm_cf/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1595 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/ibm_cf/entry_point.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    15478 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/ibm_cf/ibm_cf.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/serverless/backends/k8s/
+-rw-r--r--   0 josep     (1000) josep     (1000)       89 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/k8s/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     3792 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/k8s/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     7321 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/k8s/entry_point.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    31307 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/k8s/k8s.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/serverless/backends/knative/
+-rw-r--r--   0 josep     (1000) josep     (1000)       97 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/knative/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5986 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/knative/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2614 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/knative/entry_point.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    30354 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/knative/knative.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/serverless/backends/openwhisk/
+-rw-r--r--   0 josep     (1000) josep     (1000)       94 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/openwhisk/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2221 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/openwhisk/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1604 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/openwhisk/entry_point.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     9655 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/openwhisk/openwhisk.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/serverless/backends/oracle_f/
+-rw-r--r--   0 josep     (1000) josep     (1000)      104 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/oracle_f/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     3022 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/oracle_f/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1646 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/oracle_f/entry_point.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    15292 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/oracle_f/oracle_f.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4435 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/serverless.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/standalone/
+-rw-r--r--   0 josep     (1000) josep     (1000)      141 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/__init__.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/standalone/backends/
+-rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/__init__.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/standalone/backends/aws_ec2/
+-rw-r--r--   0 josep     (1000) josep     (1000)       89 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/aws_ec2/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    52738 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/aws_ec2/aws_ec2.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2781 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/aws_ec2/config.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/standalone/backends/azure_vms/
+-rw-r--r--   0 josep     (1000) josep     (1000)       93 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/azure_vms/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    37978 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/azure_vms/azure_vms.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2691 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/azure_vms/config.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/standalone/backends/ibm_vpc/
+-rw-r--r--   0 josep     (1000) josep     (1000)       89 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/ibm_vpc/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4082 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/ibm_vpc/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    48122 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/ibm_vpc/ibm_vpc.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/standalone/backends/vm/
+-rw-r--r--   0 josep     (1000) josep     (1000)       80 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/vm/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1059 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/vm/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5020 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/vm/vm.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4815 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/keeper.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    23693 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/master.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1961 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/runner.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    16922 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/standalone.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     8567 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/utils.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    10362 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/worker.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/storage/
+-rw-r--r--   0 josep     (1000) josep     (1000)      118 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/__init__.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/storage/backends/
+-rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/__init__.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/storage/backends/aliyun_oss/
+-rw-r--r--   0 josep     (1000) josep     (1000)      106 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/aliyun_oss/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     9631 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/aliyun_oss/aliyun_oss.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1742 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/aliyun_oss/config.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/storage/backends/aws_s3/
+-rw-r--r--   0 josep     (1000) josep     (1000)       78 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/aws_s3/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    10713 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/aws_s3/aws_s3.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1189 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/aws_s3/config.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/storage/backends/azure_storage/
+-rw-r--r--   0 josep     (1000) josep     (1000)       99 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/azure_storage/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     9192 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/azure_storage/azure_storage.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1025 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/azure_storage/config.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/storage/backends/ceph/
+-rw-r--r--   0 josep     (1000) josep     (1000)       85 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/ceph/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    11552 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/ceph/ceph.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1125 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/ceph/config.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/storage/backends/gcp_storage/
+-rw-r--r--   0 josep     (1000) josep     (1000)       91 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/gcp_storage/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1530 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/gcp_storage/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     8656 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/gcp_storage/gcp_storage.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/storage/backends/ibm_cos/
+-rw-r--r--   0 josep     (1000) josep     (1000)       98 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/ibm_cos/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     3901 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/ibm_cos/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    14099 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/ibm_cos/ibm_cos.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/storage/backends/infinispan/
+-rw-r--r--   0 josep     (1000) josep     (1000)       90 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/infinispan/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1051 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/infinispan/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    10131 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/infinispan/infinispan.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.742859 lithops-3.3.0/lithops/storage/backends/infinispan_hotrod/
+-rw-r--r--   0 josep     (1000) josep     (1000)      103 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/infinispan_hotrod/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1072 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/infinispan_hotrod/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     8918 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/infinispan_hotrod/infinispan_hotrod.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.742859 lithops-3.3.0/lithops/storage/backends/localhost/
+-rw-r--r--   0 josep     (1000) josep     (1000)       95 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/localhost/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)      789 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/localhost/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     9548 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/localhost/localhost.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.742859 lithops-3.3.0/lithops/storage/backends/minio/
+-rw-r--r--   0 josep     (1000) josep     (1000)       87 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/minio/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1131 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/minio/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    11569 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/minio/minio.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.742859 lithops-3.3.0/lithops/storage/backends/oracle_oss/
+-rw-r--r--   0 josep     (1000) josep     (1000)       96 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/oracle_oss/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1303 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/oracle_oss/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    11630 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/oracle_oss/oracle_oss.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.742859 lithops-3.3.0/lithops/storage/backends/redis/
+-rw-r--r--   0 josep     (1000) josep     (1000)       80 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/redis/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1007 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/redis/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     9625 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/redis/redis.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.742859 lithops-3.3.0/lithops/storage/backends/swift/
+-rw-r--r--   0 josep     (1000) josep     (1000)       64 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/swift/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)      993 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/swift/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     9922 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/swift/swift.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     7531 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/cloud_proxy.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    20932 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/storage.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5052 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/utils.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.742859 lithops-3.3.0/lithops/tests/
+-rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/tests/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1662 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/tests/conftest.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4176 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/tests/functions.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2025 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/tests/test_call_async.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4508 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/tests/test_map.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     9375 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/tests/test_map_reduce.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4982 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/tests/test_retries.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    12045 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/tests/test_storage.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.742859 lithops-3.3.0/lithops/util/
+-rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/util/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4204 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/util/ibm_token_manager.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.742859 lithops-3.3.0/lithops/util/joblib/
+-rw-r--r--   0 josep     (1000) josep     (1000)      464 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/util/joblib/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     7596 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/util/joblib/lithops_backend.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1057 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/util/metrics.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4708 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/util/ssh_client.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    22687 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/utils.py
+-rw-r--r--   0 josep     (1000) josep     (1000)       74 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/version.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    12264 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/wait.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.742859 lithops-3.3.0/lithops/worker/
+-rw-r--r--   0 josep     (1000) josep     (1000)      138 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/worker/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    10174 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/worker/handler.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2888 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/worker/invoker.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    12849 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/worker/jobrunner.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4510 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/worker/status.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    11178 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/worker/utils.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops.egg-info/
+-rw-r--r--   0 josep     (1000) josep     (1000)     1363 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops.egg-info/PKG-INFO
+-rw-r--r--   0 josep     (1000) josep     (1000)     7734 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops.egg-info/SOURCES.txt
+-rw-r--r--   0 josep     (1000) josep     (1000)        1 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops.egg-info/dependency_links.txt
+-rw-r--r--   0 josep     (1000) josep     (1000)       79 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops.egg-info/entry_points.txt
+-rw-r--r--   0 josep     (1000) josep     (1000)      796 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops.egg-info/requires.txt
+-rw-r--r--   0 josep     (1000) josep     (1000)        8 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops.egg-info/top_level.txt
+-rw-r--r--   0 josep     (1000) josep     (1000)       38 2024-04-25 15:46:09.742859 lithops-3.3.0/setup.cfg
+-rw-r--r--   0 josep     (1000) josep     (1000)     2694 2024-04-25 15:46:09.000000 lithops-3.3.0/setup.py
```

### Comparing `lithops-3.2.0/LICENSE` & `lithops-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/PKG-INFO` & `lithops-3.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lithops
-Version: 3.2.0
+Version: 3.3.0
 Summary: Lithops lets you transparently run your Python applications in the Cloud
 Home-page: https://github.com/lithops-cloud/lithops
 Author: Gil Vernik, Josep Sampe
 Author-email: gilv@ibm.com, josep.sampe@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,11 +27,12 @@
 Provides-Extra: aliyun
 Provides-Extra: all
 Provides-Extra: azure
 Provides-Extra: gcp
 Provides-Extra: joblib
 Provides-Extra: multiprocessing
 Provides-Extra: oracle
+Provides-Extra: tests
 License-File: LICENSE
 
 UNKNOWN
```

### Comparing `lithops-3.2.0/README.md` & `lithops-3.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -71,16 +71,16 @@
 ```python
 from lithops import FunctionExecutor
 
 def hello(name):
     return f'Hello {name}!'
 
 with FunctionExecutor() as fexec:
-    fut = fexec.call_async(hello, 'World')
-    print(fut.result())
+    f = fexec.call_async(hello, 'World')
+    print(f.result())
 ```
 </td>
 <td>
 
 ```python
 from lithops.multiprocessing import Pool
 
@@ -116,22 +116,22 @@
 
 if __name__ == "__main__":
     st = Storage()
     st.put_object(bucket='mybucket',
                   key='test.txt',
                   body='Hello World')
 
-    print(st.get_object(bucket='mybucket',
+    print(st.get_object(bucket='lithops',
                         key='test.txt'))
 ```
 </td>
 <td>
 
 ```python
-from lithops.storage.cloud_proxy import os 
+from lithops.storage.cloud_proxy import os
 
 if __name__ == "__main__":
     filepath = 'bar/foo.txt'
     with os.open(filepath, 'w') as f:
         f.write('Hello world!')
 
     dirname = os.path.dirname(filepath)
```

### Comparing `lithops-3.2.0/lithops/config.py` & `lithops-3.3.0/lithops/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,16 +241,14 @@
 def extract_storage_config(config):
     s_config = {}
     backend = config['lithops']['storage']
     s_config['backend'] = backend
     s_config[backend] = config[backend] if backend in config and config[backend] else {}
     s_config[backend]['user_agent'] = f'lithops/{__version__}'
 
-    s_config['bucket'] = s_config[backend].get('storage_bucket')
-
     return s_config
 
 
 def extract_localhost_config(config):
     localhost_config = config[c.LOCALHOST].copy()
 
     return localhost_config
```

### Comparing `lithops-3.2.0/lithops/constants.py` & `lithops-3.3.0/lithops/constants.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/executors.py` & `lithops-3.3.0/lithops/executors.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
                 config_ow['lithops'][key] = value
 
         # Load configuration
         self.config = default_config(config_file=config_file, config_data=config, config_overwrite=config_ow)
 
         self.data_cleaner = self.config['lithops'].get('data_cleaner', True)
         if self.data_cleaner and not self.is_lithops_worker:
-            atexit.register(self.clean, clean_cloudobjects=False, clean_fn=True)
+            atexit.register(self.clean, clean_cloudobjects=False, clean_fn=True, on_exit=True)
 
         storage_config = extract_storage_config(self.config)
         self.internal_storage = InternalStorage(storage_config)
         self.storage = self.internal_storage.storage
 
         self.backend = self.config['lithops']['backend']
         self.mode = self.config['lithops']['mode']
@@ -158,15 +158,15 @@
         self.job_monitor.stop()
         self.invoker.stop()
         self.compute_handler.clear()
 
     def _create_job_id(self, call_type):
         job_id = str(self.total_jobs).zfill(3)
         self.total_jobs += 1
-        return '{}{}'.format(call_type, job_id)
+        return f'{call_type}{job_id}'
 
     def call_async(
         self,
         func: Callable,
         data: Union[List[Any], Tuple[Any, ...], Dict[str, Any]],
         extra_env: Optional[Dict] = None,
         runtime_memory: Optional[int] = None,
@@ -553,26 +553,28 @@
 
     def clean(
         self,
         fs: Optional[Union[ResponseFuture, List[ResponseFuture]]] = None,
         cs: Optional[List[CloudObject]] = None,
         clean_cloudobjects: Optional[bool] = True,
         clean_fn: Optional[bool] = False,
-        force: Optional[bool] = False
+        force: Optional[bool] = False,
+        on_exit: Optional[bool] = False
     ):
         """
         Deletes all the temp files from storage. These files include the function,
         the data serialization and the function invocation results. It can also clean
         cloudobjects.
 
         :param fs: List of futures to clean
         :param cs: List of cloudobjects to clean
         :param clean_cloudobjects: Delete all cloudobjects created with this executor
         :param clean_fn: Delete cached functions in this executor
         :param force: Clean all future objects even if they have not benn completed
+        :parma on_exit: do not print logs on exit
         """
         global CLEANER_PROCESS
 
         def save_data_to_clean(data):
             with tempfile.NamedTemporaryFile(dir=CLEANER_DIR, delete=False) as temp:
                 pickle.dump(data, temp)
 
@@ -600,15 +602,16 @@
         futures = fs or self.futures
         futures = [futures] if type(futures) is not list else futures
         present_jobs = {create_job_key(f.executor_id, f.job_id) for f in futures
                         if (f.executor_id.count('-') == 1 and f.done) or force}
         jobs_to_clean = present_jobs - self.cleaned_jobs
 
         if jobs_to_clean:
-            logger.info(f'ExecutorID {self.executor_id} - Cleaning temporary data')
+            if not on_exit:
+                logger.info(f'ExecutorID {self.executor_id} - Cleaning temporary data')
             data = {
                 'jobs_to_clean': jobs_to_clean,
                 'clean_cloudobjects': clean_cloudobjects,
                 'storage_config': self.internal_storage.get_storage_config()
             }
             save_data_to_clean(data)
             self.cleaned_jobs.update(jobs_to_clean)
```

### Comparing `lithops-3.2.0/lithops/future.py` & `lithops-3.3.0/lithops/future.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/invokers.py` & `lithops-3.3.0/lithops/invokers.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/job/job.py` & `lithops-3.3.0/lithops/job/job.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/job/partitioner.py` & `lithops-3.3.0/lithops/job/partitioner.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/job/serialize.py` & `lithops-3.3.0/lithops/job/serialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from pathlib import Path
 from dis import Bytecode
 from functools import reduce
 from importlib import import_module
 from types import CodeType, FunctionType, ModuleType
 
 from lithops.libs import imp
+from lithops.libs import inspect as linspect
 from lithops.utils import bytes_to_b64str
 from lithops.libs.multyvac.module_dependency import ModuleDependencyAnalyzer
 
 logger = logging.getLogger(__name__)
 
 
 class SerializeIndependent:
@@ -128,35 +129,35 @@
         mods = set()
 
         if inspect.isfunction(obj) or (inspect.ismethod(obj) and inspect.isfunction(obj.__func__)):
             # The obj is the user's function
             worklist.append(obj)
 
         elif type(obj).__name__ == 'cython_function_or_method':
-            for k, v in inspect.getmembers(obj):
+            for k, v in linspect.getmembers_static(obj):
                 if k == '__globals__':
                     mods.add(v['__file__'])
 
         elif type(obj) is dict:
             # the obj is the user's iterdata
             for param in obj.values():
                 if type(param).__module__ == "__builtin__":
                     continue
                 elif inspect.isfunction(param):
                     # it is a user defined function
                     worklist.append(param)
                 else:
                     # it is a user defined class
-                    for k, v in inspect.getmembers(param):
+                    for k, v in linspect.getmembers_static(param):
                         if inspect.isfunction(v) or (inspect.ismethod(v) and inspect.isfunction(v.__func__)):
                             worklist.append(v)
         else:
             # The obj is the user's function but in form of a class
             found_methods = []
-            for k, v in inspect.getmembers(obj):
+            for k, v in linspect.getmembers_static(obj):
                 if inspect.isfunction(v) or (inspect.ismethod(v) and inspect.isfunction(v.__func__)):
                     found_methods.append(k)
                     worklist.append(v)
             if "__call__" not in found_methods:
                 raise Exception('The class you passed as the function to '
                                 'run must contain the "__call__" method')
```

### Comparing `lithops-3.2.0/lithops/libs/globber/globber.py` & `lithops-3.3.0/lithops/libs/globber/globber.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/libs/imp/imp.py` & `lithops-3.3.0/lithops/libs/imp/imp.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/libs/multyvac/module_dependency.py` & `lithops-3.3.0/lithops/libs/multyvac/module_dependency.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,16 @@
         else:
             # Add module to set of scanned modules, before we've analyzed it
             self._inspected_modules.add(root_module_name)
 
         # logger.debug('Inspecting module %r', root_module_name)
         try:
             fp, pathname, description = imp.find_module(root_module_name)
-            logger.debug(f"Module '{root_module_name}' found in {pathname}")
+            if pathname:
+                logger.debug(f"Module '{root_module_name}' found in {pathname}")
         except ImportError:
             logger.debug('Could not find module %r, skipping', root_module_name)
             return
         _, _, mod_type = description
         if mod_type == imp.PY_SOURCE:
             self._modules.add(root_module_name)
             self._paths_to_transmit.add(pathname)
```

### Comparing `lithops-3.2.0/lithops/libs/openwhisk/client.py` & `lithops-3.3.0/lithops/libs/openwhisk/client.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/localhost/v1/localhost.py` & `lithops-3.3.0/lithops/localhost/v1/localhost.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,18 @@
         def job_manager():
             logger.debug('Staring localhost job manager')
             self.should_run = True
 
             while self.should_run:
                 job_payload, job_filename = self.job_queue.get()
                 if job_payload is None and job_filename is None:
-                    break
+                    if self.job_queue.empty():
+                        break
+                    else:
+                        continue
                 executor_id = job_payload['executor_id']
                 job_id = job_payload['job_id']
                 total_calls = len(job_payload['call_ids'])
                 job_key = job_payload['job_key']
                 logger.debug(f'ExecutorID {executor_id} | JobID {job_id} - Running '
                              f'{total_calls} activations in the localhost worker')
                 process = self.env.run(job_key, job_filename)
```

### Comparing `lithops-3.2.0/lithops/localhost/v1/runner.py` & `lithops-3.3.0/lithops/localhost/v1/runner.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/localhost/v2/localhost.py` & `lithops-3.3.0/lithops/localhost/v2/localhost.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/localhost/v2/service.py` & `lithops-3.3.0/lithops/localhost/v2/service.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/monitor.py` & `lithops-3.3.0/lithops/monitor.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/multiprocessing/__init__.py` & `lithops-3.3.0/lithops/multiprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/multiprocessing/config.py` & `lithops-3.3.0/lithops/multiprocessing/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/multiprocessing/connection.py` & `lithops-3.3.0/lithops/multiprocessing/connection.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/multiprocessing/context.py` & `lithops-3.3.0/lithops/multiprocessing/context.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/multiprocessing/managers.py` & `lithops-3.3.0/lithops/multiprocessing/managers.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/multiprocessing/pool.py` & `lithops-3.3.0/lithops/multiprocessing/pool.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/multiprocessing/process.py` & `lithops-3.3.0/lithops/multiprocessing/process.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/multiprocessing/queues.py` & `lithops-3.3.0/lithops/multiprocessing/queues.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/multiprocessing/sharedctypes.py` & `lithops-3.3.0/lithops/multiprocessing/sharedctypes.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/multiprocessing/synchronize.py` & `lithops-3.3.0/lithops/multiprocessing/synchronize.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/multiprocessing/util.py` & `lithops-3.3.0/lithops/multiprocessing/util.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/plots.py` & `lithops-3.3.0/lithops/plots.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/scripts/cleaner.py` & `lithops-3.3.0/lithops/scripts/cleaner.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/scripts/cli.py` & `lithops-3.3.0/lithops/scripts/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,19 +27,14 @@
 from tabulate import tabulate
 from datetime import datetime
 from concurrent.futures import ThreadPoolExecutor
 
 import lithops
 from lithops import Storage
 from lithops.version import __version__
-from lithops.tests.tests_main import (
-    print_test_functions,
-    print_test_groups,
-    run_tests
-)
 from lithops.utils import (
     get_mode,
     setup_lithops_logger,
     verify_runtime_name,
     sizeof_fmt
 )
 from lithops.config import (
@@ -131,16 +126,16 @@
 
     compute_handler.clean(all=all)
 
     # Clean object storage temp dirs
     storage = internal_storage.storage
     runtimes_path = RUNTIMES_PREFIX + '/' + backend
     jobs_path = JOBS_PREFIX
-    clean_bucket(storage, storage_config['bucket'], runtimes_path, sleep=1)
-    clean_bucket(storage, storage_config['bucket'], jobs_path, sleep=1)
+    clean_bucket(storage, storage.bucket, runtimes_path, sleep=1)
+    clean_bucket(storage, storage.bucket, jobs_path, sleep=1)
 
     # Clean localhost executor temp dirs
     shutil.rmtree(LITHOPS_TEMP_DIR, ignore_errors=True)
     # Clean local lithops runtime cache
     shutil.rmtree(os.path.join(CACHE_DIR, RUNTIMES_PREFIX, backend), ignore_errors=True)
 
     logger.info('All Lithops temporary data cleaned')
@@ -148,38 +143,47 @@
 
 @lithops_cli.command('test')
 @click.option('--config', '-c', default=None, help='Path to yaml config file', type=click.Path(exists=True))
 @click.option('--backend', '-b', default=None, help='Compute backend')
 @click.option('--storage', '-s', default=None, help='Storage backend')
 @click.option('--debug', '-d', is_flag=True, help='Debug mode')
 @click.option('--region', '-r', default=None, help='compute backend region')
-@click.option('--test', '-t', default='all', help='Run a specific tester. To avoid running similarly named tests '
-                                                  'you may prefix the tester with its test class, '
-                                                  'e.g. TestClass.test_name. '
-                                                  'Type "-t help" for the complete tests list')
-@click.option('--groups', '-g', default=None, help='Run all testers belonging to a specific group.'
-                                                   ' type "-g help" for groups list')
-@click.option('--fail_fast', '-f', is_flag=True, help='Stops test run upon first occurrence of a failed test')
-@click.option('--keep_datasets', '-k', is_flag=True, help='keeps datasets in storage after the test run. '
-                                                          'Meant to serve some use-cases in github workflow.')
-def test(test, config, backend, groups, storage, debug, region, fail_fast, keep_datasets):
-    config = load_yaml_config(config) if config else None
+@click.option('--test', '-t', default=None, help='Run a specific test. To avoid running similarly named tests '
+                                                 'you may prefix the tester with its test class, '
+                                                 'e.g. TestAsync::test_call_async'
+                                                 'Type "-t help" for the complete tests list')
+@click.option('--exitfirst', '-x', is_flag=True, help='Stops test run upon first occurrence of a failed test')
+def test(test, config, backend, storage, debug, region, exitfirst):
+    import pytest
 
-    log_level = logging.INFO if not debug else logging.DEBUG
-    setup_lithops_logger(log_level)
-
-    if groups and test == 'all':  # if user specified a group(s) avoid running all tests.
-        test = ''
+    dir_path = os.path.dirname(os.path.realpath(__file__))
+    tests_path = os.path.abspath(os.path.join(dir_path, '..', 'tests'))
 
     if test == 'help':
-        print_test_functions()
-    elif groups == 'help':
-        print_test_groups()
+        pytest.main([tests_path, "--collect-only"])
     else:
-        run_tests(test, config, groups, backend, storage, region, fail_fast, keep_datasets)
+        cmd_string = [tests_path, "-v"]
+        if exitfirst:
+            cmd_string.extend(["-x"])
+        if debug:
+            cmd_string.extend(["-o", "log_cli=true", "--log-cli-level=DEBUG"])
+        if config:
+            cmd_string.extend(["--config", config])
+        if backend:
+            cmd_string.extend(["--backend", backend])
+        if storage:
+            cmd_string.extend(["--storage", storage])
+        if region:
+            cmd_string.extend(["--region", region])
+        if test:
+            cmd_string.extend(["-k", test])
+
+        print("Executing lithops tests: pytest " + ' '.join(cmd_string[1:]))
+
+        pytest.main(cmd_string)
 
 
 @lithops_cli.command('hello')
 @click.option('--config', '-c', default=None, help='path to yaml config file', type=click.Path(exists=True))
 @click.option('--backend', '-b', default=None, help='compute backend')
 @click.option('--storage', '-s', default=None, help='storage backend')
 @click.option('--debug', '-d', is_flag=True, help='debug mode')
```

### Comparing `lithops-3.2.0/lithops/serverless/backends/aliyun_fc/aliyun_fc.py` & `lithops-3.3.0/lithops/serverless/backends/aliyun_fc/aliyun_fc.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/aliyun_fc/config.py` & `lithops-3.3.0/lithops/serverless/backends/aliyun_fc/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/aliyun_fc/entry_point.py` & `lithops-3.3.0/lithops/serverless/backends/aliyun_fc/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/aws_batch/aws_batch.py` & `lithops-3.3.0/lithops/serverless/backends/aws_batch/aws_batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import copy
 import json
 import os
 import re
 import logging
 import subprocess
 import sys
+import botocore
 import time
 import boto3
 
 from lithops import utils
 from lithops.version import __version__
 from lithops.constants import COMPUTE_CLI_MSG
 from lithops.storage.utils import StorageNoSuchKeyError
@@ -32,68 +33,81 @@
 from . import config as batch_config
 
 logger = logging.getLogger(__name__)
 
 
 class AWSBatchBackend:
 
-    def __init__(self, aws_batch_config, internal_storage):
+    def __init__(self, batch_config, internal_storage):
         """
         Initialize AWS Batch Backend
         """
-        logger.debug('Creating AWS Lambda client')
+        logger.debug('Creating AWS Batch client')
 
         self.name = 'aws_batch'
         self.type = utils.BackendType.BATCH.value
-        self.aws_batch_config = aws_batch_config
+        self.aws_batch_config = batch_config
+        self.user_agent = batch_config['user_agent']
+        self.region = batch_config['region']
+        self.env_type = batch_config['env_type']
+        self.namespace = batch_config.get('namespace')
+
+        self.aws_session = boto3.Session(
+            aws_access_key_id=batch_config.get('access_key_id'),
+            aws_secret_access_key=batch_config.get('secret_access_key'),
+            aws_session_token=batch_config.get('session_token'),
+            region_name=self.region
+        )
+        self.batch_client = self.aws_session.client('batch')
 
-        self.user_key = aws_batch_config['access_key_id'][-4:]
-        self.package = f'lithops_v{__version__.replace(".", "-")}_{self.user_key}'
-        self.region_name = aws_batch_config['region']
-
-        self._env_type = self.aws_batch_config['env_type']
-        self._queue_name = f'{self.package}_{self._env_type.replace("_", "-")}_queue'
-        self._compute_env_name = f'{self.package}_{self._env_type.replace("_", "-")}_env'
-
-        logger.debug('Creating Boto3 AWS Session and Batch Client')
-        self.aws_session = boto3.Session(aws_access_key_id=aws_batch_config['access_key_id'],
-                                         aws_secret_access_key=aws_batch_config['secret_access_key'],
-                                         aws_session_token=aws_batch_config.get('session_token'),
-                                         region_name=self.region_name)
-        self.batch_client = self.aws_session.client('batch', region_name=self.region_name)
+        self.batch_client = self.aws_session.client(
+            'batch', config=botocore.client.Config(
+                user_agent_extra=self.user_agent
+            )
+        )
 
         self.internal_storage = internal_storage
 
-        if 'account_id' in self.aws_batch_config:
-            self.account_id = self.aws_batch_config['account_id']
-        else:
-            sts_client = self.aws_session.client('sts', region_name=self.region_name)
-            self.account_id = sts_client.get_caller_identity()["Account"]
+        if 'account_id' not in batch_config or 'user_id' not in batch_config:
+            sts_client = self.aws_session.client('sts')
+            identity = sts_client.get_caller_identity()
+
+        self.account_id = batch_config.get('account_id') or identity["Account"]
+        self.user_id = batch_config.get('user_id') or identity["UserId"]
+        self.user_key = self.user_id.split(":")[0][-4:].lower()
+
+        self.ecr_client = self.aws_session.client('ecr')
+        package = f'lithops_v{__version__.replace(".", "")}_{self.user_key}'
+        self.package = f"{package}_{self.namespace}" if self.namespace else package
 
-        self.ecr_client = self.aws_session.client('ecr', region_name=self.region_name)
+        self._queue_name = f'{self.package}_{self.env_type.replace("_", "-")}_queue'
+        self._compute_env_name = f'{self.package}_{self.env_type.replace("_", "-")}_env'
 
         msg = COMPUTE_CLI_MSG.format('AWS Batch')
-        logger.info("{} - Region: {}".format(msg, self.region_name))
+        if self.namespace:
+            logger.info(f"{msg} - Region: {self.region} - Namespace: {self.namespace} - Env: {self.env_type}")
+        else:
+            logger.info(f"{msg} - Region: {self.region} - Env: {self.env_type}")
 
     def _get_default_runtime_image_name(self):
         python_version = utils.CURRENT_PY_VERSION.replace('.', '')
         revision = 'latest' if 'dev' in __version__ else __version__.replace('.', '')
         return f'batch-default-runtime-v{python_version}:{revision}'
 
     def _get_full_image_name(self, runtime_name):
         full_image_name = runtime_name if ':' in runtime_name else f'{runtime_name}:latest'
-        registry = f'{self.account_id}.dkr.ecr.{self.region_name}.amazonaws.com'
+        registry = f'{self.account_id}.dkr.ecr.{self.region}.amazonaws.com'
         full_image_name = '/'.join([registry, self.package.replace('-', '.'), full_image_name]).lower()
         repo_name = full_image_name.split('/', 1)[1:].pop().split(':')[0]
         return full_image_name, registry, repo_name
 
     def _format_jobdef_name(self, runtime_name, runtime_memory, version=__version__):
         fmt_runtime_name = runtime_name.replace('/', '--').replace(':', '--')
         package = self.package.replace(__version__.replace(".", "-"), version.replace(".", "-"))
-        return f'{package}--{self._env_type}--{fmt_runtime_name}--{runtime_memory}mb'
+        return f'{package}--{self.env_type}--{fmt_runtime_name}--{runtime_memory}mb'
 
     def _unformat_jobdef_name(self, jobdef_name):
         # Default jobdef name is "lithops_v2-7-2_WU5O--FARGATE_SPOT--batch-default-runtime-v39--latest--1024mb"
         prefix, env_type, runtime = jobdef_name.split('--', 2)
         version = prefix.replace('lithops_v', '').split('_')[0].replace('-', '.')
         runtime_name, memory = runtime.rsplit("--", 1)
         return runtime_name.replace('--', ':'), memory.replace('mb', ''), version
@@ -118,18 +132,18 @@
             compute_resources_spec = {
                 'type': self.aws_batch_config['env_type'],
                 'maxvCpus': self.aws_batch_config['env_max_cpus'],
                 'subnets': self.aws_batch_config['subnets'],
                 'securityGroupIds': self.aws_batch_config['security_groups']
             }
 
-            if self._env_type == 'SPOT':
+            if self.env_type == 'SPOT':
                 compute_resources_spec['allocationStrategy'] = 'SPOT_CAPACITY_OPTIMIZED'
 
-            if self._env_type in {'EC2', 'SPOT'}:
+            if self.env_type in {'EC2', 'SPOT'}:
                 compute_resources_spec['instanceRole'] = self.aws_batch_config['instance_role']
                 compute_resources_spec['minvCpus'] = 0
                 compute_resources_spec['instanceTypes'] = ['optimal']
 
             if 'service_role' in self.aws_batch_config:
                 res = self.batch_client.create_compute_environment(
                     computeEnvironmentName=self._compute_env_name,
@@ -244,20 +258,20 @@
             logger.error(job_queues)
             raise Exception('More than one job queue with the same name')
 
     def _create_job_def(self, runtime_name, runtime_memory):
         job_def_name = self._format_jobdef_name(runtime_name, runtime_memory)
         job_def = self._get_job_def(job_def_name)
 
-        if self._env_type in {'EC2', 'SPOT'}:
+        if self.env_type in {'EC2', 'SPOT'}:
             platform_capabilities = ['EC2']
-        elif self._env_type in {'FARGATE', 'FARGATE_SPOT'}:
+        elif self.env_type in {'FARGATE', 'FARGATE_SPOT'}:
             platform_capabilities = ['FARGATE']
         else:
-            raise Exception(f'Unknown env type {self._env_type}')
+            raise Exception(f'Unknown env type {self.env_type}')
 
         if job_def is None:
             logger.debug(f'Creating new Job Definition {job_def_name}')
             image_name, _, _ = self._get_full_image_name(runtime_name)
 
             container_properties = {
                 'image': image_name,
@@ -270,15 +284,15 @@
                     {
                         'type': 'MEMORY',
                         'value': str(self.aws_batch_config['runtime_memory'])
                     }
                 ],
             }
 
-            if self._env_type in {'FARGATE', 'FARGATE_SPOT'}:
+            if self.env_type in {'FARGATE', 'FARGATE_SPOT'}:
                 container_properties['networkConfiguration'] = {
                     'assignPublicIp': 'ENABLED' if self.aws_batch_config['assign_public_ip'] else 'DISABLED'
                 }
 
             res = self.batch_client.register_job_definition(
                 jobDefinitionName=job_def_name,
                 type='container',
@@ -376,17 +390,17 @@
         auth_data = res['authorizationData'].pop()
         ecr_token = base64.b64decode(auth_data['authorizationToken']).split(b':')[1]
 
         full_image_name, registry, repo_name = self._get_full_image_name(runtime_name)
 
         if runtime_file:
             assert os.path.isfile(runtime_file), f'Cannot locate "{runtime_file}"'
-            cmd = f'{docker_path} build -t {full_image_name} -f {runtime_file} . '
+            cmd = f'{docker_path} build --platform=linux/amd64 -t {full_image_name} -f {runtime_file} . '
         else:
-            cmd = f'{docker_path} build -t {full_image_name} . '
+            cmd = f'{docker_path} build --platform=linux/amd64 -t {full_image_name} . '
         cmd = cmd + ' '.join(extra_args)
 
         try:
             entry_point = os.path.join(os.path.dirname(__file__), 'entry_point.py')
             utils.create_handler_zip(os.path.join(os.getcwd(), batch_config.RUNTIME_ZIP), entry_point)
             utils.run_command(cmd)
         finally:
@@ -581,15 +595,15 @@
                         }
                     ]
                 }
             )
 
     def get_runtime_key(self, runtime_name, runtime_memory, version=__version__):
         jobdef_name = self._format_jobdef_name(runtime_name, runtime_memory, version)
-        runtime_key = os.path.join(self.name, version, self.region_name, jobdef_name)
+        runtime_key = os.path.join(self.name, version, self.region, jobdef_name)
         return runtime_key
 
     def get_runtime_info(self):
         """
         Method that returns all the relevant information about the runtime set
         in config
         """
```

### Comparing `lithops-3.2.0/lithops/serverless/backends/aws_batch/config.py` & `lithops-3.3.0/lithops/serverless/backends/aws_batch/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,23 +69,20 @@
 
 ENTRYPOINT python entry_point.py
 """
 
 
 def load_config(config_data):
 
-    if 'aws' not in config_data:
-        raise Exception("'aws' section is mandatory in the configuration")
-
-    if not {'access_key_id', 'secret_access_key'}.issubset(set(config_data['aws'])):
-        raise Exception("'access_key_id' and 'secret_access_key' are mandatory under the 'aws' section of the configuration")
-
     if not config_data['aws_batch']:
         raise Exception("'aws_batch' section is mandatory in the configuration")
 
+    if 'aws' not in config_data:
+        config_data['aws'] = {}
+
     temp = copy.deepcopy(config_data['aws_batch'])
     config_data['aws_batch'].update(config_data['aws'])
     config_data['aws_batch'].update(temp)
 
     for param in REQ_PARAMS:
         if param not in config_data['aws_batch']:
             msg = f'"{param}" is mandatory in the "aws_batch" section of the configuration'
```

### Comparing `lithops-3.2.0/lithops/serverless/backends/aws_batch/entry_point.py` & `lithops-3.3.0/lithops/serverless/backends/aws_batch/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/aws_lambda/aws_lambda.py` & `lithops-3.3.0/lithops/serverless/backends/aws_lambda/aws_lambda.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,61 +53,52 @@
         logger.debug('Creating AWS Lambda client')
 
         self.name = 'aws_lambda'
         self.type = utils.BackendType.FAAS.value
         self.lambda_config = lambda_config
         self.internal_storage = internal_storage
         self.user_agent = lambda_config['user_agent']
-        self.region_name = lambda_config['region']
+        self.region = lambda_config['region']
         self.role_arn = lambda_config['execution_role']
         self.namespace = lambda_config.get('namespace')
 
-        logger.debug('Creating Boto3 AWS Session and Lambda Client')
-
         self.aws_session = boto3.Session(
-            aws_access_key_id=lambda_config['access_key_id'],
-            aws_secret_access_key=lambda_config['secret_access_key'],
+            aws_access_key_id=lambda_config.get('access_key_id'),
+            aws_secret_access_key=lambda_config.get('secret_access_key'),
             aws_session_token=lambda_config.get('session_token'),
-            region_name=self.region_name
+            region_name=self.region
         )
 
         self.lambda_client = self.aws_session.client(
-            'lambda', region_name=self.region_name,
-            config=botocore.client.Config(
+            'lambda', config=botocore.client.Config(
                 user_agent_extra=self.user_agent
             )
         )
 
         self.credentials = self.aws_session.get_credentials()
         self.session = URLLib3Session()
-        self.host = f'lambda.{self.region_name}.amazonaws.com'
-
-        if 'account_id' in self.lambda_config:
-            self.account_id = self.lambda_config['account_id']
-        else:
-            sts_client = self.aws_session.client('sts', region_name=self.region_name)
-            self.account_id = sts_client.get_caller_identity()["Account"]
+        self.host = f'lambda.{self.region}.amazonaws.com'
 
-        sts_client = self.aws_session.client('sts', region_name=self.region_name)
-        caller_id = sts_client.get_caller_identity()
+        if 'account_id' not in self.lambda_config or 'user_id' not in self.lambda_config:
+            sts_client = self.aws_session.client('sts')
+            identity = sts_client.get_caller_identity()
 
-        if ":" in caller_id["UserId"]:  # SSO user
-            self.user_key = caller_id["UserId"].split(":")[1]
-        else:  # IAM user
-            self.user_key = caller_id["UserId"][-4:].lower()
+        self.account_id = self.lambda_config.get('account_id') or identity["Account"]
+        self.user_id = self.lambda_config.get('user_id') or identity["UserId"]
+        self.user_key = self.user_id.split(":")[0][-4:].lower()
 
-        self.ecr_client = self.aws_session.client('ecr', region_name=self.region_name)
+        self.ecr_client = self.aws_session.client('ecr')
         package = f'lithops_v{__version__.replace(".", "")}_{self.user_key}'
         self.package = f"{package}_{self.namespace}" if self.namespace else package
 
         msg = COMPUTE_CLI_MSG.format('AWS Lambda')
         if self.namespace:
-            logger.info(f"{msg} - Region: {self.region_name} - Namespace: {self.namespace}")
+            logger.info(f"{msg} - Region: {self.region} - Namespace: {self.namespace}")
         else:
-            logger.info(f"{msg} - Region: {self.region_name}")
+            logger.info(f"{msg} - Region: {self.region}")
 
     def _format_function_name(self, runtime_name, runtime_memory, version=__version__):
         name = f'{runtime_name}-{runtime_memory}-{version}'
         name_hash = hashlib.sha1(name.encode("utf-8")).hexdigest()[:10]
         fn_name = f'lithops-worker-{self.user_key}-{version.replace(".", "")}-{name_hash}'
         return f'{self.namespace}-{fn_name}' if self.namespace else fn_name
 
@@ -342,26 +333,26 @@
         @param runtime_file: path of a Dockerfile for a container runtime
         """
         logger.info(f'Building runtime {runtime_name} from {runtime_file}')
 
         docker_path = utils.get_docker_path()
         if runtime_file:
             assert os.path.isfile(runtime_file), f'Cannot locate "{runtime_file}"'
-            cmd = f'{docker_path} build -t {runtime_name} -f {runtime_file} . '
+            cmd = f'{docker_path} build --platform=linux/amd64 -t {runtime_name} -f {runtime_file} . '
         else:
-            cmd = f'{docker_path} build -t {runtime_name} . '
+            cmd = f'{docker_path} build --platform=linux/amd64 -t {runtime_name} . '
         cmd = cmd + ' '.join(extra_args)
 
         try:
             self._create_handler_bin(remove=False)
             utils.run_command(cmd)
         finally:
             os.remove(LITHOPS_FUNCTION_ZIP)
 
-        registry = f'{self.account_id}.dkr.ecr.{self.region_name}.amazonaws.com'
+        registry = f'{self.account_id}.dkr.ecr.{self.region}.amazonaws.com'
 
         res = self.ecr_client.get_authorization_token()
         if res['ResponseMetadata']['HTTPStatusCode'] != 200:
             raise Exception(f'Could not get ECR auth token: {res}')
 
         auth_data = res['authorizationData'].pop()
         ecr_token = base64.b64decode(auth_data['authorizationToken']).split(b':')[1]
@@ -470,15 +461,15 @@
                 raise Exception(f'Runtime {runtime_name} is not present in ECR.'
                                 'Consider running "lithops runtime build -b aws_lambda ..."')
             image = list(filter(lambda image: 'imageTags' in image and tag in image['imageTags'], images)).pop()
             image_digest = image['imageDigest']
         except botocore.exceptions.ClientError:
             raise Exception(f'Runtime "{runtime_name}" is not deployed to ECR')
 
-        registry = f'{self.account_id}.dkr.ecr.{self.region_name}.amazonaws.com'
+        registry = f'{self.account_id}.dkr.ecr.{self.region}.amazonaws.com'
         image_uri = f'{registry}/{repo_name}@{image_digest}'
 
         env_vars = {t['name']: t['value'] for t in self.lambda_config['env_vars']}
 
         try:
             response = self.lambda_client.create_function(
                 FunctionName=function_name,
@@ -606,16 +597,14 @@
         response = self.lambda_client.list_functions(FunctionVersion='ALL')
         get_runtimes(response)
         while 'NextMarker' in response:
             response = self.lambda_client.list_functions(Marker=response['NextMarker'])
             get_runtimes(response)
 
         if runtime_name != 'all':
-            if self._is_container_runtime(runtime_name) and ':' not in runtime_name:
-                runtime_name = runtime_name + ':latest'
             runtimes = [tup for tup in runtimes if runtime_name in tup[0]]
 
         return runtimes
 
     def invoke(self, runtime_name, runtime_memory, payload):
         """
         Invoke lambda function asynchronously
@@ -626,15 +615,15 @@
         """
 
         function_name = self._format_function_name(runtime_name, runtime_memory)
 
         headers = {'Host': self.host, 'X-Amz-Invocation-Type': 'Event', 'User-Agent': self.user_agent}
         url = f'https://{self.host}/2015-03-31/functions/{function_name}/invocations'
         request = AWSRequest(method="POST", url=url, data=json.dumps(payload, default=str), headers=headers)
-        SigV4Auth(self.credentials, "lambda", self.region_name).add_auth(request)
+        SigV4Auth(self.credentials, "lambda", self.region).add_auth(request)
 
         invoked = False
         while not invoked:
             try:
                 r = self.session.send(request.prepare())
                 invoked = True
             except Exception:
@@ -672,15 +661,15 @@
     def get_runtime_key(self, runtime_name, runtime_memory, version=__version__):
         """
         Method that creates and returns the runtime key.
         Runtime keys are used to uniquely identify runtimes within the storage,
         in order to know which runtimes are installed and which not.
         """
         action_name = self._format_function_name(runtime_name, runtime_memory, version)
-        runtime_key = os.path.join(self.name, version, self.region_name, action_name)
+        runtime_key = os.path.join(self.name, version, self.region, action_name)
 
         return runtime_key
 
     def get_runtime_info(self):
         """
         Method that returns all the relevant information about the runtime set
         in config
```

### Comparing `lithops-3.2.0/lithops/serverless/backends/aws_lambda/build_layer.py` & `lithops-3.3.0/lithops/serverless/backends/aws_lambda/build_layer.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/aws_lambda/config.py` & `lithops-3.3.0/lithops/serverless/backends/aws_lambda/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,23 +63,21 @@
 RUNTIME_MEMORY_MAX = 10240  # Max. memory: 10240 MB
 
 RUNTIME_TMP_SZ_MIN = 512
 RUNTIME_TMP_SZ_MAX = 10240
 
 
 def load_config(config_data):
-    if 'aws' not in config_data:
-        raise Exception("'aws' section is mandatory in the configuration")
-
-    if not {'access_key_id', 'secret_access_key'}.issubset(set(config_data['aws'])):
-        raise Exception("'access_key_id' and 'secret_access_key' are mandatory under the 'aws' section of the configuration")
 
     if not config_data['aws_lambda']:
         raise Exception("'aws_lambda' section is mandatory in the configuration")
 
+    if 'aws' not in config_data:
+        config_data['aws'] = {}
+
     temp = copy.deepcopy(config_data['aws_lambda'])
     config_data['aws_lambda'].update(config_data['aws'])
     config_data['aws_lambda'].update(temp)
 
     for param in REQ_PARAMS:
         if param not in config_data['aws_lambda']:
             msg = f'"{param}" is mandatory in the "aws_lambda" section of the configuration'
```

### Comparing `lithops-3.2.0/lithops/serverless/backends/aws_lambda/entry_point.py` & `lithops-3.3.0/lithops/serverless/backends/aws_lambda/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/azure_containers/azure_containers.py` & `lithops-3.3.0/lithops/serverless/backends/azure_containers/azure_containers.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,27 +111,37 @@
         """
         logger.info(f'Building runtime {runtime_name} from {dockerfile or "Dockerfile"}')
 
         docker_path = utils.get_docker_path()
 
         if dockerfile:
             assert os.path.isfile(dockerfile), f'Cannot locate "{dockerfile}"'
-            cmd = f'{docker_path} build -t {runtime_name} -f {dockerfile} . '
+            cmd = f'{docker_path} build --platform=linux/amd64 -t {runtime_name} -f {dockerfile} . '
         else:
-            cmd = f'{docker_path} build -t {runtime_name} . '
+            cmd = f'{docker_path} build --platform=linux/amd64 -t {runtime_name} . '
         cmd = cmd + ' '.join(extra_args)
 
         try:
             entry_point = os.path.join(os.path.dirname(__file__), 'entry_point.py')
             utils.create_handler_zip(config.FH_ZIP_LOCATION, entry_point, 'lithopsentry.py')
             utils.run_command(cmd)
         finally:
             os.remove(config.FH_ZIP_LOCATION)
 
+        docker_user = self.ac_config.get("docker_user")
+        docker_password = self.ac_config.get("docker_password")
+        docker_server = self.ac_config.get("docker_server")
+
         logger.debug(f'Pushing runtime {runtime_name} to container registry')
+
+        if docker_user and docker_password:
+            logger.debug('Container registry credentials found in config. Logging in into the registry')
+            cmd = f'{docker_path} login -u {docker_user} --password-stdin {docker_server}'
+            utils.run_command(cmd, input=docker_password)
+
         if utils.is_podman(docker_path):
             cmd = f'{docker_path} push {runtime_name} --format docker --remove-signatures'
         else:
             cmd = f'{docker_path} push {runtime_name}'
         utils.run_command(cmd)
 
         logger.debug(f'Runtime {runtime_name} built successfully')
@@ -168,15 +178,15 @@
                             f'one of thses memory values: {config.ALLOWED_MEM.keys()}')
 
         ca_temaplate['properties']['template']['containers'][0]['image'] = runtime_name
         ca_temaplate['properties']['template']['containers'][0]['env'][0]['value'] = containerapp_name
         ca_temaplate['properties']['template']['scale']['rules'][0]['azureQueue']['queueName'] = containerapp_name
         ca_temaplate['properties']['template']['scale']['maxReplicas'] = min(self.ac_config['max_workers'], 30)
 
-        cmd = f"az containerapp env show -g {self.resource_group} -n {self.environment} --query id"
+        cmd = f"az containerapp env show -g {self.resource_group} -n {self.environment} --query id --only-show-errors"
         envorinemnt_id = utils.run_command(cmd, return_result=True)
         ca_temaplate['properties']['managedEnvironmentId'] = envorinemnt_id
 
         cmd = f"az storage account show-connection-string -g {self.resource_group} --name {self.storage_account_name} --query connectionString --out json"
         queueconnection = utils.run_command(cmd, return_result=True)
         ca_temaplate['properties']['configuration']['secrets'][0]['value'] = queueconnection
 
@@ -189,40 +199,40 @@
             del ca_temaplate['properties']['configuration']['registries']
 
         with open(config.CA_JSON_LOCATION, 'w') as f:
             f.write(json.dumps(ca_temaplate))
 
         cmd = (f'az containerapp create --name {containerapp_name} '
                f'--resource-group {self.resource_group} '
-               f'--yaml {config.CA_JSON_LOCATION}')
+               f'--yaml {config.CA_JSON_LOCATION} --only-show-errors')
 
         logger.debug('Deploying Azure Container App')
         deployed = False
         retries = 0
 
-        while retries < 15:
+        while retries < 10:
             try:
-                time.sleep(20)
                 utils.run_command(cmd)
                 os.remove(config.CA_JSON_LOCATION)
                 deployed = True
                 break
             except Exception:
+                time.sleep(10)
                 retries += 1
 
         if not deployed:
             raise Exception(f"The Azure Container App cannot be deployed: {cmd}")
 
     def delete_runtime(self, runtime_name, memory, version=__version__):
         """
         Deletes a runtime
         """
         logger.info(f'Deleting runtime: {runtime_name} - {memory}MB')
         containerapp_name = self._format_containerapp_name(runtime_name, memory, version)
-        cmd = f'az containerapp delete --name {containerapp_name} --resource-group {self.resource_group} -y'
+        cmd = f'az containerapp delete --name {containerapp_name} --resource-group {self.resource_group} -y --only-show-errors'
         utils.run_command(cmd)
 
         try:
             self.queue_service.delete_queue(containerapp_name)
         except Exception:
             pass
 
@@ -296,15 +306,15 @@
     def list_runtimes(self, runtime_name='all'):
         """
         List all the Azure Function Apps deployed.
         """
         logger.debug('Listing all deployed runtimes')
 
         runtimes = []
-        response = os.popen('az containerapp list --query "[].{Name:name, Tags:tags}\"').read()
+        response = os.popen('az containerapp list --query "[].{Name:name, Tags:tags}\" --only-show-errors').read()
         response = json.loads(response)
 
         for containerapp in response:
             if containerapp['Tags'] and 'type' in containerapp['Tags'] \
                and containerapp['Tags']['type'] == 'lithops-runtime':
                 name = containerapp['Tags']['runtime_name']
                 memory = containerapp['Tags']['runtime_memory']
```

### Comparing `lithops-3.2.0/lithops/serverless/backends/azure_containers/config.py` & `lithops-3.3.0/lithops/serverless/backends/azure_containers/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/azure_containers/entry_point.py` & `lithops-3.3.0/lithops/serverless/backends/azure_containers/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/azure_functions/azure_functions.py` & `lithops-3.3.0/lithops/serverless/backends/azure_functions/azure_functions.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/azure_functions/config.py` & `lithops-3.3.0/lithops/serverless/backends/azure_functions/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/azure_functions/entry_point.py` & `lithops-3.3.0/lithops/serverless/backends/azure_functions/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/code_engine/code_engine.py` & `lithops-3.3.0/lithops/serverless/backends/code_engine/code_engine.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/code_engine/config.py` & `lithops-3.3.0/lithops/serverless/backends/code_engine/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/code_engine/entry_point.py` & `lithops-3.3.0/lithops/serverless/backends/code_engine/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/gcp_cloudrun/cloudrun.py` & `lithops-3.3.0/lithops/serverless/backends/gcp_cloudrun/cloudrun.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,17 +213,17 @@
 
         docker_path = utils.get_docker_path()
 
         image_name = self._format_image_name(runtime_name)
 
         if dockerfile:
             assert os.path.isfile(dockerfile), f'Cannot locate "{dockerfile}"'
-            cmd = f'{docker_path} build -t {image_name} -f {dockerfile} . '
+            cmd = f'{docker_path} build --platform=linux/amd64 -t {image_name} -f {dockerfile} . '
         else:
-            cmd = f'{docker_path} build -t {image_name} . '
+            cmd = f'{docker_path} build --platform=linux/amd64 -t {image_name} . '
         cmd = cmd + ' '.join(extra_args)
 
         try:
             entry_point = os.path.join(os.path.dirname(__file__), 'entry_point.py')
             utils.create_handler_zip(config.FH_ZIP_LOCATION, entry_point, 'lithopsproxy.py')
             utils.run_command(cmd)
         finally:
```

### Comparing `lithops-3.2.0/lithops/serverless/backends/gcp_cloudrun/config.py` & `lithops-3.3.0/lithops/serverless/backends/gcp_cloudrun/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/gcp_cloudrun/entry_point.py` & `lithops-3.3.0/lithops/serverless/backends/gcp_cloudrun/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/gcp_functions/config.py` & `lithops-3.3.0/lithops/serverless/backends/gcp_functions/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/gcp_functions/entry_point.py` & `lithops-3.3.0/lithops/serverless/backends/gcp_functions/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/gcp_functions/gcp_functions.py` & `lithops-3.3.0/lithops/serverless/backends/gcp_functions/gcp_functions.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/ibm_cf/config.py` & `lithops-3.3.0/lithops/serverless/backends/ibm_cf/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/ibm_cf/entry_point.py` & `lithops-3.3.0/lithops/serverless/backends/ibm_cf/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/ibm_cf/ibm_cf.py` & `lithops-3.3.0/lithops/serverless/backends/ibm_cf/ibm_cf.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 
         if self.namespace_id:
             return self.namespace_id
 
         response = self.cf_client.list_namespaces(self.resource_group_id)
         if 'namespaces' in response:
             for namespace in response['namespaces']:
-                if namespace['name'] == self.namespace_name:
+                if 'name' in namespace and namespace['name'] == self.namespace_name:
                     logger.debug(f"Found Cloud Functions namespace: {self.namespace_name}")
                     self.namespace_id = namespace['id']
                     self.config['namespace_id'] = self.namespace_id
 
         if not self.namespace_id and create:
             logger.debug(f"Creating new Cloud Functions namespace: {self.namespace_name}")
             self.namespace_id = self.cf_client.create_namespace(
```

### Comparing `lithops-3.2.0/lithops/serverless/backends/k8s/config.py` & `lithops-3.3.0/lithops/serverless/backends/k8s/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/k8s/entry_point.py` & `lithops-3.3.0/lithops/serverless/backends/k8s/entry_point.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import json
 import logging
 import flask
 import time
 import requests
 from functools import partial
 from multiprocessing import Value
+from threading import Thread
 
 from lithops.version import __version__
 from lithops.utils import setup_lithops_logger, b64str_to_dict
 from lithops.worker import function_handler
 from lithops.worker.utils import get_runtime_metadata
 from lithops.constants import JOBS_PREFIX
 from lithops.storage.storage import InternalStorage
@@ -117,42 +118,45 @@
         payload['call_ids'] = call_ids[start:end]
         payload['data_byte_ranges'] = dbr
         function_handler(payload)
 
     logger.info("Finishing kubernetes execution")
 
 
-def run_job_k8s_rabbitmq(payload, running_jobs):
+def run_job_k8s_rabbitmq(payload):
     logger.info(f"Lithops v{__version__} - Starting kubernetes execution")
 
     act_id = str(uuid.uuid4()).replace('-', '')[:12]
     os.environ['__LITHOPS_ACTIVATION_ID'] = act_id
     os.environ['__LITHOPS_BACKEND'] = 'k8s_rabbitmq'
 
     function_handler(payload)
-    running_jobs.value += len(payload['call_ids'])
+    with running_jobs.get_lock():
+        running_jobs.value += len(payload['call_ids'])
 
     logger.info("Finishing kubernetes execution")
 
 
 def callback_work_queue(ch, method, properties, body):
     """Callback to receive the payload and run the jobs"""
-    global cpus_pod
-
     logger.info("Call from lithops received.")
 
     message = json.loads(body)
     tasks = message['total_calls']
 
-    running_jobs = Value('i', cpus_pod)  # Shared variable to track completed jobs
-
     # If there are more tasks than cpus in the pod, we need to send a new message
     if tasks <= running_jobs.value:
         processes_to_start = tasks
     else:
+        if running_jobs.value == 0:
+            logger.info("All cpus are busy. Waiting for a cpu to be free")
+            ch.basic_nack(delivery_tag=method.delivery_tag)
+            time.sleep(0.5)
+            return
+
         processes_to_start = running_jobs.value
 
         message_to_send = message.copy()
         message_to_send['total_calls'] = tasks - running_jobs.value
         message_to_send['call_ids'] = message_to_send['call_ids'][running_jobs.value:]
         message_to_send['data_byte_ranges'] = message_to_send['data_byte_ranges'][running_jobs.value:]
 
@@ -167,33 +171,34 @@
             properties=pika.BasicProperties(
                 delivery_mode=pika.spec.PERSISTENT_DELIVERY_MODE
             ))
 
     logger.info(f"Starting {processes_to_start} processes")
 
     message['worker_processes'] = running_jobs.value
-    running_jobs.value -= processes_to_start
-    run_job_k8s_rabbitmq(message, running_jobs)
+    with running_jobs.get_lock():
+        running_jobs.value -= processes_to_start
+
+    Thread(target=run_job_k8s_rabbitmq, args=([message])).start()
 
-    logger.info("All processes completed")
     ch.basic_ack(delivery_tag=method.delivery_tag)
 
 
 def start_rabbitmq_listening(payload):
-    global cpus_pod
+    global running_jobs
 
     # Connect to rabbitmq
     params = pika.URLParameters(payload['amqp_url'])
     connection = pika.BlockingConnection(params)
     channel = connection.channel()
     channel.queue_declare(queue='task_queue', durable=True)
     channel.basic_qos(prefetch_count=1)
 
-    # Get the number of cpus of the pod
-    cpus_pod = payload['cpus_pod']
+    # Shared variable to track completed jobs
+    running_jobs = Value('i', payload['cpus_pod'])
 
     # Start listening to the new job
     channel.basic_consume(queue='task_queue', on_message_callback=callback_work_queue)
 
     logger.info("Listening to rabbitmq...")
     channel.start_consuming()
```

### Comparing `lithops-3.2.0/lithops/serverless/backends/k8s/k8s.py` & `lithops-3.3.0/lithops/serverless/backends/k8s/k8s.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,17 +130,17 @@
         """
         logger.info(f'Building runtime {docker_image_name} from {dockerfile or "Dockerfile"}')
 
         docker_path = utils.get_docker_path()
 
         if dockerfile:
             assert os.path.isfile(dockerfile), f'Cannot locate "{dockerfile}"'
-            cmd = f'{docker_path} build -t {docker_image_name} -f {dockerfile} . '
+            cmd = f'{docker_path} build --platform=linux/amd64 -t {docker_image_name} -f {dockerfile} . '
         else:
-            cmd = f'{docker_path} build -t {docker_image_name} . '
+            cmd = f'{docker_path} build --platform=linux/amd64 -t {docker_image_name} . '
         cmd = cmd + ' '.join(extra_args)
 
         try:
             entry_point = os.path.join(os.path.dirname(__file__), 'entry_point.py')
             utils.create_handler_zip(config.FH_ZIP_LOCATION, entry_point, 'lithopsentry.py')
             utils.run_command(cmd)
         finally:
@@ -363,42 +363,49 @@
     def _create_workers(self, runtime_memory):
         default_pod_config = yaml.load(config.POD, Loader=yaml.loader.SafeLoader)
         granularity = self.k8s_config['worker_processes']
         cluster_info_cpu = {}
         cluster_info_mem = {}
         num_cpus_cluster = 0
 
+        # If the unit is not specified, assume it is in MB
+        try:
+            mem_num, mem_uni = re.match(r'(\d+)(\D*)', runtime_memory).groups()
+        except TypeError:
+            mem_num = runtime_memory
+            mem_uni = 'M'
+
         if granularity <= 1:
             granularity = False
 
         for node in self.nodes:
             cpus_node = int(float(node["cpu"]) * 0.9)
 
             if granularity:
                 times, res = divmod(cpus_node, granularity)
 
                 for i in range(times):
                     cluster_info_cpu[f"{node['name']}-{i}"] = granularity
-                    cluster_info_mem[f"{node['name']}-{i}"] = runtime_memory
+                    cluster_info_mem[f"{node['name']}-{i}"] = f"{mem_num}{mem_uni}"
                     num_cpus_cluster += granularity
                 if res != 0:
                     cluster_info_cpu[f"{node['name']}-{times}"] = res
-                    cluster_info_mem[f"{node['name']}-{times}"] = runtime_memory
+                    cluster_info_mem[f"{node['name']}-{times}"] = f"{mem_num}{mem_uni}"
                     num_cpus_cluster += res
             else:
                 cluster_info_cpu[node["name"] + "-0"] = cpus_node
                 num_cpus_cluster += cpus_node
 
                 # If runtime_memory is not defined in the config, use 80% of the node memory
                 if runtime_memory == 512:
                     mem_num, mem_uni = re.match(r'(\d+)(\D*)', node["memory"]).groups()
                     mem_num = int(float(mem_num) * 0.8)
                     cluster_info_mem[node["name"] + "-0"] = f"{mem_num}{mem_uni}"
                 else:
-                    cluster_info_mem[node["name"] + "-0"] = str(runtime_memory)
+                    cluster_info_mem[node["name"] + "-0"] = f"{mem_num}{mem_uni}"
 
         if num_cpus_cluster == 0:
             raise ValueError("Total CPUs of the cluster cannot be 0")
 
         # Create all the pods
         for pod_name in cluster_info_cpu.keys():
             self._create_pod(default_pod_config, pod_name, cluster_info_cpu[pod_name], cluster_info_mem[pod_name])
@@ -469,14 +476,27 @@
         for event in w.stream(self.core_api.list_namespaced_pod,
                               namespace=self.namespace,
                               label_selector=f"job-name={self.master_name}"):
             if event['object'].status.phase == "Running":
                 w.stop()
                 return event['object'].status.pod_ip
 
+    def convert_memory_units(self, mem_num, mem_uni):
+        mem_num = int(mem_num)
+
+        if 'i' in mem_uni:
+            mem_num *= 1024
+            mem_uni = mem_uni[:-1]
+        if 'K' in mem_uni:
+            mem_num = mem_num / (1024 if 'i' in mem_uni else 1000)
+        elif 'G' in mem_uni:
+            mem_num = mem_num * (1024 if 'i' in mem_uni else 1000)
+
+        return mem_num, 'M'
+
     # Detect if granularity, memory or runtime image changed or not
     def _has_config_changed(self, runtime_mem):
         config_granularity = False if self.k8s_config['worker_processes'] <= 1 else self.k8s_config['worker_processes']
         config_memory = self.k8s_config['runtime_memory'] if self.k8s_config['runtime_memory'] != 512 else False
 
         self.current_runtime = ""
 
@@ -497,32 +517,42 @@
 
             multiples_pods_per_node = re.search(r'-\d+(?<!-0)$', pod_name)
 
             node_cpu = int(float(node_info["cpu"]) * 0.9)
             node_mem_num, node_mem_uni = re.match(r'(\d+)(\D*)', node_info["memory"]).groups()
             pod_mem_num, pod_mem_uni = re.match(r'(\d+)(\D*)', pod_resource_memory).groups()
 
-            pod_mem_num = int(pod_mem_num)
             node_mem_num = int(float(node_mem_num) * 0.8)
 
+            # Match the same unit of runtime memory and pod memory
+            try:
+                config_mem_num, config_mem_uni = re.match(r'(\d+)(\D*)', config_memory).groups()
+                config_mem_num, config_mem_uni = self.convert_memory_units(config_mem_num, config_mem_uni)
+            except TypeError:
+                config_mem_num = config_memory
+                config_mem_uni = 'M'
+
+            pod_mem_num, pod_mem_uni = self.convert_memory_units(pod_mem_num, pod_mem_uni)
+            node_mem_num, node_mem_uni = self.convert_memory_units(node_mem_num, node_mem_uni)
+
             # There are pods with cpu granularity
             if multiples_pods_per_node:
                 # Is lithops pod with granularity and the user doesn't want it
                 if not config_granularity:
                     return True
                 # There is granularity but the pod doesn't have the default memory
                 if not config_memory and pod_mem_num != runtime_mem:
                     return True
                 # There is granularity but the pod doesn't have the desired memory
-                if config_memory and pod_mem_num != config_memory:
+                if config_memory and pod_mem_num != config_mem_num:
                     return True
             else:
                 # There is a custom memory but the pod doesn't have the desired memory
                 if config_memory:
-                    if pod_mem_num != config_memory:
+                    if pod_mem_num != config_mem_num:
                         return True
                 # The pod has custom_memory and the user doesn't want it
                 else:
                     if pod_mem_num != node_mem_num and pod_mem_num != runtime_mem:
                         return True
 
             # The cpu granularity changed
```

### Comparing `lithops-3.2.0/lithops/serverless/backends/knative/config.py` & `lithops-3.3.0/lithops/serverless/backends/knative/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/knative/entry_point.py` & `lithops-3.3.0/lithops/serverless/backends/knative/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/knative/knative.py` & `lithops-3.3.0/lithops/serverless/backends/knative/knative.py`

 * *Files 1% similar despite different names*

```diff
@@ -556,17 +556,17 @@
         """
         logger.info(f'Building runtime {runtime_name} from {dockerfile or "Dockerfile"}')
 
         docker_path = utils.get_docker_path()
 
         if dockerfile:
             assert os.path.isfile(dockerfile), f'Cannot locate "{dockerfile}"'
-            cmd = f'{docker_path} build -t {runtime_name} -f {dockerfile} . '
+            cmd = f'{docker_path} build --platform=linux/amd64 -t {runtime_name} -f {dockerfile} . '
         else:
-            cmd = f'{docker_path} build -t {runtime_name} . '
+            cmd = f'{docker_path} build --platform=linux/amd64 -t {runtime_name} . '
         cmd = cmd + ' '.join(extra_args)
 
         try:
             entry_point = os.path.join(os.path.dirname(__file__), 'entry_point.py')
             utils.create_handler_zip(config.FH_ZIP_LOCATION, entry_point, 'lithopsproxy.py')
             utils.run_command(cmd)
         finally:
```

### Comparing `lithops-3.2.0/lithops/serverless/backends/openwhisk/config.py` & `lithops-3.3.0/lithops/serverless/backends/openwhisk/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/openwhisk/entry_point.py` & `lithops-3.3.0/lithops/serverless/backends/openwhisk/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/openwhisk/openwhisk.py` & `lithops-3.3.0/lithops/serverless/backends/openwhisk/openwhisk.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/oracle_f/config.py` & `lithops-3.3.0/lithops/serverless/backends/oracle_f/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/oracle_f/entry_point.py` & `lithops-3.3.0/lithops/serverless/backends/oracle_f/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/serverless/backends/oracle_f/oracle_f.py` & `lithops-3.3.0/lithops/serverless/backends/oracle_f/oracle_f.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,17 +196,17 @@
 
         logger.info(f'Building runtime {image_name} from {dockerfile}')
         docker_path = utils.get_docker_path()
 
         # Build the Docker image
         if dockerfile:
             assert os.path.isfile(dockerfile), f'Cannot locate "{dockerfile}"'
-            cmd = f'{docker_path} build -t {image_name} -f {dockerfile} . '
+            cmd = f'{docker_path} build --platform=linux/amd64 -t {image_name} -f {dockerfile} . '
         else:
-            cmd = f'{docker_path} build -t {image_name} . '
+            cmd = f'{docker_path} build --platform=linux/amd64 -t {image_name} . '
         cmd = cmd + ' '.join(extra_args)
 
         try:
             entry_point = os.path.join(os.path.dirname(__file__), 'entry_point.py')
             utils.create_handler_zip(config.FH_ZIP_LOCATION, entry_point, 'entry_point.py')
             utils.run_command(cmd)
         finally:
```

### Comparing `lithops-3.2.0/lithops/serverless/serverless.py` & `lithops-3.3.0/lithops/serverless/serverless.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/standalone/backends/aws_ec2/aws_ec2.py` & `lithops-3.3.0/lithops/standalone/backends/aws_ec2/aws_ec2.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,21 +16,20 @@
 
 import os
 import re
 import time
 import uuid
 import logging
 import base64
+import boto3
+import botocore
 from botocore.exceptions import ClientError
 from datetime import datetime
 from concurrent.futures import ThreadPoolExecutor
 
-import boto3
-import botocore
-
 from lithops.version import __version__
 from lithops.util.ssh_client import SSHClient
 from lithops.constants import COMPUTE_CLI_MSG, CACHE_DIR
 from lithops.config import load_yaml_config, dump_yaml_config
 from lithops.standalone.utils import CLOUD_CONFIG_WORKER, CLOUD_CONFIG_WORKER_PK, StandaloneMode, get_host_setup_script
 from lithops.standalone import LithopsValidationError
 
@@ -51,47 +50,54 @@
     Base-64 encode a string and return a string
     """
     return base64.b64encode(string.encode('utf-8')).decode('ascii')
 
 
 class AWSEC2Backend:
 
-    def __init__(self, config, mode):
+    def __init__(self, ec2_config, mode):
         logger.debug("Creating AWS EC2 client")
         self.name = 'aws_ec2'
-        self.config = config
+        self.config = ec2_config
         self.mode = mode
         self.region_name = self.config['region']
 
         suffix = 'vm' if self.mode == StandaloneMode.CONSUME.value else 'vpc'
         self.cache_dir = os.path.join(CACHE_DIR, self.name)
         self.cache_file = os.path.join(self.cache_dir, f'{self.region_name}_{suffix}_data')
 
         self.vpc_data_type = 'provided' if 'vpc_id' in self.config else 'created'
         self.ssh_data_type = 'provided' if 'ssh_key_name' in self.config else 'created'
 
         self.ec2_data = {}
         self.vpc_name = None
         self.vpc_key = None
-        self.user_key = self.config['access_key_id'][-4:].lower()
 
         self.instance_types = {}
 
-        client_config = botocore.client.Config(
-            user_agent_extra=self.config['user_agent']
+        self.aws_session = boto3.Session(
+            aws_access_key_id=ec2_config.get('access_key_id'),
+            aws_secret_access_key=ec2_config.get('secret_access_key'),
+            aws_session_token=ec2_config.get('session_token'),
+            region_name=self.region_name
         )
 
-        self.ec2_client = boto3.client(
-            'ec2', aws_access_key_id=self.config['access_key_id'],
-            aws_secret_access_key=self.config['secret_access_key'],
-            aws_session_token=self.config.get('session_token'),
-            config=client_config,
-            region_name=self.region_name
+        self.ec2_client = self.aws_session.client(
+            'ec2', config=botocore.client.Config(
+                user_agent_extra=self.config['user_agent']
+            )
         )
 
+        if 'user_id' not in self.config:
+            sts_client = self.aws_session.client('sts')
+            identity = sts_client.get_caller_identity()
+
+        self.user_id = self.config.get('user_id') or identity["UserId"]
+        self.user_key = self.user_id.split(":")[0][-4:].lower()
+
         self.master = None
         self.workers = []
 
         msg = COMPUTE_CLI_MSG.format('AWS EC2')
         logger.info(f"{msg} - Region: {self.region_name}")
 
     def is_initialized(self):
```

### Comparing `lithops-3.2.0/lithops/standalone/backends/aws_ec2/config.py` & `lithops-3.3.0/lithops/standalone/backends/aws_ec2/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,32 +23,30 @@
     'master_instance_type': 't2.micro',
     'worker_instance_type': 't2.medium',
     'ssh_username': 'ubuntu',
     'ssh_password': str(uuid.uuid4()),
     'ssh_key_filename': '~/.ssh/id_rsa',
     'request_spot_instances': True,
     'delete_on_dismantle': True,
-    'max_workers': 100
+    'max_workers': 100,
+    'worker_processes': 'AUTO'
 }
 
 REQ_PARAMS_1 = ('instance_id',)
 REQ_PARAMS_2 = ('iam_role',)
 
 
 def load_config(config_data):
 
-    if 'aws' not in config_data:
-        raise Exception("'aws' section is mandatory in the configuration")
-
-    if not {'access_key_id', 'secret_access_key'}.issubset(set(config_data['aws'])):
-        raise Exception("'access_key_id' and 'secret_access_key' are mandatory under the 'aws' section of the configuration")
-
     if not config_data['aws_ec2']:
         raise Exception("'aws_ec2' section is mandatory in the configuration")
 
+    if 'aws' not in config_data:
+        config_data['aws'] = {}
+
     temp = copy.deepcopy(config_data['aws_ec2'])
     config_data['aws_ec2'].update(config_data['aws'])
     config_data['aws_ec2'].update(temp)
 
     for key in DEFAULT_CONFIG_KEYS:
         if key not in config_data['aws_ec2']:
             config_data['aws_ec2'][key] = DEFAULT_CONFIG_KEYS[key]
@@ -64,17 +62,14 @@
 
     if config_data['standalone']['exec_mode'] == 'consume':
         params_to_check = REQ_PARAMS_1
         config_data['aws_ec2']['max_workers'] = 1
     else:
         params_to_check = REQ_PARAMS_2
 
-    if "worker_processes" not in config_data['aws_ec2']:
-        config_data['aws_ec2']['worker_processes'] = "AUTO"
-
     for param in params_to_check:
         if param not in config_data['aws_ec2']:
             msg = f"'{param}' is mandatory in the 'aws_ec2' section of the configuration"
             raise Exception(msg)
 
     if 'region_name' in config_data['aws_ec2']:
         config_data['aws_ec2']['region'] = config_data['aws_ec2'].pop('region_name')
```

### Comparing `lithops-3.2.0/lithops/standalone/backends/azure_vms/azure_vms.py` & `lithops-3.3.0/lithops/standalone/backends/azure_vms/azure_vms.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,30 +222,65 @@
             )
             self.config['security_group_id'] = sg_info.id
             self.config['security_group_name'] = sg_info.name
         except ResourceNotFoundError:
             pass
 
         if 'security_group_id' not in self.config:
-            nsg_rule = {
-                "name": "allow-ssh",
-                "protocol": "Tcp",
-                "sourcePortRange": "*",
-                "destinationPortRange": "22",
-                "sourceAddressPrefix": "*",
-                "destinationAddressPrefix": "*",
-                "access": "Allow",
-                "direction": "Inbound",
-                "priority": 100
-            }
+            nsg_rules = [
+                {
+                    "name": "allow-ssh",
+                    "protocol": "Tcp",
+                    "sourcePortRange": "*",
+                    "destinationPortRange": "22",
+                    "sourceAddressPrefix": "*",
+                    "destinationAddressPrefix": "*",
+                    "access": "Allow",
+                    "direction": "Inbound",
+                    "priority": 100
+                },
+                {
+                    "name": "allow-master-port-8080",
+                    "protocol": "Tcp",
+                    "sourcePortRange": "*",
+                    "destinationPortRange": "8080",
+                    "sourceAddressPrefix": "10.0.0.0/24",
+                    "destinationAddressPrefix": "*",
+                    "access": "Allow",
+                    "direction": "Inbound",
+                    "priority": 101
+                },
+                {
+                    "name": "allow-worker-port-8081",
+                    "protocol": "Tcp",
+                    "sourcePortRange": "*",
+                    "destinationPortRange": "8081",
+                    "sourceAddressPrefix": "10.0.0.0/24",
+                    "destinationAddressPrefix": "*",
+                    "access": "Allow",
+                    "direction": "Inbound",
+                    "priority": 102
+                },
+                {
+                    "name": "allow-redis-port-6379",
+                    "protocol": "Tcp",
+                    "sourcePortRange": "*",
+                    "destinationPortRange": "6379",
+                    "sourceAddressPrefix": "10.0.0.0/24",
+                    "destinationAddressPrefix": "*",
+                    "access": "Allow",
+                    "direction": "Inbound",
+                    "priority": 103
+                }
+            ]
 
             # Define the network security group to contain the rule
             network_security_group = {
                 "location": self.location,
-                "securityRules": [nsg_rule]
+                "securityRules": nsg_rules
             }
 
             # Create or update the network security group
             poller = self.network_client.network_security_groups.begin_create_or_update(
                 self.config['resource_group'],
                 security_group_name,
                 network_security_group
@@ -853,14 +888,17 @@
 
         poller = self.compute_client.virtual_machines.begin_create_or_update(
             self.config['resource_group'],
             self.name,
             vm_parameters
         )
 
+        self.instance_data = poller.result()
+        self.instance_id = self.instance_data.vm_id
+
         return self.instance_data
 
     def get_instance_data(self):
         """
         Returns the instance information
         """
         if self.instance_data:
@@ -965,16 +1003,14 @@
         """
         Deletes the VM instance and the associated volume
         """
         logger.debug(f"Deleting VM instance {self.name}")
 
         self.get_instance_data()
 
-        logger.debug(f"Going to delete VM instance {self.name}")
-
         poller = self.compute_client.virtual_machines.begin_delete(
             self.config['resource_group'], self.name, force_deletion=True
         )
         poller.result()
 
         nic_name = self.instance_data.network_profile.network_interfaces[0].id.split('/')[-1]
         poller = self.network_client.network_interfaces.begin_delete(
```

### Comparing `lithops-3.2.0/lithops/standalone/backends/azure_vms/config.py` & `lithops-3.3.0/lithops/standalone/backends/azure_vms/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 DEFAULT_CONFIG_KEYS = {
     'master_instance_type': 'Standard_B1s',
     'worker_instance_type': 'Standard_B2s',
     'ssh_username': 'ubuntu',
     'ssh_password': str(uuid.uuid4()),
     'request_spot_instances': True,
     'delete_on_dismantle': False,
-    'max_workers': 100
+    'max_workers': 100,
+    'worker_processes': 'AUTO'
 }
 
 REQ_PARAMS_1 = ('resource_group', 'subscription_id', 'region')
 REQ_PARAMS_2 = ('instance_name',)
 
 
 def load_config(config_data):
@@ -66,10 +67,7 @@
 
     if config_data['standalone']['exec_mode'] == 'consume':
         config_data['azure_vms']['max_workers'] = 1
         for param in REQ_PARAMS_2:
             if param not in config_data['azure_vms']:
                 msg = f"'{param}' is mandatory in the 'azure_vms' section of the configuration"
                 raise Exception(msg)
-
-    if "worker_processes" not in config_data['azure_vms']:
-        config_data['azure_vms']['worker_processes'] = "AUTO"
```

### Comparing `lithops-3.2.0/lithops/standalone/backends/ibm_vpc/config.py` & `lithops-3.3.0/lithops/standalone/backends/ibm_vpc/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,16 @@
     'boot_volume_profile': 'general-purpose',
     'ssh_username': 'root',
     'ssh_password': str(uuid.uuid4()),
     'ssh_key_filename': '~/.ssh/id_rsa',
     'delete_on_dismantle': True,
     'verify_resources': True,
     'max_workers': 100,
-    'boot_volume_capacity': 100
+    'boot_volume_capacity': 100,
+    'worker_processes': 'AUTO'
 }
 
 VPC_ENDPOINT = "https://{}.iaas.cloud.ibm.com"
 
 REGIONS = ["jp-tok", "jp-osa", "au-syd", "eu-gb", "eu-de", "eu-es", "us-south", "us-east", "br-sao", "ca-tor"]
 
 
@@ -67,17 +68,14 @@
 
     if config_data['standalone']['exec_mode'] == 'consume':
         params_to_check = MANDATORY_PARAMETERS_1
         config_data['ibm_vpc']['max_workers'] = 1
     else:
         params_to_check = MANDATORY_PARAMETERS_2
 
-    if "worker_processes" not in config_data['ibm_vpc']:
-        config_data['ibm_vpc']['worker_processes'] = "AUTO"
-
     for param in params_to_check:
         if param not in config_data['ibm_vpc']:
             msg = f"'{param}' is mandatory in 'ibm_vpc' section of the configuration"
             raise Exception(msg)
 
     if "region" not in config_data['ibm_vpc'] and "endpoint" not in config_data['ibm_vpc']:
         msg = "'region' or 'endpoint' parameter is mandatory in 'ibm_vpc' section of the configuration"
```

### Comparing `lithops-3.2.0/lithops/standalone/backends/ibm_vpc/ibm_vpc.py` & `lithops-3.3.0/lithops/standalone/backends/ibm_vpc/ibm_vpc.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/standalone/backends/vm/config.py` & `lithops-3.3.0/lithops/standalone/backends/vm/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/standalone/backends/vm/vm.py` & `lithops-3.3.0/lithops/standalone/backends/vm/vm.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/standalone/keeper.py` & `lithops-3.3.0/lithops/standalone/keeper.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/standalone/master.py` & `lithops-3.3.0/lithops/standalone/master.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
     instance_type = 'unknow' if config['exec_mode'] == StandaloneMode.CONSUME.value \
         else worker.instance_type
 
     redis_client.hset(f"worker:{worker.name}", mapping={
         'name': worker.name,
         'status': WorkerStatus.STARTING.value,
         'private_ip': worker.private_ip or '',
-        'instance_id': worker.instance_id,
+        'instance_id': worker.instance_id or '',
         'instance_type': instance_type,
         'worker_processes': worker_processes,
         'created': str(time.time()),
         'ssh_credentials': json.dumps(worker.ssh_credentials),
         'queue_name': work_queue_name,
         'err': "", **config,
     })
@@ -543,21 +543,21 @@
     budget_keeper.add_job(job_key)
 
     exec_mode = job_payload['config']['standalone']['exec_mode']
     exec_mode = StandaloneMode[exec_mode.upper()]
     workers = job_payload.pop('worker_instances')
 
     if exec_mode == StandaloneMode.CONSUME:
-        queue_name = f'wq:localhost:{runtime_name.replace("/", "-")}'
+        queue_name = f'wq:localhost:{runtime_name.replace("/", "-")}'.lower()
     elif exec_mode == StandaloneMode.CREATE:
-        queue_name = f'wq:{job_key}'
+        queue_name = f'wq:{job_key}'.lower()
     elif exec_mode == StandaloneMode.REUSE:
         worker_it = job_payload['worker_instance_type']
         worker_wp = job_payload['worker_processes']
-        queue_name = f'wq:{worker_it}-{worker_wp}-{runtime_name.replace("/", "-")}'
+        queue_name = f'wq:{worker_it}-{worker_wp}-{runtime_name.replace("/", "-")}'.lower()
 
     Thread(target=handle_job, args=(job_payload, queue_name)).start()
     Thread(target=handle_workers, args=(job_payload, workers, queue_name)).start()
 
     act_id = str(uuid.uuid4()).replace('-', '')[:12]
     response = flask.jsonify({'activationId': act_id})
     response.status_code = 202
```

### Comparing `lithops-3.2.0/lithops/standalone/runner.py` & `lithops-3.3.0/lithops/standalone/runner.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/standalone/standalone.py` & `lithops-3.3.0/lithops/standalone/standalone.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/standalone/utils.py` & `lithops-3.3.0/lithops/standalone/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,15 @@
     if [ "$INSTALL_DOCKER" = true ] && [ "$DOCKER_REQUIRED" = true ]; then
     apt-get install unzip redis-server python3-pip docker-ce docker-ce-cli containerd.io -y --fix-missing;
     else
     apt-get install unzip redis-server python3-pip -y --fix-missing;
     fi;
     sudo systemctl enable redis-server.service;
     sed -i 's/^bind 127.0.0.1 ::1/bind 0.0.0.0/' /etc/redis/redis.conf;
+    sudo systemctl restart redis-server.service;
 
     fi;
 
     if [[ ! $(pip3 list|grep "lithops") ]]; then
     wait_internet_connection;
     echo "--> Installing Lithops python dependencies"
     pip3 install -U pip flask gevent lithops[all];
```

### Comparing `lithops-3.2.0/lithops/standalone/worker.py` & `lithops-3.3.0/lithops/standalone/worker.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/storage/backends/aliyun_oss/aliyun_oss.py` & `lithops-3.3.0/lithops/storage/backends/aliyun_oss/aliyun_oss.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,23 @@
             self.bucket = oss2.Bucket(self.auth, self.endpoint, bucket_name)
             bucket = self.bucket
         return bucket
 
     def get_client(self):
         return self
 
+    def generate_bucket_name(self):
+        """
+        Generates a unique bucket name
+        """
+        key = self.config['access_key_id']
+        self.config['storage_bucket'] = f'lithops-{self.region}-{key[:6].lower()}'
+
+        return self.config['storage_bucket']
+
     def create_bucket(self, bucket_name):
         """
         Create a bucket if it doesn't exist
         """
         bucket = self._connect_bucket(bucket_name)
         bucket.create_bucket()
```

### Comparing `lithops-3.2.0/lithops/storage/backends/aliyun_oss/config.py` & `lithops-3.3.0/lithops/storage/backends/aliyun_oss/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import copy
-import hashlib
 
 
 CONNECTION_POOL_SIZE = 300
 
 REQ_PARAMS_1 = ('access_key_id', 'access_key_secret')
 
 PUBLIC_ENDPOINT = "oss-{}.aliyuncs.com"
@@ -44,13 +43,7 @@
 
     if 'region' not in config_data['aliyun_oss']:
         raise Exception('"region" is mandatory under the "aliyun_oss" or "aliyun" section of the configuration')
 
     region = config_data['aliyun_oss']['region']
     config_data['aliyun_oss']['public_endpoint'] = PUBLIC_ENDPOINT.format(region)
     config_data['aliyun_oss']['internal_endpoint'] = INTERNAL_ENDPOINT.format(region)
-
-    if 'storage_bucket' not in config_data['aliyun_oss']:
-        ossc = config_data['aliyun_oss']
-        key = ossc['access_key_id']
-        endpoint = hashlib.sha1(ossc['public_endpoint'].encode()).hexdigest()[:6]
-        config_data['aliyun_oss']['storage_bucket'] = f'lithops-{endpoint}-{key[:6].lower()}'
```

### Comparing `lithops-3.2.0/lithops/storage/backends/aws_s3/aws_s3.py` & `lithops-3.3.0/lithops/storage/backends/aws_s3/aws_s3.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import os
 import logging
 import boto3
-from botocore import UNSIGNED
 from botocore.config import Config
 import botocore
 
 from lithops.storage.utils import StorageNoSuchKeyError
 from lithops.utils import sizeof_fmt
 from lithops.constants import STORAGE_CLI_MSG
 from lithops.libs.globber import match
@@ -30,97 +29,100 @@
 
 OBJ_REQ_RETRIES = 5
 CONN_READ_TIMEOUT = 10
 
 
 class S3Backend:
     def __init__(self, s3_config):
-        logger.debug("Creating S3 client")
+        logger.debug("Creating AWS S3 Client")
         self.config = s3_config
         self.user_agent = s3_config['user_agent']
-        self.region_name = s3_config.get('region')
-        self.access_key_id = s3_config.get('access_key_id')
-        self.secret_access_key = s3_config.get('secret_access_key')
-        self.session_token = s3_config.get('session_token')
-
-        if self.access_key_id and self.secret_access_key:
-            client_config = Config(
-                max_pool_connections=128,
-                user_agent_extra=self.user_agent,
-                connect_timeout=CONN_READ_TIMEOUT,
-                read_timeout=CONN_READ_TIMEOUT,
-                retries={'max_attempts': OBJ_REQ_RETRIES}
-            )
-            self.s3_client = boto3.client(
-                's3', aws_access_key_id=self.access_key_id,
-                aws_secret_access_key=self.secret_access_key,
-                aws_session_token=self.session_token,
-                config=client_config,
-                region_name=self.region_name
-            )
-        else:
-            client_config = Config(
-                signature_version=UNSIGNED,
-                user_agent_extra=self.user_agent
-            )
-            self.s3_client = boto3.client('s3', config=client_config)
+        self.region = s3_config.get('region')
+
+        self.aws_session = boto3.Session(
+            aws_access_key_id=s3_config.get('access_key_id'),
+            aws_secret_access_key=s3_config.get('secret_access_key'),
+            aws_session_token=s3_config.get('session_token'),
+            region_name=self.region
+        )
+
+        s3_client_config = Config(
+            max_pool_connections=128,
+            user_agent_extra=self.user_agent,
+            connect_timeout=CONN_READ_TIMEOUT,
+            read_timeout=CONN_READ_TIMEOUT,
+            retries={'max_attempts': OBJ_REQ_RETRIES}
+        )
+
+        self.s3_client = self.aws_session.client('s3', config=s3_client_config)
 
         msg = STORAGE_CLI_MSG.format('S3')
-        logger.info(f"{msg} - Region: {self.region_name}")
+        logger.info(f"{msg} - Region: {self.region}")
 
     def get_client(self):
-        '''
+        """
         Get boto3 client.
         :return: boto3 client
-        '''
+        """
         return self.s3_client
 
+    def generate_bucket_name(self):
+        """
+        Generates a unique bucket name
+        """
+        sts_client = self.aws_session.client('sts')
+        caller_id = sts_client.get_caller_identity()
+        user_key = caller_id["UserId"].split(":")[0][-4:].lower()
+        self.config['storage_bucket'] = f'lithops-{self.region}-{user_key}'
+
+        return self.config['storage_bucket']
+
     def create_bucket(self, bucket_name):
         """
         Create a bucket if it doesn't exist
         """
         try:
             self.s3_client.head_bucket(Bucket=bucket_name)
         except botocore.exceptions.ClientError as e:
             if e.response['ResponseMetadata']['HTTPStatusCode'] == 404:
                 logger.debug(f"Could not find the bucket {bucket_name} in the AWS S3 storage backend")
                 logger.debug(f"Creating new bucket {bucket_name} in the AWS S3 storage backend")
-                bucket_config = {'LocationConstraint': self.region_name}
+                bucket_config = {'LocationConstraint': self.region}
                 self.s3_client.create_bucket(Bucket=bucket_name, CreateBucketConfiguration=bucket_config)
             else:
                 raise e
 
     def put_object(self, bucket_name, key, data):
-        '''
+        """
         Put an object in COS. Override the object if the key already exists.
         :param key: key of the object.
         :param data: data of the object
         :type data: str/bytes
         :return: None
-        '''
+        """
         try:
             res = self.s3_client.put_object(Bucket=bucket_name, Key=key, Body=data)
             status = 'OK' if res['ResponseMetadata']['HTTPStatusCode'] == 200 else 'Error'
             try:
                 logger.debug('PUT Object {} - Size: {} - {}'.format(key, sizeof_fmt(len(data)), status))
             except Exception:
                 logger.debug('PUT Object {} {}'.format(key, status))
         except botocore.exceptions.ClientError as e:
             if e.response['Error']['Code'] == 'NoSuchKey':
                 raise StorageNoSuchKeyError(bucket_name, key)
             else:
                 raise e
 
     def get_object(self, bucket_name, key, stream=False, extra_get_args={}):
-        '''
+        """
         Get object from COS with a key. Throws StorageNoSuchKeyError if the given key does not exist.
         :param key: key of the object
         :return: Data of the object
         :rtype: str/bytes
-        '''
+        """
         try:
             r = self.s3_client.get_object(Bucket=bucket_name, Key=key, **extra_get_args)
             if stream:
                 data = r['Body']
             else:
                 data = r['Body'].read()
             return data
@@ -169,74 +171,74 @@
             self.s3_client.download_file(Bucket=bucket, Key=key, Filename=file_name, **kwargs)
         except botocore.exceptions.ClientError as e:
             logging.error(e)
             return False
         return True
 
     def head_object(self, bucket_name, key):
-        '''
+        """
         Head object from COS with a key. Throws StorageNoSuchKeyError if the given key does not exist.
         :param key: key of the object
         :return: Data of the object
         :rtype: str/bytes
-        '''
+        """
         try:
             metadata = self.s3_client.head_object(Bucket=bucket_name, Key=key)
             return metadata['ResponseMetadata']['HTTPHeaders']
         except botocore.exceptions.ClientError as e:
             if e.response['Error']['Code'] == '404':
                 raise StorageNoSuchKeyError(bucket_name, key)
             else:
                 raise e
 
     def delete_object(self, bucket_name, key):
-        '''
+        """
         Delete an object from storage.
         :param bucket: bucket name
         :param key: data key
-        '''
+        """
         return self.s3_client.delete_object(Bucket=bucket_name, Key=key)
 
     def delete_objects(self, bucket_name, key_list):
-        '''
+        """
         Delete a list of objects from storage.
         :param bucket: bucket name
         :param key_list: list of keys
-        '''
+        """
         result = []
         max_keys_num = 1000
         for i in range(0, len(key_list), max_keys_num):
             delete_keys = {'Objects': []}
             delete_keys['Objects'] = [{'Key': k} for k in key_list[i:i + max_keys_num]]
             result.append(self.s3_client.delete_objects(Bucket=bucket_name, Delete=delete_keys))
         return result
 
     def head_bucket(self, bucket_name):
-        '''
+        """
         Head bucket from COS with a name. Throws StorageNoSuchKeyError if the given bucket does not exist.
         :param bucket_name: name of the bucket
         :return: Metadata of the bucket
         :rtype: str/bytes
-        '''
+        """
         try:
             return self.s3_client.head_bucket(Bucket=bucket_name)
         except botocore.exceptions.ClientError as e:
             if e.response['Error']['Code'] == '404':
                 raise StorageNoSuchKeyError(bucket_name, '')
             else:
                 raise e
 
     def list_objects(self, bucket_name, prefix=None, match_pattern=None):
-        '''
+        """
         Return a list of objects for the given bucket and prefix.
         :param bucket_name: Name of the bucket.
         :param prefix: Prefix to filter object names.
         :return: List of objects in bucket that match the given prefix.
         :rtype: list of str
-        '''
+        """
         try:
             prefix = '' if prefix is None else prefix
             paginator = self.s3_client.get_paginator('list_objects_v2')
             page_iterator = paginator.paginate(Bucket=bucket_name, Prefix=prefix)
 
             object_list = []
             for page in page_iterator:
@@ -249,21 +251,21 @@
             if e.response['Error']['Code'] == '404':
                 raise StorageNoSuchKeyError(
                     bucket_name, '' if prefix is None else prefix)
             else:
                 raise e
 
     def list_keys(self, bucket_name, prefix=None):
-        '''
+        """
         Return a list of keys for the given prefix.
         :param bucket_name: Name of the bucket.
         :param prefix: Prefix to filter object names.
         :return: List of keys in bucket that match the given prefix.
         :rtype: list of str
-        '''
+        """
         try:
             prefix = '' if prefix is None else prefix
             paginator = self.s3_client.get_paginator('list_objects_v2')
             page_iterator = paginator.paginate(Bucket=bucket_name, Prefix=prefix)
 
             key_list = []
             for page in page_iterator:
```

### Comparing `lithops-3.2.0/lithops/storage/backends/aws_s3/config.py` & `lithops-3.3.0/lithops/storage/backends/aws_s3/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,27 +18,19 @@
 import copy
 
 
 def load_config(config_data):
 
     if 'aws' in config_data:
 
-        if not {'access_key_id', 'secret_access_key'}.issubset(set(config_data['aws'])):
-            raise Exception("'access_key_id' and 'secret_access_key' are mandatory under the 'aws' section of the configuration")
-
         if 'aws_s3' not in config_data:
             config_data['aws_s3'] = {}
 
         temp = copy.deepcopy(config_data['aws_s3'])
         config_data['aws_s3'].update(config_data['aws'])
         config_data['aws_s3'].update(temp)
 
         if 'region_name' in config_data['aws_s3']:
             config_data['aws_s3']['region'] = config_data['aws_s3'].pop('region_name')
 
         if 'region' not in config_data['aws_s3']:
             raise Exception("'region' is mandatory under 'aws_s3' or 'aws' section of the configuration")
-
-        if 'storage_bucket' not in config_data['aws_s3']:
-            key = config_data['aws_s3']['access_key_id']
-            region = config_data['aws_s3']['region']
-            config_data['aws_s3']['storage_bucket'] = f'lithops-{region}-{key[:6].lower()}'
```

### Comparing `lithops-3.2.0/lithops/storage/backends/azure_storage/azure_storage.py` & `lithops-3.3.0/lithops/storage/backends/azure_storage/azure_storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import os
+import hashlib
 import shutil
 import logging
 from io import BytesIO
 from azure.storage.blob import BlobServiceClient
 from azure.core.exceptions import ResourceNotFoundError, ResourceExistsError
 from lithops.storage.utils import StorageNoSuchKeyError
 from lithops.constants import STORAGE_CLI_MSG
@@ -26,30 +27,44 @@
 logger = logging.getLogger(__name__)
 
 
 class AzureBlobStorageBackend:
 
     def __init__(self, azure_blob_config):
         logger.debug("Creating Azure Blob Storage client")
+        self.config = azure_blob_config
         self.storage_account_name = azure_blob_config['storage_account_name']
         self.blob_service_url = 'https://{}.blob.core.windows.net'.format(self.storage_account_name)
-        self.blob_client = BlobServiceClient(account_url=self.blob_service_url,
-                                             credential=azure_blob_config['storage_account_key'])
+
+        self.blob_client = BlobServiceClient(
+            account_url=self.blob_service_url,
+            credential=azure_blob_config['storage_account_key']
+        )
 
         msg = STORAGE_CLI_MSG.format('Azure Blob')
         logger.info("{}".format(msg))
 
     def get_client(self):
         """
         Get Azure BlobServiceClient client.
         :return: storage client
         :rtype: azure.storage.blob.BlobServiceClient
         """
         return self.blob_client
 
+    def generate_bucket_name(self):
+        """
+        Generates a unique bucket name
+        """
+        key = self.config['storage_account_key']
+        account = hashlib.sha1(self.config['storage_account_name'].encode()).hexdigest()[:6]
+        self.config['storage_bucket'] = f'lithops-{account}-{key[:6].lower()}'
+
+        return self.config['storage_bucket']
+
     def create_bucket(self, bucket_name):
         """
         Create a bucket if it doesn't exist
         """
         try:
             self.blob_client.create_container(bucket_name)
         except ResourceExistsError:
```

### Comparing `lithops-3.2.0/lithops/storage/backends/ceph/ceph.py` & `lithops-3.3.0/lithops/storage/backends/ceph/ceph.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import os
 import logging
 import boto3
+import hashlib
 import botocore
 from lithops.storage.utils import StorageNoSuchKeyError
 from lithops.utils import sizeof_fmt
 from lithops.constants import STORAGE_CLI_MSG
 
 logger = logging.getLogger(__name__)
 
@@ -33,44 +34,54 @@
     A wrap-up around Ceph boto3 APIs.
     """
 
     def __init__(self, ceph_config):
         logger.debug("Creating Ceph client")
         self.config = ceph_config
         user_agent = ceph_config['user_agent']
-        service_endpoint = ceph_config['endpoint']
+        self.service_endpoint = ceph_config['endpoint']
 
-        logger.debug(f"Setting Ceph endpoint to {service_endpoint}")
+        logger.debug(f"Setting Ceph endpoint to {self.service_endpoint}")
 
         client_config = botocore.client.Config(
             max_pool_connections=128,
             user_agent_extra=user_agent,
             connect_timeout=CONN_READ_TIMEOUT,
             read_timeout=CONN_READ_TIMEOUT,
             retries={'max_attempts': OBJ_REQ_RETRIES}
         )
 
         self.s3_client = boto3.client(
             's3', aws_access_key_id=ceph_config['access_key_id'],
             aws_secret_access_key=ceph_config['secret_access_key'],
             aws_session_token=ceph_config.get('session_token'),
             config=client_config,
-            endpoint_url=service_endpoint
+            endpoint_url=self.service_endpoint
         )
 
         msg = STORAGE_CLI_MSG.format('Ceph')
-        logger.info(f"{msg} - Endpoint: {service_endpoint}")
+        logger.info(f"{msg} - Endpoint: {self.service_endpoint}")
 
     def get_client(self):
         """
         Get ibm_boto3 client.
         :return: ibm_boto3 client
         """
         return self.s3_client
 
+    def generate_bucket_name(self):
+        """
+        Generates a unique bucket name
+        """
+        key = self.config['access_key_id']
+        endpoint = hashlib.sha1(self.service_endpoint.encode()).hexdigest()[:6]
+        self.config['storage_bucket'] = f'lithops-{endpoint}-{key[:6].lower()}'
+
+        return self.config['storage_bucket']
+
     def create_bucket(self, bucket_name):
         """
         Create a bucket if it doesn't exist
         """
         try:
             self.s3_client.head_bucket(Bucket=bucket_name)
         except botocore.exceptions.ClientError as e:
```

### Comparing `lithops-3.2.0/lithops/storage/backends/ceph/config.py` & `lithops-3.3.0/lithops/storage/backends/ceph/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,29 +11,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 
-import hashlib
-
-
 REQ_PARAMS = ('endpoint', 'secret_access_key', 'access_key_id')
 
 
 def load_config(config_data):
     if 'ceph' not in config_data:
         raise Exception("ceph section is mandatory in the configuration")
 
     for param in REQ_PARAMS:
         if param not in config_data['ceph']:
             msg = f"'{param}' is mandatory under 'ceph' section of the configuration"
             raise Exception(msg)
 
     if not config_data['ceph']['endpoint'].startswith('http'):
         raise Exception('Ceph endpoint must start with http:// or https://')
-
-    if 'storage_bucket' not in config_data['ceph']:
-        key = config_data['ceph']['access_key_id']
-        endpoint = hashlib.sha1(config_data['ceph']['endpoint'].encode()).hexdigest()[:6]
-        config_data['ceph']['storage_bucket'] = f'lithops-{endpoint}-{key[:6].lower()}'
```

### Comparing `lithops-3.2.0/lithops/storage/backends/gcp_storage/config.py` & `lithops-3.3.0/lithops/storage/backends/gcp_storage/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import copy
-import hashlib
 import os
 
 
 def load_config(config_data=None):
     if 'gcp' not in config_data:
         raise Exception("gcp section is mandatory in the configuration")
 
@@ -35,13 +34,7 @@
 
     temp = copy.deepcopy(config_data['gcp_storage'])
     config_data['gcp_storage'].update(config_data['gcp'])
     config_data['gcp_storage'].update(temp)
 
     if 'region' not in config_data['gcp_storage']:
         raise Exception("'region' parameter is mandatory under 'gcp_storage' or 'gcp' section of the configuration")
-
-    if 'storage_bucket' not in config_data['gcp_storage']:
-        gcps = config_data['gcp_storage']
-        region = gcps['region']
-        key = hashlib.sha1(gcps['credentials_path'].encode()).hexdigest()[:6]
-        config_data['gcp_storage']['storage_bucket'] = f'lithops-{region}-{key[:6].lower()}'
```

### Comparing `lithops-3.2.0/lithops/storage/backends/gcp_storage/gcp_storage.py` & `lithops-3.3.0/lithops/storage/backends/gcp_storage/gcp_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # limitations under the License.
 #
 
 import re
 import os
 import shutil
 import time
+import hashlib
 import logging
 from requests.exceptions import SSLError as TooManyConnectionsError
 from io import BytesIO
 from google.api_core import exceptions as google_exceptions
 from google.cloud import storage
 from lithops.constants import STORAGE_CLI_MSG
 from lithops.storage.utils import StorageNoSuchKeyError
@@ -31,14 +32,15 @@
 TIMEOUT = 5
 
 
 class GCPStorageBackend:
 
     def __init__(self, gcp_storage_config):
         logger.debug("Creating GCP Storage client")
+        self.config = gcp_storage_config
         self.credentials_path = gcp_storage_config.get('credentials_path')
         self.region = gcp_storage_config['region']
 
         if self.credentials_path and os.path.isfile(self.credentials_path):
             logger.debug(f'Getting GCP credentials from {self.credentials_path}')
             self.client = storage.Client.from_service_account_json(self.credentials_path)
         else:
@@ -47,14 +49,23 @@
 
         msg = STORAGE_CLI_MSG.format('Google Cloud Storage')
         logger.info(f"{msg} - Region: {self.region}")
 
     def get_client(self):
         return self.client
 
+    def generate_bucket_name(self):
+        """
+        Generates a unique bucket name
+        """
+        key = hashlib.sha1(self.credentials_path.encode()).hexdigest()[:6]
+        self.config['storage_bucket'] = f'lithops-{self.region}-{key[:6].lower()}'
+
+        return self.config['storage_bucket']
+
     def exists_bucket(self, bucket_name):
         try:
             self.client.get_bucket(bucket_name, timeout=TIMEOUT)
             return True
         except google_exceptions.NotFound:
             return False
```

### Comparing `lithops-3.2.0/lithops/storage/backends/ibm_cos/config.py` & `lithops-3.3.0/lithops/storage/backends/ibm_cos/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -74,22 +74,7 @@
 
     if not config_data['ibm_cos']['endpoint'].startswith('http'):
         raise Exception('IBM COS Endpoint must start with http:// or https://')
 
     if 'region' not in config_data['ibm_cos']:
         endpoint = config_data['ibm_cos']['endpoint']
         config_data['ibm_cos']['region'] = endpoint.split('//')[1].split('.')[1]
-
-    if 'access_key' in config_data['ibm_cos']:
-        config_data['ibm_cos']['access_key_id'] = config_data['ibm_cos'].pop('access_key')
-    if 'secret_key' in config_data['ibm_cos']:
-        config_data['ibm_cos']['secret_access_key'] = config_data['ibm_cos'].pop('secret_key')
-
-    if 'storage_bucket' not in config_data['ibm_cos']:
-        if not {'access_key_id', 'secret_access_key'}.issubset(config_data['ibm_cos']):
-            msg = "'storage_bucket' parameter not found in config. "
-            msg += "You must provide HMAC Credentials if you want the bucket to be automatically created"
-            raise Exception(msg)
-        cosc = config_data['ibm_cos']
-        key = cosc.get('access_key_id') or cosc.get('api_key') or cosc.get('iam_api_key')
-        region = config_data['ibm_cos']['region']
-        config_data['ibm_cos']['storage_bucket'] = f'lithops-{region}-{key[:6].lower()}'
```

### Comparing `lithops-3.2.0/lithops/storage/backends/ibm_cos/ibm_cos.py` & `lithops-3.3.0/lithops/storage/backends/ibm_cos/ibm_cos.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,14 +112,27 @@
     def get_client(self):
         """
         Get ibm_boto3 client.
         :return: ibm_boto3 client
         """
         return self.cos_client
 
+    def generate_bucket_name(self):
+        """
+        Generates a unique bucket name
+        """
+        if not {'access_key_id', 'secret_access_key'}.issubset(self.config):
+            msg = "'storage_bucket' parameter not found in config. You must provide HMAC "
+            msg += "Credentials if you want the bucket to be automatically created"
+            raise Exception(msg)
+        key = self.config.get('access_key_id') or self.api_key or self.iam_api_key
+        self.config['storage_bucket'] = f"lithops-{self.region}-{key[:6].lower()}"
+
+        return self.config['storage_bucket']
+
     def create_bucket(self, bucket_name):
         """
         Create a bucket if it doesn't exist
         """
         try:
             self.cos_client.head_bucket(Bucket=bucket_name)
         except ibm_botocore.exceptions.ClientError as e:
```

### Comparing `lithops-3.2.0/lithops/storage/backends/infinispan/config.py` & `lithops-3.3.0/lithops/storage/backends/infinispan/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/storage/backends/infinispan/infinispan.py` & `lithops-3.3.0/lithops/storage/backends/infinispan/infinispan.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/storage/backends/infinispan_hotrod/config.py` & `lithops-3.3.0/lithops/storage/backends/infinispan_hotrod/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/storage/backends/infinispan_hotrod/infinispan_hotrod.py` & `lithops-3.3.0/lithops/storage/backends/infinispan_hotrod/infinispan_hotrod.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/storage/backends/localhost/config.py` & `lithops-3.3.0/lithops/storage/backends/localhost/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/storage/backends/localhost/localhost.py` & `lithops-3.3.0/lithops/storage/backends/localhost/localhost.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/storage/backends/minio/config.py` & `lithops-3.3.0/lithops/storage/backends/azure_storage/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# (C) Copyright Cloudlab URV 2021
+# (C) Copyright Cloudlab URV 2020
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,29 +11,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 
-import hashlib
+REQ_PARAMS = ('storage_account_name', 'storage_account_key')
 
 
-REQ_PARAMS = ('endpoint', 'secret_access_key', 'access_key_id')
+def load_config(config_data=None):
 
-
-def load_config(config_data):
-    if 'minio' not in config_data:
-        raise Exception("minio section is mandatory in the configuration")
+    if 'azure_storage' not in config_data:
+        raise Exception("'azure_storage' section is mandatory in the configuration")
 
     for param in REQ_PARAMS:
-        if param not in config_data['minio']:
-            msg = f"'{param}' is mandatory under 'minio' section of the configuration"
+        if param not in config_data['azure_storage']:
+            msg = f"'{param}' is mandatory under 'azure_storage' section of the configuration"
             raise Exception(msg)
-
-    if not config_data['minio']['endpoint'].startswith('http'):
-        raise Exception('MinIO endpoint must start with http:// or https://')
-
-    if 'storage_bucket' not in config_data['minio']:
-        key = config_data['minio']['access_key_id']
-        endpoint = hashlib.sha1(config_data['minio']['endpoint'].encode()).hexdigest()[:6]
-        config_data['minio']['storage_bucket'] = f'lithops-{endpoint}-{key[:6].lower()}'
```

### Comparing `lithops-3.2.0/lithops/storage/backends/minio/minio.py` & `lithops-3.3.0/lithops/storage/backends/minio/minio.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import os
+import hashlib
 import logging
 import boto3
 import botocore
 from lithops.storage.utils import StorageNoSuchKeyError
 from lithops.utils import sizeof_fmt
 from lithops.constants import STORAGE_CLI_MSG
 
@@ -33,44 +34,54 @@
     A wrap-up around MinIO boto3 APIs.
     """
 
     def __init__(self, minio_config):
         logger.debug("Creating MinIO client")
         self.config = minio_config
         user_agent = minio_config['user_agent']
-        service_endpoint = minio_config['endpoint']
+        self.service_endpoint = minio_config['endpoint']
 
-        logger.debug(f"Setting MinIO endpoint to {service_endpoint}")
+        logger.debug(f"Setting MinIO endpoint to {self.service_endpoint}")
 
         client_config = botocore.client.Config(
             max_pool_connections=128,
             user_agent_extra=user_agent,
             connect_timeout=CONN_READ_TIMEOUT,
             read_timeout=CONN_READ_TIMEOUT,
             retries={'max_attempts': OBJ_REQ_RETRIES}
         )
 
         self.s3_client = boto3.client(
             's3', aws_access_key_id=minio_config['access_key_id'],
             aws_secret_access_key=minio_config['secret_access_key'],
             aws_session_token=minio_config.get('session_token'),
             config=client_config,
-            endpoint_url=service_endpoint
+            endpoint_url=self.service_endpoint
         )
 
         msg = STORAGE_CLI_MSG.format('MinIO')
-        logger.info(f"{msg} - Endpoint: {service_endpoint}")
+        logger.info(f"{msg} - Endpoint: {self.service_endpoint}")
 
     def get_client(self):
         """
         Get ibm_boto3 client.
         :return: ibm_boto3 client
         """
         return self.s3_client
 
+    def generate_bucket_name(self):
+        """
+        Generates a unique bucket name
+        """
+        key = self.config['access_key_id']
+        endpoint = hashlib.sha1(self.service_endpoint.encode()).hexdigest()[:6]
+        self.config['storage_bucket'] = f'lithops-{endpoint}-{key[:6].lower()}'
+
+        return self.config['storage_bucket']
+
     def create_bucket(self, bucket_name):
         """
         Create a bucket if it doesn't exist
         """
         try:
             self.s3_client.head_bucket(Bucket=bucket_name)
         except botocore.exceptions.ClientError as e:
```

### Comparing `lithops-3.2.0/lithops/storage/backends/oracle_oss/config.py` & `lithops-3.3.0/lithops/storage/backends/oracle_oss/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -33,12 +33,7 @@
         if param not in config_data['oracle']:
             msg = f'"{param}" is mandatory under "oracle" section of the configuration'
             raise Exception(msg)
 
     temp = copy.deepcopy(config_data['oracle_oss'])
     config_data['oracle_oss'].update(config_data['oracle'])
     config_data['oracle_oss'].update(temp)
-
-    if 'storage_bucket' not in config_data['oracle_oss']:
-        user = config_data['oracle_oss']['user']
-        region = config_data['oracle_oss']['region']
-        config_data['oracle_oss']['storage_bucket'] = f'lithops-{region}-{user[-8:-1].lower()}'
```

### Comparing `lithops-3.2.0/lithops/storage/backends/oracle_oss/oracle_oss.py` & `lithops-3.3.0/lithops/storage/backends/oracle_oss/oracle_oss.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,23 @@
         else:
             self.signer = oci.auth.signers.get_resource_principals_signer()
             return ObjectStorageClient(config={}, signer=self.signer)
 
     def get_client(self):
         return self
 
+    def generate_bucket_name(self):
+        """
+        Generates a unique bucket name
+        """
+        user = self.config['user']
+        self.config['storage_bucket'] = f'lithops-{self.region}-{user[-8:-1].lower()}'
+
+        return self.config['storage_bucket']
+
     def create_bucket(self, bucket_name):
         """
         Create a bucket if it doesn't exist
         """
         try:
             self.os_client.create_bucket(
                 namespace_name=self.namespace,
```

### Comparing `lithops-3.2.0/lithops/storage/backends/redis/config.py` & `lithops-3.3.0/lithops/storage/backends/redis/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/storage/backends/redis/redis.py` & `lithops-3.3.0/lithops/storage/backends/redis/redis.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/storage/backends/swift/config.py` & `lithops-3.3.0/lithops/storage/backends/swift/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/storage/backends/swift/swift.py` & `lithops-3.3.0/lithops/storage/backends/swift/swift.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,14 +53,22 @@
         adapter = requests.adapters.HTTPAdapter(pool_maxsize=64, max_retries=3)
         self.session.mount('http://', adapter)
         self.session.mount('https://', adapter)
 
         msg = STORAGE_CLI_MSG.format('OpenStack Swift')
         logger.info("{} - Region: {}".format(msg, self.region))
 
+    def generate_bucket_name(self):
+        """
+        Generates a unique bucket name
+        """
+        self.config['storage_bucket'] = f'lithops-{self.region}-{self.user_id[:6].lower()}'
+
+        return self.config['storage_bucket']
+
     def generate_swift_token(self):
         """
         Generates new token for accessing to Swift.
         :return: token
         """
         url = self.auth_url + "/v3/auth/tokens"
         headers = {'Content-Type': 'application/json'}
@@ -85,62 +93,60 @@
                 raise Exception('Invalid region name')
 
             return r.headers['X-Subject-Token']
         else:
             message = json.loads(r.text)['error']['message']
             raise Exception("{} - {} - {}".format(r.status_code, r.reason, message))
 
-    def put_object(self, container_name, key, data):
+    def put_object(self, bucket_name, key, data):
         """
         Put an object in Swift. Override the object if the key already exists.
         :param key: key of the object.
         :param data: data of the object
         :type data: str/bytes
         :return: None
         """
-        url = '/'.join([self.endpoint, container_name, key])
+        url = '/'.join([self.endpoint, bucket_name, key])
         try:
             res = self.session.put(url, data=data)
             status = 'OK' if res.status_code == 201 else 'Error'
             try:
                 logger.debug('PUT Object {} - Size: {} - {}'.format(key, sizeof_fmt(len(data)), status))
             except Exception:
                 logger.debug('PUT Object {} - {}'.format(key, status))
         except Exception as e:
             print(e)
 
-    def get_object(self, container_name, key, stream=False, extra_get_args={}):
+    def get_object(self, bucket_name, key, stream=False, extra_get_args={}):
         """
         Get object from Swift with a key. Throws StorageNoSuchKeyError if the given key does not exist.
         :param key: key of the object
         :return: Data of the object
         :rtype: str/bytes
         """
-        if not container_name:
-            container_name = self.storage_container
-        url = '/'.join([self.endpoint, container_name, key])
+        url = '/'.join([self.endpoint, bucket_name, key])
         headers = {'X-Auth-Token': self.token}
         headers.update(extra_get_args)
         try:
             res = self.session.get(url, headers=headers, stream=stream)
             if res.status_code == 200 or res.status_code == 206:
                 if stream:
                     data = res.raw
                 else:
                     data = res.content
                 return data
             elif res.status_code == 404:
-                raise StorageNoSuchKeyError(container_name, key)
+                raise StorageNoSuchKeyError(bucket_name, key)
             else:
                 raise Exception('{} - {}'.format(res.status_code, key))
         except StorageNoSuchKeyError:
-            raise StorageNoSuchKeyError(container_name, key)
+            raise StorageNoSuchKeyError(bucket_name, key)
         except Exception as e:
             print(e)
-            raise StorageNoSuchKeyError(container_name, key)
+            raise StorageNoSuchKeyError(bucket_name, key)
 
     def upload_file(self, file_name, bucket, key=None, extra_args={}, config=None):
         """Upload a file
 
         :param file_name: File to upload
         :param bucket: Bucket to upload to
         :param key: S3 object name. If not specified then file_name is used
@@ -180,85 +186,85 @@
                 data_stream = self.get_object(bucket, key, stream=True)
                 shutil.copyfileobj(data_stream, out)
         except Exception as e:
             logging.error(e)
             return False
         return True
 
-    def head_object(self, container_name, key):
+    def head_object(self, bucket_name, key):
         """
         Head object from Swift with a key. Throws StorageNoSuchKeyError if the given key does not exist.
         :param key: key of the object
         :return: Data of the object
         :rtype: str/bytes
         """
-        url = '/'.join([self.endpoint, container_name, key])
+        url = '/'.join([self.endpoint, bucket_name, key])
         try:
             res = self.session.head(url)
             if res.status_code == 200:
                 return res.headers
             elif res.status_code == 404:
-                raise StorageNoSuchKeyError(container_name, key)
+                raise StorageNoSuchKeyError(bucket_name, key)
             else:
                 raise Exception('{} - {}'.format(res.status_code, key))
         except Exception:
-            raise StorageNoSuchKeyError(container_name, key)
+            raise StorageNoSuchKeyError(bucket_name, key)
 
-    def delete_object(self, container_name, key):
+    def delete_object(self, bucket_name, key):
         """
         Delete an object from Swift.
         :param bucket: bucket name
         :param key: data key
         """
-        url = '/'.join([self.endpoint, container_name, key])
+        url = '/'.join([self.endpoint, bucket_name, key])
         return self.session.delete(url)
 
-    def delete_objects(self, container_name, key_list):
+    def delete_objects(self, bucket_name, key_list):
         """
         Delete a list of objects from Swift.
         :param bucket: bucket name
         :param key: data key
         """
         headers = {'X-Auth-Token': self.token,
                    'X-Bulk-Delete': 'True'}
 
         keys_to_delete = []
         for key in key_list:
-            keys_to_delete.append('/{}/{}'.format(container_name, key))
+            keys_to_delete.append('/{}/{}'.format(bucket_name, key))
 
         keys_to_delete = '\n'.join(keys_to_delete)
         url = '/'.join([self.endpoint, '?bulk-delete'])
         return self.session.delete(url, data=keys_to_delete, headers=headers)
 
-    def list_objects(self, container_name, prefix='', match_pattern=None):
+    def list_objects(self, bucket_name, prefix='', match_pattern=None):
         """
         Lists the objects in a bucket. Throws StorageNoSuchKeyError if the given bucket does not exist.
         :param key: key of the object
         :return: Data of the object
         :rtype: str/bytes
         """
         if prefix:
-            url = '/'.join([self.endpoint, container_name, '?format=json&prefix=' + prefix])
+            url = '/'.join([self.endpoint, bucket_name, '?format=json&prefix=' + prefix])
         else:
-            url = '/'.join([self.endpoint, container_name, '?format=json'])
+            url = '/'.join([self.endpoint, bucket_name, '?format=json'])
         try:
             res = self.session.get(url)
             objects = res.json()
 
             # TODO: Adapt to Key and Size
             return objects
         except Exception as e:
             raise e
 
-    def list_keys(self, container_name, prefix):
+    def list_keys(self, bucket_name, prefix):
         """
         Return a list of keys for the given prefix.
         :param prefix: Prefix to filter object names.
         :return: List of keys in bucket that match the given prefix.
         :rtype: list of str
         """
         try:
-            objects = self.list_objects(container_name, prefix)
+            objects = self.list_objects(bucket_name, prefix)
             object_keys = [r['name'] for r in objects]
             return object_keys
         except Exception as e:
             raise e
```

### Comparing `lithops-3.2.0/lithops/storage/cloud_proxy.py` & `lithops-3.3.0/lithops/storage/cloud_proxy.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/storage/storage.py` & `lithops-3.3.0/lithops/storage/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,26 +54,28 @@
             self.config = storage_config
         else:
             storage_config = default_storage_config(
                 config_data=config, backend=backend)
             self.config = extract_storage_config(storage_config)
 
         self.backend = self.config['backend']
-        self.bucket = self.config['bucket']
 
         try:
             module_location = f'lithops.storage.backends.{self.backend}'
             sb_module = importlib.import_module(module_location)
             StorageBackend = getattr(sb_module, 'StorageBackend')
             self.storage_handler = StorageBackend(self.config[self.backend])
         except Exception as e:
             logger.error("An exception was produced trying to create the "
                          f"'{self.backend}' storage backend")
             raise e
 
+        bucket = self.config[self.backend].get('storage_bucket')
+        self.bucket = bucket or self.storage_handler.generate_bucket_name()
+
     def get_client(self) -> object:
         """
         Retrieves the underlying storage client.
 
         :return: Storage backend client
         """
         return self.storage_handler.get_client()
```

### Comparing `lithops-3.2.0/lithops/storage/utils.py` & `lithops-3.3.0/lithops/storage/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,17 +161,17 @@
     :return: output key
     """
     job_key = create_job_key(executor_id, job_id)
     return '/'.join([JOBS_PREFIX, job_key, call_id, f'{act_id}{init_key_suffix}'])
 
 
 def get_storage_path(storage_config):
-    storage_bucket = storage_config['bucket']
-    storage_backend = storage_config['backend']
+    backend = storage_config['backend']
+    bucket = storage_config[backend]['storage_bucket']
 
-    return [storage_backend, storage_bucket]
+    return [backend, bucket]
 
 
-def check_storage_path(config, prev_path):
-    current_path = get_storage_path(config)
+def check_storage_path(storage_config, prev_path):
+    current_path = get_storage_path(storage_config)
     if current_path != prev_path:
         raise StorageConfigMismatchError(current_path, prev_path)
```

### Comparing `lithops-3.2.0/lithops/tests/test_map_reduce.py` & `lithops-3.3.0/lithops/tests/test_map_reduce.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,171 +8,217 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+import pytest
 import math
-import unittest
+import base64
+import urllib
 import logging
-
 import lithops
-from lithops.tests import main_util
-from lithops.tests.util_func.map_reduce_util import simple_reduce_function, my_reduce_function
-from lithops.tests.util_func.map_util import simple_map_function, my_map_function_obj, my_map_function_url
-from lithops.tests.util_func.storage_util import list_dataset_keys, get_dataset_key_size
+from concurrent.futures import ThreadPoolExecutor
+from lithops.tests.conftest import TESTS_PREFIX
+from lithops.config import extract_storage_config
+from lithops.tests.functions import (
+    simple_reduce_function,
+    my_reduce_function,
+    simple_map_function,
+    my_map_function_obj,
+    my_map_function_url
+)
+
+
+DATASET_PREFIX = TESTS_PREFIX + '/dataset'
+base64_bytes = 'aHR0cHM6Ly9zMy1ldS13ZXN0LTEuYW1hem9uYXdzLmNvbS9hcnRtLw=='.encode('ascii')
+TEST_FILES_REPO = base64.b64decode(base64_bytes).decode('ascii')
+TEST_FILES_URLS = [
+    TEST_FILES_REPO + "vocab.enron.txt",
+    TEST_FILES_REPO + "vocab.kos.txt",
+    TEST_FILES_REPO + "vocab.nips.txt",
+    TEST_FILES_REPO + "vocab.nytimes.txt",
+    TEST_FILES_REPO + "vocab.pubmed.txt"
+]
 
 logger = logging.getLogger(__name__)
 
-CONFIG = None
-STORAGE_CONFIG = None
-STORAGE = None
-TEST_FILES_URLS = None
-PREFIX = '__lithops.test'
-DATASET_PREFIX = PREFIX + '/dataset'
-
 
-class TestMapReduce(unittest.TestCase):
-    words_in_cos_files = None
+class TestMapReduce:
 
     @classmethod
-    def setUpClass(cls):
-        global CONFIG, STORAGE, STORAGE_CONFIG, TEST_FILES_URLS
-
-        CONFIG, STORAGE, STORAGE_CONFIG = main_util.get_config().values()
-        TEST_FILES_URLS = main_util.get_data_sets()
-        cls.words_in_cos_files = main_util.get_words_in_files()
+    def setup_class(cls):
+        storage_config = extract_storage_config(pytest.lithops_config)
+        storage = lithops.Storage(storage_config=storage_config)
+        cls.words_in_files = upload_data_sets(storage)
+        cls.storage = storage
+        cls.storage_backend = storage.backend
+        cls.bucket = storage.bucket
 
     @classmethod
-    def setUp(cls):
-        print('\n-------------------------------------------------------------\n')
+    def teardown_class(cls):
+        for key in cls.storage.list_keys(bucket=cls.bucket, prefix=DATASET_PREFIX):
+            cls.storage.delete_object(bucket=cls.bucket, key=key)
 
-    def test_map_reduce(self):
+    def test_simple_map_reduce(self):
         logger.info('Testing map_reduce() using memory')
         iterdata = [(1, 1), (2, 2), (3, 3), (4, 4)]
-        fexec = lithops.FunctionExecutor(config=CONFIG)
-        fexec.map_reduce(simple_map_function, iterdata,
-                         simple_reduce_function)
+        fexec = lithops.FunctionExecutor(config=pytest.lithops_config)
+        fexec.map_reduce(simple_map_function, iterdata, simple_reduce_function)
         result = fexec.get_result()
-        self.assertEqual(result, 20)
+        assert result == 20
 
-    def test_map_reduce_obj_bucket(self):
+    def test_obj_bucket(self):
         logger.info('Testing map_reduce() over a bucket')
-        sb = STORAGE_CONFIG['backend']
-        data_prefix = sb + '://' + STORAGE_CONFIG['bucket'] + '/' + DATASET_PREFIX + '/'
-        fexec = lithops.FunctionExecutor(config=CONFIG)
+        data_prefix = self.storage_backend + '://' + self.bucket + '/' + DATASET_PREFIX + '/'
+        fexec = lithops.FunctionExecutor(config=pytest.lithops_config)
         fexec.map_reduce(my_map_function_obj, data_prefix,
                          my_reduce_function)
         result = fexec.get_result()
-        self.assertEqual(result, self.__class__.words_in_cos_files)
+        assert result == self.words_in_files
 
-    def test_map_reduce_obj_bucket_reduce_by_key(self):
+    def test_obj_bucket_reduce_by_key(self):
         logger.info('Testing map_reduce() over a bucket with one reducer per object')
-        sb = STORAGE_CONFIG['backend']
-        data_prefix = sb + '://' + STORAGE_CONFIG['bucket'] + '/' + DATASET_PREFIX + '/'
-        fexec = lithops.FunctionExecutor(config=CONFIG)
+        data_prefix = self.storage_backend + '://' + self.bucket + '/' + DATASET_PREFIX + '/'
+        fexec = lithops.FunctionExecutor(config=pytest.lithops_config)
         fexec.map_reduce(my_map_function_obj, data_prefix,
-                         my_reduce_function,
-                         obj_reduce_by_key=True)
+                         my_reduce_function, obj_reduce_by_key=True)
         result = fexec.get_result()
-        # the reducer returns a list containing sum of the words uploaded via each file.
-        self.assertEqual(sum(result), self.__class__.words_in_cos_files)
+        assert sum(result) == self.words_in_files
 
-    def test_map_reduce_obj_key(self):
+    def test_obj_key(self):
         logger.info('Testing map_reduce() over object keys')
-        sb = STORAGE_CONFIG['backend']
-        bucket_name = STORAGE_CONFIG['bucket']
-        iterdata = [sb + '://' + bucket_name + '/' + key for key in list_dataset_keys(STORAGE, STORAGE_CONFIG)]
-        fexec = lithops.FunctionExecutor(config=CONFIG)
-        fexec.map_reduce(my_map_function_obj, iterdata,
-                         my_reduce_function)
+        keys = self.storage.list_keys(bucket=self.bucket, prefix=DATASET_PREFIX + '/')
+        iterdata = [self.storage_backend + '://' + self.bucket + '/' + key for key in keys]
+        fexec = lithops.FunctionExecutor(config=pytest.lithops_config)
+        fexec.map_reduce(my_map_function_obj, iterdata, my_reduce_function)
         result = fexec.get_result()
-        self.assertEqual(result, self.__class__.words_in_cos_files)
+        assert result == self.words_in_files
 
-    def test_map_reduce_obj_key_reduce_by_key(self):
+    def test_obj_key_reduce_by_key(self):
         logger.info('Testing map_reduce() over object keys with one reducer per object')
-        sb = STORAGE_CONFIG['backend']
-        bucket_name = STORAGE_CONFIG['bucket']
-        iterdata = [sb + '://' + bucket_name + '/' + key for key in list_dataset_keys(STORAGE, STORAGE_CONFIG)]
-        fexec = lithops.FunctionExecutor(config=CONFIG)
+        keys = self.storage.list_keys(bucket=self.bucket, prefix=DATASET_PREFIX + '/')
+        iterdata = [self.storage_backend + '://' + self.bucket + '/' + key for key in keys]
+        fexec = lithops.FunctionExecutor(config=pytest.lithops_config)
         fexec.map_reduce(my_map_function_obj, iterdata,
-                         my_reduce_function,
-                         obj_reduce_by_key=True)
+                         my_reduce_function, obj_reduce_by_key=True)
         result = fexec.get_result()
-        self.assertEqual(sum(result), self.__class__.words_in_cos_files)
+        assert sum(result) == self.words_in_files
 
-    def test_map_reduce_url(self):
+    def test_url_processing(self):
         logger.info('Testing map_reduce() over URLs')
-        fexec = lithops.FunctionExecutor(config=CONFIG)
+        fexec = lithops.FunctionExecutor(config=pytest.lithops_config)
         fexec.map_reduce(my_map_function_url, TEST_FILES_URLS,
                          my_reduce_function, obj_chunk_number=2)
         result = fexec.get_result()
-        self.assertEqual(result, self.__class__.words_in_cos_files)
+        assert result == self.words_in_files
 
     def test_chunks_bucket(self):
-        """tests the ability to create a separate function invocation based on the following parameters:
-         chunk_size - creates [file_size//chunk_size] invocations to process each chunk_size bytes, of a given object.
-         chunk_number - creates 'chunk_number' invocations that process [file_size//chunk_number] bytes each. """
+        """tests the ability to create a separate function invocation
+        based on the following parameters: chunk_size creates [file_size//chunk_size]
+        invocations to process each chunk_size bytes, of a given object. chunk_number
+        creates 'chunk_number' invocations that process [file_size//chunk_number] bytes each.
+        """
 
         logger.info('Testing chunks on a bucket')
         OBJ_CHUNK_SIZE = 1 * 800 ** 2  # create a new invocation
         OBJ_CHUNK_NUMBER = 2
         activations = 0
 
-        sb = STORAGE_CONFIG['backend']
-        data_prefix = sb + '://' + STORAGE_CONFIG['bucket'] + '/' + DATASET_PREFIX + '/'
+        data_prefix = self.storage_backend + '://' + self.bucket + '/' + DATASET_PREFIX + '/'
 
-        fexec = lithops.FunctionExecutor(config=CONFIG)
+        fexec = lithops.FunctionExecutor(config=pytest.lithops_config)
         futures = fexec.map_reduce(my_map_function_obj, data_prefix,
                                    my_reduce_function,
                                    obj_chunk_size=OBJ_CHUNK_SIZE)
         result = fexec.get_result(futures)
-        self.assertEqual(result, self.__class__.words_in_cos_files)
+        assert result == self.words_in_files
 
-        for size in get_dataset_key_size(STORAGE, STORAGE_CONFIG):
+        for size in get_dataset_key_size(self.storage, self.bucket):
             activations += math.ceil(size / OBJ_CHUNK_SIZE)
 
-        self.assertEqual(len(futures), activations + 1)  # +1 due to the reduce function
+        assert len(futures) == activations + 1  # +1 due to the reduce function
 
-        fexec = lithops.FunctionExecutor(config=CONFIG)
+        fexec = lithops.FunctionExecutor(config=pytest.lithops_config)
         futures = fexec.map_reduce(my_map_function_obj, data_prefix,
                                    my_reduce_function, obj_chunk_number=OBJ_CHUNK_NUMBER)
         result = fexec.get_result(futures)
-        self.assertEqual(result, self.__class__.words_in_cos_files)
+        assert result == self.words_in_files
 
-        self.assertEqual(len(futures), len(TEST_FILES_URLS) * OBJ_CHUNK_NUMBER + 1)
+        assert len(futures) == len(TEST_FILES_URLS) * OBJ_CHUNK_NUMBER + 1
 
     def test_chunks_bucket_one_reducer_per_object(self):
-        """tests the ability to create a separate function invocation based on the following parameters, as well as
-         create a separate invocation of a reduce function for each object:
-         chunk_size - creates [file_size//chunk_size] invocations to process each chunk_size bytes, of a given object.
-         chunk_number - creates 'chunk_number' invocations that process [file_size//chunk_number] bytes each. """
+        """tests the ability to create a separate function invocation based
+        on the following parameters, as well as create a separate invocation
+        of a reduce function for each object: chunk_size creates [file_size//chunk_size]
+        invocations to process each chunk_size bytes, of a given object. hunk_number
+        creates 'chunk_number' invocations that process [file_size//chunk_number] bytes each.
+        """
 
         logger.info('Testing chunks on a bucket with one reducer per object')
         OBJ_CHUNK_SIZE = 1 * 1024 ** 2
         OBJ_CHUNK_NUMBER = 2
         activations = 0
 
-        sb = STORAGE_CONFIG['backend']
-        data_prefix = sb + '://' + STORAGE_CONFIG['bucket'] + '/' + DATASET_PREFIX + '/'
+        data_prefix = self.storage_backend + '://' + self.bucket + '/' + DATASET_PREFIX + '/'
 
-        fexec = lithops.FunctionExecutor(config=CONFIG)
-        futures = fexec.map_reduce(my_map_function_obj, data_prefix,
-                                   my_reduce_function,
-                                   obj_chunk_size=OBJ_CHUNK_SIZE,
-                                   obj_reduce_by_key=True)
+        fexec = lithops.FunctionExecutor(config=pytest.lithops_config)
+        futures = fexec.map_reduce(
+            my_map_function_obj, data_prefix,
+            my_reduce_function,
+            obj_chunk_size=OBJ_CHUNK_SIZE,
+            obj_reduce_by_key=True
+        )
         result = fexec.get_result(futures)
-        self.assertEqual(sum(result), self.__class__.words_in_cos_files)
+        assert sum(result) == self.words_in_files
 
-        for size in get_dataset_key_size(STORAGE, STORAGE_CONFIG):
+        for size in get_dataset_key_size(self.storage, self.bucket):
             activations += math.ceil(size / OBJ_CHUNK_SIZE)
 
-        self.assertEqual(len(futures), activations + len(TEST_FILES_URLS))  # + len(TEST_FILES_URLS) due to map_reduce activation per object
+        # + len(TEST_FILES_URLS) due to map_reduce activation per object
+        assert len(futures) == activations + len(TEST_FILES_URLS)
 
-        fexec = lithops.FunctionExecutor(config=CONFIG)
-        futures = fexec.map_reduce(my_map_function_obj, data_prefix,
-                                   my_reduce_function, obj_chunk_number=OBJ_CHUNK_NUMBER,
-                                   obj_reduce_by_key=True)
+        fexec = lithops.FunctionExecutor(config=pytest.lithops_config)
+        futures = fexec.map_reduce(
+            my_map_function_obj,
+            data_prefix,
+            my_reduce_function,
+            obj_chunk_number=OBJ_CHUNK_NUMBER,
+            obj_reduce_by_key=True
+        )
         result = fexec.get_result(futures)
-        self.assertEqual(sum(result), self.__class__.words_in_cos_files)
-        self.assertEqual(len(futures), len(TEST_FILES_URLS) * OBJ_CHUNK_NUMBER + len(TEST_FILES_URLS))  # + len(TEST_FILES_URLS) due to map_reduce activation per object
+        assert sum(result) == self.words_in_files
+        # + len(TEST_FILES_URLS) due to map_reduce activation per object
+        assert len(futures) == len(TEST_FILES_URLS) * OBJ_CHUNK_NUMBER + len(TEST_FILES_URLS)
+
+
+def get_dataset_key_size(storage, bucket):
+    """return a list of file sizes in bytes, belonging to files whose names are
+    prefixed by 'prefix' """
+    sizes = []
+    keys = storage.list_keys(bucket=bucket, prefix=DATASET_PREFIX + '/')
+    for key in keys:
+        sizes.append(float(storage.head_object(bucket, key)['content-length']))
+    return sizes
+
+
+def upload_data_sets(storage):
+    """
+    Uploads datasets to storage and return a list of
+    the number of words within each test file
+    """
+    def up(param):
+        dataset_name = param[1].split("/")[-1]
+        logger.info(f'Uploading bag-of-words dataset: {dataset_name}')
+        i, url = param
+        content = urllib.request.urlopen(url).read()
+        storage.put_object(bucket=storage.bucket,
+                           key=f'{DATASET_PREFIX}/{dataset_name}',
+                           body=content)
+        return len(content.split())
+
+    with ThreadPoolExecutor() as pool:
+        results = list(pool.map(up, enumerate(TEST_FILES_URLS)))
+
+    return sum(results)
```

### Comparing `lithops-3.2.0/lithops/tests/test_storage.py` & `lithops-3.3.0/lithops/tests/test_storage.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,301 +10,281 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-
-import unittest
+import pytest
 import logging
+import lithops
 from io import BytesIO
+from lithops.config import extract_storage_config
 from lithops.storage.utils import CloudObject, StorageNoSuchKeyError
-import lithops
-from lithops.tests import main_util
-from lithops.tests.util_func.map_reduce_util import my_reduce_function
-from lithops.tests.util_func.storage_util import my_map_function_storage, \
-    my_cloudobject_put, my_cloudobject_get, list_dataset_keys, extract_keys
+from lithops.tests.conftest import TESTS_PREFIX
+from lithops.tests.functions import my_map_function_storage, \
+    my_cloudobject_put, my_cloudobject_get, my_reduce_function
+
 
 logger = logging.getLogger(__name__)
 
-CONFIG = None
-STORAGE_CONFIG = None
-STORAGE = None
-TEST_FILES_URLS = None
-PREFIX = '__lithops.test'
-DATASET_PREFIX = PREFIX + '/dataset'
+STORAGE_PREFIX = TESTS_PREFIX + '/storage'
 
 
-class TestStorage(unittest.TestCase):
-    words_in_cos_files = None
+class TestStorage:
 
     @classmethod
-    def setUpClass(cls):
-        global CONFIG, STORAGE, STORAGE_CONFIG, TEST_FILES_URLS
-
-        CONFIG, STORAGE, STORAGE_CONFIG = main_util.get_config().values()
-        TEST_FILES_URLS = main_util.get_data_sets()
-        cls.words_in_cos_files = main_util.get_words_in_files()
+    def setup_class(cls):
+        storage_config = extract_storage_config(pytest.lithops_config)
+        storage = lithops.Storage(storage_config=storage_config)
+        cls.storage = storage
+        cls.storage_backend = storage.backend
+        cls.bucket = storage.bucket
+        storage.put_object(cls.bucket, STORAGE_PREFIX + '/test0', BytesIO(b'test storage handler'))
+        storage.put_object(cls.bucket, STORAGE_PREFIX + '/test1', BytesIO(b'test storage'))
+        cls.words_in_files = 5
 
     @classmethod
-    def setUp(cls):
-        print('\n-------------------------------------------------------------\n')
+    def teardown_class(cls):
+        for key in cls.storage.list_keys(bucket=cls.bucket, prefix=STORAGE_PREFIX):
+            cls.storage.delete_object(bucket=cls.bucket, key=key)
 
     def test_storage_handler(self):
         logger.info('Testing "storage" function arg')
-        iterdata = [(key, STORAGE_CONFIG['bucket']) for key in list_dataset_keys(STORAGE, STORAGE_CONFIG)]
-        fexec = lithops.FunctionExecutor(config=CONFIG)
-        fexec.map_reduce(my_map_function_storage, iterdata,
-                         my_reduce_function)
+        keys = self.storage.list_keys(bucket=self.bucket, prefix=STORAGE_PREFIX)
+        iterdata = [(key, self.bucket) for key in keys]
+        fexec = lithops.FunctionExecutor(config=pytest.lithops_config)
+        fexec.map_reduce(my_map_function_storage, iterdata, my_reduce_function)
         result = fexec.get_result()
-        self.assertEqual(result, self.__class__.words_in_cos_files)
+        assert result == self.words_in_files
 
     def test_cloudobject(self):
         logger.info('Testing cloudobjects')
-        sb = STORAGE_CONFIG['backend']
-        data_prefix = sb + '://' + STORAGE_CONFIG['bucket'] + '/' + DATASET_PREFIX + '/'
-        with lithops.FunctionExecutor(config=CONFIG) as fexec:
+        data_prefix = self.storage_backend + '://' + self.bucket + '/' + STORAGE_PREFIX + '/'
+        with lithops.FunctionExecutor(config=pytest.lithops_config) as fexec:
             fexec.map(my_cloudobject_put, data_prefix)
             cloudobjects = fexec.get_result()
             fexec.call_async(my_cloudobject_get, cloudobjects)
             result = fexec.get_result()
-            self.assertEqual(result, self.__class__.words_in_cos_files)
+            assert result == self.words_in_files
             fexec.clean(cs=cloudobjects)
 
-    def test_storage_put_get_by_stream(self):
+    def test_put_get_by_stream(self):
         logger.info('Testing Storage.put_object and get_object with streams')
-        bucket = STORAGE_CONFIG['bucket']
-        bytes_data = b'123'
-        bytes_key = PREFIX + '/bytes'
 
-        STORAGE.put_object(bucket, bytes_key, BytesIO(bytes_data))
-        bytes_stream = STORAGE.get_object(bucket, bytes_key, stream=True)
+        bytes_data = b'123'
+        bytes_key = STORAGE_PREFIX + '/bytes'
+        self.storage.put_object(self.bucket, bytes_key, BytesIO(bytes_data))
+        bytes_stream = self.storage.get_object(self.bucket, bytes_key, stream=True)
 
-        self.assertTrue(hasattr(bytes_stream, 'read'))
-        self.assertEqual(bytes_stream.read(), bytes_data)
+        assert hasattr(bytes_stream, 'read')
+        assert bytes_stream.read() == bytes_data
 
-    def test_storage_get_by_range(self):
+    def test_get_by_range(self):
         logger.info('Testing Storage.get_object with Range argument')
-        bucket = STORAGE_CONFIG['bucket']
-        key = PREFIX + '/bytes'
-        STORAGE.put_object(bucket, key, b'0123456789')
+        key = STORAGE_PREFIX + '/bytes'
+        self.storage.put_object(self.bucket, key, b'0123456789')
 
-        result = STORAGE.get_object(bucket, key, extra_get_args={'Range': 'bytes=1-4'})
+        result = self.storage.get_object(self.bucket, key, extra_get_args={'Range': 'bytes=1-4'})
 
-        self.assertEqual(result, b'1234')
+        assert result == b'1234'
 
-    def test_storage_list_keys(self):
+    def test_list_keys(self):
         logger.info('Testing Storage.list_keys')
-        bucket = STORAGE_CONFIG['bucket']
         test_keys = sorted([
-            PREFIX + '/foo/baz',
-            PREFIX + '/foo/bar/baz',
-            PREFIX + '/foo_bar/baz',
-            PREFIX + '/foo_baz',
-            PREFIX + '/bar',
-            PREFIX + '/bar_baz',
+            STORAGE_PREFIX + '/foo/baz',
+            STORAGE_PREFIX + '/foo/bar/baz',
+            STORAGE_PREFIX + '/foo_bar/baz',
+            STORAGE_PREFIX + '/foo_baz',
+            STORAGE_PREFIX + '/bar',
+            STORAGE_PREFIX + '/bar_baz',
         ])
         for key in test_keys:
-            STORAGE.put_object(bucket, key, key.encode())
+            self.storage.put_object(self.bucket, key, key.encode())
 
-        all_bucket_keys = STORAGE.list_keys(bucket)
-        prefix_keys = STORAGE.list_keys(bucket, PREFIX)
-        foo_keys = STORAGE.list_keys(bucket, PREFIX + '/foo')
-        foo_slash_keys = STORAGE.list_keys(bucket, PREFIX + '/foo/')
-        bar_keys = STORAGE.list_keys(bucket, PREFIX + '/bar')
-        non_existent_keys = STORAGE.list_keys(bucket, PREFIX + '/doesnt_exist')
-
-        self.assertTrue(set(all_bucket_keys).issuperset(test_keys))
-        self.assertTrue(set(prefix_keys).issuperset(test_keys))
-        self.assertTrue(all(key.startswith(PREFIX) for key in prefix_keys))
-        # To ensure parity between filesystem and object storage implementations, test that
-        # prefixes are treated as textual prefixes, not directory names.
-        self.assertEqual(sorted(foo_keys), sorted([
-            PREFIX + '/foo/baz',
-            PREFIX + '/foo/bar/baz',
-            PREFIX + '/foo_bar/baz',
-            PREFIX + '/foo_baz',
-        ]))
-        self.assertEqual(sorted(foo_slash_keys), sorted([
-            PREFIX + '/foo/baz',
-            PREFIX + '/foo/bar/baz',
-        ]))
-        self.assertEqual(sorted(bar_keys), sorted([
-            PREFIX + '/bar',
-            PREFIX + '/bar_baz',
-        ]))
+        all_bucket_keys = self.storage.list_keys(self.bucket)
+        prefix_keys = self.storage.list_keys(self.bucket, STORAGE_PREFIX)
+        foo_keys = self.storage.list_keys(self.bucket, STORAGE_PREFIX + '/foo')
+        foo_slash_keys = self.storage.list_keys(self.bucket, STORAGE_PREFIX + '/foo/')
+        bar_keys = self.storage.list_keys(self.bucket, STORAGE_PREFIX + '/bar')
+        non_existent_keys = self.storage.list_keys(self.bucket, STORAGE_PREFIX + '/doesnt_exist')
+
+        assert set(all_bucket_keys).issuperset(test_keys)
+        assert set(prefix_keys).issuperset(test_keys)
+        assert all(key.startswith(STORAGE_PREFIX) for key in prefix_keys)
+        assert sorted(foo_keys) == sorted([
+            STORAGE_PREFIX + '/foo/baz',
+            STORAGE_PREFIX + '/foo/bar/baz',
+            STORAGE_PREFIX + '/foo_bar/baz',
+            STORAGE_PREFIX + '/foo_baz',
+        ])
+        assert sorted(foo_slash_keys) == sorted([
+            STORAGE_PREFIX + '/foo/baz',
+            STORAGE_PREFIX + '/foo/bar/baz',
+        ])
+        assert sorted(bar_keys) == sorted([
+            STORAGE_PREFIX + '/bar',
+            STORAGE_PREFIX + '/bar_baz',
+        ])
 
-        self.assertEqual(non_existent_keys, [])
+        assert non_existent_keys == []
 
-    def test_storage_head_object(self):
+    def test_head_object(self):
         logger.info('Testing Storage.head_object')
-        bucket = STORAGE_CONFIG['bucket']
         data = b'123456789'
-        STORAGE.put_object(bucket, PREFIX + '/data', data)
-
-        result = STORAGE.head_object(bucket, PREFIX + '/data')
-        self.assertEqual(result['content-length'], str(len(data)))
+        self.storage.put_object(self.bucket, STORAGE_PREFIX + '/data', data)
 
-        def get_nonexistent_object():
-            STORAGE.head_object(bucket, PREFIX + '/doesnt_exist')
+        result = self.storage.head_object(self.bucket, STORAGE_PREFIX + '/data')
+        assert result['content-length'] == str(len(data))
 
-        self.assertRaises(StorageNoSuchKeyError, get_nonexistent_object)
+        with pytest.raises(StorageNoSuchKeyError):
+            self.storage.head_object(self.bucket, STORAGE_PREFIX + '/doesnt_exist')
 
-    def test_storage_list_objects(self):
+    def test_list_objects(self):
         logger.info('Testing Storage.list_objects')
-        bucket = STORAGE_CONFIG['bucket']
         test_keys = sorted([
-            PREFIX + '/foo/baz',
-            PREFIX + '/foo/bar/baz',
-            PREFIX + '/foo_bar/baz',
-            PREFIX + '/foo_baz',
-            PREFIX + '/bar',
-            PREFIX + '/bar_baz',
+            STORAGE_PREFIX + '/foo/baz',
+            STORAGE_PREFIX + '/foo/bar/baz',
+            STORAGE_PREFIX + '/foo_bar/baz',
+            STORAGE_PREFIX + '/foo_baz',
+            STORAGE_PREFIX + '/bar',
+            STORAGE_PREFIX + '/bar_baz',
         ])
         for key in test_keys:
-            STORAGE.put_object(bucket, key, key.encode())
+            self.storage.put_object(self.bucket, key, key.encode())
 
-        all_bucket_objects = STORAGE.list_objects(bucket)
-        prefix_objects = STORAGE.list_objects(bucket, PREFIX)
-        foo_objects = STORAGE.list_objects(bucket, PREFIX + '/foo')
-        foo_slash_objects = STORAGE.list_objects(bucket, PREFIX + '/foo/')
-        bar_objects = STORAGE.list_objects(bucket, PREFIX + '/bar')
-        non_existent_objects = STORAGE.list_objects(bucket, PREFIX + '/doesnt_exist')
-
-        self.assertTrue(set(extract_keys(all_bucket_objects)).issuperset(test_keys))
-        self.assertTrue(set(extract_keys(prefix_objects)).issuperset(test_keys))
-        self.assertTrue(all(key.startswith(PREFIX) for key in extract_keys(prefix_objects)))
-        self.assertEqual(sorted(extract_keys(foo_objects)), sorted([
-            PREFIX + '/foo/baz',
-            PREFIX + '/foo/bar/baz',
-            PREFIX + '/foo_bar/baz',
-            PREFIX + '/foo_baz',
-        ]))
-        self.assertEqual(sorted(extract_keys(foo_slash_objects)), sorted([
-            PREFIX + '/foo/baz',
-            PREFIX + '/foo/bar/baz',
-        ]))
-        self.assertEqual(sorted(extract_keys(bar_objects)), sorted([
-            PREFIX + '/bar',
-            PREFIX + '/bar_baz',
-        ]))
+        all_bucket_objects = self.storage.list_objects(self.bucket)
+        prefix_objects = self.storage.list_objects(self.bucket, STORAGE_PREFIX)
+        foo_objects = self.storage.list_objects(self.bucket, STORAGE_PREFIX + '/foo')
+        foo_slash_objects = self.storage.list_objects(self.bucket, STORAGE_PREFIX + '/foo/')
+        bar_objects = self.storage.list_objects(self.bucket, STORAGE_PREFIX + '/bar')
+        non_existent_objects = self.storage.list_objects(self.bucket, STORAGE_PREFIX + '/doesnt_exist')
+
+        def extract_keys(bucket_objects):
+            keys = []
+            for obj in bucket_objects:
+                keys.append(obj['Key'])
+            return keys
+
+        assert set(extract_keys(all_bucket_objects)).issuperset(test_keys)
+        assert set(extract_keys(prefix_objects)).issuperset(test_keys)
+        assert all(key.startswith(STORAGE_PREFIX) for key in extract_keys(prefix_objects))
+        assert sorted(extract_keys(foo_objects)) == sorted([
+            STORAGE_PREFIX + '/foo/baz',
+            STORAGE_PREFIX + '/foo/bar/baz',
+            STORAGE_PREFIX + '/foo_bar/baz',
+            STORAGE_PREFIX + '/foo_baz',
+        ])
+        assert sorted(extract_keys(foo_slash_objects)) == sorted([
+            STORAGE_PREFIX + '/foo/baz',
+            STORAGE_PREFIX + '/foo/bar/baz',
+        ])
+        assert sorted(extract_keys(bar_objects)) == sorted([
+            STORAGE_PREFIX + '/bar',
+            STORAGE_PREFIX + '/bar_baz',
+        ])
 
-        self.assertEqual(non_existent_objects, [])
+        assert non_existent_objects == []
 
-    def test_storage_list_objects_size(self):
+    def test_list_objects_size(self):
         logger.info('Testing Storage.list_objects_size')
-        bucket = STORAGE_CONFIG['bucket']
-        isEqual = True
-
         test_keys = sorted([
-            PREFIX + '/foo/baz',
-            PREFIX + '/foo/bar/baz',
-            PREFIX + '/foo_bar/baz',
-            PREFIX + '/foo_baz',
-            PREFIX + '/bar',
-            PREFIX + '/bar_baz',
+            STORAGE_PREFIX + '/list/foo/baz',
+            STORAGE_PREFIX + '/list/foo/bar/baz',
+            STORAGE_PREFIX + '/list/foo_bar/baz',
+            STORAGE_PREFIX + '/list/foo_baz',
+            STORAGE_PREFIX + '/list/bar',
+            STORAGE_PREFIX + '/list/bar_baz',
         ])
         for key in test_keys:
-            STORAGE.put_object(bucket, key, key.encode())
+            self.storage.put_object(self.bucket, key, key.encode())
 
-        all_bucket_objects = STORAGE.list_objects(bucket)
-
-        for key in test_keys:
-            for obj in all_bucket_objects:
-                if obj['Key'] == key and obj['Size'] != len(key.encode()):
-                    isEqual = False
-        self.assertTrue(isEqual)
+        all_bucket_objects = self.storage.list_objects(self.bucket, prefix=STORAGE_PREFIX + '/list')
+        isEqual = all(obj['Size'] == len(obj['Key'].encode()) for obj in all_bucket_objects)
+        assert isEqual
 
     def test_delete_object(self):
         logger.info('Testing Storage.delete_object')
-        bucket = STORAGE_CONFIG['bucket']
         test_keys = sorted([
-            PREFIX + '/foo/baz',
-            PREFIX + '/foo/bar/baz',
-            PREFIX + '/foo_baz',
-            PREFIX + '/bar',
-            PREFIX + '/to_be_deleted',
+            STORAGE_PREFIX + '/delete/foo/baz',
+            STORAGE_PREFIX + '/foo/bar/baz',
+            STORAGE_PREFIX + '/foo_baz',
+            STORAGE_PREFIX + '/bar',
+            STORAGE_PREFIX + '/to_be_deleted',
         ])
         for key in test_keys:
-            STORAGE.put_object(bucket, key, key.encode())
+            self.storage.put_object(self.bucket, key, key.encode())
 
-        STORAGE.delete_object(bucket, PREFIX + '/to_be_deleted')
-        all_bucket_keys = STORAGE.list_keys(bucket)
-        self.assertFalse(PREFIX + '/to_be_deleted' in all_bucket_keys)
+        self.storage.delete_object(self.bucket, STORAGE_PREFIX + '/to_be_deleted')
+        all_bucket_keys = self.storage.list_keys(self.bucket)
+        assert STORAGE_PREFIX + '/to_be_deleted' not in all_bucket_keys
 
     def test_delete_objects(self):
         logger.info('Testing Storage.delete_objects')
-        bucket = STORAGE_CONFIG['bucket']
         test_keys = sorted([
-            PREFIX + '/foo/baz',
-            PREFIX + '/foo/bar/baz',
-            PREFIX + '/foo_baz',
-            PREFIX + '/bar',
-            PREFIX + '/to_be_deleted1',
-            PREFIX + '/to_be_deleted2',
-            PREFIX + '/to_be_deleted3'
+            STORAGE_PREFIX + '/foo/baz',
+            STORAGE_PREFIX + '/foo/bar/baz',
+            STORAGE_PREFIX + '/foo_baz',
+            STORAGE_PREFIX + '/bar',
+            STORAGE_PREFIX + '/to_be_deleted1',
+            STORAGE_PREFIX + '/to_be_deleted2',
+            STORAGE_PREFIX + '/to_be_deleted3'
         ])
         keys_to_delete = [
-            PREFIX + '/to_be_deleted1',
-            PREFIX + '/to_be_deleted2',
-            PREFIX + '/to_be_deleted3'
+            STORAGE_PREFIX + '/to_be_deleted1',
+            STORAGE_PREFIX + '/to_be_deleted2',
+            STORAGE_PREFIX + '/to_be_deleted3'
         ]
         for key in test_keys:
-            STORAGE.put_object(bucket, key, key.encode())
+            self.storage.put_object(self.bucket, key, key.encode())
 
-        STORAGE.delete_objects(bucket, keys_to_delete)
-        all_bucket_keys = STORAGE.list_keys(bucket)
-        self.assertTrue(all(key not in all_bucket_keys for key in keys_to_delete))
+        self.storage.delete_objects(self.bucket, keys_to_delete)
+        all_bucket_keys = self.storage.list_keys(self.bucket)
+        assert all(key not in all_bucket_keys for key in keys_to_delete)
 
     def test_head_bucket(self):
         logger.info('Testing Storage.head_bucket')
-        bucket = STORAGE_CONFIG['bucket']
-        result = STORAGE.head_bucket(bucket)
-        self.assertEqual(result['ResponseMetadata']['HTTPStatusCode'], 200)
+        result = self.storage.head_bucket(self.bucket)
+        assert result['ResponseMetadata']['HTTPStatusCode'] == 200
 
     def test_delete_cloudobject(self):
         logger.info('Testing Storage.delete_cloudobject')
-        sb = STORAGE_CONFIG['backend']
-        bucket = STORAGE_CONFIG['bucket']
         test_keys = sorted([
-            PREFIX + '/foo/baz',
-            PREFIX + '/foo/bar/baz',
-            PREFIX + '/foo_baz',
-            PREFIX + '/bar',
-            PREFIX + '/to_be_deleted',
+            STORAGE_PREFIX + '/foo/baz',
+            STORAGE_PREFIX + '/foo/bar/baz',
+            STORAGE_PREFIX + '/foo_baz',
+            STORAGE_PREFIX + '/bar',
+            STORAGE_PREFIX + '/to_be_deleted',
         ])
         for key in test_keys:
-            STORAGE.put_object(bucket, key, key.encode())
-        cloudobject = CloudObject(sb, bucket, PREFIX + '/to_be_deleted')
-        STORAGE.delete_cloudobject(cloudobject)
-        all_bucket_keys = STORAGE.list_keys(bucket)
-        self.assertFalse(PREFIX + '/to_be_deleted' in all_bucket_keys)
+            self.storage.put_object(self.bucket, key, key.encode())
+        cloudobject = CloudObject(self.storage_backend, self.bucket, STORAGE_PREFIX + '/to_be_deleted')
+        self.storage.delete_cloudobject(cloudobject)
+        all_bucket_keys = self.storage.list_keys(self.bucket)
+        assert STORAGE_PREFIX + '/to_be_deleted' not in all_bucket_keys
 
     def test_delete_cloudobjects(self):
         logger.info('Testing Storage.delete_cloudobjects')
-        sb = STORAGE_CONFIG['backend']
-        bucket = STORAGE_CONFIG['bucket']
         test_keys = sorted([
-            PREFIX + '/foo/baz',
-            PREFIX + '/foo/bar/baz',
-            PREFIX + '/foo_baz',
-            PREFIX + '/bar',
-            PREFIX + '/to_be_deleted1',
-            PREFIX + '/to_be_deleted2',
-            PREFIX + '/to_be_deleted3'
+            STORAGE_PREFIX + '/foo/baz',
+            STORAGE_PREFIX + '/foo/bar/baz',
+            STORAGE_PREFIX + '/foo_baz',
+            STORAGE_PREFIX + '/bar',
+            STORAGE_PREFIX + '/to_be_deleted1',
+            STORAGE_PREFIX + '/to_be_deleted2',
+            STORAGE_PREFIX + '/to_be_deleted3'
         ])
         cloudobjects = []
         keys_to_delete = [
-            PREFIX + '/to_be_deleted1',
-            PREFIX + '/to_be_deleted2',
-            PREFIX + '/to_be_deleted3'
+            STORAGE_PREFIX + '/to_be_deleted1',
+            STORAGE_PREFIX + '/to_be_deleted2',
+            STORAGE_PREFIX + '/to_be_deleted3'
         ]
         for key in keys_to_delete:
-            cobject = CloudObject(sb, bucket, key)
+            cobject = CloudObject(self.storage_backend, self.bucket, key)
             cloudobjects.append(cobject)
         for key in test_keys:
-            STORAGE.put_object(bucket, key, key.encode())
+            self.storage.put_object(self.bucket, key, key.encode())
 
-        STORAGE.delete_cloudobjects(cloudobjects)
-        all_bucket_keys = STORAGE.list_keys(bucket)
-        self.assertTrue(all(key not in all_bucket_keys for key in keys_to_delete))
+        self.storage.delete_cloudobjects(cloudobjects)
+        all_bucket_keys = self.storage.list_keys(self.bucket)
+        assert all(key not in all_bucket_keys for key in keys_to_delete)
```

### Comparing `lithops-3.2.0/lithops/util/ibm_token_manager.py` & `lithops-3.3.0/lithops/util/ibm_token_manager.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/util/joblib/lithops_backend.py` & `lithops-3.3.0/lithops/util/joblib/lithops_backend.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/util/metrics.py` & `lithops-3.3.0/lithops/util/metrics.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/util/ssh_client.py` & `lithops-3.3.0/lithops/util/ssh_client.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/utils.py` & `lithops-3.3.0/lithops/utils.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/wait.py` & `lithops-3.3.0/lithops/wait.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/worker/handler.py` & `lithops-3.3.0/lithops/worker/handler.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/worker/invoker.py` & `lithops-3.3.0/lithops/worker/invoker.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops/worker/jobrunner.py` & `lithops-3.3.0/lithops/worker/jobrunner.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 import time
 import pickle
 import logging
 import inspect
 import requests
 import traceback
 from pydoc import locate
-from distutils.util import strtobool
 
 from lithops.worker.utils import peak_memory
 
 try:
     import numpy as np
     np.__version__
 except ModuleNotFoundError:
@@ -206,15 +205,15 @@
         exception = False
         fn_name = None
 
         try:
             func = pickle.loads(self.job.func)
             data = pickle.loads(self.job.data)
 
-            if strtobool(os.environ.get('__LITHOPS_REDUCE_JOB', 'False')):
+            if eval(os.environ.get('__LITHOPS_REDUCE_JOB', 'False')):
                 self._wait_futures(data)
             elif is_object_processing_function(func):
                 self._load_object(data)
 
             self._fill_optional_args(func, data)
 
             fn_name = func.__name__ if inspect.isfunction(func) \
```

### Comparing `lithops-3.2.0/lithops/worker/status.py` & `lithops-3.3.0/lithops/worker/status.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import pika
 import json
 import time
 import logging
 from tblib import pickling_support
-from distutils.util import strtobool
 from contextlib import contextmanager
 
 import lithops.worker
 from lithops.utils import sizeof_fmt
 from lithops.storage.utils import create_status_key, \
     create_init_key
 
@@ -41,15 +40,15 @@
             'host_submit_tstamp': job.host_submit_tstamp,
             'call_id': job.call_id,
             'job_id': job.job_id,
             'executor_id': job.executor_id,
             'chunksize': job.chunksize
         }
 
-        if strtobool(os.environ.get('WARM_CONTAINER', 'False')):
+        if eval(os.environ.get('WARM_CONTAINER', 'False')):
             self.status['worker_cold_start'] = False
         else:
             self.status['worker_cold_start'] = True
             os.environ['WARM_CONTAINER'] = 'True'
 
     def add(self, key, value):
         """ Adds data to the call status"""
```

### Comparing `lithops-3.2.0/lithops/worker/utils.py` & `lithops-3.3.0/lithops/worker/utils.py`

 * *Files identical despite different names*

### Comparing `lithops-3.2.0/lithops.egg-info/PKG-INFO` & `lithops-3.3.0/lithops.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lithops
-Version: 3.2.0
+Version: 3.3.0
 Summary: Lithops lets you transparently run your Python applications in the Cloud
 Home-page: https://github.com/lithops-cloud/lithops
 Author: Gil Vernik, Josep Sampe
 Author-email: gilv@ibm.com, josep.sampe@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,11 +27,12 @@
 Provides-Extra: aliyun
 Provides-Extra: all
 Provides-Extra: azure
 Provides-Extra: gcp
 Provides-Extra: joblib
 Provides-Extra: multiprocessing
 Provides-Extra: oracle
+Provides-Extra: tests
 License-File: LICENSE
 
 UNKNOWN
```

### Comparing `lithops-3.2.0/lithops.egg-info/SOURCES.txt` & `lithops-3.3.0/lithops.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 lithops/config.py
 lithops/constants.py
 lithops/executors.py
 lithops/future.py
 lithops/invokers.py
 lithops/monitor.py
 lithops/plots.py
+lithops/retries.py
 lithops/utils.py
 lithops/version.py
 lithops/wait.py
 lithops.egg-info/PKG-INFO
 lithops.egg-info/SOURCES.txt
 lithops.egg-info/dependency_links.txt
 lithops.egg-info/entry_points.txt
@@ -23,14 +24,16 @@
 lithops/job/partitioner.py
 lithops/job/serialize.py
 lithops/libs/__init__.py
 lithops/libs/globber/__init__.py
 lithops/libs/globber/globber.py
 lithops/libs/imp/__init__.py
 lithops/libs/imp/imp.py
+lithops/libs/inspect/__init__.py
+lithops/libs/inspect/inspect.py
 lithops/libs/multyvac/__init__.py
 lithops/libs/multyvac/module_dependency.py
 lithops/libs/openwhisk/__init__.py
 lithops/libs/openwhisk/client.py
 lithops/localhost/__init__.py
 lithops/localhost/v1/__init__.py
 lithops/localhost/v1/localhost.py
@@ -169,25 +172,21 @@
 lithops/storage/backends/redis/__init__.py
 lithops/storage/backends/redis/config.py
 lithops/storage/backends/redis/redis.py
 lithops/storage/backends/swift/__init__.py
 lithops/storage/backends/swift/config.py
 lithops/storage/backends/swift/swift.py
 lithops/tests/__init__.py
-lithops/tests/main_util.py
+lithops/tests/conftest.py
+lithops/tests/functions.py
 lithops/tests/test_call_async.py
 lithops/tests/test_map.py
 lithops/tests/test_map_reduce.py
+lithops/tests/test_retries.py
 lithops/tests/test_storage.py
-lithops/tests/test_template.py
-lithops/tests/tests_main.py
-lithops/tests/util_func/__init__.py
-lithops/tests/util_func/map_reduce_util.py
-lithops/tests/util_func/map_util.py
-lithops/tests/util_func/storage_util.py
 lithops/util/__init__.py
 lithops/util/ibm_token_manager.py
 lithops/util/metrics.py
 lithops/util/ssh_client.py
 lithops/util/joblib/__init__.py
 lithops/util/joblib/lithops_backend.py
 lithops/worker/__init__.py
```

### Comparing `lithops-3.2.0/lithops.egg-info/requires.txt` & `lithops-3.3.0/lithops.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 google-cloud-storage
 httplib2
 joblib
 numpy
 oci
 oss2
 pynng
+pytest
 
 [azure]
 azure-identity
 azure-mgmt-compute
 azure-mgmt-network
 azure-mgmt-resource
 azure-storage-blob
@@ -68,7 +69,10 @@
 numpy
 
 [multiprocessing]
 pynng
 
 [oracle]
 oci
+
+[tests]
+pytest
```

### Comparing `lithops-3.2.0/setup.py` & `lithops-3.3.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -57,17 +57,21 @@
     'joblib': [
         'joblib',
         'diskcache',
         'numpy'
     ],
     'oracle': [
         'oci',
+    ],
+    'tests': [
+        'pytest',
     ]
 }
 
+
 extras_require["all"] = list(set(chain.from_iterable(extras_require.values())))
 
 
 # how to get version info into the project
 exec(open('lithops/version.py').read())
 setup(
     name='lithops',
```

