# Comparing `tmp/ansible-risk-insight-0.2.4.tar.gz` & `tmp/ansible-risk-insight-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-risk-insight-0.2.4.tar", last modified: Thu Nov 16 01:44:53 2023, max compression
+gzip compressed data, was "ansible-risk-insight-0.2.5.tar", last modified: Thu Apr 25 12:40:09 2024, max compression
```

## Comparing `ansible-risk-insight-0.2.4.tar` & `ansible-risk-insight-0.2.5.tar`

### file list

```diff
@@ -1,219 +1,218 @@
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.792591 ansible-risk-insight-0.2.4/
--rw-r--r--   0 hiro       (501) staff       (20)       46 2022-12-14 05:36:09.000000 ansible-risk-insight-0.2.4/.flake8
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.725170 ansible-risk-insight-0.2.4/.github/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.731070 ansible-risk-insight-0.2.4/.github/workflows/
--rw-r--r--   0 hiro       (501) staff       (20)      832 2022-12-16 00:52:20.000000 ansible-risk-insight-0.2.4/.github/workflows/lint.yml
--rw-r--r--   0 hiro       (501) staff       (20)      793 2023-08-22 04:18:04.000000 ansible-risk-insight-0.2.4/.github/workflows/test.yml
--rw-r--r--   0 hiro       (501) staff       (20)     1799 2023-03-23 07:29:42.000000 ansible-risk-insight-0.2.4/.gitignore
--rw-r--r--   0 hiro       (501) staff       (20)      436 2022-12-16 00:52:20.000000 ansible-risk-insight-0.2.4/.pre-commit-config.yaml
--rw-r--r--   0 hiro       (501) staff       (20)      990 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.4/CONTRIBUTING.md
--rw-r--r--   0 hiro       (501) staff       (20)    11357 2022-12-14 05:36:09.000000 ansible-risk-insight-0.2.4/LICENSE
--rw-r--r--   0 hiro       (501) staff       (20)      456 2022-12-16 00:52:20.000000 ansible-risk-insight-0.2.4/Makefile
--rw-r--r--   0 hiro       (501) staff       (20)      272 2023-11-16 01:44:53.792435 ansible-risk-insight-0.2.4/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     4510 2023-02-27 07:18:31.000000 ansible-risk-insight-0.2.4/README.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.744576 ansible-risk-insight-0.2.4/ansible_risk_insight/
--rw-r--r--   0 hiro       (501) staff       (20)     1907 2023-05-19 01:44:19.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)      659 2023-11-16 01:40:50.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/_version.py
--rw-r--r--   0 hiro       (501) staff       (20)     3519 2023-04-04 07:22:15.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/analyzer.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.748298 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/
--rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     1408 2023-01-31 05:05:07.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/annotator_base.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.756443 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/
--rw-r--r--   0 hiro       (501) staff       (20)     1393 2023-02-01 01:54:20.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/apt.py
--rw-r--r--   0 hiro       (501) staff       (20)     1587 2023-05-19 01:44:14.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/apt_key.py
--rw-r--r--   0 hiro       (501) staff       (20)     1446 2023-05-19 01:44:14.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/assemble.py
--rw-r--r--   0 hiro       (501) staff       (20)     1460 2023-05-19 01:44:14.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py
--rw-r--r--   0 hiro       (501) staff       (20)     1388 2023-01-31 05:05:07.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/command.py
--rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-05-19 01:44:14.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/dnf.py
--rw-r--r--   0 hiro       (501) staff       (20)     1447 2023-02-01 01:54:20.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/expect.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-05-19 01:44:14.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/file.py
--rw-r--r--   0 hiro       (501) staff       (20)     1320 2023-01-31 05:05:07.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/get_url.py
--rw-r--r--   0 hiro       (501) staff       (20)     1317 2023-02-01 01:54:20.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/git.py
--rw-r--r--   0 hiro       (501) staff       (20)     1511 2023-05-19 01:44:14.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py
--rw-r--r--   0 hiro       (501) staff       (20)     1339 2023-02-01 01:54:20.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/pip.py
--rw-r--r--   0 hiro       (501) staff       (20)     1380 2023-02-01 01:54:20.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/raw.py
--rw-r--r--   0 hiro       (501) staff       (20)     1448 2023-05-19 01:44:14.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/replace.py
--rw-r--r--   0 hiro       (501) staff       (20)     1371 2023-05-19 01:44:14.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py
--rw-r--r--   0 hiro       (501) staff       (20)     1386 2023-02-01 01:54:20.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/script.py
--rw-r--r--   0 hiro       (501) staff       (20)     1384 2023-02-01 01:54:20.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/shell.py
--rw-r--r--   0 hiro       (501) staff       (20)     1327 2023-02-01 01:54:20.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/subversion.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-05-19 01:44:14.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/template.py
--rw-r--r--   0 hiro       (501) staff       (20)     2221 2023-05-19 01:44:14.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/unarchive.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-02-09 05:39:40.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/uri.py
--rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-05-19 01:44:14.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/yum.py
--rw-r--r--   0 hiro       (501) staff       (20)     1230 2023-01-31 05:05:07.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible_builtin.py
--rw-r--r--   0 hiro       (501) staff       (20)    46432 2023-01-31 05:05:07.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible_builtin.py.bak
--rw-r--r--   0 hiro       (501) staff       (20)     1113 2023-01-31 05:05:07.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/module_annotator_base.py
--rw-r--r--   0 hiro       (501) staff       (20)     2846 2023-03-23 08:17:01.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/risk_annotator_base.py
--rw-r--r--   0 hiro       (501) staff       (20)     2381 2023-01-31 05:05:07.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/sample_custom_annotator.py
--rw-r--r--   0 hiro       (501) staff       (20)     9222 2023-08-29 01:53:12.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/variable_resolver.py
--rw-r--r--   0 hiro       (501) staff       (20)   846979 2023-04-26 08:32:29.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/ansible_builtin_modules.json
--rw-r--r--   0 hiro       (501) staff       (20)     2306 2022-12-14 05:36:09.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/ansible_variables.txt
--rw-r--r--   0 hiro       (501) staff       (20)     3211 2023-08-30 00:43:57.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/awx_utils.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      678 2022-12-14 05:36:09.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/batch.sh
--rw-r--r--   0 hiro       (501) staff       (20)     1049 2022-12-14 05:36:09.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/builtin-modules.txt
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.756659 ansible-risk-insight-0.2.4/ansible_risk_insight/cli/
--rw-r--r--   0 hiro       (501) staff       (20)     7429 2023-04-13 09:29:16.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/cli/__init__.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.759547 ansible-risk-insight-0.2.4/ansible_risk_insight/cli/ram/
--rw-r--r--   0 hiro       (501) staff       (20)     2032 2023-09-26 03:55:49.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/cli/ram/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     1705 2022-12-14 05:36:09.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/cli/ram/diff.py
--rw-r--r--   0 hiro       (501) staff       (20)     3085 2023-04-04 07:22:15.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/cli/ram/generate.py
--rw-r--r--   0 hiro       (501) staff       (20)     1486 2022-12-14 05:36:09.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/cli/ram/list.py
--rw-r--r--   0 hiro       (501) staff       (20)     1690 2023-03-23 08:17:01.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/cli/ram/release.py
--rw-r--r--   0 hiro       (501) staff       (20)     1720 2023-01-06 06:26:43.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/cli/ram/search.py
--rw-r--r--   0 hiro       (501) staff       (20)     2033 2023-01-31 05:05:07.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/cli/ram/update.py
--rw-r--r--   0 hiro       (501) staff       (20)    31923 2023-08-29 05:51:56.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/context.py
--rw-r--r--   0 hiro       (501) staff       (20)    48633 2023-10-23 00:30:52.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/dependency_dir_preparator.py
--rw-r--r--   0 hiro       (501) staff       (20)    14850 2023-10-10 01:15:17.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/dependency_finder.py
--rw-r--r--   0 hiro       (501) staff       (20)    19877 2023-11-09 06:35:46.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/finder.py
--rw-r--r--   0 hiro       (501) staff       (20)     2683 2023-08-01 01:36:12.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/findings.py
--rw-r--r--   0 hiro       (501) staff       (20)     1291 2022-12-14 05:36:09.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/key_test.py
--rw-r--r--   0 hiro       (501) staff       (20)     8582 2023-10-26 05:03:05.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/keyutil.py
--rw-r--r--   0 hiro       (501) staff       (20)     8683 2023-04-13 09:29:16.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/loader.py
--rw-r--r--   0 hiro       (501) staff       (20)     1615 2023-02-13 09:30:01.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/logger.py
--rw-r--r--   0 hiro       (501) staff       (20)    71834 2023-11-08 02:26:14.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/model_loader.py
--rw-r--r--   0 hiro       (501) staff       (20)    82385 2023-11-07 08:35:00.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/models.py
--rw-r--r--   0 hiro       (501) staff       (20)    26942 2023-10-26 05:03:05.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/parser.py
--rw-r--r--   0 hiro       (501) staff       (20)     5955 2023-05-19 01:44:28.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/ram_generator.py
--rw-r--r--   0 hiro       (501) staff       (20)      105 2023-10-26 05:03:13.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/requirements.txt
--rw-r--r--   0 hiro       (501) staff       (20)    45040 2023-11-14 01:12:31.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/risk_assessment_model.py
--rw-r--r--   0 hiro       (501) staff       (20)     8376 2023-08-01 01:36:12.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/risk_detector.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.775485 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/
--rw-r--r--   0 hiro       (501) staff       (20)     4076 2023-10-16 02:04:57.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/P001_module_name_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     6677 2023-10-30 09:29:08.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/P002_module_argument_key_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     7106 2023-10-30 09:29:08.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/P003_module_argument_value_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     3418 2023-10-23 00:30:52.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/P004_variable_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R101_command_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)     1801 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R101_command_exec.py
--rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R102_command_instead_of_shell.md
--rw-r--r--   0 hiro       (501) staff       (20)     1684 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R102_command_instead_of_shell.py
--rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R103_download_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)     2703 2023-03-30 11:42:56.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R103_download_exec.py
--rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R104_unauthorized_download_src.md
--rw-r--r--   0 hiro       (501) staff       (20)     2370 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R104_unauthorized_download_src.py
--rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R105_outbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)     1846 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R105_outbound_transfer.py
--rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R106_inbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)     1947 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R106_inbound_transfer.py
--rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md
--rw-r--r--   0 hiro       (501) staff       (20)     2066 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py
--rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R108_privilege_escalation.md
--rw-r--r--   0 hiro       (501) staff       (20)     1536 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R108_privilege_escalation.py
--rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R109_key_config_change.md
--rw-r--r--   0 hiro       (501) staff       (20)     1756 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R109_key_config_change.py
--rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R110_non_builtin_use.md
--rw-r--r--   0 hiro       (501) staff       (20)     1642 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R110_non_builtin_use.py
--rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R111_parameterized_import_role.md
--rw-r--r--   0 hiro       (501) staff       (20)     1729 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R111_parameterized_import_role.py
--rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R112_parameterized_import_taskfile.md
--rw-r--r--   0 hiro       (501) staff       (20)     1952 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py
--rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R113_parameterized_pkg_install.md
--rw-r--r--   0 hiro       (501) staff       (20)     1875 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R113_parameterized_pkg_install.py
--rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R114_file_change.md
--rw-r--r--   0 hiro       (501) staff       (20)     2088 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R114_file_change.py
--rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R115_file_deletion.md
--rw-r--r--   0 hiro       (501) staff       (20)     1871 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R115_file_deletion.py
--rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R116_insecure_file_permission.md
--rw-r--r--   0 hiro       (501) staff       (20)     1649 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R116_insecure_file_permission.py
--rw-r--r--   0 hiro       (501) staff       (20)     1661 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R117_external_role.py
--rw-r--r--   0 hiro       (501) staff       (20)     1927 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R201_changed_data_dependence.py
--rw-r--r--   0 hiro       (501) staff       (20)     2123 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R202_unconditional_override.py
--rw-r--r--   0 hiro       (501) staff       (20)     2181 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R203_unused_override.py
--rw-r--r--   0 hiro       (501) staff       (20)     2180 2023-03-28 00:46:23.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R204_unnecessary_set_fact.py
--rw-r--r--   0 hiro       (501) staff       (20)     1707 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R205_unnecessary_include_vars.py
--rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R301_non_fqcn_use.md
--rw-r--r--   0 hiro       (501) staff       (20)     1827 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R301_non_fqcn_use.py
--rw-r--r--   0 hiro       (501) staff       (20)     1430 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R302_role_without_metadata.py
--rw-r--r--   0 hiro       (501) staff       (20)     1416 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R303_task_without_name.py
--rw-r--r--   0 hiro       (501) staff       (20)     1607 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R304_unresolved_module.py
--rw-r--r--   0 hiro       (501) staff       (20)     1712 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R305_unresolved_role.py
--rw-r--r--   0 hiro       (501) staff       (20)     1787 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R306_undefined_variable.py
--rw-r--r--   0 hiro       (501) staff       (20)     1925 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R401_list_all_inbound_src.py
--rw-r--r--   0 hiro       (501) staff       (20)     1609 2023-05-19 01:44:11.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R402_list_all_used_variables.py
--rw-r--r--   0 hiro       (501) staff       (20)     1939 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R404_show_variables.py
--rw-r--r--   0 hiro       (501) staff       (20)     1974 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R501_dependency_suggestion.py
--rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     5279 2023-04-21 02:09:38.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/rule_versions.json
--rw-r--r--   0 hiro       (501) staff       (20)     1521 2023-05-19 01:44:11.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/rules/sample_rule.py
--rw-r--r--   0 hiro       (501) staff       (20)     4224 2023-10-30 09:29:08.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/safe_glob.py
--rw-r--r--   0 hiro       (501) staff       (20)    49966 2023-11-07 08:35:00.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/scanner.py
--rw-r--r--   0 hiro       (501) staff       (20)      401 2023-08-09 02:54:04.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/task_keywords.txt
--rw-r--r--   0 hiro       (501) staff       (20)    43584 2023-11-09 06:35:46.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/tree.py
--rw-r--r--   0 hiro       (501) staff       (20)    24692 2023-11-06 06:09:52.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/utils.py
--rw-r--r--   0 hiro       (501) staff       (20)      939 2022-12-14 05:36:09.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/variable_manager.py
--rw-r--r--   0 hiro       (501) staff       (20)     2251 2023-10-25 00:46:32.000000 ansible-risk-insight-0.2.4/ansible_risk_insight/yaml.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.746093 ansible-risk-insight-0.2.4/ansible_risk_insight.egg-info/
--rw-r--r--   0 hiro       (501) staff       (20)      272 2023-11-16 01:44:53.000000 ansible-risk-insight-0.2.4/ansible_risk_insight.egg-info/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     8147 2023-11-16 01:44:53.000000 ansible-risk-insight-0.2.4/ansible_risk_insight.egg-info/SOURCES.txt
--rw-r--r--   0 hiro       (501) staff       (20)        1 2023-11-16 01:44:53.000000 ansible-risk-insight-0.2.4/ansible_risk_insight.egg-info/dependency_links.txt
--rw-r--r--   0 hiro       (501) staff       (20)       99 2023-11-16 01:44:53.000000 ansible-risk-insight-0.2.4/ansible_risk_insight.egg-info/entry_points.txt
--rw-r--r--   0 hiro       (501) staff       (20)      103 2023-11-16 01:44:53.000000 ansible-risk-insight-0.2.4/ansible_risk_insight.egg-info/requires.txt
--rw-r--r--   0 hiro       (501) staff       (20)       21 2023-11-16 01:44:53.000000 ansible-risk-insight-0.2.4/ansible_risk_insight.egg-info/top_level.txt
--rw-r--r--   0 hiro       (501) staff       (20)     1473 2022-12-14 05:36:09.000000 ansible-risk-insight-0.2.4/data-struct.txt
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.725888 ansible-risk-insight-0.2.4/doc/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.778937 ansible-risk-insight-0.2.4/doc/images/
--rw-r--r--   0 hiro       (501) staff       (20)   169018 2023-02-27 07:18:31.000000 ansible-risk-insight-0.2.4/doc/images/ari-apply-rules.png
--rw-r--r--   0 hiro       (501) staff       (20)   403143 2023-02-27 07:18:31.000000 ansible-risk-insight-0.2.4/doc/images/ari-arch.png
--rw-r--r--   0 hiro       (501) staff       (20)   316218 2023-02-27 07:18:31.000000 ansible-risk-insight-0.2.4/doc/images/ari-overview.png
--rw-r--r--   0 hiro       (501) staff       (20)   473549 2023-02-27 07:18:31.000000 ansible-risk-insight-0.2.4/doc/images/ari-ram-list.png
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.781296 ansible-risk-insight-0.2.4/docs/
--rw-r--r--   0 hiro       (501) staff       (20)     2179 2023-03-01 02:03:44.000000 ansible-risk-insight-0.2.4/docs/annotation.md
--rw-r--r--   0 hiro       (501) staff       (20)     6685 2023-02-27 08:35:40.000000 ansible-risk-insight-0.2.4/docs/customize_rules.md
--rw-r--r--   0 hiro       (501) staff       (20)      458 2023-02-07 04:27:33.000000 ansible-risk-insight-0.2.4/docs/index.md
--rw-r--r--   0 hiro       (501) staff       (20)      188 2023-02-07 04:27:33.000000 ansible-risk-insight-0.2.4/docs/installing.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.785916 ansible-risk-insight-0.2.4/docs/rules/
--rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/docs/rules/R101_command_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/docs/rules/R102_command_instead_of_shell.md
--rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/docs/rules/R103_download_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/docs/rules/R104_unauthorized_download_src.md
--rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/docs/rules/R105_outbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/docs/rules/R106_inbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/docs/rules/R107_pkg_install_with_insecure_option.md
--rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/docs/rules/R108_privilege_escalation.md
--rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/docs/rules/R109_key_config_change.md
--rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/docs/rules/R110_non_builtin_use.md
--rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/docs/rules/R111_parameterized_import_role.md
--rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/docs/rules/R112_parameterized_import_taskfile.md
--rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/docs/rules/R113_parameterized_pkg_install.md
--rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/docs/rules/R114_file_change.md
--rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/docs/rules/R115_file_deletion.md
--rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/docs/rules/R116_insecure_file_permission.md
--rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.4/docs/rules/R301_non_fqcn_use.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.786631 ansible-risk-insight-0.2.4/example/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.786989 ansible-risk-insight-0.2.4/example/playbooks/
--rw-r--r--   0 hiro       (501) staff       (20)      509 2023-03-06 00:24:15.000000 ansible-risk-insight-0.2.4/example/playbooks/sample_playbook.yml
--rw-r--r--   0 hiro       (501) staff       (20)     1106 2023-03-06 00:24:15.000000 ansible-risk-insight-0.2.4/example/readme.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.787259 ansible-risk-insight-0.2.4/example/rules/
--rw-r--r--   0 hiro       (501) staff       (20)     1366 2023-03-06 00:24:15.000000 ansible-risk-insight-0.2.4/example/rules/sample_rule.py
--rw-r--r--   0 hiro       (501) staff       (20)     1728 2023-03-23 08:17:04.000000 ansible-risk-insight-0.2.4/example/sample.py
--rw-r--r--   0 hiro       (501) staff       (20)     1300 2023-02-07 04:27:33.000000 ansible-risk-insight-0.2.4/mkdocs.yml
--rw-r--r--   0 hiro       (501) staff       (20)     1012 2023-08-01 01:36:12.000000 ansible-risk-insight-0.2.4/pyproject.toml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.789023 ansible-risk-insight-0.2.4/scripts/
--rw-r--r--   0 hiro       (501) staff       (20)     5105 2023-09-28 07:31:01.000000 ansible-risk-insight-0.2.4/scripts/gen_ram_slim.py
--rw-r--r--   0 hiro       (501) staff       (20)     5964 2023-09-26 07:25:31.000000 ansible-risk-insight-0.2.4/scripts/gen_ram_subset.py
--rw-r--r--   0 hiro       (501) staff       (20)       38 2023-11-16 01:44:53.792648 ansible-risk-insight-0.2.4/setup.cfg
--rw-r--r--   0 hiro       (501) staff       (20)       38 2022-12-16 00:52:20.000000 ansible-risk-insight-0.2.4/setup.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.789575 ansible-risk-insight-0.2.4/test/
--rw-r--r--   0 hiro       (501) staff       (20)     2668 2023-08-18 09:09:38.000000 ansible-risk-insight-0.2.4/test/test_scanner.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.727166 ansible-risk-insight-0.2.4/test/testdata/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.726635 ansible-risk-insight-0.2.4/test/testdata/projects/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.790390 ansible-risk-insight-0.2.4/test/testdata/projects/my.collection/
--rw-r--r--   0 hiro       (501) staff       (20)      845 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.4/test/testdata/projects/my.collection/MANIFEST.json
--rw-r--r--   0 hiro       (501) staff       (20)      460 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.4/test/testdata/projects/my.collection/galaxy.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.726805 ansible-risk-insight-0.2.4/test/testdata/projects/my.collection/roles/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.727055 ansible-risk-insight-0.2.4/test/testdata/projects/my.collection/roles/sample-role-1/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.790670 ansible-risk-insight-0.2.4/test/testdata/projects/my.collection/roles/sample-role-1/defaults/
--rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.4/test/testdata/projects/my.collection/roles/sample-role-1/defaults/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.790908 ansible-risk-insight-0.2.4/test/testdata/projects/my.collection/roles/sample-role-1/meta/
--rw-r--r--   0 hiro       (501) staff       (20)      418 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.4/test/testdata/projects/my.collection/roles/sample-role-1/meta/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.791139 ansible-risk-insight-0.2.4/test/testdata/projects/my.collection/roles/sample-role-1/tasks/
--rw-r--r--   0 hiro       (501) staff       (20)       79 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.4/test/testdata/projects/my.collection/roles/sample-role-1/tasks/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.727230 ansible-risk-insight-0.2.4/test/testdata/roles/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.727485 ansible-risk-insight-0.2.4/test/testdata/roles/test_role/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.791386 ansible-risk-insight-0.2.4/test/testdata/roles/test_role/defaults/
--rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.4/test/testdata/roles/test_role/defaults/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.791885 ansible-risk-insight-0.2.4/test/testdata/roles/test_role/meta/
--rw-r--r--   0 hiro       (501) staff       (20)      414 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.4/test/testdata/roles/test_role/meta/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-16 01:44:53.792159 ansible-risk-insight-0.2.4/test/testdata/roles/test_role/tasks/
--rw-r--r--   0 hiro       (501) staff       (20)      212 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.4/test/testdata/roles/test_role/tasks/main.yml
--rw-r--r--   0 hiro       (501) staff       (20)      589 2023-01-05 06:52:13.000000 ansible-risk-insight-0.2.4/tox.ini
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.449210 ansible-risk-insight-0.2.5/
+-rw-r--r--   0 hiro       (501) staff       (20)       46 2022-12-14 05:36:09.000000 ansible-risk-insight-0.2.5/.flake8
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.403555 ansible-risk-insight-0.2.5/.github/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.407896 ansible-risk-insight-0.2.5/.github/workflows/
+-rw-r--r--   0 hiro       (501) staff       (20)      832 2022-12-16 00:52:20.000000 ansible-risk-insight-0.2.5/.github/workflows/lint.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      793 2023-08-22 04:18:04.000000 ansible-risk-insight-0.2.5/.github/workflows/test.yml
+-rw-r--r--   0 hiro       (501) staff       (20)     1799 2023-03-23 07:29:42.000000 ansible-risk-insight-0.2.5/.gitignore
+-rw-r--r--   0 hiro       (501) staff       (20)      436 2022-12-16 00:52:20.000000 ansible-risk-insight-0.2.5/.pre-commit-config.yaml
+-rw-r--r--   0 hiro       (501) staff       (20)      990 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.5/CONTRIBUTING.md
+-rw-r--r--   0 hiro       (501) staff       (20)    11357 2022-12-14 05:36:09.000000 ansible-risk-insight-0.2.5/LICENSE
+-rw-r--r--   0 hiro       (501) staff       (20)      456 2022-12-16 00:52:20.000000 ansible-risk-insight-0.2.5/Makefile
+-rw-r--r--   0 hiro       (501) staff       (20)      272 2024-04-25 12:40:09.449064 ansible-risk-insight-0.2.5/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     4510 2023-02-27 07:18:31.000000 ansible-risk-insight-0.2.5/README.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.415675 ansible-risk-insight-0.2.5/ansible_risk_insight/
+-rw-r--r--   0 hiro       (501) staff       (20)     1907 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)      659 2024-04-25 12:37:00.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/_version.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3519 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/analyzer.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.418436 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/
+-rw-r--r--   0 hiro       (501) staff       (20)      636 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1408 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/annotator_base.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.422058 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/
+-rw-r--r--   0 hiro       (501) staff       (20)     1393 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/apt.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1587 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/apt_key.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1446 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/assemble.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1460 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1388 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/command.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1498 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/dnf.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1447 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/expect.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/file.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1320 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/get_url.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1317 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/git.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1511 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1339 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/pip.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1380 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/raw.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1448 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/replace.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1371 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1386 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/script.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1384 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/shell.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1327 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/subversion.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/template.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2221 2024-04-25 12:09:32.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/unarchive.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/uri.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1498 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/yum.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1230 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible_builtin.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46432 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible_builtin.py.bak
+-rw-r--r--   0 hiro       (501) staff       (20)     1113 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/module_annotator_base.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2846 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/risk_annotator_base.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2381 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/sample_custom_annotator.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9222 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/variable_resolver.py
+-rw-r--r--   0 hiro       (501) staff       (20)   846979 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/ansible_builtin_modules.json
+-rw-r--r--   0 hiro       (501) staff       (20)     2306 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/ansible_variables.txt
+-rw-r--r--   0 hiro       (501) staff       (20)     3211 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/awx_utils.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      678 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/batch.sh
+-rw-r--r--   0 hiro       (501) staff       (20)     1049 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/builtin-modules.txt
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.422228 ansible-risk-insight-0.2.5/ansible_risk_insight/cli/
+-rw-r--r--   0 hiro       (501) staff       (20)     7770 2024-04-25 11:59:38.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/cli/__init__.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.423358 ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/
+-rw-r--r--   0 hiro       (501) staff       (20)     2032 2023-09-26 03:55:49.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1705 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/diff.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3085 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/generate.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1486 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/list.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1690 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/release.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1720 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/search.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2033 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/update.py
+-rw-r--r--   0 hiro       (501) staff       (20)    31923 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/context.py
+-rw-r--r--   0 hiro       (501) staff       (20)    48633 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/dependency_dir_preparator.py
+-rw-r--r--   0 hiro       (501) staff       (20)    14850 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/dependency_finder.py
+-rw-r--r--   0 hiro       (501) staff       (20)    20780 2024-01-05 07:03:36.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/finder.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2683 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/findings.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1291 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/key_test.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8582 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/keyutil.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8728 2024-04-25 12:13:13.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/loader.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1615 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/logger.py
+-rw-r--r--   0 hiro       (501) staff       (20)    73469 2024-04-25 12:06:34.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/model_loader.py
+-rw-r--r--   0 hiro       (501) staff       (20)    82614 2024-04-25 12:09:28.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/models.py
+-rw-r--r--   0 hiro       (501) staff       (20)    26942 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/parser.py
+-rw-r--r--   0 hiro       (501) staff       (20)     5955 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/ram_generator.py
+-rw-r--r--   0 hiro       (501) staff       (20)      105 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/requirements.txt
+-rw-r--r--   0 hiro       (501) staff       (20)    45276 2024-03-26 08:07:23.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/risk_assessment_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8376 2024-01-18 10:18:59.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/risk_detector.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.436027 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)     4292 2024-04-25 11:59:38.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/P001_module_name_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     6677 2024-01-18 10:18:42.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/P002_module_argument_key_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     7106 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/P003_module_argument_value_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3418 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/P004_variable_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R101_command_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1801 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R101_command_exec.py
+-rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R102_command_instead_of_shell.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1684 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R102_command_instead_of_shell.py
+-rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R103_download_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2703 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R103_download_exec.py
+-rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R104_unauthorized_download_src.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2370 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R104_unauthorized_download_src.py
+-rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R105_outbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1846 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R105_outbound_transfer.py
+-rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R106_inbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1947 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R106_inbound_transfer.py
+-rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2066 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py
+-rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R108_privilege_escalation.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1536 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R108_privilege_escalation.py
+-rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R109_key_config_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1756 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R109_key_config_change.py
+-rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R110_non_builtin_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1642 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R110_non_builtin_use.py
+-rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R111_parameterized_import_role.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1729 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R111_parameterized_import_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R112_parameterized_import_taskfile.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1952 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R113_parameterized_pkg_install.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1875 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R113_parameterized_pkg_install.py
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R114_file_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2088 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R114_file_change.py
+-rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R115_file_deletion.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1871 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R115_file_deletion.py
+-rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R116_insecure_file_permission.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1649 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R116_insecure_file_permission.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1661 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R117_external_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1927 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R201_changed_data_dependence.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2123 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R202_unconditional_override.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2181 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R203_unused_override.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2180 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R204_unnecessary_set_fact.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1707 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R205_unnecessary_include_vars.py
+-rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R301_non_fqcn_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1827 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R301_non_fqcn_use.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1430 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R302_role_without_metadata.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1416 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R303_task_without_name.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1607 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R304_unresolved_module.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1712 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R305_unresolved_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1787 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R306_undefined_variable.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1925 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R401_list_all_inbound_src.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1609 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R402_list_all_used_variables.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1939 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R404_show_variables.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1974 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R501_dependency_suggestion.py
+-rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     5279 2023-04-21 02:09:38.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/rule_versions.json
+-rw-r--r--   0 hiro       (501) staff       (20)     1521 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/sample_rule.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4224 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/safe_glob.py
+-rw-r--r--   0 hiro       (501) staff       (20)    49966 2024-01-26 00:47:50.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/scanner.py
+-rw-r--r--   0 hiro       (501) staff       (20)      401 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/task_keywords.txt
+-rw-r--r--   0 hiro       (501) staff       (20)    43475 2024-04-25 12:17:59.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/tree.py
+-rw-r--r--   0 hiro       (501) staff       (20)    24692 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/utils.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2251 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/yaml.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.416578 ansible-risk-insight-0.2.5/ansible_risk_insight.egg-info/
+-rw-r--r--   0 hiro       (501) staff       (20)      272 2024-04-25 12:40:09.000000 ansible-risk-insight-0.2.5/ansible_risk_insight.egg-info/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     8106 2024-04-25 12:40:09.000000 ansible-risk-insight-0.2.5/ansible_risk_insight.egg-info/SOURCES.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        1 2024-04-25 12:40:09.000000 ansible-risk-insight-0.2.5/ansible_risk_insight.egg-info/dependency_links.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       99 2024-04-25 12:40:09.000000 ansible-risk-insight-0.2.5/ansible_risk_insight.egg-info/entry_points.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       99 2024-04-25 12:40:09.000000 ansible-risk-insight-0.2.5/ansible_risk_insight.egg-info/requires.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       21 2024-04-25 12:40:09.000000 ansible-risk-insight-0.2.5/ansible_risk_insight.egg-info/top_level.txt
+-rw-r--r--   0 hiro       (501) staff       (20)     1473 2022-12-14 05:36:09.000000 ansible-risk-insight-0.2.5/data-struct.txt
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.404338 ansible-risk-insight-0.2.5/doc/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.437271 ansible-risk-insight-0.2.5/doc/images/
+-rw-r--r--   0 hiro       (501) staff       (20)   169018 2023-02-27 07:18:31.000000 ansible-risk-insight-0.2.5/doc/images/ari-apply-rules.png
+-rw-r--r--   0 hiro       (501) staff       (20)   403143 2023-02-27 07:18:31.000000 ansible-risk-insight-0.2.5/doc/images/ari-arch.png
+-rw-r--r--   0 hiro       (501) staff       (20)   316218 2023-02-27 07:18:31.000000 ansible-risk-insight-0.2.5/doc/images/ari-overview.png
+-rw-r--r--   0 hiro       (501) staff       (20)   473549 2023-02-27 07:18:31.000000 ansible-risk-insight-0.2.5/doc/images/ari-ram-list.png
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.438197 ansible-risk-insight-0.2.5/docs/
+-rw-r--r--   0 hiro       (501) staff       (20)     2179 2023-03-01 02:03:44.000000 ansible-risk-insight-0.2.5/docs/annotation.md
+-rw-r--r--   0 hiro       (501) staff       (20)     6685 2023-02-27 08:35:40.000000 ansible-risk-insight-0.2.5/docs/customize_rules.md
+-rw-r--r--   0 hiro       (501) staff       (20)      458 2023-02-07 04:27:33.000000 ansible-risk-insight-0.2.5/docs/index.md
+-rw-r--r--   0 hiro       (501) staff       (20)      188 2023-02-07 04:27:33.000000 ansible-risk-insight-0.2.5/docs/installing.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.440672 ansible-risk-insight-0.2.5/docs/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R101_command_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R102_command_instead_of_shell.md
+-rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R103_download_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R104_unauthorized_download_src.md
+-rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R105_outbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R106_inbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R107_pkg_install_with_insecure_option.md
+-rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R108_privilege_escalation.md
+-rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R109_key_config_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R110_non_builtin_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R111_parameterized_import_role.md
+-rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R112_parameterized_import_taskfile.md
+-rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R113_parameterized_pkg_install.md
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R114_file_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R115_file_deletion.md
+-rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R116_insecure_file_permission.md
+-rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R301_non_fqcn_use.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.440995 ansible-risk-insight-0.2.5/example/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.441158 ansible-risk-insight-0.2.5/example/playbooks/
+-rw-r--r--   0 hiro       (501) staff       (20)      509 2023-03-06 00:24:15.000000 ansible-risk-insight-0.2.5/example/playbooks/sample_playbook.yml
+-rw-r--r--   0 hiro       (501) staff       (20)     1106 2023-03-06 00:24:15.000000 ansible-risk-insight-0.2.5/example/readme.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.441312 ansible-risk-insight-0.2.5/example/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)     1366 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.5/example/rules/sample_rule.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1728 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/example/sample.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1300 2023-02-07 04:27:33.000000 ansible-risk-insight-0.2.5/mkdocs.yml
+-rw-r--r--   0 hiro       (501) staff       (20)     1001 2024-04-25 11:59:15.000000 ansible-risk-insight-0.2.5/pyproject.toml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.441673 ansible-risk-insight-0.2.5/scripts/
+-rw-r--r--   0 hiro       (501) staff       (20)     5105 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/scripts/gen_ram_slim.py
+-rw-r--r--   0 hiro       (501) staff       (20)     5964 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/scripts/gen_ram_subset.py
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2024-04-25 12:40:09.449255 ansible-risk-insight-0.2.5/setup.cfg
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2022-12-16 00:52:20.000000 ansible-risk-insight-0.2.5/setup.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.441842 ansible-risk-insight-0.2.5/test/
+-rw-r--r--   0 hiro       (501) staff       (20)     2668 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/test/test_scanner.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.405486 ansible-risk-insight-0.2.5/test/testdata/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.405068 ansible-risk-insight-0.2.5/test/testdata/projects/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.442204 ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/
+-rw-r--r--   0 hiro       (501) staff       (20)      845 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/MANIFEST.json
+-rw-r--r--   0 hiro       (501) staff       (20)      460 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/galaxy.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.405205 ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/roles/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.405409 ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/roles/sample-role-1/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.446147 ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/roles/sample-role-1/defaults/
+-rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/roles/sample-role-1/defaults/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.446473 ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/roles/sample-role-1/meta/
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/roles/sample-role-1/meta/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.446639 ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/roles/sample-role-1/tasks/
+-rw-r--r--   0 hiro       (501) staff       (20)       79 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/roles/sample-role-1/tasks/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.405542 ansible-risk-insight-0.2.5/test/testdata/roles/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.405751 ansible-risk-insight-0.2.5/test/testdata/roles/test_role/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.447645 ansible-risk-insight-0.2.5/test/testdata/roles/test_role/defaults/
+-rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.5/test/testdata/roles/test_role/defaults/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.448667 ansible-risk-insight-0.2.5/test/testdata/roles/test_role/meta/
+-rw-r--r--   0 hiro       (501) staff       (20)      414 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.5/test/testdata/roles/test_role/meta/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.448842 ansible-risk-insight-0.2.5/test/testdata/roles/test_role/tasks/
+-rw-r--r--   0 hiro       (501) staff       (20)      212 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.5/test/testdata/roles/test_role/tasks/main.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      589 2023-01-05 06:52:13.000000 ansible-risk-insight-0.2.5/tox.ini
```

### Comparing `ansible-risk-insight-0.2.4/.github/workflows/lint.yml` & `ansible-risk-insight-0.2.5/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/.github/workflows/test.yml` & `ansible-risk-insight-0.2.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/.gitignore` & `ansible-risk-insight-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/CONTRIBUTING.md` & `ansible-risk-insight-0.2.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/LICENSE` & `ansible-risk-insight-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/README.md` & `ansible-risk-insight-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/__init__.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/_version.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
```

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/analyzer.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/analyzer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/__init__.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/annotator_base.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/apt.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/apt.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/apt_key.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/apt_key.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/assemble.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/assemble.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/command.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/command.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/dnf.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/dnf.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/expect.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/expect.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/file.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/file.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/get_url.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/get_url.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/git.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/git.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/pip.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/pip.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/raw.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/raw.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/replace.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/replace.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/script.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/script.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/shell.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/shell.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/subversion.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/subversion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/template.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/template.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/unarchive.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/unarchive.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/uri.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/uri.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible.builtin/yum.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/yum.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible_builtin.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible_builtin.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/ansible_builtin.py.bak` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible_builtin.py.bak`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/module_annotator_base.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/module_annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/risk_annotator_base.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/risk_annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/sample_custom_annotator.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/sample_custom_annotator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/annotators/variable_resolver.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/variable_resolver.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/ansible_builtin_modules.json` & `ansible-risk-insight-0.2.5/ansible_risk_insight/ansible_builtin_modules.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/ansible_variables.txt` & `ansible-risk-insight-0.2.5/ansible_risk_insight/ansible_variables.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/awx_utils.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/awx_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/batch.sh` & `ansible-risk-insight-0.2.5/ansible_risk_insight/batch.sh`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/builtin-modules.txt` & `ansible-risk-insight-0.2.5/ansible_risk_insight/builtin-modules.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/cli/__init__.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/cli/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,17 @@
             action="store_true",
             help="enable file save under ARI_DATA_DIR (default=/tmp/ari-data)",
         )
         parser.add_argument("target_type", help="Content type", choices={"project", "role", "collection", "playbook", "taskfile"})
         parser.add_argument("target_name", help="Name")
         parser.add_argument("--playbook-only", action="store_true", help="if true, don't load playbooks/roles arround the specified playbook")
         parser.add_argument("--taskfile-only", action="store_true", help="if true, don't load playbooks/roles arround the specified taskfile")
+        parser.add_argument(
+            "--skip-isolated-taskfiles", action="store_true", help="if true, skip isolated (not imported/included) taskfiles from roles"
+        )
         parser.add_argument("--skip-install", action="store_true", help="if true, skip install for the specified target")
         parser.add_argument("--dependency-dir", nargs="?", help="path to a directory that have dependencies for the target")
         parser.add_argument("--collection-name", nargs="?", help="if provided, use it as a collection name")
         parser.add_argument("--role-name", nargs="?", help="if provided, use it as a role name")
         parser.add_argument("--source", help="source server name in ansible config file (if empty, use public ansible galaxy)")
         parser.add_argument("--without-ram", action="store_true", help="if true, RAM data is not used and not even updated")
         parser.add_argument("--read-only-ram", action="store_true", help="if true, RAM data is used but not updated")
@@ -129,14 +132,17 @@
             read_ram_for_dependency = True
             read_ram = False
             write_ram = False
         elif args.include_tests:
             read_ram_for_dependency = True
             read_ram = False
             write_ram = False
+        load_all_taskfiles = True
+        if args.skip_isolated_taskfiles:
+            load_all_taskfiles = False
 
         c = ARIScanner(
             root_dir=config.data_dir,
             rules_dir=rules_dir,
             do_save=args.save,
             read_ram=read_ram,
             write_ram=write_ram,
@@ -159,10 +165,11 @@
             dependency_dir=args.dependency_dir,
             collection_name=collection_name,
             role_name=role_name,
             source_repository=args.source,
             playbook_only=args.playbook_only,
             taskfile_only=args.taskfile_only,
             include_test_contents=args.include_tests,
+            load_all_taskfiles=load_all_taskfiles,
             objects=args.objects,
             out_dir=args.out_dir,
         )
```

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/cli/ram/__init__.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/cli/ram/diff.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/diff.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/cli/ram/generate.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/generate.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/cli/ram/list.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/list.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/cli/ram/release.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/release.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/cli/ram/search.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/search.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/cli/ram/update.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/update.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/context.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/context.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/dependency_dir_preparator.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/dependency_dir_preparator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/dependency_finder.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/dependency_finder.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/finder.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/finder.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from dataclasses import dataclass
 from pathlib import Path
 import re
 import os
+import json
 import yaml
 import traceback
 
 try:
     # if `libyaml` is available, use C based loader for performance
     import _yaml  # noqa: F401
     from yaml import CSafeLoader as Loader
@@ -273,14 +274,21 @@
     ]
     files = safe_glob(patterns=inventory_file_patterns, recursive=True)
     return files
 
 
 def find_best_repo_root_path(path):
     base_path = path
+
+    manifest_json_path = os.path.join(base_path, "MANIFEST.json")
+    galaxy_yml_path = os.path.join(base_path, "galaxy.yml")
+    meta_main_yml_path = os.path.join(base_path, "meta/main.yml")
+    if os.path.exists(manifest_json_path) or os.path.exists(galaxy_yml_path) or os.path.exists(meta_main_yml_path):
+        return base_path
+
     # get all possible playbooks
     playbooks = search_playbooks(path)
     # sort by directory depth to find the most top playbook
     playbooks = sorted(playbooks, key=lambda x: len(x.split(os.sep)))
     # still "repo/xxxxx/sample1.yml" may come before
     # "repo/playbooks/sample2.yml" because the depth are same,
     # so specifically put "playbooks" or "playbook" ones first
@@ -322,38 +330,46 @@
             if len(candidate) < len(root_path):
                 root_path = candidate
 
     return root_path
 
 
 def find_collection_name_of_repo(path):
-    pattern = os.path.join(path, "**/galaxy.yml")
-    found_galaxy_ymls = safe_glob(pattern, recursive=True)
-    found_galaxy_ymls = [fpath for fpath in found_galaxy_ymls if github_workflows_dir not in fpath]
-
-    # skip galaxy ymls found in collections/roles in the repository
-    _galaxy_ymls = []
-    for gpath in found_galaxy_ymls:
-        relative_path = gpath.replace(path, "", 1)
+    galaxy_yml_pattern = os.path.join(path, "**/galaxy.yml")
+    manifest_json_pattern = os.path.join(path, "**/MANIFEST.json")
+    found_metadata_files = safe_glob([galaxy_yml_pattern, manifest_json_pattern], recursive=True)
+    found_metadata_files = [fpath for fpath in found_metadata_files if github_workflows_dir not in fpath]
+
+    # skip metadata files found in collections/roles in the repository
+    _metadata_files = []
+    for mpath in found_metadata_files:
+        relative_path = mpath.replace(path, "", 1)
         if "/collections/" in relative_path:
             continue
         if "/roles/" in relative_path:
             continue
-        _galaxy_ymls.append(gpath)
-    found_galaxy_ymls = _galaxy_ymls
+        _metadata_files.append(mpath)
+    found_metadata_files = _metadata_files
 
     my_collection_name = ""
-    if len(found_galaxy_ymls) > 0:
-        galaxy_yml = found_galaxy_ymls[0]
+    if len(found_metadata_files) > 0:
+        metadata_file = found_metadata_files[0]
         my_collection_info = None
-        with open(galaxy_yml, "r") as file:
-            try:
-                my_collection_info = yaml.load(file, Loader=Loader)
-            except Exception as e:
-                logger.debug("failed to load this yaml file to read galaxy.yml; {}".format(e.args[0]))
+        if metadata_file.endswith(".yml"):
+            with open(metadata_file, "r") as file:
+                try:
+                    my_collection_info = yaml.load(file, Loader=Loader)
+                except Exception as e:
+                    logger.debug("failed to load this yaml file to read galaxy.yml; {}".format(e.args[0]))
+        elif metadata_file.endswith(".json"):
+            with open(metadata_file, "r") as file:
+                try:
+                    my_collection_info = json.load(file).get("collection_info", {})
+                except Exception as e:
+                    logger.debug("failed to load this json file to read MANIFEST.json; {}".format(e.args[0]))
         if my_collection_info is None:
             return ""
         namespace = my_collection_info.get("namespace", "")
         name = my_collection_info.get("name", "")
         my_collection_name = "{}.{}".format(namespace, name)
     return my_collection_name
 
@@ -502,15 +518,15 @@
                     for at in _alt_targets:
                         if at in relative_path:
                             _target = at
                             break
 
                     _path = relative_path.rsplit(_target, 1)[0]
                     role_name = _path.split("/")[-1]
-                    role_path = os.path.join(parent_dir, p[1:], role_name)
+                    role_path = os.path.join(parent_dir, _path)
                     found = True
                     break
         if found:
             break
     return role_name, role_path
```

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/findings.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/findings.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/key_test.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/key_test.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/keyutil.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/keyutil.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/loader.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import pathlib
 import json
-import pygit2
 import pkg_resources
 from .models import LoadType
 
 collection_manifest_json = "MANIFEST.json"
 role_meta_main_yml = "meta/main.yml"
 role_meta_main_yaml = "meta/main.yaml"
 
@@ -55,17 +54,18 @@
         version = pkg_resources.require("ansible-risk-insight")[0].version
     except Exception:
         pass
     if version != "":
         return version
     # try to get version from commit ID in source code repository
     try:
-        script_dir = pathlib.Path(__file__).parent.resolve()
-        repo = pygit2.Repository(script_dir)
-        version = repo.head.target
+        # TODO: consider how to get git version if it is needed
+        _ = pathlib.Path(__file__).parent.resolve()
+        # repo = pygit2.Repository(script_dir)
+        # version = repo.head.target
     except Exception:
         pass
     return version
 
 
 def get_target_name(target_type, target_path):
     target_name = ""
```

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/logger.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/logger.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/model_loader.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/model_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,26 +119,32 @@
     include_test_contents=False,
     yaml_label_list=None,
     load_children=True,
 ):
     repoObj = Repository()
 
     repo_path = ""
+    repo_to_root = ""
     if path == "":
         # if path is empty, just load installed collections / roles
         repo_path = ""
     else:
         # otherwise, find the root path by searching playbooks
         try:
             repo_path = find_best_repo_root_path(path)
+            repo_to_root = os.path.relpath(path, repo_path)
         except Exception as exc:
             logger.debug(f'failed to find a root directory for a project in "{path}"; error: {exc}')
             # if an exception occurs while finding repo root, use the input path as repo root
             repo_path = path
 
+    # if `path` and `repo_path` are different, update yaml_label_list
+    if repo_to_root and yaml_label_list:
+        yaml_label_list = [(os.path.normpath(os.path.join(repo_to_root, fpath)), label, role_info) for (fpath, label, role_info) in yaml_label_list]
+
     if repo_path != "":
         if my_collection_name == "":
             my_collection_name = find_collection_name_of_repo(repo_path)
         if my_collection_name != "":
             repoObj.my_collection_name = my_collection_name
 
     if basedir == "":
@@ -472,14 +478,15 @@
             pass
         elif k == "pre_tasks":
             if not isinstance(v, list):
                 continue
             task_blocks, _ = get_task_blocks(task_dict_list=v)
             if task_blocks is None:
                 continue
+            last_task_line_num = -1
             for task_dict in task_blocks:
                 task_loading["total"] += 1
                 i = task_count
                 error = None
                 try:
                     t = load_task(
                         path=path,
@@ -488,19 +495,22 @@
                         role_name=role_name,
                         collection_name=collection_name,
                         collections_in_play=collections_in_play,
                         play_index=index,
                         parent_key=pbObj.key,
                         parent_local_key=pbObj.local_key,
                         yaml_lines=yaml_lines,
+                        previous_task_line=last_task_line_num,
                         basedir=basedir,
                     )
                     pre_tasks.append(t)
                     if t:
                         task_loading["success"] += 1
+                        if t.line_num_in_file and len(t.line_num_in_file) == 2:
+                            last_task_line_num = t.line_num_in_file[1]
                 except TaskFormatError as exc:
                     error = exc
                     if skip_task_format_error:
                         logger.debug("this task is wrong format; skip the task in {}," " index: {}; skip this".format(path, i))
                     else:
                         raise TaskFormatError(f"this task is wrong format; skip the task in {path}," " index: {i}")
                 except Exception as exc:
@@ -513,14 +523,15 @@
                         task_loading["errors"].append(error)
         elif k == "tasks":
             if not isinstance(v, list):
                 continue
             task_blocks, _ = get_task_blocks(task_dict_list=v)
             if task_blocks is None:
                 continue
+            last_task_line_num = -1
             for task_dict in task_blocks:
                 i = task_count
                 task_loading["total"] += 1
                 error = None
                 try:
                     t = load_task(
                         path=path,
@@ -529,19 +540,22 @@
                         role_name=role_name,
                         collection_name=collection_name,
                         collections_in_play=collections_in_play,
                         play_index=index,
                         parent_key=pbObj.key,
                         parent_local_key=pbObj.local_key,
                         yaml_lines=yaml_lines,
+                        previous_task_line=last_task_line_num,
                         basedir=basedir,
                     )
                     tasks.append(t)
                     if t:
                         task_loading["success"] += 1
+                        if t.line_num_in_file and len(t.line_num_in_file) == 2:
+                            last_task_line_num = t.line_num_in_file[1]
                 except TaskFormatError as exc:
                     error = exc
                     if skip_task_format_error:
                         logger.debug("this task is wrong format; skip the task in {}," " index: {}; skip this".format(path, i))
                     else:
                         raise TaskFormatError(f"this task is wrong format; skip the task in {path}," " index: {i}")
                 except Exception as exc:
@@ -554,14 +568,15 @@
                         task_loading["errors"].append(error)
         elif k == "post_tasks":
             if not isinstance(v, list):
                 continue
             task_blocks, _ = get_task_blocks(task_dict_list=v)
             if task_blocks is None:
                 continue
+            last_task_line_num = -1
             for task_dict in task_blocks:
                 i = task_count
                 task_loading["total"] += 1
                 error = None
                 try:
                     t = load_task(
                         path=path,
@@ -570,19 +585,22 @@
                         role_name=role_name,
                         collection_name=collection_name,
                         collections_in_play=collections_in_play,
                         play_index=index,
                         parent_key=pbObj.key,
                         parent_local_key=pbObj.local_key,
                         yaml_lines=yaml_lines,
+                        previous_task_line=last_task_line_num,
                         basedir=basedir,
                     )
                     post_tasks.append(t)
                     if t:
                         task_loading["success"] += 1
+                        if t.line_num_in_file and len(t.line_num_in_file) == 2:
+                            last_task_line_num = t.line_num_in_file[1]
                 except TaskFormatError as exc:
                     error = exc
                     if skip_task_format_error:
                         logger.debug("this task is wrong format; skip the task in {}," " index: {}; skip this".format(path, i))
                     else:
                         raise TaskFormatError(f"this task is wrong format; skip the task in {path}," " index: {i}")
                 except Exception as exc:
@@ -595,14 +613,15 @@
                         task_loading["errors"].append(error)
         elif k == "handlers":
             if not isinstance(v, list):
                 continue
             task_blocks, _ = get_task_blocks(task_dict_list=v)
             if task_blocks is None:
                 continue
+            last_task_line_num = -1
             for task_dict in task_blocks:
                 i = task_count
                 task_loading["total"] += 1
                 error = None
                 try:
                     t = load_task(
                         path=path,
@@ -611,19 +630,22 @@
                         role_name=role_name,
                         collection_name=collection_name,
                         collections_in_play=collections_in_play,
                         play_index=index,
                         parent_key=pbObj.key,
                         parent_local_key=pbObj.local_key,
                         yaml_lines=yaml_lines,
+                        previous_task_line=last_task_line_num,
                         basedir=basedir,
                     )
                     handlers.append(t)
                     if t:
                         task_loading["success"] += 1
+                        if t.line_num_in_file and len(t.line_num_in_file) == 2:
+                            last_task_line_num = t.line_num_in_file[1]
                 except TaskFormatError as exc:
                     error = exc
                     if skip_task_format_error:
                         logger.debug("this task is wrong format; skip the task in {}," " index: {}; skip this".format(path, i))
                     else:
                         raise TaskFormatError(f"this task is wrong format; skip the task in {path}," " index: {i}")
                 except Exception as exc:
@@ -1430,14 +1452,15 @@
     role_name="",
     collection_name="",
     collections_in_play=[],
     play_index=-1,
     parent_key="",
     parent_local_key="",
     yaml_lines="",
+    previous_task_line=-1,
     basedir="",
 ):
 
     taskObj = Task()
     fullpath = ""
     if yaml_lines:
         fullpath = path
@@ -1471,14 +1494,15 @@
     taskObj.set_yaml_lines(
         fullpath=fullpath,
         yaml_lines=yaml_lines,
         task_name=task_name,
         module_name=module_name,
         module_options=module_options,
         task_options=task_options,
+        previous_task_line=previous_task_line,
     )
 
     # module_options can be passed as a string like below
     #
     # - name: sample of string module options
     #   ufw: port={{ item }} proto=tcp rule=allow
     #   with_items:
@@ -1632,32 +1656,36 @@
     tasks = []
     task_loading = {
         "total": 0,
         "success": 0,
         "failure": 0,
         "errors": [],
     }
+    last_task_line_num = -1
     for i, t_dict in enumerate(task_dicts):
         task_loading["total"] += 1
         error = None
         try:
             t = load_task(
                 fullpath,
                 i,
                 t_dict,
                 role_name,
                 collection_name,
                 yaml_lines=yaml_lines,
                 parent_key=tfObj.key,
                 parent_local_key=tfObj.local_key,
+                previous_task_line=last_task_line_num,
                 basedir=basedir,
             )
             tasks.append(t)
             if t:
                 task_loading["success"] += 1
+                if t.line_num_in_file and len(t.line_num_in_file) == 2:
+                    last_task_line_num = t.line_num_in_file[1]
         except TaskFormatError as exc:
             error = exc
             if skip_task_format_error:
                 logger.debug("this task is wrong format; skip the task in {}, index: {}; skip this".format(fullpath, i))
                 continue
             else:
                 raise TaskFormatError(f"Task format error found; {fullpath}, index: {i}")
```

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/models.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from collections.abc import Callable
 from tabulate import tabulate
 from ruamel.yaml.scalarstring import DoubleQuotedScalarString
 
 from copy import deepcopy
 import json
 import jsonpickle
-import Levenshtein
+from rapidfuzz.distance import Levenshtein
 import ansible_risk_insight.yaml as ariyaml
 from ansible.module_utils.parsing.convert_bool import boolean
 from .keyutil import (
     set_collection_key,
     set_module_key,
     set_play_key,
     set_playbook_key,
@@ -1106,15 +1106,15 @@
     # candidates of resovled_name
     possible_candidates: list = field(default_factory=list)
 
     # embed these data when module/role/taskfile are resolved
     module_info: dict = field(default_factory=dict)
     include_info: dict = field(default_factory=dict)
 
-    def set_yaml_lines(self, fullpath="", yaml_lines="", task_name="", module_name="", module_options=None, task_options=None):
+    def set_yaml_lines(self, fullpath="", yaml_lines="", task_name="", module_name="", module_options=None, task_options=None, previous_task_line=-1):
         if not task_name and not module_options:
             return
 
         lines = []
         if yaml_lines:
             lines = yaml_lines.splitlines()
         else:
@@ -1123,14 +1123,20 @@
         # search candidates that match either of the following conditions
         #   - task name is included in the line
         #   - if module name is included,
         #       - if module option is string, it is included
         #       - if module option is dict, at least one key is included
         candidate_line_nums = []
         for i, line in enumerate(lines):
+
+            # skip lines until `previous_task_line` if provided
+            if previous_task_line > 0:
+                if i <= previous_task_line - 1:
+                    continue
+
             if task_name:
                 if task_name in line:
                     candidate_line_nums.append(i)
             elif "{}:".format(module_name) in line:
                 if isinstance(module_options, str):
                     if module_options in line:
                         candidate_line_nums.append(i)
```

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/parser.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/parser.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/ram_generator.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/ram_generator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/risk_assessment_model.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/risk_assessment_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,15 +433,19 @@
 
                     # but if a non-deprecated one is found, use it
                     if possible_index["fqcn"] == name and not possible_index["deprecated"]:
                         found_index = possible_index
 
             # if any candidates don't match with FQCN, use the first index
             if not found_index:
-                found_index = self.module_index[short_name][0]
+                non_deprecated_cands = [idx for idx in self.module_index[short_name] if not idx["deprecated"]]
+                if non_deprecated_cands:
+                    found_index = non_deprecated_cands[0]
+                else:
+                    found_index = self.module_index[short_name][0]
 
         modules_json_list = []
         if from_indices:
             _type = found_index.get("type", "")
             _name = found_index.get("name", "")
             _version = found_index.get("version", "")
             _hash = found_index.get("hash", "")
```

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/risk_detector.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/risk_detector.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/P001_module_name_validation.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/P001_module_name_validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,22 +73,28 @@
                 correct_fqcn = suggested_fqcns[0]
 
             if correct_fqcn != task.spec.module or not_exist:
                 need_correction = True
 
         # include_role, import_role
         elif task.spec.executable_type == ExecutableType.ROLE_TYPE:
-            if "ansible.builtin." not in task.spec.module:
+            if "ansible.builtin." in task.spec.module:
+                resolved_fqcn = task.spec.module
+                correct_fqcn = resolved_fqcn
+            else:
                 resolved_fqcn = "ansible.builtin." + task.spec.module
                 correct_fqcn = resolved_fqcn
                 need_correction = True
 
         # include_tasks, import_tasks
         elif task.spec.executable_type == ExecutableType.TASKFILE_TYPE:
-            if "ansible.builtin." not in task.spec.module:
+            if "ansible.builtin." in task.spec.module:
+                resolved_fqcn = task.spec.module
+                correct_fqcn = resolved_fqcn
+            else:
                 resolved_fqcn = "ansible.builtin." + task.spec.module
                 correct_fqcn = resolved_fqcn
                 need_correction = True
 
         module_examples = ""
         if task.module:
             module_examples = task.module.examples
```

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/P002_module_argument_key_validation.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/P002_module_argument_key_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/P003_module_argument_value_validation.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/P003_module_argument_value_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/P004_variable_validation.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/P004_variable_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R101_command_exec.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R101_command_exec.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R102_command_instead_of_shell.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R102_command_instead_of_shell.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R103_download_exec.md` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R103_download_exec.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R103_download_exec.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R103_download_exec.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R104_unauthorized_download_src.md` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R104_unauthorized_download_src.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R104_unauthorized_download_src.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R104_unauthorized_download_src.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R105_outbound_transfer.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R105_outbound_transfer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R106_inbound_transfer.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R106_inbound_transfer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R108_privilege_escalation.md` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R108_privilege_escalation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R108_privilege_escalation.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R108_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R109_key_config_change.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R109_key_config_change.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R110_non_builtin_use.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R110_non_builtin_use.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R111_parameterized_import_role.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R111_parameterized_import_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R113_parameterized_pkg_install.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R113_parameterized_pkg_install.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R114_file_change.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R114_file_change.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R115_file_deletion.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R115_file_deletion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R116_insecure_file_permission.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R116_insecure_file_permission.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R117_external_role.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R117_external_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R201_changed_data_dependence.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R201_changed_data_dependence.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R202_unconditional_override.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R202_unconditional_override.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R203_unused_override.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R203_unused_override.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R204_unnecessary_set_fact.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R204_unnecessary_set_fact.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R205_unnecessary_include_vars.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R205_unnecessary_include_vars.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R301_non_fqcn_use.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R301_non_fqcn_use.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R302_role_without_metadata.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R302_role_without_metadata.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R303_task_without_name.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R303_task_without_name.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R304_unresolved_module.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R304_unresolved_module.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R305_unresolved_role.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R305_unresolved_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R306_undefined_variable.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R306_undefined_variable.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R401_list_all_inbound_src.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R401_list_all_inbound_src.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R402_list_all_used_variables.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R402_list_all_used_variables.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R404_show_variables.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R404_show_variables.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/R501_dependency_suggestion.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R501_dependency_suggestion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/__init__.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/rule_versions.json` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/rule_versions.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/rules/sample_rule.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/sample_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/safe_glob.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/safe_glob.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/scanner.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/scanner.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/tree.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     TaskCall,
     PlayCall,
     RoleCall,
     call_obj_from_spec,
 )
 from .model_loader import load_builtin_modules
 from .risk_assessment_model import RAMClient
-from .variable_manager import VariableManager
 
 
 obj_type_dict = {
     "playbook": "playbooks",
     "play": "plays",
     "role": "roles",
     "taskfile": "taskfiles",
@@ -462,16 +461,14 @@
             self.taskfile_mappings = [tf for tf in self.taskfile_mappings if tf[0] == target_taskfile_path]
             self.playbook_mappings = []
             self.role_mappings = []
 
         # TODO: dependency check, especially for
         # collection dependencies for role
 
-        self.var_manager: VariableManager = VariableManager()
-
         self.target_playbook_path = target_playbook_path
         self.load_all_taskfiles = load_all_taskfiles
 
         self.module_resolve_cache = {}
         self.role_resolve_cache = {}
         self.taskfile_resolve_cache = {}
```

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/utils.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/utils.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight/yaml.py` & `ansible-risk-insight-0.2.5/ansible_risk_insight/yaml.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/ansible_risk_insight.egg-info/SOURCES.txt` & `ansible-risk-insight-0.2.5/ansible_risk_insight.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 ansible_risk_insight/risk_assessment_model.py
 ansible_risk_insight/risk_detector.py
 ansible_risk_insight/safe_glob.py
 ansible_risk_insight/scanner.py
 ansible_risk_insight/task_keywords.txt
 ansible_risk_insight/tree.py
 ansible_risk_insight/utils.py
-ansible_risk_insight/variable_manager.py
 ansible_risk_insight/yaml.py
 ansible_risk_insight.egg-info/PKG-INFO
 ansible_risk_insight.egg-info/SOURCES.txt
 ansible_risk_insight.egg-info/dependency_links.txt
 ansible_risk_insight.egg-info/entry_points.txt
 ansible_risk_insight.egg-info/requires.txt
 ansible_risk_insight.egg-info/top_level.txt
```

### Comparing `ansible-risk-insight-0.2.4/data-struct.txt` & `ansible-risk-insight-0.2.5/data-struct.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/doc/images/ari-apply-rules.png` & `ansible-risk-insight-0.2.5/doc/images/ari-apply-rules.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/doc/images/ari-arch.png` & `ansible-risk-insight-0.2.5/doc/images/ari-arch.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/doc/images/ari-overview.png` & `ansible-risk-insight-0.2.5/doc/images/ari-overview.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/doc/images/ari-ram-list.png` & `ansible-risk-insight-0.2.5/doc/images/ari-ram-list.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/docs/annotation.md` & `ansible-risk-insight-0.2.5/docs/annotation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/docs/customize_rules.md` & `ansible-risk-insight-0.2.5/docs/customize_rules.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/docs/rules/R103_download_exec.md` & `ansible-risk-insight-0.2.5/docs/rules/R103_download_exec.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/docs/rules/R104_unauthorized_download_src.md` & `ansible-risk-insight-0.2.5/docs/rules/R104_unauthorized_download_src.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/docs/rules/R107_pkg_install_with_insecure_option.md` & `ansible-risk-insight-0.2.5/docs/rules/R107_pkg_install_with_insecure_option.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/docs/rules/R108_privilege_escalation.md` & `ansible-risk-insight-0.2.5/docs/rules/R108_privilege_escalation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/example/readme.md` & `ansible-risk-insight-0.2.5/example/readme.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/example/rules/sample_rule.py` & `ansible-risk-insight-0.2.5/example/rules/sample_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/example/sample.py` & `ansible-risk-insight-0.2.5/example/sample.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/mkdocs.yml` & `ansible-risk-insight-0.2.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/pyproject.toml` & `ansible-risk-insight-0.2.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -10,25 +10,24 @@
 keywords = ["one", "two"]
 license = {text = "Apache License 2.0"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "gitdb",
-    "pygit2",
     "joblib",
     "jsonpickle",
     "PyYAML",
     "smmap",
     "tabulate",
     "requests",
-    "ansible",
+    "ansible-core",
     "ruamel.yaml",
     "filelock",
-    "Levenshtein",
+    "rapidfuzz",
 ]
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = {attr = "ansible_risk_insight._version.__version__"}
 
 [project.scripts]
```

### Comparing `ansible-risk-insight-0.2.4/scripts/gen_ram_slim.py` & `ansible-risk-insight-0.2.5/scripts/gen_ram_slim.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/scripts/gen_ram_subset.py` & `ansible-risk-insight-0.2.5/scripts/gen_ram_subset.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/test/test_scanner.py` & `ansible-risk-insight-0.2.5/test/test_scanner.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/test/testdata/projects/my.collection/MANIFEST.json` & `ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/MANIFEST.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.4/tox.ini` & `ansible-risk-insight-0.2.5/tox.ini`

 * *Files identical despite different names*

