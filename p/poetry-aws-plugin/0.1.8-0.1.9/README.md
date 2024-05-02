# Comparing `tmp/poetry_aws_plugin-0.1.8.tar.gz` & `tmp/poetry_aws_plugin-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_aws_plugin-0.1.8.tar", max compression
+gzip compressed data, was "poetry_aws_plugin-0.1.9.tar", max compression
```

## Comparing `poetry_aws_plugin-0.1.8.tar` & `poetry_aws_plugin-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.8/LICENSE
--rw-r--r--   0        0        0     2831 2024-04-12 00:00:11.575002 poetry_aws_plugin-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.8/poetry_aws_plugin/__init__.py
--rw-r--r--   0        0        0     6099 2024-04-12 16:09:16.337468 poetry_aws_plugin-0.1.8/poetry_aws_plugin/plugin.py
--rw-r--r--   0        0        0      684 2024-04-12 16:09:55.405467 poetry_aws_plugin-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3604 1970-01-01 00:00:00.000000 poetry_aws_plugin-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2848 2024-04-12 17:06:58.165764 poetry_aws_plugin-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.9/poetry_aws_plugin/__init__.py
+-rw-r--r--   0        0        0     5845 2024-04-12 17:10:33.677775 poetry_aws_plugin-0.1.9/poetry_aws_plugin/plugin.py
+-rw-r--r--   0        0        0      684 2024-04-12 17:07:18.537765 poetry_aws_plugin-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3621 1970-01-01 00:00:00.000000 poetry_aws_plugin-0.1.9/PKG-INFO
```

### Comparing `poetry_aws_plugin-0.1.8/LICENSE` & `poetry_aws_plugin-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_aws_plugin-0.1.8/README.md` & `poetry_aws_plugin-0.1.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Poetry AWS Plugin
 
 This is a poetry plugin to help with AWS CodeArtifact authorization by automatically getting the authorization token.
 
-When installing or publishing packages through poetry and running into a CodeArtifact-related authorization error, the plugin will automatically get the authorization token and retry the command.
+When installing or publishing packages through poetry, the plugin will check whether the command requires CodeArtifact authorization, and if so, adds it automatically.
 
 The plugin will try two methods of authorization, in this order:
 
 1. Use AWS credentials to run `codeartifact.GetAuthorizationToken`.
 2. Use AWS credentials to run `sts.AssumeRole`, then use that role to run `codeartifact.GetAuthorizationToken`.
 
 ## Installation
@@ -23,15 +23,15 @@
 poetry self remove poetry-aws-plugin
 ```
 
 ## Usage
 
 You must ensure that your AWS credentials are configured and discoverable by `boto3`. The [`boto3` documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html#configuring-credentials) has details on how to configure your credentials and the order in which they searched.
 
-When poetry runs a command that uses CodeArtifact and fails to authorize, the plugin will automatically attempt to get the authorization token and retry the command.
+When poetry runs a command that uses CodeArtifact, the plugin will automatically check whether the command needs authorization, and if so, requests a CodeArtifact authorization token and adds it to the command.
 
 Your AWS credentials must be authorized to do atleast one of the following:
 
 1. Run [`codeartifact.GetAuthorizationToken`](https://docs.aws.amazon.com/cli/latest/reference/codeartifact/get-authorization-token.html).
 2. Run [`sts.AssumeRole`](https://docs.aws.amazon.com/cli/latest/reference/sts/assume-role.html) to assume a role with authorization to run [`codeartifact.GetAuthorizationToken`](https://docs.aws.amazon.com/cli/latest/reference/codeartifact/get-authorization-token.html).
 
 **To use IAM roles to authorize, set the environment variable `POETRY_AWS_PLUGIN_ROLE_ARN` to the role's ARN before running any poetry commands**.
```

### Comparing `poetry_aws_plugin-0.1.8/poetry_aws_plugin/plugin.py` & `poetry_aws_plugin-0.1.9/poetry_aws_plugin/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 import logging
 import os
 import re
 from typing import Any
 
 import boto3
 import requests
-from requests.utils import rewind_body
 
 from botocore.exceptions import ClientError
-from poetry.exceptions import PoetryException
 from poetry.plugins import Plugin
 from poetry.publishing.uploader import Uploader
 from poetry.utils.authenticator import Authenticator
 
 POETRY_AWS_PLUGIN_ROLE_ARN_VAR = "POETRY_AWS_PLUGIN_ROLE_ARN"
 POETRY_AWS_PLUGIN_SESSION_NAME = "poetry-aws-plugin"
 POETRY_AWS_PLUGIN_AUTH_TOKEN_VAR = "POETRY_AWS_PLUGIN_AUTH_TOKEN"
 
-UNAUTHORIZED_STATUS_CODES = (401, 403)
 CODEARTIFACT_URL_REGEX = r"^https://([a-z][a-z-]*)-(\d+)\.d\.codeartifact\.[^.]+\.amazonaws\.com.*$"
 
-RETRY_ERROR_MESSAGE = f"""
+AUTH_ERROR_MESSAGE = f"""
 Make sure you have AWS credentials configured and up-to-date
 
 Then make sure you have atleast one of the following:
     1. Authorization for CodeArtifact with your current credentials
     2. Authorization for an IAM role that has access to CodeArtifact and
        environment variable '{POETRY_AWS_PLUGIN_ROLE_ARN_VAR}' set to that role's ARN
 """
@@ -32,18 +29,18 @@
 logger = logging.getLogger("PoetryAwsPlugin")
 
 
 authenticator_create_session = Authenticator.create_session
 uploader_make_session = Uploader.make_session
 
 
-def is_retryable(response: requests.Response) -> bool:
-    if response.status_code not in UNAUTHORIZED_STATUS_CODES:
+def requires_authorization(request: requests.PreparedRequest) -> bool:
+    if request.headers.get("Authorization", None):
         return False
-    if not re.match(CODEARTIFACT_URL_REGEX, response.url):
+    if not re.match(CODEARTIFACT_URL_REGEX, request.url):
         return False
     return True
 
 
 def get_auth_token(domain: str, domain_owner: str) -> str:
     logger.debug(
         f"Getting new CodeArtifact authorization token for domain '{domain}' and domain owner '{domain_owner}'"
@@ -70,16 +67,16 @@
     try:
         boto3.client("sts").get_caller_identity()
         return True
     except ClientError as err:
         logger.debug(f"Error using current credentials: {err}")
         return False
     except Exception as err:
-        logger.debug(f"Unexpected error while validating AWS credentials\n{RETRY_ERROR_MESSAGE}")
-        raise err
+        logger.debug(f"Unexpected error while validating AWS credentials: {err}\n{AUTH_ERROR_MESSAGE}")
+        return False
 
 
 def get_auth_token_with_current_credentials(domain: str, domain_owner: str) -> str:
     try:
         token_response = boto3.client("codeartifact").get_authorization_token(
             domain=domain,
             domainOwner=domain_owner,
@@ -128,39 +125,35 @@
 
 
 def get_auth_token_from_env(*args: Any, **kwargs: Any) -> str:
     return os.environ.get(POETRY_AWS_PLUGIN_AUTH_TOKEN_VAR, "")
 
 
 def patched_session_send(self: requests.Session, request: requests.PreparedRequest, **kwargs: Any) -> requests.Response:
-    response = requests.Session.send(self, request.copy(), **kwargs.copy())
-    if not is_retryable(response):
-        return response
+    if not requires_authorization(request):
+        return requests.Session.send(self, request, **kwargs)
 
-    logger.debug("Failed to get authorization for CodeArtifact")
+    logger.debug("Adding CodeArtifact authorization to request")
 
-    match = re.match(CODEARTIFACT_URL_REGEX, response.url)
+    match = re.match(CODEARTIFACT_URL_REGEX, request.url)
     domain, domain_owner = match.groups()
 
     auth_token = get_auth_token(domain, domain_owner)
     if not auth_token:
-        raise PoetryException(RETRY_ERROR_MESSAGE)
+        logger.warning(AUTH_ERROR_MESSAGE)
+        # Try the request anyway
+        return requests.Session.send(self, request, **kwargs)
 
-    logger.debug("Successfully got CodeArtifact authorization token\nRetrying request")
+    logger.debug("Successfully got CodeArtifact authorization token")
 
-    # Use the received auth token for the session
+    # Add the auth to session and request
     self.auth = ("aws", auth_token)
+    request.prepare_auth(self.auth)
 
-    # And create a new request using the new auth
-    new_request = request.copy()
-    rewind_body(new_request)
-    new_request.prepare_auth(self.auth, request.url)
-
-    # And finally we retry the request
-    return requests.Session.send(self, new_request, **kwargs)
+    return requests.Session.send(self, request, **kwargs)
 
 
 def patched_authenticator_create_session(self: Authenticator) -> requests.Session:
     session = authenticator_create_session(self)
     session.send = patched_session_send.__get__(session)
     return session
```

### Comparing `poetry_aws_plugin-0.1.8/pyproject.toml` & `poetry_aws_plugin-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-aws-plugin"
-version = "0.1.8"
+version = "0.1.9"
 description = "A poetry plugin to help with AWS CodeArtifact authorization automatically"
 license = "MIT"
 authors = ["Song Huang <xiasongh@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/xiasongh/poetry-aws-plugin"
 keywords = ["aws", "codeartifact", "poetry"]
 packages = [{include = "poetry_aws_plugin"}]
```

### Comparing `poetry_aws_plugin-0.1.8/PKG-INFO` & `poetry_aws_plugin-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-aws-plugin
-Version: 0.1.8
+Version: 0.1.9
 Summary: A poetry plugin to help with AWS CodeArtifact authorization automatically
 Home-page: https://github.com/xiasongh/poetry-aws-plugin
 License: MIT
 Keywords: aws,codeartifact,poetry
 Author: Song Huang
 Author-email: xiasongh@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -18,15 +18,15 @@
 Project-URL: Repository, https://github.com/xiasongh/poetry-aws-plugin
 Description-Content-Type: text/markdown
 
 # Poetry AWS Plugin
 
 This is a poetry plugin to help with AWS CodeArtifact authorization by automatically getting the authorization token.
 
-When installing or publishing packages through poetry and running into a CodeArtifact-related authorization error, the plugin will automatically get the authorization token and retry the command.
+When installing or publishing packages through poetry, the plugin will check whether the command requires CodeArtifact authorization, and if so, adds it automatically.
 
 The plugin will try two methods of authorization, in this order:
 
 1. Use AWS credentials to run `codeartifact.GetAuthorizationToken`.
 2. Use AWS credentials to run `sts.AssumeRole`, then use that role to run `codeartifact.GetAuthorizationToken`.
 
 ## Installation
@@ -43,15 +43,15 @@
 poetry self remove poetry-aws-plugin
 ```
 
 ## Usage
 
 You must ensure that your AWS credentials are configured and discoverable by `boto3`. The [`boto3` documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html#configuring-credentials) has details on how to configure your credentials and the order in which they searched.
 
-When poetry runs a command that uses CodeArtifact and fails to authorize, the plugin will automatically attempt to get the authorization token and retry the command.
+When poetry runs a command that uses CodeArtifact, the plugin will automatically check whether the command needs authorization, and if so, requests a CodeArtifact authorization token and adds it to the command.
 
 Your AWS credentials must be authorized to do atleast one of the following:
 
 1. Run [`codeartifact.GetAuthorizationToken`](https://docs.aws.amazon.com/cli/latest/reference/codeartifact/get-authorization-token.html).
 2. Run [`sts.AssumeRole`](https://docs.aws.amazon.com/cli/latest/reference/sts/assume-role.html) to assume a role with authorization to run [`codeartifact.GetAuthorizationToken`](https://docs.aws.amazon.com/cli/latest/reference/codeartifact/get-authorization-token.html).
 
 **To use IAM roles to authorize, set the environment variable `POETRY_AWS_PLUGIN_ROLE_ARN` to the role's ARN before running any poetry commands**.
```

