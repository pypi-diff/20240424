# Comparing `tmp/trycicle-0.3.0.tar.gz` & `tmp/trycicle-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trycicle-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "trycicle-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `trycicle-0.3.0.tar` & `trycicle-0.3.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0       83 2024-04-16 12:08:46.918705 trycicle-0.3.0/.gitignore
--rw-r--r--   0        0        0     3570 2024-04-16 12:08:46.918705 trycicle-0.3.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      960 2024-04-16 12:08:46.918705 trycicle-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     4714 2024-04-16 12:08:46.918705 trycicle-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     1071 2024-04-16 12:08:46.918705 trycicle-0.3.0/LICENSE
--rw-r--r--   0        0        0      615 2024-04-16 12:08:46.918705 trycicle-0.3.0/Pipfile
--rw-r--r--   0        0        0    56080 2024-04-16 12:08:46.918705 trycicle-0.3.0/Pipfile.lock
--rw-r--r--   0        0        0     9417 2024-04-16 12:08:46.918705 trycicle-0.3.0/README.md
--rw-r--r--   0        0        0       53 2024-04-16 12:08:46.918705 trycicle-0.3.0/ci/pipenv/Dockerfile
--rw-r--r--   0        0        0      175 2024-04-16 12:08:46.918705 trycicle-0.3.0/ci/pre-commit/Dockerfile
--rw-r--r--   0        0        0       76 2024-04-16 12:08:46.918705 trycicle-0.3.0/commitlint.config.js
--rw-r--r--   0        0        0     1959 2024-04-16 12:08:46.919705 trycicle-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      102 2024-04-16 12:08:46.919705 trycicle-0.3.0/setup.py
--rw-r--r--   0        0        0      109 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/basic.yml
--rw-r--r--   0        0        0     2387 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0     1152 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/example.yml
--rw-r--r--   0        0        0     1053 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/extends.yml
--rw-r--r--   0        0        0      170 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/meta.yml
--rw-r--r--   0        0        0      712 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/references.yml
--rw-r--r--   0        0        0     3794 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/test_cache.py
--rw-r--r--   0        0        0     6455 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/test_cli.py
--rw-r--r--   0        0        0     1979 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/test_git_clone.py
--rw-r--r--   0        0        0     6099 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/test_integration.py
--rw-r--r--   0        0        0     8379 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/test_parser.py
--rw-r--r--   0        0        0    15172 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/test_run.py
--rw-r--r--   0        0        0     2552 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/test_variables.py
--rw-r--r--   0        0        0        0 2024-04-16 12:08:46.947704 trycicle-0.3.0/trycicle/__init__.py
--rw-r--r--   0        0        0       59 2024-04-16 12:08:46.919705 trycicle-0.3.0/trycicle/__main__.py
--rw-r--r--   0        0        0     2149 2024-04-16 12:08:46.919705 trycicle-0.3.0/trycicle/cache.py
--rw-r--r--   0        0        0     4417 2024-04-16 12:08:46.920705 trycicle-0.3.0/trycicle/cli.py
--rw-r--r--   0        0        0     1437 2024-04-16 12:08:46.920705 trycicle-0.3.0/trycicle/git_clone.py
--rw-r--r--   0        0        0     2004 2024-04-16 12:08:46.920705 trycicle-0.3.0/trycicle/models.py
--rw-r--r--   0        0        0     6923 2024-04-16 12:08:46.920705 trycicle-0.3.0/trycicle/parser.py
--rw-r--r--   0        0        0     9652 2024-04-16 12:08:46.920705 trycicle-0.3.0/trycicle/run.py
--rw-r--r--   0        0        0      517 2024-04-16 12:08:46.920705 trycicle-0.3.0/trycicle/subprocess.py
--rw-r--r--   0        0        0     5109 2024-04-16 12:08:46.920705 trycicle-0.3.0/trycicle/variables.py
--rw-r--r--   0        0        0     9932 1970-01-01 00:00:00.000000 trycicle-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       83 2024-04-24 09:24:27.259621 trycicle-0.3.1/.gitignore
+-rw-r--r--   0        0        0     3570 2024-04-24 09:24:27.259621 trycicle-0.3.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0      960 2024-04-24 09:24:27.259621 trycicle-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4715 2024-04-24 09:24:27.259621 trycicle-0.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2024-04-24 09:24:27.259621 trycicle-0.3.1/LICENSE
+-rw-r--r--   0        0        0      615 2024-04-24 09:24:27.259621 trycicle-0.3.1/Pipfile
+-rw-r--r--   0        0        0    56080 2024-04-24 09:24:27.259621 trycicle-0.3.1/Pipfile.lock
+-rw-r--r--   0        0        0     9417 2024-04-24 09:24:27.260620 trycicle-0.3.1/README.md
+-rw-r--r--   0        0        0       53 2024-04-24 09:24:27.260620 trycicle-0.3.1/ci/pipenv/Dockerfile
+-rw-r--r--   0        0        0      175 2024-04-24 09:24:27.260620 trycicle-0.3.1/ci/pre-commit/Dockerfile
+-rw-r--r--   0        0        0       76 2024-04-24 09:24:27.260620 trycicle-0.3.1/commitlint.config.js
+-rw-r--r--   0        0        0     1959 2024-04-24 09:24:27.260620 trycicle-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      102 2024-04-24 09:24:27.260620 trycicle-0.3.1/setup.py
+-rw-r--r--   0        0        0      226 2024-04-24 09:24:27.260620 trycicle-0.3.1/tests/basic.yml
+-rw-r--r--   0        0        0     2387 2024-04-24 09:24:27.260620 trycicle-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     1152 2024-04-24 09:24:27.260620 trycicle-0.3.1/tests/example.yml
+-rw-r--r--   0        0        0     1053 2024-04-24 09:24:27.260620 trycicle-0.3.1/tests/extends.yml
+-rw-r--r--   0        0        0      170 2024-04-24 09:24:27.260620 trycicle-0.3.1/tests/meta.yml
+-rw-r--r--   0        0        0      712 2024-04-24 09:24:27.260620 trycicle-0.3.1/tests/references.yml
+-rw-r--r--   0        0        0     3794 2024-04-24 09:24:27.260620 trycicle-0.3.1/tests/test_cache.py
+-rw-r--r--   0        0        0     6455 2024-04-24 09:24:27.260620 trycicle-0.3.1/tests/test_cli.py
+-rw-r--r--   0        0        0     1979 2024-04-24 09:24:27.260620 trycicle-0.3.1/tests/test_git_clone.py
+-rw-r--r--   0        0        0     6420 2024-04-24 09:24:27.260620 trycicle-0.3.1/tests/test_integration.py
+-rw-r--r--   0        0        0     8379 2024-04-24 09:24:27.260620 trycicle-0.3.1/tests/test_parser.py
+-rw-r--r--   0        0        0    15172 2024-04-24 09:24:27.260620 trycicle-0.3.1/tests/test_run.py
+-rw-r--r--   0        0        0     2552 2024-04-24 09:24:27.261620 trycicle-0.3.1/tests/test_variables.py
+-rw-r--r--   0        0        0        0 2024-04-24 09:24:27.284620 trycicle-0.3.1/trycicle/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-24 09:24:27.261620 trycicle-0.3.1/trycicle/__main__.py
+-rw-r--r--   0        0        0     2149 2024-04-24 09:24:27.261620 trycicle-0.3.1/trycicle/cache.py
+-rw-r--r--   0        0        0     4417 2024-04-24 09:24:27.261620 trycicle-0.3.1/trycicle/cli.py
+-rw-r--r--   0        0        0     1437 2024-04-24 09:24:27.261620 trycicle-0.3.1/trycicle/git_clone.py
+-rw-r--r--   0        0        0     2004 2024-04-24 09:24:27.261620 trycicle-0.3.1/trycicle/models.py
+-rw-r--r--   0        0        0     6923 2024-04-24 09:24:27.261620 trycicle-0.3.1/trycicle/parser.py
+-rw-r--r--   0        0        0     9653 2024-04-24 09:24:27.261620 trycicle-0.3.1/trycicle/run.py
+-rw-r--r--   0        0        0      517 2024-04-24 09:24:27.261620 trycicle-0.3.1/trycicle/subprocess.py
+-rw-r--r--   0        0        0     5109 2024-04-24 09:24:27.261620 trycicle-0.3.1/trycicle/variables.py
+-rw-r--r--   0        0        0     9932 1970-01-01 00:00:00.000000 trycicle-0.3.1/PKG-INFO
```

### Comparing `trycicle-0.3.0/.gitlab-ci.yml` & `trycicle-0.3.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `trycicle-0.3.0/.pre-commit-config.yaml` & `trycicle-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `trycicle-0.3.0/CHANGELOG.md` & `trycicle-0.3.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 # CHANGELOG
 
 
 
+## v0.3.1 (2024-04-24)
+
+### Fix
+
+* fix: stop script on first failure ([`47be6b2`](https://gitlab.com/phooijenga/trycicle/-/commit/47be6b2702b02dcfb3d62b463749c0b8718ae9af))
+
+
 ## v0.3.0 (2024-04-16)
 
+### Chore
+
+* chore(release): version 0.3.0 ([`50426f7`](https://gitlab.com/phooijenga/trycicle/-/commit/50426f73430ef63a783c72552dd106ac8437ae61))
+
 ### Documentation
 
 * docs: add cache example to readme ([`dfc5336`](https://gitlab.com/phooijenga/trycicle/-/commit/dfc5336bed36ac37c10d65a1979f8f22af6bbef8))
 
 ### Feature
 
 * feat: refactor how extends are applied
@@ -104,13 +115,7 @@
 * Add interactive debugger
 
 Closes #6. ([`c72bc59`](https://gitlab.com/phooijenga/trycicle/-/commit/c72bc59f2b07a7e0fbd75610ab0979e207c6af9e))
 
 * Label containers ([`fc8471f`](https://gitlab.com/phooijenga/trycicle/-/commit/fc8471fe269e2b7b3382384595f249c6c36ffd69))
 
 * Reset log level before running integration tests ([`1f66207`](https://gitlab.com/phooijenga/trycicle/-/commit/1f66207eccffadb6f796ee7a8f540a8aae3a6bca))
-
-* Add instructions to set up tab completion to readme
-
-Closes #7. ([`14ce3a8`](https://gitlab.com/phooijenga/trycicle/-/commit/14ce3a821be9f4fff4e100429be79de04d292150))
-
-* Add shell completion for jobs and variables ([`cdbc707`](https://gitlab.com/phooijenga/trycicle/-/commit/cdbc70793f456fbf211aa23677a0718db48674fc))
```

### Comparing `trycicle-0.3.0/LICENSE` & `trycicle-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trycicle-0.3.0/Pipfile` & `trycicle-0.3.1/Pipfile`

 * *Files identical despite different names*

### Comparing `trycicle-0.3.0/Pipfile.lock` & `trycicle-0.3.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `trycicle-0.3.0/README.md` & `trycicle-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `trycicle-0.3.0/pyproject.toml` & `trycicle-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "trycicle"
-version = "0.3.0"
+version = "0.3.1"
 description = "Try CI jobs locally"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: POSIX",
     "License :: OSI Approved :: MIT License",
 ]
```

### Comparing `trycicle-0.3.0/tests/conftest.py` & `trycicle-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `trycicle-0.3.0/tests/example.yml` & `trycicle-0.3.1/tests/example.yml`

 * *Files identical despite different names*

### Comparing `trycicle-0.3.0/tests/extends.yml` & `trycicle-0.3.1/tests/extends.yml`

 * *Files identical despite different names*

### Comparing `trycicle-0.3.0/tests/references.yml` & `trycicle-0.3.1/tests/references.yml`

 * *Files identical despite different names*

### Comparing `trycicle-0.3.0/tests/test_cache.py` & `trycicle-0.3.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `trycicle-0.3.0/tests/test_cli.py` & `trycicle-0.3.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `trycicle-0.3.0/tests/test_git_clone.py` & `trycicle-0.3.1/tests/test_git_clone.py`

 * *Files identical despite different names*

### Comparing `trycicle-0.3.0/tests/test_integration.py` & `trycicle-0.3.1/tests/test_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,23 @@
     with pytest.raises(SystemExit, match="0"):
         main(["--verbose", "--file", "tests/basic.yml", "job"])
 
     out, err = capfd.readouterr()
     assert "Hello, world!" in out
 
 
+def test_basic_failure(capfd: pytest.CaptureFixture[str]) -> None:
+    with pytest.raises(SystemExit, match="1"):
+        main(["--verbose", "--file", "tests/basic.yml", "fail"])
+
+    out, err = capfd.readouterr()
+    assert "ls: does-not-exist: No such file or directory" in out
+    assert "not be printed" not in out
+
+
 def test_meta(capfd: pytest.CaptureFixture[str]) -> None:
     with pytest.raises(SystemExit, match="0"):
         main(["--verbose", "--file", "tests/meta.yml", "--workdir", ".", "test"])
 
     out, err = capfd.readouterr()
     assert "test session starts" in out
     assert "FAILURES" not in out
```

### Comparing `trycicle-0.3.0/tests/test_parser.py` & `trycicle-0.3.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `trycicle-0.3.0/tests/test_run.py` & `trycicle-0.3.1/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `trycicle-0.3.0/tests/test_variables.py` & `trycicle-0.3.1/tests/test_variables.py`

 * *Files identical despite different names*

### Comparing `trycicle-0.3.0/trycicle/cache.py` & `trycicle-0.3.1/trycicle/cache.py`

 * *Files identical despite different names*

### Comparing `trycicle-0.3.0/trycicle/cli.py` & `trycicle-0.3.1/trycicle/cli.py`

 * *Files identical despite different names*

### Comparing `trycicle-0.3.0/trycicle/git_clone.py` & `trycicle-0.3.1/trycicle/git_clone.py`

 * *Files identical despite different names*

### Comparing `trycicle-0.3.0/trycicle/models.py` & `trycicle-0.3.1/trycicle/models.py`

 * *Files identical despite different names*

### Comparing `trycicle-0.3.0/trycicle/parser.py` & `trycicle-0.3.1/trycicle/parser.py`

 * *Files identical despite different names*

### Comparing `trycicle-0.3.0/trycicle/run.py` & `trycicle-0.3.1/trycicle/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 logger = logging.getLogger(__name__)
 
 job_script_shebang = "#!/bin/sh\n"
 
 job_script_header = """\
 git config --global --add safe.directory /src 2>/dev/null || true
-set -x
+set -ex
 """
 
 job_script_debugger = """\
 # Start a shell if the script fails
 function debugger() {
     set +x
     if [ -n "$1" ]; then
```

### Comparing `trycicle-0.3.0/trycicle/subprocess.py` & `trycicle-0.3.1/trycicle/subprocess.py`

 * *Files identical despite different names*

### Comparing `trycicle-0.3.0/trycicle/variables.py` & `trycicle-0.3.1/trycicle/variables.py`

 * *Files identical despite different names*

### Comparing `trycicle-0.3.0/PKG-INFO` & `trycicle-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trycicle
-Version: 0.3.0
+Version: 0.3.1
 Summary: Try CI jobs locally
 Author-email: Paul Hooijenga <paul@founda.com>
 Requires-Python: ~= 3.11
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: MIT License
```

