# Comparing `tmp/step_in_line-0.4.0.tar.gz` & `tmp/step_in_line-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "step_in_line-0.4.0.tar", max compression
+gzip compressed data, was "step_in_line-0.4.1.tar", max compression
```

## Comparing `step_in_line-0.4.0.tar` & `step_in_line-0.4.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2024-04-24 17:28:16.698818 step_in_line-0.4.0/LICENSE
--rw-r--r--   0        0        0     3593 2024-04-24 17:28:16.698818 step_in_line-0.4.0/README.md
--rw-r--r--   0        0        0      505 2024-04-24 17:28:29.522910 step_in_line-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 17:28:16.698818 step_in_line-0.4.0/step_in_line/__init__.py
--rw-r--r--   0        0        0     4855 2024-04-24 17:28:16.698818 step_in_line-0.4.0/step_in_line/pipeline.py
--rw-r--r--   0        0        0     4818 2024-04-24 17:28:16.698818 step_in_line-0.4.0/step_in_line/step.py
--rw-r--r--   0        0        0      935 2024-04-24 17:28:16.698818 step_in_line-0.4.0/step_in_line/template_lambda.py
--rw-r--r--   0        0        0    13470 2024-04-24 17:28:16.698818 step_in_line-0.4.0/step_in_line/tf.py
--rw-r--r--   0        0        0     4258 1970-01-01 00:00:00.000000 step_in_line-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-24 23:39:28.139051 step_in_line-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3591 2024-04-24 23:39:28.143051 step_in_line-0.4.1/README.md
+-rw-r--r--   0        0        0      505 2024-04-24 23:39:43.530935 step_in_line-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 23:39:28.143051 step_in_line-0.4.1/step_in_line/__init__.py
+-rw-r--r--   0        0        0     5160 2024-04-24 23:39:28.143051 step_in_line-0.4.1/step_in_line/pipeline.py
+-rw-r--r--   0        0        0     4818 2024-04-24 23:39:28.143051 step_in_line-0.4.1/step_in_line/step.py
+-rw-r--r--   0        0        0     1729 2024-04-24 23:39:28.143051 step_in_line-0.4.1/step_in_line/template_lambda.py
+-rw-r--r--   0        0        0    13470 2024-04-24 23:39:28.143051 step_in_line-0.4.1/step_in_line/tf.py
+-rw-r--r--   0        0        0     4256 1970-01-01 00:00:00.000000 step_in_line-0.4.1/PKG-INFO
```

### Comparing `step_in_line-0.4.0/LICENSE` & `step_in_line-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `step_in_line-0.4.0/README.md` & `step_in_line-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 app = App(hcl_output=True)
 
 # function names must be unique, or you can pass a name to the step to 
 # ensure uniqueness
 @step(
     name = "preprocess_unique",
     python_runtime = "python3.9", # defaults to 3.10
-    memory_size = "128", # defaults to 512
+    memory_size = 128, # defaults to 512
     layers = ["arn:aws:lambda:us-east-2:123456789012:layer:example-layer"]
 )
 def preprocess(arg1: str) -> str:
     # do stuff here, eg run some sql code against snowflake.  
     # Make sure to "import snowflake" within this function.  
     # Will need a "layer" passed which contains the snowflake
     # dependencies.  Must run in <15 minutes.
```

### Comparing `step_in_line-0.4.0/step_in_line/pipeline.py` & `step_in_line-0.4.1/step_in_line/pipeline.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         step (Step): The `Step` to convert to a lambda
         generate_step_name (callable): Generates the ARN of the Lambda from the step
     """
     lambda_state = LambdaStep(
         state_id=step.name,
         parameters={
             "FunctionName": generate_step_name(step),  # the function arn
-            "Payload.$": "$",
+            "Payload.$": "$",  # pass in all the possible values, including outputs from previous steps
         },
     )
     if step.retry_count > 0:
         lambda_state.add_retry(
             Retry(
                 error_equals=["States.TaskFailed"],
                 interval_seconds=15,
@@ -89,15 +89,16 @@
         return len(set(step.name for step in self.get_steps())) == num_steps
 
     def get_steps(self) -> List[Step]:
         """Gets all steps, guaranteed to be unique."""
         return self.graph.nodes
 
     def generate_layers(self) -> List[List[Step]]:
-        """Create indexed sets of steps.
+        """
+        Create indexed sets of steps.
         This allows steps to be run in parallel,
         if they don't depend on each other
         """
         return list(nx.topological_generations(self.graph))
 
     def generate_step_functions(self) -> Graph:
         """Create Step Function dictionary"""
@@ -118,17 +119,22 @@
         workflow = Workflow(name=self.name, definition=chain, role="doesnotmatter")
         return workflow.definition
 
     def set_generate_step_name(self, generate_step_name: Callable[[Step], str]):
         self.generate_step_name = generate_step_name
 
     def local_run(self) -> List[List[Tuple[str, Any]]]:
-        """Runs pipeline locally, with no AWS dependency"""
-        outputs = {}
-        output_arr = []
+        """
+        Runs pipeline locally, with no AWS dependency.
+        Returns all intermediary outputs.
+        """
+        outputs = {}  # contains all intermediary output
+        output_arr = (
+            []
+        )  # constains all intermediary output, in the shape of the steps given by the topological generations
         for layer in self.generate_layers():
             layer_output = []
             for step in layer:
                 args = []
                 for arg in step.args:
                     if isinstance(arg, Step):
                         args.append(outputs[arg.name])
```

### Comparing `step_in_line-0.4.0/step_in_line/step.py` & `step_in_line-0.4.1/step_in_line/step.py`

 * *Files identical despite different names*

### Comparing `step_in_line-0.4.0/step_in_line/tf.py` & `step_in_line-0.4.1/step_in_line/tf.py`

 * *Files identical despite different names*

### Comparing `step_in_line-0.4.0/PKG-INFO` & `step_in_line-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: step-in-line
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Author: Daniel Stahl
 Author-email: danstahl1138@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -34,15 +34,15 @@
 app = App(hcl_output=True)
 
 # function names must be unique, or you can pass a name to the step to 
 # ensure uniqueness
 @step(
     name = "preprocess_unique",
     python_runtime = "python3.9", # defaults to 3.10
-    memory_size = "128", # defaults to 512
+    memory_size = 128, # defaults to 512
     layers = ["arn:aws:lambda:us-east-2:123456789012:layer:example-layer"]
 )
 def preprocess(arg1: str) -> str:
     # do stuff here, eg run some sql code against snowflake.  
     # Make sure to "import snowflake" within this function.  
     # Will need a "layer" passed which contains the snowflake
     # dependencies.  Must run in <15 minutes.
```

