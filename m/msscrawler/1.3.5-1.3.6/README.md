# Comparing `tmp/msscrawler-1.3.5.tar.gz` & `tmp/msscrawler-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msscrawler-1.3.5.tar", last modified: Sun Apr 21 11:55:38 2024, max compression
+gzip compressed data, was "msscrawler-1.3.6.tar", last modified: Thu Apr 25 15:37:47 2024, max compression
```

## Comparing `msscrawler-1.3.5.tar` & `msscrawler-1.3.6.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-21 11:55:38.041855 msscrawler-1.3.5/
--rw-r--r--   0 hoonie     (501) staff       (20)     4918 2024-04-21 11:55:38.041782 msscrawler-1.3.5/PKG-INFO
--rw-r--r--   0 hoonie     (501) staff       (20)     4347 2023-10-27 15:07:06.000000 msscrawler-1.3.5/README.md
--rw-r--r--   0 hoonie     (501) staff       (20)       86 2023-10-24 15:03:13.000000 msscrawler-1.3.5/pyproject.toml
--rw-r--r--   0 hoonie     (501) staff       (20)      719 2024-04-21 11:55:38.042338 msscrawler-1.3.5/setup.cfg
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-21 11:55:38.029926 msscrawler-1.3.5/src/
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-21 11:55:38.032020 msscrawler-1.3.5/src/msscrawler/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/__init__.py
--rw-r--r--   0 hoonie     (501) staff       (20)      488 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/base_crawler.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-21 11:55:38.032980 msscrawler-1.3.5/src/msscrawler/connectors/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/connectors/__init__.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-21 11:55:38.033539 msscrawler-1.3.5/src/msscrawler/connectors/databases/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/connectors/databases/__init__.py
--rw-r--r--   0 hoonie     (501) staff       (20)      548 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/connectors/databases/base.py
--rw-r--r--   0 hoonie     (501) staff       (20)      984 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/connectors/databases/mongodb_connector.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-21 11:55:38.034230 msscrawler-1.3.5/src/msscrawler/connectors/message_brokers/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/connectors/message_brokers/__init__.py
--rw-r--r--   0 hoonie     (501) staff       (20)      344 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/connectors/message_brokers/base.py
--rw-r--r--   0 hoonie     (501) staff       (20)     2648 2024-04-21 11:54:57.000000 msscrawler-1.3.5/src/msscrawler/connectors/message_brokers/rabbitmq_connector.py
--rw-r--r--   0 hoonie     (501) staff       (20)     8396 2024-03-17 06:30:45.000000 msscrawler-1.3.5/src/msscrawler/generic_crawler.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-21 11:55:38.036235 msscrawler-1.3.5/src/msscrawler/items/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/items/__init__.py
--rw-r--r--   0 hoonie     (501) staff       (20)      224 2024-03-08 08:12:57.000000 msscrawler-1.3.5/src/msscrawler/items/base.py
--rw-r--r--   0 hoonie     (501) staff       (20)       74 2024-03-19 08:01:55.000000 msscrawler-1.3.5/src/msscrawler/items/brand_item.py
--rw-r--r--   0 hoonie     (501) staff       (20)      394 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/items/category_item.py
--rw-r--r--   0 hoonie     (501) staff       (20)      841 2024-03-23 15:35:05.000000 msscrawler-1.3.5/src/msscrawler/items/product_item.py
--rw-r--r--   0 hoonie     (501) staff       (20)      244 2024-01-19 08:49:20.000000 msscrawler-1.3.5/src/msscrawler/items/website_item.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-21 11:55:38.036632 msscrawler-1.3.5/src/msscrawler/log/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/log/__init__.py
--rw-r--r--   0 hoonie     (501) staff       (20)      655 2023-12-14 08:19:28.000000 msscrawler-1.3.5/src/msscrawler/log/default.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-21 11:55:38.036922 msscrawler-1.3.5/src/msscrawler/middlewares/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/middlewares/__init__.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-21 11:55:38.037859 msscrawler-1.3.5/src/msscrawler/mixins/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/mixins/__init__.py
--rw-r--r--   0 hoonie     (501) staff       (20)     1069 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/mixins/database_mixin.py
--rw-r--r--   0 hoonie     (501) staff       (20)       70 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/mixins/env_loader_mixin.py
--rw-r--r--   0 hoonie     (501) staff       (20)      819 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/mixins/message_connector_mixin.py
--rw-r--r--   0 hoonie     (501) staff       (20)     1804 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/mixins/spider_cache_mixin.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-21 11:55:38.038181 msscrawler-1.3.5/src/msscrawler/pipelines/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/pipelines/__init__.py
--rw-r--r--   0 hoonie     (501) staff       (20)      480 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/pipelines/base.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-21 11:55:38.038359 msscrawler-1.3.5/src/msscrawler/sites/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/sites/__init__.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-21 11:55:38.039398 msscrawler-1.3.5/src/msscrawler/sites/shopping/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/sites/shopping/__init__.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-21 11:55:38.039839 msscrawler-1.3.5/src/msscrawler/sites/shopping/spiders/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/sites/shopping/spiders/__init__.py
--rw-r--r--   0 hoonie     (501) staff       (20)     1316 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/sites/shopping/spiders/website_theamall_spider.py
--rw-r--r--   0 hoonie     (501) staff       (20)     9636 2024-02-05 03:03:42.000000 msscrawler-1.3.5/src/msscrawler/sites/shopping/website_crawler.py
--rw-r--r--   0 hoonie     (501) staff       (20)      215 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/sites/shopping/website_item.py
--rw-r--r--   0 hoonie     (501) staff       (20)     5416 2024-02-05 03:08:25.000000 msscrawler-1.3.5/src/msscrawler/sites/shopping/website_pipeline.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-21 11:55:38.041189 msscrawler-1.3.5/src/msscrawler/spiders/
--rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.5/src/msscrawler/spiders/__init__.py
--rw-r--r--   0 hoonie     (501) staff       (20)     9969 2024-03-17 06:31:14.000000 msscrawler-1.3.5/src/msscrawler/spiders/base.py
--rw-r--r--   0 hoonie     (501) staff       (20)      429 2024-03-19 08:04:31.000000 msscrawler-1.3.5/src/msscrawler/spiders/brand.py
--rw-r--r--   0 hoonie     (501) staff       (20)     1171 2024-01-20 16:39:13.000000 msscrawler-1.3.5/src/msscrawler/spiders/category.py
--rw-r--r--   0 hoonie     (501) staff       (20)     1594 2024-04-10 14:54:27.000000 msscrawler-1.3.5/src/msscrawler/spiders/product.py
--rw-r--r--   0 hoonie     (501) staff       (20)      734 2024-02-29 02:01:52.000000 msscrawler-1.3.5/src/msscrawler/spiders/website.py
-drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-21 11:55:38.041542 msscrawler-1.3.5/src/msscrawler.egg-info/
--rw-r--r--   0 hoonie     (501) staff       (20)     4918 2024-04-21 11:55:38.000000 msscrawler-1.3.5/src/msscrawler.egg-info/PKG-INFO
--rw-r--r--   0 hoonie     (501) staff       (20)     1757 2024-04-21 11:55:38.000000 msscrawler-1.3.5/src/msscrawler.egg-info/SOURCES.txt
--rw-r--r--   0 hoonie     (501) staff       (20)        1 2024-04-21 11:55:38.000000 msscrawler-1.3.5/src/msscrawler.egg-info/dependency_links.txt
--rw-r--r--   0 hoonie     (501) staff       (20)       11 2024-04-21 11:55:38.000000 msscrawler-1.3.5/src/msscrawler.egg-info/top_level.txt
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-25 15:37:47.193458 msscrawler-1.3.6/
+-rw-r--r--   0 hoonie     (501) staff       (20)     4918 2024-04-25 15:37:47.193372 msscrawler-1.3.6/PKG-INFO
+-rw-r--r--   0 hoonie     (501) staff       (20)     4347 2023-10-27 15:07:06.000000 msscrawler-1.3.6/README.md
+-rw-r--r--   0 hoonie     (501) staff       (20)       86 2023-10-24 15:03:13.000000 msscrawler-1.3.6/pyproject.toml
+-rw-r--r--   0 hoonie     (501) staff       (20)      719 2024-04-25 15:37:47.194038 msscrawler-1.3.6/setup.cfg
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-25 15:37:47.181489 msscrawler-1.3.6/src/
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-25 15:37:47.183653 msscrawler-1.3.6/src/msscrawler/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/__init__.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      488 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/base_crawler.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-25 15:37:47.184915 msscrawler-1.3.6/src/msscrawler/connectors/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/connectors/__init__.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-25 15:37:47.185591 msscrawler-1.3.6/src/msscrawler/connectors/databases/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/connectors/databases/__init__.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      548 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/connectors/databases/base.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      984 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/connectors/databases/mongodb_connector.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-25 15:37:47.186299 msscrawler-1.3.6/src/msscrawler/connectors/message_brokers/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/connectors/message_brokers/__init__.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      344 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/connectors/message_brokers/base.py
+-rw-r--r--   0 hoonie     (501) staff       (20)     3071 2024-04-25 15:37:22.000000 msscrawler-1.3.6/src/msscrawler/connectors/message_brokers/rabbitmq_connector.py
+-rw-r--r--   0 hoonie     (501) staff       (20)     8396 2024-03-17 06:30:45.000000 msscrawler-1.3.6/src/msscrawler/generic_crawler.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-25 15:37:47.188008 msscrawler-1.3.6/src/msscrawler/items/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/items/__init__.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      224 2024-03-08 08:12:57.000000 msscrawler-1.3.6/src/msscrawler/items/base.py
+-rw-r--r--   0 hoonie     (501) staff       (20)       74 2024-03-19 08:01:55.000000 msscrawler-1.3.6/src/msscrawler/items/brand_item.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      394 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/items/category_item.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      841 2024-03-23 15:35:05.000000 msscrawler-1.3.6/src/msscrawler/items/product_item.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      244 2024-01-19 08:49:20.000000 msscrawler-1.3.6/src/msscrawler/items/website_item.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-25 15:37:47.188398 msscrawler-1.3.6/src/msscrawler/log/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/log/__init__.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      655 2023-12-14 08:19:28.000000 msscrawler-1.3.6/src/msscrawler/log/default.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-25 15:37:47.188711 msscrawler-1.3.6/src/msscrawler/middlewares/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/middlewares/__init__.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-25 15:37:47.189564 msscrawler-1.3.6/src/msscrawler/mixins/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/mixins/__init__.py
+-rw-r--r--   0 hoonie     (501) staff       (20)     1069 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/mixins/database_mixin.py
+-rw-r--r--   0 hoonie     (501) staff       (20)       70 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/mixins/env_loader_mixin.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      819 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/mixins/message_connector_mixin.py
+-rw-r--r--   0 hoonie     (501) staff       (20)     1804 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/mixins/spider_cache_mixin.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-25 15:37:47.189916 msscrawler-1.3.6/src/msscrawler/pipelines/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/pipelines/__init__.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      480 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/pipelines/base.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-25 15:37:47.190157 msscrawler-1.3.6/src/msscrawler/sites/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/sites/__init__.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-25 15:37:47.191010 msscrawler-1.3.6/src/msscrawler/sites/shopping/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/sites/shopping/__init__.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-25 15:37:47.191416 msscrawler-1.3.6/src/msscrawler/sites/shopping/spiders/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/sites/shopping/spiders/__init__.py
+-rw-r--r--   0 hoonie     (501) staff       (20)     1316 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/sites/shopping/spiders/website_theamall_spider.py
+-rw-r--r--   0 hoonie     (501) staff       (20)     9636 2024-02-05 03:03:42.000000 msscrawler-1.3.6/src/msscrawler/sites/shopping/website_crawler.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      215 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/sites/shopping/website_item.py
+-rw-r--r--   0 hoonie     (501) staff       (20)     5416 2024-02-05 03:08:25.000000 msscrawler-1.3.6/src/msscrawler/sites/shopping/website_pipeline.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-25 15:37:47.192732 msscrawler-1.3.6/src/msscrawler/spiders/
+-rw-r--r--   0 hoonie     (501) staff       (20)        0 2023-10-29 00:59:21.000000 msscrawler-1.3.6/src/msscrawler/spiders/__init__.py
+-rw-r--r--   0 hoonie     (501) staff       (20)     9969 2024-03-17 06:31:14.000000 msscrawler-1.3.6/src/msscrawler/spiders/base.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      429 2024-03-19 08:04:31.000000 msscrawler-1.3.6/src/msscrawler/spiders/brand.py
+-rw-r--r--   0 hoonie     (501) staff       (20)     1171 2024-01-20 16:39:13.000000 msscrawler-1.3.6/src/msscrawler/spiders/category.py
+-rw-r--r--   0 hoonie     (501) staff       (20)     1594 2024-04-10 14:54:27.000000 msscrawler-1.3.6/src/msscrawler/spiders/product.py
+-rw-r--r--   0 hoonie     (501) staff       (20)      734 2024-02-29 02:01:52.000000 msscrawler-1.3.6/src/msscrawler/spiders/website.py
+drwxr-xr-x   0 hoonie     (501) staff       (20)        0 2024-04-25 15:37:47.193100 msscrawler-1.3.6/src/msscrawler.egg-info/
+-rw-r--r--   0 hoonie     (501) staff       (20)     4918 2024-04-25 15:37:47.000000 msscrawler-1.3.6/src/msscrawler.egg-info/PKG-INFO
+-rw-r--r--   0 hoonie     (501) staff       (20)     1757 2024-04-25 15:37:47.000000 msscrawler-1.3.6/src/msscrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 hoonie     (501) staff       (20)        1 2024-04-25 15:37:47.000000 msscrawler-1.3.6/src/msscrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 hoonie     (501) staff       (20)       11 2024-04-25 15:37:47.000000 msscrawler-1.3.6/src/msscrawler.egg-info/top_level.txt
```

### Comparing `msscrawler-1.3.5/PKG-INFO` & `msscrawler-1.3.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msscrawler
-Version: 1.3.5
+Version: 1.3.6
 Summary: A common package for crawling
 Home-page: https://bitbucket.org/dosiin/common/src/package/
 Author: no name
 Author-email: msscrawler@gmail.com
 Project-URL: Bug Tracker, https://bitbucket.org/dosiin/common/src/package/issues
 Project-URL: repository, https://bitbucket.org/dosiin/common/src/package/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `msscrawler-1.3.5/README.md` & `msscrawler-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.5/setup.cfg` & `msscrawler-1.3.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = msscrawler
-version = 1.3.5
+version = 1.3.6
 author = no name
 author_email = msscrawler@gmail.com
 description = A common package for crawling
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://bitbucket.org/dosiin/common/src/package/
 project_urls =
```

### Comparing `msscrawler-1.3.5/src/msscrawler/connectors/databases/base.py` & `msscrawler-1.3.6/src/msscrawler/connectors/databases/base.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.5/src/msscrawler/connectors/databases/mongodb_connector.py` & `msscrawler-1.3.6/src/msscrawler/connectors/databases/mongodb_connector.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.5/src/msscrawler/connectors/message_brokers/rabbitmq_connector.py` & `msscrawler-1.3.6/src/msscrawler/connectors/message_brokers/rabbitmq_connector.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,23 +40,37 @@
             ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLSv1_2)
             ssl_context.set_ciphers("ECDHE+AESGCM:!ECDSA")
             parameters.ssl_options = pika.SSLOptions(context=ssl_context)
 
         self.rabbit_mq_conn = pika.BlockingConnection(parameters)
 
         self.channel = self.rabbit_mq_conn.channel()
+
+        # declare delay exchange
+        self.channel.exchange_declare(
+            exchange="delay_exchange",
+            exchange_type="x-delayed-message",
+            durable=True,
+            auto_delete=False,
+            arguments={"x-delayed-type": "direct"},
+        )
+
         self.channel.queue_declare(queue=queue_declare, durable=True)
 
+        self.channel.queue_bind(
+            exchange="delay_exchange", queue=queue_declare, routing_key=queue_declare
+        )
+
     def close(self):
         if self.rabbit_mq_conn:
             self.rabbit_mq_conn.close()
 
     def send(self, message, target, **kwargs):
         self.channel.basic_publish(
-            exchange="",
+            exchange="delay_exchange",
             routing_key=target,
             body=json.dumps(message),
             properties=pika.BasicProperties(
                 delivery_mode=pika.spec.PERSISTENT_DELIVERY_MODE
             ),
         )
```

### Comparing `msscrawler-1.3.5/src/msscrawler/generic_crawler.py` & `msscrawler-1.3.6/src/msscrawler/generic_crawler.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.5/src/msscrawler/items/product_item.py` & `msscrawler-1.3.6/src/msscrawler/items/product_item.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.5/src/msscrawler/log/default.py` & `msscrawler-1.3.6/src/msscrawler/log/default.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.5/src/msscrawler/mixins/database_mixin.py` & `msscrawler-1.3.6/src/msscrawler/mixins/database_mixin.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.5/src/msscrawler/mixins/message_connector_mixin.py` & `msscrawler-1.3.6/src/msscrawler/mixins/message_connector_mixin.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.5/src/msscrawler/mixins/spider_cache_mixin.py` & `msscrawler-1.3.6/src/msscrawler/mixins/spider_cache_mixin.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.5/src/msscrawler/sites/shopping/spiders/website_theamall_spider.py` & `msscrawler-1.3.6/src/msscrawler/sites/shopping/spiders/website_theamall_spider.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.5/src/msscrawler/sites/shopping/website_crawler.py` & `msscrawler-1.3.6/src/msscrawler/sites/shopping/website_crawler.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.5/src/msscrawler/sites/shopping/website_pipeline.py` & `msscrawler-1.3.6/src/msscrawler/sites/shopping/website_pipeline.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.5/src/msscrawler/spiders/base.py` & `msscrawler-1.3.6/src/msscrawler/spiders/base.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.5/src/msscrawler/spiders/category.py` & `msscrawler-1.3.6/src/msscrawler/spiders/category.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.5/src/msscrawler/spiders/product.py` & `msscrawler-1.3.6/src/msscrawler/spiders/product.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.5/src/msscrawler/spiders/website.py` & `msscrawler-1.3.6/src/msscrawler/spiders/website.py`

 * *Files identical despite different names*

### Comparing `msscrawler-1.3.5/src/msscrawler.egg-info/PKG-INFO` & `msscrawler-1.3.6/src/msscrawler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msscrawler
-Version: 1.3.5
+Version: 1.3.6
 Summary: A common package for crawling
 Home-page: https://bitbucket.org/dosiin/common/src/package/
 Author: no name
 Author-email: msscrawler@gmail.com
 Project-URL: Bug Tracker, https://bitbucket.org/dosiin/common/src/package/issues
 Project-URL: repository, https://bitbucket.org/dosiin/common/src/package/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `msscrawler-1.3.5/src/msscrawler.egg-info/SOURCES.txt` & `msscrawler-1.3.6/src/msscrawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

