# Comparing `tmp/wetlab-0.27.0.tar.gz` & `tmp/wetlab-0.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wetlab-0.27.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "wetlab-0.28.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `wetlab-0.27.0.tar` & `wetlab-0.28.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0     1988 2024-03-08 12:26:27.957200 wetlab-0.27.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      482 2024-03-08 12:26:27.957327 wetlab-0.27.0/.github/workflows/deploy-instance-apis.yml
--rw-r--r--   0        0        0      133 2024-03-08 12:26:27.957503 wetlab-0.27.0/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2024-03-08 12:26:27.957680 wetlab-0.27.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1309 2024-03-08 12:53:13.133702 wetlab-0.27.0/.gitignore
--rw-r--r--   0        0        0     1800 2024-03-08 12:26:27.957903 wetlab-0.27.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       95 2024-03-08 12:53:13.134572 wetlab-0.27.0/README.md
--rw-r--r--   0        0        0     6463 2024-03-08 12:54:17.542707 wetlab-0.27.0/docs/changelog.md
--rw-r--r--   0        0        0     1975 2024-03-08 12:53:13.135290 wetlab-0.27.0/docs/guide/01-get-started.ipynb
--rw-r--r--   0        0        0       65 2024-03-08 12:26:27.958461 wetlab-0.27.0/docs/guide/index.md
--rw-r--r--   0        0        0      122 2024-03-08 12:26:27.958539 wetlab-0.27.0/docs/index.md
--rw-r--r--   0        0        0       54 2024-03-08 12:53:13.135435 wetlab-0.27.0/docs/reference.md
--rw-r--r--   0        0        0      509 2024-03-08 12:26:27.961959 wetlab-0.27.0/noxfile.py
--rw-r--r--   0        0        0      610 2024-03-08 12:53:13.135998 wetlab-0.27.0/pyproject.toml
--rw-r--r--   0        0        0      279 2024-03-08 12:53:13.137380 wetlab-0.27.0/tests/test_integrity.py
--rw-r--r--   0        0        0      401 2024-03-08 12:26:27.962604 wetlab-0.27.0/tests/test_notebooks.py
--rw-r--r--   0        0        0      707 2024-03-08 12:53:59.212425 wetlab-0.27.0/wetlab/__init__.py
--rw-r--r--   0        0        0    12114 2024-03-08 12:53:13.140111 wetlab-0.27.0/wetlab/migrations/0001_initial.py
--rw-r--r--   0        0        0    14581 2024-03-08 12:53:13.140965 wetlab-0.27.0/wetlab/migrations/0001_initial_squashed_0012.py
--rw-r--r--   0        0        0     1176 2024-03-08 12:53:13.141152 wetlab-0.27.0/wetlab/migrations/0002_alter_biosample_options_alter_experiment_options_and_more.py
--rw-r--r--   0        0        0     2325 2024-03-08 12:53:13.141263 wetlab-0.27.0/wetlab/migrations/0003_alter_biosample_created_by_and_more.py
--rw-r--r--   0        0        0     2597 2024-03-08 12:53:13.141657 wetlab-0.27.0/wetlab/migrations/0004_remove_treatment_target_genes_treatmenttarget_and_more.py
--rw-r--r--   0        0        0     1043 2024-03-08 12:53:13.142250 wetlab-0.27.0/wetlab/migrations/0005_alter_treatmenttarget_created_by_and_more.py
--rw-r--r--   0        0        0      562 2024-03-08 12:53:13.142408 wetlab-0.27.0/wetlab/migrations/0006_remove_treatment_target_treatment_targets.py
--rw-r--r--   0        0        0     3001 2024-03-08 12:53:13.142865 wetlab-0.27.0/wetlab/migrations/0007_rename_batch_name_biosample_batch_and_more.py
--rw-r--r--   0        0        0     1231 2024-03-08 12:53:13.143458 wetlab-0.27.0/wetlab/migrations/0008_platewell_delete_well.py
--rw-r--r--   0        0        0      560 2024-03-08 12:53:13.143688 wetlab-0.27.0/wetlab/migrations/0009_alter_platewell_id.py
--rw-r--r--   0        0        0     1980 2024-03-08 12:53:13.144138 wetlab-0.27.0/wetlab/migrations/0010_rename_platewell_well.py
--rw-r--r--   0        0        0     4347 2024-03-08 12:53:13.144343 wetlab-0.27.0/wetlab/migrations/0011_migrate_to_integer_pks.py
--rw-r--r--   0        0        0     1491 2024-03-08 12:53:13.144455 wetlab-0.27.0/wetlab/migrations/0012_export_legacy_data.py
--rw-r--r--   0        0        0     1727 2024-03-08 12:53:13.144555 wetlab-0.27.0/wetlab/migrations/0013_import_legacy_data.py
--rw-r--r--   0        0        0      367 2024-03-08 12:53:13.144699 wetlab-0.27.0/wetlab/migrations/0014_rename_species_biosample_organism.py
--rw-r--r--   0        0        0     1014 2024-03-08 12:53:13.144873 wetlab-0.27.0/wetlab/migrations/0015_rename_files_biosample_artifacts_and_more.py
--rw-r--r--   0        0        0      834 2024-03-08 12:53:13.145223 wetlab-0.27.0/wetlab/migrations/0016_rename_datasets_biosample_collections_and_more.py
--rw-r--r--   0        0        0      578 2024-03-08 12:53:13.145348 wetlab-0.27.0/wetlab/migrations/0017_remove_biosample_artifacts.py
--rw-r--r--   0        0        0        0 2024-03-08 12:53:13.145388 wetlab-0.27.0/wetlab/migrations/__init__.py
--rw-r--r--   0        0        0    10298 2024-03-08 12:53:13.145679 wetlab-0.27.0/wetlab/models.py
--rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 wetlab-0.27.0/PKG-INFO
+-rw-r--r--   0        0        0     1988 2024-03-08 12:26:27.957200 wetlab-0.28.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      482 2024-03-08 12:26:27.957327 wetlab-0.28.0/.github/workflows/deploy-instance-apis.yml
+-rw-r--r--   0        0        0      133 2024-03-08 12:26:27.957503 wetlab-0.28.0/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2024-03-08 12:26:27.957680 wetlab-0.28.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1309 2024-03-08 12:53:13.133702 wetlab-0.28.0/.gitignore
+-rw-r--r--   0        0        0     1800 2024-03-08 12:26:27.957903 wetlab-0.28.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       95 2024-03-08 12:53:13.134572 wetlab-0.28.0/README.md
+-rw-r--r--   0        0        0     6598 2024-04-25 14:55:02.631764 wetlab-0.28.0/docs/changelog.md
+-rw-r--r--   0        0        0     1975 2024-03-08 12:53:13.135290 wetlab-0.28.0/docs/guide/01-get-started.ipynb
+-rw-r--r--   0        0        0       65 2024-03-08 12:26:27.958461 wetlab-0.28.0/docs/guide/index.md
+-rw-r--r--   0        0        0      122 2024-03-08 12:26:27.958539 wetlab-0.28.0/docs/index.md
+-rw-r--r--   0        0        0       54 2024-03-08 12:53:13.135435 wetlab-0.28.0/docs/reference.md
+-rw-r--r--   0        0        0      509 2024-03-08 12:26:27.961959 wetlab-0.28.0/noxfile.py
+-rw-r--r--   0        0        0      610 2024-03-08 12:53:13.135998 wetlab-0.28.0/pyproject.toml
+-rw-r--r--   0        0        0      279 2024-03-08 12:53:13.137380 wetlab-0.28.0/tests/test_integrity.py
+-rw-r--r--   0        0        0      401 2024-03-08 12:26:27.962604 wetlab-0.28.0/tests/test_notebooks.py
+-rw-r--r--   0        0        0      772 2024-04-25 14:55:06.379561 wetlab-0.28.0/wetlab/__init__.py
+-rw-r--r--   0        0        0    12114 2024-03-08 12:53:13.140111 wetlab-0.28.0/wetlab/migrations/0001_initial.py
+-rw-r--r--   0        0        0    14581 2024-03-08 12:53:13.140965 wetlab-0.28.0/wetlab/migrations/0001_initial_squashed_0012.py
+-rw-r--r--   0        0        0     1176 2024-03-08 12:53:13.141152 wetlab-0.28.0/wetlab/migrations/0002_alter_biosample_options_alter_experiment_options_and_more.py
+-rw-r--r--   0        0        0     2325 2024-03-08 12:53:13.141263 wetlab-0.28.0/wetlab/migrations/0003_alter_biosample_created_by_and_more.py
+-rw-r--r--   0        0        0     2597 2024-03-08 12:53:13.141657 wetlab-0.28.0/wetlab/migrations/0004_remove_treatment_target_genes_treatmenttarget_and_more.py
+-rw-r--r--   0        0        0     1043 2024-03-08 12:53:13.142250 wetlab-0.28.0/wetlab/migrations/0005_alter_treatmenttarget_created_by_and_more.py
+-rw-r--r--   0        0        0      562 2024-03-08 12:53:13.142408 wetlab-0.28.0/wetlab/migrations/0006_remove_treatment_target_treatment_targets.py
+-rw-r--r--   0        0        0     3001 2024-03-08 12:53:13.142865 wetlab-0.28.0/wetlab/migrations/0007_rename_batch_name_biosample_batch_and_more.py
+-rw-r--r--   0        0        0     1231 2024-03-08 12:53:13.143458 wetlab-0.28.0/wetlab/migrations/0008_platewell_delete_well.py
+-rw-r--r--   0        0        0      560 2024-03-08 12:53:13.143688 wetlab-0.28.0/wetlab/migrations/0009_alter_platewell_id.py
+-rw-r--r--   0        0        0     1980 2024-03-08 12:53:13.144138 wetlab-0.28.0/wetlab/migrations/0010_rename_platewell_well.py
+-rw-r--r--   0        0        0     4347 2024-03-08 12:53:13.144343 wetlab-0.28.0/wetlab/migrations/0011_migrate_to_integer_pks.py
+-rw-r--r--   0        0        0     1485 2024-04-25 14:12:48.980909 wetlab-0.28.0/wetlab/migrations/0012_export_legacy_data.py
+-rw-r--r--   0        0        0     1721 2024-04-25 14:12:48.981143 wetlab-0.28.0/wetlab/migrations/0013_import_legacy_data.py
+-rw-r--r--   0        0        0      367 2024-03-08 12:53:13.144699 wetlab-0.28.0/wetlab/migrations/0014_rename_species_biosample_organism.py
+-rw-r--r--   0        0        0     1014 2024-03-08 12:53:13.144873 wetlab-0.28.0/wetlab/migrations/0015_rename_files_biosample_artifacts_and_more.py
+-rw-r--r--   0        0        0      834 2024-03-08 12:53:13.145223 wetlab-0.28.0/wetlab/migrations/0016_rename_datasets_biosample_collections_and_more.py
+-rw-r--r--   0        0        0      578 2024-03-08 12:53:13.145348 wetlab-0.28.0/wetlab/migrations/0017_remove_biosample_artifacts.py
+-rw-r--r--   0        0        0     1245 2024-04-25 14:54:41.237054 wetlab-0.28.0/wetlab/migrations/0018_well_created_at_well_created_by_well_updated_at.py
+-rw-r--r--   0        0        0        0 2024-03-08 12:53:13.145388 wetlab-0.28.0/wetlab/migrations/__init__.py
+-rw-r--r--   0        0        0    10668 2024-04-25 14:54:41.238397 wetlab-0.28.0/wetlab/models.py
+-rw-r--r--   0        0        0      607 1970-01-01 00:00:00.000000 wetlab-0.28.0/PKG-INFO
```

### Comparing `wetlab-0.27.0/.github/workflows/build.yml` & `wetlab-0.28.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `wetlab-0.27.0/.github/workflows/latest-changes.yml` & `wetlab-0.28.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `wetlab-0.27.0/.gitignore` & `wetlab-0.28.0/.gitignore`

 * *Files identical despite different names*

### Comparing `wetlab-0.27.0/.pre-commit-config.yaml` & `wetlab-0.28.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `wetlab-0.27.0/docs/changelog.md` & `wetlab-0.28.0/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+✨ Updated at for Well | [48](https://github.com/laminlabs/wetlab/pull/48) | [sunnyosun](https://github.com/sunnyosun) | 2024-04-25 |
 🚚 Rename lnschema-lamin1 to wetlab | [47](https://github.com/laminlabs/wetlab/pull/47) | [sunnyosun](https://github.com/sunnyosun) | 2024-03-08 | 0.27.0
 🔥 Temporarily remove a few biosample fields | [45](https://github.com/laminlabs/wetlab/pull/45) | [sunnyosun](https://github.com/sunnyosun) | 2024-02-07 | 0.26.0
 🚚 Rename `Dataset` to `Collection` | [44](https://github.com/laminlabs/wetlab/pull/44) | [falexwolf](https://github.com/falexwolf) | 2024-01-02 | 0.25.0
 🚚 Rename `File` to `Artifact` | [43](https://github.com/laminlabs/wetlab/pull/43) | [falexwolf](https://github.com/falexwolf) | 2023-12-12 | 0.24.0
 📝 Prettify docstrings | [42](https://github.com/laminlabs/wetlab/pull/42) | [falexwolf](https://github.com/falexwolf) | 2023-11-14 |
 ⬆️ Upgrade lamindb | [41](https://github.com/laminlabs/wetlab/pull/41) | [fredericenard](https://github.com/fredericenard) | 2023-11-11 | 0.23.8
 ♻️ Add CanValidate | [40](https://github.com/laminlabs/wetlab/pull/40) | [falexwolf](https://github.com/falexwolf) | 2023-11-06 | 0.23.7
```

### Comparing `wetlab-0.27.0/docs/guide/01-get-started.ipynb` & `wetlab-0.28.0/docs/guide/01-get-started.ipynb`

 * *Files identical despite different names*

### Comparing `wetlab-0.27.0/pyproject.toml` & `wetlab-0.28.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wetlab-0.27.0/wetlab/migrations/0001_initial.py` & `wetlab-0.28.0/wetlab/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wetlab-0.27.0/wetlab/migrations/0001_initial_squashed_0012.py` & `wetlab-0.28.0/wetlab/migrations/0001_initial_squashed_0012.py`

 * *Files identical despite different names*

### Comparing `wetlab-0.27.0/wetlab/migrations/0002_alter_biosample_options_alter_experiment_options_and_more.py` & `wetlab-0.28.0/wetlab/migrations/0002_alter_biosample_options_alter_experiment_options_and_more.py`

 * *Files identical despite different names*

### Comparing `wetlab-0.27.0/wetlab/migrations/0003_alter_biosample_created_by_and_more.py` & `wetlab-0.28.0/wetlab/migrations/0003_alter_biosample_created_by_and_more.py`

 * *Files identical despite different names*

### Comparing `wetlab-0.27.0/wetlab/migrations/0004_remove_treatment_target_genes_treatmenttarget_and_more.py` & `wetlab-0.28.0/wetlab/migrations/0004_remove_treatment_target_genes_treatmenttarget_and_more.py`

 * *Files identical despite different names*

### Comparing `wetlab-0.27.0/wetlab/migrations/0005_alter_treatmenttarget_created_by_and_more.py` & `wetlab-0.28.0/wetlab/migrations/0005_alter_treatmenttarget_created_by_and_more.py`

 * *Files identical despite different names*

### Comparing `wetlab-0.27.0/wetlab/migrations/0006_remove_treatment_target_treatment_targets.py` & `wetlab-0.28.0/wetlab/migrations/0006_remove_treatment_target_treatment_targets.py`

 * *Files identical despite different names*

### Comparing `wetlab-0.27.0/wetlab/migrations/0007_rename_batch_name_biosample_batch_and_more.py` & `wetlab-0.28.0/wetlab/migrations/0007_rename_batch_name_biosample_batch_and_more.py`

 * *Files identical despite different names*

### Comparing `wetlab-0.27.0/wetlab/migrations/0008_platewell_delete_well.py` & `wetlab-0.28.0/wetlab/migrations/0008_platewell_delete_well.py`

 * *Files identical despite different names*

### Comparing `wetlab-0.27.0/wetlab/migrations/0009_alter_platewell_id.py` & `wetlab-0.28.0/wetlab/migrations/0009_alter_platewell_id.py`

 * *Files identical despite different names*

### Comparing `wetlab-0.27.0/wetlab/migrations/0010_rename_platewell_well.py` & `wetlab-0.28.0/wetlab/migrations/0010_rename_platewell_well.py`

 * *Files identical despite different names*

### Comparing `wetlab-0.27.0/wetlab/migrations/0011_migrate_to_integer_pks.py` & `wetlab-0.28.0/wetlab/migrations/0011_migrate_to_integer_pks.py`

 * *Files identical despite different names*

### Comparing `wetlab-0.27.0/wetlab/migrations/0012_export_legacy_data.py` & `wetlab-0.28.0/wetlab/migrations/0012_export_legacy_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 def export_database(apps, schema_editor):
     def export_registry(registry, directory):
         table_name = registry._meta.db_table
         df = pd.read_sql_table(table_name, ln_setup.settings.instance.db)
         df.to_parquet(directory / f"{table_name}.parquet")
 
     # export data to parquet files
-    directory = Path(f"./lamindb_export/{ln_setup.settings.instance.identifier}/")
+    directory = Path(f"./lamindb_export/{ln_setup.settings.instance.slug}/")
     directory.mkdir(parents=True, exist_ok=True)
     print(f"\nExporting data to parquet files in: {directory}\n")
     for model_name in CORE_MODELS.keys():
         registry = getattr(wetlab.models, model_name)
         export_registry(registry, directory)
         many_to_many_names = [field.name for field in registry._meta.many_to_many]
         for many_to_many_name in many_to_many_names:
```

### Comparing `wetlab-0.27.0/wetlab/migrations/0013_import_legacy_data.py` & `wetlab-0.28.0/wetlab/migrations/0013_import_legacy_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     for column in old_foreign_key_columns:
         df.drop(column, axis=1, inplace=True)
     df.to_sql(table_name, ln_setup.settings.instance.db, if_exists="append", index=False)
 
 
 def import_db(apps, schema_editor):
     # import data from parquet files
-    directory = Path(f"./lamindb_export/{ln_setup.settings.instance.identifier}/")
+    directory = Path(f"./lamindb_export/{ln_setup.settings.instance.slug}/")
     if directory.exists():
         for model_name in CORE_MODELS.keys():
             registry = getattr(wetlab.models, model_name)
             import_registry(registry, directory)
             many_to_many_names = [field.name for field in registry._meta.many_to_many]
             for many_to_many_name in many_to_many_names:
                 link_orm = getattr(registry, many_to_many_name).through
```

### Comparing `wetlab-0.27.0/wetlab/migrations/0015_rename_files_biosample_artifacts_and_more.py` & `wetlab-0.28.0/wetlab/migrations/0015_rename_files_biosample_artifacts_and_more.py`

 * *Files identical despite different names*

### Comparing `wetlab-0.27.0/wetlab/migrations/0016_rename_datasets_biosample_collections_and_more.py` & `wetlab-0.28.0/wetlab/migrations/0016_rename_datasets_biosample_collections_and_more.py`

 * *Files identical despite different names*

### Comparing `wetlab-0.27.0/wetlab/migrations/0017_remove_biosample_artifacts.py` & `wetlab-0.28.0/wetlab/migrations/0017_remove_biosample_artifacts.py`

 * *Files identical despite different names*

### Comparing `wetlab-0.27.0/wetlab/models.py` & `wetlab-0.28.0/wetlab/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,20 @@
     uid = models.CharField(unique=True, max_length=4, default=ids.base62_4)
     """Universal id, valid across DB instances."""
     name = models.CharField(max_length=32, default=None, null=True, unique=True, db_index=True)
     row = models.CharField(max_length=4, default=None)
     column = models.IntegerField()
     artifacts = models.ManyToManyField(Artifact, related_name="wells")
     collections = models.ManyToManyField(Collection, related_name="wells")
+    created_at = models.DateTimeField(auto_now_add=True, db_index=True)
+    """Time of creation of record."""
+    updated_at = models.DateTimeField(auto_now=True, db_index=True)
+    """Time of last update to record."""
+    created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_wells")
+    """Creator of record, a :class:`~lamindb.User`."""
 
     class Meta:
         unique_together = (("row", "column"),)
 
 
 class TreatmentTarget(Registry, CanValidate):
     """Treatment targets."""
@@ -97,15 +103,15 @@
     uid = models.CharField(unique=True, max_length=8, default=ids.base62_8)
     """Universal id, valid across DB instances."""
     name = models.CharField(max_length=60, default=None, db_index=True)
     """Name of the treatment target."""
     description = models.TextField(null=True, default=None)
     """Description of the treatment target."""
     genes = models.ManyToManyField("lnschema_bionty.Gene", related_name="treatment_targets")
-    """Genes of the treatment target, link to :class:`~lnschema_bionty.Gene` records."""
+    """Genes of the treatment target, link to :class:`~bionty.Gene` records."""
     artifacts = models.ManyToManyField(Artifact, related_name="treatment_targets")
     """Artifacts linked to the treatment target."""
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
     created_by = models.ForeignKey(
```

### Comparing `wetlab-0.27.0/PKG-INFO` & `wetlab-0.28.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: wetlab
-Version: 0.27.0
-Summary: Lamin's `wetlab` exemplary lab schema.
+Version: 0.28.0
+Summary: Lamin's default `wetlab` lab schema.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lamindb[bionty]
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: pytest>=6.0 ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
```

