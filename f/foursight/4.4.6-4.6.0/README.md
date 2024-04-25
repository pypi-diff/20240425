# Comparing `tmp/foursight-4.4.6.tar.gz` & `tmp/foursight-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight-4.4.6.tar", max compression
+gzip compressed data, was "foursight-4.6.0.tar", max compression
```

## Comparing `foursight-4.4.6.tar` & `foursight-4.6.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1083 2017-11-21 15:12:01.000000 foursight-4.4.6/LICENSE.txt
--rw-r--r--   0        0        0        0 2022-11-16 16:53:13.403096 foursight-4.4.6/chalicelib_fourfront/__init__.py
--rw-r--r--   0        0        0     1088 2023-07-19 18:36:43.842986 foursight-4.4.6/chalicelib_fourfront/app_utils.py
--rw-r--r--   0        0        0     5405 2022-11-16 16:53:13.404868 foursight-4.4.6/chalicelib_fourfront/check_schedules.py
--rw-r--r--   0        0        0    54908 2024-03-07 20:51:35.647720 foursight-4.4.6/chalicelib_fourfront/check_setup.json
--rw-r--r--   0        0        0      249 2022-11-16 16:53:13.406545 foursight-4.4.6/chalicelib_fourfront/checks/__init__.py
--rw-r--r--   0        0        0    63124 2024-03-22 17:29:19.867219 foursight-4.4.6/chalicelib_fourfront/checks/audit_checks.py
--rw-r--r--   0        0        0    37729 2023-07-20 15:47:44.788397 foursight-4.4.6/chalicelib_fourfront/checks/badge_checks.py
--rw-r--r--   0        0        0     1657 2023-09-14 15:07:17.515971 foursight-4.4.6/chalicelib_fourfront/checks/check_utils.py
--rw-r--r--   0        0        0    11548 2023-01-19 17:19:39.272753 foursight-4.4.6/chalicelib_fourfront/checks/deployment_checks.py
--rw-r--r--   0        0        0     2939 2023-04-19 19:52:24.091358 foursight-4.4.6/chalicelib_fourfront/checks/ecs_checks.py
--rw-r--r--   0        0        0     3914 2023-01-19 17:19:39.273550 foursight-4.4.6/chalicelib_fourfront/checks/es_checks.py
--rw-r--r--   0        0        0    15663 2023-06-09 22:12:58.101520 foursight-4.4.6/chalicelib_fourfront/checks/header_checks.py
--rw-r--r--   0        0        0      262 2022-11-16 16:53:13.426279 foursight-4.4.6/chalicelib_fourfront/checks/helpers/confchecks.py
--rw-r--r--   0        0        0    51933 2023-10-10 16:28:17.634518 foursight-4.4.6/chalicelib_fourfront/checks/helpers/google_utils.py
--rw-r--r--   0        0        0    95977 2024-03-13 13:41:24.369808 foursight-4.4.6/chalicelib_fourfront/checks/helpers/wfr_utils.py
--rw-r--r--   0        0        0    17738 2024-04-11 16:56:14.128461 foursight-4.4.6/chalicelib_fourfront/checks/helpers/wfrset_utils.py
--rw-r--r--   0        0        0     3686 2022-11-16 16:53:13.428930 foursight-4.4.6/chalicelib_fourfront/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0    99000 2024-03-22 17:29:19.869545 foursight-4.4.6/chalicelib_fourfront/checks/higlass_checks.py
--rw-r--r--   0        0        0    32926 2023-01-19 17:19:39.279026 foursight-4.4.6/chalicelib_fourfront/checks/release_updates_checks.py
--rw-r--r--   0        0        0    45209 2023-04-19 19:52:24.091978 foursight-4.4.6/chalicelib_fourfront/checks/system_checks.py
--rw-r--r--   0        0        0   131349 2024-03-07 20:07:33.211431 foursight-4.4.6/chalicelib_fourfront/checks/wfr_checks.py
--rw-r--r--   0        0        0    45350 2024-04-11 16:56:14.129826 foursight-4.4.6/chalicelib_fourfront/checks/wfr_encode_checks.py
--rw-r--r--   0        0        0   141043 2024-03-27 14:34:37.559863 foursight-4.4.6/chalicelib_fourfront/checks/wrangler_checks.py
--rw-r--r--   0        0        0       75 2024-03-07 20:07:33.211950 foursight-4.4.6/chalicelib_fourfront/gitinfo.json
--rw-r--r--   0        0        0      621 2022-11-16 16:53:13.457648 foursight-4.4.6/chalicelib_fourfront/package.py
--rw-r--r--   0        0        0      327 2023-10-11 18:26:03.611223 foursight-4.4.6/chalicelib_fourfront/scripts/local_check_execution.py
--rw-r--r--   0        0        0      316 2022-11-16 16:53:13.457903 foursight-4.4.6/chalicelib_fourfront/vars.py
--rw-r--r--   0        0        0     1610 2024-04-11 16:56:14.130960 foursight-4.4.6/pyproject.toml
--rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 foursight-4.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1083 2017-11-21 15:12:01.000000 foursight-4.6.0/LICENSE.txt
+-rw-r--r--   0        0        0        0 2022-11-16 16:53:13.403096 foursight-4.6.0/chalicelib_fourfront/__init__.py
+-rw-r--r--   0        0        0     1088 2023-07-19 18:36:43.842986 foursight-4.6.0/chalicelib_fourfront/app_utils.py
+-rw-r--r--   0        0        0     5405 2022-11-16 16:53:13.404868 foursight-4.6.0/chalicelib_fourfront/check_schedules.py
+-rw-r--r--   0        0        0    54908 2024-03-07 20:51:35.647720 foursight-4.6.0/chalicelib_fourfront/check_setup.json
+-rw-r--r--   0        0        0      249 2022-11-16 16:53:13.406545 foursight-4.6.0/chalicelib_fourfront/checks/__init__.py
+-rw-r--r--   0        0        0    65198 2024-04-25 19:24:12.957388 foursight-4.6.0/chalicelib_fourfront/checks/audit_checks.py
+-rw-r--r--   0        0        0    37729 2023-07-20 15:47:44.788397 foursight-4.6.0/chalicelib_fourfront/checks/badge_checks.py
+-rw-r--r--   0        0        0     1657 2023-09-14 15:07:17.515971 foursight-4.6.0/chalicelib_fourfront/checks/check_utils.py
+-rw-r--r--   0        0        0    11548 2023-01-19 17:19:39.272753 foursight-4.6.0/chalicelib_fourfront/checks/deployment_checks.py
+-rw-r--r--   0        0        0     2939 2023-04-19 19:52:24.091358 foursight-4.6.0/chalicelib_fourfront/checks/ecs_checks.py
+-rw-r--r--   0        0        0     3914 2023-01-19 17:19:39.273550 foursight-4.6.0/chalicelib_fourfront/checks/es_checks.py
+-rw-r--r--   0        0        0    15663 2023-06-09 22:12:58.101520 foursight-4.6.0/chalicelib_fourfront/checks/header_checks.py
+-rw-r--r--   0        0        0      262 2022-11-16 16:53:13.426279 foursight-4.6.0/chalicelib_fourfront/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0      558 2024-04-25 19:24:12.958156 foursight-4.6.0/chalicelib_fourfront/checks/helpers/es_utils.py
+-rw-r--r--   0        0        0    51933 2023-10-10 16:28:17.634518 foursight-4.6.0/chalicelib_fourfront/checks/helpers/google_utils.py
+-rw-r--r--   0        0        0    95977 2024-03-13 13:41:24.369808 foursight-4.6.0/chalicelib_fourfront/checks/helpers/wfr_utils.py
+-rw-r--r--   0        0        0    17738 2024-04-11 16:56:14.128461 foursight-4.6.0/chalicelib_fourfront/checks/helpers/wfrset_utils.py
+-rw-r--r--   0        0        0     3686 2022-11-16 16:53:13.428930 foursight-4.6.0/chalicelib_fourfront/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0    99000 2024-03-22 17:29:19.869545 foursight-4.6.0/chalicelib_fourfront/checks/higlass_checks.py
+-rw-r--r--   0        0        0    32926 2023-01-19 17:19:39.279026 foursight-4.6.0/chalicelib_fourfront/checks/release_updates_checks.py
+-rw-r--r--   0        0        0    45228 2024-04-25 19:24:12.959767 foursight-4.6.0/chalicelib_fourfront/checks/system_checks.py
+-rw-r--r--   0        0        0   131349 2024-03-07 20:07:33.211431 foursight-4.6.0/chalicelib_fourfront/checks/wfr_checks.py
+-rw-r--r--   0        0        0    45350 2024-04-11 16:56:14.129826 foursight-4.6.0/chalicelib_fourfront/checks/wfr_encode_checks.py
+-rw-r--r--   0        0        0   141107 2024-04-25 19:24:12.962591 foursight-4.6.0/chalicelib_fourfront/checks/wrangler_checks.py
+-rw-r--r--   0        0        0       75 2024-03-07 20:07:33.211950 foursight-4.6.0/chalicelib_fourfront/gitinfo.json
+-rw-r--r--   0        0        0      621 2022-11-16 16:53:13.457648 foursight-4.6.0/chalicelib_fourfront/package.py
+-rw-r--r--   0        0        0      327 2023-10-11 18:26:03.611223 foursight-4.6.0/chalicelib_fourfront/scripts/local_check_execution.py
+-rw-r--r--   0        0        0      316 2022-11-16 16:53:13.457903 foursight-4.6.0/chalicelib_fourfront/vars.py
+-rw-r--r--   0        0        0     1610 2024-04-25 19:24:12.966149 foursight-4.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 foursight-4.6.0/PKG-INFO
```

### Comparing `foursight-4.4.6/LICENSE.txt` & `foursight-4.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight-4.4.6/chalicelib_fourfront/app_utils.py` & `foursight-4.6.0/chalicelib_fourfront/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.6/chalicelib_fourfront/check_schedules.py` & `foursight-4.6.0/chalicelib_fourfront/check_schedules.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.6/chalicelib_fourfront/check_setup.json` & `foursight-4.6.0/chalicelib_fourfront/check_setup.json`

 * *Files identical despite different names*

### Comparing `foursight-4.4.6/chalicelib_fourfront/checks/audit_checks.py` & `foursight-4.6.0/chalicelib_fourfront/checks/audit_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-from dcicutils import ff_utils
+import datetime
+import os
 import re
 import requests
-import datetime
-from .helpers import wrangler_utils
-
+from typing import Optional
+from dcicutils.es_utils import create_es_client
+from dcicutils import ff_utils
+from chalicelib_fourfront.checks.helpers import wrangler_utils
+from chalicelib_fourfront.checks.helpers.es_utils import get_es_metadata
 # Use confchecks to import decorators object and its methods for each check module
 # rather than importing check_function, action_function, CheckResult, ActionResult
 # individually - they're now part of class Decorators in foursight-core::decorators
 # that requires initialization with foursight prefix.
-from .helpers.confchecks import *
+from chalicelib_fourfront.checks.helpers.confchecks import *
 
 
 STATUS_LEVEL = {
     'released': 4,
     'archived': 4,
     'current': 4,
     'revoked': 4,
@@ -569,22 +572,61 @@
         check.status = 'PASS'
         check.summary = 'No empty search links found'
         check.description = check.summary
     check.full_output = {'result': problematic_sections, 'ignore': ignored_sections}
     return check
 
 
-@check_function(id_list=None)
+# value of the tag on items where mismatch status should be ignored
+TAG_TO_IGNORE = 'ignore_status_mismatch'
+
+
+def get_items_with_ignore_tags(key):
+    query = 'search/?type=Item&tags={}'.format(TAG_TO_IGNORE)
+    delquery = query + '&status=deleted&status=replaced&status=obsolete'
+
+    res = ff_utils.search_metadata(query, key=key)
+    res.extend(ff_utils.search_metadata(delquery, key=key))
+    return [item.get('uuid') for item in res]
+
+
+@check_function(id_list=None, last_mod_date=None, run_for_all=False)
 def check_status_mismatch(connection, **kwargs):
+    # embedded sub items should have an equal or greater level
+    # than that of the item in which they are embedded
     check = CheckResult(connection, 'check_status_mismatch')
+    # if true will run on all replicate sets
+    run_for_all = kwargs['run_for_all']
+    # if values will run only on these ids
     id_list = kwargs['id_list']
+    # if provided as a param will look for items modified more recently than
+    last_mod_date = kwargs['last_mod_date']
+
+    # limit the number of top level items to query (ExperimentSets) if id_list is not 
+    # provided - if a passing result cannot be found will do what?
+    if not (run_for_all or id_list or last_mod_date):
+        last_result = check.get_primary_result()
+        days = 0
+        while last_result['status'] != 'PASS' or not last_result['kwargs'].get('primary'):
+            days += 1
+            try:
+                last_result = check.get_closest_result(diff_hours=days*24)
+            except Exception:
+                pass
+            if days > 20:
+                # no passing primary check in the past 20 days so use date from
+                # 'oldest' last_result
+                break
+        chk_uuid = last_result.get('uuid')
+        chk_uuid = chk_uuid.replace('T', ' ')
+        last_colon_idx = chk_uuid.rfind(':')
+        last_mod_date = chk_uuid[:last_colon_idx]
+
 
     MIN_CHUNK_SIZE = 200
-    # embedded sub items should have an equal or greater level
-    # than that of the item in which they are embedded
     id2links = {}
     id2status = {}
     id2item = {}
     stati2search = ['released', 'released_to_project']
     items2search = ['ExperimentSet']
     item_search = 'search/?frame=object'
     for item in items2search:
@@ -592,27 +634,36 @@
     for status in stati2search:
         item_search += '&status={}'.format(status)
 
     if id_list:
         itemids = re.split(',|\s+', id_list)
         itemids = [id for id in itemids if id]
     else:
+        if last_mod_date:
+            item_search += '&last_modified.date_modified.from={}'.format(last_mod_date)
         itemres = ff_utils.search_metadata(item_search, key=connection.ff_keys, page_limit=500)
         itemids = [item.get('uuid') for item in itemres]
-    es_items = ff_utils.get_es_metadata(itemids, key=connection.ff_keys, chunk_size=200, is_generator=True)
+
+    tagged2ignore = []
+    checked_tags = False
+    es_items = get_es_metadata(itemids, key=connection.ff_keys, chunk_size=200, is_generator=True)
+
     for es_item in es_items:
+        if not checked_tags:
+            tagged2ignore = get_items_with_ignore_tags(connection.ff_keys)
+            checked_tags = True  # only do this once if at all
         label = es_item.get('embedded').get('display_title')
         desc = es_item.get('object').get('description')
         lab = es_item.get('embedded').get('lab').get('display_title')
         status = es_item.get('properties').get('status', 'in review by lab')
         opfs = _get_all_other_processed_files(es_item)
         id2links[es_item.get('uuid')] = [li.get('uuid') for li in es_item.get('linked_uuids_embedded')]
         id2status[es_item.get('uuid')] = STATUS_LEVEL.get(status)
         id2item[es_item.get('uuid')] = {'label': label, 'status': status, 'lab': lab,
-                                        'description': desc, 'to_ignore': list(set(opfs))}
+                                        'description': desc, 'to_ignore': list(set(opfs)) + tagged2ignore}
 
     mismatches = {}
     linked2get = {}
     for i, iid in enumerate(itemids):
         linkedids = id2links.get(iid)
         if not linkedids:  # item with no link
             continue
@@ -625,16 +676,16 @@
                 ignore = id2item.get(iid).get('to_ignore')
                 if ignore is not None and lid in ignore:
                     continue
                 else:
                     mismatches.setdefault(iid, []).append(lid)
 
         if len(linked2get) > MIN_CHUNK_SIZE or i + 1 == len(itemids):  # only query es when we have more than a set number of ids (500)
-            linked2chk = ff_utils.get_es_metadata(list(linked2get.keys()), key=connection.ff_keys,
-                                                  chunk_size=200, is_generator=True)
+            linked2chk = get_es_metadata(list(linked2get.keys()), key=connection.ff_keys,
+                                         chunk_size=200, is_generator=True)
             for litem in linked2chk:
                 luuid = litem.get('uuid')
                 listatus = litem.get('properties').get('status', 'in review by lab')
                 llabel = litem.get('item_type')
                 lstatus = STATUS_LEVEL.get(listatus)
                 # add info to tracking dict
                 id2status[luuid] = lstatus
@@ -700,25 +751,25 @@
                 if case.get('higlass_view_config'):
                     files.append(case['higlass_view_config'].get('uuid'))
         if result.get('experiments_in_set'):
             for exp in result['experiments_in_set']:
                 for case in exp['other_processed_files']:
                     files.extend([i['uuid'] for i in case['files']])
     # get metadata for files, to collect status
-    resp = ff_utils.get_es_metadata(list(set(files)),
-                                    sources=['links.quality_metric', 'object.status', 'uuid'],
-                                    key=connection.ff_keys)
+    resp = get_es_metadata(list(set(files)),
+                           sources=['links.quality_metric', 'object.status', 'uuid'],
+                           key=connection.ff_keys)
     opf_status_dict = {item['uuid']: item['object']['status'] for item in resp if item['uuid'] in files}
     opf_linked_dict = {
         item['uuid']: item.get('links', {}).get('quality_metric', []) for item in resp if item['uuid'] in files
     }
     quality_metrics = [uuid for item in resp for uuid in item.get('links', {}).get('quality_metric', [])]
-    qm_resp = ff_utils.get_es_metadata(list(set(quality_metrics)),
-                                       sources=['uuid', 'object.status'],
-                                       key=connection.ff_keys)
+    qm_resp = get_es_metadata(list(set(quality_metrics)),
+                              sources=['uuid', 'object.status'],
+                              key=connection.ff_keys)
     opf_other_dict = {item['uuid']: item['object']['status'] for item in qm_resp if item not in files}
     check.full_output = {}
     for result in results:
         hg_dict = {item['title']: item.get('higlass_view_config', {}).get('uuid')
                    for item in result.get('other_processed_files', [])}
         titles = [item['title'] for item in result.get('other_processed_files', [])]
         titles.extend([item['title'] for exp in result.get('experiments_in_set', [])
@@ -881,16 +932,16 @@
                     gr_dt = genreg.get('display_title')
                     for ga, orgn in genome2orgn.items():
                         if ga in gr_dt:
                             grorgns.append(orgn)
                             assembly_in_dt = True
                             break
                     if not assembly_in_dt:
-                        gr_res = ff_utils.get_es_metadata([genreg.get('uuid')],
-                                                          key=connection.ff_keys, sources=['properties.genome_assembly'])
+                        gr_res = get_es_metadata([genreg.get('uuid')],
+                                                 key=connection.ff_keys, sources=['properties.genome_assembly'])
                         try:
                             gr_ass = gr_res[0].get('properties').get('genome_assembly')
                         except AttributeError:
                             gr_ass = None
                         if gr_ass is not None:
                             for ga, orgn in genome2orgn.items():
                                 if ga == gr_ass:
```

### Comparing `foursight-4.4.6/chalicelib_fourfront/checks/badge_checks.py` & `foursight-4.6.0/chalicelib_fourfront/checks/badge_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.6/chalicelib_fourfront/checks/check_utils.py` & `foursight-4.6.0/chalicelib_fourfront/checks/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.6/chalicelib_fourfront/checks/deployment_checks.py` & `foursight-4.6.0/chalicelib_fourfront/checks/deployment_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.6/chalicelib_fourfront/checks/ecs_checks.py` & `foursight-4.6.0/chalicelib_fourfront/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.6/chalicelib_fourfront/checks/es_checks.py` & `foursight-4.6.0/chalicelib_fourfront/checks/es_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.6/chalicelib_fourfront/checks/header_checks.py` & `foursight-4.6.0/chalicelib_fourfront/checks/header_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.6/chalicelib_fourfront/checks/helpers/google_utils.py` & `foursight-4.6.0/chalicelib_fourfront/checks/helpers/google_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.6/chalicelib_fourfront/checks/helpers/wfr_utils.py` & `foursight-4.6.0/chalicelib_fourfront/checks/helpers/wfr_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.6/chalicelib_fourfront/checks/helpers/wfrset_utils.py` & `foursight-4.6.0/chalicelib_fourfront/checks/helpers/wfrset_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.6/chalicelib_fourfront/checks/helpers/wrangler_utils.py` & `foursight-4.6.0/chalicelib_fourfront/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.6/chalicelib_fourfront/checks/higlass_checks.py` & `foursight-4.6.0/chalicelib_fourfront/checks/higlass_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.6/chalicelib_fourfront/checks/release_updates_checks.py` & `foursight-4.6.0/chalicelib_fourfront/checks/release_updates_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.6/chalicelib_fourfront/checks/system_checks.py` & `foursight-4.6.0/chalicelib_fourfront/checks/system_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 )
 from dcicutils import (
     ff_utils,
     es_utils,
     beanstalk_utils,
     env_utils
 )
+from chalicelib_fourfront.checks.helpers.es_utils import get_es_metadata
 
 # Use confchecks to import decorators object and its methods for each check module
 # rather than importing check_function, action_function, CheckResult, ActionResult
 # individually - they're now part of class Decorators in foursight-core::decorators
 # that requires initialization with foursight prefix.
 from .helpers.confchecks import *
 
@@ -829,16 +830,15 @@
     check.full_output = {}  # purged items by item type
     search = '/search/?type=TrackingItem&tracking_type=download_tracking&status=deleted&field=uuid&limit=300'
     search_res = ff_utils.search_metadata(search, key=connection.ff_keys)
     search_uuids = [res['uuid'] for res in search_res]
     client = es_utils.create_es_client(connection.ff_es, True)
     # a bit convoluted, but we want the frame=raw, which does not include uuid
     # use get_es_metadata to handle this. Use it as a generator
-    for to_purge in ff_utils.get_es_metadata(search_uuids, es_client=client, is_generator=True,
-                                             key=connection.ff_keys):
+    for to_purge in get_es_metadata(search_uuids, es_client=client, is_generator=True, key=connection.ff_keys):
         if round(time.time() - t0, 2) > time_limit:
             break
         purge_properties = to_purge['properties']
         purge_properties['uuid'] = to_purge['uuid']  # add uuid to frame=raw
         try:
             purge_res = ff_utils.purge_metadata(to_purge['uuid'], key=connection.ff_keys)
         except Exception as exc:
```

### Comparing `foursight-4.4.6/chalicelib_fourfront/checks/wfr_checks.py` & `foursight-4.6.0/chalicelib_fourfront/checks/wfr_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.6/chalicelib_fourfront/checks/wfr_encode_checks.py` & `foursight-4.6.0/chalicelib_fourfront/checks/wfr_encode_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.6/chalicelib_fourfront/checks/wrangler_checks.py` & `foursight-4.6.0/chalicelib_fourfront/checks/wrangler_checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from .helpers import wrangler_utils
 from collections import Counter
 from oauth2client.service_account import ServiceAccountCredentials
 import gspread
 from .check_utils import convert_table_to_ordered_dict
 from collections import OrderedDict
 import uuid
+from chalicelib_fourfront.checks.helpers.es_utils import get_es_metadata
 
 # Use confchecks to import decorators object and its methods for each check module
 # rather than importing check_function, action_function, CheckResult, ActionResult
 # individually - they're now part of class Decorators in foursight-core::decorators
 # that requires initialization with foursight prefix.
 from .helpers.confchecks import *
 
@@ -2119,15 +2120,15 @@
         else:  # this should not happen
             output_opfs['problematic'].append({'@id': opf['@id']})
             continue
         opf['exp_set_uuids'] = [exp_or_set['uuid'] for exp_or_set in exp_or_sets]
         exp_set_uuids_to_check.extend([uuid for uuid in opf['exp_set_uuids'] if uuid not in exp_set_uuids_to_check])
 
     # get lab of Exp/ExpSet
-    result_exp_set = ff_utils.get_es_metadata(exp_set_uuids_to_check, sources=['uuid', 'properties.lab'], key=connection.ff_keys)
+    result_exp_set = get_es_metadata(exp_set_uuids_to_check, sources=['uuid', 'properties.lab'], key=connection.ff_keys)
     es_uuid_2_lab = {}  # map Exp/Set uuid to Exp/Set lab
     for es in result_exp_set:
         es_uuid_2_lab[es['uuid']] = es['properties']['lab']
 
     # evaluate contributing lab
     for opf in other_processed_files:
         if opf['@id'] in [opf_probl['@id'] for opf_probl in output_opfs['problematic']]:
```

### Comparing `foursight-4.4.6/chalicelib_fourfront/package.py` & `foursight-4.6.0/chalicelib_fourfront/package.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.6/pyproject.toml` & `foursight-4.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [tool.poetry]
 name = "foursight"
-version = "4.4.6"
+version = "4.6.0"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "chalicelib_fourfront" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 cron-descriptor = "^1.4.0"
 click = "^7.1.2"
-dcicutils = "^8.0.0"
+dcicutils = "^8.8.4"
 PyJWT = "^2.5.0"
 Jinja2 = "^3.1.2"
 MarkupSafe = "^2.1.3"
 geocoder = "1.38.1"
 # elasticsearch 7.17.9 (at least) has a problem:
 # Error: "The client noticed that the server is not Elasticsearch and we do not support this unknown product"
 # https://stackoverflow.com/questions/68802324/elasticsearch-in-go-err-the-client-noticed-that-the-server-is-not-elasticsear
 elasticsearch = "7.13.4"
 elasticsearch-dsl = "^7.0.0"
 gitpython = "^3.1.2"
 pytz = "^2020.1"
-tibanna-ff = "^3.2.0"
+tibanna-ff = "^3.4.0"
 ## adding foursight-core
 # use below for deployment
-foursight-core = "^5.4.1"
+foursight-core = "^5.4.2"
 # use below for tests but not for deployment
 # foursight-core = { git = "https://github.com/4dn-dcic/foursight-core.git", branch="master" }
 # Need pytest-redis 3.0.2 or higher for pytest 7.4.2 (or higher).
 pytest = "^7.4.2"
 pytest-redis = "^3.0.2"
 gspread = ">=3.6.0"
 oauth2client = ">=4.1.3"
```

### Comparing `foursight-4.4.6/PKG-INFO` & `foursight-4.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight
-Version: 4.4.6
+Version: 4.6.0
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,21 +14,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: MarkupSafe (>=2.1.3,<3.0.0)
 Requires-Dist: PyJWT (>=2.5.0,<3.0.0)
 Requires-Dist: benchmark-4dn (>=0.5.17,<0.6.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
 Requires-Dist: cron-descriptor (>=1.4.0,<2.0.0)
-Requires-Dist: dcicutils (>=8.0.0,<9.0.0)
+Requires-Dist: dcicutils (>=8.8.4,<9.0.0)
 Requires-Dist: elasticsearch (==7.13.4)
 Requires-Dist: elasticsearch-dsl (>=7.0.0,<8.0.0)
-Requires-Dist: foursight-core (>=5.4.1,<6.0.0)
+Requires-Dist: foursight-core (>=5.4.2,<6.0.0)
 Requires-Dist: geocoder (==1.38.1)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google-analytics-data (>=0.17.1,<0.18.0)
 Requires-Dist: gspread (>=3.6.0)
 Requires-Dist: oauth2client (>=4.1.3)
 Requires-Dist: pytest (>=7.4.2,<8.0.0)
 Requires-Dist: pytest-redis (>=3.0.2,<4.0.0)
 Requires-Dist: pytz (>=2020.1,<2021.0)
-Requires-Dist: tibanna-ff (>=3.2.0,<4.0.0)
+Requires-Dist: tibanna-ff (>=3.4.0,<4.0.0)
 Requires-Dist: tzlocal (>=5.1,<6.0)
```

