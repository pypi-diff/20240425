# Comparing `tmp/edx-enterprise-subsidy-client-0.4.2.tar.gz` & `tmp/edx-enterprise-subsidy-client-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-enterprise-subsidy-client-0.4.2.tar", last modified: Wed Mar 20 11:22:08 2024, max compression
+gzip compressed data, was "edx-enterprise-subsidy-client-0.4.3.tar", last modified: Thu Apr 25 14:55:38 2024, max compression
```

## Comparing `edx-enterprise-subsidy-client-0.4.2.tar` & `edx-enterprise-subsidy-client-0.4.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:22:08.874937 edx-enterprise-subsidy-client-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-03-20 11:21:59.000000 edx-enterprise-subsidy-client-0.4.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-20 11:21:59.000000 edx-enterprise-subsidy-client-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-03-20 11:21:59.000000 edx-enterprise-subsidy-client-0.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-20 11:21:59.000000 edx-enterprise-subsidy-client-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9495 2024-03-20 11:22:08.874937 edx-enterprise-subsidy-client-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-03-20 11:21:59.000000 edx-enterprise-subsidy-client-0.4.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:22:08.870937 edx-enterprise-subsidy-client-0.4.2/edx_enterprise_subsidy_client/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-20 11:21:59.000000 edx-enterprise-subsidy-client-0.4.2/edx_enterprise_subsidy_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-03-20 11:21:59.000000 edx-enterprise-subsidy-client-0.4.2/edx_enterprise_subsidy_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:22:08.874937 edx-enterprise-subsidy-client-0.4.2/edx_enterprise_subsidy_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9495 2024-03-20 11:22:08.000000 edx-enterprise-subsidy-client-0.4.2/edx_enterprise_subsidy_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-20 11:22:08.000000 edx-enterprise-subsidy-client-0.4.2/edx_enterprise_subsidy_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 11:22:08.000000 edx-enterprise-subsidy-client-0.4.2/edx_enterprise_subsidy_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 11:22:08.000000 edx-enterprise-subsidy-client-0.4.2/edx_enterprise_subsidy_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-20 11:22:08.000000 edx-enterprise-subsidy-client-0.4.2/edx_enterprise_subsidy_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-20 11:22:08.000000 edx-enterprise-subsidy-client-0.4.2/edx_enterprise_subsidy_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:22:08.874937 edx-enterprise-subsidy-client-0.4.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-20 11:21:59.000000 edx-enterprise-subsidy-client-0.4.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-20 11:21:59.000000 edx-enterprise-subsidy-client-0.4.2/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-20 11:22:08.874937 edx-enterprise-subsidy-client-0.4.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     5111 2024-03-20 11:21:59.000000 edx-enterprise-subsidy-client-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:22:08.874937 edx-enterprise-subsidy-client-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-03-20 11:21:59.000000 edx-enterprise-subsidy-client-0.4.2/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:55:38.125208 edx-enterprise-subsidy-client-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-25 14:55:34.000000 edx-enterprise-subsidy-client-0.4.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-25 14:55:34.000000 edx-enterprise-subsidy-client-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-04-25 14:55:34.000000 edx-enterprise-subsidy-client-0.4.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-25 14:55:34.000000 edx-enterprise-subsidy-client-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-04-25 14:55:38.125208 edx-enterprise-subsidy-client-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-04-25 14:55:34.000000 edx-enterprise-subsidy-client-0.4.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:55:38.121208 edx-enterprise-subsidy-client-0.4.3/edx_enterprise_subsidy_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-25 14:55:34.000000 edx-enterprise-subsidy-client-0.4.3/edx_enterprise_subsidy_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13212 2024-04-25 14:55:34.000000 edx-enterprise-subsidy-client-0.4.3/edx_enterprise_subsidy_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:55:38.125208 edx-enterprise-subsidy-client-0.4.3/edx_enterprise_subsidy_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-04-25 14:55:38.000000 edx-enterprise-subsidy-client-0.4.3/edx_enterprise_subsidy_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-25 14:55:38.000000 edx-enterprise-subsidy-client-0.4.3/edx_enterprise_subsidy_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:55:38.000000 edx-enterprise-subsidy-client-0.4.3/edx_enterprise_subsidy_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:55:38.000000 edx-enterprise-subsidy-client-0.4.3/edx_enterprise_subsidy_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-25 14:55:38.000000 edx-enterprise-subsidy-client-0.4.3/edx_enterprise_subsidy_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-25 14:55:38.000000 edx-enterprise-subsidy-client-0.4.3/edx_enterprise_subsidy_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:55:38.125208 edx-enterprise-subsidy-client-0.4.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-25 14:55:34.000000 edx-enterprise-subsidy-client-0.4.3/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-25 14:55:34.000000 edx-enterprise-subsidy-client-0.4.3/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-25 14:55:38.125208 edx-enterprise-subsidy-client-0.4.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5111 2024-04-25 14:55:34.000000 edx-enterprise-subsidy-client-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:55:38.125208 edx-enterprise-subsidy-client-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-25 14:55:34.000000 edx-enterprise-subsidy-client-0.4.3/tests/test_client.py
```

### Comparing `edx-enterprise-subsidy-client-0.4.2/CHANGELOG.rst` & `edx-enterprise-subsidy-client-0.4.3/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+[0.4.3]
+*******
+* feat: adding new subsidy client method to fetch subsidy aggregate data
+
 [0.4.2]
 *******
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 * Add python 3.12 support
 
 [0.4.1]
```

### Comparing `edx-enterprise-subsidy-client-0.4.2/LICENSE` & `edx-enterprise-subsidy-client-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.4.2/LICENSE.txt` & `edx-enterprise-subsidy-client-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.4.2/PKG-INFO` & `edx-enterprise-subsidy-client-0.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-subsidy-client
-Version: 0.4.2
+Version: 0.4.3
 Summary: Client for interacting with the enterprise-subsidy service.
 Home-page: https://github.com/openedx/edx-enterprise-subsidy-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -221,14 +221,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+[0.4.3]
+*******
+* feat: adding new subsidy client method to fetch subsidy aggregate data
+
 [0.4.2]
 *******
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 * Add python 3.12 support
 
 [0.4.1]
```

### Comparing `edx-enterprise-subsidy-client-0.4.2/README.rst` & `edx-enterprise-subsidy-client-0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.4.2/edx_enterprise_subsidy_client/client.py` & `edx-enterprise-subsidy-client-0.4.3/edx_enterprise_subsidy_client/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -69,14 +69,49 @@
         """
         self.client = OAuthAPIClient(
             settings.OAUTH2_PROVIDER_URL,
             settings.BACKEND_SERVICE_EDX_OAUTH2_KEY,
             settings.BACKEND_SERVICE_EDX_OAUTH2_SECRET,
         )
 
+    def get_subsidy_aggregates_by_learner_url(self, subsidy_uuid):
+        """
+        Helper method to fetch subsidy learner aggregate data API url.
+        """
+        return f"{self.SUBSIDIES_ENDPOINT}{subsidy_uuid}/aggregates-by-learner"
+
+    def get_subsidy_aggregates_by_learner_data(self, subsidy_uuid, policy_uuid=None):
+        """
+        Client method to fetch subsidy specific learner aggregate data.
+
+        Args:
+            subsidy_uuid (str): Subsidy record UUID
+            policy_uuid (string): Optional param to filter subsidy aggregate data by subsidy access policy UUID
+        Returns:
+            json subsidy learner aggregate data response:
+                [{
+                    'lms_user_id': '1337',
+                    'enrollment_count': 45,
+                } ... ]
+        """
+        url = self.get_subsidy_aggregates_by_learner_url(subsidy_uuid)
+        if policy_uuid:
+            url += f"?subsidy_access_policy_uuid={policy_uuid}"
+        try:
+            resp = self.client.get(url)
+            response_data = resp
+            resp.raise_for_status()
+        except requests.exceptions.HTTPError as exc:
+            logger.exception(
+                f'Subsidy client failed to fetch aggregate data for {subsidy_uuid} '
+                f'and policy: {policy_uuid}'
+            )
+            raise exc
+        return response_data.json()
+
     def get_content_metadata_url(self, content_identifier):
         """Helper method to generate the subsidy service metadata API url, with a trailing slash."""
         return self.CONTENT_METADATA_ENDPOINT + content_identifier + '/'
 
     def get_subsidy_content_data(self, enterprise_customer_uuid, content_identifier):
         """
         Client method to fetch enterprise specific content data.
```

### Comparing `edx-enterprise-subsidy-client-0.4.2/edx_enterprise_subsidy_client.egg-info/PKG-INFO` & `edx-enterprise-subsidy-client-0.4.3/edx_enterprise_subsidy_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-subsidy-client
-Version: 0.4.2
+Version: 0.4.3
 Summary: Client for interacting with the enterprise-subsidy service.
 Home-page: https://github.com/openedx/edx-enterprise-subsidy-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -221,14 +221,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+[0.4.3]
+*******
+* feat: adding new subsidy client method to fetch subsidy aggregate data
+
 [0.4.2]
 *******
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 * Add python 3.12 support
 
 [0.4.1]
```

### Comparing `edx-enterprise-subsidy-client-0.4.2/edx_enterprise_subsidy_client.egg-info/SOURCES.txt` & `edx-enterprise-subsidy-client-0.4.3/edx_enterprise_subsidy_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.4.2/requirements/constraints.txt` & `edx-enterprise-subsidy-client-0.4.3/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.4.2/setup.py` & `edx-enterprise-subsidy-client-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.4.2/tests/test_client.py` & `edx-enterprise-subsidy-client-0.4.3/tests/test_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,63 @@
 """
 Tests for edx_enterprise_subsidy_client.py.
 """
 import uuid
 from unittest import mock
 
+import requests
+from pytest import raises
+
 from edx_enterprise_subsidy_client import EnterpriseSubsidyAPIClient, EnterpriseSubsidyAPIClientV2
 from test_utils.utils import MockResponse
 
 
 def test_client_init():
     """
     Tests that the client can be successfully initialized.
     """
     subsidy_client = EnterpriseSubsidyAPIClient()
     assert subsidy_client is not None
 
 
 @mock.patch('edx_enterprise_subsidy_client.client.OAuthAPIClient', return_value=mock.MagicMock())
+def test_client_fetch_subsidy_aggregate_data_success(mock_oauth_client):
+    """
+    Test the client's ability to handle api requests to fetch subsidy learner aggregate data from the subsidy service
+    """
+    mocked_data = {
+        'lms_user_id': '1337',
+        'enrollment_count': 10,
+    }
+    mock_oauth_client.return_value.get.return_value = MockResponse(mocked_data, 200)
+    subsidy_service_client = EnterpriseSubsidyAPIClient()
+    response = subsidy_service_client.get_subsidy_aggregates_by_learner_data(
+        subsidy_uuid=str(uuid.uuid4()),
+    )
+    assert response == mocked_data
+
+
+@mock.patch('edx_enterprise_subsidy_client.client.OAuthAPIClient', return_value=mock.MagicMock())
+def test_client_fetch_subsidy_aggregate_data_exception_handling(mock_oauth_client):
+    """
+    Test the client's ability to properly throw errors when the subsidy service returns an error response.
+    """
+    error_message = 'some_error_string'
+    mock_oauth_client.return_value.get.return_value = MockResponse(error_message, 400)
+    subsidy_service_client = EnterpriseSubsidyAPIClient()
+    with raises(requests.exceptions.HTTPError) as exc:
+        subsidy_service_client.get_subsidy_aggregates_by_learner_data(
+            subsidy_uuid=str(uuid.uuid4()),
+        )
+
+    assert exc.value.response.json() == error_message
+    assert exc.value.response.status_code == 400
+
+
+@mock.patch('edx_enterprise_subsidy_client.client.OAuthAPIClient', return_value=mock.MagicMock())
 def test_client_fetch_subsidy_content_data_success(mock_oauth_client):
     """
     Test the client's ability to handle api requests to fetch subsidy content metadata from the subsidy service
     """
     course_key = 'edX+DemoX'
     mocked_data = {
         'content_uuid': '484ad134-8004-43b3-ad56-b57c83e4ba24',
```

