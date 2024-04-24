# Comparing `tmp/heaserver_accounts-1.0.7.tar.gz` & `tmp/heaserver_accounts-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver_accounts-1.0.7.tar", last modified: Thu Apr 18 04:12:15 2024, max compression
+gzip compressed data, was "heaserver_accounts-1.1.0.tar", last modified: Wed Apr 24 18:02:43 2024, max compression
```

## Comparing `heaserver_accounts-1.0.7.tar` & `heaserver_accounts-1.1.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 04:12:15.219425 heaserver_accounts-1.0.7/
--rw-rw-rw-   0        0        0      261 2023-12-18 18:51:28.000000 heaserver_accounts-1.0.7/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 18:51:28.000000 heaserver_accounts-1.0.7/.gitignore
--rw-rw-rw-   0        0        0     1624 2023-12-18 18:51:28.000000 heaserver_accounts-1.0.7/Dockerfile
--rw-rw-rw-   0        0        0    11625 2023-12-18 18:51:28.000000 heaserver_accounts-1.0.7/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 18:51:28.000000 heaserver_accounts-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     5755 2024-04-18 04:12:15.217424 heaserver_accounts-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     4447 2024-04-18 04:05:48.000000 heaserver_accounts-1.0.7/README.md
--rw-rw-rw-   0        0        0     1878 2023-12-18 18:51:28.000000 heaserver_accounts-1.0.7/RELEASING.md
--rw-rw-rw-   0        0        0      441 2023-12-18 18:51:28.000000 heaserver_accounts-1.0.7/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-04-18 04:12:14.988009 heaserver_accounts-1.0.7/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-04-18 04:12:14.988009 heaserver_accounts-1.0.7/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-18 04:12:15.139874 heaserver_accounts-1.0.7/integrationtests/heaserver/accountintegrationtest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.0.7/integrationtests/heaserver/accountintegrationtest/__init__.py
--rw-rw-rw-   0        0        0      481 2023-12-18 18:51:28.000000 heaserver_accounts-1.0.7/integrationtests/heaserver/accountintegrationtest/test_all.py
--rw-rw-rw-   0        0        0     7797 2024-04-09 21:25:34.000000 heaserver_accounts-1.0.7/integrationtests/heaserver/accountintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 18:51:28.000000 heaserver_accounts-1.0.7/pytest.ini
--rw-rw-rw-   0        0        0      262 2023-12-18 18:51:28.000000 heaserver_accounts-1.0.7/requirements_dev.txt
--rw-rw-rw-   0        0        0     4294 2023-12-18 18:51:28.000000 heaserver_accounts-1.0.7/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-04-18 04:12:15.219425 heaserver_accounts-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1825 2024-04-18 04:11:35.000000 heaserver_accounts-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 04:12:14.991011 heaserver_accounts-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-18 04:12:14.990011 heaserver_accounts-1.0.7/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-18 04:12:15.142906 heaserver_accounts-1.0.7/src/heaserver/account/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.0.7/src/heaserver/account/__init__.py
--rw-rw-rw-   0        0        0    45036 2024-04-05 19:52:47.000000 heaserver_accounts-1.0.7/src/heaserver/account/service.py
-drwxrwxrwx   0        0        0        0 2024-04-18 04:12:15.144906 heaserver_accounts-1.0.7/src/heaserver/account/wstl/
--rw-rw-rw-   0        0        0    11652 2024-04-09 21:25:34.000000 heaserver_accounts-1.0.7/src/heaserver/account/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-04-18 04:12:15.216424 heaserver_accounts-1.0.7/src/heaserver_accounts.egg-info/
--rw-rw-rw-   0        0        0     5755 2024-04-18 04:12:14.000000 heaserver_accounts-1.0.7/src/heaserver_accounts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      844 2024-04-18 04:12:14.000000 heaserver_accounts-1.0.7/src/heaserver_accounts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 04:12:14.000000 heaserver_accounts-1.0.7/src/heaserver_accounts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-18 04:12:14.000000 heaserver_accounts-1.0.7/src/heaserver_accounts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-18 04:12:14.000000 heaserver_accounts-1.0.7/src/heaserver_accounts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-18 04:12:14.000000 heaserver_accounts-1.0.7/src/heaserver_accounts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-18 04:12:14.992010 heaserver_accounts-1.0.7/tests/
-drwxrwxrwx   0        0        0        0 2024-04-18 04:12:14.993010 heaserver_accounts-1.0.7/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-18 04:12:15.214424 heaserver_accounts-1.0.7/tests/heaserver/accounttest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.0.7/tests/heaserver/accounttest/__init__.py
--rw-rw-rw-   0        0        0     7626 2024-04-09 21:25:34.000000 heaserver_accounts-1.0.7/tests/heaserver/accounttest/test_all.py
--rw-rw-rw-   0        0        0     5195 2024-04-09 21:25:34.000000 heaserver_accounts-1.0.7/tests/heaserver/accounttest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.398248 heaserver_accounts-1.1.0/
+-rw-rw-rw-   0        0        0      261 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/.gitignore
+-rw-rw-rw-   0        0        0     1624 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5916 2024-04-24 18:02:43.397247 heaserver_accounts-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4608 2024-04-24 17:52:12.000000 heaserver_accounts-1.1.0/README.md
+-rw-rw-rw-   0        0        0     1878 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/RELEASING.md
+-rw-rw-rw-   0        0        0      441 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.330245 heaserver_accounts-1.1.0/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.330245 heaserver_accounts-1.1.0/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.351247 heaserver_accounts-1.1.0/integrationtests/heaserver/accountintegrationtest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/integrationtests/heaserver/accountintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0      481 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/integrationtests/heaserver/accountintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0     7797 2024-04-09 21:25:34.000000 heaserver_accounts-1.1.0/integrationtests/heaserver/accountintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/pytest.ini
+-rw-rw-rw-   0        0        0      262 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0     4294 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-04-24 18:02:43.399248 heaserver_accounts-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1825 2024-04-24 18:02:07.000000 heaserver_accounts-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.332245 heaserver_accounts-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.331245 heaserver_accounts-1.1.0/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.354251 heaserver_accounts-1.1.0/src/heaserver/account/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/src/heaserver/account/__init__.py
+-rw-rw-rw-   0        0        0    45175 2024-04-24 17:47:43.000000 heaserver_accounts-1.1.0/src/heaserver/account/service.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.356246 heaserver_accounts-1.1.0/src/heaserver/account/wstl/
+-rw-rw-rw-   0        0        0    11652 2024-04-09 21:25:34.000000 heaserver_accounts-1.1.0/src/heaserver/account/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.395248 heaserver_accounts-1.1.0/src/heaserver_accounts.egg-info/
+-rw-rw-rw-   0        0        0     5916 2024-04-24 18:02:43.000000 heaserver_accounts-1.1.0/src/heaserver_accounts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      844 2024-04-24 18:02:43.000000 heaserver_accounts-1.1.0/src/heaserver_accounts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 18:02:43.000000 heaserver_accounts-1.1.0/src/heaserver_accounts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-24 18:02:43.000000 heaserver_accounts-1.1.0/src/heaserver_accounts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-24 18:02:43.000000 heaserver_accounts-1.1.0/src/heaserver_accounts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-24 18:02:43.000000 heaserver_accounts-1.1.0/src/heaserver_accounts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.332245 heaserver_accounts-1.1.0/tests/
+drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.333245 heaserver_accounts-1.1.0/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.393247 heaserver_accounts-1.1.0/tests/heaserver/accounttest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/tests/heaserver/accounttest/__init__.py
+-rw-rw-rw-   0        0        0     7626 2024-04-09 21:25:34.000000 heaserver_accounts-1.1.0/tests/heaserver/accounttest/test_all.py
+-rw-rw-rw-   0        0        0     5460 2024-04-23 22:20:38.000000 heaserver_accounts-1.1.0/tests/heaserver/accounttest/testcase.py
```

### Comparing `heaserver_accounts-1.0.7/Dockerfile` & `heaserver_accounts-1.1.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.0.7/LICENSE` & `heaserver_accounts-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.0.7/PKG-INFO` & `heaserver_accounts-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-accounts
-Version: 1.0.7
+Version: 1.1.0
 Summary: Manages account information
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-accounts,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,28 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.4.1
+Requires-Dist: heaserver~=1.5.0
 
 # HEA Server AWS Accounts Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server AWS Accounts Microservice is It manages the AWS account information details.
 
+## Version 1.1.0
+* Removed the PUT and DELETE account calls because neither works.
+
+## Version 1.0.8
+* Addressed occasional slowdown getting one account.
+
 ## Version 1.0.7
 * Addressed occasional slowdown getting accounts.
 
 ## Version 1.0.6
 * Display type display name in properties card, and return the type display name from GET calls.
 
 ## Version 1.0.5
```

### Comparing `heaserver_accounts-1.0.7/README.md` & `heaserver_accounts-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # HEA Server AWS Accounts Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server AWS Accounts Microservice is It manages the AWS account information details.
 
+## Version 1.1.0
+* Removed the PUT and DELETE account calls because neither works.
+
+## Version 1.0.8
+* Addressed occasional slowdown getting one account.
+
 ## Version 1.0.7
 * Addressed occasional slowdown getting accounts.
 
 ## Version 1.0.6
 * Display type display name in properties card, and return the type display name from GET calls.
 
 ## Version 1.0.5
```

### Comparing `heaserver_accounts-1.0.7/RELEASING.md` & `heaserver_accounts-1.1.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.0.7/integrationtests/heaserver/accountintegrationtest/testcase.py` & `heaserver_accounts-1.1.0/integrationtests/heaserver/accountintegrationtest/testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.0.7/run-swaggerui.py` & `heaserver_accounts-1.1.0/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.0.7/setup.py` & `heaserver_accounts-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-accounts',
-    version='1.0.7',
+    version='1.1.0',
     description="Manages account information",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.account'],
     package_data={'heaserver.account': ['wstl/*.json']},
     install_requires=[
-        'heaserver~=1.4.1'
+        'heaserver~=1.5.0'
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
```

### Comparing `heaserver_accounts-1.0.7/src/heaserver/account/service.py` & `heaserver_accounts-1.1.0/src/heaserver/account/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                                                 activity_cb=publish_desktop_object) as activity:
         sub = request.headers.get(SUB, NONE_USER)
         cache_key = (sub, f'id^{request.match_info["id"]}')
         cached_value = request.app[HEA_CACHE].get(cache_key)
         if cached_value is not None:
             account_dict, volume_id = cached_value
         else:
-            account, volume_id = await _get_account_by_id(request)
+            account, volume_id = await _get_awsaccount_by_id(request)
             logger.debug('Got account %s and volume %s', account, volume_id)
             if account is None:
                 raise response.status_not_found()
             account_dict = account.to_dict()
             request.app[HEA_CACHE][cache_key] = (account_dict, volume_id)
             request.app[HEA_CACHE][(sub, f'volume_id^{volume_id}')] = (account_dict, volume_id)
         request.match_info['volume_id'] = volume_id
@@ -385,74 +385,74 @@
 #     :return: the requested awsaccounts or Not Found.
 #
 #     FIXME: should only be permitted by an AWS organization administrator, I would think. Need to sort out what the call looks like.
 #     """
 #     return await awsservicelib.post_account(request)
 
 
-@routes.put('/volumes/{volume_id}/awsaccounts/me')
-async def put_account_awsaccounts(request: web.Request) -> web.Response:
-    """
-    Puts the awsaccounts information given the correct access key and secret access key.
-
-    :param request: the HTTP request.
-    :return: the requested awsaccounts or Not Found.
-    """
-    volume_id = request['volume_id']
-    alt_contact_type = request.match_info.get("alt_contact_type", None)
-    email_address = request.match_info.get("email_address", None)
-    name = request.match_info.get("name", None)
-    phone = request.match_info.get("phone", None)
-    title = request.match_info.get("title", None)
+# @routes.put('/volumes/{volume_id}/awsaccounts/me')
+# async def put_account_awsaccounts(request: web.Request) -> web.Response:
+#     """
+#     Puts the awsaccounts information given the correct access key and secret access key.
 
-    async with DesktopObjectActionLifecycle(request=request,
-                                                code='hea-delete',
-                                                description=f'Updating my AWS account',
-                                                activity_cb=publish_desktop_object) as activity:
-        activity.old_object_type_name = AWSAccount.get_type_name()
-        activity.old_object_uri = f'volumes/{volume_id}/awsaccounts/me'
-        activity.old_volume_id = volume_id
-        try:
-            async with aws.AccountClientContext(request, volume_id) as acc_client:
-                async with aws.STSClientContext(request, volume_id) as sts_client:
-                    def do() -> str:
-                        account_id = sts_client.get_caller_identity().get('Account')
-                        acc_client.put_alternate_contact(AccountId=account_id, AlternateContactType=alt_contact_type,
-                                                        EmailAddress=email_address, Name=name, PhoneNumber=phone, Title=title)
-                        return account_id
-                    account_id = await get_running_loop().run_in_executor(None, do)
-                    sub = request.headers.get(SUB, NONE_USER)
-                    request.app[HEA_CACHE].pop((sub, f'volume_id^{volume_id}'), None)
-                    request.app[HEA_CACHE].pop((sub, f'id^{account_id}'), None)
-                    keys_to_delete = []
-                    for key in request.app[HEA_CACHE]:
-                        if key[1] is None:
-                            keys_to_delete.append(key)
-                    for key in keys_to_delete:
-                        request.app[HEA_CACHE].pop(key, None)
-                    activity.new_object_type_name = AWSAccount.get_type_name()
-                    activity.new_object_uri = f'volumes/{volume_id}/awsaccounts/me'
-                    activity.new_volume_id = volume_id
-            return web.HTTPNoContent()
-        except BotoClientError as e:
-            activity.status = Status.FAILED
-            return web.HTTPBadRequest()
+#     :param request: the HTTP request.
+#     :return: the requested awsaccounts or Not Found.
+#     """
+#     volume_id = request['volume_id']
+#     alt_contact_type = request.match_info.get("alt_contact_type", None)
+#     email_address = request.match_info.get("email_address", None)
+#     name = request.match_info.get("name", None)
+#     phone = request.match_info.get("phone", None)
+#     title = request.match_info.get("title", None)
+
+#     async with DesktopObjectActionLifecycle(request=request,
+#                                                 code='hea-delete',
+#                                                 description=f'Updating my AWS account',
+#                                                 activity_cb=publish_desktop_object) as activity:
+#         activity.old_object_type_name = AWSAccount.get_type_name()
+#         activity.old_object_uri = f'volumes/{volume_id}/awsaccounts/me'
+#         activity.old_volume_id = volume_id
+#         try:
+#             async with aws.AccountClientContext(request, volume_id) as acc_client:
+#                 async with aws.STSClientContext(request, volume_id) as sts_client:
+#                     def do() -> str:
+#                         account_id = sts_client.get_caller_identity().get('Account')
+#                         acc_client.put_alternate_contact(AccountId=account_id, AlternateContactType=alt_contact_type,
+#                                                         EmailAddress=email_address, Name=name, PhoneNumber=phone, Title=title)
+#                         return account_id
+#                     account_id = await get_running_loop().run_in_executor(None, do)
+#                     sub = request.headers.get(SUB, NONE_USER)
+#                     request.app[HEA_CACHE].pop((sub, f'volume_id^{volume_id}'), None)
+#                     request.app[HEA_CACHE].pop((sub, f'id^{account_id}'), None)
+#                     keys_to_delete = []
+#                     for key in request.app[HEA_CACHE]:
+#                         if key[1] is None:
+#                             keys_to_delete.append(key)
+#                     for key in keys_to_delete:
+#                         request.app[HEA_CACHE].pop(key, None)
+#                     activity.new_object_type_name = AWSAccount.get_type_name()
+#                     activity.new_object_uri = f'volumes/{volume_id}/awsaccounts/me'
+#                     activity.new_volume_id = volume_id
+#             return web.HTTPNoContent()
+#         except BotoClientError as e:
+#             activity.status = Status.FAILED
+#             return web.HTTPBadRequest()
 
 
-@routes.delete('/volumes/{volume_id}/awsaccounts/me')
-async def delete_account_awsaccounts(request: web.Request) -> web.Response:
-    """
-    Deletes the awsaccounts information given the correct access key and secret access key.
+# @routes.delete('/volumes/{volume_id}/awsaccounts/me')
+# async def delete_account_awsaccounts(request: web.Request) -> web.Response:
+#     """
+#     Deletes the awsaccounts information given the correct access key and secret access key.
 
-    :param request: the HTTP request.
-    :return: the requested awsaccounts or Not Found.
+#     :param request: the HTTP request.
+#     :return: the requested awsaccounts or Not Found.
 
-    FIXME: should only be permitted by an AWS organization administrator, I would think. Need to sort out what the call looks like.
-    """
-    return response.status_not_found()
+#     FIXME: should only be permitted by an AWS organization administrator, I would think. Need to sort out what the call looks like.
+#     """
+#     return response.status_not_found()
 
 
 @routes.get('/awsaccounts/{id}/creator')
 @action('heaserver-accounts-awsaccount-create-bucket', rel='hea-creator hea-default application/x.bucket',
         path='awsaccounts/{id}/newbucket')
 async def get_account_creator(request: web.Request) -> web.Response:
     """
@@ -635,15 +635,15 @@
                                                 activity_cb=publish_desktop_object) as activity:
         sub = request.headers.get(SUB, NONE_USER)
         cache_key = (sub, f'id^{request.match_info["id"]}')
         cached_value = request.app[HEA_CACHE].get(cache_key)
         if cached_value is not None:
             account_dict, volume_id = cached_value
         else:
-            account, volume_id = await _get_account_by_id(request)
+            account, volume_id = await _get_awsaccount_by_id(request)
             if account is None:
                 return response.status_not_found()
             account_dict = account.to_dict()
             request.app[HEA_CACHE][cache_key] = account_dict
         activity.new_object_id = id_
         activity.new_object_type_name = AWSAccount.get_type_name()
         activity.new_object_uri = f'awsaccounts/{id_}'
@@ -876,28 +876,29 @@
     :param volume_id: the id string of the volume representing the user's AWS account.
     :return: an HTTP response with an AWSAccount object in the body.
     FIXME: a bad volume_id should result in a 400 status code; currently has status code 500.
     """
     return await request.app[HEA_DB].get_account(request, volume_id)
 
 
-async def _get_account_by_id(request: web.Request) -> tuple[AWSAccount | None, str | None]:
+async def _get_awsaccount_by_id(request: web.Request) -> tuple[AWSAccount | None, str | None]:
     """
     Gets an account by its id and the account's volume id. The id is expected to be the request object's match_info
     mapping, with key 'id'.
 
     :param request: an aiohttp Request object (required).
     :return: a two-tuple containing an AWSAccount dict and volume id, or None if no account was found.
     """
+    account_id = request.match_info['id']
     db = request.app[HEA_DB]
-    volume_ids = [volume.id async for volume in db.get_volumes(request, AWSFileSystem)]
-    try:
-        return await anext((a, v) async for a, v in db.get_accounts(request, volume_ids) if a.id == request.match_info['id'])
-    except StopAsyncIteration:
-        return (None, None)
+    async for volume in db.get_volumes(request, AWSFileSystem, account_ids=[account_id], account_type_names=[AWSAccount.get_type_name()]):
+        volume_id = volume.id
+        return await db.get_account(request, volume_id), volume_id
+    return (None, None)
+
 
 
 async def _get_account_by_name(request: web.Request) -> tuple[AWSAccount | None, str | None]:
     """
     Gets an account by its id and the account's volume id. The id is expected to be the request object's match_info
     mapping, with key 'id'.
```

### Comparing `heaserver_accounts-1.0.7/src/heaserver/account/wstl/all.json` & `heaserver_accounts-1.1.0/src/heaserver/account/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.0.7/src/heaserver_accounts.egg-info/PKG-INFO` & `heaserver_accounts-1.1.0/src/heaserver_accounts.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-accounts
-Version: 1.0.7
+Version: 1.1.0
 Summary: Manages account information
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-accounts,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,28 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.4.1
+Requires-Dist: heaserver~=1.5.0
 
 # HEA Server AWS Accounts Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server AWS Accounts Microservice is It manages the AWS account information details.
 
+## Version 1.1.0
+* Removed the PUT and DELETE account calls because neither works.
+
+## Version 1.0.8
+* Addressed occasional slowdown getting one account.
+
 ## Version 1.0.7
 * Addressed occasional slowdown getting accounts.
 
 ## Version 1.0.6
 * Display type display name in properties card, and return the type display name from GET calls.
 
 ## Version 1.0.5
```

### Comparing `heaserver_accounts-1.0.7/src/heaserver_accounts.egg-info/SOURCES.txt` & `heaserver_accounts-1.1.0/src/heaserver_accounts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.0.7/tests/heaserver/accounttest/test_all.py` & `heaserver_accounts-1.1.0/tests/heaserver/accounttest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.0.7/tests/heaserver/accounttest/testcase.py` & `heaserver_accounts-1.1.0/tests/heaserver/accounttest/testcase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Creates a test case class for use with the unittest library that is built into Python.
 """
 
 from heaserver.account import service
 from heaobject.user import NONE_USER
+from heaobject.account import AccountAssociation, AWSAccount
 from heaserver.service.testcase import microservicetestcase, expectedvalues
 from heaserver.service.testcase.mockaws import MockS3WithMockMongoManager
 from heaserver.service.sources import AWS
 
 db_store = {
     'filesystems': [{
         'id': '666f6f2d6261722d71757578',
@@ -38,15 +39,20 @@
         'owner': NONE_USER,
         'shares': [],
         'source': None,
         'type': 'heaobject.volume.Volume',
         'version': None,
         'file_system_name': 'DEFAULT_FILE_SYSTEM',
         'file_system_type': 'heaobject.volume.AWSFileSystem',
-        'credential_id': None  # Let boto3 try to find the user's credentials.
+        'credential_id': None,  # Let boto3 try to find the user's credentials.
+        'account': {
+            'type': AccountAssociation.get_type_name(),
+            'actual_object_type_name': AWSAccount.get_type_name(),
+            'actual_object_id': "123456789012"
+        }
     }],
     'awsaccounts': [
         {
             "alternate_contact_name": None,
             "alternate_email_address": None,
             "alternate_phone_number": None,
             "created": None,
@@ -62,15 +68,15 @@
             "modified": None,
             "name": "master",
             "owner": "system|aws",
             "phone_number": None,
             "shares": [],
             "source": AWS,
             "source_detail": AWS,
-            "type": "heaobject.account.AWSAccount",
+            "type": AWSAccount.get_type_name(),
             "type_display_name": "AWS Account"
         }
     ]}
 
 AWSAccountTestCase = \
     microservicetestcase.get_test_case_cls_default(
         href='http://localhost:8080/awsaccounts',
```

