# Comparing `tmp/everai-0.1.34-py3-none-any.whl.zip` & `tmp/everai-0.1.35-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,31 +1,31 @@
-Zip file size: 418148 bytes, number of entries: 400
+Zip file size: 424700 bytes, number of entries: 407
 -rw-r--r--  2.0 unx       66 b- defN 24-Apr-24 07:43 everai/__init__.py
 -rw-r--r--  2.0 unx     1111 b- defN 24-Apr-24 07:49 everai/constants.py
--rw-r--r--  2.0 unx       23 b- defN 24-Apr-24 07:52 everai/version.py
+-rw-r--r--  2.0 unx       23 b- defN 24-Apr-24 12:38 everai/version.py
 -rw-r--r--  2.0 unx       40 b- defN 24-Mar-15 10:09 everai/api/__init__.py
--rw-r--r--  2.0 unx    14055 b- defN 24-Apr-23 15:30 everai/api/api.py
+-rw-r--r--  2.0 unx    14640 b- defN 24-Apr-24 09:55 everai/api/api.py
 -rw-r--r--  2.0 unx      208 b- defN 24-Apr-15 11:24 everai/app/__init__.py
 -rw-r--r--  2.0 unx     3667 b- defN 24-Apr-23 15:20 everai/app/app.py
--rw-r--r--  2.0 unx    11070 b- defN 24-Apr-24 07:48 everai/app/app_manager.py
+-rw-r--r--  2.0 unx    11207 b- defN 24-Apr-24 12:37 everai/app/app_manager.py
 -rw-r--r--  2.0 unx     1791 b- defN 24-Apr-24 07:37 everai/app/app_runner.py
 -rw-r--r--  2.0 unx     3223 b- defN 24-Apr-24 05:08 everai/app/app_runtime.py
 -rw-r--r--  2.0 unx     2568 b- defN 24-Apr-23 14:51 everai/app/app_setup.py
 -rw-r--r--  2.0 unx     1116 b- defN 24-Apr-24 04:14 everai/app/autocaling_handler.py
 -rw-r--r--  2.0 unx     2320 b- defN 24-Apr-23 14:26 everai/app/context.py
 -rw-r--r--  2.0 unx     2965 b- defN 24-Apr-23 09:42 everai/app/service.py
 -rw-r--r--  2.0 unx      210 b- defN 24-Mar-28 12:25 everai/app/typing.py
 -rw-r--r--  2.0 unx      327 b- defN 24-Mar-12 08:39 everai/app/volume_request.py
 -rw-r--r--  2.0 unx      310 b- defN 24-Apr-23 15:52 everai/autoscaling/__init__.py
 -rw-r--r--  2.0 unx      901 b- defN 24-Apr-23 13:29 everai/autoscaling/action.py
 -rw-r--r--  2.0 unx      291 b- defN 24-Apr-23 15:51 everai/autoscaling/autoscaling_policy.py
 -rw-r--r--  2.0 unx      184 b- defN 24-Apr-23 13:29 everai/autoscaling/autoscaling_policy.pyi
 -rw-r--r--  2.0 unx     1943 b- defN 24-Apr-23 08:23 everai/autoscaling/factors.py
 -rw-r--r--  2.0 unx      698 b- defN 24-Apr-16 13:43 everai/autoscaling/session_autoscaling.py
--rw-r--r--  2.0 unx     4666 b- defN 24-Apr-24 07:01 everai/autoscaling/simple_autoscaling.py
+-rw-r--r--  2.0 unx     4682 b- defN 24-Apr-24 12:35 everai/autoscaling/simple_autoscaling.py
 -rw-r--r--  2.0 unx       64 b- defN 24-Mar-29 07:34 everai/autoscaling/wellknown.py
 -rw-r--r--  2.0 unx       55 b- defN 24-Apr-23 06:48 everai/commands/__init__.py
 -rw-r--r--  2.0 unx     1683 b- defN 24-Apr-23 14:04 everai/commands/everai_cli.py
 -rw-r--r--  2.0 unx      163 b- defN 24-Apr-23 04:14 everai/commands/app/__init__.py
 -rw-r--r--  2.0 unx     1187 b- defN 24-Apr-24 06:26 everai/commands/app/app.py
 -rw-r--r--  2.0 unx     1407 b- defN 24-Apr-23 07:57 everai/commands/app/create.py
 -rw-r--r--  2.0 unx      676 b- defN 24-Apr-23 07:57 everai/commands/app/deploy.py
@@ -45,44 +45,47 @@
 -rw-r--r--  2.0 unx      405 b- defN 24-Apr-23 07:13 everai/commands/command/command.py
 -rw-r--r--  2.0 unx      362 b- defN 24-Apr-16 14:10 everai/commands/command/decorator.py
 -rw-r--r--  2.0 unx     2214 b- defN 24-Apr-23 12:53 everai/commands/command/list_utils.py
 -rw-r--r--  2.0 unx      341 b- defN 24-Apr-23 08:23 everai/commands/command/setup_subcommands.py
 -rw-r--r--  2.0 unx       62 b- defN 24-Apr-23 06:48 everai/commands/config/__init__.py
 -rw-r--r--  2.0 unx      701 b- defN 24-Apr-23 07:02 everai/commands/config/config.py
 -rw-r--r--  2.0 unx       72 b- defN 24-Apr-23 13:57 everai/commands/configmap/__init__.py
--rw-r--r--  2.0 unx     1289 b- defN 24-Apr-24 06:23 everai/commands/configmap/configmap.py
--rw-r--r--  2.0 unx     2008 b- defN 24-Apr-23 14:01 everai/commands/configmap/create.py
--rw-r--r--  2.0 unx      711 b- defN 24-Apr-23 13:59 everai/commands/configmap/delete.py
--rw-r--r--  2.0 unx      837 b- defN 24-Apr-23 14:03 everai/commands/configmap/get.py
--rw-r--r--  2.0 unx      723 b- defN 24-Apr-24 06:19 everai/commands/configmap/list.py
+-rw-r--r--  2.0 unx     1305 b- defN 24-Apr-24 10:45 everai/commands/configmap/configmap.py
+-rw-r--r--  2.0 unx     1995 b- defN 24-Apr-24 10:45 everai/commands/configmap/create.py
+-rw-r--r--  2.0 unx      693 b- defN 24-Apr-24 10:45 everai/commands/configmap/delete.py
+-rw-r--r--  2.0 unx      819 b- defN 24-Apr-24 10:45 everai/commands/configmap/get.py
+-rw-r--r--  2.0 unx      705 b- defN 24-Apr-24 10:45 everai/commands/configmap/list.py
+-rw-r--r--  2.0 unx     1995 b- defN 24-Apr-24 10:48 everai/commands/configmap/update.py
 -rw-r--r--  2.0 unx       60 b- defN 24-Apr-23 06:49 everai/commands/image/__init__.py
 -rw-r--r--  2.0 unx      734 b- defN 24-Apr-23 09:48 everai/commands/image/build.py
 -rw-r--r--  2.0 unx      831 b- defN 24-Apr-23 07:33 everai/commands/image/image.py
 -rw-r--r--  2.0 unx       54 b- defN 24-Apr-23 06:48 everai/commands/run/__init__.py
 -rw-r--r--  2.0 unx      925 b- defN 24-Apr-23 07:03 everai/commands/run/run.py
 -rw-r--r--  2.0 unx       63 b- defN 24-Apr-23 06:49 everai/commands/secret/__init__.py
--rw-r--r--  2.0 unx     1840 b- defN 24-Apr-23 07:05 everai/commands/secret/create.py
--rw-r--r--  2.0 unx      680 b- defN 24-Apr-23 07:05 everai/commands/secret/delete.py
--rw-r--r--  2.0 unx      965 b- defN 24-Apr-23 07:05 everai/commands/secret/get.py
--rw-r--r--  2.0 unx      777 b- defN 24-Apr-24 06:20 everai/commands/secret/list.py
--rw-r--r--  2.0 unx     1206 b- defN 24-Apr-24 06:23 everai/commands/secret/secret.py
+-rw-r--r--  2.0 unx     1833 b- defN 24-Apr-24 10:42 everai/commands/secret/create.py
+-rw-r--r--  2.0 unx      668 b- defN 24-Apr-24 10:41 everai/commands/secret/delete.py
+-rw-r--r--  2.0 unx      783 b- defN 24-Apr-24 10:43 everai/commands/secret/get.py
+-rw-r--r--  2.0 unx      765 b- defN 24-Apr-24 10:41 everai/commands/secret/list.py
+-rw-r--r--  2.0 unx     1243 b- defN 24-Apr-24 10:41 everai/commands/secret/secret.py
+-rw-r--r--  2.0 unx     1921 b- defN 24-Apr-24 10:40 everai/commands/secret/update.py
 -rw-r--r--  2.0 unx       63 b- defN 24-Apr-23 06:49 everai/commands/volume/__init__.py
 -rw-r--r--  2.0 unx      813 b- defN 24-Apr-23 07:08 everai/commands/volume/create.py
 -rw-r--r--  2.0 unx     1679 b- defN 24-Apr-23 07:09 everai/commands/volume/delete.py
 -rw-r--r--  2.0 unx      752 b- defN 24-Apr-23 07:09 everai/commands/volume/get.py
 -rw-r--r--  2.0 unx      747 b- defN 24-Apr-24 06:20 everai/commands/volume/list.py
 -rw-r--r--  2.0 unx     1507 b- defN 24-Apr-23 07:09 everai/commands/volume/pull.py
 -rw-r--r--  2.0 unx      753 b- defN 24-Apr-23 07:09 everai/commands/volume/push.py
 -rw-r--r--  2.0 unx     1395 b- defN 24-Apr-24 06:24 everai/commands/volume/volume.py
 -rw-r--r--  2.0 unx       69 b- defN 24-Apr-23 04:08 everai/commands/worker/__init__.py
 -rw-r--r--  2.0 unx      910 b- defN 24-Apr-24 06:22 everai/commands/worker/list.py
 -rw-r--r--  2.0 unx      851 b- defN 24-Apr-24 06:24 everai/commands/worker/worker.py
--rw-r--r--  2.0 unx      127 b- defN 24-Apr-23 13:53 everai/configmap/__init__.py
+-rw-r--r--  2.0 unx      270 b- defN 24-Apr-24 10:07 everai/configmap/__init__.py
 -rw-r--r--  2.0 unx     1498 b- defN 24-Apr-23 13:52 everai/configmap/configmap.py
--rw-r--r--  2.0 unx     1479 b- defN 24-Apr-23 13:55 everai/configmap/configmap_manager.py
+-rw-r--r--  2.0 unx     1848 b- defN 24-Apr-24 10:35 everai/configmap/configmap_manager.py
+-rw-r--r--  2.0 unx      741 b- defN 24-Apr-24 10:33 everai/configmap/utils.py
 -rw-r--r--  2.0 unx      157 b- defN 24-Mar-12 12:47 everai/image/__init__.py
 -rw-r--r--  2.0 unx      483 b- defN 24-Apr-09 08:31 everai/image/auth.py
 -rw-r--r--  2.0 unx     3317 b- defN 24-Apr-24 07:31 everai/image/builder.py
 -rw-r--r--  2.0 unx     1046 b- defN 24-Apr-17 14:47 everai/image/image.py
 -rw-r--r--  2.0 unx      223 b- defN 24-Apr-23 08:51 everai/logger/__init__.py
 -rw-r--r--  2.0 unx     1798 b- defN 24-Apr-23 08:57 everai/logger/logger.py
 -rw-r--r--  2.0 unx       70 b- defN 24-Apr-23 14:30 everai/placeholder/__init__.py
@@ -90,15 +93,15 @@
 -rw-r--r--  2.0 unx       79 b- defN 24-Apr-16 14:54 everai/resource_requests/__init__.py
 -rw-r--r--  2.0 unx     1686 b- defN 24-Apr-23 08:25 everai/resource_requests/resource_requests.py
 -rw-r--r--  2.0 unx      211 b- defN 24-Mar-29 07:26 everai/resource_requests/wellknown.py
 -rw-r--r--  2.0 unx       95 b- defN 24-Apr-23 03:58 everai/runner/__init__.py
 -rw-r--r--  2.0 unx     2403 b- defN 24-Apr-23 08:23 everai/runner/run.py
 -rw-r--r--  2.0 unx      109 b- defN 24-Apr-23 14:30 everai/secret/__init__.py
 -rw-r--r--  2.0 unx     2118 b- defN 24-Apr-23 13:11 everai/secret/secret.py
--rw-r--r--  2.0 unx     1484 b- defN 24-Apr-23 08:25 everai/secret/secret_manager.py
+-rw-r--r--  2.0 unx     1814 b- defN 24-Apr-24 10:36 everai/secret/secret_manager.py
 -rw-r--r--  2.0 unx       67 b- defN 24-Mar-12 09:57 everai/token_manager/__init__.py
 -rw-r--r--  2.0 unx     1547 b- defN 24-Apr-17 09:14 everai/token_manager/token_manager.py
 -rw-r--r--  2.0 unx       62 b- defN 24-Mar-07 07:15 everai/utils/__init__.py
 -rw-r--r--  2.0 unx      150 b- defN 24-Mar-29 07:04 everai/utils/bool.py
 -rw-r--r--  2.0 unx     1451 b- defN 24-Apr-23 08:23 everai/utils/cmd.py
 -rw-r--r--  2.0 unx      338 b- defN 24-Apr-15 14:59 everai/utils/datetime.py
 -rw-r--r--  2.0 unx     6189 b- defN 24-Apr-17 09:50 everai/utils/docker_manager.py
@@ -110,131 +113,133 @@
 -rw-r--r--  2.0 unx      616 b- defN 24-Mar-07 07:12 everai/utils/utils.py
 -rw-r--r--  2.0 unx      153 b- defN 24-Mar-14 15:31 everai/utils/verbose.py
 -rw-r--r--  2.0 unx      107 b- defN 24-Apr-02 06:47 everai/volume/__init__.py
 -rw-r--r--  2.0 unx     5148 b- defN 24-Apr-23 13:05 everai/volume/volume.py
 -rw-r--r--  2.0 unx    14731 b- defN 24-Apr-23 08:23 everai/volume/volume_manager.py
 -rw-r--r--  2.0 unx       55 b- defN 24-Apr-23 13:17 everai/worker/__init__.py
 -rw-r--r--  2.0 unx     1918 b- defN 24-Apr-23 13:19 everai/worker/worker.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 16:40 generated/__init__.py
--rw-r--r--  2.0 unx     1316 b- defN 24-Apr-23 16:40 generated/configmaps/__init__.py
--rw-r--r--  2.0 unx    29579 b- defN 24-Apr-23 16:40 generated/configmaps/api_client.py
--rw-r--r--  2.0 unx      852 b- defN 24-Apr-23 16:40 generated/configmaps/api_response.py
--rw-r--r--  2.0 unx    14419 b- defN 24-Apr-23 16:40 generated/configmaps/configuration.py
--rw-r--r--  2.0 unx     5462 b- defN 24-Apr-23 16:40 generated/configmaps/exceptions.py
--rw-r--r--  2.0 unx    12966 b- defN 24-Apr-23 16:40 generated/configmaps/rest.py
--rw-r--r--  2.0 unx      127 b- defN 24-Apr-23 16:40 generated/configmaps/api/__init__.py
--rw-r--r--  2.0 unx    25423 b- defN 24-Apr-23 16:40 generated/configmaps/api/configmap_service_api.py
--rw-r--r--  2.0 unx      639 b- defN 24-Apr-23 16:40 generated/configmaps/models/__init__.py
--rw-r--r--  2.0 unx     2555 b- defN 24-Apr-23 16:40 generated/configmaps/models/configmap_service_create_body.py
--rw-r--r--  2.0 unx     2764 b- defN 24-Apr-23 16:40 generated/configmaps/models/v1_configmap.py
--rw-r--r--  2.0 unx     2906 b- defN 24-Apr-23 16:40 generated/configmaps/models/v1_list_response.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 16:40 generated/configmaps/test/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 09:52 generated/__init__.py
+-rw-r--r--  2.0 unx     1413 b- defN 24-Apr-24 09:52 generated/configmaps/__init__.py
+-rw-r--r--  2.0 unx    29579 b- defN 24-Apr-24 09:52 generated/configmaps/api_client.py
+-rw-r--r--  2.0 unx      852 b- defN 24-Apr-24 09:52 generated/configmaps/api_response.py
+-rw-r--r--  2.0 unx    14419 b- defN 24-Apr-24 09:52 generated/configmaps/configuration.py
+-rw-r--r--  2.0 unx     5462 b- defN 24-Apr-24 09:52 generated/configmaps/exceptions.py
+-rw-r--r--  2.0 unx    12966 b- defN 24-Apr-24 09:52 generated/configmaps/rest.py
+-rw-r--r--  2.0 unx      127 b- defN 24-Apr-24 09:52 generated/configmaps/api/__init__.py
+-rw-r--r--  2.0 unx    32156 b- defN 24-Apr-24 09:52 generated/configmaps/api/configmap_service_api.py
+-rw-r--r--  2.0 unx      736 b- defN 24-Apr-24 09:52 generated/configmaps/models/__init__.py
+-rw-r--r--  2.0 unx     2555 b- defN 24-Apr-24 09:52 generated/configmaps/models/configmap_service_create_body.py
+-rw-r--r--  2.0 unx     2555 b- defN 24-Apr-24 09:52 generated/configmaps/models/configmap_service_update_body.py
+-rw-r--r--  2.0 unx     2764 b- defN 24-Apr-24 09:52 generated/configmaps/models/v1_configmap.py
+-rw-r--r--  2.0 unx     2906 b- defN 24-Apr-24 09:52 generated/configmaps/models/v1_list_response.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 09:52 generated/configmaps/test/__init__.py
 -rw-r--r--  2.0 unx     1357 b- defN 24-Apr-23 13:37 generated/configmaps/test/test_configmap_service_api.py
 -rw-r--r--  2.0 unx     1824 b- defN 24-Apr-23 13:37 generated/configmaps/test/test_configmap_service_create_body.py
+-rw-r--r--  2.0 unx     1824 b- defN 24-Apr-24 09:52 generated/configmaps/test/test_configmap_service_update_body.py
 -rw-r--r--  2.0 unx     1775 b- defN 24-Apr-23 13:37 generated/configmaps/test/test_v1_configmap.py
 -rw-r--r--  2.0 unx     1930 b- defN 24-Apr-23 13:37 generated/configmaps/test/test_v1_list_response.py
--rw-r--r--  2.0 unx     6396 b- defN 24-Apr-23 16:40 generated/schedulers/__init__.py
--rw-r--r--  2.0 unx    29587 b- defN 24-Apr-23 16:40 generated/schedulers/api_client.py
--rw-r--r--  2.0 unx      852 b- defN 24-Apr-23 16:40 generated/schedulers/api_response.py
--rw-r--r--  2.0 unx    14427 b- defN 24-Apr-23 16:40 generated/schedulers/configuration.py
--rw-r--r--  2.0 unx     5470 b- defN 24-Apr-23 16:40 generated/schedulers/exceptions.py
--rw-r--r--  2.0 unx    12974 b- defN 24-Apr-23 16:40 generated/schedulers/rest.py
--rw-r--r--  2.0 unx      115 b- defN 24-Apr-23 16:40 generated/schedulers/api/__init__.py
--rw-r--r--  2.0 unx    76636 b- defN 24-Apr-23 16:40 generated/schedulers/api/app_service_api.py
--rw-r--r--  2.0 unx     5731 b- defN 24-Apr-23 16:40 generated/schedulers/models/__init__.py
--rw-r--r--  2.0 unx     2744 b- defN 24-Apr-23 16:40 generated/schedulers/models/app_service_create_body.py
+-rw-r--r--  2.0 unx     6396 b- defN 24-Apr-24 09:52 generated/schedulers/__init__.py
+-rw-r--r--  2.0 unx    29587 b- defN 24-Apr-24 09:52 generated/schedulers/api_client.py
+-rw-r--r--  2.0 unx      852 b- defN 24-Apr-24 09:52 generated/schedulers/api_response.py
+-rw-r--r--  2.0 unx    14427 b- defN 24-Apr-24 09:52 generated/schedulers/configuration.py
+-rw-r--r--  2.0 unx     5470 b- defN 24-Apr-24 09:52 generated/schedulers/exceptions.py
+-rw-r--r--  2.0 unx    12974 b- defN 24-Apr-24 09:52 generated/schedulers/rest.py
+-rw-r--r--  2.0 unx      115 b- defN 24-Apr-24 09:52 generated/schedulers/api/__init__.py
+-rw-r--r--  2.0 unx    76636 b- defN 24-Apr-24 09:52 generated/schedulers/api/app_service_api.py
+-rw-r--r--  2.0 unx     5731 b- defN 24-Apr-24 09:52 generated/schedulers/models/__init__.py
+-rw-r--r--  2.0 unx     2744 b- defN 24-Apr-24 09:52 generated/schedulers/models/app_service_create_body.py
 -rw-r--r--  2.0 unx     3417 b- defN 24-Apr-17 14:31 generated/schedulers/models/app_service_inference_body.py
 -rw-r--r--  2.0 unx     2962 b- defN 24-Apr-09 08:31 generated/schedulers/models/app_service_resources_body.py
--rw-r--r--  2.0 unx     2951 b- defN 24-Apr-23 16:40 generated/schedulers/models/app_service_setup_auto_scaling_policy_body.py
+-rw-r--r--  2.0 unx     2951 b- defN 24-Apr-24 09:52 generated/schedulers/models/app_service_setup_auto_scaling_policy_body.py
 -rw-r--r--  2.0 unx     2691 b- defN 24-Apr-02 07:19 generated/schedulers/models/app_service_setup_body.py
 -rw-r--r--  2.0 unx     2978 b- defN 24-Apr-09 08:31 generated/schedulers/models/app_service_setup_resource_body.py
--rw-r--r--  2.0 unx     2859 b- defN 24-Apr-23 16:40 generated/schedulers/models/app_service_setup_resources_body.py
--rw-r--r--  2.0 unx     2532 b- defN 24-Apr-23 16:40 generated/schedulers/models/app_service_setup_secrets_body.py
--rw-r--r--  2.0 unx     3023 b- defN 24-Apr-23 16:40 generated/schedulers/models/app_service_setup_volumes_body.py
+-rw-r--r--  2.0 unx     2859 b- defN 24-Apr-24 09:52 generated/schedulers/models/app_service_setup_resources_body.py
+-rw-r--r--  2.0 unx     2532 b- defN 24-Apr-24 09:52 generated/schedulers/models/app_service_setup_secrets_body.py
+-rw-r--r--  2.0 unx     3023 b- defN 24-Apr-24 09:52 generated/schedulers/models/app_service_setup_volumes_body.py
 -rw-r--r--  2.0 unx     2523 b- defN 24-Mar-29 07:39 generated/schedulers/models/appsv1_cpu.py
 -rw-r--r--  2.0 unx     2884 b- defN 24-Mar-29 07:39 generated/schedulers/models/appsv1_gpu.py
--rw-r--r--  2.0 unx     3074 b- defN 24-Apr-23 16:40 generated/schedulers/models/appsv1_setup_image.py
--rw-r--r--  2.0 unx     3044 b- defN 24-Apr-23 16:40 generated/schedulers/models/appsv1_worker.py
--rw-r--r--  2.0 unx     6639 b- defN 24-Apr-23 16:40 generated/schedulers/models/protobuf_any.py
--rw-r--r--  2.0 unx      928 b- defN 24-Apr-23 16:40 generated/schedulers/models/rule_behavior.py
+-rw-r--r--  2.0 unx     3074 b- defN 24-Apr-24 09:52 generated/schedulers/models/appsv1_setup_image.py
+-rw-r--r--  2.0 unx     3044 b- defN 24-Apr-24 09:52 generated/schedulers/models/appsv1_worker.py
+-rw-r--r--  2.0 unx     6639 b- defN 24-Apr-24 09:52 generated/schedulers/models/protobuf_any.py
+-rw-r--r--  2.0 unx      928 b- defN 24-Apr-24 09:52 generated/schedulers/models/rule_behavior.py
 -rw-r--r--  2.0 unx     2872 b- defN 24-Mar-29 07:39 generated/schedulers/models/schedulerv1_cpu.py
 -rw-r--r--  2.0 unx     3361 b- defN 24-Mar-29 07:39 generated/schedulers/models/schedulerv1_gpu.py
--rw-r--r--  2.0 unx     3551 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_app.py
--rw-r--r--  2.0 unx     2825 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_app_service_setup_image_body.py
--rw-r--r--  2.0 unx     1151 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_app_status.py
--rw-r--r--  2.0 unx     3371 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_autoscaling_policy.py
--rw-r--r--  2.0 unx     3073 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_bandwidth.py
--rw-r--r--  2.0 unx     2483 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_bandwidth_size.py
--rw-r--r--  2.0 unx     3086 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_basic_auth.py
+-rw-r--r--  2.0 unx     3551 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_app.py
+-rw-r--r--  2.0 unx     2825 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_app_service_setup_image_body.py
+-rw-r--r--  2.0 unx     1151 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_app_status.py
+-rw-r--r--  2.0 unx     3371 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_autoscaling_policy.py
+-rw-r--r--  2.0 unx     3073 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_bandwidth.py
+-rw-r--r--  2.0 unx     2483 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_bandwidth_size.py
+-rw-r--r--  2.0 unx     3086 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_basic_auth.py
 -rw-r--r--  2.0 unx     3086 b- defN 24-Apr-09 08:31 generated/schedulers/models/v1_build_in_policy.py
--rw-r--r--  2.0 unx     2965 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_built_in_policy.py
--rw-r--r--  2.0 unx     2836 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_cpu.py
--rw-r--r--  2.0 unx     2984 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_create_volume_request.py
--rw-r--r--  2.0 unx     2876 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_create_volume_response.py
--rw-r--r--  2.0 unx     2849 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_custom_policy.py
--rw-r--r--  2.0 unx     2987 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_delete_volume_request.py
+-rw-r--r--  2.0 unx     2965 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_built_in_policy.py
+-rw-r--r--  2.0 unx     2836 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_cpu.py
+-rw-r--r--  2.0 unx     2984 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_create_volume_request.py
+-rw-r--r--  2.0 unx     2876 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_create_volume_response.py
+-rw-r--r--  2.0 unx     2849 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_custom_policy.py
+-rw-r--r--  2.0 unx     2987 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_delete_volume_request.py
 -rw-r--r--  2.0 unx     2612 b- defN 24-Mar-29 08:50 generated/schedulers/models/v1_delete_volume_response.py
--rw-r--r--  2.0 unx     4796 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_device_resource.py
--rw-r--r--  2.0 unx     2449 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_empty_response.py
--rw-r--r--  2.0 unx     2753 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_error_response.py
--rw-r--r--  2.0 unx     3247 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_filesystem.py
--rw-r--r--  2.0 unx     2546 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_get_image_request.py
--rw-r--r--  2.0 unx     2847 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_get_image_response.py
--rw-r--r--  2.0 unx     2624 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_get_volume_request.py
--rw-r--r--  2.0 unx     2864 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_get_volume_response.py
--rw-r--r--  2.0 unx     2518 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_get_worker_request.py
--rw-r--r--  2.0 unx     2900 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_get_worker_response.py
--rw-r--r--  2.0 unx     3325 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_gpu.py
--rw-r--r--  2.0 unx     2499 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_gpu_opts.py
--rw-r--r--  2.0 unx     2508 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_header_entry.py
--rw-r--r--  2.0 unx     3320 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_image.py
--rw-r--r--  2.0 unx     4574 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_image_request.py
--rw-r--r--  2.0 unx      917 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_image_status.py
+-rw-r--r--  2.0 unx     4796 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_device_resource.py
+-rw-r--r--  2.0 unx     2449 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_empty_response.py
+-rw-r--r--  2.0 unx     2753 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_error_response.py
+-rw-r--r--  2.0 unx     3247 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_filesystem.py
+-rw-r--r--  2.0 unx     2546 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_get_image_request.py
+-rw-r--r--  2.0 unx     2847 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_get_image_response.py
+-rw-r--r--  2.0 unx     2624 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_get_volume_request.py
+-rw-r--r--  2.0 unx     2864 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_get_volume_response.py
+-rw-r--r--  2.0 unx     2518 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_get_worker_request.py
+-rw-r--r--  2.0 unx     2900 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_get_worker_response.py
+-rw-r--r--  2.0 unx     3325 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_gpu.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_gpu_opts.py
+-rw-r--r--  2.0 unx     2508 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_header_entry.py
+-rw-r--r--  2.0 unx     3320 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_image.py
+-rw-r--r--  2.0 unx     4574 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_image_request.py
+-rw-r--r--  2.0 unx      917 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_image_status.py
 -rw-r--r--  2.0 unx     3436 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_inference_response.py
--rw-r--r--  2.0 unx     2924 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_list_image_request.py
--rw-r--r--  2.0 unx     3033 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_list_image_response.py
--rw-r--r--  2.0 unx     2836 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_list_response.py
--rw-r--r--  2.0 unx     2863 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_list_volume_request.py
--rw-r--r--  2.0 unx     3050 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_list_volume_response.py
--rw-r--r--  2.0 unx     2731 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_list_worker_request.py
--rw-r--r--  2.0 unx     3086 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_list_worker_response.py
--rw-r--r--  2.0 unx     2919 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_list_workers_response.py
--rw-r--r--  2.0 unx     3274 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_pull_image_request.py
--rw-r--r--  2.0 unx     2851 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_pull_image_response.py
--rw-r--r--  2.0 unx     2875 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_remove_image_request.py
--rw-r--r--  2.0 unx     3828 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_resource_claim.py
--rw-r--r--  2.0 unx     3190 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_resources.py
--rw-r--r--  2.0 unx     2616 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_restart_worker_request.py
--rw-r--r--  2.0 unx     4381 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_route_request.py
--rw-r--r--  2.0 unx     3056 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_rule.py
--rw-r--r--  2.0 unx     4243 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_run_worker_request.py
--rw-r--r--  2.0 unx     2924 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_run_worker_response.py
+-rw-r--r--  2.0 unx     2924 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_list_image_request.py
+-rw-r--r--  2.0 unx     3033 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_list_image_response.py
+-rw-r--r--  2.0 unx     2836 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_list_response.py
+-rw-r--r--  2.0 unx     2863 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_list_volume_request.py
+-rw-r--r--  2.0 unx     3050 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_list_volume_response.py
+-rw-r--r--  2.0 unx     2731 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_list_worker_request.py
+-rw-r--r--  2.0 unx     3086 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_list_worker_response.py
+-rw-r--r--  2.0 unx     2919 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_list_workers_response.py
+-rw-r--r--  2.0 unx     3274 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_pull_image_request.py
+-rw-r--r--  2.0 unx     2851 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_pull_image_response.py
+-rw-r--r--  2.0 unx     2875 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_remove_image_request.py
+-rw-r--r--  2.0 unx     3828 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_resource_claim.py
+-rw-r--r--  2.0 unx     3190 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_resources.py
+-rw-r--r--  2.0 unx     2616 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_restart_worker_request.py
+-rw-r--r--  2.0 unx     4381 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_route_request.py
+-rw-r--r--  2.0 unx     3056 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_rule.py
+-rw-r--r--  2.0 unx     4243 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_run_worker_request.py
+-rw-r--r--  2.0 unx     2924 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_run_worker_response.py
 -rw-r--r--  2.0 unx     4848 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setting.py
 -rw-r--r--  2.0 unx     3058 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setup_image.py
 -rw-r--r--  2.0 unx     2518 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setup_secrets.py
--rw-r--r--  2.0 unx     2764 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_setup_volume.py
+-rw-r--r--  2.0 unx     2764 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_setup_volume.py
 -rw-r--r--  2.0 unx     2925 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setup_volumes.py
 -rw-r--r--  2.0 unx     2890 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setup_volumes_volume.py
--rw-r--r--  2.0 unx     2749 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_stop_worker_request.py
--rw-r--r--  2.0 unx     2475 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_storage_size.py
--rw-r--r--  2.0 unx     2966 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_sync_volume_request.py
+-rw-r--r--  2.0 unx     2749 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_stop_worker_request.py
+-rw-r--r--  2.0 unx     2475 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_storage_size.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_sync_volume_request.py
 -rw-r--r--  2.0 unx     2604 b- defN 24-Mar-29 08:50 generated/schedulers/models/v1_sync_volume_response.py
--rw-r--r--  2.0 unx     2504 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_value_from_secret.py
--rw-r--r--  2.0 unx     3517 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_volume.py
--rw-r--r--  2.0 unx     2576 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_volume_mount.py
--rw-r--r--  2.0 unx     5229 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_volume_request.py
--rw-r--r--  2.0 unx      970 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_volume_status.py
+-rw-r--r--  2.0 unx     2504 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_value_from_secret.py
+-rw-r--r--  2.0 unx     3517 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_volume.py
+-rw-r--r--  2.0 unx     2576 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_volume_mount.py
+-rw-r--r--  2.0 unx     5229 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_volume_request.py
+-rw-r--r--  2.0 unx      970 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_volume_status.py
 -rw-r--r--  2.0 unx     3049 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_worker.py
--rw-r--r--  2.0 unx     5201 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_worker_request.py
+-rw-r--r--  2.0 unx     5201 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_worker_request.py
 -rw-r--r--  2.0 unx     1052 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_worker_status.py
--rw-r--r--  2.0 unx     1128 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1_worker_worker_status.py
--rw-r--r--  2.0 unx     3106 b- defN 24-Apr-23 16:40 generated/schedulers/models/v1workersv1_worker.py
+-rw-r--r--  2.0 unx     1128 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1_worker_worker_status.py
+-rw-r--r--  2.0 unx     3106 b- defN 24-Apr-24 09:52 generated/schedulers/models/v1workersv1_worker.py
 -rw-r--r--  2.0 unx     3439 b- defN 24-Apr-02 07:19 generated/schedulers/models/volumesv1_volume.py
--rw-r--r--  2.0 unx     1073 b- defN 24-Apr-23 16:40 generated/schedulers/models/workersv1_worker_status.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 16:40 generated/schedulers/test/__init__.py
+-rw-r--r--  2.0 unx     1073 b- defN 24-Apr-24 09:52 generated/schedulers/models/workersv1_worker_status.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 09:52 generated/schedulers/test/__init__.py
 -rw-r--r--  2.0 unx     1668 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_app_service_api.py
 -rw-r--r--  2.0 unx     1602 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_app_service_create_body.py
 -rw-r--r--  2.0 unx     1763 b- defN 24-Apr-17 14:12 generated/schedulers/test/test_app_service_inference_body.py
 -rw-r--r--  2.0 unx     2887 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_app_service_resources_body.py
 -rw-r--r--  2.0 unx     3598 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_app_service_setup_auto_scaling_policy_body.py
 -rw-r--r--  2.0 unx     7883 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_app_service_setup_body.py
 -rw-r--r--  2.0 unx     2936 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_app_service_setup_resource_body.py
@@ -317,63 +322,65 @@
 -rw-r--r--  2.0 unx     1891 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_worker.py
 -rw-r--r--  2.0 unx     2991 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_worker_request.py
 -rw-r--r--  2.0 unx      793 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_worker_status.py
 -rw-r--r--  2.0 unx      836 b- defN 24-Apr-23 15:39 generated/schedulers/test/test_v1_worker_worker_status.py
 -rw-r--r--  2.0 unx     1999 b- defN 24-Apr-22 10:29 generated/schedulers/test/test_v1workersv1_worker.py
 -rw-r--r--  2.0 unx     1576 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_volumesv1_volume.py
 -rw-r--r--  2.0 unx      842 b- defN 24-Apr-23 15:39 generated/schedulers/test/test_workersv1_worker_status.py
--rw-r--r--  2.0 unx     1256 b- defN 24-Apr-23 16:40 generated/secrets/__init__.py
--rw-r--r--  2.0 unx    29558 b- defN 24-Apr-23 16:40 generated/secrets/api_client.py
--rw-r--r--  2.0 unx      852 b- defN 24-Apr-23 16:40 generated/secrets/api_response.py
--rw-r--r--  2.0 unx    14413 b- defN 24-Apr-23 16:40 generated/secrets/configuration.py
--rw-r--r--  2.0 unx     5459 b- defN 24-Apr-23 16:40 generated/secrets/exceptions.py
--rw-r--r--  2.0 unx    12960 b- defN 24-Apr-23 16:40 generated/secrets/rest.py
--rw-r--r--  2.0 unx      118 b- defN 24-Apr-23 16:40 generated/secrets/api/__init__.py
--rw-r--r--  2.0 unx    25093 b- defN 24-Apr-23 16:40 generated/secrets/api/secret_service_api.py
--rw-r--r--  2.0 unx      615 b- defN 24-Apr-23 16:40 generated/secrets/models/__init__.py
--rw-r--r--  2.0 unx     2540 b- defN 24-Apr-23 16:40 generated/secrets/models/secret_service_create_body.py
--rw-r--r--  2.0 unx     2861 b- defN 24-Apr-23 16:40 generated/secrets/models/v1_list_response.py
--rw-r--r--  2.0 unx     2749 b- defN 24-Apr-23 16:40 generated/secrets/models/v1_secret.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 16:40 generated/secrets/test/__init__.py
+-rw-r--r--  2.0 unx     1344 b- defN 24-Apr-24 09:52 generated/secrets/__init__.py
+-rw-r--r--  2.0 unx    29558 b- defN 24-Apr-24 09:52 generated/secrets/api_client.py
+-rw-r--r--  2.0 unx      852 b- defN 24-Apr-24 09:52 generated/secrets/api_response.py
+-rw-r--r--  2.0 unx    14413 b- defN 24-Apr-24 09:52 generated/secrets/configuration.py
+-rw-r--r--  2.0 unx     5459 b- defN 24-Apr-24 09:52 generated/secrets/exceptions.py
+-rw-r--r--  2.0 unx    12960 b- defN 24-Apr-24 09:52 generated/secrets/rest.py
+-rw-r--r--  2.0 unx      118 b- defN 24-Apr-24 09:52 generated/secrets/api/__init__.py
+-rw-r--r--  2.0 unx    31721 b- defN 24-Apr-24 09:52 generated/secrets/api/secret_service_api.py
+-rw-r--r--  2.0 unx      703 b- defN 24-Apr-24 09:52 generated/secrets/models/__init__.py
+-rw-r--r--  2.0 unx     2540 b- defN 24-Apr-24 09:52 generated/secrets/models/secret_service_create_body.py
+-rw-r--r--  2.0 unx     2540 b- defN 24-Apr-24 09:52 generated/secrets/models/secret_service_update_body.py
+-rw-r--r--  2.0 unx     2861 b- defN 24-Apr-24 09:52 generated/secrets/models/v1_list_response.py
+-rw-r--r--  2.0 unx     2749 b- defN 24-Apr-24 09:52 generated/secrets/models/v1_secret.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 09:52 generated/secrets/test/__init__.py
 -rw-r--r--  2.0 unx     1297 b- defN 24-Mar-28 14:39 generated/secrets/test/test_secret_service_api.py
 -rw-r--r--  2.0 unx     1680 b- defN 24-Mar-28 14:39 generated/secrets/test/test_secret_service_create_body.py
+-rw-r--r--  2.0 unx     1782 b- defN 24-Apr-24 09:52 generated/secrets/test/test_secret_service_update_body.py
 -rw-r--r--  2.0 unx     1845 b- defN 24-Mar-28 14:39 generated/secrets/test/test_v1_list_response.py
 -rw-r--r--  2.0 unx     1603 b- defN 24-Mar-28 14:39 generated/secrets/test/test_v1_secret.py
--rw-r--r--  2.0 unx     2928 b- defN 24-Apr-23 16:40 generated/volumes/__init__.py
--rw-r--r--  2.0 unx    29558 b- defN 24-Apr-23 16:40 generated/volumes/api_client.py
--rw-r--r--  2.0 unx      852 b- defN 24-Apr-23 16:40 generated/volumes/api_response.py
--rw-r--r--  2.0 unx    14413 b- defN 24-Apr-23 16:40 generated/volumes/configuration.py
--rw-r--r--  2.0 unx     5459 b- defN 24-Apr-23 16:40 generated/volumes/exceptions.py
--rw-r--r--  2.0 unx    12960 b- defN 24-Apr-23 16:40 generated/volumes/rest.py
--rw-r--r--  2.0 unx      118 b- defN 24-Apr-23 16:40 generated/volumes/api/__init__.py
--rw-r--r--  2.0 unx   119008 b- defN 24-Apr-23 16:40 generated/volumes/api/volume_service_api.py
--rw-r--r--  2.0 unx     2287 b- defN 24-Apr-23 16:40 generated/volumes/models/__init__.py
--rw-r--r--  2.0 unx     2991 b- defN 24-Apr-23 16:40 generated/volumes/models/file_information.py
--rw-r--r--  2.0 unx     2986 b- defN 24-Apr-23 16:40 generated/volumes/models/v1_file.py
--rw-r--r--  2.0 unx     2415 b- defN 24-Apr-23 16:40 generated/volumes/models/v1_header_value.py
--rw-r--r--  2.0 unx     2728 b- defN 24-Apr-23 16:40 generated/volumes/models/v1_initialize_multipart_upload_response.py
--rw-r--r--  2.0 unx     2855 b- defN 24-Apr-23 16:40 generated/volumes/models/v1_list_files_response.py
--rw-r--r--  2.0 unx     2855 b- defN 24-Apr-23 16:40 generated/volumes/models/v1_list_parts_response.py
--rw-r--r--  2.0 unx     2861 b- defN 24-Apr-23 16:40 generated/volumes/models/v1_list_response.py
--rw-r--r--  2.0 unx     2592 b- defN 24-Apr-23 16:40 generated/volumes/models/v1_part.py
--rw-r--r--  2.0 unx     2897 b- defN 24-Apr-23 16:40 generated/volumes/models/v1_revision.py
--rw-r--r--  2.0 unx     3193 b- defN 24-Apr-23 16:40 generated/volumes/models/v1_sign_response.py
--rw-r--r--  2.0 unx     2910 b- defN 24-Apr-23 16:40 generated/volumes/models/v1_sign_upload_response.py
--rw-r--r--  2.0 unx      901 b- defN 24-Apr-23 16:40 generated/volumes/models/v1_upload_action.py
--rw-r--r--  2.0 unx     3159 b- defN 24-Apr-23 16:40 generated/volumes/models/v1_volume.py
--rw-r--r--  2.0 unx     2517 b- defN 24-Apr-23 16:40 generated/volumes/models/volume_service_change_revision_body.py
--rw-r--r--  2.0 unx     2809 b- defN 24-Apr-23 16:40 generated/volumes/models/volume_service_commit_file_body.py
--rw-r--r--  2.0 unx     3055 b- defN 24-Apr-23 16:40 generated/volumes/models/volume_service_commit_file_body_file.py
--rw-r--r--  2.0 unx     2876 b- defN 24-Apr-23 16:40 generated/volumes/models/volume_service_commit_revision_body.py
--rw-r--r--  2.0 unx     3092 b- defN 24-Apr-23 16:40 generated/volumes/models/volume_service_complete_multipart_upload_body.py
--rw-r--r--  2.0 unx     2464 b- defN 24-Apr-23 16:40 generated/volumes/models/volume_service_create_body.py
--rw-r--r--  2.0 unx     2801 b- defN 24-Apr-23 16:40 generated/volumes/models/volume_service_initialize_multipart_upload_body.py
--rw-r--r--  2.0 unx     2527 b- defN 24-Apr-23 16:40 generated/volumes/models/volume_service_sign_multipart_upload_body.py
--rw-r--r--  2.0 unx     2741 b- defN 24-Apr-23 16:40 generated/volumes/models/volume_service_sign_upload_body.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 16:40 generated/volumes/test/__init__.py
+-rw-r--r--  2.0 unx     2928 b- defN 24-Apr-24 09:52 generated/volumes/__init__.py
+-rw-r--r--  2.0 unx    29558 b- defN 24-Apr-24 09:52 generated/volumes/api_client.py
+-rw-r--r--  2.0 unx      852 b- defN 24-Apr-24 09:52 generated/volumes/api_response.py
+-rw-r--r--  2.0 unx    14413 b- defN 24-Apr-24 09:52 generated/volumes/configuration.py
+-rw-r--r--  2.0 unx     5459 b- defN 24-Apr-24 09:52 generated/volumes/exceptions.py
+-rw-r--r--  2.0 unx    12960 b- defN 24-Apr-24 09:52 generated/volumes/rest.py
+-rw-r--r--  2.0 unx      118 b- defN 24-Apr-24 09:52 generated/volumes/api/__init__.py
+-rw-r--r--  2.0 unx   119008 b- defN 24-Apr-24 09:52 generated/volumes/api/volume_service_api.py
+-rw-r--r--  2.0 unx     2287 b- defN 24-Apr-24 09:52 generated/volumes/models/__init__.py
+-rw-r--r--  2.0 unx     2991 b- defN 24-Apr-24 09:52 generated/volumes/models/file_information.py
+-rw-r--r--  2.0 unx     2986 b- defN 24-Apr-24 09:52 generated/volumes/models/v1_file.py
+-rw-r--r--  2.0 unx     2415 b- defN 24-Apr-24 09:52 generated/volumes/models/v1_header_value.py
+-rw-r--r--  2.0 unx     2728 b- defN 24-Apr-24 09:52 generated/volumes/models/v1_initialize_multipart_upload_response.py
+-rw-r--r--  2.0 unx     2855 b- defN 24-Apr-24 09:52 generated/volumes/models/v1_list_files_response.py
+-rw-r--r--  2.0 unx     2855 b- defN 24-Apr-24 09:52 generated/volumes/models/v1_list_parts_response.py
+-rw-r--r--  2.0 unx     2861 b- defN 24-Apr-24 09:52 generated/volumes/models/v1_list_response.py
+-rw-r--r--  2.0 unx     2592 b- defN 24-Apr-24 09:52 generated/volumes/models/v1_part.py
+-rw-r--r--  2.0 unx     2897 b- defN 24-Apr-24 09:52 generated/volumes/models/v1_revision.py
+-rw-r--r--  2.0 unx     3193 b- defN 24-Apr-24 09:52 generated/volumes/models/v1_sign_response.py
+-rw-r--r--  2.0 unx     2910 b- defN 24-Apr-24 09:52 generated/volumes/models/v1_sign_upload_response.py
+-rw-r--r--  2.0 unx      901 b- defN 24-Apr-24 09:52 generated/volumes/models/v1_upload_action.py
+-rw-r--r--  2.0 unx     3159 b- defN 24-Apr-24 09:52 generated/volumes/models/v1_volume.py
+-rw-r--r--  2.0 unx     2517 b- defN 24-Apr-24 09:52 generated/volumes/models/volume_service_change_revision_body.py
+-rw-r--r--  2.0 unx     2809 b- defN 24-Apr-24 09:52 generated/volumes/models/volume_service_commit_file_body.py
+-rw-r--r--  2.0 unx     3055 b- defN 24-Apr-24 09:52 generated/volumes/models/volume_service_commit_file_body_file.py
+-rw-r--r--  2.0 unx     2876 b- defN 24-Apr-24 09:52 generated/volumes/models/volume_service_commit_revision_body.py
+-rw-r--r--  2.0 unx     3092 b- defN 24-Apr-24 09:52 generated/volumes/models/volume_service_complete_multipart_upload_body.py
+-rw-r--r--  2.0 unx     2464 b- defN 24-Apr-24 09:52 generated/volumes/models/volume_service_create_body.py
+-rw-r--r--  2.0 unx     2801 b- defN 24-Apr-24 09:52 generated/volumes/models/volume_service_initialize_multipart_upload_body.py
+-rw-r--r--  2.0 unx     2527 b- defN 24-Apr-24 09:52 generated/volumes/models/volume_service_sign_multipart_upload_body.py
+-rw-r--r--  2.0 unx     2741 b- defN 24-Apr-24 09:52 generated/volumes/models/volume_service_sign_upload_body.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 09:52 generated/volumes/test/__init__.py
 -rw-r--r--  2.0 unx     1716 b- defN 24-Mar-28 14:39 generated/volumes/test/test_file_information.py
 -rw-r--r--  2.0 unx     1718 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_file.py
 -rw-r--r--  2.0 unx     1494 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_header_value.py
 -rw-r--r--  2.0 unx     1755 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_initialize_multipart_upload_response.py
 -rw-r--r--  2.0 unx     1949 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_list_files_response.py
 -rw-r--r--  2.0 unx     1721 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_list_parts_response.py
 -rw-r--r--  2.0 unx     2073 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_list_response.py
@@ -389,14 +396,14 @@
 -rw-r--r--  2.0 unx     1912 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_commit_file_body_file.py
 -rw-r--r--  2.0 unx     2548 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_commit_revision_body.py
 -rw-r--r--  2.0 unx     2233 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_complete_multipart_upload_body.py
 -rw-r--r--  2.0 unx     1624 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_create_body.py
 -rw-r--r--  2.0 unx     2149 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_initialize_multipart_upload_body.py
 -rw-r--r--  2.0 unx     1769 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_sign_multipart_upload_body.py
 -rw-r--r--  2.0 unx     1968 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_sign_upload_body.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 07:53 everai-0.1.34.dist-info/LICENSE
--rw-r--r--  2.0 unx     1951 b- defN 24-Apr-24 07:53 everai-0.1.34.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 07:53 everai-0.1.34.dist-info/WHEEL
--rw-r--r--  2.0 unx       98 b- defN 24-Apr-24 07:53 everai-0.1.34.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-24 07:53 everai-0.1.34.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    39817 b- defN 24-Apr-24 07:53 everai-0.1.34.dist-info/RECORD
-400 files, 1289089 bytes uncompressed, 353348 bytes compressed:  72.6%
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 12:38 everai-0.1.35.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1951 b- defN 24-Apr-24 12:38 everai-0.1.35.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 12:38 everai-0.1.35.dist-info/WHEEL
+-rw-r--r--  2.0 unx       98 b- defN 24-Apr-24 12:38 everai-0.1.35.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-24 12:38 everai-0.1.35.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    40541 b- defN 24-Apr-24 12:38 everai-0.1.35.dist-info/RECORD
+407 files, 1318255 bytes uncompressed, 358716 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -159,14 +159,17 @@
 
 Filename: everai/commands/configmap/get.py
 Comment: 
 
 Filename: everai/commands/configmap/list.py
 Comment: 
 
+Filename: everai/commands/configmap/update.py
+Comment: 
+
 Filename: everai/commands/image/__init__.py
 Comment: 
 
 Filename: everai/commands/image/build.py
 Comment: 
 
 Filename: everai/commands/image/image.py
@@ -192,14 +195,17 @@
 
 Filename: everai/commands/secret/list.py
 Comment: 
 
 Filename: everai/commands/secret/secret.py
 Comment: 
 
+Filename: everai/commands/secret/update.py
+Comment: 
+
 Filename: everai/commands/volume/__init__.py
 Comment: 
 
 Filename: everai/commands/volume/create.py
 Comment: 
 
 Filename: everai/commands/volume/delete.py
@@ -234,14 +240,17 @@
 
 Filename: everai/configmap/configmap.py
 Comment: 
 
 Filename: everai/configmap/configmap_manager.py
 Comment: 
 
+Filename: everai/configmap/utils.py
+Comment: 
+
 Filename: everai/image/__init__.py
 Comment: 
 
 Filename: everai/image/auth.py
 Comment: 
 
 Filename: everai/image/builder.py
@@ -372,14 +381,17 @@
 
 Filename: generated/configmaps/models/__init__.py
 Comment: 
 
 Filename: generated/configmaps/models/configmap_service_create_body.py
 Comment: 
 
+Filename: generated/configmaps/models/configmap_service_update_body.py
+Comment: 
+
 Filename: generated/configmaps/models/v1_configmap.py
 Comment: 
 
 Filename: generated/configmaps/models/v1_list_response.py
 Comment: 
 
 Filename: generated/configmaps/test/__init__.py
@@ -387,14 +399,17 @@
 
 Filename: generated/configmaps/test/test_configmap_service_api.py
 Comment: 
 
 Filename: generated/configmaps/test/test_configmap_service_create_body.py
 Comment: 
 
+Filename: generated/configmaps/test/test_configmap_service_update_body.py
+Comment: 
+
 Filename: generated/configmaps/test/test_v1_configmap.py
 Comment: 
 
 Filename: generated/configmaps/test/test_v1_list_response.py
 Comment: 
 
 Filename: generated/schedulers/__init__.py
@@ -990,14 +1005,17 @@
 
 Filename: generated/secrets/models/__init__.py
 Comment: 
 
 Filename: generated/secrets/models/secret_service_create_body.py
 Comment: 
 
+Filename: generated/secrets/models/secret_service_update_body.py
+Comment: 
+
 Filename: generated/secrets/models/v1_list_response.py
 Comment: 
 
 Filename: generated/secrets/models/v1_secret.py
 Comment: 
 
 Filename: generated/secrets/test/__init__.py
@@ -1005,14 +1023,17 @@
 
 Filename: generated/secrets/test/test_secret_service_api.py
 Comment: 
 
 Filename: generated/secrets/test/test_secret_service_create_body.py
 Comment: 
 
+Filename: generated/secrets/test/test_secret_service_update_body.py
+Comment: 
+
 Filename: generated/secrets/test/test_v1_list_response.py
 Comment: 
 
 Filename: generated/secrets/test/test_v1_secret.py
 Comment: 
 
 Filename: generated/volumes/__init__.py
@@ -1176,26 +1197,26 @@
 
 Filename: generated/volumes/test/test_volume_service_sign_multipart_upload_body.py
 Comment: 
 
 Filename: generated/volumes/test/test_volume_service_sign_upload_body.py
 Comment: 
 
-Filename: everai-0.1.34.dist-info/LICENSE
+Filename: everai-0.1.35.dist-info/LICENSE
 Comment: 
 
-Filename: everai-0.1.34.dist-info/METADATA
+Filename: everai-0.1.35.dist-info/METADATA
 Comment: 
 
-Filename: everai-0.1.34.dist-info/WHEEL
+Filename: everai-0.1.35.dist-info/WHEEL
 Comment: 
 
-Filename: everai-0.1.34.dist-info/entry_points.txt
+Filename: everai-0.1.35.dist-info/entry_points.txt
 Comment: 
 
-Filename: everai-0.1.34.dist-info/top_level.txt
+Filename: everai-0.1.35.dist-info/top_level.txt
 Comment: 
 
-Filename: everai-0.1.34.dist-info/RECORD
+Filename: everai-0.1.35.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## everai/version.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.34"
+__version__ = "0.1.35"
```

## everai/api/api.py

```diff
@@ -1,15 +1,15 @@
 import functools
 import typing
 
 from everai.logger import logger
 from everai.token_manager import TokenManager
 from generated.configmaps import (
     ApiClient as ConfigMapsClient,
-    ConfigmapServiceApi, V1Configmap, ConfigmapServiceCreateBody
+    ConfigmapServiceApi, V1Configmap, ConfigmapServiceCreateBody, ConfigmapServiceUpdateBody
 )
 
 from generated.schedulers import (
     ApiClient as SchedulersClient,
     V1App,
     AppServiceCreateBody,
     V1AppServiceSetupImageBody,
@@ -47,15 +47,15 @@
     VolumeServiceCreateBody
 )
 
 from generated.secrets import (
     ApiClient as SecretsClient,
     V1Secret,
     SecretServiceApi,
-    SecretServiceCreateBody,
+    SecretServiceCreateBody, SecretServiceUpdateBody,
 )
 
 from everai.constants import EVERAI_ENDPOINT
 
 
 class ValueFromSecret:
     secret_name: str
@@ -251,14 +251,21 @@
     def create_secret(self, secret: V1Secret) -> V1Secret:
         resp = self.secret_service_api.create_secret(secret.name, body=SecretServiceCreateBody(
             data=secret.data,
             labels=secret.labels,
         ))
         return resp
 
+    def update_secret(self, secret: V1Secret) -> V1Secret:
+        resp = self.secret_service_api.update_secret(secret.name, body=SecretServiceUpdateBody(
+            data=secret.data,
+            labels=secret.labels,
+        ))
+        return resp
+
     def list_secrets(self) -> typing.List[V1Secret]:
         resp = self.secret_service_api.list_secret()
         return resp.secrets or []
 
     def get_secret(self, name: str) -> V1Secret:
         resp = self.secret_service_api.get_secret(name)
         return resp
@@ -353,14 +360,21 @@
     def create_configmap(self, configmap: V1Configmap) -> V1Configmap:
         resp = self.configmap_service_api.create_configmap(configmap.name, body=ConfigmapServiceCreateBody(
             data=configmap.data,
             labels=configmap.labels,
         ))
         return resp
 
+    def update_configmap(self, configmap: V1Configmap) -> V1Configmap:
+        resp = self.configmap_service_api.update_configmap(configmap.name, body=ConfigmapServiceUpdateBody(
+            data=configmap.data,
+            labels=configmap.labels,
+        ))
+        return resp
+
     def list_configmaps(self) -> typing.List[V1Configmap]:
         resp = self.configmap_service_api.list_configmaps()
         return resp.configmaps or []
 
     def get_configmap(self, name: str) -> V1Configmap:
         resp = self.configmap_service_api.get_configmap(name)
         return resp
```

## everai/app/app_manager.py

```diff
@@ -12,15 +12,15 @@
 from everai.image import Image, BasicAuth
 from everai.resource_requests.resource_requests import ResourceRequests
 from everai.runner import must_find_target
 from everai.api import API
 from everai.secret import Secret, SecretManager
 from everai.placeholder import Placeholder
 from everai.volume import Volume, VolumeManager
-from everai.autoscaling import AutoScalingPolicy
+from everai.autoscaling import AutoScalingPolicy, SimpleAutoScalingPolicy
 from gevent.pywsgi import WSGIServer
 import gevent.signal
 import signal
 import threading
 
 from flask import Flask, Blueprint, Response
 
@@ -32,16 +32,15 @@
 )
 from generated.volumes.exceptions import NotFoundException as VolumeNotFoundException
 
 autoscaling_warning = """
 You are deploying an app without autoscaling_policy, 
 that will cause the app to run only one worker and always one worker,
 if you want to setup an autoscaling_policy for this app after deploy,
-you cloud run command everai app upgrade <your app name> --autoscaling-policy,
-or setup in your dashboard, everai.expvent.com
+you must rebuild image and upgrade it use everai app upgrade --image
 """
 
 
 class AppManager:
     def __init__(self):
         self.api = API()
         self.secret_manager = SecretManager()
@@ -200,14 +199,17 @@
     def setup_image(self, app_name: str, image: Image):
         username = None
         password = None
         if image.auth is not None:
             assert isinstance(image.auth, BasicAuth)
             assert isinstance(image.auth.username, Placeholder)
             assert isinstance(image.auth.password, Placeholder)
+            assert image.auth.username.kind == 'Secret'
+            assert image.auth.password.kind == 'Secret'
+
             username = ValueFromSecret(secret_name=image.auth.username.name,
                                        key=image.auth.username.key)
             password = ValueFromSecret(secret_name=image.auth.password.name,
                                        key=image.auth.password.key)
 
         self.api.setup_image(app_name, repository=image.repository, tag=image.tag, digest=image.digest,
                              username=username, password=password)
@@ -255,23 +257,24 @@
 
         if len(missed) > 0:
             msg = ', '.join(missed)
             raise Exception(f'resource_requests, image is required, {msg} is missed')
 
         if app.autoscaling_policy is None:
             print(f"Warning: {autoscaling_warning}")
+            autoscaling_policy = SimpleAutoScalingPolicy()
+        else:
+            autoscaling_policy = app.autoscaling_policy
 
         self.setup_image(app.name, app.image)
 
         if app.volume_requests is not None and len(app.volume_requests) > 0:
             self.setup_volume_requests(app.name, app.volume_requests)
 
         if app.secret_requests is not None and len(app.secret_requests) > 0:
             self.setup_secret_requests(app.name, app.secret_requests)
 
         self.setup_resource_requests(app.name, app.resource_requests)
 
-        self.setup_autoscaling_policy(app.name, app.autoscaling_policy)
-
     def list_worker(self, app_name: str) -> typing.List[Worker]:
         workers = self.api.list_worker(app_name=app_name)
         return [Worker.from_proto(worker) for worker in workers]
```

## everai/autoscaling/simple_autoscaling.py

```diff
@@ -20,18 +20,18 @@
     max_queue_size: ArgumentType
     # The quantity of each scale up
     scale_up_step: ArgumentType
     # The max_idle_time in seconds let scheduler witch worker should be scale down
     max_idle_time: ArgumentType
 
     def __init__(self,
-                 min_workers: ArgumentType[int],
-                 max_workers: ArgumentType[int],
-                 max_queue_size: ArgumentType[int],
-                 max_idle_time: ArgumentType[int],
+                 min_workers: ArgumentType[int] = 1,
+                 max_workers: ArgumentType[int] = 1,
+                 max_queue_size: ArgumentType[int] = 1,
+                 max_idle_time: ArgumentType[int] = 1,
                  scale_up_step: ArgumentType[int] = 1):
 
         self.min_workers = min_workers
         self.max_workers = max_workers
         self.max_queue_size = max_queue_size
         self.max_idle_time = max_idle_time
         self.scale_up_step = scale_up_step
```

## everai/commands/configmap/configmap.py

```diff
@@ -1,13 +1,14 @@
 from everai.commands.command import ClientCommand, setup_subcommands
 from argparse import _SubParsersAction
-from everai.commands.configmap.create import ConfigMapCreateCommand
-from everai.commands.configmap.delete import ConfigMapDeleteCommand
-from everai.commands.configmap.list import ConfigMapListCommand
-from everai.commands.configmap.get import ConfigMapGetCommand
+from everai.commands.configmap.create import CreateCommand
+from everai.commands.configmap.delete import DeleteCommand
+from everai.commands.configmap.list import ListCommand
+from everai.commands.configmap.get import GetCommand
+from everai.commands.configmap.update import UpdateCommand
 
 
 class ConfigMapCommand(ClientCommand):
     parser: _SubParsersAction = None
 
     def __init__(self, args):
         self.args = args
@@ -16,18 +17,19 @@
     def setup(parser: _SubParsersAction):
         configmap_parser = parser.add_parser('configmap',
                                              aliases=['cm', 'configmaps'],
                                              help='Manage configmaps')
         configmap_subparser = configmap_parser.add_subparsers(help="Configmap command help")
 
         setup_subcommands(configmap_subparser, [
-            ConfigMapCreateCommand,
-            ConfigMapDeleteCommand,
-            ConfigMapListCommand,
-            ConfigMapGetCommand,
+            CreateCommand,
+            DeleteCommand,
+            ListCommand,
+            GetCommand,
+            UpdateCommand,
         ])
 
         configmap_parser.set_defaults(func=ConfigMapCommand)
         ConfigMapCommand.parser = configmap_parser
 
     def run(self):
         ConfigMapCommand.parser.print_help()
```

## everai/commands/configmap/create.py

```diff
@@ -1,15 +1,15 @@
 from everai.commands.command import ClientCommand, command_error
 from argparse import _SubParsersAction
 
 from everai.configmap import ConfigMapManager
 from everai.secret.secret_manager import SecretManager
 
 
-class ConfigMapCreateCommand(ClientCommand):
+class CreateCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
     def setup(parser: _SubParsersAction):
         create_parser = parser.add_parser('create', help='Create ConfigMap from file or literal string')
         create_parser.add_argument('name', help='The configmap name')
@@ -25,26 +25,26 @@
             '-f',
             '--from-file',
             action='append',
             type=str,
             help='Create configmap from file, for example: --from-file filename'
         )
 
-        create_parser.set_defaults(func=ConfigMapCreateCommand)
+        create_parser.set_defaults(func=CreateCommand)
 
     @command_error
     def run(self):
         if self.args.from_literal is None and self.args.from_file is None:
             raise ValueError('Please specify either --from-literal, or --from-file arguments')
 
         if self.args.from_literal is not None and self.args.from_file is not None:
             raise ValueError('Cannot support both --from-literal and --from-file')
 
         if self.args.from_literal is not None and len(self.args.from_literal) > 0:
-            configmap = ConfigMapManager().create_from_lines(name=self.args.name, lines=self.args.from_literal)
+            configmap = ConfigMapManager().create_from_literal(name=self.args.name, literals=self.args.from_literal)
         elif self.args.from_file is not None and len(self.args.from_file) > 0:
             configmap = ConfigMapManager().create_from_file(name=self.args.name, file=self.args.from_file)
         else:
             raise RuntimeError('Never been here')
 
         print(f"Configmap `{configmap.name}` created successfully")
```

## everai/commands/configmap/delete.py

```diff
@@ -1,22 +1,22 @@
 from everai.commands.command import ClientCommand, command_error
 from argparse import _SubParsersAction
 
 from everai.configmap import ConfigMapManager
 
 
-class ConfigMapDeleteCommand(ClientCommand):
+class DeleteCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
     def setup(parser: _SubParsersAction):
         delete_parser = parser.add_parser('delete', help='Delete configmap')
         delete_parser.add_argument('name', help='The configmap name')
 
-        delete_parser.set_defaults(func=ConfigMapDeleteCommand)
+        delete_parser.set_defaults(func=DeleteCommand)
 
     @command_error
     def run(self):
         ConfigMapManager().delete(name=self.args.name)
         print(f'Configmap `{self.args.name}` deleted successfully')
```

## everai/commands/configmap/get.py

```diff
@@ -1,22 +1,22 @@
 from everai.commands.command import ClientCommand, command_error, ListDisplayer
 from argparse import _SubParsersAction
 
 from everai.configmap import ConfigMapManager, ConfigMap
 from everai.secret.secret_manager import SecretManager
 
 
-class ConfigMapGetCommand(ClientCommand):
+class GetCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
     def setup(parser: _SubParsersAction):
         get_parser = parser.add_parser('get', help='Get configmap')
         get_parser.add_argument('name', help='The configmap name')
         ListDisplayer.add_output_to_parser(get_parser)
-        get_parser.set_defaults(func=ConfigMapGetCommand)
+        get_parser.set_defaults(func=GetCommand)
 
     @command_error
     def run(self):
         configmap = ConfigMapManager().get(name=self.args.name)
         ListDisplayer[ConfigMap](configmap).show_list(self.args.output)
```

## everai/commands/configmap/list.py

```diff
@@ -1,21 +1,21 @@
 from everai.commands.command import ClientCommand, command_error, ListDisplayer
 from argparse import _SubParsersAction
 
 from everai.configmap import ConfigMapManager, ConfigMap
 
 
-class ConfigMapListCommand(ClientCommand):
+class ListCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
     def setup(parser: _SubParsersAction):
         list_parser = parser.add_parser('list', aliases=['ls'], help='List configmaps')
         ListDisplayer.add_output_to_parser(list_parser)
-        list_parser.set_defaults(func=ConfigMapListCommand)
+        list_parser.set_defaults(func=ListCommand)
 
     @command_error
     def run(self):
         configmaps = ConfigMapManager().list()
         ListDisplayer[ConfigMap](configmaps).show_list(self.args.output)
```

## everai/commands/secret/create.py

```diff
@@ -1,13 +1,13 @@
 from everai.commands.command import ClientCommand, command_error
 from argparse import _SubParsersAction
 from everai.secret.secret_manager import SecretManager
 
 
-class SecretCreateCommand(ClientCommand):
+class CreateCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
     def setup(parser: _SubParsersAction):
         create_parser = parser.add_parser('create', help='Create Secret from file or literal string')
         create_parser.add_argument('name', help='The secret name')
@@ -23,25 +23,25 @@
             '-f',
             '--from-file',
             action='append',
             type=str,
             help='Create secret from file, for example: --from-file filename'
         )
 
-        create_parser.set_defaults(func=SecretCreateCommand)
+        create_parser.set_defaults(func=CreateCommand)
 
     @command_error
     def run(self):
         if self.args.from_literal is None and self.args.from_file is None:
             raise ValueError('Please specify either --from-literal, or --from-file arguments')
 
         if self.args.from_literal is not None and self.args.from_file is not None:
             raise ValueError('Cannot support both --from-literal and --from-file')
 
         if self.args.from_literal is not None and len(self.args.from_literal) > 0:
-            secret = SecretManager().create_from_lines(name=self.args.name, lines=self.args.from_literal)
+            secret = SecretManager().create_from_literal(name=self.args.name, literals=self.args.from_literal)
 
         if self.args.from_file is not None and len(self.args.from_file) > 0:
             secret = SecretManager().create_from_file(name=self.args.name, file=self.args.from_file)
 
         print("Secret created successfully")
```

## everai/commands/secret/delete.py

```diff
@@ -1,21 +1,21 @@
 from everai.commands.command import ClientCommand, command_error
 from argparse import _SubParsersAction
 from everai.secret.secret_manager import SecretManager
 
 
-class SecretDeleteCommand(ClientCommand):
+class DeleteCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
     def setup(parser: _SubParsersAction):
         delete_parser = parser.add_parser('delete', help='Delete secret')
         delete_parser.add_argument('name', help='The secret name')
 
-        delete_parser.set_defaults(func=SecretDeleteCommand)
+        delete_parser.set_defaults(func=DeleteCommand)
 
     @command_error
     def run(self):
         SecretManager().delete(name=self.args.name)
         print('Secret deleted successfully')
```

## everai/commands/secret/get.py

```diff
@@ -1,29 +1,22 @@
-from everai.commands.command import ClientCommand, command_error
+from everai.commands.command import ClientCommand, command_error, ListDisplayer
 from argparse import _SubParsersAction
+
+from everai.secret import Secret
 from everai.secret.secret_manager import SecretManager
 
 
-class SecretGetCommand(ClientCommand):
+class GetCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
     def setup(parser: _SubParsersAction):
         get_parser = parser.add_parser('get', help='Get secret')
         get_parser.add_argument('name', help='The secret name')
-        get_parser.add_argument(
-            '-o',
-            '--output',
-            help='Output type, current support json|table',
-            default='table',
-            type=str,
-        )
-        get_parser.set_defaults(func=SecretGetCommand)
+        ListDisplayer.add_output_to_parser(get_parser)
+        get_parser.set_defaults(func=GetCommand)
 
     @command_error
     def run(self):
-        secret = SecretManager().get(name=self.args.name)
-        if self.args.output == 'table':
-            print(secret)
-        elif self.args.output == 'json':
-            print(secret.to_json())
+        configmap = SecretManager().get(name=self.args.name)
+        ListDisplayer[Secret](configmap).show_list(self.args.output)
```

## everai/commands/secret/list.py

```diff
@@ -3,22 +3,22 @@
 
 from everai.secret import Secret
 from everai.secret.secret_manager import SecretManager
 import json
 from typing import List, Dict
 
 
-class SecretListCommand(ClientCommand):
+class ListCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
     def setup(parser: _SubParsersAction):
         list_parser = parser.add_parser('list', aliases=['ls'], help='List secret')
         ListDisplayer.add_output_to_parser(list_parser)
-        list_parser.set_defaults(func=SecretListCommand)
+        list_parser.set_defaults(func=ListCommand)
 
     @command_error
     def run(self):
         secrets = SecretManager().list()
         ListDisplayer[Secret](secrets).show_list(self.args.output)
```

## everai/commands/secret/secret.py

```diff
@@ -1,13 +1,14 @@
 from everai.commands.command import ClientCommand, setup_subcommands
 from argparse import _SubParsersAction
-from everai.commands.secret.create import SecretCreateCommand
-from everai.commands.secret.delete import SecretDeleteCommand
-from everai.commands.secret.list import SecretListCommand
-from everai.commands.secret.get import SecretGetCommand
+from everai.commands.secret.create import CreateCommand
+from everai.commands.secret.delete import DeleteCommand
+from everai.commands.secret.list import ListCommand
+from everai.commands.secret.get import GetCommand
+from everai.commands.secret.update import UpdateCommand
 
 
 class SecretCommand(ClientCommand):
     parser: _SubParsersAction = None
 
     def __init__(self, args):
         self.args = args
@@ -16,18 +17,19 @@
     def setup(parser: _SubParsersAction):
         secret_parser = parser.add_parser('secret',
                                           aliases=['secrets', 'sec'],
                                           help='Manage secrets')
         secret_subparser = secret_parser.add_subparsers(help="Secret command help")
 
         setup_subcommands(secret_subparser, [
-            SecretCreateCommand,
-            SecretDeleteCommand,
-            SecretListCommand,
-            SecretGetCommand,
+            CreateCommand,
+            DeleteCommand,
+            ListCommand,
+            GetCommand,
+            UpdateCommand,
         ])
 
         secret_parser.set_defaults(func=SecretCommand)
         SecretCommand.parser = secret_parser
 
     def run(self):
         SecretCommand.parser.print_help()
```

## everai/configmap/__init__.py

```diff
@@ -1,5 +1,12 @@
 
 from .configmap import ConfigMap
 from .configmap_manager import ConfigMapManager
+from .utils import literals_to_dict, file_to_dict, stream_to_dict
 
-__all__ = ['ConfigMap', 'ConfigMapManager']
+__all__ = [
+    'ConfigMap',
+    'ConfigMapManager',
+    'literals_to_dict',
+    'file_to_dict',
+    'stream_to_dict',
+]
```

## everai/configmap/configmap_manager.py

```diff
@@ -1,40 +1,45 @@
+import yaml
+
 from everai.configmap.configmap import ConfigMap
 import typing
 from everai.api import API
-
+from .utils import literals_to_dict, file_to_dict
 
 class ConfigMapManager:
     def __init__(self):
         self.api = API()
 
     def create(self, name: str, data: typing.Dict[str, str]) -> ConfigMap:
         configmap = ConfigMap(name=name, data=data)
-        v1secret = configmap.to_proto()
-        resp = self.api.create_configmap(v1secret)
+        v1configmap = configmap.to_proto()
+        resp = self.api.create_configmap(v1configmap)
         return ConfigMap.from_proto(resp)
 
-    def create_from_lines(self, name: str, lines: typing.List[str]) -> ConfigMap:
-        data: typing.Dict[str, str] = {}
-
-        for line in lines:
-            key_value = line.split('=', 1)
+    def update(self, name: str, data: typing.Dict[str, str]) -> ConfigMap:
+        configmap = ConfigMap(name=name, data=data)
+        v1configmap = configmap.to_proto()
+        resp = self.api.update_configmap(v1configmap)
+        return ConfigMap.from_proto(resp)
 
-            if len(key_value) == 2:
-                data[key_value[0]] = key_value[1]
-            else:
-                data[key_value[0]] = ''
+    def create_from_literal(self, name: str, literals: typing.List[str]) -> ConfigMap:
+        data = literals_to_dict(literals=literals)
         return self.create(name, data)
 
+    def update_from_literal(self, name: str, literals: typing.List[str]) -> ConfigMap:
+        data = literals_to_dict(literals=literals)
+        return self.update(name, data)
+
     def create_from_file(self, name: str, file: str) -> ConfigMap:
-        lines: typing.List[str] = []
+        data = file_to_dict(file)
+        return self.create(name, data)
 
-        with open(file, "r") as f:
-            lines = f.readlines()
-            return self.create_from_lines(name, lines)
+    def update_from_file(self, name: str, file: str) -> ConfigMap:
+        data = file_to_dict(file)
+        return self.update(name, data)
 
     def delete(self, name: str):
         self.api.delete_secret(name)
 
     def list(self) -> typing.List[ConfigMap]:
         resp = self.api.list_configmaps()
         list_secrets = [ConfigMap.from_proto(configmap) for configmap in resp]
```

## everai/secret/secret_manager.py

```diff
@@ -1,7 +1,8 @@
+from everai.configmap import literals_to_dict, file_to_dict
 from everai.secret import Secret
 import typing
 from everai.api import API
 
 
 class SecretManager:
     def __init__(self):
@@ -9,32 +10,35 @@
 
     def create(self, name: str, data: typing.Dict[str, str]) -> Secret:
         secret = Secret(name=name, data=data)
         v1secret = secret.to_proto()
         resp = self.api.create_secret(v1secret)
         return Secret.from_proto(resp)
 
-    def create_from_lines(self, name: str, lines: typing.List[str]) -> Secret:
-        data: typing.Dict[str, str] = {}
-
-        for line in lines:
-            key_value = line.split('=', 1)
+    def update(self, name: str, data: typing.Dict[str, str]) -> Secret:
+        secret = Secret(name=name, data=data)
+        v1secret = secret.to_proto()
+        resp = self.api.update_secret(v1secret)
+        return Secret.from_proto(resp)
 
-            if len(key_value) == 2:
-                data[key_value[0]] = key_value[1]
-            else:
-                data[key_value[0]] = ''
+    def create_from_literal(self, name: str, literals: typing.List[str]) -> Secret:
+        data = literals_to_dict(literals=literals)
         return self.create(name, data)
 
+    def update_from_literal(self, name: str, literals: typing.List[str]) -> Secret:
+        data = literals_to_dict(literals=literals)
+        return self.update(name, data)
+
     def create_from_file(self, name: str, file: str) -> Secret:
-        lines: typing.List[str] = []
+        data = file_to_dict(file)
+        return self.create(name, data)
 
-        with open(file, "r") as f:
-            lines = f.readlines()
-            return self.create_from_lines(name, lines)
+    def update_from_file(self, name: str, file: str) -> Secret:
+        data = file_to_dict(file)
+        return self.update(name, data)
 
     def delete(self, name: str):
         self.api.delete_secret(name)
 
     def list(self) -> typing.List[Secret]:
         resp = self.api.list_secrets()
```

## generated/configmaps/__init__.py

```diff
@@ -28,9 +28,10 @@
 from generated.configmaps.exceptions import ApiValueError
 from generated.configmaps.exceptions import ApiKeyError
 from generated.configmaps.exceptions import ApiAttributeError
 from generated.configmaps.exceptions import ApiException
 
 # import models into sdk package
 from generated.configmaps.models.configmap_service_create_body import ConfigmapServiceCreateBody
+from generated.configmaps.models.configmap_service_update_body import ConfigmapServiceUpdateBody
 from generated.configmaps.models.v1_configmap import V1Configmap
 from generated.configmaps.models.v1_list_response import V1ListResponse
```

## generated/configmaps/api/configmap_service_api.py

```diff
@@ -20,14 +20,15 @@
 from typing import Dict, List, Optional, Tuple
 
 from pydantic import StrictStr
 
 from typing import Any, Dict, Union
 
 from generated.configmaps.models.configmap_service_create_body import ConfigmapServiceCreateBody
+from generated.configmaps.models.configmap_service_update_body import ConfigmapServiceUpdateBody
 from generated.configmaps.models.v1_configmap import V1Configmap
 from generated.configmaps.models.v1_list_response import V1ListResponse
 
 from generated.configmaps.api_client import ApiClient
 from generated.configmaps.api_response import ApiResponse
 from generated.configmaps.exceptions import (  # noqa: F401
     ApiTypeError,
@@ -638,14 +639,181 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    def update_configmap(
+        self,
+        configmap_name: StrictStr,
+        body: ConfigmapServiceUpdateBody,
+        **kwargs,
+    ) -> V1Configmap:
+        """Update configmap  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.update_configmap(configmap_name, body, async_req=True)
+        >>> result = thread.get()
+
+        :param configmap_name: (required)
+        :type configmap_name: str
+        :param body: (required)
+        :type body: ConfigmapServiceUpdateBody
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: V1Configmap
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the update_configmap_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+
+        return self.update_configmap_with_http_info(
+            configmap_name,
+            body,
+            **kwargs,
+        )
+
+    @validate_call
+    def update_configmap_with_http_info(
+        self,
+        configmap_name: StrictStr,
+        body: ConfigmapServiceUpdateBody,
+        **kwargs,
+    ) -> ApiResponse:
+        """Update configmap  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.update_configmap_with_http_info(configmap_name, body, async_req=True)
+        >>> result = thread.get()
+
+        :param configmap_name: (required)
+        :type configmap_name: str
+        :param body: (required)
+        :type body: ConfigmapServiceUpdateBody
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(V1Configmap, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'configmap_name',
+            'body'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method update_configmap" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats: Dict[str, str] = {}
+
+        # process the path parameters
+        _path_params: Dict[str, str] = {}
+        if _params['configmap_name'] is not None:
+            _path_params['configmapName'] = _params['configmap_name']
+
+
+        # process the query parameters
+        _query_params: List[Tuple[str, str]] = []
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        # process the body parameter
+        _body_params = None
+        if _params['body'] is not None:
+            _body_params = _params['body']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings: List[str] = []  # noqa: E501
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "V1Configmap",
+        }
+
+        return self.api_client.call_api(
+            '/api/configmaps/v1/{configmapName}', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

## generated/configmaps/models/__init__.py

```diff
@@ -11,9 +11,10 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
 from generated.configmaps.models.configmap_service_create_body import ConfigmapServiceCreateBody
+from generated.configmaps.models.configmap_service_update_body import ConfigmapServiceUpdateBody
 from generated.configmaps.models.v1_configmap import V1Configmap
 from generated.configmaps.models.v1_list_response import V1ListResponse
```

## generated/secrets/__init__.py

```diff
@@ -28,9 +28,10 @@
 from generated.secrets.exceptions import ApiValueError
 from generated.secrets.exceptions import ApiKeyError
 from generated.secrets.exceptions import ApiAttributeError
 from generated.secrets.exceptions import ApiException
 
 # import models into sdk package
 from generated.secrets.models.secret_service_create_body import SecretServiceCreateBody
+from generated.secrets.models.secret_service_update_body import SecretServiceUpdateBody
 from generated.secrets.models.v1_list_response import V1ListResponse
 from generated.secrets.models.v1_secret import V1Secret
```

## generated/secrets/api/secret_service_api.py

```diff
@@ -20,14 +20,15 @@
 from typing import Dict, List, Optional, Tuple
 
 from pydantic import StrictStr
 
 from typing import Any, Dict, Union
 
 from generated.secrets.models.secret_service_create_body import SecretServiceCreateBody
+from generated.secrets.models.secret_service_update_body import SecretServiceUpdateBody
 from generated.secrets.models.v1_list_response import V1ListResponse
 from generated.secrets.models.v1_secret import V1Secret
 
 from generated.secrets.api_client import ApiClient
 from generated.secrets.api_response import ApiResponse
 from generated.secrets.exceptions import (  # noqa: F401
     ApiTypeError,
@@ -638,14 +639,181 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    def update_secret(
+        self,
+        secret_name: StrictStr,
+        body: SecretServiceUpdateBody,
+        **kwargs,
+    ) -> V1Secret:
+        """Update secret  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.update_secret(secret_name, body, async_req=True)
+        >>> result = thread.get()
+
+        :param secret_name: (required)
+        :type secret_name: str
+        :param body: (required)
+        :type body: SecretServiceUpdateBody
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: V1Secret
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the update_secret_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+
+        return self.update_secret_with_http_info(
+            secret_name,
+            body,
+            **kwargs,
+        )
+
+    @validate_call
+    def update_secret_with_http_info(
+        self,
+        secret_name: StrictStr,
+        body: SecretServiceUpdateBody,
+        **kwargs,
+    ) -> ApiResponse:
+        """Update secret  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.update_secret_with_http_info(secret_name, body, async_req=True)
+        >>> result = thread.get()
+
+        :param secret_name: (required)
+        :type secret_name: str
+        :param body: (required)
+        :type body: SecretServiceUpdateBody
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(V1Secret, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'secret_name',
+            'body'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method update_secret" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats: Dict[str, str] = {}
+
+        # process the path parameters
+        _path_params: Dict[str, str] = {}
+        if _params['secret_name'] is not None:
+            _path_params['secretName'] = _params['secret_name']
+
+
+        # process the query parameters
+        _query_params: List[Tuple[str, str]] = []
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        # process the body parameter
+        _body_params = None
+        if _params['body'] is not None:
+            _body_params = _params['body']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings: List[str] = []  # noqa: E501
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "V1Secret",
+        }
+
+        return self.api_client.call_api(
+            '/api/secrets/v1/{secretName}', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

## generated/secrets/models/__init__.py

```diff
@@ -11,9 +11,10 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
 from generated.secrets.models.secret_service_create_body import SecretServiceCreateBody
+from generated.secrets.models.secret_service_update_body import SecretServiceUpdateBody
 from generated.secrets.models.v1_list_response import V1ListResponse
 from generated.secrets.models.v1_secret import V1Secret
```

## Comparing `everai-0.1.34.dist-info/METADATA` & `everai-0.1.35.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everai
-Version: 0.1.34
+Version: 0.1.35
 Summary: Client library to manage everai infrastructure
 Author-email: mc <mc@expvent.com>
 Maintainer-email: mc <mc@expvent.com>
 Project-URL: Homepage, https://everai.expvent.com
 Project-URL: Documentation, https://everai.expvent.com
 Project-URL: Repository, https://github.com/expvent/everai
 Project-URL: Issues, https://github.com/expvent/everai/issues
```

## Comparing `everai-0.1.34.dist-info/RECORD` & `everai-0.1.35.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 everai/__init__.py,sha256=AbgR3tVRy6TETgwXyJITEnET1TSFpEAEqQJJqzReYqQ,66
 everai/constants.py,sha256=bZuLnYDxayThik9UU4eABKRjrp6fHw5vT14gNR2LpF8,1111
-everai/version.py,sha256=79r5jd-MqbhXLbIBDVBqUJvhvcucjkaId96r46KF18I,23
+everai/version.py,sha256=ABqgofsnbWf7823vTBbZNQ81eKQbWwrVToAU6T3z-6s,23
 everai/api/__init__.py,sha256=2WLrQ_PpJ35__yOVHC89MhILujyGioyaGir-5n6hxCc,40
-everai/api/api.py,sha256=HKMYo37SZxQo-aeqrIA5S0AKKoxGxkKhhejXBR3-y2o,14055
+everai/api/api.py,sha256=0zue7tdbrbu3EfbZiWKYkUKXG5BqAyI75rN-78CkD7o,14640
 everai/app/__init__.py,sha256=A-USWcj6TDAW_hxG6wT3Qb8m3d5Tq733WWC9McNhlGI,208
 everai/app/app.py,sha256=fweD6GNTR0vCCFvYDXSzZOIcphOEhM5nOlcXDA_kB3M,3667
-everai/app/app_manager.py,sha256=SbDljStWdJSImjG6yIaA4KwUeU3G1NhfUmofrXXfRUE,11070
+everai/app/app_manager.py,sha256=QW9OLOjD1-PGljjl1cZXfZD1gyf3EC8gAztnDx-m9QA,11207
 everai/app/app_runner.py,sha256=HVlOLweFX-C2kBbgyVwuDz4vfGzQ6uzHpNVzikQhRfA,1791
 everai/app/app_runtime.py,sha256=zyj63A6VfM1P3WL7LVW_mcy9xmMwKueKzTcJduGMwSo,3223
 everai/app/app_setup.py,sha256=CLXAC83OyTqEjAEKNLHQaCT3UPhvw149mD1VQr-AEEg,2568
 everai/app/autocaling_handler.py,sha256=Exsdti0N16GlcqXIILJ1qa6_DN9cBwzWpahukDKiqEo,1116
 everai/app/context.py,sha256=BIZ0FOozDTVCZg-cWMUnpf9DEjKF2r5T1MRF8yWreG4,2320
 everai/app/service.py,sha256=tn202UvWjK3Zr34MTQB_XhrGwXYe-NqgQtdTFncrgYk,2965
 everai/app/typing.py,sha256=d7tPA7VoDY771u-v0DLwD6TTMfPotg8u_PAshDcHRQo,210
 everai/app/volume_request.py,sha256=BjyGnehuqDxXVqdc1Xq0CL0GMT-r2IExe2bmyCMVXSU,327
 everai/autoscaling/__init__.py,sha256=7KlzpxRDIFkIdEoh5Rjw32rhCGtbIqv_oN_JSHajqFY,310
 everai/autoscaling/action.py,sha256=Hat74A4kk4BMjZAAdIcX5yr1CQm64BaNhOE3t7ooJ7Q,901
 everai/autoscaling/autoscaling_policy.py,sha256=i-znbnCG3w1ovmInhFlEwDdC54MFQ3Q9qhvK86jboIE,291
 everai/autoscaling/autoscaling_policy.pyi,sha256=u_OuXVbYDdu09a-ej0j3eURTMeKfJuqvEOHGB8kifG8,184
 everai/autoscaling/factors.py,sha256=9Dg0ZpcAI2TpRSEtHaLvDK7umKGWn1FiQ004nucl8kA,1943
 everai/autoscaling/session_autoscaling.py,sha256=tnNs91zBLFfWA7kuvlJEs5eQ_MHUUa6R0UAXhxOBEc0,698
-everai/autoscaling/simple_autoscaling.py,sha256=ts9G4oNmBRVdSCodIuor5N2_rsuq373j2pmoC-ke380,4666
+everai/autoscaling/simple_autoscaling.py,sha256=blrkWse9nM39nBSJZf61m2ildtabYmnOuJKb2OMCz8c,4682
 everai/autoscaling/wellknown.py,sha256=kUa7XlknGph-XR_qjI2PpEAcNYANXtlXctvHi-OsxVM,64
 everai/commands/__init__.py,sha256=o1tcmQ2Hds3eW_8ybbs39rlUWh5uu0dQ4DkgdEnoMGI,55
 everai/commands/everai_cli.py,sha256=3-FEdOHXG5Tu5Kfm_Z_JnDaJOXn-AbEeowzfBP47PHU,1683
 everai/commands/app/__init__.py,sha256=bZsGYyqZz9ewwBfaEknc6dp8H7_z-QmXK5IyuAEfNto,163
 everai/commands/app/app.py,sha256=_QUKmvb4FFMwSBlAGytDDOi7ZhyckMD3SYmk7RDD7k4,1187
 everai/commands/app/create.py,sha256=KEN7KV0yHCqmwFmEqq2EB8b-gQ-Z8pny4joBBG4xr6A,1407
 everai/commands/app/deploy.py,sha256=o0yF3qHbpqwcMn5TY83UbZkwCPIt4UA8ckmxHQDCl9o,676
@@ -44,44 +44,47 @@
 everai/commands/command/command.py,sha256=7H3jMPHknnBDaxxn-SMOnxgMTMuk4hc-5ssrcHx2vnI,405
 everai/commands/command/decorator.py,sha256=cjG5ZBsgnhBs2vt_p5VwOG6RzDWW-I4c_AAFBtQ4AU4,362
 everai/commands/command/list_utils.py,sha256=hwx_bRD2tCrU7EmoM0ykO2feJj3Sr4dvkdzuOPYYT2Y,2214
 everai/commands/command/setup_subcommands.py,sha256=dt3OZ5jPQ9gFIgR_23C0fybtMrjeRmnR4mG27YOI5VY,341
 everai/commands/config/__init__.py,sha256=61pHrxuovd2Rz4wKj9MPbHWV8UuWIrZcUn2tTa15eGA,62
 everai/commands/config/config.py,sha256=xzEyyTWu-igHIOINKkwobqhMeYZhq3jlfNZnb3elX6o,701
 everai/commands/configmap/__init__.py,sha256=LhvxscGN2UkW59o2xdEmuemTioxZLRWUTrdCqycD4Gk,72
-everai/commands/configmap/configmap.py,sha256=tsaqRfLvSySGF-hGtllgXryPQTd1VJP4uW66qKEQhTM,1289
-everai/commands/configmap/create.py,sha256=cpm0Cytfv5TsHQZSiwvgkVt6qWeWlix1mbngdhu3LNI,2008
-everai/commands/configmap/delete.py,sha256=0CQI7wtH0cnTV_YQ5B8HDft6wYm6aykLwJjqvt3Upxg,711
-everai/commands/configmap/get.py,sha256=ix62gr_FpU9WcT0sjL8nfS94c14iPFsAOb7IRJG5L34,837
-everai/commands/configmap/list.py,sha256=hwhnH9FzAsABA73ub6eQxvEaEvCnZAKYyum_dYiw_-w,723
+everai/commands/configmap/configmap.py,sha256=mG5Jym_NJx4Sqz3TVENTWXvh0U5NHSmucFmBmoPhaCs,1305
+everai/commands/configmap/create.py,sha256=b1s6qDp7_NcRIiskqz4rTz6b6EnexqDD6vjwvfuCs7s,1995
+everai/commands/configmap/delete.py,sha256=8HI5lBdfhe0t7XZDISQyE_kTujjGsT0Uy_6vzLiBHIk,693
+everai/commands/configmap/get.py,sha256=vUVgvR20iPP2k00sq2zuKuXr7jOISklzsi0o_UmOUWw,819
+everai/commands/configmap/list.py,sha256=5f9-JmKaI39WDGmsMLucbQQRYqaUcFTO3fbE8V6lLkY,705
+everai/commands/configmap/update.py,sha256=3r1Esk1E69YRe7UKFqTL3v_dIrO1yZUl4wklAtz6bFQ,1995
 everai/commands/image/__init__.py,sha256=gEvksUFimk0y9_a1D78kgxR74FmjqqvMnoEW4lbV9QM,60
 everai/commands/image/build.py,sha256=xtmpYT_ooxmQfcJshdPUYbvQ1ueCPX9Wy4t3kxTB6lc,734
 everai/commands/image/image.py,sha256=J_GWCLdmyUzCJ0J60h1n6bohDLnEiyFCErAycPiBvBo,831
 everai/commands/run/__init__.py,sha256=K0Z4YQiwfP1S7Ac-0YyxnnRatfTJ2WKe7Nbs-qMyw7k,54
 everai/commands/run/run.py,sha256=weCezbI9fX4Hsc-Qw2uUf4mzzfiIcsJEWfAX2YI0r8A,925
 everai/commands/secret/__init__.py,sha256=O4Tj-pg2EGxcF7y_HWLsY0PAxE-cB09iGmyzrvaALiI,63
-everai/commands/secret/create.py,sha256=ztJtQikFFF7C4YHQkQP-EtxSzMIMhR40D-MrGUg427w,1840
-everai/commands/secret/delete.py,sha256=JhmqYyywPzq67rAutojGoIyJSduecJG522QTT1-6haE,680
-everai/commands/secret/get.py,sha256=pgXYDaU25bMzJnJbrKx6iGiVIZn84-iDU0b6pOfllf0,965
-everai/commands/secret/list.py,sha256=_XyAO8hmK3KkMRpJgYcfD_6pU4wFKdlSYWiORZbgzrQ,777
-everai/commands/secret/secret.py,sha256=-8vvk02gr9st6-ocCDgxb586nLkC_mpPllq9Nl68jDk,1206
+everai/commands/secret/create.py,sha256=okYRA3JDdrP7o6l_82C0_CLFruOEEMGaoALHCprBmxk,1833
+everai/commands/secret/delete.py,sha256=Us6aoFymKcq0vkC6pZb9aTvYjvC5W--ZHNHT9UvY3a0,668
+everai/commands/secret/get.py,sha256=bfOUasLLVMAHacfr8xUUs-Ah_2FB_mr8VnIKvFX_oxI,783
+everai/commands/secret/list.py,sha256=1ynwbElHGKldMDheplUx4Q73UGpuByefpyHC0bIYs3k,765
+everai/commands/secret/secret.py,sha256=tsBdfkKE9noNpe7v-qhtf7lfgNQqkkuHM6j6YJ63fhU,1243
+everai/commands/secret/update.py,sha256=Ukp0xzahxKeiEmuYKdEbelvWT20DBGak0FS5blLU-cg,1921
 everai/commands/volume/__init__.py,sha256=UlxXpx7spko6zt5QASgQf3FvKMFWVDs0z6kc9ET_Z3M,63
 everai/commands/volume/create.py,sha256=zX4Jnx81NQjK82tZsatl-ZCtQKKf5mcMz2TTRmg4Szo,813
 everai/commands/volume/delete.py,sha256=OzKZ9AN4tHQO9orWhUeIxgVxfhHgGDKWF2PG95yHgC8,1679
 everai/commands/volume/get.py,sha256=ruLx6zRKnmUZdpXhxHF2C1XIVgGaa1zLlnfU-nX0bfE,752
 everai/commands/volume/list.py,sha256=YmjnCWIl3pyDxE-F7rOmhDZu2PrlGFsR6MacnJlOFmY,747
 everai/commands/volume/pull.py,sha256=sJKByR1qWxCreb6BMj3kfbhM7w2UuO5eKySDMPtp7lQ,1507
 everai/commands/volume/push.py,sha256=lH_EB0joXOKGY4lPalWkmAPnCesDiytfhzfW_0E4jQA,753
 everai/commands/volume/volume.py,sha256=k6aTAZBo1TZGoTRRJUhVMaWglUey5nTJQm94m8-FBz8,1395
 everai/commands/worker/__init__.py,sha256=8Sswddw1RHWdpl7AHrktEodBITDspvtESL0GnPI0Oo0,69
 everai/commands/worker/list.py,sha256=K1LrybGwRpm54JndgC1Kn0tkY4FxLy-eAZ47xSAE_s4,910
 everai/commands/worker/worker.py,sha256=pInYtKYjueNPPzuMNSBwbAWOPCdnL-DYBdF6VSlCfM8,851
-everai/configmap/__init__.py,sha256=vxD7awli4BPSNCWA17I5_zTcNRZ5U0eHNr05WeIUGMU,127
+everai/configmap/__init__.py,sha256=xKvP74DWxu5UrMrLiI1_9S1AfqZErlRotGnShY_5cec,270
 everai/configmap/configmap.py,sha256=zZnYKH7aZd2DCeGSyu9kEExwTI5bpXlcQjufDk5e1-g,1498
-everai/configmap/configmap_manager.py,sha256=VDulfQsMBlHeBZxbaJ2JuIXbbNMvK57U4JBYQsO5Hr8,1479
+everai/configmap/configmap_manager.py,sha256=CRRsG63ei7gN95Va5tYrRXHlXTY_lVm0YEYtgTHDKyE,1848
+everai/configmap/utils.py,sha256=OCaJQbnQ810Vs-gjmJnjkT9ibhsQfuLUBlS7Yzdqnjk,741
 everai/image/__init__.py,sha256=vJJvzDkVDL538QQDc5QpbOKVNUCLgE4SlpotcoSmuqE,157
 everai/image/auth.py,sha256=Gi2ljWsVAoLaECQd1mFoCGBdi3g1e47g3loqwnK-iAo,483
 everai/image/builder.py,sha256=-BjhzGkeyScQH56p7VgX6uMNA9mwcNlR_QEzJLQqMk0,3317
 everai/image/image.py,sha256=XZ-L52PQu9whVZsexdYwT4au07ZVdgUMBQJrBKn2hJI,1046
 everai/logger/__init__.py,sha256=NAQI0glOTo-dcqGjFbV7zibyTXRGeN_odPXTCWugyqs,223
 everai/logger/logger.py,sha256=2hZC5GoQDPiu-rxyIDOQpF7_3h6yAWjptPb9NhTcWps,1798
 everai/placeholder/__init__.py,sha256=iJ1uynS7deIF-jIbxoHjRmaPt4jRwSkcOwMVvCNAUQM,70
@@ -89,15 +92,15 @@
 everai/resource_requests/__init__.py,sha256=J6KPJsS_sJ2mHIZ91tLVirEYWHn00noKqRrWyUlOVcQ,79
 everai/resource_requests/resource_requests.py,sha256=4T988kqofw6mNDZ6um9PMZqPKLsofhJ96yHZc4_WnG4,1686
 everai/resource_requests/wellknown.py,sha256=ovZYPhqU9UOvspcspxTGrMinAbliUk3yW9DtrQLCKx4,211
 everai/runner/__init__.py,sha256=NBFNeWn13HRoosc8NsveaVv672NaEd5hoz4rLzqoPgI,95
 everai/runner/run.py,sha256=dIpGMxEW9MAg2lSjainHUDJgthUa9kuJu14KT70skHw,2403
 everai/secret/__init__.py,sha256=8F3idFvuD9b43LM5-svA0ePhWUYs3I_ZKIwImyat8jw,109
 everai/secret/secret.py,sha256=Brb3Y99gRPdDz98_M7phs023mkGP2S0_pL5S0CrqJqo,2118
-everai/secret/secret_manager.py,sha256=1M3mIu_hLRWvv9uiriJERwCTxaTdoX5dEBXwQfJKegY,1484
+everai/secret/secret_manager.py,sha256=JS0n6lYObHTfTNqGap4jNzYRMkbjlA2qz_DfGY1pLX0,1814
 everai/token_manager/__init__.py,sha256=P6WP0oZauizhzf3zEBa92vtI3n2jfNmWznbiTbSsHPo,67
 everai/token_manager/token_manager.py,sha256=PMRHRISgJZKe9WEQ3ioY5-2iGIdG6nmDszaJY_fNpPI,1547
 everai/utils/__init__.py,sha256=OnSV1ofyEZ4OqJ3A7LpCNFDUp5g7aqv99MAox_77E2w,62
 everai/utils/bool.py,sha256=FhWoDUvb-3cUJuMkEwPoRLykUMsgwcEe-vi_KzbYtcw,150
 everai/utils/cmd.py,sha256=M-tWnwworr6heXZAC_62U2rxzzfKXVgNJaG7pilg0P0,1451
 everai/utils/datetime.py,sha256=v9CwIoXfcsT3oBCr7yiBqOqg4C4VLsguhJEITRT0HCg,338
 everai/utils/docker_manager.py,sha256=L0k8D9n2wVyW0tuwhsVo8uG2wWoUrSJvxYVODwtNvKs,6189
@@ -110,29 +113,31 @@
 everai/utils/verbose.py,sha256=aQ-nRJaMvhAia7Id_kM-2d5CHij4vudJdKSfyiSnHlw,153
 everai/volume/__init__.py,sha256=_nJ-S-Sgec1jY6byu-u9EOYE7-_1iaMj-kcM-v6pTaY,107
 everai/volume/volume.py,sha256=lW0-z0eIFhMKcz1dSPKMBNMXuQq_a17lTph6gO3Xh0Y,5148
 everai/volume/volume_manager.py,sha256=TZabXDog9dP8-QxsT7yBzBvsnuSEXiT7WM7aHba3qkU,14731
 everai/worker/__init__.py,sha256=J8ziddB4caVoslM3FG445bwHAjl9donqX3Bcn7yX3ts,55
 everai/worker/worker.py,sha256=MIS-hKL82q4-Z8L5XCh64l2PlrNxM0Gfmqz4MJpbtoY,1918
 generated/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-generated/configmaps/__init__.py,sha256=jQSfRo01wgdUiK8j8i43id14Zk6htP4eaLTDWVBvB84,1316
+generated/configmaps/__init__.py,sha256=qMsKjxY-Pzah_zlnImcqfkzzTxxl0fSKQst-JyMkhrE,1413
 generated/configmaps/api_client.py,sha256=MAq1ipqq9qhlpjWTF-fjisZeKXnVoCEmly2RJu00geM,29579
 generated/configmaps/api_response.py,sha256=uCehWdXXDnAO2HAHGKe0SgpQ_mJiGDbcu-BHDF3n_IM,852
 generated/configmaps/configuration.py,sha256=eF8KQFEyVDwkTOUtAC8O6Eq4XYMKhYOCtnuwpE7CXKU,14419
 generated/configmaps/exceptions.py,sha256=MDHay-pkZc1HraJau1WBt1xRPQlgEWqqi99_Em0Kfhs,5462
 generated/configmaps/rest.py,sha256=20aaCMcXs2dd6sHjReXFoUh0a1hI0byPX8hxYxcR888,12966
 generated/configmaps/api/__init__.py,sha256=aKYR_hq-5vxsXqGH4tLXOpinVirw-bVUrevAz8wxujc,127
-generated/configmaps/api/configmap_service_api.py,sha256=f4YRcDisTdU8Ivs131aIXNso4U_ufz55PcVcEqLF660,25423
-generated/configmaps/models/__init__.py,sha256=MxMuZ2BTNgFZeAtR-wBaw4Xd8Y5JRglwbrZxPwoO0to,639
+generated/configmaps/api/configmap_service_api.py,sha256=4W2NbgqBn4s0k0Vm2MAweIKCuA8D_i4EC7WBe-Zu7OY,32156
+generated/configmaps/models/__init__.py,sha256=0zsqNcY7OIRwHjeni9J7civWvshua-swMbJueX-kNpQ,736
 generated/configmaps/models/configmap_service_create_body.py,sha256=dUxVH5V5jVSKlARVjrA3m3PcyyW5N6nFz2dO9kUaBpc,2555
+generated/configmaps/models/configmap_service_update_body.py,sha256=FgR0YtwXGtML8oDPzzVyk2a0cPR-oKP1M0tIWpGlP1A,2555
 generated/configmaps/models/v1_configmap.py,sha256=XtoZE5N_2uWgrj70xXvla3Llg9DCWhCm6KWpT8fHpyk,2764
 generated/configmaps/models/v1_list_response.py,sha256=LKnChj1rmmH7h6ukKQl340RlQAoGg8lEpxjoMMKaBIs,2906
 generated/configmaps/test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 generated/configmaps/test/test_configmap_service_api.py,sha256=zkWVK6Cl7l9QSzDFS29qTOkrKqJQVdmakBsmeSF8_NY,1357
 generated/configmaps/test/test_configmap_service_create_body.py,sha256=CFNSGC7a3Wm4MMXqsbSNB4M5cDOPPeCT8rtACSrGUIw,1824
+generated/configmaps/test/test_configmap_service_update_body.py,sha256=Do-mRawEV2CqUbVuGAUUREmaBr2eDoL89DZEw248e74,1824
 generated/configmaps/test/test_v1_configmap.py,sha256=z_Aa474XGFDwtWoM3Ftk-FlUAMfyy58oipSfwhOmZPM,1775
 generated/configmaps/test/test_v1_list_response.py,sha256=WfadsDDBQX0iCqYDrtxarIHDlRS9wptPkac4YMUa_fQ,1930
 generated/schedulers/__init__.py,sha256=PWdjNvbCC34iumuELh1oupYXixG3iJFBPlZ8gREeu5o,6396
 generated/schedulers/api_client.py,sha256=e0gJTxEW9DNd3JO6gXX5RiS7__tvmFpHqmafJ6OAkvg,29587
 generated/schedulers/api_response.py,sha256=uCehWdXXDnAO2HAHGKe0SgpQ_mJiGDbcu-BHDF3n_IM,852
 generated/schedulers/configuration.py,sha256=8yD32fbOFvv0bdSME_YPE9IIOxUDR4shn9QIKyXQJDA,14427
 generated/schedulers/exceptions.py,sha256=MWXsijYmwsAKt57vGF9DIX-2on7-91iGlbhxSEuz2Jo,5470
@@ -316,29 +321,31 @@
 generated/schedulers/test/test_v1_worker.py,sha256=sCxwFsZvcmf8lRwxeinIrCENr3k-cyJnbsPGilS39xc,1891
 generated/schedulers/test/test_v1_worker_request.py,sha256=txevxkrZwlu47D1kmAZujiLJZT_Kf_O2BRUG47tPM78,2991
 generated/schedulers/test/test_v1_worker_status.py,sha256=ANHgI-fxVvXwP0zU2eNAGSzrO3oavu4kLJ-l3stvnOA,793
 generated/schedulers/test/test_v1_worker_worker_status.py,sha256=yxSkwK7d7HYfm3974yYxzF2Z5Wq0aPCgzOWk2SV-xwY,836
 generated/schedulers/test/test_v1workersv1_worker.py,sha256=HQlKbCt8yvYJ3vBiLw4cBQKfBiHSIu1UuZh4DQgLEGg,1999
 generated/schedulers/test/test_volumesv1_volume.py,sha256=F-OGuyTKLJBVA5n4xgfrCDBOlV6te-IaaoSDNlbPVws,1576
 generated/schedulers/test/test_workersv1_worker_status.py,sha256=6Nznu_sfgKBoXg1EpgNoIsGYSajBCA0vTxxwmCyV3vY,842
-generated/secrets/__init__.py,sha256=AHNXPEZrE4UlkQiMc7QRaUCH40EZINNOvJz9tsSz0fA,1256
+generated/secrets/__init__.py,sha256=y_sDoHK-CvHWWIuFHK53VaMFwc23cBlPe0kkViPaQ54,1344
 generated/secrets/api_client.py,sha256=bmsoKmdJNCCMGb0kLeHFiYsb49VEXR5MuCX1RpSdIcw,29558
 generated/secrets/api_response.py,sha256=uCehWdXXDnAO2HAHGKe0SgpQ_mJiGDbcu-BHDF3n_IM,852
 generated/secrets/configuration.py,sha256=8_ax7BJWUXvhUABdFBCTD2X5Vi-NomtxE3fv9V5eDQE,14413
 generated/secrets/exceptions.py,sha256=MUvjQqROv7kXGTJnJ4JhweWSv0wwla3T_ZJQH-fzbSc,5459
 generated/secrets/rest.py,sha256=8pMVu2zTuDw3kURFhoUEiueK4oH9q2ZllO7ska3NJ5k,12960
 generated/secrets/api/__init__.py,sha256=mVjfEgdP-u2gSgkreFvbg0vv2gPUzU0e6K5syAyj-lw,118
-generated/secrets/api/secret_service_api.py,sha256=c9g8gpMleShTbmtZn5S824FksyfscRdOkRdh5XuKSR4,25093
-generated/secrets/models/__init__.py,sha256=n0TrGEkzGyNGKWxYhlUBD_2dzd4MXegOxRNt0PodmLo,615
+generated/secrets/api/secret_service_api.py,sha256=QSudmu40xdIFxMUg8Fy2X33kEwIXKRDSm8BBUhRYano,31721
+generated/secrets/models/__init__.py,sha256=AOnYQZjxc7rJqQF0MlTUmQU4JHa8bmWSbcA5J_7trj8,703
 generated/secrets/models/secret_service_create_body.py,sha256=vgtmSSohFHf1kkRY9R1DrTEFEiZmku86mCafiyI5puI,2540
+generated/secrets/models/secret_service_update_body.py,sha256=MT8wPeacyDSrqtxMciWnHrP4RvtuxrqtOYLDt2-FF78,2540
 generated/secrets/models/v1_list_response.py,sha256=huCcVzTi2gbm97L_3oDkxPtX19EjgMHiT2LQyS9pNeY,2861
 generated/secrets/models/v1_secret.py,sha256=yAi4mA-i_TDykKBDi21SKHhNHYdL9DHi02e-Crvvaic,2749
 generated/secrets/test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 generated/secrets/test/test_secret_service_api.py,sha256=GIFO1TTZ5MGvP4XnTWpahK3RcdW8vR_3iswq9-Zxk5M,1297
 generated/secrets/test/test_secret_service_create_body.py,sha256=eeuiYfAQkguxgQGD3mUcmWMz4sJNL-MhOLkxv-BXepo,1680
+generated/secrets/test/test_secret_service_update_body.py,sha256=CIBEh3HEo-AJ_yy0PQgkRUu9t3TK5D2dxidq1THryNk,1782
 generated/secrets/test/test_v1_list_response.py,sha256=wsZUJa8-6SBoDNh2Unq2Yvit7g9EL_uVbm1OS5o4lhQ,1845
 generated/secrets/test/test_v1_secret.py,sha256=sp1Zw1rraRdo4U3YhwKTCgQbjfqrZ3v1R5EKMGfOhJE,1603
 generated/volumes/__init__.py,sha256=HxwVvzZ7fTycXxp6w4M7Ig_Y0i5FK0HhJVj__E_fVps,2928
 generated/volumes/api_client.py,sha256=leHtpUUBjAKU9ltZhZWmlk_EIDkXRymy6jZFvTNd9FA,29558
 generated/volumes/api_response.py,sha256=uCehWdXXDnAO2HAHGKe0SgpQ_mJiGDbcu-BHDF3n_IM,852
 generated/volumes/configuration.py,sha256=npRZ4V64YFnkCj2tkjEmUyfryXu0VBEqLj-xpeGAq-I,14413
 generated/volumes/exceptions.py,sha256=8d40RdHzGPWJrid1jnWmwfN-AzUUQV9hHPTojnZXugY,5459
@@ -388,13 +395,13 @@
 generated/volumes/test/test_volume_service_commit_file_body_file.py,sha256=F4jWVTlpo82x5j68w3hYpaHvaUZhCiFrmBSo1SVZOu0,1912
 generated/volumes/test/test_volume_service_commit_revision_body.py,sha256=UizO6O0rY4b9isgc_d2lKBUwTlCn0kiefccAD86nCcs,2548
 generated/volumes/test/test_volume_service_complete_multipart_upload_body.py,sha256=Ek6ZP78kDn1ol-guEmhm2zA42c_6XkArQf8G-_L5MgI,2233
 generated/volumes/test/test_volume_service_create_body.py,sha256=2MA4PEVNwPpMGuvpwMu4qeYvDAjrZjyUaeuo9p3qJ1c,1624
 generated/volumes/test/test_volume_service_initialize_multipart_upload_body.py,sha256=G58739S9489bMEXfaefcWch_GqgV-PTw4QCewOzxhSs,2149
 generated/volumes/test/test_volume_service_sign_multipart_upload_body.py,sha256=3b5ULrWgH38nEWU0s_MISEyj4j6LV8doFAx3CfQ6XjY,1769
 generated/volumes/test/test_volume_service_sign_upload_body.py,sha256=xX2B1LCvIu0OHX0AkyL8dXPClBTDgmZwmgPJOjjz96g,1968
-everai-0.1.34.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-everai-0.1.34.dist-info/METADATA,sha256=_qCbgJAsNzEKzgXkyEwseptWbbbL_GbfuY0wXJFzn1o,1951
-everai-0.1.34.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-everai-0.1.34.dist-info/entry_points.txt,sha256=JB8rwg4N4ctezo4f9O0QbWJkivM_s-wUhOn0mPM9xug,98
-everai-0.1.34.dist-info/top_level.txt,sha256=UNE90t4nA-FVpeYLiqPcJVSFyaKbZ-ERHUNI0Qd6co8,17
-everai-0.1.34.dist-info/RECORD,,
+everai-0.1.35.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+everai-0.1.35.dist-info/METADATA,sha256=hWRUE41CNWLiyX0uervKyomcVuVT151RWXU24ZxLrwc,1951
+everai-0.1.35.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+everai-0.1.35.dist-info/entry_points.txt,sha256=JB8rwg4N4ctezo4f9O0QbWJkivM_s-wUhOn0mPM9xug,98
+everai-0.1.35.dist-info/top_level.txt,sha256=UNE90t4nA-FVpeYLiqPcJVSFyaKbZ-ERHUNI0Qd6co8,17
+everai-0.1.35.dist-info/RECORD,,
```

