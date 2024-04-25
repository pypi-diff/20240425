# Comparing `tmp/syft-0.8.7b2.tar.gz` & `tmp/syft-0.8.7b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.7b2.tar", last modified: Sun Apr 21 12:50:56 2024, max compression
+gzip compressed data, was "syft-0.8.7b3.tar", last modified: Thu Apr 25 04:51:07 2024, max compression
```

## Comparing `syft-0.8.7b2.tar` & `syft-0.8.7b3.tar`

### file list

```diff
@@ -1,307 +1,309 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.808075 syft-0.8.7b2/
--rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-04-21 12:47:35.000000 syft-0.8.7b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-21 12:47:35.000000 syft-0.8.7b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    23134 2024-04-21 12:50:56.808075 syft-0.8.7b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18678 2024-04-21 12:48:43.000000 syft-0.8.7b2/PYPI.md
--rw-r--r--   0 runner    (1001) docker     (127)    17508 2024-04-21 12:47:35.000000 syft-0.8.7b2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-21 12:47:35.000000 syft-0.8.7b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-21 12:50:56.808075 syft-0.8.7b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-21 12:47:35.000000 syft-0.8.7b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.748079 syft-0.8.7b2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.752079 syft-0.8.7b2/src/syft/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-21 12:48:08.000000 syft-0.8.7b2/src/syft/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-04-21 12:48:08.000000 syft-0.8.7b2/src/syft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/abstract_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.756079 syft-0.8.7b2/src/syft/capnp/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/capnp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/capnp/iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.760079 syft-0.8.7b2/src/syft/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41860 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    37060 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)    18538 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/domain_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/enclave_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/gateway_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    16329 2024-04-21 12:49:56.000000 syft-0.8.7b2/src/syft/client/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/sync_decision.py
--rw-r--r--   0 runner    (1001) docker     (127)    12864 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/syncing.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/user_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.760079 syft-0.8.7b2/src/syft/custom_worker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/custom_worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/custom_worker/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/custom_worker/builder_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/custom_worker/builder_k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/custom_worker/builder_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/custom_worker/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/custom_worker/k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/custom_worker/runner_k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/custom_worker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.760079 syft-0.8.7b2/src/syft/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/exceptions/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/exceptions/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/gevent_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.760079 syft-0.8.7b2/src/syft/img/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/img/base64.py
--rw-r--r--   0 runner    (1001) docker     (127)    25535 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    41764 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/img/small-grid-symbol-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.764078 syft-0.8.7b2/src/syft/node/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/node/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/node/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/node/enclave.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/node/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    59989 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/node/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/node/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/node/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/node/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/node/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/node/worker_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.764078 syft-0.8.7b2/src/syft/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)    24381 2024-04-21 12:49:56.000000 syft-0.8.7b2/src/syft/protocol/data_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/protocol/protocol_version.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.764078 syft-0.8.7b2/src/syft/protocol/releases/
--rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/protocol/releases/0.8.2.json
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/protocol/releases/0.8.3.json
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/protocol/releases/0.8.4.json
--rw-r--r--   0 runner    (1001) docker     (127)    50490 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/protocol/releases/0.8.6.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.768078 syft-0.8.7b2/src/syft/serde/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/capnp.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/lib_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/lib_service_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)    12236 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/recursive.py
--rw-r--r--   0 runner    (1001) docker     (127)    12186 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/recursive_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/serializable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/signature.py
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/third_party.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.768078 syft-0.8.7b2/src/syft/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.772078 syft-0.8.7b2/src/syft/service/action/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/action_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/action_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    16790 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/action_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/action_graph_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    74031 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/action_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/action_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    38799 2024-04-21 12:49:57.000000 syft-0.8.7b2/src/syft/service/action/action_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/action_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/action_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.772078 syft-0.8.7b2/src/syft/service/api/
--rw-r--r--   0 runner    (1001) docker     (127)    20448 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13237 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/api/api_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/api/api_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.772078 syft-0.8.7b2/src/syft/service/blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/blob_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/blob_storage/remote_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    12511 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/blob_storage/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/blob_storage/stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.776077 syft-0.8.7b2/src/syft/service/code/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/code/code_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/code/status_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/code/unparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    55843 2024-04-21 12:49:57.000000 syft-0.8.7b2/src/syft/service/code/user_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/code/user_code_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    25113 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/code/user_code_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/code/user_code_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/code/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.776077 syft-0.8.7b2/src/syft/service/code_history/
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/code_history/code_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/code_history/code_history_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/code_history/code_history_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.776077 syft-0.8.7b2/src/syft/service/data_subject/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/data_subject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/data_subject/data_subject.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/data_subject/data_subject_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/data_subject/data_subject_member_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/data_subject/data_subject_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.776077 syft-0.8.7b2/src/syft/service/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28880 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/dataset/dataset_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/dataset/dataset_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.776077 syft-0.8.7b2/src/syft/service/enclave/
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/enclave/enclave_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.776077 syft-0.8.7b2/src/syft/service/job/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9408 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/job/job_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    24949 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/job/job_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.780077 syft-0.8.7b2/src/syft/service/log/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/log/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/log/log_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/log/log_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.780077 syft-0.8.7b2/src/syft/service/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/metadata/metadata_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/metadata/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/metadata/node_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.780077 syft-0.8.7b2/src/syft/service/network/
--rw-r--r--   0 runner    (1001) docker     (127)    30351 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/network/network_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    10813 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/network/node_peer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/network/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.780077 syft-0.8.7b2/src/syft/service/notification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14281 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/notification/email_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/notification/notification_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/notification/notification_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/notification/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.780077 syft-0.8.7b2/src/syft/service/notifier/
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/notifier/notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/notifier/notifier_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/notifier/notifier_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/notifier/notifier_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/notifier/smtp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.784077 syft-0.8.7b2/src/syft/service/object_search/
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/object_search/migration_state_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/object_search/object_migration_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.784077 syft-0.8.7b2/src/syft/service/output/
--rw-r--r--   0 runner    (1001) docker     (127)    11222 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/output/output_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.784077 syft-0.8.7b2/src/syft/service/policy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27131 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/policy/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/policy/policy_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/policy/user_policy_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.784077 syft-0.8.7b2/src/syft/service/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49644 2024-04-21 12:49:56.000000 syft-0.8.7b2/src/syft/service/project/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    15758 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/project/project_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/project/project_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.784077 syft-0.8.7b2/src/syft/service/queue/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/queue/base_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11250 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/queue/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/queue/queue_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/queue/queue_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    33929 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/queue/zmq_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.784077 syft-0.8.7b2/src/syft/service/request/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49867 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/request/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11273 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/request/request_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/request/request_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16874 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.788076 syft-0.8.7b2/src/syft/service/settings/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/settings/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/settings/settings_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/settings/settings_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.788076 syft-0.8.7b2/src/syft/service/sync/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50919 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/sync/diff_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    22083 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/sync/resolve_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/sync/sync_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/sync/sync_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/sync/sync_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.788076 syft-0.8.7b2/src/syft/service/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/user/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/user/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/user/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    20579 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/user/user_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/user/user_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.792076 syft-0.8.7b2/src/syft/service/worker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/image_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/image_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/image_registry_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/image_registry_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    22317 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/worker_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/worker_image_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/worker_image_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/worker_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    25273 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/worker_pool_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/worker_pool_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    11229 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/worker_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/worker_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/stable_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.792076 syft-0.8.7b2/src/syft/store/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.796076 syft-0.8.7b2/src/syft/store/blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/store/blob_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/store/blob_storage/on_disk.py
--rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/store/blob_storage/seaweedfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/store/dict_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    26587 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/store/document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-04-21 12:49:56.000000 syft-0.8.7b2/src/syft/store/kv_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/store/linked_obj.py
--rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/store/locks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/store/mongo_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/store/mongo_codecs.py
--rw-r--r--   0 runner    (1001) docker     (127)    37008 2024-04-21 12:49:57.000000 syft-0.8.7b2/src/syft/store/mongo_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    15863 2024-04-21 12:49:56.000000 syft-0.8.7b2/src/syft/store/sqlite_document_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.796076 syft-0.8.7b2/src/syft/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11929 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/cache_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/dicttuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/grid_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/syft_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/syft_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)    36866 2024-04-21 12:49:56.000000 syft-0.8.7b2/src/syft/types/syft_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/syncable_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/twin_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.800076 syft-0.8.7b2/src/syft/util/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/_std_stream_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/experimental_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/filterwarnings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/fonts.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/jax_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.800076 syft-0.8.7b2/src/syft/util/notebook_ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/notebook_ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.800076 syft-0.8.7b2/src/syft/util/notebook_ui/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/notebook_ui/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/notebook_ui/components/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/notebook_ui/components/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    33088 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/notebook_ui/notebook_addons.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/trace_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    24531 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.800076 syft-0.8.7b2/src/syft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23134 2024-04-21 12:50:56.000000 syft-0.8.7b2/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-04-21 12:50:56.000000 syft-0.8.7b2/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 12:50:56.000000 syft-0.8.7b2/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-21 12:50:56.000000 syft-0.8.7b2/src/syft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 12:48:09.000000 syft-0.8.7b2/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-21 12:50:56.000000 syft-0.8.7b2/src/syft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-21 12:50:56.000000 syft-0.8.7b2/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.878945 syft-0.8.7b3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-04-25 04:47:09.000000 syft-0.8.7b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-25 04:47:09.000000 syft-0.8.7b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23134 2024-04-25 04:51:07.878945 syft-0.8.7b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18678 2024-04-25 04:48:32.000000 syft-0.8.7b3/PYPI.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17508 2024-04-25 04:47:09.000000 syft-0.8.7b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-25 04:47:09.000000 syft-0.8.7b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-25 04:51:07.878945 syft-0.8.7b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-25 04:47:09.000000 syft-0.8.7b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.818946 syft-0.8.7b3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.822946 syft-0.8.7b3/src/syft/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-25 04:48:01.000000 syft-0.8.7b3/src/syft/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-25 04:48:01.000000 syft-0.8.7b3/src/syft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/abstract_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.826946 syft-0.8.7b3/src/syft/capnp/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/capnp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.830946 syft-0.8.7b3/src/syft/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42664 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37060 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18538 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/domain_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/enclave_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/gateway_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16329 2024-04-25 04:49:43.000000 syft-0.8.7b3/src/syft/client/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/sync_decision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19869 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/syncing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/user_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.830946 syft-0.8.7b3/src/syft/custom_worker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/custom_worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/custom_worker/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/custom_worker/builder_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13899 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/custom_worker/builder_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/custom_worker/builder_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/custom_worker/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/custom_worker/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/custom_worker/runner_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/custom_worker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.830946 syft-0.8.7b3/src/syft/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/exceptions/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/exceptions/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/gevent_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.830946 syft-0.8.7b3/src/syft/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/img/base64.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25535 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41764 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/img/small-grid-symbol-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.834946 syft-0.8.7b3/src/syft/node/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/node/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/node/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/node/enclave.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/node/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62557 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/node/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/node/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9289 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/node/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/node/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/node/worker_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.834946 syft-0.8.7b3/src/syft/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)    24797 2024-04-25 04:49:43.000000 syft-0.8.7b3/src/syft/protocol/data_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/protocol/protocol_version.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.834946 syft-0.8.7b3/src/syft/protocol/releases/
+-rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/protocol/releases/0.8.2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/protocol/releases/0.8.3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/protocol/releases/0.8.4.json
+-rw-r--r--   0 runner    (1001) docker     (127)    50490 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/protocol/releases/0.8.6.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.838946 syft-0.8.7b3/src/syft/serde/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/capnp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/lib_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/lib_service_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/recursive_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/third_party.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.838946 syft-0.8.7b3/src/syft/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.842946 syft-0.8.7b3/src/syft/service/action/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/action_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/action_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16790 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/action_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/action_graph_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74147 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/action_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/action_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39167 2024-04-25 04:49:43.000000 syft-0.8.7b3/src/syft/service/action/action_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/action_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/action_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.842946 syft-0.8.7b3/src/syft/service/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    23394 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20027 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/api/api_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/api/api_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.842946 syft-0.8.7b3/src/syft/service/blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/blob_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/blob_storage/remote_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12511 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/blob_storage/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/blob_storage/stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.846946 syft-0.8.7b3/src/syft/service/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/code/code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/code/status_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/code/unparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56015 2024-04-25 04:49:43.000000 syft-0.8.7b3/src/syft/service/code/user_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/code/user_code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25589 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/code/user_code_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/code/user_code_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/code/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.846946 syft-0.8.7b3/src/syft/service/code_history/
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/code_history/code_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/code_history/code_history_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/code_history/code_history_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.846946 syft-0.8.7b3/src/syft/service/data_subject/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/data_subject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/data_subject/data_subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/data_subject/data_subject_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/data_subject/data_subject_member_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/data_subject/data_subject_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.846946 syft-0.8.7b3/src/syft/service/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28880 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/dataset/dataset_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/dataset/dataset_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.846946 syft-0.8.7b3/src/syft/service/enclave/
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/enclave/enclave_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.850946 syft-0.8.7b3/src/syft/service/job/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/job/html_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/job/job_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32670 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/job/job_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.850946 syft-0.8.7b3/src/syft/service/log/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/log/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/log/log_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/log/log_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.850946 syft-0.8.7b3/src/syft/service/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/metadata/metadata_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/metadata/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/metadata/node_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.850946 syft-0.8.7b3/src/syft/service/network/
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/network/association_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29706 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/network/network_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10813 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/network/node_peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/network/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.850946 syft-0.8.7b3/src/syft/service/notification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14281 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/notification/email_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/notification/notification_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/notification/notification_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/notification/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.854946 syft-0.8.7b3/src/syft/service/notifier/
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/notifier/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/notifier/notifier_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/notifier/notifier_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/notifier/notifier_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/notifier/smtp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.854946 syft-0.8.7b3/src/syft/service/object_search/
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/object_search/migration_state_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/object_search/object_migration_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.854946 syft-0.8.7b3/src/syft/service/output/
+-rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/output/output_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.854946 syft-0.8.7b3/src/syft/service/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27131 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/policy/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/policy/policy_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/policy/user_policy_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.854946 syft-0.8.7b3/src/syft/service/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49644 2024-04-25 04:49:43.000000 syft-0.8.7b3/src/syft/service/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15758 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/project/project_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/project/project_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.854946 syft-0.8.7b3/src/syft/service/queue/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/queue/base_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/queue/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/queue/queue_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/queue/queue_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33929 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/queue/zmq_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.858945 syft-0.8.7b3/src/syft/service/request/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50424 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/request/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/request/request_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/request/request_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16887 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.858945 syft-0.8.7b3/src/syft/service/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/settings/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/settings/settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/settings/settings_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.858945 syft-0.8.7b3/src/syft/service/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52902 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/sync/diff_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20942 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/sync/resolve_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13943 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/sync/sync_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/sync/sync_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/sync/sync_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.858945 syft-0.8.7b3/src/syft/service/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/user/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/user/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21117 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/user/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/user/user_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.862945 syft-0.8.7b3/src/syft/service/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/image_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/image_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/image_registry_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/image_registry_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22317 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/worker_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/worker_image_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/worker_image_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/worker_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25273 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/worker_pool_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/worker_pool_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11229 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/worker_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/worker_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/stable_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.866945 syft-0.8.7b3/src/syft/store/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.866945 syft-0.8.7b3/src/syft/store/blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/store/blob_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/store/blob_storage/on_disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/store/blob_storage/seaweedfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/store/dict_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26587 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/store/document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-04-25 04:49:43.000000 syft-0.8.7b3/src/syft/store/kv_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/store/linked_obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/store/locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/store/mongo_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/store/mongo_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37008 2024-04-25 04:49:43.000000 syft-0.8.7b3/src/syft/store/mongo_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15863 2024-04-25 04:49:43.000000 syft-0.8.7b3/src/syft/store/sqlite_document_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.866945 syft-0.8.7b3/src/syft/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11929 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/cache_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/dicttuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/grid_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/syft_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/syft_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37820 2024-04-25 04:49:43.000000 syft-0.8.7b3/src/syft/types/syft_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/syncable_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/twin_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/uid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.870945 syft-0.8.7b3/src/syft/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/_std_stream_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/experimental_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/filterwarnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/fonts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/jax_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.870945 syft-0.8.7b3/src/syft/util/notebook_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/notebook_ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.874945 syft-0.8.7b3/src/syft/util/notebook_ui/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/notebook_ui/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/notebook_ui/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10867 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/notebook_ui/components/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34995 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/notebook_ui/notebook_addons.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/trace_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24531 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.874945 syft-0.8.7b3/src/syft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23134 2024-04-25 04:51:07.000000 syft-0.8.7b3/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-04-25 04:51:07.000000 syft-0.8.7b3/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 04:51:07.000000 syft-0.8.7b3/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-25 04:51:07.000000 syft-0.8.7b3/src/syft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 04:48:02.000000 syft-0.8.7b3/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-25 04:51:07.000000 syft-0.8.7b3/src/syft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 04:51:07.000000 syft-0.8.7b3/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.7b2/LICENSE` & `syft-0.8.7b3/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/PKG-INFO` & `syft-0.8.7b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.7b2
+Version: 0.8.7b3
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

### Comparing `syft-0.8.7b2/PYPI.md` & `syft-0.8.7b3/PYPI.md`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/README.md` & `syft-0.8.7b3/README.md`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/setup.cfg` & `syft-0.8.7b3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.7-beta.2"
+version = attr: "0.8.7-beta.3"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: PYPI.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
```

### Comparing `syft-0.8.7b2/src/syft/VERSION` & `syft-0.8.7b3/src/syft/VERSION`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.7-beta.2"
+__version__ = "0.8.7-beta.3"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.7b2/src/syft/__init__.py` & `syft-0.8.7b3/src/syft/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.7-beta.2"
+__version__ = "0.8.7-beta.3"
 
 # stdlib
 from collections.abc import Callable
 import pathlib
 from pathlib import Path
 import sys
 from typing import Any
@@ -42,17 +42,16 @@
 from .serde.serializable import serializable  # noqa: F401
 from .serde.serialize import _serialize as serialize  # noqa: F401
 from .service.action.action_data_empty import ActionDataEmpty  # noqa: F401
 from .service.action.action_object import ActionObject  # noqa: F401
 from .service.action.plan import Plan  # noqa: F401
 from .service.action.plan import planify  # noqa: F401
 from .service.api.api import api_endpoint  # noqa: F401
+from .service.api.api import api_endpoint_method  # noqa: F401
 from .service.api.api import create_new_api_endpoint as TwinAPIEndpoint  # noqa: F401
-from .service.api.api import mock_api_endpoint  # noqa: F401
-from .service.api.api import private_api_endpoint  # noqa: F401
 from .service.code.user_code import UserCodeStatus  # noqa: F401; noqa: F401
 from .service.code.user_code import syft_function  # noqa: F401; noqa: F401
 from .service.code.user_code import syft_function_single_use  # noqa: F401; noqa: F401
 from .service.data_subject import DataSubjectCreate as DataSubject  # noqa: F401
 from .service.dataset.dataset import Contributor  # noqa: F401
 from .service.dataset.dataset import CreateAsset as Asset  # noqa: F401
 from .service.dataset.dataset import CreateDataset as Dataset  # noqa: F401
```

### Comparing `syft-0.8.7b2/src/syft/abstract_node.py` & `syft-0.8.7b3/src/syft/abstract_node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/client/api.py` & `syft-0.8.7b3/src/syft/client/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,15 +249,15 @@
 
         args, kwargs = migrate_args_and_kwargs(
             to_protocol=self.communication_protocol, args=args, kwargs=kwargs
         )
 
         return args, kwargs
 
-    def __function_call(
+    def function_call(
         self, path: str, *args: Any, cache_result: bool = True, **kwargs: Any
     ) -> Any:
         if "blocking" in self.signature.parameters:
             raise Exception(
                 f"Signature {self.signature} can't have 'blocking' kwarg because it's reserved"
             )
 
@@ -292,28 +292,54 @@
         result, _ = migrate_args_and_kwargs(
             [result], kwargs={}, to_latest_protocol=True
         )
         result = result[0]
         return result
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
-        return self.__function_call(self.path, *args, **kwargs)
+        return self.function_call(self.path, *args, **kwargs)
 
-    def mock(self, *args: Any, **kwargs: Any) -> Any:
+    @property
+    def mock(self) -> Any:
         if self.custom_function:
-            return self.__function_call("api.call_public", *args, **kwargs)
+            remote_func = self
+
+            class PrivateCustomAPIReference:
+                def __call__(self, *args: Any, **kwargs: Any) -> Any:
+                    return remote_func.function_call(
+                        "api.call_public_in_jobs", *args, **kwargs
+                    )
+
+                @property
+                def context(self) -> Any:
+                    return remote_func.function_call("api.get_public_context")
+
+            return PrivateCustomAPIReference()
         return SyftError(
-            message="This function doesn't support public/private calls as it's not custom."
+            message="This function doesn't support mock/private calls as it's not custom."
         )
 
-    def private(self, *args: Any, **kwargs: Any) -> Any:
+    @property
+    def private(self) -> Any:
         if self.custom_function:
-            return self.__function_call("api.call_private", *args, **kwargs)
+            remote_func = self
+
+            class PrivateCustomAPIReference:
+                def __call__(self, *args: Any, **kwargs: Any) -> Any:
+                    return remote_func.function_call(
+                        "api.call_private_in_jobs", *args, **kwargs
+                    )
+
+                @property
+                def context(self) -> Any:
+                    return remote_func.function_call("api.get_private_context")
+
+            return PrivateCustomAPIReference()
         return SyftError(
-            message="This function doesn't support public/private calls as it's not custom."
+            message="This function doesn't support mock/private calls as it's not custom."
         )
 
     def custom_function_actionobject_id(self) -> UID | SyftError:
         if self.custom_function and self.pre_kwargs is not None:
             custom_path = self.pre_kwargs.get("path", "")
             api_call = SyftAPICall(
                 node_uid=self.node_uid,
@@ -339,15 +365,15 @@
             endpoint = self.make_call(api_call=api_call)
             if isinstance(endpoint, SyftError):
                 return endpoint._repr_html_()
 
             str_repr = "## API: " + custom_path + "\n"
             str_repr += (
                 "### Description: "
-                + f'<span style="font-weight: normal;">{endpoint.description}</span><br>'
+                + f'<span style="font-weight: lighter;">{endpoint.description}</span><br>'
                 + "\n"
             )
             str_repr += "#### Private Code:\n"
             str_repr += as_markdown_python_code(endpoint.private_function) + "\n"
             if endpoint.private_helper_functions:
                 str_repr += "##### Helper Functions:\n"
                 for helper_function in endpoint.private_helper_functions:
@@ -450,15 +476,15 @@
             make_call=make_call,
             pre_kwargs=pre_kwargs,
             communication_protocol=communication_protocol,
             warning=warning,
             user_code_id=pre_kwargs["uid"],
         )
     else:
-        custom_function = bool(path == "api.call")
+        custom_function = bool(path == "api.call_in_jobs")
         remote_function = RemoteFunction(
             node_uid=node_uid,
             signature=signature,
             path=path,
             make_call=make_call,
             pre_kwargs=pre_kwargs,
             communication_protocol=communication_protocol,
@@ -819,15 +845,15 @@
             endpoints[unique_path] = endpoint
 
         # get admin defined custom api endpoints
         method = node.get_method_with_context(APIService.get_endpoints, context)
         custom_endpoints = method()
         for custom_endpoint in custom_endpoints:
             pre_kwargs = {"path": custom_endpoint.path}
-            service_path = "api.call"
+            service_path = "api.call_in_jobs"
             path = custom_endpoint.path
             api_end = custom_endpoint.path.split(".")[-1]
             endpoint = APIEndpoint(
                 service_path=service_path,
                 module_path=path,
                 name=api_end,
                 description="",
```

### Comparing `syft-0.8.7b2/src/syft/client/client.py` & `syft-0.8.7b3/src/syft/client/client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/client/connection.py` & `syft-0.8.7b3/src/syft/client/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/client/deploy.py` & `syft-0.8.7b3/src/syft/client/deploy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/client/domain_client.py` & `syft-0.8.7b3/src/syft/client/domain_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/client/enclave_client.py` & `syft-0.8.7b3/src/syft/client/enclave_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/client/gateway_client.py` & `syft-0.8.7b3/src/syft/client/gateway_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/client/registry.py` & `syft-0.8.7b3/src/syft/client/registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/client/search.py` & `syft-0.8.7b3/src/syft/client/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/client/user_settings.py` & `syft-0.8.7b3/src/syft/client/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/custom_worker/builder.py` & `syft-0.8.7b3/src/syft/custom_worker/builder.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/custom_worker/builder_docker.py` & `syft-0.8.7b3/src/syft/custom_worker/builder_docker.py`

 * *Files 16% similar despite different names*

```diff
@@ -49,17 +49,17 @@
                 image_hash=image_result.id,
                 logs=self._parse_output(logs),
             )
 
     def push_image(
         self,
         tag: str,
-        username: str,
-        password: str,
         registry_url: str,
+        username: str | None = None,
+        password: str | None = None,
         **kwargs: Any,
     ) -> ImagePushResult:
         with contextlib.closing(docker.from_env()) as client:
             if registry_url and username and password:
                 client.login(
                     username=username,
                     password=password,
```

### Comparing `syft-0.8.7b2/src/syft/custom_worker/builder_k8s.py` & `syft-0.8.7b3/src/syft/custom_worker/builder_k8s.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 # stdlib
 from hashlib import sha256
 from pathlib import Path
+from secrets import token_hex
 from typing import Any
 
 # third party
 from kr8s.objects import ConfigMap
 from kr8s.objects import Job
 from kr8s.objects import Secret
 
 # relative
 from .builder_types import BUILD_IMAGE_TIMEOUT_SEC
 from .builder_types import BuilderBase
 from .builder_types import ImageBuildResult
 from .builder_types import ImagePushResult
 from .builder_types import PUSH_IMAGE_TIMEOUT_SEC
 from .k8s import INTERNAL_REGISTRY_HOST
-from .k8s import JOB_COMPLETION_TTL
 from .k8s import KUBERNETES_NAMESPACE
 from .k8s import KubeUtils
+from .k8s import USE_INTERNAL_REGISTRY
 from .k8s import get_kr8s_client
 from .utils import ImageUtils
 
 __all__ = ["KubernetesBuilder"]
 
 
 class BuildFailed(Exception):
     pass
 
 
 class KubernetesBuilder(BuilderBase):
+    # app.kubernetes.io/component
     COMPONENT = "builder"
 
+    # service account for the Job, useful for workload identity
+    SERVICE_ACCOUNT = "builder-service-account"
+
+    # Time after which Job will be deleted
+    JOB_COMPLETION_TTL = 60
+
     def __init__(self) -> None:
         self.client = get_kr8s_client()
 
     def build_image(
         self,
         tag: str,
         dockerfile: str | None = None,
@@ -42,31 +50,43 @@
         buildargs: dict | None = None,
         **kwargs: Any,
     ) -> ImageBuildResult:
         image_digest = None
         logs = None
         config = None
         job_id = self._new_job_id(tag)
+        kaniko_extra_args = None
 
         if dockerfile:
             pass
         elif dockerfile_path:
             dockerfile = dockerfile_path.read_text()
 
+        if USE_INTERNAL_REGISTRY:
+            # if we are using internal registry, we tweak the tag to point to it
+            tag = ImageUtils.change_registry(tag, registry=INTERNAL_REGISTRY_HOST)
+
+            # and let kaniko know about the internal registry
+            kaniko_extra_args = [
+                f"--insecure-registry={INTERNAL_REGISTRY_HOST}",
+                f"--skip-tls-verify-registry={INTERNAL_REGISTRY_HOST}",
+            ]
+
         try:
             # Create a ConfigMap with the Dockerfile
             config = self._create_build_config(job_id, dockerfile)
             config.refresh()
 
             # Create and start the job
             job = self._create_kaniko_build_job(
                 job_id=job_id,
                 tag=tag,
                 job_config=config,
                 build_args=buildargs,
+                kaniko_extra_args=kaniko_extra_args,
             )
 
             # wait for job to complete/fail
             job.wait(
                 ["condition=Complete", "condition=Failed"],
                 timeout=BUILD_IMAGE_TIMEOUT_SEC,
             )
@@ -93,30 +113,41 @@
             image_hash=image_digest,
             logs=logs,
         )
 
     def push_image(
         self,
         tag: str,
-        username: str,
-        password: str,
         registry_url: str,
+        username: str | None = None,
+        password: str | None = None,
         **kwargs: Any,
     ) -> ImagePushResult:
         exit_code = 1
         logs = None
         job_id = self._new_job_id(tag)
         push_secret = None
+        registry_auths = []
+
+        if USE_INTERNAL_REGISTRY:
+            # local registry auth can be anything
+            registry_auths.append((INTERNAL_REGISTRY_HOST, "admin", token_hex(4)))
+        else:
+            # kaniko has already pushed the image directly
+            return ImagePushResult(logs="Already pushed", exit_code=0)
+
+        # if we have external registry credentials, add them to the list
+        # elsea leave it for workload identity
+        if username and password:
+            registry_auths.append((registry_url, username, password))
 
         try:
             push_secret = self._create_push_secret(
-                id=job_id,
-                url=registry_url,
-                username=username,
-                password=password,
+                job_id=job_id,
+                registry_auths=registry_auths,
             )
             push_secret.refresh()
 
             job = self._create_push_job(
                 job_id=job_id,
                 tag=tag,
                 push_secret=push_secret,
@@ -176,21 +207,21 @@
 
     def _create_kaniko_build_job(
         self,
         job_id: str,
         tag: str,
         job_config: ConfigMap,
         build_args: dict | None = None,
+        kaniko_extra_args: list[str] | None = None,
     ) -> Job:
         # for push
         build_args = build_args or {}
+        kaniko_extra_args = kaniko_extra_args or []
         build_args_list = []
 
-        internal_tag = ImageUtils.change_registry(tag, registry=INTERNAL_REGISTRY_HOST)
-
         for k, v in build_args.items():
             build_args_list.append(f'--build-arg="{k}={v}"')
 
         job = Job(
             {
                 "metadata": {
                     "name": f"build-{job_id}",
@@ -198,61 +229,49 @@
                         "app.kubernetes.io/name": KUBERNETES_NAMESPACE,
                         "app.kubernetes.io/component": KubernetesBuilder.COMPONENT,
                         "app.kubernetes.io/managed-by": "kr8s",
                     },
                 },
                 "spec": {
                     "backoffLimit": 0,
-                    "ttlSecondsAfterFinished": JOB_COMPLETION_TTL,
+                    "ttlSecondsAfterFinished": KubernetesBuilder.JOB_COMPLETION_TTL,
                     "template": {
                         "spec": {
                             "restartPolicy": "Never",
+                            "serviceAccountName": KubernetesBuilder.SERVICE_ACCOUNT,
                             "containers": [
                                 {
                                     "name": "kaniko",
                                     "image": "gcr.io/kaniko-project/executor:latest",
                                     "args": [
                                         "--dockerfile=Dockerfile",
                                         "--context=dir:///workspace",
-                                        f"--destination={internal_tag}",
+                                        f"--destination={tag}",
                                         # Disabling --reproducible because it eats up a lot of CPU+RAM
                                         # https://github.com/GoogleContainerTools/kaniko/issues/1960
                                         # https://github.com/GoogleContainerTools/kaniko/pull/2477
                                         # "--reproducible",
-                                        # cache args
+                                        # Cache
                                         "--cache=true",
                                         "--cache-copy-layers",
                                         "--cache-run-layers",
-                                        f"--cache-repo={INTERNAL_REGISTRY_HOST}/builder-cache",
                                         # outputs args
                                         "--digest-file=/dev/termination-log",
                                         # other kaniko conf
-                                        f"--insecure-registry={INTERNAL_REGISTRY_HOST}",
-                                        f"--skip-tls-verify-registry={INTERNAL_REGISTRY_HOST}",
                                         "--log-format=text",
                                         "--verbosity=info",
                                     ]
+                                    + kaniko_extra_args
                                     + build_args_list,
                                     "volumeMounts": [
                                         {
                                             "name": "build-input",
                                             "mountPath": "/workspace",
                                         },
                                     ],
-                                    "resources": {
-                                        "requests": {
-                                            "memory": "4Gi",
-                                            "cpu": "2",
-                                        },
-                                        "limits": {
-                                            "memory": "16Gi",
-                                            "cpu": "4",
-                                        },
-                                        "ephemeral-storage": "10Gi",
-                                    },
                                 }
                             ],
                             "volumes": [
                                 {
                                     "name": "build-input",
                                     "configMap": {
                                         "name": job_config.metadata.name,
@@ -275,19 +294,19 @@
     ) -> Job:
         internal_tag = ImageUtils.change_registry(tag, registry=INTERNAL_REGISTRY_HOST)
         internal_reg, internal_repo, _ = ImageUtils.parse_tag(internal_tag)
 
         run_cmds = [
             # push with credentials
             "echo Pushing image...",
-            f"crane copy {internal_tag} {tag}",
+            f"krane copy {internal_tag} {tag}",
             # cleanup image from internal registry
             "echo Cleaning up...",
-            f"IMG_DIGEST=$(crane digest {internal_tag})",
-            f"crane delete {internal_reg}/{internal_repo}@$IMG_DIGEST; echo Done",
+            f"IMG_DIGEST=$(krane digest {internal_tag})",
+            f"krane delete {internal_reg}/{internal_repo}@$IMG_DIGEST; echo Done",
         ]
 
         job = Job(
             {
                 "metadata": {
                     # there should be only one push at a time, so keep this name unique to a push
                     "name": f"push-{job_id}",
@@ -295,44 +314,34 @@
                         "app.kubernetes.io/name": KUBERNETES_NAMESPACE,
                         "app.kubernetes.io/component": KubernetesBuilder.COMPONENT,
                         "app.kubernetes.io/managed-by": "kr8s",
                     },
                 },
                 "spec": {
                     "backoffLimit": 0,
-                    "ttlSecondsAfterFinished": JOB_COMPLETION_TTL,
+                    "ttlSecondsAfterFinished": KubernetesBuilder.JOB_COMPLETION_TTL,
                     "template": {
                         "spec": {
                             "restartPolicy": "Never",
+                            "serviceAccountName": KubernetesBuilder.SERVICE_ACCOUNT,
                             "containers": [
                                 {
                                     "name": "crane",
                                     # debug is needed for "sh" to be available
-                                    "image": "gcr.io/go-containerregistry/crane:debug",
+                                    "image": "gcr.io/go-containerregistry/krane:debug",
                                     "command": ["sh"],
                                     "args": ["-c", " && ".join(run_cmds)],
                                     "volumeMounts": [
                                         {
                                             "name": "push-secret",
                                             "mountPath": "/root/.docker/config.json",
                                             "subPath": "config.json",
                                             "readOnly": True,
                                         },
                                     ],
-                                    "resources": {
-                                        "requests": {
-                                            "memory": "2Gi",
-                                            "cpu": "1",
-                                        },
-                                        "limits": {
-                                            "memory": "4Gi",
-                                            "cpu": "2",
-                                            "ephemeral-storage": "1Gi",
-                                        },
-                                    },
                                 }
                             ],
                             "volumes": [
                                 {
                                     "name": "push-secret",
                                     "secret": {
                                         "secretName": push_secret.metadata.name,
@@ -349,18 +358,16 @@
                     },
                 },
             }
         )
         return KubeUtils.create_or_get(job)
 
     def _create_push_secret(
-        self, id: str, url: str, username: str, password: str
+        self,
+        job_id: str,
+        registry_auths: list[tuple[str, str, str]],
     ) -> Secret:
         return KubeUtils.create_dockerconfig_secret(
-            secret_name=f"push-secret-{id}",
+            secret_name=f"push-secret-{job_id}",
             component=KubernetesBuilder.COMPONENT,
-            registries=[
-                # TODO: authorize internal registry?
-                (INTERNAL_REGISTRY_HOST, "username", id),
-                (url, username, password),
-            ],
+            registries=registry_auths,
         )
```

### Comparing `syft-0.8.7b2/src/syft/custom_worker/builder_types.py` & `syft-0.8.7b3/src/syft/custom_worker/builder_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,13 +42,13 @@
     ) -> ImageBuildResult:
         pass
 
     @abstractmethod
     def push_image(
         self,
         tag: str,
-        username: str,
-        password: str,
         registry_url: str,
+        username: str | None = None,
+        password: str | None = None,
         **kwargs: Any,
     ) -> ImagePushResult:
         pass
```

### Comparing `syft-0.8.7b2/src/syft/custom_worker/config.py` & `syft-0.8.7b3/src/syft/custom_worker/config.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/custom_worker/k8s.py` & `syft-0.8.7b3/src/syft/custom_worker/k8s.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 import kr8s
 from kr8s.objects import APIObject
 from kr8s.objects import Pod
 from kr8s.objects import Secret
 from pydantic import BaseModel
 from typing_extensions import Self
 
-# Time after which Job will be deleted
-JOB_COMPLETION_TTL = 60
-
 # Kubernetes namespace
 KUBERNETES_NAMESPACE = os.getenv("K8S_NAMESPACE", "syft")
 
 # Kubernetes runtime flag
 IN_KUBERNETES = os.getenv("CONTAINER_HOST") == "k8s"
 
+# skip pushing to internal registry
+USE_INTERNAL_REGISTRY = os.getenv("USE_INTERNAL_REGISTRY", "true").lower() == "true"
+
 # Internal registry URL
 DEFAULT_INTERNAL_REGISTRY = f"registry.{KUBERNETES_NAMESPACE}.svc.cluster.local"
 INTERNAL_REGISTRY_HOST = os.getenv("INTERNAL_REGISTRY_HOST", DEFAULT_INTERNAL_REGISTRY)
 
 
 class PodPhase(Enum):
     Pending = "Pending"
```

### Comparing `syft-0.8.7b2/src/syft/custom_worker/runner_k8s.py` & `syft-0.8.7b3/src/syft/custom_worker/runner_k8s.py`

 * *Files 5% similar despite different names*

```diff
@@ -205,14 +205,16 @@
                         "metadata": {
                             "labels": {
                                 "app.kubernetes.io/name": KUBERNETES_NAMESPACE,
                                 "app.kubernetes.io/component": pool_name,
                             }
                         },
                         "spec": {
+                            # TODO: make this configurable
+                            "serviceAccountName": "backend-service-account",
                             "containers": [
                                 {
                                     "name": pool_name,
                                     "imagePullPolicy": "IfNotPresent",
                                     "image": tag,
                                     "env": env_vars,
                                     "volumeMounts": volume_mounts,
```

### Comparing `syft-0.8.7b2/src/syft/custom_worker/utils.py` & `syft-0.8.7b3/src/syft/custom_worker/utils.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/exceptions/exception.py` & `syft-0.8.7b3/src/syft/exceptions/exception.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/gevent_patch.py` & `syft-0.8.7b3/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/img/logo.png` & `syft-0.8.7b3/src/syft/img/logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/img/small-grid-symbol-logo.png` & `syft-0.8.7b3/src/syft/img/small-grid-symbol-logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/node/credentials.py` & `syft-0.8.7b3/src/syft/node/credentials.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/node/node.py` & `syft-0.8.7b3/src/syft/node/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,26 +73,27 @@
 from ..service.project.project_service import ProjectService
 from ..service.queue.base_queue import AbstractMessageHandler
 from ..service.queue.base_queue import QueueConsumer
 from ..service.queue.base_queue import QueueProducer
 from ..service.queue.queue import APICallMessageHandler
 from ..service.queue.queue import QueueManager
 from ..service.queue.queue_service import QueueService
+from ..service.queue.queue_stash import APIEndpointQueueItem
 from ..service.queue.queue_stash import ActionQueueItem
 from ..service.queue.queue_stash import QueueItem
 from ..service.queue.queue_stash import QueueStash
 from ..service.queue.zmq_queue import QueueConfig
 from ..service.queue.zmq_queue import ZMQClientConfig
 from ..service.queue.zmq_queue import ZMQQueueConfig
 from ..service.request.request_service import RequestService
 from ..service.response import SyftError
 from ..service.service import AbstractService
 from ..service.service import ServiceConfigRegistry
 from ..service.service import UserServiceConfigRegistry
-from ..service.settings.settings import NodeSettingsV2
+from ..service.settings.settings import NodeSettings
 from ..service.settings.settings_service import SettingsService
 from ..service.settings.settings_stash import SettingsStash
 from ..service.sync.sync_service import SyncService
 from ..service.user.user import User
 from ..service.user.user import UserCreate
 from ..service.user.user_roles import ServiceRole
 from ..service.user.user_service import UserService
@@ -314,14 +315,15 @@
         migrate: bool = False,
         in_memory_workers: bool = True,
         smtp_username: str | None = None,
         smtp_password: str | None = None,
         email_sender: str | None = None,
         smtp_port: int | None = None,
         smtp_host: str | None = None,
+        association_request_auto_approval: bool = False,
     ):
         # 🟡 TODO 22: change our ENV variable format and default init args to make this
         # less horrible or add some convenience functions
         self.dev_mode = dev_mode or get_dev_mode()
         self.id = UID.from_string(node_uid_env) if node_uid_env else (id or UID())
         self.packages = ""
         self.processes = processes
@@ -347,14 +349,16 @@
             skey = SyftSigningKey.from_string(signing_key_env)
         elif isinstance(signing_key, SigningKey):
             skey = SyftSigningKey(signing_key=signing_key)
         else:
             skey = signing_key
         self.signing_key = skey or SyftSigningKey.generate()
 
+        self.association_request_auto_approval = association_request_auto_approval
+
         self.queue_config = self.create_queue_config(
             n_consumers=n_consumers,
             create_producer=create_producer,
             thread_workers=thread_workers,
             queue_port=queue_port,
             queue_config=queue_config,
         )
@@ -415,18 +419,19 @@
             os.path.exists("/.dockerenv")
             or os.path.isfile(path)
             and any("docker" in line for line in open(path))
         )
 
     def get_default_store(self, use_sqlite: bool) -> StoreConfig:
         if use_sqlite:
+            path = self.get_temp_dir("db")
             return SQLiteStoreConfig(
                 client_config=SQLiteStoreClientConfig(
                     filename=f"{self.id}.sqlite",
-                    path=self.get_temp_dir("db"),
+                    path=path,
                 )
             )
         return DictStoreConfig()
 
     def init_blob_storage(self, config: BlobStorageConfig | None = None) -> None:
         if config is None:
             client_config = OnDiskBlobStorageClientConfig(
@@ -576,14 +581,15 @@
         n_consumers: int = 0,
         thread_workers: bool = False,
         create_producer: bool = False,
         queue_port: int | None = None,
         dev_mode: bool = False,
         migrate: bool = False,
         in_memory_workers: bool = True,
+        association_request_auto_approval: bool = False,
     ) -> Self:
         uid = UID.with_seed(name)
         name_hash = hashlib.sha256(name.encode("utf8")).digest()
         key = SyftSigningKey(signing_key=SigningKey(name_hash))
         blob_storage_config = None
 
         node_type = NodeType(node_type)
@@ -603,14 +609,15 @@
             n_consumers=n_consumers,
             thread_workers=thread_workers,
             create_producer=create_producer,
             dev_mode=dev_mode,
             migrate=migrate,
             in_memory_workers=in_memory_workers,
             reset=reset,
+            association_request_auto_approval=association_request_auto_approval,
         )
 
     def is_root(self, credentials: SyftVerifyKey) -> bool:
         return credentials == self.verify_key
 
     @property
     def root_client(self) -> SyftClient:
@@ -940,15 +947,15 @@
         Remove the temporary directory for this node.
         """
         rootdir = self.get_temp_dir()
         if rootdir.exists():
             shutil.rmtree(rootdir, ignore_errors=True)
 
     @property
-    def settings(self) -> NodeSettingsV2:
+    def settings(self) -> NodeSettings:
         settings_stash = SettingsStash(store=self.document_store)
         if self.signing_key is None:
             raise ValueError(f"{self} has no signing key")
         settings = settings_stash.get_all(self.signing_key.verify_key)
         if settings.is_ok() and len(settings.ok()) > 0:
             settings_data = settings.ok()[0]
         return settings_data
@@ -1188,14 +1195,53 @@
                 result = SyftError(
                     message=f"Exception calling {api_call.path}. {traceback.format_exc()}"
                 )
         else:
             return self.add_api_call_to_queue(api_call)
         return result
 
+    def add_api_endpoint_execution_to_queue(
+        self,
+        credentials: SyftVerifyKey,
+        method: str,
+        path: str,
+        *args: Any,
+        worker_pool: str | None = None,
+        **kwargs: Any,
+    ) -> Job | SyftError:
+        job_id = UID()
+        task_uid = UID()
+        worker_settings = WorkerSettings.from_node(node=self)
+
+        if worker_pool is None:
+            worker_pool = self.get_default_worker_pool()
+        else:
+            worker_pool = self.get_worker_pool_by_name(worker_pool)
+
+        # Create a Worker pool reference object
+        worker_pool_ref = LinkedObject.from_obj(
+            worker_pool,
+            service_type=SyftWorkerPoolService,
+            node_uid=self.id,
+        )
+        queue_item = APIEndpointQueueItem(
+            id=task_uid,
+            method=method,
+            node_uid=self.id,
+            syft_client_verify_key=credentials,
+            syft_node_location=self.id,
+            job_id=job_id,
+            worker_settings=worker_settings,
+            args=args,
+            kwargs={"path": path, **kwargs},
+            has_execute_permissions=True,
+            worker_pool=worker_pool_ref,  # set worker pool reference as part of queue item
+        )
+        return self.add_queueitem_to_queue(queue_item, credentials, None, None)
+
     def add_action_to_queue(
         self,
         action: Action,
         credentials: SyftVerifyKey,
         parent_job_id: UID | None = None,
         has_execute_permissions: bool = False,
         worker_pool_name: str | None = None,
@@ -1240,24 +1286,29 @@
             job_id=job_id,
             worker_settings=worker_settings,
             args=[],
             kwargs={"action": action},
             has_execute_permissions=has_execute_permissions,
             worker_pool=worker_pool_ref,  # set worker pool reference as part of queue item
         )
+        user_id = self.get_service("UserService").get_user_id_for_credentials(
+            credentials
+        )
+
         return self.add_queueitem_to_queue(
-            queue_item, credentials, action, parent_job_id
+            queue_item, credentials, action, parent_job_id, user_id
         )
 
     def add_queueitem_to_queue(
         self,
         queue_item: QueueItem,
         credentials: SyftVerifyKey,
         action: Action | None = None,
         parent_job_id: UID | None = None,
+        user_id: UID | None = None,
     ) -> Job | SyftError:
         log_id = UID()
         role = self.get_role_for_credentials(credentials=credentials)
         context = AuthedServiceContext(node=self, credentials=credentials, role=role)
 
         result_obj = ActionObject.empty()
         if action is not None:
@@ -1282,14 +1333,15 @@
             result=result_obj,
             node_uid=self.id,
             syft_client_verify_key=credentials,
             syft_node_location=self.id,
             log_id=log_id,
             parent_job_id=parent_job_id,
             action=action,
+            requested_by=user_id,
         )
 
         # 🟡 TODO 36: Needs distributed lock
         self.queue_stash.set_placeholder(credentials, queue_item)
         self.job_stash.set(credentials, job)
 
         log_service = self.get_service("logservice")
@@ -1403,15 +1455,24 @@
     @property
     def user_code_stash(self) -> UserCodeStash:
         return self.get_service(UserCodeService).stash
 
     def get_default_worker_pool(self) -> WorkerPool | None | SyftError:
         result = self.pool_stash.get_by_name(
             credentials=self.verify_key,
-            pool_name=get_default_worker_pool_name(),
+            pool_name=self.settings.default_worker_pool,
+        )
+        if result.is_err():
+            return SyftError(message=f"{result.err()}")
+        worker_pool = result.ok()
+        return worker_pool
+
+    def get_worker_pool_by_name(self, name: str) -> WorkerPool | None | SyftError:
+        result = self.pool_stash.get_by_name(
+            credentials=self.verify_key, pool_name=name
         )
         if result.is_err():
             return SyftError(message=f"{result.err()}")
         worker_pool = result.ok()
         return worker_pool
 
     def get_api(
@@ -1432,39 +1493,45 @@
         return partial(method, context=context)
 
     def get_unauthed_context(
         self, login_credentials: UserLoginCredentials
     ) -> NodeServiceContext:
         return UnauthedServiceContext(node=self, login_credentials=login_credentials)
 
-    def create_initial_settings(self, admin_email: str) -> NodeSettingsV2 | None:
+    def create_initial_settings(self, admin_email: str) -> NodeSettings | None:
         try:
             settings_stash = SettingsStash(store=self.document_store)
             if self.signing_key is None:
                 print("create_initial_settings failed as there is no signing key")
                 return None
             settings_exists = settings_stash.get_all(self.signing_key.verify_key).ok()
             if settings_exists:
-                self.name = settings_exists[0].name
+                node_settings = settings_exists[0]
+                self.name = node_settings.name
+                self.association_request_auto_approval = (
+                    node_settings.association_request_auto_approval
+                )
                 return None
             else:
                 # Currently we allow automatic user registration on enclaves,
                 # as enclaves do not have superusers
                 if self.node_type == NodeType.ENCLAVE:
                     flags.CAN_REGISTER = True
-                new_settings = NodeSettingsV2(
+                new_settings = NodeSettings(
                     id=self.id,
                     name=self.name,
                     verify_key=self.verify_key,
                     node_type=self.node_type,
                     deployed_on=datetime.now().date().strftime("%m/%d/%Y"),
                     signup_enabled=flags.CAN_REGISTER,
                     admin_email=admin_email,
                     node_side_type=self.node_side_type.value,  # type: ignore
                     show_warnings=self.enable_warnings,
+                    association_request_auto_approval=self.association_request_auto_approval,
+                    default_worker_pool=get_default_worker_pool_name(),
                 )
                 result = settings_stash.set(
                     credentials=self.signing_key.verify_key, settings=new_settings
                 )
                 if result.is_ok():
                     return result.ok()
                 return None
@@ -1551,15 +1618,15 @@
         return __version__
 
 
 def create_default_worker_pool(node: Node) -> SyftError | None:
     credentials = node.verify_key
     pull_image = not node.dev_mode
     image_stash = node.get_service(SyftWorkerImageService).stash
-    default_pool_name = get_default_worker_pool_name()
+    default_pool_name = node.settings.default_worker_pool
     default_worker_pool = node.get_default_worker_pool()
     default_worker_tag = get_default_worker_tag_by_env(node.dev_mode)
     worker_count = get_default_worker_pool_count(node)
     context = AuthedServiceContext(
         node=node,
         credentials=credentials,
         role=ServiceRole.ADMIN,
```

### Comparing `syft-0.8.7b2/src/syft/node/routes.py` & `syft-0.8.7b3/src/syft/node/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/node/run.py` & `syft-0.8.7b3/src/syft/node/run.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/node/server.py` & `syft-0.8.7b3/src/syft/node/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     reset: bool,
     dev_mode: bool,
     node_side_type: str,
     enable_warnings: bool,
     in_memory_workers: bool,
     queue_port: int | None,
     create_producer: bool,
+    association_request_auto_approval: bool,
     n_consumers: int,
 ) -> None:
     async def _run_uvicorn(
         name: str,
         node_type: NodeType,
         host: str,
         port: int,
@@ -106,28 +107,30 @@
                 node_side_type=node_side_type,
                 enable_warnings=enable_warnings,
                 migrate=True,
                 in_memory_workers=in_memory_workers,
                 queue_port=queue_port,
                 create_producer=create_producer,
                 n_consumers=n_consumers,
+                association_request_auto_approval=association_request_auto_approval,
             )
         else:
             worker = worker_class(
                 name=name,
                 processes=processes,
                 local_db=True,
                 node_type=node_type,
                 node_side_type=node_side_type,
                 enable_warnings=enable_warnings,
                 migrate=True,
                 in_memory_workers=in_memory_workers,
                 queue_port=queue_port,
                 create_producer=create_producer,
                 n_consumers=n_consumers,
+                association_request_auto_approval=association_request_auto_approval,
             )
         router = make_routes(worker=worker)
         app = make_app(worker.name, router=router)
 
         if reset:
             try:
                 python_pids = find_python_processes_on_port(port)
@@ -178,32 +181,34 @@
     dev_mode: bool = False,
     tail: bool = False,
     enable_warnings: bool = False,
     in_memory_workers: bool = True,
     queue_port: int | None = None,
     create_producer: bool = False,
     n_consumers: int = 0,
+    association_request_auto_approval: bool = False,
 ) -> tuple[Callable, Callable]:
     server_process = multiprocessing.Process(
         target=run_uvicorn,
-        args=(
-            name,
-            node_type,
-            host,
-            port,
-            processes,
-            reset,
-            dev_mode,
-            node_side_type,
-            enable_warnings,
-            in_memory_workers,
-            queue_port,
-            create_producer,
-            n_consumers,
-        ),
+        kwargs={
+            "name": name,
+            "node_type": node_type,
+            "host": host,
+            "port": port,
+            "processes": processes,
+            "reset": reset,
+            "dev_mode": dev_mode,
+            "node_side_type": node_side_type,
+            "enable_warnings": enable_warnings,
+            "in_memory_workers": in_memory_workers,
+            "queue_port": queue_port,
+            "create_producer": create_producer,
+            "n_consumers": n_consumers,
+            "association_request_auto_approval": association_request_auto_approval,
+        },
     )
 
     def stop() -> None:
         print(f"Stopping {name}")
         server_process.terminate()
         server_process.join(3)
         if server_process.is_alive():
```

### Comparing `syft-0.8.7b2/src/syft/node/worker_settings.py` & `syft-0.8.7b3/src/syft/node/worker_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/protocol/data_protocol.py` & `syft-0.8.7b3/src/syft/protocol/data_protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,26 @@
 from ..types.dicttuple import DictTuple
 from ..types.syft_object import SyftBaseObject
 from ..util.util import get_dev_mode
 
 PROTOCOL_STATE_FILENAME = "protocol_version.json"
 PROTOCOL_TYPE = str | int
 
+IGNORE_TYPES = [
+    "mock_type",
+    "MockStore",
+    "MockSyftObject",
+    "MockStoreConfig",
+    "MockWrapper",
+    "base_stash_mock_object_type",
+    "MockKeyValueBackingStore",
+    "MockObjectFromSyftBaseObj",
+    "MockObjectToSyftBaseObj",
+]
+
 
 def natural_key(key: PROTOCOL_TYPE) -> list[int | str | Any]:
     """Define key for natural ordering of strings."""
     if isinstance(key, int):
         key = str(key)
     return [int(s) if s.isdigit() else s for s in re.split(r"(\d+)", key)]
 
@@ -210,14 +222,19 @@
                 hash_exclude_attrs,
                 cls,
                 attribute_types,
                 version,
             ) = TYPE_BANK[k]
             if issubclass(cls, SyftBaseObject):
                 canonical_name = cls.__canonical_name__
+                if canonical_name in IGNORE_TYPES or canonical_name.startswith(
+                    "MockSyftObject_"
+                ):
+                    continue
+
                 hash_str = DataProtocol._calculate_object_hash(cls)
 
                 # build this up for later
                 compare_dict[canonical_name][str(version)] = hash_str
 
                 if canonical_name not in state:
                     # new object so its an add
```

### Comparing `syft-0.8.7b2/src/syft/protocol/protocol_version.json` & `syft-0.8.7b3/src/syft/protocol/protocol_version.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9829365079365079%*

 * *Differences: {"'dev'": "{'object_versions': {'CustomAPIView': {'1': {'hash': "*

 * *          "'8fe9f0fded4dbce033e2b14798a59d8635c3b73b0562f9ea686b1162ed155e91'}}, "*

 * *          "'UpdateTwinAPIEndpoint': {'1': {'hash': "*

 * *          "'cd0d4d67dc03cf6b78832f33ef584ec0ff8fa0b851629396ba27d7db63130342'}}, "*

 * *          "'CreateTwinAPIEndpoint': {'1': {'hash': "*

 * *          "'e735dc30cba1789c3fb109e35aa40ffa873951f8e00b0b971950b1735c27d1ca'}}, "*

 * *          "'TwinAPIEndpoint': {'1': {'hash': "*

 * *          "'540468be5db20efe555d2288c9aed608 […]*

```diff
@@ -9,25 +9,46 @@
         "release_name": "0.8.4.json"
     },
     "4": {
         "release_name": "0.8.6.json"
     },
     "dev": {
         "object_versions": {
+            "APIEndpointQueueItem": {
+                "1": {
+                    "action": "add",
+                    "hash": "d31b2edfb767401c810584baccd27e4f566181c3ef7706618a82eb25ae20ff6d",
+                    "version": 1
+                }
+            },
+            "AssociationRequestChange": {
+                "1": {
+                    "action": "add",
+                    "hash": "508550c43e9e3f30243813c23eb6eec20918923d7ba09498cddbcd7e8bfa4539",
+                    "version": 1
+                }
+            },
             "CreateTwinAPIEndpoint": {
                 "1": {
                     "action": "add",
-                    "hash": "98021128a9be0a9a135b43b50cb08f141faed72bc39999a9cedd162bc8814f62",
+                    "hash": "e735dc30cba1789c3fb109e35aa40ffa873951f8e00b0b971950b1735c27d1ca",
                     "version": 1
                 }
             },
             "CustomAPIView": {
                 "1": {
                     "action": "add",
-                    "hash": "5cdfaea6b5af235d0f9ab8e6f01d6cebcde7c8bf4efd00aec26c343965ef865e",
+                    "hash": "8fe9f0fded4dbce033e2b14798a59d8635c3b73b0562f9ea686b1162ed155e91",
+                    "version": 1
+                }
+            },
+            "CustomApiEndpoint": {
+                "1": {
+                    "action": "add",
+                    "hash": "13617f3dce60fa692421e0d9deda7ffd365ec02d4a062c18510b48457b6eba02",
                     "version": 1
                 }
             },
             "CustomEndpointActionObject": {
                 "1": {
                     "action": "add",
                     "hash": "642facc6cafbaad4de030a33cd619bd68ac31a32b0db07ddc1c1d5d7f914503e",
@@ -54,21 +75,47 @@
                 },
                 "2": {
                     "action": "add",
                     "hash": "854fe9df5bcbb5c7e5b7c467bac423cd98c32f93d6876fea7b8eb6c08f6596da",
                     "version": 2
                 }
             },
+            "JobItem": {
+                "4": {
+                    "action": "remove",
+                    "hash": "6a7cc7c2bb4dd234c1508b0af4d3b403cd3b7b427578a775bf80dc36891923ed",
+                    "version": 4
+                },
+                "5": {
+                    "action": "add",
+                    "hash": "82ee08442b09797ed7a3710c31de633bb308b1d2215f51b58a3e01a4c201055d",
+                    "version": 5
+                }
+            },
             "NodePeer": {
                 "3": {
                     "action": "add",
                     "hash": "dababb03d2463b6218ae22d55293a60580f5a14bebd0c664d71da104e2f0b835",
                     "version": 3
                 }
             },
+            "NodeSettings": {
+                "4": {
+                    "action": "add",
+                    "hash": "318e578f8a9af213a6af0cc2c567b62196b0ff81769d808afff4dd1eb7c372b8",
+                    "version": 4
+                }
+            },
+            "NodeSettingsUpdate": {
+                "3": {
+                    "action": "add",
+                    "hash": "0f812fdd5aecc3e3aa1a7c953bbf7f8d8b03a77c5cdbb37e981fa91c8134c9f4",
+                    "version": 3
+                }
+            },
             "PrivateAPIEndpoint": {
                 "1": {
                     "action": "add",
                     "hash": "004ec19753263440e2896b4e35d7a6305322934512f473f37d54043af5726fe6",
                     "version": 1
                 }
             },
@@ -106,25 +153,32 @@
             "SyncStateItem": {
                 "1": {
                     "action": "remove",
                     "hash": "4dbfa0813f5a3f7be0b36249ff2d67e395ad7c9e138c5a122fc7342b8dcc4b92",
                     "version": 1
                 }
             },
+            "TwinAPIContextView": {
+                "1": {
+                    "action": "add",
+                    "hash": "7d368102d0b473009af3b8c46e0ea6d35893c5ebb172b373ad7d52553c12c9fa",
+                    "version": 1
+                }
+            },
             "TwinAPIEndpoint": {
                 "1": {
                     "action": "add",
-                    "hash": "03a0244c6b322e72032c5c33c1db09b913f83d72cfad1cc51ac4ec90506afcf5",
+                    "hash": "540468be5db20efe555d2288c9aed60887306ac9b56d6a63c066246bc0010e9c",
                     "version": 1
                 }
             },
             "UpdateTwinAPIEndpoint": {
                 "1": {
                     "action": "add",
-                    "hash": "6c0c6bc042391e60d5c78893f859c8bdec4b45f0bdc7749957a425e041a4096c",
+                    "hash": "cd0d4d67dc03cf6b78832f33ef584ec0ff8fa0b851629396ba27d7db63130342",
                     "version": 1
                 }
             },
             "VeilidConnection": {
                 "1": {
                     "action": "remove",
                     "hash": "c1796e7b01c9eae0dbf59cfd5c2c2f0e7eba593e0cea615717246572b27aae4b",
```

### Comparing `syft-0.8.7b2/src/syft/protocol/releases/0.8.2.json` & `syft-0.8.7b3/src/syft/protocol/releases/0.8.2.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/protocol/releases/0.8.3.json` & `syft-0.8.7b3/src/syft/protocol/releases/0.8.3.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/protocol/releases/0.8.4.json` & `syft-0.8.7b3/src/syft/protocol/releases/0.8.4.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/protocol/releases/0.8.6.json` & `syft-0.8.7b3/src/syft/protocol/releases/0.8.6.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/serde/array.py` & `syft-0.8.7b3/src/syft/serde/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/serde/arrow.py` & `syft-0.8.7b3/src/syft/serde/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/serde/deserialize.py` & `syft-0.8.7b3/src/syft/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/serde/lib_permissions.py` & `syft-0.8.7b3/src/syft/serde/lib_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/serde/lib_service_registry.py` & `syft-0.8.7b3/src/syft/serde/lib_service_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/serde/mock.py` & `syft-0.8.7b3/src/syft/serde/mock.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/serde/recursive.py` & `syft-0.8.7b3/src/syft/serde/recursive.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # syft absolute
 import syft as sy
 
 # relative
 from ..util.util import get_fully_qualified_name
 from ..util.util import index_syft_by_module_name
 from .capnp import get_capnp_schema
+from .util import compatible_with_large_file_writes_capnp
 
 TYPE_BANK = {}
 
 recursive_scheme = get_capnp_schema("recursive_serde.capnp").RecursiveSerde
 
 SPOOLED_FILE_MAX_SIZE_SERDE = 50 * (1024**2)  # 50MB
 
@@ -167,29 +168,37 @@
     field_obj: Any,
     ser_func: Callable,
     field_name: str | int,
     builder: _DynamicStructBuilder,
 ) -> None:
     data = ser_func(field_obj)
     size_of_data = len(data)
-    with tempfile.SpooledTemporaryFile(
-        max_size=SPOOLED_FILE_MAX_SIZE_SERDE
-    ) as tmp_file:
-        # Write data to a file to save RAM
-        tmp_file.write(data)
-        tmp_file.seek(0)
-        del data
-
+    if compatible_with_large_file_writes_capnp(size_of_data):
+        with tempfile.TemporaryFile() as tmp_file:
+            # Write data to a file to save RAM
+            tmp_file.write(data)
+            tmp_file.seek(0)
+            del data
+
+            CHUNK_SIZE = int(5.12e8)  # capnp max for a List(Data) field
+            list_size = size_of_data // CHUNK_SIZE + 1
+            data_lst = builder.init(field_name, list_size)
+            for idx in range(list_size):
+                bytes_to_read = min(CHUNK_SIZE, size_of_data)
+                data_lst[idx] = tmp_file.read(bytes_to_read)
+                size_of_data -= CHUNK_SIZE
+    else:
         CHUNK_SIZE = int(5.12e8)  # capnp max for a List(Data) field
-        list_size = size_of_data // CHUNK_SIZE + 1
+        list_size = len(data) // CHUNK_SIZE + 1
         data_lst = builder.init(field_name, list_size)
+        END_INDEX = CHUNK_SIZE
         for idx in range(list_size):
-            bytes_to_read = min(CHUNK_SIZE, size_of_data)
-            data_lst[idx] = tmp_file.read(bytes_to_read)
-            size_of_data -= CHUNK_SIZE
+            START_INDEX = idx * CHUNK_SIZE
+            END_INDEX = min(START_INDEX + CHUNK_SIZE, len(data))
+            data_lst[idx] = data[START_INDEX:END_INDEX]
 
 
 def combine_bytes(capnp_list: list[bytes]) -> bytes:
     # TODO: make sure this doesn't copy, perhaps allocate a fixed size buffer
     # and move the bytes into it as we go
     bytes_value = b""
     for value in capnp_list:
```

### Comparing `syft-0.8.7b2/src/syft/serde/recursive_primitives.py` & `syft-0.8.7b3/src/syft/serde/recursive_primitives.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # stdlib
+from abc import ABCMeta
 from collections import OrderedDict
 from collections import defaultdict
 from collections.abc import Collection
 from collections.abc import Iterable
 from collections.abc import Mapping
 from enum import Enum
 from enum import EnumMeta
@@ -45,18 +46,16 @@
 
     message.init("values", len(iterable))
 
     for idx, it in enumerate(iterable):
         # serialized = _serialize(it, to_bytes=True)
         chunk_bytes(it, lambda x: _serialize(x, to_bytes=True), idx, message.values)
 
-    if compatible_with_large_file_writes_capnp():
-        with tempfile.SpooledTemporaryFile(
-            max_size=SPOOLED_FILE_MAX_SIZE_SERDE
-        ) as tmp_file:
+    if compatible_with_large_file_writes_capnp(message):
+        with tempfile.TemporaryFile() as tmp_file:
             # Write data to a file to save RAM
             message.write(tmp_file)
             del message
             tmp_file.seek(0)
             res = tmp_file.read()
             return res
     else:
@@ -433,7 +432,9 @@
     ],
 )
 recursive_serde_register_type(_SpecialGenericAlias)
 recursive_serde_register_type(GenericAlias)
 
 recursive_serde_register_type(Any)
 recursive_serde_register_type(EnumMeta)
+
+recursive_serde_register_type(ABCMeta)
```

### Comparing `syft-0.8.7b2/src/syft/serde/serializable.py` & `syft-0.8.7b3/src/syft/serde/serializable.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/serde/serialize.py` & `syft-0.8.7b3/src/syft/serde/serialize.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,20 +14,17 @@
     for_hashing: bool = False,
 ) -> Any:
     # relative
     from .recursive import rs_object2proto
 
     proto = rs_object2proto(obj, for_hashing=for_hashing)
     if to_bytes:
-        if compatible_with_large_file_writes_capnp():
-            with tempfile.SpooledTemporaryFile(
-                max_size=SPOOLED_FILE_MAX_SIZE_SERDE
-            ) as tmp_file:
+        if compatible_with_large_file_writes_capnp(proto):
+            with tempfile.TemporaryFile() as tmp_file:
                 # Write data to a file to save RAM
-
                 proto.write(tmp_file)
                 # proto in memory, and bytes in file
                 del proto
                 # bytes in file
                 tmp_file.seek(0)
                 return tmp_file.read()
         else:
```

### Comparing `syft-0.8.7b2/src/syft/serde/signature.py` & `syft-0.8.7b3/src/syft/serde/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/serde/third_party.py` & `syft-0.8.7b3/src/syft/serde/third_party.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/action/action_data_empty.py` & `syft-0.8.7b3/src/syft/service/action/action_data_empty.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/action/action_endpoint.py` & `syft-0.8.7b3/src/syft/service/action/action_endpoint.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/action/action_graph.py` & `syft-0.8.7b3/src/syft/service/action/action_graph.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/action/action_graph_service.py` & `syft-0.8.7b3/src/syft/service/action/action_graph_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/action/action_object.py` & `syft-0.8.7b3/src/syft/service/action/action_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,14 +302,15 @@
     "__hash_exclude_attrs__",  # syft
     "__private_sync_attr_mocks__",  # syft
     "__exclude_sync_diff_attrs__",  # syft
     "__repr_attrs__",  # syft
     "get_sync_dependencies",
     "_data_repr",
     "syft_eq",  # syft
+    "__table_coll_widths__",
 ]
 dont_wrap_output_attrs = [
     "__repr__",
     "__str__",
     "__repr_attrs__",
     "_repr_html_",
     "_repr_markdown_",
@@ -324,14 +325,15 @@
     "syft_action_data_node_id",
     "__sha256__",
     "__hash_exclude_attrs__",
     "__exclude_sync_diff_attrs__",  # syft
     "__repr_attrs__",  # syft
     "get_sync_dependencies",  # syft
     "syft_eq",  # syft
+    "__table_coll_widths__",
 ]
 dont_make_side_effects = [
     "__repr_attrs__",
     "_repr_html_",
     "_repr_markdown_",
     "_repr_latex_",
     "__repr__",
@@ -344,14 +346,15 @@
     "syft_action_data_node_id",
     "__sha256__",
     "__hash_exclude_attrs__",
     "__exclude_sync_diff_attrs__",  # syft
     "__repr_attrs__",
     "get_sync_dependencies",
     "syft_eq",  # syft
+    "__table_coll_widths__",
 ]
 action_data_empty_must_run = [
     "__repr__",
     "__str__",
 ]
 
 methods_to_check_in_cache = [
@@ -642,14 +645,15 @@
     "create_shareable_sync_copy",
     "_has_private_sync_attrs",
     "__exclude_sync_diff_attrs__",
     "__repr_attrs__",
     "get_sync_dependencies",
     "_data_repr",
     "syft_eq",
+    "__table_coll_widths__",
 ]
 
 
 @serializable(without=["syft_pre_hooks__", "syft_post_hooks__"])
 class ActionObject(SyncableSyftObject):
     """Action object for remote execution."""
```

### Comparing `syft-0.8.7b2/src/syft/service/action/action_permissions.py` & `syft-0.8.7b3/src/syft/service/action/action_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/action/action_service.py` & `syft-0.8.7b3/src/syft/service/action/action_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,27 +420,32 @@
         return Ok(result_action_object)
 
     def set_result_to_store(
         self,
         result_action_object: ActionObject | TwinObject,
         context: AuthedServiceContext,
         output_policy: OutputPolicy | None = None,
+        has_result_read_permission: bool = False,
     ) -> Result[ActionObject, str]:
         result_id = result_action_object.id
         # result_blob_id = result_action_object.syft_blob_storage_entry_id
 
         if output_policy is not None:
             output_readers = (
                 output_policy.output_readers
                 if not context.has_execute_permissions
                 else []
             )
         else:
             output_readers = []
 
+        # If flag is True, user has read permissions to the results in BlobStore
+        if has_result_read_permission:
+            output_readers.append(context.credentials)
+
         read_permission = ActionPermission.READ
 
         result_action_object._set_obj_location_(
             context.node.id,
             context.credentials,
         )
         blob_store_result = result_action_object._save_to_blob_storage()
@@ -450,17 +455,20 @@
         # IMPORTANT: DO THIS ONLY AFTER ._save_to_blob_storage
         if isinstance(result_action_object, TwinObject):
             result_blob_id = result_action_object.private.syft_blob_storage_entry_id
         else:
             result_blob_id = result_action_object.syft_blob_storage_entry_id  # type: ignore[unreachable]
 
         # pass permission information to the action store as extra kwargs
-        context.extra_kwargs = {"has_result_read_permission": True}
+        # context.extra_kwargs = {"has_result_read_permission": True}
 
-        set_result = self._set(context, result_action_object)
+        # Since this just meta data about the result, they always have access to it.
+        set_result = self._set(
+            context, result_action_object, has_result_read_permission=True
+        )
 
         if set_result.is_err():
             return set_result
 
         blob_storage_service: AbstractService = context.node.get_service(
             BlobStorageService
         )
```

### Comparing `syft-0.8.7b2/src/syft/service/action/action_store.py` & `syft-0.8.7b3/src/syft/service/action/action_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/action/action_types.py` & `syft-0.8.7b3/src/syft/service/action/action_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/action/numpy.py` & `syft-0.8.7b3/src/syft/service/action/numpy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/action/pandas.py` & `syft-0.8.7b3/src/syft/service/action/pandas.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/action/plan.py` & `syft-0.8.7b3/src/syft/service/action/plan.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/action/verification.py` & `syft-0.8.7b3/src/syft/service/action/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/api/api.py` & `syft-0.8.7b3/src/syft/service/api/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 from ...types.syft_object import PartialSyftObject
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
 from ...types.syncable_object import SyncableSyftObject
 from ...types.transforms import TransformContext
 from ...types.transforms import generate_action_object_id
 from ...types.transforms import generate_id
+from ...types.transforms import keep
 from ...types.transforms import transform
 from ...types.uid import UID
 from ..context import AuthedServiceContext
 from ..response import SyftError
+from ..user.user import UserView
 
 NOT_ACCESSIBLE_STRING = "N / A"
 
 
 class HelperFunctionSet:
     def __init__(self, helper_functions: dict[str, Callable]) -> None:
         self.helper_functions = helper_functions
@@ -43,19 +45,31 @@
             setattr(self, name, func)
 
 
 class TwinAPIAuthedContext(AuthedServiceContext):
     __canonical_name__ = "AuthedServiceContext"
     __version__ = SYFT_OBJECT_VERSION_1
 
+    user: UserView | None = None
     settings: dict[str, Any] | None = None
     code: HelperFunctionSet | None = None
     state: dict[Any, Any] | None = None
 
 
+@serializable()
+class TwinAPIContextView(SyftObject):
+    __canonical_name__ = "TwinAPIContextView"
+    __version__ = SYFT_OBJECT_VERSION_1
+
+    __repr_attrs__ = ["settings", "state", "user"]
+    user: UserView
+    settings: dict[str, Any]
+    state: dict[Any, Any]
+
+
 def get_signature(func: Callable) -> Signature:
     sig = inspect.signature(func)
     sig = signature_remove_context(sig)
     return sig
 
 
 @serializable()
@@ -69,18 +83,22 @@
     signature: Signature
     access: str = "Public"
     mock_function: str | None = None
     private_function: str | None = None
     description: str | None = None
     mock_helper_functions: list[str] | None = None
     private_helper_functions: list[str] | None = None
+    worker_pool: str | None = None
+    endpoint_timeout: int = 60
 
     __repr_attrs__ = [
         "path",
         "signature",
+        "worker_pool",
+        "endpoint_timeout",
     ]
 
     def _coll_repr_(self) -> dict[str, Any]:
         mock_parsed_code = ast.parse(self.mock_function)
         mock_function_name = [
             node.name
             for node in ast.walk(mock_parsed_code)
@@ -90,23 +108,28 @@
         if self.private_function != NOT_ACCESSIBLE_STRING:
             private_parsed_code = ast.parse(self.private_function)
             private_function_name = [
                 node.name
                 for node in ast.walk(private_parsed_code)
                 if isinstance(node, ast.FunctionDef)
             ][0]
+        worker_pool = "UNSET (DEFAULT)"
+        if self.worker_pool is not None:
+            worker_pool = self.worker_pool
         return {
             "API path": self.path,
             "Signature": self.path + str(self.signature),
             "Access": self.access,
             "Mock Function": mock_function_name,
             "Private Function": private_function_name,
+            "Worker Pool": worker_pool,
         }
 
 
+@serializable()
 class Endpoint(SyftObject):
     """Base class to perform basic Endpoint validation for both public/private endpoints."""
 
     # version
     __canonical_name__ = "CustomApiEndpoint"
     __version__ = SYFT_OBJECT_VERSION_1
 
@@ -158,21 +181,88 @@
         cls, settings: dict[str, Any] | None
     ) -> dict[str, Any] | None:
         return settings
 
     def update_state(self, state: dict[Any, Any]) -> None:
         self.state = state
 
+    def build_internal_context(
+        self, context: AuthedServiceContext
+    ) -> TwinAPIAuthedContext:
+        helper_function_dict: dict[str, Callable] = {}
+        self.helper_functions = self.helper_functions or {}
+        for helper_name, helper_code in self.helper_functions.items():
+            # Create a dictionary to serve as local scope
+            local_scope: dict[str, Callable] = {}
+
+            # Execute the function string within the local scope
+            exec(helper_code, local_scope)  # nosec
+            helper_function_dict[helper_name] = local_scope[helper_name]
+
+        helper_function_set = HelperFunctionSet(helper_function_dict)
+
+        user_service = context.node.get_service("userservice")
+        user = user_service.get_current_user(context)
+
+        return TwinAPIAuthedContext(
+            credentials=context.credentials,
+            role=context.role,
+            job_id=context.job_id,
+            extra_kwargs=context.extra_kwargs,
+            has_execute_permissions=context.has_execute_permissions,
+            node=context.node,
+            id=context.id,
+            settings=self.settings or {},
+            code=helper_function_set,
+            state=self.state or {},
+            user=user,
+        )
+
+    def __call__(self, *args: Any, **kwargs: Any) -> Any:
+        # relative
+        from ... import SyftSigningKey
+        from ..context import AuthedServiceContext
+
+        mock_context = AuthedServiceContext(
+            node=AbstractNode(), credentials=SyftSigningKey.generate().verify_key
+        )
+        return self.call_locally(mock_context, *args, **kwargs)
+
+    def call_locally(
+        self, context: AuthedServiceContext, *args: Any, **kwargs: Any
+    ) -> Any:
+        inner_function = ast.parse(self.api_code).body[0]
+        inner_function.decorator_list = []
+        # compile the function
+        raw_byte_code = compile(ast.unparse(inner_function), "<string>", "exec")
+
+        # load it
+        exec(raw_byte_code)  # nosec
+
+        internal_context = self.build_internal_context(context)
+
+        # execute it
+        evil_string = f"{self.func_name}(*args, **kwargs,context=internal_context)"
+        result = eval(evil_string, None, locals())  # nosec
+
+        # Update code context state
+        self.update_state(internal_context.state)
+
+        # return the results
+        return result
+
 
 @serializable()
 class PrivateAPIEndpoint(Endpoint):
     # version
     __canonical_name__ = "PrivateAPIEndpoint"
     __version__ = SYFT_OBJECT_VERSION_1
 
+    view_access: bool = False
+
 
 @serializable()
 class PublicAPIEndpoint(Endpoint):
     # version
     __canonical_name__ = "PublicAPIEndpoint"
     __version__ = SYFT_OBJECT_VERSION_1
 
@@ -229,55 +319,62 @@
     __canonical_name__ = "UpdateTwinAPIEndpoint"
     __version__ = SYFT_OBJECT_VERSION_1
 
     path: str
     private_function: PrivateAPIEndpoint | None = None
     mock_function: PublicAPIEndpoint
     description: str | None = None
+    endpoint_timeout: int = 60
 
 
 @serializable()
 class CreateTwinAPIEndpoint(BaseTwinAPIEndpoint):
     # version
     __canonical_name__ = "CreateTwinAPIEndpoint"
     __version__ = SYFT_OBJECT_VERSION_1
 
     path: str
     private_function: PrivateAPIEndpoint | None = None
     mock_function: PublicAPIEndpoint
     signature: Signature
     description: str | None = None
+    worker_pool: str | None = None
+    endpoint_timeout: int = 60
 
 
 @serializable()
 class TwinAPIEndpoint(SyncableSyftObject):
     # version
-    __canonical_name__ = "TwinAPIEndpoint"
+    __canonical_name__: str = "TwinAPIEndpoint"
     __version__ = SYFT_OBJECT_VERSION_1
 
     def __init__(self, **kwargs: Any) -> None:
         super().__init__(**kwargs)
 
     path: str
     private_function: PrivateAPIEndpoint | None = None
     mock_function: PublicAPIEndpoint
     signature: Signature
     description: str | None = None
     action_object_id: UID
+    worker_pool: str | None = None
+    endpoint_timeout: int = 60
+
     __private_sync_attr_mocks__ = {
         "private_function": None,
     }
 
     __attr_searchable__ = ["path"]
     __attr_unique__ = ["path"]
     __repr_attrs__ = [
         "path",
         "description",
         "private_function",
         "mock_function",
+        "endpoint_timeout",
     ]
 
     def has_mock(self) -> bool:
         return self.api_mock_code is not None
 
     def has_permission(self, context: AuthedServiceContext) -> bool:
         """Check if the user has permission to access the endpoint.
@@ -337,14 +434,17 @@
         Args:
             context: The context of the user requesting the code.
             *args: Any
             **kwargs: Any
         Returns:
             Any: The result of the executed code.
         """
+        if self.private_function is None:
+            return SyftError(message="No private code available")
+
         if self.has_permission(context):
             return self.exec_code(self.private_function, context, *args, **kwargs)
 
         return SyftError(message="You're not allowed to run this code.")
 
     def exec_code(
         self,
@@ -355,41 +455,19 @@
     ) -> Any:
         try:
             inner_function = ast.parse(code.api_code).body[0]
             inner_function.decorator_list = []
             # compile the function
             raw_byte_code = compile(ast.unparse(inner_function), "<string>", "exec")
 
-            helper_function_dict: dict[str, Callable] = {}
-            code.helper_functions = code.helper_functions or {}
-            for helper_name, helper_code in code.helper_functions.items():
-                # Create a dictionary to serve as local scope
-                local_scope: dict[str, Callable] = {}
-
-                # Execute the function string within the local scope
-                exec(helper_code, local_scope)  # nosec
-                helper_function_dict[helper_name] = local_scope[helper_name]
-
-            helper_function_set = HelperFunctionSet(helper_function_dict)
-
             # load it
             exec(raw_byte_code)  # nosec
 
-            internal_context = TwinAPIAuthedContext(
-                credentials=context.credentials,
-                role=context.role,
-                job_id=context.job_id,
-                extra_kwargs=context.extra_kwargs,
-                has_execute_permissions=context.has_execute_permissions,
-                node=context.node,
-                id=context.id,
-                settings=code.settings or {},
-                code=helper_function_set,
-                state=code.state or {},
-            )
+            internal_context = code.build_internal_context(context)
+
             # execute it
             evil_string = f"{code.func_name}(*args, **kwargs,context=internal_context)"
             result = eval(evil_string, None, locals())  # nosec
 
             # Update code context state
             code.update_state(internal_context.state)
 
@@ -407,15 +485,17 @@
                 raise Exception(upsert_result.err())
 
             # return the results
             return result
         except Exception as e:
             # If it's admin, return the error message.
             if context.role.value == 128:
-                return SyftError(message=f"{str(e)}")
+                return SyftError(
+                    message=f"An error was raised during the execution of the API endpoint call: \n {str(e)}"
+                )
             else:
                 return SyftError(
                     message="Ops something went wrong during this endpoint execution, please contact your admin."
                 )
 
 
 def set_access_type(context: TransformContext) -> TransformContext:
@@ -441,18 +521,18 @@
         )
     return context
 
 
 def decorator_cleanup(code: str) -> str:
     # Regular expression to remove decorator
     # It matches from "@" to "def" (non-greedy) across multiple lines
-    decorator_regex = r"@.*?def"
+    decorator_regex = r"@.*?def "
 
     # Substituting the matched pattern with "def"
-    return re.sub(decorator_regex, "def", code, count=1, flags=re.DOTALL)
+    return re.sub(decorator_regex, "def ", code, count=1, flags=re.DOTALL)
 
 
 def extract_code_string(code_field: str) -> Callable:
     def code_string(context: TransformContext) -> TransformContext:
         if context.obj is not None and context.output is not None:
             endpoint_type = (
                 context.obj.private_function
@@ -480,33 +560,73 @@
                 context.output[code_field] = NOT_ACCESSIBLE_STRING
                 context.output[helper_function_field] = []
         return context
 
     return code_string
 
 
+@transform(TwinAPIAuthedContext, TwinAPIContextView)
+def twin_api_context_to_twin_api_context_view() -> list[Callable]:
+    return [keep(["state", "settings", "user"])]
+
+
 @transform(CreateTwinAPIEndpoint, TwinAPIEndpoint)
 def endpoint_create_to_twin_endpoint() -> list[Callable]:
     return [generate_id, generate_action_object_id, check_and_cleanup_signature]
 
 
 @transform(TwinAPIEndpoint, TwinAPIEndpointView)
 def twin_endpoint_to_view() -> list[Callable]:
     return [
         set_access_type,
         extract_code_string("private_function"),
         extract_code_string("mock_function"),
     ]
 
 
+@transform(Endpoint, PrivateAPIEndpoint)
+def endpoint_to_private_endpoint() -> list[Callable]:
+    return [
+        keep(
+            [
+                "api_code",
+                "func_name",
+                "settings",
+                "helper_functions",
+                "state",
+                "signature",
+            ]
+        )
+    ]
+
+
+@transform(Endpoint, PublicAPIEndpoint)
+def endpoint_to_public_endpoint() -> list[Callable]:
+    return [
+        keep(
+            [
+                "api_code",
+                "func_name",
+                "settings",
+                "view_access",
+                "helper_functions",
+                "state",
+                "signature",
+            ]
+        )
+    ]
+
+
 def api_endpoint(
     path: str,
     settings: dict[str, str] | None = None,
     helper_functions: list[Callable] | None = None,
     description: str | None = None,
+    worker_pool: str | None = None,
+    endpoint_timeout: int = 60,
 ) -> Callable[..., TwinAPIEndpoint | SyftError]:
     def decorator(f: Callable) -> TwinAPIEndpoint | SyftError:
         try:
             helper_functions_dict = {
                 f.__name__: inspect.getsource(f) for f in (helper_functions or [])
             }
             res = CreateTwinAPIEndpoint(
@@ -516,59 +636,36 @@
                     func_name=f.__name__,
                     settings=settings,
                     signature=inspect.signature(f),
                     helper_functions=helper_functions_dict,
                 ),
                 signature=inspect.signature(f),
                 description=description,
+                worker_pool=worker_pool,
+                endpoint_timeout=endpoint_timeout,
             )
         except ValidationError as e:
             for error in e.errors():
                 error_msg = error["msg"]
             res = SyftError(message=error_msg)
         return res
 
     return decorator
 
 
-def private_api_endpoint(
-    settings: dict[str, str] | None = None,
-    helper_functions: list[Callable] | None = None,
-) -> Callable[..., PrivateAPIEndpoint | SyftError]:
-    def decorator(f: Callable) -> PrivateAPIEndpoint | SyftError:
-        try:
-            helper_functions_dict = {
-                f.__name__: inspect.getsource(f) for f in (helper_functions or [])
-            }
-            return PrivateAPIEndpoint(
-                api_code=inspect.getsource(f),
-                func_name=f.__name__,
-                settings=settings,
-                signature=inspect.signature(f),
-                helper_functions=helper_functions_dict,
-            )
-        except ValidationError as e:
-            for error in e.errors():
-                error_msg = error["msg"]
-            res = SyftError(message=error_msg)
-        return res
-
-    return decorator
-
-
-def mock_api_endpoint(
+def api_endpoint_method(
     settings: dict[str, str] | None = None,
     helper_functions: list[Callable] | None = None,
-) -> Callable[..., PublicAPIEndpoint | SyftError]:
-    def decorator(f: Callable) -> PublicAPIEndpoint | SyftError:
+) -> Callable[..., Endpoint | SyftError]:
+    def decorator(f: Callable) -> Endpoint | SyftError:
         try:
             helper_functions_dict = {
                 f.__name__: inspect.getsource(f) for f in (helper_functions or [])
             }
-            return PublicAPIEndpoint(
+            return Endpoint(
                 api_code=inspect.getsource(f),
                 func_name=f.__name__,
                 settings=settings,
                 signature=inspect.signature(f),
                 helper_functions=helper_functions_dict,
             )
         except ValidationError as e:
@@ -578,38 +675,45 @@
         return res
 
     return decorator
 
 
 def create_new_api_endpoint(
     path: str,
-    mock_function: PublicAPIEndpoint,
-    private_function: PrivateAPIEndpoint | None = None,
+    mock_function: Endpoint,
+    private_function: Endpoint | None = None,
     description: str | None = None,
+    worker_pool: str | None = None,
+    endpoint_timeout: int = 60,
 ) -> CreateTwinAPIEndpoint | SyftError:
     try:
         # Parse the string to extract the function name
 
         endpoint_signature = mock_function.signature
         if private_function is not None:
             if private_function.signature != mock_function.signature:
                 return SyftError(message="Signatures don't match")
             endpoint_signature = mock_function.signature
+            private_function.view_access = False
 
             return CreateTwinAPIEndpoint(
                 path=path,
-                private_function=private_function,
-                mock_function=mock_function,
+                private_function=private_function.to(PrivateAPIEndpoint),
+                mock_function=mock_function.to(PublicAPIEndpoint),
                 signature=endpoint_signature,
                 description=description,
+                worker_pool=worker_pool,
+                endpoint_timeout=endpoint_timeout,
             )
 
         return CreateTwinAPIEndpoint(
             path=path,
-            prublic_code=mock_function,
+            prublic_code=mock_function.to(PublicAPIEndpoint),
             signature=endpoint_signature,
+            worker_pool=worker_pool,
+            endpoint_timeout=endpoint_timeout,
         )
     except ValidationError as e:
         for error in e.errors():
             error_msg = error["msg"]
 
     return SyftError(message=error_msg)
```

### Comparing `syft-0.8.7b2/src/syft/service/api/api_service.py` & `syft-0.8.7b3/src/syft/service/api/api_service.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 # stdlib
+import time
 from typing import Any
+from typing import cast
 
 # third party
 from pydantic import ValidationError
+from result import Ok
 
 # relative
 from ...serde.serializable import serializable
 from ...service.action.action_endpoint import CustomEndpointActionObject
 from ...service.action.action_object import ActionObject
 from ...store.document_store import DocumentStore
 from ...types.uid import UID
 from ...util.telemetry import instrument
+from ..action.action_service import ActionService
 from ..context import AuthedServiceContext
 from ..response import SyftError
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import TYPE_TO_SERVICE
 from ..service import service_method
 from ..user.user_roles import ADMIN_ROLE_LEVEL
 from ..user.user_roles import DATA_SCIENTIST_ROLE_LEVEL
 from ..user.user_roles import GUEST_ROLE_LEVEL
 from .api import CreateTwinAPIEndpoint
+from .api import Endpoint
 from .api import PrivateAPIEndpoint
 from .api import PublicAPIEndpoint
+from .api import TwinAPIContextView
 from .api import TwinAPIEndpoint
 from .api import TwinAPIEndpointView
 from .api import UpdateTwinAPIEndpoint
 from .api_stash import TwinAPIEndpointStash
 
 
 @instrument
@@ -47,19 +53,21 @@
     def set(
         self,
         context: AuthedServiceContext,
         endpoint: CreateTwinAPIEndpoint | TwinAPIEndpoint,
     ) -> SyftSuccess | SyftError:
         """Register an CustomAPIEndpoint."""
         try:
+            new_endpoint = None
             if isinstance(endpoint, CreateTwinAPIEndpoint):  # type: ignore
                 new_endpoint = endpoint.to(TwinAPIEndpoint)
             elif isinstance(endpoint, TwinAPIEndpoint):  # type: ignore
                 new_endpoint = endpoint
-            else:
+
+            if new_endpoint is None:
                 return SyftError(message="Invalid endpoint type.")
         except ValueError as e:
             return SyftError(message=str(e))
 
         endpoint_exists = self.stash.path_exists(context.credentials, new_endpoint.path)
 
         if endpoint_exists.is_err():
@@ -93,66 +101,82 @@
         name="update",
         roles=ADMIN_ROLE_LEVEL,
     )
     def update(
         self,
         context: AuthedServiceContext,
         endpoint_path: str,
-        mock_function: PublicAPIEndpoint | None = None,
-        private_function: PrivateAPIEndpoint | None = None,
-        hide_definition: bool | None = None,
+        mock_function: Endpoint | None = None,
+        private_function: Endpoint | None = None,
+        hide_mock_definition: bool | None = None,
+        endpoint_timeout: int | None = None,
     ) -> SyftSuccess | SyftError:
         """Updates an specific API endpoint."""
 
+        # if any of these are supplied e.g. truthy then keep going otherwise return
+        # an error
+        # TODO: change to an Update object with autosplat
+        if not (
+            mock_function
+            or private_function
+            or (hide_mock_definition is not None)
+            or endpoint_timeout
+        ):
+            return SyftError(
+                message='At least one of "mock_function", "private_function", '
+                '"hide_mock_definition" or "endpoint_timeout" is required.'
+            )
+
         endpoint_result = self.stash.get_by_path(context.credentials, endpoint_path)
 
         if endpoint_result.is_err():
             return SyftError(message=endpoint_result.err())
 
         if not endpoint_result.ok():
             return SyftError(message=f"Enpoint at path {endpoint_path} doesn't exist")
 
         endpoint: TwinAPIEndpoint = endpoint_result.ok()
 
-        if not (mock_function or private_function or (hide_definition is not None)):
-            return SyftError(
-                message='Either "mock_function","private_function" or "hide_definition" are required.'
-            )
+        endpoint_timeout = (
+            endpoint_timeout
+            if endpoint_timeout is not None
+            else endpoint.endpoint_timeout
+        )
 
         updated_mock = (
-            mock_function if mock_function is not None else endpoint.mock_function
+            mock_function.to(PublicAPIEndpoint)
+            if mock_function is not None
+            else endpoint.mock_function
         )
         updated_private = (
-            private_function
+            private_function.to(PrivateAPIEndpoint)
             if private_function is not None
             else endpoint.private_function
         )
 
         try:
             endpoint_update = UpdateTwinAPIEndpoint(
                 path=endpoint_path,
                 mock_function=updated_mock,
                 private_function=updated_private,
+                endpoint_timeout=endpoint_timeout,
             )
         except ValidationError as e:
             return SyftError(message=str(e))
 
         endpoint.mock_function = endpoint_update.mock_function
         endpoint.private_function = endpoint_update.private_function
         endpoint.signature = updated_mock.signature
-        view_access = (
-            not hide_definition
-            if hide_definition is not None
-            else endpoint.mock_function.view_access
-        )
-        endpoint.mock_function.view_access = view_access
-        # Check if the endpoint has a private function
-        if endpoint.private_function:
-            endpoint.private_function.view_access = view_access
+        endpoint.endpoint_timeout = endpoint_update.endpoint_timeout
 
+        if hide_mock_definition is not None:
+            view_access = not hide_mock_definition
+            endpoint.mock_function.view_access = view_access
+
+        # save changes
         result = self.stash.upsert(context.credentials, endpoint=endpoint)
         if result.is_err():
             return SyftError(message=result.err())
 
         return SyftSuccess(message="Endpoint successfully updated.")
 
     @service_method(
@@ -217,14 +241,153 @@
         for api_endpoint in all_api_endpoints:
             api_endpoint_view.append(
                 api_endpoint.to(TwinAPIEndpointView, context=context)
             )
 
         return api_endpoint_view
 
+    @service_method(
+        path="api.call_in_jobs", name="call_in_jobs", roles=GUEST_ROLE_LEVEL
+    )
+    def call_in_jobs(
+        self,
+        context: AuthedServiceContext,
+        path: str,
+        *args: Any,
+        **kwargs: Any,
+    ) -> Any | SyftError:
+        """Call a Custom API Method in a Job"""
+        return self._call_in_jobs(context, "call", path, *args, **kwargs)
+
+    @service_method(
+        path="api.call_private_in_jobs",
+        name="call_private_in_jobs",
+        roles=GUEST_ROLE_LEVEL,
+    )
+    def call_private_in_jobs(
+        self,
+        context: AuthedServiceContext,
+        path: str,
+        *args: Any,
+        **kwargs: Any,
+    ) -> Any | SyftError:
+        """Call a Custom API Method in a Job"""
+        return self._call_in_jobs(context, "call_private", path, *args, **kwargs)
+
+    @service_method(
+        path="api.call_public_in_jobs",
+        name="call_public_in_jobs",
+        roles=GUEST_ROLE_LEVEL,
+    )
+    def call_public_in_jobs(
+        self,
+        context: AuthedServiceContext,
+        path: str,
+        *args: Any,
+        **kwargs: Any,
+    ) -> Any | SyftError:
+        """Call a Custom API Method in a Job"""
+        return self._call_in_jobs(context, "call_public", path, *args, **kwargs)
+
+    def _call_in_jobs(
+        self,
+        context: AuthedServiceContext,
+        method: str,
+        path: str,
+        *args: Any,
+        **kwargs: Any,
+    ) -> Any | SyftError:
+        custom_endpoint = self.get_code(
+            context=context,
+            endpoint_path=path,
+        )
+        if isinstance(custom_endpoint, SyftError):
+            return custom_endpoint
+
+        result = context.node.add_api_endpoint_execution_to_queue(
+            context.credentials,
+            method,
+            path,
+            worker_pool=custom_endpoint.worker_pool,
+            *args,
+            **kwargs,
+        )
+        if isinstance(result, SyftError):
+            return result
+        # relative
+        from ..job.job_stash import JobStatus
+
+        # So result is a Job object
+        job = result
+        job_service = context.node.get_service("jobservice")
+        job_id = job.id
+        # Question: For a small moment, when job status is updated, it doesn't return the job during the .get() as if
+        # it's not in the stash. Then afterwards if appears again. Is this a bug?
+
+        start = time.time()
+        # TODO: what can we do here?????
+        while (
+            job is None
+            or job.status == JobStatus.PROCESSING
+            or job.status == JobStatus.CREATED
+        ):
+            job = job_service.get(context, job_id)
+            time.sleep(0.1)
+            if (time.time() - custom_endpoint.endpoint_timeout) > start:
+                return SyftError(
+                    message=f"Function timed out in {custom_endpoint.endpoint_timeout} seconds. Get the Job with id: {job_id} to check results."
+                )
+
+        if job.status == JobStatus.COMPLETED:
+            return job.result
+        else:
+            return SyftError(message="Function failed to complete.")
+
+    @service_method(
+        path="api.get_public_context", name="get_public_context", roles=ADMIN_ROLE_LEVEL
+    )
+    def get_public_context(
+        self, context: AuthedServiceContext, path: str
+    ) -> dict[str, Any] | SyftError:
+        """Get specific public api context."""
+        custom_endpoint = self.get_code(
+            context=context,
+            endpoint_path=path,
+        )
+        if isinstance(custom_endpoint, SyftError):
+            return custom_endpoint
+
+        return custom_endpoint.mock_function.build_internal_context(context).to(
+            TwinAPIContextView
+        )
+
+    @service_method(
+        path="api.get_private_context",
+        name="get_private_context",
+        roles=ADMIN_ROLE_LEVEL,
+    )
+    def get_private_context(
+        self, context: AuthedServiceContext, path: str
+    ) -> dict[str, Any] | SyftError:
+        """Get specific private api context."""
+        custom_endpoint = self.get_code(
+            context=context,
+            endpoint_path=path,
+        )
+        if isinstance(custom_endpoint, SyftError):
+            return custom_endpoint
+
+        custom_endpoint.private_function = cast(
+            PrivateAPIEndpoint, custom_endpoint.private_function
+        )
+
+        return custom_endpoint.private_function.build_internal_context(context).to(
+            TwinAPIContextView
+        )
+
     @service_method(path="api.get_all", name="get_all", roles=ADMIN_ROLE_LEVEL)
     def get_all(
         self,
         context: AuthedServiceContext,
     ) -> list[TwinAPIEndpoint] | SyftError:
         """Get all API endpoints."""
         result = self.stash.get_all(context.credentials)
@@ -243,51 +406,97 @@
         """Call a Custom API Method"""
         custom_endpoint = self.get_code(
             context=context,
             endpoint_path=path,
         )
         if isinstance(custom_endpoint, SyftError):
             return custom_endpoint
-        return custom_endpoint.exec(context, *args, **kwargs)
+
+        exec_result = custom_endpoint.exec(context, *args, **kwargs)
+
+        if isinstance(exec_result, SyftError):
+            return Ok(exec_result)
+
+        action_obj = ActionObject.from_obj(exec_result)
+        action_service = cast(ActionService, context.node.get_service(ActionService))
+        result = action_service.set_result_to_store(
+            context=context,
+            result_action_object=action_obj,
+            has_result_read_permission=True,
+        )
+        if result.is_err():
+            return SyftError(message=f"Failed to set result to store: {result.err()}")
+
+        return Ok(result.ok())
 
     @service_method(path="api.call_public", name="call_public", roles=GUEST_ROLE_LEVEL)
     def call_public(
         self,
         context: AuthedServiceContext,
         path: str,
         *args: Any,
         **kwargs: Any,
-    ) -> SyftSuccess | SyftError:
+    ) -> ActionObject | SyftError:
         """Call a Custom API Method in public mode"""
         custom_endpoint = self.get_code(
             context=context,
             endpoint_path=path,
         )
         if isinstance(custom_endpoint, SyftError):
             return custom_endpoint
-        return custom_endpoint.exec_mock_function(context, *args, **kwargs)
+        exec_result = custom_endpoint.exec_mock_function(context, *args, **kwargs)
+
+        if isinstance(exec_result, SyftError):
+            return Ok(exec_result)
+
+        action_obj = ActionObject.from_obj(exec_result)
+        action_service = cast(ActionService, context.node.get_service(ActionService))
+        result = action_service.set_result_to_store(
+            context=context,
+            result_action_object=action_obj,
+            has_result_read_permission=True,
+        )
+        if result.is_err():
+            return SyftError(message=f"Failed to set result to store: {result.err()}")
+
+        return Ok(result.ok())
 
     @service_method(
         path="api.call_private", name="call_private", roles=GUEST_ROLE_LEVEL
     )
     def call_private(
         self,
         context: AuthedServiceContext,
         path: str,
         *args: Any,
         **kwargs: Any,
-    ) -> SyftSuccess | SyftError:
+    ) -> ActionObject | SyftError:
         """Call a Custom API Method in private mode"""
         custom_endpoint = self.get_code(
             context=context,
             endpoint_path=path,
         )
-        if not isinstance(custom_endpoint, SyftError):
-            result = custom_endpoint.exec_private_function(context, *args, **kwargs)
-        return result
+        if isinstance(custom_endpoint, SyftError):
+            return custom_endpoint
+
+        exec_result = custom_endpoint.exec_private_function(context, *args, **kwargs)
+
+        if isinstance(exec_result, SyftError):
+            return Ok(exec_result)
+
+        action_obj = ActionObject.from_obj(exec_result)
+
+        action_service = cast(ActionService, context.node.get_service(ActionService))
+        result = action_service.set_result_to_store(
+            context=context, result_action_object=action_obj
+        )
+        if result.is_err():
+            return SyftError(message=f"Failed to set result to store: {result.err()}")
+
+        return Ok(result.ok())
 
     @service_method(
         path="api.exists",
         name="exists",
     )
     def exists(
         self, context: AuthedServiceContext, uid: UID
```

### Comparing `syft-0.8.7b2/src/syft/service/api/api_stash.py` & `syft-0.8.7b3/src/syft/service/api/api_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/blob_storage/remote_profile.py` & `syft-0.8.7b3/src/syft/service/blob_storage/remote_profile.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/blob_storage/service.py` & `syft-0.8.7b3/src/syft/service/blob_storage/service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/blob_storage/stash.py` & `syft-0.8.7b3/src/syft/service/blob_storage/stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/code/code_parse.py` & `syft-0.8.7b3/src/syft/service/code/code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/code/status_service.py` & `syft-0.8.7b3/src/syft/service/code/status_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/code/user_code.py` & `syft-0.8.7b3/src/syft/service/code/user_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,14 +276,25 @@
     input_kwargs: list[str]
     enclave_metadata: EnclaveMetadata | None = None
     submit_time: DateTime | None = None
     uses_domain: bool = False  # tracks if the code calls domain.something, variable is set during parsing
     nested_codes: dict[str, tuple[LinkedObject, dict]] | None = {}
     worker_pool_name: str | None = None
 
+    __table_coll_widths__ = [
+        "min-content",
+        "auto",
+        "auto",
+        "auto",
+        "auto",
+        "auto",
+        "auto",
+        "auto",
+    ]
+
     __attr_searchable__: ClassVar[list[str]] = [
         "user_verify_key",
         "service_func_name",
         "code_hash",
     ]
     __attr_unique__: ClassVar[list[str]] = []
     __repr_attrs__: ClassVar[list[str]] = [
```

### Comparing `syft-0.8.7b2/src/syft/service/code/user_code_parse.py` & `syft-0.8.7b3/src/syft/service/code/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/code/user_code_service.py` & `syft-0.8.7b3/src/syft/service/code/user_code_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,17 +380,15 @@
             ):
                 mock_kwargs[k] = v
         return mock_kwargs
 
     def is_execution_on_owned_args(
         self, kwargs: dict[str, Any], context: AuthedServiceContext
     ) -> bool:
-        return bool(kwargs) and len(self.keep_owned_kwargs(kwargs, context)) == len(
-            kwargs
-        )
+        return len(self.keep_owned_kwargs(kwargs, context)) == len(kwargs)
 
     @service_method(path="code.call", name="call", roles=GUEST_ROLE_LEVEL)
     def call(
         self, context: AuthedServiceContext, uid: UID, **kwargs: Any
     ) -> CachedSyftObject | ActionObject | SyftSuccess | SyftError:
         """Call a User Code Function"""
         kwargs.pop("result_id", None)
@@ -413,15 +411,20 @@
             if code_result.is_err():
                 return code_result
             code: UserCode = code_result.ok()
 
             # Set Permissions
             if self.is_execution_on_owned_args(kwargs, context):
                 if self.is_execution_on_owned_args_allowed(context):
+                    # handles the case: if we have 1 or more owned args and execution permission
+                    # handles the case: if we have 0 owned args and execution permission
                     context.has_execute_permissions = True
+                elif len(kwargs) == 0:
+                    # handles the case: if we have 0 owned args and execution permission
+                    pass
                 else:
                     return Err(
                         "You do not have the permissions for mock execution, please contact the admin"
                     )
             override_execution_permission = (
                 context.has_execute_permissions or context.role == ServiceRole.ADMIN
             )
@@ -529,14 +532,19 @@
             # code.output_policy = output_policy
             # res = self.update_code_state(context, code)
             # print(res)
 
             has_result_read_permission = context.extra_kwargs.get(
                 "has_result_read_permission", False
             )
+
+            # TODO: Just to fix the issue with the current implementation
+            if context.role == ServiceRole.ADMIN:
+                has_result_read_permission = True
+
             if isinstance(result, TwinObject):
                 if has_result_read_permission:
                     return Ok(result.private)
                 else:
                     return Ok(result.mock)
             elif result.is_mock:
                 return Ok(result)
```

### Comparing `syft-0.8.7b2/src/syft/service/code/user_code_stash.py` & `syft-0.8.7b3/src/syft/service/code/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/code/utils.py` & `syft-0.8.7b3/src/syft/service/code/utils.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/code_history/code_history.py` & `syft-0.8.7b3/src/syft/service/code_history/code_history.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/code_history/code_history_service.py` & `syft-0.8.7b3/src/syft/service/code_history/code_history_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/code_history/code_history_stash.py` & `syft-0.8.7b3/src/syft/service/code_history/code_history_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/context.py` & `syft-0.8.7b3/src/syft/service/context.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/data_subject/data_subject.py` & `syft-0.8.7b3/src/syft/service/data_subject/data_subject.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/data_subject/data_subject_member.py` & `syft-0.8.7b3/src/syft/service/data_subject/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/data_subject/data_subject_member_service.py` & `syft-0.8.7b3/src/syft/service/data_subject/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/data_subject/data_subject_service.py` & `syft-0.8.7b3/src/syft/service/data_subject/data_subject_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/dataset/dataset.py` & `syft-0.8.7b3/src/syft/service/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/dataset/dataset_service.py` & `syft-0.8.7b3/src/syft/service/dataset/dataset_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/dataset/dataset_stash.py` & `syft-0.8.7b3/src/syft/service/dataset/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/enclave/enclave_service.py` & `syft-0.8.7b3/src/syft/service/enclave/enclave_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/job/job_service.py` & `syft-0.8.7b3/src/syft/service/job/job_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         self.stash = JobStash(store=store)
 
     @service_method(
         path="job.get",
         name="get",
         roles=GUEST_ROLE_LEVEL,
     )
-    def get(self, context: AuthedServiceContext, uid: UID) -> list[Job] | SyftError:
+    def get(self, context: AuthedServiceContext, uid: UID) -> Job | SyftError:
         res = self.stash.get_by_uid(context.credentials, uid=uid)
         if res.is_err():
             return SyftError(message=res.err())
         else:
             res = res.ok()
             return res
```

### Comparing `syft-0.8.7b2/src/syft/service/job/job_stash.py` & `syft-0.8.7b3/src/syft/service/job/job_stash.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # stdlib
 from datetime import datetime
 from datetime import timedelta
 from enum import Enum
+import random
+from string import Template
 from typing import Any
 
 # third party
 from pydantic import field_validator
 from pydantic import model_validator
 from result import Err
 from result import Ok
@@ -23,46 +25,61 @@
 from ...store.document_store import DocumentStore
 from ...store.document_store import PartitionKey
 from ...store.document_store import PartitionSettings
 from ...store.document_store import QueryKeys
 from ...store.document_store import UIDPartitionKey
 from ...types.datetime import DateTime
 from ...types.syft_object import SYFT_OBJECT_VERSION_2
-from ...types.syft_object import SYFT_OBJECT_VERSION_4
+from ...types.syft_object import SYFT_OBJECT_VERSION_5
 from ...types.syft_object import SyftObject
-from ...types.syft_object import short_uid
 from ...types.syncable_object import SyncableSyftObject
 from ...types.uid import UID
 from ...util import options
 from ...util.colors import SURFACE
 from ...util.markdown import as_markdown_code
 from ...util.telemetry import instrument
 from ...util.util import prompt_warning_message
 from ..action.action_object import Action
 from ..action.action_object import ActionObject
 from ..action.action_permissions import ActionObjectPermission
 from ..response import SyftError
 from ..response import SyftNotReady
 from ..response import SyftSuccess
 from ..user.user import UserView
+from .html_template import job_repr_template
 
 
 @serializable()
 class JobStatus(str, Enum):
     CREATED = "created"
     PROCESSING = "processing"
     ERRORED = "errored"
     COMPLETED = "completed"
     INTERRUPTED = "interrupted"
 
 
+def center_content(text: Any) -> str:
+    if isinstance(text, str):
+        text = text.replace("\n", "<br>")
+    center_div = f"""
+    <div style="
+        display: flex;
+        justify-content: center;
+        align-items: center; width: 100%; height: 100%;">
+        {text}
+    </div>
+    """
+    center_div = center_div.replace("\n", "")
+    return center_div
+
+
 @serializable()
 class Job(SyncableSyftObject):
     __canonical_name__ = "JobItem"
-    __version__ = SYFT_OBJECT_VERSION_4
+    __version__ = SYFT_OBJECT_VERSION_5
 
     id: UID
     node_uid: UID
     result: Any | None = None
     resolved: bool = False
     status: JobStatus = JobStatus.CREATED
     log_id: UID | None = None
@@ -71,25 +88,36 @@
     current_iter: int | None = None
     creation_time: str | None = None
     action: Action | None = None
     job_pid: int | None = None
     job_worker_id: UID | None = None
     updated_at: DateTime | None = None
     user_code_id: UID | None = None
+    requested_by: UID | None = None
 
     __attr_searchable__ = ["parent_job_id", "job_worker_id", "status", "user_code_id"]
     __repr_attrs__ = [
         "id",
         "result",
         "resolved",
         "progress",
         "creation_time",
         "user_code_name",
     ]
     __exclude_sync_diff_attrs__ = ["action", "node_uid"]
+    __table_coll_widths__ = [
+        "min-content",
+        "auto",
+        "auto",
+        "auto",
+        "auto",
+        "auto",
+        "auto",
+    ]
+    __syft_include_id_coll_repr__ = False
 
     @field_validator("creation_time")
     @classmethod
     def check_time(cls, time: Any) -> Any:
         return str(datetime.now()) if time is None else time
 
     @model_validator(mode="after")
@@ -403,37 +431,86 @@
         else:
             print(results_str)
             return None
 
     # def __repr__(self) -> str:
     #     return f"<Job: {self.id}>: {self.status}"
 
+    def status_badge(self) -> dict[str, str]:
+        status = self.status
+        if status in [JobStatus.COMPLETED]:
+            badge_color = "label-green"
+        elif status in [JobStatus.PROCESSING]:
+            badge_color = "label-orange"
+        elif status in [JobStatus.CREATED]:
+            badge_color = "label-gray"
+        elif status in [JobStatus.ERRORED, JobStatus.INTERRUPTED]:
+            badge_color = "label-red"
+        else:
+            badge_color = "label-orange"
+        return {"value": status.upper(), "type": badge_color}
+
+    def summary_html(self) -> str:
+        # TODO: Fix id for buttons
+        # relative
+        from ...util.notebook_ui.components.sync import CopyIDButton
+
+        try:
+            # type_html = f'<div class="label {self.type_badge_class()}">{self.object_type_name.upper()}</div>'
+            description_html = (
+                f"<span class='syncstate-description'>{self.user_code_name}</span>"
+            )
+            worker_summary = ""
+            if self.job_worker_id:
+                worker_copy_button = CopyIDButton(
+                    copy_text=str(self.job_worker_id), max_width=60
+                )
+                worker_summary = f"""
+                <div style="display: table-row">
+                    <span class='syncstate-col-footer'>{'on worker'}
+                    {worker_copy_button.to_html()}</span>
+                </div>
+                """
+
+            summary_html = f"""
+                <div style="display: flex; gap: 8px; justify-content: start; width: 100%;">
+                    {description_html}
+                    <div style="display: flex; gap: 8px; justify-content: end; width: 100%;">
+                        {CopyIDButton(copy_text=str(self.id), max_width=60).to_html()}
+                    </div>
+                </div>
+                <div style="display: table-row">
+                <span class='syncstate-col-footer'>{self.creation_time[:-7] if self.creation_time else ''}</span>
+                </div>
+                {worker_summary}
+                """
+            summary_html = summary_html.replace("\n", "")
+        except Exception as e:
+            print("Failed to build table", e)
+            raise
+        return summary_html
+
     def _coll_repr_(self) -> dict[str, Any]:
         logs = self.logs(_print=False, stderr=False)
         if logs is not None:
             log_lines = logs.split("\n")
         subjobs = self.subjobs
         if len(log_lines) > 2:
             logs = f"... ({len(log_lines)} lines)\n" + "\n".join(log_lines[-2:])
 
-        created_time = self.creation_time[:-7] if self.creation_time is not None else ""
+        def default_value(value: str) -> str:
+            return value if value else "--"
+
         return {
-            "status": f"{self.action_display_name}: {self.status}"
-            + (
-                f"\non worker {short_uid(self.job_worker_id)}"
-                if self.job_worker_id
-                else ""
-            ),
-            "progress": self.progress,
-            "eta": self.eta_string,
-            "created": f"{created_time} by {self.owner.email}",
-            "logs": logs,
-            # "result": result,
-            # "parent_id": str(self.parent_job_id) if self.parent_job_id else "-",
-            "subjobs": len(subjobs),
+            "Status": self.status_badge(),
+            "Job": self.summary_html(),
+            "# Subjobs": center_content(default_value(len(subjobs))),
+            "Progress": center_content(default_value(self.progress)),
+            "ETA": center_content(default_value(self.eta_string)),
+            "Logs": center_content(default_value(logs)),
         }
 
     @property
     def has_parent(self) -> bool:
         return self.parent_job_id is not None
 
     def _repr_markdown_(self, wrap_as_python: bool = True, indent: int = 0) -> str:
@@ -454,14 +531,142 @@
     result: {self.result.__str__()}
     logs:
 
 {logs_w_linenr}
     """
         return as_markdown_code(md)
 
+    @property
+    def requesting_user(self) -> UserView | SyftError:
+        api = APIRegistry.api_for(
+            node_uid=self.syft_node_location,
+            user_verify_key=self.syft_client_verify_key,
+        )
+        if api is None:
+            return SyftError(
+                message=f"Can't access Syft API. You must login to {self.syft_node_location}"
+            )
+        return api.services.user.view(self.requested_by)
+
+    @property
+    def node_name(self) -> str | SyftError | None:
+        api = APIRegistry.api_for(
+            node_uid=self.syft_node_location,
+            user_verify_key=self.syft_client_verify_key,
+        )
+        if api is None:
+            return SyftError(
+                message=f"Can't access Syft API. You must login to {self.syft_node_location}"
+            )
+        return api.node_name
+
+    @property
+    def parent(self) -> Self | SyftError:
+        api = APIRegistry.api_for(
+            node_uid=self.syft_node_location,
+            user_verify_key=self.syft_client_verify_key,
+        )
+        if api is None:
+            return SyftError(
+                message=f"Can't access Syft API. You must login to {self.syft_node_location}"
+            )
+        return api.services.job.get(self.parent_job_id)
+
+    @property
+    def ancestors_name_list(self) -> list[str] | SyftError:
+        if self.parent_job_id:
+            parent = self.parent
+            if isinstance(parent, SyftError):
+                return parent
+            parent_name_list = parent.ancestors_name_list
+            if isinstance(parent_name_list, SyftError):
+                return parent_name_list
+            parent_name_list.append(parent.user_code_name)
+            return parent_name_list
+        return []
+
+    def _repr_html_(self) -> str:
+        # relative
+        from ...util.notebook_ui.components.sync import CopyIDButton
+
+        identifier = random.randint(1, 2**32)  # nosec
+        result_tab_id = f"Result_{identifier}"
+        logs_tab_id = f"Logs_{identifier}"
+        job_type = "JOB" if not self.parent_job_id else "SUBJOB"
+        ancestor_name_list = self.ancestors_name_list
+        if isinstance(ancestor_name_list, SyftError):
+            return ancestor_name_list
+        api_header = f"{self.node_name}/jobs/" + "/".join(ancestor_name_list)
+        copy_id_button = CopyIDButton(copy_text=str(self.id), max_width=60)
+        button_html = copy_id_button.to_html()
+        creation_time = self.creation_time[:-7] if self.creation_time else "--"
+        updated_at = str(self.updated_at)[:-7] if self.updated_at else "--"
+
+        user_repr = "--"
+        if self.requested_by:
+            requesting_user = self.requesting_user
+            user_repr = f"{requesting_user.name} {requesting_user.email}"
+
+        worker_attr = ""
+        if self.job_worker_id:
+            worker = self.worker
+            worker_pool_id_button = CopyIDButton(
+                copy_text=str(worker.worker_pool_name), max_width=60
+            )
+            worker_attr = f"""
+                <div style="margin-top: 6px; margin-bottom: 6px;">
+                <span style="font-weight: 700; line-weight: 19.6px; font-size: 14px; font: 'Open Sans'">
+                    Worker Pool:</span>
+                    {worker.name} on worker {worker_pool_id_button.to_html()}
+                </div>
+            """
+
+        logs = self.logs(_print=False, stderr=False)
+        logs_lines = logs.split("\n") if logs else []
+        logs_lines_html = ""
+        for i, line in enumerate(logs_lines):
+            logs_lines_html += f"""
+                <tr style="width:100%">
+                    <td style="text-align: left;">
+                        <div style="margin-right:24px; align-text: center">
+                            {i}
+                        </div>
+                    </td>
+                    <td style="text-align: left;">
+                        <div style="align-text: left">
+                            {line}
+                        </div>
+                    </td>
+                </tr>
+            """
+
+        template = Template(job_repr_template)
+        return template.substitute(
+            uid=str(UID()),
+            grid_template_columns=None,
+            grid_template_cell_columns=None,
+            cols=0,
+            job_type=job_type,
+            api_header=api_header,
+            user_code_name=self.user_code_name,
+            button_html=button_html,
+            status=self.status.value.title(),
+            creation_time=creation_time,
+            user_rerp=user_repr,
+            updated_at=updated_at,
+            worker_attr=worker_attr,
+            no_subjobs=len(self.subjobs),
+            logs_tab_id=logs_tab_id,
+            result_tab_id=result_tab_id,
+            identifier=identifier,
+            logs_lines_html=logs_lines_html,
+            result=self.result,
+            user_repr=user_repr,
+        )
+
     def wait(
         self, job_only: bool = False, timeout: int | None = None
     ) -> Any | SyftNotReady:
         # stdlib
         from time import sleep
 
         api = APIRegistry.api_for(
@@ -510,15 +715,15 @@
 
         if self.resolved:
             return self.result
         return SyftNotReady(message=f"{self.id} not ready yet.")
 
     def get_sync_dependencies(self, context: AuthedServiceContext) -> list[UID]:  # type: ignore
         dependencies = []
-        if self.result is not None:
+        if self.result is not None and isinstance(self.result, ActionObject):
             dependencies.append(self.result.id.id)
 
         if self.log_id:
             dependencies.append(self.log_id)
 
         subjobs = self.get_subjobs(context)
         if isinstance(subjobs, SyftError):
@@ -655,19 +860,23 @@
     ) -> Result[Job | None, str]:
         res = self.get_all(credentials)
         if res.is_err():
             return res
         else:
             res = res.ok()
             # beautiful query
-            res = [x for x in res if x.result is not None and x.result.id.id == res_id]
+            res = [
+                x
+                for x in res
+                if isinstance(x.result, ActionObject) and x.result.id.id == res_id
+            ]
             if len(res) == 0:
                 return Ok(None)
             elif len(res) > 1:
-                return Err(message="multiple Jobs found")
+                return Err(SyftError(message="multiple Jobs found"))
             else:
                 return Ok(res[0])
 
     def set_placeholder(
         self,
         credentials: SyftVerifyKey,
         item: Job,
```

### Comparing `syft-0.8.7b2/src/syft/service/log/log.py` & `syft-0.8.7b3/src/syft/service/log/log.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/log/log_service.py` & `syft-0.8.7b3/src/syft/service/log/log_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from result import Ok
 
 # relative
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ...types.uid import UID
 from ...util.telemetry import instrument
+from ..action.action_permissions import StoragePermission
 from ..context import AuthedServiceContext
 from ..response import SyftError
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import TYPE_TO_SERVICE
 from ..service import service_method
 from ..user.user_roles import ADMIN_ROLE_LEVEL
@@ -130,15 +131,14 @@
 
     @service_method(
         path="log.has_storage_permission",
         name="has_storage_permission",
         roles=DATA_SCIENTIST_ROLE_LEVEL,
     )
     def has_storage_permission(self, context: AuthedServiceContext, uid: UID) -> bool:
-        result = self.stash.has_storage_permission(
-            uid,
-        )
+        permission = StoragePermission(uid=uid, node_uid=context.node.id)
+        result = self.stash.has_storage_permission(permission)
 
         return result
 
 
 TYPE_TO_SERVICE[SyftLog] = LogService
```

### Comparing `syft-0.8.7b2/src/syft/service/log/log_stash.py` & `syft-0.8.7b3/src/syft/service/log/log_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/metadata/metadata_service.py` & `syft-0.8.7b3/src/syft/service/metadata/metadata_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/metadata/migrations.py` & `syft-0.8.7b3/src/syft/service/metadata/migrations.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/metadata/node_metadata.py` & `syft-0.8.7b3/src/syft/service/metadata/node_metadata.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/network/network_service.py` & `syft-0.8.7b3/src/syft/service/network/network_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,41 +11,46 @@
 from ...abstract_node import NodeType
 from ...client.client import HTTPConnection
 from ...client.client import PythonConnection
 from ...client.client import SyftClient
 from ...node.credentials import SyftVerifyKey
 from ...node.worker_settings import WorkerSettings
 from ...serde.serializable import serializable
-from ...service.settings.settings import NodeSettingsV2
+from ...service.settings.settings import NodeSettings
 from ...store.document_store import BaseUIDStoreStash
 from ...store.document_store import DocumentStore
 from ...store.document_store import PartitionKey
 from ...store.document_store import PartitionSettings
 from ...store.document_store import QueryKeys
 from ...types.grid_url import GridURL
 from ...types.transforms import TransformContext
 from ...types.transforms import keep
+from ...types.transforms import make_set_default
 from ...types.transforms import transform
 from ...types.transforms import transform_method
 from ...types.uid import UID
 from ...util.telemetry import instrument
 from ...util.util import prompt_warning_message
 from ..context import AuthedServiceContext
 from ..data_subject.data_subject import NamePartitionKey
 from ..metadata.node_metadata import NodeMetadataV3
+from ..request.request import Request
+from ..request.request import SubmitRequest
+from ..request.request_service import RequestService
 from ..response import SyftError
 from ..response import SyftInfo
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import SERVICE_TO_TYPES
 from ..service import TYPE_TO_SERVICE
 from ..service import service_method
 from ..user.user_roles import DATA_OWNER_ROLE_LEVEL
 from ..user.user_roles import GUEST_ROLE_LEVEL
 from ..warnings import CRUDWarning
+from .association_request import AssociationRequestChange
 from .node_peer import NodePeer
 from .routes import HTTPNodeRoute
 from .routes import NodeRoute
 from .routes import NodeRouteType
 from .routes import PythonNodeRoute
 
 VerifyKeyPartitionKey = PartitionKey(key="verify_key", type_=SyftVerifyKey)
@@ -74,15 +79,15 @@
         self,
         credentials: SyftVerifyKey,
         peer: NodePeer,
         has_permission: bool = False,
     ) -> Result[NodePeer, str]:
         valid = self.check_type(peer, NodePeer)
         if valid.is_err():
-            return Err(message=valid.err())
+            return Err(SyftError(message=valid.err()))
         return super().update(credentials, peer)
 
     def create_or_update_peer(
         self, credentials: SyftVerifyKey, peer: NodePeer
     ) -> Result[NodePeer, str]:
         """
         Update the selected peer and its route priorities if the peer already exists
@@ -174,33 +179,31 @@
             self_node_route=remote_node_route,
             verify_key=remote_node_verify_key,
         )
 
         if isinstance(remote_res, SyftError):
             return remote_res
 
-        challenge_signature, remote_node_peer = remote_res
+        association_request_approved = not isinstance(remote_res, Request)
 
-        # Verifying if the challenge is valid
-        try:
-            remote_node_verify_key.verify_key.verify(
-                random_challenge, challenge_signature
-            )
-        except Exception as e:
-            return SyftError(message=str(e))
+        remote_node_peer = NodePeer.from_client(remote_client)
 
         # save the remote peer for later
         result = self.stash.create_or_update_peer(
             context.node.verify_key,
             remote_node_peer,
         )
         if result.is_err():
             return SyftError(message=str(result.err()))
 
-        return SyftSuccess(message="Routes Exchanged")
+        return (
+            SyftSuccess(message="Routes Exchanged")
+            if association_request_approved
+            else remote_res
+        )
 
     @service_method(path="network.add_peer", name="add_peer", roles=GUEST_ROLE_LEVEL)
     def add_peer(
         self,
         context: AuthedServiceContext,
         peer: NodePeer,
         challenge: bytes,
@@ -221,59 +224,35 @@
             )
 
         if verify_key != context.node.verify_key:
             return SyftError(
                 message="verify_key does not match the remote node's verify_key for add_peer"
             )
 
-        try:
-            remote_client = peer.client_with_context(context=context)
-            if remote_client.is_err():
-                return SyftError(
-                    message=f"Failed to create remote client for peer: "
-                    f"{peer.id}. Error: {remote_client.err()}"
-                )
-            remote_client = remote_client.ok()
-
-            random_challenge = secrets.token_bytes(16)
-            remote_res = remote_client.api.services.network.ping(
-                challenge=random_challenge
-            )
-        except Exception as e:
-            return SyftError(message="Remote Peer cannot ping peer:" + str(e))
-
-        if isinstance(remote_res, SyftError):
-            return remote_res
-
-        challenge_signature = remote_res
-
-        # Verifying if the challenge is valid
-        try:
-            peer.verify_key.verify_key.verify(random_challenge, challenge_signature)
-        except Exception as e:
-            return SyftError(message=str(e))
+        association_request_change = AssociationRequestChange(
+            self_node_route=self_node_route, challenge=challenge, remote_peer=peer
+        )
 
-        result = self.stash.create_or_update_peer(context.node.verify_key, peer)
-        if result.is_err():
-            return SyftError(message=str(result.err()))
+        submit_request = SubmitRequest(
+            changes=[association_request_change],
+            requesting_user_verify_key=context.credentials,
+        )
 
-        # this way they can match up who we are with who they think we are
-        # Sending a signed messages for the peer to verify
-        self_node_peer = self_node_route.validate_with_context(context=context)
+        request_submit_method = context.node.get_service_method(RequestService.submit)
 
-        if isinstance(self_node_peer, SyftError):
-            return self_node_peer
+        request = request_submit_method(context, submit_request)
 
-        # Q,TODO: Should the returned node peer also be signed
-        # as the challenge is already signed
-        challenge_signature = context.node.signing_key.signing_key.sign(
-            challenge
-        ).signature
+        if (
+            isinstance(request, Request)
+            and context.node.settings.association_request_auto_approval
+        ):
+            request_apply_method = context.node.get_service_method(RequestService.apply)
+            return request_apply_method(context, uid=request.id)
 
-        return [challenge_signature, self_node_peer]
+        return request
 
     @service_method(path="network.ping", name="ping", roles=GUEST_ROLE_LEVEL)
     def ping(
         self, context: AuthedServiceContext, challenge: bytes
     ) -> bytes | SyftError:
         """To check alivesness/authenticity of a peer"""
 
@@ -775,16 +754,24 @@
     ).as_container_host()
     return HTTPConnection(url=url, proxy_target_uid=obj.proxy_target_uid)
 
 
 @transform(NodeMetadataV3, NodePeer)
 def metadata_to_peer() -> list[Callable]:
     return [
-        keep(["id", "name", "verify_key", "node_type", "admin_email"]),
+        keep(
+            [
+                "id",
+                "name",
+                "verify_key",
+                "node_type",
+            ]
+        ),
+        make_set_default("admin_email", ""),
     ]
 
 
-@transform(NodeSettingsV2, NodePeer)
+@transform(NodeSettings, NodePeer)
 def settings_to_peer() -> list[Callable]:
     return [
         keep(["id", "name", "verify_key", "node_type", "admin_email"]),
     ]
```

### Comparing `syft-0.8.7b2/src/syft/service/network/node_peer.py` & `syft-0.8.7b3/src/syft/service/network/node_peer.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/network/routes.py` & `syft-0.8.7b3/src/syft/service/network/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/notification/email_templates.py` & `syft-0.8.7b3/src/syft/service/notification/email_templates.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/notification/notification_service.py` & `syft-0.8.7b3/src/syft/service/notification/notification_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/notification/notification_stash.py` & `syft-0.8.7b3/src/syft/service/notification/notification_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/notification/notifications.py` & `syft-0.8.7b3/src/syft/service/notification/notifications.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/notifier/notifier.py` & `syft-0.8.7b3/src/syft/service/notifier/notifier.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/notifier/notifier_service.py` & `syft-0.8.7b3/src/syft/service/notifier/notifier_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/notifier/notifier_stash.py` & `syft-0.8.7b3/src/syft/service/notifier/notifier_stash.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
+from ...service.response import SyftError
 from ...store.document_store import BaseStash
 from ...store.document_store import DocumentStore
 from ...store.document_store import PartitionKey
 from ...store.document_store import PartitionSettings
 from ...types.uid import UID
 from ...util.telemetry import instrument
 from ..action.action_permissions import ActionObjectPermission
@@ -46,38 +47,38 @@
                     None
                 )  # TODO: Stash shouldn't be empty after init. Return Err instead?
             result = settings[
                 0
             ]  # TODO: Should we check if theres more than one? => Report corruption
             return Ok(result)
         else:
-            return Err(message=result.err())
+            return Err(SyftError(message=result.err()))
 
     def set(
         self,
         credentials: SyftVerifyKey,
         settings: NotifierSettings,
         add_permissions: list[ActionObjectPermission] | None = None,
         add_storage_permission: bool = True,
         ignore_duplicates: bool = False,
     ) -> Result[NotifierSettings, Err]:
         result = self.check_type(settings, self.object_type)
         # we dont use and_then logic here as it is hard because of the order of the arguments
         if result.is_err():
-            return Err(message=result.err())
+            return Err(SyftError(message=result.err()))
         return super().set(
             credentials=credentials, obj=result.ok()
         )  # TODO check if result isInstance(Ok)
 
     def update(
         self,
         credentials: SyftVerifyKey,
         settings: NotifierSettings,
         has_permission: bool = False,
     ) -> Result[NotifierSettings, Err]:
         result = self.check_type(settings, self.object_type)
         # we dont use and_then logic here as it is hard because of the order of the arguments
         if result.is_err():
-            return Err(message=result.err())
+            return Err(SyftError(message=result.err()))
         return super().update(
             credentials=credentials, obj=result.ok()
         )  # TODO check if result isInstance(Ok)
```

### Comparing `syft-0.8.7b2/src/syft/service/notifier/smtp_client.py` & `syft-0.8.7b3/src/syft/service/notifier/smtp_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/object_search/migration_state_service.py` & `syft-0.8.7b3/src/syft/service/object_search/migration_state_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/object_search/object_migration_state.py` & `syft-0.8.7b3/src/syft/service/object_search/object_migration_state.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/output/output_service.py` & `syft-0.8.7b3/src/syft/service/output/output_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         if res.is_err():
             return res
         else:
             res = res.ok()
             if len(res) == 0:
                 return Ok(None)
             elif len(res) > 1:
-                return Err(message="Too many outputs found")
+                return Err(SyftError(message="Too many outputs found"))
             else:
                 return Ok(res[0])
 
     def get_by_output_policy_id(
         self, credentials: SyftVerifyKey, output_policy_id: UID
     ) -> Result[list[ExecutionOutput], str]:
         qks = QueryKeys(
```

### Comparing `syft-0.8.7b2/src/syft/service/policy/policy.py` & `syft-0.8.7b3/src/syft/service/policy/policy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/policy/policy_service.py` & `syft-0.8.7b3/src/syft/service/policy/policy_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/policy/user_policy_stash.py` & `syft-0.8.7b3/src/syft/service/policy/user_policy_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/project/project.py` & `syft-0.8.7b3/src/syft/service/project/project.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/project/project_service.py` & `syft-0.8.7b3/src/syft/service/project/project_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/project/project_stash.py` & `syft-0.8.7b3/src/syft/service/project/project_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/queue/base_queue.py` & `syft-0.8.7b3/src/syft/service/queue/base_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/queue/queue.py` & `syft-0.8.7b3/src/syft/service/queue/queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,17 +193,18 @@
             node_uid=worker.id,
             context=context,
             user_verify_key=credentials,
         )
 
         result: Any = call_method(context, *queue_item.args, **queue_item.kwargs)
 
+        status = Status.COMPLETED
+        job_status = JobStatus.COMPLETED
+
         if isinstance(result, Ok):
-            status = Status.COMPLETED
-            job_status = JobStatus.COMPLETED
             result = result.ok()
         elif isinstance(result, SyftError) or isinstance(result, Err):
             status = Status.ERRORED
             job_status = JobStatus.ERRORED
     except Exception as e:  # nosec
         status = Status.ERRORED
         job_status = JobStatus.ERRORED
```

### Comparing `syft-0.8.7b2/src/syft/service/queue/queue_service.py` & `syft-0.8.7b3/src/syft/service/queue/queue_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/queue/queue_stash.py` & `syft-0.8.7b3/src/syft/service/queue/queue_stash.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from ...store.document_store import BaseStash
 from ...store.document_store import DocumentStore
 from ...store.document_store import PartitionKey
 from ...store.document_store import PartitionSettings
 from ...store.document_store import QueryKeys
 from ...store.document_store import UIDPartitionKey
 from ...store.linked_obj import LinkedObject
+from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SYFT_OBJECT_VERSION_3
 from ...types.syft_object import SYFT_OBJECT_VERSION_4
 from ...types.syft_object import SyftObject
 from ...types.uid import UID
 from ...util.telemetry import instrument
 from ..action.action_permissions import ActionObjectPermission
 from ..response import SyftError
@@ -83,14 +84,23 @@
     __canonical_name__ = "ActionQueueItem"
     __version__ = SYFT_OBJECT_VERSION_3
 
     method: str = "execute"
     service: str = "actionservice"
 
 
+@serializable()
+class APIEndpointQueueItem(QueueItem):
+    __canonical_name__ = "APIEndpointQueueItem"
+    __version__ = SYFT_OBJECT_VERSION_1
+
+    method: str
+    service: str = "apiservice"
+
+
 @instrument
 @serializable()
 class QueueStash(BaseStash):
     object_type = QueueItem
     settings: PartitionSettings = PartitionSettings(
         name=QueueItem.__canonical_name__, object_type=QueueItem
     )
```

### Comparing `syft-0.8.7b2/src/syft/service/queue/zmq_queue.py` & `syft-0.8.7b3/src/syft/service/queue/zmq_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/request/request.py` & `syft-0.8.7b3/src/syft/service/request/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         return self._run(context=context, apply=True)
 
     def undo(self, context: ChangeContext) -> Result[SyftSuccess, SyftError]:
         return self._run(context=context, apply=False)
 
     def __repr_syft_nested__(self) -> str:
         return f"Apply <b>{self.apply_permission_type}</b> to \
-            <i>{self.linked_obj.object_type.__canonical_name__}:{self.linked_obj.object_uid.short()}</i>"
+<i>{self.linked_obj.object_type.__canonical_name__}:{self.linked_obj.object_uid.short()}</i>."
 
 
 @serializable()
 class CreateCustomImageChange(Change):
     __canonical_name__ = "CreateCustomImageChange"
     __version__ = SYFT_OBJECT_VERSION_2
 
@@ -343,14 +343,22 @@
     request_time: DateTime
     updated_at: DateTime | None = None
     node_uid: UID
     request_hash: str
     changes: list[Change]
     history: list[ChangeStatus] = []
 
+    __table_coll_widths__ = [
+        "min-content",
+        "auto",
+        "auto",
+        "auto",
+        "auto",
+    ]
+
     __attr_searchable__ = [
         "requesting_user_verify_key",
         "approving_user_verify_key",
     ]
     __attr_unique__ = ["request_hash"]
     __repr_attrs__ = [
         "request_time",
@@ -389,18 +397,20 @@
                 [f"<strong>{x}</strong>" for x in self.code.output_reader_names]
             )
             shared_with_line += (
                 f"<p><strong>Custom Policy: </strong> "
                 f"outputs are <strong>shared</strong> with the owners of {owners_string} once computed"
             )
 
+        node_info = ""
         if api is not None:
             metadata = api.services.metadata.get_metadata()
             node_name = api.node_name.capitalize() if api.node_name is not None else ""
             node_type = metadata.node_type.value.capitalize()
+            node_info = f"<p><strong>Requested on: </strong> {node_name} of type <strong>{node_type}</strong></p>"
 
         email_str = (
             f"({self.requesting_user_email})" if self.requesting_user_email else ""
         )
         institution_str = (
             f"<strong>Institution:</strong> {self.requesting_user_institution}"
             if self.requesting_user_institution
@@ -414,22 +424,34 @@
             <div class='syft-request'>
                 <h3>Request</h3>
                 <p><strong>Id: </strong>{self.id}</p>
                 <p><strong>Request time: </strong>{self.request_time}</p>
                 {updated_at_line}
                 {shared_with_line}
                 <p><strong>Status: </strong>{self.status}</p>
-                <p><strong>Requested on: </strong> {node_name} of type <strong> \
-                    {node_type}</strong></p>
+                {node_info}
                 <p><strong>Requested by:</strong> {self.requesting_user_name} {email_str} {institution_str}</p>
                 <p><strong>Changes: </strong> {str_changes}</p>
             </div>
 
             """
 
+    @property
+    def html_description(self) -> str:
+        desc = " ".join([x.__repr_syft_nested__() for x in self.changes])
+        # desc = desc.replace('\n', '')
+        # desc = desc.replace('<br>', '\n')
+        desc = desc.replace(". ", ".\n\n")
+        desc = desc.replace("<b>", "")
+        desc = desc.replace("</b>", "")
+        desc = desc.replace("<i>", "")
+        desc = desc.replace("</i>", "")
+
+        return desc
+
     def _coll_repr_(self) -> dict[str, str | dict[str, str]]:
         if self.status == RequestStatus.APPROVED:
             badge_color = "badge-green"
         elif self.status == RequestStatus.PENDING:
             badge_color = "badge-gray"
         else:
             badge_color = "badge-red"
@@ -439,15 +461,15 @@
         user_data = [
             self.requesting_user_name,
             self.requesting_user_email,
             self.requesting_user_institution,
         ]
 
         return {
-            "Description": " ".join([x.__repr_syft_nested__() for x in self.changes]),
+            "Description": self.html_description,
             "Requested By": "\n".join(user_data),
             "Status": status_badge,
         }
 
     @property
     def code_id(self) -> UID:
         for change in self.changes:
@@ -1189,23 +1211,23 @@
         return msg
 
     def __repr_syft_nested__(self) -> str:
         msg = (
             f"Request to change <b>{self.code.service_func_name}</b> "
             f"(Pool Id: <b>{self.code.worker_pool_name}</b>) "
         )
-        msg += "to permission <b>RequestStatus.APPROVED</b>"
+        msg += "to permission <strong>RequestStatus.APPROVED.</strong>"
         if self.nested_solved:
             if self.link.nested_codes == {}:  # type: ignore
-                msg += ". No nested requests"
+                msg += "No nested requests."
             else:
-                msg += ".<br><br>This change requests the following nested functions calls:<br>"
+                msg += "<br><br>This change requests the following nested functions calls:<br>"
                 msg += self.nested_repr()
         else:
-            msg += ". Nested Requests not resolved"
+            msg += "Nested Requests not resolved."
         return msg
 
     def _repr_markdown_(self, wrap_as_python: bool = True, indent: int = 0) -> str:
         code = self.code
         input_policy_type = (
             code.input_policy_type.__canonical_name__
             if code.input_policy_type is not None
```

### Comparing `syft-0.8.7b2/src/syft/service/request/request_service.py` & `syft-0.8.7b3/src/syft/service/request/request_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # stdlib
 
 # third party
-from result import Err
-from result import Ok
 
 # relative
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ...store.linked_obj import LinkedObject
 from ...types.uid import UID
 from ...util.telemetry import instrument
@@ -87,19 +85,21 @@
                         linked_obj=link,
                         notifier_types=[NOTIFIERS.EMAIL],
                         email_template=RequestEmailTemplate,
                     )
                     method = context.node.get_service_method(NotificationService.send)
                     result = method(context=context, notification=message)
                     if isinstance(result, Notification):
-                        return Ok(request)
+                        return request
                     else:
-                        return Err(result)
+                        return SyftError(
+                            message=f"Failed to send notification: {result.err()}"
+                        )
 
-                return Ok(request)
+                return request
 
             if result.is_err():
                 return SyftError(message=str(result.err()))
             return result.ok()
         except Exception as e:
             print("Failed to submit Request", e)
             raise e
```

### Comparing `syft-0.8.7b2/src/syft/service/request/request_stash.py` & `syft-0.8.7b3/src/syft/service/request/request_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/response.py` & `syft-0.8.7b3/src/syft/service/response.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/service.py` & `syft-0.8.7b3/src/syft/service/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+# future
+from __future__ import annotations
+
 # stdlib
 from collections import defaultdict
 from collections.abc import Callable
 from copy import deepcopy
 from functools import partial
 import inspect
 from inspect import Parameter
 from typing import Any
 from typing import TYPE_CHECKING
-from typing import Union
 
 # third party
 from result import Ok
 from result import OkErr
 from typing_extensions import Self
 
 # relative
@@ -437,15 +439,15 @@
         return cls.__object_transform_registry__[mapping_string]
 
 
 def from_api_or_context(
     func_or_path: str,
     syft_node_location: UID | None = None,
     syft_client_verify_key: SyftVerifyKey | None = None,
-) -> Union["APIModule", SyftError, partial] | None:
+) -> APIModule | SyftError | partial | None:
     # relative
     from ..client.api import APIRegistry
     from ..node.node import AuthNodeContextRegistry
 
     if callable(func_or_path):
         func_or_path = func_or_path.__qualname__
```

### Comparing `syft-0.8.7b2/src/syft/service/settings/settings_service.py` & `syft-0.8.7b3/src/syft/service/settings/settings_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # stdlib
 
 # stdlib
 
+# stdlib
+
 # third party
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
 from ...serde.serializable import serializable
@@ -15,16 +17,16 @@
 from ..context import UnauthedServiceContext
 from ..response import SyftError
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import service_method
 from ..user.user_roles import ADMIN_ROLE_LEVEL
 from ..warnings import HighSideCRUDWarning
+from .settings import NodeSettings
 from .settings import NodeSettingsUpdate
-from .settings import NodeSettingsV2
 from .settings_stash import SettingsStash
 
 
 @serializable()
 class SettingsService(AbstractService):
     store: DocumentStore
     stash: SettingsStash
@@ -46,33 +48,32 @@
             result = settings[0]
             return Ok(result)
         else:
             return SyftError(message=result.err())
 
     @service_method(path="settings.set", name="set")
     def set(
-        self, context: AuthedServiceContext, settings: NodeSettingsV2
+        self, context: AuthedServiceContext, settings: NodeSettings
     ) -> Result[Ok, Err]:
         """Set a new the Node Settings"""
-        print("Here!")
         result = self.stash.set(context.credentials, settings)
         if result.is_ok():
             return result
         else:
             return SyftError(message=result.err())
 
     @service_method(path="settings.update", name="update")
     def update(
         self, context: AuthedServiceContext, settings: NodeSettingsUpdate
     ) -> Result[Ok, Err]:
         result = self.stash.get_all(context.credentials)
         if result.is_ok():
             current_settings = result.ok()
             if len(current_settings) > 0:
-                new_settings = current_settings[0].copy(
+                new_settings = current_settings[0].model_copy(
                     update=settings.to_dict(exclude_empty=True)
                 )
                 update_result = self.stash.update(context.credentials, new_settings)
                 if update_result.is_ok():
                     return result
                 else:
                     return SyftError(message=update_result.err())
@@ -134,7 +135,24 @@
         result = method(context=context, settings=settings)
 
         if result.is_err():
             return SyftError(message=f"Failed to update settings: {result.err()}")
 
         message = "enabled" if enable else "disabled"
         return SyftSuccess(message=f"Registration feature successfully {message}")
+
+    @service_method(
+        path="settings.allow_association_request_auto_approval",
+        name="allow_association_request_auto_approval",
+    )
+    def allow_association_request_auto_approval(
+        self, context: AuthedServiceContext, enable: bool
+    ) -> SyftSuccess | SyftError:
+        new_settings = NodeSettingsUpdate(association_request_auto_approval=enable)
+        result = self.update(context, settings=new_settings)
+        if result.is_err():
+            return SyftError(message=result.err())
+
+        message = "enabled" if enable else "disabled"
+        return SyftSuccess(
+            message="Association request auto-approval successfully " + message
+        )
```

### Comparing `syft-0.8.7b2/src/syft/service/settings/settings_stash.py` & `syft-0.8.7b3/src/syft/service/settings/settings_stash.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,49 +9,49 @@
 from ...store.document_store import BaseUIDStoreStash
 from ...store.document_store import DocumentStore
 from ...store.document_store import PartitionKey
 from ...store.document_store import PartitionSettings
 from ...types.uid import UID
 from ...util.telemetry import instrument
 from ..action.action_permissions import ActionObjectPermission
-from .settings import NodeSettingsV2
+from .settings import NodeSettings
 
 NamePartitionKey = PartitionKey(key="name", type_=str)
 ActionIDsPartitionKey = PartitionKey(key="action_ids", type_=list[UID])
 
 
 @instrument
 @serializable()
 class SettingsStash(BaseUIDStoreStash):
-    object_type = NodeSettingsV2
+    object_type = NodeSettings
     settings: PartitionSettings = PartitionSettings(
-        name=NodeSettingsV2.__canonical_name__, object_type=NodeSettingsV2
+        name=NodeSettings.__canonical_name__, object_type=NodeSettings
     )
 
     def __init__(self, store: DocumentStore) -> None:
         super().__init__(store=store)
 
     def set(
         self,
         credentials: SyftVerifyKey,
-        settings: NodeSettingsV2,
+        settings: NodeSettings,
         add_permission: list[ActionObjectPermission] | None = None,
         add_storage_permission: bool = True,
         ignore_duplicates: bool = False,
-    ) -> Result[NodeSettingsV2, str]:
+    ) -> Result[NodeSettings, str]:
         res = self.check_type(settings, self.object_type)
         # we dont use and_then logic here as it is hard because of the order of the arguments
         if res.is_err():
             return res
         return super().set(credentials=credentials, obj=res.ok())
 
     def update(
         self,
         credentials: SyftVerifyKey,
-        settings: NodeSettingsV2,
+        settings: NodeSettings,
         has_permission: bool = False,
-    ) -> Result[NodeSettingsV2, str]:
+    ) -> Result[NodeSettings, str]:
         res = self.check_type(settings, self.object_type)
         # we dont use and_then logic here as it is hard because of the order of the arguments
         if res.is_err():
             return res
         return super().update(credentials=credentials, obj=res.ok())
```

### Comparing `syft-0.8.7b2/src/syft/service/sync/diff_state.py` & `syft-0.8.7b3/src/syft/service/sync/diff_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 from ..code.user_code import UserCode
 from ..code.user_code import UserCodeStatusCollection
 from ..job.job_stash import Job
 from ..log.log import SyftLog
 from ..output.output_service import ExecutionOutput
 from ..request.request import Request
 from ..response import SyftError
+from ..response import SyftSuccess
 from .sync_state import SyncState
 
 sketchy_tab = "‎ " * 4
 
 
 class AttrDiff(SyftObject):
     # version
@@ -532,14 +533,15 @@
     user_verify_key_low: SyftVerifyKey
     user_verify_key_high: SyftVerifyKey
 
     # Diffs are ordered in depth-first order,
     # the first diff is the root of the hierarchy
     global_diffs: dict[UID, ObjectDiff]
     global_roots: list[UID]
+    global_batches: list["ObjectDiffBatch"] | None = None
 
     hierarchy_levels: list[int]
     dependencies: dict[UID, list[UID]] = {}
     dependents: dict[UID, list[UID]] = {}
     decision: SyncDecision | None = None
     root_diff: ObjectDiff
     sync_direction: SyncDirection | None
@@ -670,29 +672,58 @@
             include_batch_root=include_batch_root,
         )
 
     def __hash__(self) -> int:
         diffs = self.get_dependents(include_roots=False)
         return sum(hash(x) for x in diffs)
 
+    def ignore(self) -> SyftSuccess | SyftError:
+        # relative
+        from ...client.syncing import handle_ignore_batch
+
+        return handle_ignore_batch(self, self.global_batches)
+
+    def unignore(self) -> SyftSuccess | SyftError:
+        # relative
+        from ...client.syncing import handle_unignore_batch
+
+        return handle_unignore_batch(self, self.global_batches)
+
     @property
     def root_id(self) -> UID:
         return self.root_diff.object_id
 
     @property
     def root_type(self) -> type:
         return self.root_diff.obj_type
 
     @property
     def is_ignored(self) -> bool:
-        return self.decision == SyncDecision.ignore
+        return self.decision == SyncDecision.IGNORE
 
     @property
     def is_skipped(self) -> bool:
-        return self.decision == SyncDecision.skip
+        return self.decision == SyncDecision.SKIP
+
+    def create_new_resolved_states(
+        self,
+    ) -> tuple["ResolvedSyncState", "ResolvedSyncState"]:
+        """
+        Returns new ResolvedSyncState objects for the source and target nodes
+        """
+        resolved_state_low = ResolvedSyncState(node_uid=self.low_node_uid, alias="low")
+        resolved_state_high = ResolvedSyncState(
+            node_uid=self.high_node_uid, alias="high"
+        )
+
+        # Return source, target
+        if self.sync_direction == SyncDirection.LOW_TO_HIGH:
+            return resolved_state_low, resolved_state_high
+        else:
+            return resolved_state_high, resolved_state_low
 
     @classmethod
     def from_dependencies(
         cls,
         root_uid: UID,
         obj_dependencies: dict[UID, list[UID]],
         obj_uid_to_diff: dict[UID, ObjectDiff],
@@ -784,15 +815,15 @@
         elif status == "SAME":
             badge_color = "label-gray"
         else:
             badge_color = "label-orange"
         return {"value": status.upper(), "type": badge_color}
 
     def _coll_repr_(self) -> dict[str, Any]:
-        no_obj_html = "<p class='diff-state-no-obj'>No object detected</p>"
+        no_obj_html = "<p class='diff-state-no-obj'>No object</p>"
         if self.root_diff.low_obj is None:
             low_html = no_obj_html
         else:
             low_html = SyncTableObject(object=self.root_diff.low_obj).to_html()
 
         if self.root_diff.high_obj is None:
             high_html = no_obj_html
@@ -965,15 +996,15 @@
         self.batch.decision = None
         required_dependencies = {
             d.object_id for d in self.batch.get_dependencies(include_roots=True)
         }
 
         for other_batch in self.other_batches:
             if (
-                other_batch.decision == SyncDecision.ignore
+                other_batch.decision == SyncDecision.IGNORE
                 and other_batch.root_id in required_dependencies
             ):
                 print(f"ignoring other batch ({other_batch.root_type.__name__})")
                 other_batch.decision = None
 
 
 class NodeDiff(SyftObject):
@@ -983,38 +1014,47 @@
     low_node_uid: UID
     high_node_uid: UID
     user_verify_key_low: SyftVerifyKey
     user_verify_key_high: SyftVerifyKey
     obj_uid_to_diff: dict[UID, ObjectDiff] = {}
     obj_dependencies: dict[UID, list[UID]] = {}
     batches: list[ObjectDiffBatch] = []
+    all_batches: list[ObjectDiffBatch] = []
     low_state: SyncState
     high_state: SyncState
     direction: SyncDirection | None
 
+    include_ignored: bool = False
+
     def __getitem__(self, idx: Any) -> ObjectDiffBatch:
         return self.batches[idx]
 
     @property
+    def ignored_batches(self) -> list[ObjectDiffBatch]:
+        return [
+            batch for batch in self.all_batches if batch.decision == SyncDecision.IGNORE
+        ]
+
+    @property
     def ignored_changes(self) -> list[IgnoredBatchView]:
-        ignored_batches = [b for b in self.batches if b.decision == SyncDecision.ignore]
         result = []
-        for ignored_batch in ignored_batches:
-            other_batches = [b for b in self.batches if b is not ignored_batch]
+        for ignored_batch in self.ignored_batches:
+            other_batches = [b for b in self.all_batches if b is not ignored_batch]
             result.append(
                 IgnoredBatchView(batch=ignored_batch, other_batches=other_batches)
             )
         return result
 
     @classmethod
     def from_sync_state(
         cls: type["NodeDiff"],
         low_state: SyncState,
         high_state: SyncState,
         direction: SyncDirection,
+        include_ignored: bool = False,
         _include_node_status: bool = False,
     ) -> "NodeDiff":
         obj_uid_to_diff = {}
         for obj_id in set(low_state.objects.keys()) | set(high_state.objects.keys()):
             low_obj = low_state.objects.get(obj_id, None)
             high_obj = high_state.objects.get(obj_id, None)
 
@@ -1047,52 +1087,60 @@
                 high_node_uid=high_state.node_uid,
                 last_sync_date_low=last_sync_date_low,
                 last_sync_date_high=last_sync_date_high,
             )
             obj_uid_to_diff[diff.object_id] = diff
 
         obj_dependencies = NodeDiff.dependencies_from_states(low_state, high_state)
-        batches = NodeDiff.hierarchies(
+        all_batches = NodeDiff.hierarchies(
             low_state,
             high_state,
             obj_dependencies,
             obj_uid_to_diff,
             direction=direction,
         )
 
         # TODO: Check if high and low ignored batches are the same else error
         previously_ignored_batches = low_state.ignored_batches
-        NodeDiff.apply_previous_ignore_state(batches, previously_ignored_batches)
+        NodeDiff.apply_previous_ignore_state(all_batches, previously_ignored_batches)
+
+        if not include_ignored:
+            batches = [b for b in all_batches if not b.is_ignored]
+        else:
+            batches = all_batches
 
         return cls(
             low_node_uid=low_state.node_uid,
             high_node_uid=high_state.node_uid,
             user_verify_key_low=low_state.syft_client_verify_key,
             user_verify_key_high=high_state.syft_client_verify_key,
             obj_uid_to_diff=obj_uid_to_diff,
             obj_dependencies=obj_dependencies,
             batches=batches,
+            all_batches=all_batches,
             low_state=low_state,
             high_state=high_state,
             direction=direction,
         )
 
     @staticmethod
     def apply_previous_ignore_state(
         batches: list[ObjectDiffBatch], previously_ignored_batches: dict[UID, int]
     ) -> None:
-        """Loop through all ignored batches in syncstate. If batch did not change, set to ignored
+        """
+        Loop through all ignored batches in syncstate. If batch did not change, set to ignored
         If another batch needs to exist in order to accept that changed batch: also unignore
-        e.g. if a job changed, also unignore the usercode"""
+        e.g. if a job changed, also unignore the usercode
+        """
 
         for root_id, batch_hash in previously_ignored_batches.items():
             for batch in batches:
                 if batch.root_id == root_id:
                     if hash(batch) == batch_hash:
-                        batch.decision = SyncDecision.ignore
+                        batch.decision = SyncDecision.IGNORE
                     else:
                         print(
                             f"""A batch with type {batch.root_type.__name__} was previously ignored but has changed
 It will be available for review again."""
                         )
                         # batch has changed, so unignore
                         batch.decision = None
@@ -1204,15 +1252,15 @@
     def hierarchies(
         low_sync_state: SyncState,
         high_sync_state: SyncState,
         obj_dependencies: dict[UID, list[UID]],
         obj_uid_to_diff: dict[UID, ObjectDiff],
         direction: SyncDirection,
     ) -> list[ObjectDiffBatch]:
-        batches = []
+        batches: list[ObjectDiffBatch] = []
         root_ids = []
 
         for diff in obj_uid_to_diff.values():
             diff_obj = diff.low_obj if diff.low_obj is not None else diff.high_obj
             if isinstance(diff_obj, Request | UserCode | TwinAPIEndpoint):
                 # TODO: Figure out nested user codes, do we even need that?
 
@@ -1230,14 +1278,19 @@
                 high_sync_state.node_uid,
                 low_sync_state.syft_client_verify_key,
                 high_sync_state.syft_client_verify_key,
                 sync_direction=direction,
             )
             batches.append(batch)
 
+        # TODO ref back to NodeDiff would clean up a lot of logic,
+        # No need to save NodeDiff state on every batch
+        for batch in batches:
+            batch.global_batches = batches
+
         hierarchies_sorted = NodeDiff._sort_batches(batches)
         return hierarchies_sorted
 
     @property
     def is_same(self) -> bool:
         return all(object_diff.status == "SAME" for object_diff in self.diffs)
 
@@ -1251,42 +1304,49 @@
     new_permissions_lowside: list[ActionObjectPermission]
     new_storage_permissions_lowside: list[StoragePermission]
     new_storage_permissions_highside: list[StoragePermission]
     unignore: bool = False
     mockify: bool
 
     @classmethod
-    def from_widget_state(
+    def from_batch_decision(
         cls,
+        diff: ObjectDiff,
         sync_direction: SyncDirection,
-        widget: Any,
+        share_private_data: bool,
+        mockify: bool,
         decision: SyncDecision,
         share_to_user: SyftVerifyKey | None,
     ) -> Self:
         # read widget state
-        diff = widget.diff
         new_permissions_low_side = []
 
         # read permissions
         if sync_direction == SyncDirection.HIGH_TO_LOW:
-            if widget.share_private_data or diff.object_type == "Job":
+            # To create read permissions for the object
+            # job/usercode/request/TwinAPIEndpoint
+            if share_private_data:  # or diff.object_type == "Job":
                 if share_to_user is None:
-                    raise ValueError("share_to_user is required for private data")
+                    # job ran by another user
+                    if not diff.object_type == "Job":
+                        raise ValueError(
+                            "share_to_user is required to share private data"
+                        )
                 else:
                     new_permissions_low_side = [
                         ActionObjectPermission(
-                            uid=widget.diff.object_id,
+                            uid=diff.object_id,
                             permission=ActionPermission.READ,
-                            credentials=share_to_user,  # type: ignore
+                            credentials=share_to_user,
                         )
                     ]
 
-        mockify = widget.mockify
-        if widget.has_unused_share_button:
-            print("Share button was not used, so we will mockify the object")
+        # TODO move this to the widget
+        # if widget.has_unused_share_button:
+        #     print("Share button was not used, so we will mockify the object")
 
         # storage permissions
         new_storage_permissions = []
 
         if sync_direction == SyncDirection.HIGH_TO_LOW:
             # TODO: apply storage permissions on both ends
             if not mockify:
@@ -1315,17 +1375,15 @@
     node_uid: UID
     create_objs: list[SyncableSyftObject] = []
     update_objs: list[SyncableSyftObject] = []
     delete_objs: list[SyftObject] = []
     new_permissions: list[ActionObjectPermission] = []
     new_storage_permissions: list[StoragePermission] = []
     ignored_batches: dict[UID, int] = {}  # batch root uid -> hash of the batch
-    unignored_batches: set[UID] = (
-        set()
-    )  # NOTE: using '{}' as default value does not work here
+    unignored_batches: set[UID] = set()
     alias: str
 
     @classmethod
     def from_client(cls, client: SyftClient) -> "ResolvedSyncState":
         alias: str = client.metadata.node_side_type  # type: ignore
         if alias not in ["low", "high"]:
             raise ValueError(
@@ -1337,16 +1395,16 @@
         self.ignored_batches[batch.root_id] = hash(batch)
 
     def add_unignored(self, root_id: UID) -> None:
         self.unignored_batches.add(root_id)
 
     def add_sync_instruction(self, sync_instruction: SyncInstruction) -> None:
         if (
-            sync_instruction.decision == SyncDecision.ignore
-            or sync_instruction.decision == SyncDecision.skip
+            sync_instruction.decision == SyncDecision.IGNORE
+            or sync_instruction.decision == SyncDecision.SKIP
         ):
             return
         diff = sync_instruction.diff
 
         if sync_instruction.unignore:
             self.unignored_batches.add(sync_instruction.batch_diff.root_id)
```

### Comparing `syft-0.8.7b2/src/syft/service/sync/resolve_widget.py` & `syft-0.8.7b3/src/syft/service/sync/resolve_widget.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from ipywidgets import VBox
 
 # relative
 from ...client.sync_decision import SyncDecision
 from ...client.sync_decision import SyncDirection
 from ...node.credentials import SyftVerifyKey
 from ...types.uid import UID
+from ...util.notebook_ui.components.sync import Alert
 from ...util.notebook_ui.components.sync import Badge
 from ...util.notebook_ui.components.sync import CopyIDButton
 from ...util.notebook_ui.components.sync import MainDescription
 from ...util.notebook_ui.components.sync import SyncWidgetHeader
 from ...util.notebook_ui.notebook_addons import CSS_CODE
 from ..action.action_object import ActionObject
 from ..api.api import TwinAPIEndpoint
@@ -96,25 +97,28 @@
 
 class MainObjectDiffWidget:
     def __init__(
         self,
         diff: ObjectDiff,
         direction: SyncDirection,
         with_box: bool = True,
+        show_share_warning: bool = False,
     ):
         self.low_properties = diff.repr_attr_dict("low")
         self.high_properties = diff.repr_attr_dict("high")
         self.statuses = diff.repr_attr_diffstatus_dict()
         self.direction = direction
         self.diff: ObjectDiff = diff
         self.with_box = with_box
-        self.widget = self.build()
+        self.show_share_warning = show_share_warning
         self.sync = True
         self.is_main_widget: bool = True
 
+        self.widget = self.build()
+
     def set_share_private_data(self) -> None:
         # No-op for main widget
         pass
 
     @property
     def mockify(self) -> bool:
         return not self.share_private_data
@@ -125,14 +129,29 @@
         return False
 
     @property
     def share_private_data(self) -> bool:
         # there are TwinAPIEndpoint.__private_sync_attr_mocks__
         return not isinstance(self.diff.non_empty_object, TwinAPIEndpoint)
 
+    @property
+    def warning_html(self) -> str:
+        if isinstance(self.diff.non_empty_object, TwinAPIEndpoint):
+            message = "Only the private function of a TwinAPI will be synced to the public node."
+            return Alert(message=message).to_html()
+        elif self.show_share_warning:
+            message = (
+                "By default only the object wrapper will be synced. "
+                "If you would like to sync the real data please "
+                'activate the "Sync Real Data" button above.'
+            )
+            return Alert(message=message).to_html()
+        else:
+            return ""
+
     def build(self) -> widgets.HBox:
         all_keys = list(self.low_properties.keys()) + list(self.high_properties.keys())
         low_properties = {}
         high_properties = {}
         for k in all_keys:
             low_properties[k] = self.low_properties.get(k, None)
             high_properties[k] = self.high_properties.get(k, None)
@@ -164,21 +183,25 @@
         css_accordion = """
             <style>
             .diff-container {
                 border: 0.5px solid #B4B0BF;
             }
             </style>
         """
-        dom_classes = []
+
+        result = widgets.HBox([HTML(css_accordion), widget_from, widget_to])
+
+        warning = self.warning_html
+        if warning:
+            result = VBox([widgets.HTML(warning), result])
+
         if self.with_box:
-            dom_classes.append("diff-container")
+            result._dom_classes = result._dom_classes + ("diff-container",)
 
-        return widgets.HBox(
-            [HTML(css_accordion), widget_from, widget_to], _dom_classes=dom_classes
-        )
+        return result
 
 
 class CollapsableObjectDiffWidget:
     def __init__(
         self,
         diff: ObjectDiff,
         direction: SyncDirection,
@@ -201,14 +224,25 @@
             return False
 
     @property
     def has_unused_share_button(self) -> bool:
         return self.show_share_button and not self.share_private_data
 
     @property
+    def warning_html(self) -> str:
+        if self.show_share_button:
+            message = (
+                "By default only the object wrapper will be synced. "
+                "If you would like to sync the real log data please "
+                "activate the “Real Data” button above."
+            )
+            return Alert(message=message).to_html()
+        return ""
+
+    @property
     def show_share_button(self) -> bool:
         return isinstance(self.diff.non_empty_object, SyftLog | ActionObject)
 
     @property
     def title(self) -> str:
         object = self.diff.non_empty_object
         if object is None:
@@ -236,15 +270,20 @@
             self._sync_checkbox.disabled = False
 
     def set_share_private_data(self) -> None:
         if self.show_share_button:
             self._share_private_checkbox.value = True
 
     def build(self) -> widgets.VBox:
-        content = MainObjectDiffWidget(self.diff, self.direction, with_box=False).widget
+        content = MainObjectDiffWidget(
+            self.diff,
+            self.direction,
+            with_box=False,
+            show_share_warning=self.show_share_button,
+        ).widget
 
         accordion, share_private_checkbox, sync_checkbox = self.build_accordion(
             accordion_body=content,
             show_sync_checkbox=True,
             show_share_private_checkbox=self.show_share_button,
         )
 
@@ -261,14 +300,15 @@
     def create_accordion_css(
         self, header_id: str, body_id: str, class_name: str
     ) -> str:
         css_accordion = f"""
             <style>
             .accordion {{
                 padding: 0 10px;
+                margin: 3px 0px;
             }}
 
             .body-hidden {{
                 display: none;
             }}
 
             .body-visible {{
@@ -383,147 +423,88 @@
         self.is_synced = False
         self.hide_result_widget()
 
     def build_css_widget(self) -> HTML:
         return widgets.HTML(value=CSS_CODE)
 
     def _repr_mimebundle_(self, **kwargs: dict) -> dict[str, str] | None:
-        # from IPython.display import display
         return self.widget._repr_mimebundle_(**kwargs)
 
-    def click_sync(self) -> SyftSuccess | SyftError:
-        return self.button_callback()
-
     def click_share_all_private_data(self) -> None:
         for widget in self.id2widget.values():
             widget.set_share_private_data()
 
     def click_share_private_data(self, uid: UID | str) -> SyftError | SyftSuccess:
         if isinstance(uid, str):
             uid = UID(uid)
         if uid not in self.id2widget:
             return SyftError(message="Object not found in this widget")
 
         widget = self.id2widget[uid]
         widget.set_share_private_data()
         return SyftSuccess(message="Private data shared")
 
-    def button_callback(self, *args: list, **kwargs: dict) -> SyftSuccess | SyftError:
+    def get_share_private_data_state(self) -> dict[UID, bool]:
+        return {
+            uid: widget.share_private_data for uid, widget in self.id2widget.items()
+        }
+
+    def get_mockify_state(self) -> dict[UID, bool]:
+        return {uid: widget.mockify for uid, widget in self.id2widget.items()}
+
+    def click_ignore(self, *args: list, **kwargs: dict) -> SyftSuccess | SyftError:
+        # relative
+        from ...client.syncing import handle_ignore_batch
+
         if self.is_synced:
             return SyftError(
                 message="The changes in this widget have already been synced."
             )
 
-        if self.obj_diff_batch.sync_direction == SyncDirection.LOW_TO_HIGH:
-            # TODO: make dynamic
-            decision = "low"
-        else:
-            decision = "high"
-
-        # previously_ignored_batches = state.low_state.ignored_batches
-        previously_ignored_batches: dict = {}
-        # TODO: only add permissions for objects where we manually give permission
-        # Maybe default read permission for some objects (high -> low)
-
-        # TODO: UID
-        resolved_state_low = ResolvedSyncState(
-            node_uid=self.obj_diff_batch.low_node_uid, alias="low"
-        )
-        resolved_state_high = ResolvedSyncState(
-            node_uid=self.obj_diff_batch.high_node_uid, alias="high"
-        )
-
-        batch_diff = self.obj_diff_batch
-        if batch_diff.is_unchanged:
-            # Hierarchy has no diffs
-            return SyftSuccess(message="No changes to sync")
-
-        if batch_diff.decision is not None:
-            # handles ignores
-            batch_decision = batch_diff.decision
-        elif decision is not None:
-            batch_decision = SyncDecision(decision)
-        else:
-            pass
-            # batch_decision = get_user_input_for_resolve()
+        res = handle_ignore_batch(
+            obj_diff_batch=self.obj_diff_batch,
+            all_batches=self.obj_diff_batch.global_batches,
+        )
 
-        batch_diff.decision = batch_decision
+        self.set_widget_result_state(res)
+        return res
 
-        # TODO: FIX
-        other_batches: list = []
-        # other_batches = [b for b in state.batches if b is not batch_diff]
+    def click_unignore(self, *args: list, **kwargs: dict) -> SyftSuccess | SyftError:
         # relative
-        from ...client.syncing import handle_ignore_skip
+        from ...client.syncing import handle_unignore_batch
 
-        handle_ignore_skip(batch_diff, batch_decision, other_batches)
+        if self.is_synced:
+            return SyftError(
+                message="The changes in this widget have already been synced."
+            )
 
-        if batch_decision not in [SyncDecision.skip, SyncDecision.ignore]:
-            sync_instructions = []
-            for diff in batch_diff.get_dependents(include_roots=True):
-                # while making widget: bind buttons to right state
-                # share_state = {diff.object_id: False for diff in obj_diff_batch.get_dependents(include_roots=False)}
-
-                # diff id -> shared (bool)
-
-                # onclick checkbox: set widget state
-                widget = self.id2widget[diff.object_id]
-                sync = widget.sync
-
-                if sync or widget.is_main_widget:
-                    share_to_user: SyftVerifyKey | None = getattr(
-                        self.obj_diff_batch.user_code_high, "user_verify_key", None
-                    )
-                    instruction = SyncInstruction.from_widget_state(
-                        widget=widget,
-                        sync_direction=self.obj_diff_batch.sync_direction,
-                        decision=decision,
-                        share_to_user=share_to_user,
-                    )
-                    sync_instructions.append(instruction)
-        else:
-            sync_instructions = []
-            if batch_decision == SyncDecision.ignore:
-                resolved_state_high.add_ignored(batch_diff)
-                resolved_state_low.add_ignored(batch_diff)
-
-        if (
-            batch_diff.root_id in previously_ignored_batches
-            and batch_diff.decision != SyncDecision.ignore
-        ):
-            resolved_state_high.add_unignored(batch_diff.root_id)
-            resolved_state_low.add_unignored(batch_diff.root_id)
-
-        print(f"Decision: Syncing {len(sync_instructions)} objects")
-
-        for sync_instruction in sync_instructions:
-            resolved_state_low.add_sync_instruction(sync_instruction)
-            resolved_state_high.add_sync_instruction(sync_instruction)
-
-        if self.obj_diff_batch.sync_direction is None:
-            raise ValueError("no direction specified")
-        sync_direction = self.obj_diff_batch.sync_direction
-        resolved_state = (
-            resolved_state_high
-            if sync_direction == SyncDirection.LOW_TO_HIGH
-            else resolved_state_low
-        )
-        res = self.obj_diff_batch.target_client.apply_state(resolved_state)
-
-        if sync_direction == SyncDirection.HIGH_TO_LOW:
-            # apply empty state to generete a new state
-            resolved_state_high = ResolvedSyncState(
-                node_uid=self.obj_diff_batch.high_node_uid, alias="high"
+        res = handle_unignore_batch(
+            obj_diff_batch=self.obj_diff_batch,
+            all_batches=self.obj_diff_batch.global_batches,
+        )
+
+        self.set_widget_result_state(res)
+        return res
+
+    def click_sync(self, *args: list, **kwargs: dict) -> SyftSuccess | SyftError:
+        # relative
+        from ...client.syncing import handle_sync_batch
+
+        if self.is_synced:
+            return SyftError(
+                message="The changes in this widget have already been synced."
             )
-            high_client = self.obj_diff_batch.source_client
-            res = high_client.apply_state(resolved_state_high)
 
-        self.is_synced = True
-        self.set_result_state(res)
-        self.hide_main_widget()
-        self.show_result_widget()
+        res = handle_sync_batch(
+            obj_diff_batch=self.obj_diff_batch,
+            share_private_data=self.get_share_private_data_state(),
+            mockify=self.get_mockify_state(),
+        )
+
+        self.set_widget_result_state(res)
         return res
 
     @property
     def batch_diff_widgets(self) -> list[CollapsableObjectDiffWidget]:
         dependents = self.obj_diff_batch.get_dependents(
             include_roots=False, include_batch_root=False
         )
@@ -556,15 +537,21 @@
     def main_object_diff_widget(self) -> MainObjectDiffWidget:
         obj_diff_widget = MainObjectDiffWidget(
             self.obj_diff_batch.root_diff,
             direction=self.obj_diff_batch.sync_direction,
         )
         return obj_diff_widget
 
-    def set_result_state(self, result: SyftSuccess | SyftError) -> None:
+    def set_widget_result_state(self, res: SyftSuccess | SyftError) -> None:
+        self.is_synced = True
+        self.set_result_message(res)
+        self.hide_main_widget()
+        self.show_result_widget()
+
+    def set_result_message(self, result: SyftSuccess | SyftError) -> None:
         result_html = result._repr_html_()
         # Wrap in div to match Jupyter Lab output styling
         result_html = NOTEBOOK_OUTPUT_DIV.format(content=result_html)
         self.result_widget.children = [widgets.HTML(value=result_html)]
 
     def hide_main_widget(self) -> None:
         self.main_widget.layout.display = "none"
@@ -589,31 +576,32 @@
 
         for widget in batch_diff_widgets:
             self.id2widget[widget.diff.object_id] = widget
 
         for widget in dependent_batch_diff_widgets:
             self.id2widget[widget.diff.object_id] = widget
 
+        # put a 4px spacer between each item
         main_batch_items = widgets.VBox(
             children=[d.widget for d in batch_diff_widgets],
         )
 
         dependency_items = widgets.VBox(
             children=[d.widget for d in dependent_batch_diff_widgets],
         )
 
         full_widget = widgets.VBox(
             [
                 self.build_header(),
                 self.main_object_diff_widget.widget,
-                self.spacer(16),
+                self.spacer(8),
                 main_batch_items,
                 self.separator(),
                 dependency_items,
-                self.spacer(16),
+                self.spacer(8),
                 self.sync_button(),
             ]
         )
         return full_widget
 
     def sync_button(self) -> Button:
         sync_button = Button(
@@ -621,22 +609,22 @@
             style={
                 "text_color": "#464A91",
                 "button_color": "transparent",
                 "float": "right",
             },
             layout=Layout(border="#464A91 solid 1.5px", width="200px"),
         )
-        sync_button.on_click(self.button_callback)
+        sync_button.on_click(self.click_sync)
         return sync_button
 
     def spacer(self, height: int) -> widgets.HTML:
         return widgets.HTML(f"<div style='height: {height}px'></div>")
 
     def separator(self) -> widgets.HTML:
         return widgets.HTML(
-            value='<div style="text-align: center; margin: 10px 0; border: 1px dashed #B4B0BF;"></div>',
+            value='<div style="text-align: center; margin: 3px 0; border: 1px dashed #B4B0BF;"></div>',
             layout=Layout(width="100%"),
         )
 
     def build_header(self) -> HTML:
         header_html = SyncWidgetHeader(diff_batch=self.obj_diff_batch).to_html()
         return HTML(value=header_html)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `syft-0.8.7b2/src/syft/service/sync/sync_service.py` & `syft-0.8.7b3/src/syft/service/sync/sync_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,15 +228,20 @@
             return SyftError(message=res.message)
         else:
             new_state = res.ok()
             res = self.stash.set(context.credentials, new_state)
             if res.is_err():
                 return SyftError(message=res.message)
             else:
-                return SyftSuccess(message=f"Synced {len(items)} items")
+                message = f"Synced {len(items)} items"
+                if len(ignored_batches) > 0:
+                    message += f", ignored {len(ignored_batches)} batches"
+                if len(unignored_batches) > 0:
+                    message += f", unignored {len(unignored_batches)} batches"
+                return SyftSuccess(message=message)
 
     @service_method(
         path="sync.get_permissions",
         name="get_permissions",
         roles=ADMIN_ROLE_LEVEL,
     )
     def get_permissions(
@@ -283,15 +288,15 @@
         action_object_ids = set()
         for obj in all_items:
             if isinstance(obj, ExecutionOutput):
                 action_object_ids |= set(obj.output_id_list)
             elif isinstance(obj, Job) and obj.result is not None:
                 if isinstance(obj.result, ActionObject):
                     obj.result = obj.result.as_empty()
-                action_object_ids.add(obj.result.id)
+                    action_object_ids.add(obj.result.id)
 
         for uid in action_object_ids:
             action_object = context.node.get_service("actionservice").get(
                 context, uid, resolve_nested=False
             )  # type: ignore
             if action_object.is_err():
                 return action_object
```

### Comparing `syft-0.8.7b2/src/syft/service/sync/sync_stash.py` & `syft-0.8.7b3/src/syft/service/sync/sync_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/sync/sync_state.py` & `syft-0.8.7b3/src/syft/service/sync/sync_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     __syft_include_id_coll_repr__ = False
 
     # TODO table formatting
     __repr_attrs__ = [
         "previous_state",
         "current_state",
     ]
+    __table_coll_widths__ = ["min-content", "auto", "auto", "auto"]
 
     def status_badge(self) -> dict[str, str]:
         status = self.status
         if status == "NEW":
             badge_color = "label-green"
         elif status == "SAME":
             badge_color = "label-gray"
```

### Comparing `syft-0.8.7b2/src/syft/service/user/user.py` & `syft-0.8.7b3/src/syft/service/user/user.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/user/user_roles.py` & `syft-0.8.7b3/src/syft/service/user/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/user/user_service.py` & `syft-0.8.7b3/src/syft/service/user/user_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from .user import UserSearch
 from .user import UserUpdate
 from .user import UserView
 from .user import UserViewPage
 from .user import check_pwd
 from .user import salt_and_hash_password
 from .user_roles import DATA_OWNER_ROLE_LEVEL
+from .user_roles import DATA_SCIENTIST_ROLE_LEVEL
 from .user_roles import GUEST_ROLE_LEVEL
 from .user_roles import ServiceRole
 from .user_roles import ServiceRoleCapability
 from .user_stash import UserStash
 
 
 @instrument
@@ -79,15 +80,15 @@
             ],
         )
         if result.is_err():
             return SyftError(message=str(result.err()))
         user = result.ok()
         return user.to(UserView)
 
-    @service_method(path="user.view", name="view")
+    @service_method(path="user.view", name="view", roles=DATA_SCIENTIST_ROLE_LEVEL)
     def view(
         self, context: AuthedServiceContext, uid: UID
     ) -> UserView | None | SyftError:
         """Get user for given uid"""
         result = self.stash.get_by_uid(credentials=context.credentials, uid=uid)
         if result.is_ok():
             user = result.ok()
@@ -193,14 +194,28 @@
     #     result = self.stash.admin_user()
     #     if result.is_ok():
     #         user = result.ok()
     #         if user:
     #             return user
     #     return SyftError(message=str(result.err()))
 
+    def get_user_id_for_credentials(
+        self, credentials: SyftVerifyKey
+    ) -> UID | SyftError:
+        result = self.stash.get_by_verify_key(
+            credentials=credentials, verify_key=credentials
+        )
+        if result.is_ok():
+            user = result.ok()
+            if user:
+                return user.id
+            else:
+                SyftError(message="User not found!")
+        return SyftError(message=str(result.err()))
+
     @service_method(
         path="user.get_current_user", name="get_current_user", roles=GUEST_ROLE_LEVEL
     )
     def get_current_user(self, context: AuthedServiceContext) -> UserView | SyftError:
         result = self.stash.get_by_verify_key(
             credentials=context.credentials, verify_key=context.credentials
         )
```

### Comparing `syft-0.8.7b2/src/syft/service/user/user_stash.py` & `syft-0.8.7b3/src/syft/service/user/user_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/warnings.py` & `syft-0.8.7b3/src/syft/service/warnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/worker/image_identifier.py` & `syft-0.8.7b3/src/syft/service/worker/image_identifier.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/worker/image_registry_service.py` & `syft-0.8.7b3/src/syft/service/worker/image_registry_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/worker/image_registry_stash.py` & `syft-0.8.7b3/src/syft/service/worker/image_registry_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/worker/utils.py` & `syft-0.8.7b3/src/syft/service/worker/utils.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/worker/worker.py` & `syft-0.8.7b3/src/syft/service/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/worker/worker_image.py` & `syft-0.8.7b3/src/syft/service/worker/worker_image.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/worker/worker_image_service.py` & `syft-0.8.7b3/src/syft/service/worker/worker_image_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/worker/worker_image_stash.py` & `syft-0.8.7b3/src/syft/service/worker/worker_image_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/worker/worker_pool.py` & `syft-0.8.7b3/src/syft/service/worker/worker_pool.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/worker/worker_pool_service.py` & `syft-0.8.7b3/src/syft/service/worker/worker_pool_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/worker/worker_pool_stash.py` & `syft-0.8.7b3/src/syft/service/worker/worker_pool_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/worker/worker_service.py` & `syft-0.8.7b3/src/syft/service/worker/worker_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/service/worker/worker_stash.py` & `syft-0.8.7b3/src/syft/service/worker/worker_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/store/blob_storage/__init__.py` & `syft-0.8.7b3/src/syft/store/blob_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/store/blob_storage/on_disk.py` & `syft-0.8.7b3/src/syft/store/blob_storage/on_disk.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/store/blob_storage/seaweedfs.py` & `syft-0.8.7b3/src/syft/store/blob_storage/seaweedfs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/store/dict_document_store.py` & `syft-0.8.7b3/src/syft/store/dict_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/store/document_store.py` & `syft-0.8.7b3/src/syft/store/document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/store/kv_document_store.py` & `syft-0.8.7b3/src/syft/store/kv_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/store/linked_obj.py` & `syft-0.8.7b3/src/syft/store/linked_obj.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/store/locks.py` & `syft-0.8.7b3/src/syft/store/locks.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/store/mongo_client.py` & `syft-0.8.7b3/src/syft/store/mongo_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/store/mongo_codecs.py` & `syft-0.8.7b3/src/syft/store/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/store/mongo_document_store.py` & `syft-0.8.7b3/src/syft/store/mongo_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/store/sqlite_document_store.py` & `syft-0.8.7b3/src/syft/store/sqlite_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/types/blob_storage.py` & `syft-0.8.7b3/src/syft/types/blob_storage.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/types/datetime.py` & `syft-0.8.7b3/src/syft/types/datetime.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/types/dicttuple.py` & `syft-0.8.7b3/src/syft/types/dicttuple.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/types/grid_url.py` & `syft-0.8.7b3/src/syft/types/grid_url.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/types/identity.py` & `syft-0.8.7b3/src/syft/types/identity.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/types/syft_metaclass.py` & `syft-0.8.7b3/src/syft/types/syft_metaclass.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/types/syft_migration.py` & `syft-0.8.7b3/src/syft/types/syft_migration.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/types/syft_object.py` & `syft-0.8.7b3/src/syft/types/syft_object.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,20 +62,22 @@
 MappingIntStrAny = Mapping[IntStr, Any]
 
 
 SYFT_OBJECT_VERSION_1 = 1
 SYFT_OBJECT_VERSION_2 = 2
 SYFT_OBJECT_VERSION_3 = 3
 SYFT_OBJECT_VERSION_4 = 4
+SYFT_OBJECT_VERSION_5 = 5
 
 supported_object_versions = [
     SYFT_OBJECT_VERSION_1,
     SYFT_OBJECT_VERSION_2,
     SYFT_OBJECT_VERSION_3,
     SYFT_OBJECT_VERSION_4,
+    SYFT_OBJECT_VERSION_5,
 ]
 
 HIGHEST_SYFT_OBJECT_VERSION = max(supported_object_versions)
 LOWEST_SYFT_OBJECT_VERSION = min(supported_object_versions)
 
 
 # These attributes are dynamically added based on node/client
@@ -415,14 +417,15 @@
     __owner__: str
 
     __repr_attrs__: ClassVar[list[str]] = []  # show these in html repr collections
     __attr_custom_repr__: ClassVar[list[str] | None] = (
         None  # show these in html repr of an object
     )
     __validate_private_attrs__: ClassVar[bool] = True
+    __table_coll_widths__: ClassVar[list[str] | None] = None
 
     def __syft_get_funcs__(self) -> list[tuple[str, Signature]]:
         funcs = print_type_cache[type(self)]
         if len(funcs) > 0:
             return funcs
 
         for attr in dir(type(self)):
@@ -851,14 +854,25 @@
 
     if "created_at" in df.columns:
         df.sort_values(by="created_at", ascending=False, inplace=True)
 
     return df.to_dict("records")  # type: ignore
 
 
+def _get_grid_template_columns(first_value: Any) -> tuple[str | None, str | None]:
+    grid_template_cols = getattr(first_value, "__table_coll_widths__", None)
+    if isinstance(grid_template_cols, list):
+        grid_template_columns = " ".join(grid_template_cols)
+        grid_template_cell_columns = "unset"
+    else:
+        grid_template_columns = None
+        grid_template_cell_columns = None
+    return grid_template_columns, grid_template_cell_columns
+
+
 def list_dict_repr_html(self: Mapping | Set | Iterable) -> str:
     try:
         max_check = 1
         items_checked = 0
         has_syft = False
         extra_fields: list = []
         if isinstance(self, Mapping):
@@ -892,30 +906,39 @@
             # if custom_repr:
             table_icon = None
             if hasattr(values[0], "icon"):
                 table_icon = values[0].icon
             # this is a list of dicts
             is_homogenous = len({type(x) for x in values}) == 1
             # third party
-            first_value = values[0]
-            if is_homogenous:
-                cls_name = first_value.__class__.__name__
-            else:
-                cls_name = ""
+
             try:
                 vals = get_repr_values_table(
                     self, is_homogenous, extra_fields=extra_fields
                 )
             except Exception:
                 return str(self)
 
+            first_value = values[0]
+            if is_homogenous:
+                cls_name = first_value.__class__.__name__
+                grid_template_columns, grid_template_cell_columns = (
+                    _get_grid_template_columns(first_value)
+                )
+            else:
+                cls_name = ""
+                grid_template_columns = None
+                grid_template_cell_columns = None
+
             return create_table_template(
                 vals,
                 f"{cls_name} {self.__class__.__name__.capitalize()}",
                 table_icon=table_icon,
+                grid_template_columns=grid_template_columns,
+                grid_template_cell_columns=grid_template_cell_columns,
             )
 
     except Exception as e:
         print(
             f"error representing {type(self)} of objects. {e}, {traceback.format_exc()}"
         )
         pass
```

### Comparing `syft-0.8.7b2/src/syft/types/syncable_object.py` & `syft-0.8.7b3/src/syft/types/syncable_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/types/transforms.py` & `syft-0.8.7b3/src/syft/types/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/types/twin_object.py` & `syft-0.8.7b3/src/syft/types/twin_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/types/uid.py` & `syft-0.8.7b3/src/syft/types/uid.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,32 @@
+# future
+from __future__ import annotations
+
 # stdlib
 from collections.abc import Callable
 from collections.abc import Sequence
 import hashlib
 from typing import Any
-from typing import Union
 import uuid
 from uuid import UUID as uuid_type
 
 # relative
 from ..serde.serializable import serializable
 from ..util.logger import critical
 from ..util.logger import traceback_and_raise
 
+try:
+    # Python >= 3.11
+    # stdlib
+    from typing import Self
+except ImportError:
+    # Python < 3.11
+    # third party
+    from typing_extensions import Self
+
 
 @serializable(attrs=["value"])
 class UID:
     """A unique ID for every Syft object.
 
     This object creates a unique ID for every object in the Syft
     ecosystem. This ID is guaranteed to be unique for the node on
@@ -34,15 +45,15 @@
     __serde_overrides__: dict[str, Sequence[Callable]] = {
         "value": (lambda x: x.bytes, lambda x: uuid.UUID(bytes=bytes(x)))
     }
 
     __slots__ = "value"
     value: uuid_type
 
-    def __init__(self, value: Union[uuid_type, str, bytes, "UID"] | None = None):
+    def __init__(self, value: Self | uuid_type | str | bytes | None = None):
         """Initializes the internal id using the uuid package.
 
         This initializes the object. Normal use for this object is
         to initialize the constructor with value==None because you
         want to initialize with a novel ID. The only major exception
         is deserialization, wherein a UID object is created with a
         specific id value.
@@ -187,38 +198,38 @@
 
         return str(self.value)[:8]
 
     @property
     def id(self) -> "UID":
         return self
 
-    @staticmethod
-    def _check_or_convert(value: Union[str, "UID", uuid.UUID]) -> "UID":
+    @classmethod
+    def _check_or_convert(cls, value: str | uuid.UUID | UID) -> UID:
         if isinstance(value, uuid.UUID):
             return UID(value)
         elif isinstance(value, str):
             return UID.from_string(value)
-        elif isinstance(value, UID):
+        elif isinstance(value, cls):
             return value
         else:
             # Ask @Madhava , can we check for  invalid types , even though type annotation is specified.
             return ValueError(  # type: ignore
-                f"Incorrect value,type:{value,type(value)} for conversion to UID, expected Union[str,UID,UUID]"
+                f"Incorrect value,type:{value,type(value)} for conversion to UID, expected str | uuid.UUID | Self"
             )
 
 
 @serializable(attrs=["syft_history_hash"])
 class LineageID(UID):
     """Extended UID containing a history hash as well, which is used for comparisons."""
 
     syft_history_hash: int
 
     def __init__(
         self,
-        value: Union[uuid_type, str, bytes, "LineageID"] | None = None,
+        value: Self | UID | uuid_type | str | bytes | None = None,
         syft_history_hash: int | None = None,
     ):
         if isinstance(value, LineageID):
             syft_history_hash = value.syft_history_hash
             value = value.value
 
         super().__init__(value)
```

### Comparing `syft-0.8.7b2/src/syft/util/_std_stream_capture.py` & `syft-0.8.7b3/src/syft/util/_std_stream_capture.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/util/autoreload.py` & `syft-0.8.7b3/src/syft/util/autoreload.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/util/decorators.py` & `syft-0.8.7b3/src/syft/util/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/util/experimental_flags.py` & `syft-0.8.7b3/src/syft/util/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/util/filterwarnings.py` & `syft-0.8.7b3/src/syft/util/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/util/fonts.py` & `syft-0.8.7b3/src/syft/util/fonts.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/util/logger.py` & `syft-0.8.7b3/src/syft/util/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/util/markdown.py` & `syft-0.8.7b3/src/syft/util/markdown.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/util/notebook_ui/components/base.py` & `syft-0.8.7b3/src/syft/util/notebook_ui/components/base.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/util/notebook_ui/components/sync.py` & `syft-0.8.7b3/src/syft/util/notebook_ui/components/sync.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,26 +22,31 @@
     "12.5 9.25979 12.4473 9.35355 12.3536C9.44732 12.2598 9.5 12.1326 9.5 12V9.5H12C12.1326 9.5 12.2598 "
     "9.44732 12.3536 9.35355C12.4473 9.25979 12.5 9.13261 12.5 9V1C12.5 0.867392 12.4473 0.740215 12.3536 "
     "0.646447C12.2598 0.552679 12.1326 0.5 12 0.5ZM8.5 11.5H1.5V4.5H8.5V11.5ZM11.5 8.5H9.5V4C9.5 3.86739 "
     '9.44732 3.74021 9.35355 3.64645C9.25979 3.55268 9.13261 3.5 9 3.5H4.5V1.5H11.5V8.5Z" fill="#B4B0BF"/>'
     "</svg>"
 )
 
+INFO_ICON = """<svg width="14" height="14" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg">
+<path d="M7 1.3125C5.87512 1.3125 4.7755 1.64607 3.8402 2.27102C2.90489 2.89597 2.17591 3.78423 1.74544 4.82349C1.31496 5.86274 1.20233 7.00631 1.42179 8.10958C1.64124 9.21284 2.18292 10.2263 2.97833 11.0217C3.77374 11.8171 4.78716 12.3588 5.89043 12.5782C6.99369 12.7977 8.13726 12.685 9.17651 12.2546C10.2158 11.8241 11.104 11.0951 11.729 10.1598C12.3539 9.2245 12.6875 8.12488 12.6875 7C12.6859 5.49207 12.0862 4.04636 11.0199 2.98009C9.95365 1.91382 8.50793 1.31409 7 1.3125ZM7 11.8125C6.04818 11.8125 5.11773 11.5303 4.32632 11.0014C3.53491 10.4726 2.91808 9.72103 2.55383 8.84166C2.18959 7.9623 2.09428 6.99466 2.27997 6.06113C2.46566 5.12759 2.92401 4.27009 3.59705 3.59705C4.27009 2.92401 5.1276 2.46566 6.06113 2.27997C6.99466 2.09428 7.9623 2.18958 8.84167 2.55383C9.72104 2.91808 10.4726 3.53491 11.0014 4.32632C11.5303 5.11773 11.8125 6.04818 11.8125 7C11.8111 8.27591 11.3036 9.49915 10.4014 10.4014C9.49915 11.3036 8.27591 11.8111 7 11.8125ZM7.875 9.625C7.875 9.74103 7.82891 9.85231 7.74686 9.93436C7.66481 10.0164 7.55353 10.0625 7.4375 10.0625C7.20544 10.0625 6.98288 9.97031 6.81878 9.80622C6.65469 9.64212 6.5625 9.41956 6.5625 9.1875V7C6.44647 7 6.33519 6.95391 6.25314 6.87186C6.1711 6.78981 6.125 6.67853 6.125 6.5625C6.125 6.44647 6.1711 6.33519 6.25314 6.25314C6.33519 6.17109 6.44647 6.125 6.5625 6.125C6.79457 6.125 7.01713 6.21719 7.18122 6.38128C7.34531 6.54538 7.4375 6.76794 7.4375 7V9.1875C7.55353 9.1875 7.66481 9.23359 7.74686 9.31564C7.82891 9.39769 7.875 9.50897 7.875 9.625ZM6.125 4.59375C6.125 4.46396 6.16349 4.33708 6.2356 4.22916C6.30771 4.12124 6.4102 4.03712 6.53012 3.98745C6.65003 3.93778 6.78198 3.92479 6.90928 3.95011C7.03658 3.97543 7.15351 4.03793 7.24529 4.12971C7.33707 4.22149 7.39957 4.33842 7.42489 4.46572C7.45021 4.59302 7.43722 4.72497 7.38755 4.84489C7.33788 4.9648 7.25377 5.06729 7.14585 5.1394C7.03793 5.21151 6.91105 5.25 6.78125 5.25C6.6072 5.25 6.44028 5.18086 6.31721 5.05779C6.19414 4.93472 6.125 4.7678 6.125 4.59375Z" fill="#1F567A"/>
+</svg>
+"""  # noqa: E501
+
 COPY_CSS = """
 .copy-container {
   cursor: pointer;
   border-radius: 3px;
   padding: 0px 3px;
   display: inline-block;
   transition: background-color 0.3s;
   user-select: none;
   color: #B4B0BF;
   overflow: hidden;
   white-space: nowrap;
-;
+  vertical-align: middle;
 }
 
 .copy-container:hover {
   background-color: #f5f5f5;
 }
 
 .copy-container:active {
@@ -123,14 +128,54 @@
             </span>
             </div>
         """  # noqa: E501
         summary_html = summary_html.replace("\n", "").replace("    ", "")
         return summary_html
 
 
+ALERT_CSS = """
+.syft-alert-container {
+    padding: 4px;
+    display: flex;
+    justify-content: center;
+}
+
+.syft-alert-info {
+    display: flex;
+    align-items: center;
+    width: 100%;
+    padding: 8px 10px;
+    gap: 8px;
+    border-radius: 4px;
+    background: #C2DEF0;
+    color: #1F567A;
+    line-height: 1.4;
+    font-size: 12px;
+    font-family: 'Open Sans';
+}
+"""
+
+
+class Alert(HTMLComponentBase):
+    __canonical_name__ = "Alert"
+    __version__ = SYFT_OBJECT_VERSION_1  # Ensure the version constant is correctly defined elsewhere
+    message: str
+
+    def to_html(self) -> str:
+        full_message = f"{INFO_ICON} {self.message}"
+        return f"""
+            <style>{ALERT_CSS}</style>
+            <div class="syft-alert-container">
+            <div class="syft-alert-info">
+            {full_message}
+            </div>
+            </div>
+            """
+
+
 class Badge(HTMLComponentBase):
     __canonical_name__ = "CopyButton"
     __version__ = SYFT_OBJECT_VERSION_1
     object: SyftObject
 
     def type_badge_class(self) -> str:
         if isinstance(self.object, UserCode):
@@ -153,15 +198,15 @@
     __version__ = SYFT_OBJECT_VERSION_1
     object: SyftObject
 
     def main_object_description_str(self) -> str:
         if isinstance(self.object, UserCode):
             return self.object.service_func_name
         elif isinstance(self.object, Job):  # type: ignore
-            return self.object.user_code_name
+            return self.object.user_code_name or ""
         elif isinstance(self.object, Request):  # type: ignore
             # TODO: handle other requests
             return f"Execute {self.object.code.service_func_name}"
         # SyftLog
         # ExecutionOutput
         # ActionObject
         # UserCodeStatusCollection
@@ -213,15 +258,15 @@
             source_side = "Low"
             target_side = "High"
 
         # Third line HTML
         third_line_html = f"<span style='color: #5E5A72;'>This would sync <span style='color: #B8520A'>{num_diffs} changes </span> from <i>{source_side} Node</i> to <i>{target_side} Node</i></span>"  # noqa: E501
 
         header_html = f"""
-        <style>{style}</style>
+        {style}
         {first_line_html}
         {second_line_html}
         {third_line_html}
         <div style='height: 16px;'></div>
         """
 
         return header_html
```

### Comparing `syft-0.8.7b2/src/syft/util/notebook_ui/notebook_addons.py` & `syft-0.8.7b3/src/syft/util/notebook_ui/notebook_addons.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,2066 +3,2186 @@
 00000020: 706f 7274 2053 6571 7565 6e63 650a 696d  port Sequence.im
 00000030: 706f 7274 206a 736f 6e0a 6672 6f6d 2073  port json.from s
 00000040: 7472 696e 6720 696d 706f 7274 2054 656d  tring import Tem
 00000050: 706c 6174 650a 6672 6f6d 2074 7970 696e  plate.from typin
 00000060: 6720 696d 706f 7274 2041 6e79 0a0a 2320  g import Any..# 
 00000070: 7265 6c61 7469 7665 0a66 726f 6d20 2e2e  relative.from ..
 00000080: 2e74 7970 6573 2e75 6964 2069 6d70 6f72  .types.uid impor
-00000090: 7420 5549 440a 0a43 5353 5f43 4f44 4520  t UID..CSS_CODE 
-000000a0: 3d20 2222 220a 3c73 7479 6c65 3e0a 2020  = """.<style>.  
-000000b0: 626f 6479 5b64 6174 612d 6a70 2d74 6865  body[data-jp-the
-000000c0: 6d65 2d6c 6967 6874 3d27 6661 6c73 6527  me-light='false'
-000000d0: 5d20 7b0a 2020 2020 2020 2020 2d2d 7072  ] {.        --pr
-000000e0: 696d 6172 792d 636f 6c6f 723a 2023 3131  imary-color: #11
-000000f0: 3131 3131 3b0a 2020 2020 2020 2020 2d2d  1111;.        --
-00000100: 7365 636f 6e64 6172 792d 636f 6c6f 723a  secondary-color:
-00000110: 2023 3231 3231 3231 3b0a 2020 2020 2020   #212121;.      
-00000120: 2020 2d2d 7465 7274 6961 7279 2d63 6f6c    --tertiary-col
-00000130: 6f72 3a20 2343 4643 4444 363b 0a20 2020  or: #CFCDD6;.   
-00000140: 2020 2020 202d 2d62 7574 746f 6e2d 636f       --button-co
-00000150: 6c6f 723a 2023 3131 3131 3131 3b0a 2020  lor: #111111;.  
-00000160: 7d0a 0a20 2062 6f64 7920 7b0a 2020 2020  }..  body {.    
-00000170: 2020 2020 2d2d 7072 696d 6172 792d 636f      --primary-co
-00000180: 6c6f 723a 2023 6666 6666 6666 3b0a 2020  lor: #ffffff;.  
-00000190: 2020 2020 2020 2d2d 7365 636f 6e64 6172        --secondar
-000001a0: 792d 636f 6c6f 723a 2023 6635 6635 6635  y-color: #f5f5f5
-000001b0: 3b0a 2020 2020 2020 2020 2d2d 7465 7274  ;.        --tert
-000001c0: 6961 7279 2d63 6f6c 6f72 3a20 2330 3030  iary-color: #000
-000001d0: 3030 3064 653b 0a20 2020 2020 2020 202d  000de;.        -
-000001e0: 2d62 7574 746f 6e2d 636f 6c6f 723a 2023  -button-color: #
-000001f0: 6431 6435 6462 3b0a 2020 7d0a 0a20 202e  d1d5db;.  }..  .
-00000200: 6865 6164 6572 2d31 207b 0a20 2020 2020  header-1 {.     
-00000210: 2020 2066 6f6e 742d 7374 796c 653a 206e     font-style: n
-00000220: 6f72 6d61 6c3b 0a20 2020 2020 2020 2066  ormal;.        f
-00000230: 6f6e 742d 7765 6967 6874 3a20 3630 303b  ont-weight: 600;
-00000240: 0a20 2020 2020 2020 2066 6f6e 742d 7369  .        font-si
-00000250: 7a65 3a20 322e 3037 3336 656d 3b0a 2020  ze: 2.0736em;.  
-00000260: 2020 2020 2020 6c69 6e65 2d68 6569 6768        line-heigh
-00000270: 743a 2031 3030 253b 0a20 2020 2020 2020  t: 100%;.       
-00000280: 206c 6561 6469 6e67 2d74 7269 6d3a 2062   leading-trim: b
-00000290: 6f74 683b 0a20 2020 2020 2020 2074 6578  oth;.        tex
-000002a0: 742d 6564 6765 3a20 6361 703b 0a20 2020  t-edge: cap;.   
-000002b0: 2020 2020 2063 6f6c 6f72 3a20 2331 3731       color: #171
-000002c0: 3631 443b 0a20 2020 207d 0a0a 2020 2e68  61D;.    }..  .h
-000002d0: 6561 6465 722d 3220 7b0a 2020 2020 2020  eader-2 {.      
-000002e0: 2020 666f 6e74 2d73 7479 6c65 3a20 6e6f    font-style: no
-000002f0: 726d 616c 3b0a 2020 2020 2020 2020 666f  rmal;.        fo
-00000300: 6e74 2d77 6569 6768 743a 2036 3030 3b0a  nt-weight: 600;.
-00000310: 2020 2020 2020 2020 666f 6e74 2d73 697a          font-siz
-00000320: 653a 2031 2e37 3238 656d 3b0a 2020 2020  e: 1.728em;.    
-00000330: 2020 2020 6c69 6e65 2d68 6569 6768 743a      line-height:
-00000340: 2031 3030 253b 0a20 2020 2020 2020 206c   100%;.        l
-00000350: 6561 6469 6e67 2d74 7269 6d3a 2062 6f74  eading-trim: bot
-00000360: 683b 0a20 2020 2020 2020 2074 6578 742d  h;.        text-
-00000370: 6564 6765 3a20 6361 703b 0a20 2020 2020  edge: cap;.     
-00000380: 2020 2063 6f6c 6f72 3a20 2331 3731 3631     color: #17161
-00000390: 443b 0a20 2020 207d 0a0a 2020 2e68 6561  D;.    }..  .hea
-000003a0: 6465 722d 3320 7b0a 2020 2020 2020 2020  der-3 {.        
-000003b0: 666f 6e74 2d73 7479 6c65 3a20 6e6f 726d  font-style: norm
-000003c0: 616c 3b0a 2020 2020 2020 2020 666f 6e74  al;.        font
-000003d0: 2d77 6569 6768 743a 2036 3030 3b0a 2020  -weight: 600;.  
-000003e0: 2020 2020 2020 666f 6e74 2d73 697a 653a        font-size:
-000003f0: 2020 312e 3434 656d 3b0a 2020 2020 2020    1.44em;.      
-00000400: 2020 6c69 6e65 2d68 6569 6768 743a 2031    line-height: 1
-00000410: 3030 253b 0a20 2020 2020 2020 206c 6561  00%;.        lea
-00000420: 6469 6e67 2d74 7269 6d3a 2062 6f74 683b  ding-trim: both;
-00000430: 0a20 2020 2020 2020 2074 6578 742d 6564  .        text-ed
-00000440: 6765 3a20 6361 703b 0a20 2020 2020 2020  ge: cap;.       
-00000450: 2063 6f6c 6f72 3a20 7661 7228 2d2d 7465   color: var(--te
-00000460: 7274 6961 7279 2d63 6f6c 6f72 293b 0a20  rtiary-color);. 
-00000470: 2020 207d 0a0a 2020 2e68 6561 6465 722d     }..  .header-
-00000480: 3420 7b0a 2020 2020 2020 2020 666f 6e74  4 {.        font
-00000490: 2d73 7479 6c65 3a20 6e6f 726d 616c 3b0a  -style: normal;.
-000004a0: 2020 2020 2020 2020 666f 6e74 2d77 6569          font-wei
-000004b0: 6768 743a 2036 3030 3b0a 2020 2020 2020  ght: 600;.      
-000004c0: 2020 666f 6e74 2d73 697a 653a 2031 2e32    font-size: 1.2
-000004d0: 656d 3b0a 2020 2020 2020 2020 6c69 6e65  em;.        line
-000004e0: 2d68 6569 6768 743a 2031 3030 253b 0a20  -height: 100%;. 
-000004f0: 2020 2020 2020 206c 6561 6469 6e67 2d74         leading-t
-00000500: 7269 6d3a 2062 6f74 683b 0a20 2020 2020  rim: both;.     
-00000510: 2020 2074 6578 742d 6564 6765 3a20 6361     text-edge: ca
-00000520: 703b 0a20 2020 2020 2020 2063 6f6c 6f72  p;.        color
-00000530: 3a20 2331 3731 3631 443b 0a20 2020 207d  : #17161D;.    }
-00000540: 0a0a 2020 2020 2e70 6172 6167 7261 7068  ..    .paragraph
-00000550: 207b 0a20 2020 2020 2020 2066 6f6e 742d   {.        font-
-00000560: 7374 796c 653a 206e 6f72 6d61 6c3b 0a20  style: normal;. 
-00000570: 2020 2020 2020 2066 6f6e 742d 7765 6967         font-weig
-00000580: 6874 3a20 3430 303b 0a20 2020 2020 2020  ht: 400;.       
-00000590: 2066 6f6e 742d 7369 7a65 3a20 3134 7078   font-size: 14px
-000005a0: 3b0a 2020 2020 2020 2020 6c69 6e65 2d68  ;.        line-h
-000005b0: 6569 6768 743a 2031 3030 253b 0a20 2020  eight: 100%;.   
-000005c0: 2020 2020 206c 6561 6469 6e67 2d74 7269       leading-tri
-000005d0: 6d3a 2062 6f74 683b 0a20 2020 2020 2020  m: both;.       
-000005e0: 2074 6578 742d 6564 6765 3a20 6361 703b   text-edge: cap;
-000005f0: 0a20 2020 2020 2020 2063 6f6c 6f72 3a20  .        color: 
-00000600: 2332 4532 4233 423b 0a20 2020 207d 0a0a  #2E2B3B;.    }..
-00000610: 2020 2020 2e70 6172 6167 7261 7068 2d73      .paragraph-s
-00000620: 6d20 7b0a 2020 2020 2020 2020 666f 6e74  m {.        font
-00000630: 2d66 616d 696c 793a 2027 526f 626f 746f  -family: 'Roboto
-00000640: 273b 0a20 2020 2020 2020 2066 6f6e 742d  ';.        font-
-00000650: 7374 796c 653a 206e 6f72 6d61 6c3b 0a20  style: normal;. 
-00000660: 2020 2020 2020 2066 6f6e 742d 7765 6967         font-weig
-00000670: 6874 3a20 3430 303b 0a20 2020 2020 2020  ht: 400;.       
-00000680: 2066 6f6e 742d 7369 7a65 3a20 3131 2e36   font-size: 11.6
-00000690: 3270 783b 0a20 2020 2020 2020 206c 696e  2px;.        lin
-000006a0: 652d 6865 6967 6874 3a20 3130 3025 3b0a  e-height: 100%;.
-000006b0: 2020 2020 2020 2020 6c65 6164 696e 672d          leading-
-000006c0: 7472 696d 3a20 626f 7468 3b0a 2020 2020  trim: both;.    
-000006d0: 2020 2020 7465 7874 2d65 6467 653a 2063      text-edge: c
-000006e0: 6170 3b0a 2020 2020 2020 2020 636f 6c6f  ap;.        colo
-000006f0: 723a 2023 3245 3242 3342 3b0a 2020 2020  r: #2E2B3B;.    
-00000700: 7d0a 2020 2020 2e63 6f64 652d 7465 7874  }.    .code-text
-00000710: 207b 0a20 2020 2020 2020 2066 6f6e 742d   {.        font-
-00000720: 6661 6d69 6c79 3a20 2743 6f6e 736f 6c61  family: 'Consola
-00000730: 7327 3b0a 2020 2020 2020 2020 666f 6e74  s';.        font
-00000740: 2d73 7479 6c65 3a20 6e6f 726d 616c 3b0a  -style: normal;.
-00000750: 2020 2020 2020 2020 666f 6e74 2d77 6569          font-wei
-00000760: 6768 743a 2034 3030 3b0a 2020 2020 2020  ght: 400;.      
-00000770: 2020 666f 6e74 2d73 697a 653a 2031 3370    font-size: 13p
-00000780: 783b 0a20 2020 2020 2020 206c 696e 652d  x;.        line-
-00000790: 6865 6967 6874 3a20 3133 3025 3b0a 2020  height: 130%;.  
-000007a0: 2020 2020 2020 6c65 6164 696e 672d 7472        leading-tr
-000007b0: 696d 3a20 626f 7468 3b0a 2020 2020 2020  im: both;.      
-000007c0: 2020 7465 7874 2d65 6467 653a 2063 6170    text-edge: cap
-000007d0: 3b0a 2020 2020 2020 2020 636f 6c6f 723a  ;.        color:
-000007e0: 2023 3245 3242 3342 3b0a 2020 2020 7d0a   #2E2B3B;.    }.
-000007f0: 0a20 2020 202e 6e75 6d62 6572 696e 672d  .    .numbering-
-00000800: 656e 7472 7920 7b20 6469 7370 6c61 793a  entry { display:
-00000810: 206e 6f6e 6520 7d0a 0a20 2020 202f 2a20   none }..    /* 
-00000820: 546f 6f6c 7469 7020 636f 6e74 6169 6e65  Tooltip containe
-00000830: 7220 2a2f 0a20 2020 202e 746f 6f6c 7469  r */.    .toolti
-00000840: 7020 7b0a 2020 2020 2020 2020 706f 7369  p {.        posi
-00000850: 7469 6f6e 3a20 7265 6c61 7469 7665 3b0a  tion: relative;.
-00000860: 2020 2020 2020 2020 6469 7370 6c61 793a          display:
-00000870: 2069 6e6c 696e 652d 626c 6f63 6b3b 0a20   inline-block;. 
-00000880: 2020 2020 2020 2062 6f72 6465 722d 626f         border-bo
-00000890: 7474 6f6d 3a20 3170 7820 646f 7474 6564  ttom: 1px dotted
-000008a0: 2062 6c61 636b 3b20 2f2a 2049 6620 796f   black; /* If yo
-000008b0: 7520 7761 6e74 2064 6f74 7320 756e 6465  u want dots unde
-000008c0: 7220 7468 6520 686f 7665 7261 626c 6520  r the hoverable 
-000008d0: 7465 7874 202a 2f0a 2020 2020 7d0a 0a20  text */.    }.. 
-000008e0: 2020 202f 2a20 546f 6f6c 7469 7020 7465     /* Tooltip te
-000008f0: 7874 202a 2f0a 2020 2020 2e74 6f6f 6c74  xt */.    .toolt
-00000900: 6970 202e 746f 6f6c 7469 7074 6578 7420  ip .tooltiptext 
-00000910: 7b0a 2020 2020 2020 2020 7669 7369 6269  {.        visibi
-00000920: 6c69 7479 3a20 6869 6464 656e 3b0a 2020  lity: hidden;.  
-00000930: 2020 2020 2020 7769 6474 683a 2031 3230        width: 120
-00000940: 7078 3b0a 2020 2020 2020 2020 6261 636b  px;.        back
-00000950: 6772 6f75 6e64 2d63 6f6c 6f72 3a20 626c  ground-color: bl
-00000960: 6163 6b3b 0a20 2020 2020 2020 2063 6f6c  ack;.        col
-00000970: 6f72 3a20 2366 6666 3b0a 2020 2020 2020  or: #fff;.      
-00000980: 2020 7465 7874 2d61 6c69 676e 3a20 6365    text-align: ce
-00000990: 6e74 6572 3b0a 2020 2020 2020 2020 7061  nter;.        pa
-000009a0: 6464 696e 673a 2035 7078 2030 3b0a 2020  dding: 5px 0;.  
-000009b0: 2020 2020 2020 626f 7264 6572 2d72 6164        border-rad
-000009c0: 6975 733a 2036 7078 3b0a 0a20 2020 2020  ius: 6px;..     
-000009d0: 2020 202f 2a20 506f 7369 7469 6f6e 2074     /* Position t
-000009e0: 6865 2074 6f6f 6c74 6970 2074 6578 7420  he tooltip text 
-000009f0: 2d20 7365 6520 6578 616d 706c 6573 2062  - see examples b
-00000a00: 656c 6f77 2120 2a2f 0a20 2020 2020 2020  elow! */.       
-00000a10: 2070 6f73 6974 696f 6e3a 2061 6273 6f6c   position: absol
-00000a20: 7574 653b 0a20 2020 2020 2020 207a 2d69  ute;.        z-i
-00000a30: 6e64 6578 3a20 313b 0a20 2020 207d 0a0a  ndex: 1;.    }..
-00000a40: 2020 2020 2e72 6570 722d 6365 6c6c 207b      .repr-cell {
-00000a50: 0a20 2020 2020 2070 6164 6469 6e67 2d74  .      padding-t
-00000a60: 6f70 3a20 3230 7078 3b0a 2020 2020 7d0a  op: 20px;.    }.
-00000a70: 0a20 2020 202e 7465 7874 2d62 6f6c 6420  .    .text-bold 
-00000a80: 7b0a 2020 2020 2020 2020 666f 6e74 2d77  {.        font-w
-00000a90: 6569 6768 743a 2062 6f6c 643b 0a20 2020  eight: bold;.   
-00000aa0: 207d 0a0a 2020 2020 2e70 722d 3820 7b0a   }..    .pr-8 {.
-00000ab0: 2020 2020 2020 2020 7061 6464 696e 672d          padding-
-00000ac0: 7269 6768 743a 2038 7078 3b0a 2020 2020  right: 8px;.    
-00000ad0: 7d0a 2020 2020 2e70 742d 3820 7b0a 2020  }.    .pt-8 {.  
-00000ae0: 2020 2020 2020 7061 6464 696e 672d 746f        padding-to
-00000af0: 703a 2038 7078 3b0a 2020 2020 7d0a 2020  p: 8px;.    }.  
-00000b00: 2020 2e70 6c2d 3820 7b0a 2020 2020 2020    .pl-8 {.      
-00000b10: 2020 7061 6464 696e 672d 6c65 6674 3a20    padding-left: 
-00000b20: 3870 783b 0a20 2020 207d 0a20 2020 202e  8px;.    }.    .
-00000b30: 7062 2d38 207b 0a20 2020 2020 2020 2070  pb-8 {.        p
-00000b40: 6164 6469 6e67 2d62 6f74 746f 6d3a 2038  adding-bottom: 8
-00000b50: 7078 3b0a 2020 2020 7d0a 0a20 2020 202e  px;.    }..    .
-00000b60: 7079 2d32 357b 0a20 2020 2020 2020 2070  py-25{.        p
-00000b70: 6164 6469 6e67 2d74 6f70 3a20 3235 7078  adding-top: 25px
-00000b80: 3b0a 2020 2020 2020 2020 7061 6464 696e  ;.        paddin
-00000b90: 672d 626f 7474 6f6d 3a20 3235 7078 3b0a  g-bottom: 25px;.
-00000ba0: 2020 2020 7d0a 0a20 2020 202e 666c 6578      }..    .flex
-00000bb0: 207b 0a20 2020 2020 2020 2064 6973 706c   {.        displ
-00000bc0: 6179 3a20 666c 6578 3b0a 2020 2020 7d0a  ay: flex;.    }.
-00000bd0: 0a20 2020 202e 6761 702d 3130 207b 0a20  .    .gap-10 {. 
-00000be0: 2020 2020 2020 2067 6170 3a20 3130 7078         gap: 10px
-00000bf0: 3b0a 2020 2020 7d0a 2020 2020 2e69 7465  ;.    }.    .ite
-00000c00: 6d73 2d63 656e 7465 727b 0a20 2020 2020  ms-center{.     
-00000c10: 2020 2061 6c69 676e 2d69 7465 6d73 3a20     align-items: 
-00000c20: 6365 6e74 6572 3b0a 2020 2020 7d0a 0a20  center;.    }.. 
-00000c30: 2020 202e 666f 6c64 6572 2d69 636f 6e20     .folder-icon 
-00000c40: 7b0a 2020 2020 2020 2020 636f 6c6f 723a  {.        color:
-00000c50: 2076 6172 282d 2d74 6572 7469 6172 792d   var(--tertiary-
-00000c60: 636f 6c6f 7229 3b0a 2020 2020 7d0a 0a20  color);.    }.. 
-00000c70: 2020 202e 7365 6172 6368 2d69 6e70 7574     .search-input
-00000c80: 7b0a 2020 2020 2020 2020 6469 7370 6c61  {.        displa
-00000c90: 793a 2066 6c65 783b 0a20 2020 2020 2020  y: flex;.       
-00000ca0: 2066 6c65 782d 6469 7265 6374 696f 6e3a   flex-direction:
-00000cb0: 2072 6f77 3b0a 2020 2020 2020 2020 616c   row;.        al
-00000cc0: 6967 6e2d 6974 656d 733a 2063 656e 7465  ign-items: cente
-00000cd0: 723b 0a20 2020 2020 2020 2070 6164 6469  r;.        paddi
-00000ce0: 6e67 3a20 3870 7820 3132 7078 3b0a 2020  ng: 8px 12px;.  
-00000cf0: 2020 2020 2020 7769 6474 683a 2033 3433        width: 343
-00000d00: 7078 3b0a 2020 2020 2020 2020 6865 6967  px;.        heig
-00000d10: 6874 3a20 3234 7078 3b0a 2020 2020 2020  ht: 24px;.      
-00000d20: 2020 2f2a 204c 7420 4f6e 2053 7572 6661    /* Lt On Surfa
-00000d30: 6365 2f4c 6f77 202a 2f0a 2020 2020 2020  ce/Low */.      
-00000d40: 2020 6261 636b 6772 6f75 6e64 2d63 6f6c    background-col
-00000d50: 6f72 3a20 7661 7228 2d2d 7365 636f 6e64  or: var(--second
-00000d60: 6172 792d 636f 6c6f 7229 3b0a 2020 2020  ary-color);.    
-00000d70: 2020 2020 626f 7264 6572 2d72 6164 6975      border-radiu
-00000d80: 733a 2033 3070 783b 0a0a 2020 2020 2020  s: 30px;..      
-00000d90: 2020 2f2a 204c 7420 4f6e 2053 7572 6661    /* Lt On Surfa
-00000da0: 6365 2f48 6967 6865 7374 202a 2f0a 2020  ce/Highest */.  
-00000db0: 2020 2020 2020 636f 6c6f 723a 2076 6172        color: var
-00000dc0: 282d 2d74 6572 7469 6172 792d 636f 6c6f  (--tertiary-colo
-00000dd0: 7229 3b0a 2020 2020 2020 2020 626f 7264  r);.        bord
-00000de0: 6572 3a6e 6f6e 653b 0a20 2020 2020 2020  er:none;.       
-00000df0: 202f 2a20 496e 7369 6465 2061 7574 6f20   /* Inside auto 
-00000e00: 6c61 796f 7574 202a 2f0a 2020 2020 2020  layout */.      
-00000e10: 2020 666c 6578 3a20 6e6f 6e65 3b0a 2020    flex: none;.  
-00000e20: 2020 2020 2020 6f72 6465 723a 2030 3b0a        order: 0;.
-00000e30: 2020 2020 2020 2020 666c 6578 2d67 726f          flex-gro
-00000e40: 773a 2030 3b0a 2020 2020 7d0a 2020 2020  w: 0;.    }.    
-00000e50: 2e73 6561 7263 682d 696e 7075 743a 666f  .search-input:fo
-00000e60: 6375 7320 7b0a 2020 2020 2020 2020 6f75  cus {.        ou
-00000e70: 746c 696e 653a 206e 6f6e 653b 0a20 2020  tline: none;.   
-00000e80: 207d 0a20 2020 2020 2020 202e 7365 6172   }.        .sear
-00000e90: 6368 2d69 6e70 7574 3a66 6f63 7573 3a3a  ch-input:focus::
-00000ea0: 706c 6163 6568 6f6c 6465 722c 0a20 2020  placeholder,.   
-00000eb0: 202e 7365 6172 6368 2d69 6e70 7574 3a3a   .search-input::
-00000ec0: 706c 6163 6568 6f6c 6465 7220 7b20 2f2a  placeholder { /*
-00000ed0: 2043 6872 6f6d 652c 2046 6972 6566 6f78   Chrome, Firefox
-00000ee0: 2c20 4f70 6572 612c 2053 6166 6172 6920  , Opera, Safari 
-00000ef0: 3130 2e31 2b20 2a2f 0a20 2020 2020 2020  10.1+ */.       
-00000f00: 2063 6f6c 6f72 3a20 7661 7228 2d2d 7465   color: var(--te
-00000f10: 7274 6961 7279 2d63 6f6c 6f72 293b 0a20  rtiary-color);. 
-00000f20: 2020 2020 2020 206f 7061 6369 7479 3a20         opacity: 
-00000f30: 313b 202f 2a20 4669 7265 666f 7820 2a2f  1; /* Firefox */
-00000f40: 0a20 2020 207d 0a0a 2020 2020 2e73 6561  .    }..    .sea
-00000f50: 7263 682d 6275 7474 6f6e 7b0a 2020 2020  rch-button{.    
-00000f60: 2020 2020 2f2a 2053 6561 7263 6820 2a2f      /* Search */
-00000f70: 0a20 2020 2020 2020 206c 6561 6469 6e67  .        leading
-00000f80: 2d74 7269 6d3a 2062 6f74 683b 0a20 2020  -trim: both;.   
-00000f90: 2020 2020 2074 6578 742d 6564 6765 3a20       text-edge: 
-00000fa0: 6361 703b 0a20 2020 2020 2020 2064 6973  cap;.        dis
-00000fb0: 706c 6179 3a20 666c 6578 3b0a 2020 2020  play: flex;.    
-00000fc0: 2020 2020 616c 6967 6e2d 6974 656d 733a      align-items:
-00000fd0: 2063 656e 7465 723b 0a20 2020 2020 2020   center;.       
-00000fe0: 2074 6578 742d 616c 6967 6e3a 2063 656e   text-align: cen
-00000ff0: 7465 723b 0a0a 2020 2020 2020 2020 2f2a  ter;..        /*
-00001000: 2050 7269 6d61 7279 2f4f 6e20 4c69 6768   Primary/On Ligh
-00001010: 7420 2a2f 0a20 2020 2020 2020 2062 6163  t */.        bac
-00001020: 6b67 726f 756e 642d 636f 6c6f 723a 2076  kground-color: v
-00001030: 6172 282d 2d62 7574 746f 6e2d 636f 6c6f  ar(--button-colo
-00001040: 7229 3b0a 2020 2020 2020 2020 636f 6c6f  r);.        colo
-00001050: 723a 2076 6172 282d 2d74 6572 7469 6172  r: var(--tertiar
-00001060: 792d 636f 6c6f 7229 3b0a 0a20 2020 2020  y-color);..     
-00001070: 2020 2062 6f72 6465 722d 7261 6469 7573     border-radius
-00001080: 3a20 3330 7078 3b0a 2020 2020 2020 2020  : 30px;.        
-00001090: 626f 7264 6572 2d63 6f6c 6f72 3a20 7661  border-color: va
-000010a0: 7228 2d2d 7365 636f 6e64 6172 792d 636f  r(--secondary-co
-000010b0: 6c6f 7229 3b0a 2020 2020 2020 2020 626f  lor);.        bo
-000010c0: 7264 6572 2d73 7479 6c65 3a20 736f 6c69  rder-style: soli
-000010d0: 643b 0a20 2020 2020 2020 2062 6f78 2d73  d;.        box-s
-000010e0: 6861 646f 773a 2072 6762 6128 3630 2c20  hadow: rgba(60, 
-000010f0: 3634 2c20 3637 2c20 302e 3329 2030 7078  64, 67, 0.3) 0px
-00001100: 2031 7078 2032 7078 2030 7078 2c20 7267   1px 2px 0px, rg
-00001110: 6261 2836 302c 2036 342c 2036 372c 2030  ba(60, 64, 67, 0
-00001120: 2e31 3529 2030 7078 2031 7078 2033 7078  .15) 0px 1px 3px
-00001130: 2031 7078 3b0a 2020 2020 2020 2020 6375   1px;.        cu
-00001140: 7273 6f72 3a20 706f 696e 7465 723b 0a20  rsor: pointer;. 
-00001150: 2020 2020 2020 202f 2a20 496e 7369 6465         /* Inside
-00001160: 2061 7574 6f20 6c61 796f 7574 202a 2f0a   auto layout */.
-00001170: 2020 2020 2020 2020 666c 6578 3a20 6e6f          flex: no
-00001180: 6e65 3b0a 2020 2020 2020 2020 6f72 6465  ne;.        orde
-00001190: 723a 2031 3b0a 2020 2020 2020 2020 666c  r: 1;.        fl
-000011a0: 6578 2d67 726f 773a 2030 3b0a 2020 2020  ex-grow: 0;.    
-000011b0: 7d0a 0a20 2020 202e 6772 6964 2d74 6162  }..    .grid-tab
-000011c0: 6c65 247b 7569 647d 207b 0a20 2020 2020  le${uid} {.     
-000011d0: 2020 2064 6973 706c 6179 3a67 7269 643b     display:grid;
-000011e0: 0a20 2020 2020 2020 2067 7269 642d 7465  .        grid-te
-000011f0: 6d70 6c61 7465 2d63 6f6c 756d 6e73 3a20  mplate-columns: 
-00001200: 3166 7220 7265 7065 6174 2824 7b63 6f6c  1fr repeat(${col
-00001210: 737d 2c20 3166 7229 3b0a 2020 2020 2020  s}, 1fr);.      
-00001220: 2020 6772 6964 2d74 656d 706c 6174 652d    grid-template-
-00001230: 726f 7773 3a20 7265 7065 6174 2832 2c20  rows: repeat(2, 
-00001240: 3166 7229 3b0a 2020 2020 2020 2020 6f76  1fr);.        ov
-00001250: 6572 666c 6f77 2d78 3a20 6175 746f 3b0a  erflow-x: auto;.
-00001260: 2020 2020 2020 2020 706f 7369 7469 6f6e          position
-00001270: 3a20 7265 6c61 7469 7665 3b0a 2020 2020  : relative;.    
-00001280: 7d0a 0a20 2020 202e 6772 6964 2d73 7464  }..    .grid-std
-00001290: 2d63 656c 6c73 207b 0a20 2020 2020 2020  -cells {.       
-000012a0: 2067 7269 642d 636f 6c75 6d6e 3a20 7370   grid-column: sp
-000012b0: 616e 2034 3b0a 0a20 2020 207d 0a20 2020  an 4;..    }.   
-000012c0: 202e 6772 6964 2d69 6e64 6578 2d63 656c   .grid-index-cel
-000012d0: 6c73 207b 0a20 2020 2020 2020 2067 7269  ls {.        gri
-000012e0: 642d 636f 6c75 6d6e 3a20 7370 616e 2031  d-column: span 1
-000012f0: 3b0a 2020 2020 2020 2020 2f2a 2074 6d70  ;.        /* tmp
-00001300: 2066 6978 2074 6f20 6d61 6b65 206c 6566   fix to make lef
-00001310: 7420 636f 6c20 7374 616e 6420 6f75 7420  t col stand out 
-00001320: 2866 6978 2077 6974 6820 666f 6e74 2d66  (fix with font-f
-00001330: 616d 696c 7929 202a 2f0a 2020 2020 2020  amily) */.      
-00001340: 2020 666f 6e74 2d77 6569 6768 743a 2036    font-weight: 6
-00001350: 3030 3b0a 2020 2020 2020 2020 6261 636b  00;.        back
-00001360: 6772 6f75 6e64 2d63 6f6c 6f72 3a20 7661  ground-color: va
-00001370: 7228 2d2d 7365 636f 6e64 6172 792d 636f  r(--secondary-co
-00001380: 6c6f 7229 2021 696d 706f 7274 616e 743b  lor) !important;
-00001390: 0a20 2020 2020 2020 2063 6f6c 6f72 3a20  .        color: 
-000013a0: 7661 7228 2d2d 7465 7274 6961 7279 2d63  var(--tertiary-c
-000013b0: 6f6c 6f72 293b 0a20 2020 207d 0a0a 2020  olor);.    }..  
-000013c0: 2020 2e67 7269 642d 6865 6164 6572 207b    .grid-header {
-000013d0: 0a20 2020 2020 2020 202f 2a20 4175 746f  .        /* Auto
-000013e0: 206c 6179 6f75 7420 2a2f 0a20 2020 2020   layout */.     
-000013f0: 2020 2064 6973 706c 6179 3a20 666c 6578     display: flex
-00001400: 3b0a 2020 2020 2020 2020 666c 6578 2d64  ;.        flex-d
-00001410: 6972 6563 7469 6f6e 3a20 636f 6c75 6d6e  irection: column
-00001420: 3b0a 2020 2020 2020 2020 616c 6967 6e2d  ;.        align-
-00001430: 6974 656d 733a 2063 656e 7465 723b 0a20  items: center;. 
-00001440: 2020 2020 2020 2070 6164 6469 6e67 3a20         padding: 
-00001450: 3670 7820 3470 783b 0a0a 2020 2020 2020  6px 4px;..      
-00001460: 2020 7265 7369 7a65 3a20 686f 7269 7a6f    resize: horizo
-00001470: 6e74 616c 3b0a 2020 2020 2020 2020 2f2a  ntal;.        /*
-00001480: 204c 7420 4f6e 2053 7572 6661 6365 2f53   Lt On Surface/S
-00001490: 7572 6661 6365 202a 2f0a 2020 2020 2020  urface */.      
-000014a0: 2020 2f2a 204c 7420 4f6e 2053 7572 6661    /* Lt On Surfa
-000014b0: 6365 2f48 6967 6820 2a2f 0a20 2020 2020  ce/High */.     
-000014c0: 2020 2062 6f72 6465 723a 2031 7078 2073     border: 1px s
-000014d0: 6f6c 6964 2023 4346 4344 4436 3b0a 2020  olid #CFCDD6;.  
-000014e0: 2020 2020 2020 2f2a 2074 6d70 2066 6978        /* tmp fix
-000014f0: 2074 6f20 6d61 6b65 2068 6561 6465 7220   to make header 
-00001500: 7374 616e 6420 6f75 7420 2866 6978 2077  stand out (fix w
-00001510: 6974 6820 666f 6e74 2d66 616d 696c 7929  ith font-family)
-00001520: 202a 2f0a 2020 2020 2020 2020 666f 6e74   */.        font
-00001530: 2d77 6569 6768 743a 2036 3030 3b0a 2020  -weight: 600;.  
-00001540: 2020 2020 2020 6261 636b 6772 6f75 6e64        background
-00001550: 2d63 6f6c 6f72 3a20 7661 7228 2d2d 7365  -color: var(--se
-00001560: 636f 6e64 6172 792d 636f 6c6f 7229 3b0a  condary-color);.
-00001570: 2020 2020 2020 2020 636f 6c6f 723a 2076          color: v
-00001580: 6172 282d 2d74 6572 7469 6172 792d 636f  ar(--tertiary-co
-00001590: 6c6f 7229 3b0a 2020 2020 7d0a 0a20 2020  lor);.    }..   
-000015a0: 202e 6772 6964 2d72 6f77 207b 0a20 2020   .grid-row {.   
-000015b0: 2020 2020 2064 6973 706c 6179 3a20 666c       display: fl
-000015c0: 6578 3b0a 2020 2020 2020 2020 666c 6578  ex;.        flex
-000015d0: 2d64 6972 6563 7469 6f6e 3a20 636f 6c75  -direction: colu
-000015e0: 6d6e 3b0a 2020 2020 2020 2020 616c 6967  mn;.        alig
-000015f0: 6e2d 6974 656d 733a 2066 6c65 782d 7374  n-items: flex-st
-00001600: 6172 743b 0a20 2020 2020 2020 2070 6164  art;.        pad
-00001610: 6469 6e67 3a20 3670 7820 3470 783b 0a20  ding: 6px 4px;. 
-00001620: 2020 2020 2020 206f 7665 7266 6c6f 773a         overflow:
-00001630: 2068 6964 6465 6e3b 0a20 2020 2020 2020   hidden;.       
-00001640: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-00001650: 6964 2023 4346 4344 4436 3b0a 2020 2020  id #CFCDD6;.    
-00001660: 2020 2020 6261 636b 6772 6f75 6e64 2d63      background-c
-00001670: 6f6c 6f72 3a20 7661 7228 2d2d 7072 696d  olor: var(--prim
-00001680: 6172 792d 636f 6c6f 7229 3b0a 2020 2020  ary-color);.    
-00001690: 2020 2020 636f 6c6f 723a 2076 6172 282d      color: var(-
-000016a0: 2d74 6572 7469 6172 792d 636f 6c6f 7229  -tertiary-color)
-000016b0: 3b0a 2020 2020 7d0a 0a0a 2020 2020 2e73  ;.    }...    .s
-000016c0: 796e 6373 7461 7465 2d63 6f6c 2d66 6f6f  yncstate-col-foo
-000016d0: 7465 7220 7b0a 2020 2020 2020 2020 666f  ter {.        fo
-000016e0: 6e74 2d66 616d 696c 793a 2027 4465 6a61  nt-family: 'Deja
-000016f0: 5675 2053 616e 7320 4d6f 6e6f 272c 2027  Vu Sans Mono', '
-00001700: 4f70 656e 2053 616e 7327 3b0a 2020 2020  Open Sans';.    
-00001710: 2020 2020 666f 6e74 2d73 697a 653a 2031      font-size: 1
-00001720: 3270 783b 0a20 2020 2020 2020 2066 6f6e  2px;.        fon
-00001730: 742d 7765 6967 6874 3a20 3430 303b 0a20  t-weight: 400;. 
-00001740: 2020 2020 2020 206c 696e 652d 6865 6967         line-heig
-00001750: 6874 3a20 3136 2e38 7078 3b0a 2020 2020  ht: 16.8px;.    
-00001760: 2020 2020 7465 7874 2d61 6c69 676e 3a20      text-align: 
-00001770: 6c65 6674 3b0a 2020 2020 2020 2020 636f  left;.        co
-00001780: 6c6f 723a 2023 3545 3541 3732 3b0a 2020  lor: #5E5A72;.  
-00001790: 2020 7d0a 0a20 2020 202e 7379 6e63 7374    }..    .syncst
-000017a0: 6174 652d 6465 7363 7269 7074 696f 6e20  ate-description 
-000017b0: 7b0a 2020 2020 2020 2020 666f 6e74 2d66  {.        font-f
-000017c0: 616d 696c 793a 204f 7065 6e20 5361 6e73  amily: Open Sans
-000017d0: 3b0a 2020 2020 2020 2020 666f 6e74 2d73  ;.        font-s
-000017e0: 697a 653a 2031 3470 783b 0a20 2020 2020  ize: 14px;.     
-000017f0: 2020 2066 6f6e 742d 7765 6967 6874 3a20     font-weight: 
-00001800: 3630 303b 0a20 2020 2020 2020 206c 696e  600;.        lin
-00001810: 652d 6865 6967 6874 3a20 3139 2e36 7078  e-height: 19.6px
-00001820: 3b0a 2020 2020 2020 2020 7465 7874 2d61  ;.        text-a
-00001830: 6c69 676e 3a20 6c65 6674 3b0a 2020 2020  lign: left;.    
-00001840: 2020 2020 7768 6974 652d 7370 6163 653a      white-space:
-00001850: 206e 6f77 7261 703b 0a20 2020 2020 2020   nowrap;.       
-00001860: 2066 6c65 782d 6772 6f77 3a20 313b 0a20   flex-grow: 1;. 
-00001870: 2020 207d 0a0a 2020 2020 2e77 6964 6765     }..    .widge
-00001880: 742d 6865 6164 6572 327b 0a20 2020 2020  t-header2{.     
-00001890: 2020 2064 6973 706c 6179 3a20 666c 6578     display: flex
-000018a0: 3b0a 2020 2020 2020 2020 6761 703a 2038  ;.        gap: 8
-000018b0: 7078 3b0a 2020 2020 2020 2020 6a75 7374  px;.        just
-000018c0: 6966 792d 636f 6e74 656e 743a 2073 7461  ify-content: sta
-000018d0: 7274 3b0a 2020 2020 2020 2020 7769 6474  rt;.        widt
-000018e0: 683a 2031 3030 253b 0a20 2020 2020 2020  h: 100%;.       
-000018f0: 206f 7665 7266 6c6f 773a 2068 6964 6465   overflow: hidde
-00001900: 6e3b 0a20 2020 2020 2020 2061 6c69 676e  n;.        align
-00001910: 2d69 7465 6d73 3a20 6365 6e74 6572 3b0a  -items: center;.
-00001920: 2020 2020 7d0a 0a20 2020 202e 7769 6467      }..    .widg
-00001930: 6574 2d68 6561 6465 7232 2d32 7b0a 2020  et-header2-2{.  
-00001940: 2020 2020 2020 6469 7370 6c61 793a 2066        display: f
-00001950: 6c65 783b 0a20 2020 2020 2020 2067 6170  lex;.        gap
-00001960: 3a20 3870 783b 0a20 2020 2020 2020 206a  : 8px;.        j
-00001970: 7573 7469 6679 2d63 6f6e 7465 6e74 3a20  ustify-content: 
-00001980: 7374 6172 743b 0a20 2020 2020 2020 2061  start;.        a
-00001990: 6c69 676e 2d69 7465 6d73 3a20 6365 6e74  lign-items: cent
-000019a0: 6572 3b0a 2020 2020 7d0a 0a20 2020 202e  er;.    }..    .
-000019b0: 6469 6666 2d73 7461 7465 2d6f 7261 6e67  diff-state-orang
-000019c0: 652d 7465 7874 7b0a 2020 2020 2020 2020  e-text{.        
-000019d0: 636f 6c6f 723a 2023 4238 3532 3041 3b0a  color: #B8520A;.
-000019e0: 2020 2020 7d0a 0a20 2020 202e 6469 6666      }..    .diff
-000019f0: 2d73 7461 7465 2d6e 6f2d 6f62 6a7b 0a20  -state-no-obj{. 
-00001a00: 2020 2020 2020 2066 6f6e 742d 6661 6d69         font-fami
-00001a10: 6c79 3a20 2744 656a 6156 7520 5361 6e73  ly: 'DejaVu Sans
-00001a20: 204d 6f6e 6f27 2c20 274f 7065 6e20 5361   Mono', 'Open Sa
-00001a30: 6e73 273b 0a20 2020 2020 2020 2066 6f6e  ns';.        fon
-00001a40: 742d 7369 7a65 3a20 3132 7078 3b0a 2020  t-size: 12px;.  
-00001a50: 2020 2020 2020 666f 6e74 2d77 6569 6768        font-weigh
-00001a60: 743a 2034 3030 3b0a 2020 2020 2020 2020  t: 400;.        
-00001a70: 6c69 6e65 2d68 6569 6768 743a 2031 362e  line-height: 16.
-00001a80: 3870 783b 0a20 2020 2020 2020 2074 6578  8px;.        tex
-00001a90: 742d 616c 6967 6e3a 206c 6566 743b 0a20  t-align: left;. 
-00001aa0: 2020 2020 2020 2063 6f6c 6f72 3a20 2335         color: #5
-00001ab0: 4535 4137 323b 0a20 2020 207d 0a0a 2020  E5A72;.    }..  
-00001ac0: 2020 2e64 6966 662d 7374 6174 652d 696e    .diff-state-in
-00001ad0: 7472 6f7b 0a20 2020 2020 2020 2066 6f6e  tro{.        fon
-00001ae0: 742d 6661 6d69 6c79 3a20 4f70 656e 2053  t-family: Open S
-00001af0: 616e 733b 0a20 2020 2020 2020 2066 6f6e  ans;.        fon
-00001b00: 742d 7369 7a65 3a20 3134 7078 3b0a 2020  t-size: 14px;.  
-00001b10: 2020 2020 2020 666f 6e74 2d77 6569 6768        font-weigh
-00001b20: 743a 2034 3030 3b0a 2020 2020 2020 2020  t: 400;.        
-00001b30: 6c69 6e65 2d68 6569 6768 743a 2031 392e  line-height: 19.
-00001b40: 3670 783b 0a20 2020 2020 2020 2074 6578  6px;.        tex
-00001b50: 742d 616c 6967 6e3a 206c 6566 743b 0a20  t-align: left;. 
-00001b60: 2020 2020 2020 2063 6f6c 6f72 3a20 2342         color: #B
-00001b70: 3442 3042 463b 0a20 2020 207d 0a0a 2020  4B0BF;.    }..  
-00001b80: 2020 2e64 6966 662d 7374 6174 652d 6865    .diff-state-he
-00001b90: 6164 6572 7b0a 2020 2020 2020 2020 666f  ader{.        fo
-00001ba0: 6e74 2d66 616d 696c 793a 204f 7065 6e20  nt-family: Open 
-00001bb0: 5361 6e73 3b0a 2020 2020 2020 2020 666f  Sans;.        fo
-00001bc0: 6e74 2d73 697a 653a 2032 3270 783b 0a20  nt-size: 22px;. 
-00001bd0: 2020 2020 2020 2066 6f6e 742d 7765 6967         font-weig
-00001be0: 6874 3a20 3630 303b 0a20 2020 2020 2020  ht: 600;.       
-00001bf0: 206c 696e 652d 6865 6967 6874 3a20 3330   line-height: 30
-00001c00: 2e38 7078 3b0a 2020 2020 2020 2020 7465  .8px;.        te
-00001c10: 7874 2d61 6c69 676e 3a20 6c65 6674 3b0a  xt-align: left;.
-00001c20: 2020 2020 2020 2020 636f 6c6f 723a 2023          color: #
-00001c30: 3335 3332 3433 3b0a 2020 2020 2020 2020  353243;.        
-00001c40: 6469 7370 6c61 793a 2066 6c65 783b 2067  display: flex; g
-00001c50: 6170 3a20 3870 783b 0a20 2020 207d 0a0a  ap: 8px;.    }..
-00001c60: 2020 2020 2e64 6966 662d 7374 6174 652d      .diff-state-
-00001c70: 7375 622d 6865 6164 6572 7b0a 2020 2020  sub-header{.    
-00001c80: 2020 2020 666f 6e74 2d66 616d 696c 793a      font-family:
-00001c90: 204f 7065 6e20 5361 6e73 3b0a 2020 2020   Open Sans;.    
-00001ca0: 2020 2020 666f 6e74 2d73 697a 653a 2031      font-size: 1
-00001cb0: 3470 783b 0a20 2020 2020 2020 2066 6f6e  4px;.        fon
-00001cc0: 742d 7765 6967 6874 3a20 3430 303b 0a20  t-weight: 400;. 
-00001cd0: 2020 2020 2020 206c 696e 652d 6865 6967         line-heig
-00001ce0: 6874 3a20 3139 2e36 7078 3b0a 2020 2020  ht: 19.6px;.    
-00001cf0: 2020 2020 7465 7874 2d61 6c69 676e 3a20      text-align: 
-00001d00: 6c65 6674 3b0a 2020 2020 2020 2020 636f  left;.        co
-00001d10: 6c6f 723a 2023 3545 3541 3732 3b0a 2020  lor: #5E5A72;.  
-00001d20: 2020 7d0a 0a20 2020 202e 6261 6467 6520    }..    .badge 
-00001d30: 7b0a 2020 2020 2020 2020 636f 6465 2d74  {.        code-t
-00001d40: 6578 743b 0a20 2020 2020 2020 2062 6f72  ext;.        bor
-00001d50: 6465 722d 7261 6469 7573 3a20 3330 7078  der-radius: 30px
-00001d60: 3b0a 2020 2020 7d0a 0a20 2020 202e 6c61  ;.    }..    .la
-00001d70: 6265 6c20 7b0a 2020 2020 2020 2020 636f  bel {.        co
-00001d80: 6465 2d74 6578 743b 0a20 2020 2020 2020  de-text;.       
-00001d90: 2062 6f72 6465 722d 7261 6469 7573 3a20   border-radius: 
-00001da0: 3470 783b 0a20 2020 2020 2020 2070 6164  4px;.        pad
-00001db0: 6469 6e67 3a20 3670 7820 3470 783b 0a20  ding: 6px 4px;. 
-00001dc0: 2020 2020 2020 2077 6869 7465 2d73 7061         white-spa
-00001dd0: 6365 3a20 6e6f 7772 6170 3b0a 2020 2020  ce: nowrap;.    
-00001de0: 2020 2020 6f76 6572 666c 6f77 3a20 6869      overflow: hi
-00001df0: 6464 656e 3b0a 2020 2020 2020 2020 6c69  dden;.        li
-00001e00: 6e65 2d68 6569 6768 743a 2031 2e32 3b0a  ne-height: 1.2;.
-00001e10: 2020 2020 2020 2020 666f 6e74 2d66 616d          font-fam
-00001e20: 696c 793a 206d 6f6e 6f73 7061 6365 3b0a  ily: monospace;.
-00001e30: 2020 2020 7d0a 0a20 2020 202e 6c61 6265      }..    .labe
-00001e40: 6c2d 6c69 6768 742d 7075 7270 6c65 207b  l-light-purple {
-00001e50: 0a20 2020 2020 2020 206c 6162 656c 3b0a  .        label;.
-00001e60: 2020 2020 2020 2020 6261 636b 6772 6f75          backgrou
-00001e70: 6e64 2d63 6f6c 6f72 3a20 2343 3943 4645  nd-color: #C9CFE
-00001e80: 383b 0a20 2020 2020 2020 2063 6f6c 6f72  8;.        color
-00001e90: 3a20 2333 3733 4237 423b 0a20 2020 207d  : #373B7B;.    }
-00001ea0: 0a0a 2020 2020 2e6c 6162 656c 2d6c 6967  ..    .label-lig
-00001eb0: 6874 2d62 6c75 6520 7b0a 2020 2020 2020  ht-blue {.      
-00001ec0: 2020 6c61 6265 6c3b 0a20 2020 2020 2020    label;.       
-00001ed0: 2062 6163 6b67 726f 756e 642d 636f 6c6f   background-colo
-00001ee0: 723a 2023 4332 4445 4630 3b0a 2020 2020  r: #C2DEF0;.    
-00001ef0: 2020 2020 636f 6c6f 723a 2023 3146 3536      color: #1F56
-00001f00: 3741 3b0a 0a20 2020 207d 0a0a 2020 2020  7A;..    }..    
-00001f10: 2e6c 6162 656c 2d6f 7261 6e67 6520 7b0a  .label-orange {.
-00001f20: 2020 2020 2020 2020 6261 6467 653b 0a20          badge;. 
-00001f30: 2020 2020 2020 2062 6163 6b67 726f 756e         backgroun
-00001f40: 642d 636f 6c6f 723a 2023 4645 4539 4344  d-color: #FEE9CD
-00001f50: 3b0a 2020 2020 2020 2020 636f 6c6f 723a  ;.        color:
-00001f60: 2023 4238 3532 3041 3b0a 2020 2020 7d0a   #B8520A;.    }.
-00001f70: 0a20 2020 202e 6c61 6265 6c2d 6772 6179  .    .label-gray
-00001f80: 207b 0a20 2020 2020 2020 2062 6164 6765   {.        badge
-00001f90: 3b0a 2020 2020 2020 2020 6261 636b 6772  ;.        backgr
-00001fa0: 6f75 6e64 2d63 6f6c 6f72 3a20 2345 4345  ound-color: #ECE
-00001fb0: 4245 463b 0a20 2020 2020 2020 2063 6f6c  BEF;.        col
-00001fc0: 6f72 3a20 2333 3533 3234 333b 0a20 2020  or: #353243;.   
-00001fd0: 207d 0a0a 2020 2020 2e6c 6162 656c 2d67   }..    .label-g
-00001fe0: 7265 656e 207b 0a20 2020 2020 2020 2062  reen {.        b
-00001ff0: 6164 6765 3b0a 2020 2020 2020 2020 6261  adge;.        ba
-00002000: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a20  ckground-color: 
-00002010: 2344 3546 3144 353b 0a20 2020 2020 2020  #D5F1D5;.       
-00002020: 2063 6f6c 6f72 3a20 2332 3536 4232 343b   color: #256B24;
-00002030: 0a20 2020 207d 0a0a 2020 2020 2e62 6164  .    }..    .bad
-00002040: 6765 2d62 6c75 6520 7b0a 2020 2020 2020  ge-blue {.      
-00002050: 2020 6261 6467 653b 0a20 2020 2020 2020    badge;.       
-00002060: 2062 6163 6b67 726f 756e 642d 636f 6c6f   background-colo
-00002070: 723a 2023 4332 4445 4630 3b0a 2020 2020  r: #C2DEF0;.    
-00002080: 2020 2020 636f 6c6f 723a 2023 3146 3536      color: #1F56
-00002090: 3741 3b0a 2020 2020 7d0a 0a20 2020 202e  7A;.    }..    .
-000020a0: 6261 6467 652d 7075 7270 6c65 207b 0a20  badge-purple {. 
-000020b0: 2020 2020 2020 2062 6164 6765 3b0a 2020         badge;.  
-000020c0: 2020 2020 2020 6261 636b 6772 6f75 6e64        background
-000020d0: 2d63 6f6c 6f72 3a20 2343 3943 4645 383b  -color: #C9CFE8;
-000020e0: 0a20 2020 2020 2020 2063 6f6c 6f72 3a20  .        color: 
-000020f0: 2333 3733 4237 423b 0a20 2020 207d 0a0a  #373B7B;.    }..
-00002100: 2020 2020 2e62 6164 6765 2d67 7265 656e      .badge-green
-00002110: 207b 0a20 2020 2020 2020 2062 6164 6765   {.        badge
-00002120: 3b0a 0a20 2020 2020 2020 202f 2a20 5375  ;..        /* Su
-00002130: 6363 6573 732f 436f 6e74 6169 6e65 7220  ccess/Container 
-00002140: 2a2f 0a20 2020 2020 2020 2062 6163 6b67  */.        backg
-00002150: 726f 756e 642d 636f 6c6f 723a 2023 4435  round-color: #D5
-00002160: 4631 4435 3b0a 2020 2020 2020 2020 636f  F1D5;.        co
-00002170: 6c6f 723a 2023 3235 3642 3234 3b0a 2020  lor: #256B24;.  
-00002180: 2020 7d0a 0a20 2020 202e 6261 6467 652d    }..    .badge-
-00002190: 7265 6420 7b0a 2020 2020 2020 2020 6261  red {.        ba
-000021a0: 6467 653b 0a20 2020 2020 2020 2062 6163  dge;.        bac
-000021b0: 6b67 726f 756e 642d 636f 6c6f 723a 2023  kground-color: #
-000021c0: 4632 4439 4445 3b0a 2020 2020 2020 2020  F2D9DE;.        
-000021d0: 636f 6c6f 723a 2023 3942 3237 3337 3b0a  color: #9B2737;.
-000021e0: 2020 2020 7d0a 0a20 2020 202e 6261 6467      }..    .badg
-000021f0: 652d 6772 6179 207b 0a20 2020 2020 2020  e-gray {.       
-00002200: 2062 6164 6765 3b0a 2020 2020 2020 2020   badge;.        
-00002210: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
-00002220: 3a20 2345 4345 4245 463b 0a20 2020 2020  : #ECEBEF;.     
-00002230: 2020 2063 6f6c 6f72 3a20 2332 4532 4233     color: #2E2B3
-00002240: 423b 0a20 2020 207d 0a20 2020 202e 7061  B;.    }.    .pa
-00002250: 6769 6e61 7469 6f6e 436f 6e74 6169 6e65  ginationContaine
-00002260: 727b 0a20 2020 2020 2020 2077 6964 7468  r{.        width
-00002270: 3a20 3130 3025 3b0a 2020 2020 2020 2020  : 100%;.        
-00002280: 2f2a 6865 6967 6874 3a20 3330 7078 3b2a  /*height: 30px;*
-00002290: 2f0a 2020 2020 2020 2020 6469 7370 6c61  /.        displa
-000022a0: 793a 2066 6c65 783b 0a20 2020 2020 2020  y: flex;.       
-000022b0: 206a 7573 7469 6679 2d63 6f6e 7465 6e74   justify-content
-000022c0: 3a20 6365 6e74 6572 3b0a 2020 2020 2020  : center;.      
-000022d0: 2020 6761 703a 2038 7078 3b0a 2020 2020    gap: 8px;.    
-000022e0: 2020 2020 7061 6464 696e 673a 2035 7078      padding: 5px
-000022f0: 3b0a 2020 2020 2020 2020 636f 6c6f 723a  ;.        color:
-00002300: 2076 6172 282d 2d74 6572 7469 6172 792d   var(--tertiary-
-00002310: 636f 6c6f 7229 3b0a 2020 2020 7d0a 0a20  color);.    }.. 
-00002320: 2020 202e 7769 6467 6574 2d6c 6162 656c     .widget-label
-00002330: 2d62 6173 6963 7b0a 2020 2020 2020 2020  -basic{.        
-00002340: 6469 7370 6c61 793a 666c 6578 3b0a 2020  display:flex;.  
-00002350: 2020 7d0a 0a20 2020 202e 7769 6467 6574    }..    .widget
-00002360: 2d6c 6162 656c 2d62 6173 6963 2069 6e70  -label-basic inp
-00002370: 7574 5b74 7970 653d 2763 6865 636b 626f  ut[type='checkbo
-00002380: 7827 5d5b 6469 7361 626c 6564 5d20 7b0a  x'][disabled] {.
-00002390: 2020 2020 2020 2020 6669 6c74 6572 3a20          filter: 
-000023a0: 7365 7069 6128 302e 3329 2068 7565 2d72  sepia(0.3) hue-r
-000023b0: 6f74 6174 6528 3637 6465 6729 2073 6174  otate(67deg) sat
-000023c0: 7572 6174 6528 3329 3b0a 2020 2020 7d0a  urate(3);.    }.
-000023d0: 0a20 2020 202e 7061 6765 7b0a 2020 2020  .    .page{.    
-000023e0: 2020 2020 636f 6c6f 723a 2062 6c61 636b      color: black
-000023f0: 3b0a 2020 2020 2020 2020 666f 6e74 2d77  ;.        font-w
-00002400: 6569 6768 743a 2062 6f6c 643b 0a20 2020  eight: bold;.   
-00002410: 2020 2020 2063 6f6c 6f72 3a20 7661 7228       color: var(
-00002420: 2d2d 7465 7274 6961 7279 2d63 6f6c 6f72  --tertiary-color
-00002430: 293b 0a20 2020 207d 0a20 2020 202e 7061  );.    }.    .pa
-00002440: 6765 3a68 6f76 6572 207b 0a20 2020 2020  ge:hover {.     
-00002450: 2063 6f6c 6f72 3a20 2333 3862 6466 383b   color: #38bdf8;
-00002460: 0a20 2020 2020 2063 7572 736f 723a 2070  .      cursor: p
-00002470: 6f69 6e74 6572 3b0a 2020 2020 7d0a 2020  ointer;.    }.  
-00002480: 2020 2e63 6c69 7062 6f61 7264 3a68 6f76    .clipboard:hov
-00002490: 6572 7b0a 2020 2020 2020 2020 6375 7273  er{.        curs
-000024a0: 6f72 3a20 706f 696e 7465 723b 0a20 2020  or: pointer;.   
-000024b0: 2020 2020 2063 6f6c 6f72 3a20 7661 7228       color: var(
-000024c0: 2d2d 7465 7274 6961 7279 2d63 6f6c 6f72  --tertiary-color
-000024d0: 293b 0a20 2020 207d 0a0a 2020 2020 2e73  );.    }..    .s
-000024e0: 6561 7263 682d 6669 656c 6420 7b0a 2020  earch-field {.  
-000024f0: 2020 2020 2020 6469 7370 6c61 793a 2066        display: f
-00002500: 6c65 783b 0a20 2020 2020 2020 2061 6c69  lex;.        ali
-00002510: 676e 2d69 7465 6d73 3a20 6365 6e74 6572  gn-items: center
-00002520: 3b0a 2020 2020 2020 2020 626f 7264 6572  ;.        border
-00002530: 2d72 6164 6975 733a 2033 3070 783b 0a20  -radius: 30px;. 
-00002540: 2020 2020 2020 2062 6163 6b67 726f 756e         backgroun
-00002550: 642d 636f 6c6f 723a 2076 6172 282d 2d73  d-color: var(--s
-00002560: 6563 6f6e 6461 7279 2d63 6f6c 6f72 293b  econdary-color);
-00002570: 0a20 2020 207d 0a0a 2020 2020 2e73 7966  .    }..    .syf
-00002580: 742d 6472 6f70 646f 776e 207b 0a20 2020  t-dropdown {.   
-00002590: 2020 2020 206d 6172 6769 6e3a 2035 7078       margin: 5px
-000025a0: 3b0a 2020 2020 2020 2020 6d61 7267 696e  ;.        margin
-000025b0: 2d6c 6566 743a 2035 7078 3b0a 2020 2020  -left: 5px;.    
-000025c0: 2020 2020 706f 7369 7469 6f6e 3a20 7265      position: re
-000025d0: 6c61 7469 7665 3b0a 2020 2020 2020 2020  lative;.        
-000025e0: 6469 7370 6c61 793a 2069 6e6c 696e 652d  display: inline-
-000025f0: 626c 6f63 6b3b 0a20 2020 2020 2020 2074  block;.        t
-00002600: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-00002610: 723b 0a20 2020 2020 2020 2062 6163 6b67  r;.        backg
-00002620: 726f 756e 642d 636f 6c6f 723a 2076 6172  round-color: var
-00002630: 282d 2d62 7574 746f 6e2d 636f 6c6f 7229  (--button-color)
-00002640: 3b0a 2020 2020 2020 2020 6d69 6e2d 7769  ;.        min-wi
-00002650: 6474 683a 2031 3030 7078 3b0a 2020 2020  dth: 100px;.    
-00002660: 2020 2020 7061 6464 696e 673a 2032 7078      padding: 2px
-00002670: 3b0a 2020 2020 2020 2020 626f 7264 6572  ;.        border
-00002680: 2d72 6164 6975 733a 2033 3070 783b 0a20  -radius: 30px;. 
-00002690: 2020 207d 0a0a 2020 2020 2e73 7966 742d     }..    .syft-
-000026a0: 6472 6f70 646f 776e 3a68 6f76 6572 207b  dropdown:hover {
-000026b0: 0a20 2020 2020 2020 2063 7572 736f 723a  .        cursor:
-000026c0: 2070 6f69 6e74 6572 3b0a 2020 2020 7d0a   pointer;.    }.
-000026d0: 2020 2020 2e73 7966 742d 6472 6f70 646f      .syft-dropdo
-000026e0: 776e 2d63 6f6e 7465 6e74 207b 0a20 2020  wn-content {.   
-000026f0: 2020 2020 206d 6172 6769 6e2d 746f 703a       margin-top:
-00002700: 3236 7078 3b0a 2020 2020 2020 2020 6469  26px;.        di
-00002710: 7370 6c61 793a 206e 6f6e 653b 0a20 2020  splay: none;.   
-00002720: 2020 2020 2070 6f73 6974 696f 6e3a 2061       position: a
-00002730: 6273 6f6c 7574 653b 0a20 2020 2020 2020  bsolute;.       
-00002740: 206d 696e 2d77 6964 7468 3a20 3130 3070   min-width: 100p
-00002750: 783b 0a20 2020 2020 2020 2062 6f78 2d73  x;.        box-s
-00002760: 6861 646f 773a 2030 7078 2038 7078 2031  hadow: 0px 8px 1
-00002770: 3670 7820 3070 7820 7267 6261 2830 2c30  6px 0px rgba(0,0
-00002780: 2c30 2c30 2e32 293b 0a20 2020 2020 2020  ,0,0.2);.       
-00002790: 2070 6164 6469 6e67 3a20 3132 7078 2036   padding: 12px 6
-000027a0: 7078 3b0a 2020 2020 2020 2020 7a2d 696e  px;.        z-in
-000027b0: 6465 783a 2031 3b0a 2020 2020 2020 2020  dex: 1;.        
-000027c0: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
-000027d0: 3a20 7661 7228 2d2d 7072 696d 6172 792d  : var(--primary-
-000027e0: 636f 6c6f 7229 3b0a 2020 2020 2020 2020  color);.        
-000027f0: 636f 6c6f 723a 2076 6172 282d 2d74 6572  color: var(--ter
-00002800: 7469 6172 792d 636f 6c6f 7229 3b0a 2020  tiary-color);.  
-00002810: 2020 7d0a 2020 2020 2e64 642d 6f70 7469    }.    .dd-opti
-00002820: 6f6e 7320 7b0a 2020 2020 2020 2020 7061  ons {.        pa
-00002830: 6464 696e 672d 746f 703a 2034 7078 3b0a  dding-top: 4px;.
-00002840: 2020 2020 7d0a 2020 2020 2e64 642d 6f70      }.    .dd-op
-00002850: 7469 6f6e 733a 6669 7273 742d 6f66 2d74  tions:first-of-t
-00002860: 7970 6520 7b0a 2020 2020 2020 2020 7061  ype {.        pa
-00002870: 6464 696e 672d 746f 703a 2030 7078 3b0a  dding-top: 0px;.
-00002880: 2020 2020 7d0a 0a20 2020 202e 6464 2d6f      }..    .dd-o
-00002890: 7074 696f 6e73 3a68 6f76 6572 207b 0a20  ptions:hover {. 
-000028a0: 2020 2020 2020 2063 7572 736f 723a 2070         cursor: p
-000028b0: 6f69 6e74 6572 3b0a 2020 2020 2020 2020  ointer;.        
-000028c0: 6261 636b 6772 6f75 6e64 3a20 2364 3164  background: #d1d
-000028d0: 3564 623b 0a20 2020 207d 0a20 2020 202e  5db;.    }.    .
-000028e0: 6172 726f 7720 7b0a 2020 2020 2020 2020  arrow {.        
-000028f0: 626f 7264 6572 3a20 736f 6c69 6420 626c  border: solid bl
-00002900: 6163 6b3b 0a20 2020 2020 2020 2062 6f72  ack;.        bor
-00002910: 6465 722d 7769 6474 683a 2030 2033 7078  der-width: 0 3px
-00002920: 2033 7078 2030 3b0a 2020 2020 2020 2020   3px 0;.        
-00002930: 6469 7370 6c61 793a 2069 6e6c 696e 652d  display: inline-
-00002940: 626c 6f63 6b3b 0a20 2020 2020 2020 2070  block;.        p
-00002950: 6164 6469 6e67 3a20 3370 783b 0a20 2020  adding: 3px;.   
-00002960: 207d 0a20 2020 202e 646f 776e 207b 0a20   }.    .down {. 
-00002970: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
-00002980: 3a20 726f 7461 7465 2834 3564 6567 293b  : rotate(45deg);
-00002990: 0a20 2020 2020 2020 202d 7765 626b 6974  .        -webkit
-000029a0: 2d74 7261 6e73 666f 726d 3a20 726f 7461  -transform: rota
-000029b0: 7465 2834 3564 6567 293b 0a20 2020 207d  te(45deg);.    }
-000029c0: 0a3c 2f73 7479 6c65 3e0a 0a22 2222 0a0a  .</style>.."""..
-000029d0: 5345 4152 4348 5f49 434f 4e20 3d20 280a  SEARCH_ICON = (.
-000029e0: 2020 2020 273c 7376 6720 7769 6474 683d      '<svg width=
-000029f0: 2231 3122 2068 6569 6768 743d 2231 3022  "11" height="10"
-00002a00: 2076 6965 7742 6f78 3d22 3020 3020 3131   viewBox="0 0 11
-00002a10: 2031 3022 2066 696c 6c3d 226e 6f6e 6522   10" fill="none"
-00002a20: 270a 2020 2020 2720 786d 6c6e 733d 2268  '.    ' xmlns="h
-00002a30: 7474 703a 2f2f 7777 772e 7733 2e6f 7267  ttp://www.w3.org
-00002a40: 2f32 3030 302f 7376 6722 3e3c 7061 7468  /2000/svg"><path
-00002a50: 2064 3d22 4d31 302e 3536 3532 2039 2e32   d="M10.5652 9.2
-00002a60: 3334 3637 4c38 2e32 3138 3139 270a 2020  3467L8.21819'.  
-00002a70: 2020 2220 362e 3838 3831 3143 382e 3839    " 6.88811C8.89
-00002a80: 3834 3620 362e 3037 3134 3120 392e 3233  846 6.07141 9.23
-00002a90: 3736 3720 352e 3032 3338 3920 392e 3136  767 5.02389 9.16
-00002aa0: 3532 3720 332e 3936 3334 3543 392e 3039  527 3.96345C9.09
-00002ab0: 3238 3720 322e 3930 3330 3220 382e 3631  287 2.90302 8.61
-00002ac0: 3434 3322 0a20 2020 2022 2031 2e39 3131  443".    " 1.911
-00002ad0: 3332 2037 2e38 3239 3438 2031 2e31 3934  32 7.82948 1.194
-00002ae0: 3636 4337 2e30 3434 3533 2030 2e34 3737  66C7.04453 0.477
-00002af0: 3939 3520 362e 3031 3334 3920 302e 3039  995 6.01349 0.09
-00002b00: 3135 3431 3420 342e 3935 3038 3722 0a20  15414 4.95087". 
-00002b10: 2020 2022 2030 2e31 3135 3639 3143 332e     " 0.115691C3.
-00002b20: 3838 3832 3420 302e 3133 3938 3431 2032  88824 0.139841 2
-00002b30: 2e38 3735 3833 2030 2e35 3732 3733 3520  .87583 0.572735 
-00002b40: 322e 3132 3432 3520 312e 3332 3433 3243  2.12425 1.32432C
-00002b50: 312e 3337 3236 3620 322e 3037 3539 220a  1.37266 2.0759".
-00002b60: 2020 2020 2220 302e 3933 3937 3638 2033      " 0.939768 3
-00002b70: 2e30 3838 3331 2030 2e39 3135 3631 3820  .08831 0.915618 
-00002b80: 342e 3135 3039 3443 302e 3839 3134 3638  4.15094C0.891468
-00002b90: 2035 2e32 3133 3537 2031 2e32 3737 3932   5.21357 1.27792
-00002ba0: 2036 2e32 3434 3620 312e 3939 3435 3922   6.2446 1.99459"
-00002bb0: 0a20 2020 2022 2037 2e30 3239 3535 4332  .    " 7.02955C2
-00002bc0: 2e37 3131 3235 2037 2e38 3134 3520 332e  .71125 7.8145 3.
-00002bd0: 3730 3239 3520 382e 3239 3239 3420 342e  70295 8.29294 4.
-00002be0: 3736 3333 3820 382e 3336 3533 3543 352e  76338 8.36535C5.
-00002bf0: 3832 3338 3120 382e 3433 3737 3520 362e  82381 8.43775 6.
-00002c00: 3837 3133 3422 0a20 2020 2022 2038 2e30  87134".    " 8.0
-00002c10: 3938 3533 2037 2e36 3838 3034 2037 2e34  9853 7.68804 7.4
-00002c20: 3138 3237 4c31 302e 3033 3436 2039 2e37  1827L10.0346 9.7
-00002c30: 3635 3343 3130 2e30 3639 3420 392e 3830  653C10.0694 9.80
-00002c40: 3031 3420 3130 2e31 3130 3820 392e 3832  014 10.1108 9.82
-00002c50: 3737 3820 3130 2e31 3536 3322 0a20 2020  778 10.1563".   
-00002c60: 2022 2039 2e38 3436 3633 4331 302e 3230   " 9.84663C10.20
-00002c70: 3138 2039 2e38 3635 3439 2031 302e 3235  18 9.86549 10.25
-00002c80: 3036 2039 2e38 3735 3139 2031 302e 3239  06 9.87519 10.29
-00002c90: 3939 2039 2e38 3735 3139 4331 302e 3334  99 9.87519C10.34
-00002ca0: 3932 2039 2e38 3735 3139 2031 302e 3339  92 9.87519 10.39
-00002cb0: 3822 0a20 2020 2022 2039 2e38 3635 3439  8".    " 9.86549
-00002cc0: 2031 302e 3434 3335 2039 2e38 3436 3633   10.4435 9.84663
-00002cd0: 4331 302e 3438 3920 392e 3832 3737 3820  C10.489 9.82778 
-00002ce0: 3130 2e35 3330 3420 392e 3830 3031 3420  10.5304 9.80014 
-00002cf0: 3130 2e35 3635 3220 392e 3736 3533 4331  10.5652 9.7653C1
-00002d00: 302e 3630 3031 220a 2020 2020 2220 392e  0.6001".    " 9.
-00002d10: 3733 3034 3620 3130 2e36 3237 3720 392e  73046 10.6277 9.
-00002d20: 3638 3930 3920 3130 2e36 3436 3620 392e  68909 10.6466 9.
-00002d30: 3634 3335 3743 3130 2e36 3635 3420 392e  64357C10.6654 9.
-00002d40: 3539 3830 3520 3130 2e36 3735 3120 392e  59805 10.6751 9.
-00002d50: 3534 3932 3620 3130 2e36 3735 3122 0a20  54926 10.6751". 
-00002d60: 2020 2022 2039 2e34 3939 3938 4331 302e     " 9.49998C10.
-00002d70: 3637 3531 2039 2e34 3530 3731 2031 302e  6751 9.45071 10.
-00002d80: 3636 3534 2039 2e34 3031 3932 2031 302e  6654 9.40192 10.
-00002d90: 3634 3636 2039 2e33 3536 3443 3130 2e36  6466 9.3564C10.6
-00002da0: 3237 3720 392e 3331 3038 3820 3130 2e36  277 9.31088 10.6
-00002db0: 3030 3122 0a20 2020 2022 2039 2e32 3639  001".    " 9.269
-00002dc0: 3531 2031 302e 3536 3532 2039 2e32 3334  51 10.5652 9.234
-00002dd0: 3637 5a4d 312e 3637 3439 3120 342e 3234  67ZM1.67491 4.24
-00002de0: 3939 3843 312e 3637 3439 3120 332e 3538  998C1.67491 3.58
-00002df0: 3234 3720 312e 3837 3238 3520 322e 3932  247 1.87285 2.92
-00002e00: 3939 3520 322e 3234 3337 220a 2020 2020  995 2.2437".    
-00002e10: 2220 322e 3337 3439 3343 322e 3631 3435  " 2.37493C2.6145
-00002e20: 3520 312e 3831 3939 3220 332e 3134 3136  5 1.81992 3.1416
-00002e30: 3520 312e 3338 3733 3420 332e 3735 3833  5 1.38734 3.7583
-00002e40: 3520 312e 3133 3138 3943 342e 3337 3530  5 1.13189C4.3750
-00002e50: 3620 302e 3837 3634 3436 2035 2e30 3533  6 0.876446 5.053
-00002e60: 3636 220a 2020 2020 2220 302e 3830 3936  66".    " 0.8096
-00002e70: 3039 2035 2e37 3038 3334 2030 2e39 3339  09 5.70834 0.939
-00002e80: 3833 3543 362e 3336 3330 3320 312e 3037  835C6.36303 1.07
-00002e90: 3030 3620 362e 3936 3433 3920 312e 3339  006 6.96439 1.39
-00002ea0: 3135 2037 2e34 3336 3420 312e 3836 3335  15 7.4364 1.8635
-00002eb0: 4337 2e39 3038 3422 0a20 2020 2022 2032  C7.9084".    " 2
-00002ec0: 2e33 3335 3520 382e 3232 3938 3420 322e  .3355 8.22984 2.
-00002ed0: 3933 3638 3720 382e 3336 3030 3620 332e  93687 8.36006 3.
-00002ee0: 3539 3135 3543 382e 3439 3032 3920 342e  59155C8.49029 4.
-00002ef0: 3234 3632 3420 382e 3432 3334 3520 342e  24624 8.42345 4.
-00002f00: 3932 3438 3420 382e 3136 3822 0a20 2020  92484 8.168".   
-00002f10: 2022 2035 2e35 3431 3534 4337 2e39 3132   " 5.54154C7.912
-00002f20: 3536 2036 2e31 3538 3234 2037 2e34 3739  56 6.15824 7.479
-00002f30: 3938 2036 2e36 3835 3335 2036 2e39 3234  98 6.68535 6.924
-00002f40: 3936 2037 2e30 3536 3139 4336 2e33 3639  96 7.05619C6.369
-00002f50: 3935 2037 2e34 3237 3034 2035 2e37 3137  95 7.42704 5.717
-00002f60: 3432 220a 2020 2020 2220 372e 3632 3439  42".    " 7.6249
-00002f70: 3820 352e 3034 3939 3120 372e 3632 3439  8 5.04991 7.6249
-00002f80: 3843 342e 3135 3531 3120 372e 3632 3339  8C4.15511 7.6239
-00002f90: 3920 332e 3239 3732 3420 372e 3236 3830  9 3.29724 7.2680
-00002fa0: 3920 322e 3636 3435 3220 362e 3633 3533  9 2.66452 6.6353
-00002fb0: 3743 322e 3033 3138 220a 2020 2020 2720  7C2.0318".    ' 
-00002fc0: 362e 3030 3236 3520 312e 3637 3539 2035  6.00265 1.6759 5
-00002fd0: 2e31 3434 3739 2031 2e36 3734 3931 2034  .14479 1.67491 4
-00002fe0: 2e32 3439 3938 5a22 2066 696c 6c3d 2263  .24998Z" fill="c
-00002ff0: 7572 7265 6e74 436f 6c6f 7222 2f3e 3c2f  urrentColor"/></
-00003000: 7376 673e 270a 290a 434c 4950 424f 4152  svg>'.).CLIPBOAR
-00003010: 445f 4943 4f4e 203d 2028 0a20 2020 2022  D_ICON = (.    "
-00003020: 3c73 7667 2077 6964 7468 3d27 3827 2068  <svg width='8' h
-00003030: 6569 6768 743d 2738 2720 7669 6577 426f  eight='8' viewBo
-00003040: 783d 2730 2030 2038 2038 2720 6669 6c6c  x='0 0 8 8' fill
-00003050: 3d27 6e6f 6e65 2722 0a20 2020 2022 2078  ='none'".    " x
-00003060: 6d6c 6e73 3d27 6874 7470 3a2f 2f77 7777  mlns='http://www
-00003070: 2e77 332e 6f72 672f 3230 3030 2f73 7667  .w3.org/2000/svg
-00003080: 273e 3c70 6174 6820 643d 274d 372e 3433  '><path d='M7.43
-00003090: 3735 2030 2e32 3548 322e 3433 3735 4332  75 0.25H2.4375C2
-000030a0: 2e33 3534 3632 2030 2e32 3522 0a20 2020  .35462 0.25".   
-000030b0: 2022 2032 2e32 3735 3133 2030 2e32 3832   " 2.27513 0.282
-000030c0: 3932 3420 322e 3231 3635 3320 302e 3334  924 2.21653 0.34
-000030d0: 3135 3239 4332 2e31 3537 3932 2030 2e34  1529C2.15792 0.4
-000030e0: 3030 3133 3420 322e 3132 3520 302e 3437  00134 2.125 0.47
-000030f0: 3936 3220 322e 3132 3522 0a20 2020 2022  962 2.125".    "
-00003100: 2030 2e35 3632 3556 322e 3132 3548 302e   0.5625V2.125H0.
-00003110: 3536 3235 4330 2e34 3739 3632 2032 2e31  5625C0.47962 2.1
-00003120: 3235 2030 2e34 3030 3133 3420 322e 3135  25 0.400134 2.15
-00003130: 3739 3220 302e 3334 3135 3239 2032 2e32  792 0.341529 2.2
-00003140: 3136 3533 4330 2e32 3832 3932 3422 0a20  1653C0.282924". 
-00003150: 2020 2022 2032 2e32 3735 3133 2030 2e32     " 2.27513 0.2
-00003160: 3520 322e 3335 3436 3220 302e 3235 2032  5 2.35462 0.25 2
-00003170: 2e34 3337 3556 372e 3433 3735 4330 2e32  .4375V7.4375C0.2
-00003180: 3520 372e 3532 3033 3820 302e 3238 3239  5 7.52038 0.2829
-00003190: 3234 2037 2e35 3939 3837 2030 2e33 3431  24 7.59987 0.341
-000031a0: 3532 3922 0a20 2020 2022 2037 2e36 3538  529".    " 7.658
-000031b0: 3437 4330 2e34 3030 3133 3420 372e 3731  47C0.400134 7.71
-000031c0: 3730 3820 302e 3437 3936 3220 372e 3735  708 0.47962 7.75
-000031d0: 2030 2e35 3632 3520 372e 3735 4835 2e35   0.5625 7.75H5.5
-000031e0: 3632 3543 352e 3634 3533 3820 372e 3735  625C5.64538 7.75
-000031f0: 2035 2e37 3234 3837 220a 2020 2020 2220   5.72487".    " 
-00003200: 372e 3731 3730 3820 352e 3738 3334 3720  7.71708 5.78347 
-00003210: 372e 3635 3834 3743 352e 3834 3230 3820  7.65847C5.84208 
-00003220: 372e 3539 3938 3720 352e 3837 3520 372e  7.59987 5.875 7.
-00003230: 3532 3033 3820 352e 3837 3522 0a20 2020  52038 5.875".   
-00003240: 2022 2037 2e34 3337 3556 352e 3837 3548   " 7.4375V5.875H
-00003250: 372e 3433 3735 4337 2e35 3230 3338 2035  7.4375C7.52038 5
-00003260: 2e38 3735 2037 2e35 3939 3837 2035 2e38  .875 7.59987 5.8
-00003270: 3432 3038 2037 2e36 3538 3437 2035 2e37  4208 7.65847 5.7
-00003280: 3833 3437 4337 2e37 3137 3038 2035 2e37  8347C7.71708 5.7
-00003290: 3234 3837 220a 2020 2020 2220 372e 3735  2487".    " 7.75
-000032a0: 2035 2e36 3435 3338 2037 2e37 3520 352e   5.64538 7.75 5.
-000032b0: 3536 3235 5630 2e35 3632 3543 372e 3735  5625V0.5625C7.75
-000032c0: 2030 2e34 3739 3632 2037 2e37 3137 3038   0.47962 7.71708
-000032d0: 2030 2e34 3030 3133 3420 372e 3635 3834   0.400134 7.6584
-000032e0: 3722 0a20 2020 2022 2030 2e33 3431 3532  7".    " 0.34152
-000032f0: 3943 372e 3539 3938 3720 302e 3238 3239  9C7.59987 0.2829
-00003300: 3234 2037 2e35 3230 3338 2030 2e32 3520  24 7.52038 0.25 
-00003310: 372e 3433 3735 2030 2e32 355a 4d35 2e32  7.4375 0.25ZM5.2
-00003320: 3522 0a20 2020 2022 2037 2e31 3235 4830  5".    " 7.125H0
-00003330: 2e38 3735 5632 2e37 3548 352e 3235 5637  .875V2.75H5.25V7
-00003340: 2e31 3235 5a4d 372e 3132 3520 352e 3235  .125ZM7.125 5.25
-00003350: 4835 2e38 3735 5632 2e34 3337 3543 352e  H5.875V2.4375C5.
-00003360: 3837 3520 322e 3335 3436 3220 352e 3834  875 2.35462 5.84
-00003370: 3230 3822 0a20 2020 2022 2032 2e32 3735  208".    " 2.275
-00003380: 3133 2035 2e37 3833 3437 2032 2e32 3136  13 5.78347 2.216
-00003390: 3533 4335 2e37 3234 3837 2032 2e31 3537  53C5.72487 2.157
-000033a0: 3932 2035 2e36 3435 3338 2032 2e31 3235  92 5.64538 2.125
-000033b0: 2035 2e35 3632 3522 0a20 2020 2022 2032   5.5625".    " 2
-000033c0: 2e31 3235 4832 2e37 3556 302e 3837 3548  .125H2.75V0.875H
-000033d0: 372e 3132 3556 352e 3235 5a27 2066 696c  7.125V5.25Z' fil
-000033e0: 6c3d 2723 3436 3431 3538 272f 3e3c 2f73  l='#464158'/></s
-000033f0: 7667 3e22 0a29 0a54 4142 4c45 5f49 434f  vg>".).TABLE_ICO
-00003400: 4e20 3d20 280a 2020 2020 273c 7376 6720  N = (.    '<svg 
-00003410: 7769 6474 683d 2233 3222 2068 6569 6768  width="32" heigh
-00003420: 743d 2233 3222 2076 6965 7742 6f78 3d22  t="32" viewBox="
-00003430: 3020 3020 3332 2033 3222 2066 696c 6c3d  0 0 32 32" fill=
-00003440: 226e 6f6e 6522 270a 2020 2020 2720 786d  "none"'.    ' xm
-00003450: 6c6e 733d 2268 7474 703a 2f2f 7777 772e  lns="http://www.
-00003460: 7733 2e6f 7267 2f32 3030 302f 7376 6722  w3.org/2000/svg"
-00003470: 3e20 3c70 6174 6820 643d 224d 3238 2036  > <path d="M28 6
-00003480: 4834 4333 2e37 3334 3738 2036 2033 2e34  H4C3.73478 6 3.4
-00003490: 3830 3433 2036 2e31 3035 3336 270a 2020  8043 6.10536'.  
-000034a0: 2020 2220 332e 3239 3238 3920 362e 3239    " 3.29289 6.29
-000034b0: 3238 3943 332e 3130 3533 3620 362e 3438  289C3.10536 6.48
-000034c0: 3034 3320 3320 362e 3733 3437 3820 3320  043 3 6.73478 3 
-000034d0: 3756 3234 4333 2032 342e 3533 3034 2033  7V24C3 24.5304 3
-000034e0: 2e32 3130 3731 2032 352e 3033 3931 220a  .21071 25.0391".
-000034f0: 2020 2020 2220 332e 3538 3537 3920 3235      " 3.58579 25
-00003500: 2e34 3134 3243 332e 3936 3038 3620 3235  .4142C3.96086 25
-00003510: 2e37 3839 3320 342e 3436 3935 3720 3236  .7893 4.46957 26
-00003520: 2035 2032 3648 3237 4332 372e 3533 3034   5 26H27C27.5304
-00003530: 2032 3620 3238 2e30 3339 3120 3235 2e37   26 28.0391 25.7
-00003540: 3839 3322 0a20 2020 2022 2032 382e 3431  893".    " 28.41
-00003550: 3432 2032 352e 3431 3432 4332 382e 3738  42 25.4142C28.78
-00003560: 3933 2032 352e 3033 3931 2032 3920 3234  93 25.0391 29 24
-00003570: 2e35 3330 3420 3239 2032 3456 3743 3239  .5304 29 24V7C29
-00003580: 2036 2e37 3334 3738 2032 382e 3839 3436   6.73478 28.8946
-00003590: 2036 2e34 3830 3433 220a 2020 2020 2220   6.48043".    " 
-000035a0: 3238 2e37 3037 3120 362e 3239 3238 3943  28.7071 6.29289C
-000035b0: 3238 2e35 3139 3620 362e 3130 3533 3620  28.5196 6.10536 
-000035c0: 3238 2e32 3635 3220 3620 3238 2036 5a4d  28.2652 6 28 6ZM
-000035d0: 3520 3134 4831 3056 3138 4835 5631 345a  5 14H10V18H5V14Z
-000035e0: 4d31 3222 0a20 2020 2027 2031 3448 3237  M12".    ' 14H27
-000035f0: 5631 3848 3132 5631 345a 4d32 3720 3856  V18H12V14ZM27 8V
-00003600: 3132 4835 5638 4832 375a 4d35 2032 3048  12H5V8H27ZM5 20H
-00003610: 3130 5632 3448 3556 3230 5a4d 3237 2032  10V24H5V20ZM27 2
-00003620: 3448 3132 5632 3048 3237 5632 345a 2227  4H12V20H27V24Z"'
-00003630: 0a20 2020 2027 2066 696c 6c3d 2223 3334  .    ' fill="#34
-00003640: 3333 3330 222f 3e3c 2f73 7667 3e27 0a29  3330"/></svg>'.)
-00003650: 0a46 4f4c 4445 525f 4943 4f4e 203d 2028  .FOLDER_ICON = (
-00003660: 0a20 2020 2027 3c73 7667 2077 6964 7468  .    '<svg width
-00003670: 3d22 3332 2220 2068 6569 6768 743d 2233  ="32"  height="3
-00003680: 3222 2076 6965 7742 6f78 3d22 3020 3020  2" viewBox="0 0 
-00003690: 3134 2031 3222 2066 696c 6c3d 226e 6f6e  14 12" fill="non
-000036a0: 6522 270a 2020 2020 2720 786d 6c6e 733d  e"'.    ' xmlns=
-000036b0: 2268 7474 703a 2f2f 7777 772e 7733 2e6f  "http://www.w3.o
-000036c0: 7267 2f32 3030 302f 7376 6722 3e3c 7061  rg/2000/svg"><pa
-000036d0: 7468 2064 3d22 4d31 3320 3248 382e 3636  th d="M13 2H8.66
-000036e0: 3638 374c 362e 3933 3331 3320 302e 3743  687L6.93313 0.7C
-000036f0: 362e 3735 3937 3827 0a20 2020 2022 2030  6.75978'.    " 0
-00003700: 2e35 3730 3636 2036 2e35 3439 3431 2030  .57066 6.54941 0
-00003710: 2e35 3030 3533 3620 362e 3333 3331 3320  .500536 6.33313 
-00003720: 302e 3548 332e 3543 332e 3233 3437 3820  0.5H3.5C3.23478 
-00003730: 302e 3520 322e 3938 3034 3320 302e 3630  0.5 2.98043 0.60
-00003740: 3533 3537 2032 2e37 3932 3839 220a 2020  5357 2.79289".  
-00003750: 2020 2220 302e 3739 3238 3933 4332 2e36    " 0.792893C2.6
-00003760: 3035 3336 2030 2e39 3830 3433 2032 2e35  0536 0.98043 2.5
-00003770: 2031 2e32 3334 3738 2032 2e35 2031 2e35   1.23478 2.5 1.5
-00003780: 5632 2e35 4831 2e35 4331 2e32 3334 3738  V2.5H1.5C1.23478
-00003790: 2032 2e35 2030 2e39 3830 3433 2032 2e36   2.5 0.98043 2.6
-000037a0: 3035 3336 220a 2020 2020 2220 302e 3739  0536".    " 0.79
-000037b0: 3238 3933 2032 2e37 3932 3839 4330 2e36  2893 2.79289C0.6
-000037c0: 3035 3335 3720 322e 3938 3034 3320 302e  05357 2.98043 0.
-000037d0: 3520 332e 3233 3437 3820 302e 3520 332e  5 3.23478 0.5 3.
-000037e0: 3556 3130 2e35 4330 2e35 2031 302e 3736  5V10.5C0.5 10.76
-000037f0: 3532 2030 2e36 3035 3335 3722 0a20 2020  52 0.605357".   
-00003800: 2022 2031 312e 3031 3936 2030 2e37 3932   " 11.0196 0.792
-00003810: 3839 3320 3131 2e32 3037 3143 302e 3938  893 11.2071C0.98
-00003820: 3034 3320 3131 2e33 3934 3620 312e 3233  043 11.3946 1.23
-00003830: 3437 3820 3131 2e35 2031 2e35 2031 312e  478 11.5 1.5 11.
-00003840: 3548 3131 2e30 3535 3643 3131 2e33 3036  5H11.0556C11.306
-00003850: 220a 2020 2020 2220 3131 2e34 3939 3720  ".    " 11.4997 
-00003860: 3131 2e35 3436 2031 312e 3430 3031 2031  11.546 11.4001 1
-00003870: 312e 3732 3320 3131 2e32 3233 4331 312e  1.723 11.223C11.
-00003880: 3930 3031 2031 312e 3034 3620 3131 2e39  9001 11.046 11.9
-00003890: 3939 3720 3130 2e38 3036 2031 3222 0a20  997 10.806 12". 
-000038a0: 2020 2022 2031 302e 3535 3536 5639 2e35     " 10.5556V9.5
-000038b0: 4831 332e 3035 3536 4331 332e 3330 3620  H13.0556C13.306 
-000038c0: 392e 3439 3936 3720 3133 2e35 3436 2039  9.49967 13.546 9
-000038d0: 2e34 3030 3037 2031 332e 3732 3320 392e  .40007 13.723 9.
-000038e0: 3232 3330 3343 3133 2e39 3030 3120 392e  22303C13.9001 9.
-000038f0: 3034 3622 0a20 2020 2022 2031 332e 3939  046".    " 13.99
-00003900: 3937 2038 2e38 3035 3939 2031 3420 382e  97 8.80599 14 8.
-00003910: 3535 3536 3256 3343 3134 2032 2e37 3334  55562V3C14 2.734
-00003920: 3738 2031 332e 3839 3436 2032 2e34 3830  78 13.8946 2.480
-00003930: 3433 2031 332e 3730 3731 2032 2e32 3932  43 13.7071 2.292
-00003940: 3839 4331 332e 3531 3936 220a 2020 2020  89C13.5196".    
-00003950: 2220 322e 3130 3533 3620 3133 2e32 3635  " 2.10536 13.265
-00003960: 3220 3220 3133 2032 5a4d 3131 2031 302e  2 2 13 2ZM11 10.
-00003970: 3548 312e 3556 332e 3548 342e 3333 3331  5H1.5V3.5H4.3331
-00003980: 334c 362e 3036 3638 3720 342e 3843 362e  3L6.06687 4.8C6.
-00003990: 3234 3032 3220 342e 3932 3933 3422 0a20  24022 4.92934". 
-000039a0: 2020 2022 2036 2e34 3530 3539 2034 2e39     " 6.45059 4.9
-000039b0: 3939 3436 2036 2e36 3636 3837 2035 4831  9946 6.66687 5H1
-000039c0: 3156 3130 2e35 5a4d 3133 2038 2e35 4831  1V10.5ZM13 8.5H1
-000039d0: 3256 3543 3132 2034 2e37 3334 3738 2031  2V5C12 4.73478 1
-000039e0: 312e 3839 3436 2034 2e34 3830 3433 2031  1.8946 4.48043 1
-000039f0: 312e 3730 3731 220a 2020 2020 2220 342e  1.7071".    " 4.
-00003a00: 3239 3238 3943 3131 2e35 3139 3620 342e  29289C11.5196 4.
-00003a10: 3130 3533 3620 3131 2e32 3635 3220 3420  10536 11.2652 4 
-00003a20: 3131 2034 4836 2e36 3636 3837 4c34 2e39  11 4H6.66687L4.9
-00003a30: 3333 3133 2032 2e37 4334 2e37 3539 3738  3313 2.7C4.75978
-00003a40: 2032 2e35 3730 3636 220a 2020 2020 2220   2.57066".    " 
-00003a50: 342e 3534 3934 3120 322e 3530 3035 3420  4.54941 2.50054 
-00003a60: 342e 3333 3331 3320 322e 3548 332e 3556  4.33313 2.5H3.5V
-00003a70: 312e 3548 362e 3333 3331 334c 382e 3036  1.5H6.33313L8.06
-00003a80: 3638 3820 322e 3843 382e 3234 3032 3220  688 2.8C8.24022 
-00003a90: 322e 3932 3933 3420 382e 3435 3035 3922  2.92934 8.45059"
-00003aa0: 0a20 2020 2027 2032 2e39 3939 3436 2038  .    ' 2.99946 8
-00003ab0: 2e36 3636 3837 2033 4831 3356 382e 355a  .66687 3H13V8.5Z
-00003ac0: 2220 6669 6c6c 3d22 6375 7272 656e 7443  " fill="currentC
-00003ad0: 6f6c 6f72 222f 3e3c 2f73 7667 3e27 0a29  olor"/></svg>'.)
-00003ae0: 0a52 4551 5545 5354 5f49 434f 4e20 3d20  .REQUEST_ICON = 
-00003af0: 280a 2020 2020 273c 7376 6720 7769 6474  (.    '<svg widt
-00003b00: 683d 2233 3222 2020 6865 6967 6874 3d22  h="32"  height="
-00003b10: 3332 2220 7669 6577 426f 783d 2230 2030  32" viewBox="0 0
-00003b20: 2031 3220 3132 2220 6669 6c6c 3d22 6e6f   12 12" fill="no
-00003b30: 6e65 2227 0a20 2020 2027 2078 6d6c 6e73  ne"'.    ' xmlns
-00003b40: 3d22 6874 7470 3a2f 2f77 7777 2e77 332e  ="http://www.w3.
-00003b50: 6f72 672f 3230 3030 2f73 7667 223e 3c70  org/2000/svg"><p
-00003b60: 6174 6820 643d 224d 3131 2030 4831 4330  ath d="M11 0H1C0
-00003b70: 2e37 3334 3738 3420 3020 302e 3438 3034  .734784 0 0.4804
-00003b80: 3320 302e 3130 3533 3537 270a 2020 2020  3 0.105357'.    
-00003b90: 2220 302e 3239 3238 3933 2030 2e32 3932  " 0.292893 0.292
-00003ba0: 3839 3343 302e 3130 3533 3537 2030 2e34  893C0.105357 0.4
-00003bb0: 3830 3433 2030 2030 2e37 3334 3738 3420  8043 0 0.734784 
-00003bc0: 3020 3156 3131 4330 2031 312e 3236 3532  0 1V11C0 11.2652
-00003bd0: 2030 2e31 3035 3335 3720 3131 2e35 3139   0.105357 11.519
-00003be0: 3622 0a20 2020 2022 2030 2e32 3932 3839  6".    " 0.29289
-00003bf0: 3320 3131 2e37 3037 3143 302e 3438 3034  3 11.7071C0.4804
-00003c00: 3320 3131 2e38 3934 3620 302e 3733 3437  3 11.8946 0.7347
-00003c10: 3834 2031 3220 3120 3132 4831 3143 3131  84 12 1 12H11C11
-00003c20: 2e32 3635 3220 3132 2031 312e 3531 3936  .2652 12 11.5196
-00003c30: 2031 312e 3839 3436 220a 2020 2020 2220   11.8946".    " 
-00003c40: 3131 2e37 3037 3120 3131 2e37 3037 3143  11.7071 11.7071C
-00003c50: 3131 2e38 3934 3620 3131 2e35 3139 3620  11.8946 11.5196 
-00003c60: 3132 2031 312e 3236 3532 2031 3220 3131  12 11.2652 12 11
-00003c70: 5631 4331 3220 302e 3733 3437 3834 2031  V1C12 0.734784 1
-00003c80: 312e 3839 3436 2030 2e34 3830 3433 220a  1.8946 0.48043".
-00003c90: 2020 2020 2220 3131 2e37 3037 3120 302e      " 11.7071 0.
-00003ca0: 3239 3238 3933 4331 312e 3531 3936 2030  292893C11.5196 0
-00003cb0: 2e31 3035 3335 3720 3131 2e32 3635 3220  .105357 11.2652 
-00003cc0: 3020 3131 2030 5a4d 3131 2031 5637 2e35  0 11 0ZM11 1V7.5
-00003cd0: 4839 2e32 3036 3235 4339 2e30 3734 3939  H9.20625C9.07499
-00003ce0: 220a 2020 2020 2220 372e 3439 3936 3620  ".    " 7.49966 
-00003cf0: 382e 3934 3439 3620 372e 3532 3534 2038  8.94496 7.5254 8
-00003d00: 2e38 3233 3732 2037 2e35 3735 3732 4338  .82372 7.57572C8
-00003d10: 2e37 3032 3438 2037 2e36 3236 3034 2038  .70248 7.62604 8
-00003d20: 2e35 3932 3435 2037 2e36 3939 3934 2038  .59245 7.69994 8
-00003d30: 2e35 220a 2020 2020 2220 372e 3739 3331  .5".    " 7.7931
-00003d40: 334c 372e 3239 3331 3320 3948 342e 3730  3L7.29313 9H4.70
-00003d50: 3638 374c 332e 3520 372e 3739 3331 3343  687L3.5 7.79313C
-00003d60: 332e 3430 3734 3820 372e 3639 3938 3620  3.40748 7.69986 
-00003d70: 332e 3239 3733 3420 372e 3632 3539 3220  3.29734 7.62592 
-00003d80: 332e 3137 3539 3922 0a20 2020 2022 2037  3.17599".    " 7
-00003d90: 2e35 3735 3643 332e 3035 3436 3420 372e  .5756C3.05464 7.
-00003da0: 3532 3532 3820 322e 3932 3435 2037 2e34  52528 2.9245 7.4
-00003db0: 3939 3538 2032 2e37 3933 3133 2037 2e35  9958 2.79313 7.5
-00003dc0: 4831 5631 4831 315a 4d31 3120 3131 4831  H1V1H11ZM11 11H1
-00003dd0: 5638 2e35 4832 2e37 3933 3133 4c34 220a  V8.5H2.79313L4".
-00003de0: 2020 2020 2220 392e 3730 3638 3743 342e      " 9.70687C4.
-00003df0: 3039 3235 3220 392e 3830 3031 3420 342e  09252 9.80014 4.
-00003e00: 3230 3236 3620 392e 3837 3430 3820 342e  20266 9.87408 4.
-00003e10: 3332 3430 3120 392e 3932 3434 4334 2e34  32401 9.9244C4.4
-00003e20: 3435 3336 2039 2e39 3734 3732 2034 2e35  4536 9.97472 4.5
-00003e30: 3735 3522 0a20 2020 2022 2031 302e 3030  755".    " 10.00
-00003e40: 3034 2034 2e37 3036 3837 2031 3048 372e  04 4.70687 10H7.
-00003e50: 3239 3331 3343 372e 3432 3435 2031 302e  29313C7.4245 10.
-00003e60: 3030 3034 2037 2e35 3534 3634 2039 2e39  0004 7.55464 9.9
-00003e70: 3734 3732 2037 2e36 3735 3939 2039 2e39  7472 7.67599 9.9
-00003e80: 3234 3443 372e 3739 3733 3422 0a20 2020  244C7.79734".   
-00003e90: 2027 2039 2e38 3734 3038 2037 2e39 3037   ' 9.87408 7.907
-00003ea0: 3438 2039 2e38 3030 3134 2038 2039 2e37  48 9.80014 8 9.7
-00003eb0: 3036 3837 4c39 2e32 3036 3837 2038 2e35  0687L9.20687 8.5
-00003ec0: 4831 3156 3131 5a22 2066 696c 6c3d 2223  H11V11Z" fill="#
-00003ed0: 3334 3333 3330 222f 3e3c 2f73 7667 3e27  343330"/></svg>'
-00003ee0: 0a29 0a0a 4152 524f 575f 4943 4f4e 203d  .)..ARROW_ICON =
-00003ef0: 2028 0a20 2020 2027 3c73 7667 2077 6964   (.    '<svg wid
-00003f00: 7468 3d22 3234 2220 6865 6967 6874 3d22  th="24" height="
-00003f10: 3234 2220 7669 6577 426f 783d 2230 2030  24" viewBox="0 0
-00003f20: 2032 3420 3234 2220 6669 6c6c 3d22 6e6f   24 24" fill="no
-00003f30: 6e65 2220 786d 6c6e 733d 2268 7474 703a  ne" xmlns="http:
-00003f40: 2f2f 7777 772e 7733 2e6f 7267 2f32 3030  //www.w3.org/200
-00003f50: 302f 7376 6722 3e27 0a20 2020 2027 3c72  0/svg">'.    '<r
-00003f60: 6563 7420 783d 2230 2e35 2220 793d 2230  ect x="0.5" y="0
-00003f70: 2e35 2220 7769 6474 683d 2232 3322 2068  .5" width="23" h
-00003f80: 6569 6768 743d 2232 3322 2072 783d 2231  eight="23" rx="1
-00003f90: 2e35 2220 6669 6c6c 3d22 2345 4345 4245  .5" fill="#ECEBE
-00003fa0: 4622 2f3e 270a 2020 2020 273c 7265 6374  F"/>'.    '<rect
-00003fb0: 2078 3d22 302e 3522 2079 3d22 302e 3522   x="0.5" y="0.5"
-00003fc0: 2077 6964 7468 3d22 3233 2220 6865 6967   width="23" heig
-00003fd0: 6874 3d22 3233 2220 7278 3d22 312e 3522  ht="23" rx="1.5"
-00003fe0: 2073 7472 6f6b 653d 2223 4234 4230 4246   stroke="#B4B0BF
-00003ff0: 222f 3e27 0a20 2020 2027 3c70 6174 6820  "/>'.    '<path 
-00004000: 643d 224d 3137 2e38 3533 3820 3132 2e33  d="M17.8538 12.3
-00004010: 3533 384c 3133 2e33 3533 3820 3136 2e38  538L13.3538 16.8
-00004020: 3533 3843 3133 2e32 3539 3920 3136 2e39  538C13.2599 16.9
-00004030: 3437 3620 3133 2e31 3332 3720 3137 2e30  476 13.1327 17.0
-00004040: 3030 3320 3133 2031 372e 3030 3033 4331  003 13 17.0003C1
-00004050: 322e 3836 3733 2031 372e 3030 3033 2031  2.8673 17.0003 1
-00004060: 322e 3734 3031 2031 362e 3934 3736 2031  2.7401 16.9476 1
-00004070: 322e 3634 3632 2031 362e 3835 3338 4331  2.6462 16.8538C1
-00004080: 322e 3535 3234 2031 362e 3736 2031 322e  2.5524 16.76 12.
-00004090: 3439 3937 2031 362e 3633 3237 2031 322e  4997 16.6327 12.
-000040a0: 3439 3937 2031 362e 3543 3132 2e34 3939  4997 16.5C12.499
-000040b0: 3720 3136 2e33 3637 3420 3132 2e35 3532  7 16.3674 12.552
-000040c0: 3420 3136 2e32 3430 3120 3132 2e36 3436  4 16.2401 12.646
-000040d0: 3220 3136 2e31 3436 334c 3136 2e32 3933  2 16.1463L16.293
-000040e0: 3120 3132 2e35 4836 2e35 4336 2e33 3637  1 12.5H6.5C6.367
-000040f0: 3339 2031 322e 3520 362e 3234 3032 3120  39 12.5 6.24021 
-00004100: 3132 2e34 3437 3420 362e 3134 3634 3520  12.4474 6.14645 
-00004110: 3132 2e33 3533 3643 362e 3035 3236 3820  12.3536C6.05268 
-00004120: 3132 2e32 3539 3820 3620 3132 2e31 3332  12.2598 6 12.132
-00004130: 3620 3620 3132 4336 2031 312e 3836 3734  6 6 12C6 11.8674
-00004140: 2036 2e30 3532 3638 2031 312e 3734 3032   6.05268 11.7402
-00004150: 2036 2e31 3436 3435 2031 312e 3634 3635   6.14645 11.6465
-00004160: 4336 2e32 3430 3231 2031 312e 3535 3237  C6.24021 11.5527
-00004170: 2036 2e33 3637 3339 2031 312e 3520 362e   6.36739 11.5 6.
-00004180: 3520 3131 2e35 4831 362e 3239 3331 4c31  5 11.5H16.2931L1
-00004190: 322e 3634 3632 2037 2e38 3533 3738 4331  2.6462 7.85378C1
-000041a0: 322e 3535 3234 2037 2e37 3539 3936 2031  2.5524 7.75996 1
-000041b0: 322e 3439 3937 2037 2e36 3332 3732 2031  2.4997 7.63272 1
-000041c0: 322e 3439 3937 2037 2e35 3030 3033 4331  2.4997 7.50003C1
-000041d0: 322e 3439 3937 2037 2e33 3637 3335 2031  2.4997 7.36735 1
-000041e0: 322e 3535 3234 2037 2e32 3430 3120 3132  2.5524 7.2401 12
-000041f0: 2e36 3436 3220 372e 3134 3632 3843 3132  .6462 7.14628C12
-00004200: 2e37 3430 3120 372e 3035 3234 3620 3132  .7401 7.05246 12
-00004210: 2e38 3637 3320 362e 3939 3937 3620 3133  .8673 6.99976 13
-00004220: 2036 2e39 3939 3736 4331 332e 3133 3237   6.99976C13.1327
-00004230: 2036 2e39 3939 3736 2031 332e 3235 3939   6.99976 13.2599
-00004240: 2037 2e30 3532 3436 2031 332e 3335 3338   7.05246 13.3538
-00004250: 2037 2e31 3436 3238 4c31 372e 3835 3338   7.14628L17.8538
-00004260: 2031 312e 3634 3633 4331 372e 3930 3032   11.6463C17.9002
-00004270: 2031 312e 3639 3237 2031 372e 3933 3731   11.6927 17.9371
-00004280: 2031 312e 3734 3739 2031 372e 3936 3233   11.7479 17.9623
-00004290: 2031 312e 3830 3836 4331 372e 3938 3734   11.8086C17.9874
-000042a0: 2031 312e 3836 3933 2031 382e 3030 3034   11.8693 18.0004
-000042b0: 2031 312e 3933 3433 2031 382e 3030 3034   11.9343 18.0004
-000042c0: 2031 3243 3138 2e30 3030 3420 3132 2e30   12C18.0004 12.0
-000042d0: 3635 3720 3137 2e39 3837 3420 3132 2e31  657 17.9874 12.1
-000042e0: 3330 3820 3137 2e39 3632 3320 3132 2e31  308 17.9623 12.1
-000042f0: 3931 3543 3137 2e39 3337 3120 3132 2e32  915C17.9371 12.2
-00004300: 3532 3220 3137 2e39 3030 3220 3132 2e33  522 17.9002 12.3
-00004310: 3037 3320 3137 2e38 3533 3820 3132 2e33  073 17.8538 12.3
-00004320: 3533 385a 2220 6669 6c6c 3d22 2335 4535  538Z" fill="#5E5
-00004330: 4137 3222 2f3e 3c2f 7376 673e 2720 2023  A72"/></svg>'  #
-00004340: 206e 6f71 613a 2045 3530 310a 290a 0a0a   noqa: E501.)...
-00004350: 6375 7374 6f6d 5f63 6f64 6520 3d20 2222  custom_code = ""
-00004360: 220a 2020 2020 3c64 6976 2073 7479 6c65  ".    <div style
-00004370: 3d27 6d61 7267 696e 2d74 6f70 3a31 3570  ='margin-top:15p
-00004380: 783b 273e 0a20 2020 2020 2020 203c 6469  x;'>.        <di
-00004390: 7620 636c 6173 733d 2766 6c65 7820 6761  v class='flex ga
-000043a0: 702d 3130 2720 7374 796c 653d 2761 6c69  p-10' style='ali
-000043b0: 676e 2d69 7465 6d73 3a20 6365 6e74 6572  gn-items: center
-000043c0: 3b27 3e0a 2020 2020 2020 2020 2020 2020  ;'>.            
-000043d0: 3c64 6976 2063 6c61 7373 3d27 666f 6c64  <div class='fold
-000043e0: 6572 2d69 636f 6e27 3e24 7b69 636f 6e7d  er-icon'>${icon}
-000043f0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00004400: 2020 203c 6469 763e 3c70 2063 6c61 7373     <div><p class
-00004410: 3d27 6865 6164 6572 2d33 273e 247b 6c69  ='header-3'>${li
-00004420: 7374 5f6e 616d 657d 3c2f 703e 3c2f 6469  st_name}</p></di
-00004430: 763e 0a20 2020 2020 2020 203c 2f64 6976  v>.        </div
-00004440: 3e0a 0a20 2020 2020 2020 2020 2020 203c  >..            <
-00004450: 6469 7620 7374 796c 653d 2270 6164 6469  div style="paddi
-00004460: 6e67 2d74 6f70 3a20 3136 7078 3b20 6469  ng-top: 16px; di
-00004470: 7370 6c61 793a 666c 6578 3b6a 7573 7469  splay:flex;justi
-00004480: 6679 2d63 6f6e 7465 6e74 3a20 7370 6163  fy-content: spac
-00004490: 652d 6265 7477 6565 6e3b 2061 6c69 676e  e-between; align
-000044a0: 2d69 7465 6d73 3a20 6365 6e74 6572 3b22  -items: center;"
-000044b0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000044c0: 2020 3c64 6976 2063 6c61 7373 3d27 7074    <div class='pt
-000044d0: 2d32 3520 6761 702d 3130 2720 7374 796c  -25 gap-10' styl
-000044e0: 653d 2264 6973 706c 6179 3a66 6c65 783b  e="display:flex;
-000044f0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00004500: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00004510: 733d 2273 6561 7263 682d 6669 656c 6422  s="search-field"
-00004520: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00004530: 2020 2020 2020 2020 2020 3c64 6976 2069            <div i
-00004540: 643d 2773 6561 7263 682d 6d65 6e75 247b  d='search-menu${
-00004550: 7569 647d 2720 636c 6173 733d 2273 7966  uid}' class="syf
-00004560: 742d 6472 6f70 646f 776e 2220 6f6e 636c  t-dropdown" oncl
-00004570: 6963 6b3d 227b 0a20 2020 2020 2020 2020  ick="{.         
-00004580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004590: 2020 206c 6574 2064 6f63 203d 2064 6f63     let doc = doc
-000045a0: 756d 656e 742e 6765 7445 6c65 6d65 6e74  ument.getElement
-000045b0: 4279 4964 2827 7365 6172 6368 2d64 726f  ById('search-dro
-000045c0: 7064 6f77 6e2d 636f 6e74 656e 7424 7b75  pdown-content${u
-000045d0: 6964 7d27 290a 2020 2020 2020 2020 2020  id}').          
-000045e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045f0: 2020 6966 2028 646f 632e 7374 796c 652e    if (doc.style.
-00004600: 6469 7370 6c61 7920 3d3d 3d20 2762 6c6f  display === 'blo
-00004610: 636b 2729 7b0a 2020 2020 2020 2020 2020  ck'){.          
-00004620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004630: 2020 2020 2020 646f 632e 7374 796c 652e        doc.style.
-00004640: 6469 7370 6c61 7920 3d20 276e 6f6e 6527  display = 'none'
-00004650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004660: 2020 2020 2020 2020 2020 2020 207d 2065               } e
-00004670: 6c73 6520 7b0a 2020 2020 2020 2020 2020  lse {.          
-00004680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004690: 2020 2020 2020 646f 632e 7374 796c 652e        doc.style.
-000046a0: 6469 7370 6c61 7920 3d20 2762 6c6f 636b  display = 'block
-000046b0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-000046c0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-000046d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046e0: 2020 2020 2020 2020 2020 2020 7d22 3e0a              }">.
-000046f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004700: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00004710: 2069 643d 2773 6561 7263 682d 6472 6f70   id='search-drop
-00004720: 646f 776e 2d63 6f6e 7465 6e74 247b 7569  down-content${ui
-00004730: 647d 2720 636c 6173 733d 2773 7966 742d  d}' class='syft-
-00004740: 6472 6f70 646f 776e 2d63 6f6e 7465 6e74  dropdown-content
-00004750: 273e 3c2f 6469 763e 0a20 2020 2020 2020  '></div>.       
-00004760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004770: 2020 2020 203c 7363 7269 7074 3e0a 2020       <script>.  
-00004780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004790: 2020 2020 2020 2020 2020 2020 2020 7661                va
-000047a0: 7220 656c 656d 656e 7424 7b75 6964 7d20  r element${uid} 
-000047b0: 3d20 247b 656c 656d 656e 747d 0a20 2020  = ${element}.   
-000047c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047d0: 2020 2020 2020 2020 2020 2020 2076 6172               var
-000047e0: 2070 6167 655f 7369 7a65 247b 7569 647d   page_size${uid}
-000047f0: 203d 2024 7b72 6f77 737d 0a20 2020 2020   = ${rows}.     
-00004800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004810: 2020 2020 2020 2020 2020 2076 6172 2070             var p
-00004820: 6167 6549 6e64 6578 247b 7569 647d 203d  ageIndex${uid} =
-00004830: 2031 0a20 2020 2020 2020 2020 2020 2020   1.             
-00004840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004850: 2020 2076 6172 2070 6167 696e 6174 6564     var paginated
-00004860: 456c 656d 656e 7473 247b 7569 647d 203d  Elements${uid} =
-00004870: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
-00004880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004890: 2020 2020 7661 7220 6163 7469 7665 4669      var activeFi
-000048a0: 6c74 6572 247b 7569 647d 3b0a 0a20 2020  lter${uid};..   
-000048b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048c0: 2020 2020 2020 2020 2020 2020 2066 756e               fun
-000048d0: 6374 696f 6e20 6275 696c 6444 726f 7044  ction buildDropD
-000048e0: 6f77 6e4d 656e 7528 656c 656d 656e 7473  ownMenu(elements
-000048f0: 297b 0a20 2020 2020 2020 2020 2020 2020  ){.             
-00004900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004910: 2020 2020 2020 206c 6574 2069 6e69 745f         let init_
-00004920: 6669 6c74 6572 3b0a 2020 2020 2020 2020  filter;.        
-00004930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004940: 2020 2020 2020 2020 2020 2020 6c65 7420              let 
-00004950: 6d65 6e75 203d 2064 6f63 756d 656e 742e  menu = document.
-00004960: 6765 7445 6c65 6d65 6e74 4279 4964 2827  getElementById('
-00004970: 7365 6172 6368 2d64 726f 7064 6f77 6e2d  search-dropdown-
-00004980: 636f 6e74 656e 7424 7b75 6964 7d27 290a  content${uid}').
-00004990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049b0: 2020 2020 6966 2028 656c 656d 656e 7473      if (elements
-000049c0: 2e6c 656e 6774 6820 3e20 3029 207b 0a20  .length > 0) {. 
-000049d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049f0: 2020 2020 2020 206c 6574 2073 616d 706c         let sampl
-00004a00: 6520 3d20 656c 656d 656e 7473 5b30 5d0a  e = elements[0].
-00004a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a30: 2020 2020 2020 2020 666f 7220 2863 6f6e          for (con
-00004a40: 7374 2061 7474 7220 696e 2073 616d 706c  st attr in sampl
-00004a50: 6529 207b 0a20 2020 2020 2020 2020 2020  e) {.           
-00004a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a80: 2069 6620 2874 7970 656f 6620 696e 6974   if (typeof init
-00004a90: 5f66 696c 7465 7220 3d3d 3d20 2775 6e64  _filter === 'und
-00004aa0: 6566 696e 6564 2729 7b0a 2020 2020 2020  efined'){.      
-00004ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ad0: 2020 2020 2020 2020 2020 696e 6974 5f66            init_f
-00004ae0: 696c 7465 7220 3d20 6174 7472 3b0a 2020  ilter = attr;.  
-00004af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b10: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00000090: 7420 5549 440a 0a53 5459 4c45 5348 4545  t UID..STYLESHEE
+000000a0: 545f 5552 4c53 203d 205b 0a20 2020 2022  T_URLS = [.    "
+000000b0: 6874 7470 733a 2f2f 666f 6e74 732e 676f  https://fonts.go
+000000c0: 6f67 6c65 6170 6973 2e63 6f6d 2f63 7373  ogleapis.com/css
+000000d0: 323f 6661 6d69 6c79 3d4b 6172 6c61 3a69  2?family=Karla:i
+000000e0: 7461 6c2c 7767 6874 4030 2c32 3030 3b30  tal,wght@0,200;0
+000000f0: 2c33 3030 3b30 2c34 3030 3b30 2c35 3030  ,300;0,400;0,500
+00000100: 3b30 2c36 3030 3b30 2c37 3030 3b30 2c38  ;0,600;0,700;0,8
+00000110: 3030 3b31 2c32 3030 3b31 2c33 3030 3b31  00;1,200;1,300;1
+00000120: 2c34 3030 3b31 2c35 3030 3b31 2c36 3030  ,400;1,500;1,600
+00000130: 3b31 2c37 3030 3b31 2c38 3030 2666 616d  ;1,700;1,800&fam
+00000140: 696c 793d 4f70 656e 2b53 616e 733a 6974  ily=Open+Sans:it
+00000150: 616c 2c77 6768 7440 302c 3330 302e 2e38  al,wght@0,300..8
+00000160: 3030 3b31 2c33 3030 2e2e 3830 3026 6469  00;1,300..800&di
+00000170: 7370 6c61 793d 7377 6170 222c 0a20 2020  splay=swap",.   
+00000180: 2022 6874 7470 733a 2f2f 666f 6e74 732e   "https://fonts.
+00000190: 6364 6e66 6f6e 7473 2e63 6f6d 2f63 7373  cdnfonts.com/css
+000001a0: 2f64 656a 6176 752d 7361 6e73 2d6d 6f6e  /dejavu-sans-mon
+000001b0: 6f22 2c0a 5d0a 5354 594c 4553 4845 4554  o",.].STYLESHEET
+000001c0: 5f4a 535f 4341 4c4c 5320 3d20 225c 6e22  _JS_CALLS = "\n"
+000001d0: 2e6a 6f69 6e28 5b66 2761 6464 5374 796c  .join([f'addStyl
+000001e0: 6553 6865 6574 2822 7b73 7d22 2927 2066  eSheet("{s}")' f
+000001f0: 6f72 2073 2069 6e20 5354 594c 4553 4845  or s in STYLESHE
+00000200: 4554 5f55 524c 535d 290a 0a0a 4a53 5f44  ET_URLS])...JS_D
+00000210: 4f57 4e4c 4f41 445f 464f 4e54 5320 3d20  OWNLOAD_FONTS = 
+00000220: 6622 2222 0a3c 7363 7269 7074 3e0a 6675  f""".<script>.fu
+00000230: 6e63 7469 6f6e 2061 6464 5374 796c 6553  nction addStyleS
+00000240: 6865 6574 2866 696c 654e 616d 6529 207b  heet(fileName) {
+00000250: 7b0a 0a20 2076 6172 2068 6561 6420 3d20  {..  var head = 
+00000260: 646f 6375 6d65 6e74 2e68 6561 643b 0a20  document.head;. 
+00000270: 2076 6172 206c 696e 6b20 3d20 646f 6375   var link = docu
+00000280: 6d65 6e74 2e63 7265 6174 6545 6c65 6d65  ment.createEleme
+00000290: 6e74 2822 6c69 6e6b 2229 3b0a 0a20 206c  nt("link");..  l
+000002a0: 696e 6b2e 7479 7065 203d 2022 7465 7874  ink.type = "text
+000002b0: 2f63 7373 223b 0a20 206c 696e 6b2e 7265  /css";.  link.re
+000002c0: 6c20 3d20 2273 7479 6c65 7368 6565 7422  l = "stylesheet"
+000002d0: 3b0a 2020 6c69 6e6b 2e68 7265 6620 3d20  ;.  link.href = 
+000002e0: 6669 6c65 4e61 6d65 3b0a 0a20 2068 6561  fileName;..  hea
+000002f0: 642e 6170 7065 6e64 4368 696c 6428 6c69  d.appendChild(li
+00000300: 6e6b 293b 0a7d 7d0a 0a7b 5354 594c 4553  nk);.}}..{STYLES
+00000310: 4845 4554 5f4a 535f 4341 4c4c 537d 0a3c  HEET_JS_CALLS}.<
+00000320: 2f73 6372 6970 743e 0a22 2222 0a0a 0a43  /script>."""...C
+00000330: 5353 203d 2022 2222 0a3c 7374 796c 653e  SS = """.<style>
+00000340: 0a20 202e 7379 6674 2d77 6964 6765 7420  .  .syft-widget 
+00000350: 626f 6479 5b64 6174 612d 6a70 2d74 6865  body[data-jp-the
+00000360: 6d65 2d6c 6967 6874 3d27 6661 6c73 6527  me-light='false'
+00000370: 5d20 7b0a 2020 2020 2020 2020 2d2d 7072  ] {.        --pr
+00000380: 696d 6172 792d 636f 6c6f 723a 2023 3131  imary-color: #11
+00000390: 3131 3131 3b0a 2020 2020 2020 2020 2d2d  1111;.        --
+000003a0: 7365 636f 6e64 6172 792d 636f 6c6f 723a  secondary-color:
+000003b0: 2023 3231 3231 3231 3b0a 2020 2020 2020   #212121;.      
+000003c0: 2020 2d2d 7465 7274 6961 7279 2d63 6f6c    --tertiary-col
+000003d0: 6f72 3a20 2343 4643 4444 363b 0a20 2020  or: #CFCDD6;.   
+000003e0: 2020 2020 202d 2d62 7574 746f 6e2d 636f       --button-co
+000003f0: 6c6f 723a 2023 3131 3131 3131 3b0a 2020  lor: #111111;.  
+00000400: 7d0a 0a20 202e 7379 6674 2d77 6964 6765  }..  .syft-widge
+00000410: 7420 626f 6479 207b 0a20 2020 2020 2020  t body {.       
+00000420: 202d 2d70 7269 6d61 7279 2d63 6f6c 6f72   --primary-color
+00000430: 3a20 2366 6666 6666 663b 0a20 2020 2020  : #ffffff;.     
+00000440: 2020 202d 2d73 6563 6f6e 6461 7279 2d63     --secondary-c
+00000450: 6f6c 6f72 3a20 2366 3566 3566 353b 0a20  olor: #f5f5f5;. 
+00000460: 2020 2020 2020 202d 2d74 6572 7469 6172         --tertiar
+00000470: 792d 636f 6c6f 723a 2023 3030 3030 3030  y-color: #000000
+00000480: 6465 3b0a 2020 2020 2020 2020 2d2d 6275  de;.        --bu
+00000490: 7474 6f6e 2d63 6f6c 6f72 3a20 2364 3164  tton-color: #d1d
+000004a0: 3564 623b 0a20 207d 0a0a 2020 2e68 6561  5db;.  }..  .hea
+000004b0: 6465 722d 3120 7b0a 2020 2020 2020 2020  der-1 {.        
+000004c0: 666f 6e74 2d73 7479 6c65 3a20 6e6f 726d  font-style: norm
+000004d0: 616c 3b0a 2020 2020 2020 2020 666f 6e74  al;.        font
+000004e0: 2d77 6569 6768 743a 2036 3030 3b0a 2020  -weight: 600;.  
+000004f0: 2020 2020 2020 666f 6e74 2d73 697a 653a        font-size:
+00000500: 2032 2e30 3733 3665 6d3b 0a20 2020 2020   2.0736em;.     
+00000510: 2020 206c 696e 652d 6865 6967 6874 3a20     line-height: 
+00000520: 3130 3025 3b0a 2020 2020 2020 2020 6c65  100%;.        le
+00000530: 6164 696e 672d 7472 696d 3a20 626f 7468  ading-trim: both
+00000540: 3b0a 2020 2020 2020 2020 7465 7874 2d65  ;.        text-e
+00000550: 6467 653a 2063 6170 3b0a 2020 2020 2020  dge: cap;.      
+00000560: 2020 636f 6c6f 723a 2023 3137 3136 3144    color: #17161D
+00000570: 3b0a 2020 2020 7d0a 0a20 202e 6865 6164  ;.    }..  .head
+00000580: 6572 2d32 207b 0a20 2020 2020 2020 2066  er-2 {.        f
+00000590: 6f6e 742d 7374 796c 653a 206e 6f72 6d61  ont-style: norma
+000005a0: 6c3b 0a20 2020 2020 2020 2066 6f6e 742d  l;.        font-
+000005b0: 7765 6967 6874 3a20 3630 303b 0a20 2020  weight: 600;.   
+000005c0: 2020 2020 2066 6f6e 742d 7369 7a65 3a20       font-size: 
+000005d0: 312e 3732 3865 6d3b 0a20 2020 2020 2020  1.728em;.       
+000005e0: 206c 696e 652d 6865 6967 6874 3a20 3130   line-height: 10
+000005f0: 3025 3b0a 2020 2020 2020 2020 6c65 6164  0%;.        lead
+00000600: 696e 672d 7472 696d 3a20 626f 7468 3b0a  ing-trim: both;.
+00000610: 2020 2020 2020 2020 7465 7874 2d65 6467          text-edg
+00000620: 653a 2063 6170 3b0a 2020 2020 2020 2020  e: cap;.        
+00000630: 636f 6c6f 723a 2023 3137 3136 3144 3b0a  color: #17161D;.
+00000640: 2020 2020 7d0a 0a20 202e 6865 6164 6572      }..  .header
+00000650: 2d33 207b 0a20 2020 2020 2020 2066 6f6e  -3 {.        fon
+00000660: 742d 7374 796c 653a 206e 6f72 6d61 6c3b  t-style: normal;
+00000670: 0a20 2020 2020 2020 2066 6f6e 742d 7765  .        font-we
+00000680: 6967 6874 3a20 3630 303b 0a20 2020 2020  ight: 600;.     
+00000690: 2020 2066 6f6e 742d 7369 7a65 3a20 2031     font-size:  1
+000006a0: 2e34 3465 6d3b 0a20 2020 2020 2020 206c  .44em;.        l
+000006b0: 696e 652d 6865 6967 6874 3a20 3130 3025  ine-height: 100%
+000006c0: 3b0a 2020 2020 2020 2020 6c65 6164 696e  ;.        leadin
+000006d0: 672d 7472 696d 3a20 626f 7468 3b0a 2020  g-trim: both;.  
+000006e0: 2020 2020 2020 7465 7874 2d65 6467 653a        text-edge:
+000006f0: 2063 6170 3b0a 2020 2020 2020 2020 636f   cap;.        co
+00000700: 6c6f 723a 2076 6172 282d 2d74 6572 7469  lor: var(--terti
+00000710: 6172 792d 636f 6c6f 7229 3b0a 2020 2020  ary-color);.    
+00000720: 7d0a 0a20 202e 6865 6164 6572 2d34 207b  }..  .header-4 {
+00000730: 0a20 2020 2020 2020 2066 6f6e 742d 7374  .        font-st
+00000740: 796c 653a 206e 6f72 6d61 6c3b 0a20 2020  yle: normal;.   
+00000750: 2020 2020 2066 6f6e 742d 7765 6967 6874       font-weight
+00000760: 3a20 3630 303b 0a20 2020 2020 2020 2066  : 600;.        f
+00000770: 6f6e 742d 7369 7a65 3a20 312e 3265 6d3b  ont-size: 1.2em;
+00000780: 0a20 2020 2020 2020 206c 696e 652d 6865  .        line-he
+00000790: 6967 6874 3a20 3130 3025 3b0a 2020 2020  ight: 100%;.    
+000007a0: 2020 2020 6c65 6164 696e 672d 7472 696d      leading-trim
+000007b0: 3a20 626f 7468 3b0a 2020 2020 2020 2020  : both;.        
+000007c0: 7465 7874 2d65 6467 653a 2063 6170 3b0a  text-edge: cap;.
+000007d0: 2020 2020 2020 2020 636f 6c6f 723a 2023          color: #
+000007e0: 3137 3136 3144 3b0a 2020 2020 7d0a 0a20  17161D;.    }.. 
+000007f0: 2020 202e 7061 7261 6772 6170 6820 7b0a     .paragraph {.
+00000800: 2020 2020 2020 2020 666f 6e74 2d73 7479          font-sty
+00000810: 6c65 3a20 6e6f 726d 616c 3b0a 2020 2020  le: normal;.    
+00000820: 2020 2020 666f 6e74 2d77 6569 6768 743a      font-weight:
+00000830: 2034 3030 3b0a 2020 2020 2020 2020 666f   400;.        fo
+00000840: 6e74 2d73 697a 653a 2031 3470 783b 0a20  nt-size: 14px;. 
+00000850: 2020 2020 2020 206c 696e 652d 6865 6967         line-heig
+00000860: 6874 3a20 3130 3025 3b0a 2020 2020 2020  ht: 100%;.      
+00000870: 2020 6c65 6164 696e 672d 7472 696d 3a20    leading-trim: 
+00000880: 626f 7468 3b0a 2020 2020 2020 2020 7465  both;.        te
+00000890: 7874 2d65 6467 653a 2063 6170 3b0a 2020  xt-edge: cap;.  
+000008a0: 2020 2020 2020 636f 6c6f 723a 2023 3245        color: #2E
+000008b0: 3242 3342 3b0a 2020 2020 7d0a 0a20 2020  2B3B;.    }..   
+000008c0: 202e 7061 7261 6772 6170 682d 736d 207b   .paragraph-sm {
+000008d0: 0a20 2020 2020 2020 2066 6f6e 742d 6661  .        font-fa
+000008e0: 6d69 6c79 3a20 2752 6f62 6f74 6f27 3b0a  mily: 'Roboto';.
+000008f0: 2020 2020 2020 2020 666f 6e74 2d73 7479          font-sty
+00000900: 6c65 3a20 6e6f 726d 616c 3b0a 2020 2020  le: normal;.    
+00000910: 2020 2020 666f 6e74 2d77 6569 6768 743a      font-weight:
+00000920: 2034 3030 3b0a 2020 2020 2020 2020 666f   400;.        fo
+00000930: 6e74 2d73 697a 653a 2031 312e 3632 7078  nt-size: 11.62px
+00000940: 3b0a 2020 2020 2020 2020 6c69 6e65 2d68  ;.        line-h
+00000950: 6569 6768 743a 2031 3030 253b 0a20 2020  eight: 100%;.   
+00000960: 2020 2020 206c 6561 6469 6e67 2d74 7269       leading-tri
+00000970: 6d3a 2062 6f74 683b 0a20 2020 2020 2020  m: both;.       
+00000980: 2074 6578 742d 6564 6765 3a20 6361 703b   text-edge: cap;
+00000990: 0a20 2020 2020 2020 2063 6f6c 6f72 3a20  .        color: 
+000009a0: 2332 4532 4233 423b 0a20 2020 207d 0a20  #2E2B3B;.    }. 
+000009b0: 2020 202e 636f 6465 2d74 6578 7420 7b0a     .code-text {.
+000009c0: 2020 2020 2020 2020 666f 6e74 2d66 616d          font-fam
+000009d0: 696c 793a 2027 436f 6e73 6f6c 6173 273b  ily: 'Consolas';
+000009e0: 0a20 2020 2020 2020 2066 6f6e 742d 7374  .        font-st
+000009f0: 796c 653a 206e 6f72 6d61 6c3b 0a20 2020  yle: normal;.   
+00000a00: 2020 2020 2066 6f6e 742d 7765 6967 6874       font-weight
+00000a10: 3a20 3430 303b 0a20 2020 2020 2020 2066  : 400;.        f
+00000a20: 6f6e 742d 7369 7a65 3a20 3133 7078 3b0a  ont-size: 13px;.
+00000a30: 2020 2020 2020 2020 6c69 6e65 2d68 6569          line-hei
+00000a40: 6768 743a 2031 3330 253b 0a20 2020 2020  ght: 130%;.     
+00000a50: 2020 206c 6561 6469 6e67 2d74 7269 6d3a     leading-trim:
+00000a60: 2062 6f74 683b 0a20 2020 2020 2020 2074   both;.        t
+00000a70: 6578 742d 6564 6765 3a20 6361 703b 0a20  ext-edge: cap;. 
+00000a80: 2020 2020 2020 2063 6f6c 6f72 3a20 2332         color: #2
+00000a90: 4532 4233 423b 0a20 2020 207d 0a0a 2020  E2B3B;.    }..  
+00000aa0: 2020 2e6e 756d 6265 7269 6e67 2d65 6e74    .numbering-ent
+00000ab0: 7279 207b 2064 6973 706c 6179 3a20 6e6f  ry { display: no
+00000ac0: 6e65 207d 0a0a 2020 2020 2f2a 2054 6f6f  ne }..    /* Too
+00000ad0: 6c74 6970 2063 6f6e 7461 696e 6572 202a  ltip container *
+00000ae0: 2f0a 2020 2020 2e74 6f6f 6c74 6970 207b  /.    .tooltip {
+00000af0: 0a20 2020 2020 2020 2070 6f73 6974 696f  .        positio
+00000b00: 6e3a 2072 656c 6174 6976 653b 0a20 2020  n: relative;.   
+00000b10: 2020 2020 2064 6973 706c 6179 3a20 696e       display: in
+00000b20: 6c69 6e65 2d62 6c6f 636b 3b0a 2020 2020  line-block;.    
+00000b30: 2020 2020 626f 7264 6572 2d62 6f74 746f      border-botto
+00000b40: 6d3a 2031 7078 2064 6f74 7465 6420 626c  m: 1px dotted bl
+00000b50: 6163 6b3b 202f 2a20 4966 2079 6f75 2077  ack; /* If you w
+00000b60: 616e 7420 646f 7473 2075 6e64 6572 2074  ant dots under t
+00000b70: 6865 2068 6f76 6572 6162 6c65 2074 6578  he hoverable tex
+00000b80: 7420 2a2f 0a20 2020 207d 0a0a 2020 2020  t */.    }..    
+00000b90: 2f2a 2054 6f6f 6c74 6970 2074 6578 7420  /* Tooltip text 
+00000ba0: 2a2f 0a20 2020 202e 746f 6f6c 7469 7020  */.    .tooltip 
+00000bb0: 2e74 6f6f 6c74 6970 7465 7874 207b 0a20  .tooltiptext {. 
+00000bc0: 2020 2020 2020 2076 6973 6962 696c 6974         visibilit
+00000bd0: 793a 2068 6964 6465 6e3b 0a20 2020 2020  y: hidden;.     
+00000be0: 2020 2077 6964 7468 3a20 3132 3070 783b     width: 120px;
+00000bf0: 0a20 2020 2020 2020 2062 6163 6b67 726f  .        backgro
+00000c00: 756e 642d 636f 6c6f 723a 2062 6c61 636b  und-color: black
+00000c10: 3b0a 2020 2020 2020 2020 636f 6c6f 723a  ;.        color:
+00000c20: 2023 6666 663b 0a20 2020 2020 2020 2074   #fff;.        t
+00000c30: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00000c40: 723b 0a20 2020 2020 2020 2070 6164 6469  r;.        paddi
+00000c50: 6e67 3a20 3570 7820 303b 0a20 2020 2020  ng: 5px 0;.     
+00000c60: 2020 2062 6f72 6465 722d 7261 6469 7573     border-radius
+00000c70: 3a20 3670 783b 0a0a 2020 2020 2020 2020  : 6px;..        
+00000c80: 2f2a 2050 6f73 6974 696f 6e20 7468 6520  /* Position the 
+00000c90: 746f 6f6c 7469 7020 7465 7874 202d 2073  tooltip text - s
+00000ca0: 6565 2065 7861 6d70 6c65 7320 6265 6c6f  ee examples belo
+00000cb0: 7721 202a 2f0a 2020 2020 2020 2020 706f  w! */.        po
+00000cc0: 7369 7469 6f6e 3a20 6162 736f 6c75 7465  sition: absolute
+00000cd0: 3b0a 2020 2020 2020 2020 7a2d 696e 6465  ;.        z-inde
+00000ce0: 783a 2031 3b0a 2020 2020 7d0a 0a20 2020  x: 1;.    }..   
+00000cf0: 202e 7265 7072 2d63 656c 6c20 7b0a 2020   .repr-cell {.  
+00000d00: 2020 2020 7061 6464 696e 672d 746f 703a      padding-top:
+00000d10: 2032 3070 783b 0a20 2020 207d 0a0a 2020   20px;.    }..  
+00000d20: 2020 2e74 6578 742d 626f 6c64 207b 0a20    .text-bold {. 
+00000d30: 2020 2020 2020 2066 6f6e 742d 7765 6967         font-weig
+00000d40: 6874 3a20 626f 6c64 3b0a 2020 2020 7d0a  ht: bold;.    }.
+00000d50: 0a20 2020 202e 7072 2d38 207b 0a20 2020  .    .pr-8 {.   
+00000d60: 2020 2020 2070 6164 6469 6e67 2d72 6967       padding-rig
+00000d70: 6874 3a20 3870 783b 0a20 2020 207d 0a20  ht: 8px;.    }. 
+00000d80: 2020 202e 7074 2d38 207b 0a20 2020 2020     .pt-8 {.     
+00000d90: 2020 2070 6164 6469 6e67 2d74 6f70 3a20     padding-top: 
+00000da0: 3870 783b 0a20 2020 207d 0a20 2020 202e  8px;.    }.    .
+00000db0: 706c 2d38 207b 0a20 2020 2020 2020 2070  pl-8 {.        p
+00000dc0: 6164 6469 6e67 2d6c 6566 743a 2038 7078  adding-left: 8px
+00000dd0: 3b0a 2020 2020 7d0a 2020 2020 2e70 622d  ;.    }.    .pb-
+00000de0: 3820 7b0a 2020 2020 2020 2020 7061 6464  8 {.        padd
+00000df0: 696e 672d 626f 7474 6f6d 3a20 3870 783b  ing-bottom: 8px;
+00000e00: 0a20 2020 207d 0a0a 2020 2020 2e70 792d  .    }..    .py-
+00000e10: 3235 7b0a 2020 2020 2020 2020 7061 6464  25{.        padd
+00000e20: 696e 672d 746f 703a 2032 3570 783b 0a20  ing-top: 25px;. 
+00000e30: 2020 2020 2020 2070 6164 6469 6e67 2d62         padding-b
+00000e40: 6f74 746f 6d3a 2032 3570 783b 0a20 2020  ottom: 25px;.   
+00000e50: 207d 0a0a 2020 2020 2e66 6c65 7820 7b0a   }..    .flex {.
+00000e60: 2020 2020 2020 2020 6469 7370 6c61 793a          display:
+00000e70: 2066 6c65 783b 0a20 2020 207d 0a0a 2020   flex;.    }..  
+00000e80: 2020 2e67 6170 2d31 3020 7b0a 2020 2020    .gap-10 {.    
+00000e90: 2020 2020 6761 703a 2031 3070 783b 0a20      gap: 10px;. 
+00000ea0: 2020 207d 0a20 2020 202e 6974 656d 732d     }.    .items-
+00000eb0: 6365 6e74 6572 7b0a 2020 2020 2020 2020  center{.        
+00000ec0: 616c 6967 6e2d 6974 656d 733a 2063 656e  align-items: cen
+00000ed0: 7465 723b 0a20 2020 207d 0a0a 2020 2020  ter;.    }..    
+00000ee0: 2e66 6f6c 6465 722d 6963 6f6e 207b 0a20  .folder-icon {. 
+00000ef0: 2020 2020 2020 2063 6f6c 6f72 3a20 7661         color: va
+00000f00: 7228 2d2d 7465 7274 6961 7279 2d63 6f6c  r(--tertiary-col
+00000f10: 6f72 293b 0a20 2020 207d 0a0a 2020 2020  or);.    }..    
+00000f20: 2e73 6561 7263 682d 696e 7075 747b 0a20  .search-input{. 
+00000f30: 2020 2020 2020 2064 6973 706c 6179 3a20         display: 
+00000f40: 666c 6578 3b0a 2020 2020 2020 2020 666c  flex;.        fl
+00000f50: 6578 2d64 6972 6563 7469 6f6e 3a20 726f  ex-direction: ro
+00000f60: 773b 0a20 2020 2020 2020 2061 6c69 676e  w;.        align
+00000f70: 2d69 7465 6d73 3a20 6365 6e74 6572 3b0a  -items: center;.
+00000f80: 2020 2020 2020 2020 7061 6464 696e 673a          padding:
+00000f90: 2038 7078 2031 3270 783b 0a20 2020 2020   8px 12px;.     
+00000fa0: 2020 2077 6964 7468 3a20 3334 3370 783b     width: 343px;
+00000fb0: 0a20 2020 2020 2020 2068 6569 6768 743a  .        height:
+00000fc0: 2032 3470 783b 0a20 2020 2020 2020 202f   24px;.        /
+00000fd0: 2a20 4c74 204f 6e20 5375 7266 6163 652f  * Lt On Surface/
+00000fe0: 4c6f 7720 2a2f 0a20 2020 2020 2020 2062  Low */.        b
+00000ff0: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
+00001000: 2076 6172 282d 2d73 6563 6f6e 6461 7279   var(--secondary
+00001010: 2d63 6f6c 6f72 293b 0a20 2020 2020 2020  -color);.       
+00001020: 2062 6f72 6465 722d 7261 6469 7573 3a20   border-radius: 
+00001030: 3330 7078 3b0a 0a20 2020 2020 2020 202f  30px;..        /
+00001040: 2a20 4c74 204f 6e20 5375 7266 6163 652f  * Lt On Surface/
+00001050: 4869 6768 6573 7420 2a2f 0a20 2020 2020  Highest */.     
+00001060: 2020 2063 6f6c 6f72 3a20 7661 7228 2d2d     color: var(--
+00001070: 7465 7274 6961 7279 2d63 6f6c 6f72 293b  tertiary-color);
+00001080: 0a20 2020 2020 2020 2062 6f72 6465 723a  .        border:
+00001090: 6e6f 6e65 3b0a 2020 2020 2020 2020 2f2a  none;.        /*
+000010a0: 2049 6e73 6964 6520 6175 746f 206c 6179   Inside auto lay
+000010b0: 6f75 7420 2a2f 0a20 2020 2020 2020 2066  out */.        f
+000010c0: 6c65 783a 206e 6f6e 653b 0a20 2020 2020  lex: none;.     
+000010d0: 2020 206f 7264 6572 3a20 303b 0a20 2020     order: 0;.   
+000010e0: 2020 2020 2066 6c65 782d 6772 6f77 3a20       flex-grow: 
+000010f0: 303b 0a20 2020 207d 0a20 2020 202e 7365  0;.    }.    .se
+00001100: 6172 6368 2d69 6e70 7574 3a66 6f63 7573  arch-input:focus
+00001110: 207b 0a20 2020 2020 2020 206f 7574 6c69   {.        outli
+00001120: 6e65 3a20 6e6f 6e65 3b0a 2020 2020 7d0a  ne: none;.    }.
+00001130: 2020 2020 2020 2020 2e73 6561 7263 682d          .search-
+00001140: 696e 7075 743a 666f 6375 733a 3a70 6c61  input:focus::pla
+00001150: 6365 686f 6c64 6572 2c0a 2020 2020 2e73  ceholder,.    .s
+00001160: 6561 7263 682d 696e 7075 743a 3a70 6c61  earch-input::pla
+00001170: 6365 686f 6c64 6572 207b 202f 2a20 4368  ceholder { /* Ch
+00001180: 726f 6d65 2c20 4669 7265 666f 782c 204f  rome, Firefox, O
+00001190: 7065 7261 2c20 5361 6661 7269 2031 302e  pera, Safari 10.
+000011a0: 312b 202a 2f0a 2020 2020 2020 2020 636f  1+ */.        co
+000011b0: 6c6f 723a 2076 6172 282d 2d74 6572 7469  lor: var(--terti
+000011c0: 6172 792d 636f 6c6f 7229 3b0a 2020 2020  ary-color);.    
+000011d0: 2020 2020 6f70 6163 6974 793a 2031 3b20      opacity: 1; 
+000011e0: 2f2a 2046 6972 6566 6f78 202a 2f0a 2020  /* Firefox */.  
+000011f0: 2020 7d0a 0a20 2020 202e 7365 6172 6368    }..    .search
+00001200: 2d62 7574 746f 6e7b 0a20 2020 2020 2020  -button{.       
+00001210: 202f 2a20 5365 6172 6368 202a 2f0a 2020   /* Search */.  
+00001220: 2020 2020 2020 6c65 6164 696e 672d 7472        leading-tr
+00001230: 696d 3a20 626f 7468 3b0a 2020 2020 2020  im: both;.      
+00001240: 2020 7465 7874 2d65 6467 653a 2063 6170    text-edge: cap
+00001250: 3b0a 2020 2020 2020 2020 6469 7370 6c61  ;.        displa
+00001260: 793a 2066 6c65 783b 0a20 2020 2020 2020  y: flex;.       
+00001270: 2061 6c69 676e 2d69 7465 6d73 3a20 6365   align-items: ce
+00001280: 6e74 6572 3b0a 2020 2020 2020 2020 7465  nter;.        te
+00001290: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+000012a0: 3b0a 0a20 2020 2020 2020 202f 2a20 5072  ;..        /* Pr
+000012b0: 696d 6172 792f 4f6e 204c 6967 6874 202a  imary/On Light *
+000012c0: 2f0a 2020 2020 2020 2020 6261 636b 6772  /.        backgr
+000012d0: 6f75 6e64 2d63 6f6c 6f72 3a20 7661 7228  ound-color: var(
+000012e0: 2d2d 6275 7474 6f6e 2d63 6f6c 6f72 293b  --button-color);
+000012f0: 0a20 2020 2020 2020 2063 6f6c 6f72 3a20  .        color: 
+00001300: 7661 7228 2d2d 7465 7274 6961 7279 2d63  var(--tertiary-c
+00001310: 6f6c 6f72 293b 0a0a 2020 2020 2020 2020  olor);..        
+00001320: 626f 7264 6572 2d72 6164 6975 733a 2033  border-radius: 3
+00001330: 3070 783b 0a20 2020 2020 2020 2062 6f72  0px;.        bor
+00001340: 6465 722d 636f 6c6f 723a 2076 6172 282d  der-color: var(-
+00001350: 2d73 6563 6f6e 6461 7279 2d63 6f6c 6f72  -secondary-color
+00001360: 293b 0a20 2020 2020 2020 2062 6f72 6465  );.        borde
+00001370: 722d 7374 796c 653a 2073 6f6c 6964 3b0a  r-style: solid;.
+00001380: 2020 2020 2020 2020 626f 782d 7368 6164          box-shad
+00001390: 6f77 3a20 7267 6261 2836 302c 2036 342c  ow: rgba(60, 64,
+000013a0: 2036 372c 2030 2e33 2920 3070 7820 3170   67, 0.3) 0px 1p
+000013b0: 7820 3270 7820 3070 782c 2072 6762 6128  x 2px 0px, rgba(
+000013c0: 3630 2c20 3634 2c20 3637 2c20 302e 3135  60, 64, 67, 0.15
+000013d0: 2920 3070 7820 3170 7820 3370 7820 3170  ) 0px 1px 3px 1p
+000013e0: 783b 0a20 2020 2020 2020 2063 7572 736f  x;.        curso
+000013f0: 723a 2070 6f69 6e74 6572 3b0a 2020 2020  r: pointer;.    
+00001400: 2020 2020 2f2a 2049 6e73 6964 6520 6175      /* Inside au
+00001410: 746f 206c 6179 6f75 7420 2a2f 0a20 2020  to layout */.   
+00001420: 2020 2020 2066 6c65 783a 206e 6f6e 653b       flex: none;
+00001430: 0a20 2020 2020 2020 206f 7264 6572 3a20  .        order: 
+00001440: 313b 0a20 2020 2020 2020 2066 6c65 782d  1;.        flex-
+00001450: 6772 6f77 3a20 303b 0a20 2020 207d 0a0a  grow: 0;.    }..
+00001460: 2020 2020 2e67 7269 642d 7461 626c 6524      .grid-table$
+00001470: 7b75 6964 7d20 7b0a 2020 2020 2020 2020  {uid} {.        
+00001480: 6469 7370 6c61 793a 6772 6964 3b0a 2020  display:grid;.  
+00001490: 2020 2020 2020 6772 6964 2d74 656d 706c        grid-templ
+000014a0: 6174 652d 636f 6c75 6d6e 733a 2024 7b67  ate-columns: ${g
+000014b0: 7269 645f 7465 6d70 6c61 7465 5f63 6f6c  rid_template_col
+000014c0: 756d 6e73 7d3b 0a20 2020 2020 2020 202f  umns};.        /
+000014d0: 2a67 7269 642d 7465 6d70 6c61 7465 2d72  *grid-template-r
+000014e0: 6f77 733a 2072 6570 6561 7428 322c 2031  ows: repeat(2, 1
+000014f0: 6672 293b 2a2f 0a20 2020 2020 2020 2070  fr);*/.        p
+00001500: 6f73 6974 696f 6e3a 2072 656c 6174 6976  osition: relativ
+00001510: 653b 0a20 2020 207d 0a0a 2020 2020 2e67  e;.    }..    .g
+00001520: 7269 642d 7374 642d 6365 6c6c 7324 7b75  rid-std-cells${u
+00001530: 6964 7d20 7b0a 2020 2020 2020 2020 6772  id} {.        gr
+00001540: 6964 2d63 6f6c 756d 6e3a 2024 7b67 7269  id-column: ${gri
+00001550: 645f 7465 6d70 6c61 7465 5f63 656c 6c5f  d_template_cell_
+00001560: 636f 6c75 6d6e 737d 3b0a 2020 2020 2020  columns};.      
+00001570: 2020 6469 7370 6c61 793a 2066 6c65 783b    display: flex;
+00001580: 0a20 2020 2020 2020 206a 7573 7469 6679  .        justify
+00001590: 2d63 6f6e 7465 6e74 3a20 6365 6e74 6572  -content: center
+000015a0: 3b0a 2020 2020 2020 2020 616c 6967 6e2d  ;.        align-
+000015b0: 6974 656d 733a 2063 656e 7465 723b 2077  items: center; w
+000015c0: 6964 7468 3a20 3130 3025 3b20 6865 6967  idth: 100%; heig
+000015d0: 6874 3a20 3130 3025 3b0a 2020 2020 7d0a  ht: 100%;.    }.
+000015e0: 0a20 2020 202e 6772 6964 2d69 6e64 6578  .    .grid-index
+000015f0: 2d63 656c 6c73 207b 0a20 2020 2020 2020  -cells {.       
+00001600: 2067 7269 642d 636f 6c75 6d6e 3a20 7370   grid-column: sp
+00001610: 616e 2031 3b0a 2020 2020 2020 2020 2f2a  an 1;.        /*
+00001620: 2074 6d70 2066 6978 2074 6f20 6d61 6b65   tmp fix to make
+00001630: 206c 6566 7420 636f 6c20 7374 616e 6420   left col stand 
+00001640: 6f75 7420 2866 6978 2077 6974 6820 666f  out (fix with fo
+00001650: 6e74 2d66 616d 696c 7929 202a 2f0a 2020  nt-family) */.  
+00001660: 2020 2020 2020 666f 6e74 2d77 6569 6768        font-weigh
+00001670: 743a 2036 3030 3b0a 2020 2020 2020 2020  t: 600;.        
+00001680: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
+00001690: 3a20 7661 7228 2d2d 7365 636f 6e64 6172  : var(--secondar
+000016a0: 792d 636f 6c6f 7229 2021 696d 706f 7274  y-color) !import
+000016b0: 616e 743b 0a20 2020 2020 2020 2063 6f6c  ant;.        col
+000016c0: 6f72 3a20 7661 7228 2d2d 7465 7274 6961  or: var(--tertia
+000016d0: 7279 2d63 6f6c 6f72 293b 0a20 2020 2020  ry-color);.     
+000016e0: 2020 2068 6569 6768 743a 2031 3030 253b     height: 100%;
+000016f0: 0a20 2020 207d 0a0a 2020 2020 2e63 656e  .    }..    .cen
+00001700: 7465 722d 636f 6e74 656e 742d 6365 6c6c  ter-content-cell
+00001710: 7b0a 2020 2020 2020 2020 6d61 7267 696e  {.        margin
+00001720: 3a20 6175 746f 3b0a 2020 2020 7d0a 0a20  : auto;.    }.. 
+00001730: 2020 202e 6772 6964 2d68 6561 6465 7220     .grid-header 
+00001740: 7b0a 2020 2020 2020 2020 2f2a 2041 7574  {.        /* Aut
+00001750: 6f20 6c61 796f 7574 202a 2f0a 2020 2020  o layout */.    
+00001760: 2020 2020 6469 7370 6c61 793a 2066 6c65      display: fle
+00001770: 783b 0a20 2020 2020 2020 2066 6c65 782d  x;.        flex-
+00001780: 6469 7265 6374 696f 6e3a 2063 6f6c 756d  direction: colum
+00001790: 6e3b 0a20 2020 2020 2020 2061 6c69 676e  n;.        align
+000017a0: 2d69 7465 6d73 3a20 6365 6e74 6572 3b0a  -items: center;.
+000017b0: 2020 2020 2020 2020 7061 6464 696e 673a          padding:
+000017c0: 2036 7078 2034 7078 3b0a 0a20 2020 2020   6px 4px;..     
+000017d0: 2020 2072 6573 697a 653a 2068 6f72 697a     resize: horiz
+000017e0: 6f6e 7461 6c3b 0a20 2020 2020 2020 202f  ontal;.        /
+000017f0: 2a20 4c74 204f 6e20 5375 7266 6163 652f  * Lt On Surface/
+00001800: 5375 7266 6163 6520 2a2f 0a20 2020 2020  Surface */.     
+00001810: 2020 202f 2a20 4c74 204f 6e20 5375 7266     /* Lt On Surf
+00001820: 6163 652f 4869 6768 202a 2f0a 2020 2020  ace/High */.    
+00001830: 2020 2020 626f 7264 6572 3a20 3170 7820      border: 1px 
+00001840: 736f 6c69 6420 2343 4643 4444 363b 0a20  solid #CFCDD6;. 
+00001850: 2020 2020 2020 202f 2a20 746d 7020 6669         /* tmp fi
+00001860: 7820 746f 206d 616b 6520 6865 6164 6572  x to make header
+00001870: 2073 7461 6e64 206f 7574 2028 6669 7820   stand out (fix 
+00001880: 7769 7468 2066 6f6e 742d 6661 6d69 6c79  with font-family
+00001890: 2920 2a2f 0a20 2020 2020 2020 2066 6f6e  ) */.        fon
+000018a0: 742d 7765 6967 6874 3a20 3630 303b 0a20  t-weight: 600;. 
+000018b0: 2020 2020 2020 2062 6163 6b67 726f 756e         backgroun
+000018c0: 642d 636f 6c6f 723a 2076 6172 282d 2d73  d-color: var(--s
+000018d0: 6563 6f6e 6461 7279 2d63 6f6c 6f72 293b  econdary-color);
+000018e0: 0a20 2020 2020 2020 2063 6f6c 6f72 3a20  .        color: 
+000018f0: 7661 7228 2d2d 7465 7274 6961 7279 2d63  var(--tertiary-c
+00001900: 6f6c 6f72 293b 0a20 2020 207d 0a0a 2020  olor);.    }..  
+00001910: 2020 2e67 7269 642d 726f 7720 7b0a 2020    .grid-row {.  
+00001920: 2020 2020 2020 6469 7370 6c61 793a 2066        display: f
+00001930: 6c65 783b 0a20 2020 2020 2020 2066 6c65  lex;.        fle
+00001940: 782d 6469 7265 6374 696f 6e3a 2063 6f6c  x-direction: col
+00001950: 756d 6e3b 0a20 2020 2020 2020 2061 6c69  umn;.        ali
+00001960: 676e 2d69 7465 6d73 3a20 666c 6578 2d73  gn-items: flex-s
+00001970: 7461 7274 3b0a 2020 2020 2020 2020 7061  tart;.        pa
+00001980: 6464 696e 673a 2036 7078 2034 7078 3b0a  dding: 6px 4px;.
+00001990: 2020 2020 2020 2020 6f76 6572 666c 6f77          overflow
+000019a0: 3a20 6869 6464 656e 3b0a 2020 2020 2020  : hidden;.      
+000019b0: 2020 626f 7264 6572 3a20 3170 7820 736f    border: 1px so
+000019c0: 6c69 6420 2343 4643 4444 363b 0a20 2020  lid #CFCDD6;.   
+000019d0: 2020 2020 2062 6163 6b67 726f 756e 642d       background-
+000019e0: 636f 6c6f 723a 2076 6172 282d 2d70 7269  color: var(--pri
+000019f0: 6d61 7279 2d63 6f6c 6f72 293b 0a20 2020  mary-color);.   
+00001a00: 2020 2020 2063 6f6c 6f72 3a20 7661 7228       color: var(
+00001a10: 2d2d 7465 7274 6961 7279 2d63 6f6c 6f72  --tertiary-color
+00001a20: 293b 0a20 2020 207d 0a0a 0a20 2020 202e  );.    }...    .
+00001a30: 7379 6e63 7374 6174 652d 636f 6c2d 666f  syncstate-col-fo
+00001a40: 6f74 6572 207b 0a20 2020 2020 2020 2066  oter {.        f
+00001a50: 6f6e 742d 6661 6d69 6c79 3a20 2744 656a  ont-family: 'Dej
+00001a60: 6156 7520 5361 6e73 204d 6f6e 6f27 2c20  aVu Sans Mono', 
+00001a70: 274f 7065 6e20 5361 6e73 273b 0a20 2020  'Open Sans';.   
+00001a80: 2020 2020 2066 6f6e 742d 7369 7a65 3a20       font-size: 
+00001a90: 3132 7078 3b0a 2020 2020 2020 2020 666f  12px;.        fo
+00001aa0: 6e74 2d77 6569 6768 743a 2034 3030 3b0a  nt-weight: 400;.
+00001ab0: 2020 2020 2020 2020 6c69 6e65 2d68 6569          line-hei
+00001ac0: 6768 743a 2031 362e 3870 783b 0a20 2020  ght: 16.8px;.   
+00001ad0: 2020 2020 2074 6578 742d 616c 6967 6e3a       text-align:
+00001ae0: 206c 6566 743b 0a20 2020 2020 2020 2063   left;.        c
+00001af0: 6f6c 6f72 3a20 2335 4535 4137 323b 0a20  olor: #5E5A72;. 
+00001b00: 2020 207d 0a0a 2020 2020 2e73 796e 6373     }..    .syncs
+00001b10: 7461 7465 2d64 6573 6372 6970 7469 6f6e  tate-description
+00001b20: 207b 0a20 2020 2020 2020 2066 6f6e 742d   {.        font-
+00001b30: 6661 6d69 6c79 3a20 4f70 656e 2053 616e  family: Open San
+00001b40: 733b 0a20 2020 2020 2020 2066 6f6e 742d  s;.        font-
+00001b50: 7369 7a65 3a20 3134 7078 3b0a 2020 2020  size: 14px;.    
+00001b60: 2020 2020 666f 6e74 2d77 6569 6768 743a      font-weight:
+00001b70: 2036 3030 3b0a 2020 2020 2020 2020 6c69   600;.        li
+00001b80: 6e65 2d68 6569 6768 743a 2031 392e 3670  ne-height: 19.6p
+00001b90: 783b 0a20 2020 2020 2020 2074 6578 742d  x;.        text-
+00001ba0: 616c 6967 6e3a 206c 6566 743b 0a20 2020  align: left;.   
+00001bb0: 2020 2020 2077 6869 7465 2d73 7061 6365       white-space
+00001bc0: 3a20 6e6f 7772 6170 3b0a 2020 2020 2020  : nowrap;.      
+00001bd0: 2020 666c 6578 2d67 726f 773a 2031 3b0a    flex-grow: 1;.
+00001be0: 2020 2020 7d0a 0a20 2020 202e 7769 6467      }..    .widg
+00001bf0: 6574 2d68 6561 6465 7232 7b0a 2020 2020  et-header2{.    
+00001c00: 2020 2020 6469 7370 6c61 793a 2066 6c65      display: fle
+00001c10: 783b 0a20 2020 2020 2020 2067 6170 3a20  x;.        gap: 
+00001c20: 3870 783b 0a20 2020 2020 2020 206a 7573  8px;.        jus
+00001c30: 7469 6679 2d63 6f6e 7465 6e74 3a20 7374  tify-content: st
+00001c40: 6172 743b 0a20 2020 2020 2020 2077 6964  art;.        wid
+00001c50: 7468 3a20 3130 3025 3b0a 2020 2020 2020  th: 100%;.      
+00001c60: 2020 6f76 6572 666c 6f77 3a20 6869 6464    overflow: hidd
+00001c70: 656e 3b0a 2020 2020 2020 2020 616c 6967  en;.        alig
+00001c80: 6e2d 6974 656d 733a 2063 656e 7465 723b  n-items: center;
+00001c90: 0a20 2020 207d 0a0a 2020 2020 2e77 6964  .    }..    .wid
+00001ca0: 6765 742d 6865 6164 6572 322d 327b 0a20  get-header2-2{. 
+00001cb0: 2020 2020 2020 2064 6973 706c 6179 3a20         display: 
+00001cc0: 666c 6578 3b0a 2020 2020 2020 2020 6761  flex;.        ga
+00001cd0: 703a 2038 7078 3b0a 2020 2020 2020 2020  p: 8px;.        
+00001ce0: 6a75 7374 6966 792d 636f 6e74 656e 743a  justify-content:
+00001cf0: 2073 7461 7274 3b0a 2020 2020 2020 2020   start;.        
+00001d00: 616c 6967 6e2d 6974 656d 733a 2063 656e  align-items: cen
+00001d10: 7465 723b 0a20 2020 207d 0a0a 2020 2020  ter;.    }..    
+00001d20: 2e6a 6f62 732d 7469 746c 6520 7b0a 2020  .jobs-title {.  
+00001d30: 2020 2020 2020 666f 6e74 2d66 616d 696c        font-famil
+00001d40: 793a 204f 7065 6e20 5361 6e73 2c20 7361  y: Open Sans, sa
+00001d50: 6e73 2d73 6572 6966 3b0a 2020 2020 2020  ns-serif;.      
+00001d60: 2020 666f 6e74 2d73 697a 653a 2031 3870    font-size: 18p
+00001d70: 783b 0a20 2020 2020 2020 2066 6f6e 742d  x;.        font-
+00001d80: 7765 6967 6874 3a20 3630 303b 0a20 2020  weight: 600;.   
+00001d90: 2020 2020 206c 696e 652d 6865 6967 6874       line-height
+00001da0: 3a20 3235 2e32 7078 3b0a 2020 2020 2020  : 25.2px;.      
+00001db0: 2020 7465 7874 2d61 6c69 676e 3a20 6c65    text-align: le
+00001dc0: 6674 3b0a 2020 2020 2020 2020 636f 6c6f  ft;.        colo
+00001dd0: 723a 2023 3146 3536 3741 3b0a 2020 2020  r: #1F567A;.    
+00001de0: 7d0a 0a20 2020 202e 6469 6666 2d73 7461  }..    .diff-sta
+00001df0: 7465 2d6f 7261 6e67 652d 7465 7874 7b0a  te-orange-text{.
+00001e00: 2020 2020 2020 2020 636f 6c6f 723a 2023          color: #
+00001e10: 4238 3532 3041 3b0a 2020 2020 7d0a 0a20  B8520A;.    }.. 
+00001e20: 2020 202e 6469 6666 2d73 7461 7465 2d6e     .diff-state-n
+00001e30: 6f2d 6f62 6a7b 0a20 2020 2020 2020 2066  o-obj{.        f
+00001e40: 6f6e 742d 6661 6d69 6c79 3a20 2744 656a  ont-family: 'Dej
+00001e50: 6156 7520 5361 6e73 204d 6f6e 6f27 2c20  aVu Sans Mono', 
+00001e60: 274f 7065 6e20 5361 6e73 273b 0a20 2020  'Open Sans';.   
+00001e70: 2020 2020 2066 6f6e 742d 7369 7a65 3a20       font-size: 
+00001e80: 3132 7078 3b0a 2020 2020 2020 2020 666f  12px;.        fo
+00001e90: 6e74 2d77 6569 6768 743a 2034 3030 3b0a  nt-weight: 400;.
+00001ea0: 2020 2020 2020 2020 6c69 6e65 2d68 6569          line-hei
+00001eb0: 6768 743a 2031 362e 3870 783b 0a20 2020  ght: 16.8px;.   
+00001ec0: 2020 2020 2074 6578 742d 616c 6967 6e3a       text-align:
+00001ed0: 206c 6566 743b 0a20 2020 2020 2020 2063   left;.        c
+00001ee0: 6f6c 6f72 3a20 2335 4535 4137 323b 0a20  olor: #5E5A72;. 
+00001ef0: 2020 207d 0a0a 2020 2020 2e64 6966 662d     }..    .diff-
+00001f00: 7374 6174 652d 696e 7472 6f7b 0a20 2020  state-intro{.   
+00001f10: 2020 2020 2066 6f6e 742d 6661 6d69 6c79       font-family
+00001f20: 3a20 4f70 656e 2053 616e 733b 0a20 2020  : Open Sans;.   
+00001f30: 2020 2020 2066 6f6e 742d 7369 7a65 3a20       font-size: 
+00001f40: 3134 7078 3b0a 2020 2020 2020 2020 666f  14px;.        fo
+00001f50: 6e74 2d77 6569 6768 743a 2034 3030 3b0a  nt-weight: 400;.
+00001f60: 2020 2020 2020 2020 6c69 6e65 2d68 6569          line-hei
+00001f70: 6768 743a 2031 392e 3670 783b 0a20 2020  ght: 19.6px;.   
+00001f80: 2020 2020 2074 6578 742d 616c 6967 6e3a       text-align:
+00001f90: 206c 6566 743b 0a20 2020 2020 2020 2063   left;.        c
+00001fa0: 6f6c 6f72 3a20 2342 3442 3042 463b 0a20  olor: #B4B0BF;. 
+00001fb0: 2020 207d 0a0a 2020 2020 2e64 6966 662d     }..    .diff-
+00001fc0: 7374 6174 652d 6865 6164 6572 7b0a 2020  state-header{.  
+00001fd0: 2020 2020 2020 666f 6e74 2d66 616d 696c        font-famil
+00001fe0: 793a 204f 7065 6e20 5361 6e73 3b0a 2020  y: Open Sans;.  
+00001ff0: 2020 2020 2020 666f 6e74 2d73 697a 653a        font-size:
+00002000: 2032 3270 783b 0a20 2020 2020 2020 2066   22px;.        f
+00002010: 6f6e 742d 7765 6967 6874 3a20 3630 303b  ont-weight: 600;
+00002020: 0a20 2020 2020 2020 206c 696e 652d 6865  .        line-he
+00002030: 6967 6874 3a20 3330 2e38 7078 3b0a 2020  ight: 30.8px;.  
+00002040: 2020 2020 2020 7465 7874 2d61 6c69 676e        text-align
+00002050: 3a20 6c65 6674 3b0a 2020 2020 2020 2020  : left;.        
+00002060: 636f 6c6f 723a 2023 3335 3332 3433 3b0a  color: #353243;.
+00002070: 2020 2020 2020 2020 6469 7370 6c61 793a          display:
+00002080: 2066 6c65 783b 2067 6170 3a20 3870 783b   flex; gap: 8px;
+00002090: 0a20 2020 207d 0a0a 2020 2020 2e64 6966  .    }..    .dif
+000020a0: 662d 7374 6174 652d 7375 622d 6865 6164  f-state-sub-head
+000020b0: 6572 7b0a 2020 2020 2020 2020 666f 6e74  er{.        font
+000020c0: 2d66 616d 696c 793a 204f 7065 6e20 5361  -family: Open Sa
+000020d0: 6e73 3b0a 2020 2020 2020 2020 666f 6e74  ns;.        font
+000020e0: 2d73 697a 653a 2031 3470 783b 0a20 2020  -size: 14px;.   
+000020f0: 2020 2020 2066 6f6e 742d 7765 6967 6874       font-weight
+00002100: 3a20 3430 303b 0a20 2020 2020 2020 206c  : 400;.        l
+00002110: 696e 652d 6865 6967 6874 3a20 3139 2e36  ine-height: 19.6
+00002120: 7078 3b0a 2020 2020 2020 2020 7465 7874  px;.        text
+00002130: 2d61 6c69 676e 3a20 6c65 6674 3b0a 2020  -align: left;.  
+00002140: 2020 2020 2020 636f 6c6f 723a 2023 3545        color: #5E
+00002150: 3541 3732 3b0a 2020 2020 7d0a 0a20 2020  5A72;.    }..   
+00002160: 202e 6261 6467 6520 7b0a 2020 2020 2020   .badge {.      
+00002170: 2020 636f 6465 2d74 6578 743b 0a20 2020    code-text;.   
+00002180: 2020 2020 2062 6f72 6465 722d 7261 6469       border-radi
+00002190: 7573 3a20 3330 7078 3b0a 2020 2020 7d0a  us: 30px;.    }.
+000021a0: 0a20 2020 202e 6c61 6265 6c20 7b0a 2020  .    .label {.  
+000021b0: 2020 2020 2020 636f 6465 2d74 6578 743b        code-text;
+000021c0: 0a20 2020 2020 2020 2062 6f72 6465 722d  .        border-
+000021d0: 7261 6469 7573 3a20 3470 783b 0a20 2020  radius: 4px;.   
+000021e0: 2020 2020 2070 6164 6469 6e67 3a20 3670       padding: 6p
+000021f0: 7820 3470 783b 0a20 2020 2020 2020 2077  x 4px;.        w
+00002200: 6869 7465 2d73 7061 6365 3a20 6e6f 7772  hite-space: nowr
+00002210: 6170 3b0a 2020 2020 2020 2020 6f76 6572  ap;.        over
+00002220: 666c 6f77 3a20 6869 6464 656e 3b0a 2020  flow: hidden;.  
+00002230: 2020 2020 2020 6c69 6e65 2d68 6569 6768        line-heigh
+00002240: 743a 2031 2e32 3b0a 2020 2020 2020 2020  t: 1.2;.        
+00002250: 666f 6e74 2d66 616d 696c 793a 206d 6f6e  font-family: mon
+00002260: 6f73 7061 6365 3b0a 2020 2020 7d0a 0a20  ospace;.    }.. 
+00002270: 2020 202e 6c61 6265 6c2d 6c69 6768 742d     .label-light-
+00002280: 7075 7270 6c65 207b 0a20 2020 2020 2020  purple {.       
+00002290: 206c 6162 656c 3b0a 2020 2020 2020 2020   label;.        
+000022a0: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
+000022b0: 3a20 2343 3943 4645 383b 0a20 2020 2020  : #C9CFE8;.     
+000022c0: 2020 2063 6f6c 6f72 3a20 2333 3733 4237     color: #373B7
+000022d0: 423b 0a20 2020 207d 0a0a 2020 2020 2e6c  B;.    }..    .l
+000022e0: 6162 656c 2d6c 6967 6874 2d62 6c75 6520  abel-light-blue 
+000022f0: 7b0a 2020 2020 2020 2020 6c61 6265 6c3b  {.        label;
+00002300: 0a20 2020 2020 2020 2062 6163 6b67 726f  .        backgro
+00002310: 756e 642d 636f 6c6f 723a 2023 4332 4445  und-color: #C2DE
+00002320: 4630 3b0a 2020 2020 2020 2020 636f 6c6f  F0;.        colo
+00002330: 723a 2023 3146 3536 3741 3b0a 2020 2020  r: #1F567A;.    
+00002340: 7d0a 0a20 2020 202e 6c61 6265 6c2d 6f72  }..    .label-or
+00002350: 616e 6765 207b 0a20 2020 2020 2020 2062  ange {.        b
+00002360: 6164 6765 3b0a 2020 2020 2020 2020 6261  adge;.        ba
+00002370: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a20  ckground-color: 
+00002380: 2346 4545 3943 443b 0a20 2020 2020 2020  #FEE9CD;.       
+00002390: 2063 6f6c 6f72 3a20 2342 3835 3230 413b   color: #B8520A;
+000023a0: 0a20 2020 207d 0a0a 2020 2020 2e6c 6162  .    }..    .lab
+000023b0: 656c 2d67 7261 7920 7b0a 2020 2020 2020  el-gray {.      
+000023c0: 2020 6261 6467 653b 0a20 2020 2020 2020    badge;.       
+000023d0: 2062 6163 6b67 726f 756e 642d 636f 6c6f   background-colo
+000023e0: 723a 2023 4543 4542 4546 3b0a 2020 2020  r: #ECEBEF;.    
+000023f0: 2020 2020 636f 6c6f 723a 2023 3335 3332      color: #3532
+00002400: 3433 3b0a 2020 2020 7d0a 0a20 2020 202e  43;.    }..    .
+00002410: 6c61 6265 6c2d 6772 6565 6e20 7b0a 2020  label-green {.  
+00002420: 2020 2020 2020 6261 6467 653b 0a20 2020        badge;.   
+00002430: 2020 2020 2062 6163 6b67 726f 756e 642d       background-
+00002440: 636f 6c6f 723a 2023 4435 4631 4435 3b0a  color: #D5F1D5;.
+00002450: 2020 2020 2020 2020 636f 6c6f 723a 2023          color: #
+00002460: 3235 3642 3234 3b0a 2020 2020 7d0a 0a20  256B24;.    }.. 
+00002470: 2020 202e 6c61 6265 6c2d 7265 6420 7b0a     .label-red {.
+00002480: 2020 2020 2020 2020 6c61 6265 6c3b 0a20          label;. 
+00002490: 2020 2020 2020 2062 6163 6b67 726f 756e         backgroun
+000024a0: 642d 636f 6c6f 723a 2023 4632 4439 4445  d-color: #F2D9DE
+000024b0: 3b0a 2020 2020 2020 2020 636f 6c6f 723a  ;.        color:
+000024c0: 2023 3942 3237 3337 3b0a 2020 2020 7d0a   #9B2737;.    }.
+000024d0: 0a20 2020 202e 6261 6467 652d 626c 7565  .    .badge-blue
+000024e0: 207b 0a20 2020 2020 2020 2062 6164 6765   {.        badge
+000024f0: 3b0a 2020 2020 2020 2020 6261 636b 6772  ;.        backgr
+00002500: 6f75 6e64 2d63 6f6c 6f72 3a20 2343 3244  ound-color: #C2D
+00002510: 4546 303b 0a20 2020 2020 2020 2063 6f6c  EF0;.        col
+00002520: 6f72 3a20 2331 4635 3637 413b 0a20 2020  or: #1F567A;.   
+00002530: 207d 0a0a 2020 2020 2e62 6164 6765 2d70   }..    .badge-p
+00002540: 7572 706c 6520 7b0a 2020 2020 2020 2020  urple {.        
+00002550: 6261 6467 653b 0a20 2020 2020 2020 2062  badge;.        b
+00002560: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
+00002570: 2023 4339 4346 4538 3b0a 2020 2020 2020   #C9CFE8;.      
+00002580: 2020 636f 6c6f 723a 2023 3337 3342 3742    color: #373B7B
+00002590: 3b0a 2020 2020 7d0a 0a20 2020 202e 6261  ;.    }..    .ba
+000025a0: 6467 652d 6772 6565 6e20 7b0a 2020 2020  dge-green {.    
+000025b0: 2020 2020 6261 6467 653b 0a0a 2020 2020      badge;..    
+000025c0: 2020 2020 2f2a 2053 7563 6365 7373 2f43      /* Success/C
+000025d0: 6f6e 7461 696e 6572 202a 2f0a 2020 2020  ontainer */.    
+000025e0: 2020 2020 6261 636b 6772 6f75 6e64 2d63      background-c
+000025f0: 6f6c 6f72 3a20 2344 3546 3144 353b 0a20  olor: #D5F1D5;. 
+00002600: 2020 2020 2020 2063 6f6c 6f72 3a20 2332         color: #2
+00002610: 3536 4232 343b 0a20 2020 207d 0a0a 2020  56B24;.    }..  
+00002620: 2020 2e62 6164 6765 2d72 6564 207b 0a20    .badge-red {. 
+00002630: 2020 2020 2020 2062 6164 6765 3b0a 2020         badge;.  
+00002640: 2020 2020 2020 6261 636b 6772 6f75 6e64        background
+00002650: 2d63 6f6c 6f72 3a20 2346 3244 3944 453b  -color: #F2D9DE;
+00002660: 0a20 2020 2020 2020 2063 6f6c 6f72 3a20  .        color: 
+00002670: 2339 4232 3733 373b 0a20 2020 207d 0a0a  #9B2737;.    }..
+00002680: 2020 2020 2e62 6164 6765 2d67 7261 7920      .badge-gray 
+00002690: 7b0a 2020 2020 2020 2020 6261 6467 653b  {.        badge;
+000026a0: 0a20 2020 2020 2020 2062 6163 6b67 726f  .        backgro
+000026b0: 756e 642d 636f 6c6f 723a 2023 4543 4542  und-color: #ECEB
+000026c0: 4546 3b0a 2020 2020 2020 2020 636f 6c6f  EF;.        colo
+000026d0: 723a 2023 3245 3242 3342 3b0a 2020 2020  r: #2E2B3B;.    
+000026e0: 7d0a 2020 2020 2e70 6167 696e 6174 696f  }.    .paginatio
+000026f0: 6e43 6f6e 7461 696e 6572 7b0a 2020 2020  nContainer{.    
+00002700: 2020 2020 7769 6474 683a 2031 3030 253b      width: 100%;
+00002710: 0a20 2020 2020 2020 202f 2a68 6569 6768  .        /*heigh
+00002720: 743a 2033 3070 783b 2a2f 0a20 2020 2020  t: 30px;*/.     
+00002730: 2020 2064 6973 706c 6179 3a20 666c 6578     display: flex
+00002740: 3b0a 2020 2020 2020 2020 6a75 7374 6966  ;.        justif
+00002750: 792d 636f 6e74 656e 743a 2063 656e 7465  y-content: cente
+00002760: 723b 0a20 2020 2020 2020 2067 6170 3a20  r;.        gap: 
+00002770: 3870 783b 0a20 2020 2020 2020 2070 6164  8px;.        pad
+00002780: 6469 6e67 3a20 3570 783b 0a20 2020 2020  ding: 5px;.     
+00002790: 2020 2063 6f6c 6f72 3a20 7661 7228 2d2d     color: var(--
+000027a0: 7465 7274 6961 7279 2d63 6f6c 6f72 293b  tertiary-color);
+000027b0: 0a20 2020 207d 0a0a 2020 2020 2e77 6964  .    }..    .wid
+000027c0: 6765 742d 6c61 6265 6c2d 6261 7369 637b  get-label-basic{
+000027d0: 0a20 2020 2020 2020 2064 6973 706c 6179  .        display
+000027e0: 3a66 6c65 783b 0a20 2020 207d 0a0a 2020  :flex;.    }..  
+000027f0: 2020 2e77 6964 6765 742d 6c61 6265 6c2d    .widget-label-
+00002800: 6261 7369 6320 696e 7075 745b 7479 7065  basic input[type
+00002810: 3d27 6368 6563 6b62 6f78 275d 5b64 6973  ='checkbox'][dis
+00002820: 6162 6c65 645d 207b 0a20 2020 2020 2020  abled] {.       
+00002830: 2066 696c 7465 723a 2073 6570 6961 2830   filter: sepia(0
+00002840: 2e33 2920 6875 652d 726f 7461 7465 2836  .3) hue-rotate(6
+00002850: 3764 6567 2920 7361 7475 7261 7465 2833  7deg) saturate(3
+00002860: 293b 0a20 2020 207d 0a0a 2020 2020 2e70  );.    }..    .p
+00002870: 6167 657b 0a20 2020 2020 2020 2063 6f6c  age{.        col
+00002880: 6f72 3a20 626c 6163 6b3b 0a20 2020 2020  or: black;.     
+00002890: 2020 2066 6f6e 742d 7765 6967 6874 3a20     font-weight: 
+000028a0: 626f 6c64 3b0a 2020 2020 2020 2020 636f  bold;.        co
+000028b0: 6c6f 723a 2076 6172 282d 2d74 6572 7469  lor: var(--terti
+000028c0: 6172 792d 636f 6c6f 7229 3b0a 2020 2020  ary-color);.    
+000028d0: 7d0a 2020 2020 2e70 6167 653a 686f 7665  }.    .page:hove
+000028e0: 7220 7b0a 2020 2020 2020 636f 6c6f 723a  r {.      color:
+000028f0: 2023 3338 6264 6638 3b0a 2020 2020 2020   #38bdf8;.      
+00002900: 6375 7273 6f72 3a20 706f 696e 7465 723b  cursor: pointer;
+00002910: 0a20 2020 207d 0a20 2020 202e 636c 6970  .    }.    .clip
+00002920: 626f 6172 643a 686f 7665 727b 0a20 2020  board:hover{.   
+00002930: 2020 2020 2063 7572 736f 723a 2070 6f69       cursor: poi
+00002940: 6e74 6572 3b0a 2020 2020 2020 2020 636f  nter;.        co
+00002950: 6c6f 723a 2076 6172 282d 2d74 6572 7469  lor: var(--terti
+00002960: 6172 792d 636f 6c6f 7229 3b0a 2020 2020  ary-color);.    
+00002970: 7d0a 0a20 2020 202e 7265 6e64 6572 6564  }..    .rendered
+00002980: 5f68 746d 6c20 7462 6f64 7920 7472 3a6e  _html tbody tr:n
+00002990: 7468 2d63 6869 6c64 286f 6464 2920 7b0a  th-child(odd) {.
+000029a0: 2020 2020 2020 2020 6261 636b 6772 6f75          backgrou
+000029b0: 6e64 3a20 7472 616e 7370 6172 656e 743b  nd: transparent;
+000029c0: 0a20 2020 207d 0a0a 2020 2020 2e73 6561  .    }..    .sea
+000029d0: 7263 682d 6669 656c 6420 7b0a 2020 2020  rch-field {.    
+000029e0: 2020 2020 6469 7370 6c61 793a 2066 6c65      display: fle
+000029f0: 783b 0a20 2020 2020 2020 2061 6c69 676e  x;.        align
+00002a00: 2d69 7465 6d73 3a20 6365 6e74 6572 3b0a  -items: center;.
+00002a10: 2020 2020 2020 2020 626f 7264 6572 2d72          border-r
+00002a20: 6164 6975 733a 2033 3070 783b 0a20 2020  adius: 30px;.   
+00002a30: 2020 2020 2062 6163 6b67 726f 756e 642d       background-
+00002a40: 636f 6c6f 723a 2076 6172 282d 2d73 6563  color: var(--sec
+00002a50: 6f6e 6461 7279 2d63 6f6c 6f72 293b 0a20  ondary-color);. 
+00002a60: 2020 207d 0a0a 2020 2020 2e73 7966 742d     }..    .syft-
+00002a70: 6472 6f70 646f 776e 207b 0a20 2020 2020  dropdown {.     
+00002a80: 2020 206d 6172 6769 6e3a 2035 7078 3b0a     margin: 5px;.
+00002a90: 2020 2020 2020 2020 6d61 7267 696e 2d6c          margin-l
+00002aa0: 6566 743a 2035 7078 3b0a 2020 2020 2020  eft: 5px;.      
+00002ab0: 2020 706f 7369 7469 6f6e 3a20 7265 6c61    position: rela
+00002ac0: 7469 7665 3b0a 2020 2020 2020 2020 6469  tive;.        di
+00002ad0: 7370 6c61 793a 2069 6e6c 696e 652d 626c  splay: inline-bl
+00002ae0: 6f63 6b3b 0a20 2020 2020 2020 2074 6578  ock;.        tex
+00002af0: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00002b00: 0a20 2020 2020 2020 2062 6163 6b67 726f  .        backgro
+00002b10: 756e 642d 636f 6c6f 723a 2076 6172 282d  und-color: var(-
+00002b20: 2d62 7574 746f 6e2d 636f 6c6f 7229 3b0a  -button-color);.
+00002b30: 2020 2020 2020 2020 6d69 6e2d 7769 6474          min-widt
+00002b40: 683a 2031 3030 7078 3b0a 2020 2020 2020  h: 100px;.      
+00002b50: 2020 7061 6464 696e 673a 2032 7078 3b0a    padding: 2px;.
+00002b60: 2020 2020 2020 2020 626f 7264 6572 2d72          border-r
+00002b70: 6164 6975 733a 2033 3070 783b 0a20 2020  adius: 30px;.   
+00002b80: 207d 0a0a 2020 2020 2e73 7966 742d 6472   }..    .syft-dr
+00002b90: 6f70 646f 776e 3a68 6f76 6572 207b 0a20  opdown:hover {. 
+00002ba0: 2020 2020 2020 2063 7572 736f 723a 2070         cursor: p
+00002bb0: 6f69 6e74 6572 3b0a 2020 2020 7d0a 2020  ointer;.    }.  
+00002bc0: 2020 2e73 7966 742d 6472 6f70 646f 776e    .syft-dropdown
+00002bd0: 2d63 6f6e 7465 6e74 207b 0a20 2020 2020  -content {.     
+00002be0: 2020 206d 6172 6769 6e2d 746f 703a 3236     margin-top:26
+00002bf0: 7078 3b0a 2020 2020 2020 2020 6469 7370  px;.        disp
+00002c00: 6c61 793a 206e 6f6e 653b 0a20 2020 2020  lay: none;.     
+00002c10: 2020 2070 6f73 6974 696f 6e3a 2061 6273     position: abs
+00002c20: 6f6c 7574 653b 0a20 2020 2020 2020 206d  olute;.        m
+00002c30: 696e 2d77 6964 7468 3a20 3130 3070 783b  in-width: 100px;
+00002c40: 0a20 2020 2020 2020 2062 6f78 2d73 6861  .        box-sha
+00002c50: 646f 773a 2030 7078 2038 7078 2031 3670  dow: 0px 8px 16p
+00002c60: 7820 3070 7820 7267 6261 2830 2c30 2c30  x 0px rgba(0,0,0
+00002c70: 2c30 2e32 293b 0a20 2020 2020 2020 2070  ,0.2);.        p
+00002c80: 6164 6469 6e67 3a20 3132 7078 2036 7078  adding: 12px 6px
+00002c90: 3b0a 2020 2020 2020 2020 7a2d 696e 6465  ;.        z-inde
+00002ca0: 783a 2031 3b0a 2020 2020 2020 2020 6261  x: 1;.        ba
+00002cb0: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a20  ckground-color: 
+00002cc0: 7661 7228 2d2d 7072 696d 6172 792d 636f  var(--primary-co
+00002cd0: 6c6f 7229 3b0a 2020 2020 2020 2020 636f  lor);.        co
+00002ce0: 6c6f 723a 2076 6172 282d 2d74 6572 7469  lor: var(--terti
+00002cf0: 6172 792d 636f 6c6f 7229 3b0a 2020 2020  ary-color);.    
+00002d00: 7d0a 2020 2020 2e64 642d 6f70 7469 6f6e  }.    .dd-option
+00002d10: 7320 7b0a 2020 2020 2020 2020 7061 6464  s {.        padd
+00002d20: 696e 672d 746f 703a 2034 7078 3b0a 2020  ing-top: 4px;.  
+00002d30: 2020 7d0a 2020 2020 2e64 642d 6f70 7469    }.    .dd-opti
+00002d40: 6f6e 733a 6669 7273 742d 6f66 2d74 7970  ons:first-of-typ
+00002d50: 6520 7b0a 2020 2020 2020 2020 7061 6464  e {.        padd
+00002d60: 696e 672d 746f 703a 2030 7078 3b0a 2020  ing-top: 0px;.  
+00002d70: 2020 7d0a 0a20 2020 202e 6464 2d6f 7074    }..    .dd-opt
+00002d80: 696f 6e73 3a68 6f76 6572 207b 0a20 2020  ions:hover {.   
+00002d90: 2020 2020 2063 7572 736f 723a 2070 6f69       cursor: poi
+00002da0: 6e74 6572 3b0a 2020 2020 2020 2020 6261  nter;.        ba
+00002db0: 636b 6772 6f75 6e64 3a20 2364 3164 3564  ckground: #d1d5d
+00002dc0: 623b 0a20 2020 207d 0a20 2020 202e 6172  b;.    }.    .ar
+00002dd0: 726f 7720 7b0a 2020 2020 2020 2020 626f  row {.        bo
+00002de0: 7264 6572 3a20 736f 6c69 6420 626c 6163  rder: solid blac
+00002df0: 6b3b 0a20 2020 2020 2020 2062 6f72 6465  k;.        borde
+00002e00: 722d 7769 6474 683a 2030 2033 7078 2033  r-width: 0 3px 3
+00002e10: 7078 2030 3b0a 2020 2020 2020 2020 6469  px 0;.        di
+00002e20: 7370 6c61 793a 2069 6e6c 696e 652d 626c  splay: inline-bl
+00002e30: 6f63 6b3b 0a20 2020 2020 2020 2070 6164  ock;.        pad
+00002e40: 6469 6e67 3a20 3370 783b 0a20 2020 207d  ding: 3px;.    }
+00002e50: 0a20 2020 202e 646f 776e 207b 0a20 2020  .    .down {.   
+00002e60: 2020 2020 2074 7261 6e73 666f 726d 3a20       transform: 
+00002e70: 726f 7461 7465 2834 3564 6567 293b 0a20  rotate(45deg);. 
+00002e80: 2020 2020 2020 202d 7765 626b 6974 2d74         -webkit-t
+00002e90: 7261 6e73 666f 726d 3a20 726f 7461 7465  ransform: rotate
+00002ea0: 2834 3564 6567 293b 0a20 2020 207d 0a3c  (45deg);.    }.<
+00002eb0: 2f73 7479 6c65 3e0a 0a22 2222 0a0a 4353  /style>.."""..CS
+00002ec0: 535f 434f 4445 203d 2066 2222 220a 7b43  S_CODE = f""".{C
+00002ed0: 5353 7d0a 2222 220a 0a53 4541 5243 485f  SS}."""..SEARCH_
+00002ee0: 4943 4f4e 203d 2028 0a20 2020 2027 3c73  ICON = (.    '<s
+00002ef0: 7667 2077 6964 7468 3d22 3131 2220 6865  vg width="11" he
+00002f00: 6967 6874 3d22 3130 2220 7669 6577 426f  ight="10" viewBo
+00002f10: 783d 2230 2030 2031 3120 3130 2220 6669  x="0 0 11 10" fi
+00002f20: 6c6c 3d22 6e6f 6e65 2227 0a20 2020 2027  ll="none"'.    '
+00002f30: 2078 6d6c 6e73 3d22 6874 7470 3a2f 2f77   xmlns="http://w
+00002f40: 7777 2e77 332e 6f72 672f 3230 3030 2f73  ww.w3.org/2000/s
+00002f50: 7667 223e 3c70 6174 6820 643d 224d 3130  vg"><path d="M10
+00002f60: 2e35 3635 3220 392e 3233 3436 374c 382e  .5652 9.23467L8.
+00002f70: 3231 3831 3927 0a20 2020 2022 2036 2e38  21819'.    " 6.8
+00002f80: 3838 3131 4338 2e38 3938 3436 2036 2e30  8811C8.89846 6.0
+00002f90: 3731 3431 2039 2e32 3337 3637 2035 2e30  7141 9.23767 5.0
+00002fa0: 3233 3839 2039 2e31 3635 3237 2033 2e39  2389 9.16527 3.9
+00002fb0: 3633 3435 4339 2e30 3932 3837 2032 2e39  6345C9.09287 2.9
+00002fc0: 3033 3032 2038 2e36 3134 3433 220a 2020  0302 8.61443".  
+00002fd0: 2020 2220 312e 3931 3133 3220 372e 3832    " 1.91132 7.82
+00002fe0: 3934 3820 312e 3139 3436 3643 372e 3034  948 1.19466C7.04
+00002ff0: 3435 3320 302e 3437 3739 3935 2036 2e30  453 0.477995 6.0
+00003000: 3133 3439 2030 2e30 3931 3534 3134 2034  1349 0.0915414 4
+00003010: 2e39 3530 3837 220a 2020 2020 2220 302e  .95087".    " 0.
+00003020: 3131 3536 3931 4333 2e38 3838 3234 2030  115691C3.88824 0
+00003030: 2e31 3339 3834 3120 322e 3837 3538 3320  .139841 2.87583 
+00003040: 302e 3537 3237 3335 2032 2e31 3234 3235  0.572735 2.12425
+00003050: 2031 2e33 3234 3332 4331 2e33 3732 3636   1.32432C1.37266
+00003060: 2032 2e30 3735 3922 0a20 2020 2022 2030   2.0759".    " 0
+00003070: 2e39 3339 3736 3820 332e 3038 3833 3120  .939768 3.08831 
+00003080: 302e 3931 3536 3138 2034 2e31 3530 3934  0.915618 4.15094
+00003090: 4330 2e38 3931 3436 3820 352e 3231 3335  C0.891468 5.2135
+000030a0: 3720 312e 3237 3739 3220 362e 3234 3436  7 1.27792 6.2446
+000030b0: 2031 2e39 3934 3539 220a 2020 2020 2220   1.99459".    " 
+000030c0: 372e 3032 3935 3543 322e 3731 3132 3520  7.02955C2.71125 
+000030d0: 372e 3831 3435 2033 2e37 3032 3935 2038  7.8145 3.70295 8
+000030e0: 2e32 3932 3934 2034 2e37 3633 3338 2038  .29294 4.76338 8
+000030f0: 2e33 3635 3335 4335 2e38 3233 3831 2038  .36535C5.82381 8
+00003100: 2e34 3337 3735 2036 2e38 3731 3334 220a  .43775 6.87134".
+00003110: 2020 2020 2220 382e 3039 3835 3320 372e      " 8.09853 7.
+00003120: 3638 3830 3420 372e 3431 3832 374c 3130  68804 7.41827L10
+00003130: 2e30 3334 3620 392e 3736 3533 4331 302e  .0346 9.7653C10.
+00003140: 3036 3934 2039 2e38 3030 3134 2031 302e  0694 9.80014 10.
+00003150: 3131 3038 2039 2e38 3237 3738 2031 302e  1108 9.82778 10.
+00003160: 3135 3633 220a 2020 2020 2220 392e 3834  1563".    " 9.84
+00003170: 3636 3343 3130 2e32 3031 3820 392e 3836  663C10.2018 9.86
+00003180: 3534 3920 3130 2e32 3530 3620 392e 3837  549 10.2506 9.87
+00003190: 3531 3920 3130 2e32 3939 3920 392e 3837  519 10.2999 9.87
+000031a0: 3531 3943 3130 2e33 3439 3220 392e 3837  519C10.3492 9.87
+000031b0: 3531 3920 3130 2e33 3938 220a 2020 2020  519 10.398".    
+000031c0: 2220 392e 3836 3534 3920 3130 2e34 3433  " 9.86549 10.443
+000031d0: 3520 392e 3834 3636 3343 3130 2e34 3839  5 9.84663C10.489
+000031e0: 2039 2e38 3237 3738 2031 302e 3533 3034   9.82778 10.5304
+000031f0: 2039 2e38 3030 3134 2031 302e 3536 3532   9.80014 10.5652
+00003200: 2039 2e37 3635 3343 3130 2e36 3030 3122   9.7653C10.6001"
+00003210: 0a20 2020 2022 2039 2e37 3330 3436 2031  .    " 9.73046 1
+00003220: 302e 3632 3737 2039 2e36 3839 3039 2031  0.6277 9.68909 1
+00003230: 302e 3634 3636 2039 2e36 3433 3537 4331  0.6466 9.64357C1
+00003240: 302e 3636 3534 2039 2e35 3938 3035 2031  0.6654 9.59805 1
+00003250: 302e 3637 3531 2039 2e35 3439 3236 2031  0.6751 9.54926 1
+00003260: 302e 3637 3531 220a 2020 2020 2220 392e  0.6751".    " 9.
+00003270: 3439 3939 3843 3130 2e36 3735 3120 392e  49998C10.6751 9.
+00003280: 3435 3037 3120 3130 2e36 3635 3420 392e  45071 10.6654 9.
+00003290: 3430 3139 3220 3130 2e36 3436 3620 392e  40192 10.6466 9.
+000032a0: 3335 3634 4331 302e 3632 3737 2039 2e33  3564C10.6277 9.3
+000032b0: 3130 3838 2031 302e 3630 3031 220a 2020  1088 10.6001".  
+000032c0: 2020 2220 392e 3236 3935 3120 3130 2e35    " 9.26951 10.5
+000032d0: 3635 3220 392e 3233 3436 375a 4d31 2e36  652 9.23467ZM1.6
+000032e0: 3734 3931 2034 2e32 3439 3938 4331 2e36  7491 4.24998C1.6
+000032f0: 3734 3931 2033 2e35 3832 3437 2031 2e38  7491 3.58247 1.8
+00003300: 3732 3835 2032 2e39 3239 3935 2032 2e32  7285 2.92995 2.2
+00003310: 3433 3722 0a20 2020 2022 2032 2e33 3734  437".    " 2.374
+00003320: 3933 4332 2e36 3134 3535 2031 2e38 3139  93C2.61455 1.819
+00003330: 3932 2033 2e31 3431 3635 2031 2e33 3837  92 3.14165 1.387
+00003340: 3334 2033 2e37 3538 3335 2031 2e31 3331  34 3.75835 1.131
+00003350: 3839 4334 2e33 3735 3036 2030 2e38 3736  89C4.37506 0.876
+00003360: 3434 3620 352e 3035 3336 3622 0a20 2020  446 5.05366".   
+00003370: 2022 2030 2e38 3039 3630 3920 352e 3730   " 0.809609 5.70
+00003380: 3833 3420 302e 3933 3938 3335 4336 2e33  834 0.939835C6.3
+00003390: 3633 3033 2031 2e30 3730 3036 2036 2e39  6303 1.07006 6.9
+000033a0: 3634 3339 2031 2e33 3931 3520 372e 3433  6439 1.3915 7.43
+000033b0: 3634 2031 2e38 3633 3543 372e 3930 3834  64 1.8635C7.9084
+000033c0: 220a 2020 2020 2220 322e 3333 3535 2038  ".    " 2.3355 8
+000033d0: 2e32 3239 3834 2032 2e39 3336 3837 2038  .22984 2.93687 8
+000033e0: 2e33 3630 3036 2033 2e35 3931 3535 4338  .36006 3.59155C8
+000033f0: 2e34 3930 3239 2034 2e32 3436 3234 2038  .49029 4.24624 8
+00003400: 2e34 3233 3435 2034 2e39 3234 3834 2038  .42345 4.92484 8
+00003410: 2e31 3638 220a 2020 2020 2220 352e 3534  .168".    " 5.54
+00003420: 3135 3443 372e 3931 3235 3620 362e 3135  154C7.91256 6.15
+00003430: 3832 3420 372e 3437 3939 3820 362e 3638  824 7.47998 6.68
+00003440: 3533 3520 362e 3932 3439 3620 372e 3035  535 6.92496 7.05
+00003450: 3631 3943 362e 3336 3939 3520 372e 3432  619C6.36995 7.42
+00003460: 3730 3420 352e 3731 3734 3222 0a20 2020  704 5.71742".   
+00003470: 2022 2037 2e36 3234 3938 2035 2e30 3439   " 7.62498 5.049
+00003480: 3931 2037 2e36 3234 3938 4334 2e31 3535  91 7.62498C4.155
+00003490: 3131 2037 2e36 3233 3939 2033 2e32 3937  11 7.62399 3.297
+000034a0: 3234 2037 2e32 3638 3039 2032 2e36 3634  24 7.26809 2.664
+000034b0: 3532 2036 2e36 3335 3337 4332 2e30 3331  52 6.63537C2.031
+000034c0: 3822 0a20 2020 2027 2036 2e30 3032 3635  8".    ' 6.00265
+000034d0: 2031 2e36 3735 3920 352e 3134 3437 3920   1.6759 5.14479 
+000034e0: 312e 3637 3439 3120 342e 3234 3939 385a  1.67491 4.24998Z
+000034f0: 2220 6669 6c6c 3d22 6375 7272 656e 7443  " fill="currentC
+00003500: 6f6c 6f72 222f 3e3c 2f73 7667 3e27 0a29  olor"/></svg>'.)
+00003510: 0a43 4c49 5042 4f41 5244 5f49 434f 4e20  .CLIPBOARD_ICON 
+00003520: 3d20 280a 2020 2020 223c 7376 6720 7769  = (.    "<svg wi
+00003530: 6474 683d 2738 2720 6865 6967 6874 3d27  dth='8' height='
+00003540: 3827 2076 6965 7742 6f78 3d27 3020 3020  8' viewBox='0 0 
+00003550: 3820 3827 2066 696c 6c3d 276e 6f6e 6527  8 8' fill='none'
+00003560: 220a 2020 2020 2220 786d 6c6e 733d 2768  ".    " xmlns='h
+00003570: 7474 703a 2f2f 7777 772e 7733 2e6f 7267  ttp://www.w3.org
+00003580: 2f32 3030 302f 7376 6727 3e3c 7061 7468  /2000/svg'><path
+00003590: 2064 3d27 4d37 2e34 3337 3520 302e 3235   d='M7.4375 0.25
+000035a0: 4832 2e34 3337 3543 322e 3335 3436 3220  H2.4375C2.35462 
+000035b0: 302e 3235 220a 2020 2020 2220 322e 3237  0.25".    " 2.27
+000035c0: 3531 3320 302e 3238 3239 3234 2032 2e32  513 0.282924 2.2
+000035d0: 3136 3533 2030 2e33 3431 3532 3943 322e  1653 0.341529C2.
+000035e0: 3135 3739 3220 302e 3430 3031 3334 2032  15792 0.400134 2
+000035f0: 2e31 3235 2030 2e34 3739 3632 2032 2e31  .125 0.47962 2.1
+00003600: 3235 220a 2020 2020 2220 302e 3536 3235  25".    " 0.5625
+00003610: 5632 2e31 3235 4830 2e35 3632 3543 302e  V2.125H0.5625C0.
+00003620: 3437 3936 3220 322e 3132 3520 302e 3430  47962 2.125 0.40
+00003630: 3031 3334 2032 2e31 3537 3932 2030 2e33  0134 2.15792 0.3
+00003640: 3431 3532 3920 322e 3231 3635 3343 302e  41529 2.21653C0.
+00003650: 3238 3239 3234 220a 2020 2020 2220 322e  282924".    " 2.
+00003660: 3237 3531 3320 302e 3235 2032 2e33 3534  27513 0.25 2.354
+00003670: 3632 2030 2e32 3520 322e 3433 3735 5637  62 0.25 2.4375V7
+00003680: 2e34 3337 3543 302e 3235 2037 2e35 3230  .4375C0.25 7.520
+00003690: 3338 2030 2e32 3832 3932 3420 372e 3539  38 0.282924 7.59
+000036a0: 3938 3720 302e 3334 3135 3239 220a 2020  987 0.341529".  
+000036b0: 2020 2220 372e 3635 3834 3743 302e 3430    " 7.65847C0.40
+000036c0: 3031 3334 2037 2e37 3137 3038 2030 2e34  0134 7.71708 0.4
+000036d0: 3739 3632 2037 2e37 3520 302e 3536 3235  7962 7.75 0.5625
+000036e0: 2037 2e37 3548 352e 3536 3235 4335 2e36   7.75H5.5625C5.6
+000036f0: 3435 3338 2037 2e37 3520 352e 3732 3438  4538 7.75 5.7248
+00003700: 3722 0a20 2020 2022 2037 2e37 3137 3038  7".    " 7.71708
+00003710: 2035 2e37 3833 3437 2037 2e36 3538 3437   5.78347 7.65847
+00003720: 4335 2e38 3432 3038 2037 2e35 3939 3837  C5.84208 7.59987
+00003730: 2035 2e38 3735 2037 2e35 3230 3338 2035   5.875 7.52038 5
+00003740: 2e38 3735 220a 2020 2020 2220 372e 3433  .875".    " 7.43
+00003750: 3735 5635 2e38 3735 4837 2e34 3337 3543  75V5.875H7.4375C
+00003760: 372e 3532 3033 3820 352e 3837 3520 372e  7.52038 5.875 7.
+00003770: 3539 3938 3720 352e 3834 3230 3820 372e  59987 5.84208 7.
+00003780: 3635 3834 3720 352e 3738 3334 3743 372e  65847 5.78347C7.
+00003790: 3731 3730 3820 352e 3732 3438 3722 0a20  71708 5.72487". 
+000037a0: 2020 2022 2037 2e37 3520 352e 3634 3533     " 7.75 5.6453
+000037b0: 3820 372e 3735 2035 2e35 3632 3556 302e  8 7.75 5.5625V0.
+000037c0: 3536 3235 4337 2e37 3520 302e 3437 3936  5625C7.75 0.4796
+000037d0: 3220 372e 3731 3730 3820 302e 3430 3031  2 7.71708 0.4001
+000037e0: 3334 2037 2e36 3538 3437 220a 2020 2020  34 7.65847".    
+000037f0: 2220 302e 3334 3135 3239 4337 2e35 3939  " 0.341529C7.599
+00003800: 3837 2030 2e32 3832 3932 3420 372e 3532  87 0.282924 7.52
+00003810: 3033 3820 302e 3235 2037 2e34 3337 3520  038 0.25 7.4375 
+00003820: 302e 3235 5a4d 352e 3235 220a 2020 2020  0.25ZM5.25".    
+00003830: 2220 372e 3132 3548 302e 3837 3556 322e  " 7.125H0.875V2.
+00003840: 3735 4835 2e32 3556 372e 3132 355a 4d37  75H5.25V7.125ZM7
+00003850: 2e31 3235 2035 2e32 3548 352e 3837 3556  .125 5.25H5.875V
+00003860: 322e 3433 3735 4335 2e38 3735 2032 2e33  2.4375C5.875 2.3
+00003870: 3534 3632 2035 2e38 3432 3038 220a 2020  5462 5.84208".  
+00003880: 2020 2220 322e 3237 3531 3320 352e 3738    " 2.27513 5.78
+00003890: 3334 3720 322e 3231 3635 3343 352e 3732  347 2.21653C5.72
+000038a0: 3438 3720 322e 3135 3739 3220 352e 3634  487 2.15792 5.64
+000038b0: 3533 3820 322e 3132 3520 352e 3536 3235  538 2.125 5.5625
+000038c0: 220a 2020 2020 2220 322e 3132 3548 322e  ".    " 2.125H2.
+000038d0: 3735 5630 2e38 3735 4837 2e31 3235 5635  75V0.875H7.125V5
+000038e0: 2e32 355a 2720 6669 6c6c 3d27 2334 3634  .25Z' fill='#464
+000038f0: 3135 3827 2f3e 3c2f 7376 673e 220a 290a  158'/></svg>".).
+00003900: 5441 424c 455f 4943 4f4e 203d 2028 0a20  TABLE_ICON = (. 
+00003910: 2020 2027 3c73 7667 2077 6964 7468 3d22     '<svg width="
+00003920: 3332 2220 6865 6967 6874 3d22 3332 2220  32" height="32" 
+00003930: 7669 6577 426f 783d 2230 2030 2033 3220  viewBox="0 0 32 
+00003940: 3332 2220 6669 6c6c 3d22 6e6f 6e65 2227  32" fill="none"'
+00003950: 0a20 2020 2027 2078 6d6c 6e73 3d22 6874  .    ' xmlns="ht
+00003960: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
+00003970: 3230 3030 2f73 7667 223e 203c 7061 7468  2000/svg"> <path
+00003980: 2064 3d22 4d32 3820 3648 3443 332e 3733   d="M28 6H4C3.73
+00003990: 3437 3820 3620 332e 3438 3034 3320 362e  478 6 3.48043 6.
+000039a0: 3130 3533 3627 0a20 2020 2022 2033 2e32  10536'.    " 3.2
+000039b0: 3932 3839 2036 2e32 3932 3839 4333 2e31  9289 6.29289C3.1
+000039c0: 3035 3336 2036 2e34 3830 3433 2033 2036  0536 6.48043 3 6
+000039d0: 2e37 3334 3738 2033 2037 5632 3443 3320  .73478 3 7V24C3 
+000039e0: 3234 2e35 3330 3420 332e 3231 3037 3120  24.5304 3.21071 
+000039f0: 3235 2e30 3339 3122 0a20 2020 2022 2033  25.0391".    " 3
+00003a00: 2e35 3835 3739 2032 352e 3431 3432 4333  .58579 25.4142C3
+00003a10: 2e39 3630 3836 2032 352e 3738 3933 2034  .96086 25.7893 4
+00003a20: 2e34 3639 3537 2032 3620 3520 3236 4832  .46957 26 5 26H2
+00003a30: 3743 3237 2e35 3330 3420 3236 2032 382e  7C27.5304 26 28.
+00003a40: 3033 3931 2032 352e 3738 3933 220a 2020  0391 25.7893".  
+00003a50: 2020 2220 3238 2e34 3134 3220 3235 2e34    " 28.4142 25.4
+00003a60: 3134 3243 3238 2e37 3839 3320 3235 2e30  142C28.7893 25.0
+00003a70: 3339 3120 3239 2032 342e 3533 3034 2032  391 29 24.5304 2
+00003a80: 3920 3234 5637 4332 3920 362e 3733 3437  9 24V7C29 6.7347
+00003a90: 3820 3238 2e38 3934 3620 362e 3438 3034  8 28.8946 6.4804
+00003aa0: 3322 0a20 2020 2022 2032 382e 3730 3731  3".    " 28.7071
+00003ab0: 2036 2e32 3932 3839 4332 382e 3531 3936   6.29289C28.5196
+00003ac0: 2036 2e31 3035 3336 2032 382e 3236 3532   6.10536 28.2652
+00003ad0: 2036 2032 3820 365a 4d35 2031 3448 3130   6 28 6ZM5 14H10
+00003ae0: 5631 3848 3556 3134 5a4d 3132 220a 2020  V18H5V14ZM12".  
+00003af0: 2020 2720 3134 4832 3756 3138 4831 3256    ' 14H27V18H12V
+00003b00: 3134 5a4d 3237 2038 5631 3248 3556 3848  14ZM27 8V12H5V8H
+00003b10: 3237 5a4d 3520 3230 4831 3056 3234 4835  27ZM5 20H10V24H5
+00003b20: 5632 305a 4d32 3720 3234 4831 3256 3230  V20ZM27 24H12V20
+00003b30: 4832 3756 3234 5a22 270a 2020 2020 2720  H27V24Z"'.    ' 
+00003b40: 6669 6c6c 3d22 2333 3433 3333 3022 2f3e  fill="#343330"/>
+00003b50: 3c2f 7376 673e 270a 290a 464f 4c44 4552  </svg>'.).FOLDER
+00003b60: 5f49 434f 4e20 3d20 280a 2020 2020 273c  _ICON = (.    '<
+00003b70: 7376 6720 7769 6474 683d 2233 3222 2020  svg width="32"  
+00003b80: 6865 6967 6874 3d22 3332 2220 7669 6577  height="32" view
+00003b90: 426f 783d 2230 2030 2031 3420 3132 2220  Box="0 0 14 12" 
+00003ba0: 6669 6c6c 3d22 6e6f 6e65 2227 0a20 2020  fill="none"'.   
+00003bb0: 2027 2078 6d6c 6e73 3d22 6874 7470 3a2f   ' xmlns="http:/
+00003bc0: 2f77 7777 2e77 332e 6f72 672f 3230 3030  /www.w3.org/2000
+00003bd0: 2f73 7667 223e 3c70 6174 6820 643d 224d  /svg"><path d="M
+00003be0: 3133 2032 4838 2e36 3636 3837 4c36 2e39  13 2H8.66687L6.9
+00003bf0: 3333 3133 2030 2e37 4336 2e37 3539 3738  3313 0.7C6.75978
+00003c00: 270a 2020 2020 2220 302e 3537 3036 3620  '.    " 0.57066 
+00003c10: 362e 3534 3934 3120 302e 3530 3035 3336  6.54941 0.500536
+00003c20: 2036 2e33 3333 3133 2030 2e35 4833 2e35   6.33313 0.5H3.5
+00003c30: 4333 2e32 3334 3738 2030 2e35 2032 2e39  C3.23478 0.5 2.9
+00003c40: 3830 3433 2030 2e36 3035 3335 3720 322e  8043 0.605357 2.
+00003c50: 3739 3238 3922 0a20 2020 2022 2030 2e37  79289".    " 0.7
+00003c60: 3932 3839 3343 322e 3630 3533 3620 302e  92893C2.60536 0.
+00003c70: 3938 3034 3320 322e 3520 312e 3233 3437  98043 2.5 1.2347
+00003c80: 3820 322e 3520 312e 3556 322e 3548 312e  8 2.5 1.5V2.5H1.
+00003c90: 3543 312e 3233 3437 3820 322e 3520 302e  5C1.23478 2.5 0.
+00003ca0: 3938 3034 3320 322e 3630 3533 3622 0a20  98043 2.60536". 
+00003cb0: 2020 2022 2030 2e37 3932 3839 3320 322e     " 0.792893 2.
+00003cc0: 3739 3238 3943 302e 3630 3533 3537 2032  79289C0.605357 2
+00003cd0: 2e39 3830 3433 2030 2e35 2033 2e32 3334  .98043 0.5 3.234
+00003ce0: 3738 2030 2e35 2033 2e35 5631 302e 3543  78 0.5 3.5V10.5C
+00003cf0: 302e 3520 3130 2e37 3635 3220 302e 3630  0.5 10.7652 0.60
+00003d00: 3533 3537 220a 2020 2020 2220 3131 2e30  5357".    " 11.0
+00003d10: 3139 3620 302e 3739 3238 3933 2031 312e  196 0.792893 11.
+00003d20: 3230 3731 4330 2e39 3830 3433 2031 312e  2071C0.98043 11.
+00003d30: 3339 3436 2031 2e32 3334 3738 2031 312e  3946 1.23478 11.
+00003d40: 3520 312e 3520 3131 2e35 4831 312e 3035  5 1.5 11.5H11.05
+00003d50: 3536 4331 312e 3330 3622 0a20 2020 2022  56C11.306".    "
+00003d60: 2031 312e 3439 3937 2031 312e 3534 3620   11.4997 11.546 
+00003d70: 3131 2e34 3030 3120 3131 2e37 3233 2031  11.4001 11.723 1
+00003d80: 312e 3232 3343 3131 2e39 3030 3120 3131  1.223C11.9001 11
+00003d90: 2e30 3436 2031 312e 3939 3937 2031 302e  .046 11.9997 10.
+00003da0: 3830 3620 3132 220a 2020 2020 2220 3130  806 12".    " 10
+00003db0: 2e35 3535 3656 392e 3548 3133 2e30 3535  .5556V9.5H13.055
+00003dc0: 3643 3133 2e33 3036 2039 2e34 3939 3637  6C13.306 9.49967
+00003dd0: 2031 332e 3534 3620 392e 3430 3030 3720   13.546 9.40007 
+00003de0: 3133 2e37 3233 2039 2e32 3233 3033 4331  13.723 9.22303C1
+00003df0: 332e 3930 3031 2039 2e30 3436 220a 2020  3.9001 9.046".  
+00003e00: 2020 2220 3133 2e39 3939 3720 382e 3830    " 13.9997 8.80
+00003e10: 3539 3920 3134 2038 2e35 3535 3632 5633  599 14 8.55562V3
+00003e20: 4331 3420 322e 3733 3437 3820 3133 2e38  C14 2.73478 13.8
+00003e30: 3934 3620 322e 3438 3034 3320 3133 2e37  946 2.48043 13.7
+00003e40: 3037 3120 322e 3239 3238 3943 3133 2e35  071 2.29289C13.5
+00003e50: 3139 3622 0a20 2020 2022 2032 2e31 3035  196".    " 2.105
+00003e60: 3336 2031 332e 3236 3532 2032 2031 3320  36 13.2652 2 13 
+00003e70: 325a 4d31 3120 3130 2e35 4831 2e35 5633  2ZM11 10.5H1.5V3
+00003e80: 2e35 4834 2e33 3333 3133 4c36 2e30 3636  .5H4.33313L6.066
+00003e90: 3837 2034 2e38 4336 2e32 3430 3232 2034  87 4.8C6.24022 4
+00003ea0: 2e39 3239 3334 220a 2020 2020 2220 362e  .92934".    " 6.
+00003eb0: 3435 3035 3920 342e 3939 3934 3620 362e  45059 4.99946 6.
+00003ec0: 3636 3638 3720 3548 3131 5631 302e 355a  66687 5H11V10.5Z
+00003ed0: 4d31 3320 382e 3548 3132 5635 4331 3220  M13 8.5H12V5C12 
+00003ee0: 342e 3733 3437 3820 3131 2e38 3934 3620  4.73478 11.8946 
+00003ef0: 342e 3438 3034 3320 3131 2e37 3037 3122  4.48043 11.7071"
+00003f00: 0a20 2020 2022 2034 2e32 3932 3839 4331  .    " 4.29289C1
+00003f10: 312e 3531 3936 2034 2e31 3035 3336 2031  1.5196 4.10536 1
+00003f20: 312e 3236 3532 2034 2031 3120 3448 362e  1.2652 4 11 4H6.
+00003f30: 3636 3638 374c 342e 3933 3331 3320 322e  66687L4.93313 2.
+00003f40: 3743 342e 3735 3937 3820 322e 3537 3036  7C4.75978 2.5706
+00003f50: 3622 0a20 2020 2022 2034 2e35 3439 3431  6".    " 4.54941
+00003f60: 2032 2e35 3030 3534 2034 2e33 3333 3133   2.50054 4.33313
+00003f70: 2032 2e35 4833 2e35 5631 2e35 4836 2e33   2.5H3.5V1.5H6.3
+00003f80: 3333 3133 4c38 2e30 3636 3838 2032 2e38  3313L8.06688 2.8
+00003f90: 4338 2e32 3430 3232 2032 2e39 3239 3334  C8.24022 2.92934
+00003fa0: 2038 2e34 3530 3539 220a 2020 2020 2720   8.45059".    ' 
+00003fb0: 322e 3939 3934 3620 382e 3636 3638 3720  2.99946 8.66687 
+00003fc0: 3348 3133 5638 2e35 5a22 2066 696c 6c3d  3H13V8.5Z" fill=
+00003fd0: 2263 7572 7265 6e74 436f 6c6f 7222 2f3e  "currentColor"/>
+00003fe0: 3c2f 7376 673e 270a 290a 5245 5155 4553  </svg>'.).REQUES
+00003ff0: 545f 4943 4f4e 203d 2028 0a20 2020 2027  T_ICON = (.    '
+00004000: 3c73 7667 2077 6964 7468 3d22 3332 2220  <svg width="32" 
+00004010: 2068 6569 6768 743d 2233 3222 2076 6965   height="32" vie
+00004020: 7742 6f78 3d22 3020 3020 3132 2031 3222  wBox="0 0 12 12"
+00004030: 2066 696c 6c3d 226e 6f6e 6522 270a 2020   fill="none"'.  
+00004040: 2020 2720 786d 6c6e 733d 2268 7474 703a    ' xmlns="http:
+00004050: 2f2f 7777 772e 7733 2e6f 7267 2f32 3030  //www.w3.org/200
+00004060: 302f 7376 6722 3e3c 7061 7468 2064 3d22  0/svg"><path d="
+00004070: 4d31 3120 3048 3143 302e 3733 3437 3834  M11 0H1C0.734784
+00004080: 2030 2030 2e34 3830 3433 2030 2e31 3035   0 0.48043 0.105
+00004090: 3335 3727 0a20 2020 2022 2030 2e32 3932  357'.    " 0.292
+000040a0: 3839 3320 302e 3239 3238 3933 4330 2e31  893 0.292893C0.1
+000040b0: 3035 3335 3720 302e 3438 3034 3320 3020  05357 0.48043 0 
+000040c0: 302e 3733 3437 3834 2030 2031 5631 3143  0.734784 0 1V11C
+000040d0: 3020 3131 2e32 3635 3220 302e 3130 3533  0 11.2652 0.1053
+000040e0: 3537 2031 312e 3531 3936 220a 2020 2020  57 11.5196".    
+000040f0: 2220 302e 3239 3238 3933 2031 312e 3730  " 0.292893 11.70
+00004100: 3731 4330 2e34 3830 3433 2031 312e 3839  71C0.48043 11.89
+00004110: 3436 2030 2e37 3334 3738 3420 3132 2031  46 0.734784 12 1
+00004120: 2031 3248 3131 4331 312e 3236 3532 2031   12H11C11.2652 1
+00004130: 3220 3131 2e35 3139 3620 3131 2e38 3934  2 11.5196 11.894
+00004140: 3622 0a20 2020 2022 2031 312e 3730 3731  6".    " 11.7071
+00004150: 2031 312e 3730 3731 4331 312e 3839 3436   11.7071C11.8946
+00004160: 2031 312e 3531 3936 2031 3220 3131 2e32   11.5196 12 11.2
+00004170: 3635 3220 3132 2031 3156 3143 3132 2030  652 12 11V1C12 0
+00004180: 2e37 3334 3738 3420 3131 2e38 3934 3620  .734784 11.8946 
+00004190: 302e 3438 3034 3322 0a20 2020 2022 2031  0.48043".    " 1
+000041a0: 312e 3730 3731 2030 2e32 3932 3839 3343  1.7071 0.292893C
+000041b0: 3131 2e35 3139 3620 302e 3130 3533 3537  11.5196 0.105357
+000041c0: 2031 312e 3236 3532 2030 2031 3120 305a   11.2652 0 11 0Z
+000041d0: 4d31 3120 3156 372e 3548 392e 3230 3632  M11 1V7.5H9.2062
+000041e0: 3543 392e 3037 3439 3922 0a20 2020 2022  5C9.07499".    "
+000041f0: 2037 2e34 3939 3636 2038 2e39 3434 3936   7.49966 8.94496
+00004200: 2037 2e35 3235 3420 382e 3832 3337 3220   7.5254 8.82372 
+00004210: 372e 3537 3537 3243 382e 3730 3234 3820  7.57572C8.70248 
+00004220: 372e 3632 3630 3420 382e 3539 3234 3520  7.62604 8.59245 
+00004230: 372e 3639 3939 3420 382e 3522 0a20 2020  7.69994 8.5".   
+00004240: 2022 2037 2e37 3933 3133 4c37 2e32 3933   " 7.79313L7.293
+00004250: 3133 2039 4834 2e37 3036 3837 4c33 2e35  13 9H4.70687L3.5
+00004260: 2037 2e37 3933 3133 4333 2e34 3037 3438   7.79313C3.40748
+00004270: 2037 2e36 3939 3836 2033 2e32 3937 3334   7.69986 3.29734
+00004280: 2037 2e36 3235 3932 2033 2e31 3735 3939   7.62592 3.17599
+00004290: 220a 2020 2020 2220 372e 3537 3536 4333  ".    " 7.5756C3
+000042a0: 2e30 3534 3634 2037 2e35 3235 3238 2032  .05464 7.52528 2
+000042b0: 2e39 3234 3520 372e 3439 3935 3820 322e  .9245 7.49958 2.
+000042c0: 3739 3331 3320 372e 3548 3156 3148 3131  79313 7.5H1V1H11
+000042d0: 5a4d 3131 2031 3148 3156 382e 3548 322e  ZM11 11H1V8.5H2.
+000042e0: 3739 3331 334c 3422 0a20 2020 2022 2039  79313L4".    " 9
+000042f0: 2e37 3036 3837 4334 2e30 3932 3532 2039  .70687C4.09252 9
+00004300: 2e38 3030 3134 2034 2e32 3032 3636 2039  .80014 4.20266 9
+00004310: 2e38 3734 3038 2034 2e33 3234 3031 2039  .87408 4.32401 9
+00004320: 2e39 3234 3443 342e 3434 3533 3620 392e  .9244C4.44536 9.
+00004330: 3937 3437 3220 342e 3537 3535 220a 2020  97472 4.5755".  
+00004340: 2020 2220 3130 2e30 3030 3420 342e 3730    " 10.0004 4.70
+00004350: 3638 3720 3130 4837 2e32 3933 3133 4337  687 10H7.29313C7
+00004360: 2e34 3234 3520 3130 2e30 3030 3420 372e  .4245 10.0004 7.
+00004370: 3535 3436 3420 392e 3937 3437 3220 372e  55464 9.97472 7.
+00004380: 3637 3539 3920 392e 3932 3434 4337 2e37  67599 9.9244C7.7
+00004390: 3937 3334 220a 2020 2020 2720 392e 3837  9734".    ' 9.87
+000043a0: 3430 3820 372e 3930 3734 3820 392e 3830  408 7.90748 9.80
+000043b0: 3031 3420 3820 392e 3730 3638 374c 392e  014 8 9.70687L9.
+000043c0: 3230 3638 3720 382e 3548 3131 5631 315a  20687 8.5H11V11Z
+000043d0: 2220 6669 6c6c 3d22 2333 3433 3333 3022  " fill="#343330"
+000043e0: 2f3e 3c2f 7376 673e 270a 290a 0a41 5252  /></svg>'.)..ARR
+000043f0: 4f57 5f49 434f 4e20 3d20 280a 2020 2020  OW_ICON = (.    
+00004400: 273c 7376 6720 7769 6474 683d 2232 3422  '<svg width="24"
+00004410: 2068 6569 6768 743d 2232 3422 2076 6965   height="24" vie
+00004420: 7742 6f78 3d22 3020 3020 3234 2032 3422  wBox="0 0 24 24"
+00004430: 2066 696c 6c3d 226e 6f6e 6522 2078 6d6c   fill="none" xml
+00004440: 6e73 3d22 6874 7470 3a2f 2f77 7777 2e77  ns="http://www.w
+00004450: 332e 6f72 672f 3230 3030 2f73 7667 223e  3.org/2000/svg">
+00004460: 270a 2020 2020 273c 7265 6374 2078 3d22  '.    '<rect x="
+00004470: 302e 3522 2079 3d22 302e 3522 2077 6964  0.5" y="0.5" wid
+00004480: 7468 3d22 3233 2220 6865 6967 6874 3d22  th="23" height="
+00004490: 3233 2220 7278 3d22 312e 3522 2066 696c  23" rx="1.5" fil
+000044a0: 6c3d 2223 4543 4542 4546 222f 3e27 0a20  l="#ECEBEF"/>'. 
+000044b0: 2020 2027 3c72 6563 7420 783d 2230 2e35     '<rect x="0.5
+000044c0: 2220 793d 2230 2e35 2220 7769 6474 683d  " y="0.5" width=
+000044d0: 2232 3322 2068 6569 6768 743d 2232 3322  "23" height="23"
+000044e0: 2072 783d 2231 2e35 2220 7374 726f 6b65   rx="1.5" stroke
+000044f0: 3d22 2342 3442 3042 4622 2f3e 270a 2020  ="#B4B0BF"/>'.  
+00004500: 2020 273c 7061 7468 2064 3d22 4d31 372e    '<path d="M17.
+00004510: 3835 3338 2031 322e 3335 3338 4c31 332e  8538 12.3538L13.
+00004520: 3335 3338 2031 362e 3835 3338 4331 332e  3538 16.8538C13.
+00004530: 3235 3939 2031 362e 3934 3736 2031 332e  2599 16.9476 13.
+00004540: 3133 3237 2031 372e 3030 3033 2031 3320  1327 17.0003 13 
+00004550: 3137 2e30 3030 3343 3132 2e38 3637 3320  17.0003C12.8673 
+00004560: 3137 2e30 3030 3320 3132 2e37 3430 3120  17.0003 12.7401 
+00004570: 3136 2e39 3437 3620 3132 2e36 3436 3220  16.9476 12.6462 
+00004580: 3136 2e38 3533 3843 3132 2e35 3532 3420  16.8538C12.5524 
+00004590: 3136 2e37 3620 3132 2e34 3939 3720 3136  16.76 12.4997 16
+000045a0: 2e36 3332 3720 3132 2e34 3939 3720 3136  .6327 12.4997 16
+000045b0: 2e35 4331 322e 3439 3937 2031 362e 3336  .5C12.4997 16.36
+000045c0: 3734 2031 322e 3535 3234 2031 362e 3234  74 12.5524 16.24
+000045d0: 3031 2031 322e 3634 3632 2031 362e 3134  01 12.6462 16.14
+000045e0: 3633 4c31 362e 3239 3331 2031 322e 3548  63L16.2931 12.5H
+000045f0: 362e 3543 362e 3336 3733 3920 3132 2e35  6.5C6.36739 12.5
+00004600: 2036 2e32 3430 3231 2031 322e 3434 3734   6.24021 12.4474
+00004610: 2036 2e31 3436 3435 2031 322e 3335 3336   6.14645 12.3536
+00004620: 4336 2e30 3532 3638 2031 322e 3235 3938  C6.05268 12.2598
+00004630: 2036 2031 322e 3133 3236 2036 2031 3243   6 12.1326 6 12C
+00004640: 3620 3131 2e38 3637 3420 362e 3035 3236  6 11.8674 6.0526
+00004650: 3820 3131 2e37 3430 3220 362e 3134 3634  8 11.7402 6.1464
+00004660: 3520 3131 2e36 3436 3543 362e 3234 3032  5 11.6465C6.2402
+00004670: 3120 3131 2e35 3532 3720 362e 3336 3733  1 11.5527 6.3673
+00004680: 3920 3131 2e35 2036 2e35 2031 312e 3548  9 11.5 6.5 11.5H
+00004690: 3136 2e32 3933 314c 3132 2e36 3436 3220  16.2931L12.6462 
+000046a0: 372e 3835 3337 3843 3132 2e35 3532 3420  7.85378C12.5524 
+000046b0: 372e 3735 3939 3620 3132 2e34 3939 3720  7.75996 12.4997 
+000046c0: 372e 3633 3237 3220 3132 2e34 3939 3720  7.63272 12.4997 
+000046d0: 372e 3530 3030 3343 3132 2e34 3939 3720  7.50003C12.4997 
+000046e0: 372e 3336 3733 3520 3132 2e35 3532 3420  7.36735 12.5524 
+000046f0: 372e 3234 3031 2031 322e 3634 3632 2037  7.2401 12.6462 7
+00004700: 2e31 3436 3238 4331 322e 3734 3031 2037  .14628C12.7401 7
+00004710: 2e30 3532 3436 2031 322e 3836 3733 2036  .05246 12.8673 6
+00004720: 2e39 3939 3736 2031 3320 362e 3939 3937  .99976 13 6.9997
+00004730: 3643 3133 2e31 3332 3720 362e 3939 3937  6C13.1327 6.9997
+00004740: 3620 3133 2e32 3539 3920 372e 3035 3234  6 13.2599 7.0524
+00004750: 3620 3133 2e33 3533 3820 372e 3134 3632  6 13.3538 7.1462
+00004760: 384c 3137 2e38 3533 3820 3131 2e36 3436  8L17.8538 11.646
+00004770: 3343 3137 2e39 3030 3220 3131 2e36 3932  3C17.9002 11.692
+00004780: 3720 3137 2e39 3337 3120 3131 2e37 3437  7 17.9371 11.747
+00004790: 3920 3137 2e39 3632 3320 3131 2e38 3038  9 17.9623 11.808
+000047a0: 3643 3137 2e39 3837 3420 3131 2e38 3639  6C17.9874 11.869
+000047b0: 3320 3138 2e30 3030 3420 3131 2e39 3334  3 18.0004 11.934
+000047c0: 3320 3138 2e30 3030 3420 3132 4331 382e  3 18.0004 12C18.
+000047d0: 3030 3034 2031 322e 3036 3537 2031 372e  0004 12.0657 17.
+000047e0: 3938 3734 2031 322e 3133 3038 2031 372e  9874 12.1308 17.
+000047f0: 3936 3233 2031 322e 3139 3135 4331 372e  9623 12.1915C17.
+00004800: 3933 3731 2031 322e 3235 3232 2031 372e  9371 12.2522 17.
+00004810: 3930 3032 2031 322e 3330 3733 2031 372e  9002 12.3073 17.
+00004820: 3835 3338 2031 322e 3335 3338 5a22 2066  8538 12.3538Z" f
+00004830: 696c 6c3d 2223 3545 3541 3732 222f 3e3c  ill="#5E5A72"/><
+00004840: 2f73 7667 3e27 2020 2320 6e6f 7161 3a20  /svg>'  # noqa: 
+00004850: 4535 3031 0a29 0a0a 0a63 7573 746f 6d5f  E501.)...custom_
+00004860: 636f 6465 203d 2022 2222 0a20 2020 203c  code = """.    <
+00004870: 6469 7620 7374 796c 653d 276d 6172 6769  div style='margi
+00004880: 6e2d 746f 703a 3135 7078 3b27 3e0a 2020  n-top:15px;'>.  
+00004890: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+000048a0: 3d27 666c 6578 2067 6170 2d31 3027 2073  ='flex gap-10' s
+000048b0: 7479 6c65 3d27 616c 6967 6e2d 6974 656d  tyle='align-item
+000048c0: 733a 2063 656e 7465 723b 273e 0a20 2020  s: center;'>.   
+000048d0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+000048e0: 6173 733d 2766 6f6c 6465 722d 6963 6f6e  ass='folder-icon
+000048f0: 273e 247b 6963 6f6e 7d3c 2f64 6976 3e0a  '>${icon}</div>.
+00004900: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00004910: 3e3c 7020 636c 6173 733d 2768 6561 6465  ><p class='heade
+00004920: 722d 3327 3e24 7b6c 6973 745f 6e61 6d65  r-3'>${list_name
+00004930: 7d3c 2f70 3e3c 2f64 6976 3e0a 2020 2020  }</p></div>.    
+00004940: 2020 2020 3c2f 6469 763e 0a0a 2020 2020      </div>..    
+00004950: 2020 2020 2020 2020 3c64 6976 2073 7479          <div sty
+00004960: 6c65 3d22 7061 6464 696e 672d 746f 703a  le="padding-top:
+00004970: 2031 3670 783b 2064 6973 706c 6179 3a66   16px; display:f
+00004980: 6c65 783b 6a75 7374 6966 792d 636f 6e74  lex;justify-cont
+00004990: 656e 743a 2073 7061 6365 2d62 6574 7765  ent: space-betwe
+000049a0: 656e 3b20 616c 6967 6e2d 6974 656d 733a  en; align-items:
+000049b0: 2063 656e 7465 723b 223e 0a20 2020 2020   center;">.     
+000049c0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+000049d0: 636c 6173 733d 2770 742d 3235 2067 6170  class='pt-25 gap
+000049e0: 2d31 3027 2073 7479 6c65 3d22 6469 7370  -10' style="disp
+000049f0: 6c61 793a 666c 6578 3b22 3e0a 2020 2020  lay:flex;">.    
+00004a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a10: 3c64 6976 2063 6c61 7373 3d22 7365 6172  <div class="sear
+00004a20: 6368 2d66 6965 6c64 223e 0a20 2020 2020  ch-field">.     
+00004a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a40: 2020 203c 6469 7620 6964 3d27 7365 6172     <div id='sear
+00004a50: 6368 2d6d 656e 7524 7b75 6964 7d27 2063  ch-menu${uid}' c
+00004a60: 6c61 7373 3d22 7379 6674 2d64 726f 7064  lass="syft-dropd
+00004a70: 6f77 6e22 206f 6e63 6c69 636b 3d22 7b0a  own" onclick="{.
+00004a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a90: 2020 2020 2020 2020 2020 2020 6c65 7420              let 
+00004aa0: 646f 6320 3d20 646f 6375 6d65 6e74 2e67  doc = document.g
+00004ab0: 6574 456c 656d 656e 7442 7949 6428 2773  etElementById('s
+00004ac0: 6561 7263 682d 6472 6f70 646f 776e 2d63  earch-dropdown-c
+00004ad0: 6f6e 7465 6e74 247b 7569 647d 2729 0a20  ontent${uid}'). 
+00004ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004af0: 2020 2020 2020 2020 2020 2069 6620 2864             if (d
+00004b00: 6f63 2e73 7479 6c65 2e64 6973 706c 6179  oc.style.display
+00004b10: 203d 3d3d 2027 626c 6f63 6b27 297b 0a20   === 'block'){. 
 00004b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b40: 2020 2020 2020 2020 6c65 7420 636f 6e74          let cont
-00004b50: 656e 7420 3d20 646f 6375 6d65 6e74 2e63  ent = document.c
-00004b60: 7265 6174 6545 6c65 6d65 6e74 2827 6469  reateElement('di
-00004b70: 7627 293b 0a20 2020 2020 2020 2020 2020  v');.           
+00004b30: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00004b40: 6f63 2e73 7479 6c65 2e64 6973 706c 6179  oc.style.display
+00004b50: 203d 2027 6e6f 6e65 270a 2020 2020 2020   = 'none'.      
+00004b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b70: 2020 2020 2020 7d20 656c 7365 207b 0a20        } else {. 
 00004b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ba0: 2063 6f6e 7465 6e74 2e6f 6e63 6c69 636b   content.onclick
-00004bb0: 203d 2066 756e 6374 696f 6e28 6576 656e   = function(even
-00004bc0: 7429 207b 0a20 2020 2020 2020 2020 2020  t) {.           
-00004bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b90: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00004ba0: 6f63 2e73 7479 6c65 2e64 6973 706c 6179  oc.style.display
+00004bb0: 203d 2027 626c 6f63 6b27 0a20 2020 2020   = 'block'.     
+00004bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004bd0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
 00004be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bf0: 2020 2020 2065 7665 6e74 2e73 746f 7050       event.stopP
-00004c00: 726f 7061 6761 7469 6f6e 2829 0a20 2020  ropagation().   
-00004c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c30: 2020 2020 2020 2020 2020 2020 2064 6f63               doc
-00004c40: 756d 656e 742e 6765 7445 6c65 6d65 6e74  ument.getElement
-00004c50: 4279 4964 2827 6d65 6e75 2d61 6374 6976  ById('menu-activ
-00004c60: 652d 6669 6c74 6572 247b 7569 647d 2729  e-filter${uid}')
-00004c70: 2e69 6e6e 6572 5465 7874 203d 2061 7474  .innerText = att
-00004c80: 723b 0a20 2020 2020 2020 2020 2020 2020  r;.             
+00004bf0: 2020 2020 207d 223e 0a20 2020 2020 2020       }">.       
+00004c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c10: 2020 2020 203c 6469 7620 6964 3d27 7365       <div id='se
+00004c20: 6172 6368 2d64 726f 7064 6f77 6e2d 636f  arch-dropdown-co
+00004c30: 6e74 656e 7424 7b75 6964 7d27 2063 6c61  ntent${uid}' cla
+00004c40: 7373 3d27 7379 6674 2d64 726f 7064 6f77  ss='syft-dropdow
+00004c50: 6e2d 636f 6e74 656e 7427 3e3c 2f64 6976  n-content'></div
+00004c60: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00004c70: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
+00004c80: 6372 6970 743e 0a20 2020 2020 2020 2020  cript>.         
 00004c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cb0: 2020 2061 6374 6976 6546 696c 7465 7224     activeFilter$
-00004cc0: 7b75 6964 7d20 3d20 6174 7472 3b0a 2020  {uid} = attr;.  
+00004ca0: 2020 2020 2020 2076 6172 2065 6c65 6d65         var eleme
+00004cb0: 6e74 247b 7569 647d 203d 2024 7b65 6c65  nt${uid} = ${ele
+00004cc0: 6d65 6e74 7d0a 2020 2020 2020 2020 2020  ment}.          
 00004cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cf0: 2020 2020 2020 2020 2020 2020 2020 646f                do
-00004d00: 6375 6d65 6e74 2e67 6574 456c 656d 656e  cument.getElemen
-00004d10: 7442 7949 6428 0a20 2020 2020 2020 2020  tById(.         
-00004d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d40: 2020 2020 2020 2020 2020 2027 7365 6172             'sear
-00004d50: 6368 2d64 726f 7064 6f77 6e2d 636f 6e74  ch-dropdown-cont
-00004d60: 656e 7424 7b75 6964 7d27 0a20 2020 2020  ent${uid}'.     
-00004d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ce0: 2020 2020 2020 7661 7220 7061 6765 5f73        var page_s
+00004cf0: 697a 6524 7b75 6964 7d20 3d20 247b 726f  ize${uid} = ${ro
+00004d00: 7773 7d0a 2020 2020 2020 2020 2020 2020  ws}.            
+00004d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d20: 2020 2020 7661 7220 7061 6765 496e 6465      var pageInde
+00004d30: 7824 7b75 6964 7d20 3d20 310a 2020 2020  x${uid} = 1.    
+00004d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d50: 2020 2020 2020 2020 2020 2020 7661 7220              var 
+00004d60: 7061 6769 6e61 7465 6445 6c65 6d65 6e74  paginatedElement
+00004d70: 7324 7b75 6964 7d20 3d20 5b5d 0a20 2020  s${uid} = [].   
 00004d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d90: 2020 2020 2020 2020 2020 2029 2e73 7479             ).sty
-00004da0: 6c65 2e64 6973 706c 6179 3d20 276e 6f6e  le.display= 'non
-00004db0: 6527 3b0a 2020 2020 2020 2020 2020 2020  e';.            
+00004d90: 2020 2020 2020 2020 2020 2020 2076 6172               var
+00004da0: 2061 6374 6976 6546 696c 7465 7224 7b75   activeFilter${u
+00004db0: 6964 7d3b 0a0a 2020 2020 2020 2020 2020  id};..          
 00004dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004de0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00004df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e00: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00004e10: 6e74 656e 742e 636c 6173 734c 6973 742e  ntent.classList.
-00004e20: 6164 6428 2264 642d 6f70 7469 6f6e 7322  add("dd-options"
-00004e30: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
+00004dd0: 2020 2020 2020 6675 6e63 7469 6f6e 2062        function b
+00004de0: 7569 6c64 4472 6f70 446f 776e 4d65 6e75  uildDropDownMenu
+00004df0: 2865 6c65 6d65 6e74 7329 7b0a 2020 2020  (elements){.    
+00004e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e20: 6c65 7420 696e 6974 5f66 696c 7465 723b  let init_filter;
+00004e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00004e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e50: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00004e60: 6f6e 7465 6e74 2e69 6e6e 6572 5465 7874  ontent.innerText
-00004e70: 203d 2061 7474 723b 0a20 2020 2020 2020   = attr;.       
-00004e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ea0: 2020 2020 206d 656e 752e 6170 7065 6e64       menu.append
-00004eb0: 4368 696c 6428 636f 6e74 656e 7429 3b0a  Child(content);.
-00004ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ee0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00004e50: 2020 2020 206c 6574 206d 656e 7520 3d20       let menu = 
+00004e60: 646f 6375 6d65 6e74 2e67 6574 456c 656d  document.getElem
+00004e70: 656e 7442 7949 6428 2773 6561 7263 682d  entById('search-
+00004e80: 6472 6f70 646f 776e 2d63 6f6e 7465 6e74  dropdown-content
+00004e90: 247b 7569 647d 2729 0a20 2020 2020 2020  ${uid}').       
+00004ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004eb0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00004ec0: 2865 6c65 6d65 6e74 732e 6c65 6e67 7468  (elements.length
+00004ed0: 203e 2030 2920 7b0a 2020 2020 2020 2020   > 0) {.        
+00004ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f00: 2020 2020 2020 2020 2020 2020 2020 7d20                } 
-00004f10: 656c 7365 207b 0a20 2020 2020 2020 2020  else {.         
+00004f00: 6c65 7420 7361 6d70 6c65 203d 2065 6c65  let sample = ele
+00004f10: 6d65 6e74 735b 305d 0a20 2020 2020 2020  ments[0].       
 00004f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f30: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00004f40: 6574 2069 6e69 745f 6669 6c74 6572 203d  et init_filter =
-00004f50: 2027 2d2d 2d27 0a20 2020 2020 2020 2020   '---'.         
+00004f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f40: 2066 6f72 2028 636f 6e73 7420 6174 7472   for (const attr
+00004f50: 2069 6e20 7361 6d70 6c65 2920 7b0a 2020   in sample) {.  
 00004f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f70: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00004f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fa0: 206c 6574 2064 726f 7064 6f77 6e5f 6669   let dropdown_fi
-00004fb0: 656c 6420 3d20 646f 6375 6d65 6e74 2e67  eld = document.g
-00004fc0: 6574 456c 656d 656e 7442 7949 6428 2773  etElementById('s
-00004fd0: 6561 7263 682d 6d65 6e75 247b 7569 647d  earch-menu${uid}
-00004fe0: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
-00004ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005000: 2020 2020 2020 206c 6574 2073 7061 6e20         let span 
-00005010: 3d20 646f 6375 6d65 6e74 2e63 7265 6174  = document.creat
-00005020: 6545 6c65 6d65 6e74 2827 7370 616e 2729  eElement('span')
-00005030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f80: 2020 2020 2020 2020 2020 6966 2028 7479            if (ty
+00004f90: 7065 6f66 2069 6e69 745f 6669 6c74 6572  peof init_filter
+00004fa0: 203d 3d3d 2027 756e 6465 6669 6e65 6427   === 'undefined'
+00004fb0: 297b 0a20 2020 2020 2020 2020 2020 2020  ){.             
+00004fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fe0: 2020 2069 6e69 745f 6669 6c74 6572 203d     init_filter =
+00004ff0: 2061 7474 723b 0a20 2020 2020 2020 2020   attr;.         
+00005000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005020: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
+00005030: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005050: 2020 2020 2073 7061 6e2e 7365 7441 7474       span.setAtt
-00005060: 7269 6275 7465 2827 6964 272c 2027 6d65  ribute('id', 'me
-00005070: 6e75 2d61 6374 6976 652d 6669 6c74 6572  nu-active-filter
-00005080: 247b 7569 647d 2729 0a20 2020 2020 2020  ${uid}').       
+00005050: 206c 6574 2063 6f6e 7465 6e74 203d 2064   let content = d
+00005060: 6f63 756d 656e 742e 6372 6561 7465 456c  ocument.createEl
+00005070: 656d 656e 7428 2764 6976 2729 3b0a 2020  ement('div');.  
+00005080: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050a0: 2020 2020 2020 2020 2020 2020 2073 7061               spa
-000050b0: 6e2e 696e 6e65 7254 6578 7420 3d20 696e  n.innerText = in
-000050c0: 6974 5f66 696c 7465 720a 2020 2020 2020  it_filter.      
+000050a0: 2020 2020 2020 2020 2020 636f 6e74 656e            conten
+000050b0: 742e 6f6e 636c 6963 6b20 3d20 6675 6e63  t.onclick = func
+000050c0: 7469 6f6e 2865 7665 6e74 2920 7b0a 2020  tion(event) {.  
 000050d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050e0: 2020 2020 2020 2020 2020 2020 2020 6163                ac
-000050f0: 7469 7665 4669 6c74 6572 247b 7569 647d  tiveFilter${uid}
-00005100: 203d 2069 6e69 745f 6669 6c74 6572 3b0a   = init_filter;.
-00005110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050f0: 2020 2020 2020 2020 2020 2020 2020 6576                ev
+00005100: 656e 742e 7374 6f70 5072 6f70 6167 6174  ent.stopPropagat
+00005110: 696f 6e28 290a 2020 2020 2020 2020 2020  ion().          
 00005120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005130: 2020 2020 6472 6f70 646f 776e 5f66 6965      dropdown_fie
-00005140: 6c64 2e61 7070 656e 6443 6869 6c64 2873  ld.appendChild(s
-00005150: 7061 6e29 0a20 2020 2020 2020 2020 2020  pan).           
-00005160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005170: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
-00005180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005190: 2020 2020 2020 2020 6275 696c 6444 726f          buildDro
-000051a0: 7044 6f77 6e4d 656e 7528 656c 656d 656e  pDownMenu(elemen
-000051b0: 7424 7b75 6964 7d29 0a20 2020 2020 2020  t${uid}).       
-000051c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051d0: 2020 2020 203c 2f73 6372 6970 743e 0a20       </script>. 
+00005130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005140: 2020 2020 2020 646f 6375 6d65 6e74 2e67        document.g
+00005150: 6574 456c 656d 656e 7442 7949 6428 276d  etElementById('m
+00005160: 656e 752d 6163 7469 7665 2d66 696c 7465  enu-active-filte
+00005170: 7224 7b75 6964 7d27 292e 696e 6e65 7254  r${uid}').innerT
+00005180: 6578 7420 3d20 6174 7472 3b0a 2020 2020  ext = attr;.    
+00005190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051b0: 2020 2020 2020 2020 2020 2020 6163 7469              acti
+000051c0: 7665 4669 6c74 6572 247b 7569 647d 203d  veFilter${uid} =
+000051d0: 2061 7474 723b 0a20 2020 2020 2020 2020   attr;.         
 000051e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051f0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-00005200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005210: 2020 2020 2020 3c69 6e70 7574 2069 643d        <input id=
-00005220: 2773 6561 7263 684b 6579 247b 7569 647d  'searchKey${uid}
-00005230: 2720 636c 6173 733d 2773 6561 7263 682d  ' class='search-
-00005240: 696e 7075 7427 2070 6c61 6365 686f 6c64  input' placehold
-00005250: 6572 3d27 456e 7465 7220 7365 6172 6368  er='Enter search
-00005260: 2068 6572 6520 2e2e 2e27 2020 2f3e 0a20   here ...'  />. 
-00005270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005280: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-00005290: 2020 2020 2020 2020 2020 2020 2020 3c62                <b
-000052a0: 7574 746f 6e20 636c 6173 733d 2773 6561  utton class='sea
-000052b0: 7263 682d 6275 7474 6f6e 2720 7479 7065  rch-button' type
-000052c0: 3d22 6275 7474 6f6e 2220 6f6e 636c 6963  ="button" onclic
-000052d0: 6b3d 2273 6561 7263 6847 7269 6424 7b75  k="searchGrid${u
-000052e0: 6964 7d28 656c 656d 656e 7424 7b75 6964  id}(element${uid
-000052f0: 7d29 223e 0a20 2020 2020 2020 2020 2020  })">.           
-00005300: 2020 2020 2020 2020 2020 2020 2024 7b73               ${s
-00005310: 6561 7263 6849 636f 6e7d 0a20 2020 2020  earchIcon}.     
-00005320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005330: 2020 203c 7370 616e 2063 6c61 7373 3d27     <span class='
-00005340: 706c 2d38 273e 5365 6172 6368 3c2f 7370  pl-8'>Search</sp
-00005350: 616e 3e0a 2020 2020 2020 2020 2020 2020  an>.            
-00005360: 2020 2020 2020 2020 3c2f 6275 7474 6f6e          </button
-00005370: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00005380: 2020 3c2f 6469 763e 0a0a 2020 2020 2020    </div>..      
-00005390: 2020 2020 2020 2020 2020 3c64 6976 3e3c            <div><
-000053a0: 6834 2069 643d 2774 6f74 616c 247b 7569  h4 id='total${ui
-000053b0: 647d 273e 303c 2f68 343e 3c2f 6469 763e  d}'>0</h4></div>
-000053c0: 0a20 2020 2020 2020 2020 2020 203c 2f64  .            </d
-000053d0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-000053e0: 3c64 6976 2069 643d 2774 6162 6c65 247b  <div id='table${
-000053f0: 7569 647d 2720 636c 6173 733d 2767 7269  uid}' class='gri
-00005400: 642d 7461 626c 6524 7b75 6964 7d27 2073  d-table${uid}' s
-00005410: 7479 6c65 3d27 6d61 7267 696e 2d74 6f70  tyle='margin-top
-00005420: 3a20 3235 7078 3b27 3e0a 2020 2020 2020  : 25px;'>.      
-00005430: 2020 2020 2020 2020 2020 3c73 6372 6970            <scrip
-00005440: 743e 0a20 2020 2020 2020 2020 2020 2020  t>.             
-00005450: 2020 2020 2020 2066 756e 6374 696f 6e20         function 
-00005460: 7061 6769 6e61 7465 247b 7569 647d 2861  paginate${uid}(a
-00005470: 7272 2c20 7369 7a65 2920 7b0a 2020 2020  rr, size) {.    
-00005480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005490: 2020 2020 636f 6e73 7420 7265 7320 3d20      const res = 
-000054a0: 5b5d 3b0a 2020 2020 2020 2020 2020 2020  [];.            
-000054b0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000054c0: 286c 6574 2069 203d 2030 3b20 6920 3c20  (let i = 0; i < 
-000054d0: 6172 722e 6c65 6e67 7468 3b20 6920 2b3d  arr.length; i +=
-000054e0: 2073 697a 6529 207b 0a20 2020 2020 2020   size) {.       
+000051f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005200: 2020 2020 2020 2064 6f63 756d 656e 742e         document.
+00005210: 6765 7445 6c65 6d65 6e74 4279 4964 280a  getElementById(.
+00005220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005250: 2020 2020 2773 6561 7263 682d 6472 6f70      'search-drop
+00005260: 646f 776e 2d63 6f6e 7465 6e74 247b 7569  down-content${ui
+00005270: 647d 270a 2020 2020 2020 2020 2020 2020  d}'.            
+00005280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052a0: 2020 2020 292e 7374 796c 652e 6469 7370      ).style.disp
+000052b0: 6c61 793d 2027 6e6f 6e65 273b 0a20 2020  lay= 'none';.   
+000052c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052e0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+000052f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005310: 2020 2020 2020 2063 6f6e 7465 6e74 2e63         content.c
+00005320: 6c61 7373 4c69 7374 2e61 6464 2822 6464  lassList.add("dd
+00005330: 2d6f 7074 696f 6e73 2229 3b0a 2020 2020  -options");.    
+00005340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005360: 2020 2020 2020 2020 636f 6e74 656e 742e          content.
+00005370: 696e 6e65 7254 6578 7420 3d20 6174 7472  innerText = attr
+00005380: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+00005390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053a0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+000053b0: 6e75 2e61 7070 656e 6443 6869 6c64 2863  nu.appendChild(c
+000053c0: 6f6e 7465 6e74 293b 0a20 2020 2020 2020  ontent);.       
+000053d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053f0: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
+00005400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005410: 2020 2020 2020 207d 2065 6c73 6520 7b0a         } else {.
+00005420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005440: 2020 2020 2020 2020 6c65 7420 696e 6974          let init
+00005450: 5f66 696c 7465 7220 3d20 272d 2d2d 270a  _filter = '---'.
+00005460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005480: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+00005490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054a0: 2020 2020 2020 2020 2020 6c65 7420 6472            let dr
+000054b0: 6f70 646f 776e 5f66 6965 6c64 203d 2064  opdown_field = d
+000054c0: 6f63 756d 656e 742e 6765 7445 6c65 6d65  ocument.getEleme
+000054d0: 6e74 4279 4964 2827 7365 6172 6368 2d6d  ntById('search-m
+000054e0: 656e 7524 7b75 6964 7d27 290a 2020 2020  enu${uid}').    
 000054f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005500: 2020 2020 2063 6f6e 7374 2063 6875 6e6b       const chunk
-00005510: 203d 2061 7272 2e73 6c69 6365 2869 2c20   = arr.slice(i, 
-00005520: 6920 2b20 7369 7a65 293b 0a20 2020 2020  i + size);.     
-00005530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005540: 2020 2020 2020 2072 6573 2e70 7573 6828         res.push(
-00005550: 6368 756e 6b29 3b0a 2020 2020 2020 2020  chunk);.        
-00005560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005570: 7d0a 0a20 2020 2020 2020 2020 2020 2020  }..             
-00005580: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00005590: 6e20 7265 733b 0a20 2020 2020 2020 2020  n res;.         
-000055a0: 2020 2020 2020 2020 2020 207d 0a0a 2020             }..  
-000055b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055c0: 2020 6675 6e63 7469 6f6e 2073 6561 7263    function searc
-000055d0: 6847 7269 6424 7b75 6964 7d28 656c 656d  hGrid${uid}(elem
-000055e0: 656e 7473 297b 0a20 2020 2020 2020 2020  ents){.         
-000055f0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00005600: 6574 2073 6561 7263 684b 6579 203d 2064  et searchKey = d
-00005610: 6f63 756d 656e 742e 6765 7445 6c65 6d65  ocument.getEleme
-00005620: 6e74 4279 4964 2827 7365 6172 6368 4b65  ntById('searchKe
-00005630: 7924 7b75 6964 7d27 292e 7661 6c75 653b  y${uid}').value;
-00005640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005650: 2020 2020 2020 2020 206c 6574 2072 6573           let res
-00005660: 756c 743b 0a20 2020 2020 2020 2020 2020  ult;.           
-00005670: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00005680: 2873 6561 7263 684b 6579 203d 3d3d 2027  (searchKey === '
-00005690: 2729 7b0a 2020 2020 2020 2020 2020 2020  '){.            
-000056a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056b0: 7265 7375 6c74 203d 2065 6c65 6d65 6e74  result = element
-000056c0: 733b 0a20 2020 2020 2020 2020 2020 2020  s;.             
-000056d0: 2020 2020 2020 2020 2020 207d 2065 6c73             } els
-000056e0: 6520 7b0a 2020 2020 2020 2020 2020 2020  e {.            
+00005500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005510: 6c65 7420 7370 616e 203d 2064 6f63 756d  let span = docum
+00005520: 656e 742e 6372 6561 7465 456c 656d 656e  ent.createElemen
+00005530: 7428 2773 7061 6e27 290a 2020 2020 2020  t('span').      
+00005540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005550: 2020 2020 2020 2020 2020 2020 2020 7370                sp
+00005560: 616e 2e73 6574 4174 7472 6962 7574 6528  an.setAttribute(
+00005570: 2769 6427 2c20 276d 656e 752d 6163 7469  'id', 'menu-acti
+00005580: 7665 2d66 696c 7465 7224 7b75 6964 7d27  ve-filter${uid}'
+00005590: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000055a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055b0: 2020 2020 2020 7370 616e 2e69 6e6e 6572        span.inner
+000055c0: 5465 7874 203d 2069 6e69 745f 6669 6c74  Text = init_filt
+000055d0: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
+000055e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055f0: 2020 2020 2020 2061 6374 6976 6546 696c         activeFil
+00005600: 7465 7224 7b75 6964 7d20 3d20 696e 6974  ter${uid} = init
+00005610: 5f66 696c 7465 723b 0a20 2020 2020 2020  _filter;.       
+00005620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005630: 2020 2020 2020 2020 2020 2020 2064 726f               dro
+00005640: 7064 6f77 6e5f 6669 656c 642e 6170 7065  pdown_field.appe
+00005650: 6e64 4368 696c 6428 7370 616e 290a 2020  ndChild(span).  
+00005660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005670: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00005680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056a0: 2062 7569 6c64 4472 6f70 446f 776e 4d65   buildDropDownMe
+000056b0: 6e75 2865 6c65 6d65 6e74 247b 7569 647d  nu(element${uid}
+000056c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000056d0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+000056e0: 7363 7269 7074 3e0a 2020 2020 2020 2020  script>.        
 000056f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005700: 7265 7375 6c74 203d 2065 6c65 6d65 6e74  result = element
-00005710: 732e 6669 6c74 6572 2828 656c 656d 656e  s.filter((elemen
-00005720: 7429 203d 3e20 7b0a 2020 2020 2020 2020  t) => {.        
-00005730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005740: 2020 2020 2020 2020 6c65 7420 7072 6f70          let prop
-00005750: 6572 7479 203d 2065 6c65 6d65 6e74 5b61  erty = element[a
-00005760: 6374 6976 6546 696c 7465 7224 7b75 6964  ctiveFilter${uid
-00005770: 7d5d 0a20 2020 2020 2020 2020 2020 2020  }].             
-00005780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005790: 2020 2069 6620 2874 7970 656f 6620 7072     if (typeof pr
-000057a0: 6f70 6572 7479 203d 3d3d 2027 6f62 6a65  operty === 'obje
-000057b0: 6374 2720 2626 2070 726f 7065 7274 7920  ct' && property 
-000057c0: 213d 3d20 6e75 6c6c 297b 0a20 2020 2020  !== null){.     
-000057d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057e0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000057f0: 6574 7572 6e20 7072 6f70 6572 7479 2e76  eturn property.v
-00005800: 616c 7565 2e74 6f4c 6f77 6572 4361 7365  alue.toLowerCase
-00005810: 2829 2e69 6e63 6c75 6465 7328 7365 6172  ().includes(sear
-00005820: 6368 4b65 792e 746f 4c6f 7765 7243 6173  chKey.toLowerCas
-00005830: 6528 2929 3b0a 2020 2020 2020 2020 2020  e());.          
-00005840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005850: 2020 2020 2020 7d20 656c 7365 2069 6620        } else if 
-00005860: 2874 7970 656f 6620 7072 6f70 6572 7479  (typeof property
-00005870: 203d 3d3d 2027 7374 7269 6e67 2720 2920   === 'string' ) 
-00005880: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00005890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058a0: 2020 2020 2020 7265 7475 726e 2065 6c65        return ele
-000058b0: 6d65 6e74 5b61 6374 6976 6546 696c 7465  ment[activeFilte
-000058c0: 7224 7b75 6964 7d5d 2e74 6f4c 6f77 6572  r${uid}].toLower
-000058d0: 4361 7365 2829 2e69 6e63 6c75 6465 7328  Case().includes(
-000058e0: 7365 6172 6368 4b65 792e 746f 4c6f 7765  searchKey.toLowe
-000058f0: 7243 6173 6528 2929 3b0a 2020 2020 2020  rCase());.      
-00005900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005910: 2020 2020 2020 2020 2020 7d20 656c 7365            } else
-00005920: 2069 6620 2870 726f 7065 7274 7920 213d   if (property !=
-00005930: 3d20 6e75 6c6c 2029 207b 0a20 2020 2020  = null ) {.     
-00005940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005950: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00005960: 6574 7572 6e20 656c 656d 656e 745b 6163  eturn element[ac
-00005970: 7469 7665 4669 6c74 6572 247b 7569 647d  tiveFilter${uid}
-00005980: 5d2e 746f 5374 7269 6e67 2829 203d 3d3d  ].toString() ===
-00005990: 2073 6561 7263 684b 6579 3b0a 2020 2020   searchKey;.    
-000059a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059b0: 2020 2020 2020 2020 2020 2020 7d20 656c              } el
-000059c0: 7365 207b 0a20 2020 2020 2020 2020 2020  se {.           
-000059d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059e0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000059f0: 656c 656d 656e 745b 6163 7469 7665 4669  element[activeFi
-00005a00: 6c74 6572 247b 7569 647d 5d20 3d3d 3d20  lter${uid}] === 
-00005a10: 7365 6172 6368 4b65 793b 0a20 2020 2020  searchKey;.     
-00005a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a30: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00005700: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00005710: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00005720: 696e 7075 7420 6964 3d27 7365 6172 6368  input id='search
+00005730: 4b65 7924 7b75 6964 7d27 2063 6c61 7373  Key${uid}' class
+00005740: 3d27 7365 6172 6368 2d69 6e70 7574 2720  ='search-input' 
+00005750: 706c 6163 6568 6f6c 6465 723d 2745 6e74  placeholder='Ent
+00005760: 6572 2073 6561 7263 6820 6865 7265 202e  er search here .
+00005770: 2e2e 2720 202f 3e0a 2020 2020 2020 2020  ..'  />.        
+00005780: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+00005790: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+000057a0: 2020 2020 2020 203c 6275 7474 6f6e 2063         <button c
+000057b0: 6c61 7373 3d27 7365 6172 6368 2d62 7574  lass='search-but
+000057c0: 746f 6e27 2074 7970 653d 2262 7574 746f  ton' type="butto
+000057d0: 6e22 206f 6e63 6c69 636b 3d22 7365 6172  n" onclick="sear
+000057e0: 6368 4772 6964 247b 7569 647d 2865 6c65  chGrid${uid}(ele
+000057f0: 6d65 6e74 247b 7569 647d 2922 3e0a 2020  ment${uid})">.  
+00005800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005810: 2020 2020 2020 247b 7365 6172 6368 4963        ${searchIc
+00005820: 6f6e 7d0a 2020 2020 2020 2020 2020 2020  on}.            
+00005830: 2020 2020 2020 2020 2020 2020 3c73 7061              <spa
+00005840: 6e20 636c 6173 733d 2770 6c2d 3827 3e53  n class='pl-8'>S
+00005850: 6561 7263 683c 2f73 7061 6e3e 0a20 2020  earch</span>.   
+00005860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005870: 203c 2f62 7574 746f 6e3e 0a20 2020 2020   </button>.     
+00005880: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00005890: 3e0a 0a20 2020 2020 2020 2020 2020 2020  >..             
+000058a0: 2020 203c 6469 763e 3c68 3420 6964 3d27     <div><h4 id='
+000058b0: 746f 7461 6c24 7b75 6964 7d27 3e30 3c2f  total${uid}'>0</
+000058c0: 6834 3e3c 2f64 6976 3e0a 2020 2020 2020  h4></div>.      
+000058d0: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
+000058e0: 2020 2020 2020 2020 203c 6469 7620 6964           <div id
+000058f0: 3d27 7461 626c 6524 7b75 6964 7d27 2063  ='table${uid}' c
+00005900: 6c61 7373 3d27 6772 6964 2d74 6162 6c65  lass='grid-table
+00005910: 247b 7569 647d 2720 7374 796c 653d 276d  ${uid}' style='m
+00005920: 6172 6769 6e2d 746f 703a 2032 3570 783b  argin-top: 25px;
+00005930: 273e 0a20 2020 2020 2020 2020 2020 2020  '>.             
+00005940: 2020 203c 7363 7269 7074 3e0a 2020 2020     <script>.    
+00005950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005960: 6675 6e63 7469 6f6e 2070 6167 696e 6174  function paginat
+00005970: 6524 7b75 6964 7d28 6172 722c 2073 697a  e${uid}(arr, siz
+00005980: 6529 207b 0a20 2020 2020 2020 2020 2020  e) {.           
+00005990: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+000059a0: 7374 2072 6573 203d 205b 5d3b 0a20 2020  st res = [];.   
+000059b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059c0: 2020 2020 2066 6f72 2028 6c65 7420 6920       for (let i 
+000059d0: 3d20 303b 2069 203c 2061 7272 2e6c 656e  = 0; i < arr.len
+000059e0: 6774 683b 2069 202b 3d20 7369 7a65 2920  gth; i += size) 
+000059f0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00005a00: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00005a10: 6e73 7420 6368 756e 6b20 3d20 6172 722e  nst chunk = arr.
+00005a20: 736c 6963 6528 692c 2069 202b 2073 697a  slice(i, i + siz
+00005a30: 6529 3b0a 2020 2020 2020 2020 2020 2020  e);.            
 00005a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a50: 2020 2020 2020 2020 207d 2029 3b0a 2020           } );.  
-00005a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a70: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00005a50: 7265 732e 7075 7368 2863 6875 6e6b 293b  res.push(chunk);
+00005a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005a70: 2020 2020 2020 2020 207d 0a0a 2020 2020           }..    
 00005a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a90: 7265 7365 7442 7949 6424 7b75 6964 7d28  resetById${uid}(
-00005aa0: 2774 6162 6c65 247b 7569 647d 2729 3b0a  'table${uid}');.
-00005ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ac0: 2020 2020 2020 2020 7265 7365 7442 7949          resetByI
-00005ad0: 6424 7b75 6964 7d28 2770 6167 247b 7569  d${uid}('pag${ui
-00005ae0: 647d 2729 3b0a 2020 2020 2020 2020 2020  d}');.          
-00005af0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00005b00: 7375 6c74 203d 2070 6167 696e 6174 6524  sult = paginate$
-00005b10: 7b75 6964 7d28 7265 7375 6c74 2c20 7061  {uid}(result, pa
-00005b20: 6765 5f73 697a 6524 7b75 6964 7d29 0a20  ge_size${uid}). 
-00005b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b40: 2020 2020 2020 2070 6167 696e 6174 6564         paginated
-00005b50: 456c 656d 656e 7473 247b 7569 647d 203d  Elements${uid} =
-00005b60: 2072 6573 756c 740a 2020 2020 2020 2020   result.        
+00005a90: 2020 2020 7265 7475 726e 2072 6573 3b0a      return res;.
+00005aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ab0: 2020 2020 7d0a 0a20 2020 2020 2020 2020      }..         
+00005ac0: 2020 2020 2020 2020 2020 2066 756e 6374             funct
+00005ad0: 696f 6e20 7365 6172 6368 4772 6964 247b  ion searchGrid${
+00005ae0: 7569 647d 2865 6c65 6d65 6e74 7329 7b0a  uid}(elements){.
+00005af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b00: 2020 2020 2020 2020 6c65 7420 7365 6172          let sear
+00005b10: 6368 4b65 7920 3d20 646f 6375 6d65 6e74  chKey = document
+00005b20: 2e67 6574 456c 656d 656e 7442 7949 6428  .getElementById(
+00005b30: 2773 6561 7263 684b 6579 247b 7569 647d  'searchKey${uid}
+00005b40: 2729 2e76 616c 7565 3b0a 2020 2020 2020  ').value;.      
+00005b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b60: 2020 6c65 7420 7265 7375 6c74 3b0a 2020    let result;.  
 00005b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b80: 6275 696c 6447 7269 6424 7b75 6964 7d28  buildGrid${uid}(
-00005b90: 7265 7375 6c74 2c70 6167 6549 6e64 6578  result,pageIndex
-00005ba0: 247b 7569 647d 293b 0a20 2020 2020 2020  ${uid});.       
-00005bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bc0: 2062 7569 6c64 5061 6769 6e61 7469 6f6e   buildPagination
-00005bd0: 436f 6e74 6169 6e65 7224 7b75 6964 7d28  Container${uid}(
-00005be0: 7265 7375 6c74 293b 0a20 2020 2020 2020  result);.       
-00005bf0: 2020 2020 2020 2020 2020 2020 207d 0a0a               }..
-00005c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c10: 2020 2020 6675 6e63 7469 6f6e 2072 6573      function res
-00005c20: 6574 4279 4964 247b 7569 647d 2869 6429  etById${uid}(id)
-00005c30: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00005c40: 2020 2020 2020 2020 2020 6c65 7420 656c            let el
-00005c50: 656d 656e 7420 3d20 646f 6375 6d65 6e74  ement = document
-00005c60: 2e67 6574 456c 656d 656e 7442 7949 6428  .getElementById(
-00005c70: 6964 293b 0a20 2020 2020 2020 2020 2020  id);.           
-00005c80: 2020 2020 2020 2020 2020 2020 2077 6869               whi
-00005c90: 6c65 2028 656c 656d 656e 742e 6669 7273  le (element.firs
-00005ca0: 7443 6869 6c64 2920 7b0a 2020 2020 2020  tChild) {.      
-00005cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cc0: 2020 2020 656c 656d 656e 742e 7265 6d6f      element.remo
-00005cd0: 7665 4368 696c 6428 656c 656d 656e 742e  veChild(element.
-00005ce0: 6669 7273 7443 6869 6c64 293b 0a20 2020  firstChild);.   
-00005cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d00: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-00005d10: 2020 2020 2020 2020 2020 207d 0a0a 2020             }..  
-00005d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d30: 2020 6675 6e63 7469 6f6e 2062 7569 6c64    function build
-00005d40: 4772 6964 247b 7569 647d 2869 7465 6d73  Grid${uid}(items
-00005d50: 2c20 7061 6765 496e 6465 7829 7b0a 2020  , pageIndex){.  
-00005d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d70: 2020 2020 2020 2020 2020 2020 2020 6c65                le
-00005d80: 7420 6865 6164 6572 7320 3d20 4f62 6a65  t headers = Obje
-00005d90: 6374 2e6b 6579 7328 656c 656d 656e 7424  ct.keys(element$
-00005da0: 7b75 6964 7d5b 305d 293b 0a0a 2020 2020  {uid}[0]);..    
-00005db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005dc0: 2020 2020 2020 2020 2020 2020 6c65 7420              let 
-00005dd0: 6772 6964 203d 2064 6f63 756d 656e 742e  grid = document.
-00005de0: 6765 7445 6c65 6d65 6e74 4279 4964 2822  getElementById("
-00005df0: 7461 626c 6524 7b75 6964 7d22 293b 0a20  table${uid}");. 
-00005e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e10: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00005e20: 6574 2064 6976 203d 2064 6f63 756d 656e  et div = documen
-00005e30: 742e 6372 6561 7465 456c 656d 656e 7428  t.createElement(
-00005e40: 2264 6976 2229 3b0a 2020 2020 2020 2020  "div");.        
+00005b80: 2020 2020 2020 6966 2028 7365 6172 6368        if (search
+00005b90: 4b65 7920 3d3d 3d20 2727 297b 0a20 2020  Key === ''){.   
+00005ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005bb0: 2020 2020 2020 2020 2072 6573 756c 7420           result 
+00005bc0: 3d20 656c 656d 656e 7473 3b0a 2020 2020  = elements;.    
+00005bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005be0: 2020 2020 7d20 656c 7365 207b 0a20 2020      } else {.   
+00005bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c00: 2020 2020 2020 2020 2072 6573 756c 7420           result 
+00005c10: 3d20 656c 656d 656e 7473 2e66 696c 7465  = elements.filte
+00005c20: 7228 2865 6c65 6d65 6e74 2920 3d3e 207b  r((element) => {
+00005c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c50: 206c 6574 2070 726f 7065 7274 7920 3d20   let property = 
+00005c60: 656c 656d 656e 745b 6163 7469 7665 4669  element[activeFi
+00005c70: 6c74 6572 247b 7569 647d 5d0a 2020 2020  lter${uid}].    
+00005c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c90: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+00005ca0: 7479 7065 6f66 2070 726f 7065 7274 7920  typeof property 
+00005cb0: 3d3d 3d20 276f 626a 6563 7427 2026 2620  === 'object' && 
+00005cc0: 7072 6f70 6572 7479 2021 3d3d 206e 756c  property !== nul
+00005cd0: 6c29 7b0a 2020 2020 2020 2020 2020 2020  l){.            
+00005ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cf0: 2020 2020 2020 2020 7265 7475 726e 2070          return p
+00005d00: 726f 7065 7274 792e 7661 6c75 652e 746f  roperty.value.to
+00005d10: 4c6f 7765 7243 6173 6528 292e 696e 636c  LowerCase().incl
+00005d20: 7564 6573 2873 6561 7263 684b 6579 2e74  udes(searchKey.t
+00005d30: 6f4c 6f77 6572 4361 7365 2829 293b 0a20  oLowerCase());. 
+00005d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d50: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00005d60: 2065 6c73 6520 6966 2028 7479 7065 6f66   else if (typeof
+00005d70: 2070 726f 7065 7274 7920 3d3d 3d20 2773   property === 's
+00005d80: 7472 696e 6727 2029 207b 0a20 2020 2020  tring' ) {.     
+00005d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005da0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00005db0: 6574 7572 6e20 656c 656d 656e 745b 6163  eturn element[ac
+00005dc0: 7469 7665 4669 6c74 6572 247b 7569 647d  tiveFilter${uid}
+00005dd0: 5d2e 746f 4c6f 7765 7243 6173 6528 292e  ].toLowerCase().
+00005de0: 696e 636c 7564 6573 2873 6561 7263 684b  includes(searchK
+00005df0: 6579 2e74 6f4c 6f77 6572 4361 7365 2829  ey.toLowerCase()
+00005e00: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
+00005e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e20: 2020 207d 2065 6c73 6520 6966 2028 7072     } else if (pr
+00005e30: 6f70 6572 7479 2021 3d3d 206e 756c 6c20  operty !== null 
+00005e40: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
 00005e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e60: 2020 2020 2020 2020 6469 762e 636c 6173          div.clas
-00005e70: 734c 6973 742e 6164 6428 2767 7269 642d  sList.add('grid-
-00005e80: 6865 6164 6572 272c 2027 6772 6964 2d69  header', 'grid-i
-00005e90: 6e64 6578 2d63 656c 6c73 2729 3b0a 2020  ndex-cells');.  
-00005ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005eb0: 2020 2020 2020 2020 2020 2020 2020 6772                gr
-00005ec0: 6964 2e61 7070 656e 6443 6869 6c64 2864  id.appendChild(d
-00005ed0: 6976 293b 0a20 2020 2020 2020 2020 2020  iv);.           
+00005e60: 2020 2020 2020 2020 7265 7475 726e 2065          return e
+00005e70: 6c65 6d65 6e74 5b61 6374 6976 6546 696c  lement[activeFil
+00005e80: 7465 7224 7b75 6964 7d5d 2e74 6f53 7472  ter${uid}].toStr
+00005e90: 696e 6728 2920 3d3d 3d20 7365 6172 6368  ing() === search
+00005ea0: 4b65 793b 0a20 2020 2020 2020 2020 2020  Key;.           
+00005eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ec0: 2020 2020 207d 2065 6c73 6520 7b0a 2020       } else {.  
+00005ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ef0: 2020 2020 2068 6561 6465 7273 2e66 6f72       headers.for
-00005f00: 4561 6368 2828 7469 746c 6529 203d 3e7b  Each((title) =>{
-00005f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f30: 2020 2020 206c 6574 2064 6976 203d 2064       let div = d
-00005f40: 6f63 756d 656e 742e 6372 6561 7465 456c  ocument.createEl
-00005f50: 656d 656e 7428 2264 6976 2229 3b0a 2020  ement("div");.  
-00005f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f80: 2020 6469 762e 636c 6173 734c 6973 742e    div.classList.
-00005f90: 6164 6428 2767 7269 642d 6865 6164 6572  add('grid-header
-00005fa0: 272c 2027 6772 6964 2d73 7464 2d63 656c  ', 'grid-std-cel
-00005fb0: 6c73 2729 3b0a 2020 2020 2020 2020 2020  ls');.          
+00005ef0: 2020 7265 7475 726e 2065 6c65 6d65 6e74    return element
+00005f00: 5b61 6374 6976 6546 696c 7465 7224 7b75  [activeFilter${u
+00005f10: 6964 7d5d 203d 3d3d 2073 6561 7263 684b  id}] === searchK
+00005f20: 6579 3b0a 2020 2020 2020 2020 2020 2020  ey;.            
+00005f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f40: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+00005f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f60: 2020 7d20 293b 0a20 2020 2020 2020 2020    } );.         
+00005f70: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00005f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005f90: 2020 2020 2020 2020 2072 6573 6574 4279           resetBy
+00005fa0: 4964 247b 7569 647d 2827 7461 626c 6524  Id${uid}('table$
+00005fb0: 7b75 6964 7d27 293b 0a20 2020 2020 2020  {uid}');.       
 00005fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fd0: 2020 2020 2020 2020 2020 6469 762e 696e            div.in
-00005fe0: 6e65 7254 6578 7420 3d20 7469 746c 653b  nerText = title;
-00005ff0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006010: 2020 2020 2020 6772 6964 2e61 7070 656e        grid.appen
-00006020: 6443 6869 6c64 2864 6976 293b 0a20 2020  dChild(div);.   
-00006030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006040: 2020 2020 2020 2020 2020 2020 207d 293b               });
-00006050: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006070: 2020 6c65 7420 7061 6765 203d 2069 7465    let page = ite
-00006080: 6d73 5b70 6167 6549 6e64 6578 202d 315d  ms[pageIndex -1]
-00006090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000060a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060b0: 2069 6620 2870 6167 6520 213d 3d20 2775   if (page !== 'u
-000060c0: 6e64 6566 696e 6527 297b 0a20 2020 2020  ndefine'){.     
-000060d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060e0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000060f0: 6574 2074 6162 6c65 5f69 6e64 6578 247b  et table_index${
-00006100: 7569 647d 203d 2028 2870 6167 6549 6e64  uid} = ((pageInd
-00006110: 6578 202d 2031 2920 2a20 7061 6765 5f73  ex - 1) * page_s
-00006120: 697a 6524 7b75 6964 7d29 0a20 2020 2020  ize${uid}).     
-00006130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006140: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00006150: 6167 652e 666f 7245 6163 6828 2869 7465  age.forEach((ite
-00006160: 6d29 203d 3e20 7b0a 2020 2020 2020 2020  m) => {.        
-00006170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fd0: 2072 6573 6574 4279 4964 247b 7569 647d   resetById${uid}
+00005fe0: 2827 7061 6724 7b75 6964 7d27 293b 0a20  ('pag${uid}');. 
+00005ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006000: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00006010: 7061 6769 6e61 7465 247b 7569 647d 2872  paginate${uid}(r
+00006020: 6573 756c 742c 2070 6167 655f 7369 7a65  esult, page_size
+00006030: 247b 7569 647d 290a 2020 2020 2020 2020  ${uid}).        
+00006040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006050: 7061 6769 6e61 7465 6445 6c65 6d65 6e74  paginatedElement
+00006060: 7324 7b75 6964 7d20 3d20 7265 7375 6c74  s${uid} = result
+00006070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006080: 2020 2020 2020 2020 2062 7569 6c64 4772           buildGr
+00006090: 6964 247b 7569 647d 2872 6573 756c 742c  id${uid}(result,
+000060a0: 7061 6765 496e 6465 7824 7b75 6964 7d29  pageIndex${uid})
+000060b0: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+000060c0: 2020 2020 2020 2020 2020 6275 696c 6450            buildP
+000060d0: 6167 696e 6174 696f 6e43 6f6e 7461 696e  aginationContain
+000060e0: 6572 247b 7569 647d 2872 6573 756c 7429  er${uid}(result)
+000060f0: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+00006100: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+00006110: 2020 2020 2020 2020 2020 2020 2066 756e               fun
+00006120: 6374 696f 6e20 7265 7365 7442 7949 6424  ction resetById$
+00006130: 7b75 6964 7d28 6964 297b 0a20 2020 2020  {uid}(id){.     
+00006140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006150: 2020 206c 6574 2065 6c65 6d65 6e74 203d     let element =
+00006160: 2064 6f63 756d 656e 742e 6765 7445 6c65   document.getEle
+00006170: 6d65 6e74 4279 4964 2869 6429 3b0a 2020  mentById(id);.  
 00006180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006190: 6c65 7420 6772 6964 203d 2064 6f63 756d  let grid = docum
-000061a0: 656e 742e 6765 7445 6c65 6d65 6e74 4279  ent.getElementBy
-000061b0: 4964 2822 7461 626c 6524 7b75 6964 7d22  Id("table${uid}"
-000061c0: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
-000061d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061e0: 2020 2020 2020 2020 2020 202f 2f20 4164             // Ad
-000061f0: 6420 6e65 7720 696e 6465 7820 7661 6c75  d new index valu
-00006200: 6520 696e 2069 6e64 6578 2063 656c 6c73  e in index cells
-00006210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006230: 2020 2020 2020 2020 206c 6574 2064 6976           let div
-00006240: 496e 6465 7820 3d20 646f 6375 6d65 6e74  Index = document
-00006250: 2e63 7265 6174 6545 6c65 6d65 6e74 2822  .createElement("
-00006260: 6469 7622 293b 0a20 2020 2020 2020 2020  div");.         
+00006190: 2020 2020 2020 7768 696c 6520 2865 6c65        while (ele
+000061a0: 6d65 6e74 2e66 6972 7374 4368 696c 6429  ment.firstChild)
+000061b0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+000061c0: 2020 2020 2020 2020 2020 2020 2065 6c65               ele
+000061d0: 6d65 6e74 2e72 656d 6f76 6543 6869 6c64  ment.removeChild
+000061e0: 2865 6c65 6d65 6e74 2e66 6972 7374 4368  (element.firstCh
+000061f0: 696c 6429 3b0a 2020 2020 2020 2020 2020  ild);.          
+00006200: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00006210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006220: 2020 2020 7d0a 0a20 2020 2020 2020 2020      }..         
+00006230: 2020 2020 2020 2020 2020 2066 756e 6374             funct
+00006240: 696f 6e20 6275 696c 6447 7269 6424 7b75  ion buildGrid${u
+00006250: 6964 7d28 6974 656d 732c 2070 6167 6549  id}(items, pageI
+00006260: 6e64 6578 297b 0a20 2020 2020 2020 2020  ndex){.         
 00006270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006280: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00006290: 6976 496e 6465 782e 636c 6173 734c 6973  ivIndex.classLis
-000062a0: 742e 6164 6428 2767 7269 642d 726f 7727  t.add('grid-row'
-000062b0: 2c20 2767 7269 642d 696e 6465 782d 6365  , 'grid-index-ce
-000062c0: 6c6c 7327 293b 0a20 2020 2020 2020 2020  lls');.         
-000062d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062e0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000062f0: 6976 496e 6465 782e 696e 6e65 7254 6578  ivIndex.innerTex
-00006300: 7420 3d20 7461 626c 655f 696e 6465 7824  t = table_index$
-00006310: 7b75 6964 7d3b 0a20 2020 2020 2020 2020  {uid};.         
-00006320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006330: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-00006340: 7269 642e 6170 7065 6e64 4368 696c 6428  rid.appendChild(
-00006350: 6469 7649 6e64 6578 293b 0a0a 2020 2020  divIndex);..    
+00006280: 2020 2020 2020 206c 6574 2068 6561 6465         let heade
+00006290: 7273 203d 204f 626a 6563 742e 6b65 7973  rs = Object.keys
+000062a0: 2865 6c65 6d65 6e74 247b 7569 647d 5b30  (element${uid}[0
+000062b0: 5d29 3b0a 0a20 2020 2020 2020 2020 2020  ]);..           
+000062c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062d0: 2020 2020 206c 6574 2067 7269 6420 3d20       let grid = 
+000062e0: 646f 6375 6d65 6e74 2e67 6574 456c 656d  document.getElem
+000062f0: 656e 7442 7949 6428 2274 6162 6c65 247b  entById("table${
+00006300: 7569 647d 2229 3b0a 2020 2020 2020 2020  uid}");.        
+00006310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006320: 2020 2020 2020 2020 6c65 7420 6469 7620          let div 
+00006330: 3d20 646f 6375 6d65 6e74 2e63 7265 6174  = document.creat
+00006340: 6545 6c65 6d65 6e74 2822 6469 7622 293b  eElement("div");
+00006350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00006360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006380: 2020 2020 2f2f 2049 7465 7261 7465 206f      // Iterate o
-00006390: 7665 7220 7468 6520 6163 7475 616c 206f  ver the actual o
-000063a0: 626a 0a20 2020 2020 2020 2020 2020 2020  bj.             
+00006370: 2064 6976 2e63 6c61 7373 4c69 7374 2e61   div.classList.a
+00006380: 6464 2827 6772 6964 2d68 6561 6465 7227  dd('grid-header'
+00006390: 2c20 2767 7269 642d 696e 6465 782d 6365  , 'grid-index-ce
+000063a0: 6c6c 7327 293b 0a20 2020 2020 2020 2020  lls');.         
 000063b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063c0: 2020 2020 2020 2020 2020 2066 6f72 2028             for (
-000063d0: 636f 6e73 7420 6174 7472 2069 6e20 6974  const attr in it
-000063e0: 656d 2920 7b0a 2020 2020 2020 2020 2020  em) {.          
-000063f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006410: 2020 6c65 7420 6469 7620 3d20 646f 6375    let div = docu
-00006420: 6d65 6e74 2e63 7265 6174 6545 6c65 6d65  ment.createEleme
-00006430: 6e74 2822 6469 7622 293b 0a20 2020 2020  nt("div");.     
-00006440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006460: 2020 2020 2020 2069 6620 2874 7970 656f         if (typeo
-00006470: 6620 6974 656d 5b61 7474 725d 203d 3d3d  f item[attr] ===
-00006480: 2027 6f62 6a65 6374 270a 2020 2020 2020   'object'.      
-00006490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064b0: 2020 2020 2020 2020 2020 2626 2069 7465            && ite
-000064c0: 6d5b 6174 7472 5d20 213d 3d20 6e75 6c6c  m[attr] !== null
-000064d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000064e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006500: 2026 2620 6974 656d 5b61 7474 725d 2e68   && item[attr].h
-00006510: 6173 4f77 6e50 726f 7065 7274 7928 2774  asOwnProperty('t
-00006520: 7970 6527 2929 207b 0a20 2020 2020 2020  ype')) {.       
-00006530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063c0: 2020 2020 2020 2067 7269 642e 6170 7065         grid.appe
+000063d0: 6e64 4368 696c 6428 6469 7629 3b0a 2020  ndChild(div);.  
+000063e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063f0: 2020 2020 2020 2020 2020 2020 2020 6865                he
+00006400: 6164 6572 732e 666f 7245 6163 6828 2874  aders.forEach((t
+00006410: 6974 6c65 2920 3d3e 7b0a 2020 2020 2020  itle) =>{.      
+00006420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006430: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+00006440: 7420 6469 7620 3d20 646f 6375 6d65 6e74  t div = document
+00006450: 2e63 7265 6174 6545 6c65 6d65 6e74 2822  .createElement("
+00006460: 6469 7622 293b 0a20 2020 2020 2020 2020  div");.         
+00006470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006480: 2020 2020 2020 2020 2020 2064 6976 2e63             div.c
+00006490: 6c61 7373 4c69 7374 2e61 6464 2827 6772  lassList.add('gr
+000064a0: 6964 2d68 6561 6465 7227 2c20 2767 7269  id-header', 'gri
+000064b0: 642d 7374 642d 6365 6c6c 7324 7b75 6964  d-std-cells${uid
+000064c0: 7d27 293b 0a20 2020 2020 2020 2020 2020  }');.           
+000064d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064e0: 2020 2020 2020 2020 2064 6976 2e69 6e6e           div.inn
+000064f0: 6572 5465 7874 203d 2074 6974 6c65 3b0a  erText = title;.
+00006500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006520: 2020 2020 2067 7269 642e 6170 7065 6e64       grid.append
+00006530: 4368 696c 6428 6469 7629 3b0a 2020 2020  Child(div);.    
 00006540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006550: 2020 2020 2020 2020 2069 6620 2869 7465           if (ite
-00006560: 6d5b 6174 7472 5d2e 7479 7065 2e69 6e63  m[attr].type.inc
-00006570: 6c75 6465 7328 2762 6164 6765 2729 297b  ludes('badge')){
-00006580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006550: 2020 2020 2020 2020 2020 2020 7d29 3b0a              });.
+00006560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006580: 206c 6574 2070 6167 6520 3d20 6974 656d   let page = item
+00006590: 735b 7061 6765 496e 6465 7820 2d31 5d0a  s[pageIndex -1].
 000065a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065b0: 2020 2020 206c 6574 2062 6164 6765 5f64       let badge_d
-000065c0: 6976 203d 2064 6f63 756d 656e 742e 6372  iv = document.cr
-000065d0: 6561 7465 456c 656d 656e 7428 2264 6976  eateElement("div
-000065e0: 2229 3b0a 2020 2020 2020 2020 2020 2020  ");.            
-000065f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006610: 2020 2020 2020 2020 6261 6467 655f 6469          badge_di
-00006620: 762e 636c 6173 734c 6973 742e 6164 6428  v.classList.add(
-00006630: 2762 6164 6765 272c 6974 656d 5b61 7474  'badge',item[att
-00006640: 725d 2e74 7970 6529 0a20 2020 2020 2020  r].type).       
-00006650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006670: 2020 2020 2020 2020 2020 2020 2062 6164               bad
-00006680: 6765 5f64 6976 2e69 6e6e 6572 5465 7874  ge_div.innerText
-00006690: 203d 2053 7472 696e 6728 6974 656d 5b61   = String(item[a
-000066a0: 7474 725d 2e76 616c 7565 292e 746f 5570  ttr].value).toUp
-000066b0: 7065 7243 6173 6528 293b 0a20 2020 2020  perCase();.     
-000066c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066e0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000066f0: 6976 2e61 7070 656e 6443 6869 6c64 2862  iv.appendChild(b
-00006700: 6164 6765 5f64 6976 293b 0a20 2020 2020  adge_div);.     
-00006710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006730: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00006740: 6976 2e63 6c61 7373 4c69 7374 2e61 6464  iv.classList.add
-00006750: 2827 6772 6964 2d72 6f77 272c 2767 7269  ('grid-row','gri
-00006760: 642d 7374 642d 6365 6c6c 7327 293b 0a20  d-std-cells');. 
-00006770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065c0: 6966 2028 7061 6765 2021 3d3d 2027 756e  if (page !== 'un
+000065d0: 6465 6669 6e65 6427 297b 0a20 2020 2020  defined'){.     
+000065e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065f0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00006600: 6574 2074 6162 6c65 5f69 6e64 6578 247b  et table_index${
+00006610: 7569 647d 203d 2028 2870 6167 6549 6e64  uid} = ((pageInd
+00006620: 6578 202d 2031 2920 2a20 7061 6765 5f73  ex - 1) * page_s
+00006630: 697a 6524 7b75 6964 7d29 0a20 2020 2020  ize${uid}).     
+00006640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006650: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00006660: 6167 652e 666f 7245 6163 6828 2869 7465  age.forEach((ite
+00006670: 6d29 203d 3e20 7b0a 2020 2020 2020 2020  m) => {.        
+00006680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066a0: 6c65 7420 6772 6964 203d 2064 6f63 756d  let grid = docum
+000066b0: 656e 742e 6765 7445 6c65 6d65 6e74 4279  ent.getElementBy
+000066c0: 4964 2822 7461 626c 6524 7b75 6964 7d22  Id("table${uid}"
+000066d0: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
+000066e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066f0: 2020 2020 2020 2020 2020 202f 2f20 4164             // Ad
+00006700: 6420 6e65 7720 696e 6465 7820 7661 6c75  d new index valu
+00006710: 6520 696e 2069 6e64 6578 2063 656c 6c73  e in index cells
+00006720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006740: 2020 2020 2020 2020 206c 6574 2064 6976           let div
+00006750: 496e 6465 7820 3d20 646f 6375 6d65 6e74  Index = document
+00006760: 2e63 7265 6174 6545 6c65 6d65 6e74 2822  .createElement("
+00006770: 6469 7622 293b 0a20 2020 2020 2020 2020  div");.         
 00006780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006790: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-000067a0: 2065 6c73 6520 6966 2028 6974 656d 5b61   else if (item[a
-000067b0: 7474 725d 2e74 7970 652e 696e 636c 7564  ttr].type.includ
-000067c0: 6573 2827 6c61 6265 6c27 2929 7b0a 2020  es('label')){.  
-000067d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006790: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000067a0: 6976 496e 6465 782e 636c 6173 734c 6973  ivIndex.classLis
+000067b0: 742e 6164 6428 2767 7269 642d 726f 7727  t.add('grid-row'
+000067c0: 2c20 2767 7269 642d 696e 6465 782d 6365  , 'grid-index-ce
+000067d0: 6c6c 7327 293b 0a20 2020 2020 2020 2020  lls');.         
 000067e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006800: 2020 6c65 7420 6c61 6265 6c5f 6469 7620    let label_div 
-00006810: 3d20 646f 6375 6d65 6e74 2e63 7265 6174  = document.creat
-00006820: 6545 6c65 6d65 6e74 2822 6469 7622 293b  eElement("div");
-00006830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006860: 2020 2020 206c 6162 656c 5f64 6976 2e63       label_div.c
-00006870: 6c61 7373 4c69 7374 2e61 6464 2827 6c61  lassList.add('la
-00006880: 6265 6c27 2c69 7465 6d5b 6174 7472 5d2e  bel',item[attr].
-00006890: 7479 7065 290a 2020 2020 2020 2020 2020  type).          
-000068a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068c0: 2020 2020 2020 2020 2020 6c61 6265 6c5f            label_
-000068d0: 6469 762e 696e 6e65 7254 6578 7420 3d20  div.innerText = 
-000068e0: 5374 7269 6e67 2869 7465 6d5b 6174 7472  String(item[attr
-000068f0: 5d2e 7661 6c75 6529 2e74 6f55 7070 6572  ].value).toUpper
-00006900: 4361 7365 2829 3b0a 2020 2020 2020 2020  Case();.        
+000067f0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00006800: 6976 496e 6465 782e 696e 6e65 7254 6578  ivIndex.innerTex
+00006810: 7420 3d20 7461 626c 655f 696e 6465 7824  t = table_index$
+00006820: 7b75 6964 7d3b 0a20 2020 2020 2020 2020  {uid};.         
+00006830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006840: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+00006850: 7269 642e 6170 7065 6e64 4368 696c 6428  rid.appendChild(
+00006860: 6469 7649 6e64 6578 293b 0a0a 2020 2020  divIndex);..    
+00006870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006890: 2020 2020 2f2f 2049 7465 7261 7465 206f      // Iterate o
+000068a0: 7665 7220 7468 6520 6163 7475 616c 206f  ver the actual o
+000068b0: 626a 0a20 2020 2020 2020 2020 2020 2020  bj.             
+000068c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068d0: 2020 2020 2020 2020 2020 2066 6f72 2028             for (
+000068e0: 636f 6e73 7420 6174 7472 2069 6e20 6974  const attr in it
+000068f0: 656d 2920 7b0a 2020 2020 2020 2020 2020  em) {.          
+00006900: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006930: 2020 2020 2020 2020 2020 2020 6469 762e              div.
-00006940: 6170 7065 6e64 4368 696c 6428 6c61 6265  appendChild(labe
-00006950: 6c5f 6469 7629 3b0a 2020 2020 2020 2020  l_div);.        
+00006920: 2020 6c65 7420 6469 7620 3d20 646f 6375    let div = docu
+00006930: 6d65 6e74 2e63 7265 6174 6545 6c65 6d65  ment.createEleme
+00006940: 6e74 2822 6469 7622 293b 0a20 2020 2020  nt("div");.     
+00006950: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006980: 2020 2020 2020 2020 2020 2020 6469 762e              div.
-00006990: 636c 6173 734c 6973 742e 6164 6428 2767  classList.add('g
-000069a0: 7269 642d 726f 7727 2c27 6772 6964 2d73  rid-row','grid-s
-000069b0: 7464 2d63 656c 6c73 2729 3b0a 2020 2020  td-cells');.    
-000069c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069e0: 2020 2020 2020 2020 2020 2020 7d20 656c              } el
-000069f0: 7365 2069 6620 2869 7465 6d5b 6174 7472  se if (item[attr
-00006a00: 5d2e 7479 7065 203d 3d3d 2022 636c 6970  ].type === "clip
-00006a10: 626f 6172 6422 2920 7b0a 2020 2020 2020  board") {.      
-00006a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a40: 2020 2020 2020 2020 2020 2020 2020 6469                di
-00006a50: 762e 636c 6173 734c 6973 742e 6164 6428  v.classList.add(
-00006a60: 2767 7269 642d 726f 7727 2c27 6772 6964  'grid-row','grid
-00006a70: 2d73 7464 2d63 656c 6c73 2729 3b0a 0a20  -std-cells');.. 
-00006a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006970: 2020 2020 2020 2069 6620 2874 7970 656f         if (typeo
+00006980: 6620 6974 656d 5b61 7474 725d 203d 3d3d  f item[attr] ===
+00006990: 2027 6f62 6a65 6374 270a 2020 2020 2020   'object'.      
+000069a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069c0: 2020 2020 2020 2020 2020 2626 2069 7465            && ite
+000069d0: 6d5b 6174 7472 5d20 213d 3d20 6e75 6c6c  m[attr] !== null
+000069e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000069f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a10: 2026 2620 6974 656d 5b61 7474 725d 2e68   && item[attr].h
+00006a20: 6173 4f77 6e50 726f 7065 7274 7928 2774  asOwnProperty('t
+00006a30: 7970 6527 2929 207b 0a20 2020 2020 2020  ype')) {.       
+00006a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a60: 2020 2020 2020 2020 2069 6620 2869 7465           if (ite
+00006a70: 6d5b 6174 7472 5d2e 7479 7065 2e69 6e63  m[attr].type.inc
+00006a80: 6c75 6465 7328 2762 6164 6765 2729 297b  ludes('badge')){
+00006a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00006aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ab0: 2020 202f 2f20 4372 6561 7465 2063 6c69     // Create cli
-00006ac0: 7062 6f61 7264 2064 6976 0a20 2020 2020  pboard div.     
-00006ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006af0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00006b00: 6574 2063 6c69 7062 6f61 7264 5f64 6976  et clipboard_div
-00006b10: 203d 2064 6f63 756d 656e 742e 6372 6561   = document.crea
-00006b20: 7465 456c 656d 656e 7428 2764 6976 2729  teElement('div')
-00006b30: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-00006b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b60: 2020 2020 2020 636c 6970 626f 6172 645f        clipboard_
-00006b70: 6469 762e 7374 796c 652e 6469 7370 6c61  div.style.displa
-00006b80: 793d 2027 666c 6578 273b 0a20 2020 2020  y= 'flex';.     
-00006b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bb0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00006bc0: 6c69 7062 6f61 7264 5f64 6976 2e63 6c61  lipboard_div.cla
-00006bd0: 7373 4c69 7374 2e61 6464 2822 6761 702d  ssList.add("gap-
-00006be0: 3130 2229 0a20 2020 2020 2020 2020 2020  10").           
-00006bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c10: 2020 2020 2020 2020 2063 6c69 7062 6f61           clipboa
-00006c20: 7264 5f64 6976 2e73 7479 6c65 2e6a 7573  rd_div.style.jus
-00006c30: 7469 6679 436f 6e74 656e 7420 3d20 2273  tifyContent = "s
-00006c40: 7061 6365 2d62 6574 7765 656e 223b 0a0a  pace-between";..
-00006c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c80: 2020 2020 6c65 7420 6964 5f74 6578 7420      let id_text 
-00006c90: 3d20 646f 6375 6d65 6e74 2e63 7265 6174  = document.creat
-00006ca0: 6545 6c65 6d65 6e74 2827 6469 7627 293b  eElement('div');
-00006cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ce0: 2020 2020 2069 6620 2869 7465 6d5b 6174       if (item[at
-00006cf0: 7472 5d2e 7661 6c75 6520 3d3d 2022 4e6f  tr].value == "No
-00006d00: 6e65 2229 7b0a 2020 2020 2020 2020 2020  ne"){.          
-00006d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d30: 2020 2020 2020 2020 2020 2020 2020 6964                id
-00006d40: 5f74 6578 742e 696e 6e65 7254 6578 7420  _text.innerText 
-00006d50: 3d20 224e 6f6e 6522 3b0a 2020 2020 2020  = "None";.      
+00006ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ac0: 2020 2020 206c 6574 2062 6164 6765 5f64       let badge_d
+00006ad0: 6976 203d 2064 6f63 756d 656e 742e 6372  iv = document.cr
+00006ae0: 6561 7465 456c 656d 656e 7428 2264 6976  eateElement("div
+00006af0: 2229 3b0a 2020 2020 2020 2020 2020 2020  ");.            
+00006b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b20: 2020 2020 2020 2020 6261 6467 655f 6469          badge_di
+00006b30: 762e 636c 6173 734c 6973 742e 6164 6428  v.classList.add(
+00006b40: 2762 6164 6765 272c 6974 656d 5b61 7474  'badge',item[att
+00006b50: 725d 2e74 7970 6529 0a20 2020 2020 2020  r].type).       
+00006b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b80: 2020 2020 2020 2020 2020 2020 2062 6164               bad
+00006b90: 6765 5f64 6976 2e69 6e6e 6572 5465 7874  ge_div.innerText
+00006ba0: 203d 2053 7472 696e 6728 6974 656d 5b61   = String(item[a
+00006bb0: 7474 725d 2e76 616c 7565 292e 746f 5570  ttr].value).toUp
+00006bc0: 7065 7243 6173 6528 293b 0a20 2020 2020  perCase();.     
+00006bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006bf0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00006c00: 6976 2e61 7070 656e 6443 6869 6c64 2862  iv.appendChild(b
+00006c10: 6164 6765 5f64 6976 293b 0a20 2020 2020  adge_div);.     
+00006c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c40: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00006c50: 6976 2e63 6c61 7373 4c69 7374 2e61 6464  iv.classList.add
+00006c60: 2827 6772 6964 2d72 6f77 272c 2767 7269  ('grid-row','gri
+00006c70: 642d 7374 642d 6365 6c6c 7324 7b75 6964  d-std-cells${uid
+00006c80: 7d27 293b 0a20 2020 2020 2020 2020 2020  }');.           
+00006c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006cb0: 2020 2020 207d 2065 6c73 6520 6966 2028       } else if (
+00006cc0: 6974 656d 5b61 7474 725d 2e74 7970 652e  item[attr].type.
+00006cd0: 696e 636c 7564 6573 2827 6c61 6265 6c27  includes('label'
+00006ce0: 2929 7b0a 2020 2020 2020 2020 2020 2020  )){.            
+00006cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d10: 2020 2020 2020 2020 6c65 7420 6c61 6265          let labe
+00006d20: 6c5f 6469 7620 3d20 646f 6375 6d65 6e74  l_div = document
+00006d30: 2e63 7265 6174 6545 6c65 6d65 6e74 2822  .createElement("
+00006d40: 6469 7622 293b 0a20 2020 2020 2020 2020  div");.         
+00006d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d80: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00006d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d70: 2020 2020 2020 2020 2020 206c 6162 656c             label
+00006d80: 5f64 6976 2e63 6c61 7373 4c69 7374 2e61  _div.classList.a
+00006d90: 6464 2827 6c61 6265 6c27 2c69 7465 6d5b  dd('label',item[
+00006da0: 6174 7472 5d2e 7479 7065 290a 2020 2020  attr].type).    
 00006db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006dc0: 2020 2020 656c 7365 7b0a 2020 2020 2020      else{.      
+00006dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e00: 2020 6964 5f74 6578 742e 696e 6e65 7254    id_text.innerT
-00006e10: 6578 7420 3d20 6974 656d 5b61 7474 725d  ext = item[attr]
-00006e20: 2e76 616c 7565 2e73 6c69 6365 2830 2c35  .value.slice(0,5
-00006e30: 2920 2b20 222e 2e2e 223b 0a20 2020 2020  ) + "...";.     
+00006de0: 6c61 6265 6c5f 6469 762e 696e 6e65 7254  label_div.innerT
+00006df0: 6578 7420 3d20 5374 7269 6e67 2869 7465  ext = String(ite
+00006e00: 6d5b 6174 7472 5d2e 7661 6c75 6529 2e74  m[attr].value).t
+00006e10: 6f55 7070 6572 4361 7365 2829 3b0a 2020  oUpperCase();.  
+00006e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e60: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00006e70: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e50: 2020 6c61 6265 6c5f 6469 762e 636c 6173    label_div.clas
+00006e60: 734c 6973 742e 6164 6428 2763 656e 7465  sList.add('cente
+00006e70: 722d 636f 6e74 656e 742d 6365 6c6c 2729  r-content-cell')
+00006e80: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
 00006e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ea0: 2020 2020 2020 636c 6970 626f 6172 645f        clipboard_
-00006eb0: 6469 762e 6170 7065 6e64 4368 696c 6428  div.appendChild(
-00006ec0: 6964 5f74 6578 7429 3b0a 2020 2020 2020  id_text);.      
-00006ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006eb0: 2020 2020 2020 6469 762e 6170 7065 6e64        div.append
+00006ec0: 4368 696c 6428 6c61 6265 6c5f 6469 7629  Child(label_div)
+00006ed0: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
 00006ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ef0: 2020 2020 2020 2020 2020 2020 2020 6c65                le
-00006f00: 7420 636c 6970 626f 6172 645f 696d 6720  t clipboard_img 
-00006f10: 3d20 646f 6375 6d65 6e74 2e63 7265 6174  = document.creat
-00006f20: 6545 6c65 6d65 6e74 2827 6469 7627 293b  eElement('div');
-00006f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f00: 2020 2020 2020 6469 762e 636c 6173 734c        div.classL
+00006f10: 6973 742e 6164 6428 2767 7269 642d 726f  ist.add('grid-ro
+00006f20: 7727 2c27 6772 6964 2d73 7464 2d63 656c  w','grid-std-cel
+00006f30: 6c73 247b 7569 647d 2729 3b0a 2020 2020  ls${uid}');.    
 00006f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f60: 2020 2020 2063 6c69 7062 6f61 7264 5f69       clipboard_i
-00006f70: 6d67 2e63 6c61 7373 4c69 7374 2e61 6464  mg.classList.add
-00006f80: 2822 636c 6970 626f 6172 6422 290a 2020  ("clipboard").  
-00006f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f60: 2020 2020 2020 2020 2020 2020 7d20 656c              } el
+00006f70: 7365 2069 6620 2869 7465 6d5b 6174 7472  se if (item[attr
+00006f80: 5d2e 7479 7065 203d 3d3d 2022 636c 6970  ].type === "clip
+00006f90: 626f 6172 6422 2920 7b0a 2020 2020 2020  board") {.      
 00006fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fc0: 2020 6469 762e 6f6e 636c 6963 6b20 3d20    div.onclick = 
-00006fd0: 6675 6e63 7469 6f6e 2829 207b 0a20 2020  function() {.   
-00006fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007010: 2020 2020 206e 6176 6967 6174 6f72 2e63       navigator.c
-00007020: 6c69 7062 6f61 7264 2e77 7269 7465 5465  lipboard.writeTe
-00007030: 7874 2869 7465 6d5b 6174 7472 5d2e 7661  xt(item[attr].va
-00007040: 6c75 6529 3b0a 2020 2020 2020 2020 2020  lue);.          
-00007050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fc0: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00006fd0: 762e 636c 6173 734c 6973 742e 6164 6428  v.classList.add(
+00006fe0: 2767 7269 642d 726f 7727 2c27 6772 6964  'grid-row','grid
+00006ff0: 2d73 7464 2d63 656c 6c73 247b 7569 647d  -std-cells${uid}
+00007000: 2729 3b0a 0a20 2020 2020 2020 2020 2020  ');..           
+00007010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007030: 2020 2020 2020 2020 202f 2f20 4372 6561           // Crea
+00007040: 7465 2063 6c69 7062 6f61 7264 2064 6976  te clipboard div
+00007050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00007060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007070: 2020 2020 2020 2020 2020 7d3b 0a20 2020            };.   
-00007080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070b0: 2063 6c69 7062 6f61 7264 5f69 6d67 2e69   clipboard_img.i
-000070c0: 6e6e 6572 4854 4d4c 203d 2022 247b 636c  nnerHTML = "${cl
-000070d0: 6970 626f 6172 6449 636f 6e7d 223b 0a0a  ipboardIcon}";..
-000070e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007110: 2020 2020 636c 6970 626f 6172 645f 6469      clipboard_di
-00007120: 762e 6170 7065 6e64 4368 696c 6428 636c  v.appendChild(cl
-00007130: 6970 626f 6172 645f 696d 6729 3b0a 2020  ipboard_img);.  
-00007140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007170: 2020 6469 762e 6170 7065 6e64 4368 696c    div.appendChil
-00007180: 6428 636c 6970 626f 6172 645f 6469 7629  d(clipboard_div)
-00007190: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-000071a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071c0: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-000071d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007080: 2020 2020 206c 6574 2063 6c69 7062 6f61       let clipboa
+00007090: 7264 5f64 6976 203d 2064 6f63 756d 656e  rd_div = documen
+000070a0: 742e 6372 6561 7465 456c 656d 656e 7428  t.createElement(
+000070b0: 2764 6976 2729 3b0a 2020 2020 2020 2020  'div');.        
+000070c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070e0: 2020 2020 2020 2020 2020 2020 636c 6970              clip
+000070f0: 626f 6172 645f 6469 762e 7374 796c 652e  board_div.style.
+00007100: 6469 7370 6c61 793d 2027 666c 6578 273b  display= 'flex';
+00007110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007140: 2020 2020 2063 6c69 7062 6f61 7264 5f64       clipboard_d
+00007150: 6976 2e63 6c61 7373 4c69 7374 2e61 6464  iv.classList.add
+00007160: 2822 6761 702d 3130 2229 0a20 2020 2020  ("gap-10").     
+00007170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007190: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000071a0: 6c69 7062 6f61 7264 5f64 6976 2e73 7479  lipboard_div.sty
+000071b0: 6c65 2e6a 7573 7469 6679 436f 6e74 656e  le.justifyConten
+000071c0: 7420 3d20 2273 7061 6365 2d62 6574 7765  t = "space-betwe
+000071d0: 656e 223b 0a0a 2020 2020 2020 2020 2020  en";..          
 000071e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071f0: 7d20 656c 7365 7b0a 2020 2020 2020 2020  } else{.        
-00007200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007220: 2020 2020 2020 2020 6469 762e 636c 6173          div.clas
-00007230: 734c 6973 742e 6164 6428 2767 7269 642d  sList.add('grid-
-00007240: 726f 7727 2c27 6772 6964 2d73 7464 2d63  row','grid-std-c
-00007250: 656c 6c73 2729 3b0a 2020 2020 2020 2020  ells');.        
-00007260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007280: 2020 2020 2020 2020 6966 2028 6974 656d          if (item
-00007290: 5b61 7474 725d 203d 3d20 6e75 6c6c 2920  [attr] == null) 
-000072a0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+000071f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007200: 2020 2020 2020 2020 2020 6c65 7420 6964            let id
+00007210: 5f74 6578 7420 3d20 646f 6375 6d65 6e74  _text = document
+00007220: 2e63 7265 6174 6545 6c65 6d65 6e74 2827  .createElement('
+00007230: 6469 7627 293b 0a20 2020 2020 2020 2020  div');.         
+00007240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007260: 2020 2020 2020 2020 2020 2069 6620 2869             if (i
+00007270: 7465 6d5b 6174 7472 5d2e 7661 6c75 6520  tem[attr].value 
+00007280: 3d3d 2022 4e6f 6e65 2229 7b0a 2020 2020  == "None"){.    
+00007290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000072b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072d0: 2020 2020 2020 7465 7874 203d 2027 2027        text = ' '
-000072e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000072c0: 2020 2020 6964 5f74 6578 742e 696e 6e65      id_text.inne
+000072d0: 7254 6578 7420 3d20 224e 6f6e 6522 3b0a  rText = "None";.
+000072e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000072f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007310: 207d 2065 6c73 6520 7b0a 2020 2020 2020   } else {.      
+00007310: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
 00007320: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007340: 2020 2020 2020 2020 2020 2020 2020 7465                te
-00007350: 7874 203d 2053 7472 696e 6728 6974 656d  xt = String(item
-00007360: 5b61 7474 725d 290a 2020 2020 2020 2020  [attr]).        
+00007340: 2020 2020 2020 2020 2020 656c 7365 7b0a            else{.
+00007350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007360: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007390: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
-000073a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073c0: 2020 2020 2020 2020 2020 2074 6578 7420             text 
-000073d0: 3d20 7465 7874 2e72 6570 6c61 6365 416c  = text.replaceAl
-000073e0: 6c28 225c 5c6e 222c 2022 3c2f 6272 3e22  l("\\n", "</br>"
-000073f0: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
+00007380: 2020 2020 2020 2020 6964 5f74 6578 742e          id_text.
+00007390: 696e 6e65 7254 6578 7420 3d20 6974 656d  innerText = item
+000073a0: 5b61 7474 725d 2e76 616c 7565 2e73 6c69  [attr].value.sli
+000073b0: 6365 2830 2c35 2920 2b20 222e 2e2e 223b  ce(0,5) + "...";
+000073c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000073d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073f0: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
 00007400: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007420: 2020 2064 6976 2e69 6e6e 6572 4854 4d4c     div.innerHTML
-00007430: 203d 2074 6578 743b 0a20 2020 2020 2020   = text;.       
-00007440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007420: 2020 2020 2020 2020 2020 2020 636c 6970              clip
+00007430: 626f 6172 645f 6469 762e 6170 7065 6e64  board_div.append
+00007440: 4368 696c 6428 6964 5f74 6578 7429 3b0a  Child(id_text);.
 00007450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007460: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
+00007460: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007490: 2020 2067 7269 642e 6170 7065 6e64 4368     grid.appendCh
-000074a0: 696c 6428 6469 7629 3b0a 2020 2020 2020  ild(div);.      
-000074b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007480: 2020 2020 6c65 7420 636c 6970 626f 6172      let clipboar
+00007490: 645f 696d 6720 3d20 646f 6375 6d65 6e74  d_img = document
+000074a0: 2e63 7265 6174 6545 6c65 6d65 6e74 2827  .createElement('
+000074b0: 6469 7627 293b 0a20 2020 2020 2020 2020  div');.         
 000074c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074d0: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-000074e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074f0: 2020 2020 2020 2020 7461 626c 655f 696e          table_in
-00007500: 6465 7824 7b75 6964 7d20 3d20 7461 626c  dex${uid} = tabl
-00007510: 655f 696e 6465 7824 7b75 6964 7d20 2b20  e_index${uid} + 
-00007520: 313b 0a20 2020 2020 2020 2020 2020 2020  1;.             
+000074d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074e0: 2020 2020 2020 2020 2020 2063 6c69 7062             clipb
+000074f0: 6f61 7264 5f69 6d67 2e63 6c61 7373 4c69  oard_img.classLi
+00007500: 7374 2e61 6464 2822 636c 6970 626f 6172  st.add("clipboar
+00007510: 6422 290a 2020 2020 2020 2020 2020 2020  d").            
+00007520: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007540: 2020 2020 2020 207d 290a 2020 2020 2020         }).      
-00007550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007560: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00007540: 2020 2020 2020 2020 6469 762e 6f6e 636c          div.oncl
+00007550: 6963 6b20 3d20 6675 6e63 7469 6f6e 2829  ick = function()
+00007560: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
 00007570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007580: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00007590: 2020 2020 2020 7061 6769 6e61 7465 6445        paginatedE
-000075a0: 6c65 6d65 6e74 7324 7b75 6964 7d20 3d20  lements${uid} = 
-000075b0: 7061 6769 6e61 7465 247b 7569 647d 2865  paginate${uid}(e
-000075c0: 6c65 6d65 6e74 247b 7569 647d 2c20 7061  lement${uid}, pa
-000075d0: 6765 5f73 697a 6524 7b75 6964 7d29 0a20  ge_size${uid}). 
+00007580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007590: 2020 2020 2020 2020 2020 206e 6176 6967             navig
+000075a0: 6174 6f72 2e63 6c69 7062 6f61 7264 2e77  ator.clipboard.w
+000075b0: 7269 7465 5465 7874 2869 7465 6d5b 6174  riteText(item[at
+000075c0: 7472 5d2e 7661 6c75 6529 3b0a 2020 2020  tr].value);.    
+000075d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000075e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075f0: 2020 2062 7569 6c64 4772 6964 247b 7569     buildGrid${ui
-00007600: 647d 2870 6167 696e 6174 6564 456c 656d  d}(paginatedElem
-00007610: 656e 7473 247b 7569 647d 2c20 3129 0a20  ents${uid}, 1). 
+000075f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007600: 7d3b 0a20 2020 2020 2020 2020 2020 2020  };.             
+00007610: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007630: 2020 2064 6f63 756d 656e 742e 6765 7445     document.getE
-00007640: 6c65 6d65 6e74 4279 4964 2827 746f 7461  lementById('tota
-00007650: 6c24 7b75 6964 7d27 292e 696e 6e65 7254  l${uid}').innerT
-00007660: 6578 7420 3d20 2254 6f74 616c 3a20 2220  ext = "Total: " 
-00007670: 2b20 656c 656d 656e 7424 7b75 6964 7d2e  + element${uid}.
-00007680: 6c65 6e67 7468 0a20 2020 2020 2020 2020  length.         
-00007690: 2020 2020 2020 203c 2f73 6372 6970 743e         </script>
-000076a0: 0a20 2020 2020 2020 2020 2020 203c 2f64  .            </d
-000076b0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-000076c0: 3c64 6976 2069 643d 2770 6167 247b 7569  <div id='pag${ui
-000076d0: 647d 2720 636c 6173 733d 2770 6167 696e  d}' class='pagin
-000076e0: 6174 696f 6e43 6f6e 7461 696e 6572 273e  ationContainer'>
-000076f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007700: 203c 7363 7269 7074 3e0a 2020 2020 2020   <script>.      
-00007710: 2020 2020 2020 2020 2020 2020 2020 6675                fu
-00007720: 6e63 7469 6f6e 2062 7569 6c64 5061 6769  nction buildPagi
-00007730: 6e61 7469 6f6e 436f 6e74 6169 6e65 7224  nationContainer$
-00007740: 7b75 6964 7d28 7061 6769 6e61 7465 6445  {uid}(paginatedE
-00007750: 6c65 6d65 6e74 7329 7b0a 2020 2020 2020  lements){.      
+00007630: 2020 2020 2020 2063 6c69 7062 6f61 7264         clipboard
+00007640: 5f69 6d67 2e69 6e6e 6572 4854 4d4c 203d  _img.innerHTML =
+00007650: 2022 247b 636c 6970 626f 6172 6449 636f   "${clipboardIco
+00007660: 6e7d 223b 0a0a 2020 2020 2020 2020 2020  n}";..          
+00007670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007690: 2020 2020 2020 2020 2020 636c 6970 626f            clipbo
+000076a0: 6172 645f 6469 762e 6170 7065 6e64 4368  ard_div.appendCh
+000076b0: 696c 6428 636c 6970 626f 6172 645f 696d  ild(clipboard_im
+000076c0: 6729 3b0a 2020 2020 2020 2020 2020 2020  g);.            
+000076d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076f0: 2020 2020 2020 2020 6469 762e 6170 7065          div.appe
+00007700: 6e64 4368 696c 6428 636c 6970 626f 6172  ndChild(clipboar
+00007710: 645f 6469 7629 3b0a 2020 2020 2020 2020  d_div);.        
+00007720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007740: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00007750: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007770: 2020 2020 2020 6c65 7420 7061 6765 436f        let pageCo
-00007780: 6e74 6169 6e65 7220 3d20 646f 6375 6d65  ntainer = docume
-00007790: 6e74 2e67 6574 456c 656d 656e 7442 7949  nt.getElementByI
-000077a0: 6428 2270 6167 247b 7569 647d 2229 3b0a  d("pag${uid}");.
-000077b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077c0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000077d0: 286c 6574 2069 203d 2030 3b20 6920 3c20  (let i = 0; i < 
-000077e0: 7061 6769 6e61 7465 6445 6c65 6d65 6e74  paginatedElement
-000077f0: 732e 6c65 6e67 7468 3b20 692b 2b29 207b  s.length; i++) {
-00007800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007820: 2020 206c 6574 2064 6976 203d 2064 6f63     let div = doc
-00007830: 756d 656e 742e 6372 6561 7465 456c 656d  ument.createElem
-00007840: 656e 7428 2264 6976 2229 3b0a 2020 2020  ent("div");.    
+00007770: 2020 2020 2020 7d20 656c 7365 7b0a 2020        } else{.  
+00007780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077a0: 2020 2020 2020 2020 2020 2020 2020 6469                di
+000077b0: 762e 636c 6173 734c 6973 742e 6164 6428  v.classList.add(
+000077c0: 2767 7269 642d 726f 7727 2c27 6772 6964  'grid-row','grid
+000077d0: 2d73 7464 2d63 656c 6c73 247b 7569 647d  -std-cells${uid}
+000077e0: 2729 3b0a 2020 2020 2020 2020 2020 2020  ');.            
+000077f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007810: 2020 2020 6966 2028 6974 656d 5b61 7474      if (item[att
+00007820: 725d 203d 3d20 6e75 6c6c 2920 7b0a 2020  r] == null) {.  
+00007830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007840: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007860: 2020 2020 2020 2020 2020 2020 2020 6469                di
-00007870: 762e 636c 6173 734c 6973 742e 6164 6428  v.classList.add(
-00007880: 2770 6167 6527 293b 0a20 2020 2020 2020  'page');.       
-00007890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078a0: 2020 2020 2020 2020 2020 2069 6628 693d             if(i=
-000078b0: 3d3d 3029 2064 6976 2e73 7479 6c65 2e63  ==0) div.style.c
-000078c0: 6f6c 6f72 203d 2022 6772 6179 223b 0a20  olor = "gray";. 
-000078d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078f0: 2065 6c73 6520 6469 762e 7374 796c 652e   else div.style.
-00007900: 636f 6c6f 7220 3d20 2776 6172 282d 2d74  color = 'var(--t
-00007910: 6572 7469 6172 792d 636f 6c6f 722c 2022  ertiary-color, "
-00007920: 6772 6179 2229 273b 0a20 2020 2020 2020  gray")';.       
+00007860: 2020 7465 7874 203d 2027 2027 0a20 2020    text = ' '.   
+00007870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007890: 2020 2020 2020 2020 2020 2020 207d 2065               } e
+000078a0: 6c73 6520 7b0a 2020 2020 2020 2020 2020  lse {.          
+000078b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078d0: 2020 2020 2020 2020 2020 7465 7874 203d            text =
+000078e0: 2053 7472 696e 6728 6974 656d 5b61 7474   String(item[att
+000078f0: 725d 290a 2020 2020 2020 2020 2020 2020  r]).            
+00007900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007920: 2020 2020 7d0a 0a20 2020 2020 2020 2020      }..         
 00007930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007940: 2020 2020 2020 2020 2020 2064 6976 2e6f             div.o
-00007950: 6e63 6c69 636b 203d 2066 756e 6374 696f  nclick = functio
-00007960: 6e28 6576 656e 7429 207b 0a20 2020 2020  n(event) {.     
-00007970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007950: 2020 2020 2020 2074 6578 7420 3d20 7465         text = te
+00007960: 7874 2e72 6570 6c61 6365 416c 6c28 225c  xt.replaceAll("\
+00007970: 5c6e 222c 2022 3c2f 6272 3e22 293b 0a20  \n", "</br>");. 
 00007980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007990: 206c 6574 2069 6e64 6578 6573 203d 2064   let indexes = d
-000079a0: 6f63 756d 656e 742e 6765 7445 6c65 6d65  ocument.getEleme
-000079b0: 6e74 7342 7943 6c61 7373 4e61 6d65 2827  ntsByClassName('
-000079c0: 7061 6765 2729 3b0a 2020 2020 2020 2020  page');.        
+00007990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000079a0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000079b0: 6976 2e69 6e6e 6572 4854 4d4c 203d 2074  iv.innerHTML = t
+000079c0: 6578 743b 0a20 2020 2020 2020 2020 2020  ext;.           
 000079d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079e0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-000079f0: 7220 286c 6574 2069 6e64 6578 206f 6620  r (let index of 
-00007a00: 696e 6465 7865 7329 207b 2069 6e64 6578  indexes) { index
-00007a10: 2e73 7479 6c65 2e63 6f6c 6f72 203d 2027  .style.color = '
-00007a20: 7661 7228 2d2d 7465 7274 6961 7279 2d63  var(--tertiary-c
-00007a30: 6f6c 6f72 2c20 2267 7261 7922 2927 207d  olor, "gray")' }
-00007a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a60: 2020 2020 2020 2065 7665 6e74 2e74 6172         event.tar
-00007a70: 6765 742e 7374 796c 652e 636f 6c6f 7220  get.style.color 
-00007a80: 3d20 2267 7261 7922 3b0a 2020 2020 2020  = "gray";.      
-00007a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ab0: 7365 7450 6167 6524 7b75 6964 7d28 6920  setPage${uid}(i 
-00007ac0: 2b20 3129 3b0a 2020 2020 2020 2020 2020  + 1);.          
-00007ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ae0: 2020 2020 2020 2020 7d3b 0a20 2020 2020          };.     
-00007af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b00: 2020 2020 2020 2020 2020 2020 2064 6976               div
-00007b10: 2e69 6e6e 6572 5465 7874 203d 2069 202b  .innerText = i +
-00007b20: 2031 3b0a 2020 2020 2020 2020 2020 2020   1;.            
-00007b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b40: 2020 2020 2020 7061 6765 436f 6e74 6169        pageContai
-00007b50: 6e65 722e 6170 7065 6e64 4368 696c 6428  ner.appendChild(
-00007b60: 6469 7629 3b0a 2020 2020 2020 2020 2020  div);.          
-00007b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b80: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00007b90: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
-00007ba0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00007bb0: 756e 6374 696f 6e20 7365 7450 6167 6524  unction setPage$
-00007bc0: 7b75 6964 7d28 6e65 7750 6167 6529 7b0a  {uid}(newPage){.
-00007bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007be0: 2020 2020 2020 2020 7061 6765 496e 6465          pageInde
-00007bf0: 7820 3d20 6e65 7750 6167 650a 2020 2020  x = newPage.    
-00007c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c10: 2020 2020 7265 7365 7442 7949 6424 7b75      resetById${u
-00007c20: 6964 7d28 2774 6162 6c65 247b 7569 647d  id}('table${uid}
-00007c30: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
-00007c40: 2020 2020 2020 2020 2020 2062 7569 6c64             build
-00007c50: 4772 6964 247b 7569 647d 2870 6167 696e  Grid${uid}(pagin
-00007c60: 6174 6564 456c 656d 656e 7473 247b 7569  atedElements${ui
-00007c70: 647d 2c20 7061 6765 496e 6465 7829 0a20  d}, pageIndex). 
-00007c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c90: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
-00007ca0: 2020 2020 2020 2020 2028 6173 796e 6320           (async 
-00007cb0: 6675 6e63 7469 6f6e 2829 207b 0a20 2020  function() {.   
-00007cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cd0: 2020 2020 2063 6f6e 7374 206d 7946 6f6e       const myFon
-00007ce0: 7420 3d20 6e65 7720 466f 6e74 4661 6365  t = new FontFace
-00007cf0: 2827 4465 6a61 5675 2053 616e 7327 2c20  ('DejaVu Sans', 
-00007d00: 2775 726c 2868 7474 7073 3a2f 2f63 646e  'url(https://cdn
-00007d10: 2e6a 7364 656c 6976 722e 6e65 742f 6e70  .jsdelivr.net/np
-00007d20: 6d2f 6465 6a61 7675 2d73 616e 7340 312e  m/dejavu-sans@1.
-00007d30: 302e 302f 6373 732f 6465 6a61 7675 2d73  0.0/css/dejavu-s
-00007d40: 616e 732e 6d69 6e2e 6373 7329 2729 3b0a  ans.min.css)');.
-00007d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d60: 2020 2020 2020 2020 6177 6169 7420 6d79          await my
-00007d70: 466f 6e74 2e6c 6f61 6428 293b 0a20 2020  Font.load();.   
-00007d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d90: 2020 2020 2064 6f63 756d 656e 742e 666f       document.fo
-00007da0: 6e74 732e 6164 6428 6d79 466f 6e74 293b  nts.add(myFont);
-00007db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007dc0: 2020 2020 2020 2020 2064 6f63 756d 656e           documen
-00007dd0: 742e 6765 7445 6c65 6d65 6e74 7342 7954  t.getElementsByT
-00007de0: 6167 4e61 6d65 2827 6831 2729 5b30 5d2e  agName('h1')[0].
-00007df0: 7374 796c 652e 666f 6e74 4661 6d69 6c79  style.fontFamily
-00007e00: 203d 2022 4465 6a61 5675 2053 616e 7322   = "DejaVu Sans"
-00007e10: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-00007e20: 2020 2020 2020 7d29 2829 3b0a 0a20 2020        })();..   
-00007e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e40: 2062 7569 6c64 5061 6769 6e61 7469 6f6e   buildPagination
-00007e50: 436f 6e74 6169 6e65 7224 7b75 6964 7d28  Container${uid}(
-00007e60: 7061 6769 6e61 7465 6445 6c65 6d65 6e74  paginatedElement
-00007e70: 7324 7b75 6964 7d29 0a20 2020 2020 2020  s${uid}).       
-00007e80: 2020 2020 2020 2020 203c 2f73 6372 6970           </scrip
-00007e90: 743e 0a20 2020 2020 2020 2020 2020 203c  t>.            <
-00007ea0: 2f64 6976 3e0a 2020 2020 2020 2020 3c2f  /div>.        </
-00007eb0: 6469 763e 0a22 2222 0a0a 0a64 6566 2063  div>."""...def c
-00007ec0: 7265 6174 655f 7461 626c 655f 7465 6d70  reate_table_temp
-00007ed0: 6c61 7465 280a 2020 2020 6974 656d 733a  late(.    items:
-00007ee0: 2053 6571 7565 6e63 652c 206c 6973 745f   Sequence, list_
-00007ef0: 6e61 6d65 3a20 416e 792c 2072 6f77 733a  name: Any, rows:
-00007f00: 2069 6e74 203d 2035 2c20 7461 626c 655f   int = 5, table_
-00007f10: 6963 6f6e 3a20 416e 7920 3d20 4e6f 6e65  icon: Any = None
-00007f20: 0a29 202d 3e20 7374 723a 0a20 2020 2069  .) -> str:.    i
-00007f30: 6620 6e6f 7420 7461 626c 655f 6963 6f6e  f not table_icon
-00007f40: 3a0a 2020 2020 2020 2020 7461 626c 655f  :.        table_
-00007f50: 6963 6f6e 203d 2054 4142 4c45 5f49 434f  icon = TABLE_ICO
-00007f60: 4e0a 0a20 2020 2069 7465 6d73 5f64 6963  N..    items_dic
-00007f70: 7420 3d20 6a73 6f6e 2e64 756d 7073 2869  t = json.dumps(i
-00007f80: 7465 6d73 290a 2020 2020 636f 6465 203d  tems).    code =
-00007f90: 2043 5353 5f43 4f44 4520 2b20 6375 7374   CSS_CODE + cust
-00007fa0: 6f6d 5f63 6f64 650a 2020 2020 7465 6d70  om_code.    temp
-00007fb0: 6c61 7465 203d 2054 656d 706c 6174 6528  late = Template(
-00007fc0: 636f 6465 290a 2020 2020 726f 7773 203d  code).    rows =
-00007fd0: 206d 696e 286c 656e 2869 7465 6d73 292c   min(len(items),
-00007fe0: 2072 6f77 7329 0a20 2020 2069 6620 6c65   rows).    if le
-00007ff0: 6e28 6974 656d 7329 203d 3d20 303a 0a20  n(items) == 0:. 
-00008000: 2020 2020 2020 2063 6f6c 7320 3d20 300a         cols = 0.
-00008010: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00008020: 2020 636f 6c73 203d 2028 6c65 6e28 6974    cols = (len(it
-00008030: 656d 735b 305d 2e6b 6579 7328 2929 2920  ems[0].keys())) 
-00008040: 2a20 340a 2020 2020 7265 7475 726e 2074  * 4.    return t
-00008050: 656d 706c 6174 652e 7375 6273 7469 7475  emplate.substitu
-00008060: 7465 280a 2020 2020 2020 2020 7569 643d  te(.        uid=
-00008070: 7374 7228 5549 4428 2929 2c0a 2020 2020  str(UID()),.    
-00008080: 2020 2020 656c 656d 656e 743d 6974 656d      element=item
-00008090: 735f 6469 6374 2c0a 2020 2020 2020 2020  s_dict,.        
-000080a0: 6c69 7374 5f6e 616d 653d 6c69 7374 5f6e  list_name=list_n
-000080b0: 616d 652c 0a20 2020 2020 2020 2063 6f6c  ame,.        col
-000080c0: 733d 636f 6c73 2c0a 2020 2020 2020 2020  s=cols,.        
-000080d0: 726f 7773 3d72 6f77 732c 0a20 2020 2020  rows=rows,.     
-000080e0: 2020 2069 636f 6e3d 7461 626c 655f 6963     icon=table_ic
-000080f0: 6f6e 2c0a 2020 2020 2020 2020 7365 6172  on,.        sear
-00008100: 6368 4963 6f6e 3d53 4541 5243 485f 4943  chIcon=SEARCH_IC
-00008110: 4f4e 2c0a 2020 2020 2020 2020 636c 6970  ON,.        clip
-00008120: 626f 6172 6449 636f 6e3d 434c 4950 424f  boardIcon=CLIPBO
-00008130: 4152 445f 4943 4f4e 2c0a 2020 2020 290a  ARD_ICON,.    ).
+000079e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000079f0: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
+00007a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a10: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+00007a20: 7269 642e 6170 7065 6e64 4368 696c 6428  rid.appendChild(
+00007a30: 6469 7629 3b0a 2020 2020 2020 2020 2020  div);.          
+00007a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a50: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00007a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a80: 2020 2020 7461 626c 655f 696e 6465 7824      table_index$
+00007a90: 7b75 6964 7d20 3d20 7461 626c 655f 696e  {uid} = table_in
+00007aa0: 6465 7824 7b75 6964 7d20 2b20 313b 0a20  dex${uid} + 1;. 
+00007ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ad0: 2020 207d 290a 2020 2020 2020 2020 2020     }).          
+00007ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007af0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00007b00: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00007b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b20: 2020 7061 6769 6e61 7465 6445 6c65 6d65    paginatedEleme
+00007b30: 6e74 7324 7b75 6964 7d20 3d20 7061 6769  nts${uid} = pagi
+00007b40: 6e61 7465 247b 7569 647d 2865 6c65 6d65  nate${uid}(eleme
+00007b50: 6e74 247b 7569 647d 2c20 7061 6765 5f73  nt${uid}, page_s
+00007b60: 697a 6524 7b75 6964 7d29 0a20 2020 2020  ize${uid}).     
+00007b70: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00007b80: 7569 6c64 4772 6964 247b 7569 647d 2870  uildGrid${uid}(p
+00007b90: 6167 696e 6174 6564 456c 656d 656e 7473  aginatedElements
+00007ba0: 247b 7569 647d 2c20 3129 0a20 2020 2020  ${uid}, 1).     
+00007bb0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00007bc0: 6f63 756d 656e 742e 6765 7445 6c65 6d65  ocument.getEleme
+00007bd0: 6e74 4279 4964 2827 746f 7461 6c24 7b75  ntById('total${u
+00007be0: 6964 7d27 292e 696e 6e65 7254 6578 7420  id}').innerText 
+00007bf0: 3d20 2254 6f74 616c 3a20 2220 2b20 656c  = "Total: " + el
+00007c00: 656d 656e 7424 7b75 6964 7d2e 6c65 6e67  ement${uid}.leng
+00007c10: 7468 0a20 2020 2020 2020 2020 2020 2020  th.             
+00007c20: 2020 203c 2f73 6372 6970 743e 0a20 2020     </script>.   
+00007c30: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00007c40: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00007c50: 2069 643d 2770 6167 247b 7569 647d 2720   id='pag${uid}' 
+00007c60: 636c 6173 733d 2770 6167 696e 6174 696f  class='paginatio
+00007c70: 6e43 6f6e 7461 696e 6572 273e 0a20 2020  nContainer'>.   
+00007c80: 2020 2020 2020 2020 2020 2020 203c 7363               <sc
+00007c90: 7269 7074 3e0a 2020 2020 2020 2020 2020  ript>.          
+00007ca0: 2020 2020 2020 2020 2020 6675 6e63 7469            functi
+00007cb0: 6f6e 2062 7569 6c64 5061 6769 6e61 7469  on buildPaginati
+00007cc0: 6f6e 436f 6e74 6169 6e65 7224 7b75 6964  onContainer${uid
+00007cd0: 7d28 7061 6769 6e61 7465 6445 6c65 6d65  }(paginatedEleme
+00007ce0: 6e74 7329 7b0a 2020 2020 2020 2020 2020  nts){.          
+00007cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d00: 2020 6c65 7420 7061 6765 436f 6e74 6169    let pageContai
+00007d10: 6e65 7220 3d20 646f 6375 6d65 6e74 2e67  ner = document.g
+00007d20: 6574 456c 656d 656e 7442 7949 6428 2270  etElementById("p
+00007d30: 6167 247b 7569 647d 2229 3b0a 2020 2020  ag${uid}");.    
+00007d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d50: 2020 2020 2020 2020 666f 7220 286c 6574          for (let
+00007d60: 2069 203d 2030 3b20 6920 3c20 7061 6769   i = 0; i < pagi
+00007d70: 6e61 7465 6445 6c65 6d65 6e74 732e 6c65  natedElements.le
+00007d80: 6e67 7468 3b20 692b 2b29 207b 0a20 2020  ngth; i++) {.   
+00007d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007da0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00007db0: 6574 2064 6976 203d 2064 6f63 756d 656e  et div = documen
+00007dc0: 742e 6372 6561 7465 456c 656d 656e 7428  t.createElement(
+00007dd0: 2264 6976 2229 3b0a 2020 2020 2020 2020  "div");.        
+00007de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007df0: 2020 2020 2020 2020 2020 6469 762e 636c            div.cl
+00007e00: 6173 734c 6973 742e 6164 6428 2770 6167  assList.add('pag
+00007e10: 6527 293b 0a20 2020 2020 2020 2020 2020  e');.           
+00007e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e30: 2020 2020 2020 2069 6628 693d 3d3d 3029         if(i===0)
+00007e40: 2064 6976 2e73 7479 6c65 2e63 6f6c 6f72   div.style.color
+00007e50: 203d 2022 6772 6179 223b 0a20 2020 2020   = "gray";.     
+00007e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e70: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00007e80: 6520 6469 762e 7374 796c 652e 636f 6c6f  e div.style.colo
+00007e90: 7220 3d20 2776 6172 282d 2d74 6572 7469  r = 'var(--terti
+00007ea0: 6172 792d 636f 6c6f 722c 2022 6772 6179  ary-color, "gray
+00007eb0: 2229 273b 0a20 2020 2020 2020 2020 2020  ")';.           
+00007ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ed0: 2020 2020 2020 2064 6976 2e6f 6e63 6c69         div.oncli
+00007ee0: 636b 203d 2066 756e 6374 696f 6e28 6576  ck = function(ev
+00007ef0: 656e 7429 207b 0a20 2020 2020 2020 2020  ent) {.         
+00007f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f10: 2020 2020 2020 2020 2020 2020 206c 6574               let
+00007f20: 2069 6e64 6578 6573 203d 2064 6f63 756d   indexes = docum
+00007f30: 656e 742e 6765 7445 6c65 6d65 6e74 7342  ent.getElementsB
+00007f40: 7943 6c61 7373 4e61 6d65 2827 7061 6765  yClassName('page
+00007f50: 2729 3b0a 2020 2020 2020 2020 2020 2020  ');.            
+00007f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f70: 2020 2020 2020 2020 2020 666f 7220 286c            for (l
+00007f80: 6574 2069 6e64 6578 206f 6620 696e 6465  et index of inde
+00007f90: 7865 7329 207b 2069 6e64 6578 2e73 7479  xes) { index.sty
+00007fa0: 6c65 2e63 6f6c 6f72 203d 2027 7661 7228  le.color = 'var(
+00007fb0: 2d2d 7465 7274 6961 7279 2d63 6f6c 6f72  --tertiary-color
+00007fc0: 2c20 2267 7261 7922 2927 207d 0a20 2020  , "gray")' }.   
+00007fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ff0: 2020 2065 7665 6e74 2e74 6172 6765 742e     event.target.
+00008000: 7374 796c 652e 636f 6c6f 7220 3d20 2267  style.color = "g
+00008010: 7261 7922 3b0a 2020 2020 2020 2020 2020  ray";.          
+00008020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008030: 2020 2020 2020 2020 2020 2020 7365 7450              setP
+00008040: 6167 6524 7b75 6964 7d28 6920 2b20 3129  age${uid}(i + 1)
+00008050: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+00008060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008070: 2020 2020 7d3b 0a20 2020 2020 2020 2020      };.         
+00008080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008090: 2020 2020 2020 2020 2064 6976 2e69 6e6e           div.inn
+000080a0: 6572 5465 7874 203d 2069 202b 2031 3b0a  erText = i + 1;.
+000080b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080d0: 2020 7061 6765 436f 6e74 6169 6e65 722e    pageContainer.
+000080e0: 6170 7065 6e64 4368 696c 6428 6469 7629  appendChild(div)
+000080f0: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+00008100: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00008110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008120: 2020 2020 7d0a 0a20 2020 2020 2020 2020      }..         
+00008130: 2020 2020 2020 2020 2020 2066 756e 6374             funct
+00008140: 696f 6e20 7365 7450 6167 6524 7b75 6964  ion setPage${uid
+00008150: 7d28 6e65 7750 6167 6529 7b0a 2020 2020  }(newPage){.    
+00008160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008170: 2020 2020 7061 6765 496e 6465 7820 3d20      pageIndex = 
+00008180: 6e65 7750 6167 650a 2020 2020 2020 2020  newPage.        
+00008190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081a0: 7265 7365 7442 7949 6424 7b75 6964 7d28  resetById${uid}(
+000081b0: 2774 6162 6c65 247b 7569 647d 2729 0a20  'table${uid}'). 
+000081c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081d0: 2020 2020 2020 2062 7569 6c64 4772 6964         buildGrid
+000081e0: 247b 7569 647d 2870 6167 696e 6174 6564  ${uid}(paginated
+000081f0: 456c 656d 656e 7473 247b 7569 647d 2c20  Elements${uid}, 
+00008200: 7061 6765 496e 6465 7829 0a20 2020 2020  pageIndex).     
+00008210: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00008220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008230: 2020 2020 2028 6173 796e 6320 6675 6e63       (async func
+00008240: 7469 6f6e 2829 207b 0a20 2020 2020 2020  tion() {.       
+00008250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008260: 2063 6f6e 7374 206d 7946 6f6e 7420 3d20   const myFont = 
+00008270: 6e65 7720 466f 6e74 4661 6365 2827 4465  new FontFace('De
+00008280: 6a61 5675 2053 616e 7327 2c20 2775 726c  jaVu Sans', 'url
+00008290: 2868 7474 7073 3a2f 2f63 646e 2e6a 7364  (https://cdn.jsd
+000082a0: 656c 6976 722e 6e65 742f 6e70 6d2f 6465  elivr.net/npm/de
+000082b0: 6a61 7675 2d73 616e 7340 312e 302e 302f  javu-sans@1.0.0/
+000082c0: 666f 6e74 732f 6465 6a61 7675 2d73 616e  fonts/dejavu-san
+000082d0: 732d 7765 6266 6f6e 742e 776f 6666 323f  s-webfont.woff2?
+000082e0: 6469 7370 6c61 793d 7377 6170 2729 3b0a  display=swap');.
+000082f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008300: 2020 2020 2020 2020 6177 6169 7420 6d79          await my
+00008310: 466f 6e74 2e6c 6f61 6428 293b 0a20 2020  Font.load();.   
+00008320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008330: 2020 2020 2064 6f63 756d 656e 742e 666f       document.fo
+00008340: 6e74 732e 6164 6428 6d79 466f 6e74 293b  nts.add(myFont);
+00008350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008360: 2020 2020 207d 2928 293b 0a0a 2020 2020       })();..    
+00008370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008380: 6275 696c 6450 6167 696e 6174 696f 6e43  buildPaginationC
+00008390: 6f6e 7461 696e 6572 247b 7569 647d 2870  ontainer${uid}(p
+000083a0: 6167 696e 6174 6564 456c 656d 656e 7473  aginatedElements
+000083b0: 247b 7569 647d 290a 2020 2020 2020 2020  ${uid}).        
+000083c0: 2020 2020 2020 2020 3c2f 7363 7269 7074          </script
+000083d0: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
+000083e0: 6469 763e 0a20 2020 2020 2020 203c 2f64  div>.        </d
+000083f0: 6976 3e0a 2222 220a 0a0a 6465 6620 6372  iv>."""...def cr
+00008400: 6561 7465 5f74 6162 6c65 5f74 656d 706c  eate_table_templ
+00008410: 6174 6528 0a20 2020 2069 7465 6d73 3a20  ate(.    items: 
+00008420: 5365 7175 656e 6365 2c0a 2020 2020 6c69  Sequence,.    li
+00008430: 7374 5f6e 616d 653a 2073 7472 2c0a 2020  st_name: str,.  
+00008440: 2020 726f 7773 3a20 696e 7420 3d20 352c    rows: int = 5,
+00008450: 0a20 2020 2074 6162 6c65 5f69 636f 6e3a  .    table_icon:
+00008460: 2073 7472 207c 204e 6f6e 6520 3d20 4e6f   str | None = No
+00008470: 6e65 2c0a 2020 2020 6772 6964 5f74 656d  ne,.    grid_tem
+00008480: 706c 6174 655f 636f 6c75 6d6e 733a 2073  plate_columns: s
+00008490: 7472 207c 204e 6f6e 6520 3d20 4e6f 6e65  tr | None = None
+000084a0: 2c0a 2020 2020 6772 6964 5f74 656d 706c  ,.    grid_templ
+000084b0: 6174 655f 6365 6c6c 5f63 6f6c 756d 6e73  ate_cell_columns
+000084c0: 3a20 7374 7220 7c20 4e6f 6e65 203d 204e  : str | None = N
+000084d0: 6f6e 652c 0a29 202d 3e20 7374 723a 0a20  one,.) -> str:. 
+000084e0: 2020 2069 6620 7461 626c 655f 6963 6f6e     if table_icon
+000084f0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00008500: 2020 7461 626c 655f 6963 6f6e 203d 2054    table_icon = T
+00008510: 4142 4c45 5f49 434f 4e0a 2020 2020 6966  ABLE_ICON.    if
+00008520: 2067 7269 645f 7465 6d70 6c61 7465 5f63   grid_template_c
+00008530: 6f6c 756d 6e73 2069 7320 4e6f 6e65 3a0a  olumns is None:.
+00008540: 2020 2020 2020 2020 6772 6964 5f74 656d          grid_tem
+00008550: 706c 6174 655f 636f 6c75 6d6e 7320 3d20  plate_columns = 
+00008560: 2231 6672 2072 6570 6561 7428 7b63 6f6c  "1fr repeat({col
+00008570: 737d 2c20 3166 7229 220a 2020 2020 6966  s}, 1fr)".    if
+00008580: 2067 7269 645f 7465 6d70 6c61 7465 5f63   grid_template_c
+00008590: 656c 6c5f 636f 6c75 6d6e 7320 6973 204e  ell_columns is N
+000085a0: 6f6e 653a 0a20 2020 2020 2020 2067 7269  one:.        gri
+000085b0: 645f 7465 6d70 6c61 7465 5f63 656c 6c5f  d_template_cell_
+000085c0: 636f 6c75 6d6e 7320 3d20 2273 7061 6e20  columns = "span 
+000085d0: 3422 0a0a 2020 2020 6974 656d 735f 6469  4"..    items_di
+000085e0: 6374 203d 206a 736f 6e2e 6475 6d70 7328  ct = json.dumps(
+000085f0: 6974 656d 7329 0a20 2020 2063 6f64 6520  items).    code 
+00008600: 3d20 4353 535f 434f 4445 202b 2063 7573  = CSS_CODE + cus
+00008610: 746f 6d5f 636f 6465 0a20 2020 2074 656d  tom_code.    tem
+00008620: 706c 6174 6520 3d20 5465 6d70 6c61 7465  plate = Template
+00008630: 2863 6f64 6529 0a20 2020 2072 6f77 7320  (code).    rows 
+00008640: 3d20 6d69 6e28 6c65 6e28 6974 656d 7329  = min(len(items)
+00008650: 2c20 726f 7773 290a 2020 2020 6966 206c  , rows).    if l
+00008660: 656e 2869 7465 6d73 2920 3d3d 2030 3a0a  en(items) == 0:.
+00008670: 2020 2020 2020 2020 636f 6c73 203d 2030          cols = 0
+00008680: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00008690: 2020 2063 6f6c 7320 3d20 286c 656e 2869     cols = (len(i
+000086a0: 7465 6d73 5b30 5d2e 6b65 7973 2829 2929  tems[0].keys()))
+000086b0: 202a 2034 0a20 2020 2069 6620 227b 636f   * 4.    if "{co
+000086c0: 6c73 7d22 2069 6e20 6772 6964 5f74 656d  ls}" in grid_tem
+000086d0: 706c 6174 655f 636f 6c75 6d6e 733a 0a20  plate_columns:. 
+000086e0: 2020 2020 2020 2067 7269 645f 7465 6d70         grid_temp
+000086f0: 6c61 7465 5f63 6f6c 756d 6e73 203d 2067  late_columns = g
+00008700: 7269 645f 7465 6d70 6c61 7465 5f63 6f6c  rid_template_col
+00008710: 756d 6e73 2e66 6f72 6d61 7428 636f 6c73  umns.format(cols
+00008720: 3d63 6f6c 7329 0a20 2020 2066 696e 616c  =cols).    final
+00008730: 5f68 746d 6c20 3d20 7465 6d70 6c61 7465  _html = template
+00008740: 2e73 7562 7374 6974 7574 6528 0a20 2020  .substitute(.   
+00008750: 2020 2020 2075 6964 3d73 7472 2855 4944       uid=str(UID
+00008760: 2829 292c 0a20 2020 2020 2020 2065 6c65  ()),.        ele
+00008770: 6d65 6e74 3d69 7465 6d73 5f64 6963 742c  ment=items_dict,
+00008780: 0a20 2020 2020 2020 206c 6973 745f 6e61  .        list_na
+00008790: 6d65 3d6c 6973 745f 6e61 6d65 2c0a 2020  me=list_name,.  
+000087a0: 2020 2020 2020 636f 6c73 3d63 6f6c 732c        cols=cols,
+000087b0: 0a20 2020 2020 2020 2072 6f77 733d 726f  .        rows=ro
+000087c0: 7773 2c0a 2020 2020 2020 2020 6963 6f6e  ws,.        icon
+000087d0: 3d74 6162 6c65 5f69 636f 6e2c 0a20 2020  =table_icon,.   
+000087e0: 2020 2020 2073 6561 7263 6849 636f 6e3d       searchIcon=
+000087f0: 5345 4152 4348 5f49 434f 4e2c 0a20 2020  SEARCH_ICON,.   
+00008800: 2020 2020 2063 6c69 7062 6f61 7264 4963       clipboardIc
+00008810: 6f6e 3d43 4c49 5042 4f41 5244 5f49 434f  on=CLIPBOARD_ICO
+00008820: 4e2c 0a20 2020 2020 2020 2067 7269 645f  N,.        grid_
+00008830: 7465 6d70 6c61 7465 5f63 6f6c 756d 6e73  template_columns
+00008840: 3d67 7269 645f 7465 6d70 6c61 7465 5f63  =grid_template_c
+00008850: 6f6c 756d 6e73 2c0a 2020 2020 2020 2020  olumns,.        
+00008860: 6772 6964 5f74 656d 706c 6174 655f 6365  grid_template_ce
+00008870: 6c6c 5f63 6f6c 756d 6e73 3d67 7269 645f  ll_columns=grid_
+00008880: 7465 6d70 6c61 7465 5f63 656c 6c5f 636f  template_cell_co
+00008890: 6c75 6d6e 732c 0a20 2020 2029 0a20 2020  lumns,.    ).   
+000088a0: 2072 6574 7572 6e20 6669 6e61 6c5f 6874   return final_ht
+000088b0: 6d6c 0a                                  ml.
```

### Comparing `syft-0.8.7b2/src/syft/util/schema.py` & `syft-0.8.7b3/src/syft/util/schema.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/util/telemetry.py` & `syft-0.8.7b3/src/syft/util/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/util/trace_decorator.py` & `syft-0.8.7b3/src/syft/util/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/util/util.py` & `syft-0.8.7b3/src/syft/util/util.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft/util/version_compare.py` & `syft-0.8.7b3/src/syft/util/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b2/src/syft.egg-info/PKG-INFO` & `syft-0.8.7b3/src/syft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.7b2
+Version: 0.8.7b3
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

### Comparing `syft-0.8.7b2/src/syft.egg-info/SOURCES.txt` & `syft-0.8.7b3/src/syft.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -128,24 +128,26 @@
 src/syft/service/data_subject/data_subject_service.py
 src/syft/service/dataset/__init__.py
 src/syft/service/dataset/dataset.py
 src/syft/service/dataset/dataset_service.py
 src/syft/service/dataset/dataset_stash.py
 src/syft/service/enclave/enclave_service.py
 src/syft/service/job/__init__.py
+src/syft/service/job/html_template.py
 src/syft/service/job/job_service.py
 src/syft/service/job/job_stash.py
 src/syft/service/log/__init__.py
 src/syft/service/log/log.py
 src/syft/service/log/log_service.py
 src/syft/service/log/log_stash.py
 src/syft/service/metadata/__init__.py
 src/syft/service/metadata/metadata_service.py
 src/syft/service/metadata/migrations.py
 src/syft/service/metadata/node_metadata.py
+src/syft/service/network/association_request.py
 src/syft/service/network/network_service.py
 src/syft/service/network/node_peer.py
 src/syft/service/network/routes.py
 src/syft/service/notification/__init__.py
 src/syft/service/notification/email_templates.py
 src/syft/service/notification/notification_service.py
 src/syft/service/notification/notification_stash.py
```

### Comparing `syft-0.8.7b2/src/syft.egg-info/requires.txt` & `syft-0.8.7b3/src/syft.egg-info/requires.txt`

 * *Files identical despite different names*

