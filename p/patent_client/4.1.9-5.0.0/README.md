# Comparing `tmp/patent_client-4.1.9.tar.gz` & `tmp/patent_client-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patent_client-4.1.9.tar", max compression
+gzip compressed data, was "patent_client-5.0.0.tar", max compression
```

## Comparing `patent_client-4.1.9.tar` & `patent_client-5.0.0.tar`

### file list

```diff
@@ -1,196 +1,409 @@
--rw-r--r--   0        0        0      593 2023-10-26 01:50:02.998756 patent_client-4.1.9/LICENSE
--rw-r--r--   0        0        0     5270 2023-12-11 17:13:20.222208 patent_client-4.1.9/README.md
--rw-r--r--   0        0        0     2601 2023-12-20 16:53:00.836281 patent_client-4.1.9/patent_client/__init__.py
--rw-r--r--   0        0        0      160 2023-11-10 19:32:12.643440 patent_client-4.1.9/patent_client/default_settings.yml
--rw-r--r--   0        0        0        0 2023-11-10 19:32:12.643469 patent_client-4.1.9/patent_client/epo/__init__.py
--rw-r--r--   0        0        0      242 2023-11-10 19:32:12.643857 patent_client-4.1.9/patent_client/epo/ops/__init__.py
--rw-r--r--   0        0        0        0 2023-11-10 19:32:12.643882 patent_client-4.1.9/patent_client/epo/ops/family/__init__.py
--rw-r--r--   0        0        0      382 2023-12-05 20:36:37.648154 patent_client-4.1.9/patent_client/epo/ops/family/api.py
--rw-r--r--   0        0        0      471 2023-12-11 16:08:08.301990 patent_client-4.1.9/patent_client/epo/ops/family/api_test.py
--rw-r--r--   0        0        0     7445 2023-12-05 02:55:55.743886 patent_client-4.1.9/patent_client/epo/ops/family/fixtures/family_api_output.json
--rw-r--r--   0        0        0     7247 2023-11-10 19:32:12.644919 patent_client-4.1.9/patent_client/epo/ops/family/fixtures/family_convert.json
--rw-r--r--   0        0        0     8854 2023-11-10 19:32:12.645352 patent_client-4.1.9/patent_client/epo/ops/family/fixtures/family_input.xml
--rw-r--r--   0        0        0     7445 2023-11-10 19:32:12.645493 patent_client-4.1.9/patent_client/epo/ops/family/fixtures/family_model_output.json
--rw-r--r--   0        0        0      346 2023-11-10 19:32:12.645709 patent_client-4.1.9/patent_client/epo/ops/family/manager.py
--rw-r--r--   0        0        0     1177 2023-11-10 19:32:12.645969 patent_client-4.1.9/patent_client/epo/ops/family/model.py
--rw-r--r--   0        0        0      834 2023-12-11 16:08:08.302089 patent_client-4.1.9/patent_client/epo/ops/family/model_test.py
--rw-r--r--   0        0        0     1577 2023-11-10 19:32:12.646410 patent_client-4.1.9/patent_client/epo/ops/family/schema.py
--rw-r--r--   0        0        0      526 2023-11-10 19:32:12.646798 patent_client-4.1.9/patent_client/epo/ops/family/schema_test.py
--rw-r--r--   0        0        0       77 2023-11-10 19:32:12.646866 patent_client-4.1.9/patent_client/epo/ops/legal/__init__.py
--rw-r--r--   0        0        0      386 2023-12-05 03:41:20.139138 patent_client-4.1.9/patent_client/epo/ops/legal/api.py
--rw-r--r--   0        0        0      329 2023-12-11 16:08:08.302236 patent_client-4.1.9/patent_client/epo/ops/legal/api_test.py
--rw-r--r--   0        0        0    76105 2023-11-10 19:32:12.651847 patent_client-4.1.9/patent_client/epo/ops/legal/fixtures/example_1.xml
--rw-r--r--   0        0        0    44094 2023-11-10 19:32:12.654429 patent_client-4.1.9/patent_client/epo/ops/legal/fixtures/example_1_convert.json
--rw-r--r--   0        0        0    78351 2023-11-10 19:32:12.654594 patent_client-4.1.9/patent_client/epo/ops/legal/fixtures/example_2.xml
--rw-r--r--   0        0        0    45316 2023-11-10 19:32:12.654896 patent_client-4.1.9/patent_client/epo/ops/legal/fixtures/example_2_convert.json
--rw-r--r--   0        0        0    22970 2023-11-10 19:32:12.655115 patent_client-4.1.9/patent_client/epo/ops/legal/fixtures/example_3.xml
--rw-r--r--   0        0        0    11923 2023-11-10 19:32:12.655250 patent_client-4.1.9/patent_client/epo/ops/legal/fixtures/example_3_convert.json
--rw-r--r--   0        0        0   291881 2023-11-10 19:32:12.656866 patent_client-4.1.9/patent_client/epo/ops/legal/legal_code_descriptions_2023-44-0.xlsx
--rw-r--r--   0        0        0      453 2023-11-10 19:32:12.656996 patent_client-4.1.9/patent_client/epo/ops/legal/manager.py
--rw-r--r--   0        0        0     2414 2023-11-14 18:50:57.754891 patent_client-4.1.9/patent_client/epo/ops/legal/model.py
--rw-r--r--   0        0        0     4855 2023-12-06 19:14:53.822126 patent_client-4.1.9/patent_client/epo/ops/legal/national_codes.py
--rw-r--r--   0        0        0      470 2023-11-10 19:32:12.657831 patent_client-4.1.9/patent_client/epo/ops/legal/national_codes_test.py
--rw-r--r--   0        0        0     4055 2023-11-10 19:32:12.657944 patent_client-4.1.9/patent_client/epo/ops/legal/schema.py
--rw-r--r--   0        0        0     1215 2023-11-10 19:32:12.658059 patent_client-4.1.9/patent_client/epo/ops/legal/schema_test.py
--rw-r--r--   0        0        0      114 2023-11-10 19:32:12.658115 patent_client-4.1.9/patent_client/epo/ops/legal/util.py
--rw-r--r--   0        0        0       67 2023-11-10 19:32:12.658179 patent_client-4.1.9/patent_client/epo/ops/number_service/__init__.py
--rw-r--r--   0        0        0     1404 2023-12-05 03:18:33.657117 patent_client-4.1.9/patent_client/epo/ops/number_service/api.py
--rw-r--r--   0        0        0     1740 2023-12-11 16:08:08.311357 patent_client-4.1.9/patent_client/epo/ops/number_service/api_test.py
--rw-r--r--   0        0        0     1141 2023-11-10 19:32:12.661490 patent_client-4.1.9/patent_client/epo/ops/number_service/errors.py
--rw-r--r--   0        0        0     5589 2023-11-10 19:32:12.661563 patent_client-4.1.9/patent_client/epo/ops/number_service/errors.txt
--rw-r--r--   0        0        0     2086 2023-11-10 19:32:12.661632 patent_client-4.1.9/patent_client/epo/ops/number_service/messages.txt
--rw-r--r--   0        0        0      782 2023-11-14 18:50:57.755164 patent_client-4.1.9/patent_client/epo/ops/number_service/model.py
--rw-r--r--   0        0        0      972 2023-11-10 19:32:12.661958 patent_client-4.1.9/patent_client/epo/ops/number_service/schema.py
--rw-r--r--   0        0        0        0 2023-11-10 19:32:12.661986 patent_client-4.1.9/patent_client/epo/ops/published/__init__.py
--rw-r--r--   0        0        0     5517 2023-12-07 21:30:06.993122 patent_client-4.1.9/patent_client/epo/ops/published/api.py
--rw-r--r--   0        0        0     2741 2023-12-11 16:08:08.306799 patent_client-4.1.9/patent_client/epo/ops/published/api_test.py
--rw-r--r--   0        0        0     1501 2023-11-10 19:32:12.671321 patent_client-4.1.9/patent_client/epo/ops/published/cql.py
--rw-r--r--   0        0        0     1956 2023-11-10 19:32:12.671453 patent_client-4.1.9/patent_client/epo/ops/published/fixtures/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0     6195 2023-12-31 15:29:43.302379 patent_client-4.1.9/patent_client/epo/ops/published/fixtures/ep1000000_biblio_result.json
--rw-r--r--   0        0        0     5148 2023-11-10 19:32:12.671931 patent_client-4.1.9/patent_client/epo/ops/published/fixtures/ep1000000_claims_result.json
--rw-r--r--   0        0        0    10706 2023-11-10 19:32:12.672112 patent_client-4.1.9/patent_client/epo/ops/published/fixtures/ep1000000_description_result.xml
--rw-r--r--   0        0        0    21196 2023-11-10 19:32:12.672191 patent_client-4.1.9/patent_client/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0    18516 2023-12-31 15:29:43.315924 patent_client-4.1.9/patent_client/epo/ops/published/fixtures/search_result.xml
--rw-r--r--   0        0        0     3244 2023-11-10 19:32:12.672635 patent_client-4.1.9/patent_client/epo/ops/published/manager.py
--rw-r--r--   0        0        0     3605 2023-12-11 17:00:45.818139 patent_client-4.1.9/patent_client/epo/ops/published/manager_test.py
--rw-r--r--   0        0        0      399 2023-11-10 19:32:12.673083 patent_client-4.1.9/patent_client/epo/ops/published/model/__init__.py
--rw-r--r--   0        0        0     2887 2023-11-10 19:32:12.673310 patent_client-4.1.9/patent_client/epo/ops/published/model/biblio.py
--rw-r--r--   0        0        0     1115 2023-11-10 19:32:12.673493 patent_client-4.1.9/patent_client/epo/ops/published/model/fulltext.py
--rw-r--r--   0        0        0     2166 2023-11-10 19:32:12.673655 patent_client-4.1.9/patent_client/epo/ops/published/model/images.py
--rw-r--r--   0        0        0      919 2023-11-10 19:32:12.673886 patent_client-4.1.9/patent_client/epo/ops/published/model/search.py
--rw-r--r--   0        0        0      306 2023-11-10 19:32:12.674071 patent_client-4.1.9/patent_client/epo/ops/published/schema/__init__.py
--rw-r--r--   0        0        0     3944 2023-11-10 19:32:12.674280 patent_client-4.1.9/patent_client/epo/ops/published/schema/biblio.py
--rw-r--r--   0        0        0      892 2023-11-10 19:32:12.674607 patent_client-4.1.9/patent_client/epo/ops/published/schema/fulltext.py
--rw-r--r--   0        0        0     1653 2023-11-10 19:32:12.674832 patent_client-4.1.9/patent_client/epo/ops/published/schema/images.py
--rw-r--r--   0        0        0      669 2023-11-10 19:32:12.674991 patent_client-4.1.9/patent_client/epo/ops/published/schema/search.py
--rw-r--r--   0        0        0     3219 2023-11-10 19:32:12.675264 patent_client-4.1.9/patent_client/epo/ops/published/schema_test.py
--rw-r--r--   0        0        0   105372 2023-11-10 19:32:12.675666 patent_client-4.1.9/patent_client/epo/ops/published/test/biblio_example.xml
--rw-r--r--   0        0        0    27945 2023-11-10 19:32:12.675917 patent_client-4.1.9/patent_client/epo/ops/published/test/biblio_example_2.xml
--rw-r--r--   0        0        0    13833 2023-11-10 19:32:12.675995 patent_client-4.1.9/patent_client/epo/ops/published/test/biblio_example_3.xml
--rw-r--r--   0        0        0    51036 2023-11-10 19:32:12.676074 patent_client-4.1.9/patent_client/epo/ops/published/test/biblio_example_4.xml
--rw-r--r--   0        0        0     7251 2023-12-31 15:29:43.496604 patent_client-4.1.9/patent_client/epo/ops/published/test/claims_example.json
--rw-r--r--   0        0        0     3973 2023-11-10 19:32:12.676450 patent_client-4.1.9/patent_client/epo/ops/published/test/claims_example.xml
--rw-r--r--   0        0        0    13020 2023-12-31 15:29:43.500703 patent_client-4.1.9/patent_client/epo/ops/published/test/claims_example_2.json
--rw-r--r--   0        0        0     5916 2023-11-10 19:32:12.676999 patent_client-4.1.9/patent_client/epo/ops/published/test/claims_example_2.xml
--rw-r--r--   0        0        0    12044 2023-11-10 19:32:12.677123 patent_client-4.1.9/patent_client/epo/ops/published/test/description_example.xml
--rw-r--r--   0        0        0     9211 2023-11-10 19:32:12.677261 patent_client-4.1.9/patent_client/epo/ops/published/test/expected/biblio_example_3.json
--rw-r--r--   0        0        0     8815 2023-11-10 19:32:12.677565 patent_client-4.1.9/patent_client/epo/ops/published/test/expected/biblio_example_4.json
--rw-r--r--   0        0        0     7197 2023-11-10 19:32:12.677964 patent_client-4.1.9/patent_client/epo/ops/published/test/expected/claims_example.json
--rw-r--r--   0        0        0     1956 2023-11-10 19:32:12.678033 patent_client-4.1.9/patent_client/epo/ops/published/test/expected/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0    13035 2023-11-10 19:32:12.678095 patent_client-4.1.9/patent_client/epo/ops/published/test/expected/ep1000000_biblio_result.xml
--rw-r--r--   0        0        0     3459 2023-11-10 19:32:12.678151 patent_client-4.1.9/patent_client/epo/ops/published/test/expected/ep1000000_claims_result.xml
--rw-r--r--   0        0        0    11421 2023-11-10 19:32:12.678236 patent_client-4.1.9/patent_client/epo/ops/published/test/expected/ep1000000_description_result.xml
--rw-r--r--   0        0        0    21196 2023-11-10 19:32:12.678301 patent_client-4.1.9/patent_client/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0     1076 2023-11-10 19:32:12.678520 patent_client-4.1.9/patent_client/epo/ops/published/test/expected/image_example.json
--rw-r--r--   0        0        0    34696 2023-11-10 19:32:12.678780 patent_client-4.1.9/patent_client/epo/ops/published/test/expected/search_result.xml
--rw-r--r--   0        0        0    21197 2023-11-10 19:32:12.678953 patent_client-4.1.9/patent_client/epo/ops/published/test/full_cycle_example.xml
--rw-r--r--   0        0        0     3059 2023-11-10 19:32:12.679045 patent_client-4.1.9/patent_client/epo/ops/published/test/image_example.xml
--rw-r--r--   0        0        0     5642 2023-11-10 19:32:12.679113 patent_client-4.1.9/patent_client/epo/ops/published/test/search_example.xml
--rw-r--r--   0        0        0     3454 2023-12-31 15:27:53.541088 patent_client-4.1.9/patent_client/epo/ops/session.py
--rw-r--r--   0        0        0     2437 2023-12-11 17:00:38.991262 patent_client-4.1.9/patent_client/epo/ops/util.py
--rw-r--r--   0        0        0     6003 2023-11-10 19:32:12.679694 patent_client-4.1.9/patent_client/parser.py
--rw-r--r--   0        0        0      331 2023-12-11 17:45:15.721394 patent_client-4.1.9/patent_client/patches.py
--rw-r--r--   0        0        0     4140 2023-12-14 22:27:14.012308 patent_client-4.1.9/patent_client/session.py
--rw-r--r--   0        0        0      667 2023-12-06 19:14:53.822998 patent_client-4.1.9/patent_client/settings.py
--rw-r--r--   0        0        0     8162 2023-11-10 19:32:12.680192 patent_client-4.1.9/patent_client/test_parser.py
--rw-r--r--   0        0        0      278 2023-11-10 19:32:12.680267 patent_client-4.1.9/patent_client/uspto/__init__.py
--rw-r--r--   0        0        0      105 2023-11-10 19:32:12.680335 patent_client-4.1.9/patent_client/uspto/assignment/__init__.py
--rw-r--r--   0        0        0     2313 2023-11-10 19:32:12.680558 patent_client-4.1.9/patent_client/uspto/assignment/api.py
--rw-r--r--   0        0        0     3543 2023-11-10 19:32:12.700066 patent_client-4.1.9/patent_client/uspto/assignment/convert.py
--rw-r--r--   0        0        0     1149 2023-11-10 19:32:12.700542 patent_client-4.1.9/patent_client/uspto/assignment/convert_test.py
--rw-r--r--   0        0        0     5926 2023-11-10 19:32:12.700803 patent_client-4.1.9/patent_client/uspto/assignment/fixtures/assignment_1.json
--rw-r--r--   0        0        0    13274 2023-11-10 19:32:12.701293 patent_client-4.1.9/patent_client/uspto/assignment/fixtures/assignment_1.xml
--rw-r--r--   0        0        0     4573 2023-11-10 19:32:12.701459 patent_client-4.1.9/patent_client/uspto/assignment/fixtures/assignment_2.json
--rw-r--r--   0        0        0    11638 2023-11-10 19:32:12.701532 patent_client-4.1.9/patent_client/uspto/assignment/fixtures/assignment_2.xml
--rw-r--r--   0        0        0   243532 2023-11-10 19:32:12.702178 patent_client-4.1.9/patent_client/uspto/assignment/fixtures/assignment_3.json
--rw-r--r--   0        0        0   277704 2023-11-10 19:32:12.702616 patent_client-4.1.9/patent_client/uspto/assignment/fixtures/assignment_3.xml
--rw-r--r--   0        0        0     3426 2023-11-10 19:32:12.705340 patent_client-4.1.9/patent_client/uspto/assignment/manager.py
--rw-r--r--   0        0        0     8609 2023-12-11 16:08:08.316372 patent_client-4.1.9/patent_client/uspto/assignment/manager_test.py
--rw-r--r--   0        0        0     5706 2023-11-14 18:50:57.755516 patent_client-4.1.9/patent_client/uspto/assignment/model.py
--rw-r--r--   0        0        0     2035 2023-11-10 19:32:12.706110 patent_client-4.1.9/patent_client/uspto/assignment/model_test.py
--rw-r--r--   0        0        0       87 2023-11-10 19:32:12.706422 patent_client-4.1.9/patent_client/uspto/assignment/session.py
--rw-r--r--   0        0        0        0 2023-11-14 21:11:03.404237 patent_client-4.1.9/patent_client/uspto/bulk_data/__init__.py
--rw-r--r--   0        0        0     3051 2023-11-14 21:11:03.404625 patent_client-4.1.9/patent_client/uspto/bulk_data/api.py
--rw-r--r--   0        0        0     1104 2023-12-11 16:08:08.320896 patent_client-4.1.9/patent_client/uspto/bulk_data/api_test.py
--rw-r--r--   0        0        0     3362 2023-11-14 21:15:19.353202 patent_client-4.1.9/patent_client/uspto/bulk_data/manager.py
--rw-r--r--   0        0        0     1427 2023-11-14 21:16:24.204077 patent_client-4.1.9/patent_client/uspto/bulk_data/manager_test.py
--rw-r--r--   0        0        0     1714 2023-11-14 21:11:03.408051 patent_client-4.1.9/patent_client/uspto/bulk_data/model.py
--rw-r--r--   0        0        0       87 2023-11-14 21:11:03.408278 patent_client-4.1.9/patent_client/uspto/bulk_data/session.py
--rw-r--r--   0        0        0        0 2023-11-10 19:32:12.706453 patent_client-4.1.9/patent_client/uspto/global_dossier/__init__.py
--rw-r--r--   0        0        0     1065 2023-11-10 19:32:12.706928 patent_client-4.1.9/patent_client/uspto/global_dossier/api.py
--rw-r--r--   0        0        0     2983 2023-11-10 19:32:12.713154 patent_client-4.1.9/patent_client/uspto/global_dossier/gd_input.csv
--rw-r--r--   0        0        0     1692 2023-11-10 19:32:12.713369 patent_client-4.1.9/patent_client/uspto/global_dossier/manager.py
--rw-r--r--   0        0        0     6656 2023-11-10 19:32:12.713602 patent_client-4.1.9/patent_client/uspto/global_dossier/model.py
--rw-r--r--   0        0        0     7393 2023-12-11 17:21:12.436848 patent_client-4.1.9/patent_client/uspto/global_dossier/model_test.py
--rw-r--r--   0        0        0     5837 2023-11-10 19:32:12.713961 patent_client-4.1.9/patent_client/uspto/global_dossier/query.py
--rw-r--r--   0        0        0     5270 2023-11-10 19:32:12.714148 patent_client-4.1.9/patent_client/uspto/global_dossier/query_test.py
--rw-r--r--   0        0        0      177 2023-12-11 17:13:20.348123 patent_client-4.1.9/patent_client/uspto/global_dossier/session.py
--rw-r--r--   0        0        0     4134 2023-11-10 19:32:12.714421 patent_client-4.1.9/patent_client/uspto/global_dossier/test/app.json
--rw-r--r--   0        0        0     2527 2023-11-10 19:32:12.714481 patent_client-4.1.9/patent_client/uspto/global_dossier/test/app_expected.json
--rw-r--r--   0        0        0    12360 2023-11-10 19:32:12.714550 patent_client-4.1.9/patent_client/uspto/global_dossier/test/doc_list.json
--rw-r--r--   0        0        0    10994 2023-11-10 19:32:12.714639 patent_client-4.1.9/patent_client/uspto/global_dossier/test/doc_list_expected.json
--rw-r--r--   0        0        0      151 2023-11-10 19:32:12.714829 patent_client-4.1.9/patent_client/uspto/peds/__init__.py
--rw-r--r--   0        0        0     4455 2023-12-05 04:04:46.087443 patent_client-4.1.9/patent_client/uspto/peds/api.py
--rw-r--r--   0        0        0      683 2023-12-11 16:08:08.316407 patent_client-4.1.9/patent_client/uspto/peds/api_test.py
--rw-r--r--   0        0        0    94707 2023-11-10 19:32:12.829444 patent_client-4.1.9/patent_client/uspto/peds/fixtures/app_1_input.json
--rw-r--r--   0        0        0    18324 2023-12-14 18:43:00.591773 patent_client-4.1.9/patent_client/uspto/peds/fixtures/app_1_output.json
--rw-r--r--   0        0        0     7977 2023-11-30 18:15:36.005924 patent_client-4.1.9/patent_client/uspto/peds/manager.py
--rw-r--r--   0        0        0    18739 2023-12-14 18:30:19.067326 patent_client-4.1.9/patent_client/uspto/peds/manager_test.py
--rw-r--r--   0        0        0    17208 2023-12-18 19:21:52.915609 patent_client-4.1.9/patent_client/uspto/peds/model.py
--rw-r--r--   0        0        0     6139 2023-11-29 17:18:13.700644 patent_client-4.1.9/patent_client/uspto/peds/query.py
--rw-r--r--   0        0        0     4469 2023-11-10 19:32:12.831687 patent_client-4.1.9/patent_client/uspto/peds/search_index.csv
--rw-r--r--   0        0        0       87 2023-12-04 20:58:32.833638 patent_client-4.1.9/patent_client/uspto/peds/session.py
--rw-r--r--   0        0        0      149 2023-11-10 19:32:12.832256 patent_client-4.1.9/patent_client/uspto/ptab/__init__.py
--rw-r--r--   0        0        0     9821 2023-11-10 19:32:12.832479 patent_client-4.1.9/patent_client/uspto/ptab/api.py
--rw-r--r--   0        0        0      688 2023-12-11 16:08:08.316336 patent_client-4.1.9/patent_client/uspto/ptab/api_test.py
--rw-r--r--   0        0        0     1300 2023-11-10 19:32:12.843557 patent_client-4.1.9/patent_client/uspto/ptab/fixtures/documents_input.json
--rw-r--r--   0        0        0     1057 2023-11-10 19:32:12.843763 patent_client-4.1.9/patent_client/uspto/ptab/fixtures/proceeding_input.json
--rw-r--r--   0        0        0     2076 2023-11-10 19:32:12.844054 patent_client-4.1.9/patent_client/uspto/ptab/manager.py
--rw-r--r--   0        0        0     4467 2023-12-11 16:08:08.316523 patent_client-4.1.9/patent_client/uspto/ptab/manager_test.py
--rw-r--r--   0        0        0     8603 2023-11-14 18:50:57.756146 patent_client-4.1.9/patent_client/uspto/ptab/model.py
--rw-r--r--   0        0        0       87 2023-11-10 19:32:12.844565 patent_client-4.1.9/patent_client/uspto/ptab/session.py
--rw-r--r--   0        0        0      242 2023-11-10 19:32:12.844758 patent_client-4.1.9/patent_client/uspto/ptab/util.py
--rw-r--r--   0        0        0      222 2023-11-10 19:32:12.845037 patent_client-4.1.9/patent_client/uspto/public_search/__init__.py
--rw-r--r--   0        0        0     5919 2023-12-14 18:43:00.592599 patent_client-4.1.9/patent_client/uspto/public_search/api.py
--rw-r--r--   0        0        0        0 2023-11-10 19:32:12.899617 patent_client-4.1.9/patent_client/uspto/public_search/convert/__init__.py
--rw-r--r--   0        0        0     2052 2023-11-10 19:32:12.899841 patent_client-4.1.9/patent_client/uspto/public_search/convert/biblio.py
--rw-r--r--   0        0        0     6607 2023-11-10 19:32:12.900044 patent_client-4.1.9/patent_client/uspto/public_search/convert/document.py
--rw-r--r--   0        0        0     1594 2023-11-10 19:32:12.900174 patent_client-4.1.9/patent_client/uspto/public_search/convert/shared.py
--rw-r--r--   0        0        0     1035 2023-11-10 19:32:12.900388 patent_client-4.1.9/patent_client/uspto/public_search/convert_test.py
--rw-r--r--   0        0        0   867778 2023-11-10 19:32:12.902368 patent_client-4.1.9/patent_client/uspto/public_search/fixtures/biblio.json
--rw-r--r--   0        0        0   270895 2023-11-10 19:32:12.903295 patent_client-4.1.9/patent_client/uspto/public_search/fixtures/biblio_convert.json
--rw-r--r--   0        0        0   220128 2023-11-10 19:32:12.903801 patent_client-4.1.9/patent_client/uspto/public_search/fixtures/biblio_output.json
--rw-r--r--   0        0        0  2431829 2023-11-10 19:32:12.912831 patent_client-4.1.9/patent_client/uspto/public_search/fixtures/doc.json
--rw-r--r--   0        0        0  2225007 2023-12-31 15:29:46.138310 patent_client-4.1.9/patent_client/uspto/public_search/fixtures/doc_convert.json
--rw-r--r--   0        0        0  3962033 2023-11-14 18:50:57.768749 patent_client-4.1.9/patent_client/uspto/public_search/fixtures/doc_output.json
--rw-r--r--   0        0        0     4187 2023-12-14 22:23:45.548378 patent_client-4.1.9/patent_client/uspto/public_search/manager.py
--rw-r--r--   0        0        0    15032 2023-12-11 16:08:08.311370 patent_client-4.1.9/patent_client/uspto/public_search/manager_test.py
--rw-r--r--   0        0        0      349 2023-11-10 19:32:12.938453 patent_client-4.1.9/patent_client/uspto/public_search/model/__init__.py
--rw-r--r--   0        0        0     3360 2023-12-14 18:43:00.592913 patent_client-4.1.9/patent_client/uspto/public_search/model/biblio.py
--rw-r--r--   0        0        0     8060 2023-12-14 18:43:00.593321 patent_client-4.1.9/patent_client/uspto/public_search/model/document.py
--rw-r--r--   0        0        0     2293 2023-12-14 18:43:00.593531 patent_client-4.1.9/patent_client/uspto/public_search/model/shared.py
--rw-r--r--   0        0        0     1557 2023-11-14 18:50:57.772944 patent_client-4.1.9/patent_client/uspto/public_search/model_test.py
--rw-r--r--   0        0        0     4331 2023-11-10 19:32:12.942652 patent_client-4.1.9/patent_client/uspto/public_search/query.py
--rw-r--r--   0        0        0     1344 2023-11-10 19:32:12.942706 patent_client-4.1.9/patent_client/uspto/public_search/query_config.csv
--rw-r--r--   0        0        0     3692 2023-11-10 19:32:12.942903 patent_client-4.1.9/patent_client/uspto/public_search/query_test.py
--rw-r--r--   0        0        0      298 2023-12-11 16:22:26.996697 patent_client-4.1.9/patent_client/uspto/public_search/session.py
--rw-r--r--   0        0        0      273 2023-11-10 19:32:12.943251 patent_client-4.1.9/patent_client/uspto/public_search/util.py
--rw-r--r--   0        0        0        0 2023-11-10 19:32:12.943277 patent_client-4.1.9/patent_client/util/__init__.py
--rw-r--r--   0        0        0     1002 2023-12-20 16:53:00.827161 patent_client-4.1.9/patent_client/util/asyncio_util.py
--rw-r--r--   0        0        0        0 2023-11-10 19:32:12.943507 patent_client-4.1.9/patent_client/util/claims/__init__.py
--rw-r--r--   0        0        0     4313 2023-12-31 15:29:47.509342 patent_client-4.1.9/patent_client/util/claims/examples/multiple_dependent.json
--rw-r--r--   0        0        0     2456 2023-11-10 19:32:12.943807 patent_client-4.1.9/patent_client/util/claims/examples/multiple_dependent.txt
--rw-r--r--   0        0        0     6924 2023-12-31 15:29:47.511974 patent_client-4.1.9/patent_client/util/claims/examples/published_claims.json
--rw-r--r--   0        0        0     3719 2023-11-10 19:32:12.943936 patent_client-4.1.9/patent_client/util/claims/examples/published_claims.txt
--rw-r--r--   0        0        0      732 2023-11-10 19:32:12.944128 patent_client-4.1.9/patent_client/util/claims/model.py
--rw-r--r--   0        0        0     3443 2023-11-10 19:32:12.944325 patent_client-4.1.9/patent_client/util/claims/parser.py
--rw-r--r--   0        0        0      938 2023-11-10 19:32:12.944520 patent_client-4.1.9/patent_client/util/claims/parser_test.py
--rw-r--r--   0        0        0      611 2023-11-10 19:32:12.944660 patent_client-4.1.9/patent_client/util/format.py
--rw-r--r--   0        0        0     5373 2023-11-10 19:32:12.944893 patent_client-4.1.9/patent_client/util/manager.py
--rw-r--r--   0        0        0     2692 2023-11-14 18:50:57.773147 patent_client-4.1.9/patent_client/util/pydantic_util.py
--rw-r--r--   0        0        0      171 2023-11-10 19:32:12.945265 patent_client-4.1.9/patent_client/util/related.py
--rw-r--r--   0        0        0      861 2023-11-10 19:32:12.945490 patent_client-4.1.9/patent_client/util/request_util.py
--rw-r--r--   0        0        0     2652 2023-11-10 19:32:12.945706 patent_client-4.1.9/patent_client/util/test.py
--rw-r--r--   0        0        0       22 2023-12-31 15:30:41.968152 patent_client-4.1.9/patent_client/version.py
--rw-r--r--   0        0        0     3627 2023-12-31 15:30:41.968388 patent_client-4.1.9/pyproject.toml
--rw-r--r--   0        0        0     6938 1970-01-01 00:00:00.000000 patent_client-4.1.9/PKG-INFO
+-rw-r--r--   0        0        0      593 2024-04-03 19:26:37.145253 patent_client-5.0.0/LICENSE
+-rw-r--r--   0        0        0     6104 2024-04-25 19:50:46.499667 patent_client-5.0.0/README.md
+-rw-r--r--   0        0        0     1708 2024-04-25 19:50:46.516333 patent_client-5.0.0/patent_client/__init__.py
+-rw-r--r--   0        0        0      839 2024-04-25 19:50:46.516665 patent_client-5.0.0/patent_client/_async/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.516700 patent_client-5.0.0/patent_client/_async/epo/__init__.py
+-rw-r--r--   0        0        0      214 2024-04-25 19:50:46.517020 patent_client-5.0.0/patent_client/_async/epo/ops/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.517050 patent_client-5.0.0/patent_client/_async/epo/ops/family/__init__.py
+-rw-r--r--   0        0        0      386 2024-04-25 19:50:46.517267 patent_client-5.0.0/patent_client/_async/epo/ops/family/api.py
+-rw-r--r--   0        0        0      471 2024-04-25 19:50:46.517324 patent_client-5.0.0/patent_client/_async/epo/ops/family/api_test.py
+-rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.518230 patent_client-5.0.0/patent_client/_async/epo/ops/family/fixtures/family_api_output.json
+-rw-r--r--   0        0        0     7247 2024-04-25 19:50:46.518338 patent_client-5.0.0/patent_client/_async/epo/ops/family/fixtures/family_convert.json
+-rw-r--r--   0        0        0     8854 2024-04-25 19:50:46.518473 patent_client-5.0.0/patent_client/_async/epo/ops/family/fixtures/family_input.xml
+-rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.518568 patent_client-5.0.0/patent_client/_async/epo/ops/family/fixtures/family_model_output.json
+-rw-r--r--   0        0        0      378 2024-04-25 19:50:46.518752 patent_client-5.0.0/patent_client/_async/epo/ops/family/manager.py
+-rw-r--r--   0        0        0     1119 2024-04-25 19:50:46.519067 patent_client-5.0.0/patent_client/_async/epo/ops/family/model.py
+-rw-r--r--   0        0        0      519 2024-04-25 19:50:46.519341 patent_client-5.0.0/patent_client/_async/epo/ops/family/model_test.py
+-rw-r--r--   0        0        0     1545 2024-04-25 19:50:46.519652 patent_client-5.0.0/patent_client/_async/epo/ops/family/schema.py
+-rw-r--r--   0        0        0      527 2024-04-25 19:50:46.520362 patent_client-5.0.0/patent_client/_async/epo/ops/family/schema_test.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.520397 patent_client-5.0.0/patent_client/_async/epo/ops/legal/__init__.py
+-rw-r--r--   0        0        0      361 2024-04-25 19:50:46.520529 patent_client-5.0.0/patent_client/_async/epo/ops/legal/api.py
+-rw-r--r--   0        0        0      320 2024-04-25 19:50:46.520929 patent_client-5.0.0/patent_client/_async/epo/ops/legal/api_test.py
+-rw-r--r--   0        0        0    76105 2024-04-25 19:50:46.522112 patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_1.xml
+-rw-r--r--   0        0        0    44094 2024-04-25 19:50:46.522207 patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_1_convert.json
+-rw-r--r--   0        0        0    78351 2024-04-25 19:50:46.522310 patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_2.xml
+-rw-r--r--   0        0        0    45316 2024-04-25 19:50:46.522377 patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_2_convert.json
+-rw-r--r--   0        0        0    22970 2024-04-25 19:50:46.522453 patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_3.xml
+-rw-r--r--   0        0        0    11923 2024-04-25 19:50:46.522568 patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_3_convert.json
+-rw-r--r--   0        0        0   292939 2024-04-25 19:50:46.528538 patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx
+-rw-r--r--   0        0        0      489 2024-04-25 19:50:46.528737 patent_client-5.0.0/patent_client/_async/epo/ops/legal/manager.py
+-rw-r--r--   0        0        0     2375 2024-04-25 19:50:46.528871 patent_client-5.0.0/patent_client/_async/epo/ops/legal/model.py
+-rw-r--r--   0        0        0     5399 2024-04-25 19:50:46.529038 patent_client-5.0.0/patent_client/_async/epo/ops/legal/national_codes.py
+-rw-r--r--   0        0        0      498 2024-04-25 19:50:46.529161 patent_client-5.0.0/patent_client/_async/epo/ops/legal/national_codes_test.py
+-rw-r--r--   0        0        0     4062 2024-04-25 19:50:46.529393 patent_client-5.0.0/patent_client/_async/epo/ops/legal/schema.py
+-rw-r--r--   0        0        0     1216 2024-04-25 19:50:46.529507 patent_client-5.0.0/patent_client/_async/epo/ops/legal/schema_test.py
+-rw-r--r--   0        0        0      114 2024-04-25 19:50:46.529573 patent_client-5.0.0/patent_client/_async/epo/ops/legal/util.py
+-rw-r--r--   0        0        0       67 2024-04-25 19:50:46.529635 patent_client-5.0.0/patent_client/_async/epo/ops/number_service/__init__.py
+-rw-r--r--   0        0        0     1417 2024-04-25 19:50:46.529887 patent_client-5.0.0/patent_client/_async/epo/ops/number_service/api.py
+-rw-r--r--   0        0        0     1806 2024-04-25 19:50:46.530201 patent_client-5.0.0/patent_client/_async/epo/ops/number_service/api_test.py
+-rw-r--r--   0        0        0     1117 2024-04-25 19:50:46.530931 patent_client-5.0.0/patent_client/_async/epo/ops/number_service/errors.py
+-rw-r--r--   0        0        0     5589 2024-04-25 19:50:46.531046 patent_client-5.0.0/patent_client/_async/epo/ops/number_service/errors.txt
+-rw-r--r--   0        0        0     2086 2024-04-25 19:50:46.531107 patent_client-5.0.0/patent_client/_async/epo/ops/number_service/messages.txt
+-rw-r--r--   0        0        0      763 2024-04-25 19:50:46.531354 patent_client-5.0.0/patent_client/_async/epo/ops/number_service/model.py
+-rw-r--r--   0        0        0      952 2024-04-25 19:50:46.531484 patent_client-5.0.0/patent_client/_async/epo/ops/number_service/schema.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.531523 patent_client-5.0.0/patent_client/_async/epo/ops/published/__init__.py
+-rw-r--r--   0        0        0     5650 2024-04-25 19:50:46.531713 patent_client-5.0.0/patent_client/_async/epo/ops/published/api.py
+-rw-r--r--   0        0        0     2849 2024-04-25 19:50:46.531966 patent_client-5.0.0/patent_client/_async/epo/ops/published/api_test.py
+-rw-r--r--   0        0        0     1501 2024-04-25 19:50:46.535532 patent_client-5.0.0/patent_client/_async/epo/ops/published/cql.py
+-rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.535641 patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0     6195 2024-04-25 19:50:46.535765 patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/ep1000000_biblio_result.json
+-rw-r--r--   0        0        0     5148 2024-04-25 19:50:46.535884 patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/ep1000000_claims_result.json
+-rw-r--r--   0        0        0    10706 2024-04-25 19:50:46.536001 patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    21196 2024-04-25 19:50:46.536077 patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0    18516 2024-04-25 19:50:46.536175 patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/search_result.xml
+-rw-r--r--   0        0        0     3261 2024-04-25 19:50:46.536305 patent_client-5.0.0/patent_client/_async/epo/ops/published/manager.py
+-rw-r--r--   0        0        0     2212 2024-04-25 19:50:46.536541 patent_client-5.0.0/patent_client/_async/epo/ops/published/manager_test.py
+-rw-r--r--   0        0        0      321 2024-04-25 19:50:46.536782 patent_client-5.0.0/patent_client/_async/epo/ops/published/model/__init__.py
+-rw-r--r--   0        0        0     2754 2024-04-25 19:50:46.536911 patent_client-5.0.0/patent_client/_async/epo/ops/published/model/biblio.py
+-rw-r--r--   0        0        0     1050 2024-04-25 19:50:46.537030 patent_client-5.0.0/patent_client/_async/epo/ops/published/model/fulltext.py
+-rw-r--r--   0        0        0     2084 2024-04-25 19:50:46.537277 patent_client-5.0.0/patent_client/_async/epo/ops/published/model/images.py
+-rw-r--r--   0        0        0      843 2024-04-25 19:50:46.537418 patent_client-5.0.0/patent_client/_async/epo/ops/published/model/search.py
+-rw-r--r--   0        0        0      285 2024-04-25 19:50:46.537840 patent_client-5.0.0/patent_client/_async/epo/ops/published/schema/__init__.py
+-rw-r--r--   0        0        0     3962 2024-04-25 19:50:46.538098 patent_client-5.0.0/patent_client/_async/epo/ops/published/schema/biblio.py
+-rw-r--r--   0        0        0      874 2024-04-25 19:50:46.538325 patent_client-5.0.0/patent_client/_async/epo/ops/published/schema/fulltext.py
+-rw-r--r--   0        0        0     1668 2024-04-25 19:50:46.538535 patent_client-5.0.0/patent_client/_async/epo/ops/published/schema/images.py
+-rw-r--r--   0        0        0      650 2024-04-25 19:50:46.538723 patent_client-5.0.0/patent_client/_async/epo/ops/published/schema/search.py
+-rw-r--r--   0        0        0     3193 2024-04-25 19:50:46.539173 patent_client-5.0.0/patent_client/_async/epo/ops/published/schema_test.py
+-rw-r--r--   0        0        0   105372 2024-04-25 19:50:46.539395 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/biblio_example.xml
+-rw-r--r--   0        0        0    27945 2024-04-25 19:50:46.539578 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/biblio_example_2.xml
+-rw-r--r--   0        0        0    13833 2024-04-25 19:50:46.539698 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/biblio_example_3.xml
+-rw-r--r--   0        0        0    51036 2024-04-25 19:50:46.539787 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/biblio_example_4.xml
+-rw-r--r--   0        0        0     7251 2024-04-25 19:50:46.539913 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/claims_example.json
+-rw-r--r--   0        0        0     3973 2024-04-25 19:50:46.539986 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/claims_example.xml
+-rw-r--r--   0        0        0    13020 2024-04-25 19:50:46.540088 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/claims_example_2.json
+-rw-r--r--   0        0        0     5916 2024-04-25 19:50:46.540212 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/claims_example_2.xml
+-rw-r--r--   0        0        0    12044 2024-04-25 19:50:46.540329 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/description_example.xml
+-rw-r--r--   0        0        0     9211 2024-04-25 19:50:46.540478 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/biblio_example_3.json
+-rw-r--r--   0        0        0     8815 2024-04-25 19:50:46.540611 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/biblio_example_4.json
+-rw-r--r--   0        0        0     7197 2024-04-25 19:50:46.540733 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/claims_example.json
+-rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.540800 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0    13035 2024-04-25 19:50:46.540898 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/ep1000000_biblio_result.xml
+-rw-r--r--   0        0        0     3459 2024-04-25 19:50:46.540961 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/ep1000000_claims_result.xml
+-rw-r--r--   0        0        0    11421 2024-04-25 19:50:46.541071 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    21196 2024-04-25 19:50:46.541138 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0     1076 2024-04-25 19:50:46.541208 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/image_example.json
+-rw-r--r--   0        0        0    34696 2024-04-25 19:50:46.541291 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/search_result.xml
+-rw-r--r--   0        0        0    21197 2024-04-25 19:50:46.541397 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/full_cycle_example.xml
+-rw-r--r--   0        0        0     3059 2024-04-25 19:50:46.541481 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/image_example.xml
+-rw-r--r--   0        0        0     5642 2024-04-25 19:50:46.541601 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/search_example.xml
+-rw-r--r--   0        0        0     3482 2024-04-25 19:50:46.541813 patent_client-5.0.0/patent_client/_async/epo/ops/session.py
+-rw-r--r--   0        0        0     2741 2024-04-25 19:50:46.541992 patent_client-5.0.0/patent_client/_async/epo/ops/util.py
+-rw-r--r--   0        0        0     3230 2024-04-25 19:50:46.542440 patent_client-5.0.0/patent_client/_async/http_client.py
+-rw-r--r--   0        0        0      202 2024-04-25 19:50:46.542670 patent_client-5.0.0/patent_client/_async/odp.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.542707 patent_client-5.0.0/patent_client/_async/uspto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.542758 patent_client-5.0.0/patent_client/_async/uspto/assignment/__init__.py
+-rw-r--r--   0        0        0     2552 2024-04-25 19:50:46.542893 patent_client-5.0.0/patent_client/_async/uspto/assignment/api.py
+-rw-r--r--   0        0        0      934 2024-04-25 19:50:46.543014 patent_client-5.0.0/patent_client/_async/uspto/assignment/api_test.py
+-rw-r--r--   0        0        0     3633 2024-04-25 19:50:46.559627 patent_client-5.0.0/patent_client/_async/uspto/assignment/convert.py
+-rw-r--r--   0        0        0     1149 2024-04-25 19:50:46.559695 patent_client-5.0.0/patent_client/_async/uspto/assignment/convert_test.py
+-rw-r--r--   0        0        0     5926 2024-04-25 19:50:46.559866 patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_1.json
+-rw-r--r--   0        0        0    13274 2024-04-25 19:50:46.560112 patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_1.xml
+-rw-r--r--   0        0        0     4573 2024-04-25 19:50:46.560215 patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_2.json
+-rw-r--r--   0        0        0    11638 2024-04-25 19:50:46.560334 patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_2.xml
+-rw-r--r--   0        0        0   243532 2024-04-25 19:50:46.560560 patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_3.json
+-rw-r--r--   0        0        0   277704 2024-04-25 19:50:46.560745 patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_3.xml
+-rw-r--r--   0        0        0     3445 2024-04-25 19:50:46.562396 patent_client-5.0.0/patent_client/_async/uspto/assignment/manager.py
+-rw-r--r--   0        0        0     4202 2024-04-25 19:50:46.562667 patent_client-5.0.0/patent_client/_async/uspto/assignment/manager_test.py
+-rw-r--r--   0        0        0     5466 2024-04-25 19:50:46.562938 patent_client-5.0.0/patent_client/_async/uspto/assignment/model.py
+-rw-r--r--   0        0        0     1932 2024-04-25 19:50:46.563119 patent_client-5.0.0/patent_client/_async/uspto/assignment/model_test.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.563151 patent_client-5.0.0/patent_client/_async/uspto/bulk_data/__init__.py
+-rw-r--r--   0        0        0     3208 2024-04-25 19:50:46.563555 patent_client-5.0.0/patent_client/_async/uspto/bulk_data/api.py
+-rw-r--r--   0        0        0     1100 2024-04-25 19:50:46.563680 patent_client-5.0.0/patent_client/_async/uspto/bulk_data/api_test.py
+-rw-r--r--   0        0        0     2781 2024-04-25 19:50:46.566025 patent_client-5.0.0/patent_client/_async/uspto/bulk_data/manager.py
+-rw-r--r--   0        0        0     1707 2024-04-25 19:50:46.566134 patent_client-5.0.0/patent_client/_async/uspto/bulk_data/manager_test.py
+-rw-r--r--   0        0        0     1558 2024-04-25 19:50:46.566440 patent_client-5.0.0/patent_client/_async/uspto/bulk_data/model.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.566476 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/__init__.py
+-rw-r--r--   0        0        0     2109 2024-04-25 19:50:46.566609 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/api.py
+-rw-r--r--   0        0        0     1143 2024-04-25 19:50:46.566720 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/api_test.py
+-rw-r--r--   0        0        0     2983 2024-04-25 19:50:46.606532 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/gd_input.csv
+-rw-r--r--   0        0        0     1902 2024-04-25 19:50:46.606761 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/manager.py
+-rw-r--r--   0        0        0     7111 2024-04-25 19:50:46.610118 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/model.py
+-rw-r--r--   0        0        0     3738 2024-04-25 19:50:46.611808 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/model_test.py
+-rw-r--r--   0        0        0     6063 2024-04-25 19:50:46.613527 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/query.py
+-rw-r--r--   0        0        0     5252 2024-04-25 19:50:46.613926 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/query_test.py
+-rw-r--r--   0        0        0     4134 2024-04-25 19:50:46.614090 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/test/app.json
+-rw-r--r--   0        0        0     2527 2024-04-25 19:50:46.614159 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/test/app_expected.json
+-rw-r--r--   0        0        0    12360 2024-04-25 19:50:46.614257 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/test/doc_list.json
+-rw-r--r--   0        0        0    10994 2024-04-25 19:50:46.614376 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/test/doc_list_expected.json
+-rw-r--r--   0        0        0        1 2024-04-25 19:50:46.614640 patent_client-5.0.0/patent_client/_async/uspto/odp/__init__.py
+-rw-r--r--   0        0        0     5524 2024-04-25 19:50:46.615019 patent_client-5.0.0/patent_client/_async/uspto/odp/api.py
+-rw-r--r--   0        0        0     2834 2024-04-25 19:50:46.615152 patent_client-5.0.0/patent_client/_async/uspto/odp/api_test.py
+-rw-r--r--   0        0        0    16485 2024-04-25 19:50:46.622009 patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/adjustment.json
+-rw-r--r--   0        0        0   187414 2024-04-25 19:50:46.622371 patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/application.json
+-rw-r--r--   0        0        0     1479 2024-04-25 19:50:46.622570 patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/assignment.json
+-rw-r--r--   0        0        0   172204 2024-04-25 19:50:46.622985 patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/attorney.json
+-rw-r--r--   0        0        0     2697 2024-04-25 19:50:46.623140 patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/biblio.json
+-rw-r--r--   0        0        0     1650 2024-04-25 19:50:46.623322 patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/continuity.json
+-rw-r--r--   0        0        0    72937 2024-04-25 19:50:46.623651 patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/documents.json
+-rw-r--r--   0        0        0      317 2024-04-25 19:50:46.623819 patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/foreign_priority.json
+-rw-r--r--   0        0        0     4077 2024-04-25 19:50:46.623951 patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/search.json
+-rw-r--r--   0        0        0    84893 2024-04-25 19:50:46.624215 patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/swagger.yaml
+-rw-r--r--   0        0        0     8767 2024-04-25 19:50:46.624391 patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/transactions.json
+-rw-r--r--   0        0        0     4863 2024-04-25 19:50:46.624619 patent_client-5.0.0/patent_client/_async/uspto/odp/manager.py
+-rw-r--r--   0        0        0     1895 2024-04-25 19:50:46.624873 patent_client-5.0.0/patent_client/_async/uspto/odp/manager_test.py
+-rw-r--r--   0        0        0    16311 2024-04-25 19:50:46.625251 patent_client-5.0.0/patent_client/_async/uspto/odp/model.py
+-rw-r--r--   0        0        0    12253 2024-04-25 19:50:46.625468 patent_client-5.0.0/patent_client/_async/uspto/odp/model_test.py
+-rw-r--r--   0        0        0     2396 2024-04-25 19:50:46.625599 patent_client-5.0.0/patent_client/_async/uspto/odp/query.py
+-rw-r--r--   0        0        0     2531 2024-04-25 19:50:46.625967 patent_client-5.0.0/patent_client/_async/uspto/odp/query_fields.csv
+-rw-r--r--   0        0        0      475 2024-04-25 19:50:46.628424 patent_client-5.0.0/patent_client/_async/uspto/odp/util.py
+-rw-r--r--   0        0        0      132 2024-04-25 19:50:46.628549 patent_client-5.0.0/patent_client/_async/uspto/peds/__init__.py
+-rw-r--r--   0        0        0     4501 2024-04-25 19:50:46.628716 patent_client-5.0.0/patent_client/_async/uspto/peds/api.py
+-rw-r--r--   0        0        0      711 2024-04-25 19:50:46.629004 patent_client-5.0.0/patent_client/_async/uspto/peds/api_test.py
+-rw-r--r--   0        0        0    94707 2024-04-25 19:50:46.659667 patent_client-5.0.0/patent_client/_async/uspto/peds/fixtures/app_1_input.json
+-rw-r--r--   0        0        0    18324 2024-04-25 19:50:46.659745 patent_client-5.0.0/patent_client/_async/uspto/peds/fixtures/app_1_output.json
+-rw-r--r--   0        0        0     8360 2024-04-25 19:50:46.659927 patent_client-5.0.0/patent_client/_async/uspto/peds/manager.py
+-rw-r--r--   0        0        0     9792 2024-04-25 19:50:46.660088 patent_client-5.0.0/patent_client/_async/uspto/peds/manager_test.py
+-rw-r--r--   0        0        0    16990 2024-04-25 19:50:46.664359 patent_client-5.0.0/patent_client/_async/uspto/peds/model.py
+-rw-r--r--   0        0        0     6116 2024-04-25 19:50:46.664816 patent_client-5.0.0/patent_client/_async/uspto/peds/query.py
+-rw-r--r--   0        0        0     4469 2024-04-25 19:50:46.665065 patent_client-5.0.0/patent_client/_async/uspto/peds/search_index.csv
+-rw-r--r--   0        0        0      149 2024-04-25 19:50:46.665140 patent_client-5.0.0/patent_client/_async/uspto/ptab/__init__.py
+-rw-r--r--   0        0        0    10200 2024-04-25 19:50:46.665671 patent_client-5.0.0/patent_client/_async/uspto/ptab/api.py
+-rw-r--r--   0        0        0      701 2024-04-25 19:50:46.666047 patent_client-5.0.0/patent_client/_async/uspto/ptab/api_test.py
+-rw-r--r--   0        0        0     1300 2024-04-25 19:50:46.668915 patent_client-5.0.0/patent_client/_async/uspto/ptab/fixtures/documents_input.json
+-rw-r--r--   0        0        0     1057 2024-04-25 19:50:46.668975 patent_client-5.0.0/patent_client/_async/uspto/ptab/fixtures/proceeding_input.json
+-rw-r--r--   0        0        0     2085 2024-04-25 19:50:46.669191 patent_client-5.0.0/patent_client/_async/uspto/ptab/manager.py
+-rw-r--r--   0        0        0     2311 2024-04-25 19:50:46.669333 patent_client-5.0.0/patent_client/_async/uspto/ptab/manager_test.py
+-rw-r--r--   0        0        0     8117 2024-04-25 19:50:46.669591 patent_client-5.0.0/patent_client/_async/uspto/ptab/model.py
+-rw-r--r--   0        0        0      242 2024-04-25 19:50:46.669654 patent_client-5.0.0/patent_client/_async/uspto/ptab/util.py
+-rw-r--r--   0        0        0      161 2024-04-25 19:50:46.669818 patent_client-5.0.0/patent_client/_async/uspto/public_search/__init__.py
+-rw-r--r--   0        0        0     6700 2024-04-25 19:50:46.670036 patent_client-5.0.0/patent_client/_async/uspto/public_search/api.py
+-rw-r--r--   0        0        0      298 2024-04-25 19:50:46.670256 patent_client-5.0.0/patent_client/_async/uspto/public_search/api_test.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.692132 patent_client-5.0.0/patent_client/_async/uspto/public_search/convert/__init__.py
+-rw-r--r--   0        0        0     2066 2024-04-25 19:50:46.694995 patent_client-5.0.0/patent_client/_async/uspto/public_search/convert/biblio.py
+-rw-r--r--   0        0        0     6678 2024-04-25 19:50:46.698061 patent_client-5.0.0/patent_client/_async/uspto/public_search/convert/document.py
+-rw-r--r--   0        0        0     1594 2024-04-25 19:50:46.698401 patent_client-5.0.0/patent_client/_async/uspto/public_search/convert/shared.py
+-rw-r--r--   0        0        0     1035 2024-04-25 19:50:46.698472 patent_client-5.0.0/patent_client/_async/uspto/public_search/convert_test.py
+-rw-r--r--   0        0        0      576 2024-04-25 19:50:46.698650 patent_client-5.0.0/patent_client/_async/uspto/public_search/count_query.json
+-rw-r--r--   0        0        0   867778 2024-04-25 19:50:46.699482 patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/biblio.json
+-rw-r--r--   0        0        0   270895 2024-04-25 19:50:46.699909 patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/biblio_convert.json
+-rw-r--r--   0        0        0   220128 2024-04-25 19:50:46.700055 patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/biblio_output.json
+-rw-r--r--   0        0        0  2431829 2024-04-25 19:50:46.704774 patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/doc.json
+-rw-r--r--   0        0        0  2225007 2024-04-25 19:50:46.706321 patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/doc_convert.json
+-rw-r--r--   0        0        0  3962033 2024-04-25 19:50:46.708274 patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/doc_output.json
+-rw-r--r--   0        0        0     4144 2024-04-25 19:50:46.712656 patent_client-5.0.0/patent_client/_async/uspto/public_search/manager.py
+-rw-r--r--   0        0        0     7743 2024-04-25 19:50:46.716625 patent_client-5.0.0/patent_client/_async/uspto/public_search/manager_test.py
+-rw-r--r--   0        0        0      330 2024-04-25 19:50:46.716790 patent_client-5.0.0/patent_client/_async/uspto/public_search/model/__init__.py
+-rw-r--r--   0        0        0     3144 2024-04-25 19:50:46.716934 patent_client-5.0.0/patent_client/_async/uspto/public_search/model/biblio.py
+-rw-r--r--   0        0        0     7574 2024-04-25 19:50:46.717130 patent_client-5.0.0/patent_client/_async/uspto/public_search/model/document.py
+-rw-r--r--   0        0        0     2249 2024-04-25 19:50:46.719323 patent_client-5.0.0/patent_client/_async/uspto/public_search/model/shared.py
+-rw-r--r--   0        0        0     1537 2024-04-25 19:50:46.719456 patent_client-5.0.0/patent_client/_async/uspto/public_search/model_test.py
+-rw-r--r--   0        0        0     4520 2024-04-25 19:50:46.722417 patent_client-5.0.0/patent_client/_async/uspto/public_search/query.py
+-rw-r--r--   0        0        0     1344 2024-04-25 19:50:46.722489 patent_client-5.0.0/patent_client/_async/uspto/public_search/query_config.csv
+-rw-r--r--   0        0        0     4313 2024-04-25 19:50:46.722791 patent_client-5.0.0/patent_client/_async/uspto/public_search/query_test.py
+-rw-r--r--   0        0        0     1049 2024-04-25 19:50:46.722977 patent_client-5.0.0/patent_client/_async/uspto/public_search/search_query.json
+-rw-r--r--   0        0        0      273 2024-04-25 19:50:46.723043 patent_client-5.0.0/patent_client/_async/uspto/public_search/util.py
+-rw-r--r--   0        0        0     1255 2024-04-25 19:50:46.723166 patent_client-5.0.0/patent_client/_sync/__init__.py
+-rw-r--r--   0        0        0      416 2024-04-25 19:50:46.723379 patent_client-5.0.0/patent_client/_sync/epo/__init__.py
+-rw-r--r--   0        0        0      630 2024-04-25 19:50:46.723511 patent_client-5.0.0/patent_client/_sync/epo/ops/__init__.py
+-rw-r--r--   0        0        0      416 2024-04-25 19:50:46.723823 patent_client-5.0.0/patent_client/_sync/epo/ops/family/__init__.py
+-rw-r--r--   0        0        0      790 2024-04-25 19:50:46.724222 patent_client-5.0.0/patent_client/_sync/epo/ops/family/api.py
+-rw-r--r--   0        0        0      855 2024-04-25 19:50:46.724547 patent_client-5.0.0/patent_client/_sync/epo/ops/family/api_test.py
+-rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.725140 patent_client-5.0.0/patent_client/_sync/epo/ops/family/fixtures/family_api_output.json
+-rw-r--r--   0        0        0     7247 2024-04-25 19:50:46.725251 patent_client-5.0.0/patent_client/_sync/epo/ops/family/fixtures/family_convert.json
+-rw-r--r--   0        0        0     8854 2024-04-25 19:50:46.725360 patent_client-5.0.0/patent_client/_sync/epo/ops/family/fixtures/family_input.xml
+-rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.725470 patent_client-5.0.0/patent_client/_sync/epo/ops/family/fixtures/family_model_output.json
+-rw-r--r--   0        0        0      772 2024-04-25 19:50:46.725581 patent_client-5.0.0/patent_client/_sync/epo/ops/family/manager.py
+-rw-r--r--   0        0        0     1535 2024-04-25 19:50:46.725776 patent_client-5.0.0/patent_client/_sync/epo/ops/family/model.py
+-rw-r--r--   0        0        0      903 2024-04-25 19:50:46.725892 patent_client-5.0.0/patent_client/_sync/epo/ops/family/model_test.py
+-rw-r--r--   0        0        0     1961 2024-04-25 19:50:46.725998 patent_client-5.0.0/patent_client/_sync/epo/ops/family/schema.py
+-rw-r--r--   0        0        0      943 2024-04-25 19:50:46.726102 patent_client-5.0.0/patent_client/_sync/epo/ops/family/schema_test.py
+-rw-r--r--   0        0        0      416 2024-04-25 19:50:46.726325 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/__init__.py
+-rw-r--r--   0        0        0      765 2024-04-25 19:50:46.726444 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/api.py
+-rw-r--r--   0        0        0      704 2024-04-25 19:50:46.726566 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/api_test.py
+-rw-r--r--   0        0        0    76105 2024-04-25 19:50:46.731050 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/fixtures/example_1.xml
+-rw-r--r--   0        0        0    44094 2024-04-25 19:50:46.731151 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/fixtures/example_1_convert.json
+-rw-r--r--   0        0        0    78351 2024-04-25 19:50:46.731269 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/fixtures/example_2.xml
+-rw-r--r--   0        0        0    45316 2024-04-25 19:50:46.731525 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/fixtures/example_2_convert.json
+-rw-r--r--   0        0        0    22970 2024-04-25 19:50:46.731642 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/fixtures/example_3.xml
+-rw-r--r--   0        0        0    11923 2024-04-25 19:50:46.731778 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/fixtures/example_3_convert.json
+-rw-r--r--   0        0        0   292939 2024-04-25 19:50:46.732730 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx
+-rw-r--r--   0        0        0   291881 2024-04-25 19:50:46.733722 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/legal_code_descriptions_2023-44-0.xlsx
+-rw-r--r--   0        0        0      883 2024-04-25 19:50:46.733910 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/manager.py
+-rw-r--r--   0        0        0     2791 2024-04-25 19:50:46.735502 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/model.py
+-rw-r--r--   0        0        0     5753 2024-04-25 19:50:46.735838 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/national_codes.py
+-rw-r--r--   0        0        0      882 2024-04-25 19:50:46.735986 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/national_codes_test.py
+-rw-r--r--   0        0        0     4478 2024-04-25 19:50:46.736419 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/schema.py
+-rw-r--r--   0        0        0     1632 2024-04-25 19:50:46.736570 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/schema_test.py
+-rw-r--r--   0        0        0      530 2024-04-25 19:50:46.736711 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/util.py
+-rw-r--r--   0        0        0      483 2024-04-25 19:50:46.736849 patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/__init__.py
+-rw-r--r--   0        0        0     1821 2024-04-25 19:50:46.736982 patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/api.py
+-rw-r--r--   0        0        0     2062 2024-04-25 19:50:46.737103 patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/api_test.py
+-rw-r--r--   0        0        0     1533 2024-04-25 19:50:46.738134 patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/errors.py
+-rw-r--r--   0        0        0     5589 2024-04-25 19:50:46.738251 patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/errors.txt
+-rw-r--r--   0        0        0     2086 2024-04-25 19:50:46.738313 patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/messages.txt
+-rw-r--r--   0        0        0     1179 2024-04-25 19:50:46.738445 patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/model.py
+-rw-r--r--   0        0        0     1368 2024-04-25 19:50:46.738569 patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/schema.py
+-rw-r--r--   0        0        0      416 2024-04-25 19:50:46.738708 patent_client-5.0.0/patent_client/_sync/epo/ops/published/__init__.py
+-rw-r--r--   0        0        0     5934 2024-04-25 19:50:46.739051 patent_client-5.0.0/patent_client/_sync/epo/ops/published/api.py
+-rw-r--r--   0        0        0     3073 2024-04-25 19:50:46.739287 patent_client-5.0.0/patent_client/_sync/epo/ops/published/api_test.py
+-rw-r--r--   0        0        0     1917 2024-04-25 19:50:46.750057 patent_client-5.0.0/patent_client/_sync/epo/ops/published/cql.py
+-rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.750171 patent_client-5.0.0/patent_client/_sync/epo/ops/published/fixtures/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0     6174 2024-04-25 19:50:46.750486 patent_client-5.0.0/patent_client/_sync/epo/ops/published/fixtures/ep1000000_biblio_result.json
+-rw-r--r--   0        0        0     5148 2024-04-25 19:50:46.750620 patent_client-5.0.0/patent_client/_sync/epo/ops/published/fixtures/ep1000000_claims_result.json
+-rw-r--r--   0        0        0    10706 2024-04-25 19:50:46.750740 patent_client-5.0.0/patent_client/_sync/epo/ops/published/fixtures/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    20102 2024-04-25 19:50:46.750995 patent_client-5.0.0/patent_client/_sync/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0    18510 2024-04-25 19:50:46.751449 patent_client-5.0.0/patent_client/_sync/epo/ops/published/fixtures/search_result.xml
+-rw-r--r--   0        0        0     3551 2024-04-25 19:50:46.751824 patent_client-5.0.0/patent_client/_sync/epo/ops/published/manager.py
+-rw-r--r--   0        0        0     2286 2024-04-25 19:50:46.752196 patent_client-5.0.0/patent_client/_sync/epo/ops/published/manager_test.py
+-rw-r--r--   0        0        0      737 2024-04-25 19:50:46.752406 patent_client-5.0.0/patent_client/_sync/epo/ops/published/model/__init__.py
+-rw-r--r--   0        0        0     3170 2024-04-25 19:50:46.753562 patent_client-5.0.0/patent_client/_sync/epo/ops/published/model/biblio.py
+-rw-r--r--   0        0        0     1466 2024-04-25 19:50:46.753818 patent_client-5.0.0/patent_client/_sync/epo/ops/published/model/fulltext.py
+-rw-r--r--   0        0        0     2500 2024-04-25 19:50:46.754620 patent_client-5.0.0/patent_client/_sync/epo/ops/published/model/images.py
+-rw-r--r--   0        0        0     1259 2024-04-25 19:50:46.755053 patent_client-5.0.0/patent_client/_sync/epo/ops/published/model/search.py
+-rw-r--r--   0        0        0      701 2024-04-25 19:50:46.755310 patent_client-5.0.0/patent_client/_sync/epo/ops/published/schema/__init__.py
+-rw-r--r--   0        0        0     4378 2024-04-25 19:50:46.756124 patent_client-5.0.0/patent_client/_sync/epo/ops/published/schema/biblio.py
+-rw-r--r--   0        0        0     1290 2024-04-25 19:50:46.756266 patent_client-5.0.0/patent_client/_sync/epo/ops/published/schema/fulltext.py
+-rw-r--r--   0        0        0     2084 2024-04-25 19:50:46.756499 patent_client-5.0.0/patent_client/_sync/epo/ops/published/schema/images.py
+-rw-r--r--   0        0        0     1066 2024-04-25 19:50:46.756981 patent_client-5.0.0/patent_client/_sync/epo/ops/published/schema/search.py
+-rw-r--r--   0        0        0     3609 2024-04-25 19:50:46.757116 patent_client-5.0.0/patent_client/_sync/epo/ops/published/schema_test.py
+-rw-r--r--   0        0        0   105372 2024-04-25 19:50:46.757289 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/biblio_example.xml
+-rw-r--r--   0        0        0    27945 2024-04-25 19:50:46.757399 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/biblio_example_2.xml
+-rw-r--r--   0        0        0    13833 2024-04-25 19:50:46.757681 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/biblio_example_3.xml
+-rw-r--r--   0        0        0    51036 2024-04-25 19:50:46.757775 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/biblio_example_4.xml
+-rw-r--r--   0        0        0     7251 2024-04-25 19:50:46.757901 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/claims_example.json
+-rw-r--r--   0        0        0     3973 2024-04-25 19:50:46.757965 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/claims_example.xml
+-rw-r--r--   0        0        0    13020 2024-04-25 19:50:46.758078 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/claims_example_2.json
+-rw-r--r--   0        0        0     5916 2024-04-25 19:50:46.758194 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/claims_example_2.xml
+-rw-r--r--   0        0        0    12044 2024-04-25 19:50:46.758423 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/description_example.xml
+-rw-r--r--   0        0        0     9211 2024-04-25 19:50:46.758601 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/biblio_example_3.json
+-rw-r--r--   0        0        0     8815 2024-04-25 19:50:46.758726 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/biblio_example_4.json
+-rw-r--r--   0        0        0     7197 2024-04-25 19:50:46.758859 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/claims_example.json
+-rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.758949 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0    13035 2024-04-25 19:50:46.759057 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/ep1000000_biblio_result.xml
+-rw-r--r--   0        0        0     3459 2024-04-25 19:50:46.759123 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/ep1000000_claims_result.xml
+-rw-r--r--   0        0        0    11421 2024-04-25 19:50:46.759232 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    21196 2024-04-25 19:50:46.759296 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0     1076 2024-04-25 19:50:46.759369 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/image_example.json
+-rw-r--r--   0        0        0    34696 2024-04-25 19:50:46.759484 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/search_result.xml
+-rw-r--r--   0        0        0    21197 2024-04-25 19:50:46.759585 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/full_cycle_example.xml
+-rw-r--r--   0        0        0     3059 2024-04-25 19:50:46.759654 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/image_example.xml
+-rw-r--r--   0        0        0     5642 2024-04-25 19:50:46.759897 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/search_example.xml
+-rw-r--r--   0        0        0     3876 2024-04-25 19:50:46.760034 patent_client-5.0.0/patent_client/_sync/epo/ops/session.py
+-rw-r--r--   0        0        0     3008 2024-04-25 19:50:46.760181 patent_client-5.0.0/patent_client/_sync/epo/ops/util.py
+-rw-r--r--   0        0        0     3607 2024-04-25 19:50:46.760452 patent_client-5.0.0/patent_client/_sync/http_client.py
+-rw-r--r--   0        0        0      617 2024-04-25 19:50:46.760692 patent_client-5.0.0/patent_client/_sync/odp.py
+-rw-r--r--   0        0        0      416 2024-04-25 19:50:46.760938 patent_client-5.0.0/patent_client/_sync/uspto/__init__.py
+-rw-r--r--   0        0        0      416 2024-04-25 19:50:46.761073 patent_client-5.0.0/patent_client/_sync/uspto/assignment/__init__.py
+-rw-r--r--   0        0        0     2936 2024-04-25 19:50:46.761193 patent_client-5.0.0/patent_client/_sync/uspto/assignment/api.py
+-rw-r--r--   0        0        0     1286 2024-04-25 19:50:46.761308 patent_client-5.0.0/patent_client/_sync/uspto/assignment/api_test.py
+-rw-r--r--   0        0        0     4049 2024-04-25 19:50:46.771159 patent_client-5.0.0/patent_client/_sync/uspto/assignment/convert.py
+-rw-r--r--   0        0        0     1565 2024-04-25 19:50:46.772719 patent_client-5.0.0/patent_client/_sync/uspto/assignment/convert_test.py
+-rw-r--r--   0        0        0     5926 2024-04-25 19:50:46.772880 patent_client-5.0.0/patent_client/_sync/uspto/assignment/fixtures/assignment_1.json
+-rw-r--r--   0        0        0    13274 2024-04-25 19:50:46.773005 patent_client-5.0.0/patent_client/_sync/uspto/assignment/fixtures/assignment_1.xml
+-rw-r--r--   0        0        0     4573 2024-04-25 19:50:46.773107 patent_client-5.0.0/patent_client/_sync/uspto/assignment/fixtures/assignment_2.json
+-rw-r--r--   0        0        0    11638 2024-04-25 19:50:46.773225 patent_client-5.0.0/patent_client/_sync/uspto/assignment/fixtures/assignment_2.xml
+-rw-r--r--   0        0        0   243532 2024-04-25 19:50:46.773450 patent_client-5.0.0/patent_client/_sync/uspto/assignment/fixtures/assignment_3.json
+-rw-r--r--   0        0        0   277704 2024-04-25 19:50:46.773639 patent_client-5.0.0/patent_client/_sync/uspto/assignment/fixtures/assignment_3.xml
+-rw-r--r--   0        0        0     3817 2024-04-25 19:50:46.773871 patent_client-5.0.0/patent_client/_sync/uspto/assignment/manager.py
+-rw-r--r--   0        0        0     4308 2024-04-25 19:50:46.774130 patent_client-5.0.0/patent_client/_sync/uspto/assignment/manager_test.py
+-rw-r--r--   0        0        0     5870 2024-04-25 19:50:46.774420 patent_client-5.0.0/patent_client/_sync/uspto/assignment/model.py
+-rw-r--r--   0        0        0     2348 2024-04-25 19:50:46.774671 patent_client-5.0.0/patent_client/_sync/uspto/assignment/model_test.py
+-rw-r--r--   0        0        0      416 2024-04-25 19:50:46.774789 patent_client-5.0.0/patent_client/_sync/uspto/bulk_data/__init__.py
+-rw-r--r--   0        0        0     3575 2024-04-25 19:50:46.774902 patent_client-5.0.0/patent_client/_sync/uspto/bulk_data/api.py
+-rw-r--r--   0        0        0     1382 2024-04-25 19:50:46.775011 patent_client-5.0.0/patent_client/_sync/uspto/bulk_data/api_test.py
+-rw-r--r--   0        0        0     3113 2024-04-25 19:50:46.776499 patent_client-5.0.0/patent_client/_sync/uspto/bulk_data/manager.py
+-rw-r--r--   0        0        0     1963 2024-04-25 19:50:46.776623 patent_client-5.0.0/patent_client/_sync/uspto/bulk_data/manager_test.py
+-rw-r--r--   0        0        0     1962 2024-04-25 19:50:46.776743 patent_client-5.0.0/patent_client/_sync/uspto/bulk_data/model.py
+-rw-r--r--   0        0        0      416 2024-04-25 19:50:46.776873 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/__init__.py
+-rw-r--r--   0        0        0     2446 2024-04-25 19:50:46.776992 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/api.py
+-rw-r--r--   0        0        0     1463 2024-04-25 19:50:46.777323 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/api_test.py
+-rw-r--r--   0        0        0     2983 2024-04-25 19:50:46.819170 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/gd_input.csv
+-rw-r--r--   0        0        0     2272 2024-04-25 19:50:46.819397 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/manager.py
+-rw-r--r--   0        0        0     7354 2024-04-25 19:50:46.820973 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/model.py
+-rw-r--r--   0        0        0     3853 2024-04-25 19:50:46.821302 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/model_test.py
+-rw-r--r--   0        0        0     6479 2024-04-25 19:50:46.822907 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/query.py
+-rw-r--r--   0        0        0     5668 2024-04-25 19:50:46.823088 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/query_test.py
+-rw-r--r--   0        0        0     4134 2024-04-25 19:50:46.823233 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/test/app.json
+-rw-r--r--   0        0        0     2527 2024-04-25 19:50:46.823291 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/test/app_expected.json
+-rw-r--r--   0        0        0    12360 2024-04-25 19:50:46.823387 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/test/doc_list.json
+-rw-r--r--   0        0        0    10994 2024-04-25 19:50:46.823499 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/test/doc_list_expected.json
+-rw-r--r--   0        0        0      417 2024-04-25 19:50:46.823618 patent_client-5.0.0/patent_client/_sync/uspto/odp/__init__.py
+-rw-r--r--   0        0        0     5822 2024-04-25 19:50:46.823779 patent_client-5.0.0/patent_client/_sync/uspto/odp/api.py
+-rw-r--r--   0        0        0     2898 2024-04-25 19:50:46.824087 patent_client-5.0.0/patent_client/_sync/uspto/odp/api_test.py
+-rw-r--r--   0        0        0    16485 2024-04-25 19:50:46.830209 patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/adjustment.json
+-rw-r--r--   0        0        0   187414 2024-04-25 19:50:46.830453 patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/application.json
+-rw-r--r--   0        0        0     1479 2024-04-25 19:50:46.830552 patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/assignment.json
+-rw-r--r--   0        0        0   172204 2024-04-25 19:50:46.830776 patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/attorney.json
+-rw-r--r--   0        0        0     2697 2024-04-25 19:50:46.830907 patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/biblio.json
+-rw-r--r--   0        0        0     1650 2024-04-25 19:50:46.830994 patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/continuity.json
+-rw-r--r--   0        0        0    72937 2024-04-25 19:50:46.831136 patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/documents.json
+-rw-r--r--   0        0        0      317 2024-04-25 19:50:46.831239 patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/foreign_priority.json
+-rw-r--r--   0        0        0     4077 2024-04-25 19:50:46.831429 patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/search.json
+-rw-r--r--   0        0        0    84893 2024-04-25 19:50:46.831608 patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/swagger.yaml
+-rw-r--r--   0        0        0     8767 2024-04-25 19:50:46.831762 patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/transactions.json
+-rw-r--r--   0        0        0     5082 2024-04-25 19:50:46.833233 patent_client-5.0.0/patent_client/_sync/uspto/odp/manager.py
+-rw-r--r--   0        0        0     1973 2024-04-25 19:50:46.833456 patent_client-5.0.0/patent_client/_sync/uspto/odp/manager_test.py
+-rw-r--r--   0        0        0    15504 2024-04-25 19:50:46.833707 patent_client-5.0.0/patent_client/_sync/uspto/odp/model.py
+-rw-r--r--   0        0        0    12669 2024-04-25 19:50:46.834120 patent_client-5.0.0/patent_client/_sync/uspto/odp/model_test.py
+-rw-r--r--   0        0        0     2812 2024-04-25 19:50:46.834328 patent_client-5.0.0/patent_client/_sync/uspto/odp/query.py
+-rw-r--r--   0        0        0     2531 2024-04-25 19:50:46.834414 patent_client-5.0.0/patent_client/_sync/uspto/odp/query_fields.csv
+-rw-r--r--   0        0        0      891 2024-04-25 19:50:46.834544 patent_client-5.0.0/patent_client/_sync/uspto/odp/util.py
+-rw-r--r--   0        0        0      548 2024-04-25 19:50:46.834685 patent_client-5.0.0/patent_client/_sync/uspto/peds/__init__.py
+-rw-r--r--   0        0        0     4838 2024-04-25 19:50:46.834873 patent_client-5.0.0/patent_client/_sync/uspto/peds/api.py
+-rw-r--r--   0        0        0     1031 2024-04-25 19:50:46.835135 patent_client-5.0.0/patent_client/_sync/uspto/peds/api_test.py
+-rw-r--r--   0        0        0    94707 2024-04-25 19:50:46.853167 patent_client-5.0.0/patent_client/_sync/uspto/peds/fixtures/app_1_input.json
+-rw-r--r--   0        0        0    18324 2024-04-25 19:50:46.853244 patent_client-5.0.0/patent_client/_sync/uspto/peds/fixtures/app_1_output.json
+-rw-r--r--   0        0        0     8674 2024-04-25 19:50:46.855392 patent_client-5.0.0/patent_client/_sync/uspto/peds/manager.py
+-rw-r--r--   0        0        0     9528 2024-04-25 19:50:46.855604 patent_client-5.0.0/patent_client/_sync/uspto/peds/manager_test.py
+-rw-r--r--   0        0        0    17335 2024-04-25 19:50:46.856041 patent_client-5.0.0/patent_client/_sync/uspto/peds/model.py
+-rw-r--r--   0        0        0     6532 2024-04-25 19:50:46.856238 patent_client-5.0.0/patent_client/_sync/uspto/peds/query.py
+-rw-r--r--   0        0        0     4469 2024-04-25 19:50:46.856357 patent_client-5.0.0/patent_client/_sync/uspto/peds/search_index.csv
+-rw-r--r--   0        0        0      565 2024-04-25 19:50:46.856654 patent_client-5.0.0/patent_client/_sync/uspto/ptab/__init__.py
+-rw-r--r--   0        0        0    10579 2024-04-25 19:50:46.856830 patent_client-5.0.0/patent_client/_sync/uspto/ptab/api.py
+-rw-r--r--   0        0        0     1021 2024-04-25 19:50:46.857052 patent_client-5.0.0/patent_client/_sync/uspto/ptab/api_test.py
+-rw-r--r--   0        0        0     1300 2024-04-25 19:50:46.859921 patent_client-5.0.0/patent_client/_sync/uspto/ptab/fixtures/documents_input.json
+-rw-r--r--   0        0        0     1057 2024-04-25 19:50:46.859981 patent_client-5.0.0/patent_client/_sync/uspto/ptab/fixtures/proceeding_input.json
+-rw-r--r--   0        0        0     2467 2024-04-25 19:50:46.860111 patent_client-5.0.0/patent_client/_sync/uspto/ptab/manager.py
+-rw-r--r--   0        0        0     2415 2024-04-25 19:50:46.860301 patent_client-5.0.0/patent_client/_sync/uspto/ptab/manager_test.py
+-rw-r--r--   0        0        0     8521 2024-04-25 19:50:46.860476 patent_client-5.0.0/patent_client/_sync/uspto/ptab/model.py
+-rw-r--r--   0        0        0      658 2024-04-25 19:50:46.860666 patent_client-5.0.0/patent_client/_sync/uspto/ptab/util.py
+-rw-r--r--   0        0        0      577 2024-04-25 19:50:46.860801 patent_client-5.0.0/patent_client/_sync/uspto/public_search/__init__.py
+-rw-r--r--   0        0        0     6951 2024-04-25 19:50:46.860978 patent_client-5.0.0/patent_client/_sync/uspto/public_search/api.py
+-rw-r--r--   0        0        0      682 2024-04-25 19:50:46.861094 patent_client-5.0.0/patent_client/_sync/uspto/public_search/api_test.py
+-rw-r--r--   0        0        0      416 2024-04-25 19:50:46.877927 patent_client-5.0.0/patent_client/_sync/uspto/public_search/convert/__init__.py
+-rw-r--r--   0        0        0     2482 2024-04-25 19:50:46.879710 patent_client-5.0.0/patent_client/_sync/uspto/public_search/convert/biblio.py
+-rw-r--r--   0        0        0     7094 2024-04-25 19:50:46.881142 patent_client-5.0.0/patent_client/_sync/uspto/public_search/convert/document.py
+-rw-r--r--   0        0        0     2010 2024-04-25 19:50:46.881444 patent_client-5.0.0/patent_client/_sync/uspto/public_search/convert/shared.py
+-rw-r--r--   0        0        0     1451 2024-04-25 19:50:46.881652 patent_client-5.0.0/patent_client/_sync/uspto/public_search/convert_test.py
+-rw-r--r--   0        0        0      576 2024-04-25 19:50:46.881727 patent_client-5.0.0/patent_client/_sync/uspto/public_search/count_query.json
+-rw-r--r--   0        0        0   867778 2024-04-25 19:50:46.882601 patent_client-5.0.0/patent_client/_sync/uspto/public_search/fixtures/biblio.json
+-rw-r--r--   0        0        0   270895 2024-04-25 19:50:46.883125 patent_client-5.0.0/patent_client/_sync/uspto/public_search/fixtures/biblio_convert.json
+-rw-r--r--   0        0        0   220128 2024-04-25 19:50:46.883285 patent_client-5.0.0/patent_client/_sync/uspto/public_search/fixtures/biblio_output.json
+-rw-r--r--   0        0        0  2431829 2024-04-25 19:50:46.885243 patent_client-5.0.0/patent_client/_sync/uspto/public_search/fixtures/doc.json
+-rw-r--r--   0        0        0  2225007 2024-04-25 19:50:46.886477 patent_client-5.0.0/patent_client/_sync/uspto/public_search/fixtures/doc_convert.json
+-rw-r--r--   0        0        0  3962033 2024-04-25 19:50:46.888518 patent_client-5.0.0/patent_client/_sync/uspto/public_search/fixtures/doc_output.json
+-rw-r--r--   0        0        0     4487 2024-04-25 19:50:46.889539 patent_client-5.0.0/patent_client/_sync/uspto/public_search/manager.py
+-rw-r--r--   0        0        0     7339 2024-04-25 19:50:46.889731 patent_client-5.0.0/patent_client/_sync/uspto/public_search/manager_test.py
+-rw-r--r--   0        0        0      746 2024-04-25 19:50:46.889860 patent_client-5.0.0/patent_client/_sync/uspto/public_search/model/__init__.py
+-rw-r--r--   0        0        0     3548 2024-04-25 19:50:46.889976 patent_client-5.0.0/patent_client/_sync/uspto/public_search/model/biblio.py
+-rw-r--r--   0        0        0     7978 2024-04-25 19:50:46.890155 patent_client-5.0.0/patent_client/_sync/uspto/public_search/model/document.py
+-rw-r--r--   0        0        0     2665 2024-04-25 19:50:46.890280 patent_client-5.0.0/patent_client/_sync/uspto/public_search/model/shared.py
+-rw-r--r--   0        0        0     1953 2024-04-25 19:50:46.890406 patent_client-5.0.0/patent_client/_sync/uspto/public_search/model_test.py
+-rw-r--r--   0        0        0     4936 2024-04-25 19:50:46.892506 patent_client-5.0.0/patent_client/_sync/uspto/public_search/query.py
+-rw-r--r--   0        0        0     1344 2024-04-25 19:50:46.892581 patent_client-5.0.0/patent_client/_sync/uspto/public_search/query_config.csv
+-rw-r--r--   0        0        0     4729 2024-04-25 19:50:46.894147 patent_client-5.0.0/patent_client/_sync/uspto/public_search/query_test.py
+-rw-r--r--   0        0        0     1049 2024-04-25 19:50:46.894230 patent_client-5.0.0/patent_client/_sync/uspto/public_search/search_query.json
+-rw-r--r--   0        0        0      689 2024-04-25 19:50:46.894466 patent_client-5.0.0/patent_client/_sync/uspto/public_search/util.py
+-rw-r--r--   0        0        0     6043 2024-04-25 19:50:46.896118 patent_client-5.0.0/patent_client/parser.py
+-rw-r--r--   0        0        0      331 2024-04-03 19:26:37.191135 patent_client-5.0.0/patent_client/patches.py
+-rw-r--r--   0        0        0     3272 2024-04-25 19:50:46.897434 patent_client-5.0.0/patent_client/session.py
+-rw-r--r--   0        0        0      685 2024-04-25 19:50:46.897630 patent_client-5.0.0/patent_client/settings.py
+-rw-r--r--   0        0        0     8162 2024-04-03 19:26:37.191401 patent_client-5.0.0/patent_client/test_parser.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:26:37.306255 patent_client-5.0.0/patent_client/util/__init__.py
+-rw-r--r--   0        0        0     1266 2024-04-25 19:50:46.899374 patent_client-5.0.0/patent_client/util/asyncio_util.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:26:37.306393 patent_client-5.0.0/patent_client/util/claims/__init__.py
+-rw-r--r--   0        0        0     4313 2024-04-25 19:37:51.159560 patent_client-5.0.0/patent_client/util/claims/examples/multiple_dependent.json
+-rw-r--r--   0        0        0     2456 2024-04-03 19:26:37.308088 patent_client-5.0.0/patent_client/util/claims/examples/multiple_dependent.txt
+-rw-r--r--   0        0        0     6924 2024-04-25 19:37:51.166864 patent_client-5.0.0/patent_client/util/claims/examples/published_claims.json
+-rw-r--r--   0        0        0     3719 2024-04-03 19:26:37.308219 patent_client-5.0.0/patent_client/util/claims/examples/published_claims.txt
+-rw-r--r--   0        0        0      732 2024-04-03 19:26:37.308282 patent_client-5.0.0/patent_client/util/claims/model.py
+-rw-r--r--   0        0        0     3546 2024-04-25 19:50:46.899557 patent_client-5.0.0/patent_client/util/claims/parser.py
+-rw-r--r--   0        0        0      939 2024-04-25 19:50:46.899709 patent_client-5.0.0/patent_client/util/claims/parser_test.py
+-rw-r--r--   0        0        0      611 2024-04-03 19:26:37.308464 patent_client-5.0.0/patent_client/util/format.py
+-rw-r--r--   0        0        0     9464 2024-04-25 19:50:46.899927 patent_client-5.0.0/patent_client/util/manager.py
+-rw-r--r--   0        0        0     3038 2024-04-25 19:50:46.900084 patent_client-5.0.0/patent_client/util/pydantic_util.py
+-rw-r--r--   0        0        0      861 2024-04-03 19:26:37.308765 patent_client-5.0.0/patent_client/util/request_util.py
+-rw-r--r--   0        0        0     1256 2024-04-25 19:50:46.900223 patent_client-5.0.0/patent_client/util/test.py
+-rw-r--r--   0        0        0       22 2024-04-25 19:50:46.900461 patent_client-5.0.0/patent_client/version.py
+-rw-r--r--   0        0        0     3376 2024-04-25 19:50:46.901426 patent_client-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7701 1970-01-01 00:00:00.000000 patent_client-5.0.0/PKG-INFO
```

### Comparing `patent_client-4.1.9/LICENSE` & `patent_client-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/README.md` & `patent_client-5.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -19,19 +19,29 @@
 - 🚀 **Performance:** Fetched data is retrieved using the [httpx][httpx] library with native HTTP/2 and asyncio support, and cached using the [hishel][hishel] library for super-fast queries, and [yankee][yankee] for data extraction.
 - 🌐 **Async/Await Support:** All API's (optionally!) support the async/await syntax.
 - 🔮 **Pydantic v2 Support:** All models retrieved are [Pydantic v2 models][pydantic] with all the goodness that comes with them!
 
 Docs, including a fulsome Getting Started and User Guide are available on [Read the Docs](http://patent-client.readthedocs.io). The Examples folder includes examples of using `patent_client` for
 many common IP tasks
 
+## ⭐ New in v5 ⭐
+
+Version 5 brings a new and more reliable way to provide synchronous and asynchronous access to the various APIs.
+In version 5, like in version 3, you can just `from patent_client import [Model]` and get a synchronous version
+of the model. No asynchronous methods or functionality at all. Or you can do `from patent_client._async import [Model]`
+and get an asynchronous version of the model.
+
+Version 5 also brings support for the USPTO's new [Open Data Portal](https://beta-data.uspto.gov/home), a system currently in beta that is scheduled to replace the current Patent Examination Data System in late 2024.
+
 ## Coverage
 
 - [United States Patent & Trademark Office][USPTO]
 
   - [Patent Examination Data][PEDS] - Full Support
+  - [Open Data Portal][ODP] - Full Support
   - [Global Dossier][GD] - Full Support
   - [Patent Assignment Data][Assignment] - Lookup Support
   - [Patent Trial & Appeal Board API v2][PTAB] - Supports Proceedings, Decisions, and Documents
   - [Patent Public Search][PPS] - Full Support
   - [Bulk Data Storage System][BDSS] - Full Support
 
 
@@ -53,14 +63,15 @@
 [PPS]:  https://ppubs.uspto.gov/pubwebapp/static/pages/landing.html
 [PEDS]: https://developer.uspto.gov/api-catalog/ped
 [PTAB]: https://developer.uspto.gov/api-catalog/ptab-api-v2
 [USPTO]: http://developer.uspto.gov
 [BDSS]: https://developer.uspto.gov/api-catalog/bdss
 [GD]: https://globaldossier.uspto.gov
 [pydantic]: https://docs.pydantic.dev/latest/
+[ODP]: https://beta-data.uspto.gov/home
 
 
 ## Installation
 
 ```
 pip install patent_client
 ```
@@ -95,17 +106,20 @@
 >>> pub.biblio.title
 'AUTOMATIC FLUID DISPENSER'
 
 ```
 
 ## Async Quick Start
 
-To use the asyncio methods, simply use `async with` for iterators, and call any methods with a `a` prefix:
+To use async with Patent Client, just import the classes you need from the async module. All methods
+and iterators that access data or create a network request are asynchronous.
 
 ```python
+from patent_client._async import USApplication
+
 apps = list()
 async for app in USApplication.objects.filter(first_named_applicant="Google"):
   apps.append(app)
 
 app = await USApplication.objects.aget("16123456")
 
 ```
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/family/fixtures/family_api_output.json` & `patent_client-5.0.0/patent_client/_async/epo/ops/family/fixtures/family_api_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/family/fixtures/family_convert.json` & `patent_client-5.0.0/patent_client/_async/epo/ops/family/fixtures/family_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/family/fixtures/family_input.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/family/fixtures/family_input.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/family/fixtures/family_model_output.json` & `patent_client-5.0.0/patent_client/_async/epo/ops/family/fixtures/family_model_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/family/model.py` & `patent_client-5.0.0/patent_client/_sync/epo/ops/family/model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-from typing import List
-from typing import Optional
+# ********************************************************************************
+# *         WARNING: This file is automatically generated by unasync.py.         *
+# *                             DO NOT MANUALLY EDIT                             *
+# *          Source File: patent_client/_async/epo/ops/family/model.py           *
+# ********************************************************************************
+
+from typing import List, Optional
 
 from pydantic import Field
 
+from ..number_service.model import DocumentId
+from ..util import EpoBaseModel
 from .schema import FamilySchema
-from patent_client.epo.ops.number_service.model import DocumentId
-from patent_client.epo.ops.util import EpoBaseModel
 
 
 class PriorityClaim(EpoBaseModel):
     application_number: Optional[str] = None
     application_reference: Optional[DocumentId] = None
     sequence: Optional[int] = None
     kind: Optional[str] = None
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/family/model_test.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/family/model_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 import json
 from pathlib import Path
 
 import pytest
 
-from .model import Family
 from patent_client.util.test import compare_dicts
 
-fixtures = Path(__file__).parent / "fixtures"
-
+from .model import Family
 
-def test_model():
-    result = Family.objects.get("EP1000000A1")
-    expected_file = fixtures / "family_model_output.json"
-    # expected_file.write_text(result.model_dump_json(indent=2))
-    expected = json.loads(expected_file.read_text())
-    compare_dicts(json.loads(result.model_dump_json()), expected)
+fixtures = Path(__file__).parent / "fixtures"
 
 
 @pytest.mark.asyncio
-async def test_async_model():
-    result = await Family.objects.aget("EP1000000A1")
+async def test_model():
+    result = await Family.objects.get("EP1000000A1")
     expected_file = fixtures / "family_model_output.json"
     # expected_file.write_text(result.model_dump_json(indent=2))
     expected = json.loads(expected_file.read_text())
     compare_dicts(json.loads(result.model_dump_json()), expected)
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/family/schema.py` & `patent_client-5.0.0/patent_client/_sync/epo/ops/family/schema.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,47 @@
+# ********************************************************************************
+# *         WARNING: This file is automatically generated by unasync.py.         *
+# *                             DO NOT MANUALLY EDIT                             *
+# *          Source File: patent_client/_async/epo/ops/family/schema.py          *
+# ********************************************************************************
+
 from yankee.xml import fields as f
-from yankee.xml.schema import fields as f
 
-from patent_client.epo.ops.number_service.schema import DocumentIdSchema
-from patent_client.epo.ops.published.schema.biblio import DocDbNumberField
-from patent_client.epo.ops.util import Schema
+from ..number_service.schema import DocumentIdSchema
+from ..published.schema.biblio import DocDbNumberField
+from ..util import Schema
 
 
 class PriorityClaimSchema(Schema):
     application_number = DocDbNumberField(".//epo:document-id")
     application_reference = DocumentIdSchema(".//epo:document-id")
     sequence = f.Int("./@sequence")
     kind = f.Str("./@kind")
     active = f.Bool(".//epo:priority-active-indicator", true_value="YES")
 
 
 class FamilyMemberSchema(Schema):
-    publication_number = DocDbNumberField('.//epo:publication-reference/epo:document-id[@document-id-type="docdb"]')
-    application_number = DocDbNumberField('.//epo:application-reference/epo:document-id[@document-id-type="docdb"]')
+    publication_number = DocDbNumberField(
+        './/epo:publication-reference/epo:document-id[@document-id-type="docdb"]'
+    )
+    application_number = DocDbNumberField(
+        './/epo:application-reference/epo:document-id[@document-id-type="docdb"]'
+    )
     family_id = f.Str("./@family-id")
-    publication_reference = f.List(DocumentIdSchema, ".//epo:publication-reference/epo:document-id")
-    application_reference = f.List(DocumentIdSchema, ".//epo:application-reference/epo:document-id")
+    publication_reference = f.List(
+        DocumentIdSchema, ".//epo:publication-reference/epo:document-id"
+    )
+    application_reference = f.List(
+        DocumentIdSchema, ".//epo:application-reference/epo:document-id"
+    )
     priority_claims = f.List(PriorityClaimSchema, ".//epo:priority-claim")
 
 
 class FamilySchema(Schema):
-    publication_reference = DocumentIdSchema(".//ops:patent-family/ops:publication-reference")
+    publication_reference = DocumentIdSchema(
+        ".//ops:patent-family/ops:publication-reference"
+    )
     num_records = f.Int(".//ops:patent-family/@total-result-count")
     publication_number = DocDbNumberField(
         './/ops:patent-family/ops:publication-reference/epo:document-id[@document-id-type="docdb"]'
     )
     family_members = f.List(FamilyMemberSchema, ".//ops:family-member")
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/family/schema_test.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/family/schema_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 from pathlib import Path
 
 import lxml.etree as ET
 
-from .schema import FamilySchema
 from patent_client.util.test import compare_dicts
 
+from .schema import FamilySchema
+
 fixtures = Path(__file__).parent / "fixtures"
 
 
 def test_example():
     tree = ET.parse(fixtures / "family_input.xml")
     result = FamilySchema().load(tree)
     expected_file = fixtures / "family_convert.json"
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/legal/fixtures/example_1.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/legal/fixtures/example_1_convert.json` & `patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_1_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/legal/fixtures/example_2.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/legal/fixtures/example_2_convert.json` & `patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_2_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/legal/fixtures/example_3.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/legal/fixtures/example_3_convert.json` & `patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_3_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/legal/legal_code_descriptions_2023-44-0.xlsx` & `patent_client-5.0.0/patent_client/_sync/epo/ops/legal/legal_code_descriptions_2023-44-0.xlsx`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/legal/model.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/legal/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Optional
 
 from pydantic import Field
 
-from .schema import LegalSchema
-from patent_client.epo.ops.number_service.model import DocumentId
-from patent_client.epo.ops.util import EpoBaseModel
 from patent_client.util.pydantic_util import Date
 
+from ..number_service.model import DocumentId
+from ..util import EpoBaseModel
+from .schema import LegalSchema
+
 
 class MetaData(EpoBaseModel):
     status_of_data: Optional[str] = None
     docdb_publication_number: Optional[str] = None
     subscriber_exchange_date: Optional[Date] = None
     epo_created_date: Optional[Date] = None
     docdb_integer: Optional[int] = None
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/legal/national_codes.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/legal/national_codes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+import asyncio
 import datetime
 import logging
 import re
 import sqlite3
 from pathlib import Path
 
 import lxml.etree as ET
 from openpyxl import load_workbook
 
 from patent_client import BASE_DIR
-from patent_client.session import PatentClientSession
-from patent_client.util.asyncio_util import run_sync
+from patent_client._async.http_client import PatentClientSession
 
 session = PatentClientSession()
 
 legal_code_dir = BASE_DIR / "epo"
 legal_code_dir.mkdir(exist_ok=True, parents=True)
 db_location = legal_code_dir / "legal_codes.sqlite"
 
@@ -21,62 +21,81 @@
 logger = logging.getLogger(__name__)
 
 
 def current_date():
     return datetime.datetime.now().date()
 
 
-def generate_legal_code_db():
-    current = has_current_spreadsheet()
+code_database_current = False
+
+
+async def generate_legal_code_db():
+    current = await has_current_spreadsheet()
     if current:
         logger.info("Legal Code Database is Current - skipping database creation")
         return
     else:
         try:
-            logger.info("Legal Code Database is out of date - creating legal code database")
-            path = get_spreadsheet()
+            logger.info(
+                "Legal Code Database is out of date - creating legal code database"
+            )
+            path = await get_spreadsheet()
         except Exception:
-            logger.exception("Could not find live code file - falling back to default dated 2023-11-05")
-            path = Path(__file__).parent / "legal_code_descriptions_2023-44-0.xlsx"
+            logger.exception(
+                "Could not find live code file - falling back to default dated 2023-11-05"
+            )
+            path = (
+                Path(__file__).parent
+                / "fixtures"
+                / "legal_code_descriptions_202417.xlsx"
+            )
         create_code_database(path)
 
 
-def has_current_spreadsheet():
+async def has_current_spreadsheet():
     con = sqlite3.connect(db_location, timeout=30)
     cur = con.cursor()
     try:
         fname = cur.execute("SELECT * FROM meta").fetchone()[0]
-        date_string = re.search(r"legal_code_descriptions_([\d-]+)\.xlsx", fname).group(1)
+        date_string = re.search(r"legal_code_descriptions_([\d-]+)\.xlsx", fname).group(
+            1
+        )
         try:
             date = datetime.datetime.strptime(date_string, "%Y-%W-%w").date()
-        except ValueError:  # Indicates using an older format and database needs to be updated
+        except (
+            ValueError
+        ):  # Indicates using an older format and database needs to be updated
             return False
         age = datetime.datetime.now().date() - date
         logger.debug(f"Legal Code Database is {age} days old")
         return age.days < 7
     except (sqlite3.OperationalError, TypeError):
         return False
 
 
-def get_spreadsheet_from_epo_website() -> tuple[datetime.date, str]:
+async def get_spreadsheet_from_epo_website() -> tuple[datetime.date, str]:
     url = "https://www.epo.org/searching-for-patents/data/coverage/weekly.html"
-    response = run_sync(session.get(url))
+    response = await session.get(url)
     response.raise_for_status()
     tree = ET.HTML(response.text)
-    date_string = tree.xpath(".//tr/td[contains(text(), 'Legal event codes')]/../td[4]")[0].text.strip()
+    date_string = tree.xpath(
+        ".//tr/td[contains(text(), 'Legal event codes')]/../td[4]"
+    )[0].text.strip()
     week, year = date_string.split()[1].split("/")
     date = datetime.datetime.strptime(f"{year}-{week}-0", "%Y-%W-%w").date()
     excel_url = tree.xpath('.//a[contains(@href, "Legal-event-codes")][1]/@href')[0]
     logger.info(f"Found new spreadsheet for {date.isoformat()}: {excel_url}")
     return (date, excel_url)
 
 
-def get_spreadsheet() -> tuple[datetime.date, Path]:
-    date, excel_url = get_spreadsheet_from_epo_website()
-    out_path = legal_code_dir / f"legal_code_descriptions_{date.strftime('%Y-%W-%w')}.xlsx"
+async def get_spreadsheet() -> tuple[datetime.date, Path]:
+    date, excel_url = await get_spreadsheet_from_epo_website()
+    out_path = (
+        legal_code_dir / f"legal_code_descriptions_{date.strftime('%Y-%W-%w')}.xlsx"
+    )
     if out_path.exists():
         logger.info(f"File already downloaded! Current as of {date.isoformat()}")
         return out_path
     out_path = session.download(excel_url, path=out_path)
     logger.info(f"Downloaded new live code file for date {date.isoformat()}")
     return out_path
 
@@ -91,36 +110,48 @@
             return
     except (sqlite3.OperationalError, TypeError):
         pass
 
     cur.execute("CREATE TABLE IF NOT EXISTS meta (file_name text)")
     cur.execute("INSERT INTO meta values (?)", (excel_path.name,))
     wb = load_workbook(excel_path)
-    data = list(tuple(i.strip() for i in r) for r in wb[wb.sheetnames[0]].iter_rows(values_only=True))
+    data = list(
+        tuple(i.strip() for i in r)
+        for r in wb[wb.sheetnames[0]].iter_rows(values_only=True)
+    )
     rows = data[1:]
     cur.execute(
         """CREATE TABLE IF NOT EXISTS legal_codes (
     country_code text,
     event_code text,
     date_created text,
     influence text,
     description text,
     last_update text,
     description_orig text,
     last_update_orig text,
     event_class text,
     event_class_description text)"""
     )
-    cur.execute("""CREATE INDEX IF NOT EXISTS country_event_code ON legal_codes (country_code, event_code)""")
-    cur.executemany("INSERT INTO legal_codes values (?, ?, ?, ?, ?, ?, ?, ?, ?, ?)", rows)
+    cur.execute(
+        """CREATE INDEX IF NOT EXISTS country_event_code ON legal_codes (country_code, event_code)"""
+    )
+    cur.executemany(
+        "INSERT INTO legal_codes values (?, ?, ?, ?, ?, ?, ?, ?, ?, ?)", rows
+    )
     con.commit()
 
 
 class LegalCodes:
     def __init__(self):
+        if not code_database_current:
+            logger.info(
+                "Legal Code Database is out of date - creating legal code database. Note this only happens once!"
+            )
+            asyncio.run(generate_legal_code_db())
         self.connection = sqlite3.connect(db_location, timeout=30)
         self.connection.row_factory = sqlite3.Row
 
     def get_code_data(self, country_code, legal_code):
         cur = self.connection.cursor()
         try:
             return dict(
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/legal/schema.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/legal/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import *
+from typing import Dict
 
 from yankee.util import clean_whitespace
 from yankee.xml import fields as f
 
+from ..number_service.schema import DocumentIdSchema
+from ..util import Schema
 from .national_codes import LegalCodes
-from patent_client.epo.ops.number_service.schema import DocumentIdSchema
-from patent_client.epo.ops.util import Schema
 
 code_db = LegalCodes()
 
 
 def ip_type_formatter(string):
     types = {
         "PI": "Patent of Invention",
@@ -99,19 +99,23 @@
     extension_states = f.Str(".//ops:L524EP", formatter=lambda x: x.split(" "))
     effective_date = f.Date(".//ops:L525EP")
     date_of_withdrawal = f.Str(".//ops:L526EP")
 
     def deserialize(self, obj) -> "Dict":
         obj = super().deserialize(obj)
         if obj.event_code == "REG":
-            code_data = code_db.get_code_data(obj.event_country, obj.regional_event_code)
+            code_data = code_db.get_code_data(
+                obj.event_country, obj.regional_event_code
+            )
             obj["event_code"] = obj.event_country + "." + obj.regional_event_code
         else:
             code_data = code_db.get_code_data(obj.country_code, obj.event_code)
             obj["event_code"] = obj.country_code + "." + obj.event_code
         obj["event_description"] = code_data["description"]
         return obj
 
 
 class LegalSchema(Schema):
-    publication_reference = DocumentIdSchema(".//ops:patent-family/ops:publication-reference")
+    publication_reference = DocumentIdSchema(
+        ".//ops:patent-family/ops:publication-reference"
+    )
     events = f.List(LegalEventSchema, ".//ops:legal")
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/legal/schema_test.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/legal/schema_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 from pathlib import Path
 
 import lxml.etree as ET
 
-from .schema import LegalSchema
 from patent_client.util.test import compare_dicts
 
+from .schema import LegalSchema
+
 fixture_dir = Path(__file__).parent / "fixtures"
 
 
 def test_example_1():
     tree = ET.parse(fixture_dir / "example_1.xml")
     result = LegalSchema().load(tree)
     expected_file = fixture_dir / "example_1_convert.json"
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/number_service/api.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/number_service/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+from ..session import asession
 from .model import NumberServiceResult
-from patent_client.epo.ops.session import asession
 
 
 class NumberServiceException(Exception):
     pass
 
 
 class NumberServiceApi:
     @classmethod
     async def convert_number(
-        cls, number, doc_type="publication", input_format="original", output_format="docdb"
+        cls,
+        number,
+        doc_type="publication",
+        input_format="original",
+        output_format="docdb",
     ) -> NumberServiceResult:
         """Number Conversion Service
         number: number to convert. Must include at least country and doc number,
             can optionally include kind code or publication date. e.g.
             MD.20050130
             MD.20050130.A
             MD.20050130.A.20050130
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/number_service/api_test.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/number_service/api_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 from .api import NumberServiceApi
 
 
 class TestNumberServiceApi:
     @pytest.mark.asyncio
     async def test_docdb_to_epodoc(self):
-        actual = await NumberServiceApi.convert_number("MD.20050130.A.20050130", "application", "docdb", "epodoc")
+        actual = await NumberServiceApi.convert_number(
+            "MD.20050130.A.20050130", "application", "docdb", "epodoc"
+        )
         assert not actual.messages
         assert actual.input_doc.id_type == "docdb"
         assert actual.output_doc.id_type == "epodoc"
 
     @pytest.mark.asyncio
     async def test_original_to_docdb(self):
         actual = await NumberServiceApi.convert_number(
@@ -18,15 +20,17 @@
         )
         assert not actual.messages
         assert actual.input_doc.id_type == "original"
         assert actual.output_doc.id_type == "docdb"
 
     @pytest.mark.asyncio
     async def test_docdb_to_original(self):
-        actual = await NumberServiceApi.convert_number("JP.2006147056.A.20060526", "application", "docdb", "original")
+        actual = await NumberServiceApi.convert_number(
+            "JP.2006147056.A.20060526", "application", "docdb", "original"
+        )
         assert not actual.messages
         assert actual.input_doc.id_type == "docdb"
         assert actual.output_doc.id_type == "original"
 
     @pytest.mark.asyncio
     async def test_original_to_epodoc(self):
         actual = await NumberServiceApi.convert_number(
@@ -34,10 +38,12 @@
         )
         assert not actual.messages
         assert actual.input_doc.id_type == "original"
         assert actual.output_doc.id_type == "epodoc"
 
     @pytest.mark.asyncio
     async def test_original_to_docdb_pct(self):
-        actual = await NumberServiceApi.convert_number("PCT/GB02/04635.20021011", "application", "original", "docdb")
+        actual = await NumberServiceApi.convert_number(
+            "PCT/GB02/04635.20021011", "application", "original", "docdb"
+        )
         assert actual.input_doc.id_type == "original"
         assert actual.output_doc.id_type == "docdb"
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/number_service/errors.py` & `patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+# ********************************************************************************
+# *         WARNING: This file is automatically generated by unasync.py.         *
+# *                             DO NOT MANUALLY EDIT                             *
+# *      Source File: patent_client/_async/epo/ops/number_service/errors.py      *
+# ********************************************************************************
+
 import re
-from dataclasses import asdict
-from dataclasses import dataclass
+from dataclasses import asdict, dataclass
 from pathlib import Path
 
 base_dir = Path(__file__).parent
 
 
 @dataclass
 class NumberServiceError:
@@ -27,15 +32,14 @@
 
 def get_messages(string):
     match = message_re.search(string)
     return match.groupdict() if match else None
 
 
 def build_error_dir():
-
     error_text = (base_dir / "errors.txt").read_text()
     errors = [get_errors(err) for err in error_text.split("\n")]
     message_text = (base_dir / "messages.txt").read_text()
     messages = [get_messages(err) for err in message_text.split("\n")]
     error_objs = [NumberServiceError(**e) for e in errors + messages if e]
     errors = {e.code: asdict(e) for e in error_objs if e}
     errors["SUCCESS"] = None
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/number_service/errors.txt` & `patent_client-5.0.0/patent_client/_async/epo/ops/number_service/errors.txt`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/number_service/messages.txt` & `patent_client-5.0.0/patent_client/_async/epo/ops/number_service/messages.txt`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/number_service/model.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/number_service/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Optional
 
 from pydantic import Field
 
-from .schema import NumberServiceResultSchema
-from patent_client.epo.ops.util import EpoBaseModel
 from patent_client.util.pydantic_util import Date
 
+from ..util import EpoBaseModel
+from .schema import NumberServiceResultSchema
+
 
 class DocumentId(EpoBaseModel):
     doc_type: Optional[str] = None
     id_type: Optional[str] = None
     country: Optional[str] = None
     number: Optional[str] = None
     kind: Optional[str] = None
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/number_service/schema.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/number_service/schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from yankee.xml import fields as f
 
+from ..util import Schema
 from . import error_dir
-from patent_client.epo.ops.util import Schema
 
 
 class TagField(f.Field):
     def deserialize(self, obj):
         obj = super().deserialize(obj)
         if obj is None:
             return None
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/api.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import logging
 from io import BytesIO
 
 from yankee.data import AttrDict
 
+from ..session import asession
 from .model.biblio import BiblioResult
-from .model.fulltext import Claims
-from .model.fulltext import Description
+from .model.fulltext import Claims, Description
 from .model.images import Images
 from .model.search import Search
-from patent_client.epo.ops.session import asession
 
 logger = logging.getLogger(__name__)
 
 
 class PublishedBiblioAsyncApi:
     @classmethod
-    async def get_constituents(cls, number, doc_type="publication", format="docdb", constituents=("biblio",)):
+    async def get_constituents(
+        cls, number, doc_type="publication", format="docdb", constituents=("biblio",)
+    ):
         """Published Data Constituents API
         number: document number to search
         doc_type: document type (application / publication)
         format: document number format (original / docdb / epodoc)
         constituents: what data to retrieve. Can be combined. (biblio / abstract / full-cycle)
 
         """
@@ -27,34 +28,44 @@
         if isinstance(constituents, str):
             constituents = (constituents,)
         url = base_url + ",".join(constituents)
         response = await asession.get(url)
         return response.text
 
     @classmethod
-    async def get_biblio(cls, number, doc_type="publication", format="docdb") -> "BiblioResult":
-        text = await cls.get_constituents(number, doc_type, format, constituents="biblio")
+    async def get_biblio(
+        cls, number, doc_type="publication", format="docdb"
+    ) -> "BiblioResult":
+        text = await cls.get_constituents(
+            number, doc_type, format, constituents="biblio"
+        )
         return BiblioResult.model_validate(text)
 
     @classmethod
     async def get_abstract(cls, number, doc_type="publication", format="docdb"):
-        return await cls.get_constituents(number, doc_type, format, constituents="abstract")
+        return await cls.get_constituents(
+            number, doc_type, format, constituents="abstract"
+        )
 
     @classmethod
     async def get_full_cycle(cls, number, doc_type="publication", format="docdb"):
-        return await cls.get_constituents(number, doc_type, format, constituents="full-cycle")
+        return await cls.get_constituents(
+            number, doc_type, format, constituents="full-cycle"
+        )
 
 
 class PublishedFulltextAsyncApi:
     fulltext_jurisdictions = "EP, WO, AT, BE, BG, CA, CH, CY, CZ, DK, EE, ES, FR, GB, GR, HR, IE, IT, LT, LU, MC, MD, ME, NO, PL, PT, RO, RS, SE, SK".split(
         ", "
     )
 
     @classmethod
-    async def get_fulltext_result(cls, number, doc_type="publication", format="docdb", inquiry="fulltext"):
+    async def get_fulltext_result(
+        cls, number, doc_type="publication", format="docdb", inquiry="fulltext"
+    ):
         """Published Fulltext API
         number: document number to search
         doc_type: document type (application / publication)
         format: document number format (original / docdb / epodoc)
         inquiry: what data to retrieve. Can be combined. (fulltext / description / claims)
 
         """
@@ -65,20 +76,26 @@
             )
         response = await asession.get(url)
         response.raise_for_status
         return response.text
 
     @classmethod
     async def get_description(cls, number, doc_type="publication", format="docdb"):
-        text = await cls.get_fulltext_result(number, doc_type="publication", format="docdb", inquiry="description")
+        text = await cls.get_fulltext_result(
+            number, doc_type="publication", format="docdb", inquiry="description"
+        )
         return Description.model_validate(text)
 
     @classmethod
-    async def get_claims(cls, number, doc_type="publication", format="docdb") -> "Claims":
-        text = await cls.get_fulltext_result(number, doc_type="publication", format="docdb", inquiry="claims")
+    async def get_claims(
+        cls, number, doc_type="publication", format="docdb"
+    ) -> "Claims":
+        text = await cls.get_fulltext_result(
+            number, doc_type="publication", format="docdb", inquiry="claims"
+        )
         return Claims.model_validate(text)
 
 
 class PublishedSearchAsyncApi:
     @classmethod
     async def search(cls, query, start=1, end=100):
         base_url = "http://ops.epo.org/3.2/rest-services/published-data/search"
@@ -103,15 +120,17 @@
     @classmethod
     async def get_images(cls, number, doc_type="publication", format="docdb"):
         base_url = f"http://ops.epo.org/3.2/rest-services/published-data/{doc_type}/{format}/{number}/images"
         response = await asession.get(base_url)
         return Images.model_validate(response.text)
 
     @classmethod
-    async def get_page_image(cls, country, number, kind, image_type, page_number, image_format="pdf"):
+    async def get_page_image(
+        cls, country, number, kind, image_type, page_number, image_format="pdf"
+    ):
         response = await asession.get(
             f"https://ops.epo.org/3.2/rest-services/published-data/images/{country}/{number}/{kind}/{image_type}.{image_format}",
             params={"Range": page_number},
             stream=True,
             extensions={"force_cache": True},
         )
         return BytesIO(response.raw.read())
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/api_test.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/api_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,32 +7,38 @@
 
 fixture_dir = Path(__file__).parent / "fixtures"
 
 
 class TestPublishedBiblioAsyncApi:
     @pytest.mark.asyncio
     async def test_doc_example_biblio(self):
-        result = await PublishedAsyncApi.biblio.get_biblio("EP1000000.A1", format="epodoc")
+        result = await PublishedAsyncApi.biblio.get_biblio(
+            "EP1000000.A1", format="epodoc"
+        )
         expected_file = fixture_dir / "ep1000000_biblio_result.json"
         expected_file.write_text(result.model_dump_json(indent=2))
         expected = json.loads(expected_file.read_text())
         actual = json.loads(result.model_dump_json())
         assert actual == expected
 
     @pytest.mark.asyncio
     async def test_doc_example_full_cycle(self):
-        result = await PublishedAsyncApi.biblio.get_full_cycle("EP1000000.A1", format="epodoc")
+        result = await PublishedAsyncApi.biblio.get_full_cycle(
+            "EP1000000.A1", format="epodoc"
+        )
         expected_file = fixture_dir / "ep1000000_full_cycle_result.xml"
-        # expected_file.write_text(result, encoding="utf8")
+        expected_file.write_text(result, encoding="utf8")
         expected = expected_file.read_text(encoding="utf8")
         assert result == expected
 
     @pytest.mark.asyncio
     async def test_doc_example_abstract(self):
-        result = await PublishedAsyncApi.biblio.get_abstract("EP1000000.A1", format="epodoc")
+        result = await PublishedAsyncApi.biblio.get_abstract(
+            "EP1000000.A1", format="epodoc"
+        )
         expected_file = fixture_dir / "ep1000000_abstract_result.xml"
         # expected_file.write_text(result, encoding="utf8")
         expected = expected_file.read_text(encoding="utf8")
         assert result == expected
 
 
 class TestSearchApi:
@@ -45,22 +51,26 @@
         actual = json.loads(result.model_dump_json())
         assert actual == expected
 
 
 class TestFullTextAsyncApi:
     @pytest.mark.asyncio
     async def test_description(self):
-        result = await PublishedAsyncApi.fulltext.get_description("EP1000000.A1", format="epodoc")
+        result = await PublishedAsyncApi.fulltext.get_description(
+            "EP1000000.A1", format="epodoc"
+        )
         expected_file = fixture_dir / "ep1000000_description_result.xml"
         # expected_file.write_text(result.model_dump_json(indent=2))
         expected = json.loads(expected_file.read_text())
         actual = json.loads(result.model_dump_json())
         assert actual == expected
 
     @pytest.mark.asyncio
     async def test_claims(self):
-        result = await PublishedAsyncApi.fulltext.get_claims("EP1000000.A1", format="epodoc")
+        result = await PublishedAsyncApi.fulltext.get_claims(
+            "EP1000000.A1", format="epodoc"
+        )
         expected_file = fixture_dir / "ep1000000_claims_result.json"
         # expected_file.write_text(result.model_dump_json(indent=2))
         expected = json.loads(expected_file.read_text())
         actual = json.loads(result.model_dump_json())
         assert actual == expected
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/cql.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/cql.py`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/fixtures/ep1000000_abstract_result.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/fixtures/ep1000000_biblio_result.json` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/ep1000000_biblio_result.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/fixtures/ep1000000_claims_result.json` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/ep1000000_claims_result.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/fixtures/ep1000000_description_result.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/fixtures/search_result.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/search_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/manager.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import math
 
+from patent_client.util.manager import AsyncManager
+
 from .api import PublishedAsyncApi
 from .cql import generate_query
 from .model.biblio import BiblioResult
-from .model.fulltext import Claims
-from .model.fulltext import Description
+from .model.fulltext import Claims, Description
 from .model.images import ImageDocument
-from patent_client.util.manager import Manager
 
 
 def get_ranges(limit=None, offset=0, page_size=100):
     offset = offset or 0
     offset += 1
     if not limit:
         page_no = 0
@@ -25,70 +25,71 @@
             start = i * page_size + offset
             yield (start, start + page_size - 1)
         if last_page_size:
             start = num_full_pages * page_size + offset
             yield (start, start + last_page_size - 1)
 
 
-class SearchManager(Manager["BiblioResult"]):
+class SearchManager(AsyncManager["BiblioResult"]):
     result_size = 100
     primary_key = "publication"
 
-    async def _aget_search_results_range(self, start=1, end=100):
+    async def _get_search_results_range(self, start=1, end=100):
         if "cql_query" in self.config.filter:
             query = self.config.filter["cql_query"]
         else:
             query = generate_query(**self.config.filter)
         return await PublishedAsyncApi.search.search(query, start, end)
 
-    async def alen(self) -> int:
-        page = await self._aget_search_results_range(1, 100)
+    async def count(self) -> int:
+        page = await self._get_search_results_range(1, 100)
         offset = self.config.offset or 0
         limit = self.config.limit or page.num_results - offset
         num_results = page.num_results
         num_results -= offset
         num_results = min(limit, num_results)
         return num_results
 
-    async def _aget_results(self):
-
-        for start, end in get_ranges(self.config.limit, self.config.offset, self.result_size):
-            page = await self._aget_search_results_range(start, end)
+    async def _get_results(self):
+        for start, end in get_ranges(
+            self.config.limit, self.config.offset, self.result_size
+        ):
+            page = await self._get_search_results_range(start, end)
             for result in page.results:
                 yield result
             if len(page.results) < self.result_size:
                 break
 
-    async def aget(self, number, doc_type="publication", format="docdb") -> BiblioResult:
+    async def get(self, number, doc_type="publication", format="docdb") -> BiblioResult:
         result = await PublishedAsyncApi.biblio.get_biblio(number, doc_type, format)
         if len(result.documents) > 1:
             raise Exception("More than one result found! Try another query")
         return result.documents[0]
 
 
-class BiblioManager(Manager):
-    async def aget(self, doc_number) -> "BiblioResult":
+class BiblioManager(AsyncManager):
+    async def get(self, doc_number) -> "BiblioResult":
         result = await PublishedAsyncApi.biblio.get_biblio(doc_number)
         if len(result.documents) > 1:
             raise ValueError(f"More than one result found for {doc_number}!")
         return result.documents[0]
 
 
-class ClaimsManager(Manager):
-    async def aget(self, doc_number) -> "Claims":
+class ClaimsManager(AsyncManager):
+    async def get(self, doc_number) -> "Claims":
         return await PublishedAsyncApi.fulltext.get_claims(doc_number)
 
 
-class DescriptionManager(Manager):
-    async def aget(self, doc_number) -> Description:
+class DescriptionManager(AsyncManager):
+    async def get(self, doc_number) -> Description:
         return await PublishedAsyncApi.fulltext.get_description(doc_number)
 
 
-class ImagesManager(Manager):
-    async def aget(self, doc_number) -> ImageDocument:
+class ImagesManager(AsyncManager):
+    async def get(self, doc_number) -> ImageDocument:
         return await PublishedAsyncApi.images.get_images(doc_number)
 
 
 class InpadocManager(SearchManager):
     pass
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/manager_test.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/manager_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,64 @@
 import pytest
 
 from .model.search import Inpadoc
 
 
 class TestPublished:
-    def test_inpadoc_manager(self):
-        result = Inpadoc.objects.filter(applicant="Microsoft")
-        assert len(result) > 20
-        countries = list(result.limit(20).values_list("country", flat=True))
-        assert sum(1 for c in countries if c == "US") >= 1
-
-    def test_get_biblio_from_result(self):
-        doc = Inpadoc.objects.filter(applicant="Google").first()
-        result = doc.biblio
-        assert len(result.titles) > 0
-
-    def test_get_claims_from_result(self):
-        result = Inpadoc.objects.get("WO2009085664A2")
-        assert len(result.claims.claims) == 20
-        assert len(result.claims.claim_text) == 4830
-
-    def test_get_description_from_result(self):
-        result = Inpadoc.objects.get("WO2009085664A2")
-        assert len(result.description) == 47955
-
-    def test_get_family_from_result(self):
-        result = Inpadoc.objects.get("WO2009085664A2")
-        assert len(result.family) >= 20
-
-    def test_get_biblio_from_wo(self):
-        result = Inpadoc.objects.get("WO2009085664A2").biblio
-        assert result.abstract is not None
-
-    def test_can_index_inpadoc_result(self):
-        result = Inpadoc.objects.filter(applicant="Tesla")
-        first_obj = result[0]
-        second_obj = result[1]
-        assert first_obj != second_obj
-
-    def test_can_handle_single_item_ipc_classes(self):
-        result = Inpadoc.objects.get("WO2020081771").biblio
-        assert result.intl_class is not None
-
-    def test_issue_41(self):
-        result = Inpadoc.objects.get("JP2005533465A").biblio
-        assert result.title == None
-
-
-class TestPublishedAsync:
     @pytest.mark.asyncio
     async def test_inpadoc_manager(self):
         result = Inpadoc.objects.filter(applicant="Microsoft")
-        assert await result.alen() > 20
-        countries = await result.limit(20).values_list("country", flat=True).ato_list()
+        assert await result.count() > 20
+        countries = [
+            c async for c in result.limit(20).values_list("country", flat=True)
+        ]
         assert sum(1 for c in countries if c == "US") >= 1
 
     @pytest.mark.asyncio
     async def test_get_biblio_from_result(self):
-        doc = await Inpadoc.objects.filter(applicant="Google").afirst()
-        result = doc.biblio
+        doc = await Inpadoc.objects.filter(applicant="Google").first()
+        result = await doc.biblio
         assert len(result.titles) > 0
 
     @pytest.mark.asyncio
     async def test_get_claims_from_result(self):
-        result = await Inpadoc.objects.aget("WO2009085664A2")
-        assert len(result.claims.claims) == 20
-        assert len(result.claims.claim_text) == 4830
+        result = await Inpadoc.objects.get("WO2009085664A2")
+        claims = await result.claims
+        assert len(claims.claims) == 20
+        assert len(claims.claim_text) == 4830
 
     @pytest.mark.asyncio
     async def test_get_description_from_result(self):
-        result = await Inpadoc.objects.aget("WO2009085664A2")
-        assert len(result.description) == 47955
+        result = await Inpadoc.objects.get("WO2009085664A2")
+        description = await result.description
+        assert len(description) == 47955
 
     @pytest.mark.asyncio
     async def test_get_family_from_result(self):
-        result = await Inpadoc.objects.aget("WO2009085664A2")
-        assert len(result.family) >= 20
+        result = await Inpadoc.objects.get("WO2009085664A2")
+        family = await result.family
+        assert len(family) >= 20
 
     @pytest.mark.asyncio
     async def test_get_biblio_from_wo(self):
-        result = await Inpadoc.objects.aget("WO2009085664A2")
-        assert result.biblio.abstract is not None
+        result = await Inpadoc.objects.get("WO2009085664A2")
+        biblio = await result.biblio
+        assert biblio.abstract is not None
 
     @pytest.mark.asyncio
     async def test_can_index_inpadoc_result(self):
         result = Inpadoc.objects.filter(applicant="Tesla")
-        first = await result.afirst()
-        second = await result.offset(1).afirst()
+        first = await result.first()
+        second = await result.offset(1).first()
         assert first != second
 
     @pytest.mark.asyncio
     async def test_can_handle_single_item_ipc_classes(self):
-        result = await Inpadoc.objects.aget("WO2020081771")
-        assert result.biblio.intl_class is not None
+        result = await Inpadoc.objects.get("WO2020081771")
+        biblio = await result.biblio
+        assert biblio.intl_class is not None
 
     @pytest.mark.asyncio
     async def test_issue_41(self):
-        result = await Inpadoc.objects.aget("JP2005533465A")
-        assert result.biblio.title == None
+        result = await Inpadoc.objects.get("JP2005533465A")
+        biblio = await result.biblio
+        assert biblio.title is None
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/model/biblio.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/model/biblio.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-from typing import List
-from typing import Optional
+from typing import List, Optional
 
-from pydantic import computed_field
-from pydantic import Field
+from pydantic import Field, computed_field
 
+from ...number_service.model import DocumentId
+from ...util import EpoBaseModel, InpadocModel
 from ..schema.biblio import BiblioResultSchema
-from patent_client.epo.ops.number_service.model import DocumentId
-from patent_client.epo.ops.util import EpoBaseModel
-from patent_client.epo.ops.util import InpadocModel
 
 
 class Citation(InpadocModel):
     cited_phase: Optional[str] = None
     cited_by: Optional[str] = None
     epodoc: Optional[DocumentId] = None
     docdb: Optional[DocumentId] = None
@@ -41,15 +38,15 @@
     if len(string) < limit:
         return string
     else:
         return f"{string[:limit]}..."
 
 
 class InpadocBiblio(InpadocModel):
-    __manager__ = "patent_client.epo.ops.published.manager.BiblioManager"
+    __manager__ = "...published.manager.BiblioManager"
     country: Optional[str] = None
     doc_number: Optional[str] = None
     kind: Optional[str] = None
     family_id: Optional[str] = None
     publication_number: Optional[str] = None
     application_number: Optional[str] = None
     publication_reference_docdb: Optional[DocumentId] = None
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/model/fulltext.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/model/fulltext.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from typing import List
-from typing import Optional
+from typing import List, Optional
 
 from pydantic import Field
 
-from ..schema.fulltext import ClaimsSchema
-from ..schema.fulltext import DescriptionSchema
-from patent_client.epo.ops.util import EpoBaseModel
 from patent_client.util.claims.model import Claim
 
+from ...util import EpoBaseModel
+from ..schema.fulltext import ClaimsSchema, DescriptionSchema
+
 
 class FTDocumentId(EpoBaseModel):
     country: Optional[str] = None
     doc_number: Optional[str] = None
     kind: Optional[str] = None
 
     def __str__(self):
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/model/images.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/model/images.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from pathlib import Path
-from typing import List
-from typing import Optional
+from typing import List, Optional
 
-from pydantic import computed_field
-from pydantic import Field
-from pypdf import PdfReader
-from pypdf import PdfWriter
+from pydantic import Field, computed_field
+from pypdf import PdfReader, PdfWriter
 
+from ...util import EpoBaseModel, InpadocModel
 from ..schema.images import ImagesSchema
-from patent_client.epo.ops.util import EpoBaseModel
-from patent_client.epo.ops.util import InpadocModel
 
 
 class Section(EpoBaseModel):
     name: Optional[str] = None
     start_page: Optional[int] = None
 
 
@@ -27,15 +23,17 @@
 
     def download(self, path="."):
         from ..api import PublishedImagesApi
 
         out_file = Path(path) / f"{self.doc_number}.pdf"
         writer = PdfWriter()
         for i in range(1, self.num_pages + 1):
-            page_data = PublishedImagesApi.get_page_image_from_link(self.link, page_number=i)
+            page_data = PublishedImagesApi.get_page_image_from_link(
+                self.link, page_number=i
+            )
             page = PdfReader(page_data).pages[0]
             if page["/Rotate"] == 90:
                 page.rotate_clockwise(-90)
             writer.add_page(page)
 
         for section in self.sections:
             writer.add_outline_item(section.name.capitalize(), section.start_page)
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/model/search.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/model/search.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-from typing import List
-from typing import Optional
+from typing import List, Optional
 
-from pydantic import computed_field
-from pydantic import Field
+from pydantic import Field, computed_field
 
-from ...util import InpadocModel
+from ...util import EpoBaseModel, InpadocModel
 from ..schema.search import SearchSchema
-from patent_client.epo.ops.util import EpoBaseModel
 
 
 class Inpadoc(InpadocModel):
     family_id: Optional[str] = None
     id_type: Optional[str] = None
     country: Optional[str] = None
     doc_number: Optional[str] = None
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/schema/biblio.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/schema/biblio.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from yankee.util import clean_whitespace
 from yankee.xml import fields as f
 
-from patent_client.epo.ops.number_service.schema import DocumentIdSchema
-from patent_client.epo.ops.util import Schema
+from ...number_service.schema import DocumentIdSchema
+from ...util import Schema
 
 
 class CpcClassificationSchema(f.Combine):
     section = f.Str("./epo:section")
     klass = f.Str("./epo:class")
     subclass = f.Str("./epo:subclass")
     main_group = f.Str("./epo:main-group")
@@ -43,25 +43,29 @@
 
 
 class InpadocBiblioSchema(Schema):
     country = f.Str("./@country")
     doc_number = f.Str("./@doc-number")
     kind = f.Str("./@kind")
     family_id = f.Str("./@family-id")
-    publication_number = DocDbNumberField('.//epo:publication-reference/epo:document-id[@document-id-type="docdb"]')
+    publication_number = DocDbNumberField(
+        './/epo:publication-reference/epo:document-id[@document-id-type="docdb"]'
+    )
     publication_reference_docdb = DocumentIdSchema(
         './/epo:publication-reference/epo:document-id[@document-id-type="docdb"]'
     )
     publication_reference_epodoc = DocumentIdSchema(
         './/epo:publication-reference/epo:document-id[@document-id-type="epodoc"]'
     )
     publication_reference_original = DocumentIdSchema(
         './/epo:publication-reference/epo:document-id[@document-id-type="original"]'
     )
-    application_number = DocDbNumberField('.//epo:application-reference/epo:document-id[@document-id-type="docdb"]')
+    application_number = DocDbNumberField(
+        './/epo:application-reference/epo:document-id[@document-id-type="docdb"]'
+    )
     application_reference_docdb = DocumentIdSchema(
         './/epo:application-reference/epo:document-id[@document-id-type="docdb"]'
     )
     application_reference_epodoc = DocumentIdSchema(
         './/epo:application-reference/epo:document-id[@document-id-type="epodoc"]'
     )
     application_reference_original = DocumentIdSchema(
@@ -80,15 +84,19 @@
         './/epo:classification-scheme[@scheme="UC"]/following-sibling::epo:classification-symbol',
     )
     priority_claims = f.List(DocumentIdSchema, ".//epo:priority-claim/epo:document-id")
     title = f.Str('.//epo:invention-title[@lang="en"]')
     titles = f.List(TitleSchema, ".//epo:invention-title")
     abstract = f.Str('.//epo:abstract[@lang="en"]')
     citations = f.List(CitationSchema, ".//epo:citation")
-    applicants_epodoc = f.List(f.Str(), './/epo:applicant[@data-format="epodoc"]//epo:name')
-    applicants_original = f.List(f.Str(), './/epo:applicant[@data-format="original"]//epo:name')
+    applicants_epodoc = f.List(
+        f.Str(), './/epo:applicant[@data-format="epodoc"]//epo:name'
+    )
+    applicants_original = f.List(
+        f.Str(), './/epo:applicant[@data-format="original"]//epo:name'
+    )
     inventors_epodoc = f.List(f.Str(), './/epo:inventor[@data-format="epodoc"]')
     inventors_original = f.List(f.Str(), './/epo:inventor[@data-format="original"]')
 
 
 class BiblioResultSchema(Schema):
     documents = f.List(InpadocBiblioSchema, ".//epo:exchange-document")
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/schema/fulltext.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/schema/fulltext.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 
 from yankee.xml import fields as f
 
-from patent_client.epo.ops.util import Schema
 from patent_client.util.claims.parser import ClaimsParser
 
+from ...util import Schema
+
 
 class FTDocumentIdSchema(Schema):
     country = f.Str("./ft:country")
     doc_number = f.Str("./ft:doc-number")
     kind = f.Str("./ft:kind")
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/schema/images.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/schema/images.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import re
 
 from yankee.xml import fields as f
 
-from patent_client.epo.ops.util import Schema
+from ...util import Schema
 
-doc_number_re = re.compile(r"published-data/images/(?P<country>[^/]+)/(?P<doc_number>[^/]+)/(?P<kind_code>[^/]+)/")
+doc_number_re = re.compile(
+    r"published-data/images/(?P<country>[^/]+)/(?P<doc_number>[^/]+)/(?P<kind_code>[^/]+)/"
+)
 
 
 def get_doc_number(string):
     data = doc_number_re.search(string).groupdict()
     return f"{data['country']}{data['doc_number']}{data['kind_code']}"
 
 
@@ -34,10 +36,14 @@
     sections = f.List(SectionSchema, "./ops:document-section")
     doc_number = f.Str("./@link", formatter=get_doc_number)
 
 
 class ImagesSchema(Schema):
     # search_reference = DocumentIdSchema(".//ops:document-inquiry/ops:publication-reference")
     publication_number = DocDbSchema(".//ops:inquiry-result/epo:publication-reference")
-    full_document = ImageDocumentSchema('.//ops:document-instance[@desc="FullDocument"]')
+    full_document = ImageDocumentSchema(
+        './/ops:document-instance[@desc="FullDocument"]'
+    )
     drawing = ImageDocumentSchema('.//ops:document-instance[@desc="Drawing"]')
-    first_page = ImageDocumentSchema('.//ops:document-instance[@desc="FirstPageClipping"]')
+    first_page = ImageDocumentSchema(
+        './/ops:document-instance[@desc="FirstPageClipping"]'
+    )
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/schema/search.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/schema/search.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from yankee.xml import fields as f
 
-from patent_client.epo.ops.util import Schema
+from ...util import Schema
 
 
 class InpadocSchema(Schema):
     family_id = f.Str("./@family-id")
     id_type = f.Str(".//epo:document-id/@document-id-type")
     country = f.Str(".//epo:document-id/epo:country")
     doc_number = f.Str(".//epo:document-id/epo:doc-number")
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/schema_test.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/schema_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import json
 from pathlib import Path
 
 import lxml.etree as ET
 import pytest
 
-from .schema import BiblioResultSchema
-from .schema import ClaimsSchema
-from .schema import DescriptionSchema
-from .schema import ImagesSchema
-from .schema import SearchSchema
 from patent_client.util.test import compare_dicts
 
+from .schema import (
+    BiblioResultSchema,
+    ClaimsSchema,
+    DescriptionSchema,
+    ImagesSchema,
+    SearchSchema,
+)
+
 test_dir = Path(__file__).parent / "test"
 expected_dir = Path(__file__).parent / "test" / "expected"
 
 
 def test_biblio():
     tree = ET.parse(test_dir / "biblio_example.xml")
     result = BiblioResultSchema().load(tree)
@@ -79,15 +82,18 @@
 
 
 def test_full_cycle():
     tree = ET.parse(test_dir / "full_cycle_example.xml")
     result = BiblioResultSchema().load(tree)
     assert len(result.documents) == 2
     d = result.documents[0]
-    assert d.title == "Apparatus for manufacturing green bricks for the brick manufacturing industry"
+    assert (
+        d.title
+        == "Apparatus for manufacturing green bricks for the brick manufacturing industry"
+    )
 
 
 def test_biblio_2():
     filename = "biblio_example_4"
     input = test_dir / f"{filename}.xml"
     tree = ET.parse(input)
     result = BiblioResultSchema().load(tree)
```

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/test/biblio_example.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/biblio_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/test/biblio_example_2.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/biblio_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/test/biblio_example_3.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/biblio_example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/test/biblio_example_4.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/biblio_example_4.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/test/claims_example.json` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/test/claims_example.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/claims_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/test/claims_example_2.json` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/claims_example_2.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/test/claims_example_2.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/claims_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/test/description_example.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/description_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/test/expected/biblio_example_3.json` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/biblio_example_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/test/expected/biblio_example_4.json` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/biblio_example_4.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/test/expected/claims_example.json` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/test/expected/ep1000000_abstract_result.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/test/expected/ep1000000_biblio_result.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/ep1000000_biblio_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/test/expected/ep1000000_claims_result.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/ep1000000_claims_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/test/expected/ep1000000_description_result.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/test/expected/image_example.json` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/image_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/test/expected/search_result.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/search_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/test/full_cycle_example.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/full_cycle_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/test/image_example.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/image_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/published/test/search_example.xml` & `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/search_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/epo/ops/session.py` & `patent_client-5.0.0/patent_client/_async/epo/ops/session.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import base64
 import datetime as dt
 from typing import Sequence
 
 import hishel
 import httpx
-from httpcore import Request
-from httpcore import Response
+from httpcore import Request, Response
 
 from patent_client import SETTINGS
+from patent_client._async.http_client import PatentClientSession
 from patent_client.session import CACHE_DIR
-from patent_client.session import PatentClientSession
 
+import logging
+
+logger = logging.getLogger(__name__)
 
 NS = {
     "http://ops.epo.org": None,
     "http://www.epo.org/exchange": None,
     "http://www.epo.org/fulltext": None,
     "http://www.epo.org/register": None,
 }
 
-import logging
 
-logger = logging.getLogger(__name__)
 
 
 class OpsAuthenticationError(Exception):
     pass
 
 
 class OpsForbiddenError(Exception):
@@ -43,15 +43,18 @@
         cacheable_status_codes: Sequence[int] = (200,),
     ):
         super().__init__()
         self.cacheable_methods = cacheable_methods
         self.cacheable_status_codes = cacheable_status_codes
 
     def is_cachable(self, request: Request, response: Response) -> bool:
-        return request.method in self.cacheable_methods and response.status_code in self.cacheable_status_codes
+        return (
+            request.method in self.cacheable_methods
+            and response.status_code in self.cacheable_status_codes
+        )
 
     def construct_response_from_cache(self, request, response, original_request):
         return response
 
 
 class OpsAuth(httpx.Auth):
     requires_response_body = True
@@ -70,17 +73,17 @@
             response = yield self.build_refresh_request()
             if response.status_code != 200:
                 logger.debug(f"EPO Authentication Error!\n{response.text}")
                 raise OpsAuthenticationError(
                     "Failed to authenticate with EPO OPS! Please check your credentials. See the setup instructions at https://patent-client.readthedocs.io/en/stable/getting_started.html"
                 )
             data = response.json()
-            self.expires = dt.datetime.fromtimestamp(int(data["issued_at"]) / 1000) + dt.timedelta(
-                seconds=int(data["expires_in"])
-            )
+            self.expires = dt.datetime.fromtimestamp(
+                int(data["issued_at"]) / 1000
+            ) + dt.timedelta(seconds=int(data["expires_in"]))
             self.authorization_header = f"Bearer {data['access_token']}"
             request.headers["Authorization"] = self.authorization_header
             yield request
 
     def build_refresh_request(self):
         token = base64.b64encode(f"{self.key}:{self.secret}".encode())
         return httpx.Request(
```

### Comparing `patent_client-4.1.9/patent_client/parser.py` & `patent_client-5.0.0/patent_client/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,17 @@
             elif self.type == "patent" and self.number.isdigit():
                 formatted_number = "{:,}".format(int(self.number))
             elif self.type == "design patent":
                 formatted_number = self.number
             elif self.type == "patent":
                 formatted_number = self.number
             elif self.type == "application":
-                formatted_number = self.number[:2] + "/" + self.number[2:5] + "," + self.number[5:]
+                formatted_number = (
+                    self.number[:2] + "/" + self.number[2:5] + "," + self.number[5:]
+                )
             return f"US {formatted_number} {self.kind_code}".strip()
         elif self.country == "CA":
             return f"CA {self.number} {self.kind_code}"
         else:
             return f"{self.country} {self.number}"
 
     def abbreviation(self):
```

### Comparing `patent_client-4.1.9/patent_client/session.py` & `patent_client-5.0.0/patent_client/_sync/http_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,27 @@
+# ********************************************************************************
+# *         WARNING: This file is automatically generated by unasync.py.         *
+# *                             DO NOT MANUALLY EDIT                             *
+# *               Source File: patent_client/_async/http_client.py               *
+# ********************************************************************************
+
 import re
 import warnings
 from hashlib import blake2b
 from pathlib import Path
 from typing import Optional
 
 import hishel
 import httpcore
 import httpx
 from hishel._utils import normalized_url
 
 from patent_client import CACHE_DIR
-from patent_client.util.asyncio_util import run_sync
 from patent_client.version import __version__
 
-try:
-    from IPython import get_ipython
-
-    if "IPKernelApp" in get_ipython().config:
-        from tqdm.notebook import tqdm
-    else:
-        from tqdm import tqdm
-except (ImportError, AttributeError):
-    from tqdm import tqdm
-
 filename_re = re.compile(r'filename="([^"]+)"')
 
 
 def cache_key_generator(request: httpcore.Request):
     encoded_url = normalized_url(request.url).encode("ascii")
     body = [c for c in request.stream]
     if isinstance(body[0], bytes):
@@ -36,51 +31,54 @@
     key = blake2b(digest_size=16)
     key.update(encoded_url)
     key.update(request.method)
     key.update(body)
     return key.hexdigest()
 
 
-patent_client_transport = hishel.AsyncCacheTransport(
-    transport=httpx.AsyncHTTPTransport(
+patent_client_transport = hishel.CacheTransport(
+    transport=httpx.HTTPTransport(
         verify=False,
         http2=True,
         retries=3,
     ),
-    storage=hishel.AsyncFileStorage(base_path=CACHE_DIR),
-    controller=hishel.Controller(allow_heuristics=True, key_generator=cache_key_generator),
+    storage=hishel.FileStorage(base_path=CACHE_DIR),
+    controller=hishel.Controller(
+        allow_heuristics=True, key_generator=cache_key_generator
+    ),
 )
 
 
-class PatentClientSession(httpx.AsyncClient):
+class PatentClientSession(httpx.Client):
     _default_user_agent = f"Mozilla/5.0 Python Patent Clientbot/{__version__} (parkerhancock@users.noreply.github.com)"
 
     def __init__(self, **kwargs):
         kwargs["transport"] = kwargs.get("transport", patent_client_transport)
         headers = kwargs.get("headers", dict())
         headers["User-Agent"] = headers.get("User-Agent", self._default_user_agent)
         kwargs["headers"] = headers
         kwargs["follow_redirects"] = kwargs.get("follow_redirects", True)
         kwargs["timeout"] = kwargs.get("timeout", 60 * 5)
-        super(PatentClientSession, self).__init__(**kwargs)
-
-    def download(self, url, method: str = "GET", path: Optional[str | Path] = None, **kwargs):
-        return run_sync(self.adownload(url, method, path, **kwargs))
+        super().__init__(**kwargs)
 
     def get_filename(self, url, path, filename, headers):
         if path.is_dir() or None:
             try:
                 filename = filename_re.search(headers["Content-Disposition"]).group(1)
             except (AttributeError, KeyError):
                 filename = url.split("/")[-1]
             path = path / filename if path else Path.cwd() / filename
         return path
 
-    async def adownload(
-        self, url, method: str = "GET", path: Optional[str | Path] = None, show_progress: bool = False, **kwargs
+    def download(
+        self,
+        url,
+        method: str = "GET",
+        path: Optional[str | Path] = None,
+        **kwargs,
     ):
         # Ensure we skip the cache for file downloads
         kwargs["extensions"] = kwargs.get("extensions", dict())
         if "force_cache" in kwargs["extensions"]:
             raise ValueError("force_cache is not supported for file downloads")
         kwargs["extensions"]["cache_disabled"] = True
         if isinstance(path, str):
@@ -88,19 +86,14 @@
         elif path is None:
             path = Path.cwd()
         if not path.is_dir() and path.exists():
             warnings.warn(
                 "File already exists at provided output! Not re-downloading. Please move the file or provide an alternative path to download"
             )
             return path
-        async with self.stream(method, url, **kwargs) as response:
+        with self.stream(method, url, **kwargs) as response:
             response.raise_for_status()
-            total = int(response.headers.get("Content-Length", 0)) or None
-            with tqdm(total=total, unit_scale=True, unit_divisor=1024, unit="B", disable=not show_progress) as progress:
-                num_bytes_downloaded = response.num_bytes_downloaded
-                path = self.get_filename(url, path, response, response.headers)
-                with path.open("wb") as f:
-                    async for chunk in response.aiter_bytes():
-                        f.write(chunk)
-                        progress.update(response.num_bytes_downloaded - num_bytes_downloaded)
-                        num_bytes_downloaded = response.num_bytes_downloaded
+            path = self.get_filename(url, path, response, response.headers)
+            with path.open("wb") as f:
+                for chunk in response.iter_bytes():
+                    f.write(chunk)
         return path
```

### Comparing `patent_client-4.1.9/patent_client/settings.py` & `patent_client-5.0.0/patent_client/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import dotenv
-
-dotenv.load_dotenv()
 from pathlib import Path
 from typing import Optional
+
 from pydantic import Field
 from pydantic_settings import BaseSettings, SettingsConfigDict
 
 
 class Settings(BaseSettings):
     model_config = SettingsConfigDict(env_prefix="patent_client_")
     base_dir: Path = Field(default=Path("~/.patent_client").expanduser())
     log_file: str = Field(default="patent_client.log")
     log_level: str = Field(default="INFO")
     epo_api_key: Optional[str] = Field(default=None)
     epo_api_secret: Optional[str] = Field(default=None)
     itc_username: Optional[str] = Field(default=None)
     itc_password: Optional[str] = Field(default=None)
+    odp_api_key: Optional[str] = Field(default=None)
```

### Comparing `patent_client-4.1.9/patent_client/test_parser.py` & `patent_client-5.0.0/patent_client/test_parser.py`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/assignment/api.py` & `patent_client-5.0.0/patent_client/_async/uspto/assignment/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pathlib import Path
-from typing import Optional
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 from yankee.base.schema import ListCollection
 
+from patent_client._async.http_client import PatentClientSession
+
 from .convert import convert_xml_to_json
 from .model import AssignmentPage
-from .session import session
 
 if TYPE_CHECKING:
     from .model import Assignment
 
 allowed_filters = [
     "PCTNumber",
     "OwnerName",
@@ -27,24 +27,27 @@
 
 
 def validate_input(input, input_name, allowed_values):
     if input not in allowed_values:
         raise ValueError(f"{input_name} must be one of {allowed_values}")
 
 
+client = PatentClientSession()
+
+
 class AssignmentApi:
     @classmethod
-    async def alookup(
-        self, query: str, filter: str, rows=8, start=0, sort="ExecutionDate+desc"
+    async def lookup(
+        cls, query: str, filter: str, rows=8, start=0, sort="ExecutionDate+desc"
     ) -> ListCollection["Assignment"]:
         # Because of their limited utility, we omit fields, highlight, and facet
         url = "https://assignment-api.uspto.gov/patent/lookup"
         validate_input(filter, "filter", allowed_filters)
         validate_input(sort, "sort", allowed_sorts)
-        response = await session.get(
+        response = await client.get(
             url,
             params={
                 "filter": filter,
                 "query": query,
                 "rows": rows,
                 "start": start,
                 "sort": sort,
@@ -52,23 +55,30 @@
             },
             headers={"Accept": "application/xml"},
         )
         response.raise_for_status()
         return AssignmentPage.model_validate(convert_xml_to_json(response.content))
 
     @classmethod
-    async def download_pdf(self, reel: str, frame: str, path: Optional[Path] = None) -> Path:
-        url = self.get_download_url(reel, frame)
+    async def download_pdf(
+        cls, reel: str, frame: str, path: Optional[Path] = None
+    ) -> Path:
+        url = cls.get_download_url(reel, frame)
 
         if path is None:
             path = Path.cwd()
             output_path = output_path = path / f"assignment-pat-{reel}-{frame}.pdf"
         elif path.is_dir():
             output_path = path / f"assignment-pat-{reel}-{frame}.pdf"
         else:
             output_path = path
 
         with output_path.open("wb") as f:
-            async with session.stream("GET", url) as response:
+            async with client.stream("GET", url) as response:
                 async for chunk in response.aiter_bytes():
                     f.write(chunk)
         return output_path
+
+    @classmethod
+    def get_download_url(cls, reel: str, frame: str) -> str:
+        url = f"https://assignment-api.uspto.gov/patent/download/{reel}/{frame}"
+        return url
```

### Comparing `patent_client-4.1.9/patent_client/uspto/assignment/convert.py` & `patent_client-5.0.0/patent_client/_async/uspto/assignment/convert.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 
 def convert_doc(doc):
     output = dict()
     for e in doc.iterchildren():
         if e.tag in ("str", "date", "int"):
             output[e.attrib["name"]] = None if e.text == "NULL" else e.text
         elif e.tag == "arr":
-            output[e.attrib["name"]] = [None if c.text == "NULL" else c.text for c in e.iterchildren()]
+            output[e.attrib["name"]] = [
+                None if c.text == "NULL" else c.text for c in e.iterchildren()
+            ]
     # Collect assignors into a list of dicts
     assignor_fields = ["patAssignorName", "patAssignorExDate", "patAssignorDateAck"]
     output["assignors"] = zip_lists(output, assignor_fields, "assignor")
     # Collect assignees into a list of dicts
     assignee_fields = [
         "patAssigneeName",
         "patAssigneeAddress1",
@@ -39,30 +41,36 @@
     ]
     output["properties"] = zip_lists(output, property_fields, "property")
     # Delete the original fields
     for key in assignor_fields + assignee_fields + property_fields:
         del output[key]
     # Collect the correspondent into a dict
     corr_address_fields = ["corrAddress1", "corrAddress2", "corrAddress3"]
-    correspondent_address = "\n".join(output[k] for k in corr_address_fields if k in output)
+    correspondent_address = "\n".join(
+        output[k] for k in corr_address_fields if k in output
+    )
     if correspondent_address:
         output["corr_address"] = correspondent_address
     for key in corr_address_fields:
         if key in output:
             del output[key]
     output["correspondent"] = {
         "name": output["corrName"],
         "address": output["corr_address"],
     }
     del output["corrName"]
     del output["corr_address"]
 
     # Collect the address for each assignee into a single string
     for assignee in output["assignees"]:
-        address_lines = "\n".join(assignee[k] for k in ["patAssigneeAddress1", "patAssigneeAddress2"] if assignee[k])
+        address_lines = "\n".join(
+            assignee[k]
+            for k in ["patAssigneeAddress1", "patAssigneeAddress2"]
+            if assignee[k]
+        )
         last_line = f"{assignee['patAssigneeCity']}, {assignee['patAssigneeState']} {assignee['patAssigneePostcode']}"
         if assignee["patAssigneeCountryName"]:
             last_line += f" ({assignee['patAssigneeCountryName']})"
         assignee_address = "\n".join([address_lines, last_line])
         if assignee_address:
             assignee["patAssigneeAddress"] = assignee_address
         for key in [
```

### Comparing `patent_client-4.1.9/patent_client/uspto/assignment/convert_test.py` & `patent_client-5.0.0/patent_client/_async/uspto/assignment/convert_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/assignment/fixtures/assignment_1.json` & `patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_1.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/assignment/fixtures/assignment_1.xml` & `patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/assignment/fixtures/assignment_2.json` & `patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_2.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/assignment/fixtures/assignment_2.xml` & `patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/assignment/fixtures/assignment_3.json` & `patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/assignment/fixtures/assignment_3.xml` & `patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/assignment/manager.py` & `patent_client-5.0.0/patent_client/_async/uspto/assignment/manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,53 +2,55 @@
 import re
 import warnings
 from collections.abc import Sequence
 from typing import AsyncIterator
 
 from urllib3.connectionpool import InsecureRequestWarning
 
+from patent_client.util.manager import AsyncManager
+from patent_client.util.request_util import get_start_and_row_count
+
 from .api import AssignmentApi
 from .model import Assignment
-from patent_client.util.manager import Manager
-from patent_client.util.request_util import get_start_and_row_count
 
 warnings.filterwarnings("ignore", category=InsecureRequestWarning)
 
 NUMBER_CLEAN_RE = re.compile(r"[^\d]")
 clean_number = lambda x: NUMBER_CLEAN_RE.sub("", str(x))
 
 
 logger = logging.getLogger(__name__)
 
 
-class AssignmentManager(Manager["Assignment"]):
+class AssignmentManager(AsyncManager["Assignment"]):
     fields = {
         "patent_number": "PatentNumber",
         "appl_id": "ApplicationNumber",
         "app_early_pub_number": "PublicationNumber",
         "assignee": "OwnerName",
         "assignor": "PriorOwnerName",
         "pct_number": "PCTNumber",
         "correspondent": "CorrespondentName",
         "id": "ReelFrame",
     }
     page_size = 100
     obj_class = "patent_client.uspto_assignments.Assignment"
     default_filter = "id"
 
-    def __init__(self, *args, **kwargs):
-        super(AssignmentManager, self).__init__(*args, **kwargs)
-
     @property
     def allowed_filters(self):
         return list(self.fields.keys())
 
-    async def _aget_results(self) -> AsyncIterator["Assignment"]:
-        for start, rows in get_start_and_row_count(self.config.limit, self.config.offset, self.page_size):
-            response = await AssignmentApi.alookup(**{**self.get_query(), "start": start, "rows": rows})
+    async def _get_results(self) -> AsyncIterator["Assignment"]:
+        for start, rows in get_start_and_row_count(
+            self.config.limit, self.config.offset, self.page_size
+        ):
+            response = await AssignmentApi.lookup(
+                **{**self.get_query(), "start": start, "rows": rows}
+            )
             for doc in response.docs:
                 yield doc
             if len(response.docs) < rows:
                 break
 
     def get_query(self):
         """Get assignments.
@@ -66,17 +68,22 @@
                 else:
                     value = value[0]
             field = self.fields[key]
             query = value
         if field in ["PatentNumber", "ApplicationNumber"]:
             query = clean_number(query)
         # Handle Ordering
-        order_map = {"execution_date": "ExecutionDate+asc", "-execution_date": "ExecutionDate+desc"}
+        order_map = {
+            "execution_date": "ExecutionDate+asc",
+            "-execution_date": "ExecutionDate+desc",
+        }
         if len(self.config.order_by) > 1:
-            raise ValueError("Assignment API does not support multiple sort parameters!")
+            raise ValueError(
+                "Assignment API does not support multiple sort parameters!"
+            )
         elif len(self.config.order_by) == 1:
             sort = order_map[self.config.order_by[0]]
         else:
             sort = "ExecutionDate+desc"
 
         # if isinstance(query, list):
         #    query = [f'"{q}"' for q in query]
@@ -84,16 +91,16 @@
         query = {
             "filter": field,
             "query": query,
             "sort": sort,
         }
         return query
 
-    async def alen(self) -> int:
-        response = await AssignmentApi.alookup(**self.get_query())
+    async def count(self) -> int:
+        response = await AssignmentApi.lookup(**self.get_query())
         max_len = response.num_found
         return min(max_len, self.config.limit) if self.config.limit else max_len
 
     @property
     def query_fields(self):
         fields = self.fields
         for k in sorted(fields.keys()):
```

### Comparing `patent_client-4.1.9/patent_client/uspto/assignment/model.py` & `patent_client-5.0.0/patent_client/_sync/uspto/assignment/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,33 @@
+# ********************************************************************************
+# *         WARNING: This file is automatically generated by unasync.py.         *
+# *                             DO NOT MANUALLY EDIT                             *
+# *         Source File: patent_client/_async/uspto/assignment/model.py          *
+# ********************************************************************************
+
 import datetime
 import warnings
 from pathlib import Path
-from typing import List
-from typing import Optional
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, List, Optional
 
 from dateutil.parser import isoparse
-from pydantic import BeforeValidator
-from pydantic import ConfigDict
-from pydantic import Field
-from pydantic import field_validator
+from pydantic import BeforeValidator, ConfigDict, Field, field_validator
 from pydantic.alias_generators import to_camel
 from typing_extensions import Annotated
 
-from patent_client.util.asyncio_util import run_sync
 from patent_client.util.pydantic_util import BaseModel
-from patent_client.util.related import get_model
 
 if TYPE_CHECKING:
-    from patent_client.uspto.peds.model import USApplication
-    from patent_client.uspto.public_search.model import Patent, PublishedApplication
-    from .manager import AssignmentManager
-
-from .session import session
+    from ..peds.model import USApplication
+    from ..public_search.model import Patent, PublishedApplication
 
-UsptoDate = Annotated[datetime.date, BeforeValidator(lambda x: datetime.datetime.strptime(x, "%Y%m%d").date())]
+UsptoDate = Annotated[
+    datetime.date,
+    BeforeValidator(lambda x: datetime.datetime.strptime(x, "%Y%m%d").date()),
+]
 YNBool = Annotated[bool, BeforeValidator(lambda x: x == "Y")]
 
 
 def parse_datetime(string):
     dt = isoparse(string)
     if dt.year == 1 and dt.month == 1 and dt.day == 1:
         return None
@@ -38,15 +37,17 @@
 def parse_date(string):
     dt = parse_datetime(string)
     if dt is None:
         return None
     return dt.date()
 
 
-DatetimeAsDate = Annotated[Optional[datetime.date], BeforeValidator(lambda x: parse_date(x))]
+DatetimeAsDate = Annotated[
+    Optional[datetime.date], BeforeValidator(lambda x: parse_date(x))
+]
 
 
 class AbstractAssignmentModel(BaseModel):
     model_config = ConfigDict(
         alias_generator=to_camel,
         str_strip_whitespace=True,
     )
@@ -79,44 +80,52 @@
 
     @property
     def application(self) -> Optional["USApplication"]:
         """The related US Application"""
         try:
             appl_id = getattr(self, "appl_id", None)
             if appl_id is not None:
-                return get_model("patent_client.uspto.peds.model.USApplication").objects.get(appl_id=appl_id)
+                return self._get_model(
+                    "patent_client.uspto.peds.model.USApplication"
+                ).objects.get(appl_id=appl_id)
             appl_id = getattr(self, "pct_num", None)
             if appl_id is not None:
-                return get_model("patent_client.uspto.peds.model.USApplication").objects.get(appl_id=appl_id)
+                return self._get_model(
+                    "patent_client.uspto.peds.model.USApplication"
+                ).objects.get(appl_id=appl_id)
             pub_num = getattr(self, "publ_num", None)
             if pub_num is not None:
-                return get_model("patent_client.uspto.peds.model.USApplication").objects.get(
-                    app_early_pub_number=pub_num
-                )
+                return self._get_model(
+                    "patent_client.uspto.peds.model.USApplication"
+                ).objects.get(app_early_pub_number=pub_num)
             pat_num = getattr(self, "pat_num", None)
             if pat_num is not None:
-                return get_model("patent_client.uspto.peds.model.USApplication").objects.get(patent_number=pat_num)
+                return self._get_model(
+                    "patent_client.uspto.peds.model.USApplication"
+                ).objects.get(patent_number=pat_num)
         except Exception:
             pass
         warnings.warn(f"Unable to find application for {self}")
         return None
 
     @property
     def patent(self) -> "Patent":
         """The related US Patent, if any"""
-        return get_model("patent_client.uspto.public_search.model.Patent").objects.get(publication_number=self.pat_num)
+        return self._get_model(
+            "patent_client.uspto.public_search.model.Patent"
+        ).objects.get(publication_number=self.pat_num)
 
     @property
     def publication(
         self,
     ) -> "PublishedApplication":
         """The related US Publication, if any"""
-        return get_model("patent_client.uspto.peds.fulltext.patent.model.PublishedApplication").objects.get(
-            publication_number=self.publ_num
-        )
+        return self._get_model(
+            "patent_client.uspto.peds.fulltext.patent.model.PublishedApplication"
+        ).objects.get(publication_number=self.publ_num)
 
 
 class Correspondent(AbstractAssignmentModel):
     name: str
     address: str
 
 
@@ -151,18 +160,19 @@
     def image_url(self):
         reel, frame = self.reel_frame
         reel = reel.rjust(6, "0")
         frame = frame.rjust(4, "0")
         return f"http://legacy-assignments.uspto.gov/assignments/assignment-pat-{reel}-{frame}.pdf"
 
     def download(self, path: Optional[str | Path] = None):
-        """downloads the PDF associated with the assignment to the current working directory"""
-        return run_sync(self.adownload(path=path))
-
-    async def adownload(self, path: Optional[str | Path] = None):
         """asynchronously downloads the PDF associated with the assignment to the current working directory"""
-        return await session.download(self.image_url, path=path)
+        from .api import client
+
+        return client.download(self.image_url, path=path)
 
 
 class AssignmentPage(AbstractAssignmentModel):
     num_found: int
     docs: list[Assignment]
+
+    def __len__(self):
+        return self.num_found
```

### Comparing `patent_client-4.1.9/patent_client/uspto/assignment/model_test.py` & `patent_client-5.0.0/patent_client/_async/uspto/assignment/model_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import datetime
 from pathlib import Path
 
 from .convert import convert_xml_to_json
-from .model import Assignment
 from .model import AssignmentPage
 
 test_dir = Path(__file__).parent / "fixtures"
 
 
 def test_assignment_1():
     xml_file = test_dir / "assignment_1.xml"
@@ -26,23 +25,21 @@
     assert len(a.assignors) == 1
     assert a.assignors[0].name == "REALTIME DATA COMPRESSION SYSTEMS, INC."
     assert a.assignors[0].execution_date.isoformat() == "2006-09-14"
     assert len(a.assignees) == 1
     assert a.assignees[0].name == "REALTIME DATA LLC"
     assert a.assignees[0].address == "15 WEST 36TH STREET\nNEW YORK, NEW YORK 10018"
     assert len(a.properties) == 5
-    assert a.properties[0].invention_title == "SYSTEM AND METHODS FOR ACCELERATED DATA STORAGE AND RETRIEVAL"
+    assert (
+        a.properties[0].invention_title
+        == "SYSTEM AND METHODS FOR ACCELERATED DATA STORAGE AND RETRIEVAL"
+    )
     assert a.properties[0].appl_num == "10628795"
     assert a.properties[0].filing_date.isoformat() == "2003-07-28"
-    assert a.properties[0].intl_publ_date == None
-    assert a.properties[0].intl_reg_num == None
+    assert a.properties[0].intl_publ_date is None
+    assert a.properties[0].intl_reg_num is None
     assert a.properties[0].inventors == "James J. Fallon"
     assert a.properties[0].issue_date.isoformat() == "2006-10-31"
     assert a.properties[0].pat_num == "7130913"
-    assert a.properties[0].pct_num == None
+    assert a.properties[0].pct_num is None
     assert a.properties[0].publ_date.isoformat() == "2004-04-15"
     assert a.properties[0].publ_num == "20040073746"
-
-
-def test_manager():
-    a = Assignment.objects.get("18247-405")
-    assert a.id == "18247-405"
```

### Comparing `patent_client-4.1.9/patent_client/uspto/bulk_data/api.py` & `patent_client-5.0.0/patent_client/_async/uspto/bulk_data/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import datetime
 import typing as tp
 
+from patent_client._async.http_client import PatentClientSession
+
 from .model import Product
-from .session import session
+
+client = PatentClientSession()
 
 
 class BulkDataApi:
     @classmethod
     async def get_latest(cls) -> tp.List[Product]:
         """Returns all products with Latest Files"""
-        response = await session.get("https://bulkdata.uspto.gov:443/BDSS-API/products/all/latest")
+        response = await client.get(
+            "https://bulkdata.uspto.gov:443/BDSS-API/products/all/latest"
+        )
         return [Product(**product) for product in response.json()]
 
     @classmethod
     async def get_by_name(
         cls,
         product_name: str,
         from_date: tp.Optional[datetime.date] = None,
@@ -31,24 +36,27 @@
         if to_date:
             if isinstance(to_date, str):
                 to_date = datetime.date.fromisoformat(to_date)
             params["toYear"] = to_date.year
             params["toMonth"] = to_date.month
             params["toDay"] = to_date.day
         params["maxFiles"] = max_files
-        response = await session.get(
-            f"https://bulkdata.uspto.gov:443/BDSS-API/products/byname/{product_name}", params=params
+        response = await client.get(
+            f"https://bulkdata.uspto.gov:443/BDSS-API/products/byname/{product_name}",
+            params=params,
         )
         response.raise_for_status()
         return [Product.model_validate(product) for product in response.json()]
 
     @classmethod
     async def get_popular(cls) -> tp.List[Product]:
         """Returns popular products along with latest files."""
-        response = await session.get("https://bulkdata.uspto.gov:443/BDSS-API/products/popular")
+        response = await client.get(
+            "https://bulkdata.uspto.gov:443/BDSS-API/products/popular"
+        )
         return [Product.model_validate(product) for product in response.json()]
 
     @classmethod
     async def get_by_short_name(
         cls,
         product_name: str,
         from_date: tp.Optional[datetime.date | str] = None,
@@ -65,9 +73,12 @@
             params["fromDay"] = from_date.day
         if to_date:
             if isinstance(to_date, str):
                 to_date = datetime.date.fromisoformat(to_date)
             params["toYear"] = to_date.year
             params["toMonth"] = to_date.month
             params["toDay"] = to_date.day
-        response = await session.get(f"https://bulkdata.uspto.gov:443/BDSS-API/products/{product_name}", params=params)
+        response = await client.get(
+            f"https://bulkdata.uspto.gov:443/BDSS-API/products/{product_name}",
+            params=params,
+        )
         return Product.model_validate(response.json())
```

### Comparing `patent_client-4.1.9/patent_client/uspto/bulk_data/api_test.py` & `patent_client-5.0.0/patent_client/_async/uspto/bulk_data/api_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pytest
 
 from .api import BulkDataApi
-from .model import File
-from .model import Product
+from .model import File, Product
 
 
 @pytest.mark.asyncio
 async def test_can_get_latest():
     latest = await BulkDataApi.get_latest()
     first = latest[0]
     assert isinstance(first, Product)
@@ -18,15 +17,17 @@
     first = await BulkDataApi.get_by_short_name("PTGRXML")
     assert isinstance(first, Product)
     assert isinstance(first.files[0], File)
 
 
 @pytest.mark.asyncio
 async def test_can_get_by_short_name_with_date_range():
-    first = await BulkDataApi.get_by_short_name("PTGRXML", from_date="2023-06-01", to_date="2023-08-01")
+    first = await BulkDataApi.get_by_short_name(
+        "PTGRXML", from_date="2023-06-01", to_date="2023-08-01"
+    )
     assert isinstance(first, Product)
     assert isinstance(first.files[0], File)
     assert len(first.files) == 10
 
 
 @pytest.mark.asyncio
 @pytest.mark.no_vcr
```

### Comparing `patent_client-4.1.9/patent_client/uspto/bulk_data/manager.py` & `patent_client-5.0.0/patent_client/_async/uspto/bulk_data/manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 import calendar
 import datetime
 import typing as tp
 
+from patent_client.util.manager import AsyncManager
+
 from .api import BulkDataApi
-from patent_client.util.asyncio_util import run_async_iterator
-from patent_client.util.asyncio_util import run_sync
-from patent_client.util.manager import Manager
 
 if tp.TYPE_CHECKING:
     from .model import File, Product
 
 
 def date_ranges(start_date: datetime.date, end_date: datetime.date):
     # First range: start date to end of month
     end_of_month = datetime.datetime(
-        start_date.year, start_date.month, calendar.monthrange(start_date.year, start_date.month)[1]
+        start_date.year,
+        start_date.month,
+        calendar.monthrange(start_date.year, start_date.month)[1],
     )
     yield (start_date, end_of_month.date())
 
     # Full months between start and end date
     current_month = start_date.replace(day=1) + datetime.timedelta(days=32)
     while current_month.replace(day=1) < end_date.replace(day=1):
-        last_day_of_month = current_month.replace(day=calendar.monthrange(current_month.year, current_month.month)[1])
+        last_day_of_month = current_month.replace(
+            day=calendar.monthrange(current_month.year, current_month.month)[1]
+        )
         yield (current_month.replace(day=1), last_day_of_month)
         current_month += datetime.timedelta(days=32)
 
     # Last range: start of month to end date
     yield (end_date.replace(day=1), end_date)
 
 
-class ProductManager(Manager):
-    def filter_by_latest(self) -> tp.Iterator["Product"]:
-        """Returns all products with Latest Files"""
-        for item in run_async_iterator(self.afilter_by_latest()):
-            yield item
-
-    async def afilter_by_latest(self) -> tp.AsyncIterator["Product"]:
+class ProductManager(AsyncManager):
+    async def filter_by_latest(self) -> tp.AsyncIterator["Product"]:
         """Returns all products with Latest Files"""
         result = await BulkDataApi.get_latest()
         for product in result:
             yield product
 
-    def get_by_short_name(self, short_name) -> "Product":
-        return run_sync(self.aget_by_short_name(short_name))
+    async def get_by_short_name(self, short_name) -> "Product":
+        result = await BulkDataApi.get_by_short_name(short_name)
+        return result
 
-    async def aget_by_short_name(self, short_name) -> "Product":
-        return await BulkDataApi.get_by_short_name(short_name)
-
-    def filter_by_name(self, short_name) -> tp.Iterator["Product"]:
-        for item in run_async_iterator(self.afilter_by_name(short_name)):
-            yield item
-
-    async def afilter_by_name(self, short_name) -> tp.AsyncIterator["Product"]:
+    async def filter_by_name(self, short_name) -> tp.AsyncIterator["Product"]:
         result = await BulkDataApi.get_by_name(short_name)
         for product in result:
             yield product
 
 
-class FileManager(Manager):
-    def filter_by_short_name(self, short_name, from_date=None, to_date=None) -> tp.Iterator["File"]:
-        for item in run_async_iterator(self.afilter_by_short_name(short_name, from_date, to_date)):
-            yield item
-
-    async def afilter_by_short_name(self, short_name, from_date=None, to_date=None) -> tp.AsyncIterator["File"]:
+class FileManager(AsyncManager):
+    async def filter_by_short_name(
+        self, short_name, from_date=None, to_date=None
+    ) -> tp.AsyncIterator["File"]:
         if from_date is not None:
-            from_date = from_date if isinstance(from_date, datetime.date) else datetime.date.fromisoformat(from_date)
+            from_date = (
+                from_date
+                if isinstance(from_date, datetime.date)
+                else datetime.date.fromisoformat(from_date)
+            )
         if to_date is not None:
-            to_date = to_date if isinstance(to_date, datetime.date) else datetime.date.fromisoformat(to_date)
+            to_date = (
+                to_date
+                if isinstance(to_date, datetime.date)
+                else datetime.date.fromisoformat(to_date)
+            )
         if from_date is None or to_date is None:
             product = await BulkDataApi.get_by_short_name(short_name)
             from_date = from_date or product.from_date
             to_date = to_date or product.to_date
         for start_date, end_date in date_ranges(from_date, to_date):
-            chunk = await BulkDataApi.get_by_short_name(short_name, from_date=start_date, to_date=end_date)
+            chunk = await BulkDataApi.get_by_short_name(
+                short_name, from_date=start_date, to_date=end_date
+            )
             if chunk.files:
                 for file in chunk.files:
                     yield file
```

### Comparing `patent_client-4.1.9/patent_client/uspto/bulk_data/manager_test.py` & `patent_client-5.0.0/patent_client/_async/uspto/bulk_data/manager_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,50 @@
 import datetime
 
+import pytest
+
 from .manager import date_ranges
-from .model import File
-from .model import Product
+from .model import File, Product
 
 
 class TestProduct:
-    def test_can_get_latest(self):
-        latest = list(Product.objects.filter_by_latest())
+    @pytest.mark.asyncio
+    async def test_can_get_latest(self):
+        latest = [p async for p in Product.objects.filter_by_latest()]
         assert isinstance(latest[0], Product)
 
-    def test_can_get_by_short_name(self):
-        first = Product.objects.get_by_short_name("PTGRXML")
+    @pytest.mark.asyncio
+    async def test_can_get_by_short_name(self):
+        first = await Product.objects.get_by_short_name("PTGRXML")
         assert isinstance(first, Product)
         assert isinstance(first.files[0], File)
 
-    def test_can_filter_by_name(self):
-        first = Product.objects.filter_by_name("Assignment")
+    @pytest.mark.asyncio
+    async def test_can_filter_by_name(self):
+        first = [p async for p in Product.objects.filter_by_name("Assignment")]
         first = list(first)[0]
         assert isinstance(first, Product)
         assert isinstance(first.files[0], File)
 
 
 class TestFile:
-    def test_can_filter_by_short_name(self):
-        results = list(File.objects.filter_by_short_name("PTGRXML", from_date="2023-06-15", to_date="2023-08-15"))
+    @pytest.mark.asyncio
+    async def test_can_filter_by_short_name(self):
+        results = [
+            f
+            async for f in File.objects.filter_by_short_name(
+                "PTGRXML", from_date="2023-06-15", to_date="2023-08-15"
+            )
+        ]
         assert len(results) == 10
         assert isinstance(results[0], File)
 
-    def test_can_get_daily_assignments(self):
-        results = list(File.objects.filter_by_short_name("PASDL"))
+    @pytest.mark.asyncio
+    async def test_can_get_daily_assignments(self):
+        results = [f async for f in File.objects.filter_by_short_name("PASDL")]
         assert len(results) > 1
         assert isinstance(results[0], File)
 
 
 def test_date_ranges():
     result = list(date_ranges(datetime.date(2020, 1, 15), datetime.date(2021, 2, 15)))
     assert result[0] == (datetime.date(2020, 1, 15), datetime.date(2020, 1, 31))
```

### Comparing `patent_client-4.1.9/patent_client/uspto/bulk_data/model.py` & `patent_client-5.0.0/patent_client/_async/uspto/bulk_data/model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 import datetime
 import typing as tp
 from pathlib import Path
 
 from pydantic import Field
 
-from patent_client.util.asyncio_util import run_sync
 from patent_client.util.pydantic_util import BaseModel
 
 
 class File(BaseModel):
     link_path: str = Field(alias="fileLinkPath")
     identifier: int = Field(alias="fileIdentifier")
     name: str = Field(alias="fileName")
     size: int = Field(alias="fileSize")
     download_url: str = Field(alias="fileDownloadUrl")
     from_date: datetime.date = Field(alias="fileFromTime")
     to_date: datetime.date = Field(alias="fileToTime")
     type: str = Field(alias="fileType")
     release_date: datetime.date = Field(alias="fileReleaseDate")
 
-    async def adownload(self, path: tp.Optional[str | Path]):
-        from .session import session
+    async def download(self, path: tp.Optional[str | Path]):
+        from .api import client
 
-        return await session.adownload(self.download_url, path=path)
-
-    def download(self, path: tp.Optional[str | Path] = None):
-        return run_sync(self.adownload(path))
+        return await client.download(self.download_url, path=path)
 
 
 class Product(BaseModel):
     link_path: str = Field(alias="productLinkPath")
     identifier: int = Field(alias="productIdentifier")
     short_name: str = Field(alias="productShortName")
     description: str = Field(alias="productDesc")
     title: str = Field(alias="productTitle")
     frequency: tp.Optional[str] = Field(alias="productFrequency", default=None)
     level: str = Field(alias="productLevel")
     from_date: datetime.date = Field(alias="productFromDate")
     to_date: datetime.date = Field(alias="productToDate")
     number_of_files: int = Field(alias="numberOfFiles")
     parent_product: tp.Optional[str] = Field(alias="parentProduct", default=None)
-    files: tp.Optional[tp.List[File]] = Field(alias="productFiles", default_factory=list)
+    files: tp.Optional[tp.List[File]] = Field(
+        alias="productFiles", default_factory=list
+    )
```

### Comparing `patent_client-4.1.9/patent_client/uspto/global_dossier/gd_input.csv` & `patent_client-5.0.0/patent_client/_async/uspto/global_dossier/gd_input.csv`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/global_dossier/manager.py` & `patent_client-5.0.0/patent_client/_async/uspto/global_dossier/manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,58 @@
+from patent_client.util.manager import AsyncManager
+
 from .api import GlobalDossierApi
 from .query import QueryBuilder
-from patent_client.util.manager import Manager
 
 query_builder = QueryBuilder()
 
 global_dossier_api = GlobalDossierApi()
 
 
-class GlobalDossierBaseManager(Manager):
+class GlobalDossierBaseManager(AsyncManager):
     def filter(self, *args, **kwargs):
-        raise NotImplementedError("GlobalDossier can only retrieve using the GET interface")
+        raise NotImplementedError(
+            "GlobalDossier can only retrieve using the GET interface"
+        )
 
     def order_by(self, *args, **kwargs):
-        raise NotImplementedError("GlobalDossier can only retrieve using the GET interface")
+        raise NotImplementedError(
+            "GlobalDossier can only retrieve using the GET interface"
+        )
 
     def limit(self, *args, **kwargs):
-        raise NotImplementedError("GlobalDossier can only retrieve using the GET interface")
+        raise NotImplementedError(
+            "GlobalDossier can only retrieve using the GET interface"
+        )
 
     def offset(self, *args, **kwargs):
-        raise NotImplementedError("GlobalDossier can only retrieve using the GET interface")
+        raise NotImplementedError(
+            "GlobalDossier can only retrieve using the GET interface"
+        )
 
 
 class GlobalDossierManager(GlobalDossierBaseManager):
-    async def aget(self, *args, **kwargs):
-        return await global_dossier_api.get_file(**query_builder.build_query(*args, **kwargs))
+    async def get(self, *args, **kwargs):
+        return await global_dossier_api.get_file(
+            **query_builder.build_query(*args, **kwargs)
+        )
 
 
 class GlobalDossierApplicationManager(GlobalDossierBaseManager):
-    async def aget(self, *args, **kwargs):
+    async def get(self, *args, **kwargs):
         query = query_builder.build_query(*args, **kwargs)
         gd_file = await global_dossier_api.get_file(**query)
         if query["type_code"] == "application":
-            return next(a for a in gd_file.applications if a.app_num in query["doc_number"])
+            return next(
+                a for a in gd_file.applications if a.app_num in query["doc_number"]
+            )
         elif query["type_code"] == "publication":
-            return next(a for a in gd_file.applications if any(p.pub_num in query["doc_number"] for p in a.pub_list))
+            return next(
+                a
+                for a in gd_file.applications
+                if any(p.pub_num in query["doc_number"] for p in a.pub_list)
+            )
 
 
 class DocumentListManager(GlobalDossierBaseManager):
-    async def aget(self, country, doc_number, kind_code):
+    async def get(self, country, doc_number, kind_code):
         return await global_dossier_api.get_doc_list(country, doc_number, kind_code)
```

### Comparing `patent_client-4.1.9/patent_client/uspto/global_dossier/model.py` & `patent_client-5.0.0/patent_client/_async/uspto/global_dossier/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,171 +1,197 @@
 import datetime
+import typing as tp
 from pathlib import Path
-from typing import *
 
-from pydantic import BeforeValidator
-from pydantic import ConfigDict
-from pydantic import Field
-from pydantic import model_validator
+from async_property import async_property
+from pydantic import BeforeValidator, ConfigDict, Field, model_validator
 from pydantic.alias_generators import to_camel
 from typing_extensions import Annotated
 
-from patent_client.util.asyncio_util import run_sync
 from patent_client.util.pydantic_util import BaseModel
-from patent_client.util.related import get_model
 
-MDYDate = Annotated[datetime.date, BeforeValidator(lambda x: datetime.datetime.strptime(x, "%m/%d/%Y").date())]
-OptionalStrList = Annotated[List[str], BeforeValidator(lambda x: x if isinstance(x, list) else list())]
+if tp.TYPE_CHECKING:
+    from ..peds.model import USApplication
+    from ..public_search.model import Patent, PublishedApplication
+    from ..assignment.model import Assignment
+
+MDYDate = Annotated[
+    datetime.date,
+    BeforeValidator(lambda x: datetime.datetime.strptime(x, "%m/%d/%Y").date()),
+]
+OptionalStrList = Annotated[
+    tp.List[str], BeforeValidator(lambda x: x if isinstance(x, list) else list())
+]
 
 
 class GlobalDossierBaseModel(BaseModel):
     model_config = ConfigDict(
         alias_generator=to_camel,
         str_strip_whitespace=True,
     )
 
 
 class GlobalDossierPublication(GlobalDossierBaseModel):
-    pub_country: Optional[str] = None
-    pub_num: Optional[str] = None
-    kind_code: Optional[str] = None
-    pub_date: Optional[MDYDate] = Field(alias="pubDateStr")
+    pub_country: tp.Optional[str] = None
+    pub_num: tp.Optional[str] = None
+    kind_code: tp.Optional[str] = None
+    pub_date: tp.Optional[MDYDate] = Field(alias="pubDateStr")
 
 
 class GlobalDossierPriorityClaim(GlobalDossierBaseModel):
-    country: Optional[str] = None
-    doc_number: Optional[str] = None
-    kind_code: Optional[str] = None
+    country: tp.Optional[str] = None
+    doc_number: tp.Optional[str] = None
+    kind_code: tp.Optional[str] = None
 
 
 class GlobalDossierDocumentNumber(GlobalDossierBaseModel):
-    country: Optional[str] = None
-    doc_number: Optional[str] = None
-    format: Optional[str] = None
-    date: Optional[MDYDate] = None
-    kind_code: Optional[str] = None
+    country: tp.Optional[str] = None
+    doc_number: tp.Optional[str] = None
+    format: tp.Optional[str] = None
+    date: tp.Optional[MDYDate] = None
+    kind_code: tp.Optional[str] = None
 
 
 class GlobalDossierApplication(GlobalDossierBaseModel):
-    app_num: Optional[str] = None
-    app_date: Optional[MDYDate] = Field(alias="appDateStr")
-    country_code: Optional[str] = None
-    kind_code: Optional[str] = None
-    doc_num: Optional["GlobalDossierDocumentNumber"] = None
-    title: Optional[str] = None
+    app_num: tp.Optional[str] = None
+    app_date: tp.Optional[MDYDate] = Field(alias="appDateStr")
+    country_code: tp.Optional[str] = None
+    kind_code: tp.Optional[str] = None
+    doc_num: tp.Optional["GlobalDossierDocumentNumber"] = None
+    title: tp.Optional[str] = None
     applicant_names: OptionalStrList = Field(default_factory=list)
-    ip_5: Optional[bool] = Field(alias="ip5")
-    priority_claim_list: "List[GlobalDossierPriorityClaim]" = Field(default_factory=list)
-    pub_list: "List[GlobalDossierPublication]" = Field(default_factory=list)
+    ip_5: tp.Optional[bool] = Field(alias="ip5")
+    priority_claim_list: "tp.List[GlobalDossierPriorityClaim]" = Field(
+        default_factory=list
+    )
+    pub_list: "tp.List[GlobalDossierPublication]" = Field(default_factory=list)
 
     def __repr__(self):
         return f"GlobalDossierApplication(app_num={self.app_num}, country_code={self.country_code})"
 
-    @property
-    def document_list(self):
-        return get_model("patent_client.uspto.global_dossier.model.DocumentList").objects.get(
+    @async_property
+    async def document_list(self) -> "DocumentList":
+        return await self._get_model(".model.DocumentList").objects.get(
             self.country_code, self.app_num, self.kind_code
         )
 
-    @property
-    def documents(self):
+    @async_property
+    async def documents(self) -> list["Document"]:
         return (
-            get_model("patent_client.uspto.global_dossier.model.DocumentList")
-            .objects.get(self.country_code, self.app_num, self.kind_code)
-            .docs
-        )
+            await self._get_model(".model.DocumentList").objects.get(
+                self.country_code, self.app_num, self.kind_code
+            )
+        ).docs
 
-    @property
-    def office_actions(self):
+    @async_property
+    async def office_actions(self) -> list["Document"]:
         return (
-            get_model("patent_client.uspto.global_dossier.model.DocumentList")
-            .objects.get(self.country_code, self.app_num, self.kind_code)
-            .office_action_docs
-        )
+            await self._get_model(".model.DocumentList").objects.get(
+                self.country_code, self.app_num, self.kind_code
+            )
+        ).office_action_docs
 
-    @property
-    def us_application(self):
+    @async_property
+    async def us_application(self) -> "USApplication":
         if self.country_code != "US":
-            raise ValueError(f"Global Dossier Application is not a US Application! {self}")
-        return get_model("patent_client.uspto.peds.model.USApplication").objects.get(self.app_num)
+            raise ValueError(
+                f"Global Dossier Application is not a US Application! {self}"
+            )
+        return await self._get_model("..peds.model.USApplication").objects.get(
+            self.app_num
+        )
 
-    @property
-    def us_publication(self):
+    @async_property
+    async def us_publication(self) -> "PublishedApplication":
         if self.country_code != "US":
-            raise ValueError(f"Global Dossier Application is not a US Application! {self}")
+            raise ValueError(
+                f"Global Dossier Application is not a US Application! {self}"
+            )
         pub = list(p for p in self.pub_list if p.kind_code == "A1")
         if len(pub) > 1:
             raise ValueError("More than one US publication for application!")
-        return get_model("patent_client.uspto.public_search.model.PublishedApplication").objects.get(pub[0].pub_num)
+        return await self._get_model(
+            "..public_search.model.PublishedApplication"
+        ).objects.get(pub[0].pub_num)
 
-    @property
-    def us_patent(self):
+    @async_property
+    async def us_patent(self) -> "Patent":
         if self.country_code != "US":
-            raise ValueError(f"Global Dossier Application is not a US Application! {self}")
+            raise ValueError(
+                f"Global Dossier Application is not a US Application! {self}"
+            )
         pat = list(p for p in self.pub_list if p.kind_code in ("A", "B1", "B2"))
         if len(pat) > 1:
             raise ValueError("More than one US patent for application!")
-        return get_model("patent_client.uspto.public_search.model.Patent").objects.get(pat[0].pub_num)
+        return await self._get_model("..public_search.model.Patent").objects.get(
+            pat[0].pub_num
+        )
 
-    @property
-    def us_assignments(self):
+    @async_property
+    async def us_assignments(self) -> list["Assignment"]:
         if self.country_code != "US":
-            raise ValueError(f"Global Dossier Application is not a US Application! {self}")
-        return get_model("patent_client.uspto.assignment.model.Assignment").objects.filter(appl_id=self.app_num)
+            raise ValueError(
+                f"Global Dossier Application is not a US Application! {self}"
+            )
+        return self._get_model("..assignment.model.Assignment").objects.filter(
+            appl_id=self.app_num
+        )
 
 
 TextBool = Annotated[bool, BeforeValidator(lambda x: x == "true")]
 
 
 class GlobalDossier(GlobalDossierBaseModel):
-    country: Optional[str] = None
-    internal: Optional[TextBool] = None
-    corr_app_num: Optional[str] = None
-    id: Optional[str] = None
-    type: Optional[str] = None
-    applications: List[GlobalDossierApplication] = Field(default_factory=list, alias="list")
+    country: tp.Optional[str] = None
+    internal: tp.Optional[TextBool] = None
+    corr_app_num: tp.Optional[str] = None
+    id: tp.Optional[str] = None
+    type: tp.Optional[str] = None
+    applications: tp.List[GlobalDossierApplication] = Field(
+        default_factory=list, alias="list"
+    )
 
     def __repr__(self):
         return f"GlobalDossier(id={self.id}, type={self.type}, country={self.country})"
 
 
 class Document(GlobalDossierBaseModel):
-    doc_number: Optional[str] = None
-    country: Optional[str] = None
-    doc_code: Optional[str] = None
-    doc_desc: Optional[str] = None
-    doc_id: Optional[str] = None
-    date: Optional[MDYDate] = Field(alias="legalDateStr")
-    doc_format: Optional[str] = None
-    pages: Optional[int] = Field(alias="numberOfPages")
-    doc_code_desc: Optional[str] = None
-    doc_group_code: Optional[str] = None
-    shareable: Optional[bool] = None
+    doc_number: tp.Optional[str] = None
+    country: tp.Optional[str] = None
+    doc_code: tp.Optional[str] = None
+    doc_desc: tp.Optional[str] = None
+    doc_id: tp.Optional[str] = None
+    date: tp.Optional[MDYDate] = Field(alias="legalDateStr")
+    doc_format: tp.Optional[str] = None
+    pages: tp.Optional[int] = Field(alias="numberOfPages")
+    doc_code_desc: tp.Optional[str] = None
+    doc_group_code: tp.Optional[str] = None
+    shareable: tp.Optional[bool] = None
 
-    def download(self, filename="", path="."):
-        return run_sync(self.adownload(filename, path))
-
-    async def adownload(self, filename="", path="."):
+    async def download(self, filename="", path="."):
         from .manager import global_dossier_api
 
         out_path = Path(path).expanduser() / (
-            f'{self.date.isoformat()} - {self.doc_desc.replace("/", "_")}.pdf' if not filename else filename
+            f'{self.date.isoformat()} - {self.doc_desc.replace("/", "_")}.pdf'
+            if not filename
+            else filename
+        )
+        return await global_dossier_api.get_document(
+            self.country, self.doc_number, self.doc_id, out_path=out_path
         )
-        return await global_dossier_api.get_document(self.country, self.doc_number, self.doc_id, out_path=out_path)
 
 
 class DocumentList(GlobalDossierBaseModel):
-    title: Optional[str] = None
-    doc_number: Optional[str] = None
-    country: Optional[str] = None
-    message: Optional[str] = None
-    applicant_names: "List[str]" = Field(default_factory=list)
-    office_action_count: Optional[int] = Field(alias="oaIndCount")
-    docs: List[Document] = Field(default_factory=list)
-    office_action_docs: List[Document] = Field(default_factory=list)
+    title: tp.Optional[str] = None
+    doc_number: tp.Optional[str] = None
+    country: tp.Optional[str] = None
+    message: tp.Optional[str] = None
+    applicant_names: "tp.List[str]" = Field(default_factory=list)
+    docs: tp.List[Document] = Field(default_factory=list)
+    office_action_docs: tp.List[Document] = Field(default_factory=list)
 
     @model_validator(mode="before")
     @classmethod
     def annotate_docs_and_office_actions(cls, values):
         update_dict = {
             "country": values["country"],
             "docNumber": values["docNumber"],
```

### Comparing `patent_client-4.1.9/patent_client/uspto/global_dossier/query.py` & `patent_client-5.0.0/patent_client/_async/uspto/global_dossier/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,17 @@
                 if "type" in kwargs:
                     return {
                         "office_code": country,
                         "type_code": kwargs["type"],
                         "doc_number": number,
                     }
                 candidates = [
-                    r for r in self.input_schema if r["office_code"] == country and r["pattern"].fullmatch(number)
+                    r
+                    for r in self.input_schema
+                    if r["office_code"] == country and r["pattern"].fullmatch(number)
                 ]
                 if not candidates:
                     raise QueryException(
                         f"While country was detected as {country}, no number format matched {number}, please check your number"
                     )
                 if len(candidates) > 1:
                     raise QueryException(
@@ -86,39 +88,49 @@
                 else:
                     raise QueryException(
                         "While country was detected as AU, no type can be inferred. Please pass a 'type' keyword to specify application/publication"
                     )
             else:
                 office_code = kwargs.get("office", "US")
                 candidates = [
-                    r for r in self.input_schema if r["office_code"] == office_code and r["pattern"].fullmatch(arg)
+                    r
+                    for r in self.input_schema
+                    if r["office_code"] == office_code and r["pattern"].fullmatch(arg)
                 ]
                 if not candidates:
                     raise QueryException(
                         f"While country was detected as {office_code}, no number format matched {arg}, please check your number"
                     )
                 if len(candidates) > 1:
                     types = [c["type_name"] for c in candidates]
                     if "Application" in types and office_code == "US":
                         return {
                             "office_code": office_code,
                             "doc_number": arg,
                             "type_code": "application",
                         }
-                    raise QueryException(f"Cannot determine number type. Possible types are {types}")
+                    raise QueryException(
+                        f"Cannot determine number type. Possible types are {types}"
+                    )
                 return {
                     "office_code": office_code,
                     "doc_number": arg,
                     "type_code": candidates[0]["type_code"],
                 }
 
         elif kwargs:
-            numbers = {k: v for k, v in kwargs.items() if k in ("publication", "application", "patent")}
+            numbers = {
+                k: v
+                for k, v in kwargs.items()
+                if k in ("publication", "application", "patent")
+            }
             if len(numbers) > 1:
-                raise QueryException("You may only pass one keyword from the set of (application, publication, patent)")
+                raise QueryException(
+                    "You may only pass one keyword from the set of (application, publication, patent)"
+                )
             elif not numbers:
                 raise QueryException("No number passed! Please pass a valid number")
             key, value = list(numbers.items())[0]
             if value[:2] in ["US", "CN", "EP", "KR", "JP"]:
                 return {
                     "office_code": value[:2],
                     "type_code": key,
```

### Comparing `patent_client-4.1.9/patent_client/uspto/global_dossier/query_test.py` & `patent_client-5.0.0/patent_client/_async/uspto/global_dossier/query_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pytest
 
-from .query import QueryBuilder
-from .query import QueryException
+from .query import QueryBuilder, QueryException
 
 builder = QueryBuilder()
 
 
 def test_garbage():
     with pytest.raises(QueryException):
         builder.build_query("garbage")
```

### Comparing `patent_client-4.1.9/patent_client/uspto/global_dossier/test/app.json` & `patent_client-5.0.0/patent_client/_async/uspto/global_dossier/test/app.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/global_dossier/test/app_expected.json` & `patent_client-5.0.0/patent_client/_async/uspto/global_dossier/test/app_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/global_dossier/test/doc_list.json` & `patent_client-5.0.0/patent_client/_async/uspto/global_dossier/test/doc_list.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/global_dossier/test/doc_list_expected.json` & `patent_client-5.0.0/patent_client/_async/uspto/global_dossier/test/doc_list_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/peds/api.py` & `patent_client-5.0.0/patent_client/_async/uspto/peds/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,67 @@
 import datetime
 import logging
-from typing import Dict
-from typing import List
-from typing import Optional
+from typing import Dict, List, Optional
 
 from httpx._exceptions import HTTPStatusError
 
-from .model import Document
-from .model import PedsPage
-from .session import session
+from patent_client._async.http_client import PatentClientSession
+
+from .model import Document, PedsPage
 
 logger = logging.getLogger(__name__)
 
 type_map = {
     "string": str,
     "date": datetime.datetime,
     "text_general": str,
     "int": int,
     "text_ws": str,
 }
 
+client = PatentClientSession()
+
 
 class PedsDownException(Exception):
     pass
 
 
 class PatentExaminationDataSystemApi:
     base_url = "https://ped.uspto.gov/api"
     search_fields: Dict = dict()
 
-    def __init__(self):
-        query_id = None
-
     async def is_online(self) -> bool:
-        response = await session.get("https://ped.uspto.gov/api/search-fields", extensions={"cache_disabled": True})
+        response = await client.get(
+            "https://ped.uspto.gov/api/search-fields",
+            extensions={"cache_disabled": True},
+        )
         if response.status_code == 200:
             return True, ""
         elif "requested resource is not available" in response.text:
             return False, "Patent Examination Data is Offline - this is a USPTO problem"
         elif "attempt failed or the origin closed the connection" in response.text:
-            return False, "The Patent Examination Data API is Broken! - this is a USPTO problem"
+            return (
+                False,
+                "The Patent Examination Data API is Broken! - this is a USPTO problem",
+            )
         else:
             return False, "There is a USPTO problem"
 
     async def check_response(self, response):
         try:
             response.raise_for_status()
         except HTTPStatusError as e:
             alive, reason = await self.is_online()
             raise e if alive else PedsDownException(reason)
 
     @classmethod
     async def get_search_fields(cls) -> dict:
         if hasattr(cls, "search_fields"):
             return cls.search_fields
-        response = await session.get("https://ped.uspto.gov/api/search-fields")
+        response = await client.get("https://ped.uspto.gov/api/search-fields")
         await cls().check_response(response)
         search_fields = response.json()
         cls.search_fields = {k: type_map[v] for k, v in search_fields.items()}
         return cls.search_fields
 
     async def create_query(
         self,
@@ -102,20 +105,20 @@
             "mm": minimum_match,
             "start": str(start),
         }
         if rows:
             params["rows"] = rows
         url = "https://ped.uspto.gov/api/queries"
         logger.debug(f"POST {url}\n{params}")
-        response = await session.post(
+        response = await client.post(
             url,
             json=params,
             headers={"Accept": "application/json"},
         )
         await self.check_response(response)
         return PedsPage.model_validate(response.json())
 
     async def get_documents(self, appl_id: str) -> List[Document]:
         url = f"https://ped.uspto.gov/api/queries/cms/public/{appl_id}"
-        response = await session.get(url)
+        response = await client.get(url)
         await self.check_response(response)
         return [Document.model_validate(d) for d in response.json()]
```

### Comparing `patent_client-4.1.9/patent_client/uspto/peds/api_test.py` & `patent_client-5.0.0/patent_client/_async/uspto/peds/api_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,15 +8,19 @@
     result = await PatentExaminationDataSystemApi().create_query("applId:(16123456)")
     assert result.num_found == 1
     assert result.applications[0].appl_id == "16123456"
 
 
 @pytest.mark.asyncio
 async def test_can_search_by_customer_number():
-    result = await PatentExaminationDataSystemApi().create_query("appCustNumber:(70155)")
+    result = await PatentExaminationDataSystemApi().create_query(
+        "appCustNumber:(70155)"
+    )
     assert result.num_found > 10
 
 
 @pytest.mark.asyncio
 async def test_can_limit_by_rows():
-    result = await PatentExaminationDataSystemApi().create_query("appCustNumber:(70155)", rows=5)
+    result = await PatentExaminationDataSystemApi().create_query(
+        "appCustNumber:(70155)", rows=5
+    )
     assert len(result.applications) == 5
```

### Comparing `patent_client-4.1.9/patent_client/uspto/peds/fixtures/app_1_input.json` & `patent_client-5.0.0/patent_client/_async/uspto/peds/fixtures/app_1_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/peds/fixtures/app_1_output.json` & `patent_client-5.0.0/patent_client/_async/uspto/peds/fixtures/app_1_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/peds/manager.py` & `patent_client-5.0.0/patent_client/_async/uspto/peds/manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import datetime
 import logging
 from collections.abc import Sequence
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import AsyncIterator
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, AsyncIterator
 
 from dateutil.parser import parse as dt_parse
 from pypdf import PdfMerger
 
+from patent_client.util.manager import AsyncManager
+from patent_client.util.request_util import get_start_and_row_count
+
 from .api import PatentExaminationDataSystemApi
 from .query import QueryFields
-from patent_client.util.asyncio_util import run_sync
-from patent_client.util.manager import Manager
-from patent_client.util.request_util import get_start_and_row_count
 
 if TYPE_CHECKING:
-    from .model import USApplication, Document
+    from .model import Document, USApplication
 
 logger = logging.getLogger(__name__)
 
 
 class HttpException(Exception):
     pass
 
 
-def cast_as_datetime(date: str | datetime.datetime | datetime.date, end_of_day=False) -> datetime.datetime:
+def cast_as_datetime(
+    date: str | datetime.datetime | datetime.date, end_of_day=False
+) -> datetime.datetime:
     if isinstance(date, datetime.datetime):
         pass
     elif isinstance(date, str):
         date = dt_parse(date)
     elif isinstance(date, datetime.date):
         date = datetime.datetime.combine(date, datetime.datetime.min.time())
     elif not isinstance(date, datetime.datetime):
@@ -41,54 +42,66 @@
     return date
 
 
 def datetime_to_solr(date: datetime.datetime) -> str:
     return date.strftime("%Y-%m-%dT%H:%M:%SZ")
 
 
-class USApplicationManager(Manager["USApplication"]):
+class USApplicationManager(AsyncManager["USApplication"]):
     default_filter = "appl_id"
 
-    async def alen(self):
+    async def count(self):
         api = PatentExaminationDataSystemApi()
         max_length = (await api.create_query(**self.get_query_params())).num_found
         return min(max_length, self.config.limit) if self.config.limit else max_length
 
-    async def _aget_results(self) -> AsyncIterator["USApplication"]:
+    async def _get_results(self) -> AsyncIterator["USApplication"]:
         query_params = self.get_query_params()
         api = PatentExaminationDataSystemApi()
-        for start, rows in get_start_and_row_count(self.config.limit, self.config.offset, page_size=20):
-            page = await api.create_query(**{**query_params, "start": start, "rows": rows})
+        for start, rows in get_start_and_row_count(
+            self.config.limit, self.config.offset, page_size=20
+        ):
+            page = await api.create_query(
+                **{**query_params, "start": start, "rows": rows}
+            )
             for app in page.applications:
                 yield app
             if len(page.applications) < rows:
                 break
 
     def get_query_params(self):
         # Short circuit processing logic if the "query" filter is specified
         if "query" in self.config.filter:
             query_text = self.config.filter["query"]
         else:
             query = list()
             date_filters = {
-                QueryFields.get(k): v for k, v in self.config.filter.items() if QueryFields.is_date_field(k)
+                QueryFields.get(k): v
+                for k, v in self.config.filter.items()
+                if QueryFields.is_date_field(k)
             }
             non_date_filters = {
-                QueryFields.get(k): v for k, v in self.config.filter.items() if QueryFields.get(k) not in date_filters
+                QueryFields.get(k): v
+                for k, v in self.config.filter.items()
+                if QueryFields.get(k) not in date_filters
             }
 
             date_filter_tuples = list()
             # Check date filters for validity
             for k, v in date_filters.items():
                 if "__" in k:
                     f, *op = k.split("__")
                     if len(op) > 1:
-                        raise ValueError(f"Invalid date filter: {k}={v}; Cannot have more than one operator")
+                        raise ValueError(
+                            f"Invalid date filter: {k}={v}; Cannot have more than one operator"
+                        )
                     if op[0] not in ("gte", "lte"):
-                        raise ValueError(f"Invalid date filter: {k}={v}; Invalid operator: {op[0]}")
+                        raise ValueError(
+                            f"Invalid date filter: {k}={v}; Invalid operator: {op[0]}"
+                        )
                     if isinstance(v, (list, tuple)):
                         raise ValueError(
                             f"Invalid date filter: {k}={v}; Cannot have multiple values with operator {op[0]}"
                         )
                     date_filter_tuples.append((f, op[0], cast_as_datetime(v)))
                 else:
                     if isinstance(v, (list, tuple)):
@@ -100,18 +113,32 @@
                         date_filter_tuples.append((k, "lte", cast_as_datetime(v[1])))
                     else:
                         date_filter_tuples.append((k, "exact", cast_as_datetime(v)))
             # Create pairs of gte/lte filters
             query_date_filter_tuples = set()
             for k, op, v in date_filter_tuples:
                 if op == "gte":
-                    lte_query = next((v for k, op, v in date_filter_tuples if k == k and op == "lte"), "*")
+                    lte_query = next(
+                        (
+                            v
+                            for k, op, v in date_filter_tuples
+                            if k == k and op == "lte"
+                        ),
+                        "*",
+                    )
                     query_date_filter_tuples.add((k, (v, lte_query)))
                 elif op == "lte":
-                    gte_query = next((v for k, op, v in date_filter_tuples if k == k and op == "gte"), "*")
+                    gte_query = next(
+                        (
+                            v
+                            for k, op, v in date_filter_tuples
+                            if k == k and op == "gte"
+                        ),
+                        "*",
+                    )
                     query_date_filter_tuples.add((k, (gte_query, v)))
                 elif op == "exact":
                     query_date_filter_tuples.add((k, (v, v)))
 
             # Create the query string
             for k, v in query_date_filter_tuples:
                 start, end = v
@@ -149,37 +176,31 @@
             query_data["sort"] = sort_query
         return query_data
 
     @property
     def allowed_filters(self):
         return QueryFields.field_names()
 
-    async def ais_online(self):
+    async def is_online(self):
         return await PatentExaminationDataSystemApi.is_online()
 
-    def is_online(self):
-        return run_sync(self.ais_online())
 
-
-class DocumentManager(Manager["Document"]):
+class DocumentManager(AsyncManager["Document"]):
     default_filter = "appl_id"
 
-    async def alen(self):
+    async def count(self):
         return len([i async for i in self])
 
-    async def _aget_results(self) -> AsyncIterator["Document"]:
+    async def _get_results(self) -> AsyncIterator["Document"]:
         api = PatentExaminationDataSystemApi()
-        docs = await api.get_documents(self.config.filter["appl_id"])
+        docs = await api.get_documents(self.config.filter["appl_id"][0])
         for doc in docs:
             yield doc
 
-    def download(self, docs, path="."):
-        run_sync(self.adownload(docs, path))
-
-    async def adownload(self, docs, path="."):
+    async def download(self, docs, path="."):
         if str(path)[-4:].lower() == ".pdf":
             # If we've been given a specific filename, use it
             out_file = Path(path)
         else:
             out_file = Path(path) / "package.pdf"
 
         files = list()
```

### Comparing `patent_client-4.1.9/patent_client/uspto/peds/model.py` & `patent_client-5.0.0/patent_client/_async/uspto/peds/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 import datetime
 from pathlib import Path
-from typing import Iterable
-from typing import List
-from typing import Optional
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Iterable, List, Optional
 
+from async_property import async_property
 from dateutil.relativedelta import relativedelta
-from pydantic import AliasPath
-from pydantic import BeforeValidator
-from pydantic import computed_field
-from pydantic import ConfigDict
-from pydantic import Field
-from pydantic import model_validator
+from pydantic import (
+    AliasPath,
+    BeforeValidator,
+    ConfigDict,
+    Field,
+    computed_field,
+    model_validator,
+)
 from pydantic.alias_generators import to_camel
-from typing_extensions import Annotated
-from typing_extensions import Self
+from typing_extensions import Annotated, Self
 
-from .session import session
-from patent_client.util.asyncio_util import run_sync
-from patent_client.util.pydantic_util import BaseModel
-from patent_client.util.pydantic_util import Date
-from patent_client.util.pydantic_util import DateTime
-from patent_client.util.related import get_model
+from patent_client.util.pydantic_util import BaseModel, Date, DateTime
 
 if TYPE_CHECKING:
-    from patent_client import PtabProceeding, Patent, PublishedApplication
-    from patent_client.epo.ops.published.model import InpadocBiblio
+    from ..public_search.model import Patent, PublishedApplication
+    from ..ptab.model import PtabProceeding
+    from ...epo.ops.published.model import InpadocBiblio
 
 
 def parse_mdy_date(string: str) -> datetime.date:
     try:
         return datetime.datetime.strptime(string, "%m-%d-%Y").date()
     except ValueError:
         return None
 
 
 MDYDate = Annotated[Optional[datetime.date], BeforeValidator(parse_mdy_date)]
 YNBool = Annotated[bool, BeforeValidator(lambda x: x == "Y")]
 OptionalInt = Annotated[Optional[int], BeforeValidator(lambda x: int(x) if x else None)]
-RelationshipStr = Annotated[str, BeforeValidator(lambda x: x.replace("This application ", "").strip())]
-ConveyanceStr = Annotated[str, BeforeValidator(lambda x: x.replace(" (SEE DOCUMENT FOR DETAILS).", ""))]
+RelationshipStr = Annotated[
+    str, BeforeValidator(lambda x: x.replace("This application ", "").strip())
+]
+ConveyanceStr = Annotated[
+    str, BeforeValidator(lambda x: x.replace(" (SEE DOCUMENT FOR DETAILS).", ""))
+]
 
 
 class PEDSBaseModel(BaseModel):
     model_config = ConfigDict(
         alias_generator=to_camel,
         str_strip_whitespace=True,
     )
@@ -234,118 +233,139 @@
 
     @property
     def expiration(self) -> Optional["Expiration"]:
         """Calculates expiration data from which the expiration date can be calculated. See
         help information for the resulting Expiration model.
         """
         if "PCT" in self.appl_id:
-            raise NotImplementedError("Expiration date not supported for PCT Applications")
+            raise NotImplementedError(
+                "Expiration date not supported for PCT Applications"
+            )
         if not self.patent_number:
             return None
         expiration_data = dict()
         term_parents = [
             p
             for p in self.parent_continuity
-            if p.relationship not in ["Claims Priority from Provisional Application", "is a Reissue of"]
+            if p.relationship
+            not in ["Claims Priority from Provisional Application", "is a Reissue of"]
         ]
         if term_parents:
-            term_parent = sorted(term_parents, key=lambda x: x.parent_app_filing_date)[0]
+            term_parent = sorted(term_parents, key=lambda x: x.parent_app_filing_date)[
+                0
+            ]
             relationship = term_parent.relationship
             parent_filing_date = term_parent.parent_app_filing_date
             parent_appl_id = term_parent.parent_appl_id
         else:
             relationship = "self"
             parent_appl_id = self.appl_id
             parent_filing_date = self.app_filing_date
 
         expiration_data["parent_appl_id"] = parent_appl_id
         expiration_data["parent_app_filing_date"] = parent_filing_date
         expiration_data["parent_relationship"] = relationship
         expiration_data["initial_term"] = parent_filing_date + relativedelta(years=20)  # type: ignore
         expiration_data["pta_or_pte"] = self.pta_pte_summary.total_days or 0  # type: ignore
-        expiration_data["extended_term"] = expiration_data["initial_term"] + relativedelta(
-            days=expiration_data["pta_or_pte"]
-        )  # type: ignore
+        expiration_data["extended_term"] = expiration_data[
+            "initial_term"
+        ] + relativedelta(days=expiration_data["pta_or_pte"])  # type: ignore
 
         transactions = self.transactions
         try:
-            disclaimer = next(t for t in transactions if t.code == "DIST")
+            _ = next(t for t in transactions if t.code == "DIST")
             expiration_data["terminal_disclaimer_filed"] = True
         except StopIteration:
             expiration_data["terminal_disclaimer_filed"] = False
 
         return Expiration(**expiration_data)  # type: ignore
 
     # Related objects
     @property
     def documents(self) -> "Iterable[Document]":
         """File History Documents from PEDS CMS"""
-        return get_model("patent_client.uspto.peds.model.Document").objects.filter(appl_id=self.appl_id)
+        return self._get_model(".Document").objects.filter(appl_id=self.appl_id)
 
     @property
     def related_assignments(
         self,
     ) -> "Iterable[Assignment]":
         """Related Assignments from the Assignments API"""
-        return get_model("patent_client.uspto.assignment.model.Assignment").objects.filter(appl_id=self.appl_id)
+        return self._get_model("..assignment.model.Assignment").objects.filter(
+            appl_id=self.appl_id
+        )
 
     @property
     def ptab_proceedings(
         self,
     ) -> "Iterable[PtabProceeding]":
         """Related PtabProceedings for this application"""
-        return get_model("patent_client.uspto.ptab.model.PtabProceeding").objects.filter(appl_id=self.appl_id)
+        return self._get_model("..ptab.model.PtabProceeding").objects.filter(
+            appl_id=self.appl_id
+        )
 
     @property
     def patent(self) -> "Optional[Patent]":
         """Fulltext version of the patent - If Available"""
-        return get_model("patent_client.uspto.fulltext.patent.model.Patent").objects.get(
+        return self._get_model("..public_search.model.Patent").objects.get(
             publication_number=self.patent_number
         )
 
     @property
     def publication(
         self,
     ) -> "Optional[PublishedApplication]":
         """Fulltext version of the Publication - If Available"""
-        return get_model("patent_client.uspto.public_search.model.PublishedApplication").objects.get(
+        return self._get_model(
+            "..public_search.model.PublishedApplication"
+        ).objects.get(
             publication_number=self.publication_number,
         )
 
     @property
     def inpadoc_patent(
         self,
     ) -> "Optional[InpadocBiblio]":
         """Fulltext version of the patent - If Available"""
-        return get_model("patent_client.epo.ops.published.model.InpadocBiblio").objects.get(
+        return self._get_model("...epo.ops.published.model.InpadocBiblio").objects.get(
             publication_number=f"US{self.patent_number}",
         )
 
     @property
     def inpadoc_publication(
         self,
     ) -> "Optional[InpadocBiblio]":
         """Fulltext version of the patent - If Available"""
-        return get_model("patent_client.epo.ops.published.model.InpadocBiblio").objects.get(
+        return self._get_model("...epo.ops.published.model.InpadocBiblio").objects.get(
             publication_number=self.app_early_pub_number,
         )
 
     @model_validator(mode="before")
     @classmethod
     def collect_related_fields(cls, values) -> dict:
         # Collect Correspondent Data
-        correspondent_name_fields = ["corrAddrNameLineOne", "corrAddrNameLineTwo", "corrAddrNameLineThree"]
-        values["corrName"] = " ".join([values[field] for field in correspondent_name_fields if field in values])
+        correspondent_name_fields = [
+            "corrAddrNameLineOne",
+            "corrAddrNameLineTwo",
+            "corrAddrNameLineThree",
+        ]
+        values["corrName"] = " ".join(
+            [values[field] for field in correspondent_name_fields if field in values]
+        )
         correspondent_adddress_lines = "\n".join(
-            values[f] for f in ("corrAddrStreetLineOne", "corrAddrStreetLineTwo") if f in values
+            values[f]
+            for f in ("corrAddrStreetLineOne", "corrAddrStreetLineTwo")
+            if f in values
         )
         correspondent_address_last_line = f"{values.get('corrAddrCity', '')}, {values.get('corrAddrGeoRegionCode', '')} {values.get('corrAddrPostalCode', '')}"
         if "corrAddrCountryName" in values:
             correspondent_address_last_line += f" ({values['corrAddrCountryName']})"
-        values["corrAddress"] = "\n".join([correspondent_adddress_lines, correspondent_address_last_line])
+        values["corrAddress"] = "\n".join(
+            [correspondent_adddress_lines, correspondent_address_last_line]
+        )
         # Collect PTA/PTE Data
         pta_pte_name_fields = (
             "totalPtoDays",
             "ptaPteInd",
             "applDelay",
             "cDelay",
             "ptoAdjustments",
@@ -355,22 +375,26 @@
             "ptoDelay",
         )
         pta_pte_summary = {k: values[k] for k in pta_pte_name_fields if k in values}
         if pta_pte_summary:
             values["ptaPteSummary"] = pta_pte_summary
         # Collect Inventor Names and Addresses
         for inventor in values.get("inventors", list()):
-            inventor["name"] = f"{inventor['nameLineOne']}; {inventor['nameLineTwo']} {inventor['suffix']}".strip()
+            inventor["name"] = (
+                f"{inventor['nameLineOne']}; {inventor['nameLineTwo']} {inventor['suffix']}".strip()
+            )
             inventor["address"] = (
                 "\n".join([inventor["streetOne"], inventor["streetTwo"]])
                 + "\n"
                 + f"{inventor['city']}{inventor['geoCode']} {inventor['country']}"
             )
         for applicant in values.get("applicants", list()):
-            applicant["name"] = f"{applicant['nameLineOne']}; {applicant['nameLineTwo']} {applicant['suffix']}".strip()
+            applicant["name"] = (
+                f"{applicant['nameLineOne']}; {applicant['nameLineTwo']} {applicant['suffix']}".strip()
+            )
             applicant["address"] = (
                 "\n".join([applicant["streetOne"], applicant["streetTwo"]])
                 + "\n"
                 + f"{applicant['city']}{applicant['geoCode']} {applicant['country']}"
             )
 
         return values
@@ -412,33 +436,33 @@
     document_description: str
     document_category: str
     access_level_category: str
     document_identifier: str
     page_count: int
     pdf_url: Optional[str] = None
 
-    def download(self, path: Optional[str | Path]) -> Path:
-        return run_sync(self.adownload(path=path))
+    async def download(self, path: Optional[str | Path]) -> Path:
+        from .api import client
 
-    async def adownload(self, path: Optional[str | Path]) -> Path:
         if self.pdf_url is None:
             raise ValueError("No PDF URL available")
         full_url = f"https://ped.uspto.gov/api/queries/cms/{self.pdf_url}"
-        out_path = await session.adownload(full_url, path=path)
+        out_path = await client.download(full_url, path=path)
         return out_path
 
-    @property
-    def application(self) -> USApplication:
-        return run_sync(self.aapplication)
-
-    @property
-    async def aapplication(self) -> USApplication:
-        return await get_model("patent_client.uspto.peds.model.USApplication").objects.aget(
+    @computed_field
+    @async_property
+    async def application(self) -> USApplication:
+        return await self._get_model(".USApplication").objects.get(
             appl_id=self.application_number_text
         )
 
 
 class PedsPage(PEDSBaseModel):
-    num_found: int = Field(validation_alias=AliasPath("queryResults", "searchResponse", "response", "numFound"))
+    num_found: int = Field(
+        validation_alias=AliasPath(
+            "queryResults", "searchResponse", "response", "numFound"
+        )
+    )
     applications: List[USApplication] = Field(
         validation_alias=AliasPath("queryResults", "searchResponse", "response", "docs")
     )
```

### Comparing `patent_client-4.1.9/patent_client/uspto/peds/query.py` & `patent_client-5.0.0/patent_client/_async/uspto/peds/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from dataclasses import dataclass
-from dataclasses import fields
+from dataclasses import dataclass, fields
 
 
 @dataclass
 class QueryFields:
     app_type_facet: str = "appTypeFacet"
     appl_id: str = "applId"
     total_pto_days: str = "totalPtoDays"
```

### Comparing `patent_client-4.1.9/patent_client/uspto/peds/search_index.csv` & `patent_client-5.0.0/patent_client/_async/uspto/peds/search_index.csv`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/ptab/api.py` & `patent_client-5.0.0/patent_client/_async/uspto/ptab/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import datetime
 import typing as tp
 from typing import Optional
 
 from dateutil.parser import parse as parse_dt
 
-from .model import PtabDecisionPage
-from .model import PtabDocumentPage
-from .model import PtabProceedingPage
-from .session import session
+from patent_client._async.http_client import PatentClientSession
+
+from .model import PtabDecisionPage, PtabDocumentPage, PtabProceedingPage
+
+client = PatentClientSession()
 
 
 def convert_date(obj):
     if isinstance(obj, datetime.datetime):
         return obj.date()
     elif isinstance(obj, str):
         return parse_dt(obj).date()
@@ -58,15 +59,17 @@
 
 
 class PtabApi:
     @classmethod
     async def get_documents(
         cls,
         document_title: Optional[tp.Optional[str]] = None,
-        document_filing_date: Optional[tp.Union[None, datetime.date, tuple[datetime.date], tuple[str]]] = None,
+        document_filing_date: Optional[
+            tp.Union[None, datetime.date, tuple[datetime.date], tuple[str]]
+        ] = None,
         style_name: Optional[tp.Optional[str]] = None,
         filing_party_category: Optional[tp.Optional[str]] = None,
         patent_owner_name: Optional[tp.Optional[str]] = None,
         party_name: Optional[tp.Optional[str]] = None,
         document_number: Optional[tp.Optional[str]] = None,
         document_type: Optional[tp.Optional[str]] = None,
         document_name: Optional[tp.Optional[str]] = None,
@@ -74,15 +77,14 @@
         proceeding_number: Optional[tp.Optional[str]] = None,
         proceeding_type: Optional[tp.Optional[str]] = None,
         application_number: Optional[tp.Optional[str]] = None,
         start: Optional[tp.Optional[int]] = None,
         rows: Optional[tp.Optional[int]] = None,
         sort: Optional[tp.Union[str, tp.List[str], None]] = None,
     ) -> PtabDocumentPage:
-
         query_dict = {
             "documentTitleText": document_title,
             "styleNameText": style_name,
             "filingPartyCategory": filing_party_category,
             "patentOwnerName": patent_owner_name,
             "partyName": party_name,
             "documentNumber": document_number,
@@ -94,45 +96,60 @@
             "applicationNumberText": application_number,
             "recordStartNumber": start,
             "recordTotalQuantity": rows,
             "sortOrderCategory": sort,
         }
         query_dict = {k: v for k, v in query_dict.items() if v is not None}
 
-        query_dict = update_query_with_date(document_filing_date, "documentFiling", query_dict)
-
-        response = await session.get(url="https://developer.uspto.gov/ptab-api/documents", params=query_dict)
+        query_dict = update_query_with_date(
+            document_filing_date, "documentFiling", query_dict
+        )
+
+        response = await client.get(
+            url="https://developer.uspto.gov/ptab-api/documents", params=query_dict
+        )
         response.raise_for_status()
         return PtabDocumentPage.model_validate_json(response.content)
 
     @classmethod
     async def get_proceedings(
         cls,
         proceeding_number: Optional[tp.Optional[str]] = None,
         technology_center_number: Optional[tp.Optional[str]] = None,
         patent_owner: Optional[tp.Optional[str]] = None,
         party_name: Optional[tp.Optional[str]] = None,
         inventor_name: Optional[tp.Optional[str]] = None,
         patent_number: Optional[tp.Optional[str]] = None,
-        declaration_date: Optional[tp.Union[None, datetime.date, tuple[datetime.date], tuple[str]]] = None,
+        declaration_date: Optional[
+            tp.Union[None, datetime.date, tuple[datetime.date], tuple[str]]
+        ] = None,
         style_name: Optional[tp.Optional[str]] = None,
         application_number: Optional[tp.Optional[str]] = None,
         proceeding_status: Optional[tp.Optional[str]] = None,
         proceeding_type: Optional[tp.Optional[str]] = None,
         subproceeding_type: Optional[tp.Optional[str]] = None,
-        institution_date: Optional[tp.Union[None, datetime.date, tuple[datetime.date], tuple[str]]] = None,
-        proceeding_filing_date: Optional[tp.Union[None, datetime.date, tuple[datetime.date], tuple[str]]] = None,
-        accorded_filing_date: Optional[tp.Union[None, datetime.date, tuple[datetime.date], tuple[str]]] = None,
-        proceeding_last_modified_date: Optional[tp.Union[None, datetime.date, tuple[datetime.date], tuple[str]]] = None,
-        grant_date: Optional[tp.Union[None, datetime.date, tuple[datetime.date], tuple[str]]] = None,
+        institution_date: Optional[
+            tp.Union[None, datetime.date, tuple[datetime.date], tuple[str]]
+        ] = None,
+        proceeding_filing_date: Optional[
+            tp.Union[None, datetime.date, tuple[datetime.date], tuple[str]]
+        ] = None,
+        accorded_filing_date: Optional[
+            tp.Union[None, datetime.date, tuple[datetime.date], tuple[str]]
+        ] = None,
+        proceeding_last_modified_date: Optional[
+            tp.Union[None, datetime.date, tuple[datetime.date], tuple[str]]
+        ] = None,
+        grant_date: Optional[
+            tp.Union[None, datetime.date, tuple[datetime.date], tuple[str]]
+        ] = None,
         start: Optional[tp.Optional[int]] = None,
         rows: Optional[tp.Optional[int]] = None,
         sort: Optional[tp.Union[str, tp.List[str], None]] = None,
     ) -> PtabDocumentPage:
-
         query_dict = {
             "proceedingNumber": proceeding_number,
             "technologyCenterNumber": technology_center_number,
             "patentOwnerName": patent_owner,
             "partyName": party_name,
             "inventorName": inventor_name,
             "patentNumber": patent_number,
@@ -144,47 +161,58 @@
             "recordStartNumber": start,
             "recordTotalQuantity": rows,
             "sortOrderCategory": sort,
         }
         query_dict = {k: v for k, v in query_dict.items() if v is not None}
         query_dict = update_query_with_date(declaration_date, "declaration", query_dict)
         query_dict = update_query_with_date(institution_date, "institution", query_dict)
-        query_dict = update_query_with_date(proceeding_filing_date, "proceedingFiling", query_dict)
-        query_dict = update_query_with_date(accorded_filing_date, "accordedFiling", query_dict)
-        query_dict = update_query_with_date(proceeding_last_modified_date, "proceedingLastModified", query_dict)
+        query_dict = update_query_with_date(
+            proceeding_filing_date, "proceedingFiling", query_dict
+        )
+        query_dict = update_query_with_date(
+            accorded_filing_date, "accordedFiling", query_dict
+        )
+        query_dict = update_query_with_date(
+            proceeding_last_modified_date, "proceedingLastModified", query_dict
+        )
         query_dict = update_query_with_date(grant_date, "grant", query_dict)
 
-        response = await session.get(url="https://developer.uspto.gov/ptab-api/proceedings", params=query_dict)
+        response = await client.get(
+            url="https://developer.uspto.gov/ptab-api/proceedings", params=query_dict
+        )
         response.raise_for_status()
         return PtabProceedingPage.model_validate_json(response.content)
 
     @classmethod
     async def get_decisions(
         cls,
         proceeding_number: Optional[tp.Optional[str]] = None,
         decision_type: Optional[tp.Optional[str]] = None,
         subdecision_type: Optional[tp.Optional[str]] = None,
         document_name: Optional[tp.Optional[str]] = None,
-        decision_date: Optional[tp.Union[None, datetime.date, tuple[datetime.date], tuple[str]]] = None,
+        decision_date: Optional[
+            tp.Union[None, datetime.date, tuple[datetime.date], tuple[str]]
+        ] = None,
         style_name: Optional[tp.Optional[str]] = None,
         proceeding_type: Optional[tp.Optional[str]] = None,
         subproceeding_type: Optional[tp.Optional[str]] = None,
         technology_center_number: Optional[tp.Optional[str]] = None,
         document_number: Optional[tp.Optional[str]] = None,
         patent_owner: Optional[tp.Optional[str]] = None,
         party_name: Optional[tp.Optional[str]] = None,
-        grant_date: Optional[tp.Union[None, datetime.date, tuple[datetime.date], tuple[str]]] = None,
+        grant_date: Optional[
+            tp.Union[None, datetime.date, tuple[datetime.date], tuple[str]]
+        ] = None,
         patent_number: Optional[tp.Optional[str]] = None,
         application_number: Optional[tp.Optional[str]] = None,
         text_search: Optional[tp.Optional[str]] = None,
         start: Optional[tp.Optional[int]] = None,
         rows: Optional[tp.Optional[int]] = None,
         sort: Optional[tp.Union[str, tp.List[str], None]] = None,
     ) -> PtabDocumentPage:
-
         query_dict = {
             "proceedingNumber": proceeding_number,
             "decisionTypeCategory": decision_type,
             "subdecisionTypeCategory": subdecision_type,
             "documentName": document_name,
             "styleNameText": style_name,
             "proceedingTypeCategory": proceeding_type,
@@ -200,10 +228,12 @@
             "recordTotalQuantity": rows,
             "sortOrderCategory": sort,
         }
         query_dict = {k: v for k, v in query_dict.items() if v is not None}
         query_dict = update_query_with_date(decision_date, "decision", query_dict)
         query_dict = update_query_with_date(grant_date, "grant", query_dict)
 
-        response = await session.get(url="https://developer.uspto.gov/ptab-api/decisions", params=query_dict)
+        response = await client.get(
+            url="https://developer.uspto.gov/ptab-api/decisions", params=query_dict
+        )
         response.raise_for_status()
         return PtabDecisionPage.model_validate_json(response.content)
```

### Comparing `patent_client-4.1.9/patent_client/uspto/ptab/fixtures/documents_input.json` & `patent_client-5.0.0/patent_client/_async/uspto/ptab/fixtures/documents_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/ptab/fixtures/proceeding_input.json` & `patent_client-5.0.0/patent_client/_async/uspto/ptab/fixtures/proceeding_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/ptab/manager.py` & `patent_client-5.0.0/patent_client/_sync/uspto/ptab/manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,61 @@
+# ********************************************************************************
+# *         WARNING: This file is automatically generated by unasync.py.         *
+# *                             DO NOT MANUALLY EDIT                             *
+# *           Source File: patent_client/_async/uspto/ptab/manager.py            *
+# ********************************************************************************
+
 from copy import deepcopy
-from typing import Callable
-from typing import Generic
-from typing import Optional
+from typing import Callable, Generic, Optional
 
 import inflection
 
+from patent_client.util.manager import Manager, ModelType
+from patent_client.util.request_util import get_start_and_row_count
+
 from .api import PtabApi
-from .model import PtabDecision
-from .model import PtabDocument
-from .model import PtabProceeding
+from .model import PtabDecision, PtabDocument, PtabProceeding
 from .util import peds_to_ptab
-from patent_client.util.manager import Manager
-from patent_client.util.manager import ModelType
-from patent_client.util.request_util import get_start_and_row_count
 
 
 class PtabManager(Manager, Generic[ModelType]):
     url = "https://developer.uspto.gov/ptab-api"
     page_size = 25
     instance_schema = None
     api_method: Optional[Callable] = None
 
-    async def _aget_results(self):
+    def _get_results(self):
         query = deepcopy(self.config.filter)
         query = peds_to_ptab(query)
-        query["sort"] = " ".join(inflection.camelize(o, uppercase_first_letter=False) for o in self.config.order_by)
-        for start, rows in get_start_and_row_count(self.config.limit, self.config.offset, self.page_size):
+        query["sort"] = " ".join(
+            inflection.camelize(o, uppercase_first_letter=False)
+            for o in self.config.order_by
+        )
+        for start, rows in get_start_and_row_count(
+            self.config.limit, self.config.offset, self.page_size
+        ):
             query["start"] = start
             query["rows"] = rows
-            page = await self.api_method(**query)
+            page = self.api_method(**query)
             for doc in page.docs:
                 yield doc
             if len(page.docs) < rows:
                 break
 
-    async def alen(self):
-        page = await self.api_method(**peds_to_ptab(self.config.filter))
-        return min(self.config.limit, page.num_found) if self.config.limit else page.num_found
-
-    def allowed_filters(self):
-        params = schema_doc["paths"][self.path]["get"]["parameters"]
-        return {inflection.underscore(p["name"]): p["description"] for p in params}
+    def count(self):
+        page = self.api_method(**peds_to_ptab(self.config.filter))
+        return (
+            min(self.config.limit, page.num_found)
+            if self.config.limit
+            else page.num_found
+        )
+
+    # def allowed_filters(self):
+    #    params = schema_doc["paths"][self.path]["get"]["parameters"]
+    #    return {inflection.underscore(p["name"]): p["description"] for p in params}
 
 
 class PtabProceedingManager(PtabManager[PtabProceeding]):
     path = "/proceedings"
     default_filter = "proceeding_number"
     api_method = PtabApi.get_proceedings
```

### Comparing `patent_client-4.1.9/patent_client/uspto/ptab/manager_test.py` & `patent_client-5.0.0/patent_client/_async/uspto/ptab/manager_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,123 +1,66 @@
 import pytest
 
-from .model import PtabDecision
-from .model import PtabDocument
-from .model import PtabProceeding
+from .model import PtabDecision, PtabDocument, PtabProceeding
 
 
 class TestPtabProceeding:
-    def test_get_by_proceeding_number(self):
-        result = PtabProceeding.objects.get("IPR2016-00831")
-        assert result.respondent_patent_number == "6162705"
-
-    def test_get_by_patent_number(self):
-        result = PtabProceeding.objects.get(patent_number="6103599")
-        assert result.proceeding_number == "IPR2016-00833"
-
-    def test_get_by_application_number(self):
-        result = PtabProceeding.objects.get(appl_id="09089931")
-        assert result.proceeding_number == "IPR2016-00833"
-
-    def test_filter_by_party(self):
-        result = PtabProceeding.objects.filter(party_name="Apple")
-        assert len(result) >= 400
-        assert result.count() >= 400
-
-    def test_filter_with_limit(self):
-        result = PtabProceeding.objects.filter(party_name="Apple").limit(26)
-        assert len(result) == 26
-        objects = list(result)
-        assert len(objects) == 26
-
-    def test_offset(self):
-        result = PtabProceeding.objects.filter(party_name="Apple").limit(3)
-        objects = list(result)
-        assert result.first() == objects[0]
-        assert result.offset(1).first() == objects[1]
-        assert result.offset(1).offset(1).first() == objects[2]
-
-
-class TestPtabDocument:
-    def test_filter_by_proceeding(self):
-        result = PtabDocument.objects.filter(proceeding_number="IPR2016-00831")
-        assert len(result) == 77
-
-    def test_sort_by_document_number(self):
-        result = (
-            PtabDocument.objects.filter(proceeding_number="IPR2016-00831")
-            .order_by("document_number")
-            .limit(3)
-            .values_list("document_number", flat=True)
-            .to_list()
-        )
-        assert len(result) == 3
-        objects = list(result)
-        assert objects == list(sorted(objects))
-
-
-class TestPtabDecision:
-    def test_get_by_proceeding(self):
-        result = PtabDecision.objects.get(proceeding_number="IPR2016-00831")
-        assert result.identifier == "a44c5f1557b7b60d00e66604d3668ce442d53f964aa597011cc476b4"
-
-
-class TestPtabProceedingAsync:
     @pytest.mark.asyncio
     async def test_get_by_proceeding_number(self):
-        result = await PtabProceeding.objects.aget("IPR2016-00831")
+        result = await PtabProceeding.objects.get("IPR2016-00831")
         assert result.respondent_patent_number == "6162705"
 
     @pytest.mark.asyncio
     async def test_get_by_patent_number(self):
-        result = await PtabProceeding.objects.aget(patent_number="6103599")
+        result = await PtabProceeding.objects.get(patent_number="6103599")
         assert result.proceeding_number == "IPR2016-00833"
 
     @pytest.mark.asyncio
     async def test_get_by_application_number(self):
-        result = await PtabProceeding.objects.aget(appl_id="09089931")
+        result = await PtabProceeding.objects.get(appl_id="09089931")
         assert result.proceeding_number == "IPR2016-00833"
 
     @pytest.mark.asyncio
     async def test_filter_by_party(self):
         result = PtabProceeding.objects.filter(party_name="Apple")
-        assert await result.alen() >= 400
+        assert await result.count() >= 400
 
     @pytest.mark.asyncio
     async def test_filter_with_limit(self):
         result = PtabProceeding.objects.filter(party_name="Apple").limit(26)
-        assert await result.alen() == 26
-        objects = await result.ato_list()
+        assert await result.count() == 26
+        objects = [a async for a in result]
         assert len(objects) == 26
 
     @pytest.mark.asyncio
     async def test_offset(self):
         result = PtabProceeding.objects.filter(party_name="Apple").limit(3)
-        objects = await result.ato_list()
-        assert await result.afirst() == objects[0]
-        assert await result.offset(1).afirst() == objects[1]
-        assert await result.offset(1).offset(1).afirst() == objects[2]
+        objects = [a async for a in result]
+        assert await result.first() == objects[0]
+        assert await result.offset(1).first() == objects[1]
+        assert await result.offset(1).offset(1).first() == objects[2]
 
 
-class TestPtabDocumentAsync:
+class TestPtabDocument:
     @pytest.mark.asyncio
     async def test_filter_by_proceeding(self):
         result = PtabDocument.objects.filter(proceeding_number="IPR2016-00831")
-        assert await result.alen() == 77
+        assert await result.count() == 77
 
     @pytest.mark.asyncio
     async def test_sort_by_document_number(self):
-        result = await (
-            PtabDocument.objects.filter(proceeding_number="IPR2016-00831")
-            .order_by("document_number")
+        result = (
+            await PtabDocument.objects.filter(proceeding_number="IPR2016-00831")
             .limit(3)
-            .values_list("document_number", flat=True)
-            .ato_list()
+            .count()
         )
-        assert len(result) == 3
+        assert result == 3
 
 
-class TestPtabDecisionAsync:
+class TestPtabDecision:
     @pytest.mark.asyncio
     async def test_get_by_proceeding(self):
-        result = await PtabDecision.objects.aget(proceeding_number="IPR2016-00831")
-        assert result.identifier == "a44c5f1557b7b60d00e66604d3668ce442d53f964aa597011cc476b4"
+        result = await PtabDecision.objects.get(proceeding_number="IPR2016-00831")
+        assert (
+            result.identifier
+            == "a44c5f1557b7b60d00e66604d3668ce442d53f964aa597011cc476b4"
+        )
```

### Comparing `patent_client-4.1.9/patent_client/uspto/ptab/model.py` & `patent_client-5.0.0/patent_client/_async/uspto/ptab/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 import datetime
 import re
 from pathlib import Path
-from typing import List
-from typing import Optional
-from typing import TYPE_CHECKING
-
-from pydantic import BeforeValidator
-from pydantic import ConfigDict
-from pydantic import Field
+from typing import TYPE_CHECKING, List, Optional
+
+from pydantic import BeforeValidator, ConfigDict, Field
 from pydantic.alias_generators import to_camel
 from typing_extensions import Annotated
 
-from ...util.related import get_model
-from .session import session
-from patent_client.util.asyncio_util import run_sync
-from patent_client.util.pydantic_util import BaseModel
-from patent_client.util.pydantic_util import DateTime
+from patent_client.util.pydantic_util import BaseModel, DateTime
 
 if TYPE_CHECKING:
-    from patent_client.uspto.peds.model import USApplication
+    from ..peds.model import USApplication
 
-MDYDate = Annotated[datetime.date, BeforeValidator(lambda x: datetime.datetime.strptime(x, "%m-%d-%Y").date())]
+MDYDate = Annotated[
+    datetime.date,
+    BeforeValidator(lambda x: datetime.datetime.strptime(x, "%m-%d-%Y").date()),
+]
 
 
 class PtabBaseModel(BaseModel):
     model_config = ConfigDict(
         alias_generator=to_camel,
         str_strip_whitespace=True,
     )
@@ -115,33 +110,33 @@
     additional_respondents: List[str] = Field(default_factory=list)
 
     @property
     def documents(
         self,
     ) -> "list[PtabDocument]":
         """Documents associated with the Proceeding"""
-        return get_model("patent_client.uspto.ptab.model.PtabDocument").objects.filter(
+        return self._get_model(".model.PtabDocument").objects.filter(
             proceeding_number=self.proceeding_number
         )
 
     @property
     def decisions(
         self,
     ) -> "list[PtabDecision]":
         """Decisions associated with the Proceeding"""
-        return get_model("patent_client.uspto.ptab.model.PtabDecision").objects.filter(
+        return self._get_model(".model.PtabDecision").objects.filter(
             proceeding_number=self.proceeding_number
         )
 
     @property
     def us_application(
         self,
     ) -> "list[USApplication]":
         """The US Application provided by PEDS associated with the Proceeding"""
-        return get_model("patent_client.uspto.peds.model.USApplication").objects.get(
+        return self._get_model(".model.USApplication").objects.get(
             patent_number=self.respondent_patent_number
         )
 
 
 fname_re = re.compile(r"[<>:\"/\|?*]")
 
 
@@ -155,53 +150,51 @@
     proceeding_number: Optional[str] = None
     proceeding_type_category: Optional[str] = Field(repr=False, default=None)
     title: Optional[str] = None
 
     @property
     def proceeding(self) -> "PtabProceeding":
         """The PTAB proceeding associated with the document"""
-        return get_model("patent_client.uspto.ptab.model.PtabProceeding").objects.get(
+        return self._get_model(".model.PtabProceeding").objects.get(
             proceeding_number=self.proceeding_number
         )
 
-    def download(self, path: Optional[str | Path]) -> Path:
-        return run_sync(self.adownload(path))
+    async def download(self, path: Optional[str | Path]) -> Path:
+        from .api import client
 
-    async def adownload(self, path: Optional[str | Path]) -> Path:
         name, ext = self.document_name.rsplit(".", 1)
         name = name[:100] + "." + ext
         filename = f"[{str(self.document_number).rjust(4, '0')}] {self.document_filing_date.isoformat()} - {name}"
         filename = filename.encode(encoding="ascii", errors="ignore").decode("ascii")
         filename = fname_re.sub("", filename)
         out_path = Path(path) if path else Path.cwd()
         if out_path.is_dir():
             out_path = Path(path) / filename
         else:
             out_path = out_path
-        donwload_url = f"https://developer.uspto.gov/ptab-api/documents/{self.document_identifier}/download"
-        return await session.download(download_url, path=out_path)
+        download_url = f"https://developer.uspto.gov/ptab-api/documents/{self.document_identifier}/download"
+        return await client.download(download_url, path=out_path)
 
 
 class PtabDecision(PtabBaseModel):
-    __manager__ = "patent_client.uspto.ptab.manager.PtabDecisionManager"
     proceeding_number: str
     board_rulings: List[str] = Field(default_factory=list)
     decision_type_category: Optional[str] = None
     document_identifier: Optional[str] = None
     document_name: Optional[str] = None
     identifier: Optional[str] = None
     subdecision_type_category: Optional[str] = None
     issue_type: List[str] = Field(default_factory=list)
     object_uu_id: Optional[str] = None
     petitioner_technology_center_number: Optional[str] = None
 
     @property
     def proceeding(self) -> "PtabProceeding":
         """The PTAB proceeding associated with the document"""
-        return get_model("patent_client.uspto.ptab.model.PtabProceeding").objects.get(
+        return self._get_model(".model.PtabProceeding").objects.get(
             proceeding_number=self.proceeding_number
         )
 
 
 class PtabDocumentPage(PtabBaseModel):
     num_found: Optional[int] = Field(alias="recordTotalQuantity")
     docs: List[PtabDocument] = Field(alias="results", default_factory=list)
```

### Comparing `patent_client-4.1.9/patent_client/uspto/public_search/api.py` & `patent_client-5.0.0/patent_client/_sync/uspto/public_search/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,22 @@
+# ********************************************************************************
+# *         WARNING: This file is automatically generated by unasync.py.         *
+# *                             DO NOT MANUALLY EDIT                             *
+# *         Source File: patent_client/_async/uspto/public_search/api.py         *
+# ********************************************************************************
+
 import asyncio
+import json
+from copy import deepcopy
 from pathlib import Path
-
 import httpx
 
-from .model import PublicSearchBiblioPage
-from .model import PublicSearchDocument
-from .session import session
+from patent_client._sync.http_client import PatentClientSession
+
+from .model import PublicSearchBiblioPage, PublicSearchDocument
 
 
 class UsptoException(Exception):
     pass
 
 
 def force_list(obj):
@@ -18,145 +25,168 @@
             obj,
         ]
     return obj
 
 
 class PublicSearchApi:
     def __init__(self):
+        self.client = PatentClientSession(
+            headers={
+                "X-Requested-With": "XMLHttpRequest",
+                "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36",
+            },
+            http2=True,
+            follow_redirects=True,
+        )
         self.session = dict()
         self.case_id = None
+        self.queries = dict()
+        self.search_query = json.loads(
+            (Path(__file__).parent / "search_query.json").read_text()
+        )
 
-    async def run_query(
+    def run_query(
         self,
         query,
         start=0,
         limit=500,
         sort="date_publ desc",
         default_operator="OR",
         sources=["US-PGPUB", "USPAT", "USOCR"],
         expand_plurals=True,
         british_equivalents=True,
-    ) -> "PublicSearch":
+    ) -> "PublicSearchBiblioPage":
         if self.case_id is None:
-            await self.get_session()
-        url = "https://ppubs.uspto.gov/dirsearch-public/searches/searchWithBeFamily"
-        data = {
-            "start": start,
-            "pageCount": limit,
-            "sort": sort,
-            "docFamilyFiltering": "familyIdFiltering",
-            "searchType": 1,
-            "familyIdEnglishOnly": True,
-            "familyIdFirstPreferred": "US-PGPUB",
-            "familyIdSecondPreferred": "USPAT",
-            "familyIdThirdPreferred": "FPRS",
-            "showDocPerFamilyPref": "showEnglish",
-            "queryId": 0,
-            "tagDocSearch": False,
-            "query": {
-                "caseId": self.case_id,
-                "hl_snippets": "2",
-                "op": default_operator,
-                "q": query,
-                "queryName": query,
-                "highlights": "1",
-                "qt": "brs",
-                "spellCheck": False,
-                "viewName": "tile",
-                "plurals": expand_plurals,
-                "britishEquivalents": british_equivalents,
-                "databaseFilters": [],
-                "searchType": 1,
-                "ignorePersist": True,
-                "userEnteredQuery": query,
-            },
-        }
-        for s in force_list(sources):
-            data["query"]["databaseFilters"].append({"databaseName": s, "countryCodes": []})
-        query_response = await session.post(url, json=data, extensions={"force_cache": True})
-        if query_response.status_code in (500, 415):  # Just need to retry
-            await asyncio.sleep(5)
-            query_response = await session.post(url, json=data, extensions={"force_cache": True})
-        elif query_response.status_code == 403:  # Session must be refreshed
-            await self.get_session()
-            query_response = await session.post(url, json=data, extensions={"force_cache": True})
+            self.get_session()
+
+        data = deepcopy(self.search_query)
+        data["start"] = start
+        data["pageCount"] = limit
+        data["sort"] = sort
+        data["query"]["caseId"] = self.case_id
+        data["query"]["op"] = default_operator
+        data["query"]["q"] = query
+        data["query"]["queryName"] = query
+        data["query"]["userEnteredQuery"] = query
+        data["query"]["databaseFilters"] = [
+            {"databaseName": s, "countryCodes": []} for s in sources
+        ]
+        data["query"]["plurals"] = expand_plurals
+        data["query"]["britishEquivalents"] = british_equivalents
+
+        counts = self.make_request(
+            "POST",
+            "https://ppubs.uspto.gov/dirsearch-public/searches/counts",
+            json=data["query"],
+        )
+        counts.raise_for_status()
+        search_url = (
+            "https://ppubs.uspto.gov/dirsearch-public/searches/searchWithBeFamily"
+        )
+        query_response = self.make_request("POST", search_url, json=data)
         query_response.raise_for_status()
         result = query_response.json()
         if result.get("error", None) is not None:
-            raise UsptoException(f"Error #{result['error']['errorCode']}\n{result['error']['errorMessage']}")
+            raise UsptoException(
+                f"Error #{result['error']['errorCode']}\n{result['error']['errorMessage']}"
+            )
         return PublicSearchBiblioPage.model_validate(result)
 
-    async def get_document(self, bib) -> "PublicSearchDocument":
-        url = f"https://ppubs.uspto.gov/dirsearch-public/patents/{bib.guid}/highlight"
+    def make_request(self, method, url, **kwargs):
+        response = self.client.request(method, url, **kwargs)
+        if response.status_code == 403:
+            self.get_session()
+            response = self.client.request(method, url, **kwargs)
+        if response.status_code == 429:
+            wait_time = int(response.headers["x-rate-limit-retry-after-seconds"]) + 1
+            asyncio.sleep(wait_time)
+            response = self.client.request(method, url, **kwargs)
+        return response
+
+    def get_document(self, bib) -> "PublicSearchDocument":
+        url = f"https://ppubs.uspto.gov/dirsearch-public/internal/patents/{bib.guid}/highlight"
         params = {
             "queryId": 1,
             "source": bib.type,
             "includeSections": True,
             "uniqueId": None,
         }
-        response = await session.get(url, params=params)
+        response = self.make_request("GET", url, params=params)
         response.raise_for_status()
         return PublicSearchDocument.model_validate(response.json())
 
-    async def get_session(self):
+    def get_session(self):
+        self.client.cookies = httpx.Cookies()
+        response = self.client.get("https://ppubs.uspto.gov/pubwebapp/")
         url = "https://ppubs.uspto.gov/dirsearch-public/users/me/session"
-        response = await session.post(
-            url, json=-1, extensions={"cache_disabled": True}
+        response = self.client.post(
+            url,
+            json=-1,
+            headers={
+                "X-Access-Token": "null",
+                "referer": "https://ppubs.uspto.gov/pubwebapp/",
+            },
         )  # json=str(random.randint(10000, 99999)))
         self.session = response.json()
         self.case_id = self.session["userCase"]["caseId"]
+        self.access_token = response.headers["X-Access-Token"]
+        self.client.headers["X-Access-Token"] = self.access_token
         return self.session
 
-    async def _request_save(self, obj):
-        page_keys = [f"{obj.image_location}/{i:0>8}.tif" for i in range(1, obj.document_structure.page_count + 1)]
-        response = await session.post(
+    def _request_save(self, obj):
+        page_keys = [
+            f"{obj.image_location}/{i:0>8}.tif"
+            for i in range(1, obj.document_structure.page_count + 1)
+        ]
+        response = self.client.post(
             "https://ppubs.uspto.gov/dirsearch-public/print/imageviewer",
             json={
                 "caseId": self.case_id,
                 "pageKeys": page_keys,
                 "patentGuid": obj.guid,
                 "saveOrPrint": "save",
                 "source": obj.type,
             },
         )
         if response.status_code == 500:
             raise UsptoException(response.text)
         return response.text
 
-    async def download_image(self, obj, path="."):
+    def download_image(self, obj, path="."):
         out_path = Path(path).expanduser() / f"{obj.guid}.pdf"
         if out_path.exists():
             return out_path
         if self.case_id is None:
-            await self.get_session()
+            self.get_session()
         try:
-            print_job_id = await self._request_save(obj)
+            print_job_id = self._request_save(obj)
         except httpx.HTTPStatusError:
-            await self.get_session()
-            print_job_id = await self._request_save(obj)
+            self.get_session()
+            print_job_id = self._request_save(obj)
         while True:
-            response = await session.post(
+            response = self.client.post(
                 "https://ppubs.uspto.gov/dirsearch-public/print/print-process",
                 json=[
                     print_job_id,
                 ],
             )
             response.raise_for_status()
             print_data = response.json()
             if print_data[0]["printStatus"] == "COMPLETED":
                 break
-            await asyncio.sleep(1)
+            asyncio.sleep(1)
         pdf_name = print_data[0]["pdfName"]
         with out_path.open("wb") as f:
             try:
-                request = session.build_request(
-                    "GET", f"https://ppubs.uspto.gov/dirsearch-public/print/save/{pdf_name}"
+                request = self.client.build_request(
+                    "GET",
+                    f"https://ppubs.uspto.gov/dirsearch-public/print/save/{pdf_name}",
                 )
-                response = await session.send(request, stream=True)
+                response = self.client.send(request, stream=True)
                 response.raise_for_status()
-                async for chunk in response.aiter_bytes():
+                for chunk in response.iter_bytes():
                     if chunk:
                         f.write(chunk)
             except httpx.HTTPStatusError as e:
-                await response.aclose()
+                response.close()
                 raise e
         return out_path
```

### Comparing `patent_client-4.1.9/patent_client/uspto/public_search/convert/biblio.py` & `patent_client-5.0.0/patent_client/_async/uspto/public_search/convert/biblio.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from yankee.json.schema import fields as f
 from yankee.json.schema import Schema
+from yankee.json.schema import fields as f
 
 from .shared import DocumentStructureSchema
 
 
 class PublicSearchBiblioSchema(Schema):
     guid = f.String("guid")
 
@@ -22,15 +22,17 @@
     primary_examiner = f.String("primaryExaminer")
     assistant_examiner = f.List(f.String, "assistantExaminer")
 
     main_classification_code = f.String("mainClassificationCode")
     cpc_additional = f.DelimitedString(f.Str(), "cpcAdditionalFlattened", delimeter=";")
     cpc_inventive = f.DelimitedString(f.Str(), "cpcInventiveFlattened", delimeter=";")
     ipc_code = f.DelimitedString(f.Str(), "ipcCodeFlattened", delimeter=";")
-    uspc_full_classification = f.DelimitedString(f.Str(), "uspcFullClassificationFlattened", delimeter=";")
+    uspc_full_classification = f.DelimitedString(
+        f.Str(), "uspcFullClassificationFlattened", delimeter=";"
+    )
 
     image_file_name = f.String("imageFileName")
     image_location = f.String("imageLocation")
     document_structure = DocumentStructureSchema(data_key=False)
 
     type = f.String("type")
     database_name = f.String("databaseName")
```

### Comparing `patent_client-4.1.9/patent_client/uspto/public_search/convert/document.py` & `patent_client-5.0.0/patent_client/_async/uspto/public_search/convert/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import datetime
 
+from yankee.json.schema import RegexSchema, Schema, ZipSchema
 from yankee.json.schema import fields as f
-from yankee.json.schema import RegexSchema
-from yankee.json.schema import Schema
-from yankee.json.schema import ZipSchema
+
+from patent_client.util.claims.parser import ClaimsParser
 
 from ..util import html_to_text
 from .shared import DocumentStructureSchema
-from patent_client.util.claims.parser import ClaimsParser
 
 
 def parse_claims(html):
     text = html_to_text(html)
     if text:
         try:
             return ClaimsParser().parse(text)
@@ -34,35 +33,43 @@
 class UsReferenceSchema(ZipSchema):
     publication_number = f.String("urpn")
     # us_class = f.String("usRefClassification")
     # cpc_class = f.String("usRefCpcClassification")
     # group = f.String("usRefGroup")
     pub_month = f.Date(
         "usRefIssueDate",
-        dt_converter=lambda s: datetime.datetime(year=int(s[:4]), month=int(s[4:6]), day=1),
+        dt_converter=lambda s: datetime.datetime(
+            year=int(s[:4]), month=int(s[4:6]), day=1
+        ),
     )
     patentee_name = f.String("usRefPatenteeName")
     cited_by_examiner = f.Boolean("usRefGroup", true_func=lambda s: "examiner" in s)
 
 
 class ForeignReferenceSchema(ZipSchema):
     citation_classification = f.String("foreignRefCitationClassification")
     citation_cpc = f.String("foreignRefCitationCpc")
     country_code = f.String("foreignRefCountryCode")
     # group = f.String("foreignRefGroup")
     patent_number = f.String("foreignRefPatentNumber")
     pub_month = f.Date(
         "foreignRefPubDate",
-        dt_converter=lambda s: datetime.datetime(year=int(s[:4]), month=int(s[4:6]), day=1),
+        dt_converter=lambda s: datetime.datetime(
+            year=int(s[:4]), month=int(s[4:6]), day=1
+        ),
+    )
+    cited_by_examiner = f.Boolean(
+        "foreignRefGroup", true_func=lambda s: "examiner" in s
     )
-    cited_by_examiner = f.Boolean("foreignRefGroup", true_func=lambda s: "examiner" in s)
 
 
 class NplReferenceSchema(RegexSchema):
-    __regex__ = r"(?P<citation>.*)(?P<cited_by_examiner>cited by (applicant|examiner).?$)"
+    __regex__ = (
+        r"(?P<citation>.*)(?P<cited_by_examiner>cited by (applicant|examiner).?$)"
+    )
     citation = f.String()
     cited_by_examiner = f.Bool(true_func=lambda s: "examiner" in s)
 
 
 class RelatedApplicationSchema(ZipSchema):
     child_patent_country = f.String("relatedApplChildPatentCountry")
     child_patent_number = f.String("relatedApplChildPatentNumber")
@@ -159,22 +166,30 @@
     composite_id = f.String("compositeId")
     database_name = f.String("databaseName")
     derwent_week_int = f.Integer("derwentWeekInt")
 
     # References Cited
     us_references = UsReferenceSchema(data_key=False)
     foreign_references = ForeignReferenceSchema(data_key=False)
-    npl_references = f.DelimitedString(NplReferenceSchema, "otherRefPub.0", delimeter="<br />")
+    npl_references = f.DelimitedString(
+        NplReferenceSchema, "otherRefPub.0", delimeter="<br />"
+    )
 
     # Classifications
     cpc_inventive = f.List(CpcCodeSchema)
     cpc_additional = f.List(CpcCodeSchema)
 
     intl_class_issued = f.DelimitedString(f.String, "ipcCodeFlattened", delimeter=";")
-    intl_class_current_primary = f.List(IntlCodeSchema, "curIntlPatentClassificationPrimary")
-    intl_class_currrent_secondary = f.List(IntlCodeSchema, "curIntlPatentClassificationSecondary")
+    intl_class_current_primary = f.List(
+        IntlCodeSchema, "curIntlPatentClassificationPrimary"
+    )
+    intl_class_currrent_secondary = f.List(
+        IntlCodeSchema, "curIntlPatentClassificationSecondary"
+    )
 
-    us_class_current = f.DelimitedString(f.Str(), "uspcFullClassificationFlattened", delimeter=";")
+    us_class_current = f.DelimitedString(
+        f.Str(), "uspcFullClassificationFlattened", delimeter=";"
+    )
     us_class_issued = f.List(f.Str, "issuedUsClassificationFull")
 
     field_of_search_us = f.List(f.Str(), "fieldOfSearchClassSubclassHighlights")
     field_of_search_cpc = f.List(f.Str(), "fieldOfSearchCpcClassification")
```

### Comparing `patent_client-4.1.9/patent_client/uspto/public_search/convert/shared.py` & `patent_client-5.0.0/patent_client/_async/uspto/public_search/convert/shared.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from yankee.json import fields as f
 from yankee.json import Schema
+from yankee.json import fields as f
 
 
 class DocumentStructureSchema(Schema):
     number_of_claims = f.Integer("numberOfClaims")
     number_of_drawing_sheets = f.Integer("numberOfDrawingSheets")
     number_of_figures = f.Integer("numberOfFigures")
     page_count = f.Integer("pageCount")
```

### Comparing `patent_client-4.1.9/patent_client/uspto/public_search/convert_test.py` & `patent_client-5.0.0/patent_client/_async/uspto/public_search/convert_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/public_search/fixtures/biblio.json` & `patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/public_search/fixtures/biblio_convert.json` & `patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/biblio_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/public_search/fixtures/biblio_output.json` & `patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/biblio_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/public_search/fixtures/doc.json` & `patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/doc.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/public_search/fixtures/doc_convert.json` & `patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/doc_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/public_search/fixtures/doc_output.json` & `patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/doc_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/public_search/manager.py` & `patent_client-5.0.0/patent_client/_async/uspto/public_search/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from typing import AsyncIterator
-from typing import Generic
-from typing import TypeVar
+from typing import AsyncIterator, Generic, TypeVar
+
+from patent_client.util.manager import AsyncManager
+from patent_client.util.request_util import get_start_and_row_count
 
 from .api import PublicSearchApi
-from .model import Patent
-from .model import PatentBiblio
-from .model import PublicSearchBiblio
-from .model import PublicSearchDocument
-from .model import PublishedApplication
-from .model import PublishedApplicationBiblio
+from .model import (
+    Patent,
+    PatentBiblio,
+    PublicSearchBiblio,
+    PublicSearchDocument,
+    PublishedApplication,
+    PublishedApplicationBiblio,
+)
 from .query import QueryBuilder
-from patent_client.util.manager import Manager
-from patent_client.util.request_util import get_start_and_row_count
 
 
 class CapacityException(Exception):
     pass
 
 
 class FinishedException(Exception):
@@ -23,15 +24,15 @@
 
 
 T = TypeVar("T")
 
 public_search_api = PublicSearchApi()
 
 
-class GenericPublicSearchManager(Manager, Generic[T]):
+class GenericPublicSearchManager(AsyncManager, Generic[T]):
     page_size = 500
     default_filter = "patent_number"
     query_builder = QueryBuilder()
 
     @property
     def _query(self):
         return self.query_builder.build_query(self.config)
@@ -44,31 +45,33 @@
     def query_fields(self):
         return self.query_builder.search_keywords
 
     @property
     def order_by_fields(self):
         return self.query_builder.order_by_keywords
 
-    async def alen(self):
+    async def count(self):
         query = self._query
         order_by = self._order_by
         sources = self.config.options.get("sources", ["US-PGPUB", "USPAT", "USOCR"])
         page = await public_search_api.run_query(
             query=query, start=0, limit=self.page_size, sort=order_by, sources=sources
         )
         max_len = page.num_found - self.config.offset
         return min(self.config.limit, max_len) if self.config.limit else max_len
 
 
 class GenericPublicSearchBiblioManager(GenericPublicSearchManager, Generic[T]):
-    async def _aget_results(self) -> AsyncIterator[T]:
+    async def _get_results(self) -> AsyncIterator[T]:
         query = self._query
         order_by = self._order_by
         sources = self.config.options.get("sources", ["US-PGPUB", "USPAT", "USOCR"])
-        for start, rows in get_start_and_row_count(self.config.limit, self.config.offset, self.page_size):
+        for start, rows in get_start_and_row_count(
+            self.config.limit, self.config.offset, self.page_size
+        ):
             page = await public_search_api.run_query(
                 query=query,
                 start=start,
                 limit=rows,
                 sort=order_by,
                 sources=sources,
             )
@@ -78,30 +81,32 @@
                 break
 
 
 capacity_limit = 501
 
 
 class GenericPublicSearchDocumentManager(GenericPublicSearchBiblioManager, Generic[T]):
-    async def _aget_results(self) -> AsyncIterator["PublicSearchDocument"]:
-        result_count = super().__len__()
+    async def _get_results(self) -> AsyncIterator["PublicSearchDocument"]:
+        result_count = await super().count()
         if result_count > capacity_limit:
             raise CapacityException(
-                f"Query would result in more than 20 results! ({result_count} > 20).\nPlease use the associated Biblio method to reduce load on the API (PublicSearch / PatentBiblio / PublishedApplicationBiblio"
+                f"Query would result in more than 501 results! ({result_count} > 20).\nPlease use the associated Biblio method to reduce load on the API (PublicSearch / PatentBiblio / PublishedApplicationBiblio"
             )
-        async for obj in super()._aget_results():
+        async for obj in super()._get_results():
             doc = await public_search_api.get_document(obj)
             yield doc
 
 
 class PublicSearchBiblioManager(GenericPublicSearchBiblioManager[PublicSearchBiblio]):
     pass
 
 
-class PublicSearchDocumentManager(GenericPublicSearchDocumentManager[PublicSearchDocument]):
+class PublicSearchDocumentManager(
+    GenericPublicSearchDocumentManager[PublicSearchDocument]
+):
     pass
 
 
 class PatentBiblioManager(GenericPublicSearchBiblioManager[PatentBiblio]):
     def __init__(self, config=None):
         super().__init__(config=config)
         self.config.options["sources"] = [
@@ -113,21 +118,25 @@
     def __init__(self, config=None):
         super().__init__(config=config)
         self.config.options["sources"] = [
             "USPAT",
         ]
 
 
-class PublishedApplicationBiblioManager(GenericPublicSearchBiblioManager[PublishedApplicationBiblio]):
+class PublishedApplicationBiblioManager(
+    GenericPublicSearchBiblioManager[PublishedApplicationBiblio]
+):
     def __init__(self, config=None):
         super().__init__(config=config)
         self.config.options["sources"] = [
             "US-PGPUB",
         ]
 
 
-class PublishedApplicationManager(GenericPublicSearchDocumentManager[PublishedApplication]):
+class PublishedApplicationManager(
+    GenericPublicSearchDocumentManager[PublishedApplication]
+):
     def __init__(self, config=None):
         super().__init__(config=config)
         self.config.options["sources"] = [
             "US-PGPUB",
         ]
```

### Comparing `patent_client-4.1.9/patent_client/uspto/public_search/model/biblio.py` & `patent_client-5.0.0/patent_client/_async/uspto/public_search/model/biblio.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,77 +1,88 @@
 import datetime
 from typing import Optional
 
-from pydantic import AliasPath
-from pydantic import Field
-from pydantic import model_validator
+from pydantic import AliasPath, Field, model_validator
 
-from ..convert.biblio import PublicSearchBiblioPageSchema
-from .shared import ApplicationNumber
-from .shared import DateTimeAsDate
-from .shared import DocumentStructure
-from .shared import HtmlString
-from .shared import OptionalList
 from patent_client.util.pydantic_util import BaseModel
-from patent_client.util.related import get_model
+
+from ..convert.biblio import PublicSearchBiblioPageSchema
+from .shared import (
+    ApplicationNumber,
+    DateTimeAsDate,
+    DocumentStructure,
+    HtmlString,
+    OptionalList,
+)
 
 
 class PublicSearchBiblio(BaseModel):
     guid: Optional[str] = None
     publication_number: Optional[str] = None
     publication_date: Optional[datetime.date] = None
     patent_title: Optional[HtmlString] = None
     type: Optional[str] = None
     main_classification_code: Optional[str] = None
-    applicant_names: OptionalList[str] = Field(alias="applicant_name", default_factory=list)
-    assignee_names: OptionalList[str] = Field(alias="assignee_name", default_factory=list)
+    applicant_names: OptionalList[str] = Field(
+        alias="applicant_name", default_factory=list
+    )
+    assignee_names: OptionalList[str] = Field(
+        alias="assignee_name", default_factory=list
+    )
     uspc_full_classification: OptionalList[str] = Field(default_factory=list)
     ipc_code: OptionalList[str] = Field(default_factory=list)
     cpc_additional: OptionalList[str] = Field(default_factory=list)
     app_filing_date: Optional[datetime.date] = None
-    related_appl_filing_date: OptionalList[DateTimeAsDate] = Field(alias="relatedApplFilingDate", default_factory=list)
+    related_appl_filing_date: OptionalList[DateTimeAsDate] = Field(
+        alias="relatedApplFilingDate", default_factory=list
+    )
     primary_examiner: Optional[str] = None
-    assistant_examiner: Optional[str] = Field(alias=AliasPath("assistant_examiner", 0), default=None)
+    assistant_examiner: Optional[str] = Field(
+        alias=AliasPath("assistant_examiner", 0), default=None
+    )
     appl_id: Optional[ApplicationNumber] = None
     document_structure: DocumentStructure
 
     def __repr__(self):
         return f"PublicSearcBiblio(publication_number={self.publication_number}, publication_date={self.publication_date}, patent_title={self.patent_title})"
 
     @property
     def document(self):
-        return get_model("patent_client.uspto.public_search.model.PublicSearchDocument").objects.get(guid=self.guid)
+        return self._get_model(".PublicSearchDocument").objects.get(guid=self.guid)
 
     @property
     def forward_citations(self):
-        return get_model("patent_client.uspto.public_search.model.PublicSearchBiblio").objects.filter(
+        return self._get_model(".PublicSearchBiblio").objects.filter(
             us_reference=self.publication_number
         )
 
     @property
     def application(self):
-        return get_model("patent_client.uspto.peds.model.USApplication").objects.get(self.appl_id)
+        return self._get_model("...peds.model.USApplication").objects.get(self.appl_id)
 
     @property
     def global_dossier(self):
-        return get_model("patent_client.uspto.global_dossier.model.GlobalDossierApplication").objects.get(self.appl_id)
+        return self._get_model(
+            "...global_dossier.model.GlobalDossierApplication"
+        ).objects.get(self.appl_id)
 
     @property
     def assignments(self):
-        return get_model("patent_client.uspto.assignment.model.Assignment").objects.filter(appl_id=self.appl_id)
+        return self._get_model("...assignment.model.Assignment").objects.filter(
+            appl_id=self.appl_id
+        )
 
     @property
     def inpadoc(self):
-        return get_model("patent_client.epo.ops.published.model.Inpadoc").objects.get("US" + self.publication_number)
-
-    def download_images(self, path="."):
-        return run_sync(self.adownload_images(path))
+        return self._get_model("...epo.ops.published.model.Inpadoc").objects.get(
+            "US" + self.publication_number
+        )
 
-    async def adownload_images(self, path="."):
-        from .manager import public_search_api
+    async def download_images(self, path="."):
+        from ..manager import public_search_api
 
         return await public_search_api.download_image(self, path)
 
 
 class PublicSearchBiblioPage(BaseModel):
     __schema__ = PublicSearchBiblioPageSchema()
     num_found: int
```

### Comparing `patent_client-4.1.9/patent_client/uspto/public_search/model/document.py` & `patent_client-5.0.0/patent_client/_async/uspto/public_search/model/document.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,16 @@
-from typing import List
-from typing import Optional
+from typing import List, Optional
 
-from pydantic import Field
-from pydantic import model_validator
+from pydantic import Field, model_validator
 
-from ..convert.document import PublicSearchDocumentSchema
-from .shared import ApplicationNumber
-from .shared import DocumentStructure
-from .shared import HtmlString
-from .shared import OptionalList
-from patent_client.util.asyncio_util import run_sync
 from patent_client.util.claims.model import Claim
-from patent_client.util.pydantic_util import BaseModel
-from patent_client.util.pydantic_util import Date
-from patent_client.util.related import get_model
+from patent_client.util.pydantic_util import BaseModel, Date
+
+from ..convert.document import PublicSearchDocumentSchema
+from .shared import ApplicationNumber, DocumentStructure, HtmlString, OptionalList
 
 
 class Document(BaseModel):
     abstract_html: Optional[str] = None
     abstract: Optional[HtmlString] = Field(alias="abstract_html", default=None)
     government_interest: Optional[str] = None
     background_html: Optional[str] = Field(alias="background_html", default=None)
@@ -167,19 +160,14 @@
 
     field_of_search_us: OptionalList[str] = Field(default_factory=list)
     field_of_search_cpc: OptionalList[str] = Field(default_factory=list)
 
     def __repr__(self):
         return f"PublicSearchDocument(publication_number={self.publication_number}, publication_date={self.publication_date}, patent_title={self.patent_title})"
 
-    @model_validator(mode="before")
-    @classmethod
-    def convert_to_json(cls, values):
-        return PublicSearchBiblioConvert.convert(values)
-
     @property
     def abstract(self):
         return self.document.abstract
 
     @property
     def description(self):
         sections = (
@@ -197,39 +185,42 @@
 
     @property
     def claims(self):
         return self.document.claims
 
     @property
     def forward_citations(self):
-        return get_model("patent_client.uspto.public_search.model.PublicSearchBiblio").objects.filter(
+        return self._get_model(".PublicSearchBiblio").objects.filter(
             us_reference=self.publication_number
         )
 
-    def download_images(self, path="."):
-        return run_sync(self.adownload_images(path))
-
-    async def adownload_images(self, path="."):
+    async def download_images(self, path="."):
         from ..manager import public_search_api
 
         return await public_search_api.download_image(self, path)
 
     @property
     def application(self):
-        return get_model("patent_client.uspto.peds.model.USApplication").objects.get(self.appl_id)
+        return self._get_model("...peds.model.USApplication").objects.get(self.appl_id)
 
     @property
     def global_dossier(self):
-        return get_model("patent_client.uspto.global_dossier.model.GlobalDossierApplication").objects.get(self.appl_id)
+        return self._get_model(
+            "...global_dossier.model.GlobalDossierApplication"
+        ).objects.get(self.appl_id)
 
     @property
     def assignments(self):
-        return get_model("patent_client.uspto.assignment.model.Assignment").objects.filter(appl_id=self.appl_id)
+        return self._get_model("...assignment.model.Assignment").objects.filter(
+            appl_id=self.appl_id
+        )
 
     @property
     def inpadoc(self):
-        return get_model("patent_client.epo.ops.published.model.Inpadoc").objects.get("US" + self.publication_number)
+        return self._get_model("...epo.ops.published.model.Inpadoc").objects.get(
+            "US" + self.publication_number
+        )
 
     @model_validator(mode="before")
     @classmethod
-    def convert_to_json(cls, values):
+    def convert_xml_to_json(cls, values):
         return cls.__schema__.deserialize(values).to_dict()
```

### Comparing `patent_client-4.1.9/patent_client/uspto/public_search/model/shared.py` & `patent_client-5.0.0/patent_client/_async/uspto/public_search/model/shared.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import datetime
-from typing import List
-from typing import Optional
-from typing import TypeVar
+from typing import List, Optional, TypeVar
 
-from pydantic import BeforeValidator
-from pydantic import ConfigDict
+from pydantic import BeforeValidator, ConfigDict
 from pydantic.alias_generators import to_camel
 from typing_extensions import Annotated
 
-from ..util import html_to_text
 from patent_client.util.pydantic_util import BaseModel
 
+from ..util import html_to_text
+
 
 class PublicSearchBaseModel(BaseModel):
     model_config = ConfigDict(
         alias_generator=to_camel,
         str_strip_whitespace=True,
     )
 
 
 T = TypeVar("T")
 
 
-OptionalList = Annotated[List[T], BeforeValidator(lambda x: x if isinstance(x, list) else list())]
+OptionalList = Annotated[
+    List[T], BeforeValidator(lambda x: x if isinstance(x, list) else list())
+]
 DateTimeAsDate = Annotated[
-    datetime.date, BeforeValidator(lambda x: x.date() if isinstance(x, datetime.datetime) else x)
+    datetime.date,
+    BeforeValidator(lambda x: x.date() if isinstance(x, datetime.datetime) else x),
 ]
 HtmlString = Annotated[str, BeforeValidator(html_to_text)]
 
 
 def format_appl_id(string):
     if string.startswith("D"):
         string = "29" + string[1:]
```

### Comparing `patent_client-4.1.9/patent_client/uspto/public_search/model_test.py` & `patent_client-5.0.0/patent_client/_sync/uspto/public_search/model_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,20 @@
+# ********************************************************************************
+# *         WARNING: This file is automatically generated by unasync.py.         *
+# *                             DO NOT MANUALLY EDIT                             *
+# *     Source File: patent_client/_async/uspto/public_search/model_test.py      *
+# ********************************************************************************
+
 import json
 from pathlib import Path
 
+from patent_client.util.test import compare_dicts, compare_lists
+
 from .model.biblio import PublicSearchBiblioPage
 from .model.document import PublicSearchDocument
-from patent_client.util.test import compare_dicts
-from patent_client.util.test import compare_lists
 
 fixtures = Path(__file__).parent / "fixtures"
 
 
 import datetime
 
 
@@ -33,9 +39,11 @@
 def test_parse_doc():
     input_file = fixtures / "doc.json"
     output_file = fixtures / "doc_output.json"
     input_data = json.loads(input_file.read_text())
     output_data = [PublicSearchDocument.model_validate(o) for o in input_data]
     # output_file.write_text(json.dumps([o.model_dump() for o in output_data], indent=2, default=json_serial))
     expected_data = json.loads(output_file.read_text())
-    output_data = json.loads(json.dumps([o.model_dump() for o in output_data], indent=2, default=json_serial))
+    output_data = json.loads(
+        json.dumps([o.model_dump() for o in output_data], indent=2, default=json_serial)
+    )
     compare_lists(output_data, expected_data)
```

### Comparing `patent_client-4.1.9/patent_client/uspto/public_search/query.py` & `patent_client-5.0.0/patent_client/_async/uspto/public_search/query.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,16 +13,20 @@
 
 class QueryBuilder:
     def __init__(self):
         config_file = Path(__file__).parent / "query_config.csv"
         with config_file.open(encoding="utf-8-sig") as csvfile:
             reader = csv.DictReader(csvfile)
             config = list(reader)
-        self.search_keywords = {r["keyword"]: r["query_field"] for r in config if r["query_field"]}
-        self.order_by_keywords = {r["keyword"]: r["order_by_field"] for r in config if r["order_by_field"]}
+        self.search_keywords = {
+            r["keyword"]: r["query_field"] for r in config if r["query_field"]
+        }
+        self.order_by_keywords = {
+            r["keyword"]: r["order_by_field"] for r in config if r["order_by_field"]
+        }
         self.date_fields = [r["keyword"] for r in config if r["is_date"] == "X"]
 
     def convert_date(self, date):
         if isinstance(date, str):
             try:
                 return parse_dt(date).strftime("%Y%m%d")
             except ParserError:
@@ -34,49 +38,55 @@
 
     def is_sequence(self, value):
         return isinstance(value, Sequence) and not isinstance(value, str)
 
     def query_value(self, key, value):
         field, *_ = key.split("__")
         if field in self.date_fields and "__" not in key:
+            value = value[0]
             if isinstance(value, str) and "->" in value:
                 start, end = value.split("->")
                 return f"@{self.search_keywords[key]}>={self.convert_date(start)}<={self.convert_date(end)}"
             else:
                 return f'@{self.search_keywords[key]}="{self.convert_date(value)}"'
         elif field in self.date_fields and "__" in key:
+            value = value[0]
             field, modifier = key.split("__")
             if modifier == "range":
                 if not self.is_sequence(value) and len(value) == 2:
-                    raise ValueError(f"Input {value} is not a valid date range! Must be a tuple/list of length 2")
+                    raise ValueError(
+                        f"Input {value} is not a valid date range! Must be a tuple/list of length 2"
+                    )
                 # breakpoint()
                 return f"@{self.search_keywords[field]}>={self.convert_date(value[0])}<={self.convert_date(value[1])}"
             elif modifier == "lt":
                 return f'@{self.search_keywords[field]}<"{self.convert_date(value)}"'
             elif modifier == "lte":
                 return f'@{self.search_keywords[field]}<="{self.convert_date(value)}"'
             elif modifier == "gt":
                 return f'@{self.search_keywords[field]}>"{self.convert_date(value)}"'
             elif modifier == "gte":
                 return f'@{self.search_keywords[field]}>="{self.convert_date(value)}"'
             else:
-                raise ValueError(f"Modifier {modifier} is invalid! must be one of range, lt, lte, gt, gte")
+                raise ValueError(
+                    f"Modifier {modifier} is invalid! must be one of range, lt, lte, gt, gte"
+                )
         elif self.is_sequence(value) and len(value) > 1:
             value = " ".join(f'"{v}"' for v in value)
             return f"({value}).{self.search_keywords[key]}."
         elif self.is_sequence(value) and len(value) == 1:
             return f'"{value[0]}".{self.search_keywords[key]}.'
         else:
             return f'"{value}".{self.search_keywords[key]}.'
 
     def build_query(self, config):
         query_components = list()
         for key, value in config.filter.items():
             if key == "query":
-                query_components.append(value)
+                query_components.append(value[0])
                 continue
             if key.split("__")[0] not in self.search_keywords:
                 raise QueryException(f"{key} is not a valid search field!")
             else:
                 query_components.append(self.query_value(key, value))
         default_operator = config.options.get("default_operator", "AND")
         return f" {default_operator} ".join(query_components)
```

### Comparing `patent_client-4.1.9/patent_client/uspto/public_search/query_config.csv` & `patent_client-5.0.0/patent_client/_async/uspto/public_search/query_config.csv`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/uspto/public_search/query_test.py` & `patent_client-5.0.0/patent_client/_async/uspto/public_search/query_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,45 +6,85 @@
 
 
 class QueryTest:
     def test_default_query(self):
         assert PatentBiblioManager().filter("6103599")._query == '"6103599".PN.'
 
     def test_plural_default_query(self):
-        assert PatentBiblioManager().filter("6103599", "6103600")._query == '("6103599" "6103600").PN.'
+        assert (
+            PatentBiblioManager().filter("6103599", "6103600")._query
+            == '("6103599" "6103600").PN.'
+        )
 
     def test_keyword_query(self):
-        assert PatentBiblioManager().filter(appl_id="6103599")._query == '"6103599".APNR.'
+        assert (
+            PatentBiblioManager().filter(appl_id="6103599")._query == '"6103599".APNR.'
+        )
 
     def test_plural_keyword_query(self):
-        assert PatentBiblioManager().filter(appl_id=("11111111", "11222222"))._query == '("11111111" "11222222").APNR.'
+        assert (
+            PatentBiblioManager().filter(appl_id=("11111111", "11222222"))._query
+            == '("11111111" "11222222").APNR.'
+        )
 
     def test_keyword_date_query(self):
-        assert PatentBiblioManager().filter(app_filing_date="2021-01-01")._query == '@APD="20210101"'
-        assert PatentBiblioManager().filter(app_filing_date=parse_dt("2021-01-01"))._query == '@APD="20210101"'
-        assert PatentBiblioManager().filter(app_filing_date=parse_dt("2021-01-01").date())._query == '@APD="20210101"'
+        assert (
+            PatentBiblioManager().filter(app_filing_date="2021-01-01")._query
+            == '@APD="20210101"'
+        )
+        assert (
+            PatentBiblioManager().filter(app_filing_date=parse_dt("2021-01-01"))._query
+            == '@APD="20210101"'
+        )
+        assert (
+            PatentBiblioManager()
+            .filter(app_filing_date=parse_dt("2021-01-01").date())
+            ._query
+            == '@APD="20210101"'
+        )
 
     def test_keyword_date_range_query(self):
         assert (
-            PatentBiblioManager().filter(app_filing_date="2021-01-01->2021-02-01")._query == "@APD>=20210101<=20210201"
+            PatentBiblioManager()
+            .filter(app_filing_date="2021-01-01->2021-02-01")
+            ._query
+            == "@APD>=20210101<=20210201"
         )
         assert (
-            PatentBiblioManager().filter(app_filing_date__range=("2021-01-01", "2021-02-01"))._query
+            PatentBiblioManager()
+            .filter(app_filing_date__range=("2021-01-01", "2021-02-01"))
+            ._query
             == "@APD>=20210101<=20210201"
         )
         assert (
-            PatentBiblioManager().filter(app_filing_date__range=(parse_dt("2021-01-01"), parse_dt("2021-02-01")))._query
+            PatentBiblioManager()
+            .filter(
+                app_filing_date__range=(parse_dt("2021-01-01"), parse_dt("2021-02-01"))
+            )
+            ._query
             == "@APD>=20210101<=20210201"
         )
 
     def test_date_operator_queries(self):
-        assert PatentBiblioManager().filter(app_filing_date__gt="2021-01-01")._query == '@APD>"20210101"'
-        assert PatentBiblioManager().filter(app_filing_date__gte="2021-01-01")._query == '@APD>="20210101"'
-        assert PatentBiblioManager().filter(app_filing_date__lt="2021-01-01")._query == '@APD<"20210101"'
-        assert PatentBiblioManager().filter(app_filing_date__lte="2021-01-01")._query == '@APD<="20210101"'
+        assert (
+            PatentBiblioManager().filter(app_filing_date__gt="2021-01-01")._query
+            == '@APD>"20210101"'
+        )
+        assert (
+            PatentBiblioManager().filter(app_filing_date__gte="2021-01-01")._query
+            == '@APD>="20210101"'
+        )
+        assert (
+            PatentBiblioManager().filter(app_filing_date__lt="2021-01-01")._query
+            == '@APD<"20210101"'
+        )
+        assert (
+            PatentBiblioManager().filter(app_filing_date__lte="2021-01-01")._query
+            == '@APD<="20210101"'
+        )
 
     def test_error_query(self):
         with pytest.raises(QueryException):
             PatentBiblioManager().filter(blargh="2021-01-01")._query
 
     def test_error_date_query(self):
         with pytest.raises(QueryException):
@@ -54,28 +94,38 @@
 
     def test_multiple_fields(self):
         assert (
             PatentBiblioManager().filter("6103599", app_filing_date="2021-01-01")._query
             == '@APD="20210101" AND "6103599".PN.'
         )
         assert (
-            PatentBiblioManager().filter("6103599").filter(app_filing_date="2021-01-01")._query
+            PatentBiblioManager()
+            .filter("6103599")
+            .filter(app_filing_date="2021-01-01")
+            ._query
             == '"6103599".PN. AND @APD="20210101"'
         )
         assert (
-            PatentBiblioManager().filter(patent_number="6103599", app_filing_date="2021-01-01")._query
+            PatentBiblioManager()
+            .filter(patent_number="6103599", app_filing_date="2021-01-01")
+            ._query
             == '@APD="20210101" AND "6103599".PN.'
         )
 
     def test_raw_query(self):
-        assert PatentBiblioManager().filter(query="example query")._query == "example query"
+        assert (
+            PatentBiblioManager().filter(query="example query")._query
+            == "example query"
+        )
 
     def test_raw_query_with_keywords(self):
         assert (
-            PatentBiblioManager().filter(query="some text", patent_number="6103599")._query
+            PatentBiblioManager()
+            .filter(query="some text", patent_number="6103599")
+            ._query
             == '"6103599".PN. AND some text'
         )
 
     def test_default_or(self):
         assert (
             PatentBiblioManager()
             .option(default_operator="OR")
```

### Comparing `patent_client-4.1.9/patent_client/util/claims/examples/multiple_dependent.json` & `patent_client-5.0.0/patent_client/util/claims/examples/multiple_dependent.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/util/claims/examples/multiple_dependent.txt` & `patent_client-5.0.0/patent_client/util/claims/examples/multiple_dependent.txt`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/util/claims/examples/published_claims.json` & `patent_client-5.0.0/patent_client/util/claims/examples/published_claims.json`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/util/claims/examples/published_claims.txt` & `patent_client-5.0.0/patent_client/util/claims/examples/published_claims.txt`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/util/claims/model.py` & `patent_client-5.0.0/patent_client/util/claims/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/util/claims/parser.py` & `patent_client-5.0.0/patent_client/util/claims/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import re
 from itertools import zip_longest
 
-
-SPLIT_RE = re.compile(r"^\s*([\d\-\.]+[\)\.]|\.Iadd\.[\d\-\.]+\.|\.\[[\d\-\.]+\.)", flags=re.MULTILINE)
+SPLIT_RE = re.compile(
+    r"^\s*([\d\-\.]+[\)\.]|\.Iadd\.[\d\-\.]+\.|\.\[[\d\-\.]+\.)", flags=re.MULTILINE
+)
 NUMERIC_RE = re.compile(r"\d")
 
 LIMITATION_RE = re.compile(r"(\s*[:;]\s*and|\s*[:;]\s*)", flags=re.IGNORECASE)
 NUMBER_RE = re.compile(r"(?P<number>\d+)[\)\.]\s+")
 WHITESPACE_RE = re.compile(r"\s+")
 CLAIM_INTRO_RE = re.compile(r"^[^\d\.\[]+")
 
 DEPENDENCY_RE = re.compile(r"claims? (?P<number>[\d,or ]+)", flags=re.IGNORECASE)
 DEPENDENT_CLAIMS_RE = re.compile(r"(?P<number>\d+)([^\d]|$)")
-DEPEND_ALL_RE = re.compile(r"(any of the foregoing claims|any of the previous claims)", flags=re.IGNORECASE)
+DEPEND_ALL_RE = re.compile(
+    r"(any of the foregoing claims|any of the previous claims)", flags=re.IGNORECASE
+)
 
 clean_text = lambda text: WHITESPACE_RE.sub(" ", text).strip()
 
 
 def grouper(iterable, n, fillvalue=None):
     "Collect data into fixed-length chunks or blocks"
     # grouper('ABCDEFG', 3, 'x') --> ABC DEF Gxx"
@@ -62,22 +65,28 @@
 
     def parse_claim_string(self, text):
         number = int(NUMBER_RE.search(text).group("number"))
         text = NUMBER_RE.sub("", text)
         return {
             "number": number,
             # "text": NUMBER_RE.sub("", text),
-            "limitations": [clean_text("".join(lim)) for lim in list(grouper(LIMITATION_RE.split(text), 2, ""))],
+            "limitations": [
+                clean_text("".join(lim))
+                for lim in list(grouper(LIMITATION_RE.split(text), 2, ""))
+            ],
             "depends_on": self.parse_dependency(text, number),
             "dependent_claims": list(),
         }
 
     def parse_dependency(self, text, number):
         dependency = DEPENDENCY_RE.search(text)
         if dependency is not None:
             claims = dependency.groupdict()["number"]
-            claim_numbers = [int(m.groupdict()["number"]) for m in DEPENDENT_CLAIMS_RE.finditer(claims)]
+            claim_numbers = [
+                int(m.groupdict()["number"])
+                for m in DEPENDENT_CLAIMS_RE.finditer(claims)
+            ]
             return claim_numbers
         elif DEPEND_ALL_RE.search(text):
             return list(range(1, number))
         else:
             return list()
```

### Comparing `patent_client-4.1.9/patent_client/util/claims/parser_test.py` & `patent_client-5.0.0/patent_client/util/claims/parser_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from pathlib import Path
 
-from .parser import ClaimsParser
 from patent_client.util.test import compare_lists
 
+from .parser import ClaimsParser
+
 example_dir = Path(__file__).parent / "examples"
 
 
 def test_multiple_dependent_claims():
     file = example_dir / "multiple_dependent.txt"
     text = file.read_text()
     result = ClaimsParser().parse(text)
```

### Comparing `patent_client-4.1.9/patent_client/util/format.py` & `patent_client-5.0.0/patent_client/util/format.py`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/patent_client/util/request_util.py` & `patent_client-5.0.0/patent_client/util/request_util.py`

 * *Files identical despite different names*

### Comparing `patent_client-4.1.9/pyproject.toml` & `patent_client-5.0.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "patent_client"
-version = "4.1.9"
+version = "5.0.0"
 description = "A set of ORM-style clients for publicly available intellectual property data"
 authors = ["Parker Hancock <633163+parkerhancock@users.noreply.github.com>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 documentation = "https://patent-client.readthedocs.io"
 homepage = "https://github.com/parkerhancock/patent_client"
 repository = "https://github.com/parkerhancock/patent_client"
@@ -25,47 +25,46 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 
 # Required Dependencies
 lxml = "^4.9.0"
 python-dateutil = "^2.8.2"
-inflection = "^0.5.1"
 openpyxl = "^3.0.10"
 #yankee = {path="../yankee", develop=true}
 yankee = "^0.1.43"
-zipp = "^3.8.1"
-httpx = {extras = ["http2"], version = "^0.25.2"}
 
 pydantic = "^2.4.2"
 pydantic-settings = "^2.0.3"
 pypdf = "^3.17.0"
 hishel = "^0.0.20"
-tqdm = "^4.66.1"
+async-property = "^0.2.2"
+httpx = {extras = ["http2"], version = "^0.27.0"}
+
+# Documentation Dependencies
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 
 # Documentation Dependencies
-furo                       = {optional=true, version="^2022.6"}
-linkify-it-py              = {optional=true, version="^2.0"}
-myst-parser                = {optional=true, version=">=0.17"}
-sphinx                     = {optional=true, version="^5.0.2"}
-sphinx-autodoc-typehints   = {optional=true, version="^1.19"}
-sphinx-automodapi          = {optional=true, version=">=0.14"}
-sphinx-copybutton          = {optional=true, version=">=0.5"}
-sphinx-design              = {optional=true, version=">=0.2"}
-sphinx-notfound-page       = {optional=true, version=">=0.8"}
-sphinxcontrib-apidoc       = {optional=true, version="^0.3"}
-sphinxcontrib-mermaid      = {optional=true, version="^0.7.1"}
-nbsphinx                   = {optional=true, version="^0.8.9"}
-IPython                    = {optional=true, version="^7.17.0"}
-nest-asyncio = "^1.5.8"
+furo                       = "^2022.6"
+linkify-it-py              = "^2.0"
+myst-parser                = ">=0.17"
+sphinx                     = "^5.0.2"
+sphinx-autodoc-typehints   = "^1.19"
+sphinx-automodapi          = ">=0.14"
+sphinx-copybutton          = ">=0.5"
+sphinx-design              = ">=0.2"
+sphinx-notfound-page       = ">=0.8"
+sphinxcontrib-apidoc       = "^0.3"
+sphinxcontrib-mermaid      = "^0.7.1"
+nbsphinx                   = "^0.8.9"
+IPython                    = "^7.17.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 pre-commit = "^2.19.0"
 pytest-xdist = "^2.5.0"
 black = {version = "^22.12.0", allow-prereleases = true}
@@ -77,14 +76,17 @@
 
 nox                   = "^2022.1.7"
 nox-poetry            = "^1.0.0"
 rich                  = ">=10.0"
 sphinx-autobuild      = "^2021.3.14"
 bump2version = "^1.0.1"
 pytest-recording = "^0.13.1"
+datamodel-code-generator = "^0.25.5"
+openapi-python-client = "^0.19.1"
+isort = "^5.13.2"
 
 
 [tool.poetry.group.types.dependencies]
 types-openpyxl = "^3.1.0.24"
 types-python-dateutil = "^2.8.19.14"
 pandas-stubs = "^2.1.1.230928"
 types-ujson = "^5.8.0.1"
@@ -110,15 +112,15 @@
 
 [tool.pytest.ini_options]
 python_files = [
     "test_*.py",
     "*_test.py",
     "tests.py",
 ]
-addopts = '-ra --strict --doctest-modules --doctest-glob="*.md" --tb=short'
+addopts = '-ra --strict-markers --doctest-modules --doctest-glob="*.md" --tb=short'
 doctest_optionflags= [
     "NORMALIZE_WHITESPACE",
     "IGNORE_EXCEPTION_DETAIL",
     "ELLIPSIS"
 ]
 asyncio_mode = "auto"
 markers = [
```

### Comparing `patent_client-4.1.9/PKG-INFO` & `patent_client-5.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: patent-client
-Version: 4.1.9
+Name: patent_client
+Version: 5.0.0
 Summary: A set of ORM-style clients for publicly available intellectual property data
 Home-page: https://github.com/parkerhancock/patent_client
 License: Apache Software License 2.0
 Keywords: patent,intellectual property,usitc,epo,ops,trademark,inpadoc,337
 Author: Parker Hancock
 Author-email: 633163+parkerhancock@users.noreply.github.com
 Requires-Python: >=3.9,<3.13
@@ -15,26 +15,24 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
+Requires-Dist: async-property (>=0.2.2,<0.3.0)
 Requires-Dist: hishel (>=0.0.20,<0.0.21)
-Requires-Dist: httpx[http2] (>=0.25.2,<0.26.0)
-Requires-Dist: inflection (>=0.5.1,<0.6.0)
+Requires-Dist: httpx[http2] (>=0.27.0,<0.28.0)
 Requires-Dist: lxml (>=4.9.0,<5.0.0)
 Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.0.3,<3.0.0)
 Requires-Dist: pypdf (>=3.17.0,<4.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Requires-Dist: yankee (>=0.1.43,<0.2.0)
-Requires-Dist: zipp (>=3.8.1,<4.0.0)
 Project-URL: Documentation, https://patent-client.readthedocs.io
 Project-URL: Repository, https://github.com/parkerhancock/patent_client
 Description-Content-Type: text/markdown
 
 [![patent_client_logo](https://raw.githubusercontent.com/parkerhancock/patent_client/master/docs/_static/patent_client_logo.svg)](https://patent-client.readthedocs.io)
 
 [![Build](https://github.com/parkerhancock/patent_client/actions/workflows/build.yaml/badge.svg)](https://github.com/parkerhancock/patent_client/actions/workflows/build.yaml)
@@ -56,19 +54,29 @@
 - 🚀 **Performance:** Fetched data is retrieved using the [httpx][httpx] library with native HTTP/2 and asyncio support, and cached using the [hishel][hishel] library for super-fast queries, and [yankee][yankee] for data extraction.
 - 🌐 **Async/Await Support:** All API's (optionally!) support the async/await syntax.
 - 🔮 **Pydantic v2 Support:** All models retrieved are [Pydantic v2 models][pydantic] with all the goodness that comes with them!
 
 Docs, including a fulsome Getting Started and User Guide are available on [Read the Docs](http://patent-client.readthedocs.io). The Examples folder includes examples of using `patent_client` for
 many common IP tasks
 
+## ⭐ New in v5 ⭐
+
+Version 5 brings a new and more reliable way to provide synchronous and asynchronous access to the various APIs.
+In version 5, like in version 3, you can just `from patent_client import [Model]` and get a synchronous version
+of the model. No asynchronous methods or functionality at all. Or you can do `from patent_client._async import [Model]`
+and get an asynchronous version of the model.
+
+Version 5 also brings support for the USPTO's new [Open Data Portal](https://beta-data.uspto.gov/home), a system currently in beta that is scheduled to replace the current Patent Examination Data System in late 2024.
+
 ## Coverage
 
 - [United States Patent & Trademark Office][USPTO]
 
   - [Patent Examination Data][PEDS] - Full Support
+  - [Open Data Portal][ODP] - Full Support
   - [Global Dossier][GD] - Full Support
   - [Patent Assignment Data][Assignment] - Lookup Support
   - [Patent Trial & Appeal Board API v2][PTAB] - Supports Proceedings, Decisions, and Documents
   - [Patent Public Search][PPS] - Full Support
   - [Bulk Data Storage System][BDSS] - Full Support
 
 
@@ -90,14 +98,15 @@
 [PPS]:  https://ppubs.uspto.gov/pubwebapp/static/pages/landing.html
 [PEDS]: https://developer.uspto.gov/api-catalog/ped
 [PTAB]: https://developer.uspto.gov/api-catalog/ptab-api-v2
 [USPTO]: http://developer.uspto.gov
 [BDSS]: https://developer.uspto.gov/api-catalog/bdss
 [GD]: https://globaldossier.uspto.gov
 [pydantic]: https://docs.pydantic.dev/latest/
+[ODP]: https://beta-data.uspto.gov/home
 
 
 ## Installation
 
 ```
 pip install patent_client
 ```
@@ -132,17 +141,20 @@
 >>> pub.biblio.title
 'AUTOMATIC FLUID DISPENSER'
 
 ```
 
 ## Async Quick Start
 
-To use the asyncio methods, simply use `async with` for iterators, and call any methods with a `a` prefix:
+To use async with Patent Client, just import the classes you need from the async module. All methods
+and iterators that access data or create a network request are asynchronous.
 
 ```python
+from patent_client._async import USApplication
+
 apps = list()
 async for app in USApplication.objects.filter(first_named_applicant="Google"):
   apps.append(app)
 
 app = await USApplication.objects.aget("16123456")
 
 ```
```

