# Comparing `tmp/pywa-1.8.0.tar.gz` & `tmp/pywa-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywa-1.8.0.tar", last modified: Thu Oct 19 22:48:18 2023, max compression
+gzip compressed data, was "pywa-1.9.0.tar", last modified: Wed Oct 25 18:32:23 2023, max compression
```

## Comparing `pywa-1.8.0.tar` & `pywa-1.9.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:48:18.870441 pywa-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-10-19 22:48:04.000000 pywa-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2023-10-19 22:48:18.866440 pywa-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2023-10-19 22:48:04.000000 pywa-1.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2023-10-19 22:48:04.000000 pywa-1.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:48:18.862440 pywa-1.8.0/pywa/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-10-19 22:48:04.000000 pywa-1.8.0/pywa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21154 2023-10-19 22:48:04.000000 pywa-1.8.0/pywa/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    52070 2023-10-19 22:48:04.000000 pywa-1.8.0/pywa/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9008 2023-10-19 22:48:04.000000 pywa-1.8.0/pywa/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    26375 2023-10-19 22:48:04.000000 pywa-1.8.0/pywa/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    24915 2023-10-19 22:48:04.000000 pywa-1.8.0/pywa/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:48:18.866440 pywa-1.8.0/pywa/types/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2023-10-19 22:48:04.000000 pywa-1.8.0/pywa/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25209 2023-10-19 22:48:04.000000 pywa-1.8.0/pywa/types/base_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    18910 2023-10-19 22:48:04.000000 pywa-1.8.0/pywa/types/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2023-10-19 22:48:04.000000 pywa-1.8.0/pywa/types/media.py
--rw-r--r--   0 runner    (1001) docker     (127)    13493 2023-10-19 22:48:04.000000 pywa-1.8.0/pywa/types/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2023-10-19 22:48:04.000000 pywa-1.8.0/pywa/types/message_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    17794 2023-10-19 22:48:04.000000 pywa-1.8.0/pywa/types/others.py
--rw-r--r--   0 runner    (1001) docker     (127)    45583 2023-10-19 22:48:04.000000 pywa-1.8.0/pywa/types/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2023-10-19 22:48:04.000000 pywa-1.8.0/pywa/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7136 2023-10-19 22:48:04.000000 pywa-1.8.0/pywa/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:48:18.866440 pywa-1.8.0/pywa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2023-10-19 22:48:18.000000 pywa-1.8.0/pywa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      526 2023-10-19 22:48:18.000000 pywa-1.8.0/pywa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-19 22:48:18.000000 pywa-1.8.0/pywa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-10-19 22:48:18.000000 pywa-1.8.0/pywa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-19 22:48:18.000000 pywa-1.8.0/pywa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-10-19 22:48:04.000000 pywa-1.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-19 22:48:18.870441 pywa-1.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:48:18.866440 pywa-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2023-10-19 22:48:04.000000 pywa-1.8.0/tests/test_callback_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 18:32:23.955019 pywa-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-10-25 18:32:08.000000 pywa-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7002 2023-10-25 18:32:23.955019 pywa-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2023-10-25 18:32:08.000000 pywa-1.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2023-10-25 18:32:08.000000 pywa-1.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 18:32:23.955019 pywa-1.9.0/pywa/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2023-10-25 18:32:08.000000 pywa-1.9.0/pywa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20803 2023-10-25 18:32:08.000000 pywa-1.9.0/pywa/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53255 2023-10-25 18:32:08.000000 pywa-1.9.0/pywa/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8741 2023-10-25 18:32:08.000000 pywa-1.9.0/pywa/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27116 2023-10-25 18:32:08.000000 pywa-1.9.0/pywa/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26141 2023-10-25 18:32:08.000000 pywa-1.9.0/pywa/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 18:32:23.955019 pywa-1.9.0/pywa/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2023-10-25 18:32:08.000000 pywa-1.9.0/pywa/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26617 2023-10-25 18:32:08.000000 pywa-1.9.0/pywa/types/base_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19338 2023-10-25 18:32:08.000000 pywa-1.9.0/pywa/types/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2023-10-25 18:32:08.000000 pywa-1.9.0/pywa/types/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13980 2023-10-25 18:32:08.000000 pywa-1.9.0/pywa/types/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2023-10-25 18:32:08.000000 pywa-1.9.0/pywa/types/message_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18549 2023-10-25 18:32:08.000000 pywa-1.9.0/pywa/types/others.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48194 2023-10-25 18:32:08.000000 pywa-1.9.0/pywa/types/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2023-10-25 18:32:08.000000 pywa-1.9.0/pywa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8167 2023-10-25 18:32:08.000000 pywa-1.9.0/pywa/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 18:32:23.955019 pywa-1.9.0/pywa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7002 2023-10-25 18:32:23.000000 pywa-1.9.0/pywa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2023-10-25 18:32:23.000000 pywa-1.9.0/pywa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-25 18:32:23.000000 pywa-1.9.0/pywa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2023-10-25 18:32:23.000000 pywa-1.9.0/pywa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-25 18:32:23.000000 pywa-1.9.0/pywa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-10-25 18:32:08.000000 pywa-1.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-25 18:32:23.955019 pywa-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 18:32:23.955019 pywa-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2023-10-25 18:32:08.000000 pywa-1.9.0/tests/test_callback_data.py
```

### Comparing `pywa-1.8.0/LICENSE` & `pywa-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywa-1.8.0/PKG-INFO` & `pywa-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pywa
-Version: 1.8.0
+Version: 1.9.0
 Summary: Python wrapper for the WhatsApp Cloud API
 Author-email: David Lev <davidlev@telegmail.com>
 License: MIT
 Project-URL: Documentation, https://pywa.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/david-lev/pywa/issues
 Project-URL: Source Code, https://github.com/david-lev/pywa
 Project-URL: Funding, https://github.com/sponsors/david-lev
+Project-URL: Changelog, https://github.com/david-lev/pywa/blob/master/CHANGELOG.md
 Keywords: whatsapp,whatsapp-api,whatsapp-cloud-api,whatsapp-cloud,whatsapp-api-python,whatsapp-cloud-api-python,pywa,wapy,wa,wa-api,wa-cloud-api,wa-cloud,wa-api-python,wa-cloud-api-python,whatsapp-webhook,whatsapp-webhook-python,whatsapp-webhook-api
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Communications
 Classifier: Topic :: Utilities
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pywa-1.8.0/README.rst` & `pywa-1.9.0/README.rst`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -186,8 +186,8 @@
 
 🙏 **Acknowledgments**
 -----------------------
 
 - `Pyrogram <https://pyrogram.org/>`_ - For the design inspiration
 
 
-.. end-readme
+.. end-readme
```

### Comparing `pywa-1.8.0/pyproject.toml` & `pywa-1.9.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -39,7 +39,11 @@
 fastapi = ['fastapi', 'uvicorn[standard]']
 
 [project.urls]
 "Documentation" = "https://pywa.readthedocs.io/"
 "Issue Tracker" = "https://github.com/david-lev/pywa/issues"
 "Source Code" = "https://github.com/david-lev/pywa"
 "Funding" = "https://github.com/sponsors/david-lev"
+"Changelog" = "https://github.com/david-lev/pywa/blob/master/CHANGELOG.md"
+
+[tool.ruff.lint]
+ignore = ["E731", "F401", "E402"]
```

### Comparing `pywa-1.8.0/pywa/api.py` & `pywa-1.9.0/pywa/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 """The internal API for the WhatsApp client."""
 
+from typing import Any, BinaryIO
+
 import requests
 import requests_toolbelt
-from typing import BinaryIO, Any
+
 from pywa.errors import WhatsAppError
 
 
 class WhatsAppCloudApi:
     """Internal methods for the WhatsApp client."""
 
     def __init__(
-            self,
-            phone_id: str,
-            token: str,
-            session: requests.Session,
-            base_url: str,
-            api_version: float,
+        self,
+        phone_id: str,
+        token: str,
+        session: requests.Session,
+        base_url: str,
+        api_version: float,
     ):
         self.phone_id = phone_id
         if session.headers.get("Authorization") is not None:
-            raise ValueError("You can't use the same requests.Session for multiple WhatsApp instances!")
+            raise ValueError(
+                "You can't use the same requests.Session for multiple WhatsApp instances!"
+            )
         self._session = session
         self._base_url = f"{base_url}/v{api_version}"
         self._session.headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {token}",
         }
         self._common_keys = {
@@ -33,37 +37,34 @@
 
     def __str__(self) -> str:
         return f"WhatsAppCloudApi(phone_id={self.phone_id!r})"
 
     def __repr__(self) -> str:
         return self.__str__()
 
-    def _make_request(
-            self,
-            method: str,
-            endpoint: str,
-            **kwargs
-    ) -> dict | list:
+    def _make_request(self, method: str, endpoint: str, **kwargs) -> dict | list:
         """
-        Internal method to make a request to the WhatsApp API.
+        Internal method to make a request to the WhatsApp Cloud API.
 
         Args:
             method: The HTTP method to use.
             endpoint: The endpoint to request.
             **kwargs: Additional arguments to pass to the request.
 
         Returns:
             The response JSON.
 
         Raises:
             WhatsAppError: If the request failed.
         """
-        res = self._session.request(method=method, url=f"{self._base_url}{endpoint}", **kwargs)
+        res = self._session.request(
+            method=method, url=f"{self._base_url}{endpoint}", **kwargs
+        )
         if res.status_code >= 400:
-            raise WhatsAppError.from_response(status_code=res.status_code, error=res.json()["error"])
+            raise WhatsAppError.from_dict(error=res.json()["error"], response=res)
         return res.json()
 
     def get_app_access_token(self, app_id: int, app_secret: str) -> dict[str, str]:
         """
         Get an access token for an app.
 
         Return example::
@@ -84,25 +85,25 @@
         """
         return self._make_request(
             method="GET",
             endpoint="/oauth/access_token",
             params={
                 "grant_type": "client_credentials",
                 "client_id": app_id,
-                "client_secret": app_secret
-            }
+                "client_secret": app_secret,
+            },
         )
 
     def set_callback_url(
-            self,
-            app_id: int,
-            app_access_token: str,
-            callback_url: str,
-            verify_token: str,
-            fields: tuple[str, ...],
+        self,
+        app_id: int,
+        app_access_token: str,
+        callback_url: str,
+        verify_token: str,
+        fields: tuple[str, ...],
     ) -> dict[str, bool]:
         """
         Set the callback URL for the webhook.
 
         Return example::
 
             {
@@ -123,24 +124,24 @@
             method="POST",
             endpoint=f"/{app_id}/subscriptions",
             params={
                 "object": "whatsapp_business_account",
                 "callback_url": callback_url,
                 "verify_token": verify_token,
                 "fields": ",".join(fields),
-                "access_token": app_access_token
-            }
+                "access_token": app_access_token,
+            },
         )
 
     def send_text_message(
-            self,
-            to: str,
-            text: str,
-            preview_url: bool = False,
-            reply_to_message_id: str | None = None,
+        self,
+        to: str,
+        text: str,
+        preview_url: bool = False,
+        reply_to_message_id: str | None = None,
     ) -> dict[str, dict | list]:
         """
         Send a text message to a WhatsApp user.
 
         Return example::
 
             {
@@ -158,33 +159,30 @@
         Returns:
             The sent message.
         """
         data = {
             **self._common_keys,
             "to": to,
             "type": "text",
-            "text": {
-                "body": text,
-                "preview_url": preview_url
-            },
+            "text": {"body": text, "preview_url": preview_url},
         }
         if reply_to_message_id:
             data["context"] = {"message_id": reply_to_message_id}
 
         return self._make_request(
             method="POST",
             endpoint=f"/{self.phone_id}/messages",
-            json=data
+            json=data,
         )
 
     def upload_media(
-            self,
-            media: bytes | BinaryIO,
-            mime_type: str,
-            filename: str,
+        self,
+        media: bytes | BinaryIO,
+        mime_type: str,
+        filename: str,
     ) -> dict[str, str]:
         """
         Upload a media file to WhatsApp.
 
         Return example::
 
             {
@@ -197,29 +195,25 @@
             filename: The name of the media file
         Returns:
             A dict with the ID of the uploaded media file.
         """
         headers = self._session.headers.copy()
         form_data = requests_toolbelt.MultipartEncoder(
             {
-                "file": (
-                    filename,
-                    media,
-                    mime_type
-                ),
+                "file": (filename, media, mime_type),
                 "messaging_product": "whatsapp",
-                "type": mime_type
+                "type": mime_type,
             }
         )
         headers["Content-Type"] = form_data.content_type
         return self._make_request(
             method="POST",
             endpoint=f"/{self.phone_id}/media",
             headers=headers,
-            data=form_data
+            data=form_data,
         )
 
     def get_media_url(self, media_id: str) -> dict:
         """
         Get the URL of a media file.
             - The url is valid for 5 minutes and can be downloaded only with access token.
             - For more info: https://developers.facebook.com/docs/whatsapp/cloud-api/reference/media#retrieve-media-url
@@ -237,22 +231,19 @@
 
         Args:
             media_id: The ID of the media file.
 
         Returns:
             A dict with the URL and other info about the media file.
         """
-        return self._make_request(
-            method="GET",
-            endpoint=f"/{media_id}"
-        )
+        return self._make_request(method="GET", endpoint=f"/{media_id}")
 
     def get_media_bytes(
-            self,
-            media_url: str,
+        self,
+        media_url: str,
     ) -> tuple[bytes, str | None]:
         """
         Get the bytes of a media file from WhatsApp servers.
 
         Args:
             media_url: The URL of the media file (from ``get_media_url``).
 
@@ -275,27 +266,24 @@
 
         Args:
             media_id: The ID of the media file.
 
         Returns:
             True if the media file was deleted successfully, False otherwise.
         """
-        return self._make_request(
-            method="DELETE",
-            endpoint=f"/{media_id}"
-        )
+        return self._make_request(method="DELETE", endpoint=f"/{media_id}")
 
     def send_media(
-            self,
-            to: str,
-            media_id_or_url: str,
-            media_type: str,
-            is_url: bool,
-            caption: str | None = None,
-            filename: str | None = None,
+        self,
+        to: str,
+        media_id_or_url: str,
+        media_type: str,
+        is_url: bool,
+        caption: str | None = None,
+        filename: str | None = None,
     ) -> dict[str, dict | list]:
         """
         Send a media file to a WhatsApp user.
 
         Return example::
 
             {
@@ -318,28 +306,28 @@
         data = {
             **self._common_keys,
             "to": to,
             "type": media_type,
             media_type: {
                 ("link" if is_url else "id"): media_id_or_url,
                 **({"caption": caption} if caption else {}),
-                **({"filename": filename} if filename else {})
-            }
+                **({"filename": filename} if filename else {}),
+            },
         }
         return self._make_request(
             method="POST",
             endpoint=f"/{self.phone_id}/messages",
-            json=data
+            json=data,
         )
 
     def send_reaction(
-            self,
-            to: str,
-            emoji: str,
-            message_id: str,
+        self,
+        to: str,
+        emoji: str,
+        message_id: str,
     ) -> dict[str, dict | list]:
         """
         Send a reaction to a message.
 
         Return example::
 
             {
@@ -359,28 +347,25 @@
         return self._make_request(
             method="POST",
             endpoint=f"/{self.phone_id}/messages/",
             json={
                 **self._common_keys,
                 "to": to,
                 "type": "reaction",
-                "reaction": {
-                    "emoji": emoji,
-                    "message_id": message_id
-                }
-            }
+                "reaction": {"emoji": emoji, "message_id": message_id},
+            },
         )
 
     def send_location(
-            self,
-            to: str,
-            latitude: float,
-            longitude: float,
-            name: str | None = None,
-            address: str | None = None,
+        self,
+        to: str,
+        latitude: float,
+        longitude: float,
+        name: str | None = None,
+        address: str | None = None,
     ) -> dict[str, dict | list]:
         """
         Send a location to a WhatsApp user.
 
         Return example::
 
             {
@@ -403,30 +388,25 @@
             **self._common_keys,
             "to": to,
             "type": "location",
             "location": {
                 "latitude": latitude,
                 "longitude": longitude,
                 "name": name,
-                "address": address
-            }
+                "address": address,
+            },
         }
 
         return self._make_request(
             method="POST",
             endpoint=f"/{self.phone_id}/messages",
-            json=data
+            json=data,
         )
 
-    def send_raw_request(
-            self,
-            method: str,
-            endpoint: str,
-            **kwargs
-    ) -> Any:
+    def send_raw_request(self, method: str, endpoint: str, **kwargs) -> Any:
         """
         Send a raw JSON message to a WhatsApp Cloud API.
 
         - The endpoint can contain path parameters (e.g. ``/v1/messages/{phone_id}``). only ``phone_id`` is supported.
         - Every request will automatically include the ``Authorization`` and ``Content-Type`` headers. you can override
             them by passing them in ``kwargs`` (headers={...}).
 
@@ -437,26 +417,26 @@
 
         Returns:
             The response from the WhatsApp Cloud API.
         """
         return self._make_request(
             method=method,
             endpoint=endpoint.format(phone_id=self.phone_id),
-            **kwargs
+            **kwargs,
         )
 
     def send_interactive_message(
-            self,
-            to: str,
-            type_: str,
-            action: dict[str, Any],
-            header: dict | None = None,
-            body: str | None = None,
-            footer: str | None = None,
-            reply_to_message_id: str | None = None,
+        self,
+        to: str,
+        type_: str,
+        action: dict[str, Any],
+        header: dict | None = None,
+        body: str | None = None,
+        footer: str | None = None,
+        reply_to_message_id: str | None = None,
     ) -> dict[str, dict | list]:
         """
         Send an interactive message to a WhatsApp user.
 
         Return example::
 
             {
@@ -487,23 +467,27 @@
                 "interactive": {
                     "type": type_,
                     "action": action,
                     **({"header": header} if header else {}),
                     **({"body": {"text": body}} if body else {}),
                     **({"footer": {"text": footer}} if footer else {}),
                 },
-                **({"context": {"message_id": reply_to_message_id}} if reply_to_message_id else {}),
-            }
+                **(
+                    {"context": {"message_id": reply_to_message_id}}
+                    if reply_to_message_id
+                    else {}
+                ),
+            },
         )
 
     def send_contacts(
-            self,
-            to: str,
-            contacts: tuple[dict[str, Any]],
-            reply_to_message_id: str | None = None,
+        self,
+        to: str,
+        contacts: tuple[dict[str, Any]],
+        reply_to_message_id: str | None = None,
     ) -> dict[str, dict | list]:
         """
         Send a list of contacts to a WhatsApp user.
 
         Return example::
 
             {
@@ -520,28 +504,25 @@
         Returns:
             The sent message.
         """
         data = {
             **self._common_keys,
             "to": to,
             "type": "contacts",
-            "contacts": tuple(contacts)
+            "contacts": tuple(contacts),
         }
         if reply_to_message_id:
             data["context"] = {"message_id": reply_to_message_id}
         return self._make_request(
             method="POST",
             endpoint=f"/{self.phone_id}/messages",
-            json=data
+            json=data,
         )
 
-    def mark_message_as_read(
-            self,
-            message_id: str
-    ) -> dict[str, bool]:
+    def mark_message_as_read(self, message_id: str) -> dict[str, bool]:
         """
         Mark a message as read.
 
         Return example::
 
             {
                 'success': True
@@ -555,19 +536,21 @@
         """
         return self._make_request(
             method="POST",
             endpoint=f"/{self.phone_id}/messages",
             json={
                 "messaging_product": "whatsapp",
                 "status": "read",
-                "message_id": message_id
-            }
+                "message_id": message_id,
+            },
         )
 
-    def get_business_profile(self) -> dict[str, list[dict[str, str | list[str]]]]:
+    def get_business_profile(
+        self,
+    ) -> dict[str, list[dict[str, str | list[str]]]]:
         """
         Get the business profile.
 
         Return example::
 
             {
               "data": [{
@@ -581,21 +564,31 @@
                    "https://WEBSITE-1",
                    "https://WEBSITE-2"
                  ],
                 "vertical": "INDUSTRY",
               }]
             }
         """
-        fields = ('about', 'address', 'description', 'email', 'profile_picture_url', 'websites', 'vertical')
+        fields = (
+            "about",
+            "address",
+            "description",
+            "email",
+            "profile_picture_url",
+            "websites",
+            "vertical",
+        )
         return self._make_request(
             method="GET",
-            endpoint=f"/{self.phone_id}/whatsapp_business_profile?fields={','.join(fields)}"
+            endpoint=f"/{self.phone_id}/whatsapp_business_profile?fields={','.join(fields)}",
         )
 
-    def update_business_profile(self, data: dict[str, str | list[str]]) -> dict[str, bool]:
+    def update_business_profile(
+        self, data: dict[str, str | list[str]]
+    ) -> dict[str, bool]:
         """
         Update the business profile.
 
         Args:
             data: The data to update the business profile with.
 
         Return example::
@@ -604,15 +597,15 @@
                 "success": True
             }
         """
         data.update(messaging_product="whatsapp")
         return self._make_request(
             method="POST",
             endpoint=f"/{self.phone_id}/whatsapp_business_profile",
-            json=data
+            json=data,
         )
 
     def get_commerce_settings(self) -> dict[str, list[dict]]:
         """
         Get the commerce settings of the business catalog.
 
         Return example::
@@ -625,15 +618,15 @@
                   "id": "727705352028726"
                 }
               ]
             }
         """
         return self._make_request(
             method="GET",
-            endpoint=f"/{self.phone_id}/whatsapp_commerce_settings"
+            endpoint=f"/{self.phone_id}/whatsapp_commerce_settings",
         )
 
     def update_commerce_settings(self, data: dict) -> dict[str, bool]:
         """
         Change the commerce settings of the business catalog.
 
         Args:
@@ -644,21 +637,21 @@
             {
               "success": True
             }
         """
         return self._make_request(
             method="POST",
             endpoint=f"/{self.phone_id}/whatsapp_commerce_settings",
-            params=data
+            params=data,
         )
 
     def create_template(
-            self,
-            business_account_id: str,
-            template: dict[str, str | list[str]]
+        self,
+        business_account_id: str,
+        template: dict[str, str | list[str]],
     ) -> dict[str, str]:
         """
         Create a message template.
 
         Args:
             business_account_id: The ID of the business account.
             template: The template to create.
@@ -670,22 +663,22 @@
                 "status": "PENDING",
                 "category": "MARKETING"
             }
         """
         return self._make_request(
             method="POST",
             endpoint=f"/{business_account_id}/message_templates",
-            json=template
+            json=template,
         )
 
     def send_template(
-            self,
-            to: str,
-            template: dict,
-            reply_to_message_id: str | None = None
+        self,
+        to: str,
+        template: dict,
+        reply_to_message_id: str | None = None,
     ) -> dict[str, dict | list]:
         """
         Send a template to a WhatsApp user.
 
         Args:
             to: The WhatsApp ID of the recipient.
             template: The template to send.
@@ -700,16 +693,16 @@
             }
 
         """
         data = {
             **self._common_keys,
             "to": to,
             "type": "template",
-            "template": template
+            "template": template,
         }
         if reply_to_message_id:
             data["context"] = {"message_id": reply_to_message_id}
         return self._make_request(
             method="POST",
             endpoint=f"/{self.phone_id}/messages",
-            json=data
+            json=data,
         )
```

### Comparing `pywa-1.8.0/pywa/client.py` & `pywa-1.9.0/pywa/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,48 +3,60 @@
 from __future__ import annotations
 
 __all__ = ["WhatsApp"]
 
 import hashlib
 import mimetypes
 import os
+import warnings
+from typing import BinaryIO, Iterable
+
 import requests
-from typing import Iterable, BinaryIO
+
 from pywa.api import WhatsAppCloudApi
 from pywa.handlers import Handler, HandlerDecorators  # noqa
 from pywa.types import (
-    Button, SectionList, Message, Contact, MediaUrlResponse,
-    ProductsSection, BusinessProfile, Industry, CommerceSettings, NewTemplate, Template, TemplateResponse, ButtonUrl
+    BusinessProfile,
+    Button,
+    ButtonUrl,
+    CommerceSettings,
+    Contact,
+    Industry,
+    MediaUrlResponse,
+    Message,
+    NewTemplate,
+    ProductsSection,
+    SectionList,
+    Template,
+    TemplateResponse,
 )
-from pywa.utils import Flask, FastAPI
+from pywa.utils import FastAPI, Flask
 from pywa.webhook import Webhook
 
 _MISSING = object()
 
 
 class WhatsApp(Webhook, HandlerDecorators):
-
-    # noinspection PyMissingConstructor
     def __init__(
-            self,
-            phone_id: str | int,
-            token: str,
-            base_url: str = 'https://graph.facebook.com',
-            api_version: float | int = 18.0,
-            session: requests.Session | None = None,
-            server: Flask | FastAPI | None = None,
-            webhook_endpoint: str = '/',
-            verify_token: str | None = None,
-            filter_updates: bool = True,
-            business_account_id: str | int | None = None,
-            callback_url: str | None = None,
-            fields: Iterable[str] | None = None,
-            app_id: int | None = None,
-            app_secret: str | None = None,
-            verify_timeout: int | None = None,
+        self,
+        phone_id: str | int,
+        token: str,
+        base_url: str = "https://graph.facebook.com",
+        api_version: float | int = 18.0,
+        session: requests.Session | None = None,
+        server: Flask | FastAPI | None = None,
+        webhook_endpoint: str = "/",
+        verify_token: str | None = None,
+        filter_updates: bool = True,
+        business_account_id: str | int | None = None,
+        callback_url: str | None = None,
+        fields: Iterable[str] | None = None,
+        app_id: int | None = None,
+        app_secret: str | None = None,
+        verify_timeout: int | None = None,
     ) -> None:
         """
         The WhatsApp client.
             - Full documentation on `pywa.readthedocs.io <https://pywa.readthedocs.io>`_.
 
         Example without webhook:
 
@@ -96,15 +108,17 @@
             filter_updates: Whether to filter out user updates that are not sent to this phone_id (default: ``True``, does
              not apply to raw updates or updates that are not user-related).
             business_account_id: The business account ID that owns the app (optional, required for some API
              methods).
         """
         self.phone_id = str(phone_id)
         self.filter_updates = filter_updates
-        self.business_account_id = str(business_account_id) if business_account_id is not None else None
+        self.business_account_id = (
+            str(business_account_id) if business_account_id is not None else None
+        )
         self.api = WhatsAppCloudApi(
             phone_id=self.phone_id,
             token=token,
             session=session or requests.Session(),
             base_url=base_url,
             api_version=float(api_version),
         )
@@ -138,28 +152,31 @@
             >>> wa = WhatsApp(...)
             >>> wa.add_handlers(
             ...     MessageHandler(print_message, fil.text),
             ...     CallbackButtonHandler(print_message),
             ... )
         """
         if self._handlers is None:
-            raise ValueError("You must initialize the WhatsApp client with an web server"
-                             " (Flask or FastAPI) in order to handle incoming updates.")
+            raise ValueError(
+                "You must initialize the WhatsApp client with an web server"
+                " (Flask or FastAPI) in order to handle incoming updates."
+            )
         for handler in handlers:
             self._handlers[handler.__class__].append(handler)
 
     def send_message(
-            self,
-            to: str | int,
-            text: str,
-            header: str | None = None,
-            footer: str | None = None,
-            keyboard: Iterable[Button] | ButtonUrl | SectionList | None = None,
-            preview_url: bool = False,
-            reply_to_message_id: str | None = None,
+        self,
+        to: str | int,
+        text: str,
+        header: str | None = None,
+        footer: str | None = None,
+        buttons: Iterable[Button] | ButtonUrl | SectionList | None = None,
+        preview_url: bool = False,
+        reply_to_message_id: str | None = None,
+        keyboard: None = None,
     ) -> str:
         """
         Send a message to a WhatsApp user.
 
         Example:
 
             >>> wa = WhatsApp(...)
@@ -174,29 +191,29 @@
             >>> from pywa.types import Button
             >>> wa = WhatsApp(...)
             >>> wa.send_message(
             ...     to="1234567890",
             ...     header="Hello from PyWa!",
             ...     text="What can I help you with?",
             ...     footer="Powered by PyWa",
-            ...     keyboard=[
+            ...     buttons=[
             ...         Button("Help", data="help"),
             ...         Button("About", data="about"),
             ...     ],
             ... )
 
         Example with a section list:
             >>> from pywa.types import SectionList, Section, SectionRow
             >>> wa = WhatsApp(...)
             >>> wa.send_message(
             ...     to="1234567890",
             ...     header="Hello from PyWa!",
             ...     text="What can I help you with?",
             ...     footer="Powered by PyWa",
-            ...     keyboard=SectionList(
+            ...     buttons=SectionList(
             ...         button_title="Choose an option",
             ...         sections=[
             ...             Section(
             ...                 title="Help",
             ...                 rows=[
             ...                     SectionRow(
             ...                         title="Help",
@@ -228,53 +245,63 @@
         Args:
             to: The phone ID of the WhatsApp user.
             text: The text to send (`markdown <https://faq.whatsapp.com/539178204879377>`_ allowed, max 4096 characters).
             header: The header of the message (if keyboard is provided, optional, up to 60 characters,
              no `markdown <https://faq.whatsapp.com/539178204879377>`_ allowed).
             footer: The footer of the message (if keyboard is provided, optional, up to 60 characters,
              `markdown <https://faq.whatsapp.com/539178204879377>`_ has no effect).
-            keyboard: The keyboard to send with the message (optional).
+            buttons: The buttons to send with the message (optional).
             preview_url: Whether to show a preview of the URL in the message (if any).
             reply_to_message_id: The message ID to reply to (optional).
+            keyboard: Deprecated and will be removed in a future version, use ``buttons`` instead.
 
         Returns:
             The message ID of the sent message.
         """
-        if not keyboard:
+        if keyboard is not None:
+            buttons = keyboard
+            warnings.simplefilter("always", DeprecationWarning)
+            warnings.warn(
+                "The `keyboard` parameter is deprecated and will be removed in a future version, use `buttons` instead.",
+                DeprecationWarning,
+            )
+        if not buttons:
             return self.api.send_text_message(
                 to=str(to),
                 text=text,
                 preview_url=preview_url,
                 reply_to_message_id=reply_to_message_id,
-            )['messages'][0]['id']
-        type_, kb = _resolve_keyboard_param(keyboard)
+            )["messages"][0]["id"]
+        type_, kb = _resolve_keyboard_param(buttons)
         return self.api.send_interactive_message(
             to=str(to),
             type_=type_,
             action=kb,
             header={
                 "type": "text",
                 "text": header,
-            } if header else None,
+            }
+            if header
+            else None,
             body=text,
             footer=footer,
-        )['messages'][0]['id']
+        )["messages"][0]["id"]
 
     send_text = send_message  # alias
 
     def send_image(
-            self,
-            to: str | int,
-            image: str | bytes | BinaryIO,
-            caption: str | None = None,
-            body: str | None = None,
-            footer: str | None = None,
-            buttons: Iterable[Button] | ButtonUrl | None = None,
-            reply_to_message_id: str | None = None,
-            mime_type: str | None = None,
+        self,
+        to: str | int,
+        image: str | bytes | BinaryIO,
+        caption: str | None = None,
+        body: str | None = None,
+        footer: str | None = None,
+        buttons: Iterable[Button] | ButtonUrl | None = None,
+        reply_to_message_id: str | None = None,
+        mime_type: str | None = None,
     ) -> str:
         """
         Send an image to a WhatsApp user.
             - Images must be 8-bit, RGB or RGBA.
 
         Example:
 
@@ -293,57 +320,64 @@
             body: The body of the message (optional, up to 1024 characters,
              `markdown <https://faq.whatsapp.com/539178204879377>`_ allowed, if buttons are provided and body is not
              provided, caption will be used as the body)
             footer: The footer of the message (if buttons is provided, optional,
              `markdown <https://faq.whatsapp.com/539178204879377>`_ has no effect).
             buttons: The buttons to send with the image (optional).
             reply_to_message_id: The message ID to reply to (optional, only works if buttons provided).
-            mime_type: The mime type of the image (optional, required when sending an image as bytes or a file object, 
+            mime_type: The mime type of the image (optional, required when sending an image as bytes or a file object,
              or file path that does not have an extension).
 
         Returns:
             The message ID of the sent image message.
         """
-        is_url, image = _resolve_media_param(wa=self, media=image, mime_type=mime_type, filename="image.jpg")
+        is_url, image = _resolve_media_param(
+            wa=self,
+            media=image,
+            mime_type=mime_type,
+            filename="image.jpg",
+        )
         if not buttons:
             return self.api.send_media(
                 to=str(to),
                 media_id_or_url=image,
                 is_url=is_url,
                 media_type="image",
                 caption=caption,
-            )['messages'][0]['id']
+            )["messages"][0]["id"]
         if not body and not caption:
-            raise ValueError("Either body or caption must be provided when sending an image with buttons.")
+            raise ValueError(
+                "Either body or caption must be provided when sending an image with buttons."
+            )
         type_, kb = _resolve_keyboard_param(buttons)
         return self.api.send_interactive_message(
             to=str(to),
             type_=type_,
             action=kb,
             header={
                 "type": "image",
                 "image": {
                     "link" if is_url else "id": image,
-                }
+                },
             },
             body=body or caption,
             footer=footer,
             reply_to_message_id=reply_to_message_id,
-        )['messages'][0]['id']
+        )["messages"][0]["id"]
 
     def send_video(
-            self,
-            to: str | int,
-            video: str | bytes | BinaryIO,
-            caption: str | None = None,
-            body: str | None = None,
-            footer: str | None = None,
-            buttons: Iterable[Button] | ButtonUrl | None = None,
-            reply_to_message_id: str | None = None,
-            mime_type: str | None = None,
+        self,
+        to: str | int,
+        video: str | bytes | BinaryIO,
+        caption: str | None = None,
+        body: str | None = None,
+        footer: str | None = None,
+        buttons: Iterable[Button] | ButtonUrl | None = None,
+        reply_to_message_id: str | None = None,
+        mime_type: str | None = None,
     ) -> str:
         """
         Send a video to a WhatsApp user.
             - Only H.264 video codec and AAC audio codec is supported.
             - Videos with a single audio stream or no audio stream are supported.
 
         Example:
@@ -369,52 +403,59 @@
             reply_to_message_id: The message ID to reply to (optional, only works if buttons provided).
             mime_type: The mime type of the video (optional, required when sending a video as bytes or a file object,
              or file path that does not have an extension).
 
         Returns:
             The message ID of the sent video.
         """
-        is_url, video = _resolve_media_param(wa=self, media=video, mime_type=mime_type, filename="video.mp4")
+        is_url, video = _resolve_media_param(
+            wa=self,
+            media=video,
+            mime_type=mime_type,
+            filename="video.mp4",
+        )
         if not buttons:
             return self.api.send_media(
                 to=str(to),
                 media_id_or_url=video,
                 is_url=is_url,
                 media_type="video",
                 caption=caption,
-            )['messages'][0]['id']
+            )["messages"][0]["id"]
         if not body and not caption:
-            raise ValueError("Either body or caption must be provided when sending a video with buttons.")
+            raise ValueError(
+                "Either body or caption must be provided when sending a video with buttons."
+            )
         type_, kb = _resolve_keyboard_param(buttons)
         return self.api.send_interactive_message(
             to=str(to),
             type_=type_,
             action=kb,
             header={
                 "type": "video",
                 "video": {
                     "link" if is_url else "id": video,
-                }
+                },
             },
             body=body or caption,
             footer=footer,
             reply_to_message_id=reply_to_message_id,
-        )['messages'][0]['id']
+        )["messages"][0]["id"]
 
     def send_document(
-            self,
-            to: str | int,
-            document: str | bytes | BinaryIO,
-            filename: str | None = None,
-            caption: str | None = None,
-            body: str | None = None,
-            footer: str | None = None,
-            buttons: Iterable[Button] | ButtonUrl | None = None,
-            reply_to_message_id: str | None = None,
-            mime_type: str | None = None,
+        self,
+        to: str | int,
+        document: str | bytes | BinaryIO,
+        filename: str | None = None,
+        caption: str | None = None,
+        body: str | None = None,
+        footer: str | None = None,
+        buttons: Iterable[Button] | ButtonUrl | None = None,
+        reply_to_message_id: str | None = None,
+        mime_type: str | None = None,
     ) -> str:
         """
         Send a document to a WhatsApp user.
 
         Example:
 
             >>> wa = WhatsApp(...)
@@ -442,48 +483,55 @@
             reply_to_message_id: The message ID to reply to (optional, only works if buttons provided).
             mime_type: The mime type of the document (optional, required when sending a document as bytes or a file
              object, or file path that does not have an extension).
 
         Returns:
             The message ID of the sent document.
         """
-        is_url, document = _resolve_media_param(wa=self, media=document, mime_type=mime_type, filename=filename)
+        is_url, document = _resolve_media_param(
+            wa=self,
+            media=document,
+            mime_type=mime_type,
+            filename=filename,
+        )
         if not buttons:
             return self.api.send_media(
                 to=str(to),
                 media_id_or_url=document,
                 is_url=is_url,
                 media_type="document",
                 caption=caption,
                 filename=filename,
-            )['messages'][0]['id']
+            )["messages"][0]["id"]
         if not body and not caption:
-            raise ValueError("Either body or caption must be provided when sending a document with buttons.")
+            raise ValueError(
+                "Either body or caption must be provided when sending a document with buttons."
+            )
         type_, kb = _resolve_keyboard_param(buttons)
         return self.api.send_interactive_message(
             to=str(to),
             type_=type_,
             action=kb,
             header={
                 "type": "document",
                 "document": {
                     "link" if is_url else "id": document,
                     "filename": filename,
-                }
+                },
             },
             body=body or caption,
             footer=footer,
             reply_to_message_id=reply_to_message_id,
-        )['messages'][0]['id']
+        )["messages"][0]["id"]
 
     def send_audio(
-            self,
-            to: str | int,
-            audio: str | bytes | BinaryIO,
-            mime_type: str | None = None,
+        self,
+        to: str | int,
+        audio: str | bytes | BinaryIO,
+        mime_type: str | None = None,
     ) -> str:
         """
         Send an audio file to a WhatsApp user.
 
         Example:
 
             >>> wa = WhatsApp(...)
@@ -497,27 +545,32 @@
             audio: The audio file to send (either a media ID, URL, file path, bytes, or an open file object).
             mime_type: The mime type of the audio file (optional, required when sending an audio file as bytes or a file
              object, or file path that does not have an extension).
 
         Returns:
             The message ID of the sent audio file.
         """
-        is_url, audio = _resolve_media_param(wa=self, media=audio, mime_type=mime_type, filename="audio.mp3")
+        is_url, audio = _resolve_media_param(
+            wa=self,
+            media=audio,
+            mime_type=mime_type,
+            filename="audio.mp3",
+        )
         return self.api.send_media(
             to=str(to),
             media_id_or_url=audio,
             is_url=is_url,
             media_type="audio",
-        )['messages'][0]['id']
+        )["messages"][0]["id"]
 
     def send_sticker(
-            self,
-            to: str | int,
-            sticker: str | bytes | BinaryIO,
-            mime_type: str | None = None,
+        self,
+        to: str | int,
+        sticker: str | bytes | BinaryIO,
+        mime_type: str | None = None,
     ) -> str:
         """
         Send a sticker to a WhatsApp user.
             - A static sticker needs to be 512x512 pixels and cannot exceed 100 KB.
             - An animated sticker must be 512x512 pixels and cannot exceed 500 KB.
 
         Example:
@@ -533,27 +586,32 @@
             sticker: The sticker to send (either a media ID, URL, file path, bytes, or an open file object).
             mime_type: The mime type of the sticker (optional, required when sending a sticker as bytes or a file
              object, or file path that does not have an extension).
 
         Returns:
             The message ID of the sent message.
         """
-        is_url, sticker = _resolve_media_param(wa=self, media=sticker, mime_type=mime_type, filename="sticker.webp")
+        is_url, sticker = _resolve_media_param(
+            wa=self,
+            media=sticker,
+            mime_type=mime_type,
+            filename="sticker.webp",
+        )
         return self.api.send_media(
             to=str(to),
             media_id_or_url=sticker,
             is_url=is_url,
             media_type="sticker",
-        )['messages'][0]['id']
+        )["messages"][0]["id"]
 
     def send_reaction(
-            self,
-            to: str | int,
-            emoji: str,
-            message_id: str,
+        self,
+        to: str | int,
+        emoji: str,
+        message_id: str,
     ) -> str:
         """
         React to a message with an emoji.
             - You can react to incoming messages by using the :py:func:`~pywa.types.base_update.BaseUserUpdate.react` method.
 
         Example:
 
@@ -573,20 +631,20 @@
             The message ID of the reaction (You can't use this message id to remove the reaction or perform any other
             action on it. instead, use the message ID of the message you reacted to).
         """
         return self.api.send_reaction(
             to=str(to),
             emoji=emoji,
             message_id=message_id,
-        )['messages'][0]['id']
+        )["messages"][0]["id"]
 
     def remove_reaction(
-            self,
-            to: str | int,
-            message_id: str,
+        self,
+        to: str | int,
+        message_id: str,
     ) -> str:
         """
         Remove a reaction from a message.
             - You can remove reactions from incoming messages by using the :py:func:`~pywa.types.base_update.BaseUserUpdate.unreact` method.
 
         Example:
 
@@ -596,27 +654,25 @@
             ...     message_id='wamid.XXX='
             ... )
 
         Returns:
             The message ID of the reaction (You can't use this message id to re-react or perform any other action on it.
             instead, use the message ID of the message you unreacted to).
         """
-        return self.api.send_reaction(
-            to=str(to),
-            emoji="",
-            message_id=message_id
-        )['messages'][0]['id']
+        return self.api.send_reaction(to=str(to), emoji="", message_id=message_id)[
+            "messages"
+        ][0]["id"]
 
     def send_location(
-            self,
-            to: str | int,
-            latitude: float,
-            longitude: float,
-            name: str | None = None,
-            address: str | None = None,
+        self,
+        to: str | int,
+        latitude: float,
+        longitude: float,
+        name: str | None = None,
+        address: str | None = None,
     ) -> str:
         """
         Send a location to a WhatsApp user.
 
         Example:
 
             >>> wa = WhatsApp(...)
@@ -640,21 +696,21 @@
         """
         return self.api.send_location(
             to=str(to),
             latitude=latitude,
             longitude=longitude,
             name=name,
             address=address,
-        )['messages'][0]['id']
+        )["messages"][0]["id"]
 
     def send_contact(
-            self,
-            to: str | int,
-            contact: Contact | Iterable[Contact],
-            reply_to_message_id: str | None = None,
+        self,
+        to: str | int,
+        contact: Contact | Iterable[Contact],
+        reply_to_message_id: str | None = None,
     ) -> str:
         """
         Send a contact/s to a WhatsApp user.
 
         Example:
 
             >>> from pywa.types import Contact
@@ -675,25 +731,27 @@
             reply_to_message_id: The message ID to reply to (optional).
 
         Returns:
             The message ID of the sent message.
         """
         return self.api.send_contacts(
             to=str(to),
-            contacts=tuple(c.to_dict() for c in contact) if isinstance(contact, Iterable) else (contact.to_dict()),
+            contacts=tuple(c.to_dict() for c in contact)
+            if isinstance(contact, Iterable)
+            else (contact.to_dict()),
             reply_to_message_id=reply_to_message_id,
-        )['messages'][0]['id']
+        )["messages"][0]["id"]
 
     def send_catalog(
-            self,
-            to: str | int,
-            body: str,
-            footer: str | None = None,
-            thumbnail_product_sku: str | None = None,
-            reply_to_message_id: str | None = None,
+        self,
+        to: str | int,
+        body: str,
+        footer: str | None = None,
+        thumbnail_product_sku: str | None = None,
+        reply_to_message_id: str | None = None,
     ) -> str:
         """
         Send the business catalog to a WhatsApp user.
 
         Example:
 
             >>> wa = WhatsApp(...)
@@ -716,31 +774,37 @@
             The message ID of the sent message.
         """
         return self.api.send_interactive_message(
             to=str(to),
             type_="catalog_message",
             action={
                 "name": "catalog_message",
-                **({"parameters": {
-                    "thumbnail_product_retailer_id": thumbnail_product_sku,
-                }} if thumbnail_product_sku else {}),
+                **(
+                    {
+                        "parameters": {
+                            "thumbnail_product_retailer_id": thumbnail_product_sku,
+                        }
+                    }
+                    if thumbnail_product_sku
+                    else {}
+                ),
             },
             body=body,
             footer=footer,
-            reply_to_message_id=reply_to_message_id
-        )['messages'][0]['id']
+            reply_to_message_id=reply_to_message_id,
+        )["messages"][0]["id"]
 
     def send_product(
-            self,
-            to: str | int,
-            catalog_id: str,
-            sku: str,
-            body: str | None = None,
-            footer: str | None = None,
-            reply_to_message_id: str | None = None,
+        self,
+        to: str | int,
+        catalog_id: str,
+        sku: str,
+        body: str | None = None,
+        footer: str | None = None,
+        reply_to_message_id: str | None = None,
     ) -> str:
         """
         Send a product from a business catalog to a WhatsApp user.
             - To send multiple products, use :py:func:`~pywa.client.WhatsApp.send_products`.
 
         Example:
 
@@ -771,26 +835,26 @@
             type_="product",
             action={
                 "catalog_id": catalog_id,
                 "product_retailer_id": sku,
             },
             body=body,
             footer=footer,
-            reply_to_message_id=reply_to_message_id
-        )['messages'][0]['id']
+            reply_to_message_id=reply_to_message_id,
+        )["messages"][0]["id"]
 
     def send_products(
-            self,
-            to: str | int,
-            catalog_id: str,
-            product_sections: Iterable[ProductsSection],
-            title: str,
-            body: str,
-            footer: str | None = None,
-            reply_to_message_id: str | None = None,
+        self,
+        to: str | int,
+        catalog_id: str,
+        product_sections: Iterable[ProductsSection],
+        title: str,
+        body: str,
+        footer: str | None = None,
+        reply_to_message_id: str | None = None,
     ) -> str:
         """
         Send products from a business catalog to a WhatsApp user.
             - To send a single product, use :py:func:`~pywa.client.WhatsApp.send_product`.
 
         Example:
 
@@ -834,20 +898,20 @@
             action={
                 "catalog_id": catalog_id,
                 "sections": tuple(ps.to_dict() for ps in product_sections),
             },
             header={"type": "text", "text": title},
             body=body,
             footer=footer,
-            reply_to_message_id=reply_to_message_id
-        )['messages'][0]['id']
+            reply_to_message_id=reply_to_message_id,
+        )["messages"][0]["id"]
 
     def mark_message_as_read(
-            self,
-            message_id: str,
+        self,
+        message_id: str,
     ) -> bool:
         """
         Mark a message as read.
             - You can mark incoming messages as read by using the :py:func:`~pywa.types.base_update.BaseUserUpdate.mark_as_read` method.
 
         Example:
 
@@ -856,21 +920,21 @@
 
         Args:
             message_id: The message ID to mark as read.
 
         Returns:
             Whether the message was marked as read.
         """
-        return self.api.mark_message_as_read(message_id=message_id)['success']
+        return self.api.mark_message_as_read(message_id=message_id)["success"]
 
     def upload_media(
-            self,
-            media: str | bytes | BinaryIO,
-            mime_type: str,
-            filename: str | None = None,
+        self,
+        media: str | bytes | BinaryIO,
+        mime_type: str,
+        filename: str | None = None,
     ) -> str:
         """
         Upload media to WhatsApp servers.
 
         Example:
 
             >>> wa = WhatsApp(...)
@@ -889,37 +953,40 @@
 
         Raises:
             ValueError: If the file is not found or the URL is invalid or if the media is bytes and the filename is not
              provided.
         """
         if isinstance(media, str):
             if os.path.isfile(media):
-                file, filename, mime_type = \
-                    open(media, 'rb'), os.path.basename(media), (mimetypes.guess_type(media)[0] or mime_type)
+                file, filename, mime_type = (
+                    open(media, "rb"),
+                    os.path.basename(media),
+                    (mimetypes.guess_type(media)[0] or mime_type),
+                )
             elif media.startswith(("https://", "http://")):
                 res = requests.get(media)
                 res.raise_for_status()
-                file, filename, mime_type = \
-                    res.content, os.path.basename(media) or filename, (res.headers['Content-Type'] or mime_type)
+                file, filename, mime_type = (
+                    res.content,
+                    os.path.basename(media) or filename,
+                    (res.headers["Content-Type"] or mime_type),
+                )
             else:
-                raise ValueError(f'File not found or invalid URL: {media}')
+                raise ValueError(f"File not found or invalid URL: {media}")
         else:
             file = media
             if filename is None:
-                raise ValueError('filename is required if media is bytes')
+                raise ValueError("filename is required if media is bytes")
         return self.api.upload_media(
             filename=filename,
             media=file,
             mime_type=mime_type,
-        )['id']
+        )["id"]
 
-    def get_media_url(
-            self,
-            media_id: str
-    ) -> MediaUrlResponse:
+    def get_media_url(self, media_id: str) -> MediaUrlResponse:
         """
         Get the URL of a media.
             - The URL is valid for 5 minutes.
             - The media can be downloaded directly from the message using the :py:func:`~pywa.types.Message.download_media` method.
 
         Example:
 
@@ -931,27 +998,27 @@
 
         Returns:
             A MediaResponse object with the media URL.
         """
         res = self.api.get_media_url(media_id=media_id)
         return MediaUrlResponse(
             _client=self,
-            id=res['id'],
-            url=res['url'],
-            mime_type=res['mime_type'],
-            sha256=res['sha256'],
-            file_size=res['file_size'],
+            id=res["id"],
+            url=res["url"],
+            mime_type=res["mime_type"],
+            sha256=res["sha256"],
+            file_size=res["file_size"],
         )
 
     def download_media(
-            self,
-            url: str,
-            path: str | None = None,
-            filename: str | None = None,
-            in_memory: bool = False,
+        self,
+        url: str,
+        path: str | None = None,
+        filename: str | None = None,
+        in_memory: bool = False,
     ) -> str | bytes:
         """
         Download a media file from WhatsApp servers.
 
         Example:
 
             >>> wa = WhatsApp(...)
@@ -972,15 +1039,19 @@
         """
         content, mimetype = self.api.get_media_bytes(media_url=url)
         if in_memory:
             return content
         if path is None:
             path = os.getcwd()
         if filename is None:
-            filename = hashlib.sha256(url.encode()).hexdigest() + mimetypes.guess_extension(mimetype) or '.bin'
+            filename = (
+                hashlib.sha256(url.encode()).hexdigest()
+                + mimetypes.guess_extension(mimetype)
+                or ".bin"
+            )
         path = os.path.join(path, filename)
         with open(path, "wb") as f:
             f.write(content)
         return path
 
     def get_business_profile(self) -> BusinessProfile:
         """
@@ -990,25 +1061,27 @@
 
             >>> wa = WhatsApp(...)
             >>> wa.get_business_profile()
 
         Returns:
             The business profile.
         """
-        return BusinessProfile.from_dict(data=self.api.get_business_profile()['data'][0])
+        return BusinessProfile.from_dict(
+            data=self.api.get_business_profile()["data"][0]
+        )
 
     def update_business_profile(
-            self,
-            about: str | None = _MISSING,
-            address: str | None = _MISSING,
-            description: str | None = _MISSING,
-            email: str | None = _MISSING,
-            profile_picture_handle: str | None = _MISSING,
-            industry: Industry | None = _MISSING,
-            websites: Iterable[str] | None = _MISSING
+        self,
+        about: str | None = _MISSING,
+        address: str | None = _MISSING,
+        description: str | None = _MISSING,
+        email: str | None = _MISSING,
+        profile_picture_handle: str | None = _MISSING,
+        industry: Industry | None = _MISSING,
+        websites: Iterable[str] | None = _MISSING,
     ) -> bool:
         """
         Update the business profile of the WhatsApp Business account.
 
         Example:
 
             >>> from pywa.types import Industry
@@ -1039,44 +1112,48 @@
              (You must include the ``http://`` or ``https://`` portion of the URL.
              There is a maximum of 2 websites with a maximum of 256 characters each.)
 
         Returns:
             Whether the business profile was updated.
         """
         data = {
-            key: value or '' for key, value in {
-                'about': about,
-                'address': address,
-                'description': description,
-                'email': email,
-                'profile_picture_handle': profile_picture_handle,
-                'vertical': industry,
-                'websites': websites,
-            }.items() if value is not _MISSING
+            key: value or ""
+            for key, value in {
+                "about": about,
+                "address": address,
+                "description": description,
+                "email": email,
+                "profile_picture_handle": profile_picture_handle,
+                "vertical": industry,
+                "websites": websites,
+            }.items()
+            if value is not _MISSING
         }
-        return self.api.update_business_profile(data)['success']
+        return self.api.update_business_profile(data)["success"]
 
     def get_commerce_settings(self) -> CommerceSettings:
         """
         Get the commerce settings of the WhatsApp Business account.
 
         Example:
 
             >>> wa = WhatsApp(...)
             >>> wa.get_commerce_settings()
 
         Returns:
             The commerce settings.
         """
-        return CommerceSettings.from_dict(data=self.api.get_commerce_settings()['data'][0])
+        return CommerceSettings.from_dict(
+            data=self.api.get_commerce_settings()["data"][0]
+        )
 
     def update_commerce_settings(
-            self,
-            is_catalog_visible: bool = None,
-            is_cart_enabled: bool = None,
+        self,
+        is_catalog_visible: bool = None,
+        is_cart_enabled: bool = None,
     ) -> bool:
         """
         Update the commerce settings of the WhatsApp Business account.
 
         Example:
 
             >>> wa = WhatsApp(...)
@@ -1092,38 +1169,40 @@
         Returns:
             Whether the commerce settings were updated.
 
         Raises:
             ValueError: If no arguments are provided.
         """
         data = {
-            key: value for key, value in {
-                'is_cart_enabled': is_cart_enabled,
-                'is_catalog_visible': is_catalog_visible,
-            }.items() if value is not None
+            key: value
+            for key, value in {
+                "is_cart_enabled": is_cart_enabled,
+                "is_catalog_visible": is_catalog_visible,
+            }.items()
+            if value is not None
         }
         if not data:
-            raise ValueError('At least one argument must be provided')
-        return self.api.update_commerce_settings(data)['success']
+            raise ValueError("At least one argument must be provided")
+        return self.api.update_commerce_settings(data)["success"]
 
     def _validate_business_account_id_provided(self):
         """Internal method to validate that the business account ID was provided."""
         if self.business_account_id is None:
             raise ValueError(
                 "You must provide the business account ID when using this method. "
                 "You can provide it when initializing the client or by setting the business_account_id attribute."
             )
 
     def create_template(
-            self,
-            template: NewTemplate,
-            placeholder: tuple[str, str] | None = None,
+        self,
+        template: NewTemplate,
+        placeholder: tuple[str, str] | None = None,
     ) -> TemplateResponse:
         """
-        `\`Create Templates\` on developers.facebook.com
+        `'Create Templates' on developers.facebook.com
         <https://developers.facebook.com/docs/whatsapp/business-management-api/message-templates>`_.
 
         - To send a template, use :py:func:`~pywa.client.WhatsApp.send_template`.
 
         ATTENTION: In case of an errors, WhatsApp does not return a proper error message, instead, it returns a message
         of `invalid parameter` with error code of 100. You need to pay attention to the following:
 
@@ -1184,24 +1263,26 @@
              <https://developers.facebook.com/docs/whatsapp/business-management-api/message-templates/supported-languages>`_).
             placeholder: The placeholders start & end (optional, default: ``('{', '}')``)).
 
         Returns:
             The template created response. containing the template ID, status and category.
         """
         self._validate_business_account_id_provided()
-        return TemplateResponse(**self.api.create_template(
-            business_account_id=self.business_account_id,
-            template=template.to_dict(placeholder=placeholder)
-        ))
+        return TemplateResponse(
+            **self.api.create_template(
+                business_account_id=self.business_account_id,
+                template=template.to_dict(placeholder=placeholder),
+            )
+        )
 
     def send_template(
-            self,
-            to: str | int,
-            template: Template,
-            reply_to_message_id: str | None = None,
+        self,
+        to: str | int,
+        template: Template,
+        reply_to_message_id: str | None = None,
     ) -> str:
         """
         Send a template to a WhatsApp user.
 
         - To create a template, use :py:func:`~pywa.client.WhatsApp.create_template`.
 
         Example:
@@ -1253,64 +1334,87 @@
         """
         is_url = None
         match type(template.header):
             case Template.TextValue:
                 pass
             case Template.Image:
                 is_url, template.header.image = _resolve_media_param(
-                    wa=self, media=template.header.image, mime_type="image/jpeg", filename="image.jpg"
+                    wa=self,
+                    media=template.header.image,
+                    mime_type="image/jpeg",
+                    filename="image.jpg",
                 )
             case Template.Document:
                 is_url, template.header.document = _resolve_media_param(
-                    wa=self, media=template.header.document, mime_type="text/plain", filename="file.pdf"
+                    wa=self,
+                    media=template.header.document,
+                    mime_type="text/plain",
+                    filename="file.pdf",
                 )
             case Template.Video:
                 is_url, template.header.video = _resolve_media_param(
-                    wa=self, media=template.header.video, mime_type="video/mp4", filename="video.mp4"
+                    wa=self,
+                    media=template.header.video,
+                    mime_type="video/mp4",
+                    filename="video.mp4",
                 )
         return self.api.send_template(
             to=str(to),
             template=template.to_dict(is_header_url=is_url),
             reply_to_message_id=reply_to_message_id,
-        )['messages'][0]['id']
+        )["messages"][0]["id"]
 
 
-def _resolve_keyboard_param(keyboard: Iterable[Button] | ButtonUrl | SectionList) -> tuple[str, dict]:
+def _resolve_keyboard_param(
+    keyboard: Iterable[Button] | ButtonUrl | SectionList,
+) -> tuple[str, dict]:
     """
     Resolve keyboard parameters to a type and an action dict.
     """
     if isinstance(keyboard, SectionList):
         return "list", keyboard.to_dict()
     elif isinstance(keyboard, ButtonUrl):
         return "cta_url", keyboard.to_dict()
     else:
         return "button", {"buttons": tuple(b.to_dict() for b in keyboard)}
 
 
 def _resolve_media_param(
-        wa: WhatsApp,
-        media: str | bytes | BinaryIO,
-        mime_type: str | None,
-        filename: str | None,
+    wa: WhatsApp,
+    media: str | bytes | BinaryIO,
+    mime_type: str | None,
+    filename: str | None,
 ) -> tuple[bool, str]:
     """
     Internal method to resolve media parameters. Returns a tuple of (is_url, media_id_or_url).
     """
     if isinstance(media, str):
         if media.startswith(("https://", "http://")):
             return True, media
         elif not os.path.isfile(media) and media.isdigit():
             return False, media  # assume it's a media ID
         else:  # assume it's a file path
             if not (mt := mimetypes.guess_type(media)[0] or mime_type):
-                raise ValueError(f"Could not determine the mime type of the file {media!r}. Please provide a mime type.")
+                raise ValueError(
+                    f"Could not determine the mime type of the file {media!r}. Please provide a mime type."
+                )
             return False, wa.upload_media(
                 media=media,
                 mime_type=mt,
-                filename=filename or os.path.basename(media)
+                filename=filename or os.path.basename(media),
             )
     else:
         if not mime_type or not filename:
             msg = "When sending media as bytes or a file object a {} must be provided."
-            raise ValueError(msg.format("mime_type and filename" if not mime_type and not filename else
-                                        ("mime_type" if not mime_type else "filename")))
-        return False, wa.api.upload_media(media=media, mime_type=mime_type, filename=filename)['id']
+            raise ValueError(
+                msg.format(
+                    "mime_type and filename"
+                    if not mime_type and not filename
+                    else ("mime_type" if not mime_type else "filename")
+                )
+            )
+        return (
+            False,
+            wa.api.upload_media(media=media, mime_type=mime_type, filename=filename)[
+                "id"
+            ],
+        )
```

### Comparing `pywa-1.8.0/pywa/errors.py` & `pywa-1.9.0/pywa/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,66 +1,64 @@
 """
 This module contains the errors that can be raised by the WhatsApp Cloud API or incoming error from the webhook.
 """
 
 import functools
-from typing import Type, cast
+from typing import Iterable, Type
+
+import requests
 
 
 class WhatsAppError(Exception):
     """
     Base exception for all WhatsApp errors.
 
-    - `\`Cloud API Error Codes\` on developers.facebook.com <https://developers.facebook.com/docs/whatsapp/cloud-api/support/error-codes>`_.
+    - `'Cloud API Error Codes' on developers.facebook.com <https://developers.facebook.com/docs/whatsapp/cloud-api/support/error-codes>`_.
 
 
     Attributes:
         error_code: The error code.
         message: The error message.
         details: The error details (optional).
         fbtrace_id: The Facebook trace ID (optional).
         href: The href to the documentation (optional).
-        status_code: The status code (in case of response, else None).
+        raw_response: The :class:`requests.Response` obj that returned the error (optional, only if the error was raised
+         from an API call).
     """
 
-    __error_codes__: tuple | range | None = ()
+    __error_codes__: Iterable[int] | None
 
     def __init__(
         self,
         error_code: int,
         message: str,
         details: str | None,
         fbtrace_id: str | None,
         href: str | None,
-        status_code: int | None,
+        raw_response: requests.Response | None,
     ) -> None:
         self.error_code = error_code
         self.message = message
         self.details = details
         self.fbtrace_id = fbtrace_id
         self.href = href
-        self.status_code = status_code
+        self.raw_response = raw_response
 
-    @classmethod
-    def from_response(cls, status_code: int, error: dict) -> "WhatsAppError":
-        """Create an error from a response."""
-        return cls._get_exception(error["code"])(
-            status_code=status_code,
-            error_code=error["code"],
-            message=error["message"],
-            details=error.get("error_data", {}).get("details", None),
-            fbtrace_id=error.get("fbtrace_id"),
-            href=error.get("href"),
-        )
+    @property
+    def status_code(self) -> int | None:
+        """The status code (in case of raw_response, else None)."""
+        return self.raw_response.status_code if self.raw_response is not None else None
 
     @classmethod
-    def from_incoming_error(cls, error: dict) -> "WhatsAppError":
-        """Create an error from an incoming error."""
+    def from_dict(
+        cls, error: dict, response: requests.Response | None = None
+    ) -> "WhatsAppError":
+        """Create an error from a response."""
         return cls._get_exception(error["code"])(
-            status_code=None,
+            raw_response=response,
             error_code=error["code"],
             message=error["message"],
             details=error.get("error_data", {}).get("details", None),
             fbtrace_id=error.get("fbtrace_id"),
             href=error.get("href"),
         )
 
@@ -73,33 +71,29 @@
         )
 
     @staticmethod
     @functools.cache
     def _get_exception(code: int) -> Type["WhatsAppError"]:
         """Get the exception class from the error code."""
         return next(
-            (
-                e
-                for e in WhatsAppError._all_exceptions()
-                if code in cast(tuple, e.__error_codes__)
-            ),
+            (e for e in WhatsAppError._all_exceptions() if code in e.__error_codes__),
             WhatsAppError,
         )
 
     def __str__(self) -> str:
         return f"{self.__class__.__name__}(message={self.message!r}, details={self.details!r}, code={self.error_code!r})"
 
     def __repr__(self) -> str:
         return self.__str__()
 
 
 class AuthorizationError(WhatsAppError):
     """Base exception for all authorization errors."""
 
-    __error_codes__: tuple | range | None = None
+    __error_codes__ = None
 
 
 class AuthException(AuthorizationError):
     """We were unable to authenticate the app user"""
 
     __error_codes__ = (0,)
 
@@ -130,15 +124,15 @@
 
 # ====================================================================================================
 
 
 class ThrottlingError(WhatsAppError):
     """Base exception for all rate limit errors."""
 
-    __error_codes__: tuple | range | None = None
+    __error_codes__ = None
 
 
 class ToManyAPICalls(ThrottlingError):
     """The app has reached its API call rate limit."""
 
     __error_codes__ = (4,)
 
@@ -174,15 +168,15 @@
 
 # ====================================================================================================
 
 
 class IntegrityError(WhatsAppError):
     """Base exception for all integrity errors."""
 
-    __error_codes__: tuple | range | None = None
+    __error_codes__ = None
 
 
 class TemporarilyBlocked(IntegrityError):
     """
     The WhatsApp Business Account associated with the app has been restricted or disabled for violating a platform policy.
     """
 
@@ -201,15 +195,15 @@
 
 # ====================================================================================================
 
 
 class SendMessageError(WhatsAppError):
     """Base exception for all message errors."""
 
-    __error_codes__: tuple | range | None = None
+    __error_codes__ = None
 
 
 class MessageUndeliverable(SendMessageError):
     """Unable to deliver message. Reasons can include:
 
     - The recipient phone number is not a WhatsApp phone number.
     - Recipient has not accepted our new Terms of Service and Privacy Policy.
```

### Comparing `pywa-1.8.0/pywa/filters.py` & `pywa-1.9.0/pywa/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,27 +23,34 @@
     "contacts",
     "order",
     "callback",
     "message_status",
     "template_status",
 ]
 
-import re
 import abc
-from typing import Callable, TYPE_CHECKING, Iterable, TypeVar, TypeAlias, Type
-from pywa.errors import WhatsAppError, ReEngagementMessage
-from pywa.types import MessageType as Mt, Message as Msg, MessageStatus as Ms, MessageStatusType as Mst, \
-    CallbackButton, CallbackSelection, TemplateStatus as Ts
-from pywa.types.base_update import BaseUpdate
+import re
+from typing import TYPE_CHECKING, Callable, Iterable, TypeAlias, TypeVar
+
+from pywa.errors import ReEngagementMessage, WhatsAppError
+from pywa.types import CallbackButton, CallbackSelection
+from pywa.types import Message as Msg
+from pywa.types import MessageStatus as Ms
+from pywa.types import MessageStatusType as Mst
+from pywa.types import MessageType as Mt
+from pywa.types import TemplateStatus as Ts
+from pywa.types.base_update import BaseUpdate  # noqa
 
 if TYPE_CHECKING:
     from pywa import WhatsApp as Wa
 
     MessageFilterT: TypeAlias = Callable[[Wa, Msg], bool]
-    CallbackFilterT: TypeAlias = Callable[[Wa, CallbackButton | CallbackSelection], bool]
+    CallbackFilterT: TypeAlias = Callable[
+        [Wa, CallbackButton | CallbackSelection], bool
+    ]
     MessageStatusFilterT: TypeAlias = Callable[[Wa, Ms], bool]
     TemplateStatusFilterT: TypeAlias = Callable[[Wa, Ts], bool]
 
 T = TypeVar("T", bound=BaseUpdate)
 
 forwarded: MessageFilterT = lambda _, m: m.forwarded  # Filter for forwarded messages.
 """
@@ -90,26 +97,30 @@
     Filter for updates that don't pass the given filter.
 
     >>> not_(text.contains("Hello"))
     """
     return lambda wa, m: not fil(wa, m)
 
 
-def from_users(*numbers: str) -> MessageFilterT | CallbackFilterT | MessageStatusFilterT:
+def from_users(
+    *numbers: str,
+) -> MessageFilterT | CallbackFilterT | MessageStatusFilterT:
     """
     Filter for messages that are sent from the given numbers.
 
     >>> from_users("+1 555-555-5555", "972123456789")
     """
     only_nums_pattern = re.compile(r"\D")
     numbers = tuple(re.sub(only_nums_pattern, "", n) for n in numbers)
     return lambda _, m: m.from_user.wa_id in numbers
 
 
-def from_countries(*prefixes: str | int) -> MessageFilterT | CallbackFilterT | MessageStatusFilterT:
+def from_countries(
+    *prefixes: str | int,
+) -> MessageFilterT | CallbackFilterT | MessageStatusFilterT:
     """
     Filter for messages that are sent from the given country codes.
 
     - See https://countrycode.org/ for a list of country codes.
 
     It is always recommended to restrict the countries that can use your bot. remember that you pay for
     every conversation that you reply to.
@@ -146,21 +157,28 @@
         return m.type in cls.__message_types__
 
 
 class MediaFilter(_BaseUpdateFilter):
     """
     Useful filters for media messages. Alias: ``filters.media``.
     """
-    __message_types__ = (Mt.IMAGE, Mt.VIDEO, Mt.AUDIO, Mt.DOCUMENT, Mt.STICKER)
+
+    __message_types__ = (
+        Mt.IMAGE,
+        Mt.VIDEO,
+        Mt.AUDIO,
+        Mt.DOCUMENT,
+        Mt.STICKER,
+    )
 
     any: MessageFilterT = lambda _, m: m.has_media
     """
     Filter for all media messages.
         - Same as ``filters.media``.
-    
+
     >>> filters.media.any
     """
 
     @classmethod
     def mimetypes(cls, *mimetypes: str) -> MessageFilterT:
         """
         Filter for media messages that match any of the given mime types.
@@ -172,48 +190,50 @@
         >>> audio.mimetypes("audio/mpeg")
         """
         return lambda _, m: cls._match_type(m) and any(
             t == getattr(m, cls.__message_types__[0].value).mime_type for t in mimetypes
         )
 
 
-media: MessageFilterT | Type[MediaFilter] = MediaFilter
+media: MessageFilterT | type[MediaFilter] = MediaFilter
 
 
 class _MediaWithCaptionFilter(MediaFilter, abc.ABC):
     @classmethod
     def _has_caption(cls, _: Wa, m: Msg) -> bool:
         return cls._match_type(m) and m.caption is not None
 
     has_caption: MessageFilterT = _has_caption
     """
     Filter for media messages that have a caption.
-    
+
     >>> filters.media.has_caption
     """
 
 
 class TextFilter(_BaseUpdateFilter):
     """Useful filters for text messages. Alias: ``filters.text``."""
 
     __message_types__ = (Mt.TEXT,)
 
     any: MessageFilterT = lambda _, m: m.type == Mt.TEXT
     """
     Filter for all text messages.
         - Same as ``filters.text``.
-    
+
     >>> filters.text.any
     """
 
-    is_command: MessageFilterT = lambda _, m: m.type == Mt.TEXT and m.text.startswith(("!", "/", "#"))
+    is_command: MessageFilterT = lambda _, m: m.type == Mt.TEXT and m.text.startswith(
+        ("!", "/", "#")
+    )
     """
     Filter for text messages that are commands (start with ``!``, ``/``, or ``#``).
         - Use TextFilter.command if you want to filter for specific commands or prefixes.
-    
+
     >>> filters.text.is_command
     """
 
     @staticmethod
     def matches(*matches: str, ignore_case: bool = False) -> MessageFilterT:
         """
         Filter for text messages that match exactly the given text/s.
@@ -221,15 +241,18 @@
         >>> text.matches("Hello","Hi")
 
         Args:
             *matches: The text/s to filter for.
             ignore_case: Whether to ignore case when matching (default: ``False``).
         """
         matches = tuple(m.lower() for m in matches) if ignore_case else matches
-        return lambda _, m: TextFilter._match_type(m) and (m.text.lower() if ignore_case else m.text) in matches
+        return (
+            lambda _, m: TextFilter._match_type(m)
+            and (m.text.lower() if ignore_case else m.text) in matches
+        )
 
     @staticmethod
     def contains(*matches: str, ignore_case: bool = False) -> MessageFilterT:
         """
         Filter for text messages that contain the given text/s.
 
         >>> text.contains("Cat","Dog",ignore_case=True)
@@ -251,208 +274,230 @@
         >>> text.startswith("What", "When", ignore_case=True)
 
         Args:
             *matches: The text/s to filter for.
             ignore_case: Whether to ignore case when matching (default: ``False``).
         """
         matches = tuple(m.lower() for m in matches) if ignore_case else matches
-        return lambda _, m: TextFilter._match_type(m) and (m.text.lower() if ignore_case else m.text).startswith(
-            matches)
+        return lambda _, m: TextFilter._match_type(m) and (
+            m.text.lower() if ignore_case else m.text
+        ).startswith(matches)
 
     @staticmethod
     def endswith(*matches: str, ignore_case: bool = False) -> MessageFilterT:
         """
         Filter for text messages that end with the given text/s.
 
         >>> text.endswith("Bye", "See you", ignore_case=True)
 
         Args:
             *matches: The text/s to filter for.
             ignore_case: Whether to ignore case when matching (default: ``False``).
         """
         matches = tuple(m.lower() for m in matches) if ignore_case else matches
-        return lambda _, m: TextFilter._match_type(m) and (m.text.lower() if ignore_case else m.text).endswith(matches)
+        return lambda _, m: TextFilter._match_type(m) and (
+            m.text.lower() if ignore_case else m.text
+        ).endswith(matches)
 
     @staticmethod
     def regex(*patterns: str | re.Pattern, flags: int = 0) -> MessageFilterT:
         """
         Filter for text messages that match the given regex/regexes.
 
         >>> text.regex(r"Hello\s+World", r"Bye\s+World", flags=re.IGNORECASE)
 
         Args:
             *patterns: The regex/regexes to filter for.
             flags: The regex flags to use (default: ``0``).
         """
-        patterns = tuple(re.compile(p, flags) if isinstance(p, str) else p for p in patterns)
-        return lambda _, m: TextFilter._match_type(m) and any(re.match(p, m.text, flags) for p in patterns)
+        patterns = tuple(
+            re.compile(p, flags) if isinstance(p, str) else p for p in patterns
+        )
+        return lambda _, m: TextFilter._match_type(m) and any(
+            re.match(p, m.text, flags) for p in patterns
+        )
 
     @staticmethod
     def length(*lengths: tuple[int, int]) -> MessageFilterT:
         """
         Filter for text messages that have a length between the given range/s.
 
         >>> text.length((1, 10), (50, 100))
 
         Args:
             *lengths: The length range/s to filter for (e.g. (1, 10), (50, 100)).
         """
-        return lambda _, m: TextFilter._match_type(m) and any(i[0] <= len(m.text) <= i[1] for i in lengths)
+        return lambda _, m: TextFilter._match_type(m) and any(
+            i[0] <= len(m.text) <= i[1] for i in lengths
+        )
 
     @staticmethod
-    def command(*cmds: str, prefixes: str | Iterable[str] = "!", ignore_case: bool = False) -> MessageFilterT:
+    def command(
+        *cmds: str,
+        prefixes: str | Iterable[str] = "!",
+        ignore_case: bool = False,
+    ) -> MessageFilterT:
         """
         Filter for text messages that are commands.
 
         >>> text.command("start", "hello", prefixes=("!", "/"), ignore_case=True)
 
         Args:
             *cmds: The command/s to filter for (e.g. "start", "hello").
             prefixes: The prefix/s to filter for (default: "!", i.e. "!start").
             ignore_case: Whether to ignore case when matching (default: ``False``).
         """
         cmds = tuple(c.lower() for c in cmds) if ignore_case else cmds
         return lambda _, m: TextFilter._match_type(m) and (
-                m.text[0] in prefixes and (m.text[1:].lower() if ignore_case else m.text[1:]).startswith(cmds)
+            m.text[0] in prefixes
+            and (m.text[1:].lower() if ignore_case else m.text[1:]).startswith(cmds)
         )
 
 
-text: MessageFilterT | Type[TextFilter] = TextFilter
+text: MessageFilterT | type[TextFilter] = TextFilter
 
 
 class ImageFilter(_MediaWithCaptionFilter):
     """Useful filters for image messages. Alias: ``filters.image``."""
 
     __message_types__ = (Mt.IMAGE,)
 
     any: MessageFilterT = lambda _, m: ImageFilter._match_type(m)
     """
     Filter for all image messages.
         - Same as ``filters.image``.
-    
+
     >>> filters.image.any
     """
 
 
-image: MessageFilterT | Type[ImageFilter] = ImageFilter
+image: MessageFilterT | type[ImageFilter] = ImageFilter
 
 
 class VideoFilter(_MediaWithCaptionFilter):
     """Useful filters for video messages. Alias: ``filters.video``."""
 
     __message_types__ = (Mt.VIDEO,)
 
     any: MessageFilterT = lambda _, m: VideoFilter._match_type(m)
     """
     Filter for all video messages.
         - Same as ``filters.video``.
-    
+
     >>> filters.video.any
     """
 
 
-video: MessageFilterT | Type[VideoFilter] = VideoFilter
+video: MessageFilterT | type[VideoFilter] = VideoFilter
 
 
 class DocumentFilter(_MediaWithCaptionFilter):
     """Useful filters for document messages. Alias: ``filters.document``."""
 
     __message_types__ = (Mt.DOCUMENT,)
 
     any: MessageFilterT = lambda _, m: DocumentFilter._match_type(m)
     """
     Filter for all document messages.
         - Same as ``filters.document``.
-    
+
     >>> filters.document.any
     """
 
 
-document: MessageFilterT | Type[DocumentFilter] = DocumentFilter
+document: MessageFilterT | type[DocumentFilter] = DocumentFilter
 
 
 class AudioFilter(MediaFilter):
     """Useful filters for audio messages. Alias: ``filters.audio``."""
 
     __message_types__ = (Mt.AUDIO,)
 
     any: MessageFilterT = lambda _, m: AudioFilter._match_type(m)
     """
     Filter for all audio messages (voice notes and audio files).
         - Same as ``filters.audio``.
-    
+
     >>> filters.audio.any
     """
 
     voice: MessageFilterT = lambda _, m: AudioFilter._match_type(m) and m.audio.voice
     """
     Filter for audio messages that are voice notes.
-    
+
     >>> filters.audio.voice
     """
 
-    audio: MessageFilterT = lambda _, m: AudioFilter._match_type(m) and not m.audio.voice
+    audio: MessageFilterT = (
+        lambda _, m: AudioFilter._match_type(m) and not m.audio.voice
+    )
     """
     Filter for audio messages that are audio files.
-    
+
     >>> filters.audio.audio
     """
 
 
-audio: MessageFilterT | Type[AudioFilter] = AudioFilter
+audio: MessageFilterT | type[AudioFilter] = AudioFilter
 
 
 class StickerFilter(MediaFilter):
     """Useful filters for sticker messages. Alias: ``filters.sticker``."""
 
     __message_types__ = (Mt.STICKER,)
 
     any: MessageFilterT = lambda _, m: StickerFilter._match_type(m)
     """
     Filter for all sticker messages.
         - Same as ``filters.sticker``.
-    
+
     >>> filters.sticker.any
     """
 
-    animated: MessageFilterT = lambda _, m: StickerFilter._match_type(m) and m.sticker.animated
+    animated: MessageFilterT = (
+        lambda _, m: StickerFilter._match_type(m) and m.sticker.animated
+    )
     """
     Filter for animated sticker messages.
-    
+
     >>> filters.sticker.animated
     """
 
-    static: MessageFilterT = lambda _, m: StickerFilter._match_type(m) and not m.sticker.animated
+    static: MessageFilterT = (
+        lambda _, m: StickerFilter._match_type(m) and not m.sticker.animated
+    )
     """
     Filter for static sticker messages.
-    
+
     >>> filters.sticker.static
     """
 
 
-sticker: MessageFilterT | Type[StickerFilter] = StickerFilter
+sticker: MessageFilterT | type[StickerFilter] = StickerFilter
 
 
 class LocationFilter(_BaseUpdateFilter):
     """Useful filters for location messages. Alias: ``filters.location``."""
 
     __message_types__ = (Mt.LOCATION,)
 
     any: MessageFilterT = lambda _, m: LocationFilter._match_type(m)
     """
     Filter for all location messages.
         - Same as ``filters.location``.
-    
+
     >>> filters.location.any
     """
 
-    current_location: MessageFilterT = lambda _, m: LocationFilter._match_type(m) and m.location.current_location
+    current_location: MessageFilterT = (
+        lambda _, m: LocationFilter._match_type(m) and m.location.current_location
+    )
     """
     Filter for location messages that are the current location of the user and not just selected manually.
-    
+
     >>> filters.location.current_location
     """
 
     @staticmethod
     def in_radius(lat: float, lon: float, radius: float | int) -> MessageFilterT:
         """
         Filter for location messages that are in a given radius.
@@ -462,150 +507,173 @@
         Args:
             lat: Latitude of the center of the radius.
             lon: Longitude of the center of the radius.
             radius: Radius in kilometers.
         """
 
         def _in_radius(_: Wa, msg: Msg) -> bool:
-            return LocationFilter._match_type(msg) and \
-                msg.location.in_radius(lat=lat, lon=lon, radius=radius)
+            return LocationFilter._match_type(msg) and msg.location.in_radius(
+                lat=lat, lon=lon, radius=radius
+            )
 
         return _in_radius
 
 
-location: MessageFilterT | Type[LocationFilter] = LocationFilter
+location: MessageFilterT | type[LocationFilter] = LocationFilter
 
 
 class ReactionFilter(_BaseUpdateFilter):
     """Useful filters for reaction messages. Alias: ``filters.reaction``."""
 
     __message_types__ = (Mt.REACTION,)
 
     any: MessageFilterT = lambda _, m: ReactionFilter._match_type(m)
     """
     Filter for all reaction updates (added or removed).
         - Same as ``filters.reaction``.
-    
+
     >>> filters.reaction.any
     """
 
-    added: MessageFilterT = lambda _, m: ReactionFilter._match_type(m) and m.reaction.emojis is not None
+    added: MessageFilterT = (
+        lambda _, m: ReactionFilter._match_type(m) and m.reaction.emojis is not None
+    )
     """
     Filter for reaction messages that were added.
-    
+
     >>> filters.reaction.added
     """
 
-    removed: MessageFilterT = lambda _, m: ReactionFilter._match_type(m) and m.reaction.emojis is None
+    removed: MessageFilterT = (
+        lambda _, m: ReactionFilter._match_type(m) and m.reaction.emojis is None
+    )
     """
     Filter for reaction messages that were removed.
-    
+
     >>> filters.reaction.removed
     """
 
     @staticmethod
     def emojis(*emojis: str) -> MessageFilterT:
         """
         Filter for custom reaction messages. pass emojis as strings.
 
         >>> reaction.emojis("👍","👎")
         """
         return lambda _, m: ReactionFilter._match_type(m) and m.reaction.emoji in emojis
 
 
-reaction: MessageFilterT | Type[ReactionFilter] = ReactionFilter
+reaction: MessageFilterT | type[ReactionFilter] = ReactionFilter
 
 
 class ContactsFilter(_BaseUpdateFilter):
     """Useful filters for contact messages. Alias: ``filters.contacts``."""
 
     __message_types__ = (Mt.CONTACTS,)
 
     any: MessageFilterT = lambda _, m: ContactsFilter._match_type(m)
     """
     Filter for all contacts messages.
         - Same as ``filters.contacts``.
-    
+
     >>> filters.contacts.any
     """
 
     has_wa: MessageFilterT = lambda _, m: ContactsFilter._match_type(m) and (
-        any((p.wa_id for p in (phone for contact in m.contacts for phone in contact.phones)))
+        any(
+            (
+                p.wa_id
+                for p in (phone for contact in m.contacts for phone in contact.phones)
+            )
+        )
     )
     """
     Filter for contacts messages that have a WhatsApp account.
-    
+
     >>> filters.contacts.has_wa
     """
 
     @staticmethod
     def count(min_count: int, max_count: int) -> MessageFilterT:
         """
         Filter for contacts messages that have a number of contacts between min_count and max_count.
 
         >>> contacts.count(1, 1) # ensure only 1 contact
         >>> contacts.count(1, 5) # between 1 and 5 contacts
         """
-        return lambda _, m: ContactsFilter._match_type(m) and min_count <= len(m.contacts) <= max_count
+        return (
+            lambda _, m: ContactsFilter._match_type(m)
+            and min_count <= len(m.contacts) <= max_count
+        )
 
     @staticmethod
     def phones(*phones: str) -> MessageFilterT:
         """
         Filter for contacts messages that have the given phone number/s.
 
         >>> contacts.phones("+1 555-555-5555","972123456789")
         """
         only_nums_pattern = re.compile(r"\D")
         phones = [re.sub(only_nums_pattern, "", p) for p in phones]
         return lambda _, m: ContactsFilter._match_type(m) and (
-            any(re.sub(only_nums_pattern, "", p.phones) in phones for contact in m.contacts for p in contact.phones)
+            any(
+                re.sub(only_nums_pattern, "", p.phones) in phones
+                for contact in m.contacts
+                for p in contact.phones
+            )
         )
 
 
-contacts: MessageFilterT | Type[ContactsFilter] = ContactsFilter
+contacts: MessageFilterT | type[ContactsFilter] = ContactsFilter
 
 
 class OrderFilter(_BaseUpdateFilter):
     """Useful filters for order messages. Alias: ``filters.order``."""
 
     __message_types__ = (Mt.ORDER,)
 
     any: MessageFilterT = lambda _, m: OrderFilter._match_type(m)
     """
     Filter for all order messages.
         - Same as ``filters.order``.
-    
+
     >>> filters.order.any
     """
 
     @staticmethod
     def price(min_price: float, max_price: float) -> MessageFilterT:
         """
         Filter for order messages that have a total price between min_price and max_price.
 
         Args:
             min_price: Minimum price.
             max_price: Maximum price.
 
         >>> order.price(1, 100) # total price between 1 and 100
         """
-        return lambda _, m: OrderFilter._match_type(m) and min_price <= m.order.total_price <= max_price
+        return (
+            lambda _, m: OrderFilter._match_type(m)
+            and min_price <= m.order.total_price <= max_price
+        )
 
     @staticmethod
     def count(min_count: int, max_count: int) -> MessageFilterT:
         """
         Filter for order messages that have a number of items between min_count and max_count.
 
         Args:
             min_count: Minimum number of items.
             max_count: Maximum number of items.
 
         >>> order.count(1, 5) # between 1 and 5 items
         """
-        return lambda _, m: OrderFilter._match_type(m) and min_count <= len(m.order.products) <= max_count
+        return (
+            lambda _, m: OrderFilter._match_type(m)
+            and min_count <= len(m.order.products) <= max_count
+        )
 
     @staticmethod
     def has_product(*skus: str) -> MessageFilterT:
         """
         Filter for order messages that have the given product/s.
 
         Args:
@@ -614,50 +682,50 @@
         >>> order.has_product("pizza_1","pizza_2")
         """
         return lambda _, m: OrderFilter._match_type(m) and (
             any(p.sku in skus for p in m.order.products)
         )
 
 
-order: MessageFilterT | Type[OrderFilter] = OrderFilter
+order: MessageFilterT | type[OrderFilter] = OrderFilter
 
 
 class UnsupportedMsgFilter(_BaseUpdateFilter):
     """Useful filters for unsupported messages. Alias: ``filters.unsupported``."""
 
     __message_types__ = (Mt.UNSUPPORTED,)
 
     def __new__(cls):
         return cls.any
 
     any: MessageFilterT = lambda _, m: m.type == Mt.UNSUPPORTED
     """
     Filter for all unsupported messages.
         - Same as ``filters.unsupported``.
-    
+
     >>> filters.unsupported.any
     """
 
 
-unsupported: MessageFilterT | Type[UnsupportedMsgFilter] = UnsupportedMsgFilter
+unsupported: MessageFilterT | type[UnsupportedMsgFilter] = UnsupportedMsgFilter
 
 
 class CallbackFilter(_BaseUpdateFilter):
     """Useful filters for callback queries. Alias: ``filters.callback``."""
 
     __message_types__ = (Mt.INTERACTIVE,)
 
     def __new__(cls):
         return cls.any
 
     any: CallbackFilterT = lambda _, __: True
     """
     Filter for all callback queries (the default).
         - Same as ``filters.callback``.
-    
+
     >>> filters.callback.any
     """
 
     @staticmethod
     def data_matches(*matches: str, ignore_case: bool = False) -> CallbackFilterT:
         """
         Filter for callbacks their data match exactly the given string/s.
@@ -680,43 +748,49 @@
         >>> callback.data_startswith("id:")
 
         Args:
             *matches: The string/s to match.
             ignore_case: Whether to ignore case when matching (default: False).
         """
         matches = tuple(m.lower() for m in matches) if ignore_case else matches
-        return lambda _, c: (c.data.lower() if ignore_case else c.data).startswith(matches)
+        return lambda _, c: (c.data.lower() if ignore_case else c.data).startswith(
+            matches
+        )
 
     @staticmethod
     def data_endswith(*matches: str, ignore_case: bool = False) -> CallbackFilterT:
         """
         Filter for callbacks their data ends with the given string/s.
 
         >>> callback.data_endswith(":true", ":false")
 
         Args:
             *matches: The string/s to match.
             ignore_case: Whether to ignore case when matching (default: False).
         """
         matches = tuple(m.lower() for m in matches) if ignore_case else matches
-        return lambda _, c: (c.data.lower() if ignore_case else c.data).endswith(matches)
+        return lambda _, c: (c.data.lower() if ignore_case else c.data).endswith(
+            matches
+        )
 
     @staticmethod
     def data_contains(*matches: str, ignore_case: bool = False) -> CallbackFilterT:
         """
         Filter for callbacks their data contains the given string/s.
 
         >>> callback.data_contains("back")
 
         Args:
             *matches: The string/s to match.
             ignore_case: Whether to ignore case when matching (default: False).
         """
         matches = tuple(m.lower() for m in matches) if ignore_case else matches
-        return lambda _, c: any((m in (c.data.lower() if ignore_case else c.data) for m in matches))
+        return lambda _, c: any(
+            (m in (c.data.lower() if ignore_case else c.data) for m in matches)
+        )
 
     @staticmethod
     def data_regex(*patterns: str | re.Pattern, flags: int = 0) -> CallbackFilterT:
         """
         Filter for callbacks their data matches the given regex/regexes.
 
         >>> callback.data_regex(r"^\d+$")  # only digits
@@ -725,96 +799,103 @@
             *patterns: The regex/regexes to match.
             flags: The regex flags to use (default: 0).
         """
         patterns = tuple(re.compile(p) if isinstance(p, str) else p for p in patterns)
         return lambda _, c: any((re.match(p, c.data, flags) for p in patterns))
 
 
-callback: CallbackFilterT | Type[CallbackFilter] = CallbackFilter
+callback: CallbackFilterT | type[CallbackFilter] = CallbackFilter
 
 
 class MessageStatusFilter(_BaseUpdateFilter):
     """Useful filters for message status updates. Alias: ``filters.message_status``."""
 
     __message_types__ = ()
 
     any: MessageStatusFilterT = lambda _, __: True
     """
     Filter for all message status updates (the default).
         - Same as ``filters.message_status``.
-        
+
     >>> filters.message_status.any
     """
 
     sent: MessageStatusFilterT = lambda _, s: s.status == Mst.SENT
     """
     Filter for messages that have been sent.
-    
+
     >>> filters.message_status.sent
     """
 
     delivered: MessageStatusFilterT = lambda _, s: s.status == Mst.DELIVERED
     """
     Filter for messages that have been delivered.
-    
+
     >>> filters.message_status.delivered
     """
 
     read: MessageStatusFilterT = lambda _, s: s.status == Mst.READ
     """
     Filter for messages that have been read.
-    
+
     >>> filters.message_status.read
     """
 
     failed: MessageStatusFilterT = lambda _, s: s.status == Mst.FAILED
     """
     Filter for status updates of messages that have failed to send.
-    
+
     >>> filters.message_status.failed
     """
 
     @staticmethod
-    def failed_with(*errors: Type[WhatsAppError] | int) -> MessageStatusFilterT:
+    def failed_with(
+        *errors: type[WhatsAppError] | int,
+    ) -> MessageStatusFilterT:
         """
         Filter for status updates of messages that have failed to send with the given error/s.
 
         Args:
             *errors: The exceptions from :mod:`pywa.errors` or error codes to match.
 
         >>> message_status.failed_with(ReEngagementMessage)
         >>> message_status.failed_with(131051)
         """
         error_codes = tuple(c for c in errors if isinstance(c, int))
-        exceptions = tuple(e for e in errors if e not in error_codes and issubclass(e, WhatsAppError))
+        exceptions = tuple(
+            e for e in errors if e not in error_codes and issubclass(e, WhatsAppError)
+        )
         return lambda _, s: s.status == Mst.FAILED and (
-            any((isinstance(s.error, e) for e in exceptions)) or s.error.error_code in error_codes
+            any((isinstance(s.error, e) for e in exceptions))
+            or s.error.error_code in error_codes
         )
 
 
-message_status: MessageStatusFilterT | Type[MessageStatusFilter] = MessageStatusFilter
+message_status: MessageStatusFilterT | type[MessageStatusFilter] = MessageStatusFilter
 
 
 class TemplateStatusFilter(_BaseUpdateFilter):
     """Useful filters for template status updates. Alias: ``filters.template_status``."""
 
     __message_types__ = ()
 
     any: TemplateStatusFilterT = lambda _, __: True
     """
     Filter for all template status updates (the default).
         - Same as ``filters.template_status``.
-        
+
     >>> filters.template_status.any
     """
 
-    template_name: lambda name: TemplateStatusFilterT = lambda name: lambda _, s: s.template_name == name
+    template_name: lambda name: TemplateStatusFilterT = (
+        lambda name: lambda _, s: s.template_name == name
+    )
     """
     Filter for template status updates that are for the given template name.
-    
+
     >>> template_status.template_name("my_template")
     """
 
     @staticmethod
     def on_event(*events: Ts.TemplateEvent) -> TemplateStatusFilterT:
         """
         Filter for template status updates that are for the given event/s.
@@ -823,20 +904,24 @@
             *events: The template events to filter for.
 
         >>> template_status.on_event(Ts.TemplateEvent.APPROVED)
         """
         return lambda _, s: s.event in events
 
     @staticmethod
-    def on_rejection_reason(*reasons: Ts.TemplateRejectionReason) -> TemplateStatusFilterT:
+    def on_rejection_reason(
+        *reasons: Ts.TemplateRejectionReason,
+    ) -> TemplateStatusFilterT:
         """
         Filter for template status updates that are for the given reason/s.
 
         Args:
             *reasons: The template reasons to filter for.
 
         >>> template_status.on_rejection_reason(Ts.TemplateRejectionReason.INCORRECT_CATEGORY)
         """
         return lambda _, s: s.reason in reasons
 
 
-template_status: TemplateStatusFilterT | Type[TemplateStatusFilter] = TemplateStatusFilter
+template_status: (
+    TemplateStatusFilterT | type[TemplateStatusFilter]
+) = TemplateStatusFilter
```

### Comparing `pywa-1.8.0/pywa/handlers.py` & `pywa-1.9.0/pywa/handlers.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,109 +9,163 @@
     "CallbackButtonHandler",
     "CallbackSelectionHandler",
     "RawUpdateHandler",
     "MessageStatusHandler",
     "TemplateStatusHandler",
 ]
 
-import dataclasses
 import abc
+import dataclasses
 import functools
-from typing import Callable, Any, TYPE_CHECKING, cast, TypeVar
-from pywa.types import Message, CallbackButton, CallbackSelection, MessageStatus, TemplateStatus
-from pywa.types.base_update import BaseUpdate
+from typing import TYPE_CHECKING, Any, Callable, TypeVar, cast
+
+from pywa.types import (
+    CallbackButton,
+    CallbackSelection,
+    Message,
+    MessageStatus,
+    TemplateStatus,
+)
 from pywa.types.callback import CallbackData
 
 if TYPE_CHECKING:
     from pywa.client import WhatsApp
+    from pywa.types.base_update import BaseUpdate
+
 
 CallbackDataFactoryT = TypeVar(
-    'CallbackDataFactoryT',
+    "CallbackDataFactoryT",
     bound=(
-            type[str] |
-            type[CallbackData] |
-            tuple[type[CallbackData | Any], ...] |
-            list[type[CallbackData | Any], ...] |
-            Callable[[str], Any]
-    )
+        type[str]
+        | type[CallbackData]
+        | tuple[type[CallbackData | Any], ...]
+        | list[type[CallbackData | Any], ...]
+        | Callable[[str], Any]
+    ),
 )
 """Type hint for the callback data factory."""
 
 
 def _safe_issubclass(obj: type, base: type) -> bool:
     """Check if an obj is a subclass of another class without raising a TypeError."""
     try:
         return issubclass(obj, base)
     except TypeError:
         return False
 
 
 def _resolve_callback_data_factory(
-        factory: CallbackDataFactoryT
+    factory: CallbackDataFactoryT,
 ) -> tuple[CallbackDataFactoryT, Callable[[WhatsApp, Any], bool] | None]:
     """Internal function to resolve the callback data factory into a constractor and a filter."""
     clb_filter = None
-    if isinstance(factory, (tuple, list)):  # The factory is a tuple|list of CallbackData subclasses or functions
+    if isinstance(
+        factory, (tuple, list)
+    ):  # The factory is a tuple|list of CallbackData subclasses or functions
         constractor = lambda data: (  # noqa
             factory.__class__(
-                map(lambda fs: (fs[0].from_str if issubclass(fs[0], CallbackData) else fs[0])(fs[1]),  # noqa
-                    zip(factory, data.split(CallbackData.__callback_sep__))))
+                map(
+                    lambda fs: (
+                        fs[0].from_str if issubclass(fs[0], CallbackData) else fs[0]
+                    )(fs[1]),
+                    zip(
+                        factory,
+                        data.split(CallbackData.__callback_sep__),
+                    ),
+                )
+            )
         )
-        if any((callback_datas := tuple(bool(issubclass(f, CallbackData)) for f in factory))):
+        if any(
+            (
+                callback_datas := tuple(
+                    bool(issubclass(f, CallbackData)) for f in factory
+                )
+            )
+        ):
 
-            def clb_filter(_: WhatsApp, btn_or_sel: CallbackButton | CallbackSelection) -> bool:
+            def clb_filter(
+                _: WhatsApp,
+                btn_or_sel: CallbackButton | CallbackSelection,
+            ) -> bool:
                 datas = btn_or_sel.data.split(CallbackData.__callback_sep__)
                 if len(datas) != len(factory):
                     return False
                 return all(
                     datas[i].startswith(
-                        str(cast(CallbackData, factory[i]).__callback_id__) +
-                        cast(CallbackData, factory[i]).__callback_data_sep__
+                        str(cast(CallbackData, factory[i]).__callback_id__)
+                        + cast(CallbackData, factory[i]).__callback_data_sep__
                     )
-                    for i, b in enumerate(callback_datas) if b
+                    for i, b in enumerate(callback_datas)
+                    if b
                 )
 
-    elif _safe_issubclass(factory, CallbackData):  # The factory is a single CallbackData subclass
+    elif _safe_issubclass(
+        factory, CallbackData
+    ):  # The factory is a single CallbackData subclass
         constractor = factory.from_str
 
-        def clb_filter(_: WhatsApp, btn_or_sel: CallbackButton | CallbackSelection) -> bool:
-            return len(btn_or_sel.data.split(CallbackData.__callback_sep__)) == 1 and \
-                btn_or_sel.data.startswith(str(factory.__callback_id__) + factory.__callback_data_sep__)
+        def clb_filter(
+            _: WhatsApp, btn_or_sel: CallbackButton | CallbackSelection
+        ) -> bool:
+            return len(
+                btn_or_sel.data.split(CallbackData.__callback_sep__)
+            ) == 1 and btn_or_sel.data.startswith(
+                str(factory.__callback_id__) + factory.__callback_data_sep__
+            )
 
     else:  # The factory is a function or custom type
         constractor = factory
 
     return constractor, clb_filter
 
 
 def _call_callback_handler(
     handler: CallbackButtonHandler | CallbackSelectionHandler,
     wa: WhatsApp,
-    clb_or_sel: CallbackButton | CallbackSelection
+    clb_or_sel: CallbackButton | CallbackSelection,
 ):
     """Internal function to call a callback handler."""
     if handler.factory_before_filters and handler.factory_filter is not None:
         if handler.factory_filter(wa, clb_or_sel):
-            clb_or_sel = dataclasses.replace(clb_or_sel, data=handler.factory(clb_or_sel.data))
+            clb_or_sel = dataclasses.replace(
+                clb_or_sel, data=handler.factory(clb_or_sel.data)
+            )
         else:
             return
     try:
-        pass_filters = all((f(wa, clb_or_sel) for f in (
-            *((handler.factory_filter,) if not handler.factory_before_filters
-                and handler.factory_filter is not None else tuple()),
-            *handler.filters
-        )))
+        pass_filters = all(
+            (
+                f(wa, clb_or_sel)
+                for f in (
+                    *(
+                        (handler.factory_filter,)
+                        if not handler.factory_before_filters
+                        and handler.factory_filter is not None
+                        else tuple()
+                    ),
+                    *handler.filters,
+                )
+            )
+        )
     except AttributeError as e:
-        if not handler.factory_before_filters and isinstance(e.obj, str) and handler.factory is not str:
-            raise TypeError("It seems like your filters tried to access a field of the callback data before the factory"
-                            " was applied. Please set `factory_before_filters=True` in the handler constructor.") from e
+        if (
+            not handler.factory_before_filters
+            and isinstance(e.obj, str)
+            and handler.factory is not str
+        ):
+            raise TypeError(
+                "It seems like your filters tried to access a field of the callback data before the factory"
+                " was applied. Please set `factory_before_filters=True` in the handler constructor."
+            ) from e
         raise
     if pass_filters:
         if not handler.factory_before_filters and handler.factory is not str:
-            clb_or_sel = dataclasses.replace(clb_or_sel, data=handler.factory(clb_or_sel.data))
+            clb_or_sel = dataclasses.replace(
+                clb_or_sel, data=handler.factory(clb_or_sel.data)
+            )
         handler.handler(wa, clb_or_sel)
 
 
 class Handler(abc.ABC):
     """Base class for all handlers."""
 
     @property
@@ -120,21 +174,23 @@
         """
         The field name of the webhook update
         https://developers.facebook.com/docs/graph-api/webhooks/reference/whatsapp-business-account
         """
 
     @property
     @abc.abstractmethod
-    def __update_constructor__(self) -> Callable[[WhatsApp, dict], BaseUpdate]:
+    def __update_constructor__(
+        self,
+    ) -> Callable[[WhatsApp, dict], BaseUpdate]:
         """The constructor to use to construct the update object from the webhook update dict."""
 
     def __init__(
-            self,
-            handler: Callable[[WhatsApp, Any], Any],
-            *filters: Callable[[WhatsApp, Any], bool]
+        self,
+        handler: Callable[[WhatsApp, Any], Any],
+        *filters: Callable[[WhatsApp, Any], bool],
     ):
         """
         Initialize a new handler.
         """
         self.handler = handler
         self.filters = filters
 
@@ -151,15 +207,19 @@
 
         **IMPORTANT:** This function is for internal use only, DO NOT USE IT to get the available handlers
         (use ``Handler.__subclasses__()`` instead).
 
         **IMPORTANT:** This function is cached, so if you subclass `Handler` after calling this function, the new class
         will not be included in the returned dict.
         """
-        return {h.__field_name__: h for h in Handler.__subclasses__() if h.__field_name__ is not None}
+        return {
+            h.__field_name__: h
+            for h in Handler.__subclasses__()
+            if h.__field_name__ is not None
+        }
 
     def __str__(self) -> str:
         return f"{self.__class__.__name__}(handler={self.handler!r}, filters={self.filters!r})"
 
     def __repr__(self) -> str:
         return self.__str__()
 
@@ -179,21 +239,22 @@
 
     Args:
         handler: The handler function (gets the :class:`pywa.WhatsApp` instance and a :class:`pywa.types.Message` as
          arguments)
         *filters: The filters to apply to the handler (gets a :class:`pywa.WhatsApp` instance and a
          :class:`pywa.types.Message` and returns a :class:`bool`)
     """
-    __field_name__ = 'messages'
+
+    __field_name__ = "messages"
     __update_constructor__ = Message.from_update
 
     def __init__(
         self,
         handler: Callable[[WhatsApp, Message], Any],
-        *filters: Callable[[WhatsApp, Message], bool]
+        *filters: Callable[[WhatsApp, Message], bool],
     ):
         super().__init__(handler, *filters)
 
 
 class CallbackButtonHandler(Handler):
     """
     Handler for callback buttons (User clicks on a :class:`pywa.types.Button`).
@@ -212,25 +273,29 @@
         *filters: The filters to apply to the handler (gets a :class:`pywa.WhatsApp` instance and a
          :class:`pywa.types.CallbackButton` and returns a :class:`bool`)
         factory: The constructor/s to use to construct the callback data (default: :class:`str`. If the factory is a
          subclass of :class:`pywa.types.CallbackData`, a matching filter is automatically added).
         factory_before_filters: Whether to apply the factory before the filters (default: ``False``. If ``True``, the
          filters will get the callback data after the factory is applied).
     """
-    __field_name__ = 'messages'
+
+    __field_name__ = "messages"
     __update_constructor__ = CallbackButton.from_update
 
     def __init__(
         self,
         handler: Callable[[WhatsApp, CallbackButton], Any],
         *filters: Callable[[WhatsApp, CallbackButton], bool],
         factory: CallbackDataFactoryT = str,
-        factory_before_filters: bool = False
+        factory_before_filters: bool = False,
     ):
-        self.factory, self.factory_filter = _resolve_callback_data_factory(factory)
+        (
+            self.factory,
+            self.factory_filter,
+        ) = _resolve_callback_data_factory(factory)
         self.factory_before_filters = factory_before_filters
         super().__init__(handler, *filters)
 
     def __call__(self, wa: WhatsApp, clb: CallbackButton):
         _call_callback_handler(self, wa, clb)
 
     def __str__(self) -> str:
@@ -256,25 +321,29 @@
         *filters: The filters to apply to the handler. (gets a :class:`pywa.WhatsApp` instance and a
          :class:`pywa.types.CallbackSelection` and returns a :class:`bool`)
         factory: The constructor/s to use to construct the callback data (default: :class:`str`. If the factory is a
          subclass of :class:`pywa.types.CallbackData`, a matching filter is automatically added).
         factory_before_filters: Whether to apply the factory before the filters (default: ``False``. If ``True``, the
          filters will get the callback data after the factory is applied).
     """
-    __field_name__ = 'messages'
+
+    __field_name__ = "messages"
     __update_constructor__ = CallbackSelection.from_update
 
     def __init__(
         self,
         handler: Callable[[WhatsApp, CallbackSelection], Any],
         *filters: Callable[[WhatsApp, CallbackSelection], bool],
         factory: CallbackDataFactoryT = str,
-        factory_before_filters: bool = False
+        factory_before_filters: bool = False,
     ):
-        self.factory, self.factory_filter = _resolve_callback_data_factory(factory)
+        (
+            self.factory,
+            self.factory_filter,
+        ) = _resolve_callback_data_factory(factory)
         self.factory_before_filters = factory_before_filters
         super().__init__(handler, *filters)
 
     def __call__(self, wa: WhatsApp, sel: CallbackSelection):
         _call_callback_handler(self, wa, sel)
 
     def __str__(self) -> str:
@@ -298,21 +367,22 @@
 
     Args:
         handler: The handler function (gets a :class:`pywa.WhatsApp` instance and a :class:`pywa.types.MessageStatus` as
             arguments)
         *filters: The filters to apply to the handler (gets a :class:`pywa.WhatsApp` instance and a
             :class:`pywa.types.MessageStatus` and returns a :class:`bool`)
     """
-    __field_name__ = 'messages'
+
+    __field_name__ = "messages"
     __update_constructor__ = MessageStatus.from_update
 
     def __init__(
         self,
         handler: Callable[[WhatsApp, MessageStatus], Any],
-        *filters: Callable[[WhatsApp, MessageStatus], bool]
+        *filters: Callable[[WhatsApp, MessageStatus], bool],
     ):
         super().__init__(handler, *filters)
 
 
 class TemplateStatusHandler(Handler):
     """
     Handler for :class:`pywa.types.TemplateStatus` updates (Template message is approved, rejected etc...).
@@ -332,21 +402,22 @@
 
     Args:
         handler: The handler function (gets a :class:`pywa.WhatsApp` instance and a
             :class:`pywa.types.TemplateStatus` as arguments)
         *filters: The filters to apply to the handler (gets a :class:`pywa.WhatsApp` instance and a
             :class:`pywa.types.TemplateStatus` and returns a :class:`bool`)
     """
-    __field_name__ = 'message_template_status_update'
+
+    __field_name__ = "message_template_status_update"
     __update_constructor__ = TemplateStatus.from_update
 
     def __init__(
         self,
         handler: Callable[[WhatsApp, TemplateStatus], Any],
-        *filters: Callable[[WhatsApp, TemplateStatus], bool]
+        *filters: Callable[[WhatsApp, TemplateStatus], bool],
     ):
         super().__init__(handler, *filters)
 
 
 class RawUpdateHandler(Handler):
     """
     A raw update handler.
@@ -362,34 +433,38 @@
         >>> wa.add_handlers(RawUpdateHandler(print_updates))
 
     Args:
         handler: The handler function (gets a :class:`pywa.WhatsApp` instance and a :class:`dict` as arguments)
         *filters: The filters to apply to the handler (gets a :class:`pywa.WhatsApp` instance and a :class:`dict` and
             returns a :class:`bool`)
     """
+
     __field_name__ = None
     __update_constructor__ = lambda _, data: data  # noqa
 
     def __init__(
         self,
         handler: Callable[[WhatsApp, dict], Any],
-        *filters: Callable[[WhatsApp, dict], bool]
+        *filters: Callable[[WhatsApp, dict], bool],
     ):
         super().__init__(handler, *filters)
 
 
 class HandlerDecorators:
     """This class is used by the :class:`WhatsApp` client to register handlers using decorators."""
 
     def __init__(self: WhatsApp):
         raise TypeError("This class cannot be instantiated.")
 
     def on_raw_update(
-            self: WhatsApp, *filters: Callable[[WhatsApp, dict], bool]
-    ) -> Callable[[Callable[[WhatsApp, dict], Any]], Callable[[WhatsApp, dict], Any]]:
+        self: WhatsApp, *filters: Callable[[WhatsApp, dict], bool]
+    ) -> Callable[
+        [Callable[[WhatsApp, dict], Any]],
+        Callable[[WhatsApp, dict], Any],
+    ]:
         """
         Decorator to register a function as a handler for raw updates (:class:`dict`).
 
         - This handler is called for **EVERY** update received from WhatsApp, even if it's not sent to the client phone number.
         - Shortcut for :func:`~pywa.client.WhatsApp.add_handlers` with a :class:`RawUpdateHandler`.
 
         Example:
@@ -399,23 +474,30 @@
             ... def raw_update_handler(_: WhatsApp, update: dict):
             ...     print(update)
 
         Args:
             *filters: Filters to apply to the incoming updates (filters are function that take a :class:`pywa.WhatsApp`
              instance and the incoming update :class:`dict` and return a :class:`bool` if the update should be handled).
         """
+
         @functools.wraps(self.on_raw_update)
-        def decorator(func: Callable[[WhatsApp, dict], Any]) -> Callable[[WhatsApp, dict], Any]:
+        def decorator(
+            func: Callable[[WhatsApp, dict], Any]
+        ) -> Callable[[WhatsApp, dict], Any]:
             self.add_handlers(RawUpdateHandler(func, *filters))
             return func
+
         return decorator
 
     def on_message(
-            self: WhatsApp, *filters: Callable[[WhatsApp, Message], bool]
-    ) -> Callable[[Callable[[WhatsApp, Message], Any]], Callable[[WhatsApp, Message], Any]]:
+        self: WhatsApp, *filters: Callable[[WhatsApp, Message], bool]
+    ) -> Callable[
+        [Callable[[WhatsApp, Message], Any]],
+        Callable[[WhatsApp, Message], Any],
+    ]:
         """
         Decorator to register a function as a handler for incoming :class:`pywa.types.Message` (User sends a message).
 
         - Shortcut for :func:`~pywa.client.WhatsApp.add_handlers` with a :class:`MessageHandler`.
 
         Example:
 
@@ -427,26 +509,33 @@
             ...     msg.react("👋")
             ...     msg.reply_text(text="Hello from PyWa!", quote=True, buttons=[Button("Help", data="help")
 
         Args:
             *filters: Filters to apply to the incoming messages (filters are function that take a :class:`pywa.WhatsApp`
              instance and the incoming :class:`pywa.types.Message` and return a boolean).
         """
+
         @functools.wraps(self.on_message)
-        def decorator(func: Callable[[WhatsApp, Message], Any]) -> Callable[[WhatsApp, Message], Any]:
+        def decorator(
+            func: Callable[[WhatsApp, Message], Any]
+        ) -> Callable[[WhatsApp, Message], Any]:
             self.add_handlers(MessageHandler(func, *filters))
             return func
+
         return decorator
 
     def on_callback_button(
-            self: WhatsApp,
-            *filters: Callable[[WhatsApp, CallbackButton], bool],
-            factory: CallbackDataFactoryT = str,
-            factory_before_filters: bool = False
-    ) -> Callable[[Callable[[WhatsApp, CallbackButton], Any]], Callable[[WhatsApp, CallbackButton], Any]]:
+        self: WhatsApp,
+        *filters: Callable[[WhatsApp, CallbackButton], bool],
+        factory: CallbackDataFactoryT = str,
+        factory_before_filters: bool = False,
+    ) -> Callable[
+        [Callable[[WhatsApp, CallbackButton], Any]],
+        Callable[[WhatsApp, CallbackButton], Any],
+    ]:
         """
         Decorator to register a function as a handler when a user clicks on a :class:`pywa.types.Button`.
 
         - Shortcut for :func:`~pywa.client.WhatsApp.add_handlers` with a :class:`CallbackButtonHandler`.
 
         Example:
 
@@ -461,30 +550,40 @@
             *filters: Filters to apply to the incoming callback button presses (filters are function that take a
              :class:`pywa.WhatsApp` instance and the incoming :class:`pywa.types.CallbackButton` and return :class:`bool`).
             factory: The constructor/s to use for the callback data (default: :class:`str`. If the factory is a
              subclass of :class:`pywa.types.CallbackData`, a matching filter is automatically added).
             factory_before_filters: Whether to apply the factory before the filters (default: ``False``. If ``True``, the
              filters will get the callback data after the factory is applied).
         """
+
         @functools.wraps(self.on_callback_button)
-        def decorator(func: Callable[[WhatsApp, CallbackButton], Any]) -> Callable[[WhatsApp, CallbackButton], Any]:
+        def decorator(
+            func: Callable[[WhatsApp, CallbackButton], Any]
+        ) -> Callable[[WhatsApp, CallbackButton], Any]:
             self.add_handlers(
                 CallbackButtonHandler(
-                    func, *filters, factory=factory, factory_before_filters=factory_before_filters
+                    func,
+                    *filters,
+                    factory=factory,
+                    factory_before_filters=factory_before_filters,
                 )
             )
             return func
+
         return decorator
 
     def on_callback_selection(
-            self: WhatsApp,
-            *filters: Callable[[WhatsApp, CallbackSelection], bool],
-            factory: CallbackDataFactoryT = str,
-            factory_before_filters: bool = False
-    ) -> Callable[[Callable[[WhatsApp, CallbackSelection], Any]], Callable[[WhatsApp, CallbackSelection], Any]]:
+        self: WhatsApp,
+        *filters: Callable[[WhatsApp, CallbackSelection], bool],
+        factory: CallbackDataFactoryT = str,
+        factory_before_filters: bool = False,
+    ) -> Callable[
+        [Callable[[WhatsApp, CallbackSelection], Any]],
+        Callable[[WhatsApp, CallbackSelection], Any],
+    ]:
         """
         Decorator to register a function as a handler when a user selects an option from a :class:`pywa.types.SectionList`.
 
         - Shortcut for :func:`~pywa.client.WhatsApp.add_handlers` with a :class:`CallbackSelectionHandler`.
 
         Example:
 
@@ -499,29 +598,38 @@
             *filters: Filters to apply to the incoming callback selections (filters are function that take a
              :class:`pywa.WhatsApp` instance and the incoming :class:`pywa.types.CallbackSelection` and return :class:`bool`).
             factory: The constructor/s to use for the callback data (default: :class:`str`. If the factory is a
              subclass of :class:`pywa.types.CallbackData`, a matching filter is automatically added).
             factory_before_filters: Whether to apply the factory before the filters (default: ``False``. If ``True``, the
              filters will get the callback data after the factory is applied).
         """
+
         @functools.wraps(self.on_callback_selection)
         def decorator(
-                func: Callable[[WhatsApp, CallbackSelection], Any]
+            func: Callable[[WhatsApp, CallbackSelection], Any]
         ) -> Callable[[WhatsApp, CallbackSelection], Any]:
             self.add_handlers(
                 CallbackSelectionHandler(
-                    func, *filters, factory=factory, factory_before_filters=factory_before_filters
+                    func,
+                    *filters,
+                    factory=factory,
+                    factory_before_filters=factory_before_filters,
                 )
             )
             return func
+
         return decorator
 
     def on_message_status(
-            self: WhatsApp, *filters: Callable[[WhatsApp, MessageStatus], bool]
-    ) -> Callable[[Callable[[WhatsApp, MessageStatus], Any]], Callable[[WhatsApp, MessageStatus], Any]]:
+        self: WhatsApp,
+        *filters: Callable[[WhatsApp, MessageStatus], bool],
+    ) -> Callable[
+        [Callable[[WhatsApp, MessageStatus], Any]],
+        Callable[[WhatsApp, MessageStatus], Any],
+    ]:
         """
         Decorator to register a function as a handler for incoming message status changes (Message is sent, delivered,
         read, failed, etc...).
 
         - Shortcut for :func:`~pywa.client.WhatsApp.add_handlers` with a :class:`MessageStatusHandler`.
 
         **DO NOT USE THIS HANDLER WITHOUT FILTERS TO SEND MESSAGES, IT WILL CAUSE AN INFINITE LOOP!**
@@ -536,24 +644,31 @@
             ...     print(f"Message {status.id} failed to send to {status.from_user.wa_id}: {status.error.message})
 
 
         Args:
             *filters: Filters to apply to the incoming message status changes (filters are function that take a
              :class:`pywa.WhatsApp` instance and the incoming :class:`pywa.types.MessageStatus` and return :class:`bool`).
         """
+
         @functools.wraps(self.on_message_status)
-        def decorator(func: Callable[[WhatsApp, MessageStatus], Any]) -> Callable[[WhatsApp, MessageStatus], Any]:
+        def decorator(
+            func: Callable[[WhatsApp, MessageStatus], Any]
+        ) -> Callable[[WhatsApp, MessageStatus], Any]:
             self.add_handlers(MessageStatusHandler(func, *filters))
             return func
 
         return decorator
 
     def on_template_status(
-            self: WhatsApp, *filters: Callable[[WhatsApp, TemplateStatus], bool]
-    ) -> Callable[[Callable[[WhatsApp, TemplateStatus], Any]], Callable[[WhatsApp, TemplateStatus], Any]]:
+        self: WhatsApp,
+        *filters: Callable[[WhatsApp, TemplateStatus], bool],
+    ) -> Callable[
+        [Callable[[WhatsApp, TemplateStatus], Any]],
+        Callable[[WhatsApp, TemplateStatus], Any],
+    ]:
         """
         Decorator to register a function as a handler for :class:`pywa.types.TemplateStatus` updates (Template message
         is approved, rejected etc...).
 
         - Shortcut for :func:`~pywa.client.WhatsApp.add_handlers` with a :class:`TemplateStatusHandler`.
 
         Example:
@@ -565,12 +680,16 @@
             ... def approved_handler(client: WhatsApp, status: TemplateStatus):
             ...     print(f"Template {status.message_template_name} just got approved!")
 
         Args:
             *filters: Filters to apply to the incoming template status changes (filters are function that take a
                 :class:`pywa.WhatsApp` instance and the incoming :class:`pywa.types.TemplateStatus` and return :class:`bool`).
         """
+
         @functools.wraps(self.on_template_status)
-        def decorator(func: Callable[[WhatsApp, TemplateStatus], Any]) -> Callable[[WhatsApp, TemplateStatus], Any]:
+        def decorator(
+            func: Callable[[WhatsApp, TemplateStatus], Any]
+        ) -> Callable[[WhatsApp, TemplateStatus], Any]:
             self.add_handlers(TemplateStatusHandler(func, *filters))
             return func
+
         return decorator
```

### Comparing `pywa-1.8.0/pywa/types/__init__.py` & `pywa-1.9.0/pywa/types/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,45 @@
 """
 This package contains all the types used in the library.
 """
 
-from .message import Message
-from .others import (Contact, User, Reaction, Location, Metadata, ReplyToMessage, Order, Product, System,
-                     ProductsSection, CommerceSettings, BusinessProfile, Industry, MessageType)
-from .callback import (CallbackButton, CallbackSelection, Button, SectionRow, Section, SectionList, CallbackData,
-                       ButtonUrl)
-from .message_status import MessageStatus, MessageStatusType, Conversation, ConversationCategory
+from .base_update import StopHandling
+from .callback import (
+    Button,
+    ButtonUrl,
+    CallbackButton,
+    CallbackData,
+    CallbackSelection,
+    Section,
+    SectionList,
+    SectionRow,
+)
 from .media import MediaUrlResponse
-from .template import NewTemplate, TemplateResponse, Template, TemplateStatus
+from .message import Message
+from .message_status import (
+    Conversation,
+    ConversationCategory,
+    MessageStatus,
+    MessageStatusType,
+)
+from .others import (
+    BusinessProfile,
+    CommerceSettings,
+    Contact,
+    Industry,
+    Location,
+    MessageType,
+    Metadata,
+    Order,
+    Product,
+    ProductsSection,
+    Reaction,
+    ReplyToMessage,
+    System,
+    User,
+)
+from .template import (
+    NewTemplate,
+    Template,
+    TemplateResponse,
+    TemplateStatus,
+)
```

### Comparing `pywa-1.8.0/pywa/types/base_update.py` & `pywa-1.9.0/pywa/types/base_update.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,111 @@
 from __future__ import annotations
 
 """This module contains the base types for all update types."""
 
+__all__ = [
+    "StopHandling",
+]
+
 import abc
 import dataclasses
 import datetime as dt
-from typing import Iterable, TYPE_CHECKING, BinaryIO
-from .others import Metadata, User, Contact, ProductsSection
+from typing import TYPE_CHECKING, BinaryIO, Iterable
+
+from .others import Contact, Metadata, ProductsSection, User
 
 if TYPE_CHECKING:
     from pywa.client import WhatsApp
-    from .callback import Button, SectionList, ButtonUrl
+
+    from .callback import Button, ButtonUrl, SectionList
     from .template import Template
 
 
+class StopHandling(Exception):
+    """
+    Raise this exception to stop handling an update.
+
+    You can call ``.stop_handling()`` on every update object to raise this exception.
+
+    Example:
+
+            >>> from pywa import WhatsApp
+            >>> from pywa.types import Message
+            >>> wa = WhatsApp(...)
+
+            >>> @wa.on_message()
+            ... def handler(_: WhatsApp, msg: Message):
+            ...     msg.reply_text("Hello from PyWa!")
+            ...     msg.stop_handling()  # or raise StopHandling
+
+            >>> @wa.on_message()
+            ... def not_called(_: WhatsApp, msg: Message):
+            ...     msg.reply_text("This message will not be sent")
+    """
+
+    pass
+
+
 @dataclasses.dataclass(frozen=True, slots=True, kw_only=True)
 class BaseUpdate(abc.ABC):
     """Base class for all update types."""
+
     _client: WhatsApp = dataclasses.field(repr=False, hash=False, compare=False)
 
     @property
     @abc.abstractmethod
-    def id(self) -> str: ...
+    def id(self) -> str:
+        ...
 
     @property
     @abc.abstractmethod
-    def timestamp(self) -> dt.datetime: ...
+    def timestamp(self) -> dt.datetime:
+        ...
 
     @abc.abstractmethod
-    def from_update(self, client: WhatsApp, update: dict) -> BaseUpdate: ...
+    def from_update(self, client: WhatsApp, update: dict) -> BaseUpdate:
+        ...
+
+    def stop_handling(self) -> None:
+        """
+        Call this method to break out of the handler loop. other handlers will not be called.
+
+        This method just raises :class:`StopHandling` which is caught by the handler loop and breaks out of it.
+
+        Example:
+
+            >>> from pywa import WhatsApp
+            >>> from pywa.types import Message
+            >>> wa = WhatsApp(...)
+
+            >>> @wa.on_message()
+            ... def handler(_: WhatsApp, msg: Message):
+            ...     msg.reply_text("Hello from PyWa!")
+            ...     msg.stop_handling()
+
+            >>> @wa.on_message()
+            ... def not_called(_: WhatsApp, msg: Message):
+            ...     msg.reply_text("This message will not be sent")
+        """
+        raise StopHandling
 
 
 @dataclasses.dataclass(frozen=True, slots=True, kw_only=True)
 class BaseUserUpdate(BaseUpdate, abc.ABC):
     """Base class for all user-related update types (message, callback, etc.)."""
+
     @property
     @abc.abstractmethod
-    def metadata(self) -> Metadata: ...
+    def metadata(self) -> Metadata:
+        ...
 
     @property
     @abc.abstractmethod
-    def from_user(self) -> User: ...
+    def from_user(self) -> User:
+        ...
 
     @property
     def sender(self) -> str:
         """
         The WhatsApp ID of the sender.
             - Shortcut for ``.from_user.wa_id``.
         """
@@ -57,21 +118,22 @@
 
         If you want to ``wa.send_x`` with ``reply_to_message_id`` in order to reply to a message, use this property
         instead of ``id`` to prevent errors.
         """
         return self.id
 
     def reply_text(
-            self,
-            text: str,
-            header: str | None = None,
-            footer: str | None = None,
-            keyboard: Iterable[Button] | ButtonUrl | SectionList | None = None,
-            quote: bool = False,
-            preview_url: bool = False,
+        self,
+        text: str,
+        header: str | None = None,
+        footer: str | None = None,
+        buttons: Iterable[Button] | ButtonUrl | SectionList | None = None,
+        quote: bool = False,
+        preview_url: bool = False,
+        keyboard: None = None,
     ) -> str:
         """
         Reply to the message with text.
             - Shortcut for :py:func:`~pywa.client.WhatsApp.send_message` with ``to`` and ``reply_to_message_id``.
 
         Example:
 
@@ -83,29 +145,29 @@
         Example with keyboard buttons:
 
             >>> from pywa.types import Button
             >>> msg.reply_text(
             ...     header="Hello from PyWa!",
             ...     text="What can I help you with?",
             ...     footer="Powered by PyWa",
-            ...     keyboard=[
+            ...     buttons=[
             ...         Button("Help", data="help"),
             ...         Button("About", data="about"),
             ...     ],
             ...     quote=True
             ... )
 
         Example with a section list:
 
             >>> from pywa.types import SectionList, Section, SectionRow
             >>> msg.reply_text(
             ...     header="Hello from PyWa!",
             ...     text="What can I help you with?",
             ...     footer="Powered by PyWa",
-            ...     keyboard=SectionList(
+            ...     buttons=SectionList(
             ...         button_title="Choose an option",
             ...         sections=[
             ...             Section(
             ...                 title="Help",
             ...                 rows=[
             ...                     SectionRow(
             ...                         title="Help",
@@ -114,15 +176,15 @@
             ...                     ),
             ...                     SectionRow(
             ...                         title="About",
             ...                         callback_data="about",
             ...                         description="Learn more about PyWa",
             ...                     ),
             ...                 ],
-            ...             ),
+            ...            ),
             ...            Section(
             ...                 title="Other",
             ...                 rows=[
             ...                     SectionRow(
             ...                         title="GitHub",
             ...                         callback_data="github",
             ...                         description="View the PyWa GitHub repository",
@@ -132,45 +194,48 @@
             ...         ],
             ...     ),
             ...     quote=True
             ... )
 
         Args:
             text: The text to reply with (markdown allowed, max 4096 characters).
-            header: The header of the reply (if keyboard is provided, optional, up to 60 characters,
+            header: The header of the reply (if buttons are provided, optional, up to 60 characters,
              no markdown allowed).
-            footer: The footer of the reply (if keyboard is provided, optional, up to 60 characters,
+            footer: The footer of the reply (if buttons are provided, optional, up to 60 characters,
              markdown has no effect).
-            keyboard: The keyboard to send with the reply (optional).
+            buttons: The buttons to send with the message (optional).
             quote: Whether to quote the replied message (default: False).
             preview_url: Whether to show a preview of the URL in the message (if any).
+            keyboard: Deprecated and will be removed in a future version, use ``buttons`` instead.
 
         Returns:
             The ID of the sent reply.
         """
         return self._client.send_message(
             to=self.sender,
             text=text,
             header=header,
             footer=footer,
-            keyboard=keyboard,
+            buttons=buttons,
             reply_to_message_id=self.message_id_to_reply if quote else None,
             preview_url=preview_url,
+            keyboard=keyboard,
         )
+
     reply = reply_text  # alias
 
     def reply_image(
-            self,
-            image: str | bytes | BinaryIO,
-            caption: str | None = None,
-            body: str | None = None,
-            footer: str | None = None,
-            buttons: Iterable[Button] | ButtonUrl | None = None,
-            quote: bool = False,
-            mime_type: str | None = None,
+        self,
+        image: str | bytes | BinaryIO,
+        caption: str | None = None,
+        body: str | None = None,
+        footer: str | None = None,
+        buttons: Iterable[Button] | ButtonUrl | None = None,
+        quote: bool = False,
+        mime_type: str | None = None,
     ) -> str:
         """
         Reply to the message with an image.
             - Shortcut for :py:func:`~pywa.client.WhatsApp.send_image` with ``to`` and ``reply_to_message_id``.
             - Images must be 8-bit, RGB or RGBA.
 
         Example:
@@ -183,15 +248,15 @@
 
         Args:
             image: The image to reply with (either a media ID, URL, file path, bytes, or an open file object. When
              buttons are provided, only URL is supported).
             caption: The caption of the image (optional, markdown allowed).
             body: The body of the reply (optional, up to 1024 characters, markdown allowed,
              if buttons are provided and body is not provided, caption will be used as the body)
-            footer: The footer of the reply (if buttons is provided, optional, markdown has no effect).
+            footer: The footer of the reply (if buttons are provided, optional, markdown has no effect).
             buttons: The buttons to send with the image (optional).
             quote: Whether to quote the replied message (default: False).
             mime_type: The mime type of the image (optional, required when sending a image as bytes or a file object,
              or file path that does not have an extension).
 
         Returns:
             The ID of the sent reply.
@@ -200,26 +265,26 @@
             to=self.sender,
             image=image,
             caption=caption,
             body=body,
             footer=footer,
             buttons=buttons,
             reply_to_message_id=self.message_id_to_reply if quote else None,
-            mime_type=mime_type
+            mime_type=mime_type,
         )
 
     def reply_video(
-            self,
-            video: str | bytes | BinaryIO,
-            caption: str | None = None,
-            body: str | None = None,
-            footer: str | None = None,
-            buttons: Iterable[Button] | ButtonUrl | None = None,
-            quote: bool = False,
-            mime_type: str | None = None,
+        self,
+        video: str | bytes | BinaryIO,
+        caption: str | None = None,
+        body: str | None = None,
+        footer: str | None = None,
+        buttons: Iterable[Button] | ButtonUrl | None = None,
+        quote: bool = False,
+        mime_type: str | None = None,
     ) -> str:
         """
         Reply to the message with a video.
             - Shortcut for :py:func:`~pywa.client.WhatsApp.send_video` with ``to`` and ``reply_to_message_id``.
             - Only H.264 video codec and AAC audio codec is supported.
             - Videos with a single audio stream or no audio stream are supported.
 
@@ -250,27 +315,27 @@
             to=self.sender,
             video=video,
             caption=caption,
             reply_to_message_id=self.message_id_to_reply if quote else None,
             buttons=buttons,
             body=body,
             footer=footer,
-            mime_type=mime_type
+            mime_type=mime_type,
         )
 
     def reply_document(
-            self,
-            document: str | bytes | BinaryIO,
-            filename: str | None = None,
-            caption: str | None = None,
-            body: str | None = None,
-            footer: str | None = None,
-            buttons: Iterable[Button] | ButtonUrl | None = None,
-            quote: bool = False,
-            mime_type: str | None = None,
+        self,
+        document: str | bytes | BinaryIO,
+        filename: str | None = None,
+        caption: str | None = None,
+        body: str | None = None,
+        footer: str | None = None,
+        buttons: Iterable[Button] | ButtonUrl | None = None,
+        quote: bool = False,
+        mime_type: str | None = None,
     ) -> str:
         """
         Reply to the message with a document.
             - Shortcut for :py:func:`~pywa.client.WhatsApp.send_document` with ``to`` and ``reply_to_message_id``.
 
         Example:
 
@@ -304,21 +369,21 @@
             document=document,
             filename=filename,
             caption=caption,
             reply_to_message_id=self.message_id_to_reply if quote else None,
             buttons=buttons,
             body=body,
             footer=footer,
-            mime_type=mime_type
+            mime_type=mime_type,
         )
 
     def reply_audio(
-            self,
-            audio: str | bytes | BinaryIO,
-            mime_type: str | None = None,
+        self,
+        audio: str | bytes | BinaryIO,
+        mime_type: str | None = None,
     ) -> str:
         """
         Reply to the message with an audio.
             - Shortcut for :py:func:`~pywa.client.WhatsApp.send_audio` with ``to`` and ``reply_to_message_id``.
 
         Example:
 
@@ -337,17 +402,17 @@
         return self._client.send_audio(
             to=self.sender,
             audio=audio,
             mime_type=mime_type,
         )
 
     def reply_sticker(
-            self,
-            sticker: str | bytes | BinaryIO,
-            mime_type: str | None = None,
+        self,
+        sticker: str | bytes | BinaryIO,
+        mime_type: str | None = None,
     ) -> str:
         """
         Reply to the message with a sticker.
             - Shortcut for :py:func:`~pywa.client.WhatsApp.send_sticker` with ``to`` and ``reply_to_message_id``.
             - A static sticker needs to be 512x512 pixels and cannot exceed 100 KB.
             - An animated sticker must be 512x512 pixels and cannot exceed 500 KB.
 
@@ -368,19 +433,19 @@
         return self._client.send_sticker(
             to=self.sender,
             sticker=sticker,
             mime_type=mime_type,
         )
 
     def reply_location(
-            self,
-            latitude: float,
-            longitude: float,
-            name: str | None = None,
-            address: str | None = None,
+        self,
+        latitude: float,
+        longitude: float,
+        name: str | None = None,
+        address: str | None = None,
     ) -> str:
         """
         Reply to the message with a location.
             - Shortcut for :py:func:`~pywa.client.WhatsApp.send_location` with ``to`` and ``reply_to_message_id``.
 
         Example:
 
@@ -402,21 +467,21 @@
             The ID of the sent reply.
         """
         return self._client.send_location(
             to=self.sender,
             latitude=latitude,
             longitude=longitude,
             name=name,
-            address=address
+            address=address,
         )
 
     def reply_contact(
-            self,
-            contact: Contact | Iterable[Contact],
-            quote: bool = False,
+        self,
+        contact: Contact | Iterable[Contact],
+        quote: bool = False,
     ) -> str:
         """
         Reply to the message with a contact/s.
             - Shortcut for :py:func:`~pywa.client.WhatsApp.send_contact` with ``to`` and ``reply_to_message_id``.
 
         Example:
 
@@ -438,15 +503,15 @@
 
         Returns:
             The ID of the sent reply.
         """
         return self._client.send_contact(
             to=self.sender,
             contact=contact,
-            reply_to_message_id=self.message_id_to_reply if quote else None
+            reply_to_message_id=self.message_id_to_reply if quote else None,
         )
 
     def react(self, emoji: str) -> str:
         """
         React to the message with an emoji.
             - Shortcut for :py:func:`~pywa.client.WhatsApp.send_reaction` with ``to`` and ``message_id``.
 
@@ -459,15 +524,15 @@
 
         Returns:
             The ID of the sent reaction.
         """
         return self._client.send_reaction(
             to=self.sender,
             emoji=emoji,
-            message_id=self.message_id_to_reply
+            message_id=self.message_id_to_reply,
         )
 
     def unreact(self) -> str:
         """
         Remove the reaction from the message.
             - Shortcut for :py:func:`~pywa.client.WhatsApp.remove_reaction` with ``to`` and ``message_id``.
 
@@ -475,24 +540,23 @@
 
             >>> msg.unreact()
 
         Returns:
             The ID of the sent unreaction.
         """
         return self._client.remove_reaction(
-            to=self.sender,
-            message_id=self.message_id_to_reply
+            to=self.sender, message_id=self.message_id_to_reply
         )
 
     def reply_catalog(
-            self,
-            body: str,
-            footer: str | None = None,
-            thumbnail_product_sku: str | None = None,
-            quote: bool = False,
+        self,
+        body: str,
+        footer: str | None = None,
+        thumbnail_product_sku: str | None = None,
+        quote: bool = False,
     ) -> str:
         """
         Reply to the message with a catalog.
             - Shortcut for :py:func:`~pywa.client.WhatsApp.send_catalog` with ``to`` and ``reply_to_message_id``.
 
         Example:
 
@@ -513,24 +577,24 @@
             The ID of the sent reply.
         """
         return self._client.send_catalog(
             to=self.sender,
             body=body,
             footer=footer,
             thumbnail_product_sku=thumbnail_product_sku,
-            reply_to_message_id=self.message_id_to_reply if quote else None
+            reply_to_message_id=self.message_id_to_reply if quote else None,
         )
 
     def reply_product(
-            self,
-            catalog_id: str,
-            sku: str,
-            body: str | None = None,
-            footer: str | None = None,
-            quote: bool = False,
+        self,
+        catalog_id: str,
+        sku: str,
+        body: str | None = None,
+        footer: str | None = None,
+        quote: bool = False,
     ) -> str:
         """
         Reply to the message with a product.
             - Shortcut for :py:func:`~pywa.client.WhatsApp.send_product` with ``to`` and ``reply_to_message_id``.
             - To reply with multiple products, use :py:func:`~BaseUserUpdate.reply_products`.
 
         Args:
@@ -547,25 +611,25 @@
         """
         return self._client.send_product(
             to=self.sender,
             catalog_id=catalog_id,
             sku=sku,
             body=body,
             footer=footer,
-            reply_to_message_id=self.message_id_to_reply if quote else None
+            reply_to_message_id=self.message_id_to_reply if quote else None,
         )
 
     def reply_products(
-            self,
-            catalog_id: str,
-            product_sections: Iterable[ProductsSection],
-            title: str,
-            body: str,
-            footer: str | None = None,
-            quote: bool = False,
+        self,
+        catalog_id: str,
+        product_sections: Iterable[ProductsSection],
+        title: str,
+        body: str,
+        footer: str | None = None,
+        quote: bool = False,
     ) -> str:
         """
         Reply to the message with a product.
             - Shortcut for :py:func:`~pywa.client.WhatsApp.send_products` with ``to`` and ``reply_to_message_id``.
             - To reply with multiple products, use :py:func:`~BaseUserUpdate.reply_products`.
 
         Example:
@@ -605,21 +669,21 @@
         return self._client.send_products(
             to=self.sender,
             catalog_id=catalog_id,
             product_sections=product_sections,
             title=title,
             body=body,
             footer=footer,
-            reply_to_message_id=self.message_id_to_reply if quote else None
+            reply_to_message_id=self.message_id_to_reply if quote else None,
         )
 
     def reply_template(
-            self,
-            template: Template,
-            quote: bool = False,
+        self,
+        template: Template,
+        quote: bool = False,
     ) -> str:
         """
         Reply to the message with a template.
 
         -- Shortcut for :py:func:`~pywa.client.WhatsApp.send_template` with ``to`` and ``reply_to_message_id``.
 
         Example:
@@ -664,25 +728,21 @@
         Returns:
             The ID of the sent reply.
 
         Raises:
 
         """
         return self._client.send_template(
-               to=self.sender,
-               template=template,
-               reply_to_message_id=quote if quote else None
-           )
-
-    def mark_as_read(
-            self
-    ) -> bool:
+            to=self.sender,
+            template=template,
+            reply_to_message_id=quote if quote else None,
+        )
+
+    def mark_as_read(self) -> bool:
         """
         Mark the message as read.
             - Shortcut for :py:func:`~pywa.client.WhatsApp.mark_message_as_read` with ``message_id``.
 
         Returns:
             Whether it was successful.
         """
-        return self._client.mark_message_as_read(
-            message_id=self.message_id_to_reply
-        )
+        return self._client.mark_message_as_read(message_id=self.message_id_to_reply)
```

### Comparing `pywa-1.8.0/pywa/types/callback.py` & `pywa-1.9.0/pywa/types/callback.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 """This module contains the callback types."""
 
 __all__ = [
-    'CallbackButton',
-    'CallbackSelection',
-    'Button',
-    'ButtonUrl',
-    'SectionRow',
-    'Section',
-    'SectionList',
-    'CallbackData',
-    'CallbackDataT'
+    "CallbackButton",
+    "CallbackSelection",
+    "Button",
+    "ButtonUrl",
+    "SectionRow",
+    "Section",
+    "SectionList",
+    "CallbackData",
+    "CallbackDataT",
 ]
 
 import dataclasses
 import datetime as dt
 import enum
-from typing import TYPE_CHECKING, Iterable, TypeVar, Generic, Any
+from typing import TYPE_CHECKING, Any, Generic, Iterable, TypeVar
+
 from .base_update import BaseUserUpdate
-from .others import Metadata, User, ReplyToMessage, MessageType
+from .others import MessageType, Metadata, ReplyToMessage, User
 
 if TYPE_CHECKING:
-    from .template import Template
     from pywa.client import WhatsApp
 
+    from .template import Template
+
 
 class CallbackData:
     """
     Base class for all callback data classes. Subclass this class to create a type-safe callback data class.
 
         If you use ``dataclasses``, which is the recommended way (You get free ordered ``__init__`` and extra features),
         you should not use ``kw_only=True``.
@@ -57,97 +59,125 @@
 
         >>> from pywa import WhatsApp
         >>> from pywa.types import Button
         >>> wa = WhatsApp(...)
         >>> wa.send_message(
         ...     to='972987654321',
         ...     text='Click the button to get the user',
-        ...     keyboard=[Button(title='Get user', callback_data=UserData(id=123, admin=True))]
+        ...     buttons=[Button(title='Get user', callback_data=UserData(id=123, admin=True))]
         ... )
 
         >>> @wa.on_callback_button(factory=UserData) # Use the factory parameter to convert the callback data
         ... def on_user_data(client: WhatsApp, btn: CallbackButton[UserData]): # For autocomplete
         ...    if btn.data.admin: print(btn.data.id) # Access the data object as an attribute
     """
+
     __callback_id__: int = 0
     """Unique ID for each callback data class. Do not override this."""
-    __callback_sep__: str = '¶'
+    __callback_sep__: str = "¶"
     """The separator between multiple callback objects, Can be overridden globally. (Default ``¶``)"""
-    __callback_data_sep__: str = '~'
+    __callback_data_sep__: str = "~"
     """The separator between the callback fields, Can be overridden individually. (Default ``~``)"""
     __allowed_types__: tuple[type, ...] = (str, int, bool, float)
     """The allowed types in the callback data."""
 
     def __init_subclass__(cls, **kwargs):
         """Validate the callback data class and set a unique ID for it."""
         super().__init_subclass__(**kwargs)
         if not (annotations := cls.__annotations__.items()):
-            raise TypeError(f"Callback data class {cls.__name__} must have at least one field.")
+            raise TypeError(
+                f"Callback data class {cls.__name__} must have at least one field."
+            )
         if unsupported_fields := {
-            (field_name, field_type) for field_name, field_type in annotations
+            (field_name, field_type)
+            for field_name, field_type in annotations
             if not issubclass(field_type, (types := cls.__allowed_types__))
         }:
-            raise TypeError(f"Unsupported types {unsupported_fields} in callback data. Use one of {types}.")
+            raise TypeError(
+                f"Unsupported types {unsupported_fields} in callback data. Use one of {types}."
+            )
         cls.__callback_id__ = CallbackData.__callback_id__
         CallbackData.__callback_id__ += 1
 
     @classmethod
     def from_str(
-            cls,
-            data: str,
-    ) -> 'CallbackData':
+        cls,
+        data: str,
+    ) -> "CallbackData":
         """
         Internal function to convert a callback string to a callback object.
         """
         try:
             # noinspection PyArgumentList
-            return cls(*(
-                annotation(value) for annotation, value in zip(
-                    cls.__annotations__.values(),
-                    data.split(cls.__callback_data_sep__)[1:],
-                    strict=True
+            return cls(
+                *(
+                    annotation(value)
+                    for annotation, value in zip(
+                        cls.__annotations__.values(),
+                        data.split(cls.__callback_data_sep__)[1:],
+                        strict=True,
+                    )
                 )
-            ))
+            )
         except (ValueError, TypeError) as e:
             raise ValueError(f"Invalid callback data for {cls.__name__}: {data}") from e
 
     @staticmethod
     def _not_contains(value: Any, *not_) -> str:
         """Internal function to validate that the value does not contain the separator."""
         if any(sep in (str_val := str(value)) for sep in not_):
-            raise ValueError(f"Callback data cannot contain the characters {not_} "
-                             f"Because they are used as separators. \nYou can change the separators by overriding "
-                             f"``__callback_data_sep__`` (for individual objects) and ``CallbackData.__callback_sep__`` "
-                             f"(In the base class level, affects all child classes).")
+            raise ValueError(
+                f"Callback data cannot contain the characters {not_} "
+                f"Because they are used as separators. \nYou can change the separators by overriding "
+                f"``__callback_data_sep__`` (for individual objects) and ``CallbackData.__callback_sep__`` "
+                f"(In the base class level, affects all child classes)."
+            )
         return str_val
 
     def to_str(self) -> str:
         """
         Internal function to convert a callback object to a callback string.
         """
-        return self.__callback_data_sep__.join((str(self.__callback_id__), *(
-            self._not_contains(getattr(self, field_name), self.__callback_sep__, self.__callback_data_sep__)
-            if not issubclass(field_type, (bool, enum.Enum)) else ('§' if getattr(self, field_name) else '')
-            if field_type is bool else self._not_contains(
-                getattr(self, field_name).value, self.__callback_sep__, self.__callback_data_sep__
+        return self.__callback_data_sep__.join(
+            (
+                str(self.__callback_id__),
+                *(
+                    self._not_contains(
+                        getattr(self, field_name),
+                        self.__callback_sep__,
+                        self.__callback_data_sep__,
+                    )
+                    if not issubclass(field_type, (bool, enum.Enum))
+                    else ("§" if getattr(self, field_name) else "")
+                    if field_type is bool
+                    else self._not_contains(
+                        getattr(self, field_name).value,
+                        self.__callback_sep__,
+                        self.__callback_data_sep__,
+                    )
+                    for field_name, field_type in self.__annotations__.items()
+                ),
             )
-            for field_name, field_type in self.__annotations__.items()
-        )))
+        )
 
     @classmethod
     def join_to_str(cls, *datas: Any) -> str:
         """Internal function to join multiple callback objects to a callback string."""
         return cls.__callback_sep__.join(
-            data.to_str() if isinstance(data, CallbackData)
+            data.to_str()
+            if isinstance(data, CallbackData)
             else cls._not_contains(data, cls.__callback_data_sep__)
             for data in datas
         )
 
 
-CallbackDataT = TypeVar('CallbackDataT', bound=str | CallbackData | Iterable[CallbackData | Any])
+CallbackDataT = TypeVar(
+    "CallbackDataT",
+    bound=str | CallbackData | Iterable[CallbackData | Any],
+)
 """Type hint for ``callback_data`` parameter in :class:`Button` and :class:`SectionRow`."""
 
 
 @dataclasses.dataclass(frozen=True, slots=True, kw_only=True)
 class CallbackButton(BaseUserUpdate, Generic[CallbackDataT]):
     """
     Represents a callback button.
@@ -167,15 +197,15 @@
 
         >>> from pywa import WhatsApp
         >>> from pywa.types import Button, CallbackButton
         >>> wa = WhatsApp(...)
         >>> wa.send_message(
         ...     to='972987654321',
         ...     text='Click the button to get the user',
-        ...     keyboard=[Button(title='Get user', callback_data=UserData(id=123, name='david', admin=True))]
+        ...     buttons=[Button(title='Get user', callback_data=UserData(id=123, name='david', admin=True))]
         ... )                                     # Here ^^^ we use the UserData class as the callback data
 
         >>> @wa.on_callback_button(factory=UserData) # Use the factory parameter to convert the callback data
         ... def on_user_data(_: WhatsApp, btn: CallbackButton[UserData]): # For autocomplete
         ...    if btn.data.admin: print(btn.data.id) # Access the data object as an attribute
 
     You can even use multiple factories, and not only ``CallbackData`` subclasses!
@@ -184,15 +214,15 @@
         >>> class State(str, Enum):
         ...     START = 's'
         ...     END = 'e'
 
         >>> wa.send_message(
         ...     to='972987654321',
         ...     text='Click the button to get the user and state',
-        ...     keyboard=[Button(title='Get user', callback_data=(UserData(id=123, name='david', admin=True), State.START))]
+        ...     buttons=[Button(title='Get user', callback_data=(UserData(id=123, name='david', admin=True), State.START))]
         ... )                                     # Here ^^^ we send a tuple of UserData and State
 
         >>> @wa.on_callback_button(factory=(UserData, State)) # Use the factory parameter to convert the callback data
         ... def on_user_data(_: WhatsApp, btn: CallbackButton[tuple[UserData, State]]): # For autocomplete
         ...    user, state = btn.data # Unpack the tuple
         ...    if user.admin: print(user.id, state)
 
@@ -206,45 +236,46 @@
         from_user: The user who sent the message.
         timestamp: The timestamp when the message was sent.
         reply_to_message: The message to which this callback button is a reply to.
         data: The data of the button (the ``callback_data`` parameter you provided in :class:`Button` or
          :class:`Template.QuickReplyButtonData`).
         title: The title of the button.
     """
+
     id: str
     type: MessageType
     metadata: Metadata
     from_user: User
     timestamp: dt.datetime
     reply_to_message: ReplyToMessage
     data: CallbackDataT
     title: str
 
     @classmethod
-    def from_update(cls, client: 'WhatsApp', update: dict) -> 'CallbackButton':
-        msg = (value := update['entry'][0]['changes'][0]['value'])['messages'][0]
-        match (msg_type := msg['type']):
+    def from_update(cls, client: "WhatsApp", update: dict) -> "CallbackButton":
+        msg = (value := update["entry"][0]["changes"][0]["value"])["messages"][0]
+        match msg_type := msg["type"]:
             case MessageType.INTERACTIVE:
-                title = msg['interactive']['button_reply']['title']
-                data = msg['interactive']['button_reply']['id']
+                title = msg["interactive"]["button_reply"]["title"]
+                data = msg["interactive"]["button_reply"]["id"]
             case MessageType.BUTTON:
-                title = msg['button']['text']
-                data = msg['button']['payload']
+                title = msg["button"]["text"]
+                data = msg["button"]["payload"]
             case _:
                 raise ValueError(f"Invalid message type {msg_type}")
         return cls(
             _client=client,
-            id=msg['id'],
-            metadata=Metadata.from_dict(value['metadata']),
+            id=msg["id"],
+            metadata=Metadata.from_dict(value["metadata"]),
             type=MessageType(msg_type),
-            from_user=User.from_dict(value['contacts'][0]),
-            timestamp=dt.datetime.fromtimestamp(int(msg['timestamp'])),
-            reply_to_message=ReplyToMessage.from_dict(msg['context']),
+            from_user=User.from_dict(value["contacts"][0]),
+            timestamp=dt.datetime.fromtimestamp(int(msg["timestamp"])),
+            reply_to_message=ReplyToMessage.from_dict(msg["context"]),
             data=data,
-            title=title
+            title=title,
         )
 
 
 @dataclasses.dataclass(frozen=True, slots=True, kw_only=True)
 class CallbackSelection(BaseUserUpdate, Generic[CallbackDataT]):
     """
     Represents a callback selection.
@@ -264,15 +295,15 @@
 
         >>> from pywa import WhatsApp
         >>> from pywa.types import SectionList, Section, SectionRow, CallbackSelection
         >>> wa = WhatsApp(...)
         >>> wa.send_message(
         ...     to='972987654321',
         ...     text='Click the button to get the user',
-        ...     keyboard=SectionList(
+        ...     buttons=SectionList(
         ...         button_title='Get user', sections=[
         ...             Section(title='Users', rows=[
         ...                 SectionRow(title='Get user', callback_data=UserData(id=123, name='david', admin=True))
         ...             ])                              # Here ^^^ we use the UserData class as the callback data
         ...         ]
         ...     )
         ... )
@@ -287,15 +318,15 @@
         >>> class State(str, Enum):
         ...     START = 's'
         ...     END = 'e'
 
         >>> wa.send_message(
         ...     to='972987654321',
         ...     text='Click the button to get the user and state',
-        ...     keyboard=SectionList(
+        ...     buttons=SectionList(
         ...         button_title='Get user', sections=[
         ...             Section(title='Users', rows=[
         ...                 SectionRow(title='Get user', callback_data=(UserData(id=123, name='david', admin=True), State.START))
         ...             ])                              # Here ^^^ we send a tuple of UserData and State
         ...         ]
         ...     )
         ... )
@@ -312,38 +343,39 @@
         from_user: The user who sent the message.
         timestamp: The timestamp when the message was sent.
         reply_to_message: The message to which this callback selection is a reply to.
         data: The data of the selection (the ``callback_data`` parameter you provided in :class:`SectionRow`).
         title: The title of the selection.
         description: The description of the selection (optional).
     """
+
     id: str
     type: MessageType
     metadata: Metadata
     from_user: User
     timestamp: dt.datetime
     reply_to_message: ReplyToMessage
     data: CallbackDataT
     title: str
     description: str | None
 
     @classmethod
-    def from_update(cls, client: 'WhatsApp', update: dict) -> 'CallbackSelection':
-        msg = (value := update['entry'][0]['changes'][0]['value'])['messages'][0]
+    def from_update(cls, client: "WhatsApp", update: dict) -> "CallbackSelection":
+        msg = (value := update["entry"][0]["changes"][0]["value"])["messages"][0]
         return cls(
             _client=client,
-            id=msg['id'],
-            metadata=Metadata.from_dict(value['metadata']),
-            type=MessageType(msg['type']),
-            from_user=User.from_dict(value['contacts'][0]),
-            timestamp=dt.datetime.fromtimestamp(int(msg['timestamp'])),
-            reply_to_message=ReplyToMessage.from_dict(msg['context']),
-            data=msg['interactive']['list_reply']['id'],
-            title=msg['interactive']['list_reply']['title'],
-            description=msg['interactive']['list_reply'].get('description')
+            id=msg["id"],
+            metadata=Metadata.from_dict(value["metadata"]),
+            type=MessageType(msg["type"]),
+            from_user=User.from_dict(value["contacts"][0]),
+            timestamp=dt.datetime.fromtimestamp(int(msg["timestamp"])),
+            reply_to_message=ReplyToMessage.from_dict(msg["context"]),
+            data=msg["interactive"]["list_reply"]["id"],
+            title=msg["interactive"]["list_reply"]["title"],
+            description=msg["interactive"]["list_reply"].get("description"),
         )
 
 
 def _resolve_callback_data(data: CallbackDataT) -> str:
     """Internal function to convert callback data to a string."""
     if isinstance(data, str):
         return data
@@ -361,68 +393,68 @@
     Represents a button in the button list.
 
     Attributes:
         title: The title of the button (up to 20 characters).
         callback_data: The data to send when the user clicks on the button (up to 256 characters, for complex data
          You can use :class:`CallbackData`).
     """
+
     title: str
     callback_data: CallbackDataT
 
     def to_dict(self) -> dict:
         return {
             "type": "reply",
             "reply": {
                 "id": _resolve_callback_data(self.callback_data),
-                "title": self.title
-            }
+                "title": self.title,
+            },
         }
 
 
 @dataclasses.dataclass(frozen=True, slots=True)
 class ButtonUrl:
     """
     Represents a button in the bottom of the message that opens a URL.
 
     Attributes:
         title: The title of the button (up to 20 characters).
         url: The URL to open when the user clicks on the button.
     """
+
     title: str
     url: str
 
     def to_dict(self) -> dict:
         return {
             "name": "cta_url",
-            "parameters": {
-                "display_text": self.title,
-                "url": self.url
-            }
+            "parameters": {"display_text": self.title, "url": self.url},
         }
 
 
 @dataclasses.dataclass(frozen=True, slots=True)
 class SectionRow:
     """
     Represents a row in a section.
 
     Attributes:
         title: The title of the row (up to 24 characters).
         callback_data: The payload to send when the user clicks on the row (up to 200 characters, for complex data
             You can use :class:`CallbackData`).
         description: The description of the row (optional, up to 72 characters).
     """
+
     title: str
     callback_data: CallbackDataT
     description: str | None = None
 
     def to_dict(self) -> dict:
         d = {
             "id": _resolve_callback_data(self.callback_data),
-            "title": self.title
+            "title": self.title,
         }
         if self.description:
             d["description"] = self.description
         return d
 
 
 @dataclasses.dataclass(frozen=True, slots=True)
@@ -430,34 +462,36 @@
     """
     Represents a section in a section list.
 
     Attributes:
         title: The title of the section (up to 24 characters).
         rows: The rows in the section (at least 1, no more than 10).
     """
+
     title: str
     rows: Iterable[SectionRow]
 
     def to_dict(self) -> dict:
         return {
             "title": self.title,
-            "rows": tuple(row.to_dict() for row in self.rows)
+            "rows": tuple(row.to_dict() for row in self.rows),
         }
 
 
 @dataclasses.dataclass(frozen=True, slots=True)
 class SectionList:
     """
     Represents a section list in an interactive message.
 
     Attributes:
         button_title: The title of the button that opens the section list (up to 20 characters).
         sections: The sections in the section list (at least 1, no more than 10).
     """
+
     button_title: str
     sections: Iterable[Section]
 
     def to_dict(self) -> dict:
         return {
             "button": self.button_title,
-            "sections": tuple(section.to_dict() for section in self.sections)
+            "sections": tuple(section.to_dict() for section in self.sections),
         }
```

### Comparing `pywa-1.8.0/pywa/types/media.py` & `pywa-1.9.0/pywa/types/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,62 +1,66 @@
 from __future__ import annotations
 
 """This module contains the types related to media."""
 
 __all__ = [
-    'Image',
-    'Video',
-    'Sticker',
-    'Document',
-    'Audio',
-    'MediaUrlResponse'
+    "Image",
+    "Video",
+    "Sticker",
+    "Document",
+    "Audio",
+    "MediaUrlResponse",
 ]
 
-import mimetypes
-import dataclasses
 import abc
+import dataclasses
+import mimetypes
 from typing import TYPE_CHECKING
+
 from pywa import utils
 
 if TYPE_CHECKING:
     from pywa.client import WhatsApp
 
 
 @dataclasses.dataclass(frozen=True, slots=True, kw_only=True)
 class MediaBase(abc.ABC, utils.FromDict):
     """Base class for all media types."""
 
     _client: WhatsApp = dataclasses.field(repr=False, hash=False, compare=False)
 
     @property
     @abc.abstractmethod
-    def id(self) -> str: ...
+    def id(self) -> str:
+        ...
 
     @property
     @abc.abstractmethod
-    def sha256(self) -> str: ...
+    def sha256(self) -> str:
+        ...
 
     @property
     @abc.abstractmethod
-    def mime_type(self) -> str: ...
+    def mime_type(self) -> str:
+        ...
 
     def get_media_url(self) -> str:
         """Gets the URL of the media. (expires after 5 minutes)"""
         return self._client.get_media_url(media_id=self.id).url
 
     @property
     def extension(self) -> str | None:
         """Gets the extension of the media (with dot.)"""
         return mimetypes.guess_extension(self.mime_type)
 
     def download(
-            self,
-            path: str | None = None,
-            filename: str | None = None,
-            in_memory: bool = False,
+        self,
+        path: str | None = None,
+        filename: str | None = None,
+        in_memory: bool = False,
     ) -> bytes | str:
         """
         Download a media file from WhatsApp servers.
             - Same as :func:`~pywa.client.WhatsApp.download_media` with ``media_url=media.get_media_url()``
 
         >>> message.image.download()
 
@@ -68,28 +72,29 @@
         Returns:
             The path of the saved file if ``in_memory`` is False, the file as bytes otherwise.
         """
         return self._client.download_media(
             url=self.get_media_url(),
             path=path,
             filename=filename,
-            in_memory=in_memory
+            in_memory=in_memory,
         )
 
 
 @dataclasses.dataclass(frozen=True, slots=True, kw_only=True)
 class Image(MediaBase):
     """
     Represents an image.
 
     Attributes:
         id: The ID of the image.
         sha256: The SHA256 hash of the image.
         mime_type: The MIME type of the image.
     """
+
     id: str
     sha256: str
     mime_type: str
 
 
 @dataclasses.dataclass(frozen=True, slots=True, kw_only=True)
 class Video(MediaBase):
@@ -97,14 +102,15 @@
     Represents a video.
 
     Attributes:
         id: The ID of the video.
         sha256: The SHA256 hash of the video.
         mime_type: The MIME type of the video.
     """
+
     id: str
     sha256: str
     mime_type: str
 
 
 @dataclasses.dataclass(frozen=True, slots=True, kw_only=True)
 class Sticker(MediaBase):
@@ -113,14 +119,15 @@
 
     Attributes:
         id: The ID of the sticker.
         sha256: The SHA256 hash of the sticker.
         mime_type: The MIME type of the sticker.
         animated: Whether the sticker is animated.
     """
+
     id: str
     sha256: str
     mime_type: str
     animated: bool
 
 
 @dataclasses.dataclass(frozen=True, slots=True, kw_only=True)
@@ -130,14 +137,15 @@
 
     Attributes:
         id: The ID of the document.
         sha256: The SHA256 hash of the document.
         mime_type: The MIME type of the document.
         filename: The filename of the document (optional).
     """
+
     id: str
     sha256: str
     mime_type: str
     filename: str | None = None
 
 
 @dataclasses.dataclass(frozen=True, slots=True, kw_only=True)
@@ -147,14 +155,15 @@
 
     Attributes:
         id: The ID of the audio.
         sha256: The SHA256 hash of the audio.
         mime_type: The MIME type of the audio.
         voice: Whether the audio is a voice message or just an audio file.
     """
+
     id: str
     sha256: str
     mime_type: str
     voice: bool
 
 
 @dataclasses.dataclass(frozen=True, slots=True)
@@ -165,32 +174,38 @@
     Attributes:
         id: The ID of the media.
         url: The URL of the media (valid for 5 minutes).
         mime_type: The MIME type of the media.
         sha256: The SHA256 hash of the media.
         file_size: The size of the media in bytes.
     """
+
     _client: WhatsApp = dataclasses.field(repr=False, hash=False, compare=False)
     id: str
     url: str
     mime_type: str
     sha256: str
     file_size: int
 
     def download(
-            self,
-            filepath: str | None = None,
-            filename: str | None = None,
-            in_memory: bool = False,
+        self,
+        filepath: str | None = None,
+        filename: str | None = None,
+        in_memory: bool = False,
     ) -> bytes | str:
         """
         Download a media file from WhatsApp servers.
 
         Args:
             filepath: The path where to save the file (if not provided, the current working directory will be used).
             filename: The name of the file (if not provided, it will be guessed from the URL + extension).
             in_memory: Whether to return the file as bytes instead of saving it to disk (default: False).
 
         Returns:
             The path of the saved file if ``in_memory`` is False, the file as bytes otherwise.
         """
-        return self._client.download_media(url=self.url, path=filepath, filename=filename, in_memory=in_memory)
+        return self._client.download_media(
+            url=self.url,
+            path=filepath,
+            filename=filename,
+            in_memory=in_memory,
+        )
```

### Comparing `pywa-1.8.0/pywa/types/message.py` & `pywa-1.9.0/pywa/types/message.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,62 @@
 from __future__ import annotations
 
 """This module contains the types related to messages."""
 
-__all__ = ['Message']
+__all__ = ["Message"]
 
 import dataclasses
 import datetime as dt
-from typing import TYPE_CHECKING, Callable, Any, Iterable
+from typing import TYPE_CHECKING, Any, Callable, Iterable
+
 from pywa.errors import WhatsAppError
-from .callback import Button, SectionList, ButtonUrl
+
 from .base_update import BaseUserUpdate
+from .callback import Button, ButtonUrl, SectionList
+from .media import Audio, Document, Image, Sticker, Video
 from .others import (
-    ReplyToMessage, Reaction, Location, Contact, User, Metadata, Order, System, MessageType, ProductsSection
+    Contact,
+    Location,
+    MessageType,
+    Metadata,
+    Order,
+    ProductsSection,
+    Reaction,
+    ReplyToMessage,
+    System,
+    User,
 )
-from .media import Image, Video, Sticker, Document, Audio
 
 if TYPE_CHECKING:
     from pywa.client import WhatsApp
 
 
 _FIELDS_TO_OBJECTS_CONSTRUCTORS: dict[str, Callable[[dict, WhatsApp], Any]] = dict(
-    text=lambda m, _client: m['body'],
+    text=lambda m, _client: m["body"],
     image=Image.from_dict,
     video=Video.from_dict,
     sticker=Sticker.from_dict,
     document=Document.from_dict,
     audio=Audio.from_dict,
     reaction=Reaction.from_dict,
     location=Location.from_dict,
     contacts=lambda m, _client: tuple(Contact.from_dict(c) for c in m),
     order=Order.from_dict,
     system=System.from_dict,
 )
 
-_MEDIA_FIELDS = ('image', 'video', 'sticker', 'document', 'audio')
+_MEDIA_FIELDS = ("image", "video", "sticker", "document", "audio")
 
 
 @dataclasses.dataclass(frozen=True, slots=True, kw_only=True)
 class Message(BaseUserUpdate):
     """
     A message received from a user.
 
-    - `\`Message\` on developers.facebook.com <https://developers.facebook.com/docs/whatsapp/cloud-api/webhooks/components#messages-object>`_
+    - `'Message' on developers.facebook.com <https://developers.facebook.com/docs/whatsapp/cloud-api/webhooks/components#messages-object>`_
 
     Attributes:
         id: The message ID (If you want to reply to the message, use ``message_id_to_reply`` instead).
         metadata: The metadata of the message (to which phone number it was sent).
         type: The message type (See :class:`MessageType`).
         from_user: The user who sent the message.
         timestamp: The timestamp when the message was sent.
@@ -64,14 +75,15 @@
         reaction: The reaction of the message (if the message type is :class:`MessageType.REACTION`).
         location: The location of the message (if the message type is :class:`MessageType.LOCATION`).
         contacts: The contacts of the message (if the message type is :class:`MessageType.CONTACTS`).
         order: The order of the message (if the message type is :class:`MessageType.ORDER`).
         system: The system update (if the message type is :class:`MessageType.SYSTEM`).
         error: The error of the message (if the message type is :class:`MessageType.UNSUPPORTED`).
     """
+
     id: str
     type: MessageType
     metadata: Metadata
     from_user: User
     timestamp: dt.datetime
     reply_to_message: ReplyToMessage | None
     forwarded: bool
@@ -89,15 +101,17 @@
     order: Order | None = None
     system: System | None = None
     error: WhatsAppError | None = None
 
     @property
     def message_id_to_reply(self) -> str:
         """The ID of the message to reply to."""
-        return self.id if self.type != MessageType.REACTION else self.reaction.message_id
+        return (
+            self.id if self.type != MessageType.REACTION else self.reaction.message_id
+        )
 
     @property
     def has_media(self) -> bool:
         """
         Whether the message has any media. (image, video, sticker, document or audio)
             - If you want to get the media of the message, use :attr:`~Message.media` instead.
         """
@@ -110,47 +124,70 @@
 
         - Reaction messages are also considered as replies (But ``.reply_to_message`` will be ``None``).
         """
         return self.reply_to_message is not None or self.reaction is not None
 
     @classmethod
     def from_update(cls, client: WhatsApp, update: dict) -> Message:
-        msg = (value := update['entry'][0]['changes'][0]['value'])['messages'][0]
-        msg_type = msg['type']
-        context = msg.get('context')
+        msg = (value := update["entry"][0]["changes"][0]["value"])["messages"][0]
+        msg_type = msg["type"]
+        context = msg.get("context")
         constructor = _FIELDS_TO_OBJECTS_CONSTRUCTORS.get(msg_type)
-        msg_content = {msg_type: constructor(msg[msg_type], _client=client)} if constructor is not None else {} # noqa
+        msg_content = (
+            {msg_type: constructor(msg[msg_type], _client=client)}  # noqa
+            if constructor is not None
+            else {}
+        )  # noqa
         return cls(
             _client=client,
-            id=msg['id'],
-            type=MessageType(msg['type']),
+            id=msg["id"],
+            type=MessageType(msg["type"]),
             **msg_content,
-            from_user=User.from_dict(value['contacts'][0]),
-            timestamp=dt.datetime.fromtimestamp(int(msg['timestamp'])),
-            metadata=Metadata.from_dict(value['metadata']),
-            forwarded=any(context.get(key) for key in ('forwarded', 'frequently_forwarded')) if context else False,
-            forwarded_many_times=context.get('frequently_forwarded', False) if context else False,
+            from_user=User.from_dict(value["contacts"][0]),
+            timestamp=dt.datetime.fromtimestamp(int(msg["timestamp"])),
+            metadata=Metadata.from_dict(value["metadata"]),
+            forwarded=any(
+                context.get(key) for key in ("forwarded", "frequently_forwarded")
+            )
+            if context
+            else False,
+            forwarded_many_times=context.get("frequently_forwarded", False)
+            if context
+            else False,
             reply_to_message=ReplyToMessage.from_dict(context),
-            caption=msg[msg_type].get('caption') if msg_type in ('image', 'video', 'document') else None,
-            error=WhatsAppError.from_incoming_error(msg['errors'][0]) if 'errors' in msg else None
+            caption=msg[msg_type].get("caption")
+            if msg_type in ("image", "video", "document")
+            else None,
+            error=WhatsAppError.from_dict(error=msg["errors"][0])
+            if "errors" in msg
+            else None,
         )
 
     @property
-    def media(self) -> Image | Video | Sticker | Document | Audio | None:
+    def media(
+        self,
+    ) -> Image | Video | Sticker | Document | Audio | None:
         """
         The media of the message if any, otherwise ``None``. (image, video, sticker, document or audio)
             - If you want to check whether the message has any media, use :attr:`~Message.has_media` instead.
         """
-        return next((getattr(self, media_type) for media_type in _MEDIA_FIELDS if getattr(self, media_type)), None)
+        return next(
+            (
+                getattr(self, media_type)
+                for media_type in _MEDIA_FIELDS
+                if getattr(self, media_type)
+            ),
+            None,
+        )
 
     def download_media(
-            self,
-            filepath: str | None = None,
-            filename: str | None = None,
-            in_memory: bool = False,
+        self,
+        filepath: str | None = None,
+        filename: str | None = None,
+        in_memory: bool = False,
     ) -> str | bytes:
         """
         Download a media file from WhatsApp servers (image, video, sticker, document or audio).
 
         Args:
             filepath: The path where to save the file (if not provided, the current working directory will be used).
             filename: The name of the file (if not provided, it will be guessed from the URL + extension).
@@ -159,41 +196,45 @@
         Returns:
             The path of the saved file if ``in_memory`` is False, the file as bytes otherwise.
 
         Raises:
             ValueError: If the message does not contain any media.
         """
         try:
-            return self.media.download(path=filepath, filename=filename, in_memory=in_memory)
+            return self.media.download(
+                path=filepath, filename=filename, in_memory=in_memory
+            )
         except AttributeError:
-            raise ValueError('Message does not contain any media.')
+            raise ValueError("Message does not contain any media.")
 
     def copy(
-            self,
-            to: str,
-            header: str | None = None,
-            body: str | None = None,
-            footer: str | None = None,
-            keyboard: Iterable[Button] | ButtonUrl | SectionList | None = None,
-            preview_url: bool = False,
-            reply_to_message_id: str = None,
+        self,
+        to: str,
+        header: str | None = None,
+        body: str | None = None,
+        footer: str | None = None,
+        buttons: Iterable[Button] | ButtonUrl | SectionList | None = None,
+        preview_url: bool = False,
+        reply_to_message_id: str = None,
+        keyboard: None = None,
     ) -> str:
         """
         Copy incoming message to another chat
             - The WhatsApp Cloud API does not offer a `real` forward option so this is just copy the message content.
 
         Args:
             to: The phone ID of the WhatsApp user to copy the message to.
             header: The header of the message (if keyboard is provided, optional, up to 60 characters, no markdown allowed).
             body: The body of the message (if keyboard are provided, optional, up to 1024 characters, markdown allowed).
             footer: The footer of the message (if keyboard is provided, optional, markdown has no effect).
-            keyboard: The buttons to send with the message (only in case of message from type ``text``, ``document``,
+            buttons: The buttons to send with the message (only in case of message from type ``text``, ``document``,
              ``video`` and ``image``. also, the ``SectionList`` is only available to ``text`` type)
             reply_to_message_id:  The message ID to reply to (optional).
             preview_url: Whether to show a preview of the URL in the message (if any).
+            keyboard: Deprecated and will be removed in a future version, use ``buttons`` instead.
 
         Returns:
             The ID of the sent message.
 
         Raises:
             ValueError: If the message type is ``reaction`` and no ``reply_to_message_id`` is provided, or if the message
              type is ``unsupported``.
@@ -202,16 +243,17 @@
             case MessageType.TEXT:
                 return self._client.send_message(
                     to=to,
                     text=self.text,
                     preview_url=preview_url,
                     header=header,
                     footer=footer,
-                    keyboard=keyboard,
+                    buttons=buttons,
                     reply_to_message_id=reply_to_message_id,
+                    keyboard=keyboard,
                 )
             case MessageType.DOCUMENT:
                 return self._client.send_document(
                     to=to,
                     document=self.document.id,
                     filename=self.document.filename,
                     caption=self.caption,
@@ -237,71 +279,69 @@
                     caption=self.caption,
                     buttons=keyboard,
                     body=body,
                     footer=footer,
                     reply_to_message_id=reply_to_message_id,
                 )
             case MessageType.STICKER:
-                return self._client.send_sticker(
-                    to=to,
-                    sticker=self.sticker.id
-                )
+                return self._client.send_sticker(to=to, sticker=self.sticker.id)
             case MessageType.LOCATION:
                 return self._client.send_location(
                     to=to,
                     latitude=self.location.latitude,
                     longitude=self.location.longitude,
                     name=self.location.name,
-                    address=self.location.address
+                    address=self.location.address,
                 )
             case MessageType.AUDIO:
-                return self._client.send_audio(
-                    to=to,
-                    audio=self.audio.id
-                )
+                return self._client.send_audio(to=to, audio=self.audio.id)
             case MessageType.CONTACTS:
                 return self._client.send_contact(
                     to=to,
                     contact=self.contacts,
                     reply_to_message_id=reply_to_message_id,
                 )
             case MessageType.REACTION:
                 if reply_to_message_id is None:
-                    raise ValueError("You need to provide `reply_to_message_id` in order to `copy` a reaction")
+                    raise ValueError(
+                        "You need to provide `reply_to_message_id` in order to `copy` a reaction"
+                    )
                 return self._client.send_reaction(
                     to=to,
                     message_id=reply_to_message_id,
-                    emoji=self.reaction.emoji or ""
+                    emoji=self.reaction.emoji or "",
                 )
             case MessageType.ORDER:
                 if len(self.order.products) == 1:
                     return self._client.send_product(
                         to=to,
                         catalog_id=self.order.catalog_id,
                         sku=self.order.products[0].sku,
                         body=body,
                         footer=footer,
                         reply_to_message_id=reply_to_message_id,
                     )
                 return self._client.send_products(
                     to=to,
                     catalog_id=self.order.catalog_id,
-                    product_sections=(ProductsSection(
-                        title=header,
-                        skus=(p.sku for p in self.order.products)
-                    ),),
+                    product_sections=(
+                        ProductsSection(
+                            title=header,
+                            skus=(p.sku for p in self.order.products),
+                        ),
+                    ),
                     title=header,
                     body=body,
                     footer=footer,
                     reply_to_message_id=reply_to_message_id,
-                    )
+                )
             case MessageType.SYSTEM:
                 return self._client.send_message(
                     to=to,
                     text=self.system.body,
                     header=header,
                     footer=footer,
-                    keyboard=keyboard,
+                    buttons=keyboard,
                     reply_to_message_id=reply_to_message_id,
                 )
             case _:
                 raise ValueError(f"Message of type {self.type} cannot be copied.")
```

### Comparing `pywa-1.8.0/pywa/types/message_status.py` & `pywa-1.9.0/pywa/types/message_status.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from __future__ import annotations
 
 """This module contains the types related to message status updates."""
 
 __all__ = [
-    'MessageStatus',
-    'MessageStatusType',
-    'Conversation',
-    'ConversationCategory'
+    "MessageStatus",
+    "MessageStatusType",
+    "Conversation",
+    "ConversationCategory",
 ]
 
 import dataclasses
 import datetime as dt
 from typing import TYPE_CHECKING
-from pywa.errors import WhatsAppError
+
 from pywa import utils
-from .base_update import BaseUserUpdate
+from pywa.errors import WhatsAppError
+
+from .base_update import BaseUserUpdate  # noqa
 from .others import Metadata, User
 
 if TYPE_CHECKING:
     from pywa.client import WhatsApp
 
 
 class MessageStatusType(utils.StrEnum):
@@ -27,18 +29,19 @@
 
     Attributes:
         SENT: The message was sent.
         DELIVERED: The message was delivered.
         READ: The message was read.
         FAILED: The message failed to send (you can access the error with ``.error`` attribute).
     """
-    SENT = 'sent'
-    DELIVERED = 'delivered'
-    READ = 'read'
-    FAILED = 'failed'
+
+    SENT = "sent"
+    DELIVERED = "delivered"
+    READ = "read"
+    FAILED = "failed"
 
     @classmethod
     def _missing_(cls, value: str) -> MessageStatusType:
         return cls.FAILED
 
 
 class ConversationCategory(utils.StrEnum):
@@ -49,88 +52,95 @@
         AUTHENTICATION: The conversation is related to authentication.
         MARKETING: The conversation is related to marketing.
         UTILITY: The conversation is related to utility.
         SERVICE: The conversation is related to service.
         REFERRAL_CONVERSION: The conversation is related to referral conversion.
         UNKNOWN: The conversation category is unknown.
     """
-    AUTHENTICATION = 'authentication'
-    MARKETING = 'marketing'
-    UTILITY = 'utility'
-    SERVICE = 'service'
-    REFERRAL_CONVERSION = 'referral_conversion'
-    UNKNOWN = 'unknown'
+
+    AUTHENTICATION = "authentication"
+    MARKETING = "marketing"
+    UTILITY = "utility"
+    SERVICE = "service"
+    REFERRAL_CONVERSION = "referral_conversion"
+    UNKNOWN = "unknown"
 
     @classmethod
     def _missing_(cls, value: str) -> ConversationCategory:
         return cls.UNKNOWN
 
 
 @dataclasses.dataclass(frozen=True, slots=True, kw_only=True)
 class MessageStatus(BaseUserUpdate):
     """
     Represents the status of a message.
 
-    - `\`MessageStatus\` on developers.facebook.com <https://developers.facebook.com/docs/whatsapp/cloud-api/webhooks/components#statuses-object>`_.
+    - `'MessageStatus' on developers.facebook.com <https://developers.facebook.com/docs/whatsapp/cloud-api/webhooks/components#statuses-object>`_.
 
     Attributes:
         id: The ID of the message that the status is for.
         metadata: The metadata of the message (to which phone number it was sent).
         status: The status of the message.
         timestamp: The timestamp when the status was updated.
         from_user: The user who the message was sent to.
         conversation: The conversation the given status notification belongs to (Optional).
         pricing_model: Type of pricing model used by the business. Current supported value is CBP.
         error: The error that occurred (if status is ``failed``).
     """
+
     id: str
     metadata: Metadata
     from_user: User
     timestamp: dt.datetime
     status: MessageStatusType
     conversation: Conversation | None
     pricing_model: str | None
     error: WhatsAppError | None
 
     @classmethod
     def from_update(cls, client: WhatsApp, update: dict) -> MessageStatus:
-        status = (value := update['entry'][0]['changes'][0]['value'])['statuses'][0]
-        status_type = MessageStatusType(status['status'])
+        status = (value := update["entry"][0]["changes"][0]["value"])["statuses"][0]
+        status_type = MessageStatusType(status["status"])
         return cls(
             _client=client,
-            id=status['id'],
-            metadata=Metadata.from_dict(value['metadata']),
+            id=status["id"],
+            metadata=Metadata.from_dict(value["metadata"]),
             status=status_type,
-            timestamp=dt.datetime.fromtimestamp(int(status['timestamp'])),
-            from_user=User(wa_id=status['recipient_id'], name=None),
-            conversation=Conversation.from_dict(status['conversation']) if 'conversation' in status else None,
-            pricing_model=status.get('pricing', {}).get('pricing_model'),
-            error=WhatsAppError.from_incoming_error(status['errors'][0])
-            if status_type == MessageStatusType.FAILED else None
+            timestamp=dt.datetime.fromtimestamp(int(status["timestamp"])),
+            from_user=User(wa_id=status["recipient_id"], name=None),
+            conversation=Conversation.from_dict(status["conversation"])
+            if "conversation" in status
+            else None,
+            pricing_model=status.get("pricing", {}).get("pricing_model"),
+            error=WhatsAppError.from_dict(error=status["errors"][0])
+            if status_type == MessageStatusType.FAILED
+            else None,
         )
 
 
 @dataclasses.dataclass(frozen=True, slots=True)
 class Conversation:
     """
     Represents a conversation.
 
-    - `\`Conversation\` on developers.facebook.com <https://developers.facebook.com/docs/whatsapp/pricing#conversations>`_.
+    - `'Conversation' on developers.facebook.com <https://developers.facebook.com/docs/whatsapp/pricing#conversations>`_.
 
     Attributes:
         id: The ID of the conversation.
         category: The category of the conversation.
         expiration: The expiration date of the conversation (Optional, only for `sent` updates).
 
     """
+
     id: str
     category: ConversationCategory
     expiration: dt.datetime | None
 
     @classmethod
     def from_dict(cls, data: dict):
         return cls(
-            id=data['id'],
-            category=ConversationCategory(data['origin']['type']),
-            expiration=dt.datetime.fromtimestamp(int(data['expiration_timestamp']))
-            if 'expiration_timestamp' in data else None
+            id=data["id"],
+            category=ConversationCategory(data["origin"]["type"]),
+            expiration=dt.datetime.fromtimestamp(int(data["expiration_timestamp"]))
+            if "expiration_timestamp" in data
+            else None,
         )
```

### Comparing `pywa-1.8.0/pywa/types/others.py` & `pywa-1.9.0/pywa/types/others.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 from __future__ import annotations
 
 """Types for other objects."""
 
 import dataclasses
 import importlib
-from typing import Any, Iterable, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Iterable
+
 from pywa import utils
 
 if TYPE_CHECKING:
-    from pywa.client import WhatsApp
     from message_status import MessageStatus
 
+    from pywa.client import WhatsApp
+
 
 @dataclasses.dataclass(frozen=True, slots=True)
 class User:
     """
     Represents a WhatsApp user.
 
     Attributes:
         wa_id: The WhatsApp ID of the user (The phone number with the country code).
         name: The name of the user (``None`` on :class:`MessageStatus`).
     """
+
     wa_id: str
     name: str | None
 
     @classmethod
     def from_dict(cls, data: dict) -> User:
         return cls(wa_id=data["wa_id"], name=data["profile"]["name"])
 
     def as_vcard(self) -> str:
         """Get the user as a vCard."""
-        return "\n".join((
-            "BEGIN:VCARD",
-            "VERSION:3.0",
-            f"FN;CHARSET=UTF-8;ENCODING=QUOTED-PRINTABLE:{self.name}",
-            f"TEL;type=CELL;type=VOICE:+{self.wa_id}",
-            "END:VCARD"
-        ))
+        return "\n".join(
+            (
+                "BEGIN:VCARD",
+                "VERSION:3.0",
+                f"FN;CHARSET=UTF-8;ENCODING=QUOTED-PRINTABLE:{self.name}",
+                f"TEL;type=CELL;type=VOICE:+{self.wa_id}",
+                "END:VCARD",
+            )
+        )
 
 
 class MessageType(utils.StrEnum):
     """
     Message types.
 
     Attributes:
@@ -56,14 +61,15 @@
         ORDER: An order message.
         SYSTEM: A system message.
         UNKNOWN: An unknown message.
         UNSUPPORTED: An unsupported message.
         INTERACTIVE: An interactive message (callback).
         BUTTON: Quick reply button (in a template message).
     """
+
     TEXT = "text"
     IMAGE = "image"
     VIDEO = "video"
     DOCUMENT = "document"
     AUDIO = "audio"
     STICKER = "sticker"
     REACTION = "reaction"
@@ -87,14 +93,15 @@
     """
     Represents a reaction to a message.
 
     Attributes:
         message_id: The ID of the message that was reacted to.
         emoji: The emoji that was used to react to the message (optional, ``None`` if removed).
     """
+
     message_id: str
     emoji: str | None = None
 
 
 @dataclasses.dataclass(frozen=True, slots=True)
 class Location(utils.FromDict):
     """
@@ -103,14 +110,15 @@
     Attributes:
         latitude: The latitude of the location.
         longitude: The longitude of the location.
         name: The name of the location (optional).
         address: The address of the location (optional).
         url: The URL of the location (optional).
     """
+
     latitude: float
     longitude: float
     name: str | None = None
     address: str | None = None
     url: str | None = None
 
     @property
@@ -124,19 +132,31 @@
 
         Args:
             lat: The latitude of the other location.
             lon: The longitude of the other location.
             radius: The radius in kilometers.
         """
         math = importlib.import_module("math")
-        lon1, lat1, lon2, lat2 = map(math.radians, [self.longitude, self.latitude, lon, lat])
-        return ((2 * math.asin(
-            math.sqrt(
-                math.sin((lat2 - lat1) / 2) ** 2 + math.cos(lat1) * math.cos(lat2) * math.sin((lon2 - lon1) / 2) ** 2)
-        )) * 6371) <= radius
+        lon1, lat1, lon2, lat2 = map(
+            math.radians, [self.longitude, self.latitude, lon, lat]
+        )
+        return (
+            (
+                2
+                * math.asin(
+                    math.sqrt(
+                        math.sin((lat2 - lat1) / 2) ** 2
+                        + math.cos(lat1)
+                        * math.cos(lat2)
+                        * math.sin((lon2 - lon1) / 2) ** 2
+                    )
+                )
+            )
+            * 6371
+        ) <= radius
 
 
 @dataclasses.dataclass(slots=True)
 class Contact:
     """
     Represents a contact.
 
@@ -145,60 +165,87 @@
         birthday: The birthday of the contact (in ``YYYY-MM-DD`` format, optional).
         phones: The phone numbers of the contact.
         emails: The email addresses of the contact.
         urls: The URLs of the contact.
         addresses: The addresses of the contact.
         org: The organization of the contact (optional).
     """
+
     name: Name
     birthday: str | None = None
     phones: Iterable[Phone] = dataclasses.field(default_factory=tuple)
     emails: Iterable[Email] = dataclasses.field(default_factory=tuple)
     urls: Iterable[Url] = dataclasses.field(default_factory=tuple)
     addresses: Iterable[Address] = dataclasses.field(default_factory=tuple)
     org: Org | None = None
 
     @classmethod
     def from_dict(cls, data: dict):
         return cls(
             name=cls.Name.from_dict(data["name"]),
             birthday=data.get("birthday"),
-            phones=tuple(cls.Phone.from_dict(phone) for phone in data.get("phones", ())),
-            emails=tuple(cls.Email.from_dict(email) for email in data.get("emails", ())),
+            phones=tuple(
+                cls.Phone.from_dict(phone) for phone in data.get("phones", ())
+            ),
+            emails=tuple(
+                cls.Email.from_dict(email) for email in data.get("emails", ())
+            ),
             urls=tuple(cls.Url.from_dict(url) for url in data.get("urls", ())),
-            addresses=tuple(cls.Address.from_dict(address) for address in data.get("addresses", ())),
-            org=cls.Org.from_dict(data["org"]) if "org" in data else None
+            addresses=tuple(
+                cls.Address.from_dict(address) for address in data.get("addresses", ())
+            ),
+            org=cls.Org.from_dict(data["org"]) if "org" in data else None,
         )
 
     def to_dict(self) -> dict[str, Any]:
         """Get the contact as a dict."""
         return {
             "name": dataclasses.asdict(self.name),
             "birthday": self.birthday,
             "phones": tuple(dataclasses.asdict(phone) for phone in self.phones),
             "emails": tuple(dataclasses.asdict(email) for email in self.emails),
             "urls": tuple(dataclasses.asdict(url) for url in self.urls),
-            "addresses": tuple(dataclasses.asdict(address) for address in self.addresses),
+            "addresses": tuple(
+                dataclasses.asdict(address) for address in self.addresses
+            ),
             "org": dataclasses.asdict(self.org) if self.org else None,
         }
 
     def as_vcard(self) -> str:
         """Get the contact as a vCard."""
-        return "\n".join(s for s in (
-            "BEGIN:VCARD",
-            "VERSION:3.0",
-            f"FN;CHARSET=UTF-8;ENCODING=QUOTED-PRINTABLE:{self.name.formatted_name}",
-            f"BDAY:{self.birthday}" if self.birthday else None,
-            "\n".join(f"TEL;type={phone.type}:{phone.phone}" for phone in self.phones) if self.phones else None,
-            "\n".join(f"EMAIL;type={email.type}:{email.email}" for email in self.emails) if self.emails else None,
-            "\n".join(f"URL;type={url.type}:{url.url}" for url in self.urls) if self.urls else None,
-            "\n".join(f"ADR;type={a.type}:;;{';'.join((getattr(a, f) or '') for f in ('street', 'city', 'state', 'zip', 'country') )}"
-                      for a in self.addresses) if self.addresses else None,
-            "END:VCARD"
-        ) if s is not None)
+        return "\n".join(
+            s
+            for s in (
+                "BEGIN:VCARD",
+                "VERSION:3.0",
+                f"FN;CHARSET=UTF-8;ENCODING=QUOTED-PRINTABLE:{self.name.formatted_name}",
+                f"BDAY:{self.birthday}" if self.birthday else None,
+                "\n".join(
+                    f"TEL;type={phone.type}:{phone.phone}" for phone in self.phones
+                )
+                if self.phones
+                else None,
+                "\n".join(
+                    f"EMAIL;type={email.type}:{email.email}" for email in self.emails
+                )
+                if self.emails
+                else None,
+                "\n".join(f"URL;type={url.type}:{url.url}" for url in self.urls)
+                if self.urls
+                else None,
+                "\n".join(
+                    f"ADR;type={a.type}:;;{';'.join((getattr(a, f) or '') for f in ('street', 'city', 'state', 'zip', 'country') )}"
+                    for a in self.addresses
+                )
+                if self.addresses
+                else None,
+                "END:VCARD",
+            )
+            if s is not None
+        )
 
     @dataclasses.dataclass(frozen=True, slots=True)
     class Name(utils.FromDict):
         """
         Represents a contact's name.
 
         - At least one of the optional parameters needs to be included along with the formatted_name parameter.
@@ -207,14 +254,15 @@
             formatted_name: The formatted name of the contact.
             first_name: The first name of the contact (optional).
             last_name: The last name of the contact (optional).
             middle_name: The middle name of the contact (optional).
             suffix: The suffix of the contact (optional).
             prefix: The prefix of the contact (optional).
         """
+
         formatted_name: str
         first_name: str | None = None
         last_name: str | None = None
         middle_name: str | None = None
         suffix: str | None = None
         prefix: str | None = None
 
@@ -224,52 +272,56 @@
         Represents a contact's phone number.
 
         Attributes:
             phone: The phone number (If ``wa_id`` is provided, No need for the ``phone``).
             type: The type of the phone number (Standard Values are CELL, MAIN, IPHONE, HOME, and WORK. optional).
             wa_id: The WhatsApp ID of the contact (optional).
         """
+
         phone: str | None = None
         type: str | None = None
         wa_id: str | None = None
 
     @dataclasses.dataclass(frozen=True, slots=True)
     class Email(utils.FromDict):
         """
         Represents a contact's email address.
 
         Attributes:
             email: The email address.
             type: The type of the email address (Standard Values are WORK and HOME. optional).
         """
+
         email: str | None = None
         type: str | None = None
 
     @dataclasses.dataclass(frozen=True, slots=True)
     class Url(utils.FromDict):
         """
         Represents a contact's URL.
 
         Attributes:
             url: The URL.
             type: The type of the URL (Standard Values are WORK and HOME. optional).
         """
+
         url: str | None = None
         type: str | None = None
 
     @dataclasses.dataclass(frozen=True, slots=True)
     class Org(utils.FromDict):
         """
         Represents a contact's organization.
 
         Attributes:
             company: The company of the contact (optional).
             department: The department of the contact (optional).
             title: The title of the business contact (optional).
         """
+
         company: str | None = None
         department: str | None = None
         title: str | None = None
 
     @dataclasses.dataclass(frozen=True, slots=True)
     class Address(utils.FromDict):
         """
@@ -280,14 +332,15 @@
             city: The city name of the address (optional).
             state: State abbreviation.
             zip: Zip code of the address (optional).
             country: Full country name.
             country_code: Two-letter country abbreviation (e.g. US, GB, IN. optional).
             type: The type of the address (Standard Values are WORK and HOME. optional).
         """
+
         street: str | None = None
         city: str | None = None
         state: str | None = None
         zip: str | None = None
         country: str | None = None
         country_code: str | None = None
         type: str | None = None
@@ -298,34 +351,37 @@
     """
     Represents a message that was replied to.
 
     Attributes:
         message_id: The ID of the message that was replied to.
         from_user_id: The ID of the user who sent the message that was replied to.
     """
+
     message_id: str
     from_user_id: str
 
     @classmethod
     def from_dict(cls, data: dict | None) -> ReplyToMessage | None:
-        return cls(
-            message_id=data['id'],
-            from_user_id=data['from']
-        ) if (data and 'id' in data) else None
+        return (
+            cls(message_id=data["id"], from_user_id=data["from"])
+            if (data and "id" in data)
+            else None
+        )
 
 
 @dataclasses.dataclass(frozen=True, slots=True)
 class Metadata(utils.FromDict):
     """
     Represents the metadata of a message.
 
     Attributes:
         display_phone_number: The phone number to which the message was sent.
         phone_number_id: The ID of the phone number to which the message was sent.
     """
+
     display_phone_number: str
     phone_number_id: str
 
 
 @dataclasses.dataclass(frozen=True, slots=True)
 class Product:
     """
@@ -333,26 +389,27 @@
 
     Attributes:
         sku: Unique identifier of the product in a catalog (also referred to as ``Content ID`` or ``Retailer ID``).
         quantity: Number of items ordered.
         price: Price of the item.
         currency: Currency of the price.
     """
+
     sku: str
     quantity: int
     price: float
     currency: str
 
     @classmethod
     def from_dict(cls, data: dict) -> Product:
         return cls(
             sku=data["product_retailer_id"],
             quantity=data["quantity"],
             price=data["item_price"],
-            currency=data["currency"]
+            currency=data["currency"],
         )
 
     @property
     def total_price(self) -> float:
         """Total price of the product."""
         return self.quantity * self.price
 
@@ -366,24 +423,25 @@
         catalog_id: The ID for the catalog the ordered item belongs to.
         products:The ordered products.
         text: Text message from the user sent along with the order (optional).
 
     Properties:
         total_price: Total price of the order.
     """
+
     catalog_id: str
     products: tuple[Product]
     text: str | None
 
     @classmethod
     def from_dict(cls, data: dict, _client: WhatsApp) -> Order:
         return cls(
-            catalog_id=data['catalog_id'],
-            text=data.get('text'),
-            products=tuple(Product.from_dict(p) for p in data['product_items'])
+            catalog_id=data["catalog_id"],
+            text=data.get("text"),
+            products=tuple(Product.from_dict(p) for p in data["product_items"]),
         )
 
     @property
     def total_price(self) -> float:
         """Total price of the order."""
         return sum(p.total_price for p in self.products)
 
@@ -396,47 +454,49 @@
     Attributes:
         type: The type of the system update (``customer_changed_number`` or ``customer_identity_changed``).
         body: Describes the change to the customer's identity or phone number.
         identity: Hash for the identity fetched from server.
         wa_id: The WhatsApp ID for the customer prior to the update.
         new_wa_id: New WhatsApp ID for the customer when their phone number is updated.
     """
+
     type: str
     body: str
     identity: str
     wa_id: str
     new_wa_id: str | None
 
     @classmethod
     def from_dict(cls, data: dict, _client: WhatsApp) -> System:
         return cls(
-            type=data['type'],
-            body=data['body'],
-            identity=data['identity'],
-            wa_id=data['customer'],
-            new_wa_id=data.get('wa_id')
+            type=data["type"],
+            body=data["body"],
+            identity=data["identity"],
+            wa_id=data["customer"],
+            new_wa_id=data.get("wa_id"),
         )
 
 
 @dataclasses.dataclass(frozen=True, slots=True)
 class ProductsSection:
     """
     Represents a section in a section list.
 
     Attributes:
         title: The title of the products section (up to 24 characters).
         skus: The SKUs of the products in the section (at least 1, no more than 30).
     """
+
     title: str
     skus: Iterable[str]
 
     def to_dict(self) -> dict:
         return {
             "title": self.title,
-            "product_items": tuple({"product_retailer_id": sku} for sku in self.skus)
+            "product_items": tuple({"product_retailer_id": sku} for sku in self.skus),
         }
 
 
 class Industry(utils.StrEnum):
     """
     Represents the industry of a business.
 
@@ -457,14 +517,15 @@
         NONPROFIT: Nonprofit.
         PROF_SERVICES: Professional services.
         RETAIL: Retail.
         TRAVEL: Travel.
         RESTAURANT: Restaurant.
         NOT_A_BIZ: Not a business.
     """
+
     UNDEFINED = "UNDEFINED"
     OTHER = "OTHER"
     AUTO = "AUTO"
     BEAUTY = "BEAUTY"
     APPAREL = "APPAREL"
     EDU = "EDU"
     ENTERTAIN = "ENTERTAIN"
@@ -497,50 +558,51 @@
         description: Description of the business. Character limit 512.
         email: The contact email address (in valid email format) of the business. Character limit 128.
         industry: The industry of the business.
         profile_picture_url: URL of the profile picture that was uploaded to Meta.
         websites: The URLs associated with the business. For instance, a website, Facebook Page, or Instagram.
          There is a maximum of 2 websites with a maximum of 256 characters each.
     """
+
     about: str
     address: str | None
     industry: Industry
     description: str | None
     email: str | None
     profile_picture_url: str | None
     websites: tuple[str] | None
 
     @classmethod
     def from_dict(cls, data: dict) -> BusinessProfile:
         return cls(
-            about=data['about'],
-            address=data.get('address'),
-            industry=Industry(data['vertical']),
-            description=data.get('description'),
-            email=data.get('email'),
-            profile_picture_url=data.get('profile_picture_url'),
-            websites=tuple(data.get('websites', [])) or None
+            about=data["about"],
+            address=data.get("address"),
+            industry=Industry(data["vertical"]),
+            description=data.get("description"),
+            email=data.get("email"),
+            profile_picture_url=data.get("profile_picture_url"),
+            websites=tuple(data.get("websites", [])) or None,
         )
 
 
 @dataclasses.dataclass(frozen=True, slots=True)
 class CommerceSettings:
     """
     Represents the WhatsApp commerce settings.
 
     Attributes:
         catalog_id: The ID of the catalog associated with the business.
         is_catalog_visible: Whether the catalog is visible to customers.
         is_cart_enabled: Whether the cart is enabled.
     """
+
     catalog_id: str
     is_catalog_visible: bool
     is_cart_enabled: bool
 
     @classmethod
     def from_dict(cls, data: dict) -> CommerceSettings:
         return cls(
-            catalog_id=data['id'],
-            is_catalog_visible=data['is_catalog_visible'],
-            is_cart_enabled=data['is_cart_enabled']
+            catalog_id=data["id"],
+            is_catalog_visible=data["is_catalog_visible"],
+            is_cart_enabled=data["is_cart_enabled"],
         )
-
```

### Comparing `pywa-1.8.0/pywa/types/template.py` & `pywa-1.9.0/pywa/types/template.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from __future__ import annotations
 
 """This module contains the types related to templates."""
 
 __all__ = [
-    'Template',
-    'NewTemplate',
-    'TemplateResponse',
-    'TemplateStatus'
+    "Template",
+    "NewTemplate",
+    "TemplateResponse",
+    "TemplateStatus",
 ]
 
 import abc
-import re
 import dataclasses
+import re
 from datetime import datetime
-from typing import Iterable, BinaryIO, TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, BinaryIO, Iterable
+
 from pywa import utils
-from .others import ProductsSection
-from .base_update import BaseUpdate
+
+from .base_update import BaseUpdate  # noqa
 from .callback import CallbackDataT, _resolve_callback_data  # noqa
+from .others import ProductsSection
 
 if TYPE_CHECKING:
     from pywa.client import WhatsApp
 
 DEFAULT = object()
 
 
 def _get_examples_from_placeholders(
-        string: str,
-        start: str = '{',
-        end: str = '}'
+    string: str, start: str = "{", end: str = "}"
 ) -> tuple[str, tuple[str]]:
     """
     Extracts the examples from a string.
 
     Example:
 
         >>> _get_examples_from_placeholders('Hello, {john}, today is {day}')
@@ -44,15 +44,15 @@
       start: The start of the example (default: ``'{'``).
       end: The end of the example (default: ``'}'``).
 
     Returns:
       A tuple of the formatted string and the examples.
     """
     examples: list[str] = []
-    for example in re.finditer(r'\%s(.*?)\%s' % (start, end), string):
+    for example in re.finditer(r"\%s(.*?)\%s" % (start, end), string):
         examples.append(example.group(1))
     for idx, example in enumerate(examples, start=1):
         string = string.replace(f"{start}{example}{end}", "{{" + str(idx) + "}}")
     return string, tuple(examples)
 
 
 @dataclasses.dataclass(frozen=True, slots=True)
@@ -60,158 +60,164 @@
     """
 
     Attributes:
         id: the template ID.
         status: the template status.
         category: the template category.
     """
+
     id: str
     status: str
     category: NewTemplate.Category
 
 
 class ComponentType(utils.StrEnum):
-    HEADER = 'HEADER'
-    BODY = 'BODY'
-    FOOTER = 'FOOTER'
-    BUTTONS = 'BUTTONS'
+    HEADER = "HEADER"
+    BODY = "BODY"
+    FOOTER = "FOOTER"
+    BUTTONS = "BUTTONS"
 
 
 class HeaderFormatType(utils.StrEnum):
-    TEXT = 'TEXT'
-    IMAGE = 'IMAGE'
-    VIDEO = 'VIDEO'
-    DOCUMENT = 'DOCUMENT'
-    LOCATION = 'LOCATION'
+    TEXT = "TEXT"
+    IMAGE = "IMAGE"
+    VIDEO = "VIDEO"
+    DOCUMENT = "DOCUMENT"
+    LOCATION = "LOCATION"
 
 
 class ButtonType(utils.StrEnum):
-    PHONE_NUMBER = 'PHONE_NUMBER'
-    URL = 'URL'
-    QUICK_REPLY = 'QUICK_REPLY'
-    OTP = 'OTP'
-    MPM = 'MPM'
-    CATALOG = 'CATALOG'
-    COPY_CODE = 'COPY_CODE'
+    PHONE_NUMBER = "PHONE_NUMBER"
+    URL = "URL"
+    QUICK_REPLY = "QUICK_REPLY"
+    OTP = "OTP"
+    MPM = "MPM"
+    CATALOG = "CATALOG"
+    COPY_CODE = "COPY_CODE"
 
 
 class Language(utils.StrEnum):
     """
     Template language and locale code.
         - Both :class:`NewTemplate` and :class:`Template` have this class as an attribute.
 
     >>> from pywa.types import NewTemplate
     >>> NewTemplate.Language.ENGLISH_US
 
     >>> from pywa.types import Template
     >>> Template.Language.ENGLISH_US
 
-    `\`Template language and locale code\` on
+    `'Template language and locale code' on
     developers.facebook.com
     <https://developers.facebook.com/docs/whatsapp/business-management-api/message-templates/supported-languages>`_
     """
-    AFRIKAANS = 'af'
-    ALBANIAN = 'sq'
-    ARABIC = 'ar'
-    AZERBAIJANI = 'az'
-    BENGALI = 'bn'
-    BULGARIAN = 'bg'
-    CATALAN = 'ca'
-    CHINESE_CHN = 'zh_CN'
-    CHINESE_HKG = 'zh_HK'
-    CHINESE_TAI = 'zh_TW'
-    CROATIAN = 'hr'
-    CZECH = 'cs'
-    DANISH = 'da'
-    DUTCH = 'nl'
-    ENGLISH = 'en'
-    ENGLISH_UK = 'en_GB'
-    ENGLISH_US = 'en_US'
-    ESTONIAN = 'et'
-    FILIPINO = 'fil'
-    FINNISH = 'fi'
-    FRENCH = 'fr'
-    GEORGIAN = 'ka'
-    GERMAN = 'de'
-    GREEK = 'el'
-    GUJARATI = 'gu'
-    HAUSA = 'ha'
-    HEBREW = 'he'
-    HINDI = 'hi'
-    HUNGARIAN = 'hu'
-    INDONESIAN = 'id'
-    IRISH = 'ga'
-    ITALIAN = 'it'
-    JAPANESE = 'ja'
-    KANNADA = 'kn'
-    KAZAKH = 'kk'
-    KINYARWANDA = 'rw_RW'
-    KOREAN = 'ko'
-    KYRGYZ_KG = 'ky_KG'
-    LAO = 'lo'
-    LATVIAN = 'lv'
-    LITHUANIAN = 'lt'
-    MACEDONIAN = 'mk'
-    MALAY = 'ms'
-    MALAYALAM = 'ml'
-    MARATHI = 'mr'
-    NORWEGIAN = 'nb'
-    PERSIAN = 'fa'
-    POLISH = 'pl'
-    PORTUGUESE_BR = 'pt_BR'
-    PORTUGUESE_POR = 'pt_PT'
-    PUNJABI = 'pa'
-    ROMANIAN = 'ro'
-    RUSSIAN = 'ru'
-    SERBIAN = 'sr'
-    SLOVAK = 'sk'
-    SLOVENIAN = 'sl'
-    SPANISH = 'es'
-    SPANISH_ARG = 'es_AR'
-    SPANISH_SPA = 'es_ES'
-    SPANISH_MEX = 'es_MX'
-    SWAHILI = 'sw'
-    SWEDISH = 'sv'
-    TAMIL = 'ta'
-    TELUGU = 'te'
-    THAI = 'th'
-    TURKISH = 'tr'
-    UKRAINIAN = 'uk'
-    URDU = 'ur'
-    UZBEK = 'uz'
-    VIETNAMESE = 'vi'
-    ZULU = 'zu'
+
+    AFRIKAANS = "af"
+    ALBANIAN = "sq"
+    ARABIC = "ar"
+    AZERBAIJANI = "az"
+    BENGALI = "bn"
+    BULGARIAN = "bg"
+    CATALAN = "ca"
+    CHINESE_CHN = "zh_CN"
+    CHINESE_HKG = "zh_HK"
+    CHINESE_TAI = "zh_TW"
+    CROATIAN = "hr"
+    CZECH = "cs"
+    DANISH = "da"
+    DUTCH = "nl"
+    ENGLISH = "en"
+    ENGLISH_UK = "en_GB"
+    ENGLISH_US = "en_US"
+    ESTONIAN = "et"
+    FILIPINO = "fil"
+    FINNISH = "fi"
+    FRENCH = "fr"
+    GEORGIAN = "ka"
+    GERMAN = "de"
+    GREEK = "el"
+    GUJARATI = "gu"
+    HAUSA = "ha"
+    HEBREW = "he"
+    HINDI = "hi"
+    HUNGARIAN = "hu"
+    INDONESIAN = "id"
+    IRISH = "ga"
+    ITALIAN = "it"
+    JAPANESE = "ja"
+    KANNADA = "kn"
+    KAZAKH = "kk"
+    KINYARWANDA = "rw_RW"
+    KOREAN = "ko"
+    KYRGYZ_KG = "ky_KG"
+    LAO = "lo"
+    LATVIAN = "lv"
+    LITHUANIAN = "lt"
+    MACEDONIAN = "mk"
+    MALAY = "ms"
+    MALAYALAM = "ml"
+    MARATHI = "mr"
+    NORWEGIAN = "nb"
+    PERSIAN = "fa"
+    POLISH = "pl"
+    PORTUGUESE_BR = "pt_BR"
+    PORTUGUESE_POR = "pt_PT"
+    PUNJABI = "pa"
+    ROMANIAN = "ro"
+    RUSSIAN = "ru"
+    SERBIAN = "sr"
+    SLOVAK = "sk"
+    SLOVENIAN = "sl"
+    SPANISH = "es"
+    SPANISH_ARG = "es_AR"
+    SPANISH_SPA = "es_ES"
+    SPANISH_MEX = "es_MX"
+    SWAHILI = "sw"
+    SWEDISH = "sv"
+    TAMIL = "ta"
+    TELUGU = "te"
+    THAI = "th"
+    TURKISH = "tr"
+    UKRAINIAN = "uk"
+    URDU = "ur"
+    UZBEK = "uz"
+    VIETNAMESE = "vi"
+    ZULU = "zu"
 
 
 class NewTemplateComponentABC(abc.ABC):
     @property
     @abc.abstractmethod
-    def type(self) -> ComponentType: ...
+    def type(self) -> ComponentType:
+        ...
 
 
 class NewTemplateHeaderABC(NewTemplateComponentABC, abc.ABC):
     @property
     @abc.abstractmethod
-    def format(self) -> HeaderFormatType: ...
+    def format(self) -> HeaderFormatType:
+        ...
 
 
 class NewButtonABC(abc.ABC):
     @property
     @abc.abstractmethod
-    def type(self) -> ButtonType: ...
+    def type(self) -> ButtonType:
+        ...
 
     @abc.abstractmethod
-    def to_dict(self, placeholder: tuple[str, str] = None) -> dict[str, str | None]: ...
+    def to_dict(self, placeholder: tuple[str, str] = None) -> dict[str, str | None]:
+        ...
 
 
 @dataclasses.dataclass(slots=True)
 class NewTemplate:
     """
     Represents a new template.
-    `\`Create Templates\` on developers.facebook.com
+    `'Create Templates' on developers.facebook.com
     <https://developers.facebook.com/docs/whatsapp/business-management-api/message-templates>`_.
 
     Attributes:
         name: Name of the template (up to 512 characters, must be unique).
         category: Category of the template.
         language: The language of the template (See `Template language and locale code
          <https://developers.facebook.com/docs/whatsapp/business-management-api/message-templates/supported-languages>`_).
@@ -261,224 +267,281 @@
     Templates are limited to 10 quick reply buttons. If using quick reply buttons with other buttons, buttons must be
     organized into two groups: quick reply buttons and non-quick reply buttons. If grouped incorrectly, error will be
     raised when submitting the template.
 
     When you send a template that has multiple quick reply buttons, the order in which the buttons appear in the template
     is the order in which they will appear in the delivered message
     """
+
     name: str
     category: Category
     language: Language | str
     body: Body | AuthBody
     header: Text | Image | Video | Document | Location | None = None
     footer: Footer | None = None
-    buttons: (Iterable[PhoneNumberButton | UrlButton | QuickReplyButton | CopyCodeButton]
-              | MPMButton | CatalogButton | OTPButton | None) = None
+    buttons: (
+        Iterable[PhoneNumberButton | UrlButton | QuickReplyButton | CopyCodeButton]
+        | MPMButton
+        | CatalogButton
+        | OTPButton
+        | None
+    ) = None
 
     def __post_init__(self):
         if self.category == self.Category.AUTHENTICATION and not (
-                isinstance(self.body, self.AuthBody) or isinstance(self.buttons, self.OTPButton)
+            isinstance(self.body, self.AuthBody)
+            or isinstance(self.buttons, self.OTPButton)
         ):
-            raise ValueError('body of AuthBody and buttons of OTPButton are required for AUTHENTICATION')
+            raise ValueError(
+                "body of AuthBody and buttons of OTPButton are required for AUTHENTICATION"
+            )
 
-    def to_dict(
-            self,
-            placeholder: tuple[str, str] = None
-    ) -> dict[str, Any]:
+    def to_dict(self, placeholder: tuple[str, str] = None) -> dict[str, Any]:
         if isinstance(self.buttons, self.OTPButton):
             components = (
-                dict(type=ComponentType.BUTTONS.value, buttons=(self.buttons.to_dict(),)),
-                dict(type=ComponentType.BODY.value,
-                     add_security_recommendation=self.body.add_security_recommendation),
-                dict(type=ComponentType.FOOTER.value, code_expiration_minutes=self.body.code_expiration_minutes)
-                if self.body.code_expiration_minutes else None,
+                dict(
+                    type=ComponentType.BUTTONS.value,
+                    buttons=(self.buttons.to_dict(),),
+                ),
+                dict(
+                    type=ComponentType.BODY.value,
+                    add_security_recommendation=self.body.add_security_recommendation,
+                ),
+                dict(
+                    type=ComponentType.FOOTER.value,
+                    code_expiration_minutes=self.body.code_expiration_minutes,
+                )
+                if self.body.code_expiration_minutes
+                else None,
             )
         else:
             components = (
                 self.body.to_dict(placeholder),
                 self.header.to_dict(placeholder) if self.header else None,
                 self.footer.to_dict() if self.footer else None,
                 dict(
                     type=ComponentType.BUTTONS.value,
-                    buttons=tuple(button.to_dict(placeholder) for button in (
-                        self.buttons if isinstance(self.buttons, Iterable) else (self.buttons,)
-                    ))
-                ) if self.buttons else None
+                    buttons=tuple(
+                        button.to_dict(placeholder)
+                        for button in (
+                            self.buttons
+                            if isinstance(self.buttons, Iterable)
+                            else (self.buttons,)
+                        )
+                    ),
+                )
+                if self.buttons
+                else None,
             )
         return dict(
             name=self.name,
             category=self.category.value,
             language=str(self.language),
-            components=tuple(component for component in components if component is not None)
+            components=tuple(
+                component for component in components if component is not None
+            ),
         )
 
     Language = Language
 
     class Category(utils.StrEnum):
         """
         Template category.
-    
-        `\`Template Categorization\` on
+
+        `'Template Categorization' on
         developers.facebook.com
         <https://developers.facebook.com/docs/whatsapp/business-management-api/message-templates#categories>`_
 
         Attributes:
             AUTHENTICATION: Authentication templates are used to send one-time passwords (OTPs) or codes to app users.
             MARKETING: Marketing templates are used to send promotional messages to app users.
             UTILITY: Utility templates are used to send non-promotional messages to app users.
         """
-        AUTHENTICATION = 'AUTHENTICATION'
-        MARKETING = 'MARKETING'
-        UTILITY = 'UTILITY'
+
+        AUTHENTICATION = "AUTHENTICATION"
+        MARKETING = "MARKETING"
+        UTILITY = "UTILITY"
 
     @dataclasses.dataclass(slots=True)
     class Text(NewTemplateHeaderABC):
         """
         Represents a text header.
-    
+
         Example:
-    
+
             >>> from pywa.types import NewTemplate
             >>> NewTemplate.Text(text='Hello, {John}!')
-    
+
         Attributes:
             text: Text to send with the header (Up to 60 characters. Supports 1 placeholder).
         """
-        type: ComponentType = dataclasses.field(default=ComponentType.HEADER, init=False, repr=False)
-        format: HeaderFormatType = dataclasses.field(default=HeaderFormatType.TEXT, init=False, repr=False)
+
+        type: ComponentType = dataclasses.field(
+            default=ComponentType.HEADER, init=False, repr=False
+        )
+        format: HeaderFormatType = dataclasses.field(
+            default=HeaderFormatType.TEXT, init=False, repr=False
+        )
         text: str
 
         def to_dict(self, placeholder: tuple[str, str] = None) -> dict[str, str | None]:
-            formatted_text, examples = _get_examples_from_placeholders(self.text, *(placeholder if placeholder else ()))
+            formatted_text, examples = _get_examples_from_placeholders(
+                self.text, *(placeholder if placeholder else ())
+            )
             return dict(
                 type=self.type.value,
                 format=self.format.value,
                 text=formatted_text,
-                **(dict(example=dict(header_text=examples)) if examples else {})
+                **(dict(example=dict(header_text=examples)) if examples else {}),
             )
 
     @dataclasses.dataclass(slots=True)
     class Image(NewTemplateHeaderABC):
         """
         Represents an image header.
-    
+
         Example:
             >>> from pywa.types.template import NewTemplate
             >>> NewTemplate.Image(example="2:c2FtcGxl...")
-    
+
         Attributes:
             example: An image handles (Use the `Resumable Upload API
              <https://developers.facebook.com/docs/graph-api/guides/upload>`_ to upload the image)
         """
-        type: ComponentType = dataclasses.field(default=ComponentType.HEADER, init=False, repr=False)
-        format: HeaderFormatType = dataclasses.field(default=HeaderFormatType.IMAGE, init=False, repr=False)
+
+        type: ComponentType = dataclasses.field(
+            default=ComponentType.HEADER, init=False, repr=False
+        )
+        format: HeaderFormatType = dataclasses.field(
+            default=HeaderFormatType.IMAGE, init=False, repr=False
+        )
         example: str
 
         def to_dict(self) -> dict[str, Any]:
             return dict(
                 type=self.type.value,
                 format=self.format.value,
-                example=dict(header_handle=(self.example,))
+                example=dict(header_handle=(self.example,)),
             )
 
     @dataclasses.dataclass(slots=True)
     class Video(NewTemplateHeaderABC):
         """
         Represents a video header.
-    
+
         Example:
             >>> from pywa.types import NewTemplate
             >>> NewTemplate.Video(example="2:c2FtcGxl...")
-    
+
         Attributes:
             example: A video handle (Use the `Resumable Upload API
              <https://developers.facebook.com/docs/graph-api/guides/upload>`_ to upload the video)
         """
-        type: ComponentType = dataclasses.field(default=ComponentType.HEADER, init=False, repr=False)
-        format: HeaderFormatType = dataclasses.field(default=HeaderFormatType.VIDEO, init=False, repr=False)
+
+        type: ComponentType = dataclasses.field(
+            default=ComponentType.HEADER, init=False, repr=False
+        )
+        format: HeaderFormatType = dataclasses.field(
+            default=HeaderFormatType.VIDEO, init=False, repr=False
+        )
         example: str
 
         def to_dict(self) -> dict[str, Any]:
             return dict(
                 type=self.type.value,
                 format=self.format.value,
-                example=dict(header_handle=(self.example,))
+                example=dict(header_handle=(self.example,)),
             )
-        
+
     @dataclasses.dataclass(slots=True)
     class Document(NewTemplateHeaderABC):
         """
         Represents a document header.
-    
+
         Example:
             >>> from pywa.types import NewTemplate
             >>> NewTemplate.Document(example="2:c2FtcGxl...")
-    
+
         Attributes:
             example: A document handle (Use the `Resumable Upload API
              <https://developers.facebook.com/docs/graph-api/guides/upload>`_ to upload the document)
         """
-        type: ComponentType = dataclasses.field(default=ComponentType.HEADER, init=False, repr=False)
-        format: HeaderFormatType = dataclasses.field(default=HeaderFormatType.DOCUMENT, init=False, repr=False)
+
+        type: ComponentType = dataclasses.field(
+            default=ComponentType.HEADER, init=False, repr=False
+        )
+        format: HeaderFormatType = dataclasses.field(
+            default=HeaderFormatType.DOCUMENT, init=False, repr=False
+        )
         example: str
 
         def to_dict(self) -> dict[str, Any]:
             return dict(
                 type=self.type.value,
                 format=self.format.value,
-                example=dict(header_handle=(self.example,))
+                example=dict(header_handle=(self.example,)),
             )
 
     @dataclasses.dataclass(slots=True)
     class Location(NewTemplateHeaderABC):
         """
         Location headers appear as generic maps at the top of the template and are useful for order tracking, delivery
         updates, ride hailing pickup/dropoff, locating physical stores, etc. When tapped, the app user's default map app
         will open and load the specified location. Locations are specified when you send the template.
-    
+
         - Location headers can only be used in templates categorized as ``UTILITY`` or ``MARKETING``. Real-time locations are not supported.
-    
+
         Example:
             >>> from pywa.types import NewTemplate
             >>> NewTemplate.Location()
         """
-        type: ComponentType = dataclasses.field(default=ComponentType.HEADER, init=False, repr=False)
-        format: HeaderFormatType = dataclasses.field(default=HeaderFormatType.LOCATION, init=False, repr=False)
+
+        type: ComponentType = dataclasses.field(
+            default=ComponentType.HEADER, init=False, repr=False
+        )
+        format: HeaderFormatType = dataclasses.field(
+            default=HeaderFormatType.LOCATION, init=False, repr=False
+        )
 
         def to_dict(self) -> dict[str, str]:
             return dict(
                 type=self.type.value,
                 format=self.format.value,
             )
 
     @dataclasses.dataclass(slots=True)
     class Body(NewTemplateComponentABC):
         """
         Represents a template body.
-    
+
         Example:
-    
+
             >>> from pywa.types import NewTemplate
             >>> NewTemplate.Body(
             ...     text='Shop now through {the end of August} and '
             ...         'use code {25OF} to get {25%} off of all merchandise',
             ... )
-    
+
         Attributes:
             text: Text to send with the body (Up to 1024 characters. Supports multiple placeholders).
         """
-        type: ComponentType = dataclasses.field(default=ComponentType.BODY, init=False, repr=False)
+
+        type: ComponentType = dataclasses.field(
+            default=ComponentType.BODY, init=False, repr=False
+        )
         text: str
 
         def to_dict(self, placeholder: tuple[str, str] = None) -> dict[str, str | None]:
-            formatted_text, examples = _get_examples_from_placeholders(self.text, *(placeholder if placeholder else ()))
+            formatted_text, examples = _get_examples_from_placeholders(
+                self.text, *(placeholder if placeholder else ())
+            )
             return dict(
                 type=self.type.value,
                 text=formatted_text,
-                **(dict(example=dict(body_text=(examples,))) if examples else {})
+                **(dict(example=dict(body_text=(examples,))) if examples else {}),
             )
 
     @dataclasses.dataclass(slots=True)
     class AuthBody:
         """
         Represents the configuration for an authentication template.
 
@@ -492,37 +555,38 @@
 
         Attributes:
             code_expiration_minutes: Indicates number of minutes the password or code is valid. If omitted, the code
              expiration warning will not be displayed in the delivered message. (Minimum ``1``, maximum ``90``).
             add_security_recommendation: Set to ``True`` if you want the template to include the string, ``"For your security,
              do not share this code"``. Set to ``False`` to exclude the string. Defaults to ``False``.
         """
+
         code_expiration_minutes: int | None = None
         add_security_recommendation: bool = False
 
     @dataclasses.dataclass(slots=True)
     class Footer(NewTemplateComponentABC):
         """
         Represents a template footer.
-    
+
         Example:
             >>> from pywa.types import NewTemplate
             >>> NewTemplate.Footer(text='Use the link below to log in to your account.')
-    
+
         Attributes:
             text: Text to send with the footer (Up to 60 characters, no placeholders allowed).
         """
-        type: ComponentType = dataclasses.field(default=ComponentType.FOOTER, init=False, repr=False)
+
+        type: ComponentType = dataclasses.field(
+            default=ComponentType.FOOTER, init=False, repr=False
+        )
         text: str
 
         def to_dict(self) -> dict[str, str | None]:
-            return dict(
-                type=self.type.value,
-                text=self.text
-            )
+            return dict(type=self.type.value, text=self.text)
 
     @dataclasses.dataclass(slots=True)
     class PhoneNumberButton(NewButtonABC):
         """
         Phone number buttons call the specified business phone number when tapped by the app user.
         Templates are limited to one phone number button.
 
@@ -533,20 +597,27 @@
             >>> NewTemplate.PhoneNumberButton(title='Call Us', phone_number='12125552368')
 
         Attributes:
             title: Button text (Up to 25 characters, no placeholders allowed).
             phone_number: Alphanumeric string. Business phone number to be (display phone number)
              called when the user taps the button (Up to 20 characters, no placeholders allowed).
         """
-        type: ButtonType = dataclasses.field(default=ButtonType.PHONE_NUMBER, init=False, repr=False)
+
+        type: ButtonType = dataclasses.field(
+            default=ButtonType.PHONE_NUMBER, init=False, repr=False
+        )
         title: str
         phone_number: int | str
 
         def to_dict(self, placeholder: None = None) -> dict[str, str]:
-            return dict(type=self.type.value, text=self.title, phone_number=str(self.phone_number))
+            return dict(
+                type=self.type.value,
+                text=self.title,
+                phone_number=str(self.phone_number),
+            )
 
     @dataclasses.dataclass(slots=True)
     class UrlButton(NewButtonABC):
         """
         URL buttons load the specified URL in the device's default web browser when tapped by the app user.
         Templates are limited to two URL buttons.
 
@@ -558,31 +629,40 @@
             ... )
 
         Attributes:
             title: Button text (Up to 25 characters, supports 1 variable).
             url: URL to be loaded when the user taps the button (Up to 2000 characters, supports 1 placeholder, which
              be appended to the end of the URL).
         """
-        type: ComponentType = dataclasses.field(default=ButtonType.URL, init=False, repr=False)
+
+        type: ComponentType = dataclasses.field(
+            default=ButtonType.URL, init=False, repr=False
+        )
         title: str
         url: str
 
         def to_dict(self, placeholder: tuple[str, str] = None) -> dict[str, str]:
-            formatted_title, title_examples = (
-                _get_examples_from_placeholders(self.title, *(placeholder if placeholder else ()))
+            (
+                formatted_title,
+                title_examples,
+            ) = _get_examples_from_placeholders(
+                self.title, *(placeholder if placeholder else ())
             )
-            formatted_url, url_examples = (
-                _get_examples_from_placeholders(self.url, *(placeholder if placeholder else ()))
+            (
+                formatted_url,
+                url_examples,
+            ) = _get_examples_from_placeholders(
+                self.url, *(placeholder if placeholder else ())
             )
             examples = title_examples + url_examples
             return dict(
                 type=self.type.value,
                 text=formatted_title,
                 url=formatted_url,
-                **(dict(example=examples if examples else {}))
+                **(dict(example=examples if examples else {})),
             )
 
     @dataclasses.dataclass(slots=True)
     class QuickReplyButton(NewButtonABC):
         """
         Quick reply buttons are custom text-only buttons that immediately message you with the specified text string when
         tapped by the app user. A common use case-case is a button that allows your customer to easily opt-out of any
@@ -599,15 +679,18 @@
             >>> from pywa.types import NewTemplate
             >>> NewTemplate.QuickReplyButton(text='Unsubscribe from Promos')
             >>> NewTemplate.QuickReplyButton(text='Unsubscribe from All')
 
         Attributes:
             text: The text to send when the user taps the button (Up to 25 characters, no placeholders allowed).
         """
-        type: ComponentType = dataclasses.field(default=ButtonType.QUICK_REPLY, init=False, repr=False)
+
+        type: ComponentType = dataclasses.field(
+            default=ButtonType.QUICK_REPLY, init=False, repr=False
+        )
         text: str
 
         def to_dict(self, placeholder: None = None) -> dict[str, str]:
             return dict(type=self.type.value, text=self.text)
 
     @dataclasses.dataclass(slots=True)
     class OTPButton(NewButtonABC):
@@ -643,75 +726,101 @@
             autofill_text: One-tap autofill button text. If omitted, the text will default to a pre-set value localized to
                 the template's language. For example, ``Autofill`` for English (US).
             package_name: Android package name of your app. Required if ``otp_type`` is ``OtpType.ONE_TAP``.
             signature_hash: Your app signing key hash. See `App Signing Key Hash
              <https://developers.facebook.com/docs/whatsapp/business-management-api/authentication-templates#app-signing-key-hash>`_
              for more information. Required if ``otp_type`` is ``OtpType.ONE_TAP``.
         """
-        type: ComponentType = dataclasses.field(default=ButtonType.OTP, init=False, repr=False)
+
+        type: ComponentType = dataclasses.field(
+            default=ButtonType.OTP, init=False, repr=False
+        )
         otp_type: OtpType
         title: str | None = None
         autofill_text: str | None = None
         package_name: str | None = None
         signature_hash: str | None = None
 
         class OtpType(utils.StrEnum):
             """
             The type of the button
 
             Attributes:
                 COPY_CODE: Copy code button copies the one-time password or code to the user's clipboard.
                 ONE_TAP: One-tap autofill button automatically loads and passes your app the one-time password or code.
             """
-            COPY_CODE = 'COPY_CODE'
-            ONE_TAP = 'ONE_TAP'
+
+            COPY_CODE = "COPY_CODE"
+            ONE_TAP = "ONE_TAP"
 
         def __post_init__(self):
-            if self.otp_type == self.OtpType.ONE_TAP and not (self.package_name and self.signature_hash):
-                raise ValueError('`package_name` and `signature_hash` are required for ONE_TAP')
+            if self.otp_type == self.OtpType.ONE_TAP and not (
+                self.package_name and self.signature_hash
+            ):
+                raise ValueError(
+                    "`package_name` and `signature_hash` are required for ONE_TAP"
+                )
 
         def to_dict(self, placeholder: None = None) -> dict[str, str | None]:
-            base = dict(type=self.type.value, otp_type=self.otp_type.value, text=self.title)
+            base = dict(
+                type=self.type.value,
+                otp_type=self.otp_type.value,
+                text=self.title,
+            )
             if self.otp_type == self.OtpType.ONE_TAP:
                 base.update(
                     package_name=self.package_name,
                     signature_hash=self.signature_hash,
-                    **(dict(autofill_text=self.autofill_text) if self.autofill_text else {})
+                    **(
+                        dict(autofill_text=self.autofill_text)
+                        if self.autofill_text
+                        else {}
+                    ),
                 )
             return base
 
     @dataclasses.dataclass(slots=True)
     class MPMButton(NewButtonABC):
         """
         Represents a button that can be used to send multi-product message (MPM)
             - This button required providing header to the new template!
 
         Example:
             >>> from pywa.types import NewTemplate
             >>> NewTemplate.MPMButton()
         """
-        type: ComponentType = dataclasses.field(default=ButtonType.MPM, init=False, repr=False)
+
+        type: ComponentType = dataclasses.field(
+            default=ButtonType.MPM, init=False, repr=False
+        )
 
         def to_dict(self, placeholder: None = None) -> dict[str, str]:
-            return dict(type=self.type.value, text='View items')  # required text for MPM button
+            return dict(
+                type=self.type.value, text="View items"
+            )  # required text for MPM button
 
     @dataclasses.dataclass(slots=True)
     class CatalogButton(NewButtonABC):
         """
         Represent a button that can be used to display a catalog.
 
         Example:
             >>> from pywa.types import NewTemplate
             >>> NewTemplate.CatalogButton()
 
         """
-        type: ComponentType = dataclasses.field(default=ButtonType.CATALOG, init=False, repr=False)
+
+        type: ComponentType = dataclasses.field(
+            default=ButtonType.CATALOG, init=False, repr=False
+        )
 
         def to_dict(self, placeholder: None = None) -> dict[str, str]:
-            return dict(type=self.type.value, text='View catalog')  # required text for catalog button
+            return dict(
+                type=self.type.value, text="View catalog"
+            )  # required text for catalog button
 
     @dataclasses.dataclass(slots=True)
     class CopyCodeButton(NewButtonABC):
         """
         Represents a button that can be used to copy coupon codes to the user's clipboard.
             - Only one copy code button is allowed per template.
             - Do not use this button to send one-time passwords (OTPs), Use :class:`NewTemplate.OTPButton` instead.
@@ -720,36 +829,40 @@
             >>> from pywa.types import NewTemplate
             >>> NewTemplate.CopyCodeButton(example='250FF')
 
 
         Attributes:
             example: An example of the coupon code (Up to 15 characters).
         """
-        type: ComponentType = dataclasses.field(default=ButtonType.COPY_CODE, init=False, repr=False)
+
+        type: ComponentType = dataclasses.field(
+            default=ButtonType.COPY_CODE, init=False, repr=False
+        )
         example: str
 
         def to_dict(self, placeholder: tuple[str, str] = None) -> dict[str, str | None]:
             return dict(type=self.type.value, example=self.example)
 
 
 class ParamType(utils.StrEnum):
-    TEXT = 'text'
-    CURRENCY = 'currency'
-    DATE_TIME = 'date_time'
-    DOCUMENT = 'document'
-    IMAGE = 'image'
-    VIDEO = 'video'
-    LOCATION = 'location'
-    BUTTON = 'button'
+    TEXT = "text"
+    CURRENCY = "currency"
+    DATE_TIME = "date_time"
+    DOCUMENT = "document"
+    IMAGE = "image"
+    VIDEO = "video"
+    LOCATION = "location"
+    BUTTON = "button"
 
 
 class ComponentABC(abc.ABC):
     @property
     @abc.abstractmethod
-    def type(self) -> ParamType: ...
+    def type(self) -> ParamType:
+        ...
 
 
 @dataclasses.dataclass(slots=True)
 class Template:
     """
     The template to send.
 
@@ -789,47 +902,75 @@
         name: The name of the template.
         language: The language of the template (See `Template language and locale code
             <https://developers.facebook.com/docs/whatsapp/business-management-api/message-templates/supported-languages>`_).
         body: The body of the template, which can include one or more text variables.
         header: The header of the template (required base on the template you are sending).
         buttons: The buttons to send with the template (required base on the template you are sending).
     """
+
     name: str
     language: Language | str
     body: Iterable[TextValue | Currency | DateTime] | None = None
     header: TextValue | Document | Image | Video | Location | None = None
-    buttons: (Iterable[QuickReplyButtonData | UrlButtonValue]
-              | OTPButtonCode | MPMButton | CatalogButton | CopyCodeButton | None) = None
+    buttons: (
+        Iterable[QuickReplyButtonData | UrlButtonValue]
+        | OTPButtonCode
+        | MPMButton
+        | CatalogButton
+        | CopyCodeButton
+        | None
+    ) = None
 
     def __post_init__(self):
         if isinstance(self.buttons, self.OTPButtonCode):
-            self.body = (self.TextValue(value=self.buttons.code),)  # auth template required the code also in the body
+            self.body = (
+                self.TextValue(value=self.buttons.code),
+            )  # auth template required the code also in the body
 
     def to_dict(self, is_header_url: bool = False) -> dict[str, Any]:
         return dict(
             name=self.name,
             language=dict(code=str(self.language)),
-            components=tuple(comp for comp in (
-                dict(
-                    type=ComponentType.BODY.value,
-                    parameters=tuple(component.to_dict() for component in self.body)
-                ) if self.body else None,
-                dict(
-                    type=ComponentType.HEADER.value,
-                    parameters=(self.header.to_dict(is_header_url),)
-                ) if self.header else None,
-                *((dict(
-                    type=b.type.value,
-                    sub_type=b.sub_type.value,
-                    index=idx,
-                    parameters=(b.to_dict(),)
-                ) for idx, b in enumerate(
-                    self.buttons if isinstance(self.buttons, Iterable) else (self.buttons,)  # case of OTPButtonCode
-                )) if self.buttons is not None else ())
-            ) if comp is not None)
+            components=tuple(
+                comp
+                for comp in (
+                    dict(
+                        type=ComponentType.BODY.value,
+                        parameters=tuple(
+                            component.to_dict() for component in self.body
+                        ),
+                    )
+                    if self.body
+                    else None,
+                    dict(
+                        type=ComponentType.HEADER.value,
+                        parameters=(self.header.to_dict(is_header_url),),
+                    )
+                    if self.header
+                    else None,
+                    *(
+                        (
+                            dict(
+                                type=b.type.value,
+                                sub_type=b.sub_type.value,
+                                index=idx,
+                                parameters=(b.to_dict(),),
+                            )
+                            for idx, b in enumerate(
+                                self.buttons
+                                if isinstance(self.buttons, Iterable)
+                                else (self.buttons,)  # case of OTPButtonCode
+                            )
+                        )
+                        if self.buttons is not None
+                        else ()
+                    ),
+                )
+                if comp is not None
+            ),
         )
 
     Language = Language
 
     @dataclasses.dataclass(slots=True)
     class TextValue(ComponentABC):
         """
@@ -838,15 +979,18 @@
         Example:
             >>> from pywa.types import Template
             >>> Template.TextValue(var='John Doe')  # The template was created with 'Hello, {John}!'
 
         Attributes:
             value: The value to assign to the placeholder.
         """
-        type: ParamType = dataclasses.field(default=ParamType.TEXT, init=False, repr=False)
+
+        type: ParamType = dataclasses.field(
+            default=ParamType.TEXT, init=False, repr=False
+        )
         value: str
 
         def to_dict(self, is_url: None = None) -> dict[str, str]:
             return dict(type=self.type.value, text=self.value)
 
     @dataclasses.dataclass(slots=True)
     class Currency(ComponentABC):
@@ -854,175 +998,217 @@
         Represents a currency variable.
 
         Attributes:
             fallback_value: Default text if localization fails.
             code: ISO 4217 currency code (e.g. USD, EUR, etc.).
             amount_1000: Amount multiplied by 1000.
         """
-        type: ParamType = dataclasses.field(default=ParamType.CURRENCY, init=False, repr=False)
+
+        type: ParamType = dataclasses.field(
+            default=ParamType.CURRENCY, init=False, repr=False
+        )
         fallback_value: str
         code: str
         amount_1000: int
 
         def to_dict(self) -> dict[str, str]:
             return dict(
                 type=self.type.value,
                 currency=dict(
                     fallback_value=self.fallback_value,
                     code=self.code,
-                    amount_1000=self.amount_1000
-                )
+                    amount_1000=self.amount_1000,
+                ),
             )
 
     @dataclasses.dataclass(slots=True)
     class DateTime(ComponentABC):
         """
         Represents a date time variable.
 
         Attributes:
             fallback_value: Default text if localization fails.
         """
-        type: ParamType = dataclasses.field(default=ParamType.DATE_TIME, init=False, repr=False)
+
+        type: ParamType = dataclasses.field(
+            default=ParamType.DATE_TIME, init=False, repr=False
+        )
         fallback_value: str
 
         def to_dict(self) -> dict[str, str]:
             return dict(
                 type=self.type.value,
                 date_time=dict(
                     fallback_value=self.fallback_value,
-                )
+                ),
             )
 
     @dataclasses.dataclass(slots=True)
     class Document(ComponentABC):
         """
         Represents a document.
 
         Attributes:
             document: The document to send (PDF only. either a media ID, URL, file path, bytes, or an open file object).
         """
-        type: ParamType = dataclasses.field(default=ParamType.DOCUMENT, init=False, repr=False)
+
+        type: ParamType = dataclasses.field(
+            default=ParamType.DOCUMENT, init=False, repr=False
+        )
         document: str | bytes | BinaryIO
 
         def to_dict(self, is_url: bool) -> dict[str, str]:
-            return dict(type=self.type.value, document=dict(link=self.document) if is_url else dict(id=self.document))
+            return dict(
+                type=self.type.value,
+                document=dict(link=self.document) if is_url else dict(id=self.document),
+            )
 
     @dataclasses.dataclass(slots=True)
     class Image(ComponentABC):
         """
         Represents an image.
 
         Attributes:
             image: The image to send (either a media ID, URL, file path, bytes, or an open file object).
         """
-        type: ParamType = dataclasses.field(default=ParamType.IMAGE, init=False, repr=False)
+
+        type: ParamType = dataclasses.field(
+            default=ParamType.IMAGE, init=False, repr=False
+        )
         image: str | bytes | BinaryIO
 
         def to_dict(self, is_url: bool) -> dict[str, str]:
-            return dict(type=self.type.value, image=dict(link=self.image) if is_url else dict(id=self.image))
+            return dict(
+                type=self.type.value,
+                image=dict(link=self.image) if is_url else dict(id=self.image),
+            )
 
     @dataclasses.dataclass(slots=True)
     class Video(ComponentABC):
         """
         Represents a video.
 
         Attributes:
             video: The video to send (either a media ID, URL, file path, bytes, or an open file object).
         """
-        type: ParamType = dataclasses.field(default=ParamType.VIDEO, init=False, repr=False)
+
+        type: ParamType = dataclasses.field(
+            default=ParamType.VIDEO, init=False, repr=False
+        )
         video: str | bytes | BinaryIO
 
         def to_dict(self, is_url: bool) -> dict[str, str]:
-            return dict(type=self.type.value, video=dict(link=self.video) if is_url else dict(id=self.video))
+            return dict(
+                type=self.type.value,
+                video=dict(link=self.video) if is_url else dict(id=self.video),
+            )
 
     @dataclasses.dataclass(slots=True)
     class Location(ComponentABC):
         """
         Represents a location.
 
         Attributes:
             latitude: The latitude of the location.
             longitude: The longitude of the location.
             name: The name of the location.
             address: The address of the location.
         """
-        type: ParamType = dataclasses.field(default=ParamType.LOCATION, init=False, repr=False)
+
+        type: ParamType = dataclasses.field(
+            default=ParamType.LOCATION, init=False, repr=False
+        )
         latitude: float
         longitude: float
         name: str | None = None
         address: str | None = None
 
         def to_dict(self) -> dict[str, str]:
             return dict(
                 type=self.type.value,
                 location=dict(
                     latitude=self.latitude,
                     longitude=self.longitude,
                     **(dict(name=self.name) if self.name else {}),
-                    **(dict(address=self.address) if self.address else {})
-                )
+                    **(dict(address=self.address) if self.address else {}),
+                ),
             )
 
     @dataclasses.dataclass(slots=True)
     class QuickReplyButtonData(ComponentABC):
         """
         Represents a quick reply button.
 
         Attributes:
             data: The data to send when the user taps the button
              (you can listen for this data with @on_callback_button decorator).
         """
-        type: ParamType = dataclasses.field(default=ParamType.BUTTON, init=False, repr=False)
-        sub_type: ButtonType = dataclasses.field(default=ButtonType.QUICK_REPLY, init=False, repr=False)
+
+        type: ParamType = dataclasses.field(
+            default=ParamType.BUTTON, init=False, repr=False
+        )
+        sub_type: ButtonType = dataclasses.field(
+            default=ButtonType.QUICK_REPLY, init=False, repr=False
+        )
         data: CallbackDataT
 
         def to_dict(self) -> dict[str, str]:
             return dict(
-                type='payload',
-                payload=_resolve_callback_data(self.data)
+                type="payload",
+                payload=_resolve_callback_data(self.data),
             )
 
     @dataclasses.dataclass(slots=True)
     class UrlButtonValue(ComponentABC):
         """
         Represents a URL button variable.
 
         Example:
             >>> from pywa.types import Template
             >>> Template.UrlButtonValue(value='COUPON123')  # The template was created with 'https://example.com/shop/{COUPON12}'
 
         Attributes:
             value: The value to assign to the variable in the template (appended to the end of the URL).
         """
-        type: ParamType = dataclasses.field(default=ParamType.BUTTON, init=False, repr=False)
-        sub_type: ButtonType = dataclasses.field(default=ButtonType.URL, init=False, repr=False)
+
+        type: ParamType = dataclasses.field(
+            default=ParamType.BUTTON, init=False, repr=False
+        )
+        sub_type: ButtonType = dataclasses.field(
+            default=ButtonType.URL, init=False, repr=False
+        )
         value: str
 
         def to_dict(self) -> dict[str, str]:
-            return dict(type='text', text=self.value)
+            return dict(type="text", text=self.value)
 
     @dataclasses.dataclass(slots=True)
     class OTPButtonCode(ComponentABC):
         """
         Represents an OTP button variable.
 
         Example:
             >>> from pywa.types import Template
             >>> Template.OTPButtonCode(value='123456')
 
         Attributes:
             code: The code to copy or autofill when the user taps the button.
         """
-        type: ParamType = dataclasses.field(default=ParamType.BUTTON, init=False, repr=False)
-        sub_type: ButtonType = dataclasses.field(default=ButtonType.URL, init=False, repr=False)
+
+        type: ParamType = dataclasses.field(
+            default=ParamType.BUTTON, init=False, repr=False
+        )
+        sub_type: ButtonType = dataclasses.field(
+            default=ButtonType.URL, init=False, repr=False
+        )
         code: str
 
         def to_dict(self) -> dict[str, str]:
-            return dict(type='text', text=self.code)
-    
+            return dict(type="text", text=self.code)
+
     @dataclasses.dataclass(slots=True)
     class MPMButton(ComponentABC):
         """
         Represent a multi-product message (MPM) button
 
         Example:
             >>> from pywa.types import Template
@@ -1040,71 +1226,88 @@
             ...     ],
             ... )
 
         Attributes:
             thumbnail_product_sku: The thumbnail of this item will be used as the template message's header image.
             product_sections: The product sections to send with the template.
         """
-        type: ParamType = dataclasses.field(default=ParamType.BUTTON, init=False, repr=False)
-        sub_type: ButtonType = dataclasses.field(default=ButtonType.MPM, init=False, repr=False)
+
+        type: ParamType = dataclasses.field(
+            default=ParamType.BUTTON, init=False, repr=False
+        )
+        sub_type: ButtonType = dataclasses.field(
+            default=ButtonType.MPM, init=False, repr=False
+        )
         thumbnail_product_sku: str
         product_sections: Iterable[ProductsSection]
 
         def to_dict(self) -> dict[str, str]:
             return dict(
-                type='action',
+                type="action",
                 action=dict(
                     thumbnail_product_retailer_id=self.thumbnail_product_sku,
-                    sections=tuple(section.to_dict() for section in self.product_sections)
-                )
+                    sections=tuple(
+                        section.to_dict() for section in self.product_sections
+                    ),
+                ),
             )
-    
+
     @dataclasses.dataclass(slots=True)
     class CatalogButton(ComponentABC):
         """
         Represent a catalog button
 
         Example:
             >>> from pywa.types import Template
             >>> Template.CatalogButton(thumbnail_product_sku='IPHONE_15')
 
         Attributes:
             thumbnail_product_sku: The thumbnail of this item will be used as the message's header image. if not
                 provided, the product image of the first item in your catalog will be used.
         """
-        type: ParamType = dataclasses.field(default=ParamType.BUTTON, init=False, repr=False)
-        sub_type: ButtonType = dataclasses.field(default=ButtonType.CATALOG, init=False, repr=False)
+
+        type: ParamType = dataclasses.field(
+            default=ParamType.BUTTON, init=False, repr=False
+        )
+        sub_type: ButtonType = dataclasses.field(
+            default=ButtonType.CATALOG, init=False, repr=False
+        )
         thumbnail_product_sku: str | None = None
 
         def to_dict(self) -> dict[str, str]:
             return dict(
-                type='action',
+                type="action",
                 action=dict(
                     thumbnail_product_retailer_id=self.thumbnail_product_sku,
-                )
+                ),
             )
 
     @dataclasses.dataclass(slots=True)
     class CopyCodeButton(ComponentABC):
         """
         Represents a copy code button variable (copies the code to the user's clipboard).
 
         Example:
             >>> from pywa.types import Template
             >>> Template.CopyCodeButton(code='COUPON123')
 
         Attributes:
             code: The code to copy when the user taps the button.
         """
-        type: ParamType = dataclasses.field(default=ParamType.BUTTON, init=False, repr=False)
-        sub_type: ButtonType = dataclasses.field(default=ButtonType.COPY_CODE, init=False, repr=False)
+
+        type: ParamType = dataclasses.field(
+            default=ParamType.BUTTON, init=False, repr=False
+        )
+        sub_type: ButtonType = dataclasses.field(
+            default=ButtonType.COPY_CODE, init=False, repr=False
+        )
         code: str
 
         def to_dict(self) -> dict[str, str]:
-            return dict(type='coupon_code', coupon_code=self.code)
+            return dict(type="coupon_code", coupon_code=self.code)
 
 
 @dataclasses.dataclass(slots=True, frozen=True, kw_only=True)
 class TemplateStatus(BaseUpdate):
     """
     Represents status of a template.
 
@@ -1115,39 +1318,47 @@
         message_template_id: The ID of the template.
         message_template_name: The name of the template.
         message_template_language: The language of the template.
         reason: The reason the template was rejected (if applicable).
         disable_date: The date the template was disabled (if applicable).
         other_info: Additional information about the template (if applicable).
     """
+
     id: str
     timestamp: datetime
     event: TemplateEvent
     message_template_id: int
     message_template_name: str
     message_template_language: str
     reason: TemplateRejectionReason
     disable_date: str | None = None
     other_info: str | None = None
 
     @classmethod
     def from_update(cls, client: WhatsApp, update: dict) -> TemplateStatus:
-        value = (data := update['entry'][0])['changes'][0]['value']
+        value = (data := update["entry"][0])["changes"][0]["value"]
         return cls(
             _client=client,
-            id=data['id'],
-            timestamp=datetime.fromtimestamp(data['time']),
-            event=cls.TemplateEvent(value['event']),
-            message_template_id=value['message_template_id'],
-            message_template_name=value['message_template_name'],
-            message_template_language=value['message_template_language'],
-            reason=cls.TemplateRejectionReason(str(value.get('reason'))),  # _missing_(str(None)) -> .NONE
-            disable_date=value.get('disable_date'),
-            other_info=(str((oi := value['other_info']).get('title')) + ': '
-                        + str(oi.get('description'))) if 'other_info' in value else None,
+            id=data["id"],
+            timestamp=datetime.fromtimestamp(data["time"]),
+            event=cls.TemplateEvent(value["event"]),
+            message_template_id=value["message_template_id"],
+            message_template_name=value["message_template_name"],
+            message_template_language=value["message_template_language"],
+            reason=cls.TemplateRejectionReason(
+                str(value.get("reason"))
+            ),  # _missing_(str(None)) -> .NONE
+            disable_date=value.get("disable_date"),
+            other_info=(
+                str((oi := value["other_info"]).get("title"))
+                + ": "
+                + str(oi.get("description"))
+            )
+            if "other_info" in value
+            else None,
         )
 
     class TemplateEvent(utils.StrEnum):
         """
         The event that occurred (the template was approved, rejected, etc.).
 
         Attributes:
@@ -1158,24 +1369,25 @@
             REINSTATED: The template was reinstated.
             REJECTED: The template was rejected.
             PENDING_DELETION: The template is pending deletion.
             FLAGGED: The template was flagged.
             PAUSED: The template was paused.
             UNKNOWN: Unknown event.
         """
-        APPROVED = 'APPROVED'
-        DISABLED = 'DISABLED'
-        IN_APPEAL = 'IN_APPEAL'
-        PENDING = 'PENDING'
-        REINSTATED = 'REINSTATED'
-        REJECTED = 'REJECTED'
-        PENDING_DELETION = 'PENDING_DELETION'
-        FLAGGED = 'FLAGGED'
-        PAUSED = 'PAUSED'
-        UNKNOWN = 'UNKNOWN'
+
+        APPROVED = "APPROVED"
+        DISABLED = "DISABLED"
+        IN_APPEAL = "IN_APPEAL"
+        PENDING = "PENDING"
+        REINSTATED = "REINSTATED"
+        REJECTED = "REJECTED"
+        PENDING_DELETION = "PENDING_DELETION"
+        FLAGGED = "FLAGGED"
+        PAUSED = "PAUSED"
+        UNKNOWN = "UNKNOWN"
 
         @classmethod
         def _missing_(cls, value: str) -> TemplateStatus.TemplateEvent:
             return cls.UNKNOWN
 
     class TemplateRejectionReason(utils.StrEnum):
         """
@@ -1184,16 +1396,17 @@
         Attributes:
             ABUSIVE_CONTENT: The template was rejected because it contained abusive content.
             INCORRECT_CATEGORY: The template was rejected because it was in the wrong category.
             INVALID_FORMAT: The template was rejected because it was in the wrong format.
             SCAM: The template was rejected because it was a scam.
             NONE: The template was not rejected.
         """
-        ABUSIVE_CONTENT = 'ABUSIVE_CONTENT'
-        INCORRECT_CATEGORY = 'INCORRECT_CATEGORY'
-        INVALID_FORMAT = 'INVALID_FORMAT'
-        SCAM = 'SCAM'
-        NONE = 'NONE'
+
+        ABUSIVE_CONTENT = "ABUSIVE_CONTENT"
+        INCORRECT_CATEGORY = "INCORRECT_CATEGORY"
+        INVALID_FORMAT = "INVALID_FORMAT"
+        SCAM = "SCAM"
+        NONE = "NONE"
 
         @classmethod
         def _missing_(cls, value: str):
             return cls.NONE
```

### Comparing `pywa-1.8.0/pywa/utils.py` & `pywa-1.9.0/pywa/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, fields
 from enum import Enum
 from importlib import import_module
-from typing import Protocol, Any, Callable
+from typing import Any, Callable, Protocol
 
 
 def is_fastapi_app(app):
     """Check if the app is a FastAPI app."""
     try:
         return isinstance(app, import_module("fastapi").FastAPI)
     except ImportError:
@@ -34,25 +34,23 @@
 class FromDict:
     """Allows to ignore extra fields when creating a dataclass from a dict."""
 
     # noinspection PyArgumentList
     @classmethod
     def from_dict(cls, data: dict, **kwargs):
         data.update(kwargs)
-        return cls(**{
-            k: v for k, v in data.items()
-            if k in (f.name for f in fields(cls))
-        })
+        return cls(
+            **{k: v for k, v in data.items() if k in (f.name for f in fields(cls))}
+        )
 
 
 class FastAPI(Protocol):
     def get(self, path: str) -> Callable:
         ...
 
     def post(self, path: str) -> Callable:
         ...
 
 
 class Flask(Protocol):
     def route(self, rule: str, **options: Any) -> Callable:
         ...
-
```

### Comparing `pywa-1.8.0/pywa.egg-info/PKG-INFO` & `pywa-1.9.0/pywa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pywa
-Version: 1.8.0
+Version: 1.9.0
 Summary: Python wrapper for the WhatsApp Cloud API
 Author-email: David Lev <davidlev@telegmail.com>
 License: MIT
 Project-URL: Documentation, https://pywa.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/david-lev/pywa/issues
 Project-URL: Source Code, https://github.com/david-lev/pywa
 Project-URL: Funding, https://github.com/sponsors/david-lev
+Project-URL: Changelog, https://github.com/david-lev/pywa/blob/master/CHANGELOG.md
 Keywords: whatsapp,whatsapp-api,whatsapp-cloud-api,whatsapp-cloud,whatsapp-api-python,whatsapp-cloud-api-python,pywa,wapy,wa,wa-api,wa-cloud-api,wa-cloud,wa-api-python,wa-cloud-api-python,whatsapp-webhook,whatsapp-webhook-python,whatsapp-webhook-api
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Communications
 Classifier: Topic :: Utilities
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pywa-1.8.0/pywa.egg-info/SOURCES.txt` & `pywa-1.9.0/pywa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywa-1.8.0/tests/test_callback_data.py` & `pywa-1.9.0/tests/test_callback_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,148 +1,173 @@
-import pytest
 import dataclasses
+
+import pytest
+
 from pywa.types import CallbackData
 
 
 def test_callback_class_uniqueness():
     """Test the uniqueness of the callback data."""
+
     @dataclasses.dataclass(slots=True, frozen=True)
     class User(CallbackData):
         id: str
         name: str
         is_admin: bool
 
     @dataclasses.dataclass(slots=True, frozen=True)
     class Group(CallbackData):
         id: str
         name: str
 
-    assert User.__callback_id__ != Group.__callback_id__, 'The callback id must be unique for each child class.'
+    assert (
+        User.__callback_id__ != Group.__callback_id__
+    ), "The callback id must be unique for each child class."
 
 
 def test_callback_class_not_empty():
     """Test if the callback data is empty."""
     with pytest.raises(TypeError):
 
         @dataclasses.dataclass(slots=True, frozen=True)
-        class User(CallbackData):
+        class User1(CallbackData):
             pass
 
     with pytest.raises(TypeError):
+
         @dataclasses.dataclass(slots=True, frozen=True)
-        class User(CallbackData):
+        class User2(CallbackData):
             id: str
             name: str
             is_admin: bool
             x: int
 
         @dataclasses.dataclass(slots=True, frozen=True)
-        class UserChild(User):
+        class UserChild(User2):
             pass
 
 
 def test_callback_supported_types():
     """Test the supported types of the callback data."""
     with pytest.raises(TypeError):
+
         @dataclasses.dataclass(slots=True, frozen=True)
         class User(CallbackData):
             id: int
             name: str
             is_admin: bool
             x: dict
             y: list
             z: set
 
 
 def test_data():
     """Test the callback data."""
+
     @dataclasses.dataclass(slots=True, frozen=True)
     class User(CallbackData):
         id: int
         name: str
         is_admin: bool
 
-    assert User(id=1234, name='xxx', is_admin=True).to_str() == '7~1234~xxx~§'
-    assert User(id=3456, name='yyy', is_admin=False).to_str() == '7~3456~yyy~'
-    assert User.from_str('1~1234~xxx~§') == User(id=1234, name='xxx', is_admin=True)
-    assert User.from_str('1~3456~yyy~') == User(id=3456, name='yyy', is_admin=False)
+    assert User(id=1234, name="xxx", is_admin=True).to_str() == "7~1234~xxx~§"
+    assert User(id=3456, name="yyy", is_admin=False).to_str() == "7~3456~yyy~"
+    assert User.from_str("1~1234~xxx~§") == User(id=1234, name="xxx", is_admin=True)
+    assert User.from_str("1~3456~yyy~") == User(id=3456, name="yyy", is_admin=False)
 
     with pytest.raises(ValueError):  # too few fields
-        User.from_str('1~3456')
+        User.from_str("1~3456")
 
     with pytest.raises(ValueError):  # too many fields
-        User.from_str('1~3456~yyy~§~')
+        User.from_str("1~3456~yyy~§~")
 
     with pytest.raises(ValueError):  # invalid type
-        User.from_str('1~x~yyy~§')
+        User.from_str("1~x~yyy~§")
 
 
 def test_multiple_data():
     """Test multiple callback data."""
+
     @dataclasses.dataclass(slots=True, frozen=True)
     class User(CallbackData):
         id: str
         name: str
         is_admin: bool
 
     @dataclasses.dataclass(slots=True, frozen=True)
     class Group(CallbackData):
         id: str
         name: str
 
-    user = User(id='1234', name='xxx', is_admin=True)
-    group = Group(id='3456', name='yyy')
-    assert CallbackData.join_to_str(user, group) == '9~1234~xxx~§¶11~3456~yyy'
-    assert CallbackData.join_to_str(user, group, user) == '9~1234~xxx~§¶11~3456~yyy¶9~1234~xxx~§'
-    x, y = '3~1234~xxx~§¶5~3456~yyy'.split(CallbackData.__callback_sep__)
+    user = User(id="1234", name="xxx", is_admin=True)
+    group = Group(id="3456", name="yyy")
+    assert CallbackData.join_to_str(user, group) == "9~1234~xxx~§¶11~3456~yyy"
+    assert (
+        CallbackData.join_to_str(user, group, user)
+        == "9~1234~xxx~§¶11~3456~yyy¶9~1234~xxx~§"
+    )
+    x, y = "3~1234~xxx~§¶5~3456~yyy".split(CallbackData.__callback_sep__)
     assert (User.from_str(x), Group.from_str(y)) == (user, group)
-    x, y, z = '3~1234~xxx~§¶5~3456~yyy¶3~1234~xxx~§'.split(CallbackData.__callback_sep__)
-    assert (User.from_str(x), Group.from_str(y), User.from_str(z)) == (user, group, user)
+    x, y, z = "3~1234~xxx~§¶5~3456~yyy¶3~1234~xxx~§".split(
+        CallbackData.__callback_sep__
+    )
+    assert (User.from_str(x), Group.from_str(y), User.from_str(z)) == (
+        user,
+        group,
+        user,
+    )
 
 
 def test_data_sep():
     """Test the data separator override."""
+
     @dataclasses.dataclass(slots=True, frozen=True)
     class User(CallbackData):
-        __callback_data_sep__ = '*'
+        __callback_data_sep__ = "*"
         id: int
         name: str
         is_admin: bool
 
-    assert User(id=1234, name='xxx', is_admin=True).to_str() == '13*1234*xxx*§'
-    assert User(id=3456, name='yyy', is_admin=False).to_str() == '13*3456*yyy*'
+    assert User(id=1234, name="xxx", is_admin=True).to_str() == "13*1234*xxx*§"
+    assert User(id=3456, name="yyy", is_admin=False).to_str() == "13*3456*yyy*"
 
     with pytest.raises(ValueError):
-        User.from_str('1*3456*David*Lev*')
+        User.from_str("1*3456*David*Lev*")
 
     try:
-        User.from_str('1*3456*David~Lev*')
+        User.from_str("1*3456*David~Lev*")
     except ValueError:
-        pytest.fail('The data separator override does not work.')
+        pytest.fail("The data separator override does not work.")
 
 
 def test_data_sep_multiple_data():
     """Test the data separator override with multiple data."""
-    CallbackData.__callback_sep__ = '^'
+    CallbackData.__callback_sep__ = "^"
 
     @dataclasses.dataclass(slots=True, frozen=True)
     class User(CallbackData):
         id: int
         name: str
         is_admin: bool
 
     @dataclasses.dataclass(slots=True, frozen=True)
     class Group(CallbackData):
         id: int
         name: str
 
-    user = User(id=1234, name='xxx', is_admin=True)
-    group = Group(id=3456, name='yyy')
-    assert CallbackData.join_to_str(user, group) == '15~1234~xxx~§^17~3456~yyy'
-    assert CallbackData.join_to_str(user, group, user) == '15~1234~xxx~§^17~3456~yyy^15~1234~xxx~§'
-    x, y = '3~1234~xxx~§^5~3456~yyy'.split(CallbackData.__callback_sep__)
+    user = User(id=1234, name="xxx", is_admin=True)
+    group = Group(id=3456, name="yyy")
+    assert CallbackData.join_to_str(user, group) == "15~1234~xxx~§^17~3456~yyy"
+    assert (
+        CallbackData.join_to_str(user, group, user)
+        == "15~1234~xxx~§^17~3456~yyy^15~1234~xxx~§"
+    )
+    x, y = "3~1234~xxx~§^5~3456~yyy".split(CallbackData.__callback_sep__)
     assert (User.from_str(x), Group.from_str(y)) == (user, group)
-    x, y, z = '3~1234~xxx~§^5~3456~yyy^3~1234~xxx~§'.split(CallbackData.__callback_sep__)
-    assert (User.from_str(x), Group.from_str(y), User.from_str(z)) == (user, group, user)
-
-
-
+    x, y, z = "3~1234~xxx~§^5~3456~yyy^3~1234~xxx~§".split(
+        CallbackData.__callback_sep__
+    )
+    assert (User.from_str(x), Group.from_str(y), User.from_str(z)) == (
+        user,
+        group,
+        user,
+    )
```

