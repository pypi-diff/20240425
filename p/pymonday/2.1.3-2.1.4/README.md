# Comparing `tmp/pymonday-2.1.3.tar.gz` & `tmp/pymonday-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonday-2.1.3.tar", last modified: Wed Apr 24 11:16:56 2024, max compression
+gzip compressed data, was "pymonday-2.1.4.tar", last modified: Thu Apr 25 09:22:22 2024, max compression
```

## Comparing `pymonday-2.1.3.tar` & `pymonday-2.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 11:16:56.983894 pymonday-2.1.3/
--rw-rw-rw-   0        0        0    35823 2024-02-26 11:34:44.000000 pymonday-2.1.3/LICENSE
--rw-rw-rw-   0        0        0      344 2024-04-24 11:16:56.982394 pymonday-2.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      112 2024-02-26 12:54:28.000000 pymonday-2.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 11:16:56.970392 pymonday-2.1.3/pymonday/
--rw-rw-rw-   0        0        0       56 2024-02-26 11:40:39.000000 pymonday-2.1.3/pymonday/__init__.py
--rw-rw-rw-   0        0        0     1259 2024-02-26 11:40:48.000000 pymonday-2.1.3/pymonday/columns.py
--rw-rw-rw-   0        0        0    50323 2024-04-24 11:16:16.000000 pymonday-2.1.3/pymonday/monday_api_client.py
-drwxrwxrwx   0        0        0        0 2024-04-24 11:16:56.980894 pymonday-2.1.3/pymonday.egg-info/
--rw-rw-rw-   0        0        0      344 2024-04-24 11:16:56.000000 pymonday-2.1.3/pymonday.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2024-04-24 11:16:56.000000 pymonday-2.1.3/pymonday.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 11:16:56.000000 pymonday-2.1.3/pymonday.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-04-24 11:16:56.000000 pymonday-2.1.3/pymonday.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-24 11:16:56.000000 pymonday-2.1.3/pymonday.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 11:16:56.983894 pymonday-2.1.3/setup.cfg
--rw-rw-rw-   0        0        0      451 2024-04-24 11:16:33.000000 pymonday-2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 09:22:22.713414 pymonday-2.1.4/
+-rw-rw-rw-   0        0        0    35823 2024-02-26 11:34:44.000000 pymonday-2.1.4/LICENSE
+-rw-rw-rw-   0        0        0      344 2024-04-25 09:22:22.712414 pymonday-2.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      112 2024-02-26 12:54:28.000000 pymonday-2.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 09:22:22.702912 pymonday-2.1.4/pymonday/
+-rw-rw-rw-   0        0        0       56 2024-02-26 11:40:39.000000 pymonday-2.1.4/pymonday/__init__.py
+-rw-rw-rw-   0        0        0     1259 2024-02-26 11:40:48.000000 pymonday-2.1.4/pymonday/columns.py
+-rw-rw-rw-   0        0        0    51064 2024-04-25 09:21:50.000000 pymonday-2.1.4/pymonday/monday_api_client.py
+drwxrwxrwx   0        0        0        0 2024-04-25 09:22:22.710914 pymonday-2.1.4/pymonday.egg-info/
+-rw-rw-rw-   0        0        0      344 2024-04-25 09:22:22.000000 pymonday-2.1.4/pymonday.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-04-25 09:22:22.000000 pymonday-2.1.4/pymonday.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 09:22:22.000000 pymonday-2.1.4/pymonday.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-04-25 09:22:22.000000 pymonday-2.1.4/pymonday.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-25 09:22:22.000000 pymonday-2.1.4/pymonday.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 09:22:22.713414 pymonday-2.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      451 2024-04-25 09:21:06.000000 pymonday-2.1.4/setup.py
```

### Comparing `pymonday-2.1.3/LICENSE` & `pymonday-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymonday-2.1.3/pymonday/columns.py` & `pymonday-2.1.4/pymonday/columns.py`

 * *Files identical despite different names*

### Comparing `pymonday-2.1.3/pymonday/monday_api_client.py` & `pymonday-2.1.4/pymonday/monday_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -962,14 +962,29 @@
         response = self.__send_post_request(data)
         if not response:
             return None
         subitem_ids = [item['id'] for item in response['data']['items'][0]['subitems']]
         return subitem_ids
 
     ####################################################################################################################
+    def get_subitem_names(self, item_id):
+        """
+        Get the UUIDs of the subitem IDs and names of an item
+        :param item_id: UUID of the parent Item
+        :return: Dict of subitem IDs & Names. Return None on API call failure.
+        """
+        query_string = f'''{{items (ids: {item_id}) {{subitems {{id name}}}}}}'''
+        data = {"query": query_string}
+        response = self.__send_post_request(data)
+        if not response:
+            return None
+        subitem_ids = {item['id']: item['name'] for item in response['data']['items'][0]['subitems']}
+        return subitem_ids
+
+    ####################################################################################################################
     def get_subitem_info(self, sub_item_id):
         """
         Get the Board ID and Parent ID from a Subitem.
         :param sub_item_id: UUID of the subitem.
         :return: Dictionary containing the parent ID and Board ID of the subitem.
         """
         query_string = f'''{{items(ids: {sub_item_id}) {{parent_item {{id}} board {{id}}}}}}'''
```

