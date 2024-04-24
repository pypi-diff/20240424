# Comparing `tmp/offspot_config-2.1.0.tar.gz` & `tmp/offspot_config-2.2.0.tar.gz`

## Comparing `offspot_config-2.1.0.tar` & `offspot_config-2.2.0.tar`

### file list

```diff
@@ -1,52 +1,54 @@
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 offspot_config-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    10259 2020-02-02 00:00:00.000000 offspot_config-2.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 offspot_config-2.1.0/tasks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/__init__.py
--rw-r--r--   0        0        0    29716 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/builder.py
--rw-r--r--   0        0        0    14110 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/catalog.json
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/catalog.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/constants.py
--rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/file.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/oci_images.py
--rw-r--r--   0        0        0     6652 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/packages.py
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/zim.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/inputs/__init__.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/inputs/base.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/inputs/checksum.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/inputs/file.py
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/inputs/mainconfig.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/inputs/oci.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/inputs/output.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/inputs/str.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/inputs/ways.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/utils/__init__.py
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/utils/dashboard.py
--rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/utils/download.py
--rw-r--r--   0        0        0    12617 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/utils/misc.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/utils/sizes.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/utils/yaml.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/__init__.py
--rwxr-xr-x   0        0        0    18295 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/ap.py
--rw-r--r--   0        0        0    21248 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/checks.py
--rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/configlib.py
--rwxr-xr-x   0        0        0     2564 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/containers.py
--rwxr-xr-x   0        0        0     3341 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/dnsmasqspoof.py
--rwxr-xr-x   0        0        0     5142 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/ethernet.py
--rwxr-xr-x   0        0        0     5210 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/firmware.py
--rwxr-xr-x   0        0        0     8362 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/fromfile.py
--rwxr-xr-x   0        0        0     2122 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/hostname.py
--rwxr-xr-x   0        0        0     1678 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/timezone.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 offspot_config-2.1.0/tests/conftest.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 offspot_config-2.1.0/tests/test_catalog.py
--rw-r--r--   0        0        0    21249 2020-02-02 00:00:00.000000 offspot_config-2.1.0/tests/test_checks.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 offspot_config-2.1.0/tests/test_humanid.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 offspot_config-2.1.0/tests/test_inputs.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 offspot_config-2.1.0/tests/test_link.py
--rw-r--r--   0        0        0     7235 2020-02-02 00:00:00.000000 offspot_config-2.1.0/tests/test_reader.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 offspot_config-2.1.0/tests/test_zim.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 offspot_config-2.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 offspot_config-2.1.0/LICENSE
--rw-r--r--   0        0        0    11831 2020-02-02 00:00:00.000000 offspot_config-2.1.0/README.md
--rw-r--r--   0        0        0     6733 2020-02-02 00:00:00.000000 offspot_config-2.1.0/pyproject.toml
--rw-r--r--   0        0        0    13707 2020-02-02 00:00:00.000000 offspot_config-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 offspot_config-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11183 2020-02-02 00:00:00.000000 offspot_config-2.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 offspot_config-2.2.0/tasks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/__init__.py
+-rw-r--r--   0        0        0    33843 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/builder.py
+-rw-r--r--   0        0        0    14110 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/catalog.json
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/catalog.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/constants.py
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/file.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/oci_images.py
+-rw-r--r--   0        0        0     6652 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/packages.py
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/zim.py
+-rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/branding/horizontal-logo-light.png
+-rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/branding/square-logo-light.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/inputs/__init__.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/inputs/base.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/inputs/checksum.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/inputs/file.py
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/inputs/mainconfig.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/inputs/oci.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/inputs/output.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/inputs/str.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/inputs/ways.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/utils/__init__.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/utils/dashboard.py
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/utils/download.py
+-rw-r--r--   0        0        0    12899 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/utils/misc.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/utils/sizes.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/utils/yaml.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/__init__.py
+-rwxr-xr-x   0        0        0    18295 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/ap.py
+-rw-r--r--   0        0        0    21248 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/checks.py
+-rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/configlib.py
+-rwxr-xr-x   0        0        0     2564 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/containers.py
+-rwxr-xr-x   0        0        0     3341 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/dnsmasqspoof.py
+-rwxr-xr-x   0        0        0     5142 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/ethernet.py
+-rwxr-xr-x   0        0        0     5210 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/firmware.py
+-rwxr-xr-x   0        0        0     8362 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/fromfile.py
+-rwxr-xr-x   0        0        0     2122 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/hostname.py
+-rwxr-xr-x   0        0        0     1678 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/timezone.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 offspot_config-2.2.0/tests/conftest.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 offspot_config-2.2.0/tests/test_catalog.py
+-rw-r--r--   0        0        0    21249 2020-02-02 00:00:00.000000 offspot_config-2.2.0/tests/test_checks.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 offspot_config-2.2.0/tests/test_humanid.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 offspot_config-2.2.0/tests/test_inputs.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 offspot_config-2.2.0/tests/test_link.py
+-rw-r--r--   0        0        0     7235 2020-02-02 00:00:00.000000 offspot_config-2.2.0/tests/test_reader.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 offspot_config-2.2.0/tests/test_zim.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 offspot_config-2.2.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 offspot_config-2.2.0/LICENSE
+-rw-r--r--   0        0        0    11831 2020-02-02 00:00:00.000000 offspot_config-2.2.0/README.md
+-rw-r--r--   0        0        0     6733 2020-02-02 00:00:00.000000 offspot_config-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0    13707 2020-02-02 00:00:00.000000 offspot_config-2.2.0/PKG-INFO
```

### Comparing `offspot_config-2.1.0/.pre-commit-config.yaml` & `offspot_config-2.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/CHANGELOG.md` & `offspot_config-2.2.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,34 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.2.0] - 2024-04-24
+
+### Added
+
+- [inputs.file] `File.is_base64_encoded` if `via` is `base64`
+- [utils.misc] `b64_encode()` and `b64_decode()` for reproducible base64 transport
+- [branding] `branding` folder in `offspot_config` containing official/original offspot branding files
+- [constants] `INTERNAL_BRANDING_PATH` pointing to code-reachable folder of branding files
+- [builder] `ORIGINAL_BRANDING_PATH` constant for '/data/branding`
+- [builder] `BRANDING_PATH` constant for `/data/contents/branding`
+
+### Changed
+
+- [builder] Using kiwix-serve 3.7.0-1
+- [builder] Using reverse-proxy 1.8
+- [builder] Original branding files copied to `ORIGINAL_BRANDING_PATH`
+- [builder] Creating empty `BRANDING_PATH` for hotspot-specific branding
+- [builder] Added mounts for `BRANDING_PATH` (and `ORIGINAL_BRANDING_PATH`) on all internal apps
+- [builder] Catalog apps can mount `${BRANDING_PATH}` or `${ORIGINAL_BRANDING_PATH}`
+
 ## [2.1.0] - 2024-04-18
 
 ### Added
 
 - [inputs.checksum] `Checksum` gets a `to_dict()` method
 - [dashboard] `Reader` gets an optional `checksum`
```

### Comparing `offspot_config-2.1.0/tasks.py` & `offspot_config-2.2.0/tasks.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_config/builder.py` & `offspot_config-2.2.0/src/offspot_config/builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from __future__ import annotations
 
 import re
 from pathlib import PurePath as Path
 from typing import Any
 
 from offspot_config.catalog import app_catalog, get_app_path
-from offspot_config.constants import CONTENT_TARGET_PATH
+from offspot_config.constants import (
+    CONTENT_TARGET_PATH,
+    DATA_PART_PATH,
+    INTERNAL_BRANDING_PATH,
+)
 from offspot_config.inputs.base import BaseConfig
 from offspot_config.inputs.checksum import Checksum
 from offspot_config.inputs.file import FileConfig
 from offspot_config.inputs.str import BlockStr
 from offspot_config.oci_images import OCIImage
 from offspot_config.packages import AppPackage, FilesPackage, ZimPackage
 from offspot_config.utils.dashboard import Link, Reader
+from offspot_config.utils.misc import b64_encode
 from offspot_config.utils.sizes import (
     get_margin_for,
     get_min_image_size_for,
     get_raw_content_size_for,
 )
 from offspot_config.utils.yaml import yaml_dump
 
@@ -30,14 +35,19 @@
 DASHBOARD_CONFIG_PATH = CONTENT_TARGET_PATH / "dashboard.yaml"
 # on-host metrics persistent data folder
 METRICS_DATA_PATH = CONTENT_TARGET_PATH / "metrics"
 # on-host metrics transient (tmpfs) log folders (caddy-created)
 KIWIXSERVE_DATA_PATH = CONTENT_TARGET_PATH / "zims"
 METRICS_VAR_LOG_PATH_HOST = Path("/var/log/metrics")
 METRICS_VAR_LOG_PATH_CONT = Path("/var/log/host/metrics")
+# hotspot original branding material (usually kept as untouched)
+ORIGINAL_BRANDING_PATH = DATA_PART_PATH / "branding"
+# actual hotspot branding. default from orig, replaced in builder
+BRANDING_PATH = CONTENT_TARGET_PATH / "branding"
+
 KIWIX_ZIM_LOAD_BALANCER_URL = "https://download.kiwix.org/zim/"
 
 # data source for “internal images” (out of catalog)
 INTERNAL_IMAGES = {
     "captive-portal": {
         "source": "ghcr.io/offspot/captive-portal:1.4.1",
         "filesize": 189911040,
@@ -55,27 +65,27 @@
     },
     "hwclock": {
         "source": "ghcr.io/offspot/hwclock:1.2",
         "filesize": 58951680,
         "fullsize": 58922600,
     },
     "kiwix-serve": {
-        "source": "ghcr.io/offspot/kiwix-serve:3.6.0",
-        "filesize": 62351360,
-        "fullsize": 62313418,
+        "source": "ghcr.io/offspot/kiwix-serve:3.7.0-1",
+        "filesize": 58480640,
+        "fullsize": 58443713,
     },
     "metrics": {
         "source": "ghcr.io/offspot/metrics:0.3.0",
         "filesize": 167311360,
         "fullsize": 167202612,
     },
     "reverse-proxy": {
-        "source": "ghcr.io/offspot/reverse-proxy:1.7",
-        "filesize": 120350720,
-        "fullsize": 120279091,
+        "source": "ghcr.io/offspot/reverse-proxy:1.8",
+        "filesize": 120432640,
+        "fullsize": 120368490,
     },
 }
 
 
 def get_internal_image(ident: str) -> OCIImage:
     """OCI Image from special key identifying internal image"""
     if ident == "file-manager":
@@ -244,14 +254,26 @@
                 },
                 {
                     "type": "bind",
                     "source": f"{CONTENT_TARGET_PATH}/zims",
                     "target": "/data/zims",
                     "read_only": True,
                 },
+                {
+                    "type": "bind",
+                    "source": BRANDING_PATH,
+                    "target": "/var/www/branding",
+                    "read_only": True,
+                },
+                {
+                    "type": "bind",
+                    "source": ORIGINAL_BRANDING_PATH,
+                    "target": "/var/www/offspot.branding",
+                    "read_only": True,
+                },
             ],
         }
 
         # add placeholder file to host fs to ensure bind succeeds
         self.ensure_host_path(KIWIXSERVE_DATA_PATH)
 
     def gen_dashboard_config(self):
@@ -322,15 +344,27 @@
                 # So we bind /var/log (mostly empty on systemd anyway) and the proxy
                 # will create the subfolder to write logs into
                 {
                     "type": "bind",
                     "source": str(METRICS_VAR_LOG_PATH_HOST.parent),
                     "target": str(METRICS_VAR_LOG_PATH_CONT),
                     "read_only": False,
-                }
+                },
+                {
+                    "type": "bind",
+                    "source": BRANDING_PATH,
+                    "target": "/var/www/branding",
+                    "read_only": True,
+                },
+                {
+                    "type": "bind",
+                    "source": ORIGINAL_BRANDING_PATH,
+                    "target": "/var/www/offspot.branding",
+                    "read_only": True,
+                },
             ],
         }
 
     def add_captive_portal(self):
         """enable captive-portal feature. WARN: check doc if you use custom network"""
         if self.with_captive_portal:
             return
@@ -379,15 +413,27 @@
                 # it's a mandatory file to use captive-portal with.
                 # created in base-image
                 {
                     "type": "bind",
                     "source": "/var/run/internet",
                     "target": "/var/run/internet",
                     "read_only": True,
-                }
+                },
+                {
+                    "type": "bind",
+                    "source": BRANDING_PATH,
+                    "target": "/src/portal/branding",
+                    "read_only": True,
+                },
+                {
+                    "type": "bind",
+                    "source": ORIGINAL_BRANDING_PATH,
+                    "target": "/src/portal/offspot.branding",
+                    "read_only": True,
+                },
             ],
         }
 
     def add_metrics(self):
         if self.with_metrics:
             return
 
@@ -437,14 +483,26 @@
                 # mandates its presence on host. taken care of by dashboard
                 {
                     "type": "bind",
                     "source": str(DASHBOARD_CONFIG_PATH),
                     "target": in_container_packages_path,
                     "read_only": True,
                 },
+                {
+                    "type": "bind",
+                    "source": BRANDING_PATH,
+                    "target": "/src/ui/branding",
+                    "read_only": True,
+                },
+                {
+                    "type": "bind",
+                    "source": ORIGINAL_BRANDING_PATH,
+                    "target": "/src/ui/offspot.branding",
+                    "read_only": True,
+                },
             ],
         }
 
         # add persistent metrics (and its logwatcher subfolder) to host for docker bind
         self.ensure_host_path(METRICS_DATA_PATH / "logwatcher")
 
         self.reversed_services.add("metrics")
@@ -464,14 +522,28 @@
             "image": image.source,
             "container_name": "hwclock",
             "pull_policy": "never",
             "read_only": True,
             "restart": "unless-stopped",
             "expose": ["80"],
             "privileged": True,
+            "volumes": [
+                {
+                    "type": "bind",
+                    "source": BRANDING_PATH,
+                    "target": "/src/branding",
+                    "read_only": True,
+                },
+                {
+                    "type": "bind",
+                    "source": ORIGINAL_BRANDING_PATH,
+                    "target": "/src/offspot.branding",
+                    "read_only": True,
+                },
+            ],
         }
 
         self.protected_services.update(
             {
                 "hwclock": (
                     self.environ.get("ADMIN_USERNAME", ""),
                     self.environ.get("ADMIN_PASSWORD", ""),
@@ -519,15 +591,27 @@
                 # mandates presence of this folder on host
                 # thus created below via a placeholder
                 {
                     "type": "bind",
                     "source": f"{CONTENT_TARGET_PATH}/zims",
                     "target": "/data",
                     "read_only": True,
-                }
+                },
+                {
+                    "type": "bind",
+                    "source": BRANDING_PATH,
+                    "target": "/data/branding",
+                    "read_only": True,
+                },
+                {
+                    "type": "bind",
+                    "source": ORIGINAL_BRANDING_PATH,
+                    "target": "/data/offspot.branding",
+                    "read_only": True,
+                },
             ],
             "command": '/bin/sh -c "kiwix-serve --blockexternal '
             '--port 80 --nodatealiases /data/*.zim"',
         }
 
         # add placeholder file to host fs to ensure bind succeeds
         self.ensure_host_path(KIWIXSERVE_DATA_PATH)
@@ -710,15 +794,27 @@
                     # mandates presence of this folder on host
                     # thus created below via a placeholder
                     {
                         "type": "bind",
                         "source": f"{CONTENT_TARGET_PATH}",
                         "target": "/data",
                         "read_only": True,
-                    }
+                    },
+                    {
+                        "type": "bind",
+                        "source": BRANDING_PATH,
+                        "target": "/branding",
+                        "read_only": True,
+                    },
+                    {
+                        "type": "bind",
+                        "source": ORIGINAL_BRANDING_PATH,
+                        "target": "/offspot.branding",
+                        "read_only": True,
+                    },
                 ],
             }
 
             # add placeholder file to host fs to ensure bind succeeds
             self.ensure_host_path(CONTENT_TARGET_PATH)
 
             self.with_files = True
@@ -757,16 +853,19 @@
         """dynamic-variables resolved string"""
 
         # replace $environ{XXX} mappings
         match = RE_ENVIRON_VAR.search(text)
         if match:
             repl = self.environ[match.groupdict()["var"]]
             text = RE_ENVIRON_VAR.sub(repl, text)
-        resolved = text.replace("${FQDN}", self.fqdn).replace(
-            "${REVERSE_NAME}", "reverse-proxy"
+        resolved = (
+            text.replace("${FQDN}", self.fqdn)
+            .replace("${REVERSE_NAME}", "reverse-proxy")
+            .replace("${BRANDING_PATH}", str(BRANDING_PATH))
+            .replace("${ORIGINAL_BRANDING_PATH}", str(ORIGINAL_BRANDING_PATH))
         )
         if package:
             app_dir = get_app_path(package=package)
             resolved = (
                 resolved.replace("${APP_DIR}", app_dir)
                 .replace("${PACKAGE_IDENT}", package.ident)
                 .replace("${PACKAGE_DOMAIN}", package.domain)
@@ -792,15 +891,29 @@
             margin=get_margin_for(content_size),
         )
 
     def render(self) -> str:
         """compute config based on requests"""
         ...
 
-        # add kiwix apps?
+        # add original branding so apps can rely on it
+        self.ensure_host_path(ORIGINAL_BRANDING_PATH)
+        data = b""
+        for fpath in INTERNAL_BRANDING_PATH.iterdir():
+            data = fpath.read_bytes()
+            self.add_file(
+                url_or_content=b64_encode(data),
+                to=str(ORIGINAL_BRANDING_PATH.joinpath(fpath.name)),
+                via="base64",
+                size=len(data),
+            )
+        del data
+
+        # make sure branding folder exists for mounts
+        self.ensure_host_path(BRANDING_PATH)
 
         # gen dashboard.yaml
         if self.with_dashboard:
             self.gen_dashboard_config()
 
         # update reverseproxy config
         # > domain to subfolder for all files packages + zim-dl
```

### Comparing `offspot_config-2.1.0/src/offspot_config/catalog.json` & `offspot_config-2.2.0/src/offspot_config/catalog.json`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_config/catalog.py` & `offspot_config-2.2.0/src/offspot_config/catalog.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_config/constants.py` & `offspot_config-2.2.0/src/offspot_config/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,7 +61,8 @@
     "desktop.ini",
     "Desktop.ini",
     # Recycle Bin used on file shares
     "$RECYCLE.BIN",
     # Windows shortcuts
     "*.lnk",
 )
+INTERNAL_BRANDING_PATH = pathlib.Path(__file__).with_name("branding")
```

### Comparing `offspot_config-2.1.0/src/offspot_config/file.py` & `offspot_config-2.2.0/src/offspot_config/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,31 @@
 
     Created from files entries in config:
     - to: str
         mandatory destination to save file into. Must be inside /data
     - size: optional[int]
         size of (expanded) content. If specified, must be >= source file
     - via: optional[str]
-        method to process source file (not for content). Values in File.unpack_formats
+        method to process source file. Values in File.unpack_formats
+        `base64` value only applies to `content`
+        other values not applicable if there's a `content` value
     - url: optional[str]
         URL to download file from
     - content: optional[str]
         plain text content to write to destination
+        can be base64 encoded (std) in which case via must be `base64`
 
     one of content or url must be supplied. content has priority"""
 
     kind: str = "file"  # Item interface
 
     unpack_formats: list[str]
 
     def __init__(self, payload: dict[str, str | int | dict[str, str]]):
-        self.unpack_formats = ["direct", *SUPPORTED_UNPACKING_FORMATS]
+        self.unpack_formats = ["direct", "base64", *SUPPORTED_UNPACKING_FORMATS]
         self.url: urllib.parse.ParseResult | None = None
         self.to: pathlib.Path = pathlib.Path(str(payload["to"])).resolve()
         self.via: str = str(payload.get("via", "direct"))
         self.content: str = str(payload.get("content", "") or "").strip()
         self.checksum: Checksum | None = None
         self._size = -1
         self._fullsize: int | None = None
@@ -101,14 +104,19 @@
 
     @property
     def is_plain(self) -> bool:
         """whether a plain text content to be written"""
         return bool(self.content)
 
     @property
+    def is_base64_encoded(self) -> bool:
+        """whether a plain text content to be written"""
+        return self.via == "base64"
+
+    @property
     def is_local(self) -> bool:
         """whether referencing a local file"""
         return not self.is_plain and bool(self.url) and self.url.scheme == "file"
 
     @property
     def is_remote(self) -> bool:
         """whether referencing a remote file"""
```

### Comparing `offspot_config-2.1.0/src/offspot_config/oci_images.py` & `offspot_config-2.2.0/src/offspot_config/oci_images.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_config/packages.py` & `offspot_config-2.2.0/src/offspot_config/packages.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_config/zim.py` & `offspot_config-2.2.0/src/offspot_config/zim.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_config/inputs/base.py` & `offspot_config-2.2.0/src/offspot_config/inputs/base.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_config/inputs/checksum.py` & `offspot_config-2.2.0/src/offspot_config/inputs/checksum.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_config/inputs/file.py` & `offspot_config-2.2.0/src/offspot_config/inputs/file.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_config/inputs/mainconfig.py` & `offspot_config-2.2.0/src/offspot_config/inputs/mainconfig.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_config/inputs/output.py` & `offspot_config-2.2.0/src/offspot_config/inputs/output.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_config/utils/dashboard.py` & `offspot_config-2.2.0/src/offspot_config/utils/dashboard.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_config/utils/download.py` & `offspot_config-2.2.0/src/offspot_config/utils/download.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_config/utils/misc.py` & `offspot_config-2.2.0/src/offspot_config/utils/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import base64
 import datetime
 import fnmatch
 import inspect
 import lzma
 import os
 import pathlib
 import platform
@@ -138,14 +139,24 @@
 
     for fpath in dest.rglob("*"):
         for pattern in POST_EXPANSION_UNWANTED_PATTERNS:
             if fnmatch.fnmatch(fpath.name, pattern):
                 fpath.unlink(missing_ok=True)
 
 
+def b64_encode(data: bytes) -> str:
+    """ASCII based64 repr of data"""
+    return base64.standard_b64encode(data).decode("ASCII")
+
+
+def b64_decode(data: str) -> bytes:
+    """ASCII based64 repr of data"""
+    return base64.standard_b64decode(data.encode("ASCII"))
+
+
 class SimpleAttrs:
     """dict-like xattr wrapper to save specifying user. prefix"""
 
     def __init__(self, path: pathlib.Path):
         self.path = path
 
     def __repr__(self):
```

### Comparing `offspot_config-2.1.0/src/offspot_config/utils/sizes.py` & `offspot_config-2.2.0/src/offspot_config/utils/sizes.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_config/utils/yaml.py` & `offspot_config-2.2.0/src/offspot_config/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_runtime/ap.py` & `offspot_config-2.2.0/src/offspot_runtime/ap.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_runtime/checks.py` & `offspot_config-2.2.0/src/offspot_runtime/checks.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_runtime/configlib.py` & `offspot_config-2.2.0/src/offspot_runtime/configlib.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_runtime/containers.py` & `offspot_config-2.2.0/src/offspot_runtime/containers.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_runtime/dnsmasqspoof.py` & `offspot_config-2.2.0/src/offspot_runtime/dnsmasqspoof.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_runtime/ethernet.py` & `offspot_config-2.2.0/src/offspot_runtime/ethernet.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_runtime/firmware.py` & `offspot_config-2.2.0/src/offspot_runtime/firmware.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_runtime/fromfile.py` & `offspot_config-2.2.0/src/offspot_runtime/fromfile.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_runtime/hostname.py` & `offspot_config-2.2.0/src/offspot_runtime/hostname.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/src/offspot_runtime/timezone.py` & `offspot_config-2.2.0/src/offspot_runtime/timezone.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/tests/conftest.py` & `offspot_config-2.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/tests/test_checks.py` & `offspot_config-2.2.0/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/tests/test_humanid.py` & `offspot_config-2.2.0/tests/test_humanid.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/tests/test_inputs.py` & `offspot_config-2.2.0/tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/tests/test_link.py` & `offspot_config-2.2.0/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/tests/test_reader.py` & `offspot_config-2.2.0/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/tests/test_zim.py` & `offspot_config-2.2.0/tests/test_zim.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/.gitignore` & `offspot_config-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/LICENSE` & `offspot_config-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/README.md` & `offspot_config-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/pyproject.toml` & `offspot_config-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `offspot_config-2.1.0/PKG-INFO` & `offspot_config-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: offspot-config
-Version: 2.1.0
+Version: 2.2.0
 Summary: Offspot Config helpers
 Project-URL: Homepage, https://github.com/offspot/offspot-config
 Project-URL: Donate, https://www.kiwix.org/en/support-us/
 Author-email: Kiwix <dev@kiwix.org>
 License: GPL-3.0-or-later
 License-File: LICENSE
 Keywords: offspot
```

