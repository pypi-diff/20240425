# Comparing `tmp/document_merge_service-6.4.4.tar.gz` & `tmp/document_merge_service-6.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "document_merge_service-6.4.4.tar", max compression
+gzip compressed data, was "document_merge_service-6.4.5.tar", max compression
```

## Comparing `document_merge_service-6.4.4.tar` & `document_merge_service-6.4.5.tar`

### file list

```diff
@@ -1,76 +1,77 @@
--rw-r--r--   0        0        0    13252 2024-01-24 13:15:06.596809 document_merge_service-6.4.4/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2024-01-24 13:15:06.596809 document_merge_service-6.4.4/LICENSE
--rw-r--r--   0        0        0     2522 2024-01-24 13:15:06.596809 document_merge_service-6.4.4/README.md
--rw-r--r--   0        0        0        0 2024-01-24 13:15:06.596809 document_merge_service-6.4.4/document_merge_service/__init__.py
--rw-r--r--   0        0        0        0 2024-01-24 13:15:06.596809 document_merge_service-6.4.4/document_merge_service/api/__init__.py
--rw-r--r--   0        0        0      405 2024-01-24 13:15:06.596809 document_merge_service-6.4.4/document_merge_service/api/apps.py
--rw-r--r--   0        0        0     3232 2024-01-24 13:15:06.596809 document_merge_service-6.4.4/document_merge_service/api/authentication.py
--rw-r--r--   0        0        0     5490 2024-01-24 13:15:06.596809 document_merge_service-6.4.4/document_merge_service/api/data/2023.test.test.docx-template.docx
--rw-r--r--   0        0        0      580 2024-01-24 13:15:06.596809 document_merge_service-6.4.4/document_merge_service/api/data/__init__.py
--rw-r--r--   0        0        0      559 2024-01-24 13:15:06.596809 document_merge_service-6.4.4/document_merge_service/api/data/black.png
--rw-r--r--   0        0        0     9125 2024-01-24 13:15:06.596809 document_merge_service-6.4.4/document_merge_service/api/data/docx-mailmerge-syntax.docx
--rw-r--r--   0        0        0    11489 2024-01-24 13:15:06.596809 document_merge_service-6.4.4/document_merge_service/api/data/docx-mailmerge.docx
--rw-r--r--   0        0        0     5735 2024-01-24 13:15:06.596809 document_merge_service-6.4.4/document_merge_service/api/data/docx-template-filters.docx
--rw-r--r--   0        0        0     6087 2024-01-24 13:15:06.596809 document_merge_service-6.4.4/document_merge_service/api/data/docx-template-loopcontrols.docx
--rw-r--r--   0        0        0     5952 2024-01-24 13:15:06.596809 document_merge_service-6.4.4/document_merge_service/api/data/docx-template-placeholdercheck.docx
--rw-r--r--   0        0        0     5091 2024-01-24 13:15:06.596809 document_merge_service-6.4.4/document_merge_service/api/data/docx-template-syntax.docx
--rw-r--r--   0        0        0     5490 2024-01-24 13:15:06.596809 document_merge_service-6.4.4/document_merge_service/api/data/docx-template.docx
--rw-r--r--   0        0        0     4750 2024-01-24 13:15:06.596809 document_merge_service-6.4.4/document_merge_service/api/data/invalid-template.xlsx
--rw-r--r--   0        0        0  1127936 2024-01-24 13:15:06.600809 document_merge_service-6.4.4/document_merge_service/api/data/loadtest/1.doc
--rw-r--r--   0        0        0   175922 2024-01-24 13:15:06.600809 document_merge_service-6.4.4/document_merge_service/api/data/loadtest/2.docx
--rw-r--r--   0        0        0   163307 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/data/loadtest/3.docx
--rw-r--r--   0        0        0   141498 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/data/loadtest/4.docx
--rw-r--r--   0        0        0    10589 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/data/odt-template.odt
--rw-r--r--   0        0        0       22 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/data/test.txt
--rw-r--r--   0        0        0        5 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/data/xlsx-not-valid.xlsx
--rw-r--r--   0        0        0     6467 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/data/xlsx-structure.xlsx
--rw-r--r--   0        0        0     6432 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/data/xlsx-syntax.xlsx
--rw-r--r--   0        0        0     4750 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/data/xlsx-template.xlsx
--rw-r--r--   0        0        0     9772 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/engines.py
--rw-r--r--   0        0        0      389 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/factories.py
--rw-r--r--   0        0        0      815 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/file_converter.py
--rw-r--r--   0        0        0     2841 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/filters.py
--rw-r--r--   0        0        0     2546 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/jinja.py
--rw-r--r--   0        0        0        0 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/management/__init__.py
--rw-r--r--   0        0        0        0 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/management/commands/__init__.py
--rw-r--r--   0        0        0     1628 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/management/commands/clean_dangling_files.py
--rw-r--r--   0        0        0     2252 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/management/commands/upload_local_templates.py
--rw-r--r--   0        0        0     1248 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/migrations/0001_initial.py
--rw-r--r--   0        0        0      488 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/migrations/0002_template_group.py
--rw-r--r--   0        0        0      374 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/migrations/0003_template_meta.py
--rw-r--r--   0        0        0      145 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/migrations/0004_cleanup_files.py
--rw-r--r--   0        0        0     1004 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/migrations/0005_xlsx_template_engine.py
--rw-r--r--   0        0        0      932 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/migrations/0006_remove_template_group.py
--rw-r--r--   0        0        0        0 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/migrations/__init__.py
--rw-r--r--   0        0        0     1845 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/models.py
--rw-r--r--   0        0        0      231 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/pagination.py
--rw-r--r--   0        0        0      289 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/permissions.py
--rw-r--r--   0        0        0     4995 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/serializers.py
--rw-r--r--   0        0        0        0 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/tests/__init__.py
--rw-r--r--   0        0        0    30689 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/tests/__snapshots__/test_template.ambr
--rw-r--r--   0        0        0     2357 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/tests/test_authentication.py
--rw-r--r--   0        0        0      942 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/tests/test_clean_dangling_files.py
--rw-r--r--   0        0        0     1446 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/tests/test_convert.py
--rw-r--r--   0        0        0     1963 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/tests/test_excel.py
--rw-r--r--   0        0        0     1372 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/tests/test_filters.py
--rw-r--r--   0        0        0     1300 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/tests/test_jinja.py
--rw-r--r--   0        0        0      749 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/tests/test_pagination.py
--rw-r--r--   0        0        0    25634 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/tests/test_template.py
--rw-r--r--   0        0        0     3425 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/tests/test_unoconv.py
--rw-r--r--   0        0        0     1712 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/tests/test_upload_local_templates.py
--rw-r--r--   0        0        0     6947 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/unoconv.py
--rw-r--r--   0        0        0      460 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/urls.py
--rw-r--r--   0        0        0     3797 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/api/views.py
--rw-r--r--   0        0        0     2909 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/conftest.py
--rw-r--r--   0        0        0        0 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/extensions/__init__.py
--rw-r--r--   0        0        0       52 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/extensions/permissions.py
--rw-r--r--   0        0        0       52 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/extensions/visibilities.py
--rw-r--r--   0        0        0      789 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/sentry.py
--rw-r--r--   0        0        0     9052 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/settings.py
--rw-r--r--   0        0        0        0 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/tests/__init__.py
--rw-r--r--   0        0        0      434 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/tests/test_sentry.py
--rw-r--r--   0        0        0      615 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/tests/test_settings.py
--rw-r--r--   0        0        0      225 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/urls.py
--rw-r--r--   0        0        0      412 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/document_merge_service/wsgi.py
--rw-r--r--   0        0        0     3594 2024-01-24 13:15:06.604809 document_merge_service-6.4.4/pyproject.toml
--rw-r--r--   0        0        0     4555 1970-01-01 00:00:00.000000 document_merge_service-6.4.4/PKG-INFO
+-rw-r--r--   0        0        0    13469 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/LICENSE
+-rw-r--r--   0        0        0     2522 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/api/__init__.py
+-rw-r--r--   0        0        0      405 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/api/apps.py
+-rw-r--r--   0        0        0     3232 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/api/authentication.py
+-rw-r--r--   0        0        0     5490 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/api/data/2023.test.test.docx-template.docx
+-rw-r--r--   0        0        0      580 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/api/data/__init__.py
+-rw-r--r--   0        0        0      559 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/api/data/black.png
+-rw-r--r--   0        0        0     9125 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/api/data/docx-mailmerge-syntax.docx
+-rw-r--r--   0        0        0    11489 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/api/data/docx-mailmerge.docx
+-rw-r--r--   0        0        0     5735 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/api/data/docx-template-filters.docx
+-rw-r--r--   0        0        0     7335 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/api/data/docx-template-image-placeholder-header-footer.docx
+-rw-r--r--   0        0        0     6087 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/api/data/docx-template-loopcontrols.docx
+-rw-r--r--   0        0        0     5952 2024-04-25 13:27:33.153890 document_merge_service-6.4.5/document_merge_service/api/data/docx-template-placeholdercheck.docx
+-rw-r--r--   0        0        0     5091 2024-04-25 13:27:33.153890 document_merge_service-6.4.5/document_merge_service/api/data/docx-template-syntax.docx
+-rw-r--r--   0        0        0     5490 2024-04-25 13:27:33.153890 document_merge_service-6.4.5/document_merge_service/api/data/docx-template.docx
+-rw-r--r--   0        0        0     4750 2024-04-25 13:27:33.153890 document_merge_service-6.4.5/document_merge_service/api/data/invalid-template.xlsx
+-rw-r--r--   0        0        0  1127936 2024-04-25 13:27:33.153890 document_merge_service-6.4.5/document_merge_service/api/data/loadtest/1.doc
+-rw-r--r--   0        0        0   175922 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/data/loadtest/2.docx
+-rw-r--r--   0        0        0   163307 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/data/loadtest/3.docx
+-rw-r--r--   0        0        0   141498 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/data/loadtest/4.docx
+-rw-r--r--   0        0        0    10589 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/data/odt-template.odt
+-rw-r--r--   0        0        0       22 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/data/test.txt
+-rw-r--r--   0        0        0        5 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/data/xlsx-not-valid.xlsx
+-rw-r--r--   0        0        0     6467 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/data/xlsx-structure.xlsx
+-rw-r--r--   0        0        0     6432 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/data/xlsx-syntax.xlsx
+-rw-r--r--   0        0        0     4750 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/data/xlsx-template.xlsx
+-rw-r--r--   0        0        0    10586 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/engines.py
+-rw-r--r--   0        0        0      389 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/factories.py
+-rw-r--r--   0        0        0      815 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/file_converter.py
+-rw-r--r--   0        0        0     2841 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/filters.py
+-rw-r--r--   0        0        0     2546 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/jinja.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/management/commands/__init__.py
+-rw-r--r--   0        0        0     1628 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/management/commands/clean_dangling_files.py
+-rw-r--r--   0        0        0     2252 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/management/commands/upload_local_templates.py
+-rw-r--r--   0        0        0     1248 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/migrations/0001_initial.py
+-rw-r--r--   0        0        0      488 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/migrations/0002_template_group.py
+-rw-r--r--   0        0        0      374 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/migrations/0003_template_meta.py
+-rw-r--r--   0        0        0      145 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/migrations/0004_cleanup_files.py
+-rw-r--r--   0        0        0     1004 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/migrations/0005_xlsx_template_engine.py
+-rw-r--r--   0        0        0      932 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/migrations/0006_remove_template_group.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/migrations/__init__.py
+-rw-r--r--   0        0        0     1845 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/models.py
+-rw-r--r--   0        0        0      231 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/pagination.py
+-rw-r--r--   0        0        0      289 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/permissions.py
+-rw-r--r--   0        0        0     4995 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/serializers.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/__init__.py
+-rw-r--r--   0        0        0    30689 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/__snapshots__/test_template.ambr
+-rw-r--r--   0        0        0     2357 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/test_authentication.py
+-rw-r--r--   0        0        0      942 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/test_clean_dangling_files.py
+-rw-r--r--   0        0        0     1446 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/test_convert.py
+-rw-r--r--   0        0        0     1963 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/test_excel.py
+-rw-r--r--   0        0        0     1372 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/test_filters.py
+-rw-r--r--   0        0        0     1300 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/test_jinja.py
+-rw-r--r--   0        0        0      749 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/test_pagination.py
+-rw-r--r--   0        0        0    25891 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/test_template.py
+-rw-r--r--   0        0        0     3425 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/test_unoconv.py
+-rw-r--r--   0        0        0     1712 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/test_upload_local_templates.py
+-rw-r--r--   0        0        0     6947 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/unoconv.py
+-rw-r--r--   0        0        0      460 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/api/urls.py
+-rw-r--r--   0        0        0     3797 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/api/views.py
+-rw-r--r--   0        0        0     2909 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/extensions/__init__.py
+-rw-r--r--   0        0        0       52 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/extensions/permissions.py
+-rw-r--r--   0        0        0       52 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/extensions/visibilities.py
+-rw-r--r--   0        0        0      789 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/sentry.py
+-rw-r--r--   0        0        0     9052 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/settings.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/tests/__init__.py
+-rw-r--r--   0        0        0      434 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/tests/test_sentry.py
+-rw-r--r--   0        0        0      615 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/tests/test_settings.py
+-rw-r--r--   0        0        0      225 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/urls.py
+-rw-r--r--   0        0        0      412 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/wsgi.py
+-rw-r--r--   0        0        0     3594 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/pyproject.toml
+-rw-r--r--   0        0        0     4555 1970-01-01 00:00:00.000000 document_merge_service-6.4.5/PKG-INFO
```

### Comparing `document_merge_service-6.4.4/CHANGELOG.md` & `document_merge_service-6.4.5/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 6.4.5 (25 April 2024)
+### Fix
+* **image:** Fix template validation with images in headers / footers ([`eccbb34`](https://github.com/adfinis/document-merge-service/commit/eccbb34ce69cd26a998a8ef15db109e8faf2a1e3))
+
 ## 6.4.4 (24 January 2024)
 ### Fix
 * **settings:** Add s3 ssl settings ([#698](https://github.com/adfinis/document-merge-service/issues/698)) ([`c92b381`](https://github.com/adfinis/document-merge-service/commit/c92b381ce6ebc45c0b96eba828b471f2bd28a169))
 
 
 ## 6.4.3 (23 October 2023)
 ### Fix
```

### Comparing `document_merge_service-6.4.4/LICENSE` & `document_merge_service-6.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/README.md` & `document_merge_service-6.4.5/README.md`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/authentication.py` & `document_merge_service-6.4.5/document_merge_service/api/authentication.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/data/2023.test.test.docx-template.docx` & `document_merge_service-6.4.5/document_merge_service/api/data/2023.test.test.docx-template.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/data/__init__.py` & `document_merge_service-6.4.5/document_merge_service/api/data/__init__.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/data/black.png` & `document_merge_service-6.4.5/document_merge_service/api/data/black.png`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/data/docx-mailmerge-syntax.docx` & `document_merge_service-6.4.5/document_merge_service/api/data/docx-mailmerge-syntax.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/data/docx-mailmerge.docx` & `document_merge_service-6.4.5/document_merge_service/api/data/docx-mailmerge.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/data/docx-template-filters.docx` & `document_merge_service-6.4.5/document_merge_service/api/data/docx-template-filters.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/data/docx-template-loopcontrols.docx` & `document_merge_service-6.4.5/document_merge_service/api/data/docx-template-loopcontrols.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/data/docx-template-placeholdercheck.docx` & `document_merge_service-6.4.5/document_merge_service/api/data/docx-template-placeholdercheck.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/data/docx-template-syntax.docx` & `document_merge_service-6.4.5/document_merge_service/api/data/docx-template-syntax.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/data/docx-template.docx` & `document_merge_service-6.4.5/document_merge_service/api/data/docx-template.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/data/invalid-template.xlsx` & `document_merge_service-6.4.5/document_merge_service/api/data/invalid-template.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/data/loadtest/1.doc` & `document_merge_service-6.4.5/document_merge_service/api/data/loadtest/1.doc`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/data/loadtest/2.docx` & `document_merge_service-6.4.5/document_merge_service/api/data/loadtest/2.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/data/loadtest/3.docx` & `document_merge_service-6.4.5/document_merge_service/api/data/loadtest/3.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/data/loadtest/4.docx` & `document_merge_service-6.4.5/document_merge_service/api/data/loadtest/4.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/data/odt-template.odt` & `document_merge_service-6.4.5/document_merge_service/api/data/odt-template.odt`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/data/xlsx-structure.xlsx` & `document_merge_service-6.4.5/document_merge_service/api/data/xlsx-structure.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/data/xlsx-syntax.xlsx` & `document_merge_service-6.4.5/document_merge_service/api/data/xlsx-syntax.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/data/xlsx-template.xlsx` & `document_merge_service-6.4.5/document_merge_service/api/data/xlsx-template.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/engines.py` & `document_merge_service-6.4.5/document_merge_service/api/engines.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,28 +99,55 @@
         return available_placeholders
 
 
 class DocxTemplateEngine(DocxValidator):
     def __init__(self, template):
         self.template = template
 
+    def _extract_image_placeholders(self, doc):
+        """Extract placeholders using the image filter.
+
+        This method extracts all placeholder names that use the image filter so
+        we can add a dummy image to the sample data for validation. We
+        explicitly need to parse headers and footers as well as the actual
+        document body.
+        """
+
+        body_xml = doc.get_xml()
+        body_xml = doc.patch_xml(body_xml)
+
+        xmls = [body_xml]
+
+        for _, part in [
+            *doc.get_headers_footers(doc.HEADER_URI),
+            *doc.get_headers_footers(doc.FOOTER_URI),
+        ]:
+            part_xml = doc.get_part_xml(part)
+            part_xml = doc.patch_xml(part_xml)
+            xmls.append(part_xml)
+
+        images = set()
+
+        for xml in xmls:
+            image_match = re.match(r".*{{\s?(\S*)\s?\|\s?image\(.*", xml)
+            matches = image_match.groups() if image_match else []
+            images.update(matches)
+
+        return images
+
     def validate_template_syntax(self, available_placeholders=None, sample_data=None):
         try:
             doc = DocxTemplate(self.template)
             root = _MagicPlaceholder()
             env = get_jinja_env()
             ph = {
                 name: root[name] for name in doc.get_undeclared_template_variables(env)
             }
 
-            xml = doc.get_xml()
-            xml = doc.patch_xml(xml)
-            image_match = re.match(r".*{{\s?(\S*)\s?\|\s?image\(.*", xml)
-            images = image_match.groups() if image_match else []
-            for image in images:
+            for image in self._extract_image_placeholders(doc):
                 cleaned_image = image.strip('"').strip("'")
                 ph[root[cleaned_image]] = django_file("black.png").file
 
             ph["_tpl"] = doc
 
             doc.render(ph, env)
```

### Comparing `document_merge_service-6.4.4/document_merge_service/api/file_converter.py` & `document_merge_service-6.4.5/document_merge_service/api/file_converter.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/filters.py` & `document_merge_service-6.4.5/document_merge_service/api/filters.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/jinja.py` & `document_merge_service-6.4.5/document_merge_service/api/jinja.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/management/commands/clean_dangling_files.py` & `document_merge_service-6.4.5/document_merge_service/api/management/commands/clean_dangling_files.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/management/commands/upload_local_templates.py` & `document_merge_service-6.4.5/document_merge_service/api/management/commands/upload_local_templates.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/migrations/0001_initial.py` & `document_merge_service-6.4.5/document_merge_service/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/migrations/0005_xlsx_template_engine.py` & `document_merge_service-6.4.5/document_merge_service/api/migrations/0005_xlsx_template_engine.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/migrations/0006_remove_template_group.py` & `document_merge_service-6.4.5/document_merge_service/api/migrations/0006_remove_template_group.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/models.py` & `document_merge_service-6.4.5/document_merge_service/api/models.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/serializers.py` & `document_merge_service-6.4.5/document_merge_service/api/serializers.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/tests/__snapshots__/test_template.ambr` & `document_merge_service-6.4.5/document_merge_service/api/tests/__snapshots__/test_template.ambr`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/tests/test_authentication.py` & `document_merge_service-6.4.5/document_merge_service/api/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/tests/test_clean_dangling_files.py` & `document_merge_service-6.4.5/document_merge_service/api/tests/test_clean_dangling_files.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/tests/test_convert.py` & `document_merge_service-6.4.5/document_merge_service/api/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/tests/test_excel.py` & `document_merge_service-6.4.5/document_merge_service/api/tests/test_excel.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/tests/test_filters.py` & `document_merge_service-6.4.5/document_merge_service/api/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/tests/test_jinja.py` & `document_merge_service-6.4.5/document_merge_service/api/tests/test_jinja.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/tests/test_pagination.py` & `document_merge_service-6.4.5/document_merge_service/api/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/tests/test_template.py` & `document_merge_service-6.4.5/document_merge_service/api/tests/test_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,14 +424,23 @@
             [],
             {"test": "hello"},
             [django_file("black.png").file],
             [],
             models.Template.DOCX_MAILMERGE,
             status.HTTP_400_BAD_REQUEST,
         ),
+        (
+            "docx-template-image-placeholder-header-footer.docx",
+            ["black.png", "white.png"],
+            None,
+            [],
+            [],
+            models.Template.DOCX_TEMPLATE,
+            status.HTTP_201_CREATED,
+        ),
     ],
 )
 def test_template_create_with_available_placeholders(
     db,
     admin_client,
     engine,
     template_name,
```

### Comparing `document_merge_service-6.4.4/document_merge_service/api/tests/test_unoconv.py` & `document_merge_service-6.4.5/document_merge_service/api/tests/test_unoconv.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/tests/test_upload_local_templates.py` & `document_merge_service-6.4.5/document_merge_service/api/tests/test_upload_local_templates.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/unoconv.py` & `document_merge_service-6.4.5/document_merge_service/api/unoconv.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/api/views.py` & `document_merge_service-6.4.5/document_merge_service/api/views.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/conftest.py` & `document_merge_service-6.4.5/document_merge_service/conftest.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/sentry.py` & `document_merge_service-6.4.5/document_merge_service/sentry.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/settings.py` & `document_merge_service-6.4.5/document_merge_service/settings.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/document_merge_service/tests/test_settings.py` & `document_merge_service-6.4.5/document_merge_service/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.4/pyproject.toml` & `document_merge_service-6.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "document-merge-service"
-version = "6.4.4"
+version = "6.4.5"
 description = "Merge Document Template Service"
 license = "GPL-3.0-or-later"
 authors = ["Adfinis AG <info@adfinis.com>"]
 homepage = "https://github.com/adfinis/document-merge-service"
 repository = "https://github.com/adfinis/document-merge-service"
 documentation = "https://github.com/adfinis/document-merge-service/blob/main/README.md"
 readme = "README.md"
@@ -57,17 +57,17 @@
 mypy = "1.7.1"
 pdbpp = "0.10.3"
 psutil = "5.9.8"
 pydocstyle = "6.3.0"
 pytest = "7.4.4"
 pytest-cov = "4.1.0"
 pytest-django = "4.7.0"
-pytest-env = "1.0.1"
+pytest-env = "1.1.3"
 pytest-factoryboy = "2.6.0"
-pytest-mock = "3.11.1"
+pytest-mock = "3.12.0"
 pytest-randomly = "3.15.0"
 python-semantic-release = "7.34.6"
 requests-mock = "1.11.0"
 syrupy = "4.6.0"
 types-python-dateutil = "2.8.19.14"
 types-requests = "2.31.0.6"
 types-setuptools = "69.0.0.0"
```

### Comparing `document_merge_service-6.4.4/PKG-INFO` & `document_merge_service-6.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: document-merge-service
-Version: 6.4.4
+Version: 6.4.5
 Summary: Merge Document Template Service
 Home-page: https://github.com/adfinis/document-merge-service
 License: GPL-3.0-or-later
 Author: Adfinis AG
 Author-email: info@adfinis.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

