# Comparing `tmp/botocore_stubs-1.34.90.tar.gz` & `tmp/botocore_stubs-1.34.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore_stubs-1.34.90.tar", max compression
+gzip compressed data, was "botocore_stubs-1.34.91.tar", max compression
```

## Comparing `botocore_stubs-1.34.90.tar` & `botocore_stubs-1.34.91.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     1071 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/LICENSE
--rw-r--r--   0        0        0     1717 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/README.md
--rw-r--r--   0        0        0      586 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/__init__.pyi
--rw-r--r--   0        0        0     2923 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/args.pyi
--rw-r--r--   0        0        0     5122 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/auth.pyi
--rw-r--r--   0        0        0     4063 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/awsrequest.pyi
--rw-r--r--   0        0        0     6013 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/client.pyi
--rw-r--r--   0        0        0     2300 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/compat.pyi
--rw-r--r--   0        0        0      600 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/compress.pyi
--rw-r--r--   0        0        0     2556 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/config.pyi
--rw-r--r--   0        0        0      335 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/configloader.pyi
--rw-r--r--   0        0        0     3824 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/configprovider.pyi
--rw-r--r--   0        0        0    11621 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/credentials.pyi
--rw-r--r--   0        0        0       74 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/crt/__init__.pyi
--rw-r--r--   0        0        0     2126 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/crt/auth.pyi
--rw-r--r--   0        0        0     2307 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/discovery.pyi
--rw-r--r--   0        0        0      168 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/__init__.pyi
--rw-r--r--   0        0        0       23 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/bcdoc/__init__.pyi
--rw-r--r--   0        0        0     2119 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/bcdoc/docstringparser.pyi
--rw-r--r--   0        0        0     1839 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/bcdoc/restdoc.pyi
--rw-r--r--   0        0        0     4163 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/bcdoc/style.pyi
--rw-r--r--   0        0        0     1085 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/client.pyi
--rw-r--r--   0        0        0      459 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/docstring.pyi
--rw-r--r--   0        0        0     2293 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/example.pyi
--rw-r--r--   0        0        0     1228 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/method.pyi
--rw-r--r--   0        0        0      583 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/paginator.pyi
--rw-r--r--   0        0        0     2117 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/params.pyi
--rw-r--r--   0        0        0      727 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/service.pyi
--rw-r--r--   0        0        0      593 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/shape.pyi
--rw-r--r--   0        0        0      565 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/sharedexample.pyi
--rw-r--r--   0        0        0      401 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/translator.pyi
--rw-r--r--   0        0        0     1383 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/utils.pyi
--rw-r--r--   0        0        0      618 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/docs/waiter.pyi
--rw-r--r--   0        0        0     2205 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/endpoint.pyi
--rw-r--r--   0        0        0     6191 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/endpoint_provider.pyi
--rw-r--r--   0        0        0      708 2024-04-23 21:10:32.608481 botocore_stubs-1.34.90/botocore-stubs/errorfactory.pyi
--rw-r--r--   0        0        0     3464 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/eventstream.pyi
--rw-r--r--   0        0        0    21546 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/exceptions.pyi
--rw-r--r--   0        0        0     6983 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/handlers.pyi
--rw-r--r--   0        0        0      570 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/history.pyi
--rw-r--r--   0        0        0     2841 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/hooks.pyi
--rw-r--r--   0        0        0     2741 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/httpchecksum.pyi
--rw-r--r--   0        0        0     2343 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/httpsession.pyi
--rw-r--r--   0        0        0     2007 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/loaders.pyi
--rw-r--r--   0        0        0     6448 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/model.pyi
--rw-r--r--   0        0        0     2885 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/monitoring.pyi
--rw-r--r--   0        0        0     1777 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/paginate.pyi
--rw-r--r--   0        0        0     2099 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/parsers.pyi
--rw-r--r--   0        0        0        0 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/py.typed
--rw-r--r--   0        0        0     3252 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/regions.pyi
--rw-r--r--   0        0        0     1033 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/response.pyi
--rw-r--r--   0        0        0        0 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/retries/__init__.pyi
--rw-r--r--   0        0        0      916 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/retries/adaptive.pyi
--rw-r--r--   0        0        0      186 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/retries/base.pyi
--rw-r--r--   0        0        0      652 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/retries/bucket.pyi
--rw-r--r--   0        0        0      348 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/retries/quota.pyi
--rw-r--r--   0        0        0      367 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/retries/special.pyi
--rw-r--r--   0        0        0     4266 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/retries/standard.pyi
--rw-r--r--   0        0        0      485 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/retries/throttling.pyi
--rw-r--r--   0        0        0     2522 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/retryhandler.pyi
--rw-r--r--   0        0        0     1717 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/serialize.pyi
--rw-r--r--   0        0        0     6959 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/session.pyi
--rw-r--r--   0        0        0     3745 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/signers.pyi
--rw-r--r--   0        0        0     1934 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/stub.pyi
--rw-r--r--   0        0        0     1198 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/tokens.pyi
--rw-r--r--   0        0        0      310 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/translate.pyi
--rw-r--r--   0        0        0     1185 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/useragent.pyi
--rw-r--r--   0        0        0    14012 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/utils.pyi
--rw-r--r--   0        0        0     1172 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/validate.pyi
--rw-r--r--   0        0        0     1591 2024-04-23 21:10:32.612481 botocore_stubs-1.34.90/botocore-stubs/waiter.pyi
--rw-r--r--   0        0        0     2818 2024-04-23 21:10:57.112978 botocore_stubs-1.34.90/pyproject.toml
--rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 botocore_stubs-1.34.90/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/LICENSE
+-rw-r--r--   0        0        0     1717 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/README.md
+-rw-r--r--   0        0        0      586 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/__init__.pyi
+-rw-r--r--   0        0        0     2923 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/args.pyi
+-rw-r--r--   0        0        0     5122 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/auth.pyi
+-rw-r--r--   0        0        0     4063 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/awsrequest.pyi
+-rw-r--r--   0        0        0     6013 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/client.pyi
+-rw-r--r--   0        0        0     2300 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/compat.pyi
+-rw-r--r--   0        0        0      600 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/compress.pyi
+-rw-r--r--   0        0        0     2556 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/config.pyi
+-rw-r--r--   0        0        0      335 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/configloader.pyi
+-rw-r--r--   0        0        0     3824 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/configprovider.pyi
+-rw-r--r--   0        0        0    11621 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/credentials.pyi
+-rw-r--r--   0        0        0       74 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/crt/__init__.pyi
+-rw-r--r--   0        0        0     2126 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/crt/auth.pyi
+-rw-r--r--   0        0        0     2307 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/discovery.pyi
+-rw-r--r--   0        0        0      168 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/docs/__init__.pyi
+-rw-r--r--   0        0        0       23 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/docs/bcdoc/__init__.pyi
+-rw-r--r--   0        0        0     2119 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/docs/bcdoc/docstringparser.pyi
+-rw-r--r--   0        0        0     1839 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/docs/bcdoc/restdoc.pyi
+-rw-r--r--   0        0        0     4163 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/docs/bcdoc/style.pyi
+-rw-r--r--   0        0        0     1085 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/docs/client.pyi
+-rw-r--r--   0        0        0      459 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/docs/docstring.pyi
+-rw-r--r--   0        0        0     2293 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/docs/example.pyi
+-rw-r--r--   0        0        0     1228 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/docs/method.pyi
+-rw-r--r--   0        0        0      583 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/docs/paginator.pyi
+-rw-r--r--   0        0        0     2117 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/docs/params.pyi
+-rw-r--r--   0        0        0      727 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/docs/service.pyi
+-rw-r--r--   0        0        0      593 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/docs/shape.pyi
+-rw-r--r--   0        0        0      565 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/docs/sharedexample.pyi
+-rw-r--r--   0        0        0      401 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/docs/translator.pyi
+-rw-r--r--   0        0        0     1383 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/docs/utils.pyi
+-rw-r--r--   0        0        0      618 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/docs/waiter.pyi
+-rw-r--r--   0        0        0     2205 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/endpoint.pyi
+-rw-r--r--   0        0        0     6191 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/endpoint_provider.pyi
+-rw-r--r--   0        0        0      708 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/errorfactory.pyi
+-rw-r--r--   0        0        0     3464 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/eventstream.pyi
+-rw-r--r--   0        0        0    21546 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/exceptions.pyi
+-rw-r--r--   0        0        0     6983 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/handlers.pyi
+-rw-r--r--   0        0        0      570 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/history.pyi
+-rw-r--r--   0        0        0     2841 2024-04-24 20:12:09.474241 botocore_stubs-1.34.91/botocore-stubs/hooks.pyi
+-rw-r--r--   0        0        0     2741 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/httpchecksum.pyi
+-rw-r--r--   0        0        0     2343 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/httpsession.pyi
+-rw-r--r--   0        0        0     2007 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/loaders.pyi
+-rw-r--r--   0        0        0     6448 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/model.pyi
+-rw-r--r--   0        0        0     2885 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/monitoring.pyi
+-rw-r--r--   0        0        0     1777 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/paginate.pyi
+-rw-r--r--   0        0        0     2099 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/parsers.pyi
+-rw-r--r--   0        0        0        0 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/py.typed
+-rw-r--r--   0        0        0     3252 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/regions.pyi
+-rw-r--r--   0        0        0     1033 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/response.pyi
+-rw-r--r--   0        0        0        0 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/retries/__init__.pyi
+-rw-r--r--   0        0        0      916 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/retries/adaptive.pyi
+-rw-r--r--   0        0        0      186 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/retries/base.pyi
+-rw-r--r--   0        0        0      652 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/retries/bucket.pyi
+-rw-r--r--   0        0        0      348 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/retries/quota.pyi
+-rw-r--r--   0        0        0      367 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/retries/special.pyi
+-rw-r--r--   0        0        0     4266 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/retries/standard.pyi
+-rw-r--r--   0        0        0      485 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/retries/throttling.pyi
+-rw-r--r--   0        0        0     2522 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/retryhandler.pyi
+-rw-r--r--   0        0        0     1717 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/serialize.pyi
+-rw-r--r--   0        0        0     6959 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/session.pyi
+-rw-r--r--   0        0        0     3745 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/signers.pyi
+-rw-r--r--   0        0        0     1934 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/stub.pyi
+-rw-r--r--   0        0        0     1198 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/tokens.pyi
+-rw-r--r--   0        0        0      310 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/translate.pyi
+-rw-r--r--   0        0        0     1185 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/useragent.pyi
+-rw-r--r--   0        0        0    14012 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/utils.pyi
+-rw-r--r--   0        0        0     1172 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/validate.pyi
+-rw-r--r--   0        0        0     1591 2024-04-24 20:12:09.478241 botocore_stubs-1.34.91/botocore-stubs/waiter.pyi
+-rw-r--r--   0        0        0     2818 2024-04-24 20:12:33.194503 botocore_stubs-1.34.91/pyproject.toml
+-rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 botocore_stubs-1.34.91/PKG-INFO
```

### Comparing `botocore_stubs-1.34.90/LICENSE` & `botocore_stubs-1.34.91/LICENSE`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/README.md` & `botocore_stubs-1.34.91/README.md`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/__init__.pyi` & `botocore_stubs-1.34.91/botocore-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/args.pyi` & `botocore_stubs-1.34.91/botocore-stubs/args.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/auth.pyi` & `botocore_stubs-1.34.91/botocore-stubs/auth.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/awsrequest.pyi` & `botocore_stubs-1.34.91/botocore-stubs/awsrequest.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/client.pyi` & `botocore_stubs-1.34.91/botocore-stubs/client.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/compat.pyi` & `botocore_stubs-1.34.91/botocore-stubs/compat.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/compress.pyi` & `botocore_stubs-1.34.91/botocore-stubs/compress.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/config.pyi` & `botocore_stubs-1.34.91/botocore-stubs/config.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/configprovider.pyi` & `botocore_stubs-1.34.91/botocore-stubs/configprovider.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/credentials.pyi` & `botocore_stubs-1.34.91/botocore-stubs/credentials.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/crt/auth.pyi` & `botocore_stubs-1.34.91/botocore-stubs/crt/auth.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/discovery.pyi` & `botocore_stubs-1.34.91/botocore-stubs/discovery.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/docs/bcdoc/docstringparser.pyi` & `botocore_stubs-1.34.91/botocore-stubs/docs/bcdoc/docstringparser.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/docs/bcdoc/restdoc.pyi` & `botocore_stubs-1.34.91/botocore-stubs/docs/bcdoc/restdoc.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/docs/bcdoc/style.pyi` & `botocore_stubs-1.34.91/botocore-stubs/docs/bcdoc/style.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/docs/client.pyi` & `botocore_stubs-1.34.91/botocore-stubs/docs/client.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/docs/example.pyi` & `botocore_stubs-1.34.91/botocore-stubs/docs/example.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/docs/method.pyi` & `botocore_stubs-1.34.91/botocore-stubs/docs/method.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/docs/paginator.pyi` & `botocore_stubs-1.34.91/botocore-stubs/docs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/docs/params.pyi` & `botocore_stubs-1.34.91/botocore-stubs/docs/params.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/docs/service.pyi` & `botocore_stubs-1.34.91/botocore-stubs/docs/service.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/docs/shape.pyi` & `botocore_stubs-1.34.91/botocore-stubs/docs/shape.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/docs/sharedexample.pyi` & `botocore_stubs-1.34.91/botocore-stubs/docs/sharedexample.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/docs/utils.pyi` & `botocore_stubs-1.34.91/botocore-stubs/docs/utils.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/docs/waiter.pyi` & `botocore_stubs-1.34.91/botocore-stubs/docs/waiter.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/endpoint.pyi` & `botocore_stubs-1.34.91/botocore-stubs/endpoint.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/endpoint_provider.pyi` & `botocore_stubs-1.34.91/botocore-stubs/endpoint_provider.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/errorfactory.pyi` & `botocore_stubs-1.34.91/botocore-stubs/errorfactory.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/eventstream.pyi` & `botocore_stubs-1.34.91/botocore-stubs/eventstream.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/exceptions.pyi` & `botocore_stubs-1.34.91/botocore-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/handlers.pyi` & `botocore_stubs-1.34.91/botocore-stubs/handlers.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/history.pyi` & `botocore_stubs-1.34.91/botocore-stubs/history.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/hooks.pyi` & `botocore_stubs-1.34.91/botocore-stubs/hooks.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/httpchecksum.pyi` & `botocore_stubs-1.34.91/botocore-stubs/httpchecksum.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/httpsession.pyi` & `botocore_stubs-1.34.91/botocore-stubs/httpsession.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/loaders.pyi` & `botocore_stubs-1.34.91/botocore-stubs/loaders.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/model.pyi` & `botocore_stubs-1.34.91/botocore-stubs/model.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/monitoring.pyi` & `botocore_stubs-1.34.91/botocore-stubs/monitoring.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/paginate.pyi` & `botocore_stubs-1.34.91/botocore-stubs/paginate.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/parsers.pyi` & `botocore_stubs-1.34.91/botocore-stubs/parsers.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/regions.pyi` & `botocore_stubs-1.34.91/botocore-stubs/regions.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/response.pyi` & `botocore_stubs-1.34.91/botocore-stubs/response.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/retries/adaptive.pyi` & `botocore_stubs-1.34.91/botocore-stubs/retries/adaptive.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/retries/bucket.pyi` & `botocore_stubs-1.34.91/botocore-stubs/retries/bucket.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/retries/standard.pyi` & `botocore_stubs-1.34.91/botocore-stubs/retries/standard.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/retryhandler.pyi` & `botocore_stubs-1.34.91/botocore-stubs/retryhandler.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/serialize.pyi` & `botocore_stubs-1.34.91/botocore-stubs/serialize.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/session.pyi` & `botocore_stubs-1.34.91/botocore-stubs/session.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/signers.pyi` & `botocore_stubs-1.34.91/botocore-stubs/signers.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/stub.pyi` & `botocore_stubs-1.34.91/botocore-stubs/stub.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/tokens.pyi` & `botocore_stubs-1.34.91/botocore-stubs/tokens.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/useragent.pyi` & `botocore_stubs-1.34.91/botocore-stubs/useragent.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/utils.pyi` & `botocore_stubs-1.34.91/botocore-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/validate.pyi` & `botocore_stubs-1.34.91/botocore-stubs/validate.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/botocore-stubs/waiter.pyi` & `botocore_stubs-1.34.91/botocore-stubs/waiter.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.34.90/pyproject.toml` & `botocore_stubs-1.34.91/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [tool.isort]
 profile = "black"
 line_length = 100
 src_paths = []
 
 [tool.poetry]
 name = "botocore-stubs"
-version = "1.34.90"
+version = "1.34.91"
 description = "Type annotations and code completion for botocore"
 authors = ["Vlad Emelianov <vlad.emelianov.nz@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://youtype.github.io/mypy_boto3_builder/"
 repository = "https://github.com/youtype/botocore-stubs"
 documentation = "https://youtype.github.io/mypy_boto3_builder/"
```

### Comparing `botocore_stubs-1.34.90/PKG-INFO` & `botocore_stubs-1.34.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-stubs
-Version: 1.34.90
+Version: 1.34.91
 Summary: Type annotations and code completion for botocore
 Home-page: https://youtype.github.io/mypy_boto3_builder/
 License: MIT
 Keywords: botocore,type-annotations,pyright,mypy,boto3
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 Requires-Python: >=3.8,<4.0
```

