# Comparing `tmp/sarmat-1.4.1.tar.gz` & `tmp/sarmat-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarmat-1.4.1.tar", last modified: Fri Sep 29 17:41:53 2023, max compression
+gzip compressed data, was "sarmat-1.5.0.tar", max compression
```

## Comparing `sarmat-1.4.1.tar` & `sarmat-1.5.0.tar`

### file list

```diff
@@ -1,79 +1,17 @@
-drwxrwxr-x   0 jn        (1000) jn        (1000)        0 2023-09-29 17:41:53.581240 sarmat-1.4.1/
--rw-rw-r--   0 jn        (1000) jn        (1000)     1074 2022-09-11 22:24:09.000000 sarmat-1.4.1/LICENSE
--rw-rw-r--   0 jn        (1000) jn        (1000)     9633 2023-09-29 17:41:53.581240 sarmat-1.4.1/PKG-INFO
--rw-rw-r--   0 jn        (1000) jn        (1000)     8032 2022-09-11 22:24:09.000000 sarmat-1.4.1/README.md
--rw-rw-r--   0 jn        (1000) jn        (1000)      529 2023-09-29 17:34:04.000000 sarmat-1.4.1/pyproject.toml
-drwxrwxr-x   0 jn        (1000) jn        (1000)        0 2023-09-29 17:41:53.517239 sarmat-1.4.1/sarmat/
--rw-rw-r--   0 jn        (1000) jn        (1000)       41 2023-09-29 17:34:04.000000 sarmat-1.4.1/sarmat/__init__.py
-drwxrwxr-x   0 jn        (1000) jn        (1000)        0 2023-09-29 17:41:53.517239 sarmat-1.4.1/sarmat/core/
--rw-rw-r--   0 jn        (1000) jn        (1000)       40 2022-09-11 22:24:09.000000 sarmat-1.4.1/sarmat/core/__init__.py
-drwxrwxr-x   0 jn        (1000) jn        (1000)        0 2023-09-29 17:41:53.537239 sarmat-1.4.1/sarmat/core/actions/
--rw-rw-r--   0 jn        (1000) jn        (1000)      412 2022-09-11 22:24:09.000000 sarmat-1.4.1/sarmat/core/actions/__init__.py
--rw-rw-r--   0 jn        (1000) jn        (1000)      360 2022-09-11 22:24:09.000000 sarmat-1.4.1/sarmat/core/actions/bases.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     9318 2023-08-08 18:39:24.000000 sarmat-1.4.1/sarmat/core/actions/dispatcher.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     1371 2023-08-11 21:19:43.000000 sarmat-1.4.1/sarmat/core/actions/geo_locations.py
--rw-rw-r--   0 jn        (1000) jn        (1000)    12121 2023-09-29 17:34:05.000000 sarmat-1.4.1/sarmat/core/actions/traffic_management.py
-drwxrwxr-x   0 jn        (1000) jn        (1000)        0 2023-09-29 17:41:53.545239 sarmat-1.4.1/sarmat/core/behavior/
--rw-rw-r--   0 jn        (1000) jn        (1000)      726 2022-09-11 22:24:09.000000 sarmat-1.4.1/sarmat/core/behavior/__init__.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     3511 2022-09-12 01:24:12.000000 sarmat-1.4.1/sarmat/core/behavior/bases.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     8778 2022-09-12 01:24:12.000000 sarmat-1.4.1/sarmat/core/behavior/geo_locations.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     2546 2022-09-12 01:24:12.000000 sarmat-1.4.1/sarmat/core/behavior/sarmat.py
--rw-rw-r--   0 jn        (1000) jn        (1000)    25382 2023-07-08 11:11:29.000000 sarmat-1.4.1/sarmat/core/behavior/traffic_management.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     6638 2022-09-12 01:24:12.000000 sarmat-1.4.1/sarmat/core/behavior/vehicle.py
-drwxrwxr-x   0 jn        (1000) jn        (1000)        0 2023-09-29 17:41:53.545239 sarmat-1.4.1/sarmat/core/constants/
--rw-rw-r--   0 jn        (1000) jn        (1000)      917 2023-07-08 11:11:29.000000 sarmat-1.4.1/sarmat/core/constants/__init__.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     1736 2022-09-11 22:24:09.000000 sarmat-1.4.1/sarmat/core/constants/exception_constants.py
--rw-rw-r--   0 jn        (1000) jn        (1000)      281 2022-09-11 22:24:09.000000 sarmat-1.4.1/sarmat/core/constants/formats.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     8330 2023-07-08 11:11:29.000000 sarmat-1.4.1/sarmat/core/constants/sarmat_constants.py
-drwxrwxr-x   0 jn        (1000) jn        (1000)        0 2023-09-29 17:41:53.545239 sarmat-1.4.1/sarmat/core/context/
--rw-rw-r--   0 jn        (1000) jn        (1000)        0 2022-09-11 22:24:09.000000 sarmat-1.4.1/sarmat/core/context/__init__.py
-drwxrwxr-x   0 jn        (1000) jn        (1000)        0 2023-09-29 17:41:53.549239 sarmat-1.4.1/sarmat/core/context/containers/
--rw-rw-r--   0 jn        (1000) jn        (1000)     1256 2022-09-11 22:24:09.000000 sarmat-1.4.1/sarmat/core/context/containers/__init__.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     5196 2023-08-10 18:06:58.000000 sarmat-1.4.1/sarmat/core/context/containers/dispatcher_containers.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     1692 2023-08-11 21:19:43.000000 sarmat-1.4.1/sarmat/core/context/containers/geo_containers.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     2393 2023-08-10 18:06:58.000000 sarmat-1.4.1/sarmat/core/context/containers/sarmat_containers.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     5863 2023-09-29 17:24:33.000000 sarmat-1.4.1/sarmat/core/context/containers/traffic_management_containers.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     2254 2023-08-10 18:06:58.000000 sarmat-1.4.1/sarmat/core/context/containers/vehicle_containers.py
-drwxrwxr-x   0 jn        (1000) jn        (1000)        0 2023-09-29 17:41:53.553239 sarmat-1.4.1/sarmat/core/context/models/
--rw-rw-r--   0 jn        (1000) jn        (1000)     1017 2022-09-11 22:24:09.000000 sarmat-1.4.1/sarmat/core/context/models/__init__.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     6408 2023-08-10 18:06:58.000000 sarmat-1.4.1/sarmat/core/context/models/dispatcher_models.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     5177 2023-08-11 21:19:43.000000 sarmat-1.4.1/sarmat/core/context/models/geo_models.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     4224 2023-08-10 18:06:58.000000 sarmat-1.4.1/sarmat/core/context/models/sarmat_models.py
--rw-rw-r--   0 jn        (1000) jn        (1000)    14949 2023-09-29 17:24:33.000000 sarmat-1.4.1/sarmat/core/context/models/traffic_management_models.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     4865 2023-08-10 18:06:58.000000 sarmat-1.4.1/sarmat/core/context/models/vehicle_models.py
-drwxrwxr-x   0 jn        (1000) jn        (1000)        0 2023-09-29 17:41:53.553239 sarmat-1.4.1/sarmat/core/exceptions/
--rw-rw-r--   0 jn        (1000) jn        (1000)      469 2022-09-11 22:24:09.000000 sarmat-1.4.1/sarmat/core/exceptions/__init__.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     1657 2022-09-11 22:24:09.000000 sarmat-1.4.1/sarmat/core/exceptions/exceptions.py
--rw-rw-r--   0 jn        (1000) jn        (1000)      712 2022-09-11 22:24:09.000000 sarmat-1.4.1/sarmat/core/exceptions/sarmat_exceptions.py
-drwxrwxr-x   0 jn        (1000) jn        (1000)        0 2023-09-29 17:41:53.569239 sarmat-1.4.1/sarmat/core/factory/
--rw-rw-r--   0 jn        (1000) jn        (1000)      646 2022-09-11 22:24:09.000000 sarmat-1.4.1/sarmat/core/factory/__init__.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     5820 2022-09-11 22:24:09.000000 sarmat-1.4.1/sarmat/core/factory/base_creator.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     1995 2022-09-11 22:24:09.000000 sarmat-1.4.1/sarmat/core/factory/geo_creator.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     8055 2022-09-11 22:24:09.000000 sarmat-1.4.1/sarmat/core/factory/traffic_manager_creator.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     2813 2022-09-11 22:24:09.000000 sarmat-1.4.1/sarmat/core/factory/vehicle_creator.py
-drwxrwxr-x   0 jn        (1000) jn        (1000)        0 2023-09-29 17:41:53.581240 sarmat-1.4.1/sarmat/core/verification/
--rw-rw-r--   0 jn        (1000) jn        (1000)     1005 2022-09-11 22:24:09.000000 sarmat-1.4.1/sarmat/core/verification/__init__.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     1482 2023-08-10 18:06:58.000000 sarmat-1.4.1/sarmat/core/verification/base_verifications.py
--rw-rw-r--   0 jn        (1000) jn        (1000)      509 2022-09-11 22:24:09.000000 sarmat-1.4.1/sarmat/core/verification/customize_verifications.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     2534 2022-09-11 22:24:09.000000 sarmat-1.4.1/sarmat/core/verification/geo_verifications.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     3113 2023-09-29 17:24:33.000000 sarmat-1.4.1/sarmat/core/verification/traffic_management_verifications.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     1657 2022-09-11 22:24:09.000000 sarmat-1.4.1/sarmat/core/verification/vehicle_verifications.py
-drwxrwxr-x   0 jn        (1000) jn        (1000)        0 2023-09-29 17:41:53.581240 sarmat-1.4.1/sarmat/tools/
--rw-rw-r--   0 jn        (1000) jn        (1000)       72 2022-09-11 22:24:09.000000 sarmat-1.4.1/sarmat/tools/__init__.py
--rw-rw-r--   0 jn        (1000) jn        (1000)    14608 2023-08-11 21:19:43.000000 sarmat-1.4.1/sarmat/tools/fare_calculation.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     2181 2023-08-11 21:19:43.000000 sarmat-1.4.1/sarmat/tools/fare_containers.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     1913 2023-09-29 17:24:33.000000 sarmat-1.4.1/sarmat/tools/geo_tools.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     1888 2023-08-10 18:06:58.000000 sarmat-1.4.1/sarmat/tools/json_encoder.py
-drwxrwxr-x   0 jn        (1000) jn        (1000)        0 2023-09-29 17:41:53.517239 sarmat-1.4.1/sarmat.egg-info/
--rw-rw-r--   0 jn        (1000) jn        (1000)     9633 2023-09-29 17:41:53.000000 sarmat-1.4.1/sarmat.egg-info/PKG-INFO
--rw-rw-r--   0 jn        (1000) jn        (1000)     2245 2023-09-29 17:41:53.000000 sarmat-1.4.1/sarmat.egg-info/SOURCES.txt
--rw-rw-r--   0 jn        (1000) jn        (1000)        1 2023-09-29 17:41:53.000000 sarmat-1.4.1/sarmat.egg-info/dependency_links.txt
--rw-rw-r--   0 jn        (1000) jn        (1000)        9 2023-09-29 17:41:53.000000 sarmat-1.4.1/sarmat.egg-info/requires.txt
--rw-rw-r--   0 jn        (1000) jn        (1000)        7 2023-09-29 17:41:53.000000 sarmat-1.4.1/sarmat.egg-info/top_level.txt
--rw-rw-r--   0 jn        (1000) jn        (1000)      448 2023-09-29 17:41:53.585240 sarmat-1.4.1/setup.cfg
--rw-rw-r--   0 jn        (1000) jn        (1000)      596 2023-09-29 17:34:04.000000 sarmat-1.4.1/setup.py
-drwxrwxr-x   0 jn        (1000) jn        (1000)        0 2023-09-29 17:41:53.581240 sarmat-1.4.1/tests/
--rw-rw-r--   0 jn        (1000) jn        (1000)     9410 2023-08-10 18:06:58.000000 sarmat-1.4.1/tests/test_constants.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     1258 2023-08-10 18:06:58.000000 sarmat-1.4.1/tests/test_fare.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     1934 2023-08-11 21:19:43.000000 sarmat-1.4.1/tests/test_fare_calculation.py
--rw-rw-r--   0 jn        (1000) jn        (1000)     4589 2023-08-11 21:19:43.000000 sarmat-1.4.1/tests/test_fare_strategy.py
+-rw-r--r--   0        0        0     1074 2022-09-11 22:24:09.704167 sarmat-1.5.0/LICENSE
+-rw-r--r--   0        0        0     8032 2022-09-11 22:24:09.704167 sarmat-1.5.0/README.md
+-rw-r--r--   0        0        0      639 2024-04-25 20:51:35.864813 sarmat-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0       57 2024-04-25 20:51:35.864813 sarmat-1.5.0/sarmat/__init__.py
+-rw-r--r--   0        0        0       39 2024-04-25 20:51:35.864813 sarmat-1.5.0/sarmat/core/__init__.py
+-rw-r--r--   0        0        0     1270 2024-04-25 20:51:35.864813 sarmat-1.5.0/sarmat/core/constants/__init__.py
+-rw-r--r--   0        0        0     2306 2024-04-25 20:51:35.864813 sarmat-1.5.0/sarmat/core/constants/exception_constants.py
+-rw-r--r--   0        0        0      281 2022-09-11 22:24:09.708167 sarmat-1.5.0/sarmat/core/constants/formats.py
+-rw-r--r--   0        0        0     5662 2024-04-25 20:51:35.864813 sarmat-1.5.0/sarmat/core/constants/sarmat_constants.py
+-rw-r--r--   0        0        0       83 2024-04-25 20:51:35.864813 sarmat-1.5.0/sarmat/core/context/__init__.py
+-rw-r--r--   0        0        0     1063 2024-04-25 20:51:35.864813 sarmat-1.5.0/sarmat/core/context/models/__init__.py
+-rw-r--r--   0        0        0     3302 2024-04-25 20:51:35.864813 sarmat-1.5.0/sarmat/core/context/models/dispatcher_models.py
+-rw-r--r--   0        0        0     2489 2024-04-25 20:51:35.864813 sarmat-1.5.0/sarmat/core/context/models/geo_models.py
+-rw-r--r--   0        0        0     2269 2024-04-25 20:51:35.864813 sarmat-1.5.0/sarmat/core/context/models/sarmat_models.py
+-rw-r--r--   0        0        0     6676 2024-04-25 20:51:35.864813 sarmat-1.5.0/sarmat/core/context/models/traffic_management_models.py
+-rw-r--r--   0        0        0     2063 2024-04-25 20:51:35.864813 sarmat-1.5.0/sarmat/core/context/models/vehicle_models.py
+-rw-r--r--   0        0        0     8583 1970-01-01 00:00:00.000000 sarmat-1.5.0/PKG-INFO
```

### Comparing `sarmat-1.4.1/LICENSE` & `sarmat-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sarmat-1.4.1/PKG-INFO` & `sarmat-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,22 @@
 Metadata-Version: 2.1
 Name: sarmat
-Version: 1.4.1
-Summary: Sarmat
-Home-page: 
-Author: Artel
-Author-email: Artel <artel61@gmail.com>
-License: Copyright (c) 2018 The Python Packaging Authority
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Classifier: Programming Language :: Python :: 3
+Version: 1.5.0
+Summary: Sarmat package for IT decisions in the passenger transport sphere
+License: MIT
+Author: jn
+Author-email: artel61@gmail.com
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Sarmat.
 
 Библиотека для построения решений в сфере пассажирского транспорта.
 
 Основу работы библиотеки составляют объекты для построения рейсов
 и шаблонов для них, выполнения диспетчерских операций,
@@ -116,7 +98,8 @@
 производится вызовом `type` с последующей инициализацией полученного класса при
 помощи данных, которые передаются в контейнере. В фабрике перечисляются
 родительские классы, а также указываются дополнительные атрибуты для будущего
 объекта: в атрибуте `controller` передается экземпляр фабрики для последующего
 использования при создании объектов во время выполнения бизнесс процессов.
 Также передается набор тегов доступа, которые были определены пользователю
 изначально.
+
```

### Comparing `sarmat-1.4.1/README.md` & `sarmat-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sarmat-1.4.1/sarmat/core/constants/exception_constants.py` & `sarmat-1.5.0/sarmat/core/constants/exception_constants.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,70 @@
 """
 Sarmat.
-
 Ядро пакета.
-
 Описание ошибок.
-
 Типы ошибок, коды, описание.
 """
-from .sarmat_constants import SarmatAttribute
+from collections import namedtuple
+from dataclasses import dataclass
+from enum import Enum
 
 
-class ErrorType(SarmatAttribute):
-    """Тип ошибки"""
+SarmatErrorType = namedtuple("SarmatErrorType", "code title")
+SarmatErrorClass = namedtuple("SarmatErrorClass", "cypher description")
 
-    information = 0
-    question = 1
-    warning = 2
-    error = 3
-    critical = 4
 
-    __description__ = {
-        information: 'Информация',
-        question: 'Вопрос',
-        warning: 'Внимание!',
-        error: 'Ошибка',
-        critical: 'Критическая ошибка',
-    }
+class MessageType(SarmatErrorType, Enum):
+    """Типы сообщений"""
+    INFORMATION = 0, "Информация"
+    QUESTION = 1, "Вопрос"
+    WARNING = 2, "Внимание"
+    ERROR = 3, "Ошибка"
+    CRITICAL = 4, "Критическая ошибка"
 
 
-class ErrorClass(SarmatAttribute):
+class ErrorClass(SarmatErrorClass, Enum):
     """Классификация ошибки"""
 
-    UNKNOWN = ''
-    SYSTEM = 'S'
-    DATA = 'D'
-    OPERATION = 'O'
-
-    __description__ = {
-        UNKNOWN: '',
-        SYSTEM: 'Системная ошибка',
-        DATA: 'Ошибка данных',
-        OPERATION: 'Ошибка выполнения операции',
-    }
-
-
-class ErrorCode(SarmatAttribute):
-    """Код ошибки"""
-
-    UNKNOWN = (-1, ErrorClass.UNKNOWN)
-    NO_ERROR = (0, ErrorClass.UNKNOWN)
-    NO_ATTRIBUTE = (1, ErrorClass.DATA)
-    NOT_FILLED = (2, ErrorClass.DATA)
-    WRONG_TYPE = (3, ErrorClass.DATA)
-    WRONG_VALUE = (4, ErrorClass.DATA)
-    IMPOSSIBLE_OPERATION = (5, ErrorClass.OPERATION)
-
-    __description__ = {
-        UNKNOWN: 'Неизвестная ошибка',
-        NO_ERROR: '',
-        NO_ATTRIBUTE: 'Отсутствует атрибут объекта',
-        NOT_FILLED: 'Атрибут не заполнен',
-        WRONG_TYPE: 'Неподходящий тип атрибута',
-        WRONG_VALUE: 'Неверное значение',
-        IMPOSSIBLE_OPERATION: 'Невозможная операция',
-    }
+    UNKNOWN = "", ""
+    SYSTEM = "S", "Системная ошибка"
+    DATA = "D", "Ошибка данных"
+    OPERATION = "O", "Ошибка выполнения операции"
+
+
+@dataclass
+class SarmatException(Exception):
+    """Класс ошибки в формате Sarmat"""
+    err_class: ErrorClass = ErrorClass.UNKNOWN
+    err_type: MessageType = MessageType.ERROR
+    title: str = ""
+    description: str = ""
+
+
+class SarmatExpectedAttributeError(SarmatException):
+    """Ошибка возникает при отсутствии атрибута в объекта"""
+    err_class = ErrorClass.DATA
+    title = "Отсутствует атрибут"
+
+
+class SarmatNotFilledAttribute(SarmatException):
+    """Ошибка возникает при обнаружении незаполненного атрибута"""
+    err_class = ErrorClass.DATA
+    title = "Не указано значение"
+
+
+class SarmatWrongTypeAttribute(SarmatException):
+    """Атрибут содержит значение неверного типа"""
+    err_class = ErrorClass.DATA
+    title = "Невертный тип данных"
+
+
+class SarmatWrongValueError(SarmatException):
+    """Атрибут содержит неверное значение"""
+    err_class = ErrorClass.DATA
+    title = "Неверное значение данных"
+
+
+class SarmatWrongOperationError(SarmatException):
+    """Невозможно выполнить операцию"""
+    err_class = ErrorClass.OPERATION
+    title = "Невозможная операция"
```

### Comparing `sarmat-1.4.1/sarmat/core/context/containers/traffic_management_containers.py` & `sarmat-1.5.0/sarmat/core/context/models/traffic_management_models.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,130 +1,139 @@
 """
 Sarmat.
-
-Описание сущностей.
-
-Контейнеры для описания объектов маршрутной сети.
+Ядро пакета.
+Описание бизнес логики.
+Модели.
+Модели для построения маршрутной сети.
 """
-import datetime
+from dataclasses import dataclass
+from datetime import time, date
 from typing import List, Optional
 
-from pydantic import field_serializer, field_validator, ConfigDict
+from sarmat.core.constants import JourneyType, RoadType, RouteType, StationType
+
+from .geo_models import DirectionModel, DestinationPointModel, RoadNameModel
+from .sarmat_models import BaseIdModel, BaseModel, CustomAttributesModel
 
-from sarmat.core.constants import (
-    DATE_FORMAT,
-    JourneyType,
-    RoadType,
-    RouteType,
-    StationType,
-)
-
-from .geo_containers import (
-    DestinationPointContainer,
-    DirectionContainer,
-    RoadNameContainer,
-)
-from .sarmat_containers import BaseIdSarmatContainer
 
+@dataclass
+class BaseStationModel(BaseModel):
+    """Станции (пункты посадки-высадки пассажиров) (основные атрибуты)"""
 
-class StationContainer(BaseIdSarmatContainer):
+    station_type: StationType           # тип станции
+    name: str                           # наименование
+    point: DestinationPointModel        # ближайший населенный пункт
+    address: str = ''                   # почтовый адрес
+
+
+@dataclass
+class StationModel(BaseIdModel, CustomAttributesModel, BaseStationModel):
     """Станции (пункты посадки-высадки пассажиров)"""
 
-    station_type: StationType               # тип станции
-    name: str                               # наименование
-    point: DestinationPointContainer        # ближайший населенный пункт
-    address: str = ""                       # почтовый адрес
+
+@dataclass
+class BaseRoadModel(BaseModel):
+    """Дороги (основные атрибуты)"""
+
+    start_point: DestinationPointModel          # начало дороги
+    end_point: DestinationPointModel            # конец дороги
+    direct_travel_time_min: int                 # время прохождения в прямом направлении
+    reverse_travel_time_min: int                # время прохождения в обратном направлении
+    direct_len_km: float                        # расстояние в прямом направлении
+    reverse_len_km: float                       # расстояние в обратном направлении
+    road_type: RoadType                         # тип дорожного покрытия
+    road_name: Optional[RoadNameModel] = None   # классификация дороги
 
 
-class RoadContainer(BaseIdSarmatContainer):
+@dataclass
+class RoadModel(BaseIdModel, CustomAttributesModel, BaseRoadModel):
     """Дороги"""
 
-    start_point: DestinationPointContainer          # начало дороги
-    end_point: DestinationPointContainer            # конец дороги
-    direct_travel_time_min: int                     # время прохождения в прямом направлении
-    reverse_travel_time_min: int                    # время прохождения в обратном направлении
-    direct_len_km: float                            # расстояние в прямом направлении
-    reverse_len_km: float                           # расстояние в обратном направлении
-    road_type: RoadType                             # тип дорожного покрытия
-    road_name: Optional[RoadNameContainer] = None   # классификация дороги
 
+@dataclass
+class BaseRouteItemModel(BaseModel):
+    """Состав маршрута (основные атрибуты)"""
+
+    length_from_last_km: float                      # расстояние от предыдущего пункта
+    travel_time_min: int                            # время движения от предыдущего пункта в минутах
+    road: Optional[RoadModel] = None                # дорога
+    order: int = 1                                  # порядок следования
+    station: Optional[StationModel] = None          # станция
+    point: Optional[DestinationPointModel] = None   # ближайший населенный пункт
+    stop_time_min: Optional[int] = None             # время стоянки в минутах
 
-class RouteItemContainer(BaseIdSarmatContainer):
+
+@dataclass
+class RouteItemModel(BaseIdModel, CustomAttributesModel, BaseRouteItemModel):
     """Состав маршрута"""
 
-    length_from_last_km: float                              # расстояние от предыдущего пункта
-    travel_time_min: int                                    # время движения от предыдущего пункта в минутах
-    road: Optional[RoadContainer] = None                    # дорога
-    order: int = 1                                          # порядок следования
-    station: Optional[StationContainer] = None              # станция
-    point: Optional[DestinationPointContainer] = None       # ближайший населенный пункт
-    stop_time_min: Optional[int] = None                     # время стоянки в минутах
+
+@dataclass
+class BaseRouteModel(BaseModel):
+    """Описание маршрута (основные атрибуты)"""
+
+    route_type: RouteType                               # тип маршрута
+    name: str                                           # наименование
+    first_station: StationModel                         # станция отправления
+    structure: List[RouteItemModel]                     # состав маршрута
+    direction: Optional[List[DirectionModel]] = None    # направления
+    comments: Optional[str] = None                      # комментарий к маршруту
+    number: Optional[int] = None                        # номер маршрута
+    literal: str = ''                                   # литера
+    is_active: bool = True                              # признак активности маршрута
 
 
-class RouteContainer(BaseIdSarmatContainer):
+@dataclass
+class RouteModel(BaseIdModel, CustomAttributesModel, BaseRouteModel):
     """Описание маршрута"""
 
-    route_type: RouteType                                       # тип маршрута
-    name: str                                                   # наименование
-    first_station: StationContainer                             # станция отправления
-    structure: List[RouteItemContainer]                         # состав маршрута
-    direction: Optional[List[DirectionContainer]] = None        # направления
-    comments: Optional[str] = None                              # комментарий к маршруту
-    number: Optional[int] = None                                # номер маршрута
-    literal: str = ""                                           # литера
-    is_active: bool = True                                      # признак активности маршрута
+
+@dataclass
+class BaseJourneyModel(BaseModel):
+    """Атрибуты рейса (основные атрибуты)"""
+
+    route_type: RouteType                               # тип маршрута
+    name: str                                           # наименование
+    first_station: StationModel                         # пункт отправления
+    structure: List[RouteItemModel]                     # состав рейса
+    journey_type: JourneyType                           # тип рейса
+    departure_time: time                                # время отправления
+    number: Optional[int] = None                        # номер рейса
+    literal: Optional[str] = None                       # литера
+    is_chartered: bool = False                          # признак заказного рейса
+    need_control: bool = False                          # признак именной продажи и мониторинга
+    season_begin: Optional[date] = None                 # начало сезона
+    season_end: Optional[date] = None                   # окончание сезона
+    direction: Optional[List[DirectionModel]] = None    # направления
+    comments: Optional[str] = None                      # комментарии по рейсу
+    is_active: bool = True                              # признак активности рейса
 
 
-class JourneyContainer(RouteContainer):
+@dataclass
+class JourneyModel(BaseIdModel, CustomAttributesModel, BaseJourneyModel):
     """Атрибуты рейса"""
 
-    journey_type: JourneyType                       # тип рейса
-    route_type: RouteType                           # тип маршрута
-    departure_time: datetime.time                   # время отправления
-    is_chartered: bool = False                      # признак заказного рейса
-    need_control: bool = False                      # признак именной продажи и мониторинга
-    season_begin: Optional[datetime.date] = None    # начало сезона
-    season_end: Optional[datetime.date] = None      # окончание сезона
-
-    @field_validator('season_begin', mode="before")
-    @classmethod
-    def parse_season_begin(cls, val):
-        if val and isinstance(val, str):
-            return cls._parse_date(val)
-        return val
-
-    @field_validator('season_end', mode="before")
-    @classmethod
-    def parse_season_end(cls, val):
-        if val and isinstance(val, str):
-            return cls._parse_date(val)
-        return val
-
-    @field_serializer('season_begin')
-    def serialize_season_begin(self, season_begin: Optional[datetime.date], _info):
-        if season_begin:
-            return season_begin.strftime(DATE_FORMAT)
-
-        return None
-
-    @field_serializer('season_end')
-    def serialize_season_end(self, season_end: Optional[datetime.date], _info):
-        if season_end:
-            return season_end.strftime(DATE_FORMAT)
 
-        return None
+@dataclass
+class BaseJourneyBunchItemModel(BaseModel):
+    """Атрибуты элемента из связки рейсов (основные атрибуты)"""
 
-    model_config = ConfigDict(arbitrary_types_allowed=True)
+    journey: JourneyModel     # рейс
+    stop_interval: int        # время простоя в часах
 
 
-class JourneyBunchItemContainer(BaseIdSarmatContainer):
+@dataclass
+class JourneyBunchItemModel(BaseIdModel, CustomAttributesModel, BaseJourneyBunchItemModel):
     """Атрибуты элемента из связки рейсов"""
 
-    journey: JourneyContainer       # рейс
-    stop_interval: int              # время простоя в часах
 
+@dataclass
+class BaseJourneyBunchModel(BaseModel):
+    """Атрибуты связки рейсов (основные атрибуты)"""
+
+    journeys: List[JourneyBunchItemModel]     # элементы связки
+    name: Optional[str] = None                # наименование связки
 
-class JourneyBunchContainer(BaseIdSarmatContainer):
-    """Атрибуты связки рейсов"""
 
-    journeys: List[JourneyBunchItemContainer]     # элементы связки
-    name: Optional[str] = None                    # наименование связки
+@dataclass
+class JourneyBunchModel(BaseIdModel, CustomAttributesModel, BaseJourneyBunchModel):
+    """Атрибуты связки рейсов"""
```

