# Comparing `tmp/inductor-0.3.8.tar.gz` & `tmp/inductor-0.3.9.tar.gz`

## Comparing `inductor-0.3.8.tar` & `inductor-0.3.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    16397 2020-02-02 00:00:00.000000 inductor-0.3.8/inductor/__init__.py
--rw-r--r--   0        0        0    13918 2020-02-02 00:00:00.000000 inductor-0.3.8/inductor/auth_session.py
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 inductor-0.3.8/inductor/backend_client.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 inductor-0.3.8/inductor/config.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 inductor-0.3.8/inductor/util.py
--rw-r--r--   0        0        0    11399 2020-02-02 00:00:00.000000 inductor-0.3.8/inductor/wire_model.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 inductor-0.3.8/inductor/cli/__init__.py
--rw-r--r--   0        0        0    13367 2020-02-02 00:00:00.000000 inductor-0.3.8/inductor/cli/cli.py
--rw-r--r--   0        0        0    15131 2020-02-02 00:00:00.000000 inductor-0.3.8/inductor/cli/data_model.py
--rw-r--r--   0        0        0    12824 2020-02-02 00:00:00.000000 inductor-0.3.8/inductor/cli/execute.py
--rw-r--r--   0        0        0     9608 2020-02-02 00:00:00.000000 inductor-0.3.8/inductor/cli/questions.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 inductor-0.3.8/.gitignore
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 inductor-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 inductor-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    16397 2020-02-02 00:00:00.000000 inductor-0.3.9/inductor/__init__.py
+-rw-r--r--   0        0        0    13918 2020-02-02 00:00:00.000000 inductor-0.3.9/inductor/auth_session.py
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 inductor-0.3.9/inductor/backend_client.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 inductor-0.3.9/inductor/config.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 inductor-0.3.9/inductor/util.py
+-rw-r--r--   0        0        0    12733 2020-02-02 00:00:00.000000 inductor-0.3.9/inductor/wire_model.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 inductor-0.3.9/inductor/cli/__init__.py
+-rw-r--r--   0        0        0    13367 2020-02-02 00:00:00.000000 inductor-0.3.9/inductor/cli/cli.py
+-rw-r--r--   0        0        0    15353 2020-02-02 00:00:00.000000 inductor-0.3.9/inductor/cli/data_model.py
+-rw-r--r--   0        0        0    12824 2020-02-02 00:00:00.000000 inductor-0.3.9/inductor/cli/execute.py
+-rw-r--r--   0        0        0     9608 2020-02-02 00:00:00.000000 inductor-0.3.9/inductor/cli/questions.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 inductor-0.3.9/.gitignore
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 inductor-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 inductor-0.3.9/PKG-INFO
```

### Comparing `inductor-0.3.8/inductor/__init__.py` & `inductor-0.3.9/inductor/__init__.py`

 * *Files identical despite different names*

### Comparing `inductor-0.3.8/inductor/auth_session.py` & `inductor-0.3.9/inductor/auth_session.py`

 * *Files identical despite different names*

### Comparing `inductor-0.3.8/inductor/backend_client.py` & `inductor-0.3.9/inductor/backend_client.py`

 * *Files identical despite different names*

### Comparing `inductor-0.3.8/inductor/config.py` & `inductor-0.3.9/inductor/config.py`

 * *Files identical despite different names*

### Comparing `inductor-0.3.8/inductor/util.py` & `inductor-0.3.9/inductor/util.py`

 * *Files identical despite different names*

### Comparing `inductor-0.3.8/inductor/wire_model.py` & `inductor-0.3.9/inductor/wire_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,32 @@
     """
     model_config = pydantic.ConfigDict(extra="forbid")
 
     inputs: Dict[str, Any]
     output: Optional[Any] = None
     description: Optional[str] = None
 
+    # Define a custom constructor to enable taking `inputs` as a positional,
+    # rather than keyword-only, argument.
+    def __init__(
+        self,
+        inputs: Dict[str, Any],
+        *,
+        output: Optional[Any] = None,
+        description: Optional[str] = None):
+        """Constructs a new test case.
+
+        Args:
+            inputs: Mapping from input parameter name to input value.
+            output: Optionally, an example of a desired high-quality output, or
+                the output that is to be considered correct, for this test case.
+            description: Optionally, a description of this test case.
+        """
+        super().__init__(inputs=inputs, output=output, description=description)
+
 
 class QualityMeasure(pydantic.BaseModel):
     """A quality measure.
     
     Attributes:
         name: Human-readable name of this quality measure.
         evaluator: Evaluator for this quality measure.  Determines whether
@@ -84,14 +102,32 @@
     """
     model_config = pydantic.ConfigDict(extra="forbid")
 
     hparam_name: str = _SUBRESOURCE_NAME_FIELD
     hparam_type: Literal["SHORT_STRING", "TEXT", "NUMBER"]
     values: List[Any]
 
+    # Define a custom constructor to enable taking `hparam_name` and
+    # `hparam_type` as `name` and `type`, respectively, within the user-facing
+    # Python API.
+    def __init__(
+        self,
+        *,
+        name: str,
+        type: Literal["SHORT_STRING", "TEXT", "NUMBER"],
+        values: List[Any]):
+        """Constructs a new hyperparameter specification.
+
+        Args:
+            name: Name of hyperparameter.
+            type: Type of hyperparameter.
+            values: List of hyperparameter values.
+        """
+        super().__init__(hparam_name=name, hparam_type=type, values=values)
+
 
 class ProgramDetails(pydantic.BaseModel):
     """Details of an LLM program.
 
     Attributes:
         fully_qualified_name: Fully qualified name of the LLM program.
         inputs_signature:  Map between input parameter names to strings
```

### Comparing `inductor-0.3.8/inductor/cli/cli.py` & `inductor-0.3.9/inductor/cli/cli.py`

 * *Files identical despite different names*

### Comparing `inductor-0.3.8/inductor/cli/data_model.py` & `inductor-0.3.9/inductor/cli/data_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -353,16 +353,19 @@
             elif key in [
                 "quality", "quality measure", "quality_measure", "measure"]:
                 quality_measure = wire_model.QualityMeasure(**value)
                 test_suite_file_args["quality_measures"].append(
                     quality_measure)
 
             elif key in ["hparam", "hparam spec", "hparam_spec"]:
-                for k in ["name", "type"]:
-                    value[f"hparam_{k}"] = value.pop(k)
+                # Disable the following field renaming for now, due to
+                # modification of wire_model.HparamSpec's constructor to
+                # support its direct usage within user-facing Python API.
+                # for k in ["name", "type"]:
+                #     value[f"hparam_{k}"] = value.pop(k)
 
                 hparam_spec = wire_model.HparamSpec(**value)
                 test_suite_file_args.setdefault("hparam_specs", []).append(
                     hparam_spec)
 
             elif key in ["config", "configuration"]:
                 if includes_config and config_found:
```

### Comparing `inductor-0.3.8/inductor/cli/execute.py` & `inductor-0.3.9/inductor/cli/execute.py`

 * *Files identical despite different names*

### Comparing `inductor-0.3.8/inductor/cli/questions.py` & `inductor-0.3.9/inductor/cli/questions.py`

 * *Files identical despite different names*

### Comparing `inductor-0.3.8/pyproject.toml` & `inductor-0.3.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "inductor"
 description = "The Inductor CLI and client library"
-version = "0.3.8"
+version = "0.3.9"
 requires-python = ">=3.7"
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = [
     "auth0-python>=4.4.2,<5",
     "pydantic-settings>=2.0.3,<3",
     "python-multipart>=0.0.6,<1",
     "requests>=2.31.0,<3",
```

### Comparing `inductor-0.3.8/PKG-INFO` & `inductor-0.3.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inductor
-Version: 0.3.8
+Version: 0.3.9
 Summary: The Inductor CLI and client library
 Project-URL: Homepage, https://inductor.ai
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: auth0-python<5,>=4.4.2
 Requires-Dist: httpx<1,>=0.25.0
 Requires-Dist: inquirer<4,>=3.1.3
```

