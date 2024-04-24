# Comparing `tmp/dplib_py-0.7.3.tar.gz` & `tmp/dplib_py-0.7.4.tar.gz`

## Comparing `dplib_py-0.7.3.tar` & `dplib_py-0.7.4.tar`

### file list

```diff
@@ -1,266 +1,269 @@
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 dplib_py-0.7.3/mkdocs.yaml
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dplib_py-0.7.3/.github/codecov.yaml
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dplib_py-0.7.3/.github/issue_template.md
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 dplib_py-0.7.3/.github/pull_request_template.md
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dplib_py-0.7.3/.github/stale.yaml
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 dplib_py-0.7.3/.github/workflows/general.yaml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/dialect-full.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/dialect-invalid.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/dialect.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/empty.json
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/package-custom-profile.json
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/package-full.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/package-invalid-dereferencing.json
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/package-invalid.json
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/package.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/profile.json
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/resource-full.json
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/resource-invalid-dereferencing.json
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/resource-invalid.json
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/resource.json
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/resource.yaml
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/schema-full.json
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/schema-invalid.json
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/schema-types.json
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/schema.json
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/text.txt
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/cassettes/test_check_package_custom_profile.yaml
--rw-r--r--   0        0        0    14982 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/cassettes/test_dialect_profile.yaml
--rw-r--r--   0        0        0    60589 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/cassettes/test_package_profile.yaml
--rw-r--r--   0        0        0   220871 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/cassettes/test_resource_profile.yaml
--rw-r--r--   0        0        0   169730 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/cassettes/test_schema_profile.yaml
--rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/plugins/ckan/package.json
--rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/plugins/datacite/package.json
--rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/plugins/dcat/package.xml
--rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/plugins/github/package.json
--rw-r--r--   0        0        0     7431 2020-02-02 00:00:00.000000 dplib_py-0.7.3/data/plugins/zenodo/package.json
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/changelog.md
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/contributing.md
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/converting-metadata.md
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/index.md
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/installation.md
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/validating-metadata.md
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/working-with-models.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/.theme/.keep
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/actions/dialect.md
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/actions/package.md
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/actions/resource.md
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/actions/schema.md
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/assets/favicon-color.png
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/assets/favicon-shaddow.png
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/assets/favicon.ico
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/assets/favicon.png
--rw-r--r--   0        0        0     8911 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/assets/logo-dark.svg
--rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/assets/logo-light.svg
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/models/dialect.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/models/package.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/models/resource.md
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/models/schema.md
--rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/plugins/ckan.md
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/plugins/cli.md
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/plugins/datacite.md
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/plugins/dcat.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/plugins/github.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/plugins/pandas.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/plugins/polars.md
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/plugins/sql.md
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 dplib_py-0.7.3/docs/plugins/zenodo.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/__init__.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/conftest.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/error.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/py.typed
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/settings.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/actions/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/actions/__spec__/test_dialect_check.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/actions/__spec__/test_package_check.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/actions/__spec__/test_resource_check.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/actions/__spec__/test_schema_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/actions/dialect/__init__.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/actions/dialect/check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/actions/metadata/__init__.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/actions/metadata/check.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/actions/metadata/convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/actions/package/__init__.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/actions/package/check.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/actions/package/convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/actions/resource/__init__.py
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/actions/resource/check.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/actions/resource/convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/actions/schema/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/actions/schema/check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/errors/__init__.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/errors/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/helpers/__init__.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/helpers/data.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/helpers/file.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/helpers/path.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/helpers/profile.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/helpers/resource.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/__init__.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/contributor.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/license.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/source.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/dialect/__init__.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/dialect/dialect.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/dialect/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/dialect/__spec__/__init__.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/dialect/__spec__/test_dialect.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/__init__.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/field.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/types.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/__spec__/test_field.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/constraints/__init__.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/constraints/base.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/constraints/collection.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/constraints/json.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/constraints/string.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/constraints/value.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/datatypes/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/datatypes/any.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/datatypes/array.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/datatypes/base.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/datatypes/boolean.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/datatypes/date.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/datatypes/datetime.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/datatypes/duration.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/datatypes/geojson.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/datatypes/geopoint.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/datatypes/integer.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/datatypes/list.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/datatypes/number.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/datatypes/object.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/datatypes/string.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/datatypes/time.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/datatypes/year.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/field/datatypes/yearmonth.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/package/__init__.py
--rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/package/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/package/__spec__/__init__.py
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/package/__spec__/test_package.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/resource/__init__.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/resource/hash.py
--rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/resource/resource.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/resource/__spec__/__init__.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/resource/__spec__/test_resource.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/resource/datatypes/__init__.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/resource/datatypes/table.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/schema/__init__.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/schema/foreignKey.py
--rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/schema/schema.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/schema/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/schema/__spec__/__init__.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/models/schema/__spec__/test_schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/ckan/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/ckan/models/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/ckan/models/organization.py
--rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/ckan/models/package.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/ckan/models/resource.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/ckan/models/tag.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/ckan/models/__spec__/__init__.py
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/ckan/models/__spec__/test_package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/__init__.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/__main__.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/program.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/commands/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/commands/main.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/commands/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/commands/__spec__/__init__.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/commands/__spec__/test_version.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/commands/dialect/__init__.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/commands/dialect/check.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/commands/dialect/main.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/commands/package/__init__.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/commands/package/check.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/commands/package/convert.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/commands/package/main.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/commands/resource/__init__.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/commands/resource/check.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/commands/resource/convert.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/commands/resource/main.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/commands/schema/__init__.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/commands/schema/check.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/commands/schema/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/helpers/__init__.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/helpers/check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/options/__init__.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/options/convert.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/options/path.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/cli/options/system.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/datacite/__init__.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/datacite/models/__init__.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/datacite/models/contributor.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/datacite/models/description.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/datacite/models/identifier.py
--rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/datacite/models/package.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/datacite/models/rights.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/datacite/models/subject.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/datacite/models/title.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/datacite/models/__spec__/__init__.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/datacite/models/__spec__/test_package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/dcat/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/dcat/models/__init__.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/dcat/models/dumpers.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/dcat/models/helpers.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/dcat/models/loaders.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/dcat/models/namespaces.py
--rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/dcat/models/package.py
--rw-r--r--   0        0        0     6362 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/dcat/models/resource.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/dcat/models/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/dcat/models/__spec__/__init__.py
--rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/dcat/models/__spec__/test_package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/github/__init__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/github/models/__init__.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/github/models/license.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/github/models/owner.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/github/models/package.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/github/models/resource.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/github/models/__spec__/__init__.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/github/models/__spec__/test_package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/pandas/__init__.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/pandas/models/__init__.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/pandas/models/field.py
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/pandas/models/schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/pandas/models/__spec__/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/polars/__init__.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/polars/models/__init__.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/polars/models/field.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/polars/models/schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/polars/models/__spec__/__init__.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/polars/models/__spec__/test_schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/sql/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/sql/models/__init__.py
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/sql/models/field.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/sql/models/schema.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/sql/models/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/sql/models/__spec__/__init__.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/sql/models/__spec__/test_schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/zenodo/__init__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/zenodo/models/__init__.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/zenodo/models/creator.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/zenodo/models/files.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/zenodo/models/metadata.py
--rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/zenodo/models/package.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/zenodo/models/pid.py
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/zenodo/models/resource.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/zenodo/models/subject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/zenodo/models/__spec__/__init__.py
--rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/plugins/zenodo/models/__spec__/test_package.py
--rw-r--r--   0        0        0   107095 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/profiles/1.0/datapackage.json
--rw-r--r--   0        0        0    85332 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/profiles/1.0/dataresource.json
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/profiles/1.0/tabledialect.json
--rw-r--r--   0        0        0    65533 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/profiles/1.0/tableschema.json
--rw-r--r--   0        0        0   142568 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/profiles/2.0/datapackage.json
--rw-r--r--   0        0        0   117144 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/profiles/2.0/dataresource.json
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/profiles/2.0/tabledialect.json
--rw-r--r--   0        0        0    94827 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/profiles/2.0/tableschema.json
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/system/__init__.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/system/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/system/__spec__/__init__.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 dplib_py-0.7.3/dplib/system/__spec__/test_model.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 dplib_py-0.7.3/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 dplib_py-0.7.3/LICENSE.md
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 dplib_py-0.7.3/README.md
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 dplib_py-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 dplib_py-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 dplib_py-0.7.4/mkdocs.yaml
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dplib_py-0.7.4/.github/codecov.yaml
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dplib_py-0.7.4/.github/issue_template.md
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 dplib_py-0.7.4/.github/pull_request_template.md
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dplib_py-0.7.4/.github/stale.yaml
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 dplib_py-0.7.4/.github/workflows/general.yaml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/dialect-full.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/dialect-invalid.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/dialect.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/empty.json
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/package-custom-profile.json
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/package-full.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/package-invalid-dereferencing.json
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/package-invalid.json
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/package.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/profile.json
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/resource-full.json
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/resource-invalid-dereferencing.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/resource-invalid.json
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/resource.json
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/resource.yaml
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/schema-full.json
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/schema-invalid.json
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/schema-types.json
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/schema.json
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/text.txt
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/cassettes/test_check_package_custom_profile.yaml
+-rw-r--r--   0        0        0    14982 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/cassettes/test_dialect_profile.yaml
+-rw-r--r--   0        0        0    60589 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/cassettes/test_package_profile.yaml
+-rw-r--r--   0        0        0   220871 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/cassettes/test_resource_profile.yaml
+-rw-r--r--   0        0        0   169730 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/cassettes/test_schema_profile.yaml
+-rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/plugins/ckan/package.json
+-rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/plugins/datacite/package.json
+-rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/plugins/dcat/package.xml
+-rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/plugins/github/package.json
+-rw-r--r--   0        0        0     7431 2020-02-02 00:00:00.000000 dplib_py-0.7.4/data/plugins/zenodo/package.json
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/changelog.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/contributing.md
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/converting-metadata.md
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/index.md
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/installation.md
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/validating-metadata.md
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/working-with-models.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/.theme/.keep
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/actions/dialect.md
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/actions/package.md
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/actions/resource.md
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/actions/schema.md
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/assets/favicon-color.png
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/assets/favicon-shaddow.png
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/assets/favicon.ico
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/assets/favicon.png
+-rw-r--r--   0        0        0     8911 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/assets/logo-dark.svg
+-rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/assets/logo-light.svg
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/models/dialect.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/models/package.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/models/resource.md
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/models/schema.md
+-rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/plugins/ckan.md
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/plugins/cli.md
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/plugins/datacite.md
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/plugins/dcat.md
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/plugins/github.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/plugins/pandas.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/plugins/polars.md
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/plugins/sql.md
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 dplib_py-0.7.4/docs/plugins/zenodo.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/__init__.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/conftest.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/error.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/py.typed
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/settings.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/actions/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/actions/__spec__/test_dialect_check.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/actions/__spec__/test_package_check.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/actions/__spec__/test_resource_check.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/actions/__spec__/test_schema_check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/actions/dialect/__init__.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/actions/dialect/check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/actions/metadata/__init__.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/actions/metadata/check.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/actions/metadata/convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/actions/package/__init__.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/actions/package/check.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/actions/package/convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/actions/resource/__init__.py
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/actions/resource/check.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/actions/resource/convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/actions/schema/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/actions/schema/check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/errors/__init__.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/errors/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/helpers/__init__.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/helpers/data.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/helpers/file.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/helpers/path.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/helpers/profile.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/helpers/resource.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/__init__.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/contributor.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/license.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/source.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/dialect/__init__.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/dialect/dialect.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/dialect/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/dialect/__spec__/__init__.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/dialect/__spec__/test_dialect.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/__init__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/field.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/types.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/__spec__/test_field.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/constraints/__init__.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/constraints/base.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/constraints/collection.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/constraints/json.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/constraints/string.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/constraints/value.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/datatypes/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/datatypes/any.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/datatypes/array.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/datatypes/base.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/datatypes/boolean.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/datatypes/date.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/datatypes/datetime.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/datatypes/duration.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/datatypes/geojson.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/datatypes/geopoint.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/datatypes/integer.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/datatypes/list.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/datatypes/number.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/datatypes/object.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/datatypes/string.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/datatypes/time.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/datatypes/year.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/field/datatypes/yearmonth.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/package/__init__.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/package/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/package/__spec__/__init__.py
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/package/__spec__/test_package.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/resource/__init__.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/resource/hash.py
+-rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/resource/resource.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/resource/__spec__/__init__.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/resource/__spec__/test_resource.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/resource/datatypes/__init__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/resource/datatypes/table.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/schema/__init__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/schema/foreignKey.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/schema/schema.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/schema/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/schema/__spec__/__init__.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/models/schema/__spec__/test_schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/ckan/__init__.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/ckan/models/__init__.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/ckan/models/field.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/ckan/models/organization.py
+-rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/ckan/models/package.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/ckan/models/resource.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/ckan/models/schema.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/ckan/models/tag.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/ckan/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/ckan/models/__spec__/test_package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/__init__.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/__main__.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/program.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/commands/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/commands/main.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/commands/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/commands/__spec__/__init__.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/commands/__spec__/test_version.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/commands/dialect/__init__.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/commands/dialect/check.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/commands/dialect/main.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/commands/package/__init__.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/commands/package/check.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/commands/package/convert.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/commands/package/main.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/commands/resource/__init__.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/commands/resource/check.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/commands/resource/convert.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/commands/resource/main.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/commands/schema/__init__.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/commands/schema/check.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/commands/schema/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/helpers/__init__.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/helpers/check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/options/__init__.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/options/convert.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/options/path.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/cli/options/system.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/datacite/__init__.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/datacite/models/__init__.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/datacite/models/contributor.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/datacite/models/description.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/datacite/models/identifier.py
+-rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/datacite/models/package.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/datacite/models/rights.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/datacite/models/subject.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/datacite/models/title.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/datacite/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/datacite/models/__spec__/test_package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/dcat/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/dcat/models/__init__.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/dcat/models/dumpers.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/dcat/models/helpers.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/dcat/models/loaders.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/dcat/models/namespaces.py
+-rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/dcat/models/package.py
+-rw-r--r--   0        0        0     6362 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/dcat/models/resource.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/dcat/models/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/dcat/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/dcat/models/__spec__/test_package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/github/__init__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/github/models/__init__.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/github/models/license.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/github/models/owner.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/github/models/package.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/github/models/resource.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/github/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/github/models/__spec__/test_package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/pandas/__init__.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/pandas/models/__init__.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/pandas/models/field.py
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/pandas/models/schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/pandas/models/__spec__/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/polars/__init__.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/polars/models/__init__.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/polars/models/field.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/polars/models/schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/polars/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/polars/models/__spec__/test_schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/sql/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/sql/models/__init__.py
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/sql/models/field.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/sql/models/schema.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/sql/models/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/sql/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/sql/models/__spec__/test_schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/zenodo/__init__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/zenodo/models/__init__.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/zenodo/models/contributor.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/zenodo/models/files.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/zenodo/models/metadata.py
+-rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/zenodo/models/package.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/zenodo/models/pid.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/zenodo/models/resource.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/zenodo/models/right.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/zenodo/models/subject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/zenodo/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/plugins/zenodo/models/__spec__/test_package.py
+-rw-r--r--   0        0        0   107095 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/profiles/1.0/datapackage.json
+-rw-r--r--   0        0        0    85332 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/profiles/1.0/dataresource.json
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/profiles/1.0/tabledialect.json
+-rw-r--r--   0        0        0    65533 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/profiles/1.0/tableschema.json
+-rw-r--r--   0        0        0   142568 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/profiles/2.0/datapackage.json
+-rw-r--r--   0        0        0   117144 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/profiles/2.0/dataresource.json
+-rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/profiles/2.0/tabledialect.json
+-rw-r--r--   0        0        0    94827 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/profiles/2.0/tableschema.json
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/system/__init__.py
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/system/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/system/__spec__/__init__.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 dplib_py-0.7.4/dplib/system/__spec__/test_model.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 dplib_py-0.7.4/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 dplib_py-0.7.4/LICENSE.md
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 dplib_py-0.7.4/README.md
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 dplib_py-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 dplib_py-0.7.4/PKG-INFO
```

### Comparing `dplib_py-0.7.3/mkdocs.yaml` & `dplib_py-0.7.4/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/.github/stale.yaml` & `dplib_py-0.7.4/.github/stale.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/.github/workflows/general.yaml` & `dplib_py-0.7.4/.github/workflows/general.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/data/package-full.json` & `dplib_py-0.7.4/data/package-full.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/data/schema-full.json` & `dplib_py-0.7.4/data/schema-full.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/data/schema-types.json` & `dplib_py-0.7.4/data/schema-types.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/data/cassettes/test_check_package_custom_profile.yaml` & `dplib_py-0.7.4/data/cassettes/test_check_package_custom_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/data/cassettes/test_dialect_profile.yaml` & `dplib_py-0.7.4/data/cassettes/test_dialect_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/data/cassettes/test_package_profile.yaml` & `dplib_py-0.7.4/data/cassettes/test_package_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/data/cassettes/test_resource_profile.yaml` & `dplib_py-0.7.4/data/cassettes/test_resource_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/data/cassettes/test_schema_profile.yaml` & `dplib_py-0.7.4/data/cassettes/test_schema_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/data/plugins/ckan/package.json` & `dplib_py-0.7.4/data/plugins/ckan/package.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/data/plugins/datacite/package.json` & `dplib_py-0.7.4/data/plugins/datacite/package.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/data/plugins/dcat/package.xml` & `dplib_py-0.7.4/data/plugins/dcat/package.xml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/data/plugins/github/package.json` & `dplib_py-0.7.4/data/plugins/github/package.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/data/plugins/zenodo/package.json` & `dplib_py-0.7.4/data/plugins/zenodo/package.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/docs/contributing.md` & `dplib_py-0.7.4/docs/contributing.md`

 * *Files 10% similar despite different names*

```diff
@@ -34,21 +34,21 @@
 ```
 
 ## Documentation
 
 Documentation is written with Mkdocs (defined in `mkdocs.yaml`). The source articles are in the `docs` directory. To start a live-reload server:
 
 ```bash
-hatch run serve
+hatch run docs
 ```
 
 Building the docs:
 
 ```bash
-hatch run build
+hatch run docs-build
 ```
 
 ## Testing
 
 To run all the checks on the codebase:
 
 ```bash
```

### Comparing `dplib_py-0.7.3/docs/converting-metadata.md` & `dplib_py-0.7.4/docs/converting-metadata.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/docs/index.md` & `dplib_py-0.7.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/docs/validating-metadata.md` & `dplib_py-0.7.4/docs/validating-metadata.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/docs/working-with-models.md` & `dplib_py-0.7.4/docs/working-with-models.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/docs/assets/favicon-shaddow.png` & `dplib_py-0.7.4/docs/assets/favicon-shaddow.png`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/docs/assets/favicon.ico` & `dplib_py-0.7.4/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/docs/assets/logo-dark.svg` & `dplib_py-0.7.4/docs/assets/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/docs/assets/logo-light.svg` & `dplib_py-0.7.4/docs/assets/logo-light.svg`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/docs/models/package.md` & `dplib_py-0.7.4/docs/models/package.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/docs/models/resource.md` & `dplib_py-0.7.4/docs/models/resource.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/docs/models/schema.md` & `dplib_py-0.7.4/docs/models/schema.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/docs/plugins/ckan.md` & `dplib_py-0.7.4/docs/plugins/ckan.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/docs/plugins/cli.md` & `dplib_py-0.7.4/docs/plugins/cli.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/docs/plugins/datacite.md` & `dplib_py-0.7.4/docs/plugins/datacite.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/docs/plugins/dcat.md` & `dplib_py-0.7.4/docs/plugins/dcat.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/docs/plugins/github.md` & `dplib_py-0.7.4/docs/plugins/github.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/docs/plugins/pandas.md` & `dplib_py-0.7.4/docs/plugins/pandas.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/docs/plugins/polars.md` & `dplib_py-0.7.4/docs/plugins/polars.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/docs/plugins/sql.md` & `dplib_py-0.7.4/docs/plugins/sql.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/docs/plugins/zenodo.md` & `dplib_py-0.7.4/docs/plugins/zenodo.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/settings.py` & `dplib_py-0.7.4/dplib/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 # Version
 
-VERSION = "0.7.3"
+VERSION = "0.7.4"
 
 # Profiles
 
 PROFILE_BASEURL = "https://datapackage.org/profiles"
 PROFILE_BASEDIR = os.path.join(os.path.dirname(__file__), "profiles")
 
 PROFILE_DEFAULT = "1.0"
```

### Comparing `dplib_py-0.7.3/dplib/actions/__spec__/test_dialect_check.py` & `dplib_py-0.7.4/dplib/actions/__spec__/test_dialect_check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/actions/__spec__/test_package_check.py` & `dplib_py-0.7.4/dplib/actions/__spec__/test_package_check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/actions/__spec__/test_resource_check.py` & `dplib_py-0.7.4/dplib/actions/__spec__/test_resource_check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/actions/__spec__/test_schema_check.py` & `dplib_py-0.7.4/dplib/actions/__spec__/test_schema_check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/actions/dialect/check.py` & `dplib_py-0.7.4/dplib/actions/dialect/check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/actions/metadata/check.py` & `dplib_py-0.7.4/dplib/actions/metadata/check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/actions/metadata/convert.py` & `dplib_py-0.7.4/dplib/actions/metadata/convert.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/actions/package/check.py` & `dplib_py-0.7.4/dplib/actions/package/check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/actions/package/convert.py` & `dplib_py-0.7.4/dplib/actions/package/convert.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/actions/resource/check.py` & `dplib_py-0.7.4/dplib/actions/resource/check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/actions/resource/convert.py` & `dplib_py-0.7.4/dplib/actions/resource/convert.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/actions/schema/check.py` & `dplib_py-0.7.4/dplib/actions/schema/check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/errors/metadata.py` & `dplib_py-0.7.4/dplib/errors/metadata.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/helpers/data.py` & `dplib_py-0.7.4/dplib/helpers/data.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/helpers/file.py` & `dplib_py-0.7.4/dplib/helpers/file.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/helpers/path.py` & `dplib_py-0.7.4/dplib/helpers/path.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/helpers/profile.py` & `dplib_py-0.7.4/dplib/helpers/profile.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/models/contributor.py` & `dplib_py-0.7.4/dplib/models/contributor.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/models/dialect/dialect.py` & `dplib_py-0.7.4/dplib/models/dialect/dialect.py`

 * *Files 9% similar despite different names*

```diff
@@ -120,7 +120,12 @@
     This property specifies a sheet number of a table in the spreadsheet file.
     """
 
     sheetName: Optional[str] = None
     """
     This property specifies a sheet name of a table in the spreadsheet file.
     """
+
+    def to_dict(self):
+        data = {"$schema": settings.PROFILE_CURRENT_DIALECT}
+        data.update(super().to_dict())
+        return data
```

### Comparing `dplib_py-0.7.3/dplib/models/dialect/__spec__/test_dialect.py` & `dplib_py-0.7.4/dplib/models/dialect/__spec__/test_dialect.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 from pydantic import ValidationError
 
+from dplib import settings
 from dplib.models import Dialect
 
 
 def test_dialect_from_path():
     dialect = Dialect.from_path("data/dialect.json")
     assert dialect.delimiter == ";"
 
@@ -51,7 +52,24 @@
         Dialect.from_dict(data)
 
 
 def test_dialect_set_proprty_invalid():
     dialect = Dialect()
     with pytest.raises(ValidationError):
         dialect.delimiter = 1  # type: ignore
+
+
+def test_dialect_to_dict():
+    dialect = Dialect()
+    assert dialect.to_dict() == {
+        "$schema": settings.PROFILE_CURRENT_DIALECT,
+    }
+    dialect.delimiter = ";"
+    assert dialect.to_dict() == {
+        "$schema": settings.PROFILE_CURRENT_DIALECT,
+        "delimiter": ";",
+    }
+    dialect.profile = settings.PROFILE_DEFAULT_DIALECT
+    assert dialect.to_dict() == {
+        "$schema": settings.PROFILE_DEFAULT_DIALECT,
+        "delimiter": ";",
+    }
```

### Comparing `dplib_py-0.7.3/dplib/models/field/types.py` & `dplib_py-0.7.4/dplib/models/field/types.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/models/field/datatypes/__init__.py` & `dplib_py-0.7.4/dplib/models/field/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/models/field/datatypes/base.py` & `dplib_py-0.7.4/dplib/models/field/datatypes/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import List, Optional
+from typing import Any, List, Optional
 
 import pydantic
 
 from .... import types
 from ....system import Model
 
 
@@ -12,14 +12,20 @@
     """Base Field"""
 
     name: Optional[str] = None
     """
     The field descriptor MUST contain a name property.
     """
 
+    # TODO: use proper abstract type (str/Literal string don't work with subclasses)
+    type: Optional[Any] = None
+    """
+    A field type i.e. string, number, etc
+    """
+
     title: Optional[str] = None
     """
     A human readable label or title for the field
     """
 
     description: Optional[str] = None
     """
@@ -27,14 +33,19 @@
     """
 
     missingValues: List[str] = [""]
     """
     A list of field values to consider as null values
     """
 
+    # This method ensures that type is not omitted as defaults in model_dump
+    @pydantic.field_serializer("type")
+    def serialize_type(self, value: str, info: Any):
+        return value
+
     # Compat
 
     @pydantic.model_validator(mode="before")
     @classmethod
     def compat(cls, data: types.IDict):
         if not isinstance(data, dict):  # type: ignore
             return data
```

### Comparing `dplib_py-0.7.3/dplib/models/field/datatypes/boolean.py` & `dplib_py-0.7.4/dplib/models/field/datatypes/boolean.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/models/field/datatypes/geojson.py` & `dplib_py-0.7.4/dplib/models/field/datatypes/geojson.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/models/field/datatypes/geopoint.py` & `dplib_py-0.7.4/dplib/models/field/datatypes/geopoint.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/models/field/datatypes/integer.py` & `dplib_py-0.7.4/dplib/models/field/datatypes/integer.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/models/field/datatypes/list.py` & `dplib_py-0.7.4/dplib/models/field/datatypes/list.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/models/field/datatypes/number.py` & `dplib_py-0.7.4/dplib/models/field/datatypes/number.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/models/field/datatypes/string.py` & `dplib_py-0.7.4/dplib/models/field/datatypes/string.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/models/package/package.py` & `dplib_py-0.7.4/dplib/models/package/package.py`

 * *Files 3% similar despite different names*

```diff
@@ -139,7 +139,14 @@
 
     def dereference(self):
         """Dereference the package
         It will dereference all the resource's dialects and schemas in the package.
         """
         for resource in self.resources:
             resource.dereference()
+
+    # Converters
+
+    def to_dict(self):
+        data = {"$schema": settings.PROFILE_CURRENT_PACKAGE}
+        data.update(super().to_dict())
+        return data
```

### Comparing `dplib_py-0.7.3/dplib/models/package/__spec__/test_package.py` & `dplib_py-0.7.4/dplib/models/package/__spec__/test_package.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 from pydantic import ValidationError
 
+from dplib import settings
 from dplib.models import Dialect, Package, Resource, Schema
 
 
 def test_package_from_path():
     package = Package.from_path("data/package.json")
     assert package.name == "name"
     assert len(package.resources) == 1
@@ -104,7 +105,24 @@
     assert len(resource.schema.fields) == 2
 
 
 def test_package_contributors_role_v1():
     package = Package.from_dict({"contributors": [{"role": "author"}]})
     assert package.contributors[0].custom == {}
     assert package.contributors[0].roles == ["author"]
+
+
+def test_package_to_dict():
+    package = Package()
+    assert package.to_dict() == {
+        "$schema": settings.PROFILE_CURRENT_PACKAGE,
+    }
+    package.add_resource(Resource(name="name"))
+    assert package.to_dict() == {
+        "$schema": settings.PROFILE_CURRENT_PACKAGE,
+        "resources": [{"name": "name"}],
+    }
+    package.profile = settings.PROFILE_DEFAULT_PACKAGE
+    assert package.to_dict() == {
+        "$schema": settings.PROFILE_DEFAULT_PACKAGE,
+        "resources": [{"name": "name"}],
+    }
```

### Comparing `dplib_py-0.7.3/dplib/models/resource/hash.py` & `dplib_py-0.7.4/dplib/models/resource/hash.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/models/resource/resource.py` & `dplib_py-0.7.4/dplib/models/resource/resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -175,14 +175,21 @@
         It will dereference all the resource's dialects and schemas
         """
         if isinstance(self.dialect, str):
             self.dialect = Dialect.from_path(self.dialect, basepath=self.basepath)
         if isinstance(self.schema, str):
             self.schema = Schema.from_path(self.schema, basepath=self.basepath)  # type: ignore
 
+    # Converters
+
+    def to_dict(self):
+        data = {"$schema": settings.PROFILE_CURRENT_RESOURCE}
+        data.update(super().to_dict())
+        return data
+
     # Compat
 
     @pydantic.model_validator(mode="before")
     @classmethod
     def compat(cls, data: types.IDict):
         if not isinstance(data, dict):  # type: ignore
             return data
```

### Comparing `dplib_py-0.7.3/dplib/models/resource/__spec__/test_resource.py` & `dplib_py-0.7.4/dplib/models/resource/__spec__/test_resource.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from pathlib import Path
 
 import pytest
 from pydantic import ValidationError
 
+from dplib import settings
 from dplib.models import Dialect, Resource, Schema
 
 
 def test_resource_from_path():
     resource = Resource.from_path("data/resource.json")
     assert resource.name == "name"
     assert resource.path == "table.csv"
@@ -116,7 +117,24 @@
     assert len(resource.schema.fields) == 2
 
 
 def test_resource_contributors_role_v1():
     resource = Resource.from_dict({"contributors": [{"role": "author"}]})
     assert resource.contributors[0].custom == {}
     assert resource.contributors[0].roles == ["author"]
+
+
+def test_resource_to_dict():
+    resource = Resource()
+    assert resource.to_dict() == {
+        "$schema": settings.PROFILE_CURRENT_RESOURCE,
+    }
+    resource.name = "name"
+    assert resource.to_dict() == {
+        "$schema": settings.PROFILE_CURRENT_RESOURCE,
+        "name": "name",
+    }
+    resource.profile = settings.PROFILE_DEFAULT_RESOURCE
+    assert resource.to_dict() == {
+        "$schema": settings.PROFILE_DEFAULT_RESOURCE,
+        "name": "name",
+    }
```

### Comparing `dplib_py-0.7.3/dplib/models/schema/foreignKey.py` & `dplib_py-0.7.4/dplib/models/schema/foreignKey.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/models/schema/schema.py` & `dplib_py-0.7.4/dplib/models/schema/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,14 +109,21 @@
         """Add a field to the schema
 
         Parameters:
             field: The field to add
         """
         self.fields.append(field)
 
+    # Converters
+
+    def to_dict(self):
+        data = {"$schema": settings.PROFILE_CURRENT_SCHEMA}
+        data.update(super().to_dict())
+        return data
+
     # Compat
 
     @pydantic.model_validator(mode="before")
     @classmethod
     def compat(cls, data: types.IDict):
         if not isinstance(data, dict):  # type: ignore
             return data
```

### Comparing `dplib_py-0.7.3/dplib/models/schema/__spec__/test_schema.py` & `dplib_py-0.7.4/dplib/models/schema/__spec__/test_schema.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 from pydantic import ValidationError
 
+from dplib import settings
 from dplib.models import IntegerField, Schema
 
 
 def test_schema_from_path():
     schema = Schema.from_path("data/schema.json")
     assert len(schema.fields) == 2
     assert schema.fields[0].name == "id"
@@ -65,25 +66,49 @@
     schema = Schema.from_path("data/schema.json")
     field = schema.get_field(name="id")
     assert field
     assert field.name == "id"
     assert field.type == "integer"
 
 
-def test_schema_to_dict():
-    schema = Schema()
-    assert schema.to_dict() == {}
-    schema.missingValues.append("x")
-    assert schema.to_dict() == {"missingValues": ["", "x"]}
-
-
 def test_schema_primary_key_v1():
     schema = Schema.from_dict({"primaryKey": "name"})
     assert schema.primaryKey == ["name"]
 
 
 def test_schema_foreign_keys_v1():
     schema = Schema.from_dict(
         {"foreignKeys": [{"fields": "name", "reference": {"fields": "name"}}]}
     )
     assert schema.foreignKeys[0].fields == ["name"]
     assert schema.foreignKeys[0].reference.fields == ["name"]
+
+
+def test_schema_to_dict():
+    schema = Schema()
+    assert schema.to_dict() == {
+        "$schema": settings.PROFILE_CURRENT_SCHEMA,
+    }
+    schema.missingValues.append("x")
+    assert schema.to_dict() == {
+        "$schema": settings.PROFILE_CURRENT_SCHEMA,
+        "missingValues": ["", "x"],
+    }
+    schema.profile = settings.PROFILE_DEFAULT_SCHEMA
+    assert schema.to_dict() == {
+        "$schema": settings.PROFILE_DEFAULT_SCHEMA,
+        "missingValues": ["", "x"],
+    }
+
+
+def test_schema_to_dict_with_fields():
+    schema = Schema()
+    schema.add_field(IntegerField(name="name"))
+    assert schema.to_dict() == {
+        "$schema": settings.PROFILE_CURRENT_SCHEMA,
+        "fields": [
+            {
+                "name": "name",
+                "type": "integer",
+            }
+        ],
+    }
```

### Comparing `dplib_py-0.7.3/dplib/plugins/ckan/models/package.py` & `dplib_py-0.7.4/dplib/plugins/ckan/models/package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/ckan/models/resource.py` & `dplib_py-0.7.4/dplib/plugins/ckan/models/resource.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/ckan/models/__spec__/test_package.py` & `dplib_py-0.7.4/dplib/plugins/ckan/models/__spec__/test_package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/cli/program.py` & `dplib_py-0.7.4/dplib/plugins/cli/program.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/cli/commands/main.py` & `dplib_py-0.7.4/dplib/plugins/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/cli/commands/package/convert.py` & `dplib_py-0.7.4/dplib/plugins/cli/commands/package/convert.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/cli/commands/resource/convert.py` & `dplib_py-0.7.4/dplib/plugins/cli/commands/resource/convert.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/cli/helpers/check.py` & `dplib_py-0.7.4/dplib/plugins/cli/helpers/check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/datacite/models/contributor.py` & `dplib_py-0.7.4/dplib/plugins/datacite/models/contributor.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/datacite/models/package.py` & `dplib_py-0.7.4/dplib/plugins/datacite/models/package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/datacite/models/__spec__/test_package.py` & `dplib_py-0.7.4/dplib/plugins/datacite/models/__spec__/test_package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/dcat/models/helpers.py` & `dplib_py-0.7.4/dplib/plugins/dcat/models/helpers.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/dcat/models/loaders.py` & `dplib_py-0.7.4/dplib/plugins/dcat/models/loaders.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/dcat/models/namespaces.py` & `dplib_py-0.7.4/dplib/plugins/dcat/models/namespaces.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/dcat/models/package.py` & `dplib_py-0.7.4/dplib/plugins/dcat/models/package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/dcat/models/resource.py` & `dplib_py-0.7.4/dplib/plugins/dcat/models/resource.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/dcat/models/__spec__/test_package.py` & `dplib_py-0.7.4/dplib/plugins/dcat/models/__spec__/test_package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/github/models/package.py` & `dplib_py-0.7.4/dplib/plugins/github/models/package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/github/models/resource.py` & `dplib_py-0.7.4/dplib/plugins/github/models/resource.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/github/models/__spec__/test_package.py` & `dplib_py-0.7.4/dplib/plugins/github/models/__spec__/test_package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/pandas/models/field.py` & `dplib_py-0.7.4/dplib/plugins/pandas/models/field.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/pandas/models/schema.py` & `dplib_py-0.7.4/dplib/plugins/pandas/models/schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/polars/models/field.py` & `dplib_py-0.7.4/dplib/plugins/polars/models/field.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/polars/models/schema.py` & `dplib_py-0.7.4/dplib/plugins/polars/models/schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/polars/models/__spec__/test_schema.py` & `dplib_py-0.7.4/dplib/plugins/polars/models/__spec__/test_schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/sql/models/field.py` & `dplib_py-0.7.4/dplib/plugins/sql/models/field.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/sql/models/schema.py` & `dplib_py-0.7.4/dplib/plugins/sql/models/schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/sql/models/__spec__/test_schema.py` & `dplib_py-0.7.4/dplib/plugins/sql/models/__spec__/test_schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/plugins/zenodo/models/resource.py` & `dplib_py-0.7.4/dplib/plugins/zenodo/models/resource.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import os
 from typing import Optional
 
 from dplib.helpers.resource import slugify_name
 from dplib.models import Resource
 from dplib.system import Model
 
 
@@ -15,21 +16,24 @@
     checksum: Optional[str] = None
     ext: Optional[str] = None
     mimetype: Optional[str] = None
     size: Optional[int] = None
 
     # Converters
 
-    def to_dp(self) -> Resource:
+    def to_dp(self, *, package_id: str) -> Resource:
         """Convert to Data Package resource
 
         Returns:
            Data Resource
         """
-        resource = Resource(path=self.key, name=slugify_name(self.key))
+        resource = Resource(
+            path=f"https://zenodo.org/records/{package_id}/files/{self.key}",
+            name=slugify_name(self.key),
+        )
 
         # Format
         if self.ext:
             resource.format = self.ext.lower()
 
         # Mediatype
         if self.mimetype:
@@ -39,14 +43,18 @@
         if self.size:
             resource.bytes = self.size
 
         # Hash
         if self.checksum:
             resource.hash = self.checksum.replace("md5:", "")
 
+        # Custom
+        if self.id:
+            resource.custom["zenodo:id"] = self.id
+
         return resource
 
     @classmethod
     def from_dp(cls, resource: Resource) -> Optional[ZenodoResource]:
         """Create Zenodo Resource from Data Resource
 
         Parameters:
@@ -55,15 +63,15 @@
         Returns:
             Zenodo Resource
         """
         if not resource.path or not isinstance(resource.path, str):
             return
 
         # Path
-        zenodo = ZenodoResource(key=resource.path)
+        zenodo = ZenodoResource(key=os.path.basename(resource.path))
 
         # Format
         if resource.format:
             zenodo.ext = resource.format
 
         # Mediatype
         if resource.mediatype:
```

### Comparing `dplib_py-0.7.3/dplib/plugins/zenodo/models/__spec__/test_package.py` & `dplib_py-0.7.4/dplib/plugins/zenodo/models/__spec__/test_package.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,22 +23,22 @@
 
 def test_zenodo_package_to_dp():
     package = ZenodoPackage.from_path("data/plugins/zenodo/package.json").to_dp()
     assert package.id == "https://doi.org/10.5281/zenodo.5770714"
     assert package.title == "Fishway_Obstruction_Data_v1.csv"
     assert package.description
     assert package.description.startswith("<p>This dataset contains pool-weir")
-    assert package.homepage == "https://zenodo.org/api/records/5770714"
+    assert package.homepage == "https://zenodo.org/records/5770714"
     assert package.version == "v1"
     assert package.created == "2021-12-10T05:47:07.709885+00:00"
     assert len(package.contributors) == 1
     assert package.contributors[0].title == "Fuentes-Pérez, Juan Francisco"
     assert package.contributors[0].givenName == "Juan Francisco"
     assert package.contributors[0].familyName == "Fuentes-Pérez"
-    assert package.contributors[0].roles == ["personal"]
+    assert package.contributors[0].roles == ["creator"]
     assert (
         package.contributors[0].organization
         == "Department of Hydraulics and Hydrology, ETSIIAA, University of Valladolid, 34004 Palencia, Spain"
     )
     assert package.keywords == [
         "fishways",
         "hydraulics",
@@ -47,21 +47,26 @@
         "hydrological variability",
         "nonuniformity",
         "clogging",
         "water-level sensors",
     ]
     assert len(package.resources) == 2
     assert package.resources[0].name == "fishway_obstruction_data_v1"
-    assert package.resources[0].path == "Fishway_Obstruction_Data_v1.csv"
+    assert (
+        package.resources[0].path
+        == "https://zenodo.org/records/5770714/files/Fishway_Obstruction_Data_v1.csv"
+    )
     assert package.resources[0].format == "csv"
     assert package.resources[0].mediatype == "text/csv"
     assert package.resources[0].bytes == 1377
     assert package.resources[0].hash == "7bdef6756c84c3aea749f8211c557684"
     assert package.resources[1].name == "readme"
-    assert package.resources[1].path == "readme.md"
+    assert (
+        package.resources[1].path == "https://zenodo.org/records/5770714/files/readme.md"
+    )
     assert package.resources[1].format == "md"
     assert package.resources[1].mediatype == "application/octet-stream"
     assert package.resources[1].bytes == 1577
     assert package.resources[1].hash == "a23a3c99befca45e706c9343e39f5926"
 
 
 def test_zenodo_package_from_dp():
```

### Comparing `dplib_py-0.7.3/dplib/profiles/1.0/datapackage.json` & `dplib_py-0.7.4/dplib/profiles/1.0/datapackage.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/profiles/1.0/dataresource.json` & `dplib_py-0.7.4/dplib/profiles/1.0/dataresource.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/profiles/1.0/tabledialect.json` & `dplib_py-0.7.4/dplib/profiles/1.0/tabledialect.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/profiles/1.0/tableschema.json` & `dplib_py-0.7.4/dplib/profiles/1.0/tableschema.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/profiles/2.0/datapackage.json` & `dplib_py-0.7.4/dplib/profiles/2.0/datapackage.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/profiles/2.0/dataresource.json` & `dplib_py-0.7.4/dplib/profiles/2.0/dataresource.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/profiles/2.0/tabledialect.json` & `dplib_py-0.7.4/dplib/profiles/2.0/tabledialect.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/profiles/2.0/tableschema.json` & `dplib_py-0.7.4/dplib/profiles/2.0/tableschema.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/dplib/system/model.py` & `dplib_py-0.7.4/dplib/system/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,17 @@
 
     @classmethod
     def from_text(cls, text: str, *, format: str, basepath: Optional[str] = None) -> Self:
         data = load_data(text, format=format)
         return cls.from_dict(data, basepath=basepath)
 
     def to_dict(self):
-        data = self.model_dump(mode="json", exclude_none=True, exclude_defaults=True)
+        data = self.model_dump(
+            mode="json", by_alias=True, exclude_none=True, exclude_defaults=True
+        )
         clean_data(data)
         return data
 
     @classmethod
     def from_dict(cls, data: types.IDict, *, basepath: Optional[str] = None) -> Self:
         if basepath and cls.model_fields.get("basepath"):
             data["basepath"] = basepath
```

### Comparing `dplib_py-0.7.3/dplib/system/__spec__/test_model.py` & `dplib_py-0.7.4/dplib/system/__spec__/test_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,48 @@
 import json
 from pathlib import Path
 
 import pytest
+import yaml
 
+from dplib import settings
 from dplib.error import Error
 from dplib.models import Resource
 
 
 def test_model_repr():
     resource = Resource.from_path("data/resource.json")
-    assert str(resource) == "{'name': 'name', 'path': 'table.csv'}"
+    repr = str(resource)
+    assert repr.count(f"'$schema': '{settings.PROFILE_CURRENT_RESOURCE}'")
+    assert repr.count("'name': 'name'")
+    assert repr.count("'path': 'table.csv'")
 
 
 def test_model_custom_properties():
     data = {"name": "name", "extra": "value"}
     resource = Resource.from_dict(data)
     assert resource.name == "name"
     assert resource.custom["extra"] == "value"
-    assert resource.to_dict() == data
+    assert resource.to_dict() == {
+        "$schema": settings.PROFILE_CURRENT_RESOURCE,
+        "name": "name",
+        "extra": "value",
+    }
 
 
 def test_model_to_path(tmp_path: Path):
     path = str(tmp_path / "resource.json")
     resource = Resource.from_path("data/resource.json")
     resource.to_path(path)
     with open(path) as file:
-        assert json.loads(file.read()) == {"name": "name", "path": "table.csv"}
+        assert json.loads(file.read()) == {
+            "$schema": settings.PROFILE_CURRENT_RESOURCE,
+            "name": "name",
+            "path": "table.csv",
+        }
 
 
 def test_model_from_path_emtpy_file():
     with pytest.raises(Error) as excinfo:
         Resource.from_path("data/empty.json")
     error = excinfo.value
     assert str(error) == "The file is empty: data/empty.json"
@@ -56,8 +69,12 @@
 
 
 def test_model_to_path_yaml(tmp_path: Path):
     path = str(tmp_path / "resource.yaml")
     resource = Resource.from_path("data/resource.json")
     resource.to_path(path)
     with open(path) as file:
-        assert file.read() == "name: name\npath: table.csv\n"
+        assert yaml.safe_load(file.read()) == {
+            "$schema": settings.PROFILE_CURRENT_RESOURCE,
+            "name": "name",
+            "path": "table.csv",
+        }
```

### Comparing `dplib_py-0.7.3/.gitignore` & `dplib_py-0.7.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/LICENSE.md` & `dplib_py-0.7.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/README.md` & `dplib_py-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/pyproject.toml` & `dplib_py-0.7.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.3/PKG-INFO` & `dplib_py-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dplib-py
-Version: 0.7.3
+Version: 0.7.4
 Summary: Python implementation of the Data Package standard
 Project-URL: homepage, https://github.com/frictionlessdata/dplib-py
 Author-email: Open Knowledge Foundation <info@okfn.org>
 License-Expression: MIT
 License-File: LICENSE.md
 Keywords: data package,data validation,json schema,json table schema,open data,tabular data package
 Classifier: Development Status :: 4 - Beta
```

