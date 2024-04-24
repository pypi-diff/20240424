# Comparing `tmp/wecom_worktool-0.0.2.tar.gz` & `tmp/wecom_worktool-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wecom_worktool-0.0.2.tar", last modified: Tue Feb 27 01:52:04 2024, max compression
+gzip compressed data, was "wecom_worktool-0.0.3.tar", last modified: Wed Apr 24 15:49:42 2024, max compression
```

## Comparing `wecom_worktool-0.0.2.tar` & `wecom_worktool-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-02-27 01:52:06.910045 wecom_worktool-0.0.2/
--rw-rw-rw-   0        0        0      789 2024-02-27 01:52:06.907986 wecom_worktool-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      560 2024-02-27 00:43:29.000000 wecom_worktool-0.0.2/README.md
--rw-rw-rw-   0        0        0      524 2024-02-27 01:51:53.000000 wecom_worktool-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-27 01:52:06.912424 wecom_worktool-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-27 01:52:06.879568 wecom_worktool-0.0.2/wecom_worktool.egg-info/
--rw-rw-rw-   0        0        0      789 2024-02-27 01:52:06.000000 wecom_worktool-0.0.2/wecom_worktool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2024-02-27 01:52:06.000000 wecom_worktool-0.0.2/wecom_worktool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-27 01:52:06.000000 wecom_worktool-0.0.2/wecom_worktool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-02-27 01:52:06.000000 wecom_worktool-0.0.2/wecom_worktool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-27 01:52:06.000000 wecom_worktool-0.0.2/wecom_worktool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1624 2024-02-27 01:50:41.000000 wecom_worktool-0.0.2/worktool.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:49:42.672603 wecom_worktool-0.0.3/
+-rw-rw-rw-   0        0        0     1080 2024-04-24 15:49:42.671604 wecom_worktool-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      851 2024-02-29 11:23:57.000000 wecom_worktool-0.0.3/README.md
+-rw-rw-rw-   0        0        0      568 2024-04-24 15:49:34.000000 wecom_worktool-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-24 15:49:42.672603 wecom_worktool-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 15:49:42.671604 wecom_worktool-0.0.3/wecom_worktool.egg-info/
+-rw-rw-rw-   0        0        0     1080 2024-04-24 15:49:42.000000 wecom_worktool-0.0.3/wecom_worktool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-04-24 15:49:42.000000 wecom_worktool-0.0.3/wecom_worktool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 15:49:42.000000 wecom_worktool-0.0.3/wecom_worktool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-24 15:49:42.000000 wecom_worktool-0.0.3/wecom_worktool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-24 15:49:42.000000 wecom_worktool-0.0.3/wecom_worktool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3140 2024-04-24 15:48:08.000000 wecom_worktool-0.0.3/worktool.py
```

### Comparing `wecom_worktool-0.0.2/pyproject.toml` & `wecom_worktool-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "wecom_worktool"
-version = "0.0.2"
+version = "0.0.3"
 description = "企业微信WorkTool机器人API的封装。"
 readme = "README.md"
 authors = [
     {name = "sqkkyzx", email = "admin@sqkkyzx.com"},
 ]
 
 dependencies = ["requests"]
@@ -15,9 +15,10 @@
 [tool.poetry.dependencies]
 python = "^3.12"
 
 [tool.poetry.publish]
 repository = "pypi"
 
 [tool.poetry.changelog]
+"0.0.3" = "封装了群管理相关接口"
 "0.0.2" = "FIX: 修正了文件类型错误"
 "0.0.1" = "封装了发送文件和发送文本的两个接口"
```

