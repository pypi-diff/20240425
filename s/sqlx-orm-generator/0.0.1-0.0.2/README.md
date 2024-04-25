# Comparing `tmp/sqlx-orm-generator-0.0.1.tar.gz` & `tmp/sqlx-orm-generator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-orm-generator-0.0.1.tar", last modified: Mon Apr 22 03:37:01 2024, max compression
+gzip compressed data, was "sqlx-orm-generator-0.0.2.tar", last modified: Thu Apr 25 09:02:35 2024, max compression
```

## Comparing `sqlx-orm-generator-0.0.1.tar` & `sqlx-orm-generator-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 03:37:01.951716 sqlx-orm-generator-0.0.1/
--rw-rw-rw-   0        0        0     3508 2024-04-22 03:37:01.950716 sqlx-orm-generator-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2502 2024-04-22 02:04:47.000000 sqlx-orm-generator-0.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-22 03:37:01.935715 sqlx-orm-generator-0.0.1/orm_generator/
--rw-rw-rw-   0        0        0     1749 2024-04-22 03:14:22.000000 sqlx-orm-generator-0.0.1/orm_generator/__init__.py
--rw-rw-rw-   0        0        0     5033 2024-04-22 03:22:08.000000 sqlx-orm-generator-0.0.1/orm_generator/base.py
--rw-rw-rw-   0        0        0     1982 2024-04-22 02:52:42.000000 sqlx-orm-generator-0.0.1/orm_generator/mysql.py
--rw-rw-rw-   0        0        0     2742 2024-04-22 03:25:20.000000 sqlx-orm-generator-0.0.1/orm_generator/postgresql.py
--rw-rw-rw-   0        0        0       42 2024-04-22 03:37:01.952716 sqlx-orm-generator-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1152 2024-04-22 02:36:04.000000 sqlx-orm-generator-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:37:01.948716 sqlx-orm-generator-0.0.1/sqlx_orm_generator.egg-info/
--rw-rw-rw-   0        0        0     3508 2024-04-22 03:37:01.000000 sqlx-orm-generator-0.0.1/sqlx_orm_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      368 2024-04-22 03:37:01.000000 sqlx-orm-generator-0.0.1/sqlx_orm_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 03:37:01.000000 sqlx-orm-generator-0.0.1/sqlx_orm_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-22 03:37:01.000000 sqlx-orm-generator-0.0.1/sqlx_orm_generator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       30 2024-04-22 03:37:01.000000 sqlx-orm-generator-0.0.1/sqlx_orm_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-22 03:37:01.000000 sqlx-orm-generator-0.0.1/sqlx_orm_generator.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-25 09:02:35.109151 sqlx-orm-generator-0.0.2/
+-rw-r--r--   0 summy      (501) staff       (20)    11357 2024-04-25 08:16:59.000000 sqlx-orm-generator-0.0.2/LICENSE
+-rw-r--r--   0 summy      (501) staff       (20)     2912 2024-04-25 09:02:35.106950 sqlx-orm-generator-0.0.2/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)     2502 2024-04-25 08:16:59.000000 sqlx-orm-generator-0.0.2/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-25 09:02:35.098890 sqlx-orm-generator-0.0.2/orm_generator/
+-rw-r--r--   0 summy      (501) staff       (20)     1782 2024-04-25 08:40:32.000000 sqlx-orm-generator-0.0.2/orm_generator/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     4687 2024-04-25 08:42:35.000000 sqlx-orm-generator-0.0.2/orm_generator/base.py
+-rw-r--r--   0 summy      (501) staff       (20)     1925 2024-04-25 08:16:59.000000 sqlx-orm-generator-0.0.2/orm_generator/mysql.py
+-rw-r--r--   0 summy      (501) staff       (20)     2484 2024-04-25 08:42:35.000000 sqlx-orm-generator-0.0.2/orm_generator/postgresql.py
+-rw-r--r--   0 summy      (501) staff       (20)     1841 2024-04-25 08:59:32.000000 sqlx-orm-generator-0.0.2/orm_generator/sqlit.py
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-04-25 09:02:35.109399 sqlx-orm-generator-0.0.2/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1116 2024-04-25 08:19:38.000000 sqlx-orm-generator-0.0.2/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-25 09:02:35.105643 sqlx-orm-generator-0.0.2/sqlx_orm_generator.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     2912 2024-04-25 09:02:34.000000 sqlx-orm-generator-0.0.2/sqlx_orm_generator.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      399 2024-04-25 09:02:34.000000 sqlx-orm-generator-0.0.2/sqlx_orm_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-25 09:02:34.000000 sqlx-orm-generator-0.0.2/sqlx_orm_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-25 09:02:34.000000 sqlx-orm-generator-0.0.2/sqlx_orm_generator.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       30 2024-04-25 09:02:34.000000 sqlx-orm-generator-0.0.2/sqlx_orm_generator.egg-info/requires.txt
+-rw-r--r--   0 summy      (501) staff       (20)       14 2024-04-25 09:02:34.000000 sqlx-orm-generator-0.0.2/sqlx_orm_generator.egg-info/top_level.txt
```

### Comparing `sqlx-orm-generator-0.0.1/PKG-INFO` & `sqlx-orm-generator-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,82 @@
-Metadata-Version: 2.1
-Name: sqlx-orm-generator
-Version: 0.0.1
-Summary: sqlx-orm-generator is a model code generator from tables for sqlx-orm_generator.
-Home-page: https://gitee.com/summry/sqlx-orm-generator
-Author: summry
-Author-email: xiazhongbiao@126.com
-License: UNKNOWN
-Description: Install
-        '''''''
-        
-        .. code:: shell
-        
-           pip install mysqlx-generator
-        
-        Usage Sample
-        ''''''''''''
-        
-        .. code:: python
-        
-               from orm_generator import Generator
-        
-               if __name__ == '__main__':
-                   coder = Generator(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test')
-                   # you can generate a model class for one table
-                   coder.generate_with_tables(tables='user', path='models.py')
-                   # you can generate model classes for tables
-                   coder.generate_with_tables(tables=['user', 'person'], path='models.py')
-                   # you can generate model classes for all tables from a given schema. default current schema if not given
-                   coder.generate_with_schema(schema='test', path='models.py')
-        
-        If you run last code, then generate a file 'models.py' in current
-        directory like follow:
-        
-        .. code:: python
-        
-               from decimal import Decimal
-               from datetime import date, datetime
-               from orm import Model, KeyStrategy
-        
-               class BaseModel(Model):
-                   __key__ = 'id'
-                   __del_flag__ = 'del_flag'
-                   __update_by__ = 'update_by'
-                   __update_time__ = 'update_time'
-                   __key_strategy__ = KeyStrategy.DB_AUTO_INCREMENT
-        
-                   def __init__(self, id: int = None, create_by: int = None, create_time: datetime = None, update_by: int = None, update_time: datetime = None,
-                           del_flag: int = None):
-                       self.id = id
-                       self.create_by = create_by
-                       self.create_time = create_time
-                       self.update_by = update_by
-                       self.update_time = update_time
-                       self.del_flag = del_flag
-        
-        
-               class User(BaseModel):
-                   __table__ = 'user'
-        
-                   def __init__(self, id: int = None, name: str = None, age: int = None, birth_date: date = None, sex: int = None, grade: float = None,
-                           point: float = None, money: Decimal = None, create_by: int = None, create_time: datetime = None, update_by: int = None,
-                           update_time: datetime = None, del_flag: int = None):
-                       super().__init__(id=id, create_by=create_by, create_time=create_time, update_by=update_by, update_time=update_time, del_flag=del_flag)
-                       self.name = name
-                       self.age = age
-                       self.birth_date = birth_date
-                       self.sex = sex
-                       self.grade = grade
-                       self.point = point
-                       self.money = money
-        
-        
-        MySqlx: https://pypi.org/project/mysqlx
-        
-Keywords: MySQL,mysqlx,python
-Platform: UNKNOWN
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: sqlx-orm-generator
+Version: 0.0.2
+Summary: sqlx-orm-generator is a model code generator from tables for sqlx-orm_generator.
+Home-page: https://gitee.com/summry/sqlx-orm-generator
+Author: summry
+Author-email: xiazhongbiao@126.com
+License: UNKNOWN
+Keywords: MySQL,mysqlx,python
+Platform: UNKNOWN
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Install
+'''''''
+
+.. code:: shell
+
+   pip install mysqlx-generator
+
+Usage Sample
+''''''''''''
+
+.. code:: python
+
+       from orm_generator import Generator
+
+       if __name__ == '__main__':
+           coder = Generator(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test')
+           # you can generate a model class for one table
+           coder.generate_with_tables(tables='user', path='models.py')
+           # you can generate model classes for tables
+           coder.generate_with_tables(tables=['user', 'person'], path='models.py')
+           # you can generate model classes for all tables from a given schema. default current schema if not given
+           coder.generate_with_schema(schema='test', path='models.py')
+
+If you run last code, then generate a file 'models.py' in current
+directory like follow:
+
+.. code:: python
+
+       from decimal import Decimal
+       from datetime import date, datetime
+       from orm import Model, KeyStrategy
+
+       class BaseModel(Model):
+           __key__ = 'id'
+           __del_flag__ = 'del_flag'
+           __update_by__ = 'update_by'
+           __update_time__ = 'update_time'
+           __key_strategy__ = KeyStrategy.DB_AUTO_INCREMENT
+
+           def __init__(self, id: int = None, create_by: int = None, create_time: datetime = None, update_by: int = None, update_time: datetime = None,
+                   del_flag: int = None):
+               self.id = id
+               self.create_by = create_by
+               self.create_time = create_time
+               self.update_by = update_by
+               self.update_time = update_time
+               self.del_flag = del_flag
+
+
+       class User(BaseModel):
+           __table__ = 'user'
+
+           def __init__(self, id: int = None, name: str = None, age: int = None, birth_date: date = None, sex: int = None, grade: float = None,
+                   point: float = None, money: Decimal = None, create_by: int = None, create_time: datetime = None, update_by: int = None,
+                   update_time: datetime = None, del_flag: int = None):
+               super().__init__(id=id, create_by=create_by, create_time=create_time, update_by=update_by, update_time=update_time, del_flag=del_flag)
+               self.name = name
+               self.age = age
+               self.birth_date = birth_date
+               self.sex = sex
+               self.grade = grade
+               self.point = point
+               self.money = money
+
+
+MySqlx: https://pypi.org/project/mysqlx
+
+
```

### Comparing `sqlx-orm-generator-0.0.1/README.rst` & `sqlx-orm-generator-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-orm-generator-0.0.1/orm_generator/base.py` & `sqlx-orm-generator-0.0.2/orm_generator/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,127 +1,123 @@
-import os
-import sqlexec as db
-from typing import Union, Iterable
-from jinja2 import FileSystemLoader, Environment
-from orm.constant import KEY, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, KEY_STRATEGY
-
-COMMON_COLS = ['create_by', 'create_time']
-ATTRIBUTES = {KEY: 'id', UPDATE_BY: 'update_by', UPDATE_TIME: 'update_time', DEL_FLAG: 'del_flag'}
-
-
-class BaseGenerator:
-
-    def __init__(self, template: str, show_table_sql=None, attribute_list=None):
-        self.template = template
-        self.show_table_sql = show_table_sql if show_table_sql else 'show tables'
-        self.attribute_list = attribute_list if attribute_list else [KEY, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, KEY_STRATEGY]
-
-    def generate_with_schema(self, schema: str = None, path: str = None, *args, **kwargs):
-        """
-        coder = Generator(user='root', password='xxx', host='127.0.0.1', port=3306, database='testdb', driver='pymysql')
-        coder.generate_with_schema('testdb', 'models.py')
-        """
-
-        if schema:
-            db.execute('use %s' % schema)
-        tables = db.select(self.show_table_sql)
-        tables = [table[0] for table in tables]
-        self.generate_with_tables(tables=tables, path=path, *args, **kwargs)
-
-    def generate_with_tables(self, tables: Union[str, Iterable[str]], path: str = None, *args, **kwargs):
-        """
-        coder = Generator(user='root', password='xxx', host='127.0.0.1', port=3306, database='testdb', driver='pymysql')
-        coder.generate_with_tables(['user', 'person'], 'models.py')
-        """
-
-        metas = None
-        only_one_table = False
-        if not args:
-            args = COMMON_COLS
-        if not kwargs:
-            kwargs = ATTRIBUTES
-
-        columns = [v for v in kwargs.values()]
-        if args:
-            args = list(args)
-            args.reverse()
-            for i in range(0, len(args)):
-                columns.insert(1, args[i])
-
-            # 去重
-            base_columns = list(set(columns))
-            # 保持原有顺序
-            base_columns.sort(key=columns.index)
-        else:
-            base_columns = columns
-
-        # 设置属性名
-        prefix = '__attribute_name'
-        for item in self.attribute_list:
-            kwargs[prefix + item] = item
-
-        if isinstance(tables, str):
-            if self.comma1 in tables:
-                tables = tables.split(self.comma1)
-            elif self.comma2 in tables:
-                tables = tables.split(self.comma2)
-            else:
-                only_one_table = True
-                metas = [self._get_table_meta(tables, base_columns)]
-
-        if not only_one_table:
-            if not isinstance(tables, set):
-                tables = set(tables)
-            metas = [self._get_table_meta(table.strip(), base_columns) for table in tables]
-
-        no_key_tables = [meta for meta in metas if isinstance(meta, str)]
-        if len(no_key_tables) > 0:
-            print("There isn't primary key in the tables %s, it will not generate model class." % no_key_tables)
-
-        metas = [meta for meta in metas if isinstance(meta, dict)]
-        if len(metas) > 0:
-            cols = [col for mata in metas for col in mata['super_columns']]
-            col_dict = {col['COLUMN_NAME']: col for col in cols}
-
-            def get_type(col):
-                if col in col_dict:
-                    return col_dict[col]['DATA_TYPE']
-                elif col == kwargs.get(KEY) or col == kwargs.get(UPDATE_BY) or col == kwargs.get(DEL_FLAG):
-                    return 'int'
-                elif col == kwargs.get('__update_time__'):
-                    return 'datetime'
-                elif col.endswith("_time"):
-                    return 'datetime'
-                elif col.endswith("_date"):
-                    return 'date'
-                else:
-                    return 'None'
-
-            kwargs['metas'] = metas
-            kwargs['base_columns'] = [{'COLUMN_NAME': col, 'DATA_TYPE': get_type(col)} for col in base_columns]
-            self._generate(kwargs, path)
-
-    def _get_table_meta(self, table: str, base_columns):
-       raise NotImplementedError
-
-    def _generate(self, metas: dict, path: str):
-        loader = FileSystemLoader(searchpath=os.path.dirname(__file__))
-        environment = Environment(loader=loader)
-        tpl = environment.get_template(self.template)
-        output = tpl.render(**metas)
-        if path:
-            suffix = '.py'
-            path = path if path.endswith(suffix) else path + suffix
-            with open(path, 'w', encoding='utf-8') as f:
-                f.write(output)
-            print('Model文件已生成：%s' % path)
-        else:
-            print(output)
-
-    @staticmethod
-    def _get_class_name(table):
-        if '_' not in table:
-            return table.capitalize()
-
-        names = table.split('_')
-        names = [name.capitalize() for name in names]
+import os
+import sqlexec as db
+from typing import Union, Iterable
+from jinja2 import FileSystemLoader, Environment
+from orm.constant import KEY, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, KEY_STRATEGY
+
+COMMON_COLS = ['create_by', 'create_time']
+ATTRIBUTES = {KEY: 'id', UPDATE_BY: 'update_by', UPDATE_TIME: 'update_time', DEL_FLAG: 'del_flag'}
+
+
+class BaseGenerator:
+
+    def __init__(self, template: str, attribute_list=None):
+        self.template = template
+        self.attribute_list = attribute_list if attribute_list else [KEY, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, KEY_STRATEGY]
+
+    def generate_with_schema(self, schema: str = None, path: str = None, *args, **kwargs):
+        """
+        coder = Generator(user='root', password='xxx', host='127.0.0.1', port=3306, database='testdb', driver='pymysql')
+        coder.generate_with_schema('testdb', 'models.py')
+        """
+
+        tables = db.show_tables(schema)
+        self.generate_with_tables(tables=tables, path=path, *args, **kwargs)
+
+    def generate_with_tables(self, tables: Union[str, Iterable[str]], path: str = None, *args, **kwargs):
+        """
+        coder = Generator(user='root', password='xxx', host='127.0.0.1', port=3306, database='testdb', driver='pymysql')
+        coder.generate_with_tables(['user', 'person'], 'models.py')
+        """
+
+        metas = None
+        only_one_table = False
+        if not args:
+            args = COMMON_COLS
+        if not kwargs:
+            kwargs = ATTRIBUTES
+
+        columns = [v for v in kwargs.values()]
+        if args:
+            args = list(args)
+            args.reverse()
+            for i in range(0, len(args)):
+                columns.insert(1, args[i])
+
+            # 去重
+            base_columns = list(set(columns))
+            # 保持原有顺序
+            base_columns.sort(key=columns.index)
+        else:
+            base_columns = columns
+
+        # 设置属性名
+        prefix = '__attribute_name'
+        for item in self.attribute_list:
+            kwargs[prefix + item] = item
+
+        if isinstance(tables, str):
+            if self.comma1 in tables:
+                tables = tables.split(self.comma1)
+            elif self.comma2 in tables:
+                tables = tables.split(self.comma2)
+            else:
+                only_one_table = True
+                metas = [self._get_table_meta(tables, base_columns)]
+
+        if not only_one_table:
+            if not isinstance(tables, set):
+                tables = set(tables)
+            metas = [self._get_table_meta(table.strip(), base_columns) for table in tables]
+
+        no_key_tables = [meta for meta in metas if isinstance(meta, str)]
+        if len(no_key_tables) > 0:
+            print("There isn't primary key in the tables %s, it will not generate model class." % no_key_tables)
+
+        metas = [meta for meta in metas if isinstance(meta, dict)]
+        if len(metas) > 0:
+            cols = [col for mata in metas for col in mata['super_columns']]
+            col_dict = {col['COLUMN_NAME']: col for col in cols}
+
+            def get_type(col):
+                if col in col_dict:
+                    return col_dict[col]['DATA_TYPE']
+                elif col == kwargs.get(KEY) or col == kwargs.get(UPDATE_BY) or col == kwargs.get(DEL_FLAG):
+                    return 'int'
+                elif col == kwargs.get('__update_time__'):
+                    return 'datetime'
+                elif col.endswith("_time"):
+                    return 'datetime'
+                elif col.endswith("_date"):
+                    return 'date'
+                else:
+                    return 'None'
+
+            kwargs['metas'] = metas
+            kwargs['base_columns'] = [{'COLUMN_NAME': col, 'DATA_TYPE': get_type(col)} for col in base_columns]
+            self._generate(kwargs, path)
+
+    def _get_table_meta(self, table: str, base_columns):
+       raise NotImplementedError
+
+    def _generate(self, metas: dict, path: str):
+        loader = FileSystemLoader(searchpath=os.path.dirname(__file__))
+        environment = Environment(loader=loader)
+        tpl = environment.get_template(self.template)
+        output = tpl.render(**metas)
+        if path:
+            suffix = '.py'
+            path = path if path.endswith(suffix) else path + suffix
+            with open(path, 'w', encoding='utf-8') as f:
+                f.write(output)
+            print('Model文件已生成：%s' % path)
+        else:
+            print(output)
+
+    @staticmethod
+    def _get_class_name(table):
+        if '_' not in table:
+            return table.capitalize()
+
+        names = table.split('_')
+        names = [name.capitalize() for name in names]
         return ''.join(names)
```

### Comparing `sqlx-orm-generator-0.0.1/orm_generator/mysql.py` & `sqlx-orm-generator-0.0.2/orm_generator/sqlit.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-import sqlexec as db
-from orm.constant import KEY, UPDATE_BY, UPDATE_TIME, DEL_FLAG
-
-from .base import BaseGenerator
-
-COMMON_COLS = ['create_by', 'create_time']
-ATTRIBUTES = {KEY: 'id', UPDATE_BY: 'update_by', UPDATE_TIME: 'update_time', DEL_FLAG: 'del_flag'}
-
-
-class MySQLGenerator(BaseGenerator):
-    comma1 = ','
-    comma2 = '，'
-    sql = '''
-    SELECT column_name, data_type, character_maximum_length, NUMERIC_precision, NUMERIC_scale, column_key FROM information_schema.columns
-     WHERE table_schema = (SELECT DATABASE()) AND table_name = ? 
-    '''
-
-    def __init__(self):
-        super().__init__('mysql.tpl')
-
-    def _get_table_meta(self, table: str, base_columns):
-        def convert_type(col_type):
-            if col_type in ('int', 'tinyint', 'bigint'):
-                return 'int'
-            elif col_type in ('float', 'double'):
-                return 'float'
-            elif col_type == 'decimal':
-                return 'Decimal'
-            elif col_type in ('char', 'varchar', 'text'):
-                return 'str'
-            elif col_type in ('date', 'datetime'):
-                return col_type
-            else:
-                return 'None'
-
-        key = None
-        super_columns = []
-        columns = db.do_query(self.sql, table)
-        for col in columns:
-            if col['COLUMN_KEY'] == 'PRI':
-                key = col['COLUMN_NAME']
-            if col['COLUMN_NAME'] in base_columns:
-                super_columns.append(col)
-            col['DATA_TYPE'] = convert_type(col['DATA_TYPE'])
-
-        if key is None:
-            return table
-
-        class_name = self._get_class_name(table)
-        return {
-            'key': key,
-            'table': table,
-            'class_name': class_name,
-            'columns': columns,
-            'self_columns': [col for col in columns if col['COLUMN_NAME'] not in base_columns],
-            'super_columns': super_columns
-        }
+import sqlexec as db
+from orm.constant import KEY, UPDATE_BY, UPDATE_TIME, DEL_FLAG
+
+from .base import BaseGenerator
+
+COMMON_COLS = ['create_by', 'create_time']
+ATTRIBUTES = {KEY: 'id', UPDATE_BY: 'update_by', UPDATE_TIME: 'update_time', DEL_FLAG: 'del_flag'}
+
+
+class SqliteGenerator(BaseGenerator):
+    comma1 = ','
+    comma2 = '，'
+    sql = 'PRAGMA table_info(%s)'
+
+    def __init__(self):
+        super().__init__('mysql.tpl')
+
+    def _get_table_meta(self, table: str, base_columns):
+        def convert_type(col_type):
+            if col_type in ('int', 'tinyint', 'bigint', 'INTEGER', 'smallint'):
+                return 'int'
+            elif col_type in ('float', 'double'):
+                return 'float'
+            elif 'decimal' in col_type:
+                return 'Decimal'
+            elif col_type in ('char', 'varchar', 'TEXT'):
+                return 'str'
+            elif col_type in ('date', 'datetime'):
+                return col_type
+            elif col_type == 'timestamp':
+                return 'datetime'
+            else:
+                return 'None'
+
+        key = None
+        super_columns = []
+        columns = db.do_query(self.sql % table)
+        for col in columns:
+            if col['pk'] == 1:
+                key = col['name']
+            if col['name'] in base_columns:
+                super_columns.append(col)
+            col['DATA_TYPE'] = convert_type(col['type'])
+            col['COLUMN_NAME'] = col['name']
+
+        if key is None:
+            return table
+
+        class_name = self._get_class_name(table)
+        return {
+            'key': key,
+            'table': table,
+            'class_name': class_name,
+            'columns': columns,
+            'self_columns': [col for col in columns if col['name'] not in base_columns],
+            'super_columns': super_columns
+        }
```

### Comparing `sqlx-orm-generator-0.0.1/orm_generator/postgresql.py` & `sqlx-orm-generator-0.0.2/orm_generator/postgresql.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,64 @@
-import sqlexec as db
-from orm.constant import KEY, UPDATE_BY, UPDATE_TIME, DEL_FLAG, KEY_SEQ, TABLE, KEY_STRATEGY
-from .base import BaseGenerator
-
-COMMON_COLS = ['create_by', 'create_time']
-ATTRIBUTES = {KEY: 'id', UPDATE_BY: 'update_by', UPDATE_TIME: 'update_time', DEL_FLAG: 'del_flag'}
-
-
-class PostgresqlGenerator(BaseGenerator):
-    comma1 = ','
-    comma2 = '，'
-    sql = '''SELECT column_name as "COLUMN_NAME", udt_name as "DATA_TYPE", column_default 
-             FROM information_schema.columns WHERE table_schema='public' AND table_name = ?'''
-    key_sql = '''SELECT a.attname FROM pg_index i
-                 JOIN pg_attribute a ON a.attrelid = i.indrelid AND a.attnum = any(i.indkey)
-                 WHERE i.indrelid = ?::regclass AND i.indisprimary LIMIT 1'''
-    show_table_sql = '''
-    SELECT tablename FROM pg_catalog.pg_tables  
-     WHERE schemaname != 'pg_catalog'  
-       AND schemaname != 'information_schema'
-    '''
-
-    def __init__(self):
-        super().__init__('postgresql.tpl', self.show_table_sql, [KEY, KEY_SEQ, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, KEY_STRATEGY])
-
-    def _get_table_meta(self, table: str, base_columns):
-        def convert_type(col_type):
-            if col_type.startswith('int'):
-                return 'int'
-            elif col_type .startswith('float'):
-                return 'float'
-            elif col_type in('numeric'):
-                return 'Decimal'
-            elif col_type in ('char', 'varchar', 'text'):
-                return 'str'
-            elif col_type == 'timestamp':
-                return 'datetime'
-            elif col_type == 'date':
-                return col_type
-            else:
-                return 'None'
-
-        key, key_seq, super_columns = None, None, []
-        columns = db.do_query(self.sql, table)
-        for col in columns:
-            if col['COLUMN_NAME'] in base_columns:
-                super_columns.append(col)
-            col['DATA_TYPE'] = convert_type(col['DATA_TYPE'])
-
-            if col['column_default'] and col['column_default'].startswith('nextval('):
-                key = col['COLUMN_NAME']
-                key_seq = col['column_default'][9:-12]
-
-        if key is None:
-            key = db.do_get(self.key_sql, table)
-            if key is None:
-                return table
-
-        class_name = self._get_class_name(table)
-        return {
-            'key': key,
-            'key_seq': key_seq,
-            'table': table,
-            'class_name': class_name,
-            'columns': columns,
-            'self_columns': [col for col in columns if col['COLUMN_NAME'] not in base_columns],
-            'super_columns': super_columns
-        }
-
+import sqlexec as db
+from orm.constant import KEY, UPDATE_BY, UPDATE_TIME, DEL_FLAG, KEY_SEQ, TABLE, KEY_STRATEGY
+from .base import BaseGenerator
+
+COMMON_COLS = ['create_by', 'create_time']
+ATTRIBUTES = {KEY: 'id', UPDATE_BY: 'update_by', UPDATE_TIME: 'update_time', DEL_FLAG: 'del_flag'}
+
+
+class PostgresqlGenerator(BaseGenerator):
+    comma1 = ','
+    comma2 = '，'
+    sql = '''SELECT column_name as "COLUMN_NAME", udt_name as "DATA_TYPE", column_default 
+             FROM information_schema.columns WHERE table_schema='public' AND table_name = ?'''
+    key_sql = '''SELECT a.attname FROM pg_index i
+                 JOIN pg_attribute a ON a.attrelid = i.indrelid AND a.attnum = any(i.indkey)
+                 WHERE i.indrelid = ?::regclass AND i.indisprimary LIMIT 1'''
+
+    def __init__(self):
+        super().__init__('postgresql.tpl', [KEY, KEY_SEQ, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, KEY_STRATEGY])
+
+    def _get_table_meta(self, table: str, base_columns):
+        def convert_type(col_type):
+            if col_type.startswith('int'):
+                return 'int'
+            elif col_type .startswith('float'):
+                return 'float'
+            elif col_type in('numeric'):
+                return 'Decimal'
+            elif col_type in ('char', 'varchar', 'text'):
+                return 'str'
+            elif col_type == 'timestamp':
+                return 'datetime'
+            elif col_type == 'date':
+                return col_type
+            else:
+                return 'None'
+
+        key, key_seq, super_columns = None, None, []
+        columns = db.do_query(self.sql, table)
+        for col in columns:
+            if col['COLUMN_NAME'] in base_columns:
+                super_columns.append(col)
+            col['DATA_TYPE'] = convert_type(col['DATA_TYPE'])
+
+            if col['column_default'] and col['column_default'].startswith('nextval('):
+                key = col['COLUMN_NAME']
+                key_seq = col['column_default'][9:-12]
+
+        if key is None:
+            key = db.do_get(self.key_sql, table)
+            if key is None:
+                return table
+
+        class_name = self._get_class_name(table)
+        return {
+            'key': key,
+            'key_seq': key_seq,
+            'table': table,
+            'class_name': class_name,
+            'columns': columns,
+            'self_columns': [col for col in columns if col['COLUMN_NAME'] not in base_columns],
+            'super_columns': super_columns
+        }
+
```

### Comparing `sqlx-orm-generator-0.0.1/setup.py` & `sqlx-orm-generator-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import os
-from setuptools import setup
-
-def read(rel_path: str) -> str:
-    here = os.path.abspath(os.path.dirname(__file__))
-    # intentionally *not* adding an encoding option to open, See:
-    #   https://github.com/pypa/virtualenv/issues/201#issuecomment-3145690
-    with open(os.path.join(here, rel_path), 'r', encoding='UTF-8') as fp:
-        return fp.read()
-
-long_description = read("README.rst")
-
-setup(
-    name='sqlx-orm-generator',
-    packages=['orm_generator'],
-    description="sqlx-orm-generator is a model code generator from tables for sqlx-orm_generator.",
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    install_requires=[
-        'Jinja2>=2.7.0',
-        'sqlx-orm>=0.0.6',
-    ],
-    version='0.0.1',
-    url='https://gitee.com/summry/sqlx-orm-generator',
-    author='summry',
-    author_email='xiazhongbiao@126.com',
-    keywords=['MySQL', 'mysqlx', 'python'],
-    package_data={
-        # include json and txt files
-        '': ['*.rst', '*.dtd', '*.tpl'],
-    },
-    include_package_data=True,
-    python_requires='>=3.5',
-    zip_safe=False
-)
-
+import os
+from setuptools import setup
+
+def read(rel_path: str) -> str:
+    here = os.path.abspath(os.path.dirname(__file__))
+    # intentionally *not* adding an encoding option to open, See:
+    #   https://github.com/pypa/virtualenv/issues/201#issuecomment-3145690
+    with open(os.path.join(here, rel_path), 'r', encoding='UTF-8') as fp:
+        return fp.read()
+
+long_description = read("README.rst")
+
+setup(
+    name='sqlx-orm-generator',
+    packages=['orm_generator'],
+    description="sqlx-orm-generator is a model code generator from tables for sqlx-orm_generator.",
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    install_requires=[
+        'Jinja2>=2.7.0',
+        'sqlx-orm>=0.0.7',
+    ],
+    version='0.0.2',
+    url='https://gitee.com/summry/sqlx-orm-generator',
+    author='summry',
+    author_email='xiazhongbiao@126.com',
+    keywords=['MySQL', 'mysqlx', 'python'],
+    package_data={
+        # include json and txt files
+        '': ['*.rst', '*.dtd', '*.tpl'],
+    },
+    include_package_data=True,
+    python_requires='>=3.5',
+    zip_safe=False
+)
+
```

### Comparing `sqlx-orm-generator-0.0.1/sqlx_orm_generator.egg-info/PKG-INFO` & `sqlx-orm-generator-0.0.2/sqlx_orm_generator.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,82 @@
-Metadata-Version: 2.1
-Name: sqlx-orm-generator
-Version: 0.0.1
-Summary: sqlx-orm-generator is a model code generator from tables for sqlx-orm_generator.
-Home-page: https://gitee.com/summry/sqlx-orm-generator
-Author: summry
-Author-email: xiazhongbiao@126.com
-License: UNKNOWN
-Description: Install
-        '''''''
-        
-        .. code:: shell
-        
-           pip install mysqlx-generator
-        
-        Usage Sample
-        ''''''''''''
-        
-        .. code:: python
-        
-               from orm_generator import Generator
-        
-               if __name__ == '__main__':
-                   coder = Generator(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test')
-                   # you can generate a model class for one table
-                   coder.generate_with_tables(tables='user', path='models.py')
-                   # you can generate model classes for tables
-                   coder.generate_with_tables(tables=['user', 'person'], path='models.py')
-                   # you can generate model classes for all tables from a given schema. default current schema if not given
-                   coder.generate_with_schema(schema='test', path='models.py')
-        
-        If you run last code, then generate a file 'models.py' in current
-        directory like follow:
-        
-        .. code:: python
-        
-               from decimal import Decimal
-               from datetime import date, datetime
-               from orm import Model, KeyStrategy
-        
-               class BaseModel(Model):
-                   __key__ = 'id'
-                   __del_flag__ = 'del_flag'
-                   __update_by__ = 'update_by'
-                   __update_time__ = 'update_time'
-                   __key_strategy__ = KeyStrategy.DB_AUTO_INCREMENT
-        
-                   def __init__(self, id: int = None, create_by: int = None, create_time: datetime = None, update_by: int = None, update_time: datetime = None,
-                           del_flag: int = None):
-                       self.id = id
-                       self.create_by = create_by
-                       self.create_time = create_time
-                       self.update_by = update_by
-                       self.update_time = update_time
-                       self.del_flag = del_flag
-        
-        
-               class User(BaseModel):
-                   __table__ = 'user'
-        
-                   def __init__(self, id: int = None, name: str = None, age: int = None, birth_date: date = None, sex: int = None, grade: float = None,
-                           point: float = None, money: Decimal = None, create_by: int = None, create_time: datetime = None, update_by: int = None,
-                           update_time: datetime = None, del_flag: int = None):
-                       super().__init__(id=id, create_by=create_by, create_time=create_time, update_by=update_by, update_time=update_time, del_flag=del_flag)
-                       self.name = name
-                       self.age = age
-                       self.birth_date = birth_date
-                       self.sex = sex
-                       self.grade = grade
-                       self.point = point
-                       self.money = money
-        
-        
-        MySqlx: https://pypi.org/project/mysqlx
-        
-Keywords: MySQL,mysqlx,python
-Platform: UNKNOWN
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: sqlx-orm-generator
+Version: 0.0.2
+Summary: sqlx-orm-generator is a model code generator from tables for sqlx-orm_generator.
+Home-page: https://gitee.com/summry/sqlx-orm-generator
+Author: summry
+Author-email: xiazhongbiao@126.com
+License: UNKNOWN
+Keywords: MySQL,mysqlx,python
+Platform: UNKNOWN
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Install
+'''''''
+
+.. code:: shell
+
+   pip install mysqlx-generator
+
+Usage Sample
+''''''''''''
+
+.. code:: python
+
+       from orm_generator import Generator
+
+       if __name__ == '__main__':
+           coder = Generator(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test')
+           # you can generate a model class for one table
+           coder.generate_with_tables(tables='user', path='models.py')
+           # you can generate model classes for tables
+           coder.generate_with_tables(tables=['user', 'person'], path='models.py')
+           # you can generate model classes for all tables from a given schema. default current schema if not given
+           coder.generate_with_schema(schema='test', path='models.py')
+
+If you run last code, then generate a file 'models.py' in current
+directory like follow:
+
+.. code:: python
+
+       from decimal import Decimal
+       from datetime import date, datetime
+       from orm import Model, KeyStrategy
+
+       class BaseModel(Model):
+           __key__ = 'id'
+           __del_flag__ = 'del_flag'
+           __update_by__ = 'update_by'
+           __update_time__ = 'update_time'
+           __key_strategy__ = KeyStrategy.DB_AUTO_INCREMENT
+
+           def __init__(self, id: int = None, create_by: int = None, create_time: datetime = None, update_by: int = None, update_time: datetime = None,
+                   del_flag: int = None):
+               self.id = id
+               self.create_by = create_by
+               self.create_time = create_time
+               self.update_by = update_by
+               self.update_time = update_time
+               self.del_flag = del_flag
+
+
+       class User(BaseModel):
+           __table__ = 'user'
+
+           def __init__(self, id: int = None, name: str = None, age: int = None, birth_date: date = None, sex: int = None, grade: float = None,
+                   point: float = None, money: Decimal = None, create_by: int = None, create_time: datetime = None, update_by: int = None,
+                   update_time: datetime = None, del_flag: int = None):
+               super().__init__(id=id, create_by=create_by, create_time=create_time, update_by=update_by, update_time=update_time, del_flag=del_flag)
+               self.name = name
+               self.age = age
+               self.birth_date = birth_date
+               self.sex = sex
+               self.grade = grade
+               self.point = point
+               self.money = money
+
+
+MySqlx: https://pypi.org/project/mysqlx
+
+
```

