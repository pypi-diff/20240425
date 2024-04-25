# Comparing `tmp/runtimepy-4.2.2.tar.gz` & `tmp/runtimepy-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtimepy-4.2.2.tar", last modified: Wed Apr 24 07:08:29 2024, max compression
+gzip compressed data, was "runtimepy-4.3.0.tar", last modified: Thu Apr 25 08:47:33 2024, max compression
```

## Comparing `runtimepy-4.2.2.tar` & `runtimepy-4.3.0.tar`

### file list

```diff
@@ -1,305 +1,305 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.020887 runtimepy-4.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 07:05:55.000000 runtimepy-4.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-24 07:08:29.020887 runtimepy-4.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-24 07:05:55.000000 runtimepy-4.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-24 07:05:55.000000 runtimepy-4.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:28.980887 runtimepy-4.2.2/runtimepy/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:28.984887 runtimepy-4.2.2/runtimepy/channel/
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:28.984887 runtimepy-4.2.2/runtimepy/channel/environment/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/channel/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/channel/environment/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/channel/environment/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:28.984887 runtimepy-4.2.2/runtimepy/channel/environment/command/
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/channel/environment/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/channel/environment/command/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/channel/environment/command/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/channel/environment/command/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/channel/environment/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/channel/environment/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/channel/environment/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/channel/environment/telemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:28.984887 runtimepy-4.2.2/runtimepy/channel/event/
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/channel/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/channel/event/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/channel/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:28.984887 runtimepy-4.2.2/runtimepy/codec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/codec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:28.984887 runtimepy-4.2.2/runtimepy/codec/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/codec/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/codec/protocol/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/codec/protocol/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:28.984887 runtimepy-4.2.2/runtimepy/codec/system/
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/codec/system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:28.988887 runtimepy-4.2.2/runtimepy/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/commands/arbiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/commands/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/commands/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/commands/tui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:28.988887 runtimepy-4.2.2/runtimepy/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:28.988887 runtimepy-4.2.2/runtimepy/data/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/css/bootstrap_extra.css
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/css/main.css
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/dummy_load.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/factories.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   362870 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:28.988887 runtimepy-4.2.2/runtimepy/data/js/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/js/DataConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/js/JsonConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/js/audio.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:28.992887 runtimepy-4.2.2/runtimepy/data/js/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/js/classes/App.js
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/js/classes/ChannelTable.js
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/js/classes/DataConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/js/classes/JsonConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/js/classes/Plot.js
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/js/classes/PlotManager.js
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/js/classes/PlotModalManager.js
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/js/classes/TabFilter.js
--rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/js/classes/TabInterface.js
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/js/classes/WindowHashManager.js
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/js/classes/WorkerInterface.js
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/js/init.js
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/js/main.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:28.992887 runtimepy-4.2.2/runtimepy/data/js/tab/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/js/tab/env.js
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/js/tab/sound.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:28.992887 runtimepy-4.2.2/runtimepy/data/js/unused/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/js/unused/pyodide.js
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/js/util.js
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/js/worker.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:28.996887 runtimepy-4.2.2/runtimepy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/schemas/BitFields.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/schemas/Channel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/schemas/ChannelCommand.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/schemas/ChannelRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/schemas/ClientConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/schemas/EnumRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/schemas/FindFile.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/schemas/PeerProcessConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/schemas/RuntimeEnum.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/schemas/ServerConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/schemas/StructConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/schemas/TaskConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/schemas/has_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/schemas/has_factory.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/schemas/has_name.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/schemas/has_request_flag.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/server.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/server_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/data/server_dev.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:28.996887 runtimepy-4.2.2/runtimepy/enum/
--rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/enum/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/enum/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:28.996887 runtimepy-4.2.2/runtimepy/message/
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/message/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10939 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/message/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/message/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:28.996887 runtimepy-4.2.2/runtimepy/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/metrics/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/metrics/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/metrics/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:28.996887 runtimepy-4.2.2/runtimepy/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/mixins/async_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/mixins/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/mixins/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/mixins/finalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/mixins/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/mixins/psutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/mixins/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.000887 runtimepy-4.2.2/runtimepy/net/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.000887 runtimepy-4.2.2/runtimepy/net/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.000887 runtimepy-4.2.2/runtimepy/net/arbiter/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14523 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/arbiter/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.000887 runtimepy-4.2.2/runtimepy/net/arbiter/config/
--rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/arbiter/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/arbiter/config/codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/arbiter/config/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.000887 runtimepy-4.2.2/runtimepy/net/arbiter/factory/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/arbiter/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/arbiter/factory/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/arbiter/factory/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.000887 runtimepy-4.2.2/runtimepy/net/arbiter/housekeeping/
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/arbiter/housekeeping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.000887 runtimepy-4.2.2/runtimepy/net/arbiter/imports/
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/arbiter/imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/arbiter/imports/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/arbiter/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/arbiter/result.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/arbiter/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.000887 runtimepy-4.2.2/runtimepy/net/arbiter/tcp/
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/arbiter/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/arbiter/tcp/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/arbiter/udp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/arbiter/websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)    11894 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.000887 runtimepy-4.2.2/runtimepy/net/factories/
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/factories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.004887 runtimepy-4.2.2/runtimepy/net/http/
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/http/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/http/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/http/request_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/http/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/http/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/http/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.004887 runtimepy-4.2.2/runtimepy/net/server/
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.004887 runtimepy-4.2.2/runtimepy/net/server/app/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/app/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.004887 runtimepy-4.2.2/runtimepy/net/server/app/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/app/bootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/app/bootstrap/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/app/bootstrap/tabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/app/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/app/elements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.008887 runtimepy-4.2.2/runtimepy/net/server/app/env/
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/app/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/app/env/modal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.008887 runtimepy-4.2.2/runtimepy/net/server/app/env/tab/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/app/env/tab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/app/env/tab/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/app/env/tab/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/app/env/tab/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/app/env/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/app/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/app/placeholder.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/app/pyodide.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/app/sound.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/app/tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.008887 runtimepy-4.2.2/runtimepy/net/server/struct/
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/struct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.008887 runtimepy-4.2.2/runtimepy/net/server/websocket/
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/server/websocket/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.008887 runtimepy-4.2.2/runtimepy/net/stream/
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/stream/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.008887 runtimepy-4.2.2/runtimepy/net/stream/json/
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/stream/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/stream/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.008887 runtimepy-4.2.2/runtimepy/net/tcp/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/tcp/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/tcp/create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.008887 runtimepy-4.2.2/runtimepy/net/tcp/http/
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/tcp/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/tcp/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.008887 runtimepy-4.2.2/runtimepy/net/tcp/telnet/
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/tcp/telnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/tcp/telnet/codes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.008887 runtimepy-4.2.2/runtimepy/net/udp/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/udp/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/udp/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/udp/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.008887 runtimepy-4.2.2/runtimepy/net/websocket/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/net/websocket/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.012887 runtimepy-4.2.2/runtimepy/primitives/
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/primitives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.012887 runtimepy-4.2.2/runtimepy/primitives/array/
--rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/primitives/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/primitives/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/primitives/byte_order.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.012887 runtimepy-4.2.2/runtimepy/primitives/field/
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/primitives/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/primitives/field/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.012887 runtimepy-4.2.2/runtimepy/primitives/field/manager/
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/primitives/field/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/primitives/field/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/primitives/float.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/primitives/scaling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.012887 runtimepy-4.2.2/runtimepy/primitives/serializable/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/primitives/serializable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/primitives/serializable/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/primitives/serializable/fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/primitives/serializable/prefixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/primitives/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.012887 runtimepy-4.2.2/runtimepy/primitives/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/primitives/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/primitives/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/primitives/types/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/primitives/types/bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/primitives/types/float.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/primitives/types/int.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.016887 runtimepy-4.2.2/runtimepy/registry/
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/registry/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/registry/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/registry/name.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.016887 runtimepy-4.2.2/runtimepy/sample/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/sample/peer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/sample/program.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.016887 runtimepy-4.2.2/runtimepy/struct/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/struct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.016887 runtimepy-4.2.2/runtimepy/subprocess/
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/subprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/subprocess/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/subprocess/peer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/subprocess/program.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/subprocess/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.016887 runtimepy-4.2.2/runtimepy/task/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/task/asynchronous.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.016887 runtimepy-4.2.2/runtimepy/task/basic/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/task/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/task/basic/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/task/basic/periodic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/task/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.016887 runtimepy-4.2.2/runtimepy/task/trig/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/task/trig/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.016887 runtimepy-4.2.2/runtimepy/telemetry/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/telemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.016887 runtimepy-4.2.2/runtimepy/tui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/tui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.016887 runtimepy-4.2.2/runtimepy/tui/channels/
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/tui/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/tui/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/tui/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/tui/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/tui/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-24 07:05:55.000000 runtimepy-4.2.2/runtimepy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.020887 runtimepy-4.2.2/runtimepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-24 07:08:28.000000 runtimepy-4.2.2/runtimepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-04-24 07:08:28.000000 runtimepy-4.2.2/runtimepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 07:08:28.000000 runtimepy-4.2.2/runtimepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 07:08:28.000000 runtimepy-4.2.2/runtimepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-24 07:08:28.000000 runtimepy-4.2.2/runtimepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 07:08:28.000000 runtimepy-4.2.2/runtimepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 07:08:29.020887 runtimepy-4.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-24 07:05:55.000000 runtimepy-4.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:08:29.020887 runtimepy-4.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-24 07:05:55.000000 runtimepy-4.2.2/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-24 07:05:55.000000 runtimepy-4.2.2/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-24 07:05:55.000000 runtimepy-4.2.2/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.442204 runtimepy-4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-25 08:44:59.000000 runtimepy-4.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-25 08:47:33.442204 runtimepy-4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-25 08:44:59.000000 runtimepy-4.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-25 08:44:59.000000 runtimepy-4.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.402204 runtimepy-4.3.0/runtimepy/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.402204 runtimepy-4.3.0/runtimepy/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.406204 runtimepy-4.3.0/runtimepy/channel/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/channel/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/channel/environment/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/channel/environment/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.406204 runtimepy-4.3.0/runtimepy/channel/environment/command/
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/channel/environment/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/channel/environment/command/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/channel/environment/command/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/channel/environment/command/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/channel/environment/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/channel/environment/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/channel/environment/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/channel/environment/telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.406204 runtimepy-4.3.0/runtimepy/channel/event/
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/channel/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/channel/event/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/channel/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.406204 runtimepy-4.3.0/runtimepy/codec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/codec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.406204 runtimepy-4.3.0/runtimepy/codec/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/codec/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/codec/protocol/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/codec/protocol/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.406204 runtimepy-4.3.0/runtimepy/codec/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/codec/system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.406204 runtimepy-4.3.0/runtimepy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/commands/arbiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/commands/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/commands/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/commands/tui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.410204 runtimepy-4.3.0/runtimepy/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.410204 runtimepy-4.3.0/runtimepy/data/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/css/bootstrap_extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/css/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/dummy_load.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/factories.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   362870 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.410204 runtimepy-4.3.0/runtimepy/data/js/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/js/DataConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/js/JsonConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/js/audio.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.410204 runtimepy-4.3.0/runtimepy/data/js/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/js/classes/App.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/js/classes/ChannelTable.js
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/js/classes/DataConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/js/classes/JsonConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/js/classes/Plot.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/js/classes/PlotManager.js
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/js/classes/PlotModalManager.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/js/classes/TabFilter.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/js/classes/TabInterface.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/js/classes/WindowHashManager.js
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/js/classes/WorkerInterface.js
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/js/init.js
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/js/main.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.414204 runtimepy-4.3.0/runtimepy/data/js/tab/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/js/tab/env.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/js/tab/sound.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.414204 runtimepy-4.3.0/runtimepy/data/js/unused/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/js/unused/pyodide.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/js/util.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/js/worker.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.414204 runtimepy-4.3.0/runtimepy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/schemas/BitFields.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/schemas/Channel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/schemas/ChannelCommand.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/schemas/ChannelRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/schemas/ClientConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/schemas/EnumRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/schemas/FindFile.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/schemas/PeerProcessConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/schemas/RuntimeEnum.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/schemas/ServerConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/schemas/StructConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/schemas/TaskConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/schemas/has_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/schemas/has_factory.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/schemas/has_name.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/schemas/has_request_flag.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/server.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/server_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/data/server_dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.414204 runtimepy-4.3.0/runtimepy/enum/
+-rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/enum/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/enum/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.418204 runtimepy-4.3.0/runtimepy/message/
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/message/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11285 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/message/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/message/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.418204 runtimepy-4.3.0/runtimepy/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/metrics/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/metrics/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/metrics/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.418204 runtimepy-4.3.0/runtimepy/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/mixins/async_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/mixins/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/mixins/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/mixins/finalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/mixins/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/mixins/psutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/mixins/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.418204 runtimepy-4.3.0/runtimepy/net/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.418204 runtimepy-4.3.0/runtimepy/net/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.422204 runtimepy-4.3.0/runtimepy/net/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14523 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/arbiter/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.422204 runtimepy-4.3.0/runtimepy/net/arbiter/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/arbiter/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/arbiter/config/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/arbiter/config/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.422204 runtimepy-4.3.0/runtimepy/net/arbiter/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/arbiter/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/arbiter/factory/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/arbiter/factory/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.422204 runtimepy-4.3.0/runtimepy/net/arbiter/housekeeping/
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/arbiter/housekeeping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.422204 runtimepy-4.3.0/runtimepy/net/arbiter/imports/
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/arbiter/imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/arbiter/imports/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/arbiter/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/arbiter/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/arbiter/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.422204 runtimepy-4.3.0/runtimepy/net/arbiter/tcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/arbiter/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/arbiter/tcp/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/arbiter/udp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/arbiter/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11894 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.422204 runtimepy-4.3.0/runtimepy/net/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/factories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.422204 runtimepy-4.3.0/runtimepy/net/http/
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/http/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/http/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/http/request_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/http/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/http/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/http/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.426204 runtimepy-4.3.0/runtimepy/net/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.426204 runtimepy-4.3.0/runtimepy/net/server/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/app/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.426204 runtimepy-4.3.0/runtimepy/net/server/app/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/app/bootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/app/bootstrap/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/app/bootstrap/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/app/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/app/elements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.426204 runtimepy-4.3.0/runtimepy/net/server/app/env/
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/app/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/app/env/modal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.426204 runtimepy-4.3.0/runtimepy/net/server/app/env/tab/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/app/env/tab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/app/env/tab/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/app/env/tab/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/app/env/tab/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/app/env/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/app/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/app/placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/app/pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/app/sound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/app/tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.426204 runtimepy-4.3.0/runtimepy/net/server/struct/
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/struct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.426204 runtimepy-4.3.0/runtimepy/net/server/websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/server/websocket/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.430204 runtimepy-4.3.0/runtimepy/net/stream/
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/stream/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.430204 runtimepy-4.3.0/runtimepy/net/stream/json/
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/stream/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/stream/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.430204 runtimepy-4.3.0/runtimepy/net/tcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/tcp/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/tcp/create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.430204 runtimepy-4.3.0/runtimepy/net/tcp/http/
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/tcp/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/tcp/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.430204 runtimepy-4.3.0/runtimepy/net/tcp/telnet/
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/tcp/telnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/tcp/telnet/codes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.430204 runtimepy-4.3.0/runtimepy/net/udp/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/udp/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/udp/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/udp/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.430204 runtimepy-4.3.0/runtimepy/net/websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/net/websocket/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.434204 runtimepy-4.3.0/runtimepy/primitives/
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/primitives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.434204 runtimepy-4.3.0/runtimepy/primitives/array/
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/primitives/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/primitives/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/primitives/byte_order.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.434204 runtimepy-4.3.0/runtimepy/primitives/field/
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/primitives/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/primitives/field/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.434204 runtimepy-4.3.0/runtimepy/primitives/field/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/primitives/field/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/primitives/field/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/primitives/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/primitives/scaling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.434204 runtimepy-4.3.0/runtimepy/primitives/serializable/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/primitives/serializable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/primitives/serializable/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/primitives/serializable/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/primitives/serializable/prefixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/primitives/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.434204 runtimepy-4.3.0/runtimepy/primitives/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/primitives/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/primitives/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/primitives/types/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/primitives/types/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/primitives/types/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/primitives/types/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.434204 runtimepy-4.3.0/runtimepy/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/registry/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/registry/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/registry/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.438204 runtimepy-4.3.0/runtimepy/sample/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/sample/peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/sample/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.438204 runtimepy-4.3.0/runtimepy/struct/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/struct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.438204 runtimepy-4.3.0/runtimepy/subprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/subprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/subprocess/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/subprocess/peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6792 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/subprocess/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/subprocess/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.438204 runtimepy-4.3.0/runtimepy/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/task/asynchronous.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.438204 runtimepy-4.3.0/runtimepy/task/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/task/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/task/basic/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/task/basic/periodic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/task/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.438204 runtimepy-4.3.0/runtimepy/task/trig/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/task/trig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.438204 runtimepy-4.3.0/runtimepy/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/telemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.438204 runtimepy-4.3.0/runtimepy/tui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/tui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.438204 runtimepy-4.3.0/runtimepy/tui/channels/
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/tui/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/tui/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/tui/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/tui/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/tui/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-25 08:44:59.000000 runtimepy-4.3.0/runtimepy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.442204 runtimepy-4.3.0/runtimepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-25 08:47:33.000000 runtimepy-4.3.0/runtimepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-04-25 08:47:33.000000 runtimepy-4.3.0/runtimepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:47:33.000000 runtimepy-4.3.0/runtimepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 08:47:33.000000 runtimepy-4.3.0/runtimepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-25 08:47:33.000000 runtimepy-4.3.0/runtimepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 08:47:33.000000 runtimepy-4.3.0/runtimepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 08:47:33.442204 runtimepy-4.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-25 08:44:59.000000 runtimepy-4.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:33.438204 runtimepy-4.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-25 08:44:59.000000 runtimepy-4.3.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-25 08:44:59.000000 runtimepy-4.3.0/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-25 08:44:59.000000 runtimepy-4.3.0/tests/test_resources.py
```

### Comparing `runtimepy-4.2.2/LICENSE` & `runtimepy-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/PKG-INFO` & `runtimepy-4.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 4.2.2
+Version: 4.3.0
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -13,18 +13,18 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: psutil
+Requires-Dist: websockets
 Requires-Dist: vcorelib>=3.2.4
 Requires-Dist: svgen>=0.6.6
-Requires-Dist: websockets
+Requires-Dist: psutil
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
@@ -40,19 +40,19 @@
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: uvloop; (sys_platform != "win32" and sys_platform != "cygwin") and extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=5f56531d1be3002a8547ddb013d713f9
+    hash=2adcb8a8e9a6b4dffec41ec316de0fee
     =====================================
 -->
 
-# runtimepy ([4.2.2](https://pypi.org/project/runtimepy/))
+# runtimepy ([4.3.0](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-4.2.2/README.md` & `runtimepy-4.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=5f56531d1be3002a8547ddb013d713f9
+    hash=2adcb8a8e9a6b4dffec41ec316de0fee
     =====================================
 -->
 
-# runtimepy ([4.2.2](https://pypi.org/project/runtimepy/))
+# runtimepy ([4.3.0](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-4.2.2/pyproject.toml` & `runtimepy-4.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "runtimepy"
-version = "4.2.2"
+version = "4.3.0"
 description = "A framework for implementing Python services."
 readme = "README.md"
 requires-python = ">=3.11"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `runtimepy-4.2.2/runtimepy/app.py` & `runtimepy-4.3.0/runtimepy/app.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/channel/__init__.py` & `runtimepy-4.3.0/runtimepy/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/channel/environment/__init__.py` & `runtimepy-4.3.0/runtimepy/channel/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/channel/environment/array.py` & `runtimepy-4.3.0/runtimepy/channel/environment/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/channel/environment/base.py` & `runtimepy-4.3.0/runtimepy/channel/environment/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/channel/environment/command/__init__.py` & `runtimepy-4.3.0/runtimepy/channel/environment/command/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/channel/environment/command/parser.py` & `runtimepy-4.3.0/runtimepy/channel/environment/command/parser.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/channel/environment/command/processor.py` & `runtimepy-4.3.0/runtimepy/channel/environment/command/processor.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/channel/environment/command/result.py` & `runtimepy-4.3.0/runtimepy/channel/environment/command/result.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/channel/environment/create.py` & `runtimepy-4.3.0/runtimepy/channel/environment/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/channel/environment/file.py` & `runtimepy-4.3.0/runtimepy/channel/environment/file.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/channel/environment/sample.py` & `runtimepy-4.3.0/runtimepy/channel/environment/sample.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/channel/environment/telemetry.py` & `runtimepy-4.3.0/runtimepy/channel/environment/telemetry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/channel/event/__init__.py` & `runtimepy-4.3.0/runtimepy/channel/event/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/channel/event/header.py` & `runtimepy-4.3.0/runtimepy/channel/event/header.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/channel/registry.py` & `runtimepy-4.3.0/runtimepy/channel/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/codec/protocol/__init__.py` & `runtimepy-4.3.0/runtimepy/codec/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/codec/protocol/base.py` & `runtimepy-4.3.0/runtimepy/codec/protocol/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/codec/protocol/json.py` & `runtimepy-4.3.0/runtimepy/codec/protocol/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/codec/system/__init__.py` & `runtimepy-4.3.0/runtimepy/codec/system/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/commands/all.py` & `runtimepy-4.3.0/runtimepy/commands/all.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/commands/arbiter.py` & `runtimepy-4.3.0/runtimepy/commands/arbiter.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/commands/common.py` & `runtimepy-4.3.0/runtimepy/commands/common.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/commands/server.py` & `runtimepy-4.3.0/runtimepy/commands/server.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/commands/task.py` & `runtimepy-4.3.0/runtimepy/commands/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/commands/tui.py` & `runtimepy-4.3.0/runtimepy/commands/tui.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/data/css/bootstrap_extra.css` & `runtimepy-4.3.0/runtimepy/data/css/bootstrap_extra.css`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/data/dummy_load.yaml` & `runtimepy-4.3.0/runtimepy/data/dummy_load.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -41,9 +41,17 @@
   - name: struct3
     factory: sample_struct
 
 # Sample peer processes.
 processes:
   - name: proc1
     factory: sample_peer
-    config: *cfg
+
+    # The peer itself runs an arbiter process.
+    config:
+      includes:
+        - package://runtimepy/server.yaml
+
+      app: runtimepy.sample.program.run
+      config: *cfg
+
     program: runtimepy.sample.program.SampleProgram
```

### Comparing `runtimepy-4.2.2/runtimepy/data/factories.yaml` & `runtimepy-4.3.0/runtimepy/data/factories.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/data/favicon.ico` & `runtimepy-4.3.0/runtimepy/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/data/js/JsonConnection.js` & `runtimepy-4.3.0/runtimepy/data/js/JsonConnection.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/data/js/audio.js` & `runtimepy-4.3.0/runtimepy/data/js/audio.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/data/js/classes/App.js` & `runtimepy-4.3.0/runtimepy/data/js/classes/App.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/data/js/classes/ChannelTable.js` & `runtimepy-4.3.0/runtimepy/data/js/classes/ChannelTable.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/data/js/classes/JsonConnection.js` & `runtimepy-4.3.0/runtimepy/data/js/classes/JsonConnection.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/data/js/classes/Plot.js` & `runtimepy-4.3.0/runtimepy/data/js/classes/Plot.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/data/js/classes/PlotManager.js` & `runtimepy-4.3.0/runtimepy/data/js/classes/PlotManager.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/data/js/classes/PlotModalManager.js` & `runtimepy-4.3.0/runtimepy/data/js/classes/PlotModalManager.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/data/js/classes/TabFilter.js` & `runtimepy-4.3.0/runtimepy/data/js/classes/TabFilter.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/data/js/classes/TabInterface.js` & `runtimepy-4.3.0/runtimepy/data/js/classes/TabInterface.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/data/js/classes/WindowHashManager.js` & `runtimepy-4.3.0/runtimepy/data/js/classes/WindowHashManager.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/data/js/tab/sound.js` & `runtimepy-4.3.0/runtimepy/data/js/tab/sound.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/data/js/unused/pyodide.js` & `runtimepy-4.3.0/runtimepy/data/js/unused/pyodide.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/data/js/util.js` & `runtimepy-4.3.0/runtimepy/data/js/util.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/data/js/worker.js` & `runtimepy-4.3.0/runtimepy/data/js/worker.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/data/schemas/BitFields.yaml` & `runtimepy-4.3.0/runtimepy/data/schemas/BitFields.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/data/schemas/ConnectionArbiterConfig.yaml` & `runtimepy-4.3.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/data/schemas/FindFile.yaml` & `runtimepy-4.3.0/runtimepy/data/schemas/FindFile.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/data/server_base.yaml` & `runtimepy-4.3.0/runtimepy/data/server_base.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/entry.py` & `runtimepy-4.3.0/runtimepy/entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/enum/__init__.py` & `runtimepy-4.3.0/runtimepy/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/enum/registry.py` & `runtimepy-4.3.0/runtimepy/enum/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/enum/types.py` & `runtimepy-4.3.0/runtimepy/enum/types.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/mapping.py` & `runtimepy-4.3.0/runtimepy/mapping.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/message/__init__.py` & `runtimepy-4.3.0/runtimepy/message/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/message/handlers.py` & `runtimepy-4.3.0/runtimepy/message/handlers.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/message/interface.py` & `runtimepy-4.3.0/runtimepy/message/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,21 @@
             ChannelCommand,
             channel_env_handler(ENVIRONMENTS.data, self.command),
         )
 
     async def poll_handler(self) -> None:
         """Poll this instance."""
 
+    def send_poll(self, loopback: int = 1) -> None:
+        """
+        Send a poll message with a default loopback of 1, so that this instance
+        will also be polled.
+        """
+        self.send_json({"poll": {"loopback": loopback}})
+
     async def _poll_handler(
         self, outbox: JsonMessage, inbox: JsonMessage
     ) -> None:
         """Handle a 'poll' message."""
 
         await self.poll_handler()
 
@@ -189,14 +196,24 @@
             data["__log_messages__"] = self._log_messages  # type: ignore
             self._log_messages = []
 
         with BytesIO() as stream:
             self.processor.encode_json(stream, data)
             self.write(stream.getvalue(), addr=addr)
 
+    def handle_log_message(self, message: JsonMessage) -> None:
+        """Handle a log message."""
+
+        if "msg" in message and message["msg"]:
+            self.logger.log(
+                message.get("level", logging.INFO),
+                "remote: " + message["msg"],
+                *message.get("args", []),
+            )
+
     def _handle_reserved(
         self, data: JsonMessage, response: JsonMessage
     ) -> bool:
         """Handle special keys in an incoming message."""
 
         should_respond = True
 
@@ -214,20 +231,15 @@
                 should_respond = False
 
             response["__id__"] = ident
 
         # Log messages sent by the peer.
         if "__log_messages__" in data:
             for message in data["__log_messages__"]:
-                if "msg" in message and message["msg"]:
-                    self.logger.log(
-                        message.get("level", logging.INFO),
-                        "remote: " + message["msg"],
-                        *message.get("args", []),
-                    )
+                self.handle_log_message(message)
             del data["__log_messages__"]
 
         return should_respond
 
     async def wait_json(
         self,
         data: Union[JsonMessage, JsonCodec] = None,
```

### Comparing `runtimepy-4.2.2/runtimepy/message/types.py` & `runtimepy-4.3.0/runtimepy/message/types.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/metrics/channel.py` & `runtimepy-4.3.0/runtimepy/metrics/channel.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/metrics/connection.py` & `runtimepy-4.3.0/runtimepy/metrics/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/metrics/task.py` & `runtimepy-4.3.0/runtimepy/metrics/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/mixins/async_command.py` & `runtimepy-4.3.0/runtimepy/mixins/async_command.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/mixins/enum.py` & `runtimepy-4.3.0/runtimepy/mixins/enum.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/mixins/environment.py` & `runtimepy-4.3.0/runtimepy/mixins/environment.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/mixins/finalize.py` & `runtimepy-4.3.0/runtimepy/mixins/finalize.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/mixins/logging.py` & `runtimepy-4.3.0/runtimepy/mixins/logging.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/mixins/psutil.py` & `runtimepy-4.3.0/runtimepy/mixins/psutil.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/mixins/regex.py` & `runtimepy-4.3.0/runtimepy/mixins/regex.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/__init__.py` & `runtimepy-4.3.0/runtimepy/net/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/apps/__init__.py` & `runtimepy-4.3.0/runtimepy/net/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/arbiter/__init__.py` & `runtimepy-4.3.0/runtimepy/net/arbiter/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/arbiter/base.py` & `runtimepy-4.3.0/runtimepy/net/arbiter/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/arbiter/config/__init__.py` & `runtimepy-4.3.0/runtimepy/net/arbiter/config/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/arbiter/config/codec.py` & `runtimepy-4.3.0/runtimepy/net/arbiter/config/codec.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/arbiter/config/util.py` & `runtimepy-4.3.0/runtimepy/net/arbiter/config/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/arbiter/factory/connection.py` & `runtimepy-4.3.0/runtimepy/net/arbiter/factory/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/arbiter/factory/task.py` & `runtimepy-4.3.0/runtimepy/net/arbiter/factory/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/arbiter/housekeeping/__init__.py` & `runtimepy-4.3.0/runtimepy/net/arbiter/housekeeping/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/arbiter/imports/__init__.py` & `runtimepy-4.3.0/runtimepy/net/arbiter/imports/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/arbiter/imports/util.py` & `runtimepy-4.3.0/runtimepy/net/arbiter/imports/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/arbiter/info.py` & `runtimepy-4.3.0/runtimepy/net/arbiter/info.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/arbiter/result.py` & `runtimepy-4.3.0/runtimepy/net/arbiter/result.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/arbiter/task.py` & `runtimepy-4.3.0/runtimepy/net/arbiter/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/arbiter/tcp/__init__.py` & `runtimepy-4.3.0/runtimepy/net/arbiter/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/arbiter/tcp/json.py` & `runtimepy-4.3.0/runtimepy/net/arbiter/tcp/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/arbiter/udp.py` & `runtimepy-4.3.0/runtimepy/net/arbiter/udp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/arbiter/websocket.py` & `runtimepy-4.3.0/runtimepy/net/arbiter/websocket.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/backoff.py` & `runtimepy-4.3.0/runtimepy/net/backoff.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/connection.py` & `runtimepy-4.3.0/runtimepy/net/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/factories/__init__.py` & `runtimepy-4.3.0/runtimepy/net/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/http/__init__.py` & `runtimepy-4.3.0/runtimepy/net/http/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/http/common.py` & `runtimepy-4.3.0/runtimepy/net/http/common.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/http/header.py` & `runtimepy-4.3.0/runtimepy/net/http/header.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/http/request_target.py` & `runtimepy-4.3.0/runtimepy/net/http/request_target.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/http/response.py` & `runtimepy-4.3.0/runtimepy/net/http/response.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/http/state.py` & `runtimepy-4.3.0/runtimepy/net/http/state.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/http/version.py` & `runtimepy-4.3.0/runtimepy/net/http/version.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/manager.py` & `runtimepy-4.3.0/runtimepy/net/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/mixin.py` & `runtimepy-4.3.0/runtimepy/net/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/server/__init__.py` & `runtimepy-4.3.0/runtimepy/net/server/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/server/app/__init__.py` & `runtimepy-4.3.0/runtimepy/net/server/app/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/server/app/base.py` & `runtimepy-4.3.0/runtimepy/net/server/app/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/server/app/bootstrap/__init__.py` & `runtimepy-4.3.0/runtimepy/net/server/app/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/server/app/bootstrap/elements.py` & `runtimepy-4.3.0/runtimepy/net/server/app/bootstrap/elements.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/server/app/bootstrap/tabs.py` & `runtimepy-4.3.0/runtimepy/net/server/app/bootstrap/tabs.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/server/app/create.py` & `runtimepy-4.3.0/runtimepy/net/server/app/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/server/app/env/__init__.py` & `runtimepy-4.3.0/runtimepy/net/server/app/env/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from runtimepy.net.arbiter.info import AppInfo
 from runtimepy.net.server.app.bootstrap.elements import input_box
 from runtimepy.net.server.app.bootstrap.tabs import TabbedContent
 from runtimepy.net.server.app.env.modal import Modal
 from runtimepy.net.server.app.env.tab import ChannelEnvironmentTab
 from runtimepy.net.server.app.placeholder import dummy_tabs, under_construction
 from runtimepy.net.server.app.sound import SoundTab
+from runtimepy.subprocess.program import PROGRAM
 
 
 def channel_environments(app: AppInfo, tabs: TabbedContent) -> None:
     """Populate application elements."""
 
     # Remove tab-content scrolling.
     tabs.set_scroll(False)
@@ -40,26 +41,43 @@
     # Struct tabs.
     for struct in app.structs.values():
         ChannelEnvironmentTab(
             struct.name, struct.command, app, tabs, icon="bucket"
         ).entry()
 
     # Subprocess tabs.
-    for name, peer in app.peers.items():
+    for peer in app.peers.values():
         # Host side.
         ChannelEnvironmentTab(
             peer.struct.name, peer.struct.command, app, tabs, icon="cpu-fill"
         ).entry()
 
         # Remote side.
         assert peer.peer is not None
         ChannelEnvironmentTab(
             peer.peer_name, peer.peer, app, tabs, icon="cpu"
         ).entry()
 
+    # If we are a peer program, load environments.
+    if PROGRAM is not None:
+        # Host side.
+        ChannelEnvironmentTab(
+            PROGRAM.struct.name,
+            PROGRAM.struct.command,
+            app,
+            tabs,
+            icon="cpu-fill",
+        ).entry()
+
+        # Remote side.
+        assert PROGRAM.peer is not None
+        ChannelEnvironmentTab(
+            PROGRAM.peer_name, PROGRAM.peer, app, tabs, icon="cpu"
+        ).entry()
+
     # Toggle channel-table button.
     tabs.add_button(
         "Toggle channel table",
         ".channel-column",
         icon="table",
         id="channels-button",
     )
```

### Comparing `runtimepy-4.2.2/runtimepy/net/server/app/env/modal.py` & `runtimepy-4.3.0/runtimepy/net/server/app/env/modal.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/server/app/env/tab/__init__.py` & `runtimepy-4.3.0/runtimepy/net/server/app/env/tab/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/server/app/env/tab/base.py` & `runtimepy-4.3.0/runtimepy/net/server/app/env/tab/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/server/app/env/tab/html.py` & `runtimepy-4.3.0/runtimepy/net/server/app/env/tab/html.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/server/app/env/tab/message.py` & `runtimepy-4.3.0/runtimepy/net/server/app/env/tab/message.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/server/app/env/widgets.py` & `runtimepy-4.3.0/runtimepy/net/server/app/env/widgets.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/server/app/files.py` & `runtimepy-4.3.0/runtimepy/net/server/app/files.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/server/app/placeholder.py` & `runtimepy-4.3.0/runtimepy/net/server/app/placeholder.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/server/app/sound.py` & `runtimepy-4.3.0/runtimepy/net/server/app/sound.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/server/app/tab.py` & `runtimepy-4.3.0/runtimepy/net/server/app/tab.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/server/html.py` & `runtimepy-4.3.0/runtimepy/net/server/html.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/server/json.py` & `runtimepy-4.3.0/runtimepy/net/server/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/server/struct/__init__.py` & `runtimepy-4.3.0/runtimepy/net/server/struct/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/server/websocket/__init__.py` & `runtimepy-4.3.0/runtimepy/net/server/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/server/websocket/state.py` & `runtimepy-4.3.0/runtimepy/net/server/websocket/state.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/stream/__init__.py` & `runtimepy-4.3.0/runtimepy/net/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/stream/base.py` & `runtimepy-4.3.0/runtimepy/net/stream/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/stream/json/__init__.py` & `runtimepy-4.3.0/runtimepy/net/stream/json/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/stream/string.py` & `runtimepy-4.3.0/runtimepy/net/stream/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/tcp/connection.py` & `runtimepy-4.3.0/runtimepy/net/tcp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/tcp/create.py` & `runtimepy-4.3.0/runtimepy/net/tcp/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/tcp/http/__init__.py` & `runtimepy-4.3.0/runtimepy/net/tcp/http/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/tcp/protocol.py` & `runtimepy-4.3.0/runtimepy/net/tcp/protocol.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/tcp/telnet/__init__.py` & `runtimepy-4.3.0/runtimepy/net/tcp/telnet/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/tcp/telnet/codes.py` & `runtimepy-4.3.0/runtimepy/net/tcp/telnet/codes.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/udp/connection.py` & `runtimepy-4.3.0/runtimepy/net/udp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/udp/create.py` & `runtimepy-4.3.0/runtimepy/net/udp/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/udp/protocol.py` & `runtimepy-4.3.0/runtimepy/net/udp/protocol.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/util.py` & `runtimepy-4.3.0/runtimepy/net/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/net/websocket/connection.py` & `runtimepy-4.3.0/runtimepy/net/websocket/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/primitives/__init__.py` & `runtimepy-4.3.0/runtimepy/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/primitives/array/__init__.py` & `runtimepy-4.3.0/runtimepy/primitives/array/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/primitives/base.py` & `runtimepy-4.3.0/runtimepy/primitives/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/primitives/bool.py` & `runtimepy-4.3.0/runtimepy/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/primitives/byte_order.py` & `runtimepy-4.3.0/runtimepy/primitives/byte_order.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/primitives/field/__init__.py` & `runtimepy-4.3.0/runtimepy/primitives/field/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/primitives/field/fields.py` & `runtimepy-4.3.0/runtimepy/primitives/field/fields.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/primitives/field/manager/__init__.py` & `runtimepy-4.3.0/runtimepy/primitives/field/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/primitives/field/manager/base.py` & `runtimepy-4.3.0/runtimepy/primitives/field/manager/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/primitives/float.py` & `runtimepy-4.3.0/runtimepy/primitives/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/primitives/int.py` & `runtimepy-4.3.0/runtimepy/primitives/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/primitives/scaling.py` & `runtimepy-4.3.0/runtimepy/primitives/scaling.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/primitives/serializable/base.py` & `runtimepy-4.3.0/runtimepy/primitives/serializable/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/primitives/serializable/fixed.py` & `runtimepy-4.3.0/runtimepy/primitives/serializable/fixed.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/primitives/serializable/prefixed.py` & `runtimepy-4.3.0/runtimepy/primitives/serializable/prefixed.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/primitives/string.py` & `runtimepy-4.3.0/runtimepy/primitives/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/primitives/types/__init__.py` & `runtimepy-4.3.0/runtimepy/primitives/types/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/primitives/types/base.py` & `runtimepy-4.3.0/runtimepy/primitives/types/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/primitives/types/bool.py` & `runtimepy-4.3.0/runtimepy/primitives/types/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/primitives/types/bounds.py` & `runtimepy-4.3.0/runtimepy/primitives/types/bounds.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/primitives/types/float.py` & `runtimepy-4.3.0/runtimepy/primitives/types/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/primitives/types/int.py` & `runtimepy-4.3.0/runtimepy/primitives/types/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/registry/__init__.py` & `runtimepy-4.3.0/runtimepy/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/registry/bool.py` & `runtimepy-4.3.0/runtimepy/registry/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/registry/item.py` & `runtimepy-4.3.0/runtimepy/registry/item.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/registry/name.py` & `runtimepy-4.3.0/runtimepy/registry/name.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/schemas.py` & `runtimepy-4.3.0/runtimepy/schemas.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/struct/__init__.py` & `runtimepy-4.3.0/runtimepy/struct/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/subprocess/__init__.py` & `runtimepy-4.3.0/runtimepy/subprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/subprocess/interface.py` & `runtimepy-4.3.0/runtimepy/subprocess/interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 A module implementing a runtimepy peer interface.
 """
 
 # built-in
 from argparse import Namespace
 import asyncio
 from io import BytesIO
-from logging import getLogger
+from json import dumps
+from logging import INFO, getLogger
 from typing import Optional
 
 # third-party
 from vcorelib.io.types import JsonObject
 
 # internal
 from runtimepy import METRICS_NAME
@@ -44,14 +45,16 @@
 
         self.processor = MessageProcessor()
 
         self.basename = name
         self.struct = self.struct_type(self.basename + HOST_SUFFIX, config)
 
         self.peer: Optional[RemoteCommandProcessor] = None
+        self.peer_config: Optional[JsonMessage] = None
+        self.peer_config_event = asyncio.Event()
         self._peer_env_event = asyncio.Event()
 
         # Set these for JsonMessageInterface.
         AsyncCommandProcessingMixin.__init__(self, logger=self.struct.logger)
         self.command = self.struct.command
 
         self._setup_async_commands()
@@ -59,14 +62,26 @@
 
         self.struct_pre_finalize()
         self._finalize_struct()
 
     def struct_pre_finalize(self) -> None:
         """Configure struct before finalization."""
 
+    def handle_log_message(self, message: JsonMessage) -> None:
+        """Handle a log message."""
+
+        logger = self.logger
+        msg = "remote: " + message["msg"]
+
+        if self.peer is not None:
+            logger = self.peer.logger
+            msg = message["msg"]
+
+        logger.log(message.get("level", INFO), msg, *message.get("args", []))
+
     @property
     def peer_name(self) -> str:
         """Get the name of the peer's environment."""
         return self.basename + PEER_SUFFIX
 
     def _set_peer_env(self, data: JsonMessage) -> bool:
         """Set the peer's environment."""
@@ -127,14 +142,35 @@
 
             # Exchange environments.
             if self._set_peer_env(inbox):
                 outbox.update(self.struct.env.export_json())
 
         self.basic_handler("env", env_handler)
 
+        async def config_handler(
+            outbox: JsonMessage, inbox: JsonMessage
+        ) -> None:
+            """Store peer's configuration."""
+
+            if self.peer_config is None:
+                self.peer_config = inbox["config"]
+                outbox["config"] = self.struct.config
+                self.logger.info(
+                    "Peer's configuration: '%s'.",
+                    dumps(self.peer_config, indent=4),
+                )
+                self.peer_config_event.set()
+
+        self.basic_handler("config", config_handler)
+
+    async def share_config(self, data: JsonMessage) -> None:
+        """Exchange configuration data."""
+
+        await self.wait_json({"config": data})
+
     async def share_environment(self) -> None:
         """Exchange channel environments."""
 
         result = await self.wait_json({"env": self.struct.env.export_json()})
         self._set_peer_env(result["env"])
 
     def _finalize_struct(self) -> None:
```

### Comparing `runtimepy-4.2.2/runtimepy/subprocess/peer.py` & `runtimepy-4.3.0/runtimepy/subprocess/peer.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import asyncio
 from contextlib import asynccontextmanager, suppress
 from pathlib import Path
 from sys import executable
 from typing import AsyncIterator, Type, TypeVar
 
 # third-party
-from vcorelib.io import ARBITER
+from vcorelib.io import ARBITER, DEFAULT_INCLUDES_KEY
 from vcorelib.io.file_writer import IndentedFileWriter
 from vcorelib.io.types import JsonObject
 from vcorelib.paths.context import tempfile
 
 # internal
 from runtimepy.subprocess import spawn_exec, spawn_shell
 from runtimepy.subprocess.interface import RuntimepyPeerInterface
@@ -69,15 +69,14 @@
         # Register task that will poll queues.
         task = asyncio.create_task(self._poll())
 
         try:
             with suppress(AssertionError):
                 if await self.loopback():
                     await self.wait_json({"meta": self.meta})
-
                     await self.share_environment()
 
             yield self
         finally:
             task.cancel()
             await task
 
@@ -118,28 +117,29 @@
         config_path: Path,
         import_str: str,
     ) -> None:
         """Write a script file for running the desired peer program."""
 
         writer.write("import sys")
         writer.write("from vcorelib.asyncio import run_handle_interrupt")
-        writer.write("from vcorelib.io import ARBITER")
+        writer.write("from vcorelib.io import ARBITER, DEFAULT_INCLUDES_KEY")
 
         from_str, to_import = import_str_and_item(import_str)
         writer.write(f"from {from_str} import {to_import}")
 
         fixed_path = str(config_path).replace("\\", "\\\\")
         writer.write(f'CONFIG_PATH = "{fixed_path}"')
 
         writer.write('if __name__ == "__main__":')
         with writer.indented():
             writer.write(
                 f'run_handle_interrupt({to_import}.run("{name}", '
                 "ARBITER.decode(CONFIG_PATH, "
-                "require_success=True).data, sys.argv))"
+                "require_success=True, includes_key=DEFAULT_INCLUDES_KEY"
+                ").data, sys.argv))"
             )
             writer.write("sys.exit(0)")
 
     @classmethod
     @asynccontextmanager
     async def running_program(
         cls: Type[T],
@@ -151,14 +151,22 @@
     ) -> AsyncIterator[T]:
         """Run a peer subprocess."""
 
         with tempfile(suffix=".json") as config_path:
             # Encode configuration data.
             assert ARBITER.encode(config_path, config)[0]
 
+            # Decode to load includes.
+            config = ARBITER.decode(
+                config_path,
+                require_success=True,
+                includes_key=DEFAULT_INCLUDES_KEY,
+            ).data
+            assert ARBITER.encode(config_path, config)[0]
+
             with tempfile(suffix=".py") as path:
                 # Write file contents.
                 with IndentedFileWriter.from_path(
                     path, per_indent=4, linesep="\n"
                 ) as writer:
                     cls._write_script(writer, name, config_path, import_str)
```

### Comparing `runtimepy-4.2.2/runtimepy/subprocess/program.py` & `runtimepy-4.3.0/runtimepy/subprocess/program.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,37 +5,51 @@
 # built-in
 import asyncio
 from contextlib import asynccontextmanager, contextmanager, suppress
 import logging
 import os
 import signal
 import sys
-from typing import AsyncIterator, BinaryIO, Iterator, Type, TypeVar
+from typing import AsyncIterator, BinaryIO, Iterator, Optional, Type, TypeVar
 
 # third-party
+from vcorelib.io import ARBITER
 from vcorelib.io.types import JsonObject
+from vcorelib.paths.context import tempfile
 
 # internal
 from runtimepy.metrics.channel import ChannelMetrics
 from runtimepy.mixins.psutil import PsutilMixin
+from runtimepy.net.arbiter import ConnectionArbiter
 from runtimepy.net.arbiter.info import RuntimeStruct, SampleStruct
 from runtimepy.subprocess.interface import RuntimepyPeerInterface
 
 T = TypeVar("T", bound="PeerProgram")
+PROGRAM: Optional["PeerProgram"] = None
 
 
 class PeerProgram(RuntimepyPeerInterface, PsutilMixin):
     """A communication interface for peer programs."""
 
     json_output: BinaryIO
     stream_output: BinaryIO
     stream_metrics: ChannelMetrics
 
     struct_type: Type[RuntimeStruct] = SampleStruct
 
+    got_eof: asyncio.Event
+
+    _singleton: Optional["PeerProgram"] = None
+
+    @classmethod
+    def singleton(cls: type[T]) -> T:
+        """Get a shared single instance of a protocol for this class."""
+        assert cls._singleton is not None
+        return cls._singleton  # type: ignore
+
     @contextmanager
     def streaming_events(self) -> Iterator[None]:
         """Stream events to the stream output."""
 
         with self.struct.env.registered(
             self.stream_output, flush=True, channel=self.stream_metrics
         ):
@@ -100,30 +114,48 @@
                     await self.process_json(msg)
                     saw_msg = True
 
                 if saw_msg:
                     self.stdin_metrics.increment(accumulator)
                     accumulator = 0
 
+        # Signal the end of input processing.
+        self.got_eof.set()
+
     @classmethod
     def run_standard(
         cls: Type[T], name: str, config: JsonObject
     ) -> tuple[asyncio.Task[None], T]:
         """Run this program using standard input and output."""
 
         peer = cls(name, config)
         peer.json_output = sys.stdout.buffer
         peer.stream_output = sys.stderr.buffer
+        peer.got_eof = asyncio.Event()
         peer.stream_metrics = ChannelMetrics()
 
+        global PROGRAM  # pylint: disable=global-statement
+        PROGRAM = peer
+        assert cls._singleton is None
+        cls._singleton = peer
+
         return asyncio.create_task(peer.io_task(sys.stdin.buffer)), peer
 
     async def main(self, argv: list[str]) -> None:
         """Program entry."""
 
+        del argv
+
+        with tempfile(suffix=".json") as config_path:
+            arbiter = ConnectionArbiter(stop_sig=self.got_eof)
+            ARBITER.encode(config_path, self.struct.config)
+            await arbiter.load_configs([config_path], wait_for_stop=True)
+
+        await arbiter.app()
+
     async def cleanup(self) -> None:
         """Runs when program 'running' context exits."""
 
     def pre_environment_exchange(self) -> None:
         """Perform early initialization tasks."""
 
     def struct_pre_finalize(self) -> None:
```

### Comparing `runtimepy-4.2.2/runtimepy/subprocess/protocol.py` & `runtimepy-4.3.0/runtimepy/subprocess/protocol.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/task/asynchronous.py` & `runtimepy-4.3.0/runtimepy/task/asynchronous.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/task/basic/manager.py` & `runtimepy-4.3.0/runtimepy/task/basic/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/task/basic/periodic.py` & `runtimepy-4.3.0/runtimepy/task/basic/periodic.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/task/sample.py` & `runtimepy-4.3.0/runtimepy/task/sample.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
         for name, struct in self.app.structs.items():
             if "struct" in name:
                 struct.poll()
 
         # Send poll message to peer process.
         for peer in self.app.peers.values():
-            peer.send_json({"poll": {"loopback": 1}})
+            peer.send_poll()
 
         return True
 
 
 class SampleApp(TaskFactory[SampleAppTask]):
     """A TUI application factory."""
```

### Comparing `runtimepy-4.2.2/runtimepy/task/trig/__init__.py` & `runtimepy-4.3.0/runtimepy/task/trig/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/tui/channels/__init__.py` & `runtimepy-4.3.0/runtimepy/tui/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/tui/cursor.py` & `runtimepy-4.3.0/runtimepy/tui/cursor.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/tui/mixin.py` & `runtimepy-4.3.0/runtimepy/tui/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/tui/mock.py` & `runtimepy-4.3.0/runtimepy/tui/mock.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/tui/task.py` & `runtimepy-4.3.0/runtimepy/tui/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy/util.py` & `runtimepy-4.3.0/runtimepy/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/runtimepy.egg-info/PKG-INFO` & `runtimepy-4.3.0/runtimepy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 4.2.2
+Version: 4.3.0
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -13,18 +13,18 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: psutil
+Requires-Dist: websockets
 Requires-Dist: vcorelib>=3.2.4
 Requires-Dist: svgen>=0.6.6
-Requires-Dist: websockets
+Requires-Dist: psutil
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
@@ -40,19 +40,19 @@
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: uvloop; (sys_platform != "win32" and sys_platform != "cygwin") and extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=5f56531d1be3002a8547ddb013d713f9
+    hash=2adcb8a8e9a6b4dffec41ec316de0fee
     =====================================
 -->
 
-# runtimepy ([4.2.2](https://pypi.org/project/runtimepy/))
+# runtimepy ([4.3.0](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-4.2.2/runtimepy.egg-info/SOURCES.txt` & `runtimepy-4.3.0/runtimepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/setup.py` & `runtimepy-4.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/tests/test_entry.py` & `runtimepy-4.3.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.2/tests/test_mapping.py` & `runtimepy-4.3.0/tests/test_mapping.py`

 * *Files identical despite different names*

