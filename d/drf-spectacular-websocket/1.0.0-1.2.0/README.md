# Comparing `tmp/drf_spectacular_websocket-1.0.0.tar.gz` & `tmp/drf_spectacular_websocket-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_spectacular_websocket-1.0.0.tar", last modified: Sun Apr 21 18:26:35 2024, max compression
+gzip compressed data, was "drf_spectacular_websocket-1.2.0.tar", last modified: Thu Apr 25 18:41:11 2024, max compression
```

## Comparing `drf_spectacular_websocket-1.0.0.tar` & `drf_spectacular_websocket-1.2.0.tar`

### file list

```diff
@@ -1,25 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 18:26:35.822616 drf_spectacular_websocket-1.0.0/
--rw-rw-rw-   0        0        0     1085 2024-04-16 14:24:28.000000 drf_spectacular_websocket-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      158 2024-04-16 20:04:20.000000 drf_spectacular_websocket-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5325 2024-04-21 18:26:35.820616 drf_spectacular_websocket-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4158 2024-04-16 21:02:04.000000 drf_spectacular_websocket-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 18:26:35.798615 drf_spectacular_websocket-1.0.0/drf_spectacular_websocket/
--rw-rw-rw-   0        0        0       25 2024-04-16 19:38:16.000000 drf_spectacular_websocket-1.0.0/drf_spectacular_websocket/__init__.py
--rw-rw-rw-   0        0        0      187 2024-04-16 21:10:28.000000 drf_spectacular_websocket-1.0.0/drf_spectacular_websocket/apps.py
--rw-rw-rw-   0        0        0      906 2024-04-16 17:36:08.000000 drf_spectacular_websocket-1.0.0/drf_spectacular_websocket/decorators.py
-drwxrwxrwx   0        0        0        0 2024-04-21 18:26:35.811615 drf_spectacular_websocket-1.0.0/drf_spectacular_websocket/schemas/
--rw-rw-rw-   0        0        0       39 2024-04-16 17:33:43.000000 drf_spectacular_websocket-1.0.0/drf_spectacular_websocket/schemas/__init__.py
--rw-rw-rw-   0        0        0     6076 2024-04-15 18:49:21.000000 drf_spectacular_websocket-1.0.0/drf_spectacular_websocket/schemas/consumer_schema.py
--rw-rw-rw-   0        0        0     3921 2024-04-16 12:25:22.000000 drf_spectacular_websocket-1.0.0/drf_spectacular_websocket/schemas/schema.py
--rw-rw-rw-   0        0        0      643 2024-04-19 13:33:02.000000 drf_spectacular_websocket-1.0.0/drf_spectacular_websocket/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-21 18:26:35.789614 drf_spectacular_websocket-1.0.0/drf_spectacular_websocket/templates/
-drwxrwxrwx   0        0        0        0 2024-04-21 18:26:35.815618 drf_spectacular_websocket-1.0.0/drf_spectacular_websocket/templates/drf_spectacular/
--rw-rw-rw-   0        0        0    21443 2024-04-15 20:31:01.000000 drf_spectacular_websocket-1.0.0/drf_spectacular_websocket/templates/drf_spectacular/swagger_ui.js
-drwxrwxrwx   0        0        0        0 2024-04-21 18:26:35.817615 drf_spectacular_websocket-1.0.0/drf_spectacular_websocket.egg-info/
--rw-rw-rw-   0        0        0     5325 2024-04-21 18:26:35.000000 drf_spectacular_websocket-1.0.0/drf_spectacular_websocket.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      641 2024-04-21 18:26:35.000000 drf_spectacular_websocket-1.0.0/drf_spectacular_websocket.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 18:26:35.000000 drf_spectacular_websocket-1.0.0/drf_spectacular_websocket.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2024-04-21 18:26:35.000000 drf_spectacular_websocket-1.0.0/drf_spectacular_websocket.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-21 18:26:35.000000 drf_spectacular_websocket-1.0.0/drf_spectacular_websocket.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 18:26:35.822616 drf_spectacular_websocket-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1400 2024-04-17 08:19:21.000000 drf_spectacular_websocket-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:41:11.778108 drf_spectacular_websocket-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 18:41:01.000000 drf_spectacular_websocket-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-25 18:41:11.778108 drf_spectacular_websocket-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-25 18:41:01.000000 drf_spectacular_websocket-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-25 18:41:01.000000 drf_spectacular_websocket-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:41:11.778108 drf_spectacular_websocket-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:41:11.774108 drf_spectacular_websocket-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:41:11.774108 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-25 18:41:01.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-25 18:41:01.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-25 18:41:01.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:41:11.778108 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:41:01.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-25 18:41:01.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/schemas/consumer_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-25 18:41:01.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/schemas/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-25 18:41:01.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:41:11.778108 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-25 18:41:11.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-25 18:41:11.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:41:11.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-25 18:41:11.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 18:41:11.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket.egg-info/top_level.txt
```

### Comparing `drf_spectacular_websocket-1.0.0/drf_spectacular_websocket/decorators.py` & `drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/decorators.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from drf_spectacular.utils import extend_schema
-
-from .schemas.consumer_schema import ConsumerAutoSchema
-
-__all__ = ('extend_ws_schema',)
-
-
-def extend_ws_schema(
-    type: str = 'send',  # noqa: A002
-    **kwargs,
-):
-    """
-    - `type`
-        - `send` - Type of interaction, [request -> response]
-        - `receive` - Type of interaction, [response without request]
-    ---
-    - Example request:
-        - request=None
-        - request=SomeSerializer
-
-    - Example responses:
-        - responses=SomeSerializer
-        - responses=SomeSerializer(many=True)
-        - responses={200: Some1Serializer, 201: Some2Serializer}
-    """
-
-    def decorator(func):
-        func.schema = ConsumerAutoSchema
-        func.type = type
-        func.event = func.__name__
-        func.include_event = False
-        return extend_schema(type, **kwargs)(func)
-
-    return decorator
+from drf_spectacular.utils import extend_schema
+
+from .schemas.consumer_schema import ConsumerAutoSchema
+
+__all__ = ('extend_ws_schema',)
+
+
+def extend_ws_schema(
+    type: str = 'send',  # noqa: A002
+    **kwargs,
+):
+    """
+    - `type`
+        - `send` - Type of interaction, [request -> response]
+        - `receive` - Type of interaction, [response without request]
+    ---
+    - Example request:
+        - request=None
+        - request=SomeSerializer
+
+    - Example responses:
+        - responses=SomeSerializer
+        - responses=SomeSerializer(many=True)
+        - responses={200: Some1Serializer, 201: Some2Serializer}
+    """
+
+    def decorator(func):
+        func.schema = ConsumerAutoSchema
+        func.type = type
+        func.event = func.__name__
+        func.include_event = False
+        return extend_schema(type, **kwargs)(func)
+
+    return decorator
```

### Comparing `drf_spectacular_websocket-1.0.0/drf_spectacular_websocket/schemas/consumer_schema.py` & `drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/schemas/consumer_schema.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,184 +1,184 @@
-from drf_spectacular.openapi import AutoSchema
-from drf_spectacular.plumbing import (
-    build_media_type_object,
-    force_instance,
-    is_list_serializer,
-    is_serializer,
-)
-from inflection import camelize
-from rest_framework import serializers, status
-from rest_framework.parsers import JSONParser
-from rest_framework.renderers import JSONRenderer
-
-
-class EmptySerializer(serializers.Serializer):
-    pass
-
-
-class NotReadyError(Exception):
-    pass
-
-
-class EventHandler:
-    request = None
-    kwargs = {}
-    versioning_class = None
-
-    def __init__(self, name):
-        self.name = name
-
-    def get_parsers(self):
-        return [JSONParser]
-
-    def get_renderers(self):
-        return [JSONRenderer]
-
-    def determine_version(self, *args, **kwargs):
-        return None, None
-
-
-class ConsumerAutoSchema(AutoSchema):
-    """"""
-
-    def __init__(self):
-        super().__init__()
-        self.method_name: str | None = None
-        self.event: str | None = None
-        self.prepared = {'request': {}, 'response': {}}
-
-    @property
-    def view(self):
-        return EventHandler(name=self.event)
-
-    def get_operation_id(self):
-        return '%s_%s' % (self.method, self.method_name)
-
-    def get_request_body(self, serializer, method):
-        _, serializer = self._force_ws_serializer(
-            serializer=serializer, serializer_type='request'
-        ).popitem()
-
-        schema, request_body_required = self._get_request_for_media_type(serializer, method)
-        if schema is None:
-            return None
-
-        content = [
-            (media_type, schema, self._get_examples(serializer, 'request', media_type))
-            for media_type in self.map_parsers()
-        ]
-
-        return {
-            'content': {
-                media_type: build_media_type_object(schema, examples)
-                for media_type, schema, examples in content
-            }
-        }
-
-    def _get_request_for_media_type(self, serializer, method):
-        component = self.resolve_serializer(serializer, method)
-
-        if not component:
-            # serializer is empty so skip content enumeration
-            return None, False
-
-        schema = component.ref
-        return schema, True
-
-    def get_response_bodies(self, response_serializers, method):
-        if response_serializers:
-            if isinstance(response_serializers, dict):
-                return {
-                    f'{self.event}   {code}': self._get_response_for_code(
-                        force_instance(serializer), code
-                    )
-                    for code, serializer in response_serializers.items()
-                }
-
-            serializers_ = self._force_ws_serializer(
-                serializer=response_serializers, direction='receive', serializer_type='response'
-            )
-
-            return {
-                f'{event}   {status.HTTP_200_OK}': self._get_response_for_code(
-                    serializer, status.HTTP_200_OK
-                )
-                for event, serializer in serializers_.items()
-            }
-
-    def _get_serializer_name(self, serializer, direction: str, bypass_extensions: bool = False):
-        return serializer.__class__.__name__
-
-    def get_tags(self):
-        return ['web_socket']
-
-    def get_summary(self):
-        return ''
-
-    def _force_ws_serializer(
-        self, serializer, direction: str | None = None, serializer_type: str | None = None
-    ) -> dict[str, serializers.Serializer]:
-        if serializer is None:
-            return {self.event: force_instance(EmptySerializer)}
-
-        serializer = force_instance(serializer)
-
-        if isinstance(serializer, EmptySerializer):
-            return {self.event: serializer}
-
-        if direction is None:
-            direction = self.method
-
-        if isinstance(serializer, list):
-            return self._force_serializers_list(events=serializer, serializer_type=serializer_type)
-
-        if self.event in self.prepared[serializer_type]:
-            return {self.event: self.prepared[serializer_type][self.event]}
-
-        if is_list_serializer(serializer):
-            serializer_name = serializer.child.__class__.__name__
-        elif is_serializer(serializer):
-            serializer_name = serializer.__class__.__name__
-        else:
-            raise AssertionError('Invalid type of serializer')
-
-        name: str = self._get_forced_serializer_name(
-            direction=direction, serializer_name=serializer_name
-        )
-
-        if is_list_serializer(serializer):
-            inner_name: str = 'Ws%sDataSerializer' % self.event.capitalize()
-            serializer = type(inner_name, (serializers.Serializer,), {self.event: serializer})()
-
-            attrs = {
-                'event': serializers.CharField(default=self.event),
-                'data': serializer,
-            }
-        else:
-            attrs = {
-                'event': serializers.CharField(default=self.event),
-                'data': serializer,
-            }
-
-        prepared = type(name, (serializers.Serializer,), attrs)() if self.include_event else serializer
-
-        self.prepared[serializer_type][self.event] = prepared
-        return {self.event: prepared}
-
-    def _force_serializers_list(self, events, serializer_type) -> dict[str, serializers.Serializer]:
-        result: dict[str, serializers.Serializer] = {}
-
-        for event in events:
-            forced = self.prepared[serializer_type].get(event)
-            if forced is None:
-                raise NotReadyError
-            result[event] = forced
-
-        return result
-
-    def _get_forced_serializer_name(self, direction: str, serializer_name: str) -> str:
-        name: str = 'Ws%s' % direction.capitalize()
-        event: str = camelize(self.event)
-        if serializer_name.startswith(event):
-            return '%s%s' % (name, serializer_name)
-
-        return '%s%s%s' % (name, event, serializer_name)
+from drf_spectacular.openapi import AutoSchema
+from drf_spectacular.plumbing import (
+    build_media_type_object,
+    force_instance,
+    is_list_serializer,
+    is_serializer,
+)
+from inflection import camelize
+from rest_framework import serializers, status
+from rest_framework.parsers import JSONParser
+from rest_framework.renderers import JSONRenderer
+
+
+class EmptySerializer(serializers.Serializer):
+    pass
+
+
+class NotReadyError(Exception):
+    pass
+
+
+class EventHandler:
+    request = None
+    kwargs = {}
+    versioning_class = None
+
+    def __init__(self, name):
+        self.name = name
+
+    def get_parsers(self):
+        return [JSONParser]
+
+    def get_renderers(self):
+        return [JSONRenderer]
+
+    def determine_version(self, *args, **kwargs):
+        return None, None
+
+
+class ConsumerAutoSchema(AutoSchema):
+    """"""
+
+    def __init__(self):
+        super().__init__()
+        self.method_name: str | None = None
+        self.event: str | None = None
+        self.prepared = {'request': {}, 'response': {}}
+
+    @property
+    def view(self):
+        return EventHandler(name=self.event)
+
+    def get_operation_id(self):
+        return '%s_%s' % (self.method, self.method_name)
+
+    def get_request_body(self, serializer, method):
+        _, serializer = self._force_ws_serializer(
+            serializer=serializer, serializer_type='request'
+        ).popitem()
+
+        schema, request_body_required = self._get_request_for_media_type(serializer, method)
+        if schema is None:
+            return None
+
+        content = [
+            (media_type, schema, self._get_examples(serializer, 'request', media_type))
+            for media_type in self.map_parsers()
+        ]
+
+        return {
+            'content': {
+                media_type: build_media_type_object(schema, examples)
+                for media_type, schema, examples in content
+            }
+        }
+
+    def _get_request_for_media_type(self, serializer, method):
+        component = self.resolve_serializer(serializer, method)
+
+        if not component:
+            # serializer is empty so skip content enumeration
+            return None, False
+
+        schema = component.ref
+        return schema, True
+
+    def get_response_bodies(self, response_serializers, method):
+        if response_serializers:
+            if isinstance(response_serializers, dict):
+                return {
+                    f'{self.event}   {code}': self._get_response_for_code(
+                        force_instance(serializer), code
+                    )
+                    for code, serializer in response_serializers.items()
+                }
+
+            serializers_ = self._force_ws_serializer(
+                serializer=response_serializers, direction='receive', serializer_type='response'
+            )
+
+            return {
+                f'{event}   {status.HTTP_200_OK}': self._get_response_for_code(
+                    serializer, status.HTTP_200_OK
+                )
+                for event, serializer in serializers_.items()
+            }
+
+    def _get_serializer_name(self, serializer, direction: str, bypass_extensions: bool = False):
+        return serializer.__class__.__name__
+
+    def get_tags(self):
+        return ['web_socket']
+
+    def get_summary(self):
+        return ''
+
+    def _force_ws_serializer(
+        self, serializer, direction: str | None = None, serializer_type: str | None = None
+    ) -> dict[str, serializers.Serializer]:
+        if serializer is None:
+            return {self.event: force_instance(EmptySerializer)}
+
+        serializer = force_instance(serializer)
+
+        if isinstance(serializer, EmptySerializer):
+            return {self.event: serializer}
+
+        if direction is None:
+            direction = self.method
+
+        if isinstance(serializer, list):
+            return self._force_serializers_list(events=serializer, serializer_type=serializer_type)
+
+        if self.event in self.prepared[serializer_type]:
+            return {self.event: self.prepared[serializer_type][self.event]}
+
+        if is_list_serializer(serializer):
+            serializer_name = serializer.child.__class__.__name__
+        elif is_serializer(serializer):
+            serializer_name = serializer.__class__.__name__
+        else:
+            raise AssertionError('Invalid type of serializer')
+
+        name: str = self._get_forced_serializer_name(
+            direction=direction, serializer_name=serializer_name
+        )
+
+        if is_list_serializer(serializer):
+            inner_name: str = 'Ws%sDataSerializer' % self.event.capitalize()
+            serializer = type(inner_name, (serializers.Serializer,), {self.event: serializer})()
+
+            attrs = {
+                'event': serializers.CharField(default=self.event),
+                'data': serializer,
+            }
+        else:
+            attrs = {
+                'event': serializers.CharField(default=self.event),
+                'data': serializer,
+            }
+
+        prepared = type(name, (serializers.Serializer,), attrs)() if self.include_event else serializer
+
+        self.prepared[serializer_type][self.event] = prepared
+        return {self.event: prepared}
+
+    def _force_serializers_list(self, events, serializer_type) -> dict[str, serializers.Serializer]:
+        result: dict[str, serializers.Serializer] = {}
+
+        for event in events:
+            forced = self.prepared[serializer_type].get(event)
+            if forced is None:
+                raise NotReadyError
+            result[event] = forced
+
+        return result
+
+    def _get_forced_serializer_name(self, direction: str, serializer_name: str) -> str:
+        name: str = 'Ws%s' % direction.capitalize()
+        event: str = camelize(self.event)
+        if serializer_name.startswith(event):
+            return '%s%s' % (name, serializer_name)
+
+        return '%s%s%s' % (name, event, serializer_name)
```

### Comparing `drf_spectacular_websocket-1.0.0/drf_spectacular_websocket/schemas/schema.py` & `drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/schemas/schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-from collections.abc import Callable
-
-from channels.routing import URLRouter
-from django.conf import settings
-from django.contrib.admindocs.views import simplify_regex
-from django.utils.module_loading import import_string
-from drf_spectacular.generators import SchemaGenerator
-
-from .consumer_schema import NotReadyError
-
-
-class WsSchemaGenerator(SchemaGenerator):
-    """"""
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.prepared = {'request': {}, 'response': {}}
-
-    def parse(self, input_request, public):
-        result = super().parse(input_request, public)
-        ws_result = self.get_ws_endpoints()
-        result.update(ws_result)
-        return result
-
-    @staticmethod
-    def get_asgi_application():
-        return import_string(settings.ASGI_APPLICATION)
-
-    def get_ws_endpoints(self):
-        application = self.get_asgi_application()
-
-        socket_routes = application.application_mapping.get('websocket')
-
-        if socket_routes is None:
-            return []
-
-        router = socket_routes
-
-        while not isinstance(router, URLRouter):
-            router = self._get_router(router)
-
-        result = {}
-
-        for route in router.routes:
-            consumer = route.callback.consumer_class()
-            result.update(self._find_methods(consumer=consumer, path=simplify_regex(str(route.pattern))))
-
-        return result
-
-    def _get_router(self, middleware):
-        try:
-            return middleware.inner
-        except AttributeError:
-            try:
-                return middleware.application
-            except AttributeError:
-                return middleware._auths[0]
-
-    def _find_methods(self, consumer, path: str):
-        consumer_endpoints = {}
-
-        methods_list = self._get_extended_methods_list(consumer)
-        while methods_list:
-            method = methods_list.pop(0)
-            event: str = method.event
-            name: str = '%s::%s' % (path, event)
-
-            action_schema = self.get_action_schema(method=method)
-            try:
-                consumer_endpoints[name] = {
-                    action_schema.method == 'receive' and 'get' or 'post': {
-                        'operationId': action_schema.get_operation_id(),
-                        'requestBody': action_schema.get_request_body(
-                            serializer=action_schema.get_request_serializer(),
-                            method=action_schema.method,
-                        ),
-                        'summary': action_schema.get_summary(),
-                        'description': action_schema.get_description(),
-                        'tags': action_schema.get_tags(),
-                        'responses': action_schema.get_response_bodies(
-                            action_schema.get_response_serializers(),
-                            method=action_schema.method,
-                        ),
-                    }
-                }
-            except NotReadyError:
-                methods_list.append(method)
-
-        return consumer_endpoints
-
-    @staticmethod
-    def _get_extended_methods_list(consumer):
-        methods_list: list[Callable] = []
-        for attr in dir(consumer):
-            method = getattr(consumer, attr)
-            if callable(method) and hasattr(method, 'kwargs'):
-                methods_list.append(method)
-
-        return methods_list
-
-    def get_action_schema(self, method: Callable):
-        schema_class = getattr(method, 'kwargs', {}).get('schema', None)
-        schema = schema_class()
-        schema.method_name = method.__name__
-        schema.method = method.type
-        schema.event = method.event
-        schema.include_event = method.include_event
-        schema.registry = self.registry
-        schema.prepared = self.prepared
-
-        return schema
+from collections.abc import Callable
+
+from channels.routing import URLRouter
+from django.conf import settings
+from django.contrib.admindocs.views import simplify_regex
+from django.utils.module_loading import import_string
+from drf_spectacular.generators import SchemaGenerator
+
+from .consumer_schema import NotReadyError
+
+
+class WsSchemaGenerator(SchemaGenerator):
+    """"""
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.prepared = {'request': {}, 'response': {}}
+
+    def parse(self, input_request, public):
+        result = super().parse(input_request, public)
+        ws_result = self.get_ws_endpoints()
+        result.update(ws_result)
+        return result
+
+    @staticmethod
+    def get_asgi_application():
+        return import_string(settings.ASGI_APPLICATION)
+
+    def get_ws_endpoints(self):
+        application = self.get_asgi_application()
+
+        socket_routes = application.application_mapping.get('websocket')
+
+        if socket_routes is None:
+            return []
+
+        router = socket_routes
+
+        while not isinstance(router, URLRouter):
+            router = self._get_router(router)
+
+        result = {}
+
+        for route in router.routes:
+            consumer = route.callback.consumer_class()
+            result.update(self._find_methods(consumer=consumer, path=simplify_regex(str(route.pattern))))
+
+        return result
+
+    def _get_router(self, middleware):
+        try:
+            return middleware.inner
+        except AttributeError:
+            try:
+                return middleware.application
+            except AttributeError:
+                return middleware._auths[0]
+
+    def _find_methods(self, consumer, path: str):
+        consumer_endpoints = {}
+
+        methods_list = self._get_extended_methods_list(consumer)
+        while methods_list:
+            method = methods_list.pop(0)
+            event: str = method.event
+            name: str = '%s::%s' % (path, event)
+
+            action_schema = self.get_action_schema(method=method)
+            try:
+                consumer_endpoints[name] = {
+                    action_schema.method == 'receive' and 'get' or 'post': {
+                        'operationId': f'{event}_{action_schema.get_operation_id()}',
+                        'requestBody': action_schema.get_request_body(
+                            serializer=action_schema.get_request_serializer(),
+                            method=action_schema.method,
+                        ),
+                        'summary': action_schema.get_summary(),
+                        'description': action_schema.get_description(),
+                        'tags': action_schema.get_tags(),
+                        'responses': action_schema.get_response_bodies(
+                            action_schema.get_response_serializers(),
+                            method=action_schema.method,
+                        ),
+                    }
+                }
+            except NotReadyError:
+                methods_list.append(method)
+
+        return consumer_endpoints
+
+    @staticmethod
+    def _get_extended_methods_list(consumer):
+        methods_list: list[Callable] = []
+        for attr in dir(consumer):
+            method = getattr(consumer, attr)
+            if callable(method) and hasattr(method, 'kwargs'):
+                methods_list.append(method)
+
+        return methods_list
+
+    def get_action_schema(self, method: Callable):
+        schema_class = getattr(method, 'kwargs', {}).get('schema', None)
+        schema = schema_class()
+        schema.method_name = method.__name__
+        schema.method = method.type
+        schema.event = method.event
+        schema.include_event = method.include_event
+        schema.registry = self.registry
+        schema.prepared = self.prepared
+
+        return schema
```

### Comparing `drf_spectacular_websocket-1.0.0/drf_spectacular_websocket/settings.py` & `drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/settings.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from django.conf import settings
-
-SPECTACULAR_SETTINGS: dict = getattr(settings, 'SPECTACULAR_SETTINGS', {})
-
-SPECTACULAR_SETTINGS['DEFAULT_GENERATOR_CLASS'] = 'drf_spectacular_websocket.schemas.WsSchemaGenerator'
-SPECTACULAR_SETTINGS['SWAGGER_UI_DIST'] = 'SIDECAR'
-SPECTACULAR_SETTINGS['SWAGGER_UI_FAVICON_HREF'] = 'SIDECAR'
-SPECTACULAR_SETTINGS['REDOC_DIST'] = 'SIDECAR'
-SWAGGER_UI_SETTINGS: dict = SPECTACULAR_SETTINGS.get('SWAGGER_UI_SETTINGS', {})
-SWAGGER_UI_SETTINGS.setdefault('connectSocket', True)
-SWAGGER_UI_SETTINGS.setdefault('socketMaxMessages', 8)
-SWAGGER_UI_SETTINGS.setdefault('socketMessagesInitialOpened', False)
+from django.conf import settings
+
+SPECTACULAR_SETTINGS: dict = getattr(settings, 'SPECTACULAR_SETTINGS', {})
+
+SPECTACULAR_SETTINGS['DEFAULT_GENERATOR_CLASS'] = 'drf_spectacular_websocket.schemas.WsSchemaGenerator'
+SPECTACULAR_SETTINGS['SWAGGER_UI_DIST'] = 'SIDECAR'
+SPECTACULAR_SETTINGS['SWAGGER_UI_FAVICON_HREF'] = 'SIDECAR'
+SPECTACULAR_SETTINGS['REDOC_DIST'] = 'SIDECAR'
+SWAGGER_UI_SETTINGS: dict = SPECTACULAR_SETTINGS.get('SWAGGER_UI_SETTINGS', {})
+SWAGGER_UI_SETTINGS.setdefault('connectSocket', True)
+SWAGGER_UI_SETTINGS.setdefault('socketMaxMessages', 8)
+SWAGGER_UI_SETTINGS.setdefault('socketMessagesInitialOpened', False)
```

