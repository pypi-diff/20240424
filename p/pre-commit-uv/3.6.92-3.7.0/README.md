# Comparing `tmp/pre_commit_uv-3.6.92.tar.gz` & `tmp/pre_commit_uv-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pre_commit_uv-3.6.92.tar", last modified: Fri Mar  1 19:24:43 2024, max compression
+gzip compressed data, was "pre_commit_uv-3.7.0.tar", last modified: Wed Apr 24 14:38:15 2024, max compression
```

## Comparing `pre_commit_uv-3.6.92.tar` & `pre_commit_uv-3.7.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:24:43.803836 pre_commit_uv-3.6.92/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-03-01 19:24:43.803836 pre_commit_uv-3.6.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:24:43.795836 pre_commit_uv-3.6.92/pre_commit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/all_languages.py
--rw-r--r--   0 runner    (1001) docker     (127)    12350 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/clientlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/color.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:24:43.795836 pre_commit_uv-3.6.92/pre_commit/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/commands/autoupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/commands/gc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9400 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/commands/hook_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/commands/init_templatedir.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/commands/install_uninstall.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/commands/migrate_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14143 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/commands/sample_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/commands/try_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/commands/validate_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/commands/validate_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/envcontext.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/lang_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:24:43.799836 pre_commit_uv-3.6.92/pre_commit/languages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/languages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/languages/conda.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/languages/coursier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/languages/dart.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/languages/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/languages/docker_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/languages/dotnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/languages/fail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/languages/golang.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/languages/haskell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/languages/lua.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/languages/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/languages/perl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/languages/pygrep.py
--rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/languages/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/languages/r.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/languages/ruby.py
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/languages/rust.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/languages/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/languages/swift.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/languages/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/logging_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    15564 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:24:43.799836 pre_commit_uv-3.6.92/pre_commit/meta_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/meta_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/meta_hooks/check_hooks_apply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/meta_hooks/check_useless_excludes.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/meta_hooks/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/parse_shebang.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     7938 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:24:43.803836 pre_commit_uv-3.6.92/pre_commit/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/resources/empty_template_.npmignore
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/resources/empty_template_Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/resources/empty_template_LICENSE.renv
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/resources/empty_template_Makefile.PL
--rw-r--r--   0 runner    (1001) docker     (127)    12037 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/resources/empty_template_activate.R
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/resources/empty_template_environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/resources/empty_template_go.mod
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/resources/empty_template_main.go
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/resources/empty_template_main.rs
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/resources/empty_template_package.json
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/resources/empty_template_pre-commit-package-dev-1.rockspec
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/resources/empty_template_pre_commit_placeholder_package.gemspec
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/resources/empty_template_pubspec.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/resources/empty_template_renv.lock
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/resources/empty_template_setup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      528 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/resources/hook-tmpl
--rw-r--r--   0 runner    (1001) docker     (127)    32551 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/resources/rbenv.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)    75808 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/resources/ruby-build.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/resources/ruby-download.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/staged_files_only.py
--rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/xargs.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/pre_commit/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:24:43.803836 pre_commit_uv-3.6.92/pre_commit_uv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-03-01 19:24:43.000000 pre_commit_uv-3.6.92/pre_commit_uv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-03-01 19:24:43.000000 pre_commit_uv-3.6.92/pre_commit_uv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 19:24:43.000000 pre_commit_uv-3.6.92/pre_commit_uv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-01 19:24:43.000000 pre_commit_uv-3.6.92/pre_commit_uv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-01 19:24:43.000000 pre_commit_uv-3.6.92/pre_commit_uv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-01 19:24:43.000000 pre_commit_uv-3.6.92/pre_commit_uv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-03-01 19:24:43.803836 pre_commit_uv-3.6.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-01 19:24:40.000000 pre_commit_uv-3.6.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:15.304863 pre_commit_uv-3.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-24 14:38:15.304863 pre_commit_uv-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:15.292863 pre_commit_uv-3.7.0/pre_commit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/all_languages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12350 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/clientlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/color.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:15.296863 pre_commit_uv-3.7.0/pre_commit/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/commands/autoupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/commands/gc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9400 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/commands/hook_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/commands/init_templatedir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/commands/install_uninstall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/commands/migrate_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14151 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/commands/sample_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/commands/try_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/commands/validate_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/commands/validate_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/envcontext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/lang_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:15.300863 pre_commit_uv-3.7.0/pre_commit/languages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/languages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/languages/conda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/languages/coursier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/languages/dart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/languages/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/languages/docker_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/languages/dotnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/languages/fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/languages/golang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/languages/haskell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/languages/lua.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/languages/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/languages/perl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/languages/pygrep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/languages/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/languages/r.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/languages/ruby.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/languages/rust.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/languages/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/languages/swift.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/languages/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/logging_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15564 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:15.300863 pre_commit_uv-3.7.0/pre_commit/meta_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/meta_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/meta_hooks/check_hooks_apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/meta_hooks/check_useless_excludes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/meta_hooks/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/parse_shebang.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7938 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:15.304863 pre_commit_uv-3.7.0/pre_commit/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/resources/empty_template_.npmignore
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/resources/empty_template_Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/resources/empty_template_LICENSE.renv
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/resources/empty_template_Makefile.PL
+-rw-r--r--   0 runner    (1001) docker     (127)    12037 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/resources/empty_template_activate.R
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/resources/empty_template_environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/resources/empty_template_go.mod
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/resources/empty_template_main.go
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/resources/empty_template_main.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/resources/empty_template_package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/resources/empty_template_pre-commit-package-dev-1.rockspec
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/resources/empty_template_pre_commit_placeholder_package.gemspec
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/resources/empty_template_pubspec.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/resources/empty_template_renv.lock
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/resources/empty_template_setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      528 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/resources/hook-tmpl
+-rw-r--r--   0 runner    (1001) docker     (127)    32551 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/resources/rbenv.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    75808 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/resources/ruby-build.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/resources/ruby-download.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/staged_files_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/xargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/pre_commit/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:15.304863 pre_commit_uv-3.7.0/pre_commit_uv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-24 14:38:15.000000 pre_commit_uv-3.7.0/pre_commit_uv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-24 14:38:15.000000 pre_commit_uv-3.7.0/pre_commit_uv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:38:15.000000 pre_commit_uv-3.7.0/pre_commit_uv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-24 14:38:15.000000 pre_commit_uv-3.7.0/pre_commit_uv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-24 14:38:15.000000 pre_commit_uv-3.7.0/pre_commit_uv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 14:38:15.000000 pre_commit_uv-3.7.0/pre_commit_uv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-24 14:38:15.308863 pre_commit_uv-3.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 14:38:11.000000 pre_commit_uv-3.7.0/setup.py
```

### Comparing `pre_commit_uv-3.6.92/LICENSE` & `pre_commit_uv-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/PKG-INFO` & `pre_commit_uv-3.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pre_commit_uv
-Version: 3.6.92
+Version: 3.7.0
 Summary: A framework for managing and maintaining multi-language pre-commit hooks (fork with uv support).
 Home-page: https://github.com/pre-commit/pre-commit
 Author: "Guilherme Espada, Anthony Sottile"
 Author-email: gjespada@fc.ul.pt
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pre_commit_uv-3.6.92/pre_commit/all_languages.py` & `pre_commit_uv-3.7.0/pre_commit/all_languages.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/clientlib.py` & `pre_commit_uv-3.7.0/pre_commit/clientlib.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/color.py` & `pre_commit_uv-3.7.0/pre_commit/color.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/commands/autoupdate.py` & `pre_commit_uv-3.7.0/pre_commit/commands/autoupdate.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/commands/gc.py` & `pre_commit_uv-3.7.0/pre_commit/commands/gc.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/commands/hook_impl.py` & `pre_commit_uv-3.7.0/pre_commit/commands/hook_impl.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/commands/init_templatedir.py` & `pre_commit_uv-3.7.0/pre_commit/commands/init_templatedir.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/commands/install_uninstall.py` & `pre_commit_uv-3.7.0/pre_commit/commands/install_uninstall.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/commands/migrate_config.py` & `pre_commit_uv-3.7.0/pre_commit/commands/migrate_config.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/commands/run.py` & `pre_commit_uv-3.7.0/pre_commit/commands/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,15 +294,15 @@
     prior_diff = _get_diff()
     for hook in hooks:
         current_retval, prior_diff = _run_single_hook(
             classifier, hook, skips, cols, prior_diff,
             verbose=args.verbose, use_color=args.color,
         )
         retval |= current_retval
-        if retval and (config['fail_fast'] or hook.fail_fast):
+        if current_retval and (config['fail_fast'] or hook.fail_fast):
             break
     if retval and args.show_diff_on_failure and prior_diff:
         if args.all_files:
             output.write_line(
                 'pre-commit hook(s) made changes.\n'
                 'If you are seeing this message in CI, '
                 'reproduce locally with: `pre-commit run --all-files`.\n'
```

### Comparing `pre_commit_uv-3.6.92/pre_commit/commands/try_repo.py` & `pre_commit_uv-3.7.0/pre_commit/commands/try_repo.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/envcontext.py` & `pre_commit_uv-3.7.0/pre_commit/envcontext.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/error_handler.py` & `pre_commit_uv-3.7.0/pre_commit/error_handler.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/file_lock.py` & `pre_commit_uv-3.7.0/pre_commit/file_lock.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/git.py` & `pre_commit_uv-3.7.0/pre_commit/git.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/hook.py` & `pre_commit_uv-3.7.0/pre_commit/hook.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/lang_base.py` & `pre_commit_uv-3.7.0/pre_commit/lang_base.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/languages/conda.py` & `pre_commit_uv-3.7.0/pre_commit/languages/conda.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/languages/coursier.py` & `pre_commit_uv-3.7.0/pre_commit/languages/coursier.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/languages/dart.py` & `pre_commit_uv-3.7.0/pre_commit/languages/dart.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/languages/docker.py` & `pre_commit_uv-3.7.0/pre_commit/languages/docker.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,18 +104,23 @@
 def get_docker_user() -> tuple[str, ...]:  # pragma: win32 no cover
     try:
         return ('-u', f'{os.getuid()}:{os.getgid()}')
     except AttributeError:
         return ()
 
 
-def docker_cmd() -> tuple[str, ...]:  # pragma: win32 no cover
+def get_docker_tty(*, color: bool) -> tuple[str, ...]:  # pragma: win32 no cover  # noqa: E501
+    return (('--tty',) if color else ())
+
+
+def docker_cmd(*, color: bool) -> tuple[str, ...]:  # pragma: win32 no cover
     return (
         'docker', 'run',
         '--rm',
+        *get_docker_tty(color=color),
         *get_docker_user(),
         # https://docs.docker.com/engine/reference/commandline/run/#mount-volumes-from-container-volumes-from
         # The `Z` option tells Docker to label the content with a private
         # unshared label. Only the current container can use a private volume.
         '-v', f'{_get_docker_path(os.getcwd())}:/src:rw,Z',
         '--workdir', '/src',
     )
@@ -135,12 +140,12 @@
     # automated cleanup of docker images.
     build_docker_image(prefix, pull=False)
 
     entry_exe, *cmd_rest = lang_base.hook_cmd(entry, args)
 
     entry_tag = ('--entrypoint', entry_exe, docker_tag(prefix))
     return lang_base.run_xargs(
-        (*docker_cmd(), *entry_tag, *cmd_rest),
+        (*docker_cmd(color=color), *entry_tag, *cmd_rest),
         file_args,
         require_serial=require_serial,
         color=color,
     )
```

### Comparing `pre_commit_uv-3.6.92/pre_commit/languages/docker_image.py` & `pre_commit_uv-3.7.0/pre_commit/languages/docker_image.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,14 +19,14 @@
         args: Sequence[str],
         file_args: Sequence[str],
         *,
         is_local: bool,
         require_serial: bool,
         color: bool,
 ) -> tuple[int, bytes]:  # pragma: win32 no cover
-    cmd = docker_cmd() + lang_base.hook_cmd(entry, args)
+    cmd = docker_cmd(color=color) + lang_base.hook_cmd(entry, args)
     return lang_base.run_xargs(
         cmd,
         file_args,
         require_serial=require_serial,
         color=color,
     )
```

### Comparing `pre_commit_uv-3.6.92/pre_commit/languages/dotnet.py` & `pre_commit_uv-3.7.0/pre_commit/languages/dotnet.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/languages/fail.py` & `pre_commit_uv-3.7.0/pre_commit/languages/fail.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/languages/golang.py` & `pre_commit_uv-3.7.0/pre_commit/languages/golang.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/languages/haskell.py` & `pre_commit_uv-3.7.0/pre_commit/languages/haskell.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/languages/lua.py` & `pre_commit_uv-3.7.0/pre_commit/languages/lua.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/languages/node.py` & `pre_commit_uv-3.7.0/pre_commit/languages/node.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/languages/perl.py` & `pre_commit_uv-3.7.0/pre_commit/languages/perl.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/languages/pygrep.py` & `pre_commit_uv-3.7.0/pre_commit/languages/pygrep.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/languages/python.py` & `pre_commit_uv-3.7.0/pre_commit/languages/python.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/languages/r.py` & `pre_commit_uv-3.7.0/pre_commit/languages/r.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/languages/ruby.py` & `pre_commit_uv-3.7.0/pre_commit/languages/ruby.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/languages/rust.py` & `pre_commit_uv-3.7.0/pre_commit/languages/rust.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/languages/script.py` & `pre_commit_uv-3.7.0/pre_commit/languages/script.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/languages/swift.py` & `pre_commit_uv-3.7.0/pre_commit/languages/swift.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/logging_handler.py` & `pre_commit_uv-3.7.0/pre_commit/logging_handler.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/main.py` & `pre_commit_uv-3.7.0/pre_commit/main.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/meta_hooks/check_hooks_apply.py` & `pre_commit_uv-3.7.0/pre_commit/meta_hooks/check_hooks_apply.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/meta_hooks/check_useless_excludes.py` & `pre_commit_uv-3.7.0/pre_commit/meta_hooks/check_useless_excludes.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/output.py` & `pre_commit_uv-3.7.0/pre_commit/output.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/parse_shebang.py` & `pre_commit_uv-3.7.0/pre_commit/parse_shebang.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/repository.py` & `pre_commit_uv-3.7.0/pre_commit/repository.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/resources/empty_template_LICENSE.renv` & `pre_commit_uv-3.7.0/pre_commit/resources/empty_template_LICENSE.renv`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/resources/empty_template_activate.R` & `pre_commit_uv-3.7.0/pre_commit/resources/empty_template_activate.R`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/resources/hook-tmpl` & `pre_commit_uv-3.7.0/pre_commit/resources/hook-tmpl`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/resources/rbenv.tar.gz` & `pre_commit_uv-3.7.0/pre_commit/resources/rbenv.tar.gz`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/resources/ruby-build.tar.gz` & `pre_commit_uv-3.7.0/pre_commit/resources/ruby-build.tar.gz`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/resources/ruby-download.tar.gz` & `pre_commit_uv-3.7.0/pre_commit/resources/ruby-download.tar.gz`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/staged_files_only.py` & `pre_commit_uv-3.7.0/pre_commit/staged_files_only.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/store.py` & `pre_commit_uv-3.7.0/pre_commit/store.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/util.py` & `pre_commit_uv-3.7.0/pre_commit/util.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit/xargs.py` & `pre_commit_uv-3.7.0/pre_commit/xargs.py`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/pre_commit_uv.egg-info/PKG-INFO` & `pre_commit_uv-3.7.0/pre_commit_uv.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pre_commit_uv
-Version: 3.6.92
+Version: 3.7.0
 Summary: A framework for managing and maintaining multi-language pre-commit hooks (fork with uv support).
 Home-page: https://github.com/pre-commit/pre-commit
 Author: "Guilherme Espada, Anthony Sottile"
 Author-email: gjespada@fc.ul.pt
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pre_commit_uv-3.6.92/pre_commit_uv.egg-info/SOURCES.txt` & `pre_commit_uv-3.7.0/pre_commit_uv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pre_commit_uv-3.6.92/setup.cfg` & `pre_commit_uv-3.7.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pre_commit_uv
-version = 3.6.92
+version = 3.7.0
 description = A framework for managing and maintaining multi-language pre-commit hooks (fork with uv support).
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pre-commit/pre-commit
 author = "Guilherme Espada, Anthony Sottile"
 author_email = gjespada@fc.ul.pt
 license = MIT
```

