# Comparing `tmp/pyVersioning-0.8.0.tar.gz` & `tmp/pyVersioning-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyVersioning-0.8.0.tar", last modified: Mon Jan 10 20:57:29 2022, max compression
+gzip compressed data, was "pyVersioning-0.9.0.tar", last modified: Wed Feb  8 21:26:44 2023, max compression
```

## Comparing `pyVersioning-0.8.0.tar` & `pyVersioning-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 20:57:29.840297 pyVersioning-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    10571 2022-01-10 20:57:20.000000 pyVersioning-0.8.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     4573 2022-01-10 20:57:29.840297 pyVersioning-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3358 2022-01-10 20:57:20.000000 pyVersioning-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 20:57:29.840297 pyVersioning-0.8.0/pyVersioning/
--rw-r--r--   0 runner    (1001) docker     (121)     4468 2022-01-10 20:57:20.000000 pyVersioning-0.8.0/pyVersioning/AppVeyor.py
--rw-r--r--   0 runner    (1001) docker     (121)     5387 2022-01-10 20:57:20.000000 pyVersioning-0.8.0/pyVersioning/CIService.py
--rw-r--r--   0 runner    (1001) docker     (121)     5878 2022-01-10 20:57:20.000000 pyVersioning-0.8.0/pyVersioning/Configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     4580 2022-01-10 20:57:20.000000 pyVersioning-0.8.0/pyVersioning/GitHub.py
--rw-r--r--   0 runner    (1001) docker     (121)     4661 2022-01-10 20:57:20.000000 pyVersioning-0.8.0/pyVersioning/GitLab.py
--rw-r--r--   0 runner    (1001) docker     (121)     4425 2022-01-10 20:57:20.000000 pyVersioning-0.8.0/pyVersioning/Travis.py
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-01-10 20:57:20.000000 pyVersioning-0.8.0/pyVersioning/Utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    15385 2022-01-10 20:57:20.000000 pyVersioning-0.8.0/pyVersioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11800 2022-01-10 20:57:20.000000 pyVersioning-0.8.0/pyVersioning/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 20:57:29.840297 pyVersioning-0.8.0/pyVersioning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4573 2022-01-10 20:57:29.000000 pyVersioning-0.8.0/pyVersioning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-01-10 20:57:29.000000 pyVersioning-0.8.0/pyVersioning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-10 20:57:29.000000 pyVersioning-0.8.0/pyVersioning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-01-10 20:57:29.000000 pyVersioning-0.8.0/pyVersioning.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-01-10 20:57:29.000000 pyVersioning-0.8.0/pyVersioning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-01-10 20:57:29.000000 pyVersioning-0.8.0/pyVersioning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-01-10 20:57:20.000000 pyVersioning-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-10 20:57:29.840297 pyVersioning-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4217 2022-01-10 20:57:20.000000 pyVersioning-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:26:44.832302 pyVersioning-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-02-08 21:26:33.000000 pyVersioning-0.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-02-08 21:26:44.832302 pyVersioning-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-02-08 21:26:33.000000 pyVersioning-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:26:44.832302 pyVersioning-0.9.0/pyVersioning/
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-02-08 21:26:33.000000 pyVersioning-0.9.0/pyVersioning/AppVeyor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-02-08 21:26:33.000000 pyVersioning-0.9.0/pyVersioning/CIService.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-02-08 21:26:33.000000 pyVersioning-0.9.0/pyVersioning/Configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-02-08 21:26:33.000000 pyVersioning-0.9.0/pyVersioning/GitHub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-02-08 21:26:33.000000 pyVersioning-0.9.0/pyVersioning/GitLab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-02-08 21:26:33.000000 pyVersioning-0.9.0/pyVersioning/Travis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-02-08 21:26:33.000000 pyVersioning-0.9.0/pyVersioning/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16762 2023-02-08 21:26:33.000000 pyVersioning-0.9.0/pyVersioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13627 2023-02-08 21:26:33.000000 pyVersioning-0.9.0/pyVersioning/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:26:44.832302 pyVersioning-0.9.0/pyVersioning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-02-08 21:26:44.000000 pyVersioning-0.9.0/pyVersioning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-08 21:26:44.000000 pyVersioning-0.9.0/pyVersioning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 21:26:44.000000 pyVersioning-0.9.0/pyVersioning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-08 21:26:44.000000 pyVersioning-0.9.0/pyVersioning.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-02-08 21:26:44.000000 pyVersioning-0.9.0/pyVersioning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-08 21:26:44.000000 pyVersioning-0.9.0/pyVersioning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-02-08 21:26:33.000000 pyVersioning-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 21:26:44.832302 pyVersioning-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-02-08 21:26:33.000000 pyVersioning-0.9.0/setup.py
```

### Comparing `pyVersioning-0.8.0/LICENSE.md` & `pyVersioning-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyVersioning-0.8.0/PKG-INFO` & `pyVersioning-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: pyVersioning
-Version: 0.8.0
+Version: 0.9.0
 Summary: Write version information for any programming language as source file.
 Home-page: https://GitHub.com/Paebbels/pyVersioning
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://Paebbels.GitHub.io/pyVersioning
 Project-URL: Source Code, https://GitHub.com/Paebbels/pyVersioning
 Project-URL: Issue Tracker, https://GitHub.com/Paebbels/pyVersioning/issues
 Keywords: Python3,Template,Versioning,Git
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE.md
 
 [![Sourcecode on GitHub](https://img.shields.io/badge/Paebbels-pyVersioning-323131.svg?logo=github&longCache=true)](https://github.com/Paebbels/pyVersioning)
 [![License](https://img.shields.io/badge/code%20license-Apache%20License%2C%202.0-lightgrey?logo=GitHub)](LICENSE.md)
@@ -87,9 +86,7 @@
 
 <!-- The accompanying documentation is licensed under Creative Commons - Attribution-4.0 (CC-BY 4.0). -->
 
 
 -------------------------
 
 SPDX-License-Identifier: Apache-2.0
-
-
```

### Comparing `pyVersioning-0.8.0/README.md` & `pyVersioning-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pyVersioning-0.8.0/pyVersioning/AppVeyor.py` & `pyVersioning-0.9.0/pyVersioning/AppVeyor.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                          |___/                                                          #
 # ==================================================================================================================== #
 # Authors:                                                                                                             #
 #   Patrick Lehmann                                                                                                    #
 #                                                                                                                      #
 # License:                                                                                                             #
 # ==================================================================================================================== #
-# Copyright 2020-2021 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2020-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
 #                                                                                                                      #
@@ -27,17 +27,20 @@
 #                                                                                                                      #
 # SPDX-License-Identifier: Apache-2.0                                                                                  #
 # ==================================================================================================================== #
 #
 """AppVeyor specific code to collect the build environment."""
 from os import environ
 
+from pyTooling.Decorators import export
+
 from pyVersioning.CIService import CIService, Platform, ServiceException
 
 
+@export
 class AppVeyor(CIService):
 	ENV_INCLUDE_FILTER =  ("APPVEYOR_")
 	ENV_EXCLUDE_FILTER =  ("_TOKEN")
 	ENV_INCLUDES =        ['CI', 'APPVEYOR', 'PLATFORM', 'CONFIGURATION']
 	ENV_EXCLUDES =        []
 
 	def getPlatform(self) -> Platform:
```

### Comparing `pyVersioning-0.8.0/pyVersioning/CIService.py` & `pyVersioning-0.9.0/pyVersioning/CIService.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                          |___/                                                          #
 # ==================================================================================================================== #
 # Authors:                                                                                                             #
 #   Patrick Lehmann                                                                                                    #
 #                                                                                                                      #
 # License:                                                                                                             #
 # ==================================================================================================================== #
-# Copyright 2020-2021 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2020-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
 #                                                                                                                      #
@@ -28,40 +28,54 @@
 # SPDX-License-Identifier: Apache-2.0                                                                                  #
 # ==================================================================================================================== #
 #
 """Module for CI service base classes."""
 from dataclasses  import make_dataclass, dataclass
 from datetime     import datetime
 from os           import environ
+
+from pyTooling.MetaClasses import ExtendedType, abstractmethod
 from typing       import Dict
 
+from pyTooling.Decorators import export
+
 from pyVersioning import SelfDescriptive
 
 
+@export
 class ServiceException(Exception):
-	pass
+	""".. todo:: ServiceException needs documentation"""
 
 
+@export
 @dataclass
 class Platform(SelfDescriptive):
-	ci_service : str
+	""".. todo:: Platform needs documentation"""
+
+	ci_service: str
 
 	_public = ['ci_service']
 
 
-class CIService:
+@export
+class CIService(metaclass=ExtendedType):
+	""".. todo:: CIService needs documentation"""
+
 	ENV_INCLUDE_FILTER =  ()
 	ENV_EXCLUDE_FILTER =  ()
 	ENV_INCLUDES =        []
 	ENV_EXCLUDES =        []
 
+	@abstractmethod
 	def getPlatform(self) -> Platform:
-		raise NotImplementedError()
+		""".. todo:: getPlatform needs documentation"""
 
 	def getEnvironment(self) -> Dict[str, str]:
+		""".. todo:: getEnvironment needs documentation"""
+
 		filteredEnv = {key:value for (key,value) in environ.items() if key.startswith(self.ENV_INCLUDE_FILTER) and not key.endswith(self.ENV_EXCLUDE_FILTER)}
 
 		# manually add some variables
 		for key in self.ENV_INCLUDES:
 			try:
 				filteredEnv[key] = environ[key]
 			except KeyError:
@@ -88,26 +102,32 @@
 				'KeyValuePairs':  lambda self: func(self)
 			},
 			repr=True
 		)
 
 		return Environment(**filteredEnv)
 
+	@abstractmethod
 	def getGitHash(self) -> str:
-		raise NotImplementedError()
+		""".. todo:: getGithash needs documentation"""
 
+	@abstractmethod
 	def getCommitDate(self) -> datetime:
-		raise NotImplementedError()
+		""".. todo:: getCommitDate needs documentation"""
 
+	@abstractmethod
 	def getGitBranch(self) -> str:
-		raise NotImplementedError()
+		""".. todo:: getGitBranch needs documentation"""
 
+	@abstractmethod
 	def getGitTag(self) -> str:
-		raise NotImplementedError()
+		""".. todo:: getGitTag needs documentation"""
 
+	@abstractmethod
 	def getGitRepository(self) -> str:
-		raise NotImplementedError()
+		""".. todo:: getGitRepository needs documentation"""
 
 
+@export
 class WorkStation(CIService):
 	def getPlatform(self) -> Platform:
 		return Platform("NO-CI")
```

### Comparing `pyVersioning-0.8.0/pyVersioning/Configuration.py` & `pyVersioning-0.9.0/pyVersioning/Configuration.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                          |___/                                                          #
 # ==================================================================================================================== #
 # Authors:                                                                                                             #
 #   Patrick Lehmann                                                                                                    #
 #                                                                                                                      #
 # License:                                                                                                             #
 # ==================================================================================================================== #
-# Copyright 2020-2021 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2020-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
 #                                                                                                                      #
@@ -25,99 +25,99 @@
 # See the License for the specific language governing permissions and                                                  #
 # limitations under the License.                                                                                       #
 #                                                                                                                      #
 # SPDX-License-Identifier: Apache-2.0                                                                                  #
 # ==================================================================================================================== #
 #
 """pyVersioning configuration file in YAML format."""
-from pathlib        import WindowsPath, PosixPath
-from typing         import Dict
+from pathlib               import Path
+from typing                import Dict, Optional as Nullable
 
-from pyTooling.MetaClasses  import Overloading
-from ruamel.yaml            import YAML
+from ruamel.yaml           import YAML
+from pyTooling.Decorators  import export
+from pyTooling.MetaClasses import ExtendedType
+from pyTooling.Versioning  import SemVersion
+
+
+@export
+class Base:
+	root:   'Base'
+	parent: Nullable['Base']
 
-from pyTooling.Versioning   import SemVersion
-
-
-class Base():
-	root:   'Base' =  None
-	parent: 'Base' =  None
-
-	def __init__(self, root: 'Base', parent: 'Base'):
-		self.root =   root
+	def __init__(self, root: 'Base', parent: Nullable['Base']):
+		self.root = root
 		self.parent = parent
 
-class Configuration(Base, metaclass=Overloading):
+
+@export
+class Configuration(Base, metaclass=ExtendedType):
 	class Project(Base):
-		name    : str     = None
-		variant : str     = None
-		version : SemVersion = None
+		name:    str
+		variant: str
+		version: SemVersion
 
 		def __init__(self, root: 'Base', parent: 'Base', settings: Dict):
 			super().__init__(root, parent)
 
-			self.name     = settings['name']
-			if 'variant' in settings:
-				self.variant  = settings['variant']
-			if 'version' in settings:
-				self.version  = SemVersion(settings['version'])
+			self.name =    settings["name"]
+			self.variant = settings["variant"] if "variant" in settings else None
+			self.version = SemVersion(settings["version"]) if "version" in settings else None
 
 	class Build(Base):
 		class Compiler(Base):
-			name          : str = None
-			version       : str = None
-			configuration : str = None
-			options       : str = None
+			name:          str
+			version:       str
+			configuration: str
+			options:       str
 
 			def __init__(self, root: 'Base', parent: 'Base', settings: Dict):
 				super().__init__(root, parent)
 
-				self.name          = settings['name']
-				self.version       = settings['version']
-				self.configuration = settings['configuration']
-				self.options       = settings['options']
+				self.name =          settings["name"]
+				self.version =       settings["version"]
+				self.configuration = settings["configuration"]
+				self.options =       settings["options"]
 
-		compiler : Compiler = None
+		compiler: Compiler
 
 		def __init__(self, root: 'Base', parent: 'Base', settings: Dict):
 			super().__init__(root, parent)
 
-			if ('compiler' in settings):
-				self.compiler = self.Compiler(root, self, settings['compiler'])
-
-
-	version : int =     None
-	project : Project = None
-	build   : Build =   None
+			self.compiler = self.Compiler(root, self, settings["compiler"]) if "compiler" in settings else None
 
-	def __init__(self):
-		self.version = 1
-		self.project = self.Project(self, self, {
-			"name": "",
-			"variant": "",
-			"version": "v0.0.0"
-		})
+	version: int
+	project: Project
+	build:   Build
 
-	def __init__(self, configFile: PosixPath):
-		self.load(configFile)
+	def __init__(self, configFile: Path = None):
+		super().__init__(self, None)
 
-	def __init__(self, configFile: WindowsPath):
-		self.load(configFile)
+		if configFile is None:
+			self.version = 1
+			self.project = self.Project(self, self, {
+				"name":    "",
+				"variant": "",
+				"version": "v0.0.0"
+			})
+			self.build = self.Build(self, self, {
+				"compiler": {
+					"name": "",
+					"version": "v0.0.0",
+					"configuration": "",
+					"options": ""
+				}
+			})
+		else:
+			self.load(configFile)
 
-	def load(self, configFile):
+	def load(self, configFile: Path):
 		yaml =   YAML()
 		config = yaml.load(configFile)
 
-		if 'version' in config:
-			self.version = int(config['version'])
-		else:
-			self.version = 1
+		self.version = int(config["version"]) if "version" in config else 1
 
 		if self.version == 1:
 			self.loadVersion1(config)
 
 	def loadVersion1(self, config):
-		if 'project' in config:
-			self.project = self.Project(self, self, config['project'])
-
-		if 'build' in config:
-			self.build = self.Build(self, self, config['build'])
+		self.project = self.Project(self, self, config["project"]) if "project" in config else None
+		self.build =   self.Build(self, self, config["build"])     if "build" in config   else None
```

### Comparing `pyVersioning-0.8.0/pyVersioning/GitHub.py` & `pyVersioning-0.9.0/pyVersioning/GitLab.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                          |___/                                                          #
 # ==================================================================================================================== #
 # Authors:                                                                                                             #
 #   Patrick Lehmann                                                                                                    #
 #                                                                                                                      #
 # License:                                                                                                             #
 # ==================================================================================================================== #
-# Copyright 2020-2021 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2020-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
 #                                                                                                                      #
@@ -24,57 +24,61 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.                                             #
 # See the License for the specific language governing permissions and                                                  #
 # limitations under the License.                                                                                       #
 #                                                                                                                      #
 # SPDX-License-Identifier: Apache-2.0                                                                                  #
 # ==================================================================================================================== #
 #
-"""GitHub specific code to collect the build environment."""
-from os import environ
+"""GitLab specific code to collect the build environment."""
+from datetime import datetime
+from os       import environ
+from typing   import Optional as Nullable
+
+from pyTooling.Decorators   import export
 
 from pyVersioning.CIService import CIService, Platform, ServiceException
 
 
-class GitHub(CIService):
-	ENV_INCLUDE_FILTER =  ("GITHUB_")
-	ENV_EXCLUDE_FILTER =  ("_TOKEN")
-	ENV_INCLUDES =        ['CI']
-	ENV_EXCLUDES =        []
+@export
+class GitLab(CIService):
+	ENV_INCLUDE_FILTER = ("CI_", "GITLAB_")
+	ENV_EXCLUDE_FILTER = ("_TOKEN", )
+	ENV_INCLUDES =       ('CI', )
+	ENV_EXCLUDES =       ('CI_JOB_TOKEN', )
 
 	def getPlatform(self) -> Platform:
-		return Platform("github")
+		return Platform("gitlab")
 
 	def getGitHash(self) -> str:
 		try:
-			return environ['GITHUB_SHA']
+			return environ['CI_COMMIT_SHA']
 		except KeyError as ex:
 			raise ServiceException from ex
 
-	def getGitBranch(self) -> str:
-		branchPrefix = "refs/heads/"
+	def getCommitDate(self) -> datetime:
+		try:
+			iso8601 = environ['CI_COMMIT_TIMESTAMP']
+			return datetime.strptime(iso8601, "%Y-%m-%dT%H:%M:%S%z")
+		except KeyError as ex:
+			raise ServiceException from ex
 
+	def getGitBranch(self) -> Nullable[str]:
 		try:
-			ref = environ['GITHUB_REF']
-			if ref.startswith(branchPrefix):
-				return ref[len(branchPrefix):]
+			return environ['CI_COMMIT_BRANCH']
 		except KeyError:
 			pass
 
 		return None
 
-	def getGitTag(self) -> str:
-		tagPrefix    = "refs/tags/"
-
+	def getGitTag(self) -> Nullable[str]:
 		try:
-			ref = environ['GITHUB_REF']
-			if ref.startswith(tagPrefix):
-				return ref[len(tagPrefix):]
+			return environ['CI_COMMIT_TAG']
 		except KeyError:
 			pass
 
 		return None
 
 	def getGitRepository(self) -> str:
 		try:
-			return environ['GITHUB_REPOSITORY']
+			return environ['CI_REPOSITORY_URL']
 		except KeyError as ex:
 			raise ServiceException from ex
```

### Comparing `pyVersioning-0.8.0/pyVersioning/GitLab.py` & `pyVersioning-0.9.0/pyVersioning/GitHub.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                          |___/                                                          #
 # ==================================================================================================================== #
 # Authors:                                                                                                             #
 #   Patrick Lehmann                                                                                                    #
 #                                                                                                                      #
 # License:                                                                                                             #
 # ==================================================================================================================== #
-# Copyright 2020-2021 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2020-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
 #                                                                                                                      #
@@ -24,57 +24,61 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.                                             #
 # See the License for the specific language governing permissions and                                                  #
 # limitations under the License.                                                                                       #
 #                                                                                                                      #
 # SPDX-License-Identifier: Apache-2.0                                                                                  #
 # ==================================================================================================================== #
 #
-"""GitLab specific code to collect the build environment."""
-from datetime import datetime
-from os       import environ
+"""GitHub specific code to collect the build environment."""
+from os     import environ
+from typing import Optional as Nullable
+
+from pyTooling.Decorators import export
 
 from pyVersioning.CIService import CIService, Platform, ServiceException
 
 
-class GitLab(CIService):
-	ENV_INCLUDE_FILTER =  ("CI_", "GITLAB_")
-	ENV_EXCLUDE_FILTER =  ("_TOKEN")
-	ENV_INCLUDES =        ['CI']
-	ENV_EXCLUDES =        ['CI_JOB_TOKEN']
+@export
+class GitHub(CIService):
+	ENV_INCLUDE_FILTER =  ("GITHUB_", )
+	ENV_EXCLUDE_FILTER =  ("_TOKEN", )
+	ENV_INCLUDES =        ('CI', )
+	ENV_EXCLUDES =        []
 
 	def getPlatform(self) -> Platform:
-		return Platform("gitlab")
+		return Platform("github")
 
 	def getGitHash(self) -> str:
 		try:
-			return environ['CI_COMMIT_SHA']
+			return environ['GITHUB_SHA']
 		except KeyError as ex:
 			raise ServiceException from ex
 
-	def getCommitDate(self) -> datetime:
-		try:
-			iso8601 = environ['CI_COMMIT_TIMESTAMP']
-			return datetime.strptime(iso8601, "%Y-%m-%dT%H:%M:%S%z")
-		except KeyError as ex:
-			raise ServiceException from ex
+	def getGitBranch(self) -> Nullable[str]:
+		branchPrefix = "refs/heads/"
 
-	def getGitBranch(self) -> str:
 		try:
-			return environ['CI_COMMIT_BRANCH']
+			ref = environ['GITHUB_REF']
+			if ref.startswith(branchPrefix):
+				return ref[len(branchPrefix):]
 		except KeyError:
 			pass
 
 		return None
 
-	def getGitTag(self) -> str:
+	def getGitTag(self) -> Nullable[str]:
+		tagPrefix    = "refs/tags/"
+
 		try:
-			return environ['CI_COMMIT_TAG']
+			ref = environ['GITHUB_REF']
+			if ref.startswith(tagPrefix):
+				return ref[len(tagPrefix):]
 		except KeyError:
 			pass
 
 		return None
 
 	def getGitRepository(self) -> str:
 		try:
-			return environ['CI_REPOSITORY_URL']
+			return environ['GITHUB_REPOSITORY']
 		except KeyError as ex:
 			raise ServiceException from ex
```

### Comparing `pyVersioning-0.8.0/pyVersioning/Travis.py` & `pyVersioning-0.9.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                          |___/                                                          #
 # ==================================================================================================================== #
 # Authors:                                                                                                             #
 #   Patrick Lehmann                                                                                                    #
 #                                                                                                                      #
 # License:                                                                                                             #
 # ==================================================================================================================== #
-# Copyright 2020-2021 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2020-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
 #                                                                                                                      #
@@ -24,49 +24,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.                                             #
 # See the License for the specific language governing permissions and                                                  #
 # limitations under the License.                                                                                       #
 #                                                                                                                      #
 # SPDX-License-Identifier: Apache-2.0                                                                                  #
 # ==================================================================================================================== #
 #
-"""Travis  specific code to collect the build environment."""
-from os import environ
-
-from pyVersioning.CIService import CIService, Platform, ServiceException
-
-
-class Travis(CIService):
-	ENV_INCLUDE_FILTER =  ("TRAVIS_")
-	ENV_EXCLUDE_FILTER =  ("_TOKEN")
-	ENV_INCLUDES =        ['CI', 'CONTINUOUS_INTEGRATION', 'TRAVIS']
-	ENV_EXCLUDES =        []
-
-	def getPlatform(self) -> Platform:
-		return Platform("travis")
-
-	def getGitHash(self) -> str:
-		try:
-			return environ['TRAVIS_COMMIT']
-		except KeyError as ex:
-			raise ServiceException from ex
-
-	def getGitBranch(self) -> str:
-		try:
-			return environ['TRAVIS_BRANCH']
-		except KeyError:
-			pass
-
-		return None
-
-	def getGitTag(self) -> str:
-		try:
-			return environ['TRAVIS_TAG']
-		except KeyError:
-			pass
-
-		return None
-
-	def getGitRepository(self) -> str:
-		try:
-			return environ['TRAVIS_REPO_SLUG']
-		except KeyError as ex:
-			raise ServiceException from ex
+"""Package installer for 'Write version information for any programming language as source file'."""
+from pathlib             import Path
+from pyTooling.Packaging import DescribePythonPackageHostedOnGitHub
+
+gitHubNamespace =        "Paebbels"
+packageName =            "pyVersioning"
+packageDirectory =       packageName.replace(".", "/")
+packageInformationFile = Path(f"{packageDirectory}/__init__.py")
+
+DescribePythonPackageHostedOnGitHub(
+	packageName=packageName,
+	description="Write version information for any programming language as source file.",
+	gitHubNamespace=gitHubNamespace,
+	sourceFileWithVersion=packageInformationFile,
+  consoleScripts={
+    "pyVersioning": "pyVersioning.cli:main",
+  }
+)
```

### Comparing `pyVersioning-0.8.0/pyVersioning/__init__.py` & `pyVersioning-0.9.0/pyVersioning/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,131 +1,142 @@
-# =============================================================================
-#            __     __            _             _
-#  _ __  _   \ \   / /__ _ __ ___(_) ___  _ __ (_)_ __   __ _
-# | '_ \| | | \ \ / / _ \ '__/ __| |/ _ \| '_ \| | '_ \ / _` |
-# | |_) | |_| |\ V /  __/ |  \__ \ | (_) | | | | | | | | (_| |
-# | .__/ \__, | \_/ \___|_|  |___/_|\___/|_| |_|_|_| |_|\__, |
-# |_|    |___/                                          |___/
-# =============================================================================
-# Authors:            Patrick Lehmann
-#
-# Python package:     pyVersioning Implementation
-#
-# Description:
-# ------------------------------------
-#		TODO
-#
-# License:
-# ============================================================================
-# Copyright 2020-2021 Patrick Lehmann - Bötzingen, Germany
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# SPDX-License-Identifier: Apache-2.0
-# ============================================================================
+# ==================================================================================================================== #
+#            __     __            _             _                                                                      #
+#  _ __  _   \ \   / /__ _ __ ___(_) ___  _ __ (_)_ __   __ _                                                          #
+# | '_ \| | | \ \ / / _ \ '__/ __| |/ _ \| '_ \| | '_ \ / _` |                                                         #
+# | |_) | |_| |\ V /  __/ |  \__ \ | (_) | | | | | | | | (_| |                                                         #
+# | .__/ \__, | \_/ \___|_|  |___/_|\___/|_| |_|_|_| |_|\__, |                                                         #
+# |_|    |___/                                          |___/                                                          #
+# ==================================================================================================================== #
+# Authors:                                                                                                             #
+#   Patrick Lehmann                                                                                                    #
+#                                                                                                                      #
+# License:                                                                                                             #
+# ==================================================================================================================== #
+# Copyright 2020-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
+#                                                                                                                      #
+# Licensed under the Apache License, Version 2.0 (the "License");                                                      #
+# you may not use this file except in compliance with the License.                                                     #
+# You may obtain a copy of the License at                                                                              #
+#                                                                                                                      #
+#   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
+#                                                                                                                      #
+# Unless required by applicable law or agreed to in writing, software                                                  #
+# distributed under the License is distributed on an "AS IS" BASIS,                                                    #
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.                                             #
+# See the License for the specific language governing permissions and                                                  #
+# limitations under the License.                                                                                       #
+#                                                                                                                      #
+# SPDX-License-Identifier: Apache-2.0                                                                                  #
+# ==================================================================================================================== #
 #
 __author__ =    "Patrick Lehmann"
 __email__ =     "Paebbels@gmail.com"
-__copyright__ = "2020-2021, Patrick Lehmann"
+__copyright__ = "2020-2023, Patrick Lehmann"
 __license__ =   "Apache License, Version 2.0"
-__version__ =   "0.8.0"
+__version__ =   "0.9.0"
 __keywords__ =  ["Python3", "Template", "Versioning", "Git"]
 
-from subprocess   import run as subprocess_run, PIPE
 from dataclasses  import dataclass, make_dataclass, field
 from datetime     import date, time, datetime
-from pathlib      import Path
+from enum         import Enum, auto
 from os           import environ
-from typing       import Union, Any
+from pathlib      import Path
+from subprocess   import run as subprocess_run, PIPE
+from typing       import Union, Any, Dict
 
-from flags                      import Flags
+from pyTooling.Decorators import export
 from pyTooling.Versioning       import SemVersion
 from pyTooling.TerminalUI       import ILineTerminal
 
 from pyVersioning.Utils         import SelfDescriptive
 from pyVersioning.AppVeyor      import AppVeyor
 from pyVersioning.CIService     import WorkStation
 from pyVersioning.Configuration import Configuration
 from pyVersioning.GitLab        import GitLab
 from pyVersioning.GitHub        import GitHub
 from pyVersioning.Travis        import Travis
 
 
+@export
 @dataclass
 class Tool(SelfDescriptive):
 	name    : str
 	version : SemVersion
 
-	_public = ['name', 'version']
+	_public = ["name", "version"]
+
+
+@export
+class Date(date, SelfDescriptive):
+	_public = ["day", "month", "year"]
 
 
+@export
+class Time(time, SelfDescriptive):
+	_public = ["hour", "minute", "second"]
+
+
+@export
 @dataclass
 class Author(SelfDescriptive):
-	name: str
+	name:  str
 	email: str
 
-	_public = ['name', 'email']
+	_public = ["name", "email"]
 
 
+@export
 @dataclass
 class Commit(SelfDescriptive):
-	hash: str
-	date: date
-	time: time
-	author: Author
+	hash:    str
+	date:    date
+	time:    time
+	author:  Author
 	comment: str
 	oneline: str = field(init=False)
 
-	_public = ['hash', 'date', 'time', 'author', 'comment', 'oneline']
+	_public = ["hash", "date", "time", "author", "comment", "oneline"]
 
 	def __post_init__(self) -> None:
 		"""Calculate `oneline` from `comment`."""
 
 		if self.comment != "":
 			self.oneline = self.comment.split("\n")[0]
 
 
+@export
 @dataclass
 class Git(SelfDescriptive):
-	commit      : Commit
-	reference   : str = field(init=False)
-	tag         : str = ""
-	branch      : str = ""
-	repository  : str = ""
+	commit:     Commit
+	reference:  str = field(init=False)
+	tag:        str = ""
+	branch:     str = ""
+	repository: str = ""
 
-	_public = ['commit', 'reference', 'tag', 'branch', 'repository']
+	_public = ["commit", "reference", "tag", "branch", "repository"]
 
 	def __post_init__(self) -> None:
 		"""Calculate `reference` from `tag` or `branch`."""
 
 		if self.tag != "":
 			self.reference = self.tag
 		elif self.branch != "":
 			self.reference = self.branch
 		else:
 			self.reference = "[Detached HEAD]"
 
 
+@export
 @dataclass
 class Project(SelfDescriptive):
 	name:     str
 	variant:  str
 	version:  SemVersion
 
-	_public = ['name', 'variant', 'version']
+	_public = ["name", "variant", "version"]
 
 	def __init__(self, name: str, version: Union[str, SemVersion] = None, variant: str = None) -> None:
 		"""Assign fields and convert version string to a `Version` object."""
 
 		self.name    = name    if name    is not None else ""
 		self.variant = variant if variant is not None else ""
 
@@ -133,22 +144,23 @@
 			self.version = version
 		elif isinstance(version, str):
 			self.version = SemVersion(version)
 		elif version is None:
 			self.version = SemVersion(0, 0, 0)
 
 
+@export
 @dataclass
 class Compiler(SelfDescriptive):
 	name:           str
 	version:        SemVersion
 	configuration:  str
 	options:        str
 
-	_public = ['name', 'version', 'configuration', 'options']
+	_public = ["name", "version", "configuration", "options"]
 
 	def __init__(self, name: str, version: Union[str, SemVersion] = "", configuration: str = "", options: str = "") -> None:
 		"""Assign fields and convert version string to a `Version` object."""
 
 		self.name          = name          if name          is not None else ""
 		self.configuration = configuration if configuration is not None else ""
 		self.options       = options       if options       is not None else ""
@@ -157,85 +169,99 @@
 			self.version     = version
 		elif isinstance(version, str):
 			self.version     = SemVersion(version)
 		elif version is None:
 			self.version     = SemVersion(0, 0, 0)
 
 
+@export
 @dataclass
 class Build(SelfDescriptive):
 	date:     date
 	time:     time
 	compiler: Compiler
 
-	_public = ['date', 'time', 'compiler']
+	_public = ["date", "time", "compiler"]
 
 
-class Platforms(Flags):
-	Workstation = 1
-	AppVeyor = 2
-	GitHub = 3
-	GitLab = 4
-	Travis = 5
+@export
+class Platforms(Enum):
+	Workstation = auto()
+	AppVeyor =    auto()
+	GitHub =      auto()
+	GitLab =      auto()
+	Travis =      auto()
+
+
+@export
+class GitShowCommand(Enum):
+	CommitDateTime =       auto()
+	CommitAuthorName =     auto()
+	CommitAuthorEmail =    auto()
+	CommitCommitterName =  auto()
+	CommitCommitterEmail = auto()
+	CommitHash =           auto()
+	CommitComment =        auto()
 
 
+@export
 class Versioning(ILineTerminal):
-	platform  : int = Platforms.Workstation
-	variables : dict
+	platform:  Platforms = Platforms.Workstation
+	variables: Dict
 
 	def __init__(self, terminal: ILineTerminal):
 		super().__init__(terminal)
 
 		self.variables = {}
 
-		if 'APPVEYOR' in environ:
+		if "APPVEYOR" in environ:
 			self.platform = Platforms.AppVeyor
-		elif 'GITHUB_ACTIONS' in environ:
+		elif "GITHUB_ACTIONS" in environ:
 			self.platform = Platforms.GitHub
-		elif 'GITLAB_CI' in environ:
+		elif "GITLAB_CI" in environ:
 			self.platform = Platforms.GitLab
-		elif 'TRAVIS' in environ:
+		elif "TRAVIS" in environ:
 			self.platform = Platforms.Travis
 		else:
 			self.platform = Platforms.Workstation
 
 	def loadDataFromConfiguration(self, config: Configuration) -> None:
 		"""Preload versioning information from configuration file."""
 
-		self.variables['project'] = self.getProject(config.project)
-		self.variables['build']   = self.getBuild(config.build)
-		self.variables['version'] = self.getVersion(config.project)
+		self.variables["project"] = self.getProject(config.project)
+		self.variables["build"]   = self.getBuild(config.build)
+		self.variables["version"] = self.getVersion(config.project)
 
 	def collectData(self) -> None:
 		"""Collect versioning information from environment including CI services (if available)."""
 
 		if self.platform is Platforms.AppVeyor:
 			self.service                = AppVeyor()
-			self.variables['appveyor']  = self.service.getEnvironment()
+			self.variables["appveyor"]  = self.service.getEnvironment()
 		elif self.platform is Platforms.GitHub:
 			self.service                = GitHub()
-			self.variables['github']    = self.service.getEnvironment()
+			self.variables["github"]    = self.service.getEnvironment()
 		elif self.platform is Platforms.GitLab:
 			self.service                = GitLab()
-			self.variables['gitlab']    = self.service.getEnvironment()
+			self.variables["gitlab"]    = self.service.getEnvironment()
 		elif self.platform is Platforms.Travis:
 			self.service                = Travis()
-			self.variables['travis']    = self.service.getEnvironment()
+			self.variables["travis"]    = self.service.getEnvironment()
 		else:
 			self.service                = WorkStation()
 
-		self.variables['tool']     = Tool("pyVersioning", SemVersion(0,7,1))
-		self.variables['git']      = self.getGitInformation()
-		self.variables['env']      = self.getEnvironment()
-		self.variables['platform'] = self.service.getPlatform()
+		self.variables["tool"]     = Tool("pyVersioning", SemVersion(0,7,1))
+		self.variables["git"]      = self.getGitInformation()
+		self.variables["env"]      = self.getEnvironment()
+		self.variables["platform"] = self.service.getPlatform()
 
 		self.calculateData()
 
 	def calculateData(self) -> None:
-		if self.variables['git'].tag != "":
+		if self.variables["git"].tag != "":
 			pass
 
 	def getVersion(self, config: Configuration.Project) -> SemVersion:
 		if config.version is not None:
 			return config.version
 		else:
 			return SemVersion("0.0.0")
@@ -259,189 +285,166 @@
 			comment=self.getCommitComment()
 		)
 
 	def getGitHash(self) -> str:
 		if self.platform is not Platforms.Workstation:
 			return self.service.getGitHash()
 
-		try:
-			command =   "git"
-			arguments=  ("rev-parse", "HEAD")
-			completed = subprocess_run((command, *arguments), stdout=PIPE, stderr=PIPE)
-		except:
-			return "0" * 40
-		if completed.returncode == 0:
-			return completed.stdout.decode('utf-8').split("\n")[0]
-		else:
-			message = completed.stderr.decode('utf-8')
-			self.WriteFatal("Message from '{command}': {message}".format(command=command, message=message))
+		return self.execGitShow(GitShowCommand.CommitHash)
 
 	def getCommitDate(self) -> datetime:
 		if self.platform is not Platforms.Workstation:
 			return self.service.getCommitDate()
 
-		try:
-			command =   "git"
-			arguments = ("show", "-s", "--format=%ct") #, "HEAD")
-			completed = subprocess_run((command, *arguments), stdout=PIPE, stderr=PIPE)
-		except:
-			raise Exception
-
-		if completed.returncode == 0:
-			ts = int(completed.stdout.decode('utf-8').split("\n")[0])
-			return datetime.fromtimestamp(ts)
-		else:
-			message = completed.stderr.decode('utf-8')
-			self.WriteFatal("Message from '{command}': {message}".format(command=command, message=message))
-			raise Exception
+		datetimeString = self.execGitShow(GitShowCommand.CommitDateTime)
+		return datetime.fromtimestamp(int(datetimeString))
 
 	def getCommitAuthor(self) -> Author:
 		return Author(
 			name=self.getCommitAuthorName(),
 			email=self.getCommitAuthorEmail()
 		)
 
 	def getCommitAuthorName(self) -> str:
-		try:
-			command =   "git"
-			arguments = ("show", "-s", "--format='%an'") #, "HEAD")
-			completed = subprocess_run((command, *arguments), stdout=PIPE, stderr=PIPE)
-		except:
-			return ""
-		if completed.returncode == 0:
-			firstLine = completed.stdout.decode('utf-8').split("\n")[0]
-			return firstLine[1:-1]
-		else:
-			message = completed.stderr.decode('utf-8')
-			self.WriteFatal("Message from '{command}': {message}".format(command=command, message=message))
+		return self.execGitShow(GitShowCommand.CommitAuthorName)
 
 	def getCommitAuthorEmail(self) -> str:
-		try:
-			command =   "git"
-			arguments = ("show", "-s", "--format='%ae'") #, "HEAD")
-			completed = subprocess_run((command, *arguments), stdout=PIPE, stderr=PIPE)
-		except:
-			return ""
-		if completed.returncode == 0:
-			firstLine = completed.stdout.decode('utf-8').split("\n")[0]
-			return firstLine[1:-1]
-		else:
-			message = completed.stderr.decode('utf-8')
-			self.WriteFatal("Message from '{command}': {message}".format(command=command, message=message))
+		return self.execGitShow(GitShowCommand.CommitAuthorEmail)
+
+	def getCommitCommitterName(self) -> str:
+		return self.execGitShow(GitShowCommand.CommitCommitterName)
+
+	def getCommitCommitterEmail(self) -> str:
+		return self.execGitShow(GitShowCommand.CommitCommitterEmail)
 
 	def getCommitComment(self) -> str:
-		try:
-			command =   "git"
-			arguments = ("show", "-s", "--format='%B'") #, "HEAD")
-			completed = subprocess_run((command, *arguments), stdout=PIPE, stderr=PIPE)
-		except:
-			return ""
-		if completed.returncode == 0:
-			comment = completed.stdout.decode('utf-8')
-			return comment[1:-2]
-		else:
-			message = completed.stderr.decode('utf-8')
-			self.WriteFatal("Message from '{command}': {message}".format(command=command, message=message))
+		return self.execGitShow(GitShowCommand.CommitComment)
 
 	def getGitLocalBranch(self) -> str:
 		if self.platform is not Platforms.Workstation:
 			return self.service.getGitBranch()
 
 		try:
 			command =   "git"
 			arguments = ("branch", "--show-current")
 			completed = subprocess_run((command, *arguments), stdout=PIPE, stderr=PIPE)
 		except:
 			return ""
 		if completed.returncode == 0:
-			return completed.stdout.decode('utf-8').split("\n")[0]
+			return completed.stdout.decode("utf-8").split("\n")[0]
 		else:
-			message = completed.stderr.decode('utf-8')
-			self.WriteFatal("Message from '{command}': {message}".format(command=command, message=message))
+			message = completed.stderr.decode("utf-8")
+			self.WriteFatal(f"Message from '{command}': {message}")
 
 	def getGitRemoteBranch(self, localBranch: str = None) -> str:
 		if self.platform is not Platforms.Workstation:
 			return self.service.getGitBranch()
 
 		if localBranch is None:
 			localBranch = self.getGitLocalBranch()
 
 		try:
 			command =   "git"
-			arguments = ("config", "branch.{localBranch}.merge".format(localBranch=localBranch))
+			arguments = ("config", f"branch.{localBranch}.merge")
 			completed = subprocess_run((command, *arguments), stdout=PIPE, stderr=PIPE)
 		except:
-			raise Exception
+			raise Exception()
 
 		if completed.returncode == 0:
-			return completed.stdout.decode('utf-8').split("\n")[0]
+			return completed.stdout.decode("utf-8").split("\n")[0]
 		else:
-			message = completed.stderr.decode('utf-8')
-			self.WriteFatal("Message from '{command}': {message}".format(command=command, message=message))
+			message = completed.stderr.decode("utf-8")
+			self.WriteFatal(f"Message from '{command}': {message}")
 			raise Exception
 
 	def getGitRemote(self, localBranch: str = None) -> str:
 		if localBranch is None:
 			localBranch = self.getGitLocalBranch()
 
 		try:
 			command =   "git"
-			arguments=  ("config", "branch.{localBranch}.remote".format(localBranch=localBranch))
+			arguments=  ("config", f"branch.{localBranch}.remote")
 			completed = subprocess_run((command, *arguments), stdout=PIPE, stderr=PIPE)
 		except:
 			raise Exception
 
 		if completed.returncode == 0:
-			return completed.stdout.decode('utf-8').split("\n")[0]
+			return completed.stdout.decode("utf-8").split("\n")[0]
 		elif completed.returncode == 1:
-			self.WriteWarning("Branch '{localBranch}' is not pushed to a remote.".format(localBranch=localBranch))
-			return "(local) {localBranch}".format(localBranch=localBranch)
+			self.WriteWarning(f"Branch '{localBranch}' is not pushed to a remote.")
+			return f"(local) {localBranch}"
 		else:
-			message = completed.stderr.decode('utf-8')
-			self.WriteFatal("Message from '{command}': {message}".format(command=command, message=message))
+			message = completed.stderr.decode("utf-8")
+			self.WriteFatal(f"Message from '{command}': {message}")
 			raise Exception
 
 	def getGitTag(self) -> str:
 		if self.platform is not Platforms.Workstation:
 			return self.service.getGitTag()
 
 		try:
 			command =   "git"
-			arguments = ("tag", "--points-at","HEAD")
+			arguments = ("tag", "--points-at", "HEAD")
 			completed = subprocess_run((command, *arguments), stdout=PIPE, stderr=PIPE)
 		except:
 			raise Exception
 
 		if completed.returncode == 0:
-			return completed.stdout.decode('utf-8').split("\n")[0]
+			return completed.stdout.decode("utf-8").split("\n")[0]
 		else:
-			message = completed.stderr.decode('utf-8')
-			self.WriteFatal("Message from '{command}': {message}".format(command=command, message=message))
+			message = completed.stderr.decode("utf-8")
+			self.WriteFatal(f"Message from '{command}': {message}")
 			raise Exception
 
 	def getGitRemoteURL(self, remote: str = None) -> str:
 		if self.platform is not Platforms.Workstation:
 			return self.service.getGitRepository()
 
 		if remote is None:
 			remote = self.getGitRemote()
 		try:
 			command =   "git"
-			arguments = ("config", "remote.{remote}.url".format(remote=remote))
+			arguments = ("config", f"remote.{remote}.url")
 			completed = subprocess_run((command, *arguments), stdout=PIPE, stderr=PIPE)
 		except:
 			raise Exception
 
 		if completed.returncode == 0:
-			return completed.stdout.decode('utf-8').split("\n")[0]
+			return completed.stdout.decode("utf-8").split("\n")[0]
 		else:
-			message = completed.stderr.decode('utf-8')
-			self.WriteFatal("Message from '{command}': {message}".format(command=command, message=message))
+			message = completed.stderr.decode("utf-8")
+			self.WriteFatal(f"Message from '{command}': {message}")
 			raise Exception
 
+	__GIT_SHOW_COMMAND_TO_FORMAT_LOOKUP = {
+		GitShowCommand.CommitHash: "%H",
+		GitShowCommand.CommitDateTime: "%ct",
+		GitShowCommand.CommitAuthorName: "%an",
+		GitShowCommand.CommitAuthorEmail: "%ae",
+		GitShowCommand.CommitCommitterName: "%cn",
+		GitShowCommand.CommitCommitterEmail: "%ce",
+		GitShowCommand.CommitComment: "%B",
+	}
+
+	def execGitShow(self, command: GitShowCommand) -> str:
+		format = f"--format='{self.__GIT_SHOW_COMMAND_TO_FORMAT_LOOKUP[command]}'"
+
+		try:
+			command =   "git"
+			arguments = ("show", "-s", format) #, "HEAD")
+			completed = subprocess_run((command, *arguments), stdout=PIPE, stderr=PIPE)
+		except:
+			return ""
+		if completed.returncode == 0:
+			comment = completed.stdout.decode("utf-8")
+			return comment[1:-2]
+		else:
+			message = completed.stderr.decode("utf-8")
+			self.WriteFatal(f"Message from '{command}': {message}")
+
 	def getProject(self, config: Configuration.Project) -> Project:
 		return Project(
 			name=config.name,
 			version=config.version,
 			variant=config.variant
 		)
 
@@ -461,15 +464,15 @@
 			options=config.options
 		)
 
 	def getEnvironment(self) -> Any:
 		env = {}
 		for key, value in environ.items():
 			if not key.isidentifier():
-				self.WriteWarning("Skipping environment variable '{key}', because it's not a valid Python identifier.".format(key=key))
+				self.WriteWarning(f"Skipping environment variable '{key}', because it's not a valid Python identifier.")
 				continue
 			key = key.replace("(", "_")
 			key = key.replace(")", "_")
 			key = key.replace(" ", "_")
 			env[key] = value
 
 		def func(s):
@@ -477,24 +480,24 @@
 				yield (e, s.__getattribute__(e))
 
 		Environment = make_dataclass(
 			"Environment",
 			[(name, str) for name in env.keys()],
 #			bases=(SelfDescriptive,),
 			namespace={
-				'as_dict':        lambda self: env,
-				'Keys':           lambda self: env.keys(),
-				'KeyValuePairs':  lambda self: func(self)
+				"as_dict":       lambda self: env,
+				"Keys":          lambda self: env.keys(),
+				"KeyValuePairs": lambda self: func(self)
 			},
 			repr=True
 		)
 
 		return Environment(**env)
 
 	def writeSourceFile(self, template: Path, filename: Path) -> None:
 		content = template.read_text()
 
 		# apply variables
 		content = content.format(**self.variables)
 
-		with filename.open('w') as file:
+		with filename.open("w") as file:
 			file.write(content)
```

### Comparing `pyVersioning-0.8.0/pyVersioning/cli.py` & `pyVersioning-0.9.0/pyVersioning/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,154 +1,157 @@
-# =============================================================================
-#            __     __            _             _
-#  _ __  _   \ \   / /__ _ __ ___(_) ___  _ __ (_)_ __   __ _
-# | '_ \| | | \ \ / / _ \ '__/ __| |/ _ \| '_ \| | '_ \ / _` |
-# | |_) | |_| |\ V /  __/ |  \__ \ | (_) | | | | | | | | (_| |
-# | .__/ \__, | \_/ \___|_|  |___/_|\___/|_| |_|_|_| |_|\__, |
-# |_|    |___/                                          |___/
-# =============================================================================
-# Authors:            Patrick Lehmann
-#
-# Python package:     pyVersioning Implementation
-#
-# Description:
-# ------------------------------------
-#		TODO
-#
-# License:
-# ============================================================================
-# Copyright 2020-2021 Patrick Lehmann - Bötzingen, Germany
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# SPDX-License-Identifier: Apache-2.0
-# ============================================================================
+# ==================================================================================================================== #
+#            __     __            _             _                                                                      #
+#  _ __  _   \ \   / /__ _ __ ___(_) ___  _ __ (_)_ __   __ _                                                          #
+# | '_ \| | | \ \ / / _ \ '__/ __| |/ _ \| '_ \| | '_ \ / _` |                                                         #
+# | |_) | |_| |\ V /  __/ |  \__ \ | (_) | | | | | | | | (_| |                                                         #
+# | .__/ \__, | \_/ \___|_|  |___/_|\___/|_| |_|_|_| |_|\__, |                                                         #
+# |_|    |___/                                          |___/                                                          #
+# ==================================================================================================================== #
+# Authors:                                                                                                             #
+#   Patrick Lehmann                                                                                                    #
+#                                                                                                                      #
+# License:                                                                                                             #
+# ==================================================================================================================== #
+# Copyright 2020-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
+#                                                                                                                      #
+# Licensed under the Apache License, Version 2.0 (the "License");                                                      #
+# you may not use this file except in compliance with the License.                                                     #
+# You may obtain a copy of the License at                                                                              #
+#                                                                                                                      #
+#   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
+#                                                                                                                      #
+# Unless required by applicable law or agreed to in writing, software                                                  #
+# distributed under the License is distributed on an "AS IS" BASIS,                                                    #
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.                                             #
+# See the License for the specific language governing permissions and                                                  #
+# limitations under the License.                                                                                       #
+#                                                                                                                      #
+# SPDX-License-Identifier: Apache-2.0                                                                                  #
+# ==================================================================================================================== #
 #
 from argparse     import RawDescriptionHelpFormatter
 from pathlib      import Path
 from textwrap     import dedent
 from typing       import NoReturn
 
+from pyTooling.Decorators import export
+from pyTooling.TerminalUI            import LineTerminal, Severity
 from pyAttributes                    import Attribute
 from pyAttributes.ArgParseAttributes import ArgParseMixin, CommandAttribute, ArgumentAttribute, DefaultAttribute
-from pyTooling.TerminalUI            import LineTerminal, Severity
 
 from pyVersioning                    import Versioning, Platforms, Project, SelfDescriptive
 from pyVersioning.Configuration      import Configuration
 
 
+@export
 class ProjectAttributeGroup(Attribute):
 	def __call__(self, func):
-		self._AppendAttribute(func, ArgumentAttribute("--project-name",    metavar='<Name>',    dest="ProjectName",    type=str, help="Name of the project."))
-		self._AppendAttribute(func, ArgumentAttribute("--project-variant", metavar='<Variant>', dest="ProjectVariant", type=str, help="Variant of the project."))
-		self._AppendAttribute(func, ArgumentAttribute("--project-version", metavar='<Version>', dest="ProjectVersion", type=str, help="Version of the project."))
+		self._AppendAttribute(func, ArgumentAttribute("--project-name",    metavar="<Name>",    dest="ProjectName",    type=str, help="Name of the project."))
+		self._AppendAttribute(func, ArgumentAttribute("--project-variant", metavar="<Variant>", dest="ProjectVariant", type=str, help="Variant of the project."))
+		self._AppendAttribute(func, ArgumentAttribute("--project-version", metavar="<Version>", dest="ProjectVersion", type=str, help="Version of the project."))
 		return func
 
+
+@export
 class CompilerAttributeGroup(Attribute):
 	def __call__(self, func):
-		self._AppendAttribute(func, ArgumentAttribute("--compiler-name",    metavar='<Name>',    dest="CompilerName",    type=str, help="Used compiler."))
-		self._AppendAttribute(func, ArgumentAttribute("--compiler-version", metavar='<Version>', dest="CompilerVersion", type=str, help="Used compiler version."))
-		self._AppendAttribute(func, ArgumentAttribute("--compiler-config",  metavar='<Config>',  dest="CompilerConfig",  type=str, help="Used compiler configuration."))
-		self._AppendAttribute(func, ArgumentAttribute("--compiler-options", metavar='<Options>', dest="CompilerOptions", type=str, help="Used compiler options."))
+		self._AppendAttribute(func, ArgumentAttribute("--compiler-name",    metavar="<Name>",    dest="CompilerName",    type=str, help="Used compiler."))
+		self._AppendAttribute(func, ArgumentAttribute("--compiler-version", metavar="<Version>", dest="CompilerVersion", type=str, help="Used compiler version."))
+		self._AppendAttribute(func, ArgumentAttribute("--compiler-config",  metavar="<Config>",  dest="CompilerConfig",  type=str, help="Used compiler configuration."))
+		self._AppendAttribute(func, ArgumentAttribute("--compiler-options", metavar="<Options>", dest="CompilerOptions", type=str, help="Used compiler options."))
 		return func
 
 
+@export
 class Application(LineTerminal, ArgParseMixin):
-	HeadLine:     str  = "Version file generator."
+	HeadLine:     str = "Version file generator."
+
 	__configFile: Path
+	_config:      Configuration
+	_versioning:  Versioning
 
-	def __init__(self, configFile: Path) -> None:
+	def __init__(self) -> None:
 		super().__init__()
 
-		self.__configFile = configFile
-
 		ArgParseMixin.__init__(
 			self,
-	    description=dedent("Version file generator"),
-	    formatter_class=RawDescriptionHelpFormatter,
-	    add_help=False
-	  )
+			description=self.HeadLine,
+			formatter_class=RawDescriptionHelpFormatter,
+			add_help=False
+		)
 
-		self._LOG_MESSAGE_FORMAT__[Severity.Fatal]   = "{DARK_RED}[FATAL] {message}{NOCOLOR}"
-		self._LOG_MESSAGE_FORMAT__[Severity.Error]   = "{RED}[ERROR] {message}{NOCOLOR}"
+		self._LOG_MESSAGE_FORMAT__[Severity.Fatal] =   "{DARK_RED}[FATAL] {message}{NOCOLOR}"
+		self._LOG_MESSAGE_FORMAT__[Severity.Error] =   "{RED}[ERROR] {message}{NOCOLOR}"
 		self._LOG_MESSAGE_FORMAT__[Severity.Warning] = "{YELLOW}[WARNING] {message}{NOCOLOR}"
-		self._LOG_MESSAGE_FORMAT__[Severity.Normal]  = "{GRAY}{message}{NOCOLOR}"
+		self._LOG_MESSAGE_FORMAT__[Severity.Normal]=   "{GRAY}{message}{NOCOLOR}"
 
 	def Initialize(self) -> None:
 		if not self.__configFile.exists():
-			self.WriteWarning("Configuration file '{file!s}' does not exist.".format(file=self.__configFile))
+			self.WriteWarning(f"Configuration file '{self.__configFile}' does not exist.")
 			self._config = Configuration()
 		else:
 			self._config = Configuration(self.__configFile)
 
 		self._versioning = Versioning(self)
 		self._versioning.loadDataFromConfiguration(self._config)
 		self._versioning.collectData()
 
 	def PrintHeadline(self) -> None:
 		self.WriteNormal("{HEADLINE}{line}".format(line="=" * 80, **LineTerminal.Foreground))
 		self.WriteNormal("{HEADLINE}{headline: ^80s}".format(headline=self.HeadLine, **LineTerminal.Foreground))
 		self.WriteNormal("{HEADLINE}{line}".format(line="=" * 80, **LineTerminal.Foreground))
 
-	def Run(self) -> NoReturn:
-		ArgParseMixin.Run(self)
+	def Run(self, configFile: Path) -> NoReturn:
+		self.__configFile = configFile
+
+		super().Run(self)
 		self.exit()
 
 	@DefaultAttribute()
 	def HandleDefault(self, args) -> None:
 		self.PrintHeadline()
 		self.MainParser.print_help()
 
 	@CommandAttribute("help", help="Display help page(s) for the given command name.")
 	@ArgumentAttribute(metavar="Command", dest="Command", type=str, nargs="?", help="Print help page(s) for a command.")
 	def HandleHelp(self, args) -> None:
 		self.PrintHeadline()
 
-		if (args.Command is None):
+		if args.Command is None:
 			self.MainParser.print_help()
-		elif (args.Command == "help"):
+		elif args.Command == "help":
 			self.WriteError("This is a recursion ...")
 		else:
 			try:
 				self.SubParsers[args.Command].print_help()
 			except KeyError:
-				self.WriteError("Command {0} is unknown.".format(args.Command))
+				self.WriteError(f"Command {args.Command} is unknown.")
 
 	@CommandAttribute("fillout", help="Read a template and replace tokens with version information.")
 	@ProjectAttributeGroup()
 	@CompilerAttributeGroup()
-	@ArgumentAttribute(metavar='<Template file>', dest="Template", type=str, help="Template input filename.")
-	@ArgumentAttribute(metavar='<Output file>',   dest="Filename", type=str, help="Output filename.")
+	@ArgumentAttribute(metavar="<Template file>", dest="Template", type=str, help="Template input filename.")
+	@ArgumentAttribute(metavar="<Output file>",   dest="Filename", type=str, help="Output filename.")
 	def HandleFillOut(self, args) -> None:
 		self.PrintHeadline()
 		self.Initialize()
 
 		templateFile = Path(args.Template)
 		if not templateFile.exists():
-			self.WriteError("Template file '{file!s}' does not exist.".format(file=templateFile))
+			self.WriteError(f"Template file '{templateFile}' does not exist.")
 
 		outputFile = Path(args.Filename)
 		if not outputFile.parent.exists():
-			self.WriteWarning("Directory for file '{file!s}' does not exist. Directory will be created".format(file=outputFile))
+			self.WriteWarning(f"Directory for file '{outputFile}' does not exist. Directory will be created")
 			try:
 				outputFile.parent.mkdir()
 			except:
-				self.WriteError("Failed to create the directory '{dir}' for the output file.".format(dir=outputFile.parent))
+				self.WriteError(f"Failed to create the directory '{outputFile.parent}' for the output file.")
 		elif outputFile.exists():
-			self.WriteWarning("Output file '{file!s}' already exists. This file will be overwritten.".format(file=outputFile))
+			self.WriteWarning(f"Output file '{outputFile}' already exists. This file will be overwritten.")
 
 		self.ExitOnPreviousErrors()
 
 		self.UpdateProject(args)
 		self.UpdateCompiler(args)
 
 		self._versioning.writeSourceFile(templateFile, outputFile)
@@ -161,26 +164,26 @@
 		self.Initialize()
 
 		self.UpdateProject(args)
 		self.UpdateCompiler(args)
 
 		def print(key, value, indent):
 			key = ("  " * indent) + str(key)
-			self.WriteNormal("{key:24}: {value!s}".format(key=key, value=value))
+			self.WriteNormal(f"{key:24}: {value!s}")
 			if isinstance(value, SelfDescriptive):
-				for k,v in value.KeyValuePairs():
+				for k, v in value.KeyValuePairs():
 					print(k, v, indent + 1)
 
 		for key,value in self._versioning.variables.items():
 			print(key, value, 0)
 
 	@CommandAttribute("json", help="Write all available variables as JSON.")
 	@ProjectAttributeGroup()
 	@CompilerAttributeGroup()
-	@ArgumentAttribute(metavar='<Output file>',   dest="Filename", type=str, nargs="?", help="Output filename.")
+	@ArgumentAttribute(metavar="<Output file>",   dest="Filename", type=str, nargs="?", help="Output filename.")
 	def HandleJSON(self, args) -> None:
 		self.Initialize()
 
 		self.UpdateProject(args)
 		self.UpdateCompiler(args)
 
 		content = dedent("""\
@@ -192,49 +195,48 @@
 		   flags: {version.flags}
 		  }}
 		}}
 		""")
 		output = content.format(**self._versioning.variables)
 		self.WriteNormal(output)
 
-
 	@CommandAttribute("yaml", help="Write all available variables as YAML.")
 	@ProjectAttributeGroup()
 	@CompilerAttributeGroup()
-	@ArgumentAttribute(metavar='<Output file>',   dest="Filename", type=str, nargs="?", help="Output filename.")
+	@ArgumentAttribute(metavar="<Output file>",   dest="Filename", type=str, nargs="?", help="Output filename.")
 	def HandleYAML(self, args) -> None:
 		self.Initialize()
 
 		self.UpdateProject(args)
 		self.UpdateCompiler(args)
 
 		yamlEnvironment = "\n"
-		# for key, value in self._versioning.variables['env'].as_dict().items():
-		# 	yamlEnvironment += f"    {key}: {value}\n".format(key=key, value=value)
+		# for key, value in self._versioning.variables["env"].as_dict().items():
+		# 	yamlEnvironment += f"    {key}: {value}\n"
 
-		yamlAppVeyor  = "\n#   not found"
-		yamlGitHub    = "\n#   not found"
-		yamlGitLab    = "\n#   not found"
-		yamlTravis    = "\n#   not found"
+		yamlAppVeyor = "\n#   not found"
+		yamlGitHub =   "\n#   not found"
+		yamlGitLab =   "\n#   not found"
+		yamlTravis =   "\n#   not found"
 		if self._versioning.platform is Platforms.AppVeyor:
 			yamlAppVeyor = "\n"
-			for key, value in self._versioning.variables['appveyor'].as_dict().items():
-				yamlAppVeyor += f"    {key}: {value}\n".format(key=key, value=value)
+			for key, value in self._versioning.variables["appveyor"].as_dict().items():
+				yamlAppVeyor += f"    {key}: {value}\n"
 		elif self._versioning.platform is Platforms.GitHub:
 			yamlGitHub = "\n"
-			for key, value in self._versioning.variables['github'].as_dict().items():
-				yamlGitHub += f"    {key}: {value}\n".format(key=key, value=value)
+			for key, value in self._versioning.variables["github"].as_dict().items():
+				yamlGitHub += f"    {key}: {value}\n"
 		elif self._versioning.platform is Platforms.GitLab:
 			yamlGitLab = "\n"
-			for key, value in self._versioning.variables['gitlab'].as_dict().items():
-				yamlGitLab += f"    {key}: {value}\n".format(key=key, value=value)
+			for key, value in self._versioning.variables["gitlab"].as_dict().items():
+				yamlGitLab += f"    {key}: {value}\n"
 		elif self._versioning.platform is Platforms.Travis:
 			yamlTravis = "\n"
-			for key, value in self._versioning.variables['travis'].as_dict().items():
-				yamlTravis += f"    {key}: {value}\n".format(key=key, value=value)
+			for key, value in self._versioning.variables["travis"].as_dict().items():
+				yamlTravis += f"    {key}: {value}\n"
 
 		content = dedent("""\
 		  version: {version!s}
 		    major: {version.major}
 		    minor: {version.minor}
 		    patch: {version.patch}
 		    flags: {version.flags}
@@ -268,39 +270,39 @@
 		  travis: {yamlTravis}
 		  env:{yamlEnvironment}
 		""")
 		output = content.format(**self._versioning.variables, yamlEnvironment=yamlEnvironment, yamlAppVeyor=yamlAppVeyor, yamlGitHub=yamlGitHub, yamlGitLab=yamlGitLab, yamlTravis=yamlTravis)
 		self.WriteNormal(output)
 
 	def UpdateProject(self, args) -> None:
-		if 'project' not in self._versioning.variables:
-			self._versioning.variables['project'] = Project(args.ProjectName, args.ProjectVersion, args.ProjectVariant)
+		if "project" not in self._versioning.variables:
+			self._versioning.variables["project"] = Project(args.ProjectName, args.ProjectVersion, args.ProjectVariant)
 		elif args.ProjectName is not None:
-			self._versioning.variables['project'].name = args.ProjectName
+			self._versioning.variables["project"].name = args.ProjectName
 
 		if args.ProjectVariant is not None:
-			self._versioning.variables['project'].variant = args.ProjectVariant
+			self._versioning.variables["project"].variant = args.ProjectVariant
 
 		if args.ProjectVersion is not None:
-			self._versioning.variables['project'].version = args.ProjectVersion
+			self._versioning.variables["project"].version = args.ProjectVersion
 
 	def UpdateCompiler(self, args) -> None:
 		if args.CompilerName is not None:
-			self._versioning.variables['build'].compiler.name = args.CompilerName
+			self._versioning.variables["build"].compiler.name = args.CompilerName
 		if args.CompilerVersion is not None:
-			self._versioning.variables['build'].compiler.version = args.CompilerVersion
+			self._versioning.variables["build"].compiler.version = args.CompilerVersion
 		if args.CompilerConfig is not None:
-			self._versioning.variables['build'].compiler.configuration = args.CompilerConfig
+			self._versioning.variables["build"].compiler.configuration = args.CompilerConfig
 		if args.CompilerOptions is not None:
-			self._versioning.variables['build'].compiler.options = args.CompilerOptions
+			self._versioning.variables["build"].compiler.options = args.CompilerOptions
 
 
 def main() -> NoReturn:
 	configFile = Path(".pyVersioning.yml")
 
-	Application.versionCheck((3,7,0))
-	application = Application(configFile)
-	application.Run()
+	Application.versionCheck((3, 7, 0))
+	application = Application()
+	application.Run(configFile)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
 	main()
```

### Comparing `pyVersioning-0.8.0/pyVersioning.egg-info/PKG-INFO` & `pyVersioning-0.9.0/pyVersioning.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: pyVersioning
-Version: 0.8.0
+Version: 0.9.0
 Summary: Write version information for any programming language as source file.
 Home-page: https://GitHub.com/Paebbels/pyVersioning
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://Paebbels.GitHub.io/pyVersioning
 Project-URL: Source Code, https://GitHub.com/Paebbels/pyVersioning
 Project-URL: Issue Tracker, https://GitHub.com/Paebbels/pyVersioning/issues
 Keywords: Python3,Template,Versioning,Git
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE.md
 
 [![Sourcecode on GitHub](https://img.shields.io/badge/Paebbels-pyVersioning-323131.svg?logo=github&longCache=true)](https://github.com/Paebbels/pyVersioning)
 [![License](https://img.shields.io/badge/code%20license-Apache%20License%2C%202.0-lightgrey?logo=GitHub)](LICENSE.md)
@@ -87,9 +86,7 @@
 
 <!-- The accompanying documentation is licensed under Creative Commons - Attribution-4.0 (CC-BY 4.0). -->
 
 
 -------------------------
 
 SPDX-License-Identifier: Apache-2.0
-
-
```

