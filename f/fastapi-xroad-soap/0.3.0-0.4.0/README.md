# Comparing `tmp/fastapi_xroad_soap-0.3.0.tar.gz` & `tmp/fastapi_xroad_soap-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_xroad_soap-0.3.0.tar", max compression
+gzip compressed data, was "fastapi_xroad_soap-0.4.0.tar", max compression
```

## Comparing `fastapi_xroad_soap-0.3.0.tar` & `fastapi_xroad_soap-0.4.0.tar`

### file list

```diff
@@ -1,62 +1,64 @@
--rw-r--r--   0        0        0    13831 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/LICENSE
--rw-r--r--   0        0        0     2939 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/README.md
--rw-r--r--   0        0        0      524 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/__init__.py
--rw-r--r--   0        0        0      574 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/elements.py
--rw-r--r--   0        0        0      471 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/faults.py
--rw-r--r--   0        0        0      340 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/__init__.py
--rw-r--r--   0        0        0      610 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/base/__init__.py
--rw-r--r--   0        0        0     4737 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/base/body.py
--rw-r--r--   0        0        0     1181 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/base/meta.py
--rw-r--r--   0        0        0     4348 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/base/spec.py
--rw-r--r--   0        0        0     1062 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/constants.py
--rw-r--r--   0        0        0      486 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/__init__.py
--rw-r--r--   0        0        0     1061 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/__init__.py
--rw-r--r--   0        0        0     1257 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/boolean.py
--rw-r--r--   0        0        0     1195 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/date.py
--rw-r--r--   0        0        0     1243 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/datetime.py
--rw-r--r--   0        0        0     1180 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/float.py
--rw-r--r--   0        0        0     1223 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/integer.py
--rw-r--r--   0        0        0     1247 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/netres.py
--rw-r--r--   0        0        0     1284 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/string.py
--rw-r--r--   0        0        0     7247 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/swaref.py
--rw-r--r--   0        0        0     1195 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/time.py
--rw-r--r--   0        0        0     2007 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/numeric_type_spec.py
--rw-r--r--   0        0        0     2158 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/string_type_spec.py
--rw-r--r--   0        0        0     3157 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/validators.py
--rw-r--r--   0        0        0      679 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/envelope/__init__.py
--rw-r--r--   0        0        0     2783 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/envelope/factory.py
--rw-r--r--   0        0        0     1401 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/envelope/generics.py
--rw-r--r--   0        0        0     1912 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/envelope/header.py
--rw-r--r--   0        0        0     1910 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/file_size.py
--rw-r--r--   0        0        0      732 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/multipart/__init__.py
--rw-r--r--   0        0        0     2801 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/multipart/bodypart.py
--rw-r--r--   0        0        0     2124 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/multipart/decoder.py
--rw-r--r--   0        0        0     2493 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/multipart/encoder.py
--rw-r--r--   0        0        0     1024 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/multipart/errors.py
--rw-r--r--   0        0        0      901 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/__init__.py
--rw-r--r--   0        0        0     5286 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/action.py
--rw-r--r--   0        0        0     4155 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/faults.py
--rw-r--r--   0        0        0     1613 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/response.py
--rw-r--r--   0        0        0     5117 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/service.py
--rw-r--r--   0        0        0     2071 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/service.pyi
--rw-r--r--   0        0        0     2122 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/validators.py
--rw-r--r--   0        0        0     5005 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/storage.py
--rw-r--r--   0        0        0     1695 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/uid_gen.py
--rw-r--r--   0        0        0      900 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/utils/__init__.py
--rw-r--r--   0        0        0     1907 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/utils/content_utils.py
--rw-r--r--   0        0        0     2673 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/utils/path_utils.py
--rw-r--r--   0        0        0      851 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/utils/route_utils.py
--rw-r--r--   0        0        0      397 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/__init__.py
--rw-r--r--   0        0        0     4747 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/generator.py
--rw-r--r--   0        0        0     3706 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/helpers.py
--rw-r--r--   0        0        0     2024 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/__init__.py
--rw-r--r--   0        0        0     2864 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/binding.py
--rw-r--r--   0        0        0     1270 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/conditions.py
--rw-r--r--   0        0        0     1360 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/definitions.py
--rw-r--r--   0        0        0     1698 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/port_type.py
--rw-r--r--   0        0        0     1315 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/restrictions.py
--rw-r--r--   0        0        0     1947 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/schema.py
--rw-r--r--   0        0        0     1361 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/service.py
--rw-r--r--   0        0        0      561 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/utils.py
--rw-r--r--   0        0        0     2579 2024-04-18 11:28:45.518821 fastapi_xroad_soap-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4660 1970-01-01 00:00:00.000000 fastapi_xroad_soap-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    13831 2024-04-23 22:01:38.002570 fastapi_xroad_soap-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2939 2024-04-23 22:01:38.002570 fastapi_xroad_soap-0.4.0/README.md
+-rw-r--r--   0        0        0      524 2024-04-23 22:01:38.002570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/__init__.py
+-rw-r--r--   0        0        0      574 2024-04-23 22:01:38.002570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/elements.py
+-rw-r--r--   0        0        0      471 2024-04-23 22:01:38.002570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/faults.py
+-rw-r--r--   0        0        0      340 2024-04-23 22:01:38.002570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/__init__.py
+-rw-r--r--   0        0        0      666 2024-04-23 22:01:38.002570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/base/__init__.py
+-rw-r--r--   0        0        0     2953 2024-04-23 22:01:38.002570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/base/base_element_spec.py
+-rw-r--r--   0        0        0     1194 2024-04-23 22:01:38.002570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/base/composite_meta.py
+-rw-r--r--   0        0        0      988 2024-04-23 22:01:38.002570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/base/dynamic_spec.py
+-rw-r--r--   0        0        0     4392 2024-04-23 22:01:38.002570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/base/message_body.py
+-rw-r--r--   0        0        0     2705 2024-04-23 22:01:38.002570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/base/validators.py
+-rw-r--r--   0        0        0     1067 2024-04-23 22:01:38.002570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/constants.py
+-rw-r--r--   0        0        0      486 2024-04-23 22:01:38.002570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-23 22:01:38.002570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/models/__init__.py
+-rw-r--r--   0        0        0     1479 2024-04-23 22:01:38.002570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/models/boolean.py
+-rw-r--r--   0        0        0     1195 2024-04-23 22:01:38.002570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/models/date.py
+-rw-r--r--   0        0        0     1243 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/models/datetime.py
+-rw-r--r--   0        0        0     1180 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/models/float.py
+-rw-r--r--   0        0        0     1223 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/models/integer.py
+-rw-r--r--   0        0        0     1247 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/models/netres.py
+-rw-r--r--   0        0        0     1284 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/models/string.py
+-rw-r--r--   0        0        0     6437 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/models/swaref.py
+-rw-r--r--   0        0        0     1195 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/models/time.py
+-rw-r--r--   0        0        0     2125 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/numeric_type_spec.py
+-rw-r--r--   0        0        0     2276 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/string_type_spec.py
+-rw-r--r--   0        0        0     3767 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/validators.py
+-rw-r--r--   0        0        0      679 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/envelope/__init__.py
+-rw-r--r--   0        0        0     2861 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/envelope/factory.py
+-rw-r--r--   0        0        0     1413 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/envelope/generics.py
+-rw-r--r--   0        0        0     1912 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/envelope/header.py
+-rw-r--r--   0        0        0     1910 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/file_size.py
+-rw-r--r--   0        0        0      742 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/multipart/__init__.py
+-rw-r--r--   0        0        0     2608 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/multipart/bodypart.py
+-rw-r--r--   0        0        0     1898 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/multipart/decoder.py
+-rw-r--r--   0        0        0     2493 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/multipart/encoder.py
+-rw-r--r--   0        0        0     1020 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/multipart/errors.py
+-rw-r--r--   0        0        0      955 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/soap/__init__.py
+-rw-r--r--   0        0        0     5257 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/soap/action.py
+-rw-r--r--   0        0        0     4997 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/soap/faults.py
+-rw-r--r--   0        0        0     1654 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/soap/response.py
+-rw-r--r--   0        0        0     5251 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/soap/service.py
+-rw-r--r--   0        0        0     2071 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/soap/service.pyi
+-rw-r--r--   0        0        0     2004 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/soap/validators.py
+-rw-r--r--   0        0        0     5172 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/storage.py
+-rw-r--r--   0        0        0     1695 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/uid_gen.py
+-rw-r--r--   0        0        0     1068 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/utils/__init__.py
+-rw-r--r--   0        0        0     3057 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/utils/content_utils.py
+-rw-r--r--   0        0        0     2673 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/utils/path_utils.py
+-rw-r--r--   0        0        0      851 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/utils/route_utils.py
+-rw-r--r--   0        0        0      397 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/wsdl/__init__.py
+-rw-r--r--   0        0        0     5349 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/wsdl/generator.py
+-rw-r--r--   0        0        0     4274 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/wsdl/helpers.py
+-rw-r--r--   0        0        0     2050 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/wsdl/models/__init__.py
+-rw-r--r--   0        0        0     2864 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/wsdl/models/binding.py
+-rw-r--r--   0        0        0     1270 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/wsdl/models/conditions.py
+-rw-r--r--   0        0        0     1360 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/wsdl/models/definitions.py
+-rw-r--r--   0        0        0     1698 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/wsdl/models/port_type.py
+-rw-r--r--   0        0        0     1315 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/wsdl/models/restrictions.py
+-rw-r--r--   0        0        0     2139 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/wsdl/models/schema.py
+-rw-r--r--   0        0        0     1361 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/wsdl/models/service.py
+-rw-r--r--   0        0        0      561 2024-04-23 22:01:38.006570 fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/utils.py
+-rw-r--r--   0        0        0     2599 2024-04-23 22:01:38.098571 fastapi_xroad_soap-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4660 1970-01-01 00:00:00.000000 fastapi_xroad_soap-0.4.0/PKG-INFO
```

### Comparing `fastapi_xroad_soap-0.3.0/LICENSE` & `fastapi_xroad_soap-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/README.md` & `fastapi_xroad_soap-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/__init__.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/elements.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/elements.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/base/body.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/base/message_body.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,99 +7,99 @@
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 from __future__ import annotations
 import typing as t
 from pydantic_xml import model
-from pydantic.fields import ModelPrivateAttr
+from pydantic import fields
 from pydantic import (
 	PrivateAttr,
 	ValidationInfo,
 	model_validator
 )
+from .. import utils
 from ..constants import A8nType
-from .meta import CompositeMeta
+from .base_element_spec import BaseElementSpec
+from .composite_meta import CompositeMeta
+from .dynamic_spec import dynamic_spec
+from . import validators as vld
 
-try:
-	from .spec import BaseElementSpec
-except ImportError:  # pragma: no cover
-	BaseElementSpec: t.TypeAlias = t.Any
 
-
-__all__ = ["NestedModels", "MessageBody", "MessageBodyType"]
-
-
-NestedModels = t.List[t.Tuple[
-	t.Type["MessageBody"],
-	t.List[t.Type["MessageBody"]]
-]]
+__all__ = ["MessageBody", "MessageBodyType"]
 
 
 class MessageBody(model.BaseXmlModel, metaclass=CompositeMeta, search_mode='unordered', skip_empty=True):
 	_element_specs: t.Dict[str, BaseElementSpec] = PrivateAttr(default_factory=dict)
+	_T = t.TypeVar('_T', bound="MessageBody")
+
+	@classmethod
+	def wsdl_name(cls) -> str:
+		return cls.__xml_tag__ or cls.__name__
+
+	@classmethod
+	def Element(
+			cls: t.Type[_T],
+			*,
+			tag: t.Optional[str] = None,
+			ns: t.Optional[str] = None,
+			nsmap: t.Optional[t.Dict[str, str]] = None,
+			min_occurs: int = None,
+			max_occurs: t.Union[int, t.Literal["unbounded"]] = None
+	) -> _T:
+		kwargs = {k: v for k, v in locals().items() if v != cls}
+		return t.cast(MessageBody, dynamic_spec(cls, **kwargs))
 
 	@classmethod
 	def model_specs(cls) -> t.Dict[str, BaseElementSpec]:
 		privates = getattr(cls, "__private_attributes__", {})
-		attr: t.Union[ModelPrivateAttr, None] = privates.get("_element_specs")
+		attr: t.Union[fields.ModelPrivateAttr, None] = privates.get("_element_specs")
 		return attr.get_default() if attr is not None else dict()
 
 	@classmethod
-	def nested_models(cls) -> NestedModels:
-		models, children = [], []
+	def nested_models(cls) -> t.List[t.Type["MessageBody"]]:
+		excluded_models = ["SwaRefInternal"]
+		models = []
 		a8ns = getattr(cls, '__annotations__', {})
 		for key, value in a8ns.items():
-			if type(value) is CompositeMeta:
-				models.extend(value.get_nested_models())
-				children.append(value)
-		models.append((cls, children))
-		return models
-
-	@staticmethod
-	def _validate_list(attr: str, data: t.List[MessageBody], spec: BaseElementSpec):
-		if not isinstance(data, list):
-			raise ValueError(
-				f"expected attribute '{attr}' value to be a list, "
-				f"but received '{type(data).__name__}' instead."
-			)
-		count = len(data)
-		if count < spec.min_occurs:
-			raise ValueError(
-				f"expected at least {spec.min_occurs} "
-				f"{spec.tag} elements, got {count}"
-			)
-		elif isinstance(spec.max_occurs, int) and count > spec.max_occurs:
-			raise ValueError(
-				f"expected at most {spec.max_occurs} "
-				f"{spec.tag} elements, got {count}"
-			)
-		expected = spec.internal_type or spec.element_type
-		for item in data:
-			if not isinstance(item, expected):
+			origin = t.get_origin(value)
+			if origin is None:
+				continue
+			args = t.get_args(value)
+			args_len = len(args)
+			opt_union = args_len == 2 and type(None) in args
+			if not opt_union and args_len != 1:
 				raise ValueError(
-					f"unexpected type '{type(item).__name__}' "
-					f"in list for argument '{attr}'"
+					f"Invalid type annotation arguments '{args}' "
+					f"for class {cls.__name__} attribute '{key}'"
 				)
+			value = [a for a in args if a is not None][0]
+			if (
+				type(value) is not CompositeMeta
+				or value.__name__ in excluded_models
+			):
+				continue
+			models.extend(value.nested_models())
+		models.append(cls)
+		return models
 
 	# noinspection PyNestedDecorators
 	@model_validator(mode="before")
 	@classmethod
 	def _validate_before(cls, data: t.Dict[str, t.Any], info: ValidationInfo) -> t.Any:
 		# Used for validating model instantiation in user code
-		is_incoming_request = (info.context or {}).get("deserializing", False)
-		if is_incoming_request or not isinstance(data, dict):
+		if utils.is_incoming_request(info) or not isinstance(data, dict):
 			return data
 
 		for attr, spec in cls.model_specs().items():
 			expected = spec.internal_type or spec.element_type
 			value = data.get(attr)
 
 			if spec.a8n_type == A8nType.LIST:
-				cls._validate_list(attr, value, spec)
+				vld.validate_list_items(attr, value, spec)
 				spec.init_instantiated_data(value)
 				continue
 			elif spec.a8n_type == A8nType.OPT and value is None:
 				data[attr] = []
 				continue
 			elif spec.a8n_type == A8nType.MAND and attr not in data:
 				raise ValueError(f"argument '{attr}' is missing")
@@ -109,39 +109,34 @@
 			data[attr] = [value]
 			spec.init_instantiated_data(data[attr])
 		return data
 
 	@model_validator(mode="after")
 	def _validate_after(self, info: ValidationInfo) -> MessageBody:
 		# Used for validating deserialized incoming requests
-		is_incoming_request = (info.context or {}).get("deserializing", False)
-		if not is_incoming_request:  # is model instantiation in user code
+		if not utils.is_incoming_request(info):
 			return self
 
 		specs = getattr(self, "_element_specs", None)
 		if not specs:
 			return self
 
 		for attr, value in vars(self).items():
 			spec = specs.get(attr)  # type: BaseElementSpec
 			if spec is None:
 				continue
 			elif not isinstance(value, list):
 				value = [value]
-			count = len(value)
 
-			if count > 1 and spec.a8n_type in [A8nType.MAND, A8nType.OPT]:
-				raise ValueError(f"only one {spec.tag} element is allowed, got {count}")
-			elif count == 0 and spec.a8n_type == A8nType.MAND:
-				raise ValueError(f"must provide at least one {spec.tag} element")
-			elif spec.a8n_type == A8nType.LIST:
-				self._validate_list(attr, value, spec)
+			vld.validate_opt_mand_a8n(attr, value, spec)
+			if spec.a8n_type == A8nType.LIST:
+				vld.validate_list_items(attr, value, spec)
 				spec.init_deserialized_data(value)
 				continue
 
 			spec.init_deserialized_data(value)
-			value = value[0] if count == 1 else None
+			value = value[0] if len(value) == 1 else None
 			setattr(self, attr, value)
 		return self
 
 
 MessageBodyType = t.TypeVar("MessageBodyType", bound=MessageBody)
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/base/meta.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/base/composite_meta.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 from pydantic_xml import model
 from ..constants import A8nType
-from .spec import BaseElementSpec
+from .base_element_spec import BaseElementSpec
 
 
 __all__ = ["ElementSpecMeta", "CompositeMeta"]
 
 
 class ElementSpecMeta(type):
 	def __new__(cls, name, bases, class_fields, **kwargs):
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/constants.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,32 +8,33 @@
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 from enum import Enum
 
 
 __all__ = [
+    "XSD",
     "ENV_NSMAP",
     "XRO_NSMAP",
     "IDEN_NSMAP",
     "HEADER_NSMAP",
     "WSDL_NSMAP",
     "A8nType"
 ]
 
 
+XSD = "http://www.w3.org/2001/XMLSchema"
 ENV_NSMAP = {"soapenv": "http://schemas.xmlsoap.org/soap/envelope/"}
 XRO_NSMAP = {"xro": "http://x-road.eu/xsd/xroad.xsd"}
 IDEN_NSMAP = {"iden": "http://x-road.eu/xsd/identifiers"}
 HEADER_NSMAP = {**ENV_NSMAP, **XRO_NSMAP, **IDEN_NSMAP}
 WSDL_NSMAP = {
     "wsdl": "http://schemas.xmlsoap.org/wsdl/",
     "soap": "http://schemas.xmlsoap.org/wsdl/soap/",
     "wsi": "http://ws-i.org/profiles/basic/1.1/xsd",
-    "xsd": "http://www.w3.org/2001/XMLSchema",
     **XRO_NSMAP
 }
 
 
 class A8nType(Enum):
     LIST = "list"
     OPT = "optional"
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/__init__.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/boolean.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/models/time.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,43 +5,40 @@
 #
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import typing as t
-from fastapi_xroad_soap.internal.base import BaseElementSpec
+from enum import Enum
+from datetime import time
+from ..numeric_type_spec import NumericTypeSpec
 
 
-__all__ = ["BooleanSpec", "Boolean"]
+__all__ = ["TimeSpec", "Time"]
 
 
-class BooleanSpec(BaseElementSpec):
+class TimeSpec(NumericTypeSpec):
 	def __init__(self, **kwargs) -> None:
-		super().__init__(element_type=bool, **kwargs)
-
-	def init_instantiated_data(self, data: t.List[bool]) -> t.List[bool]:
-		return data
-
-	def init_deserialized_data(self, data: t.List[bool]) -> t.List[bool]:
-		return data
+		super().__init__(element_type=time, **kwargs)
 
 	@property
-	def has_constraints(self) -> bool:
-		return False
-
-	def wsdl_type_name(self, *, with_tns: bool = False) -> str:
-		return "boolean"
+	def default_wsdl_type_name(self) -> str:
+		return "time"
 
 
-class Boolean:
+class Time:
 	def __new__(
 			cls,
 			*,
 			tag: t.Optional[str] = None,
 			ns: t.Optional[str] = None,
 			nsmap: t.Optional[t.Dict[str, str]] = None,
 			min_occurs: int = None,
-			max_occurs: t.Union[int, t.Literal["unbounded"]] = None
-	) -> bool:
+			max_occurs: t.Union[int, t.Literal["unbounded"]] = None,
+			min_value: t.Optional[time] = None,
+			max_value: t.Optional[time] = None,
+			enumerations: t.Optional[t.Type[Enum]] = None,
+			pattern: t.Optional[str] = None
+	) -> time:
 		kwargs = {k: v for k, v in locals().items() if v != cls}
-		return t.cast(bool, BooleanSpec(**kwargs))
+		return t.cast(time, TimeSpec(**kwargs))
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/date.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/models/date.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/datetime.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/models/datetime.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/float.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/models/float.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/integer.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/models/integer.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/netres.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/models/netres.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/string.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/models/string.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/swaref.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/models/swaref.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,17 +14,15 @@
 import typing as t
 from pydantic.fields import Field
 from fastapi_xroad_soap.internal import utils
 from fastapi_xroad_soap.internal.storage import GlobalWeakStorage
 from fastapi_xroad_soap.internal.multipart import DecodedBodyPart
 from fastapi_xroad_soap.internal.file_size import FileSize
 from fastapi_xroad_soap.internal.base import (
-	BaseElementSpec,
-	CompositeMeta,
-	MessageBody
+	BaseElementSpec, MessageBody
 )
 
 
 __all__ = [
 	"SwaRefFile",
 	"SwaRefInternal",
 	"SwaRefSpec",
@@ -143,20 +141,20 @@
 			if not hasattr(obj, "content_id"):
 				continue
 			try:
 				file: DecodedBodyPart = GlobalWeakStorage.retrieve_object(obj.content_id)
 			except ValueError:
 				raise ValueError(f"no file attachment found $${obj.content_id}$$")
 
-			obj.name = file.file_name
+			obj.name = file.name
 			obj.size = len(file.content)
 			self.validate_file(obj.name, obj.size, file.content_id)
 
 			obj.digest = self.digest(file.content)
-			obj.mimetype = utils.guess_mime_type(file.file_name)
+			obj.mimetype = utils.guess_mime_type(file.name)
 			obj.content = utils.convert_to_utf8(file.content)
 
 			setattr(obj, "_file", file)
 			delattr(obj, "content_id")
 		return data
 
 
@@ -186,34 +184,14 @@
 			"Cannot directly instantiate SwaRef, you must "
 			"instantiate one of its attribute classes."
 		)
 
 
 class SwaRefUtils:
 	@classmethod
-	def contains_swa_ref_specs(cls, content_cls: t.Type[MessageBody]) -> bool:
-		# print(type(content_cls))
-		has_swa_ref = False
-
-		# Define recursion behavior
-		fields = getattr(content_cls, "model_fields", {})
-		for sub_content_cls in fields.values():
-			res = cls.contains_swa_ref_specs(sub_content_cls)
-			has_swa_ref |= res
-
-		# Check private attributes for SwaRef specs
-		if type(content_cls) is not CompositeMeta:
-			return has_swa_ref
-		specs = content_cls.model_specs()
-		for spec in specs.values():
-			if type(spec).__name__ == "SwaRefSpec":
-				has_swa_ref |= True
-		return has_swa_ref
-
-	@classmethod
 	def gather_specs_and_files(cls, content: MessageBody) -> _SwaRefTypes:
 		specs, files = [], []
 		if not isinstance(content, MessageBody):
 			return specs, files
 
 		# Define recursion behavior
 		for sub_content in vars(content).values():
@@ -229,20 +207,13 @@
 	@staticmethod
 	def _add_specs_and_files(
 			specs: t.List[SwaRefSpec],
 			files: t.List[SwaRefFile],
 			content: MessageBody
 	) -> None:
 		_specs = getattr(content, "_element_specs", None)
-		if _specs is None:
-			return
 		for attr, spec in _specs.items():
 			if not isinstance(spec, SwaRefSpec):
 				continue
+			for item in getattr(content, attr):
+				files.append(item)
 			specs.append(spec)
-			obj = getattr(content, attr)
-			if isinstance(obj, SwaRefFile):
-				files.append(obj)
-			elif isinstance(obj, list):
-				for item in obj:
-					if isinstance(item, SwaRefFile):
-						files.append(item)
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/numeric_type_spec.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/numeric_type_spec.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,33 +8,39 @@
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import functools
 import typing as t
 from abc import abstractmethod
 from ..base import BaseElementSpec
-from .validators import CommonValidators, NumberValidators
+from .. import utils
+from .validators import (
+	CommonValidators,
+	NumberValidators
+)
 
 
 __all__ = ["NumericTypeSpec"]
 
 
 class NumericTypeSpec(BaseElementSpec, CommonValidators, NumberValidators):
 	def __init__(self, element_type: t.Any, **kwargs) -> None:
 		self.min_value = kwargs.get("min_value", None)
 		self.max_value = kwargs.get("max_value", None)
 		self.total_digits = kwargs.get("total_digits", None)
 		self.enumerations = kwargs.get("enumerations", None)
 		self.pattern = kwargs.get("pattern", None)
+		self.validate_enum_value_types(element_type)
 		super().__init__(
 			element_type=element_type,
 			**kwargs
 		)
 
 	def process(self, obj: t.Any) -> t.Any:
+		self.validate_type(obj, self.element_type)
 		self.validate_pattern(obj)
 		self.validate_total_digits(obj)
 		self.validate_min_max_value(obj)
 		self.validate_enumerations(obj)
 		return obj
 
 	def init_instantiated_data(self, data: t.List[t.Any]) -> t.List[t.Any]:
@@ -53,16 +59,16 @@
 				self.total_digits,
 				self.enumerations,
 				self.pattern
 			]
 		])
 
 	def wsdl_type_name(self, *, with_tns: bool = False) -> str:
-		return self._assemble_wsdl_type_name(
-			signature=self._compute_signature(
+		return self.assemble_wsdl_type_name(
+			signature=utils.compute_signature(
 				self.min_value,
 				self.max_value,
 				self.total_digits,
 				self.enumerations,
 				self.pattern
 			),
 			with_tns=with_tns
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/string_type_spec.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/string_type_spec.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import functools
 import typing as t
 from abc import abstractmethod
 from ..base import BaseElementSpec
-from .validators import CommonValidators, StringValidators
+from .. import utils
+from .validators import (
+	CommonValidators,
+	StringValidators
+)
 
 
 __all__ = ["StringTypeSpec"]
 
 
 class StringTypeSpec(BaseElementSpec, CommonValidators, StringValidators):
 	def __init__(self, element_type: t.Any, **kwargs) -> None:
@@ -25,20 +29,22 @@
 		self.max_length = self.length or kwargs.get("max_length", None)
 		self.enumerations = kwargs.get("enumerations", None)
 		self.pattern = kwargs.get("pattern", None)
 		self.whitespace = (
 			kwargs.get("whitespace", None)
 			or t.cast(t.Literal, "preserve")
 		)
+		self.validate_enum_value_types(element_type)
 		super().__init__(
 			element_type=element_type,
 			**kwargs
 		)
 
 	def process(self, obj: t.Any) -> t.Any:
+		self.validate_type(obj, self.element_type)
 		self.validate_string_length(obj)
 		self.validate_pattern(obj)
 		self.validate_enumerations(obj)
 		return self.process_whitespace(obj)
 
 	def init_instantiated_data(self, data: t.List[t.Any]) -> t.List[t.Any]:
 		return [self.process(obj) for obj in data]
@@ -56,16 +62,16 @@
 				self.max_length,
 				self.pattern,
 				self.enumerations
 			]
 		)
 
 	def wsdl_type_name(self, *, with_tns: bool = False) -> str:
-		return self._assemble_wsdl_type_name(
-			signature=self._compute_signature(
+		return self.assemble_wsdl_type_name(
+			signature=utils.compute_signature(
 				self.length,
 				self.min_length,
 				self.max_length,
 				self.whitespace,
 				self.enumerations,
 				self.pattern
 			),
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/validators.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/elements/validators.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,59 +6,80 @@
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import re
 import typing as t
+from collections import abc
 from enum import Enum
 
 
 __all__ = [
 	"CommonValidators",
 	"StringValidators",
 	"NumberValidators"
 ]
 
 
 class CommonValidators:
 	min_value: t.Optional[t.Any] = None
 	max_value: t.Optional[t.Any] = None
 	pattern: t.Optional[str] = None
-	enumerations: t.Optional[t.Type[Enum]] = None
+	enumerations: t.Optional[abc.Iterable[Enum]] = None
+
+	@staticmethod
+	def validate_type(obj: t.Any, expected_type: t.Any) -> None:
+		if not isinstance(obj, expected_type):
+			raise TypeError(
+				f"invalid type {type(obj).__name__} for object "
+				f"{obj}, expected type {expected_type}"
+			)
 
 	def validate_min_max_value(self, obj: t.Any) -> None:
 		if self.min_value is not None and obj < self.min_value:
 			raise ValueError(
 				f"input value is less than the minimal value "
 				f"of {self.min_value} $${obj}$$"
 			)
 		if self.max_value is not None and obj > self.max_value:
 			raise ValueError(
 				f"input value is greater than the maximum allowable "
 				f"value of {self.max_value} $${obj}$$"
 			)
 
 	def validate_pattern(self, obj: t.Any) -> None:
-		string = str(obj)
-		if self.pattern is not None:
-			match = re.search(self.pattern, string)
-			if match is None:
-				raise ValueError(
-					f"input value does not match regex "
-					f"pattern '{self.pattern}' $${string}$$"
-				)
+		if self.pattern is None:
+			return
+		string = obj.isoformat() if hasattr(obj, "isoformat") else str(obj)
+		match = re.search(self.pattern, string)
+		if match is None:
+			raise ValueError(
+				f"input value does not match regex "
+				f"pattern '{self.pattern}' $${string}$$"
+			)
 
 	def validate_enumerations(self, obj: t.Any) -> None:
-		if self.enumerations is not None:
-			values = [item.value for item in self.enumerations]
-			if obj not in values:
-				raise ValueError(
-					f"input value is not one of the "
-					f"allowed values: {values} $${obj}$$"
+		if self.enumerations is None:
+			return
+		values = [item.value for item in self.enumerations]
+		if obj not in values:
+			raise ValueError(
+				f"input value is not one of the "
+				f"allowed values: {values} $${obj}$$"
+			)
+
+	def validate_enum_value_types(self, expected_type: t.Type) -> None:
+		if self.enumerations is None:
+			return
+		for item in self.enumerations:
+			if not isinstance(item.value, expected_type):
+				raise TypeError(
+					f"enum value {item.value} is not of type {expected_type} "
+					f"in enum {self.enumerations.__name__}"
 				)
 
 
 class StringValidators:
 	length: t.Optional[int] = None
 	min_length: t.Optional[int] = None
 	max_length: t.Optional[int] = None
@@ -81,16 +102,14 @@
 			if self.max_length is not None and lstr > self.max_length:
 				raise ValueError(
 					f"input value length exceeds maximum allowable "
 					f"length of {self.max_length} chars $${string}$$"
 				)
 
 	def process_whitespace(self, obj: t.Any) -> str:
-		if not isinstance(obj, str):
-			return obj
 		if self.whitespace == "replace":
 			return re.sub(r'\s', ' ', obj)
 		elif self.whitespace == "collapse":
 			return re.sub(r'\s+', ' ', obj)
 		return obj
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/envelope/__init__.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/envelope/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/envelope/factory.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/envelope/factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,17 +35,20 @@
 
 	def __class_getitem__(cls, content_type: t.Type[MessageBody]):
 		cls_name = f"{cls.__name__}[{content_type.__name__}]"
 		if content_type.__xml_tag__ is None:
 			content_type.__xml_tag__ = content_type.__name__
 		return type(cls_name, (cls,), {"_type": content_type})
 
-	def __init__(self) -> None:
+	def __init__(self, *, exclude_xroad_nsmap: bool = False) -> None:
 		nsmap = {**ENV_NSMAP}
-		if self._type and not issubclass(self._type, GenericFault):
+		if (
+			not exclude_xroad_nsmap and self._type
+			and not issubclass(self._type, GenericFault)
+		):
 			nsmap.update({**XRO_NSMAP, **IDEN_NSMAP})
 			if isinstance(self._type.__xml_nsmap__, dict):
 				nsmap.update(self._type.__xml_nsmap__)
 		self._factory = t.cast(GenericEnvelope, type(
 			'Factory', (GenericEnvelope,), {},
 			ns="soapenv", nsmap=nsmap
 		))
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/envelope/generics.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/envelope/generics.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 bases = [MessageBody, t.Generic[MessageBodyType]]
 
 
 class GenericEnvelope(*bases, tag="Envelope", nsmap=ENV_NSMAP, search_mode='unordered'):
 	header: t.Optional[XroadHeader] = element(tag="Header", default=None)
-	body: MessageBodyType = element(tag="Body", default=None)
+	body: t.Optional[MessageBodyType] = element(tag="Body", default=None)
 
 
 class GenericFault(*bases, tag="Fault", ns="soapenv", nsmap=ENV_NSMAP):
 	faultcode: str = element(tag="faultcode", ns='')
 	faultstring: str = element(tag="faultstring", ns='')
 	faultactor: t.Optional[str] = element(tag="faultactor", ns='', default=None)
 	detail: MessageBodyType = element(tag="detail", ns='', default=None)
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/envelope/header.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/envelope/header.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/file_size.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/file_size.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/multipart/__init__.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/multipart/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 #   SPDX-License-Identifier: EUPL-1.2
 #
 from .bodypart import DecodedBodyPart
 from .decoder import MultipartDecoder
 from .encoder import MultipartEncoder
 from .errors import (
 	MultipartError,
-	NonMultipartError,
+	MultipartBoundaryError,
 	InvalidSeparatorError,
 	MissingContentIDError
 )
 
 
 __all__ = [
 	"DecodedBodyPart",
 	"MultipartDecoder",
 	"MultipartEncoder",
 	"MultipartError",
-	"NonMultipartError",
+	"MultipartBoundaryError",
 	"InvalidSeparatorError",
 	"MissingContentIDError"
 ]
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/multipart/bodypart.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/multipart/bodypart.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 
 
 __all__ = ["DecodedBodyPart"]
 
 
 class DecodedBodyPart:
     headers: t.Optional[Message] = None
-    file_name: t.Optional[str] = None
+    name: t.Optional[str] = None
     content: t.Optional[bytes] = None
     content_id: t.Optional[str] = None
     is_mixed_multipart: bool = False
 
     def __init__(self, content: bytes) -> None:
         separator = b'\r\n\r\n'
         if separator not in content:
             raise InvalidSeparatorError()
 
         headers, content = utils.split_on_find(content, separator)
-        if headers:
+        if headers:  # pragma: no branch
             decoded: str = utils.detect_decode(headers)[0]
             self.headers = HeaderParser().parsestr(decoded)
 
-            if content:
+            if content:  # pragma: no branch
                 self.content = content
                 content_type = self.headers.get_content_type()
                 content_disp = self.headers.get_content_disposition()
                 boundary = self.headers.get_boundary()
 
                 if content_type and "multipart/mixed" in content_type:
                     self.is_mixed_multipart = True
@@ -59,21 +59,18 @@
         elif transfer_enc == "quoted-printable":
             return quopri.decodestring(content)
         elif transfer_enc == "binary":
             return content
         return content
 
     def set_file_metadata(self) -> None:
-        boundary = self.headers.get_boundary()
-        content_disp = self.headers.get_content_disposition()
-        if boundary is None and content_disp == "attachment":
-            self.file_name = self.headers.get_filename()
-            if self.file_name is None:
-                self.file_name = self.headers.get_param(
-                    header='content-disposition',
-                    param='name'
-                )
-            cid = self.headers.get("Content-ID")
-            if cid is None:
-                raise MissingContentIDError
-            cid = f"cid:{cid.lstrip('<').rstrip('>')}"
-            self.content_id = cid
+        self.name = self.headers.get_filename()
+        if self.name is None:
+            self.name = self.headers.get_param(
+                header='content-disposition',
+                param='name'
+            )
+        cid = self.headers.get("Content-ID")
+        if cid is None:
+            raise MissingContentIDError
+        cid = f"cid:{cid.lstrip('<').rstrip('>')}"
+        self.content_id = cid
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/multipart/decoder.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/multipart/decoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,46 +6,40 @@
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import typing as t
 from .bodypart import DecodedBodyPart
-from .errors import NonMultipartError
+from .errors import MultipartBoundaryError
 from .. import utils
 
 
 __all__ = ["MultipartDecoder"]
 
 
 class MultipartDecoder:
-    def __init__(self, content, content_type) -> None:
-        self.content_type = content_type
+    def __init__(self, content: bytes, content_type: str) -> None:
         self.parts: t.Tuple[DecodedBodyPart, ...] = tuple()
-        self._find_boundary()
+        self.boundary = self._find_boundary(content_type)
         self._parse_body(content)
 
-    def _find_boundary(self):
-        ct_info = tuple(x.strip() for x in self.content_type.split(';'))
-        mimetype = ct_info[0]
-        if mimetype.split('/')[0].lower() != 'multipart':
-            raise NonMultipartError(mimetype)
+    @staticmethod
+    def _find_boundary(content_type) -> bytes:
+        ct_info = tuple(x.strip() for x in content_type.split(';'))
         for item in ct_info[1:]:
             attr, value = utils.split_on_find(item, separator='=')
             if attr.lower() == 'boundary':
-                string = value.strip('"')
-                if not (string is None or isinstance(string, bytes)):
-                    self.boundary = string.encode('utf-8')
-                    continue
-                self.boundary = string
+                return value.strip('"').encode('utf-8')
+        raise MultipartBoundaryError
 
     @staticmethod
     def _fix_first_part(part, boundary_marker):
         bm_len = len(boundary_marker)
-        if boundary_marker == part[:bm_len]:
+        if boundary_marker == part[:bm_len]:  # pragma: no cover
             return part[bm_len:]
         return part
 
     def _parse_body(self, content: bytes) -> None:
         boundary = b''.join((b'--', self.boundary))
 
         def body_part(part):
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/multipart/encoder.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/multipart/encoder.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/multipart/errors.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/multipart/errors.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 __all__ = [
     "MultipartError",
-    "NonMultipartError",
+    "MultipartBoundaryError",
     "InvalidSeparatorError",
     "MissingContentIDError"
 ]
 
 
 class MultipartError(Exception):
     pass
 
 
-class NonMultipartError(MultipartError):
-    def __init__(self, mimetype: str):
-        msg = f"Unexpected mimetype in content-type header: '{mimetype}'"
+class MultipartBoundaryError(MultipartError):
+    def __init__(self):
+        msg = "Unable to locate multipart boundary in Content-Type header"
         super().__init__(msg)
 
 
 class InvalidSeparatorError(MultipartError):
     def __init__(self):
         msg = "Multipart request body does not conform to RFC-5322"
         super().__init__(msg)
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/__init__.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/soap/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from .action import SoapAction
 from .faults import (
 	SoapFault,
 	ClientFault,
 	ServerFault,
 	InvalidMethodFault,
 	InvalidActionFault,
+	InvalidContentTypeFault,
 	MissingBodyFault,
 	MissingHeaderFault,
 	MissingCIDFault,
 	DuplicateCIDFault,
 	ValidationFault
 )
 
@@ -30,13 +31,14 @@
 	"SoapService",
 	"SoapAction",
 	"SoapFault",
 	"ClientFault",
 	"ServerFault",
 	"InvalidMethodFault",
 	"InvalidActionFault",
+	"InvalidContentTypeFault",
 	"MissingBodyFault",
 	"MissingHeaderFault",
 	"MissingCIDFault",
 	"DuplicateCIDFault",
 	"ValidationFault"
 ]
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/action.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/soap/action.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import re
 import typing as t
-from fastapi import Request, Response
+from fastapi import Response
 from pydantic import (
 	BaseModel,
 	ValidationError,
 	field_validator
 )
 from ..base import MessageBody
 from ..storage import GlobalWeakStorage
@@ -70,30 +70,30 @@
 			args.insert(self.body_index, envelope.body.content)
 		if self.header_type is not None:
 			if envelope.header is None:
 				raise f.MissingHeaderFault(self.name)
 			args.insert(self.header_index, envelope.header)
 		return args
 
-	def response_from(self, ret_obj: t.Optional[MessageBody], header: XroadHeader) -> _RespFrom:
+	def response_from(
+			self,
+			ret: t.Optional[MessageBody] = None,
+			header: t.Optional[XroadHeader] = None
+	) -> _RespFrom:
 		has_return = self.return_type is not None
-		if not has_return and ret_obj is None:
+		if not has_return and ret is None:
 			return Response()
-		elif has_return and isinstance(ret_obj, self.return_type):
-			return SoapResponse(content=ret_obj, header=header)
-		raise TypeError(
-			f"Expected return type {self.return_type}, "
-			f"but received {ret_obj}"
-		)
-
-	async def parse(self, http_request: Request) -> GenericEnvelope:
-		content_type = http_request.headers.get("content-type")
+		elif has_return and isinstance(ret, self.return_type):
+			return SoapResponse(content=ret, header=header)
+		raise TypeError(f"Expected return type {self.return_type}, but received {ret}")
+
+	async def parse(self, http_body: bytes, content_type: str) -> GenericEnvelope:
+		if content_type is None:
+			raise f.InvalidContentTypeFault(content_type)
 		body_type = content_type.split(';')[0]
-		http_body = await http_request.body()
-
 		if body_type in ["text/xml", "application/xml", "application/soap+xml"]:
 			return self.deserialize(http_body)
 		elif body_type in ["multipart/related", "multipart/mixed"]:
 			files: t.List[DecodedBodyPart] = list()
 			decoder = MultipartDecoder(http_body, content_type)
 			envelope = None
 			for index, part in enumerate(decoder.parts):
@@ -104,15 +104,15 @@
 					nested_decoder = MultipartDecoder(part.content, content_type)
 					for nested_part in nested_decoder.parts:
 						files.append(nested_part)
 				else:
 					files.append(part)
 			http_body = self.process_files(envelope.content, files)
 			return self.deserialize(http_body)
-		raise f.ClientFault(f"Invalid content type: {body_type}")
+		raise f.InvalidContentTypeFault(body_type)
 
 	def process_files(self, xml_str: bytes, files: t.List[DecodedBodyPart]) -> bytes:
 		ids = [file.content_id for file in files]
 		for cid in ids:
 			if ids.count(cid) > 1:
 				raise f.DuplicateCIDFault(cid)
 		for file in files:
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/faults.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/soap/faults.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 __all__ = [
 	"SoapFault",
 	"ClientFault",
 	"ServerFault",
 	"InvalidMethodFault",
 	"InvalidActionFault",
 	"MissingActionFault",
+	"InvalidContentTypeFault",
 	"MissingBodyFault",
 	"MissingHeaderFault",
 	"MissingCIDFault",
 	"DuplicateCIDFault",
 	"ValidationFault"
 ]
 
@@ -85,27 +86,33 @@
 	def __init__(self, action: str) -> None:
 		msg = f"Service does not support SOAP action: {action}"
 		super().__init__(string=msg)
 
 
 class MissingActionFault(SoapFault):
 	def __init__(self):
-		msg = "SOAP action HTTP header is missing."
+		msg = "SOAPAction HTTP header is missing"
+		super().__init__(string=msg)
+
+
+class InvalidContentTypeFault(SoapFault):
+	def __init__(self, content_type: t.Any) -> None:
+		msg = f"Invalid content type: {content_type}"
 		super().__init__(string=msg)
 
 
 class MissingBodyFault(SoapFault):
 	def __init__(self, action_name: str) -> None:
-		msg = f"Body element missing from envelope for {action_name} SOAP action"
+		msg = f"Body element missing from envelope for SOAP action: {action_name}"
 		super().__init__(string=msg)
 
 
 class MissingHeaderFault(SoapFault):
 	def __init__(self, action_name: str) -> None:
-		msg = f"X-Road header element missing from envelope for {action_name} SOAP action"
+		msg = f"X-Road header element missing from envelope for SOAP action: {action_name}"
 		super().__init__(string=msg)
 
 
 class MissingCIDFault(SoapFault):
 	def __init__(self, cid: str) -> None:
 		msg = f"Content-ID missing from envelope: {cid}"
 		super().__init__(string=msg)
@@ -121,36 +128,60 @@
 	def __init__(self, ex: Exception) -> None:
 		error = str(ex)
 		parts = re.split(r'\n(?!\s\s)', error)
 		match = re.search(r"^(.*?)\sfor", parts[0])
 		string = match.group(1) if match else "validation error"
 		super().__init__(
 			http_status_code=400,
-			detail=self.extract_details(parts[1:]),
+			detail=self.extract_details(parts),
 			string=string + " in SOAP envelope",
 			code="Client"
 		)
 
-	@staticmethod
-	def extract_details(parts: t.List[str]) -> MessageBody:
+	@classmethod
+	def extract_details(cls, parts: t.List[str]) -> MessageBody:
 		class Detail(MessageBody):
 			location: str = element()
 			reason: str = element()
 			input_value: str = element(tag="inputValue")
 
 		class ErrorDetails(MessageBody):
 			details: t.List[Detail] = element(tag="validationError")
 
 		details = list()
 		for part in parts:
-			loc, msg = part.split('\n')
-			iv_match = re.search(r"\$\$(.*?)\$\$", msg)
-			if iv_match:
-				msg = msg.replace(f"$${iv_match.group(1)}$$", '')
-			ln_match = re.search(r"(\[line -?\d+]: )", msg)
-			re_match = re.search(r"\[line -?\d+]: (.+?) \[type=", msg)
-			details.append(Detail(
-				location=inflection.camelize(loc) if ln_match else "Unknown",
-				reason=re_match.group(1) if re_match else "Unknown",
-				input_value=iv_match.group(1) if iv_match else "Unknown",
-			))
+			loc, msg = None, part
+			sub_parts = part.split('\n')
+			if len(sub_parts) >= 2:
+				loc, msg = sub_parts[:2]
+
+			msg, input_value = cls.extract_input_value(msg)
+			location = cls.extract_location(loc, msg)
+			reason = cls.extract_reason(msg)
+
+			params = [location, reason, input_value]
+			if any(d != "Unknown" for d in params):
+				details.append(Detail(
+					location=location,
+					reason=reason,
+					input_value=input_value,
+				))
 		return ErrorDetails(details=details)
+
+	@staticmethod
+	def extract_input_value(msg: str) -> t.Tuple[str, str]:
+		match = re.search(r"\$\$(.*?)\$\$", msg)
+		if match:  # pragma: no cover
+			msg = msg.replace(f"$${match.group(1)}$$", '')
+		return msg, match.group(1) if match else "Unknown"
+
+	@staticmethod
+	def extract_reason(msg: str) -> str:
+		match = re.search(r"\[line -?\d+]: (.+?) \[type=", msg)
+		if match is None:  # pragma: no cover
+			match = re.search(r"^\s\s(.+?) \[type=", msg)
+		return match.group(1) if match else "Unknown"
+
+	@staticmethod
+	def extract_location(loc: str, msg: str) -> str:
+		ln_match = re.search(r"(\[line -?\d+]: )", msg)
+		return inflection.camelize(loc) if ln_match else "Unknown"
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/response.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/soap/response.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 			content=xml_str,
 			headers=http_headers,
 			status_code=http_status_code
 		)
 
 	@staticmethod
 	def serialize(content: MessageBody, header: t.Optional[XroadHeader]) -> bytes:
-		envelope = EnvelopeFactory[content.__class__]()
+		envelope = EnvelopeFactory[content.__class__](
+			exclude_xroad_nsmap=header is None
+		)
 		return envelope.serialize(
 			content=content,
 			header=header,
 			pretty_print=False,
 			skip_empty=True
 		)
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/service.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/soap/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,51 +77,54 @@
 		try:
 			if "wsdl" in http_request.query_params:
 				if self._wsdl_response is None:
 					self.regenerate_wsdl()
 				return self._wsdl_response
 			elif http_request.method != "POST":
 				raise f.InvalidMethodFault(http_request.method)
-
 			action = self._determine_action(http_request)
-			envelope = await action.parse(http_request)
+
+			http_body = await http_request.body()
+			content_type = http_request.headers.get("content-type")
+			envelope = await action.parse(http_body, content_type)
+
 			args = action.arguments_from(envelope)
 			ret = await self._await_or_call(action.handler, *args)
 			return action.response_from(ret, envelope.header)
 
 		except f.SoapFault as ex:
 			err, resp = ex, ex.response
 		except ValidationError as ex:
 			err, resp = ex, f.ValidationFault(ex).response
 		except (MultipartError, LxmlError) as ex:
 			err, resp = ex, f.ClientFault(ex).response
-		except Exception as ex:
+		except Exception as ex:  # pragma: no cover
 			if self._hide_ise_cause:
 				ex = "Internal Server Error"
 			err, resp = ex, f.ServerFault(ex).response
 
 		if self._fault_callback is not None:
 			await self._await_or_call(
 				self._fault_callback,
 				http_request, err
 			)
 		return resp
 
 	def _determine_action(self, http_request: Request) -> SoapAction:
 		name = http_request.headers.get("soapaction", '').strip('"')
-		valid_names = self._actions.keys()
 		if not name:
 			raise f.MissingActionFault()
-		elif name in valid_names:
+		valid_names = self._actions.keys()
+		if name in valid_names:
 			return self._actions[name]
 		sep = '#' if '#' in name else '/'
 		fragment: str = name.split(sep)[-1]
 		for vn in valid_names:
 			if vn == fragment:
-				return self._actions[name]
+				return self._actions[fragment]
 		raise f.InvalidActionFault(name)
 
 	@staticmethod
 	async def _await_or_call(func: FuncOrCoro, *args, **kwargs) -> t.Any:
 		if inspect.iscoroutinefunction(func):
 			return await func(*args, **kwargs)
 		return func(*args, **kwargs)
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/service.pyi` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/soap/service.pyi`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/validators.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/soap/validators.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,42 +17,28 @@
 
 __all__ = ["validate_annotations"]
 
 
 def validate_annotations(name: str, func: DecoratedCallable) -> dict:
 	anno = utils.get_annotations(func)
 	for key, value in anno.items():
-		_validate_a8n_key(key, name)
-		if key == "return":
-			_validate_a8n_return(value, name)
-		elif key == "body":
+		if key == "body":
 			_validate_a8n_body(key, value, name)
 		elif key == "header":
 			_validate_a8n_header(value, name)
+		elif key == "return":
+			_validate_a8n_return(value, name)
+		else:
+			raise ValueError(
+				f"Parameter name '{key}' not allowed for SOAP action {name}."
+				"\nOnly names 'body' and 'header' can be used for parameters."
+			)
 	return anno
 
 
-def _validate_a8n_key(key: str, name: str) -> None:
-	if key not in ["body", "header", "return"]:
-		raise ValueError(
-			f"Parameter name '{key}' not allowed for SOAP action {name}."
-			"\nOnly names 'body' and 'header' can be used for parameters."
-		)
-
-
-def _validate_a8n_return(value: t.Any, name: str) -> None:
-	if value is None:
-		return
-	if not isinstance(value, type) or not issubclass(value, MessageBody):
-		raise TypeError(
-			f"Return type annotation of the {name} SOAP action "
-			"must be either 'None' or a subclass of 'MessageBody'."
-		)
-
-
 def _validate_a8n_body(key: str, value: t.Any, name: str) -> None:
 	if value == XroadHeader:
 		raise TypeError(
 			f"Cannot set the 'XroadHeader' class as a type annotation "
 			f"to the 'body' parameter of the {name} SOAP action."
 		)
 	elif not isinstance(value, type) or not issubclass(value, MessageBody):
@@ -64,7 +50,17 @@
 
 def _validate_a8n_header(value: t.Any, name: str) -> None:
 	if value != XroadHeader:
 		raise ValueError(
 			f"The annotation of the 'headers' parameter of the {name} "
 			f"SOAP action must be the 'XroadHeaders' class."
 		)
+
+
+def _validate_a8n_return(value: t.Any, name: str) -> None:
+	if value is None:
+		return
+	if not isinstance(value, type) or not issubclass(value, MessageBody):
+		raise TypeError(
+			f"Return type annotation of the {name} SOAP action "
+			"must be either 'None' or a subclass of 'MessageBody'."
+		)
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/storage.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,9 +133,14 @@
 		"""
 		self.validate_fingerprint(fingerprint)
 		obj_id = fingerprint.split('-$$-')[1]
 		if raise_on_miss:
 			return self._objects[obj_id]
 		return self._objects.get(obj_id, None)
 
+	@classmethod
+	def new_subclass(cls) -> t.Type[GlobalWeakStorage]:
+		new_type = type('GlobalWeakStorage', (GlobalWeakStorage,), {})
+		return t.cast(t.Type[GlobalWeakStorage], new_type)
 
-ExportableGWS = type('GlobalWeakStorage', (GlobalWeakStorage,), {})
+
+ExportableGWS = GlobalWeakStorage.new_subclass()
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/uid_gen.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/uid_gen.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/utils/__init__.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/utils/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,19 @@
 #   SPDX-License-Identifier: EUPL-1.2
 #
 from .content_utils import (
 	split_on_find,
 	guess_mime_type,
 	detect_decode,
 	convert_to_utf8,
-	remove_memory_addresses
+	remove_memory_addresses,
+	compute_signature,
+	is_incoming_request,
+	linearize_xml,
+	extract_content_ids
 )
 from .path_utils import (
 	search_upwards,
 	resolve_relpath,
 	read_cached_file,
 	read_cached_xml_file
 )
@@ -29,14 +33,18 @@
 
 __all__ = [
 	"split_on_find",
 	"guess_mime_type",
 	"detect_decode",
 	"convert_to_utf8",
 	"remove_memory_addresses",
+	"compute_signature",
+	"is_incoming_request",
+	"linearize_xml",
+	"extract_content_ids",
 	"search_upwards",
 	"resolve_relpath",
 	"read_cached_file",
 	"read_cached_xml_file",
 	"get_annotations",
 	"extract_parameter_positions"
 ]
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/utils/content_utils.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/utils/content_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,25 +6,33 @@
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import re
 import chardet
+import hashlib
+import functools
 import mimetypes
 import typing as t
 import charset_normalizer as charset
+from pydantic import ValidationInfo
+from ..uid_gen import UIDGenerator
 
 
 __all__ = [
 	"split_on_find",
 	"guess_mime_type",
 	"detect_decode",
 	"convert_to_utf8",
-	"remove_memory_addresses"
+	"remove_memory_addresses",
+	"compute_signature",
+	"is_incoming_request",
+	"linearize_xml",
+	"extract_content_ids"
 ]
 
 
 _USB = t.Union[str, bytes]
 _USN = t.Union[str, None]
 
 
@@ -63,7 +71,40 @@
 	return string
 
 
 def remove_memory_addresses(string: bytes) -> bytes:
 	pattern = r"0x[0-9A-Fa-f]+"
 	cleaned_text = re.sub(pattern, '', string.decode())
 	return cleaned_text.encode()
+
+
+@functools.lru_cache(maxsize=None)
+def compute_signature(*args) -> str:
+	repr_forms = []
+	for arg in args:
+		has_dict = hasattr(arg, "__dict__")
+		subject = vars(arg) if has_dict else arg
+		repr_forms.append(repr(subject))
+
+	raw_sig = ''.join(repr_forms).encode()
+	cleaned_sig = remove_memory_addresses(raw_sig)
+	raw_digest = hashlib.shake_128(cleaned_sig).digest(12)
+	return UIDGenerator(mode="key").generate(raw_digest)
+
+
+def is_incoming_request(info: ValidationInfo) -> bool:
+	return (info.context or {}).get("deserializing", False)
+
+
+def linearize_xml(xml: str) -> bytes:
+	return re.sub(
+		pattern=r'>(\s+)<',
+		string=xml.strip(),
+		repl='><'
+	).encode()
+
+
+def extract_content_ids(xml_string: str, *, remove_from_xml: bool = False) -> t.Tuple[t.List[str], str]:
+	matches = re.findall(r"(cid:[0-9a-fA-F]+)", xml_string)
+	if remove_from_xml:  # pragma: no branch
+		xml_string = re.sub(r"cid:[0-9a-fA-F]+", 'cid:', xml_string)
+	return matches, xml_string
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/utils/path_utils.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/utils/route_utils.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/utils/route_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/generator.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/wsdl/generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import typing as t
 import inflection
+from ..base import MessageBody
 from ..constants import WSDL_NSMAP
 from ..soap.action import SoapAction
-from ..elements.models import SwaRefUtils
-from .helpers import gather_all_types
-from . import models as mod
+from ..elements.models import SwaRefSpec
+from . import helpers, models as mod
 
 
 __all__ = ["generate"]
 
 
 def generate(actions: t.Dict[str, SoapAction], name: str, tns: str) -> bytes:
 	wsdl_def = type(
 		"WSDLDefinitions", (mod.WSDLDefinitions,),
 		{}, nsmap={**WSDL_NSMAP, "tns": tns}
 	)
-	return wsdl_def(
+	wsdl_data: str = wsdl_def(
 		target_ns=tns,
 		name=name,
 		types=mod.WSDLTypes(
 			service_schema=mod.Schema(
 				target_ns=tns,
 				includes=[],
 				imports=_generate_imports(actions),
@@ -41,57 +41,70 @@
 		port_type=_generate_port_type(actions),
 		binding=_generate_binding(actions),
 		service=mod.WSDLService(
 			port=mod.WSDLPortBinding(
 				address=mod.SOAPAddress()
 			)
 		)
-	).to_xml(pretty_print=True)
+	).to_xml(pretty_print=True).decode()
+	return helpers.format_wsdl_definitions(wsdl_data)
 
 
 def _generate_imports(actions: t.Dict[str, SoapAction]) -> t.List[mod.Import]:
-	has_specs = SwaRefUtils.contains_swa_ref_specs
-	xro_xsd = "http://x-road.eu/xsd/xroad.xsd"
+	xro = "http://x-road.eu/xsd/xroad.xsd"
 	imports = [mod.Import(
-		namespace=xro_xsd,
-		schema_loc=xro_xsd
+		namespace=xro,
+		schema_loc=xro
 	)]
 	for action in actions.values():
-		if (
-			action.body_type is not None
-			and has_specs(action.body_type)
-		):
-			wsi = "http://ws-i.org/profiles/basic/1.1/"
+		for model in [action.body_type, action.return_type]:
+			if model is None:
+				continue
+			_add_swaref_import(model, imports)
+	return imports
+
+
+def _add_swaref_import(model: t.Type[MessageBody], imports: t.List[mod.Import]) -> None:
+	wsi = "http://ws-i.org/profiles/basic/1.1/"
+	for nested_model in model.nested_models():
+		specs = nested_model.model_specs()
+		for spec in specs.values():
+			if not isinstance(spec, SwaRefSpec):
+				continue
 			imports.append(mod.Import(
 				namespace=f"{wsi}xsd",
 				schema_loc=f"{wsi}swaref.xsd"
 			))
-	return imports
+			return
 
 
 def _generate_elements(actions: t.Dict[str, SoapAction]) -> t.List[mod.Element]:
-	elements = []
+	elements = {}
 	for name, action in actions.items():
 		for model in [action.body_type, action.return_type]:
-			if model is not None:
-				elements.append(mod.Element(
-					name=model.__name__,
-					type=f"tns:{model.__name__}"
-				))
+			if model is None:
+				continue
+			wsdl_name = model.wsdl_name()
+			if wsdl_name in elements:
+				continue
+			elements[wsdl_name] = mod.Element(
+				name=wsdl_name,
+				type=f"tns:{wsdl_name}"
+			)
 	return [
-		*elements,
+		*list(elements.values()),
 		mod.Element(
 			name="FaultResponse",
 			type="tns:FaultResponse"
 		)
 	]
 
 
 def _generate_types(actions: t.Dict[str, SoapAction]) -> t.Dict:
-	complex_types, simple_types = gather_all_types(actions)
+	complex_types, simple_types = helpers.gather_all_types(actions)
 	return dict(
 		complex_types=[
 			*complex_types,
 			mod.ComplexType(
 				name="FaultResponse",
 				sequence=mod.Sequence(
 					elements=[
@@ -110,66 +123,72 @@
 			)
 		],
 		simple_types=simple_types
 	)
 
 
 def _generate_messages(actions: t.Dict[str, SoapAction]) -> t.List[mod.WSDLMessage]:
-	messages = []
-	for name, action in actions.items():
+	messages = {}
+	for action in actions.values():
 		for model in [action.body_type, action.return_type]:
-			if model is not None:
-				messages.append(mod.WSDLMessage(
-					name=model.__name__,
-					parts=[mod.WSDLPart(element=f"tns:{model.__name__}")]
-				))
+			if model is None:
+				continue
+			wsdl_name = model.wsdl_name()
+			if wsdl_name in messages:
+				continue
+			messages[wsdl_name] = mod.WSDLMessage(
+				name=wsdl_name,
+				parts=[mod.WSDLPart(
+					element=f"tns:{wsdl_name}"
+				)]
+			)
 	return [
-		*messages,
+		*list(messages.values()),
 		mod.WSDLMessage(
 			name="FaultResponse",
 			parts=[mod.WSDLPart(element="tns:FaultResponse", name="fault")]
 		),
 		mod.WSDLMessage(
 			name="xroadHeader",
 			parts=[
-				mod.WSDLPart(element="xro:userId", name="userId"),
-				mod.WSDLPart(element="xro:protocolVersion", name="protocolVersion"),
-				mod.WSDLPart(element="xro:id", name="id"),
+				mod.WSDLPart(element="xro:client", name="client"),
 				mod.WSDLPart(element="xro:service", name="service"),
-				mod.WSDLPart(element="xro:client", name="client")
+				mod.WSDLPart(element="xro:id", name="id"),
+				mod.WSDLPart(element="xro:protocolVersion", name="protocolVersion"),
+				mod.WSDLPart(element="xro:userId", name="userId")
 			]
 		)
 	]
 
 
 def _generate_port_type(actions: t.Dict[str, SoapAction]) -> mod.WSDLPortType:
 	ops = []
 	for name, action in actions.items():
+		port_docs = port_input = port_output = None
+		if action.description is not None:
+			port_docs = mod.WSDLDocumentation(
+				title=inflection.titleize(name),
+				notes=action.description
+			)
+		if action.body_type is not None:
+			wsdl_name = action.body_type.wsdl_name()
+			port_input = mod.WSDLInputPort(
+				message=f"tns:{wsdl_name}",
+				name=wsdl_name
+			)
+		if action.return_type is not None:
+			wsdl_name = action.return_type.wsdl_name()
+			port_output = mod.WSDLOutputPort(
+				message=f"tns:{wsdl_name}",
+				name=wsdl_name
+			)
 		ops.append(mod.WSDLOperationPort(
-			documentation=(
-				None if action.description is None else
-				mod.WSDLDocumentation(
-					title=inflection.titleize(name),
-					notes=action.description
-				)
-			),
-			input=(
-				None if action.body_type is None else
-				mod.WSDLInputPort(
-					message=f"tns:{action.body_type.__name__}",
-					name=action.body_type.__name__
-				)
-			),
-			output=(
-				None if action.return_type is None else
-				mod.WSDLOutputPort(
-					message=f"tns:{action.return_type.__name__}",
-					name=action.return_type.__name__
-				)
-			),
+			documentation=port_docs,
+			input=port_input,
+			output=port_output,
 			name=name
 		))
 	return mod.WSDLPortType(operations=ops)
 
 
 def _generate_binding(actions: t.Dict[str, SoapAction]) -> mod.WSDLBinding:
 	return mod.WSDLBinding(
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/helpers.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/wsdl/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,62 +4,91 @@
 #   Copyright (c) 2024, Centre of Registers and Information Systems
 #
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
+import re
 import typing as t
+import inflection
 from ..soap.action import SoapAction
+from ..constants import A8nType
 from ..elements import NumericTypeSpec
 from ..elements import StringTypeSpec
-from ..base import NestedModels, BaseElementSpec
+from ..base import (
+	MessageBody,
+	CompositeMeta,
+	BaseElementSpec
+)
 from . import models as mod
 
 
-__all__ = ["gather_all_types"]
+__all__ = [
+	"format_wsdl_definitions",
+	"gather_all_types"
+]
 
 
-AllTypes = t.Tuple[t.List[mod.ComplexType], t.List[mod.SimpleType]]
+_AllTypes = t.Tuple[
+	t.List[mod.ComplexType],
+	t.List[mod.SimpleType]
+]
 
 
-def gather_all_types(actions: t.Dict[str, SoapAction]) -> AllTypes:
+def format_wsdl_definitions(wsdl_string: str) -> bytes:
+	return re.sub(
+		pattern=r'(<wsdl:definitions[^>]*>)',
+		repl=lambda match: match.group(1).replace(' ', '\n  '),
+		string=wsdl_string,
+		count=1
+	).encode()
+
+
+def gather_all_types(actions: t.Dict[str, SoapAction]) -> _AllTypes:
 	simple_types: t.Dict[str, mod.SimpleType] = {}
 	complex_types: t.List[mod.ComplexType] = []
-	models = _gather_models(actions)
 
-	for model, children in models:
+	for model in _gather_models(actions):
 		elements = []
-		for child in children:
-			elements.append(mod.Element(
-				name=child.__name__,
-				type=f"tns:{child.__name__}"
-			))
-		for spec in model.model_specs().values():
-			_add_simple_type(spec, simple_types)
+		for name, spec in model.model_specs().items():
+			if type(spec.element_type) is not CompositeMeta:
+				_add_simple_type(spec, simple_types)
 			elements.append(mod.Element(
-				name=spec.tag,
-				type=spec.wsdl_type_name(with_tns=True)
+				name=spec.tag or inflection.camelize(name),
+				type=spec.wsdl_type_name(with_tns=True),
+				max_occurs=(
+					None if
+					spec.a8n_type != A8nType.LIST
+					else str(spec.max_occurs)
+				),
+				min_occurs={
+					A8nType.MAND: None,
+					A8nType.LIST: str(spec.min_occurs),
+					A8nType.OPT: "0"
+				}[spec.a8n_type]
 			))
 		complex_types.append(mod.ComplexType(
-			name=model.__name__,
+			name=model.wsdl_name(),
 			sequence=mod.Sequence(
 				elements=elements
 			)
 		))
 	return complex_types, list(simple_types.values())
 
 
-def _gather_models(actions: t.Dict[str, SoapAction]) -> NestedModels:
+def _gather_models(actions: t.Dict[str, SoapAction]) -> t.List[t.Type["MessageBody"]]:
 	models = []
 	for action in actions.values():
 		for model in [action.body_type, action.return_type]:
+			if model is None:
+				continue
 			nested = model.nested_models()
 			models.extend(nested)
-	return models
+	return list(set(models))
 
 
 def _add_simple_type(spec: BaseElementSpec, simple_types: t.Dict[str, mod.SimpleType]) -> None:
 	if spec.has_constraints:
 		func = (
 			_create_string_simple_type if
 			isinstance(spec, StringTypeSpec)
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/__init__.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/wsdl/models/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 	StringTypeRestriction
 )
 from .schema import (
 	SimpleType,
 	AnyXML,
 	Element,
 	Sequence,
+	Attribute,
 	ComplexType,
 	Import,
 	Include,
 	Schema
 )
 from .service import (
 	SOAPAddress,
@@ -111,14 +112,15 @@
 	"StringTypeRestriction",
 
 	# schema.py
 	"SimpleType",
 	"AnyXML",
 	"Element",
 	"Sequence",
+	"Attribute",
 	"ComplexType",
 	"Import",
 	"Include",
 	"Schema",
 
 	# service.py
 	"SOAPAddress",
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/binding.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/wsdl/models/binding.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,30 +46,30 @@
 class WSDLFaultBinding(BaseXmlModel, tag="fault", ns="wsdl", nsmap=WSDL_NSMAP):
 	name: str = attr(default="FaultResponse")
 	fault: SOAPFault = SOAPFault()
 
 
 class WSDLOutputBinding(BaseXmlModel, tag="output", ns="wsdl", nsmap=WSDL_NSMAP):
 	headers: t.List[SOAPHeader] = [
-		SOAPHeader(part="userId"),
-		SOAPHeader(part="protocolVersion"),
-		SOAPHeader(part="id"),
+		SOAPHeader(part="client"),
 		SOAPHeader(part="service"),
-		SOAPHeader(part="client")
+		SOAPHeader(part="id"),
+		SOAPHeader(part="protocolVersion"),
+		SOAPHeader(part="userId")
 	]
 	body: SOAPBody = SOAPBody()
 
 
 class WSDLInputBinding(BaseXmlModel, tag="input", ns="wsdl", nsmap=WSDL_NSMAP):
 	headers: t.List[SOAPHeader] = [
-		SOAPHeader(part="userId"),
-		SOAPHeader(part="protocolVersion"),
-		SOAPHeader(part="id"),
+		SOAPHeader(part="client"),
 		SOAPHeader(part="service"),
-		SOAPHeader(part="client")
+		SOAPHeader(part="id"),
+		SOAPHeader(part="protocolVersion"),
+		SOAPHeader(part="userId")
 	]
 	body: SOAPBody = SOAPBody()
 
 
 class XROADVersion(BaseXmlModel, tag="version", ns="xro", nsmap=WSDL_NSMAP):
 	version: str = "v1"
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/conditions.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/wsdl/models/conditions.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/definitions.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/wsdl/models/definitions.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/port_type.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/wsdl/models/port_type.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/restrictions.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/wsdl/models/restrictions.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/schema.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/wsdl/models/schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 #
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import typing as t
-from pydantic_xml import BaseXmlModel, attr
-from fastapi_xroad_soap.internal.constants import WSDL_NSMAP
+from pydantic_xml import BaseXmlModel, element, attr
+from fastapi_xroad_soap.internal.constants import XSD
 from .restrictions import (
     NumericTypeRestriction,
     StringTypeRestriction
 )
 
 
 __all__ = [
     "AnyXML",
     "Element",
     "Sequence",
+    "Attribute",
     "ComplexType",
     "SimpleType",
     "Import",
     "Include",
     "Schema"
 ]
 
@@ -40,17 +41,23 @@
     max_occurs: t.Union[str, None] = attr(name="maxOccurs", default=None)
 
 
 class Sequence(BaseXmlModel, tag="sequence"):
     elements: t.List[t.Union[Element, AnyXML]]
 
 
-class ComplexType(BaseXmlModel, tag="complexType"):
+class Attribute(BaseXmlModel, tag="attribute"):
+    name: str = attr()
+    type: str = attr()
+
+
+class ComplexType(BaseXmlModel, tag="complexType", skip_empty=True):
     name: str = attr()
     sequence: Sequence
+    attribute: t.List[Attribute] = element(tag="attribute", default=None)
 
 
 class SimpleType(BaseXmlModel, tag="simpleType"):
     name: str = attr()
     restriction: t.Union[
         NumericTypeRestriction,
         StringTypeRestriction
@@ -63,14 +70,14 @@
 
 
 class Include(BaseXmlModel, tag="include"):
     schema_loc: str = attr(name="schemaLocation")
 
 
 class Schema(BaseXmlModel, tag="schema"):
-    xmlns: str = attr(default=WSDL_NSMAP["xsd"])
+    xmlns: str = attr(default=XSD)
     target_ns: str = attr(name="targetNamespace")
     imports: t.List[Import]
     includes: t.List[Include]
     elements: t.List[Element]
     complex_types: t.List[ComplexType]
     simple_types: t.List[SimpleType]
```

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/service.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/internal/wsdl/models/service.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/utils.py` & `fastapi_xroad_soap-0.4.0/fastapi_xroad_soap/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.3.0/pyproject.toml` & `fastapi_xroad_soap-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-xroad-soap"
-version = "0.3.0"
+version = "0.4.0"
 description = "FastAPI Extension for X-Road SOAP"
 authors = ["Zero Reports Team <zero.dev@rik.ee>"]
 license = "EUPL-1.2"
 readme = "README.md"
 keywords = ["fastapi", "xroad", "soap"]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -47,21 +47,21 @@
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.4.4"
 uvicorn = "^0.29.0"
-pyright = "^1.1.358"
+pyright = "^1.1.359"
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 pytest-asyncio = "^0.23.6"
 pytest-pyright = "^0.0.6"
 devtools-cli = "^0.13.3"
-types-lxml = "^2024.3.27"
+types-lxml = "^2024.4.14"
 httpx = "^0.27.0"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 console_output_style = "count"
 filterwarnings = ["ignore::DeprecationWarning"]
 pythonpath = [".", "fastapi_xroad_soap"]
@@ -74,14 +74,15 @@
 ]
 
 [tool.coverage.run]
 source = ["fastapi_xroad_soap/*"]
 branch = true
 
 [tool.coverage.report]
+skip_covered = true
 skip_empty = true
 ignore_errors = true
 exclude_lines = [
     "@abstractmethod",
     "pragma: no cover",
     "raise AssertionError",
     "raise NotImplementedError",
```

### Comparing `fastapi_xroad_soap-0.3.0/PKG-INFO` & `fastapi_xroad_soap-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-xroad-soap
-Version: 0.3.0
+Version: 0.4.0
 Summary: FastAPI Extension for X-Road SOAP
 License: EUPL-1.2
 Keywords: fastapi,xroad,soap
 Author: Zero Reports Team
 Author-email: zero.dev@rik.ee
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

