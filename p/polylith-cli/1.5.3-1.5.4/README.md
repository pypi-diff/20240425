# Comparing `tmp/polylith_cli-1.5.3.tar.gz` & `tmp/polylith_cli-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polylith_cli-1.5.3.tar", max compression
+gzip compressed data, was "polylith_cli-1.5.4.tar", max compression
```

## Comparing `polylith_cli-1.5.3.tar` & `polylith_cli-1.5.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0     4873 2024-01-31 09:30:45.173564 polylith_cli-1.5.3/README.md
--rw-r--r--   0        0        0       84 2024-04-11 15:29:40.258991 polylith_cli-1.5.3/polylith_cli/polylith/alias/__init__.py
--rw-r--r--   0        0        0      620 2023-12-23 14:50:24.864540 polylith_cli-1.5.3/polylith_cli/polylith/alias/core.py
--rw-r--r--   0        0        0      249 2024-04-11 15:29:40.253926 polylith_cli-1.5.3/polylith_cli/polylith/bricks/__init__.py
--rw-r--r--   0        0        0      576 2024-04-11 15:29:40.255033 polylith_cli-1.5.3/polylith_cli/polylith/bricks/base.py
--rw-r--r--   0        0        0      984 2024-04-11 15:29:40.255495 polylith_cli-1.5.3/polylith_cli/polylith/bricks/brick.py
--rw-r--r--   0        0        0     1108 2024-04-11 15:29:40.254503 polylith_cli-1.5.3/polylith_cli/polylith/bricks/component.py
--rw-r--r--   0        0        0      109 2024-04-11 15:29:40.284487 polylith_cli-1.5.3/polylith_cli/polylith/check/__init__.py
--rw-r--r--   0        0        0     1343 2024-04-11 15:29:40.283981 polylith_cli-1.5.3/polylith_cli/polylith/check/collect.py
--rw-r--r--   0        0        0     1051 2023-12-23 14:50:24.865756 polylith_cli-1.5.3/polylith_cli/polylith/check/grouping.py
--rw-r--r--   0        0        0     2809 2024-04-11 15:29:40.285378 polylith_cli-1.5.3/polylith_cli/polylith/check/report.py
--rw-r--r--   0        0        0       61 2024-04-11 15:29:40.265006 polylith_cli-1.5.3/polylith_cli/polylith/cli/__init__.py
--rw-r--r--   0        0        0       68 2024-04-11 15:29:40.266584 polylith_cli-1.5.3/polylith_cli/polylith/cli/__main__.py
--rw-r--r--   0        0        0     3956 2024-04-11 15:29:40.266392 polylith_cli-1.5.3/polylith_cli/polylith/cli/core.py
--rw-r--r--   0        0        0     2210 2024-04-11 15:29:40.264856 polylith_cli-1.5.3/polylith_cli/polylith/cli/create.py
--rw-r--r--   0        0        0      647 2024-03-15 17:10:28.637200 polylith_cli-1.5.3/polylith_cli/polylith/cli/options.py
--rw-r--r--   0        0        0      156 2024-04-11 15:29:40.278886 polylith_cli-1.5.3/polylith_cli/polylith/commands/__init__.py
--rw-r--r--   0        0        0     1196 2024-04-11 15:29:40.278437 polylith_cli-1.5.3/polylith_cli/polylith/commands/check.py
--rw-r--r--   0        0        0      645 2024-04-11 15:29:40.278729 polylith_cli-1.5.3/polylith_cli/polylith/commands/create.py
--rw-r--r--   0        0        0     1385 2024-04-11 15:29:40.277917 polylith_cli-1.5.3/polylith_cli/polylith/commands/deps.py
--rw-r--r--   0        0        0     1497 2024-04-11 15:29:40.279426 polylith_cli-1.5.3/polylith_cli/polylith/commands/diff.py
--rw-r--r--   0        0        0      679 2024-04-11 15:29:40.279749 polylith_cli-1.5.3/polylith_cli/polylith/commands/info.py
--rw-r--r--   0        0        0     1596 2024-04-11 15:29:40.280371 polylith_cli-1.5.3/polylith_cli/polylith/commands/libs.py
--rw-r--r--   0        0        0      628 2024-04-11 15:29:40.277282 polylith_cli-1.5.3/polylith_cli/polylith/commands/sync.py
--rw-r--r--   0        0        0      558 2024-04-11 15:29:40.255996 polylith_cli-1.5.3/polylith_cli/polylith/configuration/__init__.py
--rw-r--r--   0        0        0     2184 2024-04-11 15:29:40.256782 polylith_cli-1.5.3/polylith_cli/polylith/configuration/core.py
--rw-r--r--   0        0        0      202 2024-04-11 15:29:40.274689 polylith_cli-1.5.3/polylith_cli/polylith/deps/__init__.py
--rw-r--r--   0        0        0      681 2024-04-11 15:29:40.274993 polylith_cli-1.5.3/polylith_cli/polylith/deps/core.py
--rw-r--r--   0        0        0     4463 2024-04-11 15:29:40.276841 polylith_cli-1.5.3/polylith_cli/polylith/deps/report.py
--rw-r--r--   0        0        0      109 2024-04-11 15:29:40.259991 polylith_cli-1.5.3/polylith_cli/polylith/development/__init__.py
--rw-r--r--   0        0        0      234 2024-04-11 15:29:40.260166 polylith_cli-1.5.3/polylith_cli/polylith/development/development.py
--rw-r--r--   0        0        0       86 2024-04-11 15:29:40.262436 polylith_cli-1.5.3/polylith_cli/polylith/diff/__init__.py
--rw-r--r--   0        0        0     2245 2024-04-11 15:29:40.262241 polylith_cli-1.5.3/polylith_cli/polylith/diff/collect.py
--rw-r--r--   0        0        0     2141 2024-04-11 15:29:40.263256 polylith_cli-1.5.3/polylith_cli/polylith/diff/report.py
--rw-r--r--   0        0        0       79 2024-04-11 15:29:40.280777 polylith_cli-1.5.3/polylith_cli/polylith/dirs/__init__.py
--rw-r--r--   0        0        0      280 2024-04-11 15:29:40.280642 polylith_cli-1.5.3/polylith_cli/polylith/dirs/dirs.py
--rw-r--r--   0        0        0      339 2024-04-11 15:29:40.287309 polylith_cli-1.5.3/polylith_cli/polylith/distributions/__init__.py
--rw-r--r--   0        0        0     1016 2024-04-11 15:29:40.287141 polylith_cli-1.5.3/polylith_cli/polylith/distributions/collect.py
--rw-r--r--   0        0        0     1546 2024-01-16 12:33:20.028826 polylith_cli-1.5.3/polylith_cli/polylith/distributions/core.py
--rw-r--r--   0        0        0       83 2024-04-11 15:29:40.274494 polylith_cli-1.5.3/polylith_cli/polylith/files/__init__.py
--rw-r--r--   0        0        0      145 2024-01-20 10:21:41.138114 polylith_cli-1.5.3/polylith_cli/polylith/files/files.py
--rw-r--r--   0        0        0      162 2024-04-11 15:29:40.263489 polylith_cli-1.5.3/polylith_cli/polylith/imports/__init__.py
--rw-r--r--   0        0        0     1730 2024-04-07 19:33:48.496851 polylith_cli-1.5.3/polylith_cli/polylith/imports/parser.py
--rw-r--r--   0        0        0      475 2024-04-11 15:29:40.273012 polylith_cli-1.5.3/polylith_cli/polylith/info/__init__.py
--rw-r--r--   0        0        0     1630 2024-04-11 15:29:40.272832 polylith_cli-1.5.3/polylith_cli/polylith/info/collect.py
--rw-r--r--   0        0        0     3039 2024-04-11 15:29:40.274175 polylith_cli-1.5.3/polylith_cli/polylith/info/report.py
--rw-r--r--   0        0        0      102 2024-04-11 15:29:40.258828 polylith_cli-1.5.3/polylith_cli/polylith/interface/__init__.py
--rw-r--r--   0        0        0      875 2024-04-11 15:29:40.258689 polylith_cli-1.5.3/polylith_cli/polylith/interface/interfaces.py
--rw-r--r--   0        0        0      225 2024-04-11 15:29:40.267888 polylith_cli-1.5.3/polylith_cli/polylith/libs/__init__.py
--rw-r--r--   0        0        0     1396 2024-04-11 15:29:40.267736 polylith_cli-1.5.3/polylith_cli/polylith/libs/grouping.py
--rw-r--r--   0        0        0     5881 2024-04-11 15:29:40.270595 polylith_cli-1.5.3/polylith_cli/polylith/libs/report.py
--rw-r--r--   0        0        0     4408 2023-12-25 21:58:57.761499 polylith_cli-1.5.3/polylith_cli/polylith/libs/stdlib.py
--rw-r--r--   0        0        0      410 2024-04-11 15:29:40.271273 polylith_cli-1.5.3/polylith_cli/polylith/project/__init__.py
--rw-r--r--   0        0        0      852 2024-04-11 15:29:40.271100 polylith_cli-1.5.3/polylith_cli/polylith/project/create.py
--rw-r--r--   0        0        0     1458 2024-04-11 15:29:40.272110 polylith_cli-1.5.3/polylith_cli/polylith/project/get.py
--rw-r--r--   0        0        0      433 2023-12-23 14:50:24.872665 polylith_cli-1.5.3/polylith_cli/polylith/project/parser.py
--rw-r--r--   0        0        0      944 2024-01-30 17:47:45.368941 polylith_cli-1.5.3/polylith_cli/polylith/project/templates.py
--rw-r--r--   0        0        0      153 2024-04-11 15:29:40.267155 polylith_cli-1.5.3/polylith_cli/polylith/readme/__init__.py
--rw-r--r--   0        0        0     1091 2024-04-11 15:29:40.267015 polylith_cli-1.5.3/polylith_cli/polylith/readme/readme.py
--rw-r--r--   0        0        0      525 2024-04-11 15:29:40.285659 polylith_cli-1.5.3/polylith_cli/polylith/repo/__init__.py
--rw-r--r--   0        0        0      852 2024-04-11 15:29:40.286496 polylith_cli-1.5.3/polylith_cli/polylith/repo/get.py
--rw-r--r--   0        0        0     1964 2024-02-04 09:48:25.380602 polylith_cli-1.5.3/polylith_cli/polylith/repo/repo.py
--rw-r--r--   0        0        0       69 2024-04-11 15:29:40.255789 polylith_cli-1.5.3/polylith_cli/polylith/reporting/__init__.py
--rw-r--r--   0        0        0      208 2024-02-14 17:46:10.570719 polylith_cli-1.5.3/polylith_cli/polylith/reporting/theme.py
--rw-r--r--   0        0        0      225 2024-04-11 15:29:40.282905 polylith_cli-1.5.3/polylith_cli/polylith/sync/__init__.py
--rw-r--r--   0        0        0     1031 2024-04-11 15:29:40.282750 polylith_cli-1.5.3/polylith_cli/polylith/sync/collect.py
--rw-r--r--   0        0        0      983 2024-04-11 15:29:40.283377 polylith_cli-1.5.3/polylith_cli/polylith/sync/report.py
--rw-r--r--   0        0        0     3897 2024-04-11 15:29:40.282270 polylith_cli-1.5.3/polylith_cli/polylith/sync/update.py
--rw-r--r--   0        0        0       82 2024-04-11 15:29:40.259366 polylith_cli-1.5.3/polylith_cli/polylith/test/__init__.py
--rw-r--r--   0        0        0      965 2024-04-11 15:29:40.259801 polylith_cli-1.5.3/polylith_cli/polylith/test/tests.py
--rw-r--r--   0        0        0      457 2024-04-11 15:29:40.256994 polylith_cli-1.5.3/polylith_cli/polylith/toml/__init__.py
--rw-r--r--   0        0        0     2910 2024-04-11 15:29:40.258265 polylith_cli-1.5.3/polylith_cli/polylith/toml/core.py
--rw-r--r--   0        0        0       87 2024-04-11 15:29:40.261223 polylith_cli-1.5.3/polylith_cli/polylith/workspace/__init__.py
--rw-r--r--   0        0        0     1198 2024-04-11 15:29:40.260613 polylith_cli-1.5.3/polylith_cli/polylith/workspace/create.py
--rw-r--r--   0        0        0      937 2024-04-11 15:29:40.261084 polylith_cli-1.5.3/polylith_cli/polylith/workspace/paths.py
--rw-r--r--   0        0        0      605 2024-04-11 15:29:40.253399 polylith_cli-1.5.3/pyproject.toml
--rw-r--r--   0        0        0     5668 1970-01-01 00:00:00.000000 polylith_cli-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     4873 2024-02-09 08:50:51.459764 polylith_cli-1.5.4/README.md
+-rw-r--r--   0        0        0       84 2024-04-25 07:49:10.693931 polylith_cli-1.5.4/polylith_cli/polylith/alias/__init__.py
+-rw-r--r--   0        0        0      620 2024-01-16 09:46:59.989578 polylith_cli-1.5.4/polylith_cli/polylith/alias/core.py
+-rw-r--r--   0        0        0      249 2024-04-25 07:49:10.688415 polylith_cli-1.5.4/polylith_cli/polylith/bricks/__init__.py
+-rw-r--r--   0        0        0      576 2024-04-25 07:49:10.689487 polylith_cli-1.5.4/polylith_cli/polylith/bricks/base.py
+-rw-r--r--   0        0        0      986 2024-04-25 07:49:10.689977 polylith_cli-1.5.4/polylith_cli/polylith/bricks/brick.py
+-rw-r--r--   0        0        0     1108 2024-04-25 07:49:10.689144 polylith_cli-1.5.4/polylith_cli/polylith/bricks/component.py
+-rw-r--r--   0        0        0      109 2024-04-25 07:49:10.722700 polylith_cli-1.5.4/polylith_cli/polylith/check/__init__.py
+-rw-r--r--   0        0        0     1343 2024-04-25 07:49:10.722238 polylith_cli-1.5.4/polylith_cli/polylith/check/collect.py
+-rw-r--r--   0        0        0     1051 2023-03-13 14:27:27.458511 polylith_cli-1.5.4/polylith_cli/polylith/check/grouping.py
+-rw-r--r--   0        0        0     2811 2024-04-25 07:49:10.723790 polylith_cli-1.5.4/polylith_cli/polylith/check/report.py
+-rw-r--r--   0        0        0       61 2024-04-25 07:49:10.700404 polylith_cli-1.5.4/polylith_cli/polylith/cli/__init__.py
+-rw-r--r--   0        0        0       68 2024-04-25 07:49:10.702282 polylith_cli-1.5.4/polylith_cli/polylith/cli/__main__.py
+-rw-r--r--   0        0        0     3956 2024-04-25 07:49:10.702109 polylith_cli-1.5.4/polylith_cli/polylith/cli/core.py
+-rw-r--r--   0        0        0     2210 2024-04-25 07:49:10.700262 polylith_cli-1.5.4/polylith_cli/polylith/cli/create.py
+-rw-r--r--   0        0        0      647 2024-02-15 14:19:22.606210 polylith_cli-1.5.4/polylith_cli/polylith/cli/options.py
+-rw-r--r--   0        0        0      156 2024-04-25 07:49:10.716363 polylith_cli-1.5.4/polylith_cli/polylith/commands/__init__.py
+-rw-r--r--   0        0        0     1196 2024-04-25 07:49:10.715849 polylith_cli-1.5.4/polylith_cli/polylith/commands/check.py
+-rw-r--r--   0        0        0      645 2024-04-25 07:49:10.716199 polylith_cli-1.5.4/polylith_cli/polylith/commands/create.py
+-rw-r--r--   0        0        0     1385 2024-04-25 07:49:10.715292 polylith_cli-1.5.4/polylith_cli/polylith/commands/deps.py
+-rw-r--r--   0        0        0     1497 2024-04-25 07:49:10.717008 polylith_cli-1.5.4/polylith_cli/polylith/commands/diff.py
+-rw-r--r--   0        0        0      679 2024-04-25 07:49:10.717369 polylith_cli-1.5.4/polylith_cli/polylith/commands/info.py
+-rw-r--r--   0        0        0     1596 2024-04-25 07:49:10.718106 polylith_cli-1.5.4/polylith_cli/polylith/commands/libs.py
+-rw-r--r--   0        0        0      628 2024-04-25 07:49:10.714539 polylith_cli-1.5.4/polylith_cli/polylith/commands/sync.py
+-rw-r--r--   0        0        0      558 2024-04-25 07:49:10.690442 polylith_cli-1.5.4/polylith_cli/polylith/configuration/__init__.py
+-rw-r--r--   0        0        0     2184 2024-04-25 07:49:10.691482 polylith_cli-1.5.4/polylith_cli/polylith/configuration/core.py
+-rw-r--r--   0        0        0      202 2024-04-25 07:49:10.711454 polylith_cli-1.5.4/polylith_cli/polylith/deps/__init__.py
+-rw-r--r--   0        0        0      681 2024-04-25 07:49:10.711775 polylith_cli-1.5.4/polylith_cli/polylith/deps/core.py
+-rw-r--r--   0        0        0     4479 2024-04-25 07:49:10.714110 polylith_cli-1.5.4/polylith_cli/polylith/deps/report.py
+-rw-r--r--   0        0        0      109 2024-04-25 07:49:10.694907 polylith_cli-1.5.4/polylith_cli/polylith/development/__init__.py
+-rw-r--r--   0        0        0      234 2024-04-25 07:49:10.695084 polylith_cli-1.5.4/polylith_cli/polylith/development/development.py
+-rw-r--r--   0        0        0       86 2024-04-25 07:49:10.697599 polylith_cli-1.5.4/polylith_cli/polylith/diff/__init__.py
+-rw-r--r--   0        0        0     2247 2024-04-25 07:49:10.697450 polylith_cli-1.5.4/polylith_cli/polylith/diff/collect.py
+-rw-r--r--   0        0        0     2141 2024-04-25 07:49:10.698555 polylith_cli-1.5.4/polylith_cli/polylith/diff/report.py
+-rw-r--r--   0        0        0       79 2024-04-25 07:49:10.718509 polylith_cli-1.5.4/polylith_cli/polylith/dirs/__init__.py
+-rw-r--r--   0        0        0      280 2024-04-25 07:49:10.718385 polylith_cli-1.5.4/polylith_cli/polylith/dirs/dirs.py
+-rw-r--r--   0        0        0      339 2024-04-25 07:49:10.725850 polylith_cli-1.5.4/polylith_cli/polylith/distributions/__init__.py
+-rw-r--r--   0        0        0     1018 2024-04-25 07:49:10.725677 polylith_cli-1.5.4/polylith_cli/polylith/distributions/collect.py
+-rw-r--r--   0        0        0     1546 2024-01-22 14:07:16.217821 polylith_cli-1.5.4/polylith_cli/polylith/distributions/core.py
+-rw-r--r--   0        0        0       83 2024-04-25 07:49:10.711295 polylith_cli-1.5.4/polylith_cli/polylith/files/__init__.py
+-rw-r--r--   0        0        0      145 2022-11-04 07:17:35.623526 polylith_cli-1.5.4/polylith_cli/polylith/files/files.py
+-rw-r--r--   0        0        0      162 2024-04-25 07:49:10.698741 polylith_cli-1.5.4/polylith_cli/polylith/imports/__init__.py
+-rw-r--r--   0        0        0     1730 2023-07-29 11:51:13.392045 polylith_cli-1.5.4/polylith_cli/polylith/imports/parser.py
+-rw-r--r--   0        0        0      475 2024-04-25 07:49:10.709613 polylith_cli-1.5.4/polylith_cli/polylith/info/__init__.py
+-rw-r--r--   0        0        0     1632 2024-04-25 07:49:10.709425 polylith_cli-1.5.4/polylith_cli/polylith/info/collect.py
+-rw-r--r--   0        0        0     3039 2024-04-25 07:49:10.711035 polylith_cli-1.5.4/polylith_cli/polylith/info/report.py
+-rw-r--r--   0        0        0      102 2024-04-25 07:49:10.693764 polylith_cli-1.5.4/polylith_cli/polylith/interface/__init__.py
+-rw-r--r--   0        0        0      875 2024-04-25 07:49:10.693626 polylith_cli-1.5.4/polylith_cli/polylith/interface/interfaces.py
+-rw-r--r--   0        0        0      225 2024-04-25 07:49:10.703715 polylith_cli-1.5.4/polylith_cli/polylith/libs/__init__.py
+-rw-r--r--   0        0        0     1400 2024-04-25 07:49:10.703554 polylith_cli-1.5.4/polylith_cli/polylith/libs/grouping.py
+-rw-r--r--   0        0        0     5887 2024-04-25 07:49:10.706985 polylith_cli-1.5.4/polylith_cli/polylith/libs/report.py
+-rw-r--r--   0        0        0     4408 2024-01-16 08:29:38.285478 polylith_cli-1.5.4/polylith_cli/polylith/libs/stdlib.py
+-rw-r--r--   0        0        0      410 2024-04-25 07:49:10.707692 polylith_cli-1.5.4/polylith_cli/polylith/project/__init__.py
+-rw-r--r--   0        0        0      852 2024-04-25 07:49:10.707503 polylith_cli-1.5.4/polylith_cli/polylith/project/create.py
+-rw-r--r--   0        0        0     1458 2024-04-25 07:49:10.708626 polylith_cli-1.5.4/polylith_cli/polylith/project/get.py
+-rw-r--r--   0        0        0      433 2023-04-01 08:55:53.793395 polylith_cli-1.5.4/polylith_cli/polylith/project/parser.py
+-rw-r--r--   0        0        0      944 2024-02-09 08:50:51.449381 polylith_cli-1.5.4/polylith_cli/polylith/project/templates.py
+-rw-r--r--   0        0        0      153 2024-04-25 07:49:10.702898 polylith_cli-1.5.4/polylith_cli/polylith/readme/__init__.py
+-rw-r--r--   0        0        0     1091 2024-04-25 07:49:10.702750 polylith_cli-1.5.4/polylith_cli/polylith/readme/readme.py
+-rw-r--r--   0        0        0      525 2024-04-25 07:49:10.724038 polylith_cli-1.5.4/polylith_cli/polylith/repo/__init__.py
+-rw-r--r--   0        0        0      852 2024-04-25 07:49:10.725178 polylith_cli-1.5.4/polylith_cli/polylith/repo/get.py
+-rw-r--r--   0        0        0     1964 2024-02-09 08:50:51.451835 polylith_cli-1.5.4/polylith_cli/polylith/repo/repo.py
+-rw-r--r--   0        0        0       69 2024-04-25 07:49:10.690237 polylith_cli-1.5.4/polylith_cli/polylith/reporting/__init__.py
+-rw-r--r--   0        0        0      208 2024-02-15 14:02:37.811309 polylith_cli-1.5.4/polylith_cli/polylith/reporting/theme.py
+-rw-r--r--   0        0        0      225 2024-04-25 07:49:10.721000 polylith_cli-1.5.4/polylith_cli/polylith/sync/__init__.py
+-rw-r--r--   0        0        0     1031 2024-04-25 07:49:10.720834 polylith_cli-1.5.4/polylith_cli/polylith/sync/collect.py
+-rw-r--r--   0        0        0      983 2024-04-25 07:49:10.721536 polylith_cli-1.5.4/polylith_cli/polylith/sync/report.py
+-rw-r--r--   0        0        0     3901 2024-04-25 07:49:10.720315 polylith_cli-1.5.4/polylith_cli/polylith/sync/update.py
+-rw-r--r--   0        0        0       82 2024-04-25 07:49:10.694308 polylith_cli-1.5.4/polylith_cli/polylith/test/__init__.py
+-rw-r--r--   0        0        0      965 2024-04-25 07:49:10.694736 polylith_cli-1.5.4/polylith_cli/polylith/test/tests.py
+-rw-r--r--   0        0        0      457 2024-04-25 07:49:10.691697 polylith_cli-1.5.4/polylith_cli/polylith/toml/__init__.py
+-rw-r--r--   0        0        0     2918 2024-04-25 07:49:10.693161 polylith_cli-1.5.4/polylith_cli/polylith/toml/core.py
+-rw-r--r--   0        0        0       87 2024-04-25 07:49:10.696225 polylith_cli-1.5.4/polylith_cli/polylith/workspace/__init__.py
+-rw-r--r--   0        0        0     1198 2024-04-25 07:49:10.695553 polylith_cli-1.5.4/polylith_cli/polylith/workspace/create.py
+-rw-r--r--   0        0        0      937 2024-04-25 07:49:10.696082 polylith_cli-1.5.4/polylith_cli/polylith/workspace/paths.py
+-rw-r--r--   0        0        0      605 2024-04-25 07:49:10.687924 polylith_cli-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0     5668 1970-01-01 00:00:00.000000 polylith_cli-1.5.4/PKG-INFO
```

### Comparing `polylith_cli-1.5.3/README.md` & `polylith_cli-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/alias/core.py` & `polylith_cli-1.5.4/polylith_cli/polylith/alias/core.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/bricks/base.py` & `polylith_cli-1.5.4/polylith_cli/polylith/bricks/base.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/bricks/brick.py` & `polylith_cli-1.5.4/polylith_cli/polylith/bricks/brick.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from polylith_cli.polylith.dirs import create_dir
 from polylith_cli.polylith.files import create_file
 from polylith_cli.polylith.interface import create_interface
 from polylith_cli.polylith.readme import create_brick_readme
 
 def create_brick(root: Path, options: dict) -> None:
     modulename = options['modulename']
-    path_kwargs = {k: v for k, v in options.items() if k in {'brick', 'namespace', 'package'}}
+    path_kwargs = {k: v for (k, v) in options.items() if k in {'brick', 'namespace', 'package'}}
     brick_structure = configuration.get_brick_structure_from_config(root)
     resources_structure = configuration.get_resources_structure_from_config(root)
     brick_path = brick_structure.format(**path_kwargs)
     resources_path = resources_structure.format(**path_kwargs)
     d = create_dir(root, brick_path)
     create_file(d, f'{modulename}.py')
     create_interface(d, options)
```

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/bricks/component.py` & `polylith_cli-1.5.4/polylith_cli/polylith/bricks/component.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/check/collect.py` & `polylith_cli-1.5.4/polylith_cli/polylith/check/collect.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/check/grouping.py` & `polylith_cli-1.5.4/polylith_cli/polylith/check/grouping.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/check/report.py` & `polylith_cli-1.5.4/polylith_cli/polylith/check/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from rich.console import Console
 
 def print_brick_imports(brick_imports: dict) -> None:
     console = Console(theme=theme.poly_theme)
     bases = brick_imports['bases']
     components = brick_imports['components']
     bricks = {**bases, **components}
-    for key, values in bricks.items():
+    for (key, values) in bricks.items():
         imports_in_brick = values.difference({key})
         if not imports_in_brick:
             continue
         joined = ', '.join(imports_in_brick)
         message = f':information: [data]{key}[/] is importing [data]{joined}[/]'
         console.print(message)
```

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/cli/core.py` & `polylith_cli-1.5.4/polylith_cli/polylith/cli/core.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/cli/create.py` & `polylith_cli-1.5.4/polylith_cli/polylith/cli/create.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/cli/options.py` & `polylith_cli-1.5.4/polylith_cli/polylith/cli/options.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/commands/check.py` & `polylith_cli-1.5.4/polylith_cli/polylith/commands/check.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/commands/create.py` & `polylith_cli-1.5.4/polylith_cli/polylith/commands/create.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/commands/deps.py` & `polylith_cli-1.5.4/polylith_cli/polylith/commands/deps.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/commands/diff.py` & `polylith_cli-1.5.4/polylith_cli/polylith/commands/diff.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/commands/info.py` & `polylith_cli-1.5.4/polylith_cli/polylith/commands/info.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/commands/libs.py` & `polylith_cli-1.5.4/polylith_cli/polylith/commands/libs.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/commands/sync.py` & `polylith_cli-1.5.4/polylith_cli/polylith/commands/sync.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/configuration/__init__.py` & `polylith_cli-1.5.4/polylith_cli/polylith/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/configuration/core.py` & `polylith_cli-1.5.4/polylith_cli/polylith/configuration/core.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/deps/core.py` & `polylith_cli-1.5.4/polylith_cli/polylith/deps/core.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/deps/report.py` & `polylith_cli-1.5.4/polylith_cli/polylith/deps/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from rich.console import Console
 from rich.table import Table
 
 def to_col(brick: str, tag: str) -> str:
     name = '\n'.join(brick)
     return f'[{tag}]{name}[/]'
 
-def brick_status(bricks: List[str], brick_name: str, imported: str) -> str:
+def brick_status(bricks: Set[str], brick_name: str, imported: str) -> str:
     status = theme.check_emoji if imported in bricks and imported != brick_name else '-'
     return f'[data]{status}[/]'
 
 def to_row(name: str, tag: str, brick_imports: dict, imported: List[str]) -> List[str]:
-    bricks = brick_imports[name]
+    bricks = brick_imports.get(name) or set()
     statuses = [brick_status(bricks, name, i) for i in imported]
     return [f'[{tag}]{name}[/]'] + statuses
 
 def flatten_import(acc: Set[str], kv: Tuple[str, Set[str]]) -> set:
     key = kv[0]
     values = kv[1]
     return set().union(acc, values.difference({key}))
@@ -59,15 +59,15 @@
 
 def sorted_usings(usings: Set[str], bases: Set[str], components: Set[str]) -> List[str]:
     usings_bases = sorted({b for b in usings if b in bases})
     usings_components = sorted({c for c in usings if c in components})
     return usings_components + usings_bases
 
 def sorted_used_by(brick: str, bases: Set[str], components: Set[str], import_data: dict) -> List[str]:
-    brick_used_by = without(brick, {k for k, v in import_data.items() if brick in v})
+    brick_used_by = without(brick, {k for (k, v) in import_data.items() if brick in v})
     return sorted_usings(brick_used_by, bases, components)
 
 def sorted_uses(brick: str, bases: Set[str], components: Set[str], import_data: dict) -> List[str]:
     brick_uses = without(brick, {b for b in import_data[brick]})
     return sorted_usings(brick_uses, bases, components)
 
 def calculate_tag(brick: str, bases: Set[str]) -> str:
@@ -81,15 +81,15 @@
     table = Table(box=box.SIMPLE_HEAD)
     table.add_column('[data]used by[/]')
     table.add_column(':backhand_index_pointing_left:')
     table.add_column(f'[{tag}]{brick}[/]')
     table.add_column(':backhand_index_pointing_right:')
     table.add_column('[data]uses[/]')
     for item in zip_longest(brick_used_by, brick_uses):
-        used_by, uses = item
+        (used_by, uses) = item
         used_by_tag = calculate_tag(used_by, bases) if used_by else ''
         uses_tag = calculate_tag(uses, bases) if uses else ''
         left = f'[{used_by_tag}]{used_by}[/]' if used_by else ''
         right = f'[{uses_tag}]{uses}[/]' if uses else ''
         row = [left, '', '', '', right]
         table.add_row(*row)
     console.print(table, overflow='ellipsis')
```

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/diff/collect.py` & `polylith_cli-1.5.4/polylith_cli/polylith/diff/collect.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,14 @@
 
 def get_files(tag: str) -> List[Path]:
     res = subprocess.run(['git', 'diff', tag, '--stat', '--name-only'], capture_output=True)
     return [Path(p) for p in res.stdout.decode('utf-8').split()]
 
 def _affected(projects_data: List[dict], brick_type: str, bricks: List[str]) -> set:
     res = {p['path'].name: set(p.get(brick_type, [])).intersection(bricks) for p in projects_data}
-    return {k for k, v in res.items() if v}
+    return {k for (k, v) in res.items() if v}
 
 def get_projects_affected_by_changes(projects_data: List[dict], projects: List[str], bases: List[str], components: List[str]) -> Set[str]:
     a = _affected(projects_data, 'components', components)
     b = _affected(projects_data, 'bases', bases)
     c = set(projects)
     return {*a, *b, *c}
```

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/diff/report.py` & `polylith_cli-1.5.4/polylith_cli/polylith/diff/report.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/distributions/collect.py` & `polylith_cli-1.5.4/polylith_cli/polylith/distributions/collect.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def known_aliases_and_sub_dependencies(deps: dict, library_alias: list) -> Set[str]:
     """Collect known aliases (packages) for third-party libraries.
 
     When the library origin is not from a lock-file:
     collect sub-dependencies for each library, and append to the result.
     """
-    third_party_libs = {k for k, _v in deps['items'].items()}
+    third_party_libs = {k for (k, _v) in deps['items'].items()}
     lock_file = str.endswith(deps['source'], '.lock')
     dists = list(importlib.metadata.distributions())
     dist_packages = distributions_packages(dists)
     custom_aliases = alias.parse(library_alias)
     sub_deps = distributions_sub_packages(dists) if not lock_file else {}
     a = alias.pick(dist_packages, third_party_libs)
     b = alias.pick(custom_aliases, third_party_libs)
```

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/distributions/core.py` & `polylith_cli-1.5.4/polylith_cli/polylith/distributions/core.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/imports/parser.py` & `polylith_cli-1.5.4/polylith_cli/polylith/imports/parser.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/info/collect.py` & `polylith_cli-1.5.4/polylith_cli/polylith/info/collect.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,14 @@
     return [c['name'] for c in component.get_components_data(root, namespace)]
 
 def get_bases(root: Path, namespace: str) -> List[str]:
     return [b['name'] for b in base.get_bases_data(root, namespace)]
 
 def get_bricks_in_projects(root: Path, components: List[str], bases: List[str], namespace: str) -> List[dict]:
     packages_for_projects = get_packages_for_projects(root)
-    res = [{**{k: v for k, v in p.items() if k not in {'packages'}}, **get_project_bricks(p['packages'], components, bases, namespace)} for p in packages_for_projects]
+    res = [{**{k: v for (k, v) in p.items() if k not in {'packages'}}, **get_project_bricks(p['packages'], components, bases, namespace)} for p in packages_for_projects]
     return res
 
 def get_projects_data(root: Path, ns: str) -> List[dict]:
     bases = get_bases(root, ns)
     components = get_components(root, ns)
     return get_bricks_in_projects(root, components, bases, ns)
```

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/info/report.py` & `polylith_cli-1.5.4/polylith_cli/polylith/info/report.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/interface/interfaces.py` & `polylith_cli-1.5.4/polylith_cli/polylith/interface/interfaces.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/libs/grouping.py` & `polylith_cli-1.5.4/polylith_cli/polylith/libs/grouping.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,18 @@
     return values[-1]
 
 def get_standard_libs(python_version: str) -> Set[str]:
     libs = standard_libs.get(python_version)
     return libs or get_latest_standard_libs()
 
 def exclude_libs(import_data: dict, to_exclude: Set) -> dict:
-    return {k: v - to_exclude for k, v in import_data.items()}
+    return {k: v - to_exclude for (k, v) in import_data.items()}
 
 def exclude_empty(import_data: dict) -> dict:
-    return {k: v for k, v in import_data.items() if v}
+    return {k: v for (k, v) in import_data.items() if v}
 
 def extract_third_party_imports(all_imports: dict, top_ns: str) -> dict:
     python_version = get_python_version()
     std_libs = get_standard_libs(python_version)
     top_level_imports = extract_top_ns(all_imports)
     with_third_party = exclude_libs(top_level_imports, std_libs.union({top_ns}))
     return exclude_empty(with_third_party)
```

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/libs/report.py` & `polylith_cli-1.5.4/polylith_cli/polylith/libs/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,17 @@
         return
     console = Console(theme=theme.poly_theme)
     table = Table(box=box.SIMPLE_HEAD)
     bases = brick_imports.get('bases', {})
     components = brick_imports.get('components', {})
     table.add_column('[data]brick[/]')
     table.add_column('[data]library[/]')
-    for brick, imports in sorted(components.items(), key=itemgetter(0)):
+    for (brick, imports) in sorted(components.items(), key=itemgetter(0)):
         table.add_row(f'[comp]{brick}[/]', ', '.join(sorted(imports)))
-    for brick, imports in sorted(bases.items(), key=itemgetter(0)):
+    for (brick, imports) in sorted(bases.items(), key=itemgetter(0)):
         table.add_row(f'[base]{brick}[/]', ', '.join(sorted(imports)))
     console.print(table, overflow='ellipsis')
 
 def print_missing_installed_libs(brick_imports: dict, third_party_libs: Set[str], project_name: str, is_strict: bool=False) -> bool:
     diff = calculate_diff(brick_imports, third_party_libs, is_strict)
     if not diff:
         return True
@@ -107,14 +107,14 @@
         printable_proj_versions = [printable_version(v, is_same) for v in proj_versions]
         printable_dev_version = printable_version(dev_version, is_same)
         cols = [markup.escape(lib)] + printable_proj_versions + [printable_dev_version]
         table.add_row(*cols)
     return table
 
 def print_libs_in_projects(development_data: dict, projects_data: List[dict], options: dict) -> None:
-    flattened = {k for proj in projects_data for k, _v in proj['deps']['items'].items()}
+    flattened = {k for proj in projects_data for (k, _v) in proj['deps']['items'].items()}
     if not flattened:
         return
     table = libs_in_projects_table(development_data, projects_data, flattened, options)
     console = Console(theme=theme.poly_theme)
     console.print(Padding('[data]Library versions in projects[/]', (1, 0, 0, 0)))
     console.print(table, overflow='ellipsis')
```

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/libs/stdlib.py` & `polylith_cli-1.5.4/polylith_cli/polylith/libs/stdlib.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/project/create.py` & `polylith_cli-1.5.4/polylith_cli/polylith/project/create.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/project/get.py` & `polylith_cli-1.5.4/polylith_cli/polylith/project/get.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/project/templates.py` & `polylith_cli-1.5.4/polylith_cli/polylith/project/templates.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/readme/readme.py` & `polylith_cli-1.5.4/polylith_cli/polylith/readme/readme.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/repo/__init__.py` & `polylith_cli-1.5.4/polylith_cli/polylith/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/repo/get.py` & `polylith_cli-1.5.4/polylith_cli/polylith/repo/get.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/repo/repo.py` & `polylith_cli-1.5.4/polylith_cli/polylith/repo/repo.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/sync/collect.py` & `polylith_cli-1.5.4/polylith_cli/polylith/sync/collect.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/sync/report.py` & `polylith_cli-1.5.4/polylith_cli/polylith/sync/report.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/sync/update.py` & `polylith_cli-1.5.4/polylith_cli/polylith/sync/update.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,29 +24,29 @@
     copy = copy_toml_data(data)
     if not copy.get('tool'):
         copy['tool'] = {'polylith': {'bricks': {}}}
     if not copy['tool'].get('polylith'):
         copy['tool']['polylith'] = {'bricks': {}}
     if not copy['tool']['polylith'].get('bricks'):
         copy['tool']['polylith']['bricks'] = {}
-    for k, v in bricks_to_add.items():
+    for (k, v) in bricks_to_add.items():
         copy['tool']['polylith']['bricks'][k] = v
     return tomlkit.dumps(copy)
 
 def generate_updated_pdm_project(data: TOMLDocument, packages: List[dict]) -> str:
     bricks_to_add: dict = reduce(to_key_value_include, packages, {})
     return generate_updated_pep_621_project(data, bricks_to_add)
 
 def generate_updated_hatch_project(data: TOMLDocument, packages: List[dict]) -> str:
     bricks_to_add: dict = reduce(to_key_value_include, packages, {})
     has_polylith = data.get('tool', {}).get('polylith', {}).get('bricks')
     has_hatch = data.get('tool', {}).get('hatch', {}).get('build', {}).get('force-include')
     if not has_polylith and has_hatch:
         copy = copy_toml_data(data)
-        for k, v in bricks_to_add.items():
+        for (k, v) in bricks_to_add.items():
             copy['tool']['hatch']['build']['force-include'][k] = v
         return tomlkit.dumps(copy)
     return generate_updated_pep_621_project(data, bricks_to_add)
 
 def generate_updated_poetry_project(data: TOMLDocument, packages: List[dict]) -> str:
     copy = copy_toml_data(data)
     if copy['tool']['poetry'].get('packages') is None:
```

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/test/tests.py` & `polylith_cli-1.5.4/polylith_cli/polylith/test/tests.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/toml/core.py` & `polylith_cli-1.5.4/polylith_cli/polylith/toml/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from functools import reduce
 from pathlib import Path
 from typing import List, Union
 import tomlkit
 from polylith_cli.polylith import repo
 
 def transform_to_package(namespace: str, include: str) -> dict:
-    path, _separator, brick = str.partition(include, f'/{namespace}/')
+    (path, _separator, brick) = str.partition(include, f'/{namespace}/')
     return {'include': f'{namespace}/{brick}', 'from': path}
 
 def get_polylith_section(data) -> dict:
     return data.get('tool', {}).get('polylith', {})
 
 def get_custom_top_namespace_from_polylith_section(data) -> Union[str, None]:
     poly_data = get_polylith_section(data)
@@ -38,20 +38,20 @@
 def get_project_name(data) -> str:
     if repo.is_pep_621_ready(data):
         return data['project']['name']
     return data['tool']['poetry']['name']
 
 def parse_pep_621_dependency(dep: str) -> dict:
     parts = re.split('[\\^~=!<>]', dep)
-    name, *_ = parts if parts else ['']
+    (name, *_) = parts if parts else ['']
     version = str.replace(dep, name, '')
     return {name: version} if name else {}
 
 def parse_poetry_dependency(acc: dict, kv: tuple) -> dict:
-    k, v = kv
+    (k, v) = kv
     if isinstance(v, dict):
         extras = sorted(v.get('extras', []))
         version = v.get('version', '')
         name = k + str.replace(f'{extras}', "'", '') if extras else k
         parsed = {name: version}
     else:
         parsed = {k: v}
@@ -59,15 +59,15 @@
 
 def parse_project_dependencies(data) -> dict:
     if repo.is_poetry(data):
         deps = data['tool']['poetry'].get('dependencies', {})
         res: dict = reduce(parse_poetry_dependency, deps.items(), {})
         return res
     deps = data['project'].get('dependencies', [])
-    return {k: v for dep in deps for k, v in parse_pep_621_dependency(dep).items()}
+    return {k: v for dep in deps for (k, v) in parse_pep_621_dependency(dep).items()}
 
 def get_project_dependencies(data) -> dict:
     items = parse_project_dependencies(data)
     return {'items': items, 'source': repo.default_toml}
 
 def read_toml_document(path: Path) -> tomlkit.TOMLDocument:
     with path.open(encoding='utf-8', errors='ignore') as f:
```

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/workspace/create.py` & `polylith_cli-1.5.4/polylith_cli/polylith/workspace/create.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/polylith_cli/polylith/workspace/paths.py` & `polylith_cli-1.5.4/polylith_cli/polylith/workspace/paths.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.3/pyproject.toml` & `polylith_cli-1.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polylith-cli"
-version = "1.5.3"
+version = "1.5.4"
 description = "Python tooling support for the Polylith Architecture"
 authors = ['David Vujic']
 homepage = "https://davidvujic.github.io/python-polylith-docs/"
 repository = "https://github.com/davidvujic/python-polylith"
 license = "MIT"
 readme = "README.md"
```

### Comparing `polylith_cli-1.5.3/PKG-INFO` & `polylith_cli-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polylith-cli
-Version: 1.5.3
+Version: 1.5.4
 Summary: Python tooling support for the Polylith Architecture
 Home-page: https://davidvujic.github.io/python-polylith-docs/
 License: MIT
 Author: David Vujic
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

