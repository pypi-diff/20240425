# Comparing `tmp/fmeval-1.0.1-py3-none-any.whl.zip` & `tmp/fmeval-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 131058 bytes, number of entries: 65
+Zip file size: 132926 bytes, number of entries: 67
 -rw-r--r--  2.0 unx       41 b- defN 80-Jan-01 00:00 fmeval/COMMIT_HASH
--rw-r--r--  2.0 unx     4864 b- defN 80-Jan-01 00:00 fmeval/constants.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fmeval/__init__.py
+-rw-r--r--  2.0 unx     4966 b- defN 80-Jan-01 00:00 fmeval/constants.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fmeval/data_loaders/__init__.py
 -rw-r--r--  2.0 unx     2685 b- defN 80-Jan-01 00:00 fmeval/data_loaders/data_config.py
 -rw-r--r--  2.0 unx     3400 b- defN 80-Jan-01 00:00 fmeval/data_loaders/data_sources.py
 -rw-r--r--  2.0 unx     1907 b- defN 80-Jan-01 00:00 fmeval/data_loaders/jmespath_util.py
 -rw-r--r--  2.0 unx     4292 b- defN 80-Jan-01 00:00 fmeval/data_loaders/json_data_loader.py
 -rw-r--r--  2.0 unx    12342 b- defN 80-Jan-01 00:00 fmeval/data_loaders/json_parser.py
 -rw-r--r--  2.0 unx     8073 b- defN 80-Jan-01 00:00 fmeval/data_loaders/util.py
@@ -39,15 +40,15 @@
 -rw-r--r--  2.0 unx     1415 b- defN 80-Jan-01 00:00 fmeval/model_runners/extractors/__init__.py
 -rw-r--r--  2.0 unx      801 b- defN 80-Jan-01 00:00 fmeval/model_runners/extractors/extractor.py
 -rw-r--r--  2.0 unx     3945 b- defN 80-Jan-01 00:00 fmeval/model_runners/extractors/json_extractor.py
 -rw-r--r--  2.0 unx     6419 b- defN 80-Jan-01 00:00 fmeval/model_runners/extractors/jumpstart_extractor.py
 -rw-r--r--  2.0 unx     2123 b- defN 80-Jan-01 00:00 fmeval/model_runners/model_runner.py
 -rw-r--r--  2.0 unx     4754 b- defN 80-Jan-01 00:00 fmeval/model_runners/sm_jumpstart_model_runner.py
 -rw-r--r--  2.0 unx     4344 b- defN 80-Jan-01 00:00 fmeval/model_runners/sm_model_runner.py
--rw-r--r--  2.0 unx     3402 b- defN 80-Jan-01 00:00 fmeval/model_runners/util.py
+-rw-r--r--  2.0 unx     4555 b- defN 80-Jan-01 00:00 fmeval/model_runners/util.py
 -rw-r--r--  2.0 unx      579 b- defN 80-Jan-01 00:00 fmeval/perf_util.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fmeval/reporting/__init__.py
 -rw-r--r--  2.0 unx    11536 b- defN 80-Jan-01 00:00 fmeval/reporting/cells.py
 -rw-r--r--  2.0 unx    18277 b- defN 80-Jan-01 00:00 fmeval/reporting/constants.py
 -rw-r--r--  2.0 unx    20645 b- defN 80-Jan-01 00:00 fmeval/reporting/eval_output_cells.py
 -rw-r--r--  2.0 unx     3932 b- defN 80-Jan-01 00:00 fmeval/reporting/util.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fmeval/transforms/__init__.py
@@ -55,13 +56,14 @@
 -rw-r--r--  2.0 unx     7049 b- defN 80-Jan-01 00:00 fmeval/transforms/common.py
 -rw-r--r--  2.0 unx    12300 b- defN 80-Jan-01 00:00 fmeval/transforms/semantic_perturbations.py
 -rw-r--r--  2.0 unx     6241 b- defN 80-Jan-01 00:00 fmeval/transforms/semantic_robustness_metrics.py
 -rw-r--r--  2.0 unx    11718 b- defN 80-Jan-01 00:00 fmeval/transforms/summarization_accuracy_metrics.py
 -rw-r--r--  2.0 unx     4437 b- defN 80-Jan-01 00:00 fmeval/transforms/transform.py
 -rw-r--r--  2.0 unx     4572 b- defN 80-Jan-01 00:00 fmeval/transforms/transform_pipeline.py
 -rw-r--r--  2.0 unx     4684 b- defN 80-Jan-01 00:00 fmeval/transforms/util.py
--rw-r--r--  2.0 unx     4526 b- defN 80-Jan-01 00:00 fmeval/util.py
--rw-r--r--  2.0 unx    10142 b- defN 80-Jan-01 00:00 fmeval-1.0.1.dist-info/LICENSE
-?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 fmeval-1.0.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx    12438 b- defN 16-Jan-01 00:00 fmeval-1.0.1.dist-info/METADATA
-?rw-r--r--  2.0 unx     6098 b- defN 16-Jan-01 00:00 fmeval-1.0.1.dist-info/RECORD
-65 files, 417041 bytes uncompressed, 121194 bytes compressed:  70.9%
+-rw-r--r--  2.0 unx     4707 b- defN 80-Jan-01 00:00 fmeval/util.py
+-rw-r--r--  2.0 unx    10142 b- defN 80-Jan-01 00:00 fmeval-1.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    15009 b- defN 80-Jan-01 00:00 fmeval-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 fmeval-1.0.2.dist-info/NOTICE
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fmeval-1.0.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     6254 b- defN 16-Jan-01 00:00 fmeval-1.0.2.dist-info/RECORD
+67 files, 421271 bytes uncompressed, 122816 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: fmeval/COMMIT_HASH
 Comment: 
 
+Filename: fmeval/__init__.py
+Comment: 
+
 Filename: fmeval/constants.py
 Comment: 
 
 Filename: fmeval/data_loaders/__init__.py
 Comment: 
 
 Filename: fmeval/data_loaders/data_config.py
@@ -177,20 +180,23 @@
 
 Filename: fmeval/transforms/util.py
 Comment: 
 
 Filename: fmeval/util.py
 Comment: 
 
-Filename: fmeval-1.0.1.dist-info/LICENSE
+Filename: fmeval-1.0.2.dist-info/LICENSE
+Comment: 
+
+Filename: fmeval-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: fmeval-1.0.1.dist-info/WHEEL
+Filename: fmeval-1.0.2.dist-info/NOTICE
 Comment: 
 
-Filename: fmeval-1.0.1.dist-info/METADATA
+Filename: fmeval-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: fmeval-1.0.1.dist-info/RECORD
+Filename: fmeval-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fmeval/COMMIT_HASH

```diff
@@ -1 +1 @@
-91e675be24800a262faf8bf6e59f07522b5314ea
+c76b9239c7d7f006609f86dbcbba22d849a6e51b
```

## fmeval/constants.py

```diff
@@ -16,14 +16,17 @@
 SAGEMAKER_SERVICE_ENDPOINT_URL = "SAGEMAKER_SERVICE_ENDPOINT_URL"
 SAGEMAKER_RUNTIME_ENDPOINT_URL = "SAGEMAKER_RUNTIME_ENDPOINT_URL"
 
 # We default the boto3 client region to us-west-2 as the dataset bucket cannot be accessed from opt-in regions.
 BUILT_IN_DATASET_PREFIX = "s3://fmeval/datasets"
 BUILT_IN_DATASET_DEFAULT_REGION = "us-west-2"
 
+# Environment variable for disabling telemetry
+DISABLE_FMEVAL_TELEMETRY = "DISABLE_FMEVAL_TELEMETRY"
+
 
 @dataclass(frozen=True)
 class Column:
     """
     This class represents a column in the Ray Dataset produced by
     an evaluation algorithm's `evaluate` method.
```

## fmeval/model_runners/util.py

```diff
@@ -1,33 +1,59 @@
 """
 Utilities for model runners.
 """
 import logging
 import os
 from typing import Literal
 import boto3
-import botocore
+import botocore.session
+import botocore.config
 import sagemaker
 
-from fmeval.constants import SAGEMAKER_SERVICE_ENDPOINT_URL, SAGEMAKER_RUNTIME_ENDPOINT_URL
+from fmeval.constants import SAGEMAKER_SERVICE_ENDPOINT_URL, SAGEMAKER_RUNTIME_ENDPOINT_URL, DISABLE_FMEVAL_TELEMETRY
+from fmeval.util import get_fmeval_package_version
+from sagemaker.user_agent import determine_prefix
 from mypy_boto3_bedrock.client import BedrockClient
 
+
 logger = logging.getLogger(__name__)
 
 
-def get_boto_session() -> boto3.session.Session:
+def get_user_agent_extra() -> str:
+    """
+    :return: A string to be used as the user_agent_extra parameter in a botocore config.
+    """
+    # Obtain user-agent headers for information such as SageMaker notebook instance type and SageMaker Studio app type.
+    # We manually obtain these headers, so we can pass them in the user_agent_extra parameter of botocore.config.Config.
+    # This is because although these headers are already obtained in the sagemaker.session.Session initializer,
+    # there is currently a bug in the sagemaker.session.Session code where these headers get assigned to an instance
+    # attribute, but don't actually show up in the user-agent header when making API calls.
+    sagemaker_python_sdk_headers = determine_prefix()
+    return (
+        sagemaker_python_sdk_headers
+        if os.getenv(DISABLE_FMEVAL_TELEMETRY)
+        else f"{sagemaker_python_sdk_headers} fmeval/{get_fmeval_package_version()}"
+    )
+
+
+def get_boto_session(
+    boto_retry_mode: Literal["legacy", "standard", "adaptive"],
+    retry_attempts: int,
+) -> boto3.session.Session:
     """
     Get boto3 session with adaptive retry config
     :return: The new session
     """
     botocore_session: botocore.session.Session = botocore.session.get_session()
     botocore_session.set_default_client_config(
         botocore.config.Config(
             # https://boto3.amazonaws.com/v1/documentation/api/latest/guide/retries.html
-            retries={"mode": "adaptive", "max_attempts": 10}
+            retries={"mode": boto_retry_mode, "max_attempts": retry_attempts},
+            # https://botocore.amazonaws.com/v1/documentation/api/latest/reference/config.html
+            user_agent_extra=get_user_agent_extra(),
         )
     )
     return boto3.session.Session(botocore_session=botocore_session)
 
 
 def get_sagemaker_session(
     boto_retry_mode: Literal["legacy", "standard", "adaptive"] = "adaptive",
@@ -35,27 +61,24 @@
 ) -> sagemaker.Session:
     """
     Get SageMaker session with adaptive retry config.
     :param boto_retry_mode: retry mode used for botocore config (legacy/standard/adaptive).
     :param retry_attempts: max retry attempts used for botocore client failures
     :return: The new session
     """
-    boto_session = get_boto_session()
-    boto_config = botocore.client.Config(retries={"mode": boto_retry_mode, "max_attempts": retry_attempts})
+    boto_session = get_boto_session(boto_retry_mode, retry_attempts)
     sagemaker_service_endpoint_url = os.getenv(SAGEMAKER_SERVICE_ENDPOINT_URL)
     sagemaker_runtime_endpoint_url = os.getenv(SAGEMAKER_RUNTIME_ENDPOINT_URL)
     sagemaker_client = boto_session.client(
         service_name="sagemaker",
         endpoint_url=sagemaker_service_endpoint_url,
-        config=boto_config,
     )
     sagemaker_runtime_client = boto_session.client(
         service_name="sagemaker-runtime",
         endpoint_url=sagemaker_runtime_endpoint_url,
-        config=boto_config,
     )
     sagemaker_session = sagemaker.session.Session(
         boto_session=boto_session,
         sagemaker_client=sagemaker_client,
         sagemaker_runtime_client=sagemaker_runtime_client,
     )
     return sagemaker_session
@@ -67,29 +90,26 @@
 ) -> BedrockClient:
     """
     Get Bedrock runtime client with adaptive retry config.
     :param boto_retry_mode: retry mode used for botocore config (legacy/standard/adaptive).
     :param retry_attempts: max retry attempts used for botocore client failures
     :return: The new session
     """
-    boto_session = get_boto_session()
-    bedrock_runtime_client = boto_session.client(  # type: ignore
-        service_name="bedrock-runtime",
-        config=botocore.client.Config(retries={"mode": boto_retry_mode, "max_attempts": retry_attempts}),
-    )
+    boto_session = get_boto_session(boto_retry_mode, retry_attempts)
+    bedrock_runtime_client = boto_session.client(service_name="bedrock-runtime")
     return bedrock_runtime_client
 
 
 def is_endpoint_in_service(
     sagemaker_session: sagemaker.session.Session,
     endpoint_name: str,
 ) -> bool:
     """
     :param sagemaker_session: SageMaker session to be reused.
     :param endpoint_name: SageMaker endpoint name.
-    :return None
+    :return: Whether the endpoint is in service
     """
     in_service = True
     desc = sagemaker_session.sagemaker_client.describe_endpoint(EndpointName=endpoint_name)
     if not desc or "EndpointStatus" not in desc or desc["EndpointStatus"] != "InService":
         in_service = False
     return in_service
```

## fmeval/util.py

```diff
@@ -1,12 +1,12 @@
 import os
 import re
-
 import ray
 import multiprocessing as mp
+import importlib.metadata
 
 from ray.actor import ActorHandle
 from fmeval.constants import EVAL_RESULTS_PATH, DEFAULT_EVAL_RESULTS_PATH, PARALLELIZATION_FACTOR
 from fmeval.exceptions import EvalAlgorithmInternalError, EvalAlgorithmClientError
 
 
 def require(expression, msg: str):
@@ -111,18 +111,25 @@
     """
     resource_cls, serialized_data = resource.__reduce__()  # type: ignore[misc]
     wrapped_resource_cls = ray.remote(num_cpus=num_cpus)(resource_cls)
     return wrapped_resource_cls.remote(*serialized_data)  # type: ignore
 
 
 def cleanup_shared_resource(resource: ActorHandle) -> None:
-    """Removes the resource from shared memory.
+    """Remove the resource from shared memory.
 
     Concretely, this function kills the Ray actor corresponding
     to `resource`, which in most cases will be an actor created
     via create_shared_resource.
 
     :param resource: A Ray actor handle to a shared resource
         (ex: a BertscoreHelperModel).
     :returns: None
     """
     ray.kill(resource)
+
+
+def get_fmeval_package_version() -> str:
+    """
+    :returns: The current fmeval package version.
+    """
+    return importlib.metadata.version("fmeval")
```

## Comparing `fmeval-1.0.1.dist-info/LICENSE` & `fmeval-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fmeval-1.0.1.dist-info/METADATA` & `fmeval-1.0.2.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: fmeval
-Version: 1.0.1
+Version: 1.0.2
 Summary: Amazon Foundation Model Evaluations
 License: Apache-2.0
 Author: Amazon FMEval Team
 Author-email: amazon-fmeval-team@amazon.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: IPython
 Requires-Dist: aiohttp (>=3.9.2,<4.0.0)
 Requires-Dist: bert-score (>=0.3.13,<0.4.0)
 Requires-Dist: evaluate (>=0.4.0,<0.5.0)
 Requires-Dist: grpcio (>=1.60.0,<2.0.0)
 Requires-Dist: ipykernel (>=6.26.0,<7.0.0)
 Requires-Dist: jiwer (>=3.0.3,<4.0.0)
 Requires-Dist: markdown
-Requires-Dist: matplotlib (>=3.8.0,<4.0.0)
+Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: mypy-boto3-bedrock (>=1.33.2,<2.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: pandas (==2.1.4)
 Requires-Dist: pyarrow
 Requires-Dist: pyfunctional (==1.4.3)
 Requires-Dist: ray (==2.9.1)
 Requires-Dist: rouge-score (>=0.1.2,<0.2.0)
@@ -51,67 +52,77 @@
 * Algorithms to evaluate LLMs for Accuracy, Toxicity, Semantic Robustness and
   Prompt Stereotyping across different tasks.
 * Implementations of the `ModelRunner` interface. `ModelRunner` encapsulates the logic for invoking different types of LLMs, exposing a `predict` method to simplify interactions with LLMs within the eval algorithm code. We have built-in support for Amazon SageMaker Endpoints and JumpStart models. The user can extend the interface for their own model classes by implementing the `predict` method.
 
 ## Installation
 `fmeval` is developed under python3.10. To install the package, simply run:
 
-```
+```sh
 pip install fmeval
 ```
 
 ## Usage
 You can see examples of running evaluations on your LLMs with built-in or custom datasets in
 the [examples folder](https://github.com/aws/fmeval/tree/main/examples).
 
 The main steps for using `fmeval` are:
 1. Create a `ModelRunner` which can perform invocation on your LLM. `fmeval` provides built-in support for Amazon SageMaker Endpoints and JumpStart LLMs. You can also extend the `ModelRunner` interface for any LLMs hosted anywhere.
 2. Use any of the supported [eval_algorithms](https://github.com/aws/fmeval/tree/main/src/fmeval/eval_algorithms).
 
 For example,
-```
+```python
 from fmeval.eval_algorithms.toxicity import Toxicity, ToxicityConfig
 
 eval_algo = Toxicity(ToxicityConfig())
 eval_output = eval_algo.evaluate(model=model_runner)
 ```
 *Note: You can update the default eval config parameters for your specific use case.*
 
 ### Using a custom dataset for an evaluation
 We have our built-in datasets configured, which are consumed for computing the scores in eval algorithms.
 You can choose to use a custom dataset in the following manner.
 1. Create a [DataConfig](https://github.com/aws/fmeval/blob/main/src/fmeval/data_loaders/data_config.py)
    for your custom dataset
-```
+```python
 config = DataConfig(
     dataset_name="custom_dataset",
     dataset_uri="./custom_dataset.jsonl",
     dataset_mime_type="application/jsonlines",
     model_input_location="question",
     target_output_location="answer",
 )
 ```
 
 2. Use an eval algorithm with a custom dataset
-```
+```python
 eval_algo = Toxicity(ToxicityConfig())
 eval_output = eval_algo.evaluate(model=model_runner, dataset_config=config)
 ```
 
 *Please refer to the [developer guide](https://docs.aws.amazon.com/sagemaker/latest/dg/clarify-foundation-model-evaluate-auto.html) and
 [examples](https://github.com/aws/fmeval/tree/main/examples) for more details around the usage of
 eval algorithms.*
 
+## Telemetry
+By default, `fmeval` has very basic telemetry enabled, purely for tracking usage of the package.
+The only data that is tracked is the number of SageMaker, JumpStart, or Bedrock `ModelRunner` objects that get created.
+*We do not collect any user-level data*.
+
+The `ModelRunner` data in question gets collected via the use of an fmeval-specific user agent header that is used by the botocore session that manages these model runners.
+See `fmeval.model_runners.util.get_user_agent_extra` and `fmeval.model_runners.util.get_boto_session` for implementation details.
+
+To opt out of telemetry, simply set the `DISABLE_FMEVAL_TELEMETRY` environment variable to any non-null value.
+
 ## Troubleshooting
 
 1. Users running `fmeval` on a Windows machine may encounter the error `OSError: [Errno 0] AssignProcessToJobObject() failed` when `fmeval` internally calls `ray.init()`. This OS error is a known Ray issue, and is detailed [here](https://github.com/ray-project/ray/issues/21994). Multiple users have reported that installing Python from the [official Python website](https://www.python.org/downloads/windows/) rather than the Microsoft store fixes this issue. You can view more details on limitations of running Ray on Windows on [Ray's webpage](https://docs.ray.io/en/latest/ray-overview/installation.html#windows-support).
 
 2. If you run into the error `error: can't find Rust compiler` while installing `fmeval` on a Mac, please try running the steps below.
 
-```
+```sh
 curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
 rustup install 1.72.1
 rustup default 1.72.1-aarch64-apple-darwin
 rustup toolchain remove stable-aarch64-apple-darwin
 rm -rf $HOME/.rustup/toolchains/stable-aarch64-apple-darwin
 mv $HOME/.rustup/toolchains/1.72.1-aarch64-apple-darwin $HOME/.rustup/toolchains/stable-aarch64-apple-darwin
 ```
@@ -121,20 +132,43 @@
 models. By default, `fmeval` loads multiple copies of the model into memory to maximize parallelization, where the exact number depends on the number of cores on the machine. To reduce the number of models that get loaded in parallel, you can
 set the environment variable `PARALLELIZATION_FACTOR` to a value that suits your machine.
 
 ## Development
 
 ### Setup and the use of `devtool`
 Once you have created a virtual environment with python3.10, run the following command to set up the development environment:
-```
+```sh
 ./devtool install_deps_dev
 ./devtool install_deps
 ./devtool all
 ```
 
+**Note**: If you are on a Mac, the `install_poetry_version` devtool command may fail when running the poetry installation script. If there is a failure, you should get error logs sent to a file with a name like `poetry-installer-error-cvulo5s0.log`. Open the logs, and if the error message looks like the following:
+```
+dyld[10908]: Library not loaded: @loader_path/../../../../Python.framework/Versions/3.10/Python
+  Referenced from: <8A5DEEDB-CE8E-325F-88B0-B0397BD5A5DE> /Users/daniezh/Library/Application Support/pypoetry/venv/bin/python3
+  Reason: tried: '/Users/daniezh/Library/Application Support/pypoetry/venv/bin/../../../../Python.framework/Versions/3.10/Python' (no such file), '/Library/Frameworks/Python.framework/Versions/3.10/Python' (no such file), '/System/Library/Frameworks/Python.framework/Versions/3.10/Python' (no such file, not in dyld cache)
+
+Traceback:
+
+  File "<string>", line 923, in main
+  File "<string>", line 562, in run
+```
+then you will need to tweak the poetry installation script and re-run it.
+
+Steps:
+1. `curl -sSL https://install.python-poetry.org > poetry_script.py`
+2. Change the `symlinks` argument in `builder = venv.EnvBuilder(clear=True, with_pip=True, symlinks=False)` to `True`. See mionker's comment [here](https://github.com/python-poetry/install.python-poetry.org/issues/56) for an explanation.
+3. `python poetry_script.py --version 1.8.2` (where `1.8.2` is the version listed in `devtool`; this may change after the time of this writing).
+4. Confirm installation via `poetry --version`
+
+Additionally, if you already have an existing version of Poetry installed and want to install a new version, before you re-run the above command, you will need to uninstall Poetry:
+
+`curl -sSL https://install.python-poetry.org | python3 - --uninstall`
+
 Before submitting a PR, rerun `./devtool all` for testing and linting. It should run without errors.
 
 ### Adding python dependencies
 We use [poetry](https://python-poetry.org/docs/) to manage python dependencies in this project. If you want to add a new
 dependency, please update the [pyproject.toml](./pyproject.toml) file, and run the `poetry update` command to update the
 `poetry.lock` file (which is checked in).
 
@@ -152,29 +186,29 @@
 #### The `Transform` class
 We represent the concept of a record-level transformation using the `Transform` class. `Transform` is a callable class where its `__call__` method takes a single argument, `record`, which represents the record to be transformed. A record is represented by a Python dictionary. To implement your own record-level transformation logic, create a concrete subclass of `Transform` and implement its `__call__` method.
 
 **Example:**
 
 Let's implement a `Transform` for a simple, toy metric.
 
-```
+```python
 class NumSpaces(Transform):
     """
     Augments the input record (which contains some text data)
     with the number of spaces found in the text.
     """
     def __call__(self, record: Dict[str, Any]) -> Dict[str, Any]:
         input_text = record["input_text"]
         record["num_spaces"] = input_text.count(" ")
         return record
 ```
 
 One issue with this simple example is that the keys used for the input text data and the output data are both hard-coded. This generally isn't desirable, so let's improve on our running example.
 
-```
+```python
 class NumSpaces(Transform):
     """
     Augments the input record (which contains some text data)
     with the number of spaces found in the text.
     """
 
     def __init__(self, text_key, output_key):
@@ -195,15 +229,15 @@
 
 **Example:**
 Here, we implement a pipeline for a very simple evaluation. The steps are:
 1. Construct LLM prompts from raw text inputs
 2. Feed the prompts to a `ModelRunner` to get the model outputs
 3. Compute the "number of spaces" metric we defined above
 
-```
+```python
 # Use the built-in utility Transform for generating prompts
 gen_prompt = GeneratePrompt(
     input_keys="model_input",
     output_keys="prompt",
     prompt_template="Answer the following question: $model_input",
 )
```

## Comparing `fmeval-1.0.1.dist-info/RECORD` & `fmeval-1.0.2.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-fmeval/COMMIT_HASH,sha256=DzsbgicgvtB-ppdM0fNgEg-Mn4F7HJlOFvAAMiXFDL8,41
-fmeval/constants.py,sha256=gNwBJQGCISMDIUMu5H-Cy9nH0nkIQ6fMwoWHulx4cTI,4864
+fmeval/COMMIT_HASH,sha256=hkFlmHZiGHktQUCNjhond_N5wh1KaAFHQW7bJi-Wvik,41
+fmeval/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+fmeval/constants.py,sha256=g3LAxWxAUVjfUGi2n8MxfykZ2cMSCfdJpo6_ylxJsms,4966
 fmeval/data_loaders/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fmeval/data_loaders/data_config.py,sha256=jZyFS6DmZ8QEgAMiIdnhHumGpIRj7WT3YPmiUpUu7O0,2685
 fmeval/data_loaders/data_sources.py,sha256=Vm6LSCrE_BG144KQKXYV23xjMyydClxBv3PyW4Ux9Ck,3400
 fmeval/data_loaders/jmespath_util.py,sha256=eYLHQnJY4woIJjm2UH1STnkIvQHfe7gl7sPlVROudOc,1907
 fmeval/data_loaders/json_data_loader.py,sha256=uPzYBJJAaCPuibKnitXCAmef5-yBNHFEqy9i6g0dVTo,4292
 fmeval/data_loaders/json_parser.py,sha256=x-ZHGXu_HToLVLEjAt1uYYdt6c5n3XOaKIGjImPGU1w,12342
 fmeval/data_loaders/util.py,sha256=y_XW6D-ICjGuNqFdAHr_OBMpRjzOR0b15glQqgOgbY0,8073
@@ -38,15 +39,15 @@
 fmeval/model_runners/extractors/__init__.py,sha256=hcL0dFcgSVl4fXZv1LCD1mYko3XkNOMFMwaXn42ieoo,1415
 fmeval/model_runners/extractors/extractor.py,sha256=4MF-ddkJSpuMgjgQ3kEvR2oF5EeJXN6jL0QI5ZOavrs,801
 fmeval/model_runners/extractors/json_extractor.py,sha256=qM-sZxHLsdgxxYdJ1FV4UcFDwTLph87XBg4MxCg5wR0,3945
 fmeval/model_runners/extractors/jumpstart_extractor.py,sha256=MvcWsQ_Ba3ChyM_54ueoO9Zo0Ku2cu1WHzed_qNV9dE,6419
 fmeval/model_runners/model_runner.py,sha256=_qRNZI1WsBinNwZ-qGBDbIfKzfk_X-0zChH1caZPo1U,2123
 fmeval/model_runners/sm_jumpstart_model_runner.py,sha256=pxRxWyZFZ5FIjVtcW-8kdbpEt9ftjcMNG5M0hHV1CxM,4754
 fmeval/model_runners/sm_model_runner.py,sha256=QFbKXNYDZcylY7as6YHDOFmgShBQR6TFvWZAwVTCpBE,4344
-fmeval/model_runners/util.py,sha256=64qvV_F_xBI9KuSh74CQcfOdiwgfvLsKtikhh9mIsZA,3402
+fmeval/model_runners/util.py,sha256=ADunfEHQ-XJSfTa8TNgw1UWTtb13EfO1P1U3lRaUoUA,4555
 fmeval/perf_util.py,sha256=h_vw4yZXvRDmoQVRhnTYf5VmuWZtjzQgbip_uOBOm54,579
 fmeval/reporting/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fmeval/reporting/cells.py,sha256=LKCv8hoUGuIc639KsNqyq0MSXcU_HwicdmYH_cJeDX4,11536
 fmeval/reporting/constants.py,sha256=4sHRHAXp40N6Zp6lZ2fSukUES8MzHsa5qZdlrS5d-wo,18277
 fmeval/reporting/eval_output_cells.py,sha256=UZIpRfiw6slOsVx1EXK04e9wDPIa8RP7EfUIyXcgtJA,20645
 fmeval/reporting/util.py,sha256=6bYcVJ6ErTrVT91J9vJ0dyDEotpX6CHbNZB9O5nq7XI,3932
 fmeval/transforms/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -54,12 +55,13 @@
 fmeval/transforms/common.py,sha256=6njUK3s0eiAsLed-jHHbtEQPxCp7DJVN8nOKb0yJpHY,7049
 fmeval/transforms/semantic_perturbations.py,sha256=etmFWOlOYJWu4sINy268GUI8YV3S7Ispj4z5hM30ClM,12300
 fmeval/transforms/semantic_robustness_metrics.py,sha256=lEv6vHVzDvUOqHTDIeS6RfFaoYXcSkXKqvYwwKzrcOU,6241
 fmeval/transforms/summarization_accuracy_metrics.py,sha256=KUAYevzgSLTjbVwddtogavfT1tPPAcEAVqsxkAag8Ag,11718
 fmeval/transforms/transform.py,sha256=brePXgZJTVRzldiCpD96ayEuVb5tOHXbauYzz6fDyWY,4437
 fmeval/transforms/transform_pipeline.py,sha256=UUZtxSrmqMqEH6su28TDz-8GCmgG0IaQ2E5iOIfcDdE,4572
 fmeval/transforms/util.py,sha256=9aQPqL7LEYCh5co-0QCrSxsePwRo9j3Co-S5frwtTIE,4684
-fmeval/util.py,sha256=GHQQepz7qX0v3cFyw3ihPNaKDLf3U-G_mmD23XJHEC4,4526
-fmeval-1.0.1.dist-info/LICENSE,sha256=CeipvOyAZxBGUsFoaFqwkx54aPnIKEtm9a5u2uXxEws,10142
-fmeval-1.0.1.dist-info/WHEEL,sha256=bbU3AyvhQ312rVm7zzRQjs6axI1UYWC3nmFA2E6FFSI,88
-fmeval-1.0.1.dist-info/METADATA,sha256=AI2I5sEXdO2uau0iRFc529tyfsfO9JKKYXEhqnhucq0,12438
-fmeval-1.0.1.dist-info/RECORD,,
+fmeval/util.py,sha256=tSKO9_T9bL2v77naWtNRs0OAAm5CFDuOXdUgbo-7JJY,4707
+fmeval-1.0.2.dist-info/LICENSE,sha256=CeipvOyAZxBGUsFoaFqwkx54aPnIKEtm9a5u2uXxEws,10142
+fmeval-1.0.2.dist-info/METADATA,sha256=-mf0DpydZ2i5Uvsr17hYYFWdMGUQjp4h1vXnZfQn3yc,15009
+fmeval-1.0.2.dist-info/NOTICE,sha256=1CkO1kwu3Q_OHYTj-d-yiBJA_lNN73a4zSntavaD4oc,67
+fmeval-1.0.2.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+fmeval-1.0.2.dist-info/RECORD,,
```

