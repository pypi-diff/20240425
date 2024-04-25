# Comparing `tmp/invenio-app-ils-2.0.0rc8.tar.gz` & `tmp/invenio-app-ils-2.0.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-app-ils-2.0.0rc8.tar", last modified: Thu Apr  4 15:01:23 2024, max compression
+gzip compressed data, was "dist/invenio-app-ils-2.0.0rc9.tar", last modified: Thu Apr 25 06:58:47 2024, max compression
```

## Comparing `invenio-app-ils-2.0.0rc8.tar` & `invenio-app-ils-2.0.0rc9.tar`

### file list

```diff
@@ -1,790 +1,790 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15821 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/docker/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/docker/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docker/backend/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/docker/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docker/frontend/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/docker/frontend/conf.d/
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docker/frontend/conf.d/default.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docker/frontend/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docker/frontend/test.crt
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docker/frontend/test.key
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/docker/lb/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docker/lb/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docker/lb/haproxy.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docker/lb/haproxy_cert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docker-compose.full.yml
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docker-services.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10108 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/jsonresolvers/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/jsonresolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/jsonresolvers/order_order_lines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/jsonresolvers/order_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/loaders/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/loaders/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/loaders/jsonschemas/order.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/mappings/os-v1/acq_orders/
--rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/mappings/os-v1/acq_orders/order-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/mappings/os-v2/acq_orders/
--rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/mappings/os-v2/acq_orders/order-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/mappings/v7/acq_orders/
--rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/mappings/v7/acq_orders/order-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/schemas/acq_orders/
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/schemas/acq_orders/order-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11220 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10955 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/jsonresolvers/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/jsonresolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/jsonresolvers/loan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/loaders/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/loaders/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/loaders/schemas/json/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/loaders/schemas/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/loaders/schemas/json/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/loaders/schemas/json/bulk_extend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/loaders/schemas/json/loan_checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/loaders/schemas/json/loan_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/loaders/schemas/json/loan_update_dates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/notifications/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/notifications/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/notifications/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/receivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/serializers/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/serializers/custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/serializers/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/stats/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/stats/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/stats/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/bulk_extend.html
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/cancel.html
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/checkin.html
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/checkout.html
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/extend.html
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/overdue_reminder.html
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/request.html
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/request_no_items.html
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/will_expire_in_reminder.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/transitions/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/transitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/transitions/transitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7046 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/views.py
--rw-r--r--   0 runner    (1001) docker     (127)    57414 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/closures/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/closures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/closures/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/closures/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    40691 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/demo_data/
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/demo_data/documents.json
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/demo_data/items.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/jsonresolvers/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/jsonresolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/jsonresolvers/document_request_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/jsonresolvers/document_request_patron.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/loaders/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/loaders/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/loaders/jsonschemas/document_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_decline.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_document.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/mappings/os-v1/document_requests/
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/mappings/os-v1/document_requests/document_request-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/mappings/os-v2/document_requests/
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/mappings/os-v2/document_requests/document_request-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/mappings/v7/document_requests/
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/mappings/v7/document_requests/document_request-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/notifications/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/notifications/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/schemas/document_requests/
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/schemas/document_requests/document_request-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_accept.html
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_decline_in_catalog.html
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_decline_not_found.html
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_decline_other.html
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_decline_user_cancel.html
--rw-r--r--   0 runner    (1001) docker     (127)     9544 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/jsonresolvers/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/jsonresolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/jsonresolvers/document_circulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/jsonresolvers/document_eitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/jsonresolvers/document_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/jsonresolvers/document_relations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/jsonresolvers/document_stock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/loaders/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/loaders/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/loaders/jsonschemas/document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/mappings/os-v1/documents/
--rw-r--r--   0 runner    (1001) docker     (127)    21341 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/mappings/os-v1/documents/document-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/mappings/os-v2/documents/
--rw-r--r--   0 runner    (1001) docker     (127)    21341 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/mappings/os-v2/documents/document-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/mappings/v7/documents/
--rw-r--r--   0 runner    (1001) docker     (127)    21341 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/mappings/v7/documents/document-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/schemas/documents/
--rw-r--r--   0 runner    (1001) docker     (127)    18138 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/schemas/documents/document-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/jsonresolvers/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/jsonresolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/jsonresolvers/eitem_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/jsonresolvers/eitem_files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/loaders/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/loaders/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/loaders/jsonschemas/eitems.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/mappings/os-v1/eitems/
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/mappings/os-v1/eitems/eitem-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/mappings/os-v2/eitems/
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/mappings/os-v2/eitems/eitem-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/mappings/v7/eitems/
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/mappings/v7/eitems/eitem-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/schemas/eitems/
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/schemas/eitems/eitem-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     9907 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/facets.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/fetchers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/files/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/files/receivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/files/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13301 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/jsonresolvers/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/jsonresolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/jsonresolvers/borrowing_request_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/jsonresolvers/borrowing_request_patron.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/jsonresolvers/borrowing_request_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/loaders/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/loaders/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/loaders/jsonschemas/borrowing_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/loaders/jsonschemas/patron_loan_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/loaders/jsonschemas/patron_loan_extension_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/mappings/os-v1/ill_borrowing_requests/
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/mappings/os-v1/ill_borrowing_requests/borrowing_request-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/mappings/os-v2/ill_borrowing_requests/
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/mappings/os-v2/ill_borrowing_requests/borrowing_request-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/mappings/v7/ill_borrowing_requests/
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/mappings/v7/ill_borrowing_requests/borrowing_request-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/notifications/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/notifications/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/schemas/ill_borrowing_requests/
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/schemas/ill_borrowing_requests/borrowing_request-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/serializers/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/serializers/custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/serializers/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/templates/invenio_app_ils_ill/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_accept.html
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_decline.html
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_request.html
--rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/jsonresolvers/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/jsonresolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/jsonresolvers/internal_location.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/loaders/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/loaders/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/loaders/jsonschemas/internal_location.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/mappings/os-v1/internal_locations/
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/mappings/os-v1/internal_locations/internal_location-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/mappings/os-v2/internal_locations/
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/mappings/os-v2/internal_locations/internal_location-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/mappings/v7/internal_locations/
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/mappings/v7/internal_locations/internal_location-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/schemas/internal_locations/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/schemas/internal_locations/internal_location-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/jsonresolvers/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/jsonresolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/jsonresolvers/item_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/jsonresolvers/item_internal_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/jsonresolvers/item_loan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/loaders/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/loaders/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/loaders/jsonschemas/items.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/mappings/os-v1/items/
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/mappings/os-v1/items/item-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/mappings/os-v2/items/
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/mappings/os-v2/items/item-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/mappings/v7/items/
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/mappings/v7/items/item-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/schemas/items/
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/schemas/items/item-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/items/serializers/item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/literature/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/literature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/literature/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/literature/covers_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/literature/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/literature/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/literature/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/literature/serializers/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/literature/serializers/custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/literature/serializers/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/loaders/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/loaders/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/loaders/jsonschemas/location.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/mappings/os-v1/locations/
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/mappings/os-v1/locations/location-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/mappings/os-v2/locations/
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/mappings/os-v2/locations/location-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/mappings/v7/locations/
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/mappings/v7/locations/location-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/receivers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/schemas/locations/
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/schemas/locations/location-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/minters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/notifications/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/notifications/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/notifications/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/notifications/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/notifications/backends/mail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/notifications/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/notifications/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/notifications/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/notifications/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/anonymization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/mappings/os-v1/patrons/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/mappings/os-v1/patrons/patron-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/mappings/os-v2/patrons/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/mappings/os-v2/patrons/patron-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/mappings/v7/patrons/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/mappings/v7/patrons/patron-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/loaders/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/loaders/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/loaders/jsonschemas/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/mappings/os-v1/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/mappings/os-v1/providers/provider-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/mappings/os-v2/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/mappings/os-v2/providers/provider-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/mappings/v7/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/mappings/v7/providers/provider-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/schemas/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/schemas/providers/provider-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records/jsonresolvers/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records/jsonresolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records/jsonresolvers/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records/listeners.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records/loaders/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records/loaders/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records/loaders/schemas/changed_by.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records/loaders/schemas/preserve_cover_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records/loaders/schemas/price.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records/metadata_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records/receivers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records/schemas/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records_relations/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records_relations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16763 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records_relations/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records_relations/indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records_relations/retriever.py
--rw-r--r--   0 runner    (1001) docker     (127)    14889 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/records_relations/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/relations/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/relations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14074 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/relations/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/relations/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/search_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/jsonresolvers/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/jsonresolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/jsonresolvers/series_relations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/loaders/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/loaders/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/loaders/jsonschemas/series.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/mappings/os-v1/series/
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/mappings/os-v1/series/series-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/mappings/os-v2/series/
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/mappings/os-v2/series/series-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/mappings/v7/series/
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/mappings/v7/series/series-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/schemas/series/
--rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/schemas/series/series-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/series/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/static/images/placeholder.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/static_pages/
--rw-r--r--   0 runner    (1001) docker     (127)    22084 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/static_pages/search_guide.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/aggregations/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/aggregations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/aggregations/aggr_file_download/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/aggregations/aggr_file_download/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/aggregations/aggr_file_download/os-v1/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/aggregations/aggr_file_download/os-v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/aggregations/aggr_file_download/os-v1/aggr-file-download-v1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/aggregations/aggr_file_download/os-v2/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/aggregations/aggr_file_download/os-v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/aggregations/aggr_file_download/os-v2/aggr-file-download-v1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/aggregations/aggr_file_download/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/aggregations/aggr_file_download/v7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/aggregations/aggr_file_download/v7/aggr-file-download-v1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/file_download/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/file_download/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/file_download/os-v1/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/file_download/os-v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/file_download/os-v1/file-download-v1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/file_download/os-v2/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/file_download/os-v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/file_download/os-v2/file-download-v1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/file_download/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/file_download/v7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/file_download/v7/file-download-v1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/templates/invenio_app_ils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/templates/invenio_app_ils/mail/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/templates/invenio_app_ils/mail/footer.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/templates/invenio_app_ils/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/templates/invenio_app_ils/notifications/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/templates/logged_out.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/translations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/translations/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/acq_mediums.json
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/acq_order_line_payment_modes.json
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/acq_order_line_purchase_types.json
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/acq_payment_modes.json
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/acq_recipients.json
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/affiliation_identifier_schemes.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/alternative_identifier_schemes.json
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/alternative_title_types.json
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/author_identifier_schemes.json
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/author_roles.json
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/author_types.json
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/conference_identifier_schemes.json
--rw-r--r--   0 runner    (1001) docker     (127)    20498 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/countries.json
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/currencies.json
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/docreq_payment_method.json
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/docreq_request_type.json
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/document_identifiers_materials.json
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/document_requests_mediums.json
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/document_subjects.json
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/eitem_sources.json
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/identifier_schemes.json
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/ill_item_types.json
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/ill_payment_modes.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/item_mediums.json
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/provider_types.json
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/series_identifier_schemes.json
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/series_url_access_restrictions.json
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/tags.json
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/jsonresolvers/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/jsonresolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/jsonresolvers/licenses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/mappings/os-v1/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/mappings/os-v1/vocabularies/vocabulary-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/mappings/os-v2/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/mappings/os-v2/vocabularies/vocabulary-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/mappings/v7/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/mappings/v7/vocabularies/vocabulary-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/schemas/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/schemas/vocabularies/vocabulary-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/sources/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/sources/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/sources/opendefinition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15821 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26919 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/invenio_app_ils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1603 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/run-tests.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      326 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/scripts/bootstrap
--rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/scripts/build_assets
--rwxr-xr-x   0 runner    (1001) docker     (127)      333 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/scripts/celery
--rwxr-xr-x   0 runner    (1001) docker     (127)      248 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/scripts/console
--rwxr-xr-x   0 runner    (1001) docker     (127)      412 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/scripts/server
--rwxr-xr-x   0 runner    (1001) docker     (127)      251 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/scripts/setup
--rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/scripts/update
--rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/tests/api/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/tests/api/acquisition/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/acquisition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/acquisition/test_acq_orders_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/acquisition/test_acq_orders_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/acquisition/test_acq_providers_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/tests/api/circulation/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/circulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/circulation/test_expired_loans.py
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/circulation/test_loan_bulk_extend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/circulation/test_loan_checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/circulation/test_loan_default_durations.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/circulation/test_loan_document_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/circulation/test_loan_extend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/circulation/test_loan_item_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/circulation/test_loan_item_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/circulation/test_loan_list_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/circulation/test_loan_patron_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    13696 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/circulation/test_loan_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/circulation/test_loan_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/circulation/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/tests/api/document_requests/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/document_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/document_requests/test_document_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/document_requests/test_document_requests_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/document_requests/test_notifications_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/tests/api/ill/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ill/test_ill_brw_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ill/test_ill_brw_reqs_patron_loan_create_action.py
--rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ill/test_ill_brw_reqs_patron_loan_extension_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ill/test_ill_brw_reqs_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ill/test_ill_providers_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/documents/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/documents/test_document_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/documents/test_document_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/documents/test_document_resolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/eitems/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/eitems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/eitems/test_eitems_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/eitems/test_eitems_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/eitems/test_files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/items/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/items/test_apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/items/test_items_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/items/test_items_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/items/test_items_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/records_relations/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/records_relations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/records_relations/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17969 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/records_relations/test_records_relations_parentchild.py
--rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/records_relations/test_records_relations_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    29301 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/records_relations/test_records_relations_siblings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/series/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/series/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/series/test_series_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/test_anonymization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/test_apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    10041 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/test_closures.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/test_facets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/test_internal_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/test_metadata_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/test_notifications_mails.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/test_notifications_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/test_patrons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/test_record_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/test_record_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/test_resolvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/api/ils/test_vocabularies.py
--rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/data/acq_orders.json
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/data/acq_providers.json
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/data/document_requests.json
--rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/data/documents.json
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/data/eitems.json
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/data/ill_borrowing_requests.json
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/data/ill_providers.json
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/data/internal_locations.json
--rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/data/items.json
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/data/loans.json
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/data/loans_most_loaned.json
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/data/locations.json
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/data/series.json
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/tests/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:23.000000 invenio-app-ils-2.0.0rc8/tests/templates/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/templates/notifications/blank.html
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/templates/notifications/title_body.html
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/templates/notifications/title_body_html.html
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/templates/notifications/title_body_html_ctx.html
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/templates/notifications/title_only.html
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/test_post_logout_redirect.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-04 15:01:18.000000 invenio-app-ils-2.0.0rc8/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15935 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/docker/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/docker/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docker/backend/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/docker/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docker/frontend/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/docker/frontend/conf.d/
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docker/frontend/conf.d/default.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docker/frontend/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docker/frontend/test.crt
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docker/frontend/test.key
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/docker/lb/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docker/lb/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docker/lb/haproxy.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docker/lb/haproxy_cert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docker-compose.full.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docker-services.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10108 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/jsonresolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/jsonresolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/jsonresolvers/order_order_lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/jsonresolvers/order_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/loaders/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/loaders/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/loaders/jsonschemas/order.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/mappings/os-v1/acq_orders/
+-rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/mappings/os-v1/acq_orders/order-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/mappings/os-v2/acq_orders/
+-rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/mappings/os-v2/acq_orders/order-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/mappings/v7/acq_orders/
+-rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/mappings/v7/acq_orders/order-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/schemas/acq_orders/
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/schemas/acq_orders/order-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11220 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10955 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/jsonresolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/jsonresolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/jsonresolvers/loan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/loaders/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/loaders/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/loaders/schemas/json/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/loaders/schemas/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/loaders/schemas/json/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/loaders/schemas/json/bulk_extend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/loaders/schemas/json/loan_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/loaders/schemas/json/loan_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/loaders/schemas/json/loan_update_dates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/notifications/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/notifications/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/notifications/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/serializers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/serializers/custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/serializers/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/stats/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/stats/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/bulk_extend.html
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/cancel.html
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/checkin.html
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/checkout.html
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/extend.html
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/overdue_reminder.html
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/request.html
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/request_no_items.html
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/will_expire_in_reminder.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/transitions/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/transitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/transitions/transitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7046 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57414 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/closures/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/closures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/closures/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/closures/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40691 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/demo_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/demo_data/documents.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/demo_data/items.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/jsonresolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/jsonresolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/jsonresolvers/document_request_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/jsonresolvers/document_request_patron.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/loaders/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/loaders/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/loaders/jsonschemas/document_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_decline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/mappings/os-v1/document_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/mappings/os-v1/document_requests/document_request-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/mappings/os-v2/document_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/mappings/os-v2/document_requests/document_request-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/mappings/v7/document_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/mappings/v7/document_requests/document_request-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/notifications/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/notifications/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/schemas/document_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/schemas/document_requests/document_request-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_accept.html
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_decline_in_catalog.html
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_decline_not_found.html
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_decline_other.html
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_decline_user_cancel.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9544 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/jsonresolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/jsonresolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/jsonresolvers/document_circulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/jsonresolvers/document_eitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/jsonresolvers/document_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/jsonresolvers/document_relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/jsonresolvers/document_stock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/loaders/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/loaders/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/loaders/jsonschemas/document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/mappings/os-v1/documents/
+-rw-r--r--   0 runner    (1001) docker     (127)    21341 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/mappings/os-v1/documents/document-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/mappings/os-v2/documents/
+-rw-r--r--   0 runner    (1001) docker     (127)    21341 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/mappings/os-v2/documents/document-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/mappings/v7/documents/
+-rw-r--r--   0 runner    (1001) docker     (127)    21341 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/mappings/v7/documents/document-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/schemas/documents/
+-rw-r--r--   0 runner    (1001) docker     (127)    18138 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/schemas/documents/document-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/jsonresolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/jsonresolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/jsonresolvers/eitem_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/jsonresolvers/eitem_files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/loaders/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/loaders/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/loaders/jsonschemas/eitems.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/mappings/os-v1/eitems/
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/mappings/os-v1/eitems/eitem-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/mappings/os-v2/eitems/
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/mappings/os-v2/eitems/eitem-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/mappings/v7/eitems/
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/mappings/v7/eitems/eitem-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/schemas/eitems/
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/schemas/eitems/eitem-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9942 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/fetchers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/files/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/files/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13301 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/jsonresolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/jsonresolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/jsonresolvers/borrowing_request_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/jsonresolvers/borrowing_request_patron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/jsonresolvers/borrowing_request_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/loaders/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/loaders/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/loaders/jsonschemas/borrowing_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/loaders/jsonschemas/patron_loan_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/loaders/jsonschemas/patron_loan_extension_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/mappings/os-v1/ill_borrowing_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/mappings/os-v1/ill_borrowing_requests/borrowing_request-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/mappings/os-v2/ill_borrowing_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/mappings/os-v2/ill_borrowing_requests/borrowing_request-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/mappings/v7/ill_borrowing_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/mappings/v7/ill_borrowing_requests/borrowing_request-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/notifications/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/notifications/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/schemas/ill_borrowing_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/schemas/ill_borrowing_requests/borrowing_request-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/serializers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/serializers/custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/serializers/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/templates/invenio_app_ils_ill/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_accept.html
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_decline.html
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_request.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/jsonresolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/jsonresolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/jsonresolvers/internal_location.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/loaders/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/loaders/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/loaders/jsonschemas/internal_location.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/mappings/os-v1/internal_locations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/mappings/os-v1/internal_locations/internal_location-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/mappings/os-v2/internal_locations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/mappings/os-v2/internal_locations/internal_location-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/mappings/v7/internal_locations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/mappings/v7/internal_locations/internal_location-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/schemas/internal_locations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/schemas/internal_locations/internal_location-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/jsonresolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/jsonresolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/jsonresolvers/item_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/jsonresolvers/item_internal_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/jsonresolvers/item_loan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/loaders/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/loaders/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/loaders/jsonschemas/items.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/mappings/os-v1/items/
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/mappings/os-v1/items/item-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/mappings/os-v2/items/
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/mappings/os-v2/items/item-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/mappings/v7/items/
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/mappings/v7/items/item-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/schemas/items/
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/schemas/items/item-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/items/serializers/item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/literature/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/literature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/literature/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/literature/covers_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/literature/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/literature/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/literature/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/literature/serializers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/literature/serializers/custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/literature/serializers/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/loaders/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/loaders/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/loaders/jsonschemas/location.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/mappings/os-v1/locations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/mappings/os-v1/locations/location-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/mappings/os-v2/locations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/mappings/os-v2/locations/location-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/mappings/v7/locations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/mappings/v7/locations/location-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/receivers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/schemas/locations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/schemas/locations/location-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/minters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/notifications/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/notifications/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/notifications/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/notifications/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/notifications/backends/mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/notifications/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/notifications/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/notifications/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/notifications/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/anonymization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/mappings/os-v1/patrons/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/mappings/os-v1/patrons/patron-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/mappings/os-v2/patrons/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/mappings/os-v2/patrons/patron-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/mappings/v7/patrons/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/mappings/v7/patrons/patron-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/loaders/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/loaders/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/loaders/jsonschemas/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/mappings/os-v1/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/mappings/os-v1/providers/provider-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/mappings/os-v2/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/mappings/os-v2/providers/provider-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/mappings/v7/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/mappings/v7/providers/provider-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/schemas/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/schemas/providers/provider-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records/jsonresolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records/jsonresolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records/jsonresolvers/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records/listeners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records/loaders/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records/loaders/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records/loaders/schemas/changed_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records/loaders/schemas/preserve_cover_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records/loaders/schemas/price.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records/metadata_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records/receivers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records/schemas/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records_relations/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records_relations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16763 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records_relations/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records_relations/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records_relations/retriever.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14889 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/records_relations/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/relations/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/relations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14074 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/relations/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/relations/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/search_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/jsonresolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/jsonresolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/jsonresolvers/series_relations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/loaders/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/loaders/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/loaders/jsonschemas/series.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/mappings/os-v1/series/
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/mappings/os-v1/series/series-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/mappings/os-v2/series/
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/mappings/os-v2/series/series-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/mappings/v7/series/
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/mappings/v7/series/series-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/schemas/series/
+-rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/schemas/series/series-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/series/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/static/images/placeholder.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/static_pages/
+-rw-r--r--   0 runner    (1001) docker     (127)    22084 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/static_pages/search_guide.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/aggregations/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/aggregations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/aggregations/aggr_file_download/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/aggregations/aggr_file_download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/aggregations/aggr_file_download/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/aggregations/aggr_file_download/os-v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/aggregations/aggr_file_download/os-v1/aggr-file-download-v1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/aggregations/aggr_file_download/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/aggregations/aggr_file_download/os-v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/aggregations/aggr_file_download/os-v2/aggr-file-download-v1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/aggregations/aggr_file_download/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/aggregations/aggr_file_download/v7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/aggregations/aggr_file_download/v7/aggr-file-download-v1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/file_download/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/file_download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/file_download/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/file_download/os-v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/file_download/os-v1/file-download-v1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/file_download/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/file_download/os-v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/file_download/os-v2/file-download-v1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/file_download/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/file_download/v7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/file_download/v7/file-download-v1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/templates/invenio_app_ils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/templates/invenio_app_ils/mail/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/templates/invenio_app_ils/mail/footer.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/templates/invenio_app_ils/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/templates/invenio_app_ils/notifications/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/templates/logged_out.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/translations/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/acq_mediums.json
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/acq_order_line_payment_modes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/acq_order_line_purchase_types.json
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/acq_payment_modes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/acq_recipients.json
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/affiliation_identifier_schemes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/alternative_identifier_schemes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/alternative_title_types.json
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/author_identifier_schemes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/author_roles.json
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/author_types.json
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/conference_identifier_schemes.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20498 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/countries.json
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/currencies.json
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/docreq_payment_method.json
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/docreq_request_type.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/document_identifiers_materials.json
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/document_requests_mediums.json
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/document_subjects.json
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/eitem_sources.json
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/identifier_schemes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/ill_item_types.json
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/ill_payment_modes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/item_mediums.json
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/provider_types.json
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/series_identifier_schemes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/series_url_access_restrictions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/tags.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/jsonresolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/jsonresolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/jsonresolvers/licenses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/mappings/os-v1/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/mappings/os-v1/vocabularies/vocabulary-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/mappings/os-v2/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/mappings/os-v2/vocabularies/vocabulary-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/mappings/v7/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/mappings/v7/vocabularies/vocabulary-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/schemas/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/schemas/vocabularies/vocabulary-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/sources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/sources/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/sources/opendefinition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15935 2024-04-25 06:58:46.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26919 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 06:58:46.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-04-25 06:58:46.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 06:58:46.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-25 06:58:46.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 06:58:46.000000 invenio-app-ils-2.0.0rc9/invenio_app_ils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1603 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/run-tests.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      326 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/scripts/bootstrap
+-rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/scripts/build_assets
+-rwxr-xr-x   0 runner    (1001) docker     (127)      333 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/scripts/celery
+-rwxr-xr-x   0 runner    (1001) docker     (127)      248 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/scripts/console
+-rwxr-xr-x   0 runner    (1001) docker     (127)      412 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/scripts/server
+-rwxr-xr-x   0 runner    (1001) docker     (127)      251 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/scripts/setup
+-rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/scripts/update
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/tests/api/acquisition/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/acquisition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/acquisition/test_acq_orders_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/acquisition/test_acq_orders_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/acquisition/test_acq_providers_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/tests/api/circulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/circulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/circulation/test_expired_loans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/circulation/test_loan_bulk_extend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/circulation/test_loan_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/circulation/test_loan_default_durations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/circulation/test_loan_document_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/circulation/test_loan_extend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/circulation/test_loan_item_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/circulation/test_loan_item_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/circulation/test_loan_list_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/circulation/test_loan_patron_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13696 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/circulation/test_loan_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/circulation/test_loan_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/circulation/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/tests/api/document_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/document_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/document_requests/test_document_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/document_requests/test_document_requests_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/document_requests/test_notifications_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/tests/api/ill/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ill/test_ill_brw_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ill/test_ill_brw_reqs_patron_loan_create_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ill/test_ill_brw_reqs_patron_loan_extension_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ill/test_ill_brw_reqs_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ill/test_ill_providers_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/documents/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/documents/test_document_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/documents/test_document_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/documents/test_document_resolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/eitems/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/eitems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/eitems/test_eitems_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/eitems/test_eitems_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/eitems/test_files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/items/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/items/test_apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/items/test_items_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/items/test_items_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/items/test_items_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/records_relations/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/records_relations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/records_relations/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17969 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/records_relations/test_records_relations_parentchild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/records_relations/test_records_relations_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29301 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/records_relations/test_records_relations_siblings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/series/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/series/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/series/test_series_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/test_anonymization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/test_apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10041 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/test_closures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/test_facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/test_internal_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/test_metadata_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/test_notifications_mails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/test_notifications_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/test_patrons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/test_record_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/test_record_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/test_resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/api/ils/test_vocabularies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/data/acq_orders.json
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/data/acq_providers.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/data/document_requests.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/data/documents.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/data/eitems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/data/ill_borrowing_requests.json
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/data/ill_providers.json
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/data/internal_locations.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/data/items.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/data/loans.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/data/loans_most_loaned.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/data/locations.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/data/series.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/tests/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:47.000000 invenio-app-ils-2.0.0rc9/tests/templates/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/templates/notifications/blank.html
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/templates/notifications/title_body.html
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/templates/notifications/title_body_html.html
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/templates/notifications/title_body_html_ctx.html
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/templates/notifications/title_only.html
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/test_post_logout_redirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-25 06:58:41.000000 invenio-app-ils-2.0.0rc9/tests/test_version.py
```

### Comparing `invenio-app-ils-2.0.0rc8/.editorconfig` & `invenio-app-ils-2.0.0rc9/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/CHANGES.rst` & `invenio-app-ils-2.0.0rc9/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
     invenio-app-ils is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 2.0.0rc9 (released 2024-04-25)
+
+- patch: add record pid to error display
+
 Version 2.0.0rc8 (released 2024-04-04)
 
 - records_relation: Simplify sorting
 - records_relations: Use sort_by paramemter from configs instead
 - relations: Add functionality to sort json refs by relation_type
 - tests: circulation: Add new location for testing closures
 - circulation: loan_request: Fix dates comparison in get_offset_duration
```

### Comparing `invenio-app-ils-2.0.0rc8/CONTRIBUTING.rst` & `invenio-app-ils-2.0.0rc9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/LICENSE` & `invenio-app-ils-2.0.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/MANIFEST.in` & `invenio-app-ils-2.0.0rc9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/PKG-INFO` & `invenio-app-ils-2.0.0rc9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-app-ils
-Version: 2.0.0rc8
+Version: 2.0.0rc9
 Summary: Invenio Integrated Library System.
 Home-page: https://github.com/inveniosoftware/invenio-app-ils
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2018-2020 CERN.
@@ -36,14 +36,18 @@
         
             invenio-app-ils is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.0.0rc9 (released 2024-04-25)
+        
+        - patch: add record pid to error display
+        
         Version 2.0.0rc8 (released 2024-04-04)
         
         - records_relation: Simplify sorting
         - records_relations: Use sort_by paramemter from configs instead
         - relations: Add functionality to sort json refs by relation_type
         - tests: circulation: Add new location for testing closures
         - circulation: loan_request: Fix dates comparison in get_offset_duration
```

### Comparing `invenio-app-ils-2.0.0rc8/README.rst` & `invenio-app-ils-2.0.0rc9/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/docker/backend/Dockerfile` & `invenio-app-ils-2.0.0rc9/docker/backend/Dockerfile`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/docker/frontend/Dockerfile` & `invenio-app-ils-2.0.0rc9/docker/frontend/Dockerfile`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/docker/frontend/conf.d/default.conf` & `invenio-app-ils-2.0.0rc9/docker/frontend/conf.d/default.conf`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/docker/frontend/nginx.conf` & `invenio-app-ils-2.0.0rc9/docker/frontend/nginx.conf`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/docker/frontend/test.crt` & `invenio-app-ils-2.0.0rc9/docker/frontend/test.crt`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/docker/frontend/test.key` & `invenio-app-ils-2.0.0rc9/docker/frontend/test.key`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/docker/lb/haproxy.cfg` & `invenio-app-ils-2.0.0rc9/docker/lb/haproxy.cfg`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/docker/lb/haproxy_cert.pem` & `invenio-app-ils-2.0.0rc9/docker/lb/haproxy_cert.pem`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/docker-compose.full.yml` & `invenio-app-ils-2.0.0rc9/docker-compose.full.yml`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/docker-compose.yml` & `invenio-app-ils-2.0.0rc9/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/docker-services.yml` & `invenio-app-ils-2.0.0rc9/docker-services.yml`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/docs/Makefile` & `invenio-app-ils-2.0.0rc9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/docs/conf.py` & `invenio-app-ils-2.0.0rc9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/docs/index.rst` & `invenio-app-ils-2.0.0rc9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/docs/make.bat` & `invenio-app-ils-2.0.0rc9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/config.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/config.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/ext.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/jsonresolvers/order_order_lines.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/jsonresolvers/order_order_lines.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/jsonresolvers/order_provider.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/jsonresolvers/order_provider.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/loaders/jsonschemas/order.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/loaders/jsonschemas/order.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/mappings/os-v1/acq_orders/order-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/mappings/os-v1/acq_orders/order-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/mappings/os-v2/acq_orders/order-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/mappings/os-v2/acq_orders/order-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/mappings/v7/acq_orders/order-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/mappings/v7/acq_orders/order-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/schemas/acq_orders/order-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/schemas/acq_orders/order-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/acquisition/search.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/acquisition/search.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/config.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/config.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/indexer.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/jsonresolvers/loan.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/jsonresolvers/loan.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/loaders/__init__.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/loaders/schemas/json/base.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/loaders/schemas/json/base.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/loaders/schemas/json/bulk_extend.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/loaders/schemas/json/bulk_extend.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/loaders/schemas/json/loan_checkout.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/loaders/schemas/json/loan_checkout.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/loaders/schemas/json/loan_request.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/loaders/schemas/json/loan_request.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/loaders/schemas/json/loan_update_dates.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/loaders/schemas/json/loan_update_dates.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/notifications/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/notifications/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/notifications/messages.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/notifications/messages.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/notifications/tasks.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/notifications/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/receivers.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/receivers.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/search.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/search.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/serializers/__init__.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/serializers/csv.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/serializers/csv.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/serializers/custom_fields.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/serializers/custom_fields.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/serializers/json.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/serializers/json.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/serializers/response.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/serializers/response.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/stats/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/stats/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/stats/views.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/stats/views.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/tasks.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/bulk_extend.html` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/bulk_extend.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/cancel.html` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/cancel.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/checkin.html` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/checkin.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/checkout.html` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/checkout.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/extend.html` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/extend.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/overdue_reminder.html` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/overdue_reminder.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/request.html` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/request.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/request_no_items.html` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/request_no_items.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/will_expire_in_reminder.html` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/templates/invenio_app_ils_circulation/notifications/will_expire_in_reminder.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/transitions/transitions.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/transitions/transitions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/utils.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/circulation/views.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/circulation/views.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/cli.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/closures/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/closures/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/closures/tasks.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/closures/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/config.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/config.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/demo_data/documents.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/demo_data/documents.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/demo_data/items.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/demo_data/items.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/indexer.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/jsonresolvers/document_request_document.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/jsonresolvers/document_request_document.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/jsonresolvers/document_request_patron.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/jsonresolvers/document_request_patron.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/loaders/__init__.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/loaders/jsonschemas/document_request.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/loaders/jsonschemas/document_request.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_decline.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_decline.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_document.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_document.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_provider.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/loaders/jsonschemas/document_request_provider.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/mappings/os-v1/document_requests/document_request-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/mappings/os-v1/document_requests/document_request-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/mappings/os-v2/document_requests/document_request-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/mappings/os-v2/document_requests/document_request-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/mappings/v7/document_requests/document_request-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/mappings/v7/document_requests/document_request-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/notifications/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/notifications/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/notifications/messages.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/notifications/messages.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/schemas/document_requests/document_request-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/schemas/document_requests/document_request-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/search.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/search.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_decline_in_catalog.html` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/templates/invenio_app_ils_document_requests/notifications/document_request_decline_in_catalog.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/document_requests/views.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/document_requests/views.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/indexer.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/jsonresolvers/document_circulation.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/jsonresolvers/document_circulation.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/jsonresolvers/document_eitem.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/jsonresolvers/document_eitem.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/jsonresolvers/document_item.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/jsonresolvers/document_item.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/jsonresolvers/document_relations.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/jsonresolvers/document_relations.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/jsonresolvers/document_stock.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/jsonresolvers/document_stock.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/loaders/jsonschemas/document.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/loaders/jsonschemas/document.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/mappings/os-v1/documents/document-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/mappings/os-v1/documents/document-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/mappings/os-v2/documents/document-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/mappings/os-v2/documents/document-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/mappings/v7/documents/document-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/mappings/v7/documents/document-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/schemas/documents/document-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/schemas/documents/document-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/documents/search.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/documents/search.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/indexer.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/jsonresolvers/eitem_document.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/jsonresolvers/eitem_document.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/jsonresolvers/eitem_files.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/jsonresolvers/eitem_files.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/loaders/jsonschemas/eitems.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/loaders/jsonschemas/eitems.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/mappings/os-v1/eitems/eitem-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/mappings/os-v1/eitems/eitem-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/mappings/os-v2/eitems/eitem-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/mappings/os-v2/eitems/eitem-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/mappings/v7/eitems/eitem-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/mappings/v7/eitems/eitem-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/schemas/eitems/eitem-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/schemas/eitems/eitem-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/eitems/search.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/eitems/search.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/errors.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,15 @@
         super().__init__(**kwargs)
         self.description = self.description.format(
             record_type=record_type,
             record_id=record_id,
             ref_type=ref_type,
             ref_ids=ref_ids,
         )
+        self.record_id = record_id
 
 
 class ItemHasActiveLoanError(IlsException):
     """The item which we are trying to update has an active loan."""
 
     description = (
         "Could not update item because it has an active loan with " "pid: {loan_pid}."
```

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ext.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/facets.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/facets.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/fetchers.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/fetchers.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/files/receivers.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/files/receivers.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/files/views.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/files/views.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/config.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/config.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/errors.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/ext.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/jsonresolvers/borrowing_request_document.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/jsonresolvers/borrowing_request_document.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/jsonresolvers/borrowing_request_patron.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/jsonresolvers/borrowing_request_patron.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/jsonresolvers/borrowing_request_provider.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/jsonresolvers/borrowing_request_provider.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/loaders/__init__.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/loaders/jsonschemas/borrowing_request.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/loaders/jsonschemas/borrowing_request.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/loaders/jsonschemas/patron_loan_actions.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/loaders/jsonschemas/patron_loan_actions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/loaders/jsonschemas/patron_loan_extension_actions.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/loaders/jsonschemas/patron_loan_extension_actions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/mappings/os-v1/ill_borrowing_requests/borrowing_request-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/mappings/os-v1/ill_borrowing_requests/borrowing_request-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/mappings/os-v2/ill_borrowing_requests/borrowing_request-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/mappings/os-v2/ill_borrowing_requests/borrowing_request-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/mappings/v7/ill_borrowing_requests/borrowing_request-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/mappings/v7/ill_borrowing_requests/borrowing_request-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/notifications/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/notifications/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/notifications/messages.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/notifications/messages.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/schemas/ill_borrowing_requests/borrowing_request-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/schemas/ill_borrowing_requests/borrowing_request-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/search.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/search.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/serializers/__init__.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/serializers/csv.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/serializers/csv.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/serializers/custom_fields.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/serializers/custom_fields.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/serializers/json.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/serializers/json.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_accept.html` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_accept.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_decline.html` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_decline.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_request.html` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/templates/invenio_app_ils_ill/notifications/patron_loan_extension_request.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/ill/views.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/ill/views.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/indexer.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/indexer.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/jsonresolvers/internal_location.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/jsonresolvers/internal_location.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/loaders/__init__.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/loaders/jsonschemas/internal_location.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/loaders/jsonschemas/internal_location.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/mappings/os-v1/internal_locations/internal_location-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/mappings/os-v1/internal_locations/internal_location-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/mappings/os-v2/internal_locations/internal_location-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/mappings/os-v2/internal_locations/internal_location-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/mappings/v7/internal_locations/internal_location-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/mappings/v7/internal_locations/internal_location-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/schemas/internal_locations/internal_location-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/schemas/internal_locations/internal_location-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/internal_locations/search.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/internal_locations/search.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/items/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/items/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/items/indexer.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/items/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/items/jsonresolvers/item_document.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/items/jsonresolvers/item_document.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/items/jsonresolvers/item_internal_location.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/items/jsonresolvers/item_internal_location.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/items/jsonresolvers/item_loan.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/items/jsonresolvers/item_loan.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/items/loaders/jsonschemas/items.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/items/loaders/jsonschemas/items.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/items/mappings/os-v1/items/item-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/items/mappings/os-v1/items/item-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/items/mappings/os-v2/items/item-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/items/mappings/os-v2/items/item-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/items/mappings/v7/items/item-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/items/mappings/v7/items/item-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/items/schemas/items/item-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/items/schemas/items/item-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/items/search.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/items/search.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/items/serializers/__init__.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/items/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/items/serializers/item.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/items/serializers/item.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/literature/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/literature/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/literature/covers_builder.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/literature/covers_builder.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/literature/search.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/literature/search.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/literature/serializers/__init__.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/literature/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/literature/serializers/csv.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/literature/serializers/csv.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/literature/serializers/custom_fields.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/literature/serializers/custom_fields.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/literature/serializers/json.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/literature/serializers/json.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/indexer.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/loaders/jsonschemas/location.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/loaders/jsonschemas/location.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/mappings/os-v1/locations/location-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/mappings/os-v1/locations/location-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/mappings/os-v2/locations/location-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/mappings/os-v2/locations/location-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/mappings/v7/locations/location-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/mappings/v7/locations/location-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/receivers.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/receivers.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/locations/schemas/locations/location-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/locations/schemas/locations/location-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/minters.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/minters.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/notifications/admin.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/notifications/admin.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/notifications/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/notifications/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/notifications/backends/mail.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/notifications/backends/mail.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/notifications/messages.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/notifications/messages.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/notifications/models.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/notifications/models.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/notifications/tasks.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/notifications/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/notifications/views.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/notifications/views.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/anonymization.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/anonymization.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/cli.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/indexer.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/mappings/os-v1/patrons/patron-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/mappings/os-v1/patrons/patron-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/mappings/os-v2/patrons/patron-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/mappings/os-v2/patrons/patron-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/mappings/v7/patrons/patron-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/mappings/v7/patrons/patron-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/patrons/views.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/patrons/views.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/permissions.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/config.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/config.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/errors.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/ext.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/indexer.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/loaders/jsonschemas/provider.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/loaders/jsonschemas/provider.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/mappings/os-v1/providers/provider-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/mappings/os-v1/providers/provider-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/mappings/os-v2/providers/provider-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/mappings/os-v2/providers/provider-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/mappings/v7/providers/provider-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/mappings/v7/providers/provider-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/providers/schemas/providers/provider-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/providers/schemas/providers/provider-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/records/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/records/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/records/jsonresolvers/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/records/jsonresolvers/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/records/listeners.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/records/listeners.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/records/loaders/__init__.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/records/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/records/loaders/schemas/changed_by.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/records/loaders/schemas/changed_by.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/records/loaders/schemas/price.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/records/loaders/schemas/price.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/records/metadata_extensions.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/records/metadata_extensions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/records/permissions.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/records/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/records/schemas/json.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/records/schemas/json.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/records/serializers/__init__.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/records/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/records/views.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/records/views.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/records_relations/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/records_relations/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/records_relations/indexer.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/records_relations/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/records_relations/retriever.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/records_relations/retriever.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/records_relations/views.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/records_relations/views.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/relations/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/relations/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/search_permissions.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/search_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/series/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/series/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/series/indexer.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/series/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/series/jsonresolvers/series_relations.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/series/jsonresolvers/series_relations.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/series/loaders/jsonschemas/series.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/series/loaders/jsonschemas/series.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/series/mappings/os-v1/series/series-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/series/mappings/os-v1/series/series-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/series/mappings/os-v2/series/series-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/series/mappings/os-v2/series/series-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/series/mappings/v7/series/series-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/series/mappings/v7/series/series-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/series/schemas/series/series-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/series/schemas/series/series-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/series/search.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/series/search.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/static/images/placeholder.png` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/static/images/placeholder.png`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/static_pages/search_guide.html` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/static_pages/search_guide.html`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/aggregations/aggr_file_download/os-v1/aggr-file-download-v1.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/aggregations/aggr_file_download/os-v1/aggr-file-download-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/aggregations/aggr_file_download/os-v2/aggr-file-download-v1.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/aggregations/aggr_file_download/os-v2/aggr-file-download-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/aggregations/aggr_file_download/v7/aggr-file-download-v1.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/aggregations/aggr_file_download/v7/aggr-file-download-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/file_download/os-v1/file-download-v1.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/file_download/os-v1/file-download-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/file_download/os-v2/file-download-v1.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/file_download/os-v2/file-download-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/stats/file_download/v7/file-download-v1.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/stats/file_download/v7/file-download-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/views.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/views.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/api.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/api.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/cli.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/author_roles.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/author_roles.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/countries.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/countries.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/data/document_identifiers_materials.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/data/document_identifiers_materials.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/indexer.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/jsonresolvers/licenses.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/jsonresolvers/licenses.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/schemas/vocabularies/vocabulary-v1.0.0.json` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/schemas/vocabularies/vocabulary-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/search.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/search.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/sources/base.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/sources/base.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/sources/json.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/sources/json.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils/vocabularies/sources/opendefinition.py` & `invenio-app-ils-2.0.0rc9/invenio_app_ils/vocabularies/sources/opendefinition.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils.egg-info/PKG-INFO` & `invenio-app-ils-2.0.0rc9/invenio_app_ils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-app-ils
-Version: 2.0.0rc8
+Version: 2.0.0rc9
 Summary: Invenio Integrated Library System.
 Home-page: https://github.com/inveniosoftware/invenio-app-ils
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2018-2020 CERN.
@@ -36,14 +36,18 @@
         
             invenio-app-ils is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.0.0rc9 (released 2024-04-25)
+        
+        - patch: add record pid to error display
+        
         Version 2.0.0rc8 (released 2024-04-04)
         
         - records_relation: Simplify sorting
         - records_relations: Use sort_by paramemter from configs instead
         - relations: Add functionality to sort json refs by relation_type
         - tests: circulation: Add new location for testing closures
         - circulation: loan_request: Fix dates comparison in get_offset_duration
```

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils.egg-info/SOURCES.txt` & `invenio-app-ils-2.0.0rc9/invenio_app_ils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils.egg-info/entry_points.txt` & `invenio-app-ils-2.0.0rc9/invenio_app_ils.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/invenio_app_ils.egg-info/requires.txt` & `invenio-app-ils-2.0.0rc9/invenio_app_ils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/run-tests.sh` & `invenio-app-ils-2.0.0rc9/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/setup.cfg` & `invenio-app-ils-2.0.0rc9/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/acquisition/test_acq_orders_crud.py` & `invenio-app-ils-2.0.0rc9/tests/api/acquisition/test_acq_orders_crud.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/acquisition/test_acq_orders_permissions.py` & `invenio-app-ils-2.0.0rc9/tests/api/acquisition/test_acq_orders_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/acquisition/test_acq_providers_permissions.py` & `invenio-app-ils-2.0.0rc9/tests/api/acquisition/test_acq_providers_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/circulation/test_expired_loans.py` & `invenio-app-ils-2.0.0rc9/tests/api/circulation/test_expired_loans.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/circulation/test_loan_bulk_extend.py` & `invenio-app-ils-2.0.0rc9/tests/api/circulation/test_loan_bulk_extend.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/circulation/test_loan_checkout.py` & `invenio-app-ils-2.0.0rc9/tests/api/circulation/test_loan_checkout.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/circulation/test_loan_default_durations.py` & `invenio-app-ils-2.0.0rc9/tests/api/circulation/test_loan_default_durations.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/circulation/test_loan_document_resolver.py` & `invenio-app-ils-2.0.0rc9/tests/api/circulation/test_loan_document_resolver.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/circulation/test_loan_extend.py` & `invenio-app-ils-2.0.0rc9/tests/api/circulation/test_loan_extend.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/circulation/test_loan_item_permissions.py` & `invenio-app-ils-2.0.0rc9/tests/api/circulation/test_loan_item_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/circulation/test_loan_item_resolver.py` & `invenio-app-ils-2.0.0rc9/tests/api/circulation/test_loan_item_resolver.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/circulation/test_loan_list_permissions.py` & `invenio-app-ils-2.0.0rc9/tests/api/circulation/test_loan_list_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/circulation/test_loan_patron_resolver.py` & `invenio-app-ils-2.0.0rc9/tests/api/circulation/test_loan_patron_resolver.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/circulation/test_loan_request.py` & `invenio-app-ils-2.0.0rc9/tests/api/circulation/test_loan_request.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/circulation/test_loan_update.py` & `invenio-app-ils-2.0.0rc9/tests/api/circulation/test_loan_update.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/circulation/test_notifications.py` & `invenio-app-ils-2.0.0rc9/tests/api/circulation/test_notifications.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/conftest.py` & `invenio-app-ils-2.0.0rc9/tests/api/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/document_requests/test_document_requests.py` & `invenio-app-ils-2.0.0rc9/tests/api/document_requests/test_document_requests.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/document_requests/test_document_requests_permissions.py` & `invenio-app-ils-2.0.0rc9/tests/api/document_requests/test_document_requests_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/document_requests/test_notifications_filter.py` & `invenio-app-ils-2.0.0rc9/tests/api/document_requests/test_notifications_filter.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ill/test_ill_brw_crud.py` & `invenio-app-ils-2.0.0rc9/tests/api/ill/test_ill_brw_crud.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ill/test_ill_brw_reqs_patron_loan_create_action.py` & `invenio-app-ils-2.0.0rc9/tests/api/ill/test_ill_brw_reqs_patron_loan_create_action.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ill/test_ill_brw_reqs_patron_loan_extension_actions.py` & `invenio-app-ils-2.0.0rc9/tests/api/ill/test_ill_brw_reqs_patron_loan_extension_actions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ill/test_ill_brw_reqs_permissions.py` & `invenio-app-ils-2.0.0rc9/tests/api/ill/test_ill_brw_reqs_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ill/test_ill_providers_permissions.py` & `invenio-app-ils-2.0.0rc9/tests/api/ill/test_ill_providers_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/documents/test_document_crud.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/documents/test_document_crud.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/documents/test_document_permissions.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/documents/test_document_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/documents/test_document_resolvers.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/documents/test_document_resolvers.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/eitems/test_eitems_crud.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/eitems/test_eitems_crud.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/eitems/test_eitems_permissions.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/eitems/test_eitems_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/eitems/test_files.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/eitems/test_files.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/items/test_apis.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/items/test_apis.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/items/test_items_crud.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/items/test_items_crud.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/items/test_items_permissions.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/items/test_items_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/items/test_items_update.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/items/test_items_update.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/records_relations/helpers.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/records_relations/helpers.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/records_relations/test_records_relations_parentchild.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/records_relations/test_records_relations_parentchild.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/records_relations/test_records_relations_sequence.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/records_relations/test_records_relations_sequence.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/records_relations/test_records_relations_siblings.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/records_relations/test_records_relations_siblings.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/series/test_series_permissions.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/series/test_series_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/test_anonymization.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/test_anonymization.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/test_apis.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/test_apis.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/test_closures.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/test_closures.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/test_errors.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/test_errors.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/test_facets.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/test_facets.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/test_internal_locations.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/test_internal_locations.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/test_loaders.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/test_loaders.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/test_metadata_extensions.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/test_metadata_extensions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/test_notifications.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/test_notifications.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/test_notifications_mails.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/test_notifications_mails.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/test_notifications_permissions.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/test_notifications_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/test_patrons.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/test_patrons.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/test_record_delete.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/test_record_delete.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/test_record_permissions.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/test_record_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/test_resolvers.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/test_resolvers.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/test_stats.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/test_stats.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/test_tasks.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/test_tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/api/ils/test_vocabularies.py` & `invenio-app-ils-2.0.0rc9/tests/api/ils/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/conftest.py` & `invenio-app-ils-2.0.0rc9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/data/acq_orders.json` & `invenio-app-ils-2.0.0rc9/tests/data/acq_orders.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/data/document_requests.json` & `invenio-app-ils-2.0.0rc9/tests/data/document_requests.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/data/documents.json` & `invenio-app-ils-2.0.0rc9/tests/data/documents.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/data/eitems.json` & `invenio-app-ils-2.0.0rc9/tests/data/eitems.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/data/ill_borrowing_requests.json` & `invenio-app-ils-2.0.0rc9/tests/data/ill_borrowing_requests.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/data/items.json` & `invenio-app-ils-2.0.0rc9/tests/data/items.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/data/loans.json` & `invenio-app-ils-2.0.0rc9/tests/data/loans.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/data/loans_most_loaned.json` & `invenio-app-ils-2.0.0rc9/tests/data/loans_most_loaned.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/data/locations.json` & `invenio-app-ils-2.0.0rc9/tests/data/locations.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/data/series.json` & `invenio-app-ils-2.0.0rc9/tests/data/series.json`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/helpers.py` & `invenio-app-ils-2.0.0rc9/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `invenio-app-ils-2.0.0rc8/tests/test_post_logout_redirect.py` & `invenio-app-ils-2.0.0rc9/tests/test_post_logout_redirect.py`

 * *Files identical despite different names*

