# Comparing `tmp/findly_unified_reporting_sdk-0.6.7.tar.gz` & `tmp/findly_unified_reporting_sdk-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findly_unified_reporting_sdk-0.6.7.tar", max compression
+gzip compressed data, was "findly_unified_reporting_sdk-0.6.8.tar", max compression
```

## Comparing `findly_unified_reporting_sdk-0.6.7.tar` & `findly_unified_reporting_sdk-0.6.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    35149 2024-03-05 17:34:31.649998 findly_unified_reporting_sdk-0.6.7/LICENSE
--rw-r--r--   0        0        0     2182 2024-03-14 18:26:39.724288 findly_unified_reporting_sdk-0.6.7/README.md
--rw-r--r--   0        0        0        0 2024-03-22 11:31:41.156543 findly_unified_reporting_sdk-0.6.7/findly/__init__.py
--rw-r--r--   0        0        0      332 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/common/__init__.py
--rw-r--r--   0        0        0     7897 2024-03-22 17:41:32.233479 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/common/common_parser.py
--rw-r--r--   0        0        0      971 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/common/date_range_helper.py
--rw-r--r--   0        0        0     3886 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/common/reports_client.py
--rw-r--r--   0        0        0     5727 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/common/where_string_comparison.py
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/fb_ads/__init__.py
--rw-r--r--   0        0        0    20703 2024-04-22 17:42:16.784701 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_client.py
--rw-r--r--   0        0        0    31246 2024-04-16 17:38:32.855858 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_query_args_parser.py
--rw-r--r--   0        0        0     1492 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/action_breakdowns.csv
--rw-r--r--   0        0        0     5778 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/breakdowns.csv
--rw-r--r--   0        0        0    16489 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/dimensions.jsonl
--rw-r--r--   0        0        0    17708 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/fields.csv
--rw-r--r--   0        0        0    20146 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/metrics.jsonl
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/ga4/__init__.py
--rw-r--r--   0        0        0    38299 2024-04-16 17:38:32.855858 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/ga4/ga4_client.py
--rw-r--r--   0        0        0    30004 2024-04-01 17:15:45.015611 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/ga4/ga4_query_args_parser.py
--rw-r--r--   0        0        0    33511 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/ga4/metadata/dimensions.jsonl
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/gsc/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/gsc/gsc_client.py
--rw-r--r--   0        0        0     1038 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/gsc/gsc_service.py
--rw-r--r--   0        0        0       27 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/protos/.gitignore
--rw-r--r--   0        0        0      137 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/protos/__init__.py
--rw-r--r--   0        0        0     6569 2024-03-22 11:32:22.277139 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.py
--rw-r--r--   0        0        0    29515 2024-03-22 11:32:22.277139 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.pyi
--rw-r--r--   0        0        0     2993 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/urs.py
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/util/__init__.py
--rw-r--r--   0        0        0      451 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/util/create_numeric_string_series.py
--rw-r--r--   0        0        0     1237 2024-04-22 17:43:33.788235 findly_unified_reporting_sdk-0.6.7/pyproject.toml
--rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 findly_unified_reporting_sdk-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-05 17:34:31.649998 findly_unified_reporting_sdk-0.6.8/LICENSE
+-rw-r--r--   0        0        0     2182 2024-03-14 18:26:39.724288 findly_unified_reporting_sdk-0.6.8/README.md
+-rw-r--r--   0        0        0        0 2024-03-22 11:31:41.156543 findly_unified_reporting_sdk-0.6.8/findly/__init__.py
+-rw-r--r--   0        0        0      342 2024-04-25 14:35:17.466011 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/common/__init__.py
+-rw-r--r--   0        0        0     7897 2024-03-22 17:41:32.233479 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/common/common_parser.py
+-rw-r--r--   0        0        0      971 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/common/date_range_helper.py
+-rw-r--r--   0        0        0     3647 2024-04-25 14:35:17.494011 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/common/reports_client.py
+-rw-r--r--   0        0        0     5671 2024-04-25 14:35:17.526011 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/common/where_string_comparison.py
+-rw-r--r--   0        0        0        0 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/__init__.py
+-rw-r--r--   0        0        0    20517 2024-04-25 14:29:11.890413 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_client.py
+-rw-r--r--   0        0        0    30965 2024-04-25 14:29:43.918010 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_query_args_parser.py
+-rw-r--r--   0        0        0     1492 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/action_breakdowns.csv
+-rw-r--r--   0        0        0     5778 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/breakdowns.csv
+-rw-r--r--   0        0        0    16489 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/dimensions.jsonl
+-rw-r--r--   0        0        0    17708 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/fields.csv
+-rw-r--r--   0        0        0    20146 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/metrics.jsonl
+-rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/ga4/__init__.py
+-rw-r--r--   0        0        0    38179 2024-04-25 14:29:11.890413 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/ga4/ga4_client.py
+-rw-r--r--   0        0        0    30064 2024-04-25 14:35:17.658009 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/ga4/ga4_query_args_parser.py
+-rw-r--r--   0        0        0    33511 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/ga4/metadata/dimensions.jsonl
+-rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/gsc/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/gsc/gsc_client.py
+-rw-r--r--   0        0        0     1038 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/gsc/gsc_service.py
+-rw-r--r--   0        0        0       27 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/protos/.gitignore
+-rw-r--r--   0        0        0      137 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/protos/__init__.py
+-rw-r--r--   0        0        0     6569 2024-03-22 11:32:22.277139 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.py
+-rw-r--r--   0        0        0    29515 2024-03-22 11:32:22.277139 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.pyi
+-rw-r--r--   0        0        0     2915 2024-04-25 14:35:17.490011 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/urs.py
+-rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/util/__init__.py
+-rw-r--r--   0        0        0      457 2024-04-25 14:35:17.470011 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/util/create_numeric_string_series.py
+-rw-r--r--   0        0        0     1237 2024-04-25 14:32:46.123787 findly_unified_reporting_sdk-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 findly_unified_reporting_sdk-0.6.8/PKG-INFO
```

### Comparing `findly_unified_reporting_sdk-0.6.7/LICENSE` & `findly_unified_reporting_sdk-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.7/README.md` & `findly_unified_reporting_sdk-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/common/common_parser.py` & `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/common/common_parser.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/common/date_range_helper.py` & `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/common/date_range_helper.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/common/reports_client.py` & `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/common/reports_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,52 +7,42 @@
     Dimension,
     Metric,
     QueryArgs,
 )
 
 
 class ReportsClient(ABC):
-
     @abstractmethod
     async def list_property_ids(self, **kwargs: str) -> Optional[List[str]]:
         """
         List all property ids for the authenticated user.
 
         Returns:
             Optional[List[str]]: A list of property ids.
         """
 
     @abstractmethod
     async def query(
-        self,
-        query_args: QueryArgs,
-        property_id: str,
-        logger: logging.LoggerAdapter,
-        **kwargs: str
+        self, query_args: QueryArgs, property_id: str, **kwargs: str
     ) -> Optional[Tuple[List[pd.DataFrame], List[pd.DataFrame]]]:
         """
         Executes the integration API request based on the SQL query parts.
 
         Args:
             query_args (QueryArgs): The parts of the SQL query to execute.
             property_id (str): The property ID to execute the query for.
-            logger (logging.LoggerAdapter): A logger instance.
 
         Returns:
             Optional[Tuple[List[pd.DataFrame], List[pd.DataFrame]]]: A tuple containing two lists of pandas DataFrames, or None if the query failed.
         """
         pass
 
     @abstractmethod
     async def get_dimension_values(
-        self,
-        dimension: Dimension,
-        top_n: int,
-        property_id: str,
-        **kwargs: str
+        self, dimension: Dimension, top_n: int, property_id: str, **kwargs: str
     ) -> Optional[List[str]]:
         """
         Retrieves a sample of the top N values of a dimension.
 
         Args:
             dimension (Dimension): The dimension to retrieve the values for.
             top_n (int): The number of top values to retrieve.
@@ -61,52 +51,45 @@
         Returns:
             Optional[List[str]]: A list of the top N dimension values, or None if the retrieval failed.
         """
         pass
 
     @abstractmethod
     async def list_dimensions(
-        self,
-        property_id: str,
-        **kwargs: str
+        self, property_id: str, **kwargs: str
     ) -> Optional[List[Dimension]]:
         """
         Retrieves a list of all property dimensions from the API.
 
         Args:
             property_id (str): The property ID to retrieve the dimensions for.
 
         Returns:
             Optional[List[Dimension]]: A list of all dimensions, or None if the retrieval failed.
         """
         pass
 
     @abstractmethod
     async def list_metrics(
-        self,
-        property_id: str,
-        **kwargs: str
+        self, property_id: str, **kwargs: str
     ) -> Optional[List[Metric]]:
         """
         Retrieves a list of all property metrics from the API.
 
         Args:
             property_id: The property ID to retrieve the metrics for.
 
         Returns:
             A list of all metrics, or None if the retrieval failed.
         """
         pass
 
     @abstractmethod
     async def get_dimension_from_name(
-        self,
-        dimension_name: str,
-        property_id: str,
-        **kwargs: str
+        self, dimension_name: str, property_id: str, **kwargs: str
     ) -> Optional[Dimension]:
         """
         Retrieves a dimension object by its name.
 
         Args:
             dimension_name (str): The name of the dimension to retrieve.
             property_id (str): The property ID to retrieve the dimension for.
@@ -114,18 +97,15 @@
         Returns:
             Optional[Dimension]: The dimension with the given name, or None if the dimension was not found.
         """
         pass
 
     @abstractmethod
     async def get_metric_from_name(
-        self,
-        metric_name: str,
-        property_id: str,
-        **kwargs: str
+        self, metric_name: str, property_id: str, **kwargs: str
     ) -> Optional[Metric]:
         """
         Retrieves a metric object by its name.
 
         Args:
             metric_name (str): The name of the metric to retrieve.
             property_id (str): The property ID to retrieve the metric for.
```

### Comparing `findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/common/where_string_comparison.py` & `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/common/where_string_comparison.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,37 +5,38 @@
 from dataclasses import dataclass
 import logging
 from typing import List, Optional
 from sqlglot import parse_one
 from sqlglot import expressions as sqlglot_expressions
 from sqlglot import Expression
 
+LOGGER = logging.getLogger(__name__)
+
 
 @dataclass
 class WhereClauseInformation:
     column_name: str
     column_operator: str
     column_value: str
     is_not_condition: bool = False
 
 
 def parse_where_columns_from_sql_query(
     sql_query: str,
     dialect: str,
-    logger: logging.LoggerAdapter,
     where_clause_str: Optional[str] = None,
 ) -> List[WhereClauseInformation]:
     try:
         where_clause_maybe: Optional[Expression] = parse_one(
             sql=sql_query,
             read=dialect.lower(),
         ).args.get("where")
 
         if where_clause_maybe is None:
-            logger.info(
+            LOGGER.info(
                 {
                     "msg": "parse_where_column_condition_no_where_clause",
                     "where_clause": where_clause_str,
                     "sql_query": sql_query,
                 }
             )
             return []
@@ -89,36 +90,36 @@
                             column_name=condition.this.sql(),
                             column_operator=condition.key,
                             column_value=condition.expression.sql(),
                             is_not_condition=not_condition,
                         )
                     )
                 except Exception as e:
-                    logger.warning(
+                    LOGGER.warning(
                         {
                             "msg": "error_parsing_where_condition",
                             "condition": condition.this.sql(),
                             "where_clause": where_clause_str,
                             "sql_query": sql_query,
                             "error": str(e),
                         }
                     )
-        logger.info(
+        LOGGER.info(
             {
                 "msg": "parse_where_column_condition_values",
                 "where_clause": where_clause_str,
                 "sql_query": sql_query,
                 "where_clause_values": [
                     dataclasses.asdict(value) for value in where_clause_values
                 ],
             }
         )
         return where_clause_values
     except Exception as e:
-        logger.error(
+        LOGGER.error(
             {
                 "msg": "error_parse_where_column_condition",
                 "where_clause": where_clause_str,
                 "sql_query": sql_query,
                 "error": str(e),
             }
         )
@@ -127,25 +128,22 @@
 
 # We are going to parse the where columns and just log them, to see if
 # we can do it correctly
 # if all things work, we can use edit distance here to fix things
 def parse_where_column_condition(
     where_clause_str: str,
     dialect: str,
-    logger: logging.LoggerAdapter,
 ) -> List[WhereClauseInformation]:
     dummy_select_string = "select * from table"
 
     # if the where_clause_str doesn't start with a where, we need to add it.
     if not where_clause_str.lower().startswith("where"):
         where_clause_str = "where " + where_clause_str
 
     # The where clause already starts with a where on the completion, so
     # just appending it to the dummy string should work
     complete_sql = dummy_select_string + " " + where_clause_str
     return parse_where_columns_from_sql_query(
         sql_query=complete_sql,
         dialect=dialect,
-        logger=logger,
         where_clause_str=where_clause_str,
     )
-
```

### Comparing `findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_client.py` & `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -298,62 +298,56 @@
             raise e
 
     @cached(ttl=300, cache=Cache.MEMORY)  # Cache results for 5 minutes
     async def _decorated_query(
         self,
         query_args: QueryArgs,
         property_id: str,
-        logger: logging.LoggerAdapter,
         **kwargs: str,
     ) -> Optional[Tuple[List[pd.DataFrame], List[pd.DataFrame]]]:
         params = await FB_PARSER.parse_query_args_to_request_params(
             query_args=query_args,
             property_id=property_id,
-            logger=logger,
         )
         insights = None
         try:
             insights, summary = await self._decorated_query_from_parts(**params)
 
         except Exception as e:
-            logger.error(
+            LOGGER.error(
                 {
                     "msg": "fb_ads_query_failed",
                     "error": str(e),
                 }
             )
             raise e
 
         if insights is None:
             return None
 
         generated_result_df = await FB_PARSER.parse_report_response_to_dataframe(
             report_response=insights,
             query_args=query_args,
-            logger=logger,
         )
 
         generated_totals_df = FB_PARSER.parse_totals_to_dataframe(
             summary=summary,
             query_args=query_args,
-            logger=logger,
         )
         return generated_result_df, generated_totals_df
 
     async def query(
         self,
         query_args: QueryArgs,
         property_id: str,
-        logger: logging.LoggerAdapter,
         **kwargs: str,
     ) -> Optional[Tuple[List[pd.DataFrame], List[pd.DataFrame]]]:
         return await self._decorated_query(
             query_args=query_args,
             property_id=property_id,
-            logger=logger,
             **kwargs,
         )
 
     @cached(
         ttl=3600, cache=Cache.MEMORY, skip_cache_func=lambda x: x is None
     )  # Cache results for 1 hour
     async def _decorated_get_dimension_values(
```

### Comparing `findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_query_args_parser.py` & `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_query_args_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 import json
 import pandas as pd
 import numpy as np
 from typing import List, Optional, Dict, Any
 from google.protobuf.json_format import ParseDict
 from facebook_business.adobjects.adsinsights import AdsInsights
-import copy
 
 from findly.unified_reporting_sdk.data_sources.common.common_parser import (
     CommonParser,
     RESERVED_TOTAL,
 )
 
 from findly.unified_reporting_sdk.util.create_numeric_string_series import (
@@ -25,14 +24,15 @@
     Metric,
     MetricValueType,
     Dimension,
     QueryArgs,
 )
 import os
 
+LOGGER = logging.getLogger(__name__)
 script_path = os.path.realpath(__file__)
 METRICS_JSONL_PATH = os.path.join(
     os.path.dirname(script_path), "metadata", "metrics.jsonl"
 )
 DIMENSION_JSONL_PATH = os.path.join(
     os.path.dirname(script_path), "metadata", "dimensions.jsonl"
 )
@@ -163,37 +163,35 @@
             split_dfs.append(temp_df)
         return split_dfs
 
     async def parse_report_response_to_dataframe(
         self,
         report_response: List[AdsInsights],
         query_args: QueryArgs,
-        logger: logging.LoggerAdapter,
     ) -> List[pd.DataFrame]:
         """
         Parses a list of AdsInsights objects into a list of pandas DataFrames.
 
         Parameters:
             report_response (List[AdsInsights]): A list with Facebook AdsInsights for the query performed.
             query_args (QueryArgs): An object containing the parts of a query.
-            logger (logging.LoggerAdapter): A logger for logging information and errors.
 
         Returns:
             List[pd.DataFrame]: A list of pandas DataFrames representing the parsed report response. Each DataFrame corresponds to a specific date range.
 
         Raises:
             Exception: If an error occurs during the parsing process, an exception is logged and an empty DataFrame is returned.
         """
-        logger.info(
+        LOGGER.info(
             {
                 "msg": "parse_report_response_to_dataframe",
             }
         )
         if not report_response:
-            logger.info(
+            LOGGER.info(
                 {
                     "msg": "empty_report_response",
                 }
             )
             return [pd.DataFrame()]
 
         metrics_headers = list(query_args.metrics)
@@ -202,48 +200,48 @@
             dim for dim in [DATE, YEARMONTH] if dim in dimensions_headers
         ]
         dimensions_headers = [
             dim for dim in dimensions_headers if dim not in [DATE, YEARMONTH]
         ]
 
         try:
-            logger.info(
+            LOGGER.info(
                 {
                     "msg": "converting_to_df",
                 }
             )
             df = pd.DataFrame(report_response)
 
-            logger.info(
+            LOGGER.info(
                 {
                     "msg": "sucefully_converted_to_df",
                 }
             )
 
             # First, chack if all the metrics and dimensions are in the response
             # If not, we will fill the column with NaN
             # List the columns
             expected_columns = metrics_headers + dimensions_headers
             column_names_list = df.columns.tolist()
             # if there are only the dates columns, return empty dataframe
             if column_names_list == [START_DATE_COLUMN_NAME, END_DATE_COLUMN_NAME]:
-                logger.info(
+                LOGGER.info(
                     {
                         "msg": "only_dates_columns_in_report_response",
                     }
                 )
                 return [pd.DataFrame()]
 
             # Find items in your_list that are not in column_names_list
             missing_items = [
                 col for col in expected_columns if col not in column_names_list
             ]
             missing_action: List[str] = []
             if len(missing_items) > 0:
-                logger.info(
+                LOGGER.info(
                     {
                         "msg": "missing_columns_in_report_response",
                         "missing_columns": missing_items,
                     }
                 )
                 # Add each missing item as a new column with NaN values
                 for col in missing_items:
@@ -255,15 +253,15 @@
                         df[col] = np.nan
 
             # Now, Check if any of the metrics is of type METRIC_VALUE_TYPE_LIST_ADS_ACTION_STATS
             # If so, we want to explode the values of that column
             try:
                 all_metrics_list = self.parse_metrics()
             except Exception as e:
-                logger.error(
+                LOGGER.error(
                     {
                         "msg": "error_parsing_metrics",
                         "error": str(e),
                     }
                 )
                 return [pd.DataFrame()]
             metrics_list = [
@@ -272,15 +270,15 @@
 
             for metric in metrics_list:
                 if (
                     metric.value_type
                     == MetricValueType.METRIC_VALUE_TYPE_LIST_ADS_ACTION_STATS
                     and metric.name not in missing_items
                 ):
-                    logger.info(
+                    LOGGER.info(
                         {
                             "msg": "struct_type_metric_found",
                             "metric": metric.name,
                         }
                     )
                     # Explode the metric column
                     exploded_df = df.explode(metric.name)
@@ -325,57 +323,57 @@
 
             # At last, return that if there is only one date range,
             # else, we need to split the dataframe into multiple dataframes
             parsed_dates = self.get_date_ranges(
                 date_str_range_list=list(query_args.date_ranges),
             )
             if len(parsed_dates) == 1:
-                logger.info(
+                LOGGER.info(
                     {
                         "msg": "one_date_range",
                         "parsed_dates": parsed_dates,
                     }
                 )
                 if date_dimensions == [DATE]:
-                    logger.info(
+                    LOGGER.info(
                         {
                             "msg": "time_increment_1",
                         }
                     )
                     # This will be the case when we have a result for each day
                     # Will be easier for the user to understand
                     # And consistent with GA4 for the code interpreter
                     df["date"] = df[START_DATE_COLUMN_NAME]
                     df = df.drop(columns=[START_DATE_COLUMN_NAME, END_DATE_COLUMN_NAME])
 
                 elif date_dimensions == [YEARMONTH]:
-                    logger.info(
+                    LOGGER.info(
                         {
                             "msg": "time_increment_monthly",
                         }
                     )
                     # This will be the case when we have a result for each month
                     # Will be easier for the user to understand
                     df["yearMonth"] = df[START_DATE_COLUMN_NAME].str.slice(
                         0, N_CHAR_YEAR_MONTH
                     )
                     df = df.drop(columns=[START_DATE_COLUMN_NAME, END_DATE_COLUMN_NAME])
                 else:
-                    logger.info(
+                    LOGGER.info(
                         {
                             "msg": "no_time_increment",
                         }
                     )
                     return [
                         df.drop(columns=[START_DATE_COLUMN_NAME, END_DATE_COLUMN_NAME])
                     ]
 
                 return [df]
 
-            logger.info(
+            LOGGER.info(
                 {
                     "msg": "split_dataframe_by_date_ranges",
                     "parsed_dates": parsed_dates,
                 }
             )
             final_df_list = self.split_dataframe_by_date_ranges(
                 df=df,
@@ -386,43 +384,42 @@
             equalized_dataframes = self.equalize_dataframe_rows(
                 dataframes=final_df_list,
                 dimensions=dimensions_headers,
             )
             return equalized_dataframes
 
         except Exception as e:
-            logger.error(
+            LOGGER.error(
                 {
                     "msg": "error_parse_report_response_to_dataframe",
                     "error": str(e),
                 }
             )
             return [pd.DataFrame()]
 
     # We want to parse the FB Ads totals into a dataframe.
     # This will be used by the frontend to display the data.
     def parse_totals_to_dataframe(
         self,
         summary: Optional[Dict],
         query_args: QueryArgs,
-        logger: logging.LoggerAdapter,
     ) -> List[pd.DataFrame]:
         if summary is None:
             return [pd.DataFrame()]
 
         metrics_headers = list(query_args.metrics)
         dimensions_headers = list(query_args.group_by_columns)
         date_dimensions = [
             dim for dim in [DATE, YEARMONTH] if dim in dimensions_headers
         ]
         dimensions_headers = [
             dim for dim in dimensions_headers if dim not in [DATE, YEARMONTH]
         ]
 
-        logger.info(
+        LOGGER.info(
             {
                 "msg": "parse_totals_to_dataframe",
             }
         )
 
         # first we convert the summary to a dataframe, this will contains the totals of the metrics
         summary_df = pd.DataFrame.from_records([summary])
@@ -433,15 +430,15 @@
         ]
         for missing_metric in missing_metrics:
             summary_df[missing_metric] = np.nan
 
         try:
             all_metrics_list = self.parse_metrics()
         except Exception as e:
-            logger.error(
+            LOGGER.error(
                 {
                     "msg": "error_parsing_metrics",
                     "error": str(e),
                 }
             )
             return [pd.DataFrame()]
 
@@ -452,15 +449,15 @@
         # now, for the struct type metrics, we need to explode the values
         for metric in metrics_list:
             if (
                 metric.value_type
                 == MetricValueType.METRIC_VALUE_TYPE_LIST_ADS_ACTION_STATS
                 and metric.name not in missing_metrics
             ):
-                logger.info(
+                LOGGER.info(
                     {
                         "msg": "struct_type_metric_found",
                         "metric": metric.name,
                     }
                 )
                 # Explode the metric column
                 exploded_df = summary_df.explode(metric.name)
@@ -538,55 +535,54 @@
 
         return [summary_df]
 
     async def parse_query_args_to_request_params(
         self,
         query_args: QueryArgs,
         property_id: str,
-        logger: logging.LoggerAdapter,
     ) -> Dict[str, Any]:
         fb_ads_metrics_list = list(query_args.metrics)
-        logger.info("sucessfully got metrics")
+        LOGGER.info("sucessfully got metrics")
 
         all_fb_dimensions = self.parse_dimensions()
         fb_ads_dimensions_list = list(
             filter(lambda x: x.name in query_args.group_by_columns, all_fb_dimensions)
         )
-        logger.info("sucessfully got dimensions")
+        LOGGER.info("sucessfully got dimensions")
 
         fb_ads_date_ranges = self.get_date_ranges(
             date_str_range_list=list(query_args.date_ranges),
         )
-        logger.info("sucessfully got date ranges")
+        LOGGER.info("sucessfully got date ranges")
 
         fb_ads_order_by_list = await self.get_order_by(
             order_by_list=list(query_args.order_by),
             order_by_candidates=list(query_args.metrics)
             + list(query_args.group_by_columns),
         )
-        logger.info("sucessfully got order by")
+        LOGGER.info("sucessfully got order by")
 
         fb_filter: List[Dict[str, str]] = []
 
         fb_ads_dimension_filter_list = self.get_filter_from_expression(
-            expr=query_args.where_clause, logger=logger
+            expr=query_args.where_clause
         )
         if fb_ads_dimension_filter_list is not None:
             fb_filter.extend(fb_ads_dimension_filter_list)
-        logger.info("sucessfully got dimension filter")
+        LOGGER.info("sucessfully got dimension filter")
 
         fb_ads_metrics_filter_list = self.get_filter_from_expression(
-            expr=query_args.having_clause, logger=logger
+            expr=query_args.having_clause
         )
         if fb_ads_metrics_filter_list is not None:
             fb_filter.extend(fb_ads_metrics_filter_list)
 
-        logger.info("sucessfully got metrics filter")
+        LOGGER.info("sucessfully got metrics filter")
 
-        logger.info(
+        LOGGER.info(
             {
                 "msg": "query_parts",
                 "metrics": fb_ads_metrics_list,
                 "dimensions": [dimension.name for dimension in fb_ads_dimensions_list],
                 "date_ranges": [
                     {"start_date": dr["since"], "end_date": dr["until"]}
                     for dr in fb_ads_date_ranges
@@ -643,15 +639,14 @@
                 )
                 return [order_by_item.lstrip("-") + direction]
 
         return None
 
     def get_filter_from_expression(
         self,
-        logger: logging.LoggerAdapter,
         expr: Optional[str] = None,
         parsed_expr: Optional[list[WhereClauseInformation]] = None,
     ) -> Optional[List[Dict[str, Any]]]:
         """
         Following Fb Ads documentation: https://developers.facebook.com/docs/marketing-api/reference/ad-account/insights/
         Filters on the report data. This parameter is an array of filter object. Each filter object has three fields: 'field', 'operator' and 'value'.
         Valid filter operator could be ('EQUAL', 'NOT_EQUAL', 'GREATER_THAN', 'GREATER_THAN_OR_EQUAL', 'LESS_THAN', 'LESS_THAN_OR_EQUAL', 'IN_RANGE', 'NOT_IN_RANGE', 'CONTAIN', 'NOT_CONTAIN', 'IN', 'NOT_IN', 'ANY', 'ALL', 'NONE').
@@ -669,29 +664,28 @@
             clean_expr = expr
             if expr.lower().startswith("having"):
                 clean_expr = expr[7:]
 
             unformatted_filter_list = parse_where_column_condition(
                 where_clause_str=clean_expr,
                 dialect="",
-                logger=logger,
             )
 
         else:
-            logger.info({"msg": "no_expression_or_parsed_expression_provided"})
+            LOGGER.info({"msg": "no_expression_or_parsed_expression_provided"})
             return None
 
         final_filter_list: List[Dict[str, Any]] = []
 
         for unformatted_filter in unformatted_filter_list:
             field = unformatted_filter.column_name
 
             # Filter account_name is not valid anymore, please use account.name instead
             if field in DIMENSION_DIFFERENT_NAME_FILTER:
-                logger.info(
+                LOGGER.info(
                     {
                         "msg": "updating_column_name_for_filter",
                         "field": field,
                     }
                 )
                 field = field.replace("_", ".")
 
@@ -719,15 +713,15 @@
                 operator = CONVERTER_SQLGLOT_FB_FILTER_OP[operator]
 
             if operator == "IN_RANGE":
                 if unformatted_filter.is_not_condition:
                     operator = "NOT_IN_RANGE"
                 array_value = convert_in_range_to_array(value.replace(" ", ""))
                 if array_value is None:
-                    logger.info(
+                    LOGGER.info(
                         {
                             "msg": "error_convert_in_range_to_array",
                             "value": value,
                         }
                     )
                     continue
                 final_filter_list.append(
```

### Comparing `findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/action_breakdowns.csv` & `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/action_breakdowns.csv`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/breakdowns.csv` & `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/breakdowns.csv`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/dimensions.jsonl` & `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/dimensions.jsonl`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/fields.csv` & `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/fields.csv`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/metrics.jsonl` & `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/metrics.jsonl`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/ga4/ga4_client.py` & `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/ga4/ga4_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,28 +325,26 @@
         )
 
     @cached(ttl=300, cache=Cache.MEMORY)  # Cache results for 5 minutes
     async def _decorated_query(
         self,
         query_args: QueryArgs,
         property_id: str,
-        logger: logging.LoggerAdapter,
         **kwargs: str,
     ) -> Optional[Tuple[List[pd.DataFrame], List[pd.DataFrame]]]:
         params = await GA4_PARSER.parse_query_args_to_request_params(
             query_args=query_args,
             property_id=property_id,
-            logger=logger,
         )
         result = None
         try:
             result = await self._query(**params)
 
         except Exception as e:
-            logger.error(
+            LOGGER.error(
                 {
                     "msg": "ga4_query_failed",
                     "error": str(e),
                 }
             )
             raise
         if result is None:
@@ -361,19 +359,18 @@
         )
         return generated_result_df, generated_totals_df
 
     async def query(
         self,
         query_args: QueryArgs,
         property_id: str,
-        logger: logging.LoggerAdapter,
         **kwargs: str,
     ) -> Optional[Tuple[List[pd.DataFrame], List[pd.DataFrame]]]:
         return await self._decorated_query(
-            query_args=query_args, property_id=property_id, logger=logger, **kwargs
+            query_args=query_args, property_id=property_id, **kwargs
         )
 
     # Function to get the top N values for a given dimension.
     # Only return something for string dimensions.
     @cached(
         ttl=3600, cache=Cache.MEMORY, skip_cache_func=lambda x: x is None
     )  # Cache results for 1 hour
```

### Comparing `findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/ga4/ga4_query_args_parser.py` & `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/ga4/ga4_query_args_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,28 +16,33 @@
 from typing import Dict, Any, List, Optional
 from findly.unified_reporting_sdk.data_sources.common.common_parser import (
     CommonParser,
     RESERVED_TOTAL,
 )
 from findly.unified_reporting_sdk.protos.findly_semantic_layer_pb2 import QueryArgs
 
+LOGGER = logging.getLogger(__name__)
+
 DATE_FORMATS = {
     "date": ("%Y%m%d", "%Y-%m-%d"),
     "dateHour": ("%Y%m%d%H", "%Y-%m-%d %H"),
     "dateHourMinute": ("%Y%m%d%H%M", "%Y-%m-%d %H:%M"),
     "firstSessionDate": ("%Y%m%d", "%Y-%m-%d"),
     "yearMonth": ("%Y%m", "%Y-%m"),
 }
 
 DATE_RANGE_HEADER = "dateRange"
 
 
-def format_ga4_date_ranges_default(start_date: datetime, end_date: datetime) -> DateRange:
+def format_ga4_date_ranges_default(
+    start_date: datetime, end_date: datetime
+) -> DateRange:
     return DateRange(
-        start_date=start_date.strftime("%Y-%m-%d"), end_date=end_date.strftime("%Y-%m-%d")
+        start_date=start_date.strftime("%Y-%m-%d"),
+        end_date=end_date.strftime("%Y-%m-%d"),
     )
 
 
 class GA4QueryArgsParser(CommonParser):
     def __init__(self) -> None:
         super().__init__()
 
@@ -221,50 +226,53 @@
 
         return [pd.DataFrame(rows)]
 
     async def parse_query_args_to_request_params(
         self,
         query_args: QueryArgs,
         property_id: str,
-        logger: logging.LoggerAdapter,
     ) -> Dict[str, Any]:
         ga4_metrics_list = await self.get_metrics(
             metrics_name_list=list(query_args.metrics),
         )
-        logger.info("sucessfully got metrics")
+        LOGGER.info("sucessfully got metrics")
 
         ga4_dimensions_list = await self.get_dimensions(
             dimensions_name_list=list(query_args.group_by_columns),
         )
-        logger.info("sucessfully got dimensions")
+        LOGGER.info("sucessfully got dimensions")
 
         ga4_date_ranges = self.get_date_ranges(
-            date_str_range_list=list(query_args.date_ranges) if query_args.date_ranges is not None else None,
+            date_str_range_list=list(query_args.date_ranges)
+            if query_args.date_ranges is not None
+            else None,
             format_function=format_ga4_date_ranges_default,
         )
-        logger.info("sucessfully got date ranges")
+        LOGGER.info("sucessfully got date ranges")
 
         ga4_order_by_list = await self.get_order_by(
-            order_by_list=list(query_args.order_by) if query_args.order_by is not None else None,
+            order_by_list=list(query_args.order_by)
+            if query_args.order_by is not None
+            else None,
             order_by_metrics_candidates=list(query_args.metrics),
             order_by_dimensions_candidates=list(query_args.group_by_columns),
         )
-        logger.info("sucessfully got order by")
+        LOGGER.info("sucessfully got order by")
 
         ga4_dimension_filter_list = await self.get_filter_clause(
             filter_clause=query_args.where_clause
         )
-        logger.info("sucessfully got dimension filter")
+        LOGGER.info("sucessfully got dimension filter")
 
         ga4_metrics_filter_list = await self.get_filter_clause(
             filter_clause=query_args.having_clause
         )
-        logger.info("sucessfully got metrics filter")
+        LOGGER.info("sucessfully got metrics filter")
 
-        logger.info(
+        LOGGER.info(
             {
                 "msg": "query_parts",
                 "metrics": [metric.name for metric in ga4_metrics_list],
                 "dimensions": [dimension.name for dimension in ga4_dimensions_list],
                 "date_ranges": [
                     {"start_date": dr.start_date, "end_date": dr.end_date}
                     for dr in ga4_date_ranges
@@ -342,15 +350,15 @@
 
         Note:
             A "-" sign can be used to specify reverse order, e.g. "-ds".
             This will be used for the GA4 API.
         """
         order_bys: List[OrderBy] = []
 
-        for order_by in (order_by_list or []):
+        for order_by in order_by_list or []:
             if order_by.startswith("-"):
                 order_by = order_by[1:]
                 if order_by in order_by_metrics_candidates:
                     order_bys.append(
                         OrderBy(
                             metric=OrderBy.MetricOrderBy(
                                 metric_name=order_by,
```

### Comparing `findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/ga4/metadata/dimensions.jsonl` & `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/ga4/metadata/dimensions.jsonl`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/data_sources/gsc/gsc_service.py` & `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/gsc/gsc_service.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.py` & `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.pyi` & `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.7/findly/unified_reporting_sdk/urs.py` & `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/urs.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,22 +39,18 @@
             raise ValueError("Integration not supported")
 
         self._client = ConcreteClientClass(
             token=token, client_id=client_id, client_secret=client_secret
         )
 
     async def query(
-        self,
-        query_args: QueryArgs,
-        property_id: str,
-        logger: logging.LoggerAdapter,
-        **kwargs: str
+        self, query_args: QueryArgs, property_id: str, **kwargs: str
     ) -> Optional[Tuple[List[pd.DataFrame], List[pd.DataFrame]]]:
         return await self._client.query(
-            query_args=query_args, property_id=property_id, logger=logger, **kwargs
+            query_args=query_args, property_id=property_id, **kwargs
         )
 
     async def list_property_ids(self, **kwargs: str) -> Optional[List[str]]:
         return await self._client.list_property_ids(**kwargs)
 
     async def get_dimension_values(
         self, dimension: Dimension, top_n: int, property_id: str, **kwargs: str
```

### Comparing `findly_unified_reporting_sdk-0.6.7/pyproject.toml` & `findly_unified_reporting_sdk-0.6.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findly.unified-reporting-sdk"
-version = "0.6.7"
+version = "0.6.8"
 license = "GPL-3.0-only"
 description = ""
 authors = []
 readme = "README.md"
 packages = [
     { include = "findly" },
 ]
```

### Comparing `findly_unified_reporting_sdk-0.6.7/PKG-INFO` & `findly_unified_reporting_sdk-0.6.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findly-unified-reporting-sdk
-Version: 0.6.7
+Version: 0.6.8
 Summary: 
 License: GPL-3.0-only
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

