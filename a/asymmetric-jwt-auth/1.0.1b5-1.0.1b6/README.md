# Comparing `tmp/asymmetric_jwt_auth-1.0.1b5.tar.gz` & `tmp/asymmetric_jwt_auth-1.0.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asymmetric_jwt_auth-1.0.1b5.tar", max compression
+gzip compressed data, was "asymmetric_jwt_auth-1.0.1b6.tar", max compression
```

## Comparing `asymmetric_jwt_auth-1.0.1b5.tar` & `asymmetric_jwt_auth-1.0.1b6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      768 2024-05-01 23:05:52.544514 asymmetric_jwt_auth-1.0.1b5/LICENSE.md
--rw-r--r--   0        0        0     2769 2024-05-01 23:05:52.544514 asymmetric_jwt_auth-1.0.1b5/README.rst
--rw-r--r--   0        0        0     1116 2024-05-01 23:05:52.545514 asymmetric_jwt_auth-1.0.1b5/pyproject.toml
--rw-r--r--   0        0        0     1311 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/__init__.py
--rw-r--r--   0        0        0      465 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/admin.py
--rw-r--r--   0        0        0      152 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/apps.py
--rw-r--r--   0        0        0     6749 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/keys.py
--rw-r--r--   0        0        0        0 2024-05-01 23:05:52.571514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/management/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 23:05:52.571514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/management/commands/__init__.py
--rw-r--r--   0        0        0      758 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/management/commands/generate_key_pair.py
--rw-r--r--   0        0        0     2820 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/middleware.py
--rw-r--r--   0        0        0     1066 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/migrations/0001_initial.py
--rw-r--r--   0        0        0      524 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/migrations/0002_publickey_comment.py
--rw-r--r--   0        0        0      500 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/migrations/0003_auto_20151112_1547.py
--rw-r--r--   0        0        0      794 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/migrations/0004_auto_20191104_1628.py
--rw-r--r--   0        0        0     2813 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/migrations/0005_auto_20210304_1116.py
--rw-r--r--   0        0        0        0 2024-05-01 23:05:52.572514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/migrations/__init__.py
--rw-r--r--   0        0        0     3944 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/models.py
--rw-r--r--   0        0        0      274 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/nonce/__init__.py
--rw-r--r--   0        0        0      429 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/nonce/base.py
--rw-r--r--   0        0        0     1372 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/nonce/django.py
--rw-r--r--   0        0        0      521 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/nonce/null.py
--rw-r--r--   0        0        0      543 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/repos/__init__.py
--rw-r--r--   0        0        0      465 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/repos/base.py
--rw-r--r--   0        0        0     1979 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/repos/django.py
--rw-r--r--   0        0        0        0 2024-05-01 23:05:52.575514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/__init__.py
--rw-r--r--   0        0        0     2912 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/data.py
--rw-r--r--   0        0        0     1704 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa.privkey
--rw-r--r--   0        0        0      451 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa.pub
--rw-r--r--   0        0        0     1766 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa_encrypted.privkey
--rw-r--r--   0        0        0      404 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa_encrypted.pub
--rw-r--r--   0        0        0       29 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_admin.py
--rw-r--r--   0        0        0     1224 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_commands.py
--rw-r--r--   0        0        0     6056 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_keys.py
--rw-r--r--   0        0        0     8685 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_middleware.py
--rw-r--r--   0        0        0     4679 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_models.py
--rw-r--r--   0        0        0      519 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_settings.py
--rw-r--r--   0        0        0     4316 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_token.py
--rw-r--r--   0        0        0       71 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_utils.py
--rw-r--r--   0        0        0     3298 2024-05-01 23:05:52.548514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_views.py
--rw-r--r--   0        0        0     3809 2024-05-01 23:05:52.548514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tokens.py
--rw-r--r--   0        0        0      341 2024-05-01 23:05:52.548514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/urls.py
--rw-r--r--   0        0        0      582 2024-05-01 23:05:52.548514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/utils.py
--rw-r--r--   0        0        0      691 2024-05-01 23:05:52.548514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/views.py
--rw-r--r--   0        0        0     3781 1970-01-01 00:00:00.000000 asymmetric_jwt_auth-1.0.1b5/PKG-INFO
+-rw-r--r--   0        0        0      768 2024-05-01 23:12:22.580585 asymmetric_jwt_auth-1.0.1b6/LICENSE.md
+-rw-r--r--   0        0        0     2769 2024-05-01 23:12:22.580585 asymmetric_jwt_auth-1.0.1b6/README.rst
+-rw-r--r--   0        0        0     1116 2024-05-01 23:12:22.581585 asymmetric_jwt_auth-1.0.1b6/pyproject.toml
+-rw-r--r--   0        0        0     1311 2024-05-01 23:12:22.581585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/__init__.py
+-rw-r--r--   0        0        0      465 2024-05-01 23:12:22.581585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/admin.py
+-rw-r--r--   0        0        0      152 2024-05-01 23:12:22.581585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/apps.py
+-rw-r--r--   0        0        0     6749 2024-05-01 23:12:22.581585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/keys.py
+-rw-r--r--   0        0        0        0 2024-05-01 23:12:22.606585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 23:12:22.606585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/management/commands/__init__.py
+-rw-r--r--   0        0        0      758 2024-05-01 23:12:22.581585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/management/commands/generate_key_pair.py
+-rw-r--r--   0        0        0     2820 2024-05-01 23:12:22.581585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/middleware.py
+-rw-r--r--   0        0        0     1066 2024-05-01 23:12:22.581585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/migrations/0001_initial.py
+-rw-r--r--   0        0        0      524 2024-05-01 23:12:22.582585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/migrations/0002_publickey_comment.py
+-rw-r--r--   0        0        0      500 2024-05-01 23:12:22.582585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/migrations/0003_auto_20151112_1547.py
+-rw-r--r--   0        0        0      794 2024-05-01 23:12:22.582585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/migrations/0004_auto_20191104_1628.py
+-rw-r--r--   0        0        0     2813 2024-05-01 23:12:22.582585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/migrations/0005_auto_20210304_1116.py
+-rw-r--r--   0        0        0        0 2024-05-01 23:12:22.607585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/migrations/__init__.py
+-rw-r--r--   0        0        0     3944 2024-05-01 23:12:22.582585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/models.py
+-rw-r--r--   0        0        0      274 2024-05-01 23:12:22.582585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/nonce/__init__.py
+-rw-r--r--   0        0        0      429 2024-05-01 23:12:22.582585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/nonce/base.py
+-rw-r--r--   0        0        0     1372 2024-05-01 23:12:22.582585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/nonce/django.py
+-rw-r--r--   0        0        0      521 2024-05-01 23:12:22.582585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/nonce/null.py
+-rw-r--r--   0        0        0      543 2024-05-01 23:12:22.582585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/repos/__init__.py
+-rw-r--r--   0        0        0      465 2024-05-01 23:12:22.582585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/repos/base.py
+-rw-r--r--   0        0        0     1979 2024-05-01 23:12:22.582585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/repos/django.py
+-rw-r--r--   0        0        0        0 2024-05-01 23:12:22.610585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/__init__.py
+-rw-r--r--   0        0        0     2912 2024-05-01 23:12:22.582585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/data.py
+-rw-r--r--   0        0        0     1704 2024-05-01 23:12:22.582585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa.privkey
+-rw-r--r--   0        0        0      451 2024-05-01 23:12:22.582585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa.pub
+-rw-r--r--   0        0        0     1766 2024-05-01 23:12:22.582585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa_encrypted.privkey
+-rw-r--r--   0        0        0      404 2024-05-01 23:12:22.582585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa_encrypted.pub
+-rw-r--r--   0        0        0       29 2024-05-01 23:12:22.582585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/test_admin.py
+-rw-r--r--   0        0        0     1224 2024-05-01 23:12:22.582585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/test_commands.py
+-rw-r--r--   0        0        0     6056 2024-05-01 23:12:22.582585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/test_keys.py
+-rw-r--r--   0        0        0     8685 2024-05-01 23:12:22.583585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/test_middleware.py
+-rw-r--r--   0        0        0     4679 2024-05-01 23:12:22.583585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/test_models.py
+-rw-r--r--   0        0        0      519 2024-05-01 23:12:22.583585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/test_settings.py
+-rw-r--r--   0        0        0     4316 2024-05-01 23:12:22.583585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/test_token.py
+-rw-r--r--   0        0        0       71 2024-05-01 23:12:22.583585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/test_utils.py
+-rw-r--r--   0        0        0     3298 2024-05-01 23:12:22.583585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/test_views.py
+-rw-r--r--   0        0        0     3809 2024-05-01 23:12:22.583585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tokens.py
+-rw-r--r--   0        0        0      341 2024-05-01 23:12:22.583585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/urls.py
+-rw-r--r--   0        0        0      582 2024-05-01 23:12:22.583585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/utils.py
+-rw-r--r--   0        0        0      691 2024-05-01 23:12:22.583585 asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/views.py
+-rw-r--r--   0        0        0     3781 1970-01-01 00:00:00.000000 asymmetric_jwt_auth-1.0.1b6/PKG-INFO
```

### Comparing `asymmetric_jwt_auth-1.0.1b5/LICENSE.md` & `asymmetric_jwt_auth-1.0.1b6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/README.rst` & `asymmetric_jwt_auth-1.0.1b6/README.rst`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/pyproject.toml` & `asymmetric_jwt_auth-1.0.1b6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asymmetric_jwt_auth"
-version = "1.0.1-b5"
+version = "1.0.1-b6"
 description = "Asymmetric key based authentication for HTTP APIs"
 authors = ["Craig Weber <crgwbr@gmail.com>"]
 maintainers = ["Craig Weber <crgwbr@gmail.com>"]
 readme = "README.rst"
 homepage = "https://gitlab.com/crgwbr/asymmetric_jwt_auth"
 repository = "https://gitlab.com/crgwbr/asymmetric_jwt_auth"
 license = "ISC"
```

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/__init__.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/keys.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/keys.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/management/commands/generate_key_pair.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/management/commands/generate_key_pair.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/middleware.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/middleware.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/migrations/0001_initial.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/migrations/0002_publickey_comment.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/migrations/0002_publickey_comment.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/migrations/0004_auto_20191104_1628.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/migrations/0004_auto_20191104_1628.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/migrations/0005_auto_20210304_1116.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/migrations/0005_auto_20210304_1116.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/models.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/models.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/nonce/django.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/nonce/django.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/nonce/null.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/nonce/null.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/repos/__init__.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/repos/__init__.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/repos/django.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/repos/django.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/data.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/data.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa.privkey` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa.privkey`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa_encrypted.privkey` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa_encrypted.privkey`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_commands.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_keys.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/test_keys.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_middleware.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_models.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_settings.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_token.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_views.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tokens.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/tokens.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/utils.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/utils.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/views.py` & `asymmetric_jwt_auth-1.0.1b6/src/asymmetric_jwt_auth/views.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.1b5/PKG-INFO` & `asymmetric_jwt_auth-1.0.1b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asymmetric_jwt_auth
-Version: 1.0.1b5
+Version: 1.0.1b6
 Summary: Asymmetric key based authentication for HTTP APIs
 Home-page: https://gitlab.com/crgwbr/asymmetric_jwt_auth
 License: ISC
 Author: Craig Weber
 Author-email: crgwbr@gmail.com
 Maintainer: Craig Weber
 Maintainer-email: crgwbr@gmail.com
```

