# Comparing `tmp/pih-answ_auto-0.17.tar.gz` & `tmp/pih-answ_auto-0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-answ_auto-0.17.tar", last modified: Fri Apr 19 02:20:38 2024, max compression
+gzip compressed data, was "pih-answ_auto-0.18.tar", last modified: Wed Apr 24 04:50:16 2024, max compression
```

## Comparing `pih-answ_auto-0.17.tar` & `pih-answ_auto-0.18.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 02:20:38.511806 pih-answ_auto-0.17/
-drwxrwxrwx   0        0        0        0 2024-04-19 02:20:37.597884 pih-answ_auto-0.17/AnswerAutomationService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-answ_auto-0.17/AnswerAutomationService/__init__.py
--rw-rw-rw-   0        0        0      158 2024-04-16 00:17:31.000000 pih-answ_auto-0.17/AnswerAutomationService/__main__.py
--rw-rw-rw-   0        0        0      412 2024-04-19 00:58:50.000000 pih-answ_auto-0.17/AnswerAutomationService/const.py
--rw-rw-rw-   0        0        0     7997 2024-04-19 01:17:29.000000 pih-answ_auto-0.17/AnswerAutomationService/service.py
--rw-rw-rw-   0        0        0      283 2024-04-19 02:20:38.479533 pih-answ_auto-0.17/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-19 02:20:38.432676 pih-answ_auto-0.17/pih_answ_auto.egg-info/
--rw-rw-rw-   0        0        0      283 2024-04-19 02:20:37.000000 pih-answ_auto-0.17/pih_answ_auto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2024-04-19 02:20:37.000000 pih-answ_auto-0.17/pih_answ_auto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 02:20:37.000000 pih-answ_auto-0.17/pih_answ_auto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-04-19 02:20:37.000000 pih-answ_auto-0.17/pih_answ_auto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-19 02:20:37.000000 pih-answ_auto-0.17/pih_answ_auto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-19 02:20:37.000000 pih-answ_auto-0.17/pih_answ_auto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 02:20:38.527450 pih-answ_auto-0.17/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 04:50:16.587168 pih-answ_auto-0.18/
+drwxrwxrwx   0        0        0        0 2024-04-24 04:50:16.191413 pih-answ_auto-0.18/AnswerAutomationService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-answ_auto-0.18/AnswerAutomationService/__init__.py
+-rw-rw-rw-   0        0        0      158 2024-04-16 00:17:31.000000 pih-answ_auto-0.18/AnswerAutomationService/__main__.py
+-rw-rw-rw-   0        0        0      412 2024-04-24 04:49:20.000000 pih-answ_auto-0.18/AnswerAutomationService/const.py
+-rw-rw-rw-   0        0        0     6914 2024-04-24 04:49:24.000000 pih-answ_auto-0.18/AnswerAutomationService/service.py
+-rw-rw-rw-   0        0        0      283 2024-04-24 04:50:16.555920 pih-answ_auto-0.18/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 04:50:16.524671 pih-answ_auto-0.18/pih_answ_auto.egg-info/
+-rw-rw-rw-   0        0        0      283 2024-04-24 04:50:15.000000 pih-answ_auto-0.18/pih_answ_auto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      363 2024-04-24 04:50:15.000000 pih-answ_auto-0.18/pih_answ_auto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 04:50:15.000000 pih-answ_auto-0.18/pih_answ_auto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-04-24 04:50:15.000000 pih-answ_auto-0.18/pih_answ_auto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-24 04:50:15.000000 pih-answ_auto-0.18/pih_answ_auto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-24 04:50:15.000000 pih-answ_auto-0.18/pih_answ_auto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 04:50:16.602791 pih-answ_auto-0.18/setup.cfg
```

### Comparing `pih-answ_auto-0.17/AnswerAutomationService/service.py` & `pih-answ_auto-0.18/AnswerAutomationService/service.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         PolibasePerson,
         WhatsAppMessage,
         PolibasePersonVisitDS as PPVDS,
         PolibasePersonNotificationConfirmation as PPNC,
     )
 
     from pih import serve, subscribe_on
-    from pih.tools import ParameterList, ne, nn, lw, one, nnt
+    from pih.tools import ParameterList, j, js, ne, nn, one, nnt
 
     SENDER: str = A.D.get(A.CT_ME_WH_W.Profiles.CALL_CENTRE)
 
     def polibase_person_name_format(value: str, polibase_person: PolibasePerson) -> str:
         return value.format(name=A.D.to_given_name(polibase_person))
 
     def server_call_handler(sc: SC, pl: ParameterList) -> bool | None:
@@ -47,72 +47,54 @@
                         notification_confirmation: PPNC | None = A.R_P_N_C.by(
                             telephone_number, sender
                         ).data
                         if (
                             ne(notification_confirmation)
                             and nnt(notification_confirmation).status == 2
                         ):
-                            visit_ds: PPVDS | None = one(
+                            polibase_person_visit_ds: PPVDS | None = one(
                                 A.R_P_V_DS.search(
                                     PPVDS(
                                         telephoneNumber=A.D_F.telephone_number(
                                             telephone_number
                                         )
                                     )
                                 )
                             )
-                            if nn(visit_ds):
-                                pin: int = nnt(nnt(visit_ds).pin)
+                            if nn(polibase_person_visit_ds):
+                                pin: int = nnt(nnt(polibase_person_visit_ds).pin)
                                 person: PolibasePerson = (
                                     PolibasePerson(
                                         pin,
-                                        nnt(visit_ds).FullName,
-                                        nnt(visit_ds).telephoneNumber,
+                                        nnt(polibase_person_visit_ds).FullName,
+                                        nnt(polibase_person_visit_ds).telephoneNumber,
                                     )
                                     if pin == A.CT_P.PRERECORDING_PIN
                                     else A.D_P.person_by_pin(pin)
                                 )
                                 if A.A_P_N_C.update(telephone_number, sender, 1):
 
                                     answer_type: int | None = None
 
                                     message: str = nnt(nnt(whatsapp_message).message)
-                                    mesasge_word_list: list[str] = lw(
-                                        A.D.not_empty_items(
-                                            nnt(A.D.space_format(message)).split(" ")
-                                        )
-                                    )  # type: ignore
-                                    tax_certificate_variant_list: list[str] = A.S.get(
-                                        A.CT_S.POLIBASE_ANSWER_PERSON_TAX_CERTIFICATE_VARIANTS
-                                    )
-                                    visit_modification_variant_list: list[str] = (
-                                        A.S.get(
-                                            A.CT_S.POLIBASE_PERSON_ANSWER_VISIT_MODIFICATION_VARIANTS
-                                        )
-                                    )
-                                    for word in mesasge_word_list:
-                                        if nn(answer_type):
+
+                                    for index, variants in enumerate(
+                                        [
+                                            A.S.get(
+                                                A.CT_S.POLIBASE_ANSWER_PERSON_TAX_CERTIFICATE_VARIANTS
+                                            ),
+                                            A.S.get(
+                                                A.CT_S.POLIBASE_PERSON_ANSWER_VISIT_MODIFICATION_VARIANTS
+                                            ),
+                                        ],
+                                    ):
+                                        if A.D.has_one_of(message, variants):
+                                            answer_type = index
                                             break
-                                        for (
-                                            tax_certificate_word
-                                        ) in tax_certificate_variant_list:
-                                            if word.startswith(tax_certificate_word):
-                                                answer_type = (
-                                                    ANSWER_TYPE.TAX_CERTIFICATE
-                                                )
-                                                break
-
-                                        for (
-                                            visit_modification_word
-                                        ) in visit_modification_variant_list:
-                                            if word.startswith(visit_modification_word):
-                                                answer_type = (
-                                                    ANSWER_TYPE.VISIT_MODIFICATION
-                                                )
-                                                break
+                                        
                                     answer_type = answer_type or ANSWER_TYPE.VISIT
 
                                     A.ME_WH_W_Q.add_message(
                                         Message(
                                             [
                                                 A.S_P_V.offer_telegram_bot_url_text(
                                                     person
@@ -145,14 +127,15 @@
                                                     A.CT_P.TAX_CERTIFICATE_URL,
                                                 ][answer_type],
                                                 telephone_number,
                                                 sender,
                                             )
                                         )
 
+                                    A.L.polibase(js(("Тип ответа:", answer_type)))
                                     A.E.polibase_person_answered(person, message)
         return None
 
     def service_starts_handler() -> None:
         subscribe_on(SC.send_event)
 
     serve(
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

