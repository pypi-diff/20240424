# Comparing `tmp/mkdocs-obsidian-interactive-graph-plugin-0.2.4.tar.gz` & `tmp/mkdocs_obsidian_interactive_graph_plugin-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-obsidian-interactive-graph-plugin-0.2.4.tar", last modified: Fri Mar 29 19:28:56 2024, max compression
+gzip compressed data, was "mkdocs_obsidian_interactive_graph_plugin-0.2.6.tar", last modified: Wed Apr 24 18:50:05 2024, max compression
```

## Comparing `mkdocs-obsidian-interactive-graph-plugin-0.2.4.tar` & `mkdocs_obsidian_interactive_graph_plugin-0.2.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:28:56.978283 mkdocs-obsidian-interactive-graph-plugin-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-29 19:28:52.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/.env
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:28:56.970283 mkdocs-obsidian-interactive-graph-plugin-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:28:56.974283 mkdocs-obsidian-interactive-graph-plugin-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-03-29 19:28:52.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-29 19:28:52.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-29 19:28:52.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-29 19:28:52.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-03-29 19:28:56.978283 mkdocs-obsidian-interactive-graph-plugin-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-03-29 19:28:52.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-29 19:28:52.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:28:56.974283 mkdocs-obsidian-interactive-graph-plugin-0.2.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:28:56.974283 mkdocs-obsidian-interactive-graph-plugin-0.2.4/docs/ObsidianVault/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-29 19:28:52.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/docs/ObsidianVault/Concept.md
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-29 19:28:52.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/docs/ObsidianVault/Docker.md
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-29 19:28:52.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/docs/ObsidianVault/Installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-29 19:28:52.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/docs/ObsidianVault/References.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:28:56.974283 mkdocs-obsidian-interactive-graph-plugin-0.2.4/docs/ObsidianVault/Usage/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-29 19:28:52.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/docs/ObsidianVault/Usage/ECharts.md
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-29 19:28:52.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/docs/ObsidianVault/Usage/Setup.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:28:56.974283 mkdocs-obsidian-interactive-graph-plugin-0.2.4/docs/ObsidianVault/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:28:56.978283 mkdocs-obsidian-interactive-graph-plugin-0.2.4/docs/ObsidianVault/assets/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-03-29 19:28:52.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/docs/ObsidianVault/assets/javascripts/interactive_graph.js
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-29 19:28:52.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/docs/ObsidianVault/assets/javascripts/obsidian_tags.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:28:56.978283 mkdocs-obsidian-interactive-graph-plugin-0.2.4/docs/ObsidianVault/assets/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-29 19:28:52.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/docs/ObsidianVault/assets/stylesheets/interactive_graph.css
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-29 19:28:52.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/docs/ObsidianVault/assets/stylesheets/obsidian_tags.css
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-03-29 19:28:52.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/docs/ObsidianVault/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-03-29 19:28:52.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:28:56.978283 mkdocs-obsidian-interactive-graph-plugin-0.2.4/mkdocs_obsidian_interactive_graph_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-03-29 19:28:56.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/mkdocs_obsidian_interactive_graph_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-29 19:28:56.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/mkdocs_obsidian_interactive_graph_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 19:28:56.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/mkdocs_obsidian_interactive_graph_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-29 19:28:56.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/mkdocs_obsidian_interactive_graph_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-29 19:28:56.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/mkdocs_obsidian_interactive_graph_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-29 19:28:56.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/mkdocs_obsidian_interactive_graph_plugin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:28:56.978283 mkdocs-obsidian-interactive-graph-plugin-0.2.4/obsidian_interactive_graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 19:28:52.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/obsidian_interactive_graph/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4844 2024-03-29 19:28:52.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/obsidian_interactive_graph/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-29 19:28:52.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 19:28:56.978283 mkdocs-obsidian-interactive-graph-plugin-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-29 19:28:52.000000 mkdocs-obsidian-interactive-graph-plugin-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:05.091239 mkdocs_obsidian_interactive_graph_plugin-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-24 18:49:58.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/.env
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:05.087239 mkdocs_obsidian_interactive_graph_plugin-0.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:05.087239 mkdocs_obsidian_interactive_graph_plugin-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-24 18:49:58.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 18:49:58.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-24 18:49:58.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-24 18:49:58.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-24 18:50:05.091239 mkdocs_obsidian_interactive_graph_plugin-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-24 18:49:58.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-24 18:49:58.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:05.087239 mkdocs_obsidian_interactive_graph_plugin-0.2.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:05.091239 mkdocs_obsidian_interactive_graph_plugin-0.2.6/docs/ObsidianVault/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-24 18:49:58.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/docs/ObsidianVault/Concept.md
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-24 18:49:58.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/docs/ObsidianVault/Docker.md
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-24 18:49:58.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/docs/ObsidianVault/Installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-24 18:49:58.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/docs/ObsidianVault/References.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:05.091239 mkdocs_obsidian_interactive_graph_plugin-0.2.6/docs/ObsidianVault/Usage/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-24 18:49:58.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/docs/ObsidianVault/Usage/ECharts.md
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-24 18:49:58.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/docs/ObsidianVault/Usage/Setup.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:05.087239 mkdocs_obsidian_interactive_graph_plugin-0.2.6/docs/ObsidianVault/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:05.091239 mkdocs_obsidian_interactive_graph_plugin-0.2.6/docs/ObsidianVault/assets/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-04-24 18:49:58.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/docs/ObsidianVault/assets/javascripts/interactive_graph.js
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-24 18:49:58.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/docs/ObsidianVault/assets/javascripts/obsidian_tags.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:05.091239 mkdocs_obsidian_interactive_graph_plugin-0.2.6/docs/ObsidianVault/assets/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-24 18:49:58.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/docs/ObsidianVault/assets/stylesheets/interactive_graph.css
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-24 18:49:58.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/docs/ObsidianVault/assets/stylesheets/obsidian_tags.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-24 18:49:58.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/docs/ObsidianVault/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-24 18:49:58.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:05.091239 mkdocs_obsidian_interactive_graph_plugin-0.2.6/mkdocs_obsidian_interactive_graph_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-24 18:50:05.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/mkdocs_obsidian_interactive_graph_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-24 18:50:05.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/mkdocs_obsidian_interactive_graph_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:50:05.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/mkdocs_obsidian_interactive_graph_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-24 18:50:05.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/mkdocs_obsidian_interactive_graph_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 18:50:05.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/mkdocs_obsidian_interactive_graph_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 18:50:05.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/mkdocs_obsidian_interactive_graph_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:05.091239 mkdocs_obsidian_interactive_graph_plugin-0.2.6/obsidian_interactive_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:49:58.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/obsidian_interactive_graph/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4845 2024-04-24 18:49:58.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/obsidian_interactive_graph/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-24 18:49:58.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 18:50:05.091239 mkdocs_obsidian_interactive_graph_plugin-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-24 18:49:58.000000 mkdocs_obsidian_interactive_graph_plugin-0.2.6/setup.py
```

### Comparing `mkdocs-obsidian-interactive-graph-plugin-0.2.4/.github/workflows/ci.yml` & `mkdocs_obsidian_interactive_graph_plugin-0.2.6/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,18 @@
     permissions:
       id-token: write
     steps:
       - name: Download Artifact
         uses: actions/download-artifact@v4
         with:
           name: dist
-      - run: mkdir dist; mv mkdocs-obsidian-interactive-graph-plugin-*.tar.gz dist
+          path: dist
+      - name: List
+        run: |
+          ls dist
       - name: Publish package distributions to PyPI
         if: startsWith(github.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           skip-existing: true
 
   deploy:
```

### Comparing `mkdocs-obsidian-interactive-graph-plugin-0.2.4/LICENSE` & `mkdocs_obsidian_interactive_graph_plugin-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-obsidian-interactive-graph-plugin-0.2.4/PKG-INFO` & `mkdocs_obsidian_interactive_graph_plugin-0.2.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-obsidian-interactive-graph-plugin
-Version: 0.2.4
+Version: 0.2.6
 Summary: A MkDocs plugin that generates a obsidian like interactive graph
 Home-page: https://github.com/daxcore/mkdocs-obsidian-interactive-graph-plugin
 Author: daxcore
 Author-email: 300ccda6-8d43-4f23-808e-961e653ff7d6@anonaddy.com
 License: MIT
 Keywords: mkdocs
 Classifier: Development Status :: 4 - Beta
@@ -25,33 +25,41 @@
 
 # Interactive Graph for Material for MkDocs
 Plugin for Material for MkDocs to draw an interactive graph like Obsidian.
 The graph inside the sidebar is just available for non-mobile website. The modal view via the button next to the light/dark mode switch shall work on all devices.
 
 Refer [Github Pages](https://daxcore.github.io/mkdocs-obsidian-interactive-graph-plugin/) for a **demonstration** of the interactive graph in Material for MkDocs.
 
+[![Build Status](https://github.com/daxcore/mkdocs-obsidian-interactive-graph-plugin/actions/workflows/ci.yml/badge.svg)](https://github.com/daxcore/mkdocs-obsidian-interactive-graph-plugin/actions/workflows/ci.yml)
+[![PyPI Version](https://img.shields.io/pypi/v/mkdocs-obsidian-interactive-graph-plugin)](https://pypi.org/project/mkdocs-obsidian-interactive-graph-plugin/)
+[![PyPi Downloads](https://img.shields.io/pypi/dm/mkdocs-obsidian-interactive-graph-plugin.svg)](https://pypi.org/project/mkdocs-obsidian-interactive-graph-plugin/)
+[![GitHub License](https://img.shields.io/github/license/daxcore/mkdocs-obsidian-interactive-graph-plugin)](https://github.com/daxcore/mkdocs-obsidian-interactive-graph-plugin/blob/main/LICENSE)
+
 # Installation
 Available on [PyPI](https://pypi.org/project/mkdocs-obsidian-interactive-graph-plugin/).
 Install via `pip install mkdocs-obsidian-interactive-graph-plugin` or add it to your `requirements.txt`.
 
 # Usage
 ## Setup in MkDocs
 Activate the plugin in `mkdocs.yml`, but **note** that this plugin has to be located before plugins, that replace wikilinks by markdown links. Currently just wikilinks like `[[Link#Anchor|Custom Text]]` are supported.
 ```
 plugins:
   - obsidian-interactive-graph
 
 extra_javascript:
-  - https://fastly.jsdelivr.net/npm/jquery@3.7.1/dist/jquery.min.js
-  - https://fastly.jsdelivr.net/npm/echarts@5.5.0/dist/echarts.min.js
-  - assets/javascripts/graph.js
+  - https://fastly.jsdelivr.net/npm/jquery/dist/jquery.min.js
+  - https://fastly.jsdelivr.net/npm/echarts/dist/echarts.min.js
+  - assets/javascripts/interactive_graph.js
+
+extra_css:
+  - assets/stylesheets/interactive_graph.css
 ```
 
 ## Graph Javascript by Apache ECharts
-A `graph.js` example can be downloaded from [here](https://raw.githubusercontent.com/daxcore/mkdocs-obsidian-interactive-graph-plugin/main/docs/ObsidianVault/assets/javascripts/graph.js) and must be located into the docs directory under `docs/YourSiteName/assets/javascripts/graph.js`.
+A `interactive_graph.js` example can be downloaded from [here](https://raw.githubusercontent.com/daxcore/mkdocs-obsidian-interactive-graph-plugin/main/docs/ObsidianVault/assets/javascripts/interactive_graph.js) and must be located into the docs directory under `docs/YourSiteName/assets/javascripts/interactive_graph.js`.
 
 # Docker
 Adapt the `.env` and `mkdocs.yml` files to your needs. `DEV=ON` will rebuild the `mkdocs-obsidian-interactive-graph-plugin` from local files. If `DEV != ON` the upstream packages of PyPI will be used. Build and start the Docker container via `docker compose up --build [-d]`.
 
 # References
 * https://www.mkdocs.org/
 * https://squidfunk.github.io/mkdocs-material/
```

### Comparing `mkdocs-obsidian-interactive-graph-plugin-0.2.4/README.md` & `mkdocs_obsidian_interactive_graph_plugin-0.2.6/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 # Interactive Graph for Material for MkDocs
 Plugin for Material for MkDocs to draw an interactive graph like Obsidian.
 The graph inside the sidebar is just available for non-mobile website. The modal view via the button next to the light/dark mode switch shall work on all devices.
 
 Refer [Github Pages](https://daxcore.github.io/mkdocs-obsidian-interactive-graph-plugin/) for a **demonstration** of the interactive graph in Material for MkDocs.
 
+[![Build Status](https://github.com/daxcore/mkdocs-obsidian-interactive-graph-plugin/actions/workflows/ci.yml/badge.svg)](https://github.com/daxcore/mkdocs-obsidian-interactive-graph-plugin/actions/workflows/ci.yml)
+[![PyPI Version](https://img.shields.io/pypi/v/mkdocs-obsidian-interactive-graph-plugin)](https://pypi.org/project/mkdocs-obsidian-interactive-graph-plugin/)
+[![PyPi Downloads](https://img.shields.io/pypi/dm/mkdocs-obsidian-interactive-graph-plugin.svg)](https://pypi.org/project/mkdocs-obsidian-interactive-graph-plugin/)
+[![GitHub License](https://img.shields.io/github/license/daxcore/mkdocs-obsidian-interactive-graph-plugin)](https://github.com/daxcore/mkdocs-obsidian-interactive-graph-plugin/blob/main/LICENSE)
+
 # Installation
 Available on [PyPI](https://pypi.org/project/mkdocs-obsidian-interactive-graph-plugin/).
 Install via `pip install mkdocs-obsidian-interactive-graph-plugin` or add it to your `requirements.txt`.
 
 # Usage
 ## Setup in MkDocs
 Activate the plugin in `mkdocs.yml`, but **note** that this plugin has to be located before plugins, that replace wikilinks by markdown links. Currently just wikilinks like `[[Link#Anchor|Custom Text]]` are supported.
 ```
 plugins:
   - obsidian-interactive-graph
 
 extra_javascript:
-  - https://fastly.jsdelivr.net/npm/jquery@3.7.1/dist/jquery.min.js
-  - https://fastly.jsdelivr.net/npm/echarts@5.5.0/dist/echarts.min.js
-  - assets/javascripts/graph.js
+  - https://fastly.jsdelivr.net/npm/jquery/dist/jquery.min.js
+  - https://fastly.jsdelivr.net/npm/echarts/dist/echarts.min.js
+  - assets/javascripts/interactive_graph.js
+
+extra_css:
+  - assets/stylesheets/interactive_graph.css
 ```
 
 ## Graph Javascript by Apache ECharts
-A `graph.js` example can be downloaded from [here](https://raw.githubusercontent.com/daxcore/mkdocs-obsidian-interactive-graph-plugin/main/docs/ObsidianVault/assets/javascripts/graph.js) and must be located into the docs directory under `docs/YourSiteName/assets/javascripts/graph.js`.
+A `interactive_graph.js` example can be downloaded from [here](https://raw.githubusercontent.com/daxcore/mkdocs-obsidian-interactive-graph-plugin/main/docs/ObsidianVault/assets/javascripts/interactive_graph.js) and must be located into the docs directory under `docs/YourSiteName/assets/javascripts/interactive_graph.js`.
 
 # Docker
 Adapt the `.env` and `mkdocs.yml` files to your needs. `DEV=ON` will rebuild the `mkdocs-obsidian-interactive-graph-plugin` from local files. If `DEV != ON` the upstream packages of PyPI will be used. Build and start the Docker container via `docker compose up --build [-d]`.
 
 # References
 * https://www.mkdocs.org/
 * https://squidfunk.github.io/mkdocs-material/
```

### Comparing `mkdocs-obsidian-interactive-graph-plugin-0.2.4/docs/ObsidianVault/References.md` & `mkdocs_obsidian_interactive_graph_plugin-0.2.6/docs/ObsidianVault/References.md`

 * *Files identical despite different names*

### Comparing `mkdocs-obsidian-interactive-graph-plugin-0.2.4/docs/ObsidianVault/assets/javascripts/interactive_graph.js` & `mkdocs_obsidian_interactive_graph_plugin-0.2.6/docs/ObsidianVault/assets/javascripts/interactive_graph.js`

 * *Files identical despite different names*

### Comparing `mkdocs-obsidian-interactive-graph-plugin-0.2.4/docs/ObsidianVault/assets/stylesheets/interactive_graph.css` & `mkdocs_obsidian_interactive_graph_plugin-0.2.6/docs/ObsidianVault/assets/stylesheets/interactive_graph.css`

 * *Files identical despite different names*

### Comparing `mkdocs-obsidian-interactive-graph-plugin-0.2.4/docs/ObsidianVault/index.md` & `mkdocs_obsidian_interactive_graph_plugin-0.2.6/docs/ObsidianVault/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs-obsidian-interactive-graph-plugin-0.2.4/mkdocs.yml` & `mkdocs_obsidian_interactive_graph_plugin-0.2.6/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 plugins:
   - search
   - callouts
   - obsidian-interactive-graph
   - obsidian-support
   - obsidian-bridge
   - glightbox
-  - privacy
 
 markdown_extensions:
   - admonition
   - attr_list
   - codehilite
   - md_in_html
   - def_list
@@ -63,11 +62,11 @@
       permalink: "#"
 
 extra_css:
   - assets/stylesheets/obsidian_tags.css
   - assets/stylesheets/interactive_graph.css
 
 extra_javascript:
-  - https://fastly.jsdelivr.net/npm/jquery@3.7.1/dist/jquery.min.js
-  - https://fastly.jsdelivr.net/npm/echarts@5.5.0/dist/echarts.min.js
+  - https://fastly.jsdelivr.net/npm/jquery/dist/jquery.min.js
+  - https://fastly.jsdelivr.net/npm/echarts/dist/echarts.min.js
   - assets/javascripts/obsidian_tags.js
   - assets/javascripts/interactive_graph.js
```

### Comparing `mkdocs-obsidian-interactive-graph-plugin-0.2.4/mkdocs_obsidian_interactive_graph_plugin.egg-info/PKG-INFO` & `mkdocs_obsidian_interactive_graph_plugin-0.2.6/mkdocs_obsidian_interactive_graph_plugin.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-obsidian-interactive-graph-plugin
-Version: 0.2.4
+Version: 0.2.6
 Summary: A MkDocs plugin that generates a obsidian like interactive graph
 Home-page: https://github.com/daxcore/mkdocs-obsidian-interactive-graph-plugin
 Author: daxcore
 Author-email: 300ccda6-8d43-4f23-808e-961e653ff7d6@anonaddy.com
 License: MIT
 Keywords: mkdocs
 Classifier: Development Status :: 4 - Beta
@@ -25,33 +25,41 @@
 
 # Interactive Graph for Material for MkDocs
 Plugin for Material for MkDocs to draw an interactive graph like Obsidian.
 The graph inside the sidebar is just available for non-mobile website. The modal view via the button next to the light/dark mode switch shall work on all devices.
 
 Refer [Github Pages](https://daxcore.github.io/mkdocs-obsidian-interactive-graph-plugin/) for a **demonstration** of the interactive graph in Material for MkDocs.
 
+[![Build Status](https://github.com/daxcore/mkdocs-obsidian-interactive-graph-plugin/actions/workflows/ci.yml/badge.svg)](https://github.com/daxcore/mkdocs-obsidian-interactive-graph-plugin/actions/workflows/ci.yml)
+[![PyPI Version](https://img.shields.io/pypi/v/mkdocs-obsidian-interactive-graph-plugin)](https://pypi.org/project/mkdocs-obsidian-interactive-graph-plugin/)
+[![PyPi Downloads](https://img.shields.io/pypi/dm/mkdocs-obsidian-interactive-graph-plugin.svg)](https://pypi.org/project/mkdocs-obsidian-interactive-graph-plugin/)
+[![GitHub License](https://img.shields.io/github/license/daxcore/mkdocs-obsidian-interactive-graph-plugin)](https://github.com/daxcore/mkdocs-obsidian-interactive-graph-plugin/blob/main/LICENSE)
+
 # Installation
 Available on [PyPI](https://pypi.org/project/mkdocs-obsidian-interactive-graph-plugin/).
 Install via `pip install mkdocs-obsidian-interactive-graph-plugin` or add it to your `requirements.txt`.
 
 # Usage
 ## Setup in MkDocs
 Activate the plugin in `mkdocs.yml`, but **note** that this plugin has to be located before plugins, that replace wikilinks by markdown links. Currently just wikilinks like `[[Link#Anchor|Custom Text]]` are supported.
 ```
 plugins:
   - obsidian-interactive-graph
 
 extra_javascript:
-  - https://fastly.jsdelivr.net/npm/jquery@3.7.1/dist/jquery.min.js
-  - https://fastly.jsdelivr.net/npm/echarts@5.5.0/dist/echarts.min.js
-  - assets/javascripts/graph.js
+  - https://fastly.jsdelivr.net/npm/jquery/dist/jquery.min.js
+  - https://fastly.jsdelivr.net/npm/echarts/dist/echarts.min.js
+  - assets/javascripts/interactive_graph.js
+
+extra_css:
+  - assets/stylesheets/interactive_graph.css
 ```
 
 ## Graph Javascript by Apache ECharts
-A `graph.js` example can be downloaded from [here](https://raw.githubusercontent.com/daxcore/mkdocs-obsidian-interactive-graph-plugin/main/docs/ObsidianVault/assets/javascripts/graph.js) and must be located into the docs directory under `docs/YourSiteName/assets/javascripts/graph.js`.
+A `interactive_graph.js` example can be downloaded from [here](https://raw.githubusercontent.com/daxcore/mkdocs-obsidian-interactive-graph-plugin/main/docs/ObsidianVault/assets/javascripts/interactive_graph.js) and must be located into the docs directory under `docs/YourSiteName/assets/javascripts/interactive_graph.js`.
 
 # Docker
 Adapt the `.env` and `mkdocs.yml` files to your needs. `DEV=ON` will rebuild the `mkdocs-obsidian-interactive-graph-plugin` from local files. If `DEV != ON` the upstream packages of PyPI will be used. Build and start the Docker container via `docker compose up --build [-d]`.
 
 # References
 * https://www.mkdocs.org/
 * https://squidfunk.github.io/mkdocs-material/
```

### Comparing `mkdocs-obsidian-interactive-graph-plugin-0.2.4/mkdocs_obsidian_interactive_graph_plugin.egg-info/SOURCES.txt` & `mkdocs_obsidian_interactive_graph_plugin-0.2.6/mkdocs_obsidian_interactive_graph_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-obsidian-interactive-graph-plugin-0.2.4/obsidian_interactive_graph/plugin.py` & `mkdocs_obsidian_interactive_graph_plugin-0.2.6/obsidian_interactive_graph/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                 "symbolSize": 0,
                 "markdown": page.markdown,
                 "is_index": page.is_index
             }
 
     def parse_markdown(self, markdown: str, page: MkDocsPage):
         # wikilinks: [[Link#Anchor|Custom Text]], just the link is needed
-        WIKI_PATTERN = re.compile(r"(?<!\!)\[\[(?P<wikilink>[^\|^\]^\#]{1,})(?:.*)\]\]")
+        WIKI_PATTERN = re.compile(r"(?<!\!)\[\[(?P<wikilink>[^\|^\]^\#]{1,})(?:.*?)\]\]")
         for match in re.finditer(WIKI_PATTERN, markdown):
             wikilink = match.group('wikilink')
 
             # get the nodes key
             page_path = self.get_page_path(page)
 
             # search page path of target page
```

### Comparing `mkdocs-obsidian-interactive-graph-plugin-0.2.4/setup.py` & `mkdocs_obsidian_interactive_graph_plugin-0.2.6/setup.py`

 * *Files identical despite different names*

