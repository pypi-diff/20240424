# Comparing `tmp/botocore_stubs-1.34.9.tar.gz` & `tmp/botocore_stubs-1.34.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore_stubs-1.34.9.tar", max compression
+gzip compressed data, was "botocore_stubs-1.34.90.tar", max compression
```

## Comparing `botocore_stubs-1.34.9.tar` & `botocore_stubs-1.34.90.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     1071 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/LICENSE
--rw-r--r--   0        0        0     1717 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/README.md
--rw-r--r--   0        0        0      586 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/__init__.pyi
--rw-r--r--   0        0        0     2923 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/args.pyi
--rw-r--r--   0        0        0     5122 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/auth.pyi
--rw-r--r--   0        0        0     4063 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/awsrequest.pyi
--rw-r--r--   0        0        0     6013 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/client.pyi
--rw-r--r--   0        0        0     2291 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/compat.pyi
--rw-r--r--   0        0        0      600 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/compress.pyi
--rw-r--r--   0        0        0     2556 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/config.pyi
--rw-r--r--   0        0        0      335 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/configloader.pyi
--rw-r--r--   0        0        0     3824 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/configprovider.pyi
--rw-r--r--   0        0        0    11621 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/credentials.pyi
--rw-r--r--   0        0        0       74 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/crt/__init__.pyi
--rw-r--r--   0        0        0     2126 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/crt/auth.pyi
--rw-r--r--   0        0        0     2307 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/discovery.pyi
--rw-r--r--   0        0        0      168 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/docs/__init__.pyi
--rw-r--r--   0        0        0       23 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/docs/bcdoc/__init__.pyi
--rw-r--r--   0        0        0     2119 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/docs/bcdoc/docstringparser.pyi
--rw-r--r--   0        0        0     1839 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/docs/bcdoc/restdoc.pyi
--rw-r--r--   0        0        0     4163 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/docs/bcdoc/style.pyi
--rw-r--r--   0        0        0     1085 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/docs/client.pyi
--rw-r--r--   0        0        0      459 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/docs/docstring.pyi
--rw-r--r--   0        0        0     2293 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/docs/example.pyi
--rw-r--r--   0        0        0     1228 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/docs/method.pyi
--rw-r--r--   0        0        0      583 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/docs/paginator.pyi
--rw-r--r--   0        0        0     2117 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/docs/params.pyi
--rw-r--r--   0        0        0      727 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/docs/service.pyi
--rw-r--r--   0        0        0      593 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/docs/shape.pyi
--rw-r--r--   0        0        0      565 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/docs/sharedexample.pyi
--rw-r--r--   0        0        0      401 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/docs/translator.pyi
--rw-r--r--   0        0        0     1383 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/docs/utils.pyi
--rw-r--r--   0        0        0      618 2023-12-27 21:10:09.753766 botocore_stubs-1.34.9/botocore-stubs/docs/waiter.pyi
--rw-r--r--   0        0        0     2205 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/endpoint.pyi
--rw-r--r--   0        0        0     6191 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/endpoint_provider.pyi
--rw-r--r--   0        0        0      708 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/errorfactory.pyi
--rw-r--r--   0        0        0     3464 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/eventstream.pyi
--rw-r--r--   0        0        0    21546 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/exceptions.pyi
--rw-r--r--   0        0        0     6983 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/handlers.pyi
--rw-r--r--   0        0        0      570 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/history.pyi
--rw-r--r--   0        0        0     2841 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/hooks.pyi
--rw-r--r--   0        0        0     2741 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/httpchecksum.pyi
--rw-r--r--   0        0        0     2343 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/httpsession.pyi
--rw-r--r--   0        0        0     2007 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/loaders.pyi
--rw-r--r--   0        0        0     6448 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/model.pyi
--rw-r--r--   0        0        0     2885 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/monitoring.pyi
--rw-r--r--   0        0        0     1777 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/paginate.pyi
--rw-r--r--   0        0        0     2099 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/parsers.pyi
--rw-r--r--   0        0        0        0 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/py.typed
--rw-r--r--   0        0        0     3252 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/regions.pyi
--rw-r--r--   0        0        0     1033 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/response.pyi
--rw-r--r--   0        0        0        0 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/retries/__init__.pyi
--rw-r--r--   0        0        0      916 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/retries/adaptive.pyi
--rw-r--r--   0        0        0      186 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/retries/base.pyi
--rw-r--r--   0        0        0      652 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/retries/bucket.pyi
--rw-r--r--   0        0        0      348 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/retries/quota.pyi
--rw-r--r--   0        0        0      367 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/retries/special.pyi
--rw-r--r--   0        0        0     4266 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/retries/standard.pyi
--rw-r--r--   0        0        0      485 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/retries/throttling.pyi
--rw-r--r--   0        0        0     2522 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/retryhandler.pyi
--rw-r--r--   0        0        0     1717 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/serialize.pyi
--rw-r--r--   0        0        0     6959 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/session.pyi
--rw-r--r--   0        0        0     3533 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/signers.pyi
--rw-r--r--   0        0        0     1934 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/stub.pyi
--rw-r--r--   0        0        0     1198 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/tokens.pyi
--rw-r--r--   0        0        0      310 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/translate.pyi
--rw-r--r--   0        0        0     1185 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/useragent.pyi
--rw-r--r--   0        0        0    14148 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/utils.pyi
--rw-r--r--   0        0        0     1172 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/validate.pyi
--rw-r--r--   0        0        0     1591 2023-12-27 21:10:09.757766 botocore_stubs-1.34.9/botocore-stubs/waiter.pyi
--rw-r--r--   0        0        0     2852 2023-12-27 21:10:34.650022 botocore_stubs-1.34.9/pyproject.toml
--rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 botocore_stubs-1.34.9/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/LICENSE
+-rw-r--r--   0        0        0     1717 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/README.md
+-rw-r--r--   0        0        0      586 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/__init__.pyi
+-rw-r--r--   0        0        0     2923 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/args.pyi
+-rw-r--r--   0        0        0     5122 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/auth.pyi
+-rw-r--r--   0        0        0     4063 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/awsrequest.pyi
+-rw-r--r--   0        0        0     6013 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/client.pyi
+-rw-r--r--   0        0        0     2300 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/compat.pyi
+-rw-r--r--   0        0        0      600 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/compress.pyi
+-rw-r--r--   0        0        0     2556 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/config.pyi
+-rw-r--r--   0        0        0      335 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/configloader.pyi
+-rw-r--r--   0        0        0     3824 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/configprovider.pyi
+-rw-r--r--   0        0        0    11621 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/credentials.pyi
+-rw-r--r--   0        0        0       74 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/crt/__init__.pyi
+-rw-r--r--   0        0        0     2126 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/crt/auth.pyi
+-rw-r--r--   0        0        0     2307 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/discovery.pyi
+-rw-r--r--   0        0        0      168 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/__init__.pyi
+-rw-r--r--   0        0        0       23 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/bcdoc/__init__.pyi
+-rw-r--r--   0        0        0     2119 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/bcdoc/docstringparser.pyi
+-rw-r--r--   0        0        0     1839 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/bcdoc/restdoc.pyi
+-rw-r--r--   0        0        0     4163 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/bcdoc/style.pyi
+-rw-r--r--   0        0        0     1085 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/client.pyi
+-rw-r--r--   0        0        0      459 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/docstring.pyi
+-rw-r--r--   0        0        0     2293 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/example.pyi
+-rw-r--r--   0        0        0     1228 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/method.pyi
+-rw-r--r--   0        0        0      583 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/paginator.pyi
+-rw-r--r--   0        0        0     2117 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/params.pyi
+-rw-r--r--   0        0        0      727 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/service.pyi
+-rw-r--r--   0        0        0      593 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/shape.pyi
+-rw-r--r--   0        0        0      565 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/sharedexample.pyi
+-rw-r--r--   0        0        0      401 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/translator.pyi
+-rw-r--r--   0        0        0     1383 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/utils.pyi
+-rw-r--r--   0        0        0      618 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/waiter.pyi
+-rw-r--r--   0        0        0     2205 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/endpoint.pyi
+-rw-r--r--   0        0        0     6191 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/endpoint_provider.pyi
+-rw-r--r--   0        0        0      708 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/errorfactory.pyi
+-rw-r--r--   0        0        0     3464 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/eventstream.pyi
+-rw-r--r--   0        0        0    21546 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/exceptions.pyi
+-rw-r--r--   0        0        0     6983 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/handlers.pyi
+-rw-r--r--   0        0        0      570 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/history.pyi
+-rw-r--r--   0        0        0     2841 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/hooks.pyi
+-rw-r--r--   0        0        0     2741 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/httpchecksum.pyi
+-rw-r--r--   0        0        0     2343 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/httpsession.pyi
+-rw-r--r--   0        0        0     2007 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/loaders.pyi
+-rw-r--r--   0        0        0     6448 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/model.pyi
+-rw-r--r--   0        0        0     2885 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/monitoring.pyi
+-rw-r--r--   0        0        0     1777 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/paginate.pyi
+-rw-r--r--   0        0        0     2099 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/parsers.pyi
+-rw-r--r--   0        0        0        0 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/py.typed
+-rw-r--r--   0        0        0     3252 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/regions.pyi
+-rw-r--r--   0        0        0     1033 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/response.pyi
+-rw-r--r--   0        0        0        0 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/retries/__init__.pyi
+-rw-r--r--   0        0        0      916 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/retries/adaptive.pyi
+-rw-r--r--   0        0        0      186 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/retries/base.pyi
+-rw-r--r--   0        0        0      652 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/retries/bucket.pyi
+-rw-r--r--   0        0        0      348 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/retries/quota.pyi
+-rw-r--r--   0        0        0      367 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/retries/special.pyi
+-rw-r--r--   0        0        0     4266 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/retries/standard.pyi
+-rw-r--r--   0        0        0      485 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/retries/throttling.pyi
+-rw-r--r--   0        0        0     2522 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/retryhandler.pyi
+-rw-r--r--   0        0        0     1717 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/serialize.pyi
+-rw-r--r--   0        0        0     6959 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/session.pyi
+-rw-r--r--   0        0        0     3745 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/signers.pyi
+-rw-r--r--   0        0        0     1934 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/stub.pyi
+-rw-r--r--   0        0        0     1198 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/tokens.pyi
+-rw-r--r--   0        0        0      310 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/translate.pyi
+-rw-r--r--   0        0        0     1185 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/useragent.pyi
+-rw-r--r--   0        0        0    14012 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/utils.pyi
+-rw-r--r--   0        0        0     1172 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/validate.pyi
+-rw-r--r--   0        0        0     1591 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/waiter.pyi
+-rw-r--r--   0        0        0     2818 2024-04-23 21:10:57.112978 botocore_stubs-1.34.90/pyproject.toml
+-rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 botocore_stubs-1.34.90/PKG-INFO
```

### Comparing `botocore_stubs-1.34.9/LICENSE` & `botocore_stubs-1.34.90/LICENSE`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/README.md` & `botocore_stubs-1.34.90/README.md`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/__init__.pyi` & `botocore_stubs-1.34.90/botocore-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/args.pyi` & `botocore_stubs-1.34.90/botocore-stubs/args.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/auth.pyi` & `botocore_stubs-1.34.90/botocore-stubs/auth.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/awsrequest.pyi` & `botocore_stubs-1.34.90/botocore-stubs/awsrequest.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/client.pyi` & `botocore_stubs-1.34.90/botocore-stubs/client.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/compat.pyi` & `botocore_stubs-1.34.90/botocore-stubs/compat.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 class HTTPHeaders(HTTPMessage):
     @classmethod
     def from_dict(cls: Type[_R], d: Mapping[str, Any]) -> _R: ...
     @classmethod
     def from_pairs(cls: Type[_R], pairs: Iterable[Tuple[str, Any]]) -> _R: ...
 
 file_type: Any
+zip: Any
 unquote_str = unquote_plus
 
 def set_socket_timeout(http_response: Any, timeout: Any) -> None: ...
 def accepts_kwargs(func: Any) -> Any: ...
 def ensure_unicode(s: Any, encoding: Optional[Any] = ..., errors: Optional[Any] = ...) -> Any: ...
 def ensure_bytes(s: Any, encoding: str = ..., errors: str = ...) -> Any: ...
```

### Comparing `botocore_stubs-1.34.9/botocore-stubs/compress.pyi` & `botocore_stubs-1.34.90/botocore-stubs/compress.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/config.pyi` & `botocore_stubs-1.34.90/botocore-stubs/config.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/configprovider.pyi` & `botocore_stubs-1.34.90/botocore-stubs/configprovider.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/credentials.pyi` & `botocore_stubs-1.34.90/botocore-stubs/credentials.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/crt/auth.pyi` & `botocore_stubs-1.34.90/botocore-stubs/crt/auth.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/discovery.pyi` & `botocore_stubs-1.34.90/botocore-stubs/discovery.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/docs/bcdoc/docstringparser.pyi` & `botocore_stubs-1.34.90/botocore-stubs/docs/bcdoc/docstringparser.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/docs/bcdoc/restdoc.pyi` & `botocore_stubs-1.34.90/botocore-stubs/docs/bcdoc/restdoc.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/docs/bcdoc/style.pyi` & `botocore_stubs-1.34.90/botocore-stubs/docs/bcdoc/style.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/docs/client.pyi` & `botocore_stubs-1.34.90/botocore-stubs/docs/client.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/docs/example.pyi` & `botocore_stubs-1.34.90/botocore-stubs/docs/example.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/docs/method.pyi` & `botocore_stubs-1.34.90/botocore-stubs/docs/method.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/docs/paginator.pyi` & `botocore_stubs-1.34.90/botocore-stubs/docs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/docs/params.pyi` & `botocore_stubs-1.34.90/botocore-stubs/docs/params.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/docs/service.pyi` & `botocore_stubs-1.34.90/botocore-stubs/docs/service.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/docs/shape.pyi` & `botocore_stubs-1.34.90/botocore-stubs/docs/shape.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/docs/sharedexample.pyi` & `botocore_stubs-1.34.90/botocore-stubs/docs/sharedexample.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/docs/utils.pyi` & `botocore_stubs-1.34.90/botocore-stubs/docs/utils.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/docs/waiter.pyi` & `botocore_stubs-1.34.90/botocore-stubs/docs/waiter.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/endpoint.pyi` & `botocore_stubs-1.34.90/botocore-stubs/endpoint.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/endpoint_provider.pyi` & `botocore_stubs-1.34.90/botocore-stubs/endpoint_provider.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/errorfactory.pyi` & `botocore_stubs-1.34.90/botocore-stubs/errorfactory.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/eventstream.pyi` & `botocore_stubs-1.34.90/botocore-stubs/eventstream.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/exceptions.pyi` & `botocore_stubs-1.34.90/botocore-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/handlers.pyi` & `botocore_stubs-1.34.90/botocore-stubs/handlers.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/history.pyi` & `botocore_stubs-1.34.90/botocore-stubs/history.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/hooks.pyi` & `botocore_stubs-1.34.90/botocore-stubs/hooks.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/httpchecksum.pyi` & `botocore_stubs-1.34.90/botocore-stubs/httpchecksum.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/httpsession.pyi` & `botocore_stubs-1.34.90/botocore-stubs/httpsession.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/loaders.pyi` & `botocore_stubs-1.34.90/botocore-stubs/loaders.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/model.pyi` & `botocore_stubs-1.34.90/botocore-stubs/model.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/monitoring.pyi` & `botocore_stubs-1.34.90/botocore-stubs/monitoring.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/paginate.pyi` & `botocore_stubs-1.34.90/botocore-stubs/paginate.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/parsers.pyi` & `botocore_stubs-1.34.90/botocore-stubs/parsers.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/regions.pyi` & `botocore_stubs-1.34.90/botocore-stubs/regions.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/response.pyi` & `botocore_stubs-1.34.90/botocore-stubs/response.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/retries/adaptive.pyi` & `botocore_stubs-1.34.90/botocore-stubs/retries/adaptive.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/retries/bucket.pyi` & `botocore_stubs-1.34.90/botocore-stubs/retries/bucket.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/retries/standard.pyi` & `botocore_stubs-1.34.90/botocore-stubs/retries/standard.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/retryhandler.pyi` & `botocore_stubs-1.34.90/botocore-stubs/retryhandler.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/serialize.pyi` & `botocore_stubs-1.34.90/botocore-stubs/serialize.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/session.pyi` & `botocore_stubs-1.34.90/botocore-stubs/session.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/signers.pyi` & `botocore_stubs-1.34.90/botocore-stubs/signers.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-from typing import Any, Mapping, Optional
+from typing import Any, Mapping, Optional, Union
 
 from botocore.awsrequest import create_request_object as create_request_object
 from botocore.awsrequest import prepare_request_dict as prepare_request_dict
 from botocore.compat import OrderedDict as OrderedDict
+from botocore.credentials import Credentials, ReadOnlyCredentials
 from botocore.exceptions import UnknownClientMethodError as UnknownClientMethodError
 from botocore.exceptions import UnknownSignatureVersionError as UnknownSignatureVersionError
 from botocore.exceptions import UnsupportedSignatureVersionError as UnsupportedSignatureVersionError
 from botocore.hooks import BaseEventHooks
 from botocore.model import ServiceId
 from botocore.utils import datetime2timestamp as datetime2timestamp
 
+_CredentialsUnion = Union[Credentials, ReadOnlyCredentials]
+
 class RequestSigner:
     def __init__(
         self,
         service_id: ServiceId,
         region_name: str,
         signing_name: str,
         signature_version: str,
-        credentials: Any,
+        credentials: _CredentialsUnion,
         event_emitter: BaseEventHooks,
         auth_token: Optional[str] = ...,
     ) -> None: ...
     @property
     def region_name(self) -> str: ...
     @property
     def signature_version(self) -> str: ...
@@ -40,14 +43,15 @@
         signing_name: Optional[str] = ...,
     ) -> None: ...
     def get_auth_instance(
         self,
         signing_name: str,
         region_name: str,
         signature_version: Optional[str] = ...,
+        request_credentials: Optional[_CredentialsUnion] = ...,
         **kwargs: Any,
     ) -> Any: ...
     get_auth: Any = ...
     def generate_presigned_url(
         self,
         request_dict: Mapping[str, Any],
         operation_name: str,
```

### Comparing `botocore_stubs-1.34.9/botocore-stubs/stub.pyi` & `botocore_stubs-1.34.90/botocore-stubs/stub.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/tokens.pyi` & `botocore_stubs-1.34.90/botocore-stubs/tokens.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/useragent.pyi` & `botocore_stubs-1.34.90/botocore-stubs/useragent.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/utils.pyi` & `botocore_stubs-1.34.90/botocore-stubs/utils.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -186,17 +186,14 @@
     def __init__(
         self,
         client: BaseClient,
         credential_cls: Type[Credentials],
         cache: Optional[S3ExpressIdentityCache] = ...,
     ) -> None: ...
     def register(self, event_emitter: Optional[BaseEventHooks] = ...) -> None: ...
-    def inject_signing_cache_key(
-        self, params: Mapping[str, Any], context: Mapping[str, Any], **kwargs: Any
-    ) -> None: ...
     def apply_signing_cache_key(
         self, params: Mapping[str, Any], context: Mapping[str, Any], **kwargs: Any
     ) -> None: ...
     def resolve_s3express_identity(
         self,
         request: Any,
         signing_name: str,
```

### Comparing `botocore_stubs-1.34.9/botocore-stubs/validate.pyi` & `botocore_stubs-1.34.90/botocore-stubs/validate.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/botocore-stubs/waiter.pyi` & `botocore_stubs-1.34.90/botocore-stubs/waiter.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.9/pyproject.toml` & `botocore_stubs-1.34.90/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.black]
 line-length = 100
 include = '(botocore-stubs)/.*\.pyi?$'
-target-version = ['py37', 'py38', 'py39', 'py310']
+target-version = ['py38', 'py39', 'py310', 'py311', 'py312']
 preview = true
 
 [tool.isort]
 profile = "black"
 line_length = 100
 src_paths = []
 
 [tool.poetry]
 name = "botocore-stubs"
-version = "1.34.9"
+version = "1.34.90"
 description = "Type annotations and code completion for botocore"
 authors = ["Vlad Emelianov <vlad.emelianov.nz@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://youtype.github.io/mypy_boto3_builder/"
 repository = "https://github.com/youtype/botocore-stubs"
 documentation = "https://youtype.github.io/mypy_boto3_builder/"
@@ -23,15 +23,14 @@
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.13",
     "Programming Language :: Python :: 3 :: Only",
@@ -82,8 +81,8 @@
 exclude = ["**/__pycache__", "tests", "typestubs"]
 reportMissingImports = "error"
 reportMissingTypeStubs = false
 reportMissingTypeArgument = "error"
 reportIncompatibleMethodOverride = "error"
 reportIncompatibleVariableOverride = false
 reportUnknownParameterType = "error"
-pythonVersion = "3.7"
+pythonVersion = "3.8"
```

### Comparing `botocore_stubs-1.34.9/PKG-INFO` & `botocore_stubs-1.34.90/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-stubs
-Version: 1.34.9
+Version: 1.34.90
 Summary: Type annotations and code completion for botocore
 Home-page: https://youtype.github.io/mypy_boto3_builder/
 License: MIT
 Keywords: botocore,type-annotations,pyright,mypy,boto3
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -17,15 +17,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.13
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Stubs Only
 Provides-Extra: botocore
 Requires-Dist: botocore ; extra == "botocore"
 Requires-Dist: types-awscrt
 Requires-Dist: typing-extensions (>=4.1.0) ; python_version < "3.9"
```

