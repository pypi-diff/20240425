# Comparing `tmp/bsl-appcli-2.5.0.tar.gz` & `tmp/bsl_appcli-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsl-appcli-2.5.0.tar", last modified: Thu Jan 11 03:00:48 2024, max compression
+gzip compressed data, was "bsl_appcli-3.0.0.tar", last modified: Wed Apr 24 22:39:04 2024, max compression
```

## Comparing `bsl-appcli-2.5.0.tar` & `bsl_appcli-3.0.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.044807 bsl-appcli-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    37532 2024-01-11 03:00:48.044807 bsl-appcli-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    37173 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.036807 bsl-appcli-2.5.0/appcli/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.036807 bsl-appcli-2.5.0/appcli/backup_manager/
--rw-r--r--   0 runner    (1001) docker     (127)    22873 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/backup_manager/backup_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/backup_manager/remote_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    18065 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/cli_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.036807 bsl-appcli-2.5.0/appcli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/commands/appcli_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/commands/backup_manager_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    10480 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/commands/configure_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/commands/configure_template_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/commands/debug_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/commands/encrypt_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/commands/init_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/commands/install_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/commands/launcher_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/commands/migrate_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/commands/service_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/commands/task_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/commands/version_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.036807 bsl-appcli-2.5.0/appcli/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/common/data_class_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.036807 bsl-appcli-2.5.0/appcli/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/configuration/configuration_dir_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    29099 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/configuration_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.036807 bsl-appcli-2.5.0/appcli/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/crypto/cipher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/crypto/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/dev_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.036807 bsl-appcli-2.5.0/appcli/git_repositories/
--rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/git_repositories/git_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)     9981 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/keycloak_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.040807 bsl-appcli-2.5.0/appcli/models/
--rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/models/cli_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     9440 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/models/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    31161 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/orchestrators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/string_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.040807 bsl-appcli-2.5.0/appcli/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/templates/installer.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/templates/launcher.j2
--rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/appcli/variables_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.040807 bsl-appcli-2.5.0/bsl_appcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    37532 2024-01-11 03:00:47.000000 bsl-appcli-2.5.0/bsl_appcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-01-11 03:00:48.000000 bsl-appcli-2.5.0/bsl_appcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 03:00:47.000000 bsl-appcli-2.5.0/bsl_appcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-01-11 03:00:47.000000 bsl-appcli-2.5.0/bsl_appcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-11 03:00:47.000000 bsl-appcli-2.5.0/bsl_appcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-11 03:00:48.044807 bsl-appcli-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.032807 bsl-appcli-2.5.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.040807 bsl-appcli-2.5.0/tests/backup_manager/
--rw-r--r--   0 runner    (1001) docker     (127)    36566 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/tests/backup_manager/test_backup_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.040807 bsl-appcli-2.5.0/tests/cipher/
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/tests/cipher/test_cipher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.040807 bsl-appcli-2.5.0/tests/commands/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.032807 bsl-appcli-2.5.0/tests/commands/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.032807 bsl-appcli-2.5.0/tests/commands/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.032807 bsl-appcli-2.5.0/tests/commands/resources/templates/baseline/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.040807 bsl-appcli-2.5.0/tests/commands/resources/templates/baseline/nesting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/tests/commands/resources/templates/baseline/nesting/nested_baseline_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/tests/commands/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/tests/commands/test_install_script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.040807 bsl-appcli-2.5.0/tests/commands_task/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.032807 bsl-appcli-2.5.0/tests/commands_task/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.032807 bsl-appcli-2.5.0/tests/commands_task/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.032807 bsl-appcli-2.5.0/tests/commands_task/resources/templates/baseline/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.040807 bsl-appcli-2.5.0/tests/commands_task/resources/templates/baseline/nesting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/tests/commands_task/resources/templates/baseline/nesting/nested_baseline_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/tests/commands_task/test_commands_task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.040807 bsl-appcli-2.5.0/tests/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/tests/configuration/test_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.040807 bsl-appcli-2.5.0/tests/configuration_manager/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.032807 bsl-appcli-2.5.0/tests/configuration_manager/expected_generated/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.040807 bsl-appcli-2.5.0/tests/configuration_manager/expected_generated/nesting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/tests/configuration_manager/expected_generated/nesting/nested_baseline_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.032807 bsl-appcli-2.5.0/tests/configuration_manager/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.032807 bsl-appcli-2.5.0/tests/configuration_manager/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.032807 bsl-appcli-2.5.0/tests/configuration_manager/resources/templates/baseline/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.040807 bsl-appcli-2.5.0/tests/configuration_manager/resources/templates/baseline/nesting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/tests/configuration_manager/resources/templates/baseline/nesting/nested_baseline_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    12006 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/tests/configuration_manager/test_configuration_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.040807 bsl-appcli-2.5.0/tests/configuration_state/
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/tests/configuration_state/test_configuration_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.040807 bsl-appcli-2.5.0/tests/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/tests/crypto/test_crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.040807 bsl-appcli-2.5.0/tests/git_repositories/
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/tests/git_repositories/test_git_repositories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.040807 bsl-appcli-2.5.0/tests/string_transformer/
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/tests/string_transformer/test_string_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.040807 bsl-appcli-2.5.0/tests/variables_manager/
--rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/tests/variables_manager/test_variables_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 03:00:48.044807 bsl-appcli-2.5.0/tests/version/
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-01-11 03:00:04.000000 bsl-appcli-2.5.0/tests/version/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.974914 bsl_appcli-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    38553 2024-04-24 22:39:04.974914 bsl_appcli-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    37519 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.966914 bsl_appcli-3.0.0/appcli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.966914 bsl_appcli-3.0.0/appcli/backup_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)    22873 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/backup_manager/backup_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/backup_manager/remote_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18065 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/cli_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.966914 bsl_appcli-3.0.0/appcli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/appcli_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/backup_manager_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10479 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/configure_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/configure_template_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/debug_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/encrypt_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/init_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/install_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/launcher_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/migrate_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10272 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/service_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/task_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/version_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.966914 bsl_appcli-3.0.0/appcli/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/common/data_class_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.966914 bsl_appcli-3.0.0/appcli/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/configuration/configuration_dir_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29934 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/configuration_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/appcli/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/crypto/cipher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/crypto/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/dev_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/appcli/git_repositories/
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/git_repositories/git_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/keycloak_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/appcli/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/models/cli_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9440 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/models/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31161 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/orchestrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/string_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/appcli/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/templates/installer.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/templates/launcher.j2
+-rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/variables_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.974914 bsl_appcli-3.0.0/bsl_appcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    38553 2024-04-24 22:39:04.000000 bsl_appcli-3.0.0/bsl_appcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-24 22:39:04.000000 bsl_appcli-3.0.0/bsl_appcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 22:39:04.000000 bsl_appcli-3.0.0/bsl_appcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-24 22:39:04.000000 bsl_appcli-3.0.0/bsl_appcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 22:39:04.000000 bsl_appcli-3.0.0/bsl_appcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 22:39:04.974914 bsl_appcli-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.962914 bsl_appcli-3.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/backup_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)    36565 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/backup_manager/test_backup_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/cipher/
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/cipher/test_cipher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/commands/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.962914 bsl_appcli-3.0.0/tests/commands/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.962914 bsl_appcli-3.0.0/tests/commands/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.962914 bsl_appcli-3.0.0/tests/commands/resources/templates/baseline/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/commands/resources/templates/baseline/nesting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/commands/resources/templates/baseline/nesting/nested_baseline_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/commands/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/commands/test_install_script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/commands_task/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.962914 bsl_appcli-3.0.0/tests/commands_task/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.962914 bsl_appcli-3.0.0/tests/commands_task/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.962914 bsl_appcli-3.0.0/tests/commands_task/resources/templates/baseline/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/commands_task/resources/templates/baseline/nesting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/commands_task/resources/templates/baseline/nesting/nested_baseline_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/commands_task/test_commands_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/configuration/test_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/configuration_manager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.962914 bsl_appcli-3.0.0/tests/configuration_manager/expected_generated/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/configuration_manager/expected_generated/nesting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/configuration_manager/expected_generated/nesting/nested_baseline_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.962914 bsl_appcli-3.0.0/tests/configuration_manager/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.962914 bsl_appcli-3.0.0/tests/configuration_manager/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.962914 bsl_appcli-3.0.0/tests/configuration_manager/resources/templates/baseline/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/configuration_manager/resources/templates/baseline/nesting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/configuration_manager/resources/templates/baseline/nesting/nested_baseline_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12006 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/configuration_manager/test_configuration_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/configuration_state/
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/configuration_state/test_configuration_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/crypto/test_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.974914 bsl_appcli-3.0.0/tests/git_repositories/
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/git_repositories/test_git_repositories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.974914 bsl_appcli-3.0.0/tests/string_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/string_transformer/test_string_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.974914 bsl_appcli-3.0.0/tests/variables_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/variables_manager/test_variables_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.974914 bsl_appcli-3.0.0/tests/version/
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/version/test_version.py
```

### Comparing `bsl-appcli-2.5.0/LICENSE` & `bsl_appcli-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/PKG-INFO` & `bsl_appcli-3.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: bsl-appcli
-Version: 2.5.0
-Summary: A library for adding CLI interfaces to applications in the brightSPARK Labs style
-Home-page: https://www.brightsparklabs.com
-Author: brightSPARK Labs
-Author-email: enquire@brightsparklabs.com
-License: MIT License
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # BSL Application CLI Library
 
 [![PyPI version](https://badge.fury.io/py/bsl-appcli.svg)](https://badge.fury.io/py/bsl-appcli)
 ![Test Python](https://github.com/brightsparklabs/appcli/actions/workflows/build_python.yml/badge.svg)
 
 A library for adding CLI interfaces to applications in the brightSPARK Labs style.
 
@@ -255,21 +243,32 @@
 # resources/templates/configurable/my-config.yml
 foobar: 5
 ```
 
 ```json
 # resources/templates/configurable/my-config.yml.schema.json
 {
+    "$schema": "http://json-schema.org/schema",
     "type": "object",
     "properties" : {
         "foobar" : {"type": "number"}
     }
 }
 ```
 
+To stop a schema file from being copied across to the `generated` config directory, add `.appcli` as an infix.
+
+```bash
+$ ls -1
+bar.json                     # -> Config-file ; Copy-on-apply
+bar.json.schema.json         # -> Schema-file ; Copy-on-apply
+foo.yaml                     # -> Config-file ; Copy-on-apply
+foo.yaml.appcli.schema.json  # -> Schema-file ; Ignore-on-apply
+```
+
 #### Application context files
 
 Template files are templated with Jinja2. The 'data' passed into the templating engine
 is a combination of the `settings.yml` and all application context files
 (stored in `resources/templates/appcli/context`, and referenced in the `Configuration`
 object as `application_context_files_dir`). Application context files that have the
 extension `.j2` are templated using the settings from `settings.yml`.
@@ -422,15 +421,15 @@
             conf_dir:
               include_list:
               exclude_list:
                 - "**/*"
         frequency: "* * *"
         remote_backups:
 
-#### Freqency
+#### Frequency
 
 Appcli supports limiting individual backups to run on only specific days using a cron-like frequency
 filter.
 
 When the `backup` command is run, each backup strategy will check if the `frequency` pattern matches
 today's date. Only strategies whose `frequency` pattern match today's date will execute.
 
@@ -858,31 +857,32 @@
     make test
 
 ## Usage while developing your CLI application
 
 While developing, it may be preferable to run your python script directly rather than having to
 rebuild a container each time you update it.
 
+NOTE: The following assumes your app name uppercase slug is `MYAPP`.
+
 - Ensure docker is installed (more specifically a docker socket at `/var/run/docker.sock`).
 - Set the environment variables which the CLI usually sets for you:
 
+        export MYAPP_DEV_MODE=true
+
+        # The above is equivalent to:
         export \
-            MYAPP_DATA_DIR=/tmp/myapp/data \
-            MYAPP_CONFIG_DIR=/tmp/myapp/config \
-            MYAPP_GENERATED_CONFIG_DIR=/tmp/myapp/config/.generated \
-            MYAPP_BACKUP_DIR=/tmp/myapp/backup \
-            MYAPP_ENVIRONMENT=dev
+            MYAPP_CLI_DEBUG=true \
+            MYAPP_DATA_DIR=/tmp/myapp/local-dev/data \
+            MYAPP_CONFIG_DIR=/tmp/myapp/local-dev/config \
+            MYAPP_BACKUP_DIR=/tmp/myapp/local-dev/backup \
+            MYAPP_ENVIRONMENT=local-dev
+
 - Run your CLI application:
 
-        ./src/myapp.py \
-              --debug \
-              --configuration-dir "${MYAPP_CONFIG_DIR}" \
-              --data-dir "${MYAPP_DATA_DIR}" \
-              --backup-dir "${MYAPP_BACKUP_DIR}" \
-              --environment "${MYAPP_ENVIRONMENT}
+        ./src/myapp.py
 
 ## Contributing
 
 When committing code, call `make all` to automatically run code formatting/ linting/testing.
 
 Appcli uses the python code formatter [black](https://pypi.org/project/black/) with default
 settings. This ensures that PR diffs are minimal and focussed on the code change rather than
```

### Comparing `bsl-appcli-2.5.0/README.md` & `bsl_appcli-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: bsl-appcli
+Version: 3.0.0
+Summary: A library for adding CLI interfaces to applications in the brightSPARK Labs style
+Home-page: https://www.brightsparklabs.com
+Author: brightSPARK Labs
+Author-email: enquire@brightsparklabs.com
+License: MIT License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: boto3==1.34.91
+Requires-Dist: click==8.1.7
+Requires-Dist: coloredlogs==15.0.1
+Requires-Dist: cronex==0.1.3.1
+Requires-Dist: dataclasses-json==0.5.7
+Requires-Dist: deepdiff==6.7.1
+Requires-Dist: GitPython==3.1.43
+Requires-Dist: jsonschema==4.21.1
+Requires-Dist: jinja2==3.1.3
+Requires-Dist: pycryptodome==3.20.0
+Requires-Dist: pydantic==2.7.1
+Requires-Dist: pyfiglet==1.0.2
+Requires-Dist: python-keycloak==3.12.0
+Requires-Dist: python-slugify==8.0.4
+Requires-Dist: ruamel-yaml==0.18.6
+Requires-Dist: tabulate==0.9.0
+Requires-Dist: wheel==0.43.0
+Provides-Extra: dev
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+
 # BSL Application CLI Library
 
 [![PyPI version](https://badge.fury.io/py/bsl-appcli.svg)](https://badge.fury.io/py/bsl-appcli)
 ![Test Python](https://github.com/brightsparklabs/appcli/actions/workflows/build_python.yml/badge.svg)
 
 A library for adding CLI interfaces to applications in the brightSPARK Labs style.
 
@@ -243,21 +275,32 @@
 # resources/templates/configurable/my-config.yml
 foobar: 5
 ```
 
 ```json
 # resources/templates/configurable/my-config.yml.schema.json
 {
+    "$schema": "http://json-schema.org/schema",
     "type": "object",
     "properties" : {
         "foobar" : {"type": "number"}
     }
 }
 ```
 
+To stop a schema file from being copied across to the `generated` config directory, add `.appcli` as an infix.
+
+```bash
+$ ls -1
+bar.json                     # -> Config-file ; Copy-on-apply
+bar.json.schema.json         # -> Schema-file ; Copy-on-apply
+foo.yaml                     # -> Config-file ; Copy-on-apply
+foo.yaml.appcli.schema.json  # -> Schema-file ; Ignore-on-apply
+```
+
 #### Application context files
 
 Template files are templated with Jinja2. The 'data' passed into the templating engine
 is a combination of the `settings.yml` and all application context files
 (stored in `resources/templates/appcli/context`, and referenced in the `Configuration`
 object as `application_context_files_dir`). Application context files that have the
 extension `.j2` are templated using the settings from `settings.yml`.
@@ -410,15 +453,15 @@
             conf_dir:
               include_list:
               exclude_list:
                 - "**/*"
         frequency: "* * *"
         remote_backups:
 
-#### Freqency
+#### Frequency
 
 Appcli supports limiting individual backups to run on only specific days using a cron-like frequency
 filter.
 
 When the `backup` command is run, each backup strategy will check if the `frequency` pattern matches
 today's date. Only strategies whose `frequency` pattern match today's date will execute.
 
@@ -846,31 +889,32 @@
     make test
 
 ## Usage while developing your CLI application
 
 While developing, it may be preferable to run your python script directly rather than having to
 rebuild a container each time you update it.
 
+NOTE: The following assumes your app name uppercase slug is `MYAPP`.
+
 - Ensure docker is installed (more specifically a docker socket at `/var/run/docker.sock`).
 - Set the environment variables which the CLI usually sets for you:
 
+        export MYAPP_DEV_MODE=true
+
+        # The above is equivalent to:
         export \
-            MYAPP_DATA_DIR=/tmp/myapp/data \
-            MYAPP_CONFIG_DIR=/tmp/myapp/config \
-            MYAPP_GENERATED_CONFIG_DIR=/tmp/myapp/config/.generated \
-            MYAPP_BACKUP_DIR=/tmp/myapp/backup \
-            MYAPP_ENVIRONMENT=dev
+            MYAPP_CLI_DEBUG=true \
+            MYAPP_DATA_DIR=/tmp/myapp/local-dev/data \
+            MYAPP_CONFIG_DIR=/tmp/myapp/local-dev/config \
+            MYAPP_BACKUP_DIR=/tmp/myapp/local-dev/backup \
+            MYAPP_ENVIRONMENT=local-dev
+
 - Run your CLI application:
 
-        ./src/myapp.py \
-              --debug \
-              --configuration-dir "${MYAPP_CONFIG_DIR}" \
-              --data-dir "${MYAPP_DATA_DIR}" \
-              --backup-dir "${MYAPP_BACKUP_DIR}" \
-              --environment "${MYAPP_ENVIRONMENT}
+        ./src/myapp.py
 
 ## Contributing
 
 When committing code, call `make all` to automatically run code formatting/ linting/testing.
 
 Appcli uses the python code formatter [black](https://pypi.org/project/black/) with default
 settings. This ensures that PR diffs are minimal and focussed on the code change rather than
```

### Comparing `bsl-appcli-2.5.0/appcli/backup_manager/backup_manager.py` & `bsl_appcli-3.0.0/appcli/backup_manager/backup_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/backup_manager/remote_strategy.py` & `bsl_appcli-3.0.0/appcli/backup_manager/remote_strategy.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/cli_builder.py` & `bsl_appcli-3.0.0/appcli/cli_builder.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/commands/appcli_command.py` & `bsl_appcli-3.0.0/appcli/commands/appcli_command.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/commands/backup_manager_cli.py` & `bsl_appcli-3.0.0/appcli/commands/backup_manager_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/commands/configure_cli.py` & `bsl_appcli-3.0.0/appcli/commands/configure_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 Configures the system.
 ________________________________________________________________________________
 
 Created by brightSPARK Labs
 www.brightsparklabs.com
 """
 
-
 # standard library
 import difflib
 import subprocess
 
 # vendor libraries
 import click
 from click.core import Context
@@ -70,20 +69,14 @@
             print_header(f"Seeding configuration directory for {self.app_name}")
 
             # Run pre-hooks
             hooks = self.cli_configuration.hooks
             logger.debug("Running pre-configure init hook")
             hooks.pre_configure_init(ctx)
 
-            # Validate the configuration schema.
-            logger.debug("Validating configuration files")
-            ConfigurationManager(
-                cli_context, self.cli_configuration
-            ).validate_configuration()
-
             # Initialise configuration directory
             logger.debug("Initialising configuration directory")
             ConfigurationManager(
                 cli_context, self.cli_configuration
             ).initialise_configuration()
 
             # Run post-hooks
@@ -116,14 +109,20 @@
             )
 
             # Run pre-hooks
             hooks = self.cli_configuration.hooks
             logger.debug("Running pre-configure apply hook")
             hooks.pre_configure_apply(ctx)
 
+            # Validate the configuration schema.
+            logger.debug("Validating configuration files")
+            ConfigurationManager(
+                cli_context, self.cli_configuration
+            ).validate_configuration()
+
             # Apply changes
             logger.debug("Applying configuration")
             ConfigurationManager(
                 cli_context, self.cli_configuration
             ).apply_configuration_changes(message)
 
             # Run post-hooks
```

### Comparing `bsl-appcli-2.5.0/appcli/commands/configure_template_cli.py` & `bsl_appcli-3.0.0/appcli/commands/configure_template_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/commands/debug_cli.py` & `bsl_appcli-3.0.0/appcli/commands/debug_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/commands/encrypt_cli.py` & `bsl_appcli-3.0.0/appcli/commands/encrypt_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/commands/init_cli.py` & `bsl_appcli-3.0.0/appcli/commands/init_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/commands/install_cli.py` & `bsl_appcli-3.0.0/appcli/commands/install_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/commands/launcher_cli.py` & `bsl_appcli-3.0.0/appcli/commands/launcher_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/commands/migrate_cli.py` & `bsl_appcli-3.0.0/appcli/commands/migrate_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/commands/service_cli.py` & `bsl_appcli-3.0.0/appcli/commands/service_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 Commands for lifecycle management of application services.
 ________________________________________________________________________________
 
 Created by brightSPARK Labs
 www.brightsparklabs.com
 """
 
-
 # standard libraries
 from __future__ import annotations
 
 import enum
 import sys
 
 # vendor libraries
```

### Comparing `bsl-appcli-2.5.0/appcli/commands/task_cli.py` & `bsl_appcli-3.0.0/appcli/commands/task_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/commands/version_cli.py` & `bsl_appcli-3.0.0/appcli/commands/version_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/common/data_class_extensions.py` & `bsl_appcli-3.0.0/appcli/common/data_class_extensions.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/configuration/configuration_dir_state.py` & `bsl_appcli-3.0.0/appcli/configuration/configuration_dir_state.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/configuration_manager.py` & `bsl_appcli-3.0.0/appcli/configuration_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,44 +16,45 @@
 import tarfile
 import tempfile
 from datetime import datetime, timezone
 from pathlib import Path
 from typing import Iterable
 
 import jsonschema
-import yaml
+import ruamel.yaml
 
 # vendor libraries
 from jinja2 import StrictUndefined, Template
 
 # local libraries
 from appcli.crypto import crypto
 from appcli.crypto.crypto import decrypt_values_in_file
 from appcli.functions import error_and_exit, print_header
 from appcli.git_repositories.git_repositories import (
     ConfigurationGitRepository,
     GeneratedConfigurationGitRepository,
 )
 from appcli.logger import logger
-from appcli.models.cli_context import SCHEMA_SUFFIX, CliContext
+from appcli.models.cli_context import SCHEMA_SUFFIX, IGNORE_INFIX, CliContext
 from appcli.models.configuration import Configuration
 from appcli.variables_manager import VariablesManager
 
 # ------------------------------------------------------------------------------
 # CONSTANTS
 # ------------------------------------------------------------------------------
 
 METADATA_FILE_NAME = "metadata-configure-apply.json"
 """ Name of the file holding metadata from running a configure (relative to the generated configuration directory) """
 
+YAML_LOADER = ruamel.yaml.YAML()
 FILETYPE_LOADERS = {
     ".json": json.load,
     ".jsn": json.load,
-    ".yaml": yaml.safe_load,
-    ".yml": yaml.safe_load,
+    ".yaml": YAML_LOADER.load,
+    ".yml": YAML_LOADER.load,
 }
 """ The supported filetypes for the validator. """
 
 # ------------------------------------------------------------------------------
 # PUBLIC CLASSES
 # ------------------------------------------------------------------------------
 
@@ -77,27 +78,36 @@
         stack_settings_schema: Path = (
             self.cli_context.get_stack_configuration_file_schema()
         )
         overrides_dir: Path = self.cli_context.get_baseline_template_overrides_dir()
         templates_dir: Path = self.cli_context.get_configurable_templates_dir()
 
         # Parse the directories to get the schema files.
-        schema_files = []
+        schema_files: list[Path] = []
         if settings_schema.is_file():
             schema_files.append(settings_schema)
         if stack_settings_schema.is_file():
             schema_files.append(stack_settings_schema)
         schema_files.extend(overrides_dir.glob(f"**/*{SCHEMA_SUFFIX}"))
         schema_files.extend(templates_dir.glob(f"**/*{SCHEMA_SUFFIX}"))
 
         for schema_file in schema_files:
-            # Take out the `schema` suffix to get the original config file.
+            # Take out the `schema` suffix and `appcli` infix (if applicable) to get the original config file.
             # NOTE: As we only need to remove part of the suffix, it is easier to convert to string
-            # and just remove part of the substring.
-            config_file: Path = Path(str(schema_file).removesuffix(SCHEMA_SUFFIX))
+            # and just remove parts of the substring.
+            # We also want to fetch just the filename (and not the path) incase any parent directories
+            # have `.appcli` in them.
+            filename_string = schema_file.name
+            filename_string = filename_string.removesuffix(
+                SCHEMA_SUFFIX
+            )  # Remove schema suffix.
+            filename_string = filename_string.replace(
+                IGNORE_INFIX, ""
+            )  # Remove ignore infix.
+            config_file = schema_file.parent / filename_string
             if not config_file.exists():
                 logger.warning(f"Found {schema_file} but no matching config file.")
                 continue
 
             # Load and validate the config/schema.
             logger.debug(f"Found schema for {config_file}. Validating...")
             self.__validate_schema(config_file, schema_file)
@@ -432,23 +442,28 @@
             target_file = generated_configuration_dir.joinpath(relative_file)
 
             if template_file.is_dir():
                 logger.debug("Creating directory [%s] ...", target_file)
                 target_file.mkdir(parents=True, exist_ok=True)
                 continue
 
-            if template_file.suffix == ".j2":
+            # If its an appcli schema file we ignore it.
+            if f"{IGNORE_INFIX}." in template_file.name:
+                logger.debug("Ignoring appcli schema file [%s] ...", template_file)
+            # If its a j2 file we template and copy.
+            elif template_file.suffix == ".j2":
                 # parse jinja2 templates against configuration
                 target_file = target_file.with_suffix("")
                 logger.debug("Generating configuration file [%s] ...", target_file)
                 self.__generate_from_template(
                     template_file,
                     target_file,
                     template_data,
                 )
+            # If its a regular file we just copy it.
             else:
                 logger.debug("Copying configuration file to [%s] ...", target_file)
                 shutil.copy2(template_file, target_file)
 
     def __directory_is_not_empty(self, directory: Path) -> bool:
         """Checks if a directory is not empty.
```

### Comparing `bsl-appcli-2.5.0/appcli/crypto/cipher.py` & `bsl_appcli-3.0.0/appcli/crypto/cipher.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/crypto/crypto.py` & `bsl_appcli-3.0.0/appcli/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/dev_mode.py` & `bsl_appcli-3.0.0/appcli/dev_mode.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/functions.py` & `bsl_appcli-3.0.0/appcli/functions.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/git_repositories/git_repositories.py` & `bsl_appcli-3.0.0/appcli/git_repositories/git_repositories.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/keycloak_manager.py` & `bsl_appcli-3.0.0/appcli/keycloak_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -192,15 +192,15 @@
                 setting additional properties on the newly-created object.
         """
 
         kc = self.__get_keycloak_admin(realm_name)
         user_id = kc.get_user_id(username)
         all_realm_roles = kc.get_realm_roles()
         roles = [role for role in all_realm_roles if role["name"] == role_name]
-        kc.assign_realm_roles(user_id, None, roles)
+        kc.assign_realm_roles(user_id, roles)
 
     def configure_default(self, app_name_slug):
         """Applies the default opinionated configuration to Keycloak
 
         This does the following:
          - Creates a realm named '<app_name_slug>'
          - For realm '<app_name_slug>', creates a client with the name '<app_name_slug>', which has an audience mapper to itself,
@@ -222,15 +222,43 @@
                     "protocolMapper": "oidc-audience-mapper",
                     "consentRequired": "false",
                     "config": {
                         "included.client.audience": app_name_slug,
                         "id.token.claim": "false",
                         "access.token.claim": "true",
                     },
-                }
+                },
+                {
+                    "name": "realm roles",
+                    "protocol": "openid-connect",
+                    "protocolMapper": "oidc-usermodel-realm-role-mapper",
+                    "consentRequired": "false",
+                    "config": {
+                        "multivalued": "true",
+                        "id.token.claim": "true",
+                        "access.token.claim": "true",
+                        "userinfo.token.claim": "true",
+                        "claim.name": "realm_access.roles",
+                        "jsonType.label": "String",
+                    },
+                },
+                {
+                    "name": "client roles",
+                    "protocol": "openid-connect",
+                    "protocolMapper": "oidc-usermodel-client-role-mapper",
+                    "consentRequired": "false",
+                    "config": {
+                        "multivalued": "true",
+                        "id.token.claim": "true",
+                        "access.token.claim": "true",
+                        "userinfo.token.claim": "true",
+                        "claim.name": "resource_access.${client_id}.roles",
+                        "jsonType.label": "String",
+                    },
+                },
             ],
         }
         self.create_client(app_name_slug, app_name_slug, client_payload)
         secret = self.get_client_secret(app_name_slug, app_name_slug)
         logger.debug(f"Created client [{app_name_slug}] with secret [{secret}]")
 
         realm_role = f"{app_name_slug}-admin"
```

### Comparing `bsl-appcli-2.5.0/appcli/logger.py` & `bsl_appcli-3.0.0/appcli/logger.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/models/cli_context.py` & `bsl_appcli-3.0.0/appcli/models/cli_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 # ------------------------------------------------------------------------------
 # CONSTANTS
 # ------------------------------------------------------------------------------
 
 SCHEMA_SUFFIX = ".schema.json"
 """ The suffix for the validation schema files. """
 
+IGNORE_INFIX = ".appcli"
+""" An infix extension to ignore when copying schema files. """
+
 
 # ------------------------------------------------------------------------------
 # PUBLIC CLASSES
 # ------------------------------------------------------------------------------
 
 
 class CliContext(NamedTuple):
```

### Comparing `bsl-appcli-2.5.0/appcli/models/configuration.py` & `bsl_appcli-3.0.0/appcli/models/configuration.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/orchestrators.py` & `bsl_appcli-3.0.0/appcli/orchestrators.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/string_transformer.py` & `bsl_appcli-3.0.0/appcli/string_transformer.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/templates/installer.j2` & `bsl_appcli-3.0.0/appcli/templates/installer.j2`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/templates/launcher.j2` & `bsl_appcli-3.0.0/appcli/templates/launcher.j2`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/appcli/variables_manager.py` & `bsl_appcli-3.0.0/appcli/variables_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/bsl_appcli.egg-info/PKG-INFO` & `bsl_appcli-3.0.0/bsl_appcli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,38 @@
 Metadata-Version: 2.1
 Name: bsl-appcli
-Version: 2.5.0
+Version: 3.0.0
 Summary: A library for adding CLI interfaces to applications in the brightSPARK Labs style
 Home-page: https://www.brightsparklabs.com
 Author: brightSPARK Labs
 Author-email: enquire@brightsparklabs.com
 License: MIT License
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: boto3==1.34.91
+Requires-Dist: click==8.1.7
+Requires-Dist: coloredlogs==15.0.1
+Requires-Dist: cronex==0.1.3.1
+Requires-Dist: dataclasses-json==0.5.7
+Requires-Dist: deepdiff==6.7.1
+Requires-Dist: GitPython==3.1.43
+Requires-Dist: jsonschema==4.21.1
+Requires-Dist: jinja2==3.1.3
+Requires-Dist: pycryptodome==3.20.0
+Requires-Dist: pydantic==2.7.1
+Requires-Dist: pyfiglet==1.0.2
+Requires-Dist: python-keycloak==3.12.0
+Requires-Dist: python-slugify==8.0.4
+Requires-Dist: ruamel-yaml==0.18.6
+Requires-Dist: tabulate==0.9.0
+Requires-Dist: wheel==0.43.0
+Provides-Extra: dev
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 
 # BSL Application CLI Library
 
 [![PyPI version](https://badge.fury.io/py/bsl-appcli.svg)](https://badge.fury.io/py/bsl-appcli)
 ![Test Python](https://github.com/brightsparklabs/appcli/actions/workflows/build_python.yml/badge.svg)
 
 A library for adding CLI interfaces to applications in the brightSPARK Labs style.
@@ -255,21 +275,32 @@
 # resources/templates/configurable/my-config.yml
 foobar: 5
 ```
 
 ```json
 # resources/templates/configurable/my-config.yml.schema.json
 {
+    "$schema": "http://json-schema.org/schema",
     "type": "object",
     "properties" : {
         "foobar" : {"type": "number"}
     }
 }
 ```
 
+To stop a schema file from being copied across to the `generated` config directory, add `.appcli` as an infix.
+
+```bash
+$ ls -1
+bar.json                     # -> Config-file ; Copy-on-apply
+bar.json.schema.json         # -> Schema-file ; Copy-on-apply
+foo.yaml                     # -> Config-file ; Copy-on-apply
+foo.yaml.appcli.schema.json  # -> Schema-file ; Ignore-on-apply
+```
+
 #### Application context files
 
 Template files are templated with Jinja2. The 'data' passed into the templating engine
 is a combination of the `settings.yml` and all application context files
 (stored in `resources/templates/appcli/context`, and referenced in the `Configuration`
 object as `application_context_files_dir`). Application context files that have the
 extension `.j2` are templated using the settings from `settings.yml`.
@@ -422,15 +453,15 @@
             conf_dir:
               include_list:
               exclude_list:
                 - "**/*"
         frequency: "* * *"
         remote_backups:
 
-#### Freqency
+#### Frequency
 
 Appcli supports limiting individual backups to run on only specific days using a cron-like frequency
 filter.
 
 When the `backup` command is run, each backup strategy will check if the `frequency` pattern matches
 today's date. Only strategies whose `frequency` pattern match today's date will execute.
 
@@ -858,31 +889,32 @@
     make test
 
 ## Usage while developing your CLI application
 
 While developing, it may be preferable to run your python script directly rather than having to
 rebuild a container each time you update it.
 
+NOTE: The following assumes your app name uppercase slug is `MYAPP`.
+
 - Ensure docker is installed (more specifically a docker socket at `/var/run/docker.sock`).
 - Set the environment variables which the CLI usually sets for you:
 
+        export MYAPP_DEV_MODE=true
+
+        # The above is equivalent to:
         export \
-            MYAPP_DATA_DIR=/tmp/myapp/data \
-            MYAPP_CONFIG_DIR=/tmp/myapp/config \
-            MYAPP_GENERATED_CONFIG_DIR=/tmp/myapp/config/.generated \
-            MYAPP_BACKUP_DIR=/tmp/myapp/backup \
-            MYAPP_ENVIRONMENT=dev
+            MYAPP_CLI_DEBUG=true \
+            MYAPP_DATA_DIR=/tmp/myapp/local-dev/data \
+            MYAPP_CONFIG_DIR=/tmp/myapp/local-dev/config \
+            MYAPP_BACKUP_DIR=/tmp/myapp/local-dev/backup \
+            MYAPP_ENVIRONMENT=local-dev
+
 - Run your CLI application:
 
-        ./src/myapp.py \
-              --debug \
-              --configuration-dir "${MYAPP_CONFIG_DIR}" \
-              --data-dir "${MYAPP_DATA_DIR}" \
-              --backup-dir "${MYAPP_BACKUP_DIR}" \
-              --environment "${MYAPP_ENVIRONMENT}
+        ./src/myapp.py
 
 ## Contributing
 
 When committing code, call `make all` to automatically run code formatting/ linting/testing.
 
 Appcli uses the python code formatter [black](https://pypi.org/project/black/) with default
 settings. This ensures that PR diffs are minimal and focussed on the code change rather than
```

### Comparing `bsl-appcli-2.5.0/bsl_appcli.egg-info/SOURCES.txt` & `bsl_appcli-3.0.0/bsl_appcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/setup.py` & `bsl_appcli-3.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,28 +53,27 @@
     license="MIT License",
     author="brightSPARK Labs",
     author_email="enquire@brightsparklabs.com",
     url="https://www.brightsparklabs.com",
     packages=find_namespace_packages(exclude=["contrib", "docs", "tests"]),
     include_package_data=True,
     install_requires=[
-        "boto3==1.34.14",
+        "boto3==1.34.91",
         "click==8.1.7",
         "coloredlogs==15.0.1",
         "cronex==0.1.3.1",
         "dataclasses-json==0.5.7",
         "deepdiff==6.7.1",
-        "GitPython==3.1.41",
-        "jsonschema==4.20.0",
-        "jinja2==3.1.2",
-        "pre-commit==3.6.0",
-        "pycryptodome==3.19.1",
-        "pydantic==2.5.3",
+        "GitPython==3.1.43",
+        "jsonschema==4.21.1",
+        "jinja2==3.1.3",
+        "pycryptodome==3.20.0",
+        "pydantic==2.7.1",
         "pyfiglet==1.0.2",
-        "python-keycloak==0.22.0",
-        "python-slugify==8.0.1",
-        "ruamel-yaml==0.18.5",
+        "python-keycloak==3.12.0",
+        "python-slugify==8.0.4",
+        "ruamel-yaml==0.18.6",
         "tabulate==0.9.0",
-        "wheel==0.42.0",
+        "wheel==0.43.0",
     ],
-    extras_require={"dev": ["ruff", "pytest"]},
+    extras_require={"dev": ["ruff", "pre-commit", "pytest"]},
 )
```

### Comparing `bsl-appcli-2.5.0/tests/backup_manager/test_backup_manager.py` & `bsl_appcli-3.0.0/tests/backup_manager/test_backup_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 Unit tests for the backup manager.
 ________________________________________________________________________________
 
 Created by brightSPARK Labs
 www.brightsparklabs.com
 """
 
-
 # standard libraries
 import datetime
 import os
 import tarfile
 from pathlib import Path, PurePath
 
 # vendor libraries
```

### Comparing `bsl-appcli-2.5.0/tests/cipher/test_cipher.py` & `bsl_appcli-3.0.0/tests/cipher/test_cipher.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/tests/commands/test_commands.py` & `bsl_appcli-3.0.0/tests/commands/test_commands.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/tests/commands/test_install_script.py` & `bsl_appcli-3.0.0/tests/commands/test_install_script.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/tests/commands_task/test_commands_task.py` & `bsl_appcli-3.0.0/tests/commands_task/test_commands_task.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/tests/configuration/test_configuration.py` & `bsl_appcli-3.0.0/tests/configuration/test_configuration.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/tests/configuration_manager/test_configuration_manager.py` & `bsl_appcli-3.0.0/tests/configuration_manager/test_configuration_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/tests/configuration_state/test_configuration_state.py` & `bsl_appcli-3.0.0/tests/configuration_state/test_configuration_state.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/tests/crypto/test_crypto.py` & `bsl_appcli-3.0.0/tests/crypto/test_crypto.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/tests/git_repositories/test_git_repositories.py` & `bsl_appcli-3.0.0/tests/git_repositories/test_git_repositories.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/tests/string_transformer/test_string_transformer.py` & `bsl_appcli-3.0.0/tests/string_transformer/test_string_transformer.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/tests/variables_manager/test_variables_manager.py` & `bsl_appcli-3.0.0/tests/variables_manager/test_variables_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.5.0/tests/version/test_version.py` & `bsl_appcli-3.0.0/tests/version/test_version.py`

 * *Files identical despite different names*

