# Comparing `tmp/spark_on_k8s-0.4.0.tar.gz` & `tmp/spark_on_k8s-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_on_k8s-0.4.0.tar", max compression
+gzip compressed data, was "spark_on_k8s-0.5.0.tar", max compression
```

## Comparing `spark_on_k8s-0.4.0.tar` & `spark_on_k8s-0.5.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11357 2024-03-24 23:53:57.897354 spark_on_k8s-0.4.0/LICENSE
--rw-r--r--   0        0        0    11020 2024-03-24 23:53:57.897354 spark_on_k8s-0.4.0/README.md
--rw-r--r--   0        0        0     2366 2024-03-24 23:54:13.057250 spark_on_k8s-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       58 2024-03-24 23:53:57.901354 spark_on_k8s-0.4.0/spark_on_k8s/__init__.py
--rw-r--r--   0        0        0        0 2024-03-24 23:53:57.901354 spark_on_k8s-0.4.0/spark_on_k8s/airflow/__init__.py
--rw-r--r--   0        0        0    14892 2024-03-24 23:53:57.901354 spark_on_k8s-0.4.0/spark_on_k8s/airflow/operators.py
--rw-r--r--   0        0        0     3114 2024-03-24 23:53:57.901354 spark_on_k8s-0.4.0/spark_on_k8s/airflow/triggers.py
--rw-r--r--   0        0        0     1190 2024-03-24 23:53:57.901354 spark_on_k8s-0.4.0/spark_on_k8s/api/__init__.py
--rw-r--r--   0        0        0     1744 2024-03-24 23:53:57.901354 spark_on_k8s-0.4.0/spark_on_k8s/api/app.py
--rw-r--r--   0        0        0     1374 2024-03-24 23:53:57.901354 spark_on_k8s-0.4.0/spark_on_k8s/api/apps.py
--rw-r--r--   0        0        0      634 2024-03-24 23:53:57.901354 spark_on_k8s-0.4.0/spark_on_k8s/api/configuration.py
--rw-r--r--   0        0        0     1305 2024-03-24 23:53:57.901354 spark_on_k8s-0.4.0/spark_on_k8s/api/main.py
--rw-r--r--   0        0        0     3927 2024-03-24 23:53:57.901354 spark_on_k8s-0.4.0/spark_on_k8s/api/webserver/__init__.py
--rw-r--r--   0        0        0      587 2024-03-24 23:53:57.901354 spark_on_k8s-0.4.0/spark_on_k8s/api/webserver/static/app_logs.css
--rw-r--r--   0        0        0      758 2024-03-24 23:53:57.901354 spark_on_k8s-0.4.0/spark_on_k8s/api/webserver/static/apps.css
--rw-r--r--   0        0        0     1092 2024-03-24 23:53:57.901354 spark_on_k8s-0.4.0/spark_on_k8s/api/webserver/templates/app_logs.html
--rw-r--r--   0        0        0     2670 2024-03-24 23:53:57.901354 spark_on_k8s-0.4.0/spark_on_k8s/api/webserver/templates/apps.html
--rw-r--r--   0        0        0      368 2024-03-24 23:53:57.901354 spark_on_k8s-0.4.0/spark_on_k8s/api/webserver/templates/error.html
--rw-r--r--   0        0        0      542 2024-03-24 23:53:57.901354 spark_on_k8s-0.4.0/spark_on_k8s/cli/__init__.py
--rw-r--r--   0        0        0     1621 2024-03-24 23:53:57.901354 spark_on_k8s-0.4.0/spark_on_k8s/cli/api.py
--rw-r--r--   0        0        0     6601 2024-03-24 23:53:57.901354 spark_on_k8s-0.4.0/spark_on_k8s/cli/app.py
--rw-r--r--   0        0        0      690 2024-03-24 23:53:57.901354 spark_on_k8s-0.4.0/spark_on_k8s/cli/apps.py
--rw-r--r--   0        0        0      553 2024-03-24 23:53:57.901354 spark_on_k8s-0.4.0/spark_on_k8s/cli/namespace.py
--rw-r--r--   0        0        0     8686 2024-03-24 23:53:57.901354 spark_on_k8s-0.4.0/spark_on_k8s/cli/options.py
--rw-r--r--   0        0        0    27728 2024-03-24 23:53:57.901354 spark_on_k8s-0.4.0/spark_on_k8s/client.py
--rw-r--r--   0        0        0        0 2024-03-24 23:53:57.901354 spark_on_k8s-0.4.0/spark_on_k8s/k8s/__init__.py
--rw-r--r--   0        0        0     3135 2024-03-24 23:53:57.905354 spark_on_k8s-0.4.0/spark_on_k8s/k8s/async_client.py
--rw-r--r--   0        0        0     2849 2024-03-24 23:53:57.905354 spark_on_k8s-0.4.0/spark_on_k8s/k8s/sync_client.py
--rw-r--r--   0        0        0        0 2024-03-24 23:53:57.905354 spark_on_k8s-0.4.0/spark_on_k8s/utils/__init__.py
--rw-r--r--   0        0        0    19764 2024-03-24 23:53:57.905354 spark_on_k8s-0.4.0/spark_on_k8s/utils/app_manager.py
--rw-r--r--   0        0        0     9617 2024-03-24 23:53:57.905354 spark_on_k8s-0.4.0/spark_on_k8s/utils/async_app_manager.py
--rw-r--r--   0        0        0     4048 2024-03-24 23:53:57.905354 spark_on_k8s-0.4.0/spark_on_k8s/utils/configuration.py
--rw-r--r--   0        0        0      488 2024-03-24 23:53:57.905354 spark_on_k8s-0.4.0/spark_on_k8s/utils/logging_mixin.py
--rw-r--r--   0        0        0     3956 2024-03-24 23:53:57.905354 spark_on_k8s-0.4.0/spark_on_k8s/utils/setup_namespace.py
--rw-r--r--   0        0        0      842 2024-03-24 23:53:57.905354 spark_on_k8s-0.4.0/spark_on_k8s/utils/spark_app_status.py
--rw-r--r--   0        0        0      141 2024-03-24 23:53:57.905354 spark_on_k8s-0.4.0/spark_on_k8s/utils/types.py
--rw-r--r--   0        0        0    12867 1970-01-01 00:00:00.000000 spark_on_k8s-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-25 21:05:34.122675 spark_on_k8s-0.5.0/LICENSE
+-rw-r--r--   0        0        0    11213 2024-04-25 21:05:34.122675 spark_on_k8s-0.5.0/README.md
+-rw-r--r--   0        0        0     2366 2024-04-25 21:05:48.250682 spark_on_k8s-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       58 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/airflow/__init__.py
+-rw-r--r--   0        0        0    14892 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/airflow/operators.py
+-rw-r--r--   0        0        0     3114 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/airflow/triggers.py
+-rw-r--r--   0        0        0     1190 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/api/__init__.py
+-rw-r--r--   0        0        0     1744 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/api/app.py
+-rw-r--r--   0        0        0     1472 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/api/apps.py
+-rw-r--r--   0        0        0      728 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/api/configuration.py
+-rw-r--r--   0        0        0     1305 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/api/main.py
+-rw-r--r--   0        0        0     6750 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/api/webserver/__init__.py
+-rw-r--r--   0        0        0      587 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/api/webserver/static/app_logs.css
+-rw-r--r--   0        0        0      758 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/api/webserver/static/apps.css
+-rw-r--r--   0        0        0     1092 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/api/webserver/templates/app_logs.html
+-rw-r--r--   0        0        0     2953 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/api/webserver/templates/apps.html
+-rw-r--r--   0        0        0      368 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/api/webserver/templates/error.html
+-rw-r--r--   0        0        0      542 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/cli/__init__.py
+-rw-r--r--   0        0        0     1621 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/cli/api.py
+-rw-r--r--   0        0        0     6601 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/cli/app.py
+-rw-r--r--   0        0        0      690 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/cli/apps.py
+-rw-r--r--   0        0        0      553 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/cli/namespace.py
+-rw-r--r--   0        0        0     8686 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/cli/options.py
+-rw-r--r--   0        0        0    27728 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/client.py
+-rw-r--r--   0        0        0        0 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/k8s/__init__.py
+-rw-r--r--   0        0        0     3135 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/k8s/async_client.py
+-rw-r--r--   0        0        0     2849 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/k8s/sync_client.py
+-rw-r--r--   0        0        0        0 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/utils/__init__.py
+-rw-r--r--   0        0        0    19764 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/utils/app_manager.py
+-rw-r--r--   0        0        0     9617 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/utils/async_app_manager.py
+-rw-r--r--   0        0        0     4048 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/utils/configuration.py
+-rw-r--r--   0        0        0      488 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/utils/logging_mixin.py
+-rw-r--r--   0        0        0     3956 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/utils/setup_namespace.py
+-rw-r--r--   0        0        0      842 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/utils/spark_app_status.py
+-rw-r--r--   0        0        0      141 2024-04-25 21:05:34.126675 spark_on_k8s-0.5.0/spark_on_k8s/utils/types.py
+-rw-r--r--   0        0        0    13060 1970-01-01 00:00:00.000000 spark_on_k8s-0.5.0/PKG-INFO
```

### Comparing `spark_on_k8s-0.4.0/LICENSE` & `spark_on_k8s-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.4.0/README.md` & `spark_on_k8s-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -135,62 +135,65 @@
 To deploy the API in production, you can use the project helm chart, that setups all the required resources in the
 cluster, including the API deployment, the service, the ingress and the RBAC resources. The API has a configuration
 class that loads the configuration from environment variables, so you can use the helm chart `env` values to configure
 the API and its Kubernetes client.
 
 To install the helm chart, you can run:
 ```bash
-helm install spark-on-k8s chart --values examples/helm/values.yaml
+helm repo add spark-on-k8s http://hussein.awala.fr/spark-on-k8s-chart
+helm repo update
+helm install spark-on-k8s-release spark-on-k8s/spark-on-k8s --values examples/helm/values.yaml
 ```
 
 ## Configuration
 
 The Python client and the CLI can be configured with environment variables to avoid passing the same arguments every
 time if you have a common configuration for all your apps. The environment variables are the same for both the client
 and the CLI. Here is a list of the available environment variables:
 
-| Environment Variable                       | Description                                           | Default      |
-|--------------------------------------------|-------------------------------------------------------|--------------|
-| SPARK_ON_K8S_DOCKER_IMAGE                  | The docker image to use for the spark pods            |              |
-| SPARK_ON_K8S_APP_PATH                      | The path to the app file                              |              |
-| SPARK_ON_K8S_NAMESPACE                     | The namespace to use                                  | default      |
-| SPARK_ON_K8S_SERVICE_ACCOUNT               | The service account to use                            | spark        |
-| SPARK_ON_K8S_SPARK_CONF                    | The spark configuration to use                        | {}           |
-| SPARK_ON_K8S_CLASS_NAME                    | The class name to use                                 |              |
-| SPARK_ON_K8S_APP_ARGUMENTS                 | The arguments to pass to the app                      | []           |
-| SPARK_ON_K8S_APP_WAITER                    | The waiter to use to wait for the app to finish       | no_wait      |
-| SPARK_ON_K8S_IMAGE_PULL_POLICY             | The image pull policy to use                          | IfNotPresent |
-| SPARK_ON_K8S_UI_REVERSE_PROXY              | Whether to use a reverse proxy to access the spark UI | false        |
-| SPARK_ON_K8S_DRIVER_CPU                    | The driver CPU                                        | 1            |
-| SPARK_ON_K8S_DRIVER_MEMORY                 | The driver memory                                     | 1024         |
-| SPARK_ON_K8S_DRIVER_MEMORY_OVERHEAD        | The driver memory overhead                            | 512          |
-| SPARK_ON_K8S_EXECUTOR_CPU                  | The executor CPU                                      | 1            |
-| SPARK_ON_K8S_EXECUTOR_MEMORY               | The executor memory                                   | 1024         |
-| SPARK_ON_K8S_EXECUTOR_MEMORY_OVERHEAD      | The executor memory overhead                          | 512          |
-| SPARK_ON_K8S_EXECUTOR_MIN_INSTANCES        | The minimum number of executor instances              |              |
-| SPARK_ON_K8S_EXECUTOR_MAX_INSTANCES        | The maximum number of executor instances              |              |
-| SPARK_ON_K8S_EXECUTOR_INITIAL_INSTANCES    | The initial number of executor instances              |              |
-| SPARK_ON_K8S_CONFIG_FILE                   | The path to the config file                           |              |
-| SPARK_ON_K8S_CONTEXT                       | The context to use                                    |              |
-| SPARK_ON_K8S_CLIENT_CONFIG                 | The sync Kubernetes client configuration to use       |              |
-| SPARK_ON_K8S_ASYNC_CLIENT_CONFIG           | The async Kubernetes client configuration to use      |              |
-| SPARK_ON_K8S_IN_CLUSTER                    | Whether to use the in cluster Kubernetes config       | false        |
-| SPARK_ON_K8S_API_DEFAULT_NAMESPACE         | The default namespace to use for the API              | default      |
-| SPARK_ON_K8S_API_HOST                      | The host to use for the API                           | 127.0.0.1    |
-| SPARK_ON_K8S_API_PORT                      | The port to use for the API                           | 8000         |
-| SPARK_ON_K8S_API_WORKERS                   | The number of workers to use for the API              | 4            |
-| SPARK_ON_K8S_API_LOG_LEVEL                 | The log level to use for the API                      | info         |
-| SPARK_ON_K8S_API_LIMIT_CONCURRENCY         | The limit concurrency to use for the API              | 1000         |
-| SPARK_ON_K8S_SPARK_DRIVER_NODE_SELECTOR    | The node selector to use for the driver pod           | {}           |
-| SPARK_ON_K8S_SPARK_EXECUTOR_NODE_SELECTOR  | The node selector to use for the executor pods        | {}           |
-| SPARK_ON_K8S_SPARK_DRIVER_LABELS           | The labels to use for the driver pod                  | {}           |
-| SPARK_ON_K8S_SPARK_EXECUTOR_LABELS         | The labels to use for the executor pods               | {}           |
-| SPARK_ON_K8S_SPARK_DRIVER_ANNOTATIONS      | The annotations to use for the driver pod             | {}           |
-| SPARK_ON_K8S_SPARK_EXECUTOR_ANNOTATIONS    | The annotations to use for the executor pods          | {}           |
-| SPARK_ON_K8S_EXECUTOR_POD_TEMPLATE_PATH    | The path to the executor pod template                 |              |
+| Environment Variable                      | Description                                           | Default      |
+|-------------------------------------------|-------------------------------------------------------|--------------|
+| SPARK_ON_K8S_DOCKER_IMAGE                 | The docker image to use for the spark pods            |              |
+| SPARK_ON_K8S_APP_PATH                     | The path to the app file                              |              |
+| SPARK_ON_K8S_NAMESPACE                    | The namespace to use                                  | default      |
+| SPARK_ON_K8S_SERVICE_ACCOUNT              | The service account to use                            | spark        |
+| SPARK_ON_K8S_SPARK_CONF                   | The spark configuration to use                        | {}           |
+| SPARK_ON_K8S_CLASS_NAME                   | The class name to use                                 |              |
+| SPARK_ON_K8S_APP_ARGUMENTS                | The arguments to pass to the app                      | []           |
+| SPARK_ON_K8S_APP_WAITER                   | The waiter to use to wait for the app to finish       | no_wait      |
+| SPARK_ON_K8S_IMAGE_PULL_POLICY            | The image pull policy to use                          | IfNotPresent |
+| SPARK_ON_K8S_UI_REVERSE_PROXY             | Whether to use a reverse proxy to access the spark UI | false        |
+| SPARK_ON_K8S_DRIVER_CPU                   | The driver CPU                                        | 1            |
+| SPARK_ON_K8S_DRIVER_MEMORY                | The driver memory                                     | 1024         |
+| SPARK_ON_K8S_DRIVER_MEMORY_OVERHEAD       | The driver memory overhead                            | 512          |
+| SPARK_ON_K8S_EXECUTOR_CPU                 | The executor CPU                                      | 1            |
+| SPARK_ON_K8S_EXECUTOR_MEMORY              | The executor memory                                   | 1024         |
+| SPARK_ON_K8S_EXECUTOR_MEMORY_OVERHEAD     | The executor memory overhead                          | 512          |
+| SPARK_ON_K8S_EXECUTOR_MIN_INSTANCES       | The minimum number of executor instances              |              |
+| SPARK_ON_K8S_EXECUTOR_MAX_INSTANCES       | The maximum number of executor instances              |              |
+| SPARK_ON_K8S_EXECUTOR_INITIAL_INSTANCES   | The initial number of executor instances              |              |
+| SPARK_ON_K8S_CONFIG_FILE                  | The path to the config file                           |              |
+| SPARK_ON_K8S_CONTEXT                      | The context to use                                    |              |
+| SPARK_ON_K8S_CLIENT_CONFIG                | The sync Kubernetes client configuration to use       |              |
+| SPARK_ON_K8S_ASYNC_CLIENT_CONFIG          | The async Kubernetes client configuration to use      |              |
+| SPARK_ON_K8S_IN_CLUSTER                   | Whether to use the in cluster Kubernetes config       | false        |
+| SPARK_ON_K8S_API_DEFAULT_NAMESPACE        | The default namespace to use for the API              | default      |
+| SPARK_ON_K8S_API_HOST                     | The host to use for the API                           | 127.0.0.1    |
+| SPARK_ON_K8S_API_PORT                     | The port to use for the API                           | 8000         |
+| SPARK_ON_K8S_API_WORKERS                  | The number of workers to use for the API              | 4            |
+| SPARK_ON_K8S_API_LOG_LEVEL                | The log level to use for the API                      | info         |
+| SPARK_ON_K8S_API_LIMIT_CONCURRENCY        | The limit concurrency to use for the API              | 1000         |
+| SPARK_ON_K8S_API_SPARK_HISTORY_HOST       | The host to use for the spark history server          |              |
+| SPARK_ON_K8S_SPARK_DRIVER_NODE_SELECTOR   | The node selector to use for the driver pod           | {}           |
+| SPARK_ON_K8S_SPARK_EXECUTOR_NODE_SELECTOR | The node selector to use for the executor pods        | {}           |
+| SPARK_ON_K8S_SPARK_DRIVER_LABELS          | The labels to use for the driver pod                  | {}           |
+| SPARK_ON_K8S_SPARK_EXECUTOR_LABELS        | The labels to use for the executor pods               | {}           |
+| SPARK_ON_K8S_SPARK_DRIVER_ANNOTATIONS     | The annotations to use for the driver pod             | {}           |
+| SPARK_ON_K8S_SPARK_EXECUTOR_ANNOTATIONS   | The annotations to use for the executor pods          | {}           |
+| SPARK_ON_K8S_EXECUTOR_POD_TEMPLATE_PATH   | The path to the executor pod template                 |              |
 
 
 ## Examples
 
 Here are some examples of how to package and submit spark apps with this package. In the examples, the base image is
 built with the spark image tool, as described in the
 [spark documentation](https://spark.apache.org/docs/latest/running-on-kubernetes.html#docker-images).
```

### Comparing `spark_on_k8s-0.4.0/pyproject.toml` & `spark_on_k8s-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spark-on-k8s"
-version = "0.4.0"
+version = "0.5.0"
 description = "A Python package to submit and manage Apache Spark applications on Kubernetes."
 authors = ["Hussein Awala <hussein@awala.fr>"]
 readme = "README.md"
 repository = "https://github.com/hussein-awala/spark-on-k8s"
 keywords = ["spark", "kubernetes", "k8s", "spark-submit", "spark-on-k8s"]
 license = "Apache-2.0"
 packages = [{include = "spark_on_k8s"}]
```

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/airflow/operators.py` & `spark_on_k8s-0.5.0/spark_on_k8s/airflow/operators.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/airflow/triggers.py` & `spark_on_k8s-0.5.0/spark_on_k8s/airflow/triggers.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/api/__init__.py` & `spark_on_k8s-0.5.0/spark_on_k8s/api/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/api/app.py` & `spark_on_k8s-0.5.0/spark_on_k8s/api/app.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/api/apps.py` & `spark_on_k8s-0.5.0/spark_on_k8s/api/apps.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 
 
 class SparkApp(BaseModel):
     """App status."""
 
     app_id: str
     status: SparkAppStatus
+    driver_logs: bool = False
     spark_ui_proxy: bool = False
+    spark_history_proxy: bool = False
 
 
 @router.get("/list_apps")
 async def list_apps_default_namespace() -> list[SparkApp]:
     """List spark apps in the default namespace."""
     return await list_apps(namespace=APIConfiguration.SPARK_ON_K8S_API_DEFAULT_NAMESPACE)
 
@@ -35,11 +37,12 @@
     driver_pods = await core_client.list_namespaced_pod(
         namespace=namespace, label_selector="spark-role=driver"
     )
     return [
         SparkApp(
             app_id=pod.metadata.labels.get("spark-app-id", pod.metadata.name),
             status=get_app_status(pod),
+            driver_logs=True,
             spark_ui_proxy=pod.metadata.labels.get("spark-ui-proxy", False),
         )
         for pod in driver_pods.items
     ]
```

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/api/configuration.py` & `spark_on_k8s-0.5.0/spark_on_k8s/api/configuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,7 +9,8 @@
     # API configuration
     SPARK_ON_K8S_API_DEFAULT_NAMESPACE = getenv("SPARK_ON_K8S_API_DEFAULT_NAMESPACE", "default")
     SPARK_ON_K8S_API_HOST = getenv("SPARK_ON_K8S_API_HOST", "127.0.0.1")
     SPARK_ON_K8S_API_PORT = int(getenv("SPARK_ON_K8S_API_PORT", "8000"))
     SPARK_ON_K8S_API_WORKERS = int(getenv("SPARK_ON_K8S_API_WORKERS", "4"))
     SPARK_ON_K8S_API_LOG_LEVEL = getenv("SPARK_ON_K8S_API_LOG_LEVEL", "info")
     SPARK_ON_K8S_API_LIMIT_CONCURRENCY = int(getenv("SPARK_ON_K8S_API_LIMIT_CONCURRENCY", "1000"))
+    SPARK_ON_K8S_API_SPARK_HISTORY_HOST = getenv("SPARK_ON_K8S_API_SPARK_HISTORY_HOST", None)
```

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/api/main.py` & `spark_on_k8s-0.5.0/spark_on_k8s/api/main.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/api/webserver/static/app_logs.css` & `spark_on_k8s-0.5.0/spark_on_k8s/api/webserver/static/app_logs.css`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/api/webserver/static/apps.css` & `spark_on_k8s-0.5.0/spark_on_k8s/api/webserver/static/apps.css`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/api/webserver/templates/app_logs.html` & `spark_on_k8s-0.5.0/spark_on_k8s/api/webserver/templates/app_logs.html`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/api/webserver/templates/apps.html` & `spark_on_k8s-0.5.0/spark_on_k8s/api/webserver/templates/apps.html`

 * *Files 4% similar despite different names*

```diff
@@ -51,31 +51,38 @@
         <th>Links</th>
     </tr>
     {% for app in apps_list %}
     <tr>
         <td>
             {{ app.app_id }}
             <div style="float: right;">
-                {% if app.spark_ui_proxy and app.status.value == 'Running' %}
+                {% if app.status.value == 'Running' %}
                 <span class="action" onclick="killApp('{{ namespace }}', '{{ app.app_id }}')">Kill</span>
                 <br>
                 {% endif %}
                 <span class="action" onclick="deleteApp('{{ namespace }}', '{{ app.app_id }}')">Delete</span>
             </div>
         </td>
         <td>{{ app.status.value }}</td>
         <td>
             {% if app.spark_ui_proxy and app.status.value == 'Running' %}
             <a href="/webserver/ui/{{ namespace }}/{{ app.app_id }}" target="_blank">
                 <button class="spark-button">Open Spark UI</button>
             </a>
             {% endif %}
+            {% if app.driver_logs %}
             <a href="/webserver/logs/{{ namespace }}/{{ app.app_id }}?tail=1000" target="_blank">
                 <button class="spark-button">View Driver Logs</button>
             </a>
+            {% endif %}
+            {% if app.spark_history_proxy %}
+            <a href="/webserver/ui-history/history/{{ app.app_id }}" target="_blank">
+                <button class="spark-button">Open Spark History</button>
+            </a>
+            {% endif %}
         </td>
     </tr>
     {% endfor %}
 </table>
 
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,8 +1,12 @@
 ************ SSppaarrkk AAppppss SSttaattuuss ************
- _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
-|_AA_pp_pp_ _II_DD_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_SS_tt_aa_tt_uu_ss_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_LL_ii_nn_kk_ss_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
-|{{ app.app_id }}        |                      |{% if app.spark_ui_proxy and|
-|{% if app.spark_ui_proxy|                      |app.status.value ==         |
-|and app.status.value == |{{ app.status.value }}|'Running' %} _O_p_e_n_ _S_p_a_r_k_ _U_I_  |
-|'Running' %} Kill       |                      |{% endif %} _V_i_e_w_ _D_r_i_v_e_r_ _L_o_g_s|
-|_{_%_ _e_n_d_i_f_ _%_}_ _D_e_l_e_t_e_ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
+ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
+|_AA_pp_pp_ _II_DD_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_SS_tt_aa_tt_uu_ss_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_LL_ii_nn_kk_ss_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
+|                         |                      |{% if app.spark_ui_proxy and|
+|                         |                      |app.status.value ==         |
+|{{ app.app_id }}         |                      |'Running' %} _O_p_e_n_ _S_p_a_r_k_ _U_I_  |
+|{% if app.status.value ==|                      |{% endif %} {% if           |
+|'Running' %} Kill        |{{ app.status.value }}|app.driver_logs %} _V_i_e_w     |
+|{% endif %} Delete       |                      |_D_r_i_v_e_r_ _L_o_g_s_ {% endif %} {%  |
+|                         |                      |if app.spark_history_proxy  |
+|                         |                      |%} _O_p_e_n_ _S_p_a_r_k_ _H_i_s_t_o_r_y_ {%    |
+|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_e_n_d_i_f_ _%_}_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
```

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/cli/__init__.py` & `spark_on_k8s-0.5.0/spark_on_k8s/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/cli/api.py` & `spark_on_k8s-0.5.0/spark_on_k8s/cli/api.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/cli/app.py` & `spark_on_k8s-0.5.0/spark_on_k8s/cli/app.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/cli/apps.py` & `spark_on_k8s-0.5.0/spark_on_k8s/cli/apps.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/cli/namespace.py` & `spark_on_k8s-0.5.0/spark_on_k8s/cli/namespace.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/cli/options.py` & `spark_on_k8s-0.5.0/spark_on_k8s/cli/options.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/client.py` & `spark_on_k8s-0.5.0/spark_on_k8s/client.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/k8s/async_client.py` & `spark_on_k8s-0.5.0/spark_on_k8s/k8s/async_client.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/k8s/sync_client.py` & `spark_on_k8s-0.5.0/spark_on_k8s/k8s/sync_client.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/utils/app_manager.py` & `spark_on_k8s-0.5.0/spark_on_k8s/utils/app_manager.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/utils/async_app_manager.py` & `spark_on_k8s-0.5.0/spark_on_k8s/utils/async_app_manager.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/utils/configuration.py` & `spark_on_k8s-0.5.0/spark_on_k8s/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/utils/setup_namespace.py` & `spark_on_k8s-0.5.0/spark_on_k8s/utils/setup_namespace.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.4.0/spark_on_k8s/utils/spark_app_status.py` & `spark_on_k8s-0.5.0/spark_on_k8s/utils/spark_app_status.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.4.0/PKG-INFO` & `spark_on_k8s-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-on-k8s
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python package to submit and manage Apache Spark applications on Kubernetes.
 Home-page: https://github.com/hussein-awala/spark-on-k8s
 License: Apache-2.0
 Keywords: spark,kubernetes,k8s,spark-submit,spark-on-k8s
 Author: Hussein Awala
 Author-email: hussein@awala.fr
 Requires-Python: >=3.8,<4.0
@@ -171,62 +171,65 @@
 To deploy the API in production, you can use the project helm chart, that setups all the required resources in the
 cluster, including the API deployment, the service, the ingress and the RBAC resources. The API has a configuration
 class that loads the configuration from environment variables, so you can use the helm chart `env` values to configure
 the API and its Kubernetes client.
 
 To install the helm chart, you can run:
 ```bash
-helm install spark-on-k8s chart --values examples/helm/values.yaml
+helm repo add spark-on-k8s http://hussein.awala.fr/spark-on-k8s-chart
+helm repo update
+helm install spark-on-k8s-release spark-on-k8s/spark-on-k8s --values examples/helm/values.yaml
 ```
 
 ## Configuration
 
 The Python client and the CLI can be configured with environment variables to avoid passing the same arguments every
 time if you have a common configuration for all your apps. The environment variables are the same for both the client
 and the CLI. Here is a list of the available environment variables:
 
-| Environment Variable                       | Description                                           | Default      |
-|--------------------------------------------|-------------------------------------------------------|--------------|
-| SPARK_ON_K8S_DOCKER_IMAGE                  | The docker image to use for the spark pods            |              |
-| SPARK_ON_K8S_APP_PATH                      | The path to the app file                              |              |
-| SPARK_ON_K8S_NAMESPACE                     | The namespace to use                                  | default      |
-| SPARK_ON_K8S_SERVICE_ACCOUNT               | The service account to use                            | spark        |
-| SPARK_ON_K8S_SPARK_CONF                    | The spark configuration to use                        | {}           |
-| SPARK_ON_K8S_CLASS_NAME                    | The class name to use                                 |              |
-| SPARK_ON_K8S_APP_ARGUMENTS                 | The arguments to pass to the app                      | []           |
-| SPARK_ON_K8S_APP_WAITER                    | The waiter to use to wait for the app to finish       | no_wait      |
-| SPARK_ON_K8S_IMAGE_PULL_POLICY             | The image pull policy to use                          | IfNotPresent |
-| SPARK_ON_K8S_UI_REVERSE_PROXY              | Whether to use a reverse proxy to access the spark UI | false        |
-| SPARK_ON_K8S_DRIVER_CPU                    | The driver CPU                                        | 1            |
-| SPARK_ON_K8S_DRIVER_MEMORY                 | The driver memory                                     | 1024         |
-| SPARK_ON_K8S_DRIVER_MEMORY_OVERHEAD        | The driver memory overhead                            | 512          |
-| SPARK_ON_K8S_EXECUTOR_CPU                  | The executor CPU                                      | 1            |
-| SPARK_ON_K8S_EXECUTOR_MEMORY               | The executor memory                                   | 1024         |
-| SPARK_ON_K8S_EXECUTOR_MEMORY_OVERHEAD      | The executor memory overhead                          | 512          |
-| SPARK_ON_K8S_EXECUTOR_MIN_INSTANCES        | The minimum number of executor instances              |              |
-| SPARK_ON_K8S_EXECUTOR_MAX_INSTANCES        | The maximum number of executor instances              |              |
-| SPARK_ON_K8S_EXECUTOR_INITIAL_INSTANCES    | The initial number of executor instances              |              |
-| SPARK_ON_K8S_CONFIG_FILE                   | The path to the config file                           |              |
-| SPARK_ON_K8S_CONTEXT                       | The context to use                                    |              |
-| SPARK_ON_K8S_CLIENT_CONFIG                 | The sync Kubernetes client configuration to use       |              |
-| SPARK_ON_K8S_ASYNC_CLIENT_CONFIG           | The async Kubernetes client configuration to use      |              |
-| SPARK_ON_K8S_IN_CLUSTER                    | Whether to use the in cluster Kubernetes config       | false        |
-| SPARK_ON_K8S_API_DEFAULT_NAMESPACE         | The default namespace to use for the API              | default      |
-| SPARK_ON_K8S_API_HOST                      | The host to use for the API                           | 127.0.0.1    |
-| SPARK_ON_K8S_API_PORT                      | The port to use for the API                           | 8000         |
-| SPARK_ON_K8S_API_WORKERS                   | The number of workers to use for the API              | 4            |
-| SPARK_ON_K8S_API_LOG_LEVEL                 | The log level to use for the API                      | info         |
-| SPARK_ON_K8S_API_LIMIT_CONCURRENCY         | The limit concurrency to use for the API              | 1000         |
-| SPARK_ON_K8S_SPARK_DRIVER_NODE_SELECTOR    | The node selector to use for the driver pod           | {}           |
-| SPARK_ON_K8S_SPARK_EXECUTOR_NODE_SELECTOR  | The node selector to use for the executor pods        | {}           |
-| SPARK_ON_K8S_SPARK_DRIVER_LABELS           | The labels to use for the driver pod                  | {}           |
-| SPARK_ON_K8S_SPARK_EXECUTOR_LABELS         | The labels to use for the executor pods               | {}           |
-| SPARK_ON_K8S_SPARK_DRIVER_ANNOTATIONS      | The annotations to use for the driver pod             | {}           |
-| SPARK_ON_K8S_SPARK_EXECUTOR_ANNOTATIONS    | The annotations to use for the executor pods          | {}           |
-| SPARK_ON_K8S_EXECUTOR_POD_TEMPLATE_PATH    | The path to the executor pod template                 |              |
+| Environment Variable                      | Description                                           | Default      |
+|-------------------------------------------|-------------------------------------------------------|--------------|
+| SPARK_ON_K8S_DOCKER_IMAGE                 | The docker image to use for the spark pods            |              |
+| SPARK_ON_K8S_APP_PATH                     | The path to the app file                              |              |
+| SPARK_ON_K8S_NAMESPACE                    | The namespace to use                                  | default      |
+| SPARK_ON_K8S_SERVICE_ACCOUNT              | The service account to use                            | spark        |
+| SPARK_ON_K8S_SPARK_CONF                   | The spark configuration to use                        | {}           |
+| SPARK_ON_K8S_CLASS_NAME                   | The class name to use                                 |              |
+| SPARK_ON_K8S_APP_ARGUMENTS                | The arguments to pass to the app                      | []           |
+| SPARK_ON_K8S_APP_WAITER                   | The waiter to use to wait for the app to finish       | no_wait      |
+| SPARK_ON_K8S_IMAGE_PULL_POLICY            | The image pull policy to use                          | IfNotPresent |
+| SPARK_ON_K8S_UI_REVERSE_PROXY             | Whether to use a reverse proxy to access the spark UI | false        |
+| SPARK_ON_K8S_DRIVER_CPU                   | The driver CPU                                        | 1            |
+| SPARK_ON_K8S_DRIVER_MEMORY                | The driver memory                                     | 1024         |
+| SPARK_ON_K8S_DRIVER_MEMORY_OVERHEAD       | The driver memory overhead                            | 512          |
+| SPARK_ON_K8S_EXECUTOR_CPU                 | The executor CPU                                      | 1            |
+| SPARK_ON_K8S_EXECUTOR_MEMORY              | The executor memory                                   | 1024         |
+| SPARK_ON_K8S_EXECUTOR_MEMORY_OVERHEAD     | The executor memory overhead                          | 512          |
+| SPARK_ON_K8S_EXECUTOR_MIN_INSTANCES       | The minimum number of executor instances              |              |
+| SPARK_ON_K8S_EXECUTOR_MAX_INSTANCES       | The maximum number of executor instances              |              |
+| SPARK_ON_K8S_EXECUTOR_INITIAL_INSTANCES   | The initial number of executor instances              |              |
+| SPARK_ON_K8S_CONFIG_FILE                  | The path to the config file                           |              |
+| SPARK_ON_K8S_CONTEXT                      | The context to use                                    |              |
+| SPARK_ON_K8S_CLIENT_CONFIG                | The sync Kubernetes client configuration to use       |              |
+| SPARK_ON_K8S_ASYNC_CLIENT_CONFIG          | The async Kubernetes client configuration to use      |              |
+| SPARK_ON_K8S_IN_CLUSTER                   | Whether to use the in cluster Kubernetes config       | false        |
+| SPARK_ON_K8S_API_DEFAULT_NAMESPACE        | The default namespace to use for the API              | default      |
+| SPARK_ON_K8S_API_HOST                     | The host to use for the API                           | 127.0.0.1    |
+| SPARK_ON_K8S_API_PORT                     | The port to use for the API                           | 8000         |
+| SPARK_ON_K8S_API_WORKERS                  | The number of workers to use for the API              | 4            |
+| SPARK_ON_K8S_API_LOG_LEVEL                | The log level to use for the API                      | info         |
+| SPARK_ON_K8S_API_LIMIT_CONCURRENCY        | The limit concurrency to use for the API              | 1000         |
+| SPARK_ON_K8S_API_SPARK_HISTORY_HOST       | The host to use for the spark history server          |              |
+| SPARK_ON_K8S_SPARK_DRIVER_NODE_SELECTOR   | The node selector to use for the driver pod           | {}           |
+| SPARK_ON_K8S_SPARK_EXECUTOR_NODE_SELECTOR | The node selector to use for the executor pods        | {}           |
+| SPARK_ON_K8S_SPARK_DRIVER_LABELS          | The labels to use for the driver pod                  | {}           |
+| SPARK_ON_K8S_SPARK_EXECUTOR_LABELS        | The labels to use for the executor pods               | {}           |
+| SPARK_ON_K8S_SPARK_DRIVER_ANNOTATIONS     | The annotations to use for the driver pod             | {}           |
+| SPARK_ON_K8S_SPARK_EXECUTOR_ANNOTATIONS   | The annotations to use for the executor pods          | {}           |
+| SPARK_ON_K8S_EXECUTOR_POD_TEMPLATE_PATH   | The path to the executor pod template                 |              |
 
 
 ## Examples
 
 Here are some examples of how to package and submit spark apps with this package. In the examples, the base image is
 built with the spark image tool, as described in the
 [spark documentation](https://spark.apache.org/docs/latest/running-on-kubernetes.html#docker-images).
```

