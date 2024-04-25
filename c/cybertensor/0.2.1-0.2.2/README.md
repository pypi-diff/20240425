# Comparing `tmp/cybertensor-0.2.1.tar.gz` & `tmp/cybertensor-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybertensor-0.2.1.tar", last modified: Fri Apr 19 06:58:31 2024, max compression
+gzip compressed data, was "cybertensor-0.2.2.tar", last modified: Thu Apr 25 08:54:21 2024, max compression
```

## Comparing `cybertensor-0.2.1.tar` & `cybertensor-0.2.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:58:31.201672 cybertensor-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-19 06:58:25.000000 cybertensor-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-19 06:58:25.000000 cybertensor-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-19 06:58:31.201672 cybertensor-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-19 06:58:25.000000 cybertensor-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:58:31.189672 cybertensor-0.2.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1996 2024-04-19 06:58:25.000000 cybertensor-0.2.1/bin/ctcli
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:58:31.193672 cybertensor-0.2.1/cybertensor/
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    67743 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/axon.py
--rw-r--r--   0 runner    (1001) docker     (127)    26316 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/chain_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11004 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:58:31.197672 cybertensor-0.2.1/cybertensor/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36930 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/commands/delegates.py
--rw-r--r--   0 runner    (1001) docker     (127)    15276 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/commands/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/commands/list.py
--rw-r--r--   0 runner    (1001) docker     (127)    10782 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/commands/metagraph.py
--rw-r--r--   0 runner    (1001) docker     (127)    33693 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/commands/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    29100 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/commands/overview.py
--rw-r--r--   0 runner    (1001) docker     (127)    17833 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/commands/register.py
--rw-r--r--   0 runner    (1001) docker     (127)    28434 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/commands/root.py
--rw-r--r--   0 runner    (1001) docker     (127)    23457 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/commands/stake.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/commands/transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12831 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/commands/unstake.py
--rw-r--r--   0 runner    (1001) docker     (127)     9023 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/commands/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    42803 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/commands/wallets.py
--rw-r--r--   0 runner    (1001) docker     (127)    14076 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/ctlogging.py
--rw-r--r--   0 runner    (1001) docker     (127)   108267 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/cwtensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    36538 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/dendrite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    30758 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/keyfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8975 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/keypair.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:58:31.197672 cybertensor-0.2.1/cybertensor/messages/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13307 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/messages/delegation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/messages/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/messages/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (127)    13319 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/messages/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/messages/root.py
--rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/messages/serving.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/messages/set_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)    17278 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/messages/staking.py
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/messages/transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14150 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/messages/unstaking.py
--rw-r--r--   0 runner    (1001) docker     (127)    22578 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/metagraph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:58:31.197672 cybertensor-0.2.1/cybertensor/mock/
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49856 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/mock/cwtensor_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/mock/keyfile_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/mock/wallet_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/subnets.py
--rw-r--r--   0 runner    (1001) docker     (127)    35924 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/synapse.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/threadpool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:58:31.201672 cybertensor-0.2.1/cybertensor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/utils/_register_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)    11666 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/utils/balance.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (127)    38150 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/utils/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/utils/wallet_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/utils/weight_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    30139 2024-04-19 06:58:25.000000 cybertensor-0.2.1/cybertensor/wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:58:31.201672 cybertensor-0.2.1/cybertensor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-19 06:58:31.000000 cybertensor-0.2.1/cybertensor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-19 06:58:31.000000 cybertensor-0.2.1/cybertensor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 06:58:31.000000 cybertensor-0.2.1/cybertensor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-19 06:58:31.000000 cybertensor-0.2.1/cybertensor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 06:58:31.000000 cybertensor-0.2.1/cybertensor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:58:31.201672 cybertensor-0.2.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-19 06:58:25.000000 cybertensor-0.2.1/requirements/cubit.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-19 06:58:25.000000 cybertensor-0.2.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-19 06:58:25.000000 cybertensor-0.2.1/requirements/prod.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 06:58:31.201672 cybertensor-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-19 06:58:25.000000 cybertensor-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:54:21.650867 cybertensor-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-25 08:54:16.000000 cybertensor-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-25 08:54:16.000000 cybertensor-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-25 08:54:21.650867 cybertensor-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-25 08:54:16.000000 cybertensor-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:54:21.634866 cybertensor-0.2.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1996 2024-04-25 08:54:16.000000 cybertensor-0.2.2/bin/ctcli
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:54:21.638867 cybertensor-0.2.2/cybertensor/
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67743 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/axon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26316 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/chain_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11004 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:54:21.642867 cybertensor-0.2.2/cybertensor/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36930 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/commands/delegates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15276 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/commands/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10782 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/commands/metagraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33693 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/commands/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29100 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/commands/overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17833 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/commands/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28434 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/commands/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23457 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/commands/stake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/commands/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12831 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/commands/unstake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9023 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42803 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/commands/wallets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14076 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/ctlogging.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108267 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/cwtensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36538 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/dendrite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30758 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/keyfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8975 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/keypair.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:54:21.642867 cybertensor-0.2.2/cybertensor/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13307 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/messages/delegation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/messages/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/messages/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13319 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/messages/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/messages/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/messages/serving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/messages/set_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17278 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/messages/staking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/messages/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14150 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/messages/unstaking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22578 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/metagraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:54:21.646867 cybertensor-0.2.2/cybertensor/mock/
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49856 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/mock/cwtensor_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/mock/keyfile_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/mock/wallet_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/subnets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35924 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/synapse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/threadpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:54:21.646867 cybertensor-0.2.2/cybertensor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/utils/_register_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11666 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/utils/balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38150 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/utils/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/utils/wallet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/utils/weight_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30139 2024-04-25 08:54:16.000000 cybertensor-0.2.2/cybertensor/wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:54:21.646867 cybertensor-0.2.2/cybertensor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-25 08:54:21.000000 cybertensor-0.2.2/cybertensor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-25 08:54:21.000000 cybertensor-0.2.2/cybertensor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:54:21.000000 cybertensor-0.2.2/cybertensor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-25 08:54:21.000000 cybertensor-0.2.2/cybertensor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 08:54:21.000000 cybertensor-0.2.2/cybertensor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:54:21.646867 cybertensor-0.2.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-25 08:54:16.000000 cybertensor-0.2.2/requirements/cubit.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-25 08:54:16.000000 cybertensor-0.2.2/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-25 08:54:16.000000 cybertensor-0.2.2/requirements/prod.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 08:54:21.650867 cybertensor-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-25 08:54:16.000000 cybertensor-0.2.2/setup.py
```

### Comparing `cybertensor-0.2.1/LICENSE` & `cybertensor-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/PKG-INFO` & `cybertensor-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybertensor
-Version: 0.2.1
+Version: 0.2.2
 Summary: cybertensor
 Home-page: https://github.com/cybercongress/cybertensor
 Author: cyberhead
 Author-email: 
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `cybertensor-0.2.1/README.md` & `cybertensor-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/bin/ctcli` & `cybertensor-0.2.2/bin/ctcli`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/__init__.py` & `cybertensor-0.2.2/cybertensor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from cosmpy.aerial.config import NetworkConfig
 from rich.console import Console
 from rich.traceback import install
 
 nest_asyncio.apply()
 
 # Cybertensor code and protocol version.
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 version_split = __version__.split(".")
 __version_as_int__ = (
     (100 * int(version_split[0]))
     + (10 * int(version_split[1]))
     + (1 * int(version_split[2]))
 )
```

### Comparing `cybertensor-0.2.1/cybertensor/axon.py` & `cybertensor-0.2.2/cybertensor/axon.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/chain_data.py` & `cybertensor-0.2.2/cybertensor/chain_data.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/cli.py` & `cybertensor-0.2.2/cybertensor/cli.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/commands/__init__.py` & `cybertensor-0.2.2/cybertensor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/commands/delegates.py` & `cybertensor-0.2.2/cybertensor/commands/delegates.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/commands/identity.py` & `cybertensor-0.2.2/cybertensor/commands/identity.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/commands/inspect.py` & `cybertensor-0.2.2/cybertensor/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/commands/list.py` & `cybertensor-0.2.2/cybertensor/commands/list.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/commands/metagraph.py` & `cybertensor-0.2.2/cybertensor/commands/metagraph.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/commands/network.py` & `cybertensor-0.2.2/cybertensor/commands/network.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/commands/overview.py` & `cybertensor-0.2.2/cybertensor/commands/overview.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/commands/register.py` & `cybertensor-0.2.2/cybertensor/commands/register.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/commands/root.py` & `cybertensor-0.2.2/cybertensor/commands/root.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/commands/stake.py` & `cybertensor-0.2.2/cybertensor/commands/stake.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/commands/transfer.py` & `cybertensor-0.2.2/cybertensor/commands/transfer.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/commands/unstake.py` & `cybertensor-0.2.2/cybertensor/commands/unstake.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/commands/utils.py` & `cybertensor-0.2.2/cybertensor/commands/utils.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/commands/wallets.py` & `cybertensor-0.2.2/cybertensor/commands/wallets.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/config.py` & `cybertensor-0.2.2/cybertensor/config.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/ctlogging.py` & `cybertensor-0.2.2/cybertensor/ctlogging.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/cwtensor.py` & `cybertensor-0.2.2/cybertensor/cwtensor.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/dendrite.py` & `cybertensor-0.2.2/cybertensor/dendrite.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/errors.py` & `cybertensor-0.2.2/cybertensor/errors.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/keyfile.py` & `cybertensor-0.2.2/cybertensor/keyfile.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/keypair.py` & `cybertensor-0.2.2/cybertensor/keypair.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/messages/__init__.py` & `cybertensor-0.2.2/cybertensor/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/messages/delegation.py` & `cybertensor-0.2.2/cybertensor/messages/delegation.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/messages/network.py` & `cybertensor-0.2.2/cybertensor/messages/network.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/messages/prometheus.py` & `cybertensor-0.2.2/cybertensor/messages/prometheus.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/messages/registration.py` & `cybertensor-0.2.2/cybertensor/messages/registration.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/messages/root.py` & `cybertensor-0.2.2/cybertensor/messages/root.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/messages/serving.py` & `cybertensor-0.2.2/cybertensor/messages/serving.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/messages/set_weights.py` & `cybertensor-0.2.2/cybertensor/messages/set_weights.py`

 * *Files 10% similar despite different names*

```diff
@@ -98,29 +98,21 @@
                 wait_for_finalization=wait_for_finalization,
             )
 
             if not wait_for_finalization:
                 return True, "Not waiting for finalization."
 
             if success is True:
-                cybertensor.__console__.print(
-                    prefix="Set weights",
-                    sufix="<green>Finalized: </green>" + str(success),
-                )
                 return True, "Successfully set weights and Finalized."
             else:
-                cybertensor.__console__.print(
-                    ":cross_mark: [red]Failed[/red]: error:{}".format(error_message)
-                )
-
                 cybertensor.logging.warning(
                     prefix="Set weights",
-                    sufix="<red>Failed: </red>" + str(error_message),
+                    sufix=f"<red>Failed: </red> {error_message}",
                 )
                 return False, error_message
 
         except Exception as e:
             # TODO( devs ): lets remove all of the cybertensor.__console__ calls and replace with loguru.
             cybertensor.logging.warning(
-                prefix="Set weights", sufix="<red>Failed: </red>" + str(e)
+                prefix="Set weights", sufix=f"<red>Failed: </red> {e}"
             )
             return False, str(e)
```

### Comparing `cybertensor-0.2.1/cybertensor/messages/staking.py` & `cybertensor-0.2.2/cybertensor/messages/staking.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/messages/transfer.py` & `cybertensor-0.2.2/cybertensor/messages/transfer.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/messages/unstaking.py` & `cybertensor-0.2.2/cybertensor/messages/unstaking.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/metagraph.py` & `cybertensor-0.2.2/cybertensor/metagraph.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/mock/__init__.py` & `cybertensor-0.2.2/cybertensor/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/mock/cwtensor_mock.py` & `cybertensor-0.2.2/cybertensor/mock/cwtensor_mock.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/mock/keyfile_mock.py` & `cybertensor-0.2.2/cybertensor/mock/keyfile_mock.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/mock/wallet_mock.py` & `cybertensor-0.2.2/cybertensor/mock/wallet_mock.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/stream.py` & `cybertensor-0.2.2/cybertensor/stream.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/subnets.py` & `cybertensor-0.2.2/cybertensor/subnets.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/synapse.py` & `cybertensor-0.2.2/cybertensor/synapse.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/tensor.py` & `cybertensor-0.2.2/cybertensor/tensor.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/threadpool.py` & `cybertensor-0.2.2/cybertensor/threadpool.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/types.py` & `cybertensor-0.2.2/cybertensor/types.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/utils/__init__.py` & `cybertensor-0.2.2/cybertensor/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/utils/_register_cuda.py` & `cybertensor-0.2.2/cybertensor/utils/_register_cuda.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/utils/balance.py` & `cybertensor-0.2.2/cybertensor/utils/balance.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/utils/formatting.py` & `cybertensor-0.2.2/cybertensor/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/utils/networking.py` & `cybertensor-0.2.2/cybertensor/utils/networking.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/utils/registration.py` & `cybertensor-0.2.2/cybertensor/utils/registration.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/utils/wallet_utils.py` & `cybertensor-0.2.2/cybertensor/utils/wallet_utils.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/utils/weight_utils.py` & `cybertensor-0.2.2/cybertensor/utils/weight_utils.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor/wallet.py` & `cybertensor-0.2.2/cybertensor/wallet.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor.egg-info/PKG-INFO` & `cybertensor-0.2.2/cybertensor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybertensor
-Version: 0.2.1
+Version: 0.2.2
 Summary: cybertensor
 Home-page: https://github.com/cybercongress/cybertensor
 Author: cyberhead
 Author-email: 
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `cybertensor-0.2.1/cybertensor.egg-info/SOURCES.txt` & `cybertensor-0.2.2/cybertensor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/cybertensor.egg-info/requires.txt` & `cybertensor-0.2.2/cybertensor.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/requirements/prod.txt` & `cybertensor-0.2.2/requirements/prod.txt`

 * *Files identical despite different names*

### Comparing `cybertensor-0.2.1/setup.py` & `cybertensor-0.2.2/setup.py`

 * *Files identical despite different names*

