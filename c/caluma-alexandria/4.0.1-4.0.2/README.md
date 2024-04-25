# Comparing `tmp/caluma_alexandria-4.0.1.tar.gz` & `tmp/caluma_alexandria-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caluma_alexandria-4.0.1.tar", max compression
+gzip compressed data, was "caluma_alexandria-4.0.2.tar", max compression
```

## Comparing `caluma_alexandria-4.0.1.tar` & `caluma_alexandria-4.0.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    24102 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/CHANGELOG.md
--rw-r--r--   0        0        0    35148 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/LICENSE
--rw-r--r--   0        0        0     8517 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/README.md
--rw-r--r--   0        0        0        0 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/__init__.py
--rw-r--r--   0        0        0     2199 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/api.py
--rw-r--r--   0        0        0      127 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/apps.py
--rw-r--r--   0        0        0    13501 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/factories.py
--rw-r--r--   0        0        0     6937 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/filters.py
--rw-r--r--   0        0        0        0 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/management/commands/__init__.py
--rw-r--r--   0        0        0     2394 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/management/commands/encrypt_files.py
--rw-r--r--   0        0        0      586 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/management/commands/generate_missing_thumbnails.py
--rw-r--r--   0        0        0     1084 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/management/commands/set_mime_type_and_size.py
--rw-r--r--   0        0        0    12553 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/migrations/0001_initial.py
--rw-r--r--   0        0        0      490 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/migrations/0002_tags_monolingual.py
--rw-r--r--   0        0        0      644 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/migrations/0003_file_upload_status.py
--rw-r--r--   0        0        0     2840 2024-04-15 11:55:05.601381 caluma_alexandria-4.0.1/alexandria/core/migrations/0004_tag_synonym_group.py
--rw-r--r--   0        0        0     1065 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0005_rename_type_and_meta.py
--rw-r--r--   0        0        0     1146 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py
--rw-r--r--   0        0        0      652 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0007_category_parent.py
--rw-r--r--   0        0        0      397 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0008_document_date.py
--rw-r--r--   0        0        0      466 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0009_file_checksum.py
--rw-r--r--   0        0        0     2973 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0010_mark.py
--rw-r--r--   0        0        0     1205 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0011_tag_uuid.py
--rw-r--r--   0        0        0     1655 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0012_tag_uuid_schema.py
--rw-r--r--   0        0        0     2086 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0013_file_content.py
--rw-r--r--   0        0        0      975 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0014_file_mime_type_size.py
--rw-r--r--   0        0        0     3304 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0015_fix_modified_by_description.py
--rw-r--r--   0        0        0      672 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/0016_category_allowed_mime_types.py
--rw-r--r--   0        0        0        0 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/migrations/__init__.py
--rw-r--r--   0        0        0    10789 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/models.py
--rw-r--r--   0        0        0     1823 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/presign_urls.py
--rw-r--r--   0        0        0    11317 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/serializers.py
--rw-r--r--   0        0        0      409 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/urls.py
--rw-r--r--   0        0        0     1463 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/validations.py
--rw-r--r--   0        0        0     9113 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/views.py
--rw-r--r--   0        0        0     1363 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/core/visibilities.py
--rw-r--r--   0        0        0     1703 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/dav.py
--rw-r--r--   0        0        0     4530 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/dav_provider.py
--rw-r--r--   0        0        0        0 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/oidc_auth/__init__.py
--rw-r--r--   0        0        0     4224 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/oidc_auth/authentication.py
--rw-r--r--   0        0        0     1021 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/oidc_auth/models.py
--rw-r--r--   0        0        0        0 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/settings/__init__.py
--rw-r--r--   0        0        0     7449 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/settings/alexandria.py
--rw-r--r--   0        0        0     5154 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/settings/django.py
--rw-r--r--   0        0        0        0 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/storages/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/storages/backends/__init__.py
--rw-r--r--   0        0        0     1493 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/storages/backends/s3.py
--rw-r--r--   0        0        0     2595 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/storages/fields.py
--rw-r--r--   0        0        0      162 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/urls.py
--rw-r--r--   0        0        0     1048 2024-04-15 11:55:05.605381 caluma_alexandria-4.0.1/alexandria/wsgi.py
--rw-r--r--   0        0        0     3265 2024-04-15 11:55:05.609381 caluma_alexandria-4.0.1/pyproject.toml
--rw-r--r--   0        0        0    10221 1970-01-01 00:00:00.000000 caluma_alexandria-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0    24432 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0    35148 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/LICENSE
+-rw-r--r--   0        0        0     8517 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/__init__.py
+-rw-r--r--   0        0        0     2199 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/api.py
+-rw-r--r--   0        0        0      127 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/apps.py
+-rw-r--r--   0        0        0    13523 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/factories.py
+-rw-r--r--   0        0        0     6937 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/filters.py
+-rw-r--r--   0        0        0        0 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/management/commands/__init__.py
+-rw-r--r--   0        0        0     2394 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/management/commands/encrypt_files.py
+-rw-r--r--   0        0        0      586 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/management/commands/generate_missing_thumbnails.py
+-rw-r--r--   0        0        0     1084 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/management/commands/set_mime_type_and_size.py
+-rw-r--r--   0        0        0    12553 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0001_initial.py
+-rw-r--r--   0        0        0      490 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0002_tags_monolingual.py
+-rw-r--r--   0        0        0      644 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0003_file_upload_status.py
+-rw-r--r--   0        0        0     2840 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0004_tag_synonym_group.py
+-rw-r--r--   0        0        0     1065 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0005_rename_type_and_meta.py
+-rw-r--r--   0        0        0     1146 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py
+-rw-r--r--   0        0        0      652 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0007_category_parent.py
+-rw-r--r--   0        0        0      397 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0008_document_date.py
+-rw-r--r--   0        0        0      466 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0009_file_checksum.py
+-rw-r--r--   0        0        0     2973 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0010_mark.py
+-rw-r--r--   0        0        0     1205 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0011_tag_uuid.py
+-rw-r--r--   0        0        0     1655 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0012_tag_uuid_schema.py
+-rw-r--r--   0        0        0     2086 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0013_file_content.py
+-rw-r--r--   0        0        0      975 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0014_file_mime_type_size.py
+-rw-r--r--   0        0        0     3304 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0015_fix_modified_by_description.py
+-rw-r--r--   0        0        0      672 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/0016_category_allowed_mime_types.py
+-rw-r--r--   0        0        0        0 2024-04-25 06:53:44.905191 caluma_alexandria-4.0.2/alexandria/core/migrations/__init__.py
+-rw-r--r--   0        0        0    10789 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/core/models.py
+-rw-r--r--   0        0        0     1823 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/core/presign_urls.py
+-rw-r--r--   0        0        0    11412 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/core/serializers.py
+-rw-r--r--   0        0        0      409 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/core/urls.py
+-rw-r--r--   0        0        0     1655 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/core/validations.py
+-rw-r--r--   0        0        0     9113 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/core/views.py
+-rw-r--r--   0        0        0     1363 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/core/visibilities.py
+-rw-r--r--   0        0        0     1703 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/dav.py
+-rw-r--r--   0        0        0     4530 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/dav_provider.py
+-rw-r--r--   0        0        0        0 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/oidc_auth/__init__.py
+-rw-r--r--   0        0        0     4224 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/oidc_auth/authentication.py
+-rw-r--r--   0        0        0     1021 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/oidc_auth/models.py
+-rw-r--r--   0        0        0        0 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/settings/__init__.py
+-rw-r--r--   0        0        0     7449 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/settings/alexandria.py
+-rw-r--r--   0        0        0     5154 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/settings/django.py
+-rw-r--r--   0        0        0        0 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/storages/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/storages/backends/__init__.py
+-rw-r--r--   0        0        0     1493 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/storages/backends/s3.py
+-rw-r--r--   0        0        0     2595 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/storages/fields.py
+-rw-r--r--   0        0        0      162 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/urls.py
+-rw-r--r--   0        0        0     1048 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/alexandria/wsgi.py
+-rw-r--r--   0        0        0     3290 2024-04-25 06:53:44.909191 caluma_alexandria-4.0.2/pyproject.toml
+-rw-r--r--   0        0        0    10267 1970-01-01 00:00:00.000000 caluma_alexandria-4.0.2/PKG-INFO
```

### Comparing `caluma_alexandria-4.0.1/CHANGELOG.md` & `caluma_alexandria-4.0.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# 4.0.2
+### Fix
+* **mime:** Allow file extension checking if all fails ([`ddaa134`](https://github.com/projectcaluma/alexandria/commit/ddaa1344b2cde98a0c52f3311772d36da6e28c28))
+* Use atomic for document and file creation ([`1a630ad`](https://github.com/projectcaluma/alexandria/commit/1a630adb83a8351d1ed01b3070790e65b00cc43d))
+
 # 4.0.1
 ### Fix
 * **thumbnails:** Enlarge the thumbnails ([`a80f7b5`](https://github.com/projectcaluma/alexandria/commit/a80f7b535ba21e3c8a3c23318cb95ca4be70f273))
 
 # 4.0.0
 ### Feature
 * **document:** Create document and file in one request! ([`444912d`](https://github.com/projectcaluma/alexandria/commit/444912d4cb584c05096ca8a78dd455b8471e9441))
```

### Comparing `caluma_alexandria-4.0.1/LICENSE` & `caluma_alexandria-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/README.md` & `caluma_alexandria-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/core/api.py` & `caluma_alexandria-4.0.2/alexandria/core/api.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/core/factories.py` & `caluma_alexandria-4.0.2/alexandria/core/factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     `thumb_v2 = FileFactory(variant=File.Variant.THUMBNAIL, document=thumb.document)`
 
 
     """
 
     name = factory.Maybe(
         factory.LazyAttribute(lambda o: o.variant == models.File.Variant.ORIGINAL),
-        yes_declaration=Faker("name"),
+        yes_declaration=Faker("file_name", extension="png"),
         no_declaration=factory.LazyAttribute(
             lambda o: f"{o.original.name}_preview.jpg"
         ),
     )
     document = SubFactory(DocumentFactory)
     variant = models.File.Variant.ORIGINAL
     content = factory.Maybe(
```

### Comparing `caluma_alexandria-4.0.1/alexandria/core/filters.py` & `caluma_alexandria-4.0.2/alexandria/core/filters.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/core/management/commands/encrypt_files.py` & `caluma_alexandria-4.0.2/alexandria/core/management/commands/encrypt_files.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/core/management/commands/generate_missing_thumbnails.py` & `caluma_alexandria-4.0.2/alexandria/core/management/commands/generate_missing_thumbnails.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/core/management/commands/set_mime_type_and_size.py` & `caluma_alexandria-4.0.2/alexandria/core/management/commands/set_mime_type_and_size.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/core/migrations/0001_initial.py` & `caluma_alexandria-4.0.2/alexandria/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/core/migrations/0003_file_upload_status.py` & `caluma_alexandria-4.0.2/alexandria/core/migrations/0003_file_upload_status.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/core/migrations/0004_tag_synonym_group.py` & `caluma_alexandria-4.0.2/alexandria/core/migrations/0004_tag_synonym_group.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/core/migrations/0005_rename_type_and_meta.py` & `caluma_alexandria-4.0.2/alexandria/core/migrations/0005_rename_type_and_meta.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py` & `caluma_alexandria-4.0.2/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/core/migrations/0007_category_parent.py` & `caluma_alexandria-4.0.2/alexandria/core/migrations/0007_category_parent.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/core/migrations/0010_mark.py` & `caluma_alexandria-4.0.2/alexandria/core/migrations/0010_mark.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/core/migrations/0011_tag_uuid.py` & `caluma_alexandria-4.0.2/alexandria/core/migrations/0011_tag_uuid.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/core/migrations/0012_tag_uuid_schema.py` & `caluma_alexandria-4.0.2/alexandria/core/migrations/0012_tag_uuid_schema.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/core/migrations/0013_file_content.py` & `caluma_alexandria-4.0.2/alexandria/core/migrations/0013_file_content.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/core/migrations/0014_file_mime_type_size.py` & `caluma_alexandria-4.0.2/alexandria/core/migrations/0014_file_mime_type_size.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/core/migrations/0015_fix_modified_by_description.py` & `caluma_alexandria-4.0.2/alexandria/core/migrations/0015_fix_modified_by_description.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/core/migrations/0016_category_allowed_mime_types.py` & `caluma_alexandria-4.0.2/alexandria/core/migrations/0016_category_allowed_mime_types.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/core/models.py` & `caluma_alexandria-4.0.2/alexandria/core/models.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/core/presign_urls.py` & `caluma_alexandria-4.0.2/alexandria/core/presign_urls.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/core/serializers.py` & `caluma_alexandria-4.0.2/alexandria/core/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import logging
 
 from django.conf import settings
+from django.db.transaction import atomic
 from django.template.defaultfilters import slugify
 from django.utils import translation
 from generic_permissions.validation import ValidatorMixin
 from generic_permissions.visibilities import (
     VisibilityResourceRelatedField,
     VisibilitySerializerMixin,
 )
@@ -280,14 +281,15 @@
     included_serializers = {
         "category": CategorySerializer,
         "tags": TagSerializer,
         "marks": MarkSerializer,
         "files": FileSerializer,
     }
 
+    @atomic
     def create(self, validated_data):
         content = validated_data.pop("content")
         document = super().create(validated_data)
 
         file_data = {
             "name": content.name,
             "document": {
@@ -302,14 +304,15 @@
 
         return document
 
     def _prepare_multipart(self):
         """Massage multipart data into jsonapi-compatible form."""
         self.initial_data = self.initial_data.dict()
 
+        self.initial_data["data"].seek(0)
         self.initial_data.update(
             json.loads(self.initial_data["data"].read().decode("utf-8"))
         )
         if not isinstance(self.initial_data.get("category"), dict):
             self.initial_data["category"] = {
                 "type": "categories",
                 "id": self.initial_data["category"],
```

### Comparing `caluma_alexandria-4.0.1/alexandria/core/validations.py` & `caluma_alexandria-4.0.2/alexandria/core/validations.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from mimetypes import guess_type
 
+import magic
 from django.utils.translation import gettext_lazy as _
 from django_clamd.validators import validate_file_infection
 from generic_permissions.validation import validator_for
 from rest_framework.exceptions import ValidationError
 
 from alexandria.core.models import File
 
@@ -36,12 +37,16 @@
 
         # Validate that the mime type is allowed in the category
         mime_type = data["content"].content_type
         if mime_type == "application/octet-stream" or not mime_type:
             guess, encoding = guess_type(data["name"])
             if guess is not None:
                 mime_type = guess
+            else:
+                data["content"].seek(0)
+                mime_type = magic.from_buffer(data["content"].read(), mime=True)
+                data["content"].seek(0)
 
         validate_mime_type(mime_type, data["document"].category)
         data["mime_type"] = mime_type
 
         return data
```

### Comparing `caluma_alexandria-4.0.1/alexandria/core/views.py` & `caluma_alexandria-4.0.2/alexandria/core/views.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/core/visibilities.py` & `caluma_alexandria-4.0.2/alexandria/core/visibilities.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/dav.py` & `caluma_alexandria-4.0.2/alexandria/dav.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/dav_provider.py` & `caluma_alexandria-4.0.2/alexandria/dav_provider.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/oidc_auth/authentication.py` & `caluma_alexandria-4.0.2/alexandria/oidc_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/oidc_auth/models.py` & `caluma_alexandria-4.0.2/alexandria/oidc_auth/models.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/settings/alexandria.py` & `caluma_alexandria-4.0.2/alexandria/settings/alexandria.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/settings/django.py` & `caluma_alexandria-4.0.2/alexandria/settings/django.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/storages/backends/s3.py` & `caluma_alexandria-4.0.2/alexandria/storages/backends/s3.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/storages/fields.py` & `caluma_alexandria-4.0.2/alexandria/storages/fields.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/alexandria/wsgi.py` & `caluma_alexandria-4.0.2/alexandria/wsgi.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-4.0.1/pyproject.toml` & `caluma_alexandria-4.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "caluma-alexandria"
-version = "4.0.1"
+version = "4.0.2"
 description = "Document management service"
 repository = "https://github.com/projectcaluma/alexandria"
 authors = ["Caluma <info@caluma.io>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -33,17 +33,18 @@
 requests = "^2.31.0"
 uwsgi = "^2.0.20"
 django-generic-api-permissions = "^0.4.4"
 django-storages = { extras = ['s3'], version = "^1.14.2" }
 boto3 = "^1.29.7"
 tqdm = "^4.66.1"
 manabi = "^1.3.3"
+python-magic = "^0.4.27"
 
 [tool.poetry.group.dev.dependencies]
-black = "24.3.0"
+black = "24.4.0"
 django-extensions = "3.2.3"
 django-test-migrations = "1.3.0"
 factory-boy = "3.3.0"
 flake8 = "7.0.0"
 flake8-blind-except = "0.2.1"
 flake8-debugger = "4.1.2"
 flake8-docstrings = "1.7.0"
```

### Comparing `caluma_alexandria-4.0.1/PKG-INFO` & `caluma_alexandria-4.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluma-alexandria
-Version: 4.0.1
+Version: 4.0.2
 Summary: Document management service
 Home-page: https://github.com/projectcaluma/alexandria
 License: GPL-3.0-or-later
 Author: Caluma
 Author-email: info@caluma.io
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -28,14 +28,15 @@
 Requires-Dist: djangorestframework-jsonapi (>=5.0.0,<7.0.0)
 Requires-Dist: manabi (>=1.3.3,<2.0.0)
 Requires-Dist: minio (>=7.1.14,<8.0.0)
 Requires-Dist: mozilla-django-oidc (>=2,<5)
 Requires-Dist: preview-generator (>=0.29,<0.30)
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: psycopg2-binary (>=2.9,<2.10)
+Requires-Dist: python-magic (>=0.4.27,<0.5.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Requires-Dist: uwsgi (>=2.0.20,<3.0.0)
 Project-URL: Repository, https://github.com/projectcaluma/alexandria
 Description-Content-Type: text/markdown
 
 # alexandria
```

