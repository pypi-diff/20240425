# Comparing `tmp/fs-attestation-safe-eth-py-1.0.0.tar.gz` & `tmp/fs-attestation-safe-eth-py-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fs-attestation-safe-eth-py-1.0.0.tar", last modified: Wed Apr 24 08:02:58 2024, max compression
+gzip compressed data, was "fs-attestation-safe-eth-py-1.0.1.tar", last modified: Thu Apr 25 06:40:15 2024, max compression
```

## Comparing `fs-attestation-safe-eth-py-1.0.0.tar` & `fs-attestation-safe-eth-py-1.0.1.tar`

### file list

```diff
@@ -1,234 +1,234 @@
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.629232 fs-attestation-safe-eth-py-1.0.0/
--rw-r--r--   0 mohan      (501) staff       (20)     1082 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/LICENSE
--rw-r--r--   0 mohan      (501) staff       (20)       71 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/MANIFEST.in
--rw-r--r--   0 mohan      (501) staff       (20)     7150 2024-04-24 08:02:58.629442 fs-attestation-safe-eth-py-1.0.0/PKG-INFO
--rw-r--r--   0 mohan      (501) staff       (20)     5786 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/README.rst
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.557604 fs-attestation-safe-eth-py-1.0.0/docs/
--rw-r--r--   0 mohan      (501) staff       (20)      638 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/docs/Makefile
--rw-r--r--   0 mohan      (501) staff       (20)      799 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/docs/make.bat
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.562286 fs-attestation-safe-eth-py-1.0.0/docs/source/
--rw-r--r--   0 mohan      (501) staff       (20)     1987 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/docs/source/conf.py
--rw-r--r--   0 mohan      (501) staff       (20)      978 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/docs/source/gnosis.eth.clients.rst
--rw-r--r--   0 mohan      (501) staff       (20)      183 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/docs/source/gnosis.eth.contracts.rst
--rw-r--r--   0 mohan      (501) staff       (20)      954 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/docs/source/gnosis.eth.django.rst
--rw-r--r--   0 mohan      (501) staff       (20)      177 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/docs/source/gnosis.eth.eip712.rst
--rw-r--r--   0 mohan      (501) staff       (20)     1198 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/docs/source/gnosis.eth.oracles.abis.rst
--rw-r--r--   0 mohan      (501) staff       (20)      450 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/docs/source/gnosis.eth.oracles.rst
--rw-r--r--   0 mohan      (501) staff       (20)      936 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/docs/source/gnosis.eth.rst
--rw-r--r--   0 mohan      (501) staff       (20)      226 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/docs/source/gnosis.rst
--rw-r--r--   0 mohan      (501) staff       (20)     1852 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/docs/source/gnosis.safe.rst
--rw-r--r--   0 mohan      (501) staff       (20)      894 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/docs/source/index.rst
--rw-r--r--   0 mohan      (501) staff       (20)       55 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/docs/source/modules.rst
--rw-r--r--   0 mohan      (501) staff       (20)     8368 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/docs/source/quickstart.rst
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.564455 fs-attestation-safe-eth-py-1.0.0/fs_attestation_safe_eth_py.egg-info/
--rw-r--r--   0 mohan      (501) staff       (20)     7150 2024-04-24 08:02:58.000000 fs-attestation-safe-eth-py-1.0.0/fs_attestation_safe_eth_py.egg-info/PKG-INFO
--rw-r--r--   0 mohan      (501) staff       (20)     7536 2024-04-24 08:02:58.000000 fs-attestation-safe-eth-py-1.0.0/fs_attestation_safe_eth_py.egg-info/SOURCES.txt
--rw-r--r--   0 mohan      (501) staff       (20)        1 2024-04-24 08:02:58.000000 fs-attestation-safe-eth-py-1.0.0/fs_attestation_safe_eth_py.egg-info/dependency_links.txt
--rw-r--r--   0 mohan      (501) staff       (20)      129 2024-04-24 08:02:58.000000 fs-attestation-safe-eth-py-1.0.0/fs_attestation_safe_eth_py.egg-info/requires.txt
--rw-r--r--   0 mohan      (501) staff       (20)        7 2024-04-24 08:02:58.000000 fs-attestation-safe-eth-py-1.0.0/fs_attestation_safe_eth_py.egg-info/top_level.txt
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.565218 fs-attestation-safe-eth-py-1.0.0/gnosis/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/__init__.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.566954 fs-attestation-safe-eth-py-1.0.0/gnosis/cowsap/
--rw-r--r--   0 mohan      (501) staff       (20)      156 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/cowsap/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     8465 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/cowsap/cow_swap_api.py
--rw-r--r--   0 mohan      (501) staff       (20)     2700 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/cowsap/order.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.567880 fs-attestation-safe-eth-py-1.0.0/gnosis/cowsap/tests/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/cowsap/tests/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     5604 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/cowsap/tests/test_cow_swap_api.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.571432 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/
--rw-r--r--   0 mohan      (501) staff       (20)     1064 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/__init__.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.573575 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/account_abstraction/
--rw-r--r--   0 mohan      (501) staff       (20)      348 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/account_abstraction/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     7060 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/account_abstraction/bundler_client.py
--rw-r--r--   0 mohan      (501) staff       (20)      986 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/account_abstraction/constants.py
--rw-r--r--   0 mohan      (501) staff       (20)      208 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/account_abstraction/exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)     4259 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/account_abstraction/user_operation.py
--rw-r--r--   0 mohan      (501) staff       (20)     3357 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/account_abstraction/user_operation_receipt.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.575689 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/clients/
--rw-r--r--   0 mohan      (501) staff       (20)      878 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/clients/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     9236 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/clients/blockscout_client.py
--rw-r--r--   0 mohan      (501) staff       (20)      194 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/clients/contract_metadata.py
--rw-r--r--   0 mohan      (501) staff       (20)     4839 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/clients/ens_client.py
--rw-r--r--   0 mohan      (501) staff       (20)     9677 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/clients/etherscan_client.py
--rw-r--r--   0 mohan      (501) staff       (20)     3345 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/clients/sourcify_client.py
--rw-r--r--   0 mohan      (501) staff       (20)     1020 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/constants.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.576283 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/
--rw-r--r--   0 mohan      (501) staff       (20)    10273 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/__init__.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.593348 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/
--rw-r--r--   0 mohan      (501) staff       (20)   328664 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/CPKFactory.json
--rw-r--r--   0 mohan      (501) staff       (20)    28908 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_3_0.json
--rw-r--r--   0 mohan      (501) staff       (20)    29485 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_4_1.json
--rw-r--r--   0 mohan      (501) staff       (20)    26897 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/DelegateConstructorProxy.json
--rw-r--r--   0 mohan      (501) staff       (20)    29068 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ERC1155.json
--rw-r--r--   0 mohan      (501) staff       (20)    54748 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ERC20.json
--rw-r--r--   0 mohan      (501) staff       (20)    89890 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ERC20TestToken.json
--rw-r--r--   0 mohan      (501) staff       (20)   622260 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ERC721.json
--rw-r--r--   0 mohan      (501) staff       (20)   983403 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/GnosisSafe_V0_0_1.json
--rw-r--r--   0 mohan      (501) staff       (20)  1158944 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/GnosisSafe_V1_0_0.json
--rw-r--r--   0 mohan      (501) staff       (20)  1347363 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/GnosisSafe_V1_1_1.json
--rw-r--r--   0 mohan      (501) staff       (20)   119875 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/GnosisSafe_V1_3_0.json
--rw-r--r--   0 mohan      (501) staff       (20)    19886 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/MultiSend.json
--rw-r--r--   0 mohan      (501) staff       (20)    78793 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/PayingProxy.json
--rw-r--r--   0 mohan      (501) staff       (20)   136946 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ProxyFactory_V1_0_0.json
--rw-r--r--   0 mohan      (501) staff       (20)   288861 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ProxyFactory_V1_1_1.json
--rw-r--r--   0 mohan      (501) staff       (20)    18975 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ProxyFactory_V1_3_0.json
--rw-r--r--   0 mohan      (501) staff       (20)    15538 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ProxyFactory_V1_4_1.json
--rw-r--r--   0 mohan      (501) staff       (20)    32495 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/Proxy_V1_0_0.json
--rw-r--r--   0 mohan      (501) staff       (20)    39032 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/Proxy_V1_1_1.json
--rw-r--r--   0 mohan      (501) staff       (20)     1862 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/Proxy_V1_3_0.json
--rw-r--r--   0 mohan      (501) staff       (20)     1849 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/Proxy_V1_4_1.json
--rw-r--r--   0 mohan      (501) staff       (20)   121611 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/Safe_V1_4_1.json
--rw-r--r--   0 mohan      (501) staff       (20)     5069 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/SignMessageLib.json
--rw-r--r--   0 mohan      (501) staff       (20)     4913 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/SimulateTxAccessor_V1_4_1.json
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     7351 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/kyber_network_proxy.json
--rw-r--r--   0 mohan      (501) staff       (20)    19012 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/multicall.py
--rw-r--r--   0 mohan      (501) staff       (20)    17165 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/uniswap_exchange.json
--rw-r--r--   0 mohan      (501) staff       (20)     2480 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/uniswap_factory.json
--rw-r--r--   0 mohan      (501) staff       (20)     2242 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/uniswap_v2_factory.json
--rw-r--r--   0 mohan      (501) staff       (20)     8293 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/uniswap_v2_pair.json
--rw-r--r--   0 mohan      (501) staff       (20)    11889 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/uniswap_v2_router.json
--rw-r--r--   0 mohan      (501) staff       (20)      954 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/contract_base.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.595419 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/django/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/django/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     3735 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/django/admin.py
--rw-r--r--   0 mohan      (501) staff       (20)      269 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/django/filters.py
--rw-r--r--   0 mohan      (501) staff       (20)     2435 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/django/forms.py
--rw-r--r--   0 mohan      (501) staff       (20)     9936 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/django/models.py
--rw-r--r--   0 mohan      (501) staff       (20)     6191 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/django/serializers.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.597084 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/django/tests/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/django/tests/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)      711 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/django/tests/models.py
--rw-r--r--   0 mohan      (501) staff       (20)     3028 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/django/tests/test_forms.py
--rw-r--r--   0 mohan      (501) staff       (20)     8621 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/django/tests/test_models.py
--rw-r--r--   0 mohan      (501) staff       (20)     7877 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/django/tests/test_serializers.py
--rw-r--r--   0 mohan      (501) staff       (20)      484 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/django/tests/test_validators.py
--rw-r--r--   0 mohan      (501) staff       (20)      320 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/django/validators.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.597538 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/eip712/
--rw-r--r--   0 mohan      (501) staff       (20)     5915 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/eip712/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)    82106 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/ethereum_client.py
--rw-r--r--   0 mohan      (501) staff       (20)    35545 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/ethereum_network.py
--rw-r--r--   0 mohan      (501) staff       (20)     1332 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)    13617 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/multicall.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.601245 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/
--rw-r--r--   0 mohan      (501) staff       (20)     1093 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/__init__.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.604197 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)    15986 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/aave_abis.py
--rw-r--r--   0 mohan      (501) staff       (20)    30036 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/balancer_abis.py
--rw-r--r--   0 mohan      (501) staff       (20)    29731 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/cream_abis.py
--rw-r--r--   0 mohan      (501) staff       (20)    27567 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/curve_abis.py
--rw-r--r--   0 mohan      (501) staff       (20)    25872 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/mooniswap_abis.py
--rw-r--r--   0 mohan      (501) staff       (20)      239 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/superfluid_abis.py
--rw-r--r--   0 mohan      (501) staff       (20)    45208 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/uniswap_v3.py
--rw-r--r--   0 mohan      (501) staff       (20)    36257 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/yearn_abis.py
--rw-r--r--   0 mohan      (501) staff       (20)     1464 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/zerion_abis.py
--rw-r--r--   0 mohan      (501) staff       (20)     2375 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/cowswap.py
--rw-r--r--   0 mohan      (501) staff       (20)      161 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/exceptions.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.604578 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/helpers/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/helpers/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     5856 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/helpers/curve_gauge_list.py
--rw-r--r--   0 mohan      (501) staff       (20)     4117 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/kyber.py
--rw-r--r--   0 mohan      (501) staff       (20)    32169 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/oracles.py
--rw-r--r--   0 mohan      (501) staff       (20)     1677 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/superfluid.py
--rw-r--r--   0 mohan      (501) staff       (20)     1516 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/sushiswap.py
--rw-r--r--   0 mohan      (501) staff       (20)     7154 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/uniswap_v3.py
--rw-r--r--   0 mohan      (501) staff       (20)     1064 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/utils.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.606447 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/__init__.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.607846 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/account_abstraction/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/account_abstraction/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     6695 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/account_abstraction/test_bundler_client.py
--rw-r--r--   0 mohan      (501) staff       (20)     2727 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/account_abstraction/test_e2e_bundler_client.py
--rw-r--r--   0 mohan      (501) staff       (20)      671 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/account_abstraction/test_user_operation.py
--rw-r--r--   0 mohan      (501) staff       (20)      947 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/account_abstraction/test_user_operation_receipt.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.609310 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/clients/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/clients/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)   107388 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/clients/mocks.py
--rw-r--r--   0 mohan      (501) staff       (20)     1047 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/clients/test_blockscout_client.py
--rw-r--r--   0 mohan      (501) staff       (20)     6185 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/clients/test_ens_client.py
--rw-r--r--   0 mohan      (501) staff       (20)     1686 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/clients/test_etherscan_client.py
--rw-r--r--   0 mohan      (501) staff       (20)     2521 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/clients/test_sourcify_client.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.609797 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/eip712/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/eip712/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)    13327 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/eip712/test_eip712.py
--rw-r--r--   0 mohan      (501) staff       (20)     3189 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/ethereum_test_case.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.613047 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)    29208 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_bundler.py
--rw-r--r--   0 mohan      (501) staff       (20)    31306 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_internal_txs.py
--rw-r--r--   0 mohan      (501) staff       (20)    10570 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_log_receipts.py
--rw-r--r--   0 mohan      (501) staff       (20)   792720 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_trace_block.py
--rw-r--r--   0 mohan      (501) staff       (20)    92795 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_trace_filter.py
--rw-r--r--   0 mohan      (501) staff       (20)   171076 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_trace_transaction.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.615758 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     2706 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/test_cowswap.py
--rw-r--r--   0 mohan      (501) staff       (20)     1820 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/test_kyber.py
--rw-r--r--   0 mohan      (501) staff       (20)     1460 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/test_superfluid.py
--rw-r--r--   0 mohan      (501) staff       (20)     2043 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/test_sushiswap.py
--rw-r--r--   0 mohan      (501) staff       (20)     3544 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/test_uniswap_v3.py
--rw-r--r--   0 mohan      (501) staff       (20)    61025 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/test_ethereum_client.py
--rw-r--r--   0 mohan      (501) staff       (20)     7087 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/test_multicall.py
--rw-r--r--   0 mohan      (501) staff       (20)    21137 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/test_oracles.py
--rw-r--r--   0 mohan      (501) staff       (20)     7287 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/test_utils.py
--rw-r--r--   0 mohan      (501) staff       (20)     5069 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/utils.py
--rw-r--r--   0 mohan      (501) staff       (20)      390 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/typing.py
--rw-r--r--   0 mohan      (501) staff       (20)     6977 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/eth/utils.py
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/py.typed
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.620731 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/
--rw-r--r--   0 mohan      (501) staff       (20)      742 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/__init__.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.621181 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/account_abstraction/
--rw-r--r--   0 mohan      (501) staff       (20)      101 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/account_abstraction/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     5647 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/account_abstraction/safe_operation.py
--rw-r--r--   0 mohan      (501) staff       (20)    63401 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/addresses.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.621860 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/api/
--rw-r--r--   0 mohan      (501) staff       (20)      346 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/api/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     2471 2024-04-24 04:21:12.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/api/base_api.py
--rw-r--r--   0 mohan      (501) staff       (20)     2913 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/api/relay_service_api.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.622921 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/api/transaction_service_api/
--rw-r--r--   0 mohan      (501) staff       (20)      103 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/api/transaction_service_api/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)    14033 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/api/transaction_service_api/transaction_service_api.py
--rw-r--r--   0 mohan      (501) staff       (20)     1732 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/api/transaction_service_api/transaction_service_messages.py
--rw-r--r--   0 mohan      (501) staff       (20)      252 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/api/transaction_service_api/transaction_service_tx.py
--rw-r--r--   0 mohan      (501) staff       (20)      105 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/enums.py
--rw-r--r--   0 mohan      (501) staff       (20)     1451 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)    11459 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/multi_send.py
--rw-r--r--   0 mohan      (501) staff       (20)    10479 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/proxy_factory.py
--rw-r--r--   0 mohan      (501) staff       (20)    36823 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/safe.py
--rw-r--r--   0 mohan      (501) staff       (20)    11975 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/safe_create2_tx.py
--rw-r--r--   0 mohan      (501) staff       (20)     9736 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/safe_creator.py
--rw-r--r--   0 mohan      (501) staff       (20)   121198 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/safe_deployments.py
--rw-r--r--   0 mohan      (501) staff       (20)    12587 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/safe_signature.py
--rw-r--r--   0 mohan      (501) staff       (20)    17225 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/safe_tx.py
--rw-r--r--   0 mohan      (501) staff       (20)     4194 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/serializers.py
--rw-r--r--   0 mohan      (501) staff       (20)     2000 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/signatures.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.626132 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/__init__.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.626512 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/account_abstraction/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/account_abstraction/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     3469 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/account_abstraction/test_safe_operation.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.626902 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/api/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/api/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     5341 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/api/test_transaction_service_api.py
--rw-r--r--   0 mohan      (501) staff       (20)    20692 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/safe_test_case.py
--rw-r--r--   0 mohan      (501) staff       (20)     1398 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_addresses.py
--rw-r--r--   0 mohan      (501) staff       (20)    10515 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_multi_send.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.627668 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_proxy_factory/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_proxy_factory/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     7798 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_proxy_factory/test_proxy_factory.py
--rw-r--r--   0 mohan      (501) staff       (20)    33486 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe.py
--rw-r--r--   0 mohan      (501) staff       (20)    16674 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe_create2_tx.py
--rw-r--r--   0 mohan      (501) staff       (20)    18510 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe_signature.py
--rw-r--r--   0 mohan      (501) staff       (20)    13004 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe_tx.py
--rw-r--r--   0 mohan      (501) staff       (20)     2563 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe_v1_0_0.py
--rw-r--r--   0 mohan      (501) staff       (20)     1073 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe_v1_3_0.py
--rw-r--r--   0 mohan      (501) staff       (20)     3731 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_serializers.py
--rw-r--r--   0 mohan      (501) staff       (20)     3711 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_signatures.py
--rw-r--r--   0 mohan      (501) staff       (20)      287 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/utils.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-24 08:02:58.628908 fs-attestation-safe-eth-py-1.0.0/gnosis/util/
--rw-r--r--   0 mohan      (501) staff       (20)       83 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/util/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     1003 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/util/http.py
--rw-r--r--   0 mohan      (501) staff       (20)      450 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/gnosis/util/util.py
--rw-r--r--   0 mohan      (501) staff       (20)     2530 2024-04-24 08:02:58.630292 fs-attestation-safe-eth-py-1.0.0/setup.cfg
--rw-r--r--   0 mohan      (501) staff       (20)       69 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.0/setup.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.684311 fs-attestation-safe-eth-py-1.0.1/
+-rw-r--r--   0 mohan      (501) staff       (20)     1082 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/LICENSE
+-rw-r--r--   0 mohan      (501) staff       (20)       71 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/MANIFEST.in
+-rw-r--r--   0 mohan      (501) staff       (20)     2234 2024-04-25 06:40:15.684529 fs-attestation-safe-eth-py-1.0.1/PKG-INFO
+-rw-r--r--   0 mohan      (501) staff       (20)      714 2024-04-25 06:38:40.000000 fs-attestation-safe-eth-py-1.0.1/README.rst
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.551139 fs-attestation-safe-eth-py-1.0.1/docs/
+-rw-r--r--   0 mohan      (501) staff       (20)      638 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/docs/Makefile
+-rw-r--r--   0 mohan      (501) staff       (20)      799 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/docs/make.bat
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.558171 fs-attestation-safe-eth-py-1.0.1/docs/source/
+-rw-r--r--   0 mohan      (501) staff       (20)     1987 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/docs/source/conf.py
+-rw-r--r--   0 mohan      (501) staff       (20)      978 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/docs/source/gnosis.eth.clients.rst
+-rw-r--r--   0 mohan      (501) staff       (20)      183 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/docs/source/gnosis.eth.contracts.rst
+-rw-r--r--   0 mohan      (501) staff       (20)      954 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/docs/source/gnosis.eth.django.rst
+-rw-r--r--   0 mohan      (501) staff       (20)      177 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/docs/source/gnosis.eth.eip712.rst
+-rw-r--r--   0 mohan      (501) staff       (20)     1198 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/docs/source/gnosis.eth.oracles.abis.rst
+-rw-r--r--   0 mohan      (501) staff       (20)      450 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/docs/source/gnosis.eth.oracles.rst
+-rw-r--r--   0 mohan      (501) staff       (20)      936 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/docs/source/gnosis.eth.rst
+-rw-r--r--   0 mohan      (501) staff       (20)      226 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/docs/source/gnosis.rst
+-rw-r--r--   0 mohan      (501) staff       (20)     1852 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/docs/source/gnosis.safe.rst
+-rw-r--r--   0 mohan      (501) staff       (20)      894 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/docs/source/index.rst
+-rw-r--r--   0 mohan      (501) staff       (20)       55 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/docs/source/modules.rst
+-rw-r--r--   0 mohan      (501) staff       (20)     8368 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/docs/source/quickstart.rst
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.561953 fs-attestation-safe-eth-py-1.0.1/fs_attestation_safe_eth_py.egg-info/
+-rw-r--r--   0 mohan      (501) staff       (20)     2234 2024-04-25 06:40:15.000000 fs-attestation-safe-eth-py-1.0.1/fs_attestation_safe_eth_py.egg-info/PKG-INFO
+-rw-r--r--   0 mohan      (501) staff       (20)     7536 2024-04-25 06:40:15.000000 fs-attestation-safe-eth-py-1.0.1/fs_attestation_safe_eth_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mohan      (501) staff       (20)        1 2024-04-25 06:40:15.000000 fs-attestation-safe-eth-py-1.0.1/fs_attestation_safe_eth_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mohan      (501) staff       (20)      129 2024-04-25 06:40:15.000000 fs-attestation-safe-eth-py-1.0.1/fs_attestation_safe_eth_py.egg-info/requires.txt
+-rw-r--r--   0 mohan      (501) staff       (20)        7 2024-04-25 06:40:15.000000 fs-attestation-safe-eth-py-1.0.1/fs_attestation_safe_eth_py.egg-info/top_level.txt
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.562985 fs-attestation-safe-eth-py-1.0.1/gnosis/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/__init__.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.565014 fs-attestation-safe-eth-py-1.0.1/gnosis/cowsap/
+-rw-r--r--   0 mohan      (501) staff       (20)      156 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/cowsap/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     8465 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/cowsap/cow_swap_api.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2700 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/cowsap/order.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.566135 fs-attestation-safe-eth-py-1.0.1/gnosis/cowsap/tests/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/cowsap/tests/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     5604 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/cowsap/tests/test_cow_swap_api.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.570194 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/
+-rw-r--r--   0 mohan      (501) staff       (20)     1064 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/__init__.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.574029 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/account_abstraction/
+-rw-r--r--   0 mohan      (501) staff       (20)      348 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/account_abstraction/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7060 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/account_abstraction/bundler_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)      986 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/account_abstraction/constants.py
+-rw-r--r--   0 mohan      (501) staff       (20)      208 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/account_abstraction/exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4259 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/account_abstraction/user_operation.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3357 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/account_abstraction/user_operation_receipt.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.577675 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/clients/
+-rw-r--r--   0 mohan      (501) staff       (20)      878 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/clients/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     9236 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/clients/blockscout_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)      194 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/clients/contract_metadata.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4839 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/clients/ens_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)     9677 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/clients/etherscan_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3345 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/clients/sourcify_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1020 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/constants.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.578734 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/
+-rw-r--r--   0 mohan      (501) staff       (20)    10273 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/__init__.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.611785 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/
+-rw-r--r--   0 mohan      (501) staff       (20)   328664 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/CPKFactory.json
+-rw-r--r--   0 mohan      (501) staff       (20)    28908 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_3_0.json
+-rw-r--r--   0 mohan      (501) staff       (20)    29485 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_4_1.json
+-rw-r--r--   0 mohan      (501) staff       (20)    26897 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/DelegateConstructorProxy.json
+-rw-r--r--   0 mohan      (501) staff       (20)    29068 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/ERC1155.json
+-rw-r--r--   0 mohan      (501) staff       (20)    54748 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/ERC20.json
+-rw-r--r--   0 mohan      (501) staff       (20)    89890 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/ERC20TestToken.json
+-rw-r--r--   0 mohan      (501) staff       (20)   622260 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/ERC721.json
+-rw-r--r--   0 mohan      (501) staff       (20)   983403 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/GnosisSafe_V0_0_1.json
+-rw-r--r--   0 mohan      (501) staff       (20)  1158944 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/GnosisSafe_V1_0_0.json
+-rw-r--r--   0 mohan      (501) staff       (20)  1347363 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/GnosisSafe_V1_1_1.json
+-rw-r--r--   0 mohan      (501) staff       (20)   119875 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/GnosisSafe_V1_3_0.json
+-rw-r--r--   0 mohan      (501) staff       (20)    19886 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/MultiSend.json
+-rw-r--r--   0 mohan      (501) staff       (20)    78793 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/PayingProxy.json
+-rw-r--r--   0 mohan      (501) staff       (20)   136946 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/ProxyFactory_V1_0_0.json
+-rw-r--r--   0 mohan      (501) staff       (20)   288861 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/ProxyFactory_V1_1_1.json
+-rw-r--r--   0 mohan      (501) staff       (20)    18975 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/ProxyFactory_V1_3_0.json
+-rw-r--r--   0 mohan      (501) staff       (20)    15538 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/ProxyFactory_V1_4_1.json
+-rw-r--r--   0 mohan      (501) staff       (20)    32495 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/Proxy_V1_0_0.json
+-rw-r--r--   0 mohan      (501) staff       (20)    39032 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/Proxy_V1_1_1.json
+-rw-r--r--   0 mohan      (501) staff       (20)     1862 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/Proxy_V1_3_0.json
+-rw-r--r--   0 mohan      (501) staff       (20)     1849 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/Proxy_V1_4_1.json
+-rw-r--r--   0 mohan      (501) staff       (20)   121611 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/Safe_V1_4_1.json
+-rw-r--r--   0 mohan      (501) staff       (20)     5069 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/SignMessageLib.json
+-rw-r--r--   0 mohan      (501) staff       (20)     4913 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/SimulateTxAccessor_V1_4_1.json
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7351 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/kyber_network_proxy.json
+-rw-r--r--   0 mohan      (501) staff       (20)    19012 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/multicall.py
+-rw-r--r--   0 mohan      (501) staff       (20)    17165 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/uniswap_exchange.json
+-rw-r--r--   0 mohan      (501) staff       (20)     2480 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/uniswap_factory.json
+-rw-r--r--   0 mohan      (501) staff       (20)     2242 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/uniswap_v2_factory.json
+-rw-r--r--   0 mohan      (501) staff       (20)     8293 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/uniswap_v2_pair.json
+-rw-r--r--   0 mohan      (501) staff       (20)    11889 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/uniswap_v2_router.json
+-rw-r--r--   0 mohan      (501) staff       (20)      954 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/contract_base.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.615056 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/django/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/django/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3735 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/django/admin.py
+-rw-r--r--   0 mohan      (501) staff       (20)      269 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/django/filters.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2435 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/django/forms.py
+-rw-r--r--   0 mohan      (501) staff       (20)     9936 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/django/models.py
+-rw-r--r--   0 mohan      (501) staff       (20)     6191 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/django/serializers.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.617577 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/django/tests/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/django/tests/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)      711 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/django/tests/models.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3028 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/django/tests/test_forms.py
+-rw-r--r--   0 mohan      (501) staff       (20)     8621 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/django/tests/test_models.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7877 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/django/tests/test_serializers.py
+-rw-r--r--   0 mohan      (501) staff       (20)      484 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/django/tests/test_validators.py
+-rw-r--r--   0 mohan      (501) staff       (20)      320 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/django/validators.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.618041 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/eip712/
+-rw-r--r--   0 mohan      (501) staff       (20)     5915 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/eip712/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)    82106 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/ethereum_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)    35545 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/ethereum_network.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1332 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)    13617 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/multicall.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.622657 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/
+-rw-r--r--   0 mohan      (501) staff       (20)     1093 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/__init__.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.628226 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/abis/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/abis/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)    15986 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/abis/aave_abis.py
+-rw-r--r--   0 mohan      (501) staff       (20)    30036 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/abis/balancer_abis.py
+-rw-r--r--   0 mohan      (501) staff       (20)    29731 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/abis/cream_abis.py
+-rw-r--r--   0 mohan      (501) staff       (20)    27567 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/abis/curve_abis.py
+-rw-r--r--   0 mohan      (501) staff       (20)    25872 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/abis/mooniswap_abis.py
+-rw-r--r--   0 mohan      (501) staff       (20)      239 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/abis/superfluid_abis.py
+-rw-r--r--   0 mohan      (501) staff       (20)    45208 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/abis/uniswap_v3.py
+-rw-r--r--   0 mohan      (501) staff       (20)    36257 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/abis/yearn_abis.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1464 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/abis/zerion_abis.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2375 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/cowswap.py
+-rw-r--r--   0 mohan      (501) staff       (20)      161 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/exceptions.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.629042 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/helpers/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/helpers/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     5856 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/helpers/curve_gauge_list.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4117 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/kyber.py
+-rw-r--r--   0 mohan      (501) staff       (20)    32169 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/oracles.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1677 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/superfluid.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1516 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/sushiswap.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7154 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/uniswap_v3.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1064 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/utils.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.631738 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/__init__.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.633869 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/account_abstraction/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/account_abstraction/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     6695 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/account_abstraction/test_bundler_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2727 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/account_abstraction/test_e2e_bundler_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)      671 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/account_abstraction/test_user_operation.py
+-rw-r--r--   0 mohan      (501) staff       (20)      947 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/account_abstraction/test_user_operation_receipt.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.636747 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/clients/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/clients/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)   107388 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/clients/mocks.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1047 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/clients/test_blockscout_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)     6185 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/clients/test_ens_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1686 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/clients/test_etherscan_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2521 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/clients/test_sourcify_client.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.637530 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/eip712/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/eip712/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)    13327 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/eip712/test_eip712.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3189 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/ethereum_test_case.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.644188 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/mocks/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/mocks/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)    29208 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/mocks/mock_bundler.py
+-rw-r--r--   0 mohan      (501) staff       (20)    31306 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/mocks/mock_internal_txs.py
+-rw-r--r--   0 mohan      (501) staff       (20)    10570 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/mocks/mock_log_receipts.py
+-rw-r--r--   0 mohan      (501) staff       (20)   792720 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/mocks/mock_trace_block.py
+-rw-r--r--   0 mohan      (501) staff       (20)    92795 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/mocks/mock_trace_filter.py
+-rw-r--r--   0 mohan      (501) staff       (20)   171076 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/mocks/mock_trace_transaction.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.649575 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/oracles/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/oracles/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2706 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/oracles/test_cowswap.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1820 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/oracles/test_kyber.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1460 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/oracles/test_superfluid.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2043 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/oracles/test_sushiswap.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3544 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/oracles/test_uniswap_v3.py
+-rw-r--r--   0 mohan      (501) staff       (20)    61025 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/test_ethereum_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7087 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/test_multicall.py
+-rw-r--r--   0 mohan      (501) staff       (20)    21137 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/test_oracles.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7287 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/test_utils.py
+-rw-r--r--   0 mohan      (501) staff       (20)     5069 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/utils.py
+-rw-r--r--   0 mohan      (501) staff       (20)      390 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/typing.py
+-rw-r--r--   0 mohan      (501) staff       (20)     6977 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/eth/utils.py
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/py.typed
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.661394 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/
+-rw-r--r--   0 mohan      (501) staff       (20)      742 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/__init__.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.662754 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/account_abstraction/
+-rw-r--r--   0 mohan      (501) staff       (20)      101 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/account_abstraction/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     5647 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/account_abstraction/safe_operation.py
+-rw-r--r--   0 mohan      (501) staff       (20)    63401 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/addresses.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.664792 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/api/
+-rw-r--r--   0 mohan      (501) staff       (20)      346 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/api/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2471 2024-04-24 04:21:12.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/api/base_api.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2913 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/api/relay_service_api.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.667778 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/api/transaction_service_api/
+-rw-r--r--   0 mohan      (501) staff       (20)      103 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/api/transaction_service_api/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)    14033 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/api/transaction_service_api/transaction_service_api.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1732 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/api/transaction_service_api/transaction_service_messages.py
+-rw-r--r--   0 mohan      (501) staff       (20)      252 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/api/transaction_service_api/transaction_service_tx.py
+-rw-r--r--   0 mohan      (501) staff       (20)      105 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/enums.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1451 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)    11459 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/multi_send.py
+-rw-r--r--   0 mohan      (501) staff       (20)    10479 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/proxy_factory.py
+-rw-r--r--   0 mohan      (501) staff       (20)    36823 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/safe.py
+-rw-r--r--   0 mohan      (501) staff       (20)    11975 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/safe_create2_tx.py
+-rw-r--r--   0 mohan      (501) staff       (20)     9736 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/safe_creator.py
+-rw-r--r--   0 mohan      (501) staff       (20)   121198 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/safe_deployments.py
+-rw-r--r--   0 mohan      (501) staff       (20)    12587 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/safe_signature.py
+-rw-r--r--   0 mohan      (501) staff       (20)    17225 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/safe_tx.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4194 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/serializers.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2000 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/signatures.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.678065 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/__init__.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.679015 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/account_abstraction/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/account_abstraction/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3469 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/account_abstraction/test_safe_operation.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.679942 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/api/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/api/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     5341 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/api/test_transaction_service_api.py
+-rw-r--r--   0 mohan      (501) staff       (20)    20692 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/safe_test_case.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1398 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_addresses.py
+-rw-r--r--   0 mohan      (501) staff       (20)    10515 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_multi_send.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.681666 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_proxy_factory/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_proxy_factory/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7798 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_proxy_factory/test_proxy_factory.py
+-rw-r--r--   0 mohan      (501) staff       (20)    33486 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_safe.py
+-rw-r--r--   0 mohan      (501) staff       (20)    16674 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_safe_create2_tx.py
+-rw-r--r--   0 mohan      (501) staff       (20)    18510 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_safe_signature.py
+-rw-r--r--   0 mohan      (501) staff       (20)    13004 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_safe_tx.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2563 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_safe_v1_0_0.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1073 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_safe_v1_3_0.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3731 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_serializers.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3711 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_signatures.py
+-rw-r--r--   0 mohan      (501) staff       (20)      287 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/utils.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:40:15.683427 fs-attestation-safe-eth-py-1.0.1/gnosis/util/
+-rw-r--r--   0 mohan      (501) staff       (20)       83 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/util/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1003 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/util/http.py
+-rw-r--r--   0 mohan      (501) staff       (20)      450 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/gnosis/util/util.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2446 2024-04-25 06:40:15.686011 fs-attestation-safe-eth-py-1.0.1/setup.cfg
+-rw-r--r--   0 mohan      (501) staff       (20)       69 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.1/setup.py
```

### Comparing `fs-attestation-safe-eth-py-1.0.0/LICENSE` & `fs-attestation-safe-eth-py-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/docs/Makefile` & `fs-attestation-safe-eth-py-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/docs/make.bat` & `fs-attestation-safe-eth-py-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/docs/source/conf.py` & `fs-attestation-safe-eth-py-1.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/docs/source/gnosis.eth.clients.rst` & `fs-attestation-safe-eth-py-1.0.1/docs/source/gnosis.eth.clients.rst`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/docs/source/gnosis.eth.django.rst` & `fs-attestation-safe-eth-py-1.0.1/docs/source/gnosis.eth.django.rst`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/docs/source/gnosis.eth.oracles.abis.rst` & `fs-attestation-safe-eth-py-1.0.1/docs/source/gnosis.eth.oracles.abis.rst`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/docs/source/gnosis.eth.rst` & `fs-attestation-safe-eth-py-1.0.1/docs/source/gnosis.eth.rst`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/docs/source/gnosis.safe.rst` & `fs-attestation-safe-eth-py-1.0.1/docs/source/gnosis.safe.rst`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/docs/source/index.rst` & `fs-attestation-safe-eth-py-1.0.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/docs/source/quickstart.rst` & `fs-attestation-safe-eth-py-1.0.1/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/fs_attestation_safe_eth_py.egg-info/SOURCES.txt` & `fs-attestation-safe-eth-py-1.0.1/fs_attestation_safe_eth_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/cowsap/cow_swap_api.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/cowsap/cow_swap_api.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/cowsap/order.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/cowsap/order.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/cowsap/tests/test_cow_swap_api.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/cowsap/tests/test_cow_swap_api.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/__init__.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/__init__.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/account_abstraction/bundler_client.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/account_abstraction/bundler_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/account_abstraction/constants.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/account_abstraction/constants.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/account_abstraction/user_operation.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/account_abstraction/user_operation.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/account_abstraction/user_operation_receipt.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/account_abstraction/user_operation_receipt.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/clients/__init__.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/clients/blockscout_client.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/clients/blockscout_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/clients/ens_client.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/clients/ens_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/clients/etherscan_client.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/clients/etherscan_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/clients/sourcify_client.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/clients/sourcify_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/constants.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/constants.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/__init__.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/CPKFactory.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/CPKFactory.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_3_0.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_4_1.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/DelegateConstructorProxy.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/DelegateConstructorProxy.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ERC1155.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/ERC1155.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ERC20.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/ERC20.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ERC20TestToken.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/ERC20TestToken.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ERC721.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/ERC721.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/GnosisSafe_V0_0_1.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/GnosisSafe_V0_0_1.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/GnosisSafe_V1_0_0.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/GnosisSafe_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/GnosisSafe_V1_1_1.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/GnosisSafe_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/GnosisSafe_V1_3_0.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/GnosisSafe_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/MultiSend.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/MultiSend.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/PayingProxy.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/PayingProxy.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ProxyFactory_V1_0_0.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/ProxyFactory_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ProxyFactory_V1_1_1.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/ProxyFactory_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ProxyFactory_V1_3_0.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/ProxyFactory_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ProxyFactory_V1_4_1.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/ProxyFactory_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/Proxy_V1_0_0.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/Proxy_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/Proxy_V1_1_1.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/Proxy_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/Proxy_V1_3_0.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/Proxy_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/Proxy_V1_4_1.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/Proxy_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/Safe_V1_4_1.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/Safe_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/SignMessageLib.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/SignMessageLib.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/SimulateTxAccessor_V1_4_1.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/SimulateTxAccessor_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/kyber_network_proxy.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/kyber_network_proxy.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/multicall.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/multicall.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/uniswap_exchange.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/uniswap_exchange.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/uniswap_factory.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/uniswap_factory.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/uniswap_v2_factory.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/uniswap_v2_factory.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/uniswap_v2_pair.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/uniswap_v2_pair.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/uniswap_v2_router.json` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/abis/uniswap_v2_router.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/contracts/contract_base.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/contracts/contract_base.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/django/admin.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/django/admin.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/django/forms.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/django/forms.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/django/models.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/django/models.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/django/serializers.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/django/serializers.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/django/tests/models.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/django/tests/models.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/django/tests/test_forms.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/django/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/django/tests/test_models.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/django/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/django/tests/test_serializers.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/django/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/eip712/__init__.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/eip712/__init__.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/ethereum_client.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/ethereum_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/ethereum_network.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/ethereum_network.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/exceptions.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/exceptions.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/multicall.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/multicall.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/__init__.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/__init__.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/aave_abis.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/abis/aave_abis.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/balancer_abis.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/abis/balancer_abis.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/cream_abis.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/abis/cream_abis.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/curve_abis.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/abis/curve_abis.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/mooniswap_abis.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/abis/mooniswap_abis.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/uniswap_v3.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/abis/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/yearn_abis.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/abis/yearn_abis.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/zerion_abis.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/abis/zerion_abis.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/cowswap.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/cowswap.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/helpers/curve_gauge_list.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/helpers/curve_gauge_list.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/kyber.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/kyber.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/oracles.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/oracles.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/superfluid.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/superfluid.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/sushiswap.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/sushiswap.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/uniswap_v3.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/oracles/utils.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/oracles/utils.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/account_abstraction/test_bundler_client.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/account_abstraction/test_bundler_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/account_abstraction/test_e2e_bundler_client.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/account_abstraction/test_e2e_bundler_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/account_abstraction/test_user_operation.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/account_abstraction/test_user_operation.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/account_abstraction/test_user_operation_receipt.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/account_abstraction/test_user_operation_receipt.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/clients/mocks.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/clients/mocks.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/clients/test_blockscout_client.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/clients/test_blockscout_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/clients/test_ens_client.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/clients/test_ens_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/clients/test_etherscan_client.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/clients/test_etherscan_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/clients/test_sourcify_client.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/clients/test_sourcify_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/eip712/test_eip712.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/eip712/test_eip712.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/ethereum_test_case.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/ethereum_test_case.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_bundler.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/mocks/mock_bundler.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_internal_txs.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/mocks/mock_internal_txs.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_log_receipts.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/mocks/mock_log_receipts.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_trace_block.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/mocks/mock_trace_block.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_trace_filter.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/mocks/mock_trace_filter.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_trace_transaction.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/mocks/mock_trace_transaction.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/test_cowswap.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/oracles/test_cowswap.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/test_kyber.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/oracles/test_kyber.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/test_superfluid.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/oracles/test_superfluid.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/test_sushiswap.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/oracles/test_sushiswap.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/test_uniswap_v3.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/oracles/test_uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/test_ethereum_client.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/test_ethereum_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/test_multicall.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/test_multicall.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/test_oracles.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/test_oracles.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/test_utils.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/tests/utils.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/tests/utils.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/eth/utils.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/eth/utils.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/__init__.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/__init__.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/account_abstraction/safe_operation.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/account_abstraction/safe_operation.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/addresses.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/addresses.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/api/base_api.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/api/base_api.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/api/relay_service_api.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/api/relay_service_api.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/api/transaction_service_api/transaction_service_api.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/api/transaction_service_api/transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/api/transaction_service_api/transaction_service_messages.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/api/transaction_service_api/transaction_service_messages.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/exceptions.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/exceptions.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/multi_send.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/multi_send.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/proxy_factory.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/proxy_factory.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/safe.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/safe.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/safe_create2_tx.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/safe_creator.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/safe_creator.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/safe_deployments.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/safe_deployments.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/safe_signature.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/safe_signature.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/safe_tx.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/safe_tx.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/serializers.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/serializers.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/signatures.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/signatures.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/account_abstraction/test_safe_operation.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/account_abstraction/test_safe_operation.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/api/test_transaction_service_api.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/api/test_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/safe_test_case.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/safe_test_case.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_addresses.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_addresses.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_multi_send.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_multi_send.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_proxy_factory/test_proxy_factory.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_proxy_factory/test_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_safe.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe_create2_tx.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe_signature.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_safe_signature.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe_tx.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_safe_tx.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe_v1_0_0.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_safe_v1_0_0.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe_v1_3_0.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_safe_v1_3_0.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_serializers.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/safe/tests/test_signatures.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/safe/tests/test_signatures.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/gnosis/util/http.py` & `fs-attestation-safe-eth-py-1.0.1/gnosis/util/http.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.0/setup.cfg` & `fs-attestation-safe-eth-py-1.0.1/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [metadata]
 name = fs-attestation-safe-eth-py
-version = 1.0.0
-description = Modified Safe Ecosystem Foundation utilities for Ethereum projects and FailSafe Attestation Service
+version = 1.0.1
+description = Modified safe-eth-py library version 6.0.0b25 to be used in FailSafe Attestation Service CLI. The original safe-eth-py is available here https://pypi.org/project/safe-eth-py/
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 keywords = 
 	ethereum
 	web3
 	django
 	safe
 	cowswap
 	gnosis
+	failsafe
+	failsafe-attestation-service
 url = https://github.com/safe-global/safe-eth-py
-author = Mohan
+author = Mohan | Team FailSafe | https://getfailsafe.com
 author_email = mohan@ethlas.com
 license = MIT License
 license_files = 
 	LICENSE
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
@@ -87,29 +89,11 @@
 python_version = 3.10
 check_untyped_defs = True
 ignore_missing_imports = True
 warn_unused_ignores = True
 warn_redundant_casts = True
 warn_unused_configs = True
 
-[coverage:report]
-exclude_lines = 
-	pragma: no cover
-	
-	raise NotImplementedError
-	
-	if __name__ == .__main__.:
-	if settings.DEBUG
-	
-	pass
-
-[coverage:run]
-include = safe_transaction_service/*
-omit = 
-	*__init__.py*
-	*tests*
-	*/migrations/*
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

