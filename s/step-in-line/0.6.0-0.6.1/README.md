# Comparing `tmp/step_in_line-0.6.0.tar.gz` & `tmp/step_in_line-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "step_in_line-0.6.0.tar", max compression
+gzip compressed data, was "step_in_line-0.6.1.tar", max compression
```

## Comparing `step_in_line-0.6.0.tar` & `step_in_line-0.6.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1069 2024-04-25 14:41:19.058361 step_in_line-0.6.0/LICENSE
--rw-r--r--   0        0        0     6947 2024-04-25 14:41:19.058361 step_in_line-0.6.0/README.md
--rw-r--r--   0        0        0      614 2024-04-25 14:41:34.626480 step_in_line-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-25 14:41:19.058361 step_in_line-0.6.0/step_in_line/__init__.py
--rw-r--r--   0        0        0     5290 2024-04-25 14:41:19.058361 step_in_line-0.6.0/step_in_line/pipeline.py
--rw-r--r--   0        0        0     5192 2024-04-25 14:41:19.058361 step_in_line-0.6.0/step_in_line/step.py
--rw-r--r--   0        0        0      594 2024-04-25 14:41:19.062361 step_in_line-0.6.0/step_in_line/stepfunctions/README.md
--rw-r--r--   0        0        0        0 2024-04-25 14:41:19.062361 step_in_line-0.6.0/step_in_line/stepfunctions/__init__.py
--rw-r--r--   0        0        0     1215 2024-04-25 14:41:19.062361 step_in_line-0.6.0/step_in_line/stepfunctions/fields.py
--rw-r--r--   0        0        0     9815 2024-04-25 14:41:19.062361 step_in_line-0.6.0/step_in_line/stepfunctions/inputs.py
--rw-r--r--   0        0        0    28067 2024-04-25 14:41:19.062361 step_in_line-0.6.0/step_in_line/stepfunctions/steps.py
--rw-r--r--   0        0        0     1695 2024-04-25 14:41:19.062361 step_in_line-0.6.0/step_in_line/template_lambda.py
--rw-r--r--   0        0        0    16251 2024-04-25 14:41:19.062361 step_in_line-0.6.0/step_in_line/tf.py
--rw-r--r--   0        0        0     7638 1970-01-01 00:00:00.000000 step_in_line-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-25 14:57:52.446437 step_in_line-0.6.1/LICENSE
+-rw-r--r--   0        0        0     6947 2024-04-25 14:57:52.446437 step_in_line-0.6.1/README.md
+-rw-r--r--   0        0        0      614 2024-04-25 14:58:06.442513 step_in_line-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-25 14:57:52.446437 step_in_line-0.6.1/step_in_line/__init__.py
+-rw-r--r--   0        0        0     5290 2024-04-25 14:57:52.446437 step_in_line-0.6.1/step_in_line/pipeline.py
+-rw-r--r--   0        0        0     5192 2024-04-25 14:57:52.446437 step_in_line-0.6.1/step_in_line/step.py
+-rw-r--r--   0        0        0      594 2024-04-25 14:57:52.446437 step_in_line-0.6.1/step_in_line/stepfunctions/README.md
+-rw-r--r--   0        0        0        0 2024-04-25 14:57:52.446437 step_in_line-0.6.1/step_in_line/stepfunctions/__init__.py
+-rw-r--r--   0        0        0     1215 2024-04-25 14:57:52.446437 step_in_line-0.6.1/step_in_line/stepfunctions/fields.py
+-rw-r--r--   0        0        0     9384 2024-04-25 14:57:52.446437 step_in_line-0.6.1/step_in_line/stepfunctions/inputs.py
+-rw-r--r--   0        0        0    28046 2024-04-25 14:57:52.446437 step_in_line-0.6.1/step_in_line/stepfunctions/steps.py
+-rw-r--r--   0        0        0     1695 2024-04-25 14:57:52.446437 step_in_line-0.6.1/step_in_line/template_lambda.py
+-rw-r--r--   0        0        0    16251 2024-04-25 14:57:52.446437 step_in_line-0.6.1/step_in_line/tf.py
+-rw-r--r--   0        0        0     7638 1970-01-01 00:00:00.000000 step_in_line-0.6.1/PKG-INFO
```

### Comparing `step_in_line-0.6.0/LICENSE` & `step_in_line-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `step_in_line-0.6.0/README.md` & `step_in_line-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `step_in_line-0.6.0/pyproject.toml` & `step_in_line-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "step-in-line"
-version = "0.6.0"
+version = "0.6.1"
 description = ""
 authors = ["Daniel Stahl <danstahl1138@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 attrs = "^23.2.0"
```

### Comparing `step_in_line-0.6.0/step_in_line/pipeline.py` & `step_in_line-0.6.1/step_in_line/pipeline.py`

 * *Files identical despite different names*

### Comparing `step_in_line-0.6.0/step_in_line/step.py` & `step_in_line-0.6.1/step_in_line/step.py`

 * *Files identical despite different names*

### Comparing `step_in_line-0.6.0/step_in_line/stepfunctions/README.md` & `step_in_line-0.6.1/step_in_line/stepfunctions/README.md`

 * *Files identical despite different names*

### Comparing `step_in_line-0.6.0/step_in_line/stepfunctions/fields.py` & `step_in_line-0.6.1/step_in_line/stepfunctions/fields.py`

 * *Files identical despite different names*

### Comparing `step_in_line-0.6.0/step_in_line/stepfunctions/inputs.py` & `step_in_line-0.6.1/step_in_line/stepfunctions/inputs.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,22 +36,14 @@
     A collection of Placeholder variables.
     """
 
     def __init__(self, schema=None, **kwargs):
         """
         Args:
             schema (dict, optional): Schema for the placeholder collection. (default: None)
-                                     Example below::
-                                        {
-                                            'ModelName': str,
-                                            'JobName': str,
-                                            'Hyperparameters': {
-                                                'tol': float
-                                            }
-                                        }
 
         Keyword Args:
             name (str, optional): Name of the placeholder variable. (default: None)
             type (type, optional): Type of the placeholder variable. (default: None)
             parent (Placeholder, optional): Parent variable for a placeholder variable. (default: None)
         """
         self.store = {}
@@ -156,17 +148,17 @@
         Validate a specified input against the placeholder collection schema.
 
         Args:
             input (dict): Input to validate against the placeholder collection schema.
 
         Returns:
             ValidationResult: Named tuple with the keys:
-                                `valid` (Boolean): Representing the result of validation ,
-                                `keys_missing` (list(str)): List of keys missing in the input ,
-                                `keys_type_mismatch` (list(str), type, type): List of tuples with key name, expected type, and provided type.
+                                "valid" (Boolean): Representing the result of validation ,
+                                "keys_missing" (list(str)): List of keys missing in the input ,
+                                "keys_type_mismatch" (list(str), type, type): List of tuples with key name, expected type, and provided type.
         """
         if input is None:
             return False, None, None
         flattened_schema = flatten(self.get_schema_as_dict())
         flattened_input = flatten(input)
         keys_missing = [i for i in flattened_schema if i not in flattened_input]
         keys_type_mismatch = []
```

### Comparing `step_in_line-0.6.0/step_in_line/stepfunctions/steps.py` & `step_in_line-0.6.1/step_in_line/stepfunctions/steps.py`

 * *Files 7% similar despite different names*

```diff
@@ -115,21 +115,21 @@
     Base class to abstract states in `Amazon States Language <https://states-language.net/spec.html>`_.
     """
 
     def __init__(self, state_id, state_type, output_schema=None, **kwargs):
         """
         Args:
             state_id (str): State name whose length **must be** less than or equal to 128 unicode characters. State names **must be** unique within the scope of the whole state machine.
-            state_type (str): Type of the state. (Allowed values: `'Pass'`, `'Succeed'`, `'Fail'`, `'Wait'`, `'Task'`, `'Choice'`, `'Parallel'`, `'Map'`).
+            state_type (str): Type of the state. (Allowed values: 'Pass', 'Succeed', 'Fail', 'Wait', 'Task', 'Choice', 'Parallel', 'Map').
             output_schema (dict): Expected output schema for the State. This is used to validate placeholder inputs used by the next state in the state machine. (default: None)
             comment (str, optional): Human-readable comment or description. (default: None)
             input_path (str, optional): Path applied to the state’s raw input to select some or all of it; that selection is used by the state. (default: '$')
             parameters (dict, optional): The value of this field becomes the effective input for the state.
             result_path (str, optional): Path specifying the raw input’s combination with or replacement by the state’s result. (default: '$')
-            output_path (str, optional): Path applied to the state’s output after the application of `result_path`, producing the effective output which serves as the raw input for the next state. (default: '$')
+            output_path (str, optional): Path applied to the state’s output after the application of 'result_path', producing the effective output which serves as the raw input for the next state. (default: '$')
         """
         super(State, self).__init__(**kwargs)
         self.fields["type"] = state_type
 
         self.state_type = state_type
         self.state_id = state_id
         self.output_schema = output_schema
@@ -149,15 +149,15 @@
             Field.OutputPath,
             Field.Parameters,
             Field.ResultPath,
         ]
 
     def update_parameters(self, params):
         """
-        Update `parameters` field in the state, if supported.
+        Update 'parameters' field in the state, if supported.
 
         Args:
             params (dict or list): The value of this field becomes the effective input for the state.
         """
         if Field.Parameters in self.allowed_fields():
             self.fields[Field.Parameters.value] = params
 
@@ -272,26 +272,26 @@
     Task State causes the interpreter to execute the work identified by the state’s `resource` field.
     """
 
     def __init__(self, state_id, retry=None, catch=None, **kwargs):
         """
         Args:
             state_id (str): State name whose length **must be** less than or equal to 128 unicode characters. State names **must be** unique within the scope of the whole state machine.
-            retry (Retry or list(Retry), optional): A retrier or list of retriers that define the state's retry policy. See `Error handling in Step Functions <https://docs.aws.amazon.com/step-functions/latest/dg/concepts-error-handling.html#error-handling-retrying-after-an-error>`_ for more details.
-            catch (Catch or list(Catch), optional): A catcher or list of catchers that define a fallback state. See `Error handling in Step Functions <https://docs.aws.amazon.com/step-functions/latest/dg/concepts-error-handling.html#error-handling-fallback-states>`_ for more details.
+            retry (Retry or list(Retry), optional): A retrier or list of retriers that define the state's retry policy. See `Error handling in Step Functions <https://docs.aws.amazon.com/step-functions/latest/dg/concepts-error-handling.html#error-handling-retrying-after-an-error>`__ for more details.
+            catch (Catch or list(Catch), optional): A catcher or list of catchers that define a fallback state. See `Error handling in Step Functions <https://docs.aws.amazon.com/step-functions/latest/dg/concepts-error-handling.html#error-handling-fallback-states>`__ for more details.
             resource (str): A URI that uniquely identifies the specific task to execute. The States language does not constrain the URI scheme nor any other part of the URI.
-            timeout_seconds (int, optional): Positive integer specifying timeout for the state in seconds. If the state runs longer than the specified timeout, then the interpreter fails the state with a `States.Timeout` Error Name. (default: 60)
+            timeout_seconds (int, optional): Positive integer specifying timeout for the state in seconds. If the state runs longer than the specified timeout, then the interpreter fails the state with a 'States.Timeout' Error Name. (default: 60)
             timeout_seconds_path (str, optional): Path specifying the state's timeout value in seconds from the state input. When resolved, the path must select a field whose value is a positive integer.
-            heartbeat_seconds (int, optional): Positive integer specifying heartbeat timeout for the state in seconds. This value should be lower than the one specified for `timeout_seconds`. If more time than the specified heartbeat elapses between heartbeats from the task, then the interpreter fails the state with a `States.Timeout` Error Name.
+            heartbeat_seconds (int, optional): Positive integer specifying heartbeat timeout for the state in seconds. This value should be lower than the one specified for 'timeout_seconds'. If more time than the specified heartbeat elapses between heartbeats from the task, then the interpreter fails the state with a `States.Timeout` Error Name.
             heartbeat_seconds_path (str, optional): Path specifying the state's heartbeat value in seconds from the state input. When resolved, the path must select a field whose value is a positive integer.
             comment (str, optional): Human-readable comment or description. (default: None)
-            input_path (str, optional): Path applied to the state’s raw input to select some or all of it; that selection is used by the state. (default: '$')
+            input_path (str, optional): Path applied to the state's raw input to select some or all of it; that selection is used by the state. (default: '$')
             parameters (dict, optional): The value of this field becomes the effective input for the state.
-            result_path (str, optional): Path specifying the raw input’s combination with or replacement by the state’s result. (default: '$')
-            output_path (str, optional): Path applied to the state’s output after the application of `result_path`, producing the effective output which serves as the raw input for the next state. (default: '$')
+            result_path (str, optional): Path specifying the raw input's combination with or replacement by the state's result. (default: '$')
+            output_path (str, optional): Path applied to the state's output after the application of 'result_path', producing the effective output which serves as the raw input for the next state. (default: '$')
         """
         super(Task, self).__init__(state_id, "Task", **kwargs)
         if self.timeout_seconds is not None and self.timeout_seconds_path is not None:
             raise ValueError(
                 "Only one of 'timeout_seconds' or 'timeout_seconds_path' can be provided."
             )
 
@@ -502,21 +502,21 @@
     A Parallel state causes the interpreter to execute each branch as concurrently as possible, and wait until each branch terminates (reaches a terminal state) before processing the next state in the Chain.
     """
 
     def __init__(self, state_id, retry=None, catch=None, **kwargs):
         """
         Args:
             state_id (str): State name whose length **must be** less than or equal to 128 unicode characters. State names **must be** unique within the scope of the whole state machine.
-            retry (Retry or list(Retry), optional): A retrier or list of retriers that define the state's retry policy. See `Error handling in Step Functions <https://docs.aws.amazon.com/step-functions/latest/dg/concepts-error-handling.html#error-handling-retrying-after-an-error>`_ for more details.
-            catch (Catch or list(Catch), optional): A catcher or list of catchers that define a fallback state. See `Error handling in Step Functions <https://docs.aws.amazon.com/step-functions/latest/dg/concepts-error-handling.html#error-handling-fallback-states>`_ for more details.
+            retry (Retry or list(Retry), optional): A retrier or list of retriers that define the state's retry policy. See `Error handling in Step Functions <https://docs.aws.amazon.com/step-functions/latest/dg/concepts-error-handling.html#error-handling-retrying-after-an-error>`__ for more details.
+            catch (Catch or list(Catch), optional): A catcher or list of catchers that define a fallback state. See `Error handling in Step Functions <https://docs.aws.amazon.com/step-functions/latest/dg/concepts-error-handling.html#error-handling-fallback-states>`__ for more details.
             comment (str, optional): Human-readable comment or description. (default: None)
             input_path (str, optional): Path applied to the state’s raw input to select some or all of it; that selection is used by the state. (default: '$')
             parameters (dict, optional): The value of this field becomes the effective input for the state.
             result_path (str, optional): Path specifying the raw input’s combination with or replacement by the state’s result. (default: '$')
-            output_path (str, optional): Path applied to the state’s output after the application of `result_path`, producing the effective output which serves as the raw input for the next state. (default: '$')
+            output_path (str, optional): Path applied to the state’s output after the application of 'result_path', producing the effective output which serves as the raw input for the next state. (default: '$')
         """
         super(Parallel, self).__init__(state_id, "Parallel", **kwargs)
         self.branches = []
 
         if retry:
             self.add_retry(retry)
 
@@ -556,15 +556,15 @@
     A class for creating a Retry block.
     """
 
     def __init__(self, **kwargs):
         """Initialize a Retry block.
 
         Args:
-            error_equals (list(str)): Non-empty list of strings, which match `Error Names <https://states-language.net/spec.html#error-names>`_. When a state reports an error, the interpreter scans through the retriers and, when the Error Name appears in the value of of a retrier’s `error_equals` field, implements the retry policy described in that retrier.
+            error_equals (list(str)): Non-empty list of strings, which match `Error Names <https://states-language.net/spec.html#error-names>`_. When a state reports an error, the interpreter scans through the retriers and, when the Error Name appears in the value of of a retrier's 'error_equals' field, implements the retry policy described in that retrier.
             interval_seconds (int, optional): Positive integer representing the number of seconds before the first retry attempt. (default: 1)
             max_attempts (int, optional): Non-negative integer representing the maximum number of retry attempts. (default: 3)
             backoff_rate(float, optional): A number which is the multiplier that increases the retry interval on each attempt. (default: 2.0)
         """
         super(Retry, self).__init__(**kwargs)
 
     def allowed_fields(self):
@@ -587,14 +587,15 @@
 
 
 def get_service_integration_arn(
     service, api, integration_pattern=IntegrationPattern.CallAndContinue, version=None
 ):
     """
     ARN builder for task integration
+
     Args:
         service (str): The service name for the service integration
         api (str): The api of the service integration
         integration_pattern (IntegrationPattern, optional): The integration pattern for the task. (Default: IntegrationPattern.CallAndContinue)
         version (int, optional): The version of the resource to use. (Default: None)
     """
     arn = ""
@@ -622,23 +623,23 @@
     """
 
     def __init__(self, state_id, wait_for_callback=False, **kwargs):
         """
         Args:
             state_id (str): State name whose length **must be** less than or equal to 128 unicode characters. State names **must be** unique within the scope of the whole state machine.
             wait_for_callback(bool, optional): Boolean value set to `True` if the Task state should wait for callback to resume the operation. (default: False)
-            timeout_seconds (int, optional): Positive integer specifying timeout for the state in seconds. If the state runs longer than the specified timeout, then the interpreter fails the state with a `States.Timeout` Error Name. (default: 60)
+            timeout_seconds (int, optional): Positive integer specifying timeout for the state in seconds. If the state runs longer than the specified timeout, then the interpreter fails the state with a 'States.Timeout' Error Name. (default: 60)
             timeout_seconds_path (str, optional): Path specifying the state's timeout value in seconds from the state input. When resolved, the path must select a field whose value is a positive integer.
-            heartbeat_seconds (int, optional): Positive integer specifying heartbeat timeout for the state in seconds. This value should be lower than the one specified for `timeout_seconds`. If more time than the specified heartbeat elapses between heartbeats from the task, then the interpreter fails the state with a `States.Timeout` Error Name.
+            heartbeat_seconds (int, optional): Positive integer specifying heartbeat timeout for the state in seconds. This value should be lower than the one specified for 'timeout_seconds'. If more time than the specified heartbeat elapses between heartbeats from the task, then the interpreter fails the state with a `States.Timeout` Error Name.
             heartbeat_seconds_path (str, optional): Path specifying the state's heartbeat value in seconds from the state input. When resolved, the path must select a field whose value is a positive integer.
             comment (str, optional): Human-readable comment or description. (default: None)
             input_path (str, optional): Path applied to the state’s raw input to select some or all of it; that selection is used by the state. (default: '$')
             parameters (dict, optional): The value of this field becomes the effective input for the state.
             result_path (str, optional): Path specifying the raw input’s combination with or replacement by the state’s result. (default: '$')
-            output_path (str, optional): Path applied to the state’s output after the application of `result_path`, producing the effective output which serves as the raw input for the next state. (default: '$')
+            output_path (str, optional): Path applied to the state’s output after the application of 'result_path', producing the effective output which serves as the raw input for the next state. (default: '$')
         """
 
         if wait_for_callback:
             """
             Example resource arn: arn:aws:states:::lambda:invoke.waitForTaskToken
             """
```

### Comparing `step_in_line-0.6.0/step_in_line/template_lambda.py` & `step_in_line-0.6.1/step_in_line/template_lambda.py`

 * *Files identical despite different names*

### Comparing `step_in_line-0.6.0/step_in_line/tf.py` & `step_in_line-0.6.1/step_in_line/tf.py`

 * *Files identical despite different names*

### Comparing `step_in_line-0.6.0/PKG-INFO` & `step_in_line-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: step-in-line
-Version: 0.6.0
+Version: 0.6.1
 Summary: 
 Author: Daniel Stahl
 Author-email: danstahl1138@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

