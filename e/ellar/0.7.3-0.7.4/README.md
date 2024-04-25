# Comparing `tmp/ellar-0.7.3.tar.gz` & `tmp/ellar-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ellar-0.7.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ellar-0.7.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ellar-0.7.3.tar` & `ellar-0.7.4.tar`

### file list

```diff
@@ -1,311 +1,311 @@
--rw-r--r--   0        0        0     6804 2024-04-07 11:54:25.295505 ellar-0.7.3/README.md
--rw-r--r--   0        0        0      149 2024-04-07 11:54:25.335506 ellar-0.7.3/ellar/__init__.py
--rw-r--r--   0        0        0      182 2024-04-07 11:54:25.335506 ellar-0.7.3/ellar/app/__init__.py
--rw-r--r--   0        0        0     3281 2024-04-07 11:54:25.335506 ellar-0.7.3/ellar/app/context.py
--rw-r--r--   0        0        0     7931 2024-04-07 11:54:25.335506 ellar-0.7.3/ellar/app/factory.py
--rw-r--r--   0        0        0     2664 2024-04-07 11:54:25.335506 ellar-0.7.3/ellar/app/lifespan.py
--rw-r--r--   0        0        0    12053 2024-04-07 11:54:25.335506 ellar-0.7.3/ellar/app/main.py
--rw-r--r--   0        0        0     2267 2024-04-07 11:54:25.335506 ellar-0.7.3/ellar/app/services.py
--rw-r--r--   0        0        0      810 2024-04-07 11:54:25.335506 ellar-0.7.3/ellar/auth/__init__.py
--rw-r--r--   0        0        0       55 2024-04-07 11:54:25.335506 ellar-0.7.3/ellar/auth/constants.py
--rw-r--r--   0        0        0     2139 2024-04-07 11:54:25.335506 ellar-0.7.3/ellar/auth/decorators.py
--rw-r--r--   0        0        0      411 2024-04-07 11:54:25.335506 ellar-0.7.3/ellar/auth/guards/__init__.py
--rw-r--r--   0        0        0     1281 2024-04-07 11:54:25.335506 ellar-0.7.3/ellar/auth/guards/apikey.py
--rw-r--r--   0        0        0     1405 2024-04-07 11:54:25.335506 ellar-0.7.3/ellar/auth/guards/auth_required.py
--rw-r--r--   0        0        0      472 2024-04-07 11:54:25.335506 ellar-0.7.3/ellar/auth/guards/http.py
--rw-r--r--   0        0        0      356 2024-04-07 11:54:25.335506 ellar-0.7.3/ellar/auth/guards/mixin.py
--rw-r--r--   0        0        0      575 2024-04-07 11:54:25.335506 ellar-0.7.3/ellar/auth/handlers/__init__.py
--rw-r--r--   0        0        0      636 2024-04-07 11:54:25.335506 ellar-0.7.3/ellar/auth/handlers/api_key.py
--rw-r--r--   0        0        0      472 2024-04-07 11:54:25.335506 ellar-0.7.3/ellar/auth/handlers/http.py
--rw-r--r--   0        0        0      698 2024-04-07 11:54:25.335506 ellar-0.7.3/ellar/auth/handlers/mixin.py
--rw-r--r--   0        0        0      683 2024-04-07 11:54:25.335506 ellar-0.7.3/ellar/auth/handlers/model.py
--rw-r--r--   0        0        0      371 2024-04-07 11:54:25.335506 ellar-0.7.3/ellar/auth/handlers/schemes/__init__.py
--rw-r--r--   0        0        0      781 2024-04-07 11:54:25.335506 ellar-0.7.3/ellar/auth/handlers/schemes/api_key.py
--rw-r--r--   0        0        0     5205 2024-04-07 11:54:25.335506 ellar-0.7.3/ellar/auth/handlers/schemes/base.py
--rw-r--r--   0        0        0     3634 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/auth/handlers/schemes/http.py
--rw-r--r--   0        0        0      223 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/auth/identity.py
--rw-r--r--   0        0        0     1750 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/auth/interceptor.py
--rw-r--r--   0        0        0      142 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/auth/middleware/__init__.py
--rw-r--r--   0        0        0     1625 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/auth/middleware/auth.py
--rw-r--r--   0        0        0     2239 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/auth/middleware/session.py
--rw-r--r--   0        0        0      370 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/auth/policy/__init__.py
--rw-r--r--   0        0        0     5189 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/auth/policy/base.py
--rw-r--r--   0        0        0      940 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/auth/policy/common.py
--rw-r--r--   0        0        0      177 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/auth/services/__init__.py
--rw-r--r--   0        0        0     1046 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/auth/services/auth_schemes.py
--rw-r--r--   0        0        0     1637 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/auth/services/middleware.py
--rw-r--r--   0        0        0      934 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/auth/session/__init__.py
--rw-r--r--   0        0        0     1622 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/auth/session/base.py
--rw-r--r--   0        0        0     1699 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/auth/session/cookie_dict.py
--rw-r--r--   0        0        0      384 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/auth/session/options.py
--rw-r--r--   0        0        0     2174 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/auth/session/strategy.py
--rw-r--r--   0        0        0      257 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/cache/__init__.py
--rw-r--r--   0        0        0      109 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/cache/backends/__init__.py
--rw-r--r--   0        0        0     4841 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/cache/backends/_aio_cache.py.ellar
--rw-r--r--   0        0        0     4633 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/cache/backends/base.py
--rw-r--r--   0        0        0     5406 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/cache/backends/local_cache.py
--rw-r--r--   0        0        0      971 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/cache/backends/pylib_cache.py
--rw-r--r--   0        0        0     2240 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/cache/backends/pymem_cache.py
--rw-r--r--   0        0        0       72 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/cache/backends/redis/__init__.py
--rw-r--r--   0        0        0     6813 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/cache/backends/redis/backend.py
--rw-r--r--   0        0        0     1413 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/cache/backends/serializer.py
--rw-r--r--   0        0        0     3018 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/cache/decorator.py
--rw-r--r--   0        0        0    11819 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/cache/interface.py
--rw-r--r--   0        0        0     2045 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/cache/make_key_decorator.py
--rw-r--r--   0        0        0     2657 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/cache/model.py
--rw-r--r--   0        0        0     1882 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/cache/module.py
--rw-r--r--   0        0        0      867 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/cache/schema.py
--rw-r--r--   0        0        0     5077 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/cache/service.py
--rw-r--r--   0        0        0     3791 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/__init__.py
--rw-r--r--   0        0        0      195 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/compatible/__init__.py
--rw-r--r--   0        0        0     1163 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/compatible/cache_properties.py
--rw-r--r--   0        0        0      891 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/compatible/dict.py
--rw-r--r--   0        0        0     4901 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/constants.py
--rw-r--r--   0        0        0     1672 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/converters.py
--rw-r--r--   0        0        0     2829 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/datastructures.py
--rw-r--r--   0        0        0      811 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/decorators/__init__.py
--rw-r--r--   0        0        0      628 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/decorators/base.py
--rw-r--r--   0        0        0     3850 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/decorators/controller.py
--rw-r--r--   0        0        0     1042 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/decorators/exception.py
--rw-r--r--   0        0        0      610 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/decorators/extra_args.py
--rw-r--r--   0        0        0     2528 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/decorators/file.py
--rw-r--r--   0        0        0     1026 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/decorators/guards.py
--rw-r--r--   0        0        0     4740 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/decorators/html.py
--rw-r--r--   0        0        0     1085 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/decorators/interceptor.py
--rw-r--r--   0        0        0      928 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/decorators/middleware.py
--rw-r--r--   0        0        0     3154 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/decorators/modules.py
--rw-r--r--   0        0        0     1184 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/decorators/serializer.py
--rw-r--r--   0        0        0      397 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/decorators/versioning.py
--rw-r--r--   0        0        0      930 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/exceptions/__init__.py
--rw-r--r--   0        0        0      472 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/exceptions/api/__init__.py
--rw-r--r--   0        0        0     1519 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/exceptions/api/base.py
--rw-r--r--   0        0        0     1251 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/exceptions/api/exceptions_types.py
--rw-r--r--   0        0        0     2588 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/exceptions/callable_exceptions.py
--rw-r--r--   0        0        0      103 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/exceptions/context.py
--rw-r--r--   0        0        0     2537 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/exceptions/handlers.py
--rw-r--r--   0        0        0      768 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/exceptions/validation.py
--rw-r--r--   0        0        0     1325 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/interfaces/__init__.py
--rw-r--r--   0        0        0      398 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/interfaces/application.py
--rw-r--r--   0        0        0     3973 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/interfaces/context.py
--rw-r--r--   0        0        0     1769 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/interfaces/exceptions.py
--rw-r--r--   0        0        0      400 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/interfaces/guard_consumer.py
--rw-r--r--   0        0        0      684 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/interfaces/identity_schemes.py
--rw-r--r--   0        0        0      406 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/interfaces/interceptor_consumer.py
--rw-r--r--   0        0        0      404 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/interfaces/middleware.py
--rw-r--r--   0        0        0     1771 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/interfaces/module.py
--rw-r--r--   0        0        0      748 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/interfaces/response_model.py
--rw-r--r--   0        0        0      907 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/interfaces/templating.py
--rw-r--r--   0        0        0      774 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/interfaces/versioning.py
--rw-r--r--   0        0        0      104 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/logging.py
--rw-r--r--   0        0        0      363 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/models/__init__.py
--rw-r--r--   0        0        0      877 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/models/controller.py
--rw-r--r--   0        0        0      803 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/models/guard.py
--rw-r--r--   0        0        0      851 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/models/identity.py
--rw-r--r--   0        0        0      320 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/models/interceptor.py
--rw-r--r--   0        0        0      802 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/operations/__init__.py
--rw-r--r--   0        0        0     9663 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/operations/base.py
--rw-r--r--   0        0        0     2759 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/operations/router.py
--rw-r--r--   0        0        0     3632 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/operations/schema.py
--rw-r--r--   0        0        0      555 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/params/__init__.py
--rw-r--r--   0        0        0      315 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/params/args/__init__.py
--rw-r--r--   0        0        0    14710 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/params/args/base.py
--rw-r--r--   0        0        0     1657 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/params/args/extra_args.py
--rw-r--r--   0        0        0     1994 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/params/args/factory.py
--rw-r--r--   0        0        0     6837 2024-04-07 11:54:25.339506 ellar-0.7.3/ellar/common/params/args/request_model.py
--rw-r--r--   0        0        0     6180 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/params/args/resolver_generators.py
--rw-r--r--   0        0        0     2429 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/params/args/websocket_model.py
--rw-r--r--   0        0        0     4165 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/params/decorators/__init__.py
--rw-r--r--   0        0        0     2366 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/params/decorators/inject.py
--rw-r--r--   0        0        0    16837 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/params/decorators/models.py
--rw-r--r--   0        0        0    15753 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/params/params.py
--rw-r--r--   0        0        0     1106 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/params/resolvers/__init__.py
--rw-r--r--   0        0        0     1702 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/params/resolvers/base.py
--rw-r--r--   0        0        0     5758 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/params/resolvers/bulk_parameter.py
--rw-r--r--   0        0        0    11220 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/params/resolvers/parameter.py
--rw-r--r--   0        0        0      776 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/params/resolvers/system_parameters/__init__.py
--rw-r--r--   0        0        0      873 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/params/resolvers/system_parameters/background.py
--rw-r--r--   0        0        0     2726 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/params/resolvers/system_parameters/base.py
--rw-r--r--   0        0        0      397 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/params/resolvers/system_parameters/connection.py
--rw-r--r--   0        0        0      334 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/params/resolvers/system_parameters/context.py
--rw-r--r--   0        0        0     1547 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/params/resolvers/system_parameters/provider.py
--rw-r--r--   0        0        0      393 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/params/resolvers/system_parameters/request.py
--rw-r--r--   0        0        0      400 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/params/resolvers/system_parameters/response.py
--rw-r--r--   0        0        0      524 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/params/resolvers/system_parameters/session.py
--rw-r--r--   0        0        0      392 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/params/resolvers/system_parameters/websocket.py
--rw-r--r--   0        0        0      415 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/responses/__init__.py
--rw-r--r--   0        0        0      839 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/responses/models/__init__.py
--rw-r--r--   0        0        0     7921 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/responses/models/base.py
--rw-r--r--   0        0        0       50 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/responses/models/exceptions.py
--rw-r--r--   0        0        0     4305 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/responses/models/file.py
--rw-r--r--   0        0        0      726 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/responses/models/helper.py
--rw-r--r--   0        0        0     2129 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/responses/models/html.py
--rw-r--r--   0        0        0     2935 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/responses/models/json.py
--rw-r--r--   0        0        0     4865 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/responses/models/route.py
--rw-r--r--   0        0        0     1688 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/responses/models/type_converter.py
--rw-r--r--   0        0        0     1253 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/responses/response_types.py
--rw-r--r--   0        0        0      357 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/serializer/__init__.py
--rw-r--r--   0        0        0     5633 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/serializer/base.py
--rw-r--r--   0        0        0      194 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/serializer/guard.py
--rw-r--r--   0        0        0      454 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/shortcuts.py
--rw-r--r--   0        0        0      613 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/templating/__init__.py
--rw-r--r--   0        0        0      593 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/templating/environment.py
--rw-r--r--   0        0        0     2020 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/templating/loader.py
--rw-r--r--   0        0        0      835 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/templating/model.py
--rw-r--r--   0        0        0     2584 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/templating/renderer.py
--rw-r--r--   0        0        0      110 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/templating/schema.py
--rw-r--r--   0        0        0      713 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/common/types.py
--rw-r--r--   0        0        0      928 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/__init__.py
--rw-r--r--   0        0        0      162 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/conf/__init__.py
--rw-r--r--   0        0        0     5454 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/conf/app_settings_models.py
--rw-r--r--   0        0        0     2397 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/conf/config.py
--rw-r--r--   0        0        0     3270 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/conf/mixins.py
--rw-r--r--   0        0        0      469 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/connection/__init__.py
--rw-r--r--   0        0        0      855 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/connection/http.py
--rw-r--r--   0        0        0      245 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/connection/websocket.py
--rw-r--r--   0        0        0       97 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/exceptions/__init__.py
--rw-r--r--   0        0        0     2157 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/exceptions/service.py
--rw-r--r--   0        0        0      457 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/execution_context/__init__.py
--rw-r--r--   0        0        0     1327 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/execution_context/execution.py
--rw-r--r--   0        0        0     2581 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/execution_context/factory.py
--rw-r--r--   0        0        0     2280 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/execution_context/host.py
--rw-r--r--   0        0        0     2089 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/execution_context/http.py
--rw-r--r--   0        0        0      801 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/execution_context/websocket.py
--rw-r--r--   0        0        0       72 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/guards/__init__.py
--rw-r--r--   0        0        0     1729 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/guards/consumer.py
--rw-r--r--   0        0        0       87 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/interceptors/__init__.py
--rw-r--r--   0        0        0     2202 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/interceptors/consumer.py
--rw-r--r--   0        0        0     1050 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/middleware/__init__.py
--rw-r--r--   0        0        0     2905 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/middleware/di.py
--rw-r--r--   0        0        0     2689 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/middleware/exceptions.py
--rw-r--r--   0        0        0     2577 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/middleware/function.py
--rw-r--r--   0        0        0      747 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/middleware/middleware.py
--rw-r--r--   0        0        0     1049 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/middleware/versioning.py
--rw-r--r--   0        0        0      363 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/modules/__init__.py
--rw-r--r--   0        0        0     1302 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/modules/base.py
--rw-r--r--   0        0        0     3082 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/modules/builder.py
--rw-r--r--   0        0        0     7614 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/modules/config.py
--rw-r--r--   0        0        0      787 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/modules/helper.py
--rw-r--r--   0        0        0     9438 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/modules/ref.py
--rw-r--r--   0        0        0      291 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/router_builders/__init__.py
--rw-r--r--   0        0        0     2094 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/router_builders/base.py
--rw-r--r--   0        0        0     4821 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/router_builders/controller.py
--rw-r--r--   0        0        0     1251 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/router_builders/module_router.py
--rw-r--r--   0        0        0      963 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/routing/__init__.py
--rw-r--r--   0        0        0     5427 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/routing/base.py
--rw-r--r--   0        0        0      272 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/routing/controller/__init__.py
--rw-r--r--   0        0        0     1068 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/routing/controller/base.py
--rw-r--r--   0        0        0      852 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/routing/controller/route.py
--rw-r--r--   0        0        0      190 2024-04-07 11:54:25.343506 ellar-0.7.3/ellar/core/routing/controller/websocket/__init__.py
--rw-r--r--   0        0        0     1844 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/routing/controller/websocket/handler.py
--rw-r--r--   0        0        0     1564 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/routing/controller/websocket/route.py
--rw-r--r--   0        0        0     2566 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/routing/file_mount.py
--rw-r--r--   0        0        0     7056 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/routing/mount.py
--rw-r--r--   0        0        0     5321 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/routing/route.py
--rw-r--r--   0        0        0     3046 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/routing/route_collections.py
--rw-r--r--   0        0        0     2324 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/routing/utils.py
--rw-r--r--   0        0        0      161 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/routing/websocket/__init__.py
--rw-r--r--   0        0        0     6628 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/routing/websocket/handler.py
--rw-r--r--   0        0        0     5618 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/routing/websocket/route.py
--rw-r--r--   0        0        0        0 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/security/__init__.py
--rw-r--r--   0        0        0     4074 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/security/hashers/__init__.py
--rw-r--r--   0        0        0     1811 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/security/hashers/argon2.py
--rw-r--r--   0        0        0     3002 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/security/hashers/base.py
--rw-r--r--   0        0        0     1739 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/security/hashers/bcrypt.py
--rw-r--r--   0        0        0     1418 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/security/hashers/md5.py
--rw-r--r--   0        0        0     1282 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/security/hashers/pbkdf.py
--rw-r--r--   0        0        0     2774 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/security/hashers/scrypt.py
--rw-r--r--   0        0        0       82 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/services/__init__.py
--rw-r--r--   0        0        0     1977 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/services/reflector.py
--rw-r--r--   0        0        0      392 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/shortcuts.py
--rw-r--r--   0        0        0     1805 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/staticfiles.py
--rw-r--r--   0        0        0      673 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/versioning/__init__.py
--rw-r--r--   0        0        0     2569 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/versioning/base.py
--rw-r--r--   0        0        0     6148 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/core/versioning/resolver.py
--rw-r--r--   0        0        0     1184 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/di/__init__.py
--rw-r--r--   0        0        0      344 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/di/asgi_args.py
--rw-r--r--   0        0        0     1071 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/di/constants.py
--rw-r--r--   0        0        0        0 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/di/context.py
--rw-r--r--   0        0        0      400 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/di/exceptions.py
--rw-r--r--   0        0        0      117 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/di/injector/__init__.py
--rw-r--r--   0        0        0     7713 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/di/injector/container.py
--rw-r--r--   0        0        0     5045 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/di/injector/ellar_injector.py
--rw-r--r--   0        0        0      154 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/di/logger.py
--rw-r--r--   0        0        0     1001 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/di/providers.py
--rw-r--r--   0        0        0     2050 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/di/scopes.py
--rw-r--r--   0        0        0     4671 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/di/service_config.py
--rw-r--r--   0        0        0       39 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/di/types.py
--rw-r--r--   0        0        0      244 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/di/utils.py
--rw-r--r--   0        0        0      231 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/events/__init__.py
--rw-r--r--   0        0        0     1951 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/events/base.py
--rw-r--r--   0        0        0      579 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/openapi/__init__.py
--rw-r--r--   0        0        0    10854 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/openapi/builder.py
--rw-r--r--   0        0        0      243 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/openapi/constants.py
--rw-r--r--   0        0        0       94 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/openapi/decorators/__init__.py
--rw-r--r--   0        0        0     1199 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/openapi/decorators/extra_info.py
--rw-r--r--   0        0        0      731 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/openapi/decorators/tags.py
--rw-r--r--   0        0        0      219 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/openapi/docs_ui/__init__.py
--rw-r--r--   0        0        0     1138 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/openapi/docs_ui/base.py
--rw-r--r--   0        0        0      932 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/openapi/docs_ui/redocs.py
--rw-r--r--   0        0        0     2226 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/openapi/docs_ui/stoplight.py
--rw-r--r--   0        0        0     1078 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/openapi/docs_ui/swagger.py
--rw-r--r--   0        0        0     5520 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/openapi/module.py
--rw-r--r--   0        0        0    13873 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/openapi/openapi_v3.py
--rw-r--r--   0        0        0    16013 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/openapi/route_doc_models.py
--rw-r--r--   0        0        0      115 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/openapi/schemas/__init__.py
--rw-r--r--   0        0        0      348 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/openapi/schemas/validation.py
--rw-r--r--   0        0        0    50277 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/openapi/static/swagger/SwaggerDark.css
--rw-r--r--   0        0        0      702 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/openapi/templates/redocs.html
--rw-r--r--   0        0        0      895 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/openapi/templates/swagger.html
--rw-r--r--   0        0        0        0 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/py.typed
--rw-r--r--   0        0        0     2082 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/pydantic/__init__.py
--rw-r--r--   0        0        0     1528 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/pydantic/decorator.py
--rw-r--r--   0        0        0      764 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/pydantic/emails.py
--rw-r--r--   0        0        0     1798 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/pydantic/encoder.py
--rw-r--r--   0        0        0     1718 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/pydantic/exceptions.py
--rw-r--r--   0        0        0      692 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/pydantic/field_constraints.py
--rw-r--r--   0        0        0     2850 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/pydantic/fields.py
--rw-r--r--   0        0        0      397 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/pydantic/types.py
--rw-r--r--   0        0        0     8596 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/pydantic/utils.py
--rw-r--r--   0        0        0      105 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/reflect/__init__.py
--rw-r--r--   0        0        0     5389 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/reflect/_reflect.py
--rw-r--r--   0        0        0       34 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/reflect/constants.py
--rw-r--r--   0        0        0       58 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/samples/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/samples/controllers/__init__.py
--rw-r--r--   0        0        0      232 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/samples/controllers/guard.py
--rw-r--r--   0        0        0      704 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/samples/controllers/home.py
--rw-r--r--   0        0        0      211 2024-04-07 11:54:25.347506 ellar-0.7.3/ellar/samples/modules.py
--rw-r--r--   0        0        0   232915 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/samples/static/css/bootstrap.min.css
--rw-r--r--   0        0        0      721 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/samples/static/css/cover.css
--rwxr-xr-x   0        0        0    25915 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/samples/static/img/EllarLogoB.png
--rwxr-xr-x   0        0        0    36744 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/samples/static/img/EllarLogoIconOnly.png
--rwxr-xr-x   0        0        0     3888 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/samples/static/img/Icon.svg
--rw-r--r--   0        0        0     2575 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/samples/templates/home/index.html
--rw-r--r--   0        0        0      629 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/socket_io/__init__.py
--rw-r--r--   0        0        0      422 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/socket_io/adapter.py
--rw-r--r--   0        0        0      543 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/socket_io/constants.py
--rw-r--r--   0        0        0     1914 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/socket_io/context.py
--rw-r--r--   0        0        0      225 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/socket_io/decorators/__init__.py
--rw-r--r--   0        0        0      667 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/socket_io/decorators/events.py
--rw-r--r--   0        0        0     3034 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/socket_io/decorators/gateway.py
--rw-r--r--   0        0        0      570 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/socket_io/decorators/subscribe_message.py
--rw-r--r--   0        0        0     4177 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/socket_io/factory.py
--rw-r--r--   0        0        0     9619 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/socket_io/gateway.py
--rw-r--r--   0        0        0      144 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/socket_io/model.py
--rw-r--r--   0        0        0      532 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/socket_io/responses.py
--rw-r--r--   0        0        0      107 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/socket_io/testing/__init__.py
--rw-r--r--   0        0        0     1700 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/socket_io/testing/module.py
--rw-r--r--   0        0        0      129 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/testing/__init__.py
--rw-r--r--   0        0        0     4656 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/testing/module.py
--rw-r--r--   0        0        0     1236 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/testing/uvicorn_server.py
--rw-r--r--   0        0        0       60 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/threading/__init__.py
--rw-r--r--   0        0        0     8476 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/threading/sync_worker.py
--rw-r--r--   0        0        0      664 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/threading/utils.py
--rw-r--r--   0        0        0     2386 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/utils/__init__.py
--rw-r--r--   0        0        0      870 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/utils/crypto.py
--rw-r--r--   0        0        0      658 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/utils/enums.py
--rw-r--r--   0        0        0      389 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/utils/event_loop.py
--rw-r--r--   0        0        0     7692 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/utils/functional.py
--rw-r--r--   0        0        0     3810 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/utils/importer.py
--rw-r--r--   0        0        0      723 2024-04-07 11:54:25.351506 ellar-0.7.3/ellar/utils/module_loading.py
--rw-r--r--   0        0        0     3363 2024-04-07 11:54:25.351506 ellar-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     9098 1970-01-01 00:00:00.000000 ellar-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     6789 2024-04-25 08:12:14.586263 ellar-0.7.4/README.md
+-rw-r--r--   0        0        0      149 2024-04-25 08:12:14.626263 ellar-0.7.4/ellar/__init__.py
+-rw-r--r--   0        0        0      182 2024-04-25 08:12:14.626263 ellar-0.7.4/ellar/app/__init__.py
+-rw-r--r--   0        0        0     3281 2024-04-25 08:12:14.626263 ellar-0.7.4/ellar/app/context.py
+-rw-r--r--   0        0        0     7931 2024-04-25 08:12:14.626263 ellar-0.7.4/ellar/app/factory.py
+-rw-r--r--   0        0        0     2664 2024-04-25 08:12:14.626263 ellar-0.7.4/ellar/app/lifespan.py
+-rw-r--r--   0        0        0    12053 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/app/main.py
+-rw-r--r--   0        0        0     2267 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/app/services.py
+-rw-r--r--   0        0        0      810 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/__init__.py
+-rw-r--r--   0        0        0       55 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/constants.py
+-rw-r--r--   0        0        0     2139 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/decorators.py
+-rw-r--r--   0        0        0      411 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/guards/__init__.py
+-rw-r--r--   0        0        0     1281 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/guards/apikey.py
+-rw-r--r--   0        0        0     1405 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/guards/auth_required.py
+-rw-r--r--   0        0        0      472 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/guards/http.py
+-rw-r--r--   0        0        0      356 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/guards/mixin.py
+-rw-r--r--   0        0        0      575 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/handlers/__init__.py
+-rw-r--r--   0        0        0      636 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/handlers/api_key.py
+-rw-r--r--   0        0        0      472 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/handlers/http.py
+-rw-r--r--   0        0        0      698 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/handlers/mixin.py
+-rw-r--r--   0        0        0      683 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/handlers/model.py
+-rw-r--r--   0        0        0      371 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/handlers/schemes/__init__.py
+-rw-r--r--   0        0        0      781 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/handlers/schemes/api_key.py
+-rw-r--r--   0        0        0     5205 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/handlers/schemes/base.py
+-rw-r--r--   0        0        0     3634 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/handlers/schemes/http.py
+-rw-r--r--   0        0        0      223 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/identity.py
+-rw-r--r--   0        0        0     1750 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/interceptor.py
+-rw-r--r--   0        0        0      142 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/middleware/__init__.py
+-rw-r--r--   0        0        0     1625 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/middleware/auth.py
+-rw-r--r--   0        0        0     2239 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/middleware/session.py
+-rw-r--r--   0        0        0      370 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/policy/__init__.py
+-rw-r--r--   0        0        0     5189 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/policy/base.py
+-rw-r--r--   0        0        0      940 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/policy/common.py
+-rw-r--r--   0        0        0      177 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/services/__init__.py
+-rw-r--r--   0        0        0     1046 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/services/auth_schemes.py
+-rw-r--r--   0        0        0     1637 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/services/middleware.py
+-rw-r--r--   0        0        0      934 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/session/__init__.py
+-rw-r--r--   0        0        0     1622 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/session/base.py
+-rw-r--r--   0        0        0     1699 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/session/cookie_dict.py
+-rw-r--r--   0        0        0      384 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/session/options.py
+-rw-r--r--   0        0        0     2174 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/session/strategy.py
+-rw-r--r--   0        0        0      257 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/__init__.py
+-rw-r--r--   0        0        0      109 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/backends/__init__.py
+-rw-r--r--   0        0        0     4841 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/backends/_aio_cache.py.ellar
+-rw-r--r--   0        0        0     4633 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/backends/base.py
+-rw-r--r--   0        0        0     5406 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/backends/local_cache.py
+-rw-r--r--   0        0        0      971 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/backends/pylib_cache.py
+-rw-r--r--   0        0        0     2240 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/backends/pymem_cache.py
+-rw-r--r--   0        0        0       72 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/backends/redis/__init__.py
+-rw-r--r--   0        0        0     6813 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/backends/redis/backend.py
+-rw-r--r--   0        0        0     1413 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/backends/serializer.py
+-rw-r--r--   0        0        0     3018 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/decorator.py
+-rw-r--r--   0        0        0    11819 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/interface.py
+-rw-r--r--   0        0        0     2045 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/make_key_decorator.py
+-rw-r--r--   0        0        0     2657 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/model.py
+-rw-r--r--   0        0        0     1882 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/module.py
+-rw-r--r--   0        0        0      867 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/schema.py
+-rw-r--r--   0        0        0     5077 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/service.py
+-rw-r--r--   0        0        0     3791 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/__init__.py
+-rw-r--r--   0        0        0      195 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/compatible/__init__.py
+-rw-r--r--   0        0        0     1163 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/compatible/cache_properties.py
+-rw-r--r--   0        0        0      891 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/compatible/dict.py
+-rw-r--r--   0        0        0     4901 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/constants.py
+-rw-r--r--   0        0        0     1672 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/converters.py
+-rw-r--r--   0        0        0     2829 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/datastructures.py
+-rw-r--r--   0        0        0      811 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/__init__.py
+-rw-r--r--   0        0        0      628 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/base.py
+-rw-r--r--   0        0        0     3850 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/controller.py
+-rw-r--r--   0        0        0     1042 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/exception.py
+-rw-r--r--   0        0        0      610 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/extra_args.py
+-rw-r--r--   0        0        0     2528 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/file.py
+-rw-r--r--   0        0        0     1026 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/guards.py
+-rw-r--r--   0        0        0     4740 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/html.py
+-rw-r--r--   0        0        0     1085 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/interceptor.py
+-rw-r--r--   0        0        0      928 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/middleware.py
+-rw-r--r--   0        0        0     3335 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/modules.py
+-rw-r--r--   0        0        0     1184 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/serializer.py
+-rw-r--r--   0        0        0      397 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/versioning.py
+-rw-r--r--   0        0        0      930 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/exceptions/__init__.py
+-rw-r--r--   0        0        0      472 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/exceptions/api/__init__.py
+-rw-r--r--   0        0        0     1519 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/exceptions/api/base.py
+-rw-r--r--   0        0        0     1251 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/exceptions/api/exceptions_types.py
+-rw-r--r--   0        0        0     2588 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/exceptions/callable_exceptions.py
+-rw-r--r--   0        0        0      103 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/exceptions/context.py
+-rw-r--r--   0        0        0     2537 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/exceptions/handlers.py
+-rw-r--r--   0        0        0      768 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/exceptions/validation.py
+-rw-r--r--   0        0        0     1325 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/interfaces/__init__.py
+-rw-r--r--   0        0        0      398 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/interfaces/application.py
+-rw-r--r--   0        0        0     3971 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/interfaces/context.py
+-rw-r--r--   0        0        0     1769 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/interfaces/exceptions.py
+-rw-r--r--   0        0        0      400 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/interfaces/guard_consumer.py
+-rw-r--r--   0        0        0      684 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/interfaces/identity_schemes.py
+-rw-r--r--   0        0        0      406 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/interfaces/interceptor_consumer.py
+-rw-r--r--   0        0        0      404 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/interfaces/middleware.py
+-rw-r--r--   0        0        0     1771 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/interfaces/module.py
+-rw-r--r--   0        0        0      748 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/interfaces/response_model.py
+-rw-r--r--   0        0        0      907 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/interfaces/templating.py
+-rw-r--r--   0        0        0      774 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/interfaces/versioning.py
+-rw-r--r--   0        0        0      104 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/logging.py
+-rw-r--r--   0        0        0      363 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/models/__init__.py
+-rw-r--r--   0        0        0      877 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/models/controller.py
+-rw-r--r--   0        0        0      803 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/models/guard.py
+-rw-r--r--   0        0        0      851 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/models/identity.py
+-rw-r--r--   0        0        0      320 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/models/interceptor.py
+-rw-r--r--   0        0        0      802 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/operations/__init__.py
+-rw-r--r--   0        0        0     9663 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/operations/base.py
+-rw-r--r--   0        0        0     2759 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/operations/router.py
+-rw-r--r--   0        0        0     3632 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/operations/schema.py
+-rw-r--r--   0        0        0      555 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/__init__.py
+-rw-r--r--   0        0        0      315 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/args/__init__.py
+-rw-r--r--   0        0        0    14710 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/args/base.py
+-rw-r--r--   0        0        0     1657 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/args/extra_args.py
+-rw-r--r--   0        0        0     1994 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/args/factory.py
+-rw-r--r--   0        0        0     6837 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/args/request_model.py
+-rw-r--r--   0        0        0     6180 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/args/resolver_generators.py
+-rw-r--r--   0        0        0     2429 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/args/websocket_model.py
+-rw-r--r--   0        0        0     4165 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/decorators/__init__.py
+-rw-r--r--   0        0        0     2366 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/decorators/inject.py
+-rw-r--r--   0        0        0    16837 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/decorators/models.py
+-rw-r--r--   0        0        0    15753 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/params.py
+-rw-r--r--   0        0        0     1106 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/__init__.py
+-rw-r--r--   0        0        0     1702 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/base.py
+-rw-r--r--   0        0        0     5758 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/bulk_parameter.py
+-rw-r--r--   0        0        0    11220 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/parameter.py
+-rw-r--r--   0        0        0      776 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/system_parameters/__init__.py
+-rw-r--r--   0        0        0      873 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/system_parameters/background.py
+-rw-r--r--   0        0        0     2726 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/system_parameters/base.py
+-rw-r--r--   0        0        0      397 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/system_parameters/connection.py
+-rw-r--r--   0        0        0      334 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/system_parameters/context.py
+-rw-r--r--   0        0        0     1547 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/system_parameters/provider.py
+-rw-r--r--   0        0        0      393 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/system_parameters/request.py
+-rw-r--r--   0        0        0      400 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/system_parameters/response.py
+-rw-r--r--   0        0        0      524 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/system_parameters/session.py
+-rw-r--r--   0        0        0      392 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/system_parameters/websocket.py
+-rw-r--r--   0        0        0      415 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/responses/__init__.py
+-rw-r--r--   0        0        0      839 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/responses/models/__init__.py
+-rw-r--r--   0        0        0     7921 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/responses/models/base.py
+-rw-r--r--   0        0        0       50 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/responses/models/exceptions.py
+-rw-r--r--   0        0        0     4305 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/responses/models/file.py
+-rw-r--r--   0        0        0      726 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/responses/models/helper.py
+-rw-r--r--   0        0        0     2129 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/responses/models/html.py
+-rw-r--r--   0        0        0     2935 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/responses/models/json.py
+-rw-r--r--   0        0        0     4865 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/responses/models/route.py
+-rw-r--r--   0        0        0     1688 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/responses/models/type_converter.py
+-rw-r--r--   0        0        0     1253 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/responses/response_types.py
+-rw-r--r--   0        0        0      357 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/serializer/__init__.py
+-rw-r--r--   0        0        0     5633 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/serializer/base.py
+-rw-r--r--   0        0        0      194 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/serializer/guard.py
+-rw-r--r--   0        0        0      454 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/shortcuts.py
+-rw-r--r--   0        0        0      613 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/templating/__init__.py
+-rw-r--r--   0        0        0      593 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/templating/environment.py
+-rw-r--r--   0        0        0     2020 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/templating/loader.py
+-rw-r--r--   0        0        0      835 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/templating/model.py
+-rw-r--r--   0        0        0     2584 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/templating/renderer.py
+-rw-r--r--   0        0        0      110 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/templating/schema.py
+-rw-r--r--   0        0        0      713 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/types.py
+-rw-r--r--   0        0        0      928 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/__init__.py
+-rw-r--r--   0        0        0      162 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/conf/__init__.py
+-rw-r--r--   0        0        0     5454 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/conf/app_settings_models.py
+-rw-r--r--   0        0        0     2397 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/conf/config.py
+-rw-r--r--   0        0        0     3270 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/conf/mixins.py
+-rw-r--r--   0        0        0      469 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/connection/__init__.py
+-rw-r--r--   0        0        0      855 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/connection/http.py
+-rw-r--r--   0        0        0      245 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/connection/websocket.py
+-rw-r--r--   0        0        0       97 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/exceptions/__init__.py
+-rw-r--r--   0        0        0     2157 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/exceptions/service.py
+-rw-r--r--   0        0        0      457 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/execution_context/__init__.py
+-rw-r--r--   0        0        0     1327 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/execution_context/execution.py
+-rw-r--r--   0        0        0     2581 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/execution_context/factory.py
+-rw-r--r--   0        0        0     2280 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/execution_context/host.py
+-rw-r--r--   0        0        0     2089 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/execution_context/http.py
+-rw-r--r--   0        0        0      801 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/execution_context/websocket.py
+-rw-r--r--   0        0        0       72 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/guards/__init__.py
+-rw-r--r--   0        0        0     1729 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/guards/consumer.py
+-rw-r--r--   0        0        0       87 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/interceptors/__init__.py
+-rw-r--r--   0        0        0     2202 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/interceptors/consumer.py
+-rw-r--r--   0        0        0     1050 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/middleware/__init__.py
+-rw-r--r--   0        0        0     2905 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/middleware/di.py
+-rw-r--r--   0        0        0     2689 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/middleware/exceptions.py
+-rw-r--r--   0        0        0     2577 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/middleware/function.py
+-rw-r--r--   0        0        0      917 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/middleware/middleware.py
+-rw-r--r--   0        0        0     1049 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/middleware/versioning.py
+-rw-r--r--   0        0        0      363 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/modules/__init__.py
+-rw-r--r--   0        0        0     1302 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/modules/base.py
+-rw-r--r--   0        0        0     3082 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/modules/builder.py
+-rw-r--r--   0        0        0     7921 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/modules/config.py
+-rw-r--r--   0        0        0      787 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/modules/helper.py
+-rw-r--r--   0        0        0     9438 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/modules/ref.py
+-rw-r--r--   0        0        0      291 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/router_builders/__init__.py
+-rw-r--r--   0        0        0     2094 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/router_builders/base.py
+-rw-r--r--   0        0        0     4821 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/router_builders/controller.py
+-rw-r--r--   0        0        0     1251 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/router_builders/module_router.py
+-rw-r--r--   0        0        0      963 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/__init__.py
+-rw-r--r--   0        0        0     5427 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/base.py
+-rw-r--r--   0        0        0      272 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/controller/__init__.py
+-rw-r--r--   0        0        0     1068 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/controller/base.py
+-rw-r--r--   0        0        0      852 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/controller/route.py
+-rw-r--r--   0        0        0      190 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/controller/websocket/__init__.py
+-rw-r--r--   0        0        0     1844 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/controller/websocket/handler.py
+-rw-r--r--   0        0        0     1564 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/controller/websocket/route.py
+-rw-r--r--   0        0        0     2566 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/file_mount.py
+-rw-r--r--   0        0        0     7056 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/mount.py
+-rw-r--r--   0        0        0     5321 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/route.py
+-rw-r--r--   0        0        0     3046 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/route_collections.py
+-rw-r--r--   0        0        0     2324 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/utils.py
+-rw-r--r--   0        0        0      161 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/websocket/__init__.py
+-rw-r--r--   0        0        0     6628 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/websocket/handler.py
+-rw-r--r--   0        0        0     5618 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/websocket/route.py
+-rw-r--r--   0        0        0        0 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/security/__init__.py
+-rw-r--r--   0        0        0     4074 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/security/hashers/__init__.py
+-rw-r--r--   0        0        0     1811 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/security/hashers/argon2.py
+-rw-r--r--   0        0        0     3002 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/security/hashers/base.py
+-rw-r--r--   0        0        0     1739 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/security/hashers/bcrypt.py
+-rw-r--r--   0        0        0     1418 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/security/hashers/md5.py
+-rw-r--r--   0        0        0     1282 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/security/hashers/pbkdf.py
+-rw-r--r--   0        0        0     2774 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/security/hashers/scrypt.py
+-rw-r--r--   0        0        0       82 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/services/__init__.py
+-rw-r--r--   0        0        0     1977 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/services/reflector.py
+-rw-r--r--   0        0        0      392 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/shortcuts.py
+-rw-r--r--   0        0        0     1805 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/staticfiles.py
+-rw-r--r--   0        0        0      673 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/versioning/__init__.py
+-rw-r--r--   0        0        0     2569 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/versioning/base.py
+-rw-r--r--   0        0        0     6176 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/versioning/resolver.py
+-rw-r--r--   0        0        0     1220 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/__init__.py
+-rw-r--r--   0        0        0      344 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/asgi_args.py
+-rw-r--r--   0        0        0     1120 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/constants.py
+-rw-r--r--   0        0        0        0 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/context.py
+-rw-r--r--   0        0        0      400 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/exceptions.py
+-rw-r--r--   0        0        0      117 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/injector/__init__.py
+-rw-r--r--   0        0        0     8754 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/injector/container.py
+-rw-r--r--   0        0        0     5912 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/injector/ellar_injector.py
+-rw-r--r--   0        0        0      154 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/logger.py
+-rw-r--r--   0        0        0     1001 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/providers.py
+-rw-r--r--   0        0        0     2050 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/scopes.py
+-rw-r--r--   0        0        0     5969 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/service_config.py
+-rw-r--r--   0        0        0       39 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/types.py
+-rw-r--r--   0        0        0      406 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/utils.py
+-rw-r--r--   0        0        0      231 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/events/__init__.py
+-rw-r--r--   0        0        0     1951 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/events/base.py
+-rw-r--r--   0        0        0      579 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/__init__.py
+-rw-r--r--   0        0        0    10854 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/builder.py
+-rw-r--r--   0        0        0      243 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/constants.py
+-rw-r--r--   0        0        0       94 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/decorators/__init__.py
+-rw-r--r--   0        0        0     1199 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/decorators/extra_info.py
+-rw-r--r--   0        0        0      731 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/decorators/tags.py
+-rw-r--r--   0        0        0      219 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/docs_ui/__init__.py
+-rw-r--r--   0        0        0     1138 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/docs_ui/base.py
+-rw-r--r--   0        0        0      932 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/docs_ui/redocs.py
+-rw-r--r--   0        0        0     2226 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/docs_ui/stoplight.py
+-rw-r--r--   0        0        0     1078 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/docs_ui/swagger.py
+-rw-r--r--   0        0        0     5497 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/module.py
+-rw-r--r--   0        0        0    13873 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/openapi_v3.py
+-rw-r--r--   0        0        0    16040 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/route_doc_models.py
+-rw-r--r--   0        0        0      115 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/schemas/__init__.py
+-rw-r--r--   0        0        0      348 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/schemas/validation.py
+-rw-r--r--   0        0        0    50277 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/static/swagger/SwaggerDark.css
+-rw-r--r--   0        0        0      702 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/templates/redocs.html
+-rw-r--r--   0        0        0      895 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/templates/swagger.html
+-rw-r--r--   0        0        0        0 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/py.typed
+-rw-r--r--   0        0        0     2082 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/pydantic/__init__.py
+-rw-r--r--   0        0        0     1528 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/pydantic/decorator.py
+-rw-r--r--   0        0        0      764 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/pydantic/emails.py
+-rw-r--r--   0        0        0     1798 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/pydantic/encoder.py
+-rw-r--r--   0        0        0     1718 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/pydantic/exceptions.py
+-rw-r--r--   0        0        0      692 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/pydantic/field_constraints.py
+-rw-r--r--   0        0        0     2850 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/pydantic/fields.py
+-rw-r--r--   0        0        0      397 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/pydantic/types.py
+-rw-r--r--   0        0        0     8596 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/pydantic/utils.py
+-rw-r--r--   0        0        0      105 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/reflect/__init__.py
+-rw-r--r--   0        0        0     5258 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/reflect/_reflect.py
+-rw-r--r--   0        0        0       34 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/reflect/constants.py
+-rw-r--r--   0        0        0       58 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/samples/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/samples/controllers/__init__.py
+-rw-r--r--   0        0        0      232 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/samples/controllers/guard.py
+-rw-r--r--   0        0        0      704 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/samples/controllers/home.py
+-rw-r--r--   0        0        0      211 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/samples/modules.py
+-rw-r--r--   0        0        0   232915 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/samples/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0      721 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/samples/static/css/cover.css
+-rwxr-xr-x   0        0        0    25915 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/samples/static/img/EllarLogoB.png
+-rwxr-xr-x   0        0        0    36744 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/samples/static/img/EllarLogoIconOnly.png
+-rwxr-xr-x   0        0        0     3888 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/samples/static/img/Icon.svg
+-rw-r--r--   0        0        0     2575 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/samples/templates/home/index.html
+-rw-r--r--   0        0        0      629 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/__init__.py
+-rw-r--r--   0        0        0      422 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/adapter.py
+-rw-r--r--   0        0        0      543 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/constants.py
+-rw-r--r--   0        0        0     1914 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/context.py
+-rw-r--r--   0        0        0      225 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/decorators/__init__.py
+-rw-r--r--   0        0        0      667 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/decorators/events.py
+-rw-r--r--   0        0        0     3034 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/decorators/gateway.py
+-rw-r--r--   0        0        0      570 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/decorators/subscribe_message.py
+-rw-r--r--   0        0        0     4177 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/factory.py
+-rw-r--r--   0        0        0     9619 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/gateway.py
+-rw-r--r--   0        0        0      144 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/model.py
+-rw-r--r--   0        0        0      532 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/responses.py
+-rw-r--r--   0        0        0      107 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/testing/__init__.py
+-rw-r--r--   0        0        0     1700 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/testing/module.py
+-rw-r--r--   0        0        0      129 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/testing/__init__.py
+-rw-r--r--   0        0        0     4656 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/testing/module.py
+-rw-r--r--   0        0        0     1236 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/testing/uvicorn_server.py
+-rw-r--r--   0        0        0       60 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/threading/__init__.py
+-rw-r--r--   0        0        0     8476 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/threading/sync_worker.py
+-rw-r--r--   0        0        0      664 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/threading/utils.py
+-rw-r--r--   0        0        0     2386 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/utils/__init__.py
+-rw-r--r--   0        0        0      870 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/utils/crypto.py
+-rw-r--r--   0        0        0      658 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/utils/enums.py
+-rw-r--r--   0        0        0      389 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/utils/event_loop.py
+-rw-r--r--   0        0        0     7692 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/utils/functional.py
+-rw-r--r--   0        0        0     3810 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/utils/importer.py
+-rw-r--r--   0        0        0      723 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/utils/module_loading.py
+-rw-r--r--   0        0        0     3363 2024-04-25 08:12:14.642263 ellar-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     9083 1970-01-01 00:00:00.000000 ellar-0.7.4/PKG-INFO
```

### Comparing `ellar-0.7.3/README.md` & `ellar-0.7.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -128,24 +128,24 @@
 Now we can test our API at [http://127.0.0.1:5000/docs](http://127.0.0.1:5000/docs#/)
 
 You can also try the [quick-project](https://python-ellar.github.io/ellar/quick-project/) setup to get a good idea of the library.
 
 
 ## **Project Status**
 
-Currently, Ellar is in beta version with the following status:
+Currently, Ellar is in **beta** version with the following status:
 
-- Documentation: 95% complete
-- Authentication and Authorization: In progress
+- Documentation: 98% complete
+- Authorization: In progress
 
 ## **Dependency Summary**
 
 Ellar has the following dependencies:
 
-- Python >= 3.7
+- Python >= 3.8
 - Starlette
 - Pydantic
 - Injector
 
 ## **Contributing**
 Contributions are Welcome! You can contribute in the following ways.
```

### Comparing `ellar-0.7.3/ellar/app/context.py` & `ellar-0.7.4/ellar/app/context.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/app/factory.py` & `ellar-0.7.4/ellar/app/factory.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/app/lifespan.py` & `ellar-0.7.4/ellar/app/lifespan.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/app/main.py` & `ellar-0.7.4/ellar/app/main.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/app/services.py` & `ellar-0.7.4/ellar/app/services.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/auth/__init__.py` & `ellar-0.7.4/ellar/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/auth/decorators.py` & `ellar-0.7.4/ellar/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/auth/guards/apikey.py` & `ellar-0.7.4/ellar/auth/guards/apikey.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/auth/guards/auth_required.py` & `ellar-0.7.4/ellar/auth/guards/auth_required.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/auth/handlers/__init__.py` & `ellar-0.7.4/ellar/auth/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/auth/handlers/api_key.py` & `ellar-0.7.4/ellar/auth/handlers/api_key.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/auth/handlers/mixin.py` & `ellar-0.7.4/ellar/auth/handlers/mixin.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/auth/handlers/model.py` & `ellar-0.7.4/ellar/auth/handlers/model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/auth/handlers/schemes/api_key.py` & `ellar-0.7.4/ellar/auth/handlers/schemes/api_key.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/auth/handlers/schemes/base.py` & `ellar-0.7.4/ellar/auth/handlers/schemes/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/auth/handlers/schemes/http.py` & `ellar-0.7.4/ellar/auth/handlers/schemes/http.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/auth/interceptor.py` & `ellar-0.7.4/ellar/auth/interceptor.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/auth/middleware/auth.py` & `ellar-0.7.4/ellar/auth/middleware/auth.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/auth/middleware/session.py` & `ellar-0.7.4/ellar/auth/middleware/session.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/auth/policy/base.py` & `ellar-0.7.4/ellar/auth/policy/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/auth/policy/common.py` & `ellar-0.7.4/ellar/auth/policy/common.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/auth/services/auth_schemes.py` & `ellar-0.7.4/ellar/auth/services/auth_schemes.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/auth/services/middleware.py` & `ellar-0.7.4/ellar/auth/services/middleware.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/auth/session/__init__.py` & `ellar-0.7.4/ellar/auth/session/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/auth/session/base.py` & `ellar-0.7.4/ellar/auth/session/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/auth/session/cookie_dict.py` & `ellar-0.7.4/ellar/auth/session/cookie_dict.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/auth/session/strategy.py` & `ellar-0.7.4/ellar/auth/session/strategy.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/cache/backends/_aio_cache.py.ellar` & `ellar-0.7.4/ellar/cache/backends/_aio_cache.py.ellar`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/cache/backends/base.py` & `ellar-0.7.4/ellar/cache/backends/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/cache/backends/local_cache.py` & `ellar-0.7.4/ellar/cache/backends/local_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/cache/backends/pylib_cache.py` & `ellar-0.7.4/ellar/cache/backends/pylib_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/cache/backends/pymem_cache.py` & `ellar-0.7.4/ellar/cache/backends/pymem_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/cache/backends/redis/backend.py` & `ellar-0.7.4/ellar/cache/backends/redis/backend.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/cache/backends/serializer.py` & `ellar-0.7.4/ellar/cache/backends/serializer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/cache/decorator.py` & `ellar-0.7.4/ellar/cache/decorator.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/cache/interface.py` & `ellar-0.7.4/ellar/cache/interface.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/cache/make_key_decorator.py` & `ellar-0.7.4/ellar/cache/make_key_decorator.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/cache/model.py` & `ellar-0.7.4/ellar/cache/model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/cache/module.py` & `ellar-0.7.4/ellar/cache/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/cache/schema.py` & `ellar-0.7.4/ellar/cache/schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/cache/service.py` & `ellar-0.7.4/ellar/cache/service.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/__init__.py` & `ellar-0.7.4/ellar/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/compatible/cache_properties.py` & `ellar-0.7.4/ellar/common/compatible/cache_properties.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/compatible/dict.py` & `ellar-0.7.4/ellar/common/compatible/dict.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/constants.py` & `ellar-0.7.4/ellar/common/constants.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/converters.py` & `ellar-0.7.4/ellar/common/converters.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/datastructures.py` & `ellar-0.7.4/ellar/common/datastructures.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/decorators/__init__.py` & `ellar-0.7.4/ellar/common/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/decorators/base.py` & `ellar-0.7.4/ellar/common/decorators/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/decorators/controller.py` & `ellar-0.7.4/ellar/common/decorators/controller.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/decorators/exception.py` & `ellar-0.7.4/ellar/common/decorators/exception.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/decorators/extra_args.py` & `ellar-0.7.4/ellar/common/decorators/extra_args.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/decorators/file.py` & `ellar-0.7.4/ellar/common/decorators/file.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/decorators/guards.py` & `ellar-0.7.4/ellar/common/decorators/guards.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/decorators/html.py` & `ellar-0.7.4/ellar/common/decorators/html.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/decorators/interceptor.py` & `ellar-0.7.4/ellar/common/decorators/interceptor.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/decorators/middleware.py` & `ellar-0.7.4/ellar/common/decorators/middleware.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/decorators/modules.py` & `ellar-0.7.4/ellar/common/decorators/modules.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import inspect
 import typing as t
-from functools import partial
 from pathlib import Path
 
 import click
 from ellar.common.compatible import AttributeDict
 from ellar.common.constants import MODULE_METADATA, MODULE_WATERMARK
 from ellar.common.exceptions import ImproperConfiguration
 from ellar.common.models import ControllerBase
 from ellar.common.operations import ModuleRouter
 from ellar.di import ProviderConfig, SingletonScope, injectable
 from ellar.reflect import reflect
 from ellar.utils.importer import get_main_directory_by_stack
 from starlette.routing import Host, Mount
 
+_ModuleClass = t.TypeVar("_ModuleClass", bound=t.Type)
+
 
 def _wrapper(
-    target: t.Type,
+    target: _ModuleClass,
     watermark_key: str,
     metadata_keys: t.List[str],
     name: str,
     kwargs: AttributeDict,
-) -> t.Type:
+) -> _ModuleClass:
     if reflect.get_metadata(watermark_key, target):
         raise ImproperConfiguration(f"{target} is already identified as a Module")
 
     if not isinstance(target, type):
         raise ImproperConfiguration(f"{name} is a class decorator - {target}")
 
     if not kwargs.base_directory:
@@ -45,15 +46,15 @@
     routers: t.Sequence[t.Union[ModuleRouter, Mount, Host]] = (),
     providers: t.Sequence[t.Union[t.Type, "ProviderConfig"]] = (),
     template_folder: t.Optional[str] = "templates",
     base_directory: t.Optional[t.Union[Path, str]] = None,
     static_folder: str = "static",
     modules: t.Sequence[t.Union[t.Type, t.Any]] = (),
     commands: t.Sequence[t.Union[click.Command, click.Group, t.Any]] = (),
-) -> t.Callable:
+) -> t.Callable[[_ModuleClass], _ModuleClass]:
     """
     ========= MODULE DECORATOR ==============
 
     Defines a class as Module
 
     :param name: Module name
 
@@ -84,14 +85,17 @@
         routers=list(routers),
         providers=list(providers),
         template_folder=template_folder,
         modules=list(modules),
         commands=list(commands),
     )
 
-    return partial(
-        _wrapper,
-        metadata_keys=MODULE_METADATA.keys,
-        watermark_key=MODULE_WATERMARK,
-        kwargs=kwargs,
-        name="Module",
-    )
+    def _decorator(klass: _ModuleClass) -> _ModuleClass:
+        return _wrapper(
+            target=klass,
+            metadata_keys=MODULE_METADATA.keys,
+            watermark_key=MODULE_WATERMARK,
+            kwargs=kwargs,
+            name="Module",
+        )
+
+    return _decorator
```

### Comparing `ellar-0.7.3/ellar/common/decorators/serializer.py` & `ellar-0.7.4/ellar/common/decorators/serializer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/exceptions/__init__.py` & `ellar-0.7.4/ellar/common/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/exceptions/api/base.py` & `ellar-0.7.4/ellar/common/exceptions/api/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/exceptions/api/exceptions_types.py` & `ellar-0.7.4/ellar/common/exceptions/api/exceptions_types.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/exceptions/callable_exceptions.py` & `ellar-0.7.4/ellar/common/exceptions/callable_exceptions.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/exceptions/handlers.py` & `ellar-0.7.4/ellar/common/exceptions/handlers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/exceptions/validation.py` & `ellar-0.7.4/ellar/common/exceptions/validation.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/interfaces/__init__.py` & `ellar-0.7.4/ellar/common/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/interfaces/context.py` & `ellar-0.7.4/ellar/common/interfaces/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from ellar.di import injectable, request_scope
 from starlette.requests import empty_send
 from starlette.responses import Response
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from ellar.app import App
     from ellar.common.models import ControllerBase, Identity
-    from ellar.common.routing import RouteOperationBase
     from ellar.core import HTTPConnection, Request, WebSocket
+    from ellar.core.routing import RouteOperationBase
     from ellar.di.injector import EllarInjector
 
 
 class IHTTPHostContext(ABC):
     @property
     @abstractmethod
     def has_response(self) -> bool:
```

### Comparing `ellar-0.7.3/ellar/common/interfaces/exceptions.py` & `ellar-0.7.4/ellar/common/interfaces/exceptions.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/interfaces/identity_schemes.py` & `ellar-0.7.4/ellar/common/interfaces/identity_schemes.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/interfaces/module.py` & `ellar-0.7.4/ellar/common/interfaces/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/interfaces/response_model.py` & `ellar-0.7.4/ellar/common/interfaces/response_model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/interfaces/templating.py` & `ellar-0.7.4/ellar/common/interfaces/templating.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/interfaces/versioning.py` & `ellar-0.7.4/ellar/common/interfaces/versioning.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/models/controller.py` & `ellar-0.7.4/ellar/common/models/controller.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/models/guard.py` & `ellar-0.7.4/ellar/common/models/guard.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/models/identity.py` & `ellar-0.7.4/ellar/common/models/identity.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/operations/__init__.py` & `ellar-0.7.4/ellar/common/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/operations/base.py` & `ellar-0.7.4/ellar/common/operations/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/operations/router.py` & `ellar-0.7.4/ellar/common/operations/router.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/operations/schema.py` & `ellar-0.7.4/ellar/common/operations/schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/params/__init__.py` & `ellar-0.7.4/ellar/common/params/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/params/args/base.py` & `ellar-0.7.4/ellar/common/params/args/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/params/args/extra_args.py` & `ellar-0.7.4/ellar/common/params/args/extra_args.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/params/args/factory.py` & `ellar-0.7.4/ellar/common/params/args/factory.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/params/args/request_model.py` & `ellar-0.7.4/ellar/common/params/args/request_model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/params/args/resolver_generators.py` & `ellar-0.7.4/ellar/common/params/args/resolver_generators.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/params/args/websocket_model.py` & `ellar-0.7.4/ellar/common/params/args/websocket_model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/params/decorators/__init__.py` & `ellar-0.7.4/ellar/common/params/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/params/decorators/inject.py` & `ellar-0.7.4/ellar/common/params/decorators/inject.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/params/decorators/models.py` & `ellar-0.7.4/ellar/common/params/decorators/models.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/params/params.py` & `ellar-0.7.4/ellar/common/params/params.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/params/resolvers/__init__.py` & `ellar-0.7.4/ellar/common/params/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/params/resolvers/base.py` & `ellar-0.7.4/ellar/common/params/resolvers/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/params/resolvers/bulk_parameter.py` & `ellar-0.7.4/ellar/common/params/resolvers/bulk_parameter.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/params/resolvers/parameter.py` & `ellar-0.7.4/ellar/common/params/resolvers/parameter.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/params/resolvers/system_parameters/__init__.py` & `ellar-0.7.4/ellar/common/params/resolvers/system_parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/params/resolvers/system_parameters/background.py` & `ellar-0.7.4/ellar/common/params/resolvers/system_parameters/background.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/params/resolvers/system_parameters/base.py` & `ellar-0.7.4/ellar/common/params/resolvers/system_parameters/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/params/resolvers/system_parameters/provider.py` & `ellar-0.7.4/ellar/common/params/resolvers/system_parameters/provider.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/params/resolvers/system_parameters/session.py` & `ellar-0.7.4/ellar/common/params/resolvers/system_parameters/session.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/responses/models/__init__.py` & `ellar-0.7.4/ellar/common/responses/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/responses/models/base.py` & `ellar-0.7.4/ellar/common/responses/models/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/responses/models/file.py` & `ellar-0.7.4/ellar/common/responses/models/file.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/responses/models/helper.py` & `ellar-0.7.4/ellar/common/responses/models/helper.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/responses/models/html.py` & `ellar-0.7.4/ellar/common/responses/models/html.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/responses/models/json.py` & `ellar-0.7.4/ellar/common/responses/models/json.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/responses/models/route.py` & `ellar-0.7.4/ellar/common/responses/models/route.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/responses/models/type_converter.py` & `ellar-0.7.4/ellar/common/responses/models/type_converter.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/responses/response_types.py` & `ellar-0.7.4/ellar/common/responses/response_types.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/serializer/base.py` & `ellar-0.7.4/ellar/common/serializer/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/templating/__init__.py` & `ellar-0.7.4/ellar/common/templating/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/templating/environment.py` & `ellar-0.7.4/ellar/common/templating/environment.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/templating/loader.py` & `ellar-0.7.4/ellar/common/templating/loader.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/templating/model.py` & `ellar-0.7.4/ellar/common/templating/model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/templating/renderer.py` & `ellar-0.7.4/ellar/common/templating/renderer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/common/types.py` & `ellar-0.7.4/ellar/common/types.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/__init__.py` & `ellar-0.7.4/ellar/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/conf/app_settings_models.py` & `ellar-0.7.4/ellar/core/conf/app_settings_models.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/conf/config.py` & `ellar-0.7.4/ellar/core/conf/config.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/conf/mixins.py` & `ellar-0.7.4/ellar/core/conf/mixins.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/connection/http.py` & `ellar-0.7.4/ellar/core/connection/http.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/exceptions/service.py` & `ellar-0.7.4/ellar/core/exceptions/service.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/execution_context/execution.py` & `ellar-0.7.4/ellar/core/execution_context/execution.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/execution_context/factory.py` & `ellar-0.7.4/ellar/core/execution_context/factory.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/execution_context/host.py` & `ellar-0.7.4/ellar/core/execution_context/host.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/execution_context/http.py` & `ellar-0.7.4/ellar/core/execution_context/http.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/execution_context/websocket.py` & `ellar-0.7.4/ellar/core/execution_context/websocket.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/guards/consumer.py` & `ellar-0.7.4/ellar/core/guards/consumer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/interceptors/consumer.py` & `ellar-0.7.4/ellar/core/interceptors/consumer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/middleware/__init__.py` & `ellar-0.7.4/ellar/core/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/middleware/di.py` & `ellar-0.7.4/ellar/core/middleware/di.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/middleware/exceptions.py` & `ellar-0.7.4/ellar/core/middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/middleware/function.py` & `ellar-0.7.4/ellar/core/middleware/function.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/middleware/middleware.py` & `ellar-0.7.4/ellar/core/middleware/middleware.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,8 +15,12 @@
         super().__init__(cls, **options)
         injectable()(self.cls)
         self.kwargs = build_init_kwargs(self.cls, self.kwargs)
 
     @t.no_type_check
     def __call__(self, app: ASGIApp, injector: EllarInjector) -> T:
         self.kwargs.update(app=app)
-        return injector.create_object(self.cls, additional_kwargs=self.kwargs)
+        try:
+            return injector.create_object(self.cls, additional_kwargs=self.kwargs)
+        except TypeError:  # pragma: no cover
+            # TODO: Fix future typing for lower python version.
+            return self.cls(**self.kwargs)
```

### Comparing `ellar-0.7.3/ellar/core/middleware/versioning.py` & `ellar-0.7.4/ellar/core/middleware/versioning.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/modules/base.py` & `ellar-0.7.4/ellar/core/modules/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/modules/builder.py` & `ellar-0.7.4/ellar/core/modules/builder.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/modules/config.py` & `ellar-0.7.4/ellar/core/modules/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import dataclasses
 import typing as t
 
+import click
 from ellar.common import ControllerBase, ModuleRouter
 from ellar.common.constants import MODULE_METADATA, MODULE_WATERMARK
 from ellar.common.exceptions import ImproperConfiguration
 from ellar.core.conf import Config
 from ellar.di import MODULE_REF_TYPES, Container, EllarInjector
 from ellar.reflect import reflect
 from ellar.utils.importer import import_from_string
@@ -30,34 +31,40 @@
     controllers: t.Sequence[t.Union[t.Type["ControllerBase"], t.Type]] = (
         dataclasses.field(default_factory=lambda: ())
     )
 
     routers: t.Sequence[t.Union[BaseRoute, ModuleRouter]] = dataclasses.field(
         default_factory=lambda: ()
     )
+
+    commands: t.Sequence[t.Union[click.Command, click.Group, t.Any]] = (
+        dataclasses.field(default_factory=lambda: ())
+    )
+
     _is_configured: bool = False
 
     def __post_init__(self) -> None:
         if not reflect.get_metadata(MODULE_WATERMARK, self.module):
             raise ImproperConfiguration(f"{self.module.__name__} is not a valid Module")
 
+        # # Commands needs to be registered so that
+        # if self.commands:
+        #     reflect.define_metadata(MODULE_METADATA.COMMANDS, self.commands, self.module)
+
     def apply_configuration(self) -> None:
         if self._is_configured:
             return
 
         kwargs = {
-            "controllers": list(self.controllers),
-            "routers": list(self.routers),
-            "providers": list(self.providers),
+            MODULE_METADATA.CONTROLLERS: list(self.controllers),
+            MODULE_METADATA.ROUTERS: list(self.routers),
+            MODULE_METADATA.PROVIDERS: list(self.providers),
+            MODULE_METADATA.COMMANDS: list(self.commands),
         }
-        for key in [
-            MODULE_METADATA.CONTROLLERS,
-            MODULE_METADATA.ROUTERS,
-            MODULE_METADATA.PROVIDERS,
-        ]:
+        for key in kwargs.keys():
             value = kwargs[key]
             if value:
                 reflect.delete_metadata(key, self.module)
                 reflect.define_metadata(key, value, self.module)
 
         self._is_configured = True
```

### Comparing `ellar-0.7.3/ellar/core/modules/helper.py` & `ellar-0.7.4/ellar/core/modules/helper.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/modules/ref.py` & `ellar-0.7.4/ellar/core/modules/ref.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/router_builders/base.py` & `ellar-0.7.4/ellar/core/router_builders/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/router_builders/controller.py` & `ellar-0.7.4/ellar/core/router_builders/controller.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/router_builders/module_router.py` & `ellar-0.7.4/ellar/core/router_builders/module_router.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/routing/__init__.py` & `ellar-0.7.4/ellar/core/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/routing/base.py` & `ellar-0.7.4/ellar/core/routing/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/routing/controller/base.py` & `ellar-0.7.4/ellar/core/routing/controller/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/routing/controller/route.py` & `ellar-0.7.4/ellar/core/routing/controller/route.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/routing/controller/websocket/handler.py` & `ellar-0.7.4/ellar/core/routing/controller/websocket/handler.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/routing/controller/websocket/route.py` & `ellar-0.7.4/ellar/core/routing/controller/websocket/route.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/routing/file_mount.py` & `ellar-0.7.4/ellar/core/routing/file_mount.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/routing/mount.py` & `ellar-0.7.4/ellar/core/routing/mount.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/routing/route.py` & `ellar-0.7.4/ellar/core/routing/route.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/routing/route_collections.py` & `ellar-0.7.4/ellar/core/routing/route_collections.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/routing/utils.py` & `ellar-0.7.4/ellar/core/routing/utils.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/routing/websocket/handler.py` & `ellar-0.7.4/ellar/core/routing/websocket/handler.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/routing/websocket/route.py` & `ellar-0.7.4/ellar/core/routing/websocket/route.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/security/hashers/__init__.py` & `ellar-0.7.4/ellar/core/security/hashers/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/security/hashers/argon2.py` & `ellar-0.7.4/ellar/core/security/hashers/argon2.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/security/hashers/base.py` & `ellar-0.7.4/ellar/core/security/hashers/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/security/hashers/bcrypt.py` & `ellar-0.7.4/ellar/core/security/hashers/bcrypt.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/security/hashers/md5.py` & `ellar-0.7.4/ellar/core/security/hashers/md5.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/security/hashers/pbkdf.py` & `ellar-0.7.4/ellar/core/security/hashers/pbkdf.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/security/hashers/scrypt.py` & `ellar-0.7.4/ellar/core/security/hashers/scrypt.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/services/reflector.py` & `ellar-0.7.4/ellar/core/services/reflector.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/staticfiles.py` & `ellar-0.7.4/ellar/core/staticfiles.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/versioning/__init__.py` & `ellar-0.7.4/ellar/core/versioning/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/versioning/base.py` & `ellar-0.7.4/ellar/core/versioning/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/core/versioning/resolver.py` & `ellar-0.7.4/ellar/core/versioning/resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     def raise_exception(self) -> None:
         raise NotAcceptable(
             self.invalid_version_message.format(parameter=self.header_parameter)
         )
 
     def resolve_version(self) -> str:
         message = email.message.Message()
-        message[self.header_parameter] = self.connection.headers.get(
+        message[self.header_parameter] = self.connection.headers.get(  # type: ignore[assignment]
             self.header_parameter
         )
         accept = dict(message.get_params(header=self.header_parameter))  # type: ignore[arg-type]
         version = accept.get(self.version_parameter, self.default_version)
         return str(version)
```

### Comparing `ellar-0.7.3/ellar/di/__init__.py` & `ellar-0.7.4/ellar/di/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     RequestScope,
     request_or_transient_scope,
     request_scope,
     singleton_scope,
     transient_scope,
 )
 from .service_config import (
+    InjectByTag,
     ProviderConfig,
     get_scope,
     has_binding,
     injectable,
     is_decorated_with_injectable,
 )
 
@@ -44,12 +45,13 @@
     "has_binding",
     "get_scope",
     "RequestScopeContext",
     "SCOPED_CONTEXT_VAR",
     "INJECTABLE_ATTRIBUTE",
     "AnnotationToValue",
     "MODULE_REF_TYPES",
+    "InjectByTag",
 ]
 
 
 def __dir__() -> t.List[str]:
     return sorted(__all__)  # pragma: no cover
```

### Comparing `ellar-0.7.3/ellar/di/constants.py` & `ellar-0.7.4/ellar/di/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 
 SCOPED_CONTEXT_VAR: contextvars.ContextVar[Optional[RequestScopeContext]] = (
     contextvars.ContextVar("SCOPED-CONTEXT-VAR")
 )
 SCOPED_CONTEXT_VAR.set(None)
 
 
+class Tag(str):
+    """Tag Placeholder Type"""
+
+
 class AnnotationToValue(type):
     keys: List[str]
 
     @no_type_check
     def __new__(mcls, name, bases, namespace):
         cls = super().__new__(mcls, name, bases, namespace)
         annotations = {}
```

### Comparing `ellar-0.7.3/ellar/di/injector/container.py` & `ellar-0.7.4/ellar/di/injector/container.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,21 +33,26 @@
 
 
 class Container(InjectorBinder):
     __slots__ = (
         "injector",
         "_auto_bind",
         "_bindings",
+        "_bindings_by_tag",
         "parent",
         "_aliases",
         "_exact_aliases",
     )
 
     injector: "EllarInjector"
 
+    def __init__(self, *args: t.Any, **kwargs: t.Any) -> None:
+        super().__init__(*args, **kwargs)
+        self._bindings_by_tag: t.Dict[str, t.Type[t.Any]] = {}
+
     @t.no_type_check
     def create_binding(
         self,
         interface: t.Type,
         to: t.Any = None,
         scope: t.Union[ScopeDecorator, t.Type[InjectorScope]] = None,
     ) -> Binding:
@@ -78,23 +83,38 @@
             ):
                 binding = self.create_binding(interface)
                 self._bindings[interface] = binding
                 return binding, self
 
         raise UnsatisfiedRequirement(None, interface)
 
-    def register_binding(self, interface: t.Type, binding: Binding) -> None:
+    def get_interface_by_tag(self, tag: str) -> t.Type[t.Any]:
+        interface = self._bindings_by_tag.get(tag)
+        if interface:
+            return interface
+        if isinstance(self.parent, Container):
+            return self.parent.get_interface_by_tag(tag)
+
+        raise UnsatisfiedRequirement(None, t.cast(t.Any, tag))
+
+    def register_binding(
+        self, interface: t.Type, binding: Binding, tag: t.Optional[str] = None
+    ) -> None:
         self._bindings[interface] = binding
 
+        if tag:
+            self._bindings_by_tag[tag] = interface
+
     @t.no_type_check
     def register(
         self,
         base_type: t.Type,
         concrete_type: t.Union[t.Type, t.Any] = None,
         scope: t.Union[t.Type[InjectorScope], ScopeDecorator] = None,
+        tag: t.Optional[str] = None,
     ) -> None:
         try:
             if concrete_type and isinstance(concrete_type, type):
                 assert issubclass(concrete_type, base_type), (
                     f"Cannot register {base_type.__name__} for abstract class "
                     f"{concrete_type.__name__}"
                 )
@@ -110,96 +130,106 @@
             _scope = get_scope(concrete_type) or TransientScope
         elif _scope is NOT_SET:
             _scope = get_scope(base_type) or TransientScope
 
         if isinstance(_scope, ScopeDecorator):
             _scope = _scope.scope
 
-        self.register_binding(base_type, Binding(base_type, provider, _scope))
+        self.register_binding(base_type, Binding(base_type, provider, _scope), tag=tag)
 
     def register_instance(
         self,
         instance: t.Any,
         concrete_type: t.Optional[t.Union[t.Type, Provider]] = None,
+        tag: t.Optional[str] = None,
     ) -> None:
         assert not isinstance(instance, type)
         _concrete_type = instance.__class__ if not concrete_type else concrete_type
-        self.register(_concrete_type, instance, scope=SingletonScope)
+        self.register(_concrete_type, instance, scope=SingletonScope, tag=tag)
 
     def register_singleton(
         self,
         base_type: t.Type,
         concrete_type: t.Union[t.Type, t.Any, Provider] = None,
+        tag: t.Optional[str] = None,
     ) -> None:
         """
 
         :param base_type:
         :param concrete_type:
         :return:
         """
         if not concrete_type:
-            self.register_exact_singleton(base_type)
-        self.register(base_type, concrete_type, scope=SingletonScope)
+            self.register_exact_singleton(base_type, tag=tag)
+        self.register(base_type, concrete_type, scope=SingletonScope, tag=tag)
 
     def register_transient(
         self,
         base_type: t.Type,
         concrete_type: t.Optional[t.Union[t.Type, Provider]] = None,
+        tag: t.Optional[str] = None,
     ) -> None:
         """
 
         :param base_type:
         :param concrete_type:
         :return:
         """
         if not concrete_type:
-            self.register_exact_transient(base_type)
-        self.register(base_type, concrete_type, scope=TransientScope)
+            self.register_exact_transient(base_type, tag=tag)
+        self.register(base_type, concrete_type, scope=TransientScope, tag=tag)
 
     def register_scoped(
         self,
         base_type: t.Type,
         concrete_type: t.Optional[t.Union[t.Type, Provider]] = None,
+        tag: t.Optional[str] = None,
     ) -> None:
         """
 
         :param base_type:
         :param concrete_type:
         :return:
         """
         if not concrete_type:
-            self.register_exact_scoped(base_type)
-        self.register(base_type, concrete_type, scope=RequestScope)
+            self.register_exact_scoped(base_type, tag=tag)
+        self.register(base_type, concrete_type, scope=RequestScope, tag=tag)
 
-    def register_exact_singleton(self, concrete_type: t.Type) -> None:
+    def register_exact_singleton(
+        self, concrete_type: t.Type, tag: t.Optional[str] = None
+    ) -> None:
         """
 
         :param concrete_type:
         :return:
         """
         assert not isabstract(concrete_type)
-        self.register(base_type=concrete_type, scope=SingletonScope)
+        self.register(base_type=concrete_type, scope=SingletonScope, tag=tag)
 
-    def register_exact_transient(self, concrete_type: t.Type) -> None:
+    def register_exact_transient(
+        self, concrete_type: t.Type, tag: t.Optional[str] = None
+    ) -> None:
         """
 
         :param concrete_type:
         :return:
         """
         assert not isabstract(concrete_type)
-        self.register(base_type=concrete_type, scope=TransientScope)
+        self.register(base_type=concrete_type, scope=TransientScope, tag=tag)
 
-    def register_exact_scoped(self, concrete_type: t.Type) -> None:
+    def register_exact_scoped(
+        self, concrete_type: t.Type, tag: t.Optional[str] = None
+    ) -> None:
         """
 
         :param concrete_type:
         :return:
         """
         assert not isabstract(concrete_type)
-        self.register(base_type=concrete_type, scope=RequestScope)
+        self.register(base_type=concrete_type, scope=RequestScope, tag=tag)
 
     @t.no_type_check
     def install(
         self,
         module: t.Union[t.Type["ModuleBase"], "ModuleBase"],
         **init_kwargs: t.Any,
     ) -> t.Union[InjectorModule, "ModuleBase"]:
@@ -240,15 +270,15 @@
         instance = t.cast(t.Union[t.Type["ModuleBase"], "ModuleBase"], module)
 
         if isinstance(instance, type) and issubclass(
             t.cast(type, instance), InjectorModule
         ):
             instance = t.cast(type, instance)(**init_kwargs)
         elif isinstance(instance, type):
-            return self.injector.get(t.cast(type, instance))
+            return self.injector.get(instance)
         elif not isinstance(instance, type) and not isinstance(
             instance, InjectorModule
         ):
             return instance
 
         instance(self)
         return instance
```

### Comparing `ellar-0.7.3/ellar/di/injector/ellar_injector.py` & `ellar-0.7.4/ellar/di/injector/ellar_injector.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,52 @@
+import sys
 import typing as t
 from collections import OrderedDict, defaultdict
 from contextlib import asynccontextmanager
 
+from ellar.di.constants import MODULE_REF_TYPES, SCOPED_CONTEXT_VAR, Tag
 from ellar.di.logger import log
 from injector import Injector, Scope, ScopeDecorator
+from typing_extensions import Annotated
 
 from ..asgi_args import RequestScopeContext
-from ..constants import MODULE_REF_TYPES, SCOPED_CONTEXT_VAR
 from ..providers import InstanceProvider, Provider
 from ..types import T
 from .container import Container
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from ellar.core.modules import (
         ModuleBase,
         ModuleRefBase,
         ModuleSetup,
         ModuleTemplateRef,
     )
 
 
+class _TagInfo(t.NamedTuple):
+    supertype: t.Type
+    tag: str
+
+
+def _tag_info_interface(type_: t.Any) -> t.Optional[_TagInfo]:
+    if (
+        sys.version_info < (3, 10)
+        and getattr(type_, "__qualname__", "") == "NewType.<locals>.new_type"
+        or sys.version_info >= (3, 10)
+        and type(type_).__module__ == "typing"
+        and type(type_).__name__ == "NewType"
+    ):
+        return _TagInfo(supertype=type_.__supertype__, tag=type_.__name__)
+
+    if isinstance(type_, (str, Tag)):
+        return _TagInfo(supertype=Tag, tag=str(type_))
+
+    return None
+
+
 class EllarInjector(Injector):
     __slots__ = (
         "_stack",
         "parent",
         "container",
         "_modules",
     )
@@ -32,15 +55,15 @@
         self,
         auto_bind: bool = True,
         parent: t.Optional["Injector"] = None,
     ) -> None:
         self._stack = ()
         self.parent = parent
         # Binder
-        self.container = Container(
+        self.container = self.binder = Container(
             self,
             auto_bind=auto_bind,
             parent=parent.binder if parent is not None else None,
         )
 
         # Bind some useful types
         self.container.register_instance(self, EllarInjector)
@@ -106,23 +129,27 @@
 
     def add_module(self, module_ref: t.Union["ModuleRefBase", "ModuleSetup"]) -> None:
         self._modules[module_ref.ref_type].update({module_ref.module: module_ref})
 
     @t.no_type_check
     def get(
         self,
-        interface: t.Type[T],
+        interface: t.Union[Annotated[t.Type[T], type], Annotated[str, type]],
         scope: t.Union[ScopeDecorator, t.Type[Scope]] = None,
     ) -> T:
+        data = _tag_info_interface(interface)
+        if data and data.supertype is Tag:
+            interface = self.container.get_interface_by_tag(data.tag)
+
         binding, binder = self.container.get_binding(interface)
         scope = binding.scope
 
         if isinstance(scope, ScopeDecorator):  # pragma: no cover
             scope = scope.scope
-        # Fetch the corresponding Scope instance from the Binder.
+        # Fetch the corresponding Scope instance from the Container.
         scope_binding, _ = binder.get_binding(scope)
         scope_instance = t.cast(Scope, scope_binding.provider.get(self))
 
         log.debug(
             f"{self._log_prefix}EllarInjector.get({interface}, scope={scope}) using {binding.provider}"
         )
```

### Comparing `ellar-0.7.3/ellar/di/providers.py` & `ellar-0.7.4/ellar/di/providers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/di/scopes.py` & `ellar-0.7.4/ellar/di/scopes.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/di/service_config.py` & `ellar-0.7.4/ellar/di/service_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,115 +1,137 @@
 import typing as t
 
+from ellar.di.constants import INJECTABLE_ATTRIBUTE, Tag
 from injector import (
+    CallableT,
     ConstructorOrClassT,
     Scope,
     ScopeDecorator,
     SingletonScope,
     inject,
 )
 from injector import (
     is_decorated_with_inject as injector_is_decorated_with_inject,
 )
 
-from .constants import INJECTABLE_ATTRIBUTE
 from .exceptions import DIImproperConfiguration
 from .types import T
 from .utils import fail_silently
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from .injector import Container
 
 __all__ = (
     "ProviderConfig",
     "injectable",
     "is_decorated_with_injectable",
     "get_scope",
     "has_binding",
+    "InjectByTag",
 )
 
 
 class ProviderConfig(t.Generic[T]):
-    __slots__ = ("base_type", "use_value", "use_class", "scope")
+    __slots__ = ("base_type", "use_value", "use_class", "scope", "tag")
 
     def __init__(
         self,
         base_type: t.Union[t.Type[T], t.Type],
         *,
         use_value: t.Optional[T] = None,
         use_class: t.Union[t.Type[T], t.Any] = None,
         scope: t.Optional[t.Union[t.Type[Scope], t.Any]] = None,
+        tag: t.Optional[str] = None,
     ):
         self.scope = scope or SingletonScope
         if use_value and use_class:
             raise DIImproperConfiguration(
                 "`use_class` and `use_value` can not be used at the same time."
             )
 
         self.base_type = base_type
         self.use_value = use_value
         self.use_class = use_class
+        self.tag = tag
 
     def register(self, container: "Container") -> None:
         scope = get_scope(self.base_type) or self.scope
         if self.use_class:
             scope = get_scope(self.use_class) or scope
             container.register(
-                base_type=self.base_type, concrete_type=self.use_class, scope=scope
+                base_type=self.base_type,
+                concrete_type=self.use_class,
+                scope=scope,
+                tag=self.tag,
             )
         elif self.use_value:
             container.register(
-                base_type=self.base_type, concrete_type=self.use_value, scope=scope
+                base_type=self.base_type,
+                concrete_type=self.use_value,
+                scope=scope,
+                tag=self.tag,
             )
         elif not isinstance(self.base_type, type):
             raise DIImproperConfiguration(
                 f"couldn't determine provider setup for {self.base_type}. "
                 f"Please use `ProviderConfig` or `register_services` function in a "
                 f"Module to configure the provider"
             )
         else:
-            container.register(base_type=self.base_type, scope=scope)
+            container.register(base_type=self.base_type, scope=scope, tag=self.tag)
 
 
-class _Injectable:
-    def __init__(
-        self, scope: t.Optional[t.Union[t.Type[Scope], ScopeDecorator]] = None
-    ) -> None:
-        self.scope = scope or SingletonScope
+@t.overload
+def injectable(
+    scope: t.Union[t.Type[Scope], ScopeDecorator, CallableT] = SingletonScope,
+) -> t.Union[CallableT, t.Callable[[t.Any], CallableT]]:  # pragma: no cover
+    pass
 
-    def __call__(self, func_or_class: ConstructorOrClassT) -> ConstructorOrClassT:
-        fail_silently(inject, constructor_or_class=func_or_class)
-        setattr(func_or_class, INJECTABLE_ATTRIBUTE, self.scope)
-        return func_or_class
+
+@t.overload
+def injectable(
+    scope: t.Union[t.Type[Scope], ScopeDecorator, t.Type[T]] = SingletonScope,
+) -> t.Union[t.Type[T], t.Callable[[t.Any], t.Type[T]]]:  # pragma: no cover
+    pass
 
 
 def injectable(
-    scope: t.Optional[t.Union[t.Type[Scope], ScopeDecorator, t.Type]] = SingletonScope,
-) -> t.Union[ConstructorOrClassT, t.Callable]:
+    scope: t.Union[t.Type[Scope], ScopeDecorator, ConstructorOrClassT] = SingletonScope,
+) -> t.Union[ConstructorOrClassT, t.Callable[[t.Any], ConstructorOrClassT]]:
     """Decorates a callable or Type with inject and Defines Type or callable scope injection scope
 
     Example use:
 
     >>> @injectable # default is 'singleton_scope'
     ... class InjectableType2:
     ...     def __init__(self):
     ...         pass
     >>>
     >>> @injectable(scope=request_scope)
     ... class InjectableType3:
     ...     def __init__(self):
     ...         pass
     """
-    if (
+
+    def _decorator(func_or_class: ConstructorOrClassT) -> ConstructorOrClassT:
+        fail_silently(inject, constructor_or_class=func_or_class)
+        setattr(func_or_class, INJECTABLE_ATTRIBUTE, scope)
+
+        return func_or_class
+
+    if not (
         isinstance(scope, ScopeDecorator)
         or isinstance(scope, type)
         and issubclass(scope, Scope)
     ):
-        return _Injectable(scope)
-    return _Injectable()(t.cast(ConstructorOrClassT, scope))
+        func_ = scope
+        scope = SingletonScope
+        return _decorator(func_)  # type: ignore[arg-type]
+
+    return _decorator
 
 
 def is_decorated_with_injectable(func_or_class: ConstructorOrClassT) -> bool:
     """See if given Type or Call is declared with a scope.
 
     Example use:
     >>> class NonInjectableType:
@@ -146,7 +168,39 @@
         t.Optional[t.Union[t.Type[Scope], ScopeDecorator]],
         getattr(
             func_or_class,
             INJECTABLE_ATTRIBUTE,
             getattr(func_or_class, "__scope__", None),
         ),
     )
+
+
+def InjectByTag(tag: str) -> t.Any:
+    """
+    Inject a provider/service by tag.
+
+    For example:
+
+    class A:
+        name = 'A'
+
+    class AnotherType:
+        name = 'AnotherType'
+
+    class SomeClass:
+        def __init__(self, a: InjectByTag('A'), b: AnotherType):
+            self.a = a
+            self.b = b
+
+    injector = EllarInjector()
+    injector.container.register_exact_scoped(A, tag='A')
+    injector.container.register_exact_scoped(AnotherType)
+    injector.container.register_exact_scoped(SomeClass)
+
+    instance = injector.get(SomeClass)
+    assert instance.a.name == 'A'
+    assert instance.b.name == 'AnotherType'
+
+    :param tag: Registered Provider/Service tag name
+    :return: typing.Any
+    """
+    return t.NewType(Tag(tag), Tag)
```

### Comparing `ellar-0.7.3/ellar/events/base.py` & `ellar-0.7.4/ellar/events/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/openapi/__init__.py` & `ellar-0.7.4/ellar/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/openapi/builder.py` & `ellar-0.7.4/ellar/openapi/builder.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/openapi/decorators/extra_info.py` & `ellar-0.7.4/ellar/openapi/decorators/extra_info.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/openapi/decorators/tags.py` & `ellar-0.7.4/ellar/openapi/decorators/tags.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/openapi/docs_ui/base.py` & `ellar-0.7.4/ellar/openapi/docs_ui/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/openapi/docs_ui/redocs.py` & `ellar-0.7.4/ellar/openapi/docs_ui/redocs.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/openapi/docs_ui/stoplight.py` & `ellar-0.7.4/ellar/openapi/docs_ui/stoplight.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/openapi/docs_ui/swagger.py` & `ellar-0.7.4/ellar/openapi/docs_ui/swagger.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/openapi/module.py` & `ellar-0.7.4/ellar/openapi/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,28 +107,28 @@
                     f"must be of type `IDocumentationUIContext`"
                 )
 
             docs_ui.template_context.setdefault("favicon_url", ICON_SVG_PATH)
             docs_ui.template_context.setdefault("openapi_url", openapi_url)
             cls._setup_document_manager(router=router, docs_ui=docs_ui)
 
-        module = Module(
+        module: t.Type = Module(
             template_folder="templates",
             providers=[],
             routers=(router,),
             base_directory=str(__BASE_DIR__),
         )(get_unique_type())
 
         module_ref = ModuleSetup(module).get_module_ref(
             app.config, app.injector.container
         )
         app.router.extend(module_ref.routes)  # type: ignore[union-attr]
         app.injector.add_module(module_ref)
 
-        return module  # type: ignore[no-any-return]
+        return module
 
     @classmethod
     def _setup_document_manager(
         cls,
         *,
         router: ModuleRouter,
         docs_ui: IDocumentationUI,
```

### Comparing `ellar-0.7.3/ellar/openapi/openapi_v3.py` & `ellar-0.7.4/ellar/openapi/openapi_v3.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/openapi/route_doc_models.py` & `ellar-0.7.4/ellar/openapi/route_doc_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,15 +278,15 @@
                 "schema": param_schema,
             }
             if field_info.description:
                 parameter["description"] = field_info.description
             if field_info.examples:  # pragma: no cover
                 parameter["examples"] = field_info.examples  # type:ignore[assignment]
             if field_info.deprecated:
-                parameter["deprecated"] = field_info.deprecated
+                parameter["deprecated"] = field_info.deprecated  # type:ignore[assignment]
             parameters.append(parameter)
         return parameters
 
     def get_openapi_operation_request_body(
         self,
         *,
         field_mapping: t.Dict[
```

### Comparing `ellar-0.7.3/ellar/openapi/static/swagger/SwaggerDark.css` & `ellar-0.7.4/ellar/openapi/static/swagger/SwaggerDark.css`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/openapi/templates/redocs.html` & `ellar-0.7.4/ellar/openapi/templates/redocs.html`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/openapi/templates/swagger.html` & `ellar-0.7.4/ellar/openapi/templates/swagger.html`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/pydantic/__init__.py` & `ellar-0.7.4/ellar/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/pydantic/decorator.py` & `ellar-0.7.4/ellar/pydantic/decorator.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/pydantic/emails.py` & `ellar-0.7.4/ellar/pydantic/emails.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/pydantic/encoder.py` & `ellar-0.7.4/ellar/pydantic/encoder.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/pydantic/exceptions.py` & `ellar-0.7.4/ellar/pydantic/exceptions.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/pydantic/field_constraints.py` & `ellar-0.7.4/ellar/pydantic/field_constraints.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/pydantic/fields.py` & `ellar-0.7.4/ellar/pydantic/fields.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/pydantic/utils.py` & `ellar-0.7.4/ellar/pydantic/utils.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/reflect/_reflect.py` & `ellar-0.7.4/ellar/reflect/_reflect.py`

 * *Files 6% similar despite different names*

```diff
@@ -127,29 +127,21 @@
         )
         for k, v in self._meta_data.items():
             _meta_data[k] = dict(v)
         return _meta_data
 
     @asynccontextmanager
     async def async_context(self) -> t.AsyncGenerator[None, None]:
-        cached_meta_data = self._meta_data
-        try:
-            self._meta_data = self._clone_meta_data()
-            yield
-        finally:
-            self._meta_data.clear()
-            self._meta_data = cached_meta_data
+        cached_meta_data = self._clone_meta_data()
+        yield
+        reflect._meta_data.clear()
+        reflect._meta_data = WeakKeyDictionary(dict=cached_meta_data)
 
     @contextmanager
-    def context(
-        self,
-    ) -> t.Generator:
-        cached_meta_data = self._meta_data
-        try:
-            self._meta_data = self._clone_meta_data()
-            yield
-        finally:
-            self._meta_data.clear()
-            self._meta_data = cached_meta_data
+    def context(self) -> t.Generator:
+        cached_meta_data = self._clone_meta_data()
+        yield
+        reflect._meta_data.clear()
+        reflect._meta_data = WeakKeyDictionary(dict=cached_meta_data)
 
 
 reflect = _Reflect()
```

### Comparing `ellar-0.7.3/ellar/samples/controllers/home.py` & `ellar-0.7.4/ellar/samples/controllers/home.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/samples/static/css/bootstrap.min.css` & `ellar-0.7.4/ellar/samples/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/samples/static/css/cover.css` & `ellar-0.7.4/ellar/samples/static/css/cover.css`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/samples/static/img/EllarLogoB.png` & `ellar-0.7.4/ellar/samples/static/img/EllarLogoB.png`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/samples/static/img/EllarLogoIconOnly.png` & `ellar-0.7.4/ellar/samples/static/img/EllarLogoIconOnly.png`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/samples/static/img/Icon.svg` & `ellar-0.7.4/ellar/samples/static/img/Icon.svg`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/samples/templates/home/index.html` & `ellar-0.7.4/ellar/samples/templates/home/index.html`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/socket_io/__init__.py` & `ellar-0.7.4/ellar/socket_io/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/socket_io/constants.py` & `ellar-0.7.4/ellar/socket_io/constants.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/socket_io/context.py` & `ellar-0.7.4/ellar/socket_io/context.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/socket_io/decorators/events.py` & `ellar-0.7.4/ellar/socket_io/decorators/events.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/socket_io/decorators/gateway.py` & `ellar-0.7.4/ellar/socket_io/decorators/gateway.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/socket_io/decorators/subscribe_message.py` & `ellar-0.7.4/ellar/socket_io/decorators/subscribe_message.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/socket_io/factory.py` & `ellar-0.7.4/ellar/socket_io/factory.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/socket_io/gateway.py` & `ellar-0.7.4/ellar/socket_io/gateway.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/socket_io/responses.py` & `ellar-0.7.4/ellar/socket_io/responses.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/socket_io/testing/module.py` & `ellar-0.7.4/ellar/socket_io/testing/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/testing/module.py` & `ellar-0.7.4/ellar/testing/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/testing/uvicorn_server.py` & `ellar-0.7.4/ellar/testing/uvicorn_server.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/threading/sync_worker.py` & `ellar-0.7.4/ellar/threading/sync_worker.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/threading/utils.py` & `ellar-0.7.4/ellar/threading/utils.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/utils/__init__.py` & `ellar-0.7.4/ellar/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/utils/crypto.py` & `ellar-0.7.4/ellar/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/utils/enums.py` & `ellar-0.7.4/ellar/utils/enums.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/utils/functional.py` & `ellar-0.7.4/ellar/utils/functional.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/utils/importer.py` & `ellar-0.7.4/ellar/utils/importer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/ellar/utils/module_loading.py` & `ellar-0.7.4/ellar/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.3/pyproject.toml` & `ellar-0.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     "Framework :: AsyncIO",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 
 dependencies = [
     "injector == 0.21.0",
-    "starlette == 0.37.1",
+    "starlette == 0.37.2",
     "pydantic >=2.5.1,<3.0.0",
     "typing-extensions>=4.8.0",
     "jinja2",
     "click >= 8.1.7",
     "passlib >= 1.7.4",
 ]
```

### Comparing `ellar-0.7.3/PKG-INFO` & `ellar-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellar
-Version: 0.7.3
+Version: 0.7.4
 Summary: Ellar - Python ASGI web framework for building fast, efficient, and scalable RESTful APIs and server-side applications.
 Author-email: Ezeudoh Tochukwu <tochukwu.ezeudoh@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: AsyncIO
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: injector == 0.21.0
-Requires-Dist: starlette == 0.37.1
+Requires-Dist: starlette == 0.37.2
 Requires-Dist: pydantic >=2.5.1,<3.0.0
 Requires-Dist: typing-extensions>=4.8.0
 Requires-Dist: jinja2
 Requires-Dist: click >= 8.1.7
 Requires-Dist: passlib >= 1.7.4
 Requires-Dist: python-multipart >=0.0.5,<0.0.10 ; extra == "all"
 Requires-Dist: itsdangerous >=1.1.0,<3.0.0 ; extra == "all"
@@ -176,24 +176,24 @@
 Now we can test our API at [http://127.0.0.1:5000/docs](http://127.0.0.1:5000/docs#/)
 
 You can also try the [quick-project](https://python-ellar.github.io/ellar/quick-project/) setup to get a good idea of the library.
 
 
 ## **Project Status**
 
-Currently, Ellar is in beta version with the following status:
+Currently, Ellar is in **beta** version with the following status:
 
-- Documentation: 95% complete
-- Authentication and Authorization: In progress
+- Documentation: 98% complete
+- Authorization: In progress
 
 ## **Dependency Summary**
 
 Ellar has the following dependencies:
 
-- Python >= 3.7
+- Python >= 3.8
 - Starlette
 - Pydantic
 - Injector
 
 ## **Contributing**
 Contributions are Welcome! You can contribute in the following ways.
```

