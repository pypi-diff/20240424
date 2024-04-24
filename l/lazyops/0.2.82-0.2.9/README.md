# Comparing `tmp/lazyops-0.2.82.tar.gz` & `tmp/lazyops-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyops-0.2.82.tar", last modified: Wed Apr 24 04:03:16 2024, max compression
+gzip compressed data, was "lazyops-0.2.9.tar", last modified: Sat Jan  7 04:38:33 2023, max compression
```

## Comparing `lazyops-0.2.82.tar` & `lazyops-0.2.9.tar`

### file list

```diff
@@ -1,429 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.287012 lazyops-0.2.82/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-24 04:03:11.000000 lazyops-0.2.82/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-24 04:03:11.000000 lazyops-0.2.82/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-24 04:03:16.287012 lazyops-0.2.82/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-24 04:03:11.000000 lazyops-0.2.82/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.227012 lazyops-0.2.82/lazyops/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.227012 lazyops-0.2.82/lazyops/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7789 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/configs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/configs/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/configs/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/configs/k8s.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.231012 lazyops-0.2.82/lazyops/imports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/imports/_aiofiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/imports/_aiohttpx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/imports/_aiokeydb.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/imports/_aiosqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/imports/_backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/imports/_bs4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/imports/_dateparser.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/imports/_fileio.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/imports/_filemagic.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/imports/_gspread.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/imports/_k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/imports/_niquests.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/imports/_psutil.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/imports/_pycryptodome.py
--rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/imports/_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/imports/_slacksdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/imports/_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/imports/_torch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/imports/_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/imports/_xxhash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.231012 lazyops-0.2.82/lazyops/libs/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.231012 lazyops-0.2.82/lazyops/libs/abcs/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.231012 lazyops-0.2.82/lazyops/libs/abcs/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16772 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/cli/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/cli/default_build_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/cli/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.235012 lazyops-0.2.82/lazyops/libs/abcs/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13010 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/clients/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/clients/browser.py
--rw-r--r--   0 runner    (1001) docker     (127)    29977 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/clients/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/clients/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/clients/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.235012 lazyops-0.2.82/lazyops/libs/abcs/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/configs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    24297 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/configs/ctx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/configs/lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/configs/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.235012 lazyops-0.2.82/lazyops/libs/abcs/sql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.235012 lazyops-0.2.82/lazyops/libs/abcs/sql/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/sql/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27855 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/sql/database/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/sql/database/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    28846 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/sql/database/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/sql/database/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.235012 lazyops-0.2.82/lazyops/libs/abcs/sql/types/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/sql/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/sql/types/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.235012 lazyops-0.2.82/lazyops/libs/abcs/state/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15413 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/state/global_ctx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/state/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/state/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.235012 lazyops-0.2.82/lazyops/libs/abcs/types/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15519 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/types/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/types/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/types/networks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.239012 lazyops-0.2.82/lazyops/libs/abcs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/utils/envvars.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/abcs/utils/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.239012 lazyops-0.2.82/lazyops/libs/aiosqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/aiosqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/aiosqlite/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/aiosqlite/v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.239012 lazyops-0.2.82/lazyops/libs/api_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/api_utils/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/api_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/api_utils/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/api_utils/nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.239012 lazyops-0.2.82/lazyops/libs/asyncz/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/asyncz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/asyncz/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/asyncz/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/asyncz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.239012 lazyops-0.2.82/lazyops/libs/authzero/
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.239012 lazyops-0.2.82/lazyops/libs/authzero/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15145 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/clients/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/clients/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    17306 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/clients/oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.239012 lazyops-0.2.82/lazyops/libs/authzero/configs/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22808 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/configs/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.243012 lazyops-0.2.82/lazyops/libs/authzero/flows/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8690 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/flows/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/flows/api_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/flows/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/flows/user_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/flows/user_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.243012 lazyops-0.2.82/lazyops/libs/authzero/types/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/types/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/types/claims.py
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/types/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/types/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    38983 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/types/current_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/types/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7181 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/types/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/types/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/types/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/types/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/types/user_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/types/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/types/user_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.243012 lazyops-0.2.82/lazyops/libs/authzero/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/utils/decoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/authzero/utils/lazy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.247012 lazyops-0.2.82/lazyops/libs/compress/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/compress/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/compress/gz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/compress/lz.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/compress/zb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/compress/ztd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.247012 lazyops-0.2.82/lazyops/libs/convertio/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/convertio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23544 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/convertio/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.247012 lazyops-0.2.82/lazyops/libs/convertio/docx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/convertio/docx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.247012 lazyops-0.2.82/lazyops/libs/convertio/pdf/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/convertio/pdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/convertio/pdf/pdftotext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.247012 lazyops-0.2.82/lazyops/libs/db_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/db_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28743 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/db_utils/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/db_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.247012 lazyops-0.2.82/lazyops/libs/dbinit/
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/dbinit/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/dbinit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/dbinit/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/dbinit/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.247012 lazyops-0.2.82/lazyops/libs/dbinit/data_structures/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/dbinit/data_structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/dbinit/data_structures/grant_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/dbinit/data_structures/grant_to.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/dbinit/data_structures/privileges.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.251012 lazyops-0.2.82/lazyops/libs/dbinit/entities/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/dbinit/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/dbinit/entities/cluster_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/dbinit/entities/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/dbinit/entities/database_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/dbinit/entities/database_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/dbinit/entities/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     9241 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/dbinit/entities/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/dbinit/entities/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/dbinit/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.251012 lazyops-0.2.82/lazyops/libs/dbinit/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/dbinit/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/dbinit/mixins/grantable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/dbinit/mixins/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/dbinit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.251012 lazyops-0.2.82/lazyops/libs/fastapi_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/fastapi_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.251012 lazyops-0.2.82/lazyops/libs/fastapi_utils/configs/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/fastapi_utils/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10680 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/fastapi_utils/configs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/fastapi_utils/configs/workers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.251012 lazyops-0.2.82/lazyops/libs/fastapi_utils/openapi/
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/fastapi_utils/openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22178 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/fastapi_utils/openapi/spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.251012 lazyops-0.2.82/lazyops/libs/fastapi_utils/openapi/stoplight/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/fastapi_utils/openapi/stoplight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/fastapi_utils/openapi/stoplight/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.251012 lazyops-0.2.82/lazyops/libs/fastapi_utils/processes/
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/fastapi_utils/processes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21522 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/fastapi_utils/processes/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/fastapi_utils/processes/workers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.255012 lazyops-0.2.82/lazyops/libs/fastapi_utils/state/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/fastapi_utils/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/fastapi_utils/state/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/fastapi_utils/state/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.255012 lazyops-0.2.82/lazyops/libs/fastapi_utils/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/fastapi_utils/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/fastapi_utils/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.255012 lazyops-0.2.82/lazyops/libs/fastapi_utils/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/fastapi_utils/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6958 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/fastapi_utils/types/persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/fastapi_utils/types/state.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/fastapi_utils/types/user_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.255012 lazyops-0.2.82/lazyops/libs/fastapi_utils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/fastapi_utils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/fastapi_utils/utils/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.255012 lazyops-0.2.82/lazyops/libs/googlesearch/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/googlesearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19494 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/googlesearch/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    36068 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/googlesearch/user_agents.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/googlesearch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.255012 lazyops-0.2.82/lazyops/libs/gsheets/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/gsheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16676 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/gsheets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/gsheets/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.259012 lazyops-0.2.82/lazyops/libs/kops/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/kops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/kops/_kopf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/kops/atypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/kops/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    48491 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/kops/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/kops/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/kops/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/kops/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.259012 lazyops-0.2.82/lazyops/libs/kz/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/kz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/kz/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9153 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/kz/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/kz/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.259012 lazyops-0.2.82/lazyops/libs/lazyload/
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/lazyload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/lazyload/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/lazyload/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.259012 lazyops-0.2.82/lazyops/libs/logging/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36330 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/logging/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.259012 lazyops-0.2.82/lazyops/libs/orm_sql/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/orm_sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28800 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/orm_sql/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/orm_sql/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/orm_sql/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.259012 lazyops-0.2.82/lazyops/libs/persistence/
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28229 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/persistence/addons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.259012 lazyops-0.2.82/lazyops/libs/persistence/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/persistence/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26731 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/persistence/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/persistence/backends/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    25510 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/persistence/backends/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.263012 lazyops-0.2.82/lazyops/libs/persistence/compression/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/persistence/compression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/persistence/compression/_gzip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/persistence/compression/_lz4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/persistence/compression/_lzma.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/persistence/compression/_zlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/persistence/compression/_zstd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/persistence/compression/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/persistence/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    40223 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/persistence/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.263012 lazyops-0.2.82/lazyops/libs/persistence/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/persistence/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/persistence/serializers/_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/persistence/serializers/_msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/persistence/serializers/_pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7882 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/persistence/serializers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.263012 lazyops-0.2.82/lazyops/libs/pooler/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/pooler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17514 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/pooler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/pooler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.263012 lazyops-0.2.82/lazyops/libs/posthog/
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/posthog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21385 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/posthog/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/posthog/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/posthog/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/posthog/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.263012 lazyops-0.2.82/lazyops/libs/proxyobj/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/proxyobj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/proxyobj/extra.py
--rw-r--r--   0 runner    (1001) docker     (127)    16912 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/proxyobj/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/proxyobj/wraps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.267012 lazyops-0.2.82/lazyops/libs/psqldb/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/psqldb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36491 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/psqldb/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    63824 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/psqldb/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    18769 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/psqldb/models_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/psqldb/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/psqldb/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/psqldb/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/psqldb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.267012 lazyops-0.2.82/lazyops/libs/slack/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19125 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/slack/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/slack/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/slack/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.267012 lazyops-0.2.82/lazyops/libs/sqlcache/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/sqlcache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15917 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/sqlcache/backends.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/sqlcache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/sqlcache/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/sqlcache/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/sqlcache/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14747 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/sqlcache/mediums.py
--rw-r--r--   0 runner    (1001) docker     (127)    84429 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/sqlcache/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/sqlcache/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.271012 lazyops-0.2.82/lazyops/libs/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26908 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/sqlite/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    33962 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/sqlite/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/sqlite/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/sqlite/static.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/sqlite/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.271012 lazyops-0.2.82/lazyops/libs/sysmon/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/sysmon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/libs/sysmon/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.271012 lazyops-0.2.82/lazyops/types/
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44233 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/types/classprops.py
--rw-r--r--   0 runner    (1001) docker     (127)    18293 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/types/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/types/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/types/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/types/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/types/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/types/lazydict.py
--rw-r--r--   0 runner    (1001) docker     (127)    15810 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/types/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11682 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/types/models_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    14293 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/types/models_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/types/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/types/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.275012 lazyops-0.2.82/lazyops/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/utils/ahelpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11544 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/utils/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/utils/dates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.275012 lazyops-0.2.82/lazyops/utils/debugging/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/utils/debugging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/utils/debugging/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    21745 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/utils/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/utils/filestream.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/utils/format_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18131 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/utils/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/utils/lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13858 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/utils/lazylib.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/utils/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/utils/pooler.py
--rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (127)    19759 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/utils/times.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.279012 lazyops-0.2.82/lazyops/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/envs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.279012 lazyops-0.2.82/lazyops/v1/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/experimental/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/experimental/gptj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.279012 lazyops-0.2.82/lazyops/v1/lazyclasses/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyclasses/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyclasses/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyclasses/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyclasses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.279012 lazyops-0.2.82/lazyops/v1/lazyconfig/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyconfig/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyconfig/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18769 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyconfig/nginx.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyconfig/tfserving.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyconfig/tfserving_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    33862 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyconfig/tfserving_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.279012 lazyops-0.2.82/lazyops/v1/lazydatabase/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazydatabase/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazydatabase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazydatabase/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazydatabase/backends.py
--rw-r--r--   0 runner    (1001) docker     (127)    18309 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazydatabase/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazydatabase/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazydatabase/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.283012 lazyops-0.2.82/lazyops/v1/lazyio/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyio/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyio/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyio/async_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    24015 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyio/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.283012 lazyops-0.2.82/lazyops/v1/lazyrpc/
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyrpc/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyrpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyrpc/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    30860 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyrpc/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyrpc/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyrpc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazyrpc/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.283012 lazyops-0.2.82/lazyops/v1/lazysources/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazysources/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazysources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.283012 lazyops-0.2.82/lazyops/v1/lazysources/gdelt/
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazysources/gdelt/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazysources/gdelt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazysources/gdelt/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazysources/gdelt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazysources/gdelt/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/lazysources/gdelt/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/mp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/mp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/v1/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-24 04:03:11.000000 lazyops-0.2.82/lazyops/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.287012 lazyops-0.2.82/lazyops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-24 04:03:16.000000 lazyops-0.2.82/lazyops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11766 2024-04-24 04:03:16.000000 lazyops-0.2.82/lazyops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 04:03:16.000000 lazyops-0.2.82/lazyops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-24 04:03:16.000000 lazyops-0.2.82/lazyops.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-24 04:03:16.000000 lazyops-0.2.82/lazyops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 04:03:16.000000 lazyops-0.2.82/lazyops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 04:03:16.287012 lazyops-0.2.82/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-24 04:03:11.000000 lazyops-0.2.82/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:03:16.283012 lazyops-0.2.82/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-24 04:03:11.000000 lazyops-0.2.82/tests/test_failafter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14004 2024-04-24 04:03:11.000000 lazyops-0.2.82/tests/test_persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-24 04:03:11.000000 lazyops-0.2.82/tests/test_pgsql.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-24 04:03:11.000000 lazyops-0.2.82/tests/test_strenums.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-04-24 04:03:11.000000 lazyops-0.2.82/tests/test_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.436811 lazyops-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-07 04:38:23.000000 lazyops-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-07 04:38:23.000000 lazyops-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-01-07 04:38:33.436811 lazyops-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-01-07 04:38:23.000000 lazyops-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.424811 lazyops-0.2.9/lazyops/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.428810 lazyops-0.2.9/lazyops/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/configs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/configs/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/configs/k8s.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.428810 lazyops-0.2.9/lazyops/imports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/imports/_aiohttpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/imports/_aiokeydb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/imports/_fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/imports/_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/imports/_psutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/imports/_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/imports/_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.428810 lazyops-0.2.9/lazyops/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40893 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/types/classprops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/types/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/types/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/types/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.428810 lazyops-0.2.9/lazyops/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/utils/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/utils/lazylib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/utils/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/utils/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.432811 lazyops-0.2.9/lazyops/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/envs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.432811 lazyops-0.2.9/lazyops/v1/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/experimental/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/experimental/gptj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.432811 lazyops-0.2.9/lazyops/v1/lazyclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyclasses/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyclasses/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyclasses/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyclasses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.432811 lazyops-0.2.9/lazyops/v1/lazyconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyconfig/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyconfig/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18769 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyconfig/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyconfig/tfserving.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyconfig/tfserving_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33862 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyconfig/tfserving_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.432811 lazyops-0.2.9/lazyops/v1/lazydatabase/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazydatabase/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazydatabase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazydatabase/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazydatabase/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18309 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazydatabase/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazydatabase/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazydatabase/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.432811 lazyops-0.2.9/lazyops/v1/lazyio/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyio/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyio/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyio/async_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24015 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyio/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.436811 lazyops-0.2.9/lazyops/v1/lazyrpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyrpc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyrpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyrpc/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30860 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyrpc/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyrpc/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyrpc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyrpc/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.436811 lazyops-0.2.9/lazyops/v1/lazysources/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazysources/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazysources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.436811 lazyops-0.2.9/lazyops/v1/lazysources/gdelt/
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazysources/gdelt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazysources/gdelt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazysources/gdelt/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazysources/gdelt/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazysources/gdelt/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazysources/gdelt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/mp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.424811 lazyops-0.2.9/lazyops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-01-07 04:38:33.000000 lazyops-0.2.9/lazyops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-01-07 04:38:33.000000 lazyops-0.2.9/lazyops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-07 04:38:33.000000 lazyops-0.2.9/lazyops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-07 04:38:33.000000 lazyops-0.2.9/lazyops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-07 04:38:33.000000 lazyops-0.2.9/lazyops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-07 04:38:33.436811 lazyops-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-01-07 04:38:23.000000 lazyops-0.2.9/setup.py
```

### Comparing `lazyops-0.2.82/LICENSE` & `lazyops-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/README.md` & `lazyops-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/configs/base.py` & `lazyops-0.2.9/lazyops/configs/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import absolute_import
 
 """
 Base Configs
 """
 import pathlib
 import contextlib
-from typing import Optional, Union, Dict, TYPE_CHECKING
+from typing import Optional, Union, TYPE_CHECKING
 from lazyops.types.models import BaseSettings
 from lazyops.types.classprops import lazyproperty
 
 from lazyops.imports._fileio import (
     File, 
     FileLike, 
     _fileio_available, 
@@ -20,15 +20,14 @@
     resolve_aiokeydb,
     _aiokeydb_available, 
 )
 
 if TYPE_CHECKING:
     from lazyops.configs.cloud import BotoSettings, AwsSettings, GcpSettings, MinioSettings
     from lazyops.configs.k8s import K8sSettings
-    from lazyops.configs.client import ClientSettings
 
 
 class DefaultSettings(BaseSettings):
 
     ## General Variables
     api_host: Optional[str] = None
     api_port: Optional[int] = None
@@ -139,26 +138,25 @@
     @lazyproperty
     def torch_device_name(self):
         from lazyops.utils.system import get_torch_device_name
         return get_torch_device_name()
     
     @lazyproperty
     def in_colab(self) -> bool:
-        with contextlib.suppress(Exception):
-            from importlib import import_module
-            import_module('google.colab')
+        with contextlib.suppress(ImportError):
+            import google.colab
             return True
         return False
     
     @lazyproperty
     def in_container(self) -> bool:
         return any(
-            [self.in_docker,
+            self.in_docker,
             self.in_app,
-            self.gpg_key is not None,]
+            self.gpg_key is not None,
         )
 
     @lazyproperty
     def in_k8s(self) -> bool:
         return self.k8s.in_cluster
     
     @lazyproperty
@@ -167,15 +165,15 @@
     
     @lazyproperty
     def in_app(self) -> bool:
         return (self.app_host is not None and self.app_port is not None) or (self.app_home and self.app_home == '/app')
     
     @lazyproperty
     def is_local(self) -> bool:
-        return not any([self.in_k8s, self.in_k8s, self.in_api, self.in_docker])
+        return not any(self.in_k8s, self.in_k8s, self.in_api, self.in_docker)
     
     @lazyproperty
     def is_remote(self) -> bool:
         return self.in_k8s or self.in_api or self.in_docker or self.in_container
     
     """
     Huggingface Variables
@@ -243,36 +241,8 @@
         return K8sSettings()
     
     @lazyproperty
     def keydb(self) -> 'aiokeydb.KeyDBSettings':
         if not _aiokeydb_available:
             resolve_aiokeydb()
         return aiokeydb.KeyDBClient.get_settings()
-    
-    @lazyproperty
-    def client(self) -> 'ClientSettings':
-        from lazyops.configs.client import ClientSettings
-        return ClientSettings()
-    
-    """
-    Client Props / Methods
-    """
-
-    def get_client_headers(self) -> Dict[str, str]:
-        return self.client.get_headers()
-
-    @property
-    def default_client_name(self):
-        """
-        Returns the default API client name
-        """
-        if self.in_k8s: return 'cluster'
-        return 'local' if self.client.api_dev_mode else 'external'
-
-    @lazyproperty
-    def client_endpoint(self) -> str:
-        """
-        Returns the client endpoint
-        """
-        return self.client.endpoints[self.default_client_name] or self.client.endpoints['local']
-
```

### Comparing `lazyops-0.2.82/lazyops/configs/cloud.py` & `lazyops-0.2.9/lazyops/configs/cloud.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/configs/k8s.py` & `lazyops-0.2.9/lazyops/configs/k8s.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/imports/_aiohttpx.py` & `lazyops-0.2.9/lazyops/imports/_aiohttpx.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     Ensures that `aiohttpx` is available
     """
     global aiohttpx, _aiohttpx_available
     if not _aiohttpx_available:
         resolve_missing('aiohttpx', required = required)
         import aiohttpx
         _aiohttpx_available = True
-        globals()['aiohttpx'] = aiohttpx
 
 
 def require_aiohttpx(
     required: bool = False,
 ):
     """
     Wrapper for `resolve_aiohttpx` that can be used as a decorator
```

### Comparing `lazyops-0.2.82/lazyops/imports/_aiokeydb.py` & `lazyops-0.2.9/lazyops/imports/_aiokeydb.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     Ensures that `aiokeydb` is available
     """
     global aiokeydb, _aiokeydb_available
     if not _aiokeydb_available:
         resolve_missing(f'aiokeydb=={version}', required = required)
         import aiokeydb
         _aiokeydb_available = True
-        globals()['aiokeydb'] = aiokeydb
 
 
 def require_aiokeydb(
     required: bool = False,
     version: str = _min_version,
 ):
     """
```

### Comparing `lazyops-0.2.82/lazyops/imports/_dateparser.py` & `lazyops-0.2.9/lazyops/imports/_psutil.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 
 """
-Import Handler for dateparser and pytz
+Import Handler for `psutil`
 """
 
+from lazyops.utils.imports import resolve_missing, require_missing_wrapper
 
 try:
-    import dateparser
-    import pytz
-    _dateparser_available = True
+    import psutil
+    _psutil_available = True
 except ImportError:
-    dateparser = object
-    pytz = object
-    _dateparser_available = False
+    psutil = object
+    _psutil_available = False
 
-def resolve_dateparser(
+def resolve_psutil(
     required: bool = False,
 ):
     """
-    Ensures that `dateparser` is available
+    Ensures that `psutil` is available
     """
-    global dateparser, pytz, _dateparser_available
-    if not _dateparser_available:
-        from lazyops.utils.imports import resolve_missing
-        resolve_missing('dateparser', required = required)
-        import dateparser
-        import pytz
-        _dateparser_available = True
-        globals()['dateparser'] = dateparser
-        globals()['pytz'] = pytz
+    global psutil, _psutil_available
+    if not _psutil_available:
+        resolve_missing('psutil', required = required)
+        import psutil
+        _psutil_available = True
 
 
-def require_dateparser(
+def require_psutil(
     required: bool = False,
 ):
     """
-    Wrapper for `resolve_dateparser` that can be used as a decorator
+    Wrapper for `resolve_psutil` that can be used as a decorator
     """
     def decorator(func):
-        from lazyops.utils.imports import require_missing_wrapper
         return require_missing_wrapper(
-            resolver = resolve_dateparser, 
+            resolver = resolve_psutil, 
             func = func, 
             required = required
         )
     return decorator
```

### Comparing `lazyops-0.2.82/lazyops/imports/_fileio.py` & `lazyops-0.2.9/lazyops/imports/_fileio.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,18 +18,17 @@
     required: bool = False,
 ):
     """
     Ensures that `fileio` is available
     """
     global fileio, _fileio_available
     if not _fileio_available:
-        resolve_missing('fileio', 'file-io', required = required)
+        resolve_missing('fileio', required = required)
         import fileio
         _fileio_available = True
-        globals()['fileio'] = fileio
 
 
 def require_fileio(
     required: bool = False,
 ):
     """
     Wrapper for `resolve_fileio` that can be used as a decorator
```

### Comparing `lazyops-0.2.82/lazyops/imports/_k8s.py` & `lazyops-0.2.9/lazyops/imports/_k8s.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,23 +54,16 @@
     import kopf
     _kopf_available = True
 
 except ImportError:
     kopf = object
     _kopf_available = False
 
-try:
-    import aiocache
-    _aiocache_available = True
 
-except ImportError:
-    aiocache = object
-    _aiocache_available = False
-
-from lazyops.utils.imports import resolve_missing, require_missing_wrapper
+from gexai.libs.imports.base import resolve_missing, require_missing_wrapper
 
 def resolve_sync_k8s(
     required: bool = True,
 ):
     """
     Ensures that `kubernetes` is availableable
     """
@@ -93,70 +86,53 @@
     required: bool = True,
 ):
     """
     Ensures that `kubernetes_asyncio` is availableable
     """
     global _async_k8_available
     global AsyncClient, AsyncConfig, AsyncStream, AsyncWatch, AsyncUtils, AsyncType, AsyncWSClient
-    
     if not _async_k8_available:
         resolve_missing('kubernetes_asyncio', required = required)
         import kubernetes_asyncio.client as AsyncClient
         import kubernetes_asyncio.config as AsyncConfig
         import kubernetes_asyncio.stream as AsyncStream
         import kubernetes_asyncio.watch as AsyncWatch
         import kubernetes_asyncio.utils as AsyncUtils
         import kubernetes_asyncio.client.models as AsyncType
         AsyncWSClient = AsyncStream.WsApiClient
-        _async_k8_available = True
 
-def resolve_aiocache(
-    required: bool = True,
-):
-    """
-    Ensures that `aiocache` is availableable
-    """
-    global _aiocache_available
-    global aiocache
-
-    if not _aiocache_available:
-        resolve_missing('aiocache', required = required)
-        import aiocache
-        _aiocache_available = True
-        globals()['aiocache'] = aiocache
+        _async_k8_available = True
 
 def resolve_kopf(
     required: bool = True,
 ):
     """
     Ensures that `kopf`
     """
     global _kopf_available
     global kopf
 
     if not _kopf_available:
         resolve_missing('kopf', required = required)
         import kopf
         _kopf_available = True
-        globals()['kopf'] = kopf
 
 def resolve_k8s(
     is_sync: bool = False,
     is_async: bool = True,
     is_operator: bool = False,
     required: bool = True,
 ):
     """
     Ensures that `kubernetes`, `kubernetes_asyncio`, `kopf` are availableable
     """
     if is_operator:
         resolve_kopf(required = required)
     if is_async:
         resolve_async_k8s(required = required)
-        resolve_aiocache(required = required)
     if is_sync or not is_async:
         resolve_sync_k8s(required = required)
 
 
 def require_k8s(
     is_sync: bool = False,
     is_async: bool = True,
```

### Comparing `lazyops-0.2.82/lazyops/imports/_torch.py` & `lazyops-0.2.9/lazyops/imports/_torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,14 @@
             elif is_win:
                 pkg += '+cpu'
             
         pkg += ' --extra-index-url https://download.pytorch.org/whl/torch'
         resolve_missing_custom(pkg, required = required)
         import torch
         _torch_available = True
-        globals()['torch'] = torch
 
 
 def require_torch(
     required: bool = False,
     version: typing.Optional[str] = None,
     cuda: typing.Union[str, bool] = False,
     rocm: typing.Optional[str] = None,
```

### Comparing `lazyops-0.2.82/lazyops/imports/_transformers.py` & `lazyops-0.2.9/lazyops/imports/_transformers.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     if not _transformers_available:
         pkg = 'transformers'
         if version is not None:
             pkg += f'=={version}'
         resolve_missing(pkg, required = required)
         import transformers
         _transformers_available = True
-        globals()['transformers'] = transformers
 
 
 def require_transformers(
     required: bool = False,
     version: str = None,
 ):
     """
```

### Comparing `lazyops-0.2.82/lazyops/libs/fastapi_utils/types/persistence.py` & `lazyops-0.2.9/lazyops/v1/lazyconfig/tfserving_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,236 +1,173 @@
-from __future__ import annotations
+import requests
+import aiohttp
+import simdjson as json
+from lazyops.utils import timed_cache
+from lazyops.serializers import async_cache
+
+from ._base import lazyclass, dataclass, List, Union, Any, Dict
+from .tfserving_pb2 import TFSModelConfig, TFSConfig
+
+jparser = json.Parser()
+
+
+@lazyclass
+@dataclass
+class TFSRequest:
+    data: Any
+
+    def to_data(self):
+        if isinstance(self.data, str):
+            return {'inputs': [self.data]}
+        if isinstance(self.data, list):
+            return {'inputs': self.data}
+        if isinstance(self.data, dict):
+            if self.data.get('inputs'):
+                return self.data
+            if self.data.get('text'):
+                if isinstance(self.data['text'], str):
+                    return {'inputs': [self.data['text']]}
+                return {'inputs': self.data['text']}
+        return {'inputs': self.data}
 
-import os
-import abc
-import atexit
-import tempfile
-import pathlib
-import filelock
-import contextlib
-from lazyops.utils.serialization import Json
-from typing import Optional, Dict, Any, Set, List, Union, Generator, TYPE_CHECKING
 
-
-
-class TemporaryData(abc.ABC):
-    """
-    Temporary Data that deletes itself on exit
-    """
+class TFSModelEndpoint(object):
     def __init__(
         self, 
-        filepath: Optional[pathlib.Path] = None,
-        is_multithreaded: Optional[bool] = False,
-        timeout: Optional[int] = 10,
-    ):
-        if not filepath: filepath = pathlib.Path(tempfile.mktemp())
-        self.filepath = pathlib.Path(filepath)
-        self.filepath.parent.mkdir(parents = True, exist_ok = True)
-        self.filelock_path = filepath.with_suffix('.lock')
-        self.timeout = timeout
-        self.is_multithreaded = is_multithreaded
-        self._filelock: Optional[filelock.SoftFileLock] = None
+        url: str,
+        config: TFSModelConfig,
+        ver: str = 'v1',
+        sess: requests.Session = requests.Session(),
+        headers: Dict[str, Any] = {},
+        ):
+        self.url = url
+        self.config = config
+        self.ver = ver
+        self.sess = sess
+        self.headers = headers
+        self.validate_endpoints()
+    
 
     @property
-    def filelock(self) -> filelock.SoftFileLock:
-        """
-        Returns the filelock
-        """
-        if self._filelock is None:
-            try:
-                self._filelock = filelock.SoftFileLock(
-                    self.filelock_path.as_posix(), 
-                    timeout = self.timeout,
-                    thread_local = False
-                )
-                with self._filelock.acquire():
-                    if not self.filepath.exists():
-                        self.filepath.write_text('{}')
-                    data = Json.loads(self.filepath.read_text())
-                    if self.is_multithreaded and not data.get('process_id'):
-                        data['process_id'] = os.getpid()
-                        self.filepath.write_text(Json.dumps(data, indent = 2))
-                atexit.register(self.cleanup_on_exit)
-            except Exception as e:
-                from lazyops.libs.logging import logger
-                logger.trace(f'Error creating filelock for {self.filepath}', e)
-                raise e
-        return self._filelock
-    
-    def _load_data(self) -> Dict[str, Any]:
-        """
-        Loads the data
-        """
-        if not self.filepath.exists():
-            self.filepath.write_text('{}')
-        return Json.loads(self.filepath.read_text())
-
+    def default_endpoint(self):
+        return f'{self.url}/{self.ver}/models/{self.config.name}'
+    
     @property
-    def data(self) -> Dict[str, Any]:
-        """
-        Returns the data
-        """
-        try:
-            with self.filelock.acquire():
-                return self._load_data()
-        except filelock.Timeout as e:
-            from lazyops.libs.logging import logger
-            logger.trace(f'Filelock timeout for {self.filepath}')
-            raise e
-        
-    @contextlib.contextmanager
-    def ctx(self) -> Generator[Dict[str, Union[List[Any], Dict[str, Any], Any]], None, None]:
-        """
-        Returns the context
-        """
-        try:
-            with self.filelock.acquire():
-                data = self._load_data()
-                try:
-                    yield data
-                finally:
-                    self.filepath.write_text(Json.dumps(data, indent = 2))
-        except filelock.Timeout as e:
-            from lazyops.libs.logging import logger
-            logger.trace(f'Filelock timeout for {self.filepath}')
-            raise e
-    
-    def get(self, key: str, default: Optional[Any] = None) -> Any:
-        """
-        Returns the value for the given key
-        """
-        return self.data.get(key, default)
-    
-    def __contains__(self, key: str) -> bool:
-        """
-        Returns whether the key is in the data
-        """
-        return key in self.data
-    
-    def __getitem__(self, key: str) -> Any:
-        """
-        Returns the value for the given key
-        """
-        return self.data.get(key)
-    
-    def __setitem__(self, key: str, value: Any):
-        """
-        Sets the value for the given key
-        """
-        with self.ctx() as data:
-            data[key] = value
-
-    def __delitem__(self, key: str):
-        """
-        Deletes the value for the given key
-        """
-        with self.ctx() as data:
-            del data[key]
-
-
-    def __iter__(self):
-        """
-        Returns the iterator
-        """
-        return iter(self.data)
-    
-    def __len__(self) -> int:
-        """
-        Returns the length
-        """
-        return len(self.data)
-    
-    def __repr__(self) -> str:
-        """
-        Returns the representation
-        """
-        return repr(self.data)
-    
-    def __str__(self) -> str:
-        """
-        Returns the string representation
-        """
-        return str(self.data)
-    
-    def __bool__(self) -> bool:
-        """
-        Returns whether the data is empty
-        """
-        return bool(self.data)
-    
-    def __eq__(self, other: Any) -> bool:
-        """
-        Returns whether the data is equal to the other
-        """
-        return self.data == other
-    
-    def keys(self) -> Set[str]:
-        """
-        Returns the keys
-        """
-        return self.data.keys()
-    
-    def setdefault(self, key: str, default: Any) -> Any:
-        """
-        Sets the default value for the given key
-        """
-        with self.ctx() as data:
-            value = data.setdefault(key, default)
-        return value
-        
-    def close(self):
-        """
-        Closes the filelock
-        """
-        self.filelock.release()
-
-    def append(self, key: str, value: Any) -> bool:
-        """
-        Appends the value to the list
-        """
-        with self.ctx() as data:
-            if key not in data:
-                data[key] = []
-            if value not in data[key]:
-                data[key].append(value)
-                return False
-        return True
-
-    def cleanup_on_exit(self):
-        """
-        Cleans up on exit
-        """
-        if not self.filepath.exists() and not self.filelock_path.exists():
-            return
-        if self.is_multithreaded and self['process_id'] != os.getpid():
-            return
-        with contextlib.suppress(Exception):
-            self.close()
-            self.filepath.unlink()
-            self.filelock_path.unlink()
-
-
-    def has_logged(self, key: str) -> bool:
-        """
-        Returns whether the key has been logged
-        """
-        return self.append('logged', key)
+    def default_url(self):
+        if self.config.default_label:
+            return self.default_endpoint + f'/labels/{self.config.default_label}'
+        if self.config.default_version:
+            return self.default_endpoint + f'/versions/{self.config.default_version}'
+        return self.default_endpoint
+    
+    @property
+    def default_predict(self):
+        return self.default_url + ':predict'
+    
+    def get_label(self, label: str = 'latest'):
+        return self.default_endpoint + '/labels/' + label
+    
+    def get_version(self, ver: Union[str, int]):
+        return self.default_endpoint + '/versions/' + str(ver)
+    
+    def get_endpoint(self, label: str = None, ver: Union[str, int] = None):
+        if label:
+            return self.get_label(label)
+        if ver:
+            return self.get_version(ver)
+        return self.default_url
+    
+    def get_predict_endpoint(self, label: str = None, ver: Union[str, int] = None):
+        if label:
+            return self.get_label(label) + ':predict'
+        if ver:
+            return self.get_version(ver) + ':predict'
+        return self.default_predict
         
+    @timed_cache(seconds=600)
+    def get_metadata(self, label: str = None, ver: Union[str, int] = None):
+        ep = self.get_endpoint(label=label, ver=ver)
+        return self.sess.get(ep + '/metadata', verify=False).json()
+    
+    async def get_aio_metadata(self, label: str = None, ver: Union[str, int] = None, **kwargs):
+        epoint = self.get_endpoint(label=label, ver=ver)
+        async with aiohttp.ClientSession(headers=self.headers) as sess:
+            async with sess.get(epoint + '/metadata', verify_ssl=False, **kwargs) as resp:
+                return await resp.json()
+
+    async def aio_predict(self, data, label: str = None, ver: Union[str, int] = None, **kwargs):
+        epoint = self.get_predict_endpoint(label=label, ver=ver)
+        item = TFSRequest(data=data)
+        async with aiohttp.ClientSession(headers=self.headers) as sess:
+            async with sess.post(epoint, json=item.to_data(), verify_ssl=False, **kwargs) as resp:
+                return await resp.json()
+    
+    @timed_cache(seconds=60)
+    def predict(self, data, label: str = None, ver: Union[str, int] = None, **kwargs):
+        epoint = self.get_predict_endpoint(label=label, ver=ver)
+        item = TFSRequest(data=data)
+        res = self.sess.post(epoint, json=item.to_data(), verify=False)
+        return res.json()
+    
+    @property
+    def is_alive(self):
+        return bool(self.get_metadata().get('model_spec'))
+    
+    def validate_endpoints(self):
+        for n, version in enumerate(self.config.model_versions):
+            r = self.get_metadata(label=version.label)
+            if r.get('error'): self.config.model_versions[n].label = None
+            r = self.get_metadata(ver=str(version.step))
+            if r.get('error'): self.config.model_versions[n].step = None
+    
+
+class TFServeModel:
+    def __init__(self, url: str, configs: List[TFSModelConfig], ver: str = 'v1', **kwargs):
+        self.url = url
+        self.configs = configs
+        self.ver = ver
+        self.headers = {'Content-Type': 'application/json'}
+        if kwargs: self.headers.update(kwargs.get('headers'))
+        self.sess = requests.Session()
+        self.sess.headers.update(self.headers)
+        self.endpoints = {config.name: TFSModelEndpoint(url, config=config, ver=ver, sess=self.sess, headers=self.headers) for config in configs}
+        self.default_model = kwargs.get('default_model') or configs[0].name
+        self.available_models = [config.name for config in configs]
+        self.validate_models()
+
+
+    def predict(self, data, model: str = None, label: str = None, ver: Union[str, int] = None, **kwargs):
+        if model: assert model in self.available_models
+        model = model or self.default_model
+        return self.endpoints[model].predict(data, label=label, ver=ver, **kwargs)
+
+    async def aio_predict(self, data, model: str = None, label: str = None, ver: Union[str, int] = None, **kwargs):
+        if model: assert model in self.available_models
+        model = model or self.default_model
+        return await self.endpoints[model].aio_predict(data, label=label, ver=ver, **kwargs)
+    
+    @property
+    def api_status(self):
+        return {model: self.endpoints[model].is_alive for model in self.available_models}
+    
+    @timed_cache(seconds=600)
+    def get_api_metadata(self):
+        return {model: self.endpoints[model].get_metadata() for model in self.available_models}
+
+    @async_cache
+    async def get_aio_api_metadata(self):
+        return {model: await self.endpoints[model].get_aio_metadata() for model in self.available_models}
+    
+
     @classmethod
-    def from_module(
-        cls, 
-        module_name: str, 
-        data_dir: Optional[str] = '.data', 
-        is_multithreaded: Optional[bool] = False,
-        **kwargs
-    ) -> TemporaryData:
-        """
-        Returns a temporary data from the module
-        """
-        from lazyops.utils.assets import get_module_path
-        module_path = get_module_path(module_name)
-        module_dir = module_path.joinpath(data_dir)
-        module_dir.mkdir(parents = True, exist_ok = True)
-        filepath = module_dir.joinpath(f'{module_name}.tmp.json')
-        if not filepath.exists():
-            filepath.write_text('{}')
-        return cls(filepath = filepath, is_multithreaded = is_multithreaded, **kwargs)
+    def from_config_file(cls, url, filepath: str, ver: str = 'v1', **kwargs):
+        configs = TFSConfig.from_config_file(filepath, as_obj=True)
+        return TFServeModel(url=url, configs=configs, ver=ver, **kwargs)
+    
+    def validate_models(self):
+        for model in list(self.available_models):
+            if not self.endpoints[model].is_alive:
+                self.available_models.remove(model)
+                _ = self.endpoints.pop(model)
+        if self.default_model not in self.available_models:
+            self.default_model = self.available_models[0]
+
```

### Comparing `lazyops-0.2.82/lazyops/types/classprops.py` & `lazyops-0.2.9/lazyops/types/classprops.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import functools
 import inspect
 import textwrap
 import threading
 import types
 import warnings
-from typing import TypeVar, Type, Callable, Any, Union
 from inspect import signature
 from functools import wraps
 
 
 
 __all__ = ['classproperty', 'cached_classproperty', 'deprecated', 'deprecated_attribute',
            'deprecated_renamed_argument', 'format_doc',
@@ -548,18 +547,14 @@
     return decorator
 
 
 
 # TODO: This can still be made to work for setters by implementing an
 # accompanying metaclass that supports it; we just don't need that right this
 # second
-
-CP = TypeVar('CP', bound='classproperty')
-CPR = TypeVar('CPR')
-
 class classproperty(property):
     """
     Similar to `property`, but allows class-level properties.  That is,
     a property whose getter is like a `classmethod`.
 
     The wrapped method may explicitly use the `classmethod` decorator (which
     must become before this decorator), or the `classmethod` may be omitted
@@ -650,26 +645,26 @@
         >>> FooSub.bar
         Performing complicated calculation
         1
         >>> FooSub.bar
         1
     """
 
-    def __new__(cls: CP, fget=None, doc=None, lazy=False) -> Union[Callable, CP]:
+    def __new__(cls, fget=None, doc=None, lazy=False):
         if fget is None:
             # Being used as a decorator--return a wrapper that implements
             # decorator syntax
             def wrapper(func):
                 return cls(func, lazy=lazy)
 
             return wrapper
 
         return super().__new__(cls)
 
-    def __init__(self, fget, doc=None, lazy=False) -> None:
+    def __init__(self, fget, doc=None, lazy=False):
         self._lazy = lazy
         if lazy:
             self._lock = threading.RLock()   # Protects _cache
             self._cache = {}
         fget = self._wrap_fget(fget)
 
         super().__init__(fget=fget, doc=doc)
@@ -678,15 +673,15 @@
         # get set properly on instances of property subclasses if
         # the doc argument was used rather than taking the docstring
         # from fget
         # Related Python issue: https://bugs.python.org/issue24766
         if doc is not None:
             self.__doc__ = doc
 
-    def __get__(self, obj: Any, objtype: Type[CP]) -> CPR:
+    def __get__(self, obj, objtype):
         if self._lazy:
             val = self._cache.get(objtype, _NotFound)
             if val is _NotFound:
                 with self._lock:
                     # Check if another thread initialised before we locked.
                     val = self._cache.get(objtype, _NotFound)
                     if val is _NotFound:
@@ -695,15 +690,15 @@
         else:
             # The base property.__get__ will just return self here;
             # instead we pass objtype through to the original wrapped
             # function (which takes the class as its sole argument)
             val = self.fget.__wrapped__(objtype)
         return val
 
-    def getter(self, fget: Callable[[Any], Any]) -> CP:
+    def getter(self, fget):
         return super().getter(self._wrap_fget(fget))
 
 
     def setter(self, fset):
         raise NotImplementedError(
             "classproperty can only be read-only; use a metaclass to "
             "implement modifiable class-level properties")
@@ -712,33 +707,28 @@
     def deleter(self, fdel):
         raise NotImplementedError(
             "classproperty can only be read-only; use a metaclass to "
             "implement modifiable class-level properties")
 
 
     @staticmethod
-    def _wrap_fget(orig_fget) -> Callable[[Any], Any]:
+    def _wrap_fget(orig_fget):
         if isinstance(orig_fget, classmethod):
             orig_fget = orig_fget.__func__
 
         # Using stock functools.wraps instead of the fancier version
         # found later in this module, which is overkill for this purpose
 
         @functools.wraps(orig_fget)
         def fget(obj):
             return orig_fget(obj.__class__)
 
         return fget
 
 
-class lazyclassproperty(classproperty):
-    def __new__(cls, fget=None, doc=None):
-        return super().__new__(cls, fget, doc, lazy=True)
-
-
 class _CachedClassProperty(object):
     """Cached class property decorator.
     Transforms a class method into a property whose value is computed once
     and then cached as a normal attribute for the life of the class.  Example
     usage:
     >>> class MyClass(object):
     ...   @cached_classproperty
@@ -1139,94 +1129,7 @@
 
         # If the original has a not-empty docstring append it to the format
         # kwargs.
         kwargs['__doc__'] = obj.__doc__ or ''
         obj.__doc__ = doc.format(*args, **kwargs)
         return obj
     return set_docstring
-
-
-def add_doc(docstring, *args, **kwargs):
-    """
-    Adds the docstring of the decorated object.
-
-    Parameters
-    ----------
-    docstring : str or object or None
-        The docstring that will replace the docstring of the decorated
-        object. If it is an object like a function or class it will
-        take the docstring of this object. If it is a string it will use the
-        string itself. One special case is if the string is ``None`` then
-        it will use the decorated functions docstring and formats it.
-    """
-
-    def set_docstring(obj):
-        if docstring is None:
-            # None means: use the objects __doc__
-            doc = obj.__doc__
-        elif isinstance(docstring, str):
-            # String: use the string that was given
-            doc = docstring
-        else:
-            # Something else: Use the __doc__ of this
-            doc = docstring.__doc__
-
-        if not doc:
-            # In case the docstring is empty it's probably not what was wanted.
-            raise ValueError('docstring must be a string or containing a '
-                             'docstring that is not empty.')
-        obj.__doc__ = doc
-        return obj
-
-    return set_docstring
-
-# Incase its not supported in lower versions of python
-try:
-    from typing import Generic
-
-    # https://discuss.python.org/t/add-a-supported-read-only-classproperty-decorator-in-the-stdlib/18090/12
-
-    T = TypeVar("T")
-    R = TypeVar("R")
-
-    class classproperty_v2(Generic[T, R]):
-        def __init__(self, func: Callable[[Type[T]], R]) -> None:
-            self.func = func
-
-        def __get__(self, obj: Any, cls: Type[T]) -> R:
-            return self.func(cls)
-        
-    class lazyclassproperty_v2(Generic[T, R]):
-        def __init__(self, func: Callable[[Type[T]], R]) -> None:
-            self.func = func
-            self._key = self.func.__name__
-            self._lock = threading.RLock()
-
-        def __get__(self, obj: Any, cls: Type[T]) -> R:
-            try:
-                obj_dict = obj.__dict__
-                val = obj_dict.get(self._key, _NotFound)
-                if val is _NotFound:
-                    with self._lock:
-                        # Check if another thread beat us to it.
-                        val = obj_dict.get(self._key, _NotFound)
-                        if val is _NotFound:
-                            val = self.func(cls)
-                            obj_dict[self._key] = val
-                return val
-            except AttributeError:
-                if obj is None:
-                    return self
-                raise
-        
-        def __set__(self, obj: Any, value: Any) -> None:
-            obj_dict = obj.__dict__
-            obj_dict[self._key] = value
-        
-        def __delete__(self, obj: Any) -> None:
-            obj_dict = obj.__dict__
-            obj_dict.pop(self._key, None)
-
-
-except Exception:
-    classproperty_v2 = classproperty
-    lazyclassproperty_v2 = lazyclassproperty
```

### Comparing `lazyops-0.2.82/lazyops/types/formatting.py` & `lazyops-0.2.9/lazyops/types/formatting.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,26 @@
 import typing
 from re import sub
 
 def to_camel_case(text: str):
-    """
-    Convert a snake str to camel case.
-    multi_master -> multiMaster
-    """
+    """Convert a snake str to camel case."""
     components = text.split("_")
     # We capitalize the first letter of each component except the first one
     # with the 'title' method and join them together.
     return components[0] + "".join(x.title() for x in components[1:])
 
 def to_snake_case(text: str):
     """
     multiMaster -> multi_master
     """
     return '_'.join(
         sub('([A-Z][a-z]+)', r' \1',
         sub('([A-Z]+)', r' \1',
         text.replace('-', ' '))).split()).lower()
 
-
-def to_snake_case_key(text: str):
-    """
-    multi_master -> multi-master
-    """
-    return '-'.join(
-        sub('([A-Z][a-z]+)', r' \1',
-        sub('([A-Z]+)', r' \1',
-        text.replace('_', ' '))).split()).lower()
-        
-
 def to_snake_case_args(text: str):
     """
     multiMaster -> multi-master
     """
     return '-'.join(
         sub('([A-Z][a-z]+)', r' \1',
         sub('([A-Z]+)', r' \1',
```

### Comparing `lazyops-0.2.82/lazyops/types/resources.py` & `lazyops-0.2.9/lazyops/types/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,155 +1,145 @@
+import os
+import pathlib
 
-from lazyops.types.models import BaseModel
-from lazyops.types.static import VALID_REQUEST_KWARGS
-from lazyops.types.classprops import lazyproperty
-from lazyops.imports._aiohttpx import aiohttpx
-from lazyops.imports._pydantic import get_pyd_fields, pyd_parse_obj, get_pyd_dict
-from typing import Optional, Dict, Any, Tuple, Type, Union, TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from pydantic.typing import AbstractSetIntStr, MappingIntStrAny
+from typing import Any, Type, Tuple, Dict, List, Union, Optional
+from pydantic import Field, validator
+from pydantic import BaseModel as _BaseModel
+from pydantic import BaseSettings as _BaseSettings
+from lazyops.types.formatting import to_snake_case, to_graphql_format
+from lazyops.types.classprops import classproperty
+from lazyops.utils.serialization import Json
+
+class BaseSettings(_BaseSettings):
+
+    class Config:
+        env_prefix: str = ""
+        case_sensitive: bool = False
+
+    def update_config(self, **kwargs):
+        """
+        Update the config for the other settings
+        """
+        for k, v in kwargs.items():
+            if not hasattr(self, k): continue
+            if isinstance(getattr(self, k), pathlib.Path):
+                setattr(self, k, pathlib.Path(v))
+            elif isinstance(getattr(self, k), BaseSettings):
+                val = getattr(self, k)
+                if hasattr(val, 'update_config'):
+                    val.update_config(**v)
+                else:
+                    val = val.__class__(**v)
+                setattr(self, k, val)
+            else: 
+                setattr(self, k, v)
+
+    def set_env(self):
+        """
+        Update the Env variables for the current session
+        """
+        data = self.dict(exclude_none=True)
+        for k, v in data.items():
+            if isinstance(v, BaseSettings):
+                v.set_env()
+            else:
+                os.environ[self.Config.env_prefix + k.upper()] = str(v)
+
+
+class BaseModel(_BaseModel):
+    class Config:
+        extra = 'allow'
+        arbitrary_types_allowed = True
+        alias_generator = to_snake_case
+        
+    def get(self, name, default: Any = None):
+        return getattr(self, name, default)
+    
+    def update(self, **kwargs):
+        for k, v in kwargs.items():
+            if not hasattr(self, k): continue
+            setattr(self, k, v)
 
-__all__ = [
-    'BaseResource',
-    'ResourceType',
-    'ResponseResource',
-    'ResponseResourceType',
-]
-
-
-class BaseResource(BaseModel):
-
-    @property
-    def exclude_none(self):
-        return True
-
-    @property
-    def exclude_fields(self):
-        return {'exclude_none', 'exclude_fields'}
 
     @classmethod
-    def parse_resource(
+    def create_one(
         cls,
         **kwargs
-    ) -> Tuple[Type['BaseResource'], Dict]:
+    ) -> Tuple[Type['BaseModel'], Dict]:
         """
         Extracts the resource from the kwargs and returns the resource 
         and the remaining kwargs
         """
-        resource_fields = [field.name for field in get_pyd_fields(cls)]
+        resource_fields = [field.name for field in cls.__fields__.values()]
         resource_kwargs = {k: v for k, v in kwargs.items() if k in resource_fields}
-        return_kwargs = {k: v for k, v in kwargs.items() if k not in resource_fields and k in VALID_REQUEST_KWARGS}
-        # resource_obj = cls.parse_obj(resource_kwargs)
-        resource_obj = pyd_parse_obj(cls, resource_kwargs)
-        return resource_obj, return_kwargs
-
-
-    @staticmethod
-    def create_resource(
-        resource: Type['BaseResource'],
-        **kwargs
-    ) -> Tuple[Type['BaseResource'], Dict]:
-        """
-        Extracts the resource from the kwargs and returns the resource 
-        and the remaining kwargs
-        """
-        resource_fields = [field.name for field in get_pyd_fields(resource)]
-        resource_kwargs = {k: v for k, v in kwargs.items() if k in resource_fields}
-        return_kwargs = {k: v for k, v in kwargs.items() if k not in resource_fields and k in VALID_REQUEST_KWARGS}
-        resource_obj = pyd_parse_obj(resource, resource_kwargs)
+        return_kwargs = {k: v for k, v in kwargs.items() if k not in resource_fields}
+        resource_obj = cls.parse_obj(resource_kwargs)
         return resource_obj, return_kwargs
     
+    @classmethod
+    def create_many(cls, data: List[Dict]) -> List['BaseModel']:
+        return [cls.parse_obj(d) for d in data]
+    
+    @classproperty
+    def model_fields(cls) -> List[str]:
+        return [field.name for field in cls.__fields__.values()]
+    
+    def get_model_fields(self) -> List[str]:
+        return [field.name for field in self.__fields__.values()]
 
-    def dict(
+    def replace(self, obj: Type['BaseModel']):
+        """Replace current attributes with `obj` attributes."""
+        for field in obj.model_fields:
+            if hasattr(self, field):
+                setattr(self, field, getattr(obj, field))
+
+    def graphql(
         self,
         *,
-        include: Optional[Union['AbstractSetIntStr', 'MappingIntStrAny']] = None,
-        exclude: Optional[Union['AbstractSetIntStr', 'MappingIntStrAny']] = None,
+        include: Optional[Any] = None,
+        exclude: Optional[Any] = None,
         by_alias: bool = False,
         skip_defaults: Optional[bool] = None,
         exclude_unset: bool = False,
         exclude_defaults: bool = False,
-        exclude_none: Optional[bool] = None,
-    ):
+        exclude_none: bool = False,
+    ) -> Union[Dict, Any]:
         """
-        Returns the dict representation of the response
+        Return the data in `graphql` format
         """
-        if exclude is None: exclude = set()
-        if self.exclude_fields:
-            exclude = set(exclude) | self.exclude_fields
-        return get_pyd_dict(
-            include = include, 
-            exclude = exclude, 
-            by_alias = by_alias,
-            skip_defaults = skip_defaults,
-            exclude_unset = exclude_unset,
-            exclude_defaults = exclude_defaults,
-            exclude_none = exclude_none if exclude_none is not None else self.exclude_none
+        data = self.dict(
+            include = include, exclude = exclude, \
+            by_alias = by_alias, skip_defaults = skip_defaults, \
+            exclude_unset = exclude_unset, exclude_defaults = exclude_defaults, \
+            exclude_none = exclude_none
         )
-        # return super().dict(
-        #     include = include, 
-        #     exclude = exclude, 
-        #     by_alias = by_alias,
-        #     skip_defaults = skip_defaults,
-        #     exclude_unset = exclude_unset,
-        #     exclude_defaults = exclude_defaults,
-        #     exclude_none = exclude_none if exclude_none is not None else self.exclude_none
-        # )
+        return to_graphql_format(data)
 
-    def parse_data(
-        self,
-        **kwargs
-    ):
-        """
-        Parses the prediction response
-        """
-        pass
 
 
-ResourceType = Type[BaseResource]
+class Schema(BaseModel):
 
+    class Config:
+        extra = 'allow'
+        arbitrary_types_allowed = True
+        json_dumps = Json.dumps
 
-class ResponseResource(BaseResource):
-    _input_obj: Optional[ResourceType] = None
-    _response: Optional['aiohttpx.Response'] = None
-    _streamed_data: Optional[str] = None
+    def get(self, name, default: Any = None):
+        return getattr(self, name, default)
 
-    @property
-    def exclude_fields(self):
-        return {'_input_obj', '_response', '_streamed_data', 'exclude_none', 'exclude_fields'}
 
-    @lazyproperty
-    def headers(self):
-        return self._response.headers
-    
-    @lazyproperty
-    def status_code(self):
-        return self._response.status_code
-
-    @lazyproperty
-    def has_stream(self):
-        return "text/event-stream" in self.headers.get("content-type", "")
-    
-    @lazyproperty
-    def json_data(self) -> Dict[str, Any]:
-        return self._response.json()
+class Constant(tuple):
+    "Pretty display of immutable constant."
 
-    @classmethod
-    def parse_from(
-        cls,
-        input_obj: ResourceType,
-        response: 'aiohttpx.Response',
-        **kwargs
-    ) -> 'ResponseResourceType':
-        """
-        Parses the response and returns the response object
-        """
-        resp = cls(
-            _input_obj = input_obj,
-            _response = response,
-            **response.json()
-        )
-        resp.parse_data(**kwargs)
-        return resp
+    def __new__(cls, name):
+        return tuple.__new__(cls, (name,))
+
+    def __repr__(self):
+        return f'{self[0]}'
 
-ResponseResourceType = Type[ResponseResource]
+__all__ = [
+    'Field',
+    'BaseModel',
+    'BaseSettings',
+    'Schema',
+    'validator',
+]
```

### Comparing `lazyops-0.2.82/lazyops/utils/helpers.py` & `lazyops-0.2.9/lazyops/v1/lazyconfig/nginx.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,577 +1,579 @@
-from __future__ import annotations
+from ._base import *
 
-import time
-import uuid
-import typing
-import random
-import inspect
-import functools
-import datetime
-import itertools
-import asyncio
-import contextlib
-import async_lru
-import signal
-
-from pathlib import Path
-from frozendict import frozendict
-from typing import Dict, Callable, List, Any, Union, Coroutine, TypeVar, Optional, TYPE_CHECKING
-from lazyops.utils.logs import default_logger
-
-from lazyops.utils.serialization import (
-    object_serializer, object_deserializer,
-    ObjectEncoder, ObjectDecoder,
-    Json,
-)
-
-# For backwards compatibility
-from lazyops.utils.lazy import (
-    import_string,
-    import_function, 
-    get_obj_class_name,
-    fetch_property,
-    is_coro_func,
-    lazy_function,
-    lazy_import,
-)
-
-if TYPE_CHECKING:
-    from lazyops.types import BaseModel
-    from pydantic.fields import FieldInfo
-    
-
-
-
-def timer(t: typing.Optional[float] = None, msg: typing.Optional[str] = None, logger = default_logger):
-    if not t: return time.perf_counter()
-    done_time = time.perf_counter() - t
-    if msg: logger.info(f'{msg} in {done_time:.2f} secs')
-    return done_time
-
-# def timed(func: typing.Callable):
-#     """
-#     Decorator to time a function
-#     """
-#     _func_name = func.__name__
-#     @functools.wraps(func)
-#     async def fx(*args, **kwargs):
-#         start = time.perf_counter()
-#         if inspect.iscoroutinefunction(func): result = await func(*args, **kwargs)
-#         else: result = func(*args, **kwargs)
-#         end = time.perf_counter()
-#         default_logger.info(f'{_func_name}: {end - start:.4f} secs')
-#         return result
-#     return fx
+# From https://github.com/peakwinter/python-nginx/blob/master/nginx.py
 
+logger = get_logger('LazyConfig', 'Nginx')
 
-def timed(verbose: typing.Optional[bool] = False):
-    """
-    Decorator to time a function
-    """
-    def decorator(func):
-        if inspect.iscoroutinefunction(func):
-            @functools.wraps(func)
-            async def wrapper(*args, **kwargs):
-                start = time.perf_counter()
-                result = await func(*args, **kwargs)
-                end = time.perf_counter()
-                if verbose: default_logger.info(f"took {end - start:.2f} secs with args: {args} and kwargs: {kwargs}", prefix = f"{func.__module__}.|g|{func.__name__}|e|", colored = True)
-                else: default_logger.info(f"took {end - start:.2f} secs", prefix = f"{func.__module__}.|g|{func.__name__}|e|", colored = True)
-                return result
-            return wrapper
-        
-        else:        
-            @functools.wraps(func)
-            def wrapper(*args, **kwargs):
-                start = time.perf_counter()
-                result = func(*args, **kwargs)
-                end = time.perf_counter()
-                if verbose: default_logger.info(f"took {end - start:.2f} secs with args: {args} and kwargs: {kwargs}", prefix = f"{func.__module__}.|g|{func.__name__}|e|", colored = True)
-                else: default_logger.info(f"took {end - start:.2f} secs", prefix = f"{func.__module__}.|g|{func.__name__}|e|", colored = True)
-                return result
-            return wrapper
-    
-    return decorator
-
-
-def merge_dicts(x: Dict, y: Dict):
-    z = x.copy()
-    z.update(y)
-    return z
-
-def exponential_backoff(
-    attempts: int,
-    base_delay: int = 1,
-    max_delay: int = None,
-    jitter: bool = True,
-):
-    """
-    Get the next delay for retries in exponential backoff.
-
-    attempts: Number of attempts so far
-    base_delay: Base delay, in seconds
-    max_delay: Max delay, in seconds. If None (default), there is no max.
-    jitter: If True, add a random jitter to the delay
-    """
-    if max_delay is None:
-        max_delay = float("inf")
-    backoff = min(max_delay, base_delay * 2 ** max(attempts - 1, 0))
-    if jitter:
-        backoff = backoff * random.random()
-    return backoff
-
-def retryable(limit: int = 3, delay: int = 3):
-    def decorator(func: Callable):
-        if not inspect.iscoroutinefunction(func):
-            def sync_wrapper(*args, **kwargs):
-                for n in range(limit - 1):
-                    with contextlib.suppress(Exception):
-                        return func(*args, **kwargs)
-                    time.sleep(exponential_backoff(n, base_delay=delay))
-                return func(*args, **kwargs)
-            return sync_wrapper
-        else:
-            async def async_wrapper(*args, **kwargs):
-                for n in range(limit-1):
-                    with contextlib.suppress(Exception):
-                        return await func(*args, **kwargs)
-                    await asyncio.sleep(exponential_backoff(n, base_delay=delay))
-                return await func(*args, **kwargs)
-            return async_wrapper
-    return decorator
-
-
-T = TypeVar('T')
-
-def get_batches_from_generator(iterable: typing.Iterable[T], n: int) -> typing.Generator[typing.List[T], None, None]:
-    """
-    Batch elements of an iterable into fixed-length chunks or blocks.
-    """
-    it = iter(iterable)
-    while x := tuple(itertools.islice(it, n)):
-        yield x
-
-def split_into_batches(items: List[T], n: int) -> typing.Iterable[typing.List[T]]:
-    """
-    Splits the items into n amount of equal items
-
-    >>> list(split_into_batches(range(11), 3))
-    [[0, 1, 2, 3], [4, 5, 6, 7], [8, 9, 10]]
-    """
-    n = min(n, len(items))
-    k, m = divmod(len(items), n)
-    return (items[i * k + min(i, m):(i + 1) * k + min(i + 1, m)] for i in range(n))
-
-def split_into_batches_of_n(iterable: typing.Iterable[T], n: int) -> typing.Iterable[typing.List[T]]:
-    """
-    Splits the items into fixed-length chunks or blocks.
-
-    >>> list(split_into_batches_of_n(range(11), 3))
-    [[0, 1, 2], [3, 4, 5], [6, 7, 8], [9, 10]]
-    """
-    return list(get_batches_from_generator(iterable, n))
-
-
-def split_into_n_batches(iterable: typing.Iterable[T], size: int) -> typing.Iterable[typing.List[T]]:
-    """
-    Splits the items into n amount of equal items
-
-    >>> list(split_into_batches_of_size(range(11), 3))
-    [[0, 1, 2], [3, 4, 5], [6, 7, 8], [9, 10]]
-    """
-    return split_into_batches(iterable, size)
-
-def build_batches(iterable: typing.Iterable[T], size: int, fixed_batch_size: bool = True) -> typing.Iterable[typing.List[T]]:
-    """
-    Builds batches of a given size from an iterable.
-    """
-    if fixed_batch_size:
-        return split_into_batches_of_n(iterable, size)
-    return split_into_n_batches(iterable, size)
-
-
-def split_into_batches_with_index(iterable: typing.Iterable[T], n: int, start: typing.Optional[int] = None) -> typing.Iterable[typing.Tuple[int, List[T]]]:
-    """
-    Splits the items into fixed-length chunks or blocks.
-
-    >>> list(split_into_batches_of_n(range(11), 3))
-    [(0, [0, 1, 2]), (1, [3, 4, 5]), (2, [6, 7, 8]), (3, [9, 10])]
-    """
-    return list(enumerate(get_batches_from_generator(iterable, n), start = start or 0))
-
-def create_unique_id(
-    method: typing.Optional[str] = 'uuid4',
-    alph_only: typing.Optional[bool] = False,
-    length: typing.Optional[int] = None,
-):
-    """
-    Creates a unique id
-    args:
-        method: uuid4, uuid1, uuid5, timestamp, secret
-        alph_only: if True, returns a string of only alphabets
-        length: if specified, returns a string of the specified length
-    """
-    meth = getattr(uuid, method, None)
-    if not meth:  raise ValueError(f'Invalid UUID method: {method}')
-    val = str(meth())
-    if alph_only: val = ''.join([c for c in val if c.isalpha()])
-    if length:
-        while len(val) < length:
-            val += str(meth())
-            if alph_only: val = ''.join([c for c in val if c.isalpha()])
-            # remove trailing hyphen
-            if val.endswith('-'): val = val[:-1]
-        val = val[:length]
-    return val
-
-def create_timestamp(
-    tz: typing.Optional[datetime.tzinfo] = datetime.timezone.utc,
-    as_str: typing.Optional[bool] = False,
-):
-    """
-    Creates a timestamp
-    args:
-        tz: timezone
-        as_str: if True, returns a string
-    """
-    dt = datetime.datetime.now(tz =tz)
-    return dt.isoformat() if as_str else dt
-
-def create_secret(
-    nbytes: typing.Optional[int] = 16,    
-):
-    import secrets
-    return secrets.token_hex(nbytes)
-
-
-def suppress(
-    *exceptions: typing.Optional[typing.Union[typing.Tuple[Exception], Exception]],
-):
-    """
-    Wrapper for suppressing exceptions
-    args:
-        exceptions: exceptions to suppress
-    """
-    if not exceptions: exceptions = (Exception,)
-    def wrapper(func):
-        if is_coro_func(func):
-            @functools.wraps(func)
-            async def wrapped_func(*args, **kwargs):
-                with contextlib.suppress(*exceptions):
-                    return await func(*args, **kwargs)
-            return wrapped_func
-        else:
-            @functools.wraps(func)
-            def wrapped_func(*args, **kwargs):
-                with contextlib.suppress(*exceptions):
-                    return func(*args, **kwargs)
-        return wrapped_func
-    return wrapper
-
-"""
-Timed Caches
-"""
-
-def recursive_freeze(value):
-    if not isinstance(value, dict):
-        return value
-    for k,v in value.items():
-        value[k] = recursive_freeze(v)
-    return frozendict(value)
-
-# To unfreeze
-def recursive_unfreeze(value):
-    if isinstance(value, frozendict):
-        value = dict(value)
-        for k,v in value.items():
-            value[k] = recursive_unfreeze(v)
-    
-    return value
-
-def freeze_args_and_kwargs(*args, **kwargs):
-    args = tuple(
-        recursive_freeze(arg) if isinstance(arg, dict) else arg
-        for arg in args
-    )
-    kwargs = {k: recursive_freeze(v) if isinstance(v, dict) else v for k, v in kwargs.items()}
-    return args, kwargs
-
-
-def timed_cache(
-    secs: typing.Optional[int] = 60 * 60, 
-    maxsize: int = 1024,
-    invalidate_cache_key: typing.Optional[str] = '_invalidate_cache',
-    cache_if_result: typing.Optional[typing.Any] = None,
-    cache_if_type: typing.Optional[typing.Type] = None,
-    exclude_none: typing.Optional[bool] = False,
-    **_kwargs,
-):
-    """
-    Wrapper for creating a expiring cached function
-    args:
-        secs: number of seconds to cache the function
-        maxsize: maxsize of the cache
-        invalidate_cache_key: key to invalidate the cache
-    """
-    if 'ttl' in _kwargs: secs = _kwargs.pop('ttl')
-    if secs is None: secs = 60
-    def wrapper_cache(func):
-        if is_coro_func(func):
-
-            @async_lru.alru_cache(maxsize = maxsize, ttl = secs)
-            async def _wrapped(*args, **kwargs):
-                return await func(*args, **kwargs)
-            
-            @functools.wraps(func)
-            async def wrapped_func(*args, **kwargs):
-                _invalidate = kwargs.pop(invalidate_cache_key, None) if invalidate_cache_key else None
-                args, kwargs = freeze_args_and_kwargs(*args, **kwargs)
-                if _invalidate is True: _wrapped.cache_invalidate(*args, **kwargs)
-                result = await _wrapped(*args, **kwargs)
-                if exclude_none is True and result is None:
-                    _wrapped.cache_invalidate(*args, **kwargs)
-                elif cache_if_result is not None and result != cache_if_result:
-                    _wrapped.cache_invalidate(*args, **kwargs)
-                elif cache_if_type is not None and not isinstance(result, cache_if_type):
-                    _wrapped.cache_invalidate(*args, **kwargs)
-                    # print(f'Invalidating cache for {func.__name__}')
-                return result
-            
-            return wrapped_func
-        
-        else:
-            func = functools.lru_cache(maxsize=maxsize)(func)
-            func.lifetime = datetime.timedelta(seconds=secs)
-            func.expiration = create_timestamp() + func.lifetime
-            def _check_cache(func, invalidate: typing.Optional[bool] = None):
-                if invalidate is True or create_timestamp() >= func.expiration:
-                    func.cache_clear()
-                    func.expiration = create_timestamp() + func.lifetime
-            
-            @functools.wraps(func)
-            def wrapped_func(*args, **kwargs):
-                _check_cache(func, invalidate = kwargs.pop(invalidate_cache_key, None) if invalidate_cache_key else None)
-                args, kwargs = freeze_args_and_kwargs(*args, **kwargs)
-                result = func(*args, **kwargs)
-                if exclude_none is True and result is None:
-                    func.cache_clear()
-                elif cache_if_result is not None and result != cache_if_result:
-                    func.cache_clear()
-                elif cache_if_type is not None and not isinstance(result, cache_if_type):
-                    func.cache_clear()
-                return result
-            
-            return wrapped_func
-
-    return wrapper_cache
-        
-
-
-def with_fail_after(delay: float):
-    """
-    Creates a timeout for a function
-    """
-
-    def wrapper(func):
-        @functools.wraps(func)
-        def time_limited(*args, **kwargs):
-            # Register an handler for the timeout
-            def handler(signum, frame):
-                raise TimeoutError(f"Timeout for function '{func.__name__}'")
-
-            # Register the signal function handler
-            signal.signal(signal.SIGALRM, handler)
-
-            # Define a timeout for your function
-            signal.alarm(delay)
-
-            result = None
-            try:
-                result = func(*args, **kwargs)
-            except Exception as exc:
-                raise exc
-            finally:
-                # disable the signal alarm
-                signal.alarm(0)
-
-            return result
-
-        return time_limited
-    return wrapper
-
-
-@contextlib.contextmanager
-def fail_after(delay: Union[int, float]):
-    """
-    Creates a timeout for a function
-    """
-    def signal_handler(signum, frame):
-        raise TimeoutError(f"Timed out after {delay}s")
-    signal.signal(signal.SIGALRM, signal_handler)
-    signal.alarm(int(delay))
-    try:
-        yield
-    finally:
-        signal.alarm(0)
-
-
-async def run_as_coro(
-    func: Callable,
-    *args,
-    **kwargs
-) -> Any:
-    """
-    Runs a function as a coroutine
-    """
-    from .pooler import ThreadPooler
-    try:
-        return await ThreadPooler.asyncish(func, *args, **kwargs)
-    except Exception as e:
-        default_logger.trace('Error running as coro', error = e)
-        raise e
-
-
-_background_tasks = set()
-
-
-def create_background_task(func: Union[Callable, Coroutine], *args, **kwargs):
-    """
-    Creates a background task and adds it to the global set of background tasks
-    """
-    if inspect.isawaitable(func):
-        task = asyncio.create_task(func)
-    else:
-        task = asyncio.create_task(
-            run_as_coro(
-                func,
-                *args,
-                **kwargs
-            )
-        )
-    _background_tasks.add(task)
-    task.add_done_callback(_background_tasks.discard)
-    return task
-
-
-async def adeferred_task(
-    func: Union[Callable, Coroutine],
-    *args,
-    wait_time: typing.Optional[float] = 10.0,
-    **kwargs,
-):
-    """
-    Runs a function as a background task
-    """
-    await asyncio.sleep(wait_time)
-    return create_background_task(func, *args, **kwargs)
-
+INDENT = '    '
 
-
-def build_dict_from_str(
-    data: str,
-    **kwargs
-) -> Union[List[Any], Dict[str, Any]]:
-    """
-    Helper to build a dictionary from a string
-    """
-    import json
-    if (data.startswith('[') and data.endswith(']')) or (data.startswith('{') and data.endswith('}')):
-        return json.loads(data)
-    return build_dict_from_list(data.split(','), **kwargs)
-
-
-def build_dict_from_list(
-    data: List[str],
-    seperator: str = '=',
-) -> Dict[str, Any]:
-    """
-    Builds a dictionary from a list of strings
-    """
-    import json
-    return json.loads(str(dict([item.split(seperator) for item in data])))
-
-
-
-def build_dict_from_query(
-    query: str,
-    **kwargs,
-) -> Dict[str, Union[int, float, str, datetime.datetime, Any]]:
-    """
-    Builds a dictionary from a query
-    """
-    # Try to base decode it
-    if not query.startswith('{') and not query.startswith('['):
-        import base64
-        query = base64.b64decode(query).decode('utf-8')
-    data = build_dict_from_str(query, **kwargs)
-    for k,v in data.items():
-        if 'date' in k:
-            with contextlib.suppress(Exception):
-                from lazyops.utils.dates import parse_datetime
-                v = parse_datetime(v)
-        data[k] = v
-    return data
-
-def is_pydantic_field_of_type(
-    field: 'FieldInfo',
-    t: typing.Any,
-) -> bool:
-    """
-    Inspects the type of a pydantic field to determine
-    whether it is of a certain type
-    """
+class Error(Exception):
     pass
 
-    # if hasattr(field, 'type_'):
-    #     return field.type_.__name__
-    # return field.type__.__name__
-
-
-
-@contextlib.contextmanager
-def patch_env(
-    env_file: Optional[Union[str, 'Path']] = None,
-    reset_on_exit: Optional[bool] = True,
-    **env_vars: Dict[str, Any],
-):
-    """
-    Context manager to patch the current environment variables
-
-    Args:
-        env_file: Path to the environment file. Supported formats: .env, .json, .yaml
-        reset_on_exit: If True, resets the environment variables on exit
-        **env_vars: Environment variables to set
-    
-    Yields:
-        None
-    """
-    import os
-    current_env = dict(os.environ)
-    try:
-        if env_file:
-            env_file = Path(env_file)
-            if not env_file.exists():
-                raise FileNotFoundError(f'Environment file not found: {env_file}')
-            if env_file.suffix == '.env':
-                from dotenv import load_dotenv
-                load_dotenv(env_file, override=True)
-            elif env_file.suffix == '.json':
-                import json
-                with open(env_file, 'r') as f:
-                    env_vars.update(json.load(f))
-            elif env_file.suffix == '.yaml':
-                import yaml
-                with open(env_file, 'r') as f:
-                    env_vars.update(yaml.safe_load(f))
-
-        for k, v in env_vars.items():
-            os.environ[k] = str(v)
-        yield
-    finally:
-        if reset_on_exit:
-            os.environ.clear()
-            os.environ.update(current_env)
-
-    
+class ParseError(Error):
+    pass
 
-    
+def bump_child_depth(obj, depth):
+    children = getattr(obj, 'children', [])
+    for child in children:
+        child._depth = depth + 1
+        bump_child_depth(child, child._depth)
+
+
+class NginxConfig(object):
+    """
+    Represents an nginx configuration.
+    A `NginxConfig` can consist of any number of server blocks, as well as Upstream
+    and other types of containers. It can also include top-level comments.
+    """
+
+    def __init__(self, *args):
+        """
+        Initialize object.
+        :param *args: Any objects to include in this NginxConfig.
+        """
+        self.children = list(args)
+
+    def add(self, *args):
+        """
+        Add object(s) to the NginxConfig.
+        :param *args: Any objects to add to the NginxConfig.
+        :returns: full list of NginxConfig's child objects
+        """
+        self.children.extend(args)
+        return self.children
+
+    def remove(self, *args):
+        """
+        Remove object(s) from the NginxConfig.
+        :param *args: Any objects to remove from the NginxConfig.
+        :returns: full list of NginxConfig's child objects
+        """
+        for x in args:
+            self.children.remove(x)
+        return self.children
+
+    def filter(self, btype='', name=''):
+        """
+        Return child object(s) of this NginxConfig that satisfy certain criteria.
+        :param str btype: Type of object to filter by (e.g. 'Key')
+        :param str name: Name of key OR container value to filter by
+        :returns: full list of matching child objects
+        """
+        filtered = []
+        for x in self.children:
+            if name and isinstance(x, Key) and x.name == name:
+                filtered.append(x)
+            elif isinstance(x, Container) and x.__class__.__name__ == btype \
+                    and x.value == name:
+                filtered.append(x)
+            elif not name and btype and x.__class__.__name__ == btype:
+                filtered.append(x)
+        return filtered
+
+    @property
+    def servers(self):
+        """Return a list of child Server objects."""
+        return [x for x in self.children if isinstance(x, Server)]
+
+    @property
+    def server(self):
+        """Convenience property to fetch the first available server only."""
+        return self.servers[0]
+
+    @property
+    def as_list(self):
+        """Return all child objects in nested lists of strings."""
+        return [x.as_list for x in self.children]
+
+    @property
+    def as_dict(self):
+        """Return all child objects in nested dict."""
+        return {'conf': [x.as_dict for x in self.children]}
+
+    @property
+    def as_strings(self):
+        """Return the entire NginxConfig as nginx config strings."""
+        ret = []
+        for x in self.children:
+            if isinstance(x, (Key, Comment)):
+                ret.append(x.as_strings)
+            else:
+                for y in x.as_strings:
+                    ret.append(y)
+        if ret:
+            ret[-1] = re.sub('}\n+$', '}\n', ret[-1])
+        return ret
+
+
+class Container(object):
+    """
+    Represents a type of child block found in an nginx config.
+    Intended to be subclassed by various types of child blocks, like
+    Locations or Geo blocks.
+    """
+
+    def __init__(self, value, *args):
+        """
+        Initialize object.
+        :param str value: Value to be used in name (e.g. regex for Location)
+        :param *args: Any objects to include in this NginxConfig.
+        """
+        self.name = ''
+        self.value = value
+        self._depth = 0
+        self.children = list(args)
+        bump_child_depth(self, self._depth)
+
+    def add(self, *args):
+        """
+        Add object(s) to the Container.
+        :param *args: Any objects to add to the Container.
+        :returns: full list of Container's child objects
+        """
+        self.children.extend(args)
+        bump_child_depth(self, self._depth)
+        return self.children
+
+    def remove(self, *args):
+        """
+        Remove object(s) from the Container.
+        :param *args: Any objects to remove from the Container.
+        :returns: full list of Container's child objects
+        """
+        for x in args:
+            self.children.remove(x)
+        return self.children
+
+    def filter(self, btype='', name=''):
+        """
+        Return child object(s) of this Server block that meet certain criteria.
+        :param str btype: Type of object to filter by (e.g. 'Key')
+        :param str name: Name of key OR container value to filter by
+        :returns: full list of matching child objects
+        """
+        filtered = []
+        for x in self.children:
+            if name and isinstance(x, Key) and x.name == name:
+                filtered.append(x)
+            elif isinstance(x, Container) and x.__class__.__name__ == btype \
+                    and x.value == name:
+                filtered.append(x)
+            elif not name and btype and x.__class__.__name__ == btype:
+                filtered.append(x)
+        return filtered
+
+    @property
+    def locations(self):
+        """Return a list of child Location objects."""
+        return [x for x in self.children if isinstance(x, Location)]
+
+    @property
+    def comments(self):
+        """Return a list of child Comment objects."""
+        return [x for x in self.children if isinstance(x, Comment)]
+
+    @property
+    def keys(self):
+        """Return a list of child Key objects."""
+        return [x for x in self.children if isinstance(x, Key)]
+
+    @property
+    def as_list(self):
+        """Return all child objects in nested lists of strings."""
+        return [self.name, self.value, [x.as_list for x in self.children]]
+
+    @property
+    def as_dict(self):
+        """Return all child objects in nested dict."""
+        dicts = [x.as_dict for x in self.children]
+        return {'{0} {1}'.format(self.name, self.value): dicts}
+
+    @property
+    def as_strings(self):
+        """Return the entire Container as nginx config strings."""
+        ret = []
+        container_title = (INDENT * self._depth)
+        container_title += '{0}{1} {{\n'.format(
+            self.name, (' {0}'.format(self.value) if self.value else '')
+        )
+        ret.append(container_title)
+        for x in self.children:
+            if isinstance(x, Key):
+                ret.append(INDENT + x.as_strings)
+            elif isinstance(x, Comment):
+                if x.inline and len(ret) >= 1:
+                    ret[-1] = ret[-1].rstrip('\n') + '  ' + x.as_strings
+                else:
+                    ret.append(INDENT + x.as_strings)
+            elif isinstance(x, Container):
+                y = x.as_strings
+                ret.append('\n' + y[0])
+                for z in y[1:]:
+                    ret.append(INDENT + z)
+            else:
+                y = x.as_strings
+                ret.append(INDENT + y)
+        ret[-1] = re.sub('}\n+$', '}\n', ret[-1])
+        ret.append('}\n\n')
+        return ret
+
+
+class Comment(object):
+    """Represents a comment in an nginx config."""
+
+    def __init__(self, comment, inline=False):
+        """
+        Initialize object.
+        :param str comment: Value of the comment
+        :param bool inline: This comment is on the same line as preceding item
+        """
+        self.comment = comment
+        self.inline = inline
+
+    @property
+    def as_list(self):
+        """Return comment as nested list of strings."""
+        return [self.comment]
+
+    @property
+    def as_dict(self):
+        """Return comment as dict."""
+        return {'#': self.comment}
+
+    @property
+    def as_strings(self):
+        """Return comment as nginx config string."""
+        return '# {0}\n'.format(self.comment)
+
+
+class Http(Container):
+    """Container for HTTP sections in the main NGINX conf file."""
+
+    def __init__(self, *args):
+        """Initialize."""
+        super(Http, self).__init__('', *args)
+        self.name = 'http'
+
+
+class Server(Container):
+    """Container for server block configurations."""
+
+    def __init__(self, *args):
+        """Initialize."""
+        super(Server, self).__init__('', *args)
+        self.name = 'server'
+
+    @property
+    def as_dict(self):
+        """Return all child objects in nested dict."""
+        return {'server': [x.as_dict for x in self.children]}
+
+
+class Location(Container):
+    """Container for Location-based options."""
+
+    def __init__(self, value, *args):
+        """Initialize."""
+        super(Location, self).__init__(value, *args)
+        self.name = 'location'
+
+
+class Events(Container):
+    """Container for Event-based options."""
+
+    def __init__(self, *args):
+        """Initialize."""
+        super(Events, self).__init__('', *args)
+        self.name = 'events'
+
+
+class LimitExcept(Container):
+    """Container for specifying HTTP method restrictions."""
+
+    def __init__(self, value, *args):
+        """Initialize."""
+        super(LimitExcept, self).__init__(value, *args)
+        self.name = 'limit_except'
+
+
+class Types(Container):
+    """Container for MIME type mapping."""
+
+    def __init__(self, *args):
+        """Initialize."""
+        super(Types, self).__init__('', *args)
+        self.name = 'types'
+
+
+class If(Container):
+    """Container for If conditionals."""
+
+    def __init__(self, value, *args):
+        """Initialize."""
+        super(If, self).__init__(value, *args)
+        self.name = 'if'
+
+
+class Upstream(Container):
+    """Container for upstream configuration (reverse proxy)."""
+
+    def __init__(self, value, *args):
+        """Initialize."""
+        super(Upstream, self).__init__(value, *args)
+        self.name = 'upstream'
+
+
+class Geo(Container):
+    """
+    Container for geo module configuration.
+    See docs here: http://nginx.org/en/docs/http/ngx_http_geo_module.html
+    """
+
+    def __init__(self, value, *args):
+        """Initialize."""
+        super(Geo, self).__init__(value, *args)
+        self.name = 'geo'
+
+
+class Map(Container):
+    """Container for map configuration."""
+
+    def __init__(self, value, *args):
+        """Initialize."""
+        super(Map, self).__init__(value, *args)
+        self.name = 'map'
+
+
+class Stream(Container):
+    """Container for stream sections in the main NGINX conf file."""
+
+    def __init__(self, *args):
+        """Initialize."""
+        super(Stream, self).__init__('', *args)
+        self.name = 'stream'
+
+
+class Key(object):
+    """Represents a simple key/value object found in an nginx config."""
+
+    def __init__(self, name, value):
+        """
+        Initialize object.
+        :param *args: Any objects to include in this Server block.
+        """
+        self.name = name
+        self.value = value
+
+    @property
+    def as_list(self):
+        """Return key as nested list of strings."""
+        return [self.name, self.value]
+
+    @property
+    def as_dict(self):
+        """Return key as dict key/value."""
+        return {self.name: self.value}
+
+    @property
+    def as_strings(self):
+        """Return key as nginx config string."""
+        if self.value == '' or self.value is None:
+            return '{0};\n'.format(self.name)
+        if type(self.value) == str and '"' not in self.value and (';' in self.value or '#' in self.value):
+            return '{0} "{1}";\n'.format(self.name, self.value)
+        return '{0} {1};\n'.format(self.name, self.value)
+
+
+class Nginx:
+
+    @classmethod
+    def loads(cls, data, conf=True):
+        """
+        Load an nginx configuration from a provided string.
+        :param str data: nginx configuration
+        :param bool conf: Load object(s) into a NginxConfig object?
+        """
+        f = NginxConfig() if conf else []
+        lopen = []
+        index = 0
+
+        while True:
+            m = re.compile(r'^\s*events\s*{').search(data[index:])
+            if m:
+                logger.debug("Open (Events)")
+                e = Events()
+                lopen.insert(0, e)
+                index += m.end()
+                continue
+
+            m = re.compile(r'^\s*http\s*{').search(data[index:])
+            if m:
+                logger.debug("Open (Http)")
+                h = Http()
+                lopen.insert(0, h)
+                index += m.end()
+                continue
+
+            m = re.compile(r'^\s*stream\s*{').search(data[index:])
+            if m:
+                logger.debug("Open (Stream)")
+                s = Stream()
+                lopen.insert(0, s)
+                index += m.end()
+                continue
+
+            m = re.compile(r'^\s*server\s*{').search(data[index:])
+            if m:
+                logger.debug("Open (Server)")
+                s = Server()
+                lopen.insert(0, s)
+                index += m.end()
+                continue
+
+            n = re.compile(r'(?!\B"[^"]*);(?![^"]*"\B)')
+            m = re.compile(r'^\s*location\s+(.*?".*?".*?|.*?)\s*{').search(data[index:])
+            if m and not n.search(m.group()):
+                logger.debug("Open (Location) {0}".format(m.group(1)))
+                l = Location(m.group(1))
+                lopen.insert(0, l)
+                index += m.end()
+                continue
+
+            m = re.compile(r'^\s*if\s+(.*?".*?".*?|.*?)\s*{').search(data[index:])
+            if m and not n.search(m.group()):
+                logger.debug("Open (If) {0}".format(m.group(1)))
+                ifs = If(m.group(1))
+                lopen.insert(0, ifs)
+                index += m.end()
+                continue
+
+            m = re.compile(r'^\s*upstream\s+(.*?)\s*{').search(data[index:])
+            if m and not n.search(m.group()):
+                logger.debug("Open (Upstream) {0}".format(m.group(1)))
+                u = Upstream(m.group(1))
+                lopen.insert(0, u)
+                index += m.end()
+                continue
+
+            m = re.compile(r'^\s*geo\s+(.*?".*?".*?|.*?)\s*{').search(data[index:])
+            if m and not n.search(m.group()):
+                logger.debug("Open (Geo) {0}".format(m.group(1)))
+                g = Geo(m.group(1))
+                lopen.insert(0, g)
+                index += m.end()
+                continue
+
+            m = re.compile(r'^\s*map\s+(.*?".*?".*?|.*?)\s*{').search(data[index:])
+            if m and not n.search(m.group()):
+                logger.debug("Open (Map) {0}".format(m.group(1)))
+                g = Map(m.group(1))
+                lopen.insert(0, g)
+                index += m.end()
+                continue
+
+            m = re.compile(r'^\s*limit_except\s+(.*?".*?".*?|.*?)\s*{').search(data[index:])
+            if m and not n.search(m.group()):
+                logger.debug("Open (LimitExcept) {0}".format(m.group(1)))
+                l = LimitExcept(m.group(1))
+                lopen.insert(0, l)
+                index += m.end()
+                continue
+
+            m = re.compile(r'^\s*types\s*{').search(data[index:])
+            if m:
+                logger.debug("Open (Types)")
+                l = Types()
+                lopen.insert(0, l)
+                index += m.end()
+                continue
+
+            m = re.compile(r'^(\s*)#[ \r\t\f]*(.*?)\n').search(data[index:])
+            if m:
+                logger.debug("Comment ({0})".format(m.group(2)))
+                c = Comment(m.group(2), inline='\n' not in m.group(1))
+                if lopen and isinstance(lopen[0], Container):
+                    lopen[0].add(c)
+                else:
+                    f.add(c) if conf else f.append(c)
+                index += m.end() - 1
+                continue
+
+            m = re.compile(r'^\s*}').search(data[index:])
+            if m:
+                if isinstance(lopen[0], Container):
+                    logger.debug("Close ({0})".format(lopen[0].__class__.__name__))
+                    c = lopen[0]
+                    lopen.pop(0)
+                    if lopen and isinstance(lopen[0], Container):
+                        lopen[0].add(c)
+                    else:
+                        f.add(c) if conf else f.append(c)
+                index += m.end()
+                continue
+
+            if ";" not in data[index:] and "}" in data[index:]:
+                # If there is still something to parse, expect ';' otherwise
+                # the Key regexp can get stuck due to regexp catastrophic backtracking
+                raise ParseError("Config syntax, missing ';' at index: {}".format(index))
+
+            double = r'\s*"[^"]*"'
+            single = r'\s*\'[^\']*\''
+            normal = r'\s*[^;\s]*'
+            s1 = r'{}|{}|{}'.format(double, single, normal)
+            s = r'^\s*({})\s*((?:{})+);'.format(s1, s1)
+            m = re.compile(s).search(data[index:])
+            if m:
+                logger.debug("Key {0} {1}".format(m.group(1), m.group(2)))
+                k = Key(m.group(1), m.group(2))
+                if lopen and isinstance(lopen[0], (Container, Server)):
+                    lopen[0].add(k)
+                else:
+                    f.add(k) if conf else f.append(k)
+                index += m.end()
+                continue
+
+            m = re.compile(r'^\s*(\S+);').search(data[index:])
+            if m:
+                logger.debug("Key {0}".format(m.group(1)))
+                k = Key(m.group(1), '')
+                if lopen and isinstance(lopen[0], (Container, Server)):
+                    lopen[0].add(k)
+                else:
+                    f.add(k) if conf else f.append(k)
+                index += m.end()
+                continue
+
+            break
+
+        return f
+
+
+    @classmethod
+    def load(cls, pathlike_or_filestr):
+        """
+        Load an nginx configuration from a provided file-like object.
+        :param obj fobj: nginx configuration
+        """
+        data = PathIO(pathlike_or_filestr).read_text() if isinstance(pathlike_or_filestr, str) else pathlike_or_filestr.read()
+        return Nginx.loads(data)
+
+    @classmethod
+    def dumps(cls, obj):
+        """
+        Dump an nginx configuration to a string.
+        :param obj obj: nginx object (NginxConfig, Server, Container)
+        :returns: nginx configuration as string
+        """
+        return ''.join(obj.as_strings)
+
+    @classmethod
+    def dump(cls, obj, pathlike_or_filestr):
+        """
+        Write an nginx configuration to a file-like object.
+        :param obj obj: nginx object (NginxConfig, Server, Container)
+        :param obj fobj: file-like object to write to
+        :returns: file-like object that was written to
+        """
+        pathlike = PathIO(pathlike_or_filestr) if isinstance(pathlike_or_filestr, str) else pathlike_or_filestr
+        pathlike.write(Nginx.dumps(obj))
+        return pathlike
```

### Comparing `lazyops-0.2.82/lazyops/utils/imports.py` & `lazyops-0.2.9/lazyops/utils/imports.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,46 @@
 """
 Base Import Handler
 """
 import typing
 import functools
-import pathlib
-import importlib.util
 from lazyops.utils.logs import default_logger as logger
 from lazyops.utils.lazylib import LazyLib
 from lazyops.utils.helpers import is_coro_func
 
 def resolve_missing(
     modules: typing.Union[str, typing.List],
-    packages: typing.Union[str, typing.List] = None,
     required: bool = True,
 ):
     if not isinstance(modules, list):
         modules = [modules]
-    if packages is not None and not isinstance(packages, list):
-        packages = [packages]
-    elif packages is None:
-        packages = modules
     kind = 'required' if required else 'optionally required'
     logger.info(f"{', '.join(modules)} are {kind}. Installing...")
-    for module, pkg in zip(modules, packages):
-        LazyLib.import_lib(module, pkg)
+    for module in modules:
+        LazyLib.import_lib(module)
 
 
 def resolve_missing_custom(
     modules: typing.Union[str, typing.List],
-    packages: typing.Union[str, typing.List] = None,
     required: bool = True,
 ):
     """
     Handles custom use cases like `torch` where we need to
     have a extra index to install from
     """
     if not isinstance(modules, list):
         modules = [modules]
-    if packages is not None and not isinstance(packages, list):
-        packages = [packages]
-    elif packages is None:
-        packages = modules
-    
     module_names = [module.split(' ', 1)[0] for module in modules]
     kind = 'required' if required else 'optionally required'
     logger.info(f"{', '.join(module_names)} are {kind}. Installing...")
-    for module, pkg in zip(modules, packages):
+    for module in modules:
         module_name = LazyLib.get_requirement(module, True)
         if LazyLib.is_available(module_name):
             continue
-        LazyLib.install_library(pkg)
+        LazyLib.install_library(module)
 
     
 def require_missing_wrapper(
     resolver: typing.Callable,
     func: typing.Callable,
     **resolver_kwargs,
 ):
@@ -67,9 +54,8 @@
             return await func(*args, **kwargs)
     else:
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             resolver(**resolver_kwargs)
             return func(*args, **kwargs)
 
-    return wrapper
-
+    return wrapper
```

### Comparing `lazyops-0.2.82/lazyops/utils/lazylib.py` & `lazyops-0.2.9/lazyops/utils/lazylib.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/utils/system.py` & `lazyops-0.2.9/lazyops/utils/system.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import time
 import socket
 import pathlib
 import tempfile
 import contextlib
 
-from typing import Union, Optional
+from typing import Union
 from functools import lru_cache
 
 __all__ = [
     'get_torch_device_name',
     'get_torch_device',
     'get_cpu_count',
     'is_readonly_dir',
@@ -19,26 +19,25 @@
     'get_k8s_namespace',
     'get_k8s_kubeconfig',
 ]
 
 # Lazily get these libraries
 
 @lru_cache()
-def get_torch_device_name(mps_enabled: bool = False):
+def get_torch_device_name():
     with contextlib.suppress(ImportError):
         import torch
         if torch.cuda.is_available(): return 'cuda'
-        if mps_enabled and torch.torch.backends.mps.is_available(): return 'mps'
     return 'cpu'
 
 @lru_cache()
-def get_torch_device(mps_enabled: bool = False):
+def get_torch_device():
     with contextlib.suppress(ImportError):
         import torch
-        return torch.device(get_torch_device_name(mps_enabled))
+        return torch.device(get_torch_device_name())
     return 'cpu'
 
 @lru_cache()
 def get_cpu_count() -> int:
     """Get the available CPU count for this system.
     Takes the minimum value from the following locations:
     - Total system cpus available on the host.
@@ -162,65 +161,7 @@
             _k8s_kubeconfig = '/var/run/secrets/kubernetes.io/serviceaccount/token'
         else:
             _k8s_kubeconfig = os.getenv(env_var, default)
             if _k8s_kubeconfig is None:
                 _k8s_kubeconfig = os.path.expanduser('~/.kube/config')
     return _k8s_kubeconfig
 
-
-# Local K8s
-_kubeconfig_dir: str = None
-
-def get_local_kubeconfig_dir(
-    env_var: str = 'KUBECONFIG_DIR',
-    default: str = None,
-) -> str:
-    """
-    Get the local kubernetes kubeconfig.
-    """
-    global _kubeconfig_dir
-    if _kubeconfig_dir is None:
-        _kubeconfig_dir = os.getenv(env_var, default) or os.path.expanduser('~/.kube')
-    return _kubeconfig_dir
-
-@lru_cache()
-def get_local_kubeconfig(
-    name: Optional[str] = None,
-    set_as_envval: bool = False,
-) -> str:
-    """
-    Get the local kubernetes kubeconfig
-    - this assumes that it's not the default one.
-    """
-    if name is None: return get_k8s_kubeconfig()
-    p = os.path.join(get_local_kubeconfig_dir(), name)
-    for stem in ('', '-cluster', '-admin-config', '-config', '-kubeconfig'):
-        for ext in ('', '.yaml', '.yml'):
-            if os.path.isfile(p + stem + ext): 
-                px = os.path.abspath(p + stem + ext)
-                if set_as_envval:
-                    os.environ['KUBECONFIG'] = px
-                return px
-    raise FileNotFoundError(f'Could not find kubeconfig file: {name} @ {p}')
-
-
-@lru_cache()
-def fetch_resolver_nameserver(
-    path: Optional[str] = '/etc/resolv.conf',
-) -> Optional[str]:
-    """
-    Fetches the nameserver from the resolv.conf
-    """
-    if path is None: return None
-    p = pathlib.Path(path)
-    if not p.exists(): return None
-    lines = p.read_text().splitlines()
-    return next(
-        (
-            line.split(' ')[-1].strip()
-            for line in lines
-            if line.startswith('nameserver')
-        ),
-        None,
-    )
-
-
```

### Comparing `lazyops-0.2.82/lazyops/v1/__init__.py` & `lazyops-0.2.9/lazyops/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/apis.py` & `lazyops-0.2.9/lazyops/v1/apis.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/common.py` & `lazyops-0.2.9/lazyops/v1/common.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/envs.py` & `lazyops-0.2.9/lazyops/v1/envs.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/experimental/gptj.py` & `lazyops-0.2.9/lazyops/v1/experimental/gptj.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/lazyclasses/core.py` & `lazyops-0.2.9/lazyops/v1/lazyclasses/core.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/lazyconfig/_base.py` & `lazyops-0.2.9/lazyops/v1/lazyconfig/_base.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/lazyconfig/tfserving.proto` & `lazyops-0.2.9/lazyops/v1/lazyconfig/tfserving.proto`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/lazyconfig/tfserving_pb2.py` & `lazyops-0.2.9/lazyops/v1/lazyconfig/tfserving_pb2.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/lazydatabase/_base.py` & `lazyops-0.2.9/lazyops/v1/lazydatabase/_base.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/lazydatabase/backends.py` & `lazyops-0.2.9/lazyops/v1/lazydatabase/backends.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/lazydatabase/core.py` & `lazyops-0.2.9/lazyops/v1/lazydatabase/core.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/lazydatabase/models.py` & `lazyops-0.2.9/lazyops/v1/lazydatabase/models.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/lazyio/__init__.py` & `lazyops-0.2.9/lazyops/v1/lazyio/__init__.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/lazyio/async_ops.py` & `lazyops-0.2.9/lazyops/v1/lazyio/async_ops.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/lazyio/models.py` & `lazyops-0.2.9/lazyops/v1/lazyio/models.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/lazyrpc/README.md` & `lazyops-0.2.9/lazyops/v1/lazyrpc/README.md`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/lazyrpc/__init__.py` & `lazyops-0.2.9/lazyops/v1/lazyrpc/__init__.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/lazyrpc/_base.py` & `lazyops-0.2.9/lazyops/v1/lazyrpc/_base.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/lazyrpc/core.py` & `lazyops-0.2.9/lazyops/v1/lazyrpc/core.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/lazyrpc/dependencies.py` & `lazyops-0.2.9/lazyops/v1/lazyrpc/dependencies.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/lazyrpc/exceptions.py` & `lazyops-0.2.9/lazyops/v1/lazyrpc/exceptions.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/lazyrpc/models.py` & `lazyops-0.2.9/lazyops/v1/lazyrpc/models.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/lazysources/gdelt/README.md` & `lazyops-0.2.9/lazyops/v1/lazysources/gdelt/README.md`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/lazysources/gdelt/core.py` & `lazyops-0.2.9/lazyops/v1/lazysources/gdelt/core.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/lazysources/gdelt/filters.py` & `lazyops-0.2.9/lazyops/v1/lazysources/gdelt/filters.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/lazysources/gdelt/models.py` & `lazyops-0.2.9/lazyops/v1/lazysources/gdelt/models.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/models.py` & `lazyops-0.2.9/lazyops/v1/models.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/mp.py` & `lazyops-0.2.9/lazyops/v1/mp.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/mp_utils.py` & `lazyops-0.2.9/lazyops/v1/mp_utils.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/retry.py` & `lazyops-0.2.9/lazyops/v1/retry.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/lazyops/v1/utils.py` & `lazyops-0.2.9/lazyops/v1/utils.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.82/setup.py` & `lazyops-0.2.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,59 +10,27 @@
 
 root = Path(__file__).parent
 version = root.joinpath(f'{pkg_name}/version.py').read_text().split('VERSION = ', 1)[-1].strip().replace('-', '').replace("'", '')
 
 requirements = [
     'loguru',
     'pydantic',
-    # 'pydantic-settings',
-    'frozendict',
-    'async_lru',
 ]
 
 if sys.version_info.minor < 8:
     requirements.append('typing_extensions')
 
-extras = {
-    'kops': [
-        'kubernetes',
-        'kubernetes_asyncio',
-        'kopf',
-        'aiocache',
-        # 'kr8s',
-    ],
-    'fastapi': [
-        'fastapi',
-        'uvicorn',
-        'filelock==3.12.4',
-        'pydantic-settings',
-        'python-multipart',
-    ],
-    'builder': [
-        'pyyaml',
-        'typer',
-    ],
-    'authzero': [
-        'niquests',
-        'tldextract',
-        'fastapi',
-        'pycryptodomex',
-        'pyjwt[crypto]',
-        'python-jose',
-    ]
-}
+extras = {}
 args = {
     'packages': find_packages(include = [f'{pkg_name}', f'{pkg_name}.*',]),
     'install_requires': requirements,
     'include_package_data': True,
     'long_description': root.joinpath('README.md').read_text(encoding='utf-8'),
     'entry_points': {
-        "console_scripts": [
-            'lazyops-build = lazyops.libs.abc.builder:main',
-        ]
+        "console_scripts": []
     },
     'extras_require': extras,
 }
 
 setup(
     name = pkg_name,
     version = version,
```

