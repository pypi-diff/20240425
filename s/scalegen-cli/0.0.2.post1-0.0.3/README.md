# Comparing `tmp/scalegen-cli-0.0.2.post1.tar.gz` & `tmp/scalegen-cli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalegen-cli-0.0.2.post1.tar", last modified: Wed Mar 20 10:44:23 2024, max compression
+gzip compressed data, was "scalegen-cli-0.0.3.tar", last modified: Thu Apr 25 11:39:02 2024, max compression
```

## Comparing `scalegen-cli-0.0.2.post1.tar` & `scalegen-cli-0.0.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:44:23.547638 scalegen-cli-0.0.2.post1/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-20 10:44:23.543638 scalegen-cli-0.0.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:44:23.543638 scalegen-cli-0.0.2.post1/scalegen_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-20 10:44:23.000000 scalegen-cli-0.0.2.post1/scalegen_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-20 10:44:23.000000 scalegen-cli-0.0.2.post1/scalegen_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 10:44:23.000000 scalegen-cli-0.0.2.post1/scalegen_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-20 10:44:23.000000 scalegen-cli-0.0.2.post1/scalegen_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-20 10:44:23.000000 scalegen-cli-0.0.2.post1/scalegen_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-20 10:44:23.000000 scalegen-cli-0.0.2.post1/scalegen_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 10:44:23.547638 scalegen-cli-0.0.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:44:23.543638 scalegen-cli-0.0.2.post1/st_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:44:23.543638 scalegen-cli-0.0.2.post1/st_cli/datamodels/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/datamodels/.git
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/datamodels/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/datamodels/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:44:23.543638 scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:44:23.543638 scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/api/
--rw-r--r--   0 runner    (1001) docker     (127)    17733 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:44:23.543638 scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:44:23.543638 scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/common/
--rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:44:23.543638 scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/jc/
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/jc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/datamodels/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/launch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/login.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    12220 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/sg_finetune.py
--rw-r--r--   0 runner    (1001) docker     (127)    16319 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/sg_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/stop.py
--rw-r--r--   0 runner    (1001) docker     (127)    12088 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/visualisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9318 2024-03-20 10:44:17.000000 scalegen-cli-0.0.2.post1/st_cli/workstation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:39:02.416766 scalegen-cli-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-25 11:39:02.416766 scalegen-cli-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:39:02.408766 scalegen-cli-0.0.3/scalegen_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-25 11:39:02.000000 scalegen-cli-0.0.3/scalegen_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-25 11:39:02.000000 scalegen-cli-0.0.3/scalegen_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 11:39:02.000000 scalegen-cli-0.0.3/scalegen_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-25 11:39:02.000000 scalegen-cli-0.0.3/scalegen_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-25 11:39:02.000000 scalegen-cli-0.0.3/scalegen_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 11:39:02.000000 scalegen-cli-0.0.3/scalegen_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 11:39:02.416766 scalegen-cli-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:39:02.412766 scalegen-cli-0.0.3/st_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:39:02.412766 scalegen-cli-0.0.3/st_cli/datamodels/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/datamodels/.git
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/datamodels/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/datamodels/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:39:02.412766 scalegen-cli-0.0.3/st_cli/datamodels/datamodels/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/datamodels/datamodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:39:02.412766 scalegen-cli-0.0.3/st_cli/datamodels/datamodels/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    18490 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/datamodels/datamodels/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:39:02.412766 scalegen-cli-0.0.3/st_cli/datamodels/datamodels/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/datamodels/datamodels/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:39:02.412766 scalegen-cli-0.0.3/st_cli/datamodels/datamodels/common/
+-rw-r--r--   0 runner    (1001) docker     (127)    13925 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/datamodels/datamodels/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:39:02.412766 scalegen-cli-0.0.3/st_cli/datamodels/datamodels/jc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/datamodels/datamodels/jc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/datamodels/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/sg_finetune.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25159 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/sg_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14098 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/visualisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9318 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/workstation.py
```

### Comparing `scalegen-cli-0.0.2.post1/scalegen_cli.egg-info/SOURCES.txt` & `scalegen-cli-0.0.3/scalegen_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2.post1/setup.py` & `scalegen-cli-0.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 from setuptools import setup, find_packages
 import os
+import requests
+from distutils.version import LooseVersion
 
-application_version = os.environ.get("APP_VERSION", "0.0.0")
+
+def versions(package_name, limit_releases=10):
+    url = f"https://pypi.org/pypi/{package_name}/json"
+    data = requests.get(url).json()
+    versions = list(data["releases"].keys())
+    versions.sort(key=LooseVersion, reverse=True)
+    return versions[:limit_releases]
+
+
+# application_version = os.environ.get("APP_VERSION", "0.0.0")
+application_version = "0.0." + str(int(versions("scalegen-cli")[0].split(".")[2]) + 1)
 
 with open("requirements.txt", "r") as fp:
     reqs = [line.strip("\n") for line in fp]
 
 binary = "scaletorch"
 if os.environ.get("PRODUCT_TYPE", "scaletorch") == "scalegen":
     binary = "scalegen"
 
 setup(
     name=f"scalegen-cli",
     version=application_version,
-    description="ScaleTorch CLI",
-    long_description="Scalegen command line application",
+    description="ScaleGenAI CLI",
+    long_description="ScaleGenAI command line application",
     url="https://github.com/ScaleTorch/st-cli",
     packages=find_packages(),
     include_package_data=True,
     python_requires=">=3.6, <3.12",
     install_requires=reqs,
     entry_points={"console_scripts": [f"{binary} = st_cli:cli"]},
 )
```

### Comparing `scalegen-cli-0.0.2.post1/st_cli/client.py` & `scalegen-cli-0.0.3/st_cli/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,20 +80,21 @@
 #     # TODO: Needs to return B2 bucket name for the user, B2 creds, Encryption Key
 #     resp = send_request('POST', '/keys')
 
 #     creds = read_credentials()
 #     raw_data = resp.raw.read()
 #     # Decrypt the response
 
+
 def get_garb(key: str) -> str:
     # Fetch it from API
     resp = send_request("GET", f"/secret/{key}")
     if resp.status_code == 200:
         content = resp.json()["secret"][key]
         # if "GS_CREDS" in key or "GDRIVE_CREDS" in key:
         #     content = base64.b64decode(content.encode()).decode("utf8")
 
         # if not content:
         #     logger.warning(f"garb: {key} is empty!")
         return content
-    
-    return ''
+
+    return ""
```

### Comparing `scalegen-cli-0.0.2.post1/st_cli/datamodels/.gitignore` & `scalegen-cli-0.0.3/st_cli/datamodels/.gitignore`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/api/__init__.py` & `scalegen-cli-0.0.3/st_cli/datamodels/datamodels/api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from decimal import Decimal
-from typing import Union, Literal
+from typing import Union, Literal, List, Optional, Any, Set
 
 from pydantic import Field, model_validator
 
 from ..common import *
 
 
 class ServicePlan(str, Enum):
@@ -336,74 +336,98 @@
 
 # On-prem models
 
 
 class OnPremNodeIn(BaseModel):
     ip: str
     username: str
-    role: VMRole
     ssh_private_key: str
     port: int
     private_ip: Optional[str] = None
+    cpu_only: bool
 
 
 class OnPremNodeDB(OnPremNodeIn):
     id: str
     ssh_key_id: str
+    role: Optional[VMRole] = None
     vcpus: int
     memory: int
     verified: bool
     verification_message: str
     gpu_type: GPUType
     gpu_count: int
     user_id: str
 
 
+class OnPremNodeCandidate(OnPremNodeDB):
+    available_resources: List[str]
+
+
+class OnPremJournalStatus(str, Enum):
+    ACTIVE = "ACTIVE"
+    INACTIVE = "INACTIVE"
+
+
+class OnPremNodeJournal(BaseModel):
+    id: str
+    user_id: str
+    timestamp: str
+    status: OnPremJournalStatus
+    role: VMRole
+    on_prem_node_id: str
+    job_id: str
+    gpu_ids: Set[str]
+
+
 class OnPremNodeEditIn(OnPremNodeIn):
     id: str
 
 
 # Inference Models
 
 
 class InferenceDeploymentInitialWorkersConfig(BaseModel):
     min_workers: int = 0
     initial_workers_gpu: Optional[GPUType] = None
     initial_workers_gpu_num: Optional[int] = None
-    use_same_gpus_when_scaling: Optional[bool] = False
+    use_other_gpus: Optional[bool] = False
     instance_types: Optional[List[str]] = None
     use_on_prem: Optional[bool] = False
     use_cloudburst: Optional[bool] = False
     on_prem_node_ids: Optional[List[str]] = None
 
 
 class InferenceDeploymentAutoscalingConfig(BaseModel):
-    time_window_sec: Optional[int] = 5*60
-    upper_allowed_latency_sec: Optional[float] = 4
-    lower_allowed_latency_sec: Optional[float] = 1
-    scaling_up_timeout_sec: Optional[int] = 20*60
-    scaling_down_timeout_sec: Optional[int] = 20*60
-    scale_to_zero_timeout_sec: Optional[int] = 30*60
+    scale_up_time_window_sec: Optional[int] = 5 * 60
+    scale_down_time_window_sec: Optional[int] = 5 * 60
+    upper_allowed_latency_sec: Optional[float] = 1
+    lower_allowed_latency_sec: Optional[float] = 0.2
+    scaling_up_timeout_sec: Optional[int] = 20 * 60
+    scaling_down_timeout_sec: Optional[int] = 20 * 60
+    scale_to_zero_timeout_sec: Optional[int] = 30 * 60
     enable_speedup_shared: Optional[bool] = False
+    scale_to_zero: Optional[bool] = False
 
 
-class InferenceDeploymentGatewaycloudChoice(BaseModel):
-    name: ProviderEnum  
+class InferenceDeploymentGatewayCloudChoice(BaseModel):
+    name: ProviderEnum
     region: str
 
+
 class InferenceDeploymentIn(BaseModel):
     name: str
     model: str
     base_model: Optional[str] = None
     inf_type: InferenceDeploymentType = InferenceDeploymentType.llm
     hf_token: Optional[str] = None
     allow_spot_instances: bool = False
     logs_store: Optional[str] = None
     cloud_providers: Optional[List[CloudProviderChoice]] = []
-    gateway_config: Optional[InferenceDeploymentGatewaycloudChoice] = None
+    gateway_config: InferenceDeploymentGatewayCloudChoice
     initial_worker_config: Optional[InferenceDeploymentInitialWorkersConfig] = None
     autoscaling_config: Optional[InferenceDeploymentAutoscalingConfig] = (
         InferenceDeploymentAutoscalingConfig()
     )
     max_price_per_hour: Optional[float] = None
     min_throughput_rate: Optional[float] = None
 
@@ -441,18 +465,18 @@
 class EstimatedPrice(BaseModel):
     on_demand_price: MinMaxPrice
     spot_price: MinMaxPrice
 
 
 class InferenceDeploymentUpdateIn(BaseModel):
     # Initial worker params
-    initial_worker_config: InferenceDeploymentInitialWorkersConfig = None
+    initial_worker_config: Optional[InferenceDeploymentInitialWorkersConfig] = None
 
     # Auto scaling parameters
-    autoscaling_config: InferenceDeploymentAutoscalingConfig = None
+    autoscaling_config: Optional[InferenceDeploymentAutoscalingConfig] = None
     imidiate_scale_down: Optional[bool] = False
 
     max_price_per_hour: Optional[float] = None
     min_throughput_rate: Optional[float] = None
     allow_spot_instances: Optional[bool] = None
 
 
@@ -466,24 +490,34 @@
     PROVISIONING = "PROVISIONING"
     DELETED = "DELETED"
     FAILED = "FAILED"
     DELETING = "DELETING"
     SCALING = "SCALING"
 
 
+class InferenceDeploymentAPIGatewayData(BaseModel):
+    provider: ProviderEnum
+    api_id: str
+    hash_value: str
+    endpoint: str
+    region: str
+
+
 class InferenceDeploymentDB(InferenceDeploymentIn):
     id: str
     user_id: str
     status: InferenceDeploymentStatus
     current_price_per_hour: float
     cost: Decimal = Decimal(0.00)
     last_cost_updated_time: Optional[str] = None
     timestamp: str
     link: Optional[str] = None
     metadata: Optional[dict] = {}
+    api_gateway_data: Optional[InferenceDeploymentAPIGatewayData] = None
+
 
 class InferenceSupportedModelOut(BaseModel):
     model: str
     type: InferenceDeploymentType
 
 
 class NodeIP(BaseModel):
```

### Comparing `scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/cli/__init__.py` & `scalegen-cli-0.0.3/st_cli/datamodels/datamodels/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/common/__init__.py` & `scalegen-cli-0.0.3/st_cli/datamodels/datamodels/common/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -99,52 +99,88 @@
     CodeCopyType.AZURE: ["AZURE_ACCOUNT_NAME", "AZURE_ACCOUNT_KEY"],
     CodeCopyType.GS: ["GS_CREDS"],
     CodeCopyType.GDRIVE: ["GDRIVE_CREDS"],
     CodeCopyType.DROPBOX: ["DROPBOX_TOKEN"],
     CodeCopyType.B2: [],
 }
 
+
 class GPUType(str, Enum):
+    A10G = "A10G"
+    A30 = "A30"
+    A40 = "A40"
     A100 = "A100"
     A100_80GB = "A100_80GB"
+    GH201 = "GH201"
     H100_80GB = "H100_80GB"
-    A10G = "A10G"
-    T4 = "T4"
-    V100 = "V100"
-    RTX_3090 = "RTX_3090"
-    RTX_4090 = "RTX_4090"
-    RTX_A6000 = "RTX_A6000"
-    RTX_A5000 = "RTX_A5000"
-    RTX_A4000 = "RTX_A4000"
-    RTX_6000_ADA = "RTX_6000_ADA"
+    K80 = "K80"
+    L4 = "L4"
     L40 = "L40"
-    A40 = "A40"
-    
-    A30 = "A30"
+    M60 = "M60"
+    P40 = "P40"
+    P100 = "P100"
     RTX_3070 = "RTX_3070"
     RTX_3080 = "RTX_3080"
     RTX_3080_TI = "RTX_3080_TI"
+    RTX_3090 = "RTX_3090"
     RTX_3090_TI = "RTX_3090_TI"
-    RTX_4080 = "RTX_4080"
+    RTX_4000 = "RTX_4000"
     RTX_4070 = "RTX_4070"
     RTX_4070_TI = "RTX_4070_TI"
-    RTX_4000 = "RTX_4000"
+    RTX_4080 = "RTX_4080"
+    RTX_4090 = "RTX_4090"
+    RTX_6000_ADA = "RTX_6000_ADA"
     RTX_A2000 = "RTX_A2000"
+    RTX_A4000 = "RTX_A4000"
     RTX_A4500 = "RTX_A4500"
-    L4 = "L4"
-
-    M60 = "M60"
-    P100 = "P100"
-    K80 = "K80"
-    P40 = "P40"
+    RTX_A5000 = "RTX_A5000"
+    RTX_A6000 = "RTX_A6000"
+    T4 = "T4"
+    V100 = "V100"
     V520 = "V520"
 
     EMPTY = ""
 
 
+on_prem_gpu_type_map = {
+    GPUType.A10G: ["a10"],
+    GPUType.A30: ["a30"],
+    GPUType.A40: ["a40"],
+    GPUType.A100: ["a100", "40gb"],
+    GPUType.A100_80GB: ["a100", "80gb"],
+    GPUType.GH201: ["xxxx"],  # TODO
+    GPUType.H100_80GB: ["h100"],
+    GPUType.K80: ["k80"],
+    GPUType.L4: ["l4"],
+    GPUType.L40: ["l40"],
+    GPUType.M60: ["m60"],
+    GPUType.P40: ["p40"],
+    GPUType.P100: ["p100"],
+    GPUType.RTX_3070: ["3070", "rtx"],
+    GPUType.RTX_3080: ["3080", "rtx"],
+    GPUType.RTX_3080_TI: ["rtx", "3080", "ti"],
+    GPUType.RTX_3090: ["3090", "rtx"],
+    GPUType.RTX_3090_TI: ["rtx", "3090", "ti"],
+    GPUType.RTX_4000: ["rtx", "4000"],
+    GPUType.RTX_4070: ["rtx", "4070"],
+    GPUType.RTX_4070_TI: ["rtx", "4070", "ti"],
+    GPUType.RTX_4080: ["rtx", "4080"],
+    GPUType.RTX_4090: ["rtx", "4090"],
+    GPUType.RTX_6000_ADA: ["rtx", "6000", "ada"],
+    GPUType.RTX_A2000: ["rtx", "a2000"],
+    GPUType.RTX_A4000: ["rtx", "a4000"],
+    GPUType.RTX_A4500: ["rtx", "a4500"],
+    GPUType.RTX_A5000: ["rtx", "a5000"],
+    GPUType.RTX_A6000: ["rtx", "a6000"],
+    GPUType.T4: ["t4"],
+    GPUType.V100: ["v100"],
+    GPUType.V520: ["v520"],
+}
+
+
 # Classes for Config
 class SearchSpaceElement(BaseModel):
     type: str
     value: List
 
 
 class Tuner(BaseModel):
@@ -402,28 +438,31 @@
 class Node(VirtualMachine):
     role: VMRole
     instance_type: str
     status: str
     job_id: str
     user_id: Optional[str] = None
     gpu_count: int = 0
-    gpu_type: Optional[GPUType] = None
+    gpu_type: GPUType = GPUType.EMPTY
     region: str
     timestamp: Optional[str] = None
     spot: bool
     to_be_persisted: bool = False
     auditor_status: Optional[NodeStatus] = NodeStatus.UNKNOWN
     ssh_key_id: Optional[str] = None
     excess: bool = False
 
     # If metadata is not present in the db, it will be set to {}
     def __init__(self, **data: Any):
         if data.get("metadata") is None:
             data["metadata"] = {}
 
+        if data.get("gpu_type") is None:
+            data["gpu_type"] = GPUType.EMPTY.value
+
         super().__init__(**data)
 
 
 class OnPremNode(Node):
     vcpus: Optional[int] = 0
     memory: Optional[int] = 0
     verified: bool = False
@@ -468,7 +507,16 @@
 
 class InferenceRecipe(BaseModel):
     model: str
     id: str
     gpu_reqs: Dict[GPUType, int]
     is_embeddings: Optional[bool] = False
     type: InferenceDeploymentType
+
+
+class InfPerformanceResult(BaseModel):
+    id: str
+    gpu_type: GPUType
+    llmperf_results: Dict[str, Any]
+    max_model_len: Optional[int] = None
+    num_gpus: int
+    results_mean_output_throughput_token_per_s: float
```

### Comparing `scalegen-cli-0.0.2.post1/st_cli/datamodels/datamodels/jc/__init__.py` & `scalegen-cli-0.0.3/st_cli/datamodels/datamodels/jc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 
 
 class ScaleInferenceDeploymentTaskPayload(TaskPayloadBase):
     scale: str
     vm_num: int = 1
     target_throughput: Optional[float] = None
     use_initial_config: bool = False
+    created_by: Optional[str] = None
 
 
 task_to_payload_type = {
     TaskType.CLEANUP: TaskPayloadBase,
     TaskType.SETUP_JOB: SetupJobTaskPayload,
     TaskType.DELETE_JOB: DeleteJobTaskPayload,
     TaskType.DELETE_DAPP_JOB: TaskPayloadBase,
```

### Comparing `scalegen-cli-0.0.2.post1/st_cli/job.py` & `scalegen-cli-0.0.3/st_cli/job.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2.post1/st_cli/launch.py` & `scalegen-cli-0.0.3/st_cli/launch.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2.post1/st_cli/list.py` & `scalegen-cli-0.0.3/st_cli/list.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2.post1/st_cli/login.py` & `scalegen-cli-0.0.3/st_cli/login.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2.post1/st_cli/main.py` & `scalegen-cli-0.0.3/st_cli/main.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2.post1/st_cli/sg_finetune.py` & `scalegen-cli-0.0.3/st_cli/sg_finetune.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import Optional
-
 import click
 from rich import box
 from rich.console import Console
 from rich.table import Table
 
 from .client import send_request
 from .utils import display_event_logs
@@ -32,27 +31,26 @@
 finetune.add_command(stop, name="stop")
 finetune.add_command(view, name="view")
 finetune.add_command(launch, name="launch")
 
 
 @finetune.command(name="create")
 # ******************************* JOB ARGS *******************************
-# @click.option('-e', '--env_var', type=click.STRING, required=False, multiple=True)
-# @click.option("--use_env", is_flag=True)
-# @click.option('-f', '--force', is_flag=True)
 @click.option("-q", "--quiet", is_flag=True, help="Display status updates of workload")
 @click.option(
     "--task",
-    type=click.Choice(["llm", "seq2seq", "text_classification", "token_classification"]),
+    type=click.Choice(
+        ["llm", "seq2seq", "text_classification", "token_classification"]
+    ),
     required=False,
     default="llm",
 )
 @click.option("--job_name", type=click.STRING, required=False)
 @click.option("--artifacts_storage", type=click.STRING, required=False)
-@click.option("--use_spot", is_flag=True, required=False)
+@click.option("--allow_spot_instances", is_flag=True, required=False)
 # ******************************* FINETUNE ARGS *******************************
 @click.option("--model", required=True, type=click.STRING, help="Model to use")
 @click.option(
     "--data_path",
     required=True,
     type=click.STRING,
     help="Data path to use. Can be a hugging face dataset or name of a virtual mount (filename is set with user_dataset)",
@@ -150,15 +148,18 @@
     "--block_size",
     required=False,
     type=click.STRING,
     default="-1",
     help="Block size to use",
 )
 @click.option(
-    "--project_name", required=False, type=click.STRING, help="Project name in Hugging Face hub"
+    "--project_name",
+    required=False,
+    type=click.STRING,
+    help="Project name in Hugging Face hub",
 )
 @click.option(
     "--model_max_length",
     required=False,
     type=click.INT,
     default=1024,
     help="Model max length to use",
@@ -210,15 +211,15 @@
 def create(**finetune_kwargs):
     """
     Function responsible for launching a scalegen finetune workload from the CLI
     """
 
     # Make request to P-API
     data = {
-        "use_spot": finetune_kwargs["use_spot"],
+        "use_spot": finetune_kwargs["allow_spot_instances"],
         "wandb_key": finetune_kwargs["wandb_key"],
         "model": finetune_kwargs["model"],
         "data_path": finetune_kwargs["data_path"],
         "job_name": finetune_kwargs["job_name"],
         "user_dataset": finetune_kwargs["user_dataset"],
         "hf_token": finetune_kwargs["hf_token"],
         "artifacts_storage": finetune_kwargs["artifacts_storage"],
@@ -332,16 +333,20 @@
         for col in ["ID", "Name", "Model", "Data", "Status"]:
             table.add_column(col, justify="left")
 
         for job in resp_data:
             if all or (
                 not all and (job["status"] == "RUNNING" or job["status"] == "QUEUED")
             ):
-                model = find_next_word_in_string(job["spec"]["config"]["entrypoint"], "--model")
-                data = find_next_word_in_string(job["spec"]["config"]["entrypoint"], "--data_path")
+                model = find_next_word_in_string(
+                    job["spec"]["config"]["entrypoint"], "--model"
+                )
+                data = find_next_word_in_string(
+                    job["spec"]["config"]["entrypoint"], "--data_path"
+                )
                 table.add_row(job["id"], job["name"], model, data, job["status"])
 
     if table.row_count <= 15:
         console.print(table, justify="left")
     else:
         with console.pager():
             console.print(table, justify="left")
```

### Comparing `scalegen-cli-0.0.2.post1/st_cli/stop.py` & `scalegen-cli-0.0.3/st_cli/stop.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2.post1/st_cli/utils.py` & `scalegen-cli-0.0.3/st_cli/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import requests
 from rich.progress import track
 from rich.live import Live
 from rich.table import Table
 from rich.text import Text
 import threading
 from typing import Dict
+from gettext import gettext as _
 
 
 from .datamodels.datamodels import CodeCopy, CodeCopyType
 from .const import MAX_FILES, MAX_SIZE_MB, PRODUCT_TYPE, UPLOAD_WORKERS
 from .client import send_request
 
 
@@ -381,7 +382,53 @@
 
 def print_to_string(*args, **kwargs):
     output = io.StringIO()
     print(*args, file=output, **kwargs)
     contents = output.getvalue()
     output.close()
     return contents
+
+
+class CategorizedMutuallyExclusiveOption(click.Option):
+    def __init__(self, *args, **kwargs):
+        self.mutually_exclusive = set(kwargs.pop("mutually_exclusive", []))
+        self.category = kwargs.pop("category", "Common options")
+        help = kwargs.get("help", "")
+        if self.mutually_exclusive:
+            ex_str = ", ".join(self.mutually_exclusive)
+            kwargs["help"] = help + click.style(
+                " NOTE: This argument is mutually exclusive with"
+                " arguments: (" + ex_str + ").",
+                italic=True,
+            )
+        super(CategorizedMutuallyExclusiveOption, self).__init__(*args, **kwargs)
+
+    def handle_parse_result(self, ctx, opts, args):
+        if self.mutually_exclusive.intersection(opts) and self.name in opts:
+            raise click.UsageError(
+                "Illegal usage: `{}` is mutually exclusive with "
+                "arguments `{}`.".format(self.name, ", ".join(self.mutually_exclusive))
+            )
+        return super(CategorizedMutuallyExclusiveOption, self).handle_parse_result(
+            ctx, opts, args
+        )
+
+
+class PatchedCommand(click.Command):
+    def format_options(
+        self, ctx: click.Context, formatter: click.HelpFormatter
+    ) -> None:
+        """Writes all the options into the formatter if they exist."""
+        categories = {}
+        for param in self.get_params(ctx):
+            rv = param.get_help_record(ctx)
+            if hasattr(param, "category") and rv is not None:
+                categories.setdefault(param.category, []).append(rv)
+            elif not hasattr(param, "category") and rv is not None:
+                categories.setdefault("Common options", []).append(rv)
+
+        if categories:
+
+            with formatter.section(_("Options")):
+                for group_name, opts in categories.items():
+                    with formatter.section(group_name):
+                        formatter.write_dl(opts, col_max=40, col_spacing=4)
```

### Comparing `scalegen-cli-0.0.2.post1/st_cli/view.py` & `scalegen-cli-0.0.3/st_cli/view.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2.post1/st_cli/visualisation.py` & `scalegen-cli-0.0.3/st_cli/visualisation.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.2.post1/st_cli/workstation.py` & `scalegen-cli-0.0.3/st_cli/workstation.py`

 * *Files identical despite different names*

