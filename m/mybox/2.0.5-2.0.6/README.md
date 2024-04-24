# Comparing `tmp/mybox-2.0.5.tar.gz` & `tmp/mybox-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mybox-2.0.5.tar", max compression
+gzip compressed data, was "mybox-2.0.6.tar", max compression
```

## Comparing `mybox-2.0.5.tar` & `mybox-2.0.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    34916 2024-04-13 00:43:12.598719 mybox-2.0.5/LICENSE.md
--rw-r--r--   0        0        0     1447 2024-04-13 00:43:12.598719 mybox-2.0.5/README.md
--rw-r--r--   0        0        0        0 2024-04-13 00:43:12.598719 mybox-2.0.5/mybox/__init__.py
--rw-r--r--   0        0        0     2621 2024-04-13 00:43:12.598719 mybox-2.0.5/mybox/compute.py
--rw-r--r--   0        0        0      741 2024-04-13 00:43:12.598719 mybox-2.0.5/mybox/configparser.py
--rw-r--r--   0        0        0    10638 2024-04-13 00:43:12.598719 mybox-2.0.5/mybox/driver.py
--rw-r--r--   0        0        0     3325 2024-04-13 00:43:12.598719 mybox-2.0.5/mybox/extractor.py
--rw-r--r--   0        0        0     2800 2024-04-13 00:43:12.598719 mybox-2.0.5/mybox/filters.py
--rw-r--r--   0        0        0     1302 2024-04-13 00:43:12.598719 mybox-2.0.5/mybox/main.py
--rw-r--r--   0        0        0     3098 2024-04-13 00:43:12.598719 mybox-2.0.5/mybox/manager.py
--rw-r--r--   0        0        0     1137 2024-04-13 00:43:12.598719 mybox-2.0.5/mybox/package/__init__.py
--rw-r--r--   0        0        0     4064 2024-04-13 00:43:12.598719 mybox-2.0.5/mybox/package/archive.py
--rw-r--r--   0        0        0     2055 2024-04-13 00:43:12.598719 mybox-2.0.5/mybox/package/base.py
--rw-r--r--   0        0        0     1008 2024-04-13 00:43:12.598719 mybox-2.0.5/mybox/package/brew_repo.py
--rw-r--r--   0        0        0     1957 2024-04-13 00:43:12.598719 mybox-2.0.5/mybox/package/clone.py
--rw-r--r--   0        0        0      339 2024-04-13 00:43:12.598719 mybox-2.0.5/mybox/package/destination.py
--rw-r--r--   0        0        0     4714 2024-04-13 00:43:12.598719 mybox-2.0.5/mybox/package/github.py
--rw-r--r--   0        0        0     9851 2024-04-13 00:43:12.598719 mybox-2.0.5/mybox/package/installer.py
--rw-r--r--   0        0        0     1939 2024-04-13 00:43:12.598719 mybox-2.0.5/mybox/package/links.py
--rw-r--r--   0        0        0     4774 2024-04-13 00:43:12.598719 mybox-2.0.5/mybox/package/manual.py
--rw-r--r--   0        0        0      858 2024-04-13 00:43:12.598719 mybox-2.0.5/mybox/package/manual_version.py
--rw-r--r--   0        0        0     1793 2024-04-13 00:43:12.598719 mybox-2.0.5/mybox/package/npm.py
--rw-r--r--   0        0        0     2963 2024-04-13 00:43:12.598719 mybox-2.0.5/mybox/package/pipx.py
--rw-r--r--   0        0        0      500 2024-04-13 00:43:12.602719 mybox-2.0.5/mybox/package/root.py
--rw-r--r--   0        0        0     1853 2024-04-13 00:43:12.602719 mybox-2.0.5/mybox/package/shell.py
--rw-r--r--   0        0        0     2389 2024-04-13 00:43:12.602719 mybox-2.0.5/mybox/package/system.py
--rw-r--r--   0        0        0      959 2024-04-13 00:43:12.602719 mybox-2.0.5/mybox/package/url.py
--rw-r--r--   0        0        0     1762 2024-04-13 00:43:12.602719 mybox-2.0.5/mybox/package/yum_repo.py
--rw-r--r--   0        0        0     2900 2024-04-13 00:43:12.602719 mybox-2.0.5/mybox/parallel.py
--rw-r--r--   0        0        0      156 2024-04-13 00:43:12.602719 mybox-2.0.5/mybox/state/__init__.py
--rw-r--r--   0        0        0     3677 2024-04-13 00:43:12.602719 mybox-2.0.5/mybox/state/base.py
--rw-r--r--   0        0        0     1546 2024-04-13 00:43:12.602719 mybox-2.0.5/mybox/state/db.py
--rw-r--r--   0        0        0      315 2024-04-13 00:43:12.602719 mybox-2.0.5/mybox/state/installed.py
--rw-r--r--   0        0        0      160 2024-04-13 00:43:12.602719 mybox-2.0.5/mybox/state/version.py
--rw-r--r--   0        0        0     2176 2024-04-13 00:43:12.602719 mybox-2.0.5/mybox/tracker.py
--rw-r--r--   0        0        0     3969 2024-04-13 00:43:12.602719 mybox-2.0.5/mybox/utils.py
--rw-r--r--   0        0        0     2099 2024-04-13 00:44:07.399253 mybox-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 mybox-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0    34916 2024-04-24 04:57:43.208145 mybox-2.0.6/LICENSE.md
+-rw-r--r--   0        0        0     1447 2024-04-24 04:57:43.208145 mybox-2.0.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/__init__.py
+-rw-r--r--   0        0        0     2621 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/compute.py
+-rw-r--r--   0        0        0      741 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/configparser.py
+-rw-r--r--   0        0        0    10638 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/driver.py
+-rw-r--r--   0        0        0     3325 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/extractor.py
+-rw-r--r--   0        0        0     2800 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/filters.py
+-rw-r--r--   0        0        0     1302 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/main.py
+-rw-r--r--   0        0        0     3098 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/manager.py
+-rw-r--r--   0        0        0     1137 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/package/__init__.py
+-rw-r--r--   0        0        0     4064 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/package/archive.py
+-rw-r--r--   0        0        0     2055 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/package/base.py
+-rw-r--r--   0        0        0     1008 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/package/brew_repo.py
+-rw-r--r--   0        0        0     1957 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/package/clone.py
+-rw-r--r--   0        0        0      339 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/package/destination.py
+-rw-r--r--   0        0        0     4714 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/package/github.py
+-rw-r--r--   0        0        0    10013 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/package/installer.py
+-rw-r--r--   0        0        0     1939 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/package/links.py
+-rw-r--r--   0        0        0     4774 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/package/manual.py
+-rw-r--r--   0        0        0      858 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/package/manual_version.py
+-rw-r--r--   0        0        0     1793 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/package/npm.py
+-rw-r--r--   0        0        0     2963 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/package/pipx.py
+-rw-r--r--   0        0        0      500 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/package/root.py
+-rw-r--r--   0        0        0     1853 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/package/shell.py
+-rw-r--r--   0        0        0     2389 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/package/system.py
+-rw-r--r--   0        0        0      959 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/package/url.py
+-rw-r--r--   0        0        0     1762 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/package/yum_repo.py
+-rw-r--r--   0        0        0     2900 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/parallel.py
+-rw-r--r--   0        0        0      156 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/state/__init__.py
+-rw-r--r--   0        0        0     3677 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/state/base.py
+-rw-r--r--   0        0        0     1546 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/state/db.py
+-rw-r--r--   0        0        0      315 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/state/installed.py
+-rw-r--r--   0        0        0      160 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/state/version.py
+-rw-r--r--   0        0        0     2176 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/tracker.py
+-rw-r--r--   0        0        0     3969 2024-04-24 04:57:43.208145 mybox-2.0.6/mybox/utils.py
+-rw-r--r--   0        0        0     2099 2024-04-24 04:58:17.132187 mybox-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 mybox-2.0.6/PKG-INFO
```

### Comparing `mybox-2.0.5/LICENSE.md` & `mybox-2.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/README.md` & `mybox-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/compute.py` & `mybox-2.0.6/mybox/compute.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/configparser.py` & `mybox-2.0.6/mybox/configparser.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/driver.py` & `mybox-2.0.6/mybox/driver.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/extractor.py` & `mybox-2.0.6/mybox/extractor.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/filters.py` & `mybox-2.0.6/mybox/filters.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/main.py` & `mybox-2.0.6/mybox/main.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/manager.py` & `mybox-2.0.6/mybox/manager.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/package/__init__.py` & `mybox-2.0.6/mybox/package/__init__.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/package/archive.py` & `mybox-2.0.6/mybox/package/archive.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/package/base.py` & `mybox-2.0.6/mybox/package/base.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/package/brew_repo.py` & `mybox-2.0.6/mybox/package/brew_repo.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/package/clone.py` & `mybox-2.0.6/mybox/package/clone.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/package/github.py` & `mybox-2.0.6/mybox/package/github.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/package/installer.py` & `mybox-2.0.6/mybox/package/installer.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,25 +78,27 @@
             if self.cache:
                 self.cache.pop(package, None)
 
     async def install(self, package: str) -> None:
         await super().install(package)
         await self.invalidate_cache(package)
 
-    async def upgrade(self, package: str) -> None:
+    async def upgrade(self, package: str) -> None:  # pragma: no cover
+        # Can't install an old version of a package in tests
         await super().upgrade(package)
         await self.invalidate_cache(package)
 
 
 class Brew(PackageCacheInstaller):
     async def install(self, package: str) -> None:
         await self.driver.run(await self.brew(), "install", package)
         await super().install(package)
 
-    async def upgrade(self, package: str) -> None:
+    async def upgrade(self, package: str) -> None:  # pragma: no cover
+        # Can't install an old version of a package in tests
         await self.driver.run(await self.brew(), "upgrade", package)
         await super().upgrade(package)
 
     async def tap(self, repo: str) -> None:
         await self.driver.run(await self.brew(), "tap", repo)
 
     async def tapped(self) -> set[str]:
```

### Comparing `mybox-2.0.5/mybox/package/links.py` & `mybox-2.0.6/mybox/package/links.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/package/manual.py` & `mybox-2.0.6/mybox/package/manual.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/package/manual_version.py` & `mybox-2.0.6/mybox/package/manual_version.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/package/npm.py` & `mybox-2.0.6/mybox/package/npm.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/package/pipx.py` & `mybox-2.0.6/mybox/package/pipx.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/package/shell.py` & `mybox-2.0.6/mybox/package/shell.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/package/system.py` & `mybox-2.0.6/mybox/package/system.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/package/url.py` & `mybox-2.0.6/mybox/package/url.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/package/yum_repo.py` & `mybox-2.0.6/mybox/package/yum_repo.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/parallel.py` & `mybox-2.0.6/mybox/parallel.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/state/base.py` & `mybox-2.0.6/mybox/state/base.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/state/db.py` & `mybox-2.0.6/mybox/state/db.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/tracker.py` & `mybox-2.0.6/mybox/tracker.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/mybox/utils.py` & `mybox-2.0.6/mybox/utils.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.5/pyproject.toml` & `mybox-2.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mybox"
-version = "2.0.5"
+version = "2.0.6"
 description = "Manage the configuration and tools on your workstation without bothering the OS too much"
 readme = "README.md"
 repository = "https://github.com/koterpillar/mybox"
 authors = ["Alexey Kotlyarov <a@koterpillar.com>"]
 license = "GPL-3.0-or-later"
 
 [tool.poetry.dependencies]
```

### Comparing `mybox-2.0.5/PKG-INFO` & `mybox-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mybox
-Version: 2.0.5
+Version: 2.0.6
 Summary: Manage the configuration and tools on your workstation without bothering the OS too much
 Home-page: https://github.com/koterpillar/mybox
 License: GPL-3.0-or-later
 Author: Alexey Kotlyarov
 Author-email: a@koterpillar.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

