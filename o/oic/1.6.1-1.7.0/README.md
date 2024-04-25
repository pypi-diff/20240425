# Comparing `tmp/oic-1.6.1.tar.gz` & `tmp/oic-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oic-1.6.1.tar", last modified: Mon Jul  3 07:08:43 2023, max compression
+gzip compressed data, was "oic-1.7.0.tar", last modified: Thu Apr 25 15:12:25 2024, max compression
```

## Comparing `oic-1.6.1.tar` & `oic-1.7.0.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.447884 oic-1.6.1/
--rw-r--r--   0 tomas     (1000) tomas     (1000)      563 2021-02-12 13:09:56.000000 oic-1.6.1/LICENSE.txt
--rw-r--r--   0 tomas     (1000) tomas     (1000)       25 2021-02-12 13:09:56.000000 oic-1.6.1/MANIFEST.in
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5407 2023-07-03 07:08:43.447884 oic-1.6.1/PKG-INFO
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4493 2023-03-27 11:11:37.000000 oic-1.6.1/README.rst
--rw-r--r--   0 tomas     (1000) tomas     (1000)      281 2023-07-03 07:08:43.447884 oic-1.6.1/setup.cfg
--rwxr-xr-x   0 tomas     (1000) tomas     (1000)     3319 2023-07-03 07:05:06.000000 oic-1.6.1/setup.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.431884 oic-1.6.1/src/
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.435884 oic-1.6.1/src/oic/
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1450 2023-07-03 07:07:13.000000 oic-1.6.1/src/oic/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1492 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/exception.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.435884 oic-1.6.1/src/oic/extension/
--rw-r--r--   0 tomas     (1000) tomas     (1000)       22 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/extension/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    13270 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/extension/client.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     3802 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/extension/device_flow.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2232 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/extension/heart.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     8286 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/extension/message.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4191 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/extension/pop.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2817 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/extension/popjwt.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5495 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/extension/proof_of_possesion.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    29599 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/extension/provider.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5033 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/extension/signed_http_req.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)      256 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/extension/single.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2430 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/extension/sts.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5217 2023-05-02 08:00:09.000000 oic-1.6.1/src/oic/extension/token.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.439884 oic-1.6.1/src/oic/oauth2/
--rw-r--r--   0 tomas     (1000) tomas     (1000)    41235 2023-05-02 08:00:09.000000 oic-1.6.1/src/oic/oauth2/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5967 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/oauth2/base.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    11396 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/oauth2/consumer.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1111 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/oauth2/exception.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4766 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/oauth2/grant.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    39288 2023-05-02 08:00:09.000000 oic-1.6.1/src/oic/oauth2/message.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    38987 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/oauth2/provider.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     7251 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/oauth2/util.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.439884 oic-1.6.1/src/oic/oic/
--rw-r--r--   0 tomas     (1000) tomas     (1000)    65757 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/oic/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     7820 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/oic/claims_provider.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    18940 2023-05-02 08:00:12.000000 oic-1.6.1/src/oic/oic/consumer.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    40833 2023-05-02 08:00:09.000000 oic-1.6.1/src/oic/oic/message.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    83873 2023-05-02 08:00:09.000000 oic-1.6.1/src/oic/oic/provider.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)        0 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/py.typed
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.443884 oic-1.6.1/src/oic/utils/
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1063 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5983 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/aes.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.443884 oic-1.6.1/src/oic/utils/authn/
--rw-r--r--   0 tomas     (1000) tomas     (1000)       23 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/utils/authn/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     7098 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/authn/authn_context.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    18164 2022-03-08 09:59:02.000000 oic-1.6.1/src/oic/utils/authn/client.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1635 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/utils/authn/client_saml.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1981 2022-03-08 09:59:02.000000 oic-1.6.1/src/oic/utils/authn/javascript_login.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)      783 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/utils/authn/ldap_member.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     3217 2022-03-08 09:59:02.000000 oic-1.6.1/src/oic/utils/authn/ldapc.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2626 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/utils/authn/multi_auth.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    14777 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/authn/saml.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    13839 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/authn/user.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     7248 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/authn/user_cas.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1951 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/authz.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)      507 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/utils/claims.py
--rwxr-xr-x   0 tomas     (1000) tomas     (1000)     6200 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/client_management.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     3901 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/clientdb.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    19258 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/http_util.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     3615 2023-05-02 08:00:09.000000 oic-1.6.1/src/oic/utils/jwt.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    37029 2023-05-02 08:00:09.000000 oic-1.6.1/src/oic/utils/keyio.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1679 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/utils/restrict.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.443884 oic-1.6.1/src/oic/utils/rp/
--rw-r--r--   0 tomas     (1000) tomas     (1000)    15154 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/rp/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    12618 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/rp/oauth2.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1765 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/sanitize.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    32421 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/sdb.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     6122 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/session_backend.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2825 2023-07-03 07:05:06.000000 oic-1.6.1/src/oic/utils/settings.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1601 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/shelve_wrapper.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     3635 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/stateless.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1640 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/utils/template_render.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    10293 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/time_util.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4535 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/utils/token_handler.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.443884 oic-1.6.1/src/oic/utils/userinfo/
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1316 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/utils/userinfo/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2307 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/userinfo/aa_info.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5011 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/userinfo/distaggr.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     3797 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/userinfo/ldap_info.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    10239 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/webfinger.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.435884 oic-1.6.1/src/oic.egg-info/
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5407 2023-07-03 07:08:43.000000 oic-1.6.1/src/oic.egg-info/PKG-INFO
--rw-r--r--   0 tomas     (1000) tomas     (1000)     3066 2023-07-03 07:08:43.000000 oic-1.6.1/src/oic.egg-info/SOURCES.txt
--rw-r--r--   0 tomas     (1000) tomas     (1000)        1 2023-07-03 07:08:43.000000 oic-1.6.1/src/oic.egg-info/dependency_links.txt
--rw-r--r--   0 tomas     (1000) tomas     (1000)       74 2023-07-03 07:08:43.000000 oic-1.6.1/src/oic.egg-info/entry_points.txt
--rw-r--r--   0 tomas     (1000) tomas     (1000)        1 2021-06-14 15:48:45.000000 oic-1.6.1/src/oic.egg-info/not-zip-safe
--rw-r--r--   0 tomas     (1000) tomas     (1000)      419 2023-07-03 07:08:43.000000 oic-1.6.1/src/oic.egg-info/requires.txt
--rw-r--r--   0 tomas     (1000) tomas     (1000)       95 2023-07-03 07:08:43.000000 oic-1.6.1/src/oic.egg-info/top_level.txt
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.447884 oic-1.6.1/tests/
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1672 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_aes.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2518 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_authn_context.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1041 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_authn_user.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1163 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_claims.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5260 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_claims_provider.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    12801 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_client.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1285 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_client_management.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4543 2023-03-27 11:11:37.000000 oic-1.6.1/tests/test_clientdb.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4372 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_grant.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     7590 2023-03-27 11:11:37.000000 oic-1.6.1/tests/test_http_util.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1522 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_jwt.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    19265 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_keyio.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    27204 2023-03-27 11:11:37.000000 oic-1.6.1/tests/test_oauth2.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    11031 2023-03-27 11:11:37.000000 oic-1.6.1/tests/test_oauth2_consumer.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    30827 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_oauth2_message.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    32548 2023-03-27 11:11:37.000000 oic-1.6.1/tests/test_oauth2_provider.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    52202 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_oic.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    43996 2023-05-02 08:00:12.000000 oic-1.6.1/tests/test_oic_consumer.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    12012 2023-03-27 11:11:37.000000 oic-1.6.1/tests/test_oic_consumer_logout.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    47073 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_oic_message.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    76101 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_oic_provider.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    40165 2023-03-27 11:11:37.000000 oic-1.6.1/tests/test_oic_provider_logout.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4670 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_pop.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     7936 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_popjwt.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2725 2023-03-27 11:11:37.000000 oic-1.6.1/tests/test_sanitize.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    27871 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_sdb.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1595 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_shelve_wrapper.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4871 2023-03-27 11:11:37.000000 oic-1.6.1/tests/test_signed_http_request.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)      914 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_stateless.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     6728 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_time_util.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    16929 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_token.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4695 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_token_handler.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4270 2023-03-27 11:11:37.000000 oic-1.6.1/tests/test_user.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    10676 2023-03-27 11:11:37.000000 oic-1.6.1/tests/test_util.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     7150 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_webfinger.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     8586 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_x_client.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    11688 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_x_dynreg.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    20499 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_x_provider.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2024-04-25 15:12:25.734464 oic-1.7.0/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      563 2021-02-12 13:09:56.000000 oic-1.7.0/LICENSE.txt
+-rw-r--r--   0 tomas     (1000) tomas     (1000)       25 2021-02-12 13:09:56.000000 oic-1.7.0/MANIFEST.in
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     6682 2024-04-25 15:12:25.734464 oic-1.7.0/PKG-INFO
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4661 2024-04-25 15:06:10.000000 oic-1.7.0/README.rst
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      281 2024-04-25 15:12:25.738464 oic-1.7.0/setup.cfg
+-rwxr-xr-x   0 tomas     (1000) tomas     (1000)     3277 2024-04-25 15:06:10.000000 oic-1.7.0/setup.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2024-04-25 15:12:25.706464 oic-1.7.0/src/
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2024-04-25 15:12:25.710464 oic-1.7.0/src/oic/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1450 2024-04-25 15:07:58.000000 oic-1.7.0/src/oic/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1492 2021-02-12 13:09:56.000000 oic-1.7.0/src/oic/exception.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2024-04-25 15:12:25.714464 oic-1.7.0/src/oic/extension/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)       22 2021-02-12 13:09:56.000000 oic-1.7.0/src/oic/extension/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    13270 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/extension/client.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     3802 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/extension/device_flow.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2232 2021-02-12 13:09:56.000000 oic-1.7.0/src/oic/extension/heart.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     8286 2021-02-12 13:09:56.000000 oic-1.7.0/src/oic/extension/message.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4191 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/extension/pop.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2817 2021-02-12 13:09:56.000000 oic-1.7.0/src/oic/extension/popjwt.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5495 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/extension/proof_of_possesion.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    29605 2024-04-25 15:06:10.000000 oic-1.7.0/src/oic/extension/provider.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5033 2021-02-12 13:09:56.000000 oic-1.7.0/src/oic/extension/signed_http_req.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      256 2021-02-12 13:09:56.000000 oic-1.7.0/src/oic/extension/single.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2431 2024-01-30 13:46:55.000000 oic-1.7.0/src/oic/extension/sts.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5217 2023-05-02 08:00:09.000000 oic-1.7.0/src/oic/extension/token.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2024-04-25 15:12:25.718464 oic-1.7.0/src/oic/oauth2/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    41235 2023-05-02 08:00:09.000000 oic-1.7.0/src/oic/oauth2/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5973 2024-04-25 15:06:10.000000 oic-1.7.0/src/oic/oauth2/base.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    11395 2024-04-25 15:06:10.000000 oic-1.7.0/src/oic/oauth2/consumer.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1111 2021-02-12 13:09:56.000000 oic-1.7.0/src/oic/oauth2/exception.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4766 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/oauth2/grant.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    39288 2023-05-02 08:00:09.000000 oic-1.7.0/src/oic/oauth2/message.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    38992 2024-04-25 15:06:10.000000 oic-1.7.0/src/oic/oauth2/provider.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     7251 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/oauth2/util.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2024-04-25 15:12:25.718464 oic-1.7.0/src/oic/oic/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    65771 2024-04-25 15:06:10.000000 oic-1.7.0/src/oic/oic/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     7820 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/oic/claims_provider.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    18926 2024-01-30 13:46:55.000000 oic-1.7.0/src/oic/oic/consumer.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    40833 2023-05-02 08:00:09.000000 oic-1.7.0/src/oic/oic/message.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    83876 2024-04-25 15:06:10.000000 oic-1.7.0/src/oic/oic/provider.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)        0 2021-02-12 13:09:56.000000 oic-1.7.0/src/oic/py.typed
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2024-04-25 15:12:25.722464 oic-1.7.0/src/oic/utils/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1063 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/utils/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5983 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/utils/aes.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2024-04-25 15:12:25.722464 oic-1.7.0/src/oic/utils/authn/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)       23 2021-02-12 13:09:56.000000 oic-1.7.0/src/oic/utils/authn/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     7098 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/utils/authn/authn_context.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    18164 2022-03-08 09:59:02.000000 oic-1.7.0/src/oic/utils/authn/client.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1635 2021-02-12 13:09:56.000000 oic-1.7.0/src/oic/utils/authn/client_saml.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1981 2022-03-08 09:59:02.000000 oic-1.7.0/src/oic/utils/authn/javascript_login.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      783 2021-02-12 13:09:56.000000 oic-1.7.0/src/oic/utils/authn/ldap_member.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     3217 2022-03-08 09:59:02.000000 oic-1.7.0/src/oic/utils/authn/ldapc.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2626 2021-02-12 13:09:56.000000 oic-1.7.0/src/oic/utils/authn/multi_auth.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    14783 2024-04-25 15:06:10.000000 oic-1.7.0/src/oic/utils/authn/saml.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    13839 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/utils/authn/user.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     7248 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/utils/authn/user_cas.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1951 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/utils/authz.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      507 2021-02-12 13:09:56.000000 oic-1.7.0/src/oic/utils/claims.py
+-rwxr-xr-x   0 tomas     (1000) tomas     (1000)     6200 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/utils/client_management.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     3902 2024-01-30 13:46:55.000000 oic-1.7.0/src/oic/utils/clientdb.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    19257 2024-04-25 15:06:10.000000 oic-1.7.0/src/oic/utils/http_util.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     3615 2023-05-02 08:00:09.000000 oic-1.7.0/src/oic/utils/jwt.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    37035 2024-04-25 15:06:10.000000 oic-1.7.0/src/oic/utils/keyio.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1679 2021-02-12 13:09:56.000000 oic-1.7.0/src/oic/utils/restrict.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2024-04-25 15:12:25.722464 oic-1.7.0/src/oic/utils/rp/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    15153 2024-04-25 15:06:10.000000 oic-1.7.0/src/oic/utils/rp/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    12619 2024-04-25 15:06:10.000000 oic-1.7.0/src/oic/utils/rp/oauth2.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1765 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/utils/sanitize.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    32421 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/utils/sdb.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     6122 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/utils/session_backend.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2826 2024-01-30 13:46:55.000000 oic-1.7.0/src/oic/utils/settings.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1601 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/utils/shelve_wrapper.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     3635 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/utils/stateless.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1640 2021-02-12 13:09:56.000000 oic-1.7.0/src/oic/utils/template_render.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    10293 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/utils/time_util.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4535 2021-02-12 13:09:56.000000 oic-1.7.0/src/oic/utils/token_handler.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2024-04-25 15:12:25.722464 oic-1.7.0/src/oic/utils/userinfo/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1316 2021-02-12 13:09:56.000000 oic-1.7.0/src/oic/utils/userinfo/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2307 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/utils/userinfo/aa_info.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5011 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/utils/userinfo/distaggr.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     3797 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/utils/userinfo/ldap_info.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    10239 2023-03-27 11:11:37.000000 oic-1.7.0/src/oic/utils/webfinger.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2024-04-25 15:12:25.734464 oic-1.7.0/src/oic.egg-info/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     6682 2024-04-25 15:12:25.000000 oic-1.7.0/src/oic.egg-info/PKG-INFO
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     3066 2024-04-25 15:12:25.000000 oic-1.7.0/src/oic.egg-info/SOURCES.txt
+-rw-r--r--   0 tomas     (1000) tomas     (1000)        1 2024-04-25 15:12:25.000000 oic-1.7.0/src/oic.egg-info/dependency_links.txt
+-rw-r--r--   0 tomas     (1000) tomas     (1000)       74 2024-04-25 15:12:25.000000 oic-1.7.0/src/oic.egg-info/entry_points.txt
+-rw-r--r--   0 tomas     (1000) tomas     (1000)        1 2021-06-14 15:48:45.000000 oic-1.7.0/src/oic.egg-info/not-zip-safe
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      426 2024-04-25 15:12:25.000000 oic-1.7.0/src/oic.egg-info/requires.txt
+-rw-r--r--   0 tomas     (1000) tomas     (1000)       95 2024-04-25 15:12:25.000000 oic-1.7.0/src/oic.egg-info/top_level.txt
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2024-04-25 15:12:25.730464 oic-1.7.0/tests/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1672 2021-02-12 13:09:56.000000 oic-1.7.0/tests/test_aes.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2518 2021-02-12 13:09:56.000000 oic-1.7.0/tests/test_authn_context.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1041 2021-02-12 13:09:56.000000 oic-1.7.0/tests/test_authn_user.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1163 2021-02-12 13:09:56.000000 oic-1.7.0/tests/test_claims.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5260 2023-05-02 08:00:09.000000 oic-1.7.0/tests/test_claims_provider.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    12801 2023-05-02 08:00:09.000000 oic-1.7.0/tests/test_client.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1285 2021-02-12 13:09:56.000000 oic-1.7.0/tests/test_client_management.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4544 2024-01-30 13:48:03.000000 oic-1.7.0/tests/test_clientdb.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4372 2021-02-12 13:09:56.000000 oic-1.7.0/tests/test_grant.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     7590 2023-03-27 11:11:37.000000 oic-1.7.0/tests/test_http_util.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1522 2023-05-02 08:00:09.000000 oic-1.7.0/tests/test_jwt.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    19265 2023-05-02 08:00:09.000000 oic-1.7.0/tests/test_keyio.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    27204 2023-03-27 11:11:37.000000 oic-1.7.0/tests/test_oauth2.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    11031 2023-03-27 11:11:37.000000 oic-1.7.0/tests/test_oauth2_consumer.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    30827 2023-05-02 08:00:09.000000 oic-1.7.0/tests/test_oauth2_message.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    32548 2023-03-27 11:11:37.000000 oic-1.7.0/tests/test_oauth2_provider.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    52202 2023-05-02 08:00:09.000000 oic-1.7.0/tests/test_oic.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    43996 2023-05-02 08:00:12.000000 oic-1.7.0/tests/test_oic_consumer.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    12012 2023-03-27 11:11:37.000000 oic-1.7.0/tests/test_oic_consumer_logout.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    47073 2023-05-02 08:00:09.000000 oic-1.7.0/tests/test_oic_message.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    76113 2024-04-25 15:06:10.000000 oic-1.7.0/tests/test_oic_provider.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    40165 2023-03-27 11:11:37.000000 oic-1.7.0/tests/test_oic_provider_logout.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4670 2021-02-12 13:09:56.000000 oic-1.7.0/tests/test_pop.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     7936 2021-02-12 13:09:56.000000 oic-1.7.0/tests/test_popjwt.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2725 2023-03-27 11:11:37.000000 oic-1.7.0/tests/test_sanitize.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    27871 2021-02-12 13:09:56.000000 oic-1.7.0/tests/test_sdb.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1595 2021-02-12 13:09:56.000000 oic-1.7.0/tests/test_shelve_wrapper.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4871 2023-03-27 11:11:37.000000 oic-1.7.0/tests/test_signed_http_request.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      914 2021-02-12 13:09:56.000000 oic-1.7.0/tests/test_stateless.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     6728 2021-02-12 13:09:56.000000 oic-1.7.0/tests/test_time_util.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    16929 2023-05-02 08:00:09.000000 oic-1.7.0/tests/test_token.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4695 2023-05-02 08:00:09.000000 oic-1.7.0/tests/test_token_handler.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4270 2023-03-27 11:11:37.000000 oic-1.7.0/tests/test_user.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    10676 2023-03-27 11:11:37.000000 oic-1.7.0/tests/test_util.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     7150 2021-02-12 13:09:56.000000 oic-1.7.0/tests/test_webfinger.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     8586 2023-05-02 08:00:09.000000 oic-1.7.0/tests/test_x_client.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    11688 2021-02-12 13:09:56.000000 oic-1.7.0/tests/test_x_dynreg.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    20505 2024-01-30 13:48:03.000000 oic-1.7.0/tests/test_x_provider.py
```

### Comparing `oic-1.6.1/LICENSE.txt` & `oic-1.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/PKG-INFO` & `oic-1.7.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: oic
-Version: 1.6.1
-Summary: Python implementation of OAuth2 and OpenID Connect
-Home-page: https://github.com/CZ-NIC/pyoidc/
-Author: Roland Hedberg
-Author-email: roland@catalogix.se
-License: Apache 2.0
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: ~=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: develop
-Provides-Extra: testing
-Provides-Extra: docs
-Provides-Extra: quality
-Provides-Extra: types
-Provides-Extra: ldap_authn
-Provides-Extra: examples
-License-File: LICENSE.txt
-
 .. image:: https://ci.appveyor.com/api/projects/status/5g3ucux767mef3f4/branch/master?svg=true
     :target: https://ci.appveyor.com/project/tpazderka/pyoidc/branch/master
 
 .. image:: https://img.shields.io/pypi/pyversions/oic.svg
     :target: https://pypi.python.org/pypi/oic
 
 .. image:: https://img.shields.io/pypi/v/oic.svg
@@ -39,14 +12,17 @@
 
 .. image:: https://codecov.io/gh/CZ-NIC/pyoidc/branch/master/graph/badge.svg
   :target: https://codecov.io/gh/CZ-NIC/pyoidc
 
 .. image:: https://api.codacy.com/project/badge/Grade/2038cfa7c56b480db6ae18b8320d7157
     :target: https://www.codacy.com/app/tpazderka/pyoidc?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=CZ-NIC/pyoidc&amp;utm_campaign=Badge_Grade
 
+.. image:: https://api.securityscorecards.dev/projects/github.com/CZ-NIC/pyoidc/badge
+    :target: https://securityscorecards.dev/viewer/?uri=github.com/CZ-NIC/pyoidc
+
 A Python OpenID Connect implementation
 ======================================
 
 This is a complete implementation of OpenID Connect as specified in the `OpenID
 Connect Core specification`_. And as a side effect, a complete implementation
 of OAuth2.0 too.
```

### Comparing `oic-1.6.1/setup.py` & `oic-1.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,25 +64,24 @@
     },
     package_dir={"": "src"},
     package_data={"oic": ["py.typed"]},
     include_package_data=True,
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Python Modules"],
-    python_requires='~=3.7',
+    python_requires='~=3.8',
     extras_require={
         'develop': ["cherrypy==3.2.4", "pyOpenSSL"],
         'testing': tests_requires,
-        'docs': ['Sphinx', 'sphinx-autobuild', 'alabaster', 'autodoc_pydantic'],
+        'docs': ['Sphinx', 'sphinx-autobuild', 'alabaster', 'autodoc_pydantic>=2.0.0'],
         'quality': ['pylama', 'isort', 'eradicate', 'mypy', 'black', 'bandit', 'readme_renderer[md]'],
         'types': ['types-requests'],
         'ldap_authn': ['python-ldap'],
         'examples': ['beaker'],
     },
     install_requires=[
         "requests",
```

### Comparing `oic-1.6.1/src/oic/__init__.py` & `oic-1.7.0/src/oic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         warnings.warn(
             "No good random number generator available on this platform. "
             "Security tokens will be weak and guessable.",
             RuntimeWarning,
         )
 
 __author__ = "Roland Hedberg"
-__version__ = "1.6.1"
+__version__ = "1.7.0"
 
 
 OIDCONF_PATTERN = "%s/.well-known/openid-configuration"
 CC_METHOD = {"S256": hashlib.sha256, "S384": hashlib.sha384, "S512": hashlib.sha512}
 
 
 def rndstr(size=16):
```

### Comparing `oic-1.6.1/src/oic/exception.py` & `oic-1.7.0/src/oic/exception.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/extension/client.py` & `oic-1.7.0/src/oic/extension/client.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/extension/device_flow.py` & `oic-1.7.0/src/oic/extension/device_flow.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/extension/heart.py` & `oic-1.7.0/src/oic/extension/heart.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/extension/message.py` & `oic-1.7.0/src/oic/extension/message.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/extension/pop.py` & `oic-1.7.0/src/oic/extension/pop.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/extension/popjwt.py` & `oic-1.7.0/src/oic/extension/popjwt.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/extension/proof_of_possesion.py` & `oic-1.7.0/src/oic/extension/proof_of_possesion.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/extension/provider.py` & `oic-1.7.0/src/oic/extension/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -740,15 +740,15 @@
         :param authn:
         :param req:
         :return:
         """
         try:
             client_id = self.client_authn(self, req, authn)
         except FailedAuthentication as err:
-            logger.error(err)
+            logger.error("%s", err)
             error = TokenErrorResponse(
                 error="unauthorized_client", error_description="%s" % err
             )
             return Response(
                 error.to_json(), content="application/json", status="401 Unauthorized"
             )
```

### Comparing `oic-1.6.1/src/oic/extension/signed_http_req.py` & `oic-1.7.0/src/oic/extension/signed_http_req.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/extension/sts.py` & `oic-1.7.0/src/oic/extension/sts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Message types in draft-ietf-oauth-token-exchange-03.
 
 :copyright: (c) 2016 by Roland Hedberg.
 :license: Apache2, see LICENSE for more details.
 
 """
+
 import json
 
 from oic.oauth2.message import OPTIONAL_LIST_OF_SP_SEP_STRINGS
 from oic.oauth2.message import OPTIONAL_LIST_OF_STRINGS
 from oic.oauth2.message import REQUIRED_LIST_OF_STRINGS
 from oic.oauth2.message import SINGLE_OPTIONAL_INT
 from oic.oauth2.message import SINGLE_OPTIONAL_STRING
```

### Comparing `oic-1.6.1/src/oic/extension/token.py` & `oic-1.7.0/src/oic/extension/token.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/oauth2/__init__.py` & `oic-1.7.0/src/oic/oauth2/__init__.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/oauth2/base.py` & `oic-1.7.0/src/oic/oauth2/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
         try:
             _cookie = r.headers["set-cookie"]
             logger.debug("RECEIVED COOKIE")
             try:
                 set_cookie(self.cookiejar, SimpleCookie(_cookie))
             except CookieError as err:
-                logger.error(err)
+                logger.error("%s", err)
                 raise NonFatalException(r, "{}".format(err))
         except (AttributeError, KeyError):
             pass
 
         return r
 
     def send(self, url, method="GET", **kwargs):
```

### Comparing `oic-1.6.1/src/oic/oauth2/consumer.py` & `oic-1.7.0/src/oic/oauth2/consumer.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,15 +285,15 @@
         if "code" in self.response_type:
             # Might be an error response
             try:
                 aresp = self.parse_response(
                     AuthorizationResponse, info=query, sformat="urlencoded"
                 )
             except Exception as err:
-                logger.error("%s" % err)
+                logger.error("%s", err)
                 raise
 
             if isinstance(aresp, Message):
                 if aresp.type().endswith("ErrorResponse"):
                     raise AuthzError(aresp["error"])
 
             try:
```

### Comparing `oic-1.6.1/src/oic/oauth2/exception.py` & `oic-1.7.0/src/oic/oauth2/exception.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/oauth2/grant.py` & `oic-1.7.0/src/oic/oauth2/grant.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/oauth2/message.py` & `oic-1.7.0/src/oic/oauth2/message.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/oauth2/provider.py` & `oic-1.7.0/src/oic/oauth2/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -588,15 +588,15 @@
         )
         logger.debug("Request: '%s'" % sanitize(request))
         # Same serialization used for GET and POST
 
         try:
             areq = self.server.parse_authorization_request(query=request)
         except (MissingRequiredValue, MissingRequiredAttribute, AuthzError) as err:
-            logger.debug("%s" % err)
+            logger.debug("%s", err)
             areq = request_class()
             areq.lax = True
             if isinstance(request, dict):
                 areq.from_dict(request)
             else:
                 areq.deserialize(request, "urlencoded")
             try:
@@ -1011,15 +1011,15 @@
             "token_endpoint"
         )().deserialize(request, dtype)
 
         # Verify client authentication
         try:
             client_id = self.client_authn(self, areq, authn)
         except (FailedAuthentication, AuthnFailure) as err:
-            logger.error(err)
+            logger.error("%s", err)
             error = TokenErrorResponse(
                 error="unauthorized_client", error_description="%s" % err
             )
             return Unauthorized(error.to_json(), content="application/json")
 
         logger.debug("AccessTokenRequest: %s" % sanitize(areq))
```

### Comparing `oic-1.6.1/src/oic/oauth2/util.py` & `oic-1.7.0/src/oic/oauth2/util.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/oic/__init__.py` & `oic-1.7.0/src/oic/oic/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1236,17 +1236,17 @@
                 pass
             if key not in PREFERENCE2PROVIDER:
                 self.behaviour[key] = val
 
     def store_registration_info(self, reginfo):
         self.registration_response = reginfo
         if "token_endpoint_auth_method" not in self.registration_response:
-            self.registration_response[
-                "token_endpoint_auth_method"  # nosec
-            ] = "client_secret_basic"
+            self.registration_response["token_endpoint_auth_method"] = (  # nosec
+                "client_secret_basic"
+            )
         self.client_id = reginfo["client_id"]
         try:
             self.client_secret = reginfo["client_secret"]
         except KeyError:  # Not required
             pass
         else:
             try:
@@ -1265,15 +1265,15 @@
             resp = self.message_factory.get_response_type(
                 "registration_endpoint"
             )().deserialize(response.text, "json")
             # Some implementations sends back a 200 with an error message inside
             try:
                 resp.verify()
             except oauth2.message.MissingRequiredAttribute as err:
-                logger.error(err)
+                logger.error("%s", err)
                 raise RegistrationError(err)
             except Exception:
                 resp = ErrorResponse().deserialize(response.text, "json")
                 if resp.verify():
                     logger.error(err_msg.format(sanitize(resp.to_json())))
                     if self.events:
                         self.events.store("protocol response", resp)
@@ -1673,15 +1673,15 @@
             self.events.store("Combined Request", _req)
 
         try:
             _req.verify(keyjar=self.keyjar)
         except Exception as err:
             if self.events:
                 self.events.store("Exception", err)
-            logger.error(err)
+            logger.error("%s", err)
             raise
 
         return _req
 
     def parse_jwt_request(
         self,
         request=AuthorizationRequest,
```

### Comparing `oic-1.6.1/src/oic/oic/claims_provider.py` & `oic-1.7.0/src/oic/oic/claims_provider.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/oic/consumer.py` & `oic-1.7.0/src/oic/oic/consumer.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,17 +363,15 @@
             self.update(_state)
         except KeyError:
             raise UnknownState(_state, aresp)
 
         self.redirect_uris = [self.sdb[_state]["redirect_uris"]]
         return aresp, _state
 
-    def parse_authz(
-        self, query="", **kwargs
-    ) -> Union[
+    def parse_authz(self, query="", **kwargs) -> Union[
         http_util.BadRequest,
         Tuple[
             Optional[AuthorizationResponse],
             Optional[AccessTokenResponse],
             Optional[IdToken],
         ],
     ]:
```

### Comparing `oic-1.6.1/src/oic/oic/message.py` & `oic-1.7.0/src/oic/oic/message.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/oic/provider.py` & `oic-1.7.0/src/oic/oic/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -870,27 +870,27 @@
         permissions = _info.get("permission", ["offline_access"]) or ["offline_access"]
         if "offline_access" in _info["scope"] and "offline_access" in permissions:
             issue_refresh = True
 
         try:
             _tinfo = _sdb.upgrade_to_token(_access_code, issue_refresh=issue_refresh)
         except AccessCodeUsed as err:
-            logger.error("%s" % err)
+            logger.error("%s", err)
             # Should revoke the token issued to this access code
             _sdb.revoke_all_tokens(_access_code)
             return error_response("access_denied", descr="Access Code already used")
 
         if "openid" in _info["scope"]:
             userinfo = self.userinfo_in_id_token_claims(_info)
             try:
                 _idtoken = self.sign_encrypt_id_token(
                     _info, client_info, areq, user_info=userinfo
                 )
             except (JWEException, NoSuitableSigningKeys) as err:
-                logger.warning(str(err))
+                logger.warning("%s", err)
                 return error_response(
                     "invalid_request", descr="Could not sign/encrypt id_token"
                 )
 
             _sdb.update_by_token(_access_code, "id_token", _idtoken)
 
         # Refresh the _tinfo
@@ -930,15 +930,15 @@
         if "openid" in _info["scope"] and "authn_event" in _info:
             userinfo = self.userinfo_in_id_token_claims(_info)
             try:
                 _idtoken = self.sign_encrypt_id_token(
                     _info, client_info, areq, user_info=userinfo
                 )
             except (JWEException, NoSuitableSigningKeys) as err:
-                logger.warning(str(err))
+                logger.warning("%s", err)
                 return error_response(
                     "invalid_request", descr="Could not sign/encrypt id_token"
                 )
 
             sid = _sdb.access_token.get_key(_info["access_token"])
             _sdb.update(sid, "id_token", _idtoken)
 
@@ -1372,15 +1372,15 @@
         :return: si_redirects, sector_id
         :raises: InvalidSectorIdentifier
         """
         si_url = request["sector_identifier_uri"]
         try:
             res = self.server.http_request(si_url)
         except RequestException as err:
-            logger.error(err)
+            logger.error("%s", err)
             res = None
 
         if not res:
             raise InvalidSectorIdentifier("Couldn't open sector_identifier_uri")
 
         logger.debug("sector_identifier_uri => %s", sanitize(res.text))
 
@@ -1794,15 +1794,15 @@
 
                 # or 'code id_token'
                 try:
                     id_token = self.sign_encrypt_id_token(
                         _sinfo, client_info, areq, user_info=user_info, **hargs
                     )
                 except (JWEException, NoSuitableSigningKeys) as err:
-                    logger.warning(str(err))
+                    logger.warning("%s", err)
                     return error_response(
                         "invalid_request", descr="Could not sign/encrypt id_token"
                     )
 
                 aresp["id_token"] = id_token
                 _sinfo["id_token"] = id_token
                 rtype.remove("id_token")
@@ -1931,15 +1931,15 @@
 
         try:
             accepted_urls = self.cdb[client_id]["post_logout_redirect_uris"]
             if self._verify_url(redirect_uri, accepted_urls):
                 return redirect_uri
         except Exception as exc:
             msg = "An error occurred while verifying redirect URI: %s"
-            logger.debug(msg, str(exc))
+            logger.debug(msg, exc)
 
         return None
 
     def let_user_verify_logout(
         self,
         uid: str,
         esr: Message,
```

### Comparing `oic-1.6.1/src/oic/utils/__init__.py` & `oic-1.7.0/src/oic/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/aes.py` & `oic-1.7.0/src/oic/utils/aes.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/authn/authn_context.py` & `oic-1.7.0/src/oic/utils/authn/authn_context.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/authn/client.py` & `oic-1.7.0/src/oic/utils/authn/client.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/authn/client_saml.py` & `oic-1.7.0/src/oic/utils/authn/client_saml.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/authn/javascript_login.py` & `oic-1.7.0/src/oic/utils/authn/javascript_login.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/authn/ldap_member.py` & `oic-1.7.0/src/oic/utils/authn/ldap_member.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/authn/ldapc.py` & `oic-1.7.0/src/oic/utils/authn/ldapc.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/authn/multi_auth.py` & `oic-1.7.0/src/oic/utils/authn/multi_auth.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/authn/saml.py` & `oic-1.7.0/src/oic/utils/authn/saml.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,15 +364,15 @@
             _rstate = rndstr()
             ht_args = _cli.apply_binding(
                 binding, msg_str, destination, relay_state=_rstate
             )
 
             logger.debug("ht_args: %s" % ht_args)
         except Exception as exc:
-            logger.exception(exc)
+            logger.exception("%s", exc)
             raise ServiceErrorException(
                 "Failed to construct the AuthnRequest: %s" % exc
             )
 
         # remember the request
         self.cache_outstanding_queries[_sid] = self.return_to
         return self.response(binding, ht_args, query)
```

### Comparing `oic-1.6.1/src/oic/utils/authn/user.py` & `oic-1.7.0/src/oic/utils/authn/user.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/authn/user_cas.py` & `oic-1.7.0/src/oic/utils/authn/user_cas.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/authz.py` & `oic-1.7.0/src/oic/utils/authz.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/client_management.py` & `oic-1.7.0/src/oic/utils/client_management.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/clientdb.py` & `oic-1.7.0/src/oic/utils/clientdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Client management databases."""
+
 from abc import ABCMeta
 from abc import abstractmethod
 from urllib.parse import quote
 from urllib.parse import urljoin
 
 import requests
```

### Comparing `oic-1.6.1/src/oic/utils/http_util.py` & `oic-1.7.0/src/oic/utils/http_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -556,15 +556,15 @@
     try:
         resp, state = args
         return resp(environ, start_response)
     except TypeError:
         resp = args
         return resp(environ, start_response)
     except Exception as err:
-        logger.error("%s" % err)
+        logger.error("%s", err)
         raise
 
 
 class CookieDealer(object):
     @property
     def srv(self):
         return self._srv
```

### Comparing `oic-1.6.1/src/oic/utils/jwt.py` & `oic-1.7.0/src/oic/utils/jwt.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/keyio.py` & `oic-1.7.0/src/oic/utils/keyio.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         if self.etag:
             args["headers"] = {"If-None-Match": self.etag}
 
         try:
             logger.debug("KeyBundle fetch keys from: %s", self.source)
             r = requests.get(self.source, timeout=self.timeout, **args)
         except Exception as err:
-            logger.error(err)
+            logger.error("%s", err)
             raise_exception(UpdateFailed, REMOTE_FAILED.format(self.source, str(err)))
 
         if r.status_code == 304:  # file has not changed
             self.time_out = time.time() + self.cache_time
             self.last_updated = time.time()
             try:
                 self.do_keys(self.imp_jwks["keys"])
```

### Comparing `oic-1.6.1/src/oic/utils/restrict.py` & `oic-1.7.0/src/oic/utils/restrict.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/rp/__init__.py` & `oic-1.7.0/src/oic/utils/rp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
                 state=authresp["state"],
                 request_args=args,
                 authn_method=self.registration_response["token_endpoint_auth_method"],
             )
             msg = "Access token response: {}"
             logger.info(msg.format(sanitize(atresp)))
         except Exception as err:
-            logger.error("%s" % err)
+            logger.error("%s", err)
             raise
 
         if isinstance(atresp, ErrorResponse):
             msg = "Error response: {}"
             self._err(msg.format(sanitize(atresp.to_dict())))
 
         _token = atresp["access_token"]
```

### Comparing `oic-1.6.1/src/oic/utils/rp/oauth2.py` & `oic-1.7.0/src/oic/utils/rp/oauth2.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,17 +112,17 @@
         """
         Call when an AuthN response has been received from the OP.
 
         :param response: The URL returned by the OP
         :return:
         """
         if self.behaviour["response_type"] == "code":
-            respcls: Union[
-                Type[AuthorizationResponse], Type[AccessTokenResponse]
-            ] = AuthorizationResponse
+            respcls: Union[Type[AuthorizationResponse], Type[AccessTokenResponse]] = (
+                AuthorizationResponse
+            )
         else:
             respcls = AccessTokenResponse
 
         try:
             authresp = self.parse_response(
                 respcls, response, sformat=format, keyjar=self.keyjar
             )
@@ -165,15 +165,15 @@
                     request_args=args,
                     authn_method=self.registration_response[
                         "token_endpoint_auth_method"
                     ],
                 )
                 logger.info("Access token response: {}".format(sanitize(atresp)))
             except Exception as err:
-                logger.error("%s" % err)
+                logger.error("%s", err)
                 raise
 
             if isinstance(atresp, ErrorResponse):
                 self._err("Error response: {}".format(atresp.to_dict()))
 
             _token = atresp["access_token"]
         else:
```

### Comparing `oic-1.6.1/src/oic/utils/sanitize.py` & `oic-1.7.0/src/oic/utils/sanitize.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/sdb.py` & `oic-1.7.0/src/oic/utils/sdb.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/session_backend.py` & `oic-1.7.0/src/oic/utils/session_backend.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/settings.py` & `oic-1.7.0/src/oic/utils/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 In order to configure some objects in PyOIDC, you need a settings object.
 If you need to add some settings, make sure that you settings class inherits from the appropriate class in this module.
 
 The settings make use of `pydantic-settings <https://docs.pydantic.dev/usage/settings/>`_ library.
 It is possible to instance them directly or use environment values to fill the settings.
 """
+
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import requests
 from pydantic_settings import BaseSettings
```

### Comparing `oic-1.6.1/src/oic/utils/shelve_wrapper.py` & `oic-1.7.0/src/oic/utils/shelve_wrapper.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/stateless.py` & `oic-1.7.0/src/oic/utils/stateless.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/template_render.py` & `oic-1.7.0/src/oic/utils/template_render.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/time_util.py` & `oic-1.7.0/src/oic/utils/time_util.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/token_handler.py` & `oic-1.7.0/src/oic/utils/token_handler.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/userinfo/__init__.py` & `oic-1.7.0/src/oic/utils/userinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/userinfo/aa_info.py` & `oic-1.7.0/src/oic/utils/userinfo/aa_info.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/userinfo/distaggr.py` & `oic-1.7.0/src/oic/utils/userinfo/distaggr.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/userinfo/ldap_info.py` & `oic-1.7.0/src/oic/utils/userinfo/ldap_info.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic/utils/webfinger.py` & `oic-1.7.0/src/oic/utils/webfinger.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/src/oic.egg-info/SOURCES.txt` & `oic-1.7.0/src/oic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_aes.py` & `oic-1.7.0/tests/test_aes.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_authn_context.py` & `oic-1.7.0/tests/test_authn_context.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_authn_user.py` & `oic-1.7.0/tests/test_authn_user.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_claims.py` & `oic-1.7.0/tests/test_claims.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_claims_provider.py` & `oic-1.7.0/tests/test_claims_provider.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_client.py` & `oic-1.7.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_client_management.py` & `oic-1.7.0/tests/test_client_management.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_clientdb.py` & `oic-1.7.0/tests/test_clientdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Unittests for ClientDatabases."""
+
 import json
 from operator import itemgetter
 from typing import Any
 from typing import Dict
 
 import pytest
 import responses
```

### Comparing `oic-1.6.1/tests/test_grant.py` & `oic-1.7.0/tests/test_grant.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_http_util.py` & `oic-1.7.0/tests/test_http_util.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_jwt.py` & `oic-1.7.0/tests/test_jwt.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_keyio.py` & `oic-1.7.0/tests/test_keyio.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_oauth2.py` & `oic-1.7.0/tests/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_oauth2_consumer.py` & `oic-1.7.0/tests/test_oauth2_consumer.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_oauth2_message.py` & `oic-1.7.0/tests/test_oauth2_message.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_oauth2_provider.py` & `oic-1.7.0/tests/test_oauth2_provider.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_oic.py` & `oic-1.7.0/tests/test_oic.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_oic_consumer.py` & `oic-1.7.0/tests/test_oic_consumer.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_oic_consumer_logout.py` & `oic-1.7.0/tests/test_oic_consumer_logout.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_oic_message.py` & `oic-1.7.0/tests/test_oic_message.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_oic_provider.py` & `oic-1.7.0/tests/test_oic_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1345,20 +1345,20 @@
         with LogCapture(level=logging.DEBUG) as logcap:
             message = "Couldn't open sector_identifier_uri"
             with pytest.raises(InvalidSectorIdentifier, match=message):
                 self.provider._verify_sector_identifier(rr)
 
         assert len(logcap.records) == 2
         # First log record is from server...
-        assert isinstance(logcap.records[1].msg, MissingSchema)
+        assert isinstance(logcap.records[1].args[0], MissingSchema)
         error = (
             "Invalid URL 'example.com': No scheme supplied. Perhaps you meant "
             "https://example.com?"
         )
-        assert str(logcap.records[1].msg) == error
+        assert logcap.records[1].getMessage() == error
 
     def test_verify_sector_identifier_nonreachable(self):
         rr = RegistrationRequest(
             operation="register", sector_identifier_uri="https://example.com"
         )
         with responses.RequestsMock() as rsps, LogCapture(
             level=logging.DEBUG
@@ -1382,15 +1382,15 @@
             with pytest.raises(
                 InvalidSectorIdentifier, match="Couldn't open sector_identifier_uri"
             ):
                 self.provider._verify_sector_identifier(rr)
 
         assert len(logcap.records) == 2
         # First log record is from server...
-        assert logcap.records[1].msg == error
+        assert logcap.records[1].args[0] == error
 
     def test_verify_sector_identifier_malformed(self):
         rr = RegistrationRequest(
             operation="register", sector_identifier_uri="https://example.com"
         )
         body = "This is not the JSON you are looking for"
         with responses.RequestsMock() as rsps, LogCapture(
```

### Comparing `oic-1.6.1/tests/test_oic_provider_logout.py` & `oic-1.7.0/tests/test_oic_provider_logout.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_pop.py` & `oic-1.7.0/tests/test_pop.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_popjwt.py` & `oic-1.7.0/tests/test_popjwt.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_sanitize.py` & `oic-1.7.0/tests/test_sanitize.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_sdb.py` & `oic-1.7.0/tests/test_sdb.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_shelve_wrapper.py` & `oic-1.7.0/tests/test_shelve_wrapper.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_signed_http_request.py` & `oic-1.7.0/tests/test_signed_http_request.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_stateless.py` & `oic-1.7.0/tests/test_stateless.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_time_util.py` & `oic-1.7.0/tests/test_time_util.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_token.py` & `oic-1.7.0/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_token_handler.py` & `oic-1.7.0/tests/test_token_handler.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_user.py` & `oic-1.7.0/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_util.py` & `oic-1.7.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_webfinger.py` & `oic-1.7.0/tests/test_webfinger.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_x_client.py` & `oic-1.7.0/tests/test_x_client.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_x_dynreg.py` & `oic-1.7.0/tests/test_x_dynreg.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.1/tests/test_x_provider.py` & `oic-1.7.0/tests/test_x_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -508,44 +508,44 @@
     def test_password_grant_type_ok(self):
         # Set a not so dummy Authn method and token policy
         self.provider.authn_broker = AUTHN_BROKER2
         self.provider.set_token_policy("client1", {"grant_type": ["password"]})
         areq = ROPCAccessTokenRequest(
             grant_type="password", username="username", password="password"
         )
-        areq[
-            "client_id"
-        ] = "client1"  # Token endpoint would fill that in based on client_authn
+        areq["client_id"] = (
+            "client1"  # Token endpoint would fill that in based on client_authn
+        )
         resp = self.provider.password_grant_type(areq)
 
         atr = AccessTokenResponse().deserialize(resp.message, "json")
         assert _eq(atr.keys(), ["access_token", "token_type", "refresh_token"])
 
     def test_password_grant_type_no_authn(self):
         # Set a blank AuthnBroker
         self.provider.authn_broker = AuthnBroker()
         self.provider.set_token_policy("client1", {"grant_type": ["password"]})
         areq = ROPCAccessTokenRequest(
             grant_type="password", username="username", password="password"
         )
-        areq[
-            "client_id"
-        ] = "client1"  # Token endpoint would fill that in based on client_authn
+        areq["client_id"] = (
+            "client1"  # Token endpoint would fill that in based on client_authn
+        )
         resp = self.provider.password_grant_type(areq)
 
         atr = TokenErrorResponse().deserialize(resp.message, "json")
         assert atr["error"] == "invalid_grant"
 
     def test_password_grant_type_bad(self):
         # Set a not so dummy Authn method and token policy
         self.provider.authn_broker = AUTHN_BROKER2
         self.provider.set_token_policy("client1", {"grant_type": ["password"]})
         areq = ROPCAccessTokenRequest(
             grant_type="password", username="username", password="bad_password"
         )
-        areq[
-            "client_id"
-        ] = "client1"  # Token endpoint would fill that in based on client_authn
+        areq["client_id"] = (
+            "client1"  # Token endpoint would fill that in based on client_authn
+        )
         resp = self.provider.password_grant_type(areq)
 
         atr = TokenErrorResponse().deserialize(resp.message, "json")
         assert atr["error"] == "invalid_grant"
```

