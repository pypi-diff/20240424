# Comparing `tmp/testsolar-testtool-sdk-py2-0.1.7.tar.gz` & `tmp/testsolar-testtool-sdk-py2-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/testsolar-testtool-sdk-py2-0.1.7.tar", last modified: Tue Apr 23 07:00:08 2024, max compression
+gzip compressed data, was "dist/testsolar-testtool-sdk-py2-0.1.8.tar", last modified: Tue Apr 23 09:36:36 2024, max compression
```

## Comparing `testsolar-testtool-sdk-py2-0.1.7.tar` & `testsolar-testtool-sdk-py2-0.1.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/
--rw-r--r--   0 root         (0) root         (0)     1052 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/setup.py
--rw-r--r--   0 root         (0) root         (0)      148 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      581 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/
--rw-r--r--   0 root         (0) root         (0)     2327 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/reporter.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)      683 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/pipe_reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/model/
--rw-r--r--   0 root         (0) root         (0)     1324 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/model/encoder.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/model/load.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2887 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/model/testresult.py
--rw-r--r--   0 root         (0) root         (0)      851 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/model/param.py
--rw-r--r--   0 root         (0) root         (0)      317 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/decoder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/tests/
--rw-r--r--   0 root         (0) root         (0)      493 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/tests/test_param.py
--rw-r--r--   0 root         (0) root         (0)      219 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/tests/test_decoder.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5961 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/tests/test_report.py
--rw-r--r--   0 root         (0) root         (0)      652 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/tests/test_testresult.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      714 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      581 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk_py2.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:36:36.000000 testsolar-testtool-sdk-py2-0.1.8/
+-rw-r--r--   0 root         (0) root         (0)     1052 2024-04-23 09:36:30.000000 testsolar-testtool-sdk-py2-0.1.8/setup.py
+-rw-r--r--   0 root         (0) root         (0)      148 2024-04-23 09:36:30.000000 testsolar-testtool-sdk-py2-0.1.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 09:36:36.000000 testsolar-testtool-sdk-py2-0.1.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      581 2024-04-23 09:36:36.000000 testsolar-testtool-sdk-py2-0.1.8/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:36:36.000000 testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk/
+-rw-r--r--   0 root         (0) root         (0)     2327 2024-04-23 09:36:30.000000 testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk/reporter.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 09:36:30.000000 testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      683 2024-04-23 09:36:30.000000 testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk/pipe_reader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:36:36.000000 testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk/model/
+-rw-r--r--   0 root         (0) root         (0)     1324 2024-04-23 09:36:30.000000 testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk/model/encoder.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-04-23 09:36:30.000000 testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk/model/load.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 09:36:30.000000 testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3070 2024-04-23 09:36:30.000000 testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk/model/testresult.py
+-rw-r--r--   0 root         (0) root         (0)      851 2024-04-23 09:36:30.000000 testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk/model/param.py
+-rw-r--r--   0 root         (0) root         (0)      317 2024-04-23 09:36:30.000000 testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk/decoder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:36:36.000000 testsolar-testtool-sdk-py2-0.1.8/tests/
+-rw-r--r--   0 root         (0) root         (0)      493 2024-04-23 09:36:30.000000 testsolar-testtool-sdk-py2-0.1.8/tests/test_param.py
+-rw-r--r--   0 root         (0) root         (0)      298 2024-04-23 09:36:30.000000 testsolar-testtool-sdk-py2-0.1.8/tests/test_decoder.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 09:36:30.000000 testsolar-testtool-sdk-py2-0.1.8/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7232 2024-04-23 09:36:30.000000 testsolar-testtool-sdk-py2-0.1.8/tests/test_report.py
+-rw-r--r--   0 root         (0) root         (0)      947 2024-04-23 09:36:30.000000 testsolar-testtool-sdk-py2-0.1.8/tests/test_testresult.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:36:36.000000 testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 09:36:36.000000 testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      714 2024-04-23 09:36:36.000000 testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-23 09:36:36.000000 testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      581 2024-04-23 09:36:36.000000 testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-23 09:36:36.000000 testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk_py2.egg-info/requires.txt
```

### Comparing `testsolar-testtool-sdk-py2-0.1.7/setup.py` & `testsolar-testtool-sdk-py2-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with open(req_file, 'r') as f:
         install_requires = [str(req) for req in parse_requirements(f)]
         return install_requires
 
 
 setup(
     name='testsolar-testtool-sdk-py2',
-    version='0.1.7',
+    version='0.1.8',
     author='asiazhang',
     author_email='asiazhang2002@gmail.com',
     description='Python2 SDK for TestSolar testtool',
     url='https://github.com/OpenTestSolar/testtool-sdk-python-py2',
     packages=find_packages(),
     python_requires='>=2.7, <3',
     classifiers=[
```

### Comparing `testsolar-testtool-sdk-py2-0.1.7/PKG-INFO` & `testsolar-testtool-sdk-py2-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: testsolar-testtool-sdk-py2
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python2 SDK for TestSolar testtool
 Home-page: https://github.com/OpenTestSolar/testtool-sdk-python-py2
 Author: asiazhang
 Author-email: asiazhang2002@gmail.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: testsolar
```

### Comparing `testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/reporter.py` & `testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk/reporter.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/pipe_reader.py` & `testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk/pipe_reader.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/model/encoder.py` & `testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk/model/encoder.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/model/testresult.py` & `testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk/model/testresult.py`

 * *Files 9% similar despite different names*

```diff
@@ -72,14 +72,23 @@
         self.Time = time
         self.Level = level
         self.Content = content
         self.AssertError = assert_error
         self.RuntimeError = runtime_error
         self.Attachments = attachments
 
+    def is_error(self):
+        # type: () -> bool
+        """
+        Checks if the log is an error
+        """
+        return self.Level in [
+            LogLevel.ERROR,
+        ]
+
 
 class TestCaseStep:
     __test__ = False
 
     def __init__(self, start_time, title, result_type, end_time, logs):
         # type:(datetime, str, ResultType, datetime, List[TestCaseLog]) -> None
         self.StartTime = start_time
```

### Comparing `testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/model/param.py` & `testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk/model/param.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-py2-0.1.7/tests/test_report.py` & `testsolar-testtool-sdk-py2-0.1.8/tests/test_report.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 from testsolar_testtool_sdk.model.load import LoadResult, LoadError
 from testsolar_testtool_sdk.model.testresult import ResultType, LogLevel, TestCase
 from testsolar_testtool_sdk.model.testresult import (
     TestResult,
     TestCaseStep,
     TestCaseAssertError,
     TestCaseLog,
+    TestCaseRuntimeError,
+    Attachment,
+    AttachmentType,
 )
 from testsolar_testtool_sdk.pipe_reader import read_result
 from testsolar_testtool_sdk.reporter import Reporter, convert_to_json
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
@@ -169,7 +172,42 @@
         assert r2.get('ResultType') == ResultType.SUCCEED
         r3 = read_result(pipe_io)
         assert r3.get('ResultType') == ResultType.SUCCEED
         r4 = read_result(pipe_io)
         assert r4.get('ResultType') == ResultType.SUCCEED
         r5 = read_result(pipe_io)
         assert r5.get('ResultType') == ResultType.SUCCEED
+
+
+def test_convert_to_json_with_custom_encoder():
+    tr = TestResult(
+        TestCase("mumu/mu.py/test_case_name_%s_p1", {"tag": "bbb"}),
+        datetime.utcnow(),
+        ResultType.SUCCEED,
+        "ファイルが見つかりません",
+        datetime.utcnow(),
+        [TestCaseStep(
+            start_time=datetime.utcnow(),
+            title="hello world",
+            result_type=ResultType.SUCCEED,
+            end_time=datetime.utcnow(),
+            logs=[
+                TestCaseLog(
+                    time=datetime.utcnow(),
+                    level=LogLevel.INFO,
+                    content="hello world 1",
+                    assert_error=TestCaseAssertError("AAA", "BBB", "AAA is not BBB"),
+                    runtime_error=TestCaseRuntimeError("AAA", "BBB"),
+                    attachments=[Attachment(
+                        name="attachment 1",
+                        attachment_type=AttachmentType.URL,
+                        url="https://example.com",
+                    )]
+                )
+            ]
+        )],
+    )
+
+    re = json.loads(convert_to_json(tr))
+
+    assert len(re['Steps']) == 1
+    assert re['Steps'][0]['Logs'][0]['RuntimeError']['Summary'] == 'AAA'
```

### Comparing `testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk_py2.egg-info/SOURCES.txt` & `testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk_py2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk_py2.egg-info/PKG-INFO` & `testsolar-testtool-sdk-py2-0.1.8/testsolar_testtool_sdk_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: testsolar-testtool-sdk-py2
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python2 SDK for TestSolar testtool
 Home-page: https://github.com/OpenTestSolar/testtool-sdk-python-py2
 Author: asiazhang
 Author-email: asiazhang2002@gmail.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: testsolar
```

