# Comparing `tmp/mojo_extension-1.3.8.tar.gz` & `tmp/mojo_extension-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_extension-1.3.8.tar", max compression
+gzip compressed data, was "mojo_extension-1.3.9.tar", max compression
```

## Comparing `mojo_extension-1.3.8.tar` & `mojo_extension-1.3.9.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1083 2024-01-26 02:54:57.671747 mojo_extension-1.3.8/LICENSE.txt
--rw-r--r--   0        0        0     4589 2024-01-27 23:48:42.230650 mojo_extension-1.3.8/README.rst
--rw-r--r--   0        0        0      851 2024-02-21 07:51:25.492452 mojo_extension-1.3.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-26 02:54:57.673374 mojo_extension-1.3.8/source/packages/mojo/extension/__init__.py
--rw-r--r--   0        0        0      294 2024-01-26 02:54:57.673459 mojo_extension-1.3.8/source/packages/mojo/extension/extensionfactory.py
--rw-r--r--   0        0        0      861 2024-01-26 02:54:57.673538 mojo_extension-1.3.8/source/packages/mojo/extension/extensionprotocol.py
--rw-r--r--   0        0        0     3590 2024-02-21 07:50:55.656363 mojo_extension-1.3.8/source/packages/mojo/extension/extensionvariables.py
--rw-r--r--   0        0        0      929 2024-01-26 02:54:57.673712 mojo_extension-1.3.8/source/packages/mojo/extension/overridepack.py
--rw-r--r--   0        0        0      664 2024-01-26 02:54:57.673802 mojo_extension-1.3.8/source/packages/mojo/extension/overrideprotocol.py
--rw-r--r--   0        0        0     5421 2024-01-27 21:33:06.210726 mojo_extension-1.3.8/source/packages/mojo/extension/superfactory.py
--rw-r--r--   0        0        0     3713 2024-01-26 02:54:57.674003 mojo_extension-1.3.8/source/packages/mojo/extension/utilities.py
--rw-r--r--   0        0        0     1032 2024-02-14 07:52:53.799058 mojo_extension-1.3.8/source/packages/mojo/extension/wellknown.py
--rw-r--r--   0        0        0     5479 1970-01-01 00:00:00.000000 mojo_extension-1.3.8/setup.py
--rw-r--r--   0        0        0     5445 1970-01-01 00:00:00.000000 mojo_extension-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-26 02:54:57.671747 mojo_extension-1.3.9/LICENSE.txt
+-rw-r--r--   0        0        0     4589 2024-01-27 23:48:42.230650 mojo_extension-1.3.9/README.rst
+-rw-r--r--   0        0        0      851 2024-03-08 12:45:38.869745 mojo_extension-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-26 02:54:57.673374 mojo_extension-1.3.9/source/packages/mojo/extension/__init__.py
+-rw-r--r--   0        0        0      294 2024-01-26 02:54:57.673459 mojo_extension-1.3.9/source/packages/mojo/extension/extensionfactory.py
+-rw-r--r--   0        0        0      861 2024-01-26 02:54:57.673538 mojo_extension-1.3.9/source/packages/mojo/extension/extensionprotocol.py
+-rw-r--r--   0        0        0     2142 2024-03-08 13:01:38.309610 mojo_extension-1.3.9/source/packages/mojo/extension/extensionsettings.py
+-rw-r--r--   0        0        0     2189 2024-03-08 13:01:52.842923 mojo_extension-1.3.9/source/packages/mojo/extension/extensionvariables.py
+-rw-r--r--   0        0        0      929 2024-01-26 02:54:57.673712 mojo_extension-1.3.9/source/packages/mojo/extension/overridepack.py
+-rw-r--r--   0        0        0      664 2024-01-26 02:54:57.673802 mojo_extension-1.3.9/source/packages/mojo/extension/overrideprotocol.py
+-rw-r--r--   0        0        0     5421 2024-01-27 21:33:06.210726 mojo_extension-1.3.9/source/packages/mojo/extension/superfactory.py
+-rw-r--r--   0        0        0     3713 2024-01-26 02:54:57.674003 mojo_extension-1.3.9/source/packages/mojo/extension/utilities.py
+-rw-r--r--   0        0        0     1032 2024-02-14 07:52:53.799058 mojo_extension-1.3.9/source/packages/mojo/extension/wellknown.py
+-rw-r--r--   0        0        0     5479 1970-01-01 00:00:00.000000 mojo_extension-1.3.9/setup.py
+-rw-r--r--   0        0        0     5445 1970-01-01 00:00:00.000000 mojo_extension-1.3.9/PKG-INFO
```

### Comparing `mojo_extension-1.3.8/LICENSE.txt` & `mojo_extension-1.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_extension-1.3.8/README.rst` & `mojo_extension-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `mojo_extension-1.3.8/pyproject.toml` & `mojo_extension-1.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mojo-extension"
 description = "Automation Mojo Extension Package"
-version = "1.3.8"
+version = "1.3.9"
 authors = [
     "Myron Walker <myron.walker@gmail.com>"
 ]
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `mojo_extension-1.3.8/source/packages/mojo/extension/extensionprotocol.py` & `mojo_extension-1.3.9/source/packages/mojo/extension/extensionprotocol.py`

 * *Files identical despite different names*

### Comparing `mojo_extension-1.3.8/source/packages/mojo/extension/overridepack.py` & `mojo_extension-1.3.9/source/packages/mojo/extension/overridepack.py`

 * *Files identical despite different names*

### Comparing `mojo_extension-1.3.8/source/packages/mojo/extension/overrideprotocol.py` & `mojo_extension-1.3.9/source/packages/mojo/extension/overrideprotocol.py`

 * *Files identical despite different names*

### Comparing `mojo_extension-1.3.8/source/packages/mojo/extension/superfactory.py` & `mojo_extension-1.3.9/source/packages/mojo/extension/superfactory.py`

 * *Files identical despite different names*

### Comparing `mojo_extension-1.3.8/source/packages/mojo/extension/utilities.py` & `mojo_extension-1.3.9/source/packages/mojo/extension/utilities.py`

 * *Files identical despite different names*

### Comparing `mojo_extension-1.3.8/source/packages/mojo/extension/wellknown.py` & `mojo_extension-1.3.9/source/packages/mojo/extension/wellknown.py`

 * *Files identical despite different names*

### Comparing `mojo_extension-1.3.8/setup.py` & `mojo_extension-1.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['mojo-startup>=1.3.5,<1.4.0']
 
 setup_kwargs = {
     'name': 'mojo-extension',
-    'version': '1.3.8',
+    'version': '1.3.9',
     'description': 'Automation Mojo Extension Package',
     'long_description': '=================================\nAutomation Mojo Extension Package\n=================================\n\nThis is a python package that provides a mechanism for extending other python packages.  This\npackage is different from other python extension packages in that it uses the python Protocol\ntyping in order to query module hierarchies for extensions.\n\n\n===============================\nDeclaring an Extension Protocol\n===============================\n\nFor example, if we want to be able to create instance of object like these from a factory.\n\n.. code:: python\n\n    class Hey:\n        def __str__(self):\n            return "Hey"\n\n    class Ho:\n        def __str__(self):\n            return "Ho"\n\n    \n    # The following class defines a protocol that defines an extenstion type.\n    # Extensions \n\n    class MyExtTypeProtocol(ExtProtocol):\n\n        ext_protocol_name = "mojo-myextypeprotocol"\n\n        @classmethod\n        def give_me_a_hey(cls):\n            ...\n\n        @classmethod\n        def give_me_a_ho(cls):\n            ...\n\n==================================\nImplementing an Extension Protocol\n==================================\n\nThe code below is implementing the extension protocol defined above.  When a class\nimplements an extension protocol, it will inherit from the protocol it is implementing.\nBy inheriting from the protocol, it pulls in the `ext_protocol_name` variable which\nensures that the derived type is declared to implement a given protocol.\n\nAnother important thing to look at in the code below is the class variable `PRECEDENCE`.\nThe `PRECEDENCE` number indicates to the SuperFactory which extensions to return when\nan extension is queried based on precedence of overload and relevance.  The higher number\nprecedence is considered by the SuperFactory to have the most relevance.\n\n.. code:: python\n\n    class MyExtTypeFactory(ExtFactory, MyExtTypeProtocol):\n\n        PRECEDENCE = 10\n\n        @classmethod\n        def give_me_a_hey(cls):\n            return Hey\n        \n        @classmethod\n        def give_me_a_ho(cls):\n            return Ho\n\n\n===================================\nConfiguration for Custom Extensions\n===================================\n\nIn order to be able to extend packages, you must tell the `mojo-extension` code where\nthe root packages are that need to be searched for extension factories.  Then what we\ndo is we register the root modules under which the factory types will be found.\n\n---------------------------------------------------------------\nSetting the MJR_CONFIGURED_FACTORY_MODULES Variable from Python\n---------------------------------------------------------------\n\n.. code:: python\n\n    from mojo.extension.extensionconfiguration import ExtensionConfiguration\n    from mojo.extension.wellknown import ConfiguredSuperFactorySingleton\n\n    ExtensionConfiguration.MJR_CONFIGURED_FACTORY_MODULES = [\n            "mypkg.factories",\n        ]\n\n---------------------------------------------------------------\nSetting the MJR_CONFIGURED_FACTORY_MODULES Environment Variable\n---------------------------------------------------------------\n\n.. code::\n    \n    MJR_CONFIGURED_FACTORY_MODULES=mypkg.a.factories,mypkg.b.factories\n\n----------------------------------------------------------------\nSetting the MJR_CONFIGURED_FACTORY_MODULES in the Startup Config\n----------------------------------------------------------------\n\n.. code::\n    \n    [MOJO-EXTENSION]\n    MJR_CONFIGURED_FACTORY_MODULES=mypkg.a.factories,mypkg.b.factories\n\n========================\nLoading Custom Factories\n========================\n\nIn order to load extension factories, we utilize the `ConfiguredSuperFactorySingleton` singleton\nobject that is maintained by the `mojo-extension` package.  You can get a reference to the super\nfactory singleton by using code similar to the code below:\n\n.. code:: python\n\n    from mojo.extension.wellknown import ConfiguredSuperFactorySingleton\n\n    superfactory = ConfiguredSuperFactorySingleton()\n\n\nThen when we want to get the type from the extension, we utilize the protocol that\nwas declared and ask for the type using the function on the protocol that will return\nthe type.\n\n.. code:: python\n\n    hey_type = self._super_factory.get_override_types_by_order(MyExtTypeProtocol.give_me_a_hey)\n    ho_type = self._super_factory.get_override_types_by_order(MyExtTypeProtocol.give_me_a_ho)\n\n    hey = hey_type()\n    ho = ho_type()\n\n    print("")\n    print(f"{hey}... {ho}... {hey}... {ho}...")\n\n\n==========\nReferences\n==========\n\n- `User Guide <userguide/userguide.rst>`_\n- `Coding Standards <userguide/10-00-coding-standards.rst>`_\n',
     'author': 'Myron Walker',
     'author_email': 'myron.walker@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'http://automationmojo.com',
```

### Comparing `mojo_extension-1.3.8/PKG-INFO` & `mojo_extension-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mojo-extension
-Version: 1.3.8
+Version: 1.3.9
 Summary: Automation Mojo Extension Package
 Home-page: http://automationmojo.com
 License: LICENSE.txt
 Keywords: python
 Author: Myron Walker
 Author-email: myron.walker@gmail.com
 Requires-Python: >=3.8,<4.0
```

