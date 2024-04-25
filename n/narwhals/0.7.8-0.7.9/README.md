# Comparing `tmp/narwhals-0.7.8.tar.gz` & `tmp/narwhals-0.7.9.tar.gz`

## Comparing `narwhals-0.7.8.tar` & `narwhals-0.7.9.tar`

### file list

```diff
@@ -1,94 +1,101 @@
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 narwhals-0.7.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 narwhals-0.7.8/CONTRIBUTING.md
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 narwhals-0.7.8/mkdocs.yml
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 narwhals-0.7.8/requirements-dev.txt
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 narwhals-0.7.8/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 narwhals-0.7.8/.github/workflows/extremes.yml
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 narwhals-0.7.8/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 narwhals-0.7.8/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 narwhals-0.7.8/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 narwhals-0.7.8/docs/extending.md
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 narwhals-0.7.8/docs/generate_members.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 narwhals-0.7.8/docs/index.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 narwhals-0.7.8/docs/installation.md
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 narwhals-0.7.8/docs/quick_start.md
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 narwhals-0.7.8/docs/related.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 narwhals-0.7.8/docs/requirements-docs.txt
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 narwhals-0.7.8/docs/roadmap.md
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 narwhals-0.7.8/docs/why.md
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 narwhals-0.7.8/docs/api-reference/dataframe.md
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 narwhals-0.7.8/docs/api-reference/expressions.md
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 narwhals-0.7.8/docs/api-reference/index.md
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.7.8/docs/api-reference/lazyframe.md
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 narwhals-0.7.8/docs/api-reference/narwhals.md
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 narwhals-0.7.8/docs/api-reference/series.md
--rwxr-xr-x   0        0        0   132699 2020-02-02 00:00:00.000000 narwhals-0.7.8/docs/assets/image.png
--rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 narwhals-0.7.8/docs/basics/column.md
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 narwhals-0.7.8/docs/basics/complete_example.md
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 narwhals-0.7.8/docs/basics/dataframe.md
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 narwhals-0.7.8/narwhals/__init__.py
--rw-r--r--   0        0        0    46236 2020-02-02 00:00:00.000000 narwhals-0.7.8/narwhals/dataframe.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 narwhals-0.7.8/narwhals/dependencies.py
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 narwhals-0.7.8/narwhals/dtypes.py
--rw-r--r--   0        0        0     9109 2020-02-02 00:00:00.000000 narwhals-0.7.8/narwhals/expression.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 narwhals-0.7.8/narwhals/functions.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 narwhals-0.7.8/narwhals/group_by.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.8/narwhals/py.typed
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 narwhals-0.7.8/narwhals/series.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 narwhals-0.7.8/narwhals/translate.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 narwhals-0.7.8/narwhals/typing.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 narwhals-0.7.8/narwhals/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.8/narwhals/_pandas_like/__init__.py
--rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 narwhals-0.7.8/narwhals/_pandas_like/dataframe.py
--rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 narwhals-0.7.8/narwhals/_pandas_like/expr.py
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 narwhals-0.7.8/narwhals/_pandas_like/group_by.py
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 narwhals-0.7.8/narwhals/_pandas_like/namespace.py
--rw-r--r--   0        0        0    11222 2020-02-02 00:00:00.000000 narwhals-0.7.8/narwhals/_pandas_like/series.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 narwhals-0.7.8/narwhals/_pandas_like/typing.py
--rw-r--r--   0        0        0    12393 2020-02-02 00:00:00.000000 narwhals-0.7.8/narwhals/_pandas_like/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.8/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.8/tests/group_by_test.py
--rw-r--r--   0        0        0    18415 2020-02-02 00:00:00.000000 narwhals-0.7.8/tests/test_common.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 narwhals-0.7.8/tests/test_dt.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 narwhals-0.7.8/tests/test_group_by.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 narwhals-0.7.8/tests/test_pandas.py
--rw-r--r--   0        0        0     6594 2020-02-02 00:00:00.000000 narwhals-0.7.8/tests/test_series.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 narwhals-0.7.8/tests/test_str.py
--rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 narwhals-0.7.8/tests/tpch_q1_test.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 narwhals-0.7.8/tests/utils.py
--rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 narwhals-0.7.8/tests/data/customer.parquet
--rw-r--r--   0        0        0    34095 2020-02-02 00:00:00.000000 narwhals-0.7.8/tests/data/lineitem.parquet
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 narwhals-0.7.8/tests/data/nation.parquet
--rw-r--r--   0        0        0    24714 2020-02-02 00:00:00.000000 narwhals-0.7.8/tests/data/orders.parquet
--rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 narwhals-0.7.8/tests/data/part.parquet
--rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 narwhals-0.7.8/tests/data/partsupp.parquet
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 narwhals-0.7.8/tests/data/region.parquet
--rw-r--r--   0        0        0    19817 2020-02-02 00:00:00.000000 narwhals-0.7.8/tests/data/supplier.parquet
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.8/tpch/__init__.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 narwhals-0.7.8/tpch/q1.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 narwhals-0.7.8/tpch/q2.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 narwhals-0.7.8/tpch/q3.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 narwhals-0.7.8/tpch/q4.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 narwhals-0.7.8/tpch/q5.py
--rwxr-xr-x   0        0        0    47336 2020-02-02 00:00:00.000000 narwhals-0.7.8/tpch/notebooks/gpu/execute.ipynb
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.7.8/tpch/notebooks/gpu/kernel-metadata.json
--rwxr-xr-x   0        0        0    15160 2020-02-02 00:00:00.000000 narwhals-0.7.8/tpch/notebooks/q1/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.8/tpch/notebooks/q1/kernel-metadata.json
--rwxr-xr-x   0        0        0    16114 2020-02-02 00:00:00.000000 narwhals-0.7.8/tpch/notebooks/q2/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.8/tpch/notebooks/q2/kernel-metadata.json
--rwxr-xr-x   0        0        0    15420 2020-02-02 00:00:00.000000 narwhals-0.7.8/tpch/notebooks/q3/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.8/tpch/notebooks/q3/kernel-metadata.json
--rwxr-xr-x   0        0        0    14794 2020-02-02 00:00:00.000000 narwhals-0.7.8/tpch/notebooks/q4/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.8/tpch/notebooks/q4/kernel-metadata.json
--rwxr-xr-x   0        0        0    15844 2020-02-02 00:00:00.000000 narwhals-0.7.8/tpch/notebooks/q5/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.8/tpch/notebooks/q5/kernel-metadata.json
--rwxr-xr-x   0        0        0    14502 2020-02-02 00:00:00.000000 narwhals-0.7.8/tpch/notebooks/q6/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.8/tpch/notebooks/q6/kernel-metadata.json
--rwxr-xr-x   0        0        0    24376 2020-02-02 00:00:00.000000 narwhals-0.7.8/tpch/notebooks/q7/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.8/tpch/notebooks/q7/kernel-metadata.json
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 narwhals-0.7.8/utils/bump_version.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 narwhals-0.7.8/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 narwhals-0.7.8/LICENSE.md
--rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 narwhals-0.7.8/README.md
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 narwhals-0.7.8/pyproject.toml
--rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 narwhals-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 narwhals-0.7.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 narwhals-0.7.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 narwhals-0.7.9/mkdocs.yml
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 narwhals-0.7.9/requirements-dev.txt
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 narwhals-0.7.9/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 narwhals-0.7.9/.github/workflows/extremes.yml
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 narwhals-0.7.9/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 narwhals-0.7.9/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 narwhals-0.7.9/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/extending.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/generate_members.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/index.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/installation.md
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/quick_start.md
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/related.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/requirements-docs.txt
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/roadmap.md
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/why.md
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/api-reference/dataframe.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/api-reference/dtypes.md
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/api-reference/expressions.md
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/api-reference/expressions_dt.md
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/api-reference/expressions_str.md
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/api-reference/index.md
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/api-reference/lazyframe.md
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/api-reference/narwhals.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/api-reference/series.md
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/api-reference/series_dt.md
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/api-reference/series_str.md
+-rwxr-xr-x   0        0        0   132699 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/assets/image.png
+-rw-r--r--   0        0        0     4475 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/basics/column.md
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/basics/complete_example.md
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/basics/dataframe.md
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/__init__.py
+-rw-r--r--   0        0        0    46236 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/dataframe.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/dependencies.py
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/dtypes.py
+-rw-r--r--   0        0        0     9357 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/expression.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/functions.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/group_by.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/py.typed
+-rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/series.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/translate.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/typing.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/_pandas_like/__init__.py
+-rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/_pandas_like/dataframe.py
+-rw-r--r--   0        0        0     8871 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/_pandas_like/expr.py
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/_pandas_like/group_by.py
+-rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/_pandas_like/namespace.py
+-rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/_pandas_like/series.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/_pandas_like/typing.py
+-rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/_pandas_like/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/group_by_test.py
+-rw-r--r--   0        0        0    19910 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/test_common.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/test_dt.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/test_group_by.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/test_pandas.py
+-rw-r--r--   0        0        0     7772 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/test_series.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/test_str.py
+-rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/tpch_q1_test.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/utils.py
+-rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/data/customer.parquet
+-rw-r--r--   0        0        0    34095 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/data/lineitem.parquet
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/data/nation.parquet
+-rw-r--r--   0        0        0    24714 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/data/orders.parquet
+-rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/data/part.parquet
+-rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/data/partsupp.parquet
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/data/region.parquet
+-rw-r--r--   0        0        0    19817 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/data/supplier.parquet
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/__init__.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/q1.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/q2.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/q3.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/q4.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/q5.py
+-rwxr-xr-x   0        0        0    47336 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/gpu/execute.ipynb
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/gpu/kernel-metadata.json
+-rwxr-xr-x   0        0        0    17858 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q1/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q1/kernel-metadata.json
+-rwxr-xr-x   0        0        0    21797 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q2/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q2/kernel-metadata.json
+-rwxr-xr-x   0        0        0    15420 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q3/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q3/kernel-metadata.json
+-rwxr-xr-x   0        0        0    14794 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q4/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q4/kernel-metadata.json
+-rwxr-xr-x   0        0        0    15844 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q5/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q5/kernel-metadata.json
+-rwxr-xr-x   0        0        0    14502 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q6/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q6/kernel-metadata.json
+-rwxr-xr-x   0        0        0    24376 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q7/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q7/kernel-metadata.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.9/utils/__init__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 narwhals-0.7.9/utils/bump_version.py
+-rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 narwhals-0.7.9/utils/check_api_reference.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 narwhals-0.7.9/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 narwhals-0.7.9/LICENSE.md
+-rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 narwhals-0.7.9/README.md
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 narwhals-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 narwhals-0.7.9/PKG-INFO
```

### Comparing `narwhals-0.7.8/.pre-commit-config.yaml` & `narwhals-0.7.9/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -16,8 +16,16 @@
       exclude: utils|tpch
 - repo: https://github.com/codespell-project/codespell
   rev: 'v2.2.6'
   hooks:
     - id: codespell
       files: \.(py|rst|md)$
       args: [--ignore-words-list=ser]
+- repo: local
+  hooks:
+    - id: check-api-reference
+      name: check-api-reference
+      pass_filenames: false
+      entry: python -m utils.check_api_reference
+      language: python
+      additional_dependencies: [polars]
```

### Comparing `narwhals-0.7.8/CONTRIBUTING.md` & `narwhals-0.7.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/.github/CODE_OF_CONDUCT.md` & `narwhals-0.7.9/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/.github/workflows/extremes.yml` & `narwhals-0.7.9/.github/workflows/extremes.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/.github/workflows/mkdocs.yml` & `narwhals-0.7.9/.github/workflows/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/.github/workflows/publish_to_pypi.yml` & `narwhals-0.7.9/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/.github/workflows/pytest.yml` & `narwhals-0.7.9/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/docs/extending.md` & `narwhals-0.7.9/docs/extending.md`

 * *Files 13% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 Currently, Narwhals recognises the following libraries as inputs:
 
 - pandas
 - Polars
 - cuDF
 - Modin
 
-If you want your own library to be recognised too, you can either:
-
-- open a PR (with tests)
-- or, make sure that, in addition to the public Narwhals API, you also define:
+If you want your own library to be recognised too, you can either open a PR (with tests) or
+you can make sure that, in addition to the public Narwhals API, you also define:
 
   - `DataFrame.__narwhals_dataframe__`: return an object which implements public methods
     from `Narwhals.DataFrame`
   - `DataFrame.__narwhals_namespace__`: return an object which implements public top-level
     functions from `narwhals` (e.g. `narwhals.col`, `narwhals.concat`, ...)
   - `LazyFrame.__narwhals_lazyframe__`: return an object which implements public methods
     from `Narwhals.LazyFrame`
```

### Comparing `narwhals-0.7.8/docs/generate_members.py` & `narwhals-0.7.9/docs/generate_members.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/docs/index.md` & `narwhals-0.7.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/docs/quick_start.md` & `narwhals-0.7.9/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/docs/related.md` & `narwhals-0.7.9/docs/related.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/docs/roadmap.md` & `narwhals-0.7.9/docs/roadmap.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/docs/why.md` & `narwhals-0.7.9/docs/why.md`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 import pandas as pd
 import polars as pl
 
 print(3 in pd.Series([1, 2, 3]))
 print(3 in pl.Series([1, 2, 3]))
 ```
 
-Try it out and see ;)
+Try it out and see ;) Spoiler alert: they don't. pandas checks if `3` is in the index,
+Polars checks if it's in the values.
 
 How about
 ```python
 df_left = pd.DataFrame({'a': [1, 2, 3], 'b': [4, 5, 6]})
 df_right = pd.DataFrame({'a': [1, 2, 3], 'c': [4, 5, 6]})
 df_left.merge(df_right, left_on='b', right_on='c', how='left')
 ```
@@ -26,13 +27,14 @@
 df_left = pl.DataFrame({'a': [1, 2, 3], 'b': [4, 5, 6]})
 df_right = pl.DataFrame({'a': [1, 2, 3], 'c': [4, 5, 6]})
 df_left.join(df_right, left_on='b', right_on='c', how='left')
 ```
 
 ?
 
-There are several such subtle difference between the libraries. By having a unified,
-simple, and predictable API, you can focus on behaviour rather than on slight implementation differences.
-
-Furthermore, both pandas and Polars frequently deprecate behaviour. By having a simple, predictable, and
-mostly stable API, which is tested nightly against the most recent commits from both pandas and Polars,
-you can develop with a lot more confidence.
+There are several such subtle difference between the libraries. Writing dataframe-agnostic code is hard!
+But by having a unified, simple, and predictable API, you can focus on behaviour rather than on subtle
+implementation differences.
+
+Furthermore, both pandas and Polars frequently deprecate behaviour. Narwhals handles this for you by
+testing against nightly builds of both libraries and handling backwards compatibility internally 
+(so you don't have to!).
```

### Comparing `narwhals-0.7.8/docs/api-reference/index.md` & `narwhals-0.7.9/docs/api-reference/index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/docs/assets/image.png` & `narwhals-0.7.9/docs/assets/image.png`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/docs/basics/column.md` & `narwhals-0.7.9/docs/basics/column.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,17 @@
 We only used DataFrame methods there - but what if we need to operate on its columns?
 
 Note that Polars does not have lazy columns. If you need to operate on columns as part of
 a dataframe operation, you should use expressions - but if you need to extract a single
 column, you need to ensure that you start with an eager `DataFrame`. To do that, we'll
 use the `nw.DataFrame` constructor, as opposed to `nw.from_native`.
 
-## Extracting a series
+## Example 1: filter based on a column's values
 
-## Example 1: filter based on a series' values
-
-This can stay lazy, so we just use `nw.from_native`:
+This can stay lazy, so we just use `nw.from_native` and expressions:
 
 ```python exec="1" source="above" session="ex1"
 import narwhals as nw
 
 def my_func(df):
     df_s = nw.from_native(df)
     df_s = df_s.filter(nw.col('a') > 0)
@@ -47,15 +45,15 @@
     df = pl.LazyFrame({'a': [-1, 1, 3], 'b': [3, 5, -3]})
     print(my_func(df).collect())
     ```
 
 ## Example 2: multiply a column's values by a constant
 
 Let's write a dataframe-agnostic function which multiplies the values in column
-`'a'` by 2. This can also stay lazy.
+`'a'` by 2. This can also stay lazy, and can use expressions:
 
 ```python exec="1" source="above" session="ex2"
 import narwhals as nw
 
 def my_func(df):
     df_s = nw.from_native(df)
     df_s = df_s.with_columns(nw.col('a')*2)
@@ -83,15 +81,15 @@
     import polars as pl
 
     df = pl.LazyFrame({'a': [-1, 1, 3], 'b': [3, 5, -3]})
     print(my_func(df).collect())
     ```
 
 Note that column `'a'` was overwritten. If we had wanted to add a new column called `'c'` containing column `'a'`'s
-values multiplied by 2, we could have used `Series.alias`:
+values multiplied by 2, we could have used `Expr.alias`:
 
 ```python exec="1" source="above" session="ex2.1"
 import narwhals as nw
 
 def my_func(df):
     df_s = nw.from_native(df)
     df_s = df_s.with_columns((nw.col('a')*2).alias('c'))
@@ -122,15 +120,16 @@
     print(my_func(df).collect())
     ```
 
 ## Example 3: finding the mean of a column as a scalar
 
 Now, we want to find the mean of column `'a'`, and we need it as a Python scalar.
 This means that computation cannot stay lazy - it must execute!
-Therefore, instead of `nw.from_native`, we'll use `nw.DataFrame`.
+Therefore, instead of `nw.from_native`, we'll use `nw.DataFrame`, and then, instead
+of using expressions, we'll extract a `Series`.
 
 ```python exec="1" source="above" session="ex2"
 import narwhals as nw
 
 def my_func(df):
     df_s = nw.DataFrame(df)
     return df_s['a'].mean()
```

### Comparing `narwhals-0.7.8/docs/basics/complete_example.md` & `narwhals-0.7.9/docs/basics/complete_example.md`

 * *Files 14% similar despite different names*

```diff
@@ -35,24 +35,23 @@
             (nw.col(col) - self._means[col]) / self._std_devs[col]
             for col in df.columns
         )
         return nw.to_native(df)
 ```
 
 Note that all the calculations here can stay lazy if the underlying library permits it.
-For Polars, the return value is a `polars.LazyFrame` - it is the caller's responsibility to
-call `.collect()` on the result if they want to materialise its values.
 
 ## Fit method
 
 Unlike the `transform` method, `fit` cannot stay lazy, as we need to compute concrete values
 for the means and standard deviations.
 
 To be able to get `Series` out of our `DataFrame`, we'll need to use `narwhals.DataFrame` (as opposed to
-`narwhals.from_native`), as Polars doesn't have a concept of lazy `Series`.
+`narwhals.from_native`). This is because Polars doesn't have a concept of lazy `Series`, and so Narwhals
+doesn't either.
 
 ```python
 import narwhals as nw
 
 class StandardScalar:
     def fit(self, df):
         df = nw.DataFrame(df)
@@ -78,15 +77,16 @@
             (nw.col(col) - self._means[col]) / self._std_devs[col]
             for col in df.columns
         )
         return nw.to_native(df)
 ```
 
 Next, let's try running it. Notice how, as `transform` doesn't use
-any eager-only features, so we can make it completely lazy!
+any eager-only features, so we can pass a Polars LazyFrame to it and have it
+stay lazy!
 
 === "pandas"
     ```python exec="true" source="material-block" result="python" session="tute-ex1"
     import pandas as pd
 
     df_train = pd.DataFrame({'a': [1, 2, 3], 'b': [4, 5, 7]})
     df_test = pd.DataFrame({'a': [1, 2, 3], 'b': [4, 5, 7]})
```

### Comparing `narwhals-0.7.8/docs/basics/dataframe.md` & `narwhals-0.7.9/docs/basics/dataframe.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/narwhals/dataframe.py` & `narwhals-0.7.9/narwhals/dataframe.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/narwhals/dependencies.py` & `narwhals-0.7.9/narwhals/dependencies.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/narwhals/dtypes.py` & `narwhals-0.7.9/narwhals/dtypes.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/narwhals/expression.py` & `narwhals-0.7.9/narwhals/expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,20 @@
 from narwhals.utils import flatten
 
 if TYPE_CHECKING:
     from narwhals.typing import IntoExpr
 
 
 def extract_native(expr: Expr, other: Any) -> Any:
+    from narwhals.series import Series
+
     if isinstance(other, Expr):
         return other._call(expr)
+    if isinstance(other, Series):
+        return other._series
     return other
 
 
 class Expr:
     def __init__(self, call: Callable[[Any], Any]) -> None:
         # callable from namespace to expr
         self._call = call
@@ -183,14 +187,17 @@
 
     def n_unique(self) -> Expr:
         return self.__class__(lambda plx: self._call(plx).n_unique())
 
     def unique(self) -> Expr:
         return self.__class__(lambda plx: self._call(plx).unique())
 
+    def sort(self, *, descending: bool = False) -> Expr:
+        return self.__class__(lambda plx: self._call(plx).sort(descending=descending))
+
     # --- transform ---
     def is_between(
         self, lower_bound: Any, upper_bound: Any, closed: str = "both"
     ) -> Expr:
         return self.__class__(
             lambda plx: self._call(plx).is_between(lower_bound, upper_bound, closed)
         )
```

### Comparing `narwhals-0.7.8/narwhals/functions.py` & `narwhals-0.7.9/narwhals/functions.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/narwhals/group_by.py` & `narwhals-0.7.9/narwhals/group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/narwhals/translate.py` & `narwhals-0.7.9/narwhals/translate.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/narwhals/utils.py` & `narwhals-0.7.9/narwhals/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 
 def remove_prefix(text: str, prefix: str) -> str:
     if text.startswith(prefix):
         return text[len(prefix) :]
     return text  # pragma: no cover
 
 
+def remove_suffix(text: str, suffix: str) -> str:  # pragma: no cover
+    if text.endswith(suffix):
+        return text[: -len(suffix)]
+    return text  # pragma: no cover
+
+
 def flatten(args: Any) -> list[Any]:
     if not args:
         return []
     if len(args) == 1 and _is_iterable(args[0]):
         return args[0]  # type: ignore[no-any-return]
     return args  # type: ignore[no-any-return]
```

### Comparing `narwhals-0.7.8/narwhals/_pandas_like/dataframe.py` & `narwhals-0.7.9/narwhals/_pandas_like/dataframe.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/narwhals/_pandas_like/expr.py` & `narwhals-0.7.9/narwhals/_pandas_like/expr.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,14 +179,17 @@
 
     def is_in(self, other: Any) -> Self:
         return register_expression_call(self, "is_in", other)
 
     def drop_nulls(self) -> Self:
         return register_expression_call(self, "drop_nulls")
 
+    def sort(self, *, descending: bool = False) -> Self:
+        return register_expression_call(self, "sort", descending=descending)
+
     def n_unique(self) -> Self:
         return register_expression_call(self, "n_unique")
 
     def unique(self) -> Self:
         return register_expression_call(self, "unique")
 
     def sample(
```

### Comparing `narwhals-0.7.8/narwhals/_pandas_like/group_by.py` & `narwhals-0.7.9/narwhals/_pandas_like/group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/narwhals/_pandas_like/namespace.py` & `narwhals-0.7.9/narwhals/_pandas_like/namespace.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/narwhals/_pandas_like/series.py` & `narwhals-0.7.9/narwhals/_pandas_like/series.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,17 @@
         from narwhals._pandas_like.namespace import PandasNamespace
 
         return PandasNamespace(self._implementation)
 
     def __narwhals_series__(self) -> Self:
         return self
 
+    def __getitem__(self, idx: int) -> Any:
+        return self._series.iloc[idx]
+
     def _rename(self, series: Any, name: str) -> Any:
         if self._use_copy_false:
             return series.rename(name, copy=False)
         return series.rename(name)  # pragma: no cover
 
     def _from_series(self, series: Any) -> Self:
         return self.__class__(
@@ -289,28 +292,24 @@
         *,
         with_replacement: bool = False,
     ) -> PandasSeries:
         ser = self._series
         return self._from_series(ser.sample(n=n, frac=fraction, replace=with_replacement))
 
     def unique(self) -> PandasSeries:
-        if self._implementation != "pandas":
-            raise NotImplementedError
-        import pandas as pd
-
         return self._from_series(
-            pd.Series(
+            self._series.__class__(
                 self._series.unique(), dtype=self._series.dtype, name=self._series.name
             )
         )
 
     def sort(
         self,
         *,
-        descending: bool | Sequence[bool] = True,
+        descending: bool | Sequence[bool] = False,
     ) -> PandasSeries:
         ser = self._series
         return self._from_series(
             ser.sort_values(ascending=not descending).rename(self.name)
         )
 
     def alias(self, name: str) -> Self:
@@ -325,7 +324,37 @@
             return self._series
         elif self._implementation == "cudf":  # pragma: no cover
             return self._series.to_pandas()
         elif self._implementation == "modin":  # pragma: no cover
             return self._series._to_pandas()
         msg = f"Unknown implementation: {self._implementation}"  # pragma: no cover
         raise AssertionError(msg)
+
+    @property
+    def str(self) -> PandasSeriesStringNamespace:
+        return PandasSeriesStringNamespace(self)
+
+    @property
+    def dt(self) -> PandasSeriesDateTimeNamespace:
+        return PandasSeriesDateTimeNamespace(self)
+
+
+class PandasSeriesStringNamespace:
+    def __init__(self, series: PandasSeries) -> None:
+        self._series = series
+
+    def ends_with(self, suffix: str) -> PandasSeries:
+        # TODO make a register_expression_call for namespaces
+
+        return self._series._from_series(
+            self._series._series.str.endswith(suffix),
+        )
+
+
+class PandasSeriesDateTimeNamespace:
+    def __init__(self, series: PandasSeries) -> None:
+        self._series = series
+
+    def year(self) -> PandasSeries:
+        return self._series._from_series(
+            self._series._series.dt.year,
+        )
```

### Comparing `narwhals-0.7.8/narwhals/_pandas_like/utils.py` & `narwhals-0.7.9/narwhals/_pandas_like/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from copy import copy
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Iterable
 from typing import TypeVar
 
+from narwhals.dependencies import get_pyarrow
 from narwhals.utils import flatten
 from narwhals.utils import isinstance_or_issubclass
 from narwhals.utils import parse_version
 
 T = TypeVar("T")
 
 if TYPE_CHECKING:
@@ -46,15 +47,15 @@
     if isinstance(other, PandasSeries):
         if other.len() == 1:
             # broadcast
             return other.item()
         if other._series.index is not index and not (other._series.index == index).all():
             msg = (
                 "Narwhals does not support automated index alignment. "
-                "Please reset the index of the Series or DataFrame."
+                "You may need to do a join before this operation."
             )
             raise ValueError(msg)
         return other._series
     return other
 
 
 def validate_dataframe_comparand(index: Any, other: Any) -> Any:
@@ -71,15 +72,15 @@
     if isinstance(other, PandasSeries):
         if other.len() == 1:
             # broadcast
             return item(other._series)
         if other._series.index is not index and not (other._series.index == index).all():
             msg = (
                 "Narwhals does not support automated index alignment. "
-                "Please reset the index of the Series or DataFrame."
+                "You may need to do a join before this operation."
             )
             raise ValueError(msg)
         return other._series
     raise AssertionError("Please report a bug")
 
 
 def maybe_evaluate_expr(df: PandasDataFrame, arg: Any) -> Any:
@@ -288,45 +289,48 @@
     msg = f"Unknown implementation: {implementation}"  # pragma: no cover
     raise TypeError(msg)  # pragma: no cover
 
 
 def translate_dtype(dtype: Any) -> DType:
     from narwhals import dtypes
 
-    if dtype in ("int64", "Int64"):
+    if dtype in ("int64", "Int64", "Int64[pyarrow]"):
         return dtypes.Int64()
-    if dtype == "int32":
+    if dtype in ("int32", "Int32", "Int32[pyarrow]"):
         return dtypes.Int32()
-    if dtype == "int16":
+    if dtype in ("int16", "Int16", "Int16[pyarrow]"):
         return dtypes.Int16()
-    if dtype == "int8":
+    if dtype in ("int8", "Int8", "Int8[pyarrow]"):
         return dtypes.Int8()
-    if dtype == "uint64":
+    if dtype in ("uint64", "UInt64", "UInt64[pyarrow]"):
         return dtypes.UInt64()
-    if dtype == "uint32":
+    if dtype in ("uint32", "UInt32", "UInt32[pyarrow]"):
         return dtypes.UInt32()
-    if dtype == "uint16":
+    if dtype in ("uint16", "UInt16", "UInt16[pyarrow]"):
         return dtypes.UInt16()
-    if dtype == "uint8":
+    if dtype in ("uint8", "UInt8", "UInt8[pyarrow]"):
         return dtypes.UInt8()
-    if dtype in ("float64", "Float64"):
+    if dtype in ("float64", "Float64", "Float64[pyarrow]"):
         return dtypes.Float64()
-    if dtype in ("float32", "Float32"):
+    if dtype in ("float32", "Float32", "Float32[pyarrow]"):
         return dtypes.Float32()
-    if dtype == ("string"):
+    if dtype in ("string", "string[python]", "string[pyarrow]"):
         return dtypes.String()
-    if dtype in ("bool", "boolean"):
+    if dtype in ("bool", "boolean", "boolean[pyarrow]"):
         return dtypes.Boolean()
     if str(dtype).startswith("datetime64"):
+        # todo: different time units and time zones
         return dtypes.Datetime()
     msg = f"Unknown dtype: {dtype}"  # pragma: no cover
     raise AssertionError(msg)
 
 
 def reverse_translate_dtype(dtype: DType | type[DType]) -> Any:
+    # Use the default pandas dtype here
+    # TODO: maybe this could be configurable?
     from narwhals import dtypes
 
     if isinstance_or_issubclass(dtype, dtypes.Float64):
         return "float64"
     if isinstance_or_issubclass(dtype, dtypes.Float32):
         return "float32"
     if isinstance_or_issubclass(dtype, dtypes.Int64):
@@ -342,23 +346,29 @@
     if isinstance_or_issubclass(dtype, dtypes.UInt32):
         return "uint32"
     if isinstance_or_issubclass(dtype, dtypes.UInt16):
         return "uint16"
     if isinstance_or_issubclass(dtype, dtypes.UInt8):
         return "uint8"
     if isinstance_or_issubclass(dtype, dtypes.String):
-        return "object"
+        if get_pyarrow() is not None:
+            return "string[pyarrow]"
+        return "string[python]"  # pragma: no cover
     if isinstance_or_issubclass(dtype, dtypes.Boolean):
         return "bool"
     if isinstance_or_issubclass(dtype, dtypes.Datetime):
+        # todo: different time units and time zones
         return "datetime64[us]"
     msg = f"Unknown dtype: {dtype}"  # pragma: no cover
     raise AssertionError(msg)
 
 
 def validate_indices(series: list[PandasSeries]) -> list[PandasSeries]:
     idx = series[0]._series.index
     for s in series[1:]:
         if s._series.index is not idx and not (s._series.index == idx).all():
-            msg = "Found implicit index alignment, which is not allowed by Narwhals."
+            msg = (
+                "Narwhals does not support automated index alignment. "
+                "You may need to do a join before this operation."
+            )
             raise RuntimeError(msg)
     return series
```

### Comparing `narwhals-0.7.8/tests/test_common.py` & `narwhals-0.7.9/tests/test_common.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,32 @@
 from pandas.testing import assert_series_equal as pd_assert_series_equal
 from polars.testing import assert_series_equal as pl_assert_series_equal
 
 import narwhals as nw
 from tests.utils import compare_dicts
 
 df_pandas = pd.DataFrame({"a": [1, 3, 2], "b": [4, 4, 6], "z": [7.0, 8, 9]})
+df_pandas_nullable = pd.DataFrame(
+    {"a": [1, 3, 2], "b": [4, 4, 6], "z": [7.0, 8, 9]}
+).astype(
+    {
+        "a": "Int64",
+        "b": "Int64",
+        "z": "Float64",
+    }
+)
+df_pandas_pyarrow = pd.DataFrame(
+    {"a": [1, 3, 2], "b": [4, 4, 6], "z": [7.0, 8, 9]}
+).astype(
+    {
+        "a": "Int64[pyarrow]",
+        "b": "Int64[pyarrow]",
+        "z": "Float64[pyarrow]",
+    }
+)
 df_polars = pl.DataFrame({"a": [1, 3, 2], "b": [4, 4, 6], "z": [7.0, 8, 9]})
 df_lazy = pl.LazyFrame({"a": [1, 3, 2], "b": [4, 4, 6], "z": [7.0, 8, 9]})
 df_pandas_na = pd.DataFrame({"a": [None, 3, 2], "b": [4, 4, 6], "z": [7.0, None, 9]})
 df_lazy_na = pl.LazyFrame({"a": [None, 3, 2], "b": [4, 4, 6], "z": [7.0, None, 9]})
 df_right_pandas = pd.DataFrame({"c": [6, 12, -1], "d": [0, -4, 2]})
 df_right_lazy = pl.LazyFrame({"c": [6, 12, -1], "d": [0, -4, 2]})
 
@@ -32,15 +50,15 @@
         )
 else:  # pragma: no cover
     df_mpd = df_pandas.copy()
 
 
 @pytest.mark.parametrize(
     "df_raw",
-    [df_pandas, df_polars, df_lazy],
+    [df_pandas, df_polars, df_lazy, df_pandas_nullable, df_pandas_pyarrow],
 )
 def test_sort(df_raw: Any) -> None:
     df = nw.LazyFrame(df_raw)
     result = df.sort("a", "b")
     result_native = nw.to_native(result)
     expected = {
         "a": [1, 2, 3],
@@ -56,15 +74,15 @@
         "z": [8.0, 9.0, 7.0],
     }
     compare_dicts(result_native, expected)
 
 
 @pytest.mark.parametrize(
     "df_raw",
-    [df_pandas, df_lazy],
+    [df_pandas, df_lazy, df_pandas_nullable, df_pandas_pyarrow],
 )
 def test_filter(df_raw: Any) -> None:
     df = nw.LazyFrame(df_raw)
     result = df.filter(nw.col("a") > 1)
     result_native = nw.to_native(result)
     expected = {"a": [3, 2], "b": [4, 6], "z": [8.0, 9.0]}
     compare_dicts(result_native, expected)
@@ -80,15 +98,15 @@
     result_native = nw.to_native(result)
     expected = {"a": [3, 2], "b": [4, 6], "z": [8.0, 9.0]}
     compare_dicts(result_native, expected)
 
 
 @pytest.mark.parametrize(
     "df_raw",
-    [df_pandas, df_lazy],
+    [df_pandas, df_lazy, df_pandas_nullable, df_pandas_pyarrow],
 )
 def test_add(df_raw: Any) -> None:
     df = nw.LazyFrame(df_raw)
     result = df.with_columns(
         c=nw.col("a") + nw.col("b"),
         d=nw.col("a") - nw.col("a").mean(),
         e=nw.col("a") - nw.col("a").std(),
@@ -103,15 +121,15 @@
         "e": [0.0, 2.0, 1.0],
     }
     compare_dicts(result_native, expected)
 
 
 @pytest.mark.parametrize(
     "df_raw",
-    [df_pandas, df_lazy],
+    [df_pandas, df_lazy, df_pandas_nullable, df_pandas_pyarrow],
 )
 def test_double(df_raw: Any) -> None:
     df = nw.LazyFrame(df_raw)
     result = df.with_columns(nw.all() * 2)
     result_native = nw.to_native(result)
     expected = {"a": [2, 6, 4], "b": [8, 8, 12], "z": [14.0, 16.0, 18.0]}
     compare_dicts(result_native, expected)
@@ -119,62 +137,68 @@
     result_native = nw.to_native(result)
     expected = {"o": [1, 3, 2], "a": [2, 6, 4], "b": [8, 8, 12], "z": [14.0, 16.0, 18.0]}
     compare_dicts(result_native, expected)
 
 
 @pytest.mark.parametrize(
     "df_raw",
-    [df_pandas, df_lazy],
+    [df_pandas, df_lazy, df_pandas_nullable, df_pandas_pyarrow],
 )
 def test_select(df_raw: Any) -> None:
     df = nw.LazyFrame(df_raw)
     result = df.select("a")
     result_native = nw.to_native(result)
     expected = {"a": [1, 3, 2]}
     compare_dicts(result_native, expected)
 
 
-@pytest.mark.parametrize("df_raw", [df_pandas, df_lazy])
+@pytest.mark.parametrize("df_raw", [df_pandas, df_lazy, df_pandas_nullable])
 def test_sumh(df_raw: Any) -> None:
     df = nw.LazyFrame(df_raw)
     result = df.with_columns(horizonal_sum=nw.sum_horizontal(nw.col("a"), nw.col("b")))
     result_native = nw.to_native(result)
     expected = {
         "a": [1, 3, 2],
         "b": [4, 4, 6],
         "z": [7.0, 8.0, 9.0],
         "horizonal_sum": [5, 7, 8],
     }
     compare_dicts(result_native, expected)
 
 
-@pytest.mark.parametrize("df_raw", [df_pandas, df_lazy])
+@pytest.mark.parametrize(
+    "df_raw", [df_pandas, df_lazy, df_pandas_nullable, df_pandas_pyarrow]
+)
 def test_sumh_literal(df_raw: Any) -> None:
     df = nw.LazyFrame(df_raw)
     result = df.with_columns(horizonal_sum=nw.sum_horizontal("a", nw.col("b")))
     result_native = nw.to_native(result)
     expected = {
         "a": [1, 3, 2],
         "b": [4, 4, 6],
         "z": [7.0, 8.0, 9.0],
         "horizonal_sum": [5, 7, 8],
     }
     compare_dicts(result_native, expected)
 
 
-@pytest.mark.parametrize("df_raw", [df_pandas, df_lazy])
+@pytest.mark.parametrize(
+    "df_raw", [df_pandas, df_lazy, df_pandas_nullable, df_pandas_pyarrow]
+)
 def test_sum_all(df_raw: Any) -> None:
     df = nw.LazyFrame(df_raw)
     result = df.select(nw.all().sum())
     result_native = nw.to_native(result)
     expected = {"a": [6], "b": [14], "z": [24.0]}
     compare_dicts(result_native, expected)
 
 
-@pytest.mark.parametrize("df_raw", [df_pandas, df_lazy])
+@pytest.mark.parametrize(
+    "df_raw", [df_pandas, df_lazy, df_pandas_nullable, df_pandas_pyarrow]
+)
 def test_double_selected(df_raw: Any) -> None:
     df = nw.LazyFrame(df_raw)
     result = df.select(nw.col("a", "b") * 2)
     result_native = nw.to_native(result)
     expected = {"a": [2, 6, 4], "b": [8, 8, 12]}
     compare_dicts(result_native, expected)
     result = df.select("z", nw.col("a", "b") * 2)
@@ -183,24 +207,28 @@
     compare_dicts(result_native, expected)
     result = df.select("a").select(nw.col("a") + nw.all())
     result_native = nw.to_native(result)
     expected = {"a": [2, 6, 4]}
     compare_dicts(result_native, expected)
 
 
-@pytest.mark.parametrize("df_raw", [df_pandas, df_lazy])
+@pytest.mark.parametrize(
+    "df_raw", [df_pandas, df_lazy, df_pandas_nullable, df_pandas_pyarrow]
+)
 def test_rename(df_raw: Any) -> None:
     df = nw.LazyFrame(df_raw)
     result = df.rename({"a": "x", "b": "y"})
     result_native = nw.to_native(result)
     expected = {"x": [1, 3, 2], "y": [4, 4, 6], "z": [7.0, 8, 9]}
     compare_dicts(result_native, expected)
 
 
-@pytest.mark.parametrize("df_raw", [df_pandas, df_lazy])
+@pytest.mark.parametrize(
+    "df_raw", [df_pandas, df_lazy, df_pandas_nullable, df_pandas_pyarrow]
+)
 def test_join(df_raw: Any) -> None:
     df = nw.LazyFrame(df_raw)
     df_right = df
     result = df.join(df_right, left_on=["a", "b"], right_on=["a", "b"], how="inner")
     result_native = nw.to_native(result)
     expected = {"a": [1, 3, 2], "b": [4, 4, 6], "z": [7.0, 8, 9], "z_right": [7.0, 8, 9]}
     compare_dicts(result_native, expected)
@@ -216,15 +244,17 @@
         "b_right": [4, 4, 6],
         "z": [7.0, 8, 9],
         "z_right": [7.0, 8, 9],
     }
     compare_dicts(result_native, expected)
 
 
-@pytest.mark.parametrize("df_raw", [df_pandas, df_lazy])
+@pytest.mark.parametrize(
+    "df_raw", [df_pandas, df_lazy, df_pandas_nullable, df_pandas_pyarrow]
+)
 def test_schema(df_raw: Any) -> None:
     result = nw.LazyFrame(df_raw).schema
     expected = {"a": nw.Int64, "b": nw.Int64, "z": nw.Float64}
     assert result == expected
     result = nw.LazyFrame(df_raw).collect().schema
     expected = {"a": nw.Int64, "b": nw.Int64, "z": nw.Float64}
     assert result == expected
@@ -232,15 +262,17 @@
     expected = ["a", "b", "z"]  # type: ignore[assignment]
     assert result == expected
     result = nw.LazyFrame(df_raw).collect().columns  # type: ignore[assignment]
     expected = ["a", "b", "z"]  # type: ignore[assignment]
     assert result == expected
 
 
-@pytest.mark.parametrize("df_raw", [df_pandas, df_lazy])
+@pytest.mark.parametrize(
+    "df_raw", [df_pandas, df_lazy, df_pandas_nullable, df_pandas_pyarrow]
+)
 def test_columns(df_raw: Any) -> None:
     df = nw.LazyFrame(df_raw)
     result = df.columns
     expected = ["a", "b", "z"]
     assert result == expected
 
 
@@ -393,38 +425,45 @@
 
 @pytest.mark.parametrize("df_raw", [df_polars, df_pandas, df_mpd, df_lazy])
 def test_expr_sample(df_raw: Any) -> None:
     df = nw.LazyFrame(df_raw)
     result_shape = nw.to_native(df.select(nw.col("a").sample(n=2)).collect()).shape
     expected = (2, 1)
     assert result_shape == expected
+    result_shape = nw.to_native(df.collect()["a"].sample(n=2)).shape
+    expected = (2,)  # type: ignore[assignment]
+    assert result_shape == expected
 
 
 @pytest.mark.parametrize("df_raw", [df_pandas_na, df_lazy_na])
 def test_expr_na(df_raw: Any) -> None:
     df = nw.LazyFrame(df_raw)
     result_nna = nw.to_native(
-        df.filter((~nw.col("a").is_null()) & (~nw.col("z").is_null()))
+        df.filter((~nw.col("a").is_null()) & (~df.collect()["z"].is_null()))
     )
     expected = {"a": [2], "b": [6], "z": [9]}
     compare_dicts(result_nna, expected)
 
 
-@pytest.mark.parametrize("df_raw", [df_pandas, df_lazy])
+@pytest.mark.parametrize(
+    "df_raw", [df_pandas, df_lazy, df_pandas_nullable, df_pandas_pyarrow]
+)
 def test_head(df_raw: Any) -> None:
     df = nw.LazyFrame(df_raw)
     result = nw.to_native(df.head(2))
     expected = {"a": [1, 3], "b": [4, 4], "z": [7.0, 8.0]}
     compare_dicts(result, expected)
     result = nw.to_native(df.collect().head(2))
     expected = {"a": [1, 3], "b": [4, 4], "z": [7.0, 8.0]}
     compare_dicts(result, expected)
 
 
-@pytest.mark.parametrize("df_raw", [df_pandas, df_lazy])
+@pytest.mark.parametrize(
+    "df_raw", [df_pandas, df_lazy, df_pandas_nullable, df_pandas_pyarrow]
+)
 def test_unique(df_raw: Any) -> None:
     df = nw.LazyFrame(df_raw)
     result = nw.to_native(df.unique("b").sort("b"))
     expected = {"a": [1, 2], "b": [4, 6], "z": [7.0, 9.0]}
     compare_dicts(result, expected)
     result = nw.to_native(df.collect().unique("b").sort("b"))
     expected = {"a": [1, 2], "b": [4, 6], "z": [7.0, 9.0]}
@@ -433,14 +472,17 @@
 
 @pytest.mark.parametrize("df_raw", [df_pandas_na, df_lazy_na])
 def test_drop_nulls(df_raw: Any) -> None:
     df = nw.LazyFrame(df_raw)
     result = nw.to_native(df.select(nw.col("a").drop_nulls()))
     expected = {"a": [3, 2]}
     compare_dicts(result, expected)
+    result = nw.to_native(df.select(df.collect()["a"].drop_nulls()))
+    expected = {"a": [3, 2]}
+    compare_dicts(result, expected)
 
 
 @pytest.mark.parametrize(
     ("df_raw", "df_raw_right"), [(df_pandas, df_right_pandas), (df_lazy, df_right_lazy)]
 )
 def test_concat_horizontal(df_raw: Any, df_raw_right: Any) -> None:
     df_left = nw.LazyFrame(df_raw)
@@ -501,15 +543,17 @@
         "b": pl.Series("b", [4, 4, 6]),
         "z": pl.Series("z", [7.0, 8, 9]),
     }
     for key in expected:
         pl_assert_series_equal(result[key], expected[key])
 
 
-@pytest.mark.parametrize("df_raw", [df_pandas, df_lazy])
+@pytest.mark.parametrize(
+    "df_raw", [df_pandas, df_lazy, df_pandas_nullable, df_pandas_pyarrow]
+)
 def test_any_all(df_raw: Any) -> None:
     df = nw.LazyFrame(df_raw)
     result = nw.to_native(df.select((nw.all() > 1).all()))
     expected = {"a": [False], "b": [True], "z": [True]}
     compare_dicts(result, expected)
     result = nw.to_native(df.select((nw.all() > 1).any()))
     expected = {"a": [True], "b": [True], "z": [True]}
@@ -521,16 +565,18 @@
     with pytest.raises(ValueError, match="Multi-output"):
         df.select(nw.all() + nw.all())
 
 
 @pytest.mark.parametrize("df_raw", [df_pandas])
 def test_reindex(df_raw: Any) -> None:
     df = nw.DataFrame(df_raw)
-    with pytest.raises(RuntimeError, match="implicit index alignment"):
-        df.select("a", df["b"].sort())
+    with pytest.raises(RuntimeError, match="automated index alignment"):
+        df.select("a", df["b"].sort(descending=True))
+    with pytest.raises(RuntimeError, match="automated index alignment"):
+        df.select("a", nw.col("b").sort(descending=True))
 
     s = df["a"]
     with pytest.raises(ValueError, match="index alignment"):
         nw.to_native(s > s.sort())
     with pytest.raises(ValueError, match="index alignment"):
         nw.to_native(df.with_columns(s.sort()))
     with pytest.raises(ValueError, match="Multi-output expressions are not supported"):
```

### Comparing `narwhals-0.7.8/tests/test_dt.py` & `narwhals-0.7.9/tests/test_dt.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,26 @@
 df_pandas = pd.DataFrame(
     {
         "a": [datetime(2020, 1, 1), datetime(2020, 1, 2), datetime(2020, 1, 3)],
         "b": [4, 4, 6],
         "z": [7.0, 8, 9],
     }
 )
+df_pandas_nullable = pd.DataFrame(
+    {
+        "a": [datetime(2020, 1, 1), datetime(2020, 1, 2), datetime(2020, 1, 3)],
+        "b": [4, 4, 6],
+        "z": [7.0, 8, 9],
+    }
+).astype(
+    {
+        "b": "Int64",
+        "z": "Float64",
+    }
+)
 df_polars = pl.DataFrame(
     {
         "a": [datetime(2020, 1, 1), datetime(2020, 1, 2), datetime(2020, 1, 3)],
         "b": [4, 4, 6],
         "z": [7.0, 8, 9],
     }
 )
@@ -29,13 +41,16 @@
         "a": [datetime(2020, 1, 1), datetime(2020, 1, 2), datetime(2020, 1, 3)],
         "b": [4, 4, 6],
         "z": [7.0, 8, 9],
     }
 )
 
 
-@pytest.mark.parametrize("df_raw", [df_pandas, df_lazy])
+@pytest.mark.parametrize("df_raw", [df_pandas, df_lazy, df_pandas_nullable])
 def test_any_all(df_raw: Any) -> None:
     df = nw.LazyFrame(df_raw)
     result = nw.to_native(df.select(nw.col("a").dt.year()))
     expected = {"a": [2020, 2020, 2020]}
     compare_dicts(result, expected)
+    result = nw.to_native(df.select(df.collect()["a"].dt.year()))
+    expected = {"a": [2020, 2020, 2020]}
+    compare_dicts(result, expected)
```

### Comparing `narwhals-0.7.8/tests/test_group_by.py` & `narwhals-0.7.9/tests/test_group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/tests/test_str.py` & `narwhals-0.7.9/tests/test_str.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,7 +32,13 @@
     df = nw.LazyFrame(df_raw)
     result = df.select(nw.col("a").str.ends_with("das"))
     result_native = nw.to_native(result)
     expected = {
         "a": [True, False],
     }
     compare_dicts(result_native, expected)
+    result = df.select(df.collect()["a"].str.ends_with("das"))
+    result_native = nw.to_native(result)
+    expected = {
+        "a": [True, False],
+    }
+    compare_dicts(result_native, expected)
```

### Comparing `narwhals-0.7.8/tests/tpch_q1_test.py` & `narwhals-0.7.9/tests/tpch_q1_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/tests/utils.py` & `narwhals-0.7.9/tests/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/tests/data/customer.parquet` & `narwhals-0.7.9/tests/data/customer.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/tests/data/lineitem.parquet` & `narwhals-0.7.9/tests/data/lineitem.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/tests/data/nation.parquet` & `narwhals-0.7.9/tests/data/nation.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/tests/data/orders.parquet` & `narwhals-0.7.9/tests/data/orders.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/tests/data/part.parquet` & `narwhals-0.7.9/tests/data/part.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/tests/data/partsupp.parquet` & `narwhals-0.7.9/tests/data/partsupp.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/tests/data/region.parquet` & `narwhals-0.7.9/tests/data/region.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/tests/data/supplier.parquet` & `narwhals-0.7.9/tests/data/supplier.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/tpch/q1.py` & `narwhals-0.7.9/tpch/q1.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/tpch/q2.py` & `narwhals-0.7.9/tpch/q2.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/tpch/q3.py` & `narwhals-0.7.9/tpch/q3.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/tpch/q4.py` & `narwhals-0.7.9/tpch/q4.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/tpch/q5.py` & `narwhals-0.7.9/tpch/q5.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/tpch/notebooks/gpu/execute.ipynb` & `narwhals-0.7.9/tpch/notebooks/gpu/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/tpch/notebooks/q1/execute.ipynb` & `narwhals-0.7.9/tpch/notebooks/q6/execute.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984022352430555%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(4, 'def q6(line_item_raw) -> None:\\n'), (5, '    var_1 = "*

 * *            "datetime(1994, 1, 1)\\n'), (6, '    var_2 = datetime(1995, 1, 1)\\n'), (7, '    var_3 "*

 * *            "= 24\\n'), (8, '\\n'), (9, '    line_item_ds = nw.from_native(line_item_raw)\\n'), "*

 * *            "(10, '\\n'), (12, '        line_item_ds.filter(\\n'), (13, '            "*

 * *            'nw.col("l_shipdate").is_between(var_1, var_2, closed="left"),\\n\'), (14, '*

 * *            '\'            nw.col("l_d […]*

```diff
@@ -101,43 +101,32 @@
             },
             "outputs": [],
             "source": [
                 "from typing import Any\n",
                 "from datetime import datetime\n",
                 "import narwhals as nw\n",
                 "\n",
-                "def q1(df_raw: Any) -> Any:\n",
-                "    var_1 = datetime(1998, 9, 2)\n",
-                "    df = nw.from_native(df_raw)\n",
+                "def q6(line_item_raw) -> None:\n",
+                "    var_1 = datetime(1994, 1, 1)\n",
+                "    var_2 = datetime(1995, 1, 1)\n",
+                "    var_3 = 24\n",
+                "\n",
+                "    line_item_ds = nw.from_native(line_item_raw)\n",
+                "\n",
                 "    result = (\n",
-                "        df.filter(nw.col(\"l_shipdate\") <= var_1)\n",
-                "        .with_columns(\n",
-                "            disc_price=nw.col(\"l_extendedprice\") * (1 - nw.col(\"l_discount\")),\n",
-                "            charge=(\n",
-                "                nw.col(\"l_extendedprice\")\n",
-                "                * (1.0 - nw.col(\"l_discount\"))\n",
-                "                * (1.0 + nw.col(\"l_tax\"))\n",
-                "            ),\n",
-                "        )\n",
-                "        .group_by([\"l_returnflag\", \"l_linestatus\"])\n",
-                "        .agg(\n",
-                "            [\n",
-                "                nw.sum(\"l_quantity\").alias(\"sum_qty\"),\n",
-                "                nw.sum(\"l_extendedprice\").alias(\"sum_base_price\"),\n",
-                "                nw.sum(\"disc_price\").alias(\"sum_disc_price\"),\n",
-                "                nw.col(\"charge\").sum().alias(\"sum_charge\"),\n",
-                "                nw.mean(\"l_quantity\").alias(\"avg_qty\"),\n",
-                "                nw.mean(\"l_extendedprice\").alias(\"avg_price\"),\n",
-                "                nw.mean(\"l_discount\").alias(\"avg_disc\"),\n",
-                "                nw.len().alias(\"count_order\"),\n",
-                "            ],\n",
+                "        line_item_ds.filter(\n",
+                "            nw.col(\"l_shipdate\").is_between(var_1, var_2, closed=\"left\"),\n",
+                "            nw.col(\"l_discount\").is_between(0.05, 0.07),\n",
+                "            nw.col(\"l_quantity\") < var_3,\n",
+                "        ).with_columns(\n",
+                "            (nw.col(\"l_extendedprice\") * nw.col(\"l_discount\")).alias(\"revenue\")\n",
                 "        )\n",
-                "        .sort([\"l_returnflag\", \"l_linestatus\"])\n",
+                "        .select(nw.sum(\"revenue\"))\n",
                 "    )\n",
-                "    return nw.to_native(result)"
+                "    return nw.to_native(result)\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "8d540303",
             "metadata": {
@@ -264,15 +253,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'pandas'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q1(fn(lineitem))\n",
+                "timings = %timeit -o q6(fn(lineitem))\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0b561017",
             "metadata": {
@@ -327,15 +316,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'pandas[pyarrow]'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q1(fn(lineitem))\n",
+                "timings = %timeit -o q6(fn(lineitem))\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a8005d7d",
             "metadata": {
@@ -390,15 +379,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'polars[eager]'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q1(fn(lineitem))\n",
+                "timings = %timeit -o q6(fn(lineitem))\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c77a701f",
             "metadata": {
@@ -453,15 +442,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'polars[lazy]'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q1(fn(lineitem)).collect()\n",
+                "timings = %timeit -o q6(fn(lineitem)).collect()\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "37ce6bf3",
             "metadata": {},
```

### Comparing `narwhals-0.7.8/tpch/notebooks/q2/execute.ipynb` & `narwhals-0.7.9/tpch/notebooks/q5/execute.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984389630149813%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(4, 'def q5(\\n'), (7, '    customer_ds_raw: Any,\\n'), (8, "*

 * *            "'    lineitem_ds_raw: Any,\\n'), (9, '    orders_ds_raw: Any,\\n'), (12, '    var_1 = "*

 * *            '"ASIA"\\n\'), (13, \'    var_2 = datetime(1994, 1, 1)\\n\'), (14, \'    var_3 = '*

 * *            "datetime(1995, 1, 1)\\n'), (18, '    customer_ds = "*

 * *            "nw.from_native(customer_ds_raw)\\n'), (19, '    line_item_ds = "*

 * *            "nw.from_native(lineitem_ds_raw)\\n'), (20, '    orders_ds = […]*

```diff
@@ -101,71 +101,56 @@
             },
             "outputs": [],
             "source": [
                 "from typing import Any\n",
                 "from datetime import datetime\n",
                 "import narwhals as nw\n",
                 "\n",
-                "def q2(\n",
+                "def q5(\n",
                 "    region_ds_raw: Any,\n",
                 "    nation_ds_raw: Any,\n",
+                "    customer_ds_raw: Any,\n",
+                "    lineitem_ds_raw: Any,\n",
+                "    orders_ds_raw: Any,\n",
                 "    supplier_ds_raw: Any,\n",
-                "    part_ds_raw: Any,\n",
-                "    part_supp_ds_raw: Any,\n",
                 ") -> Any:\n",
-                "    var_1 = 15\n",
-                "    var_2 = \"BRASS\"\n",
-                "    var_3 = \"EUROPE\"\n",
+                "    var_1 = \"ASIA\"\n",
+                "    var_2 = datetime(1994, 1, 1)\n",
+                "    var_3 = datetime(1995, 1, 1)\n",
                 "\n",
                 "    region_ds = nw.from_native(region_ds_raw)\n",
                 "    nation_ds = nw.from_native(nation_ds_raw)\n",
+                "    customer_ds = nw.from_native(customer_ds_raw)\n",
+                "    line_item_ds = nw.from_native(lineitem_ds_raw)\n",
+                "    orders_ds = nw.from_native(orders_ds_raw)\n",
                 "    supplier_ds = nw.from_native(supplier_ds_raw)\n",
-                "    part_ds = nw.from_native(part_ds_raw)\n",
-                "    part_supp_ds = nw.from_native(part_supp_ds_raw)\n",
                 "\n",
-                "    result_q2 = (\n",
-                "        part_ds.join(part_supp_ds, left_on=\"p_partkey\", right_on=\"ps_partkey\")\n",
-                "        .join(supplier_ds, left_on=\"ps_suppkey\", right_on=\"s_suppkey\")\n",
-                "        .join(nation_ds, left_on=\"s_nationkey\", right_on=\"n_nationkey\")\n",
-                "        .join(region_ds, left_on=\"n_regionkey\", right_on=\"r_regionkey\")\n",
-                "        .filter(\n",
-                "            nw.col(\"p_size\") == var_1,\n",
-                "            nw.col(\"p_type\").str.ends_with(var_2),\n",
-                "            nw.col(\"r_name\") == var_3,\n",
-                "        )\n",
-                "    )\n",
-                "\n",
-                "    final_cols = [\n",
-                "        \"s_acctbal\",\n",
-                "        \"s_name\",\n",
-                "        \"n_name\",\n",
-                "        \"p_partkey\",\n",
-                "        \"p_mfgr\",\n",
-                "        \"s_address\",\n",
-                "        \"s_phone\",\n",
-                "        \"s_comment\",\n",
-                "    ]\n",
-                "\n",
-                "    q_final = (\n",
-                "        result_q2.group_by(\"p_partkey\")\n",
-                "        .agg(nw.min(\"ps_supplycost\").alias(\"ps_supplycost\"))\n",
+                "    result = (\n",
+                "        region_ds.join(nation_ds, left_on=\"r_regionkey\", right_on=\"n_regionkey\")\n",
+                "        .join(customer_ds, left_on=\"n_nationkey\", right_on=\"c_nationkey\")\n",
+                "        .join(orders_ds, left_on=\"c_custkey\", right_on=\"o_custkey\")\n",
+                "        .join(line_item_ds, left_on=\"o_orderkey\", right_on=\"l_orderkey\")\n",
                 "        .join(\n",
-                "            result_q2,\n",
-                "            left_on=[\"p_partkey\", \"ps_supplycost\"],\n",
-                "            right_on=[\"p_partkey\", \"ps_supplycost\"],\n",
+                "            supplier_ds,\n",
+                "            left_on=[\"l_suppkey\", \"n_nationkey\"],\n",
+                "            right_on=[\"s_suppkey\", \"s_nationkey\"],\n",
+                "        )\n",
+                "        .filter(\n",
+                "            nw.col(\"r_name\") == var_1,\n",
+                "            nw.col(\"o_orderdate\").is_between(var_2, var_3, closed=\"left\")\n",
                 "        )\n",
-                "        .select(final_cols)\n",
-                "        .sort(\n",
-                "            by=[\"s_acctbal\", \"n_name\", \"s_name\", \"p_partkey\"],\n",
-                "            descending=[True, False, False, False],\n",
+                "        .with_columns(\n",
+                "            (nw.col(\"l_extendedprice\") * (1 - nw.col(\"l_discount\"))).alias(\"revenue\")\n",
                 "        )\n",
-                "        .head(100)\n",
+                "        .group_by(\"n_name\")\n",
+                "        .agg([nw.sum(\"revenue\")])\n",
+                "        .sort(by=\"revenue\", descending=True)\n",
                 "    )\n",
                 "\n",
-                "    return nw.to_native(q_final)"
+                "    return nw.to_native(result)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "8d540303",
             "metadata": {
@@ -292,15 +277,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'pandas'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q2(fn(region), fn(nation), fn(supplier), fn(part), fn(partsupp))\n",
+                "timings = %timeit -o q5(fn(region), fn(nation), fn(customer), fn(lineitem), fn(orders), fn(supplier))\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0b561017",
             "metadata": {
@@ -355,15 +340,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'pandas[pyarrow]'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q2(fn(region), fn(nation), fn(supplier), fn(part), fn(partsupp))\n",
+                "timings = %timeit -o q5(fn(region), fn(nation), fn(customer), fn(lineitem), fn(orders), fn(supplier))\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a8005d7d",
             "metadata": {
@@ -418,15 +403,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'polars[eager]'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q2(fn(region), fn(nation), fn(supplier), fn(part), fn(partsupp))\n",
+                "timings = %timeit -o q5(fn(region), fn(nation), fn(customer), fn(lineitem), fn(orders), fn(supplier))\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c77a701f",
             "metadata": {
@@ -481,15 +466,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'polars[lazy]'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q2(fn(region), fn(nation), fn(supplier), fn(part), fn(partsupp)).collect()\n",
+                "timings = %timeit -o q5(fn(region), fn(nation), fn(customer), fn(lineitem), fn(orders), fn(supplier)).collect()\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "37ce6bf3",
             "metadata": {},
```

### Comparing `narwhals-0.7.8/tpch/notebooks/q3/execute.ipynb` & `narwhals-0.7.9/tpch/notebooks/q3/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/tpch/notebooks/q4/execute.ipynb` & `narwhals-0.7.9/tpch/notebooks/q4/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/tpch/notebooks/q5/execute.ipynb` & `narwhals-0.7.9/tpch/notebooks/q1/execute.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9789082080200502%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(4, 'def q1(df_raw: Any) -> Any:\\n'), (5, '    var_1 = "*

 * *            "datetime(1998, 9, 2)\\n'), (6, '    df = nw.from_native(df_raw)\\n'), (8, '        "*

 * *            'df.filter(nw.col("l_shipdate") <= var_1)\\n\'), (10, \'            '*

 * *            'disc_price=nw.col("l_extendedprice") * (1 - nw.col("l_discount")),\\n\'), (11, '*

 * *            '\'            charge=(\\n\'), (12, \'                nw.col("l_extendedprice")\\n\'), '*

 * *            '(13, \'                * (1. […]*

```diff
@@ -77,14 +77,58 @@
                 "\n",
                 "pd.options.mode.copy_on_write = True\n",
                 "pd.options.future.infer_string = True"
             ]
         },
         {
             "cell_type": "code",
+            "execution_count": null,
+            "id": "bf899a79",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from datetime import date\n",
+                "\n",
+                "def q1_pandas_native(lineitem):\n",
+                "    VAR1 = date(1998, 9, 2)\n",
+                "\n",
+                "    sel = lineitem.l_shipdate <= VAR1\n",
+                "    lineitem_filtered = lineitem[sel]\n",
+                "\n",
+                "    # This is lenient towards pandas as normally an optimizer should decide\n",
+                "    # that this could be computed before the groupby aggregation.\n",
+                "    # Other implementations don't enjoy this benefit.\n",
+                "    lineitem_filtered[\"disc_price\"] = lineitem_filtered.l_extendedprice * (\n",
+                "        1 - lineitem_filtered.l_discount\n",
+                "    )\n",
+                "    lineitem_filtered[\"charge\"] = (\n",
+                "        lineitem_filtered.l_extendedprice\n",
+                "        * (1 - lineitem_filtered.l_discount)\n",
+                "        * (1 + lineitem_filtered.l_tax)\n",
+                "    )\n",
+                "    gb = lineitem_filtered.groupby([\"l_returnflag\", \"l_linestatus\"], as_index=False)\n",
+                "\n",
+                "    total = gb.agg(\n",
+                "        sum_qty=pd.NamedAgg(column=\"l_quantity\", aggfunc=\"sum\"),\n",
+                "        sum_base_price=pd.NamedAgg(column=\"l_extendedprice\", aggfunc=\"sum\"),\n",
+                "        sum_disc_price=pd.NamedAgg(column=\"disc_price\", aggfunc=\"sum\"),\n",
+                "        sum_charge=pd.NamedAgg(column=\"charge\", aggfunc=\"sum\"),\n",
+                "        avg_qty=pd.NamedAgg(column=\"l_quantity\", aggfunc=\"mean\"),\n",
+                "        avg_price=pd.NamedAgg(column=\"l_extendedprice\", aggfunc=\"mean\"),\n",
+                "        avg_disc=pd.NamedAgg(column=\"l_discount\", aggfunc=\"mean\"),\n",
+                "        count_order=pd.NamedAgg(column=\"l_orderkey\", aggfunc=\"size\"),\n",
+                "    )\n",
+                "\n",
+                "    result_df = total.sort_values([\"l_returnflag\", \"l_linestatus\"])\n",
+                "\n",
+                "    return result_df  # type: ignore[no-any-return]"
+            ]
+        },
+        {
+            "cell_type": "code",
             "execution_count": 4,
             "id": "42e7f0e2",
             "metadata": {
                 "execution": {
                     "iopub.execute_input": "2024-03-22T17:24:39.066341Z",
                     "iopub.status.busy": "2024-03-22T17:24:39.065881Z",
                     "iopub.status.idle": "2024-03-22T17:24:39.078875Z",
@@ -101,55 +145,42 @@
             },
             "outputs": [],
             "source": [
                 "from typing import Any\n",
                 "from datetime import datetime\n",
                 "import narwhals as nw\n",
                 "\n",
-                "def q5(\n",
-                "    region_ds_raw: Any,\n",
-                "    nation_ds_raw: Any,\n",
-                "    customer_ds_raw: Any,\n",
-                "    lineitem_ds_raw: Any,\n",
-                "    orders_ds_raw: Any,\n",
-                "    supplier_ds_raw: Any,\n",
-                ") -> Any:\n",
-                "    var_1 = \"ASIA\"\n",
-                "    var_2 = datetime(1994, 1, 1)\n",
-                "    var_3 = datetime(1995, 1, 1)\n",
-                "\n",
-                "    region_ds = nw.from_native(region_ds_raw)\n",
-                "    nation_ds = nw.from_native(nation_ds_raw)\n",
-                "    customer_ds = nw.from_native(customer_ds_raw)\n",
-                "    line_item_ds = nw.from_native(lineitem_ds_raw)\n",
-                "    orders_ds = nw.from_native(orders_ds_raw)\n",
-                "    supplier_ds = nw.from_native(supplier_ds_raw)\n",
-                "\n",
+                "def q1(df_raw: Any) -> Any:\n",
+                "    var_1 = datetime(1998, 9, 2)\n",
+                "    df = nw.from_native(df_raw)\n",
                 "    result = (\n",
-                "        region_ds.join(nation_ds, left_on=\"r_regionkey\", right_on=\"n_regionkey\")\n",
-                "        .join(customer_ds, left_on=\"n_nationkey\", right_on=\"c_nationkey\")\n",
-                "        .join(orders_ds, left_on=\"c_custkey\", right_on=\"o_custkey\")\n",
-                "        .join(line_item_ds, left_on=\"o_orderkey\", right_on=\"l_orderkey\")\n",
-                "        .join(\n",
-                "            supplier_ds,\n",
-                "            left_on=[\"l_suppkey\", \"n_nationkey\"],\n",
-                "            right_on=[\"s_suppkey\", \"s_nationkey\"],\n",
-                "        )\n",
-                "        .filter(\n",
-                "            nw.col(\"r_name\") == var_1,\n",
-                "            nw.col(\"o_orderdate\").is_between(var_2, var_3, closed=\"left\")\n",
-                "        )\n",
+                "        df.filter(nw.col(\"l_shipdate\") <= var_1)\n",
                 "        .with_columns(\n",
-                "            (nw.col(\"l_extendedprice\") * (1 - nw.col(\"l_discount\"))).alias(\"revenue\")\n",
+                "            disc_price=nw.col(\"l_extendedprice\") * (1 - nw.col(\"l_discount\")),\n",
+                "            charge=(\n",
+                "                nw.col(\"l_extendedprice\")\n",
+                "                * (1.0 - nw.col(\"l_discount\"))\n",
+                "                * (1.0 + nw.col(\"l_tax\"))\n",
+                "            ),\n",
                 "        )\n",
-                "        .group_by(\"n_name\")\n",
-                "        .agg([nw.sum(\"revenue\")])\n",
-                "        .sort(by=\"revenue\", descending=True)\n",
+                "        .group_by([\"l_returnflag\", \"l_linestatus\"])\n",
+                "        .agg(\n",
+                "            [\n",
+                "                nw.sum(\"l_quantity\").alias(\"sum_qty\"),\n",
+                "                nw.sum(\"l_extendedprice\").alias(\"sum_base_price\"),\n",
+                "                nw.sum(\"disc_price\").alias(\"sum_disc_price\"),\n",
+                "                nw.col(\"charge\").sum().alias(\"sum_charge\"),\n",
+                "                nw.mean(\"l_quantity\").alias(\"avg_qty\"),\n",
+                "                nw.mean(\"l_extendedprice\").alias(\"avg_price\"),\n",
+                "                nw.mean(\"l_discount\").alias(\"avg_disc\"),\n",
+                "                nw.len().alias(\"count_order\"),\n",
+                "            ],\n",
+                "        )\n",
+                "        .sort([\"l_returnflag\", \"l_linestatus\"])\n",
                 "    )\n",
-                "\n",
                 "    return nw.to_native(result)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "8d540303",
@@ -220,14 +251,52 @@
             "outputs": [],
             "source": [
                 "results = {}"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "64b20949",
+            "metadata": {},
+            "source": [
+                "## pandas, pyarrow dtypes, native"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "1b63cf0e",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "24 s \u00b1 142 ms per loop (mean \u00b1 std. dev. of 7 runs, 1 loop each)\n"
+                    ]
+                },
+                {
+                    "data": {
+                        "text/plain": [
+                            "23.841894793999984"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "tool = 'pandas[pyarrow]'\n",
+                "fn = IO_FUNCS[tool]\n",
+                "timings = %timeit -o q1_pandas_native(fn(lineitem))\n",
+                "results[tool+'native'] = timings.best"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "09249944",
             "metadata": {
                 "papermill": {
                     "duration": 0.005113,
                     "end_time": "2024-03-22T17:24:39.130472",
                     "exception": false,
                     "start_time": "2024-03-22T17:24:39.125359",
@@ -277,15 +346,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'pandas'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q5(fn(region), fn(nation), fn(customer), fn(lineitem), fn(orders), fn(supplier))\n",
+                "timings = %timeit -o q1(fn(lineitem))\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0b561017",
             "metadata": {
@@ -340,15 +409,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'pandas[pyarrow]'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q5(fn(region), fn(nation), fn(customer), fn(lineitem), fn(orders), fn(supplier))\n",
+                "timings = %timeit -o q1(fn(lineitem))\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a8005d7d",
             "metadata": {
@@ -403,15 +472,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'polars[eager]'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q5(fn(region), fn(nation), fn(customer), fn(lineitem), fn(orders), fn(supplier))\n",
+                "timings = %timeit -o q1(fn(lineitem))\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c77a701f",
             "metadata": {
@@ -466,15 +535,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'polars[lazy]'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q5(fn(region), fn(nation), fn(customer), fn(lineitem), fn(orders), fn(supplier)).collect()\n",
+                "timings = %timeit -o q1(fn(lineitem)).collect()\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "37ce6bf3",
             "metadata": {},
```

### Comparing `narwhals-0.7.8/tpch/notebooks/q7/execute.ipynb` & `narwhals-0.7.9/tpch/notebooks/q7/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/utils/bump_version.py` & `narwhals-0.7.9/utils/bump_version.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/LICENSE.md` & `narwhals-0.7.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/README.md` & `narwhals-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.8/pyproject.toml` & `narwhals-0.7.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "narwhals"
-version = "0.7.8"
+version = "0.7.9"
 authors = [
   { name="Marco Gorelli", email="33491632+MarcoGorelli@users.noreply.github.com" },
 ]
 description = "Extremely lightweight compatibility layer between pandas, Polars, cuDF, and Modin"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `narwhals-0.7.8/PKG-INFO` & `narwhals-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: narwhals
-Version: 0.7.8
+Version: 0.7.9
 Summary: Extremely lightweight compatibility layer between pandas, Polars, cuDF, and Modin
 Project-URL: Homepage, https://github.com/MarcoGorelli/narwhals
 Project-URL: Bug Tracker, https://github.com/MarcoGorelli/narwhals
 Author-email: Marco Gorelli <33491632+MarcoGorelli@users.noreply.github.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

