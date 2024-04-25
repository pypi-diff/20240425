# Comparing `tmp/taegis_magic-2023.9.15.tar.gz` & `tmp/taegis_magic-2024.3.29.tar.gz`

## Comparing `taegis_magic-2023.9.15.tar` & `taegis_magic-2024.3.29.tar`

### file list

```diff
@@ -1,41 +1,44 @@
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/__init__.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/_version.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/cli.py
--rw-r--r--   0        0        0     6903 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/magics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/commands/__init__.py
--rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/commands/alerts.py
--rw-r--r--   0        0        0     8066 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/commands/audits.py
--rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/commands/clients.py
--rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/commands/configure.py
--rw-r--r--   0        0        0     8309 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/commands/events.py
--rw-r--r--   0        0        0    18711 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/commands/investigations.py
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/commands/preferences.py
--rw-r--r--   0        0        0    16102 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/commands/rules.py
--rw-r--r--   0        0        0    24939 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/commands/tenant_profiles.py
--rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/commands/tenants.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/commands/threat.py
--rw-r--r--   0        0        0     7336 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/commands/users.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/commands/utils/__init__.py
--rw-r--r--   0        0        0    14693 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/commands/utils/investigations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/core/__init__.py
--rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/core/cache.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/core/callbacks.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/core/log.py
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/core/normalizer.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/core/queries.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/core/service.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/core/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/pandas/__init__.py
--rw-r--r--   0        0        0    12891 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/pandas/alerts.py
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/pandas/audits.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/pandas/rules.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/pandas/tenants.py
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/pandas/utils.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/templates/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/templates/taegis_results.md.jinja
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/taegis_magic/templates/taegis_search_results.md.jinja
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/.gitignore
--rw-r--r--   0        0        0    10173 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/LICENSE
--rw-r--r--   0        0        0     6284 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/README.md
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/pyproject.toml
--rw-r--r--   0        0        0    19202 2020-02-02 00:00:00.000000 taegis_magic-2023.9.15/PKG-INFO
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/__init__.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/_version.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/cli.py
+-rw-r--r--   0        0        0     6903 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/magics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/__init__.py
+-rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/alerts.py
+-rw-r--r--   0        0        0     8066 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/audits.py
+-rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/clients.py
+-rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/configure.py
+-rw-r--r--   0        0        0     8404 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/events.py
+-rw-r--r--   0        0        0    24637 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/investigations.py
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/preferences.py
+-rw-r--r--   0        0        0    16102 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/rules.py
+-rw-r--r--   0        0        0    24939 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/tenant_profiles.py
+-rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/tenants.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/threat.py
+-rw-r--r--   0        0        0     7336 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/users.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/utils/__init__.py
+-rw-r--r--   0        0        0    14693 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/utils/investigations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/core/__init__.py
+-rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/core/cache.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/core/callbacks.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/core/log.py
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/core/normalizer.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/core/queries.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/core/service.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/core/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/pandas/__init__.py
+-rw-r--r--   0        0        0    12891 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/pandas/alerts.py
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/pandas/assets.py
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/pandas/audits.py
+-rw-r--r--   0        0        0    20558 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/pandas/context.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/pandas/events.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/pandas/rules.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/pandas/tenants.py
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/pandas/utils.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/templates/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/templates/taegis_results.md.jinja
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/templates/taegis_search_results.md.jinja
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/.gitignore
+-rw-r--r--   0        0        0    10173 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/LICENSE
+-rw-r--r--   0        0        0     6338 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/README.md
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/pyproject.toml
+-rw-r--r--   0        0        0    19302 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/PKG-INFO
```

### Comparing `taegis_magic-2023.9.15/taegis_magic/cli.py` & `taegis_magic-2024.3.29/taegis_magic/cli.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/taegis_magic/magics.py` & `taegis_magic-2024.3.29/taegis_magic/magics.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/taegis_magic/commands/alerts.py` & `taegis_magic-2024.3.29/taegis_magic/commands/alerts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Taegis Magic alerts commands."""
+
 import logging
 from dataclasses import asdict, dataclass, field
 from pprint import pprint
 from typing import Any, Dict, List, Optional
 
 import typer
 from dataclasses_json import config, dataclass_json
@@ -137,14 +138,18 @@
         log.debug("Calling AlertsResultsNormalizer.query_identifier...")
         if not self.raw_results:
             return None
 
         if self._query_id:
             return self._query_id
 
+        if self.raw_results[0].query_id:
+            self._query_id = self.raw_results[0].query_id
+            return self._query_id
+
         if not self.query:
             raise ValueError("No query found to generate query id")
 
         query_name = "Taegis Query Magic" if self.is_saved else "alert"
         data = {
             "query": None,
             "name": query_name,
@@ -309,14 +314,17 @@
     with service(output=graphql_output):
         result = alerts_service_search_with_events(
             service,
             SearchRequestInput(
                 cql_query=cell,
                 offset=0,
                 limit=limit,
+                metadata={
+                    "callerName": "Taegis Magic",
+                },
             ),
         )
 
     poll_responses = [result]
     search_id = result.search_id
     total_parts = result.alerts.total_parts
```

### Comparing `taegis_magic-2023.9.15/taegis_magic/commands/audits.py` & `taegis_magic-2024.3.29/taegis_magic/commands/audits.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/taegis_magic/commands/clients.py` & `taegis_magic-2024.3.29/taegis_magic/commands/clients.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/taegis_magic/commands/configure.py` & `taegis_magic-2024.3.29/taegis_magic/commands/configure.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/taegis_magic/commands/events.py` & `taegis_magic-2024.3.29/taegis_magic/commands/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Taegis Magic events commands."""
+
 import inspect
 import logging
 from dataclasses import asdict, dataclass, field
 from typing import Any, Dict, List, Optional
 
 import typer
 from dataclasses_json import dataclass_json
@@ -144,18 +145,22 @@
         """
         if not self.raw_results:
             return None
 
         if self._query_id:
             return self._query_id
 
+        if self.raw_results[0].query_id:
+            self._query_id = self.raw_results[0].query_id
+            return self._query_id
+
         if not self.query:
-            raise ValueError("No query found to generate query id")
+            raise None
 
-        query_name = query if self.is_saved else "cql"
+        query_name = self.query if self.is_saved else "cql"
         data = {
             "query": None,
             "name": query_name,
             "description": self.query,
             "query_source": "cql",
             "metadata": [
                 {"id": "start"},
```

### Comparing `taegis_magic-2023.9.15/taegis_magic/commands/investigations.py` & `taegis_magic-2024.3.29/taegis_magic/commands/investigations.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Taegis Magic investigations commands."""
+
 import inspect
 import logging
 import re
 from dataclasses import asdict, dataclass, field
 from enum import Enum
 from pathlib import Path
 from textwrap import dedent
 from typing import Any, Dict, List, Optional, Union
+import mimetypes
+import requests
 
 import typer
 from dataclasses_json import dataclass_json
 from taegis_magic.commands.utils.investigations import (
     InvestigationEvidenceNormalizer,
     InvestigationEvidenceType,
     clear_search_queries,
@@ -21,40 +24,62 @@
     insert_search_query,
     list_search_queries,
     read_database,
     stage_investigation_evidence,
     unstage_investigation_evidence,
 )
 from taegis_magic.core.log import tracing
-from taegis_magic.core.normalizer import DataFrameNormalizer, TaegisResultsNormalizer
-
-from taegis_magic.core.utils import remove_output_node
-from taegis_magic.core.service import get_service
+from taegis_magic.core.normalizer import (
+    DataFrameNormalizer,
+    TaegisResult,
+    TaegisResults,
+    TaegisResultsNormalizer,
+)
 from taegis_magic.core.queries import get_query, update_query
+from taegis_magic.core.service import get_service
+from taegis_magic.core.utils import remove_output_node
+from taegis_magic.core.callbacks import verify_file
 from taegis_sdk_python import build_output_string
 from taegis_sdk_python.services.investigations2.types import (
     CreateInvestigationInput,
     InvestigationStatus,
     InvestigationsV2,
     InvestigationsV2Arguments,
     InvestigationType,
     InvestigationV2,
+    InvestigationFileV2Arguments,
+    InvestigationFilesV2Arguments,
+    DeleteInvestigationFileInput,
+    InitInvestigationFileUploadInput,
 )
+from taegis_sdk_python.services.queries.types import QLQueriesInput
 from taegis_sdk_python.services.sharelinks.types import ShareLinkCreateInput
 from typing_extensions import Annotated
 
 log = logging.getLogger(__name__)
 
 
 app = typer.Typer()
+investigations_attachment = typer.Typer()
 investigations_evidence = typer.Typer()
 investigations_search_queries = typer.Typer()
 
-app.add_typer(investigations_evidence, name="evidence")
-app.add_typer(investigations_search_queries, name="search-queries")
+app.add_typer(
+    investigations_attachment,
+    name="attachment",
+    help="Investigation File Attachment commands.",
+)
+app.add_typer(
+    investigations_evidence, name="evidence", help="Investigation Evidence commands."
+)
+app.add_typer(
+    investigations_search_queries,
+    name="search-queries",
+    help="Investigation Search Query commands.",
+)
 
 
 class InvestigationPriority(str, Enum):
     LOW = "LOW"
     MEDIUM = "MEDIUM"
     HIGH = "HIGH"
     CRITICAL = "CRITICAL"
@@ -374,15 +399,15 @@
     assignee_id: str = "@customer",
     database: str = ":memory:",
     dry_run: bool = False,
     region: Optional[str] = None,
     tenant: Optional[str] = None,
 ):
     """
-    Create a new investigation
+    Create a new Investigation.
     """
     service = get_service(environment=region, tenant_id=tenant)
 
     alerts = None
     events = None
     search_queries = None
 
@@ -390,39 +415,20 @@
         evidence = get_investigation_evidence(database, service.tenant_id, "NEW")
         alerts = evidence.alerts
         events = evidence.events
         search_queries = evidence.search_queries
 
     # verify and save valid search queries
     if not dry_run:
-        valid_search_queries = []
-        for search_query in search_queries or []:
-            query = get_query(service, search_query)
-            if query.get("error"):
-                log.error(f"Error finding search query: {search_query}")
-                continue
-
-            if query.get("id"):
-                query_update = {
-                    "name": query.get("description", f"{title} Query"),
-                    "metadata": query.get("metadata", {}),
-                }
-                for metadata in query_update.get("metadata", []):
-                    if metadata.get("id", "") == "isSaved":
-                        metadata["value"] == "true"
-
-                query = update_query(service, search_query, query_update)
-                if query.get("error"):
-                    log.error(
-                        f"Error saving search query::{search_query}::{query.get('error')}"
-                    )
-                    continue
+        if search_queries:
+            queries = service.queries.query.ql_queries(
+                QLQueriesInput(rns=search_queries)
+            )
 
-                valid_search_queries.append(search_query)
-        search_queries = valid_search_queries or None
+        search_queries = [query.rn for query in queries.queries]
 
     create_investigation_input = CreateInvestigationInput(
         alerts=alerts,
         assignee_id=assignee_id,
         events=events,
         key_findings=key_findings.read_text(),
         priority=INVESTIGATION_PRIORITY_MAP[priority],
@@ -667,7 +673,222 @@
         service="investigations",
         tenant_id="N/A",
         region="N/A",
         arguments=inspect.currentframe().f_locals,
     )
 
     return normalized_results
+
+
+@investigations_attachment.command(name="list")
+@tracing
+def investigations_attachment_list(
+    investigation_id: Annotated[str, typer.Option()],
+    tenant: Annotated[Optional[str], typer.Option()] = None,
+    region: Annotated[Optional[str], typer.Option()] = None,
+):
+    """List file attachments for a given investigation."""
+    service = get_service(environment=region, tenant_id=tenant)
+
+    page = 1
+    per_page = 20
+
+    files = []
+
+    results = service.investigations2.query.investigation_files_v2(
+        InvestigationFilesV2Arguments(
+            investigation_id=investigation_id,
+            page=page,
+            per_page=per_page,
+        )
+    )
+    total_count = results.total_count
+    files.extend(results.files)
+
+    remaining_pages = -(-(total_count - per_page) // per_page)
+
+    for page in range(2, remaining_pages + 2):
+        results = service.investigations2.query.investigation_files_v2(
+            InvestigationFilesV2Arguments(
+                investigation_id=investigation_id,
+                page=page,
+                per_page=per_page,
+            )
+        )
+        files.extend(results.files)
+
+    normalized_results = TaegisResults(
+        raw_results=files,
+        service="investigations",
+        tenant_id=service.tenant_id,
+        region=service.environment,
+        arguments=inspect.currentframe().f_locals,
+    )
+
+    return normalized_results
+
+
+@investigations_attachment.command(name="get")
+@tracing
+def investigations_attachment_get(
+    file_id: Annotated[str, typer.Option()],
+    tenant: Annotated[Optional[str], typer.Option()] = None,
+    region: Annotated[Optional[str], typer.Option()] = None,
+):
+    """Get a file attachment."""
+    service = get_service(environment=region, tenant_id=tenant)
+
+    results = service.investigations2.query.investigation_file_v2(
+        InvestigationFileV2Arguments(
+            file_id=file_id,
+        )
+    )
+
+    normalized_results = TaegisResult(
+        raw_results=results,
+        service="investigations",
+        tenant_id=service.tenant_id,
+        region=service.environment,
+        arguments=inspect.currentframe().f_locals,
+    )
+
+    return normalized_results
+
+
+@investigations_attachment.command(name="remove")
+@tracing
+def investigations_attachment_remove(
+    file_id: Annotated[str, typer.Option()],
+    tenant: Annotated[Optional[str], typer.Option()] = None,
+    region: Annotated[Optional[str], typer.Option()] = None,
+):
+    """Delete file attachment."""
+    service = get_service(environment=region, tenant_id=tenant)
+
+    results = service.investigations2.mutation.delete_investigation_file(
+        DeleteInvestigationFileInput(
+            file_id=file_id,
+        )
+    )
+
+    normalized_results = TaegisResult(
+        raw_results=results,
+        service="investigations",
+        tenant_id=service.tenant_id,
+        region=service.environment,
+        arguments=inspect.currentframe().f_locals,
+    )
+
+    return normalized_results
+
+
+@investigations_attachment.command(name="upload")
+@tracing
+def investigations_attachment_upload(
+    investigation_id: Annotated[str, typer.Option()],
+    file: Annotated[
+        Path,
+        typer.Option(
+            exists=True,
+            file_okay=True,
+            dir_okay=False,
+            writable=False,
+            readable=True,
+            resolve_path=True,
+        ),
+    ],
+    tenant: Annotated[Optional[str], typer.Option()] = None,
+    region: Annotated[Optional[str], typer.Option()] = None,
+):
+    """Upload file attachment."""
+    service = get_service(environment=region, tenant_id=tenant)
+
+    file_input = InitInvestigationFileUploadInput(
+        investigation_id=investigation_id,
+        name=file.name,
+        content_type=str(mimetypes.guess_type(file)[0]),
+        size=file.stat().st_size,
+    )
+    log.debug(file_input)
+
+    results = service.investigations2.mutation.init_investigation_file_upload(
+        input_=file_input
+    )
+    log.debug(results)
+
+    with file.open("rb") as f:
+        upload_response = requests.put(
+            results.presigned_url,
+            headers={
+                "Accept": "*/*",
+                "Content-Type": str(mimetypes.guess_type(file)[0]),
+                "Content-Length": str(file.stat().st_size),
+            },
+            data=f,
+        )
+    log.debug(upload_response)
+
+    verify_upload = service.investigations2.query.investigation_file_v2(
+        InvestigationFileV2Arguments(
+            file_id=results.file.id,
+        )
+    )
+    log.debug(verify_upload)
+
+    normalized_results = TaegisResult(
+        raw_results=verify_upload,
+        service="investigations",
+        tenant_id=service.tenant_id,
+        region=service.environment,
+        arguments=inspect.currentframe().f_locals,
+    )
+
+    return normalized_results
+
+
+@investigations_attachment.command("download")
+@tracing
+def investigations_attachment_download(
+    file_id: Annotated[
+        str,
+        typer.Option(),
+    ],
+    save_as: Annotated[Optional[str], typer.Option()] = None,
+    tenant: Annotated[Optional[str], typer.Option()] = None,
+    region: Annotated[Optional[str], typer.Option()] = None,
+):
+    """Get a file attachment."""
+    service = get_service(environment=region, tenant_id=tenant)
+
+    results = service.investigations2.query.investigation_file_v2(
+        InvestigationFileV2Arguments(
+            file_id=file_id,
+        )
+    )
+
+    if not results.download_url:
+        log.error("Cannot download file, no download url found.")
+        raise typer.Exit(code=1)
+
+    with requests.get(results.download_url, stream=True) as r:
+        r.raise_for_status()
+
+        if save_as:
+            filename = save_as
+        else:
+            filename = results.name
+
+        file_path = verify_file(filename)
+
+        with file_path.open("wb") as f:
+            for chunk in r.iter_content(chunk_size=8192):
+                f.write(chunk)
+
+    normalized_results = TaegisResult(
+        raw_results=results,
+        service="investigations",
+        tenant_id=service.tenant_id,
+        region=service.environment,
+        arguments=inspect.currentframe().f_locals,
+    )
+
+    return normalized_results
```

### Comparing `taegis_magic-2023.9.15/taegis_magic/commands/preferences.py` & `taegis_magic-2024.3.29/taegis_magic/commands/preferences.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/taegis_magic/commands/rules.py` & `taegis_magic-2024.3.29/taegis_magic/commands/rules.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/taegis_magic/commands/tenant_profiles.py` & `taegis_magic-2024.3.29/taegis_magic/commands/tenant_profiles.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/taegis_magic/commands/tenants.py` & `taegis_magic-2024.3.29/taegis_magic/commands/tenants.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/taegis_magic/commands/threat.py` & `taegis_magic-2024.3.29/taegis_magic/commands/threat.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/taegis_magic/commands/users.py` & `taegis_magic-2024.3.29/taegis_magic/commands/users.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/taegis_magic/commands/utils/investigations.py` & `taegis_magic-2024.3.29/taegis_magic/commands/utils/investigations.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/taegis_magic/core/cache.py` & `taegis_magic-2024.3.29/taegis_magic/core/cache.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/taegis_magic/core/log.py` & `taegis_magic-2024.3.29/taegis_magic/core/log.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/taegis_magic/core/normalizer.py` & `taegis_magic-2024.3.29/taegis_magic/core/normalizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Taegis Base Normalizer."""
 
-from dataclasses import dataclass, field
+from dataclasses import dataclass, field, asdict
 from typing import Any, Dict, List, Union
 
 import jinja2
 import pandas as pd
 from dataclasses_json import dataclass_json
 
 
@@ -63,14 +63,34 @@
 
         jinja_env.filters["validate_int"] = validate_int
 
         template = jinja_env.get_template(template_name)
         return template.render(obj=self)
 
 
+class TaegisResult(TaegisResultsNormalizer):
+    """Generic single result normalizer."""
+
+    raw_results: Any = field(default=None)
+
+    @property
+    def results(self):
+        return [asdict(self.raw_results)]
+
+
+class TaegisResults(TaegisResultsNormalizer):
+    """Generic multiple results normalizer."""
+
+    raw_results: List[Any] = field(default_factory=list)
+
+    @property
+    def results(self):
+        return [asdict(r) for r in self.raw_results]
+
+
 @dataclass_json
 @dataclass
 class DataFrameNormalizer(TaegisResultsNormalizer):
     raw_results: pd.DataFrame
 
     @property
     def results(self):
```

### Comparing `taegis_magic-2023.9.15/taegis_magic/core/queries.py` & `taegis_magic-2024.3.29/taegis_magic/core/queries.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/taegis_magic/core/service.py` & `taegis_magic-2024.3.29/taegis_magic/core/service.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/taegis_magic/core/utils.py` & `taegis_magic-2024.3.29/taegis_magic/core/utils.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/taegis_magic/pandas/alerts.py` & `taegis_magic-2024.3.29/taegis_magic/pandas/alerts.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/taegis_magic/pandas/audits.py` & `taegis_magic-2024.3.29/taegis_magic/pandas/audits.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/taegis_magic/pandas/rules.py` & `taegis_magic-2024.3.29/taegis_magic/pandas/rules.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/taegis_magic/pandas/tenants.py` & `taegis_magic-2024.3.29/taegis_magic/pandas/tenants.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/taegis_magic/pandas/utils.py` & `taegis_magic-2024.3.29/taegis_magic/pandas/utils.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/taegis_magic/templates/taegis_search_results.md.jinja` & `taegis_magic-2024.3.29/taegis_magic/templates/taegis_search_results.md.jinja`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/.gitignore` & `taegis_magic-2024.3.29/.gitignore`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/LICENSE` & `taegis_magic-2024.3.29/LICENSE`

 * *Files identical despite different names*

### Comparing `taegis_magic-2023.9.15/README.md` & `taegis_magic-2024.3.29/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 │ threat                                                                                          │
 │ users                                                                                           │
 ╰─────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 ## Sample Usage
 
-For more in depth examples see [docs](docs/README.md).
+For more in depth examples see [docs](https://github.com/secureworks/taegis-magic/blob/main/docs/README.md).
 
 ### CLI
 
 ```bash
 taegis alerts search --limit 2 --cell "FROM alert EARLIEST=-1d" --graphql-output "alerts { list { id metadata { title } } }"
 ```
```

### Comparing `taegis_magic-2023.9.15/pyproject.toml` & `taegis_magic-2024.3.29/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     "Jinja2",
     "nbformat",
     "pandas",
     "pandas[excel]",
     "requests",
     "taegis-sdk-python",
     "typer[all]>=0.9.0",
+    "panel",
+    "tabulator",
 ]
 
 [project.optional-dependencies]
 dev = ["black", "pylint", "jupyter"]
 
 [project.scripts]
 taegis = "taegis_magic.cli:cli"
```

### Comparing `taegis_magic-2023.9.15/PKG-INFO` & `taegis_magic-2024.3.29/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: taegis-magic
-Version: 2023.9.15
+Version: 2024.3.29
 Summary: Taegis IPython Magics
 Project-URL: Homepage, https://github.com/secureworks/taegis-magic
 Project-URL: Bug Reports, https://github.com/secureworks/taegis-magic/issues
 Project-URL: Source, https://github.com/secureworks/taegis-magic
 Project-URL: Package, https://pypi.org/project/taegis-magic/
 Author-email: Micah Pegman <sdks@secureworks.com>
 License:                                  Apache License
@@ -198,15 +198,17 @@
 Requires-Dist: gql
 Requires-Dist: ipynbname
 Requires-Dist: ipython
 Requires-Dist: jinja2
 Requires-Dist: nbformat
 Requires-Dist: pandas
 Requires-Dist: pandas[excel]
+Requires-Dist: panel
 Requires-Dist: requests
+Requires-Dist: tabulator
 Requires-Dist: taegis-sdk-python
 Requires-Dist: typer[all]>=0.9.0
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: jupyter; extra == 'dev'
 Requires-Dist: pylint; extra == 'dev'
 Description-Content-Type: text/markdown
@@ -256,15 +258,15 @@
 │ threat                                                                                          │
 │ users                                                                                           │
 ╰─────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 ## Sample Usage
 
-For more in depth examples see [docs](docs/README.md).
+For more in depth examples see [docs](https://github.com/secureworks/taegis-magic/blob/main/docs/README.md).
 
 ### CLI
 
 ```bash
 taegis alerts search --limit 2 --cell "FROM alert EARLIEST=-1d" --graphql-output "alerts { list { id metadata { title } } }"
 ```
```

