# Comparing `tmp/ckanext_datapackage-0.1.0.tar.gz` & `tmp/ckanext_datapackage-0.2.0.tar.gz`

## Comparing `ckanext_datapackage-0.1.0.tar` & `ckanext_datapackage-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,24 @@
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ckanext_datapackage-0.1.0/.github/codecov.yaml
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 ckanext_datapackage-0.1.0/.github/issue_template.md
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ckanext_datapackage-0.1.0/.github/pull_request_template.md
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 ckanext_datapackage-0.1.0/.github/stale.yaml
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 ckanext_datapackage-0.1.0/.github/workflows/general.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ckanext_datapackage-0.1.0/ckanext/__init__.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 ckanext_datapackage-0.1.0/ckanext/conftest.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ckanext_datapackage-0.1.0/ckanext/datapackage/__init__.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 ckanext_datapackage-0.1.0/ckanext/datapackage/settings.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 ckanext_datapackage-0.1.0/ckanext/datapackage/__spec__/test_placeholder.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 ckanext_datapackage-0.1.0/.gitignore
--rw-r--r--   0        0        0    34363 2020-02-02 00:00:00.000000 ckanext_datapackage-0.1.0/LICENSE.md
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 ckanext_datapackage-0.1.0/README.md
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 ckanext_datapackage-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 ckanext_datapackage-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/.github/codecov.yaml
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/.github/issue_template.md
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/.github/pull_request_template.md
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/.github/stale.yaml
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/.github/workflows/general.yaml
+-rw-r--r--   0        0        0   146468 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/assets/dataset.png
+-rw-r--r--   0        0        0    18716 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/assets/package.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/ckanext/__init__.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/ckanext/conftest.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/ckanext/datapackage/__init__.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/ckanext/datapackage/actions.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/ckanext/datapackage/auth.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/ckanext/datapackage/blueprint.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/ckanext/datapackage/plugin.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/ckanext/datapackage/settings.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/ckanext/datapackage/__spec__/test_placeholder.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/ckanext/datapackage/templates/package/snippets/additional_info.html
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     8981 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/README.md
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 ckanext_datapackage-0.2.0/PKG-INFO
```

### Comparing `ckanext_datapackage-0.1.0/.github/stale.yaml` & `ckanext_datapackage-0.2.0/.github/stale.yaml`

 * *Files identical despite different names*

### Comparing `ckanext_datapackage-0.1.0/.github/workflows/general.yaml` & `ckanext_datapackage-0.2.0/.github/workflows/general.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,18 @@
         with:
           python-version: ${{ matrix.python-version }}
       - name: Prepare environment
         run: pip3 install hatch
       - name: Test software
         run: hatch run +py=${{ matrix.py || matrix.python-version }} ci:test
       - name: Report coverage
-        uses: codecov/codecov-action@v2
+        uses: codecov/codecov-action@v4.0.1
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }}
+          slug: frictionlessdata/ckanext-datapackage
 
   # Release
 
   release:
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
     needs: [test]
```

### Comparing `ckanext_datapackage-0.1.0/.gitignore` & `ckanext_datapackage-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ckanext_datapackage-0.1.0/pyproject.toml` & `ckanext_datapackage-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "ckanext-datapackage"
 dynamic = ["version"]
 description = "Data Package integreation for CKAN"
-license = "AGPL-3.0"
+license = "MIT"
 readme = "README.md"
 requires-python = ">=3.8"
 urls.homepage = "https://github.com/frictionlessdata/ckanext-datapackage"
 authors = [
     {name = "Open Knowledge Foundation", email = "info@okfn.org"},
 ]
 keywords=[
@@ -28,34 +28,41 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
-    "dplib-py[sql]>=0.7",
+    "dplib-py==0.7.5",
 ]
 
 [project.optional-dependencies]
 dev = [
     "ruff",
     "hatch",
     "neovim",
-    "pytest",
     "pyright",
     "ipython",
+    # ckan
+    "ckan",
+    "flask",
+    # pytest
+    "pytest",
     "pytest-cov",
     "pytest-vcr",
     "pytest-mock",
     "pytest-only",
     "pytest-dotenv",
     "pytest-timeout",
     "pytest-lazy-fixtures",
 ]
 
+[project.entry-points."ckan.plugins"]
+datapackage="ckanext.datapackage.plugin:DataPackagePlugin"
+
 [tool.hatch.version]
 path = "ckanext/datapackage/settings.py"
 
 [tool.hatch.build.targets.wheel]
 packages = ["ckanext"]
 
 [tool.hatch.envs.default]
@@ -127,14 +134,14 @@
 [tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401", "F403"]
 
 [tool.pytest.ini_options]
 testpaths = ["ckanext"]
 env_files = [".env"]
 markers = [
-    "ci: integrational tests (select with '--ci')",
+  "ci: integrational tests (select with '--ci')",
 ]
 
 [tool.pyright]
-strict = ["ckanext"]
+# strict = ["ckanext"]
 include = ["ckanext"]
 ignore = ["**/__init__.py"]
```

