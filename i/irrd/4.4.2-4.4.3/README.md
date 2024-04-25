# Comparing `tmp/irrd-4.4.2.tar.gz` & `tmp/irrd-4.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irrd-4.4.2.tar", max compression
+gzip compressed data, was "irrd-4.4.3.tar", max compression
```

## Comparing `irrd-4.4.2.tar` & `irrd-4.4.3.tar`

### file list

```diff
@@ -1,183 +1,183 @@
--rw-r--r--   0        0        0     6371 2023-08-17 12:15:15.712265 irrd-4.4.2/LICENSE
--rw-r--r--   0        0        0     2209 2022-06-22 14:54:59.879208 irrd-4.4.2/README.rst
--rw-r--r--   0        0        0      158 2023-10-17 14:21:36.613842 irrd-4.4.2/irrd/__init__.py
--rw-r--r--   0        0        0    22139 2023-10-17 14:20:19.731937 irrd-4.4.2/irrd/conf/__init__.py
--rw-r--r--   0        0        0     3005 2023-08-17 12:15:15.719581 irrd-4.4.2/irrd/conf/default_config.yaml
--rw-r--r--   0        0        0      188 2023-08-17 07:59:03.555175 irrd-4.4.2/irrd/conf/defaults.py
--rw-r--r--   0        0        0     3262 2023-10-17 13:34:34.494305 irrd-4.4.2/irrd/conf/known_keys.py
--rw-r--r--   0        0        0    18928 2023-10-17 14:20:19.732509 irrd-4.4.2/irrd/conf/test_conf.py
--rw-r--r--   0        0        0        0 2020-11-10 14:53:47.000000 irrd-4.4.2/irrd/daemon/__init__.py
--rwxr-xr-x   0        0        0     8669 2023-10-17 13:34:34.496662 irrd-4.4.2/irrd/daemon/main.py
--rw-r--r--   0        0        0        0 2018-08-22 10:47:06.000000 irrd-4.4.2/irrd/mirroring/__init__.py
--rw-r--r--   0        0        0     1540 2023-08-17 12:15:15.721832 irrd-4.4.2/irrd/mirroring/jobs.py
--rw-r--r--   0        0        0     4092 2023-08-17 07:59:03.561180 irrd-4.4.2/irrd/mirroring/mirror_runners_export.py
--rw-r--r--   0        0        0    17866 2023-10-17 13:34:34.498579 irrd-4.4.2/irrd/mirroring/mirror_runners_import.py
--rw-r--r--   0        0        0     4295 2023-08-17 12:15:15.722667 irrd-4.4.2/irrd/mirroring/nrtm_generator.py
--rw-r--r--   0        0        0     5068 2023-10-17 13:34:34.499359 irrd-4.4.2/irrd/mirroring/nrtm_operation.py
--rw-r--r--   0        0        0    20006 2023-10-17 14:20:19.733306 irrd-4.4.2/irrd/mirroring/parsers.py
--rw-r--r--   0        0        0     7501 2023-10-17 13:34:34.501099 irrd-4.4.2/irrd/mirroring/scheduler.py
--rw-r--r--   0        0        0        0 2023-08-17 07:59:03.574640 irrd-4.4.2/irrd/routepref/__init__.py
--rw-r--r--   0        0        0     7977 2023-08-22 14:29:30.540794 irrd-4.4.2/irrd/routepref/routepref.py
--rw-r--r--   0        0        0      234 2023-08-17 07:59:03.576489 irrd-4.4.2/irrd/routepref/status.py
--rw-r--r--   0        0        0        0 2020-11-10 14:53:47.000000 irrd-4.4.2/irrd/rpki/__init__.py
--rw-r--r--   0        0        0     9554 2023-08-17 12:15:15.725102 irrd-4.4.2/irrd/rpki/importer.py
--rw-r--r--   0        0        0     5252 2023-08-17 12:15:15.725627 irrd-4.4.2/irrd/rpki/notifications.py
--rw-r--r--   0        0        0      245 2023-08-17 07:59:03.578837 irrd-4.4.2/irrd/rpki/status.py
--rw-r--r--   0        0        0     9350 2023-08-17 07:59:03.582654 irrd-4.4.2/irrd/rpki/validators.py
--rw-r--r--   0        0        0        0 2020-10-12 17:35:22.000000 irrd-4.4.2/irrd/rpsl/__init__.py
--rw-r--r--   0        0        0     2161 2023-08-17 12:15:15.727071 irrd-4.4.2/irrd/rpsl/auth.py
--rw-r--r--   0        0        0    26107 2023-08-17 12:15:15.727795 irrd-4.4.2/irrd/rpsl/fields.py
--rw-r--r--   0        0        0    22994 2023-08-17 12:15:15.728417 irrd-4.4.2/irrd/rpsl/parser.py
--rw-r--r--   0        0        0     1770 2023-08-17 07:59:03.584848 irrd-4.4.2/irrd/rpsl/parser_state.py
--rw-r--r--   0        0        0    32502 2023-10-17 14:20:19.734286 irrd-4.4.2/irrd/rpsl/rpsl_objects.py
--rw-r--r--   0        0        0        0 2020-11-10 14:53:47.000000 irrd-4.4.2/irrd/scopefilter/__init__.py
--rw-r--r--   0        0        0      275 2023-08-17 07:59:03.589099 irrd-4.4.2/irrd/scopefilter/status.py
--rw-r--r--   0        0        0     6344 2023-08-17 07:59:03.590438 irrd-4.4.2/irrd/scopefilter/validators.py
--rw-r--r--   0        0        0        0 2018-05-11 14:51:11.000000 irrd-4.4.2/irrd/scripts/__init__.py
--rwxr-xr-x   0        0        0     1281 2023-08-17 07:59:03.591027 irrd-4.4.2/irrd/scripts/database_downgrade.py
--rwxr-xr-x   0        0        0     1266 2023-08-17 07:59:03.591713 irrd-4.4.2/irrd/scripts/database_upgrade.py
--rwxr-xr-x   0        0        0     3128 2023-08-17 12:15:15.730421 irrd-4.4.2/irrd/scripts/expire_journal.py
--rwxr-xr-x   0        0        0    24850 2023-08-22 13:48:39.442086 irrd-4.4.2/irrd/scripts/irr_rpsl_submit.py
--rwxr-xr-x   0        0        0     4497 2023-08-17 12:15:15.731465 irrd-4.4.2/irrd/scripts/irrd_control.py
--rwxr-xr-x   0        0        0     2443 2023-08-17 12:15:15.731887 irrd-4.4.2/irrd/scripts/load_database.py
--rwxr-xr-x   0        0        0     1850 2023-08-17 07:59:03.594128 irrd-4.4.2/irrd/scripts/load_pgp_keys.py
--rwxr-xr-x   0        0        0     1415 2023-08-17 07:59:03.594651 irrd-4.4.2/irrd/scripts/load_test.py
--rwxr-xr-x   0        0        0     1224 2023-08-17 12:15:15.732319 irrd-4.4.2/irrd/scripts/mirror_force_reload.py
--rwxr-xr-x   0        0        0     8930 2023-08-17 07:59:03.595701 irrd-4.4.2/irrd/scripts/query_qa_comparison.py
--rwxr-xr-x   0        0        0     4512 2023-08-17 12:15:15.732811 irrd-4.4.2/irrd/scripts/rpsl_read.py
--rwxr-xr-x   0        0        0     2227 2023-08-17 12:15:15.733217 irrd-4.4.2/irrd/scripts/set_last_modified_auth.py
--rwxr-xr-x   0        0        0     1387 2023-08-17 12:15:15.733676 irrd-4.4.2/irrd/scripts/submit_changes.py
--rwxr-xr-x   0        0        0     1500 2023-08-17 07:59:03.598182 irrd-4.4.2/irrd/scripts/submit_email.py
--rw-r--r--   0        0        0     2197 2023-08-17 12:15:15.735734 irrd-4.4.2/irrd/scripts/update_database.py
--rw-r--r--   0        0        0        0 2018-07-06 10:44:00.000000 irrd-4.4.2/irrd/server/__init__.py
--rw-r--r--   0        0        0     1720 2023-08-17 07:59:03.606242 irrd-4.4.2/irrd/server/access_check.py
--rw-r--r--   0        0        0       67 2023-08-17 07:59:03.606821 irrd-4.4.2/irrd/server/graphql/__init__.py
--rw-r--r--   0        0        0     1890 2023-08-17 07:59:03.607337 irrd-4.4.2/irrd/server/graphql/extensions.py
--rw-r--r--   0        0        0    13955 2023-08-17 12:15:15.736295 irrd-4.4.2/irrd/server/graphql/resolvers.py
--rw-r--r--   0        0        0     3697 2023-08-17 12:15:15.736649 irrd-4.4.2/irrd/server/graphql/schema_builder.py
--rw-r--r--   0        0        0    13407 2023-08-17 12:15:15.737104 irrd-4.4.2/irrd/server/graphql/schema_generator.py
--rw-r--r--   0        0        0        0 2018-09-25 09:23:35.000000 irrd-4.4.2/irrd/server/http/__init__.py
--rw-r--r--   0        0        0     5551 2023-08-22 19:48:54.324523 irrd-4.4.2/irrd/server/http/app.py
--rw-r--r--   0        0        0     4798 2023-10-17 13:34:34.507288 irrd-4.4.2/irrd/server/http/endpoints_api.py
--rw-r--r--   0        0        0    12793 2023-10-17 13:34:34.508024 irrd-4.4.2/irrd/server/http/event_stream.py
--rw-r--r--   0        0        0     1600 2023-08-22 15:10:44.346331 irrd-4.4.2/irrd/server/http/server.py
--rw-r--r--   0        0        0     8311 2023-10-17 14:20:19.736444 irrd-4.4.2/irrd/server/http/status_generator.py
--rw-r--r--   0        0        0    19070 2023-10-17 14:20:19.737412 irrd-4.4.2/irrd/server/query_resolver.py
--rw-r--r--   0        0        0     2157 2023-08-17 07:59:03.620007 irrd-4.4.2/irrd/server/test_access_check.py
--rw-r--r--   0        0        0        0 2018-07-06 10:44:00.000000 irrd-4.4.2/irrd/server/whois/__init__.py
--rw-r--r--   0        0        0    27279 2023-08-17 12:15:15.743741 irrd-4.4.2/irrd/server/whois/query_parser.py
--rw-r--r--   0        0        0     3540 2023-08-17 07:59:03.622958 irrd-4.4.2/irrd/server/whois/query_response.py
--rw-r--r--   0        0        0     8772 2023-08-17 12:15:15.744141 irrd-4.4.2/irrd/server/whois/server.py
--rw-r--r--   0        0        0     1095 2023-10-17 13:34:34.512195 irrd-4.4.2/irrd/storage/__init__.py
--rw-r--r--   0        0        0        0 2018-08-22 10:47:06.000000 irrd-4.4.2/irrd/storage/alembic/__init__.py
--rw-r--r--   0        0        0     1677 2023-10-17 13:34:34.512874 irrd-4.4.2/irrd/storage/alembic/env.py
--rw-r--r--   0        0        0      494 2018-08-22 10:47:06.000000 irrd-4.4.2/irrd/storage/alembic/script.py.mako
--rw-r--r--   0        0        0     2763 2023-08-17 07:59:03.627157 irrd-4.4.2/irrd/storage/alembic/versions/0548f1aa4f10_add_rpsl_objects_suspended.py
--rw-r--r--   0        0        0      593 2023-08-17 07:59:03.627678 irrd-4.4.2/irrd/storage/alembic/versions/1743f98a456d_add_serial_newest_mirror.py
--rw-r--r--   0        0        0     1606 2023-08-17 07:59:03.628234 irrd-4.4.2/irrd/storage/alembic/versions/181670a62643_add_journal_entry_origin.py
--rw-r--r--   0        0        0      665 2023-08-17 12:15:15.745053 irrd-4.4.2/irrd/storage/alembic/versions/2353e60e63f8_add_setting.py
--rw-r--r--   0        0        0    10096 2023-08-17 07:59:03.628824 irrd-4.4.2/irrd/storage/alembic/versions/28dc1cd85bdc_initial_db.py
--rw-r--r--   0        0        0     1401 2023-08-17 07:59:03.629796 irrd-4.4.2/irrd/storage/alembic/versions/39e4f15ed80c_add_bogon_status.py
--rw-r--r--   0        0        0     2347 2023-08-17 07:59:03.630390 irrd-4.4.2/irrd/storage/alembic/versions/4a514ead8fc2_bogon_to_scope_filter.py
--rw-r--r--   0        0        0     2116 2023-08-17 12:15:15.745318 irrd-4.4.2/irrd/storage/alembic/versions/500027f85a55_add_api_tokens.py
--rw-r--r--   0        0        0     1905 2023-08-17 12:15:15.745519 irrd-4.4.2/irrd/storage/alembic/versions/50d1a0ef58cb_add_protected_name.py
--rw-r--r--   0        0        0     5499 2023-08-17 12:15:15.745736 irrd-4.4.2/irrd/storage/alembic/versions/5bbbc2989aa6_add_internal_auth.py
--rw-r--r--   0        0        0     3813 2023-08-17 12:15:15.746023 irrd-4.4.2/irrd/storage/alembic/versions/5d942647566e_add_changelog.py
--rw-r--r--   0        0        0     1227 2023-08-17 07:59:03.630910 irrd-4.4.2/irrd/storage/alembic/versions/64a3d6faf6d4_add_prefix_length_rpki_status_to_rpsl_objects.py
--rw-r--r--   0        0        0     1048 2023-08-17 07:59:03.631468 irrd-4.4.2/irrd/storage/alembic/versions/8744b4b906bb_fix_rpsl_unique_key.py
--rw-r--r--   0        0        0      597 2023-08-17 07:59:03.632165 irrd-4.4.2/irrd/storage/alembic/versions/893d0d5363b3_add_rpsl_prefix_idx.py
--rw-r--r--   0        0        0     2118 2023-08-17 12:15:15.746369 irrd-4.4.2/irrd/storage/alembic/versions/8b8357acd333_add_global_serial.py
--rw-r--r--   0        0        0        0 2018-08-22 10:47:06.000000 irrd-4.4.2/irrd/storage/alembic/versions/__init__.py
--rw-r--r--   0        0        0     1131 2023-10-17 13:34:34.513959 irrd-4.4.2/irrd/storage/alembic/versions/a7766c144d61_add_synchronised_serial_to_database_.py
--rw-r--r--   0        0        0     1589 2023-08-17 07:59:03.636546 irrd-4.4.2/irrd/storage/alembic/versions/a8609af97aa3_set_prefix_length_in_existing_rpsl_.py
--rw-r--r--   0        0        0      534 2023-08-17 07:59:03.637182 irrd-4.4.2/irrd/storage/alembic/versions/b175c262448f_set_rpsl_prefix.py
--rw-r--r--   0        0        0     1640 2023-08-17 07:59:03.637789 irrd-4.4.2/irrd/storage/alembic/versions/e07863eac52f_add_roa_object_table.py
--rw-r--r--   0        0        0      511 2023-08-17 07:59:03.638989 irrd-4.4.2/irrd/storage/alembic/versions/f4c837d8258c_add_rpsl_prefix.py
--rw-r--r--   0        0        0     1662 2023-08-17 07:59:03.639608 irrd-4.4.2/irrd/storage/alembic/versions/fd4473bc1a10_add_route_preference_status.py
--rw-r--r--   0        0        0    51446 2023-10-17 13:34:34.514989 irrd-4.4.2/irrd/storage/database_handler.py
--rw-r--r--   0        0        0     2222 2023-08-17 07:59:03.641277 irrd-4.4.2/irrd/storage/event_stream.py
--rw-r--r--   0        0        0    22972 2023-10-17 13:34:34.515651 irrd-4.4.2/irrd/storage/models.py
--rw-r--r--   0        0        0     3023 2023-08-17 12:15:15.747505 irrd-4.4.2/irrd/storage/orm_provider.py
--rw-r--r--   0        0        0    24197 2023-10-17 14:20:22.766919 irrd-4.4.2/irrd/storage/preload.py
--rw-r--r--   0        0        0    23886 2023-10-17 13:34:34.516804 irrd-4.4.2/irrd/storage/queries.py
--rw-r--r--   0        0        0        0 2018-07-31 14:50:32.000000 irrd-4.4.2/irrd/updates/__init__.py
--rw-r--r--   0        0        0     3162 2023-08-17 12:15:15.749599 irrd-4.4.2/irrd/updates/email.py
--rw-r--r--   0        0        0    15834 2023-08-17 12:15:15.749922 irrd-4.4.2/irrd/updates/handler.py
--rw-r--r--   0        0        0    31179 2023-10-17 14:20:19.741748 irrd-4.4.2/irrd/updates/parser.py
--rw-r--r--   0        0        0     1891 2023-10-17 14:20:19.742660 irrd-4.4.2/irrd/updates/parser_state.py
--rw-r--r--   0        0        0     7991 2023-08-17 07:59:03.649490 irrd-4.4.2/irrd/updates/suspension.py
--rw-r--r--   0        0        0    32193 2023-08-17 15:31:18.289062 irrd-4.4.2/irrd/updates/validators.py
--rw-r--r--   0        0        0        0 2023-01-30 15:26:42.092349 irrd-4.4.2/irrd/utils/__init__.py
--rw-r--r--   0        0        0     3312 2023-08-17 12:15:15.755189 irrd-4.4.2/irrd/utils/email.py
--rw-r--r--   0        0        0     2969 2023-08-17 12:15:15.755399 irrd-4.4.2/irrd/utils/factories.py
--rw-r--r--   0        0        0      338 2023-10-17 13:34:34.522283 irrd-4.4.2/irrd/utils/misc.py
--rw-r--r--   0        0        0     3101 2023-08-17 12:15:15.755688 irrd-4.4.2/irrd/utils/pgp.py
--rw-r--r--   0        0        0     1685 2023-08-22 12:35:02.260654 irrd-4.4.2/irrd/utils/process_support.py
--rw-r--r--   0        0        0    40910 2023-10-17 14:20:19.745040 irrd-4.4.2/irrd/utils/rpsl_samples.py
--rw-r--r--   0        0        0     4956 2023-10-17 13:34:34.524047 irrd-4.4.2/irrd/utils/test_utils.py
--rw-r--r--   0        0        0     3532 2023-08-17 12:15:15.758339 irrd-4.4.2/irrd/utils/text.py
--rw-r--r--   0        0        0     3930 2023-10-17 13:34:34.525909 irrd-4.4.2/irrd/utils/validators.py
--rw-r--r--   0        0        0     4823 2023-08-17 07:59:03.665228 irrd-4.4.2/irrd/utils/whois_client.py
--rw-r--r--   0        0        0        0 2020-11-10 14:53:47.000000 irrd-4.4.2/irrd/vendor/__init__.py
--rw-r--r--   0        0        0        0 2022-06-22 14:54:59.965929 irrd-4.4.2/irrd/vendor/dotted/__init__.py
--rw-r--r--   0        0        0    11736 2023-08-17 07:59:03.665703 irrd-4.4.2/irrd/vendor/dotted/collection.py
--rw-r--r--   0        0        0      104 2023-08-17 12:15:15.759001 irrd-4.4.2/irrd/vendor/mock_alchemy/__init__.py
--rw-r--r--   0        0        0     5649 2023-08-17 12:15:15.759281 irrd-4.4.2/irrd/vendor/mock_alchemy/comparison.py
--rw-r--r--   0        0        0    23640 2023-08-17 12:15:15.759689 irrd-4.4.2/irrd/vendor/mock_alchemy/mocking.py
--rw-r--r--   0        0        0     2609 2023-08-17 12:15:15.760020 irrd-4.4.2/irrd/vendor/mock_alchemy/unittests.py
--rw-r--r--   0        0        0     7298 2023-08-17 12:15:15.760442 irrd-4.4.2/irrd/vendor/mock_alchemy/utils.py
--rw-r--r--   0        0        0     6209 2023-08-17 07:59:03.666328 irrd-4.4.2/irrd/vendor/postgres_copy/__init__.py
--rw-r--r--   0        0        0      605 2023-08-17 12:15:15.760865 irrd-4.4.2/irrd/webui/__init__.py
--rw-r--r--   0        0        0        0 2023-08-17 12:15:15.760933 irrd-4.4.2/irrd/webui/auth/__init__.py
--rw-r--r--   0        0        0     2350 2023-08-17 12:15:15.761295 irrd-4.4.2/irrd/webui/auth/decorators.py
--rw-r--r--   0        0        0    11741 2023-08-17 12:15:15.761691 irrd-4.4.2/irrd/webui/auth/endpoints.py
--rw-r--r--   0        0        0    15896 2023-08-17 12:15:15.761994 irrd-4.4.2/irrd/webui/auth/endpoints_mfa.py
--rw-r--r--   0        0        0     2082 2023-08-17 12:15:15.762313 irrd-4.4.2/irrd/webui/auth/routes.py
--rw-r--r--   0        0        0     5621 2023-08-17 12:15:15.762899 irrd-4.4.2/irrd/webui/auth/users.py
--rw-r--r--   0        0        0     9166 2023-08-17 12:15:15.763676 irrd-4.4.2/irrd/webui/endpoints.py
--rw-r--r--   0        0        0    28060 2023-08-17 12:15:15.764224 irrd-4.4.2/irrd/webui/endpoints_mntners.py
--rw-r--r--   0        0        0     6618 2023-10-17 13:34:34.526980 irrd-4.4.2/irrd/webui/helpers.py
--rw-r--r--   0        0        0     2061 2023-10-17 13:34:34.527713 irrd-4.4.2/irrd/webui/rendering.py
--rw-r--r--   0        0        0     2191 2023-10-12 15:14:42.953673 irrd-4.4.2/irrd/webui/routes.py
--rw-r--r--   0        0        0   237950 2023-08-17 12:15:15.767969 irrd-4.4.2/irrd/webui/static/css/bootstrap.css
--rw-r--r--   0        0        0   194901 2023-08-17 12:15:15.769612 irrd-4.4.2/irrd/webui/static/css/bootstrap.min.css
--rw-r--r--   0        0        0   207989 2023-08-17 12:15:15.772066 irrd-4.4.2/irrd/webui/static/js/bootstrap.bundle.js
--rw-r--r--   0        0        0    80420 2023-08-17 12:15:15.773609 irrd-4.4.2/irrd/webui/static/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0    23490 2023-08-17 12:15:15.774168 irrd-4.4.2/irrd/webui/static/js/qrcode.js
--rw-r--r--   0        0        0     9409 2023-08-17 12:15:15.774598 irrd-4.4.2/irrd/webui/static/js/simplewebauthn-browser-es5-umd.js
--rw-r--r--   0        0        0      463 2023-08-17 12:15:15.775016 irrd-4.4.2/irrd/webui/templates/api_token_delete.html
--rw-r--r--   0        0        0      707 2023-08-17 12:15:15.775379 irrd-4.4.2/irrd/webui/templates/api_token_form.html
--rw-r--r--   0        0        0      209 2023-08-17 12:15:15.775714 irrd-4.4.2/irrd/webui/templates/authentication_change_mail.txt
--rw-r--r--   0        0        0       38 2023-08-17 12:15:15.776028 irrd-4.4.2/irrd/webui/templates/authentication_change_mail_subject.txt
--rw-r--r--   0        0        0     3948 2023-10-17 13:34:34.528351 irrd-4.4.2/irrd/webui/templates/base.html
--rw-r--r--   0        0        0     3879 2023-08-17 12:15:15.776818 irrd-4.4.2/irrd/webui/templates/change_log_entry.html
--rw-r--r--   0        0        0     2297 2023-08-17 12:15:15.777139 irrd-4.4.2/irrd/webui/templates/change_log_mntner.html
--rw-r--r--   0        0        0      722 2023-08-17 12:15:15.777536 irrd-4.4.2/irrd/webui/templates/create_account_confirm_form.html
--rw-r--r--   0        0        0      464 2023-08-17 12:15:15.777883 irrd-4.4.2/irrd/webui/templates/create_account_form.html
--rw-r--r--   0        0        0      246 2023-08-17 12:15:15.778241 irrd-4.4.2/irrd/webui/templates/create_account_mail.txt
--rw-r--r--   0        0        0       26 2023-08-17 12:15:15.778568 irrd-4.4.2/irrd/webui/templates/create_account_mail_subject.txt
--rw-r--r--   0        0        0     4121 2023-08-17 12:15:15.779037 irrd-4.4.2/irrd/webui/templates/index.html
--rw-r--r--   0        0        0     1742 2023-08-17 12:15:15.779363 irrd-4.4.2/irrd/webui/templates/login.html
--rw-r--r--   0        0        0     1933 2023-08-17 12:15:15.779657 irrd-4.4.2/irrd/webui/templates/maintained_objects.html
--rw-r--r--   0        0        0     2642 2023-08-17 12:15:15.779966 irrd-4.4.2/irrd/webui/templates/mfa_authenticate.html
--rw-r--r--   0        0        0     1892 2023-08-17 12:15:15.780272 irrd-4.4.2/irrd/webui/templates/mfa_status.html
--rw-r--r--   0        0        0      659 2023-08-17 12:15:15.780596 irrd-4.4.2/irrd/webui/templates/mntner_migrate_complete.html
--rw-r--r--   0        0        0      669 2023-08-17 12:15:15.780912 irrd-4.4.2/irrd/webui/templates/mntner_migrate_initiate.html
--rw-r--r--   0        0        0      610 2023-08-17 12:15:15.781235 irrd-4.4.2/irrd/webui/templates/mntner_migrate_initiate_mail.txt
--rw-r--r--   0        0        0      105 2023-08-17 12:15:15.781482 irrd-4.4.2/irrd/webui/templates/mntner_migrate_initiate_mail_subject.txt
--rw-r--r--   0        0        0      430 2023-08-17 12:15:15.781791 irrd-4.4.2/irrd/webui/templates/password_change_form.html
--rw-r--r--   0        0        0      551 2023-08-17 12:15:15.782113 irrd-4.4.2/irrd/webui/templates/permission_delete.html
--rw-r--r--   0        0        0      817 2023-08-17 12:15:15.782415 irrd-4.4.2/irrd/webui/templates/permission_form.html
--rw-r--r--   0        0        0      205 2023-08-17 12:15:15.782837 irrd-4.4.2/irrd/webui/templates/profile_change_form.html
--rw-r--r--   0        0        0      590 2023-08-17 12:15:15.783141 irrd-4.4.2/irrd/webui/templates/reset_password_request_form.html
--rw-r--r--   0        0        0      167 2023-08-17 12:15:15.783435 irrd-4.4.2/irrd/webui/templates/reset_password_request_mail.txt
--rw-r--r--   0        0        0       33 2023-08-17 12:15:15.783788 irrd-4.4.2/irrd/webui/templates/reset_password_request_mail_subject.txt
--rw-r--r--   0        0        0      726 2023-08-17 12:15:15.784138 irrd-4.4.2/irrd/webui/templates/rpsl_detail.html
--rw-r--r--   0        0        0     2813 2023-08-17 12:15:15.784500 irrd-4.4.2/irrd/webui/templates/rpsl_form.html
--rw-r--r--   0        0        0      789 2023-08-17 12:15:15.784890 irrd-4.4.2/irrd/webui/templates/totp_register.html
--rw-r--r--   0        0        0      494 2023-08-17 12:15:15.785158 irrd-4.4.2/irrd/webui/templates/totp_remove.html
--rw-r--r--   0        0        0     5564 2023-08-17 12:15:15.785422 irrd-4.4.2/irrd/webui/templates/user_permissions.html
--rw-r--r--   0        0        0     2409 2023-10-17 13:34:34.529355 irrd-4.4.2/irrd/webui/templates/webauthn_register.html
--rw-r--r--   0        0        0      222 2023-08-17 12:15:15.786101 irrd-4.4.2/irrd/webui/templates/webauthn_remove.html
--rw-r--r--   0        0        0     4486 2023-10-17 14:21:36.617748 irrd-4.4.2/pyproject.toml
--rw-r--r--   0        0        0     4374 1970-01-01 00:00:00.000000 irrd-4.4.2/PKG-INFO
+-rw-r--r--   0        0        0     6371 2024-01-25 13:52:23.245334 irrd-4.4.3/LICENSE
+-rw-r--r--   0        0        0     2209 2022-06-22 14:54:59.879208 irrd-4.4.3/README.rst
+-rw-r--r--   0        0        0      158 2024-01-25 13:52:23.251925 irrd-4.4.3/irrd/__init__.py
+-rw-r--r--   0        0        0    22139 2024-01-25 13:52:23.252257 irrd-4.4.3/irrd/conf/__init__.py
+-rw-r--r--   0        0        0     3005 2024-01-25 13:52:23.252534 irrd-4.4.3/irrd/conf/default_config.yaml
+-rw-r--r--   0        0        0      188 2024-01-25 13:44:45.127497 irrd-4.4.3/irrd/conf/defaults.py
+-rw-r--r--   0        0        0     3262 2024-01-25 13:52:23.252789 irrd-4.4.3/irrd/conf/known_keys.py
+-rw-r--r--   0        0        0    18928 2024-01-25 13:52:23.253082 irrd-4.4.3/irrd/conf/test_conf.py
+-rw-r--r--   0        0        0        0 2020-11-10 14:53:47.000000 irrd-4.4.3/irrd/daemon/__init__.py
+-rwxr-xr-x   0        0        0     8669 2024-01-25 13:52:23.253408 irrd-4.4.3/irrd/daemon/main.py
+-rw-r--r--   0        0        0        0 2018-08-22 10:47:06.000000 irrd-4.4.3/irrd/mirroring/__init__.py
+-rw-r--r--   0        0        0     1540 2024-01-25 13:52:23.254109 irrd-4.4.3/irrd/mirroring/jobs.py
+-rw-r--r--   0        0        0     4092 2023-08-17 07:59:03.561180 irrd-4.4.3/irrd/mirroring/mirror_runners_export.py
+-rw-r--r--   0        0        0    17866 2024-01-25 13:52:23.254463 irrd-4.4.3/irrd/mirroring/mirror_runners_import.py
+-rw-r--r--   0        0        0     4295 2024-01-25 13:52:23.254873 irrd-4.4.3/irrd/mirroring/nrtm_generator.py
+-rw-r--r--   0        0        0     5068 2024-01-25 13:44:45.130691 irrd-4.4.3/irrd/mirroring/nrtm_operation.py
+-rw-r--r--   0        0        0    20006 2024-01-25 13:44:45.131208 irrd-4.4.3/irrd/mirroring/parsers.py
+-rw-r--r--   0        0        0     7501 2024-01-25 13:52:23.255209 irrd-4.4.3/irrd/mirroring/scheduler.py
+-rw-r--r--   0        0        0        0 2023-08-17 07:59:03.574640 irrd-4.4.3/irrd/routepref/__init__.py
+-rw-r--r--   0        0        0     7977 2024-01-25 13:52:23.256471 irrd-4.4.3/irrd/routepref/routepref.py
+-rw-r--r--   0        0        0      234 2023-08-17 07:59:03.576489 irrd-4.4.3/irrd/routepref/status.py
+-rw-r--r--   0        0        0        0 2020-11-10 14:53:47.000000 irrd-4.4.3/irrd/rpki/__init__.py
+-rw-r--r--   0        0        0     9554 2024-01-25 13:52:23.257190 irrd-4.4.3/irrd/rpki/importer.py
+-rw-r--r--   0        0        0     5252 2024-01-25 13:52:23.257493 irrd-4.4.3/irrd/rpki/notifications.py
+-rw-r--r--   0        0        0      245 2023-08-17 07:59:03.578837 irrd-4.4.3/irrd/rpki/status.py
+-rw-r--r--   0        0        0     9350 2023-08-17 07:59:03.582654 irrd-4.4.3/irrd/rpki/validators.py
+-rw-r--r--   0        0        0        0 2020-10-12 17:35:22.000000 irrd-4.4.3/irrd/rpsl/__init__.py
+-rw-r--r--   0        0        0     2161 2024-01-25 13:52:23.258415 irrd-4.4.3/irrd/rpsl/auth.py
+-rw-r--r--   0        0        0    26107 2024-01-25 13:52:23.258728 irrd-4.4.3/irrd/rpsl/fields.py
+-rw-r--r--   0        0        0    22994 2024-01-25 13:52:23.259075 irrd-4.4.3/irrd/rpsl/parser.py
+-rw-r--r--   0        0        0     1770 2023-08-17 07:59:03.584848 irrd-4.4.3/irrd/rpsl/parser_state.py
+-rw-r--r--   0        0        0    32510 2024-01-25 13:52:23.259401 irrd-4.4.3/irrd/rpsl/rpsl_objects.py
+-rw-r--r--   0        0        0        0 2020-11-10 14:53:47.000000 irrd-4.4.3/irrd/scopefilter/__init__.py
+-rw-r--r--   0        0        0      275 2023-08-17 07:59:03.589099 irrd-4.4.3/irrd/scopefilter/status.py
+-rw-r--r--   0        0        0     6344 2023-08-17 07:59:03.590438 irrd-4.4.3/irrd/scopefilter/validators.py
+-rw-r--r--   0        0        0        0 2018-05-11 14:51:11.000000 irrd-4.4.3/irrd/scripts/__init__.py
+-rwxr-xr-x   0        0        0     1281 2023-08-17 07:59:03.591027 irrd-4.4.3/irrd/scripts/database_downgrade.py
+-rwxr-xr-x   0        0        0     1266 2023-08-17 07:59:03.591713 irrd-4.4.3/irrd/scripts/database_upgrade.py
+-rwxr-xr-x   0        0        0     3128 2024-01-25 13:52:23.260006 irrd-4.4.3/irrd/scripts/expire_journal.py
+-rwxr-xr-x   0        0        0    24850 2024-01-25 13:52:23.260341 irrd-4.4.3/irrd/scripts/irr_rpsl_submit.py
+-rwxr-xr-x   0        0        0     4497 2024-01-25 13:52:23.260611 irrd-4.4.3/irrd/scripts/irrd_control.py
+-rwxr-xr-x   0        0        0     2443 2024-01-25 13:52:23.260907 irrd-4.4.3/irrd/scripts/load_database.py
+-rwxr-xr-x   0        0        0     1850 2023-08-17 07:59:03.594128 irrd-4.4.3/irrd/scripts/load_pgp_keys.py
+-rwxr-xr-x   0        0        0     1415 2023-08-17 07:59:03.594651 irrd-4.4.3/irrd/scripts/load_test.py
+-rwxr-xr-x   0        0        0     1224 2024-01-25 13:52:23.261177 irrd-4.4.3/irrd/scripts/mirror_force_reload.py
+-rwxr-xr-x   0        0        0     8930 2023-08-17 07:59:03.595701 irrd-4.4.3/irrd/scripts/query_qa_comparison.py
+-rwxr-xr-x   0        0        0     4512 2024-01-25 13:52:23.261469 irrd-4.4.3/irrd/scripts/rpsl_read.py
+-rwxr-xr-x   0        0        0     2227 2024-01-25 13:52:23.261749 irrd-4.4.3/irrd/scripts/set_last_modified_auth.py
+-rwxr-xr-x   0        0        0     1387 2024-01-25 13:52:23.262013 irrd-4.4.3/irrd/scripts/submit_changes.py
+-rwxr-xr-x   0        0        0     1500 2023-08-17 07:59:03.598182 irrd-4.4.3/irrd/scripts/submit_email.py
+-rw-r--r--   0        0        0     2197 2024-01-25 13:52:23.263108 irrd-4.4.3/irrd/scripts/update_database.py
+-rw-r--r--   0        0        0        0 2018-07-06 10:44:00.000000 irrd-4.4.3/irrd/server/__init__.py
+-rw-r--r--   0        0        0     1720 2023-08-17 07:59:03.606241 irrd-4.4.3/irrd/server/access_check.py
+-rw-r--r--   0        0        0       67 2023-08-17 07:59:03.606821 irrd-4.4.3/irrd/server/graphql/__init__.py
+-rw-r--r--   0        0        0     1890 2023-08-17 07:59:03.607337 irrd-4.4.3/irrd/server/graphql/extensions.py
+-rw-r--r--   0        0        0    13955 2024-01-25 13:52:23.263483 irrd-4.4.3/irrd/server/graphql/resolvers.py
+-rw-r--r--   0        0        0     3697 2024-01-25 13:52:23.263730 irrd-4.4.3/irrd/server/graphql/schema_builder.py
+-rw-r--r--   0        0        0    13407 2024-01-25 13:52:23.264040 irrd-4.4.3/irrd/server/graphql/schema_generator.py
+-rw-r--r--   0        0        0        0 2018-09-25 09:23:35.000000 irrd-4.4.3/irrd/server/http/__init__.py
+-rw-r--r--   0        0        0     5551 2024-01-25 13:52:23.264999 irrd-4.4.3/irrd/server/http/app.py
+-rw-r--r--   0        0        0     4798 2024-01-25 13:52:23.265230 irrd-4.4.3/irrd/server/http/endpoints_api.py
+-rw-r--r--   0        0        0    12793 2024-01-25 13:52:23.265545 irrd-4.4.3/irrd/server/http/event_stream.py
+-rw-r--r--   0        0        0     1600 2024-01-25 13:52:23.265804 irrd-4.4.3/irrd/server/http/server.py
+-rw-r--r--   0        0        0     8311 2024-01-25 13:52:23.266099 irrd-4.4.3/irrd/server/http/status_generator.py
+-rw-r--r--   0        0        0    19070 2024-01-25 13:52:23.266941 irrd-4.4.3/irrd/server/query_resolver.py
+-rw-r--r--   0        0        0     2157 2023-08-17 07:59:03.620007 irrd-4.4.3/irrd/server/test_access_check.py
+-rw-r--r--   0        0        0        0 2018-07-06 10:44:00.000000 irrd-4.4.3/irrd/server/whois/__init__.py
+-rw-r--r--   0        0        0    27279 2024-01-25 13:52:23.267648 irrd-4.4.3/irrd/server/whois/query_parser.py
+-rw-r--r--   0        0        0     3540 2023-08-17 07:59:03.622958 irrd-4.4.3/irrd/server/whois/query_response.py
+-rw-r--r--   0        0        0     8772 2024-01-25 13:52:23.267958 irrd-4.4.3/irrd/server/whois/server.py
+-rw-r--r--   0        0        0     1095 2024-01-25 13:52:23.268514 irrd-4.4.3/irrd/storage/__init__.py
+-rw-r--r--   0        0        0        0 2018-08-22 10:47:06.000000 irrd-4.4.3/irrd/storage/alembic/__init__.py
+-rw-r--r--   0        0        0     1677 2024-01-25 13:52:23.268753 irrd-4.4.3/irrd/storage/alembic/env.py
+-rw-r--r--   0        0        0      494 2018-08-22 10:47:06.000000 irrd-4.4.3/irrd/storage/alembic/script.py.mako
+-rw-r--r--   0        0        0     2763 2023-08-17 07:59:03.627157 irrd-4.4.3/irrd/storage/alembic/versions/0548f1aa4f10_add_rpsl_objects_suspended.py
+-rw-r--r--   0        0        0      593 2023-08-17 07:59:03.627678 irrd-4.4.3/irrd/storage/alembic/versions/1743f98a456d_add_serial_newest_mirror.py
+-rw-r--r--   0        0        0     1606 2023-08-17 07:59:03.628234 irrd-4.4.3/irrd/storage/alembic/versions/181670a62643_add_journal_entry_origin.py
+-rw-r--r--   0        0        0      665 2024-01-25 13:52:23.268962 irrd-4.4.3/irrd/storage/alembic/versions/2353e60e63f8_add_setting.py
+-rw-r--r--   0        0        0    10096 2023-08-17 07:59:03.628824 irrd-4.4.3/irrd/storage/alembic/versions/28dc1cd85bdc_initial_db.py
+-rw-r--r--   0        0        0     1401 2023-08-17 07:59:03.629796 irrd-4.4.3/irrd/storage/alembic/versions/39e4f15ed80c_add_bogon_status.py
+-rw-r--r--   0        0        0     2347 2023-08-17 07:59:03.630390 irrd-4.4.3/irrd/storage/alembic/versions/4a514ead8fc2_bogon_to_scope_filter.py
+-rw-r--r--   0        0        0     2116 2024-01-25 13:52:23.269151 irrd-4.4.3/irrd/storage/alembic/versions/500027f85a55_add_api_tokens.py
+-rw-r--r--   0        0        0     1905 2024-01-25 13:52:23.269276 irrd-4.4.3/irrd/storage/alembic/versions/50d1a0ef58cb_add_protected_name.py
+-rw-r--r--   0        0        0     5499 2024-01-25 13:52:23.269513 irrd-4.4.3/irrd/storage/alembic/versions/5bbbc2989aa6_add_internal_auth.py
+-rw-r--r--   0        0        0     3813 2024-01-25 13:52:23.269728 irrd-4.4.3/irrd/storage/alembic/versions/5d942647566e_add_changelog.py
+-rw-r--r--   0        0        0     1227 2023-08-17 07:59:03.630910 irrd-4.4.3/irrd/storage/alembic/versions/64a3d6faf6d4_add_prefix_length_rpki_status_to_rpsl_objects.py
+-rw-r--r--   0        0        0     1048 2023-08-17 07:59:03.631468 irrd-4.4.3/irrd/storage/alembic/versions/8744b4b906bb_fix_rpsl_unique_key.py
+-rw-r--r--   0        0        0      597 2023-08-17 07:59:03.632165 irrd-4.4.3/irrd/storage/alembic/versions/893d0d5363b3_add_rpsl_prefix_idx.py
+-rw-r--r--   0        0        0     2118 2024-01-25 13:52:23.269974 irrd-4.4.3/irrd/storage/alembic/versions/8b8357acd333_add_global_serial.py
+-rw-r--r--   0        0        0        0 2018-08-22 10:47:06.000000 irrd-4.4.3/irrd/storage/alembic/versions/__init__.py
+-rw-r--r--   0        0        0     1131 2024-01-25 13:44:45.151239 irrd-4.4.3/irrd/storage/alembic/versions/a7766c144d61_add_synchronised_serial_to_database_.py
+-rw-r--r--   0        0        0     1589 2023-08-17 07:59:03.636546 irrd-4.4.3/irrd/storage/alembic/versions/a8609af97aa3_set_prefix_length_in_existing_rpsl_.py
+-rw-r--r--   0        0        0      534 2023-08-17 07:59:03.637182 irrd-4.4.3/irrd/storage/alembic/versions/b175c262448f_set_rpsl_prefix.py
+-rw-r--r--   0        0        0     1640 2023-08-17 07:59:03.637789 irrd-4.4.3/irrd/storage/alembic/versions/e07863eac52f_add_roa_object_table.py
+-rw-r--r--   0        0        0      511 2023-08-17 07:59:03.638989 irrd-4.4.3/irrd/storage/alembic/versions/f4c837d8258c_add_rpsl_prefix.py
+-rw-r--r--   0        0        0     1662 2023-08-17 07:59:03.639608 irrd-4.4.3/irrd/storage/alembic/versions/fd4473bc1a10_add_route_preference_status.py
+-rw-r--r--   0        0        0    51446 2024-01-25 13:52:23.270315 irrd-4.4.3/irrd/storage/database_handler.py
+-rw-r--r--   0        0        0     2222 2023-08-17 07:59:03.641277 irrd-4.4.3/irrd/storage/event_stream.py
+-rw-r--r--   0        0        0    22972 2024-01-25 13:52:23.270628 irrd-4.4.3/irrd/storage/models.py
+-rw-r--r--   0        0        0     3023 2024-01-25 13:52:23.270876 irrd-4.4.3/irrd/storage/orm_provider.py
+-rw-r--r--   0        0        0    24197 2024-01-25 13:52:23.271079 irrd-4.4.3/irrd/storage/preload.py
+-rw-r--r--   0        0        0    23886 2024-01-25 13:52:23.271368 irrd-4.4.3/irrd/storage/queries.py
+-rw-r--r--   0        0        0        0 2018-07-31 14:50:32.000000 irrd-4.4.3/irrd/updates/__init__.py
+-rw-r--r--   0        0        0     3162 2024-01-25 13:52:23.272304 irrd-4.4.3/irrd/updates/email.py
+-rw-r--r--   0        0        0    15834 2024-01-25 13:52:23.272643 irrd-4.4.3/irrd/updates/handler.py
+-rw-r--r--   0        0        0    31179 2024-01-25 13:52:23.272927 irrd-4.4.3/irrd/updates/parser.py
+-rw-r--r--   0        0        0     1891 2024-01-25 13:52:23.273167 irrd-4.4.3/irrd/updates/parser_state.py
+-rw-r--r--   0        0        0     7991 2023-08-17 07:59:03.649490 irrd-4.4.3/irrd/updates/suspension.py
+-rw-r--r--   0        0        0    32218 2024-01-25 13:52:23.274798 irrd-4.4.3/irrd/updates/validators.py
+-rw-r--r--   0        0        0        0 2023-01-30 15:26:42.092349 irrd-4.4.3/irrd/utils/__init__.py
+-rw-r--r--   0        0        0     3312 2024-01-25 13:52:23.275075 irrd-4.4.3/irrd/utils/email.py
+-rw-r--r--   0        0        0     2969 2024-01-25 13:52:23.275256 irrd-4.4.3/irrd/utils/factories.py
+-rw-r--r--   0        0        0      338 2024-01-25 13:44:45.162185 irrd-4.4.3/irrd/utils/misc.py
+-rw-r--r--   0        0        0     3101 2024-01-25 13:52:23.275510 irrd-4.4.3/irrd/utils/pgp.py
+-rw-r--r--   0        0        0     1685 2024-01-25 13:52:23.275684 irrd-4.4.3/irrd/utils/process_support.py
+-rw-r--r--   0        0        0    40910 2024-01-25 13:52:23.276138 irrd-4.4.3/irrd/utils/rpsl_samples.py
+-rw-r--r--   0        0        0     4956 2024-01-25 13:44:45.164011 irrd-4.4.3/irrd/utils/test_utils.py
+-rw-r--r--   0        0        0     3532 2024-01-25 13:52:23.277337 irrd-4.4.3/irrd/utils/text.py
+-rw-r--r--   0        0        0     3930 2024-01-25 13:52:23.277574 irrd-4.4.3/irrd/utils/validators.py
+-rw-r--r--   0        0        0     4823 2023-08-17 07:59:03.665228 irrd-4.4.3/irrd/utils/whois_client.py
+-rw-r--r--   0        0        0        0 2020-11-10 14:53:47.000000 irrd-4.4.3/irrd/vendor/__init__.py
+-rw-r--r--   0        0        0        0 2022-06-22 14:54:59.965929 irrd-4.4.3/irrd/vendor/dotted/__init__.py
+-rw-r--r--   0        0        0    11736 2023-08-17 07:59:03.665703 irrd-4.4.3/irrd/vendor/dotted/collection.py
+-rw-r--r--   0        0        0      104 2024-01-25 13:52:23.277766 irrd-4.4.3/irrd/vendor/mock_alchemy/__init__.py
+-rw-r--r--   0        0        0     5649 2024-01-25 13:52:23.277986 irrd-4.4.3/irrd/vendor/mock_alchemy/comparison.py
+-rw-r--r--   0        0        0    23640 2024-01-25 13:52:23.278194 irrd-4.4.3/irrd/vendor/mock_alchemy/mocking.py
+-rw-r--r--   0        0        0     2609 2024-01-25 13:52:23.278402 irrd-4.4.3/irrd/vendor/mock_alchemy/unittests.py
+-rw-r--r--   0        0        0     7298 2024-01-25 13:52:23.278585 irrd-4.4.3/irrd/vendor/mock_alchemy/utils.py
+-rw-r--r--   0        0        0     6209 2023-08-17 07:59:03.666328 irrd-4.4.3/irrd/vendor/postgres_copy/__init__.py
+-rw-r--r--   0        0        0      605 2024-01-25 13:52:23.278779 irrd-4.4.3/irrd/webui/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-25 13:52:23.278808 irrd-4.4.3/irrd/webui/auth/__init__.py
+-rw-r--r--   0        0        0     2350 2024-01-25 13:52:23.279450 irrd-4.4.3/irrd/webui/auth/decorators.py
+-rw-r--r--   0        0        0    11741 2024-01-25 13:52:23.279694 irrd-4.4.3/irrd/webui/auth/endpoints.py
+-rw-r--r--   0        0        0    15896 2024-01-25 13:52:23.279958 irrd-4.4.3/irrd/webui/auth/endpoints_mfa.py
+-rw-r--r--   0        0        0     2082 2024-01-25 13:52:23.280147 irrd-4.4.3/irrd/webui/auth/routes.py
+-rw-r--r--   0        0        0     5621 2024-01-25 13:52:23.280366 irrd-4.4.3/irrd/webui/auth/users.py
+-rw-r--r--   0        0        0     9166 2024-01-25 13:52:23.280570 irrd-4.4.3/irrd/webui/endpoints.py
+-rw-r--r--   0        0        0    28060 2024-01-25 13:52:23.280779 irrd-4.4.3/irrd/webui/endpoints_mntners.py
+-rw-r--r--   0        0        0     6618 2024-01-25 13:52:23.280999 irrd-4.4.3/irrd/webui/helpers.py
+-rw-r--r--   0        0        0     2061 2024-01-25 13:52:23.281185 irrd-4.4.3/irrd/webui/rendering.py
+-rw-r--r--   0        0        0     2191 2024-01-25 13:52:23.281368 irrd-4.4.3/irrd/webui/routes.py
+-rw-r--r--   0        0        0   237950 2024-01-25 13:52:23.282167 irrd-4.4.3/irrd/webui/static/css/bootstrap.css
+-rw-r--r--   0        0        0   194901 2024-01-25 13:52:23.282774 irrd-4.4.3/irrd/webui/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0   207989 2024-01-25 13:52:23.283452 irrd-4.4.3/irrd/webui/static/js/bootstrap.bundle.js
+-rw-r--r--   0        0        0    80420 2024-01-25 13:52:23.283766 irrd-4.4.3/irrd/webui/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0    23490 2024-01-25 13:52:23.284085 irrd-4.4.3/irrd/webui/static/js/qrcode.js
+-rw-r--r--   0        0        0     9409 2024-01-25 13:52:23.284398 irrd-4.4.3/irrd/webui/static/js/simplewebauthn-browser-es5-umd.js
+-rw-r--r--   0        0        0      463 2024-01-25 13:52:23.284674 irrd-4.4.3/irrd/webui/templates/api_token_delete.html
+-rw-r--r--   0        0        0      707 2024-01-25 13:52:23.284932 irrd-4.4.3/irrd/webui/templates/api_token_form.html
+-rw-r--r--   0        0        0      209 2024-01-25 13:52:23.285160 irrd-4.4.3/irrd/webui/templates/authentication_change_mail.txt
+-rw-r--r--   0        0        0       38 2024-01-25 13:52:23.285388 irrd-4.4.3/irrd/webui/templates/authentication_change_mail_subject.txt
+-rw-r--r--   0        0        0     3948 2024-01-25 13:52:23.285611 irrd-4.4.3/irrd/webui/templates/base.html
+-rw-r--r--   0        0        0     3879 2024-01-25 13:52:23.285812 irrd-4.4.3/irrd/webui/templates/change_log_entry.html
+-rw-r--r--   0        0        0     2297 2024-01-25 13:52:23.286106 irrd-4.4.3/irrd/webui/templates/change_log_mntner.html
+-rw-r--r--   0        0        0      722 2024-01-25 13:52:23.286327 irrd-4.4.3/irrd/webui/templates/create_account_confirm_form.html
+-rw-r--r--   0        0        0      464 2024-01-25 13:52:23.286531 irrd-4.4.3/irrd/webui/templates/create_account_form.html
+-rw-r--r--   0        0        0      246 2024-01-25 13:52:23.286747 irrd-4.4.3/irrd/webui/templates/create_account_mail.txt
+-rw-r--r--   0        0        0       26 2024-01-25 13:52:23.286980 irrd-4.4.3/irrd/webui/templates/create_account_mail_subject.txt
+-rw-r--r--   0        0        0     4121 2024-01-25 13:52:23.287219 irrd-4.4.3/irrd/webui/templates/index.html
+-rw-r--r--   0        0        0     1742 2024-01-25 13:52:23.287434 irrd-4.4.3/irrd/webui/templates/login.html
+-rw-r--r--   0        0        0     1933 2024-01-25 13:52:23.287666 irrd-4.4.3/irrd/webui/templates/maintained_objects.html
+-rw-r--r--   0        0        0     2642 2024-01-25 13:52:23.287879 irrd-4.4.3/irrd/webui/templates/mfa_authenticate.html
+-rw-r--r--   0        0        0     1892 2024-01-25 13:52:23.288087 irrd-4.4.3/irrd/webui/templates/mfa_status.html
+-rw-r--r--   0        0        0      659 2024-01-25 13:52:23.288316 irrd-4.4.3/irrd/webui/templates/mntner_migrate_complete.html
+-rw-r--r--   0        0        0      669 2024-01-25 13:52:23.288516 irrd-4.4.3/irrd/webui/templates/mntner_migrate_initiate.html
+-rw-r--r--   0        0        0      610 2024-01-25 13:52:23.288761 irrd-4.4.3/irrd/webui/templates/mntner_migrate_initiate_mail.txt
+-rw-r--r--   0        0        0      105 2024-01-25 13:52:23.289064 irrd-4.4.3/irrd/webui/templates/mntner_migrate_initiate_mail_subject.txt
+-rw-r--r--   0        0        0      430 2024-01-25 13:52:23.289280 irrd-4.4.3/irrd/webui/templates/password_change_form.html
+-rw-r--r--   0        0        0      551 2024-01-25 13:52:23.289491 irrd-4.4.3/irrd/webui/templates/permission_delete.html
+-rw-r--r--   0        0        0      817 2024-01-25 13:52:23.289692 irrd-4.4.3/irrd/webui/templates/permission_form.html
+-rw-r--r--   0        0        0      205 2024-01-25 13:52:23.289901 irrd-4.4.3/irrd/webui/templates/profile_change_form.html
+-rw-r--r--   0        0        0      590 2024-01-25 13:52:23.290103 irrd-4.4.3/irrd/webui/templates/reset_password_request_form.html
+-rw-r--r--   0        0        0      167 2024-01-25 13:52:23.290290 irrd-4.4.3/irrd/webui/templates/reset_password_request_mail.txt
+-rw-r--r--   0        0        0       33 2024-01-25 13:52:23.290494 irrd-4.4.3/irrd/webui/templates/reset_password_request_mail_subject.txt
+-rw-r--r--   0        0        0      726 2024-01-25 13:52:23.290694 irrd-4.4.3/irrd/webui/templates/rpsl_detail.html
+-rw-r--r--   0        0        0     2813 2024-01-25 13:52:23.290869 irrd-4.4.3/irrd/webui/templates/rpsl_form.html
+-rw-r--r--   0        0        0      789 2024-01-25 13:52:23.291053 irrd-4.4.3/irrd/webui/templates/totp_register.html
+-rw-r--r--   0        0        0      494 2024-01-25 13:52:23.291211 irrd-4.4.3/irrd/webui/templates/totp_remove.html
+-rw-r--r--   0        0        0     5564 2024-01-25 13:52:23.291428 irrd-4.4.3/irrd/webui/templates/user_permissions.html
+-rw-r--r--   0        0        0     2409 2024-01-25 13:52:23.291604 irrd-4.4.3/irrd/webui/templates/webauthn_register.html
+-rw-r--r--   0        0        0      222 2024-01-25 13:52:23.291766 irrd-4.4.3/irrd/webui/templates/webauthn_remove.html
+-rw-r--r--   0        0        0     4517 2024-01-25 13:52:23.294116 irrd-4.4.3/pyproject.toml
+-rw-r--r--   0        0        0     4425 1970-01-01 00:00:00.000000 irrd-4.4.3/PKG-INFO
```

### Comparing `irrd-4.4.2/LICENSE` & `irrd-4.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/README.rst` & `irrd-4.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/conf/__init__.py` & `irrd-4.4.3/irrd/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/conf/default_config.yaml` & `irrd-4.4.3/irrd/conf/default_config.yaml`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/conf/known_keys.py` & `irrd-4.4.3/irrd/conf/known_keys.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/conf/test_conf.py` & `irrd-4.4.3/irrd/conf/test_conf.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/daemon/main.py` & `irrd-4.4.3/irrd/daemon/main.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/mirroring/jobs.py` & `irrd-4.4.3/irrd/mirroring/jobs.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/mirroring/mirror_runners_export.py` & `irrd-4.4.3/irrd/mirroring/mirror_runners_export.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/mirroring/mirror_runners_import.py` & `irrd-4.4.3/irrd/mirroring/mirror_runners_import.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/mirroring/nrtm_generator.py` & `irrd-4.4.3/irrd/mirroring/nrtm_generator.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/mirroring/nrtm_operation.py` & `irrd-4.4.3/irrd/mirroring/nrtm_operation.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/mirroring/parsers.py` & `irrd-4.4.3/irrd/mirroring/parsers.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/mirroring/scheduler.py` & `irrd-4.4.3/irrd/mirroring/scheduler.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/routepref/routepref.py` & `irrd-4.4.3/irrd/routepref/routepref.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/rpki/importer.py` & `irrd-4.4.3/irrd/rpki/importer.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/rpki/notifications.py` & `irrd-4.4.3/irrd/rpki/notifications.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/rpki/validators.py` & `irrd-4.4.3/irrd/rpki/validators.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/rpsl/auth.py` & `irrd-4.4.3/irrd/rpsl/auth.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/rpsl/fields.py` & `irrd-4.4.3/irrd/rpsl/fields.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/rpsl/parser.py` & `irrd-4.4.3/irrd/rpsl/parser.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/rpsl/parser_state.py` & `irrd-4.4.3/irrd/rpsl/parser_state.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/rpsl/rpsl_objects.py` & `irrd-4.4.3/irrd/rpsl/rpsl_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -434,15 +434,15 @@
         dummy_matches = [auth[1] == PASSWORD_HASH_DUMMY_VALUE for auth in self._auth_lines(True)]
         if any(dummy_matches) and not all(dummy_matches):
             self.messages.error(
                 "Either all password auth hashes in a submitted mntner must be dummy objects, or none."
             )
 
     def verify_auth(self, passwords: List[str], keycert_obj_pk: Optional[str] = None) -> Optional[str]:
-        return verify_auth_lines(self.parsed_data["auth"], passwords, keycert_obj_pk)
+        return verify_auth_lines(self.parsed_data.get("auth", []), passwords, keycert_obj_pk)
 
     def has_dummy_auth_value(self) -> bool:
         """
         Check whether this object has dummy auth hashes.
         If clean() has returned successfully before, the answer from this method
         means that either all or no hashes have dummy values.
         """
```

### Comparing `irrd-4.4.2/irrd/scopefilter/validators.py` & `irrd-4.4.3/irrd/scopefilter/validators.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/scripts/database_downgrade.py` & `irrd-4.4.3/irrd/scripts/database_downgrade.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/scripts/database_upgrade.py` & `irrd-4.4.3/irrd/scripts/database_upgrade.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/scripts/expire_journal.py` & `irrd-4.4.3/irrd/scripts/expire_journal.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/scripts/irr_rpsl_submit.py` & `irrd-4.4.3/irrd/scripts/irr_rpsl_submit.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/scripts/irrd_control.py` & `irrd-4.4.3/irrd/scripts/irrd_control.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/scripts/load_database.py` & `irrd-4.4.3/irrd/scripts/load_database.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/scripts/load_pgp_keys.py` & `irrd-4.4.3/irrd/scripts/load_pgp_keys.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/scripts/load_test.py` & `irrd-4.4.3/irrd/scripts/load_test.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/scripts/mirror_force_reload.py` & `irrd-4.4.3/irrd/scripts/mirror_force_reload.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/scripts/query_qa_comparison.py` & `irrd-4.4.3/irrd/scripts/query_qa_comparison.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/scripts/rpsl_read.py` & `irrd-4.4.3/irrd/scripts/rpsl_read.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/scripts/set_last_modified_auth.py` & `irrd-4.4.3/irrd/scripts/set_last_modified_auth.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/scripts/submit_changes.py` & `irrd-4.4.3/irrd/scripts/submit_changes.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/scripts/submit_email.py` & `irrd-4.4.3/irrd/scripts/submit_email.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/scripts/update_database.py` & `irrd-4.4.3/irrd/scripts/update_database.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/server/access_check.py` & `irrd-4.4.3/irrd/server/access_check.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/server/graphql/extensions.py` & `irrd-4.4.3/irrd/server/graphql/extensions.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/server/graphql/resolvers.py` & `irrd-4.4.3/irrd/server/graphql/resolvers.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/server/graphql/schema_builder.py` & `irrd-4.4.3/irrd/server/graphql/schema_builder.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/server/graphql/schema_generator.py` & `irrd-4.4.3/irrd/server/graphql/schema_generator.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/server/http/app.py` & `irrd-4.4.3/irrd/server/http/app.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/server/http/endpoints_api.py` & `irrd-4.4.3/irrd/server/http/endpoints_api.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/server/http/event_stream.py` & `irrd-4.4.3/irrd/server/http/event_stream.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/server/http/server.py` & `irrd-4.4.3/irrd/server/http/server.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/server/http/status_generator.py` & `irrd-4.4.3/irrd/server/http/status_generator.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/server/query_resolver.py` & `irrd-4.4.3/irrd/server/query_resolver.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/server/test_access_check.py` & `irrd-4.4.3/irrd/server/test_access_check.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/server/whois/query_parser.py` & `irrd-4.4.3/irrd/server/whois/query_parser.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/server/whois/query_response.py` & `irrd-4.4.3/irrd/server/whois/query_response.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/server/whois/server.py` & `irrd-4.4.3/irrd/server/whois/server.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/__init__.py` & `irrd-4.4.3/irrd/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/alembic/env.py` & `irrd-4.4.3/irrd/storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/alembic/versions/0548f1aa4f10_add_rpsl_objects_suspended.py` & `irrd-4.4.3/irrd/storage/alembic/versions/0548f1aa4f10_add_rpsl_objects_suspended.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/alembic/versions/1743f98a456d_add_serial_newest_mirror.py` & `irrd-4.4.3/irrd/storage/alembic/versions/1743f98a456d_add_serial_newest_mirror.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/alembic/versions/181670a62643_add_journal_entry_origin.py` & `irrd-4.4.3/irrd/storage/alembic/versions/181670a62643_add_journal_entry_origin.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/alembic/versions/2353e60e63f8_add_setting.py` & `irrd-4.4.3/irrd/storage/alembic/versions/2353e60e63f8_add_setting.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/alembic/versions/28dc1cd85bdc_initial_db.py` & `irrd-4.4.3/irrd/storage/alembic/versions/28dc1cd85bdc_initial_db.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/alembic/versions/39e4f15ed80c_add_bogon_status.py` & `irrd-4.4.3/irrd/storage/alembic/versions/39e4f15ed80c_add_bogon_status.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/alembic/versions/4a514ead8fc2_bogon_to_scope_filter.py` & `irrd-4.4.3/irrd/storage/alembic/versions/4a514ead8fc2_bogon_to_scope_filter.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/alembic/versions/500027f85a55_add_api_tokens.py` & `irrd-4.4.3/irrd/storage/alembic/versions/500027f85a55_add_api_tokens.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/alembic/versions/50d1a0ef58cb_add_protected_name.py` & `irrd-4.4.3/irrd/storage/alembic/versions/50d1a0ef58cb_add_protected_name.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/alembic/versions/5bbbc2989aa6_add_internal_auth.py` & `irrd-4.4.3/irrd/storage/alembic/versions/5bbbc2989aa6_add_internal_auth.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/alembic/versions/5d942647566e_add_changelog.py` & `irrd-4.4.3/irrd/storage/alembic/versions/5d942647566e_add_changelog.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/alembic/versions/64a3d6faf6d4_add_prefix_length_rpki_status_to_rpsl_objects.py` & `irrd-4.4.3/irrd/storage/alembic/versions/64a3d6faf6d4_add_prefix_length_rpki_status_to_rpsl_objects.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/alembic/versions/8744b4b906bb_fix_rpsl_unique_key.py` & `irrd-4.4.3/irrd/storage/alembic/versions/8744b4b906bb_fix_rpsl_unique_key.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/alembic/versions/893d0d5363b3_add_rpsl_prefix_idx.py` & `irrd-4.4.3/irrd/storage/alembic/versions/893d0d5363b3_add_rpsl_prefix_idx.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/alembic/versions/8b8357acd333_add_global_serial.py` & `irrd-4.4.3/irrd/storage/alembic/versions/8b8357acd333_add_global_serial.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/alembic/versions/a7766c144d61_add_synchronised_serial_to_database_.py` & `irrd-4.4.3/irrd/storage/alembic/versions/a7766c144d61_add_synchronised_serial_to_database_.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/alembic/versions/a8609af97aa3_set_prefix_length_in_existing_rpsl_.py` & `irrd-4.4.3/irrd/storage/alembic/versions/a8609af97aa3_set_prefix_length_in_existing_rpsl_.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/alembic/versions/b175c262448f_set_rpsl_prefix.py` & `irrd-4.4.3/irrd/storage/alembic/versions/b175c262448f_set_rpsl_prefix.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/alembic/versions/e07863eac52f_add_roa_object_table.py` & `irrd-4.4.3/irrd/storage/alembic/versions/e07863eac52f_add_roa_object_table.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/alembic/versions/fd4473bc1a10_add_route_preference_status.py` & `irrd-4.4.3/irrd/storage/alembic/versions/fd4473bc1a10_add_route_preference_status.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/database_handler.py` & `irrd-4.4.3/irrd/storage/database_handler.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/event_stream.py` & `irrd-4.4.3/irrd/storage/event_stream.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/models.py` & `irrd-4.4.3/irrd/storage/models.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/orm_provider.py` & `irrd-4.4.3/irrd/storage/orm_provider.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/preload.py` & `irrd-4.4.3/irrd/storage/preload.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/storage/queries.py` & `irrd-4.4.3/irrd/storage/queries.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/updates/email.py` & `irrd-4.4.3/irrd/updates/email.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/updates/handler.py` & `irrd-4.4.3/irrd/updates/handler.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/updates/parser.py` & `irrd-4.4.3/irrd/updates/parser.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/updates/parser_state.py` & `irrd-4.4.3/irrd/updates/parser_state.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/updates/suspension.py` & `irrd-4.4.3/irrd/updates/suspension.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/updates/validators.py` & `irrd-4.4.3/irrd/updates/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -480,15 +480,15 @@
         mntner_pks_to_resolve: Set[str] = mntner_pk_set - {m.pk() for m in mntner_objs}
 
         if mntner_pks_to_resolve:
             query = RPSLDatabaseQuery().sources([source])
             query = query.object_classes(["mntner"]).rpsl_pks(mntner_pks_to_resolve)
             results = self.database_handler.execute_query(query)
 
-            retrieved_mntner_objs: List[RPSLMntner] = [rpsl_object_from_text(r["object_text"]) for r in results]  # type: ignore
+            retrieved_mntner_objs: List[RPSLMntner] = [rpsl_object_from_text(r["object_text"], strict_validation=False) for r in results]  # type: ignore
             self._mntner_db_cache.update(retrieved_mntner_objs)
             mntner_objs += retrieved_mntner_objs
 
         for mntner_name in mntner_pk_list:
             if mntner_name in self._pre_approved:
                 return MntnerCheckResult(
                     valid=True,
```

### Comparing `irrd-4.4.2/irrd/utils/email.py` & `irrd-4.4.3/irrd/utils/email.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/utils/factories.py` & `irrd-4.4.3/irrd/utils/factories.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/utils/pgp.py` & `irrd-4.4.3/irrd/utils/pgp.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/utils/process_support.py` & `irrd-4.4.3/irrd/utils/process_support.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/utils/rpsl_samples.py` & `irrd-4.4.3/irrd/utils/rpsl_samples.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/utils/test_utils.py` & `irrd-4.4.3/irrd/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/utils/text.py` & `irrd-4.4.3/irrd/utils/text.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/utils/validators.py` & `irrd-4.4.3/irrd/utils/validators.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/utils/whois_client.py` & `irrd-4.4.3/irrd/utils/whois_client.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/vendor/dotted/collection.py` & `irrd-4.4.3/irrd/vendor/dotted/collection.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/vendor/mock_alchemy/comparison.py` & `irrd-4.4.3/irrd/vendor/mock_alchemy/comparison.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/vendor/mock_alchemy/mocking.py` & `irrd-4.4.3/irrd/vendor/mock_alchemy/mocking.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/vendor/mock_alchemy/unittests.py` & `irrd-4.4.3/irrd/vendor/mock_alchemy/unittests.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/vendor/mock_alchemy/utils.py` & `irrd-4.4.3/irrd/vendor/mock_alchemy/utils.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/vendor/postgres_copy/__init__.py` & `irrd-4.4.3/irrd/vendor/postgres_copy/__init__.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/__init__.py` & `irrd-4.4.3/irrd/webui/__init__.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/auth/decorators.py` & `irrd-4.4.3/irrd/webui/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/auth/endpoints.py` & `irrd-4.4.3/irrd/webui/auth/endpoints.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/auth/endpoints_mfa.py` & `irrd-4.4.3/irrd/webui/auth/endpoints_mfa.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/auth/routes.py` & `irrd-4.4.3/irrd/webui/auth/routes.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/auth/users.py` & `irrd-4.4.3/irrd/webui/auth/users.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/endpoints.py` & `irrd-4.4.3/irrd/webui/endpoints.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/endpoints_mntners.py` & `irrd-4.4.3/irrd/webui/endpoints_mntners.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/helpers.py` & `irrd-4.4.3/irrd/webui/helpers.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/rendering.py` & `irrd-4.4.3/irrd/webui/rendering.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/routes.py` & `irrd-4.4.3/irrd/webui/routes.py`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/static/css/bootstrap.css` & `irrd-4.4.3/irrd/webui/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/static/css/bootstrap.min.css` & `irrd-4.4.3/irrd/webui/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/static/js/bootstrap.bundle.js` & `irrd-4.4.3/irrd/webui/static/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/static/js/bootstrap.bundle.min.js` & `irrd-4.4.3/irrd/webui/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/static/js/qrcode.js` & `irrd-4.4.3/irrd/webui/static/js/qrcode.js`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/static/js/simplewebauthn-browser-es5-umd.js` & `irrd-4.4.3/irrd/webui/static/js/simplewebauthn-browser-es5-umd.js`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/templates/api_token_form.html` & `irrd-4.4.3/irrd/webui/templates/api_token_form.html`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/templates/base.html` & `irrd-4.4.3/irrd/webui/templates/base.html`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/templates/change_log_entry.html` & `irrd-4.4.3/irrd/webui/templates/change_log_entry.html`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/templates/change_log_mntner.html` & `irrd-4.4.3/irrd/webui/templates/change_log_mntner.html`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/templates/create_account_confirm_form.html` & `irrd-4.4.3/irrd/webui/templates/create_account_confirm_form.html`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/templates/index.html` & `irrd-4.4.3/irrd/webui/templates/index.html`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/templates/login.html` & `irrd-4.4.3/irrd/webui/templates/login.html`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/templates/maintained_objects.html` & `irrd-4.4.3/irrd/webui/templates/maintained_objects.html`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/templates/mfa_authenticate.html` & `irrd-4.4.3/irrd/webui/templates/mfa_authenticate.html`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/templates/mfa_status.html` & `irrd-4.4.3/irrd/webui/templates/mfa_status.html`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/templates/mntner_migrate_complete.html` & `irrd-4.4.3/irrd/webui/templates/mntner_migrate_complete.html`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/templates/mntner_migrate_initiate.html` & `irrd-4.4.3/irrd/webui/templates/mntner_migrate_initiate.html`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/templates/mntner_migrate_initiate_mail.txt` & `irrd-4.4.3/irrd/webui/templates/mntner_migrate_initiate_mail.txt`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/templates/permission_delete.html` & `irrd-4.4.3/irrd/webui/templates/permission_delete.html`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/templates/permission_form.html` & `irrd-4.4.3/irrd/webui/templates/permission_form.html`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/templates/reset_password_request_form.html` & `irrd-4.4.3/irrd/webui/templates/reset_password_request_form.html`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/templates/rpsl_detail.html` & `irrd-4.4.3/irrd/webui/templates/rpsl_detail.html`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/templates/rpsl_form.html` & `irrd-4.4.3/irrd/webui/templates/rpsl_form.html`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/templates/totp_register.html` & `irrd-4.4.3/irrd/webui/templates/totp_register.html`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/templates/user_permissions.html` & `irrd-4.4.3/irrd/webui/templates/user_permissions.html`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/irrd/webui/templates/webauthn_register.html` & `irrd-4.4.3/irrd/webui/templates/webauthn_register.html`

 * *Files identical despite different names*

### Comparing `irrd-4.4.2/pyproject.toml` & `irrd-4.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 dynamic = ["version"]
 name = "irrd"
 
 [tool.poetry]
 name = "irrd"
 # Note that version is also in irrd/__init__.py
-version = "4.4.2"
+version = "4.4.3"
 description = "Internet Routing Registry daemon (IRRd)"
 authors = ["Reliably Coded for NTT Ltd. and others <irrd@reliablycoded.nl>"]
 license = "BSD"
 readme = "README.rst"
 repository = "https://github.com/irrdnet/irrd"
 documentation = "https://irrd.readthedocs.io/"
 exclude = ['irrd/*/tests', 'irrd/*/*/tests', 'irrd/integration_tests']
@@ -82,14 +82,15 @@
 smtpdfix = "^0.5.1"
 httpx = "^0.24.0"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^6.1.3"
 sphinxcontrib-spelling = "^8.0.0"
 sphinx-immaterial = "^0.11.4"
+pyenchant = "^3.2.2"
 
 [tool.poetry.scripts]
 irrd = 'irrd.daemon.main:main'
 irrdctl = 'irrd.scripts.irrd_control:cli'
 irrd_submit_email = 'irrd.scripts.submit_email:main'
 irrd_database_upgrade = 'irrd.scripts.database_upgrade:main'
 irrd_database_downgrade = 'irrd.scripts.database_downgrade:main'
@@ -163,9 +164,9 @@
     "irrd/scripts/load_test.py",
     "irrd/integration_tests/*",
     "irrd/vendor/*",
     "irrd/*/tests/*",
 ]
 
 [build-system]
-requires = ["poetry"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `irrd-4.4.2/PKG-INFO` & `irrd-4.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: irrd
-Version: 4.4.2
+Version: 4.4.3
 Summary: Internet Routing Registry daemon (IRRd)
 Home-page: https://github.com/irrdnet/irrd
 License: BSD
 Author: Reliably Coded for NTT Ltd. and others
 Author-email: irrd@reliablycoded.nl
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: alembic (==1.11.3)
 Requires-Dist: ariadne (==0.20.1)
 Requires-Dist: asgi-logger (==0.1.0)
 Requires-Dist: asgiref (==3.6.0)
 Requires-Dist: bcrypt (==4.0.1)
 Requires-Dist: beautifultable (==0.8.0)
 Requires-Dist: click (==8.1.7)
```

