# Comparing `tmp/suiteas-0.3.1.tar.gz` & `tmp/suiteas-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suiteas-0.3.1.tar", last modified: Wed Feb 14 02:17:11 2024, max compression
+gzip compressed data, was "suiteas-0.3.2.tar", last modified: Wed Apr 24 22:19:03 2024, max compression
```

## Comparing `suiteas-0.3.1.tar` & `suiteas-0.3.2.tar`

### file list

```diff
@@ -1,238 +1,240 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.186663 suiteas-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.146662 suiteas-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.162663 suiteas-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-02-14 02:16:47.000000 suiteas-0.3.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-02-14 02:16:47.000000 suiteas-0.3.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-02-14 02:16:47.000000 suiteas-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-02-14 02:16:47.000000 suiteas-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-14 02:16:47.000000 suiteas-0.3.1/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-14 02:16:47.000000 suiteas-0.3.1/.python-version
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-02-14 02:16:47.000000 suiteas-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-02-14 02:17:11.186663 suiteas-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-02-14 02:16:47.000000 suiteas-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.146662 suiteas-0.3.1/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.162663 suiteas-0.3.1/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.162663 suiteas-0.3.1/doc/source/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-14 02:16:47.000000 suiteas-0.3.1/doc/source/dev/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-02-14 02:16:47.000000 suiteas-0.3.1/doc/source/dev/release_checklist.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.162663 suiteas-0.3.1/doc/source/diagrams/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-14 02:16:47.000000 suiteas-0.3.1/doc/source/diagrams/code_entities.d2
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-02-14 02:16:47.000000 suiteas-0.3.1/doc/source/diagrams/config.d2
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-02-14 02:16:47.000000 suiteas-0.3.1/doc/source/diagrams/overall.d2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.162663 suiteas-0.3.1/doc/source/release/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.162663 suiteas-0.3.1/doc/source/release/changelog/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-02-14 02:16:47.000000 suiteas-0.3.1/doc/source/release/changelog/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-14 02:16:47.000000 suiteas-0.3.1/doc/source/release/changelog/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-14 02:16:47.000000 suiteas-0.3.1/doc/source/release/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-14 02:16:47.000000 suiteas-0.3.1/doc/source/release/notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-14 02:16:47.000000 suiteas-0.3.1/doc/source/why.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-02-14 02:16:47.000000 suiteas-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-02-14 02:16:47.000000 suiteas-0.3.1/requirements-dev.lock
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-02-14 02:16:47.000000 suiteas-0.3.1/requirements.lock
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 02:17:11.186663 suiteas-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.150662 suiteas-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.166663 suiteas-0.3.1/src/suiteas/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-14 02:16:47.000000 suiteas-0.3.1/src/suiteas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-02-14 02:16:47.000000 suiteas-0.3.1/src/suiteas/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-14 02:17:11.000000 suiteas-0.3.1/src/suiteas/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-02-14 02:16:47.000000 suiteas-0.3.1/src/suiteas/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.166663 suiteas-0.3.1/src/suiteas/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/src/suiteas/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-02-14 02:16:47.000000 suiteas-0.3.1/src/suiteas/core/check.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-14 02:16:47.000000 suiteas-0.3.1/src/suiteas/core/enforce.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-02-14 02:16:47.000000 suiteas-0.3.1/src/suiteas/core/names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-02-14 02:16:47.000000 suiteas-0.3.1/src/suiteas/core/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-02-14 02:16:47.000000 suiteas-0.3.1/src/suiteas/core/print.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-02-14 02:16:47.000000 suiteas-0.3.1/src/suiteas/core/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-02-14 02:16:47.000000 suiteas-0.3.1/src/suiteas/core/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-14 02:16:47.000000 suiteas-0.3.1/src/suiteas/core/violations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-02-14 02:16:47.000000 suiteas-0.3.1/src/suiteas/domain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.170663 suiteas-0.3.1/src/suiteas/read/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/src/suiteas/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-02-14 02:16:47.000000 suiteas-0.3.1/src/suiteas/read/codebase.py
--rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-02-14 02:16:47.000000 suiteas-0.3.1/src/suiteas/read/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-02-14 02:16:47.000000 suiteas-0.3.1/src/suiteas/read/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-02-14 02:16:47.000000 suiteas-0.3.1/src/suiteas/read/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-02-14 02:16:47.000000 suiteas-0.3.1/src/suiteas/read/pytest_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-02-14 02:16:47.000000 suiteas-0.3.1/src/suiteas/read/pytest_suite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.186663 suiteas-0.3.1/src/suiteas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-02-14 02:17:11.000000 suiteas-0.3.1/src/suiteas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-02-14 02:17:11.000000 suiteas-0.3.1/src/suiteas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 02:17:11.000000 suiteas-0.3.1/src/suiteas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-14 02:17:11.000000 suiteas-0.3.1/src/suiteas.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-14 02:17:11.000000 suiteas-0.3.1/src/suiteas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-14 02:17:11.000000 suiteas-0.3.1/src/suiteas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.170663 suiteas-0.3.1/src/suiteas_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/src/suiteas_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-14 02:16:47.000000 suiteas-0.3.1/src/suiteas_test/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-14 02:16:47.000000 suiteas-0.3.1/suiteas_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.170663 suiteas-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.150662 suiteas-0.3.1/tests/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.170663 suiteas-0.3.1/tests/assets/config_files/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/config_files/bad_ignore.toml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/config_files/badlists.toml
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/config_files/complete.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/config_files/empty.toml
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/config_files/extra_subsection.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/config_files/no_section.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/config_files/superfluous.toml
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/config_files/syntax_err.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.174663 suiteas-0.3.1/tests/assets/files/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/files/branch_logic_func.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/files/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/files/invalid_syntax.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/files/lambda_func.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/files/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/files/nested_func.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/files/one_class.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/files/one_func.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/files/test_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/files/test_one_class.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/files/test_one_class_one_func.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/files/test_two_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.158662 suiteas-0.3.1/tests/assets/projects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.150662 suiteas-0.3.1/tests/assets/projects/autoall/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.150662 suiteas-0.3.1/tests/assets/projects/autoall/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.174663 suiteas-0.3.1/tests/assets/projects/autoall/src/p8eovx9k/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/autoall/src/p8eovx9k/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.150662 suiteas-0.3.1/tests/assets/projects/autoall/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.150662 suiteas-0.3.1/tests/assets/projects/autoall/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.174663 suiteas-0.3.1/tests/assets/projects/autoall/tests/unit/p8eovx9k/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/autoall/tests/unit/p8eovx9k/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.174663 suiteas-0.3.1/tests/assets/projects/automultipkgnamesrc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.174663 suiteas-0.3.1/tests/assets/projects/automultipkgnamesrc/g5qyyvdv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/automultipkgnamesrc/g5qyyvdv/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/automultipkgnamesrc/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.150662 suiteas-0.3.1/tests/assets/projects/automultipkgnamesrc/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.150662 suiteas-0.3.1/tests/assets/projects/automultipkgnamesrc/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.174663 suiteas-0.3.1/tests/assets/projects/automultipkgnamesrc/tests/unit/g5qyyvdv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/automultipkgnamesrc/tests/unit/g5qyyvdv/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.174663 suiteas-0.3.1/tests/assets/projects/automultipkgnamesrc/tests/unit/zhd1kcvi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/automultipkgnamesrc/tests/unit/zhd1kcvi/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.174663 suiteas-0.3.1/tests/assets/projects/automultipkgnamesrc/zhd1kcvi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/automultipkgnamesrc/zhd1kcvi/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.174663 suiteas-0.3.1/tests/assets/projects/automultisetuptoolssrc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.174663 suiteas-0.3.1/tests/assets/projects/automultisetuptoolssrc/lh0fehzp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/automultisetuptoolssrc/lh0fehzp/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/automultisetuptoolssrc/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.150662 suiteas-0.3.1/tests/assets/projects/automultisetuptoolssrc/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.150662 suiteas-0.3.1/tests/assets/projects/automultisetuptoolssrc/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.174663 suiteas-0.3.1/tests/assets/projects/automultisetuptoolssrc/tests/unit/lh0fehzp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/automultisetuptoolssrc/tests/unit/lh0fehzp/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.174663 suiteas-0.3.1/tests/assets/projects/automultisetuptoolssrc/tests/unit/z00rc6ru/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/automultisetuptoolssrc/tests/unit/z00rc6ru/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.174663 suiteas-0.3.1/tests/assets/projects/automultisetuptoolssrc/z00rc6ru/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/automultisetuptoolssrc/z00rc6ru/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.174663 suiteas-0.3.1/tests/assets/projects/autopkgnamesrc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.174663 suiteas-0.3.1/tests/assets/projects/autopkgnamesrc/ixvm0b6u/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/autopkgnamesrc/ixvm0b6u/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/autopkgnamesrc/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.154662 suiteas-0.3.1/tests/assets/projects/autopkgnamesrc/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.154662 suiteas-0.3.1/tests/assets/projects/autopkgnamesrc/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.174663 suiteas-0.3.1/tests/assets/projects/autopkgnamesrc/tests/unit/ixvm0b6u/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/autopkgnamesrc/tests/unit/ixvm0b6u/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.174663 suiteas-0.3.1/tests/assets/projects/autoprojnamesrc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.174663 suiteas-0.3.1/tests/assets/projects/autoprojnamesrc/pr4a7g7m/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/autoprojnamesrc/pr4a7g7m/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/autoprojnamesrc/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.154662 suiteas-0.3.1/tests/assets/projects/autoprojnamesrc/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.154662 suiteas-0.3.1/tests/assets/projects/autoprojnamesrc/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.174663 suiteas-0.3.1/tests/assets/projects/autoprojnamesrc/tests/unit/pr4a7g7m/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/autoprojnamesrc/tests/unit/pr4a7g7m/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.178663 suiteas-0.3.1/tests/assets/projects/autosetuptoolssrc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.178663 suiteas-0.3.1/tests/assets/projects/autosetuptoolssrc/euul5ld4/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/autosetuptoolssrc/euul5ld4/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/autosetuptoolssrc/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.154662 suiteas-0.3.1/tests/assets/projects/autosetuptoolssrc/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.154662 suiteas-0.3.1/tests/assets/projects/autosetuptoolssrc/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.178663 suiteas-0.3.1/tests/assets/projects/autosetuptoolssrc/tests/unit/euul5ld4/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/autosetuptoolssrc/tests/unit/euul5ld4/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.178663 suiteas-0.3.1/tests/assets/projects/autosrc/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/autosrc/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.178663 suiteas-0.3.1/tests/assets/projects/autosrc/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/autosrc/src/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.154662 suiteas-0.3.1/tests/assets/projects/autosrc/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.178663 suiteas-0.3.1/tests/assets/projects/autosrc/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/autosrc/tests/unit/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.178663 suiteas-0.3.1/tests/assets/projects/empty/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/empty/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.178663 suiteas-0.3.1/tests/assets/projects/empty_config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/empty_config/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.178663 suiteas-0.3.1/tests/assets/projects/no_tests_dir/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/no_tests_dir/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.154662 suiteas-0.3.1/tests/assets/projects/no_tests_dir/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.178663 suiteas-0.3.1/tests/assets/projects/no_tests_dir/src/t82sedcy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/no_tests_dir/src/t82sedcy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.178663 suiteas-0.3.1/tests/assets/projects/no_unit_dir/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/no_unit_dir/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.154662 suiteas-0.3.1/tests/assets/projects/no_unit_dir/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.178663 suiteas-0.3.1/tests/assets/projects/no_unit_dir/src/tx41rdni/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/no_unit_dir/src/tx41rdni/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.178663 suiteas-0.3.1/tests/assets/projects/no_unit_dir/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/no_unit_dir/tests/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.178663 suiteas-0.3.1/tests/assets/projects/one_func_no_test/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/one_func_no_test/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.154662 suiteas-0.3.1/tests/assets/projects/one_func_no_test/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.178663 suiteas-0.3.1/tests/assets/projects/one_func_no_test/src/pp8cadfs/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/one_func_no_test/src/pp8cadfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.158662 suiteas-0.3.1/tests/assets/projects/one_func_no_test/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.158662 suiteas-0.3.1/tests/assets/projects/one_func_no_test/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.178663 suiteas-0.3.1/tests/assets/projects/one_func_no_test/tests/unit/pp8cadfs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/one_func_no_test/tests/unit/pp8cadfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.178663 suiteas-0.3.1/tests/assets/projects/srcconfig_only/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/srcconfig_only/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.178663 suiteas-0.3.1/tests/assets/projects/srcconfig_only/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/srcconfig_only/src/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.178663 suiteas-0.3.1/tests/assets/projects/trivial_pass/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/trivial_pass/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.158662 suiteas-0.3.1/tests/assets/projects/trivial_pass/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.178663 suiteas-0.3.1/tests/assets/projects/trivial_pass/src/af8o7tt1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/trivial_pass/src/af8o7tt1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.158662 suiteas-0.3.1/tests/assets/projects/trivial_pass/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.158662 suiteas-0.3.1/tests/assets/projects/trivial_pass/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.178663 suiteas-0.3.1/tests/assets/projects/trivial_pass/tests/unit/af8o7tt1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/trivial_pass/tests/unit/af8o7tt1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.178663 suiteas-0.3.1/tests/assets/projects/two_files/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/two_files/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.158662 suiteas-0.3.1/tests/assets/projects/two_files/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.182663 suiteas-0.3.1/tests/assets/projects/two_files/src/ow9xem9x/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/two_files/src/ow9xem9x/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/two_files/src/ow9xem9x/goodbye.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/two_files/src/ow9xem9x/hello.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.158662 suiteas-0.3.1/tests/assets/projects/two_files/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.158662 suiteas-0.3.1/tests/assets/projects/two_files/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.182663 suiteas-0.3.1/tests/assets/projects/two_files/tests/unit/ow9xem9x/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/two_files/tests/unit/ow9xem9x/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/two_files/tests/unit/ow9xem9x/test_goodbye.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/two_files/tests/unit/ow9xem9x/test_hello.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.182663 suiteas-0.3.1/tests/assets/projects/unitrootdir/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/unitrootdir/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.158662 suiteas-0.3.1/tests/assets/projects/unitrootdir/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.182663 suiteas-0.3.1/tests/assets/projects/unitrootdir/src/wm96nwsm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/unitrootdir/src/wm96nwsm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.182663 suiteas-0.3.1/tests/assets/projects/unitrootdir/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/assets/projects/unitrootdir/tests/test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.182663 suiteas-0.3.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/fixtures/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.182663 suiteas-0.3.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.182663 suiteas-0.3.1/tests/unit/suiteas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/unit/suiteas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.182663 suiteas-0.3.1/tests/unit/suiteas/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/unit/suiteas/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/unit/suiteas/core/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/unit/suiteas/core/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/unit/suiteas/core/test_print.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/unit/suiteas/core/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 02:17:11.186663 suiteas-0.3.1/tests/unit/suiteas/read/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/unit/suiteas/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/unit/suiteas/read/test_codebase.py
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/unit/suiteas/read/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/unit/suiteas/read/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/unit/suiteas/read/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/unit/suiteas/read/test_pytest_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/unit/suiteas/read/test_pytest_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-02-14 02:16:47.000000 suiteas-0.3.1/tests/unit/suiteas/test_domain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.486749 suiteas-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.454748 suiteas-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.466749 suiteas-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-24 22:18:40.000000 suiteas-0.3.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-24 22:18:40.000000 suiteas-0.3.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-24 22:18:40.000000 suiteas-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-24 22:18:40.000000 suiteas-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-24 22:18:40.000000 suiteas-0.3.2/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 22:18:40.000000 suiteas-0.3.2/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-24 22:18:40.000000 suiteas-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-24 22:19:03.486749 suiteas-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-24 22:18:40.000000 suiteas-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.454748 suiteas-0.3.2/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.466749 suiteas-0.3.2/doc/changelog_entries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/doc/changelog_entries/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.466749 suiteas-0.3.2/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.466749 suiteas-0.3.2/doc/source/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-24 22:18:40.000000 suiteas-0.3.2/doc/source/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-24 22:18:40.000000 suiteas-0.3.2/doc/source/dev/release_checklist.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.470749 suiteas-0.3.2/doc/source/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-24 22:18:40.000000 suiteas-0.3.2/doc/source/diagrams/code_entities.d2
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-24 22:18:40.000000 suiteas-0.3.2/doc/source/diagrams/config.d2
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-24 22:18:40.000000 suiteas-0.3.2/doc/source/diagrams/overall.d2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.470749 suiteas-0.3.2/doc/source/release/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.470749 suiteas-0.3.2/doc/source/release/changelog/
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-24 22:18:40.000000 suiteas-0.3.2/doc/source/release/changelog/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-24 22:18:40.000000 suiteas-0.3.2/doc/source/release/changelog/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-24 22:18:40.000000 suiteas-0.3.2/doc/source/release/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-24 22:18:40.000000 suiteas-0.3.2/doc/source/release/notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-24 22:18:40.000000 suiteas-0.3.2/doc/source/why.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-24 22:18:40.000000 suiteas-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-24 22:18:40.000000 suiteas-0.3.2/requirements-dev.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-24 22:18:40.000000 suiteas-0.3.2/requirements.lock
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 22:19:03.486749 suiteas-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.458749 suiteas-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.470749 suiteas-0.3.2/src/suiteas/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-24 22:18:40.000000 suiteas-0.3.2/src/suiteas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-24 22:18:40.000000 suiteas-0.3.2/src/suiteas/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-24 22:19:03.000000 suiteas-0.3.2/src/suiteas/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-24 22:18:40.000000 suiteas-0.3.2/src/suiteas/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.470749 suiteas-0.3.2/src/suiteas/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/src/suiteas/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-24 22:18:40.000000 suiteas-0.3.2/src/suiteas/core/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-24 22:18:40.000000 suiteas-0.3.2/src/suiteas/core/enforce.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-24 22:18:40.000000 suiteas-0.3.2/src/suiteas/core/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-24 22:18:40.000000 suiteas-0.3.2/src/suiteas/core/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-24 22:18:40.000000 suiteas-0.3.2/src/suiteas/core/print.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-24 22:18:40.000000 suiteas-0.3.2/src/suiteas/core/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-24 22:18:40.000000 suiteas-0.3.2/src/suiteas/core/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-24 22:18:40.000000 suiteas-0.3.2/src/suiteas/core/violations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-24 22:18:40.000000 suiteas-0.3.2/src/suiteas/domain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.474749 suiteas-0.3.2/src/suiteas/read/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/src/suiteas/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-24 22:18:40.000000 suiteas-0.3.2/src/suiteas/read/codebase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-04-24 22:18:40.000000 suiteas-0.3.2/src/suiteas/read/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-24 22:18:40.000000 suiteas-0.3.2/src/suiteas/read/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-24 22:18:40.000000 suiteas-0.3.2/src/suiteas/read/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-24 22:18:40.000000 suiteas-0.3.2/src/suiteas/read/pytest_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-24 22:18:40.000000 suiteas-0.3.2/src/suiteas/read/pytest_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.486749 suiteas-0.3.2/src/suiteas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-24 22:19:03.000000 suiteas-0.3.2/src/suiteas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-24 22:19:03.000000 suiteas-0.3.2/src/suiteas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 22:19:03.000000 suiteas-0.3.2/src/suiteas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-24 22:19:03.000000 suiteas-0.3.2/src/suiteas.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-24 22:19:03.000000 suiteas-0.3.2/src/suiteas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 22:19:03.000000 suiteas-0.3.2/src/suiteas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.474749 suiteas-0.3.2/src/suiteas_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/src/suiteas_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-24 22:18:40.000000 suiteas-0.3.2/src/suiteas_test/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-24 22:18:40.000000 suiteas-0.3.2/suiteas_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.474749 suiteas-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.458749 suiteas-0.3.2/tests/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.474749 suiteas-0.3.2/tests/assets/config_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/config_files/bad_ignore.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/config_files/badlists.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/config_files/complete.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/config_files/empty.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/config_files/extra_subsection.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/config_files/no_section.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/config_files/superfluous.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/config_files/syntax_err.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/files/branch_logic_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/files/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/files/invalid_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/files/lambda_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/files/multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/files/nested_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/files/one_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/files/one_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/files/test_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/files/test_one_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/files/test_one_class_one_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/files/test_two_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.466749 suiteas-0.3.2/tests/assets/projects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.458749 suiteas-0.3.2/tests/assets/projects/autoall/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.458749 suiteas-0.3.2/tests/assets/projects/autoall/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/projects/autoall/src/p8eovx9k/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/autoall/src/p8eovx9k/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.458749 suiteas-0.3.2/tests/assets/projects/autoall/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.458749 suiteas-0.3.2/tests/assets/projects/autoall/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/projects/autoall/tests/unit/p8eovx9k/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/autoall/tests/unit/p8eovx9k/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/projects/automultipkgnamesrc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/projects/automultipkgnamesrc/g5qyyvdv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/automultipkgnamesrc/g5qyyvdv/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/automultipkgnamesrc/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.458749 suiteas-0.3.2/tests/assets/projects/automultipkgnamesrc/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.458749 suiteas-0.3.2/tests/assets/projects/automultipkgnamesrc/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/projects/automultipkgnamesrc/tests/unit/g5qyyvdv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/automultipkgnamesrc/tests/unit/g5qyyvdv/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/projects/automultipkgnamesrc/tests/unit/zhd1kcvi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/automultipkgnamesrc/tests/unit/zhd1kcvi/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/projects/automultipkgnamesrc/zhd1kcvi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/automultipkgnamesrc/zhd1kcvi/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/projects/automultisetuptoolssrc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/projects/automultisetuptoolssrc/lh0fehzp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/automultisetuptoolssrc/lh0fehzp/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/automultisetuptoolssrc/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.458749 suiteas-0.3.2/tests/assets/projects/automultisetuptoolssrc/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.458749 suiteas-0.3.2/tests/assets/projects/automultisetuptoolssrc/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/projects/automultisetuptoolssrc/tests/unit/lh0fehzp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/automultisetuptoolssrc/tests/unit/lh0fehzp/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/projects/automultisetuptoolssrc/tests/unit/z00rc6ru/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/automultisetuptoolssrc/tests/unit/z00rc6ru/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/projects/automultisetuptoolssrc/z00rc6ru/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/automultisetuptoolssrc/z00rc6ru/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/projects/autopkgnamesrc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/projects/autopkgnamesrc/ixvm0b6u/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/autopkgnamesrc/ixvm0b6u/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/autopkgnamesrc/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.458749 suiteas-0.3.2/tests/assets/projects/autopkgnamesrc/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.458749 suiteas-0.3.2/tests/assets/projects/autopkgnamesrc/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/projects/autopkgnamesrc/tests/unit/ixvm0b6u/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/autopkgnamesrc/tests/unit/ixvm0b6u/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/projects/autoprojnamesrc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/projects/autoprojnamesrc/pr4a7g7m/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/autoprojnamesrc/pr4a7g7m/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/autoprojnamesrc/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.462749 suiteas-0.3.2/tests/assets/projects/autoprojnamesrc/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.462749 suiteas-0.3.2/tests/assets/projects/autoprojnamesrc/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/projects/autoprojnamesrc/tests/unit/pr4a7g7m/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/autoprojnamesrc/tests/unit/pr4a7g7m/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/projects/autosetuptoolssrc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/projects/autosetuptoolssrc/euul5ld4/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/autosetuptoolssrc/euul5ld4/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/autosetuptoolssrc/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.462749 suiteas-0.3.2/tests/assets/projects/autosetuptoolssrc/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.462749 suiteas-0.3.2/tests/assets/projects/autosetuptoolssrc/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/projects/autosetuptoolssrc/tests/unit/euul5ld4/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/autosetuptoolssrc/tests/unit/euul5ld4/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/projects/autosrc/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/autosrc/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.478749 suiteas-0.3.2/tests/assets/projects/autosrc/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/autosrc/src/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.462749 suiteas-0.3.2/tests/assets/projects/autosrc/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.482749 suiteas-0.3.2/tests/assets/projects/autosrc/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/autosrc/tests/unit/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.482749 suiteas-0.3.2/tests/assets/projects/empty/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/empty/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.482749 suiteas-0.3.2/tests/assets/projects/empty_config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/empty_config/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.482749 suiteas-0.3.2/tests/assets/projects/no_tests_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/no_tests_dir/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.462749 suiteas-0.3.2/tests/assets/projects/no_tests_dir/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.482749 suiteas-0.3.2/tests/assets/projects/no_tests_dir/src/t82sedcy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/no_tests_dir/src/t82sedcy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.482749 suiteas-0.3.2/tests/assets/projects/no_unit_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/no_unit_dir/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.462749 suiteas-0.3.2/tests/assets/projects/no_unit_dir/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.482749 suiteas-0.3.2/tests/assets/projects/no_unit_dir/src/tx41rdni/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/no_unit_dir/src/tx41rdni/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.482749 suiteas-0.3.2/tests/assets/projects/no_unit_dir/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/no_unit_dir/tests/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.482749 suiteas-0.3.2/tests/assets/projects/one_func_no_test/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/one_func_no_test/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.462749 suiteas-0.3.2/tests/assets/projects/one_func_no_test/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.482749 suiteas-0.3.2/tests/assets/projects/one_func_no_test/src/pp8cadfs/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/one_func_no_test/src/pp8cadfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.462749 suiteas-0.3.2/tests/assets/projects/one_func_no_test/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.462749 suiteas-0.3.2/tests/assets/projects/one_func_no_test/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.482749 suiteas-0.3.2/tests/assets/projects/one_func_no_test/tests/unit/pp8cadfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/one_func_no_test/tests/unit/pp8cadfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.482749 suiteas-0.3.2/tests/assets/projects/srcconfig_only/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/srcconfig_only/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.482749 suiteas-0.3.2/tests/assets/projects/srcconfig_only/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/srcconfig_only/src/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.482749 suiteas-0.3.2/tests/assets/projects/trivial_pass/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/trivial_pass/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.462749 suiteas-0.3.2/tests/assets/projects/trivial_pass/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.482749 suiteas-0.3.2/tests/assets/projects/trivial_pass/src/af8o7tt1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/trivial_pass/src/af8o7tt1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.462749 suiteas-0.3.2/tests/assets/projects/trivial_pass/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.462749 suiteas-0.3.2/tests/assets/projects/trivial_pass/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.482749 suiteas-0.3.2/tests/assets/projects/trivial_pass/tests/unit/af8o7tt1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/trivial_pass/tests/unit/af8o7tt1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.482749 suiteas-0.3.2/tests/assets/projects/two_files/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/two_files/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.462749 suiteas-0.3.2/tests/assets/projects/two_files/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.482749 suiteas-0.3.2/tests/assets/projects/two_files/src/ow9xem9x/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/two_files/src/ow9xem9x/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/two_files/src/ow9xem9x/goodbye.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/two_files/src/ow9xem9x/hello.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.466749 suiteas-0.3.2/tests/assets/projects/two_files/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.466749 suiteas-0.3.2/tests/assets/projects/two_files/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.482749 suiteas-0.3.2/tests/assets/projects/two_files/tests/unit/ow9xem9x/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/two_files/tests/unit/ow9xem9x/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/two_files/tests/unit/ow9xem9x/test_goodbye.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/two_files/tests/unit/ow9xem9x/test_hello.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.482749 suiteas-0.3.2/tests/assets/projects/unitrootdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/unitrootdir/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.466749 suiteas-0.3.2/tests/assets/projects/unitrootdir/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.482749 suiteas-0.3.2/tests/assets/projects/unitrootdir/src/wm96nwsm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/unitrootdir/src/wm96nwsm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.482749 suiteas-0.3.2/tests/assets/projects/unitrootdir/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/assets/projects/unitrootdir/tests/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.486749 suiteas-0.3.2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/fixtures/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.486749 suiteas-0.3.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.486749 suiteas-0.3.2/tests/unit/suiteas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/unit/suiteas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.486749 suiteas-0.3.2/tests/unit/suiteas/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/unit/suiteas/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/unit/suiteas/core/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/unit/suiteas/core/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/unit/suiteas/core/test_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/unit/suiteas/core/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:19:03.486749 suiteas-0.3.2/tests/unit/suiteas/read/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/unit/suiteas/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/unit/suiteas/read/test_codebase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/unit/suiteas/read/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/unit/suiteas/read/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/unit/suiteas/read/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/unit/suiteas/read/test_pytest_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/unit/suiteas/read/test_pytest_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-24 22:18:40.000000 suiteas-0.3.2/tests/unit/suiteas/test_domain.py
```

### Comparing `suiteas-0.3.1/.github/workflows/ci.yml` & `suiteas-0.3.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/.github/workflows/pypi-publish.yml` & `suiteas-0.3.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/.gitignore` & `suiteas-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/.pre-commit-config.yaml` & `suiteas-0.3.2/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.5.0
     hooks:
       - id: check-merge-conflict
         args: [--assume-in-merge]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.2.1 # Sync with pyproject.toml
+    rev: v0.2.2 # Sync with pyproject.toml
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.8.0 # Sync with pyproject.toml
     hooks:
```

### Comparing `suiteas-0.3.1/LICENSE` & `suiteas-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/PKG-INFO` & `suiteas-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suiteas
-Version: 0.3.1
+Version: 0.3.2
 Summary: An opinionated testing suite organizer for pytest
 Author-email: Nathan McDougall <nathan.j.mcdougall@gmail.com>
 License: MIT
 Project-URL: Source Code, https://github.com/nathanjmcdougall/suiteas
 Project-URL: Bug Tracker, https://github.com/nathanjmcdougall/suiteas/issues
 Keywords: pytest,test,testing,test suite,suite,sync,synchronize,pre-commit,boilerplate,skeleton
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -50,15 +50,15 @@
 >
 > _very satisfactory; excellent._
 
 The recommended way to use SuiteAs is using the [`pre-commit`](https://pre-commit.com/) framework. Add the following to your `.pre-commit-config.yaml` file:
 
 ```yaml
 - repo: https://github.com/nathanjmcdougall/suiteas
-    rev: v0.3.0
+    rev: v0.3.1
     hooks:
       - id: suiteas
 ```
 
 You can also install and run SuiteAs as a standalone package:
 
 ```bash
```

### Comparing `suiteas-0.3.1/README.md` & `suiteas-0.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 >
 > _very satisfactory; excellent._
 
 The recommended way to use SuiteAs is using the [`pre-commit`](https://pre-commit.com/) framework. Add the following to your `.pre-commit-config.yaml` file:
 
 ```yaml
 - repo: https://github.com/nathanjmcdougall/suiteas
-    rev: v0.3.0
+    rev: v0.3.1
     hooks:
       - id: suiteas
 ```
 
 You can also install and run SuiteAs as a standalone package:
 
 ```bash
```

### Comparing `suiteas-0.3.1/doc/source/dev/release_checklist.rst` & `suiteas-0.3.2/doc/source/dev/release_checklist.rst`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/doc/source/diagrams/config.d2` & `suiteas-0.3.2/doc/source/diagrams/config.d2`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/doc/source/diagrams/overall.d2` & `suiteas-0.3.2/doc/source/diagrams/overall.d2`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/doc/source/release/changelog/changelog.rst` & `suiteas-0.3.2/doc/source/release/changelog/changelog.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+0.3.2 (2024-04-25)
+==================
+
+Features
+--------
+
+- Better error messages are now provided for the situation where ``src_rel_path`` is set
+  incorrectly and where as a result, SuiteAs is looking for unit tests for something which
+  is not a package. (https://github.com/nathanjmcdougall/suiteas/issues/98)
+
+
+0.3.1 (2024-03-03)
+==================
+
+Features
+--------
+
+- Added support for Python 3.10
+
+
 0.3.0 (2024-01-18)
 ==================
 
 Features
 --------
 
 - Global `ignore` configuration is now supported, allowing you to disable a linting rule
```

### Comparing `suiteas-0.3.1/pyproject.toml` & `suiteas-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     "twine>=4.0.2",
     "pre-commit>=3.5.0",
     "setuptools>=68.2.2",
     "setuptools_scm[toml]>=8.0.4",
     "pytest>=7.4.3",
     "typing-extensions>=4.8.0",
     #
-    "ruff==0.2.1",
+    "ruff==0.2.2",
     "mypy==1.8.0",
     "python-dotenv==1.0.0",
     # ^Sync with .pre-commit-config.yaml
     "pysource-codegen>=0.5.0",
     "pytest-cov>=4.1.0",
 ]
 
@@ -125,15 +125,15 @@
     "PTH201",  # This is controversial, when dealing with relative paths "." is clearer.
     "PERF401", # This can hurt readability; the performance is not always worth it.
 ]
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
-[tool.ruff.extend-per-file-ignores]
+[tool.ruff.lint.extend-per-file-ignores]
 "src/suiteas/**/__init__.py" = [
     "D104", # __init__.py files do not need a docstring necessarily.
 ]
 "src/suiteas_test/**/__init__.py" = [
     "D104", # __init__.py files do not need a docstring necessarily.
 ]
 "tests/**/__init__.py" = [
```

### Comparing `suiteas-0.3.1/src/suiteas/config.py` & `suiteas-0.3.2/src/suiteas/config.py`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/src/suiteas/core/check.py` & `suiteas-0.3.2/src/suiteas/core/check.py`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/src/suiteas/core/path.py` & `suiteas-0.3.2/src/suiteas/core/path.py`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/src/suiteas/core/print.py` & `suiteas-0.3.2/src/suiteas/core/print.py`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/src/suiteas/core/rules.py` & `suiteas-0.3.2/src/suiteas/core/rules.py`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/src/suiteas/core/run.py` & `suiteas-0.3.2/src/suiteas/core/run.py`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/src/suiteas/domain.py` & `suiteas-0.3.2/src/suiteas/domain.py`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/src/suiteas/read/codebase.py` & `suiteas-0.3.2/src/suiteas/read/codebase.py`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/src/suiteas/read/config.py` & `suiteas-0.3.2/src/suiteas/read/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -121,28 +121,32 @@
 
     if pkg_names is not None:
         for pkg_name in pkg_names:
             if not (proj_dir / pkg_name).exists():
                 break
             return Path(".")
 
+    course_of_action = (
+        "Please manually configure the package name(s) and/or source directory in "
+        "pyproject.toml as follows:\n"
+        "[tool.suiteas]\n"
+        'pkg_names = ["???"]\n'
+        'src_rel_path = "???"'
+    )
+
     if found_toml:
         msg = (
-            "Could not automatically determine source directory for the project. "
-            "Please manually configure this in pyproject.toml as follows:\n"
-            "[tool.suiteas]\n"
-            'src_rel_path = "???"'
+            "Could not automatically determine source directory for the project. " +
+            course_of_action
         )
         raise ConfigFileError(msg)
 
     msg = (
         "Could not find configuration file nor determine the source directory for the "
-        "project. Please manually configure this in pyproject.toml as follows:\n"
-        "[tool.suiteas]\n"
-        'src_rel_path = "???"'
+        "project. " + course_of_action
     )
     raise FileNotFoundError(msg)
 
 
 def _heuristic1_pkg_names(*, toml_config: TOMLProjConfig) -> list[str] | None:
     if toml_config.setuptools_pkg_names is not None:
         return toml_config.setuptools_pkg_names
@@ -240,15 +244,20 @@
         pkg_dir = src_dir / pkg_name
         if not pkg_dir.exists():
             msg = f"Could not find package directory of {pkg_name} at {pkg_dir}"
             raise FileNotFoundError(msg)
 
         test_pkg_dir = unittests_dir / pkg_name
         if not test_pkg_dir.exists():
-            msg = f"Could not find unit test directory of {pkg_name} at {test_pkg_dir}"
+            msg = (
+                f"Could not find unit test directory of {pkg_name} at {test_pkg_dir}.\n"
+                f"HINT: If you are not expecting a unit test directory for {pkg_name}, "
+                f"perhaps the `src_rel_path` is set incorrectly."
+            )
+
             raise FileNotFoundError(msg)
 
 
 def _validate_unittest_dir_name(unittests_dir: Path) -> None:
     if not unittests_dir.exists():
         msg = f"Could not find unit tests directory {unittests_dir}"
         raise FileNotFoundError(msg)
```

### Comparing `suiteas-0.3.1/src/suiteas/read/file.py` & `suiteas-0.3.2/src/suiteas/read/file.py`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/src/suiteas/read/project.py` & `suiteas-0.3.2/src/suiteas/read/project.py`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/src/suiteas/read/pytest_file.py` & `suiteas-0.3.2/src/suiteas/read/pytest_file.py`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/src/suiteas/read/pytest_suite.py` & `suiteas-0.3.2/src/suiteas/read/pytest_suite.py`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/src/suiteas.egg-info/PKG-INFO` & `suiteas-0.3.2/src/suiteas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suiteas
-Version: 0.3.1
+Version: 0.3.2
 Summary: An opinionated testing suite organizer for pytest
 Author-email: Nathan McDougall <nathan.j.mcdougall@gmail.com>
 License: MIT
 Project-URL: Source Code, https://github.com/nathanjmcdougall/suiteas
 Project-URL: Bug Tracker, https://github.com/nathanjmcdougall/suiteas/issues
 Keywords: pytest,test,testing,test suite,suite,sync,synchronize,pre-commit,boilerplate,skeleton
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -50,15 +50,15 @@
 >
 > _very satisfactory; excellent._
 
 The recommended way to use SuiteAs is using the [`pre-commit`](https://pre-commit.com/) framework. Add the following to your `.pre-commit-config.yaml` file:
 
 ```yaml
 - repo: https://github.com/nathanjmcdougall/suiteas
-    rev: v0.3.0
+    rev: v0.3.1
     hooks:
       - id: suiteas
 ```
 
 You can also install and run SuiteAs as a standalone package:
 
 ```bash
```

### Comparing `suiteas-0.3.1/src/suiteas.egg-info/SOURCES.txt` & `suiteas-0.3.2/src/suiteas.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 README.md
 pyproject.toml
 requirements-dev.lock
 requirements.lock
 suiteas_hook.py
 .github/workflows/ci.yml
 .github/workflows/pypi-publish.yml
+doc/changelog_entries/.gitkeep
 doc/source/why.rst
 doc/source/dev/index.rst
 doc/source/dev/release_checklist.rst
 doc/source/diagrams/code_entities.d2
 doc/source/diagrams/config.d2
 doc/source/diagrams/overall.d2
 doc/source/release/index.rst
```

### Comparing `suiteas-0.3.1/tests/fixtures/paths.py` & `suiteas-0.3.2/tests/fixtures/paths.py`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/tests/unit/suiteas/core/test_path.py` & `suiteas-0.3.2/tests/unit/suiteas/core/test_path.py`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/tests/unit/suiteas/core/test_print.py` & `suiteas-0.3.2/tests/unit/suiteas/core/test_print.py`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/tests/unit/suiteas/read/test_codebase.py` & `suiteas-0.3.2/tests/unit/suiteas/read/test_codebase.py`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/tests/unit/suiteas/read/test_config.py` & `suiteas-0.3.2/tests/unit/suiteas/read/test_config.py`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/tests/unit/suiteas/read/test_file.py` & `suiteas-0.3.2/tests/unit/suiteas/read/test_file.py`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/tests/unit/suiteas/read/test_project.py` & `suiteas-0.3.2/tests/unit/suiteas/read/test_project.py`

 * *Files identical despite different names*

### Comparing `suiteas-0.3.1/tests/unit/suiteas/read/test_pytest_file.py` & `suiteas-0.3.2/tests/unit/suiteas/read/test_pytest_file.py`

 * *Files identical despite different names*

