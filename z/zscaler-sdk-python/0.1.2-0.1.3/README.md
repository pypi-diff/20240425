# Comparing `tmp/zscaler-sdk-python-0.1.2.tar.gz` & `tmp/zscaler_sdk_python-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zscaler-sdk-python-0.1.2.tar", last modified: Sat Apr 20 22:57:24 2024, max compression
+gzip compressed data, was "zscaler_sdk_python-0.1.3.tar", max compression
```

## Comparing `zscaler-sdk-python-0.1.2.tar` & `zscaler_sdk_python-0.1.3.tar`

### file list

```diff
@@ -1,213 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.284349 zscaler-sdk-python-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16375 2024-04-20 22:57:24.284349 zscaler-sdk-python-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15600 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.252349 zscaler-sdk-python-0.1.2/docsrc/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.252349 zscaler-sdk-python-0.1.2/docsrc/zs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.256349 zscaler-sdk-python-0.1.2/docsrc/zs/guides/
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/guides/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/guides/support.rst
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/guides/troubleshooting.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.260349 zscaler-sdk-python-0.1.2/docsrc/zs/zia/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/activate.rst
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/admin_and_role_management.rst
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/apptotal.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/audit_logs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/authentication_settings.rst
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/cloud_apps.rst
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/device_management.rst
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/dlp.rst
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/firewall.rst
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/forwarding_control.rst
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/isolation_profile.rst
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/locations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/rule_labels.rst
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/sandbox.rst
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/security.rst
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/ssl_inspection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/traffic.rst
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/url_categories.rst
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/url_filtering.rst
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/users.rst
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/web_dlp.rst
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/workload_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/zpa_gateway.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.264349 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/app_segments.rst
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/app_segments_inspection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/app_segments_pra.rst
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/certificates.rst
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/cloud_connector_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/connectors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/emergency_access.rst
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/idp.rst
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/inspection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/isolation_profile.rst
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/lss.rst
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/machine_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/policies.rst
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/posture_profiles.rst
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/privileged_remote_access.rst
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/provisioning.rst
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/saml_attributes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/scim_attributes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/scim_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/segment_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/server_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/servers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/service_edges.rst
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/trusted_networks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-20 22:57:24.284349 zscaler-sdk-python-0.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1750 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.264349 zscaler-sdk-python-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.252349 zscaler-sdk-python-0.1.2/tests/integration/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.268349 zscaler-sdk-python-0.1.2/tests/integration/zia/
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_admin_and_role_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_authentication_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_cloud_firewall_ip_destination_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_cloud_firewall_ip_source_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_cloud_firewall_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_dlp_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_dlp_engines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_dlp_icap_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_dlp_idm_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_dlp_incident_receiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_dlp_web_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_isolation_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_location_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    14311 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_location_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_rule_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_security.py
--rw-r--r--   0 runner    (1001) docker     (127)    15623 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_traffic_gre_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_traffic_static_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_traffic_vpn_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_url_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_url_filtering_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.272349 zscaler-sdk-python-0.1.2/tests/integration/zpa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_access_policy_forwarding_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_access_policy_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_access_policy_timeout_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_app_connector_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_application_segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_application_servers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_ba_certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_enrolment_certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_idp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_isolation_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_machine_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_posture_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_pra_approval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_pra_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_pra_portal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_provisioning_key_app_connector_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_provisioning_key_service_edge_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_saml_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_scim_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_scim_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_segment_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_server_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_service_edge_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_trusted_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.272349 zscaler-sdk-python-0.1.2/zscaler/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.272349 zscaler-sdk-python-0.1.2/zscaler/cache/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/cache/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/cache/no_op_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/cache/zscaler_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.272349 zscaler-sdk-python-0.1.2/zscaler/errors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/errors/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/errors/http_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/errors/zscaler_api_error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.272349 zscaler-sdk-python-0.1.2/zscaler/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/exceptions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.272349 zscaler-sdk-python-0.1.2/zscaler/ratelimiter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/ratelimiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/ratelimiter/ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/user_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    19443 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.280349 zscaler-sdk-python-0.1.2/zscaler/zia/
--rw-r--r--   0 runner    (1001) docker     (127)    22024 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/activate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14276 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/admin_and_role_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/apptotal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/authentication_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18549 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/cloud_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/device_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    27797 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/dlp.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    40386 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    11754 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/forwarding_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/isolation_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)    30972 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/ssl_inspection.py
--rw-r--r--   0 runner    (1001) docker     (127)    31149 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/traffic.py
--rw-r--r--   0 runner    (1001) docker     (127)    14744 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/url_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/url_filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/users.py
--rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/web_dlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/workload_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/zpa_gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.284349 zscaler-sdk-python-0.1.2/zscaler/zpa/
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    24790 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13393 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/app_segments.py
--rw-r--r--   0 runner    (1001) docker     (127)    12657 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/app_segments_inspection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12217 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/app_segments_pra.py
--rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/cloud_connector_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    20602 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/connectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/emergency_access.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/idp.py
--rw-r--r--   0 runner    (1001) docker     (127)    34889 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/inspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/isolation_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    21471 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/lss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/machine_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    30654 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/posture_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    32581 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/privileged_remote_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/provisioning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/saml_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/scim_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/scim_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/segment_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/server_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/servers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15606 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/service_edges.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/trusted_networks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.284349 zscaler-sdk-python-0.1.2/zscaler_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16375 2024-04-20 22:57:24.000000 zscaler-sdk-python-0.1.2/zscaler_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-04-20 22:57:24.000000 zscaler-sdk-python-0.1.2/zscaler_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 22:57:24.000000 zscaler-sdk-python-0.1.2/zscaler_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-20 22:57:24.000000 zscaler-sdk-python-0.1.2/zscaler_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 22:57:24.000000 zscaler-sdk-python-0.1.2/zscaler_sdk_python.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1113 2024-04-25 03:50:00.568967 zscaler_sdk_python-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0    15600 2024-04-25 03:50:00.568967 zscaler_sdk_python-0.1.3/README.md
+-rw-r--r--   0        0        0     2290 2024-04-25 03:50:53.977218 zscaler_sdk_python-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1278 2024-04-25 03:50:53.985218 zscaler_sdk_python-0.1.3/zscaler/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/cache/__init__.py
+-rw-r--r--   0        0        0     3195 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/cache/cache.py
+-rw-r--r--   0        0        0     1479 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/cache/no_op_cache.py
+-rw-r--r--   0        0        0     4967 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/cache/zscaler_cache.py
+-rw-r--r--   0        0        0      738 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/constants.py
+-rw-r--r--   0        0        0        0 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/errors/__init__.py
+-rw-r--r--   0        0        0      172 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/errors/error.py
+-rw-r--r--   0        0        0      638 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/errors/http_error.py
+-rw-r--r--   0        0        0      628 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/errors/zscaler_api_error.py
+-rw-r--r--   0        0        0       63 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/exceptions/__init__.py
+-rw-r--r--   0        0        0     2025 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/exceptions/exceptions.py
+-rw-r--r--   0        0        0     2099 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/logger.py
+-rw-r--r--   0        0        0        0 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/ratelimiter/__init__.py
+-rw-r--r--   0        0        0     1473 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/ratelimiter/ratelimiter.py
+-rw-r--r--   0        0        0      639 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/user_agent.py
+-rw-r--r--   0        0        0    19073 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/utils.py
+-rw-r--r--   0        0        0    21568 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/__init__.py
+-rw-r--r--   0        0        0     1534 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/activate.py
+-rw-r--r--   0        0        0    14194 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/admin_and_role_management.py
+-rw-r--r--   0        0        0     2372 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/apptotal.py
+-rw-r--r--   0        0        0     2992 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/audit_logs.py
+-rw-r--r--   0        0        0     3140 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/authentication_settings.py
+-rw-r--r--   0        0        0     2754 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/client.py
+-rw-r--r--   0        0        0    18513 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/cloud_apps.py
+-rw-r--r--   0        0        0     2872 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/device_management.py
+-rw-r--r--   0        0        0    27473 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/dlp.py
+-rw-r--r--   0        0        0      794 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/errors.py
+-rw-r--r--   0        0        0    39908 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/firewall.py
+-rw-r--r--   0        0        0    11686 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/forwarding_control.py
+-rw-r--r--   0        0        0     2909 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/isolation_profile.py
+-rw-r--r--   0        0        0     5835 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/labels.py
+-rw-r--r--   0        0        0    30762 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/locations.py
+-rw-r--r--   0        0        0     6724 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/sandbox.py
+-rw-r--r--   0        0        0     6792 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/security.py
+-rw-r--r--   0        0        0     5298 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/ssl_inspection.py
+-rw-r--r--   0        0        0    30729 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/traffic.py
+-rw-r--r--   0        0        0    14484 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zia/url_categories.py
+-rw-r--r--   0        0        0    14319 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zia/url_filtering.py
+-rw-r--r--   0        0        0    13735 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zia/users.py
+-rw-r--r--   0        0        0    12376 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zia/web_dlp.py
+-rw-r--r--   0        0        0     1897 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zia/workload_groups.py
+-rw-r--r--   0        0        0     6842 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zia/zpa_gateway.py
+-rw-r--r--   0        0        0     2709 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/README.md
+-rw-r--r--   0        0        0    24300 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/__init__.py
+-rw-r--r--   0        0        0    13187 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/app_segments.py
+-rw-r--r--   0        0        0    12445 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/app_segments_inspection.py
+-rw-r--r--   0        0        0    12019 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/app_segments_pra.py
+-rw-r--r--   0        0        0     7942 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/certificates.py
+-rw-r--r--   0        0        0     3804 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/client.py
+-rw-r--r--   0        0        0     2667 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/cloud_connector_groups.py
+-rw-r--r--   0        0        0    20370 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/connectors.py
+-rw-r--r--   0        0        0     6189 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/emergency_access.py
+-rw-r--r--   0        0        0      844 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/errors.py
+-rw-r--r--   0        0        0     2764 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/idp.py
+-rw-r--r--   0        0        0    34309 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/inspection.py
+-rw-r--r--   0        0        0     3176 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/isolation_profile.py
+-rw-r--r--   0        0        0    21113 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/lss.py
+-rw-r--r--   0        0        0     2734 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/machine_groups.py
+-rw-r--r--   0        0        0    30350 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/policies.py
+-rw-r--r--   0        0        0     4317 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/posture_profiles.py
+-rw-r--r--   0        0        0    32017 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/privileged_remote_access.py
+-rw-r--r--   0        0        0     9887 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/provisioning.py
+-rw-r--r--   0        0        0     3632 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/saml_attributes.py
+-rw-r--r--   0        0        0     4172 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/scim_attributes.py
+-rw-r--r--   0        0        0     5041 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/scim_groups.py
+-rw-r--r--   0        0        0     6103 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/segment_groups.py
+-rw-r--r--   0        0        0     7776 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/server_groups.py
+-rw-r--r--   0        0        0     6477 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/servers.py
+-rw-r--r--   0        0        0    15428 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/service_edges.py
+-rw-r--r--   0        0        0     4377 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/trusted_networks.py
+-rw-r--r--   0        0        0    17368 1970-01-01 00:00:00.000000 zscaler_sdk_python-0.1.3/PKG-INFO
```

### Comparing `zscaler-sdk-python-0.1.2/LICENSE.md` & `zscaler_sdk_python-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.2/PKG-INFO` & `zscaler_sdk_python-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: zscaler-sdk-python
-Version: 0.1.2
-Summary: Official Python SDK for the Zscaler Products (Beta)
-Home-page: https://zscaler-sdk-python.readthedocs.io
-Author: Zscaler, Inc.
-Author-email: devrel@zscaler.com
-Keywords: zscaler,sdk,zpa,zia,zdx,zcc,zcon
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8,<4.0
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.md
-
 # Official Python SDK for the Zscaler Products (Beta)
 
 [![PyPI - Downloads](https://img.shields.io/pypi/dw/zscaler-sdk-python)](https://pypistats.org/packages/zscaler-sdk-python)
 [![License](https://img.shields.io/github/license/zscaler/zscaler-sdk-python.svg)](https://github.com/zscaler/zscaler-sdk-python)
 [![Documentation Status](https://readthedocs.org/projects/zscaler-sdk-python/badge/?version=latest)](https://zscaler-sdk-python.readthedocs.io/en/latest/?badge=latest)
 [![Latest version released on PyPi](https://img.shields.io/pypi/v/zscaler-sdk-python.svg)](https://pypi.org/project/zscaler-sdk-python)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/zscaler-sdk-python.svg)](https://pypi.python.org/pypi/zscaler-sdk-python/)
```

### Comparing `zscaler-sdk-python-0.1.2/README.md` & `zscaler_sdk_python-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,56 @@
+Metadata-Version: 2.1
+Name: zscaler-sdk-python
+Version: 0.1.3
+Summary: Official Python SDK for the Zscaler Products (Beta)
+Home-page: https://github.com/zscaler/zscaler-sdk-python
+License: MIT
+Keywords: zscaler,sdk,zpa,zia,zdx,zcc,zcon
+Author: Zscaler, Inc.
+Author-email: devrel@zscaler.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Security
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: dev
+Requires-Dist: aenum ; extra == "dev"
+Requires-Dist: arrow
+Requires-Dist: black (>=24.4.1,<25.0.0) ; extra == "dev"
+Requires-Dist: certifi
+Requires-Dist: charset-normalizer
+Requires-Dist: flake8
+Requires-Dist: flatdict
+Requires-Dist: idna
+Requires-Dist: pycryptodomex
+Requires-Dist: pydash ; extra == "dev"
+Requires-Dist: python-box (>=5.4,<6.0)
+Requires-Dist: python-dateutil
+Requires-Dist: pytz
+Requires-Dist: pyyaml
+Requires-Dist: requests
+Requires-Dist: responses
+Requires-Dist: restfly
+Requires-Dist: six
+Requires-Dist: urllib3
+Requires-Dist: xmltodict
+Requires-Dist: yarl
+Project-URL: Bug Tracker, https://github.com/zscaler/zscaler-sdk-python/issues
+Project-URL: Documentation, https://zscaler-sdk-python.readthedocs.io
+Project-URL: Repository, https://github.com/zscaler/zscaler-sdk-python
+Description-Content-Type: text/markdown
+
 # Official Python SDK for the Zscaler Products (Beta)
 
 [![PyPI - Downloads](https://img.shields.io/pypi/dw/zscaler-sdk-python)](https://pypistats.org/packages/zscaler-sdk-python)
 [![License](https://img.shields.io/github/license/zscaler/zscaler-sdk-python.svg)](https://github.com/zscaler/zscaler-sdk-python)
 [![Documentation Status](https://readthedocs.org/projects/zscaler-sdk-python/badge/?version=latest)](https://zscaler-sdk-python.readthedocs.io/en/latest/?badge=latest)
 [![Latest version released on PyPi](https://img.shields.io/pypi/v/zscaler-sdk-python.svg)](https://pypi.org/project/zscaler-sdk-python)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/zscaler-sdk-python.svg)](https://pypi.python.org/pypi/zscaler-sdk-python/)
@@ -306,7 +355,8 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
+
```

### Comparing `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_machine_groups.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/machine_groups.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,73 +10,70 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
+from box import Box, BoxList
+from requests import Response
 
-import pytest
+from . import ZPAClient
 
-from tests.integration.zpa.conftest import MockZPAClient
 
-
-@pytest.fixture
-def fs():
-    yield
-
-
-class TestMachineGroups:
-    """
-    Integration Tests for the Machine Groups.
-    """
-
-    def test_machine_groups(self, fs):
-        client = MockZPAClient(fs)
-        errors = []  # Initialize an empty list to collect errors
-
-        # Attempt to list all machine groups
-        try:
-            machine_groups = client.machine_groups.list_groups()
-            assert isinstance(machine_groups, list), "Expected a list of machine groups"
-        except Exception as exc:
-            errors.append(f"Listing machine groups failed: {str(exc)}")
-
-        # Process each machine group if the list is not empty
-        if machine_groups:
-            for first_group in machine_groups:
-                group_id = first_group.get("id")
-
-                # Fetch the selected machine group by its ID
-                try:
-                    fetched_group = client.machine_groups.get_group(group_id)
-                    assert (
-                        fetched_group is not None
-                    ), "Expected a valid machine group object"
-                    assert (
-                        fetched_group.get("id") == group_id
-                    ), "Mismatch in machine group ID"
-                except Exception as exc:
-                    errors.append(f"Fetching machine group by ID failed: {str(exc)}")
-
-                # Attempt to retrieve the machine group by name
-                try:
-                    group_name = first_group.get("name")
-                    group_by_name = client.machine_groups.get_machine_group_by_name(
-                        group_name
-                    )
-                    assert (
-                        group_by_name is not None
-                    ), "Expected a valid machine group object when searching by name"
-                    assert (
-                        group_by_name.get("id") == group_id
-                    ), "Mismatch in machine group ID when searching by name"
-                except Exception as exc:
-                    errors.append(f"Fetching machine group by name failed: {str(exc)}")
-
-                # Once we've tested one group, exit the loop to avoid redundant testing
-                break
-
-        # Assert that no errors occurred during the test
-        assert (
-            len(errors) == 0
-        ), f"Errors occurred during machine group operations test: {errors}"
+class MachineGroupsAPI:
+    def __init__(self, client: ZPAClient):
+        self.rest = client
+
+    def list_groups(self, **kwargs) -> BoxList:
+        """
+        Returns a list of all configured machine groups.
+
+        Keyword Args:
+            **max_items (int):
+                The maximum number of items to request before stopping iteration.
+            **max_pages (int):
+                The maximum number of pages to request before stopping iteration.
+            **pagesize (int):
+                Specifies the page size. The default size is 20, but the maximum size is 500.
+            **search (str, optional):
+                The search string used to match against features and fields.
+
+        Returns:
+            :obj:`list`: A list of all configured machine groups.
+
+        Examples:
+            >>> for machine_group in zpa.machine_groups.list_groups():
+            ...    pprint(machine_group)
+
+        """
+        list, _ = self.rest.get_paginated_data(path="/machineGroup", **kwargs)
+        return list
+
+    def get_group(self, group_id: str) -> Box:
+        """
+        Returns information on the specified machine group.
+
+        Args:
+            group_id (str):
+                The unique identifier for the machine group.
+
+        Returns:
+            :obj:`Box`: The resource record for the machine group.
+
+        Examples:
+            >>> pprint(zpa.machine_groups.get_group('99999'))
+
+        """
+        response = self.rest.get("/machineGroup/%s" % (group_id))
+        if isinstance(response, Response):
+            status_code = response.status_code
+            if status_code != 200:
+                return None
+        return response
+
+    def get_machine_group_by_name(self, name):
+        apps = self.list_groups()
+        for app in apps:
+            if app.get("name") == name:
+                return app
+        return None
```

### Comparing `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_posture_profiles.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/isolation_profile.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,76 +11,75 @@
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 
-import pytest
+from box import BoxList
 
-from tests.integration.zpa.conftest import MockZPAClient
+from zscaler.zpa.client import ZPAClient
 
 
-@pytest.fixture
-def fs():
-    yield
-
-
-class TestPostureProfile:
-    """
-    Integration Tests for the Posture Profile.
-    """
-
-    def test_posture_profile(self, fs):
-        client = MockZPAClient(fs)
-        errors = []  # Initialize an empty list to collect errors
-
-        # Attempt to list all posture profiles
-        try:
-            posture_profile = client.posture_profiles.list_profiles()
-            assert isinstance(
-                posture_profile, list
-            ), "Expected a list of posture profiles"
-        except Exception as exc:
-            errors.append(f"Listing posture profiles failed: {str(exc)}")
-
-        # Process each posture profile if the list is not empty
-        if posture_profile:
-            for first_profile in posture_profile:
-                profile_id = first_profile.get("id")
-
-                # Fetch the selected posture profile by its ID
-                try:
-                    fetched_profile = client.posture_profiles.get_profile(profile_id)
-                    assert (
-                        fetched_profile is not None
-                    ), "Expected a valid posture profile object"
-                    assert (
-                        fetched_profile.get("id") == profile_id
-                    ), "Mismatch in posture profile ID"
-                except Exception as exc:
-                    errors.append(f"Fetching posture profile by ID failed: {str(exc)}")
-
-                # Attempt to retrieve the posture profile by name
-                try:
-                    profile_name = first_profile.get("name")
-                    profile_by_name = client.posture_profiles.get_profile_by_name(
-                        profile_name
-                    )
-                    assert (
-                        profile_by_name is not None
-                    ), "Expected a valid posture profile object when searching by name"
-                    assert (
-                        profile_by_name.get("id") == profile_id
-                    ), "Mismatch in posture profile ID when searching by name"
-                except Exception as exc:
-                    errors.append(
-                        f"Fetching posture profile by name failed: {str(exc)}"
-                    )
-
-                # Once we've tested one profile, exit the loop to avoid redundant testing
-                break
-
-        # Assert that no errors occurred during the test
-        assert (
-            len(errors) == 0
-        ), f"Errors occurred during posture profile operations test: {errors}"
+class IsolationProfileAPI:
+    def __init__(self, client: ZPAClient):
+        self.rest = client
+
+    def list_profiles(self, **kwargs) -> BoxList:
+        """
+        Returns a list of all configured isolation profiles.
+
+        Keyword Args:
+            max_items (int): The maximum number of items to request before stopping iteration.
+            max_pages (int): The maximum number of pages to request before stopping iteration.
+            pagesize (int): Specifies the page size. The default size is 20, but the maximum size is 500.
+            search (str, optional): The search string used to match against features and fields.
+
+        Returns:
+            BoxList: A list of all configured isolation profiles.
+
+        Examples:
+            >>> for isolation_profile in zpa.isolation_profiles.list_profiles():
+            ...     pprint(isolation_profile)
+        """
+        list, _ = self.rest.get_paginated_data(path="/isolation/profiles", **kwargs)
+        return list
+
+    def get_profile_by_name(self, name: str):
+        """
+        Retrieves a specific isolation profile by its name.
+
+        Args:
+            name (str): The name of the isolation profile to search for.
+
+        Returns:
+            dict or None: The isolation profile with the specified name if found, otherwise None.
+
+        Examples:
+            >>> profile = zpa.isolation_profiles.get_profile_by_name('DefaultProfile')
+            >>> print(profile)
+        """
+        profiles = self.list_profiles()
+        for profile in profiles:
+            if profile.get("name") == name:
+                return profile
+        return None
+
+    def get_profile_by_id(self, profile_id: str):
+        """
+        Retrieves a specific isolation profile by its unique identifier (ID).
+
+        Args:
+            profile_id (str): The ID of the isolation profile to retrieve.
+
+        Returns:
+            dict or None: The isolation profile with the specified ID if found, otherwise None.
+
+        Examples:
+            >>> profile = zpa.isolation_profiles.get_profile_by_id('12345')
+            >>> print(profile)
+        """
+        profiles = self.list_profiles()
+        for profile in profiles:
+            if str(profile.get("id")) == str(profile_id):  # Ensuring ID comparison as strings
+                return profile
+        return None
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/__init__.py` & `zscaler_sdk_python-0.1.3/zscaler/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,17 +10,26 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
+"""Official Python SDK for the Zscaler Products (Beta)
+
+Zscaler SDK Python is an SDK that provides a uniform and easy-to-use 
+interface for each of the Zscaler product APIs.
+
+Documentation available at https://zscaler-sdk-python.readthedocs.io
+
+"""
+
 __author__ = "Zscaler Inc"
 __email__ = "devrel@zscaler.com"
 __license__ = "MIT"
 __contributors__ = [
     "William Guilherme",
 ]
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 from zscaler.zia import ZIAClientHelper  # noqa
 from zscaler.zpa import ZPAClientHelper  # noqa
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/cache/cache.py` & `zscaler_sdk_python-0.1.3/zscaler/cache/cache.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.2/zscaler/cache/no_op_cache.py` & `zscaler_sdk_python-0.1.3/zscaler/cache/no_op_cache.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import logging
 
 from zscaler.cache.cache import Cache
 
 # Setting up the logger
-logging.basicConfig(
-    level=logging.DEBUG, format="%(asctime)s - %(levelname)s - %(message)s"
-)
+logging.basicConfig(level=logging.DEBUG, format="%(asctime)s - %(levelname)s - %(message)s")
 
 
 class NoOpCache(Cache):
     """
     This is a disabled Cache Class where no operations occur
     in the cache.
     Implementing the zscaler.cache.cache.Cache abstract class.
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/cache/zscaler_cache.py` & `zscaler_sdk_python-0.1.3/zscaler/cache/zscaler_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,17 +103,15 @@
             del self._store[key]
             logger.info(f'Removed value from cache for key "{key}".')
         url_object = urlparse(key)
         base_url = f"{url_object.netloc}{url_object.path}"
         for other_key in self._store.keys():
             other_url_object = urlparse(other_key)
             other_base_url = f"{other_url_object.netloc}{other_url_object.path}"
-            if not self._is_valid_entry(
-                self._store[other_key]
-            ) and other_base_url.startswith(base_url):
+            if not self._is_valid_entry(self._store[other_key]) and other_base_url.startswith(base_url):
                 del self._store[other_key]
                 logger.info(f'Removed also value from cache for key "{other_key}".')
 
     def clear(self):
         """
         Clear the cache.
         """
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/constants.py` & `zscaler_sdk_python-0.1.3/zscaler/constants.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.2/zscaler/errors/http_error.py` & `zscaler_sdk_python-0.1.3/zscaler/errors/http_error.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.2/zscaler/errors/zscaler_api_error.py` & `zscaler_sdk_python-0.1.3/zscaler/errors/zscaler_api_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,11 @@
 
         params_string = ", ".join(self.params)
 
         self.url = url
         self.headers = response_details.headers
         self.stack = ""
 
-        self.message = (
-            f"ZPA HTTP {self.status} {self.error_id} "
-            f"{self.reason}\nParameters: {params_string}"
-        )
+        self.message = f"ZPA HTTP {self.status} {self.error_id} " f"{self.reason}\nParameters: {params_string}"
 
 
 # ZIA API Errors
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/exceptions/exceptions.py` & `zscaler_sdk_python-0.1.3/zscaler/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.2/zscaler/logger.py` & `zscaler_sdk_python-0.1.3/zscaler/logger.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.2/zscaler/ratelimiter/ratelimiter.py` & `zscaler_sdk_python-0.1.3/zscaler/ratelimiter/ratelimiter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import threading
 import time
 
 
 class RateLimiter:
-    def __init__(
-        self, get_limit, post_put_delete_limit, get_freq, post_put_delete_freq
-    ):
+    def __init__(self, get_limit, post_put_delete_limit, get_freq, post_put_delete_freq):
         self.lock = threading.Lock()
         self.get_requests = []
         self.post_put_delete_requests = []
         self.get_limit = get_limit
         self.post_put_delete_limit = post_put_delete_limit
         self.get_freq = get_freq
         self.post_put_delete_freq = post_put_delete_freq
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/user_agent.py` & `zscaler_sdk_python-0.1.3/zscaler/user_agent.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,16 +8,14 @@
     PYTHON = "python"
 
     def __init__(self, user_agent_extra=None):
         python_version = platform.python_version()
         os_name = platform.system()
         os_version = platform.release()
         self._user_agent_string = (
-            f"{UserAgent.SDK_NAME}/{VERSION} "
-            f"{UserAgent.PYTHON}/{python_version} "
-            f"{os_name}/{os_version}"
+            f"{UserAgent.SDK_NAME}/{VERSION} " f"{UserAgent.PYTHON}/{python_version} " f"{os_name}/{os_version}"
         )
         if user_agent_extra:
             self._user_agent_string += f" {user_agent_extra}"
 
     def get_user_agent_string(self):
         return self._user_agent_string
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/utils.py` & `zscaler_sdk_python-0.1.3/zscaler/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,15 @@
     if isinstance(data, (list, BoxList)):
         return [convert_keys_to_snake(inner_dict) for inner_dict in data]
     elif isinstance(data, (dict, Box)):
         new_dict = {}
         for k in data.keys():
             v = data[k]
             new_key = camel_to_snake(k)
-            new_dict[new_key] = (
-                convert_keys_to_snake(v) if isinstance(v, (dict, list)) else v
-            )
+            new_dict[new_key] = convert_keys_to_snake(v) if isinstance(v, (dict, list)) else v
         return new_dict
     else:
         return data
 
 
 def camel_to_snake(name: str):
     """Converts Python camelCase to Zscaler's lower snake_case."""
@@ -88,18 +86,15 @@
     }
     return edge_cases.get(name, name[0].lower() + name.title()[1:].replace("_", ""))
 
 
 def recursive_snake_to_camel(data):
     """Recursively convert dictionary keys from snake_case to camelCase."""
     if isinstance(data, dict):
-        return {
-            snake_to_camel(key): recursive_snake_to_camel(value)
-            for key, value in data.items()
-        }
+        return {snake_to_camel(key): recursive_snake_to_camel(value) for key, value in data.items()}
     elif isinstance(data, list):
         return [recursive_snake_to_camel(item) for item in data]
     else:
         return data
 
 
 def chunker(lst, n):
@@ -152,17 +147,15 @@
     return
 
 
 def transform_common_id_fields(id_groups: list, kwargs: dict, payload: dict):
     for entry in id_groups:
         if kwargs.get(entry[0]):
             # Ensure each ID is treated as an integer before adding it to the payload
-            payload[entry[1]] = [
-                {"id": int(param_id)} for param_id in kwargs.pop(entry[0])
-            ]
+            payload[entry[1]] = [{"id": int(param_id)} for param_id in kwargs.pop(entry[0])]
     return
 
 
 def transform_clientless_apps(clientless_app_ids):
     transformed_apps = []
     for app in clientless_app_ids:
         # Transform each attribute in app as needed by your API
@@ -245,19 +238,15 @@
         requests.Response:
             If neither flag is True, or if the response isn't JSON data, then
             a response object is returned (pass-through).
     """
     if response.status_code > 299:
         return response
     content_type = response.headers.get("content-type", "application/json")
-    if (
-        (conv_json or conv_box)
-        and "application/json" in content_type.lower()
-        and len(response.text) > 0
-    ):  # noqa: E124
+    if (conv_json or conv_box) and "application/json" in content_type.lower() and len(response.text) > 0:  # noqa: E124
         if conv_box:
             data = convert_keys_to_snake(response.json())
             if isinstance(data, list):
                 return BoxList(data, **box_attrs)
             elif isinstance(data, dict):
                 return Box(data, **box_attrs)
         elif conv_json:
@@ -359,32 +348,26 @@
     def decorator(f):
         def wrapper(*args, **kwargs):
             x = 0
             while True:
                 resp = f(*args, **kwargs)
 
                 # Check if it's a successful status code, 400, or if it shouldn't be retried
-                if (
-                    299 >= resp.status_code >= 200
-                    or resp.status_code == 400
-                    or not should_retry(resp.status_code)
-                ):
+                if 299 >= resp.status_code >= 200 or resp.status_code == 400 or not should_retry(resp.status_code):
                     return resp
 
                 if x == retries:
                     try:
                         error_msg = resp.json()
                     except Exception as e:
                         error_msg = str(e)
                     raise Exception(f"Reached max retries. Response: {error_msg}")
                 else:
                     sleep = backoff_in_seconds * 2**x + random.uniform(0, 1)
-                    logger.info(
-                        "Args: %s, retrying after %d seconds...", str(args), sleep
-                    )
+                    logger.info("Args: %s, retrying after %d seconds...", str(args), sleep)
                     time.sleep(sleep)
                     x += 1
 
         return wrapper
 
     return decorator
 
@@ -398,17 +381,15 @@
     try:
         # Split the token into its parts
         parts = token_string.split(".")
         if len(parts) != 3:
             return True
 
         # Decode the payload
-        payload_bytes = base64.urlsafe_b64decode(
-            parts[1] + "=="
-        )  # Padding might be needed
+        payload_bytes = base64.urlsafe_b64decode(parts[1] + "==")  # Padding might be needed
         payload = jsonp.loads(payload_bytes)
 
         # Check expiration time
         if "exp" in payload:
             # Deduct 10 seconds to account for any possible latency or clock skew
             expiration_time = payload["exp"] - 10
             if time.time() > expiration_time:
@@ -497,43 +478,35 @@
     # Convert to epoch
     start_epoch = int(start_time.timestamp())
     end_epoch = int(end_time.timestamp())
 
     return start_epoch, end_epoch
 
 
-def dump_request(
-    logger, url: str, method: str, json, params, headers, request_uuid: str, body=True
-):
-    request_headers_filtered = {
-        key: value for key, value in headers.items() if key != "Authorization"
-    }
+def dump_request(logger, url: str, method: str, json, params, headers, request_uuid: str, body=True):
+    request_headers_filtered = {key: value for key, value in headers.items() if key != "Authorization"}
     # Log the request details before sending the request
     request_data = {
         "url": url,
         "method": method,
         "params": jsonp.dumps(params),
         "uuid": str(request_uuid),
         "request_headers": jsonp.dumps(request_headers_filtered),
     }
     log_lines = []
     request_body = ""
     if body:
         request_body = jsonp.dumps(json)
-    log_lines.append(
-        f"\n---[ ZSCALER SDK REQUEST | ID:{request_uuid} ]-------------------------------"
-    )
+    log_lines.append(f"\n---[ ZSCALER SDK REQUEST | ID:{request_uuid} ]-------------------------------")
     log_lines.append(f"{method} {url}")
     for key, value in headers.items():
         log_lines.append(f"{key}: {value}")
     if body and request_body != "" and request_body != "null":
         log_lines.append(f"\n{request_body}")
-    log_lines.append(
-        "--------------------------------------------------------------------"
-    )
+    log_lines.append("--------------------------------------------------------------------")
     logger.info("\n".join(log_lines))
 
 
 def dump_response(
     logger,
     url: str,
     method: str,
@@ -556,22 +529,18 @@
     log_lines = []
     response_body = ""
     if resp.text:
         response_body = resp.text
 
     if from_cache:
         log_lines.append(
-            f"\n---[ ZSCALER SDK RESPONSE | ID:{request_uuid} | "
-            f"FROM CACHE | DURATION:{duration_ms}ms ]" + "-" * 31
+            f"\n---[ ZSCALER SDK RESPONSE | ID:{request_uuid} | " f"FROM CACHE | DURATION:{duration_ms}ms ]" + "-" * 31
         )
     else:
-        log_lines.append(
-            f"\n---[ ZSCALER SDK RESPONSE | ID:{request_uuid} | "
-            f"DURATION:{duration_ms}ms ]" + "-" * 46
-        )
+        log_lines.append(f"\n---[ ZSCALER SDK RESPONSE | ID:{request_uuid} | " f"DURATION:{duration_ms}ms ]" + "-" * 46)
     log_lines.append(f"{method} {full_url}")
     for key, value in response_headers_dict.items():
         log_lines.append(f"{key}: {value}")
     if response_body and response_body != "" and response_body != "null":
         log_lines.append(f"\n{response_body}")
     log_lines.append("-" * 68)
     logger.info("\n".join(log_lines))
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/__init__.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,17 +93,15 @@
     env_cloud = "zscaler"
 
     def __init__(self, cloud, timeout=240, cache=None, fail_safe=False, **kw):
         self.api_key = kw.get("api_key", os.getenv(f"{self._env_base}_API_KEY"))
         self.username = kw.get("username", os.getenv(f"{self._env_base}_USERNAME"))
         self.password = kw.get("password", os.getenv(f"{self._env_base}_PASSWORD"))
         # The 'cloud' parameter should have precedence over environment variables
-        self.env_cloud = (
-            cloud or kw.get("cloud") or os.getenv(f"{self._env_base}_CLOUD")
-        )
+        self.env_cloud = cloud or kw.get("cloud") or os.getenv(f"{self._env_base}_CLOUD")
         if not self.env_cloud:
             raise ValueError(
                 f"Cloud environment must be set via the 'cloud' argument or the {self._env_base}_CLOUD environment variable."
             )
 
         # URL construction
         if cloud == "zspreview":
@@ -113,22 +111,18 @@
             self.url = (
                 kw.get("override_url")
                 or os.getenv(f"{self._env_base}_OVERRIDE_URL")
                 or f"https://zsapi.{self.env_cloud}.net/api/v1"
             )
 
         self.conv_box = True
-        self.sandbox_token = kw.get("sandbox_token") or os.getenv(
-            f"{self._env_base}_SANDBOX_TOKEN"
-        )
+        self.sandbox_token = kw.get("sandbox_token") or os.getenv(f"{self._env_base}_SANDBOX_TOKEN")
         self.timeout = timeout
         self.fail_safe = fail_safe
-        cache_enabled = (
-            os.environ.get("ZSCALER_CLIENT_CACHE_ENABLED", "true").lower() == "true"
-        )
+        cache_enabled = os.environ.get("ZSCALER_CLIENT_CACHE_ENABLED", "true").lower() == "true"
         if cache is None:
             if cache_enabled:
                 ttl = int(os.environ.get("ZSCALER_CLIENT_CACHE_DEFAULT_TTL", 3600))
                 tti = int(os.environ.get("ZSCALER_CLIENT_CACHE_DEFAULT_TTI", 1800))
                 self.cache = ZscalerCache(ttl=ttl, tti=tti)
             else:
                 self.cache = NoOpCache()
@@ -171,17 +165,15 @@
         return result.group(1)
 
     def is_session_expired(self):
         if self.auth_details is None:
             return True
         now = datetime.datetime.now()
         if self.auth_details["passwordExpiryTime"] > 0 and (
-            self.session_refreshed
-            + datetime.timedelta(seconds=-self.session_timeout_offset)
-            < now
+            self.session_refreshed + datetime.timedelta(seconds=-self.session_timeout_offset) < now
         ):
             return True
         return False
 
     @retry_with_backoff(retries=5)
     def authenticate(self) -> Box:
         """
@@ -216,17 +208,15 @@
         """
         logout_url = self.url + "/authenticatedSession"
 
         headers = self.headers.copy()
         headers.update({"Cookie": f"JSESSIONID={self.session_id}"})
 
         try:
-            response = requests.delete(
-                logout_url, headers=headers, timeout=self.timeout
-            )
+            response = requests.delete(logout_url, headers=headers, timeout=self.timeout)
             if response.status_code == 204:
                 self.session_id = None
                 self.auth_details = None
                 return True
             else:
                 return False
         except requests.RequestException as e:
@@ -304,38 +294,30 @@
                     url=url,
                     params=params,
                     method=method,
                     resp=resp,
                     request_uuid=request_uuid,
                     start_time=start_time,
                 )
-                if (
-                    resp.status_code == 429
-                ):  # HTTP Status code 429 indicates "Too Many Requests"
+                if resp.status_code == 429:  # HTTP Status code 429 indicates "Too Many Requests"
                     sleep_time = int(
                         resp.headers.get("Retry-After", 2)
                     )  # Default to 60 seconds if 'Retry-After' header is missing
-                    logger.warning(
-                        f"Rate limit exceeded. Retrying in {sleep_time} seconds."
-                    )
+                    logger.warning(f"Rate limit exceeded. Retrying in {sleep_time} seconds.")
                     sleep(sleep_time)
                     attempts += 1
                     continue
                 else:
                     break
             except requests.RequestException as e:
                 if attempts == 4:  # If it's the last attempt, raise the exception
-                    logger.error(
-                        f"Failed to send {method} request to {url} after 5 attempts. Error: {str(e)}"
-                    )
+                    logger.error(f"Failed to send {method} request to {url} after 5 attempts. Error: {str(e)}")
                     raise e
                 else:
-                    logger.warning(
-                        f"Failed to send {method} request to {url}. Retrying... Error: {str(e)}"
-                    )
+                    logger.warning(f"Failed to send {method} request to {url}. Retrying... Error: {str(e)}")
                     attempts += 1
                     sleep(5)  # Sleep for 5 seconds before retrying
 
         # If Non-GET call, clear the
         if method != "GET":
             self.cache.delete(cache_key)
 
@@ -409,17 +391,15 @@
 
     ERROR_MESSAGES = {
         "UNEXPECTED_STATUS": "Unexpected status code {status_code} received for page {page}.",
         "MISSING_DATA_KEY": "The key '{data_key_name}' was not found in the response for page {page}.",
         "EMPTY_RESULTS": "No results found for page {page}.",
     }
 
-    def get_paginated_data(
-        self, path=None, data_key_name=None, data_per_page=5, expected_status_code=200
-    ):
+    def get_paginated_data(self, path=None, data_key_name=None, data_per_page=5, expected_status_code=200):
         """
         Fetch paginated data from the ZIA API.
         ...
 
         Returns:
         - list: List of fetched items.
         - str: Error message, if any occurred.
@@ -439,44 +419,36 @@
             response = self.send(
                 method="GET",
                 path=required_url,
                 params={"page": page, "pageSize": data_per_page},
             )
 
             if response.status_code != expected_status_code:
-                error_message = self.ERROR_MESSAGES["UNEXPECTED_STATUS"].format(
-                    status_code=response.status_code, page=page
-                )
+                error_message = self.ERROR_MESSAGES["UNEXPECTED_STATUS"].format(status_code=response.status_code, page=page)
                 logger.error(error_message)
                 break
             data_json = response.json()
             if isinstance(data_json, list):
                 data = data_json
             else:
                 data = data_json.get(data_key_name)
 
             if data is None:
-                error_message = self.ERROR_MESSAGES["MISSING_DATA_KEY"].format(
-                    data_key_name=data_key_name, page=page
-                )
+                error_message = self.ERROR_MESSAGES["MISSING_DATA_KEY"].format(data_key_name=data_key_name, page=page)
                 logger.error(error_message)
                 break
 
             if not data:  # Checks for empty data
                 logger.info(self.ERROR_MESSAGES["EMPTY_RESULTS"].format(page=page))
                 break
 
             ret_data.extend(convert_keys_to_snake(data))
 
             # Check for more pages
-            if (
-                len(data) == 0
-                or isinstance(data_json, dict)
-                and int(response.json().get("totalPages")) <= page + 1
-            ):
+            if len(data) == 0 or isinstance(data_json, dict) and int(response.json().get("totalPages")) <= page + 1:
                 break
 
             page += 1
 
         return BoxList(ret_data), error_message
 
     @property
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/activate.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/activate.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/admin_and_role_management.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/admin_and_role_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,17 +67,15 @@
         response = self.rest.get("/adminUsers/%s" % (user_id))
         if isinstance(response, Response):
             status_code = response.status_code
             if status_code != 200:
                 return None
         return response
 
-    def add_user(
-        self, name: str, login_name: str, email: str, password: str, **kwargs
-    ) -> Box:
+    def add_user(self, name: str, login_name: str, email: str, password: str, **kwargs) -> Box:
         """
         Adds a new admin user to ZIA.
 
         Args:
             name (str): The user's full name.
             login_name (str):
                 The name that the admin user will use to login to ZIA in email format, i.e. `user@domain.tld.`
@@ -170,17 +168,15 @@
                 payload[snake_to_camel(key)] = value
 
         response = self.rest.post("adminUsers", json=payload)
         if isinstance(response, Response):
             # Handle error response
             status_code = response.status_code
             if status_code != 200:
-                raise Exception(
-                    f"API call failed with status {status_code}: {response.json()}"
-                )
+                raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_user(self, user_id: str, **kwargs) -> dict:
         """
         Update an admin user.
 
         Args:
@@ -260,17 +256,15 @@
         # Update payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
         response = self.rest.put("/adminUsers/%s" % (user_id), json=payload)
         if isinstance(response, Response) and not response.ok:
             # Handle error response
-            raise Exception(
-                f"API call failed with status {response.status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
 
         # Return the updated object
         return self.get_user(user_id)
 
     def delete_user(self, user_id: str) -> int:
         """
         Deletes the specified admin user by id.
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/apptotal.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/apptotal.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/audit_logs.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/audit_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,17 +57,15 @@
             ...    end_time='1627271676622')
 
         """
         payload = {
             "startTime": start_time,
             "endTime": end_time,
         }
-        return self.rest.post(
-            "auditlogEntryReport", json=payload, box=False
-        ).status_code
+        return self.rest.post("auditlogEntryReport", json=payload, box=False).status_code
 
     def cancel(self) -> int:
         """
         Cancels the request to create an audit log report.
 
         Returns:
             :obj:`int`: The operation response code.
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/authentication_settings.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/authentication_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,17 +54,15 @@
         Returns:
             :obj:`BoxList`: The complete and updated exempt list.
 
         """
 
         payload = {"urls": url_list}
 
-        resp = self.rest.post(
-            "authSettings/exemptedUrls?action=ADD_TO_LIST", json=payload
-        )
+        resp = self.rest.post("authSettings/exemptedUrls?action=ADD_TO_LIST", json=payload)
 
         # Check if the response object has a 'status_code' attribute before accessing it
         if hasattr(resp, "status_code"):
             if resp.status_code == 204:
                 return self.get_exempted_urls()
         else:
             # Handle case where resp is a Box object
@@ -85,14 +83,12 @@
             :obj:`BoxList`: The updated exemption list.
 
         Examples:
             >>> zia.authentication_settings.delete_urls_from_exempt_list(['example.com'])
 
         """
         payload = {"urls": url_list}
-        resp = self.rest.post(
-            "authSettings/exemptedUrls?action=REMOVE_FROM_LIST", json=payload
-        )
+        resp = self.rest.post("authSettings/exemptedUrls?action=REMOVE_FROM_LIST", json=payload)
 
         # Return the updated exemption list if the removal was successful.
         if resp == 200:
             return self.get_exempted_urls()
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/client.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/client.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/cloud_apps.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/cloud_apps.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,17 +291,15 @@
 
         """
         payload = {"duration": duration}
         convert_keys(payload.update(kwargs))
 
         return self.rest.post("shadowIT/applications/export", json=payload).text
 
-    def export_shadow_it_csv(
-        self, application: str, entity: str, duration: str = "LAST_1_DAYS", **kwargs
-    ):
+    def export_shadow_it_csv(self, application: str, entity: str, duration: str = "LAST_1_DAYS", **kwargs):
         """
         Export the Shadow IT Report (in CSV format) for the list of users or known locations
         identified with using the cloud applications specified in the request. The report
         includes details such as user interactions, application category, application usage,
         number of transactions, last accessed time, etc.
 
         You can customize the report using various filters.
@@ -363,17 +361,15 @@
         for key in ["users", "locations", "departments"]:
             id_list = kwargs.pop(key, None)
             if id_list is not None:
                 payload[key] = self._convert_ids_to_dict_list(id_list)
 
         convert_keys(payload.update(kwargs))
 
-        return self.rest.post(
-            f"shadowIT/applications/{entity}/exportCsv", json=payload
-        ).text
+        return self.rest.post(f"shadowIT/applications/{entity}/exportCsv", json=payload).text
 
     def list_apps(self):
         """
         List all predefined and custom cloud applications by name and id.
 
         Returns:
             :obj:`BoxList` of :obj:`Box`: A list of cloud applications.
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/device_management.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/device_management.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/dlp.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/dlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,17 +70,15 @@
         response = self.rest.get("/dlpDictionaries/%s" % (dict_id))
         if isinstance(response, Response):
             status_code = response.status_code
             if status_code != 200:
                 return None
         return response
 
-    def add_dict(
-        self, name: str, custom_phrase_match_type: str, dictionary_type: str, **kwargs
-    ) -> Box:
+    def add_dict(self, name: str, custom_phrase_match_type: str, dictionary_type: str, **kwargs) -> Box:
         """
         Add a new Patterns and Phrases DLP Dictionary to ZIA.
 
         Args:
             name (str): The name of the DLP Dictionary.
             match_type (str): The DLP custom phrase/pattern match type. Accepted values are ``all`` or ``any``.
             **kwargs: Optional keyword args.
@@ -157,17 +155,15 @@
             camel_key = snake_to_camel(key)
             payload[camel_key] = value
 
         response = self.rest.post("dlpDictionaries", json=payload)
         if isinstance(response, Response):
             # Handle non-successful status codes
             status_code = response.status_code
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
 
         return response
 
     def update_dict(self, dict_id: str, **kwargs) -> Box:
         """
         Updates the specified DLP Dictionary.
 
@@ -233,17 +229,15 @@
             # Convert the key to camelCase and assign the value
             camel_key = snake_to_camel(key)
             payload[camel_key] = value
 
         response = self.rest.put(f"/dlpDictionaries/{dict_id}", json=payload)
         if isinstance(response, Response):
             status_code = response.status_code
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
 
         # Return the updated object
         return self.get_dict(dict_id)
 
     def delete_dict(self, dict_id: str) -> int:
         """
         Deletes the DLP Dictionary that matches the specified DLP Dictionary id.
@@ -274,17 +268,15 @@
 
         Returns:
             :obj:`Box`: Information on the provided pattern.
 
         """
         payload = {"data": pattern}
 
-        response = self.rest.post(
-            path="dlpDictionaries/validateDlpPattern", json=payload
-        )
+        response = self.rest.post(path="dlpDictionaries/validateDlpPattern", json=payload)
         if isinstance(response, Response):
             return None
         return response
 
     # TODO: implement the remaining
     def add_dlp_engine(
         self,
@@ -315,17 +307,15 @@
         camel_payload = {snake_to_camel(key): value for key, value in payload.items()}
 
         response = self.rest.post("dlpEngines", json=camel_payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_dlp_engine(self, engine_id: str, **kwargs) -> Box:
         """
         Updates an existing dlp engine.
 
         Args:
@@ -357,27 +347,23 @@
             >>> zia.dlp.add_dlp_engine('976597',
             ...    custom_dlp_engine=True,
             ...    engine_expression="((D63.S > 1))",
             ...    description="TT#1965232866")
 
         """
         # Set payload to value of existing record
-        payload = {
-            snake_to_camel(k): v for k, v in self.get_dlp_engines(engine_id).items()
-        }
+        payload = {snake_to_camel(k): v for k, v in self.get_dlp_engines(engine_id).items()}
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
         response = self.rest.put(f"/dlpEngines/{engine_id}", json=payload)
         if isinstance(response, Response) and response.status_code != 200:
-            raise Exception(
-                f"API call failed with status {response.status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
         return self.get_dlp_engines(engine_id)
 
     def delete_dlp_engine(self, engine_id: str) -> int:
         """
         Deletes the specified dlp engine.
 
         Args:
@@ -703,17 +689,15 @@
             camel_key = snake_to_camel(key)
             payload[camel_key] = value
 
         response = self.rest.post("dlpNotificationTemplates", json=payload)
         if isinstance(response, Response):
             # Handle non-successful status codes
             status_code = response.status_code
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
 
         return response
 
     def update_dlp_template(self, template_id: str, **kwargs) -> Box:
         """
         Updates the specified DLP Notification Template.
 
@@ -747,38 +731,29 @@
 
         # Fetch the existing template details
         existing_template = self.get_dlp_templates(template_id)
         if not existing_template:
             raise ValueError("Template not found with the provided ID")
 
         # Construct the payload for update
-        payload = {
-            snake_to_camel(key): kwargs.get(
-                key, existing_template.get(snake_to_camel(key))
-            )
-            for key in kwargs
-        }
+        payload = {snake_to_camel(key): kwargs.get(key, existing_template.get(snake_to_camel(key))) for key in kwargs}
 
         # Ensure mandatory fields are included
         mandatory_fields = ["plainTextMessage", "htmlMessage"]
         for field in mandatory_fields:
             if field not in payload:
                 payload[field] = existing_template.get(field)
 
         # Add the template ID
         payload["id"] = template_id
 
         # Make the API call
-        response = self.rest.put(
-            f"/dlpNotificationTemplates/{template_id}", json=payload
-        )
+        response = self.rest.put(f"/dlpNotificationTemplates/{template_id}", json=payload)
         if isinstance(response, Response) and response.status_code != 200:
-            raise Exception(
-                f"API call failed with status {response.status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
 
         # Return the updated object
         return self.get_dlp_templates(template_id)
 
     def delete_dlp_template(self, template_id: str) -> int:
         """
         Deletes the DLP Notification Template that matches the specified Template id.
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/errors.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/errors.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/firewall.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/firewall.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,17 +158,15 @@
                 camel_payload[snake_to_camel(key)] = value
 
         # Send POST request to create the rule
         response = self.rest.post("firewallFilteringRules", json=payload)
         if isinstance(response, Response):
             status_code = response.status_code
             if status_code != 200:
-                raise Exception(
-                    f"API call failed with status {status_code}: {response.json()}"
-                )
+                raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_rule(self, rule_id: str, **kwargs) -> Box:
         """
         Updates an existing firewall filter rule.
 
         Args:
@@ -232,17 +230,15 @@
         # Add remaining optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
         response = self.rest.put(f"firewallFilteringRules/{rule_id}", json=payload)
         if isinstance(response, Response) and not response.ok:
             # Handle error response
-            raise Exception(
-                f"API call failed with status {response.status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
 
         # Return the updated object
         return self.get_rule(rule_id)
 
     def delete_rule(self, rule_id: str) -> int:
         """
         Deletes the specified firewall filter rule.
@@ -389,18 +385,15 @@
             >>> zia.firewall.update_ip_destination_group('9032668',
             ...    description="Tech News",
             ...    addresses=['arstechnica.com', 'slashdot.org'])
 
         """
 
         # Set payload to value of existing record
-        payload = {
-            snake_to_camel(k): v
-            for k, v in self.get_ip_destination_group(group_id).items()
-        }
+        payload = {snake_to_camel(k): v for k, v in self.get_ip_destination_group(group_id).items()}
 
         # Update payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
         return self.rest.put(f"ipDestinationGroups/{group_id}", json=payload)
 
@@ -459,17 +452,15 @@
 
         Examples:
             >>> zia.firewall.delete_ip_source_group('762398')
 
         """
         return self.rest.delete(f"ipSourceGroups/{group_id}").status_code
 
-    def add_ip_source_group(
-        self, name: str, ip_addresses: list, description: str = None
-    ) -> Box:
+    def add_ip_source_group(self, name: str, ip_addresses: list, description: str = None) -> Box:
         """
         Adds a new IP Source Group.
 
         Args:
             name (str): The name of the IP Source Group.
             ip_addresses (str): The list of IP addresses for the IP Source Group.
             description (str): Additional information for the IP Source Group.
@@ -523,17 +514,15 @@
             >>> zia.firewall.update_ip_source_group('9032674',
             ...    description='Local subnets, updated on 3 JUL 21'
             ...    ip_addresses=['192.0.2.0/29', '192.0.2.8/29', '192.0.2.128/25'])
 
         """
 
         # Set payload to value of existing record
-        payload = {
-            snake_to_camel(k): v for k, v in self.get_ip_source_group(group_id).items()
-        }
+        payload = {snake_to_camel(k): v for k, v in self.get_ip_source_group(group_id).items()}
 
         # Update payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
         return self.rest.put(f"ipSourceGroups/{group_id}", json=payload)
 
@@ -587,17 +576,15 @@
                 # 'response' is a Box with the expected data
                 return response
             else:
                 # Handle cases where the response Box does not contain the expected data
                 # For example, you might want to check for an 'error' or 'message' field
                 # and raise an exception or handle the situation as needed
                 # Example: raise ValueError("Failed to retrieve the network application group.")
-                return (
-                    Box()
-                )  # An empty Box indicates no data was found or an error occurred.
+                return Box()  # An empty Box indicates no data was found or an error occurred.
 
     def delete_network_app_group(self, group_id: str) -> int:
         """
         Deletes the specified Network Application Group.
 
         Args:
             group_id (str): The unique identifier for the Network Application Group.
@@ -607,17 +594,15 @@
 
         Examples:
             >>> zia.firewall.delete_network_app_group('762398')
 
         """
         return self.rest.delete(f"networkApplicationGroups/{group_id}").status_code
 
-    def add_network_app_group(
-        self, name: str, network_applications: list, description: str = None
-    ) -> Box:
+    def add_network_app_group(self, name: str, network_applications: list, description: str = None) -> Box:
         """
         Adds a new Network Application Group.
 
         Args:
             name (str): The name of the Network Application Group.
             description (str): Additional information about the Network Application Group.
             network_applications (list): A list of Application IDs to add to the group.
@@ -641,17 +626,15 @@
         }
 
         response = self.rest.post("networkApplicationGroups", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
         # return self.rest.post("networkApplicationGroups", json=payload)
 
     def update_network_app_group(self, group_id: str, **kwargs) -> Box:
         """
         Update an Network Application Group.
@@ -681,26 +664,21 @@
             >>> zia.firewall.update_network_app_group('9032674',
             ...    description='Network Application Group, updated on May 27, 2023'
             ...    network_applications=['SALESFORCE', 'GOOGLEANALYTICS', 'OFFICE365'])
 
         """
 
         # Set payload to value of existing record
-        payload = {
-            snake_to_camel(k): v
-            for k, v in self.get_network_app_group(group_id).items()
-        }
+        payload = {snake_to_camel(k): v for k, v in self.get_network_app_group(group_id).items()}
 
         # Update payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
-        resp = self.rest.put(
-            f"networkApplicationGroups/{group_id}", json=payload
-        ).status_code
+        resp = self.rest.put(f"networkApplicationGroups/{group_id}", json=payload).status_code
 
         # Return the object if it was updated successfully
         if not isinstance(resp, Response):
             return self.get_network_app_group(group_id)
 
     def list_network_apps(self, search: str = None) -> BoxList:
         """
@@ -785,17 +763,15 @@
 
         Examples:
             >>> zia.firewall.delete_network_svc_group('762398')
 
         """
         return self.rest.delete(f"networkServiceGroups/{group_id}").status_code
 
-    def add_network_svc_group(
-        self, name: str, service_ids: list, description: str = None
-    ) -> Box:
+    def add_network_svc_group(self, name: str, service_ids: list, description: str = None) -> Box:
         """
         Adds a new Network Service Group.
 
         Args:
             name (str): The name of the Network Service Group.
             service_ids (list): A list of Network Service IDs to add to the group.
             description (str): Additional information about the Network Service Group.
@@ -841,36 +817,29 @@
             >>> zia.firewall.update_network_svc_group(name='Update Network Service Group',
             ...    service_ids=['159143', '159144', '159145'],
             ...    description='Group for the new Network Service.')
 
         """
 
         # Set payload to value of existing record
-        payload = {
-            snake_to_camel(k): v
-            for k, v in self.get_network_svc_group(group_id).items()
-        }
+        payload = {snake_to_camel(k): v for k, v in self.get_network_svc_group(group_id).items()}
 
         # Update payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
         # return self.rest.put(f"networkServiceGroups/{group_id}", json=payload)
 
-        resp = self.rest.put(
-            f"networkServiceGroups/{group_id}", json=payload
-        ).status_code
+        resp = self.rest.put(f"networkServiceGroups/{group_id}", json=payload).status_code
 
         # Return the object if it was updated successfully
         if not isinstance(resp, Response):
             return self.get_network_svc_group(group_id)
 
-    def list_network_services(
-        self, search: str = None, protocol: str = None
-    ) -> BoxList:
+    def list_network_services(self, search: str = None, protocol: str = None) -> BoxList:
         """
         Returns a list of all Network Services.
 
         The search parameters find matching values within the "name" or "description" attributes.
 
         Args:
             search (str): The search string used to match against a service's name or description attributes.
@@ -971,35 +940,29 @@
 
         # Convert tuple list to dict and add to payload
         if ports is not None:
             for items in ports:
                 port_range = [{"start": items[2]}]
                 if len(items) == 4:
                     port_range.append({"end": items[3]})
-                payload.setdefault(f"{items[0]}{items[1].title()}Ports", []).extend(
-                    port_range
-                )
+                payload.setdefault(f"{items[0]}{items[1].title()}Ports", []).extend(port_range)
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
         response = self.rest.post("networkServices", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
-    def update_network_service(
-        self, service_id: str, ports: list = None, **kwargs
-    ) -> Box:
+    def update_network_service(self, service_id: str, ports: list = None, **kwargs) -> Box:
         """
         Updates the specified Network Service.
 
         If ports aren't provided then no changes will be made to the ports already defined. If ports are provided then
         the existing ports will be overwritten.
 
         Args:
@@ -1034,18 +997,15 @@
 
             >>> zia.firewall.add_network_service('959093',
             ...    ports=[
             ...        ('dest', 'tcp', '500', '510')])
 
 
         """
-        payload = {
-            snake_to_camel(k): v
-            for k, v in self.get_network_service(service_id).items()
-        }
+        payload = {snake_to_camel(k): v for k, v in self.get_network_service(service_id).items()}
 
         # Convert tuple list to dict and add to payload
         if ports is not None:
             # Clear existing ports and set new values
             for items in ports:
                 port_key = f"{items[0]}{items[1].title()}Ports"
                 payload[port_key] = []
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/forwarding_control.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/forwarding_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,17 +170,15 @@
 
         # Send POST request to create the rule
         response = self.rest.post("forwardingRules", json=payload)
         if isinstance(response, Response):
             # Handle error response
             status_code = response.status_code
             if status_code != 200:
-                raise Exception(
-                    f"API call failed with status {status_code}: {response.json()}"
-                )
+                raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_rule(self, rule_id: str, **kwargs) -> Box:
         """
         Updates an existing forwarding control  filter rule.
 
         Args:
@@ -243,17 +241,15 @@
         # Add remaining optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
         response = self.rest.put(f"forwardingRules/{rule_id}", json=payload)
         if isinstance(response, Response) and not response.ok:
             # Handle error response
-            raise Exception(
-                f"API call failed with status {response.status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
 
         # Return the updated object
         return self.get_rule(rule_id)
 
     def delete_rule(self, rule_id: str) -> int:
         """
         Deletes the specified forwarding control filter rule.
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/isolation_profile.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/isolation_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/labels.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,17 +114,15 @@
             payload[snake_to_camel(key)] = value
 
         response = self.rest.post("ruleLabels", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_label(self, label_id: str, **kwargs):
         """
         Updates information for the specified ZIA Rule Label.
 
         Args:
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/locations.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/locations.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,23 +83,17 @@
 
         Examples:
             >>> location = zia.locations.get_location('97456691')
 
             >>> location = zia.locations.get_location_name(name='stockholm_office')
         """
         if location_id and location_name:
-            raise ValueError(
-                "TOO MANY ARGUMENTS: Expected either location_id or location_name. Both were provided."
-            )
+            raise ValueError("TOO MANY ARGUMENTS: Expected either location_id or location_name. Both were provided.")
         elif location_name:
-            location = (
-                record
-                for record in self.list_locations(search=location_name)
-                if record.name == location_name
-            )
+            location = (record for record in self.list_locations(search=location_name) if record.name == location_name)
             return next(location, None)
 
         return self.rest.get(f"locations/{location_id}")
 
     def add_location(self, name: str, **kwargs) -> Box:
         """
         Adds a new location.
@@ -219,17 +213,15 @@
             payload[snake_to_camel(key)] = value
 
         response = self.rest.post("locations", json=payload)
         if isinstance(response, Response):
             # Handle error response
             status_code = response.status_code
             if status_code != 200:
-                raise Exception(
-                    f"API call failed with status {status_code}: {response.json()}"
-                )
+                raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def list_sub_locations(self, location_id: str, **kwargs) -> BoxList:
         """
         Returns sub-location information for the specified location ID.
 
         Args:
@@ -431,32 +423,28 @@
             Update the VPN credentials of a location:
 
             >>> zia.locations.update_location('99999',
             ...    vpn_credentials=[{'id': '88888', 'type': 'UFQDN'}])
 
         """
         # Set payload to value of existing record
-        payload = {
-            snake_to_camel(k): v for k, v in self.get_location(location_id).items()
-        }
+        payload = {snake_to_camel(k): v for k, v in self.get_location(location_id).items()}
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
         # Fixes edge case where the sublocation object is missing displayTimeUnit, which will result in a 500 error.
         if not payload.get("displayTimeUnit"):
             payload["displayTimeUnit"] = "MINUTE"
 
         response = self.rest.put(f"locations/{location_id}", json=payload)
         if isinstance(response, Response) and not response.ok:
             # Handle error response
-            raise Exception(
-                f"API call failed with status {response.status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
 
         # Return the updated object
         return self.get_location(location_id)
 
     def delete_location(self, location_id: str) -> int:
         """
         Deletes the location or sub-location for the specified ID
@@ -506,17 +494,15 @@
 
         Examples:
             Get a specific location group by its ID:
             >>> location = zia.locations.get_location_group_by_id(24326827)
         """
         return self.rest.get(f"locations/groups/{group_id}")
 
-    def get_location_group_by_name(
-        self, group_name: str, page: int = 1, page_size: int = 100
-    ) -> Box:
+    def get_location_group_by_name(self, group_name: str, page: int = 1, page_size: int = 100) -> Box:
         """
         Return a specific location group by its name in ZIA.
 
         Args:
             group_name (str): The name of the location group.
             page (int, optional): Page number to retrieve. Defaults to 1.
             page_size (int, optional): Number of records per page. Defaults to 100.
@@ -563,17 +549,15 @@
 
         Examples:
             Get a specific location group by its ID:
             >>> location = zia.locations.get_location_group_lite_by_id(24326827)
         """
         return self.rest.get(f"locations/groups/lite/{group_id}")
 
-    def get_location_group_lite_by_name(
-        self, group_name: str, page: int = 1, page_size: int = 100
-    ) -> BoxList:
+    def get_location_group_lite_by_name(self, group_name: str, page: int = 1, page_size: int = 100) -> BoxList:
         """
         Return specific location groups (lite version) by their name where only name and ID is returned in ZIA.
 
         Args:
             group_name (str): The name of the location group.
             page (int, optional): Page number to retrieve. Defaults to 1.
             page_size (int, optional): Number of records per page. Defaults to 100.
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/sandbox.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/sandbox.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/security.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/security.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,15 @@
         """
         response = self.rest.get("security")
 
         # ZIA removes the whitelistUrls key from the JSON response when it's empty.
         if "whitelist_urls" in self.rest.get("security"):
             return response.whitelist_urls
         else:
-            return (
-                BoxList()
-            )  # Return empty list so other methods in this class don't break
+            return BoxList()  # Return empty list so other methods in this class don't break
 
     def get_blacklist(self) -> BoxList:
         """
         Returns a list of blacklisted URLs.
 
         Returns:
             :obj:`BoxList`: A list of blacklisted URLs
@@ -161,17 +159,15 @@
         Examples:
             >>> zia.security.add_urls_to_blacklist(['example.com', 'web.example.com'])
 
         """
 
         payload = {"blacklistUrls": url_list}
 
-        resp = self.rest.post(
-            "security/advanced/blacklistUrls?action=ADD_TO_LIST", json=payload
-        ).status_code
+        resp = self.rest.post("security/advanced/blacklistUrls?action=ADD_TO_LIST", json=payload).status_code
 
         # Return the object if it was updated successfully
         if resp == 204:
             return self.get_blacklist()
 
     def replace_blacklist(self, url_list: list) -> BoxList:
         """
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/ssl_inspection.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/ssl_inspection.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,17 +102,15 @@
             "deptName": dept,
             "city": city,
             "state": state,
             "country": country,
             "signatureAlgorithm": signature,
         }
 
-        return self.rest.post(
-            "sslSettings/generatecsr", json=payload, box=False
-        ).status_code
+        return self.rest.post("sslSettings/generatecsr", json=payload, box=False).status_code
 
     def upload_int_ca_cert(self, cert: tuple) -> int:
         """
         Uploads a signed Intermediate Root CA certificate.
 
         Args:
             cert (tuple): The Intermediate Root CA certificate tuple in the following format, where `int_ca_pem` is a
@@ -128,17 +126,15 @@
 
             >>> zia.ssl.upload_int_ca_cert(('int_ca.pem', open('int_ca.pem', 'rb')))
 
         """
 
         payload = {"fileUpload": cert}
 
-        return self.rest.post(
-            "sslSettings/uploadcert/text", files=payload, box=False
-        ).status_code
+        return self.rest.post("sslSettings/uploadcert/text", files=payload, box=False).status_code
 
     def upload_int_ca_chain(self, cert: tuple) -> int:
         """
         Uploads the Intermediate Root CA certificate chain.
 
         Args:
             cert (tuple): The Intermediate Root CA chain certificate tuple in the following format, where
@@ -156,17 +152,15 @@
 
             >>> zia.ssl.upload_int_ca_chain(('int_ca_chain.pem', open('int_ca_chain.pem', 'rb')))
 
         """
 
         payload = {"fileUpload": cert}
 
-        return self.rest.post(
-            "sslSettings/uploadcertchain/text", files=payload, box=False
-        ).status_code
+        return self.rest.post("sslSettings/uploadcertchain/text", files=payload, box=False).status_code
 
     def delete_int_chain(self) -> int:
         """
         Deletes the Intermediate Root CA certificate chain.
 
         Returns:
             :obj:`int`: The status code for the operation.
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/traffic.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/traffic.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,17 +165,15 @@
             >>> closest_vips = zia.traffic.get_closest_diverse_vip_ids('203.0.113.20')
 
         """
         vips_list = self.list_vips_recommended(source_ip=ip_address)
         preferred_vip = vips_list[0]  # First entry is closest vip
 
         # Generator to find the next closest vip not in the same city as our preferred
-        secondary_vip = next(
-            (vip for vip in vips_list if vip.city != preferred_vip.city)
-        )
+        secondary_vip = next((vip for vip in vips_list if vip.city != preferred_vip.city))
         recommended_vips = (preferred_vip.id, secondary_vip.id)
 
         return recommended_vips
 
     def list_vip_group_by_dc(self, source_ip: str, **kwargs) -> BoxList:
         """
         Returns a list of recommended GRE tunnel (VIPs) grouped by data center.
@@ -215,17 +213,15 @@
 
         for key, value in kwargs.items():
             params[snake_to_camel(key)] = value
         response = self.rest.get("/vips/groupByDatacenter", params=params)
         if response is not None:
             return response
         else:
-            print(
-                "Failed to fetch VIP groups by data center. No response or error received."
-            )
+            print("Failed to fetch VIP groups by data center. No response or error received.")
             return BoxList([])
 
     def list_vips(self, **kwargs) -> BoxList:
         """
         Returns a list of virtual IP addresses (VIPs) available in the Zscaler cloud.
 
         Keyword Args:
@@ -335,17 +331,15 @@
             payload[snake_to_camel(key)] = value
 
         response = self.rest.post("greTunnels", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_gre_tunnel(
         self,
         tunnel_id: str,
         source_ip: str = None,
         primary_dest_vip_id: str = None,
@@ -353,17 +347,15 @@
         **kwargs,
     ) -> Box:
         """
         Update an existing GRE tunnel.
         """
 
         if tunnel_id is None:
-            raise ValueError(
-                "tunnel_id is a required parameter for updating a GRE tunnel."
-            )
+            raise ValueError("tunnel_id is a required parameter for updating a GRE tunnel.")
 
         # Determine VIPs based on source_ip if not provided
         if primary_dest_vip_id is None or secondary_dest_vip_id is None:
             recommended_vips = self.get_closest_diverse_vip_ids(source_ip)
             primary_dest_vip_id = primary_dest_vip_id or recommended_vips[0]
             secondary_dest_vip_id = secondary_dest_vip_id or recommended_vips[1]
 
@@ -376,17 +368,15 @@
         # Include additional optional parameters
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
         response = self.rest.put(f"greTunnels/{tunnel_id}", json=payload)
         if isinstance(response, Response) and not response.ok:
             # Handle error response
-            raise Exception(
-                f"API call failed with status {response.status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
         # Return the updated object
         return self.get_gre_tunnel(tunnel_id)
 
     def delete_gre_tunnel(self, tunnel_id: str) -> int:
         """
         Delete the specified static IP.
 
@@ -438,17 +428,15 @@
             List static IPs, returning 200 items per page for a maximum of 2 pages:
 
             >>> for ip_address in zia.traffic.list_static_ips(page_size=200, max_pages=2):
             ...    print(ip_address)
 
         """
         valid_params = ["availableForGreTunnel", "ipAddress"]
-        query_params = {
-            k: v for k, v in kwargs.items() if k in valid_params and v is not None
-        }
+        query_params = {k: v for k, v in kwargs.items() if k in valid_params and v is not None}
 
         response = self.rest.get("/staticIP", params=query_params)
         if isinstance(response, Response):
             return None
         return response
 
     def get_static_ip(self, static_ip_id: str) -> Box:
@@ -512,17 +500,15 @@
             payload[snake_to_camel(key)] = value
 
         response = self.rest.post("staticIP", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def check_static_ip(self, ip_address: str) -> bool:
         """
         Validates if a static IP object is correct.
 
         Args:
@@ -585,17 +571,15 @@
         # Add optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
         response = self.rest.put(f"staticIP/{static_ip_id}", json=payload)
         if isinstance(response, Response) and not response.ok:
             # Handle error response
-            raise Exception(
-                f"API call failed with status {response.status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
 
         # Return the updated object
         return self.get_static_ip(static_ip_id)
 
     def delete_static_ip(self, static_ip_id: str) -> int:
         """
         Delete the specified static IP.
@@ -657,17 +641,15 @@
             List VPN credentials, returning 200 items per page for a maximum of 2 pages:
 
             >>> for credential in zia.traffic.list_vpn_credentials(page_size=200, max_pages=2):
             ...    print(credential)
         """
         return BoxList(Iterator(self.rest, "vpnCredentials", **kwargs))
 
-    def add_vpn_credential(
-        self, authentication_type: str, pre_shared_key: str = None, **kwargs
-    ) -> Box:
+    def add_vpn_credential(self, authentication_type: str, pre_shared_key: str = None, **kwargs) -> Box:
         """
         Add new VPN credentials.
 
         If a pre_shared_key is not provided, one will be randomly generated.
 
         Args:
             authentication_type (str):
@@ -707,17 +689,15 @@
             payload[snake_to_camel(key)] = value
 
         response = self.rest.post("vpnCredentials", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def bulk_delete_vpn_credentials(self, credential_ids: list) -> int:
         """
         Bulk delete VPN credentials.
 
         Args:
@@ -735,17 +715,15 @@
         payload = {"ids": credential_ids}
 
         response = self.rest.post("vpnCredentials/bulkDelete", json=payload).status_code
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def get_vpn_credential(self, credential_id: str = None, fqdn: str = None) -> Box:
         """
         Get VPN credentials for the specified ID or fqdn.
 
         Args:
@@ -760,23 +738,17 @@
         Examples:
             >>> pprint(zia.traffic.get_vpn_credential('97679391'))
 
             >>> pprint(zia.traffic.get_vpn_credential(fqdn='userid@fqdn'))
 
         """
         if credential_id and fqdn:
-            raise ValueError(
-                "TOO MANY ARGUMENTS: Expected either a credential_id or an fqdn. Both were provided."
-            )
+            raise ValueError("TOO MANY ARGUMENTS: Expected either a credential_id or an fqdn. Both were provided.")
         elif fqdn:
-            credential = (
-                record
-                for record in self.list_vpn_credentials(search=fqdn)
-                if record.fqdn == fqdn
-            )
+            credential = (record for record in self.list_vpn_credentials(search=fqdn) if record.fqdn == fqdn)
             return next(credential, None)
 
         return self.rest.get(f"vpnCredentials/{credential_id}")
 
     def update_vpn_credential(self, credential_id: str, **kwargs) -> Box:
         """
         Update VPN credentials with the specified ID.
@@ -820,17 +792,15 @@
         # Add optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
         response = self.rest.put(f"vpnCredentials/{credential_id}", json=payload)
         if isinstance(response, Response) and not response.ok:
             # Handle error response
-            raise Exception(
-                f"API call failed with status {response.status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
 
         # Return the updated object
         return self.get_vpn_credential(credential_id)
 
     def delete_vpn_credential(self, credential_id: str) -> int:
         """
         Delete VPN credentials for the specified ID.
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/url_categories.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/url_categories.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,17 +51,15 @@
                 time.sleep(1)
             return results
 
         else:
             payload = urls
             return self.rest.post("urlLookup", json=payload)
 
-    def list_categories(
-        self, custom_only: bool = False, only_counts: bool = False
-    ) -> BoxList:
+    def list_categories(self, custom_only: bool = False, only_counts: bool = False) -> BoxList:
         """
         Returns information on URL categories.
 
         Args:
             custom_only (bool):
                 Returns only custom categories if True.
             only_counts (bool):
@@ -121,17 +119,15 @@
 
         Examples:
             >>> zia.url_categories.get_category('ALCOHOL_TOBACCO')
 
         """
         return self.rest.get(f"urlCategories/{category_id}")
 
-    def add_url_category(
-        self, configured_name: str, super_category: str, urls: list, **kwargs
-    ) -> Box:
+    def add_url_category(self, configured_name: str, super_category: str, urls: list, **kwargs) -> Box:
         """
         Adds a new custom URL category.
 
         Args:
             name (str):
                 Name of the URL category.
             super_category (str):
@@ -190,17 +186,15 @@
             payload[snake_to_camel(key)] = value
 
         response = self.rest.post("urlCategories", json=payload)
         if isinstance(response, Response):
             # Handle error response
             status_code = response.status_code
             if status_code != 200:
-                raise Exception(
-                    f"API call failed with status {status_code}: {response.json()}"
-                )
+                raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def add_tld_category(self, name: str, tlds: list, **kwargs) -> Box:
         """
         Adds a new custom TLD category.
 
         Args:
@@ -239,17 +233,15 @@
             payload[snake_to_camel(key)] = value
 
         response = self.rest.post("urlCategories", json=payload)
         if isinstance(response, Response):
             # Handle error response
             status_code = response.status_code
             if status_code != 200:
-                raise Exception(
-                    f"API call failed with status {status_code}: {response.json()}"
-                )
+                raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_url_category(self, category_id: str, **kwargs) -> Box:
         """
         Updates a URL category.
 
         Args:
@@ -297,17 +289,15 @@
         # Add optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
         response = self.rest.put(f"urlCategories/{category_id}", json=payload)
         if isinstance(response, Response) and not response.ok:
             # Handle error response
-            raise Exception(
-                f"API call failed with status {response.status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
 
         # Return the updated object
         return self.get_category(category_id)
 
     def add_urls_to_category(self, category_id: str, urls: list) -> Box:
         """
         Adds URLS to a URL category.
@@ -326,22 +316,18 @@
             ...    urls=['example.com'])
 
         """
 
         payload = convert_keys(self.get_category(category_id))
         payload["urls"] = urls
 
-        response = self.rest.put(
-            f"urlCategories/{category_id}?action=ADD_TO_LIST", json=payload
-        )
+        response = self.rest.put(f"urlCategories/{category_id}?action=ADD_TO_LIST", json=payload)
         if isinstance(response, Response) and not response.ok:
             # Handle error response
-            raise Exception(
-                f"API call failed with status {response.status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
 
     def delete_urls_from_category(self, category_id: str, urls: list) -> Box:
         """
         Deletes URLS from a URL category.
 
         Args:
             category_id (str):
@@ -359,17 +345,15 @@
         """
         current_config = self.get_category(category_id)
         payload = {
             "configuredName": current_config["configured_name"],
             "urls": urls,
         }  # Required for successful call
 
-        return self.rest.put(
-            f"urlCategories/{category_id}?action=REMOVE_FROM_LIST", json=payload
-        )
+        return self.rest.put(f"urlCategories/{category_id}?action=REMOVE_FROM_LIST", json=payload)
 
     def delete_from_category(self, category_id: str, **kwargs):
         """
         Deletes the specified items from a URL category.
 
         Args:
             category_id (str):
@@ -404,29 +388,25 @@
             ...    urls=['news.com', 'cnn.com'],
             ...    db_categorized_urls=['google.com, bing.com'])
 
         """
         current_config = self.get_category(category_id)
 
         payload = {
-            "configured_name": current_config[
-                "configured_name"
-            ],  # Required for successful call
+            "configured_name": current_config["configured_name"],  # Required for successful call
         }
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
             payload[key] = value
 
         # Convert snake to camelcase
         payload = convert_keys(payload)
 
-        return self.rest.put(
-            f"urlCategories/{category_id}?action=REMOVE_FROM_LIST", json=payload
-        )
+        return self.rest.put(f"urlCategories/{category_id}?action=REMOVE_FROM_LIST", json=payload)
 
     def delete_category(self, category_id: str) -> int:
         """
         Deletes the specified URL category.
 
         Args:
             category_id (str):
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/url_filtering.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/url_filtering.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,17 +190,15 @@
 
         # Send POST request to create the rule
         response = self.rest.post("urlFilteringRules", json=payload)
         if isinstance(response, Response):
             # Handle error response
             status_code = response.status_code
             if status_code != 200:
-                raise Exception(
-                    f"API call failed with status {status_code}: {response.json()}"
-                )
+                raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_rule(self, rule_id: str, **kwargs) -> Box:
         """
         Updates the specified URL Filtering Policy rule.
 
         Args:
@@ -282,17 +280,15 @@
         # Add remaining optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
         response = self.rest.put(f"urlFilteringRules/{rule_id}", json=payload)
         if isinstance(response, Response) and not response.ok:
             # Handle error response
-            raise Exception(
-                f"API call failed with status {response.status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
 
         # Return the updated object
         return self.get_rule(rule_id)
 
     def delete_rule(self, rule_id: str) -> int:
         """
         Deletes the specified URL Filtering Policy rule.
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/users.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,17 +192,15 @@
 
             >>> for user in zia.users.list_users(page_size=200, max_pages=2):
             ...    print(user)
 
         """
         return BoxList(Iterator(self.rest, "users", **kwargs))
 
-    def add_user(
-        self, name: str, email: str, groups: list, department: dict, **kwargs
-    ) -> Box:
+    def add_user(self, name: str, email: str, groups: list, department: dict, **kwargs) -> Box:
         """
         Creates a new ZIA user.
 
         Args:
             name (str):
                 User name.
             email (str):
@@ -289,24 +287,18 @@
             >>> user = zia.users.get_user('99999')
 
             >>> user = zia.users.get_user(email='jane.doe@example.com')
 
         """
 
         if user_id and email:
-            raise ValueError(
-                "TOO MANY ARGUMENTS: Expected either a user_id or an email. Both were provided."
-            )
+            raise ValueError("TOO MANY ARGUMENTS: Expected either a user_id or an email. Both were provided.")
 
         elif email:
-            user = (
-                record
-                for record in self.list_users(search=email)
-                if record.email == email
-            )
+            user = (record for record in self.list_users(search=email) if record.email == email)
             return next(user, None)
 
         return self.rest.get(f"users/{user_id}")
 
     def update_user(
         self,
         user_id: str,
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/web_dlp.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/web_dlp.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,17 +189,15 @@
                 camel_payload[snake_to_camel(key)] = value
 
         # Send POST request to create the rule
         response = self.rest.post("webDlpRules", json=payload)
         if isinstance(response, Response):
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_rule(self, rule_id: str, **kwargs) -> Box:
         """
         Updates an existing DLP policy rule. Not applicable to SaaS Security API DLP policy rules.
 
         Args:
@@ -263,17 +261,15 @@
         # Add remaining optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
         response = self.rest.put(f"webDlpRules/{rule_id}", json=payload)
         if isinstance(response, Response) and not response.ok:
             # Handle error response
-            raise Exception(
-                f"API call failed with status {response.status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {response.status_code}: {response.json()}")
 
         # Return the updated object
         return self.get_rule(rule_id)
 
     def delete_rule(self, rule_id: str) -> Box:
         """
         Deletes a DLP policy rule. This endpoint is not applicable to SaaS Security API DLP policy rules.
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/workload_groups.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/workload_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zia/zpa_gateway.py` & `zscaler_sdk_python-0.1.3/zscaler/zia/zpa_gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,29 +99,26 @@
             payload["zpaServerGroup"] = {
                 "externalId": zpa_server_group.get("external_id"),
                 "name": zpa_server_group.get("name"),
             }
 
         if zpa_app_segments:
             payload["zpaAppSegments"] = [
-                {"externalId": segment.get("external_id"), "name": segment.get("name")}
-                for segment in zpa_app_segments
+                {"externalId": segment.get("external_id"), "name": segment.get("name")} for segment in zpa_app_segments
             ]
 
         # Add other optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
         response = self.rest.post("zpaGateways", json=payload)
         if isinstance(response, Response):
             # Handle error response
             status_code = response.status_code
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_gateway(self, gateway_id: str, **kwargs):
         """
         Updates information for the specified ZPA Gateway.
 
         Args:
@@ -149,27 +146,22 @@
         # Update payload with provided arguments
         for key, value in kwargs.items():
             if key == "zpa_server_group" and isinstance(value, dict):
                 # Convert nested keys in zpa_server_group to camelCase
                 value = {snake_to_camel(k): v for k, v in value.items()}
             elif key == "zpa_app_segments" and isinstance(value, list):
                 # Convert nested keys in zpa_app_segments to camelCase
-                value = [
-                    {snake_to_camel(k): v for k, v in item.items()} for item in value
-                ]
+                value = [{snake_to_camel(k): v for k, v in item.items()} for item in value]
 
             payload[snake_to_camel(key)] = value
 
         response = self.rest.put(f"zpaGateways/{gateway_id}", json=payload)
         if isinstance(response, Response) and not response.ok:
             # Handle error response
-            raise Exception(
-                f"API call failed with status {response.status_code}: "
-                f"{response.json()}"
-            )
+            raise Exception(f"API call failed with status {response.status_code}: " f"{response.json()}")
 
         # Return the updated object
         return self.get_gateway(gateway_id)
 
     def delete_gateway(self, gateway_id):
         """
         Deletes the specified ZPA Gateway.
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/README.md` & `zscaler_sdk_python-0.1.3/zscaler/zpa/README.md`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/__init__.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,17 +113,15 @@
         self.cloud = cloud
         self.url = f"{self.baseurl}/mgmtconfig/v1/admin/customers/{customer_id}"
         self.user_config_url = f"{self.baseurl}/userconfig/v1/customers/{customer_id}"
         self.v2_url = f"{self.baseurl}/mgmtconfig/v2/admin/customers/{customer_id}"
         self.cbi_url = f"{self.baseurl}/cbiconfig/cbi/api/customers/{customer_id}"
         self.fail_safe = fail_safe
         # Cache setup
-        cache_enabled = (
-            os.environ.get("ZSCALER_CLIENT_CACHE_ENABLED", "true").lower() == "true"
-        )
+        cache_enabled = os.environ.get("ZSCALER_CLIENT_CACHE_ENABLED", "true").lower() == "true"
         if cache is None:
             if cache_enabled:
                 ttl = int(os.environ.get("ZSCALER_CLIENT_CACHE_DEFAULT_TTL", 3600))
                 tti = int(os.environ.get("ZSCALER_CLIENT_CACHE_DEFAULT_TTI", 1800))
                 self.cache = ZscalerCache(ttl=ttl, tti=tti)
             else:
                 self.cache = NoOpCache()
@@ -135,32 +133,28 @@
         self.user_agent = ua.get_user_agent_string()
         self.refreshToken()
 
     def refreshToken(self):
         # login
         response = self.login()
         if response is None or response.status_code > 299 or not response.json():
-            logger.error(
-                "Failed to login using provided credentials, response: %s", response
-            )
+            logger.error("Failed to login using provided credentials, response: %s", response)
             raise Exception("Failed to login using provided credentials.")
         self.access_token = response.json().get("access_token")
         self.headers = {
             "Content-Type": "application/json",
             "Accept": "application/json",
             "Authorization": f"Bearer {self.access_token}",
             "User-Agent": self.user_agent,
         }
 
     @retry_with_backoff(retries=5)
     def login(self):
         """Log in to the ZPA API and set the access token for subsequent requests."""
-        data = urllib.parse.urlencode(
-            {"client_id": self.client_id, "client_secret": self.client_secret}
-        )
+        data = urllib.parse.urlencode({"client_id": self.client_id, "client_secret": self.client_secret})
         headers = {
             "Content-Type": "application/x-www-form-urlencoded",
             "Accept": "application/json",
             "User-Agent": self.user_agent,
         }
         try:
             url = f"{self.baseurl}/signin"
@@ -194,17 +188,15 @@
         url = f"{api}/{path.lstrip('/')}"
         start_time = time.time()
         # Update headers to include the user agent
         headers_with_user_agent = self.headers.copy()
         headers_with_user_agent["User-Agent"] = self.user_agent
         # Generate a unique UUID for this request
         request_uuid = uuid.uuid4()
-        dump_request(
-            logger, url, method, json, params, headers_with_user_agent, request_uuid
-        )
+        dump_request(logger, url, method, json, params, headers_with_user_agent, request_uuid)
         # Check cache before sending request
         cache_key = self.cache.create_key(url, params)
         if method == "GET" and self.cache.contains(cache_key):
             resp = self.cache.get(cache_key)
             dump_response(
                 logger=logger,
                 url=url,
@@ -218,17 +210,15 @@
             return resp
 
         attempts = 0
         while attempts < 5:  # Trying a maximum of 5 times
             try:
                 # If the token is None or expired, fetch a new token
                 if is_token_expired(self.access_token):
-                    logger.warning(
-                        "The provided or fetched token was already expired. Refreshing..."
-                    )
+                    logger.warning("The provided or fetched token was already expired. Refreshing...")
                     self.refreshToken()
                 resp = requests.request(
                     method,
                     url,
                     json=json,
                     headers=headers_with_user_agent,
                     timeout=self.timeout,
@@ -238,38 +228,30 @@
                     url=url,
                     params=params,
                     method=method,
                     resp=resp,
                     request_uuid=request_uuid,
                     start_time=start_time,
                 )
-                if (
-                    resp.status_code == 429
-                ):  # HTTP Status code 429 indicates "Too Many Requests"
+                if resp.status_code == 429:  # HTTP Status code 429 indicates "Too Many Requests"
                     sleep_time = int(
                         resp.headers.get("Retry-After", 2)
                     )  # Default to 60 seconds if 'Retry-After' header is missing
-                    logger.warning(
-                        f"Rate limit exceeded. Retrying in {sleep_time} seconds."
-                    )
+                    logger.warning(f"Rate limit exceeded. Retrying in {sleep_time} seconds.")
                     sleep(sleep_time)
                     attempts += 1
                     continue
                 else:
                     break
             except requests.RequestException as e:
                 if attempts == 4:  # If it's the last attempt, raise the exception
-                    logger.error(
-                        f"Failed to send {method} request to {url} after 5 attempts. Error: {str(e)}"
-                    )
+                    logger.error(f"Failed to send {method} request to {url} after 5 attempts. Error: {str(e)}")
                     raise e
                 else:
-                    logger.warning(
-                        f"Failed to send {method} request to {url}. Retrying... Error: {str(e)}"
-                    )
+                    logger.warning(f"Failed to send {method} request to {url}. Retrying... Error: {str(e)}")
                     attempts += 1
                     sleep(5)  # Sleep for 5 seconds before retrying
 
         # If Non-GET call, clear the
         if method != "GET":
             self.cache.delete(cache_key)
 
@@ -398,24 +380,20 @@
             "MISSING_DATA_KEY": "The key 'list' was not found in the response for page {page}.",
             "EMPTY_RESULTS": "No results found for all requested pages.",
         }
 
         if params is None:
             params = {}
 
-        if (page is not None or pagesize != 20) and (
-            max_pages is not None or max_items is not None
-        ):
+        if (page is not None or pagesize != 20) and (max_pages is not None or max_items is not None):
             raise ValueError(
                 "Do not mix 'page' or 'pagesize' with 'max_pages' or 'max_items'. Choose either set of parameters."
             )
 
-        params["pagesize"] = min(
-            pagesize, 500
-        )  # Apply maximum constraint and handle default
+        params["pagesize"] = min(pagesize, 500)  # Apply maximum constraint and handle default
 
         if page:
             params["page"] = page
 
         if search:
             api_search_field = snake_to_camel(search_field)
             params["search"] = f"{api_search_field} EQ {search}"
@@ -445,33 +423,27 @@
                 if should_wait:
                     time.sleep(delay)
 
                 url = f"{path}?{urllib.parse.urlencode(params)}"
                 response = self.send("GET", url, api_version=api_version)
 
                 if response.status_code != expected_status_code:
-                    error_msg = ERROR_MESSAGES["UNEXPECTED_STATUS"].format(
-                        status_code=response.status_code, page=page
-                    )
+                    error_msg = ERROR_MESSAGES["UNEXPECTED_STATUS"].format(status_code=response.status_code, page=page)
                     logger.error(error_msg)
                     return BoxList([]), error_msg
 
                 response_data = response.json()
                 data = response_data.get("list", [])
                 if not data and (page is None or page == 1):
                     error_msg = ERROR_MESSAGES["EMPTY_RESULTS"]
                     logger.warn(error_msg)
                     return BoxList([]), error_msg
 
                 data = convert_keys_to_snake(data)
-                ret_data.extend(
-                    data[: max_items - total_collected]
-                    if max_items is not None
-                    else data
-                )
+                ret_data.extend(data[: max_items - total_collected] if max_items is not None else data)
                 total_collected += len(data)
 
                 if max_items is not None and total_collected >= max_items:
                     break
 
                 nextPage = response_data.get("nextPage")
                 if not nextPage or (max_pages is not None and page >= max_pages):
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/app_segments.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/app_segments.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,17 +55,15 @@
         Returns:
             :obj:`BoxList`: List of application segments.
 
         Examples:
             >>> app_segments = zpa.app_segments.list_segments()
 
         """
-        list, _ = self.rest.get_paginated_data(
-            path="/application", **kwargs, api_version="v1"
-        )
+        list, _ = self.rest.get_paginated_data(path="/application", **kwargs, api_version="v1")
         return list
 
     def get_segment(self, segment_id: str) -> Box:
         """
         Get information for an application segment.
 
         Args:
@@ -203,17 +201,15 @@
                 camel_payload[snake_to_camel(key)] = value
 
         response = self.rest.post("application", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_segment(self, segment_id: str, **kwargs) -> Box:
         """
         Update an application segment.
 
         Args:
@@ -275,34 +271,24 @@
             ...    name='new_app_name',
 
         """
         # Set payload to value of existing record and convert nested dict keys.
         payload = convert_keys(self.get_segment(segment_id))
 
         if kwargs.get("tcp_port_ranges"):
-            payload["tcpPortRange"] = [
-                {"from": ports[0], "to": ports[1]}
-                for ports in kwargs.pop("tcp_port_ranges")
-            ]
+            payload["tcpPortRange"] = [{"from": ports[0], "to": ports[1]} for ports in kwargs.pop("tcp_port_ranges")]
 
         if kwargs.get("udp_port_ranges"):
-            payload["udpPortRange"] = [
-                {"from": ports[0], "to": ports[1]}
-                for ports in kwargs.pop("udp_port_ranges")
-            ]
+            payload["udpPortRange"] = [{"from": ports[0], "to": ports[1]} for ports in kwargs.pop("udp_port_ranges")]
 
         # Handle the clientless_app_ids directly within this function without a separate helper
         if kwargs.get("clientless_app_ids"):
             # Here you would implement any necessary formatting directly
-            formatted_clientless_apps = [
-                {"id": app.get("id")} for app in kwargs.pop("clientless_app_ids")
-            ]
-            payload["clientlessApps"] = (
-                formatted_clientless_apps  # use the correct key expected by your API
-            )
+            formatted_clientless_apps = [{"id": app.get("id")} for app in kwargs.pop("clientless_app_ids")]
+            payload["clientlessApps"] = formatted_clientless_apps  # use the correct key expected by your API
 
         # Convert other keys in payload
         add_id_groups(self.reformat_params, kwargs, payload)
 
         # Add remaining optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/app_segments_inspection.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/app_segments_inspection.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,17 +70,15 @@
     def get_segment_inspection_by_name(self, name):
         apps = self.list_segment_inspection()
         for app in apps:
             if app.get("name") == name:
                 return app
         return None
 
-    def delete_segment_inspection(
-        self, segment_id: str, force_delete: bool = False
-    ) -> int:
+    def delete_segment_inspection(self, segment_id: str, force_delete: bool = False) -> int:
         """
         Delete an AppProtection application segment.
 
         Args:
             force_delete (bool):
                 Setting this field to true deletes the mapping between AppProtection Application Segment and Segment Group.
             segment_id (str):
@@ -204,22 +202,18 @@
                 camel_payload[snake_to_camel(key)] = value
 
         response = self.rest.post("application", json=camel_payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
-    def update_segment_inspection(
-        self, segment_id: str, common_apps_dto=None, **kwargs
-    ) -> Box:
+    def update_segment_inspection(self, segment_id: str, common_apps_dto=None, **kwargs) -> Box:
         """
         Update an AppProtection application segment.
 
         Args:
             segment_id (str):
                 The unique identifier for the AppProtection application segment.
             **kwargs:
@@ -274,32 +268,22 @@
             ...    name='new_app_name',
 
         """
         # Set payload to value of existing record and recursively convert nested dict keys from snake_case to camelCase.
         payload = convert_keys(self.get_segment_inspection(segment_id))
 
         if kwargs.get("tcp_port_ranges"):
-            payload["tcpPortRange"] = [
-                {"from": ports[0], "to": ports[1]}
-                for ports in kwargs.pop("tcp_port_ranges")
-            ]
+            payload["tcpPortRange"] = [{"from": ports[0], "to": ports[1]} for ports in kwargs.pop("tcp_port_ranges")]
 
         if kwargs.get("udp_port_ranges"):
-            payload["udpPortRange"] = [
-                {"from": ports[0], "to": ports[1]}
-                for ports in kwargs.pop("udp_port_ranges")
-            ]
+            payload["udpPortRange"] = [{"from": ports[0], "to": ports[1]} for ports in kwargs.pop("udp_port_ranges")]
 
         if common_apps_dto:
-            camel_common_apps_dto = recursive_snake_to_camel(
-                common_apps_dto
-            )  # use the recursive function
-            payload["commonAppsDto"] = (
-                camel_common_apps_dto  # ensure commonAppsDto gets added to payload
-            )
+            camel_common_apps_dto = recursive_snake_to_camel(common_apps_dto)  # use the recursive function
+            payload["commonAppsDto"] = camel_common_apps_dto  # ensure commonAppsDto gets added to payload
 
         # Convert other keys in payload
         add_id_groups(self.reformat_params, kwargs, payload)
 
         # Add remaining optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/app_segments_pra.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/app_segments_pra.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,22 +201,18 @@
                 camel_payload[snake_to_camel(key)] = value
 
         response = self.rest.post("application", json=camel_payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
-    def update_segment_pra(
-        self, segment_id: str, common_apps_dto=None, **kwargs
-    ) -> Box:
+    def update_segment_pra(self, segment_id: str, common_apps_dto=None, **kwargs) -> Box:
         """
         Update an application segment.
 
         Args:
             segment_id (str):
                 The unique identifier for the application segment.
             **kwargs:
@@ -273,32 +269,22 @@
             ...    name='new_app_name',
 
         """
         # Set payload to value of existing record and recursively convert nested dict keys from snake_case to camelCase.
         payload = convert_keys(self.get_segment_pra(segment_id))
 
         if kwargs.get("tcp_port_ranges"):
-            payload["tcpPortRange"] = [
-                {"from": ports[0], "to": ports[1]}
-                for ports in kwargs.pop("tcp_port_ranges")
-            ]
+            payload["tcpPortRange"] = [{"from": ports[0], "to": ports[1]} for ports in kwargs.pop("tcp_port_ranges")]
 
         if kwargs.get("udp_port_ranges"):
-            payload["udpPortRange"] = [
-                {"from": ports[0], "to": ports[1]}
-                for ports in kwargs.pop("udp_port_ranges")
-            ]
+            payload["udpPortRange"] = [{"from": ports[0], "to": ports[1]} for ports in kwargs.pop("udp_port_ranges")]
 
         if common_apps_dto:
-            camel_common_apps_dto = recursive_snake_to_camel(
-                common_apps_dto
-            )  # use the recursive function
-            payload["commonAppsDto"] = (
-                camel_common_apps_dto  # ensure commonAppsDto gets added to payload
-            )
+            camel_common_apps_dto = recursive_snake_to_camel(common_apps_dto)  # use the recursive function
+            payload["commonAppsDto"] = camel_common_apps_dto  # ensure commonAppsDto gets added to payload
 
         # Convert other keys in payload
         add_id_groups(self.reformat_params, kwargs, payload)
 
         # Add remaining optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/certificates.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/certificates.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,17 +79,15 @@
             :obj:`BoxList`: List of all Browser Access certificates.
 
         Examples:
             >>> for cert in zpa.certificates.list_all_certificates():
             ...    print(cert)
 
         """
-        list, _ = self.rest.get_paginated_data(
-            path="/certificate", **kwargs, api_version="v1"
-        )
+        list, _ = self.rest.get_paginated_data(path="/certificate", **kwargs, api_version="v1")
         return list
 
     def get_certificate_by_name(self, name):
         certs = self.list_all_certificates()
         for cert in certs:
             if cert.get("name") == name:
                 return cert
@@ -217,17 +215,15 @@
             :obj:`BoxList`: List of all enrollment certificates.
 
         Examples:
             >>> for cert in zpa.certificates.list_enrolment():
             ...    print(cert)
 
         """
-        list, _ = self.rest.get_paginated_data(
-            path="/enrollmentCert", **kwargs, api_version="v2"
-        )
+        list, _ = self.rest.get_paginated_data(path="/enrollmentCert", **kwargs, api_version="v2")
         return list
 
     def get_enrolment_cert_by_name(self, name):
         certs = self.list_enrolment()
         for cert in certs:
             if cert.get("name") == name:
                 return cert
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/client.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/client.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/cloud_connector_groups.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/cloud_connector_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/connectors.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/connectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,17 +54,15 @@
         Examples:
             List all configured App Connectors:
 
             >>> for connector in zpa.connectors.list_connectors():
             ...    print(connector)
 
         """
-        list, _ = self.rest.get_paginated_data(
-            path="/connector", **kwargs, api_version="v1"
-        )
+        list, _ = self.rest.get_paginated_data(path="/connector", **kwargs, api_version="v1")
         return list
 
     def get_connector(self, connector_id: str) -> Box:
         """
         Returns information on the specified App Connector.
 
         Args:
@@ -112,17 +110,15 @@
 
             >>> app_connector = zpa.connectors.update_connector('999999',
             ...    name="Updated App Connector Name",
             ...    enabled=False)
 
         """
         # Set payload to equal existing record
-        payload = {
-            snake_to_camel(k): v for k, v in self.get_connector(connector_id).items()
-        }
+        payload = {snake_to_camel(k): v for k, v in self.get_connector(connector_id).items()}
 
         # Perform formatting on simplified params
         add_id_groups(self.reformat_params, kwargs, payload)
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
@@ -181,17 +177,15 @@
         Returns:
             :obj:`BoxList`: List of all configured connector groups.
 
         Examples:
             >>> connector_groups = zpa.connectors.list_connector_groups()
 
         """
-        list, _ = self.rest.get_paginated_data(
-            path="/appConnectorGroup", **kwargs, api_version="v1"
-        )
+        list, _ = self.rest.get_paginated_data(path="/appConnectorGroup", **kwargs, api_version="v1")
         return list
 
     def get_connector_group(self, group_id: str) -> Box:
         """
         Gets information for a specified connector group.
 
         Args:
@@ -216,17 +210,15 @@
     def get_connector_group_by_name(self, name):
         groups = self.list_connector_groups()
         for group in groups:
             if group.get("name") == name:
                 return group
         return None
 
-    def add_connector_group(
-        self, name: str, latitude: int, location: str, longitude: int, **kwargs
-    ) -> Box:
+    def add_connector_group(self, name: str, latitude: int, location: str, longitude: int, **kwargs) -> Box:
         """
         Adds a new ZPA App Connector Group.
 
         Args:
             name (str): The name of the App Connector Group.
             latitude (int): The latitude representing the App Connector's physical location.
             location (str): The name of the location that the App Connector Group represents.
@@ -292,17 +284,15 @@
             payload[snake_to_camel(key)] = value
 
         response = self.rest.post("appConnectorGroup", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_connector_group(self, group_id: str, **kwargs) -> Box:
         """
         Updates an existing ZPA App Connector Group.
 
         Args:
@@ -355,17 +345,15 @@
             ...    name="Updated App Connector Group",
             ...    version_profile="new_release",
             ...    enabled=False)
 
         """
 
         # Set payload to equal existing record
-        payload = {
-            snake_to_camel(k): v for k, v in self.get_connector_group(group_id).items()
-        }
+        payload = {snake_to_camel(k): v for k, v in self.get_connector_group(group_id).items()}
 
         # Perform formatting on simplified params
         add_id_groups(self.reformat_params, kwargs, payload)
         pick_version_profile(kwargs, payload)
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
@@ -460,17 +448,15 @@
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
         response = self.rest.post("assistantSchedule", json=payload)
         if isinstance(response, Response):
             status_code = response.status_code
             if status_code >= 400:  # Check if status code indicates an error
-                raise Exception(
-                    f"API call failed with status {status_code}: {response.json()}"
-                )
+                raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_schedule(self, scheduler_id: str, **kwargs) -> bool:
         """
         Updates App Connector schedule frequency to delete the inactive connectors based on
         the configured frequency.
 
@@ -499,20 +485,16 @@
         # Get the current schedule
         current_schedule = self.get_connector_schedule(scheduler_id=scheduler_id)
 
         # Update the schedule with provided arguments
         for key, value in kwargs.items():
             # Check for customer_id and convert it to int if it's a string
             if key == "customer_id":
-                value = (
-                    int(value) if isinstance(value, str) and value.isdigit() else value
-                )
+                value = int(value) if isinstance(value, str) and value.isdigit() else value
 
             current_schedule[snake_to_camel(key)] = value
 
         # Send the updated schedule to the server
-        response = self.rest.put(
-            f"assistantSchedule/{scheduler_id}", json=current_schedule
-        )
+        response = self.rest.put(f"assistantSchedule/{scheduler_id}", json=current_schedule)
 
         # Return True if the update was successful (204 No Content), False otherwise
         return response.status_code == 204
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/emergency_access.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/emergency_access.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,24 +86,20 @@
         # Include any additional attributes passed via kwargs
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
         # Append 'activateNow=true' to the URL query parameters if activate_now is True
         query_params = {"activateNow": "true"} if activate_now else {}
 
-        response = self.rest.post(
-            "emergencyAccess/user", params=query_params, json=payload
-        )
+        response = self.rest.post("emergencyAccess/user", params=query_params, json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_user(self, user_id: str, **kwargs) -> Box:
         """
         Updates the specified emergency access user.
 
         Args:
@@ -146,23 +142,19 @@
 
         Examples:
             >>> zpa.emergency_access.activate_user('99999', send_email=True)
 
         """
         query_params = {"sendEmail": "true"} if send_email else {}
 
-        response = self.rest.put(
-            f"emergencyAccess/user/{user_id}/activate", params=query_params
-        )
+        response = self.rest.put(f"emergencyAccess/user/{user_id}/activate", params=query_params)
         if response.status_code == 200:
             return self.get_user(user_id)
         else:
-            raise Exception(
-                f"API call failed with status {response.status_code}: {response.text}"
-            )
+            raise Exception(f"API call failed with status {response.status_code}: {response.text}")
 
     def deactivate_user(self, user_id: str) -> Box:
         """
         Deactivates the emergency access user.
 
         Args:
             user_id (str): The unique identifier of the emergency access user to be deactivated.
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/errors.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/errors.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/idp.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/idp.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/inspection.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/inspection.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,29 +102,25 @@
             payload = convert_keys(payload)
 
         response = self.rest.post("inspectionControls/custom", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
         # response = self.rest.post("/inspectionControls/custom", json=payload)
         # if isinstance(response, Response):
         #     status_code = response.status_code
         #     if status_code > 299:
         #         return None
         # return self.get_custom_control(response.get("id"))
 
-    def add_profile(
-        self, name: str, paranoia_level: int, predef_controls_version: str, **kwargs
-    ):
+    def add_profile(self, name: str, paranoia_level: int, predef_controls_version: str, **kwargs):
         """
         Adds a ZPA Inspection Profile.
 
         Args:
             name (str):
                 The name of the Inspection Profile.
             paranoia_level (int):
@@ -212,39 +208,33 @@
             "predefinedControlsVersion": predef_controls_version,
         }
 
         # Extend existing list of default predefined controls if the user supplies more
         if kwargs.get("predef_controls"):
             controls = kwargs.pop("predef_controls")
             for control in controls:
-                payload["predefinedControls"].append(
-                    {"id": control[0], "action": control[1]}
-                )
+                payload["predefinedControls"].append({"id": control[0], "action": control[1]})
 
         # Add custom controls if provided
         if kwargs.get("custom_controls"):
             controls = kwargs.pop("custom_controls")
-            payload["customControls"] = [
-                {"id": control[0], "action": control[1]} for control in controls
-            ]
+            payload["customControls"] = [{"id": control[0], "action": control[1]} for control in controls]
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
             payload[key] = value
 
         payload = convert_keys(payload)
 
         response = self.rest.post("inspectionProfile", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
         # response = self.rest.post("/inspectionProfile", json=payload)
         # if isinstance(response, Response):
         #     status_code = response.status_code
         #     if status_code > 299:
         #         return None
@@ -437,17 +427,15 @@
 
             .. code-block:: python
 
                 for control_type in zpa.inspection.list_custom_control_types():
                     print(control_type)
 
         """
-        return self.rest.get(
-            "https://config.private.zscaler.com/mgmtconfig/v1/admin/inspectionControls/customControlTypes"
-        )
+        return self.rest.get("https://config.private.zscaler.com/mgmtconfig/v1/admin/inspectionControls/customControlTypes")
 
     def list_custom_controls(self, **kwargs) -> BoxList:
         """
         Returns a list of all custom ZPA Inspection Controls.
 
         Args:
             **kwargs: Optional keyword arguments.
@@ -553,31 +541,27 @@
         encoded_version = quote(version, safe="")
 
         # Construct the full URL with version query param
         url = f"/inspectionControls/predefined?version={encoded_version}"
 
         # If you have additional query parameters, add them to the URL
         if kwargs:
-            additional_params = "&".join(
-                f"{key}={quote(str(value))}" for key, value in kwargs.items()
-            )
+            additional_params = "&".join(f"{key}={quote(str(value))}" for key, value in kwargs.items())
             url += f"&{additional_params}"
 
         # Make the GET request
         response = self.rest.get(url)
         if isinstance(response, Response):
             status_code = response.status_code
             if status_code != 200:
                 # Handle error or return None based on your API handling
                 return None
         return response
 
-    def get_predef_control_by_name(
-        self, name: str, version: str = "OWASP_CRS/3.3.0"
-    ) -> Box:
+    def get_predef_control_by_name(self, name: str, version: str = "OWASP_CRS/3.3.0") -> Box:
         """
         Returns the specified predefined ZPA Inspection Control by its name.
 
         Args:
             name (str):
                 The name of the predefined ZPA Inspection Control to be returned.
             version (str):
@@ -602,17 +586,15 @@
             for control in control_group.get("predefined_inspection_controls", []):
                 if control["name"] == name:
                     return control
 
         # If we reach here, the control was not found
         raise ValueError(f"No predefined control named '{name}' found")
 
-    def get_predef_control_group_by_name(
-        self, group_name: str, version: str = "OWASP_CRS/3.3.0"
-    ) -> Box:
+    def get_predef_control_group_by_name(self, group_name: str, version: str = "OWASP_CRS/3.3.0") -> Box:
         """
         Returns the specified predefined ZPA Inspection Control Group by its name.
 
         Args:
             group_name (str):
                 The name of the predefined ZPA Inspection Control Group to be returned.
             version (str):
@@ -726,32 +708,20 @@
         """
         if action == "attach":
             payload = {"version": kwargs.pop("profile_version", "OWASP_CRS/3.3.0")}
             resp = self.rest.put(
                 f"inspectionProfile/{profile_id}/associateAllPredefinedControls",
                 params=payload,
             )
-            return (
-                self.get_profile(profile_id)
-                if resp.status_code == 204
-                else resp.status_code
-            )
+            return self.get_profile(profile_id) if resp.status_code == 204 else resp.status_code
         elif action == "detach":
-            resp = self.rest.put(
-                f"inspectionProfile/{profile_id}/deAssociateAllPredefinedControls"
-            )
-            return (
-                self.get_profile(profile_id)
-                if resp.status_code == 204
-                else resp.status_code
-            )
+            resp = self.rest.put(f"inspectionProfile/{profile_id}/deAssociateAllPredefinedControls")
+            return self.get_profile(profile_id) if resp.status_code == 204 else resp.status_code
         else:
-            raise ValueError(
-                "Unknown action provided. Valid actions are 'attach' or 'detach'."
-            )
+            raise ValueError("Unknown action provided. Valid actions are 'attach' or 'detach'.")
 
     def update_custom_control(self, control_id: str, **kwargs) -> Box:
         """
         Updates the specified custom ZPA Inspection Control.
 
         Args:
             control_id (str):
@@ -850,17 +820,15 @@
             payload_key = snake_to_camel(key)
             payload[payload_key] = value
 
             # Special handling for default_action_value
             if key == "default_action_value":
                 payload["defaultActionValue"] = value
 
-        resp = self.rest.put(
-            f"inspectionControls/custom/{control_id}", json=payload
-        ).status_code
+        resp = self.rest.put(f"inspectionControls/custom/{control_id}", json=payload).status_code
 
         # Return the object if it was updated successfully
         if not isinstance(resp, Response):
             return self.get_custom_control(control_id)
 
     def update_profile(self, profile_id: str, **kwargs):
         """
@@ -934,51 +902,41 @@
                         custom_controls=[("2", "BLOCK")],
                     )
                 )
 
         """
         # Set payload to value of existing record
         payload = self.get_profile(profile_id)
-        payload["predefinedControlsVersion"] = kwargs.get(
-            "predef_controls_version", "OWASP_CRS/3.3.0"
-        )
+        payload["predefinedControlsVersion"] = kwargs.get("predef_controls_version", "OWASP_CRS/3.3.0")
 
         # Extend existing list of default predefined controls if the user supplies more
         if kwargs.get("predef_controls"):
             controls = kwargs.pop("predef_controls")
             for control in controls:
-                payload["predefined_controls"] = [
-                    {"id": control[0], "action": control[1]} for control in controls
-                ]
+                payload["predefined_controls"] = [{"id": control[0], "action": control[1]} for control in controls]
 
         # Add custom controls if provided
         if kwargs.get("custom_controls"):
             controls = kwargs.pop("custom_controls")
-            payload["custom_controls"] = [
-                {"id": control[0], "action": control[1]} for control in controls
-            ]
+            payload["custom_controls"] = [{"id": control[0], "action": control[1]} for control in controls]
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
             payload[key] = value
 
         # Convert from snake case to camel case
         payload = convert_keys(payload)
 
-        resp = self.rest.put(
-            f"inspectionProfile/{profile_id}", json=payload
-        ).status_code
+        resp = self.rest.put(f"inspectionProfile/{profile_id}", json=payload).status_code
 
         # Return the object if it was updated successfully
         if not isinstance(resp, Response):
             return self.get_profile(profile_id)
 
-    def update_profile_and_controls(
-        self, profile_id: str, inspection_profile: dict, **kwargs
-    ):
+    def update_profile_and_controls(self, profile_id: str, inspection_profile: dict, **kwargs):
         """
         Updates the inspection profile and controls for the specified ID.
 
         Note:
             This method has not been fully implemented and will not be maintained. There seems to be functionality
             duplication with the default Inspection Profile update API call. `**kwargs` has been provided as a parameter
             for you to be able to add any additional args that Zscaler may add.
@@ -999,14 +957,12 @@
         payload = {
             "inspection_profile_id": profile_id,
             "inspection_profile": inspection_profile,
         }
 
         payload = convert_keys(payload)
 
-        resp = self.rest.put(
-            "inspectionProfile/{profile_id}/patch", json=payload
-        ).status_code
+        resp = self.rest.put("inspectionProfile/{profile_id}/patch", json=payload).status_code
 
         # Return the object if it was updated successfully
         if not isinstance(resp, Response):
             return self.get_profile(profile_id)
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/lss.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/lss.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,15 @@
         "user_status": "zpn_auth_log",
         "web_inspection": "zpn_waf_http_exchanges_log",
     }
 
     def __init__(self, client: ZPAClient):
         self.rest = client
 
-        self.v2_admin_url = (
-            "https://config.private.zscaler.com/mgmtconfig/v2/admin/lssConfig"
-        )
+        self.v2_admin_url = "https://config.private.zscaler.com/mgmtconfig/v2/admin/lssConfig"
 
     def _create_policy(self, conditions: list) -> list:
         """
         Creates a dict template for feeding conditions into the ZPA Policies API when adding or updating a policy.
 
         Args:
             conditions (list): List of condition tuples.
@@ -54,35 +52,29 @@
 
         """
 
         template = []
 
         for condition in conditions:
             # Template for SAML Policy Rule objects
-            if (
-                isinstance(condition, tuple)
-                and len(condition) == 2
-                and condition[0] == "saml"
-            ):
+            if isinstance(condition, tuple) and len(condition) == 2 and condition[0] == "saml":
                 operand = {"operands": [{"objectType": "SAML", "entryValues": []}]}
                 for item in condition[1]:
                     entry_values = {
                         "lhs": item[0],
                         "rhs": item[1],
                     }
                     operand["operands"][0]["entryValues"].append(entry_values)
             # Template for client_type Policy Rule objects
             elif condition[0] == "client_type":
                 operand = {
                     "operands": [
                         {
                             "objectType": condition[0].upper(),
-                            "values": [
-                                self.get_client_types()[item] for item in condition[1]
-                            ],
+                            "values": [self.get_client_types()[item] for item in condition[1]],
                         }
                     ]
                 }
             # Template for all other object types
             else:
                 operand = {
                     "operands": [
@@ -118,17 +110,15 @@
         # before returning it so that a lookup can be easily performed using the Client Type name in plain english.
         #
         # Example before:
         # {'zpn_client_type_exporter': 'Web Browser'}
         # Example after:
         # {'web_browser': 'zpn_client_type_exporter'}
 
-        response = requests.get(
-            f"{self.v2_admin_url}/clientTypes", headers=self.rest.headers
-        )
+        response = requests.get(f"{self.v2_admin_url}/clientTypes", headers=self.rest.headers)
 
         if response.status_code == 200:
             return response.json()
         else:
             response.raise_for_status()
 
         reverse_map = {v.lower().replace(" ", "_"): k for k, v in response.items()}
@@ -153,17 +143,15 @@
 
         Examples:
             Print all configured LSS Receivers.
 
             >>> for lss_config in zpa.lss.list_configs():
             ...    print(config)
         """
-        list, _ = self.rest.get_paginated_data(
-            path="/lssConfig", **kwargs, api_version="v2"
-        )
+        list, _ = self.rest.get_paginated_data(path="/lssConfig", **kwargs, api_version="v2")
         return list
 
     def get_config(self, lss_id: str) -> Box:
         """
         Returns information on the specified LSS Receiver config.
 
         Args:
@@ -197,17 +185,15 @@
             :obj:`Box`: Dictionary containing pre-configured LSS Log Formats.
 
         Examples:
             >>> for item in zpa.lss.get_log_formats():
             ...    print(item)
 
         """
-        response = requests.get(
-            f"{self.v2_admin_url}/logType/formats", headers=self.rest.headers
-        )
+        response = requests.get(f"{self.v2_admin_url}/logType/formats", headers=self.rest.headers)
 
         if response.status_code == 200:
             return response.json()
         else:
             response.raise_for_status()
 
     def get_status_codes(self, log_type: str = "all") -> Box:
@@ -386,31 +372,27 @@
         source_log_type = self.source_log_map[source_log_type]
 
         # If the user has supplied custom log stream content formatting then we'll use that. Otherwise map the log
         # type to internal ZPA log codes and get the preformatted log stream content formatting directly from ZPA.
         if kwargs.get("log_stream_content"):
             log_stream_content = kwargs.pop("log_stream_content")
         else:
-            log_stream_content = self.get_log_formats()[source_log_type][
-                source_log_format
-            ]
+            log_stream_content = self.get_log_formats()[source_log_type][source_log_format]
 
         payload = {
             "config": {
                 "enabled": enabled,
                 "lssHost": lss_host,
                 "lssPort": lss_port,
                 "name": name,
                 "format": log_stream_content,
                 "sourceLogType": source_log_type,
                 "useTls": use_tls,
             },
-            "connectorGroups": [
-                {"id": group_id} for group_id in app_connector_group_ids
-            ],
+            "connectorGroups": [{"id": group_id} for group_id in app_connector_group_ids],
         }
 
         # Convert tuple list to dict and add to payload
         if kwargs.get("policy_rules"):
             payload["policyRuleResource"] = {
                 "conditions": self._create_policy(kwargs.pop("policy_rules")),
                 "name": kwargs.get("policy_name", "SIEM_POLICY"),
@@ -425,17 +407,15 @@
             payload[snake_to_camel(key)] = value
 
         response = self.rest.post("/lssConfig", api_version="v2", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_lss_config(self, lss_config_id: str, **kwargs):
         """
         Update the LSS Receiver Config.
 
         Args:
@@ -510,17 +490,15 @@
         # If the user has supplied custom log stream content formatting then we'll use that. Otherwise, map the log
         # type to internal ZPA log codes and get the preformatted log stream content formatting directly from ZPA.
         if kwargs.get("log_stream_content"):
             payload["config"]["format"] = kwargs.pop("log_stream_content")
         elif kwargs.get("source_log_type"):
             source_log_type = self.source_log_map[kwargs.pop("source_log_type")]
             payload["config"]["sourceLogType"] = source_log_type
-            payload["config"]["format"] = self.get_log_formats()[source_log_type][
-                kwargs.pop("source_log_format", "csv")
-            ]
+            payload["config"]["format"] = self.get_log_formats()[source_log_type][kwargs.pop("source_log_format", "csv")]
 
         # Iterate kwargs and update payload for keys that we've renamed.
         for k in list(kwargs):
             if k in ["name", "lss_host", "lss_port", "enabled", "use_tls"]:
                 payload["config"][snake_to_camel(k)] = kwargs.pop(k)
             elif k == "filter_status_codes":
                 payload["config"]["filter"] = kwargs.pop(k)
@@ -536,17 +514,15 @@
                 "name": kwargs.pop("policy_name", policy_name),
             }
 
         # Add additional provided parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
-        resp = self.rest.put(
-            f"/lssConfig/{lss_config_id}", api_version="v2", json=payload
-        ).status_code
+        resp = self.rest.put(f"/lssConfig/{lss_config_id}", api_version="v2", json=payload).status_code
 
         # Return the object if it was updated successfully
         if not isinstance(resp, Response):
             return self.get_config(lss_config_id)
 
     def delete_lss_config(self, lss_id: str) -> int:
         """
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/policies.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,22 +308,18 @@
         payload = {
             "name": name,
             "action": action.upper(),
             "conditions": self._create_conditions(kwargs.pop("conditions", [])),
         }
 
         if app_connector_group_ids:
-            payload["appConnectorGroups"] = [
-                {"id": group_id} for group_id in app_connector_group_ids
-            ]
+            payload["appConnectorGroups"] = [{"id": group_id} for group_id in app_connector_group_ids]
 
         if app_server_group_ids:
-            payload["appServerGroups"] = [
-                {"id": group_id} for group_id in app_server_group_ids
-            ]
+            payload["appServerGroups"] = [{"id": group_id} for group_id in app_server_group_ids]
 
         add_id_groups(self.reformat_params, kwargs, payload)
 
         # Get the policy id of the provided policy type for the URL.
         policy_id = self.get_policy("access").id
 
         # Add optional parameters to payload
@@ -331,17 +327,15 @@
             payload[snake_to_camel(key)] = value
 
         response = self.rest.post(f"policySet/{policy_id}/rule", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def add_timeout_rule(self, name: str, **kwargs) -> Box:
         """
         Add a new Timeout Policy rule.
 
         See the `ZPA Timeout Policy API reference <https://help.zscaler.com/zpa/timeout-policy-use-cases>`_
@@ -400,17 +394,15 @@
             payload[snake_to_camel(key)] = value
 
         response = self.rest.post(f"policySet/{policy_id}/rule", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def add_client_forwarding_rule(self, name: str, action: str, **kwargs) -> Box:
         """
         Add a new Client Forwarding Policy rule.
 
         See the
@@ -468,22 +460,18 @@
             payload[snake_to_camel(key)] = value
 
         response = self.rest.post(f"policySet/{policy_id}/rule", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
-    def add_isolation_rule(
-        self, name: str, action: str, zpn_isolation_profile_id: str, **kwargs
-    ) -> Box:
+    def add_isolation_rule(self, name: str, action: str, zpn_isolation_profile_id: str, **kwargs) -> Box:
         """
         Add a new Isolation Policy rule.
 
         See the
         `ZPA Isolation Policy API reference <https://help.zscaler.com/zpa/configuring-isolation-policies-using-api>`_
         for further detail on optional keyword parameter structures.
 
@@ -537,22 +525,18 @@
             payload[snake_to_camel(key)] = value
 
         response = self.rest.post(f"policySet/{policy_id}/rule", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
-    def add_app_protection_rule(
-        self, name: str, action: str, zpn_inspection_profile_id: str, **kwargs
-    ) -> Box:
+    def add_app_protection_rule(self, name: str, action: str, zpn_inspection_profile_id: str, **kwargs) -> Box:
         """
         Add a new AppProtection Policy rule.
 
         See the
         `ZPA AppProtection Policy API reference <https://help.zscaler.com/zpa/configuring-appprotection-policies-using-api>`_
         for further detail on optional keyword parameter structures.
 
@@ -606,17 +590,15 @@
             payload[snake_to_camel(key)] = value
 
         response = self.rest.post(f"policySet/{policy_id}/rule", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_rule(self, policy_type: str, rule_id: str, **kwargs) -> Box:
         """
         Update an existing policy rule.
 
         Ensure you are using the correct arguments for the policy type that you want to update.
@@ -685,17 +667,15 @@
         # Add optional parameters to payload
         for key, value in kwargs.items():
             if key == "conditions":
                 payload["conditions"] = self._create_conditions(value)
             else:
                 payload[snake_to_camel(key)] = value
 
-        resp = self.rest.put(
-            f"policySet/{policy_id}/rule/{rule_id}", json=payload
-        ).status_code
+        resp = self.rest.put(f"policySet/{policy_id}/rule/{rule_id}", json=payload).status_code
 
         # Return the object if it was updated successfully
         if not isinstance(resp, Response):
             return self.get_rule(policy_type, rule_id)
 
     def update_access_rule(
         self,
@@ -748,17 +728,15 @@
         # Add optional parameters to payload
         for key, value in kwargs.items():
             if key == "conditions":
                 payload["conditions"] = self._create_conditions(value)
             else:
                 payload[snake_to_camel(key)] = value
 
-        resp = self.rest.put(
-            f"policySet/{policy_id}/rule/{rule_id}", json=payload
-        ).status_code
+        resp = self.rest.put(f"policySet/{policy_id}/rule/{rule_id}", json=payload).status_code
 
         # Return the object if it was updated successfully
         if not isinstance(resp, Response):
             return self.get_rule(policy_type, rule_id)
 
     def reorder_rule(self, policy_type: str, rule_id: str, rule_order: str) -> Box:
         """
@@ -786,17 +764,15 @@
             ...    rule_id='88888',
             ...    rule_order='2')
 
         """
         # Get policy id for specified policy type
         policy_id = self.get_policy(policy_type).id
 
-        resp = self._put(
-            f"policySet/{policy_id}/rule/{rule_id}/reorder/{rule_order}"
-        ).status_code
+        resp = self._put(f"policySet/{policy_id}/rule/{rule_id}/reorder/{rule_order}").status_code
 
         if resp == 204:
             return self.get_rule(policy_type, rule_id)
 
     def sort_key(self, rules_orders: dict[str, int]):
         def key(a, b):
             if a.id in rules_orders and b.id in rules_orders:
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/posture_profiles.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/posture_profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,17 +44,15 @@
         Returns:
             BoxList: A list of all configured posture profiles.
 
         Examples:
             >>> for posture_profile in zpa.posture_profiles.list_profiles():
             ...    pprint(posture_profile)
         """
-        list, _ = self.rest.get_paginated_data(
-            path="/posture", **kwargs, api_version="v2"
-        )
+        list, _ = self.rest.get_paginated_data(path="/posture", **kwargs, api_version="v2")
         return list
 
     def get_profile_by_name(self, name):
         profiles = self.list_profiles()
         for profile in profiles:
             if profile.get("name") == name:
                 return profile
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/privileged_remote_access.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/privileged_remote_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,15 @@
             :obj:`BoxList`: A list of all configured privileged remote access portals.
 
         Examples:
             >>> for pra_portal in zpa.privileged_remote_access.list_portals():
             ...    pprint(pra_portal)
 
         """
-        list, _ = self.rest.get_paginated_data(
-            path="/praPortal", **kwargs, api_version="v1"
-        )
+        list, _ = self.rest.get_paginated_data(path="/praPortal", **kwargs, api_version="v1")
         return list
 
     def get_portal(self, portal_id: str) -> Box:
         """
         Returns information on the specified pra portal.
 
         Args:
@@ -223,17 +221,15 @@
             :obj:`BoxList`: A list of all configured privileged remote access consoles.
 
         Examples:
             >>> for pra_console in zpa.privileged_remote_access.list_consoles():
             ...    pprint(pra_console)
 
         """
-        list, _ = self.rest.get_paginated_data(
-            path="/praConsole", **kwargs, api_version="v1"
-        )
+        list, _ = self.rest.get_paginated_data(path="/praConsole", **kwargs, api_version="v1")
         return list
 
     def get_console(self, console_id: str) -> Box:
         """
         Returns information on the specified pra console.
 
         Args:
@@ -310,17 +306,15 @@
             payload[snake_to_camel(key)] = value
 
         response = self.rest.post("praConsole", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_console(
         self,
         console_id: str,
         pra_application_id: str = None,
         pra_portal_ids: list = None,
@@ -433,17 +427,15 @@
             for console in consoles
         ]
 
         response = self.rest.post("praConsole/bulk", json=payload)
         if isinstance(response, Response):
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def list_credentials(self, **kwargs) -> BoxList:
         """
         Returns a list of all privileged remote access credentials.
 
         Keyword Args:
@@ -460,17 +452,15 @@
             :obj:`BoxList`: A list of all configured privileged remote access credentials.
 
         Examples:
             >>> for pra_credential in zpa.privileged_remote_access.list_credentials():
             ...    pprint(pra_credential)
 
         """
-        list, _ = self.rest.get_paginated_data(
-            path="/credential", **kwargs, api_version="v1"
-        )
+        list, _ = self.rest.get_paginated_data(path="/credential", **kwargs, api_version="v1")
         return list
 
     def get_credential(self, credential_id: str) -> Box:
         """
         Returns information on the specified pra credential.
 
         Args:
@@ -504,24 +494,20 @@
         """
         Validates input based on credential_type and adds a new credential.
         """
         payload = {"name": name, "credentialType": credential_type}
 
         if credential_type == "USERNAME_PASSWORD":
             if not username or not password:
-                raise ValueError(
-                    "Username and password must be provided for USERNAME_PASSWORD type."
-                )
+                raise ValueError("Username and password must be provided for USERNAME_PASSWORD type.")
             payload.update({"userName": username, "password": password})
 
         elif credential_type == "SSH_KEY":
             if not username or not private_key:
-                raise ValueError(
-                    "Username and private_key must be provided for SSH_KEY type."
-                )
+                raise ValueError("Username and private_key must be provided for SSH_KEY type.")
             if not is_valid_ssh_key(private_key):
                 raise ValueError("Invalid SSH key format.")
             payload.update({"userName": username, "privateKey": private_key})
 
         elif credential_type == "PASSWORD":
             if not password:
                 raise ValueError("Password must be provided for PASSWORD type.")
@@ -536,17 +522,15 @@
                 payload[snake_to_camel(key)] = value
 
         response = self.rest.post("credential", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_credential(self, credential_id: str, **kwargs) -> Box:
         """
         Updates a specified credential based on provided keyword arguments.
 
         Args:
@@ -581,37 +565,29 @@
         # Fetch the existing credential to determine the credential type
         existing_credential = self.get_credential(credential_id)
         if not existing_credential:
             raise Exception(f"Failed to fetch credential {credential_id}")
 
         # Validate and enforce required fields based on the credential type
         credential_type = existing_credential.credential_type
-        required_fields = (
-            ["username", "password"]
-            if credential_type in ["USERNAME_PASSWORD", "SSH_KEY"]
-            else ["password"]
-        )
+        required_fields = ["username", "password"] if credential_type in ["USERNAME_PASSWORD", "SSH_KEY"] else ["password"]
         missing_fields = [field for field in required_fields if field not in kwargs]
         if missing_fields:
-            raise ValueError(
-                f"Missing required fields for '{credential_type}': {', '.join(missing_fields)}"
-            )
+            raise ValueError(f"Missing required fields for '{credential_type}': {', '.join(missing_fields)}")
 
         # Prepare the payload with the existing details and updates from kwargs
         payload = {
             **existing_credential.to_dict(),
             **{snake_to_camel(key): value for key, value in kwargs.items()},
         }
 
         # Execute the update operation
         response = self.rest.put(f"credential/{credential_id}", json=payload)
         if not response.ok:
-            raise Exception(
-                f"Failed to update credential {credential_id}: {response.text}"
-            )
+            raise Exception(f"Failed to update credential {credential_id}: {response.text}")
 
         # Fetch and return the updated credential details
         return self.get_credential(credential_id)
 
     def delete_credential(self, credential_id: str) -> int:
         """
         Delete the specified pra credential.
@@ -665,17 +641,15 @@
 
             >>> approvals = zpa.privileged_remote_access.list_approval(
             ...     search='Example_Name', search_field='name', max_items=10)
             ... for approval in approvals:
             ...     pprint(approval)
 
         """
-        list, _ = self.rest.get_paginated_data(
-            path="/approval", **kwargs, api_version="v1"
-        )
+        list, _ = self.rest.get_paginated_data(path="/approval", **kwargs, api_version="v1")
         return list
 
     def get_approval(self, approval_id: str) -> Box:
         """
         Returns information on the specified pra approval.
 
         Args:
@@ -733,23 +707,19 @@
             ...       "start_time": "09:00",
             ...       "end_time": "17:00",
             ...       "days": ["SUN", "MON", "TUE", "WED", "THU", "FRI", "SAT"],
             ...       "time_zone": "America/Vancouver"
             ...   }
             ... )
         """
-        start_epoch, end_epoch = validate_and_convert_times(
-            start_time, end_time, working_hours["time_zone"]
-        )
+        start_epoch, end_epoch = validate_and_convert_times(start_time, end_time, working_hours["time_zone"])
 
         payload = {
             "emailIds": email_ids,
-            "applications": [
-                {"id": application_id} for application_id in application_ids
-            ],
+            "applications": [{"id": application_id} for application_id in application_ids],
             "startTime": start_epoch,
             "endTime": end_epoch,
             "status": status,
             "workingHours": {
                 "startTimeCron": working_hours["start_time_cron"],
                 "endTimeCron": working_hours["end_time_cron"],
                 "startTime": working_hours["start_time"],
@@ -763,17 +733,15 @@
             payload[snake_to_camel(key)] = value
 
         response = self.rest.post("approval", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_approval(self, approval_id: str, **kwargs) -> Box:
         """
         Updates a specified approval based on provided keyword arguments.
         ...
         """
@@ -783,20 +751,16 @@
             raise Exception(f"Failed to fetch approval {approval_id}")
 
         # Pre-process and validate start_time and end_time if provided
         if "start_time" in kwargs and "end_time" in kwargs:
             start_time = kwargs["start_time"]
             end_time = kwargs["end_time"]
             # Assuming working_hours contains the time zone
-            time_zone = kwargs.get("working_hours", {}).get(
-                "time_zone", existing_approval.working_hours.time_zone
-            )
-            start_epoch, end_epoch = validate_and_convert_times(
-                start_time, end_time, time_zone
-            )
+            time_zone = kwargs.get("working_hours", {}).get("time_zone", existing_approval.working_hours.time_zone)
+            start_epoch, end_epoch = validate_and_convert_times(start_time, end_time, time_zone)
             kwargs["start_time"] = start_epoch
             kwargs["end_time"] = end_epoch
 
         # Construct payload dynamically based on existing details and updates from kwargs
         payload = {
             "emailIds": kwargs.get("email_ids", existing_approval.email_ids),
             "applications": [
@@ -809,20 +773,16 @@
             "status": kwargs.get("status", existing_approval.status),
         }
 
         # Special handling for working_hours to preserve existing details if not fully specified in kwargs
         working_hours = kwargs.get("working_hours", {})
         existing_wh = existing_approval.working_hours
         payload["workingHours"] = {
-            "startTimeCron": working_hours.get(
-                "start_time_cron", existing_wh.start_time_cron
-            ),
-            "endTimeCron": working_hours.get(
-                "end_time_cron", existing_wh.end_time_cron
-            ),
+            "startTimeCron": working_hours.get("start_time_cron", existing_wh.start_time_cron),
+            "endTimeCron": working_hours.get("end_time_cron", existing_wh.end_time_cron),
             "startTime": working_hours.get("start_time", existing_wh.start_time),
             "endTime": working_hours.get("end_time", existing_wh.end_time),
             "days": working_hours.get("days", existing_wh.days),
             "timeZone": working_hours.get("time_zone", existing_wh.time_zone),
         }
 
         # Add any additional provided parameters to payload
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/provisioning.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/provisioning.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,17 +97,15 @@
 
             Get the specified Service Edge key.
 
             >>> provisioning_key = zpa.provisioning.get_provisioning_key("888888",
             ...    key_type="service_edge")
 
         """
-        return self.rest.get(
-            f"associationType/{simplify_key_type(key_type)}/provisioningKey/{key_id}"
-        )
+        return self.rest.get(f"associationType/{simplify_key_type(key_type)}/provisioningKey/{key_id}")
 
     def add_provisioning_key(
         self,
         key_type: str,
         name: str,
         max_usage: str,
         enrollment_cert_id: str,
@@ -171,17 +169,15 @@
             f"associationType/{simplify_key_type(key_type)}/provisioningKey",
             json=payload,
         )
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_provisioning_key(self, key_id: str, key_type: str, **kwargs) -> Box:
         """
         Updates the specified provisioning key.
 
         Args:
@@ -215,18 +211,15 @@
             >>> updated_key = zpa.provisioning.update_provisioning_key('888888',
             ...    key_type="service_edge",
             ...    max_usage=10)
 
         """
 
         # Get the provided provisioning key record
-        payload = {
-            snake_to_camel(k): v
-            for k, v in self.get_provisioning_key(key_id, key_type=key_type).items()
-        }
+        payload = {snake_to_camel(k): v for k, v in self.get_provisioning_key(key_id, key_type=key_type).items()}
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
         resp = self.rest.put(
             f"associationType/{simplify_key_type(key_type)}/provisioningKey/{key_id}",
@@ -262,10 +255,8 @@
 
             Delete a Service Edge provisioning key:
 
             >>> zpa.provisioning.delete_provisioning_key(key_id="888888",
             ...    key_type="service_edge")
 
         """
-        return self.rest.delete(
-            f"associationType/{simplify_key_type(key_type)}/provisioningKey/{key_id}"
-        ).status_code
+        return self.rest.delete(f"associationType/{simplify_key_type(key_type)}/provisioningKey/{key_id}").status_code
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/saml_attributes.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/saml_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,15 @@
             :obj:`BoxList`: A list of all configured SAML attributes.
 
         Examples:
             >>> for saml_attribute in zpa.saml_attributes.list_attributes():
             ...    pprint(saml_attribute)
 
         """
-        list, _ = self.rest.get_paginated_data(
-            path="/samlAttribute", **kwargs, api_version="v2"
-        )
+        list, _ = self.rest.get_paginated_data(path="/samlAttribute", **kwargs, api_version="v2")
         return list
 
     def list_attributes_by_idp(self, idp_id: str, **kwargs) -> BoxList:
         """
         Returns a list of all configured SAML attributes for the specified IdP.
 
         Args:
@@ -72,17 +70,15 @@
             :obj:`BoxList`: A list of all configured SAML attributes for the specified IdP.
 
         Examples:
             >>> for saml_attribute in zpa.saml_attributes.list_attributes_by_idp('99999'):
             ...    pprint(saml_attribute)
 
         """
-        path = (
-            f"/samlAttribute/idp/{idp_id}"  # Correctly format the path with the idp_id
-        )
+        path = f"/samlAttribute/idp/{idp_id}"  # Correctly format the path with the idp_id
         list, _ = self.rest.get_paginated_data(path=path, **kwargs, api_version="v2")
         return list
 
     def get_attribute(self, attribute_id: str) -> Box:
         """
         Returns information on the specified SAML attributes.
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/scim_attributes.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/scim_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,17 +71,15 @@
             :obj:`Box`: The resource record for the SCIM attribute.
 
         Examples:
             >>> pprint(zpa.scim_attributes.get_attribute('99999',
             ...    scim_attribute_id="88888"))
 
         """
-        response = self.rest.get(
-            f"/idp/{idp_id}/scimattribute/{attribute_id}", api_version="v1"
-        )
+        response = self.rest.get(f"/idp/{idp_id}/scimattribute/{attribute_id}", api_version="v1")
         return response
 
     def get_values(self, idp_id: str, attribute_id: str, **kwargs) -> BoxList:
         """
         Returns information on the specified SCIM attributes.
 
         Args:
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/scim_groups.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/scim_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,17 +88,15 @@
         Returns:
             :obj:`dict`: The resource record for the SCIM group.
 
         Examples:
             >>> pprint(zpa.scim_groups.get_group('99999'))
 
         """
-        response = self.rest.get(
-            f"/scimgroup/{group_id}", **kwargs, api_version="userconfig_v1"
-        )
+        response = self.rest.get(f"/scimgroup/{group_id}", **kwargs, api_version="userconfig_v1")
         return response
 
     def search_group(self, idp_id: str, group_name: str, **kwargs) -> dict:
         """
         Searches and returns the SCIM group with the specified name for the given IdP.
         """
         page_size = kwargs.get("pagesize", 500)  # Adjust the page size as needed
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/segment_groups.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/segment_groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,17 +35,15 @@
             :obj:`BoxList`: A list of all configured segment groups.
 
         Examples:
             >>> for segment_group in zpa.segment_groups.list_groups():
             ...    pprint(segment_group)
 
         """
-        list, _ = self.rest.get_paginated_data(
-            path="/segmentGroup", **kwargs, api_version="v1"
-        )
+        list, _ = self.rest.get_paginated_data(path="/segmentGroup", **kwargs, api_version="v1")
         return list
 
     def get_group(self, group_id: str) -> Box:
         """
         Returns information on the specified segment group.
 
         Args:
@@ -101,30 +99,26 @@
 
         payload = {
             "name": name,
             "enabled": enabled,
         }
 
         if kwargs.get("application_ids"):
-            payload["applications"] = [
-                {"id": app_id} for app_id in kwargs.pop("application_ids")
-            ]
+            payload["applications"] = [{"id": app_id} for app_id in kwargs.pop("application_ids")]
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
         response = self.rest.post("segmentGroup", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_group(self, group_id: str, **kwargs) -> Box:
         """
         Updates an existing segment group.
 
         Args:
@@ -155,17 +149,15 @@
             ...    name='updated_name')
 
         """
         # Set payload to value of existing record
         payload = {snake_to_camel(k): v for k, v in self.get_group(group_id).items()}
 
         if kwargs.get("application_ids"):
-            payload["applications"] = [
-                {"id": app_id} for app_id in kwargs.pop("application_ids")
-            ]
+            payload["applications"] = [{"id": app_id} for app_id in kwargs.pop("application_ids")]
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
         resp = self.rest.put(f"segmentGroup/{group_id}", json=payload).status_code
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/server_groups.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/server_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,17 +49,15 @@
             :obj:`BoxList`: A list of all configured server groups.
 
         Examples:
             >>> for server_group in zpa.server_groups.list_groups():
             ...    pprint(server_group)
 
         """
-        list, _ = self.rest.get_paginated_data(
-            path="/serverGroup", **kwargs, api_version="v1"
-        )
+        list, _ = self.rest.get_paginated_data(path="/serverGroup", **kwargs, api_version="v1")
         return list
 
     def get_group(self, group_id: str) -> Box:
         """
         Provides information on the specified server group.
 
         Args:
@@ -125,33 +123,29 @@
             ...      'address': '10.0.0.30',
             ...      'enabled': True}])
 
         """
         # Initialise payload
         payload = {
             "name": name,
-            "appConnectorGroups": [
-                {"id": group_id} for group_id in app_connector_group_ids
-            ],
+            "appConnectorGroups": [{"id": group_id} for group_id in app_connector_group_ids],
         }
 
         add_id_groups(self.reformat_params, kwargs, payload)
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
         response = self.rest.post("serverGroup", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_group(self, group_id: str, **kwargs) -> Box:
         """
         Updates a server group.
 
         Args:
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/servers.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/servers.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,17 +42,15 @@
 
         Returns:
             :obj:`BoxList`: List of all configured servers.
 
         Examples:
             >>> servers = zpa.servers.list_servers()
         """
-        list, _ = self.rest.get_paginated_data(
-            path="/server", **kwargs, api_version="v1"
-        )
+        list, _ = self.rest.get_paginated_data(path="/server", **kwargs, api_version="v1")
         return list
 
     def get_server(self, server_id: str) -> Box:
         """
         Gets information on the specified server.
 
         Args:
@@ -76,17 +74,15 @@
     def get_server_by_name(self, name):
         apps = self.list_servers()
         for app in apps:
             if app.get("name") == name:
                 return app
         return None
 
-    def add_server(
-        self, name: str, address: str, enabled: bool = True, **kwargs
-    ) -> Box:
+    def add_server(self, name: str, address: str, enabled: bool = True, **kwargs) -> Box:
         """
         Add a new application server.
 
         Args:
             name (str):
                 The name of the server.
             address (str):
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/service_edges.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/service_edges.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,17 +53,15 @@
             :obj:`BoxList`: List containing information on all configured ZPA Service Edges.
 
         Examples:
             >>> for service_edge in zpa.service_edges.list_service_edges():
             ...    print(service_edge)
 
         """
-        list, _ = self.rest.get_paginated_data(
-            path="/serviceEdge", **kwargs, api_version="v1"
-        )
+        list, _ = self.rest.get_paginated_data(path="/serviceEdge", **kwargs, api_version="v1")
         return list
 
     def get_service_edge(self, service_edge_id: str) -> Box:
         """
         Returns information on the specified Service Edge.
 
         Args:
@@ -110,30 +108,25 @@
             >>> updated_service_edge = zpa.service_edge.update_service_edge('99999',
             ...    description="Updated Description",
             ...    name="Updated Name")
 
         """
 
         # Set payload to equal existing record
-        payload = {
-            snake_to_camel(k): v
-            for k, v in self.get_service_edge(service_edge_id).items()
-        }
+        payload = {snake_to_camel(k): v for k, v in self.get_service_edge(service_edge_id).items()}
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
-        resp = self.rest.put(
-            "/serviceEdge/%s" % (service_edge_id), json=payload
-        ).status_code
+        resp = self.rest.put("/serviceEdge/%s" % (service_edge_id), json=payload).status_code
         if not isinstance(resp, Response):
             return self.get_service_edge(service_edge_id)
 
     def delete_service_edge(self, service_edge_id: str) -> int:
         """
         Deletes the specified Service Edge from ZPA.
 
@@ -192,17 +185,15 @@
         Examples:
             Print all Service Edge Groups in ZPA.
 
             >>> for group in zpa.service_edges.list_service_edge_groups():
             ...    print(group)
 
         """
-        list, _ = self.rest.get_paginated_data(
-            path="/serviceEdgeGroup", **kwargs, api_version="v1"
-        )
+        list, _ = self.rest.get_paginated_data(path="/serviceEdgeGroup", **kwargs, api_version="v1")
         return list
 
     def get_service_edge_group(self, group_id: str) -> Box:
         """
         Returns information on the specified ZPA Service Edge Group.
 
         Args:
@@ -225,17 +216,15 @@
     def get_service_edge_group_by_name(self, name):
         groups = self.list_service_edge_groups()
         for group in groups:
             if group.get("name") == name:
                 return group
         return None
 
-    def add_service_edge_group(
-        self, name: str, latitude: str, longitude: str, location: str, **kwargs
-    ):
+    def add_service_edge_group(self, name: str, latitude: str, longitude: str, location: str, **kwargs):
         """
         Adds a new Service Edge Group to ZPA.
 
         Args:
             latitude (str): The latitude representing the physical location of the ZPA Service Edges in this group.
             longitude (str): The longitude representing the physical location of the ZPA Service Edges in this group.
             location (str): The name of the physical location of the ZPA Service Edges in this group.
@@ -298,17 +287,15 @@
             payload[snake_to_camel(key)] = value
 
         response = self.rest.post("serviceEdgeGroup", json=payload)
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
-            raise Exception(
-                f"API call failed with status {status_code}: {response.json()}"
-            )
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
     def update_service_edge_group(self, group_id: str, **kwargs) -> Box:
         """
         Updates the specified ZPA Service Edge Group.
 
         Args:
@@ -360,18 +347,15 @@
             >>> group = zpa.service_edges.update_service_edge_group('99999',
             ...    name="Updated Name",
             ...    version_profile="default",
             ...    upgrade_day="friday")
 
         """
         # Set payload to equal existing record
-        payload = {
-            snake_to_camel(k): v
-            for k, v in self.get_service_edge_group(group_id).items()
-        }
+        payload = {snake_to_camel(k): v for k, v in self.get_service_edge_group(group_id).items()}
 
         # Perform formatting on simplified params
         add_id_groups(self.reformat_params, kwargs, payload)
         pick_version_profile(kwargs, payload)
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
```

### Comparing `zscaler-sdk-python-0.1.2/zscaler/zpa/trusted_networks.py` & `zscaler_sdk_python-0.1.3/zscaler/zpa/trusted_networks.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,17 +45,15 @@
             :obj:`BoxList`: A list of all configured trusted networks.
 
         Examples:
             >>> for trusted_network in zpa.trusted_networks.list_networks():
             ...    pprint(trusted_network)
 
         """
-        list, _ = self.rest.get_paginated_data(
-            path="/network", **kwargs, api_version="v2"
-        )
+        list, _ = self.rest.get_paginated_data(path="/network", **kwargs, api_version="v2")
         return list
 
     def get_network_by_name(self, name):
         networks = self.list_networks()
         for network in networks:
             if network.get("name") == name:
                 return network
```

