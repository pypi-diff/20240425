# Comparing `tmp/typedmongo-0.0.0.tar.gz` & `tmp/typedmongo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedmongo-0.0.0.tar", last modified: Mon Apr 22 02:20:39 2024, max compression
+gzip compressed data, was "typedmongo-1.0.0.tar", last modified: Thu Apr 25 17:15:45 2024, max compression
```

## Comparing `typedmongo-0.0.0.tar` & `typedmongo-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,25 @@
--rw-r--r--   0        0        0    11357 2024-04-22 02:20:26.106900 typedmongo-0.0.0/LICENSE
--rw-r--r--   0        0        0       13 2024-04-22 02:20:26.106900 typedmongo-0.0.0/README.md
--rw-r--r--   0        0        0     1165 2024-04-22 02:20:39.382876 typedmongo-0.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-22 02:20:26.106900 typedmongo-0.0.0/tests/__init__.py
--rw-r--r--   0        0        0     2693 2024-04-22 02:20:26.110900 typedmongo-0.0.0/tests/test_expressions.py
--rw-r--r--   0        0        0     1516 2024-04-22 02:20:26.110900 typedmongo-0.0.0/tests/test_table.py
--rw-r--r--   0        0        0      473 2024-04-22 02:20:26.110900 typedmongo-0.0.0/typedmongo/__init__.py
--rw-r--r--   0        0        0      473 2024-04-22 02:20:26.110900 typedmongo-0.0.0/typedmongo/asyncio/__init__.py
--rw-r--r--   0        0        0    10520 2024-04-22 02:20:26.110900 typedmongo-0.0.0/typedmongo/asyncio/client.py
--rw-r--r--   0        0        0     7018 2024-04-22 02:20:26.110900 typedmongo-0.0.0/typedmongo/asyncio/fields.py
--rw-r--r--   0        0        0     6316 2024-04-22 02:20:26.110900 typedmongo-0.0.0/typedmongo/asyncio/table.py
--rw-r--r--   0        0        0    10326 2024-04-22 02:20:26.110900 typedmongo-0.0.0/typedmongo/client.py
--rw-r--r--   0        0        0      163 2024-04-22 02:20:26.110900 typedmongo-0.0.0/typedmongo/exceptions.py
--rw-r--r--   0        0        0     5205 2024-04-22 02:20:26.110900 typedmongo-0.0.0/typedmongo/expressions.py
--rw-r--r--   0        0        0     7018 2024-04-22 02:20:26.110900 typedmongo-0.0.0/typedmongo/fields.py
--rw-r--r--   0        0        0     1008 2024-04-22 02:20:26.110900 typedmongo-0.0.0/typedmongo/sync.py
--rw-r--r--   0        0        0     6316 2024-04-22 02:20:26.110900 typedmongo-0.0.0/typedmongo/table.py
--rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 typedmongo-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-25 17:15:33.191543 typedmongo-1.0.0/LICENSE
+-rw-r--r--   0        0        0      108 2024-04-25 17:15:33.191543 typedmongo-1.0.0/README.md
+-rw-r--r--   0        0        0     1441 2024-04-25 17:15:45.719857 typedmongo-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-25 17:15:33.191543 typedmongo-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 17:15:33.191543 typedmongo-1.0.0/tests/asyncio/__init__.py
+-rw-r--r--   0        0        0     5347 2024-04-25 17:15:33.191543 typedmongo-1.0.0/tests/asyncio/test_client.py
+-rw-r--r--   0        0        0     2777 2024-04-25 17:15:33.191543 typedmongo-1.0.0/tests/asyncio/test_table.py
+-rw-r--r--   0        0        0     1218 2024-04-25 17:15:33.191543 typedmongo-1.0.0/tests/sync.py
+-rw-r--r--   0        0        0     5119 2024-04-25 17:15:33.191543 typedmongo-1.0.0/tests/test_client.py
+-rw-r--r--   0        0        0     2930 2024-04-25 17:15:33.191543 typedmongo-1.0.0/tests/test_expressions.py
+-rw-r--r--   0        0        0      582 2024-04-25 17:15:33.191543 typedmongo-1.0.0/tests/test_marshamallow.py
+-rw-r--r--   0        0        0     2769 2024-04-25 17:15:33.191543 typedmongo-1.0.0/tests/test_table.py
+-rw-r--r--   0        0        0      749 2024-04-25 17:15:33.191543 typedmongo-1.0.0/typedmongo/__init__.py
+-rw-r--r--   0        0        0      749 2024-04-25 17:15:33.191543 typedmongo-1.0.0/typedmongo/asyncio/__init__.py
+-rw-r--r--   0        0        0    11778 2024-04-25 17:15:33.191543 typedmongo-1.0.0/typedmongo/asyncio/client.py
+-rw-r--r--   0        0        0     8629 2024-04-25 17:15:33.191543 typedmongo-1.0.0/typedmongo/asyncio/fields.py
+-rw-r--r--   0        0        0     6954 2024-04-25 17:15:33.191543 typedmongo-1.0.0/typedmongo/asyncio/table.py
+-rw-r--r--   0        0        0    11560 2024-04-25 17:15:33.191543 typedmongo-1.0.0/typedmongo/client.py
+-rw-r--r--   0        0        0      163 2024-04-25 17:15:33.191543 typedmongo-1.0.0/typedmongo/exceptions.py
+-rw-r--r--   0        0        0     5452 2024-04-25 17:15:33.191543 typedmongo-1.0.0/typedmongo/expressions.py
+-rw-r--r--   0        0        0     8629 2024-04-25 17:15:33.191543 typedmongo-1.0.0/typedmongo/fields.py
+-rw-r--r--   0        0        0      351 2024-04-25 17:15:33.191543 typedmongo-1.0.0/typedmongo/marshamallow.py
+-rw-r--r--   0        0        0     1325 2024-04-25 17:15:33.191543 typedmongo-1.0.0/typedmongo/sync.py
+-rw-r--r--   0        0        0     6948 2024-04-25 17:15:33.195543 typedmongo-1.0.0/typedmongo/table.py
+-rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 typedmongo-1.0.0/PKG-INFO
```

### Comparing `typedmongo-0.0.0/LICENSE` & `typedmongo-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typedmongo-0.0.0/pyproject.toml` & `typedmongo-1.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [project]
 name = "typedmongo"
-version = "0.0.0"
-description = "A modern Python MongoDB ODM"
+version = "1.0.0"
+description = "A production-ready modern Python MongoDB ODM"
 authors = [
     { name = "abersheeran", email = "me@abersheeran.com" },
 ]
 dependencies = [
     "pymongo>=4.6.3",
     "motor>=3.4.0",
     "marshmallow>=3.21.1",
+    "typing-extensions>=4.11.0",
 ]
-requires-python = ">=3.12"
+requires-python = ">=3.10"
 readme = "README.md"
 
 [project.license]
 text = "Apache2.0"
 
 [build-system]
 requires = [
@@ -25,51 +26,59 @@
 [tool.pdm]
 package-type = "library"
 
 [tool.pdm.dev-dependencies]
 test = [
     "pytest>=8.1.1",
     "pytest-cov>=5.0.0",
+    "pytest-asyncio>=0.23.6",
+]
+dev = [
+    "ruff>=0.4.1",
 ]
 
 [tool.pdm.scripts]
 format = "ruff format ."
-lint = "ruff ."
-test = "pytest --cov=typedmongo tests/"
+lint = "ruff check ."
+pre_test = "python tests/sync.py"
+test = "pytest --cov=typedmongo --asyncio-mode=auto tests/"
+sync = "python typedmongo/sync.py"
 
 [tool.ruff]
-extend-select = [
-    "I",
-]
 exclude = [
     "typedmongo/client.py",
+    "typedmongo/fields.py",
+    "typedmongo/table.py",
 ]
 
 [tool.ruff.lint]
 ignore = [
     "E731",
 ]
-
-[tool.coverage]
-ignores = [
-    "raise NotImplementedError",
+extend-select = [
+    "I",
 ]
 
 [tool.coverage.run]
 omit = [
     "*/.venv/*",
     "*/tests/*",
 ]
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
+    "case _:",
+    "return NotImplemented",
     "raise NotImplementedError",
     "if False:",
     "assert False",
     "if typing.TYPE_CHECKING:",
     "if TYPE_CHECKING:",
     "pass",
     "\\.\\.\\.",
 ]
 show_missing = true
 skip_covered = true
+omit = [
+    "typedmongo/sync.py",
+]
```

### Comparing `typedmongo-0.0.0/tests/test_expressions.py` & `typedmongo-1.0.0/tests/test_expressions.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,11 +80,19 @@
                     "OR",
                     NotExpression(CompareExpression(field, ">", 18)),
                     NotExpression(CompareExpression(field, "<", 35)),
                 ),
                 NotExpression(CompareExpression(field, "==", 35)),
             ),
         ),
+        (
+            ~~((field > 18) & (field < 35)),
+            CombineExpression(
+                "AND",
+                CompareExpression(field, ">", 18),
+                CompareExpression(field, "<", 35),
+            ),
+        ),
     ],
 )
 def test_compile_expressions(expression, expected):
     assert expression == expected
```

### Comparing `typedmongo-0.0.0/typedmongo/asyncio/client.py` & `typedmongo-1.0.0/typedmongo/asyncio/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 from __future__ import annotations
 
 import dataclasses
+import decimal
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncIterable,
+    Generic,
     Mapping,
     NoReturn,
     Optional,
+    TypeAlias,
+    TypeVar,
     overload,
 )
 
+from bson.codec_options import CodecOptions, TypeCodec, TypeRegistry
+from bson.decimal128 import Decimal128
 from pymongo.operations import DeleteMany as MongoDeleteMany
 from pymongo.operations import DeleteOne as MongoDeleteOne
 from pymongo.operations import InsertOne as MongoInsertOne
 from pymongo.operations import ReplaceOne as MongoReplaceOne
 from pymongo.operations import UpdateMany as MongoUpdateMany
 from pymongo.operations import UpdateOne as MongoUpdateOne
 
@@ -26,39 +32,63 @@
     from pymongo.results import UpdateResult as MongoUpdateResult
 
     from .table import Table
 
 from typedmongo.expressions import Expression, OrderBy, compile_expression
 from typedmongo.fields import Field
 
+DocumentId: TypeAlias = Any
+T = TypeVar("T", bound="Table")
 
-def initial_collections(db: MongoDatabase, *tables: type[Table]) -> None:
+
+class DecimalCodec(TypeCodec):
+    python_type = decimal.Decimal  # type: ignore
+    bson_type = Decimal128  # type: ignore
+
+    def transform_python(self, value: decimal.Decimal) -> Decimal128:
+        """Function that transforms a custom type value into a type
+        that BSON can encode."""
+        return Decimal128(value)
+
+    def transform_bson(self, value: Decimal128) -> decimal.Decimal:
+        """Function that transforms a vanilla BSON type value into our
+        custom type."""
+        return value.to_decimal()
+
+
+async def initial_collections(db: MongoDatabase, *tables: type[Table]) -> None:
     for table in tables:
         table.__lazy_init_fields__()
         table.__database__ = db
-        table.__collection__ = db[table.__collection_name__]
+        type_registry = TypeRegistry([DecimalCodec()])
+        codec_options = CodecOptions(type_registry=type_registry)
+        table.__collection__ = collection = db.get_collection(
+            table.__collection_name__, codec_options=codec_options
+        )
+        indexes = table.indexes()
+        if indexes:
+            await collection.create_indexes(
+                [index.to_index_model() for index in indexes]
+            )
 
 
 class Manager:
     @overload
-    def __get__[T: Table](self, instance: None, cls: type[T]) -> Objects[T]:
-        ...
+    def __get__(self, instance: None, cls: type[T]) -> Objects[T]: ...
 
     @overload
-    def __get__[T: Table](self, instance: T, cls: type[T]) -> NoReturn:
-        ...
+    def __get__(self, instance: T, cls: type[T]) -> NoReturn: ...
 
     def __get__(self, instance, cls):
         if instance is None:
             return Objects(cls)
 
         raise AttributeError("Manager is not accessible via instance")
 
 
-type DocumentId = Any
 translate_filter = (
     lambda f: {}
     if f is None
     else (compile_expression(f) if isinstance(f, Expression) else f)
 )
 translate_projection = (
     lambda p: None
@@ -72,15 +102,15 @@
 translate_sort = (
     lambda s: None
     if s is None
     else [(order_by.field.field_name, order_by.order) for order_by in s]
 )
 
 
-class Objects[T: Table]:
+class Objects(Generic[T]):
     def __init__(self, table: type[T]) -> None:
         self.table = table
 
     async def insert_one(self, document: T) -> DocumentId:
         # Just for IDE display method docs
         collection: MongoCollection = self.table.__collection__
 
@@ -275,14 +305,20 @@
         # Just for IDE display method docs
         collection: MongoCollection = self.table.__collection__
 
         return await collection.bulk_write(
             [r.to_mongo() for r in requests], ordered=ordered
         )
 
+    async def drop(self) -> None:
+        # Just for IDE display method docs
+        collection: MongoCollection = self.table.__collection__
+
+        await collection.drop()
+
 
 @dataclasses.dataclass
 class DeleteMany:
     filter: Expression | dict[Any, Any]
 
     def to_mongo(self) -> MongoDeleteMany:
         return MongoDeleteMany(translate_filter(self.filter))
@@ -293,23 +329,23 @@
     filter: Expression | dict[Any, Any]
 
     def to_mongo(self) -> MongoDeleteOne:
         return MongoDeleteOne(translate_filter(self.filter))
 
 
 @dataclasses.dataclass
-class InsertOne[T: Table]:
+class InsertOne(Generic[T]):
     document: T
 
     def to_mongo(self) -> MongoInsertOne:
         return MongoInsertOne(self.document.to_mongo())
 
 
 @dataclasses.dataclass
-class ReplaceOne[T: Table]:
+class ReplaceOne(Generic[T]):
     filter: Expression | dict[Any, Any]
     replacement: T
 
     def to_mongo(self) -> MongoReplaceOne:
         return MongoReplaceOne(
             translate_filter(self.filter), self.replacement.to_mongo()
         )
```

### Comparing `typedmongo-0.0.0/typedmongo/asyncio/fields.py` & `typedmongo-1.0.0/typedmongo/asyncio/fields.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,79 @@
 from __future__ import annotations
 
 import dataclasses
+import decimal
 from datetime import datetime
-from typing import TYPE_CHECKING, Any, Self, get_args, get_origin, overload
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Generic,
+    Optional,
+    TypeVar,
+    get_args,
+    get_origin,
+    overload,
+)
 
 from bson import ObjectId
-from bson.errors import InvalidId
-from marshmallow import ValidationError, fields
+from marshmallow import fields
+from typing_extensions import Self
 
 from typedmongo.expressions import CompareMixin, HasFieldName, OrderByMixin
+from typedmongo.marshamallow import MarshamallowObjectId
 
 if TYPE_CHECKING:
     from .table import Table
 
+A = TypeVar("A")
+TypeTable = TypeVar("TypeTable", bound=type["Table"])
+T = TypeVar("T", bound="Table")
+TypeTableOrAny = TypeVar("TypeTableOrAny", bound=type["Table"] | Any)
+FieldType = TypeVar("FieldType")
+
+
+@dataclasses.dataclass
+class FieldParamters(Generic[FieldType]):
+    default: Optional[FieldType | Callable[[], FieldType]] = dataclasses.field(
+        default=None, kw_only=True
+    )
+
 
 @dataclasses.dataclass(eq=False)
-class Field[FieldType](OrderByMixin, CompareMixin):
+class Field(Generic[FieldType], OrderByMixin, CompareMixin):
     """
     Field
     """
 
+    default: Optional[FieldType | Callable[[], FieldType]] = dataclasses.field(
+        default=None, kw_only=True
+    )
     field_name: str = dataclasses.field(init=False)
     marshamallow: fields.Field = dataclasses.field(init=False)
 
     def __set_name__(self, owner: type[Table], name: str) -> None:
         self._table = owner
         self._name = name
 
         self.field_name = name
 
         if not hasattr(self, "marshamallow"):
             self.marshamallow = fields.Field(required=True)
 
+        if self.default is not None:
+            # https://github.com/marshmallow-code/marshmallow/issues/2151
+            self.marshamallow.required = False
+            self.marshamallow.load_default = self.default
+
     @overload
-    def __get__(self: Self, instance: None, cls: type) -> Self:
-        ...
+    def __get__(self: Self, instance: None, cls: type) -> Self: ...
 
     @overload
-    def __get__(self: Self, instance: object, cls: type) -> FieldType:
-        ...
+    def __get__(self: Self, instance: object, cls: type) -> FieldType: ...
 
     def __get__(self, instance, cls):
         if instance is None:  # Call from class
             return self
 
         try:
             return instance.__dict__[self._name]
@@ -70,36 +101,25 @@
                 cls.__field_type__ = generic_type = get_args(origin_base)[0]
                 return generic_type
         raise RuntimeError(f"Cannot get field type for {cls}")
 
     def load(self, value: Any, *, partial: bool = False) -> FieldType:
         return value
 
-    def to_mongo(self, value: FieldType) -> Any:
+    def dump(self, value: FieldType) -> Any:
         return value
 
 
-class _ObjectIdField(fields.Field):
-    def _serialize(self, value: ObjectId, attr, obj, **kwargs):
-        return str(value)
-
-    def _deserialize(self, value: str, attr, data, **kwargs):
-        try:
-            return ObjectId(value)
-        except (InvalidId, TypeError):
-            raise ValidationError("Invalid ObjectId.")
-
-
 @dataclasses.dataclass(eq=False)
 class ObjectIdField(Field[ObjectId]):
     """
     ObjectId field
     """
 
-    marshamallow: fields.Field = _ObjectIdField(required=True)
+    marshamallow: fields.Field = MarshamallowObjectId(required=True)
 
 
 @dataclasses.dataclass(eq=False)
 class StringField(Field[str]):
     """
     String field
     """
@@ -139,21 +159,29 @@
     """
     DateTime field
     """
 
     marshamallow: fields.Field = fields.DateTime(required=True)
 
 
+@dataclasses.dataclass(eq=False)
+class DecimalField(Field[decimal.Decimal]):
+    """
+    Decimal field
+    """
+
+    marshamallow: fields.Field = fields.Decimal(required=True)
+
+
 @dataclasses.dataclass
-class FieldNameProxy[T: type[Table]]:
+class FieldNameProxy(Generic[TypeTable]):
     prefix: HasFieldName
-    t: T
+    t: TypeTable
 
-    def __get__(self, instance, owner) -> T:
-        ...
+    def __get__(self, instance, owner) -> TypeTable: ...
 
     def __getattr__(self, name: str) -> FieldNameProxyString:
         try:
             return FieldNameProxyString(
                 f"{self.prefix.field_name}.{self.t.__fields__[name].field_name}"
             )
         except KeyError:
@@ -163,91 +191,112 @@
 
 @dataclasses.dataclass(eq=False)
 class FieldNameProxyString(OrderByMixin, CompareMixin):
     field_name: str
 
 
 @dataclasses.dataclass(eq=False)
-class EmbeddedField[T: Table](Field[T]):
+class EmbeddedField(Generic[T], Field[T]):
     """
     Embedded field
     """
 
     _: FieldNameProxy[type[T]] = dataclasses.field(init=False)
 
     schema: type[T]
 
     def __post_init__(self):
         self._ = FieldNameProxy(self, self.schema)
-        self.marshamallow = fields.Nested(self.schema.__schema__)
+        self.marshamallow = fields.Nested(lambda: self.schema.__schema__)
 
         def load(value: Any, *, partial: bool = False) -> T:
             return self.schema.load(value, partial=partial)
 
+        def dump(value: T) -> dict[str, Any]:
+            return self.schema.dump(value)
+
         self.load = load
+        self.dump = dump
+
+    def __set_name__(self, owner: type[Table], name: str) -> None:
+        if not issubclass(self.schema, owner):
+            self.schema.__lazy_init_fields__()
+        return super().__set_name__(owner, name)
 
 
 @dataclasses.dataclass(eq=False)
-class ListFieldNameProxy[T: type[Table] | Any](OrderByMixin, CompareMixin):
+class ListFieldNameProxy(Generic[TypeTableOrAny], OrderByMixin, CompareMixin):
     number: int | None
     prefix: HasFieldName
-    t: T
+    t: TypeTableOrAny
 
     @property
     def field_name(self) -> str:
         if self.number is None:
             return self.prefix.field_name
         return f"{self.prefix.field_name}.{self.number}"
 
-    def __get__(self, instance, owner) -> T:
-        ...
+    def __get__(self, instance, owner) -> TypeTableOrAny: ...
 
     def __getattr__(self, name: str) -> FieldNameProxyString:
         try:
             return FieldNameProxyString(
                 f"{self.field_name}.{self.t.__fields__[name].field_name}"
             )
         except KeyError:
             message = "{0} has no attribute '{1}'".format(self.t, name)
             raise AttributeError(message) from None
 
 
 @dataclasses.dataclass(eq=False)
-class ListField[T](Field[list[T]]):
+class ListField(Generic[A], Field[list[A]]):
     """
     List field
     """
 
-    _: ListFieldNameProxy[type[T]] = dataclasses.field(init=False)
+    _: ListFieldNameProxy[type[A]] = dataclasses.field(init=False)
 
-    type_or_schema: type[T]
+    type_or_schema: type[A]
 
-    def __getitem__(self, index: int) -> type[T]:
+    def __getitem__(self, index: int) -> type[A]:
         return ListFieldNameProxy(index, self, self.type_or_schema)  # type: ignore
 
     def __post_init__(self):
         self._ = ListFieldNameProxy(None, self, self.type_or_schema)
 
         from .table import Table
 
         if issubclass(self.type_or_schema, Table):
             self.marshamallow = fields.List(
-                fields.Nested(self.type_or_schema.__schema__)
+                fields.Nested(lambda: self.type_or_schema.__schema__)  # type: ignore
             )
 
-            def load(value: Any, *, partial: bool = False) -> list[T]:
+            def load(value: Any, *, partial: bool = False) -> list[A]:
                 return [
                     self.type_or_schema.load(item, partial=partial)  # type: ignore
                     for item in value
                 ]
 
+            def dump(value: list[A]) -> list[dict[str, Any]]:
+                return [self.type_or_schema.dump(item) for item in value]  # type: ignore
+
             self.load = load
+            self.dump = dump
         else:
             self.marshamallow = fields.List(
                 {
                     int: fields.Integer(required=True),
                     float: fields.Float(required=True),
                     bool: fields.Boolean(required=True),
                     str: fields.String(required=True),
                     datetime: fields.DateTime(required=True),
                 }[self.type_or_schema]  # type: ignore
             )
+
+    def __set_name__(self, owner: type[Table], name: str) -> None:
+        from .table import Table
+
+        if issubclass(self.type_or_schema, Table) and not issubclass(
+            self.type_or_schema, owner
+        ):
+            self.type_or_schema.__lazy_init_fields__()
+        return super().__set_name__(owner, name)
```

### Comparing `typedmongo-0.0.0/typedmongo/asyncio/table.py` & `typedmongo-1.0.0/typedmongo/table.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,42 +3,46 @@
 from functools import reduce
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Mapping,
     Optional,
-    Self,
     Sequence,
     get_args,
     get_origin,
 )
 
 from marshmallow import Schema
 from pymongo import IndexModel
+from typing_extensions import Self, dataclass_transform
 
 from typedmongo.exceptions import TableDefineError
 
 from .client import Manager
-from .fields import Field, ObjectIdField
+from .fields import Field
 
 
 def snake_case(name: str) -> str:
     """
     convert "SomeWords" to "some_words"
     """
     return "".join(
         "_" + char.lower() if char.isupper() and i > 0 else char.lower()
         for i, char in enumerate(name)
     )
 
 
 @dataclasses.dataclass
 class Index:
-    keys: Field | Sequence[tuple[Field, int]] | Mapping[Field, Any]
+    keys: (
+        Field
+        | Sequence[tuple[Field, int | str | Mapping[str, Any]]]
+        | Mapping[Field, Any]
+    )
 
     name: Optional[str] = None
     unique: bool = False
     background: bool = False
     sparse: bool = False
     expireAfterSeconds: Optional[int] = None
     partialFilterExpression: Optional[dict[str, Any]] = None
@@ -58,22 +62,25 @@
             background=self.background,
             sparse=self.sparse,
             expireAfterSeconds=self.expireAfterSeconds,
             partialFilterExpression=self.partialFilterExpression,
         )
 
 
+@dataclass_transform(eq_default=False, kw_only_default=True)
 class TableMetaClass(type):
     if TYPE_CHECKING:
         __abstract__: bool
         __database__: Any
         __collection_name__: str
         __collection__: Any
-        __fields__: dict[str, Field]
+        __pfields__: dict[str, Field]
+        __sfields__: dict[str, Field]
         __fields_loaded__: bool
+        __fields__: dict[str, Field]
         __create_schema__: Callable[[str, dict[str, Field]], Schema]
         __schema__: Schema
 
     def __new__(cls, name, bases, namespace):
         if "_" in name:  # check error name. e.g. Status_Info
             raise TableDefineError(
                 "Table class name cannot have '_': {name}".format(name=name)
@@ -83,59 +90,69 @@
                 "Table class name must be upper letter in start: {name}".format(
                     name=name
                 )
             )
         namespace.setdefault("__collection_name__", snake_case(name))
         namespace.setdefault("__abstract__", False)
 
-        # merge bases' `__fields__` to `__fields__`
-        fields = {
+        if "__fields__" in namespace:  # Clear __fields__ to avoid conflict
+            del namespace["__fields__"]
+        namespace["__fields_loaded__"] = False
+
+        namespace["__sfields__"] = {
             name: value for name, value in namespace.items() if isinstance(value, Field)
         }
-        namespace["__fields_loaded__"] = not not fields
-        namespace["__fields__"] = reduce(
+        # merge bases' `__fields__` to `__pfields__`
+        namespace["__pfields__"] = reduce(
             lambda _initial, _item: {**_item, **_initial},
-            reversed([getattr(base, "__fields__", {}) for base in bases]),
-            fields,
+            reversed(
+                [
+                    base.__lazy_init_fields__()
+                    for base in bases
+                    if isinstance(base, TableMetaClass)
+                ]
+            ),
+            {},
         )
 
         if "__create_schema__" not in namespace:
             for base in bases:
                 create_schema = base.__create_schema__
             namespace["__create_schema__"] = create_schema
-        namespace["__schema__"] = namespace["__create_schema__"](
-            name, namespace["__fields__"]
-        )
 
         return super().__new__(cls, name, bases, namespace)
 
-    def __lazy_init_fields__(cls) -> None:
+    def __lazy_init_fields__(cls) -> dict[str, Field]:
         if cls.__fields_loaded__:
-            return
+            return cls.__fields__
 
         fields = {
             **{
                 name: value()
                 for name, value in inspect.get_annotations(cls, eval_str=True).items()
                 if isinstance(value, type) and issubclass(value, Field)
             },
             **{
                 name: origin_class(*get_args(value))
                 for name, value in inspect.get_annotations(cls, eval_str=True).items()
                 if (origin_class := get_origin(value))
                 and isinstance(origin_class, type)
                 and issubclass(origin_class, Field)
             },
+            **cls.__sfields__,
         }
+        cls.__fields__ = {**cls.__pfields__, **fields}
+        cls.__fields_loaded__ = True
+
         for name, field in fields.items():
             setattr(cls, name, field)
             field.__set_name__(cls, name)
-        cls.__fields_loaded__ = True
-        cls.__fields__ = {**cls.__fields__, **fields}
-        cls.__schema__ = cls.__create_schema__(cls.__name__, fields)
+
+        cls.__schema__ = cls.__create_schema__(cls.__name__, cls.__fields__)
+        return fields
 
     def __call__(cls, **kwargs: Any):
         instance = super().__call__()
 
         if instance.__abstract__:
             raise RuntimeError(
                 "The class {} cannot be instantiated, because it's __abstract__ is True.".format(
@@ -153,17 +170,15 @@
             raise AttributeError(
                 "Can't modify the `__abstract__` attribute dynamically."
             )
         return super().__setattr__(name, value)
 
 
 class Table(metaclass=TableMetaClass):
-    __abstract__: bool = True
-
-    _id = ObjectIdField()
+    __abstract__ = True
 
     objects = Manager()
 
     def __repr__(self) -> str:
         return "{class_name}({fields})".format(
             class_name=self.__class__.__name__,
             fields=", ".join(
@@ -187,13 +202,21 @@
         validated = cls.__schema__.load(data=data, partial=partial)
         loaded = {
             key: getattr(cls.__fields__[key], "load")(value, partial=partial)
             for key, value in validated.items()  # type: ignore
         }
         return cls(**loaded)
 
-    def to_mongo(self) -> dict[str, Any]:
-        return {
-            key: getattr(self.__fields__[key], "to_mongo")(value)
-            for key, value in self.__dict__.items()
-            if key in self.__fields__
+    @classmethod
+    def dump(cls, instance: Self) -> dict[str, Any]:
+        dumped = {
+            key: getattr(instance.__fields__[key], "dump")(value)
+            for key, value in instance.__dict__.items()
         }
+        return cls.__schema__.dump(dumped)  # type: ignore
+
+    @classmethod
+    def indexes(cls) -> list[Index]:
+        return []
+
+    def to_mongo(self) -> dict[str, Any]:
+        return self.dump(self)
```

### Comparing `typedmongo-0.0.0/typedmongo/client.py` & `typedmongo-1.0.0/typedmongo/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 from __future__ import annotations
 
 import dataclasses
+import decimal
 from typing import (
     TYPE_CHECKING,
     Any,
     Iterable,
+    Generic,
     Mapping,
     NoReturn,
     Optional,
+    TypeAlias,
+    TypeVar,
     overload,
 )
 
+from bson.codec_options import CodecOptions, TypeCodec, TypeRegistry
+from bson.decimal128 import Decimal128
 from pymongo.operations import DeleteMany as MongoDeleteMany
 from pymongo.operations import DeleteOne as MongoDeleteOne
 from pymongo.operations import InsertOne as MongoInsertOne
 from pymongo.operations import ReplaceOne as MongoReplaceOne
 from pymongo.operations import UpdateMany as MongoUpdateMany
 from pymongo.operations import UpdateOne as MongoUpdateOne
 
@@ -26,39 +32,63 @@
     from pymongo.results import UpdateResult as MongoUpdateResult
 
     from .table import Table
 
 from typedmongo.expressions import Expression, OrderBy, compile_expression
 from typedmongo.fields import Field
 
+DocumentId: TypeAlias = Any
+T = TypeVar("T", bound="Table")
+
+
+class DecimalCodec(TypeCodec):
+    python_type = decimal.Decimal  # type: ignore
+    bson_type = Decimal128  # type: ignore
+
+    def transform_python(self, value: decimal.Decimal) -> Decimal128:
+        """Function that transforms a custom type value into a type
+        that BSON can encode."""
+        return Decimal128(value)
+
+    def transform_bson(self, value: Decimal128) -> decimal.Decimal:
+        """Function that transforms a vanilla BSON type value into our
+        custom type."""
+        return value.to_decimal()
+
 
 def initial_collections(db: MongoDatabase, *tables: type[Table]) -> None:
     for table in tables:
         table.__lazy_init_fields__()
         table.__database__ = db
-        table.__collection__ = db[table.__collection_name__]
+        type_registry = TypeRegistry([DecimalCodec()])
+        codec_options = CodecOptions(type_registry=type_registry)
+        table.__collection__ = collection = db.get_collection(
+            table.__collection_name__, codec_options=codec_options
+        )
+        indexes = table.indexes()
+        if indexes:
+            collection.create_indexes(
+                [index.to_index_model() for index in indexes]
+            )
 
 
 class Manager:
     @overload
-    def __get__[T: Table](self, instance: None, cls: type[T]) -> Objects[T]:
-        ...
+    def __get__(self, instance: None, cls: type[T]) -> Objects[T]: ...
 
     @overload
-    def __get__[T: Table](self, instance: T, cls: type[T]) -> NoReturn:
-        ...
+    def __get__(self, instance: T, cls: type[T]) -> NoReturn: ...
 
     def __get__(self, instance, cls):
         if instance is None:
             return Objects(cls)
 
         raise AttributeError("Manager is not accessible via instance")
 
 
-type DocumentId = Any
 translate_filter = (
     lambda f: {}
     if f is None
     else (compile_expression(f) if isinstance(f, Expression) else f)
 )
 translate_projection = (
     lambda p: None
@@ -72,15 +102,15 @@
 translate_sort = (
     lambda s: None
     if s is None
     else [(order_by.field.field_name, order_by.order) for order_by in s]
 )
 
 
-class Objects[T: Table]:
+class Objects(Generic[T]):
     def __init__(self, table: type[T]) -> None:
         self.table = table
 
     def insert_one(self, document: T) -> DocumentId:
         # Just for IDE display method docs
         collection: MongoCollection = self.table.__collection__
 
@@ -275,14 +305,20 @@
         # Just for IDE display method docs
         collection: MongoCollection = self.table.__collection__
 
         return collection.bulk_write(
             [r.to_mongo() for r in requests], ordered=ordered
         )
 
+    def drop(self) -> None:
+        # Just for IDE display method docs
+        collection: MongoCollection = self.table.__collection__
+
+        collection.drop()
+
 
 @dataclasses.dataclass
 class DeleteMany:
     filter: Expression | dict[Any, Any]
 
     def to_mongo(self) -> MongoDeleteMany:
         return MongoDeleteMany(translate_filter(self.filter))
@@ -293,23 +329,23 @@
     filter: Expression | dict[Any, Any]
 
     def to_mongo(self) -> MongoDeleteOne:
         return MongoDeleteOne(translate_filter(self.filter))
 
 
 @dataclasses.dataclass
-class InsertOne[T: Table]:
+class InsertOne(Generic[T]):
     document: T
 
     def to_mongo(self) -> MongoInsertOne:
         return MongoInsertOne(self.document.to_mongo())
 
 
 @dataclasses.dataclass
-class ReplaceOne[T: Table]:
+class ReplaceOne(Generic[T]):
     filter: Expression | dict[Any, Any]
     replacement: T
 
     def to_mongo(self) -> MongoReplaceOne:
         return MongoReplaceOne(
             translate_filter(self.filter), self.replacement.to_mongo()
         )
```

### Comparing `typedmongo-0.0.0/typedmongo/expressions.py` & `typedmongo-1.0.0/typedmongo/expressions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from __future__ import annotations
 
 import dataclasses
-from typing import Any, Literal, Protocol
+from typing import TYPE_CHECKING, Any, Literal, Protocol
 
+if TYPE_CHECKING:
+    # Solve TypeError: Cannot create a consistent method resolution
+    class HasFieldName(Protocol):
+        field_name: str
+else:
 
-class HasFieldName(Protocol):
-    field_name: str
+    class HasFieldName:
+        field_name: str
 
 
 class Expression:
     """
     Base class for all expressions.
     """
 
@@ -33,37 +38,39 @@
         """
         self & other
         """
         if not isinstance(other, Expression):
             return NotImplemented
         return CombineExpression("AND", self, other)
 
-    def __rand__(self, other: Expression) -> CombineExpression:
-        """
-        other & self
-        """
-        if not isinstance(other, Expression):
-            return NotImplemented
-        return CombineExpression("AND", other, self)
+    # Should we support it?
+    # def __rand__(self, other: Expression) -> CombineExpression:
+    #     """
+    #     other & self
+    #     """
+    #     if not isinstance(other, Expression):
+    #         return NotImplemented
+    #     return CombineExpression("AND", other, self)
 
     def __or__(self, other: Expression) -> CombineExpression:
         """
         self | other
         """
         if not isinstance(other, Expression):
             return NotImplemented
         return CombineExpression("OR", self, other)
 
-    def __ror__(self, other: Expression) -> CombineExpression:
-        """
-        other | self
-        """
-        if not isinstance(other, Expression):
-            return NotImplemented
-        return CombineExpression("OR", other, self)
+    # Should we support it?
+    # def __ror__(self, other: Expression) -> CombineExpression:
+    #     """
+    #     other | self
+    #     """
+    #     if not isinstance(other, Expression):
+    #         return NotImplemented
+    #     return CombineExpression("OR", other, self)
 
 
 class CompareMixin(HasFieldName):
     def __eq__(self, other: Any) -> CompareExpression:
         """
         self == other
         """
```

### Comparing `typedmongo-0.0.0/typedmongo/fields.py` & `typedmongo-1.0.0/typedmongo/fields.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,79 @@
 from __future__ import annotations
 
 import dataclasses
+import decimal
 from datetime import datetime
-from typing import TYPE_CHECKING, Any, Self, get_args, get_origin, overload
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Generic,
+    Optional,
+    TypeVar,
+    get_args,
+    get_origin,
+    overload,
+)
 
 from bson import ObjectId
-from bson.errors import InvalidId
-from marshmallow import ValidationError, fields
+from marshmallow import fields
+from typing_extensions import Self
 
 from typedmongo.expressions import CompareMixin, HasFieldName, OrderByMixin
+from typedmongo.marshamallow import MarshamallowObjectId
 
 if TYPE_CHECKING:
     from .table import Table
 
+A = TypeVar("A")
+TypeTable = TypeVar("TypeTable", bound=type["Table"])
+T = TypeVar("T", bound="Table")
+TypeTableOrAny = TypeVar("TypeTableOrAny", bound=type["Table"] | Any)
+FieldType = TypeVar("FieldType")
+
+
+@dataclasses.dataclass
+class FieldParamters(Generic[FieldType]):
+    default: Optional[FieldType | Callable[[], FieldType]] = dataclasses.field(
+        default=None, kw_only=True
+    )
+
 
 @dataclasses.dataclass(eq=False)
-class Field[FieldType](OrderByMixin, CompareMixin):
+class Field(Generic[FieldType], OrderByMixin, CompareMixin):
     """
     Field
     """
 
+    default: Optional[FieldType | Callable[[], FieldType]] = dataclasses.field(
+        default=None, kw_only=True
+    )
     field_name: str = dataclasses.field(init=False)
     marshamallow: fields.Field = dataclasses.field(init=False)
 
     def __set_name__(self, owner: type[Table], name: str) -> None:
         self._table = owner
         self._name = name
 
         self.field_name = name
 
         if not hasattr(self, "marshamallow"):
             self.marshamallow = fields.Field(required=True)
 
+        if self.default is not None:
+            # https://github.com/marshmallow-code/marshmallow/issues/2151
+            self.marshamallow.required = False
+            self.marshamallow.load_default = self.default
+
     @overload
-    def __get__(self: Self, instance: None, cls: type) -> Self:
-        ...
+    def __get__(self: Self, instance: None, cls: type) -> Self: ...
 
     @overload
-    def __get__(self: Self, instance: object, cls: type) -> FieldType:
-        ...
+    def __get__(self: Self, instance: object, cls: type) -> FieldType: ...
 
     def __get__(self, instance, cls):
         if instance is None:  # Call from class
             return self
 
         try:
             return instance.__dict__[self._name]
@@ -70,36 +101,25 @@
                 cls.__field_type__ = generic_type = get_args(origin_base)[0]
                 return generic_type
         raise RuntimeError(f"Cannot get field type for {cls}")
 
     def load(self, value: Any, *, partial: bool = False) -> FieldType:
         return value
 
-    def to_mongo(self, value: FieldType) -> Any:
+    def dump(self, value: FieldType) -> Any:
         return value
 
 
-class _ObjectIdField(fields.Field):
-    def _serialize(self, value: ObjectId, attr, obj, **kwargs):
-        return str(value)
-
-    def _deserialize(self, value: str, attr, data, **kwargs):
-        try:
-            return ObjectId(value)
-        except (InvalidId, TypeError):
-            raise ValidationError("Invalid ObjectId.")
-
-
 @dataclasses.dataclass(eq=False)
 class ObjectIdField(Field[ObjectId]):
     """
     ObjectId field
     """
 
-    marshamallow: fields.Field = _ObjectIdField(required=True)
+    marshamallow: fields.Field = MarshamallowObjectId(required=True)
 
 
 @dataclasses.dataclass(eq=False)
 class StringField(Field[str]):
     """
     String field
     """
@@ -139,21 +159,29 @@
     """
     DateTime field
     """
 
     marshamallow: fields.Field = fields.DateTime(required=True)
 
 
+@dataclasses.dataclass(eq=False)
+class DecimalField(Field[decimal.Decimal]):
+    """
+    Decimal field
+    """
+
+    marshamallow: fields.Field = fields.Decimal(required=True)
+
+
 @dataclasses.dataclass
-class FieldNameProxy[T: type[Table]]:
+class FieldNameProxy(Generic[TypeTable]):
     prefix: HasFieldName
-    t: T
+    t: TypeTable
 
-    def __get__(self, instance, owner) -> T:
-        ...
+    def __get__(self, instance, owner) -> TypeTable: ...
 
     def __getattr__(self, name: str) -> FieldNameProxyString:
         try:
             return FieldNameProxyString(
                 f"{self.prefix.field_name}.{self.t.__fields__[name].field_name}"
             )
         except KeyError:
@@ -163,91 +191,112 @@
 
 @dataclasses.dataclass(eq=False)
 class FieldNameProxyString(OrderByMixin, CompareMixin):
     field_name: str
 
 
 @dataclasses.dataclass(eq=False)
-class EmbeddedField[T: Table](Field[T]):
+class EmbeddedField(Generic[T], Field[T]):
     """
     Embedded field
     """
 
     _: FieldNameProxy[type[T]] = dataclasses.field(init=False)
 
     schema: type[T]
 
     def __post_init__(self):
         self._ = FieldNameProxy(self, self.schema)
-        self.marshamallow = fields.Nested(self.schema.__schema__)
+        self.marshamallow = fields.Nested(lambda: self.schema.__schema__)
 
         def load(value: Any, *, partial: bool = False) -> T:
             return self.schema.load(value, partial=partial)
 
+        def dump(value: T) -> dict[str, Any]:
+            return self.schema.dump(value)
+
         self.load = load
+        self.dump = dump
+
+    def __set_name__(self, owner: type[Table], name: str) -> None:
+        if not issubclass(self.schema, owner):
+            self.schema.__lazy_init_fields__()
+        return super().__set_name__(owner, name)
 
 
 @dataclasses.dataclass(eq=False)
-class ListFieldNameProxy[T: type[Table] | Any](OrderByMixin, CompareMixin):
+class ListFieldNameProxy(Generic[TypeTableOrAny], OrderByMixin, CompareMixin):
     number: int | None
     prefix: HasFieldName
-    t: T
+    t: TypeTableOrAny
 
     @property
     def field_name(self) -> str:
         if self.number is None:
             return self.prefix.field_name
         return f"{self.prefix.field_name}.{self.number}"
 
-    def __get__(self, instance, owner) -> T:
-        ...
+    def __get__(self, instance, owner) -> TypeTableOrAny: ...
 
     def __getattr__(self, name: str) -> FieldNameProxyString:
         try:
             return FieldNameProxyString(
                 f"{self.field_name}.{self.t.__fields__[name].field_name}"
             )
         except KeyError:
             message = "{0} has no attribute '{1}'".format(self.t, name)
             raise AttributeError(message) from None
 
 
 @dataclasses.dataclass(eq=False)
-class ListField[T](Field[list[T]]):
+class ListField(Generic[A], Field[list[A]]):
     """
     List field
     """
 
-    _: ListFieldNameProxy[type[T]] = dataclasses.field(init=False)
+    _: ListFieldNameProxy[type[A]] = dataclasses.field(init=False)
 
-    type_or_schema: type[T]
+    type_or_schema: type[A]
 
-    def __getitem__(self, index: int) -> type[T]:
+    def __getitem__(self, index: int) -> type[A]:
         return ListFieldNameProxy(index, self, self.type_or_schema)  # type: ignore
 
     def __post_init__(self):
         self._ = ListFieldNameProxy(None, self, self.type_or_schema)
 
         from .table import Table
 
         if issubclass(self.type_or_schema, Table):
             self.marshamallow = fields.List(
-                fields.Nested(self.type_or_schema.__schema__)
+                fields.Nested(lambda: self.type_or_schema.__schema__)  # type: ignore
             )
 
-            def load(value: Any, *, partial: bool = False) -> list[T]:
+            def load(value: Any, *, partial: bool = False) -> list[A]:
                 return [
                     self.type_or_schema.load(item, partial=partial)  # type: ignore
                     for item in value
                 ]
 
+            def dump(value: list[A]) -> list[dict[str, Any]]:
+                return [self.type_or_schema.dump(item) for item in value]  # type: ignore
+
             self.load = load
+            self.dump = dump
         else:
             self.marshamallow = fields.List(
                 {
                     int: fields.Integer(required=True),
                     float: fields.Float(required=True),
                     bool: fields.Boolean(required=True),
                     str: fields.String(required=True),
                     datetime: fields.DateTime(required=True),
                 }[self.type_or_schema]  # type: ignore
             )
+
+    def __set_name__(self, owner: type[Table], name: str) -> None:
+        from .table import Table
+
+        if issubclass(self.type_or_schema, Table) and not issubclass(
+            self.type_or_schema, owner
+        ):
+            self.type_or_schema.__lazy_init_fields__()
+        return super().__set_name__(owner, name)
```

### Comparing `typedmongo-0.0.0/typedmongo/sync.py` & `typedmongo-1.0.0/tests/sync.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 """
 Synchronize the asyncio module to the root module.
 """
+
 import pathlib
 
 
-def main():
+def main(just_check: bool = False):
+    exit_code = 0
     sync_dir = pathlib.Path(__file__).absolute().parent
     asyncio_dir = pathlib.Path(__file__).absolute().parent / "asyncio"
     for path in asyncio_dir.glob("*.py"):
         new_file_path = sync_dir / path.name
         content = path.read_text()
         content = (
             content.replace(
-                "from motor.motor_asyncio import AsyncIOMotorCollection",
-                "from pymongo.collection import Collection",
-            )
-            .replace(
-                "from motor.motor_asyncio import AsyncIOMotorDatabase",
-                "from pymongo.database import Database",
+                "from motor.motor_asyncio import AsyncIOMotorClient as MongoClient",
+                "from pymongo import MongoClient",
             )
+            .replace("typedmongo.asyncio", "typedmongo")
             .replace("async def ", "def ")
             .replace("await ", "")
             .replace("async for ", "for ")
             .replace("async with ", "with ")
             .replace("AsyncIterable", "Iterable")
         )
-        new_file_path.write_text(content)
+        if just_check:
+            if content != new_file_path.read_text():
+                print(f"File {new_file_path} is not synchronized.")
+                exit_code = 1
+        else:
+            new_file_path.write_text(content)
+    return exit_code
 
 
 if __name__ == "__main__":
-    main()
+    import sys
+
+    sys.exit(main("--check" in " ".join(sys.argv[1:])))
```

### Comparing `typedmongo-0.0.0/typedmongo/table.py` & `typedmongo-1.0.0/typedmongo/asyncio/table.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,42 +3,46 @@
 from functools import reduce
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Mapping,
     Optional,
-    Self,
     Sequence,
     get_args,
     get_origin,
 )
 
 from marshmallow import Schema
 from pymongo import IndexModel
+from typing_extensions import Self, dataclass_transform
 
 from typedmongo.exceptions import TableDefineError
 
 from .client import Manager
-from .fields import Field, ObjectIdField
+from .fields import Field
 
 
 def snake_case(name: str) -> str:
     """
     convert "SomeWords" to "some_words"
     """
     return "".join(
         "_" + char.lower() if char.isupper() and i > 0 else char.lower()
         for i, char in enumerate(name)
     )
 
 
 @dataclasses.dataclass
 class Index:
-    keys: Field | Sequence[tuple[Field, int]] | Mapping[Field, Any]
+    keys: (
+        Field
+        | Sequence[tuple[Field, int | str | Mapping[str, Any]]]
+        | Mapping[Field, Any]
+    )
 
     name: Optional[str] = None
     unique: bool = False
     background: bool = False
     sparse: bool = False
     expireAfterSeconds: Optional[int] = None
     partialFilterExpression: Optional[dict[str, Any]] = None
@@ -58,22 +62,25 @@
             background=self.background,
             sparse=self.sparse,
             expireAfterSeconds=self.expireAfterSeconds,
             partialFilterExpression=self.partialFilterExpression,
         )
 
 
+@dataclass_transform(eq_default=False, kw_only_default=True)
 class TableMetaClass(type):
     if TYPE_CHECKING:
         __abstract__: bool
         __database__: Any
         __collection_name__: str
         __collection__: Any
-        __fields__: dict[str, Field]
+        __pfields__: dict[str, Field]
+        __sfields__: dict[str, Field]
         __fields_loaded__: bool
+        __fields__: dict[str, Field]
         __create_schema__: Callable[[str, dict[str, Field]], Schema]
         __schema__: Schema
 
     def __new__(cls, name, bases, namespace):
         if "_" in name:  # check error name. e.g. Status_Info
             raise TableDefineError(
                 "Table class name cannot have '_': {name}".format(name=name)
@@ -83,59 +90,69 @@
                 "Table class name must be upper letter in start: {name}".format(
                     name=name
                 )
             )
         namespace.setdefault("__collection_name__", snake_case(name))
         namespace.setdefault("__abstract__", False)
 
-        # merge bases' `__fields__` to `__fields__`
-        fields = {
+        if "__fields__" in namespace:  # Clear __fields__ to avoid conflict
+            del namespace["__fields__"]
+        namespace["__fields_loaded__"] = False
+
+        namespace["__sfields__"] = {
             name: value for name, value in namespace.items() if isinstance(value, Field)
         }
-        namespace["__fields_loaded__"] = not not fields
-        namespace["__fields__"] = reduce(
+        # merge bases' `__fields__` to `__pfields__`
+        namespace["__pfields__"] = reduce(
             lambda _initial, _item: {**_item, **_initial},
-            reversed([getattr(base, "__fields__", {}) for base in bases]),
-            fields,
+            reversed(
+                [
+                    base.__lazy_init_fields__()
+                    for base in bases
+                    if isinstance(base, TableMetaClass)
+                ]
+            ),
+            {},
         )
 
         if "__create_schema__" not in namespace:
             for base in bases:
                 create_schema = base.__create_schema__
             namespace["__create_schema__"] = create_schema
-        namespace["__schema__"] = namespace["__create_schema__"](
-            name, namespace["__fields__"]
-        )
 
         return super().__new__(cls, name, bases, namespace)
 
-    def __lazy_init_fields__(cls) -> None:
+    def __lazy_init_fields__(cls) -> dict[str, Field]:
         if cls.__fields_loaded__:
-            return
+            return cls.__fields__
 
         fields = {
             **{
                 name: value()
                 for name, value in inspect.get_annotations(cls, eval_str=True).items()
                 if isinstance(value, type) and issubclass(value, Field)
             },
             **{
                 name: origin_class(*get_args(value))
                 for name, value in inspect.get_annotations(cls, eval_str=True).items()
                 if (origin_class := get_origin(value))
                 and isinstance(origin_class, type)
                 and issubclass(origin_class, Field)
             },
+            **cls.__sfields__,
         }
+        cls.__fields__ = {**cls.__pfields__, **fields}
+        cls.__fields_loaded__ = True
+
         for name, field in fields.items():
             setattr(cls, name, field)
             field.__set_name__(cls, name)
-        cls.__fields_loaded__ = True
-        cls.__fields__ = {**cls.__fields__, **fields}
-        cls.__schema__ = cls.__create_schema__(cls.__name__, fields)
+
+        cls.__schema__ = cls.__create_schema__(cls.__name__, cls.__fields__)
+        return fields
 
     def __call__(cls, **kwargs: Any):
         instance = super().__call__()
 
         if instance.__abstract__:
             raise RuntimeError(
                 "The class {} cannot be instantiated, because it's __abstract__ is True.".format(
@@ -153,25 +170,23 @@
             raise AttributeError(
                 "Can't modify the `__abstract__` attribute dynamically."
             )
         return super().__setattr__(name, value)
 
 
 class Table(metaclass=TableMetaClass):
-    __abstract__: bool = True
-
-    _id = ObjectIdField()
+    __abstract__ = True
 
     objects = Manager()
 
     def __repr__(self) -> str:
         return "{class_name}({fields})".format(
             class_name=self.__class__.__name__,
             fields=", ".join(
-                f"{name}={self.__dict__[name]}"
+                f"{name}={repr(self.__dict__[name])}"
                 for name, _ in self.__fields__.items()
                 if name in self.__dict__
             ),
         )
 
     @staticmethod
     def __create_schema__(name: str, fields: dict[str, Field]) -> Schema:
@@ -187,13 +202,21 @@
         validated = cls.__schema__.load(data=data, partial=partial)
         loaded = {
             key: getattr(cls.__fields__[key], "load")(value, partial=partial)
             for key, value in validated.items()  # type: ignore
         }
         return cls(**loaded)
 
-    def to_mongo(self) -> dict[str, Any]:
-        return {
-            key: getattr(self.__fields__[key], "to_mongo")(value)
-            for key, value in self.__dict__.items()
-            if key in self.__fields__
+    @classmethod
+    def dump(cls, instance: Self) -> dict[str, Any]:
+        dumped = {
+            key: getattr(instance.__fields__[key], "dump")(value)
+            for key, value in instance.__dict__.items()
         }
+        return cls.__schema__.dump(dumped)  # type: ignore
+
+    @classmethod
+    def indexes(cls) -> list[Index]:
+        return []
+
+    def to_mongo(self) -> dict[str, Any]:
+        return self.dump(self)
```

