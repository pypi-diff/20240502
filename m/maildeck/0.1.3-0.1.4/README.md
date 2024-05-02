# Comparing `tmp/maildeck-0.1.3.tar.gz` & `tmp/maildeck-0.1.4.tar.gz`

## Comparing `maildeck-0.1.3.tar` & `maildeck-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 maildeck-0.1.3/.python-version
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 maildeck-0.1.3/requirements-dev.lock
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 maildeck-0.1.3/requirements.lock
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 maildeck-0.1.3/src/maildeck/__init__.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 maildeck-0.1.3/src/maildeck/__main__.py
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 maildeck-0.1.3/src/maildeck/config.py
--rw-r--r--   0        0        0     4226 2020-02-02 00:00:00.000000 maildeck-0.1.3/src/maildeck/deck.py
--rw-r--r--   0        0        0     4087 2020-02-02 00:00:00.000000 maildeck-0.1.3/src/maildeck/imap.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 maildeck-0.1.3/src/maildeck/maildeck.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 maildeck-0.1.3/.gitignore
--rw-r--r--   0        0        0    13792 2020-02-02 00:00:00.000000 maildeck-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 maildeck-0.1.3/README.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 maildeck-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 maildeck-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 maildeck-0.1.4/.python-version
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 maildeck-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 maildeck-0.1.4/requirements-dev.lock
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 maildeck-0.1.4/requirements.lock
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 maildeck-0.1.4/src/maildeck/__init__.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 maildeck-0.1.4/src/maildeck/__main__.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 maildeck-0.1.4/src/maildeck/config.py
+-rw-r--r--   0        0        0     4226 2020-02-02 00:00:00.000000 maildeck-0.1.4/src/maildeck/deck.py
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 maildeck-0.1.4/src/maildeck/imap.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 maildeck-0.1.4/src/maildeck/maildeck.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 maildeck-0.1.4/.gitignore
+-rw-r--r--   0        0        0    13792 2020-02-02 00:00:00.000000 maildeck-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 maildeck-0.1.4/README.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 maildeck-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 maildeck-0.1.4/PKG-INFO
```

### Comparing `maildeck-0.1.3/src/maildeck/__init__.py` & `maildeck-0.1.4/src/maildeck/__init__.py`

 * *Files identical despite different names*

### Comparing `maildeck-0.1.3/src/maildeck/config.py` & `maildeck-0.1.4/src/maildeck/config.py`

 * *Files identical despite different names*

### Comparing `maildeck-0.1.3/src/maildeck/deck.py` & `maildeck-0.1.4/src/maildeck/deck.py`

 * *Files identical despite different names*

### Comparing `maildeck-0.1.3/src/maildeck/imap.py` & `maildeck-0.1.4/src/maildeck/imap.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,20 @@
     def __init__(self, id: str, mailbox: str, data: bytes):
         self.id = id
         self.mailbox = mailbox
         self.message = email.message_from_bytes(data)
 
     @property
     def subject(self) -> str:
-        return decode_header(self.message["Subject"])[0][0].decode("utf-8")
+        decoded_header = decode_header(self.message["Subject"])[0]
+        header_content, encoding = decoded_header[0], decoded_header[1]
+        if isinstance(header_content, bytes):
+            return header_content.decode(encoding if encoding else "utf-8")
+        else:
+            return header_content
 
     @property
     def body(self) -> str:
         if self.message.is_multipart():
             for part in self.message.walk():
                 content_type = part.get_content_type()
                 if content_type != "text/plain":
```

### Comparing `maildeck-0.1.3/src/maildeck/maildeck.py` & `maildeck-0.1.4/src/maildeck/maildeck.py`

 * *Files identical despite different names*

### Comparing `maildeck-0.1.3/LICENSE.txt` & `maildeck-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maildeck-0.1.3/README.md` & `maildeck-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `maildeck-0.1.3/pyproject.toml` & `maildeck-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "maildeck"
-version = "0.1.3"
+version = "0.1.4"
 description = "Import emails into Nextcloud Deck"
 authors = [
     { name = "Mathis Wiehl (@fahrradflucht)", email = "mail-pypi@mathiswiehl.de" }
 ]
 dependencies = []
 readme = "README.md"
 requires-python = ">= 3.10"
```

### Comparing `maildeck-0.1.3/PKG-INFO` & `maildeck-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: maildeck
-Version: 0.1.3
+Version: 0.1.4
 Summary: Import emails into Nextcloud Deck
 Author-email: "Mathis Wiehl (@fahrradflucht)" <mail-pypi@mathiswiehl.de>
 License: EUPL-1.2
 License-File: LICENSE.txt
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

