# Comparing `tmp/miniscons-0.10.1.tar.gz` & `tmp/miniscons-0.6.0.tar.gz`

## Comparing `miniscons-0.10.1.tar` & `miniscons-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 miniscons-0.10.1/src/__init__.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 miniscons-0.10.1/src/build.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 miniscons-0.10.1/src/compiler.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 miniscons-0.10.1/src/containers.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 miniscons-0.10.1/src/environment.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 miniscons-0.10.1/src/flag.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 miniscons-0.10.1/src/routine.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 miniscons-0.10.1/src/script.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 miniscons-0.10.1/src/target.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 miniscons-0.10.1/src/tasks.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 miniscons-0.10.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 miniscons-0.10.1/LICENSE.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 miniscons-0.10.1/README.md
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 miniscons-0.10.1/pyproject.toml
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 miniscons-0.10.1/PKG-INFO
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/models/__init__.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/models/tasks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/models/builds/__init__.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/models/builds/build.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/models/builds/target.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/models/scripts/__init__.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/models/scripts/flag.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/models/scripts/routine.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/models/scripts/script.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/services/__init__.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/services/compiler.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 miniscons-0.6.0/src/services/environment.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 miniscons-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 miniscons-0.6.0/LICENSE.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 miniscons-0.6.0/README.md
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 miniscons-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 miniscons-0.6.0/PKG-INFO
```

### Comparing `miniscons-0.10.1/src/target.py` & `miniscons-0.6.0/src/models/builds/target.py`

 * *Files identical despite different names*

### Comparing `miniscons-0.10.1/src/tasks.py` & `miniscons-0.6.0/src/models/tasks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import sys
-from .build import Build
-from .flag import Flag
-from .routine import Routine
-from .script import Script
-from .target import Target
+from .builds.build import Build
+from .scripts.flag import Flag
+from .scripts.routine import Routine
+from .scripts.script import Script
+from .builds.target import Target
 from dataclasses import dataclass, field
 from SCons.Environment import Environment
 
 
 @dataclass
 class Tasks:
-    builds: list[Build] = field(default_factory=list)
+    builds: list[Build]
+
     targets: list[Target] = field(default_factory=list)
     scripts: list[Script] = field(default_factory=list)
     routines: list[Routine] = field(default_factory=list)
     flags: list[Flag] = field(default_factory=list)
 
-    @property
-    def cli(self) -> str:
+    def __str__(self) -> str:
         fields = "\n\n".join(
             [
                 ":".join(
                     [k, "".join([f"\n  {i}" for i in v] if len(v) > 0 else "\n  -")]
                 )
                 for k, v in self.__dict__.items()
             ]
         )
 
         return f"\n{fields}\n"
 
     def dump(self) -> None:
-        sys.stdout.write(f"{self.cli}\n")
+        sys.stdout.write(f"{self}\n")
 
     def register(self, env: Environment) -> None:
         for group in self.__dict__.values():
             for task in group:
                 task.register(env)
```

### Comparing `miniscons-0.10.1/LICENSE.md` & `miniscons-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `miniscons-0.10.1/pyproject.toml` & `miniscons-0.6.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,71 +1,60 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "miniscons"
 description = "SCons builders."
-version = "0.10.1"
+version = "0.6.0"
 
 keywords = ["SCons", "SConstruct", "builders"]
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 requires-python = ">=3.8"
-dependencies = ["emoji==1.7.0", "psutil==5.9.1", "SCons==4.3.0"]
+dependencies = ["SCons==4.3.0"]
 
 [project.optional-dependencies]
 all = [
     "autoflake==1.4",
     "black==22.3.0",
     "build==1.2.1",
     "bump2version==1.0.1",
-    "furo==2024.1.29",
     "isort==5.10.1",
-    "matplotlib==3.8.4",
     "mypy==0.961",
-    "myst-parser==2.0.0",
     "pylint==2.17.0",
-    "pytest-cov==5.0.0",
     "pytest==7.1.2",
-    "sphinx-autoapi==3.0.0",
-    "Sphinx==7.2.6",
-    "sphinxext-opengraph==0.9.1",
-    "thx==0.5.1",
+    "pytest-cov==5.0.0",
     "trufflehog3==3.0.7",
     "twine==5.0.0",
-    "types-emoji==2.1.0.3",
-    "walkmate==1.5.0",
+    "thx==0.5.1",
 ]
 
 [project.license]
-name = "MIT"
 file = "LICENSE.md"
-content-type = "text/markdown"
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.urls]
-homepage = "https://joellefkowitz.github.io/miniscons"
-repository = "https://github.com/JoelLefkowitz/miniscons"
+Homepage = "https://github.com/JoelLefkowitz/miniscons"
 
 [[project.authors]]
 name = "Joel Lefkowitz"
 email = "joellefkowitz@hotmail.com"
 
-[tool.metadata]
+[tool.promoter.metadata]
 publisher = "PyPI"
 languages = ["Python"]
 frameworks = ["SCons"]
 paradigms = ["Object oriented"]
 lifecycle = "Alpha"
 
 [tool.hatch.build.targets.sdist]
@@ -76,26 +65,19 @@
 
 [tool.hatch.build.targets.wheel.sources]
 src = "miniscons"
 
 [tool.thx.jobs]
 lint = [
     "npx cspell . --dot",
-    "pylint src --disable=C0114,C0115,C0116,C0411,C3001",
+    "pylint src --disable=C0114,C0115,C0116,C0411",
     "mypy -m src --ignore-missing-import",
-    "trufflehog3",
 ]
 
 format = [
     "black .",
     "isort . --no-sections --remove-redundant-aliases",
     "npx prettier . --write",
 ]
 
 test = "pytest . --doctest-modules --cov --cov-report=xml"
-docs = "sphinx-build docs/sphinx docs/dist"
-
-[tool.coverage.run]
-data_file = "coverage/.coverage"
-
-[tool.coverage.xml]
-output = "coverage/cobertura.xml"
+docs = "doxygen"
```

### Comparing `miniscons-0.10.1/PKG-INFO` & `miniscons-0.6.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.3
 Name: miniscons
-Version: 0.10.1
+Version: 0.6.0
 Summary: SCons builders.
-Project-URL: homepage, https://joellefkowitz.github.io/miniscons
-Project-URL: repository, https://github.com/JoelLefkowitz/miniscons
+Project-URL: Homepage, https://github.com/JoelLefkowitz/miniscons
 Author-email: Joel Lefkowitz <joellefkowitz@hotmail.com>
 License: # MIT License
         
         Copyright (c) 2024 Joel Lefkowitz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -29,36 +28,26 @@
 Keywords: SCons,SConstruct,builders
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
-Requires-Dist: emoji==1.7.0
-Requires-Dist: psutil==5.9.1
 Requires-Dist: scons==4.3.0
 Provides-Extra: all
 Requires-Dist: autoflake==1.4; extra == 'all'
 Requires-Dist: black==22.3.0; extra == 'all'
 Requires-Dist: build==1.2.1; extra == 'all'
 Requires-Dist: bump2version==1.0.1; extra == 'all'
-Requires-Dist: furo==2024.1.29; extra == 'all'
 Requires-Dist: isort==5.10.1; extra == 'all'
-Requires-Dist: matplotlib==3.8.4; extra == 'all'
 Requires-Dist: mypy==0.961; extra == 'all'
-Requires-Dist: myst-parser==2.0.0; extra == 'all'
 Requires-Dist: pylint==2.17.0; extra == 'all'
 Requires-Dist: pytest-cov==5.0.0; extra == 'all'
 Requires-Dist: pytest==7.1.2; extra == 'all'
-Requires-Dist: sphinx-autoapi==3.0.0; extra == 'all'
-Requires-Dist: sphinx==7.2.6; extra == 'all'
-Requires-Dist: sphinxext-opengraph==0.9.1; extra == 'all'
 Requires-Dist: thx==0.5.1; extra == 'all'
 Requires-Dist: trufflehog3==3.0.7; extra == 'all'
 Requires-Dist: twine==5.0.0; extra == 'all'
-Requires-Dist: types-emoji==2.1.0.3; extra == 'all'
-Requires-Dist: walkmate==1.5.0; extra == 'all'
 Description-Content-Type: text/markdown
 
 # Miniscons
 
 SCons builders.
```

