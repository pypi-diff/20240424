# Comparing `tmp/pih-rvw_auto-0.15.tar.gz` & `tmp/pih-rvw_auto-0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-rvw_auto-0.15.tar", last modified: Mon Apr 15 23:59:58 2024, max compression
+gzip compressed data, was "pih-rvw_auto-0.17.tar", last modified: Wed Apr 24 04:50:44 2024, max compression
```

## Comparing `pih-rvw_auto-0.15.tar` & `pih-rvw_auto-0.17.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 23:59:58.925054 pih-rvw_auto-0.15/
--rw-rw-rw-   0        0        0      282 2024-04-15 23:59:58.909419 pih-rvw_auto-0.15/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 23:59:58.531289 pih-rvw_auto-0.15/ReviewAutomationService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-rvw_auto-0.15/ReviewAutomationService/__init__.py
--rw-rw-rw-   0        0        0      158 2024-04-15 23:57:16.000000 pih-rvw_auto-0.15/ReviewAutomationService/__main__.py
--rw-rw-rw-   0        0        0     2476 2024-04-15 23:57:45.000000 pih-rvw_auto-0.15/ReviewAutomationService/api.py
--rw-rw-rw-   0        0        0      519 2024-04-15 23:50:58.000000 pih-rvw_auto-0.15/ReviewAutomationService/const.py
--rw-rw-rw-   0        0        0     8798 2024-04-15 23:53:23.000000 pih-rvw_auto-0.15/ReviewAutomationService/service.py
-drwxrwxrwx   0        0        0        0 2024-04-15 23:59:58.860474 pih-rvw_auto-0.15/pih_rvw_auto.egg-info/
--rw-rw-rw-   0        0        0      282 2024-04-15 23:59:58.000000 pih-rvw_auto-0.15/pih_rvw_auto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-04-15 23:59:58.000000 pih-rvw_auto-0.15/pih_rvw_auto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 23:59:58.000000 pih-rvw_auto-0.15/pih_rvw_auto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-15 23:59:58.000000 pih-rvw_auto-0.15/pih_rvw_auto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-15 23:59:58.000000 pih-rvw_auto-0.15/pih_rvw_auto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-15 23:59:58.000000 pih-rvw_auto-0.15/pih_rvw_auto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 23:59:58.940674 pih-rvw_auto-0.15/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 04:50:44.301414 pih-rvw_auto-0.17/
+-rw-rw-rw-   0        0        0      282 2024-04-24 04:50:44.270167 pih-rvw_auto-0.17/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 04:50:43.879561 pih-rvw_auto-0.17/ReviewAutomationService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-rvw_auto-0.17/ReviewAutomationService/__init__.py
+-rw-rw-rw-   0        0        0      158 2024-04-15 23:57:16.000000 pih-rvw_auto-0.17/ReviewAutomationService/__main__.py
+-rw-rw-rw-   0        0        0     2476 2024-04-15 23:57:45.000000 pih-rvw_auto-0.17/ReviewAutomationService/api.py
+-rw-rw-rw-   0        0        0      519 2024-04-24 04:48:56.000000 pih-rvw_auto-0.17/ReviewAutomationService/const.py
+-rw-rw-rw-   0        0        0     8547 2024-04-24 04:33:37.000000 pih-rvw_auto-0.17/ReviewAutomationService/service.py
+drwxrwxrwx   0        0        0        0 2024-04-24 04:50:44.238922 pih-rvw_auto-0.17/pih_rvw_auto.egg-info/
+-rw-rw-rw-   0        0        0      282 2024-04-24 04:50:43.000000 pih-rvw_auto-0.17/pih_rvw_auto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-04-24 04:50:43.000000 pih-rvw_auto-0.17/pih_rvw_auto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 04:50:43.000000 pih-rvw_auto-0.17/pih_rvw_auto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-24 04:50:43.000000 pih-rvw_auto-0.17/pih_rvw_auto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-24 04:50:43.000000 pih-rvw_auto-0.17/pih_rvw_auto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-24 04:50:43.000000 pih-rvw_auto-0.17/pih_rvw_auto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 04:50:44.301414 pih-rvw_auto-0.17/setup.cfg
```

### Comparing `pih-rvw_auto-0.15/ReviewAutomationService/api.py` & `pih-rvw_auto-0.17/ReviewAutomationService/api.py`

 * *Files identical despite different names*

### Comparing `pih-rvw_auto-0.15/ReviewAutomationService/const.py` & `pih-rvw_auto-0.17/ReviewAutomationService/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pih.consts.hosts import Hosts
 from pih.collections.service import ServiceDescription
 
 NAME: str = "ReviewAutomation"
 
 HOST = Hosts.BACKUP_WORKER
 
-VERSION: str = "0.15"
+VERSION: str = "0.17"
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Review automation service",
     host=HOST.NAME,
     use_standalone=True,
     version=VERSION,
```

### Comparing `pih-rvw_auto-0.15/ReviewAutomationService/service.py` & `pih-rvw_auto-0.17/ReviewAutomationService/service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import ipih
 
 from pih import A, PIHThread
 from ReviewAutomationService.const import SD
 
+import re
+
 SC = A.CT_SC
 
 ISOLATED: bool = False
 
 
 def start(as_standalone: bool = False) -> None:
     from datetime import datetime
@@ -54,41 +56,38 @@
                                     nn(person)
                                     and ne(notification_confirmation)
                                     and nnt(notification_confirmation).status == 2
                                 ):
                                     yes_answer_variants: list[str] = A.S.get(
                                         A.CT_S.POLIBASE_PERSON_YES_ANSWER_VARIANTS
                                     )
-                                    answer_yes: bool = False
-                                    answer_no: bool = False
-                                    for variant in yes_answer_variants:
-                                        answer_yes = message_text.find(variant) != -1
-                                        if answer_yes:
-                                            break
-                                    if not answer_yes:
-                                        no_answer_variants: list[str] = A.S.get(
-                                            A.CT_S.POLIBASE_PERSON_NO_ANSWER_VARIANTS
-                                        )
-                                        for variant in no_answer_variants:
-                                            answer_no = message_text.find(variant) != -1
-                                            if answer_no:
-                                                break
-                                    if answer_no or answer_yes:
+
+                                    no_answer_variants: list[str] = A.S.get(
+                                        A.CT_S.POLIBASE_PERSON_NO_ANSWER_VARIANTS
+                                    )
+
+                                    answer_yes: bool = A.D.has_one_of(
+                                        message_text, yes_answer_variants
+                                    )
+                                    answer_no: bool = A.D.has_one_of(
+                                        message_text, no_answer_variants
+                                    )
+                                    if answer_yes or answer_no:
                                         if A.A_P_N_C.update(
                                             telephone_number, sender, int(answer_yes)
                                         ):
                                             review_event: EventDS | None = one(
                                                 A.R_E.get_last(
                                                     A.CT_E.POLIBASE_PERSON_REVIEW_NOTIFICATION_WAS_REGISTERED,
                                                     (nnt(person).pin,),
                                                 )
                                             )
                                             is_inpatient: bool = (
                                                 nnt(nnt(review_event).parameters)[
-                                                    "inpatient"
+                                                    A.CT_PI.INPATIENT.name
                                                 ]
                                                 if nn(review_event)
                                                 and nn(nnt(review_event).parameters)
                                                 else False
                                             )
                                             if answer_yes:
                                                 A.ME_WH_W_Q.add_message(
@@ -134,14 +133,16 @@
                                                 A.CT_E.POLIBASE_PERSON_REVIEW_NOTIFICATION_WAS_ANSWERED,
                                                 (
                                                     nnt(person).pin,
                                                     message_text,
                                                     int(answer_yes),
                                                 ),
                                             )
+                                    else:
+                                        pass
                             except NotFound as error:
                                 A.L.debug_bot(
                                     j((SD.standalone_name, ": ", error.get_details()))
                                 )
                         return True
         return None
```

