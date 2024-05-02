# Comparing `tmp/pih-ntfc_auto-0.15.tar.gz` & `tmp/pih-ntfc_auto-0.15.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-ntfc_auto-0.15.tar", last modified: Mon Apr 15 23:59:05 2024, max compression
+gzip compressed data, was "pih-ntfc_auto-0.15.1.tar", last modified: Thu May  2 01:35:27 2024, max compression
```

## Comparing `pih-ntfc_auto-0.15.tar` & `pih-ntfc_auto-0.15.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 23:59:05.988738 pih-ntfc_auto-0.15/
-drwxrwxrwx   0        0        0        0 2024-04-15 23:59:05.517294 pih-ntfc_auto-0.15/NotificationAutomationService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-ntfc_auto-0.15/NotificationAutomationService/__init__.py
--rw-rw-rw-   0        0        0      164 2024-04-15 23:57:16.000000 pih-ntfc_auto-0.15/NotificationAutomationService/__main__.py
--rw-rw-rw-   0        0        0     1615 2024-04-15 23:57:45.000000 pih-ntfc_auto-0.15/NotificationAutomationService/api.py
--rw-rw-rw-   0        0        0      424 2024-04-15 23:56:31.000000 pih-ntfc_auto-0.15/NotificationAutomationService/const.py
--rw-rw-rw-   0        0        0    19907 2024-04-15 23:57:45.000000 pih-ntfc_auto-0.15/NotificationAutomationService/service.py
--rw-rw-rw-   0        0        0      289 2024-04-15 23:59:05.942299 pih-ntfc_auto-0.15/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 23:59:05.910601 pih-ntfc_auto-0.15/pih_ntfc_auto.egg-info/
--rw-rw-rw-   0        0        0      289 2024-04-15 23:59:04.000000 pih-ntfc_auto-0.15/pih_ntfc_auto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2024-04-15 23:59:05.000000 pih-ntfc_auto-0.15/pih_ntfc_auto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 23:59:05.000000 pih-ntfc_auto-0.15/pih_ntfc_auto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2024-04-15 23:59:05.000000 pih-ntfc_auto-0.15/pih_ntfc_auto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-15 23:59:05.000000 pih-ntfc_auto-0.15/pih_ntfc_auto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2024-04-15 23:59:05.000000 pih-ntfc_auto-0.15/pih_ntfc_auto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 23:59:05.988738 pih-ntfc_auto-0.15/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-02 01:35:27.558481 pih-ntfc_auto-0.15.1/
+drwxrwxrwx   0        0        0        0 2024-05-02 01:35:27.011648 pih-ntfc_auto-0.15.1/NotificationAutomationService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-ntfc_auto-0.15.1/NotificationAutomationService/__init__.py
+-rw-rw-rw-   0        0        0      164 2024-04-15 23:57:16.000000 pih-ntfc_auto-0.15.1/NotificationAutomationService/__main__.py
+-rw-rw-rw-   0        0        0     1615 2024-04-15 23:57:45.000000 pih-ntfc_auto-0.15.1/NotificationAutomationService/api.py
+-rw-rw-rw-   0        0        0      426 2024-05-02 01:34:02.000000 pih-ntfc_auto-0.15.1/NotificationAutomationService/const.py
+-rw-rw-rw-   0        0        0    20480 2024-04-26 00:53:58.000000 pih-ntfc_auto-0.15.1/NotificationAutomationService/service.py
+-rw-rw-rw-   0        0        0      291 2024-05-02 01:35:27.495984 pih-ntfc_auto-0.15.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 01:35:27.433485 pih-ntfc_auto-0.15.1/pih_ntfc_auto.egg-info/
+-rw-rw-rw-   0        0        0      291 2024-05-02 01:35:26.000000 pih-ntfc_auto-0.15.1/pih_ntfc_auto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2024-05-02 01:35:26.000000 pih-ntfc_auto-0.15.1/pih_ntfc_auto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 01:35:26.000000 pih-ntfc_auto-0.15.1/pih_ntfc_auto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-05-02 01:35:26.000000 pih-ntfc_auto-0.15.1/pih_ntfc_auto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-02 01:35:26.000000 pih-ntfc_auto-0.15.1/pih_ntfc_auto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2024-05-02 01:35:26.000000 pih-ntfc_auto-0.15.1/pih_ntfc_auto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 01:35:27.558481 pih-ntfc_auto-0.15.1/setup.cfg
```

### Comparing `pih-ntfc_auto-0.15/NotificationAutomationService/api.py` & `pih-ntfc_auto-0.15.1/NotificationAutomationService/api.py`

 * *Files identical despite different names*

### Comparing `pih-ntfc_auto-0.15/NotificationAutomationService/service.py` & `pih-ntfc_auto-0.15.1/NotificationAutomationService/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,16 @@
         e,
         n,
         b,
         ne,
         nn,
         js,
         nl,
-        nns,
-        nni,
-        nndt,
+        jnl,
+        nnt,
         FullNameTool,
         while_not_do,
         ParameterList,
     )
     from NotificationAutomationService.api import (
         NotificationApi as Api,
     )
@@ -75,31 +74,33 @@
             MessageStatuses.REGISTERED, datetime
         )
         DH.message_stack += A.R_ME_D.get(search_critery, True).data or []
         search_critery.date = ""
         DH.message_stack += A.R_ME_D.get(search_critery, True).data or []
 
     def send_delayed_message(message: DelayedMessageDS) -> bool:
-        sender: str = nns(message.sender)
+        sender: str = nnt(message.sender)
         has_notification_confirmation: bool = A.C_P_N_С.exists(
-            nns(message.recipient), sender, True
+            nnt(message.recipient), sender, True
         )
-        message_id: int = nni(message.id)
+        message_id: int = nnt(message.id)
         if nn(message_id):
             person_visit_notification: PPVN | None = A.R_P_N.by_message_id(
                 message_id
             ).data
             if nn(person_visit_notification):
-                person_visit: PPVDS = A.R_P_V.by_id(
+                person_visit: PPVDS | None = A.R_P_V.by_id(
                     person_visit_notification.visitID
                 ).data
                 appointment_information: str | None = None
                 if nn(person_visit):
-                    is_prerecording: bool = person_visit.pin == A.CT_P.PRERECORDING_PIN
-                    if person_visit.serviceGroupID == 0:
+                    is_prerecording: bool = (
+                        nnt(person_visit).pin == A.CT_P.PRERECORDING_PIN
+                    )
+                    if nnt(person_visit).serviceGroupID == 0:
                         appointment_information = js(
                             ("приём к специалисту", b(person_visit.doctorFullName))
                         )
                     else:
                         appointment_information = A.CT_P.APPOINTMENT_SERVICE_GROUP_NAME[
                             A.D.get_by_value(
                                 A.CT_P.AppointmentServiceGroupId,
@@ -107,23 +108,25 @@
                             )
                         ]
                     message_text: str | None = None
                     person_name: str = FullNameTool.to_given_name(
                         person_visit_notification.FullName
                     )
                     type: PPVNType = A.D.get_by_value(
-                        PPVNType, person_visit_notification.type
+                        PPVNType, nnt(person_visit_notification).type
                     )
                     if type in [PPVNType.GREETING, PPVNType.DEFAULT]:
-                        if A.D.now() <= A.D.datetime_from_string(
-                            person_visit_notification.beginDate,
-                            A.CT.ISO_DATETIME_FORMAT,
+                        if A.D.now() <= nnt(
+                            A.D.datetime_from_string(
+                                person_visit_notification.beginDate,
+                                A.CT.ISO_DATETIME_FORMAT,
+                            )
                         ):
                             visit_date_time: datetime = A.D.datetime_from_string(
-                                person_visit.beginDate, A.CT.ISO_DATETIME_FORMAT
+                                nnt(person_visit).beginDate, A.CT.ISO_DATETIME_FORMAT
                             )
                             day_string: str = str(visit_date_time.day)
                             month_string: str = [
                                 "января",
                                 "февраля",
                                 "марта",
                                 "апреля",
@@ -161,21 +164,30 @@
                                 name=person_name,
                                 appointment_information=appointment_information,
                                 day_string=day_string,
                                 month_string=month_string,
                                 hour_string=hour_string,
                                 minute_string=minute_string,
                             )
+                            if is_prerecording:
+                                message_text = j(
+                                    (
+                                        message_text,
+                                        A.S.get(
+                                            A.CT_S.POLIBASE_PERSON_PRERECORDING_VISIT_NOTIFICATION
+                                        ),
+                                    )
+                                )
                         else:
                             message_text = A.S.get(
                                 A.CT_S.POLIBASE_PERSON_VISIT_GREETING_NOTIFICATION_TEXT_WITHOUT_DATE_FOR_CONFIRMED_NOTIFICATION
                                 if has_notification_confirmation
                                 else A.CT_S.POLIBASE_PERSON_VISIT_GREETING_NOTIFICATION_TEXT_WITHOUT_DATE
                             )
-                            message_text = nns(message_text).format(
+                            message_text = nnt(message_text).format(
                                 name=person_name,
                                 appointment_information=appointment_information,
                             )
                     elif type == PPVNType.REMINDER:
                         if person_visit.status == PolibasePersonVisitStatus.CONFIRMED:
                             visit_date_time: datetime = A.D.datetime_from_string(
                                 person_visit.beginDate, A.CT.ISO_DATETIME_FORMAT
@@ -192,19 +204,19 @@
                             ).format(
                                 name=person_name,
                                 visit_time=j(("в ", hour_string, minute_string)),
                                 appointment_information=appointment_information,
                             )
                         else:
                             A.L.polibase(
-                                j(
+                                js(
                                     (
-                                        "Сообщение (id: ",
+                                        "Сообщение:",
                                         message_id,
-                                        ") было сброшено. Причина: отказ от приёма",
+                                        "было сброшено. Причина: отказ от приёма",
                                     )
                                 ),
                                 A.CT_L_ME_F.ERROR,
                             )
                             A.A_ME_D.abort(message)
                     if ne(message_text):
                         message.message = message_text
@@ -232,27 +244,27 @@
         message_id: int | None = message.id
         if e(message_id):
             A.L.polibase(
                 j(
                     (
                         "Сообщение (id: ",
                         message_id,
-                        ") не было отправлено аббоненту: ",
+                        ") не было отправлено клиенту: ",
                         message.recipient,
                     )
                 ),
                 A.CT_L_ME_F.ERROR,
             )
         else:
             A.L.polibase(
-                j(
+                js(
                     (
-                        "Сообщение (id: ",
+                        "Сообщение: ",
                         message_id,
-                        ") было отправлено аббоненту: ",
+                        "было отправлено клиенту:",
                         message.recipient,
                     )
                 )
             )
             if message_id == 0:
                 return True
             return A.A_ME_D.complete(message)
@@ -273,21 +285,21 @@
                                 A.S.get(
                                     A.CT_S.WHATSAPP_BUFFERED_MESSAGE_MAX_DELAY_IN_MILLISECONDS
                                 ),
                             )
                             sleep(delay / 1000)
                 except Exception as error:
                     A.L.polibase(
-                        j(
+                        js(
                             (
-                                "Ошибка при отправке сообщения (id: ",
+                                "Ошибка при отправке сообщения:",
                                 message.id,
-                                ") аббоненту ",
+                                "клиенту",
                                 message.recipient,
-                                "! Ошибка: ",
+                                nl("Ошибка: "),
                                 error,
                             )
                         ),
                         A.CT_L_ME_F.ERROR,
                     )
             else:
                 sleep(1)
@@ -308,15 +320,15 @@
         last_visit_id: int | None = A.D.if_not_empty(
             A.R_P_V_DS.last().data, lambda item: item.id
         )
         visit_list_result: Result[list[PPVDS]] | None = None
         if n(last_visit_id):
             visit_list_result = A.R_P_V.today()
         else:
-            visit_list_result = A.R_P_V.after_id(last_visit_id)
+            visit_list_result = A.R_P_V.after_id(nnt(last_visit_id))
         if ne(visit_list_result):
             visit_map: dict[str | int, list] = defaultdict(list)
 
             def fill_person_visits_map(visit: PPVDS) -> None:
                 if visit.pin == A.CT_P.PRERECORDING_PIN:
                     visit_map[visit.telephoneNumber].append(visit)
                 else:
```

