# Comparing `tmp/asana-5.0.5.tar.gz` & `tmp/asana-5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/python-asana/python-asana/dist/.tmp-8yq0cjl2/asana-5.0.5.tar", last modified: Thu Mar 14 22:41:24 2024, max compression
+gzip compressed data, was "/home/runner/work/python-asana/python-asana/dist/.tmp-w9a3_8_v/asana-5.0.6.tar", last modified: Mon Mar 25 20:42:54 2024, max compression
```

## Comparing `asana-5.0.5.tar` & `asana-5.0.6.tar`

### file list

```diff
@@ -1,102 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:41:24.000000 asana-5.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 22:41:20.000000 asana-5.0.5/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 22:41:20.000000 asana-5.0.5/CONTRIBUTORS
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-14 22:41:20.000000 asana-5.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-14 22:41:20.000000 asana-5.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    59705 2024-03-14 22:41:24.000000 asana-5.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    59476 2024-03-14 22:41:20.000000 asana-5.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:41:24.000000 asana-5.0.5/asana/
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-03-14 22:41:20.000000 asana-5.0.5/asana/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:41:24.000000 asana-5.0.5/asana/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32257 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/attachments_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13883 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/audit_log_api_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/batch_api_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17497 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/custom_field_settings_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    59844 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/custom_fields_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9752 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/events_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    37156 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/goal_relationships_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    70089 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/goals_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27422 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14415 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/organization_exports_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23701 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/portfolio_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    84970 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/portfolios_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    28082 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/project_briefs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15697 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/project_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    29266 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/project_statuses_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    37358 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/project_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   139864 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/projects_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/rules_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    48787 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/sections_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    28774 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/status_updates_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    35054 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/stories_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    56629 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/tags_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27983 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/task_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   209249 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/tasks_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    31303 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/team_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    49884 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/teams_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15100 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/time_periods_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    37107 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/time_tracking_entries_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/typeahead_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/user_task_lists_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    39046 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    38367 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/webhooks_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23817 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/workspace_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    36352 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api/workspaces_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25258 2024-03-14 22:41:20.000000 asana-5.0.5/asana/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-03-14 22:41:20.000000 asana-5.0.5/asana/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:41:24.000000 asana-5.0.5/asana/pagination/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-14 22:41:20.000000 asana-5.0.5/asana/pagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-03-14 22:41:20.000000 asana-5.0.5/asana/pagination/event_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-03-14 22:41:20.000000 asana-5.0.5/asana/pagination/page_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13136 2024-03-14 22:41:20.000000 asana-5.0.5/asana/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:41:24.000000 asana-5.0.5/asana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    59705 2024-03-14 22:41:24.000000 asana-5.0.5/asana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-03-14 22:41:24.000000 asana-5.0.5/asana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 22:41:24.000000 asana-5.0.5/asana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-14 22:41:24.000000 asana-5.0.5/asana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-14 22:41:24.000000 asana-5.0.5/asana.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:41:24.000000 asana-5.0.5/build_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 22:41:20.000000 asana-5.0.5/build_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8834 2024-03-14 22:41:20.000000 asana-5.0.5/build_tests/test_projects_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-03-14 22:41:20.000000 asana-5.0.5/build_tests/test_tasks_api.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 22:41:24.000000 asana-5.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-03-14 22:41:20.000000 asana-5.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:41:24.000000 asana-5.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-14 22:41:20.000000 asana-5.0.5/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_attachments_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_audit_log_api_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_batch_api_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_custom_field_settings_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_custom_fields_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_events_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_goal_relationships_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_goals_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_organization_exports_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_portfolio_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_portfolios_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_project_briefs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_project_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_project_statuses_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_project_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_projects_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_rules_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_sections_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_status_updates_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_stories_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_task_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_tasks_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_team_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_teams_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_time_periods_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_time_tracking_entries_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_typeahead_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_user_task_lists_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_users_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_webhooks_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_workspace_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-14 22:41:20.000000 asana-5.0.5/test/test_workspaces_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:42:54.000000 asana-5.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 20:42:46.000000 asana-5.0.6/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 20:42:46.000000 asana-5.0.6/CONTRIBUTORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-25 20:42:46.000000 asana-5.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-25 20:42:46.000000 asana-5.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    60853 2024-03-25 20:42:54.000000 asana-5.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    60624 2024-03-25 20:42:46.000000 asana-5.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:42:54.000000 asana-5.0.6/asana/
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-03-25 20:42:46.000000 asana-5.0.6/asana/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:42:54.000000 asana-5.0.6/asana/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34861 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/allocations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32257 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/attachments_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13883 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/audit_log_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/batch_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17497 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/custom_field_settings_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59844 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/custom_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9752 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/events_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37156 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/goal_relationships_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70089 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/goals_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34125 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14415 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/organization_exports_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23701 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/portfolio_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84970 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/portfolios_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28082 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/project_briefs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15697 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/project_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29266 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/project_statuses_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37358 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/project_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   139864 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/rules_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48787 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/sections_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28774 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/status_updates_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35054 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/stories_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56629 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27983 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/task_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   209249 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/tasks_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31303 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/team_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49884 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15100 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/time_periods_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37107 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/time_tracking_entries_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/typeahead_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/user_task_lists_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39046 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38367 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/webhooks_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23817 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/workspace_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36352 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api/workspaces_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25258 2024-03-25 20:42:46.000000 asana-5.0.6/asana/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-03-25 20:42:46.000000 asana-5.0.6/asana/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:42:54.000000 asana-5.0.6/asana/pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-25 20:42:46.000000 asana-5.0.6/asana/pagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-03-25 20:42:46.000000 asana-5.0.6/asana/pagination/event_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-03-25 20:42:46.000000 asana-5.0.6/asana/pagination/page_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13136 2024-03-25 20:42:46.000000 asana-5.0.6/asana/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:42:54.000000 asana-5.0.6/asana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    60853 2024-03-25 20:42:54.000000 asana-5.0.6/asana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-03-25 20:42:54.000000 asana-5.0.6/asana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 20:42:54.000000 asana-5.0.6/asana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-25 20:42:54.000000 asana-5.0.6/asana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-25 20:42:54.000000 asana-5.0.6/asana.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:42:54.000000 asana-5.0.6/build_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 20:42:46.000000 asana-5.0.6/build_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8834 2024-03-25 20:42:46.000000 asana-5.0.6/build_tests/test_projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-03-25 20:42:46.000000 asana-5.0.6/build_tests/test_tasks_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 20:42:54.000000 asana-5.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-03-25 20:42:46.000000 asana-5.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:42:54.000000 asana-5.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-25 20:42:46.000000 asana-5.0.6/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_allocations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_attachments_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_audit_log_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_batch_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_custom_field_settings_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_custom_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_events_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_goal_relationships_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_goals_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_organization_exports_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_portfolio_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_portfolios_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_project_briefs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_project_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_project_statuses_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_project_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_rules_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_sections_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_status_updates_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_stories_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_task_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_tasks_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_team_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_time_periods_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_time_tracking_entries_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_typeahead_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_user_task_lists_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_webhooks_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_workspace_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-25 20:42:46.000000 asana-5.0.6/test/test_workspaces_api.py
```

### Comparing `asana-5.0.5/LICENSE` & `asana-5.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/PKG-INFO` & `asana-5.0.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,11 @@
-Metadata-Version: 2.1
-Name: asana
-Version: 5.0.5
-Summary: Asana
-Home-page: http://github.com/asana/python-asana
-Author: Asana, Inc
-License: MIT
-Keywords: asana,Asana
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # asana [![GitHub release][release-image]]() [![PyPi Version][pypi-image]][pypi-url]
 
 - API version: 1.0
-- Package version: 5.0.5
+- Package version: 5.0.6
 
 ## Requirements.
 
 Python 3.4+
 
 ## Installation & Usage
 ### pip install from [PyPI](https://pypi.org/project/asana/)
@@ -185,199 +174,205 @@
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://app.asana.com/api/1.0*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
-*AttachmentsApi* | [**create_attachment_for_object**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/AttachmentsApi.md#create_attachment_for_object) | **POST** /attachments | Upload an attachment
-*AttachmentsApi* | [**delete_attachment**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/AttachmentsApi.md#delete_attachment) | **DELETE** /attachments/{attachment_gid} | Delete an attachment
-*AttachmentsApi* | [**get_attachment**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/AttachmentsApi.md#get_attachment) | **GET** /attachments/{attachment_gid} | Get an attachment
-*AttachmentsApi* | [**get_attachments_for_object**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/AttachmentsApi.md#get_attachments_for_object) | **GET** /attachments | Get attachments from an object
-*AuditLogAPIApi* | [**get_audit_log_events**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/AuditLogAPIApi.md#get_audit_log_events) | **GET** /workspaces/{workspace_gid}/audit_log_events | Get audit log events
-*BatchAPIApi* | [**create_batch_request**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/BatchAPIApi.md#create_batch_request) | **POST** /batch | Submit parallel requests
-*CustomFieldSettingsApi* | [**get_custom_field_settings_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldSettingsApi.md#get_custom_field_settings_for_portfolio) | **GET** /portfolios/{portfolio_gid}/custom_field_settings | Get a portfolio&#x27;s custom fields
-*CustomFieldSettingsApi* | [**get_custom_field_settings_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldSettingsApi.md#get_custom_field_settings_for_project) | **GET** /projects/{project_gid}/custom_field_settings | Get a project&#x27;s custom fields
-*CustomFieldsApi* | [**create_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#create_custom_field) | **POST** /custom_fields | Create a custom field
-*CustomFieldsApi* | [**create_enum_option_for_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#create_enum_option_for_custom_field) | **POST** /custom_fields/{custom_field_gid}/enum_options | Create an enum option
-*CustomFieldsApi* | [**delete_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#delete_custom_field) | **DELETE** /custom_fields/{custom_field_gid} | Delete a custom field
-*CustomFieldsApi* | [**get_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#get_custom_field) | **GET** /custom_fields/{custom_field_gid} | Get a custom field
-*CustomFieldsApi* | [**get_custom_fields_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#get_custom_fields_for_workspace) | **GET** /workspaces/{workspace_gid}/custom_fields | Get a workspace&#x27;s custom fields
-*CustomFieldsApi* | [**insert_enum_option_for_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#insert_enum_option_for_custom_field) | **POST** /custom_fields/{custom_field_gid}/enum_options/insert | Reorder a custom field&#x27;s enum
-*CustomFieldsApi* | [**update_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#update_custom_field) | **PUT** /custom_fields/{custom_field_gid} | Update a custom field
-*CustomFieldsApi* | [**update_enum_option**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#update_enum_option) | **PUT** /enum_options/{enum_option_gid} | Update an enum option
-*EventsApi* | [**get_events**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/EventsApi.md#get_events) | **GET** /events | Get events on a resource
-*GoalRelationshipsApi* | [**add_supporting_relationship**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalRelationshipsApi.md#add_supporting_relationship) | **POST** /goals/{goal_gid}/addSupportingRelationship | Add a supporting goal relationship
-*GoalRelationshipsApi* | [**get_goal_relationship**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalRelationshipsApi.md#get_goal_relationship) | **GET** /goal_relationships/{goal_relationship_gid} | Get a goal relationship
-*GoalRelationshipsApi* | [**get_goal_relationships**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalRelationshipsApi.md#get_goal_relationships) | **GET** /goal_relationships | Get goal relationships
-*GoalRelationshipsApi* | [**remove_supporting_relationship**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalRelationshipsApi.md#remove_supporting_relationship) | **POST** /goals/{goal_gid}/removeSupportingRelationship | Removes a supporting goal relationship
-*GoalRelationshipsApi* | [**update_goal_relationship**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalRelationshipsApi.md#update_goal_relationship) | **PUT** /goal_relationships/{goal_relationship_gid} | Update a goal relationship
-*GoalsApi* | [**add_followers**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#add_followers) | **POST** /goals/{goal_gid}/addFollowers | Add a collaborator to a goal
-*GoalsApi* | [**create_goal**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#create_goal) | **POST** /goals | Create a goal
-*GoalsApi* | [**create_goal_metric**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#create_goal_metric) | **POST** /goals/{goal_gid}/setMetric | Create a goal metric
-*GoalsApi* | [**delete_goal**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#delete_goal) | **DELETE** /goals/{goal_gid} | Delete a goal
-*GoalsApi* | [**get_goal**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#get_goal) | **GET** /goals/{goal_gid} | Get a goal
-*GoalsApi* | [**get_goals**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#get_goals) | **GET** /goals | Get goals
-*GoalsApi* | [**get_parent_goals_for_goal**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#get_parent_goals_for_goal) | **GET** /goals/{goal_gid}/parentGoals | Get parent goals from a goal
-*GoalsApi* | [**remove_followers**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#remove_followers) | **POST** /goals/{goal_gid}/removeFollowers | Remove a collaborator from a goal
-*GoalsApi* | [**update_goal**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#update_goal) | **PUT** /goals/{goal_gid} | Update a goal
-*GoalsApi* | [**update_goal_metric**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#update_goal_metric) | **POST** /goals/{goal_gid}/setMetricCurrentValue | Update a goal metric
-*JobsApi* | [**get_job**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/JobsApi.md#get_job) | **GET** /jobs/{job_gid} | Get a job by id
-*MembershipsApi* | [**create_membership**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/MembershipsApi.md#create_membership) | **POST** /memberships | Create a membership
-*MembershipsApi* | [**delete_membership**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/MembershipsApi.md#delete_membership) | **DELETE** /memberships/{membership_gid} | Delete a membership
-*MembershipsApi* | [**get_membership**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/MembershipsApi.md#get_membership) | **GET** /memberships/{membership_gid} | Get a membership
-*MembershipsApi* | [**get_memberships**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/MembershipsApi.md#get_memberships) | **GET** /memberships | Get multiple memberships
-*OrganizationExportsApi* | [**create_organization_export**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/OrganizationExportsApi.md#create_organization_export) | **POST** /organization_exports | Create an organization export request
-*OrganizationExportsApi* | [**get_organization_export**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/OrganizationExportsApi.md#get_organization_export) | **GET** /organization_exports/{organization_export_gid} | Get details on an org export request
-*PortfolioMembershipsApi* | [**get_portfolio_membership**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfolioMembershipsApi.md#get_portfolio_membership) | **GET** /portfolio_memberships/{portfolio_membership_gid} | Get a portfolio membership
-*PortfolioMembershipsApi* | [**get_portfolio_memberships**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfolioMembershipsApi.md#get_portfolio_memberships) | **GET** /portfolio_memberships | Get multiple portfolio memberships
-*PortfolioMembershipsApi* | [**get_portfolio_memberships_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfolioMembershipsApi.md#get_portfolio_memberships_for_portfolio) | **GET** /portfolios/{portfolio_gid}/portfolio_memberships | Get memberships from a portfolio
-*PortfoliosApi* | [**add_custom_field_setting_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#add_custom_field_setting_for_portfolio) | **POST** /portfolios/{portfolio_gid}/addCustomFieldSetting | Add a custom field to a portfolio
-*PortfoliosApi* | [**add_item_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#add_item_for_portfolio) | **POST** /portfolios/{portfolio_gid}/addItem | Add a portfolio item
-*PortfoliosApi* | [**add_members_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#add_members_for_portfolio) | **POST** /portfolios/{portfolio_gid}/addMembers | Add users to a portfolio
-*PortfoliosApi* | [**create_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#create_portfolio) | **POST** /portfolios | Create a portfolio
-*PortfoliosApi* | [**delete_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#delete_portfolio) | **DELETE** /portfolios/{portfolio_gid} | Delete a portfolio
-*PortfoliosApi* | [**get_items_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#get_items_for_portfolio) | **GET** /portfolios/{portfolio_gid}/items | Get portfolio items
-*PortfoliosApi* | [**get_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#get_portfolio) | **GET** /portfolios/{portfolio_gid} | Get a portfolio
-*PortfoliosApi* | [**get_portfolios**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#get_portfolios) | **GET** /portfolios | Get multiple portfolios
-*PortfoliosApi* | [**remove_custom_field_setting_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#remove_custom_field_setting_for_portfolio) | **POST** /portfolios/{portfolio_gid}/removeCustomFieldSetting | Remove a custom field from a portfolio
-*PortfoliosApi* | [**remove_item_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#remove_item_for_portfolio) | **POST** /portfolios/{portfolio_gid}/removeItem | Remove a portfolio item
-*PortfoliosApi* | [**remove_members_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#remove_members_for_portfolio) | **POST** /portfolios/{portfolio_gid}/removeMembers | Remove users from a portfolio
-*PortfoliosApi* | [**update_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#update_portfolio) | **PUT** /portfolios/{portfolio_gid} | Update a portfolio
-*ProjectBriefsApi* | [**create_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectBriefsApi.md#create_project_brief) | **POST** /projects/{project_gid}/project_briefs | Create a project brief
-*ProjectBriefsApi* | [**delete_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectBriefsApi.md#delete_project_brief) | **DELETE** /project_briefs/{project_brief_gid} | Delete a project brief
-*ProjectBriefsApi* | [**get_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectBriefsApi.md#get_project_brief) | **GET** /project_briefs/{project_brief_gid} | Get a project brief
-*ProjectBriefsApi* | [**update_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectBriefsApi.md#update_project_brief) | **PUT** /project_briefs/{project_brief_gid} | Update a project brief
-*ProjectMembershipsApi* | [**get_project_membership**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectMembershipsApi.md#get_project_membership) | **GET** /project_memberships/{project_membership_gid} | Get a project membership
-*ProjectMembershipsApi* | [**get_project_memberships_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectMembershipsApi.md#get_project_memberships_for_project) | **GET** /projects/{project_gid}/project_memberships | Get memberships from a project
-*ProjectStatusesApi* | [**create_project_status_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectStatusesApi.md#create_project_status_for_project) | **POST** /projects/{project_gid}/project_statuses | Create a project status
-*ProjectStatusesApi* | [**delete_project_status**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectStatusesApi.md#delete_project_status) | **DELETE** /project_statuses/{project_status_gid} | Delete a project status
-*ProjectStatusesApi* | [**get_project_status**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectStatusesApi.md#get_project_status) | **GET** /project_statuses/{project_status_gid} | Get a project status
-*ProjectStatusesApi* | [**get_project_statuses_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectStatusesApi.md#get_project_statuses_for_project) | **GET** /projects/{project_gid}/project_statuses | Get statuses from a project
-*ProjectTemplatesApi* | [**delete_project_template**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectTemplatesApi.md#delete_project_template) | **DELETE** /project_templates/{project_template_gid} | Delete a project template
-*ProjectTemplatesApi* | [**get_project_template**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectTemplatesApi.md#get_project_template) | **GET** /project_templates/{project_template_gid} | Get a project template
-*ProjectTemplatesApi* | [**get_project_templates**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectTemplatesApi.md#get_project_templates) | **GET** /project_templates | Get multiple project templates
-*ProjectTemplatesApi* | [**get_project_templates_for_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectTemplatesApi.md#get_project_templates_for_team) | **GET** /teams/{team_gid}/project_templates | Get a team&#x27;s project templates
-*ProjectTemplatesApi* | [**instantiate_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectTemplatesApi.md#instantiate_project) | **POST** /project_templates/{project_template_gid}/instantiateProject | Instantiate a project from a project template
-*ProjectsApi* | [**add_custom_field_setting_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#add_custom_field_setting_for_project) | **POST** /projects/{project_gid}/addCustomFieldSetting | Add a custom field to a project
-*ProjectsApi* | [**add_followers_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#add_followers_for_project) | **POST** /projects/{project_gid}/addFollowers | Add followers to a project
-*ProjectsApi* | [**add_members_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#add_members_for_project) | **POST** /projects/{project_gid}/addMembers | Add users to a project
-*ProjectsApi* | [**create_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#create_project) | **POST** /projects | Create a project
-*ProjectsApi* | [**create_project_for_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#create_project_for_team) | **POST** /teams/{team_gid}/projects | Create a project in a team
-*ProjectsApi* | [**create_project_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#create_project_for_workspace) | **POST** /workspaces/{workspace_gid}/projects | Create a project in a workspace
-*ProjectsApi* | [**delete_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#delete_project) | **DELETE** /projects/{project_gid} | Delete a project
-*ProjectsApi* | [**duplicate_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#duplicate_project) | **POST** /projects/{project_gid}/duplicate | Duplicate a project
-*ProjectsApi* | [**get_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#get_project) | **GET** /projects/{project_gid} | Get a project
-*ProjectsApi* | [**get_projects**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#get_projects) | **GET** /projects | Get multiple projects
-*ProjectsApi* | [**get_projects_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#get_projects_for_task) | **GET** /tasks/{task_gid}/projects | Get projects a task is in
-*ProjectsApi* | [**get_projects_for_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#get_projects_for_team) | **GET** /teams/{team_gid}/projects | Get a team&#x27;s projects
-*ProjectsApi* | [**get_projects_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#get_projects_for_workspace) | **GET** /workspaces/{workspace_gid}/projects | Get all projects in a workspace
-*ProjectsApi* | [**get_task_counts_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#get_task_counts_for_project) | **GET** /projects/{project_gid}/task_counts | Get task count of a project
-*ProjectsApi* | [**project_save_as_template**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#project_save_as_template) | **POST** /projects/{project_gid}/saveAsTemplate | Create a project template from a project
-*ProjectsApi* | [**remove_custom_field_setting_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#remove_custom_field_setting_for_project) | **POST** /projects/{project_gid}/removeCustomFieldSetting | Remove a custom field from a project
-*ProjectsApi* | [**remove_followers_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#remove_followers_for_project) | **POST** /projects/{project_gid}/removeFollowers | Remove followers from a project
-*ProjectsApi* | [**remove_members_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#remove_members_for_project) | **POST** /projects/{project_gid}/removeMembers | Remove users from a project
-*ProjectsApi* | [**update_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#update_project) | **PUT** /projects/{project_gid} | Update a project
-*RulesApi* | [**trigger_rule**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/RulesApi.md#trigger_rule) | **POST** /rule_triggers/{rule_trigger_gid}/run | Trigger a rule
-*SectionsApi* | [**add_task_for_section**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/SectionsApi.md#add_task_for_section) | **POST** /sections/{section_gid}/addTask | Add task to section
-*SectionsApi* | [**create_section_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/SectionsApi.md#create_section_for_project) | **POST** /projects/{project_gid}/sections | Create a section in a project
-*SectionsApi* | [**delete_section**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/SectionsApi.md#delete_section) | **DELETE** /sections/{section_gid} | Delete a section
-*SectionsApi* | [**get_section**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/SectionsApi.md#get_section) | **GET** /sections/{section_gid} | Get a section
-*SectionsApi* | [**get_sections_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/SectionsApi.md#get_sections_for_project) | **GET** /projects/{project_gid}/sections | Get sections in a project
-*SectionsApi* | [**insert_section_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/SectionsApi.md#insert_section_for_project) | **POST** /projects/{project_gid}/sections/insert | Move or Insert sections
-*SectionsApi* | [**update_section**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/SectionsApi.md#update_section) | **PUT** /sections/{section_gid} | Update a section
-*StatusUpdatesApi* | [**create_status_for_object**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StatusUpdatesApi.md#create_status_for_object) | **POST** /status_updates | Create a status update
-*StatusUpdatesApi* | [**delete_status**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StatusUpdatesApi.md#delete_status) | **DELETE** /status_updates/{status_update_gid} | Delete a status update
-*StatusUpdatesApi* | [**get_status**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StatusUpdatesApi.md#get_status) | **GET** /status_updates/{status_update_gid} | Get a status update
-*StatusUpdatesApi* | [**get_statuses_for_object**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StatusUpdatesApi.md#get_statuses_for_object) | **GET** /status_updates | Get status updates from an object
-*StoriesApi* | [**create_story_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StoriesApi.md#create_story_for_task) | **POST** /tasks/{task_gid}/stories | Create a story on a task
-*StoriesApi* | [**delete_story**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StoriesApi.md#delete_story) | **DELETE** /stories/{story_gid} | Delete a story
-*StoriesApi* | [**get_stories_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StoriesApi.md#get_stories_for_task) | **GET** /tasks/{task_gid}/stories | Get stories from a task
-*StoriesApi* | [**get_story**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StoriesApi.md#get_story) | **GET** /stories/{story_gid} | Get a story
-*StoriesApi* | [**update_story**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StoriesApi.md#update_story) | **PUT** /stories/{story_gid} | Update a story
-*TagsApi* | [**create_tag**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#create_tag) | **POST** /tags | Create a tag
-*TagsApi* | [**create_tag_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#create_tag_for_workspace) | **POST** /workspaces/{workspace_gid}/tags | Create a tag in a workspace
-*TagsApi* | [**delete_tag**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#delete_tag) | **DELETE** /tags/{tag_gid} | Delete a tag
-*TagsApi* | [**get_tag**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#get_tag) | **GET** /tags/{tag_gid} | Get a tag
-*TagsApi* | [**get_tags**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#get_tags) | **GET** /tags | Get multiple tags
-*TagsApi* | [**get_tags_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#get_tags_for_task) | **GET** /tasks/{task_gid}/tags | Get a task&#x27;s tags
-*TagsApi* | [**get_tags_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#get_tags_for_workspace) | **GET** /workspaces/{workspace_gid}/tags | Get tags in a workspace
-*TagsApi* | [**update_tag**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#update_tag) | **PUT** /tags/{tag_gid} | Update a tag
-*TaskTemplatesApi* | [**delete_task_template**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TaskTemplatesApi.md#delete_task_template) | **DELETE** /task_templates/{task_template_gid} | Delete a task template
-*TaskTemplatesApi* | [**get_task_template**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TaskTemplatesApi.md#get_task_template) | **GET** /task_templates/{task_template_gid} | Get a task template
-*TaskTemplatesApi* | [**get_task_templates**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TaskTemplatesApi.md#get_task_templates) | **GET** /task_templates | Get multiple task templates
-*TaskTemplatesApi* | [**instantiate_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TaskTemplatesApi.md#instantiate_task) | **POST** /task_templates/{task_template_gid}/instantiateTask | Instantiate a task from a task template
-*TasksApi* | [**add_dependencies_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#add_dependencies_for_task) | **POST** /tasks/{task_gid}/addDependencies | Set dependencies for a task
-*TasksApi* | [**add_dependents_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#add_dependents_for_task) | **POST** /tasks/{task_gid}/addDependents | Set dependents for a task
-*TasksApi* | [**add_followers_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#add_followers_for_task) | **POST** /tasks/{task_gid}/addFollowers | Add followers to a task
-*TasksApi* | [**add_project_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#add_project_for_task) | **POST** /tasks/{task_gid}/addProject | Add a project to a task
-*TasksApi* | [**add_tag_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#add_tag_for_task) | **POST** /tasks/{task_gid}/addTag | Add a tag to a task
-*TasksApi* | [**create_subtask_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#create_subtask_for_task) | **POST** /tasks/{task_gid}/subtasks | Create a subtask
-*TasksApi* | [**create_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#create_task) | **POST** /tasks | Create a task
-*TasksApi* | [**delete_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#delete_task) | **DELETE** /tasks/{task_gid} | Delete a task
-*TasksApi* | [**duplicate_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#duplicate_task) | **POST** /tasks/{task_gid}/duplicate | Duplicate a task
-*TasksApi* | [**get_dependencies_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_dependencies_for_task) | **GET** /tasks/{task_gid}/dependencies | Get dependencies from a task
-*TasksApi* | [**get_dependents_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_dependents_for_task) | **GET** /tasks/{task_gid}/dependents | Get dependents from a task
-*TasksApi* | [**get_subtasks_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_subtasks_for_task) | **GET** /tasks/{task_gid}/subtasks | Get subtasks from a task
-*TasksApi* | [**get_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_task) | **GET** /tasks/{task_gid} | Get a task
-*TasksApi* | [**get_task_for_custom_id**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_task_for_custom_id) | **GET** /workspaces/{workspace_gid}/tasks/custom_id/{custom_id} | Get a task for a given custom ID
-*TasksApi* | [**get_tasks**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_tasks) | **GET** /tasks | Get multiple tasks
-*TasksApi* | [**get_tasks_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_tasks_for_project) | **GET** /projects/{project_gid}/tasks | Get tasks from a project
-*TasksApi* | [**get_tasks_for_section**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_tasks_for_section) | **GET** /sections/{section_gid}/tasks | Get tasks from a section
-*TasksApi* | [**get_tasks_for_tag**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_tasks_for_tag) | **GET** /tags/{tag_gid}/tasks | Get tasks from a tag
-*TasksApi* | [**get_tasks_for_user_task_list**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_tasks_for_user_task_list) | **GET** /user_task_lists/{user_task_list_gid}/tasks | Get tasks from a user task list
-*TasksApi* | [**remove_dependencies_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#remove_dependencies_for_task) | **POST** /tasks/{task_gid}/removeDependencies | Unlink dependencies from a task
-*TasksApi* | [**remove_dependents_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#remove_dependents_for_task) | **POST** /tasks/{task_gid}/removeDependents | Unlink dependents from a task
-*TasksApi* | [**remove_follower_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#remove_follower_for_task) | **POST** /tasks/{task_gid}/removeFollowers | Remove followers from a task
-*TasksApi* | [**remove_project_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#remove_project_for_task) | **POST** /tasks/{task_gid}/removeProject | Remove a project from a task
-*TasksApi* | [**remove_tag_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#remove_tag_for_task) | **POST** /tasks/{task_gid}/removeTag | Remove a tag from a task
-*TasksApi* | [**search_tasks_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#search_tasks_for_workspace) | **GET** /workspaces/{workspace_gid}/tasks/search | Search tasks in a workspace
-*TasksApi* | [**set_parent_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#set_parent_for_task) | **POST** /tasks/{task_gid}/setParent | Set the parent of a task
-*TasksApi* | [**update_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#update_task) | **PUT** /tasks/{task_gid} | Update a task
-*TeamMembershipsApi* | [**get_team_membership**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamMembershipsApi.md#get_team_membership) | **GET** /team_memberships/{team_membership_gid} | Get a team membership
-*TeamMembershipsApi* | [**get_team_memberships**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamMembershipsApi.md#get_team_memberships) | **GET** /team_memberships | Get team memberships
-*TeamMembershipsApi* | [**get_team_memberships_for_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamMembershipsApi.md#get_team_memberships_for_team) | **GET** /teams/{team_gid}/team_memberships | Get memberships from a team
-*TeamMembershipsApi* | [**get_team_memberships_for_user**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamMembershipsApi.md#get_team_memberships_for_user) | **GET** /users/{user_gid}/team_memberships | Get memberships from a user
-*TeamsApi* | [**add_user_for_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamsApi.md#add_user_for_team) | **POST** /teams/{team_gid}/addUser | Add a user to a team
-*TeamsApi* | [**create_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamsApi.md#create_team) | **POST** /teams | Create a team
-*TeamsApi* | [**get_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamsApi.md#get_team) | **GET** /teams/{team_gid} | Get a team
-*TeamsApi* | [**get_teams_for_user**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamsApi.md#get_teams_for_user) | **GET** /users/{user_gid}/teams | Get teams for a user
-*TeamsApi* | [**get_teams_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamsApi.md#get_teams_for_workspace) | **GET** /workspaces/{workspace_gid}/teams | Get teams in a workspace
-*TeamsApi* | [**remove_user_for_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamsApi.md#remove_user_for_team) | **POST** /teams/{team_gid}/removeUser | Remove a user from a team
-*TeamsApi* | [**update_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamsApi.md#update_team) | **PUT** /teams/{team_gid} | Update a team
-*TimePeriodsApi* | [**get_time_period**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TimePeriodsApi.md#get_time_period) | **GET** /time_periods/{time_period_gid} | Get a time period
-*TimePeriodsApi* | [**get_time_periods**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TimePeriodsApi.md#get_time_periods) | **GET** /time_periods | Get time periods
-*TimeTrackingEntriesApi* | [**create_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TimeTrackingEntriesApi.md#create_time_tracking_entry) | **POST** /tasks/{task_gid}/time_tracking_entries | Create a time tracking entry
-*TimeTrackingEntriesApi* | [**delete_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TimeTrackingEntriesApi.md#delete_time_tracking_entry) | **DELETE** /time_tracking_entries/{time_tracking_entry_gid} | Delete a time tracking entry
-*TimeTrackingEntriesApi* | [**get_time_tracking_entries_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TimeTrackingEntriesApi.md#get_time_tracking_entries_for_task) | **GET** /tasks/{task_gid}/time_tracking_entries | Get time tracking entries for a task
-*TimeTrackingEntriesApi* | [**get_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TimeTrackingEntriesApi.md#get_time_tracking_entry) | **GET** /time_tracking_entries/{time_tracking_entry_gid} | Get a time tracking entry
-*TimeTrackingEntriesApi* | [**update_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TimeTrackingEntriesApi.md#update_time_tracking_entry) | **PUT** /time_tracking_entries/{time_tracking_entry_gid} | Update a time tracking entry
-*TypeaheadApi* | [**typeahead_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TypeaheadApi.md#typeahead_for_workspace) | **GET** /workspaces/{workspace_gid}/typeahead | Get objects via typeahead
-*UserTaskListsApi* | [**get_user_task_list**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/UserTaskListsApi.md#get_user_task_list) | **GET** /user_task_lists/{user_task_list_gid} | Get a user task list
-*UserTaskListsApi* | [**get_user_task_list_for_user**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/UserTaskListsApi.md#get_user_task_list_for_user) | **GET** /users/{user_gid}/user_task_list | Get a user&#x27;s task list
-*UsersApi* | [**get_favorites_for_user**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/UsersApi.md#get_favorites_for_user) | **GET** /users/{user_gid}/favorites | Get a user&#x27;s favorites
-*UsersApi* | [**get_user**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/UsersApi.md#get_user) | **GET** /users/{user_gid} | Get a user
-*UsersApi* | [**get_users**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/UsersApi.md#get_users) | **GET** /users | Get multiple users
-*UsersApi* | [**get_users_for_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/UsersApi.md#get_users_for_team) | **GET** /teams/{team_gid}/users | Get users in a team
-*UsersApi* | [**get_users_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/UsersApi.md#get_users_for_workspace) | **GET** /workspaces/{workspace_gid}/users | Get users in a workspace or organization
-*WebhooksApi* | [**create_webhook**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WebhooksApi.md#create_webhook) | **POST** /webhooks | Establish a webhook
-*WebhooksApi* | [**delete_webhook**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WebhooksApi.md#delete_webhook) | **DELETE** /webhooks/{webhook_gid} | Delete a webhook
-*WebhooksApi* | [**get_webhook**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WebhooksApi.md#get_webhook) | **GET** /webhooks/{webhook_gid} | Get a webhook
-*WebhooksApi* | [**get_webhooks**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WebhooksApi.md#get_webhooks) | **GET** /webhooks | Get multiple webhooks
-*WebhooksApi* | [**update_webhook**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WebhooksApi.md#update_webhook) | **PUT** /webhooks/{webhook_gid} | Update a webhook
-*WorkspaceMembershipsApi* | [**get_workspace_membership**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspaceMembershipsApi.md#get_workspace_membership) | **GET** /workspace_memberships/{workspace_membership_gid} | Get a workspace membership
-*WorkspaceMembershipsApi* | [**get_workspace_memberships_for_user**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspaceMembershipsApi.md#get_workspace_memberships_for_user) | **GET** /users/{user_gid}/workspace_memberships | Get workspace memberships for a user
-*WorkspaceMembershipsApi* | [**get_workspace_memberships_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspaceMembershipsApi.md#get_workspace_memberships_for_workspace) | **GET** /workspaces/{workspace_gid}/workspace_memberships | Get the workspace memberships for a workspace
-*WorkspacesApi* | [**add_user_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspacesApi.md#add_user_for_workspace) | **POST** /workspaces/{workspace_gid}/addUser | Add a user to a workspace or organization
-*WorkspacesApi* | [**get_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspacesApi.md#get_workspace) | **GET** /workspaces/{workspace_gid} | Get a workspace
-*WorkspacesApi* | [**get_workspaces**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspacesApi.md#get_workspaces) | **GET** /workspaces | Get multiple workspaces
-*WorkspacesApi* | [**remove_user_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspacesApi.md#remove_user_for_workspace) | **POST** /workspaces/{workspace_gid}/removeUser | Remove a user from a workspace or organization
-*WorkspacesApi* | [**update_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspacesApi.md#update_workspace) | **PUT** /workspaces/{workspace_gid} | Update a workspace
+*AllocationsApi* | [**create_allocation**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AllocationsApi.md#create_allocation) | **POST** /allocations | Create an allocation
+*AllocationsApi* | [**delete_allocation**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AllocationsApi.md#delete_allocation) | **DELETE** /allocations/{allocation_gid} | Delete an allocation
+*AllocationsApi* | [**get_allocation**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AllocationsApi.md#get_allocation) | **GET** /allocations/{allocation_gid} | Get an allocation
+*AllocationsApi* | [**get_allocations**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AllocationsApi.md#get_allocations) | **GET** /allocations | Get multiple allocations
+*AllocationsApi* | [**update_allocation**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AllocationsApi.md#update_allocation) | **PUT** /allocations/{allocation_gid} | Update an allocation
+*AttachmentsApi* | [**create_attachment_for_object**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AttachmentsApi.md#create_attachment_for_object) | **POST** /attachments | Upload an attachment
+*AttachmentsApi* | [**delete_attachment**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AttachmentsApi.md#delete_attachment) | **DELETE** /attachments/{attachment_gid} | Delete an attachment
+*AttachmentsApi* | [**get_attachment**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AttachmentsApi.md#get_attachment) | **GET** /attachments/{attachment_gid} | Get an attachment
+*AttachmentsApi* | [**get_attachments_for_object**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AttachmentsApi.md#get_attachments_for_object) | **GET** /attachments | Get attachments from an object
+*AuditLogAPIApi* | [**get_audit_log_events**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AuditLogAPIApi.md#get_audit_log_events) | **GET** /workspaces/{workspace_gid}/audit_log_events | Get audit log events
+*BatchAPIApi* | [**create_batch_request**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/BatchAPIApi.md#create_batch_request) | **POST** /batch | Submit parallel requests
+*CustomFieldSettingsApi* | [**get_custom_field_settings_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldSettingsApi.md#get_custom_field_settings_for_portfolio) | **GET** /portfolios/{portfolio_gid}/custom_field_settings | Get a portfolio&#x27;s custom fields
+*CustomFieldSettingsApi* | [**get_custom_field_settings_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldSettingsApi.md#get_custom_field_settings_for_project) | **GET** /projects/{project_gid}/custom_field_settings | Get a project&#x27;s custom fields
+*CustomFieldsApi* | [**create_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#create_custom_field) | **POST** /custom_fields | Create a custom field
+*CustomFieldsApi* | [**create_enum_option_for_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#create_enum_option_for_custom_field) | **POST** /custom_fields/{custom_field_gid}/enum_options | Create an enum option
+*CustomFieldsApi* | [**delete_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#delete_custom_field) | **DELETE** /custom_fields/{custom_field_gid} | Delete a custom field
+*CustomFieldsApi* | [**get_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#get_custom_field) | **GET** /custom_fields/{custom_field_gid} | Get a custom field
+*CustomFieldsApi* | [**get_custom_fields_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#get_custom_fields_for_workspace) | **GET** /workspaces/{workspace_gid}/custom_fields | Get a workspace&#x27;s custom fields
+*CustomFieldsApi* | [**insert_enum_option_for_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#insert_enum_option_for_custom_field) | **POST** /custom_fields/{custom_field_gid}/enum_options/insert | Reorder a custom field&#x27;s enum
+*CustomFieldsApi* | [**update_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#update_custom_field) | **PUT** /custom_fields/{custom_field_gid} | Update a custom field
+*CustomFieldsApi* | [**update_enum_option**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#update_enum_option) | **PUT** /enum_options/{enum_option_gid} | Update an enum option
+*EventsApi* | [**get_events**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/EventsApi.md#get_events) | **GET** /events | Get events on a resource
+*GoalRelationshipsApi* | [**add_supporting_relationship**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalRelationshipsApi.md#add_supporting_relationship) | **POST** /goals/{goal_gid}/addSupportingRelationship | Add a supporting goal relationship
+*GoalRelationshipsApi* | [**get_goal_relationship**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalRelationshipsApi.md#get_goal_relationship) | **GET** /goal_relationships/{goal_relationship_gid} | Get a goal relationship
+*GoalRelationshipsApi* | [**get_goal_relationships**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalRelationshipsApi.md#get_goal_relationships) | **GET** /goal_relationships | Get goal relationships
+*GoalRelationshipsApi* | [**remove_supporting_relationship**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalRelationshipsApi.md#remove_supporting_relationship) | **POST** /goals/{goal_gid}/removeSupportingRelationship | Removes a supporting goal relationship
+*GoalRelationshipsApi* | [**update_goal_relationship**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalRelationshipsApi.md#update_goal_relationship) | **PUT** /goal_relationships/{goal_relationship_gid} | Update a goal relationship
+*GoalsApi* | [**add_followers**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#add_followers) | **POST** /goals/{goal_gid}/addFollowers | Add a collaborator to a goal
+*GoalsApi* | [**create_goal**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#create_goal) | **POST** /goals | Create a goal
+*GoalsApi* | [**create_goal_metric**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#create_goal_metric) | **POST** /goals/{goal_gid}/setMetric | Create a goal metric
+*GoalsApi* | [**delete_goal**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#delete_goal) | **DELETE** /goals/{goal_gid} | Delete a goal
+*GoalsApi* | [**get_goal**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#get_goal) | **GET** /goals/{goal_gid} | Get a goal
+*GoalsApi* | [**get_goals**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#get_goals) | **GET** /goals | Get goals
+*GoalsApi* | [**get_parent_goals_for_goal**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#get_parent_goals_for_goal) | **GET** /goals/{goal_gid}/parentGoals | Get parent goals from a goal
+*GoalsApi* | [**remove_followers**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#remove_followers) | **POST** /goals/{goal_gid}/removeFollowers | Remove a collaborator from a goal
+*GoalsApi* | [**update_goal**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#update_goal) | **PUT** /goals/{goal_gid} | Update a goal
+*GoalsApi* | [**update_goal_metric**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#update_goal_metric) | **POST** /goals/{goal_gid}/setMetricCurrentValue | Update a goal metric
+*JobsApi* | [**get_job**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/JobsApi.md#get_job) | **GET** /jobs/{job_gid} | Get a job by id
+*MembershipsApi* | [**create_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/MembershipsApi.md#create_membership) | **POST** /memberships | Create a membership
+*MembershipsApi* | [**delete_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/MembershipsApi.md#delete_membership) | **DELETE** /memberships/{membership_gid} | Delete a membership
+*MembershipsApi* | [**get_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/MembershipsApi.md#get_membership) | **GET** /memberships/{membership_gid} | Get a membership
+*MembershipsApi* | [**get_memberships**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/MembershipsApi.md#get_memberships) | **GET** /memberships | Get multiple memberships
+*MembershipsApi* | [**update_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/MembershipsApi.md#update_membership) | **PUT** /memberships/{membership_gid} | Update a membership
+*OrganizationExportsApi* | [**create_organization_export**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/OrganizationExportsApi.md#create_organization_export) | **POST** /organization_exports | Create an organization export request
+*OrganizationExportsApi* | [**get_organization_export**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/OrganizationExportsApi.md#get_organization_export) | **GET** /organization_exports/{organization_export_gid} | Get details on an org export request
+*PortfolioMembershipsApi* | [**get_portfolio_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfolioMembershipsApi.md#get_portfolio_membership) | **GET** /portfolio_memberships/{portfolio_membership_gid} | Get a portfolio membership
+*PortfolioMembershipsApi* | [**get_portfolio_memberships**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfolioMembershipsApi.md#get_portfolio_memberships) | **GET** /portfolio_memberships | Get multiple portfolio memberships
+*PortfolioMembershipsApi* | [**get_portfolio_memberships_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfolioMembershipsApi.md#get_portfolio_memberships_for_portfolio) | **GET** /portfolios/{portfolio_gid}/portfolio_memberships | Get memberships from a portfolio
+*PortfoliosApi* | [**add_custom_field_setting_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#add_custom_field_setting_for_portfolio) | **POST** /portfolios/{portfolio_gid}/addCustomFieldSetting | Add a custom field to a portfolio
+*PortfoliosApi* | [**add_item_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#add_item_for_portfolio) | **POST** /portfolios/{portfolio_gid}/addItem | Add a portfolio item
+*PortfoliosApi* | [**add_members_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#add_members_for_portfolio) | **POST** /portfolios/{portfolio_gid}/addMembers | Add users to a portfolio
+*PortfoliosApi* | [**create_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#create_portfolio) | **POST** /portfolios | Create a portfolio
+*PortfoliosApi* | [**delete_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#delete_portfolio) | **DELETE** /portfolios/{portfolio_gid} | Delete a portfolio
+*PortfoliosApi* | [**get_items_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#get_items_for_portfolio) | **GET** /portfolios/{portfolio_gid}/items | Get portfolio items
+*PortfoliosApi* | [**get_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#get_portfolio) | **GET** /portfolios/{portfolio_gid} | Get a portfolio
+*PortfoliosApi* | [**get_portfolios**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#get_portfolios) | **GET** /portfolios | Get multiple portfolios
+*PortfoliosApi* | [**remove_custom_field_setting_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#remove_custom_field_setting_for_portfolio) | **POST** /portfolios/{portfolio_gid}/removeCustomFieldSetting | Remove a custom field from a portfolio
+*PortfoliosApi* | [**remove_item_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#remove_item_for_portfolio) | **POST** /portfolios/{portfolio_gid}/removeItem | Remove a portfolio item
+*PortfoliosApi* | [**remove_members_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#remove_members_for_portfolio) | **POST** /portfolios/{portfolio_gid}/removeMembers | Remove users from a portfolio
+*PortfoliosApi* | [**update_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#update_portfolio) | **PUT** /portfolios/{portfolio_gid} | Update a portfolio
+*ProjectBriefsApi* | [**create_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectBriefsApi.md#create_project_brief) | **POST** /projects/{project_gid}/project_briefs | Create a project brief
+*ProjectBriefsApi* | [**delete_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectBriefsApi.md#delete_project_brief) | **DELETE** /project_briefs/{project_brief_gid} | Delete a project brief
+*ProjectBriefsApi* | [**get_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectBriefsApi.md#get_project_brief) | **GET** /project_briefs/{project_brief_gid} | Get a project brief
+*ProjectBriefsApi* | [**update_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectBriefsApi.md#update_project_brief) | **PUT** /project_briefs/{project_brief_gid} | Update a project brief
+*ProjectMembershipsApi* | [**get_project_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectMembershipsApi.md#get_project_membership) | **GET** /project_memberships/{project_membership_gid} | Get a project membership
+*ProjectMembershipsApi* | [**get_project_memberships_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectMembershipsApi.md#get_project_memberships_for_project) | **GET** /projects/{project_gid}/project_memberships | Get memberships from a project
+*ProjectStatusesApi* | [**create_project_status_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectStatusesApi.md#create_project_status_for_project) | **POST** /projects/{project_gid}/project_statuses | Create a project status
+*ProjectStatusesApi* | [**delete_project_status**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectStatusesApi.md#delete_project_status) | **DELETE** /project_statuses/{project_status_gid} | Delete a project status
+*ProjectStatusesApi* | [**get_project_status**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectStatusesApi.md#get_project_status) | **GET** /project_statuses/{project_status_gid} | Get a project status
+*ProjectStatusesApi* | [**get_project_statuses_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectStatusesApi.md#get_project_statuses_for_project) | **GET** /projects/{project_gid}/project_statuses | Get statuses from a project
+*ProjectTemplatesApi* | [**delete_project_template**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectTemplatesApi.md#delete_project_template) | **DELETE** /project_templates/{project_template_gid} | Delete a project template
+*ProjectTemplatesApi* | [**get_project_template**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectTemplatesApi.md#get_project_template) | **GET** /project_templates/{project_template_gid} | Get a project template
+*ProjectTemplatesApi* | [**get_project_templates**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectTemplatesApi.md#get_project_templates) | **GET** /project_templates | Get multiple project templates
+*ProjectTemplatesApi* | [**get_project_templates_for_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectTemplatesApi.md#get_project_templates_for_team) | **GET** /teams/{team_gid}/project_templates | Get a team&#x27;s project templates
+*ProjectTemplatesApi* | [**instantiate_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectTemplatesApi.md#instantiate_project) | **POST** /project_templates/{project_template_gid}/instantiateProject | Instantiate a project from a project template
+*ProjectsApi* | [**add_custom_field_setting_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#add_custom_field_setting_for_project) | **POST** /projects/{project_gid}/addCustomFieldSetting | Add a custom field to a project
+*ProjectsApi* | [**add_followers_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#add_followers_for_project) | **POST** /projects/{project_gid}/addFollowers | Add followers to a project
+*ProjectsApi* | [**add_members_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#add_members_for_project) | **POST** /projects/{project_gid}/addMembers | Add users to a project
+*ProjectsApi* | [**create_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#create_project) | **POST** /projects | Create a project
+*ProjectsApi* | [**create_project_for_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#create_project_for_team) | **POST** /teams/{team_gid}/projects | Create a project in a team
+*ProjectsApi* | [**create_project_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#create_project_for_workspace) | **POST** /workspaces/{workspace_gid}/projects | Create a project in a workspace
+*ProjectsApi* | [**delete_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#delete_project) | **DELETE** /projects/{project_gid} | Delete a project
+*ProjectsApi* | [**duplicate_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#duplicate_project) | **POST** /projects/{project_gid}/duplicate | Duplicate a project
+*ProjectsApi* | [**get_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#get_project) | **GET** /projects/{project_gid} | Get a project
+*ProjectsApi* | [**get_projects**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#get_projects) | **GET** /projects | Get multiple projects
+*ProjectsApi* | [**get_projects_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#get_projects_for_task) | **GET** /tasks/{task_gid}/projects | Get projects a task is in
+*ProjectsApi* | [**get_projects_for_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#get_projects_for_team) | **GET** /teams/{team_gid}/projects | Get a team&#x27;s projects
+*ProjectsApi* | [**get_projects_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#get_projects_for_workspace) | **GET** /workspaces/{workspace_gid}/projects | Get all projects in a workspace
+*ProjectsApi* | [**get_task_counts_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#get_task_counts_for_project) | **GET** /projects/{project_gid}/task_counts | Get task count of a project
+*ProjectsApi* | [**project_save_as_template**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#project_save_as_template) | **POST** /projects/{project_gid}/saveAsTemplate | Create a project template from a project
+*ProjectsApi* | [**remove_custom_field_setting_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#remove_custom_field_setting_for_project) | **POST** /projects/{project_gid}/removeCustomFieldSetting | Remove a custom field from a project
+*ProjectsApi* | [**remove_followers_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#remove_followers_for_project) | **POST** /projects/{project_gid}/removeFollowers | Remove followers from a project
+*ProjectsApi* | [**remove_members_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#remove_members_for_project) | **POST** /projects/{project_gid}/removeMembers | Remove users from a project
+*ProjectsApi* | [**update_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#update_project) | **PUT** /projects/{project_gid} | Update a project
+*RulesApi* | [**trigger_rule**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/RulesApi.md#trigger_rule) | **POST** /rule_triggers/{rule_trigger_gid}/run | Trigger a rule
+*SectionsApi* | [**add_task_for_section**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/SectionsApi.md#add_task_for_section) | **POST** /sections/{section_gid}/addTask | Add task to section
+*SectionsApi* | [**create_section_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/SectionsApi.md#create_section_for_project) | **POST** /projects/{project_gid}/sections | Create a section in a project
+*SectionsApi* | [**delete_section**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/SectionsApi.md#delete_section) | **DELETE** /sections/{section_gid} | Delete a section
+*SectionsApi* | [**get_section**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/SectionsApi.md#get_section) | **GET** /sections/{section_gid} | Get a section
+*SectionsApi* | [**get_sections_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/SectionsApi.md#get_sections_for_project) | **GET** /projects/{project_gid}/sections | Get sections in a project
+*SectionsApi* | [**insert_section_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/SectionsApi.md#insert_section_for_project) | **POST** /projects/{project_gid}/sections/insert | Move or Insert sections
+*SectionsApi* | [**update_section**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/SectionsApi.md#update_section) | **PUT** /sections/{section_gid} | Update a section
+*StatusUpdatesApi* | [**create_status_for_object**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StatusUpdatesApi.md#create_status_for_object) | **POST** /status_updates | Create a status update
+*StatusUpdatesApi* | [**delete_status**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StatusUpdatesApi.md#delete_status) | **DELETE** /status_updates/{status_update_gid} | Delete a status update
+*StatusUpdatesApi* | [**get_status**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StatusUpdatesApi.md#get_status) | **GET** /status_updates/{status_update_gid} | Get a status update
+*StatusUpdatesApi* | [**get_statuses_for_object**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StatusUpdatesApi.md#get_statuses_for_object) | **GET** /status_updates | Get status updates from an object
+*StoriesApi* | [**create_story_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StoriesApi.md#create_story_for_task) | **POST** /tasks/{task_gid}/stories | Create a story on a task
+*StoriesApi* | [**delete_story**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StoriesApi.md#delete_story) | **DELETE** /stories/{story_gid} | Delete a story
+*StoriesApi* | [**get_stories_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StoriesApi.md#get_stories_for_task) | **GET** /tasks/{task_gid}/stories | Get stories from a task
+*StoriesApi* | [**get_story**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StoriesApi.md#get_story) | **GET** /stories/{story_gid} | Get a story
+*StoriesApi* | [**update_story**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StoriesApi.md#update_story) | **PUT** /stories/{story_gid} | Update a story
+*TagsApi* | [**create_tag**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#create_tag) | **POST** /tags | Create a tag
+*TagsApi* | [**create_tag_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#create_tag_for_workspace) | **POST** /workspaces/{workspace_gid}/tags | Create a tag in a workspace
+*TagsApi* | [**delete_tag**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#delete_tag) | **DELETE** /tags/{tag_gid} | Delete a tag
+*TagsApi* | [**get_tag**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#get_tag) | **GET** /tags/{tag_gid} | Get a tag
+*TagsApi* | [**get_tags**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#get_tags) | **GET** /tags | Get multiple tags
+*TagsApi* | [**get_tags_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#get_tags_for_task) | **GET** /tasks/{task_gid}/tags | Get a task&#x27;s tags
+*TagsApi* | [**get_tags_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#get_tags_for_workspace) | **GET** /workspaces/{workspace_gid}/tags | Get tags in a workspace
+*TagsApi* | [**update_tag**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#update_tag) | **PUT** /tags/{tag_gid} | Update a tag
+*TaskTemplatesApi* | [**delete_task_template**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TaskTemplatesApi.md#delete_task_template) | **DELETE** /task_templates/{task_template_gid} | Delete a task template
+*TaskTemplatesApi* | [**get_task_template**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TaskTemplatesApi.md#get_task_template) | **GET** /task_templates/{task_template_gid} | Get a task template
+*TaskTemplatesApi* | [**get_task_templates**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TaskTemplatesApi.md#get_task_templates) | **GET** /task_templates | Get multiple task templates
+*TaskTemplatesApi* | [**instantiate_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TaskTemplatesApi.md#instantiate_task) | **POST** /task_templates/{task_template_gid}/instantiateTask | Instantiate a task from a task template
+*TasksApi* | [**add_dependencies_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#add_dependencies_for_task) | **POST** /tasks/{task_gid}/addDependencies | Set dependencies for a task
+*TasksApi* | [**add_dependents_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#add_dependents_for_task) | **POST** /tasks/{task_gid}/addDependents | Set dependents for a task
+*TasksApi* | [**add_followers_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#add_followers_for_task) | **POST** /tasks/{task_gid}/addFollowers | Add followers to a task
+*TasksApi* | [**add_project_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#add_project_for_task) | **POST** /tasks/{task_gid}/addProject | Add a project to a task
+*TasksApi* | [**add_tag_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#add_tag_for_task) | **POST** /tasks/{task_gid}/addTag | Add a tag to a task
+*TasksApi* | [**create_subtask_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#create_subtask_for_task) | **POST** /tasks/{task_gid}/subtasks | Create a subtask
+*TasksApi* | [**create_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#create_task) | **POST** /tasks | Create a task
+*TasksApi* | [**delete_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#delete_task) | **DELETE** /tasks/{task_gid} | Delete a task
+*TasksApi* | [**duplicate_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#duplicate_task) | **POST** /tasks/{task_gid}/duplicate | Duplicate a task
+*TasksApi* | [**get_dependencies_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_dependencies_for_task) | **GET** /tasks/{task_gid}/dependencies | Get dependencies from a task
+*TasksApi* | [**get_dependents_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_dependents_for_task) | **GET** /tasks/{task_gid}/dependents | Get dependents from a task
+*TasksApi* | [**get_subtasks_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_subtasks_for_task) | **GET** /tasks/{task_gid}/subtasks | Get subtasks from a task
+*TasksApi* | [**get_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_task) | **GET** /tasks/{task_gid} | Get a task
+*TasksApi* | [**get_task_for_custom_id**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_task_for_custom_id) | **GET** /workspaces/{workspace_gid}/tasks/custom_id/{custom_id} | Get a task for a given custom ID
+*TasksApi* | [**get_tasks**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_tasks) | **GET** /tasks | Get multiple tasks
+*TasksApi* | [**get_tasks_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_tasks_for_project) | **GET** /projects/{project_gid}/tasks | Get tasks from a project
+*TasksApi* | [**get_tasks_for_section**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_tasks_for_section) | **GET** /sections/{section_gid}/tasks | Get tasks from a section
+*TasksApi* | [**get_tasks_for_tag**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_tasks_for_tag) | **GET** /tags/{tag_gid}/tasks | Get tasks from a tag
+*TasksApi* | [**get_tasks_for_user_task_list**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_tasks_for_user_task_list) | **GET** /user_task_lists/{user_task_list_gid}/tasks | Get tasks from a user task list
+*TasksApi* | [**remove_dependencies_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#remove_dependencies_for_task) | **POST** /tasks/{task_gid}/removeDependencies | Unlink dependencies from a task
+*TasksApi* | [**remove_dependents_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#remove_dependents_for_task) | **POST** /tasks/{task_gid}/removeDependents | Unlink dependents from a task
+*TasksApi* | [**remove_follower_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#remove_follower_for_task) | **POST** /tasks/{task_gid}/removeFollowers | Remove followers from a task
+*TasksApi* | [**remove_project_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#remove_project_for_task) | **POST** /tasks/{task_gid}/removeProject | Remove a project from a task
+*TasksApi* | [**remove_tag_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#remove_tag_for_task) | **POST** /tasks/{task_gid}/removeTag | Remove a tag from a task
+*TasksApi* | [**search_tasks_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#search_tasks_for_workspace) | **GET** /workspaces/{workspace_gid}/tasks/search | Search tasks in a workspace
+*TasksApi* | [**set_parent_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#set_parent_for_task) | **POST** /tasks/{task_gid}/setParent | Set the parent of a task
+*TasksApi* | [**update_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#update_task) | **PUT** /tasks/{task_gid} | Update a task
+*TeamMembershipsApi* | [**get_team_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamMembershipsApi.md#get_team_membership) | **GET** /team_memberships/{team_membership_gid} | Get a team membership
+*TeamMembershipsApi* | [**get_team_memberships**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamMembershipsApi.md#get_team_memberships) | **GET** /team_memberships | Get team memberships
+*TeamMembershipsApi* | [**get_team_memberships_for_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamMembershipsApi.md#get_team_memberships_for_team) | **GET** /teams/{team_gid}/team_memberships | Get memberships from a team
+*TeamMembershipsApi* | [**get_team_memberships_for_user**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamMembershipsApi.md#get_team_memberships_for_user) | **GET** /users/{user_gid}/team_memberships | Get memberships from a user
+*TeamsApi* | [**add_user_for_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamsApi.md#add_user_for_team) | **POST** /teams/{team_gid}/addUser | Add a user to a team
+*TeamsApi* | [**create_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamsApi.md#create_team) | **POST** /teams | Create a team
+*TeamsApi* | [**get_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamsApi.md#get_team) | **GET** /teams/{team_gid} | Get a team
+*TeamsApi* | [**get_teams_for_user**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamsApi.md#get_teams_for_user) | **GET** /users/{user_gid}/teams | Get teams for a user
+*TeamsApi* | [**get_teams_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamsApi.md#get_teams_for_workspace) | **GET** /workspaces/{workspace_gid}/teams | Get teams in a workspace
+*TeamsApi* | [**remove_user_for_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamsApi.md#remove_user_for_team) | **POST** /teams/{team_gid}/removeUser | Remove a user from a team
+*TeamsApi* | [**update_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamsApi.md#update_team) | **PUT** /teams/{team_gid} | Update a team
+*TimePeriodsApi* | [**get_time_period**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TimePeriodsApi.md#get_time_period) | **GET** /time_periods/{time_period_gid} | Get a time period
+*TimePeriodsApi* | [**get_time_periods**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TimePeriodsApi.md#get_time_periods) | **GET** /time_periods | Get time periods
+*TimeTrackingEntriesApi* | [**create_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TimeTrackingEntriesApi.md#create_time_tracking_entry) | **POST** /tasks/{task_gid}/time_tracking_entries | Create a time tracking entry
+*TimeTrackingEntriesApi* | [**delete_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TimeTrackingEntriesApi.md#delete_time_tracking_entry) | **DELETE** /time_tracking_entries/{time_tracking_entry_gid} | Delete a time tracking entry
+*TimeTrackingEntriesApi* | [**get_time_tracking_entries_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TimeTrackingEntriesApi.md#get_time_tracking_entries_for_task) | **GET** /tasks/{task_gid}/time_tracking_entries | Get time tracking entries for a task
+*TimeTrackingEntriesApi* | [**get_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TimeTrackingEntriesApi.md#get_time_tracking_entry) | **GET** /time_tracking_entries/{time_tracking_entry_gid} | Get a time tracking entry
+*TimeTrackingEntriesApi* | [**update_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TimeTrackingEntriesApi.md#update_time_tracking_entry) | **PUT** /time_tracking_entries/{time_tracking_entry_gid} | Update a time tracking entry
+*TypeaheadApi* | [**typeahead_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TypeaheadApi.md#typeahead_for_workspace) | **GET** /workspaces/{workspace_gid}/typeahead | Get objects via typeahead
+*UserTaskListsApi* | [**get_user_task_list**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/UserTaskListsApi.md#get_user_task_list) | **GET** /user_task_lists/{user_task_list_gid} | Get a user task list
+*UserTaskListsApi* | [**get_user_task_list_for_user**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/UserTaskListsApi.md#get_user_task_list_for_user) | **GET** /users/{user_gid}/user_task_list | Get a user&#x27;s task list
+*UsersApi* | [**get_favorites_for_user**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/UsersApi.md#get_favorites_for_user) | **GET** /users/{user_gid}/favorites | Get a user&#x27;s favorites
+*UsersApi* | [**get_user**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/UsersApi.md#get_user) | **GET** /users/{user_gid} | Get a user
+*UsersApi* | [**get_users**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/UsersApi.md#get_users) | **GET** /users | Get multiple users
+*UsersApi* | [**get_users_for_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/UsersApi.md#get_users_for_team) | **GET** /teams/{team_gid}/users | Get users in a team
+*UsersApi* | [**get_users_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/UsersApi.md#get_users_for_workspace) | **GET** /workspaces/{workspace_gid}/users | Get users in a workspace or organization
+*WebhooksApi* | [**create_webhook**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WebhooksApi.md#create_webhook) | **POST** /webhooks | Establish a webhook
+*WebhooksApi* | [**delete_webhook**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WebhooksApi.md#delete_webhook) | **DELETE** /webhooks/{webhook_gid} | Delete a webhook
+*WebhooksApi* | [**get_webhook**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WebhooksApi.md#get_webhook) | **GET** /webhooks/{webhook_gid} | Get a webhook
+*WebhooksApi* | [**get_webhooks**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WebhooksApi.md#get_webhooks) | **GET** /webhooks | Get multiple webhooks
+*WebhooksApi* | [**update_webhook**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WebhooksApi.md#update_webhook) | **PUT** /webhooks/{webhook_gid} | Update a webhook
+*WorkspaceMembershipsApi* | [**get_workspace_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspaceMembershipsApi.md#get_workspace_membership) | **GET** /workspace_memberships/{workspace_membership_gid} | Get a workspace membership
+*WorkspaceMembershipsApi* | [**get_workspace_memberships_for_user**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspaceMembershipsApi.md#get_workspace_memberships_for_user) | **GET** /users/{user_gid}/workspace_memberships | Get workspace memberships for a user
+*WorkspaceMembershipsApi* | [**get_workspace_memberships_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspaceMembershipsApi.md#get_workspace_memberships_for_workspace) | **GET** /workspaces/{workspace_gid}/workspace_memberships | Get the workspace memberships for a workspace
+*WorkspacesApi* | [**add_user_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspacesApi.md#add_user_for_workspace) | **POST** /workspaces/{workspace_gid}/addUser | Add a user to a workspace or organization
+*WorkspacesApi* | [**get_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspacesApi.md#get_workspace) | **GET** /workspaces/{workspace_gid} | Get a workspace
+*WorkspacesApi* | [**get_workspaces**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspacesApi.md#get_workspaces) | **GET** /workspaces | Get multiple workspaces
+*WorkspacesApi* | [**remove_user_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspacesApi.md#remove_user_for_workspace) | **POST** /workspaces/{workspace_gid}/removeUser | Remove a user from a workspace or organization
+*WorkspacesApi* | [**update_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspacesApi.md#update_workspace) | **PUT** /workspaces/{workspace_gid} | Update a workspace
 
-## Accessing repsonse data
+## Accessing response data
 
 ### Example: Accessing task data
 ```python
 .
 .
 .
 try:
@@ -499,15 +494,15 @@
         print("Exception when calling TasksApi->create_task: %s\n" % e)
 ```
 
 ## Pagination
 
 The pagination feature is enabled by default. This means two things:
 
-1: Endpoints that return a single response (EX: [get_task](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_task) ([Get a task](https://developers.asana.com/reference/gettask)), [get_project](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_project) ([Get a project](https://developers.asana.com/reference/getproject)), etc...)
+1: Endpoints that return a single response (EX: [get_task](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_task) ([Get a task](https://developers.asana.com/reference/gettask)), [get_project](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_project) ([Get a project](https://developers.asana.com/reference/getproject)), etc...)
 will return a response with the `"data"` key abstracted from the response.
 
 Instead of returning:
 ```python
 {
     "data": {
         "gid": "123",
@@ -534,16 +529,16 @@
         "gid": "1234567",
         "name": "user@example.com",
         "resource_type": "workspace"
     }
 }
 ```
 
-2: Endpoints that return an array of resources (EX: [get_tasks](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_tasks) ([Get multiple tasks](https://developers.asana.com/reference/gettasks)), [get_projects](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#get_projects) ([Get multiple projects](https://developers.asana.com/reference/getprojects)), etc...)
-will return a generator object ([PageIterator.items](https://github.com/Asana/python-asana/blob/v5.0.5/asana/pagination/page_iterator.py)) that you can use to iterate through each result.
+2: Endpoints that return an array of resources (EX: [get_tasks](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_tasks) ([Get multiple tasks](https://developers.asana.com/reference/gettasks)), [get_projects](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#get_projects) ([Get multiple projects](https://developers.asana.com/reference/getprojects)), etc...)
+will return a generator object ([PageIterator.items](https://github.com/Asana/python-asana/blob/v5.0.6/asana/pagination/page_iterator.py)) that you can use to iterate through each result.
 
 Example usage 1:
 ```python
 import asana
 from asana.rest import ApiException
 from pprint import pprint
```

### Comparing `asana-5.0.5/README.md` & `asana-5.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,22 @@
+Metadata-Version: 2.1
+Name: asana
+Version: 5.0.6
+Summary: Asana
+Home-page: http://github.com/asana/python-asana
+Author: Asana, Inc
+License: MIT
+Keywords: asana,Asana
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # asana [![GitHub release][release-image]]() [![PyPi Version][pypi-image]][pypi-url]
 
 - API version: 1.0
-- Package version: 5.0.5
+- Package version: 5.0.6
 
 ## Requirements.
 
 Python 3.4+
 
 ## Installation & Usage
 ### pip install from [PyPI](https://pypi.org/project/asana/)
@@ -174,199 +185,205 @@
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://app.asana.com/api/1.0*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
-*AttachmentsApi* | [**create_attachment_for_object**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/AttachmentsApi.md#create_attachment_for_object) | **POST** /attachments | Upload an attachment
-*AttachmentsApi* | [**delete_attachment**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/AttachmentsApi.md#delete_attachment) | **DELETE** /attachments/{attachment_gid} | Delete an attachment
-*AttachmentsApi* | [**get_attachment**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/AttachmentsApi.md#get_attachment) | **GET** /attachments/{attachment_gid} | Get an attachment
-*AttachmentsApi* | [**get_attachments_for_object**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/AttachmentsApi.md#get_attachments_for_object) | **GET** /attachments | Get attachments from an object
-*AuditLogAPIApi* | [**get_audit_log_events**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/AuditLogAPIApi.md#get_audit_log_events) | **GET** /workspaces/{workspace_gid}/audit_log_events | Get audit log events
-*BatchAPIApi* | [**create_batch_request**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/BatchAPIApi.md#create_batch_request) | **POST** /batch | Submit parallel requests
-*CustomFieldSettingsApi* | [**get_custom_field_settings_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldSettingsApi.md#get_custom_field_settings_for_portfolio) | **GET** /portfolios/{portfolio_gid}/custom_field_settings | Get a portfolio&#x27;s custom fields
-*CustomFieldSettingsApi* | [**get_custom_field_settings_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldSettingsApi.md#get_custom_field_settings_for_project) | **GET** /projects/{project_gid}/custom_field_settings | Get a project&#x27;s custom fields
-*CustomFieldsApi* | [**create_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#create_custom_field) | **POST** /custom_fields | Create a custom field
-*CustomFieldsApi* | [**create_enum_option_for_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#create_enum_option_for_custom_field) | **POST** /custom_fields/{custom_field_gid}/enum_options | Create an enum option
-*CustomFieldsApi* | [**delete_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#delete_custom_field) | **DELETE** /custom_fields/{custom_field_gid} | Delete a custom field
-*CustomFieldsApi* | [**get_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#get_custom_field) | **GET** /custom_fields/{custom_field_gid} | Get a custom field
-*CustomFieldsApi* | [**get_custom_fields_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#get_custom_fields_for_workspace) | **GET** /workspaces/{workspace_gid}/custom_fields | Get a workspace&#x27;s custom fields
-*CustomFieldsApi* | [**insert_enum_option_for_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#insert_enum_option_for_custom_field) | **POST** /custom_fields/{custom_field_gid}/enum_options/insert | Reorder a custom field&#x27;s enum
-*CustomFieldsApi* | [**update_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#update_custom_field) | **PUT** /custom_fields/{custom_field_gid} | Update a custom field
-*CustomFieldsApi* | [**update_enum_option**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#update_enum_option) | **PUT** /enum_options/{enum_option_gid} | Update an enum option
-*EventsApi* | [**get_events**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/EventsApi.md#get_events) | **GET** /events | Get events on a resource
-*GoalRelationshipsApi* | [**add_supporting_relationship**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalRelationshipsApi.md#add_supporting_relationship) | **POST** /goals/{goal_gid}/addSupportingRelationship | Add a supporting goal relationship
-*GoalRelationshipsApi* | [**get_goal_relationship**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalRelationshipsApi.md#get_goal_relationship) | **GET** /goal_relationships/{goal_relationship_gid} | Get a goal relationship
-*GoalRelationshipsApi* | [**get_goal_relationships**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalRelationshipsApi.md#get_goal_relationships) | **GET** /goal_relationships | Get goal relationships
-*GoalRelationshipsApi* | [**remove_supporting_relationship**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalRelationshipsApi.md#remove_supporting_relationship) | **POST** /goals/{goal_gid}/removeSupportingRelationship | Removes a supporting goal relationship
-*GoalRelationshipsApi* | [**update_goal_relationship**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalRelationshipsApi.md#update_goal_relationship) | **PUT** /goal_relationships/{goal_relationship_gid} | Update a goal relationship
-*GoalsApi* | [**add_followers**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#add_followers) | **POST** /goals/{goal_gid}/addFollowers | Add a collaborator to a goal
-*GoalsApi* | [**create_goal**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#create_goal) | **POST** /goals | Create a goal
-*GoalsApi* | [**create_goal_metric**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#create_goal_metric) | **POST** /goals/{goal_gid}/setMetric | Create a goal metric
-*GoalsApi* | [**delete_goal**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#delete_goal) | **DELETE** /goals/{goal_gid} | Delete a goal
-*GoalsApi* | [**get_goal**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#get_goal) | **GET** /goals/{goal_gid} | Get a goal
-*GoalsApi* | [**get_goals**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#get_goals) | **GET** /goals | Get goals
-*GoalsApi* | [**get_parent_goals_for_goal**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#get_parent_goals_for_goal) | **GET** /goals/{goal_gid}/parentGoals | Get parent goals from a goal
-*GoalsApi* | [**remove_followers**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#remove_followers) | **POST** /goals/{goal_gid}/removeFollowers | Remove a collaborator from a goal
-*GoalsApi* | [**update_goal**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#update_goal) | **PUT** /goals/{goal_gid} | Update a goal
-*GoalsApi* | [**update_goal_metric**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#update_goal_metric) | **POST** /goals/{goal_gid}/setMetricCurrentValue | Update a goal metric
-*JobsApi* | [**get_job**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/JobsApi.md#get_job) | **GET** /jobs/{job_gid} | Get a job by id
-*MembershipsApi* | [**create_membership**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/MembershipsApi.md#create_membership) | **POST** /memberships | Create a membership
-*MembershipsApi* | [**delete_membership**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/MembershipsApi.md#delete_membership) | **DELETE** /memberships/{membership_gid} | Delete a membership
-*MembershipsApi* | [**get_membership**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/MembershipsApi.md#get_membership) | **GET** /memberships/{membership_gid} | Get a membership
-*MembershipsApi* | [**get_memberships**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/MembershipsApi.md#get_memberships) | **GET** /memberships | Get multiple memberships
-*OrganizationExportsApi* | [**create_organization_export**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/OrganizationExportsApi.md#create_organization_export) | **POST** /organization_exports | Create an organization export request
-*OrganizationExportsApi* | [**get_organization_export**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/OrganizationExportsApi.md#get_organization_export) | **GET** /organization_exports/{organization_export_gid} | Get details on an org export request
-*PortfolioMembershipsApi* | [**get_portfolio_membership**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfolioMembershipsApi.md#get_portfolio_membership) | **GET** /portfolio_memberships/{portfolio_membership_gid} | Get a portfolio membership
-*PortfolioMembershipsApi* | [**get_portfolio_memberships**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfolioMembershipsApi.md#get_portfolio_memberships) | **GET** /portfolio_memberships | Get multiple portfolio memberships
-*PortfolioMembershipsApi* | [**get_portfolio_memberships_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfolioMembershipsApi.md#get_portfolio_memberships_for_portfolio) | **GET** /portfolios/{portfolio_gid}/portfolio_memberships | Get memberships from a portfolio
-*PortfoliosApi* | [**add_custom_field_setting_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#add_custom_field_setting_for_portfolio) | **POST** /portfolios/{portfolio_gid}/addCustomFieldSetting | Add a custom field to a portfolio
-*PortfoliosApi* | [**add_item_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#add_item_for_portfolio) | **POST** /portfolios/{portfolio_gid}/addItem | Add a portfolio item
-*PortfoliosApi* | [**add_members_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#add_members_for_portfolio) | **POST** /portfolios/{portfolio_gid}/addMembers | Add users to a portfolio
-*PortfoliosApi* | [**create_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#create_portfolio) | **POST** /portfolios | Create a portfolio
-*PortfoliosApi* | [**delete_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#delete_portfolio) | **DELETE** /portfolios/{portfolio_gid} | Delete a portfolio
-*PortfoliosApi* | [**get_items_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#get_items_for_portfolio) | **GET** /portfolios/{portfolio_gid}/items | Get portfolio items
-*PortfoliosApi* | [**get_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#get_portfolio) | **GET** /portfolios/{portfolio_gid} | Get a portfolio
-*PortfoliosApi* | [**get_portfolios**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#get_portfolios) | **GET** /portfolios | Get multiple portfolios
-*PortfoliosApi* | [**remove_custom_field_setting_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#remove_custom_field_setting_for_portfolio) | **POST** /portfolios/{portfolio_gid}/removeCustomFieldSetting | Remove a custom field from a portfolio
-*PortfoliosApi* | [**remove_item_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#remove_item_for_portfolio) | **POST** /portfolios/{portfolio_gid}/removeItem | Remove a portfolio item
-*PortfoliosApi* | [**remove_members_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#remove_members_for_portfolio) | **POST** /portfolios/{portfolio_gid}/removeMembers | Remove users from a portfolio
-*PortfoliosApi* | [**update_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#update_portfolio) | **PUT** /portfolios/{portfolio_gid} | Update a portfolio
-*ProjectBriefsApi* | [**create_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectBriefsApi.md#create_project_brief) | **POST** /projects/{project_gid}/project_briefs | Create a project brief
-*ProjectBriefsApi* | [**delete_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectBriefsApi.md#delete_project_brief) | **DELETE** /project_briefs/{project_brief_gid} | Delete a project brief
-*ProjectBriefsApi* | [**get_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectBriefsApi.md#get_project_brief) | **GET** /project_briefs/{project_brief_gid} | Get a project brief
-*ProjectBriefsApi* | [**update_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectBriefsApi.md#update_project_brief) | **PUT** /project_briefs/{project_brief_gid} | Update a project brief
-*ProjectMembershipsApi* | [**get_project_membership**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectMembershipsApi.md#get_project_membership) | **GET** /project_memberships/{project_membership_gid} | Get a project membership
-*ProjectMembershipsApi* | [**get_project_memberships_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectMembershipsApi.md#get_project_memberships_for_project) | **GET** /projects/{project_gid}/project_memberships | Get memberships from a project
-*ProjectStatusesApi* | [**create_project_status_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectStatusesApi.md#create_project_status_for_project) | **POST** /projects/{project_gid}/project_statuses | Create a project status
-*ProjectStatusesApi* | [**delete_project_status**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectStatusesApi.md#delete_project_status) | **DELETE** /project_statuses/{project_status_gid} | Delete a project status
-*ProjectStatusesApi* | [**get_project_status**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectStatusesApi.md#get_project_status) | **GET** /project_statuses/{project_status_gid} | Get a project status
-*ProjectStatusesApi* | [**get_project_statuses_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectStatusesApi.md#get_project_statuses_for_project) | **GET** /projects/{project_gid}/project_statuses | Get statuses from a project
-*ProjectTemplatesApi* | [**delete_project_template**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectTemplatesApi.md#delete_project_template) | **DELETE** /project_templates/{project_template_gid} | Delete a project template
-*ProjectTemplatesApi* | [**get_project_template**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectTemplatesApi.md#get_project_template) | **GET** /project_templates/{project_template_gid} | Get a project template
-*ProjectTemplatesApi* | [**get_project_templates**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectTemplatesApi.md#get_project_templates) | **GET** /project_templates | Get multiple project templates
-*ProjectTemplatesApi* | [**get_project_templates_for_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectTemplatesApi.md#get_project_templates_for_team) | **GET** /teams/{team_gid}/project_templates | Get a team&#x27;s project templates
-*ProjectTemplatesApi* | [**instantiate_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectTemplatesApi.md#instantiate_project) | **POST** /project_templates/{project_template_gid}/instantiateProject | Instantiate a project from a project template
-*ProjectsApi* | [**add_custom_field_setting_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#add_custom_field_setting_for_project) | **POST** /projects/{project_gid}/addCustomFieldSetting | Add a custom field to a project
-*ProjectsApi* | [**add_followers_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#add_followers_for_project) | **POST** /projects/{project_gid}/addFollowers | Add followers to a project
-*ProjectsApi* | [**add_members_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#add_members_for_project) | **POST** /projects/{project_gid}/addMembers | Add users to a project
-*ProjectsApi* | [**create_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#create_project) | **POST** /projects | Create a project
-*ProjectsApi* | [**create_project_for_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#create_project_for_team) | **POST** /teams/{team_gid}/projects | Create a project in a team
-*ProjectsApi* | [**create_project_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#create_project_for_workspace) | **POST** /workspaces/{workspace_gid}/projects | Create a project in a workspace
-*ProjectsApi* | [**delete_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#delete_project) | **DELETE** /projects/{project_gid} | Delete a project
-*ProjectsApi* | [**duplicate_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#duplicate_project) | **POST** /projects/{project_gid}/duplicate | Duplicate a project
-*ProjectsApi* | [**get_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#get_project) | **GET** /projects/{project_gid} | Get a project
-*ProjectsApi* | [**get_projects**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#get_projects) | **GET** /projects | Get multiple projects
-*ProjectsApi* | [**get_projects_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#get_projects_for_task) | **GET** /tasks/{task_gid}/projects | Get projects a task is in
-*ProjectsApi* | [**get_projects_for_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#get_projects_for_team) | **GET** /teams/{team_gid}/projects | Get a team&#x27;s projects
-*ProjectsApi* | [**get_projects_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#get_projects_for_workspace) | **GET** /workspaces/{workspace_gid}/projects | Get all projects in a workspace
-*ProjectsApi* | [**get_task_counts_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#get_task_counts_for_project) | **GET** /projects/{project_gid}/task_counts | Get task count of a project
-*ProjectsApi* | [**project_save_as_template**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#project_save_as_template) | **POST** /projects/{project_gid}/saveAsTemplate | Create a project template from a project
-*ProjectsApi* | [**remove_custom_field_setting_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#remove_custom_field_setting_for_project) | **POST** /projects/{project_gid}/removeCustomFieldSetting | Remove a custom field from a project
-*ProjectsApi* | [**remove_followers_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#remove_followers_for_project) | **POST** /projects/{project_gid}/removeFollowers | Remove followers from a project
-*ProjectsApi* | [**remove_members_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#remove_members_for_project) | **POST** /projects/{project_gid}/removeMembers | Remove users from a project
-*ProjectsApi* | [**update_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#update_project) | **PUT** /projects/{project_gid} | Update a project
-*RulesApi* | [**trigger_rule**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/RulesApi.md#trigger_rule) | **POST** /rule_triggers/{rule_trigger_gid}/run | Trigger a rule
-*SectionsApi* | [**add_task_for_section**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/SectionsApi.md#add_task_for_section) | **POST** /sections/{section_gid}/addTask | Add task to section
-*SectionsApi* | [**create_section_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/SectionsApi.md#create_section_for_project) | **POST** /projects/{project_gid}/sections | Create a section in a project
-*SectionsApi* | [**delete_section**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/SectionsApi.md#delete_section) | **DELETE** /sections/{section_gid} | Delete a section
-*SectionsApi* | [**get_section**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/SectionsApi.md#get_section) | **GET** /sections/{section_gid} | Get a section
-*SectionsApi* | [**get_sections_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/SectionsApi.md#get_sections_for_project) | **GET** /projects/{project_gid}/sections | Get sections in a project
-*SectionsApi* | [**insert_section_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/SectionsApi.md#insert_section_for_project) | **POST** /projects/{project_gid}/sections/insert | Move or Insert sections
-*SectionsApi* | [**update_section**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/SectionsApi.md#update_section) | **PUT** /sections/{section_gid} | Update a section
-*StatusUpdatesApi* | [**create_status_for_object**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StatusUpdatesApi.md#create_status_for_object) | **POST** /status_updates | Create a status update
-*StatusUpdatesApi* | [**delete_status**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StatusUpdatesApi.md#delete_status) | **DELETE** /status_updates/{status_update_gid} | Delete a status update
-*StatusUpdatesApi* | [**get_status**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StatusUpdatesApi.md#get_status) | **GET** /status_updates/{status_update_gid} | Get a status update
-*StatusUpdatesApi* | [**get_statuses_for_object**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StatusUpdatesApi.md#get_statuses_for_object) | **GET** /status_updates | Get status updates from an object
-*StoriesApi* | [**create_story_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StoriesApi.md#create_story_for_task) | **POST** /tasks/{task_gid}/stories | Create a story on a task
-*StoriesApi* | [**delete_story**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StoriesApi.md#delete_story) | **DELETE** /stories/{story_gid} | Delete a story
-*StoriesApi* | [**get_stories_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StoriesApi.md#get_stories_for_task) | **GET** /tasks/{task_gid}/stories | Get stories from a task
-*StoriesApi* | [**get_story**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StoriesApi.md#get_story) | **GET** /stories/{story_gid} | Get a story
-*StoriesApi* | [**update_story**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StoriesApi.md#update_story) | **PUT** /stories/{story_gid} | Update a story
-*TagsApi* | [**create_tag**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#create_tag) | **POST** /tags | Create a tag
-*TagsApi* | [**create_tag_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#create_tag_for_workspace) | **POST** /workspaces/{workspace_gid}/tags | Create a tag in a workspace
-*TagsApi* | [**delete_tag**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#delete_tag) | **DELETE** /tags/{tag_gid} | Delete a tag
-*TagsApi* | [**get_tag**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#get_tag) | **GET** /tags/{tag_gid} | Get a tag
-*TagsApi* | [**get_tags**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#get_tags) | **GET** /tags | Get multiple tags
-*TagsApi* | [**get_tags_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#get_tags_for_task) | **GET** /tasks/{task_gid}/tags | Get a task&#x27;s tags
-*TagsApi* | [**get_tags_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#get_tags_for_workspace) | **GET** /workspaces/{workspace_gid}/tags | Get tags in a workspace
-*TagsApi* | [**update_tag**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#update_tag) | **PUT** /tags/{tag_gid} | Update a tag
-*TaskTemplatesApi* | [**delete_task_template**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TaskTemplatesApi.md#delete_task_template) | **DELETE** /task_templates/{task_template_gid} | Delete a task template
-*TaskTemplatesApi* | [**get_task_template**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TaskTemplatesApi.md#get_task_template) | **GET** /task_templates/{task_template_gid} | Get a task template
-*TaskTemplatesApi* | [**get_task_templates**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TaskTemplatesApi.md#get_task_templates) | **GET** /task_templates | Get multiple task templates
-*TaskTemplatesApi* | [**instantiate_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TaskTemplatesApi.md#instantiate_task) | **POST** /task_templates/{task_template_gid}/instantiateTask | Instantiate a task from a task template
-*TasksApi* | [**add_dependencies_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#add_dependencies_for_task) | **POST** /tasks/{task_gid}/addDependencies | Set dependencies for a task
-*TasksApi* | [**add_dependents_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#add_dependents_for_task) | **POST** /tasks/{task_gid}/addDependents | Set dependents for a task
-*TasksApi* | [**add_followers_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#add_followers_for_task) | **POST** /tasks/{task_gid}/addFollowers | Add followers to a task
-*TasksApi* | [**add_project_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#add_project_for_task) | **POST** /tasks/{task_gid}/addProject | Add a project to a task
-*TasksApi* | [**add_tag_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#add_tag_for_task) | **POST** /tasks/{task_gid}/addTag | Add a tag to a task
-*TasksApi* | [**create_subtask_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#create_subtask_for_task) | **POST** /tasks/{task_gid}/subtasks | Create a subtask
-*TasksApi* | [**create_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#create_task) | **POST** /tasks | Create a task
-*TasksApi* | [**delete_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#delete_task) | **DELETE** /tasks/{task_gid} | Delete a task
-*TasksApi* | [**duplicate_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#duplicate_task) | **POST** /tasks/{task_gid}/duplicate | Duplicate a task
-*TasksApi* | [**get_dependencies_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_dependencies_for_task) | **GET** /tasks/{task_gid}/dependencies | Get dependencies from a task
-*TasksApi* | [**get_dependents_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_dependents_for_task) | **GET** /tasks/{task_gid}/dependents | Get dependents from a task
-*TasksApi* | [**get_subtasks_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_subtasks_for_task) | **GET** /tasks/{task_gid}/subtasks | Get subtasks from a task
-*TasksApi* | [**get_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_task) | **GET** /tasks/{task_gid} | Get a task
-*TasksApi* | [**get_task_for_custom_id**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_task_for_custom_id) | **GET** /workspaces/{workspace_gid}/tasks/custom_id/{custom_id} | Get a task for a given custom ID
-*TasksApi* | [**get_tasks**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_tasks) | **GET** /tasks | Get multiple tasks
-*TasksApi* | [**get_tasks_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_tasks_for_project) | **GET** /projects/{project_gid}/tasks | Get tasks from a project
-*TasksApi* | [**get_tasks_for_section**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_tasks_for_section) | **GET** /sections/{section_gid}/tasks | Get tasks from a section
-*TasksApi* | [**get_tasks_for_tag**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_tasks_for_tag) | **GET** /tags/{tag_gid}/tasks | Get tasks from a tag
-*TasksApi* | [**get_tasks_for_user_task_list**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_tasks_for_user_task_list) | **GET** /user_task_lists/{user_task_list_gid}/tasks | Get tasks from a user task list
-*TasksApi* | [**remove_dependencies_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#remove_dependencies_for_task) | **POST** /tasks/{task_gid}/removeDependencies | Unlink dependencies from a task
-*TasksApi* | [**remove_dependents_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#remove_dependents_for_task) | **POST** /tasks/{task_gid}/removeDependents | Unlink dependents from a task
-*TasksApi* | [**remove_follower_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#remove_follower_for_task) | **POST** /tasks/{task_gid}/removeFollowers | Remove followers from a task
-*TasksApi* | [**remove_project_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#remove_project_for_task) | **POST** /tasks/{task_gid}/removeProject | Remove a project from a task
-*TasksApi* | [**remove_tag_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#remove_tag_for_task) | **POST** /tasks/{task_gid}/removeTag | Remove a tag from a task
-*TasksApi* | [**search_tasks_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#search_tasks_for_workspace) | **GET** /workspaces/{workspace_gid}/tasks/search | Search tasks in a workspace
-*TasksApi* | [**set_parent_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#set_parent_for_task) | **POST** /tasks/{task_gid}/setParent | Set the parent of a task
-*TasksApi* | [**update_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#update_task) | **PUT** /tasks/{task_gid} | Update a task
-*TeamMembershipsApi* | [**get_team_membership**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamMembershipsApi.md#get_team_membership) | **GET** /team_memberships/{team_membership_gid} | Get a team membership
-*TeamMembershipsApi* | [**get_team_memberships**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamMembershipsApi.md#get_team_memberships) | **GET** /team_memberships | Get team memberships
-*TeamMembershipsApi* | [**get_team_memberships_for_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamMembershipsApi.md#get_team_memberships_for_team) | **GET** /teams/{team_gid}/team_memberships | Get memberships from a team
-*TeamMembershipsApi* | [**get_team_memberships_for_user**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamMembershipsApi.md#get_team_memberships_for_user) | **GET** /users/{user_gid}/team_memberships | Get memberships from a user
-*TeamsApi* | [**add_user_for_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamsApi.md#add_user_for_team) | **POST** /teams/{team_gid}/addUser | Add a user to a team
-*TeamsApi* | [**create_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamsApi.md#create_team) | **POST** /teams | Create a team
-*TeamsApi* | [**get_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamsApi.md#get_team) | **GET** /teams/{team_gid} | Get a team
-*TeamsApi* | [**get_teams_for_user**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamsApi.md#get_teams_for_user) | **GET** /users/{user_gid}/teams | Get teams for a user
-*TeamsApi* | [**get_teams_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamsApi.md#get_teams_for_workspace) | **GET** /workspaces/{workspace_gid}/teams | Get teams in a workspace
-*TeamsApi* | [**remove_user_for_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamsApi.md#remove_user_for_team) | **POST** /teams/{team_gid}/removeUser | Remove a user from a team
-*TeamsApi* | [**update_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamsApi.md#update_team) | **PUT** /teams/{team_gid} | Update a team
-*TimePeriodsApi* | [**get_time_period**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TimePeriodsApi.md#get_time_period) | **GET** /time_periods/{time_period_gid} | Get a time period
-*TimePeriodsApi* | [**get_time_periods**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TimePeriodsApi.md#get_time_periods) | **GET** /time_periods | Get time periods
-*TimeTrackingEntriesApi* | [**create_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TimeTrackingEntriesApi.md#create_time_tracking_entry) | **POST** /tasks/{task_gid}/time_tracking_entries | Create a time tracking entry
-*TimeTrackingEntriesApi* | [**delete_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TimeTrackingEntriesApi.md#delete_time_tracking_entry) | **DELETE** /time_tracking_entries/{time_tracking_entry_gid} | Delete a time tracking entry
-*TimeTrackingEntriesApi* | [**get_time_tracking_entries_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TimeTrackingEntriesApi.md#get_time_tracking_entries_for_task) | **GET** /tasks/{task_gid}/time_tracking_entries | Get time tracking entries for a task
-*TimeTrackingEntriesApi* | [**get_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TimeTrackingEntriesApi.md#get_time_tracking_entry) | **GET** /time_tracking_entries/{time_tracking_entry_gid} | Get a time tracking entry
-*TimeTrackingEntriesApi* | [**update_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TimeTrackingEntriesApi.md#update_time_tracking_entry) | **PUT** /time_tracking_entries/{time_tracking_entry_gid} | Update a time tracking entry
-*TypeaheadApi* | [**typeahead_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TypeaheadApi.md#typeahead_for_workspace) | **GET** /workspaces/{workspace_gid}/typeahead | Get objects via typeahead
-*UserTaskListsApi* | [**get_user_task_list**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/UserTaskListsApi.md#get_user_task_list) | **GET** /user_task_lists/{user_task_list_gid} | Get a user task list
-*UserTaskListsApi* | [**get_user_task_list_for_user**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/UserTaskListsApi.md#get_user_task_list_for_user) | **GET** /users/{user_gid}/user_task_list | Get a user&#x27;s task list
-*UsersApi* | [**get_favorites_for_user**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/UsersApi.md#get_favorites_for_user) | **GET** /users/{user_gid}/favorites | Get a user&#x27;s favorites
-*UsersApi* | [**get_user**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/UsersApi.md#get_user) | **GET** /users/{user_gid} | Get a user
-*UsersApi* | [**get_users**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/UsersApi.md#get_users) | **GET** /users | Get multiple users
-*UsersApi* | [**get_users_for_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/UsersApi.md#get_users_for_team) | **GET** /teams/{team_gid}/users | Get users in a team
-*UsersApi* | [**get_users_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/UsersApi.md#get_users_for_workspace) | **GET** /workspaces/{workspace_gid}/users | Get users in a workspace or organization
-*WebhooksApi* | [**create_webhook**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WebhooksApi.md#create_webhook) | **POST** /webhooks | Establish a webhook
-*WebhooksApi* | [**delete_webhook**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WebhooksApi.md#delete_webhook) | **DELETE** /webhooks/{webhook_gid} | Delete a webhook
-*WebhooksApi* | [**get_webhook**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WebhooksApi.md#get_webhook) | **GET** /webhooks/{webhook_gid} | Get a webhook
-*WebhooksApi* | [**get_webhooks**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WebhooksApi.md#get_webhooks) | **GET** /webhooks | Get multiple webhooks
-*WebhooksApi* | [**update_webhook**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WebhooksApi.md#update_webhook) | **PUT** /webhooks/{webhook_gid} | Update a webhook
-*WorkspaceMembershipsApi* | [**get_workspace_membership**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspaceMembershipsApi.md#get_workspace_membership) | **GET** /workspace_memberships/{workspace_membership_gid} | Get a workspace membership
-*WorkspaceMembershipsApi* | [**get_workspace_memberships_for_user**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspaceMembershipsApi.md#get_workspace_memberships_for_user) | **GET** /users/{user_gid}/workspace_memberships | Get workspace memberships for a user
-*WorkspaceMembershipsApi* | [**get_workspace_memberships_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspaceMembershipsApi.md#get_workspace_memberships_for_workspace) | **GET** /workspaces/{workspace_gid}/workspace_memberships | Get the workspace memberships for a workspace
-*WorkspacesApi* | [**add_user_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspacesApi.md#add_user_for_workspace) | **POST** /workspaces/{workspace_gid}/addUser | Add a user to a workspace or organization
-*WorkspacesApi* | [**get_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspacesApi.md#get_workspace) | **GET** /workspaces/{workspace_gid} | Get a workspace
-*WorkspacesApi* | [**get_workspaces**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspacesApi.md#get_workspaces) | **GET** /workspaces | Get multiple workspaces
-*WorkspacesApi* | [**remove_user_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspacesApi.md#remove_user_for_workspace) | **POST** /workspaces/{workspace_gid}/removeUser | Remove a user from a workspace or organization
-*WorkspacesApi* | [**update_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspacesApi.md#update_workspace) | **PUT** /workspaces/{workspace_gid} | Update a workspace
+*AllocationsApi* | [**create_allocation**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AllocationsApi.md#create_allocation) | **POST** /allocations | Create an allocation
+*AllocationsApi* | [**delete_allocation**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AllocationsApi.md#delete_allocation) | **DELETE** /allocations/{allocation_gid} | Delete an allocation
+*AllocationsApi* | [**get_allocation**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AllocationsApi.md#get_allocation) | **GET** /allocations/{allocation_gid} | Get an allocation
+*AllocationsApi* | [**get_allocations**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AllocationsApi.md#get_allocations) | **GET** /allocations | Get multiple allocations
+*AllocationsApi* | [**update_allocation**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AllocationsApi.md#update_allocation) | **PUT** /allocations/{allocation_gid} | Update an allocation
+*AttachmentsApi* | [**create_attachment_for_object**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AttachmentsApi.md#create_attachment_for_object) | **POST** /attachments | Upload an attachment
+*AttachmentsApi* | [**delete_attachment**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AttachmentsApi.md#delete_attachment) | **DELETE** /attachments/{attachment_gid} | Delete an attachment
+*AttachmentsApi* | [**get_attachment**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AttachmentsApi.md#get_attachment) | **GET** /attachments/{attachment_gid} | Get an attachment
+*AttachmentsApi* | [**get_attachments_for_object**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AttachmentsApi.md#get_attachments_for_object) | **GET** /attachments | Get attachments from an object
+*AuditLogAPIApi* | [**get_audit_log_events**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AuditLogAPIApi.md#get_audit_log_events) | **GET** /workspaces/{workspace_gid}/audit_log_events | Get audit log events
+*BatchAPIApi* | [**create_batch_request**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/BatchAPIApi.md#create_batch_request) | **POST** /batch | Submit parallel requests
+*CustomFieldSettingsApi* | [**get_custom_field_settings_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldSettingsApi.md#get_custom_field_settings_for_portfolio) | **GET** /portfolios/{portfolio_gid}/custom_field_settings | Get a portfolio&#x27;s custom fields
+*CustomFieldSettingsApi* | [**get_custom_field_settings_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldSettingsApi.md#get_custom_field_settings_for_project) | **GET** /projects/{project_gid}/custom_field_settings | Get a project&#x27;s custom fields
+*CustomFieldsApi* | [**create_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#create_custom_field) | **POST** /custom_fields | Create a custom field
+*CustomFieldsApi* | [**create_enum_option_for_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#create_enum_option_for_custom_field) | **POST** /custom_fields/{custom_field_gid}/enum_options | Create an enum option
+*CustomFieldsApi* | [**delete_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#delete_custom_field) | **DELETE** /custom_fields/{custom_field_gid} | Delete a custom field
+*CustomFieldsApi* | [**get_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#get_custom_field) | **GET** /custom_fields/{custom_field_gid} | Get a custom field
+*CustomFieldsApi* | [**get_custom_fields_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#get_custom_fields_for_workspace) | **GET** /workspaces/{workspace_gid}/custom_fields | Get a workspace&#x27;s custom fields
+*CustomFieldsApi* | [**insert_enum_option_for_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#insert_enum_option_for_custom_field) | **POST** /custom_fields/{custom_field_gid}/enum_options/insert | Reorder a custom field&#x27;s enum
+*CustomFieldsApi* | [**update_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#update_custom_field) | **PUT** /custom_fields/{custom_field_gid} | Update a custom field
+*CustomFieldsApi* | [**update_enum_option**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#update_enum_option) | **PUT** /enum_options/{enum_option_gid} | Update an enum option
+*EventsApi* | [**get_events**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/EventsApi.md#get_events) | **GET** /events | Get events on a resource
+*GoalRelationshipsApi* | [**add_supporting_relationship**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalRelationshipsApi.md#add_supporting_relationship) | **POST** /goals/{goal_gid}/addSupportingRelationship | Add a supporting goal relationship
+*GoalRelationshipsApi* | [**get_goal_relationship**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalRelationshipsApi.md#get_goal_relationship) | **GET** /goal_relationships/{goal_relationship_gid} | Get a goal relationship
+*GoalRelationshipsApi* | [**get_goal_relationships**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalRelationshipsApi.md#get_goal_relationships) | **GET** /goal_relationships | Get goal relationships
+*GoalRelationshipsApi* | [**remove_supporting_relationship**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalRelationshipsApi.md#remove_supporting_relationship) | **POST** /goals/{goal_gid}/removeSupportingRelationship | Removes a supporting goal relationship
+*GoalRelationshipsApi* | [**update_goal_relationship**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalRelationshipsApi.md#update_goal_relationship) | **PUT** /goal_relationships/{goal_relationship_gid} | Update a goal relationship
+*GoalsApi* | [**add_followers**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#add_followers) | **POST** /goals/{goal_gid}/addFollowers | Add a collaborator to a goal
+*GoalsApi* | [**create_goal**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#create_goal) | **POST** /goals | Create a goal
+*GoalsApi* | [**create_goal_metric**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#create_goal_metric) | **POST** /goals/{goal_gid}/setMetric | Create a goal metric
+*GoalsApi* | [**delete_goal**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#delete_goal) | **DELETE** /goals/{goal_gid} | Delete a goal
+*GoalsApi* | [**get_goal**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#get_goal) | **GET** /goals/{goal_gid} | Get a goal
+*GoalsApi* | [**get_goals**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#get_goals) | **GET** /goals | Get goals
+*GoalsApi* | [**get_parent_goals_for_goal**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#get_parent_goals_for_goal) | **GET** /goals/{goal_gid}/parentGoals | Get parent goals from a goal
+*GoalsApi* | [**remove_followers**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#remove_followers) | **POST** /goals/{goal_gid}/removeFollowers | Remove a collaborator from a goal
+*GoalsApi* | [**update_goal**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#update_goal) | **PUT** /goals/{goal_gid} | Update a goal
+*GoalsApi* | [**update_goal_metric**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#update_goal_metric) | **POST** /goals/{goal_gid}/setMetricCurrentValue | Update a goal metric
+*JobsApi* | [**get_job**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/JobsApi.md#get_job) | **GET** /jobs/{job_gid} | Get a job by id
+*MembershipsApi* | [**create_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/MembershipsApi.md#create_membership) | **POST** /memberships | Create a membership
+*MembershipsApi* | [**delete_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/MembershipsApi.md#delete_membership) | **DELETE** /memberships/{membership_gid} | Delete a membership
+*MembershipsApi* | [**get_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/MembershipsApi.md#get_membership) | **GET** /memberships/{membership_gid} | Get a membership
+*MembershipsApi* | [**get_memberships**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/MembershipsApi.md#get_memberships) | **GET** /memberships | Get multiple memberships
+*MembershipsApi* | [**update_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/MembershipsApi.md#update_membership) | **PUT** /memberships/{membership_gid} | Update a membership
+*OrganizationExportsApi* | [**create_organization_export**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/OrganizationExportsApi.md#create_organization_export) | **POST** /organization_exports | Create an organization export request
+*OrganizationExportsApi* | [**get_organization_export**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/OrganizationExportsApi.md#get_organization_export) | **GET** /organization_exports/{organization_export_gid} | Get details on an org export request
+*PortfolioMembershipsApi* | [**get_portfolio_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfolioMembershipsApi.md#get_portfolio_membership) | **GET** /portfolio_memberships/{portfolio_membership_gid} | Get a portfolio membership
+*PortfolioMembershipsApi* | [**get_portfolio_memberships**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfolioMembershipsApi.md#get_portfolio_memberships) | **GET** /portfolio_memberships | Get multiple portfolio memberships
+*PortfolioMembershipsApi* | [**get_portfolio_memberships_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfolioMembershipsApi.md#get_portfolio_memberships_for_portfolio) | **GET** /portfolios/{portfolio_gid}/portfolio_memberships | Get memberships from a portfolio
+*PortfoliosApi* | [**add_custom_field_setting_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#add_custom_field_setting_for_portfolio) | **POST** /portfolios/{portfolio_gid}/addCustomFieldSetting | Add a custom field to a portfolio
+*PortfoliosApi* | [**add_item_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#add_item_for_portfolio) | **POST** /portfolios/{portfolio_gid}/addItem | Add a portfolio item
+*PortfoliosApi* | [**add_members_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#add_members_for_portfolio) | **POST** /portfolios/{portfolio_gid}/addMembers | Add users to a portfolio
+*PortfoliosApi* | [**create_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#create_portfolio) | **POST** /portfolios | Create a portfolio
+*PortfoliosApi* | [**delete_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#delete_portfolio) | **DELETE** /portfolios/{portfolio_gid} | Delete a portfolio
+*PortfoliosApi* | [**get_items_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#get_items_for_portfolio) | **GET** /portfolios/{portfolio_gid}/items | Get portfolio items
+*PortfoliosApi* | [**get_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#get_portfolio) | **GET** /portfolios/{portfolio_gid} | Get a portfolio
+*PortfoliosApi* | [**get_portfolios**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#get_portfolios) | **GET** /portfolios | Get multiple portfolios
+*PortfoliosApi* | [**remove_custom_field_setting_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#remove_custom_field_setting_for_portfolio) | **POST** /portfolios/{portfolio_gid}/removeCustomFieldSetting | Remove a custom field from a portfolio
+*PortfoliosApi* | [**remove_item_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#remove_item_for_portfolio) | **POST** /portfolios/{portfolio_gid}/removeItem | Remove a portfolio item
+*PortfoliosApi* | [**remove_members_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#remove_members_for_portfolio) | **POST** /portfolios/{portfolio_gid}/removeMembers | Remove users from a portfolio
+*PortfoliosApi* | [**update_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#update_portfolio) | **PUT** /portfolios/{portfolio_gid} | Update a portfolio
+*ProjectBriefsApi* | [**create_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectBriefsApi.md#create_project_brief) | **POST** /projects/{project_gid}/project_briefs | Create a project brief
+*ProjectBriefsApi* | [**delete_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectBriefsApi.md#delete_project_brief) | **DELETE** /project_briefs/{project_brief_gid} | Delete a project brief
+*ProjectBriefsApi* | [**get_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectBriefsApi.md#get_project_brief) | **GET** /project_briefs/{project_brief_gid} | Get a project brief
+*ProjectBriefsApi* | [**update_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectBriefsApi.md#update_project_brief) | **PUT** /project_briefs/{project_brief_gid} | Update a project brief
+*ProjectMembershipsApi* | [**get_project_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectMembershipsApi.md#get_project_membership) | **GET** /project_memberships/{project_membership_gid} | Get a project membership
+*ProjectMembershipsApi* | [**get_project_memberships_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectMembershipsApi.md#get_project_memberships_for_project) | **GET** /projects/{project_gid}/project_memberships | Get memberships from a project
+*ProjectStatusesApi* | [**create_project_status_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectStatusesApi.md#create_project_status_for_project) | **POST** /projects/{project_gid}/project_statuses | Create a project status
+*ProjectStatusesApi* | [**delete_project_status**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectStatusesApi.md#delete_project_status) | **DELETE** /project_statuses/{project_status_gid} | Delete a project status
+*ProjectStatusesApi* | [**get_project_status**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectStatusesApi.md#get_project_status) | **GET** /project_statuses/{project_status_gid} | Get a project status
+*ProjectStatusesApi* | [**get_project_statuses_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectStatusesApi.md#get_project_statuses_for_project) | **GET** /projects/{project_gid}/project_statuses | Get statuses from a project
+*ProjectTemplatesApi* | [**delete_project_template**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectTemplatesApi.md#delete_project_template) | **DELETE** /project_templates/{project_template_gid} | Delete a project template
+*ProjectTemplatesApi* | [**get_project_template**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectTemplatesApi.md#get_project_template) | **GET** /project_templates/{project_template_gid} | Get a project template
+*ProjectTemplatesApi* | [**get_project_templates**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectTemplatesApi.md#get_project_templates) | **GET** /project_templates | Get multiple project templates
+*ProjectTemplatesApi* | [**get_project_templates_for_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectTemplatesApi.md#get_project_templates_for_team) | **GET** /teams/{team_gid}/project_templates | Get a team&#x27;s project templates
+*ProjectTemplatesApi* | [**instantiate_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectTemplatesApi.md#instantiate_project) | **POST** /project_templates/{project_template_gid}/instantiateProject | Instantiate a project from a project template
+*ProjectsApi* | [**add_custom_field_setting_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#add_custom_field_setting_for_project) | **POST** /projects/{project_gid}/addCustomFieldSetting | Add a custom field to a project
+*ProjectsApi* | [**add_followers_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#add_followers_for_project) | **POST** /projects/{project_gid}/addFollowers | Add followers to a project
+*ProjectsApi* | [**add_members_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#add_members_for_project) | **POST** /projects/{project_gid}/addMembers | Add users to a project
+*ProjectsApi* | [**create_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#create_project) | **POST** /projects | Create a project
+*ProjectsApi* | [**create_project_for_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#create_project_for_team) | **POST** /teams/{team_gid}/projects | Create a project in a team
+*ProjectsApi* | [**create_project_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#create_project_for_workspace) | **POST** /workspaces/{workspace_gid}/projects | Create a project in a workspace
+*ProjectsApi* | [**delete_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#delete_project) | **DELETE** /projects/{project_gid} | Delete a project
+*ProjectsApi* | [**duplicate_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#duplicate_project) | **POST** /projects/{project_gid}/duplicate | Duplicate a project
+*ProjectsApi* | [**get_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#get_project) | **GET** /projects/{project_gid} | Get a project
+*ProjectsApi* | [**get_projects**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#get_projects) | **GET** /projects | Get multiple projects
+*ProjectsApi* | [**get_projects_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#get_projects_for_task) | **GET** /tasks/{task_gid}/projects | Get projects a task is in
+*ProjectsApi* | [**get_projects_for_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#get_projects_for_team) | **GET** /teams/{team_gid}/projects | Get a team&#x27;s projects
+*ProjectsApi* | [**get_projects_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#get_projects_for_workspace) | **GET** /workspaces/{workspace_gid}/projects | Get all projects in a workspace
+*ProjectsApi* | [**get_task_counts_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#get_task_counts_for_project) | **GET** /projects/{project_gid}/task_counts | Get task count of a project
+*ProjectsApi* | [**project_save_as_template**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#project_save_as_template) | **POST** /projects/{project_gid}/saveAsTemplate | Create a project template from a project
+*ProjectsApi* | [**remove_custom_field_setting_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#remove_custom_field_setting_for_project) | **POST** /projects/{project_gid}/removeCustomFieldSetting | Remove a custom field from a project
+*ProjectsApi* | [**remove_followers_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#remove_followers_for_project) | **POST** /projects/{project_gid}/removeFollowers | Remove followers from a project
+*ProjectsApi* | [**remove_members_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#remove_members_for_project) | **POST** /projects/{project_gid}/removeMembers | Remove users from a project
+*ProjectsApi* | [**update_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#update_project) | **PUT** /projects/{project_gid} | Update a project
+*RulesApi* | [**trigger_rule**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/RulesApi.md#trigger_rule) | **POST** /rule_triggers/{rule_trigger_gid}/run | Trigger a rule
+*SectionsApi* | [**add_task_for_section**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/SectionsApi.md#add_task_for_section) | **POST** /sections/{section_gid}/addTask | Add task to section
+*SectionsApi* | [**create_section_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/SectionsApi.md#create_section_for_project) | **POST** /projects/{project_gid}/sections | Create a section in a project
+*SectionsApi* | [**delete_section**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/SectionsApi.md#delete_section) | **DELETE** /sections/{section_gid} | Delete a section
+*SectionsApi* | [**get_section**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/SectionsApi.md#get_section) | **GET** /sections/{section_gid} | Get a section
+*SectionsApi* | [**get_sections_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/SectionsApi.md#get_sections_for_project) | **GET** /projects/{project_gid}/sections | Get sections in a project
+*SectionsApi* | [**insert_section_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/SectionsApi.md#insert_section_for_project) | **POST** /projects/{project_gid}/sections/insert | Move or Insert sections
+*SectionsApi* | [**update_section**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/SectionsApi.md#update_section) | **PUT** /sections/{section_gid} | Update a section
+*StatusUpdatesApi* | [**create_status_for_object**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StatusUpdatesApi.md#create_status_for_object) | **POST** /status_updates | Create a status update
+*StatusUpdatesApi* | [**delete_status**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StatusUpdatesApi.md#delete_status) | **DELETE** /status_updates/{status_update_gid} | Delete a status update
+*StatusUpdatesApi* | [**get_status**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StatusUpdatesApi.md#get_status) | **GET** /status_updates/{status_update_gid} | Get a status update
+*StatusUpdatesApi* | [**get_statuses_for_object**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StatusUpdatesApi.md#get_statuses_for_object) | **GET** /status_updates | Get status updates from an object
+*StoriesApi* | [**create_story_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StoriesApi.md#create_story_for_task) | **POST** /tasks/{task_gid}/stories | Create a story on a task
+*StoriesApi* | [**delete_story**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StoriesApi.md#delete_story) | **DELETE** /stories/{story_gid} | Delete a story
+*StoriesApi* | [**get_stories_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StoriesApi.md#get_stories_for_task) | **GET** /tasks/{task_gid}/stories | Get stories from a task
+*StoriesApi* | [**get_story**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StoriesApi.md#get_story) | **GET** /stories/{story_gid} | Get a story
+*StoriesApi* | [**update_story**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StoriesApi.md#update_story) | **PUT** /stories/{story_gid} | Update a story
+*TagsApi* | [**create_tag**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#create_tag) | **POST** /tags | Create a tag
+*TagsApi* | [**create_tag_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#create_tag_for_workspace) | **POST** /workspaces/{workspace_gid}/tags | Create a tag in a workspace
+*TagsApi* | [**delete_tag**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#delete_tag) | **DELETE** /tags/{tag_gid} | Delete a tag
+*TagsApi* | [**get_tag**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#get_tag) | **GET** /tags/{tag_gid} | Get a tag
+*TagsApi* | [**get_tags**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#get_tags) | **GET** /tags | Get multiple tags
+*TagsApi* | [**get_tags_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#get_tags_for_task) | **GET** /tasks/{task_gid}/tags | Get a task&#x27;s tags
+*TagsApi* | [**get_tags_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#get_tags_for_workspace) | **GET** /workspaces/{workspace_gid}/tags | Get tags in a workspace
+*TagsApi* | [**update_tag**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#update_tag) | **PUT** /tags/{tag_gid} | Update a tag
+*TaskTemplatesApi* | [**delete_task_template**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TaskTemplatesApi.md#delete_task_template) | **DELETE** /task_templates/{task_template_gid} | Delete a task template
+*TaskTemplatesApi* | [**get_task_template**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TaskTemplatesApi.md#get_task_template) | **GET** /task_templates/{task_template_gid} | Get a task template
+*TaskTemplatesApi* | [**get_task_templates**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TaskTemplatesApi.md#get_task_templates) | **GET** /task_templates | Get multiple task templates
+*TaskTemplatesApi* | [**instantiate_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TaskTemplatesApi.md#instantiate_task) | **POST** /task_templates/{task_template_gid}/instantiateTask | Instantiate a task from a task template
+*TasksApi* | [**add_dependencies_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#add_dependencies_for_task) | **POST** /tasks/{task_gid}/addDependencies | Set dependencies for a task
+*TasksApi* | [**add_dependents_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#add_dependents_for_task) | **POST** /tasks/{task_gid}/addDependents | Set dependents for a task
+*TasksApi* | [**add_followers_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#add_followers_for_task) | **POST** /tasks/{task_gid}/addFollowers | Add followers to a task
+*TasksApi* | [**add_project_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#add_project_for_task) | **POST** /tasks/{task_gid}/addProject | Add a project to a task
+*TasksApi* | [**add_tag_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#add_tag_for_task) | **POST** /tasks/{task_gid}/addTag | Add a tag to a task
+*TasksApi* | [**create_subtask_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#create_subtask_for_task) | **POST** /tasks/{task_gid}/subtasks | Create a subtask
+*TasksApi* | [**create_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#create_task) | **POST** /tasks | Create a task
+*TasksApi* | [**delete_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#delete_task) | **DELETE** /tasks/{task_gid} | Delete a task
+*TasksApi* | [**duplicate_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#duplicate_task) | **POST** /tasks/{task_gid}/duplicate | Duplicate a task
+*TasksApi* | [**get_dependencies_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_dependencies_for_task) | **GET** /tasks/{task_gid}/dependencies | Get dependencies from a task
+*TasksApi* | [**get_dependents_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_dependents_for_task) | **GET** /tasks/{task_gid}/dependents | Get dependents from a task
+*TasksApi* | [**get_subtasks_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_subtasks_for_task) | **GET** /tasks/{task_gid}/subtasks | Get subtasks from a task
+*TasksApi* | [**get_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_task) | **GET** /tasks/{task_gid} | Get a task
+*TasksApi* | [**get_task_for_custom_id**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_task_for_custom_id) | **GET** /workspaces/{workspace_gid}/tasks/custom_id/{custom_id} | Get a task for a given custom ID
+*TasksApi* | [**get_tasks**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_tasks) | **GET** /tasks | Get multiple tasks
+*TasksApi* | [**get_tasks_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_tasks_for_project) | **GET** /projects/{project_gid}/tasks | Get tasks from a project
+*TasksApi* | [**get_tasks_for_section**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_tasks_for_section) | **GET** /sections/{section_gid}/tasks | Get tasks from a section
+*TasksApi* | [**get_tasks_for_tag**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_tasks_for_tag) | **GET** /tags/{tag_gid}/tasks | Get tasks from a tag
+*TasksApi* | [**get_tasks_for_user_task_list**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_tasks_for_user_task_list) | **GET** /user_task_lists/{user_task_list_gid}/tasks | Get tasks from a user task list
+*TasksApi* | [**remove_dependencies_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#remove_dependencies_for_task) | **POST** /tasks/{task_gid}/removeDependencies | Unlink dependencies from a task
+*TasksApi* | [**remove_dependents_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#remove_dependents_for_task) | **POST** /tasks/{task_gid}/removeDependents | Unlink dependents from a task
+*TasksApi* | [**remove_follower_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#remove_follower_for_task) | **POST** /tasks/{task_gid}/removeFollowers | Remove followers from a task
+*TasksApi* | [**remove_project_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#remove_project_for_task) | **POST** /tasks/{task_gid}/removeProject | Remove a project from a task
+*TasksApi* | [**remove_tag_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#remove_tag_for_task) | **POST** /tasks/{task_gid}/removeTag | Remove a tag from a task
+*TasksApi* | [**search_tasks_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#search_tasks_for_workspace) | **GET** /workspaces/{workspace_gid}/tasks/search | Search tasks in a workspace
+*TasksApi* | [**set_parent_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#set_parent_for_task) | **POST** /tasks/{task_gid}/setParent | Set the parent of a task
+*TasksApi* | [**update_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#update_task) | **PUT** /tasks/{task_gid} | Update a task
+*TeamMembershipsApi* | [**get_team_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamMembershipsApi.md#get_team_membership) | **GET** /team_memberships/{team_membership_gid} | Get a team membership
+*TeamMembershipsApi* | [**get_team_memberships**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamMembershipsApi.md#get_team_memberships) | **GET** /team_memberships | Get team memberships
+*TeamMembershipsApi* | [**get_team_memberships_for_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamMembershipsApi.md#get_team_memberships_for_team) | **GET** /teams/{team_gid}/team_memberships | Get memberships from a team
+*TeamMembershipsApi* | [**get_team_memberships_for_user**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamMembershipsApi.md#get_team_memberships_for_user) | **GET** /users/{user_gid}/team_memberships | Get memberships from a user
+*TeamsApi* | [**add_user_for_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamsApi.md#add_user_for_team) | **POST** /teams/{team_gid}/addUser | Add a user to a team
+*TeamsApi* | [**create_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamsApi.md#create_team) | **POST** /teams | Create a team
+*TeamsApi* | [**get_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamsApi.md#get_team) | **GET** /teams/{team_gid} | Get a team
+*TeamsApi* | [**get_teams_for_user**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamsApi.md#get_teams_for_user) | **GET** /users/{user_gid}/teams | Get teams for a user
+*TeamsApi* | [**get_teams_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamsApi.md#get_teams_for_workspace) | **GET** /workspaces/{workspace_gid}/teams | Get teams in a workspace
+*TeamsApi* | [**remove_user_for_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamsApi.md#remove_user_for_team) | **POST** /teams/{team_gid}/removeUser | Remove a user from a team
+*TeamsApi* | [**update_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamsApi.md#update_team) | **PUT** /teams/{team_gid} | Update a team
+*TimePeriodsApi* | [**get_time_period**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TimePeriodsApi.md#get_time_period) | **GET** /time_periods/{time_period_gid} | Get a time period
+*TimePeriodsApi* | [**get_time_periods**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TimePeriodsApi.md#get_time_periods) | **GET** /time_periods | Get time periods
+*TimeTrackingEntriesApi* | [**create_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TimeTrackingEntriesApi.md#create_time_tracking_entry) | **POST** /tasks/{task_gid}/time_tracking_entries | Create a time tracking entry
+*TimeTrackingEntriesApi* | [**delete_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TimeTrackingEntriesApi.md#delete_time_tracking_entry) | **DELETE** /time_tracking_entries/{time_tracking_entry_gid} | Delete a time tracking entry
+*TimeTrackingEntriesApi* | [**get_time_tracking_entries_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TimeTrackingEntriesApi.md#get_time_tracking_entries_for_task) | **GET** /tasks/{task_gid}/time_tracking_entries | Get time tracking entries for a task
+*TimeTrackingEntriesApi* | [**get_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TimeTrackingEntriesApi.md#get_time_tracking_entry) | **GET** /time_tracking_entries/{time_tracking_entry_gid} | Get a time tracking entry
+*TimeTrackingEntriesApi* | [**update_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TimeTrackingEntriesApi.md#update_time_tracking_entry) | **PUT** /time_tracking_entries/{time_tracking_entry_gid} | Update a time tracking entry
+*TypeaheadApi* | [**typeahead_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TypeaheadApi.md#typeahead_for_workspace) | **GET** /workspaces/{workspace_gid}/typeahead | Get objects via typeahead
+*UserTaskListsApi* | [**get_user_task_list**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/UserTaskListsApi.md#get_user_task_list) | **GET** /user_task_lists/{user_task_list_gid} | Get a user task list
+*UserTaskListsApi* | [**get_user_task_list_for_user**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/UserTaskListsApi.md#get_user_task_list_for_user) | **GET** /users/{user_gid}/user_task_list | Get a user&#x27;s task list
+*UsersApi* | [**get_favorites_for_user**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/UsersApi.md#get_favorites_for_user) | **GET** /users/{user_gid}/favorites | Get a user&#x27;s favorites
+*UsersApi* | [**get_user**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/UsersApi.md#get_user) | **GET** /users/{user_gid} | Get a user
+*UsersApi* | [**get_users**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/UsersApi.md#get_users) | **GET** /users | Get multiple users
+*UsersApi* | [**get_users_for_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/UsersApi.md#get_users_for_team) | **GET** /teams/{team_gid}/users | Get users in a team
+*UsersApi* | [**get_users_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/UsersApi.md#get_users_for_workspace) | **GET** /workspaces/{workspace_gid}/users | Get users in a workspace or organization
+*WebhooksApi* | [**create_webhook**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WebhooksApi.md#create_webhook) | **POST** /webhooks | Establish a webhook
+*WebhooksApi* | [**delete_webhook**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WebhooksApi.md#delete_webhook) | **DELETE** /webhooks/{webhook_gid} | Delete a webhook
+*WebhooksApi* | [**get_webhook**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WebhooksApi.md#get_webhook) | **GET** /webhooks/{webhook_gid} | Get a webhook
+*WebhooksApi* | [**get_webhooks**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WebhooksApi.md#get_webhooks) | **GET** /webhooks | Get multiple webhooks
+*WebhooksApi* | [**update_webhook**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WebhooksApi.md#update_webhook) | **PUT** /webhooks/{webhook_gid} | Update a webhook
+*WorkspaceMembershipsApi* | [**get_workspace_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspaceMembershipsApi.md#get_workspace_membership) | **GET** /workspace_memberships/{workspace_membership_gid} | Get a workspace membership
+*WorkspaceMembershipsApi* | [**get_workspace_memberships_for_user**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspaceMembershipsApi.md#get_workspace_memberships_for_user) | **GET** /users/{user_gid}/workspace_memberships | Get workspace memberships for a user
+*WorkspaceMembershipsApi* | [**get_workspace_memberships_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspaceMembershipsApi.md#get_workspace_memberships_for_workspace) | **GET** /workspaces/{workspace_gid}/workspace_memberships | Get the workspace memberships for a workspace
+*WorkspacesApi* | [**add_user_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspacesApi.md#add_user_for_workspace) | **POST** /workspaces/{workspace_gid}/addUser | Add a user to a workspace or organization
+*WorkspacesApi* | [**get_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspacesApi.md#get_workspace) | **GET** /workspaces/{workspace_gid} | Get a workspace
+*WorkspacesApi* | [**get_workspaces**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspacesApi.md#get_workspaces) | **GET** /workspaces | Get multiple workspaces
+*WorkspacesApi* | [**remove_user_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspacesApi.md#remove_user_for_workspace) | **POST** /workspaces/{workspace_gid}/removeUser | Remove a user from a workspace or organization
+*WorkspacesApi* | [**update_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspacesApi.md#update_workspace) | **PUT** /workspaces/{workspace_gid} | Update a workspace
 
-## Accessing repsonse data
+## Accessing response data
 
 ### Example: Accessing task data
 ```python
 .
 .
 .
 try:
@@ -488,15 +505,15 @@
         print("Exception when calling TasksApi->create_task: %s\n" % e)
 ```
 
 ## Pagination
 
 The pagination feature is enabled by default. This means two things:
 
-1: Endpoints that return a single response (EX: [get_task](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_task) ([Get a task](https://developers.asana.com/reference/gettask)), [get_project](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_project) ([Get a project](https://developers.asana.com/reference/getproject)), etc...)
+1: Endpoints that return a single response (EX: [get_task](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_task) ([Get a task](https://developers.asana.com/reference/gettask)), [get_project](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_project) ([Get a project](https://developers.asana.com/reference/getproject)), etc...)
 will return a response with the `"data"` key abstracted from the response.
 
 Instead of returning:
 ```python
 {
     "data": {
         "gid": "123",
@@ -523,16 +540,16 @@
         "gid": "1234567",
         "name": "user@example.com",
         "resource_type": "workspace"
     }
 }
 ```
 
-2: Endpoints that return an array of resources (EX: [get_tasks](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_tasks) ([Get multiple tasks](https://developers.asana.com/reference/gettasks)), [get_projects](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#get_projects) ([Get multiple projects](https://developers.asana.com/reference/getprojects)), etc...)
-will return a generator object ([PageIterator.items](https://github.com/Asana/python-asana/blob/v5.0.5/asana/pagination/page_iterator.py)) that you can use to iterate through each result.
+2: Endpoints that return an array of resources (EX: [get_tasks](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_tasks) ([Get multiple tasks](https://developers.asana.com/reference/gettasks)), [get_projects](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#get_projects) ([Get multiple projects](https://developers.asana.com/reference/getprojects)), etc...)
+will return a generator object ([PageIterator.items](https://github.com/Asana/python-asana/blob/v5.0.6/asana/pagination/page_iterator.py)) that you can use to iterate through each result.
 
 Example usage 1:
 ```python
 import asana
 from asana.rest import ApiException
 from pprint import pprint
```

### Comparing `asana-5.0.5/asana/__init__.py` & `asana-5.0.6/asana/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import apis into sdk package
+from asana.api.allocations_api import AllocationsApi
 from asana.api.attachments_api import AttachmentsApi
 from asana.api.audit_log_api_api import AuditLogAPIApi
 from asana.api.batch_api_api import BatchAPIApi
 from asana.api.custom_field_settings_api import CustomFieldSettingsApi
 from asana.api.custom_fields_api import CustomFieldsApi
 from asana.api.events_api import EventsApi
 from asana.api.goal_relationships_api import GoalRelationshipsApi
```

### Comparing `asana-5.0.5/asana/api/__init__.py` & `asana-5.0.6/asana/api/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import absolute_import
 
 # flake8: noqa
 
 # import apis into api package
+from asana.api.allocations_api import AllocationsApi
 from asana.api.attachments_api import AttachmentsApi
 from asana.api.audit_log_api_api import AuditLogAPIApi
 from asana.api.batch_api_api import BatchAPIApi
 from asana.api.custom_field_settings_api import CustomFieldSettingsApi
 from asana.api.custom_fields_api import CustomFieldsApi
 from asana.api.events_api import EventsApi
 from asana.api.goal_relationships_api import GoalRelationshipsApi
```

### Comparing `asana-5.0.5/asana/api/attachments_api.py` & `asana-5.0.6/asana/api/attachments_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/audit_log_api_api.py` & `asana-5.0.6/asana/api/audit_log_api_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/batch_api_api.py` & `asana-5.0.6/asana/api/batch_api_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/custom_field_settings_api.py` & `asana-5.0.6/asana/api/custom_field_settings_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/custom_fields_api.py` & `asana-5.0.6/asana/api/custom_fields_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/events_api.py` & `asana-5.0.6/asana/api/events_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/goal_relationships_api.py` & `asana-5.0.6/asana/api/goal_relationships_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/goals_api.py` & `asana-5.0.6/asana/api/goals_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/jobs_api.py` & `asana-5.0.6/asana/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/memberships_api.py` & `asana-5.0.6/asana/api/memberships_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create_membership(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param dict body: The updated fields for the membership.
-        :return: MembershipResponseArray
+        :return: MembershipResponseData
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = kwargs.get("_return_http_data_only", True)
         if kwargs.get('async_req'):
             return self.create_membership_with_http_info(opts, **kwargs)  # noqa: E501
         else:
@@ -61,15 +61,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create_membership_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param dict body: The updated fields for the membership.
-        :return: MembershipResponseArray
+        :return: MembershipResponseData
                  If the method is called asynchronously,
                  returns the request thread.
         """
         all_params = []
         all_params.append('async_req')
         all_params.append('header_params')
         all_params.append('_return_http_data_only')
@@ -129,36 +129,33 @@
                 async_req=params.get('async_req'),
                 _return_http_data_only=params.get('_return_http_data_only'),
                 _preload_content=params.get('_preload_content', True),
                 _request_timeout=params.get('_request_timeout'),
                 collection_formats=collection_formats
             )
         elif self.api_client.configuration.return_page_iterator:
-            query_params["limit"] = query_params.get("limit", self.api_client.configuration.page_limit)
-            return PageIterator(
-                self.api_client,
-                {
-                    "resource_path": '/memberships',
-                    "method": 'POST',
-                    "path_params": path_params,
-                    "query_params": query_params,
-                    "header_params": header_params,
-                    "body": body_params,
-                    "post_params": form_params,
-                    "files": local_var_files,
-                    "response_type": object,
-                    "auth_settings": auth_settings,
-                    "async_req": params.get('async_req'),
-                    "_return_http_data_only": params.get('_return_http_data_only'),
-                    "_preload_content": params.get('_preload_content', True),
-                    "_request_timeout": params.get('_request_timeout'),
-                    "collection_formats": collection_formats
-                },
-                **kwargs
-            ).items()
+            (data) = self.api_client.call_api(
+                '/memberships', 'POST',
+                path_params,
+                query_params,
+                header_params,
+                body=body_params,
+                post_params=form_params,
+                files=local_var_files,
+                response_type=object,  # noqa: E501
+                auth_settings=auth_settings,
+                async_req=params.get('async_req'),
+                _return_http_data_only=params.get('_return_http_data_only'),
+                _preload_content=params.get('_preload_content', True),
+                _request_timeout=params.get('_request_timeout'),
+                collection_formats=collection_formats
+            )
+            if params.get('_return_http_data_only') == False:
+                return data
+            return data["data"] if data else data
         else:
             return self.api_client.call_api(
             '/memberships', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -580,13 +577,158 @@
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=object,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def update_membership(self, body, membership_gid, **kwargs):  # noqa: E501
+        """Update a membership  # noqa: E501
+
+        An existing membership can be updated by making a `PUT` request on the URL for that goal. Only the fields provided in the `data` block will be updated; any unspecified fields will remain unchanged. Memberships on `goals` and `projects` can be updated.  Returns the full record of the updated membership.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.update_membership(body, membership_gid, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param dict body: The membership to update. (required)
+        :param str membership_gid: Globally unique identifier for the membership. (required)
+        :return: MembershipResponseData
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = kwargs.get("_return_http_data_only", True)
+        if kwargs.get('async_req'):
+            return self.update_membership_with_http_info(body, membership_gid, **kwargs)  # noqa: E501
+        else:
+            (data) = self.update_membership_with_http_info(body, membership_gid, **kwargs)  # noqa: E501
+            return data
+
+    def update_membership_with_http_info(self, body, membership_gid, **kwargs):  # noqa: E501
+        """Update a membership  # noqa: E501
+
+        An existing membership can be updated by making a `PUT` request on the URL for that goal. Only the fields provided in the `data` block will be updated; any unspecified fields will remain unchanged. Memberships on `goals` and `projects` can be updated.  Returns the full record of the updated membership.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.update_membership_with_http_info(body, membership_gid, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param dict body: The membership to update. (required)
+        :param str membership_gid: Globally unique identifier for the membership. (required)
+        :return: MembershipResponseData
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        all_params = []
+        all_params.append('async_req')
+        all_params.append('header_params')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+        all_params.append('full_payload')
+        all_params.append('item_limit')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method update_membership" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'body' is set
+        if (body is None):
+            raise ValueError("Missing the required parameter `body` when calling `update_membership`")  # noqa: E501
+        # verify the required parameter 'membership_gid' is set
+        if (membership_gid is None):
+            raise ValueError("Missing the required parameter `membership_gid` when calling `update_membership`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['membership_gid'] = membership_gid  # noqa: E501
+
+        query_params = {}
+
+
+        header_params = kwargs.get("header_params", {})
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = body
+
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json; charset=UTF-8'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json; charset=UTF-8'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['personalAccessToken']  # noqa: E501
+
+        # hard checking for True boolean value because user can provide full_payload or async_req with any data type
+        if kwargs.get("full_payload", False) is True or kwargs.get('async_req', False) is True:
+            return self.api_client.call_api(
+                '/memberships/{membership_gid}', 'PUT',
+                path_params,
+                query_params,
+                header_params,
+                body=body_params,
+                post_params=form_params,
+                files=local_var_files,
+                response_type=object,  # noqa: E501
+                auth_settings=auth_settings,
+                async_req=params.get('async_req'),
+                _return_http_data_only=params.get('_return_http_data_only'),
+                _preload_content=params.get('_preload_content', True),
+                _request_timeout=params.get('_request_timeout'),
+                collection_formats=collection_formats
+            )
+        elif self.api_client.configuration.return_page_iterator:
+            (data) = self.api_client.call_api(
+                '/memberships/{membership_gid}', 'PUT',
+                path_params,
+                query_params,
+                header_params,
+                body=body_params,
+                post_params=form_params,
+                files=local_var_files,
+                response_type=object,  # noqa: E501
+                auth_settings=auth_settings,
+                async_req=params.get('async_req'),
+                _return_http_data_only=params.get('_return_http_data_only'),
+                _preload_content=params.get('_preload_content', True),
+                _request_timeout=params.get('_request_timeout'),
+                collection_formats=collection_formats
+            )
+            if params.get('_return_http_data_only') == False:
+                return data
+            return data["data"] if data else data
+        else:
+            return self.api_client.call_api(
+            '/memberships/{membership_gid}', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=object,  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `asana-5.0.5/asana/api/organization_exports_api.py` & `asana-5.0.6/asana/api/organization_exports_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/portfolio_memberships_api.py` & `asana-5.0.6/asana/api/portfolio_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/portfolios_api.py` & `asana-5.0.6/asana/api/portfolios_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/project_briefs_api.py` & `asana-5.0.6/asana/api/project_briefs_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/project_memberships_api.py` & `asana-5.0.6/asana/api/project_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/project_statuses_api.py` & `asana-5.0.6/asana/api/project_statuses_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/project_templates_api.py` & `asana-5.0.6/asana/api/project_templates_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/projects_api.py` & `asana-5.0.6/asana/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/rules_api.py` & `asana-5.0.6/asana/api/rules_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/sections_api.py` & `asana-5.0.6/asana/api/sections_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/status_updates_api.py` & `asana-5.0.6/asana/api/status_updates_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/stories_api.py` & `asana-5.0.6/asana/api/stories_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/tags_api.py` & `asana-5.0.6/asana/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/task_templates_api.py` & `asana-5.0.6/asana/api/task_templates_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/tasks_api.py` & `asana-5.0.6/asana/api/tasks_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/team_memberships_api.py` & `asana-5.0.6/asana/api/team_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/teams_api.py` & `asana-5.0.6/asana/api/teams_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/time_periods_api.py` & `asana-5.0.6/asana/api/time_periods_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/time_tracking_entries_api.py` & `asana-5.0.6/asana/api/time_tracking_entries_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/typeahead_api.py` & `asana-5.0.6/asana/api/typeahead_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/user_task_lists_api.py` & `asana-5.0.6/asana/api/user_task_lists_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/users_api.py` & `asana-5.0.6/asana/api/users_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/webhooks_api.py` & `asana-5.0.6/asana/api/webhooks_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/workspace_memberships_api.py` & `asana-5.0.6/asana/api/workspace_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api/workspaces_api.py` & `asana-5.0.6/asana/api/workspaces_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/api_client.py` & `asana-5.0.6/asana/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,20 +74,20 @@
             logging.warning('Looks like your system does not support ThreadPool but it will try without it if you do not use async requests')
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/5.0.5/python'
+        self.user_agent = 'Swagger-Codegen/5.0.6/python'
         # Add custom header
         self.default_headers['X-Asana-Client-Lib'] = urlencode(
             {
                 'language': 'Python',
-                'version': '5.0.5',
+                'version': '5.0.6',
                 'language_version': platform.python_version(),
                 'os': platform.system(),
                 'os_version': platform.release()
             }
         )
 
     def __del__(self):
```

### Comparing `asana-5.0.5/asana/configuration.py` & `asana-5.0.6/asana/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,16 @@
         self.api_key_prefix = {}
         # function to refresh API key if expired
         self.refresh_api_key_hook = None
         # Username for HTTP basic authentication
         self.username = ""
         # Password for HTTP basic authentication
         self.password = ""
+        # access token for OAuth
+        self.access_token = ""
         # Logging Settings
         self.logger = {}
         self.logger["package_logger"] = logging.getLogger("asana")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         # Log format
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         # Log stream handler
@@ -252,9 +254,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0\n"\
-               "SDK Package Version: 5.0.5".\
+               "SDK Package Version: 5.0.6".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `asana-5.0.5/asana/pagination/__init__.py` & `asana-5.0.6/asana/pagination/__init__.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/pagination/event_iterator.py` & `asana-5.0.6/asana/pagination/event_iterator.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/pagination/page_iterator.py` & `asana-5.0.6/asana/pagination/page_iterator.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana/rest.py` & `asana-5.0.6/asana/rest.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/asana.egg-info/PKG-INFO` & `asana-5.0.6/asana.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: asana
-Version: 5.0.5
+Version: 5.0.6
 Summary: Asana
 Home-page: http://github.com/asana/python-asana
 Author: Asana, Inc
 License: MIT
 Keywords: asana,Asana
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # asana [![GitHub release][release-image]]() [![PyPi Version][pypi-image]][pypi-url]
 
 - API version: 1.0
-- Package version: 5.0.5
+- Package version: 5.0.6
 
 ## Requirements.
 
 Python 3.4+
 
 ## Installation & Usage
 ### pip install from [PyPI](https://pypi.org/project/asana/)
@@ -185,199 +185,205 @@
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://app.asana.com/api/1.0*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
-*AttachmentsApi* | [**create_attachment_for_object**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/AttachmentsApi.md#create_attachment_for_object) | **POST** /attachments | Upload an attachment
-*AttachmentsApi* | [**delete_attachment**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/AttachmentsApi.md#delete_attachment) | **DELETE** /attachments/{attachment_gid} | Delete an attachment
-*AttachmentsApi* | [**get_attachment**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/AttachmentsApi.md#get_attachment) | **GET** /attachments/{attachment_gid} | Get an attachment
-*AttachmentsApi* | [**get_attachments_for_object**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/AttachmentsApi.md#get_attachments_for_object) | **GET** /attachments | Get attachments from an object
-*AuditLogAPIApi* | [**get_audit_log_events**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/AuditLogAPIApi.md#get_audit_log_events) | **GET** /workspaces/{workspace_gid}/audit_log_events | Get audit log events
-*BatchAPIApi* | [**create_batch_request**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/BatchAPIApi.md#create_batch_request) | **POST** /batch | Submit parallel requests
-*CustomFieldSettingsApi* | [**get_custom_field_settings_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldSettingsApi.md#get_custom_field_settings_for_portfolio) | **GET** /portfolios/{portfolio_gid}/custom_field_settings | Get a portfolio&#x27;s custom fields
-*CustomFieldSettingsApi* | [**get_custom_field_settings_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldSettingsApi.md#get_custom_field_settings_for_project) | **GET** /projects/{project_gid}/custom_field_settings | Get a project&#x27;s custom fields
-*CustomFieldsApi* | [**create_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#create_custom_field) | **POST** /custom_fields | Create a custom field
-*CustomFieldsApi* | [**create_enum_option_for_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#create_enum_option_for_custom_field) | **POST** /custom_fields/{custom_field_gid}/enum_options | Create an enum option
-*CustomFieldsApi* | [**delete_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#delete_custom_field) | **DELETE** /custom_fields/{custom_field_gid} | Delete a custom field
-*CustomFieldsApi* | [**get_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#get_custom_field) | **GET** /custom_fields/{custom_field_gid} | Get a custom field
-*CustomFieldsApi* | [**get_custom_fields_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#get_custom_fields_for_workspace) | **GET** /workspaces/{workspace_gid}/custom_fields | Get a workspace&#x27;s custom fields
-*CustomFieldsApi* | [**insert_enum_option_for_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#insert_enum_option_for_custom_field) | **POST** /custom_fields/{custom_field_gid}/enum_options/insert | Reorder a custom field&#x27;s enum
-*CustomFieldsApi* | [**update_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#update_custom_field) | **PUT** /custom_fields/{custom_field_gid} | Update a custom field
-*CustomFieldsApi* | [**update_enum_option**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/CustomFieldsApi.md#update_enum_option) | **PUT** /enum_options/{enum_option_gid} | Update an enum option
-*EventsApi* | [**get_events**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/EventsApi.md#get_events) | **GET** /events | Get events on a resource
-*GoalRelationshipsApi* | [**add_supporting_relationship**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalRelationshipsApi.md#add_supporting_relationship) | **POST** /goals/{goal_gid}/addSupportingRelationship | Add a supporting goal relationship
-*GoalRelationshipsApi* | [**get_goal_relationship**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalRelationshipsApi.md#get_goal_relationship) | **GET** /goal_relationships/{goal_relationship_gid} | Get a goal relationship
-*GoalRelationshipsApi* | [**get_goal_relationships**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalRelationshipsApi.md#get_goal_relationships) | **GET** /goal_relationships | Get goal relationships
-*GoalRelationshipsApi* | [**remove_supporting_relationship**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalRelationshipsApi.md#remove_supporting_relationship) | **POST** /goals/{goal_gid}/removeSupportingRelationship | Removes a supporting goal relationship
-*GoalRelationshipsApi* | [**update_goal_relationship**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalRelationshipsApi.md#update_goal_relationship) | **PUT** /goal_relationships/{goal_relationship_gid} | Update a goal relationship
-*GoalsApi* | [**add_followers**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#add_followers) | **POST** /goals/{goal_gid}/addFollowers | Add a collaborator to a goal
-*GoalsApi* | [**create_goal**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#create_goal) | **POST** /goals | Create a goal
-*GoalsApi* | [**create_goal_metric**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#create_goal_metric) | **POST** /goals/{goal_gid}/setMetric | Create a goal metric
-*GoalsApi* | [**delete_goal**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#delete_goal) | **DELETE** /goals/{goal_gid} | Delete a goal
-*GoalsApi* | [**get_goal**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#get_goal) | **GET** /goals/{goal_gid} | Get a goal
-*GoalsApi* | [**get_goals**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#get_goals) | **GET** /goals | Get goals
-*GoalsApi* | [**get_parent_goals_for_goal**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#get_parent_goals_for_goal) | **GET** /goals/{goal_gid}/parentGoals | Get parent goals from a goal
-*GoalsApi* | [**remove_followers**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#remove_followers) | **POST** /goals/{goal_gid}/removeFollowers | Remove a collaborator from a goal
-*GoalsApi* | [**update_goal**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#update_goal) | **PUT** /goals/{goal_gid} | Update a goal
-*GoalsApi* | [**update_goal_metric**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/GoalsApi.md#update_goal_metric) | **POST** /goals/{goal_gid}/setMetricCurrentValue | Update a goal metric
-*JobsApi* | [**get_job**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/JobsApi.md#get_job) | **GET** /jobs/{job_gid} | Get a job by id
-*MembershipsApi* | [**create_membership**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/MembershipsApi.md#create_membership) | **POST** /memberships | Create a membership
-*MembershipsApi* | [**delete_membership**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/MembershipsApi.md#delete_membership) | **DELETE** /memberships/{membership_gid} | Delete a membership
-*MembershipsApi* | [**get_membership**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/MembershipsApi.md#get_membership) | **GET** /memberships/{membership_gid} | Get a membership
-*MembershipsApi* | [**get_memberships**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/MembershipsApi.md#get_memberships) | **GET** /memberships | Get multiple memberships
-*OrganizationExportsApi* | [**create_organization_export**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/OrganizationExportsApi.md#create_organization_export) | **POST** /organization_exports | Create an organization export request
-*OrganizationExportsApi* | [**get_organization_export**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/OrganizationExportsApi.md#get_organization_export) | **GET** /organization_exports/{organization_export_gid} | Get details on an org export request
-*PortfolioMembershipsApi* | [**get_portfolio_membership**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfolioMembershipsApi.md#get_portfolio_membership) | **GET** /portfolio_memberships/{portfolio_membership_gid} | Get a portfolio membership
-*PortfolioMembershipsApi* | [**get_portfolio_memberships**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfolioMembershipsApi.md#get_portfolio_memberships) | **GET** /portfolio_memberships | Get multiple portfolio memberships
-*PortfolioMembershipsApi* | [**get_portfolio_memberships_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfolioMembershipsApi.md#get_portfolio_memberships_for_portfolio) | **GET** /portfolios/{portfolio_gid}/portfolio_memberships | Get memberships from a portfolio
-*PortfoliosApi* | [**add_custom_field_setting_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#add_custom_field_setting_for_portfolio) | **POST** /portfolios/{portfolio_gid}/addCustomFieldSetting | Add a custom field to a portfolio
-*PortfoliosApi* | [**add_item_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#add_item_for_portfolio) | **POST** /portfolios/{portfolio_gid}/addItem | Add a portfolio item
-*PortfoliosApi* | [**add_members_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#add_members_for_portfolio) | **POST** /portfolios/{portfolio_gid}/addMembers | Add users to a portfolio
-*PortfoliosApi* | [**create_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#create_portfolio) | **POST** /portfolios | Create a portfolio
-*PortfoliosApi* | [**delete_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#delete_portfolio) | **DELETE** /portfolios/{portfolio_gid} | Delete a portfolio
-*PortfoliosApi* | [**get_items_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#get_items_for_portfolio) | **GET** /portfolios/{portfolio_gid}/items | Get portfolio items
-*PortfoliosApi* | [**get_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#get_portfolio) | **GET** /portfolios/{portfolio_gid} | Get a portfolio
-*PortfoliosApi* | [**get_portfolios**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#get_portfolios) | **GET** /portfolios | Get multiple portfolios
-*PortfoliosApi* | [**remove_custom_field_setting_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#remove_custom_field_setting_for_portfolio) | **POST** /portfolios/{portfolio_gid}/removeCustomFieldSetting | Remove a custom field from a portfolio
-*PortfoliosApi* | [**remove_item_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#remove_item_for_portfolio) | **POST** /portfolios/{portfolio_gid}/removeItem | Remove a portfolio item
-*PortfoliosApi* | [**remove_members_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#remove_members_for_portfolio) | **POST** /portfolios/{portfolio_gid}/removeMembers | Remove users from a portfolio
-*PortfoliosApi* | [**update_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/PortfoliosApi.md#update_portfolio) | **PUT** /portfolios/{portfolio_gid} | Update a portfolio
-*ProjectBriefsApi* | [**create_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectBriefsApi.md#create_project_brief) | **POST** /projects/{project_gid}/project_briefs | Create a project brief
-*ProjectBriefsApi* | [**delete_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectBriefsApi.md#delete_project_brief) | **DELETE** /project_briefs/{project_brief_gid} | Delete a project brief
-*ProjectBriefsApi* | [**get_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectBriefsApi.md#get_project_brief) | **GET** /project_briefs/{project_brief_gid} | Get a project brief
-*ProjectBriefsApi* | [**update_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectBriefsApi.md#update_project_brief) | **PUT** /project_briefs/{project_brief_gid} | Update a project brief
-*ProjectMembershipsApi* | [**get_project_membership**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectMembershipsApi.md#get_project_membership) | **GET** /project_memberships/{project_membership_gid} | Get a project membership
-*ProjectMembershipsApi* | [**get_project_memberships_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectMembershipsApi.md#get_project_memberships_for_project) | **GET** /projects/{project_gid}/project_memberships | Get memberships from a project
-*ProjectStatusesApi* | [**create_project_status_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectStatusesApi.md#create_project_status_for_project) | **POST** /projects/{project_gid}/project_statuses | Create a project status
-*ProjectStatusesApi* | [**delete_project_status**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectStatusesApi.md#delete_project_status) | **DELETE** /project_statuses/{project_status_gid} | Delete a project status
-*ProjectStatusesApi* | [**get_project_status**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectStatusesApi.md#get_project_status) | **GET** /project_statuses/{project_status_gid} | Get a project status
-*ProjectStatusesApi* | [**get_project_statuses_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectStatusesApi.md#get_project_statuses_for_project) | **GET** /projects/{project_gid}/project_statuses | Get statuses from a project
-*ProjectTemplatesApi* | [**delete_project_template**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectTemplatesApi.md#delete_project_template) | **DELETE** /project_templates/{project_template_gid} | Delete a project template
-*ProjectTemplatesApi* | [**get_project_template**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectTemplatesApi.md#get_project_template) | **GET** /project_templates/{project_template_gid} | Get a project template
-*ProjectTemplatesApi* | [**get_project_templates**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectTemplatesApi.md#get_project_templates) | **GET** /project_templates | Get multiple project templates
-*ProjectTemplatesApi* | [**get_project_templates_for_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectTemplatesApi.md#get_project_templates_for_team) | **GET** /teams/{team_gid}/project_templates | Get a team&#x27;s project templates
-*ProjectTemplatesApi* | [**instantiate_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectTemplatesApi.md#instantiate_project) | **POST** /project_templates/{project_template_gid}/instantiateProject | Instantiate a project from a project template
-*ProjectsApi* | [**add_custom_field_setting_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#add_custom_field_setting_for_project) | **POST** /projects/{project_gid}/addCustomFieldSetting | Add a custom field to a project
-*ProjectsApi* | [**add_followers_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#add_followers_for_project) | **POST** /projects/{project_gid}/addFollowers | Add followers to a project
-*ProjectsApi* | [**add_members_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#add_members_for_project) | **POST** /projects/{project_gid}/addMembers | Add users to a project
-*ProjectsApi* | [**create_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#create_project) | **POST** /projects | Create a project
-*ProjectsApi* | [**create_project_for_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#create_project_for_team) | **POST** /teams/{team_gid}/projects | Create a project in a team
-*ProjectsApi* | [**create_project_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#create_project_for_workspace) | **POST** /workspaces/{workspace_gid}/projects | Create a project in a workspace
-*ProjectsApi* | [**delete_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#delete_project) | **DELETE** /projects/{project_gid} | Delete a project
-*ProjectsApi* | [**duplicate_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#duplicate_project) | **POST** /projects/{project_gid}/duplicate | Duplicate a project
-*ProjectsApi* | [**get_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#get_project) | **GET** /projects/{project_gid} | Get a project
-*ProjectsApi* | [**get_projects**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#get_projects) | **GET** /projects | Get multiple projects
-*ProjectsApi* | [**get_projects_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#get_projects_for_task) | **GET** /tasks/{task_gid}/projects | Get projects a task is in
-*ProjectsApi* | [**get_projects_for_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#get_projects_for_team) | **GET** /teams/{team_gid}/projects | Get a team&#x27;s projects
-*ProjectsApi* | [**get_projects_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#get_projects_for_workspace) | **GET** /workspaces/{workspace_gid}/projects | Get all projects in a workspace
-*ProjectsApi* | [**get_task_counts_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#get_task_counts_for_project) | **GET** /projects/{project_gid}/task_counts | Get task count of a project
-*ProjectsApi* | [**project_save_as_template**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#project_save_as_template) | **POST** /projects/{project_gid}/saveAsTemplate | Create a project template from a project
-*ProjectsApi* | [**remove_custom_field_setting_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#remove_custom_field_setting_for_project) | **POST** /projects/{project_gid}/removeCustomFieldSetting | Remove a custom field from a project
-*ProjectsApi* | [**remove_followers_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#remove_followers_for_project) | **POST** /projects/{project_gid}/removeFollowers | Remove followers from a project
-*ProjectsApi* | [**remove_members_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#remove_members_for_project) | **POST** /projects/{project_gid}/removeMembers | Remove users from a project
-*ProjectsApi* | [**update_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#update_project) | **PUT** /projects/{project_gid} | Update a project
-*RulesApi* | [**trigger_rule**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/RulesApi.md#trigger_rule) | **POST** /rule_triggers/{rule_trigger_gid}/run | Trigger a rule
-*SectionsApi* | [**add_task_for_section**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/SectionsApi.md#add_task_for_section) | **POST** /sections/{section_gid}/addTask | Add task to section
-*SectionsApi* | [**create_section_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/SectionsApi.md#create_section_for_project) | **POST** /projects/{project_gid}/sections | Create a section in a project
-*SectionsApi* | [**delete_section**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/SectionsApi.md#delete_section) | **DELETE** /sections/{section_gid} | Delete a section
-*SectionsApi* | [**get_section**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/SectionsApi.md#get_section) | **GET** /sections/{section_gid} | Get a section
-*SectionsApi* | [**get_sections_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/SectionsApi.md#get_sections_for_project) | **GET** /projects/{project_gid}/sections | Get sections in a project
-*SectionsApi* | [**insert_section_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/SectionsApi.md#insert_section_for_project) | **POST** /projects/{project_gid}/sections/insert | Move or Insert sections
-*SectionsApi* | [**update_section**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/SectionsApi.md#update_section) | **PUT** /sections/{section_gid} | Update a section
-*StatusUpdatesApi* | [**create_status_for_object**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StatusUpdatesApi.md#create_status_for_object) | **POST** /status_updates | Create a status update
-*StatusUpdatesApi* | [**delete_status**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StatusUpdatesApi.md#delete_status) | **DELETE** /status_updates/{status_update_gid} | Delete a status update
-*StatusUpdatesApi* | [**get_status**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StatusUpdatesApi.md#get_status) | **GET** /status_updates/{status_update_gid} | Get a status update
-*StatusUpdatesApi* | [**get_statuses_for_object**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StatusUpdatesApi.md#get_statuses_for_object) | **GET** /status_updates | Get status updates from an object
-*StoriesApi* | [**create_story_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StoriesApi.md#create_story_for_task) | **POST** /tasks/{task_gid}/stories | Create a story on a task
-*StoriesApi* | [**delete_story**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StoriesApi.md#delete_story) | **DELETE** /stories/{story_gid} | Delete a story
-*StoriesApi* | [**get_stories_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StoriesApi.md#get_stories_for_task) | **GET** /tasks/{task_gid}/stories | Get stories from a task
-*StoriesApi* | [**get_story**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StoriesApi.md#get_story) | **GET** /stories/{story_gid} | Get a story
-*StoriesApi* | [**update_story**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/StoriesApi.md#update_story) | **PUT** /stories/{story_gid} | Update a story
-*TagsApi* | [**create_tag**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#create_tag) | **POST** /tags | Create a tag
-*TagsApi* | [**create_tag_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#create_tag_for_workspace) | **POST** /workspaces/{workspace_gid}/tags | Create a tag in a workspace
-*TagsApi* | [**delete_tag**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#delete_tag) | **DELETE** /tags/{tag_gid} | Delete a tag
-*TagsApi* | [**get_tag**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#get_tag) | **GET** /tags/{tag_gid} | Get a tag
-*TagsApi* | [**get_tags**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#get_tags) | **GET** /tags | Get multiple tags
-*TagsApi* | [**get_tags_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#get_tags_for_task) | **GET** /tasks/{task_gid}/tags | Get a task&#x27;s tags
-*TagsApi* | [**get_tags_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#get_tags_for_workspace) | **GET** /workspaces/{workspace_gid}/tags | Get tags in a workspace
-*TagsApi* | [**update_tag**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TagsApi.md#update_tag) | **PUT** /tags/{tag_gid} | Update a tag
-*TaskTemplatesApi* | [**delete_task_template**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TaskTemplatesApi.md#delete_task_template) | **DELETE** /task_templates/{task_template_gid} | Delete a task template
-*TaskTemplatesApi* | [**get_task_template**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TaskTemplatesApi.md#get_task_template) | **GET** /task_templates/{task_template_gid} | Get a task template
-*TaskTemplatesApi* | [**get_task_templates**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TaskTemplatesApi.md#get_task_templates) | **GET** /task_templates | Get multiple task templates
-*TaskTemplatesApi* | [**instantiate_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TaskTemplatesApi.md#instantiate_task) | **POST** /task_templates/{task_template_gid}/instantiateTask | Instantiate a task from a task template
-*TasksApi* | [**add_dependencies_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#add_dependencies_for_task) | **POST** /tasks/{task_gid}/addDependencies | Set dependencies for a task
-*TasksApi* | [**add_dependents_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#add_dependents_for_task) | **POST** /tasks/{task_gid}/addDependents | Set dependents for a task
-*TasksApi* | [**add_followers_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#add_followers_for_task) | **POST** /tasks/{task_gid}/addFollowers | Add followers to a task
-*TasksApi* | [**add_project_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#add_project_for_task) | **POST** /tasks/{task_gid}/addProject | Add a project to a task
-*TasksApi* | [**add_tag_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#add_tag_for_task) | **POST** /tasks/{task_gid}/addTag | Add a tag to a task
-*TasksApi* | [**create_subtask_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#create_subtask_for_task) | **POST** /tasks/{task_gid}/subtasks | Create a subtask
-*TasksApi* | [**create_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#create_task) | **POST** /tasks | Create a task
-*TasksApi* | [**delete_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#delete_task) | **DELETE** /tasks/{task_gid} | Delete a task
-*TasksApi* | [**duplicate_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#duplicate_task) | **POST** /tasks/{task_gid}/duplicate | Duplicate a task
-*TasksApi* | [**get_dependencies_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_dependencies_for_task) | **GET** /tasks/{task_gid}/dependencies | Get dependencies from a task
-*TasksApi* | [**get_dependents_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_dependents_for_task) | **GET** /tasks/{task_gid}/dependents | Get dependents from a task
-*TasksApi* | [**get_subtasks_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_subtasks_for_task) | **GET** /tasks/{task_gid}/subtasks | Get subtasks from a task
-*TasksApi* | [**get_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_task) | **GET** /tasks/{task_gid} | Get a task
-*TasksApi* | [**get_task_for_custom_id**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_task_for_custom_id) | **GET** /workspaces/{workspace_gid}/tasks/custom_id/{custom_id} | Get a task for a given custom ID
-*TasksApi* | [**get_tasks**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_tasks) | **GET** /tasks | Get multiple tasks
-*TasksApi* | [**get_tasks_for_project**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_tasks_for_project) | **GET** /projects/{project_gid}/tasks | Get tasks from a project
-*TasksApi* | [**get_tasks_for_section**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_tasks_for_section) | **GET** /sections/{section_gid}/tasks | Get tasks from a section
-*TasksApi* | [**get_tasks_for_tag**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_tasks_for_tag) | **GET** /tags/{tag_gid}/tasks | Get tasks from a tag
-*TasksApi* | [**get_tasks_for_user_task_list**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_tasks_for_user_task_list) | **GET** /user_task_lists/{user_task_list_gid}/tasks | Get tasks from a user task list
-*TasksApi* | [**remove_dependencies_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#remove_dependencies_for_task) | **POST** /tasks/{task_gid}/removeDependencies | Unlink dependencies from a task
-*TasksApi* | [**remove_dependents_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#remove_dependents_for_task) | **POST** /tasks/{task_gid}/removeDependents | Unlink dependents from a task
-*TasksApi* | [**remove_follower_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#remove_follower_for_task) | **POST** /tasks/{task_gid}/removeFollowers | Remove followers from a task
-*TasksApi* | [**remove_project_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#remove_project_for_task) | **POST** /tasks/{task_gid}/removeProject | Remove a project from a task
-*TasksApi* | [**remove_tag_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#remove_tag_for_task) | **POST** /tasks/{task_gid}/removeTag | Remove a tag from a task
-*TasksApi* | [**search_tasks_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#search_tasks_for_workspace) | **GET** /workspaces/{workspace_gid}/tasks/search | Search tasks in a workspace
-*TasksApi* | [**set_parent_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#set_parent_for_task) | **POST** /tasks/{task_gid}/setParent | Set the parent of a task
-*TasksApi* | [**update_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#update_task) | **PUT** /tasks/{task_gid} | Update a task
-*TeamMembershipsApi* | [**get_team_membership**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamMembershipsApi.md#get_team_membership) | **GET** /team_memberships/{team_membership_gid} | Get a team membership
-*TeamMembershipsApi* | [**get_team_memberships**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamMembershipsApi.md#get_team_memberships) | **GET** /team_memberships | Get team memberships
-*TeamMembershipsApi* | [**get_team_memberships_for_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamMembershipsApi.md#get_team_memberships_for_team) | **GET** /teams/{team_gid}/team_memberships | Get memberships from a team
-*TeamMembershipsApi* | [**get_team_memberships_for_user**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamMembershipsApi.md#get_team_memberships_for_user) | **GET** /users/{user_gid}/team_memberships | Get memberships from a user
-*TeamsApi* | [**add_user_for_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamsApi.md#add_user_for_team) | **POST** /teams/{team_gid}/addUser | Add a user to a team
-*TeamsApi* | [**create_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamsApi.md#create_team) | **POST** /teams | Create a team
-*TeamsApi* | [**get_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamsApi.md#get_team) | **GET** /teams/{team_gid} | Get a team
-*TeamsApi* | [**get_teams_for_user**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamsApi.md#get_teams_for_user) | **GET** /users/{user_gid}/teams | Get teams for a user
-*TeamsApi* | [**get_teams_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamsApi.md#get_teams_for_workspace) | **GET** /workspaces/{workspace_gid}/teams | Get teams in a workspace
-*TeamsApi* | [**remove_user_for_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamsApi.md#remove_user_for_team) | **POST** /teams/{team_gid}/removeUser | Remove a user from a team
-*TeamsApi* | [**update_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TeamsApi.md#update_team) | **PUT** /teams/{team_gid} | Update a team
-*TimePeriodsApi* | [**get_time_period**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TimePeriodsApi.md#get_time_period) | **GET** /time_periods/{time_period_gid} | Get a time period
-*TimePeriodsApi* | [**get_time_periods**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TimePeriodsApi.md#get_time_periods) | **GET** /time_periods | Get time periods
-*TimeTrackingEntriesApi* | [**create_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TimeTrackingEntriesApi.md#create_time_tracking_entry) | **POST** /tasks/{task_gid}/time_tracking_entries | Create a time tracking entry
-*TimeTrackingEntriesApi* | [**delete_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TimeTrackingEntriesApi.md#delete_time_tracking_entry) | **DELETE** /time_tracking_entries/{time_tracking_entry_gid} | Delete a time tracking entry
-*TimeTrackingEntriesApi* | [**get_time_tracking_entries_for_task**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TimeTrackingEntriesApi.md#get_time_tracking_entries_for_task) | **GET** /tasks/{task_gid}/time_tracking_entries | Get time tracking entries for a task
-*TimeTrackingEntriesApi* | [**get_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TimeTrackingEntriesApi.md#get_time_tracking_entry) | **GET** /time_tracking_entries/{time_tracking_entry_gid} | Get a time tracking entry
-*TimeTrackingEntriesApi* | [**update_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TimeTrackingEntriesApi.md#update_time_tracking_entry) | **PUT** /time_tracking_entries/{time_tracking_entry_gid} | Update a time tracking entry
-*TypeaheadApi* | [**typeahead_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TypeaheadApi.md#typeahead_for_workspace) | **GET** /workspaces/{workspace_gid}/typeahead | Get objects via typeahead
-*UserTaskListsApi* | [**get_user_task_list**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/UserTaskListsApi.md#get_user_task_list) | **GET** /user_task_lists/{user_task_list_gid} | Get a user task list
-*UserTaskListsApi* | [**get_user_task_list_for_user**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/UserTaskListsApi.md#get_user_task_list_for_user) | **GET** /users/{user_gid}/user_task_list | Get a user&#x27;s task list
-*UsersApi* | [**get_favorites_for_user**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/UsersApi.md#get_favorites_for_user) | **GET** /users/{user_gid}/favorites | Get a user&#x27;s favorites
-*UsersApi* | [**get_user**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/UsersApi.md#get_user) | **GET** /users/{user_gid} | Get a user
-*UsersApi* | [**get_users**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/UsersApi.md#get_users) | **GET** /users | Get multiple users
-*UsersApi* | [**get_users_for_team**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/UsersApi.md#get_users_for_team) | **GET** /teams/{team_gid}/users | Get users in a team
-*UsersApi* | [**get_users_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/UsersApi.md#get_users_for_workspace) | **GET** /workspaces/{workspace_gid}/users | Get users in a workspace or organization
-*WebhooksApi* | [**create_webhook**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WebhooksApi.md#create_webhook) | **POST** /webhooks | Establish a webhook
-*WebhooksApi* | [**delete_webhook**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WebhooksApi.md#delete_webhook) | **DELETE** /webhooks/{webhook_gid} | Delete a webhook
-*WebhooksApi* | [**get_webhook**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WebhooksApi.md#get_webhook) | **GET** /webhooks/{webhook_gid} | Get a webhook
-*WebhooksApi* | [**get_webhooks**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WebhooksApi.md#get_webhooks) | **GET** /webhooks | Get multiple webhooks
-*WebhooksApi* | [**update_webhook**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WebhooksApi.md#update_webhook) | **PUT** /webhooks/{webhook_gid} | Update a webhook
-*WorkspaceMembershipsApi* | [**get_workspace_membership**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspaceMembershipsApi.md#get_workspace_membership) | **GET** /workspace_memberships/{workspace_membership_gid} | Get a workspace membership
-*WorkspaceMembershipsApi* | [**get_workspace_memberships_for_user**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspaceMembershipsApi.md#get_workspace_memberships_for_user) | **GET** /users/{user_gid}/workspace_memberships | Get workspace memberships for a user
-*WorkspaceMembershipsApi* | [**get_workspace_memberships_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspaceMembershipsApi.md#get_workspace_memberships_for_workspace) | **GET** /workspaces/{workspace_gid}/workspace_memberships | Get the workspace memberships for a workspace
-*WorkspacesApi* | [**add_user_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspacesApi.md#add_user_for_workspace) | **POST** /workspaces/{workspace_gid}/addUser | Add a user to a workspace or organization
-*WorkspacesApi* | [**get_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspacesApi.md#get_workspace) | **GET** /workspaces/{workspace_gid} | Get a workspace
-*WorkspacesApi* | [**get_workspaces**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspacesApi.md#get_workspaces) | **GET** /workspaces | Get multiple workspaces
-*WorkspacesApi* | [**remove_user_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspacesApi.md#remove_user_for_workspace) | **POST** /workspaces/{workspace_gid}/removeUser | Remove a user from a workspace or organization
-*WorkspacesApi* | [**update_workspace**](https://github.com/Asana/python-asana/blob/v5.0.5/docs/WorkspacesApi.md#update_workspace) | **PUT** /workspaces/{workspace_gid} | Update a workspace
+*AllocationsApi* | [**create_allocation**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AllocationsApi.md#create_allocation) | **POST** /allocations | Create an allocation
+*AllocationsApi* | [**delete_allocation**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AllocationsApi.md#delete_allocation) | **DELETE** /allocations/{allocation_gid} | Delete an allocation
+*AllocationsApi* | [**get_allocation**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AllocationsApi.md#get_allocation) | **GET** /allocations/{allocation_gid} | Get an allocation
+*AllocationsApi* | [**get_allocations**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AllocationsApi.md#get_allocations) | **GET** /allocations | Get multiple allocations
+*AllocationsApi* | [**update_allocation**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AllocationsApi.md#update_allocation) | **PUT** /allocations/{allocation_gid} | Update an allocation
+*AttachmentsApi* | [**create_attachment_for_object**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AttachmentsApi.md#create_attachment_for_object) | **POST** /attachments | Upload an attachment
+*AttachmentsApi* | [**delete_attachment**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AttachmentsApi.md#delete_attachment) | **DELETE** /attachments/{attachment_gid} | Delete an attachment
+*AttachmentsApi* | [**get_attachment**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AttachmentsApi.md#get_attachment) | **GET** /attachments/{attachment_gid} | Get an attachment
+*AttachmentsApi* | [**get_attachments_for_object**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AttachmentsApi.md#get_attachments_for_object) | **GET** /attachments | Get attachments from an object
+*AuditLogAPIApi* | [**get_audit_log_events**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/AuditLogAPIApi.md#get_audit_log_events) | **GET** /workspaces/{workspace_gid}/audit_log_events | Get audit log events
+*BatchAPIApi* | [**create_batch_request**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/BatchAPIApi.md#create_batch_request) | **POST** /batch | Submit parallel requests
+*CustomFieldSettingsApi* | [**get_custom_field_settings_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldSettingsApi.md#get_custom_field_settings_for_portfolio) | **GET** /portfolios/{portfolio_gid}/custom_field_settings | Get a portfolio&#x27;s custom fields
+*CustomFieldSettingsApi* | [**get_custom_field_settings_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldSettingsApi.md#get_custom_field_settings_for_project) | **GET** /projects/{project_gid}/custom_field_settings | Get a project&#x27;s custom fields
+*CustomFieldsApi* | [**create_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#create_custom_field) | **POST** /custom_fields | Create a custom field
+*CustomFieldsApi* | [**create_enum_option_for_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#create_enum_option_for_custom_field) | **POST** /custom_fields/{custom_field_gid}/enum_options | Create an enum option
+*CustomFieldsApi* | [**delete_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#delete_custom_field) | **DELETE** /custom_fields/{custom_field_gid} | Delete a custom field
+*CustomFieldsApi* | [**get_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#get_custom_field) | **GET** /custom_fields/{custom_field_gid} | Get a custom field
+*CustomFieldsApi* | [**get_custom_fields_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#get_custom_fields_for_workspace) | **GET** /workspaces/{workspace_gid}/custom_fields | Get a workspace&#x27;s custom fields
+*CustomFieldsApi* | [**insert_enum_option_for_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#insert_enum_option_for_custom_field) | **POST** /custom_fields/{custom_field_gid}/enum_options/insert | Reorder a custom field&#x27;s enum
+*CustomFieldsApi* | [**update_custom_field**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#update_custom_field) | **PUT** /custom_fields/{custom_field_gid} | Update a custom field
+*CustomFieldsApi* | [**update_enum_option**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/CustomFieldsApi.md#update_enum_option) | **PUT** /enum_options/{enum_option_gid} | Update an enum option
+*EventsApi* | [**get_events**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/EventsApi.md#get_events) | **GET** /events | Get events on a resource
+*GoalRelationshipsApi* | [**add_supporting_relationship**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalRelationshipsApi.md#add_supporting_relationship) | **POST** /goals/{goal_gid}/addSupportingRelationship | Add a supporting goal relationship
+*GoalRelationshipsApi* | [**get_goal_relationship**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalRelationshipsApi.md#get_goal_relationship) | **GET** /goal_relationships/{goal_relationship_gid} | Get a goal relationship
+*GoalRelationshipsApi* | [**get_goal_relationships**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalRelationshipsApi.md#get_goal_relationships) | **GET** /goal_relationships | Get goal relationships
+*GoalRelationshipsApi* | [**remove_supporting_relationship**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalRelationshipsApi.md#remove_supporting_relationship) | **POST** /goals/{goal_gid}/removeSupportingRelationship | Removes a supporting goal relationship
+*GoalRelationshipsApi* | [**update_goal_relationship**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalRelationshipsApi.md#update_goal_relationship) | **PUT** /goal_relationships/{goal_relationship_gid} | Update a goal relationship
+*GoalsApi* | [**add_followers**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#add_followers) | **POST** /goals/{goal_gid}/addFollowers | Add a collaborator to a goal
+*GoalsApi* | [**create_goal**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#create_goal) | **POST** /goals | Create a goal
+*GoalsApi* | [**create_goal_metric**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#create_goal_metric) | **POST** /goals/{goal_gid}/setMetric | Create a goal metric
+*GoalsApi* | [**delete_goal**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#delete_goal) | **DELETE** /goals/{goal_gid} | Delete a goal
+*GoalsApi* | [**get_goal**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#get_goal) | **GET** /goals/{goal_gid} | Get a goal
+*GoalsApi* | [**get_goals**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#get_goals) | **GET** /goals | Get goals
+*GoalsApi* | [**get_parent_goals_for_goal**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#get_parent_goals_for_goal) | **GET** /goals/{goal_gid}/parentGoals | Get parent goals from a goal
+*GoalsApi* | [**remove_followers**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#remove_followers) | **POST** /goals/{goal_gid}/removeFollowers | Remove a collaborator from a goal
+*GoalsApi* | [**update_goal**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#update_goal) | **PUT** /goals/{goal_gid} | Update a goal
+*GoalsApi* | [**update_goal_metric**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/GoalsApi.md#update_goal_metric) | **POST** /goals/{goal_gid}/setMetricCurrentValue | Update a goal metric
+*JobsApi* | [**get_job**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/JobsApi.md#get_job) | **GET** /jobs/{job_gid} | Get a job by id
+*MembershipsApi* | [**create_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/MembershipsApi.md#create_membership) | **POST** /memberships | Create a membership
+*MembershipsApi* | [**delete_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/MembershipsApi.md#delete_membership) | **DELETE** /memberships/{membership_gid} | Delete a membership
+*MembershipsApi* | [**get_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/MembershipsApi.md#get_membership) | **GET** /memberships/{membership_gid} | Get a membership
+*MembershipsApi* | [**get_memberships**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/MembershipsApi.md#get_memberships) | **GET** /memberships | Get multiple memberships
+*MembershipsApi* | [**update_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/MembershipsApi.md#update_membership) | **PUT** /memberships/{membership_gid} | Update a membership
+*OrganizationExportsApi* | [**create_organization_export**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/OrganizationExportsApi.md#create_organization_export) | **POST** /organization_exports | Create an organization export request
+*OrganizationExportsApi* | [**get_organization_export**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/OrganizationExportsApi.md#get_organization_export) | **GET** /organization_exports/{organization_export_gid} | Get details on an org export request
+*PortfolioMembershipsApi* | [**get_portfolio_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfolioMembershipsApi.md#get_portfolio_membership) | **GET** /portfolio_memberships/{portfolio_membership_gid} | Get a portfolio membership
+*PortfolioMembershipsApi* | [**get_portfolio_memberships**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfolioMembershipsApi.md#get_portfolio_memberships) | **GET** /portfolio_memberships | Get multiple portfolio memberships
+*PortfolioMembershipsApi* | [**get_portfolio_memberships_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfolioMembershipsApi.md#get_portfolio_memberships_for_portfolio) | **GET** /portfolios/{portfolio_gid}/portfolio_memberships | Get memberships from a portfolio
+*PortfoliosApi* | [**add_custom_field_setting_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#add_custom_field_setting_for_portfolio) | **POST** /portfolios/{portfolio_gid}/addCustomFieldSetting | Add a custom field to a portfolio
+*PortfoliosApi* | [**add_item_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#add_item_for_portfolio) | **POST** /portfolios/{portfolio_gid}/addItem | Add a portfolio item
+*PortfoliosApi* | [**add_members_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#add_members_for_portfolio) | **POST** /portfolios/{portfolio_gid}/addMembers | Add users to a portfolio
+*PortfoliosApi* | [**create_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#create_portfolio) | **POST** /portfolios | Create a portfolio
+*PortfoliosApi* | [**delete_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#delete_portfolio) | **DELETE** /portfolios/{portfolio_gid} | Delete a portfolio
+*PortfoliosApi* | [**get_items_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#get_items_for_portfolio) | **GET** /portfolios/{portfolio_gid}/items | Get portfolio items
+*PortfoliosApi* | [**get_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#get_portfolio) | **GET** /portfolios/{portfolio_gid} | Get a portfolio
+*PortfoliosApi* | [**get_portfolios**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#get_portfolios) | **GET** /portfolios | Get multiple portfolios
+*PortfoliosApi* | [**remove_custom_field_setting_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#remove_custom_field_setting_for_portfolio) | **POST** /portfolios/{portfolio_gid}/removeCustomFieldSetting | Remove a custom field from a portfolio
+*PortfoliosApi* | [**remove_item_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#remove_item_for_portfolio) | **POST** /portfolios/{portfolio_gid}/removeItem | Remove a portfolio item
+*PortfoliosApi* | [**remove_members_for_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#remove_members_for_portfolio) | **POST** /portfolios/{portfolio_gid}/removeMembers | Remove users from a portfolio
+*PortfoliosApi* | [**update_portfolio**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/PortfoliosApi.md#update_portfolio) | **PUT** /portfolios/{portfolio_gid} | Update a portfolio
+*ProjectBriefsApi* | [**create_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectBriefsApi.md#create_project_brief) | **POST** /projects/{project_gid}/project_briefs | Create a project brief
+*ProjectBriefsApi* | [**delete_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectBriefsApi.md#delete_project_brief) | **DELETE** /project_briefs/{project_brief_gid} | Delete a project brief
+*ProjectBriefsApi* | [**get_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectBriefsApi.md#get_project_brief) | **GET** /project_briefs/{project_brief_gid} | Get a project brief
+*ProjectBriefsApi* | [**update_project_brief**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectBriefsApi.md#update_project_brief) | **PUT** /project_briefs/{project_brief_gid} | Update a project brief
+*ProjectMembershipsApi* | [**get_project_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectMembershipsApi.md#get_project_membership) | **GET** /project_memberships/{project_membership_gid} | Get a project membership
+*ProjectMembershipsApi* | [**get_project_memberships_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectMembershipsApi.md#get_project_memberships_for_project) | **GET** /projects/{project_gid}/project_memberships | Get memberships from a project
+*ProjectStatusesApi* | [**create_project_status_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectStatusesApi.md#create_project_status_for_project) | **POST** /projects/{project_gid}/project_statuses | Create a project status
+*ProjectStatusesApi* | [**delete_project_status**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectStatusesApi.md#delete_project_status) | **DELETE** /project_statuses/{project_status_gid} | Delete a project status
+*ProjectStatusesApi* | [**get_project_status**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectStatusesApi.md#get_project_status) | **GET** /project_statuses/{project_status_gid} | Get a project status
+*ProjectStatusesApi* | [**get_project_statuses_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectStatusesApi.md#get_project_statuses_for_project) | **GET** /projects/{project_gid}/project_statuses | Get statuses from a project
+*ProjectTemplatesApi* | [**delete_project_template**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectTemplatesApi.md#delete_project_template) | **DELETE** /project_templates/{project_template_gid} | Delete a project template
+*ProjectTemplatesApi* | [**get_project_template**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectTemplatesApi.md#get_project_template) | **GET** /project_templates/{project_template_gid} | Get a project template
+*ProjectTemplatesApi* | [**get_project_templates**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectTemplatesApi.md#get_project_templates) | **GET** /project_templates | Get multiple project templates
+*ProjectTemplatesApi* | [**get_project_templates_for_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectTemplatesApi.md#get_project_templates_for_team) | **GET** /teams/{team_gid}/project_templates | Get a team&#x27;s project templates
+*ProjectTemplatesApi* | [**instantiate_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectTemplatesApi.md#instantiate_project) | **POST** /project_templates/{project_template_gid}/instantiateProject | Instantiate a project from a project template
+*ProjectsApi* | [**add_custom_field_setting_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#add_custom_field_setting_for_project) | **POST** /projects/{project_gid}/addCustomFieldSetting | Add a custom field to a project
+*ProjectsApi* | [**add_followers_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#add_followers_for_project) | **POST** /projects/{project_gid}/addFollowers | Add followers to a project
+*ProjectsApi* | [**add_members_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#add_members_for_project) | **POST** /projects/{project_gid}/addMembers | Add users to a project
+*ProjectsApi* | [**create_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#create_project) | **POST** /projects | Create a project
+*ProjectsApi* | [**create_project_for_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#create_project_for_team) | **POST** /teams/{team_gid}/projects | Create a project in a team
+*ProjectsApi* | [**create_project_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#create_project_for_workspace) | **POST** /workspaces/{workspace_gid}/projects | Create a project in a workspace
+*ProjectsApi* | [**delete_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#delete_project) | **DELETE** /projects/{project_gid} | Delete a project
+*ProjectsApi* | [**duplicate_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#duplicate_project) | **POST** /projects/{project_gid}/duplicate | Duplicate a project
+*ProjectsApi* | [**get_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#get_project) | **GET** /projects/{project_gid} | Get a project
+*ProjectsApi* | [**get_projects**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#get_projects) | **GET** /projects | Get multiple projects
+*ProjectsApi* | [**get_projects_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#get_projects_for_task) | **GET** /tasks/{task_gid}/projects | Get projects a task is in
+*ProjectsApi* | [**get_projects_for_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#get_projects_for_team) | **GET** /teams/{team_gid}/projects | Get a team&#x27;s projects
+*ProjectsApi* | [**get_projects_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#get_projects_for_workspace) | **GET** /workspaces/{workspace_gid}/projects | Get all projects in a workspace
+*ProjectsApi* | [**get_task_counts_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#get_task_counts_for_project) | **GET** /projects/{project_gid}/task_counts | Get task count of a project
+*ProjectsApi* | [**project_save_as_template**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#project_save_as_template) | **POST** /projects/{project_gid}/saveAsTemplate | Create a project template from a project
+*ProjectsApi* | [**remove_custom_field_setting_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#remove_custom_field_setting_for_project) | **POST** /projects/{project_gid}/removeCustomFieldSetting | Remove a custom field from a project
+*ProjectsApi* | [**remove_followers_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#remove_followers_for_project) | **POST** /projects/{project_gid}/removeFollowers | Remove followers from a project
+*ProjectsApi* | [**remove_members_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#remove_members_for_project) | **POST** /projects/{project_gid}/removeMembers | Remove users from a project
+*ProjectsApi* | [**update_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#update_project) | **PUT** /projects/{project_gid} | Update a project
+*RulesApi* | [**trigger_rule**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/RulesApi.md#trigger_rule) | **POST** /rule_triggers/{rule_trigger_gid}/run | Trigger a rule
+*SectionsApi* | [**add_task_for_section**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/SectionsApi.md#add_task_for_section) | **POST** /sections/{section_gid}/addTask | Add task to section
+*SectionsApi* | [**create_section_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/SectionsApi.md#create_section_for_project) | **POST** /projects/{project_gid}/sections | Create a section in a project
+*SectionsApi* | [**delete_section**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/SectionsApi.md#delete_section) | **DELETE** /sections/{section_gid} | Delete a section
+*SectionsApi* | [**get_section**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/SectionsApi.md#get_section) | **GET** /sections/{section_gid} | Get a section
+*SectionsApi* | [**get_sections_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/SectionsApi.md#get_sections_for_project) | **GET** /projects/{project_gid}/sections | Get sections in a project
+*SectionsApi* | [**insert_section_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/SectionsApi.md#insert_section_for_project) | **POST** /projects/{project_gid}/sections/insert | Move or Insert sections
+*SectionsApi* | [**update_section**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/SectionsApi.md#update_section) | **PUT** /sections/{section_gid} | Update a section
+*StatusUpdatesApi* | [**create_status_for_object**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StatusUpdatesApi.md#create_status_for_object) | **POST** /status_updates | Create a status update
+*StatusUpdatesApi* | [**delete_status**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StatusUpdatesApi.md#delete_status) | **DELETE** /status_updates/{status_update_gid} | Delete a status update
+*StatusUpdatesApi* | [**get_status**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StatusUpdatesApi.md#get_status) | **GET** /status_updates/{status_update_gid} | Get a status update
+*StatusUpdatesApi* | [**get_statuses_for_object**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StatusUpdatesApi.md#get_statuses_for_object) | **GET** /status_updates | Get status updates from an object
+*StoriesApi* | [**create_story_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StoriesApi.md#create_story_for_task) | **POST** /tasks/{task_gid}/stories | Create a story on a task
+*StoriesApi* | [**delete_story**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StoriesApi.md#delete_story) | **DELETE** /stories/{story_gid} | Delete a story
+*StoriesApi* | [**get_stories_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StoriesApi.md#get_stories_for_task) | **GET** /tasks/{task_gid}/stories | Get stories from a task
+*StoriesApi* | [**get_story**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StoriesApi.md#get_story) | **GET** /stories/{story_gid} | Get a story
+*StoriesApi* | [**update_story**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/StoriesApi.md#update_story) | **PUT** /stories/{story_gid} | Update a story
+*TagsApi* | [**create_tag**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#create_tag) | **POST** /tags | Create a tag
+*TagsApi* | [**create_tag_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#create_tag_for_workspace) | **POST** /workspaces/{workspace_gid}/tags | Create a tag in a workspace
+*TagsApi* | [**delete_tag**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#delete_tag) | **DELETE** /tags/{tag_gid} | Delete a tag
+*TagsApi* | [**get_tag**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#get_tag) | **GET** /tags/{tag_gid} | Get a tag
+*TagsApi* | [**get_tags**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#get_tags) | **GET** /tags | Get multiple tags
+*TagsApi* | [**get_tags_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#get_tags_for_task) | **GET** /tasks/{task_gid}/tags | Get a task&#x27;s tags
+*TagsApi* | [**get_tags_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#get_tags_for_workspace) | **GET** /workspaces/{workspace_gid}/tags | Get tags in a workspace
+*TagsApi* | [**update_tag**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TagsApi.md#update_tag) | **PUT** /tags/{tag_gid} | Update a tag
+*TaskTemplatesApi* | [**delete_task_template**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TaskTemplatesApi.md#delete_task_template) | **DELETE** /task_templates/{task_template_gid} | Delete a task template
+*TaskTemplatesApi* | [**get_task_template**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TaskTemplatesApi.md#get_task_template) | **GET** /task_templates/{task_template_gid} | Get a task template
+*TaskTemplatesApi* | [**get_task_templates**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TaskTemplatesApi.md#get_task_templates) | **GET** /task_templates | Get multiple task templates
+*TaskTemplatesApi* | [**instantiate_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TaskTemplatesApi.md#instantiate_task) | **POST** /task_templates/{task_template_gid}/instantiateTask | Instantiate a task from a task template
+*TasksApi* | [**add_dependencies_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#add_dependencies_for_task) | **POST** /tasks/{task_gid}/addDependencies | Set dependencies for a task
+*TasksApi* | [**add_dependents_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#add_dependents_for_task) | **POST** /tasks/{task_gid}/addDependents | Set dependents for a task
+*TasksApi* | [**add_followers_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#add_followers_for_task) | **POST** /tasks/{task_gid}/addFollowers | Add followers to a task
+*TasksApi* | [**add_project_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#add_project_for_task) | **POST** /tasks/{task_gid}/addProject | Add a project to a task
+*TasksApi* | [**add_tag_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#add_tag_for_task) | **POST** /tasks/{task_gid}/addTag | Add a tag to a task
+*TasksApi* | [**create_subtask_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#create_subtask_for_task) | **POST** /tasks/{task_gid}/subtasks | Create a subtask
+*TasksApi* | [**create_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#create_task) | **POST** /tasks | Create a task
+*TasksApi* | [**delete_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#delete_task) | **DELETE** /tasks/{task_gid} | Delete a task
+*TasksApi* | [**duplicate_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#duplicate_task) | **POST** /tasks/{task_gid}/duplicate | Duplicate a task
+*TasksApi* | [**get_dependencies_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_dependencies_for_task) | **GET** /tasks/{task_gid}/dependencies | Get dependencies from a task
+*TasksApi* | [**get_dependents_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_dependents_for_task) | **GET** /tasks/{task_gid}/dependents | Get dependents from a task
+*TasksApi* | [**get_subtasks_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_subtasks_for_task) | **GET** /tasks/{task_gid}/subtasks | Get subtasks from a task
+*TasksApi* | [**get_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_task) | **GET** /tasks/{task_gid} | Get a task
+*TasksApi* | [**get_task_for_custom_id**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_task_for_custom_id) | **GET** /workspaces/{workspace_gid}/tasks/custom_id/{custom_id} | Get a task for a given custom ID
+*TasksApi* | [**get_tasks**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_tasks) | **GET** /tasks | Get multiple tasks
+*TasksApi* | [**get_tasks_for_project**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_tasks_for_project) | **GET** /projects/{project_gid}/tasks | Get tasks from a project
+*TasksApi* | [**get_tasks_for_section**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_tasks_for_section) | **GET** /sections/{section_gid}/tasks | Get tasks from a section
+*TasksApi* | [**get_tasks_for_tag**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_tasks_for_tag) | **GET** /tags/{tag_gid}/tasks | Get tasks from a tag
+*TasksApi* | [**get_tasks_for_user_task_list**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_tasks_for_user_task_list) | **GET** /user_task_lists/{user_task_list_gid}/tasks | Get tasks from a user task list
+*TasksApi* | [**remove_dependencies_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#remove_dependencies_for_task) | **POST** /tasks/{task_gid}/removeDependencies | Unlink dependencies from a task
+*TasksApi* | [**remove_dependents_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#remove_dependents_for_task) | **POST** /tasks/{task_gid}/removeDependents | Unlink dependents from a task
+*TasksApi* | [**remove_follower_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#remove_follower_for_task) | **POST** /tasks/{task_gid}/removeFollowers | Remove followers from a task
+*TasksApi* | [**remove_project_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#remove_project_for_task) | **POST** /tasks/{task_gid}/removeProject | Remove a project from a task
+*TasksApi* | [**remove_tag_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#remove_tag_for_task) | **POST** /tasks/{task_gid}/removeTag | Remove a tag from a task
+*TasksApi* | [**search_tasks_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#search_tasks_for_workspace) | **GET** /workspaces/{workspace_gid}/tasks/search | Search tasks in a workspace
+*TasksApi* | [**set_parent_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#set_parent_for_task) | **POST** /tasks/{task_gid}/setParent | Set the parent of a task
+*TasksApi* | [**update_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#update_task) | **PUT** /tasks/{task_gid} | Update a task
+*TeamMembershipsApi* | [**get_team_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamMembershipsApi.md#get_team_membership) | **GET** /team_memberships/{team_membership_gid} | Get a team membership
+*TeamMembershipsApi* | [**get_team_memberships**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamMembershipsApi.md#get_team_memberships) | **GET** /team_memberships | Get team memberships
+*TeamMembershipsApi* | [**get_team_memberships_for_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamMembershipsApi.md#get_team_memberships_for_team) | **GET** /teams/{team_gid}/team_memberships | Get memberships from a team
+*TeamMembershipsApi* | [**get_team_memberships_for_user**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamMembershipsApi.md#get_team_memberships_for_user) | **GET** /users/{user_gid}/team_memberships | Get memberships from a user
+*TeamsApi* | [**add_user_for_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamsApi.md#add_user_for_team) | **POST** /teams/{team_gid}/addUser | Add a user to a team
+*TeamsApi* | [**create_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamsApi.md#create_team) | **POST** /teams | Create a team
+*TeamsApi* | [**get_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamsApi.md#get_team) | **GET** /teams/{team_gid} | Get a team
+*TeamsApi* | [**get_teams_for_user**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamsApi.md#get_teams_for_user) | **GET** /users/{user_gid}/teams | Get teams for a user
+*TeamsApi* | [**get_teams_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamsApi.md#get_teams_for_workspace) | **GET** /workspaces/{workspace_gid}/teams | Get teams in a workspace
+*TeamsApi* | [**remove_user_for_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamsApi.md#remove_user_for_team) | **POST** /teams/{team_gid}/removeUser | Remove a user from a team
+*TeamsApi* | [**update_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TeamsApi.md#update_team) | **PUT** /teams/{team_gid} | Update a team
+*TimePeriodsApi* | [**get_time_period**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TimePeriodsApi.md#get_time_period) | **GET** /time_periods/{time_period_gid} | Get a time period
+*TimePeriodsApi* | [**get_time_periods**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TimePeriodsApi.md#get_time_periods) | **GET** /time_periods | Get time periods
+*TimeTrackingEntriesApi* | [**create_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TimeTrackingEntriesApi.md#create_time_tracking_entry) | **POST** /tasks/{task_gid}/time_tracking_entries | Create a time tracking entry
+*TimeTrackingEntriesApi* | [**delete_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TimeTrackingEntriesApi.md#delete_time_tracking_entry) | **DELETE** /time_tracking_entries/{time_tracking_entry_gid} | Delete a time tracking entry
+*TimeTrackingEntriesApi* | [**get_time_tracking_entries_for_task**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TimeTrackingEntriesApi.md#get_time_tracking_entries_for_task) | **GET** /tasks/{task_gid}/time_tracking_entries | Get time tracking entries for a task
+*TimeTrackingEntriesApi* | [**get_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TimeTrackingEntriesApi.md#get_time_tracking_entry) | **GET** /time_tracking_entries/{time_tracking_entry_gid} | Get a time tracking entry
+*TimeTrackingEntriesApi* | [**update_time_tracking_entry**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TimeTrackingEntriesApi.md#update_time_tracking_entry) | **PUT** /time_tracking_entries/{time_tracking_entry_gid} | Update a time tracking entry
+*TypeaheadApi* | [**typeahead_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TypeaheadApi.md#typeahead_for_workspace) | **GET** /workspaces/{workspace_gid}/typeahead | Get objects via typeahead
+*UserTaskListsApi* | [**get_user_task_list**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/UserTaskListsApi.md#get_user_task_list) | **GET** /user_task_lists/{user_task_list_gid} | Get a user task list
+*UserTaskListsApi* | [**get_user_task_list_for_user**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/UserTaskListsApi.md#get_user_task_list_for_user) | **GET** /users/{user_gid}/user_task_list | Get a user&#x27;s task list
+*UsersApi* | [**get_favorites_for_user**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/UsersApi.md#get_favorites_for_user) | **GET** /users/{user_gid}/favorites | Get a user&#x27;s favorites
+*UsersApi* | [**get_user**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/UsersApi.md#get_user) | **GET** /users/{user_gid} | Get a user
+*UsersApi* | [**get_users**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/UsersApi.md#get_users) | **GET** /users | Get multiple users
+*UsersApi* | [**get_users_for_team**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/UsersApi.md#get_users_for_team) | **GET** /teams/{team_gid}/users | Get users in a team
+*UsersApi* | [**get_users_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/UsersApi.md#get_users_for_workspace) | **GET** /workspaces/{workspace_gid}/users | Get users in a workspace or organization
+*WebhooksApi* | [**create_webhook**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WebhooksApi.md#create_webhook) | **POST** /webhooks | Establish a webhook
+*WebhooksApi* | [**delete_webhook**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WebhooksApi.md#delete_webhook) | **DELETE** /webhooks/{webhook_gid} | Delete a webhook
+*WebhooksApi* | [**get_webhook**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WebhooksApi.md#get_webhook) | **GET** /webhooks/{webhook_gid} | Get a webhook
+*WebhooksApi* | [**get_webhooks**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WebhooksApi.md#get_webhooks) | **GET** /webhooks | Get multiple webhooks
+*WebhooksApi* | [**update_webhook**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WebhooksApi.md#update_webhook) | **PUT** /webhooks/{webhook_gid} | Update a webhook
+*WorkspaceMembershipsApi* | [**get_workspace_membership**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspaceMembershipsApi.md#get_workspace_membership) | **GET** /workspace_memberships/{workspace_membership_gid} | Get a workspace membership
+*WorkspaceMembershipsApi* | [**get_workspace_memberships_for_user**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspaceMembershipsApi.md#get_workspace_memberships_for_user) | **GET** /users/{user_gid}/workspace_memberships | Get workspace memberships for a user
+*WorkspaceMembershipsApi* | [**get_workspace_memberships_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspaceMembershipsApi.md#get_workspace_memberships_for_workspace) | **GET** /workspaces/{workspace_gid}/workspace_memberships | Get the workspace memberships for a workspace
+*WorkspacesApi* | [**add_user_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspacesApi.md#add_user_for_workspace) | **POST** /workspaces/{workspace_gid}/addUser | Add a user to a workspace or organization
+*WorkspacesApi* | [**get_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspacesApi.md#get_workspace) | **GET** /workspaces/{workspace_gid} | Get a workspace
+*WorkspacesApi* | [**get_workspaces**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspacesApi.md#get_workspaces) | **GET** /workspaces | Get multiple workspaces
+*WorkspacesApi* | [**remove_user_for_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspacesApi.md#remove_user_for_workspace) | **POST** /workspaces/{workspace_gid}/removeUser | Remove a user from a workspace or organization
+*WorkspacesApi* | [**update_workspace**](https://github.com/Asana/python-asana/blob/v5.0.6/docs/WorkspacesApi.md#update_workspace) | **PUT** /workspaces/{workspace_gid} | Update a workspace
 
-## Accessing repsonse data
+## Accessing response data
 
 ### Example: Accessing task data
 ```python
 .
 .
 .
 try:
@@ -499,15 +505,15 @@
         print("Exception when calling TasksApi->create_task: %s\n" % e)
 ```
 
 ## Pagination
 
 The pagination feature is enabled by default. This means two things:
 
-1: Endpoints that return a single response (EX: [get_task](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_task) ([Get a task](https://developers.asana.com/reference/gettask)), [get_project](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_project) ([Get a project](https://developers.asana.com/reference/getproject)), etc...)
+1: Endpoints that return a single response (EX: [get_task](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_task) ([Get a task](https://developers.asana.com/reference/gettask)), [get_project](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_project) ([Get a project](https://developers.asana.com/reference/getproject)), etc...)
 will return a response with the `"data"` key abstracted from the response.
 
 Instead of returning:
 ```python
 {
     "data": {
         "gid": "123",
@@ -534,16 +540,16 @@
         "gid": "1234567",
         "name": "user@example.com",
         "resource_type": "workspace"
     }
 }
 ```
 
-2: Endpoints that return an array of resources (EX: [get_tasks](https://github.com/Asana/python-asana/blob/v5.0.5/docs/TasksApi.md#get_tasks) ([Get multiple tasks](https://developers.asana.com/reference/gettasks)), [get_projects](https://github.com/Asana/python-asana/blob/v5.0.5/docs/ProjectsApi.md#get_projects) ([Get multiple projects](https://developers.asana.com/reference/getprojects)), etc...)
-will return a generator object ([PageIterator.items](https://github.com/Asana/python-asana/blob/v5.0.5/asana/pagination/page_iterator.py)) that you can use to iterate through each result.
+2: Endpoints that return an array of resources (EX: [get_tasks](https://github.com/Asana/python-asana/blob/v5.0.6/docs/TasksApi.md#get_tasks) ([Get multiple tasks](https://developers.asana.com/reference/gettasks)), [get_projects](https://github.com/Asana/python-asana/blob/v5.0.6/docs/ProjectsApi.md#get_projects) ([Get multiple projects](https://developers.asana.com/reference/getprojects)), etc...)
+will return a generator object ([PageIterator.items](https://github.com/Asana/python-asana/blob/v5.0.6/asana/pagination/page_iterator.py)) that you can use to iterate through each result.
 
 Example usage 1:
 ```python
 import asana
 from asana.rest import ApiException
 from pprint import pprint
```

### Comparing `asana-5.0.5/asana.egg-info/SOURCES.txt` & `asana-5.0.6/asana.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 asana/rest.py
 asana.egg-info/PKG-INFO
 asana.egg-info/SOURCES.txt
 asana.egg-info/dependency_links.txt
 asana.egg-info/requires.txt
 asana.egg-info/top_level.txt
 asana/api/__init__.py
+asana/api/allocations_api.py
 asana/api/attachments_api.py
 asana/api/audit_log_api_api.py
 asana/api/batch_api_api.py
 asana/api/custom_field_settings_api.py
 asana/api/custom_fields_api.py
 asana/api/events_api.py
 asana/api/goal_relationships_api.py
@@ -52,14 +53,15 @@
 asana/pagination/__init__.py
 asana/pagination/event_iterator.py
 asana/pagination/page_iterator.py
 build_tests/__init__.py
 build_tests/test_projects_api.py
 build_tests/test_tasks_api.py
 test/__init__.py
+test/test_allocations_api.py
 test/test_attachments_api.py
 test/test_audit_log_api_api.py
 test/test_batch_api_api.py
 test/test_custom_field_settings_api.py
 test/test_custom_fields_api.py
 test/test_events_api.py
 test/test_goal_relationships_api.py
```

### Comparing `asana-5.0.5/build_tests/test_projects_api.py` & `asana-5.0.6/build_tests/test_projects_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/build_tests/test_tasks_api.py` & `asana-5.0.6/build_tests/test_tasks_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/setup.py` & `asana-5.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import os
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "asana"
-VERSION = "5.0.5"
+VERSION = "5.0.6"
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     LONG_DESCRIPTION = readme.read()
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
```

### Comparing `asana-5.0.5/test/test_attachments_api.py` & `asana-5.0.6/test/test_attachments_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_audit_log_api_api.py` & `asana-5.0.6/test/test_audit_log_api_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_batch_api_api.py` & `asana-5.0.6/test/test_batch_api_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_custom_field_settings_api.py` & `asana-5.0.6/test/test_custom_field_settings_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_custom_fields_api.py` & `asana-5.0.6/test/test_custom_fields_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_events_api.py` & `asana-5.0.6/test/test_events_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_goal_relationships_api.py` & `asana-5.0.6/test/test_goal_relationships_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_goals_api.py` & `asana-5.0.6/test/test_goals_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_jobs_api.py` & `asana-5.0.6/test/test_jobs_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_memberships_api.py` & `asana-5.0.6/test/test_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_organization_exports_api.py` & `asana-5.0.6/test/test_organization_exports_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_portfolio_memberships_api.py` & `asana-5.0.6/test/test_portfolio_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_portfolios_api.py` & `asana-5.0.6/test/test_portfolios_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_project_briefs_api.py` & `asana-5.0.6/test/test_project_briefs_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_project_memberships_api.py` & `asana-5.0.6/test/test_project_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_project_statuses_api.py` & `asana-5.0.6/test/test_project_statuses_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_project_templates_api.py` & `asana-5.0.6/test/test_project_templates_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_projects_api.py` & `asana-5.0.6/test/test_projects_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_rules_api.py` & `asana-5.0.6/test/test_rules_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_sections_api.py` & `asana-5.0.6/test/test_sections_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_status_updates_api.py` & `asana-5.0.6/test/test_status_updates_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_stories_api.py` & `asana-5.0.6/test/test_stories_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_tags_api.py` & `asana-5.0.6/test/test_tags_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_task_templates_api.py` & `asana-5.0.6/test/test_task_templates_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_tasks_api.py` & `asana-5.0.6/test/test_tasks_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_team_memberships_api.py` & `asana-5.0.6/test/test_team_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_teams_api.py` & `asana-5.0.6/test/test_teams_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_time_periods_api.py` & `asana-5.0.6/test/test_time_periods_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_time_tracking_entries_api.py` & `asana-5.0.6/test/test_time_tracking_entries_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_typeahead_api.py` & `asana-5.0.6/test/test_typeahead_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_user_task_lists_api.py` & `asana-5.0.6/test/test_user_task_lists_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_users_api.py` & `asana-5.0.6/test/test_users_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_webhooks_api.py` & `asana-5.0.6/test/test_webhooks_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_workspace_memberships_api.py` & `asana-5.0.6/test/test_workspace_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-5.0.5/test/test_workspaces_api.py` & `asana-5.0.6/test/test_workspaces_api.py`

 * *Files identical despite different names*

