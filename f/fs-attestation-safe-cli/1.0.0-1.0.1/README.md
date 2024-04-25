# Comparing `tmp/fs_attestation_safe_cli-1.0.0.tar.gz` & `tmp/fs_attestation_safe_cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fs_attestation_safe_cli-1.0.0.tar", last modified: Wed Apr 24 08:08:28 2024, max compression
+gzip compressed data, was "fs_attestation_safe_cli-1.0.1.tar", last modified: Wed Apr 24 09:06:04 2024, max compression
```

## Comparing `fs_attestation_safe_cli-1.0.0.tar` & `fs_attestation_safe_cli-1.0.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:08:28.504926 fs_attestation_safe_cli-1.0.0/
--rw-r--r--   0 mohan      (501) staff       (20)     1082 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/LICENSE
--rw-r--r--   0 mohan      (501) staff       (20)     4051 2024-04-24 08:08:28.505065 fs_attestation_safe_cli-1.0.0/PKG-INFO
--rw-r--r--   0 mohan      (501) staff       (20)     3263 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/README.md
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:08:28.481144 fs_attestation_safe_cli-1.0.0/fs_attestation_safe_cli.egg-info/
--rw-r--r--   0 mohan      (501) staff       (20)     4051 2024-04-24 08:08:28.000000 fs_attestation_safe_cli-1.0.0/fs_attestation_safe_cli.egg-info/PKG-INFO
--rw-r--r--   0 mohan      (501) staff       (20)     1901 2024-04-24 08:08:28.000000 fs_attestation_safe_cli-1.0.0/fs_attestation_safe_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mohan      (501) staff       (20)        1 2024-04-24 08:08:28.000000 fs_attestation_safe_cli-1.0.0/fs_attestation_safe_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mohan      (501) staff       (20)       90 2024-04-24 08:08:28.000000 fs_attestation_safe_cli-1.0.0/fs_attestation_safe_cli.egg-info/entry_points.txt
--rw-r--r--   0 mohan      (501) staff       (20)      163 2024-04-24 08:08:28.000000 fs_attestation_safe_cli-1.0.0/fs_attestation_safe_cli.egg-info/requires.txt
--rw-r--r--   0 mohan      (501) staff       (20)       15 2024-04-24 08:08:28.000000 fs_attestation_safe_cli-1.0.0/fs_attestation_safe_cli.egg-info/top_level.txt
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:08:28.488154 fs_attestation_safe_cli-1.0.0/safe_cli/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     2085 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/argparse_validators.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:08:28.489448 fs_attestation_safe_cli-1.0.0/safe_cli/contracts/
--rw-r--r--   0 mohan      (501) staff       (20)       75 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/contracts/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)    28478 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/contracts/safe_to_l2_migration.py
--rw-r--r--   0 mohan      (501) staff       (20)     1262 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/ethereum_hd_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     5829 2024-04-24 04:24:09.000000 fs_attestation_safe_cli-1.0.0/safe_cli/main.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:08:28.492394 fs_attestation_safe_cli-1.0.0/safe_cli/operators/
--rw-r--r--   0 mohan      (501) staff       (20)      204 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/operators/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)       87 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/operators/enums.py
--rw-r--r--   0 mohan      (501) staff       (20)     1644 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/operators/exceptions.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:08:28.497086 fs_attestation_safe_cli-1.0.0/safe_cli/operators/hw_wallets/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/operators/hw_wallets/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)      113 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/operators/hw_wallets/constants.py
--rw-r--r--   0 mohan      (501) staff       (20)       98 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/operators/hw_wallets/exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)     1925 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/operators/hw_wallets/hw_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     7501 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/operators/hw_wallets/hw_wallet_manager.py
--rw-r--r--   0 mohan      (501) staff       (20)     1081 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/operators/hw_wallets/ledger_exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)     2555 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/operators/hw_wallets/ledger_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     1092 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/operators/hw_wallets/trezor_exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)     4527 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/operators/hw_wallets/trezor_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)    46527 2024-04-24 04:22:26.000000 fs_attestation_safe_cli-1.0.0/safe_cli/operators/safe_operator.py
--rw-r--r--   0 mohan      (501) staff       (20)    18731 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/operators/safe_tx_service_operator.py
--rw-r--r--   0 mohan      (501) staff       (20)    19504 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/prompt_parser.py
--rw-r--r--   0 mohan      (501) staff       (20)     4030 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/safe_addresses.py
--rw-r--r--   0 mohan      (501) staff       (20)     1824 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/safe_completer.py
--rw-r--r--   0 mohan      (501) staff       (20)     9529 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/safe_completer_constants.py
--rw-r--r--   0 mohan      (501) staff       (20)     7416 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/safe_creator.py
--rw-r--r--   0 mohan      (501) staff       (20)     1313 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/safe_lexer.py
--rw-r--r--   0 mohan      (501) staff       (20)     3329 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/utils.py
--rw-r--r--   0 mohan      (501) staff       (20)       18 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/safe_cli/version.py
--rw-r--r--   0 mohan      (501) staff       (20)      533 2024-04-24 08:08:28.505941 fs_attestation_safe_cli-1.0.0/setup.cfg
--rw-r--r--   0 mohan      (501) staff       (20)     1494 2024-04-24 08:07:50.000000 fs_attestation_safe_cli-1.0.0/setup.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:08:28.503380 fs_attestation_safe_cli-1.0.0/tests/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/tests/__init__.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:08:28.504705 fs_attestation_safe_cli-1.0.0/tests/mocks/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/tests/mocks/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     7755 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/tests/mocks/balances_mock.py
--rw-r--r--   0 mohan      (501) staff       (20)     2161 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/tests/mocks/data_decoded_mock.py
--rw-r--r--   0 mohan      (501) staff       (20)     2275 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/tests/mocks/multisig_tx_mock.py
--rw-r--r--   0 mohan      (501) staff       (20)     4217 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/tests/mocks/txs_mock.py
--rw-r--r--   0 mohan      (501) staff       (20)     1980 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/tests/safe_cli_test_case_mixin.py
--rw-r--r--   0 mohan      (501) staff       (20)     2335 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/tests/test_argparse_validators.py
--rw-r--r--   0 mohan      (501) staff       (20)     4030 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/tests/test_entrypoint.py
--rw-r--r--   0 mohan      (501) staff       (20)     2700 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/tests/test_ethereum_hd_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     8216 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/tests/test_hw_wallet_manager.py
--rw-r--r--   0 mohan      (501) staff       (20)     8870 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/tests/test_ledger_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     2309 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/tests/test_safe_addresses.py
--rw-r--r--   0 mohan      (501) staff       (20)     3051 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/tests/test_safe_cli.py
--rw-r--r--   0 mohan      (501) staff       (20)      753 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/tests/test_safe_completer.py
--rw-r--r--   0 mohan      (501) staff       (20)     1644 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/tests/test_safe_creator.py
--rw-r--r--   0 mohan      (501) staff       (20)      577 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/tests/test_safe_lexer.py
--rw-r--r--   0 mohan      (501) staff       (20)    21356 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/tests/test_safe_operator.py
--rw-r--r--   0 mohan      (501) staff       (20)    19108 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/tests/test_safe_tx_service_operator.py
--rw-r--r--   0 mohan      (501) staff       (20)     9113 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/tests/test_trezor_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     2050 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/tests/test_utils.py
--rw-r--r--   0 mohan      (501) staff       (20)     1172 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.0/tests/utils.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 09:06:04.030144 fs_attestation_safe_cli-1.0.1/
+-rw-r--r--   0 mohan      (501) staff       (20)     1082 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/LICENSE
+-rw-r--r--   0 mohan      (501) staff       (20)     4051 2024-04-24 09:06:04.030552 fs_attestation_safe_cli-1.0.1/PKG-INFO
+-rw-r--r--   0 mohan      (501) staff       (20)     3263 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/README.md
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 09:06:04.003965 fs_attestation_safe_cli-1.0.1/fs_attestation_safe_cli.egg-info/
+-rw-r--r--   0 mohan      (501) staff       (20)     4051 2024-04-24 09:06:03.000000 fs_attestation_safe_cli-1.0.1/fs_attestation_safe_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mohan      (501) staff       (20)     1901 2024-04-24 09:06:03.000000 fs_attestation_safe_cli-1.0.1/fs_attestation_safe_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mohan      (501) staff       (20)        1 2024-04-24 09:06:03.000000 fs_attestation_safe_cli-1.0.1/fs_attestation_safe_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mohan      (501) staff       (20)      105 2024-04-24 09:06:03.000000 fs_attestation_safe_cli-1.0.1/fs_attestation_safe_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mohan      (501) staff       (20)      163 2024-04-24 09:06:03.000000 fs_attestation_safe_cli-1.0.1/fs_attestation_safe_cli.egg-info/requires.txt
+-rw-r--r--   0 mohan      (501) staff       (20)       15 2024-04-24 09:06:03.000000 fs_attestation_safe_cli-1.0.1/fs_attestation_safe_cli.egg-info/top_level.txt
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 09:06:04.009324 fs_attestation_safe_cli-1.0.1/safe_cli/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2085 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/argparse_validators.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 09:06:04.010328 fs_attestation_safe_cli-1.0.1/safe_cli/contracts/
+-rw-r--r--   0 mohan      (501) staff       (20)       75 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/contracts/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)    28478 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/contracts/safe_to_l2_migration.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1262 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/ethereum_hd_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     5829 2024-04-24 04:24:09.000000 fs_attestation_safe_cli-1.0.1/safe_cli/main.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 09:06:04.012897 fs_attestation_safe_cli-1.0.1/safe_cli/operators/
+-rw-r--r--   0 mohan      (501) staff       (20)      204 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/operators/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)       87 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/operators/enums.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1644 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/operators/exceptions.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 09:06:04.018453 fs_attestation_safe_cli-1.0.1/safe_cli/operators/hw_wallets/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/operators/hw_wallets/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)      113 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/operators/hw_wallets/constants.py
+-rw-r--r--   0 mohan      (501) staff       (20)       98 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/operators/hw_wallets/exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1925 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/operators/hw_wallets/hw_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7501 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/operators/hw_wallets/hw_wallet_manager.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1081 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/operators/hw_wallets/ledger_exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2555 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/operators/hw_wallets/ledger_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1092 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/operators/hw_wallets/trezor_exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4527 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/operators/hw_wallets/trezor_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)    46527 2024-04-24 04:22:26.000000 fs_attestation_safe_cli-1.0.1/safe_cli/operators/safe_operator.py
+-rw-r--r--   0 mohan      (501) staff       (20)    18731 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/operators/safe_tx_service_operator.py
+-rw-r--r--   0 mohan      (501) staff       (20)    19504 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/prompt_parser.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4030 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/safe_addresses.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1824 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/safe_completer.py
+-rw-r--r--   0 mohan      (501) staff       (20)     9529 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/safe_completer_constants.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7416 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/safe_creator.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1313 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/safe_lexer.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3329 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/safe_cli/utils.py
+-rw-r--r--   0 mohan      (501) staff       (20)       18 2024-04-24 09:04:39.000000 fs_attestation_safe_cli-1.0.1/safe_cli/version.py
+-rw-r--r--   0 mohan      (501) staff       (20)      533 2024-04-24 09:06:04.031799 fs_attestation_safe_cli-1.0.1/setup.cfg
+-rw-r--r--   0 mohan      (501) staff       (20)     1509 2024-04-24 09:02:11.000000 fs_attestation_safe_cli-1.0.1/setup.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 09:06:04.027288 fs_attestation_safe_cli-1.0.1/tests/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/tests/__init__.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 09:06:04.029525 fs_attestation_safe_cli-1.0.1/tests/mocks/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/tests/mocks/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7755 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/tests/mocks/balances_mock.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2161 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/tests/mocks/data_decoded_mock.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2275 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/tests/mocks/multisig_tx_mock.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4217 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/tests/mocks/txs_mock.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1980 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/tests/safe_cli_test_case_mixin.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2335 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/tests/test_argparse_validators.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4030 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/tests/test_entrypoint.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2700 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/tests/test_ethereum_hd_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     8216 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/tests/test_hw_wallet_manager.py
+-rw-r--r--   0 mohan      (501) staff       (20)     8870 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/tests/test_ledger_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2309 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/tests/test_safe_addresses.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3051 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/tests/test_safe_cli.py
+-rw-r--r--   0 mohan      (501) staff       (20)      753 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/tests/test_safe_completer.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1644 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/tests/test_safe_creator.py
+-rw-r--r--   0 mohan      (501) staff       (20)      577 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/tests/test_safe_lexer.py
+-rw-r--r--   0 mohan      (501) staff       (20)    21356 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/tests/test_safe_operator.py
+-rw-r--r--   0 mohan      (501) staff       (20)    19108 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/tests/test_safe_tx_service_operator.py
+-rw-r--r--   0 mohan      (501) staff       (20)     9113 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/tests/test_trezor_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2050 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/tests/test_utils.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1172 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.1/tests/utils.py
```

### Comparing `fs_attestation_safe_cli-1.0.0/LICENSE` & `fs_attestation_safe_cli-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/PKG-INFO` & `fs_attestation_safe_cli-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fs_attestation_safe_cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: Modified Command Line Interface for Safe for FailSafe Attestation Service
 Home-page: https://github.com/gnosis/safe-cli
 Download-URL: https://github.com/gnosis/safe-cli/releases
 Author: Mohan
 Author-email: mohan@ethlas.com
 License: MIT
 Classifier: Programming Language :: Python
```

### Comparing `fs_attestation_safe_cli-1.0.0/README.md` & `fs_attestation_safe_cli-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/fs_attestation_safe_cli.egg-info/PKG-INFO` & `fs_attestation_safe_cli-1.0.1/fs_attestation_safe_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fs-attestation-safe-cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: Modified Command Line Interface for Safe for FailSafe Attestation Service
 Home-page: https://github.com/gnosis/safe-cli
 Download-URL: https://github.com/gnosis/safe-cli/releases
 Author: Mohan
 Author-email: mohan@ethlas.com
 License: MIT
 Classifier: Programming Language :: Python
```

### Comparing `fs_attestation_safe_cli-1.0.0/fs_attestation_safe_cli.egg-info/SOURCES.txt` & `fs_attestation_safe_cli-1.0.1/fs_attestation_safe_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/safe_cli/argparse_validators.py` & `fs_attestation_safe_cli-1.0.1/safe_cli/argparse_validators.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/safe_cli/contracts/safe_to_l2_migration.py` & `fs_attestation_safe_cli-1.0.1/safe_cli/contracts/safe_to_l2_migration.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/safe_cli/ethereum_hd_wallet.py` & `fs_attestation_safe_cli-1.0.1/safe_cli/ethereum_hd_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/safe_cli/main.py` & `fs_attestation_safe_cli-1.0.1/safe_cli/main.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/safe_cli/operators/exceptions.py` & `fs_attestation_safe_cli-1.0.1/safe_cli/operators/exceptions.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/safe_cli/operators/hw_wallets/hw_wallet.py` & `fs_attestation_safe_cli-1.0.1/safe_cli/operators/hw_wallets/hw_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/safe_cli/operators/hw_wallets/hw_wallet_manager.py` & `fs_attestation_safe_cli-1.0.1/safe_cli/operators/hw_wallets/hw_wallet_manager.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/safe_cli/operators/hw_wallets/ledger_exceptions.py` & `fs_attestation_safe_cli-1.0.1/safe_cli/operators/hw_wallets/ledger_exceptions.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/safe_cli/operators/hw_wallets/ledger_wallet.py` & `fs_attestation_safe_cli-1.0.1/safe_cli/operators/hw_wallets/ledger_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/safe_cli/operators/hw_wallets/trezor_exceptions.py` & `fs_attestation_safe_cli-1.0.1/safe_cli/operators/hw_wallets/trezor_exceptions.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/safe_cli/operators/hw_wallets/trezor_wallet.py` & `fs_attestation_safe_cli-1.0.1/safe_cli/operators/hw_wallets/trezor_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/safe_cli/operators/safe_operator.py` & `fs_attestation_safe_cli-1.0.1/safe_cli/operators/safe_operator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/safe_cli/operators/safe_tx_service_operator.py` & `fs_attestation_safe_cli-1.0.1/safe_cli/operators/safe_tx_service_operator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/safe_cli/prompt_parser.py` & `fs_attestation_safe_cli-1.0.1/safe_cli/prompt_parser.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/safe_cli/safe_addresses.py` & `fs_attestation_safe_cli-1.0.1/safe_cli/safe_addresses.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/safe_cli/safe_completer.py` & `fs_attestation_safe_cli-1.0.1/safe_cli/safe_completer.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/safe_cli/safe_completer_constants.py` & `fs_attestation_safe_cli-1.0.1/safe_cli/safe_completer_constants.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/safe_cli/safe_creator.py` & `fs_attestation_safe_cli-1.0.1/safe_cli/safe_creator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/safe_cli/safe_lexer.py` & `fs_attestation_safe_cli-1.0.1/safe_cli/safe_lexer.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/safe_cli/utils.py` & `fs_attestation_safe_cli-1.0.1/safe_cli/utils.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/setup.cfg` & `fs_attestation_safe_cli-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/setup.py` & `fs_attestation_safe_cli-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         "fs-attestation-safe-eth-py==1.0.0",
         "tabulate>=0.8",
     ],
     extras_require={"ledger": ["ledgereth==0.9.1"], "trezor": ["trezor==0.13.8"]},
     packages=setuptools.find_packages(),
     entry_points={
         "console_scripts": [
-            "safe-cli=safe_cli.main:main",
+            "fs-attestation-safe-cli=safe_cli.main:main",
             "safe-creator=safe_cli.safe_creator:main",
         ],
     },
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

### Comparing `fs_attestation_safe_cli-1.0.0/tests/mocks/balances_mock.py` & `fs_attestation_safe_cli-1.0.1/tests/mocks/balances_mock.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/tests/mocks/data_decoded_mock.py` & `fs_attestation_safe_cli-1.0.1/tests/mocks/data_decoded_mock.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/tests/mocks/multisig_tx_mock.py` & `fs_attestation_safe_cli-1.0.1/tests/mocks/multisig_tx_mock.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/tests/mocks/txs_mock.py` & `fs_attestation_safe_cli-1.0.1/tests/mocks/txs_mock.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/tests/safe_cli_test_case_mixin.py` & `fs_attestation_safe_cli-1.0.1/tests/safe_cli_test_case_mixin.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/tests/test_argparse_validators.py` & `fs_attestation_safe_cli-1.0.1/tests/test_argparse_validators.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/tests/test_entrypoint.py` & `fs_attestation_safe_cli-1.0.1/tests/test_entrypoint.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/tests/test_ethereum_hd_wallet.py` & `fs_attestation_safe_cli-1.0.1/tests/test_ethereum_hd_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/tests/test_hw_wallet_manager.py` & `fs_attestation_safe_cli-1.0.1/tests/test_hw_wallet_manager.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/tests/test_ledger_wallet.py` & `fs_attestation_safe_cli-1.0.1/tests/test_ledger_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/tests/test_safe_addresses.py` & `fs_attestation_safe_cli-1.0.1/tests/test_safe_addresses.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/tests/test_safe_cli.py` & `fs_attestation_safe_cli-1.0.1/tests/test_safe_cli.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/tests/test_safe_completer.py` & `fs_attestation_safe_cli-1.0.1/tests/test_safe_completer.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/tests/test_safe_creator.py` & `fs_attestation_safe_cli-1.0.1/tests/test_safe_creator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/tests/test_safe_lexer.py` & `fs_attestation_safe_cli-1.0.1/tests/test_safe_lexer.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/tests/test_safe_operator.py` & `fs_attestation_safe_cli-1.0.1/tests/test_safe_operator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/tests/test_safe_tx_service_operator.py` & `fs_attestation_safe_cli-1.0.1/tests/test_safe_tx_service_operator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/tests/test_trezor_wallet.py` & `fs_attestation_safe_cli-1.0.1/tests/test_trezor_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/tests/test_utils.py` & `fs_attestation_safe_cli-1.0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.0/tests/utils.py` & `fs_attestation_safe_cli-1.0.1/tests/utils.py`

 * *Files identical despite different names*

