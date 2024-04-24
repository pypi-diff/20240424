# Comparing `tmp/cdk_pyproject-0.1.1.tar.gz` & `tmp/cdk_pyproject-0.1.2.tar.gz`

## Comparing `cdk_pyproject-0.1.1.tar` & `cdk_pyproject-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.1/.python-version
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.1/requirements-dev.lock
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.1/requirements.lock
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.1/src/cdk_pyproject/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.1/src/cdk_pyproject/py.typed
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.1/src/cdk_pyproject/py_project.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.1/src/cdk_pyproject/dockerfiles/rye.Dockerfile
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.1/LICENSE
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.1/README.md
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.2/.python-version
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.2/requirements-dev.lock
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.2/requirements.lock
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.2/src/cdk_pyproject/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.2/src/cdk_pyproject/py.typed
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.2/src/cdk_pyproject/py_project.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.2/src/cdk_pyproject/dockerfiles/pyproject.Dockerfile
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.2/src/cdk_pyproject/dockerfiles/rye.Dockerfile
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.2/LICENSE
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.2/README.md
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 cdk_pyproject-0.1.2/PKG-INFO
```

### Comparing `cdk_pyproject-0.1.1/requirements-dev.lock` & `cdk_pyproject-0.1.2/requirements-dev.lock`

 * *Files 26% similar despite different names*

```diff
@@ -27,21 +27,25 @@
     # via jsii
 jsii==1.97.0
     # via aws-cdk-asset-awscli-v1
     # via aws-cdk-asset-kubectl-v20
     # via aws-cdk-asset-node-proxy-agent-v6
     # via aws-cdk-lib
     # via constructs
+packaging==24.0
+    # via pyproject-metadata
 publication==0.0.3
     # via aws-cdk-asset-awscli-v1
     # via aws-cdk-asset-kubectl-v20
     # via aws-cdk-asset-node-proxy-agent-v6
     # via aws-cdk-lib
     # via constructs
     # via jsii
+pyproject-metadata==0.8.0
+    # via cdk-pyproject
 python-dateutil==2.9.0.post0
     # via jsii
 six==1.16.0
     # via python-dateutil
 typeguard==2.13.3
     # via aws-cdk-asset-awscli-v1
     # via aws-cdk-asset-kubectl-v20
```

### Comparing `cdk_pyproject-0.1.1/requirements.lock` & `cdk_pyproject-0.1.2/requirements.lock`

 * *Files 26% similar despite different names*

```diff
@@ -27,21 +27,25 @@
     # via jsii
 jsii==1.97.0
     # via aws-cdk-asset-awscli-v1
     # via aws-cdk-asset-kubectl-v20
     # via aws-cdk-asset-node-proxy-agent-v6
     # via aws-cdk-lib
     # via constructs
+packaging==24.0
+    # via pyproject-metadata
 publication==0.0.3
     # via aws-cdk-asset-awscli-v1
     # via aws-cdk-asset-kubectl-v20
     # via aws-cdk-asset-node-proxy-agent-v6
     # via aws-cdk-lib
     # via constructs
     # via jsii
+pyproject-metadata==0.8.0
+    # via cdk-pyproject
 python-dateutil==2.9.0.post0
     # via jsii
 six==1.16.0
     # via python-dateutil
 typeguard==2.13.3
     # via aws-cdk-asset-awscli-v1
     # via aws-cdk-asset-kubectl-v20
```

### Comparing `cdk_pyproject-0.1.1/src/cdk_pyproject/py_project.py` & `cdk_pyproject-0.1.2/src/cdk_pyproject/py_project.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,58 @@
 import importlib.resources
 import os.path
+import tomllib
+from pathlib import Path
 from typing import Self
 
 from aws_cdk import BundlingOptions, DockerImage, aws_lambda
+from pyproject_metadata import StandardMetadata
 
 dockerfiles = importlib.resources.files("cdk_pyproject.dockerfiles")
 
 
 class PyProject:
-    def __init__(self, runtime: aws_lambda.Runtime, image: DockerImage) -> None:
+    def __init__(self, path: str, runtime: aws_lambda.Runtime, image: DockerImage) -> None:
         self.runtime = runtime
         self.image = image
+        self.path = path
 
     @classmethod
-    def from_rye(cls, runtime: aws_lambda.Runtime, path: str) -> Self:
+    def from_pyproject(cls, path: str, runtime: aws_lambda.Runtime) -> Self:
+        image = DockerImage.from_build(
+            path=path,
+            build_args={"IMAGE": runtime.bundling_image.image},
+            file=os.path.relpath(str(dockerfiles.joinpath("pyproject.Dockerfile")), start=path),
+        )
+
+        return cls(path, runtime, image)
+
+    @classmethod
+    def from_rye(cls, path: str, runtime: aws_lambda.Runtime) -> Self:
         image = DockerImage.from_build(
             path=path,
             build_args={"IMAGE": runtime.bundling_image.image},
             file=os.path.relpath(str(dockerfiles.joinpath("rye.Dockerfile")), start=path),
         )
 
-        return cls(runtime=runtime, image=image)
+        return cls(path, runtime, image)
+
+    @classmethod
+    def from_poetry(cls, path: str, runtime: aws_lambda.Runtime) -> Self:
+        raise NotImplementedError
+
+    def get_root_project_name(self) -> str:
+        pyproject = Path(self.path, "pyproject.toml")
+        metadata = StandardMetadata.from_pyproject(tomllib.loads(pyproject.read_text()))
+        return metadata.name
+
+    def code(self, project: str | None) -> aws_lambda.Code:
+        if project is None:
+            project = self.get_root_project_name()
 
-    def code(self, project: str) -> aws_lambda.Code:
         return aws_lambda.Code.from_asset(
             path=".",
             bundling=BundlingOptions(
                 image=self.image,
                 command=[
                     "bash",
                     "-eux",
```

### Comparing `cdk_pyproject-0.1.1/src/cdk_pyproject/dockerfiles/rye.Dockerfile` & `cdk_pyproject-0.1.2/src/cdk_pyproject/dockerfiles/rye.Dockerfile`

 * *Files identical despite different names*

### Comparing `cdk_pyproject-0.1.1/LICENSE` & `cdk_pyproject-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk_pyproject-0.1.1/pyproject.toml` & `cdk_pyproject-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "cdk-pyproject"
+version = "0.1.2"
 description = "Add your description here"
 authors = [{ name = "Masaki Kobayashi", email = "bayashi.cl@gmail.com" }]
-dependencies = ["aws-cdk-lib>=2.138.0"]
+dependencies = ["aws-cdk-lib>=2.138.0", "pyproject-metadata>=0.8.0"]
 readme = "README.md"
 requires-python = ">= 3.12"
-dynamic = ["version"]
 
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
 
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.12",
```

### Comparing `cdk_pyproject-0.1.1/PKG-INFO` & `cdk_pyproject-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.3
 Name: cdk-pyproject
-Version: 0.1.1
+Version: 0.1.2
 Summary: Add your description here
 Project-URL: Source, https://github.com/bayashi-cl/cdk-pyproject/
 Author-email: Masaki Kobayashi <bayashi.cl@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AWS CDK
 Classifier: Framework :: AWS CDK :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12
 Requires-Dist: aws-cdk-lib>=2.138.0
+Requires-Dist: pyproject-metadata>=0.8.0
 Description-Content-Type: text/markdown
 
 # cdk-pyproject
 
 Describe your project here.
```

