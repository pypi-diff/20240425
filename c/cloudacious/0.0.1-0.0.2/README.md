# Comparing `tmp/cloudacious-0.0.1.tar.gz` & `tmp/cloudacious-0.0.2.tar.gz`

## Comparing `cloudacious-0.0.1.tar` & `cloudacious-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudacious-0.0.1/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudacious-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 cloudacious-0.0.1/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudacious-0.0.1/config.cfg
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 cloudacious-0.0.1/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudacious-0.0.1/src/cloudacious/README.md
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 cloudacious-0.0.1/src/cloudacious/iac/ContainerImages.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudacious-0.0.1/src/cloudacious/iac/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudacious-0.0.1/.gitignore
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 cloudacious-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cloudacious-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 cloudacious-0.0.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudacious-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cloudacious-0.0.2/.pypirc
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 cloudacious-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudacious-0.0.2/config.cfg
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 cloudacious-0.0.2/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudacious-0.0.2/src/cloudacious/README.md
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 cloudacious-0.0.2/src/cloudacious/iac/ContainerImages.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudacious-0.0.2/src/cloudacious/iac/README.md
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 cloudacious-0.0.2/.gitignore
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 cloudacious-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cloudacious-0.0.2/PKG-INFO
```

### Comparing `cloudacious-0.0.1/README.md` & `cloudacious-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cloudacious-0.0.1/setup.py` & `cloudacious-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="cloudacious",
-    version="0.0.1",
+    version="0.0.2",
     description="Cloudacious's object-oriented code tooling. Call our classes all day long!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/money-marathon/cloudacious/cloudacious.git",
     author="A. SurfingDoggo",
     author_email="git@surfingdoggo.com",  # Optional
     classifiers=[
@@ -28,9 +28,12 @@
     packages=find_packages(),
     python_requires=">=3.11, <4",
     install_requires=[
         "requests",
         "python-gitlab",
         "boto3",
         "python-dotenv",
+        "pulumi",
+        "pulumi_aws",
+        "pulumi_docker",
     ],
 )
```

### Comparing `cloudacious-0.0.1/src/cloudacious/iac/ContainerImages.py` & `cloudacious-0.0.2/src/cloudacious/iac/ContainerImages.py`

 * *Files identical despite different names*

