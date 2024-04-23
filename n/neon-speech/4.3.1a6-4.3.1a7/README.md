# Comparing `tmp/neon_speech-4.3.1a6.tar.gz` & `tmp/neon_speech-4.3.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon_speech-4.3.1a6.tar", last modified: Tue Apr 23 19:14:25 2024, max compression
+gzip compressed data, was "neon_speech-4.3.1a7.tar", last modified: Tue Apr 23 21:07:25 2024, max compression
```

## Comparing `neon_speech-4.3.1a6.tar` & `neon_speech-4.3.1a7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:14:25.388106 neon_speech-4.3.1a6/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-23 19:14:19.000000 neon_speech-4.3.1a6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-23 19:14:25.388106 neon_speech-4.3.1a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-23 19:14:19.000000 neon_speech-4.3.1a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:14:25.388106 neon_speech-4.3.1a6/neon_speech/
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-23 19:14:19.000000 neon_speech-4.3.1a6/neon_speech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-23 19:14:19.000000 neon_speech-4.3.1a6/neon_speech/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-04-23 19:14:19.000000 neon_speech-4.3.1a6/neon_speech/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    27197 2024-04-23 19:14:19.000000 neon_speech-4.3.1a6/neon_speech/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-23 19:14:19.000000 neon_speech-4.3.1a6/neon_speech/stt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-23 19:14:19.000000 neon_speech-4.3.1a6/neon_speech/transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-23 19:14:19.000000 neon_speech-4.3.1a6/neon_speech/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:14:25.388106 neon_speech-4.3.1a6/neon_speech.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-23 19:14:25.000000 neon_speech-4.3.1a6/neon_speech.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-23 19:14:25.000000 neon_speech-4.3.1a6/neon_speech.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:14:25.000000 neon_speech-4.3.1a6/neon_speech.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-23 19:14:25.000000 neon_speech-4.3.1a6/neon_speech.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-23 19:14:25.000000 neon_speech-4.3.1a6/neon_speech.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 19:14:25.000000 neon_speech-4.3.1a6/neon_speech.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:14:25.388106 neon_speech-4.3.1a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-23 19:14:19.000000 neon_speech-4.3.1a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:07:25.622680 neon_speech-4.3.1a7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-23 21:07:20.000000 neon_speech-4.3.1a7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-23 21:07:25.622680 neon_speech-4.3.1a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-23 21:07:20.000000 neon_speech-4.3.1a7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:07:25.618680 neon_speech-4.3.1a7/neon_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-23 21:07:20.000000 neon_speech-4.3.1a7/neon_speech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-23 21:07:20.000000 neon_speech-4.3.1a7/neon_speech/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-04-23 21:07:20.000000 neon_speech-4.3.1a7/neon_speech/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27197 2024-04-23 21:07:20.000000 neon_speech-4.3.1a7/neon_speech/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-23 21:07:20.000000 neon_speech-4.3.1a7/neon_speech/stt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-23 21:07:20.000000 neon_speech-4.3.1a7/neon_speech/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-23 21:07:20.000000 neon_speech-4.3.1a7/neon_speech/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:07:25.622680 neon_speech-4.3.1a7/neon_speech.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-23 21:07:25.000000 neon_speech-4.3.1a7/neon_speech.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-23 21:07:25.000000 neon_speech-4.3.1a7/neon_speech.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 21:07:25.000000 neon_speech-4.3.1a7/neon_speech.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-23 21:07:25.000000 neon_speech-4.3.1a7/neon_speech.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-23 21:07:25.000000 neon_speech-4.3.1a7/neon_speech.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 21:07:25.000000 neon_speech-4.3.1a7/neon_speech.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 21:07:25.622680 neon_speech-4.3.1a7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-23 21:07:20.000000 neon_speech-4.3.1a7/setup.py
```

### Comparing `neon_speech-4.3.1a6/LICENSE.md` & `neon_speech-4.3.1a7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon_speech-4.3.1a6/PKG-INFO` & `neon_speech-4.3.1a7/neon_speech.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: neon_speech
-Version: 4.3.1a6
+Name: neon-speech
+Version: 4.3.1a7
 Summary: Neon Speech Module
 Home-page: https://github.com/NeonGeckoCom/neon_speech
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon_speech-4.3.1a6/README.md` & `neon_speech-4.3.1a7/README.md`

 * *Files identical despite different names*

### Comparing `neon_speech-4.3.1a6/neon_speech/__init__.py` & `neon_speech-4.3.1a7/neon_speech/__init__.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.3.1a6/neon_speech/__main__.py` & `neon_speech-4.3.1a7/neon_speech/__main__.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.3.1a6/neon_speech/cli.py` & `neon_speech-4.3.1a7/neon_speech/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,41 +83,43 @@
 @click.option("--module", "-m", default=None,
               help="STT Plugin to configure")
 @click.option("--package", "-p", default=None,
               help="STT package spec to install")
 @click.option("--force-install", "-f", default=False, is_flag=True,
               help="Force pip installation of configured module")
 def install_plugin(module, package, force_install):
-    log_deprecation("`install-plugin` replaced by `install-dependencies`", "2.0.0")
+    log_deprecation("`install-plugin` replaced by `install-dependencies`", "5.0.0")
     from neon_speech.utils import install_stt_plugin
     from ovos_config.config import Configuration
     speech_config = Configuration()
 
     if force_install and not (package or module):
         click.echo("Installing STT plugin from configuration")
         module = module or speech_config.get("stt", {}).get("module")
         package = package or speech_config.get("stt", {}).get("package_spec")
 
     if module:
         install_stt_plugin(package or module)
         if not module:
             click.echo("Plugin specified without module")
 
+
 @neon_speech_cli.command(help="Install neon-speech module dependencies from config & cli")
 @click.option("--package", "-p", default=[], multiple=True,
               help="Additional package to install (can be repeated)")
 def install_dependencies(package: List[str]):
     from neon_utils.packaging_utils import install_packages_from_pip
     from neon_speech.utils import build_extra_dependency_list
     config = Configuration()
     dependencies = build_extra_dependency_list(config, list(package))
     result = install_packages_from_pip("neon-speech", dependencies)
     LOG.info(f"pip exit code: {result}")
     sys.exit(result)
 
+
 @neon_speech_cli.command(help="Install a STT Plugin")
 @click.option("--plugin", "-p", default=None,
               help="STT module to init")
 def init_plugin(plugin):
     from neon_speech.utils import init_stt_plugin
     from ovos_config.config import Configuration
     plugin = plugin or Configuration().get("stt", {}).get("module")
```

### Comparing `neon_speech-4.3.1a6/neon_speech/service.py` & `neon_speech-4.3.1a7/neon_speech/service.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.3.1a6/neon_speech/stt.py` & `neon_speech-4.3.1a7/neon_speech/stt.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.3.1a6/neon_speech/transformers.py` & `neon_speech-4.3.1a7/neon_speech/transformers.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.3.1a6/neon_speech/utils.py` & `neon_speech-4.3.1a7/neon_speech/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,21 +56,23 @@
     known_plugins = {
         "deepspeech_stream_local": "neon-stt-plugin-deepspeech-stream-local",
         "polyglot": "neon-stt-plugin-polyglot",
         "google_cloud_streaming": "neon-stt-plugin-google-cloud-streaming",
     }
     return known_plugins.get(plugin) or plugin
 
+
 def build_extra_dependency_list(config: Union[dict, Configuration], additional: List[str] = []) -> List[str]:
     extra_dependencies = config.get("extra_dependencies", {})
     dependencies = additional + extra_dependencies.get("global", []) + extra_dependencies.get("voice", [])
 
     return dependencies
 
-@deprecated("Replaced by `neon_utils.packaging_utils.install_packages_from_pip`", "2.0.0")
+
+@deprecated("Replaced by `neon_utils.packaging_utils.install_packages_from_pip`", "5.0.0")
 def install_stt_plugin(plugin: str) -> bool:
     """
     Install an stt plugin using pip
     :param plugin: entrypoint of plugin to install
     :returns: True if the plugin installation is successful
     """
     import pip
```

### Comparing `neon_speech-4.3.1a6/neon_speech.egg-info/PKG-INFO` & `neon_speech-4.3.1a7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: neon-speech
-Version: 4.3.1a6
+Name: neon_speech
+Version: 4.3.1a7
 Summary: Neon Speech Module
 Home-page: https://github.com/NeonGeckoCom/neon_speech
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon_speech-4.3.1a6/setup.py` & `neon_speech-4.3.1a7/setup.py`

 * *Files identical despite different names*

