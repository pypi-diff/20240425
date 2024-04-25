# Comparing `tmp/rh_aws_saml_login-0.3.1.tar.gz` & `tmp/rh_aws_saml_login-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rh_aws_saml_login-0.3.1.tar", max compression
+gzip compressed data, was "rh_aws_saml_login-0.3.2.tar", max compression
```

## Comparing `rh_aws_saml_login-0.3.1.tar` & `rh_aws_saml_login-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3292 2024-04-18 07:57:45.743430 rh_aws_saml_login-0.3.1/README.md
--rw-r--r--   0        0        0     2131 2024-04-18 07:57:45.751430 rh_aws_saml_login-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-18 07:57:45.751430 rh_aws_saml_login-0.3.1/rh_aws_saml_login/__init__.py
--rw-r--r--   0        0        0     2795 2024-04-18 07:57:45.752430 rh_aws_saml_login-0.3.1/rh_aws_saml_login/__main__.py
--rw-r--r--   0        0        0     8107 2024-04-18 07:57:45.752430 rh_aws_saml_login-0.3.1/rh_aws_saml_login/core.py
--rw-r--r--   0        0        0     1464 2024-04-18 07:57:45.752430 rh_aws_saml_login-0.3.1/rh_aws_saml_login/utils.py
--rw-r--r--   0        0        0     4453 1970-01-01 00:00:00.000000 rh_aws_saml_login-0.3.1/setup.py
--rw-r--r--   0        0        0     4283 1970-01-01 00:00:00.000000 rh_aws_saml_login-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     3292 2024-04-25 11:27:21.656947 rh_aws_saml_login-0.3.2/README.md
+-rw-r--r--   0        0        0     2131 2024-04-25 11:27:21.665947 rh_aws_saml_login-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-25 11:27:21.665947 rh_aws_saml_login-0.3.2/rh_aws_saml_login/__init__.py
+-rw-r--r--   0        0        0     3036 2024-04-25 11:27:21.665947 rh_aws_saml_login-0.3.2/rh_aws_saml_login/__main__.py
+-rw-r--r--   0        0        0     8179 2024-04-25 11:27:21.665947 rh_aws_saml_login-0.3.2/rh_aws_saml_login/core.py
+-rw-r--r--   0        0        0     1464 2024-04-25 11:27:21.665947 rh_aws_saml_login-0.3.2/rh_aws_saml_login/utils.py
+-rw-r--r--   0        0        0     4453 1970-01-01 00:00:00.000000 rh_aws_saml_login-0.3.2/setup.py
+-rw-r--r--   0        0        0     4283 1970-01-01 00:00:00.000000 rh_aws_saml_login-0.3.2/PKG-INFO
```

### Comparing `rh_aws_saml_login-0.3.1/README.md` & `rh_aws_saml_login-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `rh_aws_saml_login-0.3.1/pyproject.toml` & `rh_aws_saml_login-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rh-aws-saml-login"
-version = "0.3.1"
+version = "0.3.2"
 description = "A CLI tool that allows you to log in and retrieve AWS temporary credentials using Red Hat SAML IDP"
 authors = ["Christian Assing <cassing@redhat.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "rh_aws_saml_login" }]
 homepage = "https://github.com/app-sre/rh-aws-saml-login"
 repository = "https://github.com/app-sre/rh-aws-saml-login"
```

### Comparing `rh_aws_saml_login-0.3.1/rh_aws_saml_login/__main__.py` & `rh_aws_saml_login-0.3.2/rh_aws_saml_login/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,24 +55,33 @@
         False, help="Open the AWS console in browser instead of a local shell"
     ),
     display_banner: bool = typer.Option(True, help="Display a shiny banner"),
     saml_url: str = typer.Option(
         "https://auth.redhat.com/auth/realms/EmployeeIDP/protocol/saml/clients/itaws",
         help="SAML URL",
     ),
+    open_command: str = typer.Option(
+        "open",
+        help="Command to open the browser (e.g. 'xdg-open' on Linux)",
+        envvar="RH_AWS_SAML_LOGIN_OPEN_COMMAND",
+    ),
 ) -> None:
     """Login to AWS using SAML."""
     logging.basicConfig(
         level=logging.INFO if not debug else logging.DEBUG, format="%(message)s"
     )
     if display_banner:
         print(blend_text(BANNER, (32, 32, 255), (255, 32, 255)))
     if debug:
         enable_requests_logging()
     accounts = core.main(
-        account_name=account_name, region=region, console=console, saml_url=saml_url
+        account_name=account_name,
+        region=region,
+        console=console,
+        saml_url=saml_url,
+        open_command=open_command,
     )
     write_accounts_cache(accounts)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `rh_aws_saml_login-0.3.1/rh_aws_saml_login/core.py` & `rh_aws_saml_login-0.3.2/rh_aws_saml_login/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import logging
 import os
 import re
+import shlex
 import subprocess
 import sys
 import urllib
 from dataclasses import dataclass
 from datetime import datetime as dt
 from textwrap import dedent
 
@@ -169,15 +170,15 @@
             "AWS_SECRET_ACCESS_KEY": credentials.secret_key,
             "AWS_SESSION_TOKEN": credentials.session_token,
             "AWS_REGION": region,
         },
     )
 
 
-def open_aws_console(account: AwsAccount, credentials: AwsCredentials) -> None:
+def open_aws_console(open_command: str, credentials: AwsCredentials) -> None:
     """Open the AWS console in a browser.
 
     See https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_providers_enable-console-custom-url.html
     """
     aws_federated_signin_endpoint = "https://signin.aws.amazon.com/federation"
     # Get a sign-in token from the AWS sign-in federation endpoint.
     response = requests.get(
@@ -199,19 +200,23 @@
     query_string = urllib.parse.urlencode({
         "Action": "login",
         "Issuer": "redhat.com",
         "Destination": "https://console.aws.amazon.com/",
         "SigninToken": signin_token["SigninToken"],
     })
     federated_url = f"{aws_federated_signin_endpoint}?{query_string}"
-    run(["open", federated_url], check=False, capture_output=False)
+    run(shlex.split(open_command) + [federated_url], check=False, capture_output=False)
 
 
 def main(  # noqa: PLR0913, PLR0917
-    account_name: str | None, region: str, console: bool, saml_url: str
+    account_name: str | None,
+    region: str,
+    console: bool,
+    saml_url: str,
+    open_command: str,
 ) -> list[str]:
     with Progress(
         SpinnerColumn(finished_text="✅"),
         TextColumn("[progress.description]{task.description}"),
     ) as progress:
         task = progress.add_task(
             description="Test for a valid Kerberos ticket ...", total=1
@@ -245,12 +250,12 @@
         task = progress.add_task(
             description="Getting temporary AWS credentials ...", total=1
         )
         credentials = assume_role_with_saml(account, saml_token)
         progress.update(task, completed=1)
 
     if console:
-        open_aws_console(account, credentials)
+        open_aws_console(open_command, credentials)
     else:
         open_aws_shell(account, credentials, region)
     bye()
     return [acc.name for acc in aws_accounts]
```

### Comparing `rh_aws_saml_login-0.3.1/rh_aws_saml_login/utils.py` & `rh_aws_saml_login-0.3.2/rh_aws_saml_login/utils.py`

 * *Files identical despite different names*

### Comparing `rh_aws_saml_login-0.3.1/setup.py` & `rh_aws_saml_login-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'tzlocal>=5.2,<6.0']
 
 entry_points = \
 {'console_scripts': ['rh-aws-saml-login = rh_aws_saml_login.__main__:app']}
 
 setup_kwargs = {
     'name': 'rh-aws-saml-login',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'A CLI tool that allows you to log in and retrieve AWS temporary credentials using Red Hat SAML IDP',
     'long_description': '# rh-aws-saml-login\n\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)\n[![PyPI](https://img.shields.io/pypi/v/rh-aws-saml-login)][pypi-link]\n[![PyPI platforms][pypi-platforms]][pypi-link]\n![PyPI - License](https://img.shields.io/pypi/l/rh-aws-saml-login)\n\nA CLI tool that allows you to log in and retrieve AWS temporary credentials using Red Hat SAML IDP.\n\n![demo](/demo/quickstart.gif)\n\n## Pre-requisites\n\n- Python 3.11 or later\n- Connected to Red Hat VPN\n- A Red Hat managed computer (Kerberos must be installed and configured) and you are logged in with your Red Hat account\n\n## How it works\n\nThe `rh-aws-saml-login` CLI is a tool that simplifies the process of logging into an AWS account via Red Hat SSO. It retrieves a SAML token from the Red Hat SSO server, then fetches and parses the AWS SSO login page to present you with a list of all available accounts and their respective roles. You can then choose your desired account and role, and `rh-aws-saml-login` uses the SAML token to generate temporary AWS role credentials. Finally, it spawns a new shell with the necessary `AWS_` environment variables already set up, so you can immediately use the `aws` CLI without any further configuration.\n\n## Installation\n\nOn CSB Fedora, you need to install the Kerberos development package:\n\n```shell\nsudo dnf install krb5-devel\n```\n\nYou can install this library from [PyPI][pypi-link] with `pip`:\n\n```shell\npython3 -m pip install rh-aws-saml-login\n```\n\nor install it with `pipx`:\n\n```shell\npipx install rh-aws-saml-login\n```\n\nYou can also use `pipx` to run the library without installing it:\n\n```shell\npipx run rh-aws-saml-login\n```\n\n## Usage\n\n```shell\nrh-aws-saml-login\n```\n\nThis spawns a new shell with the following environment variables are set:\n\n- `AWS_ACCOUNT_NAME`: The name/alias of the AWS account\n- `AWS_ROLE_NAME`:  The name of the role\n- `AWS_ROLE_ARN`: The ARN of the role\n- `AWS_ACCESS_KEY_ID`: The access key used by the AWS CLI\n- `AWS_SECRET_ACCESS_KEY`: The secret access key used by the AWS CLI\n- `AWS_SESSION_TOKEN`: The session token used by the AWS CLI\n- `AWS_REGION`: The default region used by the AWS CLI\n\n## Features\n\nrh-aws-saml-login currently provides the following features (get help with `-h` or `--help`):\n\n- No configuration needed\n- Uses Kerberos authentication\n- Open the AWS web console for an account with the `--console` option\n- Shell auto-completion (bash, zsh, and fish) including AWS account names\n- Integrates nicely with the [starship](https://starship.rs)\n\n  ```toml\n   [env_var.AWS_ACCOUNT_NAME]\n   format = "$symbol$style [$env_value]($style) "\n   style = "cyan"\n   symbol = "🚀"\n  ```\n\n## Development\n\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)\n[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)\n\n- Update CHANGELOG.md with the new version number and date\n- Bump the version number in [pyproject.toml](/pyproject.toml)\n\n[pypi-link]:                https://pypi.org/project/rh-aws-saml-login/\n[pypi-platforms]:           https://img.shields.io/pypi/pyversions/rh-aws-saml-login\n',
     'author': 'Christian Assing',
     'author_email': 'cassing@redhat.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/app-sre/rh-aws-saml-login',
```

### Comparing `rh_aws_saml_login-0.3.1/PKG-INFO` & `rh_aws_saml_login-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rh-aws-saml-login
-Version: 0.3.1
+Version: 0.3.2
 Summary: A CLI tool that allows you to log in and retrieve AWS temporary credentials using Red Hat SAML IDP
 Home-page: https://github.com/app-sre/rh-aws-saml-login
 License: MIT
 Author: Christian Assing
 Author-email: cassing@redhat.com
 Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
```

