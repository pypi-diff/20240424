# Comparing `tmp/fourmat-0.9.0.tar.gz` & `tmp/fourmat-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fourmat-0.9.0.tar", last modified: Thu Jul  8 13:42:13 2021, max compression
+gzip compressed data, was "fourmat-1.0.0.tar", last modified: Wed Apr 24 17:03:42 2024, max compression
```

## Comparing `fourmat-0.9.0.tar` & `fourmat-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 gtagliabue   (501) staff       (20)        0 2021-07-08 13:42:13.204917 fourmat-0.9.0/
--rw-r--r--   0 gtagliabue   (501) staff       (20)     1782 2021-07-08 13:42:13.205188 fourmat-0.9.0/PKG-INFO
--rw-r--r--   0 gtagliabue   (501) staff       (20)      619 2019-05-13 20:03:10.000000 fourmat-0.9.0/README.md
-drwxr-xr-x   0 gtagliabue   (501) staff       (20)        0 2021-07-08 13:42:13.199128 fourmat-0.9.0/fourmat/
--rw-r--r--   0 gtagliabue   (501) staff       (20)      732 2021-07-01 20:46:55.000000 fourmat-0.9.0/fourmat/__init__.py
-drwxr-xr-x   0 gtagliabue   (501) staff       (20)        0 2021-07-08 13:42:13.204320 fourmat-0.9.0/fourmat/assets/
--rw-r--r--   0 gtagliabue   (501) staff       (20)      148 2018-11-28 19:06:34.000000 fourmat-0.9.0/fourmat/assets/.flake8
--rw-r--r--   0 gtagliabue   (501) staff       (20)      165 2021-07-02 14:47:22.000000 fourmat-0.9.0/fourmat/assets/pyproject.toml
--rw-r--r--   0 gtagliabue   (501) staff       (20)     3377 2021-07-08 13:39:02.000000 fourmat-0.9.0/fourmat/lint.py
-drwxr-xr-x   0 gtagliabue   (501) staff       (20)        0 2021-07-08 13:42:13.202780 fourmat-0.9.0/fourmat.egg-info/
--rw-r--r--   0 gtagliabue   (501) staff       (20)     1782 2021-07-08 13:42:13.000000 fourmat-0.9.0/fourmat.egg-info/PKG-INFO
--rw-r--r--   0 gtagliabue   (501) staff       (20)      320 2021-07-08 13:42:13.000000 fourmat-0.9.0/fourmat.egg-info/SOURCES.txt
--rw-r--r--   0 gtagliabue   (501) staff       (20)        1 2021-07-08 13:42:13.000000 fourmat-0.9.0/fourmat.egg-info/dependency_links.txt
--rw-r--r--   0 gtagliabue   (501) staff       (20)       41 2021-07-08 13:42:13.000000 fourmat-0.9.0/fourmat.egg-info/entry_points.txt
--rw-r--r--   0 gtagliabue   (501) staff       (20)       71 2021-07-08 13:42:13.000000 fourmat-0.9.0/fourmat.egg-info/requires.txt
--rw-r--r--   0 gtagliabue   (501) staff       (20)        8 2021-07-08 13:42:13.000000 fourmat-0.9.0/fourmat.egg-info/top_level.txt
--rw-r--r--   0 gtagliabue   (501) staff       (20)      165 2021-07-02 14:47:22.000000 fourmat-0.9.0/pyproject.toml
--rw-r--r--   0 gtagliabue   (501) staff       (20)      131 2021-07-08 13:42:13.205976 fourmat-0.9.0/setup.cfg
--rw-r--r--   0 gtagliabue   (501) staff       (20)     1158 2021-07-08 13:39:58.000000 fourmat-0.9.0/setup.py
+drwxr-xr-x   0 sliu       (501) staff       (20)        0 2024-04-24 17:03:42.112369 fourmat-1.0.0/
+-rw-r--r--   0 sliu       (501) staff       (20)     1078 2022-01-15 20:53:01.000000 fourmat-1.0.0/LICENSE
+-rw-r--r--   0 sliu       (501) staff       (20)     1676 2024-04-24 17:03:42.112248 fourmat-1.0.0/PKG-INFO
+-rw-r--r--   0 sliu       (501) staff       (20)      619 2022-01-15 20:53:01.000000 fourmat-1.0.0/README.md
+drwxr-xr-x   0 sliu       (501) staff       (20)        0 2024-04-24 17:03:42.109039 fourmat-1.0.0/fourmat/
+-rw-r--r--   0 sliu       (501) staff       (20)      732 2022-01-15 20:53:01.000000 fourmat-1.0.0/fourmat/__init__.py
+drwxr-xr-x   0 sliu       (501) staff       (20)        0 2024-04-24 17:03:42.110897 fourmat-1.0.0/fourmat/assets/
+-rw-r--r--   0 sliu       (501) staff       (20)      148 2022-01-15 20:53:01.000000 fourmat-1.0.0/fourmat/assets/.flake8
+-rw-r--r--   0 sliu       (501) staff       (20)      182 2022-01-15 20:53:01.000000 fourmat-1.0.0/fourmat/assets/pyproject.toml
+-rw-r--r--   0 sliu       (501) staff       (20)     5342 2022-01-15 20:53:01.000000 fourmat-1.0.0/fourmat/lint.py
+drwxr-xr-x   0 sliu       (501) staff       (20)        0 2024-04-24 17:03:42.111465 fourmat-1.0.0/fourmat.egg-info/
+-rw-r--r--   0 sliu       (501) staff       (20)     1676 2024-04-24 17:03:42.000000 fourmat-1.0.0/fourmat.egg-info/PKG-INFO
+-rw-r--r--   0 sliu       (501) staff       (20)      349 2024-04-24 17:03:42.000000 fourmat-1.0.0/fourmat.egg-info/SOURCES.txt
+-rw-r--r--   0 sliu       (501) staff       (20)        1 2024-04-24 17:03:42.000000 fourmat-1.0.0/fourmat.egg-info/dependency_links.txt
+-rw-r--r--   0 sliu       (501) staff       (20)       40 2024-04-24 17:03:42.000000 fourmat-1.0.0/fourmat.egg-info/entry_points.txt
+-rw-r--r--   0 sliu       (501) staff       (20)       71 2024-04-24 17:03:42.000000 fourmat-1.0.0/fourmat.egg-info/requires.txt
+-rw-r--r--   0 sliu       (501) staff       (20)        8 2024-04-24 17:03:42.000000 fourmat-1.0.0/fourmat.egg-info/top_level.txt
+-rw-r--r--   0 sliu       (501) staff       (20)      176 2024-04-24 16:16:52.000000 fourmat-1.0.0/pyproject.toml
+-rw-r--r--   0 sliu       (501) staff       (20)      131 2024-04-24 17:03:42.112669 fourmat-1.0.0/setup.cfg
+-rw-r--r--   0 sliu       (501) staff       (20)     1257 2024-04-24 16:41:25.000000 fourmat-1.0.0/setup.py
+drwxr-xr-x   0 sliu       (501) staff       (20)        0 2024-04-24 17:03:42.111081 fourmat-1.0.0/test/
+-rw-r--r--   0 sliu       (501) staff       (20)     1140 2022-01-15 20:53:01.000000 fourmat-1.0.0/test/test_project.py
```

### Comparing `fourmat-0.9.0/README.md` & `fourmat-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `fourmat-0.9.0/fourmat/__init__.py` & `fourmat-1.0.0/fourmat/__init__.py`

 * *Files identical despite different names*

### Comparing `fourmat-0.9.0/setup.py` & `fourmat-1.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="fourmat",
-    version="0.9.0",
+    version="1.0.0",
     description="A library for batteries-included linting and autoformatting",
     url="https://github.com/4Catalyzer/fourmat",
     author="Giacomo Tagliabue",
     author_email="giacomo@gmail.com",
     license="MIT",
     python_requires=">=3.6",
     classifiers=[
@@ -14,21 +14,23 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
     ],
     keywords="lint autoformat black flake8 isort",
     packages=find_packages(),
     package_data={"fourmat": ("assets/*.*", "assets/.*")},
     install_requires=(
-        "click>=7",
-        "black==21.6b0",
-        "flake8-bugbear>=21,<22",
-        "flake8>=3,<4",
+        "click>=8",
+        "black==24.3.0",
+        "flake8-bugbear>=24,<25",
+        "flake8>=7,<8",
         "isort>=5,<6",
     ),
     entry_points={"console_scripts": ("fourmat = fourmat:cli",)},
 )
```

