# Comparing `tmp/snowflake-connector-python-nightly-2024.4.4.tar.gz` & `tmp/snowflake-connector-python-nightly-2024.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake-connector-python-nightly-2024.4.4.tar", last modified: Thu Apr  4 04:06:31 2024, max compression
+gzip compressed data, was "snowflake-connector-python-nightly-2024.4.9.tar", last modified: Tue Apr  9 04:07:44 2024, max compression
```

## Comparing `snowflake-connector-python-nightly-2024.4.4.tar` & `snowflake-connector-python-nightly-2024.4.9.tar`

### file list

```diff
@@ -1,257 +1,257 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:31.619539 snowflake-connector-python-nightly-2024.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    58242 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-04 04:06:31.619539 snowflake-connector-python-nightly-2024.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-04 04:06:31.619539 snowflake-connector-python-nightly-2024.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:31.567538 snowflake-connector-python-nightly-2024.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:31.563538 snowflake-connector-python-nightly-2024.4.4/src/snowflake/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:31.579539 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/_query_context_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/_sql_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/arrow_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:31.583539 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27978 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/auth/_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/auth/by_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/auth/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/auth/idtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/auth/keypair.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/auth/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)    11394 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/auth/okta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/auth/usrpwdmfa.py
--rw-r--r--   0 runner    (1001) docker     (127)    17958 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/auth/webbrowser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/azure_storage_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/backoff_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/bind_upload_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    23454 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    19252 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    75785 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    32728 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/connection_diagnostic.py
--rw-r--r--   0 runner    (1001) docker     (127)    12971 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    27710 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/converter_issue23517.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/converter_null.py
--rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/converter_snowsql.py
--rw-r--r--   0 runner    (1001) docker     (127)    64707 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/dbapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/encryption_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/errorcode.py
--rw-r--r--   0 runner    (1001) docker     (127)    20185 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/file_compression_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    48252 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/file_transfer_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/gcs_storage_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/gzip_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/local_storage_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:31.567538 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:31.595539 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BooleanConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BooleanConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    19180 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    42047 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IColumnConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11583 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:31.595539 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13329 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:31.595539 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/macros.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:31.599539 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_accessors.h
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_alloc.h
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_assert.h
--rw-r--r--   0 runner    (1001) docker     (127)    79675 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_builder.h
--rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_emitter.h
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_endian.h
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_epilogue.h
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_flatbuffers.h
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_identifier.h
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_iov.h
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_prologue.h
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_refmap.h
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_rtconfig.h
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_types.h
--rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_verifier.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:31.599539 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/flatcc_portable.h
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/paligned_alloc.h
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pattributes.h
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic.h
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_pop.h
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_push.h
--rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian.h
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian_detect.h
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinline.h
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinttypes.h
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable.h
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable_basic.h
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstatic_assert.h
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdalign.h
--rw-r--r--   0 runner    (1001) docker     (127)    31201 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdint.h
--rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/punaligned.h
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pversion.h
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pwarnings.h
--rw-r--r--   0 runner    (1001) docker     (127)   102952 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc.c
--rw-r--r--   0 runner    (1001) docker     (127)   107680 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.c
--rw-r--r--   0 runner    (1001) docker     (127)   132283 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.h
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_arrow_iterator.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    18580 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.c
--rw-r--r--   0 runner    (1001) docker     (127)    14382 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.h
--rw-r--r--   0 runner    (1001) docker     (127)  1616169 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.c
--rw-r--r--   0 runner    (1001) docker     (127)    17533 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:31.599539 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/Logging/
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/Logging/logging.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/Logging/logging.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    42377 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    16575 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/ocsp_asn1crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)    69704 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/ocsp_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    22553 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/pandas_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    26617 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/result_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9380 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/result_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    21870 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/s3_storage_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/secret_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/sf_dirs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/sfbinaryformat.py
--rw-r--r--   0 runner    (1001) docker     (127)    12449 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/sfdatetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/snow_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/sqlstate.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/ssd_internal_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/ssl_wrap_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)    17583 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/storage_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    19070 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/telemetry_oob.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/time_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:31.603539 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/tool/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/tool/dump_certs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/tool/dump_ocsp_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/tool/dump_ocsp_response_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/tool/probe_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/url_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10405 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/util_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:31.603539 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:31.607539 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/
--rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/_internal_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19577 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/certs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/help.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    35231 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    30373 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/status_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/structures.py
--rw-r--r--   0 runner    (1001) docker     (127)    33450 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:31.607539 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11372 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    20300 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    40285 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/connectionpool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:31.611539 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:31.611539 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17632 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/contrib/appengine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 runner    (1001) docker     (127)    16772 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 runner    (1001) docker     (127)    34431 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/contrib/socks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8579 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/filepost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:31.611539 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/packages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:31.611539 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/packages/backports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/packages/backports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/packages/backports/weakref_finalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    34665 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/packages/six.py
--rw-r--r--   0 runner    (1001) docker     (127)    19990 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/poolmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    30760 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:31.615539 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/response.py
--rw-r--r--   0 runner    (1001) docker     (127)    22013 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    17165 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/ssl_.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/ssltransport.py
--rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)    14279 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/wait.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-04 04:06:26.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:06:31.615539 snowflake-connector-python-nightly-2024.4.4/src/snowflake_connector_python_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-04 04:06:31.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake_connector_python_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13274 2024-04-04 04:06:31.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:06:31.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake_connector_python_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-04 04:06:31.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake_connector_python_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:06:31.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake_connector_python_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-04 04:06:31.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake_connector_python_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 04:06:31.000000 snowflake-connector-python-nightly-2024.4.4/src/snowflake_connector_python_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.354408 snowflake-connector-python-nightly-2024.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    58487 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-09 04:07:44.354408 snowflake-connector-python-nightly-2024.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-09 04:07:44.354408 snowflake-connector-python-nightly-2024.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.306408 snowflake-connector-python-nightly-2024.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.306408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.318408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/_query_context_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/_sql_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/arrow_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.322408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27978 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/by_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/idtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11394 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/okta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/usrpwdmfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17958 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/webbrowser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/azure_storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/backoff_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/bind_upload_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23454 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19252 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75785 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32728 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/connection_diagnostic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12971 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27710 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/converter_issue23517.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/converter_null.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/converter_snowsql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64707 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/dbapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/encryption_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/errorcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20185 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/file_compression_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48252 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/file_transfer_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/gcs_storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/gzip_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/local_storage_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.306408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.330408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BooleanConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BooleanConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19180 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    42047 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IColumnConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11583 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.334408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13329 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.334408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/macros.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.334408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_accessors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_alloc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_assert.h
+-rw-r--r--   0 runner    (1001) docker     (127)    79675 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_builder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_emitter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_endian.h
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_epilogue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_flatbuffers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_identifier.h
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_iov.h
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_prologue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_refmap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_rtconfig.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_types.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_verifier.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.338408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/flatcc_portable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/paligned_alloc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pattributes.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic.h
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_pop.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_push.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian_detect.h
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinline.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinttypes.h
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable.h
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable_basic.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstatic_assert.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdalign.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31201 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/punaligned.h
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pversion.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pwarnings.h
+-rw-r--r--   0 runner    (1001) docker     (127)   102952 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc.c
+-rw-r--r--   0 runner    (1001) docker     (127)   107680 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.c
+-rw-r--r--   0 runner    (1001) docker     (127)   132283 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_arrow_iterator.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    18580 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14382 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.h
+-rw-r--r--   0 runner    (1001) docker     (127)  1616169 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    17533 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.338408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/Logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/Logging/logging.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/Logging/logging.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    42377 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16575 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/ocsp_asn1crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69704 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/ocsp_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22495 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/pandas_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    26617 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/result_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9380 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/result_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21870 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/s3_storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/secret_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/sf_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/sfbinaryformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12449 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/sfdatetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/snow_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/sqlstate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/ssd_internal_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/ssl_wrap_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17583 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19070 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/telemetry_oob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/time_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.338408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/tool/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/tool/dump_certs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/tool/dump_ocsp_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/tool/dump_ocsp_response_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/tool/probe_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/url_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10405 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/util_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.338408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.342408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/_internal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19577 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/certs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35231 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30373 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/status_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33450 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.346408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11372 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20300 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40285 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/connectionpool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.346408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.346408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17632 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/appengine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16772 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34431 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/socks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8579 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/filepost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.346408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.346408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/packages/backports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/packages/backports/weakref_finalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34665 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/packages/six.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19990 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/poolmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30760 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.350408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22013 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17165 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/ssl_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/ssltransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14279 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/wait.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.350408 snowflake-connector-python-nightly-2024.4.9/src/snowflake_connector_python_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-09 04:07:44.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake_connector_python_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13274 2024-04-09 04:07:44.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 04:07:44.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake_connector_python_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-09 04:07:44.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake_connector_python_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 04:07:43.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake_connector_python_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-09 04:07:44.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake_connector_python_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 04:07:44.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake_connector_python_nightly.egg-info/top_level.txt
```

### Comparing `snowflake-connector-python-nightly-2024.4.4/CONTRIBUTING.md` & `snowflake-connector-python-nightly-2024.4.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/DESCRIPTION.md` & `snowflake-connector-python-nightly-2024.4.9/DESCRIPTION.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 Snowflake Documentation is available at:
 https://docs.snowflake.com/
 
 Source code is also available at: https://github.com/snowflakedb/snowflake-connector-python
 
 # Release Notes
 
+- v3.8.1(April 09, 2024)
+
+  - Reverted the change "Updated `write_pandas` to skip TABLE IF NOT EXISTS in truncate mode." introduced in v3.8.0 (yanked) as it's a breaking change. `write_pandas` will be fixed in the future in a non-breaking way.
+
 - v3.8.0(April 04,2024)
 
   - Improved `externalbrowser` auth in containerized environments
     - Instruct browser to not fetch `/favicon` on success page
     - Simple retry strategy on empty socket.recv
     - Add `SNOWFLAKE_AUTH_SOCKET_REUSE_PORT` flag (usage: `SNOWFLAKE_AUTH_SOCKET_REUSE_PORT=true`) to set the underlying socket's `SO_REUSEPORT` flag (described in the [socket man page](https://man7.org/linux/man-pages/man7/socket.7.html))
       - Useful when the randomized port used in the localhost callback url is being followed before the container engine completes port forwarding to host
```

### Comparing `snowflake-connector-python-nightly-2024.4.4/LICENSE.txt` & `snowflake-connector-python-nightly-2024.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/MANIFEST.in` & `snowflake-connector-python-nightly-2024.4.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/PKG-INFO` & `snowflake-connector-python-nightly-2024.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-connector-python-nightly
-Version: 2024.4.4
+Version: 2024.4.9
 Summary: Nigthly build of Snowflake Connector for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/user-guide/python-connector.html
 Project-URL: Source, https://github.com/keller00/snowflake-connector-python-nightlies/
```

### Comparing `snowflake-connector-python-nightly-2024.4.4/README.md` & `snowflake-connector-python-nightly-2024.4.9/README.md`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/pyproject.toml` & `snowflake-connector-python-nightly-2024.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/setup.cfg` & `snowflake-connector-python-nightly-2024.4.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/setup.py` & `snowflake-connector-python-nightly-2024.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,11 +172,11 @@
                 build_ext.build_extension(self, ext)
             finally:
                 self.compiler._compile = original__compile
 
     cmd_class = {"build_ext": MyBuildExt}
 
 setup(
-    version="2024.04.04",
+    version="2024.04.09",
     ext_modules=extensions,
     cmdclass=cmd_class,
 )
```

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/__init__.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/_query_context_cache.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/_query_context_cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/_sql_util.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/_sql_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/arrow_context.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/arrow_context.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/auth/__init__.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/auth/_auth.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/_auth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/auth/by_plugin.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/by_plugin.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/auth/default.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/default.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/auth/idtoken.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/idtoken.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/auth/keypair.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/keypair.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/auth/oauth.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/auth/okta.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/okta.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/auth/usrpwdmfa.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/usrpwdmfa.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/auth/webbrowser.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/webbrowser.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/azure_storage_client.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/azure_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/backoff_policies.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/backoff_policies.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/bind_upload_agent.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/bind_upload_agent.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/cache.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/compat.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/compat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/config_manager.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/config_manager.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/connection.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/connection_diagnostic.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/connection_diagnostic.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/constants.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/constants.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/converter.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/converter.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/converter_issue23517.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/converter_issue23517.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/converter_snowsql.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/converter_snowsql.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/cursor.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/cursor.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/dbapi.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/dbapi.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/description.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/description.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/encryption_util.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/encryption_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/errorcode.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/errorcode.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/errors.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/errors.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/file_compression_type.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/file_compression_type.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/file_transfer_agent.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/file_transfer_agent.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/file_util.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/file_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/gcs_storage_client.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/gcs_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/gzip_decoder.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/gzip_decoder.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/local_storage_client.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/local_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.cpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.hpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.cpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.hpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.cpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.hpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.cpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.hpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.cpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.hpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.cpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.hpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.cpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.hpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.cpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.hpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.cpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.hpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.cpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.hpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/LICENSE.txt` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.cpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.hpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.cpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.hpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.hpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.cpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.hpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.cpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.hpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.cpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.hpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.cpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.hpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.cpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.hpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.cpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.hpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_accessors.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_accessors.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_alloc.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_alloc.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_assert.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_assert.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_builder.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_builder.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_emitter.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_emitter.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_endian.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_endian.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_flatbuffers.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_flatbuffers.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_identifier.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_identifier.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_iov.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_iov.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_refmap.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_refmap.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_rtconfig.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_rtconfig.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_types.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_types.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_verifier.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_verifier.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/paligned_alloc.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/paligned_alloc.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pattributes.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pattributes.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_pop.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_pop.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_push.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_push.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian_detect.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian_detect.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinttypes.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinttypes.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable_basic.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable_basic.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstatic_assert.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstatic_assert.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdalign.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdalign.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdint.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdint.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/punaligned.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/punaligned.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pwarnings.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pwarnings.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc.c` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc.c`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.c` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.c`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.hpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_arrow_iterator.pyx` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_arrow_iterator.pyx`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.c` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.c`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.c` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.c`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.h` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/Logging/logging.cpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/Logging/logging.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/nanoarrow_cpp/Logging/logging.hpp` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/Logging/logging.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/network.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/network.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/ocsp_asn1crypto.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/ocsp_asn1crypto.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/ocsp_snowflake.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/ocsp_snowflake.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/options.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/options.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/pandas_tools.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/pandas_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,22 +389,21 @@
         target_table_location = build_location_helper(
             database,
             schema,
             random_string() if (overwrite and auto_create_table) else table_name,
             quote_identifiers,
         )
 
-        if auto_create_table:
-            create_table_sql = (
-                f"CREATE {table_type.upper()} TABLE IF NOT EXISTS {target_table_location} "
-                f"({create_table_columns})"
-                f" /* Python:snowflake.connector.pandas_tools.write_pandas() */ "
-            )
-            logger.debug(f"auto creating table with '{create_table_sql}'")
-            cursor.execute(create_table_sql, _is_internal=True)
+        create_table_sql = (
+            f"CREATE {table_type.upper()} TABLE IF NOT EXISTS {target_table_location} "
+            f"({create_table_columns})"
+            f" /* Python:snowflake.connector.pandas_tools.write_pandas() */ "
+        )
+        logger.debug(f"auto creating table with '{create_table_sql}'")
+        cursor.execute(create_table_sql, _is_internal=True)
         # need explicit casting when the underlying table schema is inferred
         parquet_columns = "$1:" + ",$1:".join(
             f"{quote}{snowflake_col}{quote}::{column_type_mapping[col]}"
             for snowflake_col, col in zip(snowflake_column_names, df.columns)
         )
     else:
         target_table_location = build_location_helper(
```

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/proxy.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/proxy.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/result_batch.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/result_batch.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/result_set.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/result_set.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/s3_storage_client.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/s3_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/secret_detector.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/secret_detector.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/sf_dirs.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/sf_dirs.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/sfbinaryformat.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/sfbinaryformat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/sfdatetime.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/sfdatetime.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/snow_logging.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/snow_logging.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/ssd_internal_keys.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/ssd_internal_keys.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/ssl_wrap_socket.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/ssl_wrap_socket.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/storage_client.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/telemetry.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/telemetry.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/telemetry_oob.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/telemetry_oob.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/test_util.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/test_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/time_util.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/time_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/tool/dump_certs.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/tool/dump_certs.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/tool/dump_ocsp_response.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/tool/dump_ocsp_response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/tool/dump_ocsp_response_cache.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/tool/dump_ocsp_response_cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/tool/probe_connection.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/tool/probe_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/url_util.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/url_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/util_text.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/util_text.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/LICENSE` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/__init__.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/_internal_utils.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/adapters.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/api.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/api.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/auth.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/auth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/compat.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/compat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/cookies.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/exceptions.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/help.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/help.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/hooks.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/models.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/models.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/sessions.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/status_codes.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/structures.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/structures.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/requests/utils.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/LICENSE.txt` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/__init__.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/_collections.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/connection.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/connectionpool.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/contrib/appengine.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/contrib/socks.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/exceptions.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/fields.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/filepost.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/packages/backports/weakref_finalize.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/packages/backports/weakref_finalize.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/packages/six.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/poolmanager.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/request.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/response.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/__init__.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/connection.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/proxy.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/request.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/response.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/retry.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/ssl_.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/ssltransport.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/timeout.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/url.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake/connector/vendored/urllib3/util/wait.py` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake_connector_python_nightly.egg-info/PKG-INFO` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake_connector_python_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-connector-python-nightly
-Version: 2024.4.4
+Version: 2024.4.9
 Summary: Nigthly build of Snowflake Connector for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/user-guide/python-connector.html
 Project-URL: Source, https://github.com/keller00/snowflake-connector-python-nightlies/
```

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.4/src/snowflake_connector_python_nightly.egg-info/requires.txt` & `snowflake-connector-python-nightly-2024.4.9/src/snowflake_connector_python_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

