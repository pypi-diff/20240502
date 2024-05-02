# Comparing `tmp/celestical-0.14.3-py3-none-any.whl.zip` & `tmp/celestical-0.9.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,57 +1,61 @@
-Zip file size: 112250 bytes, number of entries: 55
+Zip file size: 115023 bytes, number of entries: 59
 -rw-r--r--  2.0 unx    35150 b- defN 80-Jan-01 00:00 COPYING
 -rw-r--r--  2.0 unx     7653 b- defN 80-Jan-01 00:00 COPYING.LESSER
 -rw-r--r--  2.0 unx      108 b- defN 80-Jan-01 00:00 LICENSE
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 celestical/__init__.py
--rw-r--r--  2.0 unx     2695 b- defN 80-Jan-01 00:00 celestical/api/__init__.py
+-rw-r--r--  2.0 unx     2650 b- defN 80-Jan-01 00:00 celestical/api/__init__.py
 -rw-r--r--  2.0 unx      246 b- defN 80-Jan-01 00:00 celestical/api/api/__init__.py
--rw-r--r--  2.0 unx    51216 b- defN 80-Jan-01 00:00 celestical/api/api/app_api.py
--rw-r--r--  2.0 unx    79145 b- defN 80-Jan-01 00:00 celestical/api/api/auth_api.py
--rw-r--r--  2.0 unx     9886 b- defN 80-Jan-01 00:00 celestical/api/api/default_api.py
--rw-r--r--  2.0 unx    51169 b- defN 80-Jan-01 00:00 celestical/api/api/users_api.py
--rw-r--r--  2.0 unx    24570 b- defN 80-Jan-01 00:00 celestical/api/api_client.py
+-rw-r--r--  2.0 unx    51215 b- defN 80-Jan-01 00:00 celestical/api/api/app_api.py
+-rw-r--r--  2.0 unx    79144 b- defN 80-Jan-01 00:00 celestical/api/api/auth_api.py
+-rw-r--r--  2.0 unx     9885 b- defN 80-Jan-01 00:00 celestical/api/api/default_api.py
+-rw-r--r--  2.0 unx    10780 b- defN 80-Jan-01 00:00 celestical/api/api/stacy_api.py
+-rw-r--r--  2.0 unx    51168 b- defN 80-Jan-01 00:00 celestical/api/api/users_api.py
+-rw-r--r--  2.0 unx    24568 b- defN 80-Jan-01 00:00 celestical/api/api_client.py
 -rw-r--r--  2.0 unx      674 b- defN 80-Jan-01 00:00 celestical/api/api_response.py
--rw-r--r--  2.0 unx    14610 b- defN 80-Jan-01 00:00 celestical/api/configuration.py
--rw-r--r--  2.0 unx     5940 b- defN 80-Jan-01 00:00 celestical/api/exceptions.py
--rw-r--r--  2.0 unx     1953 b- defN 80-Jan-01 00:00 celestical/api/models/__init__.py
--rw-r--r--  2.0 unx     3731 b- defN 80-Jan-01 00:00 celestical/api/models/app.py
--rw-r--r--  2.0 unx     2939 b- defN 80-Jan-01 00:00 celestical/api/models/bearer_response.py
--rw-r--r--  2.0 unx     2691 b- defN 80-Jan-01 00:00 celestical/api/models/body_reset_forgot_password_auth_forgot_password_post.py
--rw-r--r--  2.0 unx     2983 b- defN 80-Jan-01 00:00 celestical/api/models/body_reset_reset_password_auth_reset_password_post.py
--rw-r--r--  2.0 unx     2703 b- defN 80-Jan-01 00:00 celestical/api/models/body_verify_request_token_auth_request_verify_token_post.py
--rw-r--r--  2.0 unx     2631 b- defN 80-Jan-01 00:00 celestical/api/models/body_verify_verify_auth_verify_post.py
--rw-r--r--  2.0 unx     4815 b- defN 80-Jan-01 00:00 celestical/api/models/client_id.py
--rw-r--r--  2.0 unx     4843 b- defN 80-Jan-01 00:00 celestical/api/models/client_secret.py
--rw-r--r--  2.0 unx     4787 b- defN 80-Jan-01 00:00 celestical/api/models/code.py
--rw-r--r--  2.0 unx     3041 b- defN 80-Jan-01 00:00 celestical/api/models/compose.py
--rw-r--r--  2.0 unx     4801 b- defN 80-Jan-01 00:00 celestical/api/models/deploy.py
--rw-r--r--  2.0 unx     4912 b- defN 80-Jan-01 00:00 celestical/api/models/detail.py
--rw-r--r--  2.0 unx     2605 b- defN 80-Jan-01 00:00 celestical/api/models/error_model.py
--rw-r--r--  2.0 unx     4822 b- defN 80-Jan-01 00:00 celestical/api/models/grant_type.py
--rw-r--r--  2.0 unx     2602 b- defN 80-Jan-01 00:00 celestical/api/models/http_validation_error.py
--rw-r--r--  2.0 unx     4815 b- defN 80-Jan-01 00:00 celestical/api/models/is_active.py
--rw-r--r--  2.0 unx     4836 b- defN 80-Jan-01 00:00 celestical/api/models/is_superuser.py
--rw-r--r--  2.0 unx     4829 b- defN 80-Jan-01 00:00 celestical/api/models/is_verified.py
--rw-r--r--  2.0 unx     2639 b- defN 80-Jan-01 00:00 celestical/api/models/missing_images.py
--rw-r--r--  2.0 unx     4787 b- defN 80-Jan-01 00:00 celestical/api/models/name.py
--rw-r--r--  2.0 unx     2920 b- defN 80-Jan-01 00:00 celestical/api/models/uploaded_image.py
--rw-r--r--  2.0 unx     4757 b- defN 80-Jan-01 00:00 celestical/api/models/user_create.py
--rw-r--r--  2.0 unx     4111 b- defN 80-Jan-01 00:00 celestical/api/models/user_read.py
--rw-r--r--  2.0 unx     3083 b- defN 80-Jan-01 00:00 celestical/api/models/validation_error.py
+-rw-r--r--  2.0 unx    14608 b- defN 80-Jan-01 00:00 celestical/api/configuration.py
+-rw-r--r--  2.0 unx     5939 b- defN 80-Jan-01 00:00 celestical/api/exceptions.py
+-rw-r--r--  2.0 unx     1908 b- defN 80-Jan-01 00:00 celestical/api/models/__init__.py
+-rw-r--r--  2.0 unx     3730 b- defN 80-Jan-01 00:00 celestical/api/models/app.py
+-rw-r--r--  2.0 unx     2938 b- defN 80-Jan-01 00:00 celestical/api/models/bearer_response.py
+-rw-r--r--  2.0 unx     2690 b- defN 80-Jan-01 00:00 celestical/api/models/body_reset_forgot_password_auth_forgot_password_post.py
+-rw-r--r--  2.0 unx     2982 b- defN 80-Jan-01 00:00 celestical/api/models/body_reset_reset_password_auth_reset_password_post.py
+-rw-r--r--  2.0 unx     2702 b- defN 80-Jan-01 00:00 celestical/api/models/body_verify_request_token_auth_request_verify_token_post.py
+-rw-r--r--  2.0 unx     2630 b- defN 80-Jan-01 00:00 celestical/api/models/body_verify_verify_auth_verify_post.py
+-rw-r--r--  2.0 unx     4814 b- defN 80-Jan-01 00:00 celestical/api/models/client_id.py
+-rw-r--r--  2.0 unx     4842 b- defN 80-Jan-01 00:00 celestical/api/models/client_secret.py
+-rw-r--r--  2.0 unx     3040 b- defN 80-Jan-01 00:00 celestical/api/models/compose.py
+-rw-r--r--  2.0 unx     4800 b- defN 80-Jan-01 00:00 celestical/api/models/deploy.py
+-rw-r--r--  2.0 unx     4911 b- defN 80-Jan-01 00:00 celestical/api/models/detail.py
+-rw-r--r--  2.0 unx     2604 b- defN 80-Jan-01 00:00 celestical/api/models/error_model.py
+-rw-r--r--  2.0 unx     4842 b- defN 80-Jan-01 00:00 celestical/api/models/first_creator.py
+-rw-r--r--  2.0 unx     4821 b- defN 80-Jan-01 00:00 celestical/api/models/grant_type.py
+-rw-r--r--  2.0 unx     2601 b- defN 80-Jan-01 00:00 celestical/api/models/http_validation_error.py
+-rw-r--r--  2.0 unx     4814 b- defN 80-Jan-01 00:00 celestical/api/models/is_active.py
+-rw-r--r--  2.0 unx     4835 b- defN 80-Jan-01 00:00 celestical/api/models/is_superuser.py
+-rw-r--r--  2.0 unx     4828 b- defN 80-Jan-01 00:00 celestical/api/models/is_verified.py
+-rw-r--r--  2.0 unx     2622 b- defN 80-Jan-01 00:00 celestical/api/models/missing_apps.py
+-rw-r--r--  2.0 unx     2638 b- defN 80-Jan-01 00:00 celestical/api/models/missing_images.py
+-rw-r--r--  2.0 unx     4786 b- defN 80-Jan-01 00:00 celestical/api/models/name.py
+-rw-r--r--  2.0 unx     4225 b- defN 80-Jan-01 00:00 celestical/api/models/stack.py
+-rw-r--r--  2.0 unx     2919 b- defN 80-Jan-01 00:00 celestical/api/models/uploaded_image.py
+-rw-r--r--  2.0 unx     4425 b- defN 80-Jan-01 00:00 celestical/api/models/user_create.py
+-rw-r--r--  2.0 unx     4110 b- defN 80-Jan-01 00:00 celestical/api/models/user_read.py
+-rw-r--r--  2.0 unx     3082 b- defN 80-Jan-01 00:00 celestical/api/models/validation_error.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 celestical/api/py.typed
--rw-r--r--  2.0 unx     9782 b- defN 80-Jan-01 00:00 celestical/api/rest.py
+-rw-r--r--  2.0 unx     9781 b- defN 80-Jan-01 00:00 celestical/api/rest.py
 -rw-r--r--  2.0 unx     1533 b- defN 80-Jan-01 00:00 celestical/apps.py
--rw-r--r--  2.0 unx     2579 b- defN 80-Jan-01 00:00 celestical/cli.py
--rw-r--r--  2.0 unx    17242 b- defN 80-Jan-01 00:00 celestical/compose.py
--rw-r--r--  2.0 unx     6010 b- defN 80-Jan-01 00:00 celestical/configuration.py
--rw-r--r--  2.0 unx     8793 b- defN 80-Jan-01 00:00 celestical/docker_local.py
--rw-r--r--  2.0 unx     6601 b- defN 80-Jan-01 00:00 celestical/helper.py
--rw-r--r--  2.0 unx     7294 b- defN 80-Jan-01 00:00 celestical/user.py
--rw-r--r--  2.0 unx    35150 b- defN 80-Jan-01 00:00 celestical-0.14.3.dist-info/COPYING
--rw-r--r--  2.0 unx     7653 b- defN 80-Jan-01 00:00 celestical-0.14.3.dist-info/COPYING.LESSER
--rw-r--r--  2.0 unx      108 b- defN 80-Jan-01 00:00 celestical-0.14.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     2587 b- defN 80-Jan-01 00:00 celestical-0.14.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 celestical-0.14.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 80-Jan-01 00:00 celestical-0.14.3.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     4903 b- defN 16-Jan-01 00:00 celestical-0.14.3.dist-info/RECORD
-55 files, 487070 bytes uncompressed, 104392 bytes compressed:  78.6%
+-rw-r--r--  2.0 unx     2425 b- defN 80-Jan-01 00:00 celestical/cli.py
+-rw-r--r--  2.0 unx    17341 b- defN 80-Jan-01 00:00 celestical/compose.py
+-rw-r--r--  2.0 unx     3900 b- defN 80-Jan-01 00:00 celestical/configuration.py
+-rw-r--r--  2.0 unx     6138 b- defN 80-Jan-01 00:00 celestical/docker_local.py
+-rw-r--r--  2.0 unx     6457 b- defN 80-Jan-01 00:00 celestical/helper.py
+-rw-r--r--  2.0 unx        9 b- defN 80-Jan-01 00:00 celestical/stack_upload.py
+-rw-r--r--  2.0 unx     6428 b- defN 80-Jan-01 00:00 celestical/user.py
+-rw-r--r--  2.0 unx    35150 b- defN 80-Jan-01 00:00 celestical-0.9.2.dist-info/COPYING
+-rw-r--r--  2.0 unx     7653 b- defN 80-Jan-01 00:00 celestical-0.9.2.dist-info/COPYING.LESSER
+-rw-r--r--  2.0 unx      108 b- defN 80-Jan-01 00:00 celestical-0.9.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1959 b- defN 80-Jan-01 00:00 celestical-0.9.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 celestical-0.9.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 80-Jan-01 00:00 celestical-0.9.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     5255 b- defN 16-Jan-01 00:00 celestical-0.9.2.dist-info/RECORD
+59 files, 498201 bytes uncompressed, 106609 bytes compressed:  78.6%
```

## zipnote {}

```diff
@@ -21,14 +21,17 @@
 
 Filename: celestical/api/api/auth_api.py
 Comment: 
 
 Filename: celestical/api/api/default_api.py
 Comment: 
 
+Filename: celestical/api/api/stacy_api.py
+Comment: 
+
 Filename: celestical/api/api/users_api.py
 Comment: 
 
 Filename: celestical/api/api_client.py
 Comment: 
 
 Filename: celestical/api/api_response.py
@@ -63,29 +66,29 @@
 
 Filename: celestical/api/models/client_id.py
 Comment: 
 
 Filename: celestical/api/models/client_secret.py
 Comment: 
 
-Filename: celestical/api/models/code.py
-Comment: 
-
 Filename: celestical/api/models/compose.py
 Comment: 
 
 Filename: celestical/api/models/deploy.py
 Comment: 
 
 Filename: celestical/api/models/detail.py
 Comment: 
 
 Filename: celestical/api/models/error_model.py
 Comment: 
 
+Filename: celestical/api/models/first_creator.py
+Comment: 
+
 Filename: celestical/api/models/grant_type.py
 Comment: 
 
 Filename: celestical/api/models/http_validation_error.py
 Comment: 
 
 Filename: celestical/api/models/is_active.py
@@ -93,20 +96,26 @@
 
 Filename: celestical/api/models/is_superuser.py
 Comment: 
 
 Filename: celestical/api/models/is_verified.py
 Comment: 
 
+Filename: celestical/api/models/missing_apps.py
+Comment: 
+
 Filename: celestical/api/models/missing_images.py
 Comment: 
 
 Filename: celestical/api/models/name.py
 Comment: 
 
+Filename: celestical/api/models/stack.py
+Comment: 
+
 Filename: celestical/api/models/uploaded_image.py
 Comment: 
 
 Filename: celestical/api/models/user_create.py
 Comment: 
 
 Filename: celestical/api/models/user_read.py
@@ -135,32 +144,35 @@
 
 Filename: celestical/docker_local.py
 Comment: 
 
 Filename: celestical/helper.py
 Comment: 
 
+Filename: celestical/stack_upload.py
+Comment: 
+
 Filename: celestical/user.py
 Comment: 
 
-Filename: celestical-0.14.3.dist-info/COPYING
+Filename: celestical-0.9.2.dist-info/COPYING
 Comment: 
 
-Filename: celestical-0.14.3.dist-info/COPYING.LESSER
+Filename: celestical-0.9.2.dist-info/COPYING.LESSER
 Comment: 
 
-Filename: celestical-0.14.3.dist-info/LICENSE
+Filename: celestical-0.9.2.dist-info/LICENSE
 Comment: 
 
-Filename: celestical-0.14.3.dist-info/METADATA
+Filename: celestical-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: celestical-0.14.3.dist-info/WHEEL
+Filename: celestical-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: celestical-0.14.3.dist-info/entry_points.txt
+Filename: celestical-0.9.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: celestical-0.14.3.dist-info/RECORD
+Filename: celestical-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## celestical/api/__init__.py

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 __version__ = "1.0.0"
@@ -38,15 +38,14 @@
 from celestical.api.models.bearer_response import BearerResponse
 from celestical.api.models.body_reset_forgot_password_auth_forgot_password_post import BodyResetForgotPasswordAuthForgotPasswordPost
 from celestical.api.models.body_reset_reset_password_auth_reset_password_post import BodyResetResetPasswordAuthResetPasswordPost
 from celestical.api.models.body_verify_request_token_auth_request_verify_token_post import BodyVerifyRequestTokenAuthRequestVerifyTokenPost
 from celestical.api.models.body_verify_verify_auth_verify_post import BodyVerifyVerifyAuthVerifyPost
 from celestical.api.models.client_id import ClientId
 from celestical.api.models.client_secret import ClientSecret
-from celestical.api.models.code import Code
 from celestical.api.models.compose import Compose
 from celestical.api.models.deploy import Deploy
 from celestical.api.models.detail import Detail
 from celestical.api.models.error_model import ErrorModel
 from celestical.api.models.grant_type import GrantType
 from celestical.api.models.http_validation_error import HTTPValidationError
 from celestical.api.models.is_active import IsActive
```

## celestical/api/api/app_api.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

## celestical/api/api/auth_api.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

## celestical/api/api/default_api.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

## celestical/api/api/users_api.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

## celestical/api/api_client.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import atexit
@@ -82,15 +82,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'celestical/py/0.11.4'
+        self.user_agent = 'celestical/py/0.6.6'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

## celestical/api/configuration.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import copy
@@ -371,15 +371,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.13.1\n"\
+               "Version of the API: 0.8.1\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

## celestical/api/exceptions.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from typing import Any, Optional
```

## celestical/api/models/__init__.py

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
@@ -18,15 +18,14 @@
 from celestical.api.models.bearer_response import BearerResponse
 from celestical.api.models.body_reset_forgot_password_auth_forgot_password_post import BodyResetForgotPasswordAuthForgotPasswordPost
 from celestical.api.models.body_reset_reset_password_auth_reset_password_post import BodyResetResetPasswordAuthResetPasswordPost
 from celestical.api.models.body_verify_request_token_auth_request_verify_token_post import BodyVerifyRequestTokenAuthRequestVerifyTokenPost
 from celestical.api.models.body_verify_verify_auth_verify_post import BodyVerifyVerifyAuthVerifyPost
 from celestical.api.models.client_id import ClientId
 from celestical.api.models.client_secret import ClientSecret
-from celestical.api.models.code import Code
 from celestical.api.models.compose import Compose
 from celestical.api.models.deploy import Deploy
 from celestical.api.models.detail import Detail
 from celestical.api.models.error_model import ErrorModel
 from celestical.api.models.grant_type import GrantType
 from celestical.api.models.http_validation_error import HTTPValidationError
 from celestical.api.models.is_active import IsActive
```

## celestical/api/models/app.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/bearer_response.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/body_reset_forgot_password_auth_forgot_password_post.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/body_reset_reset_password_auth_reset_password_post.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/body_verify_request_token_auth_request_verify_token_post.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/body_verify_verify_auth_verify_post.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/client_id.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/client_secret.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/compose.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/deploy.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/detail.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/error_model.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/grant_type.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/http_validation_error.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/is_active.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/is_superuser.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/is_verified.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/missing_images.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/name.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/uploaded_image.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/user_create.py

```diff
@@ -1,30 +1,29 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
 from pydantic import BaseModel
-from celestical.api.models.code import Code
 from celestical.api.models.is_active import IsActive
 from celestical.api.models.is_superuser import IsSuperuser
 from celestical.api.models.is_verified import IsVerified
 from celestical.api.models.name import Name
 try:
     from typing import Self
 except ImportError:
@@ -36,16 +35,15 @@
     """ # noqa: E501
     email: Optional[Any]
     password: Optional[Any]
     is_active: Optional[IsActive] = None
     is_superuser: Optional[IsSuperuser] = None
     is_verified: Optional[IsVerified] = None
     name: Optional[Name] = None
-    code: Optional[Code] = None
-    __properties: ClassVar[List[str]] = ["email", "password", "is_active", "is_superuser", "is_verified", "name", "code"]
+    __properties: ClassVar[List[str]] = ["email", "password", "is_active", "is_superuser", "is_verified", "name"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -88,17 +86,14 @@
             _dict['is_superuser'] = self.is_superuser.to_dict()
         # override the default output from pydantic by calling `to_dict()` of is_verified
         if self.is_verified:
             _dict['is_verified'] = self.is_verified.to_dict()
         # override the default output from pydantic by calling `to_dict()` of name
         if self.name:
             _dict['name'] = self.name.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of code
-        if self.code:
-            _dict['code'] = self.code.to_dict()
         # set to None if email (nullable) is None
         # and model_fields_set contains the field
         if self.email is None and "email" in self.model_fields_set:
             _dict['email'] = None
 
         # set to None if password (nullable) is None
         # and model_fields_set contains the field
@@ -118,13 +113,12 @@
 
         _obj = cls.model_validate({
             "email": obj.get("email"),
             "password": obj.get("password"),
             "is_active": IsActive.from_dict(obj.get("is_active")) if obj.get("is_active") is not None else None,
             "is_superuser": IsSuperuser.from_dict(obj.get("is_superuser")) if obj.get("is_superuser") is not None else None,
             "is_verified": IsVerified.from_dict(obj.get("is_verified")) if obj.get("is_verified") is not None else None,
-            "name": Name.from_dict(obj.get("name")) if obj.get("name") is not None else None,
-            "code": Code.from_dict(obj.get("code")) if obj.get("code") is not None else None
+            "name": Name.from_dict(obj.get("name")) if obj.get("name") is not None else None
         })
         return _obj
```

## celestical/api/models/user_read.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/validation_error.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/rest.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

## celestical/cli.py

```diff
@@ -6,47 +6,46 @@
 
 import typer
 
 from celestical.compose import (
     upload_compose,
     upload_images)
 from celestical.docker_local import list_local_images
-from celestical.helper import cli_panel, print_text, print_feedback
-from celestical.configuration import cli_logger, welcome
+from celestical.helper import cli_panel, welcome_message
+from celestical.configuration import cli_logger
 from celestical.user import user_login, user_register
 from celestical.apps import list_creator_apps
 
 
 cli_logger.info("Starting CLI.")
 
 app = typer.Typer(pretty_exceptions_short=False,
                   no_args_is_help=True,
-                  help=welcome(),
+                  help=welcome_message,
                   rich_markup_mode="rich")
+cli_logger.debug("Typer created successfully.")
 
 # @app.callback(invoke_without_command=True)
 @app.command()
 def apps():
     """List all apps from current user."""
     list_creator_apps()
 
 
 @app.command()
 def login() -> None:
     """Login to Parametry's Celestical Cloud Services via the CLI."""
+    cli_logger.debug("Entering the login function")
     user_login()
 
 
 @app.command()
 def register():
     """Register as a user for Celestical Cloud Services via the CLI."""
-    if not user_register():
-        print_text("User already exists or we could not connect.")
-    else:
-        print_feedback("Your account has been created.")
+    user_register()
 
 
 @app.command()
 def images():
     """ List all local docker images for you.
         Similar to 'docker image ls'.
     """
@@ -71,15 +70,13 @@
     # --- Upload images according to response
     # 1- read response, and feedback user on status
     # 2- if 200, select the list of images in response.
     # 3- compress concerned images
     # 4- upload concerned images
     # .. keep feedback to user whenever progress is made
     if enriched_compose is None:
-        msg = "To continue with deployment you need a celestical account.\n"
-        msg += "see command: [yellow]celestical register[/yellow]"
-        cli_panel(msg)
+        cli_panel("Stopping here - could not enriched compose file")
         return
 
     upload_images(app_uuid=enriched_compose["celestical"]["app_id"], e_compose=enriched_compose)
```

## celestical/compose.py

```diff
@@ -35,53 +35,64 @@
 from celestical.configuration import (
     HOTLINE,
     apiconf,
     cli_logger,
     load_config)
 
 
+def get_image_hash(image_name_tag:str) -> str:
+    """Get the hash for a certain docker image name and tag."""
+
+    client = docker.from_env()
+    image = client.images.get(image_name_tag)
+    return image.id
+
+
+def get_ports(image_id, docker_client):
+    """Get ports from containers created from the specified image."""
+    ports = set()
+    for container in docker_client.containers.list(all=True):
+        if container.image.id == image_id:
+            port_data = container.attrs['HostConfig']['PortBindings']
+            if port_data:
+                for port, bindings in port_data.items():
+                    # get only the port number, not the protocol
+                    ports.add(port.split('/')[0])
+    return ', '.join(sorted(ports))
+
+
 def richformat_services(services:dict) -> str:
     """Create a rich formatted string to display a bullet list for services
     """
     s_info = ""
     for serv in services:
         if "image" not in services[serv]:
             services[serv]["image"] = "-undefined-"
         s_info += f"\t- [yellow]{serv}[/yellow] (image)--> "
         s_info += f"{services[serv]['image']}\n"
     return s_info
 
 
-def read_docker_compose(fullpath:Path) -> dict:
+def read_docker_compose(fullpath: Path) -> dict:
     """Read the docker-compose.yml file.
 
     Params:
         fullpath(Path): absolut path to the docker-compose.yml file
     Returns:
         (dict): docker-compose.yml file content
     """
 
     compose = None
-    msg = ""
-    if not isinstance(fullpath, Path):
-        fullpath = Path(str(fullpath))
-
-    if fullpath.is_dir():
-        msg = f"Path is not a file: {fullpath}"
-    else:
-        try:
-            with open(fullpath, 'r') as f:
-                compose = yaml.safe_load(f)
-                return compose
-        except FileNotFoundError:
-            msg = f"No file found at given path: {fullpath}"
-
-    # Ending here is not a nominal case
-    print_text(msg)
-    cli_logger.error(msg)
+    try:
+        with open(fullpath, 'r') as f:
+            compose = yaml.safe_load(f)
+    except FileNotFoundError:
+        msg = f"No file found at given path: {fullpath}"
+        print_text(msg)
+        cli_logger.error(msg)
     return compose
 
 
 def enrich_compose(
     compose: dict,
     prev_comp:dict = {},
     ecomp_path:Path = None) -> Path:
@@ -323,53 +334,48 @@
     """Upload the enriched compose file to the Celestical Cloud."""
 
     cli_panel("Let's start uploading your App's images to Celestical")
 
     if compose_path is not None:
         e_compose = read_docker_compose(fullpath=compose_path)
     elif e_compose is None:
-        return False
-
-    # Build the compressed tar file for services images
-    image_names = [
-        e_compose["services"][service_name]["image"]
-        for service_name in e_compose["services"]
-    ]
+        return False 
 
-    image_paths = compress_image(images=image_names, project_name=e_compose["celestical"]["name"])
+    # Build the compressed tar file for each service
+    image_paths = []
+    for service_name in e_compose["services"]:
+        # typer.echo(service_name)
+        #typer.confirm("Do you wish to proceed setting the image_name?")
+        #image_name = e_compose["services"][service_name]["image"].split(':')[0]
+        image_name = e_compose["services"][service_name]["image"]
+        #typer.echo(image_name)
+        #typer.confirm("Do you wish to proceed compressing?")
+        ipath = compress_image(image_name=image_name, project_name=e_compose["celestical"]["name"])
+        image_paths.append(ipath)
 
     api_ires = None
     with api.ApiClient(apiconf) as api_client:
         app_api = api.AppApi(api_client)
+
         for ipath in image_paths:
             try:
                 with ipath.open(mode="rb") as ipath_desc:
-                    # This form won't work:
-                    # upfile = {"upload_file": (ipath.name, ipath_desc.read())}
-                    upfile = (ipath.name, ipath_desc.read())
+                    # upfile = {"file": ipath.name, ipath_desc, "multipart/form-data")}
+                    upfile = {"file": ipath_desc}
                     cli_logger.debug("Making compose info push request")
-                    api_ires = app_api.upload_image_compressed_file_app_app_uuid_upload_image_post_with_http_info(
+                    api_ires = app_api.upload_image_compressed_file_app_app_uuid_upload_image_post( \
                         app_uuid=app_uuid,
                         image_file=upfile)
 
-                    # Print feedback to user
-                    msg = " uploaded" \
-                          if (api_ires.status_code == 200) \
-                          else " not uploaded"
-                    msg = str(ipath.name)+msg
-                    print_feedback(msg)
-
             except Exception as oops:
-                cli_logger.debug(f"Exception in uploading image {ipath}")
-                cli_logger.debug(type(oops))
-                print_text("Could not upload file")
+                cli_logger.debug(oops)
                 pass
 
 
-def upload_compose(compose_path:str, call_nbr:int = 1) -> dict|None:
+def upload_compose(compose_path:str, call_nbr:int = 1) -> dict:
     """ This function find the compose file and ask the user for enrichment
         unless an enriched file is already present in case user is asked
         if they want to reset the enrichment.
 
         - compose_path:str: string of the folder to deploy, it should contain
           a docker compose file. It is where the enriched file will be saved
         - call_nbr:str: in case we are missing authentication we are trying to
@@ -396,15 +402,15 @@
     compose_pack = {}
     compose_pack["enriched_compose"] = enriched_compose
     # optional in case we want to upload compose for later deployment
     compose_pack["deploy"] = True
 
     setcred, mesg = load_user_creds(apiconf)
     if setcred is False:
-        cli_panel(mesg)
+        cli_panel(msg)
         return None
 
     api_response = None
     with api.ApiClient(apiconf) as api_client:
         app_api = api.AppApi(api_client)
 
         try:
@@ -419,31 +425,27 @@
         except UnauthorizedException as oops:
             # Let's try to relog again and relaunch that function
             if call_nbr > 1:
                 msg = "Please check your connection and credentials\n"
                 msg += "[red]no access authorized for now[/red]\n\n"
                 msg += "You might need to register with: "
                 msg += "[yellow]celestical register[/yellow]\n\n"
-                msg += f"If problem persists please contact us: {HOTLINE}"
+                msg += "If problem persists please contact us: {HOTLINE}"
                 cli_panel(msg)
                 return None
             # else
             cli_panel("You have to log in again, your token may have expired." \
                       +" (signing out automatically)")
-            if not user_login(force_relog=True):
-                if not user_login(force_relog=True):
-                    print_text("Please start over again checking your credentials carefully.",
-                        worry_level="ohno")
-                    return None
+            user_login(force_relog=True)
             call_nbr += 1
             cli_logger.debug(oops)
             return upload_compose(compose_path, call_nbr)
         except Exception as oops:
-            print_text("No connection yet possible to deploy your app.")
-            cli_logger.error("Error during posting of the enriched compose file")
+            cli_panel("Something undefined happened: Check your connection.")
+            cli_logger.error("Error during post of enriched compose file")
             cli_logger.error(oops)
             return None
 
     if (not isinstance(api_response, App)):
         cli_logger.error("API response is not an App.")
         msg = "Try to login again, your token might have expired.\n"
         msg += "--> [underline]celestical login[/underline]"
```

## celestical/configuration.py

```diff
@@ -1,88 +1,35 @@
 # Managing the configuration for the Celestical services
 import json
 import os
 import logging
-import importlib.metadata
 from logging import Logger
 from pathlib import Path
 
 import typer
 from prettytable import PrettyTable, ALL
 
 import celestical.api as api
 from celestical.helper import print_text
 
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 apiconf = api.Configuration(
-        host = "https://moon.celestical.net"
+        host = "http://localhost:8000"
 )
 
-current_celestical_version = importlib.metadata.version('celestical')
-
 # LOGGING_LEVEL = logging.DEBUG
 # logging.basicConfig(encoding='utf-8', level=LOGGING_LEVEL)
 
 HOTLINE = "starship@celestical.net"
-PRODUCTION = True
-
-
-def get_login_status() -> str:
-    login_status = ""
-    # [{wcol}]colored text[/{wcol}]
-    wcol = "purple"
-
-    udata = load_config()
-    if not (udata is None or udata == {}):
-        # else message that config cannot be loaded will be shown.
-        tok = udata["access_token"]
-        uname = udata["username"]
-        if uname != "":
-            login_status += f"\n\t* Current user: [{wcol}]{uname}[/{wcol}]"
-        else:
-            login_status += f"\n\t* No current user [{wcol}]logged in[/{wcol}]"
-        if tok != "":
-            # TODO checked the created date field to announce
-            # if relogging is necessary.
-            login_status += f"\n\t* [{wcol}]Already logged in[/{wcol}] once"
-
-    return login_status
-
-
-def welcome(verbose:int=2) -> str:
-    """ Return a global welcome message
-
-        verbose from 0 (short) to 2 (long)
-    """
-    wcol = "purple"
-    welcome_message:str = f"[{wcol}]Direct deployment of containers or compose" \
-                          +" files to an independent green cloud made by space" \
-                          +f" engineers[/{wcol}] " \
-                          +f"(version: {current_celestical_version})\n"
-
-    if verbose > 0:
-        welcome_message += get_login_status()
+PRODUCTION = False
 
 
-    if verbose > 1:
-        welcome_message += "\n [underline]Usual workflow steps[/underline]" \
-                        +"\n\t [1] (only once) Register with command " \
-                        +f"[{wcol}]celestical register[/{wcol}]" \
-                        +"\n\t [2] Login with command " \
-                        +f"[{wcol}]celestical login[/{wcol}]" \
-                        +"\n\t [3] Deploy with command " \
-                        +f"[{wcol}]celestical deploy[/{wcol}]"
-
-    return welcome_message
-
-
-# Service types definitions
 def get_default_config_dir() -> Path:
-    path = Path.home() / ".config" / "celestical"
+    path = Path.home() / ".config" / "celestical" 
     return path
 
 
 def get_default_config_path() -> Path:
     """Return the default config path for this application
 
     Returns:
@@ -117,48 +64,41 @@
     user_data = {}
     if path.exists():
         try:
             with open(path, 'r') as f_desc:
                 user_data = json.load(f_desc)
         except:
             print_text("Could not read the configuration file.")
-    # Useless too much info for user experience
-    #else:
-    #    print_text("The configuration file does not exist yet.")
+    else:
+        print_text("The configuration file does not exist yet.")
 
     return user_data
 
 
-def save_config(config:dict) -> bool:
+def save_config(config:dict):
     """Save config file to the default_config_path.
 
     Params:
         config(dict): configuration.
     Returns:
-        (bool): True if saving process went fine
+        (str): configuration absolut path
     """
     cpath = get_default_config_path()
 
     try:
         if not cpath.parent.exists():
             os.makedirs(cpath.parent, exist_ok=True)
-    except Exception as oops:
-        cli_logger.debug("save_config: directory couldn't be created.")
-        cli_logger.debug(oops)
-        return False
+    except Exception as e:
+        typer.echo("Config directory couldn't be created successfully")
 
-    try: 
-        with open(cpath, 'w') as f:
-            json.dump(config, f, indent=4)
-    except Exception as oops:
-        cli_logger.debug("save_config: config file couldn't be written.")
-        cli_logger.debug(oops)
-        return False
+    with open(cpath, 'w') as f:
+        json.dump(config, f, indent=4)
 
-    return True
+    typer.echo(f"Login credentials safely updated in: {cpath}")
+    return cpath
 
 
 def cli_setup() -> bool:
     """ Setup necessary directories.
     """
     config_path = get_default_config_dir()
     try:
@@ -184,15 +124,15 @@
             format=log_format,
             filemode="a",
             level=logging.DEBUG,
         )
         logger = logging.getLogger(name="Celestical CLI")
         logger.warning(f"Starting Logger in DEBUG Mode: {log_location}")
         return logger
-
+    
     logging.basicConfig(
         encoding='utf-8',
         filename=log_location,
         format=log_format,
         filemode="a",
         level=logging.WARNING,
     )
```

## celestical/docker_local.py

```diff
@@ -7,91 +7,46 @@
 
 import docker
 import gzip
 from tqdm import tqdm
 from prettytable import PrettyTable, ALL
 import typer
 from celestical.configuration import cli_logger
-from celestical.helper import print_text, confirm_user
+from celestical.helper import print_text
 
 # logging.basicConfig(encoding='utf-8', level=LOGGING_LEVEL)
 
-
 def get_docker_client():
-    """ Returns a docker client taken from local environment """
     client = None
     err_msg = ""
     try:
         client = docker.from_env()
     except:
         err_msg = "Could not connect to the docker service. Is it really running?"
     return client, err_msg
 
 
-def get_image_hash(image_name_tag:str) -> str|None:
-    """ Get the hash for a certain docker image name and tag.
-
-        Params:
-            image_name_tag(str): docker tag of the image to extract hash from
-        Returns:
+def get_ports(docker_client, image_id):
     """
-    client = docker.from_env()
-    image = client.images.get(image_name_tag)
-    if image is None:
-        return None
-    return image.id
-
-
-def get_ports(image_id:str,
-              docker_client:any=None,
-              proto:str="tcp") -> str:
-    """ Get ports from containers created from the specified image.
-        else get the ExposedPorts info from the image itself.
-
-        Params:
-            image_id(str): should the string hash of the image
-            docker_clienti(any): a docker client
-            proto(str): ports for a that specific protocol, by default 'tcp'
+        Get ports from containers created from the specified image.
 
-        Returns:
-            a string for a joint list of ports
+        returns a string for a joint list of ports
     """
     if docker_client is None:
-        docker_client, err_msg = get_docker_client()
-        if docker_client is None:
-            cli_logger.debug(err_msg)
-            return ""
-        # else continue
+        return ""
 
     ports = set()
-
-    # Checking from containers
     for container in docker_client.containers.list(all=True):
         if container.image.id == image_id:
             port_data = container.attrs['HostConfig']['PortBindings']
             if port_data:
                 for port, bindings in port_data.items():
                     # get only the port number, not the protocol
-                    ports.add(str(port.split('/')[0]))
-    
-    # Checking from listed images 
-    if len(ports) == 0:
-        try:
-            img = docker_client.images.get(image_id)
-            for tcpport in [str(attr).split("/")[0] 
-                            for attr in
-                            img.attrs["Config"]["ExposedPorts"] 
-                            if "tcp" in attr]:
-                ports.add(tcpport)
-        except Exception as oops:
-            # The image_id is not found
-            # The ports set remains empty and that's all ok.
-            cli_logger.debug(oops)
-
-    return ",".join(sorted(ports))
+                    ports.add(port.split('/')[0])
+    return ', '.join(sorted(ports)) 
 
 
 def list_local_images() -> Tuple[PrettyTable, str]:
     """List all docker images locally available with port information.
 
     Returns:
         PrettyTable of formatted table of docker images
@@ -136,119 +91,83 @@
     for image in images:
         # Split the Image ID into two lines
         half_length = len(image.id) # // 2
         formatted_id = f'{image.id[:half_length]}\n{image.id[half_length:]}'
         # Extract image name from the tags
         image_name = image.tags[0].split(':')[0] if image.tags else 'N/A'
         # Get ports
-        ports = get_ports(image.id, docker_client)
+        ports = get_ports(docker_client, image.id)
         table.add_row([formatted_id, image_name, ', '.join(image.tags), ports])
 
     return table, err_msg
 
 
-def compress_image(images: str|list[str], project_name: str) -> list[Path]:
+def compress_image(image_name: str, project_name: str) -> Path:
     """Compress a Docker image.
-
-    Params:
-        images: string or list of strings of image full tag names
-                as they should appear in the "image" field of each service
-        project_name: a string given to name the project, usually the base
-                domain name
-    Returns:
-        A list of path to gzipped images to be uploaded
     """
 
-    image_names = []
-    gz_paths = []
-
-    # --- Getting docker client
-    client, emsg = get_docker_client()
-    if client is None:
-        return gz_paths
+    client = docker.from_env()
 
-    # --- preparing save directory
     save_path = Path(f"/tmp/celestical/{project_name}/")
     # Create the save_path directory and any necessary parent directories
     save_path.mkdir(parents=True, exist_ok=True)
 
-    # --- preparing list of images, or of 1 image
-    if isinstance(images, str):
-        image_names = [images]
-    else:
-        image_names = images
-
-    # --- Compressing all images in different gzips
-    for image_name in image_names:
-        tar_filename = save_path / f'{image_name}.tar'
-        gz_filename = save_path / f'{image_name}.tar.gz'
-
-        # Step 1: Calculate the total size of the image
-        # for chunk in client.images.get(image).save(named=True):
-        #     tar_file.write(chunk)
-        print_text(f"Working on {image_name}...")
-        img = None
-        try:
-            img = client.images.get(image_name)
-        except Exception as oops:
-            cli_logger.debug(oops)
-            img = None
-
-        if img is None:
-            msg = f"Image {image_name} not found for project: {project_name}"
-            print_text(msg,
-                       worry_level="ohno")
-            cli_logger.debug(msg)
-            continue
-
-        image_data = img.save(named=True)
-        total_size = sum(len(chunk) for chunk in image_data)
-        total_size_mb = total_size / (1024 * 1024)
-
-        # Reset the image data iterator
-        image_data = img.save(named=True)
-
-        print_text(f"Image Tag Found: {image_name}"
-                   +f"\n\timage size: {total_size_mb:.2f} MB"
-                   +f"\n\tsaving in: {save_path}"
-                   +f"\n\tas file name: {gz_filename}")
-
-        # Prompt user for confirmation before proceeding with compression
-        if gz_filename.is_file():
-            if not confirm_user(f"[yellow]{image_name}[/yellow] already prepared,"
-                               +f"\n\trenew and overwrite {gz_filename} ?"):
-                print_text(f" === Ok, using ready file: {gz_filename}")
-                gz_paths.append(gz_filename)
-                continue
-
-        # Save the Docker image to a tar file with a progress bar
-        print_text(f"Export image to archive tar file {tar_filename} ...")
-        with open(tar_filename, 'wb') as tar_file:
-            with tqdm(total=total_size,
-                      unit='B',
-                      unit_scale=True,
-                      desc="archiving") as pbar:
-                for chunk in image_data:
-                    tar_file.write(chunk)
-                    pbar.update(len(chunk))
+    tar_filename = save_path / f'{image_name}.tar'
+    gz_filename = save_path / f'{image_name}.tar.gz'
 
 
-        # Step 2: Compress the tar file using gzip
-        print_text(f"Compressing exported tar image (gzip) to {gz_filename} ...")
-        file_size = os.path.getsize(tar_filename)
-        with open(tar_filename, 'rb') as tar_file:
-            with gzip.open(gz_filename, 'wb') as gz_file:
-                with tqdm(total=file_size,
-                          unit='B',
-                          unit_scale=True,
-                          desc="gzipping") as pbar:
-                    # Define a chunk size (e.g., 1 MiB)
-                    chunk_size = 1024 * 1024
-                    # Read, compress, and write data in chunks
-                    while chunk := tar_file.read(chunk_size):
-                        gz_file.write(chunk)
-                        pbar.update(len(chunk))
+    # Step 1: Save the Docker image to a tar file
+    # image = f'{image_name}:{tag}'
+    # tar_filename = f'{image_name}_{tag}.tar'
+    # with open(tar_filename, 'wb') as tar_file:
+    #     for chunk in client.images.get(image).save(named=True):
+    #         tar_file.write(chunk)
+
+    print_text("Calculating total image size ..")
+
+    # Step 1: Calculate the total size of the image
+    image_data = client.images.get(image_name).save(named=True)
+    total_size = sum(len(chunk) for chunk in image_data)
+    total_size_mb = total_size / (1024 * 1024)
+
+
+    # Reset the image data iterator
+    image_data = client.images.get(image_name).save(named=True)
+
+    print_text("\n============================================\n")
+    print_text(f"Image Name:Tag: {image_name} \t Image Size: {total_size_mb:.2f} MB")
+    print_text(f"Saving in: {save_path} \t File Name: {gz_filename}")
+    # print_text(f"App context: {context} \t Domain: {domain}")
+    print_text("\n============================================\n")
+
+    # Prompt user for confirmation before proceeding with compression
+    if not typer.confirm("Would you like to proceed with saving and compressing the image?"):
+        print_text("Aborting the program.")
+        raise typer.Abort()
+
+    print_text("Starting to save the image .. ")
+    # Save the Docker image to a tar file with a progress bar
+    with open(tar_filename, 'wb') as tar_file:
+        with tqdm(total=total_size, unit='B', unit_scale=True, desc='Saving') as pbar:
+            for chunk in image_data:
+                tar_file.write(chunk)
+                pbar.update(len(chunk))
+
+    print_text("Compressing exported tar image (gzip)...")
+
+    # Step 2: Compress the tar file using gzip
+    file_size = os.path.getsize(tar_filename)
+    with open(tar_filename, 'rb') as tar_file:
+        with gzip.open(gz_filename, 'wb') as gz_file:
+            with tqdm(total=file_size, unit='B', unit_scale=True, desc='Compressing') as pbar:
+                # Define a chunk size (e.g., 1 MiB)
+                chunk_size = 1024 * 1024
+                # Read, compress, and write data in chunks
+                while chunk := tar_file.read(chunk_size):
+                    gz_file.write(chunk)
+                    pbar.update(len(chunk))
 
-        gz_paths.append(gz_filename)
-        print_text(f"[green]succesfully prepared[/green]: {gz_filename}")
+    print_text("\n============================================\n")
+    print_text(f"Image {image_name} compressed successfully in {save_path}!")
+    print_text("\n============================================\n")
 
-    return gz_paths
+    return gz_filename
```

## celestical/helper.py

```diff
@@ -10,15 +10,19 @@
 from rich.console import Console
 from rich.panel import Panel
 from rich.table import Table
 from rich.prompt import Prompt, Confirm
 
 console = Console()
 
+welcome_message:str = "[purple]Direct deployment of containers or compose" \
+                      +"files to a green cloud made by space engineers[/purple]"
 
+# Service types definitions
+#
 # For each service type there is a list of keywords to detect them
 SERVICE_TYPES = {
     "FRONTEND": ["web", "www", "frontend", "traefik", "haproxy", "apache", "nginx"],
     "API": ["api", "backend", "service", "node"],
     "DB": ["database", "redis", "mongo", "mariadb", "postgre"],
     "BATCH": ["hidden", "compute"],
     "OTHER": []
@@ -98,27 +102,27 @@
     if "name" not in data:
         return False
 
     json_file = f'stack_{data["name"]}.json'
     try:
         with open(json_file, 'w') as jfile:
             json.dump(data, jfile, indent=4)
-    except Exception as oops:
-        print_text(f"Error: JSON file could not be saved f'stack_{data['name']}.json'")
-        cli_logger.debug(oops)
-        return False
+        print_text("Json saved successfully.")
+        return True
+    except Exception as e:
+        print(f"Error: Unable to save data to f'stack_{data['name']}.json'")
+        print(f'Error details: {e}')
 
-    return True
+    return False
 
 
-def save_yaml(data: dict, yml_file:Path = None) -> Path|None:
+def save_yaml(data: dict, yml_file:Path = None):
     """Helper function to save the complete stack info.
     Params:
-        data(dict): complete info about the stack (name, compose ..)
-        yml_file(Path):  Path where to save the file
+        stack_info(dict): complete info about the stack (name, compose ..)
     Returns:
 
     """
     #yml_file = "docker-compose.yml"
     if yml_file is None:
         yml_file = Path("./docker-compose-enriched.yml")
 
@@ -126,15 +130,14 @@
         with yml_file.open(mode='w') as yfile:
             yaml.dump(data, yfile, default_flow_style=False)
         print_text(f"YAML file created successfully: [green]{yml_file}[/green]")
 
     except Exception as e:
         print(f'Error: Unable to save data to {yml_file}')
         print(f'Error details: {e}')
-        return None
 
     # return the Path object of the saved file
     return Path(yml_file)
 
 
 def print_nested_dict(dictionary: dict):
     """Print a nested dictionary in a readable format."""
@@ -191,31 +194,22 @@
     """
     confirmation:bool = Confirm.ask(f"\n === {prompt} ", default=default)
     if confirmation is None:
         confirmation = False
     return confirmation
 
 
-def print_text(text: str, worry_level="chill"):
+def print_text(text: str):
     """Print text to the CLI.
         Params:
             text(str): the text to print
-            worry_level(str): a level of worries that would change the color; chill, oops, ohno
         Returns:
             str: the text to print
     """
-    msg = f"{text}"
-    if worry_level == "oops":
-        msg = f"[orange]{text}[/orange]"
-    elif worry_level == "ohno":
-        msg = f"[red]{text}[/red]"
-
-    # add prefix
-    msg = " --- " + msg
-
+    msg = f"\n --- {text}"
     return console.print(msg)
 
 
 def guess_service_type_by_name(service_name: str, img_name:str=""):
     """ Quick guess of service type
     """
```

## celestical/user.py

```diff
@@ -7,44 +7,31 @@
 from datetime import datetime
 from typing import Tuple
 
 from celestical.api import (
     ApiClient,
     AuthApi,
     ApiException,
-    Code,
     UserCreate)
 from celestical.configuration import (
     apiconf,
     load_config,
     save_config,
     cli_logger)
 from celestical.helper import (
     cli_panel,
-    print_text,
     prompt_user,
     confirm_user)
 
 
-def register_form(ask:str = "Register with or without a [b]special code[/b]",
-    default_code:str = ""
-    ) -> str:
-    if ask != "":
-        print_text(ask)
-    user_code = prompt_user("[b]special code[/b] (optional)", default=default_code)
-    return user_code
-
-
-def login_form(ask:str = "Please enter your [i]celestical[/i] credentials",
+def login_form(ask:str = "Please enter your wonderful Celestical credentials",
     default_email:str = None
     ) -> Tuple[str, str]:
-    """ The username/password form to login and register """
-    if ask != "":
-        print_text(ask)
-    user_mail = prompt_user("Work email", default=default_email)
+    cli_panel(ask)
+    user_mail = prompt_user("User Mail", default=default_email)
     if "@" not in user_mail:
         cli_logger.error("Entered email address is missing a '@'")
         cli_panel(message="Email is incorrect: no @ sign found.", _type="error")
         return login_form(ask)
 
     password = getpass.getpass(" *** Password: ")
     cli_logger.info("Password succesfully created.")
@@ -71,49 +58,49 @@
 
     use_user = False
     if "access_token" in user_data:
         if len(user_data["access_token"]) > 10:
             if "username" not in user_data:
                 cli_logger.warning("Oh no it seems config was manually edited.")
             elif force_relog == False:
-                use_user = confirm_user("Do you want to continue with logged " \
-                    + f"in user: [yellow]{user_data['username']}[/yellow]")
+                cli_panel(f"You are logged in as {user_data['username']}")
+                use_user = confirm_user("Do you want to continue" \
+                    + f" with user [yellow]{user_data['username']}[/yellow]")
                 if use_user:
-                    cli_panel("\t --> continuing with logged in user: " \
+                    cli_panel("\t --> continuing as " \
                         +f"[yellow]{user_data['username']}[/yellow]")
                     return True
 
         if force_relog:
             # Similar to a logout: forgetting token
             data = {
                 "created": datetime.utcnow().strftime('%Y-%m-%d_%H:%M:%S'),
                 "username": "",
                 "access_token": "",
                 "token_type": ""
             }
-            save_ok = save_config(data)
+            save_config(data)
 
             if "username" in user_data:
                 if user_data['username'] is None or user_data['username'] == "":
                     return user_login(default_email=None)
                 # else we've got a previous email info
                 return user_login(default_email=user_data['username'])
             return user_login()
 
-    (username, password) = login_form(default_email=default_email)
-
     with ApiClient(apiconf) as api_client:
         # Create an instance of the API class
         api_instance = AuthApi(api_client)
 
-        save_ok = False
+        (username, password) = login_form(default_email=default_email)
+
         try:
             # Auth:Jwt.Login
             api_response = api_instance.auth_jwt_login_auth_jwt_login_post(username, password)
-            cli_logger.debug("We did get a login api response")
+            cli_logger.debug("we did get a api response")
             if api_response.token_type != "bearer":
                 cli_logger.debug("This client does not handle non bearer type token")
                 return False
 
             if len(api_response.access_token) < 10:
                 cli_logger.debug("Received token seems invalid")
                 return False
@@ -122,72 +109,60 @@
             cli_logger.debug("Creating and saving user data/conf.")
             data = {
                 "created": datetime.utcnow().strftime('%Y-%m-%d_%H:%M:%S'),
                 "username": username,
                 "access_token": api_response.access_token,
                 "token_type": api_response.token_type
             }
-            save_ok = save_config(data)
+            save_config(data)
         except ApiException as api_exp:
-            cli_logger.error("Code Enceladus: ApiException when logging in. Assuming wrong user,password tuple.")
+            cli_logger.error("Code Enceladus: ApiException when logging in.")
             cli_logger.debug(api_exp)
-            print_text("Sorry user/password are not matching. Not logged in",
-                       worry_level="ohno")
+            cli_panel("Sorry we could not log you in at the moment")
             return False
         except Exception as oops:
             cli_logger.error("Code Mars: could not connect, try again after checking your connection.")
             cli_logger.debug(oops)
-            print_text("Sorry we could not log you in, please try again.",
-                       worry_level="ohno")
             return False
 
-    cli_panel("\t --> You are now logged in as user: "
-              +f"[yellow]{username}[/yellow]"
-              +"\n\n\t     You use other celestical commands"
-              +"\n\t     as long as your login token is valid.")
     return True
 
 
 def user_register() -> bool:
     """Register as a user for Parametry Cloud Services via the CLI."""
 
-    user_code = register_form()
-
-    (user_mail, password) = login_form("")
-
     with ApiClient(apiconf) as api_client:
         auth = AuthApi(api_client=api_client)
 
+        (user_mail, password) = login_form("Please enter new Celestical credentials")
+
         apires = None
         try:
             apires = auth.register_register_auth_register_post(
                     user_create=UserCreate(
-                        email=user_mail,
-                        password=password,
-                        code=Code(user_code)
+                        email= user_mail,
+                        password=password
                         )
                     )
         except ApiException as api_err:
             msg = f"---- Registration error ({api_err.status})"
             cli_logger.error(msg)
             cli_logger.debug(apires)
             if api_err.body:
                 cli_logger.debug(api_err.body)
             else:
                 cli_logger.debug(api_err.reason)
             return False
-        except Exception as oops:
-            cli_logger.error(oops)
-            return False
 
+        cli_panel("You are now registered and must verify your email")
         return True
 
 
 def load_user_creds(_apiconf) -> Tuple[bool, str]:
-    """ Reads user creds from config and set access token
+    """ Reads user creds from config and set access token 
 
         _apiconf from api.Configuration()
         is set with latest access token.
     """
     user_data = load_config()
 
     if user_data is not None and isinstance(user_data, dict):
```

## Comparing `celestical/api/models/code.py` & `celestical/api/models/first_creator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.13.1
+    The version of the OpenAPI document: 0.5.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -24,30 +24,30 @@
 from typing_extensions import Literal
 from pydantic import StrictStr, Field
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-CODE_ANY_OF_SCHEMAS = ["object"]
+FIRSTCREATOR_ANY_OF_SCHEMAS = ["object"]
 
-class Code(BaseModel):
+class FirstCreator(BaseModel):
     """
-    Code
+    FirstCreator
     """
 
     # data type: object
     anyof_schema_1_validator: Optional[Any] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
         actual_instance: Optional[Union[object]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Literal[CODE_ANY_OF_SCHEMAS]
+    any_of_schemas: List[str] = Literal[FIRSTCREATOR_ANY_OF_SCHEMAS]
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -58,15 +58,15 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = Code.model_construct()
+        instance = FirstCreator.model_construct()
         error_messages = []
         # validate data type: object
         try:
             instance.anyof_schema_1_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
@@ -74,15 +74,15 @@
         try:
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in Code with anyOf schemas: object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in FirstCreator with anyOf schemas: object. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
         return cls.from_json(json.dumps(obj))
 
@@ -108,15 +108,15 @@
             instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into Code with anyOf schemas: object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into FirstCreator with anyOf schemas: object. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
```

## Comparing `celestical-0.14.3.dist-info/COPYING` & `celestical-0.9.2.dist-info/COPYING`

 * *Files identical despite different names*

## Comparing `celestical-0.14.3.dist-info/COPYING.LESSER` & `celestical-0.9.2.dist-info/COPYING.LESSER`

 * *Files identical despite different names*

## Comparing `celestical-0.14.3.dist-info/RECORD` & `celestical-0.9.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 COPYING,sha256=5X8cMguM-HmKfS_4Om-eBqM6A1hfbgZf6pfx2G24QFI,35150
 COPYING.LESSER,sha256=GkWx0KhgPf4s_GRPnauXCxdi-Sur4qrG6y9dRXLEpoA,7653
 LICENSE,sha256=l4pgftTXn9aA9oyWYwUdY8St5XfN8v5bCjhSUZhNmfo,108
 celestical/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-celestical/api/__init__.py,sha256=iHihbWkJjesTORMMpYvUSFYjDBO5pPq47Q7K07Lzdro,2695
+celestical/api/__init__.py,sha256=hiZKsKSLCshfs_KFaMciEPOkZ-jZrBcZprs_sxo6Y60,2650
 celestical/api/api/__init__.py,sha256=IdA2DY2zidKnvzu-ZsR19fS-l0tkZ3Nw0OCWxMYoq1E,246
-celestical/api/api/app_api.py,sha256=9uO-dAnuV1sgZ0mD2pkMD53lzjCxKGm4PJ92sZ8Vtdo,51216
-celestical/api/api/auth_api.py,sha256=z-M3h0nlZg6tpjRnP-jymswOskOz72Y_SrCYpFs8j0M,79145
-celestical/api/api/default_api.py,sha256=z8nX2qqR9GvpYg082ZZa-JUERk4r7YcKiT2NUePpWpw,9886
-celestical/api/api/users_api.py,sha256=jycDwRXcXbSSV39q5mEQYqU2x01REs_A_I4otpZ6Dm8,51169
-celestical/api/api_client.py,sha256=5fxNjOO3WkNi61ZIv4GCxdZniAJnhgHhGpc6giskBdM,24570
+celestical/api/api/app_api.py,sha256=ZX6XXaM-fgo0gyICD9Z49m6W8Ikh29lQ0J5OPQTR-ec,51215
+celestical/api/api/auth_api.py,sha256=pwgr8PW1jpX9IrR9dN_gM7DqTit2BCEx1gSQqBZUHIA,79144
+celestical/api/api/default_api.py,sha256=SAMCrG6WYSawFkrePeKBqAZW9pt4IcA0xYgYxwCp9K4,9885
+celestical/api/api/stacy_api.py,sha256=eiQLPA7IhHBEGW9mtWx6fbxEMjSeUxnym9vyWFenR1A,10780
+celestical/api/api/users_api.py,sha256=RjS4Jd52f6T6TQgCGBjcSHcydr3m0Qq4pVvape8HtKg,51168
+celestical/api/api_client.py,sha256=H6fIscBiFiNaPUHDGPqUOFD5cdnU3GkQKeJOFYx8Frg,24568
 celestical/api/api_response.py,sha256=A7O_XgliD6y7jEv82fgIaxR3T8KiwaOqHR6djpZyh_o,674
-celestical/api/configuration.py,sha256=hIU0AKMtRawkEAl8eZ_4dbSN484WcDkrThxGBMEwlRY,14610
-celestical/api/exceptions.py,sha256=zTaasyn46CI75LKI_FXjX358-mliMbTuMjKqANe_IPU,5940
-celestical/api/models/__init__.py,sha256=HzdT7upmRlb95jWdZIo3ksntbpArqQMgLybW10pfUco,1953
-celestical/api/models/app.py,sha256=lTEXe2_Jp668InYWRWDeJK_8nytV2JNooMyKqIHN0aU,3731
-celestical/api/models/bearer_response.py,sha256=8JpYjfQ9saXEi63sTJmqxWbYTZo6CxapzSclWhyhMNU,2939
-celestical/api/models/body_reset_forgot_password_auth_forgot_password_post.py,sha256=Ahv4YaVUbS-tRdDa-DzLsQmNEloA8ZS8iK3gu7u1Sm0,2691
-celestical/api/models/body_reset_reset_password_auth_reset_password_post.py,sha256=sHn2NwTfeCYAki4GZBRhdv7xGE6LB9CUHEtuB_KYGxE,2983
-celestical/api/models/body_verify_request_token_auth_request_verify_token_post.py,sha256=syZH4A7gohpDxEaddlv3x49r0YtQcJGCRTEuVNY7Rzk,2703
-celestical/api/models/body_verify_verify_auth_verify_post.py,sha256=4pZhkps9UBt10RO4Un1OiZ2vNwZ5IVg-4PDVLDinQw0,2631
-celestical/api/models/client_id.py,sha256=dyW9e1Zj6nHOMdP91R_JWtQi3DQg3aYwy-7DcxL8CyA,4815
-celestical/api/models/client_secret.py,sha256=N76KlNSaxWoJjuJZs_rlCufz8r6QOLrQVIm70RMLEbc,4843
-celestical/api/models/code.py,sha256=sY2lEIBfOCwzSrVIVLIzFoT9E9GWL5tRnZKQBgnDV1U,4787
-celestical/api/models/compose.py,sha256=Oc_tuyvwRplzUWrC5a5aXGo-PbCVjj_FGHM5_Qt8oHg,3041
-celestical/api/models/deploy.py,sha256=iNoR_UsZ20bGAH02RTMQAsNdHjtmjvMinGmWyLyK31Q,4801
-celestical/api/models/detail.py,sha256=WYf3w7j3GPtG4XA1Z2WJEk51nqy3SIaEv0l0l6KPs_c,4912
-celestical/api/models/error_model.py,sha256=5P1uPI_BdE6Y1HBgJOxexbubWigpzPvSl-Sy3fX_Ojw,2605
-celestical/api/models/grant_type.py,sha256=GW1__w9jV0-ySKSzqqubXlUYw1JSFe7082JJ4Wgflow,4822
-celestical/api/models/http_validation_error.py,sha256=Jm-Lk2KTyEgpSC81lXxdyVlCLUcxQiNQaor7kywJxz0,2602
-celestical/api/models/is_active.py,sha256=MSV8XWTssZohqY7XMI3y8TP_MMz9AyJRw9Mt705u94E,4815
-celestical/api/models/is_superuser.py,sha256=YuFTpd0_NXpVhcCBMeHqIdfxNF5uHKijh2H6GtWyGbA,4836
-celestical/api/models/is_verified.py,sha256=no2-5X-Iy1lHofKm1MOnO24Wk5_klI8cYtPSHcKk1po,4829
-celestical/api/models/missing_images.py,sha256=leWbOlPcuyhfwFGG6s5cqS5faW9M9Ea4iKDIiC7I9hI,2639
-celestical/api/models/name.py,sha256=u-rzqcT3gRpFQcU3CSVmgV4VWSYuJ3N0cCJHGsy8R1U,4787
-celestical/api/models/uploaded_image.py,sha256=XU1vxIoSYfE1rvF315R-0ee-42IKYFCE_ELWGkEzX24,2920
-celestical/api/models/user_create.py,sha256=LwtPtoeehnOfaFXXm7O-regycgII1bF6F3FjZ7Yixfw,4757
-celestical/api/models/user_read.py,sha256=Ly7hbSciw9I3ZKSG_15dz1jj4s2Rn5O3goprPSk_sqI,4111
-celestical/api/models/validation_error.py,sha256=UOlbRh_hyKGixgRP1iVHxrCwLWVB0M08i1kb-NEI2m0,3083
+celestical/api/configuration.py,sha256=iNAihwpPKK7ziPI0pS7w9g8rASM1biNVbJ64IrGEk_w,14608
+celestical/api/exceptions.py,sha256=fT4ddGM3PkDKY-s_ARQg-U3HWUlm2Rj8zf_X53lXY2I,5939
+celestical/api/models/__init__.py,sha256=3xXSsSE49e7oEXwCeYQbglhvaj3WbVJwQtbR7Rio3wE,1908
+celestical/api/models/app.py,sha256=GCyA7wTkd91nSZaZLkBjECuGBLr47UzcwRylV_M25_o,3730
+celestical/api/models/bearer_response.py,sha256=NJ9sh54KeNdxyaGNudlX5ykYU3JjM8P3650mAuyJjRI,2938
+celestical/api/models/body_reset_forgot_password_auth_forgot_password_post.py,sha256=79ut-GVpE4RiQFFSDBgDR4H75RrT3rX-c8jt79jwgps,2690
+celestical/api/models/body_reset_reset_password_auth_reset_password_post.py,sha256=XbMhpcOHtiq-IUzwD7rsya0kyDIIBgHAr3Oe48fZJls,2982
+celestical/api/models/body_verify_request_token_auth_request_verify_token_post.py,sha256=RDqmi4Qne2KosantcQe-GQV3HbFxv7QIQJNC2xv49xQ,2702
+celestical/api/models/body_verify_verify_auth_verify_post.py,sha256=HXlcfWtKa1qLnWqiQ56hIsMKTIA9IAdjY2HrWb-Bg1E,2630
+celestical/api/models/client_id.py,sha256=RV7NcjIoJGSo_MMmVJlCYlFS4XMgyGFjLGXr_a7IAWU,4814
+celestical/api/models/client_secret.py,sha256=nOfYUMPD7nf8HlnIumVD1dD2-l0dzwuL7Bt-3DAxHcY,4842
+celestical/api/models/compose.py,sha256=cGK0C6_q8gWjhpgTyXoEri4GjxNAFsREbhnNNS1hg6k,3040
+celestical/api/models/deploy.py,sha256=0rUsci8wT75aOuBZM4ZMlqDBGb3mVFYb_7eCEuq0z50,4800
+celestical/api/models/detail.py,sha256=MX74EXNEXY_MuiCqK0wAxNKLN2Av8sTjUNtQ4NzGv4c,4911
+celestical/api/models/error_model.py,sha256=p5qNIA8MWobgK_JcEtImXZSOZ-K1qXk4UYJmk_4RjEk,2604
+celestical/api/models/first_creator.py,sha256=xRGK5to0X5GEEJPEkth6ORR1dxiwAC0bvmnfOM0m3zc,4842
+celestical/api/models/grant_type.py,sha256=-TKOZraKiAEZUMcRVrBkuukJ2V08Nl2ieT45OU37r10,4821
+celestical/api/models/http_validation_error.py,sha256=_Qo9y6bbKoLxIcJKI0m2iFbtlg-2B1GXOq--zm6-46Q,2601
+celestical/api/models/is_active.py,sha256=HYbzs3PQ3UeIPNWHmHnKdbp_uRruOIrY_Gae86tsm1Y,4814
+celestical/api/models/is_superuser.py,sha256=nxy44eJY3vLmtY8LuBdL2KrXWoYF9LvzMbVLlvy-9oY,4835
+celestical/api/models/is_verified.py,sha256=7A6Qfgztk5WuQDirb_sUsXGO9OsTWX-VM_hzFkhFMuQ,4828
+celestical/api/models/missing_apps.py,sha256=55P7VuHS4RXJ9o3G9d1xr_GKJ0ShEbdzNwzfXx504qI,2622
+celestical/api/models/missing_images.py,sha256=xh0ao8lMgJPT7bjGReOIJQah8GH2ZodZM8Rgr6UanrQ,2638
+celestical/api/models/name.py,sha256=RZe8rI7BkHRHhlWqKTxTKutdd58sMEWoJA30f78TvfQ,4786
+celestical/api/models/stack.py,sha256=Me8Qmj00_w1Ct7OcVNqYxdxrc2doHLEIOTRLPupeRIs,4225
+celestical/api/models/uploaded_image.py,sha256=-hVIIANC_nN7cjT5HgVgFytU8NmLEDQ6NHd_05VqUHY,2919
+celestical/api/models/user_create.py,sha256=szqBUrafzkpwNVv0bHvjIcVflKVuvu__6mbuK7j532Q,4425
+celestical/api/models/user_read.py,sha256=P6eCgdHAG3UHaTtT8yNrF7zpCLAeRqo2VPW19OwxHm8,4110
+celestical/api/models/validation_error.py,sha256=J7OyFxZwfrSv1AXgJJLrfFk3thtgs4K0kz78eivYBtE,3082
 celestical/api/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-celestical/api/rest.py,sha256=F01oKUWQgB9J2BbJAHRyJBum3usn1MjIEy6T128e1Zg,9782
+celestical/api/rest.py,sha256=BVDpxA9MvCU3oRg5PD1xbyFzq2i2NtefRqEf-9J4thM,9781
 celestical/apps.py,sha256=efrH9WcFLwtuLo9TFB7U5jAmHGCiQtfJHMEvVZjbofg,1533
-celestical/cli.py,sha256=F4UUrKxypFHSMF1vVAghEs5w1LV0icnBtyUdNEUKncY,2579
-celestical/compose.py,sha256=68sBKmZ124Pq6oAHJgaLlwu6WuCyEBA2lIElNbfghg8,17242
-celestical/configuration.py,sha256=jeAmff7UZdc7LxDaYMz1vXwYaQ4CeXozix-4xBJqfQI,6010
-celestical/docker_local.py,sha256=cxwfaARtdMSpn7x0NULXp9yZwWQcDSwXK94W0HpUKbY,8793
-celestical/helper.py,sha256=nenDhvj4eCABSqdn4GslwtPk7RxNWJXLl-Ty941gdMo,6601
-celestical/user.py,sha256=AN3o0mBymjIvo0j3zBYIVPhim2XsBybNMB06n5OXGUY,7294
-celestical-0.14.3.dist-info/COPYING,sha256=5X8cMguM-HmKfS_4Om-eBqM6A1hfbgZf6pfx2G24QFI,35150
-celestical-0.14.3.dist-info/COPYING.LESSER,sha256=GkWx0KhgPf4s_GRPnauXCxdi-Sur4qrG6y9dRXLEpoA,7653
-celestical-0.14.3.dist-info/LICENSE,sha256=l4pgftTXn9aA9oyWYwUdY8St5XfN8v5bCjhSUZhNmfo,108
-celestical-0.14.3.dist-info/METADATA,sha256=2o2c0iIWAVPgWAQECFOdfTsBB39gO7401Nwqn3pasMg,2587
-celestical-0.14.3.dist-info/WHEEL,sha256=d2fvjOD7sXsVzChCqf0Ty0JbHKBaLYwDbGQDwQTnJ50,88
-celestical-0.14.3.dist-info/entry_points.txt,sha256=I9_Hd8RvzIQVnSpFYLGSdlXl1SYrs2lg_4m8Rnghi1M,49
-celestical-0.14.3.dist-info/RECORD,,
+celestical/cli.py,sha256=GrP4lFfw-HXAwMFD7eo4o0cvWROA3o-qjz0MK_1JVTo,2425
+celestical/compose.py,sha256=0jzvhRW83W-xbDSExO7PUdaws9zOR71eO44qhRMw1E8,17341
+celestical/configuration.py,sha256=mVGYayYGvgQuhSP4T_0xAMoF5BXn72kCav-_UyONYkU,3900
+celestical/docker_local.py,sha256=A6tCVj3FIWmfGdB2b6Vz_apsWrzRA4eRF-PHSSjj2Jw,6138
+celestical/helper.py,sha256=krDgEOa0BtjuCSA4Wa3poP92THjTrC5pDV7iJBYpK20,6457
+celestical/stack_upload.py,sha256=y7WbQy-pgH0jI4vOiVmeHASQ_5tcLUjvK5h13PAspGI,9
+celestical/user.py,sha256=9Iz8GoMoQJe7wqHWcedp57vFLY5Bb9cutGesQ-XVbtk,6428
+celestical-0.9.2.dist-info/COPYING,sha256=5X8cMguM-HmKfS_4Om-eBqM6A1hfbgZf6pfx2G24QFI,35150
+celestical-0.9.2.dist-info/COPYING.LESSER,sha256=GkWx0KhgPf4s_GRPnauXCxdi-Sur4qrG6y9dRXLEpoA,7653
+celestical-0.9.2.dist-info/LICENSE,sha256=l4pgftTXn9aA9oyWYwUdY8St5XfN8v5bCjhSUZhNmfo,108
+celestical-0.9.2.dist-info/METADATA,sha256=U20NPz92MQJX6-DGECdzrM17RvOApDP1ybQQZcEd-Gk,1959
+celestical-0.9.2.dist-info/WHEEL,sha256=d2fvjOD7sXsVzChCqf0Ty0JbHKBaLYwDbGQDwQTnJ50,88
+celestical-0.9.2.dist-info/entry_points.txt,sha256=I9_Hd8RvzIQVnSpFYLGSdlXl1SYrs2lg_4m8Rnghi1M,49
+celestical-0.9.2.dist-info/RECORD,,
```

