# Comparing `tmp/cfn_kafka_admin-0.6.0rc3.tar.gz` & `tmp/cfn_kafka_admin-0.6.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfn_kafka_admin-0.6.0rc3.tar", max compression
+gzip compressed data, was "cfn_kafka_admin-0.6.0rc4.tar", max compression
```

## Comparing `cfn_kafka_admin-0.6.0rc3.tar` & `cfn_kafka_admin-0.6.0rc4.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0    16725 2022-03-22 06:17:38.518532 cfn_kafka_admin-0.6.0rc3/LICENSE
--rw-r--r--   0        0        0     2314 2022-05-11 06:55:41.690789 cfn_kafka_admin-0.6.0rc3/README.rst
--rw-r--r--   0        0        0      225 2024-04-18 22:54:32.979021 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/__init__.py
--rw-r--r--   0        0        0    22377 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/cfn_kafka_admin.py
--rw-r--r--   0        0        0      652 2023-04-24 12:49:19.847982 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/cfn_resources_definitions/__init__.py
--rw-r--r--   0        0        0     1958 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/cfn_resources_definitions/custom.py
--rw-r--r--   0        0        0     1793 2023-04-24 12:49:19.847982 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/cfn_resources_definitions/resource.py
--rw-r--r--   0        0        0     1852 2023-04-24 12:49:19.848981 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/cli.py
--rw-r--r--   0        0        0     2949 2023-05-05 09:04:48.510208 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/common.py
--rw-r--r--   0        0        0     1012 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/kafka_resources/__init__.py
--rw-r--r--   0        0        0     4202 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/kafka_resources/acls.py
--rw-r--r--   0        0        0     1654 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/kafka_resources/topics/__init__.py
--rw-r--r--   0        0        0     3082 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/kafka_resources/topics/create.py
--rw-r--r--   0        0        0     1895 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/kafka_resources/topics/delete.py
--rw-r--r--   0        0        0     4711 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/kafka_resources/topics/update.py
--rw-r--r--   0        0        0      136 2024-04-17 21:17:54.966767 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/lambda_functions/__init__.py
--rw-r--r--   0        0        0     3764 2024-04-18 22:54:19.306229 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/lambda_functions/acls.py
--rw-r--r--   0        0        0     6408 2024-04-18 22:54:19.306229 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/lambda_functions/schemas.py
--rw-r--r--   0        0        0     7956 2024-04-18 22:54:19.306229 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/lambda_functions/topics.py
--rw-r--r--   0        0        0     2105 2024-04-18 22:54:19.306229 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/lambda_functions/utils.py
--rw-r--r--   0        0        0      118 2023-04-24 12:49:19.850982 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/models/__init__.py
--rw-r--r--   0        0        0    13210 2024-04-18 22:54:19.306229 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/models/admin.py
--rw-r--r--   0        0        0      118 2023-04-24 12:49:19.850982 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/specs/__init__.py
--rw-r--r--   0        0        0     2998 2024-04-18 22:54:33.235017 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/specs/aws-cfn-kafka-admin-provider-schema.json
--rw-r--r--   0        0        0     2446 2024-04-18 22:54:33.235017 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/specs/ews-kafka-acl.json
--rw-r--r--   0        0        0     2560 2024-04-18 22:54:33.235017 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/specs/ews-kafka-parameters.json
--rw-r--r--   0        0        0     2150 2024-04-18 22:54:33.235017 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/specs/ews-kafka-schema.json
--rw-r--r--   0        0        0     7182 2024-04-18 22:54:33.235017 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/specs/ews-kafka-topic.json
--rw-r--r--   0        0        0     2632 2024-04-18 22:59:23.114604 cfn_kafka_admin-0.6.0rc3/pyproject.toml
--rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 cfn_kafka_admin-0.6.0rc3/PKG-INFO
+-rw-r--r--   0        0        0       95 2022-03-22 06:17:38.518532 cfn_kafka_admin-0.6.0rc4/AUTHORS.rst
+-rw-r--r--   0        0        0    16725 2022-03-22 06:17:38.518532 cfn_kafka_admin-0.6.0rc4/LICENSE
+-rw-r--r--   0        0        0     2314 2022-05-11 06:55:41.690789 cfn_kafka_admin-0.6.0rc4/README.rst
+-rw-r--r--   0        0        0      225 2024-04-23 12:40:36.323066 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/__init__.py
+-rw-r--r--   0        0        0    22743 2024-04-23 12:35:25.975168 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/cfn_kafka_admin.py
+-rw-r--r--   0        0        0      652 2023-04-24 12:49:19.847982 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/cfn_resources_definitions/__init__.py
+-rw-r--r--   0        0        0     1958 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/cfn_resources_definitions/custom.py
+-rw-r--r--   0        0        0     1793 2023-04-24 12:49:19.847982 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/cfn_resources_definitions/resource.py
+-rw-r--r--   0        0        0     1852 2023-04-24 12:49:19.848981 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/cli.py
+-rw-r--r--   0        0        0     2949 2023-05-05 09:04:48.510208 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/common.py
+-rw-r--r--   0        0        0     1012 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/kafka_resources/__init__.py
+-rw-r--r--   0        0        0     4202 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/kafka_resources/acls.py
+-rw-r--r--   0        0        0     1654 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/kafka_resources/topics/__init__.py
+-rw-r--r--   0        0        0     3082 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/kafka_resources/topics/create.py
+-rw-r--r--   0        0        0     1895 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/kafka_resources/topics/delete.py
+-rw-r--r--   0        0        0     4711 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/kafka_resources/topics/update.py
+-rw-r--r--   0        0        0      136 2024-04-17 21:17:54.966767 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/lambda_functions/__init__.py
+-rw-r--r--   0        0        0     3764 2024-04-18 22:54:19.306229 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/lambda_functions/acls.py
+-rw-r--r--   0        0        0     6408 2024-04-18 22:54:19.306229 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/lambda_functions/schemas.py
+-rw-r--r--   0        0        0     7956 2024-04-18 22:54:19.306229 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/lambda_functions/topics.py
+-rw-r--r--   0        0        0     2105 2024-04-18 22:54:19.306229 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/lambda_functions/utils.py
+-rw-r--r--   0        0        0      118 2023-04-24 12:49:19.850982 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/models/__init__.py
+-rw-r--r--   0        0        0    13210 2024-04-23 12:35:48.032734 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/models/admin.py
+-rw-r--r--   0        0        0      118 2023-04-24 12:49:19.850982 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/specs/__init__.py
+-rw-r--r--   0        0        0     2998 2024-04-23 12:40:36.507062 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/specs/aws-cfn-kafka-admin-provider-schema.json
+-rw-r--r--   0        0        0     2446 2024-04-23 12:40:36.507062 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/specs/ews-kafka-acl.json
+-rw-r--r--   0        0        0     2560 2024-04-23 12:40:36.507062 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/specs/ews-kafka-parameters.json
+-rw-r--r--   0        0        0     2150 2024-04-23 12:40:36.507062 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/specs/ews-kafka-schema.json
+-rw-r--r--   0        0        0     7182 2024-04-23 12:40:36.507062 cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/specs/ews-kafka-topic.json
+-rw-r--r--   0        0        0     2652 2024-04-23 12:40:36.323066 cfn_kafka_admin-0.6.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     3682 1970-01-01 00:00:00.000000 cfn_kafka_admin-0.6.0rc4/PKG-INFO
```

### Comparing `cfn_kafka_admin-0.6.0rc3/LICENSE` & `cfn_kafka_admin-0.6.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc3/README.rst` & `cfn_kafka_admin-0.6.0rc4/README.rst`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/cfn_kafka_admin.py` & `cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/cfn_kafka_admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,38 +245,46 @@
     def set_globals(self):
         """
         Method to set the global new_settings
         """
         self.globals_config.update(
             {
                 "BootstrapServers": self.model.Globals.BootstrapServers.__root__,
-                "SASLUsername": self.model.Globals.SASLUsername.__root__
-                if self.model.Globals.SASLUsername
-                and self.model.Globals.SASLUsername.__root__
-                else Ref(AWS_NO_VALUE),
-                "SASLPassword": self.model.Globals.SASLPassword.__root__
-                if self.model.Globals.SASLPassword
-                and self.model.Globals.SASLPassword.__root__
-                else Ref(AWS_NO_VALUE),
-                "SASLMechanism": SASLMechanism[
-                    self.model.Globals.SASLMechanism.name
-                ].value
-                if self.model.Globals.SASLMechanism
-                and isinstance(self.model.Globals.SASLMechanism, SASLMechanism)
-                else self.model.Globals.SASLMechanism,
-                "SecurityProtocol": SecurityProtocol[
-                    self.model.Globals.SecurityProtocol.name
-                ].value
-                if self.model.Globals.SecurityProtocol
-                and isinstance(self.model.Globals.SecurityProtocol, SecurityProtocol)
-                else self.model.Globals.SecurityProtocol,
-                "ClientConfig": self.model.Globals.ClientConfig
-                if self.model.Globals.ClientConfig
-                and isinstance(self.model.Globals.ClientConfig, dict)
-                else Ref(AWS_NO_VALUE),
+                "SASLUsername": (
+                    self.model.Globals.SASLUsername.__root__
+                    if self.model.Globals.SASLUsername
+                    and self.model.Globals.SASLUsername.__root__
+                    else Ref(AWS_NO_VALUE)
+                ),
+                "SASLPassword": (
+                    self.model.Globals.SASLPassword.__root__
+                    if self.model.Globals.SASLPassword
+                    and self.model.Globals.SASLPassword.__root__
+                    else Ref(AWS_NO_VALUE)
+                ),
+                "SASLMechanism": (
+                    SASLMechanism[self.model.Globals.SASLMechanism.name].value
+                    if self.model.Globals.SASLMechanism
+                    and isinstance(self.model.Globals.SASLMechanism, SASLMechanism)
+                    else self.model.Globals.SASLMechanism
+                ),
+                "SecurityProtocol": (
+                    SecurityProtocol[self.model.Globals.SecurityProtocol.name].value
+                    if self.model.Globals.SecurityProtocol
+                    and isinstance(
+                        self.model.Globals.SecurityProtocol, SecurityProtocol
+                    )
+                    else self.model.Globals.SecurityProtocol
+                ),
+                "ClientConfig": (
+                    self.model.Globals.ClientConfig
+                    if self.model.Globals.ClientConfig
+                    and isinstance(self.model.Globals.ClientConfig, dict)
+                    else Ref(AWS_NO_VALUE)
+                ),
             }
         )
 
     def define_schema_definition_path(
         self, topic_name: str, subject_suffix: str, attribute: TopicSchemaDef
     ):
         file_name = None
@@ -326,20 +334,24 @@
             f"{topic_name}{SerializerDef[attribute.Serializer.name].value}{subject_suffix}Schema",
             DeletionPolicy=deletion_policy,
             SerializeAttribute=subject_suffix,
             Serializer=SerializerDef[attribute.Serializer.name].value,
             Definition=definition,
             Subject=Sub(f"${{{topic_name}.Name}}-{subject_suffix}"),
             RegistryUrl=registry_url,
-            RegistryUsername=registry_username
-            if isinstance(registry_username, Ref)
-            else registry_username.__root__,
-            RegistryPassword=registry_password
-            if isinstance(registry_password, Ref)
-            else registry_password.__root__,
+            RegistryUsername=(
+                registry_username
+                if isinstance(registry_username, Ref)
+                else registry_username.__root__
+            ),
+            RegistryPassword=(
+                registry_password
+                if isinstance(registry_password, Ref)
+                else registry_password.__root__
+            ),
             RegistryUserInfo=registry_userinfo.__root__,
             CompatibilityMode=CompatibilityMode[attribute.CompatibilityMode.name].value,
         )
         if schema_class is CTopicSchema:
             function_name = (
                 self.model
                 if self.model.Schemas.FunctionName.startswith("arn:aws")
@@ -459,17 +471,19 @@
         for topic in self.model.Topics.Topics:
             topic_cfg = topic.dict()
             if function_name:
                 topic_cfg.update({"ServiceToken": function_name})
             topic_cfg.update(self.globals_config)
             topic_cfg.update(
                 {
-                    "ReplicationFactor": self.model.Topics.ReplicationFactor.__root__
-                    if not topic.ReplicationFactor
-                    else topic.ReplicationFactor,
+                    "ReplicationFactor": (
+                        self.model.Topics.ReplicationFactor.__root__
+                        if not topic.ReplicationFactor
+                        else topic.ReplicationFactor
+                    ),
                 }
             )
             if keypresent("Settings", topic_cfg) and not keyisset(
                 "Settings", topic_cfg
             ):
                 del topic_cfg["Settings"]
             else:
```

### Comparing `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/cfn_resources_definitions/__init__.py` & `cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/cfn_resources_definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/cfn_resources_definitions/custom.py` & `cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/cfn_resources_definitions/custom.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/cfn_resources_definitions/resource.py` & `cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/cfn_resources_definitions/resource.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/cli.py` & `cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/cli.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/common.py` & `cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/common.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/kafka_resources/__init__.py` & `cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/kafka_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/kafka_resources/acls.py` & `cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/kafka_resources/acls.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/kafka_resources/topics/__init__.py` & `cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/kafka_resources/topics/__init__.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/kafka_resources/topics/create.py` & `cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/kafka_resources/topics/create.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/kafka_resources/topics/delete.py` & `cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/kafka_resources/topics/delete.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/kafka_resources/topics/update.py` & `cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/kafka_resources/topics/update.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/lambda_functions/acls.py` & `cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/lambda_functions/acls.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/lambda_functions/schemas.py` & `cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/lambda_functions/schemas.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/lambda_functions/topics.py` & `cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/lambda_functions/topics.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/lambda_functions/utils.py` & `cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/lambda_functions/utils.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/models/admin.py` & `cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/models/admin.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/specs/aws-cfn-kafka-admin-provider-schema.json` & `cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/specs/aws-cfn-kafka-admin-provider-schema.json`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/specs/ews-kafka-acl.json` & `cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/specs/ews-kafka-acl.json`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/specs/ews-kafka-parameters.json` & `cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/specs/ews-kafka-parameters.json`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/specs/ews-kafka-schema.json` & `cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/specs/ews-kafka-schema.json`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/specs/ews-kafka-topic.json` & `cfn_kafka_admin-0.6.0rc4/cfn_kafka_admin/specs/ews-kafka-topic.json`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc3/pyproject.toml` & `cfn_kafka_admin-0.6.0rc4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cfn_kafka_admin"
-version = "0.6.0-rc3"
+version = "0.6.0-rc4"
 description = "AWS CloudFormation Resources to manage Kafka"
 authors = ["John Mille <john@compose-x.io>"]
 classifiers = [
   "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
   "Natural Language :: English",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.10",
@@ -15,26 +15,27 @@
 license = "MPL-2.0"
 
 [tool.poetry.urls]
 "Source" = "https://github.com/compose-x/cfn-kafka-admin"
 "Bug Tracker" = "https://github.com/compose-x/cfn-kafka-admin/issues"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 compose-x-common = "^1.4"
 jsonschema = "^4.21"
 importlib-resources = "^6.0"
 PyYAML = "^6.0"
 troposphere = "^4.5.1"
 kafka-schema-registry-admin = "^0.5"
 datamodel-code-generator = { extras = ["http"], version = "^0.25" }
 aws-cfn-custom-resource-resolve-parser = "^0.3"
 cfn-resource-provider = "^1.0.7"
 retry2 = "^0.9.5"
 confluent-kafka = "^2.3"
+pydantic = "1.10.15"
 
 [tool.poetry.scripts]
 aws-cfn-kafka-admin-provider = "cfn_kafka_admin.cli:main"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.7,<25.0"
 isort = "^5.10"
@@ -62,15 +63,15 @@
 disable-timestamp = "true"
 
 
 [tool.tbump]
 github_url = "https://github.com/compose-x/cfn-kafka-admin"
 
 [tool.tbump.version]
-current = "0.6.0-rc3"
+current = "0.6.0-rc4"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `cfn_kafka_admin-0.6.0rc3/PKG-INFO` & `cfn_kafka_admin-0.6.0rc4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: cfn_kafka_admin
-Version: 0.6.0rc3
+Version: 0.6.0rc4
 Summary: AWS CloudFormation Resources to manage Kafka
 License: MPL-2.0
 Author: John Mille
 Author-email: john@compose-x.io
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: aws-cfn-custom-resource-resolve-parser (>=0.3,<0.4)
 Requires-Dist: cfn-resource-provider (>=1.0.7,<2.0.0)
 Requires-Dist: compose-x-common (>=1.4,<2.0)
 Requires-Dist: confluent-kafka (>=2.3,<3.0)
 Requires-Dist: datamodel-code-generator[http] (>=0.25,<0.26)
 Requires-Dist: importlib-resources (>=6.0,<7.0)
 Requires-Dist: jsonschema (>=4.21,<5.0)
 Requires-Dist: kafka-schema-registry-admin (>=0.5,<0.6)
+Requires-Dist: pydantic (==1.10.15)
 Requires-Dist: retry2 (>=0.9.5,<0.10.0)
 Requires-Dist: troposphere (>=4.5.1,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/compose-x/cfn-kafka-admin/issues
 Project-URL: Source, https://github.com/compose-x/cfn-kafka-admin
 Description-Content-Type: text/x-rst
 
 ===============
```

