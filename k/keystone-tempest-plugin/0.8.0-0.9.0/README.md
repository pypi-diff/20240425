# Comparing `tmp/keystone_tempest_plugin-0.8.0.tar.gz` & `tmp/keystone_tempest_plugin-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keystone_tempest_plugin-0.8.0.tar", last modified: Mon Sep 13 18:04:00 2021, max compression
+gzip compressed data, was "keystone_tempest_plugin-0.9.0.tar", last modified: Fri Mar 18 16:38:43 2022, max compression
```

## Comparing `keystone_tempest_plugin-0.8.0.tar` & `keystone_tempest_plugin-0.9.0.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:04:00.530200 keystone_tempest_plugin-0.8.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/.testr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2066 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1034 2021-09-13 18:04:00.000000 keystone_tempest_plugin-0.8.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      667 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2695 2021-09-13 18:04:00.000000 keystone_tempest_plugin-0.8.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1504 2021-09-13 18:04:00.530200 keystone_tempest_plugin-0.8.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/babel.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:04:00.514201 keystone_tempest_plugin-0.8.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:04:00.514201 keystone_tempest_plugin-0.8.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2647 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/doc/source/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/doc/source/readme.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/doc/source/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:04:00.514201 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2023 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/clients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3138 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1669 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:04:00.518201 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:04:00.518201 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/services/identity/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/services/identity/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2726 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/services/identity/clients.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:04:00.518201 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/services/identity/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/services/identity/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1545 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/services/identity/v3/auth_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4218 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/services/identity/v3/identity_providers_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5918 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/services/identity/v3/limits_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1461 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/services/identity/v3/mapping_rules_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3204 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/services/identity/v3/saml2_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2668 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/services/identity/v3/service_providers_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:04:00.518201 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:04:00.522201 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:04:00.522201 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/api/identity/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/api/identity/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:04:00.522201 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/api/identity/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/api/identity/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1679 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/api/identity/v3/fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10123 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/api/identity/v3/test_identity_providers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4067 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/api/identity/v3/test_mapping_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11468 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/api/identity/v3/test_oauth1_tokens.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7707 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/api/identity/v3/test_service_providers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2110 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:04:00.522201 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:04:00.530200 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1502 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19520 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_access_rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22940 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_application_credential.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6595 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_consumer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20266 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_credential.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8651 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_domain.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13781 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_domain_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23269 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_ec2_credential.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8965 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_endpoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23291 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_endpoint_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   168690 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_grant.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    59016 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11427 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_identity_provider.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10084 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_implied_role.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14966 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_limit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9349 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_mapping.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8224 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18813 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_policy_association.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21928 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_project.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9776 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_project_endpoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25650 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_project_tag.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12006 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_protocol.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7255 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_region.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8089 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_registered_limit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15499 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_role.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    52954 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_role_assignment.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8457 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9873 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_service_provider.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12086 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23354 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_trust.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23524 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_user.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:04:00.530200 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/scenario/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13531 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/scenario/test_federated_authentication.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:04:00.518201 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1504 2021-09-13 18:04:00.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4264 2021-09-13 18:04:00.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-09-13 18:04:00.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2021-09-13 18:04:00.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-09-13 18:04:00.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-09-13 18:04:00.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2021-09-13 18:04:00.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2021-09-13 18:04:00.000000 keystone_tempest_plugin-0.8.0/keystone_tempest_plugin.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:04:00.510202 keystone_tempest_plugin-0.8.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:04:00.530200 keystone_tempest_plugin-0.8.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/releasenotes/notes/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:04:00.530200 keystone_tempest_plugin-0.8.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:04:00.530200 keystone_tempest_plugin-0.8.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:04:00.530200 keystone_tempest_plugin-0.8.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9124 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      398 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2021-09-13 18:04:00.534200 keystone_tempest_plugin-0.8.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1222 2021-09-13 18:03:25.000000 keystone_tempest_plugin-0.8.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:43.447673 keystone_tempest_plugin-0.9.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/.testr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2214 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1097 2022-03-18 16:38:43.000000 keystone_tempest_plugin-0.9.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      667 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2855 2022-03-18 16:38:43.000000 keystone_tempest_plugin-0.9.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1504 2022-03-18 16:38:43.447673 keystone_tempest_plugin-0.9.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/babel.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:43.423673 keystone_tempest_plugin-0.9.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:43.423673 keystone_tempest_plugin-0.9.0/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2647 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/doc/source/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/doc/source/readme.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/doc/source/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:43.423673 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2023 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/clients.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3138 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1669 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:43.427673 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/services/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:43.427673 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/services/identity/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/services/identity/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2746 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/services/identity/clients.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:43.431673 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/services/identity/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/services/identity/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1545 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/services/identity/v3/auth_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4218 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/services/identity/v3/identity_providers_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5918 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/services/identity/v3/limits_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1461 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/services/identity/v3/mapping_rules_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3204 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/services/identity/v3/saml2_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2668 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/services/identity/v3/service_providers_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:43.431673 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:43.431673 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:43.431673 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/api/identity/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/api/identity/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:43.431673 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/api/identity/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/api/identity/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1679 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/api/identity/v3/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10123 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/api/identity/v3/test_identity_providers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4067 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/api/identity/v3/test_mapping_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11468 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/api/identity/v3/test_oauth1_tokens.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7707 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/api/identity/v3/test_service_providers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2110 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:43.431673 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:43.443673 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1502 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19520 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_access_rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22940 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_application_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6595 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_consumer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20266 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8651 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_domain.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13781 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_domain_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23269 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_ec2_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8965 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_endpoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23291 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_endpoint_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   168690 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_grant.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    59016 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11427 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_identity_provider.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10084 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_implied_role.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14966 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_limit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9349 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_mapping.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8224 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18813 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_policy_association.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21928 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_project.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9776 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_project_endpoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25650 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_project_tag.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12006 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_protocol.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7255 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_region.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8089 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_registered_limit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15499 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_role.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    52954 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_role_assignment.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8457 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9873 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_service_provider.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12086 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23354 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_trust.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23524 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_user.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:43.443673 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/scenario/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13531 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/scenario/test_federated_authentication.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:43.427673 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1504 2022-03-18 16:38:43.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4264 2022-03-18 16:38:43.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-18 16:38:43.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2022-03-18 16:38:43.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-18 16:38:43.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-03-18 16:38:43.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2022-03-18 16:38:43.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2022-03-18 16:38:43.000000 keystone_tempest_plugin-0.9.0/keystone_tempest_plugin.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:43.415673 keystone_tempest_plugin-0.9.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:43.443673 keystone_tempest_plugin-0.9.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/releasenotes/notes/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:43.443673 keystone_tempest_plugin-0.9.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:43.447673 keystone_tempest_plugin-0.9.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:43.447673 keystone_tempest_plugin-0.9.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9124 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      398 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2022-03-18 16:38:43.447673 keystone_tempest_plugin-0.9.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1222 2022-03-18 16:38:08.000000 keystone_tempest_plugin-0.9.0/tox.ini
```

### Comparing `keystone_tempest_plugin-0.8.0/.zuul.yaml` & `keystone_tempest_plugin-0.9.0/.zuul.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -40,34 +40,39 @@
       - tempest-plugin-jobs
     check:
       jobs:
         - keystone-dsvm-py3-functional
         - keystone-dsvm-py3-functional-federation-ubuntu-focal:
             voting: false
         - keystone-dsvm-py3-functional-federation-ubuntu-focal-k2k
+        - keystone-dsvm-py3-functional-wallaby
+        - keystone-dsvm-py3-functional-victoria
         - keystone-dsvm-py3-functional-ussuri
         - keystone-dsvm-py3-functional-train
-        - keystone-dsvm-py3-functional-stein
         - keystone-protection-functional
     gate:
       jobs:
         - keystone-dsvm-py3-functional
         - keystone-dsvm-py3-functional-federation-ubuntu-focal-k2k
         - keystone-protection-functional
 
 - job:
+    name: keystone-dsvm-py3-functional-wallaby
+    parent: keystone-dsvm-py3-functional
+    override-checkout: stable/wallaby
+
+- job:
+    name: keystone-dsvm-py3-functional-victoria
+    parent: keystone-dsvm-py3-functional
+    override-checkout: stable/victoria
+
+- job:
     name: keystone-dsvm-py3-functional-ussuri
     parent: keystone-dsvm-py3-functional
     nodeset: openstack-single-node-bionic
     override-checkout: stable/ussuri
 
 - job:
     name: keystone-dsvm-py3-functional-train
     parent: keystone-dsvm-py3-functional
     nodeset: openstack-single-node-bionic
     override-checkout: stable/train
-
-- job:
-    name: keystone-dsvm-py3-functional-stein
-    parent: keystone-dsvm-py3-functional
-    nodeset: openstack-single-node-bionic
-    override-checkout: stable/stein
```

### Comparing `keystone_tempest_plugin-0.8.0/AUTHORS` & `keystone_tempest_plugin-0.9.0/AUTHORS`

 * *Files 6% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 Chandan Kumar <chkumar@redhat.com>
 Colleen Murphy <colleen.murphy@suse.com>
 Colleen Murphy <colleen.murphy@suse.de>
 Colleen Murphy <colleen@gazlene.net>
 Davanum Srinivas <davanum@gmail.com>
 Dolph Mathews <dolph.mathews@gmail.com>
 Doug Hellmann <doug@doughellmann.com>
+Douglas Viroel <dviroel@redhat.com>
 Ghanshyam Mann <gmann@ghanshyammann.com>
 Hemanth Nakkina <nh863p@att.com>
 Kristi Nikolla <kristi@nikolla.me>
 Lance Bragstad <lbragstad@gmail.com>
 Luong Anh Tuan <tuanla@vn.fujitsu.com>
 Nishant Kumar <nishant.e.kumar@ericsson.com>
 Rodrigo Duarte <rduartes@redhat.com>
 Rodrigo Duarte Sousa <rduartes@redhat.com>
 Ronald De Rose <ronald.de.rose@intel.com>
 Thomas Bechtold <tbechtold@suse.com>
 Vieri <15050873171@163.com>
 Vishakha Agarwal <agarwalvishakha18@gmail.com>
 caoyuan <cao.yuan@99cloud.net>
+gugug <gu.jin@99cloud.net>
 huang.zhiping <huang.zhiping@99cloud.net>
 inspurericzhang <zhanglf01@inspur.com>
 lvxianguo <lvxianguo@inspur.com>
 pengyuesheng <pengyuesheng@gohighsec.com>
 wangxiyuan <wangxiyuan1007@gmail.com>
```

### Comparing `keystone_tempest_plugin-0.8.0/CONTRIBUTING.rst` & `keystone_tempest_plugin-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/ChangeLog` & `keystone_tempest_plugin-0.9.0/ChangeLog`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGES
 =======
 
+0.9.0
+-----
+
+* Replace Identity client endpoint type
+* Add victoria/wallaby stable branch jobs on master gate
+
 0.8.0
 -----
 
 * Increase protection testing for application credentials
 
 0.7.0
 -----
@@ -13,14 +19,15 @@
 * Update federation jobs to use ubuntu focal
 
 0.6.0
 -----
 
 * [goal] Migrate keystone-tempest-plugin jobs to focal
 * Add tempest clients for limits
+* Replace assertItemsEqual with assertCountEqual
 * Update docs building, cleanup
 * Add addCleanup just after resource creation
 * Use ephemeral test user for k2k tests
 * Add stable branches testing on keystone-tempest-plugin master gate
 * Remove func not in use in test\_service\_providers
 * Don't test openstack\_groups on stable branches
```

### Comparing `keystone_tempest_plugin-0.8.0/LICENSE` & `keystone_tempest_plugin-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/PKG-INFO` & `keystone_tempest_plugin-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: keystone_tempest_plugin
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tempest plugin keystone_tempest_plugin
 Home-page: https://docs.openstack.org/keystone/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =======================
         keystone-tempest-plugin
```

### Comparing `keystone_tempest_plugin-0.8.0/README.rst` & `keystone_tempest_plugin-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/doc/source/conf.py` & `keystone_tempest_plugin-0.9.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/clients.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/clients.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/config.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/config.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/plugin.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/services/identity/clients.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/services/identity/clients.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     api_version = 'v3'
 
     def __init__(self, auth_provider):
         super(Identity, self).__init__(
             auth_provider,
             SERVICE_TYPE,
             CONF.identity.region,
-            endpoint_type='adminURL')
+            endpoint_type=CONF.identity.v3_endpoint_type)
 
 
 class Federation(Identity):
     """Tempest REST client for keystone's Federated Identity API."""
 
     subpath_prefix = 'OS-FEDERATION'
     subpath_suffix = None
```

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/services/identity/v3/auth_client.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/services/identity/v3/auth_client.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/services/identity/v3/identity_providers_client.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/services/identity/v3/identity_providers_client.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/services/identity/v3/limits_client.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/services/identity/v3/limits_client.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/services/identity/v3/mapping_rules_client.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/services/identity/v3/mapping_rules_client.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/services/identity/v3/saml2_client.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/services/identity/v3/saml2_client.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/services/identity/v3/service_providers_client.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/services/identity/v3/service_providers_client.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/api/identity/v3/fixtures.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/api/identity/v3/fixtures.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/api/identity/v3/test_identity_providers.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/api/identity/v3/test_identity_providers.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         if idp_ref:
             self.assertEqual(idp_ref['description'], idp['description'])
 
             if 'enabled' in idp_ref:
                 self.assertEqual(idp_ref['enabled'], idp['enabled'])
 
             if 'remote_ids' in idp_ref:
-                self.assertItemsEqual(idp_ref['remote_ids'], idp['remote_ids'])
+                self.assertCountEqual(idp_ref['remote_ids'], idp['remote_ids'])
 
     def _create_idp(self, idp_id, idp_ref):
         idp = self.idps_client.create_identity_provider(
             idp_id, **idp_ref)['identity_provider']
         if not idp_ref.get('domain_id'):
             self.addCleanup(
                 self.keystone_manager.domains_client.delete_domain,
```

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/api/identity/v3/test_mapping_rules.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/api/identity/v3/test_mapping_rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                                          mapping_ref=None):
         self.assertIn('id', mapping)
         self.assertEqual(mapping_id, mapping['id'])
 
         self.assertIn('rules', mapping)
 
         if mapping_ref:
-            self.assertItemsEqual(mapping_ref['rules'], mapping['rules'])
+            self.assertCountEqual(mapping_ref['rules'], mapping['rules'])
 
     def _create_mapping_rule(self, mapping_id, mapping_ref):
         mapping = self.mappings_client.create_mapping_rule(
             mapping_id, mapping_ref)['mapping']
         self.addCleanup(self.mappings_client.delete_mapping_rule, mapping_id)
         return mapping
```

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/api/identity/v3/test_oauth1_tokens.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/api/identity/v3/test_oauth1_tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,15 +215,15 @@
             user_id, access_token['oauth_token'])['roles']
         fetched_role_ids = [role['id'] for role in fetched_roles]
         roles = self.roles_client.list_user_roles_on_project(
             project_id, user_id)
         role_ids = [role['id'] for role in roles['roles']]
 
         # check that role ids matches
-        self.assertItemsEqual(fetched_role_ids, role_ids)
+        self.assertCountEqual(fetched_role_ids, role_ids)
 
     @decorators.idempotent_id('28aee994-86b1-4596-a652-572f558045e7')
     def test_show_role_for_access_token(self):
         """Test to show role details for an access token."""
         consumer = self._create_consumer()
         access_token = self._create_access_token(consumer)
```

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/api/identity/v3/test_service_providers.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/api/identity/v3/test_service_providers.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/base.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/base.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/base.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/base.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_access_rule.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_access_rule.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_application_credential.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_application_credential.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_consumer.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_consumer.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_credential.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_credential.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_domain.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_domain.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_domain_config.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_domain_config.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_ec2_credential.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_ec2_credential.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_endpoint.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_endpoint_group.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_endpoint_group.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_grant.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_grant.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_group.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_group.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_identity_provider.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_identity_provider.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_implied_role.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_implied_role.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_limit.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_limit.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_mapping.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_mapping.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_policy.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_policy.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_policy_association.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_policy_association.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_project.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_project.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_project_endpoint.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_project_endpoint.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_project_tag.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_project_tag.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_protocol.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_protocol.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_region.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_region.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_registered_limit.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_registered_limit.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_role.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_role.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_role_assignment.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_role_assignment.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_service.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_service.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_service_provider.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_service_provider.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_token.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_token.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_trust.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_trust.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/rbac/v3/test_user.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/rbac/v3/test_user.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin/tests/scenario/test_federated_authentication.py` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin/tests/scenario/test_federated_authentication.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin.egg-info/PKG-INFO` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: keystone-tempest-plugin
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tempest plugin keystone_tempest_plugin
 Home-page: https://docs.openstack.org/keystone/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =======================
         keystone-tempest-plugin
```

### Comparing `keystone_tempest_plugin-0.8.0/keystone_tempest_plugin.egg-info/SOURCES.txt` & `keystone_tempest_plugin-0.9.0/keystone_tempest_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/releasenotes/source/conf.py` & `keystone_tempest_plugin-0.9.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/setup.cfg` & `keystone_tempest_plugin-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/setup.py` & `keystone_tempest_plugin-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `keystone_tempest_plugin-0.8.0/tox.ini` & `keystone_tempest_plugin-0.9.0/tox.ini`

 * *Files identical despite different names*

