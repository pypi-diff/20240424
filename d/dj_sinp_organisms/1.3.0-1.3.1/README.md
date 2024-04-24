# Comparing `tmp/dj_sinp_organisms-1.3.0.tar.gz` & `tmp/dj_sinp_organisms-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_sinp_organisms-1.3.0.tar", max compression
+gzip compressed data, was "dj_sinp_organisms-1.3.1.tar", max compression
```

## Comparing `dj_sinp_organisms-1.3.0.tar` & `dj_sinp_organisms-1.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    34523 2024-04-22 13:44:29.156165 dj_sinp_organisms-1.3.0/LICENSE
--rw-r--r--   0        0        0     1266 2024-04-22 13:44:29.156165 dj_sinp_organisms-1.3.0/README.md
--rw-r--r--   0        0        0     1851 2024-04-22 13:44:29.156165 dj_sinp_organisms-1.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-22 13:44:29.156165 dj_sinp_organisms-1.3.0/sinp_organisms/__init__.py
--rw-r--r--   0        0        0     1164 2024-04-22 13:44:29.156165 dj_sinp_organisms-1.3.0/sinp_organisms/admin.py
--rw-r--r--   0        0        0      159 2024-04-22 13:44:29.156165 dj_sinp_organisms-1.3.0/sinp_organisms/apps.py
--rw-r--r--   0        0        0        0 2024-04-22 13:44:29.156165 dj_sinp_organisms-1.3.0/sinp_organisms/fixtures/.gitkeep
--rw-r--r--   0        0        0  4643951 2024-04-22 13:44:29.172165 dj_sinp_organisms-1.3.0/sinp_organisms/fixtures/inpn_organisms.json
--rw-r--r--   0        0        0    21517 2024-04-22 13:44:29.172165 dj_sinp_organisms-1.3.0/sinp_organisms/fixtures/nomenclatures.json
--rw-r--r--   0        0        0  7113254 2024-04-22 13:44:29.192165 dj_sinp_organisms-1.3.0/sinp_organisms/fixtures/test_data.json
--rw-r--r--   0        0        0      840 2024-04-22 13:44:29.192165 dj_sinp_organisms-1.3.0/sinp_organisms/managers.py
--rw-r--r--   0        0        0     9393 2024-04-22 13:44:29.192165 dj_sinp_organisms-1.3.0/sinp_organisms/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-22 13:44:29.192165 dj_sinp_organisms-1.3.0/sinp_organisms/migrations/__init__.py
--rw-r--r--   0        0        0     2241 2024-04-22 13:44:29.192165 dj_sinp_organisms-1.3.0/sinp_organisms/mixins.py
--rw-r--r--   0        0        0     5513 2024-04-22 13:44:29.192165 dj_sinp_organisms-1.3.0/sinp_organisms/models.py
--rw-r--r--   0        0        0     1308 2024-04-22 13:44:29.192165 dj_sinp_organisms-1.3.0/sinp_organisms/serializers.py
--rw-r--r--   0        0        0     2570 2024-04-22 13:44:29.192165 dj_sinp_organisms-1.3.0/sinp_organisms/tests.py
--rw-r--r--   0        0        0      376 2024-04-22 13:44:29.192165 dj_sinp_organisms-1.3.0/sinp_organisms/urls.py
--rw-r--r--   0        0        0      330 2024-04-22 13:44:29.192165 dj_sinp_organisms-1.3.0/sinp_organisms/validators.py
--rw-r--r--   0        0        0     1386 2024-04-22 13:44:29.192165 dj_sinp_organisms-1.3.0/sinp_organisms/views.py
--rw-r--r--   0        0        0     2180 1970-01-01 00:00:00.000000 dj_sinp_organisms-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-24 13:13:28.264237 dj_sinp_organisms-1.3.1/LICENSE
+-rw-r--r--   0        0        0     1266 2024-04-24 13:13:28.264237 dj_sinp_organisms-1.3.1/README.md
+-rw-r--r--   0        0        0     1851 2024-04-24 13:13:28.268237 dj_sinp_organisms-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 13:13:28.268237 dj_sinp_organisms-1.3.1/sinp_organisms/__init__.py
+-rw-r--r--   0        0        0     1164 2024-04-24 13:13:28.268237 dj_sinp_organisms-1.3.1/sinp_organisms/admin.py
+-rw-r--r--   0        0        0      159 2024-04-24 13:13:28.268237 dj_sinp_organisms-1.3.1/sinp_organisms/apps.py
+-rw-r--r--   0        0        0        0 2024-04-24 13:13:28.268237 dj_sinp_organisms-1.3.1/sinp_organisms/fixtures/.gitkeep
+-rw-r--r--   0        0        0  6612607 2024-04-24 13:13:28.284237 dj_sinp_organisms-1.3.1/sinp_organisms/fixtures/inpn_organisms.json
+-rw-r--r--   0        0        0    21517 2024-04-24 13:13:28.288237 dj_sinp_organisms-1.3.1/sinp_organisms/fixtures/nomenclatures.json
+-rw-r--r--   0        0        0  7113254 2024-04-24 13:13:28.304237 dj_sinp_organisms-1.3.1/sinp_organisms/fixtures/test_data.json
+-rw-r--r--   0        0        0      840 2024-04-24 13:13:28.304237 dj_sinp_organisms-1.3.1/sinp_organisms/managers.py
+-rw-r--r--   0        0        0     9393 2024-04-24 13:13:28.304237 dj_sinp_organisms-1.3.1/sinp_organisms/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-24 13:13:28.304237 dj_sinp_organisms-1.3.1/sinp_organisms/migrations/__init__.py
+-rw-r--r--   0        0        0     2241 2024-04-24 13:13:28.304237 dj_sinp_organisms-1.3.1/sinp_organisms/mixins.py
+-rw-r--r--   0        0        0     5513 2024-04-24 13:13:28.304237 dj_sinp_organisms-1.3.1/sinp_organisms/models.py
+-rw-r--r--   0        0        0     1308 2024-04-24 13:13:28.304237 dj_sinp_organisms-1.3.1/sinp_organisms/serializers.py
+-rw-r--r--   0        0        0     2570 2024-04-24 13:13:28.304237 dj_sinp_organisms-1.3.1/sinp_organisms/tests.py
+-rw-r--r--   0        0        0      376 2024-04-24 13:13:28.304237 dj_sinp_organisms-1.3.1/sinp_organisms/urls.py
+-rw-r--r--   0        0        0      330 2024-04-24 13:13:28.308237 dj_sinp_organisms-1.3.1/sinp_organisms/validators.py
+-rw-r--r--   0        0        0     1386 2024-04-24 13:13:28.308237 dj_sinp_organisms-1.3.1/sinp_organisms/views.py
+-rw-r--r--   0        0        0     2180 1970-01-01 00:00:00.000000 dj_sinp_organisms-1.3.1/PKG-INFO
```

### Comparing `dj_sinp_organisms-1.3.0/LICENSE` & `dj_sinp_organisms-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.3.0/README.md` & `dj_sinp_organisms-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.3.0/pyproject.toml` & `dj_sinp_organisms-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dj_sinp_organisms"
-version = "1.3.0"
+version = "1.3.1"
 description = "Django app to manage french SINP organisms standard"
 authors = ["dbChiro project", "hypsug0"]
 license = "AGPLv3"
 keywords = ["SINP", "Nomenclatures", "Django", "France", "dbChiroWeb"]
 readme = "README.md"
 homepage = "https://github.com/dbchiro/DjangoSinpOrganisms"
 repository = "https://github.com/dbchiro/DjangoSinpOrganisms"
```

### Comparing `dj_sinp_organisms-1.3.0/sinp_organisms/admin.py` & `dj_sinp_organisms-1.3.1/sinp_organisms/admin.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.3.0/sinp_organisms/fixtures/nomenclatures.json` & `dj_sinp_organisms-1.3.1/sinp_organisms/fixtures/nomenclatures.json`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.3.0/sinp_organisms/fixtures/test_data.json` & `dj_sinp_organisms-1.3.1/sinp_organisms/fixtures/test_data.json`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.3.0/sinp_organisms/managers.py` & `dj_sinp_organisms-1.3.1/sinp_organisms/managers.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.3.0/sinp_organisms/migrations/0001_initial.py` & `dj_sinp_organisms-1.3.1/sinp_organisms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.3.0/sinp_organisms/mixins.py` & `dj_sinp_organisms-1.3.1/sinp_organisms/mixins.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.3.0/sinp_organisms/models.py` & `dj_sinp_organisms-1.3.1/sinp_organisms/models.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.3.0/sinp_organisms/serializers.py` & `dj_sinp_organisms-1.3.1/sinp_organisms/serializers.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.3.0/sinp_organisms/tests.py` & `dj_sinp_organisms-1.3.1/sinp_organisms/tests.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.3.0/sinp_organisms/views.py` & `dj_sinp_organisms-1.3.1/sinp_organisms/views.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.3.0/PKG-INFO` & `dj_sinp_organisms-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj_sinp_organisms
-Version: 1.3.0
+Version: 1.3.1
 Summary: Django app to manage french SINP organisms standard
 Home-page: https://github.com/dbchiro/DjangoSinpOrganisms
 License: AGPLv3
 Keywords: SINP,Nomenclatures,Django,France,dbChiroWeb
 Author: dbChiro project
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: Other/Proprietary License
```

