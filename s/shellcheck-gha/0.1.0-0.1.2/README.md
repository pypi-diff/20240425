# Comparing `tmp/shellcheck_gha-0.1.0.tar.gz` & `tmp/shellcheck_gha-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellcheck_gha-0.1.0.tar", max compression
+gzip compressed data, was "shellcheck_gha-0.1.2.tar", max compression
```

## Comparing `shellcheck_gha-0.1.0.tar` & `shellcheck_gha-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1502 2024-02-28 17:08:20.809602 shellcheck_gha-0.1.0/LICENSE
--rw-r--r--   0        0        0     2780 2024-02-28 17:08:20.809602 shellcheck_gha-0.1.0/README.md
--rw-r--r--   0        0        0     1173 2024-02-28 17:08:20.809602 shellcheck_gha-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-28 17:08:20.809602 shellcheck_gha-0.1.0/shellcheck_gha/__init__.py
--rw-r--r--   0        0        0        0 2024-02-28 17:08:20.809602 shellcheck_gha-0.1.0/shellcheck_gha/console/__init__.py
--rw-r--r--   0        0        0     1968 2024-02-28 17:08:20.809602 shellcheck_gha-0.1.0/shellcheck_gha/console/app.py
--rw-r--r--   0        0        0      756 2024-02-28 17:08:20.809602 shellcheck_gha-0.1.0/shellcheck_gha/console/colors.py
--rw-r--r--   0        0        0     3593 2024-02-28 17:08:20.809602 shellcheck_gha-0.1.0/shellcheck_gha/console/result_renderer.py
--rw-r--r--   0        0        0     4320 2024-02-28 17:08:20.809602 shellcheck_gha-0.1.0/shellcheck_gha/extractor.py
--rw-r--r--   0        0        0        0 2024-02-28 17:08:20.809602 shellcheck_gha-0.1.0/shellcheck_gha/models/__init__.py
--rw-r--r--   0        0        0      822 2024-02-28 17:08:20.809602 shellcheck_gha-0.1.0/shellcheck_gha/models/github_workflow.py
--rw-r--r--   0        0        0      617 2024-02-28 17:08:20.809602 shellcheck_gha-0.1.0/shellcheck_gha/models/shell_check_json1.py
--rw-r--r--   0        0        0     3920 1970-01-01 00:00:00.000000 shellcheck_gha-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1502 2024-04-25 12:56:43.511009 shellcheck_gha-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4307 2024-04-25 12:56:43.511009 shellcheck_gha-0.1.2/README.md
+-rw-r--r--   0        0        0     1173 2024-04-25 12:56:43.511009 shellcheck_gha-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-25 12:56:43.511009 shellcheck_gha-0.1.2/shellcheck_gha/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:56:43.511009 shellcheck_gha-0.1.2/shellcheck_gha/console/__init__.py
+-rw-r--r--   0        0        0     2512 2024-04-25 12:56:43.511009 shellcheck_gha-0.1.2/shellcheck_gha/console/app.py
+-rw-r--r--   0        0        0      756 2024-04-25 12:56:43.511009 shellcheck_gha-0.1.2/shellcheck_gha/console/colors.py
+-rw-r--r--   0        0        0     3589 2024-04-25 12:56:43.511009 shellcheck_gha-0.1.2/shellcheck_gha/console/result_renderer.py
+-rw-r--r--   0        0        0     4324 2024-04-25 12:56:43.511009 shellcheck_gha-0.1.2/shellcheck_gha/extractor.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:56:43.511009 shellcheck_gha-0.1.2/shellcheck_gha/models/__init__.py
+-rw-r--r--   0        0        0     2603 2024-04-25 12:56:43.511009 shellcheck_gha-0.1.2/shellcheck_gha/models/github_action.py
+-rw-r--r--   0        0        0      617 2024-04-25 12:56:43.511009 shellcheck_gha-0.1.2/shellcheck_gha/models/shell_check_json1.py
+-rw-r--r--   0        0        0     5447 1970-01-01 00:00:00.000000 shellcheck_gha-0.1.2/PKG-INFO
```

### Comparing `shellcheck_gha-0.1.0/LICENSE` & `shellcheck_gha-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shellcheck_gha-0.1.0/pyproject.toml` & `shellcheck_gha-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "shellcheck-gha"
 description = "Extracts and checks shell scripts in Github Workflows for potential issues using shellcheck (https://github.com/koalaman/shellcheck)."
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.2"
 authors = ["Saleor Commerce <hello@saleor.io>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/saleor/shellcheck-gha"
 keywords = [
     "linter",
     "static-analysis",
     "shell",
```

### Comparing `shellcheck_gha-0.1.0/shellcheck_gha/console/app.py` & `shellcheck_gha-0.1.2/shellcheck_gha/console/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from shellcheck_gha.console.result_renderer import ResultRenderer
 from shellcheck_gha.extractor import Extractor, DEFAULT_SHELL
 
 
 def parse_args(args: list[str] | None) -> argparse.Namespace:
     parser = argparse.ArgumentParser()
-    parser.add_argument("directory", nargs="?", default=".github/workflows")
+    parser.add_argument("directory", nargs="?", default=".github/")
     parser.add_argument(
         "--default-shell",
         help="The default shell running in the workflow(s)",
         # 'bash' assumes GitHub workflow is running on Linux or MacOS,
         # and that 'bash' is in the PATH otherwise it will use 'sh'.
         # If it's running on Windows then it's 'cmd'.
         default=DEFAULT_SHELL,
@@ -24,14 +24,26 @@
         help="Show more details about the execution.",
     )
     parser.add_argument(
         "--debug",
         action="store_true",
         help="Add debug information (takes precedence over --verbose).",
     )
+    parser.add_argument(
+        "--skip-unknown-files",
+        action=argparse.BooleanOptionalAction,
+        help=(
+            "Whether to exit with an error on when parsing non-GitHub workflow "
+            "or composite action YAML files. Skipping is useful when a directory "
+            "may be mixed with other YAML files "
+            "(e.g. config files such as .github/dependabot.yaml). "
+            "Unknown files are skipped by default."
+        ),
+        default=True,
+    )
     return parser.parse_args(args)
 
 
 def main(out=sys.stdout, args: list[str] | None = None) -> None:
     ns = parse_args(args)
 
     if ns.debug:
@@ -49,14 +61,15 @@
     if not (directory := Path(ns.directory).absolute()).is_dir():
         sys.stderr.write(f"No such directory {directory}.\n")
         sys.exit(1)
 
     num_files_scanned, num_snippets_scanned, findings = Extractor(
         directory=directory,
         default_shell=ns.default_shell,
+        raise_on_unsupported_yaml=not ns.skip_unknown_files,
     ).run()
 
     print(f"=== Results: {len(findings)} file(s) have findings ===")
     print(f"Scanned {num_files_scanned} files ({num_snippets_scanned} shell scripts)")
 
     for part in ResultRenderer().render(findings):
         out.write(part)
```

### Comparing `shellcheck_gha-0.1.0/shellcheck_gha/console/colors.py` & `shellcheck_gha-0.1.2/shellcheck_gha/console/colors.py`

 * *Files identical despite different names*

### Comparing `shellcheck_gha-0.1.0/shellcheck_gha/console/result_renderer.py` & `shellcheck_gha-0.1.2/shellcheck_gha/console/result_renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from shellcheck_gha.extractor import Finding
 from shellcheck_gha.models.shell_check_json1 import ShellCheckComment
 
 TTY_TEMPLATE = """\
 {% for finding in findings %}\
 {% for comment in finding.shellcheck_data.comments %}\
 {% set color = comment.level | level_ansi_code %}\
-[{{ comment.level | upper | wrap_color(color) }}] In {{finding.shell_snippet.workflow_path}}:
+[{{ comment.level | upper | wrap_color(color) }}] In {{finding.shell_snippet.yaml_path}}:
     Message: {{ comment.message }}
     More information: https://www.shellcheck.net/wiki/SC{{ comment.code }}
     Code:
         {{ finding | extract_code(comment) | indent(8) }}
         {{ ' ' * (comment.column - 1) }}{{ '^' * (comment.endColumn - comment.column + 1) }}
 {% endfor %}\
 {% endfor %}\
```

### Comparing `shellcheck_gha-0.1.0/shellcheck_gha/extractor.py` & `shellcheck_gha-0.1.2/shellcheck_gha/extractor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,57 @@
 import dataclasses
 import logging
 import subprocess
 import sys
 from pathlib import Path
 
 import yaml
+from pydantic import ValidationError
 
-from shellcheck_gha.models.github_workflow import GitHubWorkflow, GitHubStepRun
+from shellcheck_gha.models.github_action import (
+    GitHubYAML,
+    ShellSnippet,
+    UnknownYAMLFileException,
+)
 from shellcheck_gha.models.shell_check_json1 import ShellCheckOutput
 
 logger = logging.getLogger(__name__)
 
 SUPPORTED_SHELLS = ["sh", "bash", "dash", "ksh"]
 DEFAULT_SHELL = "bash"
 
 
 @dataclasses.dataclass
-class ShellSnippet:
-    workflow_path: Path
-
-    job_id: str  # The value from jobs.<job_id>.
-    step_id: str  # The value from jobs.<job_id>.steps[*].id.
-    step_number: int  # The nth position of the step inside the job.
-
-    step_specs: GitHubStepRun
-
-    def __str__(self):
-        return f"{self.workflow_path}:jobs.{self.job_id}.steps[{self.step_number}]"
-
-
-@dataclasses.dataclass
 class Finding:
     shellcheck_data: ShellCheckOutput
     shell_snippet: ShellSnippet
 
 
 @dataclasses.dataclass
 class Extractor:
     directory: Path
+
+    # Whether to raise an exception when the parsed YAML
+    # file is not a GitHub workflow or action.
+    # ``raise_on_invalid_yaml=False`` is useful when a folder
+    # may contain other files (e.g., dependabot config files).
+    raise_on_unsupported_yaml: bool = True
+
     default_shell: str = DEFAULT_SHELL
 
     def iter_workflow_paths(self):
         """Yields all yaml files recursively."""
-        for path in self.directory.rglob("*.y[a]ml"):
-            if path.is_file() and not path.is_symlink():
+        for path in self.directory.rglob("*"):
+            if (
+                path.is_file()
+                and not path.is_symlink()
+                and (path.name.endswith(".yml") or path.name.endswith(".yaml"))
+            ):
                 yield path
 
-    @staticmethod
-    def iter_shell_scripts(workflow_file: Path):
-        """Yields all shell script steps contained within a GitHub workflow YAML file."""
-        with workflow_file.open() as fp:
-            contents = yaml.safe_load(fp)
-
-        obj = GitHubWorkflow.model_validate(contents)
-        for job_id, job_defs in obj.jobs.items():
-            for step_num, step in enumerate(job_defs.steps):
-                if not step.run:
-                    continue
-
-                yield ShellSnippet(
-                    workflow_path=workflow_file,
-                    job_id=job_id,
-                    step_id=step.id,
-                    step_number=step_num,
-                    step_specs=step,
-                )
-
     def check_snippet(self, snippet: ShellSnippet) -> Finding | None:
         """
         Analyzes a shell snippet from a GitHub workflow using shellcheck.
 
         Returns None if there are no findings.
         """
 
@@ -118,19 +100,33 @@
         and the list of findings.
         """
         findings: list[Finding] = []
         num_files_scanned: int = 0
         num_snippets_scanned: int = 0
 
         logger.info("Scanning the directory: %s", self.directory)
-        for workflow in self.iter_workflow_paths():
+        for yaml_path in self.iter_workflow_paths():
+            logger.info("Checking the YAML file: %s", yaml_path)
+
+            with yaml_path.open() as fp:
+                try:
+                    parsed_yaml = GitHubYAML.model_validate(yaml.safe_load(fp))
+                except ValidationError as exc:
+                    # Skip the file if we are not in a strict mode.
+                    if self.raise_on_unsupported_yaml is False:
+                        logger.warning(
+                            "Skipping unsupported YAML file (%s): %s", yaml_path, exc
+                        )
+                        continue
+                    raise UnknownYAMLFileException(exc) from exc
+
+            # Only increment if the file is successfully parsed.
             num_files_scanned += 1
-            logger.info("Checking the workflow: %s", workflow)
 
-            for snippet in self.iter_shell_scripts(workflow):
+            for snippet in parsed_yaml.iter_shell_scripts(yaml_path):
                 num_snippets_scanned += 1
                 finding = self.check_snippet(snippet)
 
                 if finding is not None:
                     findings.append(finding)
 
         return num_files_scanned, num_snippets_scanned, findings
```

### Comparing `shellcheck_gha-0.1.0/shellcheck_gha/models/shell_check_json1.py` & `shellcheck_gha-0.1.2/shellcheck_gha/models/shell_check_json1.py`

 * *Files identical despite different names*

### Comparing `shellcheck_gha-0.1.0/PKG-INFO` & `shellcheck_gha-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,73 @@
-Metadata-Version: 2.1
-Name: shellcheck-gha
-Version: 0.1.0
-Summary: Extracts and checks shell scripts in Github Workflows for potential issues using shellcheck (https://github.com/koalaman/shellcheck).
-Home-page: https://github.com/saleor/shellcheck-gha
-License: BSD-3-Clause
-Keywords: linter,static-analysis,shell,bash,dash,github,workflows,shellcheck
-Author: Saleor Commerce
-Author-email: hello@saleor.io
-Requires-Python: >=3.11
-Classifier: Development Status :: 1 - Planning
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.13
-Classifier: Topic :: Security
-Classifier: Topic :: Software Development :: Quality Assurance
-Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
-Requires-Dist: pydantic (>=2.6.0,<3.0.0)
-Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Project-URL: Repository, https://github.com/saleor/shellcheck-gha
-Description-Content-Type: text/markdown
-
 shellcheck-gha
 ==============
 
 ![PyPI Project Version](https://img.shields.io/pypi/v/shellcheck-gha.svg)
 ![Supported Python Versions](https://img.shields.io/pypi/pyversions/shellcheck-gha.svg)
 ![Project Python Implementations](https://img.shields.io/pypi/implementation/shellcheck-gha.svg)
 
 This Python script extracts shell scripts from GitHub workflows
 (`jobs.<job_id>.steps[*].run`) and runs them against [ShellCheck].
 
+<!-- TOC -->
+* [shellcheck-gha](#shellcheck-gha)
+  * [Installation](#installation)
+    * [Using GitHub Actions (recommended)](#using-github-actions-recommended)
+    * [PyPI](#pypi)
+    * [From Source](#from-source)
+  * [Usage](#usage)
+  * [Example](#example)
+  * [Goals](#goals)
+  * [Non-Goals](#non-goals)
+<!-- TOC -->
+
 ## Installation
 
 **Requirements:**
 
 - Python ≥ 3.11
 - [ShellCheck] ≥ 0.9.0, available on `apt`, `brew`, `cabal`, `dnf`, and `pkg`.
 
-### PyPI (prefered)
+### Using GitHub Actions (recommended)
+
+The `shellcheck-gha` project can be used as a GitHub Workflow step:
+
+```yaml
+on:
+  push:
+    paths:
+      - .github/**
+  pull_request:
+    paths:
+      - .github/**
+
+permissions:
+  contents: read
+
+jobs:
+  check:
+    runs-on: ubuntu-latest
+    steps:
+      - name: Checkout
+        uses: actions/checkout@v4
+
+      - name: Run ShellCheck
+        uses: saleor/shellcheck-gha@v0
+        # Uncomment to customize the scan directory:
+        # with:
+        #   scan-directory-path: .github/
+```
+
+> [!IMPORTANT]  
+> By default only the `./.github` directory is scanned (recursively).
+> If some GitHub Composite actions are defined outside the `.github` directory,
+> consider adding steps to scan the additional directories by changing the `scan-directory-path`
+> parameter.
+
+### PyPI
 
 The project is hosted on PyPI at https://pypi.org/project/shellcheck-gha/.
 To install the project, run:
 
 ```
 $ pip install shellcheck-gha
 ```
@@ -61,25 +83,28 @@
 $ shellcheck-gha --help
 ```
 
 ## Usage
 
 ```
 $ shellcheck-gha --help
-usage: shellcheck-gha [-h] [--default-shell DEFAULT_SHELL] [--verbose] [--debug] directory
+usage: shellcheck-gha [-h] [--default-shell DEFAULT_SHELL] [--verbose] [--debug] [--skip-unknown-files | --no-skip-unknown-files] [directory]
 
 positional arguments:
   directory
 
 options:
   -h, --help            show this help message and exit
   --default-shell DEFAULT_SHELL
                         The default shell running in the workflow(s)
   --verbose             Show more details about the execution.
   --debug               Add debug information (takes precedence over --verbose).
+  --skip-unknown-files, --no-skip-unknown-files
+                        Whether to exit with an error on when parsing non-GitHub workflow or composite action YAML files. Skipping is useful when a directory
+                        may be mixed with other YAML files (e.g. config files such as .github/dependabot.yaml). Unknown files are skipped by default.
 ```
 
 ## Example
 
 ```
 $ shellcheck-gha .
 === Results: 2 file(s) have findings ===
@@ -96,15 +121,15 @@
     Code:
         echo $BAD_JOB1
              ^^^^^^^^^^
 [INFO] In tests/sample_workflows/with-findings.yaml:
     Message: Double quote to prevent globbing and word splitting.
     More information: https://www.shellcheck.net/wiki/SC2086
     Code:
-        echo $BAD_JOB1
+        echo $BAD_JOB2
              ^^^^^^^^^^
 ```
 
 ## Goals
 
 - Only check *nix related shells (sh, bash, ksh)
 - Provide useful logs that allow the users to quickly find the problematic 
@@ -116,8 +141,7 @@
 - Logical understanding of GitHub workflows, such as (but not limited to):
   - Handling `defaults.run.shell`
   - Support for string interpolation (`${{ ... }}`)
 - Tracking down exact locations of the findings (line numbers, columns)
 
 [ShellCheck]: https://github.com/koalaman/shellcheck
 [poetry]: https://pypi.org/project/poetry/
-
```

