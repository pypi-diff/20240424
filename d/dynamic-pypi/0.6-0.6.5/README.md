# Comparing `tmp/dynamic_pypi-0.6.tar.gz` & `tmp/dynamic_pypi-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic_pypi-0.6.tar", max compression
+gzip compressed data, was "dynamic_pypi-0.6.5.tar", max compression
```

## Comparing `dynamic_pypi-0.6.tar` & `dynamic_pypi-0.6.5.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0        0 2024-01-31 21:50:06.575108 dynamic_pypi-0.6/LICENSE.md
--rw-r--r--   0        0        0       14 2024-01-31 21:49:21.010503 dynamic_pypi-0.6/README.md
--rw-r--r--   0        0        0      166 2024-01-31 22:03:30.872875 dynamic_pypi-0.6/dpypi/__init__.py
--rw-r--r--   0        0        0     4433 2024-01-31 22:46:00.276450 dynamic_pypi-0.6/dpypi/github_connection.py
--rw-r--r--   0        0        0     3988 2024-01-31 22:57:53.146209 dynamic_pypi-0.6/dpypi/serve.py
--rw-r--r--   0        0        0     1166 2024-01-31 22:59:05.208228 dynamic_pypi-0.6/dpypi/web_utils.py
--rw-r--r--   0        0        0      655 2024-01-31 22:01:51.170697 dynamic_pypi-0.6/dpypi/wheel.py
--rw-r--r--   0        0        0      418 2024-01-31 23:00:26.475256 dynamic_pypi-0.6/pyproject.toml
--rw-r--r--   0        0        0      455 1970-01-01 00:00:00.000000 dynamic_pypi-0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-31 21:50:06.575108 dynamic_pypi-0.6.5/LICENSE.md
+-rw-r--r--   0        0        0       16 2024-04-24 01:48:04.598909 dynamic_pypi-0.6.5/README.md
+-rw-r--r--   0        0        0      168 2024-04-23 16:28:28.283358 dynamic_pypi-0.6.5/dpypi/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:46:22.795368 dynamic_pypi-0.6.5/dpypi/connections/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-23 19:19:06.768356 dynamic_pypi-0.6.5/dpypi/connections/connection.py
+-rw-r--r--   0        0        0     4767 2024-04-23 23:27:46.925085 dynamic_pypi-0.6.5/dpypi/connections/github_connection.py
+-rw-r--r--   0        0        0     2616 2024-04-24 01:42:13.830850 dynamic_pypi-0.6.5/dpypi/connections/local_connection.py
+-rw-r--r--   0        0        0     5620 2024-04-24 01:36:24.894451 dynamic_pypi-0.6.5/dpypi/serve.py
+-rw-r--r--   0        0        0     1077 2024-04-23 23:27:56.412277 dynamic_pypi-0.6.5/dpypi/web_utils.py
+-rw-r--r--   0        0        0      655 2024-01-31 22:01:51.170697 dynamic_pypi-0.6.5/dpypi/wheel.py
+-rw-r--r--   0        0        0      420 2024-04-24 01:47:48.740576 dynamic_pypi-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 dynamic_pypi-0.6.5/PKG-INFO
```

### Comparing `dynamic_pypi-0.6/dpypi/github_connection.py` & `dynamic_pypi-0.6.5/dpypi/connections/github_connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,76 +8,82 @@
 from github.GitRelease import GitRelease
 from github.GitReleaseAsset import GitReleaseAsset
 from github.Repository import Repository
 from pi_conf import Config
 
 log = getLogger(__name__)
 
+REDACT_KEYS = set(["access_token"])
+
 
 @dataclass
 class IndexConfig(Config):
     name: str
     uri: str
     repos: list[str] = None
     access_token: str = None
 
 
 @dataclass
 class ReleaseAsset(GitReleaseAsset):
     ## Hack to add a local_path attribute to GitReleaseAsset for type hinting
     local_path: str = None
 
+    # def name(self) -> str:
+    #     return self.browser_download_url.split("/")[-1]
 
-@dataclass
-class GithubConnections:
-    config: Config
-    connections: dict[str, "GithubConnection"] = field(default_factory=dict)
-    _repo_2_connection: dict = None
-
-    def __post_init__(self):
-        index_cfg: IndexConfig
-        redact = set(["access_token"])
-        for index_cfg in self.config.index:
-            for k in index_cfg:
-                cfg = index_cfg.copy()
-                if k in redact:
-                    cfg[k] = "*****"
-                log.debug(f"{k}={cfg[k]}")
-            gc = GithubConnection(index_cfg)
-            self.connections[index_cfg.name] = gc
-
-        self.projects = {}
 
-    @property
-    def repo_2_connection(self) -> dict[str, "GithubConnection"]:
-        if self._repo_2_connection is None:
-            self._repo_2_connection = self._make_repos()
-        return self._repo_2_connection
-
-    def _make_repos(self) -> dict:
-        d: dict[str, GithubConnection] = {}
-        for gc in self.connections.values():
-            repo_filter = set(gc.config.repos) if "repos" in gc.config else None
-            for repo in gc.g.get_user().get_repos():
-                if repo_filter and repo.name not in repo_filter:
-                    continue
-                d[repo.name] = gc
-        return d
+# @dataclass
+# class GithubConnections:
+#     config: Config
+#     connections: dict[str, "GithubConnection"] = field(default_factory=dict)
+#     _repo_2_connection: dict = None
+
+#     def __post_init__(self):
+#         index_cfg: IndexConfig
+#         redact = set(["access_token"])
+#         for index_cfg in self.config.index:
+#             for k in index_cfg:
+#                 cfg = index_cfg.copy()
+#                 if k in redact:
+#                     cfg[k] = "*****"
+#                 log.debug(f"{k}={cfg[k]}")
+#             gc = GithubConnection(index_cfg)
+#             self.connections[index_cfg.name] = gc
+
+#         self.projects = {}
+
+#     @property
+#     def repo_2_connection(self) -> dict[str, "GithubConnection"]:
+#         if self._repo_2_connection is None:
+#             self._repo_2_connection = self._make_repos()
+#         return self._repo_2_connection
+
+#     def _make_repos(self) -> dict:
+#         d: dict[str, GithubConnection] = {}
+#         for gc in self.connections.values():
+#             repo_filter = set(gc.config.repos) if "repos" in gc.config else None
+#             for repo in gc.g.get_user().get_repos():
+#                 if repo_filter and repo.name not in repo_filter:
+#                     continue
+#                 d[repo.name] = gc
+#         return d
 
 
 @dataclass
 class GithubConnection:
+    name: str
     config: IndexConfig
 
     _g: Github = None
     _auth = None
 
-    @property
-    def name(self) -> str:
-        return self.config.name
+    # @property
+    # def name(self) -> str:
+    #     return self.config.name
 
     @property
     def uri(self) -> str:
         return self.config.uri
 
     @property
     def repo_names(self) -> list[str]:
@@ -92,28 +98,32 @@
     @property
     def g(self) -> Github:
         if self._g is None:
             self._g = Github(auth=self.auth)
 
         return self._g
 
+    def get_repo(self, repo_name: str) -> Repository:
+        return self.g.get_repo[repo_name]
+
     def list_release_assets(
         self,
         repo: Repository,
-    ) -> list[GitReleaseAsset]:
+    ) -> list[ReleaseAsset]:
         """
         Get all assets for all releases in a repository
         args:
             repo: Repository.Repository
         returns:
             list[GitReleaseAsset.GitReleaseAsset]
         """
         assets = []
         for release in repo.get_releases():
             for asset in release.get_assets():
+                asset.local_path
                 assets.append(asset)
         return assets
 
     def get_release_asset(
         self,
         repo: Repository,
         release: str | GitRelease,
```

### Comparing `dynamic_pypi-0.6/dpypi/web_utils.py` & `dynamic_pypi-0.6.5/dpypi/web_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,19 +25,18 @@
         artifact_dir: the directory where the release assets are stored
     returns:
     str: the path to the index.html file
     """
     
     links = []
     for asset in release_assets:
-        name = asset.browser_download_url.split("/")[-1]
-        # tag = soup.new_tag("a", href=f"/{artifact_dir}/{project}/{asset.name}")
+        # name = asset.browser_download_url.split("/")[-1]
+        name = asset.name
         s = f'<a href="/{artifact_dir}/{project}/{asset.name}">{name}</a>'
         links.append(s)
     html = html_index.format(links="\n    ".join(links))
     
     os.makedirs(os.path.dirname(html_path), exist_ok=True)
 
     with open(html_path, "w") as f:
         f.write(html)
-        # f.write(soup.prettify())
     return html_path
```

#### html2text {}

```diff
@@ -2,12 +2,11 @@
 {links}
 """ def write_index_html( project: str, release_assets: list
 [GitReleaseAsset.GitReleaseAsset], html_path: str, artifact_dir: str, ) -> str:
 """ Write an index.html file for a project's distribution. args: project: the
 name of the project release_assets: a list of release assets html_path: the
 path to the index.html artifact_dir: the directory where the release assets are
 stored returns: str: the path to the index.html file """ links = [] for asset
-in release_assets: name = asset.browser_download_url.split("/")[-1] # tag =
-soup.new_tag("a", href=f"/{artifact_dir}/{project}/{asset.name}") s = f'_{_n_a_m_e_}'
-links.append(s) html = html_index.format(links="\n ".join(links)) os.makedirs
-(os.path.dirname(html_path), exist_ok=True) with open(html_path, "w") as f:
-f.write(html) # f.write(soup.prettify()) return html_path
+in release_assets: # name = asset.browser_download_url.split("/")[-1] name =
+asset.name s = f'_{_n_a_m_e_}' links.append(s) html = html_index.format(links="\n
+".join(links)) os.makedirs(os.path.dirname(html_path), exist_ok=True) with open
+(html_path, "w") as f: f.write(html) return html_path
```

### Comparing `dynamic_pypi-0.6/dpypi/wheel.py` & `dynamic_pypi-0.6.5/dpypi/wheel.py`

 * *Files identical despite different names*

