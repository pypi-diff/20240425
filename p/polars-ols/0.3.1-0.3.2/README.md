# Comparing `tmp/polars_ols-0.3.1.tar.gz` & `tmp/polars_ols-0.3.2.tar.gz`

## Comparing `polars_ols-0.3.1.tar` & `polars_ols-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1885 1970-01-01 00:00:00.000000 polars_ols-0.3.1/Cargo.toml
--rw-r--r--   0     1001      127     5579 2024-04-22 18:01:51.000000 polars_ols-0.3.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      139 2024-04-22 18:01:51.000000 polars_ols-0.3.1/.gitignore
--rw-r--r--   0     1001      127      912 2024-04-22 18:01:51.000000 polars_ols-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0     1001      127     1067 2024-04-22 18:01:51.000000 polars_ols-0.3.1/LICENSE
--rw-r--r--   0     1001      127      678 2024-04-22 18:01:51.000000 polars_ols-0.3.1/Makefile
--rw-r--r--   0     1001      127    15313 2024-04-22 18:01:51.000000 polars_ols-0.3.1/README.md
--rw-r--r--   0     1001      127    71469 2024-04-22 18:01:51.000000 polars_ols-0.3.1/notebooks/polars_ols_demo.ipynb
--rw-r--r--   0     1001      127    13029 2024-04-22 18:01:51.000000 polars_ols-0.3.1/polars_ols/__init__.py
--rw-r--r--   0     1001      127    17054 2024-04-22 18:01:51.000000 polars_ols-0.3.1/polars_ols/least_squares.py
--rw-r--r--   0     1001      127     3915 2024-04-22 18:01:51.000000 polars_ols-0.3.1/polars_ols/utils.py
--rw-r--r--   0     1001      127       64 2024-04-22 18:01:51.000000 polars_ols-0.3.1/requirements.txt
--rw-r--r--   0     1001      127       32 2024-04-22 18:01:51.000000 polars_ols-0.3.1/rust-toolchain.toml
--rw-r--r--   0     1001      127    20633 2024-04-22 18:01:51.000000 polars_ols-0.3.1/src/expressions.rs
--rw-r--r--   0     1001      127    34387 2024-04-22 18:01:51.000000 polars_ols-0.3.1/src/least_squares.rs
--rw-r--r--   0     1001      127     5853 2024-04-22 18:01:51.000000 polars_ols-0.3.1/src/lib.rs
--rw-r--r--   0     1001      127        0 2024-04-22 18:01:51.000000 polars_ols-0.3.1/tests/__init__.py
--rw-r--r--   0     1001      127     7820 2024-04-22 18:01:51.000000 polars_ols-0.3.1/tests/benchmark.py
--rw-r--r--   0     1001      127       87 2024-04-22 18:01:51.000000 polars_ols-0.3.1/tests/requirements-test.txt
--rw-r--r--   0     1001      127    31369 2024-04-22 18:01:51.000000 polars_ols-0.3.1/tests/test_ols.py
--rw-r--r--   0     1001      127    78185 2024-04-22 18:02:06.000000 polars_ols-0.3.1/Cargo.lock
--rw-r--r--   0     1001      127     1865 2024-04-22 18:01:51.000000 polars_ols-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    16021 1970-01-01 00:00:00.000000 polars_ols-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1885 1970-01-01 00:00:00.000000 polars_ols-0.3.2/Cargo.toml
+-rw-r--r--   0     1001      127     5579 2024-04-25 20:31:59.000000 polars_ols-0.3.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      139 2024-04-25 20:31:59.000000 polars_ols-0.3.2/.gitignore
+-rw-r--r--   0     1001      127      912 2024-04-25 20:31:59.000000 polars_ols-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127     1067 2024-04-25 20:31:59.000000 polars_ols-0.3.2/LICENSE
+-rw-r--r--   0     1001      127      678 2024-04-25 20:31:59.000000 polars_ols-0.3.2/Makefile
+-rw-r--r--   0     1001      127    15313 2024-04-25 20:31:59.000000 polars_ols-0.3.2/README.md
+-rw-r--r--   0     1001      127    82321 2024-04-25 20:31:59.000000 polars_ols-0.3.2/notebooks/polars_ols_demo.ipynb
+-rw-r--r--   0     1001      127    13543 2024-04-25 20:31:59.000000 polars_ols-0.3.2/polars_ols/__init__.py
+-rw-r--r--   0     1001      127    19123 2024-04-25 20:31:59.000000 polars_ols-0.3.2/polars_ols/least_squares.py
+-rw-r--r--   0     1001      127     3915 2024-04-25 20:31:59.000000 polars_ols-0.3.2/polars_ols/utils.py
+-rw-r--r--   0     1001      127       64 2024-04-25 20:31:59.000000 polars_ols-0.3.2/requirements.txt
+-rw-r--r--   0     1001      127       32 2024-04-25 20:31:59.000000 polars_ols-0.3.2/rust-toolchain.toml
+-rw-r--r--   0     1001      127    24154 2024-04-25 20:31:59.000000 polars_ols-0.3.2/src/expressions.rs
+-rw-r--r--   0     1001      127    35767 2024-04-25 20:31:59.000000 polars_ols-0.3.2/src/least_squares.rs
+-rw-r--r--   0     1001      127     5853 2024-04-25 20:31:59.000000 polars_ols-0.3.2/src/lib.rs
+-rw-r--r--   0     1001      127        0 2024-04-25 20:31:59.000000 polars_ols-0.3.2/tests/__init__.py
+-rw-r--r--   0     1001      127     9412 2024-04-25 20:31:59.000000 polars_ols-0.3.2/tests/benchmark.py
+-rw-r--r--   0     1001      127       87 2024-04-25 20:31:59.000000 polars_ols-0.3.2/tests/requirements-test.txt
+-rw-r--r--   0     1001      127    32589 2024-04-25 20:31:59.000000 polars_ols-0.3.2/tests/test_ols.py
+-rw-r--r--   0     1001      127    78185 2024-04-25 20:32:13.000000 polars_ols-0.3.2/Cargo.lock
+-rw-r--r--   0     1001      127     1865 2024-04-25 20:31:59.000000 polars_ols-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    16021 1970-01-01 00:00:00.000000 polars_ols-0.3.2/PKG-INFO
```

### Comparing `polars_ols-0.3.1/Cargo.toml` & `polars_ols-0.3.2/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 cargo-features = ["profile-rustflags"]
 
 [package]
 name = "polars_ols"
-version = "0.3.1"
+version = "0.3.2"
 edition = "2021"
 
 [lib]
 name = "polars_ols"
 crate-type = ["cdylib"]
 
 [dependencies]
```

### Comparing `polars_ols-0.3.1/.github/workflows/CI.yml` & `polars_ols-0.3.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `polars_ols-0.3.1/.pre-commit-config.yaml` & `polars_ols-0.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `polars_ols-0.3.1/LICENSE` & `polars_ols-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_ols-0.3.1/Makefile` & `polars_ols-0.3.2/Makefile`

 * *Files identical despite different names*

### Comparing `polars_ols-0.3.1/README.md` & `polars_ols-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `polars_ols-0.3.1/notebooks/polars_ols_demo.ipynb` & `polars_ols-0.3.2/notebooks/polars_ols_demo.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9904030866539358%*

 * *Differences: {"'cells'": "{0: {'metadata': {'execution': {'iopub.execute_input': '2024-04-25T17:42:58.884510Z', "*

 * *            "'iopub.status.busy': '2024-04-25T17:42:58.884072Z', 'iopub.status.idle': "*

 * *            "'2024-04-25T17:42:58.997067Z', 'shell.execute_reply': '2024-04-25T17:42:58.996495Z', "*

 * *            "'shell.execute_reply.started': '2024-04-25T17:42:58.884482Z'}}}, 1: {'metadata': "*

 * *            "{'execution': {'iopub.execute_input': '2024-04-25T17:42:59.178866Z', "*

 * *            "'iopub.status.busy': '2024-04- […]*

```diff
@@ -2,19 +2,19 @@
     "cells": [
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "8d7bae54-e858-410c-a574-da1aa325d90a",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:52:52.460965Z",
-                    "iopub.status.busy": "2024-04-22T17:52:52.460792Z",
-                    "iopub.status.idle": "2024-04-22T17:52:52.551749Z",
-                    "shell.execute_reply": "2024-04-22T17:52:52.551071Z",
-                    "shell.execute_reply.started": "2024-04-22T17:52:52.460951Z"
+                    "iopub.execute_input": "2024-04-25T17:42:58.884510Z",
+                    "iopub.status.busy": "2024-04-25T17:42:58.884072Z",
+                    "iopub.status.idle": "2024-04-25T17:42:58.997067Z",
+                    "shell.execute_reply": "2024-04-25T17:42:58.996495Z",
+                    "shell.execute_reply.started": "2024-04-25T17:42:58.884482Z"
                 }
             },
             "outputs": [],
             "source": [
                 "import os; os.environ[\"POLARS_VERBOSE\"] = \"1\"\n",
                 "import polars as pl\n",
                 "import polars_ols as pls\n",
@@ -23,19 +23,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "35076da5-137a-4d90-a671-ed1e9d650930",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:52:52.707925Z",
-                    "iopub.status.busy": "2024-04-22T17:52:52.707584Z",
-                    "iopub.status.idle": "2024-04-22T17:52:52.716339Z",
-                    "shell.execute_reply": "2024-04-22T17:52:52.715460Z",
-                    "shell.execute_reply.started": "2024-04-22T17:52:52.707901Z"
+                    "iopub.execute_input": "2024-04-25T17:42:59.178866Z",
+                    "iopub.status.busy": "2024-04-25T17:42:59.177794Z",
+                    "iopub.status.idle": "2024-04-25T17:42:59.193372Z",
+                    "shell.execute_reply": "2024-04-25T17:42:59.188864Z",
+                    "shell.execute_reply.started": "2024-04-25T17:42:59.178827Z"
                 }
             },
             "outputs": [],
             "source": [
                 "rng = np.random.default_rng(0)\n",
                 "\n",
                 "def insert_nulls(val):\n",
@@ -66,19 +66,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "5ad1869e-d884-48e2-8f37-f790057ada1a",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:52:53.086757Z",
-                    "iopub.status.busy": "2024-04-22T17:52:53.086450Z",
-                    "iopub.status.idle": "2024-04-22T17:52:53.090536Z",
-                    "shell.execute_reply": "2024-04-22T17:52:53.090160Z",
-                    "shell.execute_reply.started": "2024-04-22T17:52:53.086745Z"
+                    "iopub.execute_input": "2024-04-25T17:42:59.881263Z",
+                    "iopub.status.busy": "2024-04-25T17:42:59.880780Z",
+                    "iopub.status.idle": "2024-04-25T17:42:59.888232Z",
+                    "shell.execute_reply": "2024-04-25T17:42:59.887741Z",
+                    "shell.execute_reply.started": "2024-04-25T17:42:59.881235Z"
                 }
             },
             "outputs": [],
             "source": [
                 "df = _make_data(n_samples=2_000, n_features=3, n_groups=5)"
             ]
         },
@@ -98,19 +98,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "id": "f7604a81-cf0b-41ab-b39b-4cd6282797af",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:52:53.470288Z",
-                    "iopub.status.busy": "2024-04-22T17:52:53.470000Z",
-                    "iopub.status.idle": "2024-04-22T17:52:53.495235Z",
-                    "shell.execute_reply": "2024-04-22T17:52:53.494788Z",
-                    "shell.execute_reply.started": "2024-04-22T17:52:53.470273Z"
+                    "iopub.execute_input": "2024-04-25T17:43:00.574656Z",
+                    "iopub.status.busy": "2024-04-25T17:43:00.574219Z",
+                    "iopub.status.idle": "2024-04-25T17:43:00.621773Z",
+                    "shell.execute_reply": "2024-04-25T17:43:00.621217Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:00.574627Z"
                 },
                 "scrolled": true
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
@@ -159,19 +159,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "c7748165-bc22-4c0d-98d0-a7813d211449",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:52:53.638774Z",
-                    "iopub.status.busy": "2024-04-22T17:52:53.638593Z",
-                    "iopub.status.idle": "2024-04-22T17:52:53.643090Z",
-                    "shell.execute_reply": "2024-04-22T17:52:53.642763Z",
-                    "shell.execute_reply.started": "2024-04-22T17:52:53.638761Z"
+                    "iopub.execute_input": "2024-04-25T17:43:00.947207Z",
+                    "iopub.status.busy": "2024-04-25T17:43:00.946753Z",
+                    "iopub.status.idle": "2024-04-25T17:43:00.956159Z",
+                    "shell.execute_reply": "2024-04-25T17:43:00.955383Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:00.947179Z"
                 }
             },
             "outputs": [],
             "source": [
                 "# you can use the function 'compute_least_squares'\n",
                 "ols_expr = pls.compute_least_squares(pl.col(\"y\"),  # target\n",
                 "                          pl.selectors.starts_with(\"x\"),  # features - can use wildcard expressions or multiple feature expressions/names\n",
@@ -199,19 +199,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "id": "c824074b-cecd-43ef-a8b9-bfaeb44f77ad",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:52:54.087503Z",
-                    "iopub.status.busy": "2024-04-22T17:52:54.087329Z",
-                    "iopub.status.idle": "2024-04-22T17:52:54.100681Z",
-                    "shell.execute_reply": "2024-04-22T17:52:54.100236Z",
-                    "shell.execute_reply.started": "2024-04-22T17:52:54.087488Z"
+                    "iopub.execute_input": "2024-04-25T17:43:01.498312Z",
+                    "iopub.status.busy": "2024-04-25T17:43:01.498014Z",
+                    "iopub.status.idle": "2024-04-25T17:43:01.517574Z",
+                    "shell.execute_reply": "2024-04-25T17:43:01.517156Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:01.498293Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
@@ -269,19 +269,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "id": "8b14b8ac-c34c-449c-a109-5198ee01e06e",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:52:54.626201Z",
-                    "iopub.status.busy": "2024-04-22T17:52:54.625912Z",
-                    "iopub.status.idle": "2024-04-22T17:52:54.652919Z",
-                    "shell.execute_reply": "2024-04-22T17:52:54.652647Z",
-                    "shell.execute_reply.started": "2024-04-22T17:52:54.626177Z"
+                    "iopub.execute_input": "2024-04-25T17:43:02.041125Z",
+                    "iopub.status.busy": "2024-04-25T17:43:02.040386Z",
+                    "iopub.status.idle": "2024-04-25T17:43:02.053982Z",
+                    "shell.execute_reply": "2024-04-25T17:43:02.053292Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:02.041075Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
@@ -326,19 +326,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "id": "4271adf2-6cb4-46ee-90c7-4e1ac1d28d93",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:52:55.093128Z",
-                    "iopub.status.busy": "2024-04-22T17:52:55.092923Z",
-                    "iopub.status.idle": "2024-04-22T17:52:55.099203Z",
-                    "shell.execute_reply": "2024-04-22T17:52:55.098880Z",
-                    "shell.execute_reply.started": "2024-04-22T17:52:55.093108Z"
+                    "iopub.execute_input": "2024-04-25T17:43:02.609745Z",
+                    "iopub.status.busy": "2024-04-25T17:43:02.609300Z",
+                    "iopub.status.idle": "2024-04-25T17:43:02.622906Z",
+                    "shell.execute_reply": "2024-04-25T17:43:02.622154Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:02.609719Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -398,70 +398,70 @@
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "id": "e67f6d5f-89fe-44cb-8b8e-4d67cc8323e6",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:52:55.946208Z",
-                    "iopub.status.busy": "2024-04-22T17:52:55.945919Z",
-                    "iopub.status.idle": "2024-04-22T17:52:56.000325Z",
-                    "shell.execute_reply": "2024-04-22T17:52:55.997692Z",
-                    "shell.execute_reply.started": "2024-04-22T17:52:55.946174Z"
+                    "iopub.execute_input": "2024-04-25T17:43:03.962050Z",
+                    "iopub.status.busy": "2024-04-25T17:43:03.961579Z",
+                    "iopub.status.idle": "2024-04-25T17:43:03.986651Z",
+                    "shell.execute_reply": "2024-04-25T17:43:03.986223Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:03.962021Z"
                 }
             },
             "outputs": [],
             "source": [
                 "df_missing = _make_data(missing=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "id": "92e17a52-16b5-4f0f-ae87-dbf2d0a402c1",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:52:56.138821Z",
-                    "iopub.status.busy": "2024-04-22T17:52:56.138659Z",
-                    "iopub.status.idle": "2024-04-22T17:52:56.142457Z",
-                    "shell.execute_reply": "2024-04-22T17:52:56.141989Z",
-                    "shell.execute_reply.started": "2024-04-22T17:52:56.138808Z"
+                    "iopub.execute_input": "2024-04-25T17:43:04.174480Z",
+                    "iopub.status.busy": "2024-04-25T17:43:04.173771Z",
+                    "iopub.status.idle": "2024-04-25T17:43:04.184481Z",
+                    "shell.execute_reply": "2024-04-25T17:43:04.183813Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:04.174431Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (2_000, 8)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>x1</th><th>x2</th><th>x3</th><th>x4</th><th>x5</th><th>y</th><th>group</th><th>sample_weights</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>0.12573</td><td>-0.132105</td><td>0.640423</td><td>0.1049</td><td>-0.535669</td><td>-0.154338</td><td>2.0</td><td>0.313882</td></tr><tr><td>0.361595</td><td>1.304</td><td>0.947081</td><td>-0.703735</td><td>null</td><td>-0.777174</td><td>1.0</td><td>0.215647</td></tr><tr><td>null</td><td>0.041326</td><td>-2.325031</td><td>null</td><td>-1.245911</td><td>4.260299</td><td>0.0</td><td>0.975329</td></tr><tr><td>null</td><td>-0.544259</td><td>-0.3163</td><td>0.411631</td><td>1.042513</td><td>0.093387</td><td>1.0</td><td>0.349839</td></tr><tr><td>-0.128535</td><td>1.366463</td><td>-0.665195</td><td>0.35151</td><td>null</td><td>-1.659732</td><td>1.0</td><td>0.180044</td></tr><tr><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td></tr><tr><td>null</td><td>0.433351</td><td>null</td><td>0.659305</td><td>0.346436</td><td>null</td><td>2.0</td><td>0.921171</td></tr><tr><td>0.73432</td><td>-0.562784</td><td>0.642383</td><td>-0.328101</td><td>-0.704787</td><td>0.239824</td><td>1.0</td><td>0.930792</td></tr><tr><td>-0.880797</td><td>-0.497476</td><td>-0.464837</td><td>1.577698</td><td>0.045559</td><td>0.249027</td><td>1.0</td><td>0.120942</td></tr><tr><td>null</td><td>0.479883</td><td>null</td><td>-0.459391</td><td>null</td><td>-0.395502</td><td>2.0</td><td>0.86176</td></tr><tr><td>1.338043</td><td>null</td><td>-0.416367</td><td>-1.266301</td><td>1.031231</td><td>-0.20221</td><td>1.0</td><td>null</td></tr></tbody></table></div>"
+                            "<small>shape: (2_000, 8)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>x1</th><th>x2</th><th>x3</th><th>x4</th><th>x5</th><th>y</th><th>group</th><th>sample_weights</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>0.12573</td><td>-0.132105</td><td>0.640423</td><td>0.1049</td><td>-0.535669</td><td>-0.154338</td><td>2.0</td><td>0.313882</td></tr><tr><td>0.361595</td><td>1.304</td><td>0.947081</td><td>-0.703735</td><td>null</td><td>-0.777174</td><td>1.0</td><td>0.215647</td></tr><tr><td>null</td><td>null</td><td>-2.325031</td><td>-0.218792</td><td>-1.245911</td><td>4.260299</td><td>0.0</td><td>0.975329</td></tr><tr><td>null</td><td>-0.544259</td><td>-0.3163</td><td>0.411631</td><td>1.042513</td><td>0.093387</td><td>1.0</td><td>0.349839</td></tr><tr><td>-0.128535</td><td>1.366463</td><td>-0.665195</td><td>0.35151</td><td>null</td><td>-1.659732</td><td>1.0</td><td>0.180044</td></tr><tr><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td></tr><tr><td>null</td><td>0.433351</td><td>-1.199857</td><td>null</td><td>0.346436</td><td>null</td><td>2.0</td><td>0.921171</td></tr><tr><td>0.73432</td><td>-0.562784</td><td>0.642383</td><td>-0.328101</td><td>-0.704787</td><td>0.239824</td><td>1.0</td><td>0.930792</td></tr><tr><td>-0.880797</td><td>-0.497476</td><td>-0.464837</td><td>1.577698</td><td>0.045559</td><td>0.249027</td><td>1.0</td><td>0.120942</td></tr><tr><td>null</td><td>0.479883</td><td>0.611798</td><td>null</td><td>null</td><td>-0.395502</td><td>2.0</td><td>0.86176</td></tr><tr><td>1.338043</td><td>-0.443767</td><td>null</td><td>-1.266301</td><td>1.031231</td><td>-0.20221</td><td>1.0</td><td>null</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (2_000, 8)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 x1        \u2506 x2        \u2506 x3        \u2506 x4        \u2506 x5        \u2506 y         \u2506 group \u2506 sample_weights \u2502\n",
                             "\u2502 ---       \u2506 ---       \u2506 ---       \u2506 ---       \u2506 ---       \u2506 ---       \u2506 ---   \u2506 ---            \u2502\n",
                             "\u2502 f64       \u2506 f64       \u2506 f64       \u2506 f64       \u2506 f64       \u2506 f64       \u2506 f64   \u2506 f64            \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
                             "\u2502 0.12573   \u2506 -0.132105 \u2506 0.640423  \u2506 0.1049    \u2506 -0.535669 \u2506 -0.154338 \u2506 2.0   \u2506 0.313882       \u2502\n",
                             "\u2502 0.361595  \u2506 1.304     \u2506 0.947081  \u2506 -0.703735 \u2506 null      \u2506 -0.777174 \u2506 1.0   \u2506 0.215647       \u2502\n",
-                            "\u2502 null      \u2506 0.041326  \u2506 -2.325031 \u2506 null      \u2506 -1.245911 \u2506 4.260299  \u2506 0.0   \u2506 0.975329       \u2502\n",
+                            "\u2502 null      \u2506 null      \u2506 -2.325031 \u2506 -0.218792 \u2506 -1.245911 \u2506 4.260299  \u2506 0.0   \u2506 0.975329       \u2502\n",
                             "\u2502 null      \u2506 -0.544259 \u2506 -0.3163   \u2506 0.411631  \u2506 1.042513  \u2506 0.093387  \u2506 1.0   \u2506 0.349839       \u2502\n",
                             "\u2502 -0.128535 \u2506 1.366463  \u2506 -0.665195 \u2506 0.35151   \u2506 null      \u2506 -1.659732 \u2506 1.0   \u2506 0.180044       \u2502\n",
                             "\u2502 \u2026         \u2506 \u2026         \u2506 \u2026         \u2506 \u2026         \u2506 \u2026         \u2506 \u2026         \u2506 \u2026     \u2506 \u2026              \u2502\n",
-                            "\u2502 null      \u2506 0.433351  \u2506 null      \u2506 0.659305  \u2506 0.346436  \u2506 null      \u2506 2.0   \u2506 0.921171       \u2502\n",
+                            "\u2502 null      \u2506 0.433351  \u2506 -1.199857 \u2506 null      \u2506 0.346436  \u2506 null      \u2506 2.0   \u2506 0.921171       \u2502\n",
                             "\u2502 0.73432   \u2506 -0.562784 \u2506 0.642383  \u2506 -0.328101 \u2506 -0.704787 \u2506 0.239824  \u2506 1.0   \u2506 0.930792       \u2502\n",
                             "\u2502 -0.880797 \u2506 -0.497476 \u2506 -0.464837 \u2506 1.577698  \u2506 0.045559  \u2506 0.249027  \u2506 1.0   \u2506 0.120942       \u2502\n",
-                            "\u2502 null      \u2506 0.479883  \u2506 null      \u2506 -0.459391 \u2506 null      \u2506 -0.395502 \u2506 2.0   \u2506 0.86176        \u2502\n",
-                            "\u2502 1.338043  \u2506 null      \u2506 -0.416367 \u2506 -1.266301 \u2506 1.031231  \u2506 -0.20221  \u2506 1.0   \u2506 null           \u2502\n",
+                            "\u2502 null      \u2506 0.479883  \u2506 0.611798  \u2506 null      \u2506 null      \u2506 -0.395502 \u2506 2.0   \u2506 0.86176        \u2502\n",
+                            "\u2502 1.338043  \u2506 -0.443767 \u2506 null      \u2506 -1.266301 \u2506 1.031231  \u2506 -0.20221  \u2506 1.0   \u2506 null           \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -472,19 +472,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "id": "527c85d6-0054-44ac-a099-dcb7068b2f3f",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:52:56.330351Z",
-                    "iopub.status.busy": "2024-04-22T17:52:56.330133Z",
-                    "iopub.status.idle": "2024-04-22T17:52:56.333519Z",
-                    "shell.execute_reply": "2024-04-22T17:52:56.332947Z",
-                    "shell.execute_reply.started": "2024-04-22T17:52:56.330335Z"
+                    "iopub.execute_input": "2024-04-25T17:43:04.533718Z",
+                    "iopub.status.busy": "2024-04-25T17:43:04.533291Z",
+                    "iopub.status.idle": "2024-04-25T17:43:04.538348Z",
+                    "shell.execute_reply": "2024-04-25T17:43:04.537800Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:04.533693Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "typing.Literal['zero', 'drop', 'ignore', 'drop_zero', 'drop_y_zero_x', 'drop_window']"
@@ -509,38 +509,38 @@
         },
         {
             "cell_type": "code",
             "execution_count": 12,
             "id": "a4d04c0b-f464-456f-b292-c0576718ddf9",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:52:56.820409Z",
-                    "iopub.status.busy": "2024-04-22T17:52:56.820230Z",
-                    "iopub.status.idle": "2024-04-22T17:52:56.826103Z",
-                    "shell.execute_reply": "2024-04-22T17:52:56.825776Z",
-                    "shell.execute_reply.started": "2024-04-22T17:52:56.820393Z"
+                    "iopub.execute_input": "2024-04-25T17:43:05.013674Z",
+                    "iopub.status.busy": "2024-04-25T17:43:05.013240Z",
+                    "iopub.status.idle": "2024-04-25T17:43:05.025901Z",
+                    "shell.execute_reply": "2024-04-25T17:43:05.025161Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:05.013648Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "shape: (5, 1)\n",
-                        "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
-                        "\u2502 y         \u2502\n",
-                        "\u2502 ---       \u2502\n",
-                        "\u2502 f64       \u2502\n",
-                        "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                        "\u2502 null      \u2502\n",
-                        "\u2502 0.081255  \u2502\n",
-                        "\u2502 0.026447  \u2502\n",
-                        "\u2502 -0.377051 \u2502\n",
-                        "\u2502 0.409127  \u2502\n",
-                        "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518\n"
+                        "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                        "\u2502 y        \u2502\n",
+                        "\u2502 ---      \u2502\n",
+                        "\u2502 f64      \u2502\n",
+                        "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                        "\u2502 null     \u2502\n",
+                        "\u2502 0.082407 \u2502\n",
+                        "\u2502 0.06314  \u2502\n",
+                        "\u2502 0.571505 \u2502\n",
+                        "\u2502 0.419788 \u2502\n",
+                        "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518\n"
                     ]
                 }
             ],
             "source": [
                 "pred_zero = df_missing.select(\n",
                 "    pls.compute_least_squares(\"y\", pl.selectors.starts_with(\"x\"), \n",
                 "                              mode=\"predictions\",\n",
@@ -579,19 +579,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": 13,
             "id": "9a605974-3218-4dea-929d-71752577d018",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:52:57.353780Z",
-                    "iopub.status.busy": "2024-04-22T17:52:57.353532Z",
-                    "iopub.status.idle": "2024-04-22T17:52:57.361291Z",
-                    "shell.execute_reply": "2024-04-22T17:52:57.360911Z",
-                    "shell.execute_reply.started": "2024-04-22T17:52:57.353759Z"
+                    "iopub.execute_input": "2024-04-25T17:43:05.639743Z",
+                    "iopub.status.busy": "2024-04-25T17:43:05.639233Z",
+                    "iopub.status.idle": "2024-04-25T17:43:05.651328Z",
+                    "shell.execute_reply": "2024-04-25T17:43:05.650462Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:05.639712Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
@@ -633,19 +633,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": 14,
             "id": "9966577c-e91f-4fdd-88c6-bd26ee2b63b8",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:52:57.957569Z",
-                    "iopub.status.busy": "2024-04-22T17:52:57.957371Z",
-                    "iopub.status.idle": "2024-04-22T17:52:57.963563Z",
-                    "shell.execute_reply": "2024-04-22T17:52:57.963259Z",
-                    "shell.execute_reply.started": "2024-04-22T17:52:57.957554Z"
+                    "iopub.execute_input": "2024-04-25T17:43:06.388226Z",
+                    "iopub.status.busy": "2024-04-25T17:43:06.387787Z",
+                    "iopub.status.idle": "2024-04-25T17:43:06.399037Z",
+                    "shell.execute_reply": "2024-04-25T17:43:06.398286Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:06.388201Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
@@ -670,19 +670,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": 15,
             "id": "e1454e57-7a21-4da2-a525-233eda2c2d8b",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:52:58.278029Z",
-                    "iopub.status.busy": "2024-04-22T17:52:58.277781Z",
-                    "iopub.status.idle": "2024-04-22T17:52:58.281106Z",
-                    "shell.execute_reply": "2024-04-22T17:52:58.280662Z",
-                    "shell.execute_reply.started": "2024-04-22T17:52:58.278008Z"
+                    "iopub.execute_input": "2024-04-25T17:43:06.905749Z",
+                    "iopub.status.busy": "2024-04-25T17:43:06.905410Z",
+                    "iopub.status.idle": "2024-04-25T17:43:06.909660Z",
+                    "shell.execute_reply": "2024-04-25T17:43:06.909155Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:06.905727Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "typing.Literal['qr', 'svd', 'chol', 'lu', 'cd', 'cd_active_set']"
@@ -721,19 +721,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": 16,
             "id": "2ab3d26e-aaea-4869-9a4d-393288409f7d",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:52:59.297817Z",
-                    "iopub.status.busy": "2024-04-22T17:52:59.297321Z",
-                    "iopub.status.idle": "2024-04-22T17:52:59.304207Z",
-                    "shell.execute_reply": "2024-04-22T17:52:59.303417Z",
-                    "shell.execute_reply.started": "2024-04-22T17:52:59.297797Z"
+                    "iopub.execute_input": "2024-04-25T17:43:08.187603Z",
+                    "iopub.status.busy": "2024-04-25T17:43:08.187153Z",
+                    "iopub.status.idle": "2024-04-25T17:43:08.192389Z",
+                    "shell.execute_reply": "2024-04-25T17:43:08.191846Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:08.187577Z"
                 }
             },
             "outputs": [],
             "source": [
                 "df_collinear = (\n",
                 "    df\n",
                 "    .select(\"x1\", \"x2\", \"x3\")\n",
@@ -752,19 +752,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": 17,
             "id": "ef238917-1c96-4ed0-ad6e-eca4f1bf7b34",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:52:59.916023Z",
-                    "iopub.status.busy": "2024-04-22T17:52:59.915843Z",
-                    "iopub.status.idle": "2024-04-22T17:52:59.920547Z",
-                    "shell.execute_reply": "2024-04-22T17:52:59.920218Z",
-                    "shell.execute_reply.started": "2024-04-22T17:52:59.916011Z"
+                    "iopub.execute_input": "2024-04-25T17:43:08.946456Z",
+                    "iopub.status.busy": "2024-04-25T17:43:08.946042Z",
+                    "iopub.status.idle": "2024-04-25T17:43:08.954321Z",
+                    "shell.execute_reply": "2024-04-25T17:43:08.953706Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:08.946432Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -796,19 +796,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": 18,
             "id": "76ae5386-d457-48e1-847a-ff31b881bf61",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:53:00.579546Z",
-                    "iopub.status.busy": "2024-04-22T17:53:00.579234Z",
-                    "iopub.status.idle": "2024-04-22T17:53:00.585891Z",
-                    "shell.execute_reply": "2024-04-22T17:53:00.585584Z",
-                    "shell.execute_reply.started": "2024-04-22T17:53:00.579529Z"
+                    "iopub.execute_input": "2024-04-25T17:43:09.620185Z",
+                    "iopub.status.busy": "2024-04-25T17:43:09.619734Z",
+                    "iopub.status.idle": "2024-04-25T17:43:09.630995Z",
+                    "shell.execute_reply": "2024-04-25T17:43:09.630532Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:09.620159Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -857,19 +857,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": 19,
             "id": "943b6e4d-09b0-410a-b571-85497907eb57",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:53:01.174401Z",
-                    "iopub.status.busy": "2024-04-22T17:53:01.174152Z",
-                    "iopub.status.idle": "2024-04-22T17:53:01.179057Z",
-                    "shell.execute_reply": "2024-04-22T17:53:01.178706Z",
-                    "shell.execute_reply.started": "2024-04-22T17:53:01.174387Z"
+                    "iopub.execute_input": "2024-04-25T17:43:10.252089Z",
+                    "iopub.status.busy": "2024-04-25T17:43:10.251654Z",
+                    "iopub.status.idle": "2024-04-25T17:43:10.262793Z",
+                    "shell.execute_reply": "2024-04-25T17:43:10.261609Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:10.252062Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
@@ -919,19 +919,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": 20,
             "id": "bcb50dae-4325-46c6-a939-4bc3ec48633a",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:53:02.035744Z",
-                    "iopub.status.busy": "2024-04-22T17:53:02.035577Z",
-                    "iopub.status.idle": "2024-04-22T17:53:02.039188Z",
-                    "shell.execute_reply": "2024-04-22T17:53:02.038816Z",
-                    "shell.execute_reply.started": "2024-04-22T17:53:02.035731Z"
+                    "iopub.execute_input": "2024-04-25T17:43:11.307722Z",
+                    "iopub.status.busy": "2024-04-25T17:43:11.307119Z",
+                    "iopub.status.idle": "2024-04-25T17:43:11.314434Z",
+                    "shell.execute_reply": "2024-04-25T17:43:11.313739Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:11.307692Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([1., 1., 1.])"
@@ -966,19 +966,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": 21,
             "id": "e35fbf57-3edb-4450-bcf7-a6c2aeef1e6f",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:53:02.800514Z",
-                    "iopub.status.busy": "2024-04-22T17:53:02.800172Z",
-                    "iopub.status.idle": "2024-04-22T17:53:02.806164Z",
-                    "shell.execute_reply": "2024-04-22T17:53:02.805877Z",
-                    "shell.execute_reply.started": "2024-04-22T17:53:02.800499Z"
+                    "iopub.execute_input": "2024-04-25T17:43:12.870745Z",
+                    "iopub.status.busy": "2024-04-25T17:43:12.870321Z",
+                    "iopub.status.idle": "2024-04-25T17:43:12.883332Z",
+                    "shell.execute_reply": "2024-04-25T17:43:12.882600Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:12.870720Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
@@ -1033,56 +1033,56 @@
         },
         {
             "cell_type": "code",
             "execution_count": 22,
             "id": "e81f59b7-5c81-4cc5-9f5f-06fd0ef8b90b",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:53:04.108677Z",
-                    "iopub.status.busy": "2024-04-22T17:53:04.108504Z",
-                    "iopub.status.idle": "2024-04-22T17:53:04.548357Z",
-                    "shell.execute_reply": "2024-04-22T17:53:04.547978Z",
-                    "shell.execute_reply.started": "2024-04-22T17:53:04.108663Z"
+                    "iopub.execute_input": "2024-04-25T17:43:13.398423Z",
+                    "iopub.status.busy": "2024-04-25T17:43:13.397966Z",
+                    "iopub.status.idle": "2024-04-25T17:43:13.747421Z",
+                    "shell.execute_reply": "2024-04-25T17:43:13.747110Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:13.398393Z"
                 }
             },
             "outputs": [],
             "source": [
                 "from sklearn.linear_model import ElasticNet"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 46,
+            "execution_count": 23,
             "id": "95136952-e737-4c58-a86c-7c14ce085169",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:58:17.454692Z",
-                    "iopub.status.busy": "2024-04-22T17:58:17.454451Z",
-                    "iopub.status.idle": "2024-04-22T17:58:17.472629Z",
-                    "shell.execute_reply": "2024-04-22T17:58:17.472265Z",
-                    "shell.execute_reply.started": "2024-04-22T17:58:17.454679Z"
+                    "iopub.execute_input": "2024-04-25T17:43:13.748154Z",
+                    "iopub.status.busy": "2024-04-25T17:43:13.748058Z",
+                    "iopub.status.idle": "2024-04-25T17:43:13.760530Z",
+                    "shell.execute_reply": "2024-04-25T17:43:13.760250Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:13.748147Z"
                 }
             },
             "outputs": [],
             "source": [
                 "df_wide = _make_data(n_samples=1_000, n_features=1_000, sparsity=0.9)\n",
                 "features = [pl.col(f\"x{i+1}\") for i in range(1_000)]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 52,
+            "execution_count": 24,
             "id": "892cc6d9-3e6c-45d7-ae52-f66014d94a5d",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:59:24.217475Z",
-                    "iopub.status.busy": "2024-04-22T17:59:24.217222Z",
-                    "iopub.status.idle": "2024-04-22T17:59:24.324690Z",
-                    "shell.execute_reply": "2024-04-22T17:59:24.324081Z",
-                    "shell.execute_reply.started": "2024-04-22T17:59:24.217461Z"
+                    "iopub.execute_input": "2024-04-25T17:43:13.828227Z",
+                    "iopub.status.busy": "2024-04-25T17:43:13.828075Z",
+                    "iopub.status.idle": "2024-04-25T17:43:13.901990Z",
+                    "shell.execute_reply": "2024-04-25T17:43:13.901482Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:13.828215Z"
                 }
             },
             "outputs": [],
             "source": [
                 "# implementation matches sklearn \n",
                 "coef = df_wide.select(pl.col(\"y\").least_squares.elastic_net(\n",
                 "    *features,\n",
@@ -1099,31 +1099,31 @@
                 "mdl.fit(x, y)\n",
                 "\n",
                 "assert np.allclose(mdl.coef_, coef.to_numpy(), rtol=1.e-4, atol=1.e-4)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 53,
+            "execution_count": 25,
             "id": "0cbb5c0d-5093-4125-825a-c8f6e7c2083d",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:59:24.873713Z",
-                    "iopub.status.busy": "2024-04-22T17:59:24.873412Z",
-                    "iopub.status.idle": "2024-04-22T17:59:31.285254Z",
-                    "shell.execute_reply": "2024-04-22T17:59:31.284434Z",
-                    "shell.execute_reply.started": "2024-04-22T17:59:24.873693Z"
+                    "iopub.execute_input": "2024-04-25T17:43:14.048807Z",
+                    "iopub.status.busy": "2024-04-25T17:43:14.047868Z",
+                    "iopub.status.idle": "2024-04-25T17:43:17.569604Z",
+                    "shell.execute_reply": "2024-04-25T17:43:17.569354Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:14.048787Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "45.7 ms \u00b1 3.26 ms per loop (mean \u00b1 std. dev. of 7 runs, 20 loops each)\n"
+                        "25.1 ms \u00b1 795 \u00b5s per loop (mean \u00b1 std. dev. of 7 runs, 20 loops each)\n"
                     ]
                 }
             ],
             "source": [
                 "%%timeit -n 20\n",
                 "df_wide.with_columns(pl.col(\"y\").least_squares.elastic_net(\n",
                 "    *features,\n",
@@ -1134,31 +1134,31 @@
                 "    max_iter=1_000,\n",
                 "    tol=0.0001,\n",
                 ").alias(\"predictions\"))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 54,
+            "execution_count": 26,
             "id": "1adbc415-672d-41cc-ba70-7efc98c952ff",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:59:31.286509Z",
-                    "iopub.status.busy": "2024-04-22T17:59:31.286355Z",
-                    "iopub.status.idle": "2024-04-22T17:59:34.255025Z",
-                    "shell.execute_reply": "2024-04-22T17:59:34.254677Z",
-                    "shell.execute_reply.started": "2024-04-22T17:59:31.286495Z"
+                    "iopub.execute_input": "2024-04-25T17:43:17.570341Z",
+                    "iopub.status.busy": "2024-04-25T17:43:17.570262Z",
+                    "iopub.status.idle": "2024-04-25T17:43:19.144026Z",
+                    "shell.execute_reply": "2024-04-25T17:43:19.143767Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:17.570333Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "21.2 ms \u00b1 4.02 ms per loop (mean \u00b1 std. dev. of 7 runs, 20 loops each)\n"
+                        "11.2 ms \u00b1 305 \u00b5s per loop (mean \u00b1 std. dev. of 7 runs, 20 loops each)\n"
                     ]
                 }
             ],
             "source": [
                 "%%timeit -n 20\n",
                 "df_wide.with_columns(pl.col(\"y\").least_squares.elastic_net(\n",
                 "    *features,\n",
@@ -1181,23 +1181,23 @@
                 "- For those who like specifying models in patsy formula syntax, that is also supported\n",
                 "- You can either use the `least_squares_from_formula` module level public function or `least_squares.from_formula` from registed namespace\n",
                 "- It tries to be clever and maps to the correct underlying implementation based on the model specific parameters you specify"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 55,
+            "execution_count": 27,
             "id": "8965d16a-1703-4a75-9729-d8fbadb7a1c7",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:59:38.308011Z",
-                    "iopub.status.busy": "2024-04-22T17:59:38.307828Z",
-                    "iopub.status.idle": "2024-04-22T17:59:38.534424Z",
-                    "shell.execute_reply": "2024-04-22T17:59:38.533146Z",
-                    "shell.execute_reply.started": "2024-04-22T17:59:38.307996Z"
+                    "iopub.execute_input": "2024-04-25T17:43:19.144482Z",
+                    "iopub.status.busy": "2024-04-25T17:43:19.144412Z",
+                    "iopub.status.idle": "2024-04-25T17:43:19.285784Z",
+                    "shell.execute_reply": "2024-04-25T17:43:19.285493Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:19.144476Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
@@ -1217,15 +1217,15 @@
                             "\u2502 f64         \u2506 f64         \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
                             "\u2502 1.0         \u2506 1.0         \u2502\n",
                             "\u2502 1.0         \u2506 1.0         \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 55,
+                    "execution_count": 27,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# compute the residuals in two equivalent ways\n",
                 "df.select(\n",
@@ -1233,23 +1233,23 @@
                 "    pls.compute_least_squares_from_formula(\"y ~ x1 + x2:x3 -1\", mode=\"residuals\").alias(\"residuals_1\"), \n",
                 "    (pl.col(\"y\") - pl.col(\"y\").least_squares.from_formula(\"x1 + x2:x3 -1\", mode=\"predictions\")).alias(\"residuals_2\"),\n",
                 ").corr()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 56,
+            "execution_count": 28,
             "id": "aa610cd9-3b3f-43ce-b9cc-24a92df55307",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:59:38.951969Z",
-                    "iopub.status.busy": "2024-04-22T17:59:38.951696Z",
-                    "iopub.status.idle": "2024-04-22T17:59:38.955717Z",
-                    "shell.execute_reply": "2024-04-22T17:59:38.955314Z",
-                    "shell.execute_reply.started": "2024-04-22T17:59:38.951953Z"
+                    "iopub.execute_input": "2024-04-25T17:43:19.286825Z",
+                    "iopub.status.busy": "2024-04-25T17:43:19.286732Z",
+                    "iopub.status.idle": "2024-04-25T17:43:19.289073Z",
+                    "shell.execute_reply": "2024-04-25T17:43:19.288869Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:19.286817Z"
                 }
             },
             "outputs": [],
             "source": [
                 "nnls_formula_expr = pl.col(\"y\").least_squares.from_formula(\"x1 + x2 + x3\",\n",
                 "                                       alpha=0.0001,\n",
                 "                                       positive=True,\n",
@@ -1275,23 +1275,23 @@
                 "- This extension package provides rust implementations `.least_squares.{rolling_ols, expanding_ols, rls}` which efficiently update coefficients as new samples are observed\n",
                 "- The key idea is to make use of Sherman-Morrison or Woodbury Identity to recursively update summary statistics or coefficient vectors\n",
                 "- Formula API is also supported and the correct implementation is chosen based on parameters provided"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 57,
+            "execution_count": 29,
             "id": "33a8ee68-dc8b-4a2e-a590-73a4998bc33e",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:59:39.402297Z",
-                    "iopub.status.busy": "2024-04-22T17:59:39.398741Z",
-                    "iopub.status.idle": "2024-04-22T17:59:39.456982Z",
-                    "shell.execute_reply": "2024-04-22T17:59:39.456425Z",
-                    "shell.execute_reply.started": "2024-04-22T17:59:39.402269Z"
+                    "iopub.execute_input": "2024-04-25T17:43:19.289563Z",
+                    "iopub.status.busy": "2024-04-25T17:43:19.289458Z",
+                    "iopub.status.idle": "2024-04-25T17:43:19.298677Z",
+                    "shell.execute_reply": "2024-04-25T17:43:19.298408Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:19.289555Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
@@ -1320,15 +1320,15 @@
                             "\u2502 {-0.995348,-1.004411,-0.99898}  \u2506 {-0.985392,-1.011036,-1.00789}  \u2506 -3.506569          \u2502\n",
                             "\u2502 {-1.001142,-1.002267,-1.002736} \u2506 {-1.001857,-0.980484,-1.007321} \u2506 -0.618197          \u2502\n",
                             "\u2502 {-1.001257,-1.001316,-1.003019} \u2506 {-1.002182,-0.978417,-1.006454} \u2506 -0.692359          \u2502\n",
                             "\u2502 {-1.002536,-0.993688,-0.998938} \u2506 {-0.968934,-1.00696,-1.010813}  \u2506 0.159536           \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 57,
+                    "execution_count": 29,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df.select(\n",
                 "    pl.col(\"y\").least_squares.rolling_ols(\"x1\", \"x2\", \"x3\", \n",
@@ -1357,54 +1357,54 @@
                 "### 5. Out Of Sample Prediction\n",
                 "\n",
                 "- If you want to fit on some data then predict on test data, you can do so with `least_squares.predict(...)`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 58,
+            "execution_count": 30,
             "id": "ff412921-2c2d-46b3-baad-d54067fa3312",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:59:39.761606Z",
-                    "iopub.status.busy": "2024-04-22T17:59:39.761430Z",
-                    "iopub.status.idle": "2024-04-22T17:59:39.790918Z",
-                    "shell.execute_reply": "2024-04-22T17:59:39.790278Z",
-                    "shell.execute_reply.started": "2024-04-22T17:59:39.761592Z"
+                    "iopub.execute_input": "2024-04-25T17:43:19.299183Z",
+                    "iopub.status.busy": "2024-04-25T17:43:19.299105Z",
+                    "iopub.status.idle": "2024-04-25T17:43:19.305997Z",
+                    "shell.execute_reply": "2024-04-25T17:43:19.305759Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:19.299176Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>group</th><th>coefficients</th></tr><tr><td>i64</td><td>struct[2]</td></tr></thead><tbody><tr><td>3</td><td>{-1.074243,-1.050159}</td></tr><tr><td>0</td><td>{-1.028893,-1.004733}</td></tr><tr><td>2</td><td>{-0.948578,-0.917406}</td></tr><tr><td>4</td><td>{-1.037308,-0.981468}</td></tr><tr><td>1</td><td>{-1.094156,-0.946028}</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>group</th><th>coefficients</th></tr><tr><td>i64</td><td>struct[2]</td></tr></thead><tbody><tr><td>2</td><td>{-0.948578,-0.917406}</td></tr><tr><td>1</td><td>{-1.094156,-0.946028}</td></tr><tr><td>0</td><td>{-1.028893,-1.004733}</td></tr><tr><td>3</td><td>{-1.074243,-1.050159}</td></tr><tr><td>4</td><td>{-1.037308,-0.981468}</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 2)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 group \u2506 coefficients          \u2502\n",
                             "\u2502 ---   \u2506 ---                   \u2502\n",
                             "\u2502 i64   \u2506 struct[2]             \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 3     \u2506 {-1.074243,-1.050159} \u2502\n",
-                            "\u2502 0     \u2506 {-1.028893,-1.004733} \u2502\n",
                             "\u2502 2     \u2506 {-0.948578,-0.917406} \u2502\n",
-                            "\u2502 4     \u2506 {-1.037308,-0.981468} \u2502\n",
                             "\u2502 1     \u2506 {-1.094156,-0.946028} \u2502\n",
+                            "\u2502 0     \u2506 {-1.028893,-1.004733} \u2502\n",
+                            "\u2502 3     \u2506 {-1.074243,-1.050159} \u2502\n",
+                            "\u2502 4     \u2506 {-1.037308,-0.981468} \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 58,
+                    "execution_count": 30,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# make some random training data\n",
                 "df_train = _make_data(n_groups=1)\n",
@@ -1422,23 +1422,23 @@
                 ")\n",
                 "\n",
                 "df_coefficients.collect()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 59,
+            "execution_count": 31,
             "id": "931b667e-cf4d-4b53-be9b-85278c6fd16c",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2024-04-22T17:59:39.931175Z",
-                    "iopub.status.busy": "2024-04-22T17:59:39.929688Z",
-                    "iopub.status.idle": "2024-04-22T17:59:39.979453Z",
-                    "shell.execute_reply": "2024-04-22T17:59:39.970658Z",
-                    "shell.execute_reply.started": "2024-04-22T17:59:39.931155Z"
+                    "iopub.execute_input": "2024-04-25T17:43:19.306593Z",
+                    "iopub.status.busy": "2024-04-25T17:43:19.306517Z",
+                    "iopub.status.idle": "2024-04-25T17:43:19.311957Z",
+                    "shell.execute_reply": "2024-04-25T17:43:19.311739Z",
+                    "shell.execute_reply.started": "2024-04-25T17:43:19.306585Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
@@ -1469,15 +1469,15 @@
                             "\u2502 0     \u2506 -1.682214        \u2502\n",
                             "\u2502 0     \u2506 0.599761         \u2502\n",
                             "\u2502 0     \u2506 1.30026          \u2502\n",
                             "\u2502 0     \u2506 -1.240682        \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 59,
+                    "execution_count": 31,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# make some test data\n",
                 "df_test = _make_data(n_groups=1)\n",
@@ -1496,33 +1496,171 @@
                 "    .collect()\n",
                 ")\n",
                 "\n",
                 "predictions.head()"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "0859cfce-2084-429d-b9ee-7b54bf5b5f4d",
+            "cell_type": "markdown",
+            "id": "441f1497-ca42-4550-8f2d-74e38dcf1512",
             "metadata": {},
-            "outputs": [],
-            "source": []
+            "source": [
+                "### 6. Multi-output Regression\n",
+                "\n",
+                "- Say you are dealing with a situation where multiple targets are being regressed on the same set of features\n",
+                "- Given solution to OLS problem is `inv(X.T @ X) X.T @ Y` one can note that this is equivalent to running multiple independent regressions for each target\n",
+                "- But that is wasteful as `inv(X.T @ X) X.T` is a common factor\n",
+                "- For this reason the package exposes `compute_multi_target_least_squares` & `least_squares.multi_target_ols` which use SVD (and compute it on `X` only once)\n",
+                "- To use this functionality: pass a polars expression yielding a struct series as target. Other parameters are the same as standard least squares functions."
+            ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 33,
             "id": "8e681f36-f53c-4085-8f61-802f00922e34",
-            "metadata": {},
+            "metadata": {
+                "execution": {
+                    "iopub.execute_input": "2024-04-25T17:49:01.929212Z",
+                    "iopub.status.busy": "2024-04-25T17:49:01.928773Z",
+                    "iopub.status.idle": "2024-04-25T17:49:01.937337Z",
+                    "shell.execute_reply": "2024-04-25T17:49:01.936382Z",
+                    "shell.execute_reply.started": "2024-04-25T17:49:01.929186Z"
+                }
+            },
             "outputs": [],
-            "source": []
+            "source": [
+                "df_multi_target = df.with_columns(\n",
+                "    pl.struct(\n",
+                "        y1=pl.col(\"x1\") + pl.col(\"x2\") + pl.col(\"x3\"),\n",
+                "        y2=pl.col(\"x1\") - pl.col(\"x2\") + pl.col(\"x3\"),\n",
+                "        y3=-pl.col(\"x1\") + pl.col(\"x2\") - pl.col(\"x3\"),\n",
+                "    ).alias(\"y\")\n",
+                ")"
+            ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 35,
             "id": "e3f80629-bf32-4c41-a75c-4490f245ebce",
+            "metadata": {
+                "execution": {
+                    "iopub.execute_input": "2024-04-25T17:49:56.704869Z",
+                    "iopub.status.busy": "2024-04-25T17:49:56.704139Z",
+                    "iopub.status.idle": "2024-04-25T17:49:56.713067Z",
+                    "shell.execute_reply": "2024-04-25T17:49:56.712279Z",
+                    "shell.execute_reply.started": "2024-04-25T17:49:56.704819Z"
+                }
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div><style>\n",
+                            ".dataframe > thead > tr,\n",
+                            ".dataframe > tbody > tr {\n",
+                            "  text-align: right;\n",
+                            "  white-space: pre-wrap;\n",
+                            "}\n",
+                            "</style>\n",
+                            "<small>shape: (5, 6)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>x1</th><th>x2</th><th>x3</th><th>y</th><th>group</th><th>sample_weights</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>struct[3]</td><td>i64</td><td>f64</td></tr></thead><tbody><tr><td>0.12573</td><td>-0.132105</td><td>0.640423</td><td>{0.634048,0.898258,-0.898258}</td><td>1</td><td>0.709215</td></tr><tr><td>0.1049</td><td>-0.535669</td><td>0.361595</td><td>{-0.069174,1.002165,-1.002165}</td><td>0</td><td>0.731333</td></tr><tr><td>1.304</td><td>0.947081</td><td>-0.703735</td><td>{1.547346,-0.346816,0.346816}</td><td>4</td><td>0.701351</td></tr><tr><td>-1.265421</td><td>-0.623274</td><td>0.041326</td><td>{-1.84737,-0.600821,0.600821}</td><td>3</td><td>0.052596</td></tr><tr><td>-2.325031</td><td>-0.218792</td><td>-1.245911</td><td>{-3.789733,-3.35215,3.35215}</td><td>3</td><td>0.963254</td></tr></tbody></table></div>"
+                        ],
+                        "text/plain": [
+                            "shape: (5, 6)\n",
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 x1        \u2506 x2        \u2506 x3        \u2506 y                              \u2506 group \u2506 sample_weights \u2502\n",
+                            "\u2502 ---       \u2506 ---       \u2506 ---       \u2506 ---                            \u2506 ---   \u2506 ---            \u2502\n",
+                            "\u2502 f64       \u2506 f64       \u2506 f64       \u2506 struct[3]                      \u2506 i64   \u2506 f64            \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 0.12573   \u2506 -0.132105 \u2506 0.640423  \u2506 {0.634048,0.898258,-0.898258}  \u2506 1     \u2506 0.709215       \u2502\n",
+                            "\u2502 0.1049    \u2506 -0.535669 \u2506 0.361595  \u2506 {-0.069174,1.002165,-1.002165} \u2506 0     \u2506 0.731333       \u2502\n",
+                            "\u2502 1.304     \u2506 0.947081  \u2506 -0.703735 \u2506 {1.547346,-0.346816,0.346816}  \u2506 4     \u2506 0.701351       \u2502\n",
+                            "\u2502 -1.265421 \u2506 -0.623274 \u2506 0.041326  \u2506 {-1.84737,-0.600821,0.600821}  \u2506 3     \u2506 0.052596       \u2502\n",
+                            "\u2502 -2.325031 \u2506 -0.218792 \u2506 -1.245911 \u2506 {-3.789733,-3.35215,3.35215}   \u2506 3     \u2506 0.963254       \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                        ]
+                    },
+                    "execution_count": 35,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "df_multi_target.head()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 50,
+            "id": "1cc3738f-89f4-4bce-b780-04f0c96c2bc9",
+            "metadata": {
+                "execution": {
+                    "iopub.execute_input": "2024-04-25T17:55:18.525628Z",
+                    "iopub.status.busy": "2024-04-25T17:55:18.525326Z",
+                    "iopub.status.idle": "2024-04-25T17:55:18.534221Z",
+                    "shell.execute_reply": "2024-04-25T17:55:18.533746Z",
+                    "shell.execute_reply.started": "2024-04-25T17:55:18.525605Z"
+                }
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div><style>\n",
+                            ".dataframe > thead > tr,\n",
+                            ".dataframe > tbody > tr {\n",
+                            "  text-align: right;\n",
+                            "  white-space: pre-wrap;\n",
+                            "}\n",
+                            "</style>\n",
+                            "<small>shape: (5, 7)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>x1</th><th>x2</th><th>x3</th><th>y</th><th>group</th><th>sample_weights</th><th>residuals</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>struct[3]</td><td>i64</td><td>f64</td><td>struct[3]</td></tr></thead><tbody><tr><td>0.12573</td><td>-0.132105</td><td>0.640423</td><td>{0.634048,0.898258,-0.898258}</td><td>1</td><td>0.709215</td><td>{4.4409e-16,4.4409e-16,-4.4409e-16}</td></tr><tr><td>0.1049</td><td>-0.535669</td><td>0.361595</td><td>{-0.069174,1.002165,-1.002165}</td><td>0</td><td>0.731333</td><td>{-1.6515e-15,-8.8818e-16,8.8818e-16}</td></tr><tr><td>1.304</td><td>0.947081</td><td>-0.703735</td><td>{1.547346,-0.346816,0.346816}</td><td>4</td><td>0.701351</td><td>{1.3323e-15,3.8858e-16,-6.1062e-16}</td></tr><tr><td>-1.265421</td><td>-0.623274</td><td>0.041326</td><td>{-1.84737,-0.600821,0.600821}</td><td>3</td><td>0.052596</td><td>{-8.8818e-16,-1.3323e-15,1.3323e-15}</td></tr><tr><td>-2.325031</td><td>-0.218792</td><td>-1.245911</td><td>{-3.789733,-3.35215,3.35215}</td><td>3</td><td>0.963254</td><td>{-1.3323e-15,-4.4409e-16,4.4409e-16}</td></tr></tbody></table></div>"
+                        ],
+                        "text/plain": [
+                            "shape: (5, 7)\n",
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 x1        \u2506 x2        \u2506 x3        \u2506 y                \u2506 group \u2506 sample_weights \u2506 residuals        \u2502\n",
+                            "\u2502 ---       \u2506 ---       \u2506 ---       \u2506 ---              \u2506 ---   \u2506 ---            \u2506 ---              \u2502\n",
+                            "\u2502 f64       \u2506 f64       \u2506 f64       \u2506 struct[3]        \u2506 i64   \u2506 f64            \u2506 struct[3]        \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 0.12573   \u2506 -0.132105 \u2506 0.640423  \u2506 {0.634048,0.8982 \u2506 1     \u2506 0.709215       \u2506 {4.4409e-16,4.44 \u2502\n",
+                            "\u2502           \u2506           \u2506           \u2506 58,-0.898258}    \u2506       \u2506                \u2506 09e-16,-4.4409e- \u2502\n",
+                            "\u2502           \u2506           \u2506           \u2506                  \u2506       \u2506                \u2506 \u2026                \u2502\n",
+                            "\u2502 0.1049    \u2506 -0.535669 \u2506 0.361595  \u2506 {-0.069174,1.002 \u2506 0     \u2506 0.731333       \u2506 {-1.6515e-15,-8. \u2502\n",
+                            "\u2502           \u2506           \u2506           \u2506 165,-1.002165}   \u2506       \u2506                \u2506 8818e-16,8.8818e \u2502\n",
+                            "\u2502           \u2506           \u2506           \u2506                  \u2506       \u2506                \u2506 \u2026                \u2502\n",
+                            "\u2502 1.304     \u2506 0.947081  \u2506 -0.703735 \u2506 {1.547346,-0.346 \u2506 4     \u2506 0.701351       \u2506 {1.3323e-15,3.88 \u2502\n",
+                            "\u2502           \u2506           \u2506           \u2506 816,0.346816}    \u2506       \u2506                \u2506 58e-16,-6.1062e- \u2502\n",
+                            "\u2502           \u2506           \u2506           \u2506                  \u2506       \u2506                \u2506 \u2026                \u2502\n",
+                            "\u2502 -1.265421 \u2506 -0.623274 \u2506 0.041326  \u2506 {-1.84737,-0.600 \u2506 3     \u2506 0.052596       \u2506 {-8.8818e-16,-1. \u2502\n",
+                            "\u2502           \u2506           \u2506           \u2506 821,0.600821}    \u2506       \u2506                \u2506 3323e-15,1.3323e \u2502\n",
+                            "\u2502           \u2506           \u2506           \u2506                  \u2506       \u2506                \u2506 \u2026                \u2502\n",
+                            "\u2502 -2.325031 \u2506 -0.218792 \u2506 -1.245911 \u2506 {-3.789733,-3.35 \u2506 3     \u2506 0.963254       \u2506 {-1.3323e-15,-4. \u2502\n",
+                            "\u2502           \u2506           \u2506           \u2506 215,3.35215}     \u2506       \u2506                \u2506 4409e-16,4.4409e \u2502\n",
+                            "\u2502           \u2506           \u2506           \u2506                  \u2506       \u2506                \u2506 \u2026                \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                        ]
+                    },
+                    "execution_count": 50,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# do multi-target .. it works\n",
+                "df_multi_target.with_columns(\n",
+                "    pl.col(\"y\").least_squares.multi_target_ols(\"x1\", \"x2\", \"x3\", \n",
+                "                                               sample_weights=\"sample_weights\",\n",
+                "                                               mode=\"residuals\",\n",
+                "                                              ).over(\"group\").alias(\"residuals\")\n",
+                ").head()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "e010b5cf-aa98-4bc4-a1d3-9a32ee43d611",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `polars_ols-0.3.1/polars_ols/__init__.py` & `polars_ols-0.3.2/polars_ols/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,28 +9,32 @@
     OLSKwargs,
     OutputMode,
     RLSKwargs,
     RollingKwargs,
     SolveMethod,
     compute_least_squares,
     compute_least_squares_from_formula,
+    compute_multi_target_least_squares,
     compute_recursive_least_squares,
     compute_rolling_least_squares,
     predict,
 )
 from polars_ols.utils import build_expressions_from_patsy_formula
 
 __all__ = [
     "compute_least_squares",
     "compute_recursive_least_squares",
     "compute_rolling_least_squares",
-    "LeastSquares",
+    "compute_multi_target_least_squares",
     "compute_least_squares_from_formula",
+    "LeastSquares",
 ]
 
+ExprOrStr = Union[pl.Expr, str]
+
 
 @pl.api.register_expr_namespace("least_squares")
 class LeastSquares:
     """Registers the `.least_squares` namespace and provide entry points for the various models
      supported by this extension package.
 
      The below are parameters common to all models:
@@ -56,78 +60,84 @@
     """
 
     def __init__(self, expr: pl.Expr):
         self._expr = expr
 
     def least_squares(
         self,
-        *features: pl.Expr,
-        sample_weights: Optional[pl.Expr] = None,
+        *features: ExprOrStr,
+        sample_weights: Optional[ExprOrStr] = None,
         add_intercept: bool = False,
         mode: OutputMode = "predictions",
         null_policy: NullPolicy = "ignore",
         solve_method: Optional[SolveMethod] = None,
+        multi_target: bool = False,
         **ols_kwargs,
     ) -> pl.Expr:
         """Perform least squares regression.
 
         :param features: Variable number of feature expressions.
         :param sample_weights: Optional expression representing sample weights.
         :param add_intercept: Whether to add an intercept column.
         :param mode: Mode of operation ("predictions", "residuals", "coefficients").
         :param null_policy: Strategy for handling missing data.
         :param solve_method: Algorithm used for computing least squares solution.
                              Defaults to None, where a recommended default method is chosen based
                              on parametrization of the least-squares problem.
                              It can be one of ("qr", "svd", "chol", "lu", "cd").
+        :param multi_target: boolean indicating if the target expression is multi-target struct.
         :param ols_kwargs: Additional, optional, model specific kwargs. See OLSKwargs.
         """
-        return compute_least_squares(
+        ols_func = compute_least_squares if not multi_target else compute_multi_target_least_squares
+        return ols_func(
             self._expr,
             *features,
             sample_weights=sample_weights,
             add_intercept=add_intercept,
             mode=mode,
             ols_kwargs=OLSKwargs(null_policy=null_policy, solve_method=solve_method, **ols_kwargs),
         )
 
-    def ols(self, *features: pl.Expr, **kwargs) -> pl.Expr:
+    def ols(self, *features: ExprOrStr, **kwargs) -> pl.Expr:
         """Performs ordinary least squares. Alias for `least_squares`."""
         return self.least_squares(*features, **kwargs)
 
-    def wls(self, *features: pl.Expr, sample_weights: pl.Expr, **kwargs) -> pl.Expr:
+    def multi_target_ols(self, *features: ExprOrStr, **kwargs) -> pl.Expr:
+        return self.least_squares(*features, multi_target=True, **kwargs)
+
+    def wls(self, *features: ExprOrStr, sample_weights: ExprOrStr, **kwargs) -> pl.Expr:
         """Performs weighted least squares. Alias for `least_squares`.
 
         :param features: Variable number of feature expressions.
         :param sample_weights: optional expression representing sample weights.
         :param kwargs: additional kwargs passed to `least_squares` function.
         """
         return self.least_squares(*features, sample_weights=sample_weights, **kwargs)
 
-    def ridge(self, *features: pl.Expr, alpha: float, **kwargs) -> pl.Expr:
+    def ridge(self, *features: ExprOrStr, alpha: float, **kwargs) -> pl.Expr:
         """Performs ridge regression. Alias for `least_squares`.
 
         :param features: Variable number of feature expressions.
         :param alpha: L2 regularization parameter. Must be non-negative.
         :param kwargs: additional kwargs passed to `least_squares` function.
         """
         return self.least_squares(*features, alpha=alpha, l1_ratio=0.0, **kwargs)
 
-    def lasso(self, *features: pl.Expr, alpha: float, **kwargs) -> pl.Expr:
+    def lasso(self, *features: ExprOrStr, alpha: float, **kwargs) -> pl.Expr:
         """Performs lasso regression. Alias for `least_squares`.
 
         :param features: Variable number of feature expressions.
         :param alpha: L1 regularization parameter. Must be non-negative.
         :param kwargs: additional kwargs passed to `least_squares` function.
         """
         return self.least_squares(*features, alpha=alpha, l1_ratio=1.0, **kwargs)
 
     def elastic_net(
         self,
-        *features: pl.Expr,
+        *features: ExprOrStr,
         alpha: float,
         l1_ratio: float = 0.5,
         positive: bool = False,
         **kwargs,
     ):
         """Performs lasso regression. Alias for `least_squares`.
 
@@ -142,16 +152,16 @@
         """
         return self.least_squares(
             *features, alpha=alpha, l1_ratio=l1_ratio, positive=positive, **kwargs
         )
 
     def rls(
         self,
-        *features: pl.Expr,
-        sample_weights: Optional[pl.Expr] = None,
+        *features: ExprOrStr,
+        sample_weights: Optional[ExprOrStr] = None,
         add_intercept: bool = False,
         mode: OutputMode = "predictions",
         null_policy: NullPolicy = "drop",
         half_life: Optional[float] = None,
         initial_state_covariance: Optional[float] = 10.0,
         initial_state_mean: Union[Optional[List[float], float]] = None,
     ):
@@ -190,17 +200,17 @@
                 initial_state_mean=initial_state_mean,
                 initial_state_covariance=initial_state_covariance,
             ),
         )
 
     def rolling_ols(
         self,
-        *features: pl.Expr,
+        *features: ExprOrStr,
         window_size: int,
-        sample_weights: Optional[pl.Expr] = None,
+        sample_weights: Optional[ExprOrStr] = None,
         add_intercept: bool = False,
         mode: OutputMode = "predictions",
         null_policy: NullPolicy = "drop",
         min_periods: Optional[int] = None,
         use_woodbury: Optional[bool] = None,
         alpha: Optional[float] = None,
     ):
@@ -243,15 +253,15 @@
                 min_periods=min_periods,
                 use_woodbury=use_woodbury,
                 alpha=alpha,
                 null_policy=null_policy,
             ),
         )
 
-    def expanding_ols(self, *features: pl.Expr, **kwargs):
+    def expanding_ols(self, *features: ExprOrStr, **kwargs):
         return self.rls(*features, half_life=None, **kwargs)
 
     def from_formula(self, formula: str, **kwargs) -> pl.Expr:
         features, add_intercept = build_expressions_from_patsy_formula(
             formula, include_dependent_variable=False
         )
         if kwargs.get("half_life"):
@@ -259,15 +269,15 @@
         elif kwargs.get("window_size"):
             return self.rolling_ols(*features, add_intercept=add_intercept, **kwargs)
         else:
             return self.least_squares(*features, add_intercept=add_intercept, **kwargs)
 
     def predict(
         self,
-        *features: pl.Expr,
+        *features: ExprOrStr,
         name: Optional[str] = None,
         add_intercept: bool = False,
         null_policy: NullPolicy = "zero",
     ) -> pl.Expr:
         return predict(
             self._expr,
             *features,
```

### Comparing `polars_ols-0.3.1/polars_ols/least_squares.py` & `polars_ols-0.3.2/polars_ols/least_squares.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,23 +22,23 @@
 
 if TYPE_CHECKING:
     import polars as pl
     from polars.type_aliases import IntoExpr
 
     ExprOrStr = Union[pl.Expr, str]
 
-
 logger = logging.getLogger(__name__)
 
 __all__ = [
     # fitting and prediction functions
     "compute_least_squares",
     "compute_recursive_least_squares",
     "compute_rolling_least_squares",
     "compute_least_squares_from_formula",
+    "compute_multi_target_least_squares",
     "predict",
     # model specific parameters
     "OLSKwargs",
     "RLSKwargs",
     "RollingKwargs",
     # types controlling general modelling behaviour
     "NullPolicy",
@@ -241,17 +241,17 @@
         if mode == "predictions":
             return predictions
         else:
             return target - predictions
 
 
 def compute_least_squares(
-    target: IntoExpr,
-    *features: pl.Expr,
-    sample_weights: Optional[pl.Expr] = None,
+    target: ExprOrStr,
+    *features: ExprOrStr,
+    sample_weights: Optional[ExprOrStr] = None,
     add_intercept: bool = False,
     mode: OutputMode = "predictions",
     ols_kwargs: Optional[OLSKwargs] = None,
 ) -> pl.Expr:
     """Performs least squares regression.
 
     Depending on parameters provided this method supports a combination of sample weighting (WLS),
@@ -266,27 +266,77 @@
         mode: Mode of operation ("predictions", "residuals", "coefficients").
         ols_kwargs: Additional keyword arguments specific for regularized OLS models. See OLSKwargs.
     Returns:
         Resulting expression based on the chosen mode.
     """
     assert mode in _VALID_OUTPUT_MODES, f"'mode' must be one of {_VALID_OUTPUT_MODES}"
     ols_kwargs: OLSKwargs = ols_kwargs or OLSKwargs()
+
     # register either coefficient or prediction plugin functions
     return _register_least_squares_plugin(
         target,
         *features,
         mode=mode,
         function_name="least_squares",
         ols_kwargs=ols_kwargs,
         sample_weights=sample_weights,
         add_intercept=add_intercept,
         returns_scalar_coefficients=True,
     )
 
 
+def compute_multi_target_least_squares(
+    targets: ExprOrStr,
+    *features: ExprOrStr,
+    sample_weights: Optional[ExprOrStr] = None,
+    add_intercept: bool = False,
+    mode: OutputMode = "predictions",
+    ols_kwargs: Optional[OLSKwargs] = None,
+) -> pl.Expr:
+    """Performs multi-target least squares regression.
+
+    This function expects 'targets' to be of type struct with field names corresponding
+    to each target series name. It returns an expression yielding a struct with similar field names
+    and either predictions or residuals as values depending on the chosen mode.
+
+    This is more efficient, but equivalent to, running 'N' multiple linear regressions of each
+    underlying target onto the same set of features.
+
+    OLS, WLS, & Ridge for both "prediction" and "residuals" modes are currently supported.
+    For other configurations (e.g. LASSO): consider running multiple independent regressions on
+    a multi-expression "target" using 'compute_least_squares'.
+    """
+    ols_kwargs = ols_kwargs or OLSKwargs()
+    multi_target_conditions = not ols_kwargs.positive and (
+        ols_kwargs.l1_ratio is None or ols_kwargs.l1_ratio == 0.0
+    )
+    msg = "Consider running multiple independent regressions on a multi-expression target!"
+    assert multi_target_conditions, (
+        "Multi-target regression is only supported " "for unconstrained OLS & Ridge problems." + msg
+    )
+    assert ols_kwargs.solve_method in {"svd", None}, (
+        "only solve_method='svd' is supported for " "multi-target regressions"
+    )
+    if mode == "coefficients":
+        raise NotImplementedError(
+            "Only mode={'predictions', 'residuals'} " "is currently supported. " + msg
+        )
+
+    return _register_least_squares_plugin(
+        targets,
+        *features,
+        function_name="multi_target_least_squares",
+        ols_kwargs=ols_kwargs,
+        sample_weights=sample_weights,
+        add_intercept=add_intercept,
+        returns_scalar_coefficients=True,
+        mode=mode,
+    )
+
+
 def compute_recursive_least_squares(
     target: ExprOrStr,
     *features: ExprOrStr,
     sample_weights: Optional[ExprOrStr] = None,
     add_intercept: bool = False,
     mode: OutputMode = "predictions",
     rls_kwargs: Optional[RLSKwargs] = None,
```

### Comparing `polars_ols-0.3.1/polars_ols/utils.py` & `polars_ols-0.3.2/polars_ols/utils.py`

 * *Files identical despite different names*

### Comparing `polars_ols-0.3.1/src/expressions.rs` & `polars_ols-0.3.2/src/expressions.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #![allow(clippy::unit_arg, clippy::unused_unit)]
-use ndarray::{Array, Array1, Array2, Axis};
+use ndarray::{s, Array, Array1, Array2, Axis};
 use polars::datatypes::{DataType, Field, Float64Type};
 use polars::error::{polars_err, PolarsResult};
 use polars::frame::DataFrame;
 use polars::prelude::{
     lit, BooleanChunked, FillNullStrategy, IndexOrder, IntoLazy, IntoSeries, NamedFrom,
     NamedFromOwned, Series, NULL,
 };
 use pyo3_polars::derive::polars_expr;
 use serde::Deserialize;
 use std::str::FromStr;
 
 use crate::least_squares::{
-    solve_elastic_net, solve_ols, solve_recursive_least_squares, solve_ridge, solve_rolling_ols,
-    NullPolicy, SolveMethod,
+    solve_elastic_net, solve_multi_target, solve_ols, solve_recursive_least_squares, solve_ridge,
+    solve_rolling_ols, NullPolicy, SolveMethod,
 };
 
 /// convert a slice of polars series into a 2D feature array.
 fn construct_features_array(inputs: &[Series], fill_zero: bool) -> Array2<f64> {
     let m = inputs.len();
     let n = inputs[0].len();
     // Prepare features ndarray
@@ -100,18 +100,22 @@
     Ok(Field::new(
         "coefficients",
         DataType::Struct(input_fields[1..].to_vec()),
     ))
 }
 
 /// Convert the coefficients into a Polars series of struct dtype.
-fn coefficients_to_struct_series(coefficients: &Array2<f64>, feature_names: &[&str]) -> Series {
+fn convert_array_to_struct_series(
+    array: &Array2<f64>,
+    feature_names: &[&str],
+    name: Option<&str>,
+) -> Series {
     // Convert 2D ndarray into DataFrame
     let df: DataFrame = DataFrame::new(
-        coefficients
+        array
             .axis_iter(Axis(1))
             .enumerate()
             .map(|(i, col)| {
                 // TODO: clean below up once https://github.com/pola-rs/pyo3-polars/issues/79
                 //  is resolved
                 let i_str = i.to_string();
                 let name = if feature_names[i].is_empty() {
@@ -126,15 +130,15 @@
     )
     .unwrap()
     .lazy()
     .fill_nan(lit(NULL))
     .collect()
     .unwrap();
     // Convert DataFrame to a Series of struct dtype
-    df.into_struct("coefficients").into_series()
+    df.into_struct(name.unwrap_or("coefficients")).into_series()
 }
 
 fn mask_predictions(predictions: Vec<f64>, is_valid_mask: &BooleanChunked) -> Vec<Option<f64>> {
     is_valid_mask
         .iter()
         .zip(&predictions)
         // apply validity mask to predictions
@@ -185,27 +189,39 @@
     }
 }
 
 fn convert_option_vec_to_array1(opt_vec: Option<Vec<f64>>) -> Option<Array1<f64>> {
     opt_vec.map(Array1::from)
 }
 
-fn compute_is_valid_mask(inputs: &[Series], null_policy: &NullPolicy) -> Option<BooleanChunked> {
+fn compute_is_valid_mask(
+    inputs: &[Series],
+    null_policy: &NullPolicy,
+    multi_target_index: Option<usize>,
+) -> Option<BooleanChunked> {
+    let multi_target_index = multi_target_index.unwrap_or(0);
     match null_policy {
         // Compute the intersection of all non-null rows across input series
         NullPolicy::Drop | NullPolicy::DropZero | NullPolicy::DropWindow => {
             let is_valid_mask = inputs[0].is_not_null();
             Some(
                 inputs[1..]
                     .iter()
                     .fold(is_valid_mask, |acc, s| acc & s.is_not_null()),
             )
         }
         // Compute non-null mask based on the first input series (i.e. targets)
-        NullPolicy::DropYZeroX => Some(inputs[0].is_not_null()),
+        NullPolicy::DropYZeroX => match multi_target_index {
+            0 => Some(inputs[0].is_not_null()),
+            _ => Some(
+                inputs[1..multi_target_index]
+                    .iter()
+                    .fold(inputs[0].is_not_null(), |acc, s| acc & s.is_not_null()),
+            ),
+        },
         _ => None,
     }
 }
 
 fn convert_is_valid_mask_to_vec(is_valid: &Option<BooleanChunked>, n_samples: usize) -> Vec<bool> {
     if let Some(boolean_chunked) = is_valid {
         assert_eq!(
@@ -365,15 +381,15 @@
         )
     }
 }
 
 #[polars_expr(output_type=Float64)]
 fn least_squares(inputs: &[Series], kwargs: OLSKwargs) -> PolarsResult<Series> {
     let null_policy = kwargs.get_null_policy();
-    let is_valid = compute_is_valid_mask(inputs, &null_policy);
+    let is_valid = compute_is_valid_mask(inputs, &null_policy, None);
     let (y_fit, x_fit) = convert_polars_to_ndarray(inputs, &null_policy, is_valid.as_ref());
     let coefficients =
         Coefficients::Array1(_get_least_squares_coefficients(&y_fit, &x_fit, kwargs));
 
     if matches!(null_policy, NullPolicy::Ignore | NullPolicy::Zero) {
         // absent additional filtering: features for fitting is the same as for prediction
         Ok(make_predictions(
@@ -405,37 +421,119 @@
         }
     }
 }
 
 #[polars_expr(output_type_func=coefficients_struct_dtype)]
 fn least_squares_coefficients(inputs: &[Series], kwargs: OLSKwargs) -> PolarsResult<Series> {
     let null_policy = kwargs.get_null_policy();
-    let is_valid = compute_is_valid_mask(inputs, &null_policy);
+    let is_valid = compute_is_valid_mask(inputs, &null_policy, None);
     let (y, x) = convert_polars_to_ndarray(inputs, &null_policy, is_valid.as_ref());
     // force into 1 x K 2-d array, so that we can return a series of struct
     let coefficients = _get_least_squares_coefficients(&y, &x, kwargs).insert_axis(Axis(0));
     // convert coefficients to a polars struct
     let feature_names: Vec<&str> = inputs[1..].iter().map(|input| input.name()).collect();
     assert_eq!(
         feature_names.len(),
         coefficients.len_of(Axis(1)),
         "number of coefficients must match number of features!"
     );
-    let series = coefficients_to_struct_series(&coefficients, &feature_names);
+    let series = convert_array_to_struct_series(&coefficients, &feature_names, None);
     Ok(series.with_name("coefficients"))
 }
 
+fn multi_target_struct_dtype(input_fields: &[Field]) -> PolarsResult<Field> {
+    let dtype = input_fields[0].dtype.to_owned();
+    assert!(
+        dtype.is_struct(),
+        "the first series in a multi-target regression \
+        must be of polars struct dtype with each field corresponding to an output"
+    );
+    Ok(Field::new("predictions", dtype))
+}
+
+#[polars_expr(output_type_func=multi_target_struct_dtype)]
+fn multi_target_least_squares(inputs: &[Series], kwargs: OLSKwargs) -> PolarsResult<Series> {
+    let null_policy = kwargs.get_null_policy();
+
+    // compute targets
+    let targets_struct = inputs[0]
+        .struct_()
+        .expect("the first series in a multi-target regression must be a struct");
+    let targets_df = targets_struct.to_owned().unnest();
+    let target_series = targets_df.iter().as_slice();
+
+    // concatenate multi-target and feature series
+    let series = [target_series, &inputs[1..]].concat();
+
+    // define number of target series
+    let m = target_series.len();
+
+    // compute validity mask
+    let is_valid = compute_is_valid_mask(&series, &null_policy, Some(m));
+
+    // handle nulls according to the specified null policy (this should just work for multi-target)
+    let mut filtered_series = Vec::new();
+    handle_nulls(
+        &series,
+        &null_policy,
+        is_valid.as_ref(),
+        &mut filtered_series,
+    );
+
+    // compute filtered features & targets array
+    let features_array = construct_features_array(&filtered_series[m..], true);
+    let targets_array = construct_features_array(&filtered_series[..m], true);
+
+    // this should be K x M, where K is number of features
+    let coefficients =
+        solve_multi_target(&targets_array, &features_array, kwargs.alpha, kwargs.rcond);
+    assert_eq!(coefficients.nrows(), features_array.ncols());
+    assert_eq!(coefficients.ncols(), targets_array.ncols());
+
+    let target_names: Vec<&str> = target_series.iter().map(|s| s.name()).collect();
+
+    if matches!(null_policy, NullPolicy::Ignore | NullPolicy::Zero) {
+        let predictions = features_array.dot(&coefficients);
+        Ok(convert_array_to_struct_series(
+            &predictions,
+            &target_names,
+            Some("predictions"),
+        ))
+    } else {
+        // compute unfiltered features array and predictions assuming zero filled features
+        let features_array_predict = construct_features_array(&inputs[1..], true);
+        let mut predictions = features_array_predict.dot(&coefficients);
+
+        // re-mask invalid predictions
+        if null_policy == NullPolicy::Drop {
+            if let Some(is_valid) = is_valid {
+                for (i, valid) in is_valid.iter().enumerate() {
+                    if !valid.unwrap_or(false) {
+                        predictions.slice_mut(s![i, ..]).fill(f64::NAN);
+                    }
+                }
+            }
+        }
+
+        Ok(convert_array_to_struct_series(
+            &predictions,
+            &target_names,
+            Some("predictions"),
+        ))
+    }
+}
+
 #[polars_expr(output_type_func=coefficients_struct_dtype)]
 fn recursive_least_squares_coefficients(
     inputs: &[Series],
     kwargs: RLSKwargs,
 ) -> PolarsResult<Series> {
     let null_policy = kwargs.get_null_policy();
 
-    let is_valid = compute_is_valid_mask(inputs, &null_policy);
+    let is_valid = compute_is_valid_mask(inputs, &null_policy, None);
     let is_valid = convert_is_valid_mask_to_vec(&is_valid, inputs[0].len());
 
     let (y, x) = convert_polars_to_ndarray(inputs, &NullPolicy::Zero, None);
     let initial_state_mean = convert_option_vec_to_array1(kwargs.initial_state_mean);
     let coefficients = solve_recursive_least_squares(
         &y,
         &x,
@@ -447,22 +545,22 @@
     // convert coefficients to a polars struct
     let feature_names: Vec<&str> = inputs[1..].iter().map(|input| input.name()).collect();
     assert_eq!(
         feature_names.len(),
         coefficients.len_of(Axis(1)),
         "number of coefficients must match number of features!"
     );
-    let series = coefficients_to_struct_series(&coefficients, &feature_names);
+    let series = convert_array_to_struct_series(&coefficients, &feature_names, None);
     Ok(series.with_name("coefficients"))
 }
 
 #[polars_expr(output_type=Float64)]
 fn recursive_least_squares(inputs: &[Series], kwargs: RLSKwargs) -> PolarsResult<Series> {
     let null_policy = kwargs.get_null_policy();
-    let is_valid = compute_is_valid_mask(inputs, &null_policy);
+    let is_valid = compute_is_valid_mask(inputs, &null_policy, None);
     let is_valid_vec = convert_is_valid_mask_to_vec(&is_valid, inputs[0].len());
     let (y, x) = convert_polars_to_ndarray(inputs, &NullPolicy::Zero, None);
 
     let coefficients = Coefficients::Array2(solve_recursive_least_squares(
         &y,
         &x,
         kwargs.half_life,
@@ -481,15 +579,15 @@
 
 #[polars_expr(output_type_func=coefficients_struct_dtype)]
 fn rolling_least_squares_coefficients(
     inputs: &[Series],
     kwargs: RollingKwargs,
 ) -> PolarsResult<Series> {
     let null_policy = kwargs.get_null_policy();
-    let is_valid = compute_is_valid_mask(inputs, &null_policy);
+    let is_valid = compute_is_valid_mask(inputs, &null_policy, None);
     let is_valid = convert_is_valid_mask_to_vec(&is_valid, inputs[0].len());
     let (y, x) = convert_polars_to_ndarray(inputs, &NullPolicy::Zero, None);
     let coefficients = solve_rolling_ols(
         &y,
         &x,
         kwargs.window_size,
         kwargs.min_periods,
@@ -501,22 +599,22 @@
     // convert coefficients to a polars struct
     let feature_names: Vec<&str> = inputs[1..].iter().map(|input| input.name()).collect();
     assert_eq!(
         feature_names.len(),
         coefficients.len_of(Axis(1)),
         "number of coefficients must match number of features!"
     );
-    let series = coefficients_to_struct_series(&coefficients, &feature_names);
+    let series = convert_array_to_struct_series(&coefficients, &feature_names, None);
     Ok(series.with_name("coefficients"))
 }
 
 #[polars_expr(output_type=Float64)]
 fn rolling_least_squares(inputs: &[Series], kwargs: RollingKwargs) -> PolarsResult<Series> {
     let null_policy = kwargs.get_null_policy();
-    let is_valid = compute_is_valid_mask(inputs, &null_policy);
+    let is_valid = compute_is_valid_mask(inputs, &null_policy, None);
     let is_valid_vec = convert_is_valid_mask_to_vec(&is_valid, inputs[0].len());
     let (y, x) = convert_polars_to_ndarray(inputs, &NullPolicy::Zero, None);
     let coefficients = Coefficients::Array2(solve_rolling_ols(
         &y,
         &x,
         kwargs.window_size,
         kwargs.min_periods,
@@ -559,15 +657,15 @@
     let coefficients: Array2<f64> = coefficients_df
         .to_ndarray::<Float64Type>(IndexOrder::C)
         .unwrap();
     let predictions = (&features * &coefficients).sum_axis(Axis(1)).to_vec();
 
     if null_policy == NullPolicy::Drop {
         // If user has opted for "Drop" policy: mask predictions
-        let is_valid = compute_is_valid_mask(inputs, &null_policy).unwrap();
+        let is_valid = compute_is_valid_mask(inputs, &null_policy, None).unwrap();
         Ok(Series::new(
             inputs[0].name(),
             mask_predictions(predictions, &is_valid),
         ))
     } else {
         // Otherwise, simply return predictions
         Ok(Series::from_vec(inputs[0].name(), predictions))
```

### Comparing `polars_ols-0.3.1/src/least_squares.rs` & `polars_ols-0.3.2/src/least_squares.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+use std::cmp::{max, min};
+use std::collections::VecDeque;
+use std::str::FromStr;
+
 use faer::linalg::solvers::SolverCore;
 use faer::prelude::*;
 use faer::Side;
 use faer_ext::{IntoFaer, IntoNdarray};
-use ndarray::{array, s, Array, Array1, Array2, ArrayView1, Axis, NewAxis};
-use std::cmp::{max, min};
-use std::collections::VecDeque;
-use std::str::FromStr;
+
+#[allow(unused_imports)]
+use ndarray::{array, s, Array, Array1, Array2, ArrayBase, ArrayView1, Axis, Dimension, Ix2, NewAxis,
+    OwnedRepr, Dim,
+};
 
 #[cfg(any(
     all(target_os = "linux", any(target_arch = "x86_64", target_arch = "x64")),
     target_os = "macos"
 ))]
 use ndarray_linalg::LeastSquaresSvd;
 
@@ -95,22 +100,39 @@
 /// * `alpha` - Ridge parameter.
 /// * `rcond` - Relative condition number used to determine cutoff for small singular values.
 ///
 /// # Returns
 ///
 /// * Result of ridge regression as a 1-dimensional array.
 #[inline]
-fn solve_ridge_svd(
-    y: &Array1<f64>,
+fn solve_ridge_svd<I>(
+    y: &ArrayBase<OwnedRepr<f64>, I>,
     x: &Array2<f64>,
     alpha: f64,
     rcond: Option<f64>,
-) -> Array1<f64> {
+) -> ArrayBase<OwnedRepr<f64>, I>
+where
+    I: Dimension,
+{
     let x_faer = x.view().into_faer();
-    let y_faer = y.view().insert_axis(Axis(1)).into_faer();
+
+    let y_faer = if y.ndim() == 2 {
+        y.view()
+            .into_dimensionality::<Ix2>()
+            .expect("could not reshape y")
+            .into_faer()
+    } else {
+        y.view()
+            .insert_axis(Axis(1))
+            .into_dimensionality::<Ix2>()
+            .expect("could not reshape y")
+            .into_faer()
+    };
+
+    let is_multi_target = y_faer.ncols() > 1;
 
     // compute SVD and extract u, s, vt
     let svd = x_faer.thin_svd();
     let u = svd.u();
     let v = svd.v().into_ndarray();
     let s = svd.s_diagonal();
 
@@ -120,41 +142,60 @@
 
     // set singular values less than or equal to ``rcond * largest_singular_value`` to zero.
     let cutoff =
         rcond.unwrap_or(f64::EPSILON * max(x_faer.ncols(), x_faer.nrows()) as f64) * max_value;
     let s = s.map(|v| if v < &cutoff { 0. } else { *v });
 
     let binding = u.transpose() * y_faer;
-    let u_t_y: Array1<f64> = binding
-        .as_ref()
-        .into_ndarray()
-        .slice(s![.., 0])
-        .into_owned();
     let d = &s / (&s * &s + alpha);
-    let d_ut_y = &d * &u_t_y;
-    v.dot(&d_ut_y)
+
+    if is_multi_target {
+        let u_t_y = binding.as_ref().into_ndarray().to_owned();
+        let d_ut_y_t = &d * &u_t_y.t();
+        v.dot(&d_ut_y_t.t())
+            .to_owned()
+            .into_dimensionality::<I>()
+            .expect("could not reshape output")
+    } else {
+        let u_t_y: Array1<f64> = binding
+            .as_ref()
+            .into_ndarray()
+            .slice(s![.., 0])
+            .into_owned();
+        let d_ut_y = &d * &u_t_y;
+        v.dot(&d_ut_y)
+            .into_dimensionality::<I>()
+            .expect("could not reshape output")
+    }
 }
 
 #[cfg(not(any(
     all(target_os = "linux", any(target_arch = "x86_64", target_arch = "x64")),
     target_os = "macos"
 )))]
-fn solve_ols_svd(y: &Array1<f64>, x: &Array2<f64>, rcond: Option<f64>) -> Array1<f64> {
+fn solve_ols_svd<D>(y: &Array<f64, D>, x: &Array2<f64>, rcond: Option<f64>) -> Array<f64, D>
+where
+    D: Dimension,
+{
     // fallback SVD solver for platforms which don't (easily) support LAPACK solver
     solve_ridge_svd(y, x, 1.0e-64, rcond) // near zero ridge penalty
 }
 
 /// Solves least-squares regression using divide and conquer SVD. Thin wrapper to LAPACK: DGESLD.
 #[cfg(any(
     all(target_os = "linux", any(target_arch = "x86_64", target_arch = "x64")),
     target_os = "macos"
 ))]
 #[allow(unused_variables)]
 #[inline]
-fn solve_ols_svd(y: &Array1<f64>, x: &Array2<f64>, rcond: Option<f64>) -> Array1<f64> {
+fn solve_ols_svd<D>(y: &Array<f64, D>, x: &Array2<f64>, rcond: Option<f64>) -> Array<f64, D>
+where
+    D: Dimension,
+    ArrayBase<OwnedRepr<f64>, Dim<[usize; 2]>>: LeastSquaresSvd<OwnedRepr<f64>, f64, D>,
+{
     x.least_squares(y)
         .expect("Failed to compute LAPACK SVD solution!")
         .solution
 }
 
 /// Solves least-squares regression using QR decomposition w/ pivoting.
 #[inline]
@@ -200,14 +241,29 @@
         // compute least squares solution via QR
         solve_ols_qr(y, x)
     } else {
         solve_ols_svd(y, x, rcond)
     }
 }
 
+/// Solve multi-target least squares regression using SVD
+pub fn solve_multi_target(
+    y: &Array2<f64>,
+    x: &Array2<f64>,
+    alpha: Option<f64>,
+    rcond: Option<f64>,
+) -> Array2<f64> {
+    let alpha = alpha.unwrap_or(0.0);
+    if alpha > 0.0 {
+        solve_ridge_svd(y, x, alpha, rcond)
+    } else {
+        solve_ols_svd(y, x, rcond)
+    }
+}
+
 /// Solves least-squares regression using LU with partial pivoting
 #[inline]
 fn solve_ols_lu(y: &Array1<f64>, x: &Array2<f64>) -> Array1<f64> {
     let x_faer = x.view().into_faer();
     x_faer
         .partial_piv_lu()
         .solve(&y.slice(s![.., NewAxis]).into_faer())
```

### Comparing `polars_ols-0.3.1/src/lib.rs` & `polars_ols-0.3.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_ols-0.3.1/tests/benchmark.py` & `polars_ols-0.3.2/tests/benchmark.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,45 @@
 import numpy as np
 import polars as pl
 import pyperf
 import scipy
 import statsmodels.formula.api as smf
-from sklearn.linear_model import ElasticNet, Ridge
+from sklearn.linear_model import ElasticNet, LinearRegression, Ridge
 from statsmodels.regression.recursive_ls import RecursiveLS
 from statsmodels.regression.rolling import RollingOLS
 
 import polars_ols as pls  # import package to register the .least_squares namespace
 from polars_ols.least_squares import SolveMethod
 
 
-def _make_data(n_samples: int = 2_000, n_features: int = 5, sparsity: float = 0.5) -> pl.DataFrame:
-    x = np.random.normal(size=(n_samples, n_features))
-    eps = np.random.normal(size=n_samples, scale=0.1)
-    return pl.DataFrame(data=x, schema=[f"x{i + 1}" for i in range(n_features)]).with_columns(
-        y=pl.lit(x[:, : int(n_features * (1.0 - sparsity))].sum(1) + eps)
-    )
+def _make_data(
+    n_samples: int = 2_000,
+    n_features: int = 5,
+    sparsity: float = 0.5,
+    n_targets: int = 1,
+) -> pl.DataFrame:
+    x = np.random.normal(size=(n_samples, n_features))  # N x K
+    features = pl.DataFrame(data=x, schema=[f"x{i + 1}" for i in range(n_features)])
+    # make single output
+    if n_targets == 1:
+        eps = np.random.normal(size=n_samples, scale=0.1)
+        return features.with_columns(
+            y=pl.lit(x[:, : int(n_features * (1.0 - sparsity))].sum(1) + eps)
+        )
+    # make multi-target
+    else:
+        # create a random linear kernel
+        w = np.random.normal(size=(x.shape[1], n_targets))
+        eps = np.random.normal(size=(n_samples, n_targets), scale=0.1)
+        sparsity_mask = np.random.choice([True, False], size=w.shape, p=[1 - sparsity, sparsity])
+        w *= sparsity_mask
+        y = x @ w + eps
+        return features.with_columns(
+            pl.lit(y).list.to_struct(fields=[f"y{i}" for i in range(n_targets)]).alias("y")
+        )
 
 
 def benchmark_least_squares(data: pl.DataFrame, solve_method: SolveMethod = "qr"):
     return (
         data.lazy()
         .with_columns(
             (
@@ -167,40 +186,67 @@
     res = RecursiveLS(
         df["y"].to_numpy(),
         x,
     ).fit()
     return data.lazy().with_columns(predictions=pl.lit((res.params * x).sum(1))).collect()
 
 
+def benchmark_multi_target(data: pl.DataFrame):
+    return (
+        data.lazy()
+        .with_columns(
+            predictions=pl.col("y").least_squares.multi_target_ols(
+                pl.all().exclude("y"),
+                mode="predictions",
+            )
+        )
+        .collect()
+    )
+
+
+def benchmark_multi_target_sklearn(data: pl.DataFrame):
+    y, x = data.select("y").unnest("y").to_numpy(), data.select(pl.all().exclude("y")).to_numpy()
+    mdl = LinearRegression(fit_intercept=False)
+    mdl.fit(x, y)
+    return data.with_columns(
+        pl.lit(mdl.predict(x)).list.to_struct(fields=[f"y{i}" for i in range(y.shape[1])])
+    )
+
+
 if __name__ == "__main__":
     # example: python tests/benchmark.py --quiet --rigorous
     # we run the benchmarks in python (as opposed to rust) so that overhead of pyO3 is included
-    df = _make_data(n_features=5, n_samples=2_000)
-    runner = pyperf.Runner()
+    df = _make_data(n_features=100, n_samples=10_000)
+    df_multi_target = _make_data(n_features=100, n_targets=20, n_samples=10_000)
 
-    runner.bench_func("benchmark_least_squares_qr", benchmark_least_squares, df, "qr")
+    runner = pyperf.Runner()
     runner.bench_func("benchmark_least_squares_svd", benchmark_least_squares, df, "svd")
-    runner.bench_func("benchmark_ridge_cholesky", benchmark_ridge, df, "chol")
-    runner.bench_func("benchmark_ridge_svd", benchmark_ridge, df, "svd")
-    runner.bench_func("benchmark_wls_from_formula", benchmark_wls_from_formula, df)
-    runner.bench_func("benchmark_elastic_net", benchmark_elastic_net, df, "cd")
-    runner.bench_func(
-        "benchmark_elastic_net_active_set", benchmark_elastic_net, df, "cd_active_set"
-    )
+    runner.bench_func("benchmark_least_squares_qr", benchmark_least_squares, df, "qr")
+    runner.bench_func("benchmark_multi_target", benchmark_multi_target, df_multi_target)
+
+    runner.bench_func("benchmark_least_squares_numpy_svd", benchmark_least_squares_numpy_svd, df)
+    runner.bench_func("benchmark_least_squares_numpy_qr", benchmark_least_squares_numpy_qr, df)
+    runner.bench_func("benchmark_multi_target_sklearn", benchmark_multi_target, df_multi_target)
+
+    # runner.bench_func("benchmark_ridge_cholesky", benchmark_ridge, df, "chol")
+    # runner.bench_func("benchmark_ridge_svd", benchmark_ridge, df, "svd")
+    # runner.bench_func("benchmark_wls_from_formula", benchmark_wls_from_formula, df)
+    # runner.bench_func("benchmark_elastic_net", benchmark_elastic_net, df, "cd")
+    # runner.bench_func(
+    #     "benchmark_elastic_net_active_set", benchmark_elastic_net, df, "cd_active_set"
+    # )
     # runner.bench_func("benchmark_recursive_least_squares", benchmark_recursive_least_squares, df)
     # runner.bench_func("benchmark_rolling_least_squares", benchmark_rolling_least_squares, df)
 
-    runner.bench_func("benchmark_least_squares_numpy_qr", benchmark_least_squares_numpy_qr, df)
-    runner.bench_func("benchmark_least_squares_numpy_svd", benchmark_least_squares_numpy_svd, df)
-    runner.bench_func("benchmark_ridge_sklearn_cholesky", benchmark_ridge_sklearn, df, "cholesky")
-    runner.bench_func("benchmark_ridge_sklearn_svd", benchmark_ridge_sklearn, df, "svd")
-    runner.bench_func(
-        "benchmark_wls_from_formula_statsmodels", benchmark_wls_from_formula_statsmodels, df
-    )
-    runner.bench_func("benchmark_elastic_net_sklearn", benchmark_elastic_net_sklearn, df)
+    # runner.bench_func("benchmark_ridge_sklearn_cholesky", benchmark_ridge_sklearn, df, "cholesky")
+    # runner.bench_func("benchmark_ridge_sklearn_svd", benchmark_ridge_sklearn, df, "svd")
+    # runner.bench_func(
+    #     "benchmark_wls_from_formula_statsmodels", benchmark_wls_from_formula_statsmodels, df
+    # )
+    # runner.bench_func("benchmark_elastic_net_sklearn", benchmark_elastic_net_sklearn, df)
     # runner.bench_func(
     #     "benchmark_recursive_least_squares_statsmodels",
     #     benchmark_recursive_least_squares_statsmodels,
     #     df,
     # )
     # runner.bench_func(
     #     "benchmark_rolling_least_squares_statsmodels",
```

### Comparing `polars_ols-0.3.1/tests/test_ols.py` & `polars_ols-0.3.2/tests/test_ols.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,65 @@
-from typing import Optional
+from typing import Optional, Tuple
 
 import numpy as np
 import polars as pl
 import pytest
 import statsmodels.formula.api as smf
 from sklearn.linear_model import ElasticNet, Ridge
 from statsmodels.regression.rolling import RollingOLS
 
 from polars_ols import (
     NullPolicy,
     OLSKwargs,
     SolveMethod,
     compute_least_squares,
     compute_least_squares_from_formula,
+    compute_multi_target_least_squares,
 )
 from polars_ols.utils import timer
 
 
 def _make_data(
     n_samples: int = 5_000,
     n_features: int = 2,
     n_groups: Optional[int] = None,
     scale: float = 0.1,
     sparsity: float = 0.0,
+    add_missing: bool = False,
+    missing_columns: Optional[Tuple[str, ...]] = None,
 ) -> pl.DataFrame:
     rng = np.random.default_rng(0)
     x = rng.normal(size=(n_samples, n_features))
     eps = rng.normal(size=n_samples, scale=scale)
 
     df = pl.DataFrame(data=x, schema=[f"x{i + 1}" for i in range(n_features)]).with_columns(
         y=pl.lit(x[:, : int(n_features * (1.0 - sparsity))].sum(1) + eps)
     )
 
     if n_groups is not None:
         df = df.with_columns(group=pl.lit(rng.integers(n_groups, size=n_samples)))
 
+    if add_missing:
+
+        def insert_nulls(val):
+            return None if rng.random() < 0.1 else val
+
+        columns = missing_columns or df.columns
+        df = df.with_columns(
+            *(pl.col(c).map_elements(insert_nulls, return_dtype=pl.Float64) for c in columns)
+        )
     return df
 
 
 @pytest.mark.parametrize("solve_method", ("qr", "svd", "chol", "lu", None))
 def test_ols(solve_method: SolveMethod):
     import os
 
     os.environ["POLARS_VERBOSE"] = "1"
-    df = _make_data(n_samples=10, n_features=2)
+    df = _make_data(n_samples=1_000, n_features=2)
     # compute OLS w/ polars-ols
     with timer(f"\nOLS {solve_method}", precision=5):
         for _ in range(1_000):
             expr = compute_least_squares(
                 pl.col("y"),
                 pl.col("x1"),
                 pl.col("x2"),
@@ -59,32 +71,77 @@
         for _ in range(1_000):
             x, y = df.select("x1", "x2").to_numpy(), df.select("y").to_numpy().flatten()
             coef = np.linalg.lstsq(x, y, rcond=None)[0]
             df = df.with_columns(predictions2=pl.lit(x @ coef).flatten())
     assert np.allclose(df["predictions"], df["predictions2"], atol=1.0e-4, rtol=1.0e-4)
 
 
-def test_fit_missing_data_coefficients():
-    df = _make_data()
-    rng = np.random.default_rng(0)
+@pytest.mark.parametrize(
+    "alpha,mode,null_policy",
+    [
+        (0.0, "residuals", "ignore"),
+        (0.0, "residuals", "drop"),
+        (0.0001, "residuals", "drop_y_zero_x"),
+        (0.01, "residuals", "drop_zero"),
+    ],
+)
+def test_multi_target_regression(alpha, mode, null_policy):
+    df = _make_data(
+        n_samples=10_000,
+        n_features=3,
+        add_missing=null_policy not in {"zero", "ignore"},
+        missing_columns=("x1",),
+    )
+    df = df.with_columns(
+        pl.struct(
+            y1=pl.col("x1") + pl.col("x2") + pl.col("x3"),
+            y2=pl.col("x1") - pl.col("x2") + pl.col("x3"),
+            y3=-pl.col("x1") + pl.col("x2") - pl.col("x3"),
+        ).alias("y")
+    )
+    ols_kwargs = OLSKwargs(null_policy=null_policy, solve_method="svd", alpha=alpha)
+
+    with timer(f"compute multi-target (alpha={alpha}, null_policy={null_policy}, mode={mode})"):
+        multi_target = df.select(
+            compute_multi_target_least_squares(
+                "y",
+                "x1",
+                "x2",
+                "x3",
+                mode=mode,
+                ols_kwargs=ols_kwargs,
+            ).alias(mode)
+        )
+
+    with timer("compute multiple linear regressions"):
+        expected = df.unnest("y").select(
+            compute_least_squares(
+                target,
+                "x1",
+                "x2",
+                "x3",
+                mode=mode,
+                ols_kwargs=ols_kwargs,
+            ).alias(target)
+            for target in ("y1", "y2", "y3")
+        )
 
-    def insert_nulls(val):
-        return None if rng.random() < 0.1 else val
+    assert np.allclose(multi_target.unnest(mode), expected, equal_nan=True)
 
-    df = df.with_columns(
-        *(pl.col(c).map_elements(insert_nulls, return_dtype=pl.Float64) for c in df.columns)
-    )
 
-    # in presence of unhandled nulls assert the rust library raises ComputeError
-    with pytest.raises(pl.exceptions.ComputeError):
-        df.select(
-            pl.col("y").least_squares.ols(
-                pl.col("x1"), pl.col("x2"), null_policy="ignore", mode="coefficients"
-            )
-        )
+def test_fit_missing_data_coefficients():
+    df = _make_data(add_missing=True)
+
+    # # in presence of unhandled nulls assert the rust library raises ComputeError
+    # with pytest.raises(pl.exceptions.ComputeError):
+    #     df.select(
+    #         pl.col("y").least_squares.ols(
+    #             pl.col("x1"), pl.col("x2"), null_policy="ignore", mode="coefficients"
+    #         )
+    #     )
 
     # test rust zero policy is sane
     assert np.allclose(
         df.select(
             pl.col("y").least_squares.ols(
                 pl.col("x1"), pl.col("x2"), null_policy="zero", mode="coefficients"
             )
@@ -130,23 +187,15 @@
         )
         .unnest("coefficients"),
     )
 
 
 @pytest.mark.parametrize("null_policy", ["drop", "drop_zero", "drop_y_zero_x"])
 def test_fit_missing_data_predictions_and_residuals(null_policy: NullPolicy):
-    df = _make_data()
-    rng = np.random.default_rng(0)
-
-    def insert_nulls(val):
-        return None if rng.random() < 0.1 else val
-
-    df = df.with_columns(
-        *(pl.col(c).map_elements(insert_nulls, return_dtype=pl.Float64) for c in df.columns)
-    )
+    df = _make_data(add_missing=True)
 
     # check predictions logic
     with timer("numpy lstsq w/ manual nan policy", precision=5):
         # compute desired behaviour for "drop" in numpy:
         x, y = (
             df.select("x1", "x2").to_numpy(),
             df.select("y").to_numpy().flatten(),
@@ -687,23 +736,15 @@
         (10, 2, True),
         (63, 5, False),
         (252, 5, False),
         (252, 5, True),
     ],
 )
 def test_rolling_least_squares(window_size: int, min_periods: int, use_woodbury: bool):
-    df = _make_data(n_samples=1_000)
-    rng = np.random.default_rng(0)
-
-    def insert_nulls(val):
-        return None if rng.random() < 0.1 else val
-
-    df = df.with_columns(
-        *(pl.col(c).map_elements(insert_nulls, return_dtype=pl.Float64) for c in ("y",))
-    )
+    df = _make_data(n_samples=1_000, add_missing=True, missing_columns=("y",))
 
     with timer("\nrolling ols"):
         coef_rolling = (
             df.lazy()
             .select(
                 pl.col("y")
                 .least_squares.rolling_ols(
@@ -776,24 +817,15 @@
         )
 
     assert coef_rolling.count().max_horizontal().item() == expected
 
 
 @pytest.mark.parametrize("window_size", (21, 252))
 def test_rolling_window_drop(window_size: int):
-    df = _make_data(n_samples=1_000)
-    rng = np.random.default_rng(0)
-
-    def insert_nulls(val):
-        return None if rng.random() < 0.1 else val
-
-    df = df.with_columns(
-        *(pl.col(c).map_elements(insert_nulls, return_dtype=pl.Float64) for c in ("y",))
-    ).with_row_index()
-
+    df = _make_data(n_samples=1_000, add_missing=True, missing_columns=("y",)).with_row_index()
     df_drop = df.drop_nulls()
 
     df_merged = (
         df_drop.lazy()
         .select(
             "index",
             pl.col("y")
```

### Comparing `polars_ols-0.3.1/Cargo.lock` & `polars_ols-0.3.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1912,15 +1912,15 @@
  "stacker",
  "sysinfo",
  "version_check",
 ]
 
 [[package]]
 name = "polars_ols"
-version = "0.3.1"
+version = "0.3.2"
 dependencies = [
  "approx",
  "blas-src",
  "faer",
  "faer-ext",
  "jemallocator",
  "lapack-src",
```

### Comparing `polars_ols-0.3.1/pyproject.toml` & `polars_ols-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polars_ols-0.3.1/PKG-INFO` & `polars_ols-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: polars-ols
-Version: 0.3.1
+Version: 0.3.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: polars >=0.20.16
 Requires-Dist: numpy ; extra == 'dev'
 Requires-Dist: pytest >=7.4.1 ; extra == 'dev'
 Requires-Dist: pre-commit ; extra == 'dev'
```

