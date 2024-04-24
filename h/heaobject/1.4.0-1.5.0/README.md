# Comparing `tmp/heaobject-1.4.0.tar.gz` & `tmp/heaobject-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaobject-1.4.0.tar", last modified: Thu Apr 18 01:58:27 2024, max compression
+gzip compressed data, was "heaobject-1.5.0.tar", last modified: Wed Apr 24 17:29:04 2024, max compression
```

## Comparing `heaobject-1.4.0.tar` & `heaobject-1.5.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 01:58:27.040990 heaobject-1.4.0/
--rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:08.000000 heaobject-1.4.0/LICENSE
--rw-rw-rw-   0        0        0     4708 2024-04-18 01:58:27.038983 heaobject-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     3202 2024-04-18 01:57:27.000000 heaobject-1.4.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-18 01:58:27.040990 heaobject-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     2603 2024-04-18 01:57:54.000000 heaobject-1.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 01:58:26.981137 heaobject-1.4.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-18 01:58:27.026978 heaobject-1.4.0/src/heaobject/
--rw-rw-rw-   0        0        0     1247 2023-12-16 22:23:08.000000 heaobject-1.4.0/src/heaobject/__init__.py
--rw-rw-rw-   0        0        0     4970 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/account.py
--rw-rw-rw-   0        0        0    15629 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/activity.py
--rw-rw-rw-   0        0        0     4030 2023-12-16 22:23:08.000000 heaobject-1.4.0/src/heaobject/aws.py
--rw-rw-rw-   0        0        0     6945 2023-12-16 22:23:08.000000 heaobject-1.4.0/src/heaobject/awss3key.py
--rw-rw-rw-   0        0        0     7587 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/bucket.py
--rw-rw-rw-   0        0        0     9918 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/data.py
--rw-rw-rw-   0        0        0     2604 2023-12-16 22:23:08.000000 heaobject-1.4.0/src/heaobject/dataadapter.py
--rw-rw-rw-   0        0        0      272 2022-03-11 01:28:08.000000 heaobject-1.4.0/src/heaobject/dataelement.py
--rw-rw-rw-   0        0        0     1601 2022-03-11 01:28:08.000000 heaobject-1.4.0/src/heaobject/datamodel.py
--rw-rw-rw-   0        0        0      430 2022-03-11 01:28:08.000000 heaobject-1.4.0/src/heaobject/datapattern.py
--rw-rw-rw-   0        0        0      238 2023-12-16 22:23:08.000000 heaobject-1.4.0/src/heaobject/datatransform.py
--rw-rw-rw-   0        0        0      353 2023-12-16 22:23:08.000000 heaobject-1.4.0/src/heaobject/error.py
--rw-rw-rw-   0        0        0    22016 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/folder.py
--rw-rw-rw-   0        0        0     4662 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/keychain.py
--rw-rw-rw-   0        0        0     2859 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/mimetype.py
--rw-rw-rw-   0        0        0     9112 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/organization.py
--rw-rw-rw-   0        0        0    10842 2024-04-18 01:33:48.000000 heaobject-1.4.0/src/heaobject/person.py
--rw-rw-rw-   0        0        0     5129 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/project.py
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:08.000000 heaobject-1.4.0/src/heaobject/py.typed
--rw-rw-rw-   0        0        0      211 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/record.py
--rw-rw-rw-   0        0        0    24659 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/registry.py
--rw-rw-rw-   0        0        0    76096 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/root.py
--rw-rw-rw-   0        0        0      597 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/settings.py
--rw-rw-rw-   0        0        0       66 2024-03-26 22:41:59.000000 heaobject-1.4.0/src/heaobject/source.py
--rw-rw-rw-   0        0        0     1165 2023-12-16 22:23:08.000000 heaobject-1.4.0/src/heaobject/source2target.py
--rw-rw-rw-   0        0        0     4074 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/storage.py
--rw-rw-rw-   0        0        0    10289 2024-04-18 01:52:57.000000 heaobject-1.4.0/src/heaobject/trash.py
--rw-rw-rw-   0        0        0     1135 2024-03-26 22:41:59.000000 heaobject-1.4.0/src/heaobject/user.py
--rw-rw-rw-   0        0        0      498 2023-12-16 22:23:08.000000 heaobject-1.4.0/src/heaobject/util.py
--rw-rw-rw-   0        0        0     6618 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/volume.py
-drwxrwxrwx   0        0        0        0 2024-04-18 01:58:27.037983 heaobject-1.4.0/src/heaobject.egg-info/
--rw-rw-rw-   0        0        0     4708 2024-04-18 01:58:26.000000 heaobject-1.4.0/src/heaobject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      995 2024-04-18 01:58:26.000000 heaobject-1.4.0/src/heaobject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 01:58:26.000000 heaobject-1.4.0/src/heaobject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-04-18 01:58:26.000000 heaobject-1.4.0/src/heaobject.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-18 01:58:26.000000 heaobject-1.4.0/src/heaobject.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 17:29:04.979987 heaobject-1.5.0/
+-rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:08.000000 heaobject-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0     4832 2024-04-24 17:29:04.978987 heaobject-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3326 2024-04-24 17:10:28.000000 heaobject-1.5.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 17:29:04.980988 heaobject-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     2603 2024-04-24 17:08:43.000000 heaobject-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:29:04.921704 heaobject-1.5.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 17:29:04.969800 heaobject-1.5.0/src/heaobject/
+-rw-rw-rw-   0        0        0     1247 2023-12-16 22:23:08.000000 heaobject-1.5.0/src/heaobject/__init__.py
+-rw-rw-rw-   0        0        0     4970 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/account.py
+-rw-rw-rw-   0        0        0    15629 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/activity.py
+-rw-rw-rw-   0        0        0     4030 2023-12-16 22:23:08.000000 heaobject-1.5.0/src/heaobject/aws.py
+-rw-rw-rw-   0        0        0     6945 2023-12-16 22:23:08.000000 heaobject-1.5.0/src/heaobject/awss3key.py
+-rw-rw-rw-   0        0        0     7587 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/bucket.py
+-rw-rw-rw-   0        0        0     9918 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/data.py
+-rw-rw-rw-   0        0        0     2604 2023-12-16 22:23:08.000000 heaobject-1.5.0/src/heaobject/dataadapter.py
+-rw-rw-rw-   0        0        0      272 2022-03-11 01:28:08.000000 heaobject-1.5.0/src/heaobject/dataelement.py
+-rw-rw-rw-   0        0        0     1601 2022-03-11 01:28:08.000000 heaobject-1.5.0/src/heaobject/datamodel.py
+-rw-rw-rw-   0        0        0      430 2022-03-11 01:28:08.000000 heaobject-1.5.0/src/heaobject/datapattern.py
+-rw-rw-rw-   0        0        0      238 2023-12-16 22:23:08.000000 heaobject-1.5.0/src/heaobject/datatransform.py
+-rw-rw-rw-   0        0        0      353 2023-12-16 22:23:08.000000 heaobject-1.5.0/src/heaobject/error.py
+-rw-rw-rw-   0        0        0    22016 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/folder.py
+-rw-rw-rw-   0        0        0     4662 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/keychain.py
+-rw-rw-rw-   0        0        0     2859 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/mimetype.py
+-rw-rw-rw-   0        0        0    14028 2024-04-24 17:07:44.000000 heaobject-1.5.0/src/heaobject/organization.py
+-rw-rw-rw-   0        0        0    10911 2024-04-21 20:58:31.000000 heaobject-1.5.0/src/heaobject/person.py
+-rw-rw-rw-   0        0        0     5129 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/project.py
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:08.000000 heaobject-1.5.0/src/heaobject/py.typed
+-rw-rw-rw-   0        0        0      211 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/record.py
+-rw-rw-rw-   0        0        0    24659 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/registry.py
+-rw-rw-rw-   0        0        0    80257 2024-04-22 18:17:42.000000 heaobject-1.5.0/src/heaobject/root.py
+-rw-rw-rw-   0        0        0      597 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/settings.py
+-rw-rw-rw-   0        0        0       66 2024-03-26 22:41:59.000000 heaobject-1.5.0/src/heaobject/source.py
+-rw-rw-rw-   0        0        0     1165 2023-12-16 22:23:08.000000 heaobject-1.5.0/src/heaobject/source2target.py
+-rw-rw-rw-   0        0        0     4074 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/storage.py
+-rw-rw-rw-   0        0        0    10289 2024-04-18 02:00:20.000000 heaobject-1.5.0/src/heaobject/trash.py
+-rw-rw-rw-   0        0        0     1135 2024-03-26 22:41:59.000000 heaobject-1.5.0/src/heaobject/user.py
+-rw-rw-rw-   0        0        0      498 2023-12-16 22:23:08.000000 heaobject-1.5.0/src/heaobject/util.py
+-rw-rw-rw-   0        0        0     6618 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/volume.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:29:04.977988 heaobject-1.5.0/src/heaobject.egg-info/
+-rw-rw-rw-   0        0        0     4832 2024-04-24 17:29:04.000000 heaobject-1.5.0/src/heaobject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      995 2024-04-24 17:29:04.000000 heaobject-1.5.0/src/heaobject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 17:29:04.000000 heaobject-1.5.0/src/heaobject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-04-24 17:29:04.000000 heaobject-1.5.0/src/heaobject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-24 17:29:04.000000 heaobject-1.5.0/src/heaobject.egg-info/top_level.txt
```

### Comparing `heaobject-1.4.0/LICENSE` & `heaobject-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaobject-1.4.0/PKG-INFO` & `heaobject-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaobject
-Version: 1.4.0
+Version: 1.5.0
 Summary: Data and other classes that are passed into and out of HEA REST APIs.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,18 @@
 Requires-Dist: mimetype-description~=0.1.0
 
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.5.0
+* Added attribute-level permissions.
+* Fixed bug in checking equality of AbstractAssociation objects.
+
 ## Version 1.4.0
 * Added "deleted" attribute to the trash module's TrashItem class.
 * Added Group class to the person module.
 
 ## Version 1.3.0
 * Added type_display_name attribute to all HEA objects.
```

### Comparing `heaobject-1.4.0/README.md` & `heaobject-1.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.5.0
+* Added attribute-level permissions.
+* Fixed bug in checking equality of AbstractAssociation objects.
+
 ## Version 1.4.0
 * Added "deleted" attribute to the trash module's TrashItem class.
 * Added Group class to the person module.
 
 ## Version 1.3.0
 * Added type_display_name attribute to all HEA objects.
```

### Comparing `heaobject-1.4.0/setup.py` & `heaobject-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(name='heaobject',
-                 version='1.4.0',
+                 version='1.5.0',
                  description='Data and other classes that are passed into and out of HEA REST APIs.',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://risr.hci.utah.edu',
                  author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
                  author_email='Andrew.Post@hci.utah.edu',
                  python_requires='>=3.10',
```

### Comparing `heaobject-1.4.0/src/heaobject/__init__.py` & `heaobject-1.5.0/src/heaobject/__init__.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.4.0/src/heaobject/account.py` & `heaobject-1.5.0/src/heaobject/account.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.4.0/src/heaobject/activity.py` & `heaobject-1.5.0/src/heaobject/activity.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.4.0/src/heaobject/aws.py` & `heaobject-1.5.0/src/heaobject/aws.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.4.0/src/heaobject/awss3key.py` & `heaobject-1.5.0/src/heaobject/awss3key.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.4.0/src/heaobject/bucket.py` & `heaobject-1.5.0/src/heaobject/bucket.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.4.0/src/heaobject/data.py` & `heaobject-1.5.0/src/heaobject/data.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.4.0/src/heaobject/dataadapter.py` & `heaobject-1.5.0/src/heaobject/dataadapter.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.4.0/src/heaobject/datamodel.py` & `heaobject-1.5.0/src/heaobject/datamodel.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.4.0/src/heaobject/folder.py` & `heaobject-1.5.0/src/heaobject/folder.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.4.0/src/heaobject/keychain.py` & `heaobject-1.5.0/src/heaobject/keychain.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.4.0/src/heaobject/mimetype.py` & `heaobject-1.5.0/src/heaobject/mimetype.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.4.0/src/heaobject/organization.py` & `heaobject-1.5.0/src/heaobject/trash.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,237 +1,292 @@
-import logging
-
-from .account import AccountAssociation, AWSAccount
-from .root import Permission
-from .data import DataObject, SameMimeType
+"""
+Classes for HEA's trash facility. The trash is a location to delete desktop
+objects where they can be put back later if the user realizes the deletion was
+a mistake.
+"""
+from abc import ABC, abstractmethod
+from heaobject.aws import S3_URI_PATTERN, s3_uri, S3StorageClassMixin
+from heaobject.awss3key import KeyDecodeException, decode_key, encode_key, is_folder
+from heaobject.data import AWSS3FileObject
+from heaobject.folder import AWSS3Folder
+from .root import AbstractDesktopObject, HasSize, View, desktop_object_type_for_name
+from datetime import date
 from typing import Optional
-from copy import deepcopy
-
-permission_id_dict = {
-    'admin_ids': [Permission.COOWNER],
-    'manager_ids': [Permission.VIEWER, Permission.EDITOR, Permission.SHARER, Permission.DELETER],
-    'member_ids': [Permission.VIEWER, Permission.SHARER]
-}
-
+from dateutil import parser as dateparser
 
-class Organization(DataObject, SameMimeType):
+class TrashItem(AbstractDesktopObject, View, ABC):
     """
-    Represents a directory in the HEA desktop.
+    Abstract base class for trash items. Trash items are an alternative
+    representation of the desktop object that was put in the trash.
     """
-
+    @abstractmethod
     def __init__(self) -> None:
         super().__init__()
-        # id is a super field
-        self.__accounts: dict[AccountAssociation, None] = {}
-        self.__principal_investigator_id: Optional[str] = None  # this would be a people id
-        self.__admin_ids: list[str] = []  # list of user ids to be managers
-        self.__manager_ids: list[str] = []  # list of user ids to be managers
-        self.__member_ids: list[str] = []  # list of user ids to be members
-        # super's name and display name would be used as org name(required)
+        self.__deleted: date | None = None
 
-    @classmethod
-    def get_mime_type(cls) -> str:
+    @property
+    @abstractmethod
+    def original_location(self) -> str | None:
         """
-        Returns the mime type of instances of the Organization class.
-
-        :return: application/x.organization
+        The object's original location. The format of the location string is
+        unique for different subclasses.
         """
-        return 'application/x.organization'
+        pass
 
-    @property
-    def mime_type(self) -> str:
-        """Read-only. The mime type for Organization objects, application/x.organization."""
-        return type(self).get_mime_type()
+    @original_location.setter
+    @abstractmethod
+    def original_location(self, original_location: str | None):
+        pass
 
     @property
-    def accounts(self) -> list[AccountAssociation]:
-        """The list of accounts owned by this organization."""
-        return list(deepcopy(account) for account in self.__accounts)
+    def deleted(self) -> Optional[date]:
+        """
+        The date the deleted object was deleted (the date the objects' delete marker was created).
+        """
+        return self.__deleted
 
-    @accounts.setter
-    def accounts(self, accounts: list[AccountAssociation]):
-        if accounts is None:
-            self.__accounts.clear()
-        elif isinstance(accounts, AccountAssociation):
-            self.__accounts.clear()
-            self.__accounts[deepcopy(accounts)] = None
-        else:
-            if not all(isinstance(account, AccountAssociation) for account in accounts):
-                raise TypeError('accounts can only contain AccountAssociation objects')
-            self.__accounts.clear()
-            for account in accounts:
-                self.__accounts[deepcopy(account)] = None
-
-    def add_account(self, account: AccountAssociation):
-        if isinstance(account, AccountAssociation):
-            self.__accounts[deepcopy(account)] = None
-        else:
-            raise TypeError('account must be an AccountAssociation')
 
-    def remove_account(self, account: AccountAssociation):
-        try:
-            del self.__accounts[account]
-        except KeyError:
-            raise ValueError(f'Account {account} not found')
-
-    @property
-    def aws_account_ids(self) -> list[str]:
-        """
-        The list of aws account ids owned by this organization.
-        """
-        return [account.actual_object_id for account in self.__accounts
-                if account.actual_object_type_name == AWSAccount.get_type_name()]
-
-    @aws_account_ids.setter
-    def aws_account_ids(self, value: list[str]) -> None:
-        aws_account_type_name = AWSAccount.get_type_name()
-        keys_to_remove = (account for account in self.__accounts if
-                          account.actual_object_type_name != aws_account_type_name)
-        for key in keys_to_remove:
-            del self.__accounts[key]
-        if value is None:
-            pass
-        elif isinstance(value, str):
-            self.add_aws_account_id(value)
+    @deleted.setter
+    def deleted(self, deleted: date | None):
+        if deleted is None or isinstance(deleted, date):
+            self.__deleted = deleted
         else:
-            for account_id in value:
-                self.add_aws_account_id(account_id)
+            self.__deleted = dateparser.isoparse(deleted) # TODO Use datetime.fromisoformat after we switch to python 3.11.
 
-    def add_aws_account_id(self, value: str) -> None:
+    @property
+    def human_readable_original_location(self) -> str | None:
         """
-        Adds a REST resource to the list of resources that are served by this component.
-        :param value: a Resource object.
+        The object's original location in human readable form. By default, it
+        mirrors the value of the original_location property.
         """
-        account = AccountAssociation()
-        account.actual_object_id = value
-        account.actual_object_type_name = AWSAccount.get_type_name()
-        self.__accounts[deepcopy(account)] = None
-
-    def remove_aws_account_id(self, value: str) -> None:
-        """
-        Removes a REST aws_account_id from the list of ids that are served by this organization. Ignores None values.
-        :param value: str representing the aws account id.
-        :raises ValueError: if the value is not among this organization's AWS account ids.
-        """
-        account_to_remove: AccountAssociation | None = None
-        for account in self.__accounts:
-            if account.actual_object_type_name == AWSAccount.get_type_name() and account.actual_object_id == value:
-                account_to_remove = account
-                break
-        if account_to_remove is not None:
-            del self.__accounts[account_to_remove]
-        else:
-            raise ValueError(f'AWS account id {value} not found')
+        return self.original_location
+
+    @human_readable_original_location.setter
+    def human_readable_original_location(self, human_readable_original_location: str | None):
+        self.original_location = human_readable_original_location
 
     @property
-    def principal_investigator_id(self) -> Optional[str]:
-        """
-        The principal investigator People ID.
-        """
-        return self.__principal_investigator_id
+    def type_display_name(self) -> str:
+        return "Trash Item"
+
+
+class InVolumeTrashItem(TrashItem, HasSize, ABC):
+    """
+    Abstract base class for trash items in a volume's trash.
+    """
+    PATH_SEPARATOR = '/'
 
-    @principal_investigator_id.setter
-    def principal_investigator_id(self, principal_investigator_id: Optional[str]) -> None:
-        self.__principal_investigator_id = str(principal_investigator_id) \
-            if principal_investigator_id is not None else None
+    @abstractmethod
+    def __init__(self) -> None:
+        super().__init__()
+        self.__volume_id: str | None = None
 
     @property
-    def admin_ids(self) -> list[str]:
+    def volume_id(self) -> str | None:
         """
-        The organization manager ids.
+        The id of this item's volume.
         """
-        return [i for i in self.__admin_ids] if self.__admin_ids else []
+        return self.__volume_id
 
-    @admin_ids.setter
-    def admin_ids(self, admin_ids: list[str]) -> None:
-        if admin_ids is None:
-            self.__admin_ids = []
-        elif not isinstance(admin_ids, str):
-            self.__admin_ids = [str(i) for i in admin_ids]
-        else:
-            self.__admin_ids = [str(admin_ids)]
+    @volume_id.setter
+    def volume_id(self, volume_id: str | None) -> None:
+        self.__volume_id = str(volume_id) if volume_id is not None else None
 
-    def add_admin_id(self, value: str) -> None:
-        self.__admin_ids.append(str(value))
 
-    def remove_admin_id(self, value: str) -> None:
-        """
-        Removes a REST manager id from the list of ids that are served by this organization. Ignores None values.
-        :param value:  str representing the manager id.
-        """
-        self.__admin_ids.remove(str(value))
+
+class AWSS3FolderFileTrashItem(InVolumeTrashItem, S3StorageClassMixin):
+    """
+    Trash items from Amazon Web Services Simple Storage Service buckets.
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.__version: str | None = None
 
     @property
-    def manager_ids(self) -> list[str]:
+    def id(self) -> str | None:
+        key_ = self.key
+        version_ = self.version
+        return encode_key(key_) + ',' + version_ if key_ and version_ else None
+
+    @id.setter
+    def id(self, id_: str | None):
+        try:
+            id__ = str(id_) if id_ is not None else None
+            if id__ is not None and ',' not in id__:
+                raise ValueError(f'Invalid value {id_}')
+            key_, version_ = id__.split(',', 1) if id__ is not None else (None, None)
+            self.key = decode_key(key_) if key_ is not None else None
+            self.version = version_ if version_ is not None else None
+        except KeyDecodeException as e:
+            raise ValueError(f'Invalid value {id_}') from e
+
+    @property
+    def name(self) -> str | None:
+        return self.id
+
+    @name.setter
+    def name(self, name: str | None):
+        self.id = name
+
+    @property
+    def version(self) -> str | None:
+        return self.__version
+
+    @version.setter
+    def version(self, version: str | None):
+        self.__version = str(version) if version is not None else None
+
+    @property
+    def key(self) -> str | None:
         """
-        The organization manager ids.
+        The object's key.
         """
-        return [i for i in self.__manager_ids] if self.__manager_ids else []
-
-    @manager_ids.setter
-    def manager_ids(self, manager_ids: list[str]) -> None:
-        if manager_ids is None:
-            self.__manager_ids = []
-        elif not isinstance(manager_ids, str):
-            self.__manager_ids = [str(i) for i in manager_ids]
+        try:
+            return self.__key
+        except AttributeError:
+            self.__key: str | None = None
+            return self.__key
+
+    @key.setter
+    def key(self, key: str | None):
+        if key:
+            self.__key = key
+            if self.__key is not None and is_folder(self.__key):
+                key_: str | None = self.__key.strip('/')
+            else:
+                key_ = self.__key
+            if key_ is not None:
+                self.__display_name: str | None = key_.rsplit('/', maxsplit=1)[-1]
+            else:
+                self.__display_name = None
         else:
-            self.__manager_ids = [str(manager_ids)]
-
-    def add_manager_id(self, value: str) -> None:
-        self.__manager_ids.append(str(value))
+            self.__display_name = None
 
-    def remove_manager_id(self, value: str) -> None:
+    @property
+    def display_name(self) -> str:
         """
-        Removes a REST manager id from the list of ids that are served by this organization. Ignores None values.
-        :param value:  str representing the manager id.
+        The object's display name. It's the last part of the object's key, minus any trailing slash for folders.
+        Setting this property will make this item a file.
         """
-        self.__manager_ids.remove(str(value))
+        try:
+            result = self.__display_name
+        except AttributeError:
+            self.__display_name = None
+            result = self.__display_name
+        return result if result is not None else super().display_name  # type: ignore
+
+    @display_name.setter
+    def display_name(self, display_name: str):
+        if display_name is not None:
+            if '/' in display_name:
+                raise ValueError(f'display_name {display_name} cannot contain slashes')
+            try:
+                key = self.__key
+                old_key = key
+            except AttributeError:
+                key = None
+                old_key = None
+            key_end_part = f'{display_name}/' if self.actual_object_type_name and issubclass(
+                desktop_object_type_for_name(self.actual_object_type_name), AWSS3Folder) else f'{display_name}'
+            if key is not None:
+                key_rsplit = key[:-1].rsplit('/', 1)
+                if len(key_rsplit) > 1:
+                    key = key_rsplit[-2] + f'/{key_end_part}' if len(key_rsplit) > 1 else key_end_part
+                else:
+                    key = f'{key_end_part}'
+            else:
+                key = f'{key_end_part}'
+            if old_key and old_key.endswith('/'):
+                self.key = key + '/' if not key.endswith('/') else ''
+            else:
+                self.key = key
 
     @property
-    def member_ids(self) -> list[str]:
+    def s3_uri(self) -> str | None:
         """
-        The organization member ids.
+        The object's S3 URI, computed from the bucket id and the id field.
         """
-        return [i for i in self.__member_ids]
+        return s3_uri(self.bucket_id, self.key)
 
-    @member_ids.setter
-    def member_ids(self, member_ids: list[str]) -> None:
-        if member_ids is None:
-            self.__member_ids = []
-        elif not isinstance(member_ids, str):
-            self.__member_ids = [str(i) for i in member_ids]
+    @s3_uri.setter
+    def s3_uri(self, s3_uri: str | None):
+        """
+        The object's S3 URI, computed from the bucket id and the id field.
+        """
+        match = S3_URI_PATTERN.fullmatch(s3_uri) if s3_uri else None
+        if match:
+            bucket_and_key = match.groupdict()
+            self.bucket_id = bucket_and_key['bucket']
+            self.key = bucket_and_key['key']
+        elif s3_uri is not None:
+            raise ValueError(f'Invalid s3 URI {s3_uri}')
         else:
-            self.__member_ids = [str(member_ids)]
+            self.bucket_id = None
+            self.key = None
 
-    def add_member_id(self, value: str) -> None:
-        self.__member_ids.append(str(value))
-
-    def remove_member_id(self, value: str) -> None:
+    @property
+    def bucket_id(self) -> str | None:
         """
-        Removes a REST member id from the list of member ids that are served by this organization. Ignores None values.
-        :param value: a str representing the member id.
+        The object's bucket name.
         """
-        self.__member_ids.remove(str(value))
+        try:
+            return self.__bucket_id
+        except AttributeError:
+            self.__bucket_id: str | None = None
+            return self.__bucket_id
+
+    @bucket_id.setter
+    def bucket_id(self, bucket_id: str | None):
+        self.__bucket_id = bucket_id
 
-    def dynamic_permission(self, sub: str) -> list[Permission]:
+    @property
+    def actual_object_id(self) -> str | None:
         """
-        Returns permissions if the sub is in the member_ids list, or an empty list if not.
+        Gets the id of the actual object in the trash. It is always the same
+        as this object's id. Setting this property also sets the id property
+        and vice versa.
+        """
+        key_ = self.key
+        return encode_key(key_) if key_ is not None else None
+
+    @actual_object_id.setter
+    def actual_object_id(self, actual_object_id: str | None):
+        self.key = decode_key(actual_object_id) if actual_object_id is not None else None
 
-        :param sub: the user id (required).
-        :return: A list containing Permissions or the empty list.
-        """
-        try:
-            perms: set[Permission] = set()
-            if sub == self.principal_investigator_id:
-                perms.add(Permission.COOWNER)
+    @property
+    def actual_object_type_name(self) -> str | None:
+        return self.__actual_object_type_name
+
+    @actual_object_type_name.setter
+    def actual_object_type_name(self, actual_object_type_name: str | None):
+        if actual_object_type_name:
+            type_ = desktop_object_type_for_name(actual_object_type_name)
+            if issubclass(type_, AWSS3Folder):
+                key = self.key
+                if key and not key.endswith('/'):
+                    self.key = key + '/'
+            elif issubclass(type_, AWSS3FileObject):
+                key = self.key
+                if key and key.endswith('/'):
+                    self.key = key[:-1]
             else:
-                for p_id in permission_id_dict:
-                    if sub in getattr(self, p_id):
-                        perms.update(permission_id_dict[p_id])
-            return list(perms)
-        except:
-            logging.exception('Permissions are not correctly configured...returning empty permissions set')
-            return []
+                raise TypeError(f'Type must be {AWSS3Folder} or {AWSS3FileObject} but was {type_}')
+            self.__actual_object_type_name = actual_object_type_name
+        else:
+            key = self.key
+            if key and key.endswith('/'):
+                self.key = key[:-1]
+            self.__actual_object_type_name = None
 
     @property
-    def type_display_name(self) -> str:
-        return "Organization"
+    def original_location(self) -> str | None:
+        return f'/{self.bucket_id}/{self.key}' if self.bucket_id and self.key else None
+
+    @original_location.setter
+    def original_location(self, original_location: str | None):
+        path_as_list = original_location.split(self.PATH_SEPARATOR)
+        self.bucket_id = path_as_list[1]
+        try:
+            self.key = self.PATH_SEPARATOR.join(path_as_list[2:])
+        except KeyDecodeException as e:
+            raise ValueError(f'Invalid original location {original_location}') from e
```

### Comparing `heaobject-1.4.0/src/heaobject/person.py` & `heaobject-1.5.0/src/heaobject/person.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,26 +190,27 @@
     A user group, for authorization purposes. The id and name attributes are synchronized with the group attribute such
     that setting one automatically populates the others.
     """
     def __init__(self):
         super().__init__()
         self.__group: str | None = None
         self.__display_name: str | None = None
+        self.__id: str | None = None
 
     @property
     def id(self) -> str | None:
         """
         The group, base64-encoded using this module's encode_group() function. Setting this attribute automatically
         generates values for the name and group attributes.
         """
-        return self.name
+        return self.__id
 
     @id.setter
     def id(self, id_: str | None):
-        self.name = id_
+        self.__id = str(id_) if id_ is not None else None
 
     @property
     def name(self) -> str | None:
         """
         The group, base64-encoded using this module's encode_group() function. Setting this attribute automatically
         generates values for the id and group attributes.
         """
@@ -311,13 +312,13 @@
     """
     return [get_system_person(id_) for id_ in _system_user_display_names]
 
 
 _validate_email = partial(validate_email, check_deliverability=False)
 
 _system_user_display_names = {
-    NONE_USER: 'No user',
+    NONE_USER: 'None',
     ALL_USERS: 'All users',
     TEST_USER: 'Test user',
     SOURCE_USER: 'Source user',
     AWS_USER: 'AWS account holder'
 }
```

### Comparing `heaobject-1.4.0/src/heaobject/project.py` & `heaobject-1.5.0/src/heaobject/project.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.4.0/src/heaobject/registry.py` & `heaobject-1.5.0/src/heaobject/registry.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.4.0/src/heaobject/root.py` & `heaobject-1.5.0/src/heaobject/root.py`

 * *Files 2% similar despite different names*

```diff
@@ -352,15 +352,17 @@
 class MemberObject(HEAObject, abc.ABC):
     """
     Interface for HEA objects that have a part-of relationship with a desktop objects and whose lifecycle is
     managed by the desktop object. Owned objects have the same permissions as the owning desktop object. As a result,
     they can be accessed by anyone who can access the desktop object, and they can be modified by anyone who can modify
     the desktop object.
     """
-    pass
+    @abc.abstractmethod
+    def get_member_attribute_permissions(self, sub: str, desktop_object: 'DesktopObject', attr: str) -> list[Permission]:
+        pass
 
 
 class PermissionAssignment(MemberObject, abc.ABC):
     """
     Interface for permission assignments for desktop objects. Desktop objects are owned by the user who created them.
     After creating an object, the object's owner can share the object with other users with the desired set of
     permissions. Optionally, users can invite another users to access the object with the desired set of permissions,
@@ -463,15 +465,17 @@
     object type. Additional HEA microservices may implement actions that use specific desktop object types.
 
     Desktop objects implement no capability to check the current user when getting and setting owned objects, and
     different users may only have access to a subset of its owned objects. Similarly, owned objects have no knowledge of
     permissions at all. It is imperative that users gain access to desktop objects by calling an appropriate HEA
     microservice as themselves, which will filter the owned objects that are returned according to their permissions.
 
-    Desktop objects may employ three authorization mechanisms:
+    Desktop objects may employ three permissions mechanisms. These permissions do not affect whether a user may get
+    or set attribute values of a desktop object, but they may be used to determine whether to return a desktop object
+    to a user or save the desktop object with a user's changes.
 
     1) User-based: if the user is the object's owner, then the user can do anything with the object.
     2) Shares-based: if the owner has shared the object with a user, then the user can use the object according to the
     values of the heaobject.root.Permission enum.
     3) Dynamic permissions: Implemented using the dynamic_permission function, it uses the object's field values to
     determine the user's permissions. It will only be invoked if the user has some level of shares-based permission. In
     the absence of the object actually having been shared with a user, a Share object can be added to the shares list
@@ -479,14 +483,21 @@
     traverse relationships between objects via their *_id fields so that related objects' field values might be used to
     determine permissions.
 
     The level of permissions granted will be the greatest of the 3 approaches. Being an object's owner trumps
     everything. The shares-based and dynamic permissions-based approaches both return heaobject.root.Permission objects,
     and in the event of conflicting Permissions, the most permissive permissions will prevail.
 
+    Furthermore, desktop objects support attribute-level permissions, implemented by the get_attribute_permissions
+    function. Attribute may have Permission.VIEWER and/or Permission.EDITOR permissions. The default implementation of
+    get_attribute_permissions grants the id, modified, and created attributes only Permission.VIEWER permissions, and
+    it grants all other attributes Permission.VIEWER and Permission.EDITOR permissions. Object-level permissions
+    override attribute-level permissions. For example, an object cannot grant a user Permission.EDITOR permissions to
+    an attribute if the user's object-level permissions do not include Permission.EDITOR or Permission.COOWNER.
+
     Desktop objects may have a class variable, associations, with type Dict[property, str]. For properties ending in
     _id or _ids that represent an association relationship with another desktop object type, it defines the type name
     of the desktop object being referred to. The associations variable is intended to have many purposes. In the future,
     implementations of the dynamic_permission() method might use these annotations to traverse an association
     relationship to another desktop object as part of permissions checking.
     """
 
@@ -753,14 +764,36 @@
         :param sub: the user (required).
         :param perms: the permissions to check (required), which may be passed as an iterable of Permission objects or
         an object adhering to the PermissionGroup protocol.
         :return: True or False.
         """
         pass
 
+    @abc.abstractmethod
+    def get_attribute_permissions(self, sub: str, attr: str) -> list[Permission]:
+        """
+        Gets the subject's permissions for the specified attribute of this object.
+
+        :param sub: the user (required).
+        :param attr: the attribute to check (required).
+        :return: list of Permission.VIEWER and/or Permission.EDITOR, or the empty list.
+        """
+        pass
+
+    @abc.abstractmethod
+    def is_attribute_read_only(self, sub: str, attr: str) -> bool:
+        """
+        Uses the subject's permissions to determine whether the given attribute is read-only.
+
+        :param sub: the user (required).
+        :param attr: the attribute to check (required).
+        :return: True or False.
+        """
+        pass
+
     @classmethod
     @abc.abstractmethod
     def get_subclasses(cls) -> Iterator[Type['DesktopObject']]:
         """
         Returns an iterator of subclasses of this class that have previously been loaded into the python interpreter.
         :return: an iterator of DesktopObject types.
         """
@@ -886,14 +919,34 @@
     def get_attributes(self) -> Iterator[str]:
         type_ = type(self)
         if type_._attributes is None:
             type_._attributes = _get_attributes(self, type_.__get_type_attributes())
         self.__attributes.update(type_._attributes)
         return iter(self.__attributes)
 
+    def _default_get_attribute_permissions(self, sub: str, attr: str) -> list[Permission]:
+        """
+        Default implementation for getting the subject's permissions for the specified attribute of this object.
+
+        :param sub: the user (required).
+        :param attr: the attribute to check (required).
+        :return: list of Permission.VIEWER and/or Permission.EDITOR, or the empty list.
+        """
+        whole_object_perms = set(self.get_permissions(sub))
+        perms: list[Permission] = []
+        if Permission.COOWNER in whole_object_perms:
+            perms.append(Permission.EDITOR)
+            perms.append(Permission.VIEWER)
+            return perms
+        if Permission.EDITOR in whole_object_perms:
+            perms.append(Permission.EDITOR)
+        if Permission.VIEWER in whole_object_perms:
+            perms.append(Permission.VIEWER)
+        return perms
+
     @classmethod
     def __get_type_attributes(cls):
         if cls._type_attributes is None:
             cls._type_attributes = _get_type_attributes(cls)
         return cls._type_attributes
 
     def get_all_attributes(self) -> Iterator[str]:
@@ -973,14 +1026,17 @@
     composition relationship in UML. Owned objects have the same permissions as the owning desktop object. As a result,
     they can be accessed by anyone who can access the desktop object, and they can be modified by anyone who can modify
     the desktop object.
     """
     def __new__(cls, *args, **kwargs):
         return make_abstract(AbstractMemberObject, cls, *args, **kwargs)
 
+    def get_member_attribute_permissions(self, sub: str, desktop_object: 'DesktopObject', attr: str) -> list[Permission]:
+        return self._default_get_attribute_permissions(sub, attr)
+
 
 class VersionedDesktopObject(DesktopObject, abc.ABC):
     """
     Interface for desktop objects that can be versioned.
     """
     @property  # type: ignore
     @abc.abstractmethod
@@ -1311,15 +1367,15 @@
         Default implementation that returns an empty list, signifying no permissions.
 
         :param sub: the user id.
         :return: an empty list.
         """
         return []
 
-    def get_permissions(self, sub: str) -> List[Permission]:
+    def get_permissions(self, sub: str) -> list[Permission]:
         if sub is None:
             raise ValueError('sub cannot be None')
 
         if self.owner == sub:
             return list(p for p in Permission)
 
         result = set(perm for share in self.__shares for perm in share.permissions
@@ -1341,14 +1397,36 @@
         else:
             perms_ = perms
 
         return self.owner == sub or \
                any(perm is not Permission.CHECK_DYNAMIC and perm in user_perms for perm in perms_) or \
                ((Permission.CHECK_DYNAMIC in user_perms) and any(perm in perms_ for perm in self.dynamic_permission(sub)))
 
+    def get_attribute_permissions(self, sub: str, attr: str) -> list[Permission]:
+        """
+        Default implementation for getting the subject's permissions for the specified attribute of this object.
+
+        :param sub: the user (required).
+        :param attr: the attribute to check (required).
+        :return: list of Permission.VIEWER and/or Permission.EDITOR, or the empty list.
+        """
+        if attr in ('id', 'type', 'created', 'modified'):
+            return [Permission.VIEWER]
+        elif attr == 'owner' and sub != getattr(self, attr):
+            return [Permission.VIEWER]
+        elif attr in ('shares', 'invites'):
+            perms = self.get_permissions(sub)
+            if Permission.COOWNER not in perms and Permission.SHARER not in perms:
+                return [Permission.VIEWER]
+        return self._default_get_attribute_permissions(sub, attr)
+
+    def is_attribute_read_only(self, sub: str, attr: str) -> bool:
+        permissions = self.get_attribute_permissions(sub, attr)
+        return Permission.VIEWER in permissions and (Permission.EDITOR not in permissions and Permission.COOWNER not in permissions)
+
     @classmethod
     def get_subclasses(cls) -> Iterator[Type['AbstractDesktopObject']]:
         for subclass in cls.__subclasses__():
             yield from subclass.get_subclasses()
             yield subclass
 
     def __default_display_name(self):
@@ -1542,15 +1620,15 @@
         self.__name = str(name) if name is not None else None
 
     def __eq__(self, other):
         """
         Overrides the default equality implementation. Objects of the same type and that have the same values for the
         actual_object_type_name, actual_object_id, and name attributes are equal.
         """
-        if self is not type(other):
+        if type(self) is not type(other):
             return False
         if self.actual_object_type_name != other.actual_object_type_name:
             return False
         if self.actual_object_id != other.actual_object_id:
             return False
         if self.name != other.name:
             return False
```

### Comparing `heaobject-1.4.0/src/heaobject/settings.py` & `heaobject-1.5.0/src/heaobject/settings.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.4.0/src/heaobject/source2target.py` & `heaobject-1.5.0/src/heaobject/source2target.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.4.0/src/heaobject/storage.py` & `heaobject-1.5.0/src/heaobject/storage.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.4.0/src/heaobject/user.py` & `heaobject-1.5.0/src/heaobject/user.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.4.0/src/heaobject/volume.py` & `heaobject-1.5.0/src/heaobject/volume.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.4.0/src/heaobject.egg-info/PKG-INFO` & `heaobject-1.5.0/src/heaobject.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaobject
-Version: 1.4.0
+Version: 1.5.0
 Summary: Data and other classes that are passed into and out of HEA REST APIs.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,18 @@
 Requires-Dist: mimetype-description~=0.1.0
 
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.5.0
+* Added attribute-level permissions.
+* Fixed bug in checking equality of AbstractAssociation objects.
+
 ## Version 1.4.0
 * Added "deleted" attribute to the trash module's TrashItem class.
 * Added Group class to the person module.
 
 ## Version 1.3.0
 * Added type_display_name attribute to all HEA objects.
```

### Comparing `heaobject-1.4.0/src/heaobject.egg-info/SOURCES.txt` & `heaobject-1.5.0/src/heaobject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

