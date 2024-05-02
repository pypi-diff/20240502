# Comparing `tmp/email_profile-0.2.0.tar.gz` & `tmp/email_profile-0.3.0.tar.gz`

## Comparing `email_profile-0.2.0.tar` & `email_profile-0.3.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 email_profile-0.2.0/.env-example
--rw-r--r--   0        0        0    52850 2020-02-02 00:00:00.000000 email_profile-0.2.0/_poetry.lock
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 email_profile-0.2.0/_pyproject-poetry.toml
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 email_profile-0.2.0/example.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 email_profile-0.2.0/requirements-dev.txt
--rwxr-xr-x   0        0        0     1726 2020-02-02 00:00:00.000000 email_profile-0.2.0/setup.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 email_profile-0.2.0/tox.ini
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 email_profile-0.2.0/.github/workflows/python-app-code-quality.yml
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 email_profile-0.2.0/.github/workflows/python-app-test.yml
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 email_profile-0.2.0/.github/workflows/python-publish-pypi-test.yml
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 email_profile-0.2.0/.github/workflows/python-publish-pypi.yml
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/__init__.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/cli.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/core.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/data.py
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/message.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/utils.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/where.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/config/__init__.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/config/controller.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/config/database.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/models/__init__.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/models/attachment.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/models/email.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/models/mailbox.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/serializers/__init__.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/serializers/where.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.2.0/tests/email_profile/__init__.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 email_profile-0.2.0/tests/email_profile/test_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.2.0/tests/email_profile/test_message.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.2.0/tests/email_profile/serializers/__init__.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 email_profile-0.2.0/tests/email_profile/serializers/test_where.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.2.0/tests/email_profile/utils/__init__.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 email_profile-0.2.0/tests/email_profile/utils/test_mailbox.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 email_profile-0.2.0/tests/email_profile/utils/test_mode.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 email_profile-0.2.0/tests/email_profile/utils/test_status.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 email_profile-0.2.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 email_profile-0.2.0/LICENSE
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 email_profile-0.2.0/README.md
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 email_profile-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 email_profile-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 email_profile-0.3.0/.env-example
+-rw-r--r--   0        0        0    52850 2020-02-02 00:00:00.000000 email_profile-0.3.0/_poetry.lock
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 email_profile-0.3.0/_pyproject-poetry.toml
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 email_profile-0.3.0/example.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 email_profile-0.3.0/requirements-dev.txt
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 email_profile-0.3.0/setup.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 email_profile-0.3.0/tox.ini
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 email_profile-0.3.0/.github/workflows/python-app-code-quality.yml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 email_profile-0.3.0/.github/workflows/python-app-test.yml
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 email_profile-0.3.0/.github/workflows/python-publish-pypi-test.yml
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 email_profile-0.3.0/.github/workflows/python-publish-pypi.yml
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/__init__.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/cli.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/core.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/data.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/message.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/status.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/utils.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/where.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/abstract/__init__.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/abstract/controller.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/abstract/model.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/models/__init__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/models/attachment.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/models/email.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/models/mailbox.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/serializers/__init__.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 email_profile-0.3.0/email_profile/serializers/where.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.3.0/tests/email_profile/__init__.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 email_profile-0.3.0/tests/email_profile/test_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.3.0/tests/email_profile/test_message.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 email_profile-0.3.0/tests/email_profile/test_status.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 email_profile-0.3.0/tests/email_profile/test_where_mailbox.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 email_profile-0.3.0/tests/email_profile/test_where_mode.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.3.0/tests/email_profile/serializers/__init__.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 email_profile-0.3.0/tests/email_profile/serializers/test_where.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 email_profile-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 email_profile-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 email_profile-0.3.0/README.md
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 email_profile-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 email_profile-0.3.0/PKG-INFO
```

### Comparing `email_profile-0.2.0/_poetry.lock` & `email_profile-0.3.0/_poetry.lock`

 * *Files identical despite different names*

### Comparing `email_profile-0.2.0/_pyproject-poetry.toml` & `email_profile-0.3.0/_pyproject-poetry.toml`

 * *Files identical despite different names*

### Comparing `email_profile-0.2.0/example.py` & `email_profile-0.3.0/example.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,12 +40,17 @@
         # Email data model
         print(content.email.subject)
 
         # Attachments data model
         print(content.attachments)
 
         # Dump Json
-        print(content.json())
+        json = content.json()
+        print(json)
+
+        # Dump HMTL
+        html = content.html()
+        print(html)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `email_profile-0.2.0/setup.py` & `email_profile-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `email_profile-0.2.0/tox.ini` & `email_profile-0.3.0/tox.ini`

 * *Files identical despite different names*

### Comparing `email_profile-0.2.0/.github/workflows/python-app-code-quality.yml` & `email_profile-0.3.0/.github/workflows/python-app-code-quality.yml`

 * *Files identical despite different names*

### Comparing `email_profile-0.2.0/.github/workflows/python-app-test.yml` & `email_profile-0.3.0/.github/workflows/python-app-test.yml`

 * *Files identical despite different names*

### Comparing `email_profile-0.2.0/.github/workflows/python-publish-pypi-test.yml` & `email_profile-0.3.0/.github/workflows/python-publish-pypi-test.yml`

 * *Files identical despite different names*

### Comparing `email_profile-0.2.0/.github/workflows/python-publish-pypi.yml` & `email_profile-0.3.0/.github/workflows/python-publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `email_profile-0.2.0/email_profile/__init__.py` & `email_profile-0.3.0/email_profile/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 __author__ = 'Fernando Celmer <email@fernandocelmer.com>'
 __copyright__ = """MIT License
 
 Copyright (c) 2024 Email Profile
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,8 +21,10 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE."""
 
 from email_profile.core import Email
 
-__all__ = ['Email']
+__all__ = [
+    'Email'
+]
```

### Comparing `email_profile-0.2.0/email_profile/message.py` & `email_profile-0.3.0/email_profile/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 Message Module
 """
 
 from email import message_from_bytes
 from email.header import decode_header
 from email.utils import parsedate_to_datetime
 
-from email_profile.data import DataClass as Data
+from email_profile.data import DataClass
 from email_profile.models import AttachmentModel, EmailModel
 
 
 class Message:
 
     def __init__(self, message: bytes, id: int) -> None:
         self.message = message_from_bytes(message)
         self.id = id
         self.body_text_plain = ""
         self.body_text_html = ""
-        self.data = Data()
+        self.data = DataClass()
 
     def decode_field(self, header) -> str:
         field = ""
         for sub in decode_header(header):
             encoding = sub[1] or "utf-8"
             try:
                 field += sub[0].decode(encoding)
@@ -52,45 +52,43 @@
                 self.body_text_html = part.get_payload(decode=True)
                 if isinstance(self.body_text_html, bytes):
                     self.body_text_html = part.get_payload()
 
         if "attachment" in str(part.get("Content-Disposition")):
             filename = part.get_filename()
             if filename:
-                self.data.add_attachment(
-                    AttachmentModel(
-                        email_id=self.id,
-                        file_name=filename,
-                        content_type=part.get_content_type(),
-                        content_ascii=part.get_payload().encode("ascii")
-                    )
+                model = AttachmentModel(
+                    id=self.id,
+                    file_name=filename,
+                    content_type=part.get_content_type(),
+                    content_ascii=part.get_payload().encode("ascii")
                 )
+                self.data.add_attachment(model)
 
     def result(self) -> EmailModel:
         for part in self.message.walk():
             self.get_content(part=part)
 
-        self.data.add_email(
-            EmailModel(
-                id=self.id,
-                body_text_plain=self.body_text_plain,
-                body_text_html=self.body_text_html,
-                return_path=self.message.get("Return-Path"),
-                delivered_to=self.message.get("Delivered-To"),
-                received=self.message.get("Received"),
-                dkim_signature=self.message.get("DKIM-Signature"),
-                content_type=self.message.get_content_type(),
-                date=self.parsedate_to_datetime(self.message.get("Date")),
-                from_who=self.decode_field(self.message.get("From")),
-                mime_version=self.message.get("Mime-Version"),
-                message_id=self.message.get("Message-ID"),
-                subject=self.decode_field(self.message["Subject"]),
-                reply_to=self.message.get("Reply-To"),
-                precedence=self.message.get("Precedence"),
-                x_sg_eid=self.message.get("X-SG-EID"),
-                x_sg_id=self.message.get("X-SG-ID"),
-                to_who=self.message.get("To"),
-                x_entity_id=self.message.get("X-Entity-ID")
-            )
+        model = EmailModel(
+            id=self.id,
+            body_text_plain=self.body_text_plain,
+            body_text_html=self.body_text_html,
+            return_path=self.message.get("Return-Path"),
+            delivered_to=self.message.get("Delivered-To"),
+            received=self.message.get("Received"),
+            dkim_signature=self.message.get("DKIM-Signature"),
+            content_type=self.message.get_content_type(),
+            date=self.parsedate_to_datetime(self.message.get("Date")),
+            from_who=self.decode_field(self.message.get("From")),
+            mime_version=self.message.get("Mime-Version"),
+            message_id=self.message.get("Message-ID"),
+            subject=self.decode_field(self.message["Subject"]),
+            reply_to=self.message.get("Reply-To"),
+            precedence=self.message.get("Precedence"),
+            x_sg_eid=self.message.get("X-SG-EID"),
+            x_sg_id=self.message.get("X-SG-ID"),
+            to_who=self.message.get("To"),
+            x_entity_id=self.message.get("X-Entity-ID")
         )
+        self.data.add_email(model)
 
         return self.data
```

### Comparing `email_profile-0.2.0/email_profile/where.py` & `email_profile-0.3.0/email_profile/where.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 """
 Where Module
 """
 
 
-import logging
-
 from datetime import date
 from typing import Optional, List
 
-from email_profile.config.controller import (
-    AttachmentController,
-    EmailController
-)
-from email_profile.serializers import WhereSerializer
-from email_profile.utils import Status, Mode, Mailbox
+from email_profile.status import Status
 from email_profile.message import Message
+from email_profile.serializers import WhereSerializer
+
+
+class Mailbox:
+
+    INBOX = "INBOX"
+    SENT = "INBOX.Sent"
+    JUNK = "INBOX.Junk"
+    DRAFTS = "INBOX.Drafts"
+
+
+class Mode:
+
+    ALL = "ALL"
+    UNSEEN = "UNSEEN"
 
 
 class Where:
 
     _data = []
     _message = []
     _status = False
@@ -76,26 +84,14 @@
 
             for group_mail in splited:
                 _sum_searching += len(group_mail)
 
                 status, messages = self.server.fetch(','.join(group_mail), '(RFC822)')
                 messages = [message for message in messages if message != b')']
 
-                print(f"Searching: {_sum_searching}/{len(self._data)}")
+                print(f"Loading: {_sum_searching}/{len(self._data)}", end="\r")
 
                 for reference, text in messages:
                     _id = int(reference.split()[0])
                     self._message.append(Message(text, _id).result())
 
         return self._message
-
-    def dump_sqlite(self):
-        logging.warning(" Function 'dump_sqlite' not implemented")
-
-        sql_email = EmailController()
-        sql_attachmentl = AttachmentController()
-
-        for message in self._message:
-            sql_email.create(data=message.email)
-
-            for attachment in message.attachments:
-                sql_attachmentl.create(data=attachment)
```

### Comparing `email_profile-0.2.0/email_profile/models/email.py` & `email_profile-0.3.0/email_profile/models/email.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from typing import Optional
 from datetime import datetime
 from dataclasses import dataclass, field
 
+from email_profile.abstract import AbstractModel
+
 
 @dataclass
-class EmailModel:
+class EmailModel(AbstractModel):
 
-    __tablename__ = 'email'
+    class Meta:
+        table_name = 'email'
 
-    id: Optional[int] = field(default=None)
+    id: int = field(default=None)
     body_text_plain: str = field(default=None)
     body_text_html: str = field(default=None)
     return_path: str = field(default=None)
     delivered_to: str = field(default=None)
     received: str = field(default=None)
     dkim_signature: str = field(default=None)
     received: str = field(default=None)
```

### Comparing `email_profile-0.2.0/email_profile/serializers/where.py` & `email_profile-0.3.0/email_profile/serializers/where.py`

 * *Files identical despite different names*

### Comparing `email_profile-0.2.0/tests/email_profile/test_data.py` & `email_profile-0.3.0/tests/email_profile/test_data.py`

 * *Files identical despite different names*

### Comparing `email_profile-0.2.0/tests/email_profile/serializers/test_where.py` & `email_profile-0.3.0/tests/email_profile/serializers/test_where.py`

 * *Files identical despite different names*

### Comparing `email_profile-0.2.0/tests/email_profile/utils/test_status.py` & `email_profile-0.3.0/tests/email_profile/test_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from email_profile.utils import Status, StatusResponse
+from email_profile.status import Status, StatusResponse
 
 
 def test_status_ok():
     assert Status.OK == 'OK'
 
 
 def test_status_no():
```

### Comparing `email_profile-0.2.0/.gitignore` & `email_profile-0.3.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -138,8 +138,11 @@
 
 
 # Pypi
 .pypirc
 
 # Database
 *.sqlite3
-*.db
+*.db
+
+# Others
+html
```

### Comparing `email_profile-0.2.0/LICENSE` & `email_profile-0.3.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Fernando Celmer
+Copyright (c) 2024 Fernando Celmer
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `email_profile-0.2.0/README.md` & `email_profile-0.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 
 ---
 
 ## Check list
 
 - [x] Query API Structure
 - [x] Data table structure
-- [ ] SQLlite Backup
+- [x] Response JSON
+- [ ] Dump JSON
+- [x] Dump HTML
+- [x] Response HTML
 - [ ] CLI Email
 - [ ] Documentation
 
 ## How to install?
 
 ```python
 pip install email-profile
@@ -71,15 +74,21 @@
     # Email data model
     print(content.email.subject)
 
     # Attachments data model
     print(content.attachments)
 
     # Dump Json
-    print(content.json())
+    json = content.json()
+    print(json)
+
+    # Dump HMTL
+    html = content.html()
+    print(html)
+
 ```
 
 ## Commit Style
 
 - ⚙️ FEATURE
 - 📝 PEP8
 - 📌 ISSUE
```

### Comparing `email_profile-0.2.0/pyproject.toml` & `email_profile-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "email-profile"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="Fernando Celmer", email="email@fernandocelmer.com" },
 ]
 license = {file = "LICENSE"}
 description = "📩 Email Profile"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `email_profile-0.2.0/PKG-INFO` & `email_profile-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: email-profile
-Version: 0.2.0
+Version: 0.3.0
 Summary: 📩 Email Profile
 Project-URL: Homepage, https://github.com/linux-profile/email-profile
 Project-URL: Issues, https://github.com/linux-profile/email-profile/issues
 Project-URL: Repository, https://github.com/linux-profile/email-profile
 Project-URL: Documentation, https://github.com/linux-profile/email-profile/blob/master/README.md
 Author-email: Fernando Celmer <email@fernandocelmer.com>
 License: MIT License
         
-        Copyright (c) 2023 Fernando Celmer
+        Copyright (c) 2024 Fernando Celmer
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -53,15 +53,18 @@
 
 ---
 
 ## Check list
 
 - [x] Query API Structure
 - [x] Data table structure
-- [ ] SQLlite Backup
+- [x] Response JSON
+- [ ] Dump JSON
+- [x] Dump HTML
+- [x] Response HTML
 - [ ] CLI Email
 - [ ] Documentation
 
 ## How to install?
 
 ```python
 pip install email-profile
@@ -115,15 +118,21 @@
     # Email data model
     print(content.email.subject)
 
     # Attachments data model
     print(content.attachments)
 
     # Dump Json
-    print(content.json())
+    json = content.json()
+    print(json)
+
+    # Dump HMTL
+    html = content.html()
+    print(html)
+
 ```
 
 ## Commit Style
 
 - ⚙️ FEATURE
 - 📝 PEP8
 - 📌 ISSUE
```

