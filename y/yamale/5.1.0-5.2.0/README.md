# Comparing `tmp/yamale-5.1.0.tar.gz` & `tmp/yamale-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamale-5.1.0.tar", last modified: Wed Mar 20 17:35:03 2024, max compression
+gzip compressed data, was "yamale-5.2.0.tar", last modified: Thu Apr 25 15:24:09 2024, max compression
```

## Comparing `yamale-5.1.0.tar` & `yamale-5.2.0.tar`

### file list

```diff
@@ -1,142 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:35:03.956931 yamale-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-20 17:34:45.000000 yamale-5.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-20 17:34:45.000000 yamale-5.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20898 2024-03-20 17:35:03.956931 yamale-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20046 2024-03-20 17:34:45.000000 yamale-5.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-20 17:34:45.000000 yamale-5.1.0/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 17:35:03.956931 yamale-5.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1315 2024-03-20 17:34:45.000000 yamale-5.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:35:03.936931 yamale-5.1.0/yamale/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/command_line.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:35:03.940931 yamale-5.1.0/yamale/readers/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/readers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:35:03.940931 yamale-5.1.0/yamale/readers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/readers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/readers/tests/test_bad_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/readers/tests/test_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/readers/yaml_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:35:03.940931 yamale-5.1.0/yamale/schema/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/schema/datapath.py
--rw-r--r--   0 runner    (1001) docker     (127)     7303 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/schema/validationresults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:35:03.940931 yamale-5.1.0/yamale/syntax/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/syntax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/syntax/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:35:03.940931 yamale-5.1.0/yamale/syntax/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/syntax/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/syntax/tests/test_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:35:03.940931 yamale-5.1.0/yamale/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:35:03.956931 yamale-5.1.0/yamale/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/any.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/any_bad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/any_good.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/bad_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/bad_schema_rce.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/bad_schema_rce2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/bad_schema_rce3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/bad_schema_rce4.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/custom_types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/custom_types_bad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/custom_types_good.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/empty_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/include_validator.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/include_validator_bad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/include_validator_good.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/ip.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/ip_bad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/ip_good.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/issue_22.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/issue_22_good.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/issue_50.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/issue_50_good.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/keywords.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/keywords_bad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/keywords_good.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/list_include.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/list_include_good.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/lists.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/lists_bad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/lists_bad2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/lists_good.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/mac.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/mac_bad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/mac_good.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/map.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/map_bad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/map_bad2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/map_good.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/map_key_constraint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/map_key_constraint_bad_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/map_key_constraint_bad_nest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/map_key_constraint_bad_nest_con.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/map_key_constraint_good.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/mixed_strict_map.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/mixed_strict_map_bad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/mixed_strict_map_good.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/nested.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/nested_bad_data.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/nested_good_data.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/nested_issue_54.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/nested_map.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/nested_map2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/nested_map2_bad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/nested_map2_good.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/nested_map_good.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/numeric_bool_coercion.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/numeric_bool_coercion_bad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/numeric_bool_coercion_good.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/regex.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/regex_bad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/regex_good.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/static_list.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/static_list_bad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/static_list_good.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/strict_list.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/strict_list_bad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/strict_list_good.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/strict_map.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/strict_map_bad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/strict_map_good.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/subset.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/subset_bad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/subset_bad2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/subset_bad3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/subset_empty.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/subset_empty_good.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/subset_empty_good2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/subset_good.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/subset_good2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/subset_nodef.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/top_level_map.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/top_level_map_good.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/types_bad_data.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/fixtures/types_good_data.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/test_command_line.py
--rw-r--r--   0 runner    (1001) docker     (127)    10965 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/tests/test_meta_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:35:03.956931 yamale-5.1.0/yamale/validators/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/validators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/validators/constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:35:03.956931 yamale-5.1.0/yamale/validators/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/validators/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/validators/tests/test_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/validators/tests/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/validators/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/yamale.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/yamale_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-20 17:34:45.000000 yamale-5.1.0/yamale/yamale_testcase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:35:03.956931 yamale-5.1.0/yamale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20898 2024-03-20 17:35:03.000000 yamale-5.1.0/yamale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-03-20 17:35:03.000000 yamale-5.1.0/yamale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 17:35:03.000000 yamale-5.1.0/yamale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-20 17:35:03.000000 yamale-5.1.0/yamale.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-20 17:35:03.000000 yamale-5.1.0/yamale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-20 17:35:03.000000 yamale-5.1.0/yamale.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:09.990926 yamale-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-25 15:24:01.000000 yamale-5.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-25 15:24:01.000000 yamale-5.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21331 2024-04-25 15:24:09.990926 yamale-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20479 2024-04-25 15:24:01.000000 yamale-5.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-25 15:24:01.000000 yamale-5.2.0/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:24:09.990926 yamale-5.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1315 2024-04-25 15:24:01.000000 yamale-5.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:09.970926 yamale-5.2.0/yamale/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/command_line.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:09.970926 yamale-5.2.0/yamale/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/readers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:09.974926 yamale-5.2.0/yamale/readers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/readers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/readers/tests/test_bad_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/readers/tests/test_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/readers/yaml_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:09.974926 yamale-5.2.0/yamale/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/schema/datapath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/schema/validationresults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:09.974926 yamale-5.2.0/yamale/syntax/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/syntax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/syntax/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:09.974926 yamale-5.2.0/yamale/syntax/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/syntax/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/syntax/tests/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:09.974926 yamale-5.2.0/yamale/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:09.990926 yamale-5.2.0/yamale/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/any.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/any_bad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/any_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/any_undefined.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/any_undefined_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/bad_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/bad_schema_rce.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/bad_schema_rce2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/bad_schema_rce3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/bad_schema_rce4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/custom_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/custom_types_bad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/custom_types_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/empty_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/include_validator.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/include_validator_bad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/include_validator_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/ip.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/ip_bad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/ip_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/issue_22.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/issue_22_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/issue_50.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/issue_50_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/keywords.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/keywords_bad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/keywords_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/list_include.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/list_include_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/lists.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/lists_bad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/lists_bad2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/lists_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/mac.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/mac_bad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/mac_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/map.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/map_bad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/map_bad2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/map_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/map_key_constraint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/map_key_constraint_bad_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/map_key_constraint_bad_nest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/map_key_constraint_bad_nest_con.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/map_key_constraint_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/mixed_strict_map.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/mixed_strict_map_bad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/mixed_strict_map_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/nested.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/nested_bad_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/nested_good_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/nested_issue_54.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/nested_map.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/nested_map2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/nested_map2_bad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/nested_map2_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/nested_map_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/numeric_bool_coercion.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/numeric_bool_coercion_bad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/numeric_bool_coercion_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/regex.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/regex_bad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/regex_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/semver_bad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/semver_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/semver_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/static_list.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/static_list_bad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/static_list_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/strict_list.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/strict_list_bad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/strict_list_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/strict_map.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/strict_map_bad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/strict_map_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/subset.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/subset_bad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/subset_bad2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/subset_bad3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/subset_empty.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/subset_empty_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/subset_empty_good2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/subset_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/subset_good2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/subset_nodef.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/top_level_map.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/top_level_map_good.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/types_bad_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/fixtures/types_good_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/test_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11309 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/tests/test_meta_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:09.990926 yamale-5.2.0/yamale/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/validators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/validators/constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:09.990926 yamale-5.2.0/yamale/validators/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/validators/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/validators/tests/test_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/validators/tests/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/validators/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/yamale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/yamale_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-25 15:24:01.000000 yamale-5.2.0/yamale/yamale_testcase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:09.990926 yamale-5.2.0/yamale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21331 2024-04-25 15:24:09.000000 yamale-5.2.0/yamale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-25 15:24:09.000000 yamale-5.2.0/yamale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:24:09.000000 yamale-5.2.0/yamale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 15:24:09.000000 yamale-5.2.0/yamale.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 15:24:09.000000 yamale-5.2.0/yamale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 15:24:09.000000 yamale-5.2.0/yamale.egg-info/top_level.txt
```

### Comparing `yamale-5.1.0/LICENSE` & `yamale-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yamale-5.1.0/PKG-INFO` & `yamale-5.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamale
-Version: 5.1.0
+Version: 5.2.0
 Summary: A schema and validator for YAML.
 Home-page: https://github.com/23andMe/Yamale
 Author: Bo Lopker
 Author-email: blopker@23andme.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -420,14 +420,20 @@
 
 ### MAC Address - `mac()`
 Validates MAC addresses.
 
 Examples:
 - `mac()`: Allows any valid MAC address
 
+### SemVer (Semantic Versioning) - `semver()`
+Validates [Semantic Versioning](https://semver.org/) strings.
+
+Examples:
+- `semver()`: Allows any valid SemVer string
+
 ### Any - `any([validators])`
 Validates against a union of types. Use when a node **must** contain **one and only one** of several types. It is valid
 if at least one of the listed validators is valid. If no validators are given, accept any value.
 - arguments: validators to test values with (if none is given, allow any value; if one or more are given,
 one must be present)
 
 Examples:
@@ -622,14 +628,19 @@
 
 `schema`: String of path to the schema file to use. One schema file per test case.
 
 `yaml`: String or list of yaml files to validate. Accepts globs.
 
 Developers
 ----------
+### Linting + Formatting
+Yamale is formatted with [ruff](https://github.com/astral-sh/ruff). There is a github action enforcing
+ruff formatting and linting rules. You can run this locally via `make lint` or by installing
+the pre-commit hooks via `make install-hooks`
+
 ### Testing
 Yamale uses [Tox](https://tox.readthedocs.org/en/latest/) to run its tests against multiple Python
 versions. To run tests, first checkout Yamale, install Tox, then run `make test` in Yamale's root
 directory. You may also have to install the correct Python versions to test with as well.
 
 NOTE on Python versions: `tox.ini` specifies the lowest and highest versions of Python supported by
 Yamale. Unless your development environment is configured to support testing against multiple Python
```

### Comparing `yamale-5.1.0/README.md` & `yamale-5.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -396,14 +396,20 @@
 
 ### MAC Address - `mac()`
 Validates MAC addresses.
 
 Examples:
 - `mac()`: Allows any valid MAC address
 
+### SemVer (Semantic Versioning) - `semver()`
+Validates [Semantic Versioning](https://semver.org/) strings.
+
+Examples:
+- `semver()`: Allows any valid SemVer string
+
 ### Any - `any([validators])`
 Validates against a union of types. Use when a node **must** contain **one and only one** of several types. It is valid
 if at least one of the listed validators is valid. If no validators are given, accept any value.
 - arguments: validators to test values with (if none is given, allow any value; if one or more are given,
 one must be present)
 
 Examples:
@@ -598,14 +604,19 @@
 
 `schema`: String of path to the schema file to use. One schema file per test case.
 
 `yaml`: String or list of yaml files to validate. Accepts globs.
 
 Developers
 ----------
+### Linting + Formatting
+Yamale is formatted with [ruff](https://github.com/astral-sh/ruff). There is a github action enforcing
+ruff formatting and linting rules. You can run this locally via `make lint` or by installing
+the pre-commit hooks via `make install-hooks`
+
 ### Testing
 Yamale uses [Tox](https://tox.readthedocs.org/en/latest/) to run its tests against multiple Python
 versions. To run tests, first checkout Yamale, install Tox, then run `make test` in Yamale's root
 directory. You may also have to install the correct Python versions to test with as well.
 
 NOTE on Python versions: `tox.ini` specifies the lowest and highest versions of Python supported by
 Yamale. Unless your development environment is configured to support testing against multiple Python
```

### Comparing `yamale-5.1.0/SECURITY.md` & `yamale-5.2.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `yamale-5.1.0/setup.py` & `yamale-5.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `yamale-5.1.0/yamale/command_line.py` & `yamale-5.2.0/yamale/command_line.py`

 * *Files identical despite different names*

### Comparing `yamale-5.1.0/yamale/readers/tests/test_yaml.py` & `yamale-5.2.0/yamale/readers/tests/test_yaml.py`

 * *Files identical despite different names*

### Comparing `yamale-5.1.0/yamale/readers/yaml_reader.py` & `yamale-5.2.0/yamale/readers/yaml_reader.py`

 * *Files identical despite different names*

### Comparing `yamale-5.1.0/yamale/schema/schema.py` & `yamale-5.2.0/yamale/schema/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 from .datapath import DataPath
 from .validationresults import ValidationResult
 from .. import syntax, util
 from .. import validators as val
 
 
+class FatalValidationError(Exception):
+    def __init__(self, error):
+        super().__init__()
+        self.error = error
+
+
 class Schema(object):
     """
     Makes a Schema object from a schema dict.
     Still acts like a dict.
     """
 
     def __init__(self, schema_dict, name="", validators=None, includes=None):
@@ -41,15 +47,18 @@
         except SyntaxError as e:
             # Tack on some more context and rethrow.
             error = str(e) + " at node '%s'" % str(path)
             raise SyntaxError(error)
 
     def validate(self, data, data_name, strict):
         path = DataPath()
-        errors = self._validate(self._schema, data, path, strict)
+        try:
+            errors = self._validate(self._schema, data, path, strict)
+        except FatalValidationError as e:
+            errors = [e.error]
         return ValidationResult(data_name, self.name, errors)
 
     def _validate_item(self, validator, data, path, strict, key):
         """
         Fetch item from data at the position key and validate with validator.
 
         Returns an array of errors.
@@ -87,15 +96,14 @@
         errors += self._validate_primitive(validator, data, path)
 
         if errors:
             return errors
 
         if isinstance(validator, val.Include):
             errors += self._validate_include(validator, data, path, strict)
-
         elif isinstance(validator, (val.Map, val.List)):
             errors += self._validate_map_list(validator, data, path, strict)
 
         elif isinstance(validator, val.Any):
             errors += self._validate_any(validator, data, path, strict)
 
         elif isinstance(validator, val.Subset):
@@ -142,15 +150,15 @@
                     errors += err
 
         return errors
 
     def _validate_include(self, validator, data, path, strict):
         include_schema = self.includes.get(validator.include_name)
         if not include_schema:
-            return [("Include '%s' has not been defined." % validator.include_name)]
+            raise FatalValidationError("Include '%s' has not been defined." % validator.include_name)
         strict = strict if validator.strict is None else validator.strict
         return include_schema._validate(include_schema._schema, data, path, strict)
 
     def _validate_any(self, validator, data, path, strict):
         if not validator.validators:
             return []
 
@@ -168,16 +176,16 @@
                 errors += err
 
         return errors
 
     def _validate_subset(self, validator, data, path, strict):
         def _internal_validate(internal_data):
             sub_errors = []
-            for val in validator.validators:
-                err = self._validate(val, internal_data, path, strict)
+            for v in validator.validators:
+                err = self._validate(v, internal_data, path, strict)
                 if not err:
                     break
                 sub_errors += err
             else:
                 return sub_errors
             return []
```

### Comparing `yamale-5.1.0/yamale/schema/validationresults.py` & `yamale-5.2.0/yamale/schema/validationresults.py`

 * *Files identical despite different names*

### Comparing `yamale-5.1.0/yamale/syntax/parser.py` & `yamale-5.2.0/yamale/syntax/parser.py`

 * *Files identical despite different names*

### Comparing `yamale-5.1.0/yamale/syntax/tests/test_parser.py` & `yamale-5.2.0/yamale/syntax/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `yamale-5.1.0/yamale/tests/test_command_line.py` & `yamale-5.2.0/yamale/tests/test_command_line.py`

 * *Files identical despite different names*

### Comparing `yamale-5.1.0/yamale/tests/test_functional.py` & `yamale-5.2.0/yamale/tests/test_functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 lists = {"schema": "lists.yaml", "bad": "lists_bad.yaml", "bad2": "lists_bad2.yaml", "good": "lists_good.yaml"}
 
 maps = {"schema": "map.yaml", "bad": "map_bad.yaml", "bad2": "map_bad2.yaml", "good": "map_good.yaml"}
 
 anys = {"schema": "any.yaml", "bad": "any_bad.yaml", "good": "any_good.yaml"}
 
+any_undefined = {"schema": "any_undefined_schema.yaml", "bad": "any_undefined.yaml"}
+
 list_include = {"schema": "list_include.yaml", "good": "list_include_good.yaml"}
 
 issue_22 = {"schema": "issue_22.yaml", "good": "issue_22_good.yaml"}
 
 issue_50 = {"schema": "issue_50.yaml", "good": "issue_50_good.yaml"}
 
 regexes = {"schema": "regex.yaml", "bad": "regex_bad.yaml", "good": "regex_good.yaml"}
@@ -32,14 +34,17 @@
 
 macs = {"schema": "mac.yaml", "bad": "mac_bad.yaml", "good": "mac_good.yaml"}
 
 nested_map = {"schema": "nested_map.yaml", "good": "nested_map_good.yaml"}
 
 top_level_map = {"schema": "top_level_map.yaml", "good": "top_level_map_good.yaml"}
 
+semver = {"schema": "semver_schema.yaml", "good": "semver_good.yaml", "bad": "semver_bad.yaml"}
+
+
 include_validator = {
     "schema": "include_validator.yaml",
     "good": "include_validator_good.yaml",
     "bad": "include_validator_bad.yaml",
 }
 
 strict_map = {"schema": "strict_map.yaml", "good": "strict_map_good.yaml", "bad": "strict_map_bad.yaml"}
@@ -89,14 +94,15 @@
     types,
     nested,
     custom,
     keywords,
     lists,
     maps,
     anys,
+    any_undefined,
     list_include,
     issue_22,
     issue_50,
     regexes,
     ips,
     macs,
     nested_map,
@@ -106,47 +112,43 @@
     mixed_strict_map,
     strict_list,
     nested_map2,
     static_list,
     nested_issue_54,
     map_key_constraint,
     numeric_bool_coercion,
+    semver,
     subset,
     subset_empty,
 ]
 
 for d in test_data:
     for key in d.keys():
         if key == "schema":
             d[key] = yamale.make_schema(get_fixture(d[key]))
         else:
             d[key] = yamale.make_data(get_fixture(d[key]))
 
 
-def test_tests():
-    """Make sure the test runner is working."""
-    assert 1 + 1 == 2
-
-
 def test_flat_make_schema():
     assert isinstance(types["schema"]._schema["string"], val.String)
 
 
 def test_nested_schema():
     nested_schema = nested["schema"]._schema
     assert isinstance(nested_schema["string"], val.String)
     assert isinstance(nested_schema["list"], (list, tuple))
     assert isinstance(nested_schema["list"][0], val.String)
 
 
 @pytest.mark.parametrize("data_map", test_data)
 def test_good(data_map):
-    for k, v in data_map.items():
+    for k, good_data in data_map.items():
         if k.startswith("good"):
-            yamale.validate(data_map["schema"], data_map[k])
+            yamale.validate(data_map["schema"], good_data)
 
 
 def test_bad_validate():
     assert count_exception_lines(types["schema"], types["bad"]) == 9
 
 
 def test_bad_nested():
@@ -191,14 +193,22 @@
     assert count_exception_lines(keywords["schema"], keywords["bad"]) == 9
 
 
 def test_bad_anys():
     assert count_exception_lines(anys["schema"], anys["bad"]) == 5
 
 
+def test_undefined_include():
+    assert count_exception_lines(any_undefined["schema"], any_undefined["bad"]) == 1
+
+
+def test_bad_semver():
+    assert count_exception_lines(semver["schema"], semver["bad"]) == 1
+
+
 def test_bad_regexes():
     assert count_exception_lines(regexes["schema"], regexes["bad"]) == 4
 
 
 def test_bad_include_validator():
     exp = ["key1: 'a_string' is not a int."]
     match_exception_lines(include_validator["schema"], include_validator["bad"], exp)
```

### Comparing `yamale-5.1.0/yamale/tests/test_meta_test.py` & `yamale-5.2.0/yamale/tests/test_meta_test.py`

 * *Files identical despite different names*

### Comparing `yamale-5.1.0/yamale/util.py` & `yamale-5.2.0/yamale/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,16 @@
-# ABCs for containers were moved to their own module
-try:
-    from collections.abc import Mapping, Set, Sequence
-except ImportError:
-    from collections import Mapping, Set, Sequence
+from collections.abc import Mapping, Sequence
 
 
-# Python 3 has no basestring, lets test it.
-try:
-    basestring  # attempt to evaluate basestring
+def isstr(s):
+    return isinstance(s, str)
 
-    def isstr(s):
-        return isinstance(s, basestring)
 
-    def to_unicode(s):
-        return unicode(s)
-
-except NameError:
-
-    def isstr(s):
-        return isinstance(s, str)
-
-    def to_unicode(s):
-        return s
+def to_unicode(s):
+    return s
 
 
 def is_list(obj):
     return isinstance(obj, Sequence) and not isstr(obj)
 
 
 def is_map(obj):
```

### Comparing `yamale-5.1.0/yamale/validators/base.py` & `yamale-5.2.0/yamale/validators/base.py`

 * *Files identical despite different names*

### Comparing `yamale-5.1.0/yamale/validators/constraints.py` & `yamale-5.2.0/yamale/validators/constraints.py`

 * *Files identical despite different names*

### Comparing `yamale-5.1.0/yamale/validators/tests/test_constraint.py` & `yamale-5.2.0/yamale/validators/tests/test_constraint.py`

 * *Files identical despite different names*

### Comparing `yamale-5.1.0/yamale/validators/validators.py` & `yamale-5.2.0/yamale/validators/validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -244,13 +244,26 @@
         super(Mac, self).__init__(*args, **kwargs)
         self.regexes = [
             re.compile("[0-9a-fA-F]{2}([-:]?)[0-9a-fA-F]{2}(\\1[0-9a-fA-F]{2}){4}$"),
             re.compile("[0-9a-fA-F]{4}([-:]?)[0-9a-fA-F]{4}(\\1[0-9a-fA-F]{4})$"),
         ]
 
 
+class SemVer(Regex):
+    """Semantic Versioning (semver.org) validator"""
+
+    tag = "semver"
+
+    def __init__(self, *args, **kwargs):
+        super(SemVer, self).__init__(*args, **kwargs)
+        self.regexes = [
+            # https://semver.org/#is-there-a-suggested-regular-expression-regex-to-check-a-semver-string
+            re.compile("^(?P<major>0|[1-9]\d*)\.(?P<minor>0|[1-9]\d*)\.(?P<patch>0|[1-9]\d*)(?:-(?P<prerelease>(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*)(?:\.(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*))*))?(?:\+(?P<buildmetadata>[0-9a-zA-Z-]+(?:\.[0-9a-zA-Z-]+)*))?$"),
+        ]
+
+
 DefaultValidators = {}
 
 for v in util.get_subclasses(Validator):
     # Allow validator nodes to contain either tags or actual name
     DefaultValidators[v.tag] = v
     DefaultValidators[v.__name__] = v
```

### Comparing `yamale-5.1.0/yamale/yamale.py` & `yamale-5.2.0/yamale/yamale.py`

 * *Files identical despite different names*

### Comparing `yamale-5.1.0/yamale/yamale_testcase.py` & `yamale-5.2.0/yamale/yamale_testcase.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         schema = self.schema
         yaml = self.yaml
         base_dir = self.base_dir
 
         if schema is None:
             return
 
-        if type(yaml) != list:
+        if not isinstance(yaml, list):
             yaml = [yaml]
 
         if base_dir is not None:
             schema = os.path.join(base_dir, schema)
             yaml = {os.path.join(base_dir, y) for y in yaml}
 
         # Run yaml through glob and flatten list
```

### Comparing `yamale-5.1.0/yamale.egg-info/PKG-INFO` & `yamale-5.2.0/yamale.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamale
-Version: 5.1.0
+Version: 5.2.0
 Summary: A schema and validator for YAML.
 Home-page: https://github.com/23andMe/Yamale
 Author: Bo Lopker
 Author-email: blopker@23andme.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -420,14 +420,20 @@
 
 ### MAC Address - `mac()`
 Validates MAC addresses.
 
 Examples:
 - `mac()`: Allows any valid MAC address
 
+### SemVer (Semantic Versioning) - `semver()`
+Validates [Semantic Versioning](https://semver.org/) strings.
+
+Examples:
+- `semver()`: Allows any valid SemVer string
+
 ### Any - `any([validators])`
 Validates against a union of types. Use when a node **must** contain **one and only one** of several types. It is valid
 if at least one of the listed validators is valid. If no validators are given, accept any value.
 - arguments: validators to test values with (if none is given, allow any value; if one or more are given,
 one must be present)
 
 Examples:
@@ -622,14 +628,19 @@
 
 `schema`: String of path to the schema file to use. One schema file per test case.
 
 `yaml`: String or list of yaml files to validate. Accepts globs.
 
 Developers
 ----------
+### Linting + Formatting
+Yamale is formatted with [ruff](https://github.com/astral-sh/ruff). There is a github action enforcing
+ruff formatting and linting rules. You can run this locally via `make lint` or by installing
+the pre-commit hooks via `make install-hooks`
+
 ### Testing
 Yamale uses [Tox](https://tox.readthedocs.org/en/latest/) to run its tests against multiple Python
 versions. To run tests, first checkout Yamale, install Tox, then run `make test` in Yamale's root
 directory. You may also have to install the correct Python versions to test with as well.
 
 NOTE on Python versions: `tox.ini` specifies the lowest and highest versions of Python supported by
 Yamale. Unless your development environment is configured to support testing against multiple Python
```

### Comparing `yamale-5.1.0/yamale.egg-info/SOURCES.txt` & `yamale-5.2.0/yamale.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 yamale/tests/__init__.py
 yamale/tests/test_command_line.py
 yamale/tests/test_functional.py
 yamale/tests/test_meta_test.py
 yamale/tests/fixtures/any.yaml
 yamale/tests/fixtures/any_bad.yaml
 yamale/tests/fixtures/any_good.yaml
+yamale/tests/fixtures/any_undefined.yaml
+yamale/tests/fixtures/any_undefined_schema.yaml
 yamale/tests/fixtures/bad_schema.yaml
 yamale/tests/fixtures/bad_schema_rce.yaml
 yamale/tests/fixtures/bad_schema_rce2.yaml
 yamale/tests/fixtures/bad_schema_rce3.yaml
 yamale/tests/fixtures/bad_schema_rce4.yaml
 yamale/tests/fixtures/custom_types.yaml
 yamale/tests/fixtures/custom_types_bad.yaml
@@ -91,14 +93,17 @@
 yamale/tests/fixtures/nested_map_good.yaml
 yamale/tests/fixtures/numeric_bool_coercion.yaml
 yamale/tests/fixtures/numeric_bool_coercion_bad.yaml
 yamale/tests/fixtures/numeric_bool_coercion_good.yaml
 yamale/tests/fixtures/regex.yaml
 yamale/tests/fixtures/regex_bad.yaml
 yamale/tests/fixtures/regex_good.yaml
+yamale/tests/fixtures/semver_bad.yaml
+yamale/tests/fixtures/semver_good.yaml
+yamale/tests/fixtures/semver_schema.yaml
 yamale/tests/fixtures/static_list.yaml
 yamale/tests/fixtures/static_list_bad.yaml
 yamale/tests/fixtures/static_list_good.yaml
 yamale/tests/fixtures/strict_list.yaml
 yamale/tests/fixtures/strict_list_bad.yaml
 yamale/tests/fixtures/strict_list_good.yaml
 yamale/tests/fixtures/strict_map.yaml
```

