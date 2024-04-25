# Comparing `tmp/iam_actions-1.2.20240424.tar.gz` & `tmp/iam_actions-1.2.20240425.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240424.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240425.tar", max compression
```

## Comparing `iam_actions-1.2.20240424.tar` & `iam_actions-1.2.20240425.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-04-24 02:18:09.669309 iam_actions-1.2.20240424/LICENSE
--rw-r--r--   0        0        0     2302 2024-04-24 02:18:09.669309 iam_actions-1.2.20240424/README.md
--rw-r--r--   0        0        0      228 2024-04-24 02:18:09.669309 iam_actions-1.2.20240424/iam_actions/__init__.py
--rw-r--r--   0        0        0  4810963 2024-04-24 02:19:12.613362 iam_actions-1.2.20240424/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-04-24 02:18:09.669309 iam_actions-1.2.20240424/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-04-24 02:18:09.669309 iam_actions-1.2.20240424/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-04-24 02:18:09.669309 iam_actions-1.2.20240424/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-04-24 02:18:09.669309 iam_actions-1.2.20240424/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-04-24 02:18:09.669309 iam_actions-1.2.20240424/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-04-24 02:18:09.669309 iam_actions-1.2.20240424/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-04-24 02:18:09.669309 iam_actions-1.2.20240424/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-04-24 02:18:09.669309 iam_actions-1.2.20240424/iam_actions/generate/services.py
--rw-r--r--   0        0        0   625454 2024-04-24 02:19:12.613362 iam_actions-1.2.20240424/iam_actions/policies.json
--rw-r--r--   0        0        0   208315 2024-04-24 02:19:12.613362 iam_actions-1.2.20240424/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   606809 2024-04-24 02:19:12.613362 iam_actions-1.2.20240424/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-04-24 02:19:13.269362 iam_actions-1.2.20240424/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240424/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240424/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-25 02:46:09.757853 iam_actions-1.2.20240425/LICENSE
+-rw-r--r--   0        0        0     2302 2024-04-25 02:46:09.757853 iam_actions-1.2.20240425/README.md
+-rw-r--r--   0        0        0      228 2024-04-25 02:46:09.757853 iam_actions-1.2.20240425/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4811893 2024-04-25 02:47:12.682419 iam_actions-1.2.20240425/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-04-25 02:46:09.757853 iam_actions-1.2.20240425/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-04-25 02:46:09.757853 iam_actions-1.2.20240425/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-04-25 02:46:09.757853 iam_actions-1.2.20240425/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-04-25 02:46:09.757853 iam_actions-1.2.20240425/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-04-25 02:46:09.757853 iam_actions-1.2.20240425/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-04-25 02:46:09.757853 iam_actions-1.2.20240425/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-04-25 02:46:09.757853 iam_actions-1.2.20240425/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-04-25 02:46:09.757853 iam_actions-1.2.20240425/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   625607 2024-04-25 02:47:12.682419 iam_actions-1.2.20240425/iam_actions/policies.json
+-rw-r--r--   0        0        0   208315 2024-04-25 02:47:12.682419 iam_actions-1.2.20240425/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   606958 2024-04-25 02:47:12.682419 iam_actions-1.2.20240425/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-04-25 02:47:13.326425 iam_actions-1.2.20240425/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240425/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240425/PKG-INFO
```

### Comparing `iam_actions-1.2.20240424/LICENSE` & `iam_actions-1.2.20240425/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240424/README.md` & `iam_actions-1.2.20240425/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240424/iam_actions/actions.json` & `iam_actions-1.2.20240425/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999526380600551%*

 * *Differences: {"'gamelift'": "{'CreateContainerGroupDefinition': OrderedDict([('access_level', 'Undocumented'), "*

 * *               "('action', 'CreateContainerGroupDefinition'), ('condition_keys', []), "*

 * *               "('description', 'Not Documented by AWS'), ('orphan', False), ('resources', [])]), "*

 * *               "'DeleteContainerGroupDefinition': OrderedDict([('access_level', 'Undocumented'), "*

 * *               "('action', 'DeleteContainerGroupDefinition'), ('condition_keys', []), "*

 * *               "('description', 'Not  […]*

```diff
@@ -73013,14 +73013,22 @@
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create a new game build using files stored in an Amazon S3 bucket",
             "orphan": false,
             "resources": []
         },
+        "CreateContainerGroupDefinition": {
+            "access_level": "Undocumented",
+            "action": "CreateContainerGroupDefinition",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateFleet": {
             "access_level": "Write",
             "action": "CreateFleet",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -73160,14 +73168,22 @@
             "condition_keys": [],
             "description": "Grants permission to delete a game build",
             "orphan": false,
             "resources": [
                 "build"
             ]
         },
+        "DeleteContainerGroupDefinition": {
+            "access_level": "Undocumented",
+            "action": "DeleteContainerGroupDefinition",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteFleet": {
             "access_level": "Write",
             "action": "DeleteFleet",
             "condition_keys": [],
             "description": "Grants permission to delete an empty fleet",
             "orphan": false,
             "resources": [
@@ -73316,14 +73332,22 @@
             "condition_keys": [],
             "description": "Grants permission to retrieve general properties of the compute such as ARN, fleet details, SDK endpoints, and location",
             "orphan": false,
             "resources": [
                 "fleet"
             ]
         },
+        "DescribeContainerGroupDefinition": {
+            "access_level": "Undocumented",
+            "action": "DescribeContainerGroupDefinition",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeEC2InstanceLimits": {
             "access_level": "Read",
             "action": "DescribeEC2InstanceLimits",
             "condition_keys": [],
             "description": "Grants permission to retrieve the maximum allowed and current usage for EC2 instance types",
             "orphan": false,
             "resources": []
@@ -73612,14 +73636,22 @@
             "condition_keys": [],
             "description": "Grants permission to retrieve all compute resources in the current Region",
             "orphan": false,
             "resources": [
                 "fleet"
             ]
         },
+        "ListContainerGroupDefinitions": {
+            "access_level": "Undocumented",
+            "action": "ListContainerGroupDefinitions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListFleets": {
             "access_level": "List",
             "action": "ListFleets",
             "condition_keys": [],
             "description": "Grants permission to retrieve a list of fleet IDs for all fleets in the current Region",
             "orphan": false,
             "resources": []
```

### Comparing `iam_actions-1.2.20240424/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240425/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240424/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240425/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240424/iam_actions/generate/generate.py` & `iam_actions-1.2.20240425/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240424/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240425/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240424/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240425/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240424/iam_actions/generate/services.py` & `iam_actions-1.2.20240425/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240424/iam_actions/policies.json` & `iam_actions-1.2.20240425/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999996226870718%*

 * *Differences: {"'serviceMap'": "{'Amazon GameLift': {'Actions': {insert: [(4, 'CreateContainerGroupDefinition'), "*

 * *                 "(20, 'DeleteContainerGroupDefinition'), (37, "*

 * *                 "'DescribeContainerGroupDefinition'), (71, 'ListContainerGroupDefinitions')]}}}"}*

```diff
@@ -16018,14 +16018,15 @@
             "ARNFormat": "arn:aws:gamelift:${Region}:${Account}:${ResourceType}/${ResourceId}",
             "ARNRegex": "^arn:aws:gamelift:.+",
             "Actions": [
                 "AcceptMatch",
                 "ClaimGameServer",
                 "CreateAlias",
                 "CreateBuild",
+                "CreateContainerGroupDefinition",
                 "CreateFleet",
                 "CreateFleetLocations",
                 "CreateGameServerGroup",
                 "CreateGameSession",
                 "CreateGameSessionQueue",
                 "CreateLocation",
                 "CreateMatchmakingConfiguration",
@@ -16033,14 +16034,15 @@
                 "CreatePlayerSession",
                 "CreatePlayerSessions",
                 "CreateScript",
                 "CreateVpcPeeringAuthorization",
                 "CreateVpcPeeringConnection",
                 "DeleteAlias",
                 "DeleteBuild",
+                "DeleteContainerGroupDefinition",
                 "DeleteFleet",
                 "DeleteFleetLocations",
                 "DeleteGameServerGroup",
                 "DeleteGameSessionQueue",
                 "DeleteLocation",
                 "DeleteMatchmakingConfiguration",
                 "DeleteMatchmakingRuleSet",
@@ -16049,14 +16051,15 @@
                 "DeleteVpcPeeringAuthorization",
                 "DeleteVpcPeeringConnection",
                 "DeregisterCompute",
                 "DeregisterGameServer",
                 "DescribeAlias",
                 "DescribeBuild",
                 "DescribeCompute",
+                "DescribeContainerGroupDefinition",
                 "DescribeEC2InstanceLimits",
                 "DescribeFleetAttributes",
                 "DescribeFleetCapacity",
                 "DescribeFleetEvents",
                 "DescribeFleetLocationAttributes",
                 "DescribeFleetLocationCapacity",
                 "DescribeFleetLocationUtilization",
@@ -16082,14 +16085,15 @@
                 "GetComputeAccess",
                 "GetComputeAuthToken",
                 "GetGameSessionLogUrl",
                 "GetInstanceAccess",
                 "ListAliases",
                 "ListBuilds",
                 "ListCompute",
+                "ListContainerGroupDefinitions",
                 "ListFleets",
                 "ListGameServerGroups",
                 "ListGameServers",
                 "ListLocations",
                 "ListScripts",
                 "ListTagsForResource",
                 "PutScalingPolicy",
```

### Comparing `iam_actions-1.2.20240424/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240425/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240424/iam_actions/services.json` & `iam_actions-1.2.20240425/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999960531716712%*

 * *Differences: {"'gamelift'": "{'Actions': {insert: [(4, 'CreateContainerGroupDefinition'), (20, "*

 * *               "'DeleteContainerGroupDefinition'), (37, 'DescribeContainerGroupDefinition'), (71, "*

 * *               "'ListContainerGroupDefinitions')]}}"}*

```diff
@@ -10026,14 +10026,15 @@
             "^arn:aws:gamelift:.+"
         ],
         "Actions": [
             "AcceptMatch",
             "ClaimGameServer",
             "CreateAlias",
             "CreateBuild",
+            "CreateContainerGroupDefinition",
             "CreateFleet",
             "CreateFleetLocations",
             "CreateGameServerGroup",
             "CreateGameSession",
             "CreateGameSessionQueue",
             "CreateLocation",
             "CreateMatchmakingConfiguration",
@@ -10041,14 +10042,15 @@
             "CreatePlayerSession",
             "CreatePlayerSessions",
             "CreateScript",
             "CreateVpcPeeringAuthorization",
             "CreateVpcPeeringConnection",
             "DeleteAlias",
             "DeleteBuild",
+            "DeleteContainerGroupDefinition",
             "DeleteFleet",
             "DeleteFleetLocations",
             "DeleteGameServerGroup",
             "DeleteGameSessionQueue",
             "DeleteLocation",
             "DeleteMatchmakingConfiguration",
             "DeleteMatchmakingRuleSet",
@@ -10057,14 +10059,15 @@
             "DeleteVpcPeeringAuthorization",
             "DeleteVpcPeeringConnection",
             "DeregisterCompute",
             "DeregisterGameServer",
             "DescribeAlias",
             "DescribeBuild",
             "DescribeCompute",
+            "DescribeContainerGroupDefinition",
             "DescribeEC2InstanceLimits",
             "DescribeFleetAttributes",
             "DescribeFleetCapacity",
             "DescribeFleetEvents",
             "DescribeFleetLocationAttributes",
             "DescribeFleetLocationCapacity",
             "DescribeFleetLocationUtilization",
@@ -10090,14 +10093,15 @@
             "GetComputeAccess",
             "GetComputeAuthToken",
             "GetGameSessionLogUrl",
             "GetInstanceAccess",
             "ListAliases",
             "ListBuilds",
             "ListCompute",
+            "ListContainerGroupDefinitions",
             "ListFleets",
             "ListGameServerGroups",
             "ListGameServers",
             "ListLocations",
             "ListScripts",
             "ListTagsForResource",
             "PutScalingPolicy",
```

### Comparing `iam_actions-1.2.20240424/pyproject.toml` & `iam_actions-1.2.20240425/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240424"
+version = "1.2.20240425"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240424/setup.py` & `iam_actions-1.2.20240425/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240424',
+    'version': '1.2.20240425',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240424/PKG-INFO` & `iam_actions-1.2.20240425/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240424
+Version: 1.2.20240425
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

