# Comparing `tmp/step_in_line-0.5.1.tar.gz` & `tmp/step_in_line-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "step_in_line-0.5.1.tar", max compression
+gzip compressed data, was "step_in_line-0.6.0.tar", max compression
```

## Comparing `step_in_line-0.5.1.tar` & `step_in_line-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,14 @@
--rw-r--r--   0        0        0     1069 2024-04-25 00:54:58.430348 step_in_line-0.5.1/LICENSE
--rw-r--r--   0        0        0     5904 2024-04-25 00:54:58.430348 step_in_line-0.5.1/README.md
--rw-r--r--   0        0        0      505 2024-04-25 00:55:12.262416 step_in_line-0.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-25 00:54:58.430348 step_in_line-0.5.1/step_in_line/__init__.py
--rw-r--r--   0        0        0     5160 2024-04-25 00:54:58.430348 step_in_line-0.5.1/step_in_line/pipeline.py
--rw-r--r--   0        0        0     4818 2024-04-25 00:54:58.430348 step_in_line-0.5.1/step_in_line/step.py
--rw-r--r--   0        0        0     1729 2024-04-25 00:54:58.430348 step_in_line-0.5.1/step_in_line/template_lambda.py
--rw-r--r--   0        0        0    14445 2024-04-25 00:54:58.430348 step_in_line-0.5.1/step_in_line/tf.py
--rw-r--r--   0        0        0     6569 1970-01-01 00:00:00.000000 step_in_line-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-25 14:41:19.058361 step_in_line-0.6.0/LICENSE
+-rw-r--r--   0        0        0     6947 2024-04-25 14:41:19.058361 step_in_line-0.6.0/README.md
+-rw-r--r--   0        0        0      614 2024-04-25 14:41:34.626480 step_in_line-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-25 14:41:19.058361 step_in_line-0.6.0/step_in_line/__init__.py
+-rw-r--r--   0        0        0     5290 2024-04-25 14:41:19.058361 step_in_line-0.6.0/step_in_line/pipeline.py
+-rw-r--r--   0        0        0     5192 2024-04-25 14:41:19.058361 step_in_line-0.6.0/step_in_line/step.py
+-rw-r--r--   0        0        0      594 2024-04-25 14:41:19.062361 step_in_line-0.6.0/step_in_line/stepfunctions/README.md
+-rw-r--r--   0        0        0        0 2024-04-25 14:41:19.062361 step_in_line-0.6.0/step_in_line/stepfunctions/__init__.py
+-rw-r--r--   0        0        0     1215 2024-04-25 14:41:19.062361 step_in_line-0.6.0/step_in_line/stepfunctions/fields.py
+-rw-r--r--   0        0        0     9815 2024-04-25 14:41:19.062361 step_in_line-0.6.0/step_in_line/stepfunctions/inputs.py
+-rw-r--r--   0        0        0    28067 2024-04-25 14:41:19.062361 step_in_line-0.6.0/step_in_line/stepfunctions/steps.py
+-rw-r--r--   0        0        0     1695 2024-04-25 14:41:19.062361 step_in_line-0.6.0/step_in_line/template_lambda.py
+-rw-r--r--   0        0        0    16251 2024-04-25 14:41:19.062361 step_in_line-0.6.0/step_in_line/tf.py
+-rw-r--r--   0        0        0     7638 1970-01-01 00:00:00.000000 step_in_line-0.6.0/PKG-INFO
```

### Comparing `step_in_line-0.5.1/LICENSE` & `step_in_line-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `step_in_line-0.5.1/README.md` & `step_in_line-0.6.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,47 @@
 ## Step-in-line
 
-Step functions are awesome.  It is a fully managed serverless AWS offering, so there is no upkeep or maintenance required.  Unfortunately, programatically created workflows of Lambda functions requires creating complex JSON definitions.  This library generates these JSON definitions automatically from Python decorators.  In addition, it generates the Lambda functions for each Python function.  
+[AWS Step Functions](https://aws.amazon.com/step-functions/) is awesome.  It is a fully managed serverless AWS offering, so there is no upkeep or maintenance required.  Unfortunately, programatically created workflows of Lambda functions using Terraform requires creating complex JSON definitions.  `step-in-line` generates these JSON definitions automatically from Python decorators.  In addition, it generates the Terraform files needed for deploying Step Functions, Lambdas, and EventBridge events.    
 
 The API is intentionally similar to the Sagemaker Pipeline API.  
 
 ## Usage
 
 ### Install
-`pip install step-in-line`
+
+Full install (recommended):
+
+`pip install step-in-line[terraform]`
+
+Don't include Terraform related dependencies:
+
+`pip install step-in-line`.
 
 ### Example Pipeline
 ```python
-from cdktf import App
+
 from step_in_line.step import step
 from step_in_line.pipeline import Pipeline
 from step_in_line.tf import StepInLine, rename_tf_output
 from pathlib import Path
 
-app = App(hcl_output=True)
+lambda_iam_policy = "" # put an IAM policy here, formatted as JSON
 
-# function names must be unique, or you can pass a name to the step to 
-# ensure uniqueness
 @step(
+    # function names must be unique, or you can pass a name to the step to 
+    # ensure uniqueness
     name = "preprocess_unique",
     python_runtime = "python3.9", # defaults to 3.10
     memory_size = 128, # defaults to 512
-    layers = ["arn:aws:lambda:us-east-2:123456789012:layer:example-layer"]
+    layers = ["arn:aws:lambda:us-east-2:123456789012:layer:example-layer"],
+    # be default, Lambda will only get bare permissions; to 
+    # interact with additional AWS Services, need to provide 
+    # IAM policies here.  They will automatically get attached 
+    # to the Lambda Role.  
+    policies = [lambda_iam_policy] 
 )
 def preprocess(arg1: str) -> str:
     # do stuff here, eg run some sql code against snowflake.  
     # Make sure to "import snowflake" within this function.  
     # Will need a "layer" passed which contains the snowflake
     # dependencies.  Must run in <15 minutes.
     return "hello"
@@ -70,20 +82,26 @@
 # "schedule" is optional, and can be cron or rate based
 pipe = Pipeline("mytest", steps=[step_train_result], schedule="rate(2 minutes)")
 
 # to run locally
 print(pipe.local_run()) # will print output of each step
 
 # to extract the step function definition
-print(pipe.generate_step_functions().to_json())
+print(pipe.generate_step_functions())
+
+# to extract the step function definition as a string
+import json
+print(json.dumps(pipe.generate_step_functions()))
 
 # generate terraform json including step function code and lambdas
+# Optionally installed with `pip install step-in-line[terraform]`
+from cdktf import App
+app = App(hcl_output=True)
 instance_name = "aws_instance"
 stack = StepInLine(app, instance_name, pipe, "us-east-1")
-
 # write the terraform json for use by `terraform apply`
 tf_path = Path(app.outdir, "stacks", instance_name)
 app.synth()
 # Terraform Python SDK does not add ".json" extension; this function
 # renames the generated Terraform file and copies it to the project root.
 rename_tf_output(tf_path)
 
@@ -123,21 +141,18 @@
             if "Payload" in ev:
                 payload = {**payload, **ev["Payload"]}
     return payload
 
 
 # Retrieve transform job name from event and return transform job status.
 def lambda_handler(event, context):
-    print(event)
-
+    
     with open("args.pickle", "rb") as f:
         args = pickle.load(f)
-
-    print(args)
-
+    
     with open("name.pickle", "rb") as f:
         name = pickle.load(f)
 
     arg_values = []
     payload = combine_payload(event)
     for arg in args:
         if arg in payload:
@@ -161,10 +176,18 @@
 
 ```python
 stack = StepInLine(app, instance_name, pipe, "us-east-1", template_file="/path/to/your/custom/template.py")
 ```
 
 The `"{{PUT_FUNCTION_HERE}}"` and `"{{PUT_FUNCTION_NAME_HERE}}"` will automatically be replaced by the code of your function defined inside the `@step` decorator and the name of the function, respectively.  
 
+### Limitations
+
+Only Lambda steps are supported.  For other types of steps, including Sagemaker jobs, [Sagemaker Pipelines](https://docs.aws.amazon.com/sagemaker/latest/dg/pipelines-step-decorator-create-pipeline.html) are likely a better option.
+
+All limitations of Lambdas apply.  Each step can only run for 15 minutes before timing out.
+
+
+
 ## API Docs
 
 https://danielhstahl.github.io/step-in-line/index.html
```

### Comparing `step_in_line-0.5.1/step_in_line/pipeline.py` & `step_in_line-0.6.0/step_in_line/pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-"""The Pipeline entity for workflow."""
-
-from __future__ import absolute_import
-
 import logging
 from typing import Sequence, Optional, List, Callable, Any, Tuple
 import networkx as nx
 from .step import Step
-from stepfunctions.steps import LambdaStep, Chain, Retry, Parallel, Graph
-from stepfunctions.workflow import Workflow
+from .stepfunctions.steps import LambdaStep, Chain, Retry, Parallel, Graph
 
 logger = logging.getLogger(__name__)
 
 
 def crawl_back(graph: nx.DiGraph, step: Step):
     """Create the Graph of Steps
 
@@ -45,14 +40,15 @@
             Retry(
                 error_equals=["States.TaskFailed"],
                 interval_seconds=15,
                 max_attempts=step.retry_count,
                 backoff_rate=4.0,
             )
         )
+    logger.debug(f"Converted {step.name} to Lambda")
     return lambda_state
 
 
 def _default_lambda_name(s: Step) -> str:
     return "${aws_lambda_function." + s.name + "lambda.arn}"
 
 
@@ -96,51 +92,55 @@
         """
         Create indexed sets of steps.
         This allows steps to be run in parallel,
         if they don't depend on each other
         """
         return list(nx.topological_generations(self.graph))
 
-    def generate_step_functions(self) -> Graph:
-        """Create Step Function dictionary"""
+    def generate_step_functions(self) -> dict:
+        """Create Step Function workflow definition"""
         dag_lambda = []
         for index, layer in enumerate(self.generate_layers()):
             if len(layer) == 1:
                 dag_lambda.append(
                     convert_step_to_lambda(layer[0], self.generate_step_name)
                 )
             else:
                 parallel_state = Parallel(f"parallel at {index}")
                 for step in layer:
                     parallel_state.add_branch(
                         convert_step_to_lambda(step, self.generate_step_name)
                     )
                 dag_lambda.append(parallel_state)
         chain = Chain(dag_lambda)
-        workflow = Workflow(name=self.name, definition=chain, role="doesnotmatter")
-        return workflow.definition
+        workflow = Graph(
+            chain
+        )  # Workflow(name=self.name, definition=chain, role="doesnotmatter")
+        logger.debug(f"Converted {self.name} to step function Workflow")
+        return workflow.to_dict()
 
     def set_generate_step_name(self, generate_step_name: Callable[[Step], str]):
         self.generate_step_name = generate_step_name
 
     def local_run(self) -> List[List[Tuple[str, Any]]]:
         """
         Runs pipeline locally, with no AWS dependency.
         Returns all intermediary outputs.
         """
         outputs = {}  # contains all intermediary output
         output_arr = (
             []
-        )  # constains all intermediary output, in the shape of the steps given by the topological generations
+        )  # contains all intermediary output, in the shape of the steps given by the topological generations
         for layer in self.generate_layers():
             layer_output = []
             for step in layer:
                 args = []
                 for arg in step.args:
                     if isinstance(arg, Step):
                         args.append(outputs[arg.name])
                     else:
                         args.append(arg)
                 outputs[step.name] = step.func(*args)
+                logger.debug(f"Output from step {step.name}: {outputs[step.name]}")
                 layer_output.append((step.name, outputs[step.name]))
             output_arr.append(layer_output)
         return output_arr
```

### Comparing `step_in_line-0.5.1/step_in_line/step.py` & `step_in_line-0.6.0/step_in_line/step.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-from __future__ import absolute_import
-
 from typing import List, Optional, Callable, Any, Dict
-
 from functools import wraps
 
 
 class Step:
     """`Step` for step function workflows"""
 
     def __init__(
@@ -13,41 +10,46 @@
         name: str,
         func: Callable,
         args: List[Any],
         python_runtime: str,
         memory_size: int = 512,
         description: Optional[str] = None,
         retry_count: int = 0,
+        policies: List[str] = [],
         layers: List[str] = [],
         env_variables: Dict[str, str] = {},  # to pass in to lambda
         depends_on: Optional[List["Step"]] = None,
     ):
         """Initialize a Step
 
         Args:
             name (str): The name of the `Step`.
             func (callable): The function that should be executed as part of this step
             args (list): The arguments to the function.  If not a step, these are considered "static" and are used even in the Step Function execution
             python_runtime (str): Lambda runtime.
             memory_size (int): Megabytes of memory for the lambda.  Defaults to 512.
             description (str): The description of the `Step`.
             retry_count (int): Number of times to retry a failure
+            policies (List[str]): IAM policies, in JSON, to provide to the Lambda
             layers (list): the ARNs of layers to add to the lambda function
             env_variables (dict): environment variables to pass to lambda function
             depends_on (List[Step]): The list of Steps that the current `Step` depends on.
         """
         self.name = name
         self.description = description
         self.retry_count = retry_count
         self.layers = layers
         self.func = func
         self.args = args
         self.memory_size = memory_size
         self.python_runtime = python_runtime
         self.env_variables = env_variables
+        self.additional_policies = (
+            policies  # by default, Lambda gets minimal permission
+        )
         if depends_on is not None:
             self._depends_on = depends_on
         else:
             self._depends_on = None
 
     @property
     def depends_on(
@@ -82,14 +84,15 @@
     _func=None,
     *,
     name: Optional[str] = None,
     description: Optional[str] = None,
     layers: Optional[List[str]] = None,
     python_runtime: str = "python3.10",
     memory_size: int = 512,
+    policies: List[str] = [],
     retry_count: int = 0,
     env_variables: Dict[str, str] = {}
 ):
     """Decorator for converting a python function to a pipeline step.
 
     This decorator wraps the annotated code into a `Step` object which can then be passed
     to a pipeline as a step.
@@ -97,28 +100,30 @@
     Args:
         _func: A Python function to run as a SageMaker pipeline step.
         name (str): Name of the pipeline step. Defaults to a generated name using function name and uuid4 identifier to avoid duplicates.
         description (str): Description of the step
         layers (list): Lambda layers
         python_runtime (str): Lambda runtime.
         memory_size (int): Megabytes of memory for the lambda.  Defaults to 512.
+        policies (List[str]): IAM policies, in JSON, to provide to the Lambda
         retry_count (int): number of retries to attempt.  Defaults to 0 (no retries).
         env_variables (dict): environment variables to pass to lambda function
 
     """
 
     def _step(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             depends_on = {}
             arg_list = []
             for arg in list(args) + list(kwargs.values()):
                 if isinstance(arg, Step):
                     depends_on[id(arg)] = arg
                 arg_list.append(arg)
+
             # setup default values for name, display_name and description if not provided
 
             _name = func.__name__ if not name else name
 
             _description = description
             if not _description:
                 _description = (
@@ -126,14 +131,16 @@
                 )
             return Step(
                 name=_name,
                 depends_on=list(depends_on.values()),
                 retry_count=retry_count,
                 layers=layers,
                 python_runtime=python_runtime,
+                memory_size=memory_size,
+                policies=policies,
                 func=func,
                 args=arg_list,
                 env_variables=env_variables,
             )
 
         return wrapper
```

### Comparing `step_in_line-0.5.1/step_in_line/template_lambda.py` & `step_in_line-0.6.0/step_in_line/template_lambda.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,21 +20,18 @@
             if "Payload" in ev:
                 payload = {**payload, **ev["Payload"]}
     return payload
 
 
 # Retrieve transform job name from event and return transform job status.
 def lambda_handler(event, context):
-    print(event)
 
     with open("args.pickle", "rb") as f:
         args = pickle.load(f)
 
-    print(args)
-
     with open("name.pickle", "rb") as f:
         name = pickle.load(f)
 
     arg_values = []
     payload = combine_payload(event)
     for arg in args:
         if arg in payload:
```

### Comparing `step_in_line-0.5.1/step_in_line/tf.py` & `step_in_line-0.6.0/step_in_line/tf.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 from constructs import Construct
-from cdktf import (
-    App,
-    TerraformStack,
-    IResolvable,
-)
+from cdktf import App, TerraformStack, IResolvable, TerraformOutput
 from cdktf_cdktf_provider_aws.provider import AwsProvider
 from cdktf_cdktf_provider_aws import (
     data_aws_subnets,
     security_group,
     iam_role_policy_attachment,
     lambda_function,
     sfn_state_machine,
@@ -24,40 +20,44 @@
 import json
 import zipfile
 import pickle
 from pathlib import Path
 import inspect
 import textwrap
 from hashlib import sha256
+import logging
+import os
+
+logger = logging.getLogger(__name__)
 
 
 def remove_decorators(src: str) -> str:
     """Removes any decorators from source code and
             truncates code so that there is no space
             in front of function definition
 
     Args:
         src (str): Source code for lambda
     """
     lines = []
     for line in src.splitlines():
         if not line.lstrip().startswith("@"):
             lines.append(line)
-
     return textwrap.dedent("\n".join(lines))
 
 
 def get_python_code(python_template_path: str, step: Step) -> str:
     """Generates full python code for lambda
 
     Args:
         python_template_path (str): Location of template python code
         step (Step): Step to place inside template
     """
     code = remove_decorators(inspect.getsource(step.func))
+    logger.debug(f"Code for {step.name}: {code}")
     with open(python_template_path, "r") as f:
         template = f.read()
     template = template.replace('"{{PUT_FUNCTION_HERE}}"', code)
     template = template.replace('"{{PUT_FUNCTION_NAME_HERE}}"', step.func.__name__)
     new_file_name = f"{step.func.__name__}.py"
     with open(new_file_name, "w") as f:
         f.write(template)
@@ -71,45 +71,54 @@
 
     Args:
         python_template_path (str): Location of template python code
         step (Step): `Step` to place inside template
         lambda_entry (str): Name of python entry file
     """
     lambda_python_file = get_python_code(python_template_path, step)
+    args_file = "args.pickle"
+    name_file = "name.pickle"
 
-    with open("args.pickle", "wb") as f:
+    with open(args_file, "wb") as f:
         pickle.dump(
             [step.name if isinstance(step, Step) else step for step in step.args], f
         )
 
-    with open("name.pickle", "wb") as f:
+    with open(name_file, "wb") as f:
         pickle.dump(step.name, f)
 
     zip_name = f"{step.name}.zip"
 
     zf = zipfile.ZipFile(zip_name, mode="w")
     zf.write(lambda_python_file, arcname=f"{lambda_entry}.py")
-    zf.write("args.pickle")
-    zf.write("name.pickle")
+    zf.write(args_file)
+    zf.write(name_file)
     zf.close()
     with open(zip_name, "rb") as f:
         data = f.read()
         hash_sha256 = sha256(data).hexdigest()
+    os.remove(args_file)
+    os.remove(name_file)
+    os.remove(lambda_python_file)
+    logger.info(f"Successfully packaged files for Lambda {step.name}")
+
     return zip_name, hash_sha256
 
 
 def generate_lambda_function(
     scope: Construct,
     name_prefix: str,
     step: Step,
     template_file: str,
     subnet_ids: Optional[List[str]] = None,
     security_group_ids: Optional[List[str]] = None,
 ):
-    """Creates Terraform resource for Lambda
+    """Creates Terraform resource for Lambda.  Automatically
+        adds an environment variable "VAULT_LAMBDA_ROLE" for
+        easier Vault integration.
 
     Args:
         scope
         name_prefix (str): Prefix for lambda name to ensure uniqueness.
         step (Step): Step to create Lambda from
         template_file (str): Location of template file to populate.  Defaults to internal template, but a custom file can be provided.
         subnet_ids (list): Optional subnet IDs.  Required if VPC is specified.
@@ -147,45 +156,62 @@
 
     lambda_role = iam_role.IamRole(
         scope,
         f"{step.name}role",
         assume_role_policy=json.dumps(role),
         name_prefix=step.name,
     )
-    stepfunction_policy = iam_policy.IamPolicy(
+    cloudwatch_policy = iam_policy.IamPolicy(
         scope,
         f"{step.name}policy",
         policy=json.dumps(policy),
     )
     lambda_policy_attachment = iam_role_policy_attachment.IamRolePolicyAttachment(
         scope,
         f"{step.name}policyattachment",
-        policy_arn=stepfunction_policy.arn,
+        policy_arn=cloudwatch_policy.arn,
         role=lambda_role.name,
     )
+    for index, additional_policy in enumerate(step.additional_policies):
+        local_policy = iam_policy.IamPolicy(
+            scope,
+            f"{step.name}_{index}_policy",
+            policy=additional_policy,
+        )
+        local_policy_attachment = iam_role_policy_attachment.IamRolePolicyAttachment(
+            scope,
+            f"{step.name}_{index}policyattachment",
+            policy_arn=local_policy.arn,
+            role=lambda_role.name,
+        )
     vpc_config = (
         None
         if subnet_ids is None
         else {"subnet_ids": subnet_ids, "security_group_ids": security_group_ids}
     )
-    return lambda_function.LambdaFunction(
+    TerraformOutput(scope, f"{step.name}_lambda_role_arn", value=lambda_role.arn)
+    lambda_f = lambda_function.LambdaFunction(
         scope,
         step.name,
         function_name=f"{name_prefix}_{step.name}",
         role=lambda_role.arn,
         filename=lambda_filename,
         timeout=900,
         memory_size=step.memory_size,
         runtime=step.python_runtime,
         handler=lambda_handler,
         vpc_config=vpc_config,
         layers=step.layers,
         source_code_hash=sha256_hash,
-        environment=step.env_variables,
+        environment={
+            "variables": {**step.env_variables, "VAULT_AUTH_ROLE": lambda_role.name}
+        },
     )
+    TerraformOutput(scope, f"{step.name}_lambda_arn", value=lambda_f.arn)
+    return lambda_f
 
 
 def generate_event_bridge(scope: Construct, pipeline: Pipeline, step_function_arn: str):
     """Creates Terraform resource for event bridge to schedule step function run
 
     Args:
         scope
@@ -321,28 +347,30 @@
     )
     stepfunction_policy_attachment = iam_role_policy_attachment.IamRolePolicyAttachment(
         scope,
         f"{pipeline.name}policyattachment",
         policy_arn=stepfunction_policy.arn,
         role=stepfunction_role.name,
     )
-    return sfn_state_machine.SfnStateMachine(
+    step_function = sfn_state_machine.SfnStateMachine(
         scope,
         pipeline.name,
         role_arn=stepfunction_role.arn,
         name=pipeline.name,
         type="STANDARD",
-        definition=pipeline.generate_step_functions().to_json(),
+        definition=json.dumps(pipeline.generate_step_functions()),
         logging_configuration={
             "include_execution_data": True,
             "level": "ALL",
             "log_destination": f"{log_group.arn}:*",
         },
         tracing_configuration={"enabled": True},
     )
+    TerraformOutput(scope, f"{pipeline.name}_stepfunction_arn", value=step_function.arn)
+    return step_function
 
 
 class StepInLine(TerraformStack):
     def __init__(
         self,
         scope: Construct,
         name: str,
@@ -391,28 +419,39 @@
                     }
                 ],
                 vpc_id=vpc_id,
             )
 
             subnet_ids = subnets.ids
             security_group_ids = [security_group_for_lambda.id]
+            logger.info(f"Successfully generated VPC Terraform resources")
 
         step_to_lambda_tf = {}
         for step in pipeline.get_steps():
             step_lambda = generate_lambda_function(
-                self, pipeline.name, step, template_file, subnet_ids, security_group_ids
+                self,
+                pipeline.name,
+                step,
+                template_file,
+                subnet_ids,
+                security_group_ids,
             )
             step_to_lambda_tf[step.name] = step_lambda.arn
+            logger.info(
+                f"Successfully generated Lambda Terraform resource for step {step.name}"
+            )
 
         pipeline.set_generate_step_name(lambda s: step_to_lambda_tf[s.name])
         step_function = generate_step_function(
             self, pipeline, region, list(step_to_lambda_tf.values())
         )
+        logger.info(f"Successfully generated Step Function Terraform resource")
         if pipeline.schedule is not None:
             generate_event_bridge(self, pipeline, step_function.arn)
+            logger.info(f"Successfully generated Event Bridge Terraform resource")
 
 
 def rename_tf_output(path: Path):
     """Terraform creates .tf, but expects .tf.json.  This function
             adds the .json extension and moves it into the root
             directory
 
@@ -422,14 +461,15 @@
     for file in path.glob("*.tf"):
         new_name = file.with_suffix(".tf.json")
         file.replace(new_name.name)  # put in root directory
 
 
 ## example, for testing
 def main():
+    logging.basicConfig(level=logging.INFO)
     app = App(hcl_output=True)
 
     @step
     def preprocess(arg1: str) -> str:
         return "hello"
 
     @step
@@ -448,11 +488,12 @@
     step_process_result_2 = preprocess_2(step_process_result)
     step_process_result_3 = preprocess_3(step_process_result)
     step_train_result = train(
         step_process_result, step_process_result_2, step_process_result_3
     )
     instance_name = "aws_instance"
     pipe = Pipeline("mytest", steps=[step_train_result], schedule="rate(2 minutes)")
+    print(pipe.generate_step_functions())
     stack = StepInLine(app, instance_name, pipe, "us-east-1")
     tf_path = Path(app.outdir, "stacks", instance_name)
     app.synth()
     rename_tf_output(tf_path)
```

### Comparing `step_in_line-0.5.1/PKG-INFO` & `step_in_line-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,66 @@
 Metadata-Version: 2.1
 Name: step-in-line
-Version: 0.5.1
+Version: 0.6.0
 Summary: 
 Author: Daniel Stahl
 Author-email: danstahl1138@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: terraform
 Requires-Dist: attrs (>=23.2.0,<24.0.0)
-Requires-Dist: cdktf (>=0.20.7,<0.21.0)
-Requires-Dist: cdktf-cdktf-provider-aws (>=19.15.0,<20.0.0)
+Requires-Dist: cdktf (>=0.20.7,<0.21.0) ; extra == "terraform"
+Requires-Dist: cdktf-cdktf-provider-aws (>=19.15.0,<20.0.0) ; extra == "terraform"
 Requires-Dist: networkx (==3.2.1)
-Requires-Dist: stepfunctions (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 ## Step-in-line
 
-Step functions are awesome.  It is a fully managed serverless AWS offering, so there is no upkeep or maintenance required.  Unfortunately, programatically created workflows of Lambda functions requires creating complex JSON definitions.  This library generates these JSON definitions automatically from Python decorators.  In addition, it generates the Lambda functions for each Python function.  
+[AWS Step Functions](https://aws.amazon.com/step-functions/) is awesome.  It is a fully managed serverless AWS offering, so there is no upkeep or maintenance required.  Unfortunately, programatically created workflows of Lambda functions using Terraform requires creating complex JSON definitions.  `step-in-line` generates these JSON definitions automatically from Python decorators.  In addition, it generates the Terraform files needed for deploying Step Functions, Lambdas, and EventBridge events.    
 
 The API is intentionally similar to the Sagemaker Pipeline API.  
 
 ## Usage
 
 ### Install
-`pip install step-in-line`
+
+Full install (recommended):
+
+`pip install step-in-line[terraform]`
+
+Don't include Terraform related dependencies:
+
+`pip install step-in-line`.
 
 ### Example Pipeline
 ```python
-from cdktf import App
+
 from step_in_line.step import step
 from step_in_line.pipeline import Pipeline
 from step_in_line.tf import StepInLine, rename_tf_output
 from pathlib import Path
 
-app = App(hcl_output=True)
+lambda_iam_policy = "" # put an IAM policy here, formatted as JSON
 
-# function names must be unique, or you can pass a name to the step to 
-# ensure uniqueness
 @step(
+    # function names must be unique, or you can pass a name to the step to 
+    # ensure uniqueness
     name = "preprocess_unique",
     python_runtime = "python3.9", # defaults to 3.10
     memory_size = 128, # defaults to 512
-    layers = ["arn:aws:lambda:us-east-2:123456789012:layer:example-layer"]
+    layers = ["arn:aws:lambda:us-east-2:123456789012:layer:example-layer"],
+    # be default, Lambda will only get bare permissions; to 
+    # interact with additional AWS Services, need to provide 
+    # IAM policies here.  They will automatically get attached 
+    # to the Lambda Role.  
+    policies = [lambda_iam_policy] 
 )
 def preprocess(arg1: str) -> str:
     # do stuff here, eg run some sql code against snowflake.  
     # Make sure to "import snowflake" within this function.  
     # Will need a "layer" passed which contains the snowflake
     # dependencies.  Must run in <15 minutes.
     return "hello"
@@ -89,20 +101,26 @@
 # "schedule" is optional, and can be cron or rate based
 pipe = Pipeline("mytest", steps=[step_train_result], schedule="rate(2 minutes)")
 
 # to run locally
 print(pipe.local_run()) # will print output of each step
 
 # to extract the step function definition
-print(pipe.generate_step_functions().to_json())
+print(pipe.generate_step_functions())
+
+# to extract the step function definition as a string
+import json
+print(json.dumps(pipe.generate_step_functions()))
 
 # generate terraform json including step function code and lambdas
+# Optionally installed with `pip install step-in-line[terraform]`
+from cdktf import App
+app = App(hcl_output=True)
 instance_name = "aws_instance"
 stack = StepInLine(app, instance_name, pipe, "us-east-1")
-
 # write the terraform json for use by `terraform apply`
 tf_path = Path(app.outdir, "stacks", instance_name)
 app.synth()
 # Terraform Python SDK does not add ".json" extension; this function
 # renames the generated Terraform file and copies it to the project root.
 rename_tf_output(tf_path)
 
@@ -142,21 +160,18 @@
             if "Payload" in ev:
                 payload = {**payload, **ev["Payload"]}
     return payload
 
 
 # Retrieve transform job name from event and return transform job status.
 def lambda_handler(event, context):
-    print(event)
-
+    
     with open("args.pickle", "rb") as f:
         args = pickle.load(f)
-
-    print(args)
-
+    
     with open("name.pickle", "rb") as f:
         name = pickle.load(f)
 
     arg_values = []
     payload = combine_payload(event)
     for arg in args:
         if arg in payload:
@@ -180,10 +195,18 @@
 
 ```python
 stack = StepInLine(app, instance_name, pipe, "us-east-1", template_file="/path/to/your/custom/template.py")
 ```
 
 The `"{{PUT_FUNCTION_HERE}}"` and `"{{PUT_FUNCTION_NAME_HERE}}"` will automatically be replaced by the code of your function defined inside the `@step` decorator and the name of the function, respectively.  
 
+### Limitations
+
+Only Lambda steps are supported.  For other types of steps, including Sagemaker jobs, [Sagemaker Pipelines](https://docs.aws.amazon.com/sagemaker/latest/dg/pipelines-step-decorator-create-pipeline.html) are likely a better option.
+
+All limitations of Lambdas apply.  Each step can only run for 15 minutes before timing out.
+
+
+
 ## API Docs
 
 https://danielhstahl.github.io/step-in-line/index.html
```

