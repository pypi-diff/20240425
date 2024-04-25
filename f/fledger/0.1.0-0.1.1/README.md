# Comparing `tmp/fledger-0.1.0.tar.gz` & `tmp/fledger-0.1.1.tar.gz`

## Comparing `fledger-0.1.0.tar` & `fledger-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 fledger-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5432 2020-02-02 00:00:00.000000 fledger-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 fledger-0.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    13487 2020-02-02 00:00:00.000000 fledger-0.1.0/assessments/project/overview_project_matrix.md
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 fledger-0.1.0/assessments/user/evidence.json
--rw-r--r--   0        0        0    13756 2020-02-02 00:00:00.000000 fledger-0.1.0/assessments/user/overview_skills_and_project_matrix.md
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fledger-0.1.0/examples/ML/Example_CatDog_CN_release_Note.txt
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 fledger-0.1.0/examples/ML/Example_CatDog_OD_Release_Note.txt
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fledger-0.1.0/examples/ML/Example_Release_Note.txt
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 fledger-0.1.0/rubric/general/README_file_check.json
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 fledger-0.1.0/src/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fledger-0.1.0/src/__init__.py
--rw-r--r--   0        0        0    13691 2020-02-02 00:00:00.000000 fledger-0.1.0/src/assessments/user/overview_skills_and_project_matrix.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fledger-0.1.0/src/cli/__init__.py
--rw-r--r--   0        0        0     8801 2020-02-02 00:00:00.000000 fledger-0.1.0/src/cli/helpers.py
--rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 fledger-0.1.0/src/cli/main.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fledger-0.1.0/src/cli/requirements.txt
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 fledger-0.1.0/src/cli/templates/job_matrix_overview.md
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 fledger-0.1.0/src/cli/templates/skill_matrix_overview.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fledger-0.1.0/src/tests/__init__.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 fledger-0.1.0/src/tests/test_cli_commands.py
--rw-r--r--   0        0        0    17770 2020-02-02 00:00:00.000000 fledger-0.1.0/src/tests/data/OpenSSF_Standards_Passing.json
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 fledger-0.1.0/src/tests/data/TwilioAITrust.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 fledger-0.1.0/src/tests/data/openssf_example.json
--rw-r--r--   0        0        0    17770 2020-02-02 00:00:00.000000 fledger-0.1.0/standards/OpenSSF.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 fledger-0.1.0/.gitignore
--rw-r--r--   0        0        0    11417 2020-02-02 00:00:00.000000 fledger-0.1.0/LICENSE
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 fledger-0.1.0/README.md
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 fledger-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 fledger-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 fledger-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     5432 2020-02-02 00:00:00.000000 fledger-0.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 fledger-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    13487 2020-02-02 00:00:00.000000 fledger-0.1.1/assessments/project/overview_project_matrix.md
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 fledger-0.1.1/assessments/user/evidence.json
+-rw-r--r--   0        0        0    13756 2020-02-02 00:00:00.000000 fledger-0.1.1/assessments/user/overview_skills_and_project_matrix.md
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fledger-0.1.1/examples/ML/Example_CatDog_CN_release_Note.txt
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 fledger-0.1.1/examples/ML/Example_CatDog_OD_Release_Note.txt
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fledger-0.1.1/examples/ML/Example_Release_Note.txt
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 fledger-0.1.1/rubric/general/README_file_check.json
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 fledger-0.1.1/src/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fledger-0.1.1/src/__init__.py
+-rw-r--r--   0        0        0    13691 2020-02-02 00:00:00.000000 fledger-0.1.1/src/assessments/user/overview_skills_and_project_matrix.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fledger-0.1.1/src/cli/__init__.py
+-rw-r--r--   0        0        0     8801 2020-02-02 00:00:00.000000 fledger-0.1.1/src/cli/helpers.py
+-rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 fledger-0.1.1/src/cli/main.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fledger-0.1.1/src/cli/requirements.txt
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 fledger-0.1.1/src/cli/templates/job_matrix_overview.md
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 fledger-0.1.1/src/cli/templates/skill_matrix_overview.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fledger-0.1.1/src/tests/__init__.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 fledger-0.1.1/src/tests/test_cli_commands.py
+-rw-r--r--   0        0        0    17770 2020-02-02 00:00:00.000000 fledger-0.1.1/src/tests/data/OpenSSF_Standards_Passing.json
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 fledger-0.1.1/src/tests/data/TwilioAITrust.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 fledger-0.1.1/src/tests/data/openssf_example.json
+-rw-r--r--   0        0        0    17770 2020-02-02 00:00:00.000000 fledger-0.1.1/standards/OpenSSF.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 fledger-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11417 2020-02-02 00:00:00.000000 fledger-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 fledger-0.1.1/README.md
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 fledger-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 fledger-0.1.1/PKG-INFO
```

### Comparing `fledger-0.1.0/.pre-commit-config.yaml` & `fledger-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fledger-0.1.0/CODE_OF_CONDUCT.md` & `fledger-0.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `fledger-0.1.0/CONTRIBUTING.md` & `fledger-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fledger-0.1.0/assessments/project/overview_project_matrix.md` & `fledger-0.1.1/assessments/project/overview_project_matrix.md`

 * *Files identical despite different names*

### Comparing `fledger-0.1.0/assessments/user/evidence.json` & `fledger-0.1.1/assessments/user/evidence.json`

 * *Files identical despite different names*

### Comparing `fledger-0.1.0/assessments/user/overview_skills_and_project_matrix.md` & `fledger-0.1.1/assessments/user/overview_skills_and_project_matrix.md`

 * *Files identical despite different names*

### Comparing `fledger-0.1.0/examples/ML/Example_CatDog_CN_release_Note.txt` & `fledger-0.1.1/examples/ML/Example_CatDog_CN_release_Note.txt`

 * *Files identical despite different names*

### Comparing `fledger-0.1.0/examples/ML/Example_CatDog_OD_Release_Note.txt` & `fledger-0.1.1/examples/ML/Example_CatDog_OD_Release_Note.txt`

 * *Files identical despite different names*

### Comparing `fledger-0.1.0/rubric/general/README_file_check.json` & `fledger-0.1.1/rubric/general/README_file_check.json`

 * *Files identical despite different names*

### Comparing `fledger-0.1.0/src/assessments/user/overview_skills_and_project_matrix.md` & `fledger-0.1.1/src/assessments/user/overview_skills_and_project_matrix.md`

 * *Files identical despite different names*

### Comparing `fledger-0.1.0/src/cli/helpers.py` & `fledger-0.1.1/src/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `fledger-0.1.0/src/cli/main.py` & `fledger-0.1.1/src/cli/main.py`

 * *Files identical despite different names*

### Comparing `fledger-0.1.0/src/cli/templates/job_matrix_overview.md` & `fledger-0.1.1/src/cli/templates/job_matrix_overview.md`

 * *Files identical despite different names*

### Comparing `fledger-0.1.0/src/tests/test_cli_commands.py` & `fledger-0.1.1/src/tests/test_cli_commands.py`

 * *Files identical despite different names*

### Comparing `fledger-0.1.0/src/tests/data/OpenSSF_Standards_Passing.json` & `fledger-0.1.1/src/tests/data/OpenSSF_Standards_Passing.json`

 * *Files identical despite different names*

### Comparing `fledger-0.1.0/src/tests/data/TwilioAITrust.json` & `fledger-0.1.1/src/tests/data/TwilioAITrust.json`

 * *Files identical despite different names*

### Comparing `fledger-0.1.0/standards/OpenSSF.json` & `fledger-0.1.1/standards/OpenSSF.json`

 * *Files identical despite different names*

### Comparing `fledger-0.1.0/LICENSE` & `fledger-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fledger-0.1.0/README.md` & `fledger-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fledger-0.1.0/pyproject.toml` & `fledger-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 # https://hatch.pypa.io/1.9/config/metadata/#license Cheat sheet
 [project]
 name = "fledger"
 #dynamic = ["version"]
-version = '0.1.0'
+version = '0.1.1'
 description = "Fledger is a Python Framework that simplifies software engineering and development under standards. "
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "Jason Burt", email = "jason2burt+fledger@gmail.com" },
```

### Comparing `fledger-0.1.0/PKG-INFO` & `fledger-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fledger
-Version: 0.1.0
+Version: 0.1.1
 Summary: Fledger is a Python Framework that simplifies software engineering and development under standards. 
 Project-URL: Documentation, https://github.com/jasonburt/fledger/blob/main/README.md
 Project-URL: Issues, https://github.com/jasonburt/fledger/issues
 Project-URL: Source, https://github.com/jasonburt/fledger
 Author-email: Jason Burt <jason2burt+fledger@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

