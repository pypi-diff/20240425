# Comparing `tmp/mogo-0.5.1.tar.gz` & `tmp/mogo-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mogo-0.5.1.tar", last modified: Thu May 27 00:28:51 2021, max compression
+gzip compressed data, was "mogo-0.6.0.tar", last modified: Thu Apr 25 12:52:33 2024, max compression
```

## Comparing `mogo-0.5.1.tar` & `mogo-0.6.0.tar`

### file list

```diff
@@ -1,13 +1,29 @@
-drwxrwxr-x   0 jmarshall  (1000) jmarshall  (1000)        0 2021-05-27 00:28:51.595469 mogo-0.5.1/
--rw-rw-r--   0 jmarshall  (1000) jmarshall  (1000)      296 2021-05-27 00:28:51.595469 mogo-0.5.1/PKG-INFO
--rw-rw-r--   0 jmarshall  (1000) jmarshall  (1000)    11518 2021-05-18 03:28:34.056918 mogo-0.5.1/README
-drwxrwxr-x   0 jmarshall  (1000) jmarshall  (1000)        0 2021-05-27 00:28:51.595469 mogo-0.5.1/mogo/
--rw-rw-r--   0 jmarshall  (1000) jmarshall  (1000)      558 2021-05-18 03:28:34.056918 mogo-0.5.1/mogo/__init__.py
--rw-rw-r--   0 jmarshall  (1000) jmarshall  (1000)     4062 2021-05-18 03:28:34.056918 mogo-0.5.1/mogo/connection.py
--rw-rw-r--   0 jmarshall  (1000) jmarshall  (1000)     4325 2021-05-18 03:28:34.056918 mogo-0.5.1/mogo/cursor.py
--rw-rw-r--   0 jmarshall  (1000) jmarshall  (1000)      749 2021-05-18 03:28:34.056918 mogo-0.5.1/mogo/decorators.py
--rw-rw-r--   0 jmarshall  (1000) jmarshall  (1000)     9070 2021-05-18 03:28:34.056918 mogo-0.5.1/mogo/field.py
--rw-rw-r--   0 jmarshall  (1000) jmarshall  (1000)      194 2021-05-18 03:28:34.056918 mogo-0.5.1/mogo/helpers.py
--rw-rw-r--   0 jmarshall  (1000) jmarshall  (1000)    26201 2021-05-27 00:25:20.011389 mogo-0.5.1/mogo/model.py
--rw-rw-r--   0 jmarshall  (1000) jmarshall  (1000)        0 2021-05-18 03:28:34.056918 mogo-0.5.1/mogo/py.typed
--rw-rw-r--   0 jmarshall  (1000) jmarshall  (1000)      995 2021-05-27 00:25:20.011389 mogo-0.5.1/setup.py
+drwxr-xr-x   0 jmarshall  (1000) jmarshall  (1000)        0 2024-04-25 12:52:33.004234 mogo-0.6.0/
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)      524 2022-10-12 07:21:55.000000 mogo-0.6.0/LICENSE.txt
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)      311 2024-04-25 12:52:32.999234 mogo-0.6.0/PKG-INFO
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)    11518 2022-10-12 07:21:55.000000 mogo-0.6.0/README
+drwxr-xr-x   0 jmarshall  (1000) jmarshall  (1000)        0 2024-04-25 12:52:32.880234 mogo-0.6.0/mogo/
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)      558 2022-10-12 07:21:55.000000 mogo-0.6.0/mogo/__init__.py
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)     4161 2024-04-25 12:45:14.000000 mogo-0.6.0/mogo/connection.py
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)     4174 2024-04-25 12:45:14.000000 mogo-0.6.0/mogo/cursor.py
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)      761 2024-04-25 12:45:14.000000 mogo-0.6.0/mogo/decorators.py
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)     9070 2024-04-25 12:45:09.000000 mogo-0.6.0/mogo/field.py
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)      264 2024-04-25 12:45:14.000000 mogo-0.6.0/mogo/helpers.py
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)    25932 2024-04-25 12:45:14.000000 mogo-0.6.0/mogo/model.py
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)        0 2022-10-12 07:21:55.000000 mogo-0.6.0/mogo/py.typed
+drwxr-xr-x   0 jmarshall  (1000) jmarshall  (1000)        0 2024-04-25 12:52:32.994235 mogo-0.6.0/mogo.egg-info/
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)      311 2024-04-25 12:52:32.000000 mogo-0.6.0/mogo.egg-info/PKG-INFO
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)      443 2024-04-25 12:52:32.000000 mogo-0.6.0/mogo.egg-info/SOURCES.txt
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)        1 2024-04-25 12:52:32.000000 mogo-0.6.0/mogo.egg-info/dependency_links.txt
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)        1 2024-04-25 12:52:32.000000 mogo-0.6.0/mogo.egg-info/not-zip-safe
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)       13 2024-04-25 12:52:32.000000 mogo-0.6.0/mogo.egg-info/requires.txt
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)        5 2024-04-25 12:52:32.000000 mogo-0.6.0/mogo.egg-info/top_level.txt
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)      100 2022-10-12 07:21:55.000000 mogo-0.6.0/pyproject.toml
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)       38 2024-04-25 12:52:33.004234 mogo-0.6.0/setup.cfg
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)      995 2024-04-25 12:45:14.000000 mogo-0.6.0/setup.py
+drwxr-xr-x   0 jmarshall  (1000) jmarshall  (1000)        0 2024-04-25 12:52:32.981234 mogo-0.6.0/tests/
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)      850 2022-11-03 04:29:48.000000 mogo-0.6.0/tests/test_decorators.py
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)     6494 2024-04-25 12:45:09.000000 mogo-0.6.0/tests/test_field.py
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)      552 2022-10-12 07:21:55.000000 mogo-0.6.0/tests/test_helpers.py
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)    11753 2024-04-25 12:45:14.000000 mogo-0.6.0/tests/test_model.py
+-rw-r--r--   0 jmarshall  (1000) jmarshall  (1000)    25604 2024-04-25 12:45:14.000000 mogo-0.6.0/tests/test_usage.py
```

### Comparing `mogo-0.5.1/README` & `mogo-0.6.0/README`

 * *Files identical despite different names*

### Comparing `mogo-0.5.1/mogo/__init__.py` & `mogo-0.6.0/mogo/__init__.py`

 * *Files identical despite different names*

### Comparing `mogo-0.5.1/mogo/connection.py` & `mogo-0.6.0/mogo/connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """ The wrapper for pymongo's connection stuff. """
 
+from mogo.helpers import Document
+
 from urllib.parse import urlparse
 from pymongo import MongoClient
 from pymongo.collection import Collection
 from pymongo.database import Database
 from pymongo.errors import ConnectionFailure
 
 from types import TracebackType
@@ -14,28 +16,28 @@
     """
     This just caches a pymongo connection and adds
     a few shortcuts.
     """
 
     _instance = None  # type: Optional['Connection']
     _database = None  # type: Optional[str]
-    connection = None  # type: Optional[MongoClient]
+    connection: Optional[MongoClient[Document]] = None
 
     @classmethod
     def instance(cls) -> "Connection":
         """ Retrieves the shared connection. """
         if not cls._instance:
             cls._instance = Connection()
         return cls._instance
 
     @classmethod
     def connect(
             cls, database: Optional[str] = None,
             uri: str = "mongodb://localhost:27017",
-            **kwargs: Any) -> MongoClient:
+            **kwargs: Any) -> MongoClient[Document]:
         """
         Wraps a pymongo connection.
         TODO: Allow some of the URI stuff.
         """
         if not database:
             database = urlparse(uri).path
             while database.startswith("/"):
@@ -44,28 +46,31 @@
                 raise ValueError("A database name is required to connect.")
 
         conn = cls.instance()
         conn._database = database
         conn.connection = MongoClient(uri, **kwargs)
         return conn.connection
 
-    def get_database(self, database: Optional[str] = None) -> Database:
+    def get_database(
+        self,
+        database: Optional[str] = None
+    ) -> Database[Document]:
         """ Retrieves a database from an existing connection. """
         if not self.connection:
             raise ConnectionFailure('No connection')
         if not database:
             if not self._database:
                 raise Exception('No database submitted')
             database = self._database
         return self.connection[database]
 
     def get_collection(
             self,
             collection: str,
-            database: Optional[str] = None) -> Collection:
+            database: Optional[str] = None) -> Collection[Document]:
         """ Retrieve a collection from an existing connection. """
         return self.get_database(database=database)[collection]
 
 
 class Session(object):
     """ This class just wraps a connection instance """
 
@@ -107,15 +112,15 @@
             exc_type: Optional[Type[Exception]],
             exc_value: Optional[Exception],
             traceback: Optional[TracebackType]) -> None:
         """ Close the connection """
         self.disconnect()
 
 
-def connect(*args: Any, **kwargs: Any) -> MongoClient:
+def connect(*args: Any, **kwargs: Any) -> MongoClient[Document]:
     """
     Initializes a connection and the database. It returns
     the pymongo connection object so that end_request, etc.
     can be called if necessary.
     """
     return Connection.connect(*args, **kwargs)
```

### Comparing `mogo-0.5.1/mogo/cursor.py` & `mogo-0.6.0/mogo/cursor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-from mogo.helpers import check_none
+from mogo.helpers import check_none, Document
 
 from pymongo import ASCENDING, DESCENDING
 from pymongo.collation import Collation
 from pymongo.cursor import Cursor as PyCursor
 
-from typing import Any, cast, Dict, Generic, Iterator, List, Optional, Tuple
+from typing import Any, cast, Dict, Generic, Optional
 from typing import Type, TypeVar, TYPE_CHECKING
 
+from typing import List, Tuple  # noqa: F401
+
 
 ASC = ASCENDING
 DESC = DESCENDING
 
 T = TypeVar("T", bound="Model")
 
 
 class Cursor(Generic[T]):
     """ A simple wrapper around pymongo's Cursor class. """
 
     _order_entries = []  # type: List[Tuple[str, int]]
     _query = None  # type: Optional[Dict[str, Any]]
     _model = None  # type: Optional[Type[T]]
     _model_class = None  # type: Optional[Type[T]]
-    _cursor = None  # type: Optional[PyCursor]
+    _cursor: Optional[PyCursor[Document]] = None
 
     def __init__(
             self,
             model: Type[T],
             spec: Optional[Dict[str, Any]] = None,
             *args: Any,
             **kwargs: Any) -> None:
@@ -46,18 +48,15 @@
     def next(self) -> T:
         # still need this, since pymongo's cursor still implements next()
         # and returns the raw dict.
         return self.__next__()
 
     def count(self) -> int:
         collection = check_none(self._model_class)._get_collection()
-        if hasattr(collection, "count_documents"):
-            return collection.count_documents(self._query or {})
-        # count on a cursor is deprecated, ultimately this will be removed
-        return check_none(self._cursor).count()
+        return collection.count_documents(self._query or {})
 
     # convenient because if it quacks like a list...
     def __len__(self) -> int:
         return self.count()
 
     def __getitem__(self, index: int) -> T:
         value = check_none(self._cursor).__getitem__(index)
@@ -69,17 +68,18 @@
         return check_none(self._cursor).close()
 
     def rewind(self) -> "Cursor[T]":
         check_none(self._cursor).rewind()
         return self
 
     def first(self) -> Optional[T]:
-        if self.count() == 0:
+        try:
+            return self.next()
+        except StopIteration:
             return None
-        return self.next()
 
     def collation(self, collation: Collation) -> "Cursor[T]":
         check_none(self._cursor).collation(collation)
         return self
 
     def skip(self, skip: int) -> "Cursor[T]":
         check_none(self._cursor).skip(skip)
@@ -118,16 +118,16 @@
             self._query, modifier, multi=True)
         return self
 
     def change(self, **kwargs: Any) -> "Cursor[T]":
         modifier = {"$set": kwargs}
         return self.update(modifier)
 
-    def distinct(self, key: str) -> Iterator[Any]:
-        return cast(Iterator[Any], check_none(self._cursor).distinct(key))
+    def distinct(self, key: str) -> list[Any]:
+        return check_none(self._cursor).distinct(key)
 
 
 if TYPE_CHECKING:
     from mogo.model import Model  # noqa: F401
 
 
 __all__ = ["Cursor", "ASC", "DESC"]
```

### Comparing `mogo-0.5.1/mogo/decorators.py` & `mogo-0.6.0/mogo/decorators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """
 Just various decorators.
 """
 
-from typing import Any, cast, Callable, Optional, Type, TypeVar, Union
+from typing import Any, Callable, Optional, Type, TypeVar, Union
 
 
 T = TypeVar("T")
 
 
 class notinstancemethod(object):
     """
     Used to refuse access to a classmethod if called from an instance.
     """
 
-    def __init__(self, func: Union[Callable[..., T], classmethod]) -> None:
+    def __init__(
+        self,
+        func: Union[Callable[..., T], "classmethod[Any, ..., T]"]
+    ) -> None:
         if type(func) is not classmethod:
             raise ValueError("`notinstancemethod` called on non-classmethod")
         self.func = func
 
     def __get__(
             self, obj: Any,
             objtype: Optional[Type[Any]] = None) -> Callable[..., T]:
         if obj is not None:
             raise TypeError("Cannot call this method on an instance.")
-        return cast(classmethod, self.func).__get__(obj, objtype)
+        return self.func.__get__(obj, objtype)
```

### Comparing `mogo-0.5.1/mogo/field.py` & `mogo-0.6.0/mogo/field.py`

 * *Files identical despite different names*

### Comparing `mogo-0.5.1/mogo/model.py` & `mogo-0.6.0/mogo/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 import warnings
 
 import mogo
 from mogo.connection import Connection, Session
 from mogo.decorators import notinstancemethod
 from mogo.cursor import Cursor
 from mogo.field import Field, EmptyRequiredField
-from mogo.helpers import check_none
+from mogo.helpers import check_none, Document
 
 from bson.dbref import DBRef
 from bson.objectid import ObjectId
 from pymongo.collection import Collection
 from pymongo.results import DeleteResult, UpdateResult
 
 import typing
@@ -86,15 +86,15 @@
     """
     pass
 
 
 class NewModelClass(type):
     """ Metaclass for inheriting field lists """
 
-    def __new__(  # type: ignore
+    def __new__(
             cls,
             name: str,
             bases: Tuple[type, ...],
             attributes: Dict[str, Any]) -> Type[M]:
         # Emptying fields by default
         attributes["__fields"] = {}
         new_model = cast(
@@ -127,16 +127,16 @@
     for result in Foo.find({'user':'admin'}):
         print result.password
     """
 
     _id_field = "_id"  # type: str
     _id_type = ObjectId  # type: Any
     _name = None  # type: Optional[str]
-    _pymongo_data = None  # type: Optional[Dict[str, Any]]
-    _collection = None  # type: Optional[Collection]
+    _pymongo_data: Optional[dict[str, Any]] = None
+    _collection: Optional[Collection[Document]] = None
     _child_models = None  # type: Optional[Dict[Any, Type["PolyModel"]]]
     _init_okay = False  # type: bool
     __fields = None  # type: Optional[Dict[int, str]]
 
     AUTO_CREATE_FIELDS = None  # type: Optional[bool]
 
     # DEPRECATED
@@ -189,15 +189,15 @@
             pass
 
         Wrapped.__name__ = cls.__name__
         connection = session.connection
         if connection is None:
             raise Exception("No connection for session.")
         collection = connection.get_collection(
-            Wrapped._get_name())  # type: Collection
+            Wrapped._get_name())  # type: Collection[Any]
         Wrapped._collection = collection
         return Wrapped
 
     @classmethod
     def create(cls: Type[M], **kwargs: Any) -> M:
         """ Create a new model and save it. """
         if hasattr(cls, "new"):
@@ -260,15 +260,15 @@
 
     @classmethod
     def add_field(
             cls: Type[M],
             field_name: str,
             new_field_descriptor: Any) -> None:
         """ Adds a new field to the class """
-        assert(isinstance(new_field_descriptor, Field))
+        assert isinstance(new_field_descriptor, Field)
         setattr(cls, field_name, new_field_descriptor)
         cls._update_fields()
 
     def _get_id(self: M) -> Optional[Any]:
         """
         This is the internal id retrieval.
         The .id property is the public method for getting
@@ -297,15 +297,15 @@
     @classmethod
     def _class_update(
             cls: Type[M], *args: Any, **kwargs: Any) -> UpdateResult:
         """ Direct passthru to PyMongo's update. """
         if "safe" in kwargs:
             warn_about_keyword_deprecation("safe")
             del kwargs["safe"]
-        coll = cls._get_collection()  # type: Collection
+        coll = cls._get_collection()  # type: Collection[Any]
         if "multi" in kwargs and kwargs.pop("multi") is True:
             return coll.update_many(*args, **kwargs)
         return coll.update_one(*args, **kwargs)
 
     def _instance_update(self: M, **kwargs: Any) -> UpdateResult:
         """ Wraps keyword arguments with setattr and then uses PyMongo's
         update call.
@@ -420,15 +420,15 @@
             # Model.find_one({}, timeout=False)
             raise ValueError(
                 "find_one() requires a query when called with "
                 "keyword arguments")
         if "timeout" in kwargs:
             warn_about_keyword_deprecation("timeout")
             del kwargs["timeout"]
-        coll = cls._get_collection()  # type: Collection
+        coll = cls._get_collection()  # type: Collection[Any]
         find_result = coll.find_one(
             *args, **kwargs)  # type: Optional[Dict[str, Any]]
         result = None  # type: Optional[M]
         if find_result is not None:
             result = cls(**find_result)
         return result
 
@@ -447,28 +447,20 @@
 
         if "timeout" in kwargs:
             warn_about_keyword_deprecation("timeout")
             del kwargs["timeout"]
 
         return Cursor(cls, *args, **kwargs)
 
-    @classmethod
-    def group(
-            cls: Type[M],
-            *args: Any,
-            **kwargs: Any) -> Iterator[Dict[str, Any]]:
-        # This is deprecated, and will be removed from PyMongo in version 4.0
-        return cls._get_collection().group(*args, **kwargs)
-
     @notinstancemethod
     @classmethod
     def aggregate(
             cls: Type[M],
             pipeline: Sequence[Dict[str, Any]],
-            **kwargs: Any) -> Iterator[Dict[str, Any]]:
+            **kwargs: Any) -> Iterator[Document]:
         return cls._get_collection().aggregate(pipeline, **kwargs)
 
     @classmethod
     def search(cls: Type[M], **kwargs: Any) -> Cursor[M]:
         """
         Helper method that wraps keywords to dict and automatically
         turns instances into DBRefs.
@@ -500,15 +492,15 @@
         """ Helper for returning Blah.search(foo=bar).first(). """
         result = cls.search(**kwargs)  # type: Cursor[M]
         return result.first()
 
     @classmethod
     def grab(cls: Type[M], object_id: Any) -> Optional[M]:
         """ A shortcut to retrieve one object by its id. """
-        if type(object_id) != cls._id_type:
+        if not isinstance(object_id, cls._id_type):
             object_id = cls._id_type(object_id)
         return cls.find_one({cls._id_field: object_id})
 
     @classmethod
     def create_index(cls: Type[M], *args: Any, **kwargs: Any) -> Any:
         """ Wrapper for collection create_index() """
         return cls._get_collection().create_index(*args, **kwargs)
@@ -520,28 +512,29 @@
 
     @classmethod
     def drop_indexes(cls: Type[M], *args: Any, **kwargs: Any) -> Any:
         """ Wrapper for collection drop_indexes() """
         return cls._get_collection().drop_indexes(*args, **kwargs)
 
     @classmethod
-    def distinct(cls: Type[M], key: str) -> Iterator[Any]:
+    def distinct(cls: Type[M], key: str) -> list[Any]:
         """ Wrapper for collection distinct() """
         return cls.find().distinct(key)
 
     # Map Reduce and Group methods eventually go here.
 
     @classmethod
-    def _get_collection(cls: Type[M]) -> Collection:
+    def _get_collection(cls: Type[M]) -> Collection[Document]:
         """ Connects and caches the collection connection object. """
-        if not cls._collection:
-            conn = Connection.instance()
-            coll = conn.get_collection(cls._get_name())  # type: Collection
-            cls._collection = coll
-        return cls._collection
+        if cls._collection is not None:
+            # Use collection provided by Session, if available.
+            return cls._collection
+
+        conn = Connection.instance()
+        return conn.get_collection(cls._get_name())
 
     @classmethod
     def _get_name(cls: Type[M]) -> str:
         """
         Retrieves the collection name.
         Overwrite _name to set it manually.
         """
@@ -585,15 +578,15 @@
             **kwargs: Any) -> int:
         return cls._get_collection().count_documents(filter, *args, **kwargs)
 
     @notinstancemethod
     @classmethod
     def make_ref(cls: Type[M], idval: Any) -> DBRef:
         """ Generates a DBRef for a given id. """
-        if type(idval) != cls._id_type and callable(cls._id_type):
+        if not isinstance(idval, cls._id_type) and callable(cls._id_type):
             # Casting to ObjectId (or str, or whatever is configured)
             id_type = cast(Callable[..., M], cls._id_type)
             idval = id_type(idval)
         return DBRef(cls._get_name(), idval)
 
     def get_ref(self: M) -> DBRef:
         """ Returns a DBRef for an document. """
@@ -626,15 +619,15 @@
         key_field = getattr(cls, cls.get_child_key(), None)
         key = kwargs.get(cls.get_child_key())
         if cls._child_models is not None:
             if not key and key_field:
                 key = key_field._get_default()
             if key in cls._child_models:
                 create_class = cast(Type[P], cls._child_models[key])
-        return cast(P, super().__new__(create_class))
+        return super().__new__(create_class)
 
     @classmethod
     def get_child_key(cls: Type[P]) -> str:
         raise NotImplementedError("`get_child_key() -> str` not implemented.")
 
     # the following need double noqa: comments because Flake8 performs the
     # check at different levels depending on the version of Python...
@@ -667,15 +660,15 @@
             return wrap
         elif not inspect.isclass(value):
             def wrap(child_cls: Type[P]) -> Type[P]:
                 poly_name = name or child_cls.__name__.lower()
                 return _wrap_polymodel(cls, poly_name, value, child_cls)
             return wrap
         elif issubclass(value, cls):
-            child_cls = cast(Type[P], value)
+            child_cls = value
             name = child_cls.__name__.lower()
             value = name
             return _wrap_polymodel(cls, name, value, child_cls)
         else:
             raise ValueError(
                 "Could not register polymodel value {}".format(value))
```

### Comparing `mogo-0.5.1/setup.py` & `mogo-0.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 limitations under the License.
 """
 
 from distutils.core import setup
 
 setup(
     name='mogo',
-    version='0.5.1',
+    version='0.6.0',
     description='Simple PyMongo "schema-less" object wrapper',
     author='Josh Marshall',
     author_email='catchjosh@gmail.com',
     url="http://github.com/joshmarshall/mogo/",
     license="http://www.apache.org/licenses/LICENSE-2.0",
     package_data={"mogo": ["py.typed"]},
     packages=['mogo', ],
-    install_requires=["pymongo>=3.0"],
+    install_requires=["pymongo>=4.1"],
     zip_safe=False)
```

