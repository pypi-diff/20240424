# Comparing `tmp/dbt_common-1.0.1.tar.gz` & `tmp/dbt_common-1.0.2.tar.gz`

## Comparing `dbt_common-1.0.1.tar` & `dbt_common-1.0.2.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_common-1.0.1/CHANGELOG.md
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_common-1.0.1/codecov.yml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/__init__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/constants.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/context.py
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/dataclass_schema.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/helper_types.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/invocation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/py.typed
--rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/record.py
--rw-r--r--   0        0        0    13954 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/semver.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/tests.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/ui.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/clients/__init__.py
--rw-r--r--   0        0        0    12947 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/clients/_jinja_blocks.py
--rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/clients/agate_helper.py
--rw-r--r--   0        0        0    18502 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/clients/jinja.py
--rw-r--r--   0        0        0    23014 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/clients/system.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/contracts/__init__.py
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/contracts/constraints.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/contracts/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/contracts/config/__init__.py
--rw-r--r--   0        0        0     8356 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/contracts/config/base.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/contracts/config/materialization.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/contracts/config/metadata.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/contracts/config/properties.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/events/README.md
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/events/__init__.py
--rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/events/base_types.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/events/contextvars.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/events/event_handler.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/events/event_manager.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/events/event_manager_client.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/events/format.py
--rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/events/functions.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/events/helpers.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/events/interfaces.py
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/events/logger.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/events/types.proto
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/events/types.py
--rw-r--r--   0        0        0     5569 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/events/types_pb2.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/exceptions/__init__.py
--rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/exceptions/base.py
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/exceptions/cache.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/exceptions/connection.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/exceptions/contracts.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/exceptions/events.py
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/exceptions/jinja.py
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/exceptions/macros.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/exceptions/system.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/utils/__init__.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/utils/casting.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/utils/connection.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/utils/dict.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/utils/encoding.py
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/utils/executor.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/utils/formatting.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 dbt_common-1.0.1/dbt_common/utils/jinja.py
--rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 dbt_common-1.0.1/docs/arch/adr-0001-build-tooling.md
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/agate/__init__.pyi
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/agate/data_types.pyi
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/colorama/__init__.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/isodate/__init__.pyi
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/__init__.pyi
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/config.pyi
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/dialect.pyi
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/exceptions.pyi
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/helper.pyi
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/types.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/core/__init__.pyi
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/core/const.pyi
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/core/helpers.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/core/meta/__init__.pyi
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/core/meta/helpers.pyi
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/core/meta/mixin.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/core/meta/code/__init__.pyi
--rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/core/meta/code/builder.pyi
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/core/meta/code/lines.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/core/meta/types/__init__.pyi
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/core/meta/types/common.pyi
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/core/meta/types/pack.pyi
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/core/meta/types/unpack.pyi
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/jsonschema/__init__.pyi
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/jsonschema/annotations.pyi
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/jsonschema/builder.pyi
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/jsonschema/dialects.pyi
--rw-r--r--   0        0        0     5864 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/jsonschema/models.pyi
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/jsonschema/schema.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/mixins/__init__.pyi
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/mixins/dict.pyi
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/mixins/json.pyi
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/mixins/msgpack.pyi
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/mixins/orjson.pyi
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/mixins/toml.pyi
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 dbt_common-1.0.1/third-party-stubs/mashumaro/mixins/yaml.pyi
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 dbt_common-1.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_common-1.0.1/LICENSE
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 dbt_common-1.0.1/README.md
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 dbt_common-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5219 2020-02-02 00:00:00.000000 dbt_common-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_common-1.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_common-1.0.2/codecov.yml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/__init__.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/constants.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/context.py
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/dataclass_schema.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/helper_types.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/invocation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/py.typed
+-rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/record.py
+-rw-r--r--   0        0        0    13954 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/semver.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/tests.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/ui.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/clients/__init__.py
+-rw-r--r--   0        0        0    12947 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/clients/_jinja_blocks.py
+-rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/clients/agate_helper.py
+-rw-r--r--   0        0        0    18502 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/clients/jinja.py
+-rw-r--r--   0        0        0    23014 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/clients/system.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/contracts/__init__.py
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/contracts/constraints.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/contracts/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/contracts/config/__init__.py
+-rw-r--r--   0        0        0     8356 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/contracts/config/base.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/contracts/config/materialization.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/contracts/config/metadata.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/contracts/config/properties.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/events/README.md
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/events/__init__.py
+-rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/events/base_types.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/events/contextvars.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/events/event_handler.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/events/event_manager.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/events/event_manager_client.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/events/format.py
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/events/functions.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/events/helpers.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/events/interfaces.py
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/events/logger.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/events/types.proto
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/events/types.py
+-rw-r--r--   0        0        0     5569 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/events/types_pb2.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/exceptions/__init__.py
+-rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/exceptions/base.py
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/exceptions/cache.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/exceptions/connection.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/exceptions/contracts.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/exceptions/events.py
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/exceptions/jinja.py
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/exceptions/macros.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/exceptions/system.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/utils/__init__.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/utils/casting.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/utils/connection.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/utils/dict.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/utils/encoding.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/utils/executor.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/utils/formatting.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 dbt_common-1.0.2/dbt_common/utils/jinja.py
+-rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 dbt_common-1.0.2/docs/arch/adr-0001-build-tooling.md
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/agate/__init__.pyi
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/agate/data_types.pyi
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/colorama/__init__.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/isodate/__init__.pyi
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/__init__.pyi
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/config.pyi
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/dialect.pyi
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/exceptions.pyi
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/helper.pyi
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/types.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/core/__init__.pyi
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/core/const.pyi
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/core/helpers.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/core/meta/__init__.pyi
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/core/meta/helpers.pyi
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/core/meta/mixin.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/core/meta/code/__init__.pyi
+-rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/core/meta/code/builder.pyi
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/core/meta/code/lines.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/core/meta/types/__init__.pyi
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/core/meta/types/common.pyi
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/core/meta/types/pack.pyi
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/core/meta/types/unpack.pyi
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/jsonschema/__init__.pyi
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/jsonschema/annotations.pyi
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/jsonschema/builder.pyi
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/jsonschema/dialects.pyi
+-rw-r--r--   0        0        0     5864 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/jsonschema/models.pyi
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/jsonschema/schema.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/mixins/__init__.pyi
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/mixins/dict.pyi
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/mixins/json.pyi
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/mixins/msgpack.pyi
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/mixins/orjson.pyi
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/mixins/toml.pyi
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 dbt_common-1.0.2/third-party-stubs/mashumaro/mixins/yaml.pyi
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 dbt_common-1.0.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_common-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 dbt_common-1.0.2/README.md
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 dbt_common-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5219 2020-02-02 00:00:00.000000 dbt_common-1.0.2/PKG-INFO
```

### Comparing `dbt_common-1.0.1/dbt_common/context.py` & `dbt_common-1.0.2/dbt_common/context.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/dataclass_schema.py` & `dbt_common-1.0.2/dbt_common/dataclass_schema.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/helper_types.py` & `dbt_common-1.0.2/dbt_common/helper_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,33 +50,45 @@
 
         if isinstance(self.include, list):
             self._validate_items(self.include)
 
         if isinstance(self.exclude, list):
             self._validate_items(self.exclude)
 
-    def includes(self, item_name: str):
+    def includes(self, item_name: str) -> bool:
         return (
             item_name in self.include or self.include in self.INCLUDE_ALL
         ) and item_name not in self.exclude
 
     def _validate_items(self, items: List[str]):
         pass
 
 
 class WarnErrorOptions(IncludeExclude):
     def __init__(
         self,
         include: Union[str, List[str]],
         exclude: Optional[List[str]] = None,
         valid_error_names: Optional[Set[str]] = None,
+        silence: Optional[List[str]] = None,
     ):
+        self.silence = silence or []
         self._valid_error_names: Set[str] = valid_error_names or set()
         super().__init__(include=include, exclude=(exclude or []))
 
+    def __post_init__(self):
+        super().__post_init__()
+        self._validate_items(self.silence)
+
+    def includes(self, item_name: str) -> bool:
+        return super().includes(item_name) and not self.silenced(item_name)
+
+    def silenced(self, item_name: str) -> bool:
+        return item_name in self.silence
+
     def _validate_items(self, items: List[str]):
         for item in items:
             if item not in self._valid_error_names:
                 raise ValidationError(f"{item} is not a valid dbt error name.")
 
 
 FQNPath = Tuple[str, ...]
```

### Comparing `dbt_common-1.0.1/dbt_common/record.py` & `dbt_common-1.0.2/dbt_common/record.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/semver.py` & `dbt_common-1.0.2/dbt_common/semver.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/ui.py` & `dbt_common-1.0.2/dbt_common/ui.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/clients/_jinja_blocks.py` & `dbt_common-1.0.2/dbt_common/clients/_jinja_blocks.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/clients/agate_helper.py` & `dbt_common-1.0.2/dbt_common/clients/agate_helper.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/clients/jinja.py` & `dbt_common-1.0.2/dbt_common/clients/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/clients/system.py` & `dbt_common-1.0.2/dbt_common/clients/system.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/contracts/constraints.py` & `dbt_common-1.0.2/dbt_common/contracts/constraints.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/contracts/util.py` & `dbt_common-1.0.2/dbt_common/contracts/util.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/contracts/config/base.py` & `dbt_common-1.0.2/dbt_common/contracts/config/base.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/contracts/config/metadata.py` & `dbt_common-1.0.2/dbt_common/contracts/config/metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/contracts/config/properties.py` & `dbt_common-1.0.2/dbt_common/contracts/config/properties.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/events/README.md` & `dbt_common-1.0.2/dbt_common/events/README.md`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/events/base_types.py` & `dbt_common-1.0.2/dbt_common/events/base_types.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/events/contextvars.py` & `dbt_common-1.0.2/dbt_common/events/contextvars.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/events/event_handler.py` & `dbt_common-1.0.2/dbt_common/events/event_handler.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/events/event_manager.py` & `dbt_common-1.0.2/dbt_common/events/event_manager.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/events/event_manager_client.py` & `dbt_common-1.0.2/dbt_common/events/event_manager_client.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/events/format.py` & `dbt_common-1.0.2/dbt_common/events/format.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/events/functions.py` & `dbt_common-1.0.2/dbt_common/events/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pathlib import Path
 
 from dbt_common.events.event_manager_client import get_event_manager
+from dbt_common.exceptions import EventCompilationError
 from dbt_common.invocation import get_invocation_id
 from dbt_common.helper_types import WarnErrorOptions
 from dbt_common.utils.encoding import ForgivingJSONEncoder
 from dbt_common.events.base_types import BaseEvent, EventLevel, EventMsg
 from dbt_common.events.logger import LoggerConfig, LineFormat
 from dbt_common.exceptions import scrub_secrets, env_secrets
 from dbt_common.events.types import Note
@@ -110,20 +111,18 @@
         and msg_dict["data"]["node_info"]["node_name"] == ""
     ):
         del msg_dict["data"]["node_info"]
     return msg_dict
 
 
 def warn_or_error(event, node=None) -> None:
-    if WARN_ERROR or WARN_ERROR_OPTIONS.includes(type(event).__name__):
-        # TODO: resolve this circular import when at top
-        from dbt_common.exceptions import EventCompilationError
-
+    event_name = type(event).__name__
+    if WARN_ERROR or WARN_ERROR_OPTIONS.includes(event_name):
         raise EventCompilationError(event.message(), node)
-    else:
+    elif not WARN_ERROR_OPTIONS.silenced(event_name):
         fire_event(event)
 
 
 # an alternative to fire_event which only creates and logs the event value
 # if the condition is met. Does nothing otherwise.
 def fire_event_if(
     conditional: bool, lazy_e: Callable[[], BaseEvent], level: Optional[EventLevel] = None
```

### Comparing `dbt_common-1.0.1/dbt_common/events/logger.py` & `dbt_common-1.0.2/dbt_common/events/logger.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/events/types.proto` & `dbt_common-1.0.2/dbt_common/events/types.proto`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/events/types.py` & `dbt_common-1.0.2/dbt_common/events/types.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/events/types_pb2.py` & `dbt_common-1.0.2/dbt_common/events/types_pb2.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/exceptions/base.py` & `dbt_common-1.0.2/dbt_common/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/exceptions/cache.py` & `dbt_common-1.0.2/dbt_common/exceptions/cache.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/exceptions/contracts.py` & `dbt_common-1.0.2/dbt_common/exceptions/contracts.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/exceptions/jinja.py` & `dbt_common-1.0.2/dbt_common/exceptions/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/exceptions/macros.py` & `dbt_common-1.0.2/dbt_common/exceptions/macros.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/exceptions/system.py` & `dbt_common-1.0.2/dbt_common/exceptions/system.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/utils/__init__.py` & `dbt_common-1.0.2/dbt_common/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/utils/casting.py` & `dbt_common-1.0.2/dbt_common/utils/casting.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/utils/connection.py` & `dbt_common-1.0.2/dbt_common/utils/connection.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/utils/dict.py` & `dbt_common-1.0.2/dbt_common/utils/dict.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/utils/encoding.py` & `dbt_common-1.0.2/dbt_common/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/utils/executor.py` & `dbt_common-1.0.2/dbt_common/utils/executor.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/dbt_common/utils/jinja.py` & `dbt_common-1.0.2/dbt_common/utils/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/docs/arch/adr-0001-build-tooling.md` & `dbt_common-1.0.2/docs/arch/adr-0001-build-tooling.md`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/third-party-stubs/agate/__init__.pyi` & `dbt_common-1.0.2/third-party-stubs/agate/__init__.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/third-party-stubs/agate/data_types.pyi` & `dbt_common-1.0.2/third-party-stubs/agate/data_types.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/third-party-stubs/mashumaro/config.pyi` & `dbt_common-1.0.2/third-party-stubs/mashumaro/config.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/third-party-stubs/mashumaro/exceptions.pyi` & `dbt_common-1.0.2/third-party-stubs/mashumaro/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/third-party-stubs/mashumaro/helper.pyi` & `dbt_common-1.0.2/third-party-stubs/mashumaro/helper.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/third-party-stubs/mashumaro/types.pyi` & `dbt_common-1.0.2/third-party-stubs/mashumaro/types.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/third-party-stubs/mashumaro/core/meta/helpers.pyi` & `dbt_common-1.0.2/third-party-stubs/mashumaro/core/meta/helpers.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/third-party-stubs/mashumaro/core/meta/code/builder.pyi` & `dbt_common-1.0.2/third-party-stubs/mashumaro/core/meta/code/builder.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/third-party-stubs/mashumaro/core/meta/types/common.pyi` & `dbt_common-1.0.2/third-party-stubs/mashumaro/core/meta/types/common.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/third-party-stubs/mashumaro/core/meta/types/unpack.pyi` & `dbt_common-1.0.2/third-party-stubs/mashumaro/core/meta/types/unpack.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/third-party-stubs/mashumaro/jsonschema/annotations.pyi` & `dbt_common-1.0.2/third-party-stubs/mashumaro/jsonschema/annotations.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/third-party-stubs/mashumaro/jsonschema/builder.pyi` & `dbt_common-1.0.2/third-party-stubs/mashumaro/jsonschema/builder.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/third-party-stubs/mashumaro/jsonschema/dialects.pyi` & `dbt_common-1.0.2/third-party-stubs/mashumaro/jsonschema/dialects.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/third-party-stubs/mashumaro/jsonschema/models.pyi` & `dbt_common-1.0.2/third-party-stubs/mashumaro/jsonschema/models.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/third-party-stubs/mashumaro/jsonschema/schema.pyi` & `dbt_common-1.0.2/third-party-stubs/mashumaro/jsonschema/schema.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/third-party-stubs/mashumaro/mixins/dict.pyi` & `dbt_common-1.0.2/third-party-stubs/mashumaro/mixins/dict.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/third-party-stubs/mashumaro/mixins/json.pyi` & `dbt_common-1.0.2/third-party-stubs/mashumaro/mixins/json.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/third-party-stubs/mashumaro/mixins/msgpack.pyi` & `dbt_common-1.0.2/third-party-stubs/mashumaro/mixins/msgpack.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/third-party-stubs/mashumaro/mixins/orjson.pyi` & `dbt_common-1.0.2/third-party-stubs/mashumaro/mixins/orjson.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/third-party-stubs/mashumaro/mixins/toml.pyi` & `dbt_common-1.0.2/third-party-stubs/mashumaro/mixins/toml.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/third-party-stubs/mashumaro/mixins/yaml.pyi` & `dbt_common-1.0.2/third-party-stubs/mashumaro/mixins/yaml.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/.gitignore` & `dbt_common-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/LICENSE` & `dbt_common-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/README.md` & `dbt_common-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/pyproject.toml` & `dbt_common-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.1/PKG-INFO` & `dbt_common-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dbt-common
-Version: 1.0.1
+Version: 1.0.2
 Summary: The shared common utilities that dbt-core and adapter implementations use
 Project-URL: Homepage, https://github.com/dbt-labs/dbt-common
 Project-URL: Repository, https://github.com/dbt-labs/dbt-common.git
 Project-URL: Issues, https://github.com/dbt-labs/dbt-common/issues
 Project-URL: Changelog, https://github.com/dbt-labs/dbt-common/blob/main/CHANGELOG.md
 Author-email: dbt Labs <info@dbtlabs.com>
 Maintainer-email: dbt Labs <info@dbtlabs.com>
```

