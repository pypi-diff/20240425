# Comparing `tmp/platformio-6.1.8.tar.gz` & `tmp/platformio-6.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platformio-6.1.8.tar", last modified: Wed Jul  5 12:47:07 2023, max compression
+gzip compressed data, was "platformio-6.1.9.tar", last modified: Thu Jul  6 11:52:12 2023, max compression
```

## Comparing `platformio-6.1.8.tar` & `platformio-6.1.9.tar`

### file list

```diff
@@ -1,363 +1,363 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.234894 platformio-6.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-07-05 12:32:56.000000 platformio-6.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-05 12:47:07.234894 platformio-6.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-05 12:32:56.000000 platformio-6.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.130888 platformio-6.1.8/platformio/
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.134889 platformio-6.1.8/platformio/account/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.138889 platformio-6.1.8/platformio/account/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/commands/destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/commands/forgot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/commands/logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/commands/password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/commands/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/commands/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/commands/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/commands/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.138889 platformio-6.1.8/platformio/account/org/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/org/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/org/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.142889 platformio-6.1.8/platformio/account/org/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/org/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/org/commands/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/org/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/org/commands/destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/org/commands/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/org/commands/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/org/commands/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.142889 platformio-6.1.8/platformio/account/team/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/team/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/team/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.146889 platformio-6.1.8/platformio/account/team/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/team/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/team/commands/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/team/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/team/commands/destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/team/commands/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/team/commands/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/team/commands/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.118888 platformio-6.1.8/platformio/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.146889 platformio-6.1.8/platformio/assets/system/
--rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/assets/system/99-platformio-udev.rules
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.146889 platformio-6.1.8/platformio/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.154890 platformio-6.1.8/platformio/builder/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/pioasm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12663 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/piobuild.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/piohooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/pioino.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/piointegration.py
--rw-r--r--   0 runner    (1001) docker     (123)    42536 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/piolib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/piomaxlen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/piomisc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/pioplatform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/pioproject.py
--rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/piosize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/piotarget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/piotest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/pioupload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.158890 platformio-6.1.8/platformio/check/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/check/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/check/defect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.158890 platformio-6.1.8/platformio/check/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/check/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/check/tools/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/check/tools/clangtidy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/check/tools/cppcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/check/tools/pvsstudio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.162890 platformio-6.1.8/platformio/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/commands/boards.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/commands/ci.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.162890 platformio-6.1.8/platformio/commands/device/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/commands/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16025 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/commands/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/commands/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/commands/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/commands/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/commands/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.166890 platformio-6.1.8/platformio/debug/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.166890 platformio-6.1.8/platformio/debug/config/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/config/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/config/blackmagic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/config/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/config/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/config/jlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/config/mspdebug.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/config/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/config/qemu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/config/renode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.170891 platformio-6.1.8/platformio/debug/process/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/process/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/process/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/process/gdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/process/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.170891 platformio-6.1.8/platformio/device/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.170891 platformio-6.1.8/platformio/device/list/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/list/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/list/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.170891 platformio-6.1.8/platformio/device/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/monitor/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.174891 platformio-6.1.8/platformio/device/monitor/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/monitor/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/monitor/filters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/monitor/filters/hexlify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/monitor/filters/log2file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/monitor/filters/send_on_enter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/monitor/filters/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/monitor/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.174891 platformio-6.1.8/platformio/home/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.174891 platformio-6.1.8/platformio/home/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.178891 platformio-6.1.8/platformio/home/rpc/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/handlers/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/handlers/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/handlers/ide.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/handlers/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/handlers/os.py
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/handlers/piocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/handlers/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)    13217 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/handlers/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/handlers/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/maintenance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.182891 platformio-6.1.8/platformio/package/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.186891 platformio-6.1.8/platformio/package/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/outdated.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/publish.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/uninstall.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/unpublish.py
--rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/lockfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.190892 platformio-6.1.8/platformio/package/manager/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/_install.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/_symlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/_uninstall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.190892 platformio-6.1.8/platformio/package/manifest/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24640 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manifest/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manifest/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    16117 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/unpack.py
--rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/vcsclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.194892 platformio-6.1.8/platformio/platform/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/platform/_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/platform/_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/platform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/platform/board.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/platform/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/platform/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/proc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.198892 platformio-6.1.8/platformio/project/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.198892 platformio-6.1.8/platformio/project/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12843 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/commands/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/commands/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.198892 platformio-6.1.8/platformio/project/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.122888 platformio-6.1.8/platformio/project/integration/tpls/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.198892 platformio-6.1.8/platformio/project/integration/tpls/clion/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/clion/.gitignore.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/clion/CMakeLists.txt.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/clion/CMakeListsPrivate.txt.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.198892 platformio-6.1.8/platformio/project/integration/tpls/codeblocks/
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/codeblocks/platformio.cbp.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.202892 platformio-6.1.8/platformio/project/integration/tpls/eclipse/
--rw-r--r--   0 runner    (1001) docker     (123)    20663 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/eclipse/.cproject.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/eclipse/.project.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.202892 platformio-6.1.8/platformio/project/integration/tpls/eclipse/.settings/
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/eclipse/.settings/PlatformIO Debugger.launch.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/eclipse/.settings/language.settings.xml.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/eclipse/.settings/org.eclipse.cdt.core.prefs.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.202892 platformio-6.1.8/platformio/project/integration/tpls/emacs/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/emacs/.ccls.tpl
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/emacs/.gitignore.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.122888 platformio-6.1.8/platformio/project/integration/tpls/netbeans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.202892 platformio-6.1.8/platformio/project/integration/tpls/netbeans/nbproject/
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/netbeans/nbproject/configurations.xml.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.202892 platformio-6.1.8/platformio/project/integration/tpls/netbeans/nbproject/private/
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/netbeans/nbproject/private/configurations.xml.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/netbeans/nbproject/private/launcher.properties.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/netbeans/nbproject/private/private.xml.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/netbeans/nbproject/project.xml.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.206893 platformio-6.1.8/platformio/project/integration/tpls/qtcreator/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/qtcreator/.gitignore.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/qtcreator/Makefile.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/qtcreator/platformio.cflags.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/qtcreator/platformio.config.tpl
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/qtcreator/platformio.creator.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/qtcreator/platformio.cxxflags.tpl
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/qtcreator/platformio.files.tpl
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/qtcreator/platformio.includes.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.210893 platformio-6.1.8/platformio/project/integration/tpls/sublimetext/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/sublimetext/.ccls.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/sublimetext/platformio.sublime-project.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.210893 platformio-6.1.8/platformio/project/integration/tpls/vim/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/vim/.ccls.tpl
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/vim/.gitignore.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.210893 platformio-6.1.8/platformio/project/integration/tpls/visualstudio/
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/visualstudio/platformio.vcxproj.filters.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/visualstudio/platformio.vcxproj.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.210893 platformio-6.1.8/platformio/project/integration/tpls/vscode/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/vscode/.gitignore.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.210893 platformio-6.1.8/platformio/project/integration/tpls/vscode/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/vscode/.vscode/c_cpp_properties.json.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/vscode/.vscode/extensions.json.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/vscode/.vscode/launch.json.tpl
--rw-r--r--   0 runner    (1001) docker     (123)    31475 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/savedeps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/public.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.210893 platformio-6.1.8/platformio/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.214893 platformio-6.1.8/platformio/registry/access/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/access/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.214893 platformio-6.1.8/platformio/registry/access/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/access/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/access/commands/grant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/access/commands/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/access/commands/private.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/access/commands/public.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/access/commands/revoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/access/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/mirror.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.214893 platformio-6.1.8/platformio/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.214893 platformio-6.1.8/platformio/remote/ac/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/ac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/ac/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/ac/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/ac/psync.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/ac/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.218893 platformio-6.1.8/platformio/remote/client/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/client/agent_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/client/agent_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/client/async_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/client/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/client/device_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/client/device_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/client/run_or_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/client/update_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.218893 platformio-6.1.8/platformio/remote/factory/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/factory/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/factory/ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/projectsync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.222894 platformio-6.1.8/platformio/run/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9788 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/run/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/run/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/run/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.222894 platformio-6.1.8/platformio/system/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/system/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.222894 platformio-6.1.8/platformio/system/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/system/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/system/commands/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/system/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/system/commands/prune.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/system/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/system/prune.py
--rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/telemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.226894 platformio-6.1.8/platformio/test/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.230894 platformio-6.1.8/platformio/test/reports/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/reports/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/reports/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/reports/junit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/reports/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.230894 platformio-6.1.8/platformio/test/runners/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/runners/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/runners/doctest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/runners/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/runners/googletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.234894 platformio-6.1.8/platformio/test/runners/readers/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/runners/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/runners/readers/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/runners/readers/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/runners/unity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.134889 platformio-6.1.8/platformio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-05 12:47:07.000000 platformio-6.1.8/platformio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-07-05 12:47:07.000000 platformio-6.1.8/platformio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 12:47:07.000000 platformio-6.1.8/platformio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-05 12:47:07.000000 platformio-6.1.8/platformio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-05 12:47:07.000000 platformio-6.1.8/platformio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 12:47:07.000000 platformio-6.1.8/platformio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 12:47:07.234894 platformio-6.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-05 12:32:57.000000 platformio-6.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.234894 platformio-6.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-05 12:32:57.000000 platformio-6.1.8/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.238586 platformio-6.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-07-06 11:38:35.000000 platformio-6.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-06 11:52:12.238586 platformio-6.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-06 11:38:35.000000 platformio-6.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.150580 platformio-6.1.9/platformio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.154580 platformio-6.1.9/platformio/account/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.158580 platformio-6.1.9/platformio/account/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/commands/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/commands/forgot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/commands/logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/commands/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/commands/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/commands/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/commands/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/commands/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.158580 platformio-6.1.9/platformio/account/org/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/org/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/org/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.162581 platformio-6.1.9/platformio/account/org/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/org/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/org/commands/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/org/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/org/commands/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/org/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/org/commands/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/org/commands/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.162581 platformio-6.1.9/platformio/account/team/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/team/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/team/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.162581 platformio-6.1.9/platformio/account/team/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/team/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/team/commands/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/team/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/team/commands/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/team/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/team/commands/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/team/commands/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/account/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.134579 platformio-6.1.9/platformio/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.162581 platformio-6.1.9/platformio/assets/system/
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/assets/system/99-platformio-udev.rules
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.166581 platformio-6.1.9/platformio/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/builder/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.170581 platformio-6.1.9/platformio/builder/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/builder/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/builder/tools/pioasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/builder/tools/piobuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/builder/tools/piohooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/builder/tools/pioino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/builder/tools/piointegration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42536 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/builder/tools/piolib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/builder/tools/piomaxlen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/builder/tools/piomisc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/builder/tools/pioplatform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/builder/tools/pioproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/builder/tools/piosize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/builder/tools/piotarget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/builder/tools/piotest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/builder/tools/pioupload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.170581 platformio-6.1.9/platformio/check/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/check/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/check/defect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.174581 platformio-6.1.9/platformio/check/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/check/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/check/tools/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/check/tools/clangtidy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/check/tools/cppcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/check/tools/pvsstudio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.174581 platformio-6.1.9/platformio/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/commands/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/commands/ci.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.174581 platformio-6.1.9/platformio/commands/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/commands/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16025 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/commands/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/commands/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/commands/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/commands/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/commands/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.174581 platformio-6.1.9/platformio/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/debug/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.178582 platformio-6.1.9/platformio/debug/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/debug/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/debug/config/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/debug/config/blackmagic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/debug/config/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/debug/config/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/debug/config/jlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/debug/config/mspdebug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/debug/config/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/debug/config/qemu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/debug/config/renode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/debug/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/debug/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.178582 platformio-6.1.9/platformio/debug/process/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/debug/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/debug/process/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/debug/process/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/debug/process/gdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/debug/process/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.182582 platformio-6.1.9/platformio/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/device/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/device/finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.182582 platformio-6.1.9/platformio/device/list/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/device/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/device/list/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/device/list/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.182582 platformio-6.1.9/platformio/device/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/device/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/device/monitor/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.186582 platformio-6.1.9/platformio/device/monitor/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/device/monitor/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/device/monitor/filters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/device/monitor/filters/hexlify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/device/monitor/filters/log2file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/device/monitor/filters/send_on_enter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/device/monitor/filters/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/device/monitor/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.186582 platformio-6.1.9/platformio/home/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/home/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/home/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.186582 platformio-6.1.9/platformio/home/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/home/rpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.186582 platformio-6.1.9/platformio/home/rpc/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/home/rpc/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/home/rpc/handlers/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/home/rpc/handlers/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/home/rpc/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/home/rpc/handlers/ide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/home/rpc/handlers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/home/rpc/handlers/os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/home/rpc/handlers/piocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/home/rpc/handlers/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13217 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/home/rpc/handlers/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/home/rpc/handlers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/home/rpc/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/home/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/maintenance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.190582 platformio-6.1.9/platformio/package/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.194583 platformio-6.1.9/platformio/package/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/commands/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/commands/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/commands/outdated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/commands/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/commands/publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/commands/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/commands/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/commands/uninstall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/commands/unpublish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/commands/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/lockfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.198583 platformio-6.1.9/platformio/package/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/manager/_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/manager/_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/manager/_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/manager/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/manager/_symlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/manager/_uninstall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/manager/_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/manager/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/manager/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/manager/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/manager/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.198583 platformio-6.1.9/platformio/package/manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24640 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/manifest/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/manifest/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16117 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/unpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/vcsclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/package/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.202583 platformio-6.1.9/platformio/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/platform/_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/platform/_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/platform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/platform/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/platform/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/platform/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/proc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.202583 platformio-6.1.9/platformio/project/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.206584 platformio-6.1.9/platformio/project/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12843 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/commands/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.206584 platformio-6.1.9/platformio/project/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.142579 platformio-6.1.9/platformio/project/integration/tpls/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.206584 platformio-6.1.9/platformio/project/integration/tpls/clion/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/clion/.gitignore.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/clion/CMakeLists.txt.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/clion/CMakeListsPrivate.txt.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.206584 platformio-6.1.9/platformio/project/integration/tpls/codeblocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/codeblocks/platformio.cbp.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.206584 platformio-6.1.9/platformio/project/integration/tpls/eclipse/
+-rw-r--r--   0 runner    (1001) docker     (123)    20663 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/eclipse/.cproject.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/eclipse/.project.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.206584 platformio-6.1.9/platformio/project/integration/tpls/eclipse/.settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/eclipse/.settings/PlatformIO Debugger.launch.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/eclipse/.settings/language.settings.xml.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/eclipse/.settings/org.eclipse.cdt.core.prefs.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.210584 platformio-6.1.9/platformio/project/integration/tpls/emacs/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/emacs/.ccls.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/emacs/.gitignore.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.142579 platformio-6.1.9/platformio/project/integration/tpls/netbeans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.210584 platformio-6.1.9/platformio/project/integration/tpls/netbeans/nbproject/
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/netbeans/nbproject/configurations.xml.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.210584 platformio-6.1.9/platformio/project/integration/tpls/netbeans/nbproject/private/
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/netbeans/nbproject/private/configurations.xml.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/netbeans/nbproject/private/launcher.properties.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/netbeans/nbproject/private/private.xml.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/netbeans/nbproject/project.xml.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.214584 platformio-6.1.9/platformio/project/integration/tpls/qtcreator/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/qtcreator/.gitignore.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/qtcreator/Makefile.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/qtcreator/platformio.cflags.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/qtcreator/platformio.config.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/qtcreator/platformio.creator.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/qtcreator/platformio.cxxflags.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/qtcreator/platformio.files.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/qtcreator/platformio.includes.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.214584 platformio-6.1.9/platformio/project/integration/tpls/sublimetext/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/sublimetext/.ccls.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/sublimetext/platformio.sublime-project.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.214584 platformio-6.1.9/platformio/project/integration/tpls/vim/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/vim/.ccls.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/vim/.gitignore.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.214584 platformio-6.1.9/platformio/project/integration/tpls/visualstudio/
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/visualstudio/platformio.vcxproj.filters.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/visualstudio/platformio.vcxproj.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.214584 platformio-6.1.9/platformio/project/integration/tpls/vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/vscode/.gitignore.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.214584 platformio-6.1.9/platformio/project/integration/tpls/vscode/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/vscode/.vscode/c_cpp_properties.json.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/vscode/.vscode/extensions.json.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/integration/tpls/vscode/.vscode/launch.json.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)    31475 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/project/savedeps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/public.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.214584 platformio-6.1.9/platformio/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.218584 platformio-6.1.9/platformio/registry/access/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/registry/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/registry/access/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.218584 platformio-6.1.9/platformio/registry/access/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/registry/access/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/registry/access/commands/grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/registry/access/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/registry/access/commands/private.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/registry/access/commands/public.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/registry/access/commands/revoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/registry/access/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/registry/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/registry/mirror.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.218584 platformio-6.1.9/platformio/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/remote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.222585 platformio-6.1.9/platformio/remote/ac/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/remote/ac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/remote/ac/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/remote/ac/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/remote/ac/psync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/remote/ac/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/remote/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.226585 platformio-6.1.9/platformio/remote/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/remote/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/remote/client/agent_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/remote/client/agent_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/remote/client/async_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/remote/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/remote/client/device_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/remote/client/device_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/remote/client/run_or_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/remote/client/update_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.226585 platformio-6.1.9/platformio/remote/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/remote/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/remote/factory/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/remote/factory/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/remote/projectsync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.230585 platformio-6.1.9/platformio/run/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9788 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/run/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/run/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/run/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.230585 platformio-6.1.9/platformio/system/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/system/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.230585 platformio-6.1.9/platformio/system/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/system/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/system/commands/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/system/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/system/commands/prune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/system/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/system/prune.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.234585 platformio-6.1.9/platformio/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/test/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/test/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/test/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.234585 platformio-6.1.9/platformio/test/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/test/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/test/reports/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/test/reports/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/test/reports/junit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/test/reports/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/test/result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.238586 platformio-6.1.9/platformio/test/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/test/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/test/runners/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/test/runners/doctest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/test/runners/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/test/runners/googletest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.238586 platformio-6.1.9/platformio/test/runners/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/test/runners/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/test/runners/readers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/test/runners/readers/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/test/runners/unity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-06 11:38:35.000000 platformio-6.1.9/platformio/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.154580 platformio-6.1.9/platformio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-06 11:52:12.000000 platformio-6.1.9/platformio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-07-06 11:52:12.000000 platformio-6.1.9/platformio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:52:12.000000 platformio-6.1.9/platformio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-06 11:52:12.000000 platformio-6.1.9/platformio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-06 11:52:12.000000 platformio-6.1.9/platformio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 11:52:12.000000 platformio-6.1.9/platformio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 11:52:12.238586 platformio-6.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-06 11:38:35.000000 platformio-6.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:12.238586 platformio-6.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-06 11:38:35.000000 platformio-6.1.9/tests/test_examples.py
```

### Comparing `platformio-6.1.8/LICENSE` & `platformio-6.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/PKG-INFO` & `platformio-6.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platformio
-Version: 6.1.8
+Version: 6.1.9
 Summary: A professional collaborative platform for embedded development. Cross-platform IDE and Unified Debugger. Static Code Analyzer and Remote Unit Testing. Multi-platform and Multi-architecture Build System. Firmware File Explorer and Memory Inspection. IoT, Arduino, CMSIS, ESP-IDF, FreeRTOS, libOpenCM3, mbedOS, Pulp OS, SPL, STM32Cube, Zephyr RTOS, ARM, AVR, Espressif (ESP8266/ESP32), FPGA, MCS-51 (8051), MSP430, Nordic (nRF51/nRF52), NXP i.MX RT, PIC32, RISC-V, STMicroelectronics (STM8/STM32), Teensy
 Home-page: https://platformio.org
 Author: PlatformIO Labs
 Author-email: contact@piolabs.com
 License: Apache Software License
 Keywords: iot,embedded,arduino,mbed,esp8266,esp32,fpga,firmware,continuous-integration,cloud-ide,avr,arm,ide,unit-testing,hardware,verilog,microcontroller,debug
 Platform: UNKNOWN
```

### Comparing `platformio-6.1.8/README.rst` & `platformio-6.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/__init__.py` & `platformio-6.1.9/platformio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-VERSION = (6, 1, 8)
+VERSION = (6, 1, 9)
 __version__ = ".".join([str(s) for s in VERSION])
 
 __title__ = "platformio"
 __description__ = (
     "A professional collaborative platform for embedded development. "
     "Cross-platform IDE and Unified Debugger. "
     "Static Code Analyzer and Remote Unit Testing. "
```

### Comparing `platformio-6.1.8/platformio/__main__.py` & `platformio-6.1.9/platformio/__main__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/__init__.py` & `platformio-6.1.9/platformio/account/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/cli.py` & `platformio-6.1.9/platformio/account/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/client.py` & `platformio-6.1.9/platformio/account/client.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/commands/__init__.py` & `platformio-6.1.9/platformio/account/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/commands/destroy.py` & `platformio-6.1.9/platformio/account/commands/destroy.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/commands/forgot.py` & `platformio-6.1.9/platformio/account/commands/forgot.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/commands/login.py` & `platformio-6.1.9/platformio/account/commands/login.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/commands/logout.py` & `platformio-6.1.9/platformio/account/commands/logout.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/commands/password.py` & `platformio-6.1.9/platformio/account/commands/password.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/commands/register.py` & `platformio-6.1.9/platformio/account/commands/register.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/commands/show.py` & `platformio-6.1.9/platformio/account/commands/show.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/commands/token.py` & `platformio-6.1.9/platformio/account/commands/token.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/commands/update.py` & `platformio-6.1.9/platformio/account/commands/update.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/org/__init__.py` & `platformio-6.1.9/platformio/account/org/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/org/cli.py` & `platformio-6.1.9/platformio/account/org/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/org/commands/__init__.py` & `platformio-6.1.9/platformio/account/org/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/org/commands/add.py` & `platformio-6.1.9/platformio/account/org/commands/add.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/org/commands/create.py` & `platformio-6.1.9/platformio/account/org/commands/create.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/org/commands/destroy.py` & `platformio-6.1.9/platformio/account/org/commands/destroy.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/org/commands/list.py` & `platformio-6.1.9/platformio/account/org/commands/list.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/org/commands/remove.py` & `platformio-6.1.9/platformio/account/org/commands/remove.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/org/commands/update.py` & `platformio-6.1.9/platformio/account/org/commands/update.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/team/__init__.py` & `platformio-6.1.9/platformio/account/team/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/team/cli.py` & `platformio-6.1.9/platformio/account/team/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/team/commands/__init__.py` & `platformio-6.1.9/platformio/account/team/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/team/commands/add.py` & `platformio-6.1.9/platformio/account/team/commands/add.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/team/commands/create.py` & `platformio-6.1.9/platformio/account/team/commands/create.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/team/commands/destroy.py` & `platformio-6.1.9/platformio/account/team/commands/destroy.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/team/commands/list.py` & `platformio-6.1.9/platformio/account/team/commands/list.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/team/commands/remove.py` & `platformio-6.1.9/platformio/account/team/commands/remove.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/team/commands/update.py` & `platformio-6.1.9/platformio/account/team/commands/update.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/account/validate.py` & `platformio-6.1.9/platformio/account/validate.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/app.py` & `platformio-6.1.9/platformio/app.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/assets/system/99-platformio-udev.rules` & `platformio-6.1.9/platformio/assets/system/99-platformio-udev.rules`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/builder/__init__.py` & `platformio-6.1.9/platformio/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/builder/main.py` & `platformio-6.1.9/platformio/builder/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from SCons.Script import Default  # pylint: disable=import-error
 from SCons.Script import DefaultEnvironment  # pylint: disable=import-error
 from SCons.Script import Import  # pylint: disable=import-error
 from SCons.Script import Variables  # pylint: disable=import-error
 
 from platformio import app, fs
 from platformio.platform.base import PlatformBase
-from platformio.proc import get_pythonexe_path, where_is_program
+from platformio.proc import get_pythonexe_path
 from platformio.project.helpers import get_project_dir
 
 AllowSubstExceptions(NameError)
 
 # append CLI arguments to build environment
 clivars = Variables(None)
 clivars.AddVariables(
@@ -191,21 +191,14 @@
     # Replace platform's "size" target with our
     _new_targets = [t for t in DEFAULT_TARGETS if str(t) != "size"]
     Default(None)
     Default(_new_targets)
     Default("checkprogsize")
 
 if "compiledb" in COMMAND_LINE_TARGETS:
-    # Resolve absolute path of toolchain
-    for cmd in ("CC", "CXX", "AS"):
-        if cmd not in env:
-            continue
-        if os.path.isabs(env[cmd]):
-            continue
-        env[cmd] = where_is_program(env.subst("$%s" % cmd), env.subst("${ENV['PATH']}"))
     env.Alias("compiledb", env.CompilationDatabase("$COMPILATIONDB_PATH"))
 
 # Print configured protocols
 env.AddPreAction(
     "upload",
     env.VerboseAction(
         lambda source, target, env: env.PrintUploadInfo(),
```

### Comparing `platformio-6.1.8/platformio/builder/tools/__init__.py` & `platformio-6.1.9/platformio/builder/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/builder/tools/pioasm.py` & `platformio-6.1.9/platformio/builder/tools/pioasm.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/builder/tools/piobuild.py` & `platformio-6.1.9/platformio/builder/tools/piobuild.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from SCons.Script import AlwaysBuild  # pylint: disable=import-error
 from SCons.Script import DefaultEnvironment  # pylint: disable=import-error
 from SCons.Script import SConscript  # pylint: disable=import-error
 
 from platformio import __version__, fs
 from platformio.compat import IS_MACOS, string_types
 from platformio.package.version import pepver_to_semver
+from platformio.proc import where_is_program
 
 SRC_HEADER_EXT = ["h", "hpp"]
 SRC_ASM_EXT = ["S", "spp", "SPP", "sx", "s", "asm", "ASM"]
 SRC_C_EXT = ["c"]
 SRC_CXX_EXT = ["cc", "cpp", "cxx", "c++"]
 SRC_BUILD_EXT = SRC_C_EXT + SRC_CXX_EXT + SRC_ASM_EXT
 SRC_FILTER_DEFAULT = ["+<*>", "-<.git%s>" % os.sep, "-<.svn%s>" % os.sep]
@@ -121,20 +122,29 @@
 
     if "debug" in env["BUILD_TYPE"]:
         env.ConfigureDebugTarget()
 
     # remove specified flags
     env.ProcessUnFlags(env.get("BUILD_UNFLAGS"))
 
-    if "compiledb" in COMMAND_LINE_TARGETS and env.get(
-        "COMPILATIONDB_INCLUDE_TOOLCHAIN"
-    ):
-        for scope, includes in env.DumpIntegrationIncludes().items():
-            if scope in ("toolchain",):
-                env.Append(CPPPATH=includes)
+    if "compiledb" in COMMAND_LINE_TARGETS:
+        # Resolve absolute path of toolchain
+        for cmd in ("CC", "CXX", "AS"):
+            if cmd not in env:
+                continue
+            if os.path.isabs(env[cmd]):
+                continue
+            env[cmd] = where_is_program(
+                env.subst("$%s" % cmd), env.subst("${ENV['PATH']}")
+            )
+
+        if env.get("COMPILATIONDB_INCLUDE_TOOLCHAIN"):
+            for scope, includes in env.DumpIntegrationIncludes().items():
+                if scope in ("toolchain",):
+                    env.Append(CPPPATH=includes)
 
 
 def ProcessProjectDeps(env):
     plb = env.ConfigureProjectLibBuilder()
 
     # prepend project libs to the beginning of list
     env.Prepend(LIBS=plb.build())
@@ -203,17 +213,15 @@
             p = env.subst(p)
             if os.path.isdir(p):
                 result[k][i] = os.path.abspath(p)
 
     # fix relative path for "-include"
     for i, f in enumerate(result.get("CCFLAGS", [])):
         if isinstance(f, tuple) and f[0] == "-include":
-            p = env.subst(f[1].get_path())
-            if os.path.exists(p):
-                result["CCFLAGS"][i] = (f[0], os.path.abspath(p))
+            result["CCFLAGS"][i] = (f[0], env.subst(f[1].get_path()))
 
     return result
 
 
 def ProcessFlags(env, flags):  # pylint: disable=too-many-branches
     if not flags:
         return
```

### Comparing `platformio-6.1.8/platformio/builder/tools/piohooks.py` & `platformio-6.1.9/platformio/builder/tools/piohooks.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/builder/tools/pioino.py` & `platformio-6.1.9/platformio/builder/tools/pioino.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/builder/tools/piointegration.py` & `platformio-6.1.9/platformio/builder/tools/piointegration.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/builder/tools/piolib.py` & `platformio-6.1.9/platformio/builder/tools/piolib.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/builder/tools/piomaxlen.py` & `platformio-6.1.9/platformio/builder/tools/piomaxlen.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/builder/tools/piomisc.py` & `platformio-6.1.9/platformio/builder/tools/piomisc.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/builder/tools/pioplatform.py` & `platformio-6.1.9/platformio/builder/tools/pioplatform.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/builder/tools/pioproject.py` & `platformio-6.1.9/platformio/builder/tools/pioproject.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/builder/tools/piosize.py` & `platformio-6.1.9/platformio/builder/tools/piosize.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/builder/tools/piotarget.py` & `platformio-6.1.9/platformio/builder/tools/piotarget.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/builder/tools/piotest.py` & `platformio-6.1.9/platformio/builder/tools/piotest.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/builder/tools/pioupload.py` & `platformio-6.1.9/platformio/builder/tools/pioupload.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/cache.py` & `platformio-6.1.9/platformio/cache.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/check/__init__.py` & `platformio-6.1.9/platformio/check/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/check/cli.py` & `platformio-6.1.9/platformio/check/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/check/defect.py` & `platformio-6.1.9/platformio/check/defect.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/check/tools/__init__.py` & `platformio-6.1.9/platformio/check/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/check/tools/base.py` & `platformio-6.1.9/platformio/check/tools/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/check/tools/clangtidy.py` & `platformio-6.1.9/platformio/check/tools/clangtidy.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/check/tools/cppcheck.py` & `platformio-6.1.9/platformio/check/tools/cppcheck.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/check/tools/pvsstudio.py` & `platformio-6.1.9/platformio/check/tools/pvsstudio.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/cli.py` & `platformio-6.1.9/platformio/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/commands/__init__.py` & `platformio-6.1.9/platformio/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/commands/boards.py` & `platformio-6.1.9/platformio/commands/boards.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/commands/ci.py` & `platformio-6.1.9/platformio/commands/ci.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/commands/device/__init__.py` & `platformio-6.1.9/platformio/commands/device/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/commands/lib.py` & `platformio-6.1.9/platformio/commands/lib.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/commands/platform.py` & `platformio-6.1.9/platformio/commands/platform.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/commands/settings.py` & `platformio-6.1.9/platformio/commands/settings.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/commands/update.py` & `platformio-6.1.9/platformio/commands/update.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/commands/upgrade.py` & `platformio-6.1.9/platformio/commands/upgrade.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/compat.py` & `platformio-6.1.9/platformio/compat.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/debug/__init__.py` & `platformio-6.1.9/platformio/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/debug/cli.py` & `platformio-6.1.9/platformio/debug/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/debug/config/__init__.py` & `platformio-6.1.9/platformio/debug/config/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/debug/config/base.py` & `platformio-6.1.9/platformio/debug/config/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/debug/config/blackmagic.py` & `platformio-6.1.9/platformio/debug/config/blackmagic.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/debug/config/factory.py` & `platformio-6.1.9/platformio/debug/config/factory.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/debug/config/generic.py` & `platformio-6.1.9/platformio/debug/config/generic.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/debug/config/jlink.py` & `platformio-6.1.9/platformio/debug/config/jlink.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/debug/config/mspdebug.py` & `platformio-6.1.9/platformio/debug/config/mspdebug.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/debug/config/native.py` & `platformio-6.1.9/platformio/debug/config/native.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/debug/config/qemu.py` & `platformio-6.1.9/platformio/debug/config/qemu.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/debug/config/renode.py` & `platformio-6.1.9/platformio/debug/config/renode.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/debug/exception.py` & `platformio-6.1.9/platformio/debug/exception.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/debug/helpers.py` & `platformio-6.1.9/platformio/debug/helpers.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/debug/process/__init__.py` & `platformio-6.1.9/platformio/debug/process/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/debug/process/base.py` & `platformio-6.1.9/platformio/debug/process/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/debug/process/client.py` & `platformio-6.1.9/platformio/debug/process/client.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/debug/process/gdb.py` & `platformio-6.1.9/platformio/debug/process/gdb.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/debug/process/server.py` & `platformio-6.1.9/platformio/debug/process/server.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/device/__init__.py` & `platformio-6.1.9/platformio/device/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/device/cli.py` & `platformio-6.1.9/platformio/device/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/device/finder.py` & `platformio-6.1.9/platformio/device/finder.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/device/list/__init__.py` & `platformio-6.1.9/platformio/device/list/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/device/list/command.py` & `platformio-6.1.9/platformio/device/list/command.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/device/list/util.py` & `platformio-6.1.9/platformio/device/list/util.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/device/monitor/__init__.py` & `platformio-6.1.9/platformio/device/monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/device/monitor/command.py` & `platformio-6.1.9/platformio/device/monitor/command.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/device/monitor/filters/__init__.py` & `platformio-6.1.9/platformio/device/monitor/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/device/monitor/filters/base.py` & `platformio-6.1.9/platformio/device/monitor/filters/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/device/monitor/filters/hexlify.py` & `platformio-6.1.9/platformio/device/monitor/filters/hexlify.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/device/monitor/filters/log2file.py` & `platformio-6.1.9/platformio/device/monitor/filters/log2file.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/device/monitor/filters/send_on_enter.py` & `platformio-6.1.9/platformio/device/monitor/filters/send_on_enter.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/device/monitor/filters/time.py` & `platformio-6.1.9/platformio/device/monitor/filters/time.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/device/monitor/terminal.py` & `platformio-6.1.9/platformio/device/monitor/terminal.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/exception.py` & `platformio-6.1.9/platformio/exception.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/fs.py` & `platformio-6.1.9/platformio/fs.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/home/__init__.py` & `platformio-6.1.9/platformio/home/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/home/cli.py` & `platformio-6.1.9/platformio/home/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/home/rpc/__init__.py` & `platformio-6.1.9/platformio/home/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/home/rpc/handlers/__init__.py` & `platformio-6.1.9/platformio/home/rpc/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/home/rpc/handlers/account.py` & `platformio-6.1.9/platformio/home/rpc/handlers/account.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/home/rpc/handlers/app.py` & `platformio-6.1.9/platformio/home/rpc/handlers/app.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/home/rpc/handlers/base.py` & `platformio-6.1.9/platformio/home/rpc/handlers/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/home/rpc/handlers/ide.py` & `platformio-6.1.9/platformio/home/rpc/handlers/ide.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/home/rpc/handlers/misc.py` & `platformio-6.1.9/platformio/home/rpc/handlers/misc.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/home/rpc/handlers/os.py` & `platformio-6.1.9/platformio/home/rpc/handlers/os.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/home/rpc/handlers/piocore.py` & `platformio-6.1.9/platformio/home/rpc/handlers/piocore.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/home/rpc/handlers/platform.py` & `platformio-6.1.9/platformio/home/rpc/handlers/platform.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/home/rpc/handlers/project.py` & `platformio-6.1.9/platformio/home/rpc/handlers/project.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/home/rpc/handlers/registry.py` & `platformio-6.1.9/platformio/home/rpc/handlers/registry.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/home/rpc/server.py` & `platformio-6.1.9/platformio/home/rpc/server.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/home/run.py` & `platformio-6.1.9/platformio/home/run.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/http.py` & `platformio-6.1.9/platformio/http.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/maintenance.py` & `platformio-6.1.9/platformio/maintenance.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/__init__.py` & `platformio-6.1.9/platformio/package/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/cli.py` & `platformio-6.1.9/platformio/package/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/commands/__init__.py` & `platformio-6.1.9/platformio/package/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/commands/exec.py` & `platformio-6.1.9/platformio/package/commands/exec.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/commands/install.py` & `platformio-6.1.9/platformio/package/commands/install.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/commands/list.py` & `platformio-6.1.9/platformio/package/commands/list.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/commands/outdated.py` & `platformio-6.1.9/platformio/package/commands/outdated.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/commands/pack.py` & `platformio-6.1.9/platformio/package/commands/pack.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/commands/publish.py` & `platformio-6.1.9/platformio/package/commands/publish.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/commands/search.py` & `platformio-6.1.9/platformio/package/commands/search.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/commands/show.py` & `platformio-6.1.9/platformio/package/commands/show.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/commands/uninstall.py` & `platformio-6.1.9/platformio/package/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/commands/unpublish.py` & `platformio-6.1.9/platformio/package/commands/unpublish.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/commands/update.py` & `platformio-6.1.9/platformio/package/commands/update.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/download.py` & `platformio-6.1.9/platformio/package/download.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/exception.py` & `platformio-6.1.9/platformio/package/exception.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/lockfile.py` & `platformio-6.1.9/platformio/package/lockfile.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/manager/__init__.py` & `platformio-6.1.9/platformio/package/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/manager/_download.py` & `platformio-6.1.9/platformio/package/manager/_download.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/manager/_install.py` & `platformio-6.1.9/platformio/package/manager/_install.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/manager/_legacy.py` & `platformio-6.1.9/platformio/package/manager/_legacy.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/manager/_registry.py` & `platformio-6.1.9/platformio/package/manager/_registry.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/manager/_symlink.py` & `platformio-6.1.9/platformio/package/manager/_symlink.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/manager/_uninstall.py` & `platformio-6.1.9/platformio/package/manager/_uninstall.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/manager/_update.py` & `platformio-6.1.9/platformio/package/manager/_update.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/manager/base.py` & `platformio-6.1.9/platformio/package/manager/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/manager/core.py` & `platformio-6.1.9/platformio/package/manager/core.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/manager/library.py` & `platformio-6.1.9/platformio/package/manager/library.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/manager/platform.py` & `platformio-6.1.9/platformio/package/manager/platform.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/manager/tool.py` & `platformio-6.1.9/platformio/package/manager/tool.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/manifest/__init__.py` & `platformio-6.1.9/platformio/package/manifest/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/manifest/parser.py` & `platformio-6.1.9/platformio/package/manifest/parser.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/manifest/schema.py` & `platformio-6.1.9/platformio/package/manifest/schema.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/meta.py` & `platformio-6.1.9/platformio/package/meta.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/pack.py` & `platformio-6.1.9/platformio/package/pack.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/unpack.py` & `platformio-6.1.9/platformio/package/unpack.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/vcsclient.py` & `platformio-6.1.9/platformio/package/vcsclient.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/package/version.py` & `platformio-6.1.9/platformio/package/version.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/platform/__init__.py` & `platformio-6.1.9/platformio/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/platform/_packages.py` & `platformio-6.1.9/platformio/platform/_packages.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/platform/_run.py` & `platformio-6.1.9/platformio/platform/_run.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/platform/base.py` & `platformio-6.1.9/platformio/platform/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/platform/board.py` & `platformio-6.1.9/platformio/platform/board.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/platform/exception.py` & `platformio-6.1.9/platformio/platform/exception.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/platform/factory.py` & `platformio-6.1.9/platformio/platform/factory.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/proc.py` & `platformio-6.1.9/platformio/proc.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/__init__.py` & `platformio-6.1.9/platformio/project/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/cli.py` & `platformio-6.1.9/platformio/project/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/commands/__init__.py` & `platformio-6.1.9/platformio/project/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/commands/config.py` & `platformio-6.1.9/platformio/project/commands/config.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/commands/init.py` & `platformio-6.1.9/platformio/project/commands/init.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/commands/metadata.py` & `platformio-6.1.9/platformio/project/commands/metadata.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/config.py` & `platformio-6.1.9/platformio/project/config.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/exception.py` & `platformio-6.1.9/platformio/project/exception.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/helpers.py` & `platformio-6.1.9/platformio/project/helpers.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/integration/__init__.py` & `platformio-6.1.9/platformio/project/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/integration/generator.py` & `platformio-6.1.9/platformio/project/integration/generator.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/integration/tpls/clion/CMakeLists.txt.tpl` & `platformio-6.1.9/platformio/project/integration/tpls/clion/CMakeLists.txt.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/integration/tpls/clion/CMakeListsPrivate.txt.tpl` & `platformio-6.1.9/platformio/project/integration/tpls/clion/CMakeListsPrivate.txt.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/integration/tpls/codeblocks/platformio.cbp.tpl` & `platformio-6.1.9/platformio/project/integration/tpls/codeblocks/platformio.cbp.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/integration/tpls/eclipse/.cproject.tpl` & `platformio-6.1.9/platformio/project/integration/tpls/eclipse/.cproject.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/integration/tpls/eclipse/.project.tpl` & `platformio-6.1.9/platformio/project/integration/tpls/eclipse/.project.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/integration/tpls/eclipse/.settings/PlatformIO Debugger.launch.tpl` & `platformio-6.1.9/platformio/project/integration/tpls/eclipse/.settings/PlatformIO Debugger.launch.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/integration/tpls/eclipse/.settings/language.settings.xml.tpl` & `platformio-6.1.9/platformio/project/integration/tpls/eclipse/.settings/language.settings.xml.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/integration/tpls/eclipse/.settings/org.eclipse.cdt.core.prefs.tpl` & `platformio-6.1.9/platformio/project/integration/tpls/eclipse/.settings/org.eclipse.cdt.core.prefs.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/integration/tpls/netbeans/nbproject/configurations.xml.tpl` & `platformio-6.1.9/platformio/project/integration/tpls/netbeans/nbproject/configurations.xml.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/integration/tpls/netbeans/nbproject/private/configurations.xml.tpl` & `platformio-6.1.9/platformio/project/integration/tpls/netbeans/nbproject/private/configurations.xml.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/integration/tpls/netbeans/nbproject/private/launcher.properties.tpl` & `platformio-6.1.9/platformio/project/integration/tpls/netbeans/nbproject/private/launcher.properties.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/integration/tpls/netbeans/nbproject/project.xml.tpl` & `platformio-6.1.9/platformio/project/integration/tpls/netbeans/nbproject/project.xml.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/integration/tpls/sublimetext/platformio.sublime-project.tpl` & `platformio-6.1.9/platformio/project/integration/tpls/sublimetext/platformio.sublime-project.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/integration/tpls/visualstudio/platformio.vcxproj.filters.tpl` & `platformio-6.1.9/platformio/project/integration/tpls/visualstudio/platformio.vcxproj.filters.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/integration/tpls/visualstudio/platformio.vcxproj.tpl` & `platformio-6.1.9/platformio/project/integration/tpls/visualstudio/platformio.vcxproj.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/integration/tpls/vscode/.vscode/c_cpp_properties.json.tpl` & `platformio-6.1.9/platformio/project/integration/tpls/vscode/.vscode/c_cpp_properties.json.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/integration/tpls/vscode/.vscode/extensions.json.tpl` & `platformio-6.1.9/platformio/project/integration/tpls/vscode/.vscode/extensions.json.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/integration/tpls/vscode/.vscode/launch.json.tpl` & `platformio-6.1.9/platformio/project/integration/tpls/vscode/.vscode/launch.json.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/options.py` & `platformio-6.1.9/platformio/project/options.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/project/savedeps.py` & `platformio-6.1.9/platformio/project/savedeps.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/public.py` & `platformio-6.1.9/platformio/public.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/registry/__init__.py` & `platformio-6.1.9/platformio/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/registry/access/__init__.py` & `platformio-6.1.9/platformio/registry/access/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/registry/access/cli.py` & `platformio-6.1.9/platformio/registry/access/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/registry/access/commands/__init__.py` & `platformio-6.1.9/platformio/registry/access/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/registry/access/commands/grant.py` & `platformio-6.1.9/platformio/registry/access/commands/grant.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/registry/access/commands/list.py` & `platformio-6.1.9/platformio/registry/access/commands/list.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/registry/access/commands/private.py` & `platformio-6.1.9/platformio/registry/access/commands/private.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/registry/access/commands/public.py` & `platformio-6.1.9/platformio/registry/access/commands/public.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/registry/access/commands/revoke.py` & `platformio-6.1.9/platformio/registry/access/commands/revoke.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/registry/access/validate.py` & `platformio-6.1.9/platformio/registry/access/validate.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/registry/client.py` & `platformio-6.1.9/platformio/registry/client.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/registry/mirror.py` & `platformio-6.1.9/platformio/registry/mirror.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/remote/__init__.py` & `platformio-6.1.9/platformio/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/remote/ac/__init__.py` & `platformio-6.1.9/platformio/remote/ac/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/remote/ac/base.py` & `platformio-6.1.9/platformio/remote/ac/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/remote/ac/process.py` & `platformio-6.1.9/platformio/remote/ac/process.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/remote/ac/psync.py` & `platformio-6.1.9/platformio/remote/ac/psync.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/remote/ac/serial.py` & `platformio-6.1.9/platformio/remote/ac/serial.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/remote/cli.py` & `platformio-6.1.9/platformio/remote/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/remote/client/__init__.py` & `platformio-6.1.9/platformio/remote/client/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/remote/client/agent_list.py` & `platformio-6.1.9/platformio/remote/client/agent_list.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/remote/client/agent_service.py` & `platformio-6.1.9/platformio/remote/client/agent_service.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/remote/client/async_base.py` & `platformio-6.1.9/platformio/remote/client/async_base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/remote/client/base.py` & `platformio-6.1.9/platformio/remote/client/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/remote/client/device_list.py` & `platformio-6.1.9/platformio/remote/client/device_list.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/remote/client/device_monitor.py` & `platformio-6.1.9/platformio/remote/client/device_monitor.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/remote/client/run_or_test.py` & `platformio-6.1.9/platformio/remote/client/run_or_test.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/remote/client/update_core.py` & `platformio-6.1.9/platformio/remote/client/update_core.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/remote/factory/__init__.py` & `platformio-6.1.9/platformio/remote/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/remote/factory/client.py` & `platformio-6.1.9/platformio/remote/factory/client.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/remote/factory/ssl.py` & `platformio-6.1.9/platformio/remote/factory/ssl.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/remote/projectsync.py` & `platformio-6.1.9/platformio/remote/projectsync.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/run/__init__.py` & `platformio-6.1.9/platformio/run/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/run/cli.py` & `platformio-6.1.9/platformio/run/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/run/helpers.py` & `platformio-6.1.9/platformio/run/helpers.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/run/processor.py` & `platformio-6.1.9/platformio/run/processor.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/system/__init__.py` & `platformio-6.1.9/platformio/system/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/system/cli.py` & `platformio-6.1.9/platformio/system/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/system/commands/__init__.py` & `platformio-6.1.9/platformio/system/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/system/commands/completion.py` & `platformio-6.1.9/platformio/system/commands/completion.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/system/commands/info.py` & `platformio-6.1.9/platformio/system/commands/info.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/system/commands/prune.py` & `platformio-6.1.9/platformio/system/commands/prune.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/system/completion.py` & `platformio-6.1.9/platformio/system/completion.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/system/prune.py` & `platformio-6.1.9/platformio/system/prune.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/telemetry.py` & `platformio-6.1.9/platformio/telemetry.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/test/__init__.py` & `platformio-6.1.9/platformio/test/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/test/cli.py` & `platformio-6.1.9/platformio/test/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/test/exception.py` & `platformio-6.1.9/platformio/test/exception.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/test/helpers.py` & `platformio-6.1.9/platformio/test/helpers.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/test/reports/__init__.py` & `platformio-6.1.9/platformio/test/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/test/reports/base.py` & `platformio-6.1.9/platformio/test/reports/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/test/reports/json.py` & `platformio-6.1.9/platformio/test/reports/json.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/test/reports/junit.py` & `platformio-6.1.9/platformio/test/reports/junit.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/test/reports/stdout.py` & `platformio-6.1.9/platformio/test/reports/stdout.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/test/result.py` & `platformio-6.1.9/platformio/test/result.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/test/runners/__init__.py` & `platformio-6.1.9/platformio/test/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/test/runners/base.py` & `platformio-6.1.9/platformio/test/runners/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/test/runners/doctest.py` & `platformio-6.1.9/platformio/test/runners/doctest.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/test/runners/factory.py` & `platformio-6.1.9/platformio/test/runners/factory.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/test/runners/googletest.py` & `platformio-6.1.9/platformio/test/runners/googletest.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/test/runners/readers/__init__.py` & `platformio-6.1.9/platformio/test/runners/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/test/runners/readers/native.py` & `platformio-6.1.9/platformio/test/runners/readers/native.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/test/runners/readers/serial.py` & `platformio-6.1.9/platformio/test/runners/readers/serial.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/test/runners/unity.py` & `platformio-6.1.9/platformio/test/runners/unity.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio/util.py` & `platformio-6.1.9/platformio/util.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/platformio.egg-info/PKG-INFO` & `platformio-6.1.9/platformio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platformio
-Version: 6.1.8
+Version: 6.1.9
 Summary: A professional collaborative platform for embedded development. Cross-platform IDE and Unified Debugger. Static Code Analyzer and Remote Unit Testing. Multi-platform and Multi-architecture Build System. Firmware File Explorer and Memory Inspection. IoT, Arduino, CMSIS, ESP-IDF, FreeRTOS, libOpenCM3, mbedOS, Pulp OS, SPL, STM32Cube, Zephyr RTOS, ARM, AVR, Espressif (ESP8266/ESP32), FPGA, MCS-51 (8051), MSP430, Nordic (nRF51/nRF52), NXP i.MX RT, PIC32, RISC-V, STMicroelectronics (STM8/STM32), Teensy
 Home-page: https://platformio.org
 Author: PlatformIO Labs
 Author-email: contact@piolabs.com
 License: Apache Software License
 Keywords: iot,embedded,arduino,mbed,esp8266,esp32,fpga,firmware,continuous-integration,cloud-ide,avr,arm,ide,unit-testing,hardware,verilog,microcontroller,debug
 Platform: UNKNOWN
```

### Comparing `platformio-6.1.8/platformio.egg-info/SOURCES.txt` & `platformio-6.1.9/platformio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/setup.py` & `platformio-6.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.8/tests/test_examples.py` & `platformio-6.1.9/tests/test_examples.py`

 * *Files identical despite different names*

