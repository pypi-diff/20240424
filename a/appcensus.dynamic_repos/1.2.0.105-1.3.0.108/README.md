# Comparing `tmp/appcensus_dynamic_repos-1.2.0.105.tar.gz` & `tmp/appcensus_dynamic_repos-1.3.0.108.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appcensus_dynamic_repos-1.2.0.105.tar", max compression
+gzip compressed data, was "appcensus_dynamic_repos-1.3.0.108.tar", max compression
```

## Comparing `appcensus_dynamic_repos-1.2.0.105.tar` & `appcensus_dynamic_repos-1.3.0.108.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2024-03-07 15:08:54.853967 appcensus_dynamic_repos-1.2.0.105/README-public.md
--rwxr-xr-x   0        0        0     5003 2024-03-07 15:09:05.493980 appcensus_dynamic_repos-1.2.0.105/pyproject.toml
--rw-r--r--   0        0        0      965 2024-03-07 15:08:54.857967 appcensus_dynamic_repos-1.2.0.105/src/appcensus/dynamic_repos/__init__.py
--rw-r--r--   0        0        0     6744 2024-03-07 15:08:54.857967 appcensus_dynamic_repos-1.2.0.105/src/appcensus/dynamic_repos/auth.py
--rw-r--r--   0        0        0    10607 2024-03-07 15:08:54.857967 appcensus_dynamic_repos-1.2.0.105/src/appcensus/dynamic_repos/commands.py
--rw-r--r--   0        0        0     6537 2024-03-07 15:08:54.857967 appcensus_dynamic_repos-1.2.0.105/src/appcensus/dynamic_repos/models.py
--rw-r--r--   0        0        0     5563 2024-03-07 15:08:54.857967 appcensus_dynamic_repos-1.2.0.105/src/appcensus/dynamic_repos/plugin.py
--rw-r--r--   0        0        0     2085 2024-03-07 15:08:54.857967 appcensus_dynamic_repos-1.2.0.105/src/appcensus/dynamic_repos/repo_collector.py
--rw-r--r--   0        0        0     1898 2024-03-07 15:08:54.857967 appcensus_dynamic_repos-1.2.0.105/src/appcensus/dynamic_repos/source_manager.py
--rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 appcensus_dynamic_repos-1.2.0.105/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-24 19:55:05.954150 appcensus_dynamic_repos-1.3.0.108/README-public.md
+-rwxr-xr-x   0        0        0     5003 2024-04-24 19:55:10.038172 appcensus_dynamic_repos-1.3.0.108/pyproject.toml
+-rw-r--r--   0        0        0      965 2024-04-24 19:55:05.958150 appcensus_dynamic_repos-1.3.0.108/src/appcensus/dynamic_repos/__init__.py
+-rw-r--r--   0        0        0     6744 2024-04-24 19:55:05.958150 appcensus_dynamic_repos-1.3.0.108/src/appcensus/dynamic_repos/auth.py
+-rw-r--r--   0        0        0     9868 2024-04-24 19:55:05.958150 appcensus_dynamic_repos-1.3.0.108/src/appcensus/dynamic_repos/commands.py
+-rw-r--r--   0        0        0     6537 2024-04-24 19:55:05.958150 appcensus_dynamic_repos-1.3.0.108/src/appcensus/dynamic_repos/models.py
+-rw-r--r--   0        0        0     5563 2024-04-24 19:55:05.958150 appcensus_dynamic_repos-1.3.0.108/src/appcensus/dynamic_repos/plugin.py
+-rw-r--r--   0        0        0     2089 2024-04-24 19:55:05.958150 appcensus_dynamic_repos-1.3.0.108/src/appcensus/dynamic_repos/repo_collector.py
+-rw-r--r--   0        0        0     1898 2024-04-24 19:55:05.958150 appcensus_dynamic_repos-1.3.0.108/src/appcensus/dynamic_repos/source_manager.py
+-rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 appcensus_dynamic_repos-1.3.0.108/PKG-INFO
```

### Comparing `appcensus_dynamic_repos-1.2.0.105/pyproject.toml` & `appcensus_dynamic_repos-1.3.0.108/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "appcensus.dynamic_repos"
-version = "1.2.0.105"
+version = "1.3.0.108"
 description = "Dynamic Poetry Repositories for AppCensus"
 authors = ["AppCensus <engineering@appcensus.io>"]
 license = "(c) 2022 App Census - All Rights Reserved"
 readme = "README-public.md"
 packages = [{include = "appcensus", from = 'src'}]
 
 [tool.poetry.dependencies]
```

### Comparing `appcensus_dynamic_repos-1.2.0.105/src/appcensus/dynamic_repos/__init__.py` & `appcensus_dynamic_repos-1.3.0.108/src/appcensus/dynamic_repos/__init__.py`

 * *Files identical despite different names*

### Comparing `appcensus_dynamic_repos-1.2.0.105/src/appcensus/dynamic_repos/auth.py` & `appcensus_dynamic_repos-1.3.0.108/src/appcensus/dynamic_repos/auth.py`

 * *Files identical despite different names*

### Comparing `appcensus_dynamic_repos-1.2.0.105/src/appcensus/dynamic_repos/commands.py` & `appcensus_dynamic_repos-1.3.0.108/src/appcensus/dynamic_repos/commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from typing import Optional
 from typing import Union
 
 import tomlkit
 from cleo.helpers import argument
 from cleo.ui.table_cell import TableCell
 from cleo.ui.table_separator import TableSeparator
-from poetry.config.source import Source
 from poetry.console.commands.command import Command
 from poetry.utils.password_manager import PasswordManager
 from tomlkit.items import Table
 from tomlkit.toml_document import TOMLDocument
 
 from appcensus.dynamic_repos import REPO_FILE_PATH
 from appcensus.dynamic_repos.auth import CredentialCache
@@ -25,26 +24,14 @@
 logger = logging.getLogger(__name__)
 
 
 class RepoShowCommand(Command):
     name = "acrepo show"
     description = "Show the configuration of active dynamic repos"
 
-    # Repo prioritization has shifted between using a combination of definition order, and two flags to
-    # an clearer definition of enumerated priorities. We detect what is in play and adjust accordingly.
-    def _use_flags(self, repo: Source) -> bool:
-        return hasattr(repo, "default") and hasattr(repo, "secondary")
-
-    def _flags2prio(self, repo: Source) -> str:
-        if repo.default:  # type: ignore[attr-defined]
-            return "default"
-        elif repo.secondary:  # type: ignore[attr-defined]
-            return "secondary"
-        return "normal"
-
     def handle(self) -> int:
         try:
             for repo in RepoCollector(self.poetry.pool).repositories():
                 creds = CredentialCache.get(repo.name)
                 table = self.table(style="compact")
                 active_state = f" : <c1>{'yes' if creds and creds.valid() else 'no'}</>"
                 if creds:
@@ -52,17 +39,15 @@
                         f" expires <c1>{creds.expires.isoformat() if creds.expires else 'never'}</>"
                     )
                 rows: List[Union[List[Union[str, TableCell]], TableSeparator]] = [
                     [
                         "<info>name</>",
                         f" : <c1>{repo.name}</>",
                     ],
-                    ["<info>priority</>", f" : {self._flags2prio(repo)}"]
-                    if self._use_flags(repo)
-                    else ["<info>priority</>", f" : {repo.priority.name.lower()}"],
+                    ["<info>priority</>", f" : {repo.priority.name.lower()}"],
                     ["<info>url</>", f" : {repo.url}"],
                     ["<info>active auth</info>", active_state]
                     if creds and creds.valid()
                     else ["<info>auth</info>", " : <c1>no</c1>"],
                     ["", ""],
                 ]
                 table.add_rows(rows)
```

### Comparing `appcensus_dynamic_repos-1.2.0.105/src/appcensus/dynamic_repos/models.py` & `appcensus_dynamic_repos-1.3.0.108/src/appcensus/dynamic_repos/models.py`

 * *Files identical despite different names*

### Comparing `appcensus_dynamic_repos-1.2.0.105/src/appcensus/dynamic_repos/plugin.py` & `appcensus_dynamic_repos-1.3.0.108/src/appcensus/dynamic_repos/plugin.py`

 * *Files identical despite different names*

### Comparing `appcensus_dynamic_repos-1.2.0.105/src/appcensus/dynamic_repos/repo_collector.py` & `appcensus_dynamic_repos-1.3.0.108/src/appcensus/dynamic_repos/repo_collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 class PrioritizedRepoStrategy(RepoStrategy):
     def __init__(self, pool: RepositoryPool):
         super().__init__(pool)
 
     def repositories(self) -> List[Source]:
         repos = []
         logger.debug("Collecting repos from a prioritized repo:")
-        for repo in self._pool.repositories:
+        for repo in self._pool.all_repositories:
             if type(repo) is PyPiRepository:
                 continue
             prio = self._pool.get_priority(repo.name)
             repos.append(
                 Source(name=repo.name, url=repo.url, priority=prio)  # type: ignore[attr-defined]
             )
         return repos
```

### Comparing `appcensus_dynamic_repos-1.2.0.105/src/appcensus/dynamic_repos/source_manager.py` & `appcensus_dynamic_repos-1.3.0.108/src/appcensus/dynamic_repos/source_manager.py`

 * *Files identical despite different names*

### Comparing `appcensus_dynamic_repos-1.2.0.105/PKG-INFO` & `appcensus_dynamic_repos-1.3.0.108/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appcensus.dynamic_repos
-Version: 1.2.0.105
+Version: 1.3.0.108
 Summary: Dynamic Poetry Repositories for AppCensus
 License: (c) 2022 App Census - All Rights Reserved
 Author: AppCensus
 Author-email: engineering@appcensus.io
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

