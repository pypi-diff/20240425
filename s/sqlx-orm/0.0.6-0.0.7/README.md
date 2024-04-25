# Comparing `tmp/sqlx-orm-0.0.6.tar.gz` & `tmp/sqlx-orm-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-orm-0.0.6.tar", last modified: Mon Apr 22 02:20:33 2024, max compression
+gzip compressed data, was "sqlx-orm-0.0.7.tar", last modified: Thu Apr 25 08:16:19 2024, max compression
```

## Comparing `sqlx-orm-0.0.6.tar` & `sqlx-orm-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 02:20:33.000000 sqlx-orm-0.0.6/
-drwxrwxrwx   0        0        0        0 2024-04-22 02:20:33.000000 sqlx-orm-0.0.6/orm/
--rw-rw-rw-   0        0        0     1064 2024-04-22 01:59:30.000000 sqlx-orm-0.0.6/orm/constant.py
--rw-rw-rw-   0        0        0     2392 2024-04-22 01:59:30.000000 sqlx-orm-0.0.6/orm/log_support.py
--rw-rw-rw-   0        0        0    30035 2024-04-22 01:59:30.000000 sqlx-orm-0.0.6/orm/orm.py
--rw-rw-rw-   0        0        0    14408 2024-04-22 01:59:30.000000 sqlx-orm-0.0.6/orm/orm_support.py
--rw-rw-rw-   0        0        0     2674 2024-04-22 01:59:30.000000 sqlx-orm-0.0.6/orm/snowflake.py
--rw-rw-rw-   0        0        0      135 2024-04-22 01:59:30.000000 sqlx-orm-0.0.6/orm/support.py
--rw-rw-rw-   0        0        0      303 2024-04-22 01:59:30.000000 sqlx-orm-0.0.6/orm/__init__.py
--rw-rw-rw-   0        0        0     2219 2024-04-22 02:20:33.000000 sqlx-orm-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1792 2024-04-22 01:59:30.000000 sqlx-orm-0.0.6/README.rst
--rw-rw-rw-   0        0        0       42 2024-04-22 02:20:33.000000 sqlx-orm-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1248 2024-04-22 02:17:40.000000 sqlx-orm-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 02:20:33.000000 sqlx-orm-0.0.6/sqlx_orm.egg-info/
--rw-rw-rw-   0        0        0        1 2024-04-22 02:20:32.000000 sqlx-orm-0.0.6/sqlx_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-22 01:59:55.000000 sqlx-orm-0.0.6/sqlx_orm.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2219 2024-04-22 02:20:32.000000 sqlx-orm-0.0.6/sqlx_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-04-22 02:20:32.000000 sqlx-orm-0.0.6/sqlx_orm.egg-info/requires.txt
--rw-rw-rw-   0        0        0      322 2024-04-22 02:20:32.000000 sqlx-orm-0.0.6/sqlx_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        4 2024-04-22 02:20:32.000000 sqlx-orm-0.0.6/sqlx_orm.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-25 08:16:19.980454 sqlx-orm-0.0.7/
+-rw-r--r--   0 summy      (501) staff       (20)     2127 2024-04-25 08:16:19.979749 sqlx-orm-0.0.7/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)     1733 2024-04-04 10:08:32.000000 sqlx-orm-0.0.7/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-25 08:16:19.967272 sqlx-orm-0.0.7/orm/
+-rw-r--r--   0 summy      (501) staff       (20)      288 2024-04-04 08:43:34.000000 sqlx-orm-0.0.7/orm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     1036 2024-04-05 02:16:39.000000 sqlx-orm-0.0.7/orm/constant.py
+-rw-r--r--   0 summy      (501) staff       (20)     2344 2024-04-05 02:37:00.000000 sqlx-orm-0.0.7/orm/log_support.py
+-rw-r--r--   0 summy      (501) staff       (20)    29313 2024-04-21 13:10:06.000000 sqlx-orm-0.0.7/orm/orm.py
+-rw-r--r--   0 summy      (501) staff       (20)    14014 2024-04-21 13:02:31.000000 sqlx-orm-0.0.7/orm/orm_support.py
+-rw-r--r--   0 summy      (501) staff       (20)     2603 2024-04-04 01:12:05.000000 sqlx-orm-0.0.7/orm/snowflake.py
+-rw-r--r--   0 summy      (501) staff       (20)      128 2024-04-04 01:12:05.000000 sqlx-orm-0.0.7/orm/support.py
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-04-25 08:16:19.980706 sqlx-orm-0.0.7/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1185 2024-04-25 08:16:15.000000 sqlx-orm-0.0.7/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-25 08:16:19.978477 sqlx-orm-0.0.7/sqlx_orm.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     2127 2024-04-25 08:16:19.000000 sqlx-orm-0.0.7/sqlx_orm.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      322 2024-04-25 08:16:19.000000 sqlx-orm-0.0.7/sqlx_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-25 08:16:19.000000 sqlx-orm-0.0.7/sqlx_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-04 10:07:39.000000 sqlx-orm-0.0.7/sqlx_orm.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       17 2024-04-25 08:16:19.000000 sqlx-orm-0.0.7/sqlx_orm.egg-info/requires.txt
+-rw-r--r--   0 summy      (501) staff       (20)        4 2024-04-25 08:16:19.000000 sqlx-orm-0.0.7/sqlx_orm.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sqlx-orm-0.0.6/orm/constant.py` & `sqlx-orm-0.0.7/orm/constant.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from sqlexec.constant import LIMIT_1
-
-NO_LIMIT = 0
-
-CACHE_SIZE = 256
-
-MAPPER_PATH = 'mapper_path'
-
-MYSQL_SELECT_KEY = "SELECT LAST_INSERT_ID()"
-
-SQLITE_SELECT_KEY = 'SELECT last_insert_rowid()'
-
-MYSQL_COLUMN_SQL = '''SELECT GROUP_CONCAT(CONCAT("`",column_name,"`") SEPARATOR ",") 
-                        FROM information_schema.columns WHERE table_schema = (SELECT DATABASE()) AND table_name = ? LIMIT ?'''
-
-POSTGRES_COLUMN_SQL = '''SELECT array_to_string(array_agg(column_name),',') as column_name FROM information_schema.columns 
-                          WHERE table_schema='public' and table_name = ? LIMIT ?'''
-
-DYNAMIC_REGEX = '{%|{{|}}|%}'
-
-DEFAULT_KEY_FIELD = 'id'
-
-KEY, SELECT_KEY, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, KEY_STRATEGY = '__key__', '__select_key__', '__table__', \
-                                                                         '__update_by__', '__update_time__',\
-                                                                         '__del_flag__', '__key_strategy__'
-
-KEY_SEQ = '__key_seq__'
-
+from sqlexec.constant import LIMIT_1
+
+NO_LIMIT = 0
+
+CACHE_SIZE = 256
+
+MAPPER_PATH = 'mapper_path'
+
+MYSQL_SELECT_KEY = "SELECT LAST_INSERT_ID()"
+
+SQLITE_SELECT_KEY = 'SELECT last_insert_rowid()'
+
+MYSQL_COLUMN_SQL = '''SELECT GROUP_CONCAT(CONCAT("`",column_name,"`") SEPARATOR ",") 
+                        FROM information_schema.columns WHERE table_schema = (SELECT DATABASE()) AND table_name = ? LIMIT ?'''
+
+POSTGRES_COLUMN_SQL = '''SELECT array_to_string(array_agg(column_name),',') as column_name FROM information_schema.columns 
+                          WHERE table_schema='public' and table_name = ? LIMIT ?'''
+
+DYNAMIC_REGEX = '{%|{{|}}|%}'
+
+DEFAULT_KEY_FIELD = 'id'
+
+KEY, SELECT_KEY, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, KEY_STRATEGY = '__key__', '__select_key__', '__table__', \
+                                                                         '__update_by__', '__update_time__',\
+                                                                         '__del_flag__', '__key_strategy__'
+
+KEY_SEQ = '__key_seq__'
+
```

### Comparing `sqlx-orm-0.0.6/orm/log_support.py` & `sqlx-orm-0.0.7/orm/log_support.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from sqlexec.log_support import logger
-
-
-def orm_insert_log(function, class_name, **kwargs):
-    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', kwargs: %s" % (function, class_name, kwargs))
-
-
-def orm_delete_by_id_log(function, class_name, _id, update_by):
-    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', id: %d, update_by: %s" % (function, class_name, _id, update_by))
-
-
-def orm_by_log(function, class_name, where, *args, **kwargs):
-    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', where: %s, args: %s, kwargs: %s" % (function, class_name, where, args, kwargs))
-
-
-def orm_inst_log(function, class_name):
-    logger.debug("Exec func 'sqlbatis.orm.Model.%s', Class: '%s'" % (function, class_name))
-
-
-def orm_logical_delete_by_ids_log(function, class_name, ids, update_by, batch_size):
-    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', ids: %s, update_by: %s, batch_size: %s" % (
-        function, class_name, ids, update_by, batch_size))
-
-
-def orm_count_log(function, class_name, **kwargs):
-    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', kwargs: %s" % (function, class_name, kwargs))
-
-
-def orm_find_log(function, class_name, *fields, **kwargs):
-    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', fields: %s, kwargs: %s" % (function, class_name, fields, kwargs))
-
-
-def orm_find_by_id_log(function, class_name, _id, *fields):
-    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', id: %d, fields: %s" % (function, class_name, _id, fields))
-
-
-def orm_find_by_ids_log(function, class_name, ids, *fields):
-    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', ids: %s, fields: %s" % (function, class_name, ids, fields))
-
-
-def orm_page_log(function, page_num, page_size, class_name, *fields, **kwargs):
-    logger.debug("Exec func 'pgsqlx.orm.Model.%s', page_num: %d, page_size: %d \n\t Class: '%s', fields: %s, kwargs: %s" % (
-        function, page_num, page_size, class_name, fields, kwargs))
-
-
-def orm_by_page_log(function, page_num, page_size, class_name, where, *args, **kwargs):
-    logger.debug("Exec func 'sqlx-batis.orm.Model.%s', page_num: %d, page_size: %d \n\t Class: '%s', where: %s, args: %s, kwargs: %s" % (
-        function, page_num, page_size, class_name, where, args, kwargs))
+from sqlexec.log_support import logger
+
+
+def orm_insert_log(function, class_name, **kwargs):
+    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', kwargs: %s" % (function, class_name, kwargs))
+
+
+def orm_delete_by_id_log(function, class_name, _id, update_by):
+    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', id: %d, update_by: %s" % (function, class_name, _id, update_by))
+
+
+def orm_by_log(function, class_name, where, *args, **kwargs):
+    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', where: %s, args: %s, kwargs: %s" % (function, class_name, where, args, kwargs))
+
+
+def orm_inst_log(function, class_name):
+    logger.debug("Exec func 'sqlbatis.orm.Model.%s', Class: '%s'" % (function, class_name))
+
+
+def orm_logical_delete_by_ids_log(function, class_name, ids, update_by, batch_size):
+    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', ids: %s, update_by: %s, batch_size: %s" % (
+        function, class_name, ids, update_by, batch_size))
+
+
+def orm_count_log(function, class_name, **kwargs):
+    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', kwargs: %s" % (function, class_name, kwargs))
+
+
+def orm_find_log(function, class_name, *fields, **kwargs):
+    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', fields: %s, kwargs: %s" % (function, class_name, fields, kwargs))
+
+
+def orm_find_by_id_log(function, class_name, _id, *fields):
+    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', id: %d, fields: %s" % (function, class_name, _id, fields))
+
+
+def orm_find_by_ids_log(function, class_name, ids, *fields):
+    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', ids: %s, fields: %s" % (function, class_name, ids, fields))
+
+
+def orm_page_log(function, page_num, page_size, class_name, *fields, **kwargs):
+    logger.debug("Exec func 'pgsqlx.orm.Model.%s', page_num: %d, page_size: %d \n\t Class: '%s', fields: %s, kwargs: %s" % (
+        function, page_num, page_size, class_name, fields, kwargs))
+
+
+def orm_by_page_log(function, page_num, page_size, class_name, where, *args, **kwargs):
+    logger.debug("Exec func 'sqlx-batis.orm.Model.%s', page_num: %d, page_size: %d \n\t Class: '%s', where: %s, args: %s, kwargs: %s" % (
+        function, page_num, page_size, class_name, where, args, kwargs))
```

### Comparing `sqlx-orm-0.0.6/orm/orm.py` & `sqlx-orm-0.0.7/orm/orm.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,722 +1,722 @@
-import sys
-from datetime import datetime
-from enum import Enum, IntEnum
-from typing import Sequence, Union
-from .snowflake import get_snowflake_id
-from .support import DBError, NotFoundError
-from . import db, log_support, transaction, orm_support, Dialect
-from .constant import LIMIT_1, NO_LIMIT, DEFAULT_KEY_FIELD, KEY, SELECT_KEY, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, \
-    KEY_STRATEGY, KEY_SEQ
-
-
-class DelFlag(IntEnum):
-    UN_DELETE = 0
-    DELETED = 1
-
-
-class KeyStrategy(Enum):
-    """
-    SNOWFLAKE: 由Snowflake算法生成主键
-    DB_AUTO_INCREMENT: 由数据库的AUTO_INCREMENT自动生成主键
-
-    在Windows上，使用Snowflake可能会报下列错误，这是因为Snowflake生成的id是15位的数字，而Windows上C语言的long类型是32位的
-    OverflowError: Python int too large to convert to C long
-
-    如果用的是mysql.connector，且在Windows上开发测试，可以就在初始化数据库的时候加上参数'use_pure'为True用纯python的connect; 在linux是部署生成环境时去掉'use_pure'用
-    C语言写的connect, 以提高性能.
-    """
-    SNOWFLAKE = 'snowflake'
-    DB_AUTO_INCREMENT = 'db_auto_increment'
-
-
-class Model:
-    """
-    Create a class extends Model:
-
-    class Person(Model):
-        __key__ = 'id'
-        __table__ = 'person'
-        __update_by__ = 'update_by'
-        __update_time__ = 'update_time'
-        __del_flag__ = 'del_flag'
-        __key_seq__ = 'person_id_seq'
-
-        def __init__(self, id: int = None, name: str = None, age: int = None, update_by: int = None, update_time: datetime = None, del_flag: int = None):
-            self.id = id
-
-            self.update_by = update_by
-            self.update_time = update_time
-            self.del_flag = del_flag
-            self.name = name
-            self.age = age
-
-    then you can use like follow:
-        orm.init(person='xxx', password='xxx', database='xxx', host='xxx', ...)  # or db.init(...) init db first,
-        person = Person(name='张三', age=55)
-        effect_rowcount = person.persist()
-        id = person.inst_save()
-    """
-
-    def __str__(self):
-        return str({k: v for k, v in self.__dict__.items() if not k.startswith("__")})
-
-    def __getattr__(self, name):
-        if KEY == name:
-            return self._get_key()
-        elif TABLE == name:
-            return self.get_table()
-        elif UPDATE_BY == name:
-            return self._get_update_by_field()
-        elif UPDATE_TIME == name:
-            return self._get_update_time_field()
-        else:
-            return None
-
-    def persist(self, ignored_none=True, *fields):
-        """
-        person = Person(name='张三', age=55)
-        effect_rowcount = person.persist()
-        :return: effect rowcount
-        """
-        log_support.orm_inst_log('persist', self.__class__.__name__)
-        kv = self._get_kv(ignored_none, None, *fields)
-        return self.insert(**kv)
-
-    def inst_save(self, ignored_none=True, *fields):
-        """
-        person = Person(name='张三', age=55)
-        id = person.save()
-        :return: Primary key
-        """
-        log_support.orm_inst_log('inst_save', self.__class__.__name__)
-        key = self._get_key()
-        kv = self._get_kv(ignored_none, None, *fields)
-        _id = self.save(**kv)
-        if key not in kv:
-            self.__dict__.update({key: _id})
-        return _id
-
-    def update(self, ignored_none=True, *fields):
-        """
-        person = Person(id=1, name='李四', age=66)
-        rowcount = person.update()
-        :return: Effect rowcount
-        """
-        log_support.orm_inst_log('update', self.__class__.__name__)
-        key, table = self._get_key_and_table()
-        kv = self._get_kv(ignored_none, key, *fields)
-        _id = kv[key]
-        assert _id is not None, 'Primary key must not be None.'
-        update_kv = {k: v for k, v in kv.items() if k != key}
-        if update_kv:
-            return self.update_by_id(_id, **update_kv)
-        else:
-            log_support.logger.warning("Exec func 'sqlbatis.orm.Model.%s' not set fields, Class: '%s:'\n\t   %s" % ('update', self.__class__.__name__, self))
-            return 0
-
-    def load(self, *fields):
-        """
-        Return new object from database and update itself.
-        :param fields: Default select all fields if not set. like: ('id', 'name', 'age')
-        person = Person(id=1)
-        person2 = person.load()
-        """
-        log_support.logger.debug("Exec func 'sqlbatis.orm.Model.%s', Class: '%s', fields: %s" % ('load', self.__class__.__name__, fields))
-        key = self._get_key()
-        kv = self.__dict__
-        _id = kv.get(key)
-        assert _id is not None, 'Primary key must not be None.'
-        if not fields:
-            fields, _ = zip(*kv.items())
-        result = self.query_by_id(_id, *fields)
-        if result:
-            self.__dict__.update(result)
-            return self
-        else:
-            raise NotFoundError("Load not found from db, Class: '%s', %s=%d." % (self.__class__.__name__, key, _id))
-
-    def logical_delete(self):
-        """
-        Logic delete only update the del flag
-        person = Person(id=1)
-        rowcount = person.logical_delete()
-        """
-        log_support.orm_inst_log('logical_delete', self.__class__.__name__)
-        key = self._get_key()
-        kv = self.__dict__
-        _id = kv.get(key)
-        assert _id is not None, 'Primary key must not be None.'
-        update_by = kv.get(self._get_update_by_field())
-        return self.logical_delete_by_id(_id, update_by)
-
-    def logical_undelete(self):
-        """
-        Logic un delete only update the del flag
-        person = Person(id=1)
-        rowcount = person.logical_undelete()
-        """
-        log_support.orm_inst_log('logical_undelete', self.__class__.__name__)
-        key = self._get_key()
-        kv = self.__dict__
-        _id = kv.get(key)
-        assert _id is not None, 'Primary key must not be None.'
-        update_by = kv.get(self._get_update_by_field())
-        return self.logical_undelete_by_id(_id, update_by)
-
-    def remove(self):
-        """
-        Physical delete
-        person = Person(id=1)
-        rowcount = person.remove()
-        """
-        log_support.orm_inst_log('remove', self.__class__.__name__)
-        key = self._get_key()
-        _id = self.__dict__.get(key)
-        assert _id is not None, 'Primary key must not be None.'
-        return self.delete_by_id(_id)
-
-    # ----------------------------------------------------------Class method------------------------------------------------------------------
-    @classmethod
-    def insert(cls, **kwargs):
-        """
-        rowcount = Person.insert(name='张三', age=20)
-        return: Effect rowcount
-        """
-        log_support.orm_insert_log('insert', cls.__name__, **kwargs)
-        key, table = cls._get_key_and_table()
-        key_strategy = cls._get_key_strategy()
-        if key_strategy == KeyStrategy.SNOWFLAKE and key not in kwargs:
-            kwargs[key] = get_snowflake_id()
-        return db.insert(table, **kwargs)
-
-    @classmethod
-    def save(cls, **kwargs):
-        """
-        id = Person.save(name='张三', age=20)
-        :return: Primary key
-        """
-        log_support.orm_insert_log('save', cls.__name__, **kwargs)
-        key, table = cls._get_key_and_table()
-        if key in kwargs:
-            db.insert(table, **kwargs)
-            return kwargs[key]
-
-        key_strategy = cls._get_key_strategy()
-        if key_strategy == KeyStrategy.SNOWFLAKE:
-            kwargs[key] = get_snowflake_id()
-            db.insert(table, **kwargs)
-            return kwargs[key]
-        else:
-            select_key = cls._get_select_key()
-            if not select_key:
-                keq_seq = cls._get_key_seq()
-                try:
-                    select_key = Dialect.get_select_key(keq_seq=keq_seq, table=table, key=key)
-                except NotImplementedError:
-                    raise DBError("Expect 'select_key'. you can set it in model class with '__select_key__'. "
-                                  "You can also set primary key sequence with '__key_seq__' for PostgreSQL.'")
-            return db.save_select_key(select_key, table, **kwargs)
-
-    @classmethod
-    def create(cls, **kwargs):
-        """
-        person = Person.create(name='张三', age=20)
-        :return: Instance object
-        """
-        log_support.orm_insert_log('create', cls.__name__, **kwargs)
-        key = cls._get_key()
-        kwargs[key] = cls.save(**kwargs)
-        return cls.to_obj(**kwargs)
-
-    @classmethod
-    def update_by_id(cls, _id: Union[int, str], **kwargs):
-        """
-        rowcount = Person.update_by_id(id=1, name='王五')
-        return: Effect rowcount
-        """
-        log_support.logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', id: %d, kwargs: %s" % ('update_by_id', cls.__name__, _id, kwargs))
-        assert kwargs, 'Must set update kv'
-        key, table_name = cls._get_key_and_table()
-        where_kwargs = {key: _id}
-        kwargs = cls._update_time(**kwargs)
-        db.table(table_name).where(**where_kwargs).update(**kwargs)
-
-    @classmethod
-    def logical_delete_by_id(cls, _id: Union[int, str], update_by: Union[int, str] = None):
-        """
-        Logic delete only update the del flag
-        rowcount = Person.delete_by_id(id=1, update_by=100)
-        return: Effect rowcount
-        """
-        log_support.orm_delete_by_id_log('logical_delete_by_id', cls.__name__, _id, update_by)
-        return cls._logical_delete_by_id_op(_id, update_by, DelFlag.DELETED)
-
-    @classmethod
-    def logical_undelete_by_id(cls, _id: Union[int, str], update_by: Union[int, str] = None):
-        """
-        Logic delete only update the del flag
-        rowcount = Person.logical_undelete_by_id(id=1, update_by=100)
-        return: Effect rowcount
-        """
-        log_support.orm_delete_by_id_log('logical_undelete_by_id', cls.__name__, _id, update_by)
-        return cls._logical_delete_by_id_op(_id, update_by, DelFlag.UN_DELETE)
-
-    @classmethod
-    def logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128):
-        """
-        Logic delete only update the del flag
-        rowcount = Person.logical_delete_by_ids(id=[1,2], update_by=100)
-        return: Effect rowcount
-        """
-        log_support.orm_logical_delete_by_ids_log('logical_delete_by_ids', cls.__name__, ids, update_by, batch_size)
-        return cls._logical_delete_by_ids_op(ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.DELETED)
-
-    @classmethod
-    def logical_undelete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128):
-        """
-        Logic delete only update the del flag
-        rowcount = Person.logical_undelete_by_ids(id=[1,2], update_by=100)
-        return: Effect rowcount
-        """
-        log_support.orm_logical_delete_by_ids_log('logical_undelete_by_ids', cls.__name__, ids, update_by, batch_size)
-        return cls._logical_delete_by_ids_op(ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.UN_DELETE)
-
-    @classmethod
-    def delete(cls, **kwargs):
-        """
-        Physical delete
-        rowcount = Person.delete(name='张三', age=55)
-        return: Effect rowcount
-        """
-        log_support.orm_count_log(sys._getframe().f_code.co_name, cls.__name__, **kwargs)
-        table = cls.get_table()
-        return db.table(table).where(**kwargs).delete()
-
-    @classmethod
-    def delete_by_id(cls, _id: Union[int, str]):
-        """
-        Physical delete
-        rowcount = Person.delete_by_id(id=1)
-        return: Effect rowcount
-        """
-        log_support.logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', id: %d" % ('delete_by_id', cls.__name__, _id))
-        key, table = cls._get_key_and_table()
-        where_kwargs = {key: _id}
-        return db.table(table).where(**where_kwargs).delete()
-
-    @classmethod
-    def delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], batch_size=128):
-        """
-        Batch physical delete, they will be executed in batches if there are too many
-        rowcount = Person.delete_by_ids(id=[1,2])
-        return: Effect rowcount
-        """
-        log_support.logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', ids: %s, batch_size: %s" % ('delete_by_ids', cls.__name__, ids, batch_size))
-        ids_size = len(ids)
-        assert ids_size > 0, 'ids must not be empty.'
-        if ids_size == 1:
-            return cls.delete_by_id(ids[0])
-        elif ids_size <= batch_size:
-            return cls.do_delete_by_ids(ids)
-        else:
-            slices = orm_support.split_ids(ids, batch_size)
-            with transaction():
-                results = list(map(cls.do_delete_by_ids, slices))
-            return sum(results)
-
-    @classmethod
-    def do_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]]):
-        """
-        Batch physical delete, please use delete_by_ids if there are too many
-        rowcount = Person.do_delete_by_ids(id=[1,2])
-        return: Effect rowcount
-        """
-        key, table = cls._get_key_and_table()
-        where_kwargs = {'{}__in'.format(key): ids}
-        return db.table(table).where(**where_kwargs).delete()
-
-    @classmethod
-    def batch_insert(cls, *args):
-        """
-        Batch insert
-        rowcount = Person.batch_insert([{'name': '张三', 'age': 55},{'name': '李四', 'age': 66}])
-        :param args: All number must have same key.
-        :return: Effect rowcount
-        """
-        log_support.logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', args: %s" % ('batch_insert', cls.__name__, args))
-        assert len(args) > 0, 'args must not be empty.'
-        key, table = cls._get_key_and_table()
-        key_strategy = cls._get_key_strategy()
-        if key_strategy == KeyStrategy.SNOWFLAKE:
-            for arg in args:
-                if key not in arg:
-                    arg[key] = get_snowflake_id()
-
-        return db.batch_insert(table, *args)
-
-    # ------------------------------------------------Class query method------------------------------------------------
-    @classmethod
-    def count(cls, **kwargs):
-        """
-        count = Person.count(name='张三', age=55)
-        """
-        log_support.orm_count_log('count', cls.__name__, **kwargs)
-        table = cls.get_table()
-        return db.table(table).where(**kwargs).count()
-
-    @classmethod
-    def exists(cls, **kwargs):
-        log_support.orm_count_log('exists', cls.__name__, **kwargs)
-        table = cls.get_table()
-        return db.table(table).where(**kwargs).exists()
-
-    @classmethod
-    def exists_by_id(cls, _id: Union[int, str]):
-        key = cls._get_key()
-        kwargs = {key: _id}
-        return cls.exists(**kwargs)
-
-    @classmethod
-    def find(cls, *fields, **kwargs):
-        """
-        Return list(object) or empty list if no result.
-        persons = Person.find('id', 'name', 'age', name='张三', age=55)
-        :param fields: Default select all fields if not set
-        """
-        log_support.orm_find_log('find', cls.__name__, *fields, **kwargs)
-        return [cls.to_obj(**d) for d in cls.query(*fields, **kwargs)]
-
-    @classmethod
-    def find_one(cls, *fields, **kwargs):
-        """
-        Return unique result(object) or None if no result.
-        person = Person.find_one('id', 'name', 'age', name='张三', age=55)
-        :param fields: Default select all fields if not set
-        """
-        log_support.orm_find_log('find_one', cls.__name__, *fields, **kwargs)
-        result = cls.query_one(*fields, **kwargs)
-        return cls.to_obj(**result) if result else None
-
-    @classmethod
-    def find_by_id(cls, _id: Union[int, str], *fields):
-        """
-        Return one class object or None if no result.
-        person = Person.find_by_id(1, 'id', 'name', 'age')
-        :param _id: key
-        :param fields: Default select all fields if not set
-        """
-        log_support.orm_find_by_id_log('find_by_id', cls.__name__, _id, *fields)
-        result = cls.query_by_id(_id, *fields)
-        return cls.to_obj(**result) if result else None
-
-    @classmethod
-    def find_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
-        """
-        Return list(class object) or empty list if no result.
-        persons = Person.find_by_ids([1,2], 'id', 'name', 'age')
-        :param ids: List of key
-        :param fields: Default select all fields if not set
-        """
-        log_support.orm_find_by_ids_log('find_by_ids', cls.__name__, ids, *fields)
-        return [cls.to_obj(**d) for d in cls.query_by_ids(ids, *fields)]
-
-    @classmethod
-    def query(cls, *fields, **kwargs):
-        """
-        Return list(dict) or empty list if no result.
-        persons = Person.query('id', 'name', 'age', name='张三', age=55)
-        :param fields: Default select all fields if not set
-        """
-        log_support.orm_find_log('query', cls.__name__, *fields, **kwargs)
-        table = cls.get_table()
-        return db.table(table).columns(*fields).where(**kwargs).query()
-
-    @classmethod
-    def query_one(cls, *fields, **kwargs):
-        """
-        Return unique result(dict) or None if no result.
-        persons = Person.query_one('id', 'name', 'age', name='张三', age=55)
-        :param fields: Default select all fields if not set
-        """
-        log_support.orm_find_log('query_one', cls.__name__, *fields, **kwargs)
-        table = cls.get_table()
-        return db.table(table).columns(*fields).where(**kwargs).query_one()
-
-    @classmethod
-    def query_by_id(cls, _id: Union[int, str], *fields):
-        """
-        Return one row(dict) or None if no result.
-        person = Person.query_by_id(1, 'id', 'name', 'age')
-        :param _id: key
-        :param fields: Default select all fields if not set
-        """
-        log_support.orm_find_by_id_log('query_by_id', cls.__name__, _id, *fields)
-        key, table = cls._get_key_and_table()
-        kwargs = {key: _id}
-        return db.table(table).columns(*fields).where(**kwargs).query_one()
-
-    @classmethod
-    def query_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
-        """
-        Return list(dict) or empty list if no result.
-        persons = Person.query_by_ids([1,2], 'id', 'name', 'age')
-        :param ids: List of key
-        :param fields: Default select all fields if not set
-        """
-        log_support.orm_find_by_ids_log('query_by_ids', cls.__name__, ids, *fields)
-        assert len(ids) > 0, 'ids must not be empty.'
-
-        key, table = cls._get_key_and_table()
-        kwargs = {'{}__in'.format(key): ids}
-        return db.table(table).columns(*fields).where(**kwargs).query()
-
-    @classmethod
-    def select(cls, *fields, **kwargs):
-        """
-        Return list(dict) or empty list if no result.
-        rows = Person.select('id', 'name', 'age', name='张三', age=55)
-        :param fields: Default select all fields if not set
-        """
-        log_support.orm_find_log('select', cls.__name__, *fields, **kwargs)
-        table = cls.get_table()
-        return db.table(table).columns(*fields).where(**kwargs).select()
-
-    @classmethod
-    def select_one(cls, *fields, **kwargs):
-        """
-        Return unique result(tuple) or None if no result.
-        row = Person.select_one('id', 'name', 'age', name='张三', age=55)
-        :param fields: Default select all fields if not set
-        """
-        log_support.orm_find_log('select_one', cls.__name__, *fields, **kwargs)
-        table = cls.get_table()
-        return db.table(table).columns(*fields).where(**kwargs).select_one()
-
-    @classmethod
-    def select_by_id(cls, _id: Union[int, str], *fields):
-        """
-        Return one row(dict) or None if no result.
-        row = Person.select_by_id(1, 'id', 'name', 'age')
-        :param _id: key
-        :param fields: Default select all fields if not set
-        """
-        log_support.orm_find_by_id_log('select_by_id', cls.__name__, _id, *fields)
-        key, table = cls._get_key_and_table()
-        kwargs = {key: _id}
-        return db.table(table).columns(*fields).where(**kwargs).select_one()
-
-    @classmethod
-    def select_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
-        """
-        Return list(dict) or empty list if no result.
-        rows = Person.select_by_ids([1,2], 'id', 'name', 'age')
-        :param ids: List of key
-        :param fields: Default select all fields if not set
-        """
-        log_support.orm_find_by_ids_log('select_by_ids', cls.__name__, ids, *fields)
-        assert len(ids) > 0, 'ids must not be empty.'
-
-        key, table = cls._get_key_and_table()
-        kwargs = {'{}__in'.format(key): ids}
-        return db.table(table).columns(*fields).where(**kwargs).select()
-
-    @classmethod
-    def find_page(cls, page_num=1, page_size=10, *fields, **kwargs):
-        """
-        Return list(object) or empty list if no result.
-        persons = Person.find_page(1, 10, 'name', 'age', name='张三', age=55)
-        :param page_num: page number
-        :param page_size: page size
-        :param fields: Default select all fields if not set
-        """
-        log_support.orm_page_log('find_page', page_num, page_size, cls.__name__, *fields, **kwargs)
-        result = cls.query_page(page_num, page_size, *fields, **kwargs)
-        return [cls.to_obj(**d) for d in result]
-
-    @classmethod
-    def query_page(cls, page_num=1, page_size=10, *fields, **kwargs):
-        """
-        Return list(dict) or empty list if no result.
-        persons = Person.query_page(1, 10, 'id', 'name', 'age', name='张三', age=55)
-        :param page_num: page number
-        :param page_size: page size
-        :param fields: Default select all fields if not set
-        """
-        log_support.orm_page_log('query_page', page_num, page_size, cls.__name__, *fields, **kwargs)
-        table = cls.get_table()
-        return db.table(table).columns(*fields).where(**kwargs).page(page_num, page_size).query()
-
-    @classmethod
-    def select_page(cls, page_num=1, page_size=10, *fields, **kwargs):
-        """
-        Return list(dict) or empty list if no result.
-        rows = Person.select_page('id', 'name', 'age', name='张三', age=55)
-        :param page_num: page number
-        :param page_size: page size
-        :param fields: Default select all fields if not set
-        """
-        log_support.orm_page_log('select_page', page_num, page_size, cls.__name__, *fields, **kwargs)
-        table = cls.get_table()
-        return db.table(table).columns(*fields).where(**kwargs).page(page_num, page_size).select()
-
-    @classmethod
-    def fields(cls, *fields) -> orm_support.FieldExec:
-        return orm_support.FieldExec(cls, *fields)
-
-    @classmethod
-    def where(cls, **kwargs) -> orm_support.WhereExec:
-        return orm_support.WhereExec(cls, **kwargs)
-
-    @classmethod
-    def page(cls, page_num=1, page_size=10) -> orm_support.PageExec:
-        return orm_support.PageExec(cls, page_num, page_size)
-
-    @classmethod
-    def to_obj(cls, **kwargs):
-        model = cls.__new__(cls)
-        model.__dict__.update(**kwargs)
-        return model
-
-    def _get_kv(self, ignored_none: bool, key: None, *fields):
-        if fields:
-            if key:
-                fields = (key, *fields)
-            if ignored_none:
-                return {k: v for k, v in self.__dict__.items() if v is not None and k in fields}
-            return {k: v for k, v in self.__dict__.items() if k in fields}
-
-        if ignored_none:
-            return {k: v for k, v in self.__dict__.items() if v is not None}
-        return {k: v for k, v in self.__dict__.items()}
-
-    # ------------------------------------------------Private class method----------------------------------------------
-    @classmethod
-    def _logical_delete_by_id_op(cls, _id: Union[int, str], update_by: Union[int, str] = None, del_status=DelFlag.DELETED):
-        key, table = cls._get_key_and_table()
-        del_flag_field = cls._get_del_flag_field()
-        update_by_field = cls._get_update_by_field()
-
-        where = '%s = ?' % key
-        if update_by is not None and update_by_field is not None:
-            sql, update_time_arg = cls._update_sql(where, del_flag_field, update_by_field)
-            if update_time_arg:
-                return db.do_execute(sql, del_status.value, update_by, update_time_arg, _id)
-            return db.do_execute(sql, del_status.value, update_by, _id)
-        else:
-            sql, update_time_arg = cls._update_sql(where, del_flag_field)
-            if update_time_arg:
-                return db.do_execute(sql, del_status.value, update_time_arg, _id)
-            return db.do_execute(sql, del_status.value, _id)
-
-    @classmethod
-    def _logical_delete_by_ids_op(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128,
-            del_status=DelFlag.DELETED):
-        ids_size = len(ids)
-        assert ids_size > 0, 'ids must not be empty.'
-
-        if ids_size == 1:
-            return cls._logical_delete_by_id_op(ids[0], update_by, del_status)
-        elif ids_size <= batch_size:
-            return cls._do_logical_delete_by_ids(ids, update_by, del_status)
-        else:
-            slices = orm_support.split_ids(ids, batch_size)
-            with transaction():
-                results = [cls._do_logical_delete_by_ids(ids, update_by, del_status) for ids in slices]
-            return sum(results)
-
-    @classmethod
-    def _do_logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, del_status=DelFlag.DELETED):
-        key = cls._get_key()
-        del_flag_field = cls._get_del_flag_field()
-        update_by_field = cls._get_update_by_field()
-
-        where = '%s in (%s)' % (key, ','.join(['?' for _ in range(len(ids))]))
-        if update_by is not None and update_by_field is not None:
-            sql, update_time_arg = cls._update_sql(where, del_flag_field, update_by_field)
-            if update_time_arg:
-                return db.do_execute(sql, del_status.value, update_by, update_time_arg, *ids)
-            return db.do_execute(sql, del_status.value, update_by, *ids)
-        else:
-            sql, update_time_arg = cls._update_sql(where, del_flag_field)
-            if update_time_arg:
-                return db.do_execute(sql, del_status.value, update_time_arg, *ids)
-            return db.do_execute(sql, del_status.value, *ids)
-
-    @classmethod
-    def _get_key(cls):
-        if hasattr(cls, KEY):
-            return cls.__key__
-        log_support.logger.warning("%s not set attribute '%s'" % (cls.__name__, KEY))
-        return DEFAULT_KEY_FIELD
-
-    @classmethod
-    def _get_select_key(cls):
-        return cls.__select_key__ if hasattr(cls, SELECT_KEY) else None
-
-    @classmethod
-    def _get_key_seq(cls):
-        return cls.__key_seq__ if hasattr(cls, KEY_SEQ) else None
-
-    @classmethod
-    def get_table(cls):
-        if hasattr(cls, TABLE):
-            return cls.__table__
-        log_support.logger.warning("%s not set attribute '%s'" % (cls.__name__, TABLE))
-        return orm_support.get_table_name(cls.__name__)
-
-    @classmethod
-    def _get_key_and_table(cls):
-        return cls._get_key(), cls.get_table()
-
-    @classmethod
-    def _get_key_strategy(cls):
-        if hasattr(cls, KEY_STRATEGY):
-            return cls.__key_strategy__
-        return None
-
-    @classmethod
-    def _get_update_by_field(cls):
-        if hasattr(cls, UPDATE_BY):
-            return cls.__update_by__
-        return None
-
-    @classmethod
-    def _get_update_time_field(cls):
-        if hasattr(cls, UPDATE_TIME):
-            return cls.__update_time__
-        return None
-
-    @classmethod
-    def _get_del_flag_field(cls):
-        assert hasattr(cls, DEL_FLAG), "%s not set attribute '%s'" % (cls.__name__, DEL_FLAG)
-        return cls.__del_flag__
-
-    @classmethod
-    def _update_time(cls, **kwargs):
-        update_time_field = cls._get_update_time_field()
-        if update_time_field is not None and update_time_field not in kwargs:
-            kwargs[update_time_field] = datetime.now()
-        return kwargs
-
-    @classmethod
-    def _update_sql(cls, where, *update_fields):
-        update_time_arg = None
-        table = cls.get_table()
-        table = Dialect.get_dialect_str(table)
-        update_time_field = cls._get_update_time_field()
-        if update_time_field is not None and update_time_field not in update_fields:
-            update_fields = [*update_fields, update_time_field]
-            update_time_arg = datetime.now()
-
-        update_fields = ', '.join(['{} = ?'.format(Dialect.get_dialect_str(col)) for col in update_fields])
-        return 'UPDATE {} SET {} WHERE {}'.format(table, update_fields, where), update_time_arg
-
-    @classmethod
-    def _where_sql(cls, where: str):
-        low_where = where.strip().lower()
-        if low_where.startswith('where'):
-            table = cls.get_table()
-            return orm_support.get_table_select_sql(table, where, NO_LIMIT)
-        elif low_where.startswith('select'):
-            return where
-        raise DBError("The where parameter must be a complete SQL statement or conditions start with 'where'")
+import sys
+from datetime import datetime
+from enum import Enum, IntEnum
+from typing import Sequence, Union
+from .snowflake import get_snowflake_id
+from .support import DBError, NotFoundError
+from . import db, log_support, transaction, orm_support, Dialect
+from .constant import LIMIT_1, NO_LIMIT, DEFAULT_KEY_FIELD, KEY, SELECT_KEY, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, \
+    KEY_STRATEGY, KEY_SEQ
+
+
+class DelFlag(IntEnum):
+    UN_DELETE = 0
+    DELETED = 1
+
+
+class KeyStrategy(Enum):
+    """
+    SNOWFLAKE: 由Snowflake算法生成主键
+    DB_AUTO_INCREMENT: 由数据库的AUTO_INCREMENT自动生成主键
+
+    在Windows上，使用Snowflake可能会报下列错误，这是因为Snowflake生成的id是15位的数字，而Windows上C语言的long类型是32位的
+    OverflowError: Python int too large to convert to C long
+
+    如果用的是mysql.connector，且在Windows上开发测试，可以就在初始化数据库的时候加上参数'use_pure'为True用纯python的connect; 在linux是部署生成环境时去掉'use_pure'用
+    C语言写的connect, 以提高性能.
+    """
+    SNOWFLAKE = 'snowflake'
+    DB_AUTO_INCREMENT = 'db_auto_increment'
+
+
+class Model:
+    """
+    Create a class extends Model:
+
+    class Person(Model):
+        __key__ = 'id'
+        __table__ = 'person'
+        __update_by__ = 'update_by'
+        __update_time__ = 'update_time'
+        __del_flag__ = 'del_flag'
+        __key_seq__ = 'person_id_seq'
+
+        def __init__(self, id: int = None, name: str = None, age: int = None, update_by: int = None, update_time: datetime = None, del_flag: int = None):
+            self.id = id
+
+            self.update_by = update_by
+            self.update_time = update_time
+            self.del_flag = del_flag
+            self.name = name
+            self.age = age
+
+    then you can use like follow:
+        orm.init(person='xxx', password='xxx', database='xxx', host='xxx', ...)  # or db.init(...) init db first,
+        person = Person(name='张三', age=55)
+        effect_rowcount = person.persist()
+        id = person.inst_save()
+    """
+
+    def __str__(self):
+        return str({k: v for k, v in self.__dict__.items() if not k.startswith("__")})
+
+    def __getattr__(self, name):
+        if KEY == name:
+            return self._get_key()
+        elif TABLE == name:
+            return self.get_table()
+        elif UPDATE_BY == name:
+            return self._get_update_by_field()
+        elif UPDATE_TIME == name:
+            return self._get_update_time_field()
+        else:
+            return None
+
+    def persist(self, ignored_none=True, *fields):
+        """
+        person = Person(name='张三', age=55)
+        effect_rowcount = person.persist()
+        :return: effect rowcount
+        """
+        log_support.orm_inst_log('persist', self.__class__.__name__)
+        kv = self._get_kv(ignored_none, None, *fields)
+        return self.insert(**kv)
+
+    def inst_save(self, ignored_none=True, *fields):
+        """
+        person = Person(name='张三', age=55)
+        id = person.save()
+        :return: Primary key
+        """
+        log_support.orm_inst_log('inst_save', self.__class__.__name__)
+        key = self._get_key()
+        kv = self._get_kv(ignored_none, None, *fields)
+        _id = self.save(**kv)
+        if key not in kv:
+            self.__dict__.update({key: _id})
+        return _id
+
+    def update(self, ignored_none=True, *fields):
+        """
+        person = Person(id=1, name='李四', age=66)
+        rowcount = person.update()
+        :return: Effect rowcount
+        """
+        log_support.orm_inst_log('update', self.__class__.__name__)
+        key, table = self._get_key_and_table()
+        kv = self._get_kv(ignored_none, key, *fields)
+        _id = kv[key]
+        assert _id is not None, 'Primary key must not be None.'
+        update_kv = {k: v for k, v in kv.items() if k != key}
+        if update_kv:
+            return self.update_by_id(_id, **update_kv)
+        else:
+            log_support.logger.warning("Exec func 'sqlbatis.orm.Model.%s' not set fields, Class: '%s:'\n\t   %s" % ('update', self.__class__.__name__, self))
+            return 0
+
+    def load(self, *fields):
+        """
+        Return new object from database and update itself.
+        :param fields: Default select all fields if not set. like: ('id', 'name', 'age')
+        person = Person(id=1)
+        person2 = person.load()
+        """
+        log_support.logger.debug("Exec func 'sqlbatis.orm.Model.%s', Class: '%s', fields: %s" % ('load', self.__class__.__name__, fields))
+        key = self._get_key()
+        kv = self.__dict__
+        _id = kv.get(key)
+        assert _id is not None, 'Primary key must not be None.'
+        if not fields:
+            fields, _ = zip(*kv.items())
+        result = self.query_by_id(_id, *fields)
+        if result:
+            self.__dict__.update(result)
+            return self
+        else:
+            raise NotFoundError("Load not found from db, Class: '%s', %s=%d." % (self.__class__.__name__, key, _id))
+
+    def logical_delete(self):
+        """
+        Logic delete only update the del flag
+        person = Person(id=1)
+        rowcount = person.logical_delete()
+        """
+        log_support.orm_inst_log('logical_delete', self.__class__.__name__)
+        key = self._get_key()
+        kv = self.__dict__
+        _id = kv.get(key)
+        assert _id is not None, 'Primary key must not be None.'
+        update_by = kv.get(self._get_update_by_field())
+        return self.logical_delete_by_id(_id, update_by)
+
+    def logical_undelete(self):
+        """
+        Logic un delete only update the del flag
+        person = Person(id=1)
+        rowcount = person.logical_undelete()
+        """
+        log_support.orm_inst_log('logical_undelete', self.__class__.__name__)
+        key = self._get_key()
+        kv = self.__dict__
+        _id = kv.get(key)
+        assert _id is not None, 'Primary key must not be None.'
+        update_by = kv.get(self._get_update_by_field())
+        return self.logical_undelete_by_id(_id, update_by)
+
+    def remove(self):
+        """
+        Physical delete
+        person = Person(id=1)
+        rowcount = person.remove()
+        """
+        log_support.orm_inst_log('remove', self.__class__.__name__)
+        key = self._get_key()
+        _id = self.__dict__.get(key)
+        assert _id is not None, 'Primary key must not be None.'
+        return self.delete_by_id(_id)
+
+    # ----------------------------------------------------------Class method------------------------------------------------------------------
+    @classmethod
+    def insert(cls, **kwargs):
+        """
+        rowcount = Person.insert(name='张三', age=20)
+        return: Effect rowcount
+        """
+        log_support.orm_insert_log('insert', cls.__name__, **kwargs)
+        key, table = cls._get_key_and_table()
+        key_strategy = cls._get_key_strategy()
+        if key_strategy == KeyStrategy.SNOWFLAKE and key not in kwargs:
+            kwargs[key] = get_snowflake_id()
+        return db.insert(table, **kwargs)
+
+    @classmethod
+    def save(cls, **kwargs):
+        """
+        id = Person.save(name='张三', age=20)
+        :return: Primary key
+        """
+        log_support.orm_insert_log('save', cls.__name__, **kwargs)
+        key, table = cls._get_key_and_table()
+        if key in kwargs:
+            db.insert(table, **kwargs)
+            return kwargs[key]
+
+        key_strategy = cls._get_key_strategy()
+        if key_strategy == KeyStrategy.SNOWFLAKE:
+            kwargs[key] = get_snowflake_id()
+            db.insert(table, **kwargs)
+            return kwargs[key]
+        else:
+            select_key = cls._get_select_key()
+            if not select_key:
+                keq_seq = cls._get_key_seq()
+                try:
+                    select_key = Dialect.get_select_key(keq_seq=keq_seq, table=table, key=key)
+                except NotImplementedError:
+                    raise DBError("Expect 'select_key'. you can set it in model class with '__select_key__'. "
+                                  "You can also set primary key sequence with '__key_seq__' for PostgreSQL.'")
+            return db.save_select_key(select_key, table, **kwargs)
+
+    @classmethod
+    def create(cls, **kwargs):
+        """
+        person = Person.create(name='张三', age=20)
+        :return: Instance object
+        """
+        log_support.orm_insert_log('create', cls.__name__, **kwargs)
+        key = cls._get_key()
+        kwargs[key] = cls.save(**kwargs)
+        return cls.to_obj(**kwargs)
+
+    @classmethod
+    def update_by_id(cls, _id: Union[int, str], **kwargs):
+        """
+        rowcount = Person.update_by_id(id=1, name='王五')
+        return: Effect rowcount
+        """
+        log_support.logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', id: %d, kwargs: %s" % ('update_by_id', cls.__name__, _id, kwargs))
+        assert kwargs, 'Must set update kv'
+        key, table_name = cls._get_key_and_table()
+        where_kwargs = {key: _id}
+        kwargs = cls._update_time(**kwargs)
+        db.table(table_name).where(**where_kwargs).update(**kwargs)
+
+    @classmethod
+    def logical_delete_by_id(cls, _id: Union[int, str], update_by: Union[int, str] = None):
+        """
+        Logic delete only update the del flag
+        rowcount = Person.delete_by_id(id=1, update_by=100)
+        return: Effect rowcount
+        """
+        log_support.orm_delete_by_id_log('logical_delete_by_id', cls.__name__, _id, update_by)
+        return cls._logical_delete_by_id_op(_id, update_by, DelFlag.DELETED)
+
+    @classmethod
+    def logical_undelete_by_id(cls, _id: Union[int, str], update_by: Union[int, str] = None):
+        """
+        Logic delete only update the del flag
+        rowcount = Person.logical_undelete_by_id(id=1, update_by=100)
+        return: Effect rowcount
+        """
+        log_support.orm_delete_by_id_log('logical_undelete_by_id', cls.__name__, _id, update_by)
+        return cls._logical_delete_by_id_op(_id, update_by, DelFlag.UN_DELETE)
+
+    @classmethod
+    def logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128):
+        """
+        Logic delete only update the del flag
+        rowcount = Person.logical_delete_by_ids(id=[1,2], update_by=100)
+        return: Effect rowcount
+        """
+        log_support.orm_logical_delete_by_ids_log('logical_delete_by_ids', cls.__name__, ids, update_by, batch_size)
+        return cls._logical_delete_by_ids_op(ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.DELETED)
+
+    @classmethod
+    def logical_undelete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128):
+        """
+        Logic delete only update the del flag
+        rowcount = Person.logical_undelete_by_ids(id=[1,2], update_by=100)
+        return: Effect rowcount
+        """
+        log_support.orm_logical_delete_by_ids_log('logical_undelete_by_ids', cls.__name__, ids, update_by, batch_size)
+        return cls._logical_delete_by_ids_op(ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.UN_DELETE)
+
+    @classmethod
+    def delete(cls, **kwargs):
+        """
+        Physical delete
+        rowcount = Person.delete(name='张三', age=55)
+        return: Effect rowcount
+        """
+        log_support.orm_count_log(sys._getframe().f_code.co_name, cls.__name__, **kwargs)
+        table = cls.get_table()
+        return db.table(table).where(**kwargs).delete()
+
+    @classmethod
+    def delete_by_id(cls, _id: Union[int, str]):
+        """
+        Physical delete
+        rowcount = Person.delete_by_id(id=1)
+        return: Effect rowcount
+        """
+        log_support.logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', id: %d" % ('delete_by_id', cls.__name__, _id))
+        key, table = cls._get_key_and_table()
+        where_kwargs = {key: _id}
+        return db.table(table).where(**where_kwargs).delete()
+
+    @classmethod
+    def delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], batch_size=128):
+        """
+        Batch physical delete, they will be executed in batches if there are too many
+        rowcount = Person.delete_by_ids(id=[1,2])
+        return: Effect rowcount
+        """
+        log_support.logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', ids: %s, batch_size: %s" % ('delete_by_ids', cls.__name__, ids, batch_size))
+        ids_size = len(ids)
+        assert ids_size > 0, 'ids must not be empty.'
+        if ids_size == 1:
+            return cls.delete_by_id(ids[0])
+        elif ids_size <= batch_size:
+            return cls.do_delete_by_ids(ids)
+        else:
+            slices = orm_support.split_ids(ids, batch_size)
+            with transaction():
+                results = list(map(cls.do_delete_by_ids, slices))
+            return sum(results)
+
+    @classmethod
+    def do_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]]):
+        """
+        Batch physical delete, please use delete_by_ids if there are too many
+        rowcount = Person.do_delete_by_ids(id=[1,2])
+        return: Effect rowcount
+        """
+        key, table = cls._get_key_and_table()
+        where_kwargs = {'{}__in'.format(key): ids}
+        return db.table(table).where(**where_kwargs).delete()
+
+    @classmethod
+    def batch_insert(cls, *args):
+        """
+        Batch insert
+        rowcount = Person.batch_insert([{'name': '张三', 'age': 55},{'name': '李四', 'age': 66}])
+        :param args: All number must have same key.
+        :return: Effect rowcount
+        """
+        log_support.logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', args: %s" % ('batch_insert', cls.__name__, args))
+        assert len(args) > 0, 'args must not be empty.'
+        key, table = cls._get_key_and_table()
+        key_strategy = cls._get_key_strategy()
+        if key_strategy == KeyStrategy.SNOWFLAKE:
+            for arg in args:
+                if key not in arg:
+                    arg[key] = get_snowflake_id()
+
+        return db.batch_insert(table, *args)
+
+    # ------------------------------------------------Class query method------------------------------------------------
+    @classmethod
+    def count(cls, **kwargs):
+        """
+        count = Person.count(name='张三', age=55)
+        """
+        log_support.orm_count_log('count', cls.__name__, **kwargs)
+        table = cls.get_table()
+        return db.table(table).where(**kwargs).count()
+
+    @classmethod
+    def exists(cls, **kwargs):
+        log_support.orm_count_log('exists', cls.__name__, **kwargs)
+        table = cls.get_table()
+        return db.table(table).where(**kwargs).exists()
+
+    @classmethod
+    def exists_by_id(cls, _id: Union[int, str]):
+        key = cls._get_key()
+        kwargs = {key: _id}
+        return cls.exists(**kwargs)
+
+    @classmethod
+    def find(cls, *fields, **kwargs):
+        """
+        Return list(object) or empty list if no result.
+        persons = Person.find('id', 'name', 'age', name='张三', age=55)
+        :param fields: Default select all fields if not set
+        """
+        log_support.orm_find_log('find', cls.__name__, *fields, **kwargs)
+        return [cls.to_obj(**d) for d in cls.query(*fields, **kwargs)]
+
+    @classmethod
+    def find_one(cls, *fields, **kwargs):
+        """
+        Return unique result(object) or None if no result.
+        person = Person.find_one('id', 'name', 'age', name='张三', age=55)
+        :param fields: Default select all fields if not set
+        """
+        log_support.orm_find_log('find_one', cls.__name__, *fields, **kwargs)
+        result = cls.query_one(*fields, **kwargs)
+        return cls.to_obj(**result) if result else None
+
+    @classmethod
+    def find_by_id(cls, _id: Union[int, str], *fields):
+        """
+        Return one class object or None if no result.
+        person = Person.find_by_id(1, 'id', 'name', 'age')
+        :param _id: key
+        :param fields: Default select all fields if not set
+        """
+        log_support.orm_find_by_id_log('find_by_id', cls.__name__, _id, *fields)
+        result = cls.query_by_id(_id, *fields)
+        return cls.to_obj(**result) if result else None
+
+    @classmethod
+    def find_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
+        """
+        Return list(class object) or empty list if no result.
+        persons = Person.find_by_ids([1,2], 'id', 'name', 'age')
+        :param ids: List of key
+        :param fields: Default select all fields if not set
+        """
+        log_support.orm_find_by_ids_log('find_by_ids', cls.__name__, ids, *fields)
+        return [cls.to_obj(**d) for d in cls.query_by_ids(ids, *fields)]
+
+    @classmethod
+    def query(cls, *fields, **kwargs):
+        """
+        Return list(dict) or empty list if no result.
+        persons = Person.query('id', 'name', 'age', name='张三', age=55)
+        :param fields: Default select all fields if not set
+        """
+        log_support.orm_find_log('query', cls.__name__, *fields, **kwargs)
+        table = cls.get_table()
+        return db.table(table).columns(*fields).where(**kwargs).query()
+
+    @classmethod
+    def query_one(cls, *fields, **kwargs):
+        """
+        Return unique result(dict) or None if no result.
+        persons = Person.query_one('id', 'name', 'age', name='张三', age=55)
+        :param fields: Default select all fields if not set
+        """
+        log_support.orm_find_log('query_one', cls.__name__, *fields, **kwargs)
+        table = cls.get_table()
+        return db.table(table).columns(*fields).where(**kwargs).query_one()
+
+    @classmethod
+    def query_by_id(cls, _id: Union[int, str], *fields):
+        """
+        Return one row(dict) or None if no result.
+        person = Person.query_by_id(1, 'id', 'name', 'age')
+        :param _id: key
+        :param fields: Default select all fields if not set
+        """
+        log_support.orm_find_by_id_log('query_by_id', cls.__name__, _id, *fields)
+        key, table = cls._get_key_and_table()
+        kwargs = {key: _id}
+        return db.table(table).columns(*fields).where(**kwargs).query_one()
+
+    @classmethod
+    def query_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
+        """
+        Return list(dict) or empty list if no result.
+        persons = Person.query_by_ids([1,2], 'id', 'name', 'age')
+        :param ids: List of key
+        :param fields: Default select all fields if not set
+        """
+        log_support.orm_find_by_ids_log('query_by_ids', cls.__name__, ids, *fields)
+        assert len(ids) > 0, 'ids must not be empty.'
+
+        key, table = cls._get_key_and_table()
+        kwargs = {'{}__in'.format(key): ids}
+        return db.table(table).columns(*fields).where(**kwargs).query()
+
+    @classmethod
+    def select(cls, *fields, **kwargs):
+        """
+        Return list(dict) or empty list if no result.
+        rows = Person.select('id', 'name', 'age', name='张三', age=55)
+        :param fields: Default select all fields if not set
+        """
+        log_support.orm_find_log('select', cls.__name__, *fields, **kwargs)
+        table = cls.get_table()
+        return db.table(table).columns(*fields).where(**kwargs).select()
+
+    @classmethod
+    def select_one(cls, *fields, **kwargs):
+        """
+        Return unique result(tuple) or None if no result.
+        row = Person.select_one('id', 'name', 'age', name='张三', age=55)
+        :param fields: Default select all fields if not set
+        """
+        log_support.orm_find_log('select_one', cls.__name__, *fields, **kwargs)
+        table = cls.get_table()
+        return db.table(table).columns(*fields).where(**kwargs).select_one()
+
+    @classmethod
+    def select_by_id(cls, _id: Union[int, str], *fields):
+        """
+        Return one row(dict) or None if no result.
+        row = Person.select_by_id(1, 'id', 'name', 'age')
+        :param _id: key
+        :param fields: Default select all fields if not set
+        """
+        log_support.orm_find_by_id_log('select_by_id', cls.__name__, _id, *fields)
+        key, table = cls._get_key_and_table()
+        kwargs = {key: _id}
+        return db.table(table).columns(*fields).where(**kwargs).select_one()
+
+    @classmethod
+    def select_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
+        """
+        Return list(dict) or empty list if no result.
+        rows = Person.select_by_ids([1,2], 'id', 'name', 'age')
+        :param ids: List of key
+        :param fields: Default select all fields if not set
+        """
+        log_support.orm_find_by_ids_log('select_by_ids', cls.__name__, ids, *fields)
+        assert len(ids) > 0, 'ids must not be empty.'
+
+        key, table = cls._get_key_and_table()
+        kwargs = {'{}__in'.format(key): ids}
+        return db.table(table).columns(*fields).where(**kwargs).select()
+
+    @classmethod
+    def find_page(cls, page_num=1, page_size=10, *fields, **kwargs):
+        """
+        Return list(object) or empty list if no result.
+        persons = Person.find_page(1, 10, 'name', 'age', name='张三', age=55)
+        :param page_num: page number
+        :param page_size: page size
+        :param fields: Default select all fields if not set
+        """
+        log_support.orm_page_log('find_page', page_num, page_size, cls.__name__, *fields, **kwargs)
+        result = cls.query_page(page_num, page_size, *fields, **kwargs)
+        return [cls.to_obj(**d) for d in result]
+
+    @classmethod
+    def query_page(cls, page_num=1, page_size=10, *fields, **kwargs):
+        """
+        Return list(dict) or empty list if no result.
+        persons = Person.query_page(1, 10, 'id', 'name', 'age', name='张三', age=55)
+        :param page_num: page number
+        :param page_size: page size
+        :param fields: Default select all fields if not set
+        """
+        log_support.orm_page_log('query_page', page_num, page_size, cls.__name__, *fields, **kwargs)
+        table = cls.get_table()
+        return db.table(table).columns(*fields).where(**kwargs).page(page_num, page_size).query()
+
+    @classmethod
+    def select_page(cls, page_num=1, page_size=10, *fields, **kwargs):
+        """
+        Return list(dict) or empty list if no result.
+        rows = Person.select_page('id', 'name', 'age', name='张三', age=55)
+        :param page_num: page number
+        :param page_size: page size
+        :param fields: Default select all fields if not set
+        """
+        log_support.orm_page_log('select_page', page_num, page_size, cls.__name__, *fields, **kwargs)
+        table = cls.get_table()
+        return db.table(table).columns(*fields).where(**kwargs).page(page_num, page_size).select()
+
+    @classmethod
+    def fields(cls, *fields) -> orm_support.FieldExec:
+        return orm_support.FieldExec(cls, *fields)
+
+    @classmethod
+    def where(cls, **kwargs) -> orm_support.WhereExec:
+        return orm_support.WhereExec(cls, **kwargs)
+
+    @classmethod
+    def page(cls, page_num=1, page_size=10) -> orm_support.PageExec:
+        return orm_support.PageExec(cls, page_num, page_size)
+
+    @classmethod
+    def to_obj(cls, **kwargs):
+        model = cls.__new__(cls)
+        model.__dict__.update(**kwargs)
+        return model
+
+    def _get_kv(self, ignored_none: bool, key: None, *fields):
+        if fields:
+            if key:
+                fields = (key, *fields)
+            if ignored_none:
+                return {k: v for k, v in self.__dict__.items() if v is not None and k in fields}
+            return {k: v for k, v in self.__dict__.items() if k in fields}
+
+        if ignored_none:
+            return {k: v for k, v in self.__dict__.items() if v is not None}
+        return {k: v for k, v in self.__dict__.items()}
+
+    # ------------------------------------------------Private class method----------------------------------------------
+    @classmethod
+    def _logical_delete_by_id_op(cls, _id: Union[int, str], update_by: Union[int, str] = None, del_status=DelFlag.DELETED):
+        key, table = cls._get_key_and_table()
+        del_flag_field = cls._get_del_flag_field()
+        update_by_field = cls._get_update_by_field()
+
+        where = '%s = ?' % key
+        if update_by is not None and update_by_field is not None:
+            sql, update_time_arg = cls._update_sql(where, del_flag_field, update_by_field)
+            if update_time_arg:
+                return db.do_execute(sql, del_status.value, update_by, update_time_arg, _id)
+            return db.do_execute(sql, del_status.value, update_by, _id)
+        else:
+            sql, update_time_arg = cls._update_sql(where, del_flag_field)
+            if update_time_arg:
+                return db.do_execute(sql, del_status.value, update_time_arg, _id)
+            return db.do_execute(sql, del_status.value, _id)
+
+    @classmethod
+    def _logical_delete_by_ids_op(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128,
+            del_status=DelFlag.DELETED):
+        ids_size = len(ids)
+        assert ids_size > 0, 'ids must not be empty.'
+
+        if ids_size == 1:
+            return cls._logical_delete_by_id_op(ids[0], update_by, del_status)
+        elif ids_size <= batch_size:
+            return cls._do_logical_delete_by_ids(ids, update_by, del_status)
+        else:
+            slices = orm_support.split_ids(ids, batch_size)
+            with transaction():
+                results = [cls._do_logical_delete_by_ids(ids, update_by, del_status) for ids in slices]
+            return sum(results)
+
+    @classmethod
+    def _do_logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, del_status=DelFlag.DELETED):
+        key = cls._get_key()
+        del_flag_field = cls._get_del_flag_field()
+        update_by_field = cls._get_update_by_field()
+
+        where = '%s in (%s)' % (key, ','.join(['?' for _ in range(len(ids))]))
+        if update_by is not None and update_by_field is not None:
+            sql, update_time_arg = cls._update_sql(where, del_flag_field, update_by_field)
+            if update_time_arg:
+                return db.do_execute(sql, del_status.value, update_by, update_time_arg, *ids)
+            return db.do_execute(sql, del_status.value, update_by, *ids)
+        else:
+            sql, update_time_arg = cls._update_sql(where, del_flag_field)
+            if update_time_arg:
+                return db.do_execute(sql, del_status.value, update_time_arg, *ids)
+            return db.do_execute(sql, del_status.value, *ids)
+
+    @classmethod
+    def _get_key(cls):
+        if hasattr(cls, KEY):
+            return cls.__key__
+        log_support.logger.warning("%s not set attribute '%s'" % (cls.__name__, KEY))
+        return DEFAULT_KEY_FIELD
+
+    @classmethod
+    def _get_select_key(cls):
+        return cls.__select_key__ if hasattr(cls, SELECT_KEY) else None
+
+    @classmethod
+    def _get_key_seq(cls):
+        return cls.__key_seq__ if hasattr(cls, KEY_SEQ) else None
+
+    @classmethod
+    def get_table(cls):
+        if hasattr(cls, TABLE):
+            return cls.__table__
+        log_support.logger.warning("%s not set attribute '%s'" % (cls.__name__, TABLE))
+        return orm_support.get_table_name(cls.__name__)
+
+    @classmethod
+    def _get_key_and_table(cls):
+        return cls._get_key(), cls.get_table()
+
+    @classmethod
+    def _get_key_strategy(cls):
+        if hasattr(cls, KEY_STRATEGY):
+            return cls.__key_strategy__
+        return None
+
+    @classmethod
+    def _get_update_by_field(cls):
+        if hasattr(cls, UPDATE_BY):
+            return cls.__update_by__
+        return None
+
+    @classmethod
+    def _get_update_time_field(cls):
+        if hasattr(cls, UPDATE_TIME):
+            return cls.__update_time__
+        return None
+
+    @classmethod
+    def _get_del_flag_field(cls):
+        assert hasattr(cls, DEL_FLAG), "%s not set attribute '%s'" % (cls.__name__, DEL_FLAG)
+        return cls.__del_flag__
+
+    @classmethod
+    def _update_time(cls, **kwargs):
+        update_time_field = cls._get_update_time_field()
+        if update_time_field is not None and update_time_field not in kwargs:
+            kwargs[update_time_field] = datetime.now()
+        return kwargs
+
+    @classmethod
+    def _update_sql(cls, where, *update_fields):
+        update_time_arg = None
+        table = cls.get_table()
+        table = Dialect.get_dialect_str(table)
+        update_time_field = cls._get_update_time_field()
+        if update_time_field is not None and update_time_field not in update_fields:
+            update_fields = [*update_fields, update_time_field]
+            update_time_arg = datetime.now()
+
+        update_fields = ', '.join(['{} = ?'.format(Dialect.get_dialect_str(col)) for col in update_fields])
+        return 'UPDATE {} SET {} WHERE {}'.format(table, update_fields, where), update_time_arg
+
+    @classmethod
+    def _where_sql(cls, where: str):
+        low_where = where.strip().lower()
+        if low_where.startswith('where'):
+            table = cls.get_table()
+            return orm_support.get_table_select_sql(table, where, NO_LIMIT)
+        elif low_where.startswith('select'):
+            return where
+        raise DBError("The where parameter must be a complete SQL statement or conditions start with 'where'")
```

### Comparing `sqlx-orm-0.0.6/orm/orm_support.py` & `sqlx-orm-0.0.7/orm/orm_support.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,394 +1,394 @@
-from sqlexec.sql_support import get_table_select_sql
-from typing import Sequence, Union, List, Tuple
-from sqlexec.table_exec import get_condition_arg, get_where_arg_limit
-
-
-class FieldWherePageExec:
-    def __init__(self, field_where_exec, page_num, page_size):
-        self.field_where_exec = field_where_exec
-        self.page_num = page_num
-        self.page_size = page_size
-
-    def find(self):
-        return self.field_where_exec.find_page(self.page_num, self.page_size)
-
-    def query(self):
-        return self.field_where_exec.query_page(self.page_num, self.page_size)
-
-    def select(self):
-        return self.field_where_exec.select_page(self.page_num, self.page_size)
-
-
-class FieldWhereExec:
-    def __init__(self, field_exec, **kwargs):
-        self.field_exec = field_exec
-        self.kwargs = kwargs
-
-    def find(self):
-        """
-        Return list(object) or empty list if no result.
-        persons = Person.fields('id', 'name', 'age').where(name='张三', age=55).find()
-        """
-        return self.field_exec.find(**self.kwargs)
-
-    def find_one(self):
-        """
-        Return unique result(object) or None if no result.
-        person = Person.fields('id', 'name', 'age').where(name='张三', age=55).find_one()
-        """
-        return self.field_exec.find_one(**self.kwargs)
-
-    def query(self):
-        """
-        Return list(dict) or empty list if no result.
-        persons = Person.fields('id', 'name', 'age').where(name='张三', age=55).query()
-        """
-        return self.field_exec.query(**self.kwargs)
-
-    def query_one(self):
-        """
-        Return unique result(dict) or None if no result.
-        persons = Person.fields('id', 'name', 'age').where(name='张三', age=55).query_one()
-        """
-        return self.field_exec.query_one(**self.kwargs)
-
-    def select(self):
-        """
-        Return list(dict) or empty list if no result.
-        rows = Person.fields('id', 'name', 'age').where(name='张三', age=55).select()
-        """
-        return self.field_exec.select(**self.kwargs)
-
-    def select_one(self):
-        """
-        Return unique result(tuple) or None if no result.
-        row = Person.fields('id', 'name', 'age').where(name='张三', age=55).select_one()
-        """
-        return self.field_exec.select_one(**self.kwargs)
-
-    def find_page(self, page_num=1, page_size=10):
-        """
-        Return list(object) or empty list if no result.
-        persons = Person.fields('id', 'name', 'age').where(name='张三', age=55).find_page(1, 10)
-        :param page_num: page number
-        :param page_size: page size
-        """
-        return self.field_exec.find_page(page_num, page_size, **self.kwargs)
-
-    def query_page(self, page_num=1, page_size=10):
-        """
-        Return list(dict) or empty list if no result.
-        persons = Person.fields('id', 'name', 'age').where(name='张三', age=55).query_page(1, 10)
-        :param page_num: page number
-        :param page_size: page size
-        """
-        return self.field_exec.query_page(page_num, page_size, **self.kwargs)
-
-    def select_page(self, page_num=1, page_size=10):
-        """
-        Return list(dict) or empty list if no result.
-        rows = Person.fields('id', 'name', 'age').where(name='张三', age=55).select_page(1, 10)
-        :param page_num: page number
-        :param page_size: page size
-        """
-        return self.field_exec.select_page(page_num, page_size, **self.kwargs)
-
-    def page(self, page_num=1, page_size=10) -> FieldWherePageExec:
-        return FieldWherePageExec(self, page_num, page_size)
-
-
-class FieldPageExec:
-    def __init__(self, field_exec, page_num=1, page_size=10):
-        self.field_exec = field_exec
-        self.page_num = page_num
-        self.page_size = page_size
-
-    def find(self, **kwargs):
-        return self.field_exec.find_page(self.page_num, self.page_size, **kwargs)
-
-    def query(self, **kwargs):
-        return self.field_exec.query_page(self.page_num, self.page_size, **kwargs)
-
-    def select(self, **kwargs):
-        return self.field_exec.select_page(self.page_num, self.page_size, **kwargs)
-
-    def where(self, **kwargs) -> FieldWherePageExec:
-        return FieldWherePageExec(FieldWhereExec(self.field_exec, **kwargs), self.page_num, self.page_size)
-
-
-class FieldExec:
-    def __init__(self, cls, *fields):
-        self.cls = cls
-        self.fields = fields
-
-    def find(self, **kwargs):
-        """
-        Return list(object) or empty list if no result.
-        persons = Person.fields('id', 'name', 'age').find(name='张三', age=55)
-        """
-        return self.cls.find(*self.fields, **kwargs)
-
-    def find_one(self, **kwargs):
-        """
-        Return unique result(object) or None if no result.
-        person = Person.fields('id', 'name', 'age').find_one(name='张三', age=55)
-        """
-        return self.cls.find_one(*self.fields, **kwargs)
-
-    def find_by_id(self, _id: Union[int, str]):
-        """
-        Return one class object or None if no result.
-        person = Person.fields('id', 'name', 'age').find_by_id(1)
-        :param _id: key
-        """
-        return self.cls.find_by_id(_id, *self.fields)
-
-    def find_by_ids(self, *ids):
-        """
-        Return list(class object) or empty list if no result.
-        persons = Person.fields('id', 'name', 'age').find_by_ids(1,2)
-        :param ids: List of key
-        """
-        return self.cls.find_by_ids(ids, *self.fields)
-
-    def query(self, **kwargs):
-        """
-        Return list(dict) or empty list if no result.
-        persons = Person.fields('id', 'name', 'age').query(name='张三', age=55)
-        """
-        return self.cls.query(*self.fields, **kwargs)
-
-    def query_one(self, **kwargs):
-        """
-        Return unique result(dict) or None if no result.
-        persons = Person.fields('id', 'name', 'age').query_one(name='张三', age=55)
-        """
-        return self.cls.query_one(*self.fields, **kwargs)
-
-    def query_by_id(self, _id: Union[int, str]):
-        """
-        Return one row(dict) or None if no result.
-        person = Person.fields('id', 'name', 'age').query_by_id(1)
-        :param _id: key
-        """
-        return self.cls.query_by_id(_id, *self.fields)
-
-    def query_by_ids(self, *ids):
-        """
-        Return list(dict) or empty list if no result.
-        persons = Person.fields('id', 'name', 'age').query_by_ids(1,2)
-        :param ids: List of key
-        """
-        return self.cls.query_by_ids(ids, *self.fields)
-
-    def select(self, **kwargs):
-        """
-        Return list(dict) or empty list if no result.
-        rows = Person.fields('id', 'name', 'age').select(name='张三', age=55)
-        """
-        return self.cls.select(*self.fields, **kwargs)
-
-    def select_one(self, **kwargs):
-        """
-        Return unique result(tuple) or None if no result.
-        row = Person.fields('id', 'name', 'age').select_one(name='张三', age=55)
-        """
-        return self.cls.select_one(*self.fields, **kwargs)
-
-    def select_by_id(self, _id: Union[int, str]):
-        """
-        Return one row(dict) or None if no result.
-        row = Person.fields('id', 'name', 'age').select_by_id(1)
-        :param _id: key
-        """
-        return self.cls.select_by_id(_id, *self.fields)
-
-    def select_by_ids(self, *ids):
-        """
-        Return list(dict) or empty list if no result.
-        rows = Person.select_by_ids([1,2], 'id', 'name', 'age')
-        :param ids: List of key
-        :param fields: Default select all fields if not set
-        """
-        return self.cls.select_by_ids(ids, *self.fields)
-
-    def find_page(self, page_num=1, page_size=10, **kwargs):
-        """
-        Return list(object) or empty list if no result.
-        persons = Person.fields('id', 'name', 'age').find_page(1, 10, name='张三', age=55)
-        :param page_num: page number
-        :param page_size: page size
-        """
-        return self.cls.find_page(page_num, page_size, *self.fields, **kwargs)
-
-    def query_page(self, page_num=1, page_size=10, **kwargs):
-        """
-        Return list(dict) or empty list if no result.
-        persons = Person.fields('id', 'name', 'age').query_page(1, 10, name='张三', age=55)
-        :param page_num: page number
-        :param page_size: page size
-        """
-        return self.cls.query_page(page_num, page_size, *self.fields, **kwargs)
-
-    def select_page(self, page_num=1, page_size=10, **kwargs):
-        """
-        Return list(dict) or empty list if no result.
-        rows = Person.fields('id', 'name', 'age').select_page(1, 10, name='张三', age=55)
-        :param page_num: page number
-        :param page_size: page size
-        """
-        return self.cls.select_page(page_num, page_size, *self.fields, **kwargs)
-
-    def where(self, **kwargs) -> FieldWhereExec:
-        return FieldWhereExec(self, **kwargs)
-
-    def page(self, page_num=1, page_size=10) -> FieldPageExec:
-        return FieldPageExec(self, page_num, page_size)
-
-
-class WherePageExec:
-    def __init__(self, where_exec, page_num=1, page_size=10):
-        self.where_exec = where_exec
-        self.page_num = page_num
-        self.page_size = page_size
-
-    def select(self, *fields):
-        """
-        Return list(dict) or empty list if no result.
-        rows = Person.where(name='张三', age=55).page(1, 10).select()
-        """
-        return self.where_exec.select_page(self.page_num, self.page_size, *fields)
-
-    def query(self, *fields):
-        """
-        Return list(dict) or empty list if no result.
-        rows = Person.where(name='张三', age=55).page(1, 10).query()
-        """
-        return self.where_exec.query_page(self.page_num, self.page_size, *fields)
-
-    def find(self, *fields):
-        """
-        Return list(dict) or empty list if no result.
-        rows = Person.where(name='张三', age=55).page(1, 10).find()
-        """
-        return self.where_exec.find_page(self.page_num, self.page_size, *fields)
-
-    def fields(self, *fields) -> FieldWherePageExec:
-        return FieldWherePageExec(FieldWhereExec(FieldExec(self.where_exec.cls, *fields), **self.where_exec.kwargs), self.page_num, self.page_size)
-
-
-class WhereExec:
-    def __init__(self, cls, **kwargs):
-        self.cls = cls
-        self.kwargs = kwargs
-
-    def delete(self):
-        """
-        Physical delete
-        rowcount = Person.where(name='张三', age=55).delete()
-        return: Effect rowcount
-        """
-        return self.cls.delete(**self.kwargs)
-
-    def count(self):
-        """
-        count = Person.where(name='张三', age=55).count()
-        """
-        return self.cls.count(**self.kwargs)
-
-    def exists(self):
-        """
-        flag = Person.where(name='张三', age=55).exists()
-        """
-        return self.cls.exists(**self.kwargs)
-
-    def select(self, *fields):
-        """
-        Return list(dict) or empty list if no result.
-        rows = Person.where(name='张三', age=55).select()
-        """
-        return self.cls.select(*fields, **self.kwargs)
-
-    def query(self, *fields):
-        """
-        Return list(dict) or empty list if no result.
-        rows = Person.where(name='张三', age=55).query()
-        """
-        return self.cls.query(*fields, **self.kwargs)
-
-    def find(self, *fields):
-        """
-        Return list(dict) or empty list if no result.
-        rows = Person.where(name='张三', age=55).find()
-        """
-        return self.cls.find(*fields, **self.kwargs)
-
-    def select_page(self, page_num=1, page_size=10, *fields):
-        """
-        Return list(dict) or empty list if no result.
-        rows = Person.where(name='张三', age=55).select_page()
-        """
-        return self.cls.select_page(page_num, page_size, *fields, **self.kwargs)
-
-    def query_page(self, page_num=1, page_size=10, *fields):
-        """
-        Return list(dict) or empty list if no result.
-        rows = Person.where(name='张三', age=55).query_page()
-        """
-        return self.cls.query_page(page_num, page_size, *fields, **self.kwargs)
-
-    def find_page(self, page_num=1, page_size=10, *fields):
-        """
-        Return list(dict) or empty list if no result.
-        rows = Person.where(name='张三', age=55).find_page()
-        """
-        return self.cls.find_page(page_num, page_size, *fields, **self.kwargs)
-
-    def fields(self, *fields) -> FieldWhereExec:
-        return FieldWhereExec(FieldExec(self.cls, *fields), **self.kwargs)
-
-    def page(self, page_num=1, page_size=10) -> WherePageExec:
-        return WherePageExec(self, page_num, page_size)
-
-
-class PageExec:
-    
-    def __init__(self, cls, page_num=1, page_size=10):
-        self.cls = cls
-        self.page_num = page_num
-        self.page_size = page_size
-
-    def select(self, *fields, **kwargs):
-        """
-        Person.page(1, 10).select('id', 'name', 'age', name='张三', age=55)
-        """
-        return self.cls.select_page(self.page_num, self.page_size, *fields, **kwargs)
-
-    def query(self, *fields, **kwargs):
-        """
-        Person.page(1, 10).query('id', 'name', 'age', name='张三', age=55)
-        """
-        return self.cls.query_page(self.page_num, self.page_size, *fields, **kwargs)
-
-    def find(self, *fields, **kwargs):
-        """
-        Person.page(1, 10).query('id', 'name', 'age', name='张三', age=55)
-        """
-        return self.cls.find_page(self.page_num, self.page_size, *fields, **kwargs)
-
-    def where(self, **kwargs) -> WherePageExec:
-        return WherePageExec(WhereExec(self.cls, **kwargs), self.page_num, self.page_size)
-
-    def fields(self, *fields) -> FieldPageExec:
-        return FieldPageExec(FieldExec(self.cls, *fields), self.page_num, self.page_size)
-
-
-def split_ids(ids: Sequence[int], batch_size):
-    return [ids[i:i + batch_size] for i in range(0, len(ids), batch_size)]
-
-
-def get_table_name(class_name):
-    for i in range(1, len(class_name) - 1)[::-1]:
-        if class_name[i].isupper():
-            class_name = class_name[:i] + '_' + class_name[i:]
-    return class_name.lower()
+from sqlexec.sql_support import get_table_select_sql
+from typing import Sequence, Union, List, Tuple
+from sqlexec.table_exec import get_condition_arg, get_where_arg_limit
+
+
+class FieldWherePageExec:
+    def __init__(self, field_where_exec, page_num, page_size):
+        self.field_where_exec = field_where_exec
+        self.page_num = page_num
+        self.page_size = page_size
+
+    def find(self):
+        return self.field_where_exec.find_page(self.page_num, self.page_size)
+
+    def query(self):
+        return self.field_where_exec.query_page(self.page_num, self.page_size)
+
+    def select(self):
+        return self.field_where_exec.select_page(self.page_num, self.page_size)
+
+
+class FieldWhereExec:
+    def __init__(self, field_exec, **kwargs):
+        self.field_exec = field_exec
+        self.kwargs = kwargs
+
+    def find(self):
+        """
+        Return list(object) or empty list if no result.
+        persons = Person.fields('id', 'name', 'age').where(name='张三', age=55).find()
+        """
+        return self.field_exec.find(**self.kwargs)
+
+    def find_one(self):
+        """
+        Return unique result(object) or None if no result.
+        person = Person.fields('id', 'name', 'age').where(name='张三', age=55).find_one()
+        """
+        return self.field_exec.find_one(**self.kwargs)
+
+    def query(self):
+        """
+        Return list(dict) or empty list if no result.
+        persons = Person.fields('id', 'name', 'age').where(name='张三', age=55).query()
+        """
+        return self.field_exec.query(**self.kwargs)
+
+    def query_one(self):
+        """
+        Return unique result(dict) or None if no result.
+        persons = Person.fields('id', 'name', 'age').where(name='张三', age=55).query_one()
+        """
+        return self.field_exec.query_one(**self.kwargs)
+
+    def select(self):
+        """
+        Return list(dict) or empty list if no result.
+        rows = Person.fields('id', 'name', 'age').where(name='张三', age=55).select()
+        """
+        return self.field_exec.select(**self.kwargs)
+
+    def select_one(self):
+        """
+        Return unique result(tuple) or None if no result.
+        row = Person.fields('id', 'name', 'age').where(name='张三', age=55).select_one()
+        """
+        return self.field_exec.select_one(**self.kwargs)
+
+    def find_page(self, page_num=1, page_size=10):
+        """
+        Return list(object) or empty list if no result.
+        persons = Person.fields('id', 'name', 'age').where(name='张三', age=55).find_page(1, 10)
+        :param page_num: page number
+        :param page_size: page size
+        """
+        return self.field_exec.find_page(page_num, page_size, **self.kwargs)
+
+    def query_page(self, page_num=1, page_size=10):
+        """
+        Return list(dict) or empty list if no result.
+        persons = Person.fields('id', 'name', 'age').where(name='张三', age=55).query_page(1, 10)
+        :param page_num: page number
+        :param page_size: page size
+        """
+        return self.field_exec.query_page(page_num, page_size, **self.kwargs)
+
+    def select_page(self, page_num=1, page_size=10):
+        """
+        Return list(dict) or empty list if no result.
+        rows = Person.fields('id', 'name', 'age').where(name='张三', age=55).select_page(1, 10)
+        :param page_num: page number
+        :param page_size: page size
+        """
+        return self.field_exec.select_page(page_num, page_size, **self.kwargs)
+
+    def page(self, page_num=1, page_size=10) -> FieldWherePageExec:
+        return FieldWherePageExec(self, page_num, page_size)
+
+
+class FieldPageExec:
+    def __init__(self, field_exec, page_num=1, page_size=10):
+        self.field_exec = field_exec
+        self.page_num = page_num
+        self.page_size = page_size
+
+    def find(self, **kwargs):
+        return self.field_exec.find_page(self.page_num, self.page_size, **kwargs)
+
+    def query(self, **kwargs):
+        return self.field_exec.query_page(self.page_num, self.page_size, **kwargs)
+
+    def select(self, **kwargs):
+        return self.field_exec.select_page(self.page_num, self.page_size, **kwargs)
+
+    def where(self, **kwargs) -> FieldWherePageExec:
+        return FieldWherePageExec(FieldWhereExec(self.field_exec, **kwargs), self.page_num, self.page_size)
+
+
+class FieldExec:
+    def __init__(self, cls, *fields):
+        self.cls = cls
+        self.fields = fields
+
+    def find(self, **kwargs):
+        """
+        Return list(object) or empty list if no result.
+        persons = Person.fields('id', 'name', 'age').find(name='张三', age=55)
+        """
+        return self.cls.find(*self.fields, **kwargs)
+
+    def find_one(self, **kwargs):
+        """
+        Return unique result(object) or None if no result.
+        person = Person.fields('id', 'name', 'age').find_one(name='张三', age=55)
+        """
+        return self.cls.find_one(*self.fields, **kwargs)
+
+    def find_by_id(self, _id: Union[int, str]):
+        """
+        Return one class object or None if no result.
+        person = Person.fields('id', 'name', 'age').find_by_id(1)
+        :param _id: key
+        """
+        return self.cls.find_by_id(_id, *self.fields)
+
+    def find_by_ids(self, *ids):
+        """
+        Return list(class object) or empty list if no result.
+        persons = Person.fields('id', 'name', 'age').find_by_ids(1,2)
+        :param ids: List of key
+        """
+        return self.cls.find_by_ids(ids, *self.fields)
+
+    def query(self, **kwargs):
+        """
+        Return list(dict) or empty list if no result.
+        persons = Person.fields('id', 'name', 'age').query(name='张三', age=55)
+        """
+        return self.cls.query(*self.fields, **kwargs)
+
+    def query_one(self, **kwargs):
+        """
+        Return unique result(dict) or None if no result.
+        persons = Person.fields('id', 'name', 'age').query_one(name='张三', age=55)
+        """
+        return self.cls.query_one(*self.fields, **kwargs)
+
+    def query_by_id(self, _id: Union[int, str]):
+        """
+        Return one row(dict) or None if no result.
+        person = Person.fields('id', 'name', 'age').query_by_id(1)
+        :param _id: key
+        """
+        return self.cls.query_by_id(_id, *self.fields)
+
+    def query_by_ids(self, *ids):
+        """
+        Return list(dict) or empty list if no result.
+        persons = Person.fields('id', 'name', 'age').query_by_ids(1,2)
+        :param ids: List of key
+        """
+        return self.cls.query_by_ids(ids, *self.fields)
+
+    def select(self, **kwargs):
+        """
+        Return list(dict) or empty list if no result.
+        rows = Person.fields('id', 'name', 'age').select(name='张三', age=55)
+        """
+        return self.cls.select(*self.fields, **kwargs)
+
+    def select_one(self, **kwargs):
+        """
+        Return unique result(tuple) or None if no result.
+        row = Person.fields('id', 'name', 'age').select_one(name='张三', age=55)
+        """
+        return self.cls.select_one(*self.fields, **kwargs)
+
+    def select_by_id(self, _id: Union[int, str]):
+        """
+        Return one row(dict) or None if no result.
+        row = Person.fields('id', 'name', 'age').select_by_id(1)
+        :param _id: key
+        """
+        return self.cls.select_by_id(_id, *self.fields)
+
+    def select_by_ids(self, *ids):
+        """
+        Return list(dict) or empty list if no result.
+        rows = Person.select_by_ids([1,2], 'id', 'name', 'age')
+        :param ids: List of key
+        :param fields: Default select all fields if not set
+        """
+        return self.cls.select_by_ids(ids, *self.fields)
+
+    def find_page(self, page_num=1, page_size=10, **kwargs):
+        """
+        Return list(object) or empty list if no result.
+        persons = Person.fields('id', 'name', 'age').find_page(1, 10, name='张三', age=55)
+        :param page_num: page number
+        :param page_size: page size
+        """
+        return self.cls.find_page(page_num, page_size, *self.fields, **kwargs)
+
+    def query_page(self, page_num=1, page_size=10, **kwargs):
+        """
+        Return list(dict) or empty list if no result.
+        persons = Person.fields('id', 'name', 'age').query_page(1, 10, name='张三', age=55)
+        :param page_num: page number
+        :param page_size: page size
+        """
+        return self.cls.query_page(page_num, page_size, *self.fields, **kwargs)
+
+    def select_page(self, page_num=1, page_size=10, **kwargs):
+        """
+        Return list(dict) or empty list if no result.
+        rows = Person.fields('id', 'name', 'age').select_page(1, 10, name='张三', age=55)
+        :param page_num: page number
+        :param page_size: page size
+        """
+        return self.cls.select_page(page_num, page_size, *self.fields, **kwargs)
+
+    def where(self, **kwargs) -> FieldWhereExec:
+        return FieldWhereExec(self, **kwargs)
+
+    def page(self, page_num=1, page_size=10) -> FieldPageExec:
+        return FieldPageExec(self, page_num, page_size)
+
+
+class WherePageExec:
+    def __init__(self, where_exec, page_num=1, page_size=10):
+        self.where_exec = where_exec
+        self.page_num = page_num
+        self.page_size = page_size
+
+    def select(self, *fields):
+        """
+        Return list(dict) or empty list if no result.
+        rows = Person.where(name='张三', age=55).page(1, 10).select()
+        """
+        return self.where_exec.select_page(self.page_num, self.page_size, *fields)
+
+    def query(self, *fields):
+        """
+        Return list(dict) or empty list if no result.
+        rows = Person.where(name='张三', age=55).page(1, 10).query()
+        """
+        return self.where_exec.query_page(self.page_num, self.page_size, *fields)
+
+    def find(self, *fields):
+        """
+        Return list(dict) or empty list if no result.
+        rows = Person.where(name='张三', age=55).page(1, 10).find()
+        """
+        return self.where_exec.find_page(self.page_num, self.page_size, *fields)
+
+    def fields(self, *fields) -> FieldWherePageExec:
+        return FieldWherePageExec(FieldWhereExec(FieldExec(self.where_exec.cls, *fields), **self.where_exec.kwargs), self.page_num, self.page_size)
+
+
+class WhereExec:
+    def __init__(self, cls, **kwargs):
+        self.cls = cls
+        self.kwargs = kwargs
+
+    def delete(self):
+        """
+        Physical delete
+        rowcount = Person.where(name='张三', age=55).delete()
+        return: Effect rowcount
+        """
+        return self.cls.delete(**self.kwargs)
+
+    def count(self):
+        """
+        count = Person.where(name='张三', age=55).count()
+        """
+        return self.cls.count(**self.kwargs)
+
+    def exists(self):
+        """
+        flag = Person.where(name='张三', age=55).exists()
+        """
+        return self.cls.exists(**self.kwargs)
+
+    def select(self, *fields):
+        """
+        Return list(dict) or empty list if no result.
+        rows = Person.where(name='张三', age=55).select()
+        """
+        return self.cls.select(*fields, **self.kwargs)
+
+    def query(self, *fields):
+        """
+        Return list(dict) or empty list if no result.
+        rows = Person.where(name='张三', age=55).query()
+        """
+        return self.cls.query(*fields, **self.kwargs)
+
+    def find(self, *fields):
+        """
+        Return list(dict) or empty list if no result.
+        rows = Person.where(name='张三', age=55).find()
+        """
+        return self.cls.find(*fields, **self.kwargs)
+
+    def select_page(self, page_num=1, page_size=10, *fields):
+        """
+        Return list(dict) or empty list if no result.
+        rows = Person.where(name='张三', age=55).select_page()
+        """
+        return self.cls.select_page(page_num, page_size, *fields, **self.kwargs)
+
+    def query_page(self, page_num=1, page_size=10, *fields):
+        """
+        Return list(dict) or empty list if no result.
+        rows = Person.where(name='张三', age=55).query_page()
+        """
+        return self.cls.query_page(page_num, page_size, *fields, **self.kwargs)
+
+    def find_page(self, page_num=1, page_size=10, *fields):
+        """
+        Return list(dict) or empty list if no result.
+        rows = Person.where(name='张三', age=55).find_page()
+        """
+        return self.cls.find_page(page_num, page_size, *fields, **self.kwargs)
+
+    def fields(self, *fields) -> FieldWhereExec:
+        return FieldWhereExec(FieldExec(self.cls, *fields), **self.kwargs)
+
+    def page(self, page_num=1, page_size=10) -> WherePageExec:
+        return WherePageExec(self, page_num, page_size)
+
+
+class PageExec:
+    
+    def __init__(self, cls, page_num=1, page_size=10):
+        self.cls = cls
+        self.page_num = page_num
+        self.page_size = page_size
+
+    def select(self, *fields, **kwargs):
+        """
+        Person.page(1, 10).select('id', 'name', 'age', name='张三', age=55)
+        """
+        return self.cls.select_page(self.page_num, self.page_size, *fields, **kwargs)
+
+    def query(self, *fields, **kwargs):
+        """
+        Person.page(1, 10).query('id', 'name', 'age', name='张三', age=55)
+        """
+        return self.cls.query_page(self.page_num, self.page_size, *fields, **kwargs)
+
+    def find(self, *fields, **kwargs):
+        """
+        Person.page(1, 10).query('id', 'name', 'age', name='张三', age=55)
+        """
+        return self.cls.find_page(self.page_num, self.page_size, *fields, **kwargs)
+
+    def where(self, **kwargs) -> WherePageExec:
+        return WherePageExec(WhereExec(self.cls, **kwargs), self.page_num, self.page_size)
+
+    def fields(self, *fields) -> FieldPageExec:
+        return FieldPageExec(FieldExec(self.cls, *fields), self.page_num, self.page_size)
+
+
+def split_ids(ids: Sequence[int], batch_size):
+    return [ids[i:i + batch_size] for i in range(0, len(ids), batch_size)]
+
+
+def get_table_name(class_name):
+    for i in range(1, len(class_name) - 1)[::-1]:
+        if class_name[i].isupper():
+            class_name = class_name[:i] + '_' + class_name[i:]
+    return class_name.lower()
```

### Comparing `sqlx-orm-0.0.6/PKG-INFO` & `sqlx-orm-0.0.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-Metadata-Version: 2.1
-Name: sqlx-orm
-Version: 0.0.6
-Summary: A single table ORM framework for python. Support MySQL, PostgreSQL, SQLite etc.
-Home-page: https://gitee.com/summry/sqlx-orm
-Author: summy
-Author-email: xiazhongbiao@126.com
-License: UNKNOWN
-Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python,RDB
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-Usage Sample
-''''''''''''
-
-.. code:: python
-
-    from orm import Model, db
-    from typing import List, Tuple, Mapping
-
-    class Person(Model):
-        __pk__ = 'id'
-        __table__ = 'person'
-
-        def __init__(self, id: int = None, name: str = None, age: int = None):
-            self.id = id
-            self.name = name
-            self.age = age
-
-
-    if __name__ == '__main__':
-        db.init('test.db', driver='sqlite3', show_sql=True, debug=True)
-        db.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5)
-        db.init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', pool_size=5, show_sql=True)
-
-        effected_rowcount = Person.insert(name='tianqi', age=77)
-
-        persons = Person.query(name='tianqi')
-        # select id, name, age from person where name = :name
-        # result:
-        # {'id': 7, 'name': 'tianqi', 'age': 77}
-
-        persons = Person.query(name__eq='zhangsan')
-        # select id, name, age from person where name = :name
-        # result:
-        # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
-
-Transaction
-'''''''''''
-
-.. code:: python
-
-    from orm import with_transaction, transaction
-
-    @with_transaction
-    def test_transaction():
-        insert_func(....)
-        update_func(....)
-
-
-    def test_transaction2():
-        with transaction():
-            insert_func(....)
-            update_func(....)
-
-
-If you want to operate MySQL database, may be you need MySqlx: https://pypi.org/project/mysqlx
-
-If you want to operate PostgreSQL database, may be you need MySqlx: https://pypi.org/project/pgsqlx
-
-If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlx-exec
-
-
+Metadata-Version: 2.1
+Name: sqlx-orm
+Version: 0.0.7
+Summary: A single table ORM framework for python. Support MySQL, PostgreSQL, SQLite etc.
+Home-page: https://gitee.com/summry/sqlx-orm
+Author: summy
+Author-email: xiazhongbiao@126.com
+License: UNKNOWN
+Keywords: SQL,MySQL,PostgreSQL,SQLite,Database,Python,RDB
+Platform: UNKNOWN
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+Usage Sample
+''''''''''''
+
+.. code:: python
+
+    from orm import Model, db
+    from typing import List, Tuple, Mapping
+
+    class Person(Model):
+        __pk__ = 'id'
+        __table__ = 'person'
+
+        def __init__(self, id: int = None, name: str = None, age: int = None):
+            self.id = id
+            self.name = name
+            self.age = age
+
+
+    if __name__ == '__main__':
+        db.init('test.db', driver='sqlite3', show_sql=True, debug=True)
+        db.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5)
+        db.init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', pool_size=5, show_sql=True)
+
+        effected_rowcount = Person.insert(name='tianqi', age=77)
+
+        persons = Person.query(name='tianqi')
+        # select id, name, age from person where name = :name
+        # result:
+        # {'id': 7, 'name': 'tianqi', 'age': 77}
+
+        persons = Person.query(name__eq='zhangsan')
+        # select id, name, age from person where name = :name
+        # result:
+        # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+
+Transaction
+'''''''''''
+
+.. code:: python
+
+    from orm import with_transaction, transaction
+
+    @with_transaction
+    def test_transaction():
+        insert_func(....)
+        update_func(....)
+
+
+    def test_transaction2():
+        with transaction():
+            insert_func(....)
+            update_func(....)
+
+
+If you want to operate MySQL database, may be you need MySqlx: https://pypi.org/project/mysqlx
+
+If you want to operate PostgreSQL database, may be you need MySqlx: https://pypi.org/project/pgsqlx
+
+If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlx-exec
+
+
```

### Comparing `sqlx-orm-0.0.6/README.rst` & `sqlx-orm-0.0.7/README.rst`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-Usage Sample
-''''''''''''
-
-.. code:: python
-
-    from orm import Model, db
-    from typing import List, Tuple, Mapping
-
-    class Person(Model):
-        __pk__ = 'id'
-        __table__ = 'person'
-
-        def __init__(self, id: int = None, name: str = None, age: int = None):
-            self.id = id
-            self.name = name
-            self.age = age
-
-
-    if __name__ == '__main__':
-        db.init('test.db', driver='sqlite3', show_sql=True, debug=True)
-        db.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5)
-        db.init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', pool_size=5, show_sql=True)
-
-        effected_rowcount = Person.insert(name='tianqi', age=77)
-
-        persons = Person.query(name='tianqi')
-        # select id, name, age from person where name = :name
-        # result:
-        # {'id': 7, 'name': 'tianqi', 'age': 77}
-
-        persons = Person.query(name__eq='zhangsan')
-        # select id, name, age from person where name = :name
-        # result:
-        # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
-
-Transaction
-'''''''''''
-
-.. code:: python
-
-    from orm import with_transaction, transaction
-
-    @with_transaction
-    def test_transaction():
-        insert_func(....)
-        update_func(....)
-
-
-    def test_transaction2():
-        with transaction():
-            insert_func(....)
-            update_func(....)
-
-
-If you want to operate MySQL database, may be you need MySqlx: https://pypi.org/project/mysqlx
-
-If you want to operate PostgreSQL database, may be you need MySqlx: https://pypi.org/project/pgsqlx
-
-If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlx-exec
+Usage Sample
+''''''''''''
+
+.. code:: python
+
+    from orm import Model, db
+    from typing import List, Tuple, Mapping
+
+    class Person(Model):
+        __pk__ = 'id'
+        __table__ = 'person'
+
+        def __init__(self, id: int = None, name: str = None, age: int = None):
+            self.id = id
+            self.name = name
+            self.age = age
+
+
+    if __name__ == '__main__':
+        db.init('test.db', driver='sqlite3', show_sql=True, debug=True)
+        db.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5)
+        db.init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', pool_size=5, show_sql=True)
+
+        effected_rowcount = Person.insert(name='tianqi', age=77)
+
+        persons = Person.query(name='tianqi')
+        # select id, name, age from person where name = :name
+        # result:
+        # {'id': 7, 'name': 'tianqi', 'age': 77}
+
+        persons = Person.query(name__eq='zhangsan')
+        # select id, name, age from person where name = :name
+        # result:
+        # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+
+Transaction
+'''''''''''
+
+.. code:: python
+
+    from orm import with_transaction, transaction
+
+    @with_transaction
+    def test_transaction():
+        insert_func(....)
+        update_func(....)
+
+
+    def test_transaction2():
+        with transaction():
+            insert_func(....)
+            update_func(....)
+
+
+If you want to operate MySQL database, may be you need MySqlx: https://pypi.org/project/mysqlx
+
+If you want to operate PostgreSQL database, may be you need MySqlx: https://pypi.org/project/pgsqlx
+
+If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlx-exec
```

### Comparing `sqlx-orm-0.0.6/sqlx_orm.egg-info/PKG-INFO` & `sqlx-orm-0.0.7/sqlx_orm.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-Metadata-Version: 2.1
-Name: sqlx-orm
-Version: 0.0.6
-Summary: A single table ORM framework for python. Support MySQL, PostgreSQL, SQLite etc.
-Home-page: https://gitee.com/summry/sqlx-orm
-Author: summy
-Author-email: xiazhongbiao@126.com
-License: UNKNOWN
-Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python,RDB
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-Usage Sample
-''''''''''''
-
-.. code:: python
-
-    from orm import Model, db
-    from typing import List, Tuple, Mapping
-
-    class Person(Model):
-        __pk__ = 'id'
-        __table__ = 'person'
-
-        def __init__(self, id: int = None, name: str = None, age: int = None):
-            self.id = id
-            self.name = name
-            self.age = age
-
-
-    if __name__ == '__main__':
-        db.init('test.db', driver='sqlite3', show_sql=True, debug=True)
-        db.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5)
-        db.init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', pool_size=5, show_sql=True)
-
-        effected_rowcount = Person.insert(name='tianqi', age=77)
-
-        persons = Person.query(name='tianqi')
-        # select id, name, age from person where name = :name
-        # result:
-        # {'id': 7, 'name': 'tianqi', 'age': 77}
-
-        persons = Person.query(name__eq='zhangsan')
-        # select id, name, age from person where name = :name
-        # result:
-        # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
-
-Transaction
-'''''''''''
-
-.. code:: python
-
-    from orm import with_transaction, transaction
-
-    @with_transaction
-    def test_transaction():
-        insert_func(....)
-        update_func(....)
-
-
-    def test_transaction2():
-        with transaction():
-            insert_func(....)
-            update_func(....)
-
-
-If you want to operate MySQL database, may be you need MySqlx: https://pypi.org/project/mysqlx
-
-If you want to operate PostgreSQL database, may be you need MySqlx: https://pypi.org/project/pgsqlx
-
-If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlx-exec
-
-
+Metadata-Version: 2.1
+Name: sqlx-orm
+Version: 0.0.7
+Summary: A single table ORM framework for python. Support MySQL, PostgreSQL, SQLite etc.
+Home-page: https://gitee.com/summry/sqlx-orm
+Author: summy
+Author-email: xiazhongbiao@126.com
+License: UNKNOWN
+Keywords: SQL,MySQL,PostgreSQL,SQLite,Database,Python,RDB
+Platform: UNKNOWN
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+Usage Sample
+''''''''''''
+
+.. code:: python
+
+    from orm import Model, db
+    from typing import List, Tuple, Mapping
+
+    class Person(Model):
+        __pk__ = 'id'
+        __table__ = 'person'
+
+        def __init__(self, id: int = None, name: str = None, age: int = None):
+            self.id = id
+            self.name = name
+            self.age = age
+
+
+    if __name__ == '__main__':
+        db.init('test.db', driver='sqlite3', show_sql=True, debug=True)
+        db.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5)
+        db.init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', pool_size=5, show_sql=True)
+
+        effected_rowcount = Person.insert(name='tianqi', age=77)
+
+        persons = Person.query(name='tianqi')
+        # select id, name, age from person where name = :name
+        # result:
+        # {'id': 7, 'name': 'tianqi', 'age': 77}
+
+        persons = Person.query(name__eq='zhangsan')
+        # select id, name, age from person where name = :name
+        # result:
+        # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+
+Transaction
+'''''''''''
+
+.. code:: python
+
+    from orm import with_transaction, transaction
+
+    @with_transaction
+    def test_transaction():
+        insert_func(....)
+        update_func(....)
+
+
+    def test_transaction2():
+        with transaction():
+            insert_func(....)
+            update_func(....)
+
+
+If you want to operate MySQL database, may be you need MySqlx: https://pypi.org/project/mysqlx
+
+If you want to operate PostgreSQL database, may be you need MySqlx: https://pypi.org/project/pgsqlx
+
+If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlx-exec
+
+
```

