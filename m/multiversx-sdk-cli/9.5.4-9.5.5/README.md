# Comparing `tmp/multiversx_sdk_cli-9.5.4.tar.gz` & `tmp/multiversx_sdk_cli-9.5.5.tar.gz`

## Comparing `multiversx_sdk_cli-9.5.4.tar` & `multiversx_sdk_cli-9.5.5.tar`

### file list

```diff
@@ -1,110 +1,110 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/__init__.py
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/accounts.py
--rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_accounts.py
--rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_config.py
--rw-r--r--   0        0        0    22514 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_contracts.py
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_data.py
--rw-r--r--   0        0        0    15634 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_delegation.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_deps.py
--rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_dns.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_ledger.py
--rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_localnet.py
--rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_output.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_password.py
--rw-r--r--   0        0        0    14251 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_shared.py
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_transactions.py
--rw-r--r--   0        0        0     8856 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_validators.py
--rw-r--r--   0        0        0    11681 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_wallet.py
--rw-r--r--   0        0        0     8226 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/config.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/constants.py
--rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/contract_verification.py
--rw-r--r--   0        0        0    11938 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/contracts.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cosign_transaction.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/custom_network_provider.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/dependency_checker.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/dns.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/docker.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/downloader.py
--rw-r--r--   0        0        0     5541 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/errors.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/guards.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/interfaces.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/myprocess.py
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/sign_verify.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/simulation.py
--rw-r--r--   0        0        0     7799 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/transactions.py
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/utils.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/ux.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/version.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/workstation.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/.vscode/settings.json
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/delegation/__init__.py
--rw-r--r--   0        0        0    12763 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/delegation/staking_provider.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/dependencies/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/dependencies/install.py
--rw-r--r--   0        0        0    15051 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/dependencies/modules.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/dependencies/resolution.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/ledger/__init__.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/ledger/config.py
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/ledger/ledger_app_handler.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/ledger/ledger_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/__init__.py
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/config_default.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/config_general.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/config_networking.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/config_part.py
--rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/config_root.py
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/config_sharding.py
--rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/config_software.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/constants.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/genesis.py
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/genesis_json.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/genesis_smart_contracts_json.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/libraries.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/node.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/node_config_toml.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/nodes_setup_json.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/p2p_toml.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/seednode_p2pKey.pem
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/step_build_software.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/step_clean.py
--rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/step_config.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/step_new.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/step_prerequisites.py
--rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/step_start.py
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/wallets.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/__init__.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/constants.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/core.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/interfaces.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/migrations.py
--rw-r--r--   0        0        0     7079 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/project_base.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/project_rust.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/shared.py
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/templates.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/__init__.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/do_report.py
--rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/report_creator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/data/__init__.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/data/common.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/data/extracted_feature.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/data/folder_report.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/data/project_report.py
--rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/data/report.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/data/wasm_report.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/features/__init__.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/features/features.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/features/report_option.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/features/size.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/format/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/format/change_type.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/format/format_options.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/validators/__init__.py
--rw-r--r--   0        0        0     7053 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/validators/core.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/validators/validators_file.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/LICENSE
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/README.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/pyproject.toml
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/__init__.py
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/accounts.py
+-rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_accounts.py
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_config.py
+-rw-r--r--   0        0        0    22514 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_contracts.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_data.py
+-rw-r--r--   0        0        0    15634 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_delegation.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_deps.py
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_dns.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_ledger.py
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_localnet.py
+-rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_output.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_password.py
+-rw-r--r--   0        0        0    14251 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_shared.py
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_transactions.py
+-rw-r--r--   0        0        0     8856 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_validators.py
+-rw-r--r--   0        0        0    11681 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_wallet.py
+-rw-r--r--   0        0        0     8226 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/config.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/constants.py
+-rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/contract_verification.py
+-rw-r--r--   0        0        0    11938 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/contracts.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cosign_transaction.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/custom_network_provider.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/dependency_checker.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/dns.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/docker.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/downloader.py
+-rw-r--r--   0        0        0     5541 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/errors.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/guards.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/interfaces.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/myprocess.py
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/sign_verify.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/simulation.py
+-rw-r--r--   0        0        0     7799 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/transactions.py
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/utils.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/ux.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/version.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/workstation.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/.vscode/settings.json
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/delegation/__init__.py
+-rw-r--r--   0        0        0    12763 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/delegation/staking_provider.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/dependencies/__init__.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/dependencies/install.py
+-rw-r--r--   0        0        0    15051 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/dependencies/modules.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/dependencies/resolution.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/ledger/__init__.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/ledger/config.py
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/ledger/ledger_app_handler.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/ledger/ledger_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/__init__.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_default.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_general.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_networking.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_part.py
+-rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_root.py
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_sharding.py
+-rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_software.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/constants.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/genesis.py
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/genesis_json.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/genesis_smart_contracts_json.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/libraries.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/node.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/node_config_toml.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/nodes_setup_json.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/p2p_toml.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/seednode_p2pKey.pem
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/step_build_software.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/step_clean.py
+-rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/step_config.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/step_new.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/step_prerequisites.py
+-rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/step_start.py
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/wallets.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/__init__.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/constants.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/core.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/interfaces.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/migrations.py
+-rw-r--r--   0        0        0     7079 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/project_base.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/project_rust.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/shared.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/templates.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/__init__.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/do_report.py
+-rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/report_creator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/__init__.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/common.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/extracted_feature.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/folder_report.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/project_report.py
+-rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/report.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/wasm_report.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/features/__init__.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/features/features.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/features/report_option.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/features/size.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/format/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/format/change_type.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/format/format_options.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/validators/__init__.py
+-rw-r--r--   0        0        0     7053 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/validators/core.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/validators/validators_file.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/LICENSE
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/README.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/pyproject.toml
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/PKG-INFO
```

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/accounts.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/accounts.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_accounts.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_accounts.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_config.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_contracts.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_contracts.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_data.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_data.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_delegation.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_delegation.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_deps.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_deps.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_dns.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_dns.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_ledger.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_ledger.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_localnet.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_localnet.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_output.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_output.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_shared.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_shared.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_transactions.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_transactions.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_validators.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_validators.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cli_wallet.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_wallet.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/config.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/constants.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/constants.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/contract_verification.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/contract_verification.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/contracts.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/contracts.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/cosign_transaction.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cosign_transaction.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/custom_network_provider.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/custom_network_provider.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/dns.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/dns.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/docker.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/docker.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/downloader.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/downloader.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/errors.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/errors.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/interfaces.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/interfaces.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/myprocess.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/myprocess.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/sign_verify.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/sign_verify.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/simulation.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/simulation.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/transactions.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/transactions.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/utils.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/utils.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/ux.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/ux.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/version.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/version.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/workstation.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/workstation.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/delegation/staking_provider.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/delegation/staking_provider.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/dependencies/install.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/dependencies/install.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/dependencies/modules.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/dependencies/modules.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/ledger/config.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/ledger/config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/ledger/ledger_app_handler.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/ledger/ledger_app_handler.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/ledger/ledger_functions.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/ledger/ledger_functions.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/config_default.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_default.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/config_general.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_general.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/config_networking.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_networking.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/config_part.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_part.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/config_root.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_root.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/config_sharding.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_sharding.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/config_software.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_software.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/genesis.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/genesis.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/genesis_json.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/genesis_json.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/libraries.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/libraries.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/node.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/node.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/node_config_toml.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/node_config_toml.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/nodes_setup_json.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/nodes_setup_json.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/p2p_toml.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/p2p_toml.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/step_build_software.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/step_build_software.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/step_config.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/step_config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/step_prerequisites.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/step_prerequisites.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/step_start.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/step_start.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/localnet/wallets.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/wallets.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/__init__.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/core.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/core.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/migrations.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/migrations.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/project_base.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/project_base.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/project_rust.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/project_rust.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/templates.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/templates.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/do_report.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/do_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/report_creator.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/report_creator.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/data/common.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/common.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/data/extracted_feature.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/extracted_feature.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/data/folder_report.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/folder_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/data/project_report.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/project_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/data/report.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/data/wasm_report.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/wasm_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/features/report_option.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/features/report_option.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/projects/report/format/change_type.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/format/change_type.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/validators/__init__.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/validators/core.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/validators/core.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/multiversx_sdk_cli/validators/validators_file.py` & `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/validators/validators_file.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/LICENSE` & `multiversx_sdk_cli-9.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/README.md` & `multiversx_sdk_cli-9.5.5/README.md`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.4/pyproject.toml` & `multiversx_sdk_cli-9.5.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "multiversx-sdk-cli"
-version = "9.5.4"
+version = "9.5.5"
 authors = [
   { name="MultiversX" },
 ]
 license = "MIT"
 description = "MultiversX Smart Contracts Tools"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -23,17 +23,17 @@
   "toml>=0.10.2",
   "requests",
   "prettytable",
   "ledgercomm[hid]",
   "semver",
   "requests-cache",
   "rich==13.3.4",
-  "multiversx-sdk-network-providers>=0.12.0,<0.13.0",
-  "multiversx-sdk-wallet>=0.8.0,<0.9.0,",
-  "multiversx-sdk-core>=0.7.0,<0.8.0"
+  "multiversx-sdk-network-providers>=0.13.0,<0.14.0",
+  "multiversx-sdk-wallet>=0.9.0,<0.10.0",
+  "multiversx-sdk-core>=0.8.0,<0.9.0"
 ]
 
 [project.scripts]
 mxpy = "multiversx_sdk_cli.cli:main"
 
 [tool.hatch.build]
 include = [
```

### Comparing `multiversx_sdk_cli-9.5.4/PKG-INFO` & `multiversx_sdk_cli-9.5.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.3
 Name: multiversx-sdk-cli
-Version: 9.5.4
+Version: 9.5.5
 Summary: MultiversX Smart Contracts Tools
 Project-URL: Homepage, https://github.com/multiversx/mx-sdk-py-cli
 Author: MultiversX
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: ledgercomm[hid]
-Requires-Dist: multiversx-sdk-core<0.8.0,>=0.7.0
-Requires-Dist: multiversx-sdk-network-providers<0.13.0,>=0.12.0
-Requires-Dist: multiversx-sdk-wallet<0.9.0,>=0.8.0
+Requires-Dist: multiversx-sdk-core<0.9.0,>=0.8.0
+Requires-Dist: multiversx-sdk-network-providers<0.14.0,>=0.13.0
+Requires-Dist: multiversx-sdk-wallet<0.10.0,>=0.9.0
 Requires-Dist: prettytable
 Requires-Dist: requests
 Requires-Dist: requests-cache
 Requires-Dist: rich==13.3.4
 Requires-Dist: semver
 Requires-Dist: toml>=0.10.2
 Description-Content-Type: text/markdown
```

