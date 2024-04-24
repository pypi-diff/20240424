# Comparing `tmp/tabpfn_client-0.0.8.tar.gz` & `tmp/tabpfn_client-0.0.9.tar.gz`

## Comparing `tabpfn_client-0.0.8.tar` & `tabpfn_client-0.0.9.tar`

### file list

```diff
@@ -1,40 +1,34 @@
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/.gitmodules
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/README.md
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/quick_test.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/requirements.txt
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/.github/workflows/pull_request.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/.idea/.gitignore
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/.idea/misc.xml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/.idea/modules.xml
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/.idea/tabpfn-client.iml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/.idea/vcs.xml
--rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/.idea/workspace.xml
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/__init__.py
--rw-r--r--   0        0        0    12180 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/client.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/constants.py
--rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/prompt_agent.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/remote_tabpfn_classifier.py
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/server_config.yaml
--rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/service_wrapper.py
--rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tabpfn_classifier.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tabpfn_common_utils/.git
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tabpfn_common_utils/.gitignore
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tabpfn_common_utils/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tabpfn_common_utils/__init__.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tabpfn_common_utils/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tabpfn_common_utils/tests/__init__.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tabpfn_common_utils/tests/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tests/__init__.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tests/mock_tabpfn_server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tests/integration/__init__.py
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tests/integration/test_tabpfn_classifier.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tests/unit/__init__.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tests/unit/test_client.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tests/unit/test_remote_tabpfn_classifier.py
--rw-r--r--   0        0        0    10517 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tests/unit/test_service_wrapper.py
--rw-r--r--   0        0        0     5709 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/tabpfn_client/tests/unit/test_tabpfn_classifier.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/.gitignore
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 tabpfn_client-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/.gitmodules
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/README.md
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/quick_test.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/.github/pull_request_template.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/.github/workflows/pull_request.yml
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/__init__.py
+-rw-r--r--   0        0        0    14996 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/client.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/constants.py
+-rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/prompt_agent.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/remote_tabpfn_classifier.py
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/server_config.yaml
+-rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/service_wrapper.py
+-rw-r--r--   0        0        0     6868 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/tabpfn_classifier.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/tabpfn_common_utils/.git
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/tabpfn_common_utils/.gitignore
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/tabpfn_common_utils/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/tabpfn_common_utils/__init__.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/tabpfn_common_utils/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/tabpfn_common_utils/tests/__init__.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/tabpfn_common_utils/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/tests/__init__.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/tests/mock_tabpfn_server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/tests/integration/__init__.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/tests/integration/test_tabpfn_classifier.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/tests/unit/__init__.py
+-rw-r--r--   0        0        0     7178 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/tests/unit/test_client.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/tests/unit/test_prompt_agent.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/tests/unit/test_remote_tabpfn_classifier.py
+-rw-r--r--   0        0        0    10536 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/tests/unit/test_service_wrapper.py
+-rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/tabpfn_client/tests/unit/test_tabpfn_classifier.py
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/.gitignore
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 tabpfn_client-0.0.9/PKG-INFO
```

### Comparing `tabpfn_client-0.0.8/README.md` & `tabpfn_client-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 Password for registration / validation link: tabpfn-2023
 
 This is an alpha family and friends service, so please do not expect this to never be down or run into errors.
 We did test it though and can say that it seems to work fine in the settings that we tried.
 
 PLEASE DO NOT SHARE THIS REPOSITORY at this point outside of the NeurIPS Tabular Representation workshop.
 
-### What model is behind the API?
+What model is behind the API? For now, this version is the light version to save compute on our side, not the TabPFN (Fast) or TabPFN (Best-Q) which we presented at the Neurips Workshop. We will change this once we see our server is working stably. It is a new TabPFN which we allow to handle up to 10K instances with up to 500 features.
+This TabPFN is not ensembled, we will put out improved and ensembled models soon.
 
-**For now, this version is the light version to save compute on our side, not the TabPFN (Fast) or TabPFN (Best-Q) which we presented at the Neurips Workshop. We will change this once we see our server is working stably. It is a new TabPFN which we allow to handle up to 10K instances with up to 500 features.
-This TabPFN is not ensembled, we will put out improved and ensembled models soon.**
-
-**We release this to get feedback, if you encounter bugs or curiosities please create an issue or email me (samuelgabrielmuller (at) gmail com).**
+### We would really appreciate your feedback! If you encounter bugs or suggestions for improvement please create an issue or email me (samuelgabrielmuller (at) gmail com).
 
 
 # How To
 
 ### Tutorial
 
 [![colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ns_KdtyHgl29AOVwTw9c-DZrPj7fx_DW?usp=sharing)
```

### Comparing `tabpfn_client-0.0.8/quick_test.py` & `tabpfn_client-0.0.9/quick_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,28 +18,26 @@
     # use_server = False
 
     X, y = load_breast_cancer(return_X_y=True)
     X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.33, random_state=42)
 
     if not use_server:
         tabpfn_classifier.init(use_server=False)
-        tabpfn = TabPFNClassifier(device="cpu", N_ensemble_configurations=4)
+        tabpfn = TabPFNClassifier(device="cpu", N_ensemble_configurations=4, model="tabpfn_1_local")
         # check_estimator(tabpfn)
         tabpfn.fit(np.repeat(X_train,100,axis=0), np.repeat(y_train,100,axis=0))
         print("predicting")
         print(tabpfn.predict(X_test))
         print("predicting_proba")
         print(tabpfn.predict_proba(X_test))
 
     else:
         tabpfn_classifier.init()
-        tabpfn = TabPFNClassifier()
+        tabpfn = TabPFNClassifier(model="latest_tabpfn_hosted")
         # print("checking estimator", check_estimator(tabpfn))
-        print(X_train.shape[0]*100)
-        #tabpfn.fit(np.repeat(X_train, 100, axis=0), np.repeat(y_train, 100, axis=0))
-        tabpfn.fit(X_train, y_train)
+        tabpfn.fit(X_train[:99], y_train[:99])
         print("predicting")
         print(tabpfn.predict(X_test))
         print("predicting_proba")
         print(tabpfn.predict_proba(X_test))
 
         print(UserDataClient().get_data_summary())
```

### Comparing `tabpfn_client-0.0.8/.github/workflows/pull_request.yml` & `tabpfn_client-0.0.9/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.8/tabpfn_client/remote_tabpfn_classifier.py` & `tabpfn_client-0.0.9/tabpfn_client/remote_tabpfn_classifier.py`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.8/tabpfn_client/server_config.yaml` & `tabpfn_client-0.0.9/tabpfn_client/server_config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -14,24 +14,39 @@
     description: "Root endpoint"
 
   password_policy:
     path: "/auth/password_policy/"
     methods: [ "GET" ]
     description: "Password policy"
 
+  validate_email:
+    path: "/auth/validate_email/"
+    methods: [ "POST" ]
+    description: "Validate email"
+
   register:
     path: "/auth/register/"
     methods: [ "POST" ]
     description: "User registration"
 
   login:
     path: "/auth/login/"
     methods: [ "POST" ]
     description: "User login"
 
+  retrieve_greeting_messages:
+    path: "/retrieve_greeting_messages/"
+    methods: [ "GET" ]
+    description: "Retrieve new greeting messages"
+
+  add_user_information:
+    path: "/add_user_information/"
+    methods: [ "POST" ]
+    description: "Add additional user information to database"
+
   protected_root:
     path: "/protected/"
     methods: [ "GET" ]
     description: "Protected root"
 
   upload_test_set:
     path: "/upload/test_set/"
```

### Comparing `tabpfn_client-0.0.8/tabpfn_client/service_wrapper.py` & `tabpfn_client-0.0.9/tabpfn_client/service_wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,38 +26,40 @@
         return self.service_client.try_connection()
 
     def set_token(self, access_token: str):
         self.service_client.authorize(access_token)
         self.CACHED_TOKEN_FILE.parent.mkdir(parents=True, exist_ok=True)
         self.CACHED_TOKEN_FILE.write_text(access_token)
 
+    def validate_email(self, email: str) -> tuple[bool, str]:
+        is_valid, message = self.service_client.validate_email(email)
+        return is_valid, message
+
     def set_token_by_registration(
             self,
             email: str,
             password: str,
             password_confirm: str,
             validation_link: str
-    ) -> None:
-        if password != password_confirm:
-            raise ValueError("Password and password_confirm must be the same.")
+    ) -> tuple[bool, str]:
 
         is_created, message = self.service_client.register(email, password, password_confirm, validation_link)
-        if not is_created:
-            raise RuntimeError(f"Failed to register user: {message}")
-
-        # login after registration
-        self.set_token_by_login(email, password)
+        if is_created:
+            # login after registration
+            self.set_token_by_login(email, password)
+        return is_created, message
 
-    def set_token_by_login(self, email: str, password: str) -> None:
-        access_token = self.service_client.login(email, password)
+    def set_token_by_login(self, email: str, password: str) -> tuple[bool, str]:
+        access_token, message = self.service_client.login(email, password)
 
         if access_token is None:
-            raise RuntimeError("Failed to login, please check your email and password.")
+            return False, message
 
         self.set_token(access_token)
+        return True, message
 
     def try_reuse_existing_token(self) -> bool:
         if self.service_client.access_token is None:
             if not self.CACHED_TOKEN_FILE.exists():
                 return False
 
             access_token = self.CACHED_TOKEN_FILE.read_text()
@@ -74,21 +76,29 @@
         self.set_token(access_token)
 
         return True
 
     def get_password_policy(self):
         return self.service_client.get_password_policy()
 
+    def add_user_information(
+            self, company: str | None, role: str | None, use_case: str | None, contact_via_email: bool
+    ):
+        self.service_client.add_user_information(company, role, use_case, contact_via_email)
+
     def reset_cache(self):
         self._reset_token()
 
     def _reset_token(self):
         self.service_client.reset_authorization()
         self.CACHED_TOKEN_FILE.unlink(missing_ok=True)
 
+    def retrieve_greeting_messages(self):
+        return self.service_client.retrieve_greeting_messages()
+
 
 class UserDataClient(ServiceClientWrapper):
     """
     Wrapper of ServiceClient to handle user data, including:
     - query, or delete user account data
     - query, download, or delete uploaded data
     """
```

### Comparing `tabpfn_client-0.0.8/tabpfn_client/tabpfn_classifier.py` & `tabpfn_client-0.0.9/tabpfn_client/tabpfn_classifier.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     user_auth_handler = None
     inference_handler = None
 
 
 g_tabpfn_config = TabPFNConfig()
 
 
-# def init(use_server=True):
-def init():
-    use_server = True
+def init(use_server=True):
+    # initialize config
+    use_server = use_server
     global g_tabpfn_config
 
     if use_server:
         PromptAgent.prompt_welcome()
 
         service_client = ServiceClient()
         user_auth_handler = UserAuthenticationClient(service_client)
@@ -48,14 +48,17 @@
         else:
             if not PromptAgent.prompt_terms_and_cond():
                 raise RuntimeError("You must agree to the terms and conditions to use TabPFN")
 
             # prompt for login / register
             PromptAgent.prompt_and_set_token(user_auth_handler)
 
+        # Print new greeting messages. If there are no new messages, nothing will be printed.
+        PromptAgent.prompt_retrieved_greeting_messages(user_auth_handler.retrieve_greeting_messages())
+
         g_tabpfn_config.use_server = True
         g_tabpfn_config.user_auth_handler = user_auth_handler
         g_tabpfn_config.inference_handler = InferenceClient(service_client)
 
     else:
         g_tabpfn_config.use_server = False
 
@@ -72,96 +75,104 @@
         g_tabpfn_config.user_auth_handler.reset_cache()
 
     # remove cache dir
     shutil.rmtree(CACHE_DIR, ignore_errors=True)
 
 
 class TabPFNClassifier(BaseEstimator, ClassifierMixin):
-    def __init__(self):
+    # def __init__(self):
         # Configuration for TabPFNClassifier is still under development.
-        pass
-
-    # def __init__(
-    #         self,
-    #         model=None,
-    #         device="cpu",
-    #         base_path=Path(__file__).parent.parent.resolve(),
-    #         model_string="",
-    #         batch_size_inference=4,
-    #         fp16_inference=False,
-    #         inference_mode=True,
-    #         c=None,
-    #         N_ensemble_configurations=10,
-    #         preprocess_transforms=("none", "power_all"),
-    #         feature_shift_decoder=False,
-    #         normalize_with_test=False,
-    #         average_logits=False,
-    #         categorical_features=tuple(),
-    #         optimize_metric=None,
-    #         seed=None,
-    #         transformer_predict_kwargs_init=None,
-    #         multiclass_decoder="permutation",
-    # ):
-    #     # config for tabpfn
-    #     self.model = model
-    #     self.device = device
-    #     self.base_path = base_path
-    #     self.model_string = model_string
-    #     self.batch_size_inference = batch_size_inference
-    #     self.fp16_inference = fp16_inference
-    #     self.inference_mode = inference_mode
-    #     self.c = c
-    #     self.N_ensemble_configurations = N_ensemble_configurations
-    #     self.preprocess_transforms = preprocess_transforms
-    #     self.feature_shift_decoder = feature_shift_decoder
-    #     self.normalize_with_test = normalize_with_test
-    #     self.average_logits = average_logits
-    #     self.categorical_features = categorical_features
-    #     self.optimize_metric = optimize_metric
-    #     self.seed = seed
-    #     self.transformer_predict_kwargs_init = transformer_predict_kwargs_init
-    #     self.multiclass_decoder = multiclass_decoder
+    #     pass
+    
+    def __init__(
+            self,
+            model="latest_tabpfn_hosted",
+            device="cpu",
+            base_path=Path(__file__).parent.parent.resolve(),
+            model_string="",
+            batch_size_inference=4,
+            fp16_inference=False,
+            inference_mode=True,
+            c=None,
+            N_ensemble_configurations=10,
+            preprocess_transforms=("none", "power_all"),
+            feature_shift_decoder=False,
+            normalize_with_test=False,
+            average_logits=False,
+            categorical_features=tuple(),
+            optimize_metric=None,
+            seed=None,
+            transformer_predict_kwargs_init=None,
+            multiclass_decoder="permutation",
+    ):
+        # config for tabpfn
+        self.model = model
+        self.device = device
+        self.base_path = base_path
+        self.model_string = model_string
+        self.batch_size_inference = batch_size_inference
+        self.fp16_inference = fp16_inference
+        self.inference_mode = inference_mode
+        self.c = c
+        self.N_ensemble_configurations = N_ensemble_configurations
+        self.preprocess_transforms = preprocess_transforms
+        self.feature_shift_decoder = feature_shift_decoder
+        self.normalize_with_test = normalize_with_test
+        self.average_logits = average_logits
+        self.categorical_features = categorical_features
+        self.optimize_metric = optimize_metric
+        self.seed = seed
+        self.transformer_predict_kwargs_init = transformer_predict_kwargs_init
+        self.multiclass_decoder = multiclass_decoder
 
     def fit(self, X, y):
         # assert init() is called
         if not g_tabpfn_config.is_initialized:
             raise RuntimeError("TabPFNClassifier.init() must be called before using TabPFNClassifier")
 
         # create classifier if not created yet
         if not hasattr(self, "classifier"):
             # arguments that are commented out are not used at the moment
             # (not supported until new TabPFN interface is released)
-            # classifier_cfg = {
-            #     # "model": self.model,
-            #     "device": self.device,
-            #     "base_path": self.base_path,
-            #     "model_string": self.model_string,
-            #     "batch_size_inference": self.batch_size_inference,
-            #     # "fp16_inference": self.fp16_inference,
-            #     # "inference_mode": self.inference_mode,
-            #     # "c": self.c,
-            #     "N_ensemble_configurations": self.N_ensemble_configurations,
-            #     # "preprocess_transforms": self.preprocess_transforms,
-            #     "feature_shift_decoder": self.feature_shift_decoder,
-            #     # "normalize_with_test": self.normalize_with_test,
-            #     # "average_logits": self.average_logits,
-            #     # "categorical_features": self.categorical_features,
-            #     # "optimize_metric": self.optimize_metric,
-            #     "seed": self.seed,
-            #     # "transformer_predict_kwargs_init": self.transformer_predict_kwargs_init,
-            #     "multiclass_decoder": self.multiclass_decoder
-            # }
-            classifier_cfg = {}
+            classifier_cfg = {
+                # "model": self.model,
+                "device": self.device,
+                "base_path": self.base_path,
+                "model_string": self.model_string,
+                "batch_size_inference": self.batch_size_inference,
+                # "fp16_inference": self.fp16_inference,
+                # "inference_mode": self.inference_mode,
+                # "c": self.c,
+                "N_ensemble_configurations": self.N_ensemble_configurations,
+                # "preprocess_transforms": self.preprocess_transforms,
+                "feature_shift_decoder": self.feature_shift_decoder,
+                # "normalize_with_test": self.normalize_with_test,
+                # "average_logits": self.average_logits,
+                # "categorical_features": self.categorical_features,
+                # "optimize_metric": self.optimize_metric,
+                "seed": self.seed,
+                # "transformer_predict_kwargs_init": self.transformer_predict_kwargs_init,
+                "multiclass_decoder": self.multiclass_decoder
+            }
+            #classifier_cfg = {}
 
             if g_tabpfn_config.use_server:
+                try:
+                    assert self.model == "latest_tabpfn_hosted", "Only 'latest_tabpfn_hosted' model is supported at the moment for tabpfn_classifier.init(use_server=True)"
+                except AssertionError as e:
+                    print(e)
                 self.classifier_ = RemoteTabPFNClassifier(
                     **classifier_cfg,
                     inference_handler=g_tabpfn_config.inference_handler
                 )
             else:
+                try:
+                    assert self.model == "tabpfn_1_local", "Only 'tabpfn_1_local' model is supported at the moment for tabpfn_classifier.init(use_server=False)"
+                except AssertionError as e:
+                    print(e)
                 self.classifier_ = LocalTabPFNClassifier(**classifier_cfg)
 
         self.classifier_.fit(X, y)
         return self
 
     def predict(self, X):
         check_is_fitted(self)
```

### Comparing `tabpfn_client-0.0.8/tabpfn_client/tabpfn_common_utils/.gitignore` & `tabpfn_client-0.0.9/tabpfn_client/tabpfn_common_utils/.gitignore`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.8/tabpfn_client/tabpfn_common_utils/utils.py` & `tabpfn_client-0.0.9/tabpfn_client/tabpfn_common_utils/utils.py`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.8/tabpfn_client/tabpfn_common_utils/tests/test_utils.py` & `tabpfn_client-0.0.9/tabpfn_client/tabpfn_common_utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.8/tabpfn_client/tests/mock_tabpfn_server.py` & `tabpfn_client-0.0.9/tabpfn_client/tests/mock_tabpfn_server.py`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.8/tabpfn_client/tests/integration/test_tabpfn_classifier.py` & `tabpfn_client-0.0.9/tabpfn_client/tests/integration/test_tabpfn_classifier.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     def tearDown(self):
         tabpfn_classifier.reset()
         ServiceClient().delete_instance()
 
     def test_use_local_tabpfn_classifier(self):
         tabpfn_classifier.init(use_server=False)
-        tabpfn = TabPFNClassifier(device="cpu")
+        tabpfn = TabPFNClassifier(device="cpu", model="tabpfn_1_local")
         tabpfn.fit(self.X_train, self.y_train)
 
         self.assertTrue(isinstance(tabpfn.classifier_, LocalTabPFNClassifier))
         pred = tabpfn.predict(self.X_test)
         self.assertEqual(pred.shape[0], self.X_test.shape[0])
 
     @with_mock_server()
@@ -34,14 +34,16 @@
         token_file = UserAuthenticationClient.CACHED_TOKEN_FILE
         token_file.parent.mkdir(parents=True, exist_ok=True)
         token_file.write_text("dummy token")
 
         # mock connection and authentication
         mock_server.router.get(mock_server.endpoints.root.path).respond(200)
         mock_server.router.get(mock_server.endpoints.protected_root.path).respond(200)
+        mock_server.router.get(mock_server.endpoints.retrieve_greeting_messages.path).respond(
+            200, json={"messages": []})
         tabpfn_classifier.init(use_server=True)
 
         tabpfn = TabPFNClassifier()
 
         # mock fitting
         mock_server.router.post(mock_server.endpoints.upload_train_set.path).respond(
             200, json={"train_set_uid": 5})
```

### Comparing `tabpfn_client-0.0.8/tabpfn_client/tests/unit/test_remote_tabpfn_classifier.py` & `tabpfn_client-0.0.9/tabpfn_client/tests/unit/test_remote_tabpfn_classifier.py`

 * *Files identical despite different names*

### Comparing `tabpfn_client-0.0.8/tabpfn_client/tests/unit/test_service_wrapper.py` & `tabpfn_client-0.0.9/tabpfn_client/tests/unit/test_service_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,30 +25,28 @@
         # mock valid login response
         dummy_token = "dummy_token"
         mock_server.router.post(mock_server.endpoints.login.path).respond(
             200,
             json={"access_token": dummy_token}
         )
 
-        # assert no exception is raised
-        UserAuthenticationClient(ServiceClient()).set_token_by_login("dummy_email", "dummy_password")
+        self.assertTrue(UserAuthenticationClient(ServiceClient()).set_token_by_login(
+            "dummy_email", "dummy_password")[0])
 
         # assert token is set
         self.assertEqual(dummy_token, ServiceClient().access_token)
 
     @with_mock_server()
     def test_set_token_by_invalid_login(self, mock_server):
         # mock invalid login response
-        mock_server.router.post(mock_server.endpoints.login.path).respond(400)
-
-        # assert exception is raised
-        self.assertRaises(
-            RuntimeError,
-            UserAuthenticationClient(ServiceClient()).set_token_by_login,
-            "dummy_email", "dummy_password"
+        mock_server.router.post(mock_server.endpoints.login.path).respond(401, json={
+            "detail": "Incorrect email or password"})
+        self.assertEqual(
+            (False, "Incorrect email or password"),
+            UserAuthenticationClient(ServiceClient()).set_token_by_login("dummy_email", "dummy_password")
         )
 
         # assert token is not set
         self.assertIsNone(ServiceClient().access_token)
 
     @with_mock_server()
     def test_try_reusing_existing_token(self, mock_server):
@@ -83,35 +81,33 @@
             json={"message": "doesn't matter"}
         )
         mock_server.router.post(mock_server.endpoints.login.path).respond(
             200,
             json={"access_token": dummy_token}
         )
 
-        # assert no exception is raised
-        UserAuthenticationClient(ServiceClient()).set_token_by_registration(
-            "dummy_email", "dummy_password", "dummy_password", "dummy_validation"
+        self.assertTrue(
+            UserAuthenticationClient(ServiceClient()).set_token_by_registration(
+                "dummy_email", "dummy_password", "dummy_password", "dummy_validation"
+            )[0]
         )
 
         # assert token is set
         self.assertEqual(dummy_token, ServiceClient().access_token)
 
     @with_mock_server()
     def test_set_token_by_invalid_registration(self, mock_server):
         # mock invalid registration response
-        mock_server.router.post(mock_server.endpoints.register.path).respond(
-            400,
-            json={"detail": "doesn't matter"}
-        )
-
-        # assert exception is raised
-        self.assertRaises(
-            RuntimeError,
-            UserAuthenticationClient(ServiceClient()).set_token_by_registration,
-            "dummy_email", "dummy_password", "dummy_password", "dummy_validation"
+        mock_server.router.post(mock_server.endpoints.register.path).respond(401, json={
+            "detail": "Password mismatch"})
+        self.assertEqual(
+            (False, "Password mismatch"),
+            UserAuthenticationClient(ServiceClient()).set_token_by_registration(
+                "dummy_email", "dummy_password", "dummy_password",
+                "dummy_validation")
         )
 
         # assert token is not set
         self.assertIsNone(ServiceClient().access_token)
 
     @with_mock_server()
     def test_reset_cache_after_token_set(self, mock_server):
```

### Comparing `tabpfn_client-0.0.8/tabpfn_client/tests/unit/test_tabpfn_classifier.py` & `tabpfn_client-0.0.9/tabpfn_client/tests/unit/test_tabpfn_classifier.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         ServiceClient().delete_instance()
 
         # remove cache dir
         shutil.rmtree(CACHE_DIR, ignore_errors=True)
 
     def test_init_local_classifier(self):
         tabpfn_classifier.init(use_server=False)
-        tabpfn = TabPFNClassifier().fit(self.X_train, self.y_train)
+        tabpfn = TabPFNClassifier(model="tabpfn_1_local").fit(self.X_train, self.y_train)
         self.assertTrue(isinstance(tabpfn.classifier_, LocalTabPFNClassifier))
 
     @with_mock_server()
     @patch("tabpfn_client.prompt_agent.PromptAgent.prompt_and_set_token")
     @patch("tabpfn_client.prompt_agent.PromptAgent.prompt_terms_and_cond",
            return_value=True)
     def test_init_remote_classifier(self, mock_server, mock_prompt_for_terms_and_cond, mock_prompt_and_set_token):
@@ -48,26 +48,30 @@
             lambda user_auth_handler: user_auth_handler.set_token(self.dummy_token)
 
         # mock server connection
         mock_server.router.get(mock_server.endpoints.root.path).respond(200)
         mock_server.router.post(mock_server.endpoints.upload_train_set.path).respond(
             200, json={"train_set_uid": 5}
         )
+        mock_server.router.get(mock_server.endpoints.retrieve_greeting_messages.path).respond(
+            200, json={"messages": []})
 
         tabpfn_classifier.init(use_server=True)
         tabpfn = TabPFNClassifier().fit(self.X_train, self.y_train)
         self.assertTrue(isinstance(tabpfn.classifier_, RemoteTabPFNClassifier))
         self.assertTrue(mock_prompt_and_set_token.called)
         self.assertTrue(mock_prompt_for_terms_and_cond.called)
 
     @with_mock_server()
     def test_reuse_saved_access_token(self, mock_server):
         # mock connection and authentication
         mock_server.router.get(mock_server.endpoints.root.path).respond(200)
         mock_server.router.get(mock_server.endpoints.protected_root.path).respond(200)
+        mock_server.router.get(mock_server.endpoints.retrieve_greeting_messages.path).respond(
+            200, json={"messages": []})
 
         # create dummy token file
         token_file = UserAuthenticationClient.CACHED_TOKEN_FILE
         token_file.parent.mkdir(parents=True, exist_ok=True)
         token_file.write_text(self.dummy_token)
 
         # init is called without error
@@ -106,14 +110,16 @@
         token_file = UserAuthenticationClient.CACHED_TOKEN_FILE
         token_file.parent.mkdir(parents=True, exist_ok=True)
         token_file.write_text(self.dummy_token)
 
         # init classifier as usual
         mock_server.router.get(mock_server.endpoints.root.path).respond(200)
         mock_server.router.get(mock_server.endpoints.protected_root.path).respond(200)
+        mock_server.router.get(mock_server.endpoints.retrieve_greeting_messages.path).respond(
+            200, json={"messages": []})
         tabpfn_classifier.init(use_server=True)
 
         # check if access token is saved
         self.assertTrue(UserAuthenticationClient.CACHED_TOKEN_FILE.exists())
 
         # reset
         tabpfn_classifier.reset()
```

### Comparing `tabpfn_client-0.0.8/.gitignore` & `tabpfn_client-0.0.9/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -153,8 +153,11 @@
 cython_debug/
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+.idea/
+
+models_diff/
+tabpfn_client/.tabpfn/
```

