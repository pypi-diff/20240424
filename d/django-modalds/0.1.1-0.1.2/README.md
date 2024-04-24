# Comparing `tmp/django_modalds-0.1.1.tar.gz` & `tmp/django_modalds-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_modalds-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_modalds-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_modalds-0.1.1.tar` & `django_modalds-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     6148 2024-03-20 06:31:46.234580 django_modalds-0.1.1/.DS_Store
--rw-r--r--   0        0        0       66 2024-03-20 06:31:24.352716 django_modalds-0.1.1/.gitattributes
--rw-r--r--   0        0        0        7 2024-03-20 06:42:27.733546 django_modalds-0.1.1/.gitignore
--rw-r--r--   0        0        0      561 2024-03-20 06:42:46.246240 django_modalds-0.1.1/.idea/django-modalds.iml
--rw-r--r--   0        0        0      174 2024-03-20 06:42:46.266987 django_modalds-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      419 2024-03-20 06:42:46.257139 django_modalds-0.1.1/.idea/misc.xml
--rw-r--r--   0        0        0      280 2024-03-20 06:42:46.249379 django_modalds-0.1.1/.idea/modules.xml
--rw-r--r--   0        0        0      167 2024-03-20 06:42:46.269904 django_modalds-0.1.1/.idea/vcs.xml
--rw-r--r--   0        0        0     3349 2024-04-12 05:19:57.446364 django_modalds-0.1.1/.idea/workspace.xml
--rw-r--r--   0        0        0     1079 2024-03-17 02:01:04.369747 django_modalds-0.1.1/LICENSE
--rw-r--r--   0        0        0      986 2024-03-20 06:37:57.974200 django_modalds-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-03-19 12:26:04.845135 django_modalds-0.1.1/__init__.py
--rw-r--r--   0        0        0     6148 2024-03-20 04:57:42.962921 django_modalds-0.1.1/django_modalds/.DS_Store
--rw-r--r--   0        0        0        0 2024-03-20 04:56:14.425896 django_modalds-0.1.1/django_modalds/__init__.py
--rw-r--r--   0        0        0      673 2024-03-20 04:58:10.906719 django_modalds-0.1.1/django_modalds/admin.py
--rw-r--r--   0        0        0      159 2024-03-20 06:34:50.496883 django_modalds-0.1.1/django_modalds/apps.py
--rw-r--r--   0        0        0     5451 2024-03-20 05:16:29.358222 django_modalds-0.1.1/django_modalds/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-03-20 04:56:14.427712 django_modalds-0.1.1/django_modalds/migrations/__init__.py
--rw-r--r--   0        0        0     5597 2024-03-20 04:58:30.866086 django_modalds-0.1.1/django_modalds/models.py
--rw-r--r--   0        0        0     6148 2024-03-17 02:26:18.949539 django_modalds-0.1.1/django_modalds/static/popupds/.DS_Store
--rw-r--r--   0        0        0    89501 2023-03-21 07:33:49.921877 django_modalds-0.1.1/django_modalds/static/popupds/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0     3252 2023-03-21 07:33:49.693764 django_modalds-0.1.1/django_modalds/static/popupds/js/jquery.cookie.js
--rw-r--r--   0        0        0     2515 2024-04-12 05:18:38.250197 django_modalds-0.1.1/django_modalds/templates/django_modalds/modalds.html
--rw-r--r--   0        0        0     3154 2024-03-18 03:18:17.556824 django_modalds-0.1.1/django_modalds/templates/django_modalds/type1.html
--rw-r--r--   0        0        0     3319 2024-03-18 03:18:17.567128 django_modalds-0.1.1/django_modalds/templates/django_modalds/type2.html
--rw-r--r--   0        0        0     3069 2024-03-18 03:18:17.563552 django_modalds-0.1.1/django_modalds/templates/django_modalds/type3.html
--rw-r--r--   0        0        0     2501 2024-03-18 03:18:17.561054 django_modalds-0.1.1/django_modalds/templates/django_modalds/type4.html
--rw-r--r--   0        0        0      632 2024-03-18 03:18:17.565436 django_modalds-0.1.1/django_modalds/templates/django_modalds/type5.html
--rw-r--r--   0        0        0        0 2024-03-15 04:56:10.557033 django_modalds-0.1.1/django_modalds/templatetags/__init__.py
--rw-r--r--   0        0        0     1759 2024-03-20 06:37:57.977861 django_modalds-0.1.1/django_modalds/templatetags/django_modalds_tags.py
--rw-r--r--   0        0        0       60 2024-03-20 04:56:14.427567 django_modalds-0.1.1/django_modalds/tests.py
--rw-r--r--   0        0        0       63 2024-03-20 04:56:14.426329 django_modalds-0.1.1/django_modalds/views.py
--rw-r--r--   0        0        0      684 2024-04-12 07:06:23.609744 django_modalds-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 django_modalds-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2024-03-20 06:31:46.234580 django_modalds-0.1.2/.DS_Store
+-rw-r--r--   0        0        0       66 2024-03-20 06:31:24.352716 django_modalds-0.1.2/.gitattributes
+-rw-r--r--   0        0        0        7 2024-03-20 06:42:27.733546 django_modalds-0.1.2/.gitignore
+-rw-r--r--   0        0        0      561 2024-03-20 06:42:46.246240 django_modalds-0.1.2/.idea/django-modalds.iml
+-rw-r--r--   0        0        0      174 2024-03-20 06:42:46.266987 django_modalds-0.1.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      419 2024-03-20 06:42:46.257139 django_modalds-0.1.2/.idea/misc.xml
+-rw-r--r--   0        0        0      280 2024-03-20 06:42:46.249379 django_modalds-0.1.2/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2024-03-20 06:42:46.269904 django_modalds-0.1.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     4075 2024-04-12 07:06:44.870789 django_modalds-0.1.2/.idea/workspace.xml
+-rw-r--r--   0        0        0     1079 2024-03-17 02:01:04.369747 django_modalds-0.1.2/LICENSE
+-rw-r--r--   0        0        0      986 2024-03-20 06:37:57.974200 django_modalds-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-03-19 12:26:04.845135 django_modalds-0.1.2/__init__.py
+-rw-r--r--   0        0        0     6148 2024-03-20 04:57:42.962921 django_modalds-0.1.2/django_modalds/.DS_Store
+-rw-r--r--   0        0        0        0 2024-03-20 04:56:14.425896 django_modalds-0.1.2/django_modalds/__init__.py
+-rw-r--r--   0        0        0      673 2024-03-20 04:58:10.906719 django_modalds-0.1.2/django_modalds/admin.py
+-rw-r--r--   0        0        0      159 2024-03-20 06:34:50.496883 django_modalds-0.1.2/django_modalds/apps.py
+-rw-r--r--   0        0        0     5451 2024-03-20 05:16:29.358222 django_modalds-0.1.2/django_modalds/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-03-20 04:56:14.427712 django_modalds-0.1.2/django_modalds/migrations/__init__.py
+-rw-r--r--   0        0        0     5597 2024-03-20 04:58:30.866086 django_modalds-0.1.2/django_modalds/models.py
+-rw-r--r--   0        0        0     6148 2024-03-17 02:26:18.949539 django_modalds-0.1.2/django_modalds/static/popupds/.DS_Store
+-rw-r--r--   0        0        0    89501 2023-03-21 07:33:49.921877 django_modalds-0.1.2/django_modalds/static/popupds/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0     3252 2023-03-21 07:33:49.693764 django_modalds-0.1.2/django_modalds/static/popupds/js/jquery.cookie.js
+-rw-r--r--   0        0        0     2515 2024-04-12 05:18:38.250197 django_modalds-0.1.2/django_modalds/templates/django_modalds/modalds.html
+-rw-r--r--   0        0        0     3154 2024-03-18 03:18:17.556824 django_modalds-0.1.2/django_modalds/templates/django_modalds/type1.html
+-rw-r--r--   0        0        0     3319 2024-03-18 03:18:17.567128 django_modalds-0.1.2/django_modalds/templates/django_modalds/type2.html
+-rw-r--r--   0        0        0     3069 2024-03-18 03:18:17.563552 django_modalds-0.1.2/django_modalds/templates/django_modalds/type3.html
+-rw-r--r--   0        0        0     2501 2024-03-18 03:18:17.561054 django_modalds-0.1.2/django_modalds/templates/django_modalds/type4.html
+-rw-r--r--   0        0        0      632 2024-03-18 03:18:17.565436 django_modalds-0.1.2/django_modalds/templates/django_modalds/type5.html
+-rw-r--r--   0        0        0        0 2024-03-15 04:56:10.557033 django_modalds-0.1.2/django_modalds/templatetags/__init__.py
+-rw-r--r--   0        0        0     1759 2024-03-20 06:37:57.977861 django_modalds-0.1.2/django_modalds/templatetags/django_modalds_tags.py
+-rw-r--r--   0        0        0       60 2024-03-20 04:56:14.427567 django_modalds-0.1.2/django_modalds/tests.py
+-rw-r--r--   0        0        0       63 2024-03-20 04:56:14.426329 django_modalds-0.1.2/django_modalds/views.py
+-rw-r--r--   0        0        0      685 2024-04-24 01:49:10.694190 django_modalds-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1332 1970-01-01 00:00:00.000000 django_modalds-0.1.2/PKG-INFO
```

### Comparing `django_modalds-0.1.1/.DS_Store` & `django_modalds-0.1.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.1/.idea/django-modalds.iml` & `django_modalds-0.1.2/.idea/django-modalds.iml`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.1/.idea/workspace.xml` & `django_modalds-0.1.2/.idea/workspace.xml`

 * *Files 18% similar despite different names*

#### Comparing `django_modalds-0.1.1/.idea/workspace.xml` & `django_modalds-0.1.2/.idea/workspace.xml`

```diff
@@ -1,37 +1,41 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="e7de678e-305c-4307-87c6-2108e448b4bf" name="변경" comment="">
+      <change beforePath="$PROJECT_DIR$/.idea/workspace.xml" beforeDir="false" afterPath="$PROJECT_DIR$/.idea/workspace.xml" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/db.sqlite3" beforeDir="false" afterPath="$PROJECT_DIR$/db.sqlite3" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/dist/django_modalds-0.1.0-py2.py3-none-any.whl" beforeDir="false" afterPath="$PROJECT_DIR$/dist/django_modalds-0.1.0-py2.py3-none-any.whl" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/dist/django_modalds-0.1.0.tar.gz" beforeDir="false" afterPath="$PROJECT_DIR$/dist/django_modalds-0.1.0.tar.gz" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/django_modalds/templates/django_modalds/modalds.html" beforeDir="false" afterPath="$PROJECT_DIR$/django_modalds/templates/django_modalds/modalds.html" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
   </component>
-  <component name="GitHubPullRequestSearchHistory"><![CDATA[{
-  "lastFilter": {
-    "state": "OPEN",
-    "assignee": "hj3415"
+  <component name="GitHubPullRequestSearchHistory">{
+  &quot;lastFilter&quot;: {
+    &quot;state&quot;: &quot;OPEN&quot;,
+    &quot;assignee&quot;: &quot;hj3415&quot;
   }
-}]]></component>
-  <component name="GithubPullRequestsUISettings"><![CDATA[{
-  "selectedUrlAndAccountId": {
-    "url": "https://github.com/hj3415/django-modalds.git",
-    "accountId": "c5909c03-ef4c-41ae-b532-d8fddfd35a45"
+}</component>
+  <component name="GithubPullRequestsUISettings">{
+  &quot;selectedUrlAndAccountId&quot;: {
+    &quot;url&quot;: &quot;https://github.com/hj3415/django-modalds.git&quot;,
+    &quot;accountId&quot;: &quot;c5909c03-ef4c-41ae-b532-d8fddfd35a45&quot;
   }
-}]]></component>
+}</component>
   <component name="MarkdownSettingsMigration">
     <option name="stateVersion" value="1"/>
   </component>
   <component name="ProjectColorInfo">{
   &quot;associatedIndex&quot;: 0
 }</component>
   <component name="ProjectId" id="2dwPmduLHTMDOVsXPLIrEwNTfn4"/>
```

### Comparing `django_modalds-0.1.1/LICENSE` & `django_modalds-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.1/README.md` & `django_modalds-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.1/django_modalds/.DS_Store` & `django_modalds-0.1.2/django_modalds/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.1/django_modalds/admin.py` & `django_modalds-0.1.2/django_modalds/admin.py`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.1/django_modalds/migrations/0001_initial.py` & `django_modalds-0.1.2/django_modalds/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.1/django_modalds/models.py` & `django_modalds-0.1.2/django_modalds/models.py`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.1/django_modalds/static/popupds/.DS_Store` & `django_modalds-0.1.2/django_modalds/static/popupds/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.1/django_modalds/static/popupds/js/jquery-3.6.0.min.js` & `django_modalds-0.1.2/django_modalds/static/popupds/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.1/django_modalds/static/popupds/js/jquery.cookie.js` & `django_modalds-0.1.2/django_modalds/static/popupds/js/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.1/django_modalds/templates/django_modalds/modalds.html` & `django_modalds-0.1.2/django_modalds/templates/django_modalds/modalds.html`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.1/django_modalds/templates/django_modalds/type1.html` & `django_modalds-0.1.2/django_modalds/templates/django_modalds/type1.html`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.1/django_modalds/templates/django_modalds/type2.html` & `django_modalds-0.1.2/django_modalds/templates/django_modalds/type2.html`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.1/django_modalds/templates/django_modalds/type3.html` & `django_modalds-0.1.2/django_modalds/templates/django_modalds/type3.html`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.1/django_modalds/templates/django_modalds/type4.html` & `django_modalds-0.1.2/django_modalds/templates/django_modalds/type4.html`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.1/django_modalds/templates/django_modalds/type5.html` & `django_modalds-0.1.2/django_modalds/templates/django_modalds/type5.html`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.1/django_modalds/templatetags/django_modalds_tags.py` & `django_modalds-0.1.2/django_modalds/templatetags/django_modalds_tags.py`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.1/pyproject.toml` & `django_modalds-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "django-modalds"
-version = "0.1.1"
+version = "0.1.2"
 description = "One of the my demiansoft apps"
 authors = [{name = "Hyungjin Kim", email = "hj3415@gmail.com"}]
 license = {file = "LICENSE"}
 readme = "README.md"
 classifiers = ["License :: OSI Approved :: MIT License"]
 dependencies = [
-    "Django >= 5.0.3",
+    "Django >= 4.2.11",
     "pillow >= 10.2.0", # 파일 업로드 위해
 ]
 
 [project.urls]
 Home = "https://www.demiansoft.com"
 
 [tool.flit.sdist]
```

### Comparing `django_modalds-0.1.1/PKG-INFO` & `django_modalds-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: django-modalds
-Version: 0.1.1
+Version: 0.1.2
 Summary: One of the my demiansoft apps
 Author-email: Hyungjin Kim <hj3415@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: Django >= 5.0.3
+Requires-Dist: Django >= 4.2.11
 Requires-Dist: pillow >= 10.2.0
 Project-URL: Home, https://www.demiansoft.com
 
 ### django-modalds
 
 #### Introduction
```

