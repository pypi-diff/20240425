# Comparing `tmp/mypy-boto3-s3-1.34.65.tar.gz` & `tmp/mypy_boto3_s3-1.34.91-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-s3-1.34.65.tar", last modified: Mon Mar 18 20:47:31 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

