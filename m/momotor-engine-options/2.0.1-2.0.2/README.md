# Comparing `tmp/momotor_engine_options-2.0.1.tar.gz` & `tmp/momotor_engine_options-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momotor_engine_options-2.0.1.tar", last modified: Tue Apr 16 07:31:38 2024, max compression
+gzip compressed data, was "momotor_engine_options-2.0.2.tar", last modified: Thu Apr 25 07:11:24 2024, max compression
```

## Comparing `momotor_engine_options-2.0.1.tar` & `momotor_engine_options-2.0.2.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     1215 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     3220 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/.idea/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/.idea/inspectionProfiles/
--rw-rw-rw-   0 root         (0) root         (0)      779 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-rw-rw-   0 root         (0) root         (0)      174 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0 root         (0) root         (0)      296 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/.idea/modules.xml
--rw-rw-rw-   0 root         (0) root         (0)      566 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/.idea/momotor.lib.engine-options.iml
--rw-rw-rw-   0 root         (0) root         (0)      238 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/.idea/workspace.xml
--rw-rw-rw-   0 root         (0) root         (0)    17342 2024-04-16 07:31:33.000000 momotor_engine_options-2.0.1/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     2658 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      778 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      764 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/docs/source/_static/
--rw-rw-rw-   0 root         (0) root         (0)     6988 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/_static/logo-text-negative.png
--rw-rw-rw-   0 root         (0) root         (0)     6887 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/_static/logo-text.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/docs/source/_templates/
--rw-rw-rw-   0 root         (0) root         (0)      672 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/_templates/projectlinks.html
--rw-rw-rw-   0 root         (0) root         (0)     4647 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/dependencies.rst
--rw-rw-rw-   0 root         (0) root         (0)      161 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/exceptions.rst
--rw-rw-rw-   0 root         (0) root         (0)      583 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/option.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/docs/source/options/
--rw-rw-rw-   0 root         (0) root         (0)      516 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/options/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      411 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/options/scheduler.rst
--rw-rw-rw-   0 root         (0) root         (0)      895 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/options/tools.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/docs/source/parser/
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/parser/index.rst
--rw-rw-rw-   0 root         (0) root         (0)    31565 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/parser/syntax.rst
--rw-rw-rw-   0 root         (0) root         (0)      134 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/providers.rst
--rw-rw-rw-   0 root         (0) root         (0)     6992 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/registry.rst
--rw-rw-rw-   0 root         (0) root         (0)    11618 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/result_query.rst
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/task_id.rst
--rw-rw-rw-   0 root         (0) root         (0)      618 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/utilities.rst
--rw-rw-rw-   0 root         (0) root         (0)      436 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/publish-docs.sh
--rw-rw-rw-   0 root         (0) root         (0)     2673 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      413 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/semver.sh
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor/options/
--rw-rw-rw-   0 root         (0) root         (0)      120 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7428 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/convert.py
--rw-rw-rw-   0 root         (0) root         (0)     8438 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/dependencies.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/doc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor/options/domain/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/domain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor/options/domain/scheduler/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/domain/scheduler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/domain/scheduler/_domain.py
--rw-rw-rw-   0 root         (0) root         (0)    11580 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/domain/scheduler/preflight.py
--rw-rw-rw-   0 root         (0) root         (0)     8274 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/domain/scheduler/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     4367 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/domain/scheduler/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor/options/domain/tools/
--rw-rw-rw-   0 root         (0) root         (0)     6226 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/domain/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/domain/tools/_domain.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/exception.py
--rw-rw-rw-   0 root         (0) root         (0)     1723 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/filter_files.py
--rw-rw-rw-   0 root         (0) root         (0)    13396 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/option.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor/options/parser/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/parser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1996 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/parser/consts.py
--rw-rw-rw-   0 root         (0) root         (0)     3581 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/parser/keyvalue.py
--rw-rw-rw-   0 root         (0) root         (0)     4151 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/parser/modifier.py
--rw-rw-rw-   0 root         (0) root         (0)     2103 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/parser/placeholders.py
--rw-rw-rw-   0 root         (0) root         (0)    24967 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/parser/reference.py
--rw-rw-rw-   0 root         (0) root         (0)     8335 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/parser/selector.py
--rw-rw-rw-   0 root         (0) root         (0)     1710 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/parser/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     1055 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/providers.py
--rw-rw-rw-   0 root         (0) root         (0)     6490 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/result_query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor/options/sphinx/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/sphinx/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2555 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/sphinx/fixextref.py
--rw-rw-rw-   0 root         (0) root         (0)    16823 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/sphinx/option.py
--rw-rw-rw-   0 root         (0) root         (0)     1461 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/split.py
--rw-rw-rw-   0 root         (0) root         (0)     9202 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/task_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor/options/tools/
--rw-rw-rw-   0 root         (0) root         (0)      919 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6312 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/tools/registry.py
--rw-rw-rw-   0 root         (0) root         (0)    12546 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/tools/tool.py
--rw-rw-rw-   0 root         (0) root         (0)      507 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/tools/types.py
--rw-rw-rw-   0 root         (0) root         (0)     6103 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/tools/version.py
--rw-rw-rw-   0 root         (0) root         (0)      776 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor_engine_options.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2658 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor_engine_options.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3296 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor_engine_options.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor_engine_options.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      360 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor_engine_options.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor_engine_options.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     7508 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/test_option_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     4365 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/test_parser_modifier.py
--rw-rw-rw-   0 root         (0) root         (0)     6167 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/test_parser_placeholders.py
--rw-rw-rw-   0 root         (0) root         (0)     9529 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/test_parser_reference.py
--rw-rw-rw-   0 root         (0) root         (0)     8543 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/test_parser_selector.py
--rw-rw-rw-   0 root         (0) root         (0)     8110 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/test_utils_dependencies.py
--rw-rw-rw-   0 root         (0) root         (0)     9006 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/test_utils_tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/tests/tools/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/tests/tools/files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/nodefault/
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/nodefault/1
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/nodefault/2.1
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/nodefault/named
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/tool/
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/tool/1
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/tool/2.1
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/tool/2.2
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/tool/_default
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/tool/envs
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/variant/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/variant/2.0/
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/variant/2.0/a
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/variant/2.0/b
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/variant/2.1/
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/variant/2.1/b
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/variant/2.1/c
--rw-rw-rw-   0 root         (0) root         (0)     3834 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/test_tool_registry.py
--rw-rw-rw-   0 root         (0) root         (0)     2995 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/test_tools_match.py
--rw-rw-rw-   0 root         (0) root         (0)     3221 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/test_tools_options.py
--rw-rw-rw-   0 root         (0) root         (0)       37 2024-04-16 07:31:33.000000 momotor_engine_options-2.0.1/version.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/.idea/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/.idea/inspectionProfiles/
+-rw-rw-rw-   0 root         (0) root         (0)      779 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-rw-rw-   0 root         (0) root         (0)      174 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0 root         (0) root         (0)      296 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/.idea/modules.xml
+-rw-rw-rw-   0 root         (0) root         (0)      566 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/.idea/momotor.lib.engine-options.iml
+-rw-rw-rw-   0 root         (0) root         (0)      238 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/.idea/workspace.xml
+-rw-rw-rw-   0 root         (0) root         (0)    16748 2024-04-25 07:11:19.000000 momotor_engine_options-2.0.2/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     2658 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      778 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      764 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/docs/source/_static/
+-rw-rw-rw-   0 root         (0) root         (0)     6988 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/docs/source/_static/logo-text-negative.png
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/docs/source/_static/logo-text.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/docs/source/_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      672 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/docs/source/_templates/projectlinks.html
+-rw-rw-rw-   0 root         (0) root         (0)     4647 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/docs/source/dependencies.rst
+-rw-rw-rw-   0 root         (0) root         (0)      161 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/docs/source/exceptions.rst
+-rw-rw-rw-   0 root         (0) root         (0)      583 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/docs/source/option.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/docs/source/options/
+-rw-rw-rw-   0 root         (0) root         (0)      516 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/docs/source/options/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/docs/source/options/scheduler.rst
+-rw-rw-rw-   0 root         (0) root         (0)      895 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/docs/source/options/tools.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/docs/source/parser/
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/docs/source/parser/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    31565 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/docs/source/parser/syntax.rst
+-rw-rw-rw-   0 root         (0) root         (0)      134 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/docs/source/providers.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6992 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/docs/source/registry.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11618 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/docs/source/result_query.rst
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/docs/source/task_id.rst
+-rw-rw-rw-   0 root         (0) root         (0)      618 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/docs/source/utilities.rst
+-rw-rw-rw-   0 root         (0) root         (0)      436 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/publish-docs.sh
+-rw-rw-rw-   0 root         (0) root         (0)     2673 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      413 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/semver.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/src/momotor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/src/momotor/options/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7428 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/convert.py
+-rw-rw-rw-   0 root         (0) root         (0)     8438 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/dependencies.py
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/doc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/src/momotor/options/domain/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/domain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/src/momotor/options/domain/scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/domain/scheduler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/domain/scheduler/_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)    11584 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/domain/scheduler/preflight.py
+-rw-rw-rw-   0 root         (0) root         (0)     8274 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/domain/scheduler/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4367 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/domain/scheduler/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/src/momotor/options/domain/tools/
+-rw-rw-rw-   0 root         (0) root         (0)     6226 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/domain/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/domain/tools/_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      630 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/exception.py
+-rw-rw-rw-   0 root         (0) root         (0)     1723 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/filter_files.py
+-rw-rw-rw-   0 root         (0) root         (0)    13396 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/option.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/src/momotor/options/parser/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/parser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1996 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/parser/consts.py
+-rw-rw-rw-   0 root         (0) root         (0)     3581 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/parser/keyvalue.py
+-rw-rw-rw-   0 root         (0) root         (0)     4151 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/parser/modifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     2103 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/parser/placeholders.py
+-rw-rw-rw-   0 root         (0) root         (0)    24967 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/parser/reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     8335 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/parser/selector.py
+-rw-rw-rw-   0 root         (0) root         (0)     1710 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/parser/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1055 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/providers.py
+-rw-rw-rw-   0 root         (0) root         (0)     6490 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/result_query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/src/momotor/options/sphinx/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/sphinx/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2555 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/sphinx/fixextref.py
+-rw-rw-rw-   0 root         (0) root         (0)    16823 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/sphinx/option.py
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/split.py
+-rw-rw-rw-   0 root         (0) root         (0)     9202 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/task_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/src/momotor/options/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      919 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6312 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/tools/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)    12546 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/tools/tool.py
+-rw-rw-rw-   0 root         (0) root         (0)      507 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/tools/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     6103 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/tools/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      776 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/src/momotor/options/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/src/momotor_engine_options.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2658 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/src/momotor_engine_options.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3296 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/src/momotor_engine_options.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/src/momotor_engine_options.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      360 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/src/momotor_engine_options.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/src/momotor_engine_options.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     7508 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/tests/test_option_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4365 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/tests/test_parser_modifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     6167 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/tests/test_parser_placeholders.py
+-rw-rw-rw-   0 root         (0) root         (0)     9529 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/tests/test_parser_reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     8543 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/tests/test_parser_selector.py
+-rw-rw-rw-   0 root         (0) root         (0)     8110 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/tests/test_utils_dependencies.py
+-rw-rw-rw-   0 root         (0) root         (0)     9006 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/tests/test_utils_tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/tests/tools/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/tests/tools/files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/tests/tools/files/toolregistry.d/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/tests/tools/files/toolregistry.d/nodefault/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/tests/tools/files/toolregistry.d/nodefault/1
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/tests/tools/files/toolregistry.d/nodefault/2.1
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/tests/tools/files/toolregistry.d/nodefault/named
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/tests/tools/files/toolregistry.d/tool/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/tests/tools/files/toolregistry.d/tool/1
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/tests/tools/files/toolregistry.d/tool/2.1
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/tests/tools/files/toolregistry.d/tool/2.2
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/tests/tools/files/toolregistry.d/tool/_default
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/tests/tools/files/toolregistry.d/tool/envs
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/tests/tools/files/toolregistry.d/variant/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/tests/tools/files/toolregistry.d/variant/2.0/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/tests/tools/files/toolregistry.d/variant/2.0/a
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/tests/tools/files/toolregistry.d/variant/2.0/b
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:11:24.000000 momotor_engine_options-2.0.2/tests/tools/files/toolregistry.d/variant/2.1/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/tests/tools/files/toolregistry.d/variant/2.1/b
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/tests/tools/files/toolregistry.d/variant/2.1/c
+-rw-rw-rw-   0 root         (0) root         (0)     3834 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/tests/tools/test_tool_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     2995 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/tests/tools/test_tools_match.py
+-rw-rw-rw-   0 root         (0) root         (0)     3221 2024-04-25 07:10:46.000000 momotor_engine_options-2.0.2/tests/tools/test_tools_options.py
+-rw-rw-rw-   0 root         (0) root         (0)       37 2024-04-25 07:11:19.000000 momotor_engine_options-2.0.2/version.toml
```

### Comparing `momotor_engine_options-2.0.1/.gitignore` & `momotor_engine_options-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/.gitlab-ci.yml` & `momotor_engine_options-2.0.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/.idea/inspectionProfiles/Project_Default.xml` & `momotor_engine_options-2.0.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/.idea/momotor.lib.engine-options.iml` & `momotor_engine_options-2.0.2/.idea/momotor.lib.engine-options.iml`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/CHANGELOG.md` & `momotor_engine_options-2.0.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # CHANGELOG
 
 
 
+## v2.0.2 (2024-04-25)
+
+### Fix
+
+* fix: do not add an empty or None label property ([`2f887e7`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/2f887e750499ccc662b2dd00ad9f89d600f5d0df))
+
+
 ## v2.0.1 (2024-04-16)
 
 ### Fix
 
 * fix: update dependencies ([`1b4261a`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/1b4261a04486ff6174ae9cd1b7f3109b4f2684ed))
 
 
@@ -115,16 +122,14 @@
 
 ### Unknown
 
 * doc: small doc update ([`36a526d`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/36a526da74d136d5054964c754ab7686e559c3a1))
 
 * doc: use full path to reference Checklet options ([`5b1d1f1`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/5b1d1f1ecc705949ce1927031fe9840131567540))
 
-* doc: update intersphinx links for momotor.org docs ([`590d9e8`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/590d9e87cba36e75c13272b1cf2a625ce6e89204))
-
 
 ## v1.2.0 (2023-10-26)
 
 ### Chore
 
 * chore: show exact reference used in exception message ([`177fed1`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/177fed1379073bab8738a9b3785d1d0be7966ef0))
 
@@ -292,16 +297,14 @@
 
 * feat: add `sumf` and `sumr` modifiers ([`533f0cb`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/533f0cb7033cc2ff5d4e005852bd75b259ae7923))
 
 * feat: add `empty_values` argument to `convert_intlist` ([`6be2ea1`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/6be2ea14c10d60fb2967424fe691df28eb95ed5f))
 
 * feat: add convert.convert_intlist ([`9a071c8`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/9a071c8816ea8e913baac322ab409bafe8fb7bd8))
 
-* feat: update ToolName.factory to accept a deconstructed tool base name and versions list ([`7d1b8e2`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/7d1b8e283d9c99bd3ab5effc03f9d0692fbb7267))
-
 ### Fix
 
 * fix: handle tool options provided as child content ([`1a99ffb`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/1a99ffbbcbafdaba7e2451dec8e5bf46ee893e6a))
 
 * fix: relax task reference parsing even more. the initial dot is now not required anymore. the $ and internal operators can be escaped to ignore them ([`f353e7d`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/f353e7d6d52f772f76c326611bdbdb5513b8113b))
 
 * fix: relax task reference parsing, allowing trailing text immediately after the references without a dot as seperator ([`829b40c`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/829b40cee42ad376d4d000d3a3f0f780953eac94))
@@ -365,25 +368,12 @@
 This reverts commit 5cbfdf4834ad5bafc9c91972371f5978ee2c0a13. ([`279d15c`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/279d15cb7e294d3febeedee4fde2fb60fe2e4703))
 
 * add OptionDefinition.deprecated ([`5cbfdf4`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/5cbfdf4834ad5bafc9c91972371f5978ee2c0a13))
 
 
 ## v0.3.0 (2022-03-14)
 
-### Fix
-
-* fix: add more unit tests for cases with defaults ([`fd425a2`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/fd425a211f4d34bbc10b9a1d84204d5f4563ca26))
-
 ### Unknown
 
 * 0.3.0
 
 &#39;chore: bump version number&#39; ([`3439b8a`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/3439b8a8eb29b2d4976b2374873aec6f22e45347))
-
-
-## v0.2.3 (2022-01-24)
-
-### Unknown
-
-* 0.2.3
-
-&#39;chore: bump version number&#39; ([`be35ea1`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/be35ea1b1c0ff327d209d74360ef7e0df0126c84))
```

### Comparing `momotor_engine_options-2.0.1/PKG-INFO` & `momotor_engine_options-2.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momotor-engine-options
-Version: 2.0.1
+Version: 2.0.2
 Summary: Momotor Engine Options Library
 Author-email: Erik Scheffers <e.t.j.scheffers@tue.nl>
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Homepage, https://momotor.org
 Project-URL: Documentation, https://momotor.org/doc/engine/momotor-engine-options/
 Project-URL: Repository, https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/
 Project-URL: Tracker, https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/issues
```

### Comparing `momotor_engine_options-2.0.1/README.md` & `momotor_engine_options-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/docs/Makefile` & `momotor_engine_options-2.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/docs/make.bat` & `momotor_engine_options-2.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/docs/source/_static/logo-text-negative.png` & `momotor_engine_options-2.0.2/docs/source/_static/logo-text-negative.png`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/docs/source/_static/logo-text.png` & `momotor_engine_options-2.0.2/docs/source/_static/logo-text.png`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/docs/source/_templates/projectlinks.html` & `momotor_engine_options-2.0.2/docs/source/_templates/projectlinks.html`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/docs/source/conf.py` & `momotor_engine_options-2.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/docs/source/index.rst` & `momotor_engine_options-2.0.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/docs/source/options/index.rst` & `momotor_engine_options-2.0.2/docs/source/options/index.rst`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/docs/source/options/tools.rst` & `momotor_engine_options-2.0.2/docs/source/options/tools.rst`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/docs/source/parser/index.rst` & `momotor_engine_options-2.0.2/docs/source/parser/index.rst`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/docs/source/parser/syntax.rst` & `momotor_engine_options-2.0.2/docs/source/parser/syntax.rst`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/docs/source/registry.rst` & `momotor_engine_options-2.0.2/docs/source/registry.rst`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/docs/source/result_query.rst` & `momotor_engine_options-2.0.2/docs/source/result_query.rst`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/docs/source/utilities.rst` & `momotor_engine_options-2.0.2/docs/source/utilities.rst`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/pyproject.toml` & `momotor_engine_options-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/convert.py` & `momotor_engine_options-2.0.2/src/momotor/options/convert.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/dependencies.py` & `momotor_engine_options-2.0.2/src/momotor/options/dependencies.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/doc.py` & `momotor_engine_options-2.0.2/src/momotor/options/doc.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/domain/scheduler/preflight.py` & `momotor_engine_options-2.0.2/src/momotor/options/domain/scheduler/preflight.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import collections
 import json
 import logging
-import typing
 import warnings
 
 from typing_extensions import TypeAlias  # Py 3.10+
 
 from momotor.bundles import ResultsBundle
 from momotor.bundles.elements.properties import Property
 from momotor.bundles.elements.result import Result, Outcome
@@ -166,18 +165,19 @@
     properties = {
         **status_props,
         **action_props,
         'preflight-trigger': trigger,
         'source': __name__,
     }
 
+    # Emulate LabelOptionMixin's handling of the label option
     if 'label' not in properties:
-        # Emulate LabelOptionMixin's handling of the label option
         label = LABEL_OPTION.resolve(providers, subdomains=True)
-        properties['label'] = replace_task_placeholder(label, providers.task_id)
+        if label:
+            properties['label'] = replace_task_placeholder(label, providers.task_id)
 
     bundle = ResultsBundle()
 
     step = providers.step
     if step:
         options = (option.recreate(bundle) for option in step.options)
     else:
```

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/domain/scheduler/tasks.py` & `momotor_engine_options-2.0.2/src/momotor/options/domain/scheduler/tasks.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/domain/scheduler/tools.py` & `momotor_engine_options-2.0.2/src/momotor/options/domain/scheduler/tools.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/domain/tools/__init__.py` & `momotor_engine_options-2.0.2/src/momotor/options/domain/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/exception.py` & `momotor_engine_options-2.0.2/src/momotor/options/exception.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/filter_files.py` & `momotor_engine_options-2.0.2/src/momotor/options/filter_files.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/option.py` & `momotor_engine_options-2.0.2/src/momotor/options/option.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/parser/consts.py` & `momotor_engine_options-2.0.2/src/momotor/options/parser/consts.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/parser/keyvalue.py` & `momotor_engine_options-2.0.2/src/momotor/options/parser/keyvalue.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/parser/modifier.py` & `momotor_engine_options-2.0.2/src/momotor/options/parser/modifier.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/parser/placeholders.py` & `momotor_engine_options-2.0.2/src/momotor/options/parser/placeholders.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/parser/reference.py` & `momotor_engine_options-2.0.2/src/momotor/options/parser/reference.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/parser/selector.py` & `momotor_engine_options-2.0.2/src/momotor/options/parser/selector.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/parser/tasks.py` & `momotor_engine_options-2.0.2/src/momotor/options/parser/tasks.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/providers.py` & `momotor_engine_options-2.0.2/src/momotor/options/providers.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/result_query.py` & `momotor_engine_options-2.0.2/src/momotor/options/result_query.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/sphinx/fixextref.py` & `momotor_engine_options-2.0.2/src/momotor/options/sphinx/fixextref.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/sphinx/option.py` & `momotor_engine_options-2.0.2/src/momotor/options/sphinx/option.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/split.py` & `momotor_engine_options-2.0.2/src/momotor/options/split.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/task_id.py` & `momotor_engine_options-2.0.2/src/momotor/options/task_id.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/tools/__init__.py` & `momotor_engine_options-2.0.2/src/momotor/options/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/tools/registry.py` & `momotor_engine_options-2.0.2/src/momotor/options/tools/registry.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/tools/tool.py` & `momotor_engine_options-2.0.2/src/momotor/options/tools/tool.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/tools/version.py` & `momotor_engine_options-2.0.2/src/momotor/options/tools/version.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor/options/types.py` & `momotor_engine_options-2.0.2/src/momotor/options/types.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/src/momotor_engine_options.egg-info/PKG-INFO` & `momotor_engine_options-2.0.2/src/momotor_engine_options.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momotor-engine-options
-Version: 2.0.1
+Version: 2.0.2
 Summary: Momotor Engine Options Library
 Author-email: Erik Scheffers <e.t.j.scheffers@tue.nl>
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Homepage, https://momotor.org
 Project-URL: Documentation, https://momotor.org/doc/engine/momotor-engine-options/
 Project-URL: Repository, https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/
 Project-URL: Tracker, https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/issues
```

### Comparing `momotor_engine_options-2.0.1/src/momotor_engine_options.egg-info/SOURCES.txt` & `momotor_engine_options-2.0.2/src/momotor_engine_options.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/tests/test_option_definition.py` & `momotor_engine_options-2.0.2/tests/test_option_definition.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/tests/test_parser_modifier.py` & `momotor_engine_options-2.0.2/tests/test_parser_modifier.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/tests/test_parser_placeholders.py` & `momotor_engine_options-2.0.2/tests/test_parser_placeholders.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/tests/test_parser_reference.py` & `momotor_engine_options-2.0.2/tests/test_parser_reference.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/tests/test_parser_selector.py` & `momotor_engine_options-2.0.2/tests/test_parser_selector.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/tests/test_utils_dependencies.py` & `momotor_engine_options-2.0.2/tests/test_utils_dependencies.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/tests/test_utils_tasks.py` & `momotor_engine_options-2.0.2/tests/test_utils_tasks.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/tests/tools/test_tool_registry.py` & `momotor_engine_options-2.0.2/tests/tools/test_tool_registry.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/tests/tools/test_tools_match.py` & `momotor_engine_options-2.0.2/tests/tools/test_tools_match.py`

 * *Files identical despite different names*

### Comparing `momotor_engine_options-2.0.1/tests/tools/test_tools_options.py` & `momotor_engine_options-2.0.2/tests/tools/test_tools_options.py`

 * *Files identical despite different names*

