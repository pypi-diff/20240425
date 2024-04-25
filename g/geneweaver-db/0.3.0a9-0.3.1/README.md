# Comparing `tmp/geneweaver_db-0.3.0a9.tar.gz` & `tmp/geneweaver_db-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneweaver_db-0.3.0a9.tar", max compression
+gzip compressed data, was "geneweaver_db-0.3.1.tar", max compression
```

## Comparing `geneweaver_db-0.3.0a9.tar` & `geneweaver_db-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,39 @@
--rw-r--r--   0        0        0    11356 2024-02-29 15:51:18.452181 geneweaver_db-0.3.0a9/LICENSE
--rw-r--r--   0        0        0      828 2024-02-29 15:51:18.452181 geneweaver_db-0.3.0a9/README.md
--rw-r--r--   0        0        0      932 2024-02-29 15:51:18.452181 geneweaver_db-0.3.0a9/pyproject.toml
--rw-r--r--   0        0        0       51 2024-02-29 15:51:18.452181 geneweaver_db-0.3.0a9/src/geneweaver/db/__init__.py
--rw-r--r--   0        0        0       46 2024-02-29 15:51:18.452181 geneweaver_db-0.3.0a9/src/geneweaver/db/aio/__init__.py
--rw-r--r--   0        0        0     3354 2024-02-29 15:51:18.452181 geneweaver_db-0.3.0a9/src/geneweaver/db/aio/gene.py
--rw-r--r--   0        0        0     1743 2024-02-29 15:51:18.452181 geneweaver_db-0.3.0a9/src/geneweaver/db/aio/publication.py
--rw-r--r--   0        0        0     1309 2024-02-29 15:51:18.452181 geneweaver_db-0.3.0a9/src/geneweaver/db/aio/species.py
--rw-r--r--   0        0        0       56 2024-02-29 15:51:18.452181 geneweaver_db-0.3.0a9/src/geneweaver/db/core/__init__.py
--rw-r--r--   0        0        0      144 2024-02-29 15:51:18.452181 geneweaver_db-0.3.0a9/src/geneweaver/db/core/settings.py
--rw-r--r--   0        0        0     1768 2024-02-29 15:51:18.452181 geneweaver_db-0.3.0a9/src/geneweaver/db/core/settings_class.py
--rw-r--r--   0        0        0      437 2024-02-29 15:51:18.452181 geneweaver_db-0.3.0a9/src/geneweaver/db/exceptions.py
--rw-r--r--   0        0        0    10536 2024-02-29 15:51:18.456181 geneweaver_db-0.3.0a9/src/geneweaver/db/gene.py
--rw-r--r--   0        0        0     8023 2024-02-29 15:51:18.456181 geneweaver_db-0.3.0a9/src/geneweaver/db/geneset.py
--rw-r--r--   0        0        0     7886 2024-02-29 15:51:18.456181 geneweaver_db-0.3.0a9/src/geneweaver/db/geneset_value.py
--rw-r--r--   0        0        0     1640 2024-02-29 15:51:18.456181 geneweaver_db-0.3.0a9/src/geneweaver/db/publication.py
--rw-r--r--   0        0        0       42 2024-02-29 15:51:18.456181 geneweaver_db-0.3.0a9/src/geneweaver/db/query/__init__.py
--rw-r--r--   0        0        0     3919 2024-02-29 15:51:18.456181 geneweaver_db-0.3.0a9/src/geneweaver/db/query/gene.py
--rw-r--r--   0        0        0     2343 2024-02-29 15:51:18.456181 geneweaver_db-0.3.0a9/src/geneweaver/db/query/publication.py
--rw-r--r--   0        0        0     1498 2024-02-29 15:51:18.456181 geneweaver_db-0.3.0a9/src/geneweaver/db/query/species.py
--rw-r--r--   0        0        0     1248 2024-02-29 15:51:18.456181 geneweaver_db-0.3.0a9/src/geneweaver/db/species.py
--rw-r--r--   0        0        0     6886 2024-02-29 15:51:18.456181 geneweaver_db-0.3.0a9/src/geneweaver/db/user.py
--rw-r--r--   0        0        0     3084 2024-02-29 15:51:18.456181 geneweaver_db-0.3.0a9/src/geneweaver/db/utils.py
--rw-r--r--   0        0        0     1642 1970-01-01 00:00:00.000000 geneweaver_db-0.3.0a9/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2162 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/README.md
+-rw-r--r--   0        0        0      953 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      156 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/__init__.py
+-rw-r--r--   0        0        0      132 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/aio/__init__.py
+-rw-r--r--   0        0        0     3134 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/aio/gene.py
+-rw-r--r--   0        0        0     4802 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/aio/geneset.py
+-rw-r--r--   0        0        0     2189 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/aio/publication.py
+-rw-r--r--   0        0        0     1310 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/aio/species.py
+-rw-r--r--   0        0        0      692 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/aio/threshold.py
+-rw-r--r--   0        0        0       56 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/core/__init__.py
+-rw-r--r--   0        0        0      845 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/core/cursor.py
+-rw-r--r--   0        0        0      145 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/core/settings.py
+-rw-r--r--   0        0        0     1769 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/core/settings_class.py
+-rw-r--r--   0        0        0      438 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/exceptions.py
+-rw-r--r--   0        0        0    10316 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/gene.py
+-rw-r--r--   0        0        0     8651 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/geneset.py
+-rw-r--r--   0        0        0     7887 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/geneset_value.py
+-rw-r--r--   0        0        0     2063 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/publication.py
+-rw-r--r--   0        0        0       42 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/query/__init__.py
+-rw-r--r--   0        0        0     4859 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/query/gene.py
+-rw-r--r--   0        0        0      364 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/query/geneset/__init__.py
+-rw-r--r--   0        0        0     1351 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/query/geneset/const.py
+-rw-r--r--   0        0        0     4638 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/query/geneset/read.py
+-rw-r--r--   0        0        0     3928 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/query/geneset/utils.py
+-rw-r--r--   0        0        0     4014 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/query/geneset/write.py
+-rw-r--r--   0        0        0      982 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/query/project.py
+-rw-r--r--   0        0        0     4683 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/query/publication.py
+-rw-r--r--   0        0        0       60 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/query/search/__init__.py
+-rw-r--r--   0        0        0       50 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/query/search/search.py
+-rw-r--r--   0        0        0     1571 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/query/search/utils.py
+-rw-r--r--   0        0        0     1603 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/query/species.py
+-rw-r--r--   0        0        0     1959 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/query/threshold.py
+-rw-r--r--   0        0        0     1776 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/query/utils.py
+-rw-r--r--   0        0        0     1249 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/species.py
+-rw-r--r--   0        0        0      664 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/threshold.py
+-rw-r--r--   0        0        0     6887 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/user.py
+-rw-r--r--   0        0        0     3085 2024-04-25 14:09:17.499545 geneweaver_db-0.3.1/src/geneweaver/db/utils.py
+-rw-r--r--   0        0        0     2982 1970-01-01 00:00:00.000000 geneweaver_db-0.3.1/PKG-INFO
```

### Comparing `geneweaver_db-0.3.0a9/LICENSE` & `geneweaver_db-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.0a9/pyproject.toml` & `geneweaver_db-0.3.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 [tool.poetry]
 name = "geneweaver-db"
-version = "0.3.0a9"
+version = "0.3.1"
 description = "Database Interaction Services for GeneWeaver"
 authors = ["Jax Computational Sciences <cssc@jax.org>"]
 readme = "README.md"
 license = "Apache-2.0"
-homepage = "https://bergsalex.github.io/geneweaver-docs/"
-repository = "https://bitbucket.org/jacksonlaboratory/geneweaver-db"
+homepage = "https://thejacksonlaboratory.github.io/geneweaver-docs/"
+repository = "https://github.com/TheJacksonLaboratory/geneweaver-db"
 packages = [
     { include = "geneweaver/db", from = "src" },
 ]
 
-
 [tool.poetry.dependencies]
 python = "^3.9"
-geneweaver-core = "^0.9.0a5"
+geneweaver-core = ">=0.9.1,<1.0.0"
 psycopg = {extras = ["binary"], version = "^3.1.13"}
 
-
 [tool.poetry.group.dev.dependencies]
-geneweaver-testing = "^0.0.3"
+geneweaver-testing = ">=0.1.2,<1.0.0"
 pytest-asyncio = "^0.23.5"
 
 [tool.ruff]
 select = ['F', 'E', 'W', 'A', 'C90', 'N', 'B', 'ANN', 'D', 'I', 'ERA', 'PD', 'NPY', 'PT']
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["ANN001", "ANN201"]
```

### Comparing `geneweaver_db-0.3.0a9/src/geneweaver/db/aio/gene.py` & `geneweaver_db-0.3.1/src/geneweaver/db/aio/gene.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Database interaction code relating to Gene IDs."""
+
 from typing import List, Optional
 
 from geneweaver.core.enum import GeneIdentifier, Species
 from geneweaver.db.query import gene as gene_query
 from psycopg import AsyncCursor, rows
 
 
@@ -40,32 +41,26 @@
 
     return await cursor.fetchall()
 
 
 async def get_preferred(
     cursor: AsyncCursor,
     gene_id: int,
-    limit: Optional[int] = None,
-    offset: Optional[int] = None,
 ) -> Optional[rows.Row]:
     """Get the preferred gene from the database for a given ode_id.
 
     :param cursor: An async database cursor.
     :param gene_id: The id of the gene to get.
-    :param limit: The limit of results to return.
-    :param offset: The offset of results to return.
 
     :return: The preferred gene using `.fetchone()`
     """
     await cursor.execute(
         *gene_query.get(
             gene_id=gene_id,
             preferred=True,
-            limit=limit,
-            offset=offset,
         )
     )
 
     return await cursor.fetchone()
 
 
 async def mapping(
```

### Comparing `geneweaver_db-0.3.0a9/src/geneweaver/db/aio/publication.py` & `geneweaver_db-0.3.1/src/geneweaver/db/aio/publication.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """Database code for interacting with Publication table."""
+
 from typing import Iterable, List, Optional
 
+from geneweaver.core.schema.publication import PublicationInfo
 from geneweaver.db.query import publication as publication_query
 from psycopg import AsyncCursor, rows
 
 
-async def by_pubmed_id(cursor: AsyncCursor, pubmed_id: str) -> Optional[rows.Row]:
+async def by_pubmed_id(cursor: AsyncCursor, pubmed_id: int) -> Optional[rows.Row]:
     """Get a publication by PubMed ID.
 
     :param cursor: The database cursor.
     :param pubmed_id: The PubMed ID to search for.
 
     :return: optional row using `.fetchone()`
     """
     await cursor.execute(*publication_query.by_pubmed_id(pubmed_id))
     return await cursor.fetchone()
 
 
 async def by_pubmed_ids(
-    cursor: AsyncCursor, pubmed_ids: Iterable[str]
+    cursor: AsyncCursor, pubmed_ids: Iterable[int]
 ) -> List[rows.Row]:
     """Get publications by a list of PubMed IDs.
 
     :param cursor: The database cursor.
     :param pubmed_ids: The PubMed IDs to search for.
 
     :return: list of results using `.fetchall()`
@@ -49,7 +51,19 @@
     :param cursor: The database cursor.
     :param geneset_id: The geneset ID to search for.
 
     :return: optional row using `.fetchone()`
     """
     await cursor.execute(*publication_query.by_geneset_id(geneset_id))
     return await cursor.fetchone()
+
+
+async def add(cursor: AsyncCursor, publication: PublicationInfo) -> Optional[rows.Row]:
+    """Add a publication to the database.
+
+    :param cursor: The database cursor.
+    :param publication: The publication to add.
+
+    :return: optional row using `.fetchone()`
+    """
+    await cursor.execute(*publication_query.add(**publication.dict()))
+    return await cursor.fetchone()
```

### Comparing `geneweaver_db-0.3.0a9/src/geneweaver/db/aio/species.py` & `geneweaver_db-0.3.1/src/geneweaver/db/aio/species.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Species database functions."""
+
 from typing import List, Optional
 
 from geneweaver.core.enum import GeneIdentifier, Species
 from geneweaver.db.query import species as species_query
 from psycopg import AsyncCursor, rows
```

### Comparing `geneweaver_db-0.3.0a9/src/geneweaver/db/core/settings_class.py` & `geneweaver_db-0.3.1/src/geneweaver/db/core/settings_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 load them from a `.env` file in the root of the project. The following environment
 variables are used:
 GWDB_SERVER=your_server
 GWDB_USERNAME=your_user
 GWDB_PASSWORD=your_password
 GWDB_NAME=your_database_name
 """
+
 # ruff: noqa: N805, ANN101, ANN401
 from typing import Any, Dict, Optional
 
 from pydantic import BaseSettings, PostgresDsn, validator
 
 
 class Settings(BaseSettings):
```

### Comparing `geneweaver_db-0.3.0a9/src/geneweaver/db/gene.py` & `geneweaver_db-0.3.1/src/geneweaver/db/gene.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Database interaction code relating to Gene IDs."""
+
 from typing import Iterable, List, Optional
 
 from geneweaver.core.enum import GeneIdentifier, Species
 from geneweaver.db.query import gene as gene_query
 from psycopg import Cursor, rows
 from psycopg.sql import SQL
 
@@ -41,32 +42,26 @@
 
     return cursor.fetchall()
 
 
 def get_preferred(
     cursor: Cursor,
     gene_id: int,
-    limit: Optional[int] = None,
-    offset: Optional[int] = None,
 ) -> Optional[rows.Row]:
     """Get the preferred gene from the database for a given ode_id.
 
     :param cursor: The database cursor.
     :param gene_id: The id of the gene to get.
-    :param limit: The limit of results to return.
-    :param offset: The offset of results to return.
 
     :return: The preferred gene using `.fetchone()`
     """
     cursor.execute(
         *gene_query.get(
             gene_id=gene_id,
             preferred=True,
-            limit=limit,
-            offset=offset,
         )
     )
 
     return cursor.fetchone()
 
 
 def mapping(
```

### Comparing `geneweaver_db-0.3.0a9/src/geneweaver/db/geneset.py` & `geneweaver_db-0.3.1/src/geneweaver/db/geneset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,141 +1,157 @@
 """Geneset database functions."""
+
 from typing import List, Optional
 
-from geneweaver.db.query.publication import PUB_FIELD_MAP
-from geneweaver.db.utils import format_sql_fields, temp_override_row_factory
+from geneweaver.core.enum import GeneIdentifier, GenesetTier, Species
+from geneweaver.db.query import geneset as geneset_query
+from geneweaver.db.utils import temp_override_row_factory
 from psycopg import Cursor, rows
-from psycopg.sql import SQL, Composed
-
-GENESET_FIELDS_MAP = {
-    "gs_id": "id",
-    "usr_id": "user_id",
-    "file_id": "file_id",
-    "cur_id": "curation_id",
-    "sp_id": "species_id",
-    "gs_name": "name",
-    "gs_abbreviation": "abbreviation",
-    "pub_id": "publication_id",
-    "gs_description": "description",
-    "gs_count": "count",
-    "gs_threshold_type": "score_type",
-    "gs_threshold": "threshold",
-    "gs_status": "status",
-    "gs_gene_id_type": "gene_id_type",
-    "gs_attribution": "attribution",
-    "gs_created": "created",
-    "gs_updated": "updated",
-}
-
-GENESET_FIELDS = format_sql_fields(GENESET_FIELDS_MAP, query_table="geneset")
-PUB_FIELDS = format_sql_fields(
-    PUB_FIELD_MAP, query_table="publication", resp_prefix="publication"
-)
+from psycopg.rows import Row
 
 
-def _format_geneset_query(with_publication_info: bool = False) -> Composed:
-    """Format the geneset query.
+def get(
+    cursor: Cursor,
+    is_readable_by: Optional[int] = None,
+    gs_id: Optional[int] = None,
+    owner_id: Optional[int] = None,
+    curation_tier: Optional[GenesetTier] = None,
+    species: Optional[Species] = None,
+    name: Optional[str] = None,
+    abbreviation: Optional[str] = None,
+    publication_id: Optional[int] = None,
+    pubmed_id: Optional[int] = None,
+    gene_id_type: Optional[GeneIdentifier] = None,
+    search_text: Optional[str] = None,
+    limit: Optional[int] = None,
+    offset: Optional[int] = None,
+    with_publication_info: bool = True,
+) -> List[Row]:
+    """Get genesets from the database.
+
+    :param cursor: An async database cursor.
+    :param is_readable_by: A user ID to check if the user can read the results.
+    :param gs_id: Show only results with this geneset ID.
+    :param owner_id: Show only results owned by this user ID.
+    :param curation_tier: Show only results of this curation tier.
+    :param species: Show only results associated with this species.
+    :param name: Show only results with this name.
+    :param abbreviation: Show only results with this abbreviation.
+    :param publication_id: Show only results with this publication ID (internal).
+    :param pubmed_id: Show only results with this PubMed ID.
+    :param gene_id_type: Show only results with this gene ID type.
+    :param search_text: Return genesets that match this search text (using PostgreSQL
+                        full-text search).
+    :param limit: Limit the number of results.
+    :param offset: Offset the results.
+    :param with_publication_info: Include publication info in the return.
 
-    :param with_publication_info: Whether to include publication info.
-
-    :return: The formatted query.
+    :return: list of results using `.fetchall()`
     """
-    query = SQL("SELECT")
-    if with_publication_info:
-        query = (
-            query
-            + SQL(",").join(GENESET_FIELDS + PUB_FIELDS)
-            + SQL("FROM geneset LEFT OUTER JOIN publication")
-            + SQL("ON geneset.pub_id = publication.pub_id")
+    cursor.execute(
+        *geneset_query.get(
+            is_readable_by=is_readable_by,
+            gs_id=gs_id,
+            owner_id=owner_id,
+            curation_tier=curation_tier,
+            species=species,
+            name=name,
+            abbreviation=abbreviation,
+            publication_id=publication_id,
+            pubmed_id=pubmed_id,
+            gene_id_type=gene_id_type,
+            search_text=search_text,
+            limit=limit,
+            offset=offset,
+            with_publication_info=with_publication_info,
         )
-    else:
-        query = query + SQL(",").join(GENESET_FIELDS) + SQL("FROM geneset")
-    return query
-
-
-def by_id(
-    cursor: Cursor, geneset_id: int, with_publication_info: bool = False
-) -> Optional[rows.Row]:
-    """Get geneset info by geneset id.
-
-    :param cursor: The database cursor.
-    :param geneset_id: The geneset id to search for.
-    :param with_publication_info: Whether to include publication info.
-
-    :return: optional row using `.fetchone()`
-    """
-    query = _format_geneset_query(with_publication_info=with_publication_info)
-    query = (query + SQL("WHERE gs_id = %(geneset_id)s")).join(" ")
-    cursor.execute(query, {"geneset_id": geneset_id})
-    return cursor.fetchone()
+    )
 
+    return cursor.fetchall()
 
-def by_user_id(
-    cursor: Cursor, user_id: int, with_publication_info: bool = False
-) -> List[rows.Row]:
-    """Get geneset info by user id.
 
-    :param cursor: The database cursor.
-    :param user_id: The user id (internal) to search for.
-    :param with_publication_info: Whether to include publication info.
-
-    :return: list of results using `.fetchall()`
+def by_id(
+    cursor: Cursor,
+    gs_id: int,
+    is_readable_by: Optional[int] = None,
+    with_publication_info: bool = True,
+) -> Optional[Row]:
+    """Get a geneset by its ID.
+
+    :param cursor: A database cursor.
+    :param gs_id: The geneset ID to search for.
+    :param is_readable_by: A user ID to check if the user can read the results.
+    :param with_publication_info: Include publication info in the return.
     """
-    query = _format_geneset_query(with_publication_info=with_publication_info)
-    query = (query + SQL("WHERE usr_id = %(user_id)s")).join(" ")
-    cursor.execute(query, {"user_id": user_id})
-    return cursor.fetchall()
+    cursor.execute(
+        *geneset_query.get(
+            gs_id=gs_id,
+            is_readable_by=is_readable_by,
+            with_publication_info=with_publication_info,
+        )
+    )
 
+    return cursor.fetchone()
 
-def by_project_id(cursor: Cursor, project_id: int) -> List:
-    """Get geneset info by project id.
 
-    :param cursor: The database cursor.
-    :param project_id: The project id to search for.
+def by_owner_id(
+    cursor: Cursor,
+    owner_id: int,
+    is_readable_by: Optional[int] = None,
+    with_publication_info: bool = True,
+) -> List[Row]:
+    """Get genesets by owner ID.
+
+    :param cursor: A database cursor.
+    :param owner_id: The owner ID to search for.
+    :param is_readable_by: A user ID to check if the user can read the results.
+    :param with_publication_info: Include publication info in the return.
 
     :return: list of results using `.fetchall()`
     """
     cursor.execute(
-        """
-        -- selects all genesets for the given project ID
-        SELECT geneset.*
-        FROM production.geneset INNER JOIN production.project2geneset
-        ON geneset.gs_id=project2geneset.gs_id
-        WHERE project2geneset.pj_id=%(project_id)s
-        """,
-        {"project_id": project_id},
+        *geneset_query.get(
+            owner_id=owner_id,
+            is_readable_by=is_readable_by,
+            with_publication_info=with_publication_info,
+        )
     )
     return cursor.fetchall()
 
 
-def by_project_id_and_user_id(cursor: Cursor, project_id: int, user_id: int) -> List:
-    """Get geneset info by project id.
-
-    :param cursor: The database cursor.
-    :param project_id: The project id to search for.
-    :param user_id: The user id (internal) to limit results to.
+def by_project_id(
+    cursor: Cursor,
+    project_id: int,
+    is_readable_by: Optional[int] = None,
+    with_publication_info: bool = True,
+) -> List[Row]:
+    """Get a list of genesets by their membership in a project.
+
+    :param cursor: An async database cursor.
+    :param project_id: The project ID to search for.
+    :param is_readable_by: A user ID to check if the user can read the results.
+    :param with_publication_info: Include publication info in the return.
 
     :return: list of results using `.fetchall()`
     """
     cursor.execute(
-        """
-        -- selects all genesets for the given project ID
-        SELECT geneset.*
-        FROM production.geneset INNER JOIN production.project2geneset
-        ON geneset.gs_id=project2geneset.gs_id
-        WHERE project2geneset.pj_id=%(project_id)s
-            -- security check: make sure the authenticated user has the
-            -- right to view the geneset
-        AND production.geneset_is_readable2(%(user_id)s, geneset.gs_id);
-        """,
-        {"project_id": project_id, "user_id": user_id},
+        *geneset_query.by_project_id(
+            project_id=project_id,
+            is_readable_by=is_readable_by,
+            with_publication_info=with_publication_info,
+        )
     )
     return cursor.fetchall()
 
 
+# --------------------------------------------------------------------------------------
+# The following functions are not yet implemented in the aio/concurrent paradigm.
+# They are subject to change and may be deprecated in the future.
+
+
 @temp_override_row_factory(rows.tuple_row)
 def is_readable(cursor: Cursor, user_id: int, geneset_id: int) -> bool:
     """Check if a geneset is readable by a user.
 
     :param cursor: The database cursor.
     :param user_id: The user id (internal) to check.
     :param geneset_id: The geneset id to check.
```

### Comparing `geneweaver_db-0.3.0a9/src/geneweaver/db/geneset_value.py` & `geneweaver_db-0.3.1/src/geneweaver/db/geneset_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Database functions for geneset values."""
+
 from typing import List, Optional
 
 from geneweaver.core.enum import GeneIdentifier
 from geneweaver.core.schema.batch import GenesetValueInput
 from geneweaver.db.exceptions import GeneweaverTypeError
 from psycopg import Cursor
```

### Comparing `geneweaver_db-0.3.0a9/src/geneweaver/db/publication.py` & `geneweaver_db-0.3.1/src/geneweaver/db/publication.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """Database code for interacting with Publication table."""
+
 from typing import Iterable, List, Optional
 
+from geneweaver.core.schema.publication import PublicationInfo
 from geneweaver.db.query import publication as publication_query
 from psycopg import Cursor, rows
 
 
-def by_pubmed_id(cursor: Cursor, pubmed_id: str) -> Optional[rows.Row]:
+def by_pubmed_id(cursor: Cursor, pubmed_id: int) -> Optional[rows.Row]:
     """Get a publication by PubMed ID.
 
     :param cursor: The database cursor.
     :param pubmed_id: The PubMed ID to search for.
 
     :return: optional row using `.fetchone()`
     """
     cursor.execute(*publication_query.by_pubmed_id(pubmed_id))
     return cursor.fetchone()
 
 
-def by_pubmed_ids(cursor: Cursor, pubmed_ids: Iterable[str]) -> List[rows.Row]:
+def by_pubmed_ids(cursor: Cursor, pubmed_ids: Iterable[int]) -> List[rows.Row]:
     """Get publications by a list of PubMed IDs.
 
     :param cursor: The database cursor.
     :param pubmed_ids: The PubMed IDs to search for.
 
     :return: list of results using `.fetchall()`
     """
@@ -47,7 +49,19 @@
     :param cursor: The database cursor.
     :param geneset_id: The geneset ID to search for.
 
     :return: optional row using `.fetchone()`
     """
     cursor.execute(*publication_query.by_geneset_id(geneset_id))
     return cursor.fetchone()
+
+
+def add(cursor: Cursor, publication: PublicationInfo) -> Optional[rows.Row]:
+    """Add a publication to the database.
+
+    :param cursor: The database cursor.
+    :param publication: The publication to add.
+
+    :return: optional row using `.fetchone()`
+    """
+    cursor.execute(*publication_query.add(**publication.dict()))
+    return cursor.fetchone()
```

### Comparing `geneweaver_db-0.3.0a9/src/geneweaver/db/query/gene.py` & `geneweaver_db-0.3.1/src/geneweaver/db/query/gene.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Generate SQL queries to get Gene information."""
+
 from typing import List, Optional, Tuple
 
 from geneweaver.core.enum import GeneIdentifier, Species
 from geneweaver.core.mapping import AON_ID_TYPE_FOR_SPECIES
 from geneweaver.db.utils import format_sql_fields, limit_and_offset
 from psycopg.sql import SQL, Composed
 
@@ -80,29 +81,60 @@
     """Create a query to get a list of gene IDs in an alternate identifier type.
 
     :param source_ids: The list of gene IDs to map.
     :param target_gene_id_type: The gene identifier type to map to.
     :param species: The species of the identifiers.
     :return: A query (and params) that can be executed on a cursor.
     """
-    params = {}
     query = (
-        SQL("SELECT g1.ode_ref_id AS original_ref_id, g2.ode_ref_id AS mapped_ref_id")
-        + SQL("FROM gene g1 JOIN gene g2")
-        + SQL("ON g1.ode_gene_id = g2.ode_gene_id")
-        + SQL("AND g1.ode_ref_id != g2.ode_ref_id")
-        + SQL("AND g1.sp_id = g2.sp_id")
-        + SQL("WHERE g1.ode_ref_id = ANY(%(source_ids)s)")
-        + SQL("AND g2.gdb_id = %(target_gene_id_type)s")
-        + SQL("AND g2.sp_id = %(species_id)s")
-        + SQL("AND g2.ode_pref = TRUE")
+        SQL(
+            """
+    WITH PrefTrueCheck AS
+        (SELECT CASE
+                WHEN EXISTS(SELECT 1
+                            FROM extsrc.gene AS g1
+                                   JOIN extsrc.gene AS g2
+                                        ON g1.ode_gene_id = g2.ode_gene_id
+                                        AND g1.ode_ref_id != g2.ode_ref_id
+                                        AND g1.sp_id = g2.sp_id
+                             WHERE g1.ode_ref_id = ANY(%(source_ids)s)
+                               AND g2.gdb_id = %(target_gene_id_type)s
+                               AND g2.sp_id = %(species_id)s
+                               AND g2.ode_pref = True)
+                  THEN True ELSE False
+                  END AS PrefExists)
+    """
+        )
+        + SQL(
+            """
+    SELECT g1.ode_ref_id AS original_ref_id,
+           g2.ode_ref_id AS mapped_ref_id
+    FROM extsrc.gene AS g1
+             JOIN extsrc.gene AS g2
+                  ON g1.ode_gene_id = g2.ode_gene_id
+                  AND g1.ode_ref_id != g2.ode_ref_id
+                  AND g1.sp_id = g2.sp_id,
+         PrefTrueCheck
+    WHERE g1.ode_ref_id = ANY (%(source_ids)s)
+      AND g2.gdb_id = %(target_gene_id_type)s
+      AND g2.sp_id = %(species_id)s
+      AND (
+        (PrefTrueCheck.PrefExists AND g2.ode_pref = True)
+            OR
+        (NOT PrefTrueCheck.PrefExists)
+        );
+    """
+        )
     ).join(" ")
-    params["source_ids"] = source_ids
-    params["target_gene_id_type"] = int(target_gene_id_type)
-    params["species_id"] = int(species)
+
+    params = {
+        "source_ids": source_ids,
+        "target_gene_id_type": int(target_gene_id_type),
+        "species_id": int(species),
+    }
     return query, params
 
 
 def aon_mapping(
     source_ids: List[str],
     species: Species,
 ) -> Tuple[Composed, dict]:
```

### Comparing `geneweaver_db-0.3.0a9/src/geneweaver/db/query/species.py` & `geneweaver_db-0.3.1/src/geneweaver/db/query/species.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Generate SQL queries to get Species information."""
+
 from typing import Optional, Tuple
 
 from geneweaver.core.enum import GeneIdentifier, Species
 from geneweaver.db.utils import format_sql_fields
 from psycopg.sql import SQL, Composed
 
 SPECIES_FIELD_MAP = {
@@ -28,22 +29,27 @@
     :param species: The species id.
 
     :return: A query (and params) that can be executed on a cursor.
     """
     params = {}
     query = SQL("SELECT") + SQL(",").join(SPECIES_FIELDS) + SQL("FROM species")
 
+    filters = []
+
     if species:
-        query += SQL("WHERE sp_id = %(species_id)s")
+        filters.append(SQL("sp_id = %(species_id)s"))
         params["species_id"] = int(species)
 
     if taxonomic_id:
-        query += SQL("WHERE sp_taxid = %(taxonomic_id)s")
+        filters.append(SQL("sp_taxid = %(taxonomic_id)s"))
         params["taxonomic_id"] = taxonomic_id
 
     if reference_gene_db_id:
-        query += SQL("WHERE sp_ref_gdb_id = %(reference_gene_db_id)s")
+        filters.append(SQL("sp_ref_gdb_id = %(reference_gene_db_id)s"))
         params["reference_gene_db_id"] = int(reference_gene_db_id)
 
+    if len(filters) > 0:
+        query += SQL("WHERE") + SQL("AND").join(filters)
+
     query = query.join(" ")
 
     return query, params
```

### Comparing `geneweaver_db-0.3.0a9/src/geneweaver/db/species.py` & `geneweaver_db-0.3.1/src/geneweaver/db/species.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Species database functions."""
+
 from typing import List, Optional
 
 from geneweaver.core.enum import GeneIdentifier, Species
 from geneweaver.db.query import species as species_query
 from psycopg import Cursor, rows
```

### Comparing `geneweaver_db-0.3.0a9/src/geneweaver/db/user.py` & `geneweaver_db-0.3.1/src/geneweaver/db/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 - by_user_id
 - by_email
 
 The functions that return a single value from a user record are:
 - user_id_from_api_key
 - user_id_from_sso_id
 """
+
 from typing import List, Optional
 
 from geneweaver.db.utils import temp_override_row_factory
 from psycopg import Cursor, rows
 
 
 @temp_override_row_factory(rows.tuple_row)
```

### Comparing `geneweaver_db-0.3.0a9/src/geneweaver/db/utils.py` & `geneweaver_db-0.3.1/src/geneweaver/db/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for the GeneWeaver database functions."""
+
 # ruff: noqa: ANN001, ANN002, ANN003, ANN201, ANN202
 import functools
 from typing import List, Optional
 
 from geneweaver.db.exceptions import GeneweaverDoesNotExistError, GeneweaverValueError
 from psycopg import sql
 from psycopg.rows import Row
```

