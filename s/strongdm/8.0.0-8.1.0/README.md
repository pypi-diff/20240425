# Comparing `tmp/strongdm-8.0.0.zip` & `tmp/strongdm-8.1.0.zip`

## zipinfo {}

```diff
@@ -1,132 +1,132 @@
-Zip file size: 376498 bytes, number of entries: 130
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 19:47 strongdm-8.0.0/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 19:47 strongdm-8.0.0/strongdm/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 19:47 strongdm-8.0.0/strongdm.egg-info/
--rw-r--r--  2.0 unx     2875 b- defN 24-Apr-09 19:46 strongdm-8.0.0/README.md
--rw-r--r--  2.0 unx    11342 b- defN 24-Apr-09 19:46 strongdm-8.0.0/LICENSE
--rw-r--r--  2.0 unx     1908 b- defN 24-Apr-09 19:47 strongdm-8.0.0/setup.py
--rw-r--r--  2.0 unx     3599 b- defN 24-Apr-09 19:47 strongdm-8.0.0/PKG-INFO
--rw-r--r--  2.0 unx       38 b- defN 24-Apr-09 19:47 strongdm-8.0.0/setup.cfg
--rw-r--r--  2.0 unx     8792 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflows_history_pb2.py
--rw-r--r--  2.0 unx     3361 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/replays_pb2_grpc.py
--rw-r--r--  2.0 unx     5092 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/activities_pb2_grpc.py
--rw-r--r--  2.0 unx    29219 b- defN 24-Apr-09 19:47 strongdm-8.0.0/strongdm/accounts_pb2.py
--rw-r--r--  2.0 unx     7476 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/role_resources_pb2.py
--rw-r--r--  2.0 unx    17204 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_approvers_pb2.py
--rw-r--r--  2.0 unx     6849 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/secret_store_healths_pb2_grpc.py
--rw-r--r--  2.0 unx      808 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/__init__.py
--rw-r--r--  2.0 unx     3424 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/remote_identities_history_pb2_grpc.py
--rw-r--r--  2.0 unx     3505 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_approvers_history_pb2_grpc.py
--rw-r--r--  2.0 unx     8901 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_resources_pb2.py
--rw-r--r--  2.0 unx    18385 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/roles_pb2.py
--rw-r--r--  2.0 unx     9416 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflow_approvers_history_pb2.py
--rw-r--r--  2.0 unx      741 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/options_pb2_grpc.py
--rw-r--r--  2.0 unx   433936 b- defN 24-Apr-09 19:47 strongdm-8.0.0/strongdm/plumbing.py
--rw-r--r--  2.0 unx    12455 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/resources_pb2_grpc.py
--rw-r--r--  2.0 unx     3259 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflows_history_pb2_grpc.py
--rw-r--r--  2.0 unx     7818 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/nodes_history_pb2.py
--rw-r--r--  2.0 unx      741 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/spec_pb2_grpc.py
--rw-r--r--  2.0 unx     3557 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/access_request_events_history_pb2_grpc.py
--rw-r--r--  2.0 unx     3420 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/queries_pb2_grpc.py
--rw-r--r--  2.0 unx     7932 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/peering_groups_pb2_grpc.py
--rw-r--r--  2.0 unx     3111 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/nodes_history_pb2_grpc.py
--rw-r--r--  2.0 unx     8550 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_grants_history_pb2.py
--rw-r--r--  2.0 unx    17034 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/organization_history_pb2.py
--rw-r--r--  2.0 unx     8412 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/secret_stores_history_pb2.py
--rw-r--r--  2.0 unx     3223 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/resources_history_pb2_grpc.py
--rw-r--r--  2.0 unx     6176 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/remote_identity_groups_pb2_grpc.py
--rw-r--r--  2.0 unx    17214 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/secret_stores_pb2.py
--rw-r--r--  2.0 unx     3479 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_assignments_pb2_grpc.py
--rw-r--r--  2.0 unx     8773 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_resources_history_pb2.py
--rw-r--r--  2.0 unx    27237 b- defN 24-Apr-09 19:47 strongdm-8.0.0/strongdm/client.py
--rw-r--r--  2.0 unx    16423 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/peering_group_peers_pb2.py
--rw-r--r--  2.0 unx     8708 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflow_approvers_pb2_grpc.py
--rw-r--r--  2.0 unx     9790 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/remote_identities_pb2_grpc.py
--rw-r--r--  2.0 unx      741 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/drivers_pb2_grpc.py
--rw-r--r--  2.0 unx     3470 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_permissions_pb2_grpc.py
--rw-r--r--  2.0 unx     8983 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/access_request_events_history_pb2.py
--rw-r--r--  2.0 unx    29937 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/nodes_pb2.py
--rw-r--r--  2.0 unx     3320 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/organization_history_pb2_grpc.py
--rw-r--r--  2.0 unx     3493 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_attachments_history_pb2_grpc.py
--rw-r--r--  2.0 unx   893989 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/drivers_pb2.py
--rw-r--r--  2.0 unx    16584 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_grants_pb2.py
--rw-r--r--  2.0 unx     3388 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_resources_pb2_grpc.py
--rw-r--r--  2.0 unx    15576 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/access_requests_pb2.py
--rw-r--r--  2.0 unx     9837 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/nodes_pb2_grpc.py
--rw-r--r--  2.0 unx     9376 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/secret_stores_pb2_grpc.py
--rw-r--r--  2.0 unx     3295 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/role_resources_pb2_grpc.py
--rw-r--r--  2.0 unx    17173 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/peering_group_resources_pb2.py
--rw-r--r--  2.0 unx     8102 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_attachments_pb2_grpc.py
--rw-r--r--  2.0 unx     8478 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/role_resources_history_pb2.py
--rw-r--r--  2.0 unx     8167 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/peering_group_peers_pb2_grpc.py
--rw-r--r--  2.0 unx     9665 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflows_pb2_grpc.py
--rw-r--r--  2.0 unx     8646 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/access_requests_history_pb2.py
--rw-r--r--  2.0 unx     8961 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_assignments_history_pb2.py
--rw-r--r--  2.0 unx     3561 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/remote_identity_groups_history_pb2_grpc.py
--rw-r--r--  2.0 unx     6598 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/control_panel_pb2_grpc.py
--rw-r--r--  2.0 unx     3198 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/accounts_history_pb2_grpc.py
--rw-r--r--  2.0 unx     3465 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflows_history_pb2_grpc.py
--rw-r--r--  2.0 unx     3390 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_roles_history_pb2_grpc.py
--rw-r--r--  2.0 unx     3417 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/access_requests_history_pb2_grpc.py
--rw-r--r--  2.0 unx    16079 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_roles_pb2.py
--rw-r--r--  2.0 unx     4600 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/tags_pb2.py
--rw-r--r--  2.0 unx     8650 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/remote_identities_history_pb2.py
--rw-r--r--  2.0 unx     8320 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/replays_pb2.py
--rw-r--r--  2.0 unx    16300 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/activities_pb2.py
--rw-r--r--  2.0 unx     7340 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_assignments_pb2.py
--rw-r--r--  2.0 unx     3353 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_grants_history_pb2_grpc.py
--rw-r--r--  2.0 unx   202826 b- defN 24-Apr-09 19:47 strongdm-8.0.0/strongdm/svc.py
--rw-r--r--  2.0 unx     3592 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflow_steps_history_pb2_grpc.py
--rwxr-xr-x  2.0 unx    18511 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/constants.py
--rw-r--r--  2.0 unx     8255 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/peering_group_nodes_pb2_grpc.py
--rw-r--r--  2.0 unx     9027 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/remote_identity_groups_history_pb2.py
--rw-r--r--  2.0 unx      741 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/tags_pb2_grpc.py
--rw-r--r--  2.0 unx     3322 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/secret_stores_history_pb2_grpc.py
--rw-r--r--  2.0 unx    15297 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/peering_groups_pb2.py
--rw-r--r--  2.0 unx      741 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/secret_store_types_pb2_grpc.py
--rw-r--r--  2.0 unx     7980 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_grants_pb2_grpc.py
--rw-r--r--  2.0 unx    20122 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflows_pb2.py
--rw-r--r--  2.0 unx     8404 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflow_steps_pb2_grpc.py
--rw-r--r--  2.0 unx     9960 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflows_pb2_grpc.py
--rw-r--r--  2.0 unx     3180 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/access_requests_pb2_grpc.py
--rw-r--r--  2.0 unx    17037 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_attachments_pb2.py
--rw-r--r--  2.0 unx     3350 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/role_resources_history_pb2_grpc.py
--rw-r--r--  2.0 unx     3111 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/roles_history_pb2_grpc.py
--rw-r--r--  2.0 unx    19200 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/queries_pb2.py
--rw-r--r--  2.0 unx    14899 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/options_pb2.py
--rw-r--r--  2.0 unx    17070 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflow_steps_pb2.py
--rw-r--r--  2.0 unx    18708 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflow_approvers_pb2.py
--rw-r--r--  2.0 unx     9758 b- defN 24-Apr-09 19:47 strongdm-8.0.0/strongdm/accounts_pb2_grpc.py
--rw-r--r--  2.0 unx     8546 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/peering_group_resources_pb2_grpc.py
--rw-r--r--  2.0 unx     8901 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_attachments_history_pb2.py
--rw-r--r--  2.0 unx    75244 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/secret_store_types_pb2.py
--rw-r--r--  2.0 unx     8396 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_permissions_pb2.py
--rw-r--r--  2.0 unx     3434 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_resources_history_pb2_grpc.py
--rw-r--r--  2.0 unx    15880 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/spec_pb2.py
--rw-r--r--  2.0 unx     2196 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/errors.py
--rw-r--r--  2.0 unx     3704 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflow_approvers_history_pb2_grpc.py
--rw-r--r--  2.0 unx     8506 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_roles_history_pb2.py
--rw-r--r--  2.0 unx    22207 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/resources_pb2.py
--rw-r--r--  2.0 unx    11611 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/control_panel_pb2.py
--rw-r--r--  2.0 unx   788329 b- defN 24-Apr-09 19:47 strongdm-8.0.0/strongdm/models.py
--rw-r--r--  2.0 unx    16005 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/secret_store_healths_pb2.py
--rw-r--r--  2.0 unx     8138 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/accounts_history_pb2.py
--rw-r--r--  2.0 unx     9042 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/roles_pb2_grpc.py
--rw-r--r--  2.0 unx     8140 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflows_history_pb2.py
--rw-r--r--  2.0 unx    20009 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflows_pb2.py
--rw-r--r--  2.0 unx    16380 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/peering_group_nodes_pb2.py
--rw-r--r--  2.0 unx     3561 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_assignments_history_pb2_grpc.py
--rw-r--r--  2.0 unx     9113 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflow_steps_history_pb2.py
--rw-r--r--  2.0 unx     8165 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_approvers_pb2_grpc.py
--rw-r--r--  2.0 unx    19858 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/remote_identities_pb2.py
--rw-r--r--  2.0 unx     8808 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_approvers_history_pb2.py
--rw-r--r--  2.0 unx     8132 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/resources_history_pb2.py
--rw-r--r--  2.0 unx     7818 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/roles_history_pb2.py
--rw-r--r--  2.0 unx     9971 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/remote_identity_groups_pb2.py
--rw-r--r--  2.0 unx     8071 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_roles_pb2_grpc.py
--rw-r--r--  2.0 unx       50 b- defN 24-Apr-09 19:47 strongdm-8.0.0/strongdm.egg-info/requires.txt
--rw-r--r--  2.0 unx        9 b- defN 24-Apr-09 19:47 strongdm-8.0.0/strongdm.egg-info/top_level.txt
--rw-r--r--  2.0 unx     3599 b- defN 24-Apr-09 19:47 strongdm-8.0.0/strongdm.egg-info/PKG-INFO
--rw-r--r--  2.0 unx     4399 b- defN 24-Apr-09 19:47 strongdm-8.0.0/strongdm.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-09 19:47 strongdm-8.0.0/strongdm.egg-info/dependency_links.txt
-130 files, 3454949 bytes uncompressed, 354058 bytes compressed:  89.8%
+Zip file size: 378959 bytes, number of entries: 130
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 15:31 strongdm-8.1.0/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 15:31 strongdm-8.1.0/strongdm.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 15:31 strongdm-8.1.0/strongdm/
+-rw-r--r--  2.0 unx     3599 b- defN 24-Apr-25 15:31 strongdm-8.1.0/PKG-INFO
+-rw-r--r--  2.0 unx     1908 b- defN 24-Apr-25 15:31 strongdm-8.1.0/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 24-Apr-25 15:31 strongdm-8.1.0/setup.cfg
+-rw-r--r--  2.0 unx     2875 b- defN 24-Apr-25 15:31 strongdm-8.1.0/README.md
+-rw-r--r--  2.0 unx    11342 b- defN 24-Apr-25 15:31 strongdm-8.1.0/LICENSE
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     3599 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx     4399 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx       50 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm.egg-info/requires.txt
+-rw-r--r--  2.0 unx    15880 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/spec_pb2.py
+-rw-r--r--  2.0 unx     3353 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/account_grants_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     9665 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/workflows_pb2_grpc.py
+-rw-r--r--  2.0 unx     9042 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/roles_pb2_grpc.py
+-rw-r--r--  2.0 unx   795208 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/models.py
+-rw-r--r--  2.0 unx      741 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/secret_store_types_pb2_grpc.py
+-rw-r--r--  2.0 unx    19858 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/remote_identities_pb2.py
+-rw-r--r--  2.0 unx     7932 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/peering_groups_pb2_grpc.py
+-rw-r--r--  2.0 unx    17070 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/approval_workflow_steps_pb2.py
+-rw-r--r--  2.0 unx    16300 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/activities_pb2.py
+-rw-r--r--  2.0 unx     3417 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/access_requests_history_pb2_grpc.py
+-rw-r--r--  2.0 unx    17214 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/secret_stores_pb2.py
+-rw-r--r--  2.0 unx    16584 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/account_grants_pb2.py
+-rw-r--r--  2.0 unx     9971 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/remote_identity_groups_pb2.py
+-rw-r--r--  2.0 unx    16423 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/peering_group_peers_pb2.py
+-rw-r--r--  2.0 unx     8412 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/secret_stores_history_pb2.py
+-rw-r--r--  2.0 unx     6176 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/remote_identity_groups_pb2_grpc.py
+-rw-r--r--  2.0 unx     3259 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/workflows_history_pb2_grpc.py
+-rw-r--r--  2.0 unx    16079 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/workflow_roles_pb2.py
+-rw-r--r--  2.0 unx     3295 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/role_resources_pb2_grpc.py
+-rw-r--r--  2.0 unx    20009 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/approval_workflows_pb2.py
+-rw-r--r--  2.0 unx     8808 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/workflow_approvers_history_pb2.py
+-rw-r--r--  2.0 unx     3561 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/remote_identity_groups_history_pb2_grpc.py
+-rw-r--r--  2.0 unx    18708 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/approval_workflow_approvers_pb2.py
+-rw-r--r--  2.0 unx     9113 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/approval_workflow_steps_history_pb2.py
+-rw-r--r--  2.0 unx     7980 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/account_grants_pb2_grpc.py
+-rw-r--r--  2.0 unx    17034 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/organization_history_pb2.py
+-rw-r--r--  2.0 unx    12455 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/resources_pb2_grpc.py
+-rw-r--r--  2.0 unx     3390 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/workflow_roles_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     5092 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/activities_pb2_grpc.py
+-rw-r--r--  2.0 unx     9837 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/nodes_pb2_grpc.py
+-rw-r--r--  2.0 unx     3592 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/approval_workflow_steps_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     3420 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/queries_pb2_grpc.py
+-rw-r--r--  2.0 unx     8404 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/approval_workflow_steps_pb2_grpc.py
+-rw-r--r--  2.0 unx     3180 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/access_requests_pb2_grpc.py
+-rw-r--r--  2.0 unx     3322 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/secret_stores_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8792 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/approval_workflows_history_pb2.py
+-rw-r--r--  2.0 unx     3465 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/approval_workflows_history_pb2_grpc.py
+-rw-r--r--  2.0 unx    16005 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/secret_store_healths_pb2.py
+-rw-r--r--  2.0 unx     3479 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/workflow_assignments_pb2_grpc.py
+-rw-r--r--  2.0 unx    27237 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/client.py
+-rw-r--r--  2.0 unx     8650 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/remote_identities_history_pb2.py
+-rw-r--r--  2.0 unx     3505 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/workflow_approvers_history_pb2_grpc.py
+-rw-r--r--  2.0 unx   202867 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/svc.py
+-rw-r--r--  2.0 unx     8901 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/account_attachments_history_pb2.py
+-rw-r--r--  2.0 unx     3320 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/organization_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8708 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/approval_workflow_approvers_pb2_grpc.py
+-rw-r--r--  2.0 unx      741 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/options_pb2_grpc.py
+-rw-r--r--  2.0 unx     8961 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/workflow_assignments_history_pb2.py
+-rwxr-xr-x  2.0 unx    18827 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/constants.py
+-rw-r--r--  2.0 unx     6598 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/control_panel_pb2_grpc.py
+-rw-r--r--  2.0 unx    15297 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/peering_groups_pb2.py
+-rw-r--r--  2.0 unx     8138 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/accounts_history_pb2.py
+-rw-r--r--  2.0 unx   893989 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/drivers_pb2.py
+-rw-r--r--  2.0 unx      808 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/__init__.py
+-rw-r--r--  2.0 unx     8132 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/resources_history_pb2.py
+-rw-r--r--  2.0 unx     3704 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/approval_workflow_approvers_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     3350 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/role_resources_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     3223 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/resources_history_pb2_grpc.py
+-rw-r--r--  2.0 unx    17173 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/peering_group_resources_pb2.py
+-rw-r--r--  2.0 unx     8478 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/role_resources_history_pb2.py
+-rw-r--r--  2.0 unx     8983 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/access_request_events_history_pb2.py
+-rw-r--r--  2.0 unx     8901 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/account_resources_pb2.py
+-rw-r--r--  2.0 unx     7818 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/roles_history_pb2.py
+-rw-r--r--  2.0 unx    14958 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/options_pb2.py
+-rw-r--r--  2.0 unx     2196 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/errors.py
+-rw-r--r--  2.0 unx      741 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/drivers_pb2_grpc.py
+-rw-r--r--  2.0 unx      741 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/spec_pb2_grpc.py
+-rw-r--r--  2.0 unx     9790 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/remote_identities_pb2_grpc.py
+-rw-r--r--  2.0 unx     3470 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/account_permissions_pb2_grpc.py
+-rw-r--r--  2.0 unx     8255 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/peering_group_nodes_pb2_grpc.py
+-rw-r--r--  2.0 unx     8396 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/account_permissions_pb2.py
+-rw-r--r--  2.0 unx     8550 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/account_grants_history_pb2.py
+-rw-r--r--  2.0 unx    22207 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/resources_pb2.py
+-rw-r--r--  2.0 unx     7818 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/nodes_history_pb2.py
+-rw-r--r--  2.0 unx     3388 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/account_resources_pb2_grpc.py
+-rw-r--r--  2.0 unx     3434 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/account_resources_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8102 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/account_attachments_pb2_grpc.py
+-rw-r--r--  2.0 unx      741 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/tags_pb2_grpc.py
+-rw-r--r--  2.0 unx    29937 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/nodes_pb2.py
+-rw-r--r--  2.0 unx     3424 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/remote_identities_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8546 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/peering_group_resources_pb2_grpc.py
+-rw-r--r--  2.0 unx    29031 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/accounts_pb2.py
+-rw-r--r--  2.0 unx     3561 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/workflow_assignments_history_pb2_grpc.py
+-rw-r--r--  2.0 unx    17204 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/workflow_approvers_pb2.py
+-rw-r--r--  2.0 unx     8773 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/account_resources_history_pb2.py
+-rw-r--r--  2.0 unx     7476 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/role_resources_pb2.py
+-rw-r--r--  2.0 unx     8165 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/workflow_approvers_pb2_grpc.py
+-rw-r--r--  2.0 unx    11611 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/control_panel_pb2.py
+-rw-r--r--  2.0 unx    18385 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/roles_pb2.py
+-rw-r--r--  2.0 unx     8071 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/workflow_roles_pb2_grpc.py
+-rw-r--r--  2.0 unx    15576 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/access_requests_pb2.py
+-rw-r--r--  2.0 unx     3361 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/replays_pb2_grpc.py
+-rw-r--r--  2.0 unx    82330 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/secret_store_types_pb2.py
+-rw-r--r--  2.0 unx     7340 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/workflow_assignments_pb2.py
+-rw-r--r--  2.0 unx    16380 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/peering_group_nodes_pb2.py
+-rw-r--r--  2.0 unx     3557 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/access_request_events_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     9960 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/approval_workflows_pb2_grpc.py
+-rw-r--r--  2.0 unx    20122 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/workflows_pb2.py
+-rw-r--r--  2.0 unx     9376 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/secret_stores_pb2_grpc.py
+-rw-r--r--  2.0 unx     6849 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/secret_store_healths_pb2_grpc.py
+-rw-r--r--  2.0 unx    17037 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/account_attachments_pb2.py
+-rw-r--r--  2.0 unx     3493 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/account_attachments_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     3198 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/accounts_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8506 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/workflow_roles_history_pb2.py
+-rw-r--r--  2.0 unx     9758 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/accounts_pb2_grpc.py
+-rw-r--r--  2.0 unx     3111 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/roles_history_pb2_grpc.py
+-rw-r--r--  2.0 unx   436781 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/plumbing.py
+-rw-r--r--  2.0 unx     3111 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/nodes_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8167 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/peering_group_peers_pb2_grpc.py
+-rw-r--r--  2.0 unx     4600 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/tags_pb2.py
+-rw-r--r--  2.0 unx     8646 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/access_requests_history_pb2.py
+-rw-r--r--  2.0 unx     9416 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/approval_workflow_approvers_history_pb2.py
+-rw-r--r--  2.0 unx     9027 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/remote_identity_groups_history_pb2.py
+-rw-r--r--  2.0 unx     8140 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/workflows_history_pb2.py
+-rw-r--r--  2.0 unx    19200 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/queries_pb2.py
+-rw-r--r--  2.0 unx     8320 b- defN 24-Apr-25 15:31 strongdm-8.1.0/strongdm/replays_pb2.py
+130 files, 3471987 bytes uncompressed, 356519 bytes compressed:  89.8%
```

## zipnote {}

```diff
@@ -1,391 +1,391 @@
-Filename: strongdm-8.0.0/
+Filename: strongdm-8.1.0/
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/
+Filename: strongdm-8.1.0/strongdm.egg-info/
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm.egg-info/
+Filename: strongdm-8.1.0/strongdm/
 Comment: 
 
-Filename: strongdm-8.0.0/README.md
+Filename: strongdm-8.1.0/PKG-INFO
 Comment: 
 
-Filename: strongdm-8.0.0/LICENSE
+Filename: strongdm-8.1.0/setup.py
 Comment: 
 
-Filename: strongdm-8.0.0/setup.py
+Filename: strongdm-8.1.0/setup.cfg
 Comment: 
 
-Filename: strongdm-8.0.0/PKG-INFO
+Filename: strongdm-8.1.0/README.md
 Comment: 
 
-Filename: strongdm-8.0.0/setup.cfg
+Filename: strongdm-8.1.0/LICENSE
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/approval_workflows_history_pb2.py
+Filename: strongdm-8.1.0/strongdm.egg-info/top_level.txt
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/replays_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm.egg-info/PKG-INFO
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/activities_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm.egg-info/SOURCES.txt
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/accounts_pb2.py
+Filename: strongdm-8.1.0/strongdm.egg-info/dependency_links.txt
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/role_resources_pb2.py
+Filename: strongdm-8.1.0/strongdm.egg-info/requires.txt
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/workflow_approvers_pb2.py
+Filename: strongdm-8.1.0/strongdm/spec_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/secret_store_healths_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/account_grants_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/__init__.py
+Filename: strongdm-8.1.0/strongdm/workflows_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/remote_identities_history_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/roles_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/workflow_approvers_history_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/models.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/account_resources_pb2.py
+Filename: strongdm-8.1.0/strongdm/secret_store_types_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/roles_pb2.py
+Filename: strongdm-8.1.0/strongdm/remote_identities_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/approval_workflow_approvers_history_pb2.py
+Filename: strongdm-8.1.0/strongdm/peering_groups_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/options_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/approval_workflow_steps_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/plumbing.py
+Filename: strongdm-8.1.0/strongdm/activities_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/resources_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/access_requests_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/workflows_history_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/secret_stores_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/nodes_history_pb2.py
+Filename: strongdm-8.1.0/strongdm/account_grants_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/spec_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/remote_identity_groups_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/access_request_events_history_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/peering_group_peers_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/queries_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/secret_stores_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/peering_groups_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/remote_identity_groups_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/nodes_history_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/workflows_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/account_grants_history_pb2.py
+Filename: strongdm-8.1.0/strongdm/workflow_roles_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/organization_history_pb2.py
+Filename: strongdm-8.1.0/strongdm/role_resources_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/secret_stores_history_pb2.py
+Filename: strongdm-8.1.0/strongdm/approval_workflows_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/resources_history_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/workflow_approvers_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/remote_identity_groups_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/remote_identity_groups_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/secret_stores_pb2.py
+Filename: strongdm-8.1.0/strongdm/approval_workflow_approvers_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/workflow_assignments_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/approval_workflow_steps_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/account_resources_history_pb2.py
+Filename: strongdm-8.1.0/strongdm/account_grants_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/client.py
+Filename: strongdm-8.1.0/strongdm/organization_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/peering_group_peers_pb2.py
+Filename: strongdm-8.1.0/strongdm/resources_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/approval_workflow_approvers_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/workflow_roles_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/remote_identities_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/activities_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/drivers_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/nodes_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/account_permissions_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/approval_workflow_steps_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/access_request_events_history_pb2.py
+Filename: strongdm-8.1.0/strongdm/queries_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/nodes_pb2.py
+Filename: strongdm-8.1.0/strongdm/approval_workflow_steps_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/organization_history_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/access_requests_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/account_attachments_history_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/secret_stores_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/drivers_pb2.py
+Filename: strongdm-8.1.0/strongdm/approval_workflows_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/account_grants_pb2.py
+Filename: strongdm-8.1.0/strongdm/approval_workflows_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/account_resources_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/secret_store_healths_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/access_requests_pb2.py
+Filename: strongdm-8.1.0/strongdm/workflow_assignments_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/nodes_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/client.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/secret_stores_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/remote_identities_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/role_resources_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/workflow_approvers_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/peering_group_resources_pb2.py
+Filename: strongdm-8.1.0/strongdm/svc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/account_attachments_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/account_attachments_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/role_resources_history_pb2.py
+Filename: strongdm-8.1.0/strongdm/organization_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/peering_group_peers_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/approval_workflow_approvers_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/workflows_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/options_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/access_requests_history_pb2.py
+Filename: strongdm-8.1.0/strongdm/workflow_assignments_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/workflow_assignments_history_pb2.py
+Filename: strongdm-8.1.0/strongdm/constants.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/remote_identity_groups_history_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/control_panel_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/control_panel_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/peering_groups_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/accounts_history_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/accounts_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/approval_workflows_history_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/drivers_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/workflow_roles_history_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/__init__.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/access_requests_history_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/resources_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/workflow_roles_pb2.py
+Filename: strongdm-8.1.0/strongdm/approval_workflow_approvers_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/tags_pb2.py
+Filename: strongdm-8.1.0/strongdm/role_resources_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/remote_identities_history_pb2.py
+Filename: strongdm-8.1.0/strongdm/resources_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/replays_pb2.py
+Filename: strongdm-8.1.0/strongdm/peering_group_resources_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/activities_pb2.py
+Filename: strongdm-8.1.0/strongdm/role_resources_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/workflow_assignments_pb2.py
+Filename: strongdm-8.1.0/strongdm/access_request_events_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/account_grants_history_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/account_resources_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/svc.py
+Filename: strongdm-8.1.0/strongdm/roles_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/approval_workflow_steps_history_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/options_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/constants.py
+Filename: strongdm-8.1.0/strongdm/errors.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/peering_group_nodes_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/drivers_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/remote_identity_groups_history_pb2.py
+Filename: strongdm-8.1.0/strongdm/spec_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/tags_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/remote_identities_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/secret_stores_history_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/account_permissions_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/peering_groups_pb2.py
+Filename: strongdm-8.1.0/strongdm/peering_group_nodes_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/secret_store_types_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/account_permissions_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/account_grants_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/account_grants_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/workflows_pb2.py
+Filename: strongdm-8.1.0/strongdm/resources_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/approval_workflow_steps_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/nodes_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/approval_workflows_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/account_resources_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/access_requests_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/account_resources_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/account_attachments_pb2.py
+Filename: strongdm-8.1.0/strongdm/account_attachments_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/role_resources_history_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/tags_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/roles_history_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/nodes_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/queries_pb2.py
+Filename: strongdm-8.1.0/strongdm/remote_identities_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/options_pb2.py
+Filename: strongdm-8.1.0/strongdm/peering_group_resources_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/approval_workflow_steps_pb2.py
+Filename: strongdm-8.1.0/strongdm/accounts_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/approval_workflow_approvers_pb2.py
+Filename: strongdm-8.1.0/strongdm/workflow_assignments_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/accounts_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/workflow_approvers_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/peering_group_resources_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/account_resources_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/account_attachments_history_pb2.py
+Filename: strongdm-8.1.0/strongdm/role_resources_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/secret_store_types_pb2.py
+Filename: strongdm-8.1.0/strongdm/workflow_approvers_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/account_permissions_pb2.py
+Filename: strongdm-8.1.0/strongdm/control_panel_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/account_resources_history_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/roles_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/spec_pb2.py
+Filename: strongdm-8.1.0/strongdm/workflow_roles_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/errors.py
+Filename: strongdm-8.1.0/strongdm/access_requests_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/approval_workflow_approvers_history_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/replays_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/workflow_roles_history_pb2.py
+Filename: strongdm-8.1.0/strongdm/secret_store_types_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/resources_pb2.py
+Filename: strongdm-8.1.0/strongdm/workflow_assignments_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/control_panel_pb2.py
+Filename: strongdm-8.1.0/strongdm/peering_group_nodes_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/models.py
+Filename: strongdm-8.1.0/strongdm/access_request_events_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/secret_store_healths_pb2.py
+Filename: strongdm-8.1.0/strongdm/approval_workflows_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/accounts_history_pb2.py
+Filename: strongdm-8.1.0/strongdm/workflows_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/roles_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/secret_stores_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/workflows_history_pb2.py
+Filename: strongdm-8.1.0/strongdm/secret_store_healths_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/approval_workflows_pb2.py
+Filename: strongdm-8.1.0/strongdm/account_attachments_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/peering_group_nodes_pb2.py
+Filename: strongdm-8.1.0/strongdm/account_attachments_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/workflow_assignments_history_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/accounts_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/approval_workflow_steps_history_pb2.py
+Filename: strongdm-8.1.0/strongdm/workflow_roles_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/workflow_approvers_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/accounts_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/remote_identities_pb2.py
+Filename: strongdm-8.1.0/strongdm/roles_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/workflow_approvers_history_pb2.py
+Filename: strongdm-8.1.0/strongdm/plumbing.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/resources_history_pb2.py
+Filename: strongdm-8.1.0/strongdm/nodes_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/roles_history_pb2.py
+Filename: strongdm-8.1.0/strongdm/peering_group_peers_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/remote_identity_groups_pb2.py
+Filename: strongdm-8.1.0/strongdm/tags_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm/workflow_roles_pb2_grpc.py
+Filename: strongdm-8.1.0/strongdm/access_requests_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm.egg-info/requires.txt
+Filename: strongdm-8.1.0/strongdm/approval_workflow_approvers_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm.egg-info/top_level.txt
+Filename: strongdm-8.1.0/strongdm/remote_identity_groups_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm.egg-info/PKG-INFO
+Filename: strongdm-8.1.0/strongdm/workflows_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm.egg-info/SOURCES.txt
+Filename: strongdm-8.1.0/strongdm/queries_pb2.py
 Comment: 
 
-Filename: strongdm-8.0.0/strongdm.egg-info/dependency_links.txt
+Filename: strongdm-8.1.0/strongdm/replays_pb2.py
 Comment: 
 
 Zip file comment:
```

## Comparing `strongdm-8.0.0/README.md` & `strongdm-8.1.0/README.md`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/LICENSE` & `strongdm-8.1.0/LICENSE`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/setup.py` & `strongdm-8.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 from setuptools import setup
 setup(
     name='strongdm',
     packages=['strongdm'],
-    version='8.0.0',
+    version='8.1.0',
     license='apache-2.0',
     description='strongDM SDK for the Python programming language.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='strongDM Team',
     author_email='sdk-feedback@strongdm.com',
     url='https://github.com/strongdm/strongdm-sdk-python',
     download_url=
-    'https://github.com/strongdm/strongdm-sdk-python/archive/v8.0.0.tar.gz',
+    'https://github.com/strongdm/strongdm-sdk-python/archive/v8.1.0.tar.gz',
     keywords=[
         'strongDM', 'sdm', 'api', 'automation', 'security', 'audit',
         'database', 'server', 'ssh', 'rdp'
     ],
     install_requires=[
         'grpcio>=1.42.0',
         'googleapis-common-protos>1.56.2,<2',
```

## Comparing `strongdm-8.0.0/PKG-INFO` & `strongdm-8.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: strongdm
-Version: 8.0.0
+Version: 8.1.0
 Summary: strongDM SDK for the Python programming language.
 Home-page: https://github.com/strongdm/strongdm-sdk-python
 Author: strongDM Team
 Author-email: sdk-feedback@strongdm.com
 License: apache-2.0
-Download-URL: https://github.com/strongdm/strongdm-sdk-python/archive/v8.0.0.tar.gz
+Download-URL: https://github.com/strongdm/strongdm-sdk-python/archive/v8.1.0.tar.gz
 Keywords: strongDM,sdm,api,automation,security,audit,database,server,ssh,rdp
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `strongdm-8.0.0/strongdm/approval_workflows_history_pb2.py` & `strongdm-8.1.0/strongdm/approval_workflows_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/replays_pb2_grpc.py` & `strongdm-8.1.0/strongdm/replays_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/activities_pb2_grpc.py` & `strongdm-8.1.0/strongdm/activities_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/accounts_pb2.py` & `strongdm-8.1.0/strongdm/accounts_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from . import options_pb2 as options__pb2
 from . import spec_pb2 as spec__pb2
 from . import tags_pb2 as tags__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x61\x63\x63ounts.proto\x12\x02v1\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\roptions.proto\x1a\nspec.proto\x1a\ntags.proto\"i\n\x14\x41\x63\x63ountCreateRequest\x12\'\n\x04meta\x18\x01 \x01(\x0b\x32\x19.v1.CreateRequestMetadata\x12(\n\x07\x61\x63\x63ount\x18\x02 \x01(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\"\xf8\x02\n\x15\x41\x63\x63ountCreateResponse\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32\x1a.v1.CreateResponseMetadataB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12(\n\x07\x61\x63\x63ount\x18\x02 \x01(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1e\n\x05token\x18\x03 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xf0\xf3\xb3\x07\x01\x12W\n\nrate_limit\x18\x04 \x01(\x0b\x32\x15.v1.RateLimitMetadataB,\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\xf2\xf8\xb3\x07\x06\xb2\xf4\xb3\x07\x01*\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway\x12<\n\naccess_key\x18\x05 \x01(\tB(\xf2\xf8\xb3\x07#\xb0\xf3\xb3\x07\x01\xb2\xf4\xb3\x07\x01*\xb2\xf4\xb3\x07\x13!terraform-provider\x12<\n\nsecret_key\x18\x06 \x01(\tB(\xf2\xf8\xb3\x07#\xb0\xf3\xb3\x07\x01\xb2\xf4\xb3\x07\x01*\xb2\xf4\xb3\x07\x13!terraform-provider:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"Q\n\x11\x41\x63\x63ountGetRequest\x12$\n\x04meta\x18\x01 \x01(\x0b\x32\x16.v1.GetRequestMetadata\x12\x16\n\x02id\x18\x02 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\"\xd6\x01\n\x12\x41\x63\x63ountGetResponse\x12\x31\n\x04meta\x18\x01 \x01(\x0b\x32\x17.v1.GetResponseMetadataB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12(\n\x07\x61\x63\x63ount\x18\x02 \x01(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12W\n\nrate_limit\x18\x03 \x01(\x0b\x32\x15.v1.RateLimitMetadataB,\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\xf2\xf8\xb3\x07\x06\xb2\xf4\xb3\x07\x01*\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"u\n\x14\x41\x63\x63ountUpdateRequest\x12\'\n\x04meta\x18\x01 \x01(\x0b\x32\x19.v1.UpdateRequestMetadata\x12\n\n\x02id\x18\x02 \x01(\t\x12(\n\x07\x61\x63\x63ount\x18\x03 \x01(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\"\xdc\x01\n\x15\x41\x63\x63ountUpdateResponse\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32\x1a.v1.UpdateResponseMetadataB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12(\n\x07\x61\x63\x63ount\x18\x02 \x01(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12W\n\nrate_limit\x18\x03 \x01(\x0b\x32\x15.v1.RateLimitMetadataB,\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\xf2\xf8\xb3\x07\x06\xb2\xf4\xb3\x07\x01*\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"W\n\x14\x41\x63\x63ountDeleteRequest\x12\'\n\x04meta\x18\x01 \x01(\x0b\x32\x19.v1.DeleteRequestMetadata\x12\x16\n\x02id\x18\x02 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\"\xb2\x01\n\x15\x41\x63\x63ountDeleteResponse\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32\x1a.v1.DeleteResponseMetadataB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12W\n\nrate_limit\x18\x02 \x01(\x0b\x32\x15.v1.RateLimitMetadataB,\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\xf2\xf8\xb3\x07\x06\xb2\xf4\xb3\x07\x01*\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"W\n\x12\x41\x63\x63ountListRequest\x12%\n\x04meta\x18\x01 \x01(\x0b\x32\x17.v1.ListRequestMetadata\x12\x1a\n\x06\x66ilter\x18\x02 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\"\xc1\x01\n\x13\x41\x63\x63ountListResponse\x12&\n\x04meta\x18\x01 \x01(\x0b\x32\x18.v1.ListResponseMetadata\x12)\n\x08\x61\x63\x63ounts\x18\x02 \x03(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb8\xf3\xb3\x07\x01\x12W\n\nrate_limit\x18\x03 \x01(\x0b\x32\x15.v1.RateLimitMetadataB,\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\xf2\xf8\xb3\x07\x06\xb2\xf4\xb3\x07\x01*\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway\"\xb2\x02\n\x07\x41\x63\x63ount\x12$\n\x04user\x18\x01 \x01(\x0b\x32\x08.v1.UserB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12*\n\x07service\x18\x02 \x01(\x0b\x32\x0b.v1.ServiceB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x44\n\x05token\x18\x03 \x01(\x0b\x32\t.v1.TokenB(\xf2\xf8\xb3\x07#\xb0\xf3\xb3\x07\x01\xb2\xf4\xb3\x07\x01*\xb2\xf4\xb3\x07\x13!terraform-providerH\x00:a\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\xfa\xf8\xb3\x07R\xc2\xf3\xb3\x07M\xa2\xf3\xb3\x07 tf_examples/account_resource.txt\xaa\xf3\xb3\x07#tf_examples/account_data_source.txtB,\n\x07\x61\x63\x63ount\x12!\xaa\xf8\xb3\x07\x0e\xaa\xf8\xb3\x07\tsuspended\xaa\xf8\xb3\x07\t\xaa\xf8\xb3\x07\x04tags\"\xd2\x06\n\x04User\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1e\n\x05\x65mail\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12#\n\nfirst_name\x18\x03 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\"\n\tlast_name\x18\x04 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12*\n\tsuspended\x18\x05 \x01(\x08\x42\x17\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway\x12\"\n\x04tags\x18\x06 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x36\n\x10permission_level\x18\x07 \x01(\tB\x1c\xf2\xf8\xb3\x07\x17\x98\xf4\xb3\x07\x01\xb2\xf4\xb3\x07\r!json_gateway\x12#\n\nmanaged_by\x18\x08 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\x98\xf4\xb3\x07\x01\x12\x1f\n\x0b\x65xternal_id\x18\t \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\xdb\x01\n\x0bsuspendedRO\x18\n \x01(\x08\x42\xc5\x01\xf2\xf8\xb3\x07\xbf\x01\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\xaf\x01\xc2\xf4\xb3\x07\x0f\n\x02go\x12\tSuspended\xc2\xf4\xb3\x07\x10\n\x03\x63li\x12\tsuspended\xc2\xf4\xb3\x07\x11\n\x04ruby\x12\tsuspended\xc2\xf4\xb3\x07\x13\n\x06python\x12\tsuspended\xc2\xf4\xb3\x07\x11\n\x04java\x12\tSuspended\xc2\xf4\xb3\x07\x1f\n\x12terraform-provider\x12\tsuspended\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tsuspended\x98\xf4\xb3\x07\x01\x12\x90\x02\n\x12permission_levelRW\x18\x0b \x01(\tB\xf3\x01\xf2\xf8\xb3\x07\xed\x01\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\xdd\x01\xc2\xf4\xb3\x07\x15\n\x02go\x12\x0fPermissionLevel\xc2\xf4\xb3\x07\x17\n\x03\x63li\x12\x10permission-level\xc2\xf4\xb3\x07\x18\n\x04ruby\x12\x10permission_level\xc2\xf4\xb3\x07\x1a\n\x06python\x12\x10permission_level\xc2\xf4\xb3\x07\x17\n\x04java\x12\x0fPermissionLevel\xc2\xf4\xb3\x07&\n\x12terraform-provider\x12\x10permission_level\xc2\xf4\xb3\x07\x1f\n\x0cjson_gateway\x12\x0fpermissionLevel\xd0\xf4\xb3\x07\x01:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"\x8f\x01\n\x07Service\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x1d\n\tsuspended\x18\x03 \x01(\x08\x42\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"\x9a\x03\n\x05Token\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x1d\n\tsuspended\x18\x03 \x01(\x08\x42\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x37\n\x07rekeyed\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x38\n\x08\x64\x65\x61\x64line\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12 \n\x0c\x61\x63\x63ount_type\x18\x07 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1f\n\x0bpermissions\x18\x08 \x03(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x37\n\x08\x64uration\x18\t \x01(\x0b\x32\x19.google.protobuf.DurationB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:(\xfa\xf8\xb3\x07#\xa8\xf3\xb3\x07\x01\xd2\xf3\xb3\x07\x01*\xd2\xf3\xb3\x07\x13!terraform-provider2\xab\x04\n\x08\x41\x63\x63ounts\x12\x63\n\x06\x43reate\x12\x18.v1.AccountCreateRequest\x1a\x19.v1.AccountCreateResponse\"$\x82\xf9\xb3\x07\t\xa2\xf3\xb3\x07\x04post\x82\xf9\xb3\x07\x11\xaa\xf3\xb3\x07\x0c/v1/accounts\x12^\n\x03Get\x12\x15.v1.AccountGetRequest\x1a\x16.v1.AccountGetResponse\"(\x82\xf9\xb3\x07\x08\xa2\xf3\xb3\x07\x03get\x82\xf9\xb3\x07\x16\xaa\xf3\xb3\x07\x11/v1/accounts/{id}\x12g\n\x06Update\x12\x18.v1.AccountUpdateRequest\x1a\x19.v1.AccountUpdateResponse\"(\x82\xf9\xb3\x07\x08\xa2\xf3\xb3\x07\x03put\x82\xf9\xb3\x07\x16\xaa\xf3\xb3\x07\x11/v1/accounts/{id}\x12j\n\x06\x44\x65lete\x12\x18.v1.AccountDeleteRequest\x1a\x19.v1.AccountDeleteResponse\"+\x82\xf9\xb3\x07\x0b\xa2\xf3\xb3\x07\x06\x64\x65lete\x82\xf9\xb3\x07\x16\xaa\xf3\xb3\x07\x11/v1/accounts/{id}\x12\\\n\x04List\x12\x16.v1.AccountListRequest\x1a\x17.v1.AccountListResponse\"#\x82\xf9\xb3\x07\x08\xa2\xf3\xb3\x07\x03get\x82\xf9\xb3\x07\x11\xaa\xf3\xb3\x07\x0c/v1/accounts\x1a\'\xca\xf9\xb3\x07\x0c\xc2\xf9\xb3\x07\x07\x41\x63\x63ount\xca\xf9\xb3\x07\x07\xd2\xf9\xb3\x07\x02\x61-\xca\xf9\xb3\x07\x05\xe0\xf9\xb3\x07\x01\x42\x64\n\x19\x63om.strongdm.api.plumbingB\x10\x41\x63\x63ountsPlumbingZ5github.com/strongdm/strongdm-sdk-go/v3/internal/v1;v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x61\x63\x63ounts.proto\x12\x02v1\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\roptions.proto\x1a\nspec.proto\x1a\ntags.proto\"i\n\x14\x41\x63\x63ountCreateRequest\x12\'\n\x04meta\x18\x01 \x01(\x0b\x32\x19.v1.CreateRequestMetadata\x12(\n\x07\x61\x63\x63ount\x18\x02 \x01(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\"\xf8\x02\n\x15\x41\x63\x63ountCreateResponse\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32\x1a.v1.CreateResponseMetadataB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12(\n\x07\x61\x63\x63ount\x18\x02 \x01(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1e\n\x05token\x18\x03 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xf0\xf3\xb3\x07\x01\x12W\n\nrate_limit\x18\x04 \x01(\x0b\x32\x15.v1.RateLimitMetadataB,\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\xf2\xf8\xb3\x07\x06\xb2\xf4\xb3\x07\x01*\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway\x12<\n\naccess_key\x18\x05 \x01(\tB(\xf2\xf8\xb3\x07#\xb0\xf3\xb3\x07\x01\xb2\xf4\xb3\x07\x01*\xb2\xf4\xb3\x07\x13!terraform-provider\x12<\n\nsecret_key\x18\x06 \x01(\tB(\xf2\xf8\xb3\x07#\xb0\xf3\xb3\x07\x01\xb2\xf4\xb3\x07\x01*\xb2\xf4\xb3\x07\x13!terraform-provider:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"Q\n\x11\x41\x63\x63ountGetRequest\x12$\n\x04meta\x18\x01 \x01(\x0b\x32\x16.v1.GetRequestMetadata\x12\x16\n\x02id\x18\x02 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\"\xd6\x01\n\x12\x41\x63\x63ountGetResponse\x12\x31\n\x04meta\x18\x01 \x01(\x0b\x32\x17.v1.GetResponseMetadataB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12(\n\x07\x61\x63\x63ount\x18\x02 \x01(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12W\n\nrate_limit\x18\x03 \x01(\x0b\x32\x15.v1.RateLimitMetadataB,\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\xf2\xf8\xb3\x07\x06\xb2\xf4\xb3\x07\x01*\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"u\n\x14\x41\x63\x63ountUpdateRequest\x12\'\n\x04meta\x18\x01 \x01(\x0b\x32\x19.v1.UpdateRequestMetadata\x12\n\n\x02id\x18\x02 \x01(\t\x12(\n\x07\x61\x63\x63ount\x18\x03 \x01(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\"\xdc\x01\n\x15\x41\x63\x63ountUpdateResponse\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32\x1a.v1.UpdateResponseMetadataB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12(\n\x07\x61\x63\x63ount\x18\x02 \x01(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12W\n\nrate_limit\x18\x03 \x01(\x0b\x32\x15.v1.RateLimitMetadataB,\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\xf2\xf8\xb3\x07\x06\xb2\xf4\xb3\x07\x01*\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"W\n\x14\x41\x63\x63ountDeleteRequest\x12\'\n\x04meta\x18\x01 \x01(\x0b\x32\x19.v1.DeleteRequestMetadata\x12\x16\n\x02id\x18\x02 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\"\xb2\x01\n\x15\x41\x63\x63ountDeleteResponse\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32\x1a.v1.DeleteResponseMetadataB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12W\n\nrate_limit\x18\x02 \x01(\x0b\x32\x15.v1.RateLimitMetadataB,\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\xf2\xf8\xb3\x07\x06\xb2\xf4\xb3\x07\x01*\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"W\n\x12\x41\x63\x63ountListRequest\x12%\n\x04meta\x18\x01 \x01(\x0b\x32\x17.v1.ListRequestMetadata\x12\x1a\n\x06\x66ilter\x18\x02 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\"\xc1\x01\n\x13\x41\x63\x63ountListResponse\x12&\n\x04meta\x18\x01 \x01(\x0b\x32\x18.v1.ListResponseMetadata\x12)\n\x08\x61\x63\x63ounts\x18\x02 \x03(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb8\xf3\xb3\x07\x01\x12W\n\nrate_limit\x18\x03 \x01(\x0b\x32\x15.v1.RateLimitMetadataB,\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\xf2\xf8\xb3\x07\x06\xb2\xf4\xb3\x07\x01*\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway\"\x94\x02\n\x07\x41\x63\x63ount\x12$\n\x04user\x18\x01 \x01(\x0b\x32\x08.v1.UserB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12*\n\x07service\x18\x02 \x01(\x0b\x32\x0b.v1.ServiceB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12&\n\x05token\x18\x03 \x01(\x0b\x32\t.v1.TokenB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00:a\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\xfa\xf8\xb3\x07R\xc2\xf3\xb3\x07M\xa2\xf3\xb3\x07 tf_examples/account_resource.txt\xaa\xf3\xb3\x07#tf_examples/account_data_source.txtB,\n\x07\x61\x63\x63ount\x12!\xaa\xf8\xb3\x07\x0e\xaa\xf8\xb3\x07\tsuspended\xaa\xf8\xb3\x07\t\xaa\xf8\xb3\x07\x04tags\"\xd2\x06\n\x04User\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1e\n\x05\x65mail\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12#\n\nfirst_name\x18\x03 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\"\n\tlast_name\x18\x04 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12*\n\tsuspended\x18\x05 \x01(\x08\x42\x17\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway\x12\"\n\x04tags\x18\x06 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x36\n\x10permission_level\x18\x07 \x01(\tB\x1c\xf2\xf8\xb3\x07\x17\x98\xf4\xb3\x07\x01\xb2\xf4\xb3\x07\r!json_gateway\x12#\n\nmanaged_by\x18\x08 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\x98\xf4\xb3\x07\x01\x12\x1f\n\x0b\x65xternal_id\x18\t \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\xdb\x01\n\x0bsuspendedRO\x18\n \x01(\x08\x42\xc5\x01\xf2\xf8\xb3\x07\xbf\x01\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\xaf\x01\xc2\xf4\xb3\x07\x0f\n\x02go\x12\tSuspended\xc2\xf4\xb3\x07\x10\n\x03\x63li\x12\tsuspended\xc2\xf4\xb3\x07\x11\n\x04ruby\x12\tsuspended\xc2\xf4\xb3\x07\x13\n\x06python\x12\tsuspended\xc2\xf4\xb3\x07\x11\n\x04java\x12\tSuspended\xc2\xf4\xb3\x07\x1f\n\x12terraform-provider\x12\tsuspended\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tsuspended\x98\xf4\xb3\x07\x01\x12\x90\x02\n\x12permission_levelRW\x18\x0b \x01(\tB\xf3\x01\xf2\xf8\xb3\x07\xed\x01\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\xdd\x01\xc2\xf4\xb3\x07\x15\n\x02go\x12\x0fPermissionLevel\xc2\xf4\xb3\x07\x17\n\x03\x63li\x12\x10permission-level\xc2\xf4\xb3\x07\x18\n\x04ruby\x12\x10permission_level\xc2\xf4\xb3\x07\x1a\n\x06python\x12\x10permission_level\xc2\xf4\xb3\x07\x17\n\x04java\x12\x0fPermissionLevel\xc2\xf4\xb3\x07&\n\x12terraform-provider\x12\x10permission_level\xc2\xf4\xb3\x07\x1f\n\x0cjson_gateway\x12\x0fpermissionLevel\xd0\xf4\xb3\x07\x01:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"\x8f\x01\n\x07Service\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x1d\n\tsuspended\x18\x03 \x01(\x08\x42\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"\x81\x03\n\x05Token\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x1d\n\tsuspended\x18\x03 \x01(\x08\x42\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x37\n\x07rekeyed\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x38\n\x08\x64\x65\x61\x64line\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12 \n\x0c\x61\x63\x63ount_type\x18\x07 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1f\n\x0bpermissions\x18\x08 \x03(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x37\n\x08\x64uration\x18\t \x01(\x0b\x32\x19.google.protobuf.DurationB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\x0f\xfa\xf8\xb3\x07\n\xa8\xf3\xb3\x07\x01\xd8\xf3\xb3\x07\x01\x32\xab\x04\n\x08\x41\x63\x63ounts\x12\x63\n\x06\x43reate\x12\x18.v1.AccountCreateRequest\x1a\x19.v1.AccountCreateResponse\"$\x82\xf9\xb3\x07\t\xa2\xf3\xb3\x07\x04post\x82\xf9\xb3\x07\x11\xaa\xf3\xb3\x07\x0c/v1/accounts\x12^\n\x03Get\x12\x15.v1.AccountGetRequest\x1a\x16.v1.AccountGetResponse\"(\x82\xf9\xb3\x07\x08\xa2\xf3\xb3\x07\x03get\x82\xf9\xb3\x07\x16\xaa\xf3\xb3\x07\x11/v1/accounts/{id}\x12g\n\x06Update\x12\x18.v1.AccountUpdateRequest\x1a\x19.v1.AccountUpdateResponse\"(\x82\xf9\xb3\x07\x08\xa2\xf3\xb3\x07\x03put\x82\xf9\xb3\x07\x16\xaa\xf3\xb3\x07\x11/v1/accounts/{id}\x12j\n\x06\x44\x65lete\x12\x18.v1.AccountDeleteRequest\x1a\x19.v1.AccountDeleteResponse\"+\x82\xf9\xb3\x07\x0b\xa2\xf3\xb3\x07\x06\x64\x65lete\x82\xf9\xb3\x07\x16\xaa\xf3\xb3\x07\x11/v1/accounts/{id}\x12\\\n\x04List\x12\x16.v1.AccountListRequest\x1a\x17.v1.AccountListResponse\"#\x82\xf9\xb3\x07\x08\xa2\xf3\xb3\x07\x03get\x82\xf9\xb3\x07\x11\xaa\xf3\xb3\x07\x0c/v1/accounts\x1a\'\xca\xf9\xb3\x07\x0c\xc2\xf9\xb3\x07\x07\x41\x63\x63ount\xca\xf9\xb3\x07\x07\xd2\xf9\xb3\x07\x02\x61-\xca\xf9\xb3\x07\x05\xe0\xf9\xb3\x07\x01\x42\x64\n\x19\x63om.strongdm.api.plumbingB\x10\x41\x63\x63ountsPlumbingZ5github.com/strongdm/strongdm-sdk-go/v3/internal/v1;v1b\x06proto3')
 
 
 
 _ACCOUNTCREATEREQUEST = DESCRIPTOR.message_types_by_name['AccountCreateRequest']
 _ACCOUNTCREATERESPONSE = DESCRIPTOR.message_types_by_name['AccountCreateResponse']
 _ACCOUNTGETREQUEST = DESCRIPTOR.message_types_by_name['AccountGetRequest']
 _ACCOUNTGETRESPONSE = DESCRIPTOR.message_types_by_name['AccountGetResponse']
@@ -207,15 +207,15 @@
   _ACCOUNT.oneofs_by_name['account']._options = None
   _ACCOUNT.oneofs_by_name['account']._serialized_options = b'\252\370\263\007\016\252\370\263\007\tsuspended\252\370\263\007\t\252\370\263\007\004tags'
   _ACCOUNT.fields_by_name['user']._options = None
   _ACCOUNT.fields_by_name['user']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _ACCOUNT.fields_by_name['service']._options = None
   _ACCOUNT.fields_by_name['service']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _ACCOUNT.fields_by_name['token']._options = None
-  _ACCOUNT.fields_by_name['token']._serialized_options = b'\362\370\263\007#\260\363\263\007\001\262\364\263\007\001*\262\364\263\007\023!terraform-provider'
+  _ACCOUNT.fields_by_name['token']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _ACCOUNT._options = None
   _ACCOUNT._serialized_options = b'\372\370\263\007\005\250\363\263\007\001\372\370\263\007R\302\363\263\007M\242\363\263\007 tf_examples/account_resource.txt\252\363\263\007#tf_examples/account_data_source.txt'
   _USER.fields_by_name['id']._options = None
   _USER.fields_by_name['id']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _USER.fields_by_name['email']._options = None
   _USER.fields_by_name['email']._serialized_options = b'\362\370\263\007\n\260\363\263\007\001\300\363\263\007\001'
   _USER.fields_by_name['first_name']._options = None
@@ -263,15 +263,15 @@
   _TOKEN.fields_by_name['account_type']._options = None
   _TOKEN.fields_by_name['account_type']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _TOKEN.fields_by_name['permissions']._options = None
   _TOKEN.fields_by_name['permissions']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _TOKEN.fields_by_name['duration']._options = None
   _TOKEN.fields_by_name['duration']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _TOKEN._options = None
-  _TOKEN._serialized_options = b'\372\370\263\007#\250\363\263\007\001\322\363\263\007\001*\322\363\263\007\023!terraform-provider'
+  _TOKEN._serialized_options = b'\372\370\263\007\n\250\363\263\007\001\330\363\263\007\001'
   _ACCOUNTS._options = None
   _ACCOUNTS._serialized_options = b'\312\371\263\007\014\302\371\263\007\007Account\312\371\263\007\007\322\371\263\007\002a-\312\371\263\007\005\340\371\263\007\001'
   _ACCOUNTS.methods_by_name['Create']._options = None
   _ACCOUNTS.methods_by_name['Create']._serialized_options = b'\202\371\263\007\t\242\363\263\007\004post\202\371\263\007\021\252\363\263\007\014/v1/accounts'
   _ACCOUNTS.methods_by_name['Get']._options = None
   _ACCOUNTS.methods_by_name['Get']._serialized_options = b'\202\371\263\007\010\242\363\263\007\003get\202\371\263\007\026\252\363\263\007\021/v1/accounts/{id}'
   _ACCOUNTS.methods_by_name['Update']._options = None
@@ -297,17 +297,17 @@
   _ACCOUNTDELETERESPONSE._serialized_start=1344
   _ACCOUNTDELETERESPONSE._serialized_end=1522
   _ACCOUNTLISTREQUEST._serialized_start=1524
   _ACCOUNTLISTREQUEST._serialized_end=1611
   _ACCOUNTLISTRESPONSE._serialized_start=1614
   _ACCOUNTLISTRESPONSE._serialized_end=1807
   _ACCOUNT._serialized_start=1810
-  _ACCOUNT._serialized_end=2116
-  _USER._serialized_start=2119
-  _USER._serialized_end=2969
-  _SERVICE._serialized_start=2972
-  _SERVICE._serialized_end=3115
-  _TOKEN._serialized_start=3118
-  _TOKEN._serialized_end=3528
-  _ACCOUNTS._serialized_start=3531
-  _ACCOUNTS._serialized_end=4086
+  _ACCOUNT._serialized_end=2086
+  _USER._serialized_start=2089
+  _USER._serialized_end=2939
+  _SERVICE._serialized_start=2942
+  _SERVICE._serialized_end=3085
+  _TOKEN._serialized_start=3088
+  _TOKEN._serialized_end=3473
+  _ACCOUNTS._serialized_start=3476
+  _ACCOUNTS._serialized_end=4031
 # @@protoc_insertion_point(module_scope)
```

## Comparing `strongdm-8.0.0/strongdm/role_resources_pb2.py` & `strongdm-8.1.0/strongdm/role_resources_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/workflow_approvers_pb2.py` & `strongdm-8.1.0/strongdm/workflow_approvers_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/secret_store_healths_pb2_grpc.py` & `strongdm-8.1.0/strongdm/secret_store_healths_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/__init__.py` & `strongdm-8.1.0/strongdm/__init__.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/remote_identities_history_pb2_grpc.py` & `strongdm-8.1.0/strongdm/remote_identities_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/workflow_approvers_history_pb2_grpc.py` & `strongdm-8.1.0/strongdm/workflow_approvers_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/account_resources_pb2.py` & `strongdm-8.1.0/strongdm/account_resources_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/roles_pb2.py` & `strongdm-8.1.0/strongdm/roles_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/approval_workflow_approvers_history_pb2.py` & `strongdm-8.1.0/strongdm/approval_workflow_approvers_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/options_pb2_grpc.py` & `strongdm-8.1.0/strongdm/secret_store_types_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/plumbing.py` & `strongdm-8.1.0/strongdm/plumbing.py`

 * *Files 0% similar despite different names*

```diff
@@ -5046,14 +5046,76 @@
 
 def convert_repeated_http_no_auth_to_porcelain(plumbings):
     return [
         convert_http_no_auth_to_porcelain(plumbing) for plumbing in plumbings
     ]
 
 
+def convert_keyfactor_x_509_store_to_porcelain(plumbing):
+    if plumbing is None:
+        return None
+    porcelain = models.KeyfactorX509Store()
+    porcelain.ca_file_path = (plumbing.ca_file_path)
+    porcelain.certificate_file_path = (plumbing.certificate_file_path)
+    porcelain.default_certificate_authority_name = (
+        plumbing.default_certificate_authority_name)
+    porcelain.default_certificate_profile_name = (
+        plumbing.default_certificate_profile_name)
+    porcelain.default_end_entity_profile_name = (
+        plumbing.default_end_entity_profile_name)
+    porcelain.enrollment_code_env_var = (plumbing.enrollment_code_env_var)
+    porcelain.enrollment_username_env_var = (
+        plumbing.enrollment_username_env_var)
+    porcelain.id = (plumbing.id)
+    porcelain.key_file_path = (plumbing.key_file_path)
+    porcelain.key_password_env_var = (plumbing.key_password_env_var)
+    porcelain.name = (plumbing.name)
+    porcelain.server_address = (plumbing.server_address)
+    porcelain.tags = convert_tags_to_porcelain(plumbing.tags)
+    return porcelain
+
+
+def convert_keyfactor_x_509_store_to_plumbing(porcelain):
+    plumbing = KeyfactorX509Store()
+    if porcelain is None:
+        return plumbing
+    plumbing.ca_file_path = (porcelain.ca_file_path)
+    plumbing.certificate_file_path = (porcelain.certificate_file_path)
+    plumbing.default_certificate_authority_name = (
+        porcelain.default_certificate_authority_name)
+    plumbing.default_certificate_profile_name = (
+        porcelain.default_certificate_profile_name)
+    plumbing.default_end_entity_profile_name = (
+        porcelain.default_end_entity_profile_name)
+    plumbing.enrollment_code_env_var = (porcelain.enrollment_code_env_var)
+    plumbing.enrollment_username_env_var = (
+        porcelain.enrollment_username_env_var)
+    plumbing.id = (porcelain.id)
+    plumbing.key_file_path = (porcelain.key_file_path)
+    plumbing.key_password_env_var = (porcelain.key_password_env_var)
+    plumbing.name = (porcelain.name)
+    plumbing.server_address = (porcelain.server_address)
+    plumbing.tags.CopyFrom(convert_tags_to_plumbing(porcelain.tags))
+    return plumbing
+
+
+def convert_repeated_keyfactor_x_509_store_to_plumbing(porcelains):
+    return [
+        convert_keyfactor_x_509_store_to_plumbing(porcelain)
+        for porcelain in porcelains
+    ]
+
+
+def convert_repeated_keyfactor_x_509_store_to_porcelain(plumbings):
+    return [
+        convert_keyfactor_x_509_store_to_porcelain(plumbing)
+        for plumbing in plumbings
+    ]
+
+
 def convert_kubernetes_to_porcelain(plumbing):
     if plumbing is None:
         return None
     porcelain = models.Kubernetes()
     porcelain.bind_interface = (plumbing.bind_interface)
     porcelain.certificate_authority = (plumbing.certificate_authority)
     porcelain.client_certificate = (plumbing.client_certificate)
@@ -9643,14 +9705,17 @@
     if isinstance(porcelain, models.DelineaStore):
         plumbing.delinea.CopyFrom(convert_delinea_store_to_plumbing(porcelain))
     if isinstance(porcelain, models.GCPStore):
         plumbing.gcp.CopyFrom(convert_gcp_store_to_plumbing(porcelain))
     if isinstance(porcelain, models.GCPCertX509Store):
         plumbing.gcp_cert_x_509.CopyFrom(
             convert_gcp_cert_x_509_store_to_plumbing(porcelain))
+    if isinstance(porcelain, models.KeyfactorX509Store):
+        plumbing.keyfactor_x_509.CopyFrom(
+            convert_keyfactor_x_509_store_to_plumbing(porcelain))
     if isinstance(porcelain, models.VaultAppRoleStore):
         plumbing.vault_app_role.CopyFrom(
             convert_vault_app_role_store_to_plumbing(porcelain))
     if isinstance(porcelain, models.VaultAppRoleCertSSHStore):
         plumbing.vault_app_role_cert_ssh.CopyFrom(
             convert_vault_app_role_cert_ssh_store_to_plumbing(porcelain))
     if isinstance(porcelain, models.VaultAppRoleCertX509Store):
@@ -9701,14 +9766,17 @@
     if plumbing.HasField('delinea'):
         return convert_delinea_store_to_porcelain(plumbing.delinea)
     if plumbing.HasField('gcp'):
         return convert_gcp_store_to_porcelain(plumbing.gcp)
     if plumbing.HasField('gcp_cert_x_509'):
         return convert_gcp_cert_x_509_store_to_porcelain(
             plumbing.gcp_cert_x_509)
+    if plumbing.HasField('keyfactor_x_509'):
+        return convert_keyfactor_x_509_store_to_porcelain(
+            plumbing.keyfactor_x_509)
     if plumbing.HasField('vault_app_role'):
         return convert_vault_app_role_store_to_porcelain(
             plumbing.vault_app_role)
     if plumbing.HasField('vault_app_role_cert_ssh'):
         return convert_vault_app_role_cert_ssh_store_to_porcelain(
             plumbing.vault_app_role_cert_ssh)
     if plumbing.HasField('vault_app_role_cert_x_509'):
```

## Comparing `strongdm-8.0.0/strongdm/resources_pb2_grpc.py` & `strongdm-8.1.0/strongdm/resources_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/workflows_history_pb2_grpc.py` & `strongdm-8.1.0/strongdm/workflows_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/nodes_history_pb2.py` & `strongdm-8.1.0/strongdm/nodes_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/spec_pb2_grpc.py` & `strongdm-8.1.0/strongdm/options_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/access_request_events_history_pb2_grpc.py` & `strongdm-8.1.0/strongdm/access_request_events_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/queries_pb2_grpc.py` & `strongdm-8.1.0/strongdm/queries_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/peering_groups_pb2_grpc.py` & `strongdm-8.1.0/strongdm/peering_groups_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/nodes_history_pb2_grpc.py` & `strongdm-8.1.0/strongdm/nodes_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/account_grants_history_pb2.py` & `strongdm-8.1.0/strongdm/account_grants_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/organization_history_pb2.py` & `strongdm-8.1.0/strongdm/organization_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/secret_stores_history_pb2.py` & `strongdm-8.1.0/strongdm/secret_stores_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/resources_history_pb2_grpc.py` & `strongdm-8.1.0/strongdm/resources_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/remote_identity_groups_pb2_grpc.py` & `strongdm-8.1.0/strongdm/remote_identity_groups_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/secret_stores_pb2.py` & `strongdm-8.1.0/strongdm/secret_stores_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/workflow_assignments_pb2_grpc.py` & `strongdm-8.1.0/strongdm/workflow_assignments_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/account_resources_history_pb2.py` & `strongdm-8.1.0/strongdm/account_resources_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/client.py` & `strongdm-8.1.0/strongdm/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 # These defaults are taken from AWS. Customization of these values
 # is a future step in the API.
 DEFAULT_MAX_RETRIES = 3
 DEFAULT_BASE_RETRY_DELAY = 0.0030  # 30 ms
 DEFAULT_MAX_RETRY_DELAY = 300  # 300 seconds
 API_VERSION = '2024-03-28'
-USER_AGENT = 'strongdm-sdk-python/8.0.0'
+USER_AGENT = 'strongdm-sdk-python/8.1.0'
 
 
 class Client:
     '''Client interacts with the strongDM API.'''
     def __init__(self,
                  api_access_key,
                  api_secret,
```

## Comparing `strongdm-8.0.0/strongdm/peering_group_peers_pb2.py` & `strongdm-8.1.0/strongdm/peering_group_peers_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/approval_workflow_approvers_pb2_grpc.py` & `strongdm-8.1.0/strongdm/approval_workflow_approvers_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/remote_identities_pb2_grpc.py` & `strongdm-8.1.0/strongdm/remote_identities_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/drivers_pb2_grpc.py` & `strongdm-8.1.0/strongdm/drivers_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/account_permissions_pb2_grpc.py` & `strongdm-8.1.0/strongdm/account_permissions_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/access_request_events_history_pb2.py` & `strongdm-8.1.0/strongdm/access_request_events_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/nodes_pb2.py` & `strongdm-8.1.0/strongdm/nodes_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/organization_history_pb2_grpc.py` & `strongdm-8.1.0/strongdm/organization_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/account_attachments_history_pb2_grpc.py` & `strongdm-8.1.0/strongdm/account_attachments_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/drivers_pb2.py` & `strongdm-8.1.0/strongdm/drivers_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/account_grants_pb2.py` & `strongdm-8.1.0/strongdm/account_grants_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/account_resources_pb2_grpc.py` & `strongdm-8.1.0/strongdm/account_resources_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/access_requests_pb2.py` & `strongdm-8.1.0/strongdm/access_requests_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/nodes_pb2_grpc.py` & `strongdm-8.1.0/strongdm/nodes_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/secret_stores_pb2_grpc.py` & `strongdm-8.1.0/strongdm/secret_stores_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/role_resources_pb2_grpc.py` & `strongdm-8.1.0/strongdm/role_resources_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/peering_group_resources_pb2.py` & `strongdm-8.1.0/strongdm/peering_group_resources_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/account_attachments_pb2_grpc.py` & `strongdm-8.1.0/strongdm/account_attachments_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/role_resources_history_pb2.py` & `strongdm-8.1.0/strongdm/role_resources_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/peering_group_peers_pb2_grpc.py` & `strongdm-8.1.0/strongdm/peering_group_peers_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/workflows_pb2_grpc.py` & `strongdm-8.1.0/strongdm/workflows_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/access_requests_history_pb2.py` & `strongdm-8.1.0/strongdm/access_requests_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/workflow_assignments_history_pb2.py` & `strongdm-8.1.0/strongdm/workflow_assignments_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/remote_identity_groups_history_pb2_grpc.py` & `strongdm-8.1.0/strongdm/remote_identity_groups_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/control_panel_pb2_grpc.py` & `strongdm-8.1.0/strongdm/control_panel_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/accounts_history_pb2_grpc.py` & `strongdm-8.1.0/strongdm/accounts_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/approval_workflows_history_pb2_grpc.py` & `strongdm-8.1.0/strongdm/approval_workflows_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/workflow_roles_history_pb2_grpc.py` & `strongdm-8.1.0/strongdm/workflow_roles_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/access_requests_history_pb2_grpc.py` & `strongdm-8.1.0/strongdm/access_requests_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/workflow_roles_pb2.py` & `strongdm-8.1.0/strongdm/workflow_roles_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/tags_pb2.py` & `strongdm-8.1.0/strongdm/tags_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/remote_identities_history_pb2.py` & `strongdm-8.1.0/strongdm/remote_identities_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/replays_pb2.py` & `strongdm-8.1.0/strongdm/replays_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/activities_pb2.py` & `strongdm-8.1.0/strongdm/activities_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/workflow_assignments_pb2.py` & `strongdm-8.1.0/strongdm/workflow_assignments_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/account_grants_history_pb2_grpc.py` & `strongdm-8.1.0/strongdm/account_grants_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/svc.py` & `strongdm-8.1.0/strongdm/svc.py`

 * *Files 0% similar despite different names*

```diff
@@ -4308,14 +4308,15 @@
     `strongdm.models.AzureStore`
     `strongdm.models.CyberarkConjurStore`
     `strongdm.models.CyberarkPAMStore`
     `strongdm.models.CyberarkPAMExperimentalStore`
     `strongdm.models.DelineaStore`
     `strongdm.models.GCPStore`
     `strongdm.models.GCPCertX509Store`
+    `strongdm.models.KeyfactorX509Store`
     `strongdm.models.VaultAppRoleStore`
     `strongdm.models.VaultAppRoleCertSSHStore`
     `strongdm.models.VaultAppRoleCertX509Store`
     `strongdm.models.VaultTLSStore`
     `strongdm.models.VaultTLSCertSSHStore`
     `strongdm.models.VaultTLSCertX509Store`
     `strongdm.models.VaultTokenStore`
```

## Comparing `strongdm-8.0.0/strongdm/approval_workflow_steps_history_pb2_grpc.py` & `strongdm-8.1.0/strongdm/approval_workflow_steps_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/constants.py` & `strongdm-8.1.0/strongdm/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,17 +236,21 @@
     ORG_EXTEND_TRIAL = "trial extended"
     SECRET_STORE_ADDED = "secret store added"
     SECRET_STORE_UPDATED = "secret store updated"
     SECRET_STORE_DELETED = "secret store deleted"
     REMOTE_IDENTITY_GROUP_CREATED = "remote identity group created"
     REMOTE_IDENTITY_GROUP_UPDATED = "remote identity group updated"
     REMOTE_IDENTITY_GROUP_DELETED = "remote identity group deleted"
+    IDENTITY_SET_PROVISIONING_ENABLED = "identity set provisioning enabled"
+    IDENTITY_SET_PROVISIONING_DISABLED = "identity set provisioning disabled"
     REMOTE_IDENTITY_CREATED = "remote identity created"
     REMOTE_IDENTITY_UPDATED = "remote identity updated"
     REMOTE_IDENTITY_DELETED = "remote identity deleted"
+    IDENTITY_ALIAS_PROVISIONING_ENABLED = "identity alias provisioning enabled"
+    IDENTITY_ALIAS_PROVISIONING_DISABLED = "identity alias provisioning disabled"
     ACCESS_REQUESTED_TO_RESOURCE = "access requested to resource"
     ACCESS_REQUEST_TO_RESOURCE_APPROVAL_ADDED = "access request to resource approval added"
     ACCESS_REQUEST_TO_RESOURCE_CANCELED = "access request to resource canceled"
     ACCESS_REQUEST_TO_RESOURCE_DENIED = "access request to resource denied"
     ACCESS_REQUEST_TO_RESOURCE_TIMED_OUT = "access request to resource timed out"
     ACCESS_REQUEST_TO_RESOURCE_GRANTED = "access request to resource granted"
     ACCESS_REQUEST_TO_RESOURCE_GRANTED_AUTOMATICALLY = "access request to resource granted automatically"
```

## Comparing `strongdm-8.0.0/strongdm/peering_group_nodes_pb2_grpc.py` & `strongdm-8.1.0/strongdm/peering_group_nodes_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/remote_identity_groups_history_pb2.py` & `strongdm-8.1.0/strongdm/remote_identity_groups_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/tags_pb2_grpc.py` & `strongdm-8.1.0/strongdm/spec_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/secret_stores_history_pb2_grpc.py` & `strongdm-8.1.0/strongdm/secret_stores_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/peering_groups_pb2.py` & `strongdm-8.1.0/strongdm/peering_groups_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/secret_store_types_pb2_grpc.py` & `strongdm-8.1.0/strongdm/tags_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/account_grants_pb2_grpc.py` & `strongdm-8.1.0/strongdm/account_grants_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/workflows_pb2.py` & `strongdm-8.1.0/strongdm/workflows_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/approval_workflow_steps_pb2_grpc.py` & `strongdm-8.1.0/strongdm/approval_workflow_steps_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/approval_workflows_pb2_grpc.py` & `strongdm-8.1.0/strongdm/approval_workflows_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/access_requests_pb2_grpc.py` & `strongdm-8.1.0/strongdm/access_requests_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/account_attachments_pb2.py` & `strongdm-8.1.0/strongdm/account_attachments_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/role_resources_history_pb2_grpc.py` & `strongdm-8.1.0/strongdm/role_resources_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/roles_history_pb2_grpc.py` & `strongdm-8.1.0/strongdm/roles_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/queries_pb2.py` & `strongdm-8.1.0/strongdm/queries_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/options_pb2.py` & `strongdm-8.1.0/strongdm/options_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\roptions.proto\x12\x02v1\x1a google/protobuf/descriptor.proto\"9\n\x0b\x46ileOptions\x12\x11\n\x07targets\x18\xc4\xc1v \x03(\t:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"\xaa\x01\n\x0eServiceOptions\x12\x13\n\tmain_noun\x18\x98\xbfv \x01(\t\x12\x13\n\tid_prefix\x18\x9a\xbfv \x01(\t\x12\x11\n\x07targets\x18\x99\xbfv \x03(\t\x12#\n\x19\x64isable_snapshot_vertical\x18\x9b\xbfv \x01(\x08\x12\x1d\n\x13skip_cli_generation\x18\x9c\xbfv \x01(\x08:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"x\n\rMethodOptions\x12\x10\n\x06method\x18\xb4\xbev \x01(\t\x12\r\n\x03url\x18\xb5\xbev \x01(\t\x12\x1a\n\x10\x64\x65precation_date\x18\xb6\xbev \x01(\t\x12\x11\n\x07targets\x18\x99\xbfv \x03(\t:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"\xcd\x01\n\x0eMessageOptions\x12\x13\n\tporcelain\x18\xb5\xbev \x01(\x08\x12\x0f\n\x05\x65rror\x18\xb6\xbev \x01(\x05\x12\x17\n\roptions_field\x18\xb7\xbev \x01(\t\x12\x11\n\x07targets\x18\xba\xbev \x03(\t\x12+\n\x0eterraform_docs\x18\xb8\xbev \x01(\x0b\x32\x11.v1.TerraformDocs\x12#\n\x06\x63ustom\x18\xb9\xbev \x01(\x0b\x32\x11.v1.CustomOptions:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"@\n\x0cOneofOptions\x12\x17\n\rcommon_fields\x18\x85\xbfv \x03(\t:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"\x8f\x04\n\x0c\x46ieldOptions\x12\x13\n\tporcelain\x18\xb6\xbev \x01(\x08\x12\x12\n\x08iterable\x18\xb7\xbev \x01(\x08\x12\x12\n\x08required\x18\xb8\xbev \x01(\x08\x12\x14\n\nwrite_only\x18\xbd\xbev \x01(\x08\x12\x13\n\tread_only\x18\xc3\xbev \x01(\x08\x12\x17\n\ris_credential\x18\xc4\xbev \x01(\x08\x12\x11\n\x07targets\x18\xc6\xbev \x03(\t\x12\x1d\n\x13terraform_force_new\x18\xbc\xbev \x01(\x08\x12\x1d\n\x13terraform_sensitive\x18\xbe\xbev \x01(\x08\x12&\n\x1cterraform_diff_suppress_func\x18\xc7\xbev \x01(\t\x12\x1c\n\x12terraform_computed\x18\xca\xbev \x01(\x08\x12#\n\x06\x63ustom\x18\xb9\xbev \x01(\x0b\x32\x11.v1.CustomOptions\x12\x44\n\x12read_only_override\x18\xc0\xbev \x03(\x0b\x32&.v1.FieldOptions.ReadOnlyOverrideEntry\x12\x13\n\tcondition\x18\xcb\xbev \x01(\t\x12\x15\n\x0b\x65xpect_file\x18\xcc\xbev \x01(\x08\x1a\x37\n\x15ReadOnlyOverrideEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"\x8f\x05\n\rCustomOptions\x12\x13\n\tconverter\x18\xbd\xbev \x01(\t\x12O\n\x17porcelain_type_override\x18\xbe\xbev \x03(\x0b\x32,.v1.CustomOptions.PorcelainTypeOverrideEntry\x12O\n\x17porcelain_name_override\x18\xc8\xbev \x03(\x0b\x32,.v1.CustomOptions.PorcelainNameOverrideEntry\x12\x42\n\x10\x63omment_override\x18\xd3\xbev \x03(\x0b\x32&.v1.CustomOptions.CommentOverrideEntry\x12H\n\x13\x64\x65precated_override\x18\xc0\xbev \x03(\x0b\x32).v1.CustomOptions.DeprecatedOverrideEntry\x12\x1d\n\x13terraform_elem_type\x18\xbf\xbev \x01(\t\x12\x12\n\x08unstable\x18\xc1\xbev \x01(\x08\x1a<\n\x1aPorcelainTypeOverrideEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a<\n\x1aPorcelainNameOverrideEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x36\n\x14\x43ommentOverrideEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x39\n\x17\x44\x65precatedOverrideEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"m\n\rTerraformDocs\x12\x1f\n\x15resource_example_path\x18\xb4\xbev \x01(\t\x12\"\n\x18\x64\x61ta_source_example_path\x18\xb5\xbev \x01(\t:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway:E\n\x0c\x66ile_options\x12\x1c.google.protobuf.FileOptions\x18\xa8\xc2v \x01(\x0b\x32\x0f.v1.FileOptions:N\n\x0fservice_options\x12\x1f.google.protobuf.ServiceOptions\x18\x99\xbfv \x01(\x0b\x32\x12.v1.ServiceOptions:K\n\x0emethod_options\x12\x1e.google.protobuf.MethodOptions\x18\x90\xbfv \x01(\x0b\x32\x11.v1.MethodOptions:N\n\x0fmessage_options\x12\x1f.google.protobuf.MessageOptions\x18\x8f\xbfv \x01(\x0b\x32\x12.v1.MessageOptions:H\n\roneof_options\x12\x1d.google.protobuf.OneofOptions\x18\x85\xbfv \x01(\x0b\x32\x10.v1.OneofOptions:H\n\rfield_options\x12\x1d.google.protobuf.FieldOptions\x18\x8e\xbfv \x01(\x0b\x32\x10.v1.FieldOptionsBR\n\x19\x63om.strongdm.api.plumbingZ5github.com/strongdm/strongdm-sdk-go/v3/internal/v1;v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\roptions.proto\x12\x02v1\x1a google/protobuf/descriptor.proto\"9\n\x0b\x46ileOptions\x12\x11\n\x07targets\x18\xc4\xc1v \x03(\t:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"\xaa\x01\n\x0eServiceOptions\x12\x13\n\tmain_noun\x18\x98\xbfv \x01(\t\x12\x13\n\tid_prefix\x18\x9a\xbfv \x01(\t\x12\x11\n\x07targets\x18\x99\xbfv \x03(\t\x12#\n\x19\x64isable_snapshot_vertical\x18\x9b\xbfv \x01(\x08\x12\x1d\n\x13skip_cli_generation\x18\x9c\xbfv \x01(\x08:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"x\n\rMethodOptions\x12\x10\n\x06method\x18\xb4\xbev \x01(\t\x12\r\n\x03url\x18\xb5\xbev \x01(\t\x12\x1a\n\x10\x64\x65precation_date\x18\xb6\xbev \x01(\t\x12\x11\n\x07targets\x18\x99\xbfv \x03(\t:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"\xf2\x01\n\x0eMessageOptions\x12\x13\n\tporcelain\x18\xb5\xbev \x01(\x08\x12\x0f\n\x05\x65rror\x18\xb6\xbev \x01(\x05\x12\x17\n\roptions_field\x18\xb7\xbev \x01(\t\x12\x11\n\x07targets\x18\xba\xbev \x03(\t\x12+\n\x0eterraform_docs\x18\xb8\xbev \x01(\x0b\x32\x11.v1.TerraformDocs\x12#\n\x06\x63ustom\x18\xb9\xbev \x01(\x0b\x32\x11.v1.CustomOptions\x12#\n\x19terraform_datasource_only\x18\xbb\xbev \x01(\x08:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"@\n\x0cOneofOptions\x12\x17\n\rcommon_fields\x18\x85\xbfv \x03(\t:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"\x8f\x04\n\x0c\x46ieldOptions\x12\x13\n\tporcelain\x18\xb6\xbev \x01(\x08\x12\x12\n\x08iterable\x18\xb7\xbev \x01(\x08\x12\x12\n\x08required\x18\xb8\xbev \x01(\x08\x12\x14\n\nwrite_only\x18\xbd\xbev \x01(\x08\x12\x13\n\tread_only\x18\xc3\xbev \x01(\x08\x12\x17\n\ris_credential\x18\xc4\xbev \x01(\x08\x12\x11\n\x07targets\x18\xc6\xbev \x03(\t\x12\x1d\n\x13terraform_force_new\x18\xbc\xbev \x01(\x08\x12\x1d\n\x13terraform_sensitive\x18\xbe\xbev \x01(\x08\x12&\n\x1cterraform_diff_suppress_func\x18\xc7\xbev \x01(\t\x12\x1c\n\x12terraform_computed\x18\xca\xbev \x01(\x08\x12#\n\x06\x63ustom\x18\xb9\xbev \x01(\x0b\x32\x11.v1.CustomOptions\x12\x44\n\x12read_only_override\x18\xc0\xbev \x03(\x0b\x32&.v1.FieldOptions.ReadOnlyOverrideEntry\x12\x13\n\tcondition\x18\xcb\xbev \x01(\t\x12\x15\n\x0b\x65xpect_file\x18\xcc\xbev \x01(\x08\x1a\x37\n\x15ReadOnlyOverrideEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"\x8f\x05\n\rCustomOptions\x12\x13\n\tconverter\x18\xbd\xbev \x01(\t\x12O\n\x17porcelain_type_override\x18\xbe\xbev \x03(\x0b\x32,.v1.CustomOptions.PorcelainTypeOverrideEntry\x12O\n\x17porcelain_name_override\x18\xc8\xbev \x03(\x0b\x32,.v1.CustomOptions.PorcelainNameOverrideEntry\x12\x42\n\x10\x63omment_override\x18\xd3\xbev \x03(\x0b\x32&.v1.CustomOptions.CommentOverrideEntry\x12H\n\x13\x64\x65precated_override\x18\xc0\xbev \x03(\x0b\x32).v1.CustomOptions.DeprecatedOverrideEntry\x12\x1d\n\x13terraform_elem_type\x18\xbf\xbev \x01(\t\x12\x12\n\x08unstable\x18\xc1\xbev \x01(\x08\x1a<\n\x1aPorcelainTypeOverrideEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a<\n\x1aPorcelainNameOverrideEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x36\n\x14\x43ommentOverrideEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x39\n\x17\x44\x65precatedOverrideEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway\"m\n\rTerraformDocs\x12\x1f\n\x15resource_example_path\x18\xb4\xbev \x01(\t\x12\"\n\x18\x64\x61ta_source_example_path\x18\xb5\xbev \x01(\t:\x17\xfa\xf8\xb3\x07\x12\xd2\xf3\xb3\x07\r!json_gateway:E\n\x0c\x66ile_options\x12\x1c.google.protobuf.FileOptions\x18\xa8\xc2v \x01(\x0b\x32\x0f.v1.FileOptions:N\n\x0fservice_options\x12\x1f.google.protobuf.ServiceOptions\x18\x99\xbfv \x01(\x0b\x32\x12.v1.ServiceOptions:K\n\x0emethod_options\x12\x1e.google.protobuf.MethodOptions\x18\x90\xbfv \x01(\x0b\x32\x11.v1.MethodOptions:N\n\x0fmessage_options\x12\x1f.google.protobuf.MessageOptions\x18\x8f\xbfv \x01(\x0b\x32\x12.v1.MessageOptions:H\n\roneof_options\x12\x1d.google.protobuf.OneofOptions\x18\x85\xbfv \x01(\x0b\x32\x10.v1.OneofOptions:H\n\rfield_options\x12\x1d.google.protobuf.FieldOptions\x18\x8e\xbfv \x01(\x0b\x32\x10.v1.FieldOptionsBR\n\x19\x63om.strongdm.api.plumbingZ5github.com/strongdm/strongdm-sdk-go/v3/internal/v1;v1b\x06proto3')
 
 
 FILE_OPTIONS_FIELD_NUMBER = 1941800
 file_options = DESCRIPTOR.extensions_by_name['file_options']
 SERVICE_OPTIONS_FIELD_NUMBER = 1941401
 service_options = DESCRIPTOR.extensions_by_name['service_options']
 METHOD_OPTIONS_FIELD_NUMBER = 1941392
@@ -193,27 +193,27 @@
   _FILEOPTIONS._serialized_start=55
   _FILEOPTIONS._serialized_end=112
   _SERVICEOPTIONS._serialized_start=115
   _SERVICEOPTIONS._serialized_end=285
   _METHODOPTIONS._serialized_start=287
   _METHODOPTIONS._serialized_end=407
   _MESSAGEOPTIONS._serialized_start=410
-  _MESSAGEOPTIONS._serialized_end=615
-  _ONEOFOPTIONS._serialized_start=617
-  _ONEOFOPTIONS._serialized_end=681
-  _FIELDOPTIONS._serialized_start=684
-  _FIELDOPTIONS._serialized_end=1211
-  _FIELDOPTIONS_READONLYOVERRIDEENTRY._serialized_start=1131
-  _FIELDOPTIONS_READONLYOVERRIDEENTRY._serialized_end=1186
-  _CUSTOMOPTIONS._serialized_start=1214
-  _CUSTOMOPTIONS._serialized_end=1869
-  _CUSTOMOPTIONS_PORCELAINTYPEOVERRIDEENTRY._serialized_start=1607
-  _CUSTOMOPTIONS_PORCELAINTYPEOVERRIDEENTRY._serialized_end=1667
-  _CUSTOMOPTIONS_PORCELAINNAMEOVERRIDEENTRY._serialized_start=1669
-  _CUSTOMOPTIONS_PORCELAINNAMEOVERRIDEENTRY._serialized_end=1729
-  _CUSTOMOPTIONS_COMMENTOVERRIDEENTRY._serialized_start=1731
-  _CUSTOMOPTIONS_COMMENTOVERRIDEENTRY._serialized_end=1785
-  _CUSTOMOPTIONS_DEPRECATEDOVERRIDEENTRY._serialized_start=1787
-  _CUSTOMOPTIONS_DEPRECATEDOVERRIDEENTRY._serialized_end=1844
-  _TERRAFORMDOCS._serialized_start=1871
-  _TERRAFORMDOCS._serialized_end=1980
+  _MESSAGEOPTIONS._serialized_end=652
+  _ONEOFOPTIONS._serialized_start=654
+  _ONEOFOPTIONS._serialized_end=718
+  _FIELDOPTIONS._serialized_start=721
+  _FIELDOPTIONS._serialized_end=1248
+  _FIELDOPTIONS_READONLYOVERRIDEENTRY._serialized_start=1168
+  _FIELDOPTIONS_READONLYOVERRIDEENTRY._serialized_end=1223
+  _CUSTOMOPTIONS._serialized_start=1251
+  _CUSTOMOPTIONS._serialized_end=1906
+  _CUSTOMOPTIONS_PORCELAINTYPEOVERRIDEENTRY._serialized_start=1644
+  _CUSTOMOPTIONS_PORCELAINTYPEOVERRIDEENTRY._serialized_end=1704
+  _CUSTOMOPTIONS_PORCELAINNAMEOVERRIDEENTRY._serialized_start=1706
+  _CUSTOMOPTIONS_PORCELAINNAMEOVERRIDEENTRY._serialized_end=1766
+  _CUSTOMOPTIONS_COMMENTOVERRIDEENTRY._serialized_start=1768
+  _CUSTOMOPTIONS_COMMENTOVERRIDEENTRY._serialized_end=1822
+  _CUSTOMOPTIONS_DEPRECATEDOVERRIDEENTRY._serialized_start=1824
+  _CUSTOMOPTIONS_DEPRECATEDOVERRIDEENTRY._serialized_end=1881
+  _TERRAFORMDOCS._serialized_start=1908
+  _TERRAFORMDOCS._serialized_end=2017
 # @@protoc_insertion_point(module_scope)
```

## Comparing `strongdm-8.0.0/strongdm/approval_workflow_steps_pb2.py` & `strongdm-8.1.0/strongdm/approval_workflow_steps_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/approval_workflow_approvers_pb2.py` & `strongdm-8.1.0/strongdm/approval_workflow_approvers_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/accounts_pb2_grpc.py` & `strongdm-8.1.0/strongdm/accounts_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/peering_group_resources_pb2_grpc.py` & `strongdm-8.1.0/strongdm/peering_group_resources_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/account_attachments_history_pb2.py` & `strongdm-8.1.0/strongdm/account_attachments_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/secret_store_types_pb2.py` & `strongdm-8.1.0/strongdm/secret_store_types_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,29 +26,30 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import options_pb2 as options__pb2
 from . import tags_pb2 as tags__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18secret_store_types.proto\x12\x02v1\x1a\roptions.proto\x1a\ntags.proto\"\xa6\x10\n\x0bSecretStore\x12I\n\x03\x61ws\x18\x03 \x01(\x0b\x32\x0c.v1.AWSStoreB,\xf2\xf8\xb3\x07\x1d\xca\xf3\xb3\x07\x18\xc2\xf4\xb3\x07\x13\n\x0cjson_gateway\x12\x03\x61ws\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x64\n\x0e\x61ws_cert_x_509\x18\x1e \x01(\x0b\x32\x14.v1.AWSCertX509StoreB4\xf2\xf8\xb3\x07%\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0b\x61wsCertX509\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12o\n\x10\x61\x63tive_directory\x18\x9a\x05 \x01(\x0b\x32\x18.v1.ActiveDirectoryStoreB8\xf2\xf8\xb3\x07)\xca\xf3\xb3\x07$\xc2\xf4\xb3\x07\x1f\n\x0cjson_gateway\x12\x0f\x61\x63tiveDirectory\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12O\n\x05\x61zure\x18\x65 \x01(\x0b\x32\x0e.v1.AzureStoreB.\xf2\xf8\xb3\x07\x1f\xca\xf3\xb3\x07\x1a\xc2\xf4\xb3\x07\x15\n\x0cjson_gateway\x12\x05\x61zure\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12l\n\x0f\x63yberark_conjur\x18\xad\x02 \x01(\x0b\x32\x17.v1.CyberarkConjurStoreB7\xf2\xf8\xb3\x07(\xca\xf3\xb3\x07#\xc2\xf4\xb3\x07\x1e\n\x0cjson_gateway\x12\x0e\x63yberarkConjur\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x63\n\x0c\x63yberark_pam\x18\xaf\x02 \x01(\x0b\x32\x14.v1.CyberarkPAMStoreB4\xf2\xf8\xb3\x07%\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0b\x63yberarkPAM\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x88\x01\n\x19\x63yberark_pam_experimental\x18\xae\x02 \x01(\x0b\x32 .v1.CyberarkPAMExperimentalStoreB@\xf2\xf8\xb3\x07\x31\xca\xf3\xb3\x07,\xc2\xf4\xb3\x07\'\n\x0cjson_gateway\x12\x17\x63yberarkPAMExperimental\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12V\n\x07\x64\x65linea\x18\xd4\x16 \x01(\x0b\x32\x10.v1.DelineaStoreB0\xf2\xf8\xb3\x07!\xca\xf3\xb3\x07\x1c\xc2\xf4\xb3\x07\x17\n\x0cjson_gateway\x12\x07\x64\x65linea\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12J\n\x03gcp\x18\xc9\x01 \x01(\x0b\x32\x0c.v1.GCPStoreB,\xf2\xf8\xb3\x07\x1d\xca\xf3\xb3\x07\x18\xc2\xf4\xb3\x07\x13\n\x0cjson_gateway\x12\x03gcp\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x65\n\x0egcp_cert_x_509\x18\xca\x01 \x01(\x0b\x32\x14.v1.GCPCertX509StoreB4\xf2\xf8\xb3\x07%\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bgcpCertX509\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x66\n\x0evault_app_role\x18\x04 \x01(\x0b\x32\x15.v1.VaultAppRoleStoreB5\xf2\xf8\xb3\x07&\xca\xf3\xb3\x07!\xc2\xf4\xb3\x07\x1c\n\x0cjson_gateway\x12\x0cvaultAppRole\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12}\n\x17vault_app_role_cert_ssh\x18^ \x01(\x0b\x32\x1c.v1.VaultAppRoleCertSSHStoreB<\xf2\xf8\xb3\x07-\xca\xf3\xb3\x07(\xc2\xf4\xb3\x07#\n\x0cjson_gateway\x12\x13vaultAppRoleCertSSH\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x81\x01\n\x19vault_app_role_cert_x_509\x18_ \x01(\x0b\x32\x1d.v1.VaultAppRoleCertX509StoreB=\xf2\xf8\xb3\x07.\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14vaultAppRoleCertX509\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12Y\n\tvault_tls\x18\x01 \x01(\x0b\x32\x11.v1.VaultTLSStoreB1\xf2\xf8\xb3\x07\"\xca\xf3\xb3\x07\x1d\xc2\xf4\xb3\x07\x18\n\x0cjson_gateway\x12\x08vaultTLS\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12p\n\x12vault_tls_cert_ssh\x18\\ \x01(\x0b\x32\x18.v1.VaultTLSCertSSHStoreB8\xf2\xf8\xb3\x07)\xca\xf3\xb3\x07$\xc2\xf4\xb3\x07\x1f\n\x0cjson_gateway\x12\x0fvaultTLSCertSSH\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12t\n\x14vault_tls_cert_x_509\x18] \x01(\x0b\x32\x19.v1.VaultTLSCertX509StoreB9\xf2\xf8\xb3\x07*\xca\xf3\xb3\x07%\xc2\xf4\xb3\x07 \n\x0cjson_gateway\x12\x10vaultTLSCertX509\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12_\n\x0bvault_token\x18\x02 \x01(\x0b\x32\x13.v1.VaultTokenStoreB3\xf2\xf8\xb3\x07$\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\nvaultToken\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12v\n\x14vault_token_cert_ssh\x18Z \x01(\x0b\x32\x1a.v1.VaultTokenCertSSHStoreB:\xf2\xf8\xb3\x07+\xca\xf3\xb3\x07&\xc2\xf4\xb3\x07!\n\x0cjson_gateway\x12\x11vaultTokenCertSSH\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12z\n\x16vault_token_cert_x_509\x18[ \x01(\x0b\x32\x1b.v1.VaultTokenCertX509StoreB;\xf2\xf8\xb3\x07,\xca\xf3\xb3\x07\'\xc2\xf4\xb3\x07\"\n\x0cjson_gateway\x12\x12vaultTokenCertX509\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\x42,\n\x0csecret_store\x12\x1c\xaa\xf8\xb3\x07\t\xaa\xf8\xb3\x07\x04tags\xaa\xf8\xb3\x07\t\xaa\xf8\xb3\x07\x04name\"\xfc\x01\n\x08\x41WSStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12?\n\x06region\x18\x03 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1b\xc2\xf4\xb3\x07\x16\n\x0cjson_gateway\x12\x06region\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:T\xfa\xf8\xb3\x07O\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x45\xc2\xf4\xb3\x07\n\n\x03\x63li\x12\x03\x61ws\xc2\xf4\xb3\x07\x13\n\x0cjson_gateway\x12\x03\x61ws\xc2\xf4\xb3\x07\x19\n\x12terraform-provider\x12\x03\x61ws\"\xe6\x04\n\x10\x41WSCertX509Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12=\n\x05\x63\x61\x41rn\x18\x05 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1a\xc2\xf4\xb3\x07\x15\n\x0cjson_gateway\x12\x05\x63\x61\x41rn\x12_\n\x16\x63\x65rtificateTemplateArn\x18\x07 \x01(\tB?\xf2\xf8\xb3\x07:\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07+\xc2\xf4\xb3\x07&\n\x0cjson_gateway\x12\x16\x63\x65rtificateTemplateArn\x12[\n\x14issuedCertTTLMinutes\x18\x08 \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12?\n\x06region\x18\x03 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1b\xc2\xf4\xb3\x07\x16\n\x0cjson_gateway\x12\x06region\x12I\n\x0bsigningAlgo\x18\x06 \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningAlgo\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:n\xfa\xf8\xb3\x07i\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07_\xc2\xf4\xb3\x07\x12\n\x03\x63li\x12\x0b\x61wsCertX509\xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0b\x61wsCertX509\xc2\xf4\xb3\x07#\n\x12terraform-provider\x12\raws_cert_x509\"\x93\x02\n\x14\x41\x63tiveDirectoryStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:N\xfa\xf8\xb3\x07I\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07?\xc2\xf4\xb3\x07\x16\n\x03\x63li\x12\x0f\x61\x63tiveDirectory\xc2\xf4\xb3\x07\x1f\n\x0cjson_gateway\x12\x0f\x61\x63tiveDirectory\"\xeb\x01\n\nAzureStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x44\n\tvault_uri\x18\x03 \x01(\tB1\xf2\xf8\xb3\x07,\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1d\xc2\xf4\xb3\x07\x18\n\x0cjson_gateway\x12\x08vaultUri\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01::\xfa\xf8\xb3\x07\x35\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07+\xc2\xf4\xb3\x07\x0c\n\x03\x63li\x12\x05\x61zure\xc2\xf4\xb3\x07\x15\n\x0cjson_gateway\x12\x05\x61zure\"\xab\x02\n\x13\x43yberarkConjurStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12?\n\x06\x61ppURL\x18\x03 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1b\xc2\xf4\xb3\x07\x16\n\x0cjson_gateway\x12\x06\x61ppUrl\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:v\xfa\xf8\xb3\x07q\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07g\xc2\xf4\xb3\x07\x15\n\x03\x63li\x12\x0e\x63yberarkConjur\xc2\xf4\xb3\x07\x1e\n\x0cjson_gateway\x12\x0e\x63yberarkConjur\xc2\xf4\xb3\x07%\n\x12terraform-provider\x12\x0f\x63yberark_conjur\"\x9f\x02\n\x10\x43yberarkPAMStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12?\n\x06\x61ppURL\x18\x03 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1b\xc2\xf4\xb3\x07\x16\n\x0cjson_gateway\x12\x06\x61ppUrl\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:m\xfa\xf8\xb3\x07h\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07^\xc2\xf4\xb3\x07\x12\n\x03\x63li\x12\x0b\x63yberarkPAM\xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0b\x63yberarkPAM\xc2\xf4\xb3\x07\"\n\x12terraform-provider\x12\x0c\x63yberark_pam\"\xd8\x02\n\x1c\x43yberarkPAMExperimentalStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12?\n\x06\x61ppURL\x18\x03 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1b\xc2\xf4\xb3\x07\x16\n\x0cjson_gateway\x12\x06\x61ppUrl\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\x99\x01\xfa\xf8\xb3\x07\x93\x01\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x88\x01\x88\xf4\xb3\x07\x01\xc2\xf4\xb3\x07\x1e\n\x03\x63li\x12\x17\x63yberarkPAMExperimental\xc2\xf4\xb3\x07\'\n\x0cjson_gateway\x12\x17\x63yberarkPAMExperimental\xc2\xf4\xb3\x07/\n\x12terraform-provider\x12\x19\x63yberark_pam_experimental\"\xb3\x02\n\x0c\x44\x65lineaStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x41\n\nserver_url\x18\x03 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tserverUrl\x12\x43\n\x0btenant_name\x18\x04 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\ntenantName\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:>\xfa\xf8\xb3\x07\x39\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07/\xc2\xf4\xb3\x07\x0e\n\x03\x63li\x12\x07\x64\x65linea\xc2\xf4\xb3\x07\x17\n\x0cjson_gateway\x12\x07\x64\x65linea\"\xe6\x01\n\x08GCPStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x45\n\tprojectID\x18\x03 \x01(\tB2\xf2\xf8\xb3\x07-\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tprojectId\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:6\xfa\xf8\xb3\x07\x31\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\'\xc2\xf4\xb3\x07\n\n\x03\x63li\x12\x03gcp\xc2\xf4\xb3\x07\x13\n\x0cjson_gateway\x12\x03gcp\"\x9d\x04\n\x10GCPCertX509Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x36\n\x04\x63\x61ID\x18\x06 \x01(\tB(\xf2\xf8\xb3\x07#\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x19\xc2\xf4\xb3\x07\x14\n\x0cjson_gateway\x12\x04\x63\x61Id\x12\x43\n\x08\x63\x61PoolID\x18\x05 \x01(\tB1\xf2\xf8\xb3\x07,\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1d\xc2\xf4\xb3\x07\x18\n\x0cjson_gateway\x12\x08\x63\x61PoolId\x12[\n\x14issuedCertTTLMinutes\x18\x07 \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12\x43\n\x08location\x18\x04 \x01(\tB1\xf2\xf8\xb3\x07,\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1d\xc2\xf4\xb3\x07\x18\n\x0cjson_gateway\x12\x08location\x12\x45\n\tprojectID\x18\x03 \x01(\tB2\xf2\xf8\xb3\x07-\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tprojectId\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:F\xfa\xf8\xb3\x07\x41\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x37\xc2\xf4\xb3\x07\x12\n\x03\x63li\x12\x0bgcpCertX509\xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bgcpCertX509\"\xf2\x02\n\x11VaultAppRoleStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12\"\n\x04tags\x18\x08 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:p\xfa\xf8\xb3\x07k\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x61\xc2\xf4\xb3\x07\x13\n\x03\x63li\x12\x0cvaultAppRole\xc2\xf4\xb3\x07\x1c\n\x0cjson_gateway\x12\x0cvaultAppRole\xc2\xf4\xb3\x07#\n\x12terraform-provider\x12\rvault_approle\"\x8c\x05\n\x18VaultAppRoleCertSSHStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12[\n\x14issuedCertTTLMinutes\x18\t \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\x07 \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12O\n\x0fssh_mount_point\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rsshMountPoint\x12\"\n\x04tags\x18\x08 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\x88\x01\xfa\xf8\xb3\x07\x82\x01\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07x\xc2\xf4\xb3\x07\x1a\n\x03\x63li\x12\x13vaultAppRoleCertSSH\xc2\xf4\xb3\x07#\n\x0cjson_gateway\x12\x13vaultAppRoleCertSSH\xc2\xf4\xb3\x07,\n\x12terraform-provider\x12\x16vault_approle_cert_ssh\"\x90\x05\n\x19VaultAppRoleCertX509Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12[\n\x14issuedCertTTLMinutes\x18\t \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12O\n\x0fpki_mount_point\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rpkiMountPoint\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\x07 \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12\"\n\x04tags\x18\x08 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\x8b\x01\xfa\xf8\xb3\x07\x85\x01\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07{\xc2\xf4\xb3\x07\x1b\n\x03\x63li\x12\x14vaultAppRoleCertX509\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14vaultAppRoleCertX509\xc2\xf4\xb3\x07-\n\x12terraform-provider\x12\x17vault_approle_cert_x509\"\xcc\x04\n\rVaultTLSStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x44\n\x0c\x43\x41_cert_path\x18\x04 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\ncaCertPath\x12Q\n\x10\x63lient_cert_path\x18\x05 \x01(\tB7\xf2\xf8\xb3\x07\x32\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07#\xc2\xf4\xb3\x07\x1e\n\x0cjson_gateway\x12\x0e\x63lientCertPath\x12O\n\x0f\x63lient_key_path\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rclientKeyPath\x12@\n\tnamespace\x18\x08 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12\"\n\x04tags\x18\x07 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:d\xfa\xf8\xb3\x07_\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07U\xc2\xf4\xb3\x07\x0f\n\x03\x63li\x12\x08vaultTLS\xc2\xf4\xb3\x07\x18\n\x0cjson_gateway\x12\x08vaultTLS\xc2\xf4\xb3\x07\x1f\n\x12terraform-provider\x12\tvault_tls\"\xe4\x06\n\x14VaultTLSCertSSHStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x44\n\x0c\x43\x41_cert_path\x18\x04 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\ncaCertPath\x12Q\n\x10\x63lient_cert_path\x18\x05 \x01(\tB7\xf2\xf8\xb3\x07\x32\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07#\xc2\xf4\xb3\x07\x1e\n\x0cjson_gateway\x12\x0e\x63lientCertPath\x12O\n\x0f\x63lient_key_path\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rclientKeyPath\x12[\n\x14issuedCertTTLMinutes\x18\x0b \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x08 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\n \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12O\n\x0fssh_mount_point\x18\t \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rsshMountPoint\x12\"\n\x04tags\x18\x07 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:{\xfa\xf8\xb3\x07v\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07l\xc2\xf4\xb3\x07\x16\n\x03\x63li\x12\x0fvaultTLSCertSSH\xc2\xf4\xb3\x07\x1f\n\x0cjson_gateway\x12\x0fvaultTLSCertSSH\xc2\xf4\xb3\x07(\n\x12terraform-provider\x12\x12vault_tls_cert_ssh\"\xe8\x06\n\x15VaultTLSCertX509Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x44\n\x0c\x43\x41_cert_path\x18\x04 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\ncaCertPath\x12Q\n\x10\x63lient_cert_path\x18\x05 \x01(\tB7\xf2\xf8\xb3\x07\x32\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07#\xc2\xf4\xb3\x07\x1e\n\x0cjson_gateway\x12\x0e\x63lientCertPath\x12O\n\x0f\x63lient_key_path\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rclientKeyPath\x12[\n\x14issuedCertTTLMinutes\x18\x0b \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x08 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12O\n\x0fpki_mount_point\x18\t \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rpkiMountPoint\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\n \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12\"\n\x04tags\x18\x07 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:~\xfa\xf8\xb3\x07y\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07o\xc2\xf4\xb3\x07\x17\n\x03\x63li\x12\x10vaultTLSCertX509\xc2\xf4\xb3\x07 \n\x0cjson_gateway\x12\x10vaultTLSCertX509\xc2\xf4\xb3\x07)\n\x12terraform-provider\x12\x13vault_tls_cert_x509\"\xea\x02\n\x0fVaultTokenStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:j\xfa\xf8\xb3\x07\x65\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07[\xc2\xf4\xb3\x07\x11\n\x03\x63li\x12\nvaultToken\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\nvaultToken\xc2\xf4\xb3\x07!\n\x12terraform-provider\x12\x0bvault_token\"\x83\x05\n\x16VaultTokenCertSSHStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12[\n\x14issuedCertTTLMinutes\x18\t \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\x07 \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12O\n\x0fssh_mount_point\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rsshMountPoint\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\x81\x01\xfa\xf8\xb3\x07|\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07r\xc2\xf4\xb3\x07\x18\n\x03\x63li\x12\x11vaultTokenCertSSH\xc2\xf4\xb3\x07!\n\x0cjson_gateway\x12\x11vaultTokenCertSSH\xc2\xf4\xb3\x07*\n\x12terraform-provider\x12\x14vault_token_cert_ssh\"\x87\x05\n\x17VaultTokenCertX509Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12[\n\x14issuedCertTTLMinutes\x18\x08 \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12O\n\x0fpki_mount_point\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rpkiMountPoint\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\x07 \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\x84\x01\xfa\xf8\xb3\x07\x7f\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07u\xc2\xf4\xb3\x07\x19\n\x03\x63li\x12\x12vaultTokenCertX509\xc2\xf4\xb3\x07\"\n\x0cjson_gateway\x12\x12vaultTokenCertX509\xc2\xf4\xb3\x07+\n\x12terraform-provider\x12\x15vault_token_cert_x509Bm\n\x19\x63om.strongdm.api.plumbingB\x19SecretStoresTypesPlumbingZ5github.com/strongdm/strongdm-sdk-go/v3/internal/v1;v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18secret_store_types.proto\x12\x02v1\x1a\roptions.proto\x1a\ntags.proto\"\x92\x11\n\x0bSecretStore\x12I\n\x03\x61ws\x18\x03 \x01(\x0b\x32\x0c.v1.AWSStoreB,\xf2\xf8\xb3\x07\x1d\xca\xf3\xb3\x07\x18\xc2\xf4\xb3\x07\x13\n\x0cjson_gateway\x12\x03\x61ws\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x64\n\x0e\x61ws_cert_x_509\x18\x1e \x01(\x0b\x32\x14.v1.AWSCertX509StoreB4\xf2\xf8\xb3\x07%\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0b\x61wsCertX509\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12o\n\x10\x61\x63tive_directory\x18\x9a\x05 \x01(\x0b\x32\x18.v1.ActiveDirectoryStoreB8\xf2\xf8\xb3\x07)\xca\xf3\xb3\x07$\xc2\xf4\xb3\x07\x1f\n\x0cjson_gateway\x12\x0f\x61\x63tiveDirectory\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12O\n\x05\x61zure\x18\x65 \x01(\x0b\x32\x0e.v1.AzureStoreB.\xf2\xf8\xb3\x07\x1f\xca\xf3\xb3\x07\x1a\xc2\xf4\xb3\x07\x15\n\x0cjson_gateway\x12\x05\x61zure\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12l\n\x0f\x63yberark_conjur\x18\xad\x02 \x01(\x0b\x32\x17.v1.CyberarkConjurStoreB7\xf2\xf8\xb3\x07(\xca\xf3\xb3\x07#\xc2\xf4\xb3\x07\x1e\n\x0cjson_gateway\x12\x0e\x63yberarkConjur\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x63\n\x0c\x63yberark_pam\x18\xaf\x02 \x01(\x0b\x32\x14.v1.CyberarkPAMStoreB4\xf2\xf8\xb3\x07%\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0b\x63yberarkPAM\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x88\x01\n\x19\x63yberark_pam_experimental\x18\xae\x02 \x01(\x0b\x32 .v1.CyberarkPAMExperimentalStoreB@\xf2\xf8\xb3\x07\x31\xca\xf3\xb3\x07,\xc2\xf4\xb3\x07\'\n\x0cjson_gateway\x12\x17\x63yberarkPAMExperimental\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12V\n\x07\x64\x65linea\x18\xd4\x16 \x01(\x0b\x32\x10.v1.DelineaStoreB0\xf2\xf8\xb3\x07!\xca\xf3\xb3\x07\x1c\xc2\xf4\xb3\x07\x17\n\x0cjson_gateway\x12\x07\x64\x65linea\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12J\n\x03gcp\x18\xc9\x01 \x01(\x0b\x32\x0c.v1.GCPStoreB,\xf2\xf8\xb3\x07\x1d\xca\xf3\xb3\x07\x18\xc2\xf4\xb3\x07\x13\n\x0cjson_gateway\x12\x03gcp\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x65\n\x0egcp_cert_x_509\x18\xca\x01 \x01(\x0b\x32\x14.v1.GCPCertX509StoreB4\xf2\xf8\xb3\x07%\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bgcpCertX509\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12j\n\x0fkeyfactor_x_509\x18\xc8\x01 \x01(\x0b\x32\x16.v1.KeyfactorX509StoreB6\xf2\xf8\xb3\x07\'\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rkeyfactorX509\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x66\n\x0evault_app_role\x18\x04 \x01(\x0b\x32\x15.v1.VaultAppRoleStoreB5\xf2\xf8\xb3\x07&\xca\xf3\xb3\x07!\xc2\xf4\xb3\x07\x1c\n\x0cjson_gateway\x12\x0cvaultAppRole\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12}\n\x17vault_app_role_cert_ssh\x18^ \x01(\x0b\x32\x1c.v1.VaultAppRoleCertSSHStoreB<\xf2\xf8\xb3\x07-\xca\xf3\xb3\x07(\xc2\xf4\xb3\x07#\n\x0cjson_gateway\x12\x13vaultAppRoleCertSSH\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x81\x01\n\x19vault_app_role_cert_x_509\x18_ \x01(\x0b\x32\x1d.v1.VaultAppRoleCertX509StoreB=\xf2\xf8\xb3\x07.\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14vaultAppRoleCertX509\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12Y\n\tvault_tls\x18\x01 \x01(\x0b\x32\x11.v1.VaultTLSStoreB1\xf2\xf8\xb3\x07\"\xca\xf3\xb3\x07\x1d\xc2\xf4\xb3\x07\x18\n\x0cjson_gateway\x12\x08vaultTLS\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12p\n\x12vault_tls_cert_ssh\x18\\ \x01(\x0b\x32\x18.v1.VaultTLSCertSSHStoreB8\xf2\xf8\xb3\x07)\xca\xf3\xb3\x07$\xc2\xf4\xb3\x07\x1f\n\x0cjson_gateway\x12\x0fvaultTLSCertSSH\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12t\n\x14vault_tls_cert_x_509\x18] \x01(\x0b\x32\x19.v1.VaultTLSCertX509StoreB9\xf2\xf8\xb3\x07*\xca\xf3\xb3\x07%\xc2\xf4\xb3\x07 \n\x0cjson_gateway\x12\x10vaultTLSCertX509\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12_\n\x0bvault_token\x18\x02 \x01(\x0b\x32\x13.v1.VaultTokenStoreB3\xf2\xf8\xb3\x07$\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\nvaultToken\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12v\n\x14vault_token_cert_ssh\x18Z \x01(\x0b\x32\x1a.v1.VaultTokenCertSSHStoreB:\xf2\xf8\xb3\x07+\xca\xf3\xb3\x07&\xc2\xf4\xb3\x07!\n\x0cjson_gateway\x12\x11vaultTokenCertSSH\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12z\n\x16vault_token_cert_x_509\x18[ \x01(\x0b\x32\x1b.v1.VaultTokenCertX509StoreB;\xf2\xf8\xb3\x07,\xca\xf3\xb3\x07\'\xc2\xf4\xb3\x07\"\n\x0cjson_gateway\x12\x12vaultTokenCertX509\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\x42,\n\x0csecret_store\x12\x1c\xaa\xf8\xb3\x07\t\xaa\xf8\xb3\x07\x04tags\xaa\xf8\xb3\x07\t\xaa\xf8\xb3\x07\x04name\"\xfc\x01\n\x08\x41WSStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12?\n\x06region\x18\x03 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1b\xc2\xf4\xb3\x07\x16\n\x0cjson_gateway\x12\x06region\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:T\xfa\xf8\xb3\x07O\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x45\xc2\xf4\xb3\x07\n\n\x03\x63li\x12\x03\x61ws\xc2\xf4\xb3\x07\x13\n\x0cjson_gateway\x12\x03\x61ws\xc2\xf4\xb3\x07\x19\n\x12terraform-provider\x12\x03\x61ws\"\xe6\x04\n\x10\x41WSCertX509Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12=\n\x05\x63\x61\x41rn\x18\x05 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1a\xc2\xf4\xb3\x07\x15\n\x0cjson_gateway\x12\x05\x63\x61\x41rn\x12_\n\x16\x63\x65rtificateTemplateArn\x18\x07 \x01(\tB?\xf2\xf8\xb3\x07:\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07+\xc2\xf4\xb3\x07&\n\x0cjson_gateway\x12\x16\x63\x65rtificateTemplateArn\x12[\n\x14issuedCertTTLMinutes\x18\x08 \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12?\n\x06region\x18\x03 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1b\xc2\xf4\xb3\x07\x16\n\x0cjson_gateway\x12\x06region\x12I\n\x0bsigningAlgo\x18\x06 \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningAlgo\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:n\xfa\xf8\xb3\x07i\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07_\xc2\xf4\xb3\x07\x12\n\x03\x63li\x12\x0b\x61wsCertX509\xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0b\x61wsCertX509\xc2\xf4\xb3\x07#\n\x12terraform-provider\x12\raws_cert_x509\"\x93\x02\n\x14\x41\x63tiveDirectoryStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:N\xfa\xf8\xb3\x07I\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07?\xc2\xf4\xb3\x07\x16\n\x03\x63li\x12\x0f\x61\x63tiveDirectory\xc2\xf4\xb3\x07\x1f\n\x0cjson_gateway\x12\x0f\x61\x63tiveDirectory\"\xeb\x01\n\nAzureStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x44\n\tvault_uri\x18\x03 \x01(\tB1\xf2\xf8\xb3\x07,\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1d\xc2\xf4\xb3\x07\x18\n\x0cjson_gateway\x12\x08vaultUri\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01::\xfa\xf8\xb3\x07\x35\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07+\xc2\xf4\xb3\x07\x0c\n\x03\x63li\x12\x05\x61zure\xc2\xf4\xb3\x07\x15\n\x0cjson_gateway\x12\x05\x61zure\"\xab\x02\n\x13\x43yberarkConjurStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12?\n\x06\x61ppURL\x18\x03 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1b\xc2\xf4\xb3\x07\x16\n\x0cjson_gateway\x12\x06\x61ppUrl\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:v\xfa\xf8\xb3\x07q\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07g\xc2\xf4\xb3\x07\x15\n\x03\x63li\x12\x0e\x63yberarkConjur\xc2\xf4\xb3\x07\x1e\n\x0cjson_gateway\x12\x0e\x63yberarkConjur\xc2\xf4\xb3\x07%\n\x12terraform-provider\x12\x0f\x63yberark_conjur\"\x9f\x02\n\x10\x43yberarkPAMStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12?\n\x06\x61ppURL\x18\x03 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1b\xc2\xf4\xb3\x07\x16\n\x0cjson_gateway\x12\x06\x61ppUrl\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:m\xfa\xf8\xb3\x07h\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07^\xc2\xf4\xb3\x07\x12\n\x03\x63li\x12\x0b\x63yberarkPAM\xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0b\x63yberarkPAM\xc2\xf4\xb3\x07\"\n\x12terraform-provider\x12\x0c\x63yberark_pam\"\xd8\x02\n\x1c\x43yberarkPAMExperimentalStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12?\n\x06\x61ppURL\x18\x03 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1b\xc2\xf4\xb3\x07\x16\n\x0cjson_gateway\x12\x06\x61ppUrl\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\x99\x01\xfa\xf8\xb3\x07\x93\x01\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x88\x01\x88\xf4\xb3\x07\x01\xc2\xf4\xb3\x07\x1e\n\x03\x63li\x12\x17\x63yberarkPAMExperimental\xc2\xf4\xb3\x07\'\n\x0cjson_gateway\x12\x17\x63yberarkPAMExperimental\xc2\xf4\xb3\x07/\n\x12terraform-provider\x12\x19\x63yberark_pam_experimental\"\xb3\x02\n\x0c\x44\x65lineaStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x41\n\nserver_url\x18\x03 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tserverUrl\x12\x43\n\x0btenant_name\x18\x04 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\ntenantName\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:>\xfa\xf8\xb3\x07\x39\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07/\xc2\xf4\xb3\x07\x0e\n\x03\x63li\x12\x07\x64\x65linea\xc2\xf4\xb3\x07\x17\n\x0cjson_gateway\x12\x07\x64\x65linea\"\xe6\x01\n\x08GCPStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x45\n\tprojectID\x18\x03 \x01(\tB2\xf2\xf8\xb3\x07-\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tprojectId\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:6\xfa\xf8\xb3\x07\x31\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\'\xc2\xf4\xb3\x07\n\n\x03\x63li\x12\x03gcp\xc2\xf4\xb3\x07\x13\n\x0cjson_gateway\x12\x03gcp\"\x9d\x04\n\x10GCPCertX509Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x36\n\x04\x63\x61ID\x18\x06 \x01(\tB(\xf2\xf8\xb3\x07#\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x19\xc2\xf4\xb3\x07\x14\n\x0cjson_gateway\x12\x04\x63\x61Id\x12\x43\n\x08\x63\x61PoolID\x18\x05 \x01(\tB1\xf2\xf8\xb3\x07,\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1d\xc2\xf4\xb3\x07\x18\n\x0cjson_gateway\x12\x08\x63\x61PoolId\x12[\n\x14issuedCertTTLMinutes\x18\x07 \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12\x43\n\x08location\x18\x04 \x01(\tB1\xf2\xf8\xb3\x07,\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1d\xc2\xf4\xb3\x07\x18\n\x0cjson_gateway\x12\x08location\x12\x45\n\tprojectID\x18\x03 \x01(\tB2\xf2\xf8\xb3\x07-\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tprojectId\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:F\xfa\xf8\xb3\x07\x41\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x37\xc2\xf4\xb3\x07\x12\n\x03\x63li\x12\x0bgcpCertX509\xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bgcpCertX509\"\xe2\x08\n\x12KeyfactorX509Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x44\n\x0c\x63\x61_file_path\x18\x06 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\ncaFilePath\x12[\n\x15\x63\x65rtificate_file_path\x18\x04 \x01(\tB<\xf2\xf8\xb3\x07\x37\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07(\xc2\xf4\xb3\x07#\n\x0cjson_gateway\x12\x13\x63\x65rtificateFilePath\x12t\n\"default_certificate_authority_name\x18\n \x01(\tBH\xf2\xf8\xb3\x07\x43\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x34\xc2\xf4\xb3\x07/\n\x0cjson_gateway\x12\x1f\x64\x65\x66\x61ultCertificateAuthorityName\x12p\n default_certificate_profile_name\x18\x08 \x01(\tBF\xf2\xf8\xb3\x07\x41\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x32\xc2\xf4\xb3\x07-\n\x0cjson_gateway\x12\x1d\x64\x65\x66\x61ultCertificateProfileName\x12m\n\x1f\x64\x65\x66\x61ult_end_entity_profile_name\x18\t \x01(\tBD\xf2\xf8\xb3\x07?\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x30\xc2\xf4\xb3\x07+\n\x0cjson_gateway\x12\x1b\x64\x65\x66\x61ultEndEntityProfileName\x12Y\n\x17\x65nrollment_code_env_var\x18\x0c \x01(\tB8\xf2\xf8\xb3\x07\x33\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14\x65nrollmentCodeEnvVar\x12\x61\n\x1b\x65nrollment_username_env_var\x18\x0b \x01(\tB<\xf2\xf8\xb3\x07\x37\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07-\xc2\xf4\xb3\x07(\n\x0cjson_gateway\x12\x18\x65nrollmentUsernameEnvVar\x12\x46\n\rkey_file_path\x18\x05 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bkeyFilePath\x12S\n\x14key_password_env_var\x18\x07 \x01(\tB5\xf2\xf8\xb3\x07\x30\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07&\xc2\xf4\xb3\x07!\n\x0cjson_gateway\x12\x11keyPasswordEnvVar\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:J\xfa\xf8\xb3\x07\x45\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07;\xc2\xf4\xb3\x07\x14\n\x03\x63li\x12\rkeyfactorX509\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rkeyfactorX509\"\xf2\x02\n\x11VaultAppRoleStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12\"\n\x04tags\x18\x08 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:p\xfa\xf8\xb3\x07k\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x61\xc2\xf4\xb3\x07\x13\n\x03\x63li\x12\x0cvaultAppRole\xc2\xf4\xb3\x07\x1c\n\x0cjson_gateway\x12\x0cvaultAppRole\xc2\xf4\xb3\x07#\n\x12terraform-provider\x12\rvault_approle\"\x8c\x05\n\x18VaultAppRoleCertSSHStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12[\n\x14issuedCertTTLMinutes\x18\t \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\x07 \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12O\n\x0fssh_mount_point\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rsshMountPoint\x12\"\n\x04tags\x18\x08 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\x88\x01\xfa\xf8\xb3\x07\x82\x01\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07x\xc2\xf4\xb3\x07\x1a\n\x03\x63li\x12\x13vaultAppRoleCertSSH\xc2\xf4\xb3\x07#\n\x0cjson_gateway\x12\x13vaultAppRoleCertSSH\xc2\xf4\xb3\x07,\n\x12terraform-provider\x12\x16vault_approle_cert_ssh\"\x90\x05\n\x19VaultAppRoleCertX509Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12[\n\x14issuedCertTTLMinutes\x18\t \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12O\n\x0fpki_mount_point\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rpkiMountPoint\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\x07 \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12\"\n\x04tags\x18\x08 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\x8b\x01\xfa\xf8\xb3\x07\x85\x01\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07{\xc2\xf4\xb3\x07\x1b\n\x03\x63li\x12\x14vaultAppRoleCertX509\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14vaultAppRoleCertX509\xc2\xf4\xb3\x07-\n\x12terraform-provider\x12\x17vault_approle_cert_x509\"\xcc\x04\n\rVaultTLSStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x44\n\x0c\x43\x41_cert_path\x18\x04 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\ncaCertPath\x12Q\n\x10\x63lient_cert_path\x18\x05 \x01(\tB7\xf2\xf8\xb3\x07\x32\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07#\xc2\xf4\xb3\x07\x1e\n\x0cjson_gateway\x12\x0e\x63lientCertPath\x12O\n\x0f\x63lient_key_path\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rclientKeyPath\x12@\n\tnamespace\x18\x08 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12\"\n\x04tags\x18\x07 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:d\xfa\xf8\xb3\x07_\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07U\xc2\xf4\xb3\x07\x0f\n\x03\x63li\x12\x08vaultTLS\xc2\xf4\xb3\x07\x18\n\x0cjson_gateway\x12\x08vaultTLS\xc2\xf4\xb3\x07\x1f\n\x12terraform-provider\x12\tvault_tls\"\xe4\x06\n\x14VaultTLSCertSSHStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x44\n\x0c\x43\x41_cert_path\x18\x04 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\ncaCertPath\x12Q\n\x10\x63lient_cert_path\x18\x05 \x01(\tB7\xf2\xf8\xb3\x07\x32\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07#\xc2\xf4\xb3\x07\x1e\n\x0cjson_gateway\x12\x0e\x63lientCertPath\x12O\n\x0f\x63lient_key_path\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rclientKeyPath\x12[\n\x14issuedCertTTLMinutes\x18\x0b \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x08 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\n \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12O\n\x0fssh_mount_point\x18\t \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rsshMountPoint\x12\"\n\x04tags\x18\x07 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:{\xfa\xf8\xb3\x07v\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07l\xc2\xf4\xb3\x07\x16\n\x03\x63li\x12\x0fvaultTLSCertSSH\xc2\xf4\xb3\x07\x1f\n\x0cjson_gateway\x12\x0fvaultTLSCertSSH\xc2\xf4\xb3\x07(\n\x12terraform-provider\x12\x12vault_tls_cert_ssh\"\xe8\x06\n\x15VaultTLSCertX509Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x44\n\x0c\x43\x41_cert_path\x18\x04 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\ncaCertPath\x12Q\n\x10\x63lient_cert_path\x18\x05 \x01(\tB7\xf2\xf8\xb3\x07\x32\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07#\xc2\xf4\xb3\x07\x1e\n\x0cjson_gateway\x12\x0e\x63lientCertPath\x12O\n\x0f\x63lient_key_path\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rclientKeyPath\x12[\n\x14issuedCertTTLMinutes\x18\x0b \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x08 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12O\n\x0fpki_mount_point\x18\t \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rpkiMountPoint\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\n \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12\"\n\x04tags\x18\x07 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:~\xfa\xf8\xb3\x07y\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07o\xc2\xf4\xb3\x07\x17\n\x03\x63li\x12\x10vaultTLSCertX509\xc2\xf4\xb3\x07 \n\x0cjson_gateway\x12\x10vaultTLSCertX509\xc2\xf4\xb3\x07)\n\x12terraform-provider\x12\x13vault_tls_cert_x509\"\xea\x02\n\x0fVaultTokenStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:j\xfa\xf8\xb3\x07\x65\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07[\xc2\xf4\xb3\x07\x11\n\x03\x63li\x12\nvaultToken\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\nvaultToken\xc2\xf4\xb3\x07!\n\x12terraform-provider\x12\x0bvault_token\"\x83\x05\n\x16VaultTokenCertSSHStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12[\n\x14issuedCertTTLMinutes\x18\t \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\x07 \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12O\n\x0fssh_mount_point\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rsshMountPoint\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\x81\x01\xfa\xf8\xb3\x07|\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07r\xc2\xf4\xb3\x07\x18\n\x03\x63li\x12\x11vaultTokenCertSSH\xc2\xf4\xb3\x07!\n\x0cjson_gateway\x12\x11vaultTokenCertSSH\xc2\xf4\xb3\x07*\n\x12terraform-provider\x12\x14vault_token_cert_ssh\"\x87\x05\n\x17VaultTokenCertX509Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12[\n\x14issuedCertTTLMinutes\x18\x08 \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12O\n\x0fpki_mount_point\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rpkiMountPoint\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\x07 \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\x84\x01\xfa\xf8\xb3\x07\x7f\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07u\xc2\xf4\xb3\x07\x19\n\x03\x63li\x12\x12vaultTokenCertX509\xc2\xf4\xb3\x07\"\n\x0cjson_gateway\x12\x12vaultTokenCertX509\xc2\xf4\xb3\x07+\n\x12terraform-provider\x12\x15vault_token_cert_x509Bm\n\x19\x63om.strongdm.api.plumbingB\x19SecretStoresTypesPlumbingZ5github.com/strongdm/strongdm-sdk-go/v3/internal/v1;v1b\x06proto3')
 
 
 
 _SECRETSTORE = DESCRIPTOR.message_types_by_name['SecretStore']
 _AWSSTORE = DESCRIPTOR.message_types_by_name['AWSStore']
 _AWSCERTX509STORE = DESCRIPTOR.message_types_by_name['AWSCertX509Store']
 _ACTIVEDIRECTORYSTORE = DESCRIPTOR.message_types_by_name['ActiveDirectoryStore']
 _AZURESTORE = DESCRIPTOR.message_types_by_name['AzureStore']
 _CYBERARKCONJURSTORE = DESCRIPTOR.message_types_by_name['CyberarkConjurStore']
 _CYBERARKPAMSTORE = DESCRIPTOR.message_types_by_name['CyberarkPAMStore']
 _CYBERARKPAMEXPERIMENTALSTORE = DESCRIPTOR.message_types_by_name['CyberarkPAMExperimentalStore']
 _DELINEASTORE = DESCRIPTOR.message_types_by_name['DelineaStore']
 _GCPSTORE = DESCRIPTOR.message_types_by_name['GCPStore']
 _GCPCERTX509STORE = DESCRIPTOR.message_types_by_name['GCPCertX509Store']
+_KEYFACTORX509STORE = DESCRIPTOR.message_types_by_name['KeyfactorX509Store']
 _VAULTAPPROLESTORE = DESCRIPTOR.message_types_by_name['VaultAppRoleStore']
 _VAULTAPPROLECERTSSHSTORE = DESCRIPTOR.message_types_by_name['VaultAppRoleCertSSHStore']
 _VAULTAPPROLECERTX509STORE = DESCRIPTOR.message_types_by_name['VaultAppRoleCertX509Store']
 _VAULTTLSSTORE = DESCRIPTOR.message_types_by_name['VaultTLSStore']
 _VAULTTLSCERTSSHSTORE = DESCRIPTOR.message_types_by_name['VaultTLSCertSSHStore']
 _VAULTTLSCERTX509STORE = DESCRIPTOR.message_types_by_name['VaultTLSCertX509Store']
 _VAULTTOKENSTORE = DESCRIPTOR.message_types_by_name['VaultTokenStore']
@@ -127,14 +128,21 @@
 GCPCertX509Store = _reflection.GeneratedProtocolMessageType('GCPCertX509Store', (_message.Message,), {
   'DESCRIPTOR' : _GCPCERTX509STORE,
   '__module__' : 'secret_store_types_pb2'
   # @@protoc_insertion_point(class_scope:v1.GCPCertX509Store)
   })
 _sym_db.RegisterMessage(GCPCertX509Store)
 
+KeyfactorX509Store = _reflection.GeneratedProtocolMessageType('KeyfactorX509Store', (_message.Message,), {
+  'DESCRIPTOR' : _KEYFACTORX509STORE,
+  '__module__' : 'secret_store_types_pb2'
+  # @@protoc_insertion_point(class_scope:v1.KeyfactorX509Store)
+  })
+_sym_db.RegisterMessage(KeyfactorX509Store)
+
 VaultAppRoleStore = _reflection.GeneratedProtocolMessageType('VaultAppRoleStore', (_message.Message,), {
   'DESCRIPTOR' : _VAULTAPPROLESTORE,
   '__module__' : 'secret_store_types_pb2'
   # @@protoc_insertion_point(class_scope:v1.VaultAppRoleStore)
   })
 _sym_db.RegisterMessage(VaultAppRoleStore)
 
@@ -216,14 +224,16 @@
   _SECRETSTORE.fields_by_name['cyberark_pam_experimental']._serialized_options = b'\362\370\263\0071\312\363\263\007,\302\364\263\007\'\n\014json_gateway\022\027cyberarkPAMExperimental\362\370\263\007\005\260\363\263\007\001'
   _SECRETSTORE.fields_by_name['delinea']._options = None
   _SECRETSTORE.fields_by_name['delinea']._serialized_options = b'\362\370\263\007!\312\363\263\007\034\302\364\263\007\027\n\014json_gateway\022\007delinea\362\370\263\007\005\260\363\263\007\001'
   _SECRETSTORE.fields_by_name['gcp']._options = None
   _SECRETSTORE.fields_by_name['gcp']._serialized_options = b'\362\370\263\007\035\312\363\263\007\030\302\364\263\007\023\n\014json_gateway\022\003gcp\362\370\263\007\005\260\363\263\007\001'
   _SECRETSTORE.fields_by_name['gcp_cert_x_509']._options = None
   _SECRETSTORE.fields_by_name['gcp_cert_x_509']._serialized_options = b'\362\370\263\007%\312\363\263\007 \302\364\263\007\033\n\014json_gateway\022\013gcpCertX509\362\370\263\007\005\260\363\263\007\001'
+  _SECRETSTORE.fields_by_name['keyfactor_x_509']._options = None
+  _SECRETSTORE.fields_by_name['keyfactor_x_509']._serialized_options = b'\362\370\263\007\'\312\363\263\007\"\302\364\263\007\035\n\014json_gateway\022\rkeyfactorX509\362\370\263\007\005\260\363\263\007\001'
   _SECRETSTORE.fields_by_name['vault_app_role']._options = None
   _SECRETSTORE.fields_by_name['vault_app_role']._serialized_options = b'\362\370\263\007&\312\363\263\007!\302\364\263\007\034\n\014json_gateway\022\014vaultAppRole\362\370\263\007\005\260\363\263\007\001'
   _SECRETSTORE.fields_by_name['vault_app_role_cert_ssh']._options = None
   _SECRETSTORE.fields_by_name['vault_app_role_cert_ssh']._serialized_options = b'\362\370\263\007-\312\363\263\007(\302\364\263\007#\n\014json_gateway\022\023vaultAppRoleCertSSH\362\370\263\007\005\260\363\263\007\001'
   _SECRETSTORE.fields_by_name['vault_app_role_cert_x_509']._options = None
   _SECRETSTORE.fields_by_name['vault_app_role_cert_x_509']._serialized_options = b'\362\370\263\007.\312\363\263\007)\302\364\263\007$\n\014json_gateway\022\024vaultAppRoleCertX509\362\370\263\007\005\260\363\263\007\001'
   _SECRETSTORE.fields_by_name['vault_tls']._options = None
@@ -354,14 +364,42 @@
   _GCPCERTX509STORE.fields_by_name['location']._serialized_options = b'\362\370\263\007,\260\363\263\007\001\300\363\263\007\001\312\363\263\007\035\302\364\263\007\030\n\014json_gateway\022\010location'
   _GCPCERTX509STORE.fields_by_name['projectID']._options = None
   _GCPCERTX509STORE.fields_by_name['projectID']._serialized_options = b'\362\370\263\007-\260\363\263\007\001\300\363\263\007\001\312\363\263\007\036\302\364\263\007\031\n\014json_gateway\022\tprojectId'
   _GCPCERTX509STORE.fields_by_name['tags']._options = None
   _GCPCERTX509STORE.fields_by_name['tags']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _GCPCERTX509STORE._options = None
   _GCPCERTX509STORE._serialized_options = b'\372\370\263\007A\250\363\263\007\001\312\363\263\0077\302\364\263\007\022\n\003cli\022\013gcpCertX509\302\364\263\007\033\n\014json_gateway\022\013gcpCertX509'
+  _KEYFACTORX509STORE.fields_by_name['id']._options = None
+  _KEYFACTORX509STORE.fields_by_name['id']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
+  _KEYFACTORX509STORE.fields_by_name['name']._options = None
+  _KEYFACTORX509STORE.fields_by_name['name']._serialized_options = b'\362\370\263\007\n\260\363\263\007\001\300\363\263\007\001'
+  _KEYFACTORX509STORE.fields_by_name['ca_file_path']._options = None
+  _KEYFACTORX509STORE.fields_by_name['ca_file_path']._serialized_options = b'\362\370\263\007)\260\363\263\007\001\312\363\263\007\037\302\364\263\007\032\n\014json_gateway\022\ncaFilePath'
+  _KEYFACTORX509STORE.fields_by_name['certificate_file_path']._options = None
+  _KEYFACTORX509STORE.fields_by_name['certificate_file_path']._serialized_options = b'\362\370\263\0077\260\363\263\007\001\300\363\263\007\001\312\363\263\007(\302\364\263\007#\n\014json_gateway\022\023certificateFilePath'
+  _KEYFACTORX509STORE.fields_by_name['default_certificate_authority_name']._options = None
+  _KEYFACTORX509STORE.fields_by_name['default_certificate_authority_name']._serialized_options = b'\362\370\263\007C\260\363\263\007\001\300\363\263\007\001\312\363\263\0074\302\364\263\007/\n\014json_gateway\022\037defaultCertificateAuthorityName'
+  _KEYFACTORX509STORE.fields_by_name['default_certificate_profile_name']._options = None
+  _KEYFACTORX509STORE.fields_by_name['default_certificate_profile_name']._serialized_options = b'\362\370\263\007A\260\363\263\007\001\300\363\263\007\001\312\363\263\0072\302\364\263\007-\n\014json_gateway\022\035defaultCertificateProfileName'
+  _KEYFACTORX509STORE.fields_by_name['default_end_entity_profile_name']._options = None
+  _KEYFACTORX509STORE.fields_by_name['default_end_entity_profile_name']._serialized_options = b'\362\370\263\007?\260\363\263\007\001\300\363\263\007\001\312\363\263\0070\302\364\263\007+\n\014json_gateway\022\033defaultEndEntityProfileName'
+  _KEYFACTORX509STORE.fields_by_name['enrollment_code_env_var']._options = None
+  _KEYFACTORX509STORE.fields_by_name['enrollment_code_env_var']._serialized_options = b'\362\370\263\0073\260\363\263\007\001\312\363\263\007)\302\364\263\007$\n\014json_gateway\022\024enrollmentCodeEnvVar'
+  _KEYFACTORX509STORE.fields_by_name['enrollment_username_env_var']._options = None
+  _KEYFACTORX509STORE.fields_by_name['enrollment_username_env_var']._serialized_options = b'\362\370\263\0077\260\363\263\007\001\312\363\263\007-\302\364\263\007(\n\014json_gateway\022\030enrollmentUsernameEnvVar'
+  _KEYFACTORX509STORE.fields_by_name['key_file_path']._options = None
+  _KEYFACTORX509STORE.fields_by_name['key_file_path']._serialized_options = b'\362\370\263\007*\260\363\263\007\001\312\363\263\007 \302\364\263\007\033\n\014json_gateway\022\013keyFilePath'
+  _KEYFACTORX509STORE.fields_by_name['key_password_env_var']._options = None
+  _KEYFACTORX509STORE.fields_by_name['key_password_env_var']._serialized_options = b'\362\370\263\0070\260\363\263\007\001\312\363\263\007&\302\364\263\007!\n\014json_gateway\022\021keyPasswordEnvVar'
+  _KEYFACTORX509STORE.fields_by_name['server_address']._options = None
+  _KEYFACTORX509STORE.fields_by_name['server_address']._serialized_options = b'\362\370\263\0071\260\363\263\007\001\300\363\263\007\001\312\363\263\007\"\302\364\263\007\035\n\014json_gateway\022\rserverAddress'
+  _KEYFACTORX509STORE.fields_by_name['tags']._options = None
+  _KEYFACTORX509STORE.fields_by_name['tags']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
+  _KEYFACTORX509STORE._options = None
+  _KEYFACTORX509STORE._serialized_options = b'\372\370\263\007E\250\363\263\007\001\312\363\263\007;\302\364\263\007\024\n\003cli\022\rkeyfactorX509\302\364\263\007\035\n\014json_gateway\022\rkeyfactorX509'
   _VAULTAPPROLESTORE.fields_by_name['id']._options = None
   _VAULTAPPROLESTORE.fields_by_name['id']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _VAULTAPPROLESTORE.fields_by_name['name']._options = None
   _VAULTAPPROLESTORE.fields_by_name['name']._serialized_options = b'\362\370\263\007\n\260\363\263\007\001\300\363\263\007\001'
   _VAULTAPPROLESTORE.fields_by_name['namespace']._options = None
   _VAULTAPPROLESTORE.fields_by_name['namespace']._serialized_options = b'\362\370\263\007(\260\363\263\007\001\312\363\263\007\036\302\364\263\007\031\n\014json_gateway\022\tnamespace'
   _VAULTAPPROLESTORE.fields_by_name['server_address']._options = None
@@ -517,47 +555,49 @@
   _VAULTTOKENCERTX509STORE.fields_by_name['signing_role']._options = None
   _VAULTTOKENCERTX509STORE.fields_by_name['signing_role']._serialized_options = b'\362\370\263\007/\260\363\263\007\001\300\363\263\007\001\312\363\263\007 \302\364\263\007\033\n\014json_gateway\022\013signingRole'
   _VAULTTOKENCERTX509STORE.fields_by_name['tags']._options = None
   _VAULTTOKENCERTX509STORE.fields_by_name['tags']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _VAULTTOKENCERTX509STORE._options = None
   _VAULTTOKENCERTX509STORE._serialized_options = b'\372\370\263\007\177\250\363\263\007\001\312\363\263\007u\302\364\263\007\031\n\003cli\022\022vaultTokenCertX509\302\364\263\007\"\n\014json_gateway\022\022vaultTokenCertX509\302\364\263\007+\n\022terraform-provider\022\025vault_token_cert_x509'
   _SECRETSTORE._serialized_start=60
-  _SECRETSTORE._serialized_end=2146
-  _AWSSTORE._serialized_start=2149
-  _AWSSTORE._serialized_end=2401
-  _AWSCERTX509STORE._serialized_start=2404
-  _AWSCERTX509STORE._serialized_end=3018
-  _ACTIVEDIRECTORYSTORE._serialized_start=3021
-  _ACTIVEDIRECTORYSTORE._serialized_end=3296
-  _AZURESTORE._serialized_start=3299
-  _AZURESTORE._serialized_end=3534
-  _CYBERARKCONJURSTORE._serialized_start=3537
-  _CYBERARKCONJURSTORE._serialized_end=3836
-  _CYBERARKPAMSTORE._serialized_start=3839
-  _CYBERARKPAMSTORE._serialized_end=4126
-  _CYBERARKPAMEXPERIMENTALSTORE._serialized_start=4129
-  _CYBERARKPAMEXPERIMENTALSTORE._serialized_end=4473
-  _DELINEASTORE._serialized_start=4476
-  _DELINEASTORE._serialized_end=4783
-  _GCPSTORE._serialized_start=4786
-  _GCPSTORE._serialized_end=5016
-  _GCPCERTX509STORE._serialized_start=5019
-  _GCPCERTX509STORE._serialized_end=5560
-  _VAULTAPPROLESTORE._serialized_start=5563
-  _VAULTAPPROLESTORE._serialized_end=5933
-  _VAULTAPPROLECERTSSHSTORE._serialized_start=5936
-  _VAULTAPPROLECERTSSHSTORE._serialized_end=6588
-  _VAULTAPPROLECERTX509STORE._serialized_start=6591
-  _VAULTAPPROLECERTX509STORE._serialized_end=7247
-  _VAULTTLSSTORE._serialized_start=7250
-  _VAULTTLSSTORE._serialized_end=7838
-  _VAULTTLSCERTSSHSTORE._serialized_start=7841
-  _VAULTTLSCERTSSHSTORE._serialized_end=8709
-  _VAULTTLSCERTX509STORE._serialized_start=8712
-  _VAULTTLSCERTX509STORE._serialized_end=9584
-  _VAULTTOKENSTORE._serialized_start=9587
-  _VAULTTOKENSTORE._serialized_end=9949
-  _VAULTTOKENCERTSSHSTORE._serialized_start=9952
-  _VAULTTOKENCERTSSHSTORE._serialized_end=10595
-  _VAULTTOKENCERTX509STORE._serialized_start=10598
-  _VAULTTOKENCERTX509STORE._serialized_end=11245
+  _SECRETSTORE._serialized_end=2254
+  _AWSSTORE._serialized_start=2257
+  _AWSSTORE._serialized_end=2509
+  _AWSCERTX509STORE._serialized_start=2512
+  _AWSCERTX509STORE._serialized_end=3126
+  _ACTIVEDIRECTORYSTORE._serialized_start=3129
+  _ACTIVEDIRECTORYSTORE._serialized_end=3404
+  _AZURESTORE._serialized_start=3407
+  _AZURESTORE._serialized_end=3642
+  _CYBERARKCONJURSTORE._serialized_start=3645
+  _CYBERARKCONJURSTORE._serialized_end=3944
+  _CYBERARKPAMSTORE._serialized_start=3947
+  _CYBERARKPAMSTORE._serialized_end=4234
+  _CYBERARKPAMEXPERIMENTALSTORE._serialized_start=4237
+  _CYBERARKPAMEXPERIMENTALSTORE._serialized_end=4581
+  _DELINEASTORE._serialized_start=4584
+  _DELINEASTORE._serialized_end=4891
+  _GCPSTORE._serialized_start=4894
+  _GCPSTORE._serialized_end=5124
+  _GCPCERTX509STORE._serialized_start=5127
+  _GCPCERTX509STORE._serialized_end=5668
+  _KEYFACTORX509STORE._serialized_start=5671
+  _KEYFACTORX509STORE._serialized_end=6793
+  _VAULTAPPROLESTORE._serialized_start=6796
+  _VAULTAPPROLESTORE._serialized_end=7166
+  _VAULTAPPROLECERTSSHSTORE._serialized_start=7169
+  _VAULTAPPROLECERTSSHSTORE._serialized_end=7821
+  _VAULTAPPROLECERTX509STORE._serialized_start=7824
+  _VAULTAPPROLECERTX509STORE._serialized_end=8480
+  _VAULTTLSSTORE._serialized_start=8483
+  _VAULTTLSSTORE._serialized_end=9071
+  _VAULTTLSCERTSSHSTORE._serialized_start=9074
+  _VAULTTLSCERTSSHSTORE._serialized_end=9942
+  _VAULTTLSCERTX509STORE._serialized_start=9945
+  _VAULTTLSCERTX509STORE._serialized_end=10817
+  _VAULTTOKENSTORE._serialized_start=10820
+  _VAULTTOKENSTORE._serialized_end=11182
+  _VAULTTOKENCERTSSHSTORE._serialized_start=11185
+  _VAULTTOKENCERTSSHSTORE._serialized_end=11828
+  _VAULTTOKENCERTX509STORE._serialized_start=11831
+  _VAULTTOKENCERTX509STORE._serialized_end=12478
 # @@protoc_insertion_point(module_scope)
```

## Comparing `strongdm-8.0.0/strongdm/account_permissions_pb2.py` & `strongdm-8.1.0/strongdm/account_permissions_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/account_resources_history_pb2_grpc.py` & `strongdm-8.1.0/strongdm/account_resources_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/spec_pb2.py` & `strongdm-8.1.0/strongdm/spec_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/errors.py` & `strongdm-8.1.0/strongdm/errors.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/approval_workflow_approvers_history_pb2_grpc.py` & `strongdm-8.1.0/strongdm/approval_workflow_approvers_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/workflow_roles_history_pb2.py` & `strongdm-8.1.0/strongdm/workflow_roles_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/resources_pb2.py` & `strongdm-8.1.0/strongdm/resources_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/control_panel_pb2.py` & `strongdm-8.1.0/strongdm/control_panel_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/models.py` & `strongdm-8.1.0/strongdm/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -10489,14 +10489,165 @@
             secret_store_id=d.get('secret_store_id'),
             subdomain=d.get('subdomain'),
             tags=d.get('tags'),
             url=d.get('url'),
         )
 
 
+class KeyfactorX509Store:
+    __slots__ = [
+        'ca_file_path',
+        'certificate_file_path',
+        'default_certificate_authority_name',
+        'default_certificate_profile_name',
+        'default_end_entity_profile_name',
+        'enrollment_code_env_var',
+        'enrollment_username_env_var',
+        'id',
+        'key_file_path',
+        'key_password_env_var',
+        'name',
+        'server_address',
+        'tags',
+    ]
+
+    def __init__(
+        self,
+        ca_file_path=None,
+        certificate_file_path=None,
+        default_certificate_authority_name=None,
+        default_certificate_profile_name=None,
+        default_end_entity_profile_name=None,
+        enrollment_code_env_var=None,
+        enrollment_username_env_var=None,
+        id=None,
+        key_file_path=None,
+        key_password_env_var=None,
+        name=None,
+        server_address=None,
+        tags=None,
+    ):
+        self.ca_file_path = ca_file_path if ca_file_path is not None else ''
+        '''
+         Path to the root CA that signed the certificate passed to the client for HTTPS connection.
+         This is not required if the CA is trusted by the host operating system. This should be a PEM
+         formatted certificate, and doesn't necessarily have to be the CA that signed CertificateFile.
+        '''
+        self.certificate_file_path = certificate_file_path if certificate_file_path is not None else ''
+        '''
+         Path to client certificate in PEM format. This certificate must contain a client certificate that
+         is recognized by the EJBCA instance represented by Hostname. This PEM file may also contain the private
+         key associated with the certificate, but KeyFile can also be set to configure the private key.
+        '''
+        self.default_certificate_authority_name = default_certificate_authority_name if default_certificate_authority_name is not None else ''
+        '''
+         Name of EJBCA certificate authority that will enroll CSR.
+        '''
+        self.default_certificate_profile_name = default_certificate_profile_name if default_certificate_profile_name is not None else ''
+        '''
+         Certificate profile name that EJBCA will enroll the CSR with.
+        '''
+        self.default_end_entity_profile_name = default_end_entity_profile_name if default_end_entity_profile_name is not None else ''
+        '''
+         End entity profile that EJBCA will enroll the CSR with.
+        '''
+        self.enrollment_code_env_var = enrollment_code_env_var if enrollment_code_env_var is not None else ''
+        '''
+         code used by EJBCA during enrollment. May be left blank if no code is required.
+        '''
+        self.enrollment_username_env_var = enrollment_username_env_var if enrollment_username_env_var is not None else ''
+        '''
+         username that used by the EJBCA during enrollment. This can be left out. 
+         If so, the username must be auto-generated on the Keyfactor side.
+        '''
+        self.id = id if id is not None else ''
+        '''
+         Unique identifier of the SecretStore.
+        '''
+        self.key_file_path = key_file_path if key_file_path is not None else ''
+        '''
+         Path to private key in PEM format. This file should contain the private key associated with the
+         client certificate configured in CertificateFile.
+        '''
+        self.key_password_env_var = key_password_env_var if key_password_env_var is not None else ''
+        '''
+         optional environment variable housing the password that is used to decrypt the key file.
+        '''
+        self.name = name if name is not None else ''
+        '''
+         Unique human-readable name of the SecretStore.
+        '''
+        self.server_address = server_address if server_address is not None else ''
+        '''
+         the host of the Key Factor CA
+        '''
+        self.tags = tags if tags is not None else _porcelain_zero_value_tags()
+        '''
+         Tags is a map of key, value pairs.
+        '''
+
+    def __repr__(self):
+        return '<sdm.KeyfactorX509Store ' + \
+            'ca_file_path: ' + repr(self.ca_file_path) + ' ' +\
+            'certificate_file_path: ' + repr(self.certificate_file_path) + ' ' +\
+            'default_certificate_authority_name: ' + repr(self.default_certificate_authority_name) + ' ' +\
+            'default_certificate_profile_name: ' + repr(self.default_certificate_profile_name) + ' ' +\
+            'default_end_entity_profile_name: ' + repr(self.default_end_entity_profile_name) + ' ' +\
+            'enrollment_code_env_var: ' + repr(self.enrollment_code_env_var) + ' ' +\
+            'enrollment_username_env_var: ' + repr(self.enrollment_username_env_var) + ' ' +\
+            'id: ' + repr(self.id) + ' ' +\
+            'key_file_path: ' + repr(self.key_file_path) + ' ' +\
+            'key_password_env_var: ' + repr(self.key_password_env_var) + ' ' +\
+            'name: ' + repr(self.name) + ' ' +\
+            'server_address: ' + repr(self.server_address) + ' ' +\
+            'tags: ' + repr(self.tags) + ' ' +\
+            '>'
+
+    def to_dict(self):
+        return {
+            'ca_file_path': self.ca_file_path,
+            'certificate_file_path': self.certificate_file_path,
+            'default_certificate_authority_name':
+            self.default_certificate_authority_name,
+            'default_certificate_profile_name':
+            self.default_certificate_profile_name,
+            'default_end_entity_profile_name':
+            self.default_end_entity_profile_name,
+            'enrollment_code_env_var': self.enrollment_code_env_var,
+            'enrollment_username_env_var': self.enrollment_username_env_var,
+            'id': self.id,
+            'key_file_path': self.key_file_path,
+            'key_password_env_var': self.key_password_env_var,
+            'name': self.name,
+            'server_address': self.server_address,
+            'tags': self.tags,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            ca_file_path=d.get('ca_file_path'),
+            certificate_file_path=d.get('certificate_file_path'),
+            default_certificate_authority_name=d.get(
+                'default_certificate_authority_name'),
+            default_certificate_profile_name=d.get(
+                'default_certificate_profile_name'),
+            default_end_entity_profile_name=d.get(
+                'default_end_entity_profile_name'),
+            enrollment_code_env_var=d.get('enrollment_code_env_var'),
+            enrollment_username_env_var=d.get('enrollment_username_env_var'),
+            id=d.get('id'),
+            key_file_path=d.get('key_file_path'),
+            key_password_env_var=d.get('key_password_env_var'),
+            name=d.get('name'),
+            server_address=d.get('server_address'),
+            tags=d.get('tags'),
+        )
+
+
 class Kubernetes:
     __slots__ = [
         'bind_interface',
         'certificate_authority',
         'client_certificate',
         'client_key',
         'egress_filter',
```

## Comparing `strongdm-8.0.0/strongdm/secret_store_healths_pb2.py` & `strongdm-8.1.0/strongdm/secret_store_healths_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/accounts_history_pb2.py` & `strongdm-8.1.0/strongdm/accounts_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/roles_pb2_grpc.py` & `strongdm-8.1.0/strongdm/roles_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/workflows_history_pb2.py` & `strongdm-8.1.0/strongdm/workflows_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/approval_workflows_pb2.py` & `strongdm-8.1.0/strongdm/approval_workflows_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/peering_group_nodes_pb2.py` & `strongdm-8.1.0/strongdm/peering_group_nodes_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/workflow_assignments_history_pb2_grpc.py` & `strongdm-8.1.0/strongdm/workflow_assignments_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/approval_workflow_steps_history_pb2.py` & `strongdm-8.1.0/strongdm/approval_workflow_steps_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/workflow_approvers_pb2_grpc.py` & `strongdm-8.1.0/strongdm/workflow_approvers_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/remote_identities_pb2.py` & `strongdm-8.1.0/strongdm/remote_identities_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/workflow_approvers_history_pb2.py` & `strongdm-8.1.0/strongdm/workflow_approvers_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/resources_history_pb2.py` & `strongdm-8.1.0/strongdm/resources_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/roles_history_pb2.py` & `strongdm-8.1.0/strongdm/roles_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/remote_identity_groups_pb2.py` & `strongdm-8.1.0/strongdm/remote_identity_groups_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm/workflow_roles_pb2_grpc.py` & `strongdm-8.1.0/strongdm/workflow_roles_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.0.0/strongdm.egg-info/PKG-INFO` & `strongdm-8.1.0/strongdm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: strongdm
-Version: 8.0.0
+Version: 8.1.0
 Summary: strongDM SDK for the Python programming language.
 Home-page: https://github.com/strongdm/strongdm-sdk-python
 Author: strongDM Team
 Author-email: sdk-feedback@strongdm.com
 License: apache-2.0
-Download-URL: https://github.com/strongdm/strongdm-sdk-python/archive/v8.0.0.tar.gz
+Download-URL: https://github.com/strongdm/strongdm-sdk-python/archive/v8.1.0.tar.gz
 Keywords: strongDM,sdm,api,automation,security,audit,database,server,ssh,rdp
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `strongdm-8.0.0/strongdm.egg-info/SOURCES.txt` & `strongdm-8.1.0/strongdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

