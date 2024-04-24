# Comparing `tmp/snakedeploy-0.8.6.tar.gz` & `tmp/snakedeploy-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakedeploy-0.8.6.tar", last modified: Mon Feb  6 09:27:29 2023, max compression
+gzip compressed data, was "snakedeploy-0.9.1.tar", last modified: Mon Oct 30 18:54:06 2023, max compression
```

## Comparing `snakedeploy-0.8.6.tar` & `snakedeploy-0.9.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 09:27:29.961643 snakedeploy-0.8.6/
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-02-06 09:27:22.000000 snakedeploy-0.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-02-06 09:27:22.000000 snakedeploy-0.8.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-02-06 09:27:29.961643 snakedeploy-0.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-02-06 09:27:22.000000 snakedeploy-0.8.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-02-06 09:27:29.961643 snakedeploy-0.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-02-06 09:27:22.000000 snakedeploy-0.8.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 09:27:29.961643 snakedeploy-0.8.6/snakedeploy/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-02-06 09:27:22.000000 snakedeploy-0.8.6/snakedeploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-06 09:27:29.961643 snakedeploy-0.8.6/snakedeploy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-02-06 09:27:22.000000 snakedeploy-0.8.6/snakedeploy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-02-06 09:27:22.000000 snakedeploy-0.8.6/snakedeploy/collect_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-02-06 09:27:22.000000 snakedeploy-0.8.6/snakedeploy/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)    25635 2023-02-06 09:27:22.000000 snakedeploy-0.8.6/snakedeploy/conda_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-02-06 09:27:22.000000 snakedeploy-0.8.6/snakedeploy/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-02-06 09:27:22.000000 snakedeploy-0.8.6/snakedeploy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-02-06 09:27:22.000000 snakedeploy-0.8.6/snakedeploy/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-02-06 09:27:22.000000 snakedeploy-0.8.6/snakedeploy/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-02-06 09:27:22.000000 snakedeploy-0.8.6/snakedeploy/snakemake_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 09:27:29.961643 snakedeploy-0.8.6/snakedeploy/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-02-06 09:27:22.000000 snakedeploy-0.8.6/snakedeploy/templates/post-instructions.txt.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-02-06 09:27:22.000000 snakedeploy-0.8.6/snakedeploy/templates/use_module.smk.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-02-06 09:27:22.000000 snakedeploy-0.8.6/snakedeploy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-02-06 09:27:22.000000 snakedeploy-0.8.6/snakedeploy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 09:27:29.961643 snakedeploy-0.8.6/snakedeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-02-06 09:27:29.000000 snakedeploy-0.8.6/snakedeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-02-06 09:27:29.000000 snakedeploy-0.8.6/snakedeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 09:27:29.000000 snakedeploy-0.8.6/snakedeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-06 09:27:29.000000 snakedeploy-0.8.6/snakedeploy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 09:27:29.000000 snakedeploy-0.8.6/snakedeploy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-06 09:27:29.000000 snakedeploy-0.8.6/snakedeploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-06 09:27:29.000000 snakedeploy-0.8.6/snakedeploy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    70238 2023-02-06 09:27:22.000000 snakedeploy-0.8.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 18:54:06.962353 snakedeploy-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    15830 2023-10-30 18:53:59.000000 snakedeploy-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2023-10-30 18:53:59.000000 snakedeploy-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2023-10-30 18:54:06.962353 snakedeploy-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2023-10-30 18:53:59.000000 snakedeploy-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2023-10-30 18:54:06.962353 snakedeploy-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2023-10-30 18:53:59.000000 snakedeploy-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 18:54:06.962353 snakedeploy-0.9.1/snakedeploy/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2023-10-30 18:53:59.000000 snakedeploy-0.9.1/snakedeploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2023-10-30 18:54:06.962353 snakedeploy-0.9.1/snakedeploy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11400 2023-10-30 18:53:59.000000 snakedeploy-0.9.1/snakedeploy/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2023-10-30 18:53:59.000000 snakedeploy-0.9.1/snakedeploy/collect_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13529 2023-10-30 18:53:59.000000 snakedeploy-0.9.1/snakedeploy/conda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25635 2023-10-30 18:53:59.000000 snakedeploy-0.9.1/snakedeploy/conda_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2023-10-30 18:53:59.000000 snakedeploy-0.9.1/snakedeploy/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2023-10-30 18:53:59.000000 snakedeploy-0.9.1/snakedeploy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2023-10-30 18:53:59.000000 snakedeploy-0.9.1/snakedeploy/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2023-10-30 18:53:59.000000 snakedeploy-0.9.1/snakedeploy/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2023-10-30 18:53:59.000000 snakedeploy-0.9.1/snakedeploy/snakemake_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 18:54:06.962353 snakedeploy-0.9.1/snakedeploy/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2023-10-30 18:53:59.000000 snakedeploy-0.9.1/snakedeploy/templates/post-instructions.txt.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2023-10-30 18:53:59.000000 snakedeploy-0.9.1/snakedeploy/templates/use_module.smk.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2023-10-30 18:53:59.000000 snakedeploy-0.9.1/snakedeploy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2023-10-30 18:53:59.000000 snakedeploy-0.9.1/snakedeploy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 18:54:06.962353 snakedeploy-0.9.1/snakedeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2023-10-30 18:54:06.000000 snakedeploy-0.9.1/snakedeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2023-10-30 18:54:06.000000 snakedeploy-0.9.1/snakedeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-30 18:54:06.000000 snakedeploy-0.9.1/snakedeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-30 18:54:06.000000 snakedeploy-0.9.1/snakedeploy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-30 18:54:06.000000 snakedeploy-0.9.1/snakedeploy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2023-10-30 18:54:06.000000 snakedeploy-0.9.1/snakedeploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-30 18:54:06.000000 snakedeploy-0.9.1/snakedeploy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    70238 2023-10-30 18:53:59.000000 snakedeploy-0.9.1/versioneer.py
```

### Comparing `snakedeploy-0.8.6/LICENSE` & `snakedeploy-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snakedeploy-0.8.6/PKG-INFO` & `snakedeploy-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: snakedeploy
-Version: 0.8.6
+Version: 0.9.1
 Summary: Deploy a snakemake pipeline from GitHub
 Home-page: https://github.com/snakemake/snakedeploy
 Author: Vanessa Sochat
 Author-email: vsochat@stanford.edu
 Maintainer: Vanessa Sochat
 Maintainer-email: vsochat@stanford.edu
 License: LICENSE
 Keywords: snakemake,pipeline,deployment
+Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
@@ -39,7 +40,8 @@
 [snakedeploy.readthedocs.io](https://snakedeploy.readthedocs.io).
 
 
 ## License
 
  * Free software: MPL 2.0 License
  * `snakedeploy/conda_version.py`: the [source](https://github.com/conda/conda/raw/23.1.0/conda/models/version.py) of this file is distributed under the BSD 3-clause license by Anaconda Inc.
+
```

### Comparing `snakedeploy-0.8.6/README.md` & `snakedeploy-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `snakedeploy-0.8.6/setup.py` & `snakedeploy-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,14 @@
     LONG_DESCRIPTION = filey.read()
 
 ################################################################################
 # MAIN #########################################################################
 ################################################################################
 
 if __name__ == "__main__":
-
     INSTALL_REQUIRES = get_reqs(lookup)
     TESTS_REQUIRES = get_reqs(lookup, "TESTS_REQUIRES")
     ALL_REQUIRES = get_reqs(lookup, "ALL_REQUIRES")
 
     setup(
         name=NAME,
         version=versioneer.get_version(),
```

### Comparing `snakedeploy-0.8.6/snakedeploy/client.py` & `snakedeploy-0.9.1/snakedeploy/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -129,14 +129,41 @@
     )
     pin_conda_envs.add_argument(
         "--conda-frontend",
         choices=["mamba", "conda"],
         default="mamba",
         help="Conda frontend to use (default: mamba).",
     )
+    pin_conda_envs.add_argument(
+        "--create-prs",
+        action="store_true",
+        help="Create pull request for each updated environment. "
+        "Requires GITHUB_TOKEN and GITHUB_REPOSITORY (the repo name) and one of GITHUB_REF_NAME or GITHUB_BASE_REF "
+        "(preferring the latter, representing the target branch, e.g. main or master) environment "
+        "variables to be set (the latter three are available when running as github action). "
+        "In order to enable further actions (e.g. checks) to run on the generated PRs, the "
+        "provided GITHUB_TOKEN may not be the default github actions token. See here for "
+        "options: https://github.com/peter-evans/create-pull-request/blob/main/docs/concepts-guidelines.md#triggering-further-workflow-runs.",
+    )
+    pin_conda_envs.add_argument(
+        "--entity-regex",
+        help="Regular expression for deriving an entity name from the environment file name "
+        "(will be used for adding a label and for title and description). Has to contain a group 'entity' "
+        "(e.g. '(?P<entity>.+)/environment.yaml').",
+    )
+    pin_conda_envs.add_argument(
+        "--pr-add-label",
+        action="store_true",
+        help="Add a label to the PR. Has to be used in combination with --entity-regex.",
+    )
+    pin_conda_envs.add_argument(
+        "--warn-on-error",
+        action="store_true",
+        help="Only warn if conda env evaluation fails and go on with the other envs.",
+    )
 
     update_conda_envs = subparsers.add_parser(
         "update-conda-envs",
         description="Update given conda environment definition files (in YAML format) "
         "so that all contained packages are set to the latest feasible versions.",
     )
     update_conda_envs.add_argument(
@@ -244,14 +271,18 @@
             )
         elif args.subcommand == "collect-files":
             collect_files(config_sheet_path=args.config)
         elif args.subcommand == "pin-conda-envs":
             pin_conda_envs(
                 args.envfiles,
                 conda_frontend=args.conda_frontend,
+                create_prs=args.create_prs,
+                entity_regex=args.entity_regex,
+                pr_add_label=args.pr_add_label,
+                warn_on_error=args.warn_on_error,
             )
         elif args.subcommand == "update-conda-envs":
             update_conda_envs(
                 args.envfiles,
                 conda_frontend=args.conda_frontend,
                 create_prs=args.create_prs,
                 pin_envs=args.pin_envs,
```

### Comparing `snakedeploy-0.8.6/snakedeploy/collect_files.py` & `snakedeploy-0.9.1/snakedeploy/collect_files.py`

 * *Files identical despite different names*

### Comparing `snakedeploy-0.8.6/snakedeploy/conda.py` & `snakedeploy-0.9.1/snakedeploy/conda.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,19 +18,32 @@
 
 from snakedeploy.exceptions import UserError
 from snakedeploy.logger import logger
 from snakedeploy.utils import YamlDumper
 from snakedeploy.conda_version import VersionOrder
 
 
-def pin_conda_envs(conda_env_paths: list, conda_frontend="mamba"):
+def pin_conda_envs(
+    conda_env_paths: list,
+    conda_frontend="mamba",
+    create_prs=False,
+    pr_add_label=False,
+    entity_regex=None,
+    warn_on_error=False,
+):
     """Pin given conda envs by creating <conda-env>.<platform>.pin.txt
     files with explicit URLs for all packages in each env."""
     return CondaEnvProcessor(conda_frontend=conda_frontend).process(
-        conda_env_paths, create_prs=False, update_envs=False, pin_envs=True
+        conda_env_paths,
+        update_envs=False,
+        pin_envs=True,
+        create_prs=create_prs,
+        pr_add_label=pr_add_label,
+        entity_regex=entity_regex,
+        warn_on_error=warn_on_error,
     )
 
 
 def update_conda_envs(
     conda_env_paths: list,
     conda_frontend="mamba",
     create_prs=False,
@@ -91,18 +104,14 @@
 
         if not conda_envs:
             logger.info(
                 f"No conda envs found at given paths: {', '.join(conda_env_paths)}"
             )
         for conda_env_path in conda_envs:
             if create_prs:
-                if not update_envs:
-                    raise UserError(
-                        "Creating PRs for only pinning updates is not supported."
-                    )
                 entity = conda_env_path
                 if entity_regex is not None:
                     m = re.match(entity_regex, conda_env_path)
                     if m is None:
                         raise UserError(
                             f"Given --entity-regex did not match any {conda_env_path}."
                         )
@@ -112,31 +121,40 @@
                         raise UserError(
                             "No group 'entity' found in given --entity-regex."
                         )
                 if pr_add_label and not entity_regex:
                     raise UserError(
                         "Cannot add label to PR without --entity-regex specified."
                     )
+
+                assert (
+                    pin_envs or update_envs
+                ), "bug: either pin_envs or update_envs must be True"
+                mode = "bump" if update_envs else "pin"
                 pr = PR(
-                    f"perf: autobump {entity}",
-                    f"Automatic update of {entity}.",
-                    f"autobump/{entity.replace('/', '-')}",
+                    f"perf: auto{mode} {entity}",
+                    f"Automatic {mode} of {entity}.",
+                    f"auto{mode}/{entity.replace('/', '-')}",
                     repo,
                     label=entity if pr_add_label else None,
                 )
             else:
                 pr = None
             try:
                 updated = False
                 if update_envs:
                     logger.info(f"Updating {conda_env_path}...")
                     updated = self.update_env(
                         conda_env_path, pr=pr, warn_on_error=warn_on_error
                     )
-                if pin_envs and (not update_envs or updated):
+                if pin_envs and (
+                    not update_envs
+                    or updated
+                    or not self.get_pin_file_path(conda_env_path).exists()
+                ):
                     logger.info(f"Pinning {conda_env_path}...")
                     self.update_pinning(conda_env_path, pr)
             except sp.CalledProcessError as e:
                 msg = f"Failed for conda env {conda_env_path}:\n{e.stderr}\n{e.stdout}"
                 if warn_on_error:
                     logger.warning(msg)
                 else:
@@ -235,16 +253,19 @@
                     msg=f"perf: update {conda_env_path}.",
                 )
             return True
         else:
             logger.info("No updates in env.")
             return False
 
+    def get_pin_file_path(self, conda_env_path):
+        return Path(conda_env_path).with_suffix(f".{self.info['platform']}.pin.txt")
+
     def update_pinning(self, conda_env_path, pr=None):
-        pin_file = Path(conda_env_path).with_suffix(f".{self.info['platform']}.pin.txt")
+        pin_file = self.get_pin_file_path(conda_env_path)
         old_content = None
         updated = False
         if pin_file.exists():
             with open(pin_file, "r") as infile:
                 old_content = infile.read()
 
         with tempfile.TemporaryDirectory(dir=".", prefix=".") as tmpdir:
@@ -292,15 +313,15 @@
         self.repo = repo
         self.base_ref = (
             os.environ.get("GITHUB_BASE_REF") or os.environ["GITHUB_REF_NAME"]
         )
         self.label = label
 
     def add_file(self, filepath, content, is_updated, msg):
-        self.files.append(File(filepath, content, is_updated, msg))
+        self.files.append(File(str(filepath), content, is_updated, msg))
 
     @retry(tries=2, delay=60)
     def create(self):
         if not self.files:
             logger.info("No files to commit.")
             return
```

### Comparing `snakedeploy-0.8.6/snakedeploy/conda_version.py` & `snakedeploy-0.9.1/snakedeploy/conda_version.py`

 * *Files identical despite different names*

### Comparing `snakedeploy-0.8.6/snakedeploy/deploy.py` & `snakedeploy-0.9.1/snakedeploy/deploy.py`

 * *Files identical despite different names*

### Comparing `snakedeploy-0.8.6/snakedeploy/exceptions.py` & `snakedeploy-0.9.1/snakedeploy/exceptions.py`

 * *Files identical despite different names*

### Comparing `snakedeploy-0.8.6/snakedeploy/logger.py` & `snakedeploy-0.9.1/snakedeploy/logger.py`

 * *Files identical despite different names*

### Comparing `snakedeploy-0.8.6/snakedeploy/providers.py` & `snakedeploy-0.9.1/snakedeploy/providers.py`

 * *Files identical despite different names*

### Comparing `snakedeploy-0.8.6/snakedeploy/snakemake_wrappers.py` & `snakedeploy-0.9.1/snakedeploy/snakemake_wrappers.py`

 * *Files identical despite different names*

### Comparing `snakedeploy-0.8.6/snakedeploy/utils.py` & `snakedeploy-0.9.1/snakedeploy/utils.py`

 * *Files identical despite different names*

### Comparing `snakedeploy-0.8.6/snakedeploy/version.py` & `snakedeploy-0.9.1/snakedeploy/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = "Vanessa Sochat"
 __copyright__ = "Copyright 2020-2021, Vanessa Sochat"
 __license__ = "MPL 2.0"
 
-__version__ = "0.8.6"
+__version__ = "0.9.1"
 AUTHOR = "Vanessa Sochat"
 AUTHOR_EMAIL = "vsochat@stanford.edu"
 NAME = "snakedeploy"
 PACKAGE_URL = "https://github.com/snakemake/snakedeploy"
 KEYWORDS = "snakemake,pipeline,deployment"
 DESCRIPTION = "Deploy a snakemake pipeline from GitHub"
 LICENSE = "LICENSE"
```

### Comparing `snakedeploy-0.8.6/snakedeploy.egg-info/PKG-INFO` & `snakedeploy-0.9.1/snakedeploy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: snakedeploy
-Version: 0.8.6
+Version: 0.9.1
 Summary: Deploy a snakemake pipeline from GitHub
 Home-page: https://github.com/snakemake/snakedeploy
 Author: Vanessa Sochat
 Author-email: vsochat@stanford.edu
 Maintainer: Vanessa Sochat
 Maintainer-email: vsochat@stanford.edu
 License: LICENSE
 Keywords: snakemake,pipeline,deployment
+Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
@@ -39,7 +40,8 @@
 [snakedeploy.readthedocs.io](https://snakedeploy.readthedocs.io).
 
 
 ## License
 
  * Free software: MPL 2.0 License
  * `snakedeploy/conda_version.py`: the [source](https://github.com/conda/conda/raw/23.1.0/conda/models/version.py) of this file is distributed under the BSD 3-clause license by Anaconda Inc.
+
```

### Comparing `snakedeploy-0.8.6/snakedeploy.egg-info/SOURCES.txt` & `snakedeploy-0.9.1/snakedeploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snakedeploy-0.8.6/versioneer.py` & `snakedeploy-0.9.1/versioneer.py`

 * *Files identical despite different names*

