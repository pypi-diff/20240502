# Comparing `tmp/arched_emailer-0.2.8-py3-none-any.whl.zip` & `tmp/arched_emailer-0.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 8804 bytes, number of entries: 7
+Zip file size: 8837 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       42 b- defN 24-Jan-29 21:39 arched_emailer/__init__.py
--rw-r--r--  2.0 unx    22597 b- defN 24-Feb-09 23:48 arched_emailer/arched_emailer.py
+-rw-r--r--  2.0 unx    22707 b- defN 24-Feb-10 11:10 arched_emailer/arched_emailer.py
 -rw-r--r--  2.0 unx     1833 b- defN 24-Feb-09 09:41 arched_emailer/encryption.py
--rw-r--r--  2.0 unx     3453 b- defN 24-Feb-09 23:48 arched_emailer-0.2.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-09 23:48 arched_emailer-0.2.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 24-Feb-09 23:48 arched_emailer-0.2.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      582 b- defN 24-Feb-09 23:48 arched_emailer-0.2.8.dist-info/RECORD
-7 files, 28614 bytes uncompressed, 7766 bytes compressed:  72.9%
+-rw-r--r--  2.0 unx     3453 b- defN 24-Feb-10 11:10 arched_emailer-0.2.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Feb-10 11:10 arched_emailer-0.2.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-Feb-10 11:10 arched_emailer-0.2.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      582 b- defN 24-Feb-10 11:10 arched_emailer-0.2.9.dist-info/RECORD
+7 files, 28724 bytes uncompressed, 7799 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: arched_emailer/arched_emailer.py
 Comment: 
 
 Filename: arched_emailer/encryption.py
 Comment: 
 
-Filename: arched_emailer-0.2.8.dist-info/METADATA
+Filename: arched_emailer-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: arched_emailer-0.2.8.dist-info/WHEEL
+Filename: arched_emailer-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: arched_emailer-0.2.8.dist-info/top_level.txt
+Filename: arched_emailer-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: arched_emailer-0.2.8.dist-info/RECORD
+Filename: arched_emailer-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## arched_emailer/arched_emailer.py

```diff
@@ -8,15 +8,15 @@
 
 import requests
 from flask import request
 from smtpymailer import SmtpMailer
 
 from arched_emailer.encryption import obfuscate_sensitive_info, generate_random_string
 
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 
 BASE_URL = "https://arched.dev"
 
 
 class ArchedEmailer:
     """
     A class for sending emails.
@@ -329,22 +329,24 @@
         Returns:
             None
         """
         if kwargs.get("task_id"):
             data = {"sent_to": kwargs.get("recipients"), "sent_from": kwargs.get("sender"), "success": success,
                     "html_response": kwargs.get("html"), "task_id": kwargs.get("task_id")}
             self._make_request(f"{BASE_URL}/email/tasks/taskrun", method="POST", body=data)
-    def _get_html_content(self):
+    def _get_html_content(self, mailer:SmtpMailer):
         """
         Get the HTML content of the email.
+        Args:
+            mailer (SmtpMailer): The mailer object.
         Returns:
             str: The HTML content of the email.
         """
         html_content = ""
-        for part in self.mailer.message.walk():
+        for part in mailer.message.walk():
             # Check if the content type is HTML
             if part.get_content_type() == 'text/html':
                 # Get the HTML content and stop looping
                 return part.get_payload(decode=True).decode(part.get_content_charset())
 
         return html_content
 
@@ -387,15 +389,15 @@
 
             app_name = app if app else self.app
             if not update_db_only:
                 self.success_mailer.send_email(recipients, subject=f"Success: {app_name} - {generate_random_string()}",
                                            template=email_path, date=date, app=app_name,
                                            **kwargs)
             self._send_to_db(success=True, recipients=recipients, sender=self.success_mailer.sender.email,
-                             html=self._get_html_content(), task_id=task_id if task_id else self.task_id,
+                             html=self._get_html_content(self.success_mailer), task_id=task_id if task_id else self.task_id,
                              **kwargs)
 
         except Exception as e:
             print(e)
 
     def send_error_email(self, recipients: Union[str, list],
                          error_text: Optional[str] = None,
@@ -459,15 +461,15 @@
                     app_name = app if app else self.app
                     self.mailer.send_email(recipients, subject=f"Error: {app_name} - {error_id}",
                                            template=email_path, date=date, app=app_name, error_id=error_id,
                                            exception=exception, error_text=error_text, **template_data)
 
 
                     self._send_to_db(success=False, recipients=recipients, sender=self.mailer.sender.email,
-                                     html=self._get_html_content(), task_id=task_id if task_id else self.task_id)
+                                     html=self._get_html_content(self.mailer), task_id=task_id if task_id else self.task_id)
         except Exception as e:
             print(e)
 
     def try_log_function(self, error_recipients: Union[str, list], send_success: Optional[bool] = False,
                          success_recipients: Optional[Union[str, list]] = None, allowed_minutes=60,
                          task_id: Optional[int] = None, *args, **kwargs):
         """
```

## Comparing `arched_emailer-0.2.8.dist-info/METADATA` & `arched_emailer-0.2.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arched-emailer
-Version: 0.2.8
+Version: 0.2.9
 Summary: A emailing python library
 Home-page: https://github.com/lewis-morris/arched_emailer
 Author: lewis
 Author-email: lewis@arched.dev
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

