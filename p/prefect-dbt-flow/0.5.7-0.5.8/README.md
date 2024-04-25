# Comparing `tmp/prefect_dbt_flow-0.5.7.tar.gz` & `tmp/prefect_dbt_flow-0.5.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_dbt_flow-0.5.7.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

