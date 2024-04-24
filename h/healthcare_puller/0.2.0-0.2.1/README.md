# Comparing `tmp/healthcare_puller-0.2.0.tar.gz` & `tmp/healthcare_puller-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healthcare_puller-0.2.0.tar", max compression
+gzip compressed data, was "healthcare_puller-0.2.1.tar", max compression
```

## Comparing `healthcare_puller-0.2.0.tar` & `healthcare_puller-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-24 03:21:34.568452 healthcare_puller-0.2.0/README.md
--rw-r--r--   0        0        0       55 2024-04-24 04:07:58.282060 healthcare_puller-0.2.0/healthcare_puller/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 04:03:08.802308 healthcare_puller-0.2.0/healthcare_puller/federal_register/__init__.py
--rw-r--r--   0        0        0     1811 2024-04-24 04:37:01.044572 healthcare_puller-0.2.0/healthcare_puller/federal_register/cms_pullers.py
--rw-r--r--   0        0        0      348 2024-04-24 04:37:34.080543 healthcare_puller-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 healthcare_puller-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      190 2024-04-24 18:51:08.404900 healthcare_puller-0.2.1/README.md
+-rw-r--r--   0        0        0       88 2024-04-24 18:43:51.444957 healthcare_puller-0.2.1/healthcare_puller/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 04:03:08.000000 healthcare_puller-0.2.1/healthcare_puller/federal_register/__init__.py
+-rw-r--r--   0        0        0     2164 2024-04-24 18:47:38.824929 healthcare_puller-0.2.1/healthcare_puller/federal_register/cms_pullers.py
+-rw-r--r--   0        0        0      348 2024-04-24 18:51:45.024895 healthcare_puller-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      641 1970-01-01 00:00:00.000000 healthcare_puller-0.2.1/PKG-INFO
```

### Comparing `healthcare_puller-0.2.0/healthcare_puller/federal_register/cms_pullers.py` & `healthcare_puller-0.2.1/healthcare_puller/federal_register/cms_pullers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 
+import pandas as pd
 import requests
 from tqdm import tqdm
 
 RULE_URL = "https://www.federalregister.gov/api/v1/documents.json?fields[]=abstract&fields[]=docket_id&fields[]=document_number&fields[]=effective_on&fields[]=pdf_url&fields[]=topics&per_page=1000&conditions[agencies][]=centers-for-medicare-medicaid-services&conditions[type][]=RULE"
 PRORULE_URL = "https://www.federalregister.gov/api/v1/documents.json?fields[]=abstract&fields[]=docket_id&fields[]=document_number&fields[]=effective_on&fields[]=pdf_url&fields[]=topics&per_page=1000&conditions[agencies][]=centers-for-medicare-medicaid-services&conditions[type][]=PRORULE"
 
 
@@ -37,12 +38,22 @@
         return
     rule_json = get_rule_json(rule_type, doc_limit)
     for rule in rule_json:
         save_pdf(save_dir, rule['pdf_url'], check_exists)
     print("All done!")
 
 
+def get_cms_rule_lookup(rule_type, doc_limit=None, save_csv=False, save_loc=None):
+    rule_json = get_rule_json(rule_type, doc_limit)
+    df = pd.DataFrame(rule_json)
+    df['implied_pdf_name'] = df['pdf_url'].apply(lambda x: x.split("/")[-1])
+    if save_csv:
+        df.to_csv(save_loc, index=False)
+    else:
+        return df
+
+
```

