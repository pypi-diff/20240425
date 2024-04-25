# Comparing `tmp/pyorchestra-0.6.1.tar.gz` & `tmp/pyorchestra-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyorchestra-0.6.1.tar", max compression
+gzip compressed data, was "pyorchestra-0.6.2.tar", max compression
```

## Comparing `pyorchestra-0.6.1.tar` & `pyorchestra-0.6.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     7652 2024-04-19 15:24:00.264519 pyorchestra-0.6.1/LICENSE
--rwxr-xr-x   0        0        0    25961 2024-04-19 15:24:00.264519 pyorchestra-0.6.1/README.md
--rwxr-xr-x   0        0        0       62 2024-04-19 15:24:00.264519 pyorchestra-0.6.1/orchestra/__init__.py
--rwxr-xr-x   0        0        0      265 2024-04-19 15:24:00.264519 pyorchestra-0.6.1/orchestra/api/dto/__init__.py
--rwxr-xr-x   0        0        0     2514 2024-04-19 15:24:00.264519 pyorchestra-0.6.1/orchestra/api/dto/job.py
--rwxr-xr-x   0        0        0      844 2024-04-19 15:24:00.264519 pyorchestra-0.6.1/orchestra/api/dto/run.py
--rwxr-xr-x   0        0        0      786 2024-04-19 15:24:00.268519 pyorchestra-0.6.1/orchestra/api/dto/schedule_definition.py
--rwxr-xr-x   0        0        0     1294 2024-04-19 15:24:00.268519 pyorchestra-0.6.1/orchestra/api/dto/task.py
--rwxr-xr-x   0        0        0      656 2024-04-19 15:24:00.268519 pyorchestra-0.6.1/orchestra/api/main.py
--rwxr-xr-x   0        0        0    10318 2024-04-19 15:24:00.268519 pyorchestra-0.6.1/orchestra/api/routers/jobs.py
--rwxr-xr-x   0        0        0      531 2024-04-19 15:24:00.268519 pyorchestra-0.6.1/orchestra/api/routers/tags.py
--rwxr-xr-x   0        0        0      603 2024-04-19 15:24:00.268519 pyorchestra-0.6.1/orchestra/api/routers/tasks.py
--rwxr-xr-x   0        0        0     1839 2024-04-19 15:24:00.268519 pyorchestra-0.6.1/orchestra/backend.py
--rwxr-xr-x   0        0        0    20422 2024-04-19 15:24:00.268519 pyorchestra-0.6.1/orchestra/core.py
--rwxr-xr-x   0        0        0     1104 2024-04-19 15:24:00.268519 pyorchestra-0.6.1/orchestra/formatting.py
--rwxr-xr-x   0        0        0      168 2024-04-19 15:24:00.268519 pyorchestra-0.6.1/orchestra/job.py
--rwxr-xr-x   0        0        0     1575 2024-04-19 15:24:00.268519 pyorchestra-0.6.1/orchestra/models.py
--rwxr-xr-x   0        0        0    10840 2024-04-19 15:24:00.268519 pyorchestra-0.6.1/orchestra/scheduling.py
--rwxr-xr-x   0        0        0     1104 2024-04-19 15:24:00.268519 pyorchestra-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    26835 1970-01-01 00:00:00.000000 pyorchestra-0.6.1/PKG-INFO
+-rwxr-xr-x   0        0        0     7652 2024-04-25 07:24:25.946858 pyorchestra-0.6.2/LICENSE
+-rwxr-xr-x   0        0        0    25961 2024-04-25 07:24:25.946858 pyorchestra-0.6.2/README.md
+-rwxr-xr-x   0        0        0       62 2024-04-25 07:24:25.946858 pyorchestra-0.6.2/orchestra/__init__.py
+-rwxr-xr-x   0        0        0      265 2024-04-25 07:24:25.946858 pyorchestra-0.6.2/orchestra/api/dto/__init__.py
+-rwxr-xr-x   0        0        0     2514 2024-04-25 07:24:25.946858 pyorchestra-0.6.2/orchestra/api/dto/job.py
+-rwxr-xr-x   0        0        0      844 2024-04-25 07:24:25.946858 pyorchestra-0.6.2/orchestra/api/dto/run.py
+-rwxr-xr-x   0        0        0      786 2024-04-25 07:24:25.946858 pyorchestra-0.6.2/orchestra/api/dto/schedule_definition.py
+-rwxr-xr-x   0        0        0     1416 2024-04-25 07:24:25.946858 pyorchestra-0.6.2/orchestra/api/dto/task.py
+-rwxr-xr-x   0        0        0      656 2024-04-25 07:24:25.946858 pyorchestra-0.6.2/orchestra/api/main.py
+-rwxr-xr-x   0        0        0    10318 2024-04-25 07:24:25.946858 pyorchestra-0.6.2/orchestra/api/routers/jobs.py
+-rwxr-xr-x   0        0        0      531 2024-04-25 07:24:25.946858 pyorchestra-0.6.2/orchestra/api/routers/tags.py
+-rwxr-xr-x   0        0        0      603 2024-04-25 07:24:25.946858 pyorchestra-0.6.2/orchestra/api/routers/tasks.py
+-rwxr-xr-x   0        0        0     1839 2024-04-25 07:24:25.946858 pyorchestra-0.6.2/orchestra/backend.py
+-rwxr-xr-x   0        0        0    20422 2024-04-25 07:24:25.946858 pyorchestra-0.6.2/orchestra/core.py
+-rwxr-xr-x   0        0        0     1104 2024-04-25 07:24:25.946858 pyorchestra-0.6.2/orchestra/formatting.py
+-rwxr-xr-x   0        0        0      168 2024-04-25 07:24:25.946858 pyorchestra-0.6.2/orchestra/job.py
+-rwxr-xr-x   0        0        0     1575 2024-04-25 07:24:25.946858 pyorchestra-0.6.2/orchestra/models.py
+-rwxr-xr-x   0        0        0    10840 2024-04-25 07:24:25.946858 pyorchestra-0.6.2/orchestra/scheduling.py
+-rwxr-xr-x   0        0        0     1104 2024-04-25 07:24:25.950857 pyorchestra-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0    26835 1970-01-01 00:00:00.000000 pyorchestra-0.6.2/PKG-INFO
```

### Comparing `pyorchestra-0.6.1/LICENSE` & `pyorchestra-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.6.1/README.md` & `pyorchestra-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.6.1/orchestra/api/dto/job.py` & `pyorchestra-0.6.2/orchestra/api/dto/job.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.6.1/orchestra/api/dto/run.py` & `pyorchestra-0.6.2/orchestra/api/dto/run.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.6.1/orchestra/api/dto/schedule_definition.py` & `pyorchestra-0.6.2/orchestra/api/dto/schedule_definition.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.6.1/orchestra/api/dto/task.py` & `pyorchestra-0.6.2/orchestra/api/dto/task.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import json
 import datetime
 from typing import Any
 
+import pytz
 from pydantic import BaseModel
 
 from orchestra.models import TimingAwareTask, Status
 
 
 class TaskDTO(BaseModel):
     id: int
     task_id: str
     run_id: int
     job_name: str
     status: Status
     result: Any
-    date_done: datetime.datetime
+    date_done: datetime.datetime | None
     traceback: str | None
     args: list
     kwargs: dict
     worker: str
     retries: int
     queue: str
     date_created: datetime.datetime
@@ -28,17 +29,17 @@
     def map(cls, task: TimingAwareTask) -> "TaskDTO":
         return TaskDTO(id=task.id,
                        task_id=task.task_id,
                        run_id=task.run_id,
                        job_name=task.job_name,
                        status=Status[task.status.lower()],
                        result=task.result,
-                       date_done=task.date_done,
+                       date_done=task.date_done.replace(tzinfo=pytz.utc) if task.date_done else None,
                        traceback=task.traceback,
                        args=json.loads(task.args.decode("utf-8")),
                        kwargs=json.loads(task.kwargs.decode("utf-8")),
                        worker=task.worker,
                        retries=task.retries,
                        queue=task.queue,
-                       date_created=task.date_created,
-                       date_started=task.date_started)
+                       date_created=task.date_created.replace(tzinfo=pytz.utc),
+                       date_started=task.date_started.replace(tzinfo=pytz.utc))
```

### Comparing `pyorchestra-0.6.1/orchestra/api/main.py` & `pyorchestra-0.6.2/orchestra/api/main.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.6.1/orchestra/api/routers/jobs.py` & `pyorchestra-0.6.2/orchestra/api/routers/jobs.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.6.1/orchestra/api/routers/tags.py` & `pyorchestra-0.6.2/orchestra/api/routers/tags.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.6.1/orchestra/api/routers/tasks.py` & `pyorchestra-0.6.2/orchestra/api/routers/tasks.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.6.1/orchestra/backend.py` & `pyorchestra-0.6.2/orchestra/backend.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.6.1/orchestra/core.py` & `pyorchestra-0.6.2/orchestra/core.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.6.1/orchestra/formatting.py` & `pyorchestra-0.6.2/orchestra/formatting.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.6.1/orchestra/models.py` & `pyorchestra-0.6.2/orchestra/models.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.6.1/orchestra/scheduling.py` & `pyorchestra-0.6.2/orchestra/scheduling.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.6.1/pyproject.toml` & `pyorchestra-0.6.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyorchestra"
-version = "0.6.1"
+version = "0.6.2"
 description = "Orchestra is a job scheduler on top of Celery"
 authors = ["András Vidosits <andras@hyperplane.hu>"]
 readme = "README.md"
 license = "LGPLv3"
 repository = "https://github.com/vidosits/orchestra"
 packages = [
 	{ include = "orchestra" },
```

### Comparing `pyorchestra-0.6.1/PKG-INFO` & `pyorchestra-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyorchestra
-Version: 0.6.1
+Version: 0.6.2
 Summary: Orchestra is a job scheduler on top of Celery
 Home-page: https://github.com/vidosits/orchestra
 License: LGPLv3
 Author: András Vidosits
 Author-email: andras@hyperplane.hu
 Requires-Python: >=3.11.7,<4.0.0
 Classifier: License :: Other/Proprietary License
```

