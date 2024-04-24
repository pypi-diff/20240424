# Comparing `tmp/python_recentx-1.4.1.tar.gz` & `tmp/python_recentx-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_recentx-1.4.1.tar", max compression
+gzip compressed data, was "python_recentx-1.4.2.tar", max compression
```

## Comparing `python_recentx-1.4.1.tar` & `python_recentx-1.4.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     1114 2024-04-24 08:53:19.000000 python_recentx-1.4.1/LICENSE
--rw-r--r--   0        0        0     7334 2024-04-24 08:58:54.000000 python_recentx-1.4.1/README.md
--rw-r--r--   0        0        0        0 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/__init__.py
--rw-r--r--   0        0        0    15261 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/asyncio.py
--rw-r--r--   0        0        0      206 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/base.py
--rw-r--r--   0        0        0     6048 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/browser.py
--rw-r--r--   0        0        0      234 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/README.md
--rw-r--r--   0        0        0      732 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/__init__.py
--rw-r--r--   0        0        0    23089 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/accessibility.py
--rw-r--r--   0        0        0    11444 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/animation.py
--rw-r--r--   0        0        0    54218 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/audits.py
--rw-r--r--   0        0        0     3586 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/autofill.py
--rw-r--r--   0        0        0     6073 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/background_service.py
--rw-r--r--   0        0        0    21953 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/browser.py
--rw-r--r--   0        0        0     9245 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/cache_storage.py
--rw-r--r--   0        0        0     4453 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/cast.py
--rw-r--r--   0        0        0     2886 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/console.py
--rw-r--r--   0        0        0    67281 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/css.py
--rw-r--r--   0        0        0     4090 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/database.py
--rw-r--r--   0        0        0    50929 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/debugger.py
--rw-r--r--   0        0        0     3381 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/device_access.py
--rw-r--r--   0        0        0     1211 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/device_orientation.py
--rw-r--r--   0        0        0    63055 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/dom.py
--rw-r--r--   0        0        0     9644 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/dom_debugger.py
--rw-r--r--   0        0        0    38667 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/dom_snapshot.py
--rw-r--r--   0        0        0     5861 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/dom_storage.py
--rw-r--r--   0        0        0    26693 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/emulation.py
--rw-r--r--   0        0        0     1291 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/event_breakpoints.py
--rw-r--r--   0        0        0     5768 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/fed_cm.py
--rw-r--r--   0        0        0    20450 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/fetch.py
--rw-r--r--   0        0        0     4941 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/headless_experimental.py
--rw-r--r--   0        0        0    14064 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/heap_profiler.py
--rw-r--r--   0        0        0    17634 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/indexed_db.py
--rw-r--r--   0        0        0    28548 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/input_.py
--rw-r--r--   0        0        0     1720 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/inspector.py
--rw-r--r--   0        0        0     3047 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/io.py
--rw-r--r--   0        0        0    15572 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/layer_tree.py
--rw-r--r--   0        0        0     5520 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/log.py
--rw-r--r--   0        0        0     7928 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/media.py
--rw-r--r--   0        0        0     7014 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/memory.py
--rw-r--r--   0        0        0   133854 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/network.py
--rw-r--r--   0        0        0    52885 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/overlay.py
--rw-r--r--   0        0        0   110499 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/page.py
--rw-r--r--   0        0        0     3090 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/performance.py
--rw-r--r--   0        0        0     7013 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/performance_timeline.py
--rw-r--r--   0        0        0    20254 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/preload.py
--rw-r--r--   0        0        0    13439 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/profiler.py
--rw-r--r--   0        0        0        0 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/py.typed
--rw-r--r--   0        0        0    64384 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/runtime.py
--rw-r--r--   0        0        0     1164 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/schema.py
--rw-r--r--   0        0        0    17694 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/security.py
--rw-r--r--   0        0        0    11444 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/service_worker.py
--rw-r--r--   0        0        0    45041 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/storage.py
--rw-r--r--   0        0        0    12099 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/system_info.py
--rw-r--r--   0        0        0    24568 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/target.py
--rw-r--r--   0        0        0     1540 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/tethering.py
--rw-r--r--   0        0        0    13459 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/tracing.py
--rw-r--r--   0        0        0      454 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/util.py
--rw-r--r--   0        0        0    17483 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/web_audio.py
--rw-r--r--   0        0        0    16125 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/cdp/web_authn.py
--rw-r--r--   0        0        0     1196 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/exceptions.py
--rw-r--r--   0        0        0     3147 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/gen/README.md
--rw-r--r--   0        0        0        0 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/gen/__init__.py
--rw-r--r--   0        0        0  1083602 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/gen/browser_protocol.json
--rw-r--r--   0        0        0    36994 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/gen/generate.py
--rw-r--r--   0        0        0   179101 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/gen/js_protocol.json
--rw-r--r--   0        0        0    33263 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/gen/test_generate.py
--rw-r--r--   0        0        0    12078 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/twisted.py
--rw-r--r--   0        0        0    12112 2024-04-24 08:53:19.000000 python_recentx-1.4.1/pycdp/utils.py
--rw-r--r--   0        0        0      972 2024-04-24 09:11:46.101785 python_recentx-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     8277 1970-01-01 00:00:00.000000 python_recentx-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1114 2024-04-24 08:53:19.000000 python_recentx-1.4.2/LICENSE
+-rw-r--r--   0        0        0     7334 2024-04-24 08:58:54.000000 python_recentx-1.4.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/__init__.py
+-rw-r--r--   0        0        0    15261 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/asyncio.py
+-rw-r--r--   0        0        0      206 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/base.py
+-rw-r--r--   0        0        0     6048 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/browser.py
+-rw-r--r--   0        0        0      234 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/README.md
+-rw-r--r--   0        0        0      732 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/__init__.py
+-rw-r--r--   0        0        0    23089 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/accessibility.py
+-rw-r--r--   0        0        0    11444 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/animation.py
+-rw-r--r--   0        0        0    54218 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/audits.py
+-rw-r--r--   0        0        0     3586 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/autofill.py
+-rw-r--r--   0        0        0     6073 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/background_service.py
+-rw-r--r--   0        0        0    21953 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/browser.py
+-rw-r--r--   0        0        0     9245 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/cache_storage.py
+-rw-r--r--   0        0        0     4453 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/cast.py
+-rw-r--r--   0        0        0     2886 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/console.py
+-rw-r--r--   0        0        0    67281 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/css.py
+-rw-r--r--   0        0        0     4090 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/database.py
+-rw-r--r--   0        0        0    50929 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/debugger.py
+-rw-r--r--   0        0        0     3381 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/device_access.py
+-rw-r--r--   0        0        0     1211 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/device_orientation.py
+-rw-r--r--   0        0        0    63055 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/dom.py
+-rw-r--r--   0        0        0     9644 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/dom_debugger.py
+-rw-r--r--   0        0        0    38667 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/dom_snapshot.py
+-rw-r--r--   0        0        0     5861 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/dom_storage.py
+-rw-r--r--   0        0        0    26693 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/emulation.py
+-rw-r--r--   0        0        0     1291 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/event_breakpoints.py
+-rw-r--r--   0        0        0     5768 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/fed_cm.py
+-rw-r--r--   0        0        0    20450 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/fetch.py
+-rw-r--r--   0        0        0     4941 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/headless_experimental.py
+-rw-r--r--   0        0        0    14064 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/heap_profiler.py
+-rw-r--r--   0        0        0    17634 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/indexed_db.py
+-rw-r--r--   0        0        0    28548 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/input_.py
+-rw-r--r--   0        0        0     1720 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/inspector.py
+-rw-r--r--   0        0        0     3047 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/io.py
+-rw-r--r--   0        0        0    15572 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/layer_tree.py
+-rw-r--r--   0        0        0     5520 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/log.py
+-rw-r--r--   0        0        0     7928 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/media.py
+-rw-r--r--   0        0        0     7014 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/memory.py
+-rw-r--r--   0        0        0   133854 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/network.py
+-rw-r--r--   0        0        0    52885 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/overlay.py
+-rw-r--r--   0        0        0   110499 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/page.py
+-rw-r--r--   0        0        0     3090 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/performance.py
+-rw-r--r--   0        0        0     7013 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/performance_timeline.py
+-rw-r--r--   0        0        0    20254 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/preload.py
+-rw-r--r--   0        0        0    13439 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/profiler.py
+-rw-r--r--   0        0        0        0 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/py.typed
+-rw-r--r--   0        0        0    64384 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/runtime.py
+-rw-r--r--   0        0        0     1164 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/schema.py
+-rw-r--r--   0        0        0    17694 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/security.py
+-rw-r--r--   0        0        0    11444 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/service_worker.py
+-rw-r--r--   0        0        0    45041 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/storage.py
+-rw-r--r--   0        0        0    12099 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/system_info.py
+-rw-r--r--   0        0        0    24568 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/target.py
+-rw-r--r--   0        0        0     1540 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/tethering.py
+-rw-r--r--   0        0        0    13459 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/tracing.py
+-rw-r--r--   0        0        0      454 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/util.py
+-rw-r--r--   0        0        0    17483 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/web_audio.py
+-rw-r--r--   0        0        0    16125 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/cdp/web_authn.py
+-rw-r--r--   0        0        0     1196 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/exceptions.py
+-rw-r--r--   0        0        0     3147 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/gen/README.md
+-rw-r--r--   0        0        0        0 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/gen/__init__.py
+-rw-r--r--   0        0        0  1083602 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/gen/browser_protocol.json
+-rw-r--r--   0        0        0    36994 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/gen/generate.py
+-rw-r--r--   0        0        0   179101 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/gen/js_protocol.json
+-rw-r--r--   0        0        0    33263 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/gen/test_generate.py
+-rw-r--r--   0        0        0    12078 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/twisted.py
+-rw-r--r--   0        0        0    12112 2024-04-24 08:53:19.000000 python_recentx-1.4.2/pycdp/utils.py
+-rw-r--r--   0        0        0      954 2024-04-24 09:15:08.525600 python_recentx-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     8244 1970-01-01 00:00:00.000000 python_recentx-1.4.2/PKG-INFO
```

### Comparing `python_recentx-1.4.1/LICENSE` & `python_recentx-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/README.md` & `python_recentx-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/asyncio.py` & `python_recentx-1.4.2/pycdp/asyncio.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/browser.py` & `python_recentx-1.4.2/pycdp/browser.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/__init__.py` & `python_recentx-1.4.2/pycdp/cdp/__init__.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/accessibility.py` & `python_recentx-1.4.2/pycdp/cdp/accessibility.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/animation.py` & `python_recentx-1.4.2/pycdp/cdp/animation.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/audits.py` & `python_recentx-1.4.2/pycdp/cdp/audits.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/autofill.py` & `python_recentx-1.4.2/pycdp/cdp/autofill.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/background_service.py` & `python_recentx-1.4.2/pycdp/cdp/background_service.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/browser.py` & `python_recentx-1.4.2/pycdp/cdp/browser.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/cache_storage.py` & `python_recentx-1.4.2/pycdp/cdp/cache_storage.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/cast.py` & `python_recentx-1.4.2/pycdp/cdp/cast.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/console.py` & `python_recentx-1.4.2/pycdp/cdp/console.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/css.py` & `python_recentx-1.4.2/pycdp/cdp/css.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/database.py` & `python_recentx-1.4.2/pycdp/cdp/database.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/debugger.py` & `python_recentx-1.4.2/pycdp/cdp/debugger.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/device_access.py` & `python_recentx-1.4.2/pycdp/cdp/device_access.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/device_orientation.py` & `python_recentx-1.4.2/pycdp/cdp/device_orientation.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/dom.py` & `python_recentx-1.4.2/pycdp/cdp/dom.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/dom_debugger.py` & `python_recentx-1.4.2/pycdp/cdp/dom_debugger.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/dom_snapshot.py` & `python_recentx-1.4.2/pycdp/cdp/dom_snapshot.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/dom_storage.py` & `python_recentx-1.4.2/pycdp/cdp/dom_storage.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/emulation.py` & `python_recentx-1.4.2/pycdp/cdp/emulation.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/event_breakpoints.py` & `python_recentx-1.4.2/pycdp/cdp/event_breakpoints.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/fed_cm.py` & `python_recentx-1.4.2/pycdp/cdp/fed_cm.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/fetch.py` & `python_recentx-1.4.2/pycdp/cdp/fetch.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/headless_experimental.py` & `python_recentx-1.4.2/pycdp/cdp/headless_experimental.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/heap_profiler.py` & `python_recentx-1.4.2/pycdp/cdp/heap_profiler.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/indexed_db.py` & `python_recentx-1.4.2/pycdp/cdp/indexed_db.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/input_.py` & `python_recentx-1.4.2/pycdp/cdp/input_.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/inspector.py` & `python_recentx-1.4.2/pycdp/cdp/inspector.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/io.py` & `python_recentx-1.4.2/pycdp/cdp/io.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/layer_tree.py` & `python_recentx-1.4.2/pycdp/cdp/layer_tree.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/log.py` & `python_recentx-1.4.2/pycdp/cdp/log.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/media.py` & `python_recentx-1.4.2/pycdp/cdp/media.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/memory.py` & `python_recentx-1.4.2/pycdp/cdp/memory.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/network.py` & `python_recentx-1.4.2/pycdp/cdp/network.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/overlay.py` & `python_recentx-1.4.2/pycdp/cdp/overlay.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/page.py` & `python_recentx-1.4.2/pycdp/cdp/page.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/performance.py` & `python_recentx-1.4.2/pycdp/cdp/performance.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/performance_timeline.py` & `python_recentx-1.4.2/pycdp/cdp/performance_timeline.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/preload.py` & `python_recentx-1.4.2/pycdp/cdp/preload.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/profiler.py` & `python_recentx-1.4.2/pycdp/cdp/profiler.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/runtime.py` & `python_recentx-1.4.2/pycdp/cdp/runtime.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/schema.py` & `python_recentx-1.4.2/pycdp/cdp/schema.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/security.py` & `python_recentx-1.4.2/pycdp/cdp/security.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/service_worker.py` & `python_recentx-1.4.2/pycdp/cdp/service_worker.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/storage.py` & `python_recentx-1.4.2/pycdp/cdp/storage.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/system_info.py` & `python_recentx-1.4.2/pycdp/cdp/system_info.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/target.py` & `python_recentx-1.4.2/pycdp/cdp/target.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/tethering.py` & `python_recentx-1.4.2/pycdp/cdp/tethering.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/tracing.py` & `python_recentx-1.4.2/pycdp/cdp/tracing.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/web_audio.py` & `python_recentx-1.4.2/pycdp/cdp/web_audio.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/cdp/web_authn.py` & `python_recentx-1.4.2/pycdp/cdp/web_authn.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/exceptions.py` & `python_recentx-1.4.2/pycdp/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/gen/README.md` & `python_recentx-1.4.2/pycdp/gen/README.md`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/gen/browser_protocol.json` & `python_recentx-1.4.2/pycdp/gen/browser_protocol.json`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/gen/generate.py` & `python_recentx-1.4.2/pycdp/gen/generate.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/gen/js_protocol.json` & `python_recentx-1.4.2/pycdp/gen/js_protocol.json`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/gen/test_generate.py` & `python_recentx-1.4.2/pycdp/gen/test_generate.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/twisted.py` & `python_recentx-1.4.2/pycdp/twisted.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pycdp/utils.py` & `python_recentx-1.4.2/pycdp/utils.py`

 * *Files identical despite different names*

### Comparing `python_recentx-1.4.1/pyproject.toml` & `python_recentx-1.4.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-recentx"
-version = "1.4.1"
+version = "1.4.2"
 description = "Python type wrappers for Chrome DevTools Protocol (CDP)"
 packages = [
     {include = "pycdp"}
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/HMaker/python-recentx"
@@ -20,15 +20,14 @@
     "Heraldo Lucena <heraldo.dev@gmail.com>"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 deprecated = "1.2.9"
 inflection = "0.4.0"
-aiohttp = "3.8.3"
 
 [tool.poetry.dev-dependencies]
 mypy = "^0.770"
 pytest = "^5.4.1"
 sphinx = "^3.0.1"
 sphinx-autodoc-typehints = "^1.10.3"
 sphinx-rtd-theme = "^0.4.3"
```

### Comparing `python_recentx-1.4.1/PKG-INFO` & `python_recentx-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-recentx
-Version: 1.4.1
+Version: 1.4.2
 Summary: Python type wrappers for Chrome DevTools Protocol (CDP)
 Home-page: https://github.com/HMaker/python-recentx
 License: MIT
 Author: Mark E. Haase
 Author-email: mehaase@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -14,15 +14,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet
-Requires-Dist: aiohttp (==3.8.3)
 Requires-Dist: deprecated (==1.2.9)
 Requires-Dist: inflection (==0.4.0)
 Description-Content-Type: text/markdown
 
 # Python CDP
 #### Currently supports CDP [r1179426][2] (Chrome 117).
```

