# Comparing `tmp/pysql-repo-0.5.9.tar.gz` & `tmp/pysql-repo-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysql-repo-0.5.9.tar", last modified: Fri Feb  2 17:20:02 2024, max compression
+gzip compressed data, was "pysql-repo-0.6.0.tar", last modified: Thu Apr 25 15:17:45 2024, max compression
```

## Comparing `pysql-repo-0.5.9.tar` & `pysql-repo-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 17:20:02.235446 pysql-repo-0.5.9/
--rw-r--r--   0 runner    (1001) docker     (127)    41331 2024-02-02 17:20:02.235446 pysql-repo-0.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    40730 2024-02-02 17:20:00.000000 pysql-repo-0.5.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 17:20:02.231446 pysql-repo-0.5.9/pysql_repo/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-02-02 17:20:00.000000 pysql-repo-0.5.9/pysql_repo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 17:20:02.235446 pysql-repo-0.5.9/pysql_repo/_constants/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-02 17:20:00.000000 pysql-repo-0.5.9/pysql_repo/_constants/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-02 17:20:00.000000 pysql-repo-0.5.9/pysql_repo/_constants/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-02-02 17:20:00.000000 pysql-repo-0.5.9/pysql_repo/_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-02-02 17:20:00.000000 pysql-repo-0.5.9/pysql_repo/_database_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-02-02 17:20:00.000000 pysql-repo-0.5.9/pysql_repo/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-02-02 17:20:00.000000 pysql-repo-0.5.9/pysql_repo/_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-02-02 17:20:00.000000 pysql-repo-0.5.9/pysql_repo/_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    16118 2024-02-02 17:20:00.000000 pysql-repo-0.5.9/pysql_repo/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 17:20:02.235446 pysql-repo-0.5.9/pysql_repo/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-02 17:20:00.000000 pysql-repo-0.5.9/pysql_repo/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-02-02 17:20:00.000000 pysql-repo-0.5.9/pysql_repo/asyncio/async_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-02-02 17:20:00.000000 pysql-repo-0.5.9/pysql_repo/asyncio/async_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12391 2024-02-02 17:20:00.000000 pysql-repo-0.5.9/pysql_repo/asyncio/async_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-02-02 17:20:00.000000 pysql-repo-0.5.9/pysql_repo/asyncio/async_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 17:20:02.235446 pysql-repo-0.5.9/pysql_repo/libs/
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-02-02 17:20:00.000000 pysql-repo-0.5.9/pysql_repo/libs/file_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 17:20:02.235446 pysql-repo-0.5.9/pysql_repo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41331 2024-02-02 17:20:02.000000 pysql-repo-0.5.9/pysql_repo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-02-02 17:20:02.000000 pysql-repo-0.5.9/pysql_repo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 17:20:02.000000 pysql-repo-0.5.9/pysql_repo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-02 17:20:02.000000 pysql-repo-0.5.9/pysql_repo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-02 17:20:02.000000 pysql-repo-0.5.9/pysql_repo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-02 17:20:02.235446 pysql-repo-0.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-02-02 17:20:01.000000 pysql-repo-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:17:45.073656 pysql-repo-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    41337 2024-04-25 15:17:45.073656 pysql-repo-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    40736 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:17:45.073656 pysql-repo-0.6.0/pysql_repo/
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:17:45.073656 pysql-repo-0.6.0/pysql_repo/_constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/_constants/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/_database_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18597 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22775 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:17:45.073656 pysql-repo-0.6.0/pysql_repo/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/asyncio/async_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/asyncio/async_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19391 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/asyncio/async_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/asyncio/async_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:17:45.073656 pysql-repo-0.6.0/pysql_repo/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-25 15:17:35.000000 pysql-repo-0.6.0/pysql_repo/libs/file_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:17:45.073656 pysql-repo-0.6.0/pysql_repo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41337 2024-04-25 15:17:45.000000 pysql-repo-0.6.0/pysql_repo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-25 15:17:45.000000 pysql-repo-0.6.0/pysql_repo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:17:45.000000 pysql-repo-0.6.0/pysql_repo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 15:17:45.000000 pysql-repo-0.6.0/pysql_repo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 15:17:45.000000 pysql-repo-0.6.0/pysql_repo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:17:45.073656 pysql-repo-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-25 15:17:42.000000 pysql-repo-0.6.0/setup.py
```

### Comparing `pysql-repo-0.5.9/PKG-INFO` & `pysql-repo-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysql-repo
-Version: 0.5.9
+Version: 0.6.0
 Summary: A project to have a base repository class to perform select/insert/update/delete with dynamic syntax
 Home-page: https://github.com/Impro02/pysql-repo
-Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.5.9.tar.gz
+Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.6.0.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -595,16 +595,16 @@
     def __init__(
         self,
         user_repository: UserRepository,
         logger: Logger,
     ) -> None:
         super().__init__(
             repository=user_repository,
-            logger=logger,
         )
+        self._logger = logger
 
     @with_session()
     def get_users(
         self,
         ids_in: Optional[List[int]] = None,
         ids_not_in: Optional[List[int]] = None,
         emails_iin: Optional[List[str]] = None,
@@ -1163,16 +1163,16 @@
     def __init__(
         self,
         user_repository: AsyncUserRepository,
         logger: Logger,
     ) -> None:
         super().__init__(
             repository=user_repository,
-            logger=logger,
         )
+        self._logger = logger
 
     @with_async_session()
     async def get_users(
         self,
         session: Optional[AsyncSession] = None,
         ids_in: Optional[List[int]] = None,
         ids_not_in: Optional[List[int]] = None,
```

### Comparing `pysql-repo-0.5.9/README.md` & `pysql-repo-0.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -580,16 +580,16 @@
     def __init__(
         self,
         user_repository: UserRepository,
         logger: Logger,
     ) -> None:
         super().__init__(
             repository=user_repository,
-            logger=logger,
         )
+        self._logger = logger
 
     @with_session()
     def get_users(
         self,
         ids_in: Optional[List[int]] = None,
         ids_not_in: Optional[List[int]] = None,
         emails_iin: Optional[List[str]] = None,
@@ -1148,16 +1148,16 @@
     def __init__(
         self,
         user_repository: AsyncUserRepository,
         logger: Logger,
     ) -> None:
         super().__init__(
             repository=user_repository,
-            logger=logger,
         )
+        self._logger = logger
 
     @with_async_session()
     async def get_users(
         self,
         session: Optional[AsyncSession] = None,
         ids_in: Optional[List[int]] = None,
         ids_not_in: Optional[List[int]] = None,
```

### Comparing `pysql-repo-0.5.9/pysql_repo/__init__.py` & `pysql-repo-0.6.0/pysql_repo/__init__.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.5.9/pysql_repo/_constants/enum.py` & `pysql-repo-0.6.0/pysql_repo/_constants/enum.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # MODULES
 import enum
 
 
 class Operators(enum.Enum):
+    """
+    Enum class representing various operators used in SQL queries.
+    """
+
     LIKE = "LIKE"
     NOT_LIKE = "NOT_LIKE"
     ILIKE = "ILIKE"
     NOT_ILIKE = "NOT_ILIKE"
     EQUAL = "EQUAL"
     IEQUAL = "IEQUAL"
     DIFFERENT = "DIFFERENT"
@@ -22,14 +26,18 @@
     NOT_IN = "NOT_IN"
     NOT_IIN = "NOT_IIN"
     HAS = "HAS"
     ANY = "ANY"
 
 
 class LoadingTechnique(enum.Enum):
+    """
+    Enum class representing different loading techniques.
+    """
+
     CONTAINS_EAGER = "contains_eager"
     LAZY = "select"
     JOINED = "joined"
     SUBQUERY = "subquery"
     SELECTIN = "selectin"
     RAISE = "raise"
     NOLOAD = "noload"
```

### Comparing `pysql-repo-0.5.9/pysql_repo/_utils.py` & `pysql-repo-0.6.0/pysql_repo/_repository.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,506 +1,607 @@
 # MODULES
-from ast import Delete
-from dataclasses import dataclass, field
-import json
 from typing import (
     Any,
+    Callable,
     Dict,
-    Iterable,
     List,
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
+    Sequence,
 )
 
+# CONTEXTLIB
+from contextlib import AbstractContextManager
+
 # SQLALCHEMY
-from sqlalchemy import (
-    ColumnExpressionArgument,
-    Select,
-    Update,
-    and_,
-    asc,
-    delete,
-    desc,
-    insert,
-    select,
-    distinct,
-    tuple_,
-    func,
-    update,
-)
-from sqlalchemy.ext.asyncio import AsyncSession
+from sqlalchemy import ColumnExpressionArgument, Select
 from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.orm import (
-    Session,
-    noload,
-    lazyload,
-    joinedload,
-    subqueryload,
-    selectinload,
-    raiseload,
-    contains_eager,
-)
-from sqlalchemy.orm.attributes import InstrumentedAttribute
-from sqlalchemy.sql.dml import ReturningDelete, ReturningInsert, ReturningUpdate
-from sqlalchemy.sql.elements import Null, BinaryExpression
+from sqlalchemy.orm import Session, InstrumentedAttribute
 
-# Enum
-from pysql_repo._constants.enum import LoadingTechnique, Operators
+# DECORATORS
+from pysql_repo._decorators import check_values as _check_values, with_session
+
+# UTILS
+from pysql_repo._utils import (
+    _FilterType,
+    RelationshipOption,
+    build_delete_stmt as _build_delete_stmt,
+    build_insert_stmt as _build_insert_stmt,
+    build_select_stmt as _build_select_stmt,
+    build_update_stmt as _build_update_stmt,
+    select_distinct as _select_distinct,
+    apply_pagination as _apply_pagination,
+)
 
-_FilterType = Dict[Union[InstrumentedAttribute, Tuple[InstrumentedAttribute]], Any]
 
 _T = TypeVar("_T", bound=declarative_base())
 
 
-@dataclass
-class RelationshipOption:
-    lazy: LoadingTechnique
-    added_criteria: Optional[BinaryExpression] = field(default=None)
-    children: Dict[InstrumentedAttribute, "RelationshipOption"] = field(default=None)
-
-
-def build_select_stmt(
-    stmt: Select[Tuple[_T]],
-    model: Optional[Type[_T]] = None,
-    filters: Optional[_FilterType] = None,
-    optional_filters: Optional[_FilterType] = None,
-    relationship_options: Optional[
-        Dict[InstrumentedAttribute, RelationshipOption]
-    ] = None,
-    group_by: Optional[ColumnExpressionArgument] = None,
-    order_by: Optional[Union[List[str], str]] = None,
-    direction: Optional[Union[List[str], str]] = None,
-    limit: int = None,
-) -> Select[Tuple[_T]]:
-    stmt = apply_relationship_options(
-        stmt=stmt,
-        relationship_options=relationship_options,
-    )
-
-    stmt = apply_filters(
-        stmt=stmt,
-        filter_dict=filters,
-    )
-    stmt = apply_filters(
-        stmt=stmt,
-        filter_dict=optional_filters,
-        with_optional=True,
-    )
-
-    stmt = apply_group_by(
-        stmt=stmt,
-        group_by=group_by,
-    )
-
-    stmt = apply_order_by(
-        stmt=stmt,
-        model=model,
-        order_by=order_by,
-        direction=direction,
-    )
-
-    return apply_limit(
-        stmt=stmt,
-        limit=limit,
-    )
-
-
-def build_update_stmt(
-    model: Type[_T],
-    values: Dict,
-    filters: Optional[_FilterType] = None,
-) -> ReturningUpdate[Tuple[_T]]:
-    return (
-        apply_filters(
-            stmt=update(model),
-            filter_dict=filters,
-        )
-        .values(values)
-        .returning(model)
-    )
-
-
-def build_insert_stmt(
-    model: Type[_T],
-) -> ReturningInsert[Tuple[_T]]:
-    return insert(model).returning(model)
-
-
-def build_delete_stmt(
-    model: Type[_T],
-    filters: _FilterType,
-) -> ReturningDelete[Tuple[_T]]:
-    return apply_filters(
-        stmt=delete(model),
-        filter_dict=filters,
-    ).returning(model)
-
-
-def select_distinct(
-    model: Type[_T],
-    expr: ColumnExpressionArgument,
-) -> Select[Tuple[_T]]:
-    return select(distinct(expr)) if expr is not None else select(model)
-
-
-def apply_group_by(
-    stmt: Select[Tuple[_T]],
-    group_by: ColumnExpressionArgument,
-) -> Select[Tuple[_T]]:
-    return stmt.group_by(group_by) if group_by is not None else stmt
-
-
-def apply_relationship_options(
-    stmt: Union[Select[Tuple[_T]], Update],
-    relationship_options: Dict[InstrumentedAttribute, RelationshipOption],
-    parents: List[InstrumentedAttribute] = None,
-) -> Union[Select[Tuple[_T]], Update]:
-    def get_load(
-        loading_technique: LoadingTechnique,
-        items: List[InstrumentedAttribute],
-        extra_conditions: Optional[BinaryExpression] = None,
-    ):
-        items_post = []
-        for item in items:
-            if extra_conditions is not None:
-                items_post.append(item.and_(*extra_conditions))
-            else:
-                items_post.append(item)
-
-        if loading_technique == LoadingTechnique.CONTAINS_EAGER:
-            return contains_eager(*items_post)
-        elif loading_technique == LoadingTechnique.LAZY:
-            return lazyload(*items_post)
-        elif loading_technique == LoadingTechnique.JOINED:
-            return joinedload(*items_post)
-        elif loading_technique == LoadingTechnique.SUBQUERY:
-            return subqueryload(*items_post)
-        elif loading_technique == LoadingTechnique.SELECTIN:
-            return selectinload(*items_post)
-        elif loading_technique == LoadingTechnique.RAISE:
-            return raiseload(*items_post)
-        elif loading_technique == LoadingTechnique.NOLOAD:
-            return noload(*items_post)
-
-        return None
-
-    if relationship_options is None:
-        return stmt
-
-    for relationship, sub_relationships in relationship_options.items():
-        if any(
-            [
-                relationship is None,
-                not isinstance(relationship, InstrumentedAttribute),
-                sub_relationships is None,
-                not isinstance(sub_relationships, RelationshipOption),
-            ]
-        ):
-            continue
-
-        sub_items = [relationship] if parents is None else [*parents, relationship]
-
-        load = get_load(
-            loading_technique=sub_relationships.lazy,
-            items=sub_items,
-            extra_conditions=sub_relationships.added_criteria,
-        )
-
-        if load is not None:
-            stmt = stmt.options(load)
-
-        if (children := sub_relationships.children) is not None:
-            stmt = apply_relationship_options(
-                stmt,
-                relationship_options=children,
-                parents=sub_items,
-            )
-
-    return stmt
-
-
-def apply_filters(
-    stmt: Union[Select[Tuple[_T]], Update],
-    filter_dict: _FilterType,
-    with_optional: bool = False,
-) -> Union[Select[Tuple[_T]], Update, Delete]:
-    filters = get_filters(
-        filters=filter_dict,
-        with_optional=with_optional,
-    )
-
-    return stmt if len(filters) == 0 else stmt.filter(and_(*filters))
-
-
-def apply_order_by(
-    stmt: Select[Tuple[_T]],
-    model: Type[_T],
-    order_by: Union[List[str], str],
-    direction: Union[List[str], str],
-) -> Select[Tuple[_T]]:
-    if order_by is None or direction is None:
-        return stmt
-
-    if isinstance(order_by, str):
-        order_by = [order_by]
-
-    if isinstance(direction, str):
-        direction = [direction]
-
-    if len(order_by) != len(direction):
-        raise ValueError("order_by length must be equals to direction length")
-
-    order_by_list = []
-    for column, dir in zip(order_by, direction):
-        if dir == "desc":
-            order_by_list.append(desc(getattr(model, column)))
-        elif dir == "asc":
-            order_by_list.append(asc(getattr(model, column)))
-
-    return stmt.order_by(*order_by_list)
-
-
-def apply_pagination(
-    session: Session,
-    stmt: Select[Tuple[_T]],
-    page: int,
-    per_page: int,
-) -> Tuple[Select[Tuple[_T]], str]:
-    if page is None or per_page is None:
-        return stmt, None
-
-    total_results = session.scalar(select(func.count()).select_from(stmt))
-    total_pages = (total_results + per_page - 1) // per_page
-
-    pagination = {
-        "total": total_results,
-        "page": page,
-        "per_page": per_page,
-        "total_pages": total_pages,
-    }
-
-    pagination = json.dumps(pagination)
-
-    stmt = stmt.offset((page - 1) * per_page).limit(per_page)
-
-    return stmt, pagination
-
-
-async def async_apply_pagination(
-    session: AsyncSession,
-    stmt: Select[Tuple[_T]],
-    page: int,
-    per_page: int,
-) -> Tuple[Select[Tuple[_T]], str]:
-    if page is None or per_page is None:
-        return stmt, None
-
-    total_results = await session.scalar(select(func.count()).select_from(stmt))
-    total_pages = (total_results + per_page - 1) // per_page
-
-    pagination = {
-        "total": total_results,
-        "page": page,
-        "per_page": per_page,
-        "total_pages": total_pages,
-    }
-
-    pagination = json.dumps(pagination)
-
-    stmt = stmt.offset((page - 1) * per_page).limit(per_page)
-
-    return stmt, pagination
-
-
-def apply_limit(
-    stmt: Select[Tuple[_T]],
-    limit: int,
-) -> Select[Tuple[_T]]:
-    return stmt.limit(limit) if limit is not None else stmt
-
-
-def get_conditions_from_dict(
-    values: _FilterType,
-    with_optional: bool = False,
-) -> List[ColumnExpressionArgument]:
-    conditions = []
-    for key, value in values.items():
-        if type(value) is set:
-            value = list(value)
-        elif type(value) is dict:
-            for k, v in value.items():
-                if with_optional and v is None:
-                    continue
-
-                match k:
-                    case Operators.EQUAL:
-                        conditions.append(key == v)
-                    case Operators.IEQUAL:
-                        if not isinstance(v, Null):
-                            conditions.append(func.lower(key) == func.lower(v))
-                        else:
-                            conditions.append(key == v)
-                    case Operators.DIFFERENT:
-                        conditions.append(key != v)
-                    case Operators.IDIFFERENT:
-                        if not isinstance(v, Null):
-                            conditions.append(func.lower(key) != func.lower(v))
-                        else:
-                            conditions.append(key != v)
-                    case Operators.LIKE:
-                        if not isinstance(v, Null):
-                            conditions.append(key.like(v))
-                        else:
-                            conditions.append(key == v)
-                    case Operators.NOT_LIKE:
-                        if not isinstance(v, Null):
-                            conditions.append(~key.like(v))
-                        else:
-                            conditions.append(key != v)
-                    case Operators.ILIKE:
-                        if not isinstance(v, Null):
-                            conditions.append(key.ilike(v))
-                        else:
-                            conditions.append(key == v)
-                    case Operators.NOT_ILIKE:
-                        if not isinstance(v, Null):
-                            conditions.append(~key.ilike(v))
-                        else:
-                            conditions.append(key != v)
-                    case Operators.BETWEEN:
-                        if len(v) != 2:
-                            continue
-                        if v[0] is not None:
-                            conditions.append(key > v[0])
-                        if v[1] is not None:
-                            conditions.append(key < v[1])
-                    case Operators.BETWEEN_OR_EQUAL:
-                        if len(v) != 2:
-                            continue
-                        if v[0] is not None:
-                            conditions.append(key >= v[0])
-                        if v[1] is not None:
-                            conditions.append(key <= v[1])
-                    case Operators.SUPERIOR:
-                        conditions.append(key > v)
-                    case Operators.INFERIOR:
-                        conditions.append(key < v)
-                    case Operators.SUPERIOR_OR_EQUAL:
-                        conditions.append(key >= v)
-                    case Operators.INFERIOR_OR_EQUAL:
-                        conditions.append(key <= v)
-                    case Operators.IN:
-                        v = v if isinstance(v, Iterable) else [v]
-                        if isinstance(key, tuple):
-                            conditions.append(tuple_(*key).in_(v))
-                        else:
-                            conditions.append(key.in_(v))
-                    case Operators.IIN:
-                        v = v if isinstance(v, Iterable) else [v]
-                        if isinstance(key, tuple):
-                            conditions.append(
-                                tuple_([func.lower(key_) for key_ in key]).in_(
-                                    [
-                                        (
-                                            func.lower(v_)
-                                            if not isinstance(v_, Null)
-                                            else v_
-                                        )
-                                        for v_ in v
-                                    ]
-                                )
-                            )
-                        else:
-                            conditions.append(
-                                func.lower(key).in_(
-                                    [
-                                        (
-                                            func.lower(v_)
-                                            if not isinstance(v_, Null)
-                                            else v_
-                                        )
-                                        for v_ in v
-                                    ]
-                                )
-                            )
-                    case Operators.NOT_IN:
-                        v = v if isinstance(v, Iterable) else [v]
-                        if isinstance(key, tuple):
-                            conditions.append(tuple_(*key).notin_(v))
-                        else:
-                            conditions.append(key.notin_(v))
-
-                    case Operators.NOT_IIN:
-                        v = v if isinstance(v, Iterable) else [v]
-                        if isinstance(key, tuple):
-                            conditions.append(
-                                tuple_([func.lower(key_) for key_ in key]).notin_(
-                                    [
-                                        (
-                                            func.lower(v_)
-                                            if not isinstance(v_, Null)
-                                            else v_
-                                        )
-                                        for v_ in v
-                                    ]
-                                )
-                            )
-                        else:
-                            conditions.append(
-                                func.lower(key).notin_(
-                                    [
-                                        (
-                                            func.lower(v_)
-                                            if not isinstance(v_, Null)
-                                            else v_
-                                        )
-                                        for v_ in v
-                                    ]
-                                )
-                            )
-                    case Operators.HAS:
-                        v = get_filters(
-                            v,
-                            with_optional=with_optional,
-                        )
-                        for condition in v:
-                            conditions.append(key.has(condition))
-                    case Operators.ANY:
-                        v = get_filters(
-                            v,
-                            with_optional=with_optional,
-                        )
-
-                        if len(v) == 0:
-                            continue
-
-                        conditions.append(key.any(and_(*v)))
-
-    return conditions
-
-
-def get_filters(
-    filters: _FilterType,
-    with_optional: bool = False,
-) -> List[ColumnExpressionArgument]:
-    if filters is None:
-        return []
-    if not isinstance(filters, dict):
-        raise TypeError("<filters> must be type of <dict>")
-
-    filters = [{x: y} for x, y in filters.items()]
-
-    conditions = []
-    for filter_c in filters:
-        if type(filter_c) is not dict:
-            continue
-
-        conditions_from_dict = get_conditions_from_dict(
-            filter_c,
-            with_optional=with_optional,
+class Repository:
+    """
+    Represents a repository for database operations.
+
+    Attributes:
+        _session_factory: The session factory used for creating sessions.
+
+    Methods:
+        session_manager: Returns the session factory.
+        _select: Selects a single row from the database.
+        _select_stmt: Selects a single row from the database using a custom statement.
+        _select_all: Selects all rows from the database.
+        _select_all_stmt: Selects all rows from the database using a custom statement.
+        _select_paginate: Selects a paginated set of rows from the database.
+        _select_paginate_stmt: Selects a paginated set of rows from the database using a custom statement.
+    """
+
+    def __init__(
+        self,
+        session_factory: Callable[..., AbstractContextManager[Session]],
+    ) -> None:
+        """
+        Initializes the Repository.
+
+        Args:
+            session_factory: A callable that returns a context manager
+                             for creating and managing database sessions.
+
+        Returns:
+            None
+        """
+        self._session_factory = session_factory
+
+    def session_manager(self) -> AbstractContextManager[Session]:
+        """
+        Get a session manager.
+
+        Returns:
+            AbstractContextManager[Session]: An context manager for managing database sessions.
+        """
+        return self._session_factory()
+
+    @with_session()
+    def _select(
+        self,
+        model: Type[_T],
+        distinct: Optional[ColumnExpressionArgument] = None,
+        filters: Optional[_FilterType] = None,
+        optional_filters: Optional[_FilterType] = None,
+        relationship_options: Optional[
+            Dict[InstrumentedAttribute, RelationshipOption]
+        ] = None,
+        session: Optional[Session] = None,
+    ) -> Optional[_T]:
+        """
+        Selects a single object from the database.
+
+        Args:
+            model: The model class representing the table.
+            distinct: The distinct column expression.
+            filters: The filters to apply.
+            optional_filters: The optional filters to apply.
+            relationship_options: The relationship options.
+            session: The session to use.
+
+        Returns:
+            The selected object or None if not found.
+        """
+        stmt = _select_distinct(
+            model=model,
+            expr=distinct,
+        )
+
+        return self._select_stmt(
+            stmt=stmt,
+            filters=filters,
+            optional_filters=optional_filters,
+            relationship_options=relationship_options,
+            session=session,
+        )
+
+    @with_session()
+    def _select_stmt(
+        self,
+        stmt: Select[Tuple[_T]],
+        filters: Optional[_FilterType] = None,
+        optional_filters: Optional[_FilterType] = None,
+        relationship_options: Optional[
+            Dict[InstrumentedAttribute, RelationshipOption]
+        ] = None,
+        group_by: Optional[ColumnExpressionArgument] = None,
+        session: Optional[Session] = None,
+    ) -> Optional[_T]:
+        """
+        Selects a single object from the database using a custom statement.
+
+        Args:
+            stmt: The custom select statement.
+            filters: The filters to apply.
+            optional_filters: The optional filters to apply.
+            relationship_options: The relationship options.
+            group_by: The column expression to group by.
+            session: The session to use.
+
+        Returns:
+            The selected object or None if not found.
+        """
+        stmt = _build_select_stmt(
+            stmt=stmt,
+            filters=filters,
+            optional_filters=optional_filters,
+            relationship_options=relationship_options,
+            group_by=group_by,
+        )
+
+        return session.execute(stmt).unique().scalar_one_or_none()
+
+    @with_session()
+    def _select_all(
+        self,
+        model: Type[_T],
+        distinct: Optional[List[ColumnExpressionArgument]] = None,
+        filters: Optional[_FilterType] = None,
+        optional_filters: Optional[_FilterType] = None,
+        relationship_options: Optional[
+            Dict[InstrumentedAttribute, RelationshipOption]
+        ] = None,
+        order_by: Optional[Union[List[str], str]] = None,
+        direction: Optional[str] = None,
+        limit: int = None,
+        session: Optional[Session] = None,
+    ) -> Sequence[_T]:
+        """
+        Selects all objects from the database.
+
+        Args:
+            model: The model class representing the table.
+            distinct: The distinct column expressions.
+            filters: The filters to apply.
+            optional_filters: The optional filters to apply.
+            relationship_options: The relationship options.
+            order_by: The column(s) to order by.
+            direction: The direction of the ordering.
+            limit: The maximum number of objects to return.
+            session: The session to use.
+
+        Returns:
+            A sequence of selected objects.
+        """
+        stmt = _select_distinct(
+            model=model,
+            expr=distinct,
+        )
+
+        return self._select_all_stmt(
+            stmt=stmt,
+            model=model,
+            filters=filters,
+            optional_filters=optional_filters,
+            relationship_options=relationship_options,
+            order_by=order_by,
+            direction=direction,
+            limit=limit,
+            session=session,
+        )
+
+    @with_session()
+    def _select_all_stmt(
+        self,
+        stmt: Select[Tuple[_T]],
+        model: Type[_T],
+        filters: Optional[_FilterType] = None,
+        optional_filters: Optional[_FilterType] = None,
+        relationship_options: Optional[
+            Dict[InstrumentedAttribute, RelationshipOption]
+        ] = None,
+        group_by: Optional[ColumnExpressionArgument] = None,
+        order_by: Optional[Union[List[str], str]] = None,
+        direction: Optional[Union[List[str], str]] = None,
+        limit: int = None,
+        session: Optional[Session] = None,
+    ) -> Sequence[_T]:
+        """
+        Selects all objects from the database using a custom statement.
+
+        Args:
+            stmt: The custom select statement.
+            model: The model class representing the table.
+            filters: The filters to apply.
+            optional_filters: The optional filters to apply.
+            relationship_options: The relationship options.
+            group_by: The column expression to group by.
+            order_by: The column(s) to order by.
+            direction: The direction of the ordering.
+            limit: The maximum number of rows to return.
+            session: The session to use.
+
+        Returns:
+            A sequence of selected objects.
+        """
+        stmt = _build_select_stmt(
+            stmt=stmt,
+            model=model,
+            filters=filters,
+            optional_filters=optional_filters,
+            relationship_options=relationship_options,
+            group_by=group_by,
+            order_by=order_by,
+            direction=direction,
+            limit=limit,
+        )
+
+        return session.execute(stmt).unique().scalars().all()
+
+    @with_session()
+    def _select_paginate(
+        self,
+        model: Type[_T],
+        page: int,
+        per_page: int,
+        distinct: Optional[ColumnExpressionArgument] = None,
+        filters: Optional[_FilterType] = None,
+        optional_filters: Optional[_FilterType] = None,
+        relationship_options: Optional[
+            Dict[InstrumentedAttribute, RelationshipOption]
+        ] = None,
+        order_by: Optional[Union[List[str], str]] = None,
+        direction: Optional[str] = None,
+        limit: int = None,
+        session: Optional[Session] = None,
+    ) -> Tuple[Sequence[_T], str]:
+        """
+        Selects a paginated set of objects from the database.
+
+        Args:
+            model: The model class representing the table.
+            page: The page number.
+            per_page: The number of items per page.
+            distinct: The distinct column expression.
+            filters: The filters to apply.
+            optional_filters: The optional filters to apply.
+            relationship_options: The relationship options.
+            order_by: The column(s) to order by.
+            direction: The direction of the ordering.
+            limit: The maximum number of objects to return.
+            session: The session to use.
+
+        Returns:
+            A tuple containing the selected objects and pagination information.
+        """
+        stmt = _select_distinct(
+            model=model,
+            expr=distinct,
+        )
+
+        return self._select_paginate_stmt(
+            stmt=stmt,
+            model=model,
+            page=page,
+            per_page=per_page,
+            filters=filters,
+            optional_filters=optional_filters,
+            relationship_options=relationship_options,
+            order_by=order_by,
+            direction=direction,
+            limit=limit,
+            session=session,
+        )
+
+    @with_session()
+    def _select_paginate_stmt(
+        self,
+        stmt: Select[Tuple[_T]],
+        model: Type[_T],
+        page: int,
+        per_page: int,
+        filters: Optional[_FilterType] = None,
+        optional_filters: Optional[_FilterType] = None,
+        relationship_options: Optional[
+            Dict[InstrumentedAttribute, RelationshipOption]
+        ] = None,
+        group_by: Optional[ColumnExpressionArgument] = None,
+        order_by: Optional[Union[List[str], str]] = None,
+        direction: Optional[str] = None,
+        limit: int = None,
+        session: Optional[Session] = None,
+    ) -> Tuple[Sequence[_T], str]:
+        """
+        Selects a paginated set of rows from the database using a custom statement.
+
+        Args:
+            stmt: The custom select statement.
+            model: The model class representing the table.
+            page: The page number.
+            per_page: The number of items per page.
+            filters: The filters to apply.
+            optional_filters: The optional filters to apply.
+            relationship_options: The relationship options.
+            group_by: The column expression to group by.
+            order_by: The column(s) to order by.
+            direction: The direction of the ordering.
+            limit: The maximum number of rows to return.
+            session: The session to use.
+
+        Returns:
+            A tuple containing the selected objects and pagination information.
+        """
+        stmt = _build_select_stmt(
+            stmt=stmt,
+            model=model,
+            filters=filters,
+            optional_filters=optional_filters,
+            relationship_options=relationship_options,
+            group_by=group_by,
+            order_by=order_by,
+            direction=direction,
+            limit=limit,
+        )
+
+        stmt, pagination = _apply_pagination(
+            session=session,
+            stmt=stmt,
+            page=page,
+            per_page=per_page,
         )
-        conditions.extend(conditions_from_dict)
 
-    return conditions
+        return session.execute(stmt).unique().scalars().all(), pagination
+
+    @_check_values(as_list=False)
+    @with_session()
+    def _update_all(
+        self,
+        model: Type[_T],
+        values: Dict[str, Any],
+        filters: Optional[_FilterType] = None,
+        flush: bool = False,
+        commit: bool = False,
+        session: Optional[Session] = None,
+    ) -> Sequence[_T]:
+        """
+        Updates multiple objects in the database.
+
+        Args:
+            model: The model class representing the table.
+            values: A dictionary of column-value pairs to update.
+            filters: The filters to apply.
+            flush: Whether to flush the session after the update.
+            commit: Whether to commit the session after the update.
+            session: The session to use.
+
+        Returns:
+            A sequence of updated objects.
+        """
+        stmt = _build_update_stmt(
+            model=model,
+            values=values,
+            filters=filters,
+        )
+
+        sequence = session.execute(stmt).unique().scalars().all()
+
+        if flush:
+            session.flush()
+        if commit:
+            session.commit()
+
+        [session.refresh(item) for item in sequence]
+
+        return sequence
+
+    @_check_values(as_list=False)
+    @with_session()
+    def _update(
+        self,
+        model: Type[_T],
+        values: Dict[str, Any],
+        filters: Optional[_FilterType] = None,
+        flush: bool = False,
+        commit: bool = False,
+        session: Optional[Session] = None,
+    ) -> Optional[_T]:
+        """
+        Updates a single object in the database.
+
+        Args:
+            model: The model class representing the table.
+            values: A dictionary of column-value pairs to update.
+            filters: The filters to apply.
+            flush: Whether to flush the session after the update.
+            commit: Whether to commit the session after the update.
+            session: The session to use.
+
+        Returns:
+            The updated object or None if not found.
+        """
+        stmt = _build_update_stmt(
+            model=model,
+            values=values,
+            filters=filters,
+        )
+
+        item = session.execute(stmt).unique().scalar_one_or_none()
+
+        if item is None:
+            return None
+
+        if flush:
+            session.flush()
+        if commit:
+            session.commit()
+
+        session.refresh(item)
+
+        return item
+
+    @_check_values(as_list=True)
+    @with_session()
+    def _add_all(
+        self,
+        model: Type[_T],
+        values: List[Dict[str, Any]],
+        flush: bool = False,
+        commit: bool = False,
+        session: Optional[Session] = None,
+    ) -> Sequence[_T]:
+        """
+        Adds multiple objects to the database.
+
+        Args:
+            model: The model class representing the table.
+            values: A list of dictionaries containing column-value pairs for each object.
+            flush: Whether to flush the session after adding the objects.
+            commit: Whether to commit the session after adding the objects.
+            session: The session to use.
+
+        Returns:
+            A sequence of added objects.
+        """
+        stmt = _build_insert_stmt(model=model)
+
+        sequence = session.execute(stmt, values).unique().scalars().all()
+
+        if flush:
+            session.flush()
+        if commit:
+            session.commit()
+
+        if flush or commit:
+            [session.refresh(item) for item in sequence]
+
+        return sequence
+
+    @_check_values(as_list=False)
+    @with_session()
+    def _add(
+        self,
+        model: Type[_T],
+        values: Dict[str, Any],
+        flush: bool = False,
+        commit: bool = False,
+        session: Optional[Session] = None,
+    ) -> _T:
+        """
+        Adds a single object to the database.
+
+        Args:
+            model: The model class representing the table.
+            values: A dictionary of column-value pairs for the object.
+            flush: Whether to flush the session after adding the object.
+            commit: Whether to commit the session after adding the object.
+            session: The session to use.
+
+        Returns:
+            The added object.
+        """
+        stmt = _build_insert_stmt(model=model)
+
+        item = session.execute(stmt, values).unique().scalar_one()
+
+        if flush:
+            session.flush()
+        if commit:
+            session.commit()
+
+        if flush or commit:
+            session.refresh(item)
+
+        return item
+
+    @with_session()
+    def _delete_all(
+        self,
+        model: Type[_T],
+        filters: Optional[_FilterType] = None,
+        flush: bool = True,
+        commit: bool = False,
+        session: Optional[Session] = None,
+    ) -> bool:
+        """
+        Deletes multiple objects from the database.
+
+        Args:
+            model: The model class representing the table.
+            filters: The filters to apply.
+            flush: Whether to flush the session after the deletion.
+            commit: Whether to commit the session after the deletion.
+            session: The session to use.
+
+        Returns:
+            True if any objects were deleted, False otherwise.
+        """
+        stmt = _build_delete_stmt(
+            model=model,
+            filters=filters,
+        )
+
+        sequence = session.execute(stmt).unique().scalars().all()
+
+        if len(sequence) == 0:
+            return False
+
+        if flush:
+            session.flush()
+        if commit:
+            session.commit()
+
+        return True
+
+    @with_session()
+    def _delete(
+        self,
+        model: Type[_T],
+        filters: Optional[_FilterType] = None,
+        flush: bool = True,
+        commit: bool = False,
+        session: Optional[Session] = None,
+    ) -> bool:
+        """
+        Deletes a single object from the database.
+
+        Args:
+            model: The model class representing the table.
+            filters: The filters to apply.
+            flush: Whether to flush the session after the deletion.
+            commit: Whether to commit the session after the deletion.
+            session: The session to use.
+
+        Returns:
+            True if the object was deleted, False otherwise.
+        """
+        stmt = _build_delete_stmt(
+            model=model,
+            filters=filters,
+        )
+
+        item = session.execute(stmt).unique().scalar_one_or_none()
+
+        if item is None:
+            return False
+
+        if flush:
+            session.flush()
+        if commit:
+            session.commit()
+
+        return True
```

### Comparing `pysql-repo-0.5.9/pysql_repo/asyncio/async_decorator.py` & `pysql-repo-0.6.0/pysql_repo/asyncio/async_decorator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,30 @@
 # SQLALCHEMY
 from sqlalchemy.ext.asyncio import AsyncSession
 
-# _CONSTANTS
-from pysql_repo._constants.constants import _PARAM_SESSION
-
 
 def with_async_session(
-    param_session: str = _PARAM_SESSION,
+    param_session: str = "session",
 ):
+    """
+    Decorator that provides an async session to the decorated method.
+    If the session is not provided as a keyword argument, it creates a new session using the session manager.
+    The session is then passed as a keyword argument to the decorated method.
+
+    Args:
+        param_session (str, optional): The name of the session parameter. Defaults to "session".
+
+    Raises:
+        TypeError: If the decorated object is not an instance of AsyncRepository or AsyncService.
+        TypeError: If the session is not an instance of AsyncSession.
+
+    Returns:
+        Callable: The decorated method.
+    """
+
     def decorator(func):
         async def wrapper(self, *args, **kwargs):
             if not isinstance(self, (AsyncRepository, AsyncService)):
                 raise TypeError(
                     f"{self.__class__.__name__} must be instance of {AsyncRepository.__name__} or {AsyncService.__name__}"
                 )
```

### Comparing `pysql-repo-0.5.9/pysql_repo.egg-info/PKG-INFO` & `pysql-repo-0.6.0/pysql_repo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysql-repo
-Version: 0.5.9
+Version: 0.6.0
 Summary: A project to have a base repository class to perform select/insert/update/delete with dynamic syntax
 Home-page: https://github.com/Impro02/pysql-repo
-Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.5.9.tar.gz
+Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.6.0.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -595,16 +595,16 @@
     def __init__(
         self,
         user_repository: UserRepository,
         logger: Logger,
     ) -> None:
         super().__init__(
             repository=user_repository,
-            logger=logger,
         )
+        self._logger = logger
 
     @with_session()
     def get_users(
         self,
         ids_in: Optional[List[int]] = None,
         ids_not_in: Optional[List[int]] = None,
         emails_iin: Optional[List[str]] = None,
@@ -1163,16 +1163,16 @@
     def __init__(
         self,
         user_repository: AsyncUserRepository,
         logger: Logger,
     ) -> None:
         super().__init__(
             repository=user_repository,
-            logger=logger,
         )
+        self._logger = logger
 
     @with_async_session()
     async def get_users(
         self,
         session: Optional[AsyncSession] = None,
         ids_in: Optional[List[int]] = None,
         ids_not_in: Optional[List[int]] = None,
```

### Comparing `pysql-repo-0.5.9/pysql_repo.egg-info/SOURCES.txt` & `pysql-repo-0.6.0/pysql_repo.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 pysql_repo/_service.py
 pysql_repo/_utils.py
 pysql_repo.egg-info/PKG-INFO
 pysql_repo.egg-info/SOURCES.txt
 pysql_repo.egg-info/dependency_links.txt
 pysql_repo.egg-info/requires.txt
 pysql_repo.egg-info/top_level.txt
-pysql_repo/_constants/constants.py
 pysql_repo/_constants/enum.py
 pysql_repo/asyncio/__init__.py
 pysql_repo/asyncio/async_database.py
 pysql_repo/asyncio/async_decorator.py
 pysql_repo/asyncio/async_repository.py
 pysql_repo/asyncio/async_service.py
 pysql_repo/libs/file_lib.py
```

### Comparing `pysql-repo-0.5.9/setup.py` & `pysql-repo-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.5.9"
+version = "0.6.0"
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="pysql-repo",
     version=version,
```

