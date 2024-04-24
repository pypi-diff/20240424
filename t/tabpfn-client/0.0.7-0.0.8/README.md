# Comparing `tmp/tabpfn_client-0.0.7.tar.gz` & `tmp/tabpfn_client-0.0.8.tar.gz`

## Comparing `tabpfn_client-0.0.7.tar` & `tabpfn_client-0.0.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/.gitmodules
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/README.md
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/quick_test.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/requirements.txt
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/.github/workflows/pull_request.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/.idea/.gitignore
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/.idea/misc.xml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/.idea/modules.xml
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/.idea/tabpfn-client.iml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/.idea/vcs.xml
--rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/.idea/workspace.xml
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/__init__.py
--rw-r--r--   0        0        0    12180 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/client.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/constants.py
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/prompt_agent.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/remote_tabpfn_classifier.py
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/server_config.yaml
--rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/service_wrapper.py
--rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/tabpfn_classifier.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/tabpfn_common_utils/.git
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/tabpfn_common_utils/.gitignore
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/tabpfn_common_utils/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/tabpfn_common_utils/__init__.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/tabpfn_common_utils/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/tabpfn_common_utils/tests/__init__.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/tabpfn_common_utils/tests/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/tests/__init__.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/tests/mock_tabpfn_server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/tests/integration/__init__.py
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/tests/integration/test_tabpfn_classifier.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/tests/unit/__init__.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/tests/unit/test_client.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/tests/unit/test_remote_tabpfn_classifier.py
--rw-r--r--   0        0        0    10517 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/tests/unit/test_service_wrapper.py
--rw-r--r--   0        0        0     5709 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/tabpfn_client/tests/unit/test_tabpfn_classifier.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/.gitignore
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 tabpfn_client-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/.gitmodules
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/README.md
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/quick_test.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/requirements.txt
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/.github/workflows/pull_request.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/.idea/.gitignore
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/.idea/misc.xml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/.idea/modules.xml
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/.idea/tabpfn-client.iml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/.idea/vcs.xml
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/.idea/workspace.xml
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/__init__.py
+-rw-r--r--   0        0        0    12180 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/client.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/constants.py
+-rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/prompt_agent.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/remote_tabpfn_classifier.py
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/server_config.yaml
+-rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/service_wrapper.py
+-rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tabpfn_classifier.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tabpfn_common_utils/.git
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tabpfn_common_utils/.gitignore
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tabpfn_common_utils/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tabpfn_common_utils/__init__.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tabpfn_common_utils/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tabpfn_common_utils/tests/__init__.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tabpfn_common_utils/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tests/__init__.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tests/mock_tabpfn_server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tests/integration/__init__.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tests/integration/test_tabpfn_classifier.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tests/unit/__init__.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tests/unit/test_client.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tests/unit/test_remote_tabpfn_classifier.py
+-rw-r--r--   0        0        0    10517 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tests/unit/test_service_wrapper.py
+-rw-r--r--   0        0        0     5709 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tests/unit/test_tabpfn_classifier.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/.gitignore
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/PKG-INFO
```

### Comparing `tabpfn_client-0.0.7/README.md` & `tabpfn_client-0.0.8/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,37 @@
-# Free client to use an updated TabPFN
+# PLEASE READ: Alpha Client for the Updated TabPFN
+
+Password for registration / validation link: tabpfn-2023
 
 This is an alpha family and friends service, so please do not expect this to never be down or run into errors.
 We did test it though and can say that it seems to work fine in the settings that we tried.
 
+PLEASE DO NOT SHARE THIS REPOSITORY at this point outside of the NeurIPS Tabular Representation workshop.
+
+### What model is behind the API?
+
+**For now, this version is the light version to save compute on our side, not the TabPFN (Fast) or TabPFN (Best-Q) which we presented at the Neurips Workshop. We will change this once we see our server is working stably. It is a new TabPFN which we allow to handle up to 10K instances with up to 500 features.
+This TabPFN is not ensembled, we will put out improved and ensembled models soon.**
+
 **We release this to get feedback, if you encounter bugs or curiosities please create an issue or email me (samuelgabrielmuller (at) gmail com).**
 
 
-# How to
+# How To
 
 ### Tutorial
 
-We created a [![colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/liam-sbhoo/a78a0fab40d8940c218cf2dc3b4f2bf8/tabpfndemo.ipynb)
+[![colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ns_KdtyHgl29AOVwTw9c-DZrPj7fx_DW?usp=sharing)
+
+We created a [colab](https://colab.research.google.com/drive/1ns_KdtyHgl29AOVwTw9c-DZrPj7fx_DW?usp=sharing)
 tutorial to get started quickly.
 
 ### Installation
 
 ```bash
-pip install --extra-index-url https://test.pypi.org/simple/ tabpfn-client
+pip install tabpfn-client
 ```
 
 ### Usage
 
 Import and login
 ```python
 from tabpfn_client import init, TabPFNClassifier
```

### Comparing `tabpfn_client-0.0.7/quick_test.py` & `tabpfn_client-0.0.8/quick_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         print(tabpfn.predict_proba(X_test))
 
     else:
         tabpfn_classifier.init()
         tabpfn = TabPFNClassifier()
         # print("checking estimator", check_estimator(tabpfn))
         print(X_train.shape[0]*100)
-        tabpfn.fit(np.repeat(X_train, 100, axis=0), np.repeat(y_train, 100, axis=0))
+        #tabpfn.fit(np.repeat(X_train, 100, axis=0), np.repeat(y_train, 100, axis=0))
+        tabpfn.fit(X_train, y_train)
         print("predicting")
         print(tabpfn.predict(X_test))
         print("predicting_proba")
         print(tabpfn.predict_proba(X_test))
 
         print(UserDataClient().get_data_summary())
```

### Comparing `tabpfn_client-0.0.7/.github/workflows/pull_request.yml` & `tabpfn_client-0.0.8/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.7/.idea/tabpfn-client.iml` & `tabpfn_client-0.0.8/.idea/tabpfn-client.iml`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.7/.idea/workspace.xml` & `tabpfn_client-0.0.8/.idea/workspace.xml`

 * *Files 20% similar despite different names*

#### Comparing `tabpfn_client-0.0.7/.idea/workspace.xml` & `tabpfn_client-0.0.8/.idea/workspace.xml`

```diff
@@ -1,16 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="ed2419b1-6341-4630-84c5-9846f2c56c69" name="Changes" comment="">
+    <list default="true" id="ed2419b1-6341-4630-84c5-9846f2c56c69" name="Changes" comment="no validation link">
+      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/quick_test.py" beforeDir="false" afterPath="$PROJECT_DIR$/quick_test.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tabpfn_client/client.py" beforeDir="false" afterPath="$PROJECT_DIR$/tabpfn_client/client.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
@@ -68,16 +68,47 @@
     <task active="true" id="Default" summary="Default task">
       <changelist id="ed2419b1-6341-4630-84c5-9846f2c56c69" name="Changes" comment=""/>
       <created>1702653043433</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1702653043433</updated>
     </task>
+    <task id="LOCAL-00001" summary="better error messages">
+      <created>1702658579193</created>
+      <option name="number" value="00001"/>
+      <option name="presentableId" value="LOCAL-00001"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1702658579193</updated>
+    </task>
+    <task id="LOCAL-00002" summary="no validation link">
+      <created>1702663259850</created>
+      <option name="number" value="00002"/>
+      <option name="presentableId" value="LOCAL-00002"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1702663259850</updated>
+    </task>
+    <option name="localTasksCounter" value="3"/>
     <servers/>
   </component>
+  <component name="Vcs.Log.Tabs.Properties">
+    <option name="TAB_STATES">
+      <map>
+        <entry key="MAIN">
+          <value>
+            <State/>
+          </value>
+        </entry>
+      </map>
+    </option>
+  </component>
+  <component name="VcsManagerConfiguration">
+    <MESSAGE value="better error messages"/>
+    <MESSAGE value="no validation link"/>
+    <option name="LAST_COMMIT_MESSAGE" value="no validation link"/>
+  </component>
   <component name="XDebuggerManager">
     <watches-manager>
       <configuration name="PythonConfigurationType">
         <watch expression="response.content"/>
       </configuration>
     </watches-manager>
   </component>
```

### Comparing `tabpfn_client-0.0.7/.idea/inspectionProfiles/Project_Default.xml` & `tabpfn_client-0.0.8/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.7/tabpfn_client/client.py` & `tabpfn_client-0.0.8/tabpfn_client/client.py`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.7/tabpfn_client/prompt_agent.py` & `tabpfn_client-0.0.8/tabpfn_client/prompt_agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,16 @@
             "",
             "Please enter your choice: ",
         ])
 
         choice = input(cls.indent(prompt))
 
         if choice == "1":
+            #validation_link = input(cls.indent("Please enter your secret code: "))
+            validation_link = "tabpfn-2023"
             # create account
             email = input(cls.indent("Please enter your email: "))
 
             password_req = user_auth_handler.get_password_policy()
             password_req_prompt = "\n".join([
                 "",
                 "Password requirements (minimum):",
@@ -45,16 +47,14 @@
                 "",
                 "Please enter your password: ",
             ])
 
             password = getpass.getpass(cls.indent(password_req_prompt))
             password_confirm = getpass.getpass(cls.indent("Please confirm your password: "))
 
-            validation_link = input(cls.indent("Please enter your secret code: "))
-            
             user_auth_handler.set_token_by_registration(email, password, password_confirm, validation_link)
 
             print(cls.indent("Account created successfully!") + "\n")
 
         elif choice == "2":
             # login to account
             email = input(cls.indent("Please enter your email: "))
@@ -66,18 +66,16 @@
 
         else:
             raise RuntimeError("Invalid choice")
 
     @classmethod
     def prompt_terms_and_cond(cls) -> bool:
         t_and_c = "\n".join([
-            "",
-            "Please refer to our terms and conditions at: https://www.priorlabs.ai/terms-eu-en"
+            "Please refer to our terms and conditions at: https://www.priorlabs.ai/terms-eu-en "
             "By using TabPFN, you agree to the following terms and conditions:",
-            "",
             "Do you agree to the above terms and conditions? (y/n): ",
         ])
 
         choice = input(cls.indent(t_and_c))
 
         # retry for 3 attempts until valid choice is made
         is_valid_choice = False
```

### Comparing `tabpfn_client-0.0.7/tabpfn_client/remote_tabpfn_classifier.py` & `tabpfn_client-0.0.8/tabpfn_client/remote_tabpfn_classifier.py`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.7/tabpfn_client/server_config.yaml` & `tabpfn_client-0.0.8/tabpfn_client/server_config.yaml`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.7/tabpfn_client/service_wrapper.py` & `tabpfn_client-0.0.8/tabpfn_client/service_wrapper.py`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.7/tabpfn_client/tabpfn_classifier.py` & `tabpfn_client-0.0.8/tabpfn_client/tabpfn_classifier.py`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.7/tabpfn_client/tabpfn_common_utils/.gitignore` & `tabpfn_client-0.0.8/tabpfn_client/tabpfn_common_utils/.gitignore`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.7/tabpfn_client/tabpfn_common_utils/utils.py` & `tabpfn_client-0.0.8/tabpfn_client/tabpfn_common_utils/utils.py`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.7/tabpfn_client/tabpfn_common_utils/tests/test_utils.py` & `tabpfn_client-0.0.8/tabpfn_client/tabpfn_common_utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.7/tabpfn_client/tests/mock_tabpfn_server.py` & `tabpfn_client-0.0.8/tabpfn_client/tests/mock_tabpfn_server.py`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.7/tabpfn_client/tests/integration/test_tabpfn_classifier.py` & `tabpfn_client-0.0.8/tabpfn_client/tests/integration/test_tabpfn_classifier.py`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.7/tabpfn_client/tests/unit/test_client.py` & `tabpfn_client-0.0.8/tabpfn_client/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.7/tabpfn_client/tests/unit/test_remote_tabpfn_classifier.py` & `tabpfn_client-0.0.8/tabpfn_client/tests/unit/test_remote_tabpfn_classifier.py`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.7/tabpfn_client/tests/unit/test_service_wrapper.py` & `tabpfn_client-0.0.8/tabpfn_client/tests/unit/test_service_wrapper.py`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.7/tabpfn_client/tests/unit/test_tabpfn_classifier.py` & `tabpfn_client-0.0.8/tabpfn_client/tests/unit/test_tabpfn_classifier.py`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.7/.gitignore` & `tabpfn_client-0.0.8/.gitignore`

 * *Files identical despite different names*

