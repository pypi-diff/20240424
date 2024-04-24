# Comparing `tmp/healthcare_puller-0.2.1.tar.gz` & `tmp/healthcare_puller-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healthcare_puller-0.2.1.tar", max compression
+gzip compressed data, was "healthcare_puller-0.2.2.tar", max compression
```

## Comparing `healthcare_puller-0.2.1.tar` & `healthcare_puller-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      190 2024-04-24 18:51:08.404900 healthcare_puller-0.2.1/README.md
--rw-r--r--   0        0        0       88 2024-04-24 18:43:51.444957 healthcare_puller-0.2.1/healthcare_puller/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 04:03:08.000000 healthcare_puller-0.2.1/healthcare_puller/federal_register/__init__.py
--rw-r--r--   0        0        0     2164 2024-04-24 18:47:38.824929 healthcare_puller-0.2.1/healthcare_puller/federal_register/cms_pullers.py
--rw-r--r--   0        0        0      348 2024-04-24 18:51:45.024895 healthcare_puller-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      641 1970-01-01 00:00:00.000000 healthcare_puller-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      348 2024-04-24 19:30:29.373938 healthcare_puller-0.2.2/README.md
+-rw-r--r--   0        0        0       88 2024-04-24 18:43:51.000000 healthcare_puller-0.2.2/healthcare_puller/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 04:03:08.000000 healthcare_puller-0.2.2/healthcare_puller/federal_register/__init__.py
+-rw-r--r--   0        0        0     3098 2024-04-24 19:27:17.538104 healthcare_puller-0.2.2/healthcare_puller/federal_register/cms_pullers.py
+-rw-r--r--   0        0        0      238 2024-04-24 19:05:10.000000 healthcare_puller-0.2.2/healthcare_puller/michigan_legislature/bill_and_analysis_puller.py
+-rw-r--r--   0        0        0      348 2024-04-24 19:31:06.457906 healthcare_puller-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      799 1970-01-01 00:00:00.000000 healthcare_puller-0.2.2/PKG-INFO
```

### Comparing `healthcare_puller-0.2.1/healthcare_puller/federal_register/cms_pullers.py` & `healthcare_puller-0.2.2/healthcare_puller/federal_register/cms_pullers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,65 @@
+from datetime import datetime
 import os
 
 import pandas as pd
 import requests
 from tqdm import tqdm
 
 RULE_URL = "https://www.federalregister.gov/api/v1/documents.json?fields[]=abstract&fields[]=docket_id&fields[]=document_number&fields[]=effective_on&fields[]=pdf_url&fields[]=topics&per_page=1000&conditions[agencies][]=centers-for-medicare-medicaid-services&conditions[type][]=RULE"
 PRORULE_URL = "https://www.federalregister.gov/api/v1/documents.json?fields[]=abstract&fields[]=docket_id&fields[]=document_number&fields[]=effective_on&fields[]=pdf_url&fields[]=topics&per_page=1000&conditions[agencies][]=centers-for-medicare-medicaid-services&conditions[type][]=PRORULE"
+PUBLIC_INSPECTION_URL = "https://www.federalregister.gov/api/v1/public-inspection-documents.json?fields[]=agency_names&fields[]=pdf_url&fields[]=publication_date&fields[]=title&per_page=1000&conditions[available_on]=2024-04-24&conditions[agencies][]=centers-for-medicare-medicaid-services&conditions[type][]=RULE"
 
 
 def get_rule_json(datatype='rule', doc_limit=None):
     if datatype == 'rule':
         url = RULE_URL
     elif datatype == 'prorule':
         url = PRORULE_URL
     if doc_limit:
         url = url.replace("per_page=1000", f"per_page={doc_limit}")
     rule_json = requests.get(url).json()['results']
     if doc_limit:
         rule_json = rule_json[:doc_limit]
     return rule_json
-    
+
+
+def get_public_inspection_json(doc_limit=None, date=None):
+    if not date:
+        date = datetime.today().strftime("%Y-%m-%d")
+    url = PUBLIC_INSPECTION_URL.replace("2024-04-24", date)
+    pi_json = requests.get(url).json()['results']
+    needed_data = [ item for item in pi_json if 'Centers for Medicare & Medicaid Services' in item['agency_names']]
+    if doc_limit:
+        return needed_data[:doc_limit]
+    else:
+        return needed_data
+
 
 def save_pdf(save_dir, url, check_exists):
     save_loc = f'{save_dir}/{url.split("/")[-1]}'
     response = requests.get(url)
     current_files = [ f"{save_dir}/{filename}" for filename in os.listdir(save_dir) ]
     if check_exists and save_loc in current_files:
         print(f"File {save_loc.split("/")[-1]} already exists, skipping")
     with open(save_loc, 'wb') as f:
         f.write(response.content)
         print(f"Saved to {save_loc}")
 
 
-def save_cms_docs(save_dir, rule_type, doc_limit=None, check_exists=True):
-    if rule_type not in ('rule', 'prorule'):
+def save_cms_docs(save_dir, rule_type, doc_limit=None, check_exists=True, date=None):
+    if rule_type not in ('rule', 'prorule', 'public_inspection'):
         print("Rule type must be rule or prorule")
         return
-    rule_json = get_rule_json(rule_type, doc_limit)
+    if rule_type == 'public_inspection':
+        rule_json = get_public_inspection_json(doc_limit=doc_limit, date=date)
+    else:
+        rule_json = get_rule_json(rule_type, doc_limit)
     for rule in rule_json:
         save_pdf(save_dir, rule['pdf_url'], check_exists)
-    print("All done!")
 
 
 def get_cms_rule_lookup(rule_type, doc_limit=None, save_csv=False, save_loc=None):
     rule_json = get_rule_json(rule_type, doc_limit)
     df = pd.DataFrame(rule_json)
     df['implied_pdf_name'] = df['pdf_url'].apply(lambda x: x.split("/")[-1])
     if save_csv:
```

### Comparing `healthcare_puller-0.2.1/PKG-INFO` & `healthcare_puller-0.2.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healthcare_puller
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: Ryan Wiley
 Author-email: wileyrya@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
@@ -14,8 +14,10 @@
 Description-Content-Type: text/markdown
 
 ## Healthcare_Puller
 
 ### This project aggregates several functions to pull down various healthcare regulations from various sources
 
 ### Current implementations
-- CMS Federal Register Rules
+* CMS Federal Register Rules
+1. Rule and Prospective Rules (last 1000 but currently around 850 historically)
+2. Public inspection documents on a given date (defaults to the current date)
```

