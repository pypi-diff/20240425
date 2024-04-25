# Comparing `tmp/Fr1997v011-1.3.0.tar.gz` & `tmp/Fr1997v011-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.3.0.tar", last modified: Tue Apr 23 10:39:21 2024, max compression
+gzip compressed data, was "Fr1997v011-1.3.1.tar", last modified: Wed Apr 24 10:40:21 2024, max compression
```

## Comparing `Fr1997v011-1.3.0.tar` & `Fr1997v011-1.3.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 10:39:21.243054 Fr1997v011-1.3.0/
-drwxrwxrwx   0        0        0        0 2024-04-23 10:39:21.229538 Fr1997v011-1.3.0/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-04-23 10:39:20.000000 Fr1997v011-1.3.0/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2024-04-23 10:39:21.000000 Fr1997v011-1.3.0/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 10:39:20.000000 Fr1997v011-1.3.0/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-23 10:39:20.000000 Fr1997v011-1.3.0/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-04-23 10:39:20.000000 Fr1997v011-1.3.0/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.3.0/LICENSE
--rw-rw-rw-   0        0        0      182 2024-04-23 10:39:21.242054 Fr1997v011-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-04-23 02:41:51.000000 Fr1997v011-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 10:39:21.231542 Fr1997v011-1.3.0/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.3.0/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 10:39:21.236542 Fr1997v011-1.3.0/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2023-10-09 02:29:18.000000 Fr1997v011-1.3.0/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   164931 2024-04-23 10:33:35.000000 Fr1997v011-1.3.0/fr1997_mode/mode_func/all_func.py
--rw-rw-rw-   0        0        0    37242 2024-04-23 03:22:03.000000 Fr1997v011-1.3.0/fr1997_mode/mode_func/json_data_fastgpt.py
-drwxrwxrwx   0        0        0        0 2024-04-23 10:39:21.240054 Fr1997v011-1.3.0/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.3.0/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-23 10:39:21.243054 Fr1997v011-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-04-23 10:39:18.000000 Fr1997v011-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:40:21.290806 Fr1997v011-1.3.1/
+drwxrwxrwx   0        0        0        0 2024-04-24 10:40:21.266722 Fr1997v011-1.3.1/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-04-24 10:40:20.000000 Fr1997v011-1.3.1/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-04-24 10:40:21.000000 Fr1997v011-1.3.1/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 10:40:20.000000 Fr1997v011-1.3.1/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-24 10:40:20.000000 Fr1997v011-1.3.1/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-04-24 10:40:20.000000 Fr1997v011-1.3.1/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-04-24 10:40:21.288285 Fr1997v011-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-04-24 02:47:42.000000 Fr1997v011-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 10:40:21.271737 Fr1997v011-1.3.1/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.3.1/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:40:21.281767 Fr1997v011-1.3.1/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       63 2024-04-23 10:58:22.000000 Fr1997v011-1.3.1/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   169672 2024-04-24 10:40:19.000000 Fr1997v011-1.3.1/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:40:21.284769 Fr1997v011-1.3.1/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.3.1/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-24 10:40:21.290806 Fr1997v011-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-04-24 02:39:08.000000 Fr1997v011-1.3.1/setup.py
```

### Comparing `Fr1997v011-1.3.0/LICENSE` & `Fr1997v011-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.3.0/README.md` & `Fr1997v011-1.3.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```sh
 python setup.py sdist
 ```
 
 ### （本地）安装包
 
 ```sh
-pip install dist/Fr1997v011-1.2.9.tar.gz
+pip install dist/Fr1997v011-1.3.1.tar.gz
 ```
 
 ### 下载包
 
 ```sh
 pip install Fr1997v011
 ```
```

### Comparing `Fr1997v011-1.3.0/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.3.1/fr1997_mode/mode_func/all_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 """
     配置文件
         所有配置在这个地方读取 
         使用内存缓存机制 memcache
         没有读取到内存中的配置，这个包相当于不能用
     pip3 cache purge
-    pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple Fr1997v011==1.2.8
+    pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple Fr1997v011==1.3.0
 """
 
 
 # 存储内存数据
 def cache_set(key, data, save_time=None):
     mc = memcache.Client(['127.0.0.1:11211'], debug=True)
     if save_time:
@@ -2363,15 +2363,15 @@
         """
         sql = kwargs.get('sql', '')
         save_data = kwargs.get('save_data')
 
         # mysql链接 【自动】0=内网 1=外网
         conn = self.db_mysql(path=conn_tp)
 
-        # 通用sql
+        # 通用sql 查看表是否存在
         sql_table_exist = f"SELECT * FROM information_schema.tables WHERE table_name = '{table}'"
 
         # 数据库操作
         try:
             with conn.cursor() as cursor:
                 if method == 'insert' or method == 'ins':
                     save_data = kwargs['save_data']
@@ -2421,29 +2421,28 @@
                     """
                         TINYINT = [-128,127]
                         SMALLINT = [-32768,32767]
                     """
                     fields_sql = []
                     field_cfg = kwargs['field_cfg']
                     for f in field_cfg['fields']:
-                        name = f['f_name']
-                        field_type = f['field_type']
-                        comment = f.get('comment', '待增加注释')
+                        name = f[0]
+                        field_type = f[1]
+                        length = f[2]
+                        default = f[3]
+                        comment = f[4]
 
                         if field_type == 'VARCHAR':
-                            length = f.get('length', 255)
-                            default = f.get('default', '')
                             fields_sql.append(f"{name} {field_type}({length}) DEFAULT '{default}' COMMENT '{comment}'")
                         elif field_type == 'INT' or field_type == 'TINYINT' or field_type == 'SMALLINT':
-                            length = f.get('length', 11)
-                            default = f.get('default', 0)
                             fields_sql.append(f"{name} {field_type}({length}) DEFAULT {default} COMMENT '{comment}'")
                         elif field_type == 'TEXT':  # 新增条件处理 TEXT 类型
-                            default = f.get('default', '')
                             fields_sql.append(f"{name} {field_type} DEFAULT '{default}' COMMENT '{comment}'")
+                        elif field_type == 'JSON':
+                            fields_sql.append(f"{name} {field_type} DEFAULT NULL COMMENT '{comment}'")
                     if fields_sql:
                         this_time = time.strftime("%Y-%m-%d %X", time.localtime(int(time.time())))
                         table_notes = f'{this_time} 【高阳】创建此表'  # 表备注
                         sql_create_base = f"CREATE TABLE {table} ({field_cfg['id']} INT AUTO_INCREMENT PRIMARY KEY,{','.join(fields_sql)}) COMMENT='{table_notes}'"
                         cursor.execute(sql_create_base)
 
                         # 增加唯一索引
@@ -2452,14 +2451,80 @@
                             if len(field_index) == 1:
                                 sql_index = f"ALTER TABLE {table} ADD UNIQUE INDEX field_index ({field_index[0]});"
                             else:
                                 sql_index = f"ALTER TABLE {table} ADD CONSTRAINT field_index UNIQUE ({','.join(field_index)});"
                             cursor.execute(sql_index)
                         print(f"创建{table}成功")
                         return f"创建{table}成功"
+                elif method == 'field_add':
+                    # 查看一个表所有字段
+                    sql_columns = f"SHOW COLUMNS FROM {table};"
+                    cursor.execute(sql_columns)
+                    columns = cursor.fetchall()
+                    columns_list = [i[0] for i in columns]
+                    field_change = kwargs.get('field_change')  # ['user', 'VARCHAR', 50, '', '用户名称']
+                    field_name = field_change[0]
+                    if field_name in columns_list:
+                        print(f"{field_name}字段已经存在")
+                        return
+
+                    # 增加字段
+                    field_type = field_change[1]
+                    length = field_change[2]
+                    default = field_change[3]
+                    comment = field_change[4]
+                    if field_type == 'VARCHAR':
+                        query = f"ALTER TABLE {table} ADD COLUMN {field_name} {field_type}({length}) COMMENT '{comment}'"
+                    elif field_type == 'INT' or field_type == 'TINYINT' or field_type == 'SMALLINT':
+                        query = f"ALTER TABLE {table} ADD COLUMN {field_name} {field_type}({length}) DEFAULT {default} COMMENT '{comment}'"
+                    elif field_type == 'TEXT':  # 新增条件处理 TEXT 类型
+                        query = f"ALTER TABLE {table} ADD COLUMN {field_name} {field_type} COMMENT '{comment}'"
+                    elif field_type == 'JSON':
+                        query = f"ALTER TABLE {table} ADD COLUMN {field_name} {field_type} DEFAULT NULL COMMENT '{comment}'"
+                    cursor.execute(query)
+                    print(f"字段{field_name}增加成功")
+                elif method == 'field_del':
+                    sql_columns = f"SHOW COLUMNS FROM {table};"
+                    cursor.execute(sql_columns)
+                    columns = cursor.fetchall()
+                    columns_list = [i[0] for i in columns]
+                    field_del = kwargs.get('field_del')  # ['user', 'VARCHAR', 50, '', '用户名称']
+                    if field_del not in columns_list:
+                        print(f"{field_del}字段不存在")
+                        return
+
+                    query = f"ALTER TABLE {table} DROP COLUMN {field_del}"
+                    cursor.execute(query)
+                    print(f"字段{field_del}删除成功")
+                elif method == 'field_up':
+                    sql_columns = f"SELECT * FROM INFORMATION_SCHEMA.COLUMNS WHERE TABLE_NAME = '{table}'"
+
+                    cursor.execute(sql_columns)
+                    columns = cursor.fetchall()
+                    field_old = kwargs.get('field_old')
+                    field_dict = {i[3]: i for i in columns}
+                    if field_old not in field_dict:
+                        print(f"{field_old} 老字段不存在")
+                        return
+
+                    change_name = kwargs.get('change_name')
+                    if change_name is None:
+                        change_name = field_old
+
+                    change_type = kwargs.get('change_type')
+                    if change_type is None:
+                        change_type = field_dict[field_old][15]
+
+                    change_comment = kwargs.get('change_comment')
+                    if change_comment is None:
+                        change_comment = field_dict[field_old][-3]
+
+                    query = f"ALTER TABLE {table} CHANGE COLUMN {field_old} {change_name} {change_type} COMMENT '{change_comment}'"
+                    cursor.execute(query)
+                    print(f"字段{field_old}修改名字成功")
                 elif method == 'sql':
                     cursor.execute(sql)
                     conn.commit()
                 elif method == 'update_more_byid' or method == 'up':  # 更新 根据id进行批量更新
                     if save_data:
                         fields = list(save_data[0].keys())
                         update_fields = [f'{i}=%s' for i in fields[:-1]]
@@ -3747,31 +3812,47 @@
 
     # app list
     def lit(self):
         response = requests.get(f'{self.base_url}/core/app/list', headers=self.get_token_header())
         print(response.json())
 
     # 应用 创建
-    def app_create(self):
-        import json_data_fastgpt
-        member_id = 15315
-        response = requests.post(f'{self.base_url}/core/app/create', headers=self.get_token_header(),
-                                 json=json_data_fastgpt.json_app_create(member_id))
-        if response.status_code == 200:
-            data_data = response.json()
-            code = data_data['code']
-            if code == 200:
-                return data_data['data']
+    def app_create(self, member_id):
+        sql = 'SELECT name,json_data FROM `cd_python_json` where `name` = "fastgpt_app_create_json"'
+        all_data = mode_pro.mysql_db(method="s", table="cd_python_json", sql=sql)
+        for at in all_data:
+            fastgpt_app_create_json = json.loads(at[1])
+            time_data = time.strftime("%Y%m%d", time.localtime(int(time.time())))
+            fastgpt_app_create_json['avatar'] = "/icon/logo.svg"
+            fastgpt_app_create_json['name'] = f'{time_data}-{int(time.time())}-{str(member_id)}'
+            response = requests.post(f'{self.base_url}/core/app/create', headers=self.get_token_header(),
+                                     json=fastgpt_app_create_json)
+            if response.status_code == 200:
+                data_data = response.json()
+                code = data_data['code']
+                if code == 200:
+                    return data_data
+        return {'code': 500}
 
     # 应用 修改 【知识库】 【提示词】
     def app_update(self, app_id, dataset_id, cue_word):
-        import json_data_fastgpt
-        response = requests.post(f'{self.base_url}/core/app/update?appId={app_id}', headers=self.get_token_header(),
-                                 json=json_data_fastgpt.json_app_update(dataset_id, cue_word))
-        print(response.text)
+        sql = 'SELECT name,json_data FROM `cd_python_json` where `name` = "fastgpt_app_update_json"'
+        all_data = mode_pro.mysql_db(method="s", table="cd_python_json", sql=sql)
+        for at in all_data:
+            fastgpt_app_create_json = json.loads(at[1])
+            fastgpt_app_create_json['modules'][2]['inputs'][7]['value'] = cue_word
+            fastgpt_app_create_json['modules'][3]['inputs'][1]['value'][0]['datasetId'] = dataset_id
+            response = requests.post(f'{self.base_url}/core/app/update?appId={app_id}', headers=self.get_token_header(),
+                                     json=fastgpt_app_create_json)
+            if response.status_code == 200:
+                data_data = response.json()
+                code = data_data['code']
+                if code == 200:
+                    return data_data
+        return {'code': 500}
 
     # 知识库 创建
     def dataset_create(self, dataset_name):
         data = {
             "parentId": None,
             "type": "dataset",
             "name": dataset_name,
```

