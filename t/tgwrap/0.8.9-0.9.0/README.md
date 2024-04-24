# Comparing `tmp/tgwrap-0.8.9.tar.gz` & `tmp/tgwrap-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgwrap-0.8.9.tar", max compression
+gzip compressed data, was "tgwrap-0.9.0.tar", max compression
```

## Comparing `tgwrap-0.8.9.tar` & `tgwrap-0.9.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.8.9/LICENSE
--rw-r--r--   0        0        0    10353 2023-11-21 08:08:14.362959 tgwrap-0.8.9/README.md
--rw-r--r--   0        0        0      922 2024-02-01 11:00:32.533856 tgwrap-0.8.9/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.8.9/tgwrap/__init__.py
--rw-r--r--   0        0        0     8726 2023-10-20 14:35:12.875311 tgwrap-0.8.9/tgwrap/analyze.py
--rwxr-xr-x   0        0        0    29060 2023-11-27 12:41:28.897080 tgwrap-0.8.9/tgwrap/cli.py
--rw-r--r--   0        0        0     9577 2024-02-01 10:59:51.328863 tgwrap-0.8.9/tgwrap/deploy.py
--rwxr-xr-x   0        0        0    74105 2024-01-31 12:13:03.117600 tgwrap-0.8.9/tgwrap/main.py
--rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.8.9/tgwrap/printer.py
--rw-r--r--   0        0        0    11528 1970-01-01 00:00:00.000000 tgwrap-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.9.0/LICENSE
+-rw-r--r--   0        0        0    12159 2024-04-24 11:33:21.171629 tgwrap-0.9.0/README.md
+-rw-r--r--   0        0        0      922 2024-04-24 11:29:31.368994 tgwrap-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.9.0/tgwrap/__init__.py
+-rw-r--r--   0        0        0     8726 2023-10-20 14:35:12.875311 tgwrap-0.9.0/tgwrap/analyze.py
+-rwxr-xr-x   0        0        0    29727 2024-04-24 07:14:54.956803 tgwrap-0.9.0/tgwrap/cli.py
+-rw-r--r--   0        0        0    10421 2024-04-15 08:15:36.473440 tgwrap-0.9.0/tgwrap/deploy.py
+-rwxr-xr-x   0        0        0    80691 2024-04-24 11:32:17.978883 tgwrap-0.9.0/tgwrap/main.py
+-rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.9.0/tgwrap/printer.py
+-rw-r--r--   0        0        0    13334 1970-01-01 00:00:00.000000 tgwrap-0.9.0/PKG-INFO
```

### Comparing `tgwrap-0.8.9/LICENSE` & `tgwrap-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tgwrap-0.8.9/README.md` & `tgwrap-0.9.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -108,14 +108,64 @@
 
 ```console
 export TGWRAP_PLANFILE_DIR=".terragrunt-cache/current"
 ```
 
 Or pass it along with the `--planfile-dir|-P` option and it will use that.
 
+### Logging the results
+
+`tgwrap` supports logging the analyze results to an [Azure Log Analytics](https://learn.microsoft.com/en-us/azure/azure-monitor/logs/log-analytics-overview) custom table.
+
+For that, the custom table need to be present, including a [data collection endpoint](https://learn.microsoft.com/en-us/azure/azure-monitor/essentials/data-collection-endpoint-overview?tabs=portal) and associated [data collection rule](https://learn.microsoft.com/en-us/azure/azure-monitor/essentials/data-collection-rule-overview?tabs=portal).
+
+When you want to activate this, just pass `--data-collection-endpoint` (or, more conveniently, set the `TGWRAP_ANALYZE_DATA_COLLECTION_ENDPOINT` environment variable) with the url to which the data can be posted.
+
+> Note that for this to work, `tgwrap` assumes that there is a functioning [azure cli](https://learn.microsoft.com/en-us/cli/azure/) available on the system.
+
+A payload as below will be posted, and the log analytics table should be able to accomodate for that:
+
+```json
+[
+  {
+    "scope": "terragrunt/dlzs/data-platform/global/platform/rbac/",
+    "principal": "myself",
+    "repo": "https://gitlab.com/my-git-repo.git",
+    "creations": 0,
+    "updates": 0,
+    "deletions": 0,
+    "minor": 0,
+    "medium": 0,
+    "major": 0,
+    "unknown": 0,
+    "total": 0,
+    "score": 0.0,
+    "details": [
+      {
+        "drifts": {
+          "minor": 0,
+          "medium": 0,
+          "major": 0,
+          "unknown": 0,
+          "total": 0,
+          "score": 0.0
+        },
+        "all": [],
+        "creations": [],
+        "updates": [],
+        "deletions": [],
+        "unauthorized": [],
+        "unknowns": [],
+        "module": ""
+      }
+    ]
+  }
+]
+```
+
 ## More than a wrapper
 
 Over time, tgwrap became more than a wrapper, blantly violating [#1 of the unix philosophy](https://en.wikipedia.org/wiki/Unix_philosophy#:~:text=The%20Unix%20philosophy%20is%20documented,%2C%20as%20yet%20unknown%2C%20program.): 'Make each program do one thing well'.
 
 For instance, the 'analyze' functionality is already an example, but more features such as deploying a landing zone has crept into the application. It makes sense for how we're using it, but we're fully aware this makes it less generically applicable.
 
 ## Usage
@@ -196,24 +246,26 @@
     include_modules: {} # omit or use an empty dict for all of them
       # or specify your modules as follows
       # base: {} # just a simple include
       # networking-connected: # or a bit more complicated
       #  - source: networking
       #  - target: networking-connected
 
-sub_stacks:
+substacks:
   is01:
     source: shared-integration/intsvc01
     target: integration/is01
     exclude_modules:  # a list of modules that will always be excluded, can be omitted
       - my-specific-module
     configs:
       - my-ss-config.hcl
       - ../my-ss-config-dir
   is02:
+    applies_to_stages: # optional list of stages to include the substack in
+      - dev
     source: shared-integration/intsvc01
     target: integration/is02
 
 # global configuration files that are deployed as well
 # note that these files are typically applicable to all landing zones and stages!
 # this might lead to unexpected behaviour
 # note that you can exclude syncing these files with a command line switch
```

### Comparing `tgwrap-0.8.9/pyproject.toml` & `tgwrap-0.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tgwrap"
-version = "0.8.9"
+version = "0.9.0"
 description = "A (terragrunt) wrapper around a (terraform) wrapper around ...."
 authors = ["Gerco Grandia <gerco.grandia@4synergy.nl>", "Pascal Alma <pascal.alma@4synergy.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/lunadata/tgwrap"
 repository = "https://gitlab.com/lunadata/tgwrap"
 documentation = "https://gitlab.com/lunadata/tgwrap/"
```

### Comparing `tgwrap-0.8.9/tgwrap/analyze.py` & `tgwrap-0.9.0/tgwrap/analyze.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.8.9/tgwrap/cli.py` & `tgwrap-0.9.0/tgwrap/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         echo('Could not determine package version, continue nevertheless.')
         pass
 
 CLICK_CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
 TG_COMMANDS=[
     'init', 'validate', 'validate-inputs', 'plan', 'apply',
-    'destroy', 'info', 'output', 'show',
+    'destroy', 'info', 'output', 'show', 'state',
     ]
 STAGES=['global', 'sbx', 'dev', 'qas', 'run', 'tst', 'acc', 'prd']
 class DefaultGroup(click.Group):
     '''
     Allow a default command for a group
     '''
     ignore_unknown_options = True
@@ -103,15 +103,15 @@
 
 @main.command(
     name="run",
     context_settings=dict(
         ignore_unknown_options=True,
     ),
 )
-@click.argument('command', type=click.Choice(TG_COMMANDS + ['state', 'render-json']))
+@click.argument('command', type=click.Choice(TG_COMMANDS + ['render-json']))
 @click.option('--verbose', '-v', is_flag=True, default=False,
     help='Verbose printing',
     show_default=True
     )
 @click.option('--debug', '-d', is_flag=True, default=False,
     help='Run the terragrunt command with debug logging enabled (where applicable)',
     show_default=True
@@ -206,14 +206,18 @@
     help='Whether or not external dependencies must be ignored',
     show_default=True
     )
 @click.option('--step-by-step', '-s', is_flag=True, default=False,
     help='Run the command step by step and stop when an error occurs (where applicable)',
     show_default=True
     )
+@click.option('--continue-on-error', '-C', is_flag=True, default=False,
+    help='When running in step by step, continue when an error occurs',
+    show_default=True
+    )
 @click.option('--planfile', '-p', is_flag=True, default=False,
     help='Use the generated planfile when applying the changes',
     show_default=True
     )
 @click.option('--auto-approve', '-a', is_flag=True, default=False,
     help='Do not ask for confirmation before applying planned changes (where applicable)',
     show_default=True
@@ -240,15 +244,15 @@
     multiple=True, default=[],
     help='A glob of a directory that needs to be excluded, this option can be used multiple times. For example: -E "integrations/\*/\*"',
     show_default=True,
     )
 @click.argument('terragrunt-args', nargs=-1, type=click.UNPROCESSED)
 @click.version_option(version=__version__)
 def run_all(command, verbose, debug, dry_run, no_lock, update, upgrade, exclude_external_dependencies,
-    step_by_step, planfile, auto_approve, clean, working_dir, start_at_step,
+    step_by_step, continue_on_error, planfile, auto_approve, clean, working_dir, start_at_step,
     limit_parallelism, include_dir, exclude_dir, terragrunt_args):
     """ Executes a terragrunt command across multiple projects """
 
     check_latest_version(verbose)
 
     tgwrap = TgWrap(verbose=verbose, check_tg_source=True)
     tgwrap.run_all(
@@ -256,14 +260,15 @@
         debug=debug,
         dry_run=dry_run,
         no_lock=no_lock,
         update=update,
         upgrade=upgrade,
         exclude_external_dependencies=exclude_external_dependencies,
         step_by_step=step_by_step,
+        continue_on_error=continue_on_error,
         planfile=planfile,
         auto_approve=auto_approve,
         clean=clean,
         working_dir=working_dir,
         start_at_step=start_at_step,
         limit_parallelism=limit_parallelism,
         include_dirs=include_dir,
@@ -283,17 +288,18 @@
     )
 @click.option('--working-dir', '-w', default=None,
     help='Working directory, when omitted the current directory is used',
     )
 @click.option('--json', '-j', is_flag=True, default=False,
     help='Show output in json format',
     )
-@click.option('--planfile-dir', '-P', default=None,
+@click.option('--planfile-dir', '-P', default='.terragrunt-cache/current',
     help='Relative path to directory with plan file (or set TGWRAP_PLANFILE_DIR environment variable), see README for more details',
     envvar='TGWRAP_PLANFILE_DIR', type=click.Path(),
+    show_default=True,
     )
 @click.argument('terragrunt-args', nargs=-1, type=click.UNPROCESSED)
 @click.version_option(version=__version__)
 def show(verbose, json, working_dir, planfile_dir, terragrunt_args):
     """ Reads and outputs a Terraform state or plan file in a human-readable or json form. """
 
     check_latest_version(verbose)
@@ -388,23 +394,29 @@
     show_default=True
     )
 @click.option('--exclude-dir', '-E',
     multiple=True, default=[],
     help='A glob of a directory that needs to be excluded, this option can be used multiple times. For example: -E "integrations/\*/\*"',
     show_default=True,
     )
-@click.option('--planfile-dir', '-P', default=None,
+@click.option('--planfile-dir', '-P', default='.terragrunt-cache/current',
     help='Relative path to directory with plan file (or set TGWRAP_PLANFILE_DIR environment variable), see README for more details',
     envvar='TGWRAP_PLANFILE_DIR', type=click.Path(),
+    show_default=True,
+    )
+@click.option('--data-collection-endpoint', '-D', default=None,
+    help='Optional URI of an (Azure) data collection endpoint, to which the analyse results will be sent',
+    envvar='TGWRAP_ANALYZE_DATA_COLLECTION_ENDPOINT',
+    show_default=True,
     )
 @click.argument('terragrunt-args', nargs=-1, type=click.UNPROCESSED)
 @click.version_option(version=__version__)
 def run_analyze(verbose, exclude_external_dependencies, working_dir, start_at_step,
-            out, analyze_config, parallel_execution,
-            include_dir, exclude_dir, planfile_dir, terragrunt_args):
+            out, analyze_config, parallel_execution, include_dir, exclude_dir,
+            planfile_dir, data_collection_endpoint, terragrunt_args):
     """ Analyzes the plan files """
 
     check_latest_version(verbose)
 
     tgwrap = TgWrap(verbose=verbose)
     tgwrap.analyze(
         exclude_external_dependencies=exclude_external_dependencies,
@@ -412,14 +424,15 @@
         start_at_step=start_at_step,
         out=out,
         analyze_config=analyze_config,
         parallel_execution=parallel_execution,
         include_dirs=include_dir,
         exclude_dirs=exclude_dir,
         planfile_dir=planfile_dir,
+        data_collection_endpoint=data_collection_endpoint,
         terragrunt_args=terragrunt_args,
     )
 
 @main.command(
     name="lock",
     context_settings=dict(
         ignore_unknown_options=True,
```

### Comparing `tgwrap-0.8.9/tgwrap/deploy.py` & `tgwrap-0.9.0/tgwrap/deploy.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         # a directory, which is not always what you want!!!!!
         #
         if os.path.isdir(target_path):
             include_statements = \
                 f"--include='{terragrunt_file}' {lock_file_stmt} {env_file_stmt} {excludes_stmt} " + \
                 "--exclude='.terragrunt-cache/' --exclude='.terraform/' " + \
                 "--exclude='terragrunt-debug.tfvars.json' --exclude=planfile " + \
-                "--exclude='.DS_Store' --exclude='*.log'"
+                "--exclude='.DS_Store' --exclude='*.log' "
 
         cmd = f"rsync -aim {dry_run_stmt} {clean_stmt} " + \
             include_statements + \
             f"{source_path} {target_path}"
 
         cmd = re.sub(' +', ' ', cmd)
 
@@ -167,70 +167,80 @@
                 "source": source_path,
                 "target": full_target_path,
             }
         else:
             printer.warning(f'Source path of config file does not exist: {source_path}')
 
     for ss, substack in substack_configs:
-        printer.verbose(f'Found substack : {ss}')
-
-        source_path = os.path.join(
-            source_dir, source_stage, substack['source'], ''
-            )
-        target_path = os.path.join(
-            target_dir, substack['target'], ''
-            )
-
-        include_modules = substack['include_modules'] if len(substack.get('include_modules', {})) > 0 else []
-        printer.verbose(f'Include modules: {include_modules}')
-
-        if include_modules:
-            # get all directories in the substack and create an exlude_modules list from that
-            source_directories = get_directories(source_path)
-            exclude_modules = list(set(source_directories) - set(include_modules))
-        else:
-            exclude_modules = substack.get('exclude_modules', [])
-        
-        if os.path.exists(source_path):
-            deploy_actions[f'substack -> {substack["target"]}'] = {
-                "source": source_path,
-                "target": target_path,
-                "excludes": exclude_modules,
-            }
+        if 'applies_to_stages' in substack and target_stage not in substack['applies_to_stages']:
+            printer.verbose(f'Target stage {target_stage} not applicable for substack {ss}.')
         else:
-            printer.warning(f'Source path of substack does not exist: {source_path}')
-
-        if len(substack.get('configs', [])) > 0:
-            # run some checks and sets some variables
-            if not source_config_dir:
-                raise Exception("Config files must be deployed but 'config_path' variable is not set!")
-            elif not config_dir:
-                raise Exception("Config files must be deployed but 'config_dir' variable is not set!")
+            printer.verbose(f'Found substack : {ss}')
 
+            source_path = os.path.join(
+                source_dir, source_stage, substack['source'], ''
+                )
+            source_modules = {
+                entry:{} for entry in os.listdir(source_path) if os.path.isdir(os.path.join(source_path, entry))
+            }
             target_path = os.path.join(
-                target_dir, config_dir, module_name, target_stage, substack['target'], '',
+                target_dir, substack['target'], ''
                 )
-            # the target path might not exist
-            try:
-                os.makedirs(target_path)
-            except FileExistsError:
-                pass
 
-        for cfg in substack.get('configs', []):
-            printer.verbose(f'Found substack config file : {cfg}')
+            printer.verbose(f'Include substack modules: {include_modules}')
 
-            full_source_path = os.path.join(
-                source_config_dir, source_stage, substack['source'], cfg
-                )
+    # printer.verbose(f'Found modules: {source_modules}')
+        # include_modules = config['include_modules'] if len(config.get('include_modules')) > 0 else source_modules
+            include_modules = substack['include_modules'] if len(substack.get('include_modules', {})) > 0 else source_modules
+            printer.verbose(f'Include modules: {include_modules}')
+
+            if include_modules:
+                # get all directories in the substack and create an exlude_modules list from that
+                source_directories = get_directories(source_path)
+                exclude_modules = list(set(source_directories) - set(include_modules))
+            else:
+                exclude_modules = substack.get('exclude_modules', [])
             
-            full_target_path = os.path.dirname(os.path.join(target_path, cfg))
-            # print("source: ", full_source_path)
-            # print("target: ", full_target_path)
             if os.path.exists(source_path):
-                deploy_actions[f"substack {substack['target']} configs -> {os.path.join(substack['source'], cfg)}"] = {
-                    "source": full_source_path,
-                    "target": full_target_path,
+                deploy_actions[f'substack -> {substack["target"]}'] = {
+                    "source": source_path,
+                    "target": target_path,
+                    "excludes": exclude_modules,
                 }
             else:
-                printer.warning(f'Source path of config file does not exist: {source_path}')
+                printer.warning(f'Source path of substack does not exist: {source_path}')
+
+            if len(substack.get('configs', [])) > 0:
+                # run some checks and sets some variables
+                if not source_config_dir:
+                    raise Exception("Config files must be deployed but 'config_path' variable is not set!")
+                elif not config_dir:
+                    raise Exception("Config files must be deployed but 'config_dir' variable is not set!")
+
+                target_path = os.path.join(
+                    target_dir, config_dir, module_name, target_stage, substack['target'], '',
+                    )
+                # the target path might not exist
+                try:
+                    os.makedirs(target_path)
+                except FileExistsError:
+                    pass
+
+            for cfg in substack.get('configs', []):
+                printer.verbose(f'Found substack config file : {cfg}')
+
+                full_source_path = os.path.join(
+                    source_config_dir, source_stage, substack['source'], cfg
+                    )
+                
+                full_target_path = os.path.dirname(os.path.join(target_path, cfg))
+                # print("source: ", full_source_path)
+                # print("target: ", full_target_path)
+                if os.path.exists(source_path):
+                    deploy_actions[f"substack {substack['target']} configs -> {os.path.join(substack['source'], cfg)}"] = {
+                        "source": full_source_path,
+                        "target": full_target_path,
+                    }
+                else:
+                    printer.warning(f'Source path of config file does not exist: {source_path}')
 
     return deploy_actions
```

### Comparing `tgwrap-0.8.9/tgwrap/main.py` & `tgwrap-0.9.0/tgwrap/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # - https://github.com/bcochofel/terraplanfeed/tree/main/terraplanfeed
 
 import os
 import sys
 import subprocess
 import shlex
 import shutil
+import requests
 import re
 import tempfile
 import json
 import yaml
 import threading
 import queue
 import multiprocessing
@@ -30,21 +31,21 @@
 import fnmatch
 import inquirer
 
 from datetime import datetime, timezone
 from .printer import Printer
 from .analyze import run_analyze
 from .deploy import prepare_deploy_config, run_sync
+
 class DateTimeEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, datetime):
             return obj.isoformat()
         return super().default(obj)
 
-
 class TgWrap():
     """
     A wrapper around terragrunt with the sole purpose to make it a bit
     (in an opiionated way) easier to use
     """
     SEPARATOR=':|:'
     TERRAGRUNT_FILE='terragrunt.hcl'
@@ -98,15 +99,15 @@
         """ Constructs the command """
 
         commands = {
             'generic': '{base_command} {command} --terragrunt-non-interactive {no_auto_approve} {update} {upgrade} {parallelism} {common}',
             'info': '{base_command} terragrunt-info --terragrunt-non-interactive {update} {upgrade} {common}',
             'plan': '{base_command} {command} --terragrunt-non-interactive  -out={planfile_name} {lock_level} {update} {parallelism} {common}',
             'apply': '{base_command} {command} {non_interactive} {no_auto_approve} {update} {parallelism} {common} {planfile}',
-            'show': '{base_command} {command} --terragrunt-non-interactive {planfile_name} {common}',
+            'show': '{base_command} {command} --terragrunt-non-interactive {common} {planfile_name}',
             'destroy': '{base_command} {command} {non_interactive} {no_auto_approve} {parallelism} {common} {planfile}',
         }
 
         lock_stmt = ''
         if no_lock and command in ['init', 'validate', 'validate-inputs', 'plan', 'info', 'output', 'show', 'state']:
             lock_stmt = '-lock=false'
             self.printer.warning('Terraform state will NOT be locked')
@@ -155,14 +156,15 @@
             base_command      = 'terragrunt run-all'
             ignore_deps_stmt  = '--terragrunt-ignore-external-dependencies' if exclude_external_dependencies else '--terragrunt-include-external-dependencies'
             auto_approve_stmt = '--terragrunt-no-auto-approve' if no_auto_approve else ''
             interactive_stmt  = '--terragrunt-non-interactive' if non_interactive else ''
             parallelism_stmt  = f'--terragrunt-parallelism {limit_parallelism}' if limit_parallelism else ''
             include_dir_stmt  = f'--terragrunt-strict-include  --terragrunt-include-dir {" --terragrunt-include-dir ".join(include_dirs)}' if len(include_dirs) > 0 else ""
             exclude_dir_stmt  = f'--terragrunt-exclude-dir {" --terragrunt-exclude-dir ".join(exclude_dirs)}' if len(exclude_dirs) > 0 else ""
+
         else:
             base_command      = 'terragrunt'
             ignore_deps_stmt  = ''
             auto_approve_stmt = '' if no_auto_approve else '-auto-approve'
             interactive_stmt  = ''
             parallelism_stmt  = ''
             include_dir_stmt  = ''
@@ -210,14 +212,18 @@
         # ensure consistency, remove possible trailing slashes from the dirs                
         directory = directory.rstrip(os.path.sep)
 
         # ensure consistency, remove possible ./ prefixes from the dirs
         include_dirs = [dir.lstrip(f'.{os.path.sep}') for dir in include_dirs]
         exclude_dirs = [dir.lstrip(f'.{os.path.sep}') for dir in exclude_dirs]
 
+        # if the dir is not ending on '/*', add it
+        include_dirs = [dir.rstrip(f'.{os.path.sep}*') + f'{os.path.sep}*' for dir in include_dirs]
+        exclude_dirs = [dir.rstrip(f'.{os.path.sep}*') + f'{os.path.sep}*' for dir in exclude_dirs]
+
         common_path = os.path.commonpath([os.path.abspath(working_dir), os.path.abspath(directory)])
         self.printer.verbose(f'Common path for dir {directory}: {common_path}')
 
         if common_path != os.path.abspath(working_dir) \
             and exclude_external_dependencies:
             dir_excluded = True
             dir_excluded_reason = "directory out of scope"
@@ -647,15 +653,15 @@
 
         return stop_processing
 
     def _run_di_graph(
         self, command, exclude_external_dependencies, start_at_step, dry_run,
         parallel_execution=False, ask_for_confirmation=False, collect_output_file=None,
         backwards=False, working_dir=None, include_dirs=[], exclude_dirs=[],
-        use_native_terraform=False, add_to_workdir=None,
+        use_native_terraform=False, add_to_workdir=None, continue_on_error=False,
         ):
         "Runs the desired command in the directories as defined in the directed graph"
 
         if use_native_terraform:
             module_dirs = self._get_subdirectories_with_file(
                 root_dir = working_dir if working_dir else ".",
                 file_name=self.TERRAGRUNT_FILE,
@@ -744,15 +750,15 @@
                         add_to_workdir=add_to_workdir,
                         module=module,
                         collect_output_file=collect_output_file,
                         dry_run=dry_run,
                         progress=progress,
                     )
 
-                    if stop_processing:
+                    if stop_processing and not continue_on_error:
                         self.printer.warning(f"Processing needs to be stopped at step {step_nbr}.")
                         self.printer.normal(
                             f"After you've fixed the problem, you can continue where you left off by adding '--start-at-step {step_nbr}'."
                             )
                         sys.exit(1)
 
         if parallel_execution:
@@ -766,14 +772,158 @@
                 t.join()
                 collect_output_file.write(q.get())
 
         if self.printer.print_verbose:
             total_items = sum(len(group) for group in groups)
             self.printer.verbose(f'Executed {group_nbr} groups and {total_items} steps')
 
+    def _post_analyze_results_to_dce(self, data_collection_endpoint:str, payload:object):
+        """
+        Posts the payload to the given (Azure) data collection endpoint
+        """
+
+        #
+        # Everything we do here, can be done using native python. And probably this is preferable as well.
+        # But I have decided to follow (at least for now) the overall approach of the app and that is
+        # executing systems commands.
+        # This does require the az cli to be installed, but that is a fair assumption if you are working
+        # with terragrunt/terraform and want to post the analyze results to a Data Collection Endpoint.
+        # However, not ruling out this will change, but then the change should be transparant.
+        #
+
+        # Get the Azure information
+        rc = subprocess.run(
+            shlex.split('az account show'),
+            check=True,
+            stdout=subprocess.PIPE,
+            stderr=sys.stderr,
+        )
+        self.printer.verbose(rc)
+
+        # Do a few checks
+        if rc.returncode != 0:
+            raise Exception(f'Could not get Azure account info')
+        
+        # Get the ouptut
+        output = json.loads(rc.stdout.decode())
+        if output.get('environmentName') != 'AzureCloud':
+            raise Exception(f'Environment is not an Azure cloud:\n{json.dumps(output, indent=2)}')
+        
+        tenant_id = output.get('tenantId')
+        if not tenant_id:
+            raise Exception(f'Could not determine Azure tenant id:\n{json.dumps(output, indent=2)}')
+
+        principal = output.get('user').get('name')
+        if not principal:
+            raise Exception(f'Could not determine principal:\n{json.dumps(output, indent=2)}')
+
+        # TOKEN=$(az account get-access-token --scope "https://monitor.azure.com//.default" | jq -r '.accessToken')
+        # Get the Azure OAUTH token
+        rc = subprocess.run(
+            shlex.split('az account get-access-token --scope "https://monitor.azure.com//.default"'),
+            check=True,
+            stdout=subprocess.PIPE,
+            stderr=sys.stderr,
+        )
+        self.printer.verbose(rc.returncode) # do not print the token to output
+
+        # Do a few checks
+        if rc.returncode != 0:
+            raise Exception(f'Could not get Azure OAUTH token')
+        
+        # Get the ouptut
+        output = json.loads(rc.stdout.decode())
+        token = output.get('accessToken')
+        if not token:
+            raise Exception(f'Could not retrieve an access token:\n{json.dumps(output, indent=2)}')
+
+        # Get the repo info
+        rc = subprocess.run(
+            shlex.split('git config --get remote.origin.url'),
+            check=True,
+            stdout=subprocess.PIPE,
+            stderr=sys.stderr,
+        )
+        self.printer.verbose(rc)
+
+        # Do a few checks
+        if rc.returncode != 0:
+            raise Exception(f'Could not get git repo info')
+        
+        # Get the ouptut
+        repo = rc.stdout.decode().rstrip('\n')
+        if not repo:
+            raise Exception(f'Could not get git repo info: {repo}')
+
+        # Get the current path in the repo
+        rc = subprocess.run(
+            shlex.split('git rev-parse --show-prefix'),
+            check=True,
+            stdout=subprocess.PIPE,
+            stderr=sys.stderr,
+        )
+        self.printer.verbose(rc)
+
+        # Do a few checks
+        if rc.returncode != 0:
+            raise Exception(f'Could not get current scope')
+        
+        # Get the ouptut
+        scope = rc.stdout.decode().rstrip('\n')
+        if not scope:
+            raise Exception(f'Could not get scope: {scope}')
+
+        # So now we have everything, we can construct the final payload
+        dce_payload = [
+            {
+                "scope": scope,
+                "principal": principal,
+                "repo": repo,
+                "creations": payload.get("summary").get("creations"),
+                "updates": payload.get("summary").get("updates"),
+                "deletions": payload.get("summary").get("deletions"),
+                "minor": payload.get("summary").get("minor"),
+                "medium": payload.get("summary").get("medium"),
+                "major": payload.get("summary").get("major"),
+                "unknown": payload.get("summary").get("unknown"),
+                "total": payload.get("summary").get("total"),
+                "score": payload.get("summary").get("score"),
+                "details": payload.get('details'),
+            },
+        ]
+        
+        self.printer.verbose('About to log:')
+        self.printer.verbose(f'- to: {data_collection_endpoint}')
+        self.printer.verbose(f'- payload:\n{json.dumps(dce_payload, indent=2)}')
+
+        # now do the actual post
+        try:
+            headers = {
+                'Authorization': f"Bearer {token}",
+                'Content-Type': 'application/json',
+            }
+            resp = requests.post(
+                url=data_collection_endpoint,
+                headers=headers,
+                json=dce_payload,
+            )
+
+            resp.raise_for_status()
+
+        except requests.exceptions.RequestException as e:
+            # we warn but continue
+            self.printer.warning(f'Error while posting the analyze results ({type(e)}): {e}')
+        except Exception as e:
+            self.printer.error(f'Unexpected error: {e}')
+            if self.printer.print_verbose:
+                raise(e)
+            sys.exit(1)
+
+        self.printer.verbose('Done')
+
     def run(self, command, debug, dry_run, no_lock, update, upgrade,
         planfile, auto_approve, clean, working_dir, terragrunt_args):
         """ Executes a terragrunt command on a single module """
 
         self.printer.verbose(f"Attempting to execute 'run {command}'")
         if terragrunt_args:
             self.printer.verbose(f"- with additional parameters: {' '.join(terragrunt_args)}")
@@ -875,22 +1025,22 @@
             cmd = f"terraform show {json_stmt} {self.PLANFILE_NAME}"
 
         # the `posix=False` is to prevent the split command to remove quotes from strings,
         # e.g. when executing commands like this:
         # tgwrap state mv 'azuread_group.this["viewers"]' 'azuread_group.this["readers"]'
         rc = subprocess.run(
             shlex.split(cmd, posix=False),
-            cwd=cwd,
+            cwd=cwd if cwd else None,
             )
         self.printer.verbose(rc)
 
         sys.exit(rc.returncode)
 
     def run_all(self, command, debug, dry_run, no_lock, update, upgrade,
-        exclude_external_dependencies, step_by_step, planfile, auto_approve, clean,
+        exclude_external_dependencies, step_by_step, continue_on_error, planfile, auto_approve, clean,
         working_dir, start_at_step, limit_parallelism, include_dirs, exclude_dirs, terragrunt_args):
         """ Executes a terragrunt command across multiple modules """
 
         self.printer.verbose(f"Attempting to execute 'run-all {command}'")
         if terragrunt_args:
             self.printer.verbose(f"- with additional parameters: {' '.join(terragrunt_args)}")
 
@@ -920,19 +1070,24 @@
             self.clean(working_dir=working_dir)
 
         if step_by_step:
             self.printer.verbose(
                 f'This command will be executed for each individual module:\n$ {cmd}'
                 )
 
+            # if the dir is not ending on '/*', add it
+            include_dirs = [dir.rstrip(f'.{os.path.sep}*') + f'{os.path.sep}*' for dir in include_dirs]
+            exclude_dirs = [dir.rstrip(f'.{os.path.sep}*') + f'{os.path.sep}*' for dir in exclude_dirs]
+
             self._run_di_graph(
                 command=cmd,
                 exclude_external_dependencies=exclude_external_dependencies,
                 working_dir=working_dir,
                 ask_for_confirmation=(not auto_approve),
+                continue_on_error=continue_on_error,
                 dry_run=dry_run,
                 start_at_step=start_at_step,
                 backwards=True if command.lower() in ['destroy'] else False,
                 include_dirs=include_dirs,
                 exclude_dirs=exclude_dirs,
             )
         else:
@@ -987,16 +1142,16 @@
             rc = subprocess.run(
                 shlex.split(cmd, posix=False),
                 env=env,
             )
             self.printer.verbose(rc)
 
     def analyze(self, exclude_external_dependencies, working_dir, start_at_step,
-        out, analyze_config, parallel_execution,
-        include_dirs, exclude_dirs, planfile_dir, terragrunt_args):
+        out, analyze_config, parallel_execution, include_dirs, exclude_dirs, 
+        planfile_dir, data_collection_endpoint, terragrunt_args):
         """ Analyzes the plan files """
 
         def calculate_score(major: int, medium: int, minor: int) -> float :
             return major * 10 + medium + minor / 10
 
         self.printer.verbose("Attempting to 'analyze'")
         if terragrunt_args:
@@ -1037,15 +1192,15 @@
         else:
             self.printer.verbose(
                 f"\nAnalyze using config {analyze_config}"
                 )
             config = self.load_yaml_file(analyze_config)
 
         ts_validation_successful = True
-        changes = {}
+        details = {}
         drifts = {}
         try:
             # then run it and capture the output
             with tempfile.NamedTemporaryFile(mode='w+', prefix='tgwrap-', delete=False) as f:
                 self.printer.verbose(f"Opened temp file for output collection: {f.name}")
 
                 self._run_di_graph(
@@ -1079,15 +1234,15 @@
                         if len(plan_file) > 1:
                             data = json.loads(plan_file)
 
                             # do we have an exception logged?
                             if 'exception' in data:
                                 raise Exception(data['exception'])
 
-                            changes[module], ts_success = run_analyze(
+                            details[module], ts_success = run_analyze(
                                 config=config,
                                 data=data,
                                 verbose=self.printer.print_verbose,
                                 )
                             if not ts_success:
                                 ts_validation_successful = False
                         else:
@@ -1109,15 +1264,15 @@
             "major": 0,
             "unknown": 0,
             "total": 0,
             "score": 0,
         }
 
         self.printer.header("Analysis results:", print_line_before=True)
-        for key, value in changes.items():
+        for key, value in details.items():
             self.printer.header(f'Module: {key}')
             if not value["all"]:
                 self.printer.success('No changes detected')
             if value["unauthorized"]:
                 self.printer.error('Unauthorized deletions:')
                 for m in value["unauthorized"]:
                     self.printer.error(f'-> {m}')
@@ -1133,15 +1288,15 @@
                     self.printer.normal(f'-> {m}')
             if value["updates"]:
                 self.printer.normal('Updates:')
                 for m in value["updates"]:
                     total_drifts["updates"] = total_drifts["updates"] + 1
                     self.printer.normal(f'-> {m}')
 
-        for key, value in changes.items():
+        for key, value in details.items():
             for type in ["minor", "medium", "major", "unknown", "total"]:
                 total_drifts[type] += value["drifts"][type]
             
             # the formula below is just a way to achieve a numeric results that is coming from the various drift categories
             value['drifts']['score'] = calculate_score(
                 major = value['drifts']['major'],
                 medium = value['drifts']['medium'],
@@ -1153,32 +1308,39 @@
         total_drift_score = total_drifts['major'] * 10 + total_drifts['medium'] + total_drifts['minor'] / 10
         total_drifts['score'] = total_drift_score
 
         self.printer.header(f"Drift score: {total_drift_score} ({total_drifts['major']}.{total_drifts['medium']}.{total_drifts['minor']})")
         if total_drifts["unknown"] > 0:
             self.printer.warning(f"For {total_drifts['unknown']} resources, drift score is not configured, please update configuration!")
             self.printer.warning('- Unknowns:')
-            for key, value in changes.items():
+            for key, value in details.items():
                 for m in value["unknowns"]:
                     self.printer.warning(f' -> {m}')
 
-        if out:
+        if out or data_collection_endpoint:
             # in the output we convert the dict of dicts to a list of dicts as it makes processing
             # (e.g. by telegraph) easier.
             output = {
-                "changes": [],
+                "details": [],
                 "summary": {},
             }
-            for key, value in changes.items():
+            for key, value in details.items():
                 value['module'] = key
-                output["changes"].append(value)
+                output["details"].append(value)
 
             output["summary"] = total_drifts
 
-            print(json.dumps(output, indent=4))
+            if out:
+                print(json.dumps(output, indent=4))
+
+            if data_collection_endpoint:
+                self._post_analyze_results_to_dce(
+                    data_collection_endpoint=data_collection_endpoint,
+                    payload=output,
+                )
 
         if not ts_validation_successful:
             self.printer.error("Analysis detected unauthorised deletions, please check your configuration!!!")
             sys.exit(1)
 
     def set_lock(self, module, lock_status, auto_approve, dry_run, working_dir):
         """ Set the lock status of the stage you're in """
@@ -1301,14 +1463,18 @@
             for ss, substack in manifest.get('sub_stacks', {}).items():
                 # get the base directory of the sub stack so that we can ignore it when deploying the regular modules
                 substacks.append(substack['source'].split(os.path.sep)[0])
 
             # and make it unique
             substacks = set(substacks)
 
+            # the manifest file supports both `sub_stacks` and `substack` config name. Annoying to be a bit autistic when it comes to naming :-/
+            substack_configs = manifest.get('sub_stacks', {})
+            substack_configs.update(manifest.get('substacks', {}))
+
             for target_stage in target_stages:
                 target_dir = os.path.join(working_dir, '', target_stage)
                 self.printer.header(f'Deploy stage {target_stage} to {target_dir}...')
                 try:
                     os.makedirs(target_dir)
                 except FileExistsError:
                     pass
@@ -1324,15 +1490,15 @@
                                 step=key,
                                 config=value,
                                 source_dir=source_dir,
                                 source_config_dir=source_config_dir,
                                 target_dir=target_dir,
                                 target_stage=target_stage,
                                 substacks=substacks,
-                                substack_configs=manifest.get('sub_stacks', {}).items(),
+                                substack_configs=substack_configs.items(),
                                 tg_file_name=self.TERRAGRUNT_FILE,
                                 verbose=self.printer.print_verbose,
                             )
                         ) 
 
                 if include_global_config_files:
                     for gc, global_config in manifest.get('global_config_files', {}).items():
@@ -1564,17 +1730,14 @@
     def show_graph(self, backwards, exclude_external_dependencies, working_dir, include_dirs, exclude_dirs, terragrunt_args):
         """ Shows the dependencies of a project """
 
         self.printer.verbose(f"Attempting to show dependencies")
         if terragrunt_args:
             self.printer.verbose(f"- with additional parameters: {' '.join(terragrunt_args)}")
 
-        # self.printer.verbose(f"Include dirs: {'; '.join(include_dirs)}")
-        # self.printer.verbose(f"Exclude dirs: {'; '.join(exclude_dirs)}")
-
         "Runs the desired command in the directories as defined in the directed graph"
         graph = self._get_di_graph(backwards=backwards, working_dir=working_dir)
 
         # first go through the groups and clean up where needed
         groups = self._prepare_groups(
             graph=graph,
             exclude_external_dependencies=exclude_external_dependencies,
```

### Comparing `tgwrap-0.8.9/tgwrap/printer.py` & `tgwrap-0.9.0/tgwrap/printer.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.8.9/PKG-INFO` & `tgwrap-0.9.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgwrap
-Version: 0.8.9
+Version: 0.9.0
 Summary: A (terragrunt) wrapper around a (terraform) wrapper around ....
 Home-page: https://gitlab.com/lunadata/tgwrap
 License: MIT
 Keywords: terraform,terragrunt,terrasafe,python
 Author: Gerco Grandia
 Author-email: gerco.grandia@4synergy.nl
 Requires-Python: >=3.8,<4.0
@@ -138,14 +138,64 @@
 
 ```console
 export TGWRAP_PLANFILE_DIR=".terragrunt-cache/current"
 ```
 
 Or pass it along with the `--planfile-dir|-P` option and it will use that.
 
+### Logging the results
+
+`tgwrap` supports logging the analyze results to an [Azure Log Analytics](https://learn.microsoft.com/en-us/azure/azure-monitor/logs/log-analytics-overview) custom table.
+
+For that, the custom table need to be present, including a [data collection endpoint](https://learn.microsoft.com/en-us/azure/azure-monitor/essentials/data-collection-endpoint-overview?tabs=portal) and associated [data collection rule](https://learn.microsoft.com/en-us/azure/azure-monitor/essentials/data-collection-rule-overview?tabs=portal).
+
+When you want to activate this, just pass `--data-collection-endpoint` (or, more conveniently, set the `TGWRAP_ANALYZE_DATA_COLLECTION_ENDPOINT` environment variable) with the url to which the data can be posted.
+
+> Note that for this to work, `tgwrap` assumes that there is a functioning [azure cli](https://learn.microsoft.com/en-us/cli/azure/) available on the system.
+
+A payload as below will be posted, and the log analytics table should be able to accomodate for that:
+
+```json
+[
+  {
+    "scope": "terragrunt/dlzs/data-platform/global/platform/rbac/",
+    "principal": "myself",
+    "repo": "https://gitlab.com/my-git-repo.git",
+    "creations": 0,
+    "updates": 0,
+    "deletions": 0,
+    "minor": 0,
+    "medium": 0,
+    "major": 0,
+    "unknown": 0,
+    "total": 0,
+    "score": 0.0,
+    "details": [
+      {
+        "drifts": {
+          "minor": 0,
+          "medium": 0,
+          "major": 0,
+          "unknown": 0,
+          "total": 0,
+          "score": 0.0
+        },
+        "all": [],
+        "creations": [],
+        "updates": [],
+        "deletions": [],
+        "unauthorized": [],
+        "unknowns": [],
+        "module": ""
+      }
+    ]
+  }
+]
+```
+
 ## More than a wrapper
 
 Over time, tgwrap became more than a wrapper, blantly violating [#1 of the unix philosophy](https://en.wikipedia.org/wiki/Unix_philosophy#:~:text=The%20Unix%20philosophy%20is%20documented,%2C%20as%20yet%20unknown%2C%20program.): 'Make each program do one thing well'.
 
 For instance, the 'analyze' functionality is already an example, but more features such as deploying a landing zone has crept into the application. It makes sense for how we're using it, but we're fully aware this makes it less generically applicable.
 
 ## Usage
@@ -226,24 +276,26 @@
     include_modules: {} # omit or use an empty dict for all of them
       # or specify your modules as follows
       # base: {} # just a simple include
       # networking-connected: # or a bit more complicated
       #  - source: networking
       #  - target: networking-connected
 
-sub_stacks:
+substacks:
   is01:
     source: shared-integration/intsvc01
     target: integration/is01
     exclude_modules:  # a list of modules that will always be excluded, can be omitted
       - my-specific-module
     configs:
       - my-ss-config.hcl
       - ../my-ss-config-dir
   is02:
+    applies_to_stages: # optional list of stages to include the substack in
+      - dev
     source: shared-integration/intsvc01
     target: integration/is02
 
 # global configuration files that are deployed as well
 # note that these files are typically applicable to all landing zones and stages!
 # this might lead to unexpected behaviour
 # note that you can exclude syncing these files with a command line switch
```

