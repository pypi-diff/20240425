# Comparing `tmp/pydantic-mongo-2.2.0.tar.gz` & `tmp/pydantic_mongo-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-mongo-2.2.0.tar", last modified: Thu Apr 11 22:54:04 2024, max compression
+gzip compressed data, was "pydantic_mongo-2.3.0.tar", last modified: Thu Apr 25 03:05:34 2024, max compression
```

## Comparing `pydantic-mongo-2.2.0.tar` & `pydantic_mongo-2.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:54:04.614344 pydantic-mongo-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-11 22:54:04.614344 pydantic-mongo-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:54:04.614344 pydantic-mongo-2.2.0/pydantic_mongo/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/pydantic_mongo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9672 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/pydantic_mongo/abstract_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/pydantic_mongo/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/pydantic_mongo/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/pydantic_mongo/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/pydantic_mongo/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/pydantic_mongo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:54:04.614344 pydantic-mongo-2.2.0/pydantic_mongo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-11 22:54:04.000000 pydantic-mongo-2.2.0/pydantic_mongo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-11 22:54:04.000000 pydantic-mongo-2.2.0/pydantic_mongo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:54:04.000000 pydantic-mongo-2.2.0/pydantic_mongo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-11 22:54:04.000000 pydantic-mongo-2.2.0/pydantic_mongo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 22:54:04.000000 pydantic-mongo-2.2.0/pydantic_mongo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-11 22:54:04.614344 pydantic-mongo-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:54:04.614344 pydantic-mongo-2.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/test/test_enhance_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/test/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/test/test_pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/test/test_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:05:34.607514 pydantic_mongo-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-25 03:05:25.000000 pydantic_mongo-2.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-25 03:05:34.607514 pydantic_mongo-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-25 03:05:25.000000 pydantic_mongo-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:05:34.607514 pydantic_mongo-2.3.0/pydantic_mongo/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-25 03:05:25.000000 pydantic_mongo-2.3.0/pydantic_mongo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-25 03:05:25.000000 pydantic_mongo-2.3.0/pydantic_mongo/abstract_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-25 03:05:25.000000 pydantic_mongo-2.3.0/pydantic_mongo/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-25 03:05:25.000000 pydantic_mongo-2.3.0/pydantic_mongo/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-25 03:05:25.000000 pydantic_mongo-2.3.0/pydantic_mongo/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 03:05:25.000000 pydantic_mongo-2.3.0/pydantic_mongo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 03:05:25.000000 pydantic_mongo-2.3.0/pydantic_mongo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:05:34.607514 pydantic_mongo-2.3.0/pydantic_mongo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-25 03:05:34.000000 pydantic_mongo-2.3.0/pydantic_mongo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-25 03:05:34.000000 pydantic_mongo-2.3.0/pydantic_mongo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 03:05:34.000000 pydantic_mongo-2.3.0/pydantic_mongo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 03:05:34.000000 pydantic_mongo-2.3.0/pydantic_mongo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 03:05:34.000000 pydantic_mongo-2.3.0/pydantic_mongo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-25 03:05:25.000000 pydantic_mongo-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-25 03:05:34.607514 pydantic_mongo-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-25 03:05:25.000000 pydantic_mongo-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:05:34.607514 pydantic_mongo-2.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-25 03:05:25.000000 pydantic_mongo-2.3.0/test/test_enhance_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-25 03:05:25.000000 pydantic_mongo-2.3.0/test/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-25 03:05:25.000000 pydantic_mongo-2.3.0/test/test_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-04-25 03:05:25.000000 pydantic_mongo-2.3.0/test/test_repository.py
```

### Comparing `pydantic-mongo-2.2.0/LICENSE.md` & `pydantic_mongo-2.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pydantic-mongo-2.2.0/PKG-INFO` & `pydantic_mongo-2.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-mongo
-Version: 2.2.0
+Version: 2.3.0
 Summary: Document object mapper for pydantic and pymongo
 Home-page: https://github.com/jefersondaniel/pydantic-mongo
 Author: Jeferson Daniel
 Author-email: jeferson.daniel412@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -33,29 +33,30 @@
 ```
 
 ### Example Code
 
 ```python
 from bson import ObjectId
 from pydantic import BaseModel
-from pydantic_mongo import AbstractRepository, ObjectIdField
+from pydantic_mongo import AbstractRepository, PydanticObjectId
 from pymongo import MongoClient
-from typing import List
+from typing import Optional, List
 import os
 
 class Foo(BaseModel):
    count: int
    size: float = None
 
 class Bar(BaseModel):
    apple: str = 'x'
    banana: str = 'y'
 
 class Spam(BaseModel):
-   id: ObjectIdField = None
+   # PydanticObjectId is an alias to Annotated[ObjectId, ObjectIdAnnotation]
+   id: Optional[PydanticObjectId] = None
    foo: Foo
    bars: List[Bar]
 
 class SpamRepository(AbstractRepository[Spam]):
    class Meta:
       collection_name = 'spams'
 
@@ -80,15 +81,15 @@
 
 # Delete
 spam_repository.delete(spam)
 
 # Find One By Id
 result = spam_repository.find_one_by_id(spam.id)
 
-# Find One By Id using string if the id attribute is a ObjectIdField
+# Find One By Id using string if the id attribute is a PydanticObjectId
 result = spam_repository.find_one_by_id(ObjectId('611827f2878b88b49ebb69fc'))
 assert result.foo.count == 2
 
 # Find One By Query
 result = spam_repository.find_one_by({'foo.count': 1})
 
 # Find By Query
```

### Comparing `pydantic-mongo-2.2.0/README.md` & `pydantic_mongo-2.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -13,29 +13,30 @@
 ```
 
 ### Example Code
 
 ```python
 from bson import ObjectId
 from pydantic import BaseModel
-from pydantic_mongo import AbstractRepository, ObjectIdField
+from pydantic_mongo import AbstractRepository, PydanticObjectId
 from pymongo import MongoClient
-from typing import List
+from typing import Optional, List
 import os
 
 class Foo(BaseModel):
    count: int
    size: float = None
 
 class Bar(BaseModel):
    apple: str = 'x'
    banana: str = 'y'
 
 class Spam(BaseModel):
-   id: ObjectIdField = None
+   # PydanticObjectId is an alias to Annotated[ObjectId, ObjectIdAnnotation]
+   id: Optional[PydanticObjectId] = None
    foo: Foo
    bars: List[Bar]
 
 class SpamRepository(AbstractRepository[Spam]):
    class Meta:
       collection_name = 'spams'
 
@@ -60,15 +61,15 @@
 
 # Delete
 spam_repository.delete(spam)
 
 # Find One By Id
 result = spam_repository.find_one_by_id(spam.id)
 
-# Find One By Id using string if the id attribute is a ObjectIdField
+# Find One By Id using string if the id attribute is a PydanticObjectId
 result = spam_repository.find_one_by_id(ObjectId('611827f2878b88b49ebb69fc'))
 assert result.foo.count == 2
 
 # Find One By Query
 result = spam_repository.find_one_by({'foo.count': 1})
 
 # Find By Query
```

### Comparing `pydantic-mongo-2.2.0/pydantic_mongo/abstract_repository.py` & `pydantic_mongo-2.3.0/pydantic_mongo/abstract_repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     Iterable,
     Optional,
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
+    cast,
 )
 
 from pydantic import BaseModel
 from pymongo import UpdateOne
 from pymongo.collection import Collection
 from pymongo.database import Database
 from pymongo.results import InsertOneResult, UpdateResult
@@ -22,18 +23,21 @@
     decode_pagination_cursor,
     encode_pagination_cursor,
     get_pagination_cursor_payload,
 )
 
 T = TypeVar("T", bound=BaseModel)
 OutputT = TypeVar("OutputT", bound=BaseModel)
-
 Sort = Sequence[Tuple[str, int]]
 
 
+class ModelWithId(BaseModel):
+    id: Any
+
+
 class AbstractRepository(Generic[T]):
     class Meta:
         collection_name: str
 
     def __init__(self, database: Database):
         super().__init__()
         self.__database: Database = database
@@ -49,32 +53,31 @@
     Get pymongo collection
     """
 
     def get_collection(self) -> Collection:
         return self.__database[self.__collection_name]
 
     def __validate(self):
-        if not issubclass(self.__document_class, BaseModel):
-            raise Exception("Document class should inherit BaseModel")
         if "id" not in self.__document_class.model_fields:
             raise Exception("Document class should have id field")
         if not self.__collection_name:
             raise Exception("Meta should contain collection name")
 
     @staticmethod
     def to_document(model: T) -> dict:
         """
         Convert model to document
         :param model:
         :return: dict
         """
-        data = model.model_dump()
+        model_with_id = cast(ModelWithId, model)
+        data = model_with_id.model_dump()
         data.pop("id")
-        if model.id:
-            data["_id"] = model.id
+        if model_with_id.id:
+            data["_id"] = model_with_id.id
         return data
 
     def __map_id(self, data: dict) -> dict:
         query = data.copy()
         if "id" in data:
             query["_id"] = query.pop("id")
         return query
@@ -105,58 +108,60 @@
         return self.to_model_custom(self.__document_class, data)
 
     def save(self, model: T) -> Union[InsertOneResult, UpdateResult]:
         """
         Save entity to database. It will update the entity if it has id, otherwise it will insert it.
         """
         document = self.to_document(model)
+        model_with_id = cast(ModelWithId, model)
 
-        if model.id:
+        if model_with_id.id:
             mongo_id = document.pop("_id")
             return self.get_collection().update_one(
                 {"_id": mongo_id}, {"$set": document}, upsert=True
             )
 
         result = self.get_collection().insert_one(document)
-        model.id = result.inserted_id
+        model_with_id.id = result.inserted_id
         return result
 
     def save_many(self, models: Iterable[T]):
         """
         Save multiple entities to database
         """
         models_to_insert = []
         models_to_update = []
 
         for model in models:
-            if model.id:
+            model_with_id = cast(ModelWithId, model)
+            if model_with_id.id:
                 models_to_update.append(model)
             else:
                 models_to_insert.append(model)
         if len(models_to_insert) > 0:
             result = self.get_collection().insert_many(
                 (self.to_document(model) for model in models_to_insert)
             )
 
             for idx, inserted_id in enumerate(result.inserted_ids):
-                models_to_insert[idx].id = inserted_id
+                cast(ModelWithId, models_to_insert[idx]).id = inserted_id
 
         if len(models_to_update) == 0:
             return
 
         documents_to_update = [self.to_document(model) for model in models_to_update]
         mongo_ids = [doc.pop("_id") for doc in documents_to_update]
         bulk_operations = [
             UpdateOne({"_id": mongo_id}, {"$set": document}, upsert=True)
             for mongo_id, document in zip(mongo_ids, documents_to_update)
         ]
         self.get_collection().bulk_write(bulk_operations)
 
     def delete(self, model: T):
-        return self.get_collection().delete_one({"_id": model.id})
+        return self.get_collection().delete_one({"_id": cast(ModelWithId, model).id})
 
     def delete_by_id(self, _id: Any):
         return self.get_collection().delete_one({"_id": _id})
 
     def find_one_by_id(self, _id: Any) -> Optional[T]:
         """
         Find entity by id
@@ -194,15 +199,15 @@
         mapped_projection = self.__map_id(projection) if projection else None
         mapped_sort = self.__map_sort(sort) if sort else None
         cursor = self.get_collection().find(self.__map_id(query), mapped_projection)
         if limit:
             cursor.limit(limit)
         if skip:
             cursor.skip(skip)
-        if sort:
+        if mapped_sort:
             cursor.sort(mapped_sort)
         return map(lambda doc: self.to_model_custom(output_type, doc), cursor)
 
     def find_by(
         self,
         query: dict,
         skip: Optional[int] = None,
@@ -281,15 +286,15 @@
             ),
             limit=limit,
             sort=sort,
             projection=projection,
         )
 
         return map(
-            lambda model: Edge[T](
+            lambda model: Edge[OutputT](
                 node=model,
                 cursor=encode_pagination_cursor(
                     get_pagination_cursor_payload(model, sort_keys)
                 ),
             ),
             models,
         )
```

### Comparing `pydantic-mongo-2.2.0/pydantic_mongo/pagination.py` & `pydantic_mongo-2.3.0/pydantic_mongo/pagination.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class Edge(BaseModel, Generic[DataT]):
     node: DataT
     cursor: str
 
 
 def encode_pagination_cursor(data: List) -> str:
-    byte_data = bson.BSON.encode({"v": data})
+    byte_data: bytes = bson.BSON.encode({"v": data})
     byte_data = zlib.compress(byte_data, 9)
     return b64encode(byte_data).decode("utf-8")
 
 
 def decode_pagination_cursor(data: str) -> List:
     try:
         byte_data = b64decode(data.encode("utf-8"))
```

### Comparing `pydantic-mongo-2.2.0/pydantic_mongo.egg-info/PKG-INFO` & `pydantic_mongo-2.3.0/pydantic_mongo.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-mongo
-Version: 2.2.0
+Version: 2.3.0
 Summary: Document object mapper for pydantic and pymongo
 Home-page: https://github.com/jefersondaniel/pydantic-mongo
 Author: Jeferson Daniel
 Author-email: jeferson.daniel412@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -33,29 +33,30 @@
 ```
 
 ### Example Code
 
 ```python
 from bson import ObjectId
 from pydantic import BaseModel
-from pydantic_mongo import AbstractRepository, ObjectIdField
+from pydantic_mongo import AbstractRepository, PydanticObjectId
 from pymongo import MongoClient
-from typing import List
+from typing import Optional, List
 import os
 
 class Foo(BaseModel):
    count: int
    size: float = None
 
 class Bar(BaseModel):
    apple: str = 'x'
    banana: str = 'y'
 
 class Spam(BaseModel):
-   id: ObjectIdField = None
+   # PydanticObjectId is an alias to Annotated[ObjectId, ObjectIdAnnotation]
+   id: Optional[PydanticObjectId] = None
    foo: Foo
    bars: List[Bar]
 
 class SpamRepository(AbstractRepository[Spam]):
    class Meta:
       collection_name = 'spams'
 
@@ -80,15 +81,15 @@
 
 # Delete
 spam_repository.delete(spam)
 
 # Find One By Id
 result = spam_repository.find_one_by_id(spam.id)
 
-# Find One By Id using string if the id attribute is a ObjectIdField
+# Find One By Id using string if the id attribute is a PydanticObjectId
 result = spam_repository.find_one_by_id(ObjectId('611827f2878b88b49ebb69fc'))
 assert result.foo.count == 2
 
 # Find One By Query
 result = spam_repository.find_one_by({'foo.count': 1})
 
 # Find By Query
```

### Comparing `pydantic-mongo-2.2.0/pydantic_mongo.egg-info/SOURCES.txt` & `pydantic_mongo-2.3.0/pydantic_mongo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydantic-mongo-2.2.0/setup.py` & `pydantic_mongo-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `pydantic-mongo-2.2.0/test/test_enhance_meta.py` & `pydantic_mongo-2.3.0/test/test_enhance_meta.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 from pydantic import BaseModel, Field
-
-from pydantic_mongo import AbstractRepository, ObjectIdField
+from pydantic_mongo import AbstractRepository, PydanticObjectId
+from typing_extensions import Optional
 
 
 class HamModel(BaseModel):
-    id: ObjectIdField = Field(default=None)
+    id: Optional[PydanticObjectId]
     name: str
 
 
 class HamRepository(AbstractRepository):
     class Meta:
         collection_name = "ham"
         document_class = HamModel
@@ -27,11 +27,11 @@
 
 def test_repository_with_v2_meta(ham_repo):
     assert not list(ham_repo.find_by({})), "should have no documents in db"
     assert ham_repo.get_collection().name == "ham"
 
 
 def test_save_with_new_repo(clean_ham_collection, ham_repo):
-    m = HamModel(name="wilfred")
+    m = HamModel(id=None, name="wilfred")
     assert m.id is None, "should have no id"
     ham_repo.save(m)
     assert m.id
```

### Comparing `pydantic-mongo-2.2.0/test/test_fields.py` & `pydantic_mongo-2.3.0/test/test_fields.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import pytest
+from typing import Optional
 from bson import ObjectId
 from pydantic import BaseModel, ValidationError
 
 from pydantic_mongo import ObjectIdField
 
 
 class User(BaseModel):
-    id: ObjectIdField = None
+    id: ObjectIdField
 
 
 class TestFields:
     def test_object_id_validation(self):
         with pytest.raises(ValidationError):
             User.model_validate({"id": "lala"})
         User.model_validate({"id": "611827f2878b88b49ebb69fc"})
@@ -22,9 +23,10 @@
 
     def test_modify_schema(self):
         user = User(id=ObjectId("611827f2878b88b49ebb69fc"))
         schema = user.model_json_schema()
         assert {
             "title": "User",
             "type": "object",
-            "properties": {"id": {"default": None, "title": "Id", "type": "string"}},
+            "properties": {"id": {"title": "Id", "type": "string"}},
+            "required": ["id"],
         } == schema
```

### Comparing `pydantic-mongo-2.2.0/test/test_pagination.py` & `pydantic_mongo-2.3.0/test/test_pagination.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-import datetime
-from typing import List
+from typing import List, Optional
 
 from bson import ObjectId
 from pydantic import BaseModel
 
 from pydantic_mongo.pagination import (
     decode_pagination_cursor,
     encode_pagination_cursor,
     get_pagination_cursor_payload,
 )
 
 
 class Foo(BaseModel):
     count: int
-    size: float = None
+    size: Optional[float] = None
 
 
 class Bar(BaseModel):
     apple: str = "x"
     banana: str = "y"
 
 
 class Spam(BaseModel):
-    id: str = None
+    id: Optional[str] = None
     foo: Foo
     bars: List[Bar]
 
 
 class TestPagination:
     def test_get_pagination_cursor_payload(self):
         spam = Spam(id="lala", foo=Foo(count=1, size=1.0), bars=[Bar()])
```

### Comparing `pydantic-mongo-2.2.0/test/test_repository.py` & `pydantic_mongo-2.3.0/test/test_repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from typing import List
+from typing import List, Optional, cast
 
 import mongomock
 import pytest
 from bson import ObjectId
 from pydantic import BaseModel, Field
 
-from pydantic_mongo import AbstractRepository, ObjectIdField
+from pydantic_mongo import AbstractRepository, PydanticObjectId
 from pydantic_mongo.errors import PaginationError
 
 
 class Foo(BaseModel):
     count: int
-    size: float = None
+    size: Optional[float] = None
 
 
 class Bar(BaseModel):
     apple: str = Field(default="x")
     banana: str = Field(default="y")
 
 
 class Spam(BaseModel):
-    id: ObjectIdField = None
-    foo: Foo = None
-    bars: List[Bar] = None
+    id: Optional[PydanticObjectId] = None
+    foo: Optional[Foo] = None
+    bars: Optional[List[Bar]] = None
 
 
 class SpamRepository(AbstractRepository[Spam]):
     class Meta:
         collection_name = "spams"
 
 
@@ -45,15 +45,15 @@
 
         assert {
             "_id": ObjectId(spam.id),
             "foo": {"count": 1, "size": 1.0},
             "bars": [{"apple": "x", "banana": "y"}],
         } == database["spams"].find()[0]
 
-        spam.foo.count = 2
+        cast(Foo, spam.foo).count = 2
         spam_repository.save(spam)
 
         assert {
             "_id": ObjectId(spam.id),
             "foo": {"count": 2, "size": 1.0},
             "bars": [{"apple": "x", "banana": "y"}],
         } == database["spams"].find()[0]
@@ -143,14 +143,16 @@
                 "bars": [{"apple": "x", "banana": "y"}],
             }
         )
 
         spam_repository = SpamRepository(database=database)
         result = spam_repository.find_one_by_id(spam_id)
 
+        assert result is not None
+        assert result.bars is not None
         assert issubclass(Spam, type(result))
         assert spam_id == result.id
         assert "x" == result.bars[0].apple
 
     def test_find_by(self, database):
         database.spams.insert_many(
             [
@@ -167,32 +169,26 @@
 
         spam_repository = SpamRepository(database=database)
 
         # Simple Find
         result = spam_repository.find_by({})
         results = [x for x in result]
         assert 2 == len(results)
+        assert results[0].foo is not None
+        assert results[1].foo is not None
         assert 2 == results[0].foo.count
         assert 3 == results[1].foo.count
 
         # Find with optional parameters
         result = spam_repository.find_by(
             {}, skip=10, limit=10, sort=[("foo.count", 1), ("id", 1)]
         )
         results = [x for x in result]
         assert 0 == len(results)
 
-    def test_invalid_model_class(self, database):
-        class BrokenRepository(AbstractRepository[int]):
-            class Meta:
-                collection_name = "spams"
-
-        with pytest.raises(Exception):
-            BrokenRepository(database=database)
-
     def test_invalid_model_id_field(self, database):
         class NoIdModel(BaseModel):
             something: str
 
         class BrokenRepository(AbstractRepository[NoIdModel]):
             class Meta:
                 collection_name = "spams"
```

