# Comparing `tmp/geneweaver_client-0.7.0a8.tar.gz` & `tmp/geneweaver_client-0.7.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneweaver_client-0.7.0a8.tar", max compression
+gzip compressed data, was "geneweaver_client-0.7.0a9.tar", max compression
```

## Comparing `geneweaver_client-0.7.0a8.tar` & `geneweaver_client-0.7.0a9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0    11356 2024-03-22 13:01:55.081563 geneweaver_client-0.7.0a8/LICENSE
--rw-r--r--   0        0        0     2961 2024-03-22 13:01:55.081563 geneweaver_client-0.7.0a8/README.md
--rw-r--r--   0        0        0     1193 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/pyproject.toml
--rw-r--r--   0        0        0      163 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/__init__.py
--rw-r--r--   0        0        0       37 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/api/__init__.py
--rw-r--r--   0        0        0      227 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/api/exc.py
--rw-r--r--   0        0        0     1466 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/api/genes.py
--rw-r--r--   0        0        0     1166 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/api/genesets.py
--rw-r--r--   0        0        0       37 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/api/graph/__init__.py
--rw-r--r--   0        0        0     7607 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/api/graph/graph.py
--rw-r--r--   0        0        0     1765 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/api/utils.py
--rw-r--r--   0        0        0     4987 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/auth.py
--rw-r--r--   0        0        0       66 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/batch/__init__.py
--rw-r--r--   0        0        0       48 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/cli/__init__.py
--rw-r--r--   0        0        0      855 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/cli/alpha/__init__.py
--rw-r--r--   0        0        0      402 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/cli/alpha/api/__init__.py
--rw-r--r--   0        0        0     1144 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/cli/alpha/api/genes.py
--rw-r--r--   0        0        0      843 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/cli/alpha/api/genesets.py
--rw-r--r--   0        0        0      180 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/cli/alpha/api/list.py
--rw-r--r--   0        0        0      356 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/cli/alpha/datasets/__init__.py
--rw-r--r--   0        0        0      347 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/cli/alpha/datasets/main.py
--rw-r--r--   0        0        0      293 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/cli/alpha/parse/__init__.py
--rw-r--r--   0        0        0     4308 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/cli/alpha/parse/batch.py
--rw-r--r--   0        0        0     7867 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/cli/alpha/parse/convert.py
--rw-r--r--   0        0        0      551 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/cli/alpha/parse/main.py
--rw-r--r--   0        0        0     5039 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/cli/alpha/parse/utils.py
--rw-r--r--   0        0        0      587 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/cli/beta/__init__.py
--rw-r--r--   0        0        0     1035 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/cli/beta/auth.py
--rw-r--r--   0        0        0     1071 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/cli/main.py
--rw-r--r--   0        0        0      110 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/core/__init__.py
--rw-r--r--   0        0        0     1425 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/core/app_dir.py
--rw-r--r--   0        0        0      136 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/core/config.py
--rw-r--r--   0        0        0     1282 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/core/config_class.py
--rw-r--r--   0        0        0      117 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/datasets/__init__.py
--rw-r--r--   0        0        0     1476 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/datasets/base.py
--rw-r--r--   0        0        0      186 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/datasets/nci60/__init__.py
--rw-r--r--   0        0        0     1668 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/datasets/nci60/dna_combined_acgh_gene_summary.py
--rw-r--r--   0        0        0      139 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/exceptions.py
--rw-r--r--   0        0        0    10536 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/gedb.py
--rw-r--r--   0        0        0      127 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/parser/__init__.py
--rw-r--r--   0        0        0     5003 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/parser/batch.py
--rw-r--r--   0        0        0     5031 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/parser/general.py
--rw-r--r--   0        0        0       72 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/render/__init__.py
--rw-r--r--   0        0        0     1357 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/user_config.py
--rw-r--r--   0        0        0       51 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/utils/__init__.py
--rw-r--r--   0        0        0       43 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/utils/cli/__init__.py
--rw-r--r--   0        0        0       52 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/utils/cli/decorators/__init__.py
--rw-r--r--   0        0        0      507 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/utils/cli/decorators/errors.py
--rw-r--r--   0        0        0     1353 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/utils/cli/decorators/options.py
--rw-r--r--   0        0        0       46 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/utils/cli/print/__init__.py
--rw-r--r--   0        0        0     1056 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/utils/cli/print/file_info.py
--rw-r--r--   0        0        0      541 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/utils/cli/print/tables.py
--rw-r--r--   0        0        0       48 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/utils/cli/prompt/__init__.py
--rw-r--r--   0        0        0      659 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/utils/cli/prompt/bool.py
--rw-r--r--   0        0        0     4382 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/utils/cli/prompt/enum.py
--rw-r--r--   0        0        0     2780 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/utils/cli/prompt/generic.py
--rw-r--r--   0        0        0     2120 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/utils/cli/prompt/list.py
--rw-r--r--   0        0        0     1306 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/utils/cli/prompt/none.py
--rw-r--r--   0        0        0     3753 2024-03-22 13:01:55.085563 geneweaver_client-0.7.0a8/src/geneweaver/client/utils/cli/prompt/pydantic.py
--rw-r--r--   0        0        0     4042 1970-01-01 00:00:00.000000 geneweaver_client-0.7.0a8/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/LICENSE
+-rw-r--r--   0        0        0     2961 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/README.md
+-rw-r--r--   0        0        0     1193 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/pyproject.toml
+-rw-r--r--   0        0        0      163 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/__init__.py
+-rw-r--r--   0        0        0       37 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/api/__init__.py
+-rw-r--r--   0        0        0      227 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/api/exc.py
+-rw-r--r--   0        0        0     1466 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/api/genes.py
+-rw-r--r--   0        0        0     1166 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/api/genesets.py
+-rw-r--r--   0        0        0       37 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/api/graph/__init__.py
+-rw-r--r--   0        0        0     7607 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/api/graph/graph.py
+-rw-r--r--   0        0        0     1765 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/api/utils.py
+-rw-r--r--   0        0        0     4987 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/auth.py
+-rw-r--r--   0        0        0       66 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/batch/__init__.py
+-rw-r--r--   0        0        0       48 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/cli/__init__.py
+-rw-r--r--   0        0        0      855 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/cli/alpha/__init__.py
+-rw-r--r--   0        0        0      402 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/cli/alpha/api/__init__.py
+-rw-r--r--   0        0        0     1144 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/cli/alpha/api/genes.py
+-rw-r--r--   0        0        0      843 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/cli/alpha/api/genesets.py
+-rw-r--r--   0        0        0      180 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/cli/alpha/api/list.py
+-rw-r--r--   0        0        0      356 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/cli/alpha/datasets/__init__.py
+-rw-r--r--   0        0        0      347 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/cli/alpha/datasets/main.py
+-rw-r--r--   0        0        0      293 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/cli/alpha/parse/__init__.py
+-rw-r--r--   0        0        0     4308 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/cli/alpha/parse/batch.py
+-rw-r--r--   0        0        0     7867 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/cli/alpha/parse/convert.py
+-rw-r--r--   0        0        0      551 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/cli/alpha/parse/main.py
+-rw-r--r--   0        0        0     5039 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/cli/alpha/parse/utils.py
+-rw-r--r--   0        0        0      587 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/cli/beta/__init__.py
+-rw-r--r--   0        0        0     1035 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/cli/beta/auth.py
+-rw-r--r--   0        0        0     1071 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/cli/main.py
+-rw-r--r--   0        0        0      110 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/core/__init__.py
+-rw-r--r--   0        0        0     1425 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/core/app_dir.py
+-rw-r--r--   0        0        0      136 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/core/config.py
+-rw-r--r--   0        0        0     1282 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/core/config_class.py
+-rw-r--r--   0        0        0      117 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/datasets/__init__.py
+-rw-r--r--   0        0        0     1476 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/datasets/base.py
+-rw-r--r--   0        0        0      186 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/datasets/nci60/__init__.py
+-rw-r--r--   0        0        0     1668 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/datasets/nci60/dna_combined_acgh_gene_summary.py
+-rw-r--r--   0        0        0      139 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/exceptions.py
+-rw-r--r--   0        0        0    10944 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/gedb.py
+-rw-r--r--   0        0        0      127 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/parser/__init__.py
+-rw-r--r--   0        0        0     5003 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/parser/batch.py
+-rw-r--r--   0        0        0     5031 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/parser/general.py
+-rw-r--r--   0        0        0       72 2024-03-22 18:36:35.566365 geneweaver_client-0.7.0a9/src/geneweaver/client/render/__init__.py
+-rw-r--r--   0        0        0     1357 2024-03-22 18:36:35.570365 geneweaver_client-0.7.0a9/src/geneweaver/client/user_config.py
+-rw-r--r--   0        0        0       51 2024-03-22 18:36:35.570365 geneweaver_client-0.7.0a9/src/geneweaver/client/utils/__init__.py
+-rw-r--r--   0        0        0       43 2024-03-22 18:36:35.570365 geneweaver_client-0.7.0a9/src/geneweaver/client/utils/cli/__init__.py
+-rw-r--r--   0        0        0       52 2024-03-22 18:36:35.570365 geneweaver_client-0.7.0a9/src/geneweaver/client/utils/cli/decorators/__init__.py
+-rw-r--r--   0        0        0      507 2024-03-22 18:36:35.570365 geneweaver_client-0.7.0a9/src/geneweaver/client/utils/cli/decorators/errors.py
+-rw-r--r--   0        0        0     1353 2024-03-22 18:36:35.570365 geneweaver_client-0.7.0a9/src/geneweaver/client/utils/cli/decorators/options.py
+-rw-r--r--   0        0        0       46 2024-03-22 18:36:35.570365 geneweaver_client-0.7.0a9/src/geneweaver/client/utils/cli/print/__init__.py
+-rw-r--r--   0        0        0     1056 2024-03-22 18:36:35.570365 geneweaver_client-0.7.0a9/src/geneweaver/client/utils/cli/print/file_info.py
+-rw-r--r--   0        0        0      541 2024-03-22 18:36:35.570365 geneweaver_client-0.7.0a9/src/geneweaver/client/utils/cli/print/tables.py
+-rw-r--r--   0        0        0       48 2024-03-22 18:36:35.570365 geneweaver_client-0.7.0a9/src/geneweaver/client/utils/cli/prompt/__init__.py
+-rw-r--r--   0        0        0      659 2024-03-22 18:36:35.570365 geneweaver_client-0.7.0a9/src/geneweaver/client/utils/cli/prompt/bool.py
+-rw-r--r--   0        0        0     4382 2024-03-22 18:36:35.570365 geneweaver_client-0.7.0a9/src/geneweaver/client/utils/cli/prompt/enum.py
+-rw-r--r--   0        0        0     2780 2024-03-22 18:36:35.570365 geneweaver_client-0.7.0a9/src/geneweaver/client/utils/cli/prompt/generic.py
+-rw-r--r--   0        0        0     2120 2024-03-22 18:36:35.570365 geneweaver_client-0.7.0a9/src/geneweaver/client/utils/cli/prompt/list.py
+-rw-r--r--   0        0        0     1306 2024-03-22 18:36:35.570365 geneweaver_client-0.7.0a9/src/geneweaver/client/utils/cli/prompt/none.py
+-rw-r--r--   0        0        0     3753 2024-03-22 18:36:35.570365 geneweaver_client-0.7.0a9/src/geneweaver/client/utils/cli/prompt/pydantic.py
+-rw-r--r--   0        0        0     4042 1970-01-01 00:00:00.000000 geneweaver_client-0.7.0a9/PKG-INFO
```

### Comparing `geneweaver_client-0.7.0a8/LICENSE` & `geneweaver_client-0.7.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/README.md` & `geneweaver_client-0.7.0a9/README.md`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/pyproject.toml` & `geneweaver_client-0.7.0a9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geneweaver-client"
-version = "0.7.0a8"
+version = "0.7.0a9"
 description = "A Python Client for the Geneweaver API"
 authors = ["Jax Computational Sciences <cssc@jax.org>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://thejacksonlaboratory.github.io/geneweaver-docs/"
 repository = "https://github.com/TheJacksonLaboratory/geneweaver-client"
 packages = [
```

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/api/genes.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/api/genes.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/api/genesets.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/api/genesets.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/api/graph/graph.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/api/graph/graph.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/api/utils.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/api/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/auth.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/auth.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/cli/alpha/__init__.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/cli/alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/cli/alpha/api/genes.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/cli/alpha/api/genes.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/cli/alpha/api/genesets.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/cli/alpha/api/genesets.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/cli/alpha/parse/batch.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/cli/alpha/parse/batch.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/cli/alpha/parse/convert.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/cli/alpha/parse/convert.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/cli/alpha/parse/main.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/cli/alpha/parse/main.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/cli/alpha/parse/utils.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/cli/alpha/parse/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/cli/beta/__init__.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/cli/beta/__init__.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/cli/beta/auth.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/cli/beta/auth.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/cli/main.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/cli/main.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/core/app_dir.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/core/app_dir.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/core/config_class.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/core/config_class.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/datasets/base.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/datasets/base.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/datasets/nci60/dna_combined_acgh_gene_summary.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/datasets/nci60/dna_combined_acgh_gene_summary.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/gedb.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/gedb.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,20 @@
 """
 The source either experimentally determined or imputed using
 machine learning ridge regression. For strain recommender, the
 imputed sources are most often used.
 @usage: from org.jax.gedb import SourceType
 """
 
+Sex = Enum("Sex", ["Female", "Male", "Both"])
+"""
+The imputed sex field. This is not direct biological sex
+but a representation of the input sex(s) to the alg.
+"""
+
 
 # TODO Should data access objects go in api?
 @dataclass
 class DataRequest:
     """Object to request data e.g. a search.
 
     This request mirrors the available fields in:
@@ -57,15 +63,17 @@
     """
 
     values: List[float] = None  # noqa: N815
     names: List[str] = None  # noqa: N815
     weights: List[float] = None  # noqa: N815
     geneIds: List[str] = None  # noqa: N815
     strains: List[str] = None  # noqa: N815
+    strain: str = None  # noqa: N815
     tissue: str = None  # noqa: N815
+    sexes: List[str] = None  # noqa: N815
 
 
 # TODO Should data access objects go in api?
 @dataclass
 class Metadata:
     """Object to contain Metadata.
 
@@ -127,15 +135,15 @@
         """
         url = self._get_search_url()
 
         response = self._post(url, drequest.__dict__)
 
         # TODO Not sure if need to deal with typing here.
         # Need to write test to check.
-        return response.json()
+        return [self._class_from_args(DataResult, item) for item in response.json()]
 
     def distinct(self, field: str) -> Set[str]:
         """Get list of unique fields from metadata.
 
         @param field: For instance to get the
          strains return field = "tissue"
         Available fields are listed in swagger
@@ -179,15 +187,15 @@
         """Sort the data results by any of their properties.
 
         @param property: String e.g. "strain" to sort by strain
         @param the raw list of data results returned from a 'search' call.
         """
         ret = {}
         for dr in expressions:
-            pvalue = dr.get(prop)
+            pvalue = getattr(dr, prop)
 
             collection = ret.get(pvalue, None)
             if collection is None:
                 collection = []
                 ret[pvalue] = collection
             collection.append(dr)
 
@@ -199,39 +207,41 @@
         """Sort the data results by property then group the genes and individual names.
 
         @param property: String e.g. "strain" to sort by strain
         @param the raw list of data results returned from a 'search' call.
         """
         ret = {}
         for dr in expressions:
-            pvalue = dr.get(prop)
+            pvalue = getattr(dr, prop)
 
-            gene_id = dr.get("geneIds")[0]
+            gene_id = dr.geneIds[0]
             # Map of values by indiv name
             indivs = ret.get(pvalue, None)
             if indivs is None:
                 indivs = {}
                 ret[pvalue] = indivs
 
-            names: List[str] = dr.get("names")
-            values: List[float] = dr.get("values")
-
-            for name, value in zip(names, values):
-                geneset = indivs.get(name)
+            names: List[str] = dr.names
+            values: List[float] = dr.values  # noqa: PD011
+            sexes: List[str] = dr.sexes
+
+            for name, value, sex in zip(names, values, sexes):
+                key = (name, sex)
+                geneset = indivs.get(key)
                 if geneset is None:
                     geneset = OrderedDict()
-                    indivs[name] = geneset
+                    indivs[key] = geneset
 
                 geneset[gene_id] = value
 
         return ret
 
-    def frame(self, data: dict, strain: str, indiv_name: str) -> DataFrame:
+    def frame(self, data: dict, strain: str, indiv_name: str, sex: Sex) -> DataFrame:
         """Convert a dictionary of gene expression to frame."""
-        ar = numpy.array(list(data[strain][indiv_name].items()))
+        ar = numpy.array(list(data[strain][(indiv_name, sex.name)].items()))
         return DataFrame(ar, columns=["gene_id", "expr"])
 
     def random(self, ingest_id: str, size: int) -> DataFrame:
         """Get a random gene expression frame."""
         url = "{}/{}?gsize={}".format(self._get_random_url(), ingest_id, size)
         response = self._get(url)
```

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/parser/batch.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/parser/batch.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/parser/general.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/parser/general.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/user_config.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/user_config.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/utils/cli/decorators/options.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/utils/cli/decorators/options.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/utils/cli/print/file_info.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/utils/cli/print/file_info.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/utils/cli/print/tables.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/utils/cli/print/tables.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/utils/cli/prompt/bool.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/utils/cli/prompt/bool.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/utils/cli/prompt/enum.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/utils/cli/prompt/enum.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/utils/cli/prompt/generic.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/utils/cli/prompt/generic.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/utils/cli/prompt/list.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/utils/cli/prompt/list.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/utils/cli/prompt/none.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/utils/cli/prompt/none.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/src/geneweaver/client/utils/cli/prompt/pydantic.py` & `geneweaver_client-0.7.0a9/src/geneweaver/client/utils/cli/prompt/pydantic.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.7.0a8/PKG-INFO` & `geneweaver_client-0.7.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneweaver-client
-Version: 0.7.0a8
+Version: 0.7.0a9
 Summary: A Python Client for the Geneweaver API
 Home-page: https://thejacksonlaboratory.github.io/geneweaver-docs/
 License: Apache-2.0
 Author: Jax Computational Sciences
 Author-email: cssc@jax.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

