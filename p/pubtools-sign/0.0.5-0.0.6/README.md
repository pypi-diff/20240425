# Comparing `tmp/pubtools_sign-0.0.5.tar.gz` & `tmp/pubtools_sign-0.0.6.tar.gz`

## Comparing `pubtools_sign-0.0.5.tar` & `pubtools_sign-0.0.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/.coveragerc
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/AppImageBuilder.yml
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/MANIFEST.in
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/mypy.ini
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/requirements-test.txt
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/requirements.txt
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/tox.ini
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/.github/renovate.json
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/.github/workflows/docs.yml
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/.github/workflows/owasp.yml
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/.github/workflows/release.yml
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/.github/workflows/tox-tests.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/docs/make.bat
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/docs/source/CHANGELOG.rst
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/docs/source/conf.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/docs/source/index.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/__init__.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/bundle.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/exceptions.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/ansible/__init__.py
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/ansible/msg_clear_sign.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/clients/__init__.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/clients/msg.py
--rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/clients/msg_recv_client.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/clients/msg_send_client.py
--rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/clients/registry.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/conf/conf.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/models/msg.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/operations/__init__.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/operations/base.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/operations/clearsign.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/operations/containersign.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/results/__init__.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/results/clearsign.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/results/containersign.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/results/operation_result.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/results/signing_results.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/signers/__init__.py
--rw-r--r--   0        0        0    14474 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/signers/cosignsigner.py
--rw-r--r--   0        0        0    22321 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/src/pubtools/sign/signers/msgsigner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0    16386 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/tests/conftest.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/tests/conftest_cosignsig.py
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/tests/conftest_msgsig.py
--rw-r--r--   0        0        0     5293 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/tests/test_ansible_clearsign.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/tests/test_bundle.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/tests/test_config.py
--rw-r--r--   0        0        0    25481 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/tests/test_cosign_signer.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/tests/test_msg_handle.py
--rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/tests/test_msg_recv_client.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/tests/test_msg_send_client.py
--rw-r--r--   0        0        0    33832 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/tests/test_msg_signer.py
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/tests/test_registry_client.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/tests/test_results.py
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/tests/test_sign_operations.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/tests/test_utils.py
--rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/utils/pre-commit
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/.gitignore
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/LICENSE
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/README.rst
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 pubtools_sign-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/.coveragerc
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/AppImageBuilder.yml
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/MANIFEST.in
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/mypy.ini
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/requirements-test.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/requirements.txt
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tox.ini
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/.github/renovate.json
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/.github/workflows/owasp.yml
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/.github/workflows/tox-tests.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/docs/make.bat
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/docs/source/CHANGELOG.rst
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/docs/source/conf.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/__init__.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/bundle.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/exceptions.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/ansible/__init__.py
+-rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/ansible/msg_clear_sign.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/clients/__init__.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/clients/msg.py
+-rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/clients/msg_recv_client.py
+-rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/clients/msg_send_client.py
+-rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/clients/registry.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/conf/conf.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/models/msg.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/operations/__init__.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/operations/base.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/operations/clearsign.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/operations/containersign.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/results/__init__.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/results/clearsign.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/results/containersign.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/results/operation_result.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/results/signing_results.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/signers/__init__.py
+-rw-r--r--   0        0        0    14528 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/signers/cosignsigner.py
+-rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/src/pubtools/sign/signers/msgsigner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0    16932 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/conftest.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/conftest_cosignsig.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/conftest_msgsig.py
+-rw-r--r--   0        0        0     5293 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_ansible_clearsign.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_bundle.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_config.py
+-rw-r--r--   0        0        0    25384 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_cosign_signer.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_msg_handle.py
+-rw-r--r--   0        0        0    12970 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_msg_recv_client.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_msg_send_client.py
+-rw-r--r--   0        0        0    42730 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_msg_signer.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_registry_client.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_results.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_sign_operations.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/tests/test_utils.py
+-rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/utils/pre-commit
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/.gitignore
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/LICENSE
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/README.rst
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pubtools_sign-0.0.6/PKG-INFO
```

### Comparing `pubtools_sign-0.0.5/AppImageBuilder.yml` & `pubtools_sign-0.0.6/AppImageBuilder.yml`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/tox.ini` & `pubtools_sign-0.0.6/tox.ini`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/.github/workflows/docs.yml` & `pubtools_sign-0.0.6/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/.github/workflows/owasp.yml` & `pubtools_sign-0.0.6/.github/workflows/owasp.yml`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/.github/workflows/release.yml` & `pubtools_sign-0.0.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/.github/workflows/tox-tests.yml` & `pubtools_sign-0.0.6/.github/workflows/tox-tests.yml`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/docs/Makefile` & `pubtools_sign-0.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/docs/make.bat` & `pubtools_sign-0.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/docs/source/CHANGELOG.rst` & `pubtools_sign-0.0.6/docs/source/CHANGELOG.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 ChangeLog
 =========
 
+0.0.6 (25-04-2024)
+-------------------
+Add OTEL trace instrument for signing
+Added send+recv retry cycles
+
 0.0.5 (19-02-2024)
 -------------------
 * Added cosin support
 * Added support of key aliases
 * Added --log-level for cli entrypoints
 * Exposed operation model to signed results
 * Starts receiver before sender in msg signer
```

### Comparing `pubtools_sign-0.0.5/docs/source/conf.py` & `pubtools_sign-0.0.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/src/pubtools/sign/ansible/msg_clear_sign.py` & `pubtools_sign-0.0.6/src/pubtools/sign/ansible/msg_clear_sign.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/src/pubtools/sign/clients/msg.py` & `pubtools_sign-0.0.6/src/pubtools/sign/clients/msg.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/src/pubtools/sign/clients/msg_send_client.py` & `pubtools_sign-0.0.6/src/pubtools/sign/clients/msg_send_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 import json
 import logging
-from typing import List
+from typing import List, Dict, Any
 
 from ..models.msg import MsgMessage, MsgError
 
 from .msg import _MsgClient
 
 import proton
 import proton.utils
 from proton.reactor import Container
 
+from pubtools.tracing import get_trace_wrapper
+
+from opentelemetry.trace.propagation.tracecontext import TraceContextTextMapPropagator
+
+tw = get_trace_wrapper()
+propagator = TraceContextTextMapPropagator()
 LOG = logging.getLogger("pubtools.sign.signers.radas")
 
 
 class _SendClient(_MsgClient):
     def __init__(
         self,
         messages: List[MsgMessage],
         broker_urls: List[str],
         cert: str,
         ca_cert: str,
         errors: List[MsgError],
-    ):
-        super().__init__(errors=errors)
+        **kwargs: Dict[str, Any],
+    ) -> None:
+        super().__init__(errors=errors, **kwargs)
         self.broker_urls = broker_urls
         self.messages = messages
         self.ssl_domain = proton.SSLDomain(proton.SSLDomain.MODE_CLIENT)
         if cert:
             self.ssl_domain.set_credentials(cert, cert, None)
         if ca_cert:
             self.ssl_domain.set_trusted_ca_db(ca_cert)
@@ -37,33 +44,35 @@
 
     def on_start(self, event: proton.Event) -> None:
         conn = event.container.connect(
             urls=self.broker_urls, ssl_domain=self.ssl_domain, sasl_enabled=False
         )
         self.sender = event.container.create_sender(conn)
 
+    @tw.instrument_func()
     def on_sendable(self, event: proton.Event) -> None:
-        LOG.debug("Sender on_sendable")
-        if self.sent < self.total:
+        if event.sender.credit and self.sent < self.total:
             message = self.messages[self.sent]
+            # Inject trace context to message properties
+            propagator.inject(carrier=message.headers)
             LOG.debug("Sending message: %s %s %s", message.body, message.address, message.headers)
             event.sender.send(
                 proton.Message(
                     properties=message.headers,
                     address=message.address,
                     body=json.dumps(message.body),
                 )
             )
             self.sent += 1
 
     def on_accepted(self, event: proton.Event) -> None:
-        LOG.debug("Sender accepted")
+        # LOG.info("Sender accepted")
         self.confirmed += 1
         if self.confirmed == self.total:
-            LOG.debug("Sender closing")
+            LOG.info("Sender closing")
             event.connection.close()
 
     def on_disconnected(self, event: proton.Event) -> None:  # pragma: no cover
         self.sent = self.confirmed  # pragma: no cover
 
 
 class SendClient(Container):
@@ -73,15 +82,16 @@
         self,
         messages: List[MsgMessage],
         broker_urls: List[str],
         cert: str,
         ca_cert: str,
         retries: int,
         errors: List[MsgError],
-    ):
+        **kwargs: Dict[str, Any],
+    ) -> None:
         """Send Client Initializer.
 
         :param messages: List of messages to send.
         :type messages: List[MsgMessage]
         :param broker_urls: List of addresses of messaging broker
         :type messages: List[str]
         :param cert: Messaging client certificate
@@ -93,15 +103,15 @@
         """
         self.messages = messages
         self.handler = _SendClient(
             messages=messages, broker_urls=broker_urls, cert=cert, ca_cert=ca_cert, errors=errors
         )
         self._retries = retries
         self._errors = errors
-        super().__init__(self.handler)
+        super().__init__(self.handler, **kwargs)
 
     def run(self) -> List[MsgError]:
         """Run the SendClient."""
         errors_len = 0
         if not len(self.messages):
             LOG.warning("No messages to send")
             return []
```

### Comparing `pubtools_sign-0.0.5/src/pubtools/sign/clients/registry.py` & `pubtools_sign-0.0.6/src/pubtools/sign/clients/registry.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/src/pubtools/sign/conf/conf.py` & `pubtools_sign-0.0.6/src/pubtools/sign/conf/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     messaging_ca_cert = ma.fields.String(required=True)
     topic_send_to = ma.fields.String(required=True)
     topic_listen_to = ma.fields.String(required=True)
     environment = ma.fields.String(required=True)
     service = ma.fields.String(required=True)
     timeout = ma.fields.Integer(required=True)
     retries = ma.fields.Integer(required=True)
+    send_retries = ma.fields.Integer(required=True)
     message_id_key = ma.fields.String(required=True)
     log_level = ma.fields.String(default="INFO")
     key_aliases = ma.fields.Dict(required=False, keys=ma.fields.String(), values=ma.fields.String())
 
 
 class CosignSignerSchema(ma.Schema):
     """Cosign signer configuration schema."""
```

### Comparing `pubtools_sign-0.0.5/src/pubtools/sign/operations/base.py` & `pubtools_sign-0.0.6/src/pubtools/sign/operations/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 @dataclass
 class SignOperation(ABC):
     """SignOperation Abstract class."""
 
     ResultType: ClassVar[OperationResult]
     signing_key: str
-    repo: str
 
     @classmethod
     def doc_arguments(cls: Type[Self]) -> Dict[str, Any]:
         """Return dictionary with arguments description of the operation."""
         doc_arguments = {}
         options_arguments_doc = {}
         exmaple_arguments_doc = {}
```

### Comparing `pubtools_sign-0.0.5/src/pubtools/sign/operations/clearsign.py` & `pubtools_sign-0.0.6/src/pubtools/sign/operations/clearsign.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/src/pubtools/sign/operations/containersign.py` & `pubtools_sign-0.0.6/src/pubtools/sign/operations/containersign.py`

 * *Files 25% similar despite different names*

```diff
@@ -18,25 +18,16 @@
     references: List[str] = field(metadata={"description": "List of references to sign"})
     signing_key: str = field(
         metadata={"description": "Signing key short id which should be used for signing"}
     )
     task_id: str = field(
         metadata={"description": "Usually pub task id, serves as identifier for in signing request"}
     )
-    repo: str = field(
-        metadata={
-            "type": "str",
-            "description": "Repository name",
-            "required": "true",
-            "sample": "repo",
-        }
-    )
 
     def to_dict(self) -> dict[str, Any]:
         """Return a dict representation of the object."""
         return dict(
             digests=self.digests,
             references=self.references,
             signing_key=self.signing_key,
             task_id=self.task_id,
-            repo=self.repo,
         )
```

### Comparing `pubtools_sign-0.0.5/src/pubtools/sign/results/__init__.py` & `pubtools_sign-0.0.6/src/pubtools/sign/results/__init__.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/src/pubtools/sign/results/clearsign.py` & `pubtools_sign-0.0.6/src/pubtools/sign/results/clearsign.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/src/pubtools/sign/results/containersign.py` & `pubtools_sign-0.0.6/src/pubtools/sign/results/containersign.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/src/pubtools/sign/results/signing_results.py` & `pubtools_sign-0.0.6/src/pubtools/sign/results/signing_results.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/src/pubtools/sign/signers/__init__.py` & `pubtools_sign-0.0.6/src/pubtools/sign/signers/__init__.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/src/pubtools/sign/signers/cosignsigner.py` & `pubtools_sign-0.0.6/src/pubtools/sign/signers/cosignsigner.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,14 +268,15 @@
             outputs[ref] = (stdout, stderr, process.returncode)
 
         for ref, (stdout, stderr, returncode) in outputs.items():
             if returncode != 0:
                 operation_result.results.append(stderr)
                 operation_result.failed = True
                 signing_results.signer_results.status = "failed"
+                signing_results.signer_results.error_message += stderr
             else:
                 operation_result.results.append(stderr)
         signing_results.operation_result = operation_result
         return signing_results
 
     def existing_signatures(self, reference: str) -> Tuple[bool, str]:
         """Return list of existing signatures for given reference.
@@ -338,15 +339,14 @@
     cosign_signer.load_config(load_config(os.path.expanduser(config)))
 
     operation = ContainerSignOperation(
         digests=digest,
         references=reference,
         signing_key=signing_key,
         task_id="",
-        repo="",
     )
     signing_result = cosign_signer.sign(operation)
     return {
         "signer_result": signing_result.signer_results.to_dict(),
         "operation_results": signing_result.operation_result.results,  # type: ignore
         "operation": signing_result.operation.to_dict(),
         "signing_key": signing_result.operation_result.signing_key,
```

### Comparing `pubtools_sign-0.0.5/src/pubtools/sign/signers/msgsigner.py` & `pubtools_sign-0.0.6/src/pubtools/sign/signers/msgsigner.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,22 @@
 from ..results import ClearSignResult, ContainerSignResult
 from ..results import SignerResults
 from ..exceptions import UnsupportedOperation
 from ..clients.msg_send_client import SendClient
 from ..clients.msg_recv_client import RecvClient, RecvThread
 from ..models.msg import MsgMessage, MsgError
 from ..conf.conf import load_config, CONFIG_PATHS
-from ..utils import set_log_level, sanitize_log_level, isodate_now, _get_config_file
+from ..utils import (
+    set_log_level,
+    sanitize_log_level,
+    isodate_now,
+    _get_config_file,
+    run_in_parallel,
+    FData,
+)
 
 
 LOG = logging.getLogger("pubtools.sign.signers.msgsigner")
 
 
 class SignRequestType(str, enum.Enum):
     """Sign request type enum."""
@@ -116,20 +123,25 @@
     )
     service: str = field(
         init=False, metadata={"description": "Service identificator", "sample": "pubtools-sign"}
     )
     timeout: int = field(
         init=False,
         default=60,
-        metadata={"description": "Timeout for messaging sent/receive", "sample": 1},
+        metadata={"description": "Timeout for messaging receive", "sample": 1},
     )
     retries: int = field(
         init=False,
-        default=60,
-        metadata={"description": "Retries for messaging sent/receive", "sample": 3},
+        default=3,
+        metadata={"description": "Retries for messaging receive", "sample": 3},
+    )
+    send_retries: int = field(
+        init=False,
+        default=2,
+        metadata={"description": "Retries for messaging send+receive", "sample": 2},
     )
     message_id_key: str = field(
         init=False,
         metadata={
             "description": "Attribute name in message body which should be used as message id",
             "sample": "123",
         },
@@ -186,28 +198,29 @@
         if extra_attrs:
             headers.update(extra_attrs)
         return headers
 
     def _create_msg_message(
         self: MsgSigner,
         data: str,
+        repo: str,
         operation: SignOperation,
         sig_type: SignRequestType,
         extra_attrs: Optional[Dict[str, Any]] = None,
     ) -> MsgMessage:
         if operation.signing_key in self.key_aliases:
             signing_key = self.key_aliases[operation.signing_key]
         else:
             signing_key = operation.signing_key
         ret = MsgMessage(
             headers=self._construct_headers(sig_type, extra_attrs=extra_attrs),
             body=self._construct_signing_message(
                 data,
                 signing_key,
-                repo=operation.repo,
+                repo,
                 extra_attrs=extra_attrs,
                 sig_type=sig_type.value,
             ),
             address=self.topic_send_to.format(
                 **dict(list(asdict(self).items()) + list(asdict(operation).items()))
             ),
         )
@@ -223,24 +236,25 @@
         self.messaging_ca_cert = os.path.expanduser(config_data["msg_signer"]["messaging_ca_cert"])
         self.topic_send_to = config_data["msg_signer"]["topic_send_to"]
         self.topic_listen_to = config_data["msg_signer"]["topic_listen_to"]
         self.environment = config_data["msg_signer"]["environment"]
         self.service = config_data["msg_signer"]["service"]
         self.message_id_key = config_data["msg_signer"]["message_id_key"]
         self.retries = config_data["msg_signer"]["retries"]
+        self.send_retries = config_data["msg_signer"]["send_retries"]
         self.log_level = config_data["msg_signer"]["log_level"]
         self.timeout = config_data["msg_signer"]["timeout"]
         self.creator = self._get_cert_subject_cn()
         self.key_aliases = config_data["msg_signer"].get("key_aliases", {})
 
     def _get_cert_subject_cn(self) -> str:
         x509 = crypto.load_certificate(
             crypto.FILETYPE_PEM, open(os.path.expanduser(self.messaging_cert_key)).read().encode()
         )
-        return x509.get_subject().CN
+        return x509.get_subject().CN or x509.get_subject().UID  # type: ignore[attr-defined]
 
     def operations(self: MsgSigner) -> List[Type[SignOperation]]:
         """Return list of supported operations."""
         return self.SUPPORTED_OPERATIONS
 
     def sign(self: MsgSigner, operation: SignOperation) -> SigningResults:
         """Run signing operation.
@@ -267,21 +281,24 @@
         """
         set_log_level(LOG, self.log_level)
         messages = []
         message_to_data = {}
         for in_data in operation.inputs:
             message = self._create_msg_message(
                 base64.b64encode(in_data.encode("latin1")).decode("latin-1"),
+                operation.repo,
                 operation,
                 SignRequestType.CLEARSIGN,
                 extra_attrs={"pub_task_id": operation.task_id},
             )
             message_to_data[message.body["request_id"]] = message
             messages.append(message)
 
+        all_messages = [x for x in messages]
+
         signing_key = operation.signing_key
         if signing_key in self.key_aliases:
             signing_key = self.key_aliases[signing_key]
             LOG.info(f"Using signing key alias {signing_key} for {operation.signing_key}")
 
         signer_results = MsgSignerResults(status="ok", error_message="")
         operation_result = ClearSignResult(
@@ -289,65 +306,107 @@
         )
         signing_results = SigningResults(
             signer=self,
             operation=operation,
             signer_results=signer_results,
             operation_result=operation_result,
         )
-        LOG.debug(f"{len(messages)} messages to send")
-
         errors: List[MsgError] = []
-        message_ids = [message.body["request_id"] for message in messages]
+        received: Dict[int, Any] = {}
+        LOG.info("errors " + str(errors))
 
-        recvc = RecvClient(
-            message_ids=message_ids,
-            topic=self.topic_listen_to.format(
-                **dict(list(asdict(self).items()) + list(asdict(operation).items()))
-            ),
-            id_key=self.message_id_key,
-            broker_urls=self.messaging_brokers,
-            cert=self.messaging_cert_key,
-            ca_cert=self.messaging_ca_cert,
-            timeout=self.timeout,
-            retries=self.retries,
-            errors=errors,
-        )
-        recvt = RecvThread(recvc)
-        recvt.start()
-
-        errors = SendClient(
-            messages=messages,
-            broker_urls=self.messaging_brokers,
-            cert=self.messaging_cert_key,
-            ca_cert=self.messaging_ca_cert,
-            retries=self.retries,
-            errors=errors,
-        ).run()
-
-        if errors:
-            signer_results.status = "error"
-            for error in errors:
-                signer_results.error_message += f"{error.name} : {error.description}\n"
-            return signing_results
+        for i in range(self.send_retries):
+            message_ids = [message.body["request_id"] for message in messages]
+            LOG.debug(f"{len(messages)} messages to send")
+            recvc = RecvClient(
+                uid=str(i),
+                message_ids=message_ids,
+                topic=self.topic_listen_to.format(
+                    **dict(list(asdict(self).items()) + list(asdict(operation).items()))
+                ),
+                id_key=self.message_id_key,
+                broker_urls=self.messaging_brokers,
+                cert=self.messaging_cert_key,
+                ca_cert=self.messaging_ca_cert,
+                timeout=self.timeout,
+                retries=self.retries,
+                errors=errors,
+                received=received,
+            )
+            recvt = RecvThread(recvc)
+            recvt.start()
 
-        recvt.join()
+            errors = SendClient(
+                messages=messages,
+                broker_urls=self.messaging_brokers,
+                cert=self.messaging_cert_key,
+                ca_cert=self.messaging_ca_cert,
+                retries=self.retries,
+                errors=errors,
+            ).run()
+            # check sender errors
+            if errors:
+                signer_results.status = "error"
+                for error in errors:
+                    signer_results.error_message += f"{error.name} : {error.description}\n"
+                return signing_results
+
+            # wait for receiver to finish
+            recvt.join()
+            recvt.stop()
+
+            # check receiver errors
+            for x in range(self.retries - 1):
+                errors = recvc._errors
+                if errors and errors[0].name == "MessagingTimeout":
+                    LOG.info("RETRYING %s", x)
+                    _messages = []
+                    for message in messages:
+                        if message.body["request_id"] not in received:
+                            _messages.append(message)
+                    if x != self.retries - 1:
+                        errors.pop(0)
+                    messages = _messages
+                    message_ids = [message.body["request_id"] for message in messages]
+
+                    LOG.info("Retrying recv")
+                    recvc = RecvClient(
+                        uid=str(i) + "-" + str(x),
+                        message_ids=message_ids,
+                        topic=self.topic_listen_to.format(
+                            **dict(list(asdict(self).items()) + list(asdict(operation).items()))
+                        ),
+                        id_key=self.message_id_key,
+                        broker_urls=self.messaging_brokers,
+                        cert=self.messaging_cert_key,
+                        ca_cert=self.messaging_ca_cert,
+                        timeout=self.timeout,
+                        retries=self.retries,
+                        errors=errors,
+                        received=received,
+                    )
+                    recvt = RecvThread(recvc)
+                    recvt.start()
+                    recvt.join()
+                elif not errors:
+                    break
 
         errors = recvc._errors
         if errors:
             signer_results.status = "error"
             for error in errors:
                 signer_results.error_message += f"{error.name} : {error.description}\n"
             return signing_results
 
         operation_result = ClearSignResult(
-            signing_key=operation.signing_key, outputs=[""] * len(messages)
+            signing_key=operation.signing_key, outputs=[""] * len(all_messages)
         )
 
-        for recv_id, received in recvc.recv.items():
-            operation_result.outputs[messages.index(message_to_data[recv_id])] = received
+        for recv_id, _received in recvc.recv.items():
+            operation_result.outputs[all_messages.index(message_to_data[recv_id])] = _received
         signing_results.operation_result = operation_result
         return signing_results
 
     @staticmethod
     def create_manifest_claim_message(signature_key: str, digest: str, reference: str) -> str:
         """Create manifest claim for container signing.
 
@@ -379,86 +438,158 @@
             raise ValueError("Digests must pairs with references")
 
         signing_key = operation.signing_key
         if signing_key in self.key_aliases:
             signing_key = self.key_aliases[signing_key]
             LOG.info(f"Using signing key alias {signing_key} for {operation.signing_key}")
 
+        LOG.info(f"Container sign operation for {len(operation.digests)}")
+
+        fargs = []
         for digest, reference in zip(operation.digests, operation.references):
-            message = self._create_msg_message(
-                self.create_manifest_claim_message(signing_key, digest=digest, reference=reference),
-                operation,
-                SignRequestType.CONTAINER,
-                extra_attrs={"pub_task_id": operation.task_id, "manifest_digest": digest},
+            repo = reference.split("/", 1)[1].split(":")[0]
+            fargs.append(
+                FData(
+                    args=[
+                        self.create_manifest_claim_message(
+                            signing_key, digest=digest, reference=reference
+                        ),
+                        repo,
+                        operation,
+                        SignRequestType.CONTAINER,
+                    ],
+                    kwargs={
+                        "extra_attrs": {"pub_task_id": operation.task_id, "manifest_digest": digest}
+                    },
+                )
             )
+        ret = run_in_parallel(self._create_msg_message, fargs)
+        for n, message in ret.items():
             message_to_data[message.body["request_id"]] = message
             messages.append(message)
 
+        all_messages = [x for x in messages]
+        LOG.info(f"Signing {len(all_messages)}")
+
         signer_results = MsgSignerResults(status="ok", error_message="")
         operation_result = ContainerSignResult(
             signing_key=operation.signing_key, results=[""] * len(operation.digests), failed=False
         )
         signing_results = SigningResults(
             signer=self,
             operation=operation,
             signer_results=signer_results,
             operation_result=operation_result,
         )
         LOG.debug(f"{len(messages)} messages to send")
 
         errors: List[MsgError] = []
+        received: Dict[int, Any] = {}
+        LOG.info(
+            "Starting signing process. Retries %d,%d, timeout: %d",
+            self.send_retries,
+            self.retries,
+            self.timeout,
+        )
+
+        for i in range(self.send_retries):
+            message_ids = [message.body["request_id"] for message in messages]
+            recvc = RecvClient(
+                uid=str(i),
+                message_ids=message_ids,
+                topic=self.topic_listen_to.format(
+                    **dict(list(asdict(self).items()) + list(asdict(operation).items()))
+                ),
+                id_key=self.message_id_key,
+                broker_urls=self.messaging_brokers,
+                cert=self.messaging_cert_key,
+                ca_cert=self.messaging_ca_cert,
+                timeout=self.timeout,
+                retries=self.retries,
+                errors=errors,
+                received=received,
+            )
+            recvt = RecvThread(recvc)
+            recvt.start()
 
-        message_ids = [message.body["request_id"] for message in messages]
-        recvc = RecvClient(
-            message_ids=message_ids,
-            topic=self.topic_listen_to.format(
-                **dict(list(asdict(self).items()) + list(asdict(operation).items()))
-            ),
-            id_key=self.message_id_key,
-            broker_urls=self.messaging_brokers,
-            cert=self.messaging_cert_key,
-            ca_cert=self.messaging_ca_cert,
-            timeout=self.timeout,
-            retries=self.retries,
-            errors=errors,
-        )
-        recvt = RecvThread(recvc)
-        recvt.start()
-
-        errors = SendClient(
-            messages=messages,
-            broker_urls=self.messaging_brokers,
-            cert=self.messaging_cert_key,
-            ca_cert=self.messaging_ca_cert,
-            retries=self.retries,
-            errors=errors,
-        ).run()
-
-        if errors:
-            signer_results.status = "error"
-            for error in errors:
-                signer_results.error_message += f"{error.name} : {error.description}\n"
-            return signing_results
-
-        # wait for receiver to finish
-        recvt.join()
+            errors = SendClient(
+                messages=messages,
+                broker_urls=self.messaging_brokers,
+                cert=self.messaging_cert_key,
+                ca_cert=self.messaging_ca_cert,
+                retries=self.retries,
+                errors=errors,
+            ).run()
+
+            # check sender errors
+            if errors:
+                signer_results.status = "error"
+                for error in errors:
+                    signer_results.error_message += f"{error.name} : {error.description}\n"
+                return signing_results
+
+            # wait for receiver to finish
+            recvt.join()
+            recvt.stop()
+            received = recvc.get_received()
+
+            for x in range(self.retries):
+                errors = recvc.get_errors()
+                if errors and errors[0].name == "MessagingTimeout":
+                    LOG.info("Retrying receiving %s/%s", x, self.retries)
+                    _messages = []
+                    for message in messages:
+                        if message.body["request_id"] not in received:
+                            _messages.append(message)
+                    if x != self.retries - 1:
+                        errors.pop(0)
+                    messages = _messages
+                    if not messages:
+                        break
+                    message_ids = [message.body["request_id"] for message in messages]
+
+                    recvc = RecvClient(
+                        uid=str(i) + "-" + str(x),
+                        message_ids=message_ids,
+                        topic=self.topic_listen_to.format(
+                            **dict(list(asdict(self).items()) + list(asdict(operation).items()))
+                        ),
+                        id_key=self.message_id_key,
+                        broker_urls=self.messaging_brokers,
+                        cert=self.messaging_cert_key,
+                        ca_cert=self.messaging_ca_cert,
+                        timeout=self.timeout,
+                        retries=self.retries,
+                        errors=errors,
+                        received=received,
+                    )
+                    recvt = RecvThread(recvc)
+                    recvt.start()
+                    recvt.join()
+                elif not errors:
+                    break
+                received = recvc.get_received()
+
+            # check receiver errors
+            errors = recvc.get_errors()
+            if not errors:
+                break
 
-        errors = recvc._errors
         if errors:
             signer_results.status = "error"
             for error in errors:
                 signer_results.error_message += f"{error.name} : {error.description}\n"
             return signing_results
 
         operation_result = ContainerSignResult(
-            signing_key=operation.signing_key, results=[""] * len(messages), failed=False
+            signing_key=operation.signing_key, results=[""] * len(all_messages), failed=False
         )
-        for recv_id, received in recvc.recv.items():
-            operation_result.failed = True if received[0]["msg"]["errors"] else False
-            operation_result.results[messages.index(message_to_data[recv_id])] = received
+        for recv_id, _received in recvc.recv.items():
+            operation_result.failed = True if _received[0]["msg"]["errors"] else False
+            operation_result.results[all_messages.index(message_to_data[recv_id])] = _received
         signing_results.operation_result = operation_result
         return signing_results
 
 
 def msg_clear_sign(
     inputs: List[str],
     signing_key: str = "",
@@ -491,27 +622,25 @@
 
 def msg_container_sign(
     signing_key: str = "",
     task_id: str = "",
     config_file: str = "",
     digest: list[str] = [],
     reference: list[str] = [],
-    repo: str = "",
 ) -> Dict[str, Any]:
     """Run containersign operation with cli arguments."""
     msg_signer = MsgSigner()
     config = _get_config_file(config_file)
     msg_signer.load_config(load_config(os.path.expanduser(config)))
 
     operation = ContainerSignOperation(
         digests=digest,
         references=reference,
         signing_key=signing_key,
         task_id=task_id,
-        repo=repo,
     )
     signing_result = msg_signer.sign(operation)
     return {
         "signer_result": signing_result.signer_results.to_dict(),
         "operation_results": signing_result.operation_result.results,  # type: ignore
         "operation": signing_result.operation.to_dict(),
         "signing_key": signing_result.operation_result.signing_key,
@@ -601,38 +730,35 @@
 @click.option("--raw", default=False, is_flag=True, help="Print raw output instead of json")
 @click.option(
     "--log-level",
     type=click.Choice(["DEBUG", "INFO", "WARNING", "ERROR"]),
     default="INFO",
     help="Set log level",
 )
-@click.option("--repo", help="Repository reference")
 def msg_container_sign_main(
     signing_key: str = "",
     task_id: str = "",
     config_file: str = "",
     digest: List[str] = [],
     reference: List[str] = [],
     raw: bool = False,
     log_level: str = "INFO",
-    repo: str = "",
 ) -> None:
     """Entry point method for containersign operation."""
     ch = logging.StreamHandler()
     ch.setLevel(getattr(logging, sanitize_log_level(log_level)))
     LOG.addHandler(ch)
     logging.basicConfig(level=getattr(logging, sanitize_log_level(log_level)))
 
     ret = msg_container_sign(
         signing_key=signing_key,
         task_id=task_id,
         config_file=config_file,
         digest=digest,
         reference=reference,
-        repo=repo,
     )
     if not raw:
         click.echo(json.dumps(ret))
         if ret["signer_result"]["status"] == "error":
             sys.exit(1)
     else:
         for claim in ret["operation_results"]:
```

### Comparing `pubtools_sign-0.0.5/tests/conftest.py` & `pubtools_sign-0.0.6/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,22 @@
 import socket
 import logging
 from multiprocessing import Process
 import threading
 import tempfile
 import uuid
 import os
+import sys
+
 from unittest.mock import patch
 
 from .conftest_msgsig import (  # noqa: F401
     f_msg_signer,  # noqa: F401
     f_config_msg_signer_ok,  # noqa: F401
+    f_config_msg_signer_ok2,  # noqa: F401
     f_config_msg_signer_aliases,  # noqa: F401
 )  # noqa: F401
 from .conftest_cosignsig import (  # noqa: F401
     f_cosign_signer,  # noqa: F401
     f_config_cosign_signer_ok,  # noqa: F401
     f_config_cosign_signer_aliases,  # noqa: F401
     f_config_cosign_signer_no_auth,
@@ -29,14 +32,15 @@
 
 from pytest import fixture
 
 from pubtools.sign.clients.msg import _MsgClient
 
 
 LOG = logging.getLogger("pubtools.sign.signers.radas")
+LOG.addHandler(logging.StreamHandler(sys.stdout))
 
 
 class _Queue(object):
     def __init__(self, address, dynamic=False):
         self.address = address
         self.dynamic = dynamic
         self.queue = collections.deque()
@@ -83,24 +87,37 @@
 class _Broker(_MsgClient):
     def __init__(self, url):
         super().__init__(errors=[])
         self.url = url
         self.queues = {}
 
     def on_start(self, event):
-        LOG.debug("BROKER on start", self.url)
+        print("BROKER on start", self.url)
+        LOG.info("BROKER on start", self.url)
         self.acceptor = event.container.listen(self.url)
 
     def _queue(self, address):
         if address not in self.queues:
             self.queues[address] = _Queue(address)
         return self.queues[address]
 
     def on_link_opening(self, event):
-        LOG.debug(
+        LOG.info(
+            "BROKER on_link_opening event",
+            event.link,
+            "source addr:",
+            event.link.source.address,
+            "remote source addr",
+            event.link.remote_source.address,
+            "target addr:",
+            event.link.target.address,
+            "remote target addr",
+            event.link.remote_target.address,
+        )
+        print(
             "BROKER on_link_opening event",
             event.link,
             "source addr:",
             event.link.source.address,
             "remote source addr",
             event.link.remote_source.address,
             "target addr:",
@@ -124,46 +141,46 @@
     def _unsubscribe(self, link):
         if link.source.address in self.queues and self.queues[link.source.address].unsubscribe(
             link
         ):
             del self.queues[link.source.address]
 
     def on_link_closing(self, event):
-        LOG.debug(">> BROKER On link closing", event)
+        LOG.info(">> BROKER On link closing", event)
         if event.link.is_sender:
             self._unsubscribe(event.link)
 
     def on_disconnected(self, event):
-        LOG.debug(">> BROKER On disconnected", event)
+        LOG.info(">> BROKER On disconnected", event)
         self.remove_stale_consumers(event.connection)
 
     def remove_stale_consumers(self, connection):
         link = connection.link_head(Endpoint.REMOTE_ACTIVE)
-        LOG.debug("BROKER removing stale consumer", link)
+        LOG.info("BROKER removing stale consumer", link)
         while link:
             if link.is_sender:
                 self._unsubscribe(link)
             link = link.next(Endpoint.REMOTE_ACTIVE)
 
     def on_sendable(self, event):
-        LOG.debug("BROKER on_sendable", event.link.source.address)
+        LOG.info("BROKER on_sendable", event.link.source.address)
         self._queue(event.link.source.address).dispatch(event.link)
 
     def on_message(self, event):
-        LOG.debug("BROKER ON MESSAGE", event.message)
+        LOG.info("BROKER ON MESSAGE", event.message)
         address = event.link.target.address
         if address is None:
             address = event.message.address
         LOG.debug("BROKER publish", address)
         self._queue(address).publish(event.message)
 
 
 class _BrokenBroker(_Broker):
     def on_sendable(self, event):
-        LOG.debug("BROKER on_sendable", event.link.source.address)
+        LOG.info("BROKER on_sendable", event.link.source.address)
         self._queue(event.link.source.address).dispatch(event.link)
         raise ValueError("Simulated broker error")
         event.on_link_error(event)
 
 
 class _FakeMsgSigner(proton.handlers.MessagingHandler):
     def __init__(self, broker_urls, listen_to, send_to, cert, ca_cert, received_messages):
@@ -233,14 +250,19 @@
 
         reply.properties = event.message.properties
 
         sender = event.container.create_sender(event.connection)
         sender.send(reply)
 
 
+def run_broker(broker, stdout):
+    sys.stdout = stdout
+    broker.run()
+
+
 @fixture(scope="session")
 def f_msgsigner_listen_to_topic():
     return "topic://Topic.pubtools.sign"
 
 
 @fixture(scope="session")
 def f_msgsigner_send_to_queue():
@@ -283,20 +305,20 @@
     port = sock.getsockname()[1]
     sock.close()
     return port
 
 
 @fixture(scope="session")
 def f_qpid_broker(f_find_available_port):
-    LOG.debug("starting broker", f"localhost:{f_find_available_port}")
+    LOG.info("starting broker", f"localhost:{f_find_available_port}")
     broker = Container(_Broker(f"localhost:{f_find_available_port}"))
-    p = Process(target=broker.run, args=())
+    p = Process(target=run_broker, args=(broker, sys.stdout))
     p.start()
     yield (broker, f_find_available_port)
-    LOG.debug("destroying qpid broker")
+    LOG.info("destroying qpid broker")
     p.terminate()
 
 
 @fixture(scope="session")
 def f_broken_qpid_broker(f_find_available_port_for_broken):
     LOG.debug("starting broker", f"localhost:{f_find_available_port_for_broken}")
     broker = Container(_BrokenBroker(f"localhost:{f_find_available_port_for_broken}"))
@@ -352,64 +374,64 @@
 
 
 @fixture
 def f_client_certificate():
     with tempfile.NamedTemporaryFile() as tmpf:
         tmpf.write(
             """
------BEGIN RSA PRIVATE KEY-----
-MIIEpQIBAAKCAQEAxcdD7r4IdRBrylZnLNmHMu4AHnt1ReE7LhvIJj9XF+akW9pa
-Nc7rY+dHGZVd45VUsS37MuGRzkl4gUs/wAh+4PQK+dDGqDY5nJL7QNgw96s1129d
-O09inhUBFp7tMfc+xAuNvDSrxRHthwnDIU2Jrbl6fzube07g0qx7geCqxti/g5cg
-xuQBQpHSpaRgZ7cyNuiyww1vssbqqAG8UZHb4SpwaqjXnPp6Vd/yrU3bRKAtD5s5
-+ZxCa/dUJfsqS3jxQMlfH0lbvxZ5yR+4pLRAISKLfdTDcN56XJ6IstNyusNhr/76
-C/CfWUN+oe5yCWbRx4L5Q6lcpDq5DcbMNswEoQIDAQABAoIBAQCUDQWCW0jzcNZv
-wdw8S54Udusp5ls0c1Ucv/lFAFdO8f2JMNwkuX+l6oRj11dQPQIIHBaV0RuXo5IM
-n2racsGf3a+1sB513xmjZreko/GMBOMqIRhWhKebFLga2d9PbvjSQp/YCkmnHTOE
-yb8DWAq/PEBBrDpIxRQxQKK355mPfW/OT2ds/C9Qeg/JtqX8N+OyPLzXNV1Ga1OE
-GSMm0sv4TTyq5MrQDxx3C/MkjEwnDWkjV5kQhQHGJ+ehlXbkQqIAyfOLvWLIhu7t
-e9mWRykqoBJUU1/eks9QohHtrgFHdbwwI1bsxxZCTirRXPpen0/SEWZ4jUkPB6MV
-vdqGxJoRAoGBAP92liL2yMP/27Bi/hBjTpKMCZsH7Hl04RSrJZ6AzxPlglh2deCG
-bpmffItcvUymLKMbIixo2mdQ0M3tqIFtA7k7M/ZGRNkYRI17J4kXoFa0qvX4zULl
-csLDau0DMVTrCoXRlWmozp9Ony4kAp5xh7ygIFyE+rw2G48pxNkotOkNAoGBAMYx
-pnZQn1eD4TLERy+s679LWupFLjlasaYhHM4mOZR36ABIjzbUSTe5qG8qXs2V0UXF
-G8vaGp8LLIwWg304WWTcErJru6qrp08OlHHPqytuDrQcpqwMkAgA4/xezGJW9ljJ
-wYWTEonWMlfKFP04kVg+CqATBnjVMCii5SjAmrzlAoGBANF8f1WgpbYEZDTamJj7
-tnz6FQ5qiwJ2U/TM/AZkfmtEc4Tzb2p1EtErNchafmkSg9wk7fsY6LB8Vx3nW5z2
-tmz5HX1A1khoXB7g9OS42SUA9ojKRBgta9RGx7IgQh3uuCxQV4PTh8yffm0p3nPr
-iXGmpaL48VvRyvu1NtUVSnUpAoGAeyWEigVkTItsFRAyLyRhwxW+YswjgY2hzljK
-viiwJFkwtWRgYDAdYluglZodF96cDp7/u3VEj0fxIQYoI1ks6md30pbwH4bSyWOE
-xwbDE5Qp3K3kvgh8QgzTnA8HLZ9dKCQMc8PDhBOsajHtQr2wScUa8wV/QvssFkPI
-4b5zJyUCgYEAra20VWtCDvtgVkEYEV3Taqp9lx8g4sW+E3O0/q5hUKjmyC1+xjwS
-i4CYcqbOwSpEBJ6SInJ8qO9mr5H34IrNVMDqQFtQeUs14BubD5SL789jPzzYlPuf
-WtgtGGUuxENK+DcU7zn6px9PqS0Rd8paC7CWrVZpn9fLusC8DAYNyG8=
------END RSA PRIVATE KEY-----
+-----BEGIN PRIVATE KEY-----
+MIIEvQIBADANBgkqhkiG9w0BAQEFAASCBKcwggSjAgEAAoIBAQC1y5rshMkYqfP2
+k7z2IJXto3AvLCAYDN9WX5mUUFgPFAFur38bDopqj5dSkXlR5f3MwZeRCNsxRXKD
+USjv1T9HjD2t2D7eOAQhhx7dtgMPEYRJes02/ejzGojqrXEoG3TsCf8wBmb5ALDc
+VrgEWShRRGi3qzsDXijMtzns+30+/rOfR68+353iLXTJ3g/MkVRLks6xwq35ZbH4
+Ichu/6ISRU7Lk3tOq811a/SFuHdSLrOzU13VDK+6nQiWMUPbHy6OHK88dC+6mRws
+RJuqHg0cKSIA5aiE7T7o9S3v10P0wJnn8B7d+bsHZJPxqLxFdbQ5Ogjrc195TEmf
+kAd4kB8BAgMBAAECggEABwvEdhfuK58cLBWVKoCwMOr/jEuAdbAriI9pXlvIEvMI
+fG3PvkinrZpBwB7wad/BMMo8za+vP6tQdTWcQaHlK0ispBAUXTRkeBhypj8Rgqgw
+FXE9kozgJkp0LazR3L8mLqcTSX0pCOv5ftu7U3tRZkdxi9NWlOKFkCwmkghcBgjE
+M2LZx4mCNbtD0WQYqMr0HdGJsedCNRrmCAZ5eoTM+HIh8C2eCRT4mBirNLIHsg/d
+TqLI9TN0JvDkpTHt7W94Cxi7th5uLrXfE+D5cbHT0OV4L/kwQj3JjZDekUTCqljX
+OcC8X0l8+SYo6+qlc0mmd324LzGmD+fuP9LXnHkc8QKBgQDwUABdZKZWRWMdypj4
+jgzSBZa1k6cDt39373MFwhk+c5nYUm7ijsRncz85Vb8n0vwY6K0DWuP3yNfuKyVe
+BDXZHfgncz3hc+pBa3B/NIxDmI16D2SEomhe+/JyHh1wnOI5DPJFSrWhYtuMvKpv
+QBpQ0rNP8Xq+6c/Gg06g1SFRkQKBgQDBqbCpPOt6+dlR/7aRzbWBe9hUqYegRKw+
+Is+Ap9hcup7zstsKOdjBGt89wV7BV9KQQnE69uOqBx6CdqEUId47C3F661hT/npR
+B9bBdwW7m8FKbu5i86d1V3ddvdNbIkAeqwjSpnkrLzITPJ74w9yhxAxqO/7wMAs1
+PBTpNHo+cQKBgE/f128zYBI2t+4UA+pBlMNN9jzeGdojaKvdm9ajIC7gz5bWN2L4
+XxGffbk55fJ/ryk8VR1TXYhjaloQXzgzoA5NZsj+Behk1czuwBKXzbM+BnA2o4tu
+S9CeX4RMvC5NBug9hF1BqsM8j4rkvqWBof2ROuZsdgb0wgnSZRUSIiPxAoGAHMUg
+wYOTWAmWB2B9tttgg4Pqd2lYBK8vB2wUd4B33A69XmbLs5E0ajubvojjksWBOn0k
+ZSYYXEICfk8xTtRZN1xT13bvAEtl0HPhq4wLBfv1kyE3uOuJjR0ZVovEwl0sOWIf
+RWwFxCyWu9TdqQcv17hQP9f536TDhX0PfjWVk4ECgYEAp5ze8TFxH8PyTqGOGikn
+aKhWL4DD3dNoXCYOrcEmTKOXftlvlrR+6VjCT0DFro9QxQM9S7BEhugmbm/kQoD3
+0jxXWkX9wkN2thOrUwJBHBtj/PUqA+s5bbi//V8pSmdSfXn3HgKaXD40sAoX8HWn
+8n8nYo3EMM6kk5gbZToN33k=
+-----END PRIVATE KEY-----
 -----BEGIN CERTIFICATE-----
-MIIDvjCCAqagAwIBAgIUTTW9wgsEcsPa+nC9LNIY2NQHs/gwDQYJKoZIhvcNAQEL
-BQAwazELMAkGA1UEBhMCdVMxFTATBgNVBAcMDERlZmF1bHQgQ2l0eTEQMA4GA1UE
-CgwHUmVkIEhhdDEbMBkGA1UECwwSQ2xvdWQgRGlzdHJpYnV0aW9uMRYwFAYDVQQD
-DA1wdWJ0b29scy1zaWduMB4XDTIzMDUyNTEyNDQwNVoXDTI1MDgyNzEyNDQwNVow
-cDELMAkGA1UEBhMCVVMxFTATBgNVBAcMDERlZmF1bHQgQ2l0eTEQMA4GA1UECgwH
-UmVkIEhhdDEbMBkGA1UECwwSQ2xvdWQgRGlzdHJpYnV0aW9uMRswGQYDVQQDDBJw
-dWJ0b29scy1zaWduLXRlc3QwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIB
-AQDFx0Puvgh1EGvKVmcs2Ycy7gAee3VF4TsuG8gmP1cX5qRb2lo1zutj50cZlV3j
-lVSxLfsy4ZHOSXiBSz/ACH7g9Ar50MaoNjmckvtA2DD3qzXXb107T2KeFQEWnu0x
-9z7EC428NKvFEe2HCcMhTYmtuXp/O5t7TuDSrHuB4KrG2L+DlyDG5AFCkdKlpGBn
-tzI26LLDDW+yxuqoAbxRkdvhKnBqqNec+npV3/KtTdtEoC0Pmzn5nEJr91Ql+ypL
-ePFAyV8fSVu/FnnJH7iktEAhIot91MNw3npcnoiy03K6w2Gv/voL8J9ZQ36h7nIJ
-ZtHHgvlDqVykOrkNxsw2zAShAgMBAAGjVTBTMB8GA1UdIwQYMBaAFA/iBvXjjDuu
-XOQQoMnHcOtLe896MAkGA1UdEwQCMAAwCwYDVR0PBAQDAgTwMBgGA1UdEQQRMA+C
-DWhlbGxmaXNoLnRlc3QwDQYJKoZIhvcNAQELBQADggEBAMpT7zdPkO4gb3tn74Nb
-aFIhRDr4sQorpMlxRYQZSKV5qjvZ364bHaig380iQMwVs2H09z6IpO/8eXbrtlaD
-z3QH2bt+yofk+JbWjQky7fKB1ZXvpugcNMTgr2OuupqPIkHaE4N+lZmaasMDY3+i
-+1F5U/0EaNYuFt7Tv6uS9cqkbUuvm9Elm71arkDSrdOycTXGmm+DB8XnAGnQpNWQ
-L3WmvVmWzvgjYOxvef2nNE3SeM3+/ZDCNYIJGC3KS/pOdshF95Xy00mkXv+Z0wAL
-iuT88ZskJ2WDrduvxxKPSFUZ1ncZMsRAcNp8B0+JeR9Q30TGJCMNqJ3jg4u8Pvod
-lq4=
+MIIDdTCCAl2gAwIBAgIUSd6+UGxdN+U6W7tYnZwrY1Tn5NYwDQYJKoZIhvcNAQEL
+BQAwSjFIMAkGA1UEBhMCVVMwGQYDVQQDDBJwdWJ0b29scy1zaWduLXRlc3QwIAYK
+CZImiZPyLGQBAQwScHVidG9vbHMtc2lnbi10ZXN0MB4XDTI0MDMwNjEyMzY0MloX
+DTI0MDQwNTEyMzY0MlowSjFIMAkGA1UEBhMCVVMwGQYDVQQDDBJwdWJ0b29scy1z
+aWduLXRlc3QwIAYKCZImiZPyLGQBAQwScHVidG9vbHMtc2lnbi10ZXN0MIIBIjAN
+BgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAtcua7ITJGKnz9pO89iCV7aNwLywg
+GAzfVl+ZlFBYDxQBbq9/Gw6Kao+XUpF5UeX9zMGXkQjbMUVyg1Eo79U/R4w9rdg+
+3jgEIYce3bYDDxGESXrNNv3o8xqI6q1xKBt07An/MAZm+QCw3Fa4BFkoUURot6s7
+A14ozLc57Pt9Pv6zn0evPt+d4i10yd4PzJFUS5LOscKt+WWx+CHIbv+iEkVOy5N7
+TqvNdWv0hbh3Ui6zs1Nd1Qyvup0IljFD2x8ujhyvPHQvupkcLESbqh4NHCkiAOWo
+hO0+6PUt79dD9MCZ5/Ae3fm7B2ST8ai8RXW0OToI63NfeUxJn5AHeJAfAQIDAQAB
+o1MwUTAdBgNVHQ4EFgQU8A73Ay/YOz2vLvTPwfptk48pndQwHwYDVR0jBBgwFoAU
+8A73Ay/YOz2vLvTPwfptk48pndQwDwYDVR0TAQH/BAUwAwEB/zANBgkqhkiG9w0B
+AQsFAAOCAQEAnOmCHWw5UAxJJwxzEW0KRx56qmVawJ6QJCEvBLMXqZuR+kR6Sw7b
+WysDTqsD091GVSpvu76RXJLSH/BiP+HbmjPLtb5qb55XM+i7dcz9pIB505jovvC4
+t+OA/JZtx/8OmtIhhF1Se2n6gj8dG1H0tuaKbW3E95K7pC59yyW0zKP08ensy2QD
+MfggkSRenn4VoA91+jRMylnawn4jIUlWyvUsvturSVz2WP7NmlYTnlCcifyBuYqq
+IQ1XIX6F1jjody+3I+8b2tBpaPuNXDAtfoEoUWZW0ToTfAi+6Li7IMjXRZ6wPVxU
+aoKJ9jBURYeYzd/Zi2RPLpjt8TYPir8vKQ==
 -----END CERTIFICATE-----
+
 """.encode(
                 "utf-8"
             )
         )
         tmpf.flush()
         yield tmpf.name
```

### Comparing `pubtools_sign-0.0.5/tests/conftest_cosignsig.py` & `pubtools_sign-0.0.6/tests/conftest_cosignsig.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/tests/conftest_msgsig.py` & `pubtools_sign-0.0.6/tests/conftest_msgsig.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,30 +7,59 @@
 @fixture
 def f_msg_signer(f_config_msg_signer_ok):
     with patch("pubtools.sign.signers.msgsigner.MsgSigner") as msgsigner:
         yield msgsigner
 
 
 @fixture
-def f_config_msg_signer_ok(f_client_certificate):
+def f_config_msg_signer_ok(f_client_certificate, f_ca_certificate):
     with tempfile.NamedTemporaryFile() as tmpf:
         tmpf.write(
             f"""
 msg_signer:
   messaging_brokers:
     - amqps://broker-01:5671
     - amqps://broker-02:5671
   messaging_cert_key: {f_client_certificate}
-  messaging_ca_cert: ~/messaging/ca-cert.crt
+  messaging_ca_cert: {f_ca_certificate}
   topic_send_to: topic://Topic.sign
   topic_listen_to: queue://Consumer.{{creator}}.{{task_id}}.Topic.sign.{{task_id}}
   environment: prod
   service: pubtools-sign
   timeout: 1
   retries: 3
+  send_retries: 2
+  message_id_key: request_id
+  log_level: debug
+        """.encode(
+                "utf-8"
+            )
+        )
+        tmpf.flush()
+        yield tmpf.name
+
+
+@fixture
+def f_config_msg_signer_ok2(f_client_certificate, f_ca_certificate, f_qpid_broker):
+    qpid_broker, port = f_qpid_broker
+    with tempfile.NamedTemporaryFile() as tmpf:
+        tmpf.write(
+            f"""
+msg_signer:
+  messaging_brokers:
+    - localhost:{port}
+  messaging_cert_key: {f_client_certificate}
+  messaging_ca_cert: {f_ca_certificate}
+  topic_send_to: topic://Topic.sign
+  topic_listen_to: queue://Consumer.{{creator}}.{{task_id}}.Topic.sign.{{task_id}}
+  environment: prod
+  service: pubtools-sign
+  timeout: 2
+  retries: 2
+  send_retries: 2
   message_id_key: request_id
   log_level: debug
         """.encode(
                 "utf-8"
             )
         )
         tmpf.flush()
@@ -50,14 +79,15 @@
   messaging_ca_cert: ~/messaging/ca-cert.crt
   topic_send_to: topic://Topic.sign
   topic_listen_to: queue://Consumer.{{creator}}.{{task_id}}.Topic.sign.{{task_id}}
   environment: prod
   service: pubtools-sign
   timeout: 1
   retries: 3
+  send_retries: 2
   message_id_key: request_id
   log_level: debug
   key_aliases:
     beta: abcde1245
         """.encode(
                 "utf-8"
             )
```

### Comparing `pubtools_sign-0.0.5/tests/test_ansible_clearsign.py` & `pubtools_sign-0.0.6/tests/test_ansible_clearsign.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/tests/test_bundle.py` & `pubtools_sign-0.0.6/tests/test_bundle.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,16 +18,14 @@
             "test-signing-key",
             "--digest",
             "some-digest",
             "--reference",
             "some-reference",
             "--task-id",
             "1",
-            "--repo",
-            "repo",
             "--config-file",
             f_config_msg_signer_ok,
         ],
     )
     assert result.exit_code == 0, result.output
 
 
@@ -42,15 +40,13 @@
         cli,
         [
             "msg-clear-sign",
             "--signing-key",
             "test-signing-key",
             "--task-id",
             "1",
-            "--repo",
-            "repo",
             "--config-file",
             f_config_msg_signer_ok,
             "hello world",
         ],
     )
     assert result.exit_code == 0, result.output
```

### Comparing `pubtools_sign-0.0.5/tests/test_config.py` & `pubtools_sign-0.0.6/tests/test_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import pytest
 import piny
 
 from pubtools.sign.conf.conf import load_config
 
 
-def test_load_config_radas_ok(f_config_msg_signer_ok, f_client_certificate):
+def test_load_config_radas_ok(f_config_msg_signer_ok, f_client_certificate, f_ca_certificate):
     assert load_config(f_config_msg_signer_ok) == {
         "msg_signer": {
             "messaging_brokers": ["amqps://broker-01:5671", "amqps://broker-02:5671"],
             "messaging_cert_key": f_client_certificate,
-            "messaging_ca_cert": "~/messaging/ca-cert.crt",
+            "messaging_ca_cert": f_ca_certificate,
             "topic_send_to": "topic://Topic.sign",
             "topic_listen_to": "queue://Consumer.{creator}.{task_id}.Topic.sign.{task_id}",
             "environment": "prod",
             "service": "pubtools-sign",
             "timeout": 1,
             "retries": 3,
+            "send_retries": 2,
             "message_id_key": "request_id",
             "log_level": "debug",
         }
     }
 
 
 def test_load_config_missing(f_config_msg_signer_missing):
```

### Comparing `pubtools_sign-0.0.5/tests/test_cosign_signer.py` & `pubtools_sign-0.0.6/tests/test_cosign_signer.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,14 @@
     signer = CosignSigner()
     signer.load_config(load_config(f_config_cosign_signer_ok))
     container_sign_operation = ContainerSignOperation(
         digests=("some-digest",),
         references=("some-reference",),
         signing_key="test-signing-key",
         task_id="",
-        repo="r",
     )
     with patch(
         "pubtools.sign.signers.cosignsigner.CosignSigner.container_sign"
     ) as patched_container_sign:
         signer.sign(container_sign_operation)
         patched_container_sign.assert_called_once()
         with pytest.raises(UnsupportedOperation):
@@ -189,15 +188,14 @@
 
 def test_container_sign(f_config_cosign_signer_ok, f_environ, f_expected_cosign_sign_args):
     container_sign_operation = ContainerSignOperation(
         task_id="",
         digests=["sha256:abcdefg"],
         references=["some-registry/namespace/repo:tag"],
         signing_key="test-signing-key",
-        repo="",
     )
 
     with patch("subprocess.Popen") as patched_popen:
         patched_popen().returncode = 0
         patched_popen().communicate.return_value = ("stdout", "stderr")
 
         signer = CosignSigner()
@@ -228,15 +226,14 @@
 
 def test_container_sign_alias(f_config_cosign_signer_aliases, f_environ):
     container_sign_operation = ContainerSignOperation(
         task_id="",
         digests=["sha256:abcdefg"],
         references=["some-registry/namespace/repo:tag"],
         signing_key="beta",
-        repo="",
     )
 
     with patch("subprocess.Popen") as patched_popen:
         patched_popen().returncode = 0
         patched_popen().communicate.return_value = ("stdout", "stderr")
 
         signer = CosignSigner()
@@ -283,15 +280,14 @@
 
 def test_container_sign_error(f_config_cosign_signer_ok, f_environ, f_expected_cosign_sign_args):
     container_sign_operation = ContainerSignOperation(
         task_id="",
         digests=["sha256:abcdefg"],
         references=["some-registry/namespace/repo:tag"],
         signing_key="test-signing-key",
-        repo="",
     )
 
     with patch("subprocess.Popen") as patched_popen:
         patched_popen().returncode = 1
         patched_popen().communicate.return_value = ("stdout", "stderr")
 
         signer = CosignSigner()
@@ -309,30 +305,29 @@
                 )
             ]
         )
 
         assert res == SigningResults(
             signer=signer,
             operation=container_sign_operation,
-            signer_results=CosignSignerResults(status="failed", error_message=""),
+            signer_results=CosignSignerResults(status="failed", error_message="stderr"),
             operation_result=ContainerSignResult(
                 results=["stderr"], signing_key="test-signing-key", failed=True
             ),
         )
 
 
 def test_container_sign_digests_only(
     f_config_cosign_signer_ok, f_environ, f_expected_cosign_sign_args
 ):
     container_sign_operation = ContainerSignOperation(
         task_id="",
         digests=["some-registry/namespace/repo@sha256:abcdefg"],
         references=[],
         signing_key="test-signing-key",
-        repo="",
     )
 
     with patch("subprocess.Popen") as patched_popen:
         patched_popen().returncode = 0
         patched_popen().communicate.return_value = ("stdout", "stderr")
 
         signer = CosignSigner()
@@ -381,15 +376,14 @@
 
 def test_container_sign_mismatch_refs(f_config_cosign_signer_ok):
     container_sign_operation = ContainerSignOperation(
         task_id="",
         digests=["sha256:abcdefg"],
         references=["some-registry/namespace/repo:tag1", "some-registry/namespace/repo:tag2"],
         signing_key="test-signing-key",
-        repo="",
     )
 
     with patch("subprocess.Popen") as patched_popen:
         signer = CosignSigner()
         signer.load_config(load_config(f_config_cosign_signer_ok))
         with pytest.raises(ValueError):
             signer.container_sign(container_sign_operation)
```

### Comparing `pubtools_sign-0.0.5/tests/test_msg_handle.py` & `pubtools_sign-0.0.6/tests/test_msg_handle.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/tests/test_msg_recv_client.py` & `pubtools_sign-0.0.6/tests/test_msg_recv_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,24 +13,27 @@
     f_fake_msgsigner,
     f_msgsigner_send_to_queue,
     f_client_certificate,
     f_ca_certificate,
 ):
     qpid_broker, port = f_qpid_broker
     errors = []
+    received = {}
     rc = RecvClient(
+        "uid-1",
         f_msgsigner_send_to_queue,
         [],
         [f"localhost:{port}"],
         "request_id",
         f_client_certificate,
         f_ca_certificate,
         1.0,
         1,
         errors,
+        received,
     )
     rc.run()
     msgsigner, _, received_messages = f_fake_msgsigner
     assert [x.body for x in msgsigner.received_messages] == []
 
 
 def test_recv_client_recv_message(
@@ -45,24 +48,27 @@
         headers={"mtype": "test"},
         address=f_msgsigner_listen_to_topic,
         body={"msg": {"message": "test_message", "request_id": "1"}},
     )
 
     sender = SendClient([message], [f"localhost:{port}"], "", "", 10, [])
     errors = []
+    received = {}
     receiver = RecvClient(
+        "uid-1",
         f_msgsigner_send_to_queue,
         ["1"],
         "request_id",
         [f"localhost:{port}"],
         "",
         "",
         60.0,
         2,
         errors,
+        received,
     )
 
     tsc = Thread(target=sender.run, args=())
     trc = Thread(target=receiver.run, args=())
 
     trc.start()
     tsc.start()
@@ -89,25 +95,28 @@
     qpid_broker, port = f_qpid_broker
     message = MsgMessage(
         headers={"mtype": "test"},
         address=f_msgsigner_listen_to_topic,
         body={"msg": {"message": "test_message", "request_id": "1"}},
     )
     errors = []
+    received = {}
     sender = SendClient([message], [f"localhost:{port}"], "", "", 10, [])
     receiver = RecvClient(
+        "uid-1",
         f_msgsigner_send_to_queue + "_wrong",
         ["1"],
         "request_id",
         [f"localhost:{port}"],
         "",
         "",
         10.0,
         1,
         errors,
+        received,
     )
 
     tsc = Thread(target=sender.run, args=())
     trc = Thread(target=receiver.run, args=())
 
     trc.start()
     tsc.start()
@@ -122,24 +131,27 @@
     f_qpid_broker,
     f_msgsigner_listen_to_topic,
     f_fake_msgsigner,
     f_msgsigner_send_to_queue,
 ):
     qpid_broker, port = f_qpid_broker
     errors = []
+    received = {}
     receiver = RecvClient(
+        "uid-1",
         f_msgsigner_send_to_queue,
         ["1"],
         "request_id",
         [f"localhost:{port+1}"],
         "",
         "",
         10.0,
         1,
         errors,
+        received,
     )
 
     trc = Thread(target=receiver.run, args=())
 
     trc.start()
 
     time.sleep(1)
@@ -157,24 +169,27 @@
     message = MsgMessage(
         headers={"mtype": "test"},
         address=f_msgsigner_listen_to_topic,
         body={"msg": {"message": "test_message", "request_id": "1"}},
     )
     sender = SendClient([message], [f"localhostx:{port}"], "", "", 10, [])
     errors = []
+    received = {}
     receiver = RecvClient(
+        "uid-1",
         f_msgsigner_send_to_queue,
         ["1"],
         "request_id",
         [f"localhost:{port}"],
         "",
         "",
         10.0,
         1,
         errors,
+        received,
     )
 
     tsc = Thread(target=sender.run, args=())
     trc = Thread(target=receiver.run, args=())
 
     trc.start()
     tsc.start()
@@ -191,47 +206,102 @@
 ):
     qpid_broker, port = f_qpid_broker
     message = MsgMessage(
         headers={"mtype": "test"},
         address=f_msgsigner_listen_to_topic,
         body={"msg": {"message": "test_message", "request_id": "1"}},
     )
-    sender = SendClient([message], [f"localhostx:{port}"], "", "", 10, [])
+    sender = SendClient([message], [f"localhost:{port}"], "", "", 10, [])
     errors = []
+    received = {}
 
+    print(id(errors))
     on_message_original = _RecvClient.on_message
     with patch(
         "pubtools.sign.clients.msg_recv_client._RecvClient.on_message", autospec=True
     ) as patched_on_message:
         patched_on_message.side_effect = lambda self, event: [
             self.errors.append("1"),
             on_message_original(self, event),
         ]
 
         receiver = RecvClient(
+            "uid-1",
             f_msgsigner_send_to_queue,
             ["1"],
             "request_id",
             [f"localhost:{port}"],
             "",
             "",
             10.0,
             1,
             errors,
+            received,
         )
 
         tsc = Thread(target=sender.run, args=())
         trc = Thread(target=receiver.run, args=())
 
         trc.start()
         tsc.start()
-        time.sleep(1)
+        # time.sleep(1)
+        trc.join()
         assert len(errors) == 1
 
 
+def test_recv_client_timeout_recv_in_time(
+    f_cleanup_msgsigner_messages,
+    f_qpid_broker,
+    f_msgsigner_listen_to_topic,
+    f_fake_msgsigner,
+    f_msgsigner_send_to_queue,
+):
+    qpid_broker, port = f_qpid_broker
+    message = MsgMessage(
+        headers={"mtype": "test"},
+        address=f_msgsigner_listen_to_topic,
+        body={"msg": {"message": "test_message", "request_id": "1"}},
+    )
+    message2 = MsgMessage(
+        headers={"mtype": "test"},
+        address=f_msgsigner_listen_to_topic,
+        body={"msg": {"message": "test_message", "request_id": "2"}},
+    )
+    sender = SendClient([message, message2], [f"localhost:{port}"], "", "", 10, [], prefetch=1)
+    errors = []
+    received = {}
+
+    # on_message_original = _RecvClient.on_message
+    receiver = RecvClient(
+        "uid-1",
+        f_msgsigner_send_to_queue,
+        ["1", "2"],
+        "request_id",
+        [f"localhost:{port}"],
+        "",
+        "",
+        8,
+        1,
+        errors,
+        received,
+    )
+
+    sender.handler.handlers[0].on_start(Mock())
+    receiver._handler.on_start(Mock())
+    sender.handler.handlers[0].on_sendable(Mock())
+    receiver._handler.on_message(
+        Mock(message=Mock(body='{"msg":{"message":"test_message","request_id":"2"}}'))
+    )
+    receiver._handler.on_timer_task(Mock())
+    receiver._handler.on_message(
+        Mock(message=Mock(body='{"msg":{"message":"test_message","request_id":"2"}}'))
+    )
+    assert receiver.errors == []
+
+
 def test_recv_client_recv_message_stray(
     f_cleanup_msgsigner_messages,
     f_qpid_broker,
     f_msgsigner_listen_to_topic_stray,
     f_msgsigner_send_to_queue_stray,
     f_fake_msgsigner_stray,
 ):
@@ -240,24 +310,27 @@
         headers={"mtype": "test"},
         address=f_msgsigner_listen_to_topic_stray,
         body={"msg": {"message": "test_message", "request_id": "1"}},
     )
 
     sender = SendClient([message], [f"localhost:{port}"], "", "", 10, [])
     errors = []
+    received = {}
     receiver = RecvClient(
+        "uid-1",
         f_msgsigner_send_to_queue_stray,
         ["1"],
         "request_id",
         [f"localhost:{port}"],
         "",
         "",
         60.0,
         2,
         errors,
+        received,
     )
 
     tsc = Thread(target=sender.run, args=())
     trc = Thread(target=receiver.run, args=())
 
     trc.start()
     tsc.start()
@@ -293,24 +366,27 @@
         patched_on_sendable.side_effect = lambda self, event: [
             on_sendable_original(self, event),
             time.sleep(10),
         ]
 
         sender = SendClient([message], [f"localhost:{port}"], "", "", 10, [])
         errors = []
+        received = {}
         receiver = RecvClient(
+            "uid-1",
             f_msgsigner_send_to_queue,
             ["1"],
             "request_id",
             [f"localhost:{port}"],
             "",
             "",
             1.0,
             2,
             errors,
+            received,
         )
 
         tsc = Thread(target=sender.run, args=())
         trc = Thread(target=receiver.run, args=())
 
         trc.start()
         tsc.start()
@@ -377,30 +453,66 @@
             setattr(self, "conn", Mock()),
             setattr(self, "receiver", Mock()),
             time.sleep(1),
         ]
 
         sender = SendClient([message], [f"localhost:{port}"], "", "", 10, [])
         errors = []
+        received = {}
         receiver = RecvClient(
+            "uid-1",
             f_msgsigner_send_to_queue,
             ["1"],
             "request_id",
             [f"localhost:{port}"],
             "",
             "",
             1.0,
             2,
             errors,
+            received,
         )
 
         tsc = Thread(target=sender.run, args=())
         rcvt = RecvThread(recv=receiver)
 
         rcvt.start()
         tsc.start()
         sender.stop()
         rcvt.stop()
         time.sleep(1)
 
         tsc.join()
         rcvt.join()
+
+
+def test_recv_client_close_method(f_msgsigner_send_to_queue, f_qpid_broker):
+    qpid_broker, port = f_qpid_broker
+    errors = []
+    received = {}
+    with patch(
+        "pubtools.sign.clients.msg_recv_client._RecvClient.on_start", autospec=True
+    ) as patched_on_start:
+        patched_on_start.side_effect = lambda self, event: [
+            setattr(self, "timer_task", Mock()),
+            setattr(self, "conn", Mock()),
+            setattr(self, "receiver", Mock()),
+            time.sleep(1),
+        ]
+        receiver = RecvClient(
+            "uid-1",
+            f_msgsigner_send_to_queue,
+            ["1"],
+            "request_id",
+            [f"localhost:{port}"],
+            "",
+            "",
+            1.0,
+            2,
+            errors,
+            received,
+        )
+        receiver.handler.on_start(Mock())
+        receiver.close()
+        receiver.handler.timer_task.cancel.assert_called_once()
+        receiver.handler.receiver.close.assert_called_once()
+        receiver.handler.conn.close.assert_called_once()
```

### Comparing `pubtools_sign-0.0.5/tests/test_msg_send_client.py` & `pubtools_sign-0.0.6/tests/test_msg_send_client.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/tests/test_msg_signer.py` & `pubtools_sign-0.0.6/tests/test_msg_signer.py`

 * *Files 16% similar despite different names*

```diff
@@ -396,15 +396,15 @@
     with patch("uuid.uuid4", return_value="1234-5678-abcd-efgh"):
         with patch("pubtools.sign.signers.msgsigner.isodate_now") as patched_date:
             patched_date.return_value = "created-date-Z"
             operation = ClearSignOperation(
                 inputs=["test-data-inputs"], signing_key="test-key", task_id="1", repo="repo"
             )
             assert signer._create_msg_message(
-                data, operation, SignRequestType.CONTAINER
+                data, "repo", operation, SignRequestType.CONTAINER
             ) == MsgMessage(
                 headers={
                     "service": "pubtools-sign",
                     "environment": "prod",
                     "owner_id": "pubtools-sign-test",
                     "mtype": SignRequestType.CONTAINER,
                     "source": "metadata",
@@ -416,15 +416,15 @@
                     "request_id": "1234-5678-abcd-efgh",
                     "created": "created-date-Z",
                     "requested_by": "pubtools-sign-test",
                     "repo": "repo",
                 },
             )
             assert signer._create_msg_message(
-                data, operation, SignRequestType.CLEARSIGN
+                data, "repo", operation, SignRequestType.CLEARSIGN
             ) == MsgMessage(
                 headers={
                     "service": "pubtools-sign",
                     "environment": "prod",
                     "owner_id": "pubtools-sign-test",
                     "mtype": SignRequestType.CLEARSIGN,
                     "source": "metadata",
@@ -445,15 +445,14 @@
     signer = MsgSigner()
     signer.load_config(load_config(f_config_msg_signer_ok))
     container_sign_operation = ContainerSignOperation(
         digests=("some-digest",),
         references=("some-reference",),
         signing_key="test-signing-key",
         task_id="1",
-        repo="repo",
     )
     clear_sign_operation = ClearSignOperation(
         inputs=["hello world"], signing_key="test-signing-key", task_id="1", repo="repo"
     )
 
     with patch("pubtools.sign.signers.msgsigner.MsgSigner.clear_sign") as patched_clear_sign:
         with patch(
@@ -534,15 +533,15 @@
                 patch_construct_signing_message.return_value = {
                     "request_id": "1234-5678-abcd-efgh",
                 }
                 res = signer.clear_sign(clear_sign_operation)
                 patch_construct_signing_message.assert_called_once_with(
                     "aGVsbG8gd29ybGQ=",
                     "abcde1245",
-                    repo="repo",
+                    "repo",
                     extra_attrs={"pub_task_id": "1"},
                     sig_type="clearsign_signature",
                 )
 
             assert res == SigningResults(
                 signer=signer,
                 operation=clear_sign_operation,
@@ -609,46 +608,47 @@
                     status="error", error_message="TestError : test error description\n"
                 ),
                 operation_result=ClearSignResult(outputs=[""], signing_key="test-signing-key"),
             )
 
 
 @patch("uuid.uuid4", return_value="1234-5678-abcd-efgh")
-def test_container_sign(patched_uuid, f_config_msg_signer_ok, f_client_certificate):
+def test_container_sign(
+    patched_uuid, f_config_msg_signer_ok, f_client_certificate, f_ca_certificate
+):
     container_sign_operation = ContainerSignOperation(
         task_id="1",
         digests=["sha256:abcdefg"],
         references=["some-registry/namespace/repo:tag"],
         signing_key="test-signing-key",
-        repo="repo",
     )
 
     with patch("pubtools.sign.signers.msgsigner.SendClient") as patched_send_client:
         with patch("pubtools.sign.signers.msgsigner.RecvClient") as patched_recv_client:
             patched_send_client.return_value.run.return_value = []
             patched_recv_client.return_value.run.return_value = []
             patched_recv_client.return_value.recv = {
                 "1234-5678-abcd-efgh": (
                     {"msg": {"errors": [], "signed_claim": "signed:'claim'"}},
                     {"fake": "headers"},
                 )
             }
-            patched_recv_client.return_value._errors = []
+            patched_recv_client.return_value.get_errors.return_value = []
 
             signer = MsgSigner()
             signer.load_config(load_config(f_config_msg_signer_ok))
             res = signer.container_sign(container_sign_operation)
 
             patched_send_client.assert_called_with(
                 messages=[ANY],
                 broker_urls=["amqps://broker-01:5671", "amqps://broker-02:5671"],
                 cert=f_client_certificate,
-                ca_cert=os.path.expanduser("~/messaging/ca-cert.crt"),
+                ca_cert=f_ca_certificate,
                 retries=3,
-                errors=[],
+                errors=patched_recv_client.return_value.get_errors.return_value,
             )
 
             assert res == SigningResults(
                 signer=signer,
                 operation=container_sign_operation,
                 signer_results=MsgSignerResults(status="ok", error_message=""),
                 operation_result=ContainerSignResult(
@@ -667,54 +667,53 @@
 @patch("uuid.uuid4", return_value="1234-5678-abcd-efgh")
 def test_container_sign_alias(patched_uuid, f_config_msg_signer_aliases, f_client_certificate):
     container_sign_operation = ContainerSignOperation(
         task_id="1",
         digests=["sha256:abcdefg"],
         references=["some-registry/namespace/repo:tag"],
         signing_key="beta",
-        repo="repo",
     )
 
     with patch("pubtools.sign.signers.msgsigner.SendClient") as patched_send_client:
         with patch("pubtools.sign.signers.msgsigner.RecvClient") as patched_recv_client:
             patched_send_client.return_value.run.return_value = []
             patched_recv_client.return_value.run.return_value = []
             patched_recv_client.return_value.recv = {
                 "1234-5678-abcd-efgh": (
                     {"msg": {"errors": [], "signed_claim": "signed:'claim'"}},
                     {"fake": "headers"},
                 )
             }
-            patched_recv_client.return_value._errors = []
+            patched_recv_client.return_value.get_errors.return_value = []
 
             signer = MsgSigner()
             signer.load_config(load_config(f_config_msg_signer_aliases))
 
             with patch(
                 "pubtools.sign.signers.msgsigner.MsgSigner._construct_signing_message"
             ) as patch_construct_signing_message:
                 patch_construct_signing_message.return_value = {
                     "request_id": "1234-5678-abcd-efgh",
                 }
                 res = signer.container_sign(container_sign_operation)
                 patch_construct_signing_message.assert_called_once_with(
                     ANY,
                     "abcde1245",
-                    repo="repo",
+                    "namespace/repo",
                     extra_attrs={"pub_task_id": "1", "manifest_digest": "sha256:abcdefg"},
                     sig_type="container_signature",
                 )
 
             patched_send_client.assert_called_with(
                 messages=[ANY],
                 broker_urls=["amqps://broker-01:5671", "amqps://broker-02:5671"],
                 cert=f_client_certificate,
                 ca_cert=os.path.expanduser("~/messaging/ca-cert.crt"),
                 retries=3,
-                errors=[],
+                errors=patched_recv_client.return_value.get_errors.return_value,
             )
 
             assert res == SigningResults(
                 signer=signer,
                 operation=container_sign_operation,
                 signer_results=MsgSignerResults(status="ok", error_message=""),
                 operation_result=ContainerSignResult(
@@ -733,21 +732,20 @@
 @patch("uuid.uuid4", return_value="1234-5678-abcd-efgh")
 def test_container_sign_recv_errors(patched_uuid, f_config_msg_signer_ok):
     container_sign_operation = ContainerSignOperation(
         task_id="1",
         digests=["sha256:abcdefg"],
         references=["some-registry/namespace/repo:tag"],
         signing_key="test-signing-key",
-        repo="repo",
     )
 
     with patch("pubtools.sign.signers.msgsigner.SendClient") as patched_send_client:
         with patch("pubtools.sign.signers.msgsigner.RecvClient") as patched_recv_client:
             patched_send_client.return_value.run.return_value = []
-            patched_recv_client.return_value._errors = [
+            patched_recv_client.return_value.get_errors.return_value = [
                 MsgError(
                     name="TestError", description="test error description", source="test-source"
                 )
             ]
             patched_recv_client.return_value.recv = {"1234-5678-abcd-efgh": "signed:'hello world'"}
 
             signer = MsgSigner()
@@ -769,15 +767,14 @@
 @patch("uuid.uuid4", return_value="1234-5678-abcd-efgh")
 def test_container_sign_send_errors(patched_uuid, f_config_msg_signer_ok):
     container_sign_operation = ContainerSignOperation(
         task_id="1",
         digests=["sha256:abcdefg"],
         references=["some-registry/namespace/repo:tag"],
         signing_key="test-signing-key",
-        repo="repo",
     )
     with patch("pubtools.sign.signers.msgsigner.SendClient") as patched_send_client:
         with patch("pubtools.sign.signers.msgsigner.RecvClient") as patched_recv_client:
             patched_send_client.return_value.run.return_value = [
                 MsgError(
                     name="TestError", description="test error description", source="test-source"
                 )
@@ -804,38 +801,263 @@
 @patch("uuid.uuid4", return_value="1234-5678-abcd-efgh")
 def test_container_sign_wrong_inputs(patched_uuid, f_config_msg_signer_ok):
     container_sign_operation = ContainerSignOperation(
         task_id="1",
         digests=["sha256:abcdefg"],
         references=["some-registry/namespace/repo:tag", "some-registry/namespace/repo:tag2"],
         signing_key="test-signing-key",
-        repo="repo",
     )
 
     signer = MsgSigner()
     signer.load_config(load_config(f_config_msg_signer_ok))
     with pytest.raises(ValueError):
         signer.container_sign(container_sign_operation)
 
 
+@patch("uuid.uuid4", return_value="1234-5678-abcd-efgh")
+def test_container_sign_recv_timeout_fails(patched_uuid, f_config_msg_signer_ok):
+    container_sign_operation = ContainerSignOperation(
+        task_id="1",
+        digests=["sha256:abcdefg"],
+        references=["some-registry/namespace/repo:tag"],
+        signing_key="test-signing-key",
+    )
+
+    with patch("pubtools.sign.signers.msgsigner.SendClient") as patched_send_client:
+        with patch("pubtools.sign.signers.msgsigner.RecvClient") as patched_recv_client:
+            patched_send_client.return_value.run.return_value = []
+            patched_recv_client.return_value.get_errors.return_value = [
+                MsgError(
+                    name="MessagingTimeout",
+                    description="Out of time when receiving messages",
+                    source="test-source",
+                ),
+                MsgError(
+                    name="MessagingTimeout",
+                    description="Out of time when receiving messages",
+                    source="test-source",
+                ),
+                MsgError(
+                    name="MessagingTimeout",
+                    description="Out of time when receiving messages",
+                    source="test-source",
+                ),
+            ]
+            patched_recv_client.return_value.recv = {
+                "1234-5678-abcd-efgh": (
+                    {"msg": {"errors": [], "signed_claim": "signed:'claim'"}},
+                    {"fake": "headers"},
+                )
+            }
+
+            signer = MsgSigner()
+            signer.load_config(load_config(f_config_msg_signer_ok))
+            signer.retries = 2
+            signer.send_retries = 1
+
+            res = signer.container_sign(container_sign_operation)
+
+            assert res == SigningResults(
+                signer=signer,
+                operation=container_sign_operation,
+                signer_results=MsgSignerResults(
+                    status="error",
+                    error_message="MessagingTimeout : Out of time when receiving messages\n"
+                    "MessagingTimeout : Out of time when receiving messages\n",
+                ),
+                operation_result=ContainerSignResult(
+                    results=[""], signing_key="test-signing-key", failed=False
+                ),
+            )
+
+
+@patch("uuid.uuid4", return_value="1234-5678-abcd-efgh")
+def test_container_sign_recv_timeout_ok(patched_uuid, f_config_msg_signer_ok):
+    container_sign_operation = ContainerSignOperation(
+        task_id="1",
+        digests=["sha256:abcdefg"],
+        references=["some-registry/namespace/repo:tag"],
+        signing_key="test-signing-key",
+    )
+
+    with patch("pubtools.sign.signers.msgsigner.SendClient") as patched_send_client:
+        with patch("pubtools.sign.signers.msgsigner.RecvClient") as patched_recv_client:
+            patched_send_client.return_value.run.return_value = []
+            patched_recv_client.return_value.get_errors.return_value = [
+                MsgError(
+                    name="MessagingTimeout",
+                    description="Out of time when receiving messages",
+                    source="test-source",
+                ),
+            ]
+            patched_recv_client.return_value.recv = {
+                "1234-5678-abcd-efgh": (
+                    {"msg": {"errors": [], "signed_claim": "signed:'claim'"}},
+                    {"fake": "headers"},
+                )
+            }
+
+            signer = MsgSigner()
+            signer.retries = 2
+            signer.send_retries = 1
+
+            signer.load_config(load_config(f_config_msg_signer_ok))
+            res = signer.container_sign(container_sign_operation)
+
+            assert res == SigningResults(
+                signer=signer,
+                operation=container_sign_operation,
+                signer_results=MsgSignerResults(
+                    status="ok",
+                    error_message="",
+                ),
+                operation_result=ContainerSignResult(
+                    results=[
+                        (
+                            {"msg": {"errors": [], "signed_claim": "signed:'claim'"}},
+                            {"fake": "headers"},
+                        )
+                    ],
+                    signing_key="test-signing-key",
+                    failed=False,
+                ),
+            )
+
+
+@patch("uuid.uuid4", return_value="1234-5678-abcd-efgh")
+def test_clear_sign_recv_timeout(patched_uuid, f_config_msg_signer_ok):
+    clear_sign_operation = ClearSignOperation(
+        inputs=["hello world"], signing_key="test-signing-key", task_id="1", repo="repo"
+    )
+
+    with patch("pubtools.sign.signers.msgsigner.SendClient") as patched_send_client:
+        with patch("pubtools.sign.signers.msgsigner.RecvClient") as patched_recv_client:
+            patched_send_client.return_value.run.return_value = []
+            patched_recv_client.return_value._errors = [
+                MsgError(
+                    name="MessagingTimeout",
+                    description="Out of time when receiving messages",
+                    source="test-source",
+                ),
+                MsgError(
+                    name="MessagingTimeout",
+                    description="Out of time when receiving messages",
+                    source="test-source",
+                ),
+                MsgError(
+                    name="MessagingTimeout",
+                    description="Out of time when receiving messages",
+                    source="test-source",
+                ),
+            ]
+            patched_recv_client.return_value.recv = {"1234-5678-abcd-efgh": "signed:'hello world'"}
+
+            signer = MsgSigner()
+            signer.load_config(load_config(f_config_msg_signer_ok))
+            signer.retries = 2
+            signer.send_retries = 1
+
+            res = signer.clear_sign(clear_sign_operation)
+
+            assert res == SigningResults(
+                signer=signer,
+                operation=clear_sign_operation,
+                signer_results=MsgSignerResults(
+                    status="error",
+                    error_message="MessagingTimeout : Out of time when receiving messages\n"
+                    "MessagingTimeout : Out of time when receiving messages\n",
+                ),
+                operation_result=ClearSignResult(outputs=[""], signing_key="test-signing-key"),
+            )
+
+
+def test_recv_client_recv_message_break(
+    f_cleanup_msgsigner_messages,
+    f_qpid_broker,
+    f_msgsigner_listen_to_topic,
+    f_fake_msgsigner,
+    f_msgsigner_send_to_queue,
+    f_client_certificate,
+    f_ca_certificate,
+    f_config_msg_signer_ok2,
+):
+    qpid_broker, port = f_qpid_broker
+    container_sign_operation = ContainerSignOperation(
+        digests=("some-digest",),
+        references=("some/reference:some-tag",),
+        signing_key="test-signing-key",
+        task_id="1",
+    )
+    with patch(
+        "pubtools.sign.clients.msg_recv_client.RecvClient.get_errors", autospec=True
+    ) as patched_recv_get_errors, patch(
+        "pubtools.sign.clients.msg_recv_client.RecvClient.get_received", autospec=True
+    ) as patched_recv_get_received, patch(
+        "uuid.uuid4", return_value="1234-5678-abcd-efgh"
+    ) as _:
+        patched_recv_get_errors.side_effect = [
+            [
+                MsgError(
+                    name="MessagingTimeout",
+                    description="Out of time when receiving messages",
+                    source=ANY,
+                )
+            ],
+            [
+                MsgError(
+                    name="MessagingTimeout",
+                    description="Out of time when receiving messages",
+                    source=ANY,
+                )
+            ],
+            [
+                MsgError(
+                    name="MessagingTimeout",
+                    description="Out of time when receiving messages",
+                    source=ANY,
+                )
+            ],
+            [],
+        ]
+        patched_recv_get_received.side_effect = [{"1234-5678-abcd-efgh": True}]
+        signer = MsgSigner()
+        signer.load_config(load_config(f_config_msg_signer_ok2))
+        signer.retries = 2
+        signer.send_retries = 1
+        res = signer.container_sign(container_sign_operation)
+
+        assert res == SigningResults(
+            signer=signer,
+            operation=container_sign_operation,
+            signer_results=MsgSignerResults(
+                status="error",
+                error_message="MessagingTimeout : Out of time when receiving messages\n",
+            ),
+            operation_result=ContainerSignResult(
+                results=[""], signing_key="test-signing-key", failed=False
+            ),
+        )
+
+
 def test_msgsig_doc_arguments():
     assert MsgSigner.doc_arguments() == {
         "options": {
             "messaging_brokers": {"description": "List of brokers URLS"},
             "messaging_cert_key": {
                 "description": "Client certificate + key for messaging authorization"
             },
             "messaging_ca_cert": {"description": "Messaging CA certificate"},
             "topic_send_to": {"description": "Topic where to send the messages"},
             "topic_listen_to": {"description": "Topic where to listen for replies"},
             "creator": {"description": "Identification of creator of signing request"},
             "environment": {"description": "Environment indetification in sent messages"},
             "service": {"description": "Service identificator"},
-            "timeout": {"description": "Timeout for messaging sent/receive"},
-            "retries": {"description": "Retries for messaging sent/receive"},
+            "timeout": {"description": "Timeout for messaging receive"},
+            "retries": {"description": "Retries for messaging receive"},
+            "send_retries": {"description": "Retries for messaging send+receive"},
             "message_id_key": {
                 "description": "Attribute name in message body which should be used as message id"
             },
             "log_level": {"description": "Log level"},
             "key_aliases": {"description": "Aliases for signing keys"},
         },
         "examples": {
@@ -847,14 +1069,15 @@
                 "topic_listen_to": "queue://Consumer.{{creator}}.{{task_id}}.Topic.sign."
                 "{{task_id}}",
                 "creator": "pubtools-sign",
                 "environment": "prod",
                 "service": "pubtools-sign",
                 "timeout": 1,
                 "retries": 3,
+                "send_retries": 2,
                 "message_id_key": "123",
                 "log_level": "debug",
                 "key_aliases": "{'production':'abcde1245'}",
             }
         },
     }
```

### Comparing `pubtools_sign-0.0.5/tests/test_registry_client.py` & `pubtools_sign-0.0.6/tests/test_registry_client.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/tests/test_results.py` & `pubtools_sign-0.0.6/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/tests/test_sign_operations.py` & `pubtools_sign-0.0.6/tests/test_sign_operations.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,26 +9,20 @@
         "options": {
             "digests": {"description": "List of digest to sign"},
             "references": {"description": "List of references to sign"},
             "signing_key": {"description": "Signing key short id which should be used for signing"},
             "task_id": {
                 "description": "Usually pub task id, serves as identifier for in signing request"
             },
-            "repo": {
-                "type": "str",
-                "description": "Repository name",
-                "required": "true",
-            },
         },
         "examples": {
             "digests": "",
             "references": "",
             "signing_key": "",
             "task_id": "",
-            "repo": "repo",
         },
     }
 
 
 def test_clearsign_operation_doc_argument():
     assert ClearSignOperation.doc_arguments() == {
         "options": {
@@ -60,21 +54,19 @@
 
 def test_container_sign_to_dict():
     assert ContainerSignOperation(
         digests=["digest"],
         references=["references"],
         signing_key="sig-key",
         task_id="task-id",
-        repo="repo",
     ).to_dict() == dict(
         digests=["digest"],
         references=["references"],
         signing_key="sig-key",
         task_id="task-id",
-        repo="repo",
     )
 
 
 def test_clear_sign_to_dict():
     assert ClearSignOperation(
         inputs=["input1"], signing_key="sig-key", task_id="task-id", repo="repo"
     ).to_dict() == dict(inputs=["input1"], signing_key="sig-key", task_id="task-id", repo="repo")
```

### Comparing `pubtools_sign-0.0.5/.gitignore` & `pubtools_sign-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/LICENSE` & `pubtools_sign-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pubtools_sign-0.0.5/pyproject.toml` & `pubtools_sign-0.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "pubtools-sign"
 description = "Collection of tools producing signed artifacts"
 readme = "README.rst"
 requires-python = ">=3.7"
-version = "0.0.5"
+version = "0.0.6"
 
 classifiers = [  # Optional
   # How mature is this project? Common values are
   #   3 - Alpha
   #   4 - Beta
   #   5 - Production/Stable
   "Development Status :: 3 - Alpha",
@@ -39,15 +39,19 @@
     "requests",
     "piny",
     "python-qpid-proton",
     "monotonic",
     "marshmallow",
     "pyOpenSSL",
     "typing_extensions",
-    "ansible-core"
+    "ansible-core",
+    "pubtools>=1.4.0",
+    "opentelemetry-api==1.20.0",
+    "opentelemetry-sdk==1.20.0",
+    "opentelemetry-exporter-otlp==1.20.0"
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]  # list of folders that contain the packages (["."] by default)
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/pubtools"]
```

### Comparing `pubtools_sign-0.0.5/PKG-INFO` & `pubtools_sign-0.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pubtools-sign
-Version: 0.0.5
+Version: 0.0.6
 Summary: Collection of tools producing signed artifacts
 Author-email: Jindrich Luza <jluza@redhat.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.7
 Requires-Dist: ansible-core
 Requires-Dist: click
 Requires-Dist: marshmallow
 Requires-Dist: monotonic
+Requires-Dist: opentelemetry-api==1.20.0
+Requires-Dist: opentelemetry-exporter-otlp==1.20.0
+Requires-Dist: opentelemetry-sdk==1.20.0
 Requires-Dist: piny
+Requires-Dist: pubtools>=1.4.0
 Requires-Dist: pyopenssl
 Requires-Dist: python-qpid-proton
 Requires-Dist: requests
 Requires-Dist: typing-extensions
 Provides-Extra: dev
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: tox; extra == 'dev'
```

