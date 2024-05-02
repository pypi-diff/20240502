# Comparing `tmp/pih-answ_auto-0.18.tar.gz` & `tmp/pih-answ_auto-0.18.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-answ_auto-0.18.tar", last modified: Wed Apr 24 04:50:16 2024, max compression
+gzip compressed data, was "pih-answ_auto-0.18.2.tar", last modified: Thu May  2 01:34:41 2024, max compression
```

## Comparing `pih-answ_auto-0.18.tar` & `pih-answ_auto-0.18.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 04:50:16.587168 pih-answ_auto-0.18/
-drwxrwxrwx   0        0        0        0 2024-04-24 04:50:16.191413 pih-answ_auto-0.18/AnswerAutomationService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-answ_auto-0.18/AnswerAutomationService/__init__.py
--rw-rw-rw-   0        0        0      158 2024-04-16 00:17:31.000000 pih-answ_auto-0.18/AnswerAutomationService/__main__.py
--rw-rw-rw-   0        0        0      412 2024-04-24 04:49:20.000000 pih-answ_auto-0.18/AnswerAutomationService/const.py
--rw-rw-rw-   0        0        0     6914 2024-04-24 04:49:24.000000 pih-answ_auto-0.18/AnswerAutomationService/service.py
--rw-rw-rw-   0        0        0      283 2024-04-24 04:50:16.555920 pih-answ_auto-0.18/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 04:50:16.524671 pih-answ_auto-0.18/pih_answ_auto.egg-info/
--rw-rw-rw-   0        0        0      283 2024-04-24 04:50:15.000000 pih-answ_auto-0.18/pih_answ_auto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2024-04-24 04:50:15.000000 pih-answ_auto-0.18/pih_answ_auto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 04:50:15.000000 pih-answ_auto-0.18/pih_answ_auto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-04-24 04:50:15.000000 pih-answ_auto-0.18/pih_answ_auto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-24 04:50:15.000000 pih-answ_auto-0.18/pih_answ_auto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-24 04:50:15.000000 pih-answ_auto-0.18/pih_answ_auto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 04:50:16.602791 pih-answ_auto-0.18/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-02 01:34:41.984393 pih-answ_auto-0.18.2/
+drwxrwxrwx   0        0        0        0 2024-05-02 01:34:41.146307 pih-answ_auto-0.18.2/AnswerAutomationService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-answ_auto-0.18.2/AnswerAutomationService/__init__.py
+-rw-rw-rw-   0        0        0      158 2024-04-16 00:17:31.000000 pih-answ_auto-0.18.2/AnswerAutomationService/__main__.py
+-rw-rw-rw-   0        0        0      414 2024-05-02 01:30:04.000000 pih-answ_auto-0.18.2/AnswerAutomationService/const.py
+-rw-rw-rw-   0        0        0     6961 2024-05-02 01:29:52.000000 pih-answ_auto-0.18.2/AnswerAutomationService/service.py
+-rw-rw-rw-   0        0        0      285 2024-05-02 01:34:41.953139 pih-answ_auto-0.18.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 01:34:41.903836 pih-answ_auto-0.18.2/pih_answ_auto.egg-info/
+-rw-rw-rw-   0        0        0      285 2024-05-02 01:34:39.000000 pih-answ_auto-0.18.2/pih_answ_auto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      363 2024-05-02 01:34:40.000000 pih-answ_auto-0.18.2/pih_answ_auto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 01:34:39.000000 pih-answ_auto-0.18.2/pih_answ_auto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-05-02 01:34:39.000000 pih-answ_auto-0.18.2/pih_answ_auto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-02 01:34:39.000000 pih-answ_auto-0.18.2/pih_answ_auto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-02 01:34:39.000000 pih-answ_auto-0.18.2/pih_answ_auto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 01:34:42.000014 pih-answ_auto-0.18.2/setup.cfg
```

### Comparing `pih-answ_auto-0.18/AnswerAutomationService/service.py` & `pih-answ_auto-0.18.2/AnswerAutomationService/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import ipih
 
 from pih import A
+from pih.tools import BitMask as BM
 from AnswerAutomationService.const import SD
 
 SC = A.CT_SC
 
 ISOLATED: bool = False
 
 
 class ANSWER_TYPE:
 
-    VISIT = 0
-    TAX_CERTIFICATE = 1
-    VISIT_MODIFICATION = 2
+    VISIT = 1
+    TAX_CERTIFICATE = 2
+    VISIT_MODIFICATION = 4
 
 
 def start(as_standalone: bool = False) -> None:
 
     from pih.collections import (
         Message,
         PolibasePerson,
@@ -69,72 +70,76 @@
                                         nnt(polibase_person_visit_ds).telephoneNumber,
                                     )
                                     if pin == A.CT_P.PRERECORDING_PIN
                                     else A.D_P.person_by_pin(pin)
                                 )
                                 if A.A_P_N_C.update(telephone_number, sender, 1):
 
-                                    answer_type: int | None = None
+                                    answer_type: int = 0
 
                                     message: str = nnt(nnt(whatsapp_message).message)
 
                                     for index, variants in enumerate(
                                         [
                                             A.S.get(
                                                 A.CT_S.POLIBASE_ANSWER_PERSON_TAX_CERTIFICATE_VARIANTS
                                             ),
                                             A.S.get(
                                                 A.CT_S.POLIBASE_PERSON_ANSWER_VISIT_MODIFICATION_VARIANTS
                                             ),
                                         ],
                                     ):
                                         if A.D.has_one_of(message, variants):
-                                            answer_type = index
-                                            break
-                                        
-                                    answer_type = answer_type or ANSWER_TYPE.VISIT
-
-                                    A.ME_WH_W_Q.add_message(
-                                        Message(
-                                            [
-                                                A.S_P_V.offer_telegram_bot_url_text(
-                                                    person
-                                                ),
-                                                polibase_person_name_format(
-                                                    A.S.get(
-                                                        A.CT_S.POLIBASE_PERSON_ANSWER_TAX_CERTIFICATE_TEXT
-                                                    ),
-                                                    person,
-                                                ),
-                                                polibase_person_name_format(
-                                                    A.S.get(
-                                                        A.CT_S.POLIBASE_PERSON_ANSWER_VISIT_MODIFICATION_TEXT
-                                                    ),
-                                                    person,
-                                                ),
-                                            ][answer_type],
-                                            telephone_number,
-                                            sender,
-                                        )
-                                    )
-                                    if answer_type in (
-                                        ANSWER_TYPE.VISIT,
-                                        ANSWER_TYPE.TAX_CERTIFICATE,
-                                    ):
+                                            answer_type |= 2 ^ (index + 1)
+
+                                    if answer_type == 0:
+                                        answer_type = ANSWER_TYPE.VISIT
+
+                                    def send_message(value: str) -> None:
                                         A.ME_WH_W_Q.add_message(
                                             Message(
-                                                [
-                                                    A.CT_P.TELEGRAM_BOT_URL,
-                                                    A.CT_P.TAX_CERTIFICATE_URL,
-                                                ][answer_type],
+                                                value,
                                                 telephone_number,
                                                 sender,
                                             )
                                         )
 
+                                    if BM.has(answer_type, ANSWER_TYPE.VISIT):
+                                        send_message(
+                                            A.S_P_V.offer_telegram_bot_url_text(person)
+                                        )
+                                        send_message(
+                                            A.S.get(A.CT_S.TELEGRAM_BOT_URL),
+                                        )
+
+                                    if BM.has(answer_type, ANSWER_TYPE.TAX_CERTIFICATE):
+                                        send_message(
+                                            polibase_person_name_format(
+                                                A.S.get(
+                                                    A.CT_S.POLIBASE_PERSON_ANSWER_TAX_CERTIFICATE_TEXT
+                                                ),
+                                                person,
+                                            )
+                                        )
+                                        send_message(
+                                            A.S.get(A.CT_S.TAX_CERTIFICATE_URL),
+                                        )
+
+                                    if BM.has(
+                                        answer_type, ANSWER_TYPE.VISIT_MODIFICATION
+                                    ):
+                                        send_message(
+                                            polibase_person_name_format(
+                                                A.S.get(
+                                                    A.CT_S.POLIBASE_PERSON_ANSWER_VISIT_MODIFICATION_TEXT
+                                                ),
+                                                person,
+                                            ),
+                                        )
+
                                     A.L.polibase(js(("Тип ответа:", answer_type)))
                                     A.E.polibase_person_answered(person, message)
         return None
 
     def service_starts_handler() -> None:
         subscribe_on(SC.send_event)
```

