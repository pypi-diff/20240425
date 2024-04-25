# Comparing `tmp/attune-project-api-24.2.8.tar.gz` & `tmp/attune_project_api-24.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attune-project-api-24.2.8.tar", last modified: Sat Mar  9 11:37:07 2024, max compression
+gzip compressed data, was "attune_project_api-24.2.9.tar", last modified: Thu Apr 25 10:28:46 2024, max compression
```

## Comparing `attune-project-api-24.2.8.tar` & `attune_project_api-24.2.9.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-03-09 11:37:07.307379 attune-project-api-24.2.8/
--rw-r--r--   0 jchesney   (501) staff       (20)      493 2024-03-09 11:37:07.307142 attune-project-api-24.2.8/PKG-INFO
--rw-r--r--   0 jchesney   (501) staff       (20)       60 2021-12-30 21:22:50.000000 attune-project-api-24.2.8/README.rst
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-03-09 11:37:07.189013 attune-project-api-24.2.8/attune_project_api/
--rw-r--r--   0 jchesney   (501) staff       (20)      692 2022-10-03 05:25:18.000000 attune-project-api-24.2.8/attune_project_api/Exceptions.py
--rw-r--r--   0 jchesney   (501) staff       (20)    29522 2023-12-21 13:19:59.000000 attune-project-api-24.2.8/attune_project_api/ObjectStorageContext.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4257 2022-02-24 06:08:44.000000 attune-project-api-24.2.8/attune_project_api/RelationField.py
--rw-r--r--   0 jchesney   (501) staff       (20)     5040 2023-12-22 23:16:51.000000 attune-project-api-24.2.8/attune_project_api/StorageTuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2113 2022-01-07 01:53:29.000000 attune-project-api-24.2.8/attune_project_api/TupleFieldValidators.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2820 2022-01-12 10:25:43.000000 attune-project-api-24.2.8/attune_project_api/TupleValidators.py
--rw-r--r--   0 jchesney   (501) staff       (20)      316 2024-03-09 11:37:06.000000 attune-project-api-24.2.8/attune_project_api/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-03-09 11:37:07.196751 attune-project-api-24.2.8/attune_project_api/_contexts/
--rw-r--r--   0 jchesney   (501) staff       (20)    30585 2024-03-03 12:55:55.000000 attune-project-api-24.2.8/attune_project_api/_contexts/GitLibMixin.py
--rw-r--r--   0 jchesney   (501) staff       (20)    37244 2024-03-09 11:19:22.000000 attune-project-api-24.2.8/attune_project_api/_contexts/GitObjectStorageContext.py
--rw-r--r--   0 jchesney   (501) staff       (20)       39 2021-12-30 21:22:50.000000 attune-project-api-24.2.8/attune_project_api/_contexts/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-03-09 11:37:07.206473 attune-project-api-24.2.8/attune_project_api/_private/
--rw-r--r--   0 jchesney   (501) staff       (20)     1142 2022-01-07 01:53:29.000000 attune-project-api-24.2.8/attune_project_api/_private/RelationGraph.py
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2021-12-30 21:22:50.000000 attune-project-api-24.2.8/attune_project_api/_private/__init__.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3241 2022-05-23 00:41:40.000000 attune-project-api-24.2.8/attune_project_api/_private/archive_format.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3428 2023-02-28 01:54:20.000000 attune-project-api-24.2.8/attune_project_api/_private/archive_get_file_content.py
--rw-r--r--   0 jchesney   (501) staff       (20)      596 2022-01-07 03:41:18.000000 attune-project-api-24.2.8/attune_project_api/_private/archive_hasher.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3019 2022-05-23 00:41:40.000000 attune-project-api-24.2.8/attune_project_api/_private/archive_list_files.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4604 2023-04-01 02:14:20.000000 attune-project-api-24.2.8/attune_project_api/_private/large_file_http_downloader.py
--rw-r--r--   0 jchesney   (501) staff       (20)      661 2022-01-25 22:57:26.000000 attune-project-api-24.2.8/attune_project_api/_private/large_file_http_downloader_test.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1689 2023-06-24 03:58:21.000000 attune-project-api-24.2.8/attune_project_api/_private/readme_compiler.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-03-09 11:37:07.217649 attune-project-api-24.2.8/attune_project_api/_private/templates/
--rw-r--r--   0 jchesney   (501) staff       (20)     1598 2023-12-28 07:05:36.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/ProjectReadme.md.mako
--rw-r--r--   0 jchesney   (501) staff       (20)     2100 2023-11-28 06:54:00.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/ProjectReadmeAttune.md.mako
--rw-r--r--   0 jchesney   (501) staff       (20)      267 2023-02-10 03:43:12.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/ProjectReadmeBlueprints.md.mako
--rw-r--r--   0 jchesney   (501) staff       (20)      365 2023-11-28 06:54:00.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/ProjectReadmeCloneInstructions.md.mako
--rw-r--r--   0 jchesney   (501) staff       (20)     1007 2023-11-28 06:54:00.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/ProjectReadmeContribute.md.mako
--rw-r--r--   0 jchesney   (501) staff       (20)      242 2023-06-24 03:58:21.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/ProjectReadmeFiles.md.mako
--rw-r--r--   0 jchesney   (501) staff       (20)      375 2023-06-24 03:58:21.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/ProjectReadmeParameters.md.mako
--rw-r--r--   0 jchesney   (501) staff       (20)       27 2022-10-21 00:47:49.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-03-09 11:37:07.250175 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/
--rw-r--r--   0 jchesney   (501) staff       (20)     1583 2023-07-28 01:18:07.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprint.html.mako
--rw-r--r--   0 jchesney   (501) staff       (20)      624 2023-12-28 07:05:36.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintBreadcrumbs.html.mako
--rw-r--r--   0 jchesney   (501) staff       (20)     2653 2023-07-28 01:18:07.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintHead.html.mako
--rw-r--r--   0 jchesney   (501) staff       (20)     2050 2023-12-28 07:05:36.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintHeader.html.mako
--rw-r--r--   0 jchesney   (501) staff       (20)     1270 2023-12-28 07:05:36.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintRunWithAttune.html.mako
--rw-r--r--   0 jchesney   (501) staff       (20)      967 2023-07-28 01:18:07.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintScripts.html.mako
--rw-r--r--   0 jchesney   (501) staff       (20)      733 2023-07-28 01:18:07.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStep.html.mako
--rw-r--r--   0 jchesney   (501) staff       (20)     2503 2023-07-28 01:18:07.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStepConnection.html.mako
--rw-r--r--   0 jchesney   (501) staff       (20)     1037 2023-07-28 01:18:07.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStepFile.html.mako
--rw-r--r--   0 jchesney   (501) staff       (20)     1909 2023-07-28 01:18:07.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStepInner.html.mako
--rw-r--r--   0 jchesney   (501) staff       (20)     3118 2024-02-25 06:55:14.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStepScript.html.mako
--rw-r--r--   0 jchesney   (501) staff       (20)      599 2023-07-28 01:18:07.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStepTcpPing.html.mako
--rw-r--r--   0 jchesney   (501) staff       (20)      566 2023-07-28 01:18:07.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintToc.html.mako
--rw-r--r--   0 jchesney   (501) staff       (20)      773 2023-07-28 01:18:07.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintTocInner.html.mako
--rw-r--r--   0 jchesney   (501) staff       (20)     1085 2023-07-28 01:18:07.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteIndex.html.mako
--rw-r--r--   0 jchesney   (501) staff       (20)     1296 2023-07-28 01:18:07.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexAttuneAd.html.mako
--rw-r--r--   0 jchesney   (501) staff       (20)     1676 2023-07-28 01:18:07.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexBlueprintsList.html.mako
--rw-r--r--   0 jchesney   (501) staff       (20)      685 2023-07-28 01:18:07.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexFooter.html.mako
--rw-r--r--   0 jchesney   (501) staff       (20)     2395 2023-07-28 01:18:07.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexHead.html.mako
--rw-r--r--   0 jchesney   (501) staff       (20)     3106 2023-12-28 07:05:36.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexHeader.html.mako
--rw-r--r--   0 jchesney   (501) staff       (20)     1207 2023-12-28 07:05:36.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexJoinDiscord.html.mako
--rw-r--r--   0 jchesney   (501) staff       (20)     1662 2023-12-28 07:05:36.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexNavBar.html.mako
--rw-r--r--   0 jchesney   (501) staff       (20)      633 2023-06-24 03:58:21.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexScripts.html.mako
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-03-09 11:37:07.252484 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/styles/
--rw-r--r--   0 jchesney   (501) staff       (20)     2127 2023-12-28 07:05:36.000000 attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/styles/ProjectWebsiteStyle.css.mako
--rw-r--r--   0 jchesney   (501) staff       (20)     3044 2023-08-28 04:25:32.000000 attune-project-api-24.2.8/attune_project_api/_private/website_compiler.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2239 2023-12-28 07:05:36.000000 attune-project-api-24.2.8/attune_project_api/_private/website_compiler_test.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2948 2022-05-04 02:21:42.000000 attune-project-api-24.2.8/attune_project_api/alembic.ini
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-03-09 11:37:07.255409 attune-project-api-24.2.8/attune_project_api/alembic_migrations/
--rw-r--r--   0 jchesney   (501) staff       (20)       38 2022-05-04 02:21:42.000000 attune-project-api-24.2.8/attune_project_api/alembic_migrations/README
--rw-r--r--   0 jchesney   (501) staff       (20)     2038 2022-05-04 02:21:42.000000 attune-project-api-24.2.8/attune_project_api/alembic_migrations/env.py
--rw-r--r--   0 jchesney   (501) staff       (20)      494 2022-05-04 02:21:42.000000 attune-project-api-24.2.8/attune_project_api/alembic_migrations/script.py.mako
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-03-09 11:37:07.265852 attune-project-api-24.2.8/attune_project_api/alembic_migrations/versions/
--rw-r--r--   0 jchesney   (501) staff       (20)     1173 2024-01-21 03:37:06.000000 attune-project-api-24.2.8/attune_project_api/alembic_migrations/versions/0aa489aa66b2_store_name_in_project_metadata.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1173 2023-02-10 02:46:44.000000 attune-project-api-24.2.8/attune_project_api/alembic_migrations/versions/145c6dc54454_rename_comment_md_to_readme_md_for_items.py
--rw-r--r--   0 jchesney   (501) staff       (20)      417 2022-05-04 02:21:42.000000 attune-project-api-24.2.8/attune_project_api/alembic_migrations/versions/16e34a42a9a1_attune_v5_starting_point.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1853 2024-01-21 11:29:11.000000 attune-project-api-24.2.8/attune_project_api/alembic_migrations/versions/58b1656aac40_move_sql_to_script_txt_file_in_oracle_.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1326 2024-01-21 03:37:06.000000 attune-project-api-24.2.8/attune_project_api/alembic_migrations/versions/ba6a8e4d7e2b_move_metadata_json_file_to_project_.py
--rw-r--r--   0 jchesney   (501) staff       (20)      237 2023-12-23 03:15:25.000000 attune-project-api-24.2.8/attune_project_api/context_project_info.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-03-09 11:37:07.268627 attune-project-api-24.2.8/attune_project_api/items/
--rw-r--r--   0 jchesney   (501) staff       (20)      489 2022-01-07 01:53:29.000000 attune-project-api-24.2.8/attune_project_api/items/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-03-09 11:37:07.273440 attune-project-api-24.2.8/attune_project_api/items/file_archive_tuples/
--rw-r--r--   0 jchesney   (501) staff       (20)      163 2022-01-07 01:53:29.000000 attune-project-api-24.2.8/attune_project_api/items/file_archive_tuples/__init__.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4726 2023-05-11 05:39:25.000000 attune-project-api-24.2.8/attune_project_api/items/file_archive_tuples/file_archive_large_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2358 2023-12-23 09:26:09.000000 attune-project-api-24.2.8/attune_project_api/items/file_archive_tuples/file_archive_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     6108 2023-05-11 05:39:25.000000 attune-project-api-24.2.8/attune_project_api/items/file_archive_tuples/file_archive_versioned_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)      482 2022-02-28 06:52:20.000000 attune-project-api-24.2.8/attune_project_api/items/file_archive_tuples/file_tuple_constants.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3693 2023-12-21 13:19:59.000000 attune-project-api-24.2.8/attune_project_api/items/parameter_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)      690 2024-01-29 10:56:08.000000 attune-project-api-24.2.8/attune_project_api/items/project_metadata_tuple.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-03-09 11:37:07.294643 attune-project-api-24.2.8/attune_project_api/items/step_tuples/
--rw-r--r--   0 jchesney   (501) staff       (20)      928 2022-01-12 10:38:07.000000 attune-project-api-24.2.8/attune_project_api/items/step_tuples/__init__.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1905 2024-01-21 11:29:11.000000 attune-project-api-24.2.8/attune_project_api/items/step_tuples/step_bootstrap_linux_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2612 2024-01-19 07:06:31.000000 attune-project-api-24.2.8/attune_project_api/items/step_tuples/step_group_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4915 2024-02-20 02:20:53.000000 attune-project-api-24.2.8/attune_project_api/items/step_tuples/step_project_link_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4687 2024-01-21 11:29:11.000000 attune-project-api-24.2.8/attune_project_api/items/step_tuples/step_push_design_file_compiled_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2628 2024-01-19 09:34:23.000000 attune-project-api-24.2.8/attune_project_api/items/step_tuples/step_push_design_file_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2909 2024-01-21 11:29:11.000000 attune-project-api-24.2.8/attune_project_api/items/step_tuples/step_sql_oracle_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1582 2024-01-21 11:29:11.000000 attune-project-api-24.2.8/attune_project_api/items/step_tuples/step_ssh_prompted_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3125 2024-02-04 01:40:15.000000 attune-project-api-24.2.8/attune_project_api/items/step_tuples/step_ssh_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1659 2024-01-19 09:34:23.000000 attune-project-api-24.2.8/attune_project_api/items/step_tuples/step_tcp_ping_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3011 2024-01-21 11:29:11.000000 attune-project-api-24.2.8/attune_project_api/items/step_tuples/step_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3493 2024-02-04 01:33:43.000000 attune-project-api-24.2.8/attune_project_api/items/step_tuples/step_winrm_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)      544 2023-01-23 02:29:43.000000 attune-project-api-24.2.8/attune_project_api/key_util.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4275 2023-12-21 13:19:59.000000 attune-project-api-24.2.8/attune_project_api/migration.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-03-09 11:37:07.297495 attune-project-api-24.2.8/attune_project_api/remote/
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2023-08-28 04:25:32.000000 attune-project-api-24.2.8/attune_project_api/remote/__init__.py
--rw-r--r--   0 jchesney   (501) staff       (20)     5301 2023-08-28 04:25:32.000000 attune-project-api-24.2.8/attune_project_api/remote/project_api_clone_controller.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4238 2023-08-28 04:25:32.000000 attune-project-api-24.2.8/attune_project_api/remote/project_api_clone_controller_test.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-03-09 11:37:07.300527 attune-project-api-24.2.8/attune_project_api/tuples/
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2021-12-30 21:22:50.000000 attune-project-api-24.2.8/attune_project_api/tuples/__init__.py
--rw-r--r--   0 jchesney   (501) staff       (20)      366 2022-01-07 01:53:29.000000 attune-project-api-24.2.8/attune_project_api/tuples/git_commit_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1316 2023-12-28 07:05:36.000000 attune-project-api-24.2.8/attune_project_api/tuples/project_modified_tuple.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-03-09 11:37:07.306301 attune-project-api-24.2.8/attune_project_api.egg-info/
--rw-r--r--   0 jchesney   (501) staff       (20)      493 2024-03-09 11:37:07.000000 attune-project-api-24.2.8/attune_project_api.egg-info/PKG-INFO
--rw-r--r--   0 jchesney   (501) staff       (20)     6360 2024-03-09 11:37:07.000000 attune-project-api-24.2.8/attune_project_api.egg-info/SOURCES.txt
--rw-r--r--   0 jchesney   (501) staff       (20)        1 2024-03-09 11:37:07.000000 attune-project-api-24.2.8/attune_project_api.egg-info/dependency_links.txt
--rw-r--r--   0 jchesney   (501) staff       (20)        1 2024-03-09 11:37:07.000000 attune-project-api-24.2.8/attune_project_api.egg-info/not-zip-safe
--rw-r--r--   0 jchesney   (501) staff       (20)      127 2024-03-09 11:37:07.000000 attune-project-api-24.2.8/attune_project_api.egg-info/requires.txt
--rw-r--r--   0 jchesney   (501) staff       (20)       19 2024-03-09 11:37:07.000000 attune-project-api-24.2.8/attune_project_api.egg-info/top_level.txt
--rw-r--r--   0 jchesney   (501) staff       (20)       80 2024-03-09 11:37:07.308296 attune-project-api-24.2.8/setup.cfg
--rw-r--r--   0 jchesney   (501) staff       (20)     2193 2024-03-09 11:37:06.000000 attune-project-api-24.2.8/setup.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-03-09 11:37:07.305183 attune-project-api-24.2.8/tests/
--rw-r--r--   0 jchesney   (501) staff       (20)     5821 2023-12-23 23:12:49.000000 attune-project-api-24.2.8/tests/test_error_handling.py
--rw-r--r--   0 jchesney   (501) staff       (20)    10907 2024-01-21 11:29:11.000000 attune-project-api-24.2.8/tests/test_git_context.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3612 2023-12-21 13:19:59.000000 attune-project-api-24.2.8/tests/test_item_operations.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-04-25 10:28:46.743015 attune_project_api-24.2.9/
+-rw-r--r--   0 jchesney   (501) staff       (20)      493 2024-04-25 10:28:46.742843 attune_project_api-24.2.9/PKG-INFO
+-rw-r--r--   0 jchesney   (501) staff       (20)       60 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/README.rst
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-04-25 10:28:46.661453 attune_project_api-24.2.9/attune_project_api/
+-rw-r--r--   0 jchesney   (501) staff       (20)      692 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/Exceptions.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    29522 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/ObjectStorageContext.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4257 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/RelationField.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     5040 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/StorageTuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2113 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/TupleFieldValidators.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2820 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/TupleValidators.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      316 2024-04-25 10:28:46.000000 attune_project_api-24.2.9/attune_project_api/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-04-25 10:28:46.666632 attune_project_api-24.2.9/attune_project_api/_contexts/
+-rw-r--r--   0 jchesney   (501) staff       (20)    30585 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_contexts/GitLibMixin.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    37244 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_contexts/GitObjectStorageContext.py
+-rw-r--r--   0 jchesney   (501) staff       (20)       39 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_contexts/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-04-25 10:28:46.674961 attune_project_api-24.2.9/attune_project_api/_private/
+-rw-r--r--   0 jchesney   (501) staff       (20)     1142 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/RelationGraph.py
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/__init__.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3241 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/archive_format.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3428 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/archive_get_file_content.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      596 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/archive_hasher.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3019 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/archive_list_files.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4604 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/large_file_http_downloader.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      661 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/large_file_http_downloader_test.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1689 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/readme_compiler.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-04-25 10:28:46.683554 attune_project_api-24.2.9/attune_project_api/_private/templates/
+-rw-r--r--   0 jchesney   (501) staff       (20)     1598 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/ProjectReadme.md.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)     2100 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/ProjectReadmeAttune.md.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)      267 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/ProjectReadmeBlueprints.md.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)      365 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/ProjectReadmeCloneInstructions.md.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)     1007 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/ProjectReadmeContribute.md.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)      242 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/ProjectReadmeFiles.md.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)      375 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/ProjectReadmeParameters.md.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)       27 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-04-25 10:28:46.708159 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/
+-rw-r--r--   0 jchesney   (501) staff       (20)     1583 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprint.html.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)      624 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintBreadcrumbs.html.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)     2653 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintHead.html.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)     2050 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintHeader.html.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)     1270 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintRunWithAttune.html.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)      967 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintScripts.html.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)      733 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStep.html.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)     2503 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStepConnection.html.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)     1037 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStepFile.html.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)     1909 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStepInner.html.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)     3118 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStepScript.html.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)      599 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStepTcpPing.html.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)      566 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintToc.html.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)      773 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintTocInner.html.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)     1085 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteIndex.html.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)     1296 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexAttuneAd.html.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)     1676 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexBlueprintsList.html.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)      685 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexFooter.html.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)     2395 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexHead.html.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)     3106 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexHeader.html.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)     1207 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexJoinDiscord.html.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)     1662 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexNavBar.html.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)      633 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexScripts.html.mako
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-04-25 10:28:46.708550 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/styles/
+-rw-r--r--   0 jchesney   (501) staff       (20)     2127 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/styles/ProjectWebsiteStyle.css.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)     3044 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/website_compiler.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2239 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/_private/website_compiler_test.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2948 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/alembic.ini
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-04-25 10:28:46.714481 attune_project_api-24.2.9/attune_project_api/alembic_migrations/
+-rw-r--r--   0 jchesney   (501) staff       (20)       38 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/alembic_migrations/README
+-rw-r--r--   0 jchesney   (501) staff       (20)     2038 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/alembic_migrations/env.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      494 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/alembic_migrations/script.py.mako
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-04-25 10:28:46.717811 attune_project_api-24.2.9/attune_project_api/alembic_migrations/versions/
+-rw-r--r--   0 jchesney   (501) staff       (20)     1173 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/alembic_migrations/versions/0aa489aa66b2_store_name_in_project_metadata.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1173 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/alembic_migrations/versions/145c6dc54454_rename_comment_md_to_readme_md_for_items.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      417 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/alembic_migrations/versions/16e34a42a9a1_attune_v5_starting_point.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1853 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/alembic_migrations/versions/58b1656aac40_move_sql_to_script_txt_file_in_oracle_.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1326 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/alembic_migrations/versions/ba6a8e4d7e2b_move_metadata_json_file_to_project_.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      237 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/context_project_info.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-04-25 10:28:46.719410 attune_project_api-24.2.9/attune_project_api/items/
+-rw-r--r--   0 jchesney   (501) staff       (20)      489 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/items/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-04-25 10:28:46.722709 attune_project_api-24.2.9/attune_project_api/items/file_archive_tuples/
+-rw-r--r--   0 jchesney   (501) staff       (20)      163 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/items/file_archive_tuples/__init__.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4726 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/items/file_archive_tuples/file_archive_large_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2358 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/items/file_archive_tuples/file_archive_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     6108 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/items/file_archive_tuples/file_archive_versioned_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      482 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/items/file_archive_tuples/file_tuple_constants.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3693 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/items/parameter_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      690 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/items/project_metadata_tuple.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-04-25 10:28:46.731333 attune_project_api-24.2.9/attune_project_api/items/step_tuples/
+-rw-r--r--   0 jchesney   (501) staff       (20)      928 2024-04-24 15:21:19.000000 attune_project_api-24.2.9/attune_project_api/items/step_tuples/__init__.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1884 2024-04-24 15:21:19.000000 attune_project_api-24.2.9/attune_project_api/items/step_tuples/step_bootstrap_linux_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2612 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/items/step_tuples/step_group_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4915 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/items/step_tuples/step_project_link_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4640 2024-04-24 15:21:19.000000 attune_project_api-24.2.9/attune_project_api/items/step_tuples/step_push_design_file_compiled_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2596 2024-04-24 15:21:19.000000 attune_project_api-24.2.9/attune_project_api/items/step_tuples/step_push_design_file_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2866 2024-04-24 15:21:19.000000 attune_project_api-24.2.9/attune_project_api/items/step_tuples/step_sql_oracle_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1621 2024-04-24 15:21:19.000000 attune_project_api-24.2.9/attune_project_api/items/step_tuples/step_ssh_prompted_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3092 2024-04-24 15:21:19.000000 attune_project_api-24.2.9/attune_project_api/items/step_tuples/step_ssh_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1648 2024-04-24 15:21:19.000000 attune_project_api-24.2.9/attune_project_api/items/step_tuples/step_tcp_ping_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3015 2024-04-24 15:21:19.000000 attune_project_api-24.2.9/attune_project_api/items/step_tuples/step_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3461 2024-04-24 15:21:19.000000 attune_project_api-24.2.9/attune_project_api/items/step_tuples/step_winrm_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      544 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/key_util.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4275 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/migration.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-04-25 10:28:46.733561 attune_project_api-24.2.9/attune_project_api/remote/
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/remote/__init__.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     5301 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/remote/project_api_clone_controller.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4238 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/remote/project_api_clone_controller_test.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-04-25 10:28:46.735912 attune_project_api-24.2.9/attune_project_api/tuples/
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/tuples/__init__.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      366 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/tuples/git_commit_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1316 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/attune_project_api/tuples/project_modified_tuple.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-04-25 10:28:46.742077 attune_project_api-24.2.9/attune_project_api.egg-info/
+-rw-r--r--   0 jchesney   (501) staff       (20)      493 2024-04-25 10:28:46.000000 attune_project_api-24.2.9/attune_project_api.egg-info/PKG-INFO
+-rw-r--r--   0 jchesney   (501) staff       (20)     6360 2024-04-25 10:28:46.000000 attune_project_api-24.2.9/attune_project_api.egg-info/SOURCES.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)        1 2024-04-25 10:28:46.000000 attune_project_api-24.2.9/attune_project_api.egg-info/dependency_links.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)        1 2024-04-25 10:28:46.000000 attune_project_api-24.2.9/attune_project_api.egg-info/not-zip-safe
+-rw-r--r--   0 jchesney   (501) staff       (20)      127 2024-04-25 10:28:46.000000 attune_project_api-24.2.9/attune_project_api.egg-info/requires.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)       19 2024-04-25 10:28:46.000000 attune_project_api-24.2.9/attune_project_api.egg-info/top_level.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)       80 2024-04-25 10:28:46.743705 attune_project_api-24.2.9/setup.cfg
+-rw-r--r--   0 jchesney   (501) staff       (20)     2193 2024-04-25 10:28:46.000000 attune_project_api-24.2.9/setup.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-04-25 10:28:46.741257 attune_project_api-24.2.9/tests/
+-rw-r--r--   0 jchesney   (501) staff       (20)     5821 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/tests/test_error_handling.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    10907 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/tests/test_git_context.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3612 2024-04-15 07:51:52.000000 attune_project_api-24.2.9/tests/test_item_operations.py
```

### Comparing `attune-project-api-24.2.8/attune_project_api/Exceptions.py` & `attune_project_api-24.2.9/attune_project_api/Exceptions.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/ObjectStorageContext.py` & `attune_project_api-24.2.9/attune_project_api/ObjectStorageContext.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/RelationField.py` & `attune_project_api-24.2.9/attune_project_api/RelationField.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/StorageTuple.py` & `attune_project_api-24.2.9/attune_project_api/StorageTuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/TupleFieldValidators.py` & `attune_project_api-24.2.9/attune_project_api/TupleFieldValidators.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/TupleValidators.py` & `attune_project_api-24.2.9/attune_project_api/TupleValidators.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_contexts/GitLibMixin.py` & `attune_project_api-24.2.9/attune_project_api/_contexts/GitLibMixin.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_contexts/GitObjectStorageContext.py` & `attune_project_api-24.2.9/attune_project_api/_contexts/GitObjectStorageContext.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/RelationGraph.py` & `attune_project_api-24.2.9/attune_project_api/_private/RelationGraph.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/archive_format.py` & `attune_project_api-24.2.9/attune_project_api/_private/archive_format.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/archive_get_file_content.py` & `attune_project_api-24.2.9/attune_project_api/_private/archive_get_file_content.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/archive_hasher.py` & `attune_project_api-24.2.9/attune_project_api/_private/archive_hasher.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/archive_list_files.py` & `attune_project_api-24.2.9/attune_project_api/_private/archive_list_files.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/large_file_http_downloader.py` & `attune_project_api-24.2.9/attune_project_api/_private/large_file_http_downloader.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/large_file_http_downloader_test.py` & `attune_project_api-24.2.9/attune_project_api/_private/large_file_http_downloader_test.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/readme_compiler.py` & `attune_project_api-24.2.9/attune_project_api/_private/readme_compiler.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/ProjectReadme.md.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/ProjectReadme.md.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/ProjectReadmeAttune.md.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/ProjectReadmeAttune.md.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/ProjectReadmeContribute.md.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/ProjectReadmeContribute.md.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprint.html.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprint.html.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintBreadcrumbs.html.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintBreadcrumbs.html.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintHead.html.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintHead.html.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintHeader.html.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintHeader.html.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintRunWithAttune.html.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintRunWithAttune.html.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintScripts.html.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintScripts.html.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStep.html.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStep.html.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStepConnection.html.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStepConnection.html.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStepFile.html.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStepFile.html.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStepInner.html.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStepInner.html.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStepScript.html.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStepScript.html.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStepTcpPing.html.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintStepTcpPing.html.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintToc.html.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintToc.html.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintTocInner.html.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteBlueprintTocInner.html.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteIndex.html.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteIndex.html.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexAttuneAd.html.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexAttuneAd.html.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexBlueprintsList.html.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexBlueprintsList.html.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexFooter.html.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexFooter.html.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexHead.html.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexHead.html.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexHeader.html.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexHeader.html.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexJoinDiscord.html.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexJoinDiscord.html.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexNavBar.html.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexNavBar.html.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexScripts.html.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/ProjectWebsiteIndexScripts.html.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/templates/project_website/styles/ProjectWebsiteStyle.css.mako` & `attune_project_api-24.2.9/attune_project_api/_private/templates/project_website/styles/ProjectWebsiteStyle.css.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/website_compiler.py` & `attune_project_api-24.2.9/attune_project_api/_private/website_compiler.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/_private/website_compiler_test.py` & `attune_project_api-24.2.9/attune_project_api/_private/website_compiler_test.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/alembic.ini` & `attune_project_api-24.2.9/attune_project_api/alembic.ini`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/alembic_migrations/env.py` & `attune_project_api-24.2.9/attune_project_api/alembic_migrations/env.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/alembic_migrations/versions/0aa489aa66b2_store_name_in_project_metadata.py` & `attune_project_api-24.2.9/attune_project_api/alembic_migrations/versions/0aa489aa66b2_store_name_in_project_metadata.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/alembic_migrations/versions/145c6dc54454_rename_comment_md_to_readme_md_for_items.py` & `attune_project_api-24.2.9/attune_project_api/alembic_migrations/versions/145c6dc54454_rename_comment_md_to_readme_md_for_items.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/alembic_migrations/versions/58b1656aac40_move_sql_to_script_txt_file_in_oracle_.py` & `attune_project_api-24.2.9/attune_project_api/alembic_migrations/versions/58b1656aac40_move_sql_to_script_txt_file_in_oracle_.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/alembic_migrations/versions/ba6a8e4d7e2b_move_metadata_json_file_to_project_.py` & `attune_project_api-24.2.9/attune_project_api/alembic_migrations/versions/ba6a8e4d7e2b_move_metadata_json_file_to_project_.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/items/file_archive_tuples/file_archive_large_tuple.py` & `attune_project_api-24.2.9/attune_project_api/items/file_archive_tuples/file_archive_large_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/items/file_archive_tuples/file_archive_tuple.py` & `attune_project_api-24.2.9/attune_project_api/items/file_archive_tuples/file_archive_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/items/file_archive_tuples/file_archive_versioned_tuple.py` & `attune_project_api-24.2.9/attune_project_api/items/file_archive_tuples/file_archive_versioned_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/items/parameter_tuple.py` & `attune_project_api-24.2.9/attune_project_api/items/parameter_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/items/project_metadata_tuple.py` & `attune_project_api-24.2.9/attune_project_api/items/project_metadata_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/items/step_tuples/__init__.py` & `attune_project_api-24.2.9/attune_project_api/items/step_tuples/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         stepNiceNames[cls.tupleType()] = niceName
         STEP_TYPES[cls.tupleType()] = cls
         return cls
 
     return f
 
 
-def extractTextPlaceholders(text):
+def extractScriptReferences(text):
     # NOTE, Duplicated client side, AttunePlaceholderMod.js,
     # $scope.textPhName = function () { ...
     return re.findall(r"(?<![$]){([A-Za-z0-9_.]+)}", text)
 
 
 def loadStorageStepTuples():
     from . import step_sql_oracle_tuple
```

### Comparing `attune-project-api-24.2.8/attune_project_api/items/step_tuples/step_bootstrap_linux_tuple.py` & `attune_project_api-24.2.9/attune_project_api/items/step_tuples/step_bootstrap_linux_tuple.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+from vortex.Tuple import TupleField
+from vortex.Tuple import addTupleType
+
 from attune_project_api import ObjectStorageContext
 from attune_project_api import ParameterTuple
 from attune_project_api.RelationField import RelationField
 from attune_project_api.items import NotZeroLenStr
 from attune_project_api.items.step_tuples import addStepDeclarative
 from attune_project_api.items.step_tuples.step_tuple import (
     StepFieldNeedingSubstitution,
 )
 from attune_project_api.items.step_tuples.step_tuple import StepTuple
 from attune_project_api.items.step_tuples.step_tuple import StepTupleTypeEnum
-from vortex.Tuple import TupleField
-from vortex.Tuple import addTupleType
 
 
 @ObjectStorageContext.registerItemClass
 @addStepDeclarative("Setup Linux SSH Keys")
 @addTupleType
 class StepBootstrapLinuxTuple(StepTuple):
     __tupleType__ = StepTupleTypeEnum.BOOTSTRAP_LINUX.value
@@ -39,19 +40,15 @@
     def fieldsNeedingSubstitutions(
         self,
     ) -> list[StepFieldNeedingSubstitution]:
         return [
             StepFieldNeedingSubstitution(
                 fieldName="server",
                 displayName="Target SSH Node",
-                value=self.server,
-                isScriptOrCode=False,
-                order=0,
+                value=self.server,                isScriptReference = (False,)order=0,
             ),
             StepFieldNeedingSubstitution(
                 fieldName="osCred",
                 displayName="SSH Credential",
-                value=self.osCred,
-                isScriptOrCode=False,
-                order=1,
+                value=self.osCred,                isScriptReference = (False,)order=1,
             ),
         ]
```

### Comparing `attune-project-api-24.2.8/attune_project_api/items/step_tuples/step_group_tuple.py` & `attune_project_api-24.2.9/attune_project_api/items/step_tuples/step_group_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/items/step_tuples/step_project_link_tuple.py` & `attune_project_api-24.2.9/attune_project_api/items/step_tuples/step_project_link_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/items/step_tuples/step_push_design_file_compiled_tuple.py` & `attune_project_api-24.2.9/attune_project_api/items/step_tuples/step_push_design_file_compiled_tuple.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,22 +7,23 @@
  *
  *  All rights to this software are reserved by
  *  ServerTribe HQ Pty Ltd
  *
 """
 import logging
 
+from vortex.Tuple import TupleField
+from vortex.Tuple import addTupleType
+
 from attune_project_api import ObjectStorageContext
 from attune_project_api.items.file_archive_tuples.file_archive_tuple import (
     FileArchiveTuple,
 )
-from vortex.Tuple import TupleField
-from vortex.Tuple import addTupleType
 from . import addStepDeclarative
-from . import extractTextPlaceholders
+from . import extractScriptReferences
 from .step_tuple import StepFieldNeedingSubstitution
 from .step_tuple import StepTuple
 from .step_tuple import StepTupleTypeEnum
 from .. import NotZeroLenStr
 from ..parameter_tuple import ParameterTuple
 from ...RelationField import RelationField
 from ...StorageTuple import StorageMemberTuple
@@ -89,51 +90,43 @@
 
     def parameters(self) -> list["ParameterTuple"]:
         return [self.server, self.osCred] + [
             param.parameter for param in self.makoParameters
         ]
 
     def scriptReferences(self) -> list[str]:
-        return extractTextPlaceholders(self.deployPath)
+        return extractScriptReferences(self.deployPath)
 
     def fieldsNeedingSubstitutions(
         self,
     ) -> list[StepFieldNeedingSubstitution]:
         results = [
             StepFieldNeedingSubstitution(
                 fieldName="server",
                 displayName="Target Node",
-                value=self.server,
-                isScriptOrCode=False,
-                order=0,
+                value=self.server,                isScriptReference = (False,)order=0,
             ),
             StepFieldNeedingSubstitution(
                 fieldName="osCred",
                 displayName="Target Node Credential",
-                value=self.osCred,
-                isScriptOrCode=False,
-                order=1,
+                value=self.osCred,                isScriptReference = (False,)order=1,
             ),
             StepFieldNeedingSubstitution(
                 fieldName="deployPath",
                 displayName="Remote Deployment Path",
-                value=self.deployPath,
-                isScriptOrCode=False,
-                order=2,
+                value=self.deployPath,                isScriptReference = (False,)order=2,
             ),
         ]
 
         for param in self.makoParameters:
             results.append(
                 StepFieldNeedingSubstitution(
                     fieldName="makoParameters[%s]" % param.name,
                     displayName="Mako Parameter: %s" % param.name,
-                    value=param.parameter,
-                    isScriptOrCode=False,
-                    order=10 + len(results),
+                    value=param.parameter,                    isScriptReference = (False,)order=10 + len(results),
                 )
             )
 
         return results
 
     @property
     def hasErrors(self) -> bool:
```

### Comparing `attune-project-api-24.2.8/attune_project_api/items/step_tuples/step_push_design_file_tuple.py` & `attune_project_api-24.2.9/attune_project_api/items/step_tuples/step_push_design_file_tuple.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
+from vortex.Tuple import TupleField
+from vortex.Tuple import addTupleType
+
 from attune_project_api import ObjectStorageContext
 from attune_project_api import ParameterTuple
 from attune_project_api.RelationField import RelationField
 from attune_project_api.items import NotZeroLenStr
 from attune_project_api.items.file_archive_tuples.file_archive_tuple import (
     FileArchiveTuple,
 )
 from attune_project_api.items.step_tuples import addStepDeclarative
-from attune_project_api.items.step_tuples import extractTextPlaceholders
+from attune_project_api.items.step_tuples import extractScriptReferences
 from attune_project_api.items.step_tuples.step_tuple import (
     StepFieldNeedingSubstitution,
 )
 from attune_project_api.items.step_tuples.step_tuple import StepTuple
 from attune_project_api.items.step_tuples.step_tuple import StepTupleTypeEnum
-from vortex.Tuple import TupleField
-from vortex.Tuple import addTupleType
 
 
 @ObjectStorageContext.registerItemClass
 @addStepDeclarative("Push Files")
 @addTupleType
 class StepPushDesignFileTuple(StepTuple):
     __tupleType__ = StepTupleTypeEnum.PUSH_DESIGN_FILE.value
@@ -41,35 +42,29 @@
         referenceKeyFieldName="archiveKey",
     )
 
     def parameters(self) -> list["ParameterTuple"]:
         return [self.server, self.osCred]
 
     def scriptReferences(self) -> list[str]:
-        return extractTextPlaceholders(self.deployPath)
+        return extractScriptReferences(self.deployPath)
 
     def fieldsNeedingSubstitutions(
         self,
     ) -> list[StepFieldNeedingSubstitution]:
         return [
             StepFieldNeedingSubstitution(
                 fieldName="server",
                 displayName="Target Node",
-                value=self.server,
-                isScriptOrCode=False,
-                order=0,
+                value=self.server,                isScriptReference = (False,)order=0,
             ),
             StepFieldNeedingSubstitution(
                 fieldName="osCred",
                 displayName="Target Node Credential",
-                value=self.osCred,
-                isScriptOrCode=False,
-                order=1,
+                value=self.osCred,                isScriptReference = (False,)order=1,
             ),
             StepFieldNeedingSubstitution(
                 fieldName="deployPath",
                 displayName="Remote Deployment Path",
-                value=self.deployPath,
-                isScriptOrCode=False,
-                order=2,
+                value=self.deployPath,                isScriptReference = (False,)order=2,
             ),
         ]
```

### Comparing `attune-project-api-24.2.8/attune_project_api/items/step_tuples/step_sql_oracle_tuple.py` & `attune_project_api-24.2.9/attune_project_api/items/step_tuples/step_sql_oracle_tuple.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,19 +7,20 @@
  *
  *  All rights to this software are reserved by
  *  ServerTribe HQ Pty Ltd
  *
 """
 from typing import Optional
 
-from attune_project_api.items import NotZeroLenStr
 from vortex.Tuple import TupleField
 from vortex.Tuple import addTupleType
+
+from attune_project_api.items import NotZeroLenStr
 from . import addStepDeclarative
-from . import extractTextPlaceholders
+from . import extractScriptReferences
 from .step_tuple import StepFieldNeedingSubstitution
 from .step_tuple import StepTuple
 from .step_tuple import StepTupleTypeEnum
 from ... import ParameterTuple
 from ...ObjectStorageContext import ObjectStorageContext
 from ...RelationField import RelationField
 
@@ -51,42 +52,34 @@
         referenceKeyFieldName="sqlCredKey",
     )
 
     def parameters(self) -> list["ParameterTuple"]:
         return [self.server, self.osCred, self.sqlCred]
 
     def scriptReferences(self) -> list[str]:
-        return extractTextPlaceholders(self.sql)
+        return extractScriptReferences(self.sql)
 
     def fieldsNeedingSubstitutions(
         self,
     ) -> list[StepFieldNeedingSubstitution]:
         return [
             StepFieldNeedingSubstitution(
                 fieldName="server",
                 displayName="Target SSH Node",
-                value=self.server,
-                isScriptOrCode=False,
-                order=0,
+                value=self.server,                isScriptReference = (False,)order=0,
             ),
             StepFieldNeedingSubstitution(
                 fieldName="osCred",
                 displayName="SSH Credential",
-                value=self.osCred,
-                isScriptOrCode=False,
-                order=1,
+                value=self.osCred,                isScriptReference = (False,)order=1,
             ),
             StepFieldNeedingSubstitution(
                 fieldName="sqlCred",
                 displayName="Oracle SQL Credential",
-                value=self.sqlCred,
-                isScriptOrCode=False,
-                order=2,
+                value=self.sqlCred,                isScriptReference = (False,)order=2,
             ),
             StepFieldNeedingSubstitution(
                 fieldName="sql",
                 displayName="SQL / PLSql",
-                value=self.sql,
-                isScriptOrCode=True,
-                order=3,
+                value=self.sql,                isScriptReference = (True,)order=3,
             ),
         ]
```

### Comparing `attune-project-api-24.2.8/attune_project_api/items/step_tuples/step_ssh_prompted_tuple.py` & `attune_project_api-24.2.9/attune_project_api/items/step_tuples/step_ssh_prompted_tuple.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,43 @@
+from vortex.Tuple import TupleField
+from vortex.Tuple import addTupleType
+
 from attune_project_api import ObjectStorageContext
 from attune_project_api import ParameterTuple
 from attune_project_api.items import NotZeroLenStr
 from attune_project_api.items.step_tuples import addStepDeclarative
-from attune_project_api.items.step_tuples import extractTextPlaceholders
+from attune_project_api.items.step_tuples import extractScriptReferences
 from attune_project_api.items.step_tuples.step_ssh_tuple import StepSshTuple
 from attune_project_api.items.step_tuples.step_tuple import (
     StepFieldNeedingSubstitution,
 )
 from attune_project_api.items.step_tuples.step_tuple import StepTupleTypeEnum
-from vortex.Tuple import TupleField
-from vortex.Tuple import addTupleType
 
 
 @ObjectStorageContext.registerItemClass
 @addStepDeclarative("Execute Linux Script With Responses")
 @addTupleType
 class StepSshPromptedTuple(StepSshTuple):
     __tupleType__ = StepTupleTypeEnum.SSH_PROMPTED.value
 
     promptResponses: NotZeroLenStr = TupleField()
 
     def parameters(self) -> list["ParameterTuple"]:
-        return [self.server, self.osCred]
+        return StepSshTuple.parameters(self)
 
     def scriptReferences(self) -> list[str]:
-        return extractTextPlaceholders(self.script + self.promptResponses)
+        return StepSshTuple.scriptReferences(self) + extractScriptReferences(
+            self.promptResponses
+        )
 
     def fieldsNeedingSubstitutions(
         self,
     ) -> list[StepFieldNeedingSubstitution]:
         results = StepSshTuple.fieldsNeedingSubstitutions(self)
         results.append(
             StepFieldNeedingSubstitution(
                 fieldName="promptResponses",
                 displayName="Prompt Responses",
-                value=self.promptResponses,
-                isScriptOrCode=False,
-                order=len(results),
+                value=self.promptResponses,                isScriptReference = (False,)order=len(results),
             )
         )
         return results
```

### Comparing `attune-project-api-24.2.8/attune_project_api/items/step_tuples/step_ssh_tuple.py` & `attune_project_api-24.2.9/attune_project_api/items/step_tuples/step_ssh_tuple.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
  *
 """
 
 from vortex.Tuple import TupleField
 from vortex.Tuple import addTupleType
 
 from . import addStepDeclarative
-from . import extractTextPlaceholders
+from . import extractScriptReferences
 from .step_tuple import StepFieldNeedingSubstitution
 from .step_tuple import StepTupleTypeEnum
 from .. import NotZeroLenStr
 from ... import ParameterTuple
 from ... import StepTuple
 from ...ObjectStorageContext import ObjectStorageContext
 from ...RelationField import RelationField
@@ -73,35 +73,29 @@
         referenceKeyFieldName="osCredKey",
     )
 
     def parameters(self) -> list["ParameterTuple"]:
         return [self.server, self.osCred]
 
     def scriptReferences(self) -> list[str]:
-        return extractTextPlaceholders(self.script)
+        return extractScriptReferences(self.script)
 
     def fieldsNeedingSubstitutions(
         self,
     ) -> list[StepFieldNeedingSubstitution]:
         return [
             StepFieldNeedingSubstitution(
                 fieldName="server",
                 displayName="Target SSH Node",
-                value=self.server,
-                isScriptOrCode=False,
-                order=0,
+                value=self.server,                isScriptReference = (False,)order=0,
             ),
             StepFieldNeedingSubstitution(
                 fieldName="osCred",
                 displayName="SSH Credential",
-                value=self.osCred,
-                isScriptOrCode=False,
-                order=1,
+                value=self.osCred,                isScriptReference = (False,)order=1,
             ),
             StepFieldNeedingSubstitution(
                 fieldName="script",
                 displayName="Script",
-                value=self.script,
-                isScriptOrCode=True,
-                order=2,
+                value=self.script,                isScriptReference = (True,)order=2,
             ),
         ]
```

### Comparing `attune-project-api-24.2.8/attune_project_api/items/step_tuples/step_tcp_ping_tuple.py` & `attune_project_api-24.2.9/attune_project_api/items/step_tuples/step_tcp_ping_tuple.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,12 +49,10 @@
     def fieldsNeedingSubstitutions(
         self,
     ) -> list[StepFieldNeedingSubstitution]:
         return [
             StepFieldNeedingSubstitution(
                 fieldName="server",
                 displayName="Target Node",
-                value=self.server,
-                isScriptOrCode=False,
-                order=0,
+                value=self.server,                isScriptReference = (False,)order=0,
             )
         ]
```

### Comparing `attune-project-api-24.2.8/attune_project_api/items/step_tuples/step_tuple.py` & `attune_project_api-24.2.9/attune_project_api/items/step_tuples/step_tuple.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from abc import ABCMeta
 from collections import namedtuple
 from enum import Enum
 from typing import Optional
 
+from vortex.Tuple import PolymorphicTupleTypeFieldArg
+from vortex.Tuple import TupleField
+
 from attune_project_api import ObjectStorageContext
 from attune_project_api import StorageTuple
 from attune_project_api.StorageTuple import ItemStorageGroupEnum
 from attune_project_api.items import NotZeroLenStr
-from vortex.Tuple import PolymorphicTupleTypeFieldArg
-from vortex.Tuple import TupleField
 
 
 class StepTupleTypeEnum(Enum):
     GROUP = "com.servertribe.attune.tuples.StepGroupTuple"
     SQL_ORACLE = "com.servertribe.attune.tuples.StepSqlOracleTuple"
     SSH = "com.servertribe.attune.tuples.StepSshTuple"
     SSH_PROMPTED = "com.servertribe.attune.tuples.StepSshPromptedTuple"
@@ -33,15 +34,15 @@
 class StepTupleActionOnStepFailEnum:
     STOP_ON_ERROR = "stop"
     CONTINUE_ON_ERROR = "continue"
 
 
 StepFieldNeedingSubstitution = namedtuple(
     "StepFieldNeedingSubstitution",
-    ("fieldName", "displayName", "value", "isScriptOrCode", "order"),
+    ("fieldName", "displayName", "value", "isScriptReference", "order"),
 )
 
 
 @ObjectStorageContext.registerItemClass
 class StepTuple(StorageTuple, metaclass=ABCMeta):
     __tupleArgs__ = (PolymorphicTupleTypeFieldArg("type"),)
     __group__ = ItemStorageGroupEnum.Step
```

### Comparing `attune-project-api-24.2.8/attune_project_api/items/step_tuples/step_winrm_tuple.py` & `attune_project_api-24.2.9/attune_project_api/items/step_tuples/step_winrm_tuple.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,19 +7,20 @@
  *
  *  All rights to this software are reserved by
  *  ServerTribe HQ Pty Ltd
  *
 """
 from typing import Optional
 
-from attune_project_api.items import NotZeroLenStr
 from vortex.Tuple import TupleField
 from vortex.Tuple import addTupleType
+
+from attune_project_api.items import NotZeroLenStr
 from . import addStepDeclarative
-from . import extractTextPlaceholders
+from . import extractScriptReferences
 from .step_tuple import StepFieldNeedingSubstitution
 from .step_tuple import StepTupleTypeEnum
 from ... import ParameterTuple
 from ... import StepTuple
 from ...ObjectStorageContext import ObjectStorageContext
 from ...RelationField import RelationField
 
@@ -71,38 +72,32 @@
     def interpreterWinCmd(self):
         return STEP_WIN_CMD_INTERPRETERS[self.interpreter]
 
     def parameters(self) -> list["ParameterTuple"]:
         return [self.server, self.osCred]
 
     def scriptReferences(self) -> list[str]:
-        textPh = extractTextPlaceholders(self.script)
+        textPh = extractScriptReferences(self.script)
         if self.interpreterCommand:
-            textPh += extractTextPlaceholders(self.interpreterCommand)
+            textPh += extractScriptReferences(self.interpreterCommand)
         return textPh
 
     def fieldsNeedingSubstitutions(
         self,
     ) -> list[StepFieldNeedingSubstitution]:
         return [
             StepFieldNeedingSubstitution(
                 fieldName="server",
                 displayName="Target WinRM Node",
-                value=self.server,
-                isScriptOrCode=False,
-                order=0,
+                value=self.server,                isScriptReference = (False,)order=0,
             ),
             StepFieldNeedingSubstitution(
                 fieldName="osCred",
                 displayName="WinRM Credential",
-                value=self.osCred,
-                isScriptOrCode=False,
-                order=1,
+                value=self.osCred,                isScriptReference = (False,)order=1,
             ),
             StepFieldNeedingSubstitution(
                 fieldName="script",
                 displayName="Script",
-                value=self.script,
-                isScriptOrCode=True,
-                order=2,
+                value=self.script,                isScriptReference = (True,)order=2,
             ),
         ]
```

### Comparing `attune-project-api-24.2.8/attune_project_api/key_util.py` & `attune_project_api-24.2.9/attune_project_api/key_util.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/migration.py` & `attune_project_api-24.2.9/attune_project_api/migration.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/remote/project_api_clone_controller.py` & `attune_project_api-24.2.9/attune_project_api/remote/project_api_clone_controller.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/remote/project_api_clone_controller_test.py` & `attune_project_api-24.2.9/attune_project_api/remote/project_api_clone_controller_test.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api/tuples/project_modified_tuple.py` & `attune_project_api-24.2.9/attune_project_api/tuples/project_modified_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/attune_project_api.egg-info/SOURCES.txt` & `attune_project_api-24.2.9/attune_project_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/setup.py` & `attune_project_api-24.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import shutil
 
 from setuptools import find_packages
 from setuptools import setup
 
 pip_package_name = "attune-project-api"
 py_package_folder = "attune_project_api"
-package_version = '24.2.8'
+package_version = '24.2.9'
 
 egg_info = "%s.egg-info" % pip_package_name
 if os.path.isdir(egg_info):
     shutil.rmtree(egg_info)
 
 if os.path.isfile("MANIFEST"):
     os.remove("MANIFEST")
```

### Comparing `attune-project-api-24.2.8/tests/test_error_handling.py` & `attune_project_api-24.2.9/tests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/tests/test_git_context.py` & `attune_project_api-24.2.9/tests/test_git_context.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-24.2.8/tests/test_item_operations.py` & `attune_project_api-24.2.9/tests/test_item_operations.py`

 * *Files identical despite different names*

