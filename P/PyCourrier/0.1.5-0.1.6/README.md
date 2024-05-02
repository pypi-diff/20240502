# Comparing `tmp/PyCourrier-0.1.5.tar.gz` & `tmp/PyCourrier-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCourrier-0.1.5.tar", last modified: Mon Apr 29 20:02:23 2024, max compression
+gzip compressed data, was "PyCourrier-0.1.6.tar", last modified: Thu May  2 02:31:56 2024, max compression
```

## Comparing `PyCourrier-0.1.5.tar` & `PyCourrier-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 20:02:23.269662 PyCourrier-0.1.5/
--rw-rw-rw-   0        0        0     1096 2024-04-29 15:53:14.000000 PyCourrier-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     3089 2024-04-29 20:02:23.263677 PyCourrier-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-29 20:02:23.229769 PyCourrier-0.1.5/PyCourrier/
--rw-rw-rw-   0        0        0     4392 2024-04-29 19:17:51.000000 PyCourrier-0.1.5/PyCourrier/MailSender.py
--rw-rw-rw-   0        0        0       34 2024-04-29 16:41:54.000000 PyCourrier-0.1.5/PyCourrier/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 20:02:23.261691 PyCourrier-0.1.5/PyCourrier.egg-info/
--rw-rw-rw-   0        0        0     3089 2024-04-29 20:02:23.000000 PyCourrier-0.1.5/PyCourrier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-04-29 20:02:23.000000 PyCourrier-0.1.5/PyCourrier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 20:02:23.000000 PyCourrier-0.1.5/PyCourrier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-29 20:02:23.000000 PyCourrier-0.1.5/PyCourrier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2649 2024-04-29 19:57:25.000000 PyCourrier-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 20:02:23.269662 PyCourrier-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      686 2024-04-29 20:01:30.000000 PyCourrier-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 02:31:56.866898 PyCourrier-0.1.6/
+-rw-rw-rw-   0        0        0     1096 2024-04-29 15:53:14.000000 PyCourrier-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     3223 2024-05-02 02:31:56.862077 PyCourrier-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 02:31:56.788350 PyCourrier-0.1.6/PyCourrier/
+-rw-rw-rw-   0        0        0     5938 2024-05-02 02:28:17.000000 PyCourrier-0.1.6/PyCourrier/MailSender.py
+-rw-rw-rw-   0        0        0       34 2024-04-29 16:41:54.000000 PyCourrier-0.1.6/PyCourrier/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 02:31:56.859038 PyCourrier-0.1.6/PyCourrier.egg-info/
+-rw-rw-rw-   0        0        0     3223 2024-05-02 02:31:56.000000 PyCourrier-0.1.6/PyCourrier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-05-02 02:31:56.000000 PyCourrier-0.1.6/PyCourrier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 02:31:56.000000 PyCourrier-0.1.6/PyCourrier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-02 02:31:56.000000 PyCourrier-0.1.6/PyCourrier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2783 2024-05-02 02:30:24.000000 PyCourrier-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-02 02:31:56.868893 PyCourrier-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      686 2024-05-02 02:28:31.000000 PyCourrier-0.1.6/setup.py
```

### Comparing `PyCourrier-0.1.5/LICENSE` & `PyCourrier-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCourrier-0.1.5/PKG-INFO` & `PyCourrier-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCourrier
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple email sender utility
 Home-page: https://github.com/mjiid/PyCourrier
 Author: Abdelmajid Habouch
 Author-email: Habush1610@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -32,48 +32,56 @@
 ```
 
 ## Usage
 
 Here's a quick guide on how to use MailSender:
 
 ```python
-from PyCourrier import MailSender
+from PyCourrier import MailSender, run
 
-# Create a MailSender instance within a context manager
-with MailSender('your_email@gmail.com', 'your_generated_app_password') as mailSender:
+async def main():
+    # Create a MailSender instance within a context manager
+    with MailSender('your_email@gmail.com', 'your_generated_app_password') as sender:
 
-    # Set recipients
-    recipients = ['recipient1@gmail.com']
-    mailSender.set_recipients(recipients)
-
-    # Set email message details
-    in_subject='Hello from PyCourrier!',
-    in_plaintext='This is the plain text content of the email.',
-    in_from='your_email@gmail.com (optioanl)',
-    in_htmltext='<p>This is the HTML content of the email.</p> (optional)',
-    attachment="path/to/file (optional)",
-    filename="filename_for_the_attachment (optional)"
+        # Set recipients
+        recipients = ['recipient1@gmail.com', 'recipient2@gmail.com', 'recipient3@gmail.com']
+        sender.set_recipients(recipients)
 
-    mailSender.set_message(in_plaintext=plaintext_body, in_subject=in_subject, in_from=in_from, in_htmltext=in_htmltext, attachment=attachment, filename=filename)
+        # Set email message details
+        in_subject='Hello from PyCourrier!'
+        in_plaintext='This is the plain text content of the email.'
+        in_htmltext='<p>This is the HTML content of the email.</p> (optional)'
+
+        # Add attachments (optional)
+        sender.add_attachment('path/to/attachment', 'filename')
+
+        # set the message
+        sender.set_message(in_plaintext=in_plaintext, in_subject=in_subject, in_htmltext=in_htmltext)
+        await sender.send_all_async()
+
+
+# Run the async main function
+if __name__ == "__main__":
+    run(main())
 
-    # Send the email to all recipients
-    mailSender.send_all()
 ```
 
-## Constructor Parameters
+## Parameters:
 - **in_username**: Your email address used for SMTP login.
-- **in_password**: Your Generated app password.
+- **in_password**: Your generated app password for SMTP login.
 - **in_server**: Tuple containing the SMTP server address and port (default is Gmail).
 - **use_SSL**: Boolean indicating whether to use SSL (True) or TLS (False, default) for the connection.
-Methods
-- **set_message**: Compose the email message with subject, plaintext, HTML content, and optional attachments.
+
+## Methods:
+- **set_message**: Compose the email message with subject, plaintext, and HTML content.
+- **add_attachment**: Add an attachment to the email.
 - **set_recipients**: Set the list of email recipients.
-- **add_recipient**: Add a single recipient to the list of recipients.
 - **connect**: Connect to the SMTP server.
 - **disconnect**: Disconnect from the SMTP server.
-- **send_all**: Send the composed email to all recipients.
+- **send_all_async**: Send the composed email to all recipients asynchronously.
+- **send_email**: Send the composed email to a specific recipient.
 
 ## Contribution
 Contributions to PyCourrier are welcome! If you encounter any issues or have suggestions for improvements, please open an [issue on GitHub](https://github.com/mjiid/PyCourrier/issues).
 
 ## License
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `PyCourrier-0.1.5/PyCourrier/MailSender.py` & `PyCourrier-0.1.6/PyCourrier/MailSender.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import smtplib
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from email.mime.base import MIMEBase
 from email import encoders
 from contextlib import AbstractContextManager
+import logging
+from asyncio import gather, get_event_loop, run
+
+
+# Setup logging
+logging.basicConfig(level=logging.DEBUG)
 
 class MailSender(AbstractContextManager):
     """
     A class that facilitates composing and sending emails via SMTP.
 
     :param in_username: Username for mail server login
     :param in_password: Password for mail server login
@@ -18,99 +24,132 @@
         self.username = in_username
         self.password = in_password
         self.server_name, self.server_port = in_server
         self.use_SSL = use_SSL
         self.smtpserver = None
         self.connected = False
         self.recipients = []
+        self.attachments = []
+        self.msg = None
 
     def __enter__(self):
         self.connect()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.disconnect()
 
-    def __str__(self):
-        return f"MailSender connected to {self.server_name}:{self.server_port}, Connected: {self.connected}"
+    def connect(self):
+        """Connect to the SMTP server."""
+        try:
+            if self.use_SSL:
+                self.smtpserver = smtplib.SMTP_SSL(self.server_name, self.server_port)
+            else:
+                self.smtpserver = smtplib.SMTP(self.server_name, self.server_port)
+                self.smtpserver.starttls()
 
-    def set_message(self, in_plaintext="", in_subject="", in_from=None, in_htmltext=None, attachment=None, filename=None):
+            self.smtpserver.login(self.username, self.password)
+            self.connected = True
+            logging.info(f"Connected to {self.server_name}")
+        except (smtplib.SMTPException, ConnectionError) as error:
+            self.connected = False
+            logging.error(f"Failed to connect to {self.server_name}: {error}")
+            raise ConnectionError(f"Failed to connect to {self.server_name}: {error}")
+
+    def disconnect(self):
+        """Disconnect from the SMTP server."""
+        if self.smtpserver:
+            try:
+                self.smtpserver.quit()
+            except Exception as e:
+                logging.warning(f"Error disconnecting from SMTP server: {e}")
+            finally:
+                self.connected = False
+                logging.info("Disconnected.")
+
+    def set_message(self, in_subject="", in_from=None, in_plaintext=None, in_htmltext=None):
         """
         Compose an email message.
 
         :param in_plaintext: Plain text email body (required if no HTML text is provided)
         :param in_subject: Subject line
         :param in_from: Sender address
         :param in_htmltext: HTML version of the email body
-        :param attachment: Path to attachment file
-        :param filename: Filename for the attachment
         """
         self.msg = MIMEMultipart('alternative')
+        self.msg['Subject'] = in_subject
+        self.msg['From'] = in_from or self.username
 
-        if in_htmltext:
-            self.msg.attach(MIMEText(in_htmltext, 'html'))
         if in_plaintext:
             self.msg.attach(MIMEText(in_plaintext, 'plain'))
-
-        self.msg['Subject'] = in_subject
-        self.msg['From'] = in_from or self.username
+        if in_htmltext:
+            self.msg.attach(MIMEText(in_htmltext, 'html'))
 
         # Include an attachment if specified
-        if attachment:
-            part = MIMEBase('application', "octet-stream")
-            part.set_payload(open(attachment, "rb").read())
-            encoders.encode_base64(part)
-            part.add_header('Content-Disposition', f"attachment; filename={filename}")
-            self.msg.attach(part)
+        for attachment in self.attachments:
+            try:
+                with open(attachment['path'], 'rb') as f:
+                    part = MIMEBase('application', 'octet-stream')
+                    part.set_payload(f.read())
+                    encoders.encode_base64(part)
+                    part.add_header(
+                        'Content-Disposition', 
+                        f'attachment; filename={attachment["filename"]}'
+                    )
+                    self.msg.attach(part)
+            except IOError as e:
+                logging.error(f"Failed to attach file {attachment['path']}: {e}")
+                raise
+
+    def add_attachment(self, path, filename):
+        """Add an attachment"""
+        self.attachments.append({'path': path, 'filename': filename})
 
     def set_recipients(self, in_recipients):
         """
         Set the recipients for the email.
 
         :param in_recipients: List of recipient email addresses
         """
         if isinstance(in_recipients, (list, tuple)):
             self.recipients = in_recipients
         else:
+            logging.error("Recipients must be a list or tuple")
             raise TypeError("Recipients must be a list or tuple")
 
-    def add_recipient(self, in_recipient):
-        """Add a recipient to the list of recipients."""
-        self.recipients.append(in_recipient)
-
-    def connect(self):
-        """Connect to the SMTP server."""
-        try:
-            if self.use_SSL:
-                self.smtpserver = smtplib.SMTP_SSL(self.server_name, self.server_port)
-            else:
-                self.smtpserver = smtplib.SMTP(self.server_name, self.server_port)
-                self.smtpserver.starttls()
-
-            self.smtpserver.login(self.username, self.password)
-            self.connected = True
-            print(f"Connected to {self.server_name}")
-        except (smtplib.SMTPException, ConnectionError) as error:
-            self.connected = False
-            raise ConnectionError(f"Failed to connect to {self.server_name}: {error}")
-
-
-    def disconnect(self):
-        """Disconnect from the SMTP server."""
-        if self.smtpserver:
-            self.smtpserver.quit()
-            self.connected = False
-
-    def send_all(self, close_connection=True):
+    async def send_all_async(self):
         """Send the email to all recipients."""
         if not self.connected:
+            logging.error("Not connected to any server. Please connect first.")
             raise ConnectionError("Not connected to any server. Please connect first.")
 
-        for recipient in self.recipients:
-            self.msg['To'] = recipient 
-            print(f"Sending to {recipient}")
+        if not self.msg:
+            logging.error("Message not set. Please set the message before sending.")
+            raise ValueError("Message not set.")
 
-            # Convert the message to a string and then send it
-            self.smtpserver.sendmail(self.username, recipient, self.msg.as_string())
+        try:
+            # Set the 'To' header with all recipients
+            self.msg['To'] = ", ".join(self.recipients)
+
+            tasks = []
+            loop = get_event_loop()
 
-        print("All messages sent")
+            for recipient in self.recipients:
+                task = loop.create_task(self.send_email(recipient))
+                tasks.append(task)
+
+            await gather(*tasks)
+            logging.info("All messages sent")
+        except smtplib.SMTPException as error:
+            logging.error(f"Failed to send mail: {error}")
+            raise
 
+    async def send_email(self, recipient):
+        """Send the email to a recipient."""
+        try:
+            logging.info(f"Sending to {recipient}")
+            
+            # Convert the message to a string and then send it
+            self.smtpserver.sendmail(self.username, recipient, self.msg.as_string())
+        except smtplib.SMTPException as error:
+            logging.error(f"Failed to send mail to {recipient}: {error}")
+            raise
```

### Comparing `PyCourrier-0.1.5/PyCourrier.egg-info/PKG-INFO` & `PyCourrier-0.1.6/PyCourrier.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCourrier
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple email sender utility
 Home-page: https://github.com/mjiid/PyCourrier
 Author: Abdelmajid Habouch
 Author-email: Habush1610@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -32,48 +32,56 @@
 ```
 
 ## Usage
 
 Here's a quick guide on how to use MailSender:
 
 ```python
-from PyCourrier import MailSender
+from PyCourrier import MailSender, run
 
-# Create a MailSender instance within a context manager
-with MailSender('your_email@gmail.com', 'your_generated_app_password') as mailSender:
+async def main():
+    # Create a MailSender instance within a context manager
+    with MailSender('your_email@gmail.com', 'your_generated_app_password') as sender:
 
-    # Set recipients
-    recipients = ['recipient1@gmail.com']
-    mailSender.set_recipients(recipients)
-
-    # Set email message details
-    in_subject='Hello from PyCourrier!',
-    in_plaintext='This is the plain text content of the email.',
-    in_from='your_email@gmail.com (optioanl)',
-    in_htmltext='<p>This is the HTML content of the email.</p> (optional)',
-    attachment="path/to/file (optional)",
-    filename="filename_for_the_attachment (optional)"
+        # Set recipients
+        recipients = ['recipient1@gmail.com', 'recipient2@gmail.com', 'recipient3@gmail.com']
+        sender.set_recipients(recipients)
 
-    mailSender.set_message(in_plaintext=plaintext_body, in_subject=in_subject, in_from=in_from, in_htmltext=in_htmltext, attachment=attachment, filename=filename)
+        # Set email message details
+        in_subject='Hello from PyCourrier!'
+        in_plaintext='This is the plain text content of the email.'
+        in_htmltext='<p>This is the HTML content of the email.</p> (optional)'
+
+        # Add attachments (optional)
+        sender.add_attachment('path/to/attachment', 'filename')
+
+        # set the message
+        sender.set_message(in_plaintext=in_plaintext, in_subject=in_subject, in_htmltext=in_htmltext)
+        await sender.send_all_async()
+
+
+# Run the async main function
+if __name__ == "__main__":
+    run(main())
 
-    # Send the email to all recipients
-    mailSender.send_all()
 ```
 
-## Constructor Parameters
+## Parameters:
 - **in_username**: Your email address used for SMTP login.
-- **in_password**: Your Generated app password.
+- **in_password**: Your generated app password for SMTP login.
 - **in_server**: Tuple containing the SMTP server address and port (default is Gmail).
 - **use_SSL**: Boolean indicating whether to use SSL (True) or TLS (False, default) for the connection.
-Methods
-- **set_message**: Compose the email message with subject, plaintext, HTML content, and optional attachments.
+
+## Methods:
+- **set_message**: Compose the email message with subject, plaintext, and HTML content.
+- **add_attachment**: Add an attachment to the email.
 - **set_recipients**: Set the list of email recipients.
-- **add_recipient**: Add a single recipient to the list of recipients.
 - **connect**: Connect to the SMTP server.
 - **disconnect**: Disconnect from the SMTP server.
-- **send_all**: Send the composed email to all recipients.
+- **send_all_async**: Send the composed email to all recipients asynchronously.
+- **send_email**: Send the composed email to a specific recipient.
 
 ## Contribution
 Contributions to PyCourrier are welcome! If you encounter any issues or have suggestions for improvements, please open an [issue on GitHub](https://github.com/mjiid/PyCourrier/issues).
 
 ## License
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `PyCourrier-0.1.5/README.md` & `PyCourrier-0.1.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -18,48 +18,56 @@
 ```
 
 ## Usage
 
 Here's a quick guide on how to use MailSender:
 
 ```python
-from PyCourrier import MailSender
+from PyCourrier import MailSender, run
 
-# Create a MailSender instance within a context manager
-with MailSender('your_email@gmail.com', 'your_generated_app_password') as mailSender:
+async def main():
+    # Create a MailSender instance within a context manager
+    with MailSender('your_email@gmail.com', 'your_generated_app_password') as sender:
 
-    # Set recipients
-    recipients = ['recipient1@gmail.com']
-    mailSender.set_recipients(recipients)
-
-    # Set email message details
-    in_subject='Hello from PyCourrier!',
-    in_plaintext='This is the plain text content of the email.',
-    in_from='your_email@gmail.com (optioanl)',
-    in_htmltext='<p>This is the HTML content of the email.</p> (optional)',
-    attachment="path/to/file (optional)",
-    filename="filename_for_the_attachment (optional)"
+        # Set recipients
+        recipients = ['recipient1@gmail.com', 'recipient2@gmail.com', 'recipient3@gmail.com']
+        sender.set_recipients(recipients)
 
-    mailSender.set_message(in_plaintext=plaintext_body, in_subject=in_subject, in_from=in_from, in_htmltext=in_htmltext, attachment=attachment, filename=filename)
+        # Set email message details
+        in_subject='Hello from PyCourrier!'
+        in_plaintext='This is the plain text content of the email.'
+        in_htmltext='<p>This is the HTML content of the email.</p> (optional)'
+
+        # Add attachments (optional)
+        sender.add_attachment('path/to/attachment', 'filename')
+
+        # set the message
+        sender.set_message(in_plaintext=in_plaintext, in_subject=in_subject, in_htmltext=in_htmltext)
+        await sender.send_all_async()
+
+
+# Run the async main function
+if __name__ == "__main__":
+    run(main())
 
-    # Send the email to all recipients
-    mailSender.send_all()
 ```
 
-## Constructor Parameters
+## Parameters:
 - **in_username**: Your email address used for SMTP login.
-- **in_password**: Your Generated app password.
+- **in_password**: Your generated app password for SMTP login.
 - **in_server**: Tuple containing the SMTP server address and port (default is Gmail).
 - **use_SSL**: Boolean indicating whether to use SSL (True) or TLS (False, default) for the connection.
-Methods
-- **set_message**: Compose the email message with subject, plaintext, HTML content, and optional attachments.
+
+## Methods:
+- **set_message**: Compose the email message with subject, plaintext, and HTML content.
+- **add_attachment**: Add an attachment to the email.
 - **set_recipients**: Set the list of email recipients.
-- **add_recipient**: Add a single recipient to the list of recipients.
 - **connect**: Connect to the SMTP server.
 - **disconnect**: Disconnect from the SMTP server.
-- **send_all**: Send the composed email to all recipients.
+- **send_all_async**: Send the composed email to all recipients asynchronously.
+- **send_email**: Send the composed email to a specific recipient.
 
 ## Contribution
 Contributions to PyCourrier are welcome! If you encounter any issues or have suggestions for improvements, please open an [issue on GitHub](https://github.com/mjiid/PyCourrier/issues).
 
 ## License
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `PyCourrier-0.1.5/setup.py` & `PyCourrier-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name='PyCourrier',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(),
     description='A simple email sender utility',
     author='Abdelmajid Habouch',
     author_email='Habush1610@gmail.com',
     url='https://github.com/mjiid/PyCourrier',
     license='MIT',
     install_requires=[
```

