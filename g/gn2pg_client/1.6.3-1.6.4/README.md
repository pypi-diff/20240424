# Comparing `tmp/gn2pg_client-1.6.3.tar.gz` & `tmp/gn2pg_client-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gn2pg_client-1.6.3.tar", max compression
+gzip compressed data, was "gn2pg_client-1.6.4.tar", max compression
```

## Comparing `gn2pg_client-1.6.3.tar` & `gn2pg_client-1.6.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    34523 2024-04-11 09:32:30.355228 gn2pg_client-1.6.3/LICENSE
--rw-r--r--   0        0        0     6629 2024-04-11 09:32:30.355228 gn2pg_client-1.6.3/README.md
--rw-r--r--   0        0        0     1059 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/__init__.py
--rw-r--r--   0        0        0     7245 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/api.py
--rw-r--r--   0        0        0        0 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/app/__init__.py
--rw-r--r--   0        0        0     1041 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/app/admin_views.py
--rw-r--r--   0        0        0     1391 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/app/app.py
--rw-r--r--   0        0        0     1943 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/app/config.py
--rw-r--r--   0        0        0      456 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/app/database.py
--rw-r--r--   0        0        0      241 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/app/env.py
--rw-r--r--   0        0        0      202 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/app/index.py
--rw-r--r--   0        0        0     1954 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/app/models.py
--rw-r--r--   0        0        0      216 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/app/static/css/custom_flaks_admin.css
--rw-r--r--   0        0        0    30240 2024-04-11 09:32:30.359228 gn2pg_client-1.6.3/gn2pg/app/static/img/src_gn2pg.png
--rw-r--r--   0        0        0      186 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/app/templates/admin/master.html
--rw-r--r--   0        0        0      353 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/app/templates/index.html
--rw-r--r--   0        0        0        0 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/app/utils/__init__.py
--rw-r--r--   0        0        0      582 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/app/utils/admin_views.py
--rw-r--r--   0        0        0    11145 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/check_conf.py
--rw-r--r--   0        0        0     1835 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/data/gn2pgconfig.toml
--rw-r--r--   0        0        0    46535 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/data/to_gnsynthese.sql
--rw-r--r--   0        0        0     8840 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/download.py
--rw-r--r--   0        0        0      241 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/env.py
--rw-r--r--   0        0        0     3968 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/helpers.py
--rw-r--r--   0        0        0     4100 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/locale/en_US/LC_MESAGES/gn2pg.po
--rw-r--r--   0        0        0    10575 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po
--rw-r--r--   0        0        0    10307 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po~
--rwxr-xr-x   0        0        0     6063 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/main.py
--rw-r--r--   0        0        0      765 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/metadata.py
--rw-r--r--   0        0        0    20657 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/store_postgresql.py
--rw-r--r--   0        0        0     1411 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/gn2pg/utils.py
--rw-r--r--   0        0        0     3133 2024-04-11 09:32:30.363227 gn2pg_client-1.6.3/pyproject.toml
--rw-r--r--   0        0        0     8665 1970-01-01 00:00:00.000000 gn2pg_client-1.6.3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-24 14:33:33.759258 gn2pg_client-1.6.4/LICENSE
+-rw-r--r--   0        0        0     6629 2024-04-24 14:33:33.759258 gn2pg_client-1.6.4/README.md
+-rw-r--r--   0        0        0     1059 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/__init__.py
+-rw-r--r--   0        0        0     7245 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/api.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/app/__init__.py
+-rw-r--r--   0        0        0     1041 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/app/admin_views.py
+-rw-r--r--   0        0        0     1391 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/app/app.py
+-rw-r--r--   0        0        0     1943 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/app/config.py
+-rw-r--r--   0        0        0      456 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/app/database.py
+-rw-r--r--   0        0        0      241 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/app/env.py
+-rw-r--r--   0        0        0      202 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/app/index.py
+-rw-r--r--   0        0        0     1954 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/app/models.py
+-rw-r--r--   0        0        0      216 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/app/static/css/custom_flaks_admin.css
+-rw-r--r--   0        0        0    30240 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/app/static/img/src_gn2pg.png
+-rw-r--r--   0        0        0      186 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/app/templates/admin/master.html
+-rw-r--r--   0        0        0      353 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/app/templates/index.html
+-rw-r--r--   0        0        0        0 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/app/utils/__init__.py
+-rw-r--r--   0        0        0      582 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/app/utils/admin_views.py
+-rw-r--r--   0        0        0    11145 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/check_conf.py
+-rw-r--r--   0        0        0     1835 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/data/gn2pgconfig.toml
+-rw-r--r--   0        0        0    46536 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/data/to_gnsynthese.sql
+-rw-r--r--   0        0        0     8840 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/download.py
+-rw-r--r--   0        0        0      241 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/env.py
+-rw-r--r--   0        0        0     3968 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/helpers.py
+-rw-r--r--   0        0        0     4100 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/locale/en_US/LC_MESAGES/gn2pg.po
+-rw-r--r--   0        0        0    10575 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po
+-rw-r--r--   0        0        0    10307 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po~
+-rwxr-xr-x   0        0        0     6063 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/main.py
+-rw-r--r--   0        0        0      765 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/metadata.py
+-rw-r--r--   0        0        0    20657 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/store_postgresql.py
+-rw-r--r--   0        0        0     1411 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/gn2pg/utils.py
+-rw-r--r--   0        0        0     3133 2024-04-24 14:33:33.767258 gn2pg_client-1.6.4/pyproject.toml
+-rw-r--r--   0        0        0     8665 1970-01-01 00:00:00.000000 gn2pg_client-1.6.4/PKG-INFO
```

### Comparing `gn2pg_client-1.6.3/LICENSE` & `gn2pg_client-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.3/README.md` & `gn2pg_client-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.3/gn2pg/__init__.py` & `gn2pg_client-1.6.4/gn2pg/__init__.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.3/gn2pg/api.py` & `gn2pg_client-1.6.4/gn2pg/api.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.3/gn2pg/app/admin_views.py` & `gn2pg_client-1.6.4/gn2pg/app/admin_views.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.3/gn2pg/app/app.py` & `gn2pg_client-1.6.4/gn2pg/app/app.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.3/gn2pg/app/config.py` & `gn2pg_client-1.6.4/gn2pg/app/config.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.3/gn2pg/app/models.py` & `gn2pg_client-1.6.4/gn2pg/app/models.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.3/gn2pg/app/static/img/src_gn2pg.png` & `gn2pg_client-1.6.4/gn2pg/app/static/img/src_gn2pg.png`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.3/gn2pg/app/utils/admin_views.py` & `gn2pg_client-1.6.4/gn2pg/app/utils/admin_views.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.3/gn2pg/check_conf.py` & `gn2pg_client-1.6.4/gn2pg/check_conf.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.3/gn2pg/data/gn2pgconfig.toml` & `gn2pg_client-1.6.4/gn2pg/data/gn2pgconfig.toml`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.3/gn2pg/data/to_gnsynthese.sql` & `gn2pg_client-1.6.4/gn2pg/data/to_gnsynthese.sql`

 * *Files 0% similar despite different names*

```diff
@@ -695,15 +695,15 @@
                WHEN 'synthese_with_label' THEN gn2pg_import.fct_c_get_id_nomenclature_from_label('TYPE',
                                                                                                  new.item #>> '{label}')
                ELSE ref_nomenclatures.get_id_nomenclature('TYPE', new.item #>> '{label}')
                END AS id_nomenclature_determination_method
     INTO the_id_nomenclature_determination_method;
     SELECT new.item #>> '{comment_releve}'
     INTO the_comment_context;
-    SELECT new.item #>> '{comment_occurence}'
+    SELECT new.item #>> '{comment_occurrence}'
     INTO the_comment_description;
     SELECT new.item #> '{additional_data}'
     INTO the_additional_data;
     SELECT NULL
     INTO the_meta_validation_date;
 
     /* Proceed to upsert */
```

### Comparing `gn2pg_client-1.6.3/gn2pg/download.py` & `gn2pg_client-1.6.4/gn2pg/download.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.3/gn2pg/helpers.py` & `gn2pg_client-1.6.4/gn2pg/helpers.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.3/gn2pg/locale/en_US/LC_MESAGES/gn2pg.po` & `gn2pg_client-1.6.4/gn2pg/locale/en_US/LC_MESAGES/gn2pg.po`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.3/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po` & `gn2pg_client-1.6.4/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.3/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po~` & `gn2pg_client-1.6.4/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po~`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.3/gn2pg/main.py` & `gn2pg_client-1.6.4/gn2pg/main.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.3/gn2pg/metadata.py` & `gn2pg_client-1.6.4/gn2pg/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Information describing the project.
 """
 
 # The package name, which is also the "UNIX name" for the project.
 PACKAGE = "gn2pg_client"
 PROJECT = "GeoNature 2 PostgreSQL Client application"
 PROJECT_NO_SPACES = PROJECT.replace(" ", "")
-VERSION = "1.6.2"
+VERSION = "1.6.4"
 DESCRIPTION = "Import tool from GeoNature to a PostgreSQL database through Export module API"
 AUTHORS = [
     "@lpofredc (LPOAuRA)",
     "@ophdlv (@NaturalSolutions)",
     "@mvergez (@NaturalSolutions)",
     "@Adrien-Pajot (@NaturalSolutions)",
     "@camillemonchicourt (@PnEcrins)",
```

### Comparing `gn2pg_client-1.6.3/gn2pg/store_postgresql.py` & `gn2pg_client-1.6.4/gn2pg/store_postgresql.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.3/gn2pg/utils.py` & `gn2pg_client-1.6.4/gn2pg/utils.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.6.3/pyproject.toml` & `gn2pg_client-1.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "gn2pg_client"
 packages = [{ include = "gn2pg" }]
-version = "1.6.3"
+version = "1.6.4"
 description = "Import tool from GeoNature to a PostgreSQL database through Export module API (client side)"
 authors = ["lpofredc <frederic.cloitre@lpo.fr>"]
 maintainers = ["lpofredc <frederic.cloitre@lpo.fr>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/lpoaura/gn2gn_client/"
 keywords = ["GeoNature", "Export", "SINP", "opendata", "biodiversity"]
```

### Comparing `gn2pg_client-1.6.3/PKG-INFO` & `gn2pg_client-1.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gn2pg_client
-Version: 1.6.3
+Version: 1.6.4
 Summary: Import tool from GeoNature to a PostgreSQL database through Export module API (client side)
 Home-page: https://github.com/lpoaura/gn2gn_client/
 License: AGPL-3.0-or-later
 Keywords: GeoNature,Export,SINP,opendata,biodiversity
 Author: lpofredc
 Author-email: frederic.cloitre@lpo.fr
 Maintainer: lpofredc
```

