# Comparing `tmp/twitch_dl-2.2.1.tar.gz` & `tmp/twitch_dl-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitch_dl-2.2.1.tar", last modified: Tue Apr 23 15:26:10 2024, max compression
+gzip compressed data, was "twitch_dl-2.2.2.tar", last modified: Tue Apr 23 16:14:46 2024, max compression
```

## Comparing `twitch_dl-2.2.1.tar` & `twitch_dl-2.2.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 15:26:10.520835 twitch_dl-2.2.1/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       41 2023-08-11 10:29:42.000000 twitch_dl-2.2.1/.flake8
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      166 2023-08-11 10:29:32.000000 twitch_dl-2.2.1/.gitignore
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       65 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/.vermin
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9873 2024-04-23 15:25:40.000000 twitch_dl-2.2.1/CHANGELOG.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    35147 2023-08-11 10:29:42.000000 twitch_dl-2.2.1/LICENSE
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      951 2024-03-23 06:29:27.000000 twitch_dl-2.2.1/Makefile
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    43171 2024-04-23 15:26:10.520835 twitch_dl-2.2.1/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1627 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/README.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      343 2023-08-11 10:29:32.000000 twitch_dl-2.2.1/TODO.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      481 2023-08-11 10:29:32.000000 twitch_dl-2.2.1/book.css
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      223 2023-08-11 10:29:32.000000 twitch_dl-2.2.1/book.toml
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     8276 2024-04-23 15:25:30.000000 twitch_dl-2.2.1/changelog.yaml
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 15:26:10.516835 twitch_dl-2.2.1/docs/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      484 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/docs/SUMMARY.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      282 2023-08-11 10:29:47.000000 twitch_dl-2.2.1/docs/advanced.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9873 2024-04-23 15:25:40.000000 twitch_dl-2.2.1/docs/changelog.md
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 15:26:10.517835 twitch_dl-2.2.1/docs/commands/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    69599 2023-08-11 10:29:47.000000 twitch_dl-2.2.1/docs/commands/auth_token.png
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2499 2024-04-23 15:25:40.000000 twitch_dl-2.2.1/docs/commands/clips.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     6159 2024-04-23 15:25:40.000000 twitch_dl-2.2.1/docs/commands/download.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      722 2024-04-23 15:25:40.000000 twitch_dl-2.2.1/docs/commands/env.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      670 2024-04-23 15:25:40.000000 twitch_dl-2.2.1/docs/commands/info.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2030 2024-04-23 15:25:40.000000 twitch_dl-2.2.1/docs/commands/videos.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      420 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/docs/environment_variables.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1653 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/docs/installation.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1169 2023-08-11 10:29:47.000000 twitch_dl-2.2.1/docs/introduction.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    34916 2023-08-11 10:29:47.000000 twitch_dl-2.2.1/docs/license.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      664 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/docs/shell_completion.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      690 2023-08-11 10:29:47.000000 twitch_dl-2.2.1/docs/usage.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1269 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/pyproject.toml
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 15:26:10.517835 twitch_dl-2.2.1/scripts/
--rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     1026 2023-10-08 19:39:41.000000 twitch_dl-2.2.1/scripts/generate_changelog
--rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     3686 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/scripts/generate_docs
--rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     1587 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/scripts/tag_version
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2024-04-23 15:26:10.520835 twitch_dl-2.2.1/setup.cfg
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 15:26:10.518835 twitch_dl-2.2.1/tests/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1578 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/tests/test_api.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2020 2023-08-11 10:29:32.000000 twitch_dl-2.2.1/tests/test_patterns.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2605 2023-08-11 10:29:32.000000 twitch_dl-2.2.1/tests/test_progress.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      456 2023-08-11 10:29:32.000000 twitch_dl-2.2.1/tests/test_utils.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1350 2023-08-11 10:29:42.000000 twitch_dl-2.2.1/twitch-dl.1.scd
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 15:26:10.519835 twitch_dl-2.2.1/twitch_dl.egg-info/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    43171 2024-04-23 15:26:10.000000 twitch_dl-2.2.1/twitch_dl.egg-info/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1195 2024-04-23 15:26:10.000000 twitch_dl-2.2.1/twitch_dl.egg-info/SOURCES.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2024-04-23 15:26:10.000000 twitch_dl-2.2.1/twitch_dl.egg-info/dependency_links.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       47 2024-04-23 15:26:10.000000 twitch_dl-2.2.1/twitch_dl.egg-info/entry_points.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      111 2024-04-23 15:26:10.000000 twitch_dl-2.2.1/twitch_dl.egg-info/requires.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        9 2024-04-23 15:26:10.000000 twitch_dl-2.2.1/twitch_dl.egg-info/top_level.txt
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 15:26:10.519835 twitch_dl-2.2.1/twitchdl/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      196 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/twitchdl/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       36 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/twitchdl/__main__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9588 2024-04-23 15:10:23.000000 twitch_dl-2.2.1/twitchdl/cli.py
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 15:26:10.519835 twitch_dl-2.2.1/twitchdl/commands/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/twitchdl/commands/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2561 2024-04-23 15:09:23.000000 twitch_dl-2.2.1/twitchdl/commands/clips.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    11571 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/twitchdl/commands/download.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2929 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/twitchdl/commands/info.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2083 2024-04-23 15:09:38.000000 twitch_dl-2.2.1/twitchdl/commands/videos.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      931 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/twitchdl/download.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      510 2024-04-23 15:08:18.000000 twitch_dl-2.2.1/twitchdl/entities.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      139 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/twitchdl/exceptions.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4138 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/twitchdl/http.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4571 2024-04-23 15:10:46.000000 twitch_dl-2.2.1/twitchdl/output.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3652 2024-04-23 15:11:10.000000 twitch_dl-2.2.1/twitchdl/playlists.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4722 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/twitchdl/progress.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    11149 2024-04-23 15:12:20.000000 twitch_dl-2.2.1/twitchdl/twitch.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3099 2024-04-23 15:13:11.000000 twitch_dl-2.2.1/twitchdl/utils.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 16:14:46.794407 twitch_dl-2.2.2/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       41 2023-08-11 10:29:42.000000 twitch_dl-2.2.2/.flake8
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      166 2023-08-11 10:29:32.000000 twitch_dl-2.2.2/.gitignore
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       65 2024-04-23 15:07:42.000000 twitch_dl-2.2.2/.vermin
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    10004 2024-04-23 16:14:10.000000 twitch_dl-2.2.2/CHANGELOG.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    35147 2023-08-11 10:29:42.000000 twitch_dl-2.2.2/LICENSE
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      951 2024-03-23 06:29:27.000000 twitch_dl-2.2.2/Makefile
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    43171 2024-04-23 16:14:46.794407 twitch_dl-2.2.2/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1627 2024-04-23 15:07:42.000000 twitch_dl-2.2.2/README.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      343 2023-08-11 10:29:32.000000 twitch_dl-2.2.2/TODO.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      481 2023-08-11 10:29:32.000000 twitch_dl-2.2.2/book.css
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      223 2023-08-11 10:29:32.000000 twitch_dl-2.2.2/book.toml
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     8366 2024-04-23 16:14:08.000000 twitch_dl-2.2.2/changelog.yaml
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 16:14:46.791407 twitch_dl-2.2.2/docs/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      484 2024-04-23 15:07:42.000000 twitch_dl-2.2.2/docs/SUMMARY.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      282 2023-08-11 10:29:47.000000 twitch_dl-2.2.2/docs/advanced.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    10004 2024-04-23 16:14:10.000000 twitch_dl-2.2.2/docs/changelog.md
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 16:14:46.792407 twitch_dl-2.2.2/docs/commands/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    69599 2023-08-11 10:29:47.000000 twitch_dl-2.2.2/docs/commands/auth_token.png
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2499 2024-04-23 16:14:10.000000 twitch_dl-2.2.2/docs/commands/clips.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     6159 2024-04-23 16:14:10.000000 twitch_dl-2.2.2/docs/commands/download.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      722 2024-04-23 16:14:10.000000 twitch_dl-2.2.2/docs/commands/env.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      670 2024-04-23 16:14:10.000000 twitch_dl-2.2.2/docs/commands/info.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2030 2024-04-23 16:14:10.000000 twitch_dl-2.2.2/docs/commands/videos.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      420 2024-04-23 15:07:42.000000 twitch_dl-2.2.2/docs/environment_variables.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1653 2024-04-23 15:07:42.000000 twitch_dl-2.2.2/docs/installation.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1169 2023-08-11 10:29:47.000000 twitch_dl-2.2.2/docs/introduction.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    34916 2023-08-11 10:29:47.000000 twitch_dl-2.2.2/docs/license.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      664 2024-04-23 15:07:42.000000 twitch_dl-2.2.2/docs/shell_completion.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      690 2023-08-11 10:29:47.000000 twitch_dl-2.2.2/docs/usage.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1291 2024-04-23 16:07:59.000000 twitch_dl-2.2.2/pyproject.toml
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 16:14:46.792407 twitch_dl-2.2.2/scripts/
+-rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     1026 2023-10-08 19:39:41.000000 twitch_dl-2.2.2/scripts/generate_changelog
+-rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     3686 2024-04-23 15:07:42.000000 twitch_dl-2.2.2/scripts/generate_docs
+-rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     1587 2024-04-23 15:07:42.000000 twitch_dl-2.2.2/scripts/tag_version
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2024-04-23 16:14:46.794407 twitch_dl-2.2.2/setup.cfg
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 16:14:46.792407 twitch_dl-2.2.2/tests/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1578 2024-04-23 15:07:42.000000 twitch_dl-2.2.2/tests/test_api.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2020 2023-08-11 10:29:32.000000 twitch_dl-2.2.2/tests/test_patterns.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2605 2023-08-11 10:29:32.000000 twitch_dl-2.2.2/tests/test_progress.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      456 2023-08-11 10:29:32.000000 twitch_dl-2.2.2/tests/test_utils.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1350 2023-08-11 10:29:42.000000 twitch_dl-2.2.2/twitch-dl.1.scd
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 16:14:46.794407 twitch_dl-2.2.2/twitch_dl.egg-info/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    43171 2024-04-23 16:14:46.000000 twitch_dl-2.2.2/twitch_dl.egg-info/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1195 2024-04-23 16:14:46.000000 twitch_dl-2.2.2/twitch_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2024-04-23 16:14:46.000000 twitch_dl-2.2.2/twitch_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       47 2024-04-23 16:14:46.000000 twitch_dl-2.2.2/twitch_dl.egg-info/entry_points.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      111 2024-04-23 16:14:46.000000 twitch_dl-2.2.2/twitch_dl.egg-info/requires.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        9 2024-04-23 16:14:46.000000 twitch_dl-2.2.2/twitch_dl.egg-info/top_level.txt
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 16:14:46.793407 twitch_dl-2.2.2/twitchdl/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      196 2024-04-23 15:35:36.000000 twitch_dl-2.2.2/twitchdl/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       36 2024-04-23 15:35:35.000000 twitch_dl-2.2.2/twitchdl/__main__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9588 2024-04-23 16:07:01.000000 twitch_dl-2.2.2/twitchdl/cli.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 16:14:46.794407 twitch_dl-2.2.2/twitchdl/commands/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 15:07:42.000000 twitch_dl-2.2.2/twitchdl/commands/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2561 2024-04-23 15:09:23.000000 twitch_dl-2.2.2/twitchdl/commands/clips.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    11601 2024-04-23 16:13:32.000000 twitch_dl-2.2.2/twitchdl/commands/download.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2954 2024-04-23 16:10:44.000000 twitch_dl-2.2.2/twitchdl/commands/info.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2089 2024-04-23 16:11:06.000000 twitch_dl-2.2.2/twitchdl/commands/videos.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      932 2024-04-23 15:35:34.000000 twitch_dl-2.2.2/twitchdl/download.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      522 2024-04-23 16:09:59.000000 twitch_dl-2.2.2/twitchdl/entities.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      139 2024-04-23 15:35:32.000000 twitch_dl-2.2.2/twitchdl/exceptions.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4138 2024-04-23 15:35:32.000000 twitch_dl-2.2.2/twitchdl/http.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4577 2024-04-23 16:11:39.000000 twitch_dl-2.2.2/twitchdl/output.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3658 2024-04-23 16:11:56.000000 twitch_dl-2.2.2/twitchdl/playlists.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4722 2024-04-23 15:35:30.000000 twitch_dl-2.2.2/twitchdl/progress.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    11186 2024-04-23 16:12:23.000000 twitch_dl-2.2.2/twitchdl/twitch.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3099 2024-04-23 15:35:15.000000 twitch_dl-2.2.2/twitchdl/utils.py
```

### Comparing `twitch_dl-2.2.1/CHANGELOG.md` & `twitch_dl-2.2.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 twitch-dl changelog
 ===================
 
 <!-- Do not edit. This file is automatically generated from changelog.yaml.-->
 
+### [2.2.2 (2024-04-23)](https://github.com/ihabunek/twitch-dl/releases/tag/2.2.2)
+
+* Fix more compat issues Python < 3.10 (#152)
+
 ### [2.2.1 (2024-04-23)](https://github.com/ihabunek/twitch-dl/releases/tag/2.2.1)
 
-* Fix compat with < Python 3.10 (#152)
+* Fix compat with Python < 3.10 (#152)
 * Fix division by zero in progress calculation when video duration is reported
   as 0
 
 ### [2.2.0 (2024-04-10)](https://github.com/ihabunek/twitch-dl/releases/tag/2.2.0)
 
 * **Requires Python 3.8+**
 * Migrated to Click library for generating the commandline interface
```

### Comparing `twitch_dl-2.2.1/LICENSE` & `twitch_dl-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/Makefile` & `twitch_dl-2.2.2/Makefile`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/PKG-INFO` & `twitch_dl-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-dl
-Version: 2.2.1
+Version: 2.2.2
 Summary: Quickly download videos from twitch.tv from the comort of your terminal emulator
 Author-email: Ivan Habunek <ivan@habunek.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `twitch_dl-2.2.1/README.md` & `twitch_dl-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/changelog.yaml` & `twitch_dl-2.2.2/changelog.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
+2.2.2:
+  date: 2024-04-23
+  changes:
+    - "Fix more compat issues Python < 3.10 (#152)"
+
 2.2.1:
   date: 2024-04-23
   changes:
-    - "Fix compat with < Python 3.10 (#152)"
+    - "Fix compat with Python < 3.10 (#152)"
     - "Fix division by zero in progress calculation when video duration is reported as 0"
 
 2.2.0:
   date: 2024-04-10
   changes:
     - "**Requires Python 3.8+**"
     - "Migrated to Click library for generating the commandline interface"
```

### Comparing `twitch_dl-2.2.1/docs/changelog.md` & `twitch_dl-2.2.2/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 twitch-dl changelog
 ===================
 
 <!-- Do not edit. This file is automatically generated from changelog.yaml.-->
 
+### [2.2.2 (2024-04-23)](https://github.com/ihabunek/twitch-dl/releases/tag/2.2.2)
+
+* Fix more compat issues Python < 3.10 (#152)
+
 ### [2.2.1 (2024-04-23)](https://github.com/ihabunek/twitch-dl/releases/tag/2.2.1)
 
-* Fix compat with < Python 3.10 (#152)
+* Fix compat with Python < 3.10 (#152)
 * Fix division by zero in progress calculation when video duration is reported
   as 0
 
 ### [2.2.0 (2024-04-10)](https://github.com/ihabunek/twitch-dl/releases/tag/2.2.0)
 
 * **Requires Python 3.8+**
 * Migrated to Click library for generating the commandline interface
```

### Comparing `twitch_dl-2.2.1/docs/commands/auth_token.png` & `twitch_dl-2.2.2/docs/commands/auth_token.png`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/docs/commands/clips.md` & `twitch_dl-2.2.2/docs/commands/clips.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/docs/commands/download.md` & `twitch_dl-2.2.2/docs/commands/download.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/docs/commands/env.md` & `twitch_dl-2.2.2/docs/commands/env.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/docs/commands/info.md` & `twitch_dl-2.2.2/docs/commands/info.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/docs/commands/videos.md` & `twitch_dl-2.2.2/docs/commands/videos.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/docs/installation.md` & `twitch_dl-2.2.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/docs/introduction.md` & `twitch_dl-2.2.2/docs/introduction.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/docs/license.md` & `twitch_dl-2.2.2/docs/license.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/docs/shell_completion.md` & `twitch_dl-2.2.2/docs/shell_completion.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/docs/usage.md` & `twitch_dl-2.2.2/docs/usage.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/pyproject.toml` & `twitch_dl-2.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -49,11 +49,12 @@
 
 [project.scripts]
 twitch-dl = "twitchdl.cli:cli"
 
 [tool.pyright]
 include = ["twitchdl"]
 typeCheckingMode = "strict"
+pythonVersion = "3.8"
 
 [tool.ruff]
 line-length = 100
 target-version = "py38"
```

### Comparing `twitch_dl-2.2.1/scripts/generate_changelog` & `twitch_dl-2.2.2/scripts/generate_changelog`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/scripts/generate_docs` & `twitch_dl-2.2.2/scripts/generate_docs`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/scripts/tag_version` & `twitch_dl-2.2.2/scripts/tag_version`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/tests/test_api.py` & `twitch_dl-2.2.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/tests/test_patterns.py` & `twitch_dl-2.2.2/tests/test_patterns.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/tests/test_progress.py` & `twitch_dl-2.2.2/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/twitch-dl.1.scd` & `twitch_dl-2.2.2/twitch-dl.1.scd`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/twitch_dl.egg-info/PKG-INFO` & `twitch_dl-2.2.2/twitch_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-dl
-Version: 2.2.1
+Version: 2.2.2
 Summary: Quickly download videos from twitch.tv from the comort of your terminal emulator
 Author-email: Ivan Habunek <ivan@habunek.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `twitch_dl-2.2.1/twitch_dl.egg-info/SOURCES.txt` & `twitch_dl-2.2.2/twitch_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/twitchdl/cli.py` & `twitch_dl-2.2.2/twitchdl/cli.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/twitchdl/commands/clips.py` & `twitch_dl-2.2.2/twitchdl/commands/clips.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/twitchdl/commands/download.py` & `twitch_dl-2.2.2/twitchdl/commands/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import platform
 import re
 import shutil
 import subprocess
 import tempfile
 from os import path
 from pathlib import Path
+from typing import Dict, List
 from urllib.parse import urlencode, urlparse
 
 import click
 import httpx
 
 from twitchdl import twitch, utils
 from twitchdl.download import download_file
@@ -24,15 +25,15 @@
     make_join_playlist,
     parse_playlists,
     select_playlist,
 )
 from twitchdl.twitch import Chapter, Clip, ClipAccessToken, Video
 
 
-def download(ids: list[str], args: DownloadOptions):
+def download(ids: List[str], args: DownloadOptions):
     for video_id in ids:
         download_one(video_id, args)
 
 
 def download_one(video: str, args: DownloadOptions):
     video_id = utils.parse_video_identifier(video)
     if video_id:
@@ -74,25 +75,25 @@
 
     click.secho(f"{' '.join(command)}", dim=True)
     result = subprocess.run(command)
     if result.returncode != 0:
         raise ConsoleError("Joining files failed")
 
 
-def _concat_vods(vod_paths: list[str], target: str):
+def _concat_vods(vod_paths: List[str], target: str):
     tool = "type" if platform.system() == "Windows" else "cat"
     command = [tool] + vod_paths
 
     with open(target, "wb") as target_file:
         result = subprocess.run(command, stdout=target_file)
         if result.returncode != 0:
             raise ConsoleError(f"Joining files failed: {result.stderr}")
 
 
-def get_video_placeholders(video: Video, format: str) -> dict[str, str]:
+def get_video_placeholders(video: Video, format: str) -> Dict[str, str]:
     date, time = video["publishedAt"].split("T")
     game = video["game"]["name"] if video["game"] else "Unknown"
 
     return {
         "channel": video["creator"]["displayName"],
         "channel_login": video["creator"]["login"],
         "date": date,
@@ -346,15 +347,15 @@
         start = chapter["positionMilliseconds"] // 1000
         duration = chapter["durationMilliseconds"] // 1000
         return start, start + duration
 
     return None, None
 
 
-def _choose_chapter_interactive(chapters: list[Chapter]):
+def _choose_chapter_interactive(chapters: List[Chapter]):
     click.echo("\nChapters:")
     for index, chapter in enumerate(chapters):
         duration = utils.format_time(chapter["durationMilliseconds"] // 1000)
         click.echo(f'{index + 1}) {bold(chapter["description"])} ({duration})')
     index = utils.read_int("Select a chapter", 1, len(chapters))
     chapter = chapters[index - 1]
     return chapter
```

### Comparing `twitch_dl-2.2.1/twitchdl/commands/info.py` & `twitch_dl-2.2.2/twitchdl/commands/info.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import List
+
 import click
 import m3u8
 
 from twitchdl import twitch, utils
 from twitchdl.commands.download import get_video_placeholders
 from twitchdl.exceptions import ConsoleError
 from twitchdl.output import bold, print_clip, print_json, print_log, print_table, print_video
@@ -44,15 +46,15 @@
         else:
             clip_info(clip)
         return
 
     raise ConsoleError(f"Invalid input: {id}")
 
 
-def video_info(video: Video, playlists, chapters: list[Chapter]):
+def video_info(video: Video, playlists, chapters: List[Chapter]):
     click.echo()
     print_video(video)
 
     click.echo("Playlists:")
     for p in m3u8.loads(playlists).playlists:
         click.echo(f"{bold(p.stream_info.video)} {p.uri}")
```

### Comparing `twitch_dl-2.2.1/twitchdl/commands/videos.py` & `twitch_dl-2.2.2/twitchdl/commands/videos.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import sys
-from typing import Optional
+from typing import List, Optional
 
 import click
 
 from twitchdl import twitch
 from twitchdl.exceptions import ConsoleError
 from twitchdl.output import print_json, print_log, print_paged, print_video, print_video_compact
 
 
 def videos(
     channel_name: str,
     *,
     all: bool,
     compact: bool,
-    games: list[str],
+    games: List[str],
     json: bool,
     limit: Optional[int],
     pager: Optional[int],
     sort: twitch.VideosSort,
     type: twitch.VideosType,
 ):
     game_ids = _get_game_ids(games)
@@ -63,15 +63,15 @@
         click.secho(
             "\nThere are more videos. "
             + "Increase the --limit, use --all or --pager to see the rest.",
             dim=True,
         )
 
 
-def _get_game_ids(names: list[str]) -> list[str]:
+def _get_game_ids(names: List[str]) -> List[str]:
     if not names:
         return []
 
     game_ids = []
     for name in names:
         print_log(f"Looking up game '{name}'...")
         game_id = twitch.get_game_id(name)
```

### Comparing `twitch_dl-2.2.1/twitchdl/download.py` & `twitch_dl-2.2.2/twitchdl/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+
 import httpx
 
 from twitchdl.exceptions import ConsoleError
 
 CHUNK_SIZE = 1024
 CONNECT_TIMEOUT = 5
 RETRY_COUNT = 5
```

### Comparing `twitch_dl-2.2.1/twitchdl/http.py` & `twitch_dl-2.2.2/twitchdl/http.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/twitchdl/output.py` & `twitch_dl-2.2.2/twitchdl/output.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from itertools import islice
-from typing import Any, Callable, Generator, Optional, TypeVar
+from typing import Any, Callable, Generator, List, Optional, TypeVar
 
 import click
 
 from twitchdl import utils
 from twitchdl.twitch import Clip, Video
 
 T = TypeVar("T")
@@ -21,20 +21,20 @@
     click.echo(json.dumps(data))
 
 
 def print_log(message: Any):
     click.secho(message, err=True, dim=True)
 
 
-def print_table(headers: list[str], data: list[list[str]]):
+def print_table(headers: List[str], data: List[List[str]]):
     widths = [[len(cell) for cell in row] for row in data + [headers]]
     widths = [max(width) for width in zip(*widths)]
     underlines = ["-" * width for width in widths]
 
-    def print_row(row: list[str]):
+    def print_row(row: List[str]):
         for idx, cell in enumerate(row):
             width = widths[idx]
             click.echo(cell.ljust(width), nl=False)
             click.echo("  ", nl=False)
         click.echo()
 
     print_row(headers)
```

### Comparing `twitch_dl-2.2.1/twitchdl/playlists.py` & `twitch_dl-2.2.2/twitchdl/playlists.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Parse and manipulate m3u8 playlists.
 """
 
 from dataclasses import dataclass
-from typing import Generator, Optional, OrderedDict
+from typing import Generator, List, Optional, OrderedDict
 
 import click
 import m3u8
 
 from twitchdl import utils
 from twitchdl.output import bold, dim
 
@@ -51,15 +51,15 @@
     return m3u8.loads(playlist_m3u8)
 
 
 def enumerate_vods(
     document: m3u8.M3U8,
     start: Optional[int] = None,
     end: Optional[int] = None,
-) -> list[Vod]:
+) -> List[Vod]:
     """Extract VODs for download from document."""
     vods = []
     vod_start = 0
 
     for index, segment in enumerate(document.segments):
         vod_end = vod_start + segment.duration
 
@@ -74,16 +74,16 @@
         vod_start = vod_end
 
     return vods
 
 
 def make_join_playlist(
     playlist: m3u8.M3U8,
-    vods: list[Vod],
-    targets: list[str],
+    vods: List[Vod],
+    targets: List[str],
 ) -> m3u8.Playlist:
     """
     Make a modified playlist which references downloaded VODs
     Keep only the downloaded segments and skip the rest
     """
     org_segments = playlist.segments.copy()
 
@@ -93,36 +93,36 @@
         if segment.uri in path_map:
             segment.uri = path_map[segment.uri]
             playlist.segments.append(segment)
 
     return playlist
 
 
-def select_playlist(playlists: list[Playlist], quality: Optional[str]) -> Playlist:
+def select_playlist(playlists: List[Playlist], quality: Optional[str]) -> Playlist:
     return (
         select_playlist_by_name(playlists, quality)
         if quality is not None
         else select_playlist_interactive(playlists)
     )
 
 
-def select_playlist_by_name(playlists: list[Playlist], quality: str) -> Playlist:
+def select_playlist_by_name(playlists: List[Playlist], quality: str) -> Playlist:
     if quality == "source":
         return playlists[0]
 
     for playlist in playlists:
         if playlist.name == quality:
             return playlist
 
     available = ", ".join([p.name for p in playlists])
     msg = f"Quality '{quality}' not found. Available qualities are: {available}"
     raise click.ClickException(msg)
 
 
-def select_playlist_interactive(playlists: list[Playlist]) -> Playlist:
+def select_playlist_interactive(playlists: List[Playlist]) -> Playlist:
     click.echo("\nAvailable qualities:")
     for n, playlist in enumerate(playlists):
         if playlist.resolution:
             click.echo(f"{n + 1}) {bold(playlist.name)} {dim(f'({playlist.resolution})')}")
         else:
             click.echo(f"{n + 1}) {bold(playlist.name)}")
```

### Comparing `twitch_dl-2.2.1/twitchdl/progress.py` & `twitch_dl-2.2.2/twitchdl/progress.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.1/twitchdl/twitch.py` & `twitch_dl-2.2.2/twitchdl/twitch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Twitch API access.
 """
 
 import json
-from typing import Dict, Generator, Literal, TypedDict, Optional
+from typing import Dict, Generator, List, Literal, Mapping, Optional, TypedDict
 
 import click
 import httpx
 
 from twitchdl import CLIENT_ID
 from twitchdl.entities import Data
 from twitchdl.exceptions import ConsoleError
@@ -37,26 +37,26 @@
     quality: str
     sourceURL: str
 
 
 class ClipAccessToken(TypedDict):
     id: str
     playbackAccessToken: AccessToken
-    videoQualities: list[VideoQuality]
+    videoQualities: List[VideoQuality]
 
 
 class Clip(TypedDict):
     id: str
     slug: str
     title: str
     createdAt: str
     viewCount: int
     durationSeconds: int
     url: str
-    videoQualities: list[VideoQuality]
+    videoQualities: List[VideoQuality]
     game: Game
     broadcaster: User
 
 
 class Video(TypedDict):
     id: str
     title: str
@@ -76,15 +76,15 @@
     description: str
     subDescription: str
     thumbnailURL: str
     game: Game
 
 
 class GQLError(click.ClickException):
-    def __init__(self, errors: list[str]):
+    def __init__(self, errors: List[str]):
         message = "GraphQL query failed."
         for error in errors:
             message += f"\n* {error}"
         super().__init__(message)
 
 
 def authenticated_post(url, data=None, json=None, headers={}):
@@ -205,15 +205,20 @@
     }}
     """
 
     response = gql_post(query.strip())
     return response["data"]["clip"]
 
 
-def get_channel_clips(channel_id: str, period: ClipsPeriod, limit: int, after: Optional[str] = None):
+def get_channel_clips(
+    channel_id: str,
+    period: ClipsPeriod,
+    limit: int,
+    after: Optional[str] = None,
+):
     """
     List channel clips.
 
     At the time of writing this:
     * filtering by game name returns an error
     * sorting by anything but VIEWS_DESC or TRENDING returns an error
     * sorting by VIEWS_DESC and TRENDING returns the same results
@@ -290,15 +295,15 @@
 
 
 def get_channel_videos(
     channel_id: str,
     limit: int,
     sort: str,
     type: str = "archive",
-    game_ids: Optional[list[str]] = None,
+    game_ids: Optional[List[str]] = None,
     after: Optional[str] = None,
 ):
     game_ids = game_ids or []
 
     query = f"""
     {{
         user(login: "{channel_id}") {{
@@ -335,15 +340,15 @@
 
 
 def channel_videos_generator(
     channel_id: str,
     max_videos: int,
     sort: VideosSort,
     type: VideosType,
-    game_ids: Optional[list[str]] = None,
+    game_ids: Optional[List[str]] = None,
 ) -> tuple[int, Generator[Video, None, None]]:
     game_ids = game_ids or []
 
     def _generator(videos: Data, max_videos: int) -> Generator[Video, None, None]:
         for video in videos["edges"]:
             if max_videos < 1:
                 return
@@ -377,15 +382,15 @@
         ) {{
             signature
             value
         }}
     }}
     """
 
-    headers: dict[str, str] = {}
+    headers: Mapping[str, str] = {}
     if auth_token is not None:
         headers["authorization"] = f"OAuth {auth_token}"
 
     try:
         response = gql_query(query, headers=headers)
         return response["data"]["videoPlaybackAccessToken"]
     except httpx.HTTPStatusError as error:
@@ -434,15 +439,15 @@
 
     response = gql_query(query)
     game = response["data"]["game"]
     if game:
         return game["id"]
 
 
-def get_video_chapters(video_id: str) -> list[Chapter]:
+def get_video_chapters(video_id: str) -> List[Chapter]:
     query = {
         "operationName": "VideoPlayer_ChapterSelectButtonVideo",
         "variables": {
             "includePrivate": False,
             "videoID": video_id,
         },
         "extensions": {
```

### Comparing `twitch_dl-2.2.1/twitchdl/utils.py` & `twitch_dl-2.2.2/twitchdl/utils.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
-from typing import Optional, Union
 import unicodedata
+from typing import Optional, Union
 
 import click
 
 
 def _format_size(value: float, digits: int, unit: str):
     if digits > 0:
         return f"{{:.{digits}f}}{unit}".format(value)
```

