# Comparing `tmp/vjer-34.2.0.tar.gz` & `tmp/vjer-35.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vjer-34.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vjer-35.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vjer-34.2.0.tar` & `vjer-35.0.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1783 2024-04-22 17:35:51.241248 vjer-34.2.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     2134 2024-04-22 17:35:51.241248 vjer-34.2.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     5245 2024-04-22 17:35:51.241248 vjer-34.2.0/.gitignore
--rw-r--r--   0        0        0     4999 2024-04-22 17:35:51.241248 vjer-34.2.0/.p4ignore
--rw-r--r--   0        0        0       42 2024-04-22 17:35:51.241248 vjer-34.2.0/.readthedocs.yml
--rw-r--r--   0        0        0    40850 2024-04-22 17:35:51.241248 vjer-34.2.0/CHANGELOG.md
--rw-r--r--   0        0        0       64 2024-04-22 17:35:51.241248 vjer-34.2.0/DOCUMENTATION.md
--rw-r--r--   0        0        0     1072 2024-04-22 17:35:51.241248 vjer-34.2.0/LICENSE
--rw-r--r--   0        0        0       90 2024-04-22 17:35:51.245248 vjer-34.2.0/MANIFEST.in
--rw-r--r--   0        0        0      973 2024-04-22 17:35:51.245248 vjer-34.2.0/README.md
--rwxr-xr-x   0        0        0     1046 2024-04-22 17:35:51.245248 vjer-34.2.0/cicd-support/cicd.sh
--rw-r--r--   0        0        0      634 2024-04-22 17:35:51.245248 vjer-34.2.0/docs/Makefile
--rw-r--r--   0        0        0     9167 2024-04-22 17:35:51.245248 vjer-34.2.0/docs/coding_standards.py
--rw-r--r--   0        0        0     2103 2024-04-22 17:35:51.245248 vjer-34.2.0/docs/conf.py
--rw-r--r--   0        0        0      795 2024-04-22 17:35:51.245248 vjer-34.2.0/docs/make.bat
--rw-r--r--   0        0        0       59 2024-04-22 17:35:51.245248 vjer-34.2.0/docs/modules.rst
--rw-r--r--   0        0        0      229 2024-04-22 17:35:51.245248 vjer-34.2.0/docs/requirements.txt
--rw-r--r--   0        0        0     2184 2024-04-22 17:36:19.717290 vjer-34.2.0/pyproject.toml
--rw-r--r--   0        0        0       90 2024-04-22 17:35:51.245248 vjer-34.2.0/tests/vjer.yml
--rw-r--r--   0        0        0      305 2024-04-22 17:35:51.245248 vjer-34.2.0/util/New-Env.ps1
--rw-r--r--   0        0        0      259 2024-04-22 17:35:51.245248 vjer-34.2.0/util/Update-Env.ps1
--rwxr-xr-x   0        0        0      261 2024-04-22 17:35:51.245248 vjer-34.2.0/util/new-env.sh
--rwxr-xr-x   0        0        0      234 2024-04-22 17:35:51.245248 vjer-34.2.0/util/update-env.sh
--rw-r--r--   0        0        0      476 2024-04-22 17:35:51.245248 vjer-34.2.0/vjer.yml
--rw-r--r--   0        0        0      654 2024-04-22 17:36:19.717290 vjer-34.2.0/vjer/__init__.py
--rw-r--r--   0        0        0      205 2024-04-22 17:35:51.245248 vjer-34.2.0/vjer/__main__.py
--rw-r--r--   0        0        0     5278 2024-04-22 17:35:51.245248 vjer-34.2.0/vjer/build.py
--rw-r--r--   0        0        0     1185 2024-04-22 17:35:51.245248 vjer-34.2.0/vjer/deploy.py
--rw-r--r--   0        0        0     2875 2024-04-22 17:35:51.245248 vjer-34.2.0/vjer/freeze.py
--rw-r--r--   0        0        0     1663 2024-04-22 17:35:51.245248 vjer-34.2.0/vjer/pre_release.py
--rw-r--r--   0        0        0        0 2024-04-22 17:35:51.245248 vjer-34.2.0/vjer/py.typed
--rw-r--r--   0        0        0     3170 2024-04-22 17:35:51.245248 vjer-34.2.0/vjer/release.py
--rw-r--r--   0        0        0      769 2024-04-22 17:35:51.245248 vjer-34.2.0/vjer/rollback.py
--rw-r--r--   0        0        0     3457 2024-04-22 17:35:51.245248 vjer-34.2.0/vjer/test.py
--rw-r--r--   0        0        0     3060 2024-04-22 17:35:51.245248 vjer-34.2.0/vjer/tool_reporter.py
--rw-r--r--   0        0        0    26660 2024-04-22 17:35:51.245248 vjer-34.2.0/vjer/utils.py
--rwxr-xr-x   0        0        0     2825 2024-04-22 17:35:51.245248 vjer-34.2.0/vjer/vjer.py
--rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 vjer-34.2.0/setup.py
--rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 vjer-34.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1783 2024-04-25 17:46:54.197277 vjer-35.0.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2134 2024-04-25 17:46:54.197277 vjer-35.0.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     5245 2024-04-25 17:46:54.197277 vjer-35.0.0/.gitignore
+-rw-r--r--   0        0        0     4999 2024-04-25 17:46:54.197277 vjer-35.0.0/.p4ignore
+-rw-r--r--   0        0        0       42 2024-04-25 17:46:54.197277 vjer-35.0.0/.readthedocs.yml
+-rw-r--r--   0        0        0    40951 2024-04-25 17:46:54.197277 vjer-35.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0       64 2024-04-25 17:46:54.197277 vjer-35.0.0/DOCUMENTATION.md
+-rw-r--r--   0        0        0     1072 2024-04-25 17:46:54.197277 vjer-35.0.0/LICENSE
+-rw-r--r--   0        0        0       90 2024-04-25 17:46:54.197277 vjer-35.0.0/MANIFEST.in
+-rw-r--r--   0        0        0      973 2024-04-25 17:46:54.197277 vjer-35.0.0/README.md
+-rwxr-xr-x   0        0        0     1046 2024-04-25 17:46:54.197277 vjer-35.0.0/cicd-support/cicd.sh
+-rw-r--r--   0        0        0      634 2024-04-25 17:46:54.197277 vjer-35.0.0/docs/Makefile
+-rw-r--r--   0        0        0     9167 2024-04-25 17:46:54.197277 vjer-35.0.0/docs/coding_standards.py
+-rw-r--r--   0        0        0     2103 2024-04-25 17:46:54.197277 vjer-35.0.0/docs/conf.py
+-rw-r--r--   0        0        0      795 2024-04-25 17:46:54.197277 vjer-35.0.0/docs/make.bat
+-rw-r--r--   0        0        0       59 2024-04-25 17:46:54.197277 vjer-35.0.0/docs/modules.rst
+-rw-r--r--   0        0        0      229 2024-04-25 17:46:54.197277 vjer-35.0.0/docs/requirements.txt
+-rw-r--r--   0        0        0     2184 2024-04-25 17:47:26.781378 vjer-35.0.0/pyproject.toml
+-rw-r--r--   0        0        0       90 2024-04-25 17:46:54.197277 vjer-35.0.0/tests/vjer.yml
+-rw-r--r--   0        0        0      305 2024-04-25 17:46:54.197277 vjer-35.0.0/util/New-Env.ps1
+-rw-r--r--   0        0        0      259 2024-04-25 17:46:54.197277 vjer-35.0.0/util/Update-Env.ps1
+-rwxr-xr-x   0        0        0      261 2024-04-25 17:46:54.197277 vjer-35.0.0/util/new-env.sh
+-rwxr-xr-x   0        0        0      234 2024-04-25 17:46:54.197277 vjer-35.0.0/util/update-env.sh
+-rw-r--r--   0        0        0      476 2024-04-25 17:46:54.201277 vjer-35.0.0/vjer.yml
+-rw-r--r--   0        0        0      654 2024-04-25 17:47:26.781378 vjer-35.0.0/vjer/__init__.py
+-rw-r--r--   0        0        0      205 2024-04-25 17:46:54.201277 vjer-35.0.0/vjer/__main__.py
+-rw-r--r--   0        0        0     5278 2024-04-25 17:46:54.201277 vjer-35.0.0/vjer/build.py
+-rw-r--r--   0        0        0     1185 2024-04-25 17:46:54.201277 vjer-35.0.0/vjer/deploy.py
+-rw-r--r--   0        0        0     2875 2024-04-25 17:46:54.201277 vjer-35.0.0/vjer/freeze.py
+-rw-r--r--   0        0        0     1649 2024-04-25 17:46:54.201277 vjer-35.0.0/vjer/pre_release.py
+-rw-r--r--   0        0        0        0 2024-04-25 17:46:54.201277 vjer-35.0.0/vjer/py.typed
+-rw-r--r--   0        0        0     3170 2024-04-25 17:46:54.201277 vjer-35.0.0/vjer/release.py
+-rw-r--r--   0        0        0      769 2024-04-25 17:46:54.201277 vjer-35.0.0/vjer/rollback.py
+-rw-r--r--   0        0        0     3457 2024-04-25 17:46:54.201277 vjer-35.0.0/vjer/test.py
+-rw-r--r--   0        0        0     3060 2024-04-25 17:46:54.201277 vjer-35.0.0/vjer/tool_reporter.py
+-rw-r--r--   0        0        0    26635 2024-04-25 17:46:54.201277 vjer-35.0.0/vjer/utils.py
+-rwxr-xr-x   0        0        0     2825 2024-04-25 17:46:54.201277 vjer-35.0.0/vjer/vjer.py
+-rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 vjer-35.0.0/setup.py
+-rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 vjer-35.0.0/PKG-INFO
```

### Comparing `vjer-34.2.0/.github/workflows/build.yml` & `vjer-35.0.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `vjer-34.2.0/.github/workflows/publish.yml` & `vjer-35.0.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `vjer-34.2.0/.gitignore` & `vjer-35.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `vjer-34.2.0/.p4ignore` & `vjer-35.0.0/.p4ignore`

 * *Files identical despite different names*

### Comparing `vjer-34.2.0/CHANGELOG.md` & `vjer-35.0.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,21 +3,26 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
 ## Current Release
 
-### [34.2.0] - 2024-04-22
+### [35.0.0] - 2024-04-25
 
 - Changed
-  - Sanitize Docker tags and Helm versions. (GitHub #14)
+  - Remove bad characters for Helm versions. (GitHub #15)
 
 ## Release History
 
+### [34.2.0] - 2024-04-22
+
+- Changed
+  - Sanitize Docker tags and Helm versions. (GitHub #14)
+
 ### [34.1.1] - 2024-04-19
 
 - Added
   - Report the Google SDK version. (GitHub #13)
 
 ### [34.1.0] - 2024-04-19
```

### Comparing `vjer-34.2.0/LICENSE` & `vjer-35.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vjer-34.2.0/README.md` & `vjer-35.0.0/README.md`

 * *Files identical despite different names*

### Comparing `vjer-34.2.0/cicd-support/cicd.sh` & `vjer-35.0.0/cicd-support/cicd.sh`

 * *Files identical despite different names*

### Comparing `vjer-34.2.0/docs/Makefile` & `vjer-35.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vjer-34.2.0/docs/coding_standards.py` & `vjer-35.0.0/docs/coding_standards.py`

 * *Files identical despite different names*

### Comparing `vjer-34.2.0/docs/conf.py` & `vjer-35.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vjer-34.2.0/docs/make.bat` & `vjer-35.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vjer-34.2.0/pyproject.toml` & `vjer-35.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "xmlrunner.*"
 ignore_missing_imports = true
 
 [tool.bumpver]
-current_version = "v34.2.0"
+current_version = "v35.0.0"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version} [skip ci]"
 commit = true
 tag = false
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `vjer-34.2.0/vjer/__init__.py` & `vjer-35.0.0/vjer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
            '__author__', '__email__',
            '__license__', '__copyright__')
 
 __title__ = 'Vjer'
 __summary__ = 'CI/CD Toolkit'
 __uri__ = 'https://github.com/tardis4500/vjer/'
 
-__version__ = '34.2.0'
+__version__ = '35.0.0'
 __build_name__ = '{var:build_name}'
 __build_date__ = '{var:build_date}'
 
 __author__ = 'Jeffery G. Smith'
 __email__ = 'web@pobox.com'
 
 __license__ = 'MIT'
```

### Comparing `vjer-34.2.0/vjer/build.py` & `vjer-35.0.0/vjer/build.py`

 * *Files identical despite different names*

### Comparing `vjer-34.2.0/vjer/deploy.py` & `vjer-35.0.0/vjer/deploy.py`

 * *Files identical despite different names*

### Comparing `vjer-34.2.0/vjer/freeze.py` & `vjer-35.0.0/vjer/freeze.py`

 * *Files identical despite different names*

### Comparing `vjer-34.2.0/vjer/pre_release.py` & `vjer-35.0.0/vjer/pre_release.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """This module provides pre_release actions."""
 
 # Import standard modules
 from typing import cast
 
 # Import project modules
 from .release import ReleaseStep
-from .utils import sanitize_docker_tag, VjerAction, VjerStep
+from .utils import sanitize_tag, VjerAction, VjerStep
 
 
 class PreReleaseStep(ReleaseStep):
     """Provide pre_release support.
 
     Attributes:
         is_pre_release: Specifies to the ReleaseStep parent class that this is a pre_release action.
@@ -27,15 +27,15 @@
             self.step_info.args = {'tag-num': True}
         super().release_bumpver()
 
     def release_helm(self) -> None:
         """Pre_release a Helm chart."""
         self._release_helm()
         for version in self.step_info.extra_versions:
-            self.project.version = sanitize_docker_tag(version).lower()
+            self.project.version = sanitize_tag(version).lower()
             self._release_helm()
 
     def _release_helm(self) -> None:
         if self.helm_repo.type == 'oci':
             self.update_version_files()
             try:
                 self.helm_build()
```

### Comparing `vjer-34.2.0/vjer/release.py` & `vjer-35.0.0/vjer/release.py`

 * *Files identical despite different names*

### Comparing `vjer-34.2.0/vjer/rollback.py` & `vjer-35.0.0/vjer/rollback.py`

 * *Files identical despite different names*

### Comparing `vjer-34.2.0/vjer/test.py` & `vjer-35.0.0/vjer/test.py`

 * *Files identical despite different names*

### Comparing `vjer-34.2.0/vjer/tool_reporter.py` & `vjer-35.0.0/vjer/tool_reporter.py`

 * *Files identical despite different names*

### Comparing `vjer-34.2.0/vjer/utils.py` & `vjer-35.0.0/vjer/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -459,15 +459,15 @@
         Returns:
             Nothing.
         """
         if (registry := self.project.container_registry).type not in ('gcp', 'gcp-art'):
             (image := self.registry_client.get_image(source_tag)).pull()
         for tag in tags:
             (repo, candidate_tag) = tag.split(':', 1) if (':' in tag) else ('', tag)
-            sanitized_tag = sanitize_docker_tag(candidate_tag)
+            sanitized_tag = sanitize_tag(candidate_tag)
             final_tag = f'{repo}:{sanitized_tag}' if (':' in tag) else sanitized_tag
             self.log_message(f'Tagging image: {final_tag}')
             match registry.type:
                 case 'gcp':
                     gcloud('container', 'images', 'add-tag', source_tag, final_tag, syscmd_args={'ignore_stderr': True})
                 case 'gcp-art':
                     gcloud('artifacts', 'docker', 'tags', 'add', source_tag, final_tag, syscmd_args={'ignore_stderr': True})
@@ -578,27 +578,27 @@
             step.is_first_step = is_first_step
             VjerStep().log_message(f'Executing {self.action_type} step: {step.type if (not step.name) else step.name}', True)
             (executor := cast(Callable, self.action_step_class)()).step_info = step
             executor.execute()
             is_first_step = False
 
 
-def sanitize_docker_tag(tag: str, replacement_char: str = '-') -> str:
+def sanitize_tag(tag: str, replacement_char: str = '-') -> str:
     """Sanitize a Docker tag by replacing invalid characters with a specified valid character.
 
         Args:
             tag: The Docker tag to sanitize.
             replacement_char (optional, default=_): The character to replace invalid characters with.
 
         Returns:
             The sanitized Docker tag.
     """
-    valid_pattern = re_compile(r'^[a-zA-Z0-9][a-zA-Z0-9._-]{0,127}$')
-    sanitized_tag = re_sub(r'[^a-zA-Z0-9._-]', replacement_char, tag)
-    if sanitized_tag[0] in ['.', '-']:
+    valid_pattern = re_compile(r'^[a-zA-Z0-9][a-zA-Z0-9-]{0,127}$')
+    sanitized_tag = re_sub(r'[^a-zA-Z0-9-]', replacement_char, tag)
+    if sanitized_tag[0] == '-':
         sanitized_tag = replacement_char + sanitized_tag[1:]
     sanitized_tag = sanitized_tag[:128]
     if not valid_pattern.match(sanitized_tag):
         raise ValueError(f"The sanitized tag '{sanitized_tag}' is still not valid according to Docker's specifications.")
     return sanitized_tag
 
 # cSpell:ignore batcave bumpver cloudmgr dotmap platarch syscmd vjer checkin
```

### Comparing `vjer-34.2.0/vjer/vjer.py` & `vjer-35.0.0/vjer/vjer.py`

 * *Files identical despite different names*

### Comparing `vjer-34.2.0/setup.py` & `vjer-35.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 extras_require = \
 {'dev': ['twine'], 'test': ['types-PyYAML', 'types-requests']}
 
 entry_points = \
 {'console_scripts': ['vjer = vjer.vjer:main']}
 
 setup(name='vjer',
-      version='34.2.0',
+      version='35.0.0',
       description='Vjer CI/CD module.',
       author=None,
       author_email='"Jeffery G. Smith" <web@pobox.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `vjer-34.2.0/PKG-INFO` & `vjer-35.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vjer
-Version: 34.2.0
+Version: 35.0.0
 Summary: Vjer CI/CD module.
 Keywords: python,programming,utilities
 Author-email: "Jeffery G. Smith" <web@pobox.com>
 Requires-Python: ~=3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

