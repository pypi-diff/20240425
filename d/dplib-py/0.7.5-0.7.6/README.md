# Comparing `tmp/dplib_py-0.7.5.tar.gz` & `tmp/dplib_py-0.7.6.tar.gz`

## Comparing `dplib_py-0.7.5.tar` & `dplib_py-0.7.6.tar`

### file list

```diff
@@ -1,269 +1,269 @@
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 dplib_py-0.7.5/mkdocs.yaml
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dplib_py-0.7.5/.github/codecov.yaml
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dplib_py-0.7.5/.github/issue_template.md
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 dplib_py-0.7.5/.github/pull_request_template.md
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dplib_py-0.7.5/.github/stale.yaml
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 dplib_py-0.7.5/.github/workflows/general.yaml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/dialect-full.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/dialect-invalid.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/dialect.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/empty.json
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/package-custom-profile.json
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/package-full.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/package-invalid-dereferencing.json
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/package-invalid.json
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/package.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/profile.json
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/resource-full.json
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/resource-invalid-dereferencing.json
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/resource-invalid.json
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/resource.json
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/resource.yaml
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/schema-full.json
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/schema-invalid.json
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/schema-types.json
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/schema.json
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/text.txt
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/cassettes/test_check_package_custom_profile.yaml
--rw-r--r--   0        0        0    14982 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/cassettes/test_dialect_profile.yaml
--rw-r--r--   0        0        0    60589 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/cassettes/test_package_profile.yaml
--rw-r--r--   0        0        0   220871 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/cassettes/test_resource_profile.yaml
--rw-r--r--   0        0        0   169730 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/cassettes/test_schema_profile.yaml
--rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/plugins/ckan/package.json
--rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/plugins/datacite/package.json
--rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/plugins/dcat/package.xml
--rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/plugins/github/package.json
--rw-r--r--   0        0        0     7431 2020-02-02 00:00:00.000000 dplib_py-0.7.5/data/plugins/zenodo/package.json
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/changelog.md
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/contributing.md
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/converting-metadata.md
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/index.md
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/installation.md
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/validating-metadata.md
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/working-with-models.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/.theme/.keep
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/actions/dialect.md
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/actions/package.md
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/actions/resource.md
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/actions/schema.md
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/assets/favicon-color.png
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/assets/favicon-shaddow.png
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/assets/favicon.ico
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/assets/favicon.png
--rw-r--r--   0        0        0     8911 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/assets/logo-dark.svg
--rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/assets/logo-light.svg
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/models/dialect.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/models/package.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/models/resource.md
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/models/schema.md
--rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/plugins/ckan.md
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/plugins/cli.md
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/plugins/datacite.md
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/plugins/dcat.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/plugins/github.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/plugins/pandas.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/plugins/polars.md
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/plugins/sql.md
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 dplib_py-0.7.5/docs/plugins/zenodo.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/__init__.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/conftest.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/error.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/py.typed
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/settings.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/actions/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/actions/__spec__/test_dialect_check.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/actions/__spec__/test_package_check.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/actions/__spec__/test_resource_check.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/actions/__spec__/test_schema_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/actions/dialect/__init__.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/actions/dialect/check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/actions/metadata/__init__.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/actions/metadata/check.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/actions/metadata/convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/actions/package/__init__.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/actions/package/check.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/actions/package/convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/actions/resource/__init__.py
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/actions/resource/check.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/actions/resource/convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/actions/schema/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/actions/schema/check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/errors/__init__.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/errors/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/helpers/__init__.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/helpers/data.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/helpers/file.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/helpers/path.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/helpers/profile.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/helpers/resource.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/__init__.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/contributor.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/license.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/source.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/dialect/__init__.py
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/dialect/dialect.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/dialect/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/dialect/__spec__/__init__.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/dialect/__spec__/test_dialect.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/__init__.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/field.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/types.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/__spec__/test_field.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/constraints/__init__.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/constraints/base.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/constraints/collection.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/constraints/json.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/constraints/string.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/constraints/value.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/datatypes/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/datatypes/any.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/datatypes/array.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/datatypes/base.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/datatypes/boolean.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/datatypes/date.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/datatypes/datetime.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/datatypes/duration.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/datatypes/geojson.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/datatypes/geopoint.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/datatypes/integer.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/datatypes/list.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/datatypes/number.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/datatypes/object.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/datatypes/string.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/datatypes/time.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/datatypes/year.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/field/datatypes/yearmonth.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/package/__init__.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/package/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/package/__spec__/__init__.py
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/package/__spec__/test_package.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/resource/__init__.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/resource/hash.py
--rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/resource/resource.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/resource/__spec__/__init__.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/resource/__spec__/test_resource.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/resource/datatypes/__init__.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/resource/datatypes/table.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/schema/__init__.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/schema/foreignKey.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/schema/schema.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/schema/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/schema/__spec__/__init__.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/models/schema/__spec__/test_schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/ckan/__init__.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/ckan/models/__init__.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/ckan/models/field.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/ckan/models/organization.py
--rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/ckan/models/package.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/ckan/models/resource.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/ckan/models/schema.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/ckan/models/tag.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/ckan/models/__spec__/__init__.py
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/ckan/models/__spec__/test_package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/__init__.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/__main__.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/program.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/commands/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/commands/main.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/commands/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/commands/__spec__/__init__.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/commands/__spec__/test_version.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/commands/dialect/__init__.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/commands/dialect/check.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/commands/dialect/main.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/commands/package/__init__.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/commands/package/check.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/commands/package/convert.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/commands/package/main.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/commands/resource/__init__.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/commands/resource/check.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/commands/resource/convert.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/commands/resource/main.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/commands/schema/__init__.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/commands/schema/check.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/commands/schema/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/helpers/__init__.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/helpers/check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/options/__init__.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/options/convert.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/options/path.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/cli/options/system.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/datacite/__init__.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/datacite/models/__init__.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/datacite/models/contributor.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/datacite/models/description.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/datacite/models/identifier.py
--rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/datacite/models/package.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/datacite/models/rights.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/datacite/models/subject.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/datacite/models/title.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/datacite/models/__spec__/__init__.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/datacite/models/__spec__/test_package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/dcat/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/dcat/models/__init__.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/dcat/models/dumpers.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/dcat/models/helpers.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/dcat/models/loaders.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/dcat/models/namespaces.py
--rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/dcat/models/package.py
--rw-r--r--   0        0        0     6362 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/dcat/models/resource.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/dcat/models/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/dcat/models/__spec__/__init__.py
--rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/dcat/models/__spec__/test_package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/github/__init__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/github/models/__init__.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/github/models/license.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/github/models/owner.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/github/models/package.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/github/models/resource.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/github/models/__spec__/__init__.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/github/models/__spec__/test_package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/pandas/__init__.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/pandas/models/__init__.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/pandas/models/field.py
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/pandas/models/schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/pandas/models/__spec__/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/polars/__init__.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/polars/models/__init__.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/polars/models/field.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/polars/models/schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/polars/models/__spec__/__init__.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/polars/models/__spec__/test_schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/sql/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/sql/models/__init__.py
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/sql/models/field.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/sql/models/schema.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/sql/models/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/sql/models/__spec__/__init__.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/sql/models/__spec__/test_schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/zenodo/__init__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/zenodo/models/__init__.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/zenodo/models/contributor.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/zenodo/models/files.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/zenodo/models/metadata.py
--rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/zenodo/models/package.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/zenodo/models/pid.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/zenodo/models/resource.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/zenodo/models/right.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/zenodo/models/subject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/zenodo/models/__spec__/__init__.py
--rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/plugins/zenodo/models/__spec__/test_package.py
--rw-r--r--   0        0        0   107095 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/profiles/1.0/datapackage.json
--rw-r--r--   0        0        0    85332 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/profiles/1.0/dataresource.json
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/profiles/1.0/tabledialect.json
--rw-r--r--   0        0        0    65533 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/profiles/1.0/tableschema.json
--rw-r--r--   0        0        0   142568 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/profiles/2.0/datapackage.json
--rw-r--r--   0        0        0   117144 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/profiles/2.0/dataresource.json
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/profiles/2.0/tabledialect.json
--rw-r--r--   0        0        0    94827 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/profiles/2.0/tableschema.json
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/system/__init__.py
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/system/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/system/__spec__/__init__.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 dplib_py-0.7.5/dplib/system/__spec__/test_model.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 dplib_py-0.7.5/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 dplib_py-0.7.5/LICENSE.md
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 dplib_py-0.7.5/README.md
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 dplib_py-0.7.5/pyproject.toml
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 dplib_py-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 dplib_py-0.7.6/mkdocs.yaml
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dplib_py-0.7.6/.github/codecov.yaml
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dplib_py-0.7.6/.github/issue_template.md
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 dplib_py-0.7.6/.github/pull_request_template.md
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dplib_py-0.7.6/.github/stale.yaml
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 dplib_py-0.7.6/.github/workflows/general.yaml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/dialect-full.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/dialect-invalid.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/dialect.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/empty.json
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/package-custom-profile.json
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/package-full.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/package-invalid-dereferencing.json
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/package-invalid.json
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/package.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/profile.json
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/resource-full.json
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/resource-invalid-dereferencing.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/resource-invalid.json
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/resource.json
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/resource.yaml
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/schema-full.json
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/schema-invalid.json
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/schema-types.json
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/schema.json
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/text.txt
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/cassettes/test_check_package_custom_profile.yaml
+-rw-r--r--   0        0        0    14982 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/cassettes/test_dialect_profile.yaml
+-rw-r--r--   0        0        0    60589 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/cassettes/test_package_profile.yaml
+-rw-r--r--   0        0        0   220871 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/cassettes/test_resource_profile.yaml
+-rw-r--r--   0        0        0   169730 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/cassettes/test_schema_profile.yaml
+-rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/plugins/ckan/package.json
+-rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/plugins/datacite/package.json
+-rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/plugins/dcat/package.xml
+-rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/plugins/github/package.json
+-rw-r--r--   0        0        0     7431 2020-02-02 00:00:00.000000 dplib_py-0.7.6/data/plugins/zenodo/package.json
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/changelog.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/contributing.md
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/converting-metadata.md
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/index.md
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/installation.md
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/validating-metadata.md
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/working-with-models.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/.theme/.keep
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/actions/dialect.md
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/actions/package.md
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/actions/resource.md
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/actions/schema.md
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/assets/favicon-color.png
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/assets/favicon-shaddow.png
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/assets/favicon.ico
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/assets/favicon.png
+-rw-r--r--   0        0        0     8911 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/assets/logo-dark.svg
+-rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/assets/logo-light.svg
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/models/dialect.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/models/package.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/models/resource.md
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/models/schema.md
+-rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/plugins/ckan.md
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/plugins/cli.md
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/plugins/datacite.md
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/plugins/dcat.md
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/plugins/github.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/plugins/pandas.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/plugins/polars.md
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/plugins/sql.md
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 dplib_py-0.7.6/docs/plugins/zenodo.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/__init__.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/conftest.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/error.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/py.typed
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/settings.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/actions/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/actions/__spec__/test_dialect_check.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/actions/__spec__/test_package_check.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/actions/__spec__/test_resource_check.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/actions/__spec__/test_schema_check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/actions/dialect/__init__.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/actions/dialect/check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/actions/metadata/__init__.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/actions/metadata/check.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/actions/metadata/convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/actions/package/__init__.py
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/actions/package/check.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/actions/package/convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/actions/resource/__init__.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/actions/resource/check.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/actions/resource/convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/actions/schema/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/actions/schema/check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/errors/__init__.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/errors/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/helpers/__init__.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/helpers/dict.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/helpers/file.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/helpers/path.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/helpers/profile.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/helpers/resource.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/__init__.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/contributor.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/license.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/source.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/dialect/__init__.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/dialect/dialect.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/dialect/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/dialect/__spec__/__init__.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/dialect/__spec__/test_dialect.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/__init__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/field.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/types.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/__spec__/test_field.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/constraints/__init__.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/constraints/base.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/constraints/collection.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/constraints/json.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/constraints/string.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/constraints/value.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/datatypes/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/datatypes/any.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/datatypes/array.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/datatypes/base.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/datatypes/boolean.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/datatypes/date.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/datatypes/datetime.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/datatypes/duration.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/datatypes/geojson.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/datatypes/geopoint.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/datatypes/integer.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/datatypes/list.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/datatypes/number.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/datatypes/object.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/datatypes/string.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/datatypes/time.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/datatypes/year.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/field/datatypes/yearmonth.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/package/__init__.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/package/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/package/__spec__/__init__.py
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/package/__spec__/test_package.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/resource/__init__.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/resource/hash.py
+-rw-r--r--   0        0        0     5572 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/resource/resource.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/resource/__spec__/__init__.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/resource/__spec__/test_resource.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/resource/datatypes/__init__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/resource/datatypes/table.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/schema/__init__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/schema/foreignKey.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/schema/schema.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/schema/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/schema/__spec__/__init__.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/models/schema/__spec__/test_schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/ckan/__init__.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/ckan/models/__init__.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/ckan/models/field.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/ckan/models/organization.py
+-rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/ckan/models/package.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/ckan/models/resource.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/ckan/models/schema.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/ckan/models/tag.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/ckan/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/ckan/models/__spec__/test_package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/__init__.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/__main__.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/program.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/commands/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/commands/main.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/commands/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/commands/__spec__/__init__.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/commands/__spec__/test_version.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/commands/dialect/__init__.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/commands/dialect/check.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/commands/dialect/main.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/commands/package/__init__.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/commands/package/check.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/commands/package/convert.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/commands/package/main.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/commands/resource/__init__.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/commands/resource/check.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/commands/resource/convert.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/commands/resource/main.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/commands/schema/__init__.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/commands/schema/check.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/commands/schema/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/helpers/__init__.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/helpers/check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/options/__init__.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/options/convert.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/options/path.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/cli/options/system.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/datacite/__init__.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/datacite/models/__init__.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/datacite/models/contributor.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/datacite/models/description.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/datacite/models/identifier.py
+-rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/datacite/models/package.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/datacite/models/rights.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/datacite/models/subject.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/datacite/models/title.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/datacite/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/datacite/models/__spec__/test_package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/dcat/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/dcat/models/__init__.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/dcat/models/dumpers.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/dcat/models/helpers.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/dcat/models/loaders.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/dcat/models/namespaces.py
+-rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/dcat/models/package.py
+-rw-r--r--   0        0        0     6362 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/dcat/models/resource.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/dcat/models/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/dcat/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/dcat/models/__spec__/test_package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/github/__init__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/github/models/__init__.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/github/models/license.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/github/models/owner.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/github/models/package.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/github/models/resource.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/github/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/github/models/__spec__/test_package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/pandas/__init__.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/pandas/models/__init__.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/pandas/models/field.py
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/pandas/models/schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/pandas/models/__spec__/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/polars/__init__.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/polars/models/__init__.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/polars/models/field.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/polars/models/schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/polars/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/polars/models/__spec__/test_schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/sql/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/sql/models/__init__.py
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/sql/models/field.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/sql/models/schema.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/sql/models/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/sql/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/sql/models/__spec__/test_schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/zenodo/__init__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/zenodo/models/__init__.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/zenodo/models/contributor.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/zenodo/models/files.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/zenodo/models/metadata.py
+-rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/zenodo/models/package.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/zenodo/models/pid.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/zenodo/models/resource.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/zenodo/models/right.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/zenodo/models/subject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/zenodo/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/plugins/zenodo/models/__spec__/test_package.py
+-rw-r--r--   0        0        0   107095 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/profiles/1.0/datapackage.json
+-rw-r--r--   0        0        0    85332 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/profiles/1.0/dataresource.json
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/profiles/1.0/tabledialect.json
+-rw-r--r--   0        0        0    65533 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/profiles/1.0/tableschema.json
+-rw-r--r--   0        0        0   142568 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/profiles/2.0/datapackage.json
+-rw-r--r--   0        0        0   117144 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/profiles/2.0/dataresource.json
+-rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/profiles/2.0/tabledialect.json
+-rw-r--r--   0        0        0    94827 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/profiles/2.0/tableschema.json
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/system/__init__.py
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/system/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/system/__spec__/__init__.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 dplib_py-0.7.6/dplib/system/__spec__/test_model.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 dplib_py-0.7.6/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 dplib_py-0.7.6/LICENSE.md
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 dplib_py-0.7.6/README.md
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 dplib_py-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 dplib_py-0.7.6/PKG-INFO
```

### Comparing `dplib_py-0.7.5/mkdocs.yaml` & `dplib_py-0.7.6/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/.github/stale.yaml` & `dplib_py-0.7.6/.github/stale.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/.github/workflows/general.yaml` & `dplib_py-0.7.6/.github/workflows/general.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/data/package-full.json` & `dplib_py-0.7.6/data/package-full.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/data/schema-full.json` & `dplib_py-0.7.6/data/schema-full.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/data/schema-types.json` & `dplib_py-0.7.6/data/schema-types.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/data/cassettes/test_check_package_custom_profile.yaml` & `dplib_py-0.7.6/data/cassettes/test_check_package_custom_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/data/cassettes/test_dialect_profile.yaml` & `dplib_py-0.7.6/data/cassettes/test_dialect_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/data/cassettes/test_package_profile.yaml` & `dplib_py-0.7.6/data/cassettes/test_package_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/data/cassettes/test_resource_profile.yaml` & `dplib_py-0.7.6/data/cassettes/test_resource_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/data/cassettes/test_schema_profile.yaml` & `dplib_py-0.7.6/data/cassettes/test_schema_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/data/plugins/ckan/package.json` & `dplib_py-0.7.6/data/plugins/ckan/package.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/data/plugins/datacite/package.json` & `dplib_py-0.7.6/data/plugins/datacite/package.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/data/plugins/dcat/package.xml` & `dplib_py-0.7.6/data/plugins/dcat/package.xml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/data/plugins/github/package.json` & `dplib_py-0.7.6/data/plugins/github/package.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/data/plugins/zenodo/package.json` & `dplib_py-0.7.6/data/plugins/zenodo/package.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/docs/contributing.md` & `dplib_py-0.7.6/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/docs/converting-metadata.md` & `dplib_py-0.7.6/docs/converting-metadata.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/docs/index.md` & `dplib_py-0.7.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/docs/validating-metadata.md` & `dplib_py-0.7.6/docs/validating-metadata.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/docs/working-with-models.md` & `dplib_py-0.7.6/docs/working-with-models.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/docs/assets/favicon-shaddow.png` & `dplib_py-0.7.6/docs/assets/favicon-shaddow.png`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/docs/assets/favicon.ico` & `dplib_py-0.7.6/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/docs/assets/logo-dark.svg` & `dplib_py-0.7.6/docs/assets/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/docs/assets/logo-light.svg` & `dplib_py-0.7.6/docs/assets/logo-light.svg`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/docs/models/package.md` & `dplib_py-0.7.6/docs/models/package.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/docs/models/resource.md` & `dplib_py-0.7.6/docs/models/resource.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/docs/models/schema.md` & `dplib_py-0.7.6/docs/models/schema.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/docs/plugins/ckan.md` & `dplib_py-0.7.6/docs/plugins/ckan.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/docs/plugins/cli.md` & `dplib_py-0.7.6/docs/plugins/cli.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/docs/plugins/datacite.md` & `dplib_py-0.7.6/docs/plugins/datacite.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/docs/plugins/dcat.md` & `dplib_py-0.7.6/docs/plugins/dcat.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/docs/plugins/github.md` & `dplib_py-0.7.6/docs/plugins/github.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/docs/plugins/pandas.md` & `dplib_py-0.7.6/docs/plugins/pandas.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/docs/plugins/polars.md` & `dplib_py-0.7.6/docs/plugins/polars.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/docs/plugins/sql.md` & `dplib_py-0.7.6/docs/plugins/sql.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/docs/plugins/zenodo.md` & `dplib_py-0.7.6/docs/plugins/zenodo.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/settings.py` & `dplib_py-0.7.6/dplib/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 # Version
 
-VERSION = "0.7.5"
+VERSION = "0.7.6"
 
 # Profiles
 
 PROFILE_BASEURL = "https://datapackage.org/profiles"
 PROFILE_BASEDIR = os.path.join(os.path.dirname(__file__), "profiles")
 
 PROFILE_DEFAULT = "1.0"
```

### Comparing `dplib_py-0.7.5/dplib/actions/__spec__/test_dialect_check.py` & `dplib_py-0.7.6/dplib/actions/__spec__/test_dialect_check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/actions/__spec__/test_package_check.py` & `dplib_py-0.7.6/dplib/actions/__spec__/test_package_check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/actions/__spec__/test_resource_check.py` & `dplib_py-0.7.6/dplib/actions/__spec__/test_resource_check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/actions/__spec__/test_schema_check.py` & `dplib_py-0.7.6/dplib/actions/__spec__/test_schema_check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/actions/dialect/check.py` & `dplib_py-0.7.6/dplib/actions/dialect/check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/actions/metadata/check.py` & `dplib_py-0.7.6/dplib/actions/metadata/check.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 from typing import List, Union
 
 from ... import settings, types
 from ...errors.metadata import MetadataError
-from ...helpers.data import read_data
-from ...helpers.profile import check_profile
+from ...helpers.dict import read_dict
+from ...helpers.profile import check_against_profile
 
 
 def check_metadata(
     metadata: Union[str, types.IDict], *, type: types.IMetadataType
 ) -> List[MetadataError]:
     if isinstance(metadata, str):
-        metadata = read_data(metadata)
+        metadata = read_dict(metadata)
 
     # Get default profile
     if type == "dialect":
         default_profile = settings.PROFILE_DEFAULT_DIALECT
     elif type == "package":
         default_profile = settings.PROFILE_DEFAULT_PACKAGE
     elif type == "resource":
@@ -24,10 +24,10 @@
     elif type == "schema":
         default_profile = settings.PROFILE_DEFAULT_SCHEMA
     else:
         raise ValueError(f"Invalid metadata type: {type}")
 
     # Validate metadata
     profile = metadata.get("$schema", default_profile)
-    errors = check_profile(metadata=metadata, profile=profile)
+    errors = check_against_profile(metadata=metadata, profile=profile)
 
     return errors
```

### Comparing `dplib_py-0.7.5/dplib/actions/metadata/convert.py` & `dplib_py-0.7.6/dplib/actions/metadata/convert.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/actions/package/check.py` & `dplib_py-0.7.6/dplib/actions/package/check.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import List, Union
 
 from ... import types
 from ...errors.metadata import MetadataError
-from ...helpers.data import read_data
-from ...helpers.path import infer_basepath
+from ...helpers.dict import read_dict
+from ...helpers.path import assert_safe_path, infer_basepath
 from ...models import Package
 from ..metadata.check import check_metadata
 
 
 def check_package(package: Union[str, types.IDict, Package]) -> List[MetadataError]:
     """Check the validity of a Data Package descriptor
 
@@ -21,24 +21,25 @@
 
     Returns:
         A list of errors
     """
     basepath = None
     if isinstance(package, str):
         basepath = infer_basepath(package)
-        package = read_data(package)
+        package = read_dict(package)
     if isinstance(package, Package):
         basepath = package.basepath
         package = package.to_dict()
 
     # Validate (including nested descriptors)
     errors = check_metadata(package, type="package")
     resources = package.get("resources", [])
     if isinstance(resources, list):
         for resource in resources:  # type: ignore
             for type in ["dialect", "schema"]:
                 value = resource.get(type)  # type: ignore
                 if isinstance(value, str):
-                    metadata = read_data(value, basepath=basepath)
+                    assert_safe_path(value, basepath=basepath)
+                    metadata = read_dict(value, basepath=basepath)
                     errors.extend(check_metadata(metadata, type=type))  # type: ignore
 
     return errors
```

### Comparing `dplib_py-0.7.5/dplib/actions/package/convert.py` & `dplib_py-0.7.6/dplib/actions/package/convert.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/actions/resource/check.py` & `dplib_py-0.7.6/dplib/actions/resource/check.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import List, Union
 
 from ... import types
 from ...errors.metadata import MetadataError
-from ...helpers.data import read_data
-from ...helpers.path import infer_basepath
+from ...helpers.dict import read_dict
+from ...helpers.path import assert_safe_path, infer_basepath
 from ...models import Resource
 from ..metadata.check import check_metadata
 
 
 def check_resource(resource: Union[str, types.IDict, Resource]) -> List[MetadataError]:
     """Check the validity of a Data Resource descriptor
 
@@ -21,21 +21,22 @@
 
     Returns:
         A list of errors
     """
     basepath = None
     if isinstance(resource, str):
         basepath = infer_basepath(resource)
-        resource = read_data(resource)
+        resource = read_dict(resource)
     if isinstance(resource, Resource):
         basepath = resource.basepath
         resource = resource.to_dict()
 
     # Validate (including nested descriptors)
     errors = check_metadata(resource, type="resource")
     for type in ["dialect", "schema"]:
         value = resource.get(type)
         if isinstance(value, str):
-            metadata = read_data(value, basepath=basepath)
+            assert_safe_path(value, basepath=basepath)
+            metadata = read_dict(value, basepath=basepath)
             errors.extend(check_metadata(metadata, type=type))  # type: ignore
 
     return errors
```

### Comparing `dplib_py-0.7.5/dplib/actions/resource/convert.py` & `dplib_py-0.7.6/dplib/actions/resource/convert.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/actions/schema/check.py` & `dplib_py-0.7.6/dplib/actions/schema/check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/errors/metadata.py` & `dplib_py-0.7.6/dplib/errors/metadata.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/helpers/data.py` & `dplib_py-0.7.6/dplib/helpers/dict.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,58 +6,58 @@
 
 from .. import types
 from ..error import Error
 from .file import read_file, write_file
 from .path import infer_format
 
 
-def read_data(
+def read_dict(
     path: str, *, format: Optional[str] = None, basepath: Optional[str] = None
 ) -> types.IDict:
     if not format:
         format = infer_format(path, raise_missing=True)
     text = read_file(path, basepath=basepath)
-    data = load_data(text, format=format)
+    data = load_dict(text, format=format)
     return data
 
 
-def write_data(path: str, data: types.IDict, *, format: Optional[str] = None):
+def write_dict(path: str, data: types.IDict, *, format: Optional[str] = None):
     if not format:
         format = infer_format(path, raise_missing=True)
-    text = dump_data(data, format=format)
+    text = dump_dict(data, format=format)
     write_file(path, text)
 
 
-def load_data(text: str, *, format: str) -> types.IDict:
+def load_dict(text: str, *, format: str) -> types.IDict:
     try:
         if format == "json":
             return json.loads(text)
         elif format == "yaml":
             yaml = import_module("yaml")
             return yaml.safe_load(text)
     except Exception:
         raise Error(f'Cannot load "{format}" data from text: {text}')
     raise Error(f"Cannot load data from text with format: {format}")
 
 
-def dump_data(data: types.IDict, *, format: str) -> str:
+def dump_dict(data: types.IDict, *, format: str) -> str:
     try:
         if format == "json":
             return json.dumps(data, indent=2)
         elif format == "yaml":
             yaml = import_module("yaml")
             return yaml.dump(data)
     except Exception:
         raise Error(f'Cannot dump "{format}" text from data: {data}')
     raise Error(f"Cannot dump data to text with format: {format}")
 
 
-def clean_data(data: types.IDict):
+def clean_dict(data: types.IDict):
     for key, value in list(data.items()):
         if isinstance(value, dict):
-            clean_data(value)  # type: ignore
+            clean_dict(value)  # type: ignore
         elif isinstance(value, list):
             for item in value:  # type: ignore
                 if isinstance(item, dict):
-                    clean_data(item)  # type: ignore
+                    clean_dict(item)  # type: ignore
         if value is None or value == [] or value == {}:
             data.pop(key)
```

### Comparing `dplib_py-0.7.5/dplib/helpers/file.py` & `dplib_py-0.7.6/dplib/helpers/file.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/helpers/path.py` & `dplib_py-0.7.6/dplib/helpers/path.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     if not format and raise_missing:
         raise Error(f"Cannot infer format from path: {path}")
     return format
 
 
 def infer_basepath(path: str):
     basepath = os.path.dirname(path)
-    if basepath and not is_remote_path(basepath):
+    if basepath and not is_url_path(basepath):
         if not os.path.abspath(basepath):
             basepath = os.path.relpath(basepath, start=os.getcwd())
     return basepath
 
 
 def ensure_basepath(path: str, basepath: Optional[str] = None) -> Tuple[str, str]:
     if basepath:
@@ -34,22 +34,27 @@
         basepath = infer_basepath(path)
     return path, basepath
 
 
 def join_basepath(path: str, basepath: Optional[str] = None) -> str:
     if not basepath:
         return path
-    if is_remote_path(path):
+    if is_url_path(path):
         return path
-    if is_remote_path(basepath):
+    if is_url_path(basepath):
         return f"{basepath}/{path}"
     return os.path.join(basepath, path)
 
 
-def is_remote_path(path: str) -> bool:
-    path = path[0] if path and isinstance(path, list) else path
+def is_url_path(path: str) -> bool:
     scheme = urlparse(path).scheme
-    if not scheme:
-        return False
-    if path.lower().startswith(scheme + ":\\"):
-        return False
-    return True
+    return scheme in ["http", "https"]
+
+
+def assert_safe_path(path: str, *, basepath: Optional[str] = None):
+    """Assert that the path (untrusted) is not outside the basepath (trusted)"""
+    try:
+        root = Path(basepath or os.getcwd()).resolve()
+        item = root.joinpath(path).resolve()
+        item.relative_to(root)
+    except Exception:
+        raise Error(f"Path is not safe: {path}")
```

### Comparing `dplib_py-0.7.5/dplib/helpers/profile.py` & `dplib_py-0.7.6/dplib/helpers/profile.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 from typing import List
 
 from jsonschema.validators import validator_for  # type: ignore
 
 from .. import settings, types
 from ..error import Error
 from ..errors.metadata import MetadataError
-from .data import load_data
+from .dict import load_dict
 from .file import read_file
+from .path import is_url_path
 
 # TODO: implement additional user-side profile caching
 
 
-def check_profile(*, metadata: types.IDict, profile: str) -> List[MetadataError]:
+def check_against_profile(*, metadata: types.IDict, profile: str) -> List[MetadataError]:
     # Prepare validator
     jsonSchema = read_profile(profile=profile)
     Validator = validator_for(jsonSchema)  # type: ignore
     validator = Validator(jsonSchema)  # type: ignore
 
     # Validate metadata
     errors: List[MetadataError] = []
@@ -34,20 +35,31 @@
     parts = parse_profile(profile)
 
     # Replace with builtin copy
     if parts:
         version, filename = parts
         profile = os.path.join(settings.PROFILE_BASEDIR, version, filename)
 
+    # Ensure profile is URL
+    if not is_url_path(profile):
+        raise Error(f'Profile MUST be a URL: "{profile}"')
+
     # Read jsonSchema
     try:
         text = read_file(profile)
-        data = load_data(text, format="json")
+        data = load_dict(text, format="json")
+    except Exception:
+        raise Error(f'Profile MUST be resolvable: "{profile}"')
+
+    # Validate jsonSchema
+    try:
+        Validator = validator_for(data)  # type: ignore
+        Validator.check_schema(data)  # type: ignore
     except Exception:
-        raise Error(f'Cannot read profile: "{profile}"')
+        raise Error(f'Profile MUST resolve to a valid JSON Schema: "{profile}"')
 
     return data
 
 
 def parse_profile(profile: str):
     parts = profile.rsplit("/", 3)
```

### Comparing `dplib_py-0.7.5/dplib/models/contributor.py` & `dplib_py-0.7.6/dplib/models/contributor.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/models/dialect/dialect.py` & `dplib_py-0.7.6/dplib/models/dialect/dialect.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/models/dialect/__spec__/test_dialect.py` & `dplib_py-0.7.6/dplib/models/dialect/__spec__/test_dialect.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/models/field/types.py` & `dplib_py-0.7.6/dplib/models/field/types.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/models/field/__spec__/test_field.py` & `dplib_py-0.7.6/dplib/models/field/__spec__/test_field.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/models/field/datatypes/__init__.py` & `dplib_py-0.7.6/dplib/models/field/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/models/field/datatypes/base.py` & `dplib_py-0.7.6/dplib/models/field/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/models/field/datatypes/boolean.py` & `dplib_py-0.7.6/dplib/models/field/datatypes/boolean.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/models/field/datatypes/geojson.py` & `dplib_py-0.7.6/dplib/models/field/datatypes/geojson.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/models/field/datatypes/geopoint.py` & `dplib_py-0.7.6/dplib/models/field/datatypes/geopoint.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/models/field/datatypes/integer.py` & `dplib_py-0.7.6/dplib/models/field/datatypes/integer.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/models/field/datatypes/list.py` & `dplib_py-0.7.6/dplib/models/field/datatypes/list.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/models/field/datatypes/number.py` & `dplib_py-0.7.6/dplib/models/field/datatypes/number.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/models/field/datatypes/string.py` & `dplib_py-0.7.6/dplib/models/field/datatypes/string.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/models/package/package.py` & `dplib_py-0.7.6/dplib/models/package/package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/models/package/__spec__/test_package.py` & `dplib_py-0.7.6/dplib/models/package/__spec__/test_package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/models/resource/hash.py` & `dplib_py-0.7.6/dplib/models/resource/hash.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/models/resource/resource.py` & `dplib_py-0.7.6/dplib/models/resource/resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from typing import Any, List, Optional, Union
 
 import pydantic
 
 from ... import settings, types
 from ...helpers.file import join_basepath
+from ...helpers.path import assert_safe_path
 from ...system import Model
 from ..contributor import Contributor
 from ..dialect import Dialect
 from ..license import License
 from ..schema import Schema
 from ..source import Source
 from .hash import Hash
@@ -171,16 +172,18 @@
     # Methods
 
     def dereference(self):
         """Dereference the package
         It will dereference all the resource's dialects and schemas
         """
         if isinstance(self.dialect, str):
+            assert_safe_path(self.dialect, basepath=self.basepath)
             self.dialect = Dialect.from_path(self.dialect, basepath=self.basepath)
         if isinstance(self.schema, str):
+            assert_safe_path(self.schema, basepath=self.basepath)
             self.schema = Schema.from_path(self.schema, basepath=self.basepath)  # type: ignore
 
     # Converters
 
     def to_dict(self):
         data = {"$schema": settings.PROFILE_CURRENT_RESOURCE}
         data.update(super().to_dict())
```

### Comparing `dplib_py-0.7.5/dplib/models/resource/__spec__/test_resource.py` & `dplib_py-0.7.6/dplib/models/resource/__spec__/test_resource.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/models/schema/foreignKey.py` & `dplib_py-0.7.6/dplib/models/schema/foreignKey.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/models/schema/schema.py` & `dplib_py-0.7.6/dplib/models/schema/schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/models/schema/__spec__/test_schema.py` & `dplib_py-0.7.6/dplib/models/schema/__spec__/test_schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/ckan/models/field.py` & `dplib_py-0.7.6/dplib/plugins/ckan/models/field.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/ckan/models/package.py` & `dplib_py-0.7.6/dplib/plugins/ckan/models/package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/ckan/models/resource.py` & `dplib_py-0.7.6/dplib/plugins/ckan/models/resource.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/ckan/models/schema.py` & `dplib_py-0.7.6/dplib/plugins/ckan/models/schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/ckan/models/__spec__/test_package.py` & `dplib_py-0.7.6/dplib/plugins/ckan/models/__spec__/test_package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/cli/program.py` & `dplib_py-0.7.6/dplib/plugins/cli/program.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/cli/commands/main.py` & `dplib_py-0.7.6/dplib/plugins/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/cli/commands/package/convert.py` & `dplib_py-0.7.6/dplib/plugins/cli/commands/package/convert.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/cli/commands/resource/convert.py` & `dplib_py-0.7.6/dplib/plugins/cli/commands/resource/convert.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/cli/helpers/check.py` & `dplib_py-0.7.6/dplib/plugins/cli/helpers/check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/datacite/models/contributor.py` & `dplib_py-0.7.6/dplib/plugins/datacite/models/contributor.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/datacite/models/package.py` & `dplib_py-0.7.6/dplib/plugins/datacite/models/package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/datacite/models/__spec__/test_package.py` & `dplib_py-0.7.6/dplib/plugins/datacite/models/__spec__/test_package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/dcat/models/helpers.py` & `dplib_py-0.7.6/dplib/plugins/dcat/models/helpers.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/dcat/models/loaders.py` & `dplib_py-0.7.6/dplib/plugins/dcat/models/loaders.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/dcat/models/namespaces.py` & `dplib_py-0.7.6/dplib/plugins/dcat/models/namespaces.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/dcat/models/package.py` & `dplib_py-0.7.6/dplib/plugins/dcat/models/package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/dcat/models/resource.py` & `dplib_py-0.7.6/dplib/plugins/dcat/models/resource.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/dcat/models/__spec__/test_package.py` & `dplib_py-0.7.6/dplib/plugins/dcat/models/__spec__/test_package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/github/models/package.py` & `dplib_py-0.7.6/dplib/plugins/github/models/package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/github/models/resource.py` & `dplib_py-0.7.6/dplib/plugins/github/models/resource.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/github/models/__spec__/test_package.py` & `dplib_py-0.7.6/dplib/plugins/github/models/__spec__/test_package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/pandas/models/field.py` & `dplib_py-0.7.6/dplib/plugins/pandas/models/field.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/pandas/models/schema.py` & `dplib_py-0.7.6/dplib/plugins/pandas/models/schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/polars/models/field.py` & `dplib_py-0.7.6/dplib/plugins/polars/models/field.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/polars/models/schema.py` & `dplib_py-0.7.6/dplib/plugins/polars/models/schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/polars/models/__spec__/test_schema.py` & `dplib_py-0.7.6/dplib/plugins/polars/models/__spec__/test_schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/sql/models/field.py` & `dplib_py-0.7.6/dplib/plugins/sql/models/field.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/sql/models/schema.py` & `dplib_py-0.7.6/dplib/plugins/sql/models/schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/sql/models/__spec__/test_schema.py` & `dplib_py-0.7.6/dplib/plugins/sql/models/__spec__/test_schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/zenodo/models/contributor.py` & `dplib_py-0.7.6/dplib/plugins/zenodo/models/contributor.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/zenodo/models/metadata.py` & `dplib_py-0.7.6/dplib/plugins/zenodo/models/metadata.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/zenodo/models/package.py` & `dplib_py-0.7.6/dplib/plugins/zenodo/models/package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/zenodo/models/resource.py` & `dplib_py-0.7.6/dplib/plugins/zenodo/models/resource.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/zenodo/models/right.py` & `dplib_py-0.7.6/dplib/plugins/zenodo/models/right.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/plugins/zenodo/models/__spec__/test_package.py` & `dplib_py-0.7.6/dplib/plugins/zenodo/models/__spec__/test_package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/profiles/1.0/datapackage.json` & `dplib_py-0.7.6/dplib/profiles/1.0/datapackage.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/profiles/1.0/dataresource.json` & `dplib_py-0.7.6/dplib/profiles/1.0/dataresource.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/profiles/1.0/tabledialect.json` & `dplib_py-0.7.6/dplib/profiles/1.0/tabledialect.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/profiles/1.0/tableschema.json` & `dplib_py-0.7.6/dplib/profiles/1.0/tableschema.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/profiles/2.0/datapackage.json` & `dplib_py-0.7.6/dplib/profiles/2.0/datapackage.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/profiles/2.0/dataresource.json` & `dplib_py-0.7.6/dplib/profiles/2.0/dataresource.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/profiles/2.0/tabledialect.json` & `dplib_py-0.7.6/dplib/profiles/2.0/tabledialect.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/profiles/2.0/tableschema.json` & `dplib_py-0.7.6/dplib/profiles/2.0/tableschema.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/dplib/system/model.py` & `dplib_py-0.7.6/dplib/system/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Optional
 
 from pydantic import BaseModel
 from typing_extensions import Self
 
 from .. import types
 from ..error import Error
-from ..helpers.data import clean_data, dump_data, load_data
+from ..helpers.dict import clean_dict, dump_dict, load_dict
 from ..helpers.file import read_file, write_file
 from ..helpers.path import ensure_basepath, infer_format
 
 
 class Model(BaseModel, extra="allow", validate_assignment=True):
     def __str__(self) -> str:
         return repr(self)
@@ -44,27 +44,27 @@
         text = read_file(path)
         if not text:
             raise Error(f"The file is empty: {path}")
         return cls.from_text(text, format=format, basepath=basepath)
 
     def to_text(self, *, format: str) -> str:
         data = self.to_dict()
-        text = dump_data(data, format=format)
+        text = dump_dict(data, format=format)
         return text
 
     @classmethod
     def from_text(cls, text: str, *, format: str, basepath: Optional[str] = None) -> Self:
-        data = load_data(text, format=format)
+        data = load_dict(text, format=format)
         return cls.from_dict(data, basepath=basepath)
 
     def to_dict(self):
         data = self.model_dump(
             mode="json", by_alias=True, exclude_none=True, exclude_defaults=True
         )
-        clean_data(data)
+        clean_dict(data)
         return data
 
     @classmethod
     def from_dict(cls, data: types.IDict, *, basepath: Optional[str] = None) -> Self:
         if basepath and cls.model_fields.get("basepath"):
             data["basepath"] = basepath
         return cls(**data)
```

### Comparing `dplib_py-0.7.5/dplib/system/__spec__/test_model.py` & `dplib_py-0.7.6/dplib/system/__spec__/test_model.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/.gitignore` & `dplib_py-0.7.6/.gitignore`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/LICENSE.md` & `dplib_py-0.7.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/README.md` & `dplib_py-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/pyproject.toml` & `dplib_py-0.7.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.5/PKG-INFO` & `dplib_py-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dplib-py
-Version: 0.7.5
+Version: 0.7.6
 Summary: Python implementation of the Data Package standard
 Project-URL: homepage, https://github.com/frictionlessdata/dplib-py
 Author-email: Open Knowledge Foundation <info@okfn.org>
 License-Expression: MIT
 License-File: LICENSE.md
 Keywords: data package,data validation,json schema,json table schema,open data,tabular data package
 Classifier: Development Status :: 4 - Beta
```

