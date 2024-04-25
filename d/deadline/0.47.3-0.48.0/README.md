# Comparing `tmp/deadline-0.47.3.tar.gz` & `tmp/deadline-0.48.0.tar.gz`

## Comparing `deadline-0.47.3.tar` & `deadline-0.48.0.tar`

### file list

```diff
@@ -1,107 +1,108 @@
--rw-r--r--   0        0        0    50578 2020-02-02 00:00:00.000000 deadline-0.47.3/THIRD_PARTY_LICENSES
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.47.3/_version.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/__main__.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/_version.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/exceptions.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/py.typed
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/api/__init__.py
--rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/api/_list_apis.py
--rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/api/_loginout.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/api/_queue_parameters.py
--rw-r--r--   0        0        0    13355 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/api/_session.py
--rw-r--r--   0        0        0    17160 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/api/_submit_job_bundle.py
--rw-r--r--   0        0        0    14070 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/api/_telemetry.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/__init__.py
--rw-r--r--   0        0        0     6214 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_common.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_deadline_cli.py
--rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_deadline_web_url.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/deadline_cli_main.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/deadline_dev_gui_main.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_groups/__init__.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_groups/_sigint_handler.py
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_groups/auth_group.py
--rw-r--r--   0        0        0    10522 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_groups/bundle_group.py
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_groups/config_group.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_groups/farm_group.py
--rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_groups/fleet_group.py
--rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_groups/handle_web_url_command.py
--rw-r--r--   0        0        0    39347 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_groups/job_group.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_groups/queue_group.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_groups/worker_group.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/config/__init__.py
--rw-r--r--   0        0        0    17510 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/config/config_file.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/job_bundle/__init__.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/job_bundle/_yaml.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/job_bundle/adaptors.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/job_bundle/job_template.py
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/job_bundle/loader.py
--rw-r--r--   0        0        0    32688 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/job_bundle/parameters.py
--rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/job_bundle/submission.py
--rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/__init__.py
--rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/cli_job_submitter.py
--rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/deadline_authentication_status.py
--rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/dev_application.py
--rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/job_bundle_submitter.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/dataclasses/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/dialogs/__init__.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/dialogs/_types.py
--rw-r--r--   0        0        0    34201 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/dialogs/deadline_config_dialog.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/dialogs/deadline_login_dialog.py
--rw-r--r--   0        0        0    26025 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/dialogs/submit_job_progress_dialog.py
--rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/dialogs/submit_job_to_deadline_dialog.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/resources/deadline_logo.svg
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/resources/info.svg
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/resources/blender_example_bundle/template.yaml
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/resources/cli_job_bundle/template.yaml
--rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/resources/controls_demo_job_bundle/template.yaml
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/widgets/__init__.py
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/widgets/cli_job_settings_tab.py
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/widgets/deadline_authentication_status_widget.py
--rw-r--r--   0        0        0    36343 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/widgets/host_requirements_tab.py
--rw-r--r--   0        0        0    14402 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/widgets/job_attachments_tab.py
--rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/widgets/job_bundle_settings_tab.py
--rw-r--r--   0        0        0    31193 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/widgets/openjd_parameters_widget.py
--rw-r--r--   0        0        0     8735 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/widgets/path_widgets.py
--rw-r--r--   0        0        0    23261 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/widgets/shared_job_settings_tab.py
--rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/widgets/spinbox_widgets.py
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/README.md
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/__init__.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/_utils.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/_version.py
--rw-r--r--   0        0        0    28207 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/asset_sync.py
--rw-r--r--   0        0        0    46754 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/download.py
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/exceptions.py
--rw-r--r--   0        0        0    10861 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/models.py
--rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/os_file_permission.py
--rw-r--r--   0        0        0    15063 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/progress_tracker.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/py.typed
--rw-r--r--   0        0        0    52783 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/upload.py
--rw-r--r--   0        0        0    21984 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/vfs.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/_aws/__init__.py
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/_aws/aws_clients.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/_aws/aws_config.py
--rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/_aws/deadline.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/_windows/__init__.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/_windows/file.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/asset_manifests/__init__.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/asset_manifests/_canonical_json.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/asset_manifests/base_manifest.py
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/asset_manifests/decode.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/asset_manifests/hash_algorithms.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/asset_manifests/manifest_model.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/asset_manifests/versions.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/asset_manifests/schemas/2023-03-03.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/asset_manifests/v2023_03_03/__init__.py
--rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/asset_manifests/v2023_03_03/asset_manifest.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/caches/__init__.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/caches/cache_db.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/caches/hash_cache.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/caches/s3_check_cache.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 deadline-0.47.3/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline-0.47.3/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline-0.47.3/NOTICE
--rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 deadline-0.47.3/README.md
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 deadline-0.47.3/hatch.toml
--rw-r--r--   0        0        0     6717 2020-02-02 00:00:00.000000 deadline-0.47.3/pyproject.toml
--rw-r--r--   0        0        0     7931 2020-02-02 00:00:00.000000 deadline-0.47.3/PKG-INFO
+-rw-r--r--   0        0        0    50578 2020-02-02 00:00:00.000000 deadline-0.48.0/THIRD_PARTY_LICENSES
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.48.0/_version.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/__main__.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/_version.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/exceptions.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/py.typed
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/api/__init__.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/api/_get_storage_profile_for_queue.py
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/api/_list_apis.py
+-rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/api/_loginout.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/api/_queue_parameters.py
+-rw-r--r--   0        0        0    13355 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/api/_session.py
+-rw-r--r--   0        0        0    18628 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/api/_submit_job_bundle.py
+-rw-r--r--   0        0        0    14070 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/api/_telemetry.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/__init__.py
+-rw-r--r--   0        0        0     6214 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_common.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_deadline_cli.py
+-rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_deadline_web_url.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/deadline_cli_main.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/deadline_dev_gui_main.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_groups/__init__.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_groups/_sigint_handler.py
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_groups/auth_group.py
+-rw-r--r--   0        0        0    12134 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_groups/bundle_group.py
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_groups/config_group.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_groups/farm_group.py
+-rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_groups/fleet_group.py
+-rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_groups/handle_web_url_command.py
+-rw-r--r--   0        0        0    39347 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_groups/job_group.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_groups/queue_group.py
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_groups/worker_group.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/config/__init__.py
+-rw-r--r--   0        0        0    17510 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/config/config_file.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/job_bundle/__init__.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/job_bundle/_yaml.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/job_bundle/adaptors.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/job_bundle/job_template.py
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/job_bundle/loader.py
+-rw-r--r--   0        0        0    32688 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/job_bundle/parameters.py
+-rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/job_bundle/submission.py
+-rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/__init__.py
+-rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/cli_job_submitter.py
+-rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/deadline_authentication_status.py
+-rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/dev_application.py
+-rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/job_bundle_submitter.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/dataclasses/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/dialogs/__init__.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/dialogs/_types.py
+-rw-r--r--   0        0        0    34196 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/dialogs/deadline_config_dialog.py
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/dialogs/deadline_login_dialog.py
+-rw-r--r--   0        0        0    29733 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/dialogs/submit_job_progress_dialog.py
+-rw-r--r--   0        0        0    20978 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/dialogs/submit_job_to_deadline_dialog.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/resources/deadline_logo.svg
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/resources/info.svg
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/resources/blender_example_bundle/template.yaml
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/resources/cli_job_bundle/template.yaml
+-rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/resources/controls_demo_job_bundle/template.yaml
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/widgets/__init__.py
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/widgets/cli_job_settings_tab.py
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/widgets/deadline_authentication_status_widget.py
+-rw-r--r--   0        0        0    36343 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/widgets/host_requirements_tab.py
+-rw-r--r--   0        0        0    15622 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/widgets/job_attachments_tab.py
+-rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/widgets/job_bundle_settings_tab.py
+-rw-r--r--   0        0        0    31193 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/widgets/openjd_parameters_widget.py
+-rw-r--r--   0        0        0     8735 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/widgets/path_widgets.py
+-rw-r--r--   0        0        0    23261 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/widgets/shared_job_settings_tab.py
+-rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/widgets/spinbox_widgets.py
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/README.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/__init__.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/_utils.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/_version.py
+-rw-r--r--   0        0        0    28207 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/asset_sync.py
+-rw-r--r--   0        0        0    46754 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/download.py
+-rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/exceptions.py
+-rw-r--r--   0        0        0    10785 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/models.py
+-rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/os_file_permission.py
+-rw-r--r--   0        0        0    15063 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/progress_tracker.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/py.typed
+-rw-r--r--   0        0        0    52996 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/upload.py
+-rw-r--r--   0        0        0    21984 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/vfs.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/_aws/__init__.py
+-rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/_aws/aws_clients.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/_aws/aws_config.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/_aws/deadline.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/_windows/__init__.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/_windows/file.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/asset_manifests/__init__.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/asset_manifests/_canonical_json.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/asset_manifests/base_manifest.py
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/asset_manifests/decode.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/asset_manifests/hash_algorithms.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/asset_manifests/manifest_model.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/asset_manifests/versions.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/asset_manifests/schemas/2023-03-03.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/asset_manifests/v2023_03_03/__init__.py
+-rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/asset_manifests/v2023_03_03/asset_manifest.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/caches/__init__.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/caches/cache_db.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/caches/hash_cache.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/caches/s3_check_cache.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 deadline-0.48.0/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline-0.48.0/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline-0.48.0/NOTICE
+-rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 deadline-0.48.0/README.md
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 deadline-0.48.0/hatch.toml
+-rw-r--r--   0        0        0     6722 2020-02-02 00:00:00.000000 deadline-0.48.0/pyproject.toml
+-rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 deadline-0.48.0/PKG-INFO
```

### Comparing `deadline-0.47.3/THIRD_PARTY_LICENSES` & `deadline-0.48.0/THIRD_PARTY_LICENSES`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/exceptions.py` & `deadline-0.48.0/src/deadline/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/api/__init__.py` & `deadline-0.48.0/src/deadline/client/api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     "list_jobs",
     "list_fleets",
     "list_storage_profiles_for_queue",
     "get_queue_user_boto3_session",
     "get_queue_parameter_definitions",
     "get_telemetry_client",
     "get_deadline_cloud_library_telemetry_client",
+    "get_storage_profile_for_queue",
 ]
 
 # The following import is needed to prevent the following sporadic failure:
 # botocore.exceptions.HTTPClientError: An HTTP Client raised an unhandled exception: unknown
 # encoding: idna
 import encodings.idna  # noqa # pylint: disable=unused-import
 from configparser import ConfigParser
@@ -53,14 +54,15 @@
 from ._queue_parameters import get_queue_parameter_definitions
 from ._submit_job_bundle import create_job_from_job_bundle, wait_for_create_job_to_complete
 from ._telemetry import (
     get_telemetry_client,
     get_deadline_cloud_library_telemetry_client,
     TelemetryClient,
 )
+from ._get_storage_profile_for_queue import get_storage_profile_for_queue
 
 logger = getLogger(__name__)
 
 
 def check_deadline_api_available(config: Optional[ConfigParser] = None) -> bool:
     """
     Returns True if AWS Deadline Cloud APIs are authorized in the session,
```

### Comparing `deadline-0.47.3/src/deadline/client/api/_list_apis.py` & `deadline-0.48.0/src/deadline/client/api/_list_apis.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/api/_loginout.py` & `deadline-0.48.0/src/deadline/client/api/_loginout.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/api/_queue_parameters.py` & `deadline-0.48.0/src/deadline/client/api/_queue_parameters.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/api/_session.py` & `deadline-0.48.0/src/deadline/client/api/_session.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/api/_submit_job_bundle.py` & `deadline-0.48.0/src/deadline/client/api/_submit_job_bundle.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,18 +28,20 @@
 from ..job_bundle.parameters import (
     apply_job_parameters,
     merge_queue_job_parameters,
     read_job_bundle_parameters,
     JobParameter,
 )
 from ..job_bundle.submission import AssetReferences, split_parameter_args
+from ...job_attachments.exceptions import MisconfiguredInputsError
 from ...job_attachments.models import (
     JobAttachmentsFileSystem,
     AssetRootGroup,
     AssetRootManifest,
+    AssetUploadGroup,
     JobAttachmentS3Settings,
 )
 from ...job_attachments.progress_tracker import SummaryStatistics, ProgressReportMetadata
 from ...job_attachments.upload import S3AssetManager
 
 logger = logging.getLogger(__name__)
 
@@ -53,29 +55,30 @@
     job_attachments_file_system: Optional[str] = None,
     config: Optional[ConfigParser] = None,
     priority: Optional[int] = None,
     max_failed_tasks_count: Optional[int] = None,
     max_retries_per_task: Optional[int] = None,
     print_function_callback: Callable[[str], None] = lambda msg: None,
     decide_cancel_submission_callback: Callable[
-        [dict[str, int], int, int], bool
-    ] = lambda paths, files, bytes: False,
+        [AssetUploadGroup], bool
+    ] = lambda upload_group: False,
     hashing_progress_callback: Optional[Callable[[ProgressReportMetadata], bool]] = None,
     upload_progress_callback: Optional[Callable[[ProgressReportMetadata], bool]] = None,
     create_job_result_callback: Optional[Callable[[], bool]] = None,
+    require_paths_exist: bool = False,
 ) -> Union[str, None]:
     """
     Creates a job in the AWS Deadline Cloud farm/queue configured as default for the
     workstation from the job bundle in the provided directory.
 
     A job bundle has the following directory structure:
 
     /template.json|yaml (required): An Open Job Description job template that specifies the work to be done. Job parameters
             are embedded here.
-    /parameter_values.yson|yaml (optional): If provided, these are parameter values for the job template and for
+    /parameter_values.json|yaml (optional): If provided, these are parameter values for the job template and for
             the render farm. AWS Deadline Cloud-specific parameters are like "deadline:priority".
             Looks like:
             {
                 "parameterValues": [
                     {"name": "<name>", "value": "<value>"},
                     ...
                 ]
@@ -122,15 +125,15 @@
         decide_cancel_submission_callback (Callable dict[str, int], int, int -> bool): If the job has job
                 attachments, decide whether or not to cancel the submission given what assets will
                 or will not be uploaded. If returns true, the submission is canceled. If False,
                 the submission continues. By default the submission always continues.
         hashing_progress_callback / upload_progress_callback / create_job_result_callback (Callable -> bool):
                 Callbacks periodically called while hashing / uploading / waiting for job creation. If returns false,
                 the operation will be cancelled. If return true, the operation continues. Default behavior for each
-                is to not cancel the operation. hashing_progress_callback and upload_progress_callback both recieve
+                is to not cancel the operation. hashing_progress_callback and upload_progress_callback both receive
                 ProgressReport as a parameter, which can be used for projecting remaining time, as in done in the CLI.
     """
 
     # Ensure the job bundle doesn't contain files that resolve outside of the bundle directory
     validate_directory_symlink_containment(job_bundle_dir)
 
     # Read in the job template
@@ -167,16 +170,20 @@
         "queueId": queue_id,
         "template": file_contents,
         "templateType": file_type,
         "priority": 50,
     }
 
     storage_profile_id = get_setting("settings.storage_profile_id", config=config)
+    storage_profile = None
     if storage_profile_id:
         create_job_args["storageProfileId"] = storage_profile_id
+        storage_profile = api.get_storage_profile_for_queue(
+            farm_id, queue_id, storage_profile_id, deadline
+        )
 
     # The job parameters
     job_bundle_parameters = read_job_bundle_parameters(job_bundle_dir)
 
     asset_references_obj = read_yaml_or_json_object(
         job_bundle_dir, "asset_references", required=False
     )
@@ -202,21 +209,50 @@
     app_parameters_formatted, job_parameters_formatted = split_parameter_args(
         parameters, job_bundle_dir
     )
 
     # Hash and upload job attachments if there are any
     if asset_references and "jobAttachmentSettings" in queue:
         # Extend input_filenames with all the files in the input_directories
+        missing_directories: set[str] = set()
         for directory in asset_references.input_directories:
+            if not os.path.isdir(directory):
+                if require_paths_exist:
+                    missing_directories.add(directory)
+                else:
+                    logger.warning(
+                        f"Input path '{directory}' does not exist. Adding to referenced paths."
+                    )
+                    asset_references.referenced_paths.add(directory)
+                continue
+
+            is_dir_empty = True
             for root, _, files in os.walk(directory):
+                if not files:
+                    continue
+                is_dir_empty = False
                 asset_references.input_filenames.update(
                     os.path.normpath(os.path.join(root, file)) for file in files
                 )
+            # Empty directories just become references since there's nothing to upload
+            if is_dir_empty:
+                logger.info(f"Input directory '{directory}' is empty. Adding to referenced paths.")
+                asset_references.referenced_paths.add(directory)
         asset_references.input_directories.clear()
 
+        if missing_directories:
+            all_missing_directories = "\n\t".join(sorted(list(missing_directories)))
+            misconfigured_directories_msg = (
+                "Job submission contains misconfigured input directories and cannot be submitted."
+                " All input directories must exist."
+                f"\nNon-existent directories:\n\t{all_missing_directories}"
+            )
+
+            raise MisconfiguredInputsError(misconfigured_directories_msg)
+
         queue_role_session = api.get_queue_user_boto3_session(
             deadline=deadline,
             config=config,
             farm_id=farm_id,
             queue_id=queue_id,
             queue_display_name=queue["displayName"],
         )
@@ -225,26 +261,22 @@
             farm_id=farm_id,
             queue_id=queue_id,
             job_attachment_settings=JobAttachmentS3Settings(**queue["jobAttachmentSettings"]),
             session=queue_role_session,
         )
 
         upload_group = asset_manager.prepare_paths_for_upload(
-            job_bundle_path=job_bundle_dir,
             input_paths=sorted(asset_references.input_filenames),
             output_paths=sorted(asset_references.output_directories),
             referenced_paths=sorted(asset_references.referenced_paths),
-            storage_profile_id=storage_profile_id,
+            storage_profile=storage_profile,
+            require_paths_exist=require_paths_exist,
         )
         if upload_group.asset_groups:
-            if decide_cancel_submission_callback(
-                upload_group.num_outside_files_by_root,
-                upload_group.total_input_files,
-                upload_group.total_input_bytes,
-            ):
+            if decide_cancel_submission_callback(upload_group):
                 print_function_callback("Job submission canceled.")
                 return None
 
             _, asset_manifests = _hash_attachments(
                 asset_manager=asset_manager,
                 asset_groups=upload_group.asset_groups,
                 total_input_files=upload_group.total_input_files,
```

### Comparing `deadline-0.47.3/src/deadline/client/api/_telemetry.py` & `deadline-0.48.0/src/deadline/client/api/_telemetry.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/cli/_common.py` & `deadline-0.48.0/src/deadline/client/cli/_common.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/cli/_deadline_cli.py` & `deadline-0.48.0/src/deadline/client/cli/_deadline_cli.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/cli/_deadline_web_url.py` & `deadline-0.48.0/src/deadline/client/cli/_deadline_web_url.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/cli/deadline_dev_gui_main.py` & `deadline-0.48.0/src/deadline/client/cli/deadline_dev_gui_main.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/cli/_groups/_sigint_handler.py` & `deadline-0.48.0/src/deadline/client/cli/_groups/_sigint_handler.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/cli/_groups/auth_group.py` & `deadline-0.48.0/src/deadline/client/cli/_groups/auth_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/cli/_groups/bundle_group.py` & `deadline-0.48.0/src/deadline/client/cli/_groups/bundle_group.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,16 +10,20 @@
 
 import click
 from contextlib import ExitStack
 from botocore.exceptions import ClientError
 
 from deadline.client import api
 from deadline.client.config import config_file, get_setting, set_setting
-from deadline.job_attachments.exceptions import AssetSyncError, AssetSyncCancelledError
-from deadline.job_attachments.models import JobAttachmentsFileSystem
+from deadline.job_attachments.exceptions import (
+    AssetSyncError,
+    AssetSyncCancelledError,
+    MisconfiguredInputsError,
+)
+from deadline.job_attachments.models import AssetUploadGroup, JobAttachmentsFileSystem
 from deadline.job_attachments.progress_tracker import ProgressReportMetadata
 from deadline.job_attachments._utils import _human_readable_file_size
 
 from ...exceptions import DeadlineOperationError, CreateJobWaiterCanceled
 from .._common import _apply_cli_options_to_config, _handle_error
 from ._sigint_handler import SigIntHandler
 
@@ -83,68 +87,93 @@
     type=click.Choice([e.value for e in JobAttachmentsFileSystem]),
 )
 @click.option(
     "--yes",
     is_flag=True,
     help="Skip any confirmation prompts",
 )
+@click.option(
+    "--require-paths-exist",
+    is_flag=True,
+    help="Require all input paths to exist",
+)
 @click.argument("job_bundle_dir")
 @_handle_error
 def bundle_submit(
     job_bundle_dir,
     job_attachments_file_system,
     parameter,
     yes,
     name,
     priority,
     max_failed_tasks_count,
     max_retries_per_task,
+    require_paths_exist,
     **args,
 ):
     """
     Submits an Open Job Description job bundle to AWS Deadline Cloud.
     """
     # Get a temporary config object with the standard options handled
     config = _apply_cli_options_to_config(required_options={"farm_id", "queue_id"}, **args)
 
     hash_callback_manager = _ProgressBarCallbackManager(length=100, label="Hashing Attachments")
     upload_callback_manager = _ProgressBarCallbackManager(length=100, label="Uploading Attachments")
 
     def _check_create_job_wait_canceled() -> bool:
         return sigint_handler.continue_operation
 
-    def _decide_cancel_submission(
-        deviated_file_count_by_root: dict[str, int],
-        num_files: int,
-        upload_size: int,
-    ):
+    def _decide_cancel_submission(upload_group: AssetUploadGroup) -> bool:
+        """
+        Callback to decide if submission should be cancelled or not. Return 'True' to cancel.
+        Prints a warning that requires confirmation if paths are found outside of configured storage profile locations.
+        """
+        warning_message = ""
+        for group in upload_group.asset_groups:
+            if not group.file_system_location_name:
+                warning_message += f"\n\nUnder the directory '{group.root_path}':"
+                warning_message += (
+                    f"\n\t{len(group.inputs)} input file{'' if len(group.inputs) == 1 else 's'}"
+                    if len(group.inputs) > 0
+                    else ""
+                )
+                warning_message += (
+                    f"\n\t{len(group.outputs)} output director{'y' if len(group.outputs) == 1 else 'ies'}"
+                    if len(group.outputs) > 0
+                    else ""
+                )
+                warning_message += (
+                    f"\n\t{len(group.references)} referenced file{'' if len(group.references) == 1 else 's'} and/or director{'y' if len(group.outputs) == 1 else 'ies'}"
+                    if len(group.references) > 0
+                    else ""
+                )
+
+        # Exit early if there are no warnings and we've either set auto accept or there's no files to confirm
+        if not warning_message and (
+            yes
+            or config_file.str2bool(get_setting("settings.auto_accept", config=config))
+            or upload_group.total_input_files == 0
+        ):
+            return False
+
         message_text = (
-            f"Job submission contains {num_files} files totaling {_human_readable_file_size(upload_size)}. "
-            " All files will be uploaded to S3 if they are not already present in the job attachments bucket."
+            f"Job submission contains {upload_group.total_input_files} input files totaling {_human_readable_file_size(upload_group.total_input_bytes)}. "
+            " All input files will be uploaded to S3 if they are not already present in the job attachments bucket."
         )
-        if deviated_file_count_by_root:
-            root_by_count_message = "\n\n".join(
-                [
-                    f"{file_count} files from : '{directory}'"
-                    for directory, file_count in deviated_file_count_by_root.items()
-                ]
-            )
+        if warning_message:
             message_text += (
-                f"\n\nFiles were found outside of the configured storage profile location(s). "
-                " Please confirm that you intend to upload files from the following directories:\n\n"
-                f"{root_by_count_message}"
+                f"\n\nFiles were specified outside of the configured storage profile location(s). "
+                " Please confirm that you intend to submit a job that uses files from the following directories:"
+                f"{warning_message}\n\n"
+                "To permanently remove this warning you must only use files located within a storage profile location."
             )
         message_text += "\n\nDo you wish to proceed?"
-        return (
-            not (yes or config_file.str2bool(get_setting("settings.auto_accept", config=config)))
-            and num_files > 0
-            and not click.confirm(
-                message_text,
-                default=not deviated_file_count_by_root,
-            )
+        return not click.confirm(
+            message_text,
+            default=not warning_message,
         )
 
     try:
         job_id = api.create_job_from_job_bundle(
             job_bundle_dir=job_bundle_dir,
             job_parameters=parameter,
             name=name,
@@ -154,14 +183,15 @@
             max_failed_tasks_count=max_failed_tasks_count,
             max_retries_per_task=max_retries_per_task,
             hashing_progress_callback=hash_callback_manager.callback,
             upload_progress_callback=upload_callback_manager.callback,
             create_job_result_callback=_check_create_job_wait_canceled,
             print_function_callback=click.echo,
             decide_cancel_submission_callback=_decide_cancel_submission,
+            require_paths_exist=require_paths_exist,
         )
 
         # Check Whether the CLI options are modifying any of the default settings that affect
         # the job id. If not, we'll save the job id submitted as the default job id.
         # If the submission is canceled by the user job_id will be None, so ignore this case as well.
         if (
             job_id is not None
@@ -187,14 +217,18 @@
         else:
             click.echo("Canceled waiting for final status of CreateJob.")
             return
     except ClientError as exc:
         raise DeadlineOperationError(
             f"Failed to submit the job bundle to AWS Deadline Cloud:\n{exc}"
         ) from exc
+    except MisconfiguredInputsError as exc:
+        click.echo(str(exc))
+        click.echo("Job submission canceled.")
+        return
     except Exception as exc:
         api.get_deadline_cloud_library_telemetry_client().record_error(
             event_details={"exception_scope": "on_submit"},
             exception_type=str(type(exc)),
         )
         raise
```

### Comparing `deadline-0.47.3/src/deadline/client/cli/_groups/config_group.py` & `deadline-0.48.0/src/deadline/client/cli/_groups/config_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/cli/_groups/farm_group.py` & `deadline-0.48.0/src/deadline/client/cli/_groups/farm_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/cli/_groups/fleet_group.py` & `deadline-0.48.0/src/deadline/client/cli/_groups/fleet_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/cli/_groups/handle_web_url_command.py` & `deadline-0.48.0/src/deadline/client/cli/_groups/handle_web_url_command.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/cli/_groups/job_group.py` & `deadline-0.48.0/src/deadline/client/cli/_groups/job_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/cli/_groups/queue_group.py` & `deadline-0.48.0/src/deadline/client/cli/_groups/queue_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/cli/_groups/worker_group.py` & `deadline-0.48.0/src/deadline/client/cli/_groups/worker_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/config/__init__.py` & `deadline-0.48.0/src/deadline/client/config/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/config/config_file.py` & `deadline-0.48.0/src/deadline/client/config/config_file.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/job_bundle/__init__.py` & `deadline-0.48.0/src/deadline/client/job_bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/job_bundle/_yaml.py` & `deadline-0.48.0/src/deadline/client/job_bundle/_yaml.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/job_bundle/adaptors.py` & `deadline-0.48.0/src/deadline/client/job_bundle/adaptors.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/job_bundle/job_template.py` & `deadline-0.48.0/src/deadline/client/job_bundle/job_template.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/job_bundle/loader.py` & `deadline-0.48.0/src/deadline/client/job_bundle/loader.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/job_bundle/parameters.py` & `deadline-0.48.0/src/deadline/client/job_bundle/parameters.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/job_bundle/submission.py` & `deadline-0.48.0/src/deadline/client/job_bundle/submission.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/ui/__init__.py` & `deadline-0.48.0/src/deadline/client/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/ui/cli_job_submitter.py` & `deadline-0.48.0/src/deadline/client/ui/cli_job_submitter.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/ui/deadline_authentication_status.py` & `deadline-0.48.0/src/deadline/client/ui/deadline_authentication_status.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/ui/dev_application.py` & `deadline-0.48.0/src/deadline/client/ui/dev_application.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/ui/job_bundle_submitter.py` & `deadline-0.48.0/src/deadline/client/ui/job_bundle_submitter.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/ui/dataclasses/__init__.py` & `deadline-0.48.0/src/deadline/client/ui/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/ui/dialogs/deadline_config_dialog.py` & `deadline-0.48.0/src/deadline/client/ui/dialogs/deadline_config_dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,15 @@
             label_text="Job Attachments FileSystem Options",
             label_tooltip=job_attachments_file_system_tooltip,
             values_with_tooltips=values_with_tooltips,
         )
 
     def _build_general_settings_ui(self, group, layout):
         self.auto_accept = self._init_checkbox_setting(
-            group, layout, "settings.auto_accept", "Auto Accept Confirmation Prompts"
+            group, layout, "settings.auto_accept", "Auto Accept Prompt Defaults"
         )
         self.telemetry_opt_out = self._init_checkbox_setting(
             group, layout, "telemetry.opt_out", "Telemetry Opt Out"
         )
 
         self._conflict_resolution_options = [option.name for option in FileConflictResolution]
         self.conflict_resolution_box = self._init_combobox_setting(
```

### Comparing `deadline-0.47.3/src/deadline/client/ui/dialogs/deadline_login_dialog.py` & `deadline-0.48.0/src/deadline/client/ui/dialogs/deadline_login_dialog.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/ui/dialogs/submit_job_progress_dialog.py` & `deadline-0.48.0/src/deadline/client/ui/dialogs/submit_job_progress_dialog.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     QApplication,
     QDialog,
     QDialogButtonBox,
     QFormLayout,
     QGroupBox,
     QLabel,
     QMessageBox,
-    QProgressBar,
     QPushButton,
+    QProgressBar,
     QTextEdit,
     QVBoxLayout,
     QWidget,
 )
 
 from deadline.client import api
 from deadline.client.exceptions import (
@@ -48,16 +48,21 @@
     merge_queue_job_parameters,
     read_job_bundle_parameters,
 )
 from deadline.client.job_bundle.submission import (
     AssetReferences,
     split_parameter_args,
 )
-from deadline.job_attachments.exceptions import AssetSyncCancelledError
-from deadline.job_attachments.models import AssetRootGroup, AssetRootManifest
+from deadline.job_attachments.exceptions import AssetSyncCancelledError, MisconfiguredInputsError
+from deadline.job_attachments.models import (
+    AssetRootGroup,
+    AssetRootManifest,
+    AssetUploadGroup,
+    StorageProfile,
+)
 from deadline.job_attachments.progress_tracker import ProgressReportMetadata, SummaryStatistics
 from deadline.job_attachments.upload import S3AssetManager
 from deadline.job_attachments._utils import _human_readable_file_size
 
 __all__ = ["SubmitJobProgressDialog"]
 
 logger = logging.getLogger(__name__)
@@ -96,46 +101,48 @@
 
         self._build_ui()
 
     def start_submission(
         self,
         farm_id: str,
         queue_id: str,
-        storage_profile_id: str,
+        storage_profile: Optional[StorageProfile],
         job_bundle_dir: str,
         queue_parameters: list[JobParameter],
         asset_manager: Optional[S3AssetManager],
         deadline_client: BaseClient,
         auto_accept: bool = False,
+        require_paths_exist: bool = False,
     ) -> Optional[Dict[str, Any]]:
         """
         Starts a submission. Returns the response from calling create job. If an error occurs
         or the submission is canceled then None is returned.
 
         Args:
             farm_id (str): Id of the farm to submit to
             queue_id (str): Id of the queue to submit to
-            storage_profile_id (str): Id of the storage profile to associate
+            storage_profile (StorageProfile): the storage profile to associate
                 with the job.
             job_bundle_dir (str): Path to the folder containing the job bundle to
                 submit.
             asset_manager (S3AssetManager): A job attachments S3AssetManager
                 configured for the farm/queue to submit to
             deadline_client (BaseClient): A boto client for AWS Deadline Cloud
             auto_accept (bool, default False): Flag for whether any confirmation
                 prompts should automatically be accepted.
         """
         self._farm_id = farm_id
         self._queue_id = queue_id
-        self._storage_profile_id = storage_profile_id
+        self._storage_profile = storage_profile
         self._job_bundle_dir = job_bundle_dir
         self._queue_parameters = queue_parameters
         self._asset_manager = asset_manager
         self._deadline_client = deadline_client
         self._auto_accept = auto_accept
+        self._require_paths_exist = require_paths_exist
 
         self._start_submission()
         return self.exec_()
 
     def _build_ui(self):
         """Builds up the Dialog UI"""
         # Remove help button from title bar
@@ -197,16 +204,16 @@
         )
 
         self._create_job_args["farmId"] = self._farm_id
         self._create_job_args["queueId"] = self._queue_id
         self._create_job_args["template"] = file_contents
         self._create_job_args["templateType"] = file_type
 
-        if self._storage_profile_id:
-            self._create_job_args["storageProfileId"] = self._storage_profile_id
+        if self._storage_profile:
+            self._create_job_args["storageProfileId"] = self._storage_profile.storageProfileId
 
         # The job parameters
         job_bundle_parameters = read_job_bundle_parameters(self._job_bundle_dir)
 
         asset_references_obj = read_yaml_or_json_object(
             self._job_bundle_dir, "asset_references", required=False
         )
@@ -236,38 +243,78 @@
 
         if self._asset_manager and (
             self.asset_references.input_filenames
             or self.asset_references.input_directories
             or self.asset_references.output_directories
         ):
             # Extend input_filenames with all the files in the input_directories
+            missing_directories: set[str] = set()
             for directory in self.asset_references.input_directories:
+                if not os.path.isdir(directory):
+                    if self._require_paths_exist:
+                        missing_directories.add(directory)
+                    else:
+                        logging.warning(
+                            f"Input directory '{directory}' does not exist. Adding to referenced paths."
+                        )
+                        self.asset_references.referenced_paths.add(directory)
+                    continue
+
+                is_dir_empty = True
                 for root, _, files in os.walk(directory):
+                    if not files:
+                        continue
+                    is_dir_empty = False
                     self.asset_references.input_filenames.update(
                         os.path.normpath(os.path.join(root, file)) for file in files
                     )
+                # Empty directories just become references since there's nothing to upload
+                if is_dir_empty:
+                    logging.info(
+                        f"Input directory '{directory}' is empty. Adding to referenced paths."
+                    )
+                    self.asset_references.referenced_paths.add(directory)
             self.asset_references.input_directories.clear()
 
+            if missing_directories:
+                sample_size = 3
+                misconfigured_directories_msg = (
+                    "Job submission contains misconfigured input directories and cannot be submitted."
+                    " All input directories must exist."
+                )
+
+                missing_directory_list = sorted(list(missing_directories))
+                sample_of_missing_directories = "\n\t".join(missing_directory_list[:sample_size])
+                sample_of_misconfigured_inputs = (
+                    f"\nNon-existent directories:\n\t{sample_of_missing_directories}\n"
+                )
+                all_missing_directories = "\n\t".join(missing_directory_list)
+                all_misconfigured_inputs = (
+                    f"\nNon-existent directories:\n\t{all_missing_directories}"
+                )
+
+                logging.error(misconfigured_directories_msg + all_misconfigured_inputs)
+                if len(missing_directories) > sample_size:
+                    misconfigured_directories_msg += (
+                        " Check logs for all occurrences, here's a sample:\n"
+                    )
+                misconfigured_directories_msg += f"{sample_of_misconfigured_inputs}"
+
+                raise MisconfiguredInputsError(misconfigured_directories_msg)
+
             upload_group = self._asset_manager.prepare_paths_for_upload(
-                job_bundle_path=self._job_bundle_dir,
                 input_paths=sorted(self.asset_references.input_filenames),
                 output_paths=sorted(self.asset_references.output_directories),
                 referenced_paths=sorted(self.asset_references.referenced_paths),
-                storage_profile_id=self._storage_profile_id,
+                storage_profile=self._storage_profile,
+                require_paths_exist=self._require_paths_exist,
             )
             # If we find any Job Attachments, start a background thread
             if upload_group.asset_groups:
-                if (
-                    not self._auto_accept
-                    and not self._confirm_asset_references_outside_storage_profile(
-                        upload_group.num_outside_files_by_root,
-                        upload_group.total_input_files,
-                        upload_group.total_input_bytes,
-                    )
-                ):
+                if not self._confirm_asset_references_outside_storage_profile(upload_group):
                     raise UserInitiatedCancel("Submission canceled.")
 
                 self._start_hashing(
                     upload_group.asset_groups,
                     upload_group.total_input_files,
                     upload_group.total_input_bytes,
                 )
@@ -540,50 +587,75 @@
         self.button_box.setStandardButtons(QDialogButtonBox.Close)
         self.summary_edit.setText(f"Error Occurred: {str(e)}")
         self.summary_edit.setVisible(True)
         self.adjustSize()
         logger.error(str(e))
 
     def _confirm_asset_references_outside_storage_profile(
-        self,
-        deviated_file_count_by_root: dict[str, int],
-        num_files: int,
-        upload_size: int,
+        self, upload_group: AssetUploadGroup
     ) -> bool:
         """
         Creates a dialog to prompt the user to confirm that they want to proceed
         with uploading when files were found outside of the configured storage profile locations.
         """
-        message_box = QMessageBox(self)
         message_text = (
-            f"Job submission contains {num_files} files totaling {_human_readable_file_size(upload_size)}. "
-            " All files will be uploaded to S3 if they are not already present in the job attachments bucket."
+            f"Job submission contains {upload_group.total_input_files} input files totaling {_human_readable_file_size(upload_group.total_input_bytes)}. "
+            " All input files will be uploaded to S3 if they are not already present in the job attachments bucket."
         )
-        if deviated_file_count_by_root:
-            root_by_count_message = "\n\n".join(
-                [
-                    f"{file_count} files from : '{directory}'"
-                    for directory, file_count in deviated_file_count_by_root.items()
-                ]
-            )
+        warning_message = ""
+        for group in upload_group.asset_groups:
+            if not group.file_system_location_name:
+                warning_message += f"\n\nUnder the directory '{group.root_path}':"
+                warning_message += (
+                    f"\n\t{len(group.inputs)} input file{'' if len(group.inputs) == 1 else 's'}"
+                    if len(group.inputs) > 0
+                    else ""
+                )
+                warning_message += (
+                    f"\n\t{len(group.outputs)} output director{'y' if len(group.outputs) == 1 else 'ies'}"
+                    if len(group.outputs) > 0
+                    else ""
+                )
+                warning_message += (
+                    f"\n\t{len(group.references)} referenced file{'' if len(group.references) == 1 else 's'} and/or director{'y' if len(group.outputs) == 1 else 'ies'}"
+                    if len(group.references) > 0
+                    else ""
+                )
+
+        # Exit early if we've set auto accept and there are no warnings
+        if not warning_message and self._auto_accept:
+            return True
+
+        # Build the UI
+        message_box = QMessageBox(self)
+        if warning_message:
+            if self._storage_profile:
+                fs_locations_text = "\n\t".join(
+                    [fs_location.path for fs_location in self._storage_profile.fileSystemLocations]
+                )
+                message_text += f"\n\nFiles were specified outside of the configured storage profile location(s):\n{fs_locations_text}\n"
+            else:
+                message_text += "\n\nNo storage profile locations are configured for this queue."
             message_text += (
-                f"\n\nFiles were found outside of the configured storage profile location(s). "
-                " Please confirm that you intend to upload files from the following directories:\n\n"
-                f"{root_by_count_message}"
+                "\nPlease confirm that you intend to submit a job that uses files from the following directories:"
+                f"{warning_message}\n\n"
+                "To permanently remove this warning you must only use files located within a storage profile location."
             )
             message_box.setIcon(QMessageBox.Warning)
+
         message_box.setText(message_text)
         message_box.setStandardButtons(QMessageBox.Ok | QMessageBox.Cancel)
         message_box.setDefaultButton(QMessageBox.Ok)
 
-        # Add the "Do not ask again" button that acts like 'OK' but sets the config
-        # setting to always auto-accept similar prompts in the future.
-        dont_ask_button = QPushButton("Do not ask again", self)
-        dont_ask_button.clicked.connect(lambda: set_setting("settings.auto_accept", "true"))
-        message_box.addButton(dont_ask_button, QMessageBox.ActionRole)
+        if not warning_message:
+            # If we don't have any warnings, add the "Do not ask again" button that acts like 'OK' but sets the config
+            # setting to always auto-accept similar prompts in the future.
+            dont_ask_button = QPushButton("Do not ask again", self)
+            dont_ask_button.clicked.connect(lambda: set_setting("settings.auto_accept", "true"))
+            message_box.addButton(dont_ask_button, QMessageBox.ActionRole)
 
         message_box.setWindowTitle("Job Attachments Valid Files Confirmation")
         selection = message_box.exec()
 
         return selection != QMessageBox.Cancel
 
     def closeEvent(self, event: QCloseEvent) -> None:
```

### Comparing `deadline-0.47.3/src/deadline/client/ui/dialogs/submit_job_to_deadline_dialog.py` & `deadline-0.48.0/src/deadline/client/ui/dialogs/submit_job_to_deadline_dialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,14 +428,20 @@
                     purpose=JobBundlePurpose.SUBMISSION,
                 )
 
             farm_id = get_setting("defaults.farm_id")
             queue_id = get_setting("defaults.queue_id")
             storage_profile_id = get_setting("settings.storage_profile_id")
 
+            storage_profile = None
+            if storage_profile_id:
+                storage_profile = api.get_storage_profile_for_queue(
+                    farm_id, queue_id, storage_profile_id, deadline
+                )
+
             queue = deadline.get_queue(farmId=farm_id, queueId=queue_id)
 
             queue_role_session = api.get_queue_user_boto3_session(
                 deadline=deadline,
                 farm_id=farm_id,
                 queue_id=queue_id,
                 queue_display_name=queue["displayName"],
@@ -459,20 +465,21 @@
                 },
                 from_gui=True,
             )
 
             self.create_job_response = job_progress_dialog.start_submission(
                 farm_id,
                 queue_id,
-                storage_profile_id,
+                storage_profile,
                 job_history_bundle_dir,
                 queue_parameters,
                 asset_manager,
                 deadline,
                 auto_accept=str2bool(get_setting("settings.auto_accept")),
+                require_paths_exist=self.job_attachments.get_require_paths_exist(),
             )
         except UserInitiatedCancel as uic:
             logger.info("Canceling submission.")
             QMessageBox.information(self, f"{settings.submitter_name} Job Submission", str(uic))
             job_progress_dialog.close()
         except Exception as exc:
             logger.exception("error submitting job")
```

### Comparing `deadline-0.47.3/src/deadline/client/ui/resources/deadline_logo.svg` & `deadline-0.48.0/src/deadline/client/ui/resources/deadline_logo.svg`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/ui/resources/blender_example_bundle/template.yaml` & `deadline-0.48.0/src/deadline/client/ui/resources/blender_example_bundle/template.yaml`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/ui/resources/cli_job_bundle/template.yaml` & `deadline-0.48.0/src/deadline/client/ui/resources/cli_job_bundle/template.yaml`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/ui/resources/controls_demo_job_bundle/template.yaml` & `deadline-0.48.0/src/deadline/client/ui/resources/controls_demo_job_bundle/template.yaml`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/ui/widgets/cli_job_settings_tab.py` & `deadline-0.48.0/src/deadline/client/ui/widgets/cli_job_settings_tab.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/ui/widgets/deadline_authentication_status_widget.py` & `deadline-0.48.0/src/deadline/client/ui/widgets/deadline_authentication_status_widget.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/ui/widgets/host_requirements_tab.py` & `deadline-0.48.0/src/deadline/client/ui/widgets/host_requirements_tab.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/ui/widgets/job_attachments_tab.py` & `deadline-0.48.0/src/deadline/client/ui/widgets/job_attachments_tab.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,19 +54,27 @@
 
         self._build_ui()
         self._populate_attachment_lists()
 
     def _build_ui(self) -> None:
         tab_layout = QVBoxLayout(self)
 
+        # Create a group box for general settings
+        size_policy = QSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
+        size_policy.setVerticalStretch(10)
+        self.general_group = QGroupBox("General Submission Settings", self)
+        tab_layout.addWidget(self.general_group)
+        self.general_group.setSizePolicy(size_policy)
+        general_layout = QVBoxLayout(self.general_group)
+
         # Create a group box for each type of attachment
         self.input_files_group = QGroupBox("Attach Input Files", self)
-        tab_layout.addWidget(self.input_files_group)
         size_policy = QSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
         size_policy.setVerticalStretch(80)
+        tab_layout.addWidget(self.input_files_group)
         self.input_files_group.setSizePolicy(size_policy)
         input_files_layout = QVBoxLayout(self.input_files_group)
 
         self.input_directories_group = QGroupBox("Attach Input Directories", self)
         size_policy = QSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
         size_policy.setVerticalStretch(10)
         self.input_directories_group.setSizePolicy(size_policy)
@@ -76,14 +84,18 @@
         self.output_directories_group = QGroupBox("Specify Output Directories", self)
         size_policy = QSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
         size_policy.setVerticalStretch(10)
         self.output_directories_group.setSizePolicy(size_policy)
         tab_layout.addWidget(self.output_directories_group)
         output_directories_layout = QVBoxLayout(self.output_directories_group)
 
+        # General settings
+        self.general_settings = JobAttachmentsGeneralWidget(self)
+        general_layout.addWidget(self.general_settings)
+
         # The "Attach Input Files" attachments
         self.input_files_controls = JobAttachmentsControlsWidget(self)
         self.input_files_controls.show_auto_detected.stateChanged.connect(
             self.show_auto_detected_change
         )
         self.input_files_controls.add.clicked.connect(self._add_input_files)
         self.input_files_controls.remove_selected.clicked.connect(self._remove_selected_input_files)
@@ -304,14 +316,35 @@
     def get_asset_references(self) -> AssetReferences:
         """
         Creates an asset_references object that can be saved as the
         asset_references.json|yaml file in a Job Bundle.
         """
         return self.auto_detected_attachments.union(self.attachments)
 
+    def get_require_paths_exist(self) -> bool:
+        """
+        Returns the checkbox value of whether to allow empty paths or not.
+        """
+        return self.general_settings.require_paths_exist.isChecked()
+
+
+class JobAttachmentsGeneralWidget(QWidget):
+    """
+    A Widget that contains general settings for a specific submission.
+    """
+
+    def __init__(self, parent=None) -> None:
+        super().__init__(parent=parent)
+
+        layout = QHBoxLayout(self)
+        layout.setContentsMargins(0, 0, 0, 0)
+
+        self.require_paths_exist = QCheckBox("Require all input paths exist", parent=self)
+        layout.addWidget(self.require_paths_exist)
+
 
 class JobAttachmentsControlsWidget(QWidget):
     """
     A Widget that contains buttons for the actions to add/remove files or directories
     in a job attachments list.
     """
```

### Comparing `deadline-0.47.3/src/deadline/client/ui/widgets/job_bundle_settings_tab.py` & `deadline-0.48.0/src/deadline/client/ui/widgets/job_bundle_settings_tab.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/ui/widgets/openjd_parameters_widget.py` & `deadline-0.48.0/src/deadline/client/ui/widgets/openjd_parameters_widget.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/ui/widgets/path_widgets.py` & `deadline-0.48.0/src/deadline/client/ui/widgets/path_widgets.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/ui/widgets/shared_job_settings_tab.py` & `deadline-0.48.0/src/deadline/client/ui/widgets/shared_job_settings_tab.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/client/ui/widgets/spinbox_widgets.py` & `deadline-0.48.0/src/deadline/client/ui/widgets/spinbox_widgets.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/job_attachments/README.md` & `deadline-0.48.0/src/deadline/job_attachments/README.md`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/job_attachments/_utils.py` & `deadline-0.48.0/src/deadline/job_attachments/_utils.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/job_attachments/asset_sync.py` & `deadline-0.48.0/src/deadline/job_attachments/asset_sync.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/job_attachments/download.py` & `deadline-0.48.0/src/deadline/job_attachments/download.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/job_attachments/exceptions.py` & `deadline-0.48.0/src/deadline/job_attachments/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,21 @@
 
 class AssetOutsideOfRootError(JobAttachmentsError):
     """
     Exception for errors related to assets being outside of the asset root.
     """
 
 
+class MisconfiguredInputsError(JobAttachmentsError):
+    """
+    Exception for errors related to missing input directories, empty input directories,
+    missing input files, and input directories classified as files
+    """
+
+
 class ManifestDecodeValidationError(JobAttachmentsError):
     """
     Exception for errors related to asset manifest decoding.
     """
 
 
 class MissingManifestError(JobAttachmentsError):
```

### Comparing `deadline-0.47.3/src/deadline/job_attachments/models.py` & `deadline-0.48.0/src/deadline/job_attachments/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 
 
 @dataclass
 class AssetUploadGroup:
     """Represents all of the information needed to prepare to upload assets"""
 
     asset_groups: List[AssetRootGroup] = field(default_factory=list)
-    num_outside_files_by_root: dict[str, int] = field(default_factory=dict)
     total_input_files: int = 0
     total_input_bytes: int = 0
 
 
 @dataclass
 class ManifestPathGroup:
     """
```

### Comparing `deadline-0.47.3/src/deadline/job_attachments/os_file_permission.py` & `deadline-0.48.0/src/deadline/job_attachments/os_file_permission.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/job_attachments/progress_tracker.py` & `deadline-0.48.0/src/deadline/job_attachments/progress_tracker.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/job_attachments/upload.py` & `deadline-0.48.0/src/deadline/job_attachments/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,34 +36,35 @@
 )
 from ._aws.aws_clients import (
     get_account_id,
     get_boto3_session,
     get_s3_client,
     get_s3_transfer_manager,
 )
-from ._aws.deadline import get_storage_profile_for_queue
 from .exceptions import (
     COMMON_ERROR_GUIDANCE_FOR_S3,
     AssetSyncCancelledError,
     AssetSyncError,
     JobAttachmentS3BotoCoreError,
     JobAttachmentsS3ClientError,
+    MisconfiguredInputsError,
     MissingS3BucketError,
     MissingS3RootPrefixError,
 )
 from .caches import HashCache, HashCacheEntry, S3CheckCache, S3CheckCacheEntry
 from .models import (
     AssetRootGroup,
     AssetRootManifest,
     AssetUploadGroup,
     Attachments,
     FileSystemLocationType,
     JobAttachmentS3Settings,
     ManifestProperties,
     PathFormat,
+    StorageProfile,
 )
 from .progress_tracker import (
     ProgressStatus,
     ProgressTracker,
     SummaryStatistics,
 )
 from ._utils import (
@@ -819,14 +820,15 @@
     def _get_asset_groups(
         self,
         input_paths: set[str],
         output_paths: set[str],
         referenced_paths: set[str],
         local_type_locations: dict[str, str] = {},
         shared_type_locations: dict[str, str] = {},
+        require_paths_exist: bool = False,
     ) -> list[AssetRootGroup]:
         """
         For the given input paths and output paths, a list of groups is returned, where paths sharing
         the same root path are grouped together. Note that paths can be files or directories.
 
         The returned list satisfies the following conditions:
         - If a path is relative to any of the paths in the given `shared_type_locations` paths, it is
@@ -834,25 +836,32 @@
         - The given `local_type_locations` paths can each form a group based on its root path. In other
           words, if there are paths relative to any of the `local_type_locations` paths, they are grouped
           together as one.
         - The referenced paths may have no files or directories associated, but they always live
           relative to one of the AssetRootGroup objects returned.
         """
         groupings: dict[str, AssetRootGroup] = {}
+        missing_input_paths = set()
+        misconfigured_directories = set()
 
         # Resolve full path, then cast to pure path to get top-level directory
-        # Note for inputs, we only upload individual files so user doesn't unintentionally upload the entire hard drive
         for _path in input_paths:
             # Need to use absolute to not resolve symlinks, but need normpath to get rid of relative paths, i.e. '..'
             abs_path = Path(os.path.normpath(Path(_path).absolute()))
             if not abs_path.exists():
-                logger.warning(f"Skipping uploading input as it doesn't exist: {abs_path}")
+                if require_paths_exist:
+                    missing_input_paths.add(abs_path)
+                else:
+                    logger.warning(
+                        f"Input path '{_path}' resolving to '{abs_path}' does not exist. Adding to referenced paths."
+                    )
+                    referenced_paths.add(_path)
                 continue
             if abs_path.is_dir():
-                logger.warning(f"Skipping uploading input as it is a directory: {abs_path}")
+                misconfigured_directories.add(abs_path)
                 continue
 
             # Skips the upload if the path is relative to any of the File System Location
             # of SHARED type that was set in the Job.
             if any(_is_relative_to(abs_path, shared) for shared in shared_type_locations):
                 continue
 
@@ -862,14 +871,34 @@
                 groupings=groupings,
                 abs_path=abs_path,
                 local_type_locations=local_type_locations,
             )
             matched_group = self._get_matched_group(matched_root, groupings)
             matched_group.inputs.add(abs_path)
 
+        if missing_input_paths or misconfigured_directories:
+            all_misconfigured_inputs = ""
+            misconfigured_inputs_msg = (
+                "Job submission contains missing input files or directories specified as files."
+                " All inputs must exist and be classified properly."
+            )
+            if missing_input_paths:
+                missing_inputs_list: list[str] = sorted([str(i) for i in missing_input_paths])
+                all_missing_inputs = "\n\t".join(missing_inputs_list)
+                all_misconfigured_inputs += f"\nMissing input files:\n\t{all_missing_inputs}"
+            if misconfigured_directories:
+                misconfigured_directories_list: list[str] = sorted(
+                    [str(d) for d in misconfigured_directories]
+                )
+                all_misconfigured_directories = "\n\t".join(misconfigured_directories_list)
+                all_misconfigured_inputs += (
+                    f"\nDirectories classified as files:\n\t{all_misconfigured_directories}"
+                )
+            raise MisconfiguredInputsError(misconfigured_inputs_msg + all_misconfigured_inputs)
+
         for _path in output_paths:
             abs_path = Path(os.path.normpath(Path(_path).absolute()))
 
             # Skips the upload if the path is relative to any of the File System Location
             # of SHARED type that was set in the Job.
             if any(_is_relative_to(abs_path, shared) for shared in shared_type_locations):
                 continue
@@ -1000,108 +1029,84 @@
             input_paths = [str(input) for input in group.inputs]
             total_bytes += self._get_total_size_of_files(input_paths)
             total_files += len(input_paths)
         return (total_files, total_bytes)
 
     def _get_file_system_locations_by_type(
         self,
-        storage_profile_id: str,
-        session: Optional[boto3.Session] = None,
+        storage_profile_for_queue: StorageProfile,
     ) -> Tuple[dict, dict]:
         """
-        Given the Storage Profile ID, fetches Storage Profile for Queue object, and
-        extracts and groups path and name pairs from the File System Locations into
-        two dicts - LOCAL and SHARED type, respectively. Returns a tuple of two dicts.
-        """
-        storage_profile_for_queue = get_storage_profile_for_queue(
-            farm_id=self.farm_id,
-            queue_id=self.queue_id,
-            storage_profile_id=storage_profile_id,
-            session=session,
-        )
-
+        Given the Storage Profile for Queue object, extracts and groups
+        path and name pairs from the File System Locations into two dicts,
+        LOCAL and SHARED type, respectively. Returns a tuple of two dicts.
+        """
         local_type_locations: dict[str, str] = {}
         shared_type_locations: dict[str, str] = {}
         for fs_loc in storage_profile_for_queue.fileSystemLocations:
             if fs_loc.type == FileSystemLocationType.LOCAL:
                 local_type_locations[fs_loc.path] = fs_loc.name
             elif fs_loc.type == FileSystemLocationType.SHARED:
                 shared_type_locations[fs_loc.path] = fs_loc.name
         return local_type_locations, shared_type_locations
 
-    def _get_deviated_file_count_by_root(
-        self, groups: list[AssetRootGroup], root_path: str
-    ) -> dict[str, int]:
-        """
-        Given a list of AssetRootGroups and a root directory, return a dict of root paths and file counts that
-        are outside of that root path, and aren't in any storage profile locations.
-        """
-        real_root_path = Path(root_path).resolve()
-        deviated_file_count_by_root: dict[str, int] = {}
-        for group in groups:
-            if (
-                not str(Path(group.root_path).resolve()).startswith(str(real_root_path))
-                and not group.file_system_location_name
-                and group.inputs
-            ):
-                deviated_file_count_by_root[group.root_path] = len(group.inputs)
-        return deviated_file_count_by_root
-
     def _group_asset_paths(
         self,
         input_paths: list[str],
         output_paths: list[str],
         referenced_paths: list[str],
-        storage_profile_id: Optional[str] = None,
+        storage_profile: Optional[StorageProfile] = None,
+        require_paths_exist: bool = False,
     ) -> list[AssetRootGroup]:
         """
         Resolves all of the paths that will be uploaded, sorting by storage profile location.
         """
         local_type_locations: dict[str, str] = {}
         shared_type_locations: dict[str, str] = {}
-        if storage_profile_id:
+        if storage_profile:
             (
                 local_type_locations,
                 shared_type_locations,
-            ) = self._get_file_system_locations_by_type(storage_profile_id)
+            ) = self._get_file_system_locations_by_type(storage_profile)
 
         # Group the paths by asset root, removing duplicates and empty strings
         asset_groups: list[AssetRootGroup] = self._get_asset_groups(
             {ip_path for ip_path in input_paths if ip_path},
             {op_path for op_path in output_paths if op_path},
             {rf_path for rf_path in referenced_paths if rf_path},
             local_type_locations,
             shared_type_locations,
+            require_paths_exist,
         )
 
         return asset_groups
 
     def prepare_paths_for_upload(
         self,
-        job_bundle_path: str,
         input_paths: list[str],
         output_paths: list[str],
         referenced_paths: list[str],
-        storage_profile_id: Optional[str] = None,
+        storage_profile: Optional[StorageProfile] = None,
+        require_paths_exist: bool = False,
     ) -> AssetUploadGroup:
         """
         Processes all of the paths required for upload, grouping them by asset root and local storage profile locations.
         Returns an object containing the grouped paths, which also includes a dictionary of input directories and file counts
         for files that were not under the root path or any local storage profile locations.
         """
         asset_groups = self._group_asset_paths(
-            input_paths, output_paths, referenced_paths, storage_profile_id
+            input_paths,
+            output_paths,
+            referenced_paths,
+            storage_profile,
+            require_paths_exist,
         )
         (input_file_count, input_bytes) = self._get_total_input_size_from_asset_group(asset_groups)
-        num_outside_files_by_bundle_path = self._get_deviated_file_count_by_root(
-            asset_groups, job_bundle_path
-        )
         return AssetUploadGroup(
             asset_groups=asset_groups,
-            num_outside_files_by_root=num_outside_files_by_bundle_path,
             total_input_files=input_file_count,
             total_input_bytes=input_bytes,
         )
 
     def hash_assets_and_create_manifest(
         self,
         asset_groups: list[AssetRootGroup],
```

### Comparing `deadline-0.47.3/src/deadline/job_attachments/vfs.py` & `deadline-0.48.0/src/deadline/job_attachments/vfs.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/job_attachments/_aws/aws_clients.py` & `deadline-0.48.0/src/deadline/job_attachments/_aws/aws_clients.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/job_attachments/_aws/deadline.py` & `deadline-0.48.0/src/deadline/job_attachments/_aws/deadline.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,23 +6,19 @@
 import boto3
 from botocore.exceptions import ClientError
 
 from ..exceptions import JobAttachmentsError
 from ..models import (
     Attachments,
     JobAttachmentsFileSystem,
-    FileSystemLocation,
-    FileSystemLocationType,
     Job,
     JobAttachmentS3Settings,
     ManifestProperties,
-    StorageProfileOperatingSystemFamily,
     PathFormat,
     Queue,
-    StorageProfile,
 )
 from .aws_clients import get_deadline_client
 
 
 def get_queue(
     farm_id: str,
     queue_id: str,
@@ -106,42 +102,7 @@
                     response["attachments"].get("fileSystem", JobAttachmentsFileSystem.COPIED.value)
                 ),
             )
             if "attachments" in response and response["attachments"]
             else None
         ),
     )
-
-
-def get_storage_profile_for_queue(
-    farm_id: str,
-    queue_id: str,
-    storage_profile_id: str,
-    session: Optional[boto3.Session] = None,
-    deadline_endpoint_url: Optional[str] = None,
-) -> StorageProfile:
-    """
-    Retrieves a specific storage profile for queue from AWS Deadline Cloud.
-    """
-    try:
-        response = get_deadline_client(
-            session=session, endpoint_url=deadline_endpoint_url
-        ).get_storage_profile_for_queue(
-            farmId=farm_id, queueId=queue_id, storageProfileId=storage_profile_id
-        )
-    except ClientError as exc:
-        raise JobAttachmentsError(
-            f'Failed to get Storage profile "{storage_profile_id}" from Deadline'
-        ) from exc
-    return StorageProfile(
-        storageProfileId=response["storageProfileId"],
-        displayName=response["displayName"],
-        osFamily=StorageProfileOperatingSystemFamily(response["osFamily"]),
-        fileSystemLocations=[
-            FileSystemLocation(
-                name=file_system_location["name"],
-                path=file_system_location["path"],
-                type=FileSystemLocationType(file_system_location["type"]),
-            )
-            for file_system_location in response.get("fileSystemLocations", [])
-        ],
-    )
```

### Comparing `deadline-0.47.3/src/deadline/job_attachments/_windows/file.py` & `deadline-0.48.0/src/deadline/job_attachments/_windows/file.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/job_attachments/asset_manifests/__init__.py` & `deadline-0.48.0/src/deadline/job_attachments/asset_manifests/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/job_attachments/asset_manifests/_canonical_json.py` & `deadline-0.48.0/src/deadline/job_attachments/asset_manifests/_canonical_json.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/job_attachments/asset_manifests/base_manifest.py` & `deadline-0.48.0/src/deadline/job_attachments/asset_manifests/base_manifest.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/job_attachments/asset_manifests/decode.py` & `deadline-0.48.0/src/deadline/job_attachments/asset_manifests/decode.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/job_attachments/asset_manifests/hash_algorithms.py` & `deadline-0.48.0/src/deadline/job_attachments/asset_manifests/hash_algorithms.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/job_attachments/asset_manifests/manifest_model.py` & `deadline-0.48.0/src/deadline/job_attachments/asset_manifests/manifest_model.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/job_attachments/asset_manifests/schemas/2023-03-03.json` & `deadline-0.48.0/src/deadline/job_attachments/asset_manifests/schemas/2023-03-03.json`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/job_attachments/asset_manifests/v2023_03_03/asset_manifest.py` & `deadline-0.48.0/src/deadline/job_attachments/asset_manifests/v2023_03_03/asset_manifest.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/job_attachments/caches/cache_db.py` & `deadline-0.48.0/src/deadline/job_attachments/caches/cache_db.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/job_attachments/caches/hash_cache.py` & `deadline-0.48.0/src/deadline/job_attachments/caches/hash_cache.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/src/deadline/job_attachments/caches/s3_check_cache.py` & `deadline-0.48.0/src/deadline/job_attachments/caches/s3_check_cache.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/LICENSE` & `deadline-0.48.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/README.md` & `deadline-0.48.0/README.md`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/hatch.toml` & `deadline-0.48.0/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline-0.47.3/pyproject.toml` & `deadline-0.48.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 # Applications that consume this library should be the ones that are more strictly
 # limiting dependencies if they want/need to.
 dependencies = [
     "boto3 >= 1.34.75",
     "click >= 8.1.7",
     "pyyaml >= 6.0",
     # Job Attachments
-    "typing_extensions == 4.7.*; python_version == '3.7'",
+    "typing_extensions >= 4.7,< 4.12; python_version == '3.7'",
     "typing_extensions >= 4.8; python_version > '3.7'",
     # Pinning due to 3.4 not being available upstream
     "xxhash == 3.4.*",
     # Pinning due to new 4.18 dependencies breaking pyinstaller implementation
     "jsonschema == 4.17.*",
     "pywin32 == 306; sys_platform == 'win32'",
     "QtPy == 2.4.*",
```

### Comparing `deadline-0.47.3/PKG-INFO` & `deadline-0.48.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline
-Version: 0.47.3
+Version: 0.48.0
 Summary: Multi-purpose library and command line tool that implements functionality to support applications using AWS Deadline Cloud.
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud
 Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
@@ -26,15 +26,15 @@
 Requires-Python: >=3.8
 Requires-Dist: boto3>=1.34.75
 Requires-Dist: click>=8.1.7
 Requires-Dist: jsonschema==4.17.*
 Requires-Dist: pywin32==306; sys_platform == 'win32'
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: qtpy==2.4.*
-Requires-Dist: typing-extensions==4.7.*; python_version == '3.7'
+Requires-Dist: typing-extensions<4.12,>=4.7; python_version == '3.7'
 Requires-Dist: typing-extensions>=4.8; python_version > '3.7'
 Requires-Dist: xxhash==3.4.*
 Provides-Extra: gui
 Requires-Dist: pyside6-essentials==6.6.*; extra == 'gui'
 Description-Content-Type: text/markdown
 
 # AWS Deadline Cloud client
```

