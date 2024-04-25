# Comparing `tmp/django-gdrive-backup-0.0.8.tar.gz` & `tmp/django-gdrive-backup-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\django-gdrive-backup-0.0.8.tar", last modified: Tue Jan 18 15:31:54 2022, max compression
+gzip compressed data, was "dist\django-gdrive-backup-0.0.9.tar", last modified: Wed Jan 19 09:36:00 2022, max compression
```

## Comparing `django-gdrive-backup-0.0.8.tar` & `django-gdrive-backup-0.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2022-01-18 15:31:54.806937 django-gdrive-backup-0.0.8/
--rw-rw-rw-   0        0        0       45 2020-10-26 10:36:44.000000 django-gdrive-backup-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4755 2022-01-18 15:31:54.805936 django-gdrive-backup-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3289 2022-01-06 17:54:52.000000 django-gdrive-backup-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-01-18 15:31:54.785936 django-gdrive-backup-0.0.8/django_gdrive_backup.egg-info/
--rw-rw-rw-   0        0        0     4755 2022-01-18 15:31:54.000000 django-gdrive-backup-0.0.8/django_gdrive_backup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      936 2022-01-18 15:31:54.000000 django-gdrive-backup-0.0.8/django_gdrive_backup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-18 15:31:54.000000 django-gdrive-backup-0.0.8/django_gdrive_backup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2022-01-18 15:31:54.000000 django-gdrive-backup-0.0.8/django_gdrive_backup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-01-18 15:31:54.000000 django-gdrive-backup-0.0.8/django_gdrive_backup.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-01-18 15:31:54.798937 django-gdrive-backup-0.0.8/gdrive_backup/
--rw-rw-rw-   0        0        0        0 2020-10-21 17:01:17.000000 django-gdrive-backup-0.0.8/gdrive_backup/__init__.py
--rw-rw-rw-   0        0        0       98 2022-01-07 12:15:08.000000 django-gdrive-backup-0.0.8/gdrive_backup/apps.py
--rw-rw-rw-   0        0        0     2357 2022-01-14 12:00:56.000000 django-gdrive-backup-0.0.8/gdrive_backup/backup.py
--rw-rw-rw-   0        0        0     5758 2022-01-14 12:11:09.000000 django-gdrive-backup-0.0.8/gdrive_backup/backup_db.py
--rw-rw-rw-   0        0        0     1754 2022-01-03 15:08:59.000000 django-gdrive-backup-0.0.8/gdrive_backup/backup_local_files.py
--rw-rw-rw-   0        0        0     5152 2022-01-03 15:18:20.000000 django-gdrive-backup-0.0.8/gdrive_backup/backup_s3.py
--rw-rw-rw-   0        0        0     2160 2022-01-10 17:51:45.000000 django-gdrive-backup-0.0.8/gdrive_backup/base_backup.py
--rw-rw-rw-   0        0        0     1086 2020-10-25 17:31:11.000000 django-gdrive-backup-0.0.8/gdrive_backup/compression.py
--rw-rw-rw-   0        0        0     9451 2022-01-18 13:54:52.000000 django-gdrive-backup-0.0.8/gdrive_backup/enhanced_views.py
-drwxrwxrwx   0        0        0        0 2022-01-18 15:31:54.798937 django-gdrive-backup-0.0.8/gdrive_backup/management/
--rw-rw-rw-   0        0        0        0 2020-10-26 10:16:50.000000 django-gdrive-backup-0.0.8/gdrive_backup/management/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-18 15:31:54.800936 django-gdrive-backup-0.0.8/gdrive_backup/management/commands/
--rw-rw-rw-   0        0        0        0 2020-06-22 14:15:42.000000 django-gdrive-backup-0.0.8/gdrive_backup/management/commands/__init__.py
--rw-rw-rw-   0        0        0     1864 2022-01-14 12:13:37.000000 django-gdrive-backup-0.0.8/gdrive_backup/management/commands/backup_website.py
--rw-rw-rw-   0        0        0      844 2022-01-13 09:25:24.000000 django-gdrive-backup-0.0.8/gdrive_backup/management/commands/restore_db.py
--rw-rw-rw-   0        0        0     3198 2022-01-13 13:32:06.000000 django-gdrive-backup-0.0.8/gdrive_backup/modals.py
--rw-rw-rw-   0        0        0     1593 2020-10-22 16:51:22.000000 django-gdrive-backup-0.0.8/gdrive_backup/prune_backups.py
--rw-rw-rw-   0        0        0     1861 2022-01-14 17:59:57.000000 django-gdrive-backup-0.0.8/gdrive_backup/sql_functions.py
--rw-rw-rw-   0        0        0     1091 2022-01-14 13:19:47.000000 django-gdrive-backup-0.0.8/gdrive_backup/tasks.py
-drwxrwxrwx   0        0        0        0 2022-01-18 15:31:54.755937 django-gdrive-backup-0.0.8/gdrive_backup/templates/
-drwxrwxrwx   0        0        0        0 2022-01-18 15:31:54.804936 django-gdrive-backup-0.0.8/gdrive_backup/templates/gdrive_backup/
--rw-rw-rw-   0        0        0     1336 2022-01-13 17:21:07.000000 django-gdrive-backup-0.0.8/gdrive_backup/templates/gdrive_backup/backup.html
--rw-rw-rw-   0        0        0     3516 2020-11-15 15:44:15.000000 django-gdrive-backup-0.0.8/gdrive_backup/templates/gdrive_backup/info.html
--rw-rw-rw-   0        0        0     1619 2022-01-13 13:32:06.000000 django-gdrive-backup-0.0.8/gdrive_backup/urls.py
--rw-rw-rw-   0        0        0     1502 2022-01-10 17:04:42.000000 django-gdrive-backup-0.0.8/gdrive_backup/views.py
--rw-rw-rw-   0        0        0       42 2022-01-18 15:31:54.806937 django-gdrive-backup-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      931 2022-01-18 15:31:10.000000 django-gdrive-backup-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-01-19 09:36:00.944261 django-gdrive-backup-0.0.9/
+-rw-rw-rw-   0        0        0       45 2020-10-26 10:36:44.000000 django-gdrive-backup-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4755 2022-01-19 09:36:00.943750 django-gdrive-backup-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3289 2022-01-06 17:54:52.000000 django-gdrive-backup-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-01-19 09:36:00.832673 django-gdrive-backup-0.0.9/django_gdrive_backup.egg-info/
+-rw-rw-rw-   0        0        0     4755 2022-01-19 09:36:00.000000 django-gdrive-backup-0.0.9/django_gdrive_backup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      936 2022-01-19 09:36:00.000000 django-gdrive-backup-0.0.9/django_gdrive_backup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-19 09:36:00.000000 django-gdrive-backup-0.0.9/django_gdrive_backup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2022-01-19 09:36:00.000000 django-gdrive-backup-0.0.9/django_gdrive_backup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2022-01-19 09:36:00.000000 django-gdrive-backup-0.0.9/django_gdrive_backup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-01-19 09:36:00.917347 django-gdrive-backup-0.0.9/gdrive_backup/
+-rw-rw-rw-   0        0        0        0 2020-10-21 17:01:17.000000 django-gdrive-backup-0.0.9/gdrive_backup/__init__.py
+-rw-rw-rw-   0        0        0       98 2022-01-07 12:15:08.000000 django-gdrive-backup-0.0.9/gdrive_backup/apps.py
+-rw-rw-rw-   0        0        0     2357 2022-01-14 12:00:56.000000 django-gdrive-backup-0.0.9/gdrive_backup/backup.py
+-rw-rw-rw-   0        0        0     5758 2022-01-14 12:11:09.000000 django-gdrive-backup-0.0.9/gdrive_backup/backup_db.py
+-rw-rw-rw-   0        0        0     1754 2022-01-03 15:08:59.000000 django-gdrive-backup-0.0.9/gdrive_backup/backup_local_files.py
+-rw-rw-rw-   0        0        0     5152 2022-01-03 15:18:20.000000 django-gdrive-backup-0.0.9/gdrive_backup/backup_s3.py
+-rw-rw-rw-   0        0        0     2160 2022-01-10 17:51:45.000000 django-gdrive-backup-0.0.9/gdrive_backup/base_backup.py
+-rw-rw-rw-   0        0        0     1086 2020-10-25 17:31:11.000000 django-gdrive-backup-0.0.9/gdrive_backup/compression.py
+-rw-rw-rw-   0        0        0    10090 2022-01-19 09:20:00.000000 django-gdrive-backup-0.0.9/gdrive_backup/enhanced_views.py
+drwxrwxrwx   0        0        0        0 2022-01-19 09:36:00.918377 django-gdrive-backup-0.0.9/gdrive_backup/management/
+-rw-rw-rw-   0        0        0        0 2020-10-26 10:16:50.000000 django-gdrive-backup-0.0.9/gdrive_backup/management/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-19 09:36:00.929014 django-gdrive-backup-0.0.9/gdrive_backup/management/commands/
+-rw-rw-rw-   0        0        0        0 2020-06-22 14:15:42.000000 django-gdrive-backup-0.0.9/gdrive_backup/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     1864 2022-01-14 12:13:37.000000 django-gdrive-backup-0.0.9/gdrive_backup/management/commands/backup_website.py
+-rw-rw-rw-   0        0        0      844 2022-01-13 09:25:24.000000 django-gdrive-backup-0.0.9/gdrive_backup/management/commands/restore_db.py
+-rw-rw-rw-   0        0        0     3198 2022-01-13 13:32:06.000000 django-gdrive-backup-0.0.9/gdrive_backup/modals.py
+-rw-rw-rw-   0        0        0     1593 2020-10-22 16:51:22.000000 django-gdrive-backup-0.0.9/gdrive_backup/prune_backups.py
+-rw-rw-rw-   0        0        0     1996 2022-01-19 09:26:38.000000 django-gdrive-backup-0.0.9/gdrive_backup/sql_functions.py
+-rw-rw-rw-   0        0        0     1091 2022-01-14 13:19:47.000000 django-gdrive-backup-0.0.9/gdrive_backup/tasks.py
+drwxrwxrwx   0        0        0        0 2022-01-19 09:36:00.783954 django-gdrive-backup-0.0.9/gdrive_backup/templates/
+drwxrwxrwx   0        0        0        0 2022-01-19 09:36:00.942181 django-gdrive-backup-0.0.9/gdrive_backup/templates/gdrive_backup/
+-rw-rw-rw-   0        0        0     1336 2022-01-13 17:21:07.000000 django-gdrive-backup-0.0.9/gdrive_backup/templates/gdrive_backup/backup.html
+-rw-rw-rw-   0        0        0     3516 2020-11-15 15:44:15.000000 django-gdrive-backup-0.0.9/gdrive_backup/templates/gdrive_backup/info.html
+-rw-rw-rw-   0        0        0     1619 2022-01-13 13:32:06.000000 django-gdrive-backup-0.0.9/gdrive_backup/urls.py
+-rw-rw-rw-   0        0        0     1502 2022-01-10 17:04:42.000000 django-gdrive-backup-0.0.9/gdrive_backup/views.py
+-rw-rw-rw-   0        0        0       42 2022-01-19 09:36:00.944786 django-gdrive-backup-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      931 2022-01-19 09:31:44.000000 django-gdrive-backup-0.0.9/setup.py
```

### Comparing `django-gdrive-backup-0.0.8/PKG-INFO` & `django-gdrive-backup-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-gdrive-backup
-Version: 0.0.8
+Version: 0.0.9
 Summary: Backs up django postgres databases, local folders and S3 folders to a Google Drive folder through a google service account.
 Home-page: https://github.com/jonesim/django-gdrive-backup
 Author: Ian Jones
 License: UNKNOWN
 Description: [![PyPI version](https://badge.fury.io/py/django-gdrive-backup.svg)](https://badge.fury.io/py/django-gdrive-backup)
```

### Comparing `django-gdrive-backup-0.0.8/README.md` & `django-gdrive-backup-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `django-gdrive-backup-0.0.8/django_gdrive_backup.egg-info/PKG-INFO` & `django-gdrive-backup-0.0.9/django_gdrive_backup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-gdrive-backup
-Version: 0.0.8
+Version: 0.0.9
 Summary: Backs up django postgres databases, local folders and S3 folders to a Google Drive folder through a google service account.
 Home-page: https://github.com/jonesim/django-gdrive-backup
 Author: Ian Jones
 License: UNKNOWN
 Description: [![PyPI version](https://badge.fury.io/py/django-gdrive-backup.svg)](https://badge.fury.io/py/django-gdrive-backup)
```

### Comparing `django-gdrive-backup-0.0.8/django_gdrive_backup.egg-info/SOURCES.txt` & `django-gdrive-backup-0.0.9/django_gdrive_backup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-gdrive-backup-0.0.8/gdrive_backup/backup.py` & `django-gdrive-backup-0.0.9/gdrive_backup/backup.py`

 * *Files identical despite different names*

### Comparing `django-gdrive-backup-0.0.8/gdrive_backup/backup_db.py` & `django-gdrive-backup-0.0.9/gdrive_backup/backup_db.py`

 * *Files identical despite different names*

### Comparing `django-gdrive-backup-0.0.8/gdrive_backup/backup_local_files.py` & `django-gdrive-backup-0.0.9/gdrive_backup/backup_local_files.py`

 * *Files identical despite different names*

### Comparing `django-gdrive-backup-0.0.8/gdrive_backup/backup_s3.py` & `django-gdrive-backup-0.0.9/gdrive_backup/backup_s3.py`

 * *Files identical despite different names*

### Comparing `django-gdrive-backup-0.0.8/gdrive_backup/base_backup.py` & `django-gdrive-backup-0.0.9/gdrive_backup/base_backup.py`

 * *Files identical despite different names*

### Comparing `django-gdrive-backup-0.0.8/gdrive_backup/compression.py` & `django-gdrive-backup-0.0.9/gdrive_backup/compression.py`

 * *Files identical despite different names*

### Comparing `django-gdrive-backup-0.0.8/gdrive_backup/enhanced_views.py` & `django-gdrive-backup-0.0.9/gdrive_backup/enhanced_views.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import base64
+import datetime
 from io import BytesIO
 
 from ajax_helpers.mixins import AjaxHelpers, AjaxTaskMixin
 from django.conf import settings
 from django.contrib.auth.mixins import PermissionRequiredMixin
 from django_datatables.columns import DateTimeColumn, DatatableColumn, ColumnLink, ColumnBase
 from django_datatables.datatables import DatatableView
@@ -73,14 +74,15 @@
                 (f'gdrive_backup:schema_info,{self.schemas[0][0]}', f'View {self.schemas[0][0]}',
                  {'visible': len(self.schemas) == 1}),
                 ('gdrive_backup:confirm_empty_trash', 'Empty Trash', {'css_classes': 'btn btn-warning'}),
                 ('gdrive_backup:confirm_drop_schema,-', 'Drop Public Schema',
                  {'css_classes': 'btn btn-danger', 'visible': getattr(settings, 'DEBUG', False)}),
             )
 
+    # noinspection PyAttributeOutsideInit
     def dispatch(self, request, *args, schema=None, **kwargs):
         self.schema = schema
         self.schemas = get_schemas()
         return super().dispatch(request, *args, **kwargs)
 
     def add_tables(self):
         self.add_table('files')
@@ -89,21 +91,25 @@
             self.add_table('schemas')
 
     @staticmethod
     def setup_files(table):
         table.add_columns('.id', 'ip_address', 'table', 'name', 'size',
                           DateTimeColumn(title='Backup Date', field='createdTime'),
                           restore_table_button('Restore DB'))
+        table.sort('-createdTime')
+        table.table_options['stateSave'] = False
 
     @staticmethod
     def setup_deleted_files(table):
         table.add_columns('.id', 'name', 'size', DateTimeColumn(title='Backup Date', field='createdTime'),
                           DatatableColumn(column_name='Undelete', render=[row_button(
                               'undelete', 'Undelete', button_classes='btn btn-secondary btn-sm'
                           )]))
+        table.sort('-createdTime')
+        table.table_options['stateSave'] = False
 
     def row_undelete(self, row_no, **_kwargs):
         db = Backup().get_backup_db()
         db.drive.service.files().update(fileId=row_no[1:], body={'trashed': False}).execute()
         return self.command_response('reload')
 
     def setup_schemas(self, table):
@@ -114,14 +120,16 @@
                 link_html='<button class="btn btn-sm btn-outline-dark">VIEW</button>'
             ),
             ColumnBase(column_name='Backup',
                        render=[row_button('backup_schema', 'Backup', button_classes='btn btn-success btn-sm',)])
         )
         table.table_data = [{'schema': s[0], 'size': s[1]} for s in self.schemas]
         table.table_options['column_id'] = 0
+        table.sort('schema')
+        table.table_options['stateSave'] = False
 
     def get_context_data(self, **kwargs):
         self.add_page_command('ajax_post', data={'ajax': 'read_storage_info'})
         context = super().get_context_data(**kwargs)
         context['schema'] = self.schema
         return context
 
@@ -163,36 +171,41 @@
         self.add_table('schema_tables')
 
     @staticmethod
     def setup_files(table):
         table.add_columns('.id', 'ip_address', 'table', 'name', 'size',
                           DateTimeColumn(title='Backup Date', field='createdTime'),
                           restore_table_button('Restore Table'))
+        table.sort('-createdTime')
+        table.table_options['stateSave'] = False
 
     def row_download_xls(self,  **kwargs):
         workbook = Workbook()
         sheet = workbook.active
         sheet.append(get_table_column_names(self.kwargs['schema'], table_name=kwargs['row_no'][1:]))
         for r in get_table_data(self.kwargs['schema'], table_name=kwargs['row_no'][1:]):
-            sheet.append(r)
+            sheet.append([c.replace(tzinfo=None) if isinstance(c, datetime.datetime) else c for c in r])
         output = BytesIO()
         workbook.save(output)
         output.seek(0)
         filename = f'{kwargs["row_no"][1:]}.xlsx'
         return self.command_response('save_file', data=base64.b64encode(output.read()).decode('ascii'),
                                      filename=filename)
 
     def setup_schema_tables(self, table):
         table.add_columns(
-            'table', 'size',
+            'table', 'size', ('rows', {'title': 'No. Rows (Approx)'}),
             ColumnBase(column_name='Download',
                        render=[row_button('download_xls', '<i class="far fa-file-excel"></i>',
                                           button_classes='btn btn-outline-secondary btn-sm', )]),
             ColumnBase(column_name='Backup',
                        render=[row_button('backup_schema', 'Backup', button_classes='btn btn-success btn-sm', )])
         )
-        table.table_data = [{'table': s[0], 'size': s[1]} for s in get_schema_tables(self.kwargs['schema'])]
+        table.table_data = [{'table': s[0], 'size': s[1], 'rows': s[2]}
+                            for s in get_schema_tables(self.kwargs['schema'])]
         table.table_options['column_id'] = 0
+        table.sort('table')
+        table.table_options['stateSave'] = False
 
     def get_table_query(self, table, **kwargs):
         files = Backup().get_backup_db(schema=self.kwargs.get('schema')).get_db_backup_files()
         return [dict(**f, **f['appProperties']) for f in files if f.get('appProperties', {}).get('table')]
```

### Comparing `django-gdrive-backup-0.0.8/gdrive_backup/management/commands/backup_website.py` & `django-gdrive-backup-0.0.9/gdrive_backup/management/commands/backup_website.py`

 * *Files identical despite different names*

### Comparing `django-gdrive-backup-0.0.8/gdrive_backup/management/commands/restore_db.py` & `django-gdrive-backup-0.0.9/gdrive_backup/management/commands/restore_db.py`

 * *Files identical despite different names*

### Comparing `django-gdrive-backup-0.0.8/gdrive_backup/modals.py` & `django-gdrive-backup-0.0.9/gdrive_backup/modals.py`

 * *Files identical despite different names*

### Comparing `django-gdrive-backup-0.0.8/gdrive_backup/prune_backups.py` & `django-gdrive-backup-0.0.9/gdrive_backup/prune_backups.py`

 * *Files identical despite different names*

### Comparing `django-gdrive-backup-0.0.8/gdrive_backup/sql_functions.py` & `django-gdrive-backup-0.0.9/gdrive_backup/sql_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,28 +16,31 @@
         )
         return [schema for schema in cursor.fetchall() if not schema[0].startswith('pg_')
                 and schema[0] not in ['information_schema']]
 
 
 def get_schema_tables(schema):
     with connection.cursor() as cursor:
-        cursor.execute(f"SELECT table_name, pg_relation_size(table_schema||'.'||table_name)"
-                       f"from information_schema.tables where table_schema='{schema}'")
+        cursor.execute(
+            f" SELECT relname , pg_relation_size(relfilenode), reltuples FROM pg_catalog.pg_class "
+            f"LEFT JOIN pg_catalog.pg_namespace ON relnamespace = pg_catalog.pg_namespace.oid "
+            f"WHERE pg_catalog.pg_namespace.nspname = 'public' AND relkind='r' "
+        )
         return cursor.fetchall()
 
 
 def get_table_column_names(schema, table_name):
     with connection.cursor() as cursor:
         cursor.execute(f"SELECT column_name from INFORMATION_SCHEMA.COLUMNS WHERE "
                        f"table_name='{table_name}' and table_schema='{schema}'")
         return [c[0] for c in cursor.fetchall()]
 
 
 def get_table_data(schema, table_name):
     with connection.cursor() as cursor:
-        cursor.execute(f"SELECT * from {schema}.{table_name}")
+        cursor.execute(f'SELECT * from {schema}."{table_name}"')
         return cursor.fetchall()
 
 
 def delete_table(schema, table_name):
     with connection.cursor() as cursor:
         cursor.execute(f'DELETE from {schema}.{table_name}')
```

### Comparing `django-gdrive-backup-0.0.8/gdrive_backup/tasks.py` & `django-gdrive-backup-0.0.9/gdrive_backup/tasks.py`

 * *Files identical despite different names*

### Comparing `django-gdrive-backup-0.0.8/gdrive_backup/templates/gdrive_backup/backup.html` & `django-gdrive-backup-0.0.9/gdrive_backup/templates/gdrive_backup/backup.html`

 * *Files identical despite different names*

### Comparing `django-gdrive-backup-0.0.8/gdrive_backup/templates/gdrive_backup/info.html` & `django-gdrive-backup-0.0.9/gdrive_backup/templates/gdrive_backup/info.html`

 * *Files identical despite different names*

### Comparing `django-gdrive-backup-0.0.8/gdrive_backup/urls.py` & `django-gdrive-backup-0.0.9/gdrive_backup/urls.py`

 * *Files identical despite different names*

### Comparing `django-gdrive-backup-0.0.8/gdrive_backup/views.py` & `django-gdrive-backup-0.0.9/gdrive_backup/views.py`

 * *Files identical despite different names*

### Comparing `django-gdrive-backup-0.0.8/setup.py` & `django-gdrive-backup-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-gdrive-backup",
-    version="0.0.8",
+    version="0.0.9",
     author="Ian Jones",
     description=("Backs up django postgres databases, local folders and S3 folders to a Google Drive folder "
                  "through a google service account."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jonesim/django-gdrive-backup",
     include_package_data=True,
```

