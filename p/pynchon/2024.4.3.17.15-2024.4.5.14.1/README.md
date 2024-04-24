# Comparing `tmp/pynchon-2024.4.3.17.15.tar.gz` & `tmp/pynchon-2024.4.5.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynchon-2024.4.3.17.15.tar", last modified: Wed Apr  3 17:15:50 2024, max compression
+gzip compressed data, was "pynchon-2024.4.5.14.1.tar", last modified: Fri Apr  5 14:01:10 2024, max compression
```

## Comparing `pynchon-2024.4.3.17.15.tar` & `pynchon-2024.4.5.14.1.tar`

### file list

```diff
@@ -1,297 +1,297 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.255286 pynchon-2024.4.3.17.15/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-03 17:15:50.255286 pynchon-2024.4.3.17.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-03 17:15:50.255286 pynchon-2024.4.3.17.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.191285 pynchon-2024.4.3.17.15/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.207285 pynchon-2024.4.3.17.15/src/pynchon/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 17:15:47.000000 pynchon-2024.4.3.17.15/src/pynchon/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.207285 pynchon-2024.4.3.17.15/src/pynchon/abcs/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/abcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/abcs/attrdict.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/abcs/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/abcs/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/abcs/visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/annotate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.211285 pynchon-2024.4.3.17.15/src/pynchon/api/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.211285 pynchon-2024.4.3.17.15/src/pynchon/api/git/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/api/git/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.211285 pynchon-2024.4.3.17.15/src/pynchon/api/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/api/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.211285 pynchon-2024.4.3.17.15/src/pynchon/api/project/
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/api/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/api/pynchon.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/api/render.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/app.py
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/bin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.211285 pynchon-2024.4.3.17.15/src/pynchon/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/cli/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.211285 pynchon-2024.4.3.17.15/src/pynchon/codemod/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/codemod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.211285 pynchon-2024.4.3.17.15/src/pynchon/codemod/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/codemod/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.211285 pynchon-2024.4.3.17.15/src/pynchon/codemod/commands/docstrings/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/codemod/commands/docstrings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/codemod/commands/docstrings/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/codemod/commands/docstrings/javadoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/codemod/commands/docstrings/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.211285 pynchon-2024.4.3.17.15/src/pynchon/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/config/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.215285 pynchon-2024.4.3.17.15/src/pynchon/models/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/models/planner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/models/planning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.215285 pynchon-2024.4.3.17.15/src/pynchon/models/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/models/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/models/plugins/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/models/plugins/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/models/plugins/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/models/plugins/pynchon.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/models/plugins/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/models/plugins/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/models/python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.219285 pynchon-2024.4.3.17.15/src/pynchon/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/__template__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/cicd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/deck.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/dockerhub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.223285 pynchon-2024.4.3.17.15/src/pynchon/plugins/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/docs/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/docs/opener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.223285 pynchon-2024.4.3.17.15/src/pynchon/plugins/doctor/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/doctor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/drawio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/fixme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/github.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/griffe.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/makefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/mermaid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/mkdocs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/pandoc.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    14638 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.223285 pynchon-2024.4.3.17.15/src/pynchon/plugins/python/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/python/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17560 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/python/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/python/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/python/cst.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/python/libcst.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/python/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/python/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/python/pypi.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/release.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/render.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/rtd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.223285 pynchon-2024.4.3.17.15/src/pynchon/plugins/scaffolding/
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/scaffolding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/scaffolding/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/src.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/tox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/tagging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.195285 pynchon-2024.4.3.17.15/src/pynchon/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.223285 pynchon-2024.4.3.17.15/src/pynchon/templates/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/docker/Dockerfile.pandoc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.223285 pynchon-2024.4.3.17.15/src/pynchon/templates/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.191285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.195285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.223285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/github/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/github/header.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.195285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.227285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/VERSIONS.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.227285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bash.sh
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bashrc.sh
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/makefile.j2
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/python.j2
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.227285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/fixme/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/fixme/FIXME.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.227285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/makefile/
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/makefile/mermaid-graph.mmd.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.195285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.227285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/TOC.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/modules.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/names.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.195285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/gen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.227285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/function.txt.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/module.txt.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.231285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python_cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python_cli/TOC.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python_cli/detail.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python_cli/main.module.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python_cli/script.console.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python_cli/subcommand.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.195285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.231285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/src/header/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/src/header/jinja-md.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/src/header/jinja.j2
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/src/header/python.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.231285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.195285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/ansible/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.231285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/ansible/role/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/ansible/role/.ansible-lint
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.195285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/ansible/role/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.231285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/ansible/role/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/ansible/role/.github/workflows/ansible-lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/ansible/role/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.231285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/docker/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/docker/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/docker/.scaffold.advice.json5
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/docker/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.199285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.231285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/docs/includes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/docs/includes/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.231285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.199285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/github/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.231285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/github/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/github/.github/workflows/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/github/.github/workflows/hello-world.yml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/github/.scaffold.advice.json5
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/github/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.199285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.235285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/.ackrc
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/.libcst.codemod.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/.scaffold.advice.json5
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.235285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/docs/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.235285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/docs/html/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/docs/html/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.199285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.235285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/app.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/lme.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/tagging.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.239285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.239285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/integration/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/integration/test_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.239285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/test_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.239285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/units/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/units/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/units/test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.239285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/workspace/.scaffold.advice.json5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.199285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.239285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/automation/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/automation/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.239285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/tests/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.203285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/tests/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.239285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/tests/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/tests/tests/integration/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.239285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/tests/tests/smoke/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/tests/tests/smoke/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.239285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/tests/tests/units/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/tests/tests/units/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.243285 pynchon-2024.4.3.17.15/src/pynchon/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/complexity.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.243285 pynchon-2024.4.3.17.15/src/pynchon/util/console/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/console/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.243285 pynchon-2024.4.3.17.15/src/pynchon/util/files/
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/files/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/files/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/lme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.243285 pynchon-2024.4.3.17.15/src/pynchon/util/makefile/
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/makefile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/makefile/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/oop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.243285 pynchon-2024.4.3.17.15/src/pynchon/util/os/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/os/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/os/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/os/pidfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/os/pids.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/python.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/splitvt.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.251285 pynchon-2024.4.3.17.15/src/pynchon/util/text/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/text/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.251285 pynchon-2024.4.3.17.15/src/pynchon/util/text/dumpf/
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/text/dumpf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/text/dumpf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/text/dumps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.251285 pynchon-2024.4.3.17.15/src/pynchon/util/text/loadf/
--rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/text/loadf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/text/loadf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/text/loads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.251285 pynchon-2024.4.3.17.15/src/pynchon/util/text/normalize/
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/text/normalize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.251285 pynchon-2024.4.3.17.15/src/pynchon/util/text/render/
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/text/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/text/render/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.251285 pynchon-2024.4.3.17.15/src/pynchon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-03 17:15:50.000000 pynchon-2024.4.3.17.15/src/pynchon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-04-03 17:15:50.000000 pynchon-2024.4.3.17.15/src/pynchon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:15:50.000000 pynchon-2024.4.3.17.15/src/pynchon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 17:15:50.000000 pynchon-2024.4.3.17.15/src/pynchon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:15:50.000000 pynchon-2024.4.3.17.15/src/pynchon.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-03 17:15:50.000000 pynchon-2024.4.3.17.15/src/pynchon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 17:15:50.000000 pynchon-2024.4.3.17.15/src/pynchon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.440942 pynchon-2024.4.5.14.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-05 14:01:10.440942 pynchon-2024.4.5.14.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27572 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-05 14:01:10.444942 pynchon-2024.4.5.14.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.368942 pynchon-2024.4.5.14.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.380942 pynchon-2024.4.5.14.1/src/pynchon/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-05 14:01:07.000000 pynchon-2024.4.5.14.1/src/pynchon/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.384942 pynchon-2024.4.5.14.1/src/pynchon/abcs/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/abcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/abcs/attrdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/abcs/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/abcs/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/abcs/visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/annotate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.384942 pynchon-2024.4.5.14.1/src/pynchon/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.384942 pynchon-2024.4.5.14.1/src/pynchon/api/git/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/api/git/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.384942 pynchon-2024.4.5.14.1/src/pynchon/api/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/api/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.384942 pynchon-2024.4.5.14.1/src/pynchon/api/project/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/api/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/api/pynchon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7341 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/api/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/bin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.384942 pynchon-2024.4.5.14.1/src/pynchon/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/cli/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.384942 pynchon-2024.4.5.14.1/src/pynchon/codemod/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/codemod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.384942 pynchon-2024.4.5.14.1/src/pynchon/codemod/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/codemod/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.384942 pynchon-2024.4.5.14.1/src/pynchon/codemod/commands/docstrings/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/codemod/commands/docstrings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/codemod/commands/docstrings/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/codemod/commands/docstrings/javadoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/codemod/commands/docstrings/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.388942 pynchon-2024.4.5.14.1/src/pynchon/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/config/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.388942 pynchon-2024.4.5.14.1/src/pynchon/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9273 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/models/planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/models/planning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.388942 pynchon-2024.4.5.14.1/src/pynchon/models/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/models/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/models/plugins/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/models/plugins/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/models/plugins/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/models/plugins/pynchon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/models/plugins/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/models/plugins/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/models/python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.396942 pynchon-2024.4.5.14.1/src/pynchon/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/__template__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/cicd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/deck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/dockerhub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.396942 pynchon-2024.4.5.14.1/src/pynchon/plugins/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/docs/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/docs/opener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.396942 pynchon-2024.4.5.14.1/src/pynchon/plugins/doctor/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/doctor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/drawio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/fixme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/griffe.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8015 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/mkdocs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/pandoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14638 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.396942 pynchon-2024.4.5.14.1/src/pynchon/plugins/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/python/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17587 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/python/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/python/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/python/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/python/libcst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/python/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/python/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/python/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/rtd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.396942 pynchon-2024.4.5.14.1/src/pynchon/plugins/scaffolding/
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/scaffolding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/scaffolding/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7353 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/src.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/tagging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.372942 pynchon-2024.4.5.14.1/src/pynchon/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.396942 pynchon-2024.4.5.14.1/src/pynchon/templates/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/docker/Dockerfile.pandoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.400942 pynchon-2024.4.5.14.1/src/pynchon/templates/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.372942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.400942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.400942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/github/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/github/header.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.372942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.400942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/VERSIONS.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.400942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bash.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bashrc.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/makefile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/python.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.400942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/fixme/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/fixme/FIXME.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.400942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/makefile/
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/makefile/mermaid-graph.mmd.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.372942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.400942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/TOC.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/modules.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/names.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.372942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/gen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.404942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/function.txt.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/module.txt.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.404942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python_cli/TOC.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python_cli/detail.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python_cli/main.module.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python_cli/script.console.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python_cli/subcommand.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.372942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.404942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/src/header/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/src/header/jinja-md.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/src/header/jinja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/src/header/python.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/pydantic-model.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.404942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.372942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/ansible/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.404942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/ansible/role/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/ansible/role/.ansible-lint
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.372942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/ansible/role/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.404942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/ansible/role/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/ansible/role/.github/workflows/ansible-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/ansible/role/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.404942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/docker/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/docker/.scaffold.advice.json5
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/docker/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.372942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.404942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/docs/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/docs/includes/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.404942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.372942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/github/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.408942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/github/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/github/.github/workflows/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/github/.github/workflows/hello-world.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/github/.scaffold.advice.json5
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/github/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.376942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.408942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/.ackrc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/.libcst.codemod.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/.scaffold.advice.json5
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.408942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/docs/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.408942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/docs/html/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/docs/html/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.376942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.412942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/lme.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/tagging.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.412942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.412942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/integration/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/integration/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.416942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.416942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/units/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/units/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/units/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.416942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/workspace/.scaffold.advice.json5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.376942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.416942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/automation/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/automation/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.416942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/tests/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.376942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/tests/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.420942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/tests/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/tests/tests/integration/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.420942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/tests/tests/smoke/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/tests/tests/smoke/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.420942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/tests/tests/units/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/tests/tests/units/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.424942 pynchon-2024.4.5.14.1/src/pynchon/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/complexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.428942 pynchon-2024.4.5.14.1/src/pynchon/util/console/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/console/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.428942 pynchon-2024.4.5.14.1/src/pynchon/util/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/files/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/files/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/lme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.428942 pynchon-2024.4.5.14.1/src/pynchon/util/makefile/
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/makefile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/makefile/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/oop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.432942 pynchon-2024.4.5.14.1/src/pynchon/util/os/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/os/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/os/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/os/pidfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/os/pids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/splitvt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.432942 pynchon-2024.4.5.14.1/src/pynchon/util/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/text/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.436941 pynchon-2024.4.5.14.1/src/pynchon/util/text/dumpf/
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/text/dumpf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/text/dumpf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/text/dumps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.436941 pynchon-2024.4.5.14.1/src/pynchon/util/text/loadf/
+-rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/text/loadf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/text/loadf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/text/loads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.436941 pynchon-2024.4.5.14.1/src/pynchon/util/text/normalize/
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/text/normalize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.440942 pynchon-2024.4.5.14.1/src/pynchon/util/text/render/
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/text/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/text/render/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.440942 pynchon-2024.4.5.14.1/src/pynchon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-05 14:01:10.000000 pynchon-2024.4.5.14.1/src/pynchon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9308 2024-04-05 14:01:10.000000 pynchon-2024.4.5.14.1/src/pynchon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:01:10.000000 pynchon-2024.4.5.14.1/src/pynchon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 14:01:10.000000 pynchon-2024.4.5.14.1/src/pynchon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:01:10.000000 pynchon-2024.4.5.14.1/src/pynchon.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-05 14:01:10.000000 pynchon-2024.4.5.14.1/src/pynchon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 14:01:10.000000 pynchon-2024.4.5.14.1/src/pynchon.egg-info/top_level.txt
```

### Comparing `pynchon-2024.4.3.17.15/PKG-INFO` & `pynchon-2024.4.5.14.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynchon
-Version: 2024.4.3.17.15
+Version: 2024.4.5.14.1
 Summary: Autodocs for python projects
 Home-page: https://github.com/elo-enterprises/pynchon/
 Author: elo
 Author-email: engineering@elo.enterprises
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/pynchon/
 Project-URL: Source, https://github.com/elo-enterprises/pynchon/
@@ -12,15 +12,15 @@
 Platform: any
 Classifier: Programming Language :: Python
 Requires-Python: >3.6
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Requires-Dist: gripe>=2024.2.24.1.31
 Requires-Dist: shil>=2023.7.17.7.1
 Requires-Dist: shimport>=2023.7.11.23.36
-Requires-Dist: fleks==2024.2.9.23.58
+Requires-Dist: fleks==2024.4.5.9.29
 Requires-Dist: memoization==0.4.0
 Requires-Dist: multipledispatch==0.6.0
 Requires-Dist: pygments
 Requires-Dist: pyjson5==1.6.1
 Requires-Dist: marko==2.0.0
 Requires-Dist: pyyaml
 Requires-Dist: trogon
```

### Comparing `pynchon-2024.4.3.17.15/pyproject.toml` & `pynchon-2024.4.5.14.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/setup.cfg` & `pynchon-2024.4.5.14.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 package_dir = 
 	=src
 python_requires = >3.6
 install_requires = 
 	gripe>=2024.2.24.1.31
 	shil>=2023.7.17.7.1
 	shimport>=2023.7.11.23.36
-	fleks==2024.2.9.23.58
+	fleks==2024.4.5.9.29
 	memoization==0.4.0
 	multipledispatch==0.6.0
 	
 	pygments
 	pyjson5==1.6.1
 	marko==2.0.0     # parsing markdown
 	pyyaml           # parsing yaml
```

### Comparing `pynchon-2024.4.3.17.15/setup.py` & `pynchon-2024.4.5.14.1/setup.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/abcs/attrdict.py` & `pynchon-2024.4.5.14.1/src/pynchon/abcs/attrdict.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/abcs/path.py` & `pynchon-2024.4.5.14.1/src/pynchon/abcs/path.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/abcs/visitor.py` & `pynchon-2024.4.5.14.1/src/pynchon/abcs/visitor.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/annotate.py` & `pynchon-2024.4.5.14.1/src/pynchon/annotate.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/api/project/__init__.py` & `pynchon-2024.4.5.14.1/src/pynchon/api/project/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/api/render.py` & `pynchon-2024.4.5.14.1/src/pynchon/api/render.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,16 +55,18 @@
     events.lifecycle.send(__name__, msg="finalizing jinja globals")
 
     def is_markdown_list_item(text: str):
         return text.rstrip().startswith("* ")
 
     def invoke_helper(*args, **kwargs) -> typing.StringMaybe:
         """A jinja filter/extension"""
+        strict = kwargs.pop("strict", True)
         out = invoke(*args, **kwargs)
-        assert out.succeeded
+        if not out.succeeded:
+            raise Exception(out)
         return out.stdout
 
     def markdown_toc(fname: str, level=None):
         """ """
         import markdown
 
         with open(fname) as fhandle:
@@ -84,14 +86,15 @@
     # result = invoke(
     #     f"markdown-toc --type github --no-write {fname}",
     #     command_logger=LOGGER.critical
     # )
     # assert result.succeeded
     # return result.stdout
     return dict(
+        str=str,
         sh=invoke_helper,
         bash=invoke_helper,
         is_markdown_list_item=is_markdown_list_item,
         invoke=invoke_helper,
         map=map,
         markdown_toc=markdown_toc,
         eval=eval,
@@ -146,32 +149,14 @@
 
         msg = "Known template search paths (includes folders only): "
         tmp = list({p.parents[0] for p in known_templates})
         LOGGER.info(msg + util_text.to_json(tmp))
     return env
 
 
-def get_template_from_string(content, **kwargs):
-    """ """
-    return get_template(from_string=content, **kwargs)
-
-
-def get_template_from_file(
-    file: str = None,
-    **kwargs,
-):
-    """
-    :param file: str = None:
-    :param **kwargs:
-    """
-    with open(file) as fhandle:
-        content = fhandle.read()
-    return get_template_from_string(content, file=file, **kwargs)
-
-
 def get_template(
     template_name: typing.Union[str, abcs.Path] = None,
     env=None,
     from_string: str = None,
     **jinja_context,
 ):
     """ """
@@ -234,10 +219,28 @@
         panic=panic,
     )
 
     template.render = functools.partial(template.render, **jinja_context)
     return template
 
 
+def get_template_from_string(content, **kwargs):
+    """ """
+    return get_template(from_string=content, **kwargs)
+
+
+def get_template_from_file(
+    file: str = None,
+    **kwargs,
+):
+    """
+    :param file: str = None:
+    :param **kwargs:
+    """
+    with open(file) as fhandle:
+        content = fhandle.read()
+    return get_template_from_string(content, file=file, **kwargs)
+
+
 def clean_whitespace(txt: str):
     # return txt
     return "\n".join([x for x in txt.split("\n") if x.strip()])
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/app.py` & `pynchon-2024.4.5.14.1/src/pynchon/app.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/bin.py` & `pynchon-2024.4.5.14.1/src/pynchon/bin.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,29 +37,30 @@
     plugins: str = "",
     set_config: str = "",  # noqa
     get_config: str = "",
 ):
     """ """
 
 
-def bootstrap():
-    """
-    :param :
-    """
+def bootstrap(plugins: list = []):
+    """ """
+    from pynchon import constants
     from pynchon.app import app
+
+    constants.PLUGINS = plugins
     from pynchon.plugins import registry as plugin_registry
 
     from pynchon import config  # isort: skip
 
     events = app.events
     events.lifecycle.send(__name__, stage="Building CLIs from plugins..")
     registry = click_registry = {}
     loop = plugin_registry.items()
     for name, plugin_meta in loop:
-        if name not in config.PLUGINS:
+        if name not in config.PLUGINS + constants.PLUGINS:
             LOGGER.warning(f"skipping `{name}`")
             continue
         plugin_kls = plugin_meta["kls"]
         init_fxn = plugin_kls.init_cli
         # LOGGER.critical(f'\t{name}.init_cli: {init_fxn}')
         try:
             p_entry = init_fxn()
@@ -86,10 +87,10 @@
 def default(
     ctx, plugins: str = "", set_config: str = "", get_config: str = "", **kwargs  # noqa
 ):
     """this is always executed, regardless of subcommands and before them"""
     # LOGGER.critical('top-level')
     setters = ctx.params.get("set_config", []) or []
     plugins = ctx.params.get("plugins", "")
-    plugins and setters.append([f'pynchon.plugins={plugins.split(",")}'])
+    # plugins and setters.append(f'pynchon.plugins+={}')
     setters and LOGGER.critical(f"--set: {setters}")
-    bootstrap()
+    bootstrap(plugins=plugins.split(",") if plugins else [])
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/cli/common.py` & `pynchon-2024.4.5.14.1/src/pynchon/cli/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         out.append(
             kommand(
                 name=alias.replace("_", "-"),
                 parent=entry,
                 help=(
                     fxn.__doc__
                     if alias == fxn.__name__
-                    else f"alias for `{fxn.__name__}`"
+                    else f"Alias for `{fxn.__name__}`"
                 ),
             )(fxn)
         )
     return out
 
 
 class groop(kommand):
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/codemod/commands/docstrings/base.py` & `pynchon-2024.4.5.14.1/src/pynchon/codemod/commands/docstrings/base.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/codemod/commands/docstrings/javadoc.py` & `pynchon-2024.4.5.14.1/src/pynchon/codemod/commands/docstrings/javadoc.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/codemod/commands/docstrings/simple.py` & `pynchon-2024.4.5.14.1/src/pynchon/codemod/commands/docstrings/simple.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/config/__init__.py` & `pynchon-2024.4.5.14.1/src/pynchon/config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
 pynchon = PYNCHON = CoreConfig(
     skip_instance_validation=True,  # still bootstrapping..
     config_files=CONFIG_FILES,
     **MERGED_CONFIG_FILES,
 )
 RAW = PYNCHON.copy()
+# from pynchon.constants import CLI_SETTERS
 PLUGINS = PYNCHON["plugins"]
 LOGGER.warning(f"plugins: {PLUGINS}")
 # FIXME: get from registry or mcls
 _all_names = PLUGINS + Meta.NAMES
 
 msg = "Splitting core config.."
 events.lifecycle.send(
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/config/util.py` & `pynchon-2024.4.5.14.1/src/pynchon/config/util.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/constants.py` & `pynchon-2024.4.5.14.1/src/pynchon/constants.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/core.py` & `pynchon-2024.4.5.14.1/src/pynchon/core.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/events.py` & `pynchon-2024.4.5.14.1/src/pynchon/events.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/models/planner.py` & `pynchon-2024.4.5.14.1/src/pynchon/models/planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,21 @@
 LOGGER = lme.get_logger(" ")
 
 
 @tags(cli_label="Planner")
 class AbstractPlanner(BasePlugin):
     """A plugin-type that provides plan/apply basics"""
 
+    cli_label = "Planner"
+
     def _list(self, use_glob=None, changes=False):
         """
         Lists affected resources for this project
         """
-        use_glob = use_glob or getattr(self.__class__, "file_glob", None)
+        use_glob = use_glob or getattr(self.config, "file_glob", None)
         assert use_glob
         default = self[:"project"]
         proj_conf = self[:"project.subproject":default]
         project_root = proj_conf.get("root", None) or self[:"git.root":"."]
         globs = [
             abcs.Path(project_root).joinpath(f"**/{use_glob}"),
         ]
@@ -82,14 +84,38 @@
         else:
             self.logger.critical(f"packing  {len(goals)} goals")
             for g in goals:
                 plan.append(g)
         app.status_bar.update(app="Pynchon", stage=f"{len(plan)}")
         return plan
 
+    def _dispatch_apply_hooks(self, results: planning.ApplyResults):
+        """ """
+        # write status event (used by the app-console)
+        app.status_bar.update(
+            app="Pynchon::HOOKS",
+            stage=f"{self.__class__.name}",
+        )
+        if results.finished:
+            hooks = self.apply_hooks
+            if hooks:
+                LOGGER.warning(
+                    f"{self.name}.apply: dispatching {len(hooks)} hooks: {hooks}"
+                )
+                hook_results = []
+                for hook in hooks:
+                    hook_results.append(self.run_hook(hook, results))
+            else:
+                LOGGER.warning(f"{self.name}.apply: no hooks to run.")
+        else:
+            LOGGER.critical(f"{self.name}: Skipping hooks: ")
+            LOGGER.critical(
+                f"  {len(results.goals)-len(results.actions)} goals incomplete"
+            )
+
     @cli.options.quiet
     @cli.options.parallelism
     @cli.options.fail_fast
     def apply(
         self,
         plan: planning.Plan = None,
         parallelism: str = "0",
@@ -113,38 +139,14 @@
         LOGGER.critical(
             f"{self.name}.apply finished ( {len(results.actions)}/{len(results.goals)} goals )"
         )
         self._dispatch_apply_hooks(results)
         if not quiet:
             return results
 
-    def _dispatch_apply_hooks(self, results: planning.ApplyResults):
-        """ """
-        # write status event (used by the app-console)
-        app.status_bar.update(
-            app="Pynchon::HOOKS",
-            stage=f"{self.__class__.name}",
-        )
-        if results.finished:
-            hooks = self.apply_hooks
-            if hooks:
-                LOGGER.warning(
-                    f"{self.name}.apply: dispatching {len(hooks)} hooks: {hooks}"
-                )
-                hook_results = []
-                for hook in hooks:
-                    hook_results.append(self.run_hook(hook, results))
-            else:
-                LOGGER.warning(f"{self.name}.apply: no hooks to run.")
-        else:
-            LOGGER.critical(f"{self.name}: Skipping hooks: ")
-            LOGGER.critical(
-                f"  {len(results.goals)-len(results.actions)} goals incomplete"
-            )
-
     def _validate_hooks(self, hooks):
         # FIXME: validation elsewhere
         for x in hooks:
             assert isinstance(x, (str,))
             assert " " not in x
             assert "_" not in x
             assert x.strip()
@@ -215,15 +217,16 @@
     """
 
     contribute_plan_apply = False
 
 
 @tags(cli_label="Manager")
 class Manager(ShyPlanner):
-    cli_label = "Manager"
+    cli_label = "Project Tools"
+    cli_description = "Tools for project management"
 
 
 class ResourceManager(Manager):
     @property
     def changes(self):
         """Set(git_changes).intersection(plugin_resources)"""
         git = self.siblings["git"]
@@ -268,7 +271,13 @@
 
 class Planner(ShyPlanner):
     """Planner uses plan/apply workflows, and contributes it's plans
     to ProjectPlugin (or any other parent plugins).
     """
 
     contribute_plan_apply = True
+    cli_description = ""
+
+
+class RenderingPlugin(Planner):
+    cli_label = "Rendering Tools"
+    cli_description = ""
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/models/planning.py` & `pynchon-2024.4.5.14.1/src/pynchon/models/planning.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -215,14 +215,59 @@
             ),
             subtitle=app.Text(f"{self.label or self.owner}", style="dim"),
             # + app.Text(" rsrc=", style="bold italic")
             # + app.Text(f"{self.rel_resource}", style="dim italic"),
         )
 
 
+class ApplyResults(typing.BaseModel):
+    # typing.List[Action], metaclass=meta.namespace):
+    """ """
+    goals: typing.List[Goal] = typing.Field(default=[])
+    actions: typing.List[Action] = typing.Field(default=[])
+
+    @property
+    def finished(self):
+        """ """
+        return len(self.goals) == len(self.actions)
+
+    @property
+    def ok(self) -> bool:
+        return self.finished and all([a.ok for a in self])
+
+    @property
+    def action_types(self):
+        tmp = list({g.type for g in self})
+        return {k: [] for k in tmp}
+
+    @property
+    def _dict(self):
+        """ """
+        result = collections.OrderedDict()
+        result["ok"] = self.ok
+        result["resources"] = list({a.resource for a in self})
+        result["actions"] = [
+            g.command if g.command else self.callable.__name__ for g in self
+        ]
+        result["action_types"] = self.action_types
+        result["changed"] = list({a.resource for a in self if a.changed})
+        for g in self:
+            result["action_types"][g.type].append(g.resource)
+        return result
+
+    def __iter__(self):
+        return iter(self.actions)
+
+    def __len__(self):
+        return len(self.actions)
+
+    def __str__(self):
+        return f"<{self.__class__.__name__}[{len(self)} actions]>"
+
+
 class Plan(typing.BaseModel):
     """ """
 
     goals: typing.List[Goal] = typing.Field(default=[])
     owner: typing.StringMaybe = typing.Field(
         help="Name of the plugin that owns this Plan", default=None
     )
@@ -371,52 +416,7 @@
             ),
         ):
             return Plan(goals=self.goals + list(other))
         else:
             raise NotImplementedError(type(other))
 
     __iadd__ = __add__
-
-
-class ApplyResults(typing.BaseModel):
-    # typing.List[Action], metaclass=meta.namespace):
-    """ """
-    goals: typing.List[Goal] = typing.Field(default=[])
-    actions: typing.List[Action] = typing.Field(default=[])
-
-    @property
-    def finished(self):
-        """ """
-        return len(self.goals) == len(self.actions)
-
-    def __len__(self):
-        return len(self.actions)
-
-    def __iter__(self):
-        return iter(self.actions)
-
-    @property
-    def ok(self) -> bool:
-        return self.finished and all([a.ok for a in self])
-
-    @property
-    def action_types(self):
-        tmp = list({g.type for g in self})
-        return {k: [] for k in tmp}
-
-    @property
-    def _dict(self):
-        """ """
-        result = collections.OrderedDict()
-        result["ok"] = self.ok
-        result["resources"] = list({a.resource for a in self})
-        result["actions"] = [
-            g.command if g.command else self.callable.__name__ for g in self
-        ]
-        result["action_types"] = self.action_types
-        result["changed"] = list({a.resource for a in self if a.changed})
-        for g in self:
-            result["action_types"][g.type].append(g.resource)
-        return result
-
-    def __str__(self):
-        return f"<{self.__class__.__name__}[{len(self)} actions]>"
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/models/plugins/__init__.py` & `pynchon-2024.4.5.14.1/src/pynchon/models/plugins/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 from fleks import tagging
 
 from pynchon import abcs, api, cli, events  # noqa
 from pynchon.util import lme, typing  # noqa
 
 from . import validators  # noqa
 from .cli import CliPlugin  # noqa
-from .docker import DockerWrapper  # noqa
+from .docker import DiagramTool, DockerWrapper  # noqa
 from .provider import Provider  # noqa
 from .pynchon import PynchonPlugin  # noqa
-from .tool import ToolPlugin  # noqa
+from .tool import AutomationTool, ToolPlugin  # noqa
 
 LOGGER = lme.get_logger(__name__)
 classproperty = fleks.util.typing.classproperty
 
 
 class BasePlugin(CliPlugin):
     """The default plugin-type most new plugins will use"""
@@ -39,18 +39,15 @@
 
         globals = plugin_util.get_plugin("globals").get_current_config()
         global_ex = globals["exclude_patterns"]
         my_ex = self.get("exclude_patterns", [])
         return list(set(global_ex + my_ex + ["**/pynchon/templates/includes/**"]))
 
 
-@tagging.tags(cli_label="NameSpace")
+@tagging.tags(cli_label="NameSpaces")
 class NameSpace(CliPlugin):
-    """`CliNamespace` collects functionality
-    from elsewhere under a single namespace
-
-
-    """
+    """Collects functionality from other plugins under a single namespace"""
 
     cli_label = "NameSpace"
     contribute_plan_apply = False
+    cli_description = __doc__
     priority = 1
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/models/plugins/cli.py` & `pynchon-2024.4.5.14.1/src/pynchon/models/plugins/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,16 @@
         kls._finalized_click_groups[kls] = plugin_main
 
         tags = tagging.tags.get(kls) or {}
         gr_aliases = list(set(tags.get("click_aliases", [])))
         for alias in gr_aliases:
             g2 = cli.click.group_copy(plugin_main, name=alias, hidden=True)
             kls.click_entry.add_command(g2)
-
+        # WARNING: bad coupling.  this important backlink is expected by fleks
+        plugin_main.plugin_class = kls
         return plugin_main
 
     @classproperty
     @functools.lru_cache(maxsize=None)
     def click_commands(kls) -> typing.List[str]:
         return [
             name
@@ -188,15 +189,15 @@
                 update_kwargs.update(
                     name=name,
                 )
                 update_kwargs.update(via=kls)
                 kls = kls.siblings[click_parent_plugin]
                 normalized_subcommand_name = fxn.__name__.replace("_", "-")
                 update_kwargs.update(
-                    help=f"(alias for `{okls.click_entry.name} {okls.cli_name} {normalized_subcommand_name}`)"
+                    help=f"(Alias for `{okls.click_entry.name} {okls.cli_name} {normalized_subcommand_name}`)"
                 )
             tmp = kls.click_create_cmd(
                 fxn,
                 wrapper=wrapper,
                 **{
                     **update_kwargs,
                     **dict(hidden=hidden, alias=alias),
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/models/plugins/docker.py` & `pynchon-2024.4.5.14.1/src/pynchon/models/plugins/docker.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,38 +9,57 @@
 from pynchon.util import lme, typing  # noqa
 
 from . import validators  # noqa
 
 LOGGER = lme.get_logger("DOCKER")
 
 
-# @tagging.tags(cli_label="Docker-Wrapper")
 class DockerWrapper(ToolPlugin):
     """
-    General wrapper for a dockerized tool.
+    Wrappers for dockerized tools
     """
 
     class BaseConfig(abcs.Config):
         docker_image: str = typing.Field(default="docker/hello-world")
         docker_args: typing.List = typing.Field(default=[])
 
-    cli_label = "DockerWrapper"
+    cli_label = "Docker Wrappers"
+    cli_description = "Plugins that wrap invocations on containers"
     contribute_plan_apply = False
     priority = 2
     __class_validators__ = [
         validators.require_conf_key,
     ]
 
     @property
     def command_extra(self):
         import sys
 
         command = sys.argv[sys.argv.index(self.click_group.name) + 2 :]
         return " ".join(command)
 
+    def _get_docker_command_base(self, *args, **kwargs):
+        docker_image = kwargs.pop("docker_image", self["docker_image"])
+        docker_args = kwargs.pop("docker_args", "")
+        docker_args = (
+            docker_args + " " + " ".join(f'--{k}="{v}"' for k, v in kwargs.items())
+        )
+        return (
+            "docker run -v `pwd`:/workspace -w /workspace "
+            f"{docker_args} {docker_image} {' '.join(args)}"
+        )
+
+    def _get_docker_command(self, *args, **kwargs):
+        """ """
+        cmd_t = self._get_docker_command_base(" ".join(args))
+        docker_args = " ".join(self["docker_args"])
+        zip_kws = " ".join(["{k}={v}" for k, v in kwargs.items()])
+        cmd_t += f" {docker_args} {zip_kws}"
+        return cmd_t
+
     @click.command(
         context_settings=dict(
             ignore_unknown_options=True,
             allow_extra_args=True,
         )
     )
     def run(self, *args, **kwargs):
@@ -68,25 +87,11 @@
         from pynchon.util.os import invoke
 
         LOGGER.critical(cmd)
         result = invoke(cmd, **kwargs)
         LOGGER.warning(result.stdout)
         return result
 
-    def _get_docker_command_base(self, *args, **kwargs):
-        docker_image = kwargs.pop("docker_image", self["docker_image"])
-        docker_args = kwargs.pop("docker_args", "")
-        docker_args = (
-            docker_args + " " + " ".join(f'--{k}="{v}"' for k, v in kwargs.items())
-        )
-        return (
-            "docker run -v `pwd`:/workspace -w /workspace "
-            f"{docker_args} {docker_image} {' '.join(args)}"
-        )
 
-    def _get_docker_command(self, *args, **kwargs):
-        """ """
-        cmd_t = self._get_docker_command_base(" ".join(args))
-        docker_args = " ".join(self["docker_args"])
-        zip_kws = " ".join(["{k}={v}" for k, v in kwargs.items()])
-        cmd_t += f" {docker_args} {zip_kws}"
-        return cmd_t
+class DiagramTool(DockerWrapper):
+    cli_label = "Diagramming Tools"
+    cli_description = "View and render technical diagrams from source, in several formats.  (Usually these require docker, but no other system dependencies.)"
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/models/plugins/provider.py` & `pynchon-2024.4.5.14.1/src/pynchon/models/plugins/provider.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,20 +10,18 @@
 from .cli import CliPlugin  # noqa
 
 LOGGER = lme.get_logger(__name__)
 
 
 @tagging.tags(cli_label="Provider")
 class Provider(CliPlugin):
-    """ProviderPlugin provides context-information,
-    but little other functionality
-
-
-    """
+    """A wrapper for context that other plugins can use"""
 
     cli_label = "Provider"
+    cli_description = __doc__
+
     contribute_plan_apply = False
     priority = 2
     __class_validators__ = [
         validators.require_conf_key,
         # validators.warn_config_kls,
     ]
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/models/plugins/pynchon.py` & `pynchon-2024.4.5.14.1/src/pynchon/models/plugins/pynchon.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 
 @tagging.tags(cli_label="<<Abstract>>")
 class PynchonPlugin(fleks.Plugin):
     """Pynchon-specific plugin-functionality"""
 
     name = "<<Abstract>>"
     cli_label = "<<Abstract>>"
+    cli_description = __doc__
+
     config_class = None
     __class_validators__ = [
         validators.require_conf_key,
         validators.warn_config_kls,
     ]
 
     @classproperty
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/models/plugins/validators.py` & `pynchon-2024.4.5.14.1/src/pynchon/models/plugins/validators.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/models/python.py` & `pynchon-2024.4.5.14.1/src/pynchon/models/python.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,38 +6,40 @@
 from pynchon import abcs
 from pynchon.util import lme, typing
 
 LOGGER = lme.get_logger(__name__)
 
 
 class EntrypointMetadata(BaseModel):
-    is_click: bool = typing.Field(help="", required=False, default=False)
-    is_package_entrypoint: bool = typing.Field(help="", required=False, default=False)
-    is_module: bool = typing.Field(help="", required=False, default=True)
+    is_click: bool = typing.Field(description="", required=False, default=False)
+    is_package_entrypoint: bool = typing.Field(
+        description="", required=False, default=False
+    )
+    is_module: bool = typing.Field(description="", required=False, default=True)
     bin_name: typing.StringMaybe = typing.Field(
-        help="Name for this console script. (Nil if module-entrypoint)",
+        description="Name for this console script. (Nil if module-entrypoint)",
         required=False,
         default=None,
     )
     help_command: typing.StringMaybe = typing.Field(
-        help="Command that returns help for this entrypoint",
+        description="Command that returns help for this entrypoint",
         required=False,
         default=None,
     )
     dotpath: str = typing.Field(
-        help="",
+        description="",
         required=True,
     )
     file: str = typing.Field(
-        help="",
+        description="",
         required=True,
     )
-    resource: abcs.Path = typing.Field(help="", required=True)
-    path: abcs.Path = typing.Field(help="", required=True)
-    entrypoints: typing.List = typing.Field(help="", required=False, default=[])
+    resource: abcs.Path = typing.Field(description="", required=True)
+    path: abcs.Path = typing.Field(description="", required=True)
+    entrypoints: typing.List = typing.Field(description="", required=False, default=[])
     src_root: abcs.Path = typing.Field(required=True)
     inside_src_root: bool = typing.Field(default=True)
 
     @property
     def src_url(self) -> str:
         if not self.inside_src_root:
             return ""
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/__init__.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 """
 
 import collections
 
 import fleks
 import shimport
 
-from pynchon import config, events  # noqa
+from pynchon import config, constants, events  # noqa
 from pynchon.util import lme, typing  # noqa
 
 from .util import get_plugin, get_plugin_obj  # noqa
 
 LOGGER = lme.get_logger(__name__)
 mod_wrap = shimport.wrap(__name__, import_children="**/*.py")
 registry = {
     **mod_wrap.prune(
         exclude_names="git".split(),  # FIXME: hack
         types_in=[fleks.Plugin],
         filter_vals=[
-            lambda val: val.name in config.PLUGINS,
+            lambda val: val.name in config.PLUGINS + constants.PLUGINS,
         ],
     ).namespace
 }
 registry = registry.items()
 registry = collections.OrderedDict(sorted(registry, key=lambda x: x[1].priority))
 registry = collections.OrderedDict(
     [
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/cicd.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/cicd.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/core.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,27 +41,14 @@
         return result
 
     def cfg(self):
         """Show current project config (with templating/interpolation)"""
         tmp = self.project_config
         return tmp
 
-    def init(self, strict=True):
-        """Write .pynchon.json5 if it's not present"""
-        default_config = abcs.Path(".") / ".pynchon.json5"
-        if default_config.exists():
-            LOGGER.critical(f"{default_config} exists, nothing to do.")
-            err = f"Refusing to create {default_config} (file already exists)"
-            LOGGER.critical(err)
-            if strict:
-                raise SystemExit(1)
-        else:
-            self._init_config(default_config)
-            return True
-
     def _init_config(self, config_path):
         """ """
         cfg = self.cfg().dict()
         pop_list = ["apply_hooks"]
         for plugin_name in cfg:
             try:
                 sib = self.siblings[plugin_name]
@@ -73,30 +60,45 @@
         for p in pop_list:
             cfg.pop(p)
         LOGGER.critical(f"Writing {config_path.absolute()}")
         from pynchon.util.text import dumpf
 
         dumpf.json(cfg, file=config_path)
 
-    @cli.click.flag("--bash", help="bootstrap bash")
+    def init(self, strict=True):
+        """Write .pynchon.json5 if it's not present"""
+        default_config = abcs.Path(".") / ".pynchon.json5"
+        if default_config.exists():
+            LOGGER.critical(f"{default_config} exists, nothing to do.")
+            err = f"Refusing to create {default_config} (file already exists)"
+            LOGGER.critical(err)
+            if strict:
+                raise SystemExit(1)
+        else:
+            self._init_config(default_config)
+            return True
+
+    # @cli.click.flag("--bash", help="bootstrap bash")
     @cli.click.flag("--bashrc", help="bootstrap bashrc")
-    @cli.click.flag("--bash-completions", help="bootstrap completions")
+    # @cli.click.flag("--bash-completions", help="bootstrap completions")
     @cli.click.flag("--pynchon", help="bootstrap .pynchon.json5")
-    @cli.click.flag("--makefile", help="bootstrap Makefile")
-    @cli.click.flag("--tox", help="bootstrap tox")
+    # @cli.click.flag("--makefile", help="bootstrap Makefile")
+    # @cli.click.flag("--tox", help="bootstrap tox")
     def bootstrap(
         self,
         pynchon: bool = False,
+        bashrc: bool = False,  # noqa
         bash: bool = False,
         bash_completions: bool = False,
-        bashrc: bool = False,  # noqa
         makefile: bool = False,
         tox: bool = False,
     ) -> None:
-        """Bootstrap for shell integration, etc"""
+        """
+        Helpers for bootstraping various project boilerplate.
+        """
         template_prefix = f"{self.plugin_templates_prefix}/bootstrap"
         pynchon_completions_script = ".tmp.pynchon.completions.sh"
         bashrc_snippet = ".tmp.pynchon.bashrc"
         if bash_completions:
             pass
 
             gr = self.__class__.click_entry
@@ -188,15 +190,15 @@
     @cli.options.quiet
     def plan(
         self,
         config=None,
         quiet: bool = False,
         flattened: bool = True,
     ) -> models.Plan:
-        """Runs plan for all plugins"""
+        """Runs planning for all plugins"""
 
         config = config or self.project_config
         plan = super(self.__class__, self).plan(config)
         plans = [] if not flattened else None
         plugins = self.sorted_plugins
         self.logger.critical(f"Planning on behalf of: {[p.name for p in plugins]}")
         for plugin_obj in plugins:
@@ -222,15 +224,15 @@
         self,
         plan: planning.Plan = None,
         parallelism: str = "1",
         quiet: bool = False,
         fail_fast: bool = False,
     ) -> planning.ApplyResults:
         """
-        Executes the plan for this plugin
+        Executes the plan for all plugins
         """
         parallelism = int(parallelism)
         plans = plan or self.plan(flattened=False)
         for plan in plans:
             results = plan.apply(parallelism=parallelism, git=self.siblings["git"])
             LOGGER.critical(
                 f"Finished apply for subplan ({len(results.actions)}/{len(results.goals)} goals)"
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/deck.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/deck.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,29 +3,28 @@
 
 from pynchon import abcs, cli, events, models  # noqa
 from pynchon.util import lme, typing  # noqa
 
 LOGGER = lme.get_logger(__name__)
 
 
-class Deck(models.ResourceManager):
+class Deck(models.DiagramTool):
     """Tool for working with markdown based slide-decks"""
 
     class config_class(abcs.Config):
         config_key: typing.ClassVar[str] = "deck"
         root: str = typing.Field(default="{{docs.root}}/slides")
         pandoc_docker: str = typing.Field(default="pandoc/core")
         pandoc_engine: str = typing.Field(default="dzslides")
         pandoc_args: typing.List[str] = typing.Field(default=[])
         apply_hooks: typing.List[str] = typing.Field(default=["open-after"])
         include_patterns: typing.List[str] = typing.Field(default=["*.md"])
 
     name = "deck"
     cli_name = "deck"
-    cli_label = "Tool"
     contribute_plan_apply = True
 
     def plan(self, **kwargs):
         plan = super().plan()
         root = self["root"]
         root = abcs.Path(root)
         if not root.exists():
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/dockerhub.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/dockerhub.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-""" pynchon.plugins.mermaid
+""" pynchon.plugins.dockerhub
 """
 
+import webbrowser
+
 from fleks import cli, tagging  # noqa
 
 from pynchon import abcs, events, models  # noqa
 from pynchon.util import files, lme, typing  # noqa
 
 LOGGER = lme.get_logger(__name__)
 
 
-class Dockerhub(models.Planner):
-    """Dockerhub Plugin"""
+class Dockerhub(models.Provider):
+    """Context for Dockerhub"""
 
     class config_class(abcs.Config):
         config_key: typing.ClassVar[str] = "dockerhub"
         org_name: typing.StringMaybe = typing.Field(default=None, help="")
         repo_name: typing.StringMaybe = typing.Field(default=None, help="")
 
         @property
@@ -27,12 +29,10 @@
                 self.repo_name and self.org_url and f"{self.org_url}/{self.repo_name}"
             )
 
     name = "dockerhub"
     cli_name = "dockerhub"
 
     def open(self):
-        import webbrowser
-
+        """Open this dockerhub project's webpage"""
         url = self.config.repo_url or self.config.org_url
-        # assert url,err
         webbrowser.open(url)
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/docs/main.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/docs/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         config_key: typing.ClassVar[str] = "docs"
         include_patterns: typing.List[str] = typing.Field(default=[])
         root: typing.Union[str, abcs.Path, None] = typing.Field()
         exclude_patterns: typing.List[str] = typing.Field(default=[])
 
     name = "docs"
     cli_name = "docs"
-    cli_label = "Manager"
+    cli_label = "Docs Tools"
     priority = 0
     serving = None
 
     # @property
     # def root(self):
     #     if "root" not in self.__dict__:
     #         from pynchon.config import GIT, pynchon
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/docs/opener.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/docs/opener.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/dot.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/dot.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from pynchon import abcs, api, models  # noqa
 from pynchon.util import files, lme, typing  # noqa
 
 LOGGER = lme.get_logger(__name__)
 
 
-class Dot(models.Planner):
+class Dot(models.DiagramTool, models.Planner):
     """Finds / Renders (graphviz) dot files for this project"""
 
     class config_class(abcs.Config):
         config_key: typing.ClassVar[str] = "dot"
         exclude_patterns: typing.List[str] = typing.Field(default=[])
 
     name = "dot"
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/drawio.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/drawio.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 """ pynchon.plugins.drawio
 
-    https://hub.docker.com/r/jgraph/drawio
-    https://www.drawio.com/blog/diagrams-docker-app
+    A Wrapper for docker-containers that
+    provide the "drawio" diagramming utility
+
+    Live Cloud Version:
+        https://app.diagrams.net/
+    Local Server:
+        https://hub.docker.com/r/jgraph/drawio
+        https://www.drawio.com/blog/diagrams-docker-app
+    CLI Tools:
+        https://github.com/rlespinasse/docker-drawio-desktop-headless
 """
 
 import webbrowser
 
 from fleks import tagging
 
 from pynchon import abcs, api, cli, events, models  # noqa
@@ -14,20 +22,27 @@
 LOGGER = lme.get_logger(__name__)
 
 ElementList = typing.List[typing.Dict]
 DEFAULT_HTTP_PORT = 8080
 DEFAULT_DOCKER_NAME = "drawio-server"
 
 
-@tagging.tags(click_aliases=["drawio", "draw"])
-class DrawIO(models.DockerWrapper, models.Planner):
-    """Helpers for initializing pynchon"""
+@tagging.tags(click_aliases=["draw"])
+class DrawIO(models.DiagramTool, models.Planner):
+    """
+    Wrapper for docker-containers that
+    provide the "drawio" diagramming utility
+    """
 
     class config_class(abcs.Config):
         config_key: typing.ClassVar[str] = "drawio"
+        file_glob: str = typing.Field(
+            default="*.drawio", description="Where to find jinja templates"
+        )
+
         docker_image: str = typing.Field(
             default="jgraph/drawio", help="Docker image to use"
         )
         http_port: str = typing.Field(help="Port to use", default=DEFAULT_HTTP_PORT)
         docker_args: typing.List = typing.Field(
             default=[f"-it --rm --name={DEFAULT_DOCKER_NAME}"],
             help="Docker args to use",
@@ -43,30 +58,30 @@
                 "--embed-svg-images",
                 "--embed-diagram",
                 "--svg-theme light",
             ],
         )
 
     name = "drawio"
-    cli_name = "draw"
+    cli_name = "drawio"
     priority = 0
-    file_glob = "*.drawio"
 
     @tagging.tags(click_aliases=["ls"])
     def list(self, changes=False, **kwargs):
         """
-        Lists affected resources for this project
+        Lists affected resources (*.drawio files) for this project
         """
         return self._list(changes=changes, **kwargs)
 
     @cli.click.argument("output", required=False)
     @cli.click.argument("input")
     def export(self, input, output=None, format="svg"):
         """
-        Export the given .drawio file (default format is SVG)
+        Exports a given .drawio file to some
+        output file/format (default format is SVG)
         """
         assert input.endswith(".drawio") or input.endswith(
             ".xml"
         ), "Expected an xml or drawio file as input"
         output = output or ".".join(
             list(filter(None, input.split(".")[:-1])) + [format]
         )
@@ -80,19 +95,23 @@
             ),
             strict=True,
         )
         print(result.stdout if result.succeeded else result)
         raise SystemExit(0 if result.succeeded else 1)
 
     def serve(self):
-        """Runs drawio-UI in a docker-container"""
+        """
+        Runs the drawio-UI in a docker-container
+        """
         port = self.config.http_port
         dargs = self.config.docker_args
         dimg = self.config.docker_image
         cmd_t = f"docker run {dargs} -p {port}:{port} {dimg}"
         return self._run_docker(cmd_t, strict=True, interactive=True)
 
     def open(self, *args, **kwargs):
-        """Opens browser for docker-container"""
+        """
+        Opens a browser for the container started by `serve`
+        """
         return webbrowser.open(
             f"http://localhost:{self.config.http_port}/?offline=1&https=0"
         )
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/fixme.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/fixme.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ pynchon.plugins.fixme
 """
 
 from fnmatch import fnmatch
 
-from pynchon import abcs, constants, models
+from pynchon import abcs, models
 from pynchon.util import lme, typing
 from pynchon.util.os import invoke
 
 from fleks.cli import click, options  # noqa
 
 
 LOGGER = lme.get_logger(__name__)
@@ -28,14 +28,15 @@
 
 
 class FixMe(models.Planner):
     """Generates {docs_root}/FIXME.md from source"""
 
     name = "fixme"
     config_class = FixMeConfig
+    cli_label = "Docs Tools"
 
     def plan(self, config: dict = None) -> typing.List:
         """ """
         config = config or self.__class__.get_current_config()
         plan = super(self.__class__, self).plan(config)
         target = abcs.Path(self.project_config["docs"]["root"]) / "FIXME.md"
         plan.append(
@@ -54,23 +55,19 @@
         help=("output file to write.  (optional)"),
     )
     @options.should_print
     @options.header
     def gen(
         self,
         output,
-        should_print,
+        should_print: bool,
         header,
     ):
-        """Generate FIXME.md files, aggregating references to all FIXME's in code-base
-
-        :param output: param should_print:
-        :param header:
-        :param should_print:
-
+        """
+        Generate FIXME.md files, aggregating references to all FIXME's in code-base
         """
         from pynchon import api
 
         config = self.__class__.project_config
         src_root = config.src["root"]
         exclude_patterns = self["exclude_patterns"]
         cmd = invoke(f"grep --line-number -R FIXME {src_root}")
@@ -106,18 +103,16 @@
             "pynchon/plugins/fixme/FIXME.md.j2",
         ).render(**dict(items=items))
         msg = result
         print(msg, file=open(output, "w"))
         if should_print and output != "/dev/stdout":
             print(msg)
 
-    @classmethod
-    def asdasdinit_cli(kls):
-        """
-
-        :param kls:
-
-        """
-        parent = kls.click_group
-        T_FIXME = constants.ENV.get_template(
-            "pynchon/plugins/plugins/fixme/FIXME.md.j2"
-        )
+    #
+    # @classmethod
+    # def asdasdinit_cli(kls):
+    #     """
+    #     """
+    #     parent = kls.click_group
+    #     T_FIXME = constants.ENV.get_template(
+    #         "pynchon/plugins/plugins/fixme/FIXME.md.j2"
+    #     )
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/gen.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/gen.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/git.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/git.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,23 +8,16 @@
 
 LOGGER = lme.get_logger(__name__)
 
 
 class GitConfig(abcs.Config):
     """ """
 
-    # _root: str = None
     config_key: typing.ClassVar[str] = "git"
 
-    # class Config:
-    #     fields = {
-    #         # '_root': 'root',
-    #         '_repo': 'repo',
-    #     }
-
     def _run(self, cmd, log_command=False, **kwargs):
         """
         :param cmd: param log_command:  (Default value = False)
         :param log_command:  (Default value = False)
         :param **kwargs:
         """
         if self.root:
@@ -37,78 +30,78 @@
     #     """ """
     #     tmp = self._run("git remote show origin " "| sed -n '/HEAD branch/s/.*: //p'")
     #     if tmp and tmp.succeeded:
     #         return tmp.stdout.strip() or None
 
     @property
     def root(self) -> typing.StringMaybe:
-        """ """
+        """Root path for this git project"""
         tmp = self.__dict__.get("_root")
         if tmp:
             return tmp
         tmp = files.get_git_root(abcs.Path("."))
         return tmp and tmp.parents[0]
 
     @property
     def repo(self) -> typing.StringMaybe:
-        """ """
+        """Repo name for this git project"""
         if "repo" not in self.__dict__:
             cmd = self._run("git config --get remote.origin.url")
             self.__dict__.update(
                 repo=cmd and (cmd.stdout.strip() if cmd.succeeded else None)
             )
         return self.__dict__["repo"]
 
     @property
-    def is_github(self):
-        """ """
+    def is_github(self) -> typing.Bool:
+        """True if this is a github repository"""
         tmp = "git@github https://github.com http://github.com".split()
         return self.repo and any([self.repo.startswith(x) for x in tmp])
 
     @property
     def github_org(self) -> typing.StringMaybe:
-        """ """
+        """Name of this github organization"""
         if self.is_github:
             tmp = self.repo.split(":")[-1]
             try:
                 org, _repo_name = tmp.split("/")
             except (ValueError,):
                 return None
             return org
 
     @property
     def repo_name(self) -> typing.StringMaybe:
-        """ """
+        """Repository name"""
         if self.repo:
             tmp = self.repo.split(":")[-1]
             try:
                 _org, repo_name = tmp.split("/")
             except (ValueError,):
                 return None
             repo_name = repo_name.split(".git")[0]
             return repo_name
 
     @property
-    def repo_url(self):
-        """ """
+    def repo_url(self) -> typing.StringMaybe:
+        """Repository URL"""
         if all([self.github_org, self.repo_name]):
             return f"https://github.com/{self.github_org}/{self.repo_name}"
 
     @property
-    def branch_name(self):
-        """ """
+    def branch_name(self) -> typing.StringMaybe:
+        """Name of current branch"""
         if "branch_name" not in self.__dict__:
             cmd = self._run("git rev-parse --abbrev-ref HEAD")
             tmp = cmd and cmd.succeeded and cmd.stdout.strip()
             self.__dict__.update(branch_name=tmp or None)
         return self.__dict__["branch_name"]
 
     @property
-    def hash(self) -> str:
-        """ """
+    def hash(self) -> typing.StringMaybe:
+        """Current git hash"""
         if "hash" not in self.__dict__:
             cmd = self._run("git rev-parse HEAD")
             tmp = cmd and cmd.succeeded and cmd.stdout.strip()
             self.__dict__.update(hash=tmp or None)
         return self.__dict__["hash"]
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/github.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/github.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,28 +19,31 @@
 @tagging.tags(click_aliases=["gh"])
 class GitHub(models.ToolPlugin):
     """Tools for working with GitHub"""
 
     class config_class(abcs.Config):
         config_key: typing.ClassVar[str] = "github"
         enterprise: bool = typing.Field(default=False)
-        org_name: str = typing.Field(default=None)
-        org_url: str = typing.Field(default=None)
-        repo_url: str = typing.Field(default=None)
+        org_name: typing.StringMaybe = typing.Field(default=None)
+        org_url: typing.StringMaybe = typing.Field(default=None)
+        repo_url: typing.StringMaybe = typing.Field(default=None)
         actions: typing.List[abcs.Path] = typing.Field(default=[None])
-        raw_url: str = typing.Field(default=None)
-        repo_ssh_url: str = typing.Field(default=None)
+        raw_url: typing.StringMaybe = typing.Field(default=None)
+        repo_ssh_url: typing.StringMaybe = typing.Field(default=None)
 
         @property
         def raw_url(self):
-            return f"https://raw.githubusercontent.com/{self.org_name}/{config.git.repo_name}"
+            """URL for serving raw content"""
+            repo_name = config.git.repo_name
+            if self.org_name and config.git.repo_name:
+                return f"https://raw.githubusercontent.com/{self.org_name}/{repo_name}"
 
         @property
         def actions(self) -> typing.List[typing.Dict]:
-            """ """
+            """Github Action information"""
             groot = config.git.root
             if groot:
                 wflows = abcs.Path(groot) / ".github" / "workflows"
                 if wflows.exists():
                     return [
                         dict(
                             name=fname,
@@ -48,34 +51,40 @@
                             url=f"{self.repo_url}/actions/workflows/{fname}",
                         )
                         for fname in wflows.list()
                     ]
             return []
 
         @property
-        def repo_url(self):
+        def repo_url(self) -> typing.StringMaybe:
+            """Repository URL"""
             return config.git.repo_url
 
         @property
-        def repo_ssh_url(self):
-            if self.repo_url:
+        def repo_ssh_url(self) -> typing.StringMaybe:
+            """Repository SSH URL"""
+            if self.org_name and self.repo_url:
                 return (
                     f"git@github.com:{self.org_name}/{self.repo_url.split('/')[-1]}.git"
                 )
 
         @property
-        def org_url(self):
-            return f"https://github.com/{self.org_name}"
+        def org_url(self) -> typing.StringMaybe:
+            """Org URL"""
+            if self.org_name:
+                return f"https://github.com/{self.org_name}"
 
         @property
-        def org_name(self):
+        def org_name(self) -> typing.StringMaybe:
+            """Org name"""
             return config.git.github_org
 
     name = "github"
     cli_name = "github"
+    cli_label = "Provider"
     cli_aliases = []
 
     @cli.click.option("--org", "-o")
     def open(self, org=None):
         """Opens org/repo github in a webbrowser
 
         :param org: Default value = None)
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/griffe.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/griffe.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 from fleks import tagging
 
 from pynchon import abcs, cli, events, models  # noqa
 from pynchon.util import lme, os, typing  # noqa
 
 LOGGER = lme.get_logger(__name__)
 
+from pynchon.plugins.python.common import PythonPlanner
+
 
 @tagging.tags(click_aliases=["g", "gr"])
-class Griffe(models.ToolPlugin):
+class Griffe(PythonPlanner):
     """Tools for working with Python ASTs"""
 
     class config_class(abcs.Config):
         config_key: typing.ClassVar[str] = "griffe"
 
     name = "griffe"
     cli_name = "griffe"
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/jinja.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/jinja.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,47 @@
 """ pynchon.plugins.jinja
 """
 
 from fleks import tagging
 
-from pynchon import abcs, api, cli, models
+from pynchon import abcs, api, cli
 
 from pynchon.util import files, lme, text, typing  # noqa
 
 LOGGER = lme.get_logger(__name__)
 
+from pynchon.models.planner import RenderingPlugin  # noqa
+
 
 @tagging.tags(click_aliases=["j"])
-class Jinja(models.Planner):
+class Jinja(RenderingPlugin):
     """Renders files with {jinja.template_includes}"""
 
-    file_glob = "*.j2"
     # diff --color --minimal -w --side-by-side /etc/bash.bashrc <(bash --pretty-print /etc/bash.bashrc )
 
     class config_class(abcs.Config):
         config_key: typing.ClassVar[str] = "jinja"
-        template_includes: typing.List[str] = typing.Field(default=[])
-        exclude_patterns: typing.List[str] = typing.Field()
-        vars: typing.Dict[str, str] = typing.Field(default={}, help="")
+        file_glob: str = typing.Field(
+            default="*.j2", description="Where to find jinja templates"
+        )
+        template_includes: typing.List[str] = typing.Field(
+            default=[],
+            description="Where to find files for use with Jinja's `include` blocks",
+        )
+        exclude_patterns: typing.List[str] = typing.Field(
+            description="File patterns to exclude from resource-listing"
+        )
+        vars: typing.Dict[str, str] = typing.Field(
+            default={}, description="Extra variables for template rendering"
+        )
 
         # @tagging.tagged_property(conflict_strategy="override")
         @property
         def exclude_patterns(self):
+            "File patterns to exclude from resource-listing"
             from pynchon.config import globals
 
             # globals = plugin_util.get_plugin("globals").get_current_config()
             global_ex = globals.exclude_patterns
             my_ex = self.__dict__.get("exclude_patterns", [])
             return list(set(global_ex + my_ex + ["**/pynchon/templates/includes/**"]))
 
@@ -61,15 +73,15 @@
         self,
         local: bool = False,
     ):
         """Lists full path of each include-file"""
         includes = self._include_folders
         if local:
             includes.remove(api.render.PYNCHON_CORE_INCLUDES)
-        includes = [abcs.Path(t) / "**/*.j2" for t in includes]
+        includes = [abcs.Path(t) / "**" / self.config.file_glob for t in includes]
         LOGGER.warning(includes)
         matches = files.find_globs(includes)
         return matches
 
     @cli.click.flag("--local")
     def list_include_args(
         self,
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/json.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/json.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 """
 
 from pynchon import abcs, models  # noqa
 from pynchon.util import lme, typing  # noqa
 
 LOGGER = lme.get_logger(__name__)
 
+from pynchon.models.planner import RenderingPlugin  # noqa
 
-class Json(models.ToolPlugin):
+
+class Json(RenderingPlugin):
     """Tools for working with JSON & JSON5"""
 
     class config_class(abcs.Config):
         config_key: typing.ClassVar[str] = "json"
 
     # cli_subsumes: typing.List[typing.Callable] = [
     #     loadf_main.json5,
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/makefile.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/makefile.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 from pynchon import abcs, api, events, models  # noqa
 from pynchon.util import lme, typing  # noqa
 
 LOGGER = lme.get_logger(__name__)
 
 
 class Make(models.Planner):
-    """Makefile parser"""
+    """Visualization and parsing tools for inspecting Makefiles"""
 
     class config_class(abcs.Config):
         config_key: typing.ClassVar[str] = "makefile"
         file: str = typing.Field(default=None)
 
         @property
         def file(self):
             # from pynchon.config import project
             tmp = abcs.Path(".").absolute()
             return tmp / "Makefile"
 
     priority = 6  # before mermaid
     name = "makefile"
     cli_name = "makefile"
-    cli_label = "Meta"
+    cli_label = "Project Tools"
 
     def _get_template_file(self, relpath: str = ""):
         tfile = self.plugin_templates_root / relpath
         return api.render.get_template(str(tfile))
 
     @property
     def diagrams_root(self):
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/markdown.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/markdown.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,64 @@
 """ pynchon.plugins.markdown
 """
 
 import marko
-from bs4 import BeautifulSoup
 from fleks import tagging
 
 from pynchon import abcs, api, cli, events, models  # noqa
 from pynchon.util import files, lme, text, typing  # noqa
 
 LOGGER = lme.get_logger(__name__)
 
 ElementList = typing.List[typing.Dict]
 
 
-class Markdown(models.Planner):
-    """
-    Example usage:
-        # normalize markdown syntax (in-place)
-        $ pynchon markdown normalize file1 file2
-    """
+class Markdown(models.DockerWrapper, models.Planner):
+    """Markdown Tools"""
 
     class config_class(abcs.Config):
         config_key: typing.ClassVar[str] = "markdown"
-        goals: typing.List[str] = typing.Field(default=[])
-        include_patterns: typing.List[str] = typing.Field(default=[])
-        exclude_patterns: typing.List[str] = typing.Field(default=[])
-        root: typing.Union[str, abcs.Path, None] = typing.Field(default=None)
+        goals: typing.List[str] = typing.Field(
+            default=[], description="Extra goals related to markdown"
+        )
+        include_patterns: typing.List[str] = typing.Field(
+            default=[], description="Patterns to include"
+        )
+        exclude_patterns: typing.List[str] = typing.Field(
+            default=[], description="File globs to exclude from listing"
+        )
+        root: typing.Union[str, abcs.Path, None] = typing.Field(
+            default=None, description=""
+        )
         linter_docker_image: str = typing.Field(
-            default="peterdavehello/markdownlint", help=""
+            default="peterdavehello/markdownlint",
+            description="Container to use for markdown linter",
         )
         linter_args: typing.List[str] = typing.Field(
-            help="arguments to pass to `linter_docker_image`",
+            description="Arguments to pass to `linter_docker_image`",
             default=[
                 "--disable MD013",  # line-length
                 "--disable MD045",  # Images should have alternate text
                 "--disable MD033",  # Allow HTML
                 "--disable MD041",  # first-line-h1
                 "--disable MD042",  # No empty links
                 "--fix",
             ],
         )
-        goals: typing.List[typing.Dict] = typing.Field(default=[], help="")
+        goals: typing.List[typing.Dict] = typing.Field(default=[], description="")
 
     name = "markdown"
     cli_name = "markdown"
+    cli_label = "Docs Tools"
     priority = 0
 
     @tagging.tags(click_aliases=["ls"])
     def list(self, changes=False):
         """
-        Lists affected resources for this project
+        Lists affected resources (**.md) for this project
         """
         default = self[:"project"]
         proj_conf = self[:"project.subproject":default]
         project_root = proj_conf.get("root", None) or self[:"git.root":"."]
         # project_root = proj_conf.get("root", None) or '.'
         globs = [
             abcs.Path(project_root).joinpath("**/*.md"),
@@ -86,14 +91,41 @@
                         f"-w /workspace {docker_image} "
                         f"markdownlint {linter_args} {path}"
                     ),
                 )
             )
         return self.apply(plan=self.plan(goals=goals))
 
+    @cli.click.argument("paths", nargs=-1)
+    @tagging.tags(click_aliases=["show"])
+    def preview(self, paths):
+        """
+        Previews markdown in the terminal
+        """
+        # FIXME?: rich doesn't link hypertext.  patch upstream?
+        from rich.console import Console
+        from rich.markdown import Markdown
+
+        console = Console()
+        for p in paths:
+            with open(p) as fhandle:
+                md = Markdown(fhandle.read())
+                console.print(md)
+        # FIXME: glow is awesome but using it from docker seems to strip color
+        # viewer_docker_image: str = typing.Field(
+        #     default='charmcli/glow',
+        #     help="Container to use for markdown console viewer")
+        # docker_image = self["viewer_docker_image"]
+        #         # viewer_args = " ".join(self["viewer_args"])
+        #         return self._run_docker(
+        #                         f"docker run -t -v `pwd`:/workspace "
+        #                         f"-w /workspace {docker_image} "
+        #                         f" {' '.join(paths)}"
+        #                     )
+
     @cli.click.flag("-p", "--python", help="only python codeblocks")
     @cli.click.flag("-b", "--bash", help="only bash codeblocks")
     @cli.click.argument("file")
     def doctest(
         self,
         file: str = None,
         python: bool = False,
@@ -130,14 +162,16 @@
         all: bool = False,
         codeblocks: bool = False,
         python: bool = False,
         links: bool = False,
         bash: bool = False,
     ) -> ElementList:
         """Parses given markdown file into JSON"""
+        from bs4 import BeautifulSoup  # noqa
+        from marko.ast_renderer import ASTRenderer  # noqa
 
         codeblocks = codeblocks or python or bash
         assert files or all and not (files and all)
         if files:
             files = list(files)
         else:
             files = self.list()
@@ -155,16 +189,14 @@
                 for a in soup.find_all("a", href=True):
                     this_link = a["href"]
                     if this_link.strip() == "#":
                         LOGGER.warning(f"{file}: has placeholder link '#' ")
                     else:
                         out[file] += [this_link]
             else:
-                from marko.ast_renderer import ASTRenderer
-
                 parsed = marko.Markdown(renderer=ASTRenderer)(content)
                 children = parsed["children"]
                 out[file] = []
                 for child in children:
                     if child.get("element") == "fenced_code":
                         lang = child.get("lang")
                         if lang is not None:
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/mermaid.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/mermaid.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 
 from pynchon import abcs, events, models  # noqa
 from pynchon.util import files, lme, typing  # noqa
 
 LOGGER = lme.get_logger(__name__)
 
 
-class Mermaid(models.DockerWrapper):
-    """Mermaid Plugin"""
+class Mermaid(models.DiagramTool):
+    """
+    Finds & renders Mermaid diagram files
+    """
 
     class config_class(abcs.Config):
         config_key: typing.ClassVar[str] = "mermaid"
         apply_hooks: typing.List[str] = typing.Field(default=["open-after"])
         docker_image: str = typing.Field(
             default="ghcr.io/mermaid-js/mermaid-cli/mermaid-cli:10.8.1-beta.15"
         )
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/mkdocs.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/mkdocs.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
 
 class Mkdocs(models.Planner):
     """Mkdocs helper"""
 
     priority = 8  # before mermaid
     name = "mkdocs"
     cli_name = "mkdocs"
-    cli_label = "Docs"
+    cli_label = "Docs Tools"
     config_class = MkdocsPluginConfig
 
     @property
     def config_file(self) -> str:
         return self["config_file"]
 
     def serve(self, background: bool = True):
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/pandoc.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/pandoc.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,27 +8,29 @@
 from pynchon import abcs, events, models  # noqa
 from pynchon.util import lme, typing  # noqa
 
 LOGGER = lme.get_logger(__name__)
 
 
 class Pandoc(models.DockerWrapper, models.Planner):
-    """Tool for working with Pandoc"""
+    """
+    Wrapper around `pandoc` docker image
+    """
 
     class config_class(models.DockerWrapper.BaseConfig):
         config_key: typing.ClassVar[str] = "pandoc"
         docker_args: typing.List = typing.Field(
             default=["--toc", "--variable fontsize=10pt"]
         )
         docker_image: str = typing.Field(default="pandoc/extra:latest")
         goals: typing.List[typing.Dict] = typing.Field(default=[], help="")
 
     name = "pandoc"
     cli_name = "pandoc"
-    cli_label = "Tool"
+    cli_label = "Docs Tools"
     # contribute_plan_apply = False
 
     @cli.click.command(
         context_settings=dict(
             ignore_unknown_options=True,
             allow_extra_args=True,
         )
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/pattern.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/pattern.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/project.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/project.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/python/api.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/python/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """ pynchon.plugins.python.api
 """
 
 from fleks import cli, tagging
 
-from pynchon import abcs, models
+from pynchon import abcs
 from pynchon.api import render
 from pynchon.util import complexity, lme, typing
 
+from .common import PythonPlanner
+
 LOGGER = lme.get_logger(__name__)
 
 
 @tagging.tags(click_aliases=["pa"])
-class PythonAPI(models.Planner):
+class PythonAPI(PythonPlanner):
     """Generators for Python API docs"""
 
     class config_class(abcs.Config):
         config_key: typing.ClassVar[str] = "python-api"
         skip_private_methods: bool = typing.Field(default=True)
         skip_patterns: typing.List[str] = typing.Field(default=[])
         apply_hooks: typing.List[str] = typing.Field(default=["diff-after"])
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/python/cli.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/python/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,22 @@
 import importlib
 
 import shimport
 from fleks import cli, tagging
 from fleks.util.click import click_recursive_help
 from memoized_property import memoized_property
 
-from pynchon import abcs, api, models
+from pynchon import abcs, api
 from pynchon.models.python import EntrypointMetadata
 
+from .common import PythonPlanner
+
 from pynchon.util import lme, typing  # noqa
 
+
 config_mod = shimport.lazy(
     "pynchon.config",
 )
 LOGGER = lme.get_logger(__name__)
 import click
 
 
@@ -146,15 +149,15 @@
             }
         result = list(matches.values())
         result = [EntrypointMetadata(src_root=self.src_root, **x) for x in result]
         return result
 
 
 @tagging.tags(click_aliases=["pc"])
-class PythonCLI(models.Planner):
+class PythonCLI(PythonPlanner):
     """Generators for Python CLI docs"""
 
     name = "python-cli"
     cli_name = "python-cli"
     config_class = PythonCliConfig
 
     @cli.click.group
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/python/libcst.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/python/libcst.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 
 from pynchon import abcs, events, models  # noqa
 from pynchon.util import lme, python, typing  # noqa
 
 LOGGER = lme.get_logger(__name__)
 F_CODEMOD_YAML = ".libcst.codemod.yaml"
 
+from .common import PythonPlanner
 
-class LibCST(models.Planner):
+
+class LibCST(PythonPlanner):
     """
     Code-transforms via libcst[1]
     """
 
     class config_class(abcs.Config):
         config_key: typing.ClassVar[str] = "python-libcst"
 
     name = "python-libcst"
     cli_name = "python-libcst"
-    cli_label = "Tool"
 
     @cli.click.group("gen")
     def gen(self):
         """Generates code for python modules, packages, etc"""
 
     @tagging.tags(click_aliases=["src.transform"])
     @cli.click.argument("transform_name", nargs=1)
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/python/platform.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/python/platform.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """ pynchon.plugins.python.platform:
 """
 
 import platform as stdlib_platform
 
 from fleks import tagging
 
-from pynchon import abcs, cli, models
+from pynchon import abcs, cli
 from pynchon.util import lme, python, typing
 from pynchon.util.os import invoke
 
+from .common import PythonPlanner
+
 LOGGER = lme.get_logger(__name__)
 
 
 @tagging.tags(click_aliases=["py"])
-class PythonPlatform(models.Planner):
+class PythonPlatform(PythonPlanner):
     """
-    Code transformation and docs-generation utilities for python projects.
+    Tools and info for Python projects and platforms
     """
 
     class config_class(abcs.Config):
         config_key: typing.ClassVar[str] = "python"
         libcst: typing.Dict[str, typing.Any] = typing.Field(default={})
 
         @property
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/python/pypi.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/python/pypi.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/release.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/release.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/render.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/render.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/scaffolding/__init__.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/scaffolding/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/scaffolding/config.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/scaffolding/config.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/src.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/src.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,17 @@
 
     class config_class(abcs.Config):
         config_key: typing.ClassVar[str] = "src"
         goals: typing.List[str] = typing.Field(default=[])
         include_patterns: typing.List[str] = typing.Field(default=[])
         exclude_patterns: typing.List[str] = typing.Field(default=[])
         root: typing.Union[str, abcs.Path, None] = typing.Field(default=None)
-        sorted: bool = typing.Field(default=False, help="Whether to sort source code")
+        sorted: bool = typing.Field(
+            default=False, description="Whether to sort source code"
+        )
 
     name = "src"
     cli_name = "src"
     priority = 0
 
     # @tagging.tagged_property(conflict_strategy="override")
     # @property
@@ -159,19 +161,19 @@
         with open(fname, "w") as fhandle:
             fhandle.write(result)
         LOGGER.warning(f"wrote {fname}")
         return fname
 
     @cli.click.group("open")
     def _open(self):
-        """helper for opening project source files"""
+        """Helper for opening project source files"""
 
     @_open.command("recent")
     def open_recent(self):
-        """opens recently changed files"""
+        """Opens recently changed files"""
 
     @_open.command("changed")
     def open_changed(self):
         """opens changed files"""
 
     def plan(self, config=None):
         """Describe plan for this plugin"""
@@ -195,25 +197,18 @@
                 self.goal(
                     resource=rsrc,
                     type="change",
                     label=f"Adding file header for '{ext}'",
                     command=f"{cmd_t} {fhdr} {rsrc}",
                 )
             )
-        # for rsrc in self._plan_empties(resources):
-        #     plan.append(
-        #         self.goal(
-        #             resource=rsrc,
-        #             type='delete',
-        #             command=f'rm {rsrc}',
-        #         )
-        #     )
         return plan
 
-    def find(self):
-        """file finder"""
-
-    def header(self):
-        """creates file headers for source in {src_root}"""
-
-    def map(self):
-        """file mapper"""
+    #
+    # def find(self):
+    #     """file finder"""
+    #
+    # def header(self):
+    #     """creates file headers for source in {src_root}"""
+    #
+    # def map(self):
+    #     """file mapper"""
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/tests.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 
 class Tests(models.Planner):
     """Management tool for project tests"""
 
     config_class = TestConfig
     name = "test"
     cli_name = "test"
+    cli_label = "Project Tools"
 
     def _test_md(self, fname):
         """ """
         cfg = self.config
         LOGGER.warning(f"testing markdown: {fname}")
 
     # @cli.click.flag(
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/plugins/util.py` & `pynchon-2024.4.5.14.1/src/pynchon/plugins/util.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/templates/docker/Dockerfile.pandoc` & `pynchon-2024.4.5.14.1/src/pynchon/templates/docker/Dockerfile.pandoc`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bash.sh` & `pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bash.sh`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bashrc.sh` & `pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bashrc.sh`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/tox.ini` & `pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/tox.ini`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/makefile/mermaid-graph.mmd.j2` & `pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/makefile/mermaid-graph.mmd.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2` & `pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2` & `pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2` & `pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2` & `pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python_cli/TOC.md.j2` & `pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python_cli/TOC.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python_cli/main.module.md.j2` & `pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python_cli/main.module.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python_cli/script.console.md.j2` & `pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python_cli/script.console.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/docker/.dockerignore` & `pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/docker/.dockerignore`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/docker/README.md.j2` & `pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/docker/README.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/.libcst.codemod.yaml` & `pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/Makefile` & `pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/Makefile`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/README.md` & `pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/README.md`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/README.md.j2` & `pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/README.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/setup.cfg` & `pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/setup.cfg`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/setup.py` & `pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/setup.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tox.ini` & `pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tox.ini`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/__init__.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/complexity.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/complexity.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/docker.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/docker.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/events.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/events.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/files/__init__.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/files/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/files/__main__.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/files/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     .starmap(
         lambda fxn, aliases: [
             entry.command(
                 name=alias.replace("_", "-"),
                 help=(
                     fxn.__doc__
                     if alias == fxn.__name__
-                    else f"alias for `{fxn.__name__}`"
+                    else f"Alias for `{fxn.__name__}`"
                 ),
             )(fxn)
             for alias in aliases
         ]
     )
 )
 if __name__ == "__main__":
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/files/diff.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/files/diff.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/lme.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/lme.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/makefile/__init__.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/makefile/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/oop.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/oop.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/os/__init__.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/os/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/os/models.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/os/models.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/os/pids.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/os/pids.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/python.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/python.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/text/__init__.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/text/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/text/dumpf/__init__.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/text/dumpf/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/text/dumpf/__main__.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/text/dumpf/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         lambda fxn, aliases: [
             common.kommand(
                 name=alias.replace("_", "-"),
                 parent=entry,
                 help=(
                     fxn.__doc__
                     if alias == fxn.__name__
-                    else f"alias for `{fxn.__name__}`"
+                    else f"Alias for `{fxn.__name__}`"
                 ),
             )(fxn)
             for alias in aliases
         ],
         logger=LOGGER,
     )
 )
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/text/dumps.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/text/dumps.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/text/loadf/__init__.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/text/loadf/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/text/loadf/__main__.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/text/loadf/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         lambda fxn, aliases: [
             common.kommand(
                 name=alias.replace("_", "-"),
                 parent=entry,
                 help=(
                     fxn.__doc__
                     if alias == fxn.__name__
-                    else f"alias for `{fxn.__name__}`"
+                    else f"Alias for `{fxn.__name__}`"
                 ),
             )(fxn)
             for alias in aliases
         ],
         logger=LOGGER,
     )
 )
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/text/loads.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/text/loads.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/text/normalize/__init__.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/text/normalize/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/text/render/__init__.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/text/render/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/text/render/__main__.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/text/render/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     .starmap(
         lambda fxn, aliases: [
             entry.command(
                 name=alias.replace("_", "-"),
                 help=(
                     fxn.__doc__
                     if alias == fxn.__name__
-                    else f"alias for `{fxn.__name__}`"
+                    else f"Alias for `{fxn.__name__}`"
                 ),
             )(fxn)
             for alias in aliases
         ]
     )
 )
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon/util/typing.py` & `pynchon-2024.4.5.14.1/src/pynchon/util/typing.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.15/src/pynchon.egg-info/PKG-INFO` & `pynchon-2024.4.5.14.1/src/pynchon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynchon
-Version: 2024.4.3.17.15
+Version: 2024.4.5.14.1
 Summary: Autodocs for python projects
 Home-page: https://github.com/elo-enterprises/pynchon/
 Author: elo
 Author-email: engineering@elo.enterprises
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/pynchon/
 Project-URL: Source, https://github.com/elo-enterprises/pynchon/
@@ -12,15 +12,15 @@
 Platform: any
 Classifier: Programming Language :: Python
 Requires-Python: >3.6
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Requires-Dist: gripe>=2024.2.24.1.31
 Requires-Dist: shil>=2023.7.17.7.1
 Requires-Dist: shimport>=2023.7.11.23.36
-Requires-Dist: fleks==2024.2.9.23.58
+Requires-Dist: fleks==2024.4.5.9.29
 Requires-Dist: memoization==0.4.0
 Requires-Dist: multipledispatch==0.6.0
 Requires-Dist: pygments
 Requires-Dist: pyjson5==1.6.1
 Requires-Dist: marko==2.0.0
 Requires-Dist: pyyaml
 Requires-Dist: trogon
```

### Comparing `pynchon-2024.4.3.17.15/src/pynchon.egg-info/SOURCES.txt` & `pynchon-2024.4.5.14.1/src/pynchon.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -83,33 +83,33 @@
 src/pynchon/plugins/plugins.py
 src/pynchon/plugins/project.py
 src/pynchon/plugins/release.py
 src/pynchon/plugins/render.py
 src/pynchon/plugins/rtd.py
 src/pynchon/plugins/src.py
 src/pynchon/plugins/tests.py
-src/pynchon/plugins/tox.py
 src/pynchon/plugins/util.py
 src/pynchon/plugins/docs/__init__.py
 src/pynchon/plugins/docs/main.py
 src/pynchon/plugins/docs/opener.py
 src/pynchon/plugins/doctor/__init__.py
 src/pynchon/plugins/python/__init__.py
 src/pynchon/plugins/python/api.py
 src/pynchon/plugins/python/cli.py
+src/pynchon/plugins/python/common.py
 src/pynchon/plugins/python/config.py
-src/pynchon/plugins/python/cst.py
 src/pynchon/plugins/python/libcst.py
 src/pynchon/plugins/python/models.py
 src/pynchon/plugins/python/platform.py
 src/pynchon/plugins/python/pypi.py
 src/pynchon/plugins/scaffolding/__init__.py
 src/pynchon/plugins/scaffolding/config.py
 src/pynchon/templates/docker/Dockerfile.pandoc
 src/pynchon/templates/docs/README.md
+src/pynchon/templates/includes/pynchon/pydantic-model.md.j2
 src/pynchon/templates/includes/pynchon/github/header.md.j2
 src/pynchon/templates/includes/pynchon/plugins/core/VERSIONS.md.j2
 src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/Makefile
 src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bash.sh
 src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bashrc.sh
 src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/makefile.j2
 src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/python.j2
```

