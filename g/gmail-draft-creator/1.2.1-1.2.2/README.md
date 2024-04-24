# Comparing `tmp/gmail_draft_creator-1.2.1.tar.gz` & `tmp/gmail_draft_creator-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmail_draft_creator-1.2.1.tar", max compression
+gzip compressed data, was "gmail_draft_creator-1.2.2.tar", max compression
```

## Comparing `gmail_draft_creator-1.2.1.tar` & `gmail_draft_creator-1.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1071 2023-07-14 21:25:27.494420 gmail_draft_creator-1.2.1/LICENSE
--rw-r--r--   0        0        0     4719 2023-07-14 21:25:27.494420 gmail_draft_creator-1.2.1/gmail_draft_creator/__init__.py
--rw-r--r--   0        0        0     1186 2023-07-14 21:25:49.062650 gmail_draft_creator-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     1905 2023-07-14 21:25:27.494420 gmail_draft_creator-1.2.1/readme.md
--rw-r--r--   0        0        0     2744 1970-01-01 00:00:00.000000 gmail_draft_creator-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-24 18:00:55.034434 gmail_draft_creator-1.2.2/LICENSE
+-rw-r--r--   0        0        0     4848 2024-04-24 18:00:55.034434 gmail_draft_creator-1.2.2/gmail_draft_creator/__init__.py
+-rw-r--r--   0        0        0     1326 2024-04-24 18:01:23.778924 gmail_draft_creator-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2820 2024-04-24 18:00:55.034434 gmail_draft_creator-1.2.2/readme.md
+-rw-r--r--   0        0        0     3787 1970-01-01 00:00:00.000000 gmail_draft_creator-1.2.2/PKG-INFO
```

### Comparing `gmail_draft_creator-1.2.1/LICENSE` & `gmail_draft_creator-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gmail_draft_creator-1.2.1/gmail_draft_creator/__init__.py` & `gmail_draft_creator-1.2.2/gmail_draft_creator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,21 +55,28 @@
 def send_drafts_from_csv(csv_file_path, template_file_path, subject, dry_run):
     with open(template_file_path, "r") as template_file:
         template_string = template_file.read()
 
     with open(csv_file_path, "r") as file:
         reader = csv.DictReader(file)
         for row in reader:
-            email = row.pop("email", None) or row.pop("Email", None)
+            email = None
+
+            for key in row.keys():
+                if key.lower() == 'email':
+                    email = row.pop(key)
+                    break
+
+            if email:
+                email = email.strip()
 
             if email is None:
                 print("No email found for row, skipping")
                 continue
 
-            email = email.strip()
             template_params = {k.lower().strip(): v.strip() for k, v in row.items()}
 
             if email is not None:
                 create_draft(email, template_string, template_params, subject, dry_run)
 
 
 # TODO this should really be much smarter
```

### Comparing `gmail_draft_creator-1.2.1/pyproject.toml` & `gmail_draft_creator-1.2.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [tool.poetry]
 name = "gmail_draft_creator"
-version = "1.2.1"
-description = "Create draft messages in Gmail"
+version = "1.2.2"
+description = "Simple tool to take a CSV and a template and create drafts in your Gmail. Can be used as a command line tool, or as a library."
 authors = ["Michael Bianco <mike@mikebian.co>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/iloveitaly/gmail-draft-creator"
+keywords = ["gmail", "email", "gmail-api"]
 
 [project.urls]
 'Changelog' = 'https://github.com/iloveitaly/gmail-draft-creator/blob/master/CHANGELOG.md'
 
 [tool.poetry.dependencies]
 python = "^3.9"
-google-api-python-client = "^2.21.0"
+google-api-python-client = "^2.97.0"
 python-decouple = "^3.5"
 google-auth-httplib2 = "^0.1.0"
 google-auth-oauthlib = "^0.4.6"
-click = "^8.1.3"
-markdown = "^3.4.3"
+click = "^8.1.7"
+markdown = "^3.5.1"
 
 [tool.poetry.scripts]
 gmail-draft-creator = "gmail_draft_creator:main"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.3.0"
+black = "^23.10.1"
 isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
```

### Comparing `gmail_draft_creator-1.2.1/readme.md` & `gmail_draft_creator-1.2.2/readme.md`

 * *Files 15% similar despite different names*

```diff
@@ -16,48 +16,76 @@
 
 Options:
   --csv PATH       Path to the CSV file.  [required]
   --template PATH  Path to the template file.  [required]
   --subject TEXT   Subject for the email drafts.
   --dry-run        Run script without creating drafts.
   --help           Show this message and exit.
-
 ```
 
 You can also import the `create_draft` function and use it in your own scripts.
 
+### CSV Files
+
+Must contain an `email` column (case insensitive).
+
 ### Template Files
 
 You can include subject line and variables in the template file:
 
 ```text
 Subject: Hello $NAME
 
 Hi, here's another ${REASON} why I'm emailing you.
 ```
 
+### CSV Files
+
+A CSV file that would work with this template might be something like this:
+
+```
+Email,Name,Reason,OtherColumn,...
+joe@test.com,Joe,reminder,...
+jeff@email.com,Jeff,sales pitch,...
+```
+
 ## Setup
 
+You need to create a "OAuth 2.0 Client IDs" which has to be done with a Google Workspace (gsuite). This will not work on a personal gmail account (unless you create a app on a workspace and add your personal account as a test account).
+
 ### Generating a Gmail API Token
 
 1. Navigate to the Google Cloud Console. https://console.developers.google.com/
 2. Create a new project or select an existing one.
 3. Go to "APIs & Services" -> "Library" and enable the Gmail API.
 4. Navigate to "APIs & Services" -> "Credentials".
 5. Click "Create Credentials" -> "OAuth client ID".
 6. Select "Desktop app" as the application type, then click "Create".
-7. Download the JSON file, rename it to `credentials.json`, and place it in the root of your project.
+7. Download the JSON file, rename it to `credentials.json`, and place it in the root of this project.
 8. Run the script and oauth into your account
 
+If you want to edit scopes on an existing application, you can:
+
+1. OAuth Consent Screen
+2. Edit
+3. Continue to step 2
+4. Add or remove scopes
+5. Add scopes and save
+
 #### Credential Scopes Needed
 
-* https://www.googleapis.com/auth/gmail.compose
-* https://www.googleapis.com/auth/gmail.readonly
-* https://www.googleapis.com/auth/calendar.readonly
-* https://www.googleapis.com/auth/calendar.event
+Two main scopes are required for this:
+
+* `https://www.googleapis.com/auth/gmail.compose`
+* `https://www.googleapis.com/auth/gmail.readonly`
+
+Some other scopes I'd add so you can reuse the credentials in other projects, [like gmailctl](https://github.com/mbrt/gmailctl) or calendar scripts:
 
-Some of these are in place for possible future improvements.
+* `https://www.googleapis.com/auth/calendar.readonly`
+* `https://www.googleapis.com/auth/calendar.event`
+* `https://www.googleapis.com/auth/gmail.labels`
+* `https://www.googleapis.com/auth/gmail.settings.basic`
 
 ## TODO
 
 - [ ] add credentials as a command line argument
-- [ ] add serialized token as a CLI argument
+- [ ] add serialized token as a CLI argument
```

### Comparing `gmail_draft_creator-1.2.1/PKG-INFO` & `gmail_draft_creator-1.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: gmail-draft-creator
-Version: 1.2.1
-Summary: Create draft messages in Gmail
+Version: 1.2.2
+Summary: Simple tool to take a CSV and a template and create drafts in your Gmail. Can be used as a command line tool, or as a library.
 Home-page: https://github.com/iloveitaly/gmail-draft-creator
 License: MIT
+Keywords: gmail,email,gmail-api
 Author: Michael Bianco
 Author-email: mike@mikebian.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: google-api-python-client (>=2.21.0,<3.0.0)
+Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: google-api-python-client (>=2.97.0,<3.0.0)
 Requires-Dist: google-auth-httplib2 (>=0.1.0,<0.2.0)
 Requires-Dist: google-auth-oauthlib (>=0.4.6,<0.5.0)
-Requires-Dist: markdown (>=3.4.3,<4.0.0)
+Requires-Dist: markdown (>=3.5.1,<4.0.0)
 Requires-Dist: python-decouple (>=3.5,<4.0)
 Description-Content-Type: text/markdown
 
 # Gmail Drafter: Create Mail Merge Drafts
 
 Simple tool to take a CSV and a template and create drafts in your Gmail. Useful for sending emails to large-ish numbers
 of people where you want to slightly customize the emails for each user. You can quickly run through drafts, customize it, and send.
@@ -38,48 +39,77 @@
 
 Options:
   --csv PATH       Path to the CSV file.  [required]
   --template PATH  Path to the template file.  [required]
   --subject TEXT   Subject for the email drafts.
   --dry-run        Run script without creating drafts.
   --help           Show this message and exit.
-
 ```
 
 You can also import the `create_draft` function and use it in your own scripts.
 
+### CSV Files
+
+Must contain an `email` column (case insensitive).
+
 ### Template Files
 
 You can include subject line and variables in the template file:
 
 ```text
 Subject: Hello $NAME
 
 Hi, here's another ${REASON} why I'm emailing you.
 ```
 
+### CSV Files
+
+A CSV file that would work with this template might be something like this:
+
+```
+Email,Name,Reason,OtherColumn,...
+joe@test.com,Joe,reminder,...
+jeff@email.com,Jeff,sales pitch,...
+```
+
 ## Setup
 
+You need to create a "OAuth 2.0 Client IDs" which has to be done with a Google Workspace (gsuite). This will not work on a personal gmail account (unless you create a app on a workspace and add your personal account as a test account).
+
 ### Generating a Gmail API Token
 
 1. Navigate to the Google Cloud Console. https://console.developers.google.com/
 2. Create a new project or select an existing one.
 3. Go to "APIs & Services" -> "Library" and enable the Gmail API.
 4. Navigate to "APIs & Services" -> "Credentials".
 5. Click "Create Credentials" -> "OAuth client ID".
 6. Select "Desktop app" as the application type, then click "Create".
-7. Download the JSON file, rename it to `credentials.json`, and place it in the root of your project.
+7. Download the JSON file, rename it to `credentials.json`, and place it in the root of this project.
 8. Run the script and oauth into your account
 
+If you want to edit scopes on an existing application, you can:
+
+1. OAuth Consent Screen
+2. Edit
+3. Continue to step 2
+4. Add or remove scopes
+5. Add scopes and save
+
 #### Credential Scopes Needed
 
-* https://www.googleapis.com/auth/gmail.compose
-* https://www.googleapis.com/auth/gmail.readonly
-* https://www.googleapis.com/auth/calendar.readonly
-* https://www.googleapis.com/auth/calendar.event
+Two main scopes are required for this:
 
-Some of these are in place for possible future improvements.
+* `https://www.googleapis.com/auth/gmail.compose`
+* `https://www.googleapis.com/auth/gmail.readonly`
+
+Some other scopes I'd add so you can reuse the credentials in other projects, [like gmailctl](https://github.com/mbrt/gmailctl) or calendar scripts:
+
+* `https://www.googleapis.com/auth/calendar.readonly`
+* `https://www.googleapis.com/auth/calendar.event`
+* `https://www.googleapis.com/auth/gmail.labels`
+* `https://www.googleapis.com/auth/gmail.settings.basic`
 
 ## TODO
 
 - [ ] add credentials as a command line argument
 - [ ] add serialized token as a CLI argument
+
```

