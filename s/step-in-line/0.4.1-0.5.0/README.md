# Comparing `tmp/step_in_line-0.4.1.tar.gz` & `tmp/step_in_line-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "step_in_line-0.4.1.tar", max compression
+gzip compressed data, was "step_in_line-0.5.0.tar", max compression
```

## Comparing `step_in_line-0.4.1.tar` & `step_in_line-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2024-04-24 23:39:28.139051 step_in_line-0.4.1/LICENSE
--rw-r--r--   0        0        0     3591 2024-04-24 23:39:28.143051 step_in_line-0.4.1/README.md
--rw-r--r--   0        0        0      505 2024-04-24 23:39:43.530935 step_in_line-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 23:39:28.143051 step_in_line-0.4.1/step_in_line/__init__.py
--rw-r--r--   0        0        0     5160 2024-04-24 23:39:28.143051 step_in_line-0.4.1/step_in_line/pipeline.py
--rw-r--r--   0        0        0     4818 2024-04-24 23:39:28.143051 step_in_line-0.4.1/step_in_line/step.py
--rw-r--r--   0        0        0     1729 2024-04-24 23:39:28.143051 step_in_line-0.4.1/step_in_line/template_lambda.py
--rw-r--r--   0        0        0    13470 2024-04-24 23:39:28.143051 step_in_line-0.4.1/step_in_line/tf.py
--rw-r--r--   0        0        0     4256 1970-01-01 00:00:00.000000 step_in_line-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-25 00:43:45.400320 step_in_line-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5879 2024-04-25 00:43:45.400320 step_in_line-0.5.0/README.md
+-rw-r--r--   0        0        0      505 2024-04-25 00:44:00.884309 step_in_line-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-25 00:43:45.400320 step_in_line-0.5.0/step_in_line/__init__.py
+-rw-r--r--   0        0        0     5160 2024-04-25 00:43:45.404320 step_in_line-0.5.0/step_in_line/pipeline.py
+-rw-r--r--   0        0        0     4818 2024-04-25 00:43:45.404320 step_in_line-0.5.0/step_in_line/step.py
+-rw-r--r--   0        0        0     1729 2024-04-25 00:43:45.404320 step_in_line-0.5.0/step_in_line/template_lambda.py
+-rw-r--r--   0        0        0    14445 2024-04-25 00:43:45.404320 step_in_line-0.5.0/step_in_line/tf.py
+-rw-r--r--   0        0        0     6544 1970-01-01 00:00:00.000000 step_in_line-0.5.0/PKG-INFO
```

### Comparing `step_in_line-0.4.1/LICENSE` & `step_in_line-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `step_in_line-0.4.1/step_in_line/pipeline.py` & `step_in_line-0.5.0/step_in_line/pipeline.py`

 * *Files identical despite different names*

### Comparing `step_in_line-0.4.1/step_in_line/step.py` & `step_in_line-0.5.0/step_in_line/step.py`

 * *Files identical despite different names*

### Comparing `step_in_line-0.4.1/step_in_line/template_lambda.py` & `step_in_line-0.5.0/step_in_line/template_lambda.py`

 * *Files identical despite different names*

### Comparing `step_in_line-0.4.1/step_in_line/tf.py` & `step_in_line-0.5.0/step_in_line/tf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from constructs import Construct
 from cdktf import (
     App,
     TerraformStack,
     IResolvable,
 )
 from cdktf_cdktf_provider_aws.provider import AwsProvider
-
 from cdktf_cdktf_provider_aws import (
     data_aws_subnets,
     security_group,
     iam_role_policy_attachment,
     lambda_function,
     sfn_state_machine,
     iam_role,
     iam_policy,
     cloudwatch_event_rule,
     cloudwatch_event_target,
     cloudwatch_log_group,
 )
+from importlib import resources as impresources
 from .step import Step, step
 from .pipeline import Pipeline
 from typing import List, Union, Optional, Tuple
 import json
 import zipfile
 import pickle
 from pathlib import Path
@@ -97,23 +97,25 @@
     return zip_name, hash_sha256
 
 
 def generate_lambda_function(
     scope: Construct,
     name_prefix: str,
     step: Step,
+    template_file: str,
     subnet_ids: Optional[List[str]] = None,
     security_group_ids: Optional[List[str]] = None,
 ):
     """Creates Terraform resource for Lambda
 
     Args:
         scope
         name_prefix (str): Prefix for lambda name to ensure uniqueness.
         step (Step): Step to create Lambda from
+        template_file (str): Location of template file to populate.  Defaults to internal template, but a custom file can be provided.
         subnet_ids (list): Optional subnet IDs.  Required if VPC is specified.
         security_group_ids (list): Option security group IDs.  Required if VPC is specified.
     """
     role = {
         "Version": "2012-10-17",
         "Statement": [
             {
@@ -135,17 +137,16 @@
                 ],
                 "Resource": ["arn:aws:logs:*:*:*"],
             },
         ],
     }
 
     lambda_entry = "index"
-    lambda_filename, sha256_hash = package_lambda(
-        "step_in_line/template_lambda.py", step, lambda_entry
-    )
+
+    lambda_filename, sha256_hash = package_lambda(template_file, step, lambda_entry)
     lambda_handler = f"{lambda_entry}.lambda_handler"
 
     lambda_role = iam_role.IamRole(
         scope,
         f"{step.name}role",
         assume_role_policy=json.dumps(role),
         name_prefix=step.name,
@@ -340,26 +341,39 @@
     )
 
 
 class StepInLine(TerraformStack):
     def __init__(
         self,
         scope: Construct,
-        ns: str,
+        name: str,
         pipeline: Pipeline,
         region: str,
+        template_file: str = impresources.files(__package__) / "template_lambda.py",
         vpc_id: Optional[str] = None,
         subnet_filter: Optional[
             Union[IResolvable, List[data_aws_subnets.DataAwsSubnetsFilter]]
         ] = None,
         outbound_cidr: Optional[List[str]] = [
             "0.0.0.0/0",
         ],
     ):
-        super().__init__(scope, ns)
+        """Initialize a StepInLine terraform stack
+
+        Args:
+            scope (Construct)
+            name (str): Unique name for Stack resource
+            pipeline (Pipeline): The pipeline to instantiate in AWS
+            region (str): AWS Region
+            template_file (str): Location of template file to populate.  Defaults to internal template, but a custom file can be provided.
+            vpc_id (Optional[str]): If Lambda needs to be in a VPC, supply the VPC ID
+            subnet_filter: If vpc_id is needed, provide a filter to access the subnets
+            outbound_cidr: Optional[List[str]]: The CIDRs to allow Lambda to access.  Only required if VPC is needed.
+        """
+        super().__init__(scope, name)
 
         AwsProvider(self, "AWS", region=region)
 
         subnet_ids = None
         security_group_ids = None
         if vpc_id is not None:
             subnets = data_aws_subnets.DataAwsSubnets(
@@ -381,15 +395,15 @@
 
             subnet_ids = subnets.ids
             security_group_ids = [security_group_for_lambda.id]
 
         step_to_lambda_tf = {}
         for step in pipeline.get_steps():
             step_lambda = generate_lambda_function(
-                self, pipeline.name, step, subnet_ids, security_group_ids
+                self, pipeline.name, step, template_file, subnet_ids, security_group_ids
             )
             step_to_lambda_tf[step.name] = step_lambda.arn
 
         pipeline.set_generate_step_name(lambda s: step_to_lambda_tf[s.name])
         step_function = generate_step_function(
             self, pipeline, region, list(step_to_lambda_tf.values())
         )
```

