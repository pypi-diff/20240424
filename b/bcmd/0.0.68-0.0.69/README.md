# Comparing `tmp/bcmd-0.0.68.tar.gz` & `tmp/bcmd-0.0.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcmd-0.0.68.tar", last modified: Wed Mar 27 02:09:18 2024, max compression
+gzip compressed data, was "bcmd-0.0.69.tar", last modified: Tue Apr 23 08:39:40 2024, max compression
```

## Comparing `bcmd-0.0.68.tar` & `bcmd-0.0.69.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 02:09:18.737811 bcmd-0.0.68/
--rw-rw-rw-   0        0        0       29 2023-09-28 02:51:40.000000 bcmd-0.0.68/MANIFEST.in
--rw-rw-rw-   0        0        0      285 2024-03-27 02:09:18.736812 bcmd-0.0.68/PKG-INFO
--rw-rw-rw-   0        0        0       17 2023-08-28 06:50:10.000000 bcmd-0.0.68/README.md
-drwxrwxrwx   0        0        0        0 2024-03-27 02:09:18.710962 bcmd-0.0.68/bcmd/
--rw-rw-rw-   0        0        0        0 2023-08-28 06:50:11.000000 bcmd-0.0.68/bcmd/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 02:09:18.718184 bcmd-0.0.68/bcmd/common/
--rw-rw-rw-   0        0        0        0 2023-10-10 06:24:00.000000 bcmd-0.0.68/bcmd/common/__init__.py
--rw-rw-rw-   0        0        0     1347 2024-02-28 09:10:56.000000 bcmd-0.0.68/bcmd/common/password.py
--rw-rw-rw-   0        0        0      132 2024-02-19 06:30:11.000000 bcmd-0.0.68/bcmd/main.py
-drwxrwxrwx   0        0        0        0 2024-03-27 02:09:18.734292 bcmd-0.0.68/bcmd/tasks/
--rw-rw-rw-   0        0        0      311 2024-03-27 02:04:27.000000 bcmd-0.0.68/bcmd/tasks/__init__.py
--rw-rw-rw-   0        0        0     3082 2023-10-11 06:16:53.000000 bcmd-0.0.68/bcmd/tasks/bin.py
--rw-rw-rw-   0        0        0     3127 2024-02-28 09:11:35.000000 bcmd-0.0.68/bcmd/tasks/crypto.py
--rw-rw-rw-   0        0        0     3004 2024-03-04 08:51:50.000000 bcmd-0.0.68/bcmd/tasks/debian.py
--rw-rw-rw-   0        0        0     1052 2024-01-24 02:30:52.000000 bcmd-0.0.68/bcmd/tasks/download.py
--rw-rw-rw-   0        0        0      635 2023-09-18 08:06:47.000000 bcmd-0.0.68/bcmd/tasks/json.py
--rw-rw-rw-   0        0        0     2407 2024-02-19 03:06:05.000000 bcmd-0.0.68/bcmd/tasks/jwt.py
--rw-rw-rw-   0        0        0     4528 2024-03-27 01:51:35.000000 bcmd-0.0.68/bcmd/tasks/lib.py
--rw-rw-rw-   0        0        0     4302 2023-09-18 08:06:47.000000 bcmd-0.0.68/bcmd/tasks/math.py
--rw-rw-rw-   0        0        0     1448 2023-09-18 08:06:47.000000 bcmd-0.0.68/bcmd/tasks/mirror.py
--rw-rw-rw-   0        0        0      939 2024-03-27 02:03:22.000000 bcmd-0.0.68/bcmd/tasks/project.py
--rw-rw-rw-   0        0        0      660 2023-09-18 08:06:47.000000 bcmd-0.0.68/bcmd/tasks/proxy.py
--rw-rw-rw-   0        0        0     4738 2024-03-27 02:07:27.000000 bcmd-0.0.68/bcmd/tasks/task.py
--rw-rw-rw-   0        0        0      766 2024-01-24 01:21:39.000000 bcmd-0.0.68/bcmd/tasks/temp.py
--rw-rw-rw-   0        0        0     2586 2023-09-18 08:06:47.000000 bcmd-0.0.68/bcmd/tasks/time.py
--rw-rw-rw-   0        0        0     4127 2024-02-02 07:36:25.000000 bcmd-0.0.68/bcmd/tasks/venv.py
-drwxrwxrwx   0        0        0        0 2024-03-27 02:09:18.735805 bcmd-0.0.68/bcmd.egg-info/
--rw-rw-rw-   0        0        0      285 2024-03-27 02:09:18.000000 bcmd-0.0.68/bcmd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      603 2024-03-27 02:09:18.000000 bcmd-0.0.68/bcmd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 02:09:18.000000 bcmd-0.0.68/bcmd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-03-27 02:09:18.000000 bcmd-0.0.68/bcmd.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-03-27 02:09:18.000000 bcmd-0.0.68/bcmd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-03-27 02:09:18.000000 bcmd-0.0.68/bcmd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      529 2024-03-27 02:08:33.000000 bcmd-0.0.68/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-27 02:09:18.737811 bcmd-0.0.68/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-23 08:39:40.177699 bcmd-0.0.69/
+-rw-rw-rw-   0        0        0       29 2023-09-28 02:51:40.000000 bcmd-0.0.69/MANIFEST.in
+-rw-rw-rw-   0        0        0      285 2024-04-23 08:39:40.176697 bcmd-0.0.69/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2023-08-28 06:50:10.000000 bcmd-0.0.69/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 08:39:40.152903 bcmd-0.0.69/bcmd/
+-rw-rw-rw-   0        0        0        0 2023-08-28 06:50:11.000000 bcmd-0.0.69/bcmd/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:39:40.158909 bcmd-0.0.69/bcmd/common/
+-rw-rw-rw-   0        0        0        0 2023-10-10 06:24:00.000000 bcmd-0.0.69/bcmd/common/__init__.py
+-rw-rw-rw-   0        0        0     1347 2024-02-28 09:10:56.000000 bcmd-0.0.69/bcmd/common/password.py
+-rw-rw-rw-   0        0        0      131 2024-04-23 08:32:30.000000 bcmd-0.0.69/bcmd/main.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:39:40.174698 bcmd-0.0.69/bcmd/tasks/
+-rw-rw-rw-   0        0        0      311 2024-03-27 02:11:31.000000 bcmd-0.0.69/bcmd/tasks/__init__.py
+-rw-rw-rw-   0        0        0     3082 2023-10-11 06:16:53.000000 bcmd-0.0.69/bcmd/tasks/bin.py
+-rw-rw-rw-   0        0        0     3127 2024-02-28 09:11:35.000000 bcmd-0.0.69/bcmd/tasks/crypto.py
+-rw-rw-rw-   0        0        0     3004 2024-03-04 08:51:50.000000 bcmd-0.0.69/bcmd/tasks/debian.py
+-rw-rw-rw-   0        0        0     1052 2024-01-24 02:30:52.000000 bcmd-0.0.69/bcmd/tasks/download.py
+-rw-rw-rw-   0        0        0      635 2023-09-18 08:06:47.000000 bcmd-0.0.69/bcmd/tasks/json.py
+-rw-rw-rw-   0        0        0     2407 2024-02-19 03:06:05.000000 bcmd-0.0.69/bcmd/tasks/jwt.py
+-rw-rw-rw-   0        0        0     4528 2024-03-27 02:16:57.000000 bcmd-0.0.69/bcmd/tasks/lib.py
+-rw-rw-rw-   0        0        0     4302 2023-09-18 08:06:47.000000 bcmd-0.0.69/bcmd/tasks/math.py
+-rw-rw-rw-   0        0        0     1448 2023-09-18 08:06:47.000000 bcmd-0.0.69/bcmd/tasks/mirror.py
+-rw-rw-rw-   0        0        0      939 2024-03-27 02:03:22.000000 bcmd-0.0.69/bcmd/tasks/project.py
+-rw-rw-rw-   0        0        0      660 2023-09-18 08:06:47.000000 bcmd-0.0.69/bcmd/tasks/proxy.py
+-rw-rw-rw-   0        0        0     4738 2024-03-27 02:07:27.000000 bcmd-0.0.69/bcmd/tasks/task.py
+-rw-rw-rw-   0        0        0      766 2024-01-24 01:21:39.000000 bcmd-0.0.69/bcmd/tasks/temp.py
+-rw-rw-rw-   0        0        0     2586 2023-09-18 08:06:47.000000 bcmd-0.0.69/bcmd/tasks/time.py
+-rw-rw-rw-   0        0        0     4127 2024-04-07 07:18:21.000000 bcmd-0.0.69/bcmd/tasks/venv.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:39:40.175700 bcmd-0.0.69/bcmd.egg-info/
+-rw-rw-rw-   0        0        0      285 2024-04-23 08:39:40.000000 bcmd-0.0.69/bcmd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      603 2024-04-23 08:39:40.000000 bcmd-0.0.69/bcmd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 08:39:40.000000 bcmd-0.0.69/bcmd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-23 08:39:40.000000 bcmd-0.0.69/bcmd.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2024-04-23 08:39:40.000000 bcmd-0.0.69/bcmd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-23 08:39:40.000000 bcmd-0.0.69/bcmd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      529 2024-04-23 08:38:55.000000 bcmd-0.0.69/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 08:39:40.177699 bcmd-0.0.69/setup.cfg
```

### Comparing `bcmd-0.0.68/bcmd/common/password.py` & `bcmd-0.0.69/bcmd/common/password.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.68/bcmd/tasks/bin.py` & `bcmd-0.0.69/bcmd/tasks/bin.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.68/bcmd/tasks/crypto.py` & `bcmd-0.0.69/bcmd/tasks/crypto.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.68/bcmd/tasks/debian.py` & `bcmd-0.0.69/bcmd/tasks/debian.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.68/bcmd/tasks/download.py` & `bcmd-0.0.69/bcmd/tasks/download.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.68/bcmd/tasks/json.py` & `bcmd-0.0.69/bcmd/tasks/json.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.68/bcmd/tasks/jwt.py` & `bcmd-0.0.69/bcmd/tasks/jwt.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.68/bcmd/tasks/lib.py` & `bcmd-0.0.69/bcmd/tasks/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 @app.command()
 @syncCall
 async def version(
     workspace_path: Path = typer.Argument(None, help='workspace 路径'),
     disabled_commit: bool = typer.Option(False, '--disabled-commit', '-d', help='是否提交git'),
     tidy_dependencies: bool = typer.Option(False, '--tidy-dependencies', help='是否整理依赖'),
-    with_dependencies_version: bool = typer.Option(False, '--with_dependencies_version', help='第三方库是否带版本号')
+    with_dependencies_version: bool = typer.Option(False, '--with-dependencies-version', help='第三方库是否带版本号')
 ):
     '修改 pyproject.toml 版本号（同时会更新依赖列表）'
     if not workspace_path:
         workspace_path = Path.cwd()
     file = workspace_path / 'pyproject.toml'
     btask.check(file.is_file(), '文件不存在', file)
     if tidy_dependencies:
```

### Comparing `bcmd-0.0.68/bcmd/tasks/math.py` & `bcmd-0.0.69/bcmd/tasks/math.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.68/bcmd/tasks/mirror.py` & `bcmd-0.0.69/bcmd/tasks/mirror.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.68/bcmd/tasks/project.py` & `bcmd-0.0.69/bcmd/tasks/project.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.68/bcmd/tasks/proxy.py` & `bcmd-0.0.69/bcmd/tasks/proxy.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.68/bcmd/tasks/task.py` & `bcmd-0.0.69/bcmd/tasks/task.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.68/bcmd/tasks/temp.py` & `bcmd-0.0.69/bcmd/tasks/temp.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.68/bcmd/tasks/time.py` & `bcmd-0.0.69/bcmd/tasks/time.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.68/bcmd/tasks/venv.py` & `bcmd-0.0.69/bcmd/tasks/venv.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.68/bcmd.egg-info/SOURCES.txt` & `bcmd-0.0.69/bcmd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.68/pyproject.toml` & `bcmd-0.0.69/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # https://peps.python.org/pep-0621/#example
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/#declaring-project-metadata
 
 [project]
 name = 'bcmd'
-version = '0.0.68'
+version = '0.0.69'
 description = 'Commands for Beni'
 requires-python = '>=3.10'
 keywords = ['benimang', 'beni', 'bcmd']
 authors = [{ name = 'Beni Mang', email = 'benimang@126.com' }]
 maintainers = [{ name = 'Beni Mang', email = 'benimang@126.com' }]
 
 
 dependencies = [
-  'benimang==0.5.23',
+  'benimang==0.5.25',
   'pathspec',
 ]
 
 [project.scripts]
 beni = 'bcmd.main:run'
```

