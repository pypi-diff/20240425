# Comparing `tmp/alteia-2.9.0.tar.gz` & `tmp/alteia-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alteia-2.9.0.tar", max compression
+gzip compressed data, was "alteia-2.9.1.tar", max compression
```

## Comparing `alteia-2.9.0.tar` & `alteia-2.9.1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0     1084 2023-10-26 13:51:12.990179 alteia-2.9.0/LICENSE
--rw-r--r--   0        0        0     1426 2023-10-26 13:51:12.990179 alteia-2.9.0/README.md
--rw-r--r--   0        0        0      257 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/__init__.py
--rw-r--r--   0        0        0        0 2023-10-26 13:51:13.118179 alteia-2.9.0/alteia/apis/__init__.py
--rw-r--r--   0        0        0        0 2023-10-26 13:51:13.118179 alteia-2.9.0/alteia/apis/client/__init__.py
--rw-r--r--   0        0        0        0 2023-10-26 13:51:13.118179 alteia-2.9.0/alteia/apis/client/analytics/__init__.py
--rw-r--r--   0        0        0    26328 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/analytics/analyticsimpl.py
--rwxr-xr-x   0        0        0    16721 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/analytics/configurationsimpl.py
--rw-r--r--   0        0        0     7927 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/analytics/productsimpl.py
--rw-r--r--   0        0        0        0 2023-10-26 13:51:13.118179 alteia-2.9.0/alteia/apis/client/annotations/__init__.py
--rw-r--r--   0        0        0    30043 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/annotations/annotationsimpl.py
--rw-r--r--   0        0        0        0 2023-10-26 13:51:13.118179 alteia-2.9.0/alteia/apis/client/auth/__init__.py
--rw-r--r--   0        0        0     4227 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/auth/companiesimpl.py
--rw-r--r--   0        0        0     4316 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/auth/oauthclientsimpl.py
--rw-r--r--   0        0        0     5681 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/auth/sharetokensimpl.py
--rw-r--r--   0        0        0     3619 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/auth/usersimpl.py
--rw-r--r--   0        0        0        0 2023-10-26 13:51:13.118179 alteia-2.9.0/alteia/apis/client/comments/__init__.py
--rw-r--r--   0        0        0     7097 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/comments/commentsimpl.py
--rw-r--r--   0        0        0        0 2023-10-26 13:51:13.118179 alteia-2.9.0/alteia/apis/client/credentials/__init__.py
--rw-r--r--   0        0        0     7742 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/credentials/credentialsimpl.py
--rw-r--r--   0        0        0        0 2023-10-26 13:51:13.118179 alteia-2.9.0/alteia/apis/client/datacapture/__init__.py
--rw-r--r--   0        0        0     4263 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/datacapture/carriersimpl.py
--rw-r--r--   0        0        0     5288 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/datacapture/carriersmodelsimpl.py
--rw-r--r--   0        0        0    11560 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/datacapture/collectiontasksimpl.py
--rw-r--r--   0        0        0     1445 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/datacapture/pilotsimpl.py
--rw-r--r--   0        0        0     4924 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/datacapture/teamsimpl.py
--rw-r--r--   0        0        0       94 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/datamngt/__init__.py
--rw-r--r--   0        0        0    49466 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/datamngt/datasetsimpl.py
--rw-r--r--   0        0        0        0 2023-10-26 13:51:13.118179 alteia-2.9.0/alteia/apis/client/datastream/__init__.py
--rw-r--r--   0        0        0     3757 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/datastream/datastreamassetmonitoredimpl.py
--rw-r--r--   0        0        0     3705 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/datastream/datastreamsfilesimpl.py
--rw-r--r--   0        0        0     6023 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/datastream/datastreamsimpl.py
--rw-r--r--   0        0        0     8351 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/datastreamtemplate/datastreamtemplateimpl.py
--rw-r--r--   0        0        0        0 2023-10-26 13:51:13.118179 alteia-2.9.0/alteia/apis/client/featuresservice/__init__.py
--rw-r--r--   0        0        0     6443 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/featuresservice/collectionsimpl.py
--rw-r--r--   0        0        0    12604 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/featuresservice/featuresimpl.py
--rw-r--r--   0        0        0        0 2023-10-26 13:51:13.118179 alteia-2.9.0/alteia/apis/client/projectmngt/__init__.py
--rw-r--r--   0        0        0    14906 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/projectmngt/flightsimpl.py
--rw-r--r--   0        0        0    20382 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/projectmngt/missionsimpl.py
--rw-r--r--   0        0        0    18356 2023-10-26 13:51:12.990179 alteia-2.9.0/alteia/apis/client/projectmngt/projectsimpl.py
--rw-r--r--   0        0        0        0 2023-10-26 13:51:13.118179 alteia-2.9.0/alteia/apis/client/tags/__init__.py
--rw-r--r--   0        0        0     5779 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/apis/client/tags/tagsimpl.py
--rw-r--r--   0        0        0     6637 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/apis/provider.py
--rw-r--r--   0        0        0        0 2023-10-26 13:51:13.118179 alteia-2.9.0/alteia/core/__init__.py
--rw-r--r--   0        0        0     3023 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/config.py
--rw-r--r--   0        0        0        0 2023-10-26 13:51:13.118179 alteia-2.9.0/alteia/core/connection/__init__.py
--rw-r--r--   0        0        0     2853 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/connection/abstract_connection.py
--rw-r--r--   0        0        0     4115 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/connection/async_connection.py
--rw-r--r--   0        0        0     6077 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/connection/connection.py
--rw-r--r--   0        0        0     1441 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/connection/credentials.py
--rw-r--r--   0        0        0     3202 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/connection/token.py
--rw-r--r--   0        0        0     1527 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/errors.py
--rw-r--r--   0        0        0        0 2023-10-26 13:51:13.118179 alteia-2.9.0/alteia/core/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-10-26 13:51:13.118179 alteia-2.9.0/alteia/core/resources/analytics/__init__.py
--rw-r--r--   0        0        0      364 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/resources/analytics/products.py
--rw-r--r--   0        0        0     1734 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/resources/comments.py
--rw-r--r--   0        0        0        0 2023-10-26 13:51:13.118179 alteia-2.9.0/alteia/core/resources/datamngt/__init__.py
--rw-r--r--   0        0        0    11346 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/resources/datamngt/upload.py
--rw-r--r--   0        0        0        0 2023-10-26 13:51:13.118179 alteia-2.9.0/alteia/core/resources/projectmngt/__init__.py
--rw-r--r--   0        0        0      636 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/resources/projectmngt/flights.py
--rw-r--r--   0        0        0      914 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/resources/projectmngt/missions.py
--rw-r--r--   0        0        0     1105 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/resources/projectmngt/projects.py
--rw-r--r--   0        0        0     1514 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/resources/resource.py
--rw-r--r--   0        0        0     1842 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/resources/tags.py
--rw-r--r--   0        0        0     5819 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/resources/utils.py
--rw-r--r--   0        0        0        0 2023-10-26 13:51:13.118179 alteia-2.9.0/alteia/core/utils/__init__.py
--rw-r--r--   0        0        0     1232 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/utils/filehelper.py
--rw-r--r--   0        0        0     1200 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/utils/geo_utils.py
--rw-r--r--   0        0        0     3178 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/utils/requests.py
--rw-r--r--   0        0        0     1769 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/utils/srs.py
--rw-r--r--   0        0        0      344 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/utils/typing.py
--rw-r--r--   0        0        0     6114 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/utils/utils.py
--rw-r--r--   0        0        0      696 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/utils/versions.py
--rw-r--r--   0        0        0        0 2023-10-26 13:51:13.118179 alteia-2.9.0/alteia/core/utils/vertcrs/__init__.py
--rw-r--r--   0        0        0      119 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/utils/vertcrs/arbitrary.wkt
--rw-r--r--   0        0        0      130 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/utils/vertcrs/arbitrary_feet.wkt
--rw-r--r--   0        0        0      149 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/utils/vertcrs/arbitrary_feet_us.wkt
--rw-r--r--   0        0        0      211 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/utils/vertcrs/egm2008.wkt
--rw-r--r--   0        0        0      213 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/utils/vertcrs/egm2008_feet.wkt
--rw-r--r--   0        0        0      232 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/utils/vertcrs/egm2008_feet_us.wkt
--rw-r--r--   0        0        0      207 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/utils/vertcrs/egm96.wkt
--rw-r--r--   0        0        0      209 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/utils/vertcrs/egm96_feet.wkt
--rw-r--r--   0        0        0      228 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/utils/vertcrs/egm96_feet_us.wkt
--rw-r--r--   0        0        0      140 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/utils/vertcrs/wgs84.wkt
--rw-r--r--   0        0        0      136 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/utils/vertcrs/wgs84_feet.wkt
--rw-r--r--   0        0        0      155 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/utils/vertcrs/wgs84_feet_us.wkt
--rw-r--r--   0        0        0     1614 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/core/utils/warnings.py
--rw-r--r--   0        0        0        0 2023-10-26 13:51:13.118179 alteia-2.9.0/alteia/py.typed
--rw-r--r--   0        0        0    11832 2023-10-26 13:51:12.994179 alteia-2.9.0/alteia/sdk.py
--rw-r--r--   0        0        0     2810 2023-10-26 13:51:12.994179 alteia-2.9.0/pyproject.toml
--rw-r--r--   0        0        0     3353 2023-10-26 13:51:14.120536 alteia-2.9.0/setup.py
--rw-r--r--   0        0        0     3113 2023-10-26 13:51:14.120853 alteia-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-11-17 11:22:37.331566 alteia-2.9.1/LICENSE
+-rw-r--r--   0        0        0     1426 2023-11-17 11:22:37.331566 alteia-2.9.1/README.md
+-rw-r--r--   0        0        0      257 2023-11-17 11:22:37.331566 alteia-2.9.1/alteia/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-17 11:22:37.447566 alteia-2.9.1/alteia/apis/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-17 11:22:37.447566 alteia-2.9.1/alteia/apis/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-17 11:22:37.447566 alteia-2.9.1/alteia/apis/client/analytics/__init__.py
+-rw-r--r--   0        0        0    26328 2023-11-17 11:22:37.331566 alteia-2.9.1/alteia/apis/client/analytics/analyticsimpl.py
+-rwxr-xr-x   0        0        0    16721 2023-11-17 11:22:37.331566 alteia-2.9.1/alteia/apis/client/analytics/configurationsimpl.py
+-rw-r--r--   0        0        0     7927 2023-11-17 11:22:37.331566 alteia-2.9.1/alteia/apis/client/analytics/productsimpl.py
+-rw-r--r--   0        0        0        0 2023-11-17 11:22:37.447566 alteia-2.9.1/alteia/apis/client/annotations/__init__.py
+-rw-r--r--   0        0        0    30043 2023-11-17 11:22:37.331566 alteia-2.9.1/alteia/apis/client/annotations/annotationsimpl.py
+-rw-r--r--   0        0        0        0 2023-11-17 11:22:37.447566 alteia-2.9.1/alteia/apis/client/auth/__init__.py
+-rw-r--r--   0        0        0     4227 2023-11-17 11:22:37.331566 alteia-2.9.1/alteia/apis/client/auth/companiesimpl.py
+-rw-r--r--   0        0        0     4316 2023-11-17 11:22:37.331566 alteia-2.9.1/alteia/apis/client/auth/oauthclientsimpl.py
+-rw-r--r--   0        0        0     5681 2023-11-17 11:22:37.331566 alteia-2.9.1/alteia/apis/client/auth/sharetokensimpl.py
+-rw-r--r--   0        0        0     3619 2023-11-17 11:22:37.331566 alteia-2.9.1/alteia/apis/client/auth/usersimpl.py
+-rw-r--r--   0        0        0        0 2023-11-17 11:22:37.507566 alteia-2.9.1/alteia/apis/client/comments/__init__.py
+-rw-r--r--   0        0        0     7097 2023-11-17 11:22:37.331566 alteia-2.9.1/alteia/apis/client/comments/commentsimpl.py
+-rw-r--r--   0        0        0        0 2023-11-17 11:22:37.507566 alteia-2.9.1/alteia/apis/client/credentials/__init__.py
+-rw-r--r--   0        0        0     7742 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/apis/client/credentials/credentialsimpl.py
+-rw-r--r--   0        0        0        0 2023-11-17 11:22:37.507566 alteia-2.9.1/alteia/apis/client/datacapture/__init__.py
+-rw-r--r--   0        0        0     4263 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/apis/client/datacapture/carriersimpl.py
+-rw-r--r--   0        0        0     5288 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/apis/client/datacapture/carriersmodelsimpl.py
+-rw-r--r--   0        0        0    11560 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/apis/client/datacapture/collectiontasksimpl.py
+-rw-r--r--   0        0        0     1445 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/apis/client/datacapture/pilotsimpl.py
+-rw-r--r--   0        0        0     4924 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/apis/client/datacapture/teamsimpl.py
+-rw-r--r--   0        0        0       94 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/apis/client/datamngt/__init__.py
+-rw-r--r--   0        0        0    49466 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/apis/client/datamngt/datasetsimpl.py
+-rw-r--r--   0        0        0        0 2023-11-17 11:22:37.507566 alteia-2.9.1/alteia/apis/client/datastream/__init__.py
+-rw-r--r--   0        0        0     3757 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/apis/client/datastream/datastreamassetmonitoredimpl.py
+-rw-r--r--   0        0        0     3705 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/apis/client/datastream/datastreamsfilesimpl.py
+-rw-r--r--   0        0        0     6023 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/apis/client/datastream/datastreamsimpl.py
+-rw-r--r--   0        0        0     8351 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/apis/client/datastreamtemplate/datastreamtemplateimpl.py
+-rw-r--r--   0        0        0        0 2023-11-17 11:22:37.507566 alteia-2.9.1/alteia/apis/client/featuresservice/__init__.py
+-rw-r--r--   0        0        0     6443 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/apis/client/featuresservice/collectionsimpl.py
+-rw-r--r--   0        0        0    12604 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/apis/client/featuresservice/featuresimpl.py
+-rw-r--r--   0        0        0        0 2023-11-17 11:22:37.507566 alteia-2.9.1/alteia/apis/client/projectmngt/__init__.py
+-rw-r--r--   0        0        0    14906 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/apis/client/projectmngt/flightsimpl.py
+-rw-r--r--   0        0        0    20382 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/apis/client/projectmngt/missionsimpl.py
+-rw-r--r--   0        0        0    18356 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/apis/client/projectmngt/projectsimpl.py
+-rw-r--r--   0        0        0        0 2023-11-17 11:22:37.507566 alteia-2.9.1/alteia/apis/client/tags/__init__.py
+-rw-r--r--   0        0        0     5779 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/apis/client/tags/tagsimpl.py
+-rw-r--r--   0        0        0     6637 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/apis/provider.py
+-rw-r--r--   0        0        0        0 2023-11-17 11:22:37.507566 alteia-2.9.1/alteia/core/__init__.py
+-rw-r--r--   0        0        0     3023 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/core/config.py
+-rw-r--r--   0        0        0        0 2023-11-17 11:22:37.507566 alteia-2.9.1/alteia/core/connection/__init__.py
+-rw-r--r--   0        0        0     2853 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/core/connection/abstract_connection.py
+-rw-r--r--   0        0        0     4115 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/core/connection/async_connection.py
+-rw-r--r--   0        0        0     6077 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/core/connection/connection.py
+-rw-r--r--   0        0        0     1441 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/core/connection/credentials.py
+-rw-r--r--   0        0        0     3202 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/core/connection/token.py
+-rw-r--r--   0        0        0     1527 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/core/errors.py
+-rw-r--r--   0        0        0        0 2023-11-17 11:22:37.507566 alteia-2.9.1/alteia/core/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-17 11:22:37.507566 alteia-2.9.1/alteia/core/resources/analytics/__init__.py
+-rw-r--r--   0        0        0      364 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/core/resources/analytics/products.py
+-rw-r--r--   0        0        0     1734 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/core/resources/comments.py
+-rw-r--r--   0        0        0        0 2023-11-17 11:22:37.507566 alteia-2.9.1/alteia/core/resources/datamngt/__init__.py
+-rw-r--r--   0        0        0    11346 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/core/resources/datamngt/upload.py
+-rw-r--r--   0        0        0        0 2023-11-17 11:22:37.507566 alteia-2.9.1/alteia/core/resources/projectmngt/__init__.py
+-rw-r--r--   0        0        0      636 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/core/resources/projectmngt/flights.py
+-rw-r--r--   0        0        0      914 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/core/resources/projectmngt/missions.py
+-rw-r--r--   0        0        0     1105 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/core/resources/projectmngt/projects.py
+-rw-r--r--   0        0        0     1514 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/core/resources/resource.py
+-rw-r--r--   0        0        0     1842 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/core/resources/tags.py
+-rw-r--r--   0        0        0     5819 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/core/resources/utils.py
+-rw-r--r--   0        0        0        0 2023-11-17 11:22:37.507566 alteia-2.9.1/alteia/core/utils/__init__.py
+-rw-r--r--   0        0        0     1232 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/core/utils/filehelper.py
+-rw-r--r--   0        0        0     1200 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/core/utils/geo_utils.py
+-rw-r--r--   0        0        0     3178 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/core/utils/requests.py
+-rw-r--r--   0        0        0     1761 2023-11-17 11:22:37.335566 alteia-2.9.1/alteia/core/utils/srs.py
+-rw-r--r--   0        0        0      344 2023-11-17 11:22:37.339566 alteia-2.9.1/alteia/core/utils/typing.py
+-rw-r--r--   0        0        0     6114 2023-11-17 11:22:37.339566 alteia-2.9.1/alteia/core/utils/utils.py
+-rw-r--r--   0        0        0      696 2023-11-17 11:22:37.339566 alteia-2.9.1/alteia/core/utils/versions.py
+-rw-r--r--   0        0        0        0 2023-11-17 11:22:37.507566 alteia-2.9.1/alteia/core/utils/vertcrs/__init__.py
+-rw-r--r--   0        0        0      119 2023-11-17 11:22:37.339566 alteia-2.9.1/alteia/core/utils/vertcrs/arbitrary.wkt
+-rw-r--r--   0        0        0      130 2023-11-17 11:22:37.339566 alteia-2.9.1/alteia/core/utils/vertcrs/arbitrary_feet.wkt
+-rw-r--r--   0        0        0      149 2023-11-17 11:22:37.339566 alteia-2.9.1/alteia/core/utils/vertcrs/arbitrary_feet_us.wkt
+-rw-r--r--   0        0        0      211 2023-11-17 11:22:37.339566 alteia-2.9.1/alteia/core/utils/vertcrs/egm2008.wkt
+-rw-r--r--   0        0        0      213 2023-11-17 11:22:37.339566 alteia-2.9.1/alteia/core/utils/vertcrs/egm2008_feet.wkt
+-rw-r--r--   0        0        0      232 2023-11-17 11:22:37.339566 alteia-2.9.1/alteia/core/utils/vertcrs/egm2008_feet_us.wkt
+-rw-r--r--   0        0        0      207 2023-11-17 11:22:37.339566 alteia-2.9.1/alteia/core/utils/vertcrs/egm96.wkt
+-rw-r--r--   0        0        0      209 2023-11-17 11:22:37.339566 alteia-2.9.1/alteia/core/utils/vertcrs/egm96_feet.wkt
+-rw-r--r--   0        0        0      228 2023-11-17 11:22:37.339566 alteia-2.9.1/alteia/core/utils/vertcrs/egm96_feet_us.wkt
+-rw-r--r--   0        0        0      140 2023-11-17 11:22:37.339566 alteia-2.9.1/alteia/core/utils/vertcrs/wgs84.wkt
+-rw-r--r--   0        0        0      136 2023-11-17 11:22:37.339566 alteia-2.9.1/alteia/core/utils/vertcrs/wgs84_feet.wkt
+-rw-r--r--   0        0        0      155 2023-11-17 11:22:37.339566 alteia-2.9.1/alteia/core/utils/vertcrs/wgs84_feet_us.wkt
+-rw-r--r--   0        0        0     1614 2023-11-17 11:22:37.339566 alteia-2.9.1/alteia/core/utils/warnings.py
+-rw-r--r--   0        0        0        0 2023-11-17 11:22:37.507566 alteia-2.9.1/alteia/py.typed
+-rw-r--r--   0        0        0    11832 2023-11-17 11:22:37.339566 alteia-2.9.1/alteia/sdk.py
+-rw-r--r--   0        0        0     2810 2023-11-17 11:22:37.339566 alteia-2.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3353 2023-11-17 11:22:38.520173 alteia-2.9.1/setup.py
+-rw-r--r--   0        0        0     3113 2023-11-17 11:22:38.520540 alteia-2.9.1/PKG-INFO
```

### Comparing `alteia-2.9.0/LICENSE` & `alteia-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/README.md` & `alteia-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/analytics/analyticsimpl.py` & `alteia-2.9.1/alteia/apis/client/analytics/analyticsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/analytics/configurationsimpl.py` & `alteia-2.9.1/alteia/apis/client/analytics/configurationsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/analytics/productsimpl.py` & `alteia-2.9.1/alteia/apis/client/analytics/productsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/annotations/annotationsimpl.py` & `alteia-2.9.1/alteia/apis/client/annotations/annotationsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/auth/companiesimpl.py` & `alteia-2.9.1/alteia/apis/client/auth/companiesimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/auth/oauthclientsimpl.py` & `alteia-2.9.1/alteia/apis/client/auth/oauthclientsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/auth/sharetokensimpl.py` & `alteia-2.9.1/alteia/apis/client/auth/sharetokensimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/auth/usersimpl.py` & `alteia-2.9.1/alteia/apis/client/auth/usersimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/comments/commentsimpl.py` & `alteia-2.9.1/alteia/apis/client/comments/commentsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/credentials/credentialsimpl.py` & `alteia-2.9.1/alteia/apis/client/credentials/credentialsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/datacapture/carriersimpl.py` & `alteia-2.9.1/alteia/apis/client/datacapture/carriersimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/datacapture/carriersmodelsimpl.py` & `alteia-2.9.1/alteia/apis/client/datacapture/carriersmodelsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/datacapture/collectiontasksimpl.py` & `alteia-2.9.1/alteia/apis/client/datacapture/collectiontasksimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/datacapture/pilotsimpl.py` & `alteia-2.9.1/alteia/apis/client/datacapture/pilotsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/datacapture/teamsimpl.py` & `alteia-2.9.1/alteia/apis/client/datacapture/teamsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/datamngt/datasetsimpl.py` & `alteia-2.9.1/alteia/apis/client/datamngt/datasetsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/datastream/datastreamassetmonitoredimpl.py` & `alteia-2.9.1/alteia/apis/client/datastream/datastreamassetmonitoredimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/datastream/datastreamsfilesimpl.py` & `alteia-2.9.1/alteia/apis/client/datastream/datastreamsfilesimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/datastream/datastreamsimpl.py` & `alteia-2.9.1/alteia/apis/client/datastream/datastreamsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/datastreamtemplate/datastreamtemplateimpl.py` & `alteia-2.9.1/alteia/apis/client/datastreamtemplate/datastreamtemplateimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/featuresservice/collectionsimpl.py` & `alteia-2.9.1/alteia/apis/client/featuresservice/collectionsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/featuresservice/featuresimpl.py` & `alteia-2.9.1/alteia/apis/client/featuresservice/featuresimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/projectmngt/flightsimpl.py` & `alteia-2.9.1/alteia/apis/client/projectmngt/flightsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/projectmngt/missionsimpl.py` & `alteia-2.9.1/alteia/apis/client/projectmngt/missionsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/projectmngt/projectsimpl.py` & `alteia-2.9.1/alteia/apis/client/projectmngt/projectsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/client/tags/tagsimpl.py` & `alteia-2.9.1/alteia/apis/client/tags/tagsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/apis/provider.py` & `alteia-2.9.1/alteia/apis/provider.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/core/config.py` & `alteia-2.9.1/alteia/core/config.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/core/connection/abstract_connection.py` & `alteia-2.9.1/alteia/core/connection/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/core/connection/async_connection.py` & `alteia-2.9.1/alteia/core/connection/async_connection.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/core/connection/connection.py` & `alteia-2.9.1/alteia/core/connection/connection.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/core/connection/credentials.py` & `alteia-2.9.1/alteia/core/connection/credentials.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/core/connection/token.py` & `alteia-2.9.1/alteia/core/connection/token.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/core/errors.py` & `alteia-2.9.1/alteia/core/errors.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/core/resources/comments.py` & `alteia-2.9.1/alteia/core/resources/comments.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/core/resources/datamngt/upload.py` & `alteia-2.9.1/alteia/core/resources/datamngt/upload.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/core/resources/projectmngt/flights.py` & `alteia-2.9.1/alteia/core/resources/projectmngt/flights.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/core/resources/projectmngt/missions.py` & `alteia-2.9.1/alteia/core/resources/projectmngt/missions.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/core/resources/projectmngt/projects.py` & `alteia-2.9.1/alteia/core/resources/projectmngt/projects.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/core/resources/resource.py` & `alteia-2.9.1/alteia/core/resources/resource.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/core/resources/tags.py` & `alteia-2.9.1/alteia/core/resources/tags.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/core/resources/utils.py` & `alteia-2.9.1/alteia/core/resources/utils.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/core/utils/filehelper.py` & `alteia-2.9.1/alteia/core/utils/filehelper.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/core/utils/geo_utils.py` & `alteia-2.9.1/alteia/core/utils/geo_utils.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/core/utils/requests.py` & `alteia-2.9.1/alteia/core/utils/requests.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/core/utils/srs.py` & `alteia-2.9.1/alteia/core/utils/srs.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """
     name = name.lower()
     res_name = f'{name}.wkt'
     try:
         wkt = read_text_from_resource(vertcrs.__name__, res_name)
         flatten_wkt = ''.join([line.strip() for line in wkt.splitlines()])
         return flatten_wkt
-    except FileNotFoundError:
+    except Exception:
         raise ValueError(f'Unknown SRS name: {name}')
 
 
 def expand_vertcrs_to_wkt(desc: str) -> str:
     """Expand a vertical SRS description to WKT format.
 
     The supported SRS names are ``"arbitrary"``, ``"arbitrary_feet"``,
```

### Comparing `alteia-2.9.0/alteia/core/utils/utils.py` & `alteia-2.9.1/alteia/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/core/utils/versions.py` & `alteia-2.9.1/alteia/core/utils/versions.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/core/utils/warnings.py` & `alteia-2.9.1/alteia/core/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/alteia/sdk.py` & `alteia-2.9.1/alteia/sdk.py`

 * *Files identical despite different names*

### Comparing `alteia-2.9.0/pyproject.toml` & `alteia-2.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alteia"
-version = "2.9.0"  # must match the version in alteia/__init__.py
+version = "2.9.1"  # must match the version in alteia/__init__.py
 description = "High-level Python interface to Alteia API"
 authors = ["Alteia Backend team <backend-team@alteia.com>"]
 repository = "https://github.com/alteia-ai/alteia-python-sdk"
 documentation = "https://alteia.readthedocs.io/en/latest/index.html"
 license = "MIT"
 readme = "README.md"
 keywords = ["sdk",
```

### Comparing `alteia-2.9.0/setup.py` & `alteia-2.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
  'documentation:python_version >= "3.8"': ['sphinx>=4.1.2,<5.0.0',
                                            'sphinx_autodoc_typehints>=1.12.0,<2.0.0',
                                            'sphinx-autobuild>=2021.3.14,<2022.0.0',
                                            'recommonmark>=0.7.1,<0.8.0']}
 
 setup_kwargs = {
     'name': 'alteia',
-    'version': '2.9.0',
+    'version': '2.9.1',
     'description': 'High-level Python interface to Alteia API',
     'long_description': '<p align="center">\n<img src="https://raw.githubusercontent.com/alteia-ai/alteia-python-sdk/master/docs/images/SDK_Python.png" alt="logo" style="max-width:100%;">\n\n<p align="center">\n<a href="https://pypi.org/project/alteia/" rel="nofollow"><img src="https://img.shields.io/pypi/v/alteia.svg" alt="pypi version" style="max-width:100%;"></a>\n<a href="https://pypi.org/project/alteia/" rel="nofollow"><img src="https://img.shields.io/pypi/pyversions/alteia.svg" alt="compatible python versions" style="max-width:100%;"></a>\n</p>\n\n> This SDK offers a high-level Python interface to [Alteia APIs](https://www.alteia.com).\n\n## Installation\n\n```bash\npip install alteia\n```\n\n**requires Python >= 3.6.1, pip >= 20.3*\n\n## Basic usage\n\n```python\nimport alteia\n\nsdk = alteia.SDK(user="YOUR_EMAIL_ADDRESS", password="YOUR_ALTEIA_PASSWORD")\n\nprojects = sdk.projects.search()\n\nfor project in projects:\n    print(project.name)\n\n# My awesome project\n```\n\n<p>&nbsp;</p>\n\n## 📕 Documentation\n\n- [Reference documentation](https://alteia.readthedocs.io/en/latest/index.html)\n- [Jupyter notebook tutorials](https://github.com/alteia-ai/tutorials)\n\n## Contributing\n\nPackage installation:\n\n```bash\npoetry install\n```\n\n(Optional) To install pre-commit hooks (and detect problems before the pipelines):\n\n```bash\npip install pre-commit\npre-commit install\npre-commit run --all-files\npre-commit autoupdate  # Optional, to update pre-commit versions\n```\n',
     'author': 'Alteia Backend team',
     'author_email': 'backend-team@alteia.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/alteia-ai/alteia-python-sdk',
```

#### html2text {}

```diff
@@ -11,15 +11,15 @@
 'alteia.core.utils', 'alteia.core.utils.vertcrs'] package_data = \ {'': ['*']}
 install_requires = \ ['appdirs>=1.4.3,<2.0.0', 'pathvalidate>=2.3.0,<3.0.0',
 'semantic-version>=2.8.5,<3.0.0', 'urllib3==1.26.16'] extras_require = \ {':
 python_version < "3.7"': ['importlib-resources>=1.4'], 'documentation:
 python_version >= "3.8"': ['sphinx>=4.1.2,<5.0.0',
 'sphinx_autodoc_typehints>=1.12.0,<2.0.0', 'sphinx-
 autobuild>=2021.3.14,<2022.0.0', 'recommonmark>=0.7.1,<0.8.0']} setup_kwargs =
-{ 'name': 'alteia', 'version': '2.9.0', 'description': 'High-level Python
+{ 'name': 'alteia', 'version': '2.9.1', 'description': 'High-level Python
 interface to Alteia API', 'long_description': '
                                  \n[logo]\n\n
                \n_[_p_y_p_i_ _v_e_r_s_i_o_n_]\n_[_c_o_m_p_a_t_i_b_l_e_ _p_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]\n
 \n\n> This SDK offers a high-level Python interface to [Alteia APIs](https://
 www.alteia.com).\n\n## Installation\n\n```bash\npip install
 alteia\n```\n\n**requires Python >= 3.6.1, pip >= 20.3*\n\n## Basic
 usage\n\n```python\nimport alteia\n\nsdk = alteia.SDK
```

### Comparing `alteia-2.9.0/PKG-INFO` & `alteia-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alteia
-Version: 2.9.0
+Version: 2.9.1
 Summary: High-level Python interface to Alteia API
 Home-page: https://github.com/alteia-ai/alteia-python-sdk
 License: MIT
 Keywords: sdk,alteia
 Author: Alteia Backend team
 Author-email: backend-team@alteia.com
 Requires-Python: >=3.6.1,<4.0.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alteia Version: 2.9.0 Summary: High-level Python
+Metadata-Version: 2.1 Name: alteia Version: 2.9.1 Summary: High-level Python
 interface to Alteia API Home-page: https://github.com/alteia-ai/alteia-python-
 sdk License: MIT Keywords: sdk,alteia Author: Alteia Backend team Author-email:
 backend-team@alteia.com Requires-Python: >=3.6.1,<4.0.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
```

