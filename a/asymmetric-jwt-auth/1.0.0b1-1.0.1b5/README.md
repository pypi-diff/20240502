# Comparing `tmp/asymmetric_jwt_auth-1.0.0b1.tar.gz` & `tmp/asymmetric_jwt_auth-1.0.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asymmetric_jwt_auth-1.0.0b1.tar", last modified: Fri Mar  5 22:43:32 2021, max compression
+gzip compressed data, was "asymmetric_jwt_auth-1.0.1b5.tar", max compression
```

## Comparing `asymmetric_jwt_auth-1.0.0b1.tar` & `asymmetric_jwt_auth-1.0.1b5.tar`

### file list

```diff
@@ -1,72 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-05 22:43:32.516067 asymmetric_jwt_auth-1.0.0b1/
--rw-rw-rw-   0 root         (0) root         (0)      748 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)      129 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3881 2021-03-05 22:43:32.516067 asymmetric_jwt_auth-1.0.0b1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2574 2021-03-05 22:43:23.000000 asymmetric_jwt_auth-1.0.0b1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-05 22:43:32.512067 asymmetric_jwt_auth-1.0.0b1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     1373 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/docs/api.rst
--rw-rw-rw-   0 root         (0) root         (0)     2067 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/docs/changes.rst
--rw-rw-rw-   0 root         (0) root         (0)      127 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1383 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/docs/install.rst
--rw-rw-rw-   0 root         (0) root         (0)       44 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/docs/license.rst
--rw-rw-rw-   0 root         (0) root         (0)     3689 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/docs/usage.rst
--rw-rw-rw-   0 root         (0) root         (0)      894 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      237 2021-03-05 22:43:32.516067 asymmetric_jwt_auth-1.0.0b1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1827 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-05 22:43:32.508067 asymmetric_jwt_auth-1.0.0b1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-05 22:43:32.512067 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/
--rw-rw-rw-   0 root         (0) root         (0)     1380 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      465 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      152 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     6718 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-05 22:43:32.512067 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-05 22:43:32.512067 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      782 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/management/commands/generate_key_pair.py
--rw-rw-rw-   0 root         (0) root         (0)     2822 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-05 22:43:32.512067 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      735 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/migrations/0002_publickey_comment.py
--rw-rw-rw-   0 root         (0) root         (0)      471 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/migrations/0003_auto_20151112_1547.py
--rw-rw-rw-   0 root         (0) root         (0)      718 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/migrations/0004_auto_20191104_1628.py
--rw-rw-rw-   0 root         (0) root         (0)     2060 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/migrations/0005_auto_20210304_1116.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3893 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-05 22:43:32.512067 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/nonce/
--rw-rw-rw-   0 root         (0) root         (0)      274 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/nonce/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      404 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/nonce/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1352 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/nonce/django.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/nonce/null.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-05 22:43:32.516067 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/repos/
--rw-rw-rw-   0 root         (0) root         (0)      543 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/repos/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      451 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/repos/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1984 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/repos/django.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-05 22:43:32.516067 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2912 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-05 22:43:32.516067 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)     1704 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa.privkey
--rw-rw-rw-   0 root         (0) root         (0)      451 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa.pub
--rw-rw-rw-   0 root         (0) root         (0)     1766 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa_encrypted.privkey
--rw-rw-rw-   0 root         (0) root         (0)      404 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa_encrypted.pub
--rw-rw-rw-   0 root         (0) root         (0)       29 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/test_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     1263 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/test_commands.py
--rw-rw-rw-   0 root         (0) root         (0)     5861 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/test_keys.py
--rw-rw-rw-   0 root         (0) root         (0)     8787 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/test_middleware.py
--rw-rw-rw-   0 root         (0) root         (0)     4712 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)      521 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/test_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     4233 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/test_token.py
--rw-rw-rw-   0 root         (0) root         (0)       71 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3076 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/test_views.py
--rw-rw-rw-   0 root         (0) root         (0)     3754 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tokens.py
--rw-rw-rw-   0 root         (0) root         (0)      357 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      582 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      693 2021-03-05 22:38:54.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-05 22:43:32.512067 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3881 2021-03-05 22:43:32.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2264 2021-03-05 22:43:32.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-03-05 22:43:32.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      235 2021-03-05 22:43:32.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2021-03-05 22:43:32.000000 asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        9 2021-03-05 22:43:32.000000 asymmetric_jwt_auth-1.0.0b1/version.txt
+-rw-r--r--   0        0        0      768 2024-05-01 23:05:52.544514 asymmetric_jwt_auth-1.0.1b5/LICENSE.md
+-rw-r--r--   0        0        0     2769 2024-05-01 23:05:52.544514 asymmetric_jwt_auth-1.0.1b5/README.rst
+-rw-r--r--   0        0        0     1116 2024-05-01 23:05:52.545514 asymmetric_jwt_auth-1.0.1b5/pyproject.toml
+-rw-r--r--   0        0        0     1311 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/__init__.py
+-rw-r--r--   0        0        0      465 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/admin.py
+-rw-r--r--   0        0        0      152 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/apps.py
+-rw-r--r--   0        0        0     6749 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/keys.py
+-rw-r--r--   0        0        0        0 2024-05-01 23:05:52.571514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 23:05:52.571514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/management/commands/__init__.py
+-rw-r--r--   0        0        0      758 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/management/commands/generate_key_pair.py
+-rw-r--r--   0        0        0     2820 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/middleware.py
+-rw-r--r--   0        0        0     1066 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/migrations/0001_initial.py
+-rw-r--r--   0        0        0      524 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/migrations/0002_publickey_comment.py
+-rw-r--r--   0        0        0      500 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/migrations/0003_auto_20151112_1547.py
+-rw-r--r--   0        0        0      794 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/migrations/0004_auto_20191104_1628.py
+-rw-r--r--   0        0        0     2813 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/migrations/0005_auto_20210304_1116.py
+-rw-r--r--   0        0        0        0 2024-05-01 23:05:52.572514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/migrations/__init__.py
+-rw-r--r--   0        0        0     3944 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/models.py
+-rw-r--r--   0        0        0      274 2024-05-01 23:05:52.546514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/nonce/__init__.py
+-rw-r--r--   0        0        0      429 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/nonce/base.py
+-rw-r--r--   0        0        0     1372 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/nonce/django.py
+-rw-r--r--   0        0        0      521 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/nonce/null.py
+-rw-r--r--   0        0        0      543 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/repos/__init__.py
+-rw-r--r--   0        0        0      465 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/repos/base.py
+-rw-r--r--   0        0        0     1979 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/repos/django.py
+-rw-r--r--   0        0        0        0 2024-05-01 23:05:52.575514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/__init__.py
+-rw-r--r--   0        0        0     2912 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/data.py
+-rw-r--r--   0        0        0     1704 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa.privkey
+-rw-r--r--   0        0        0      451 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa.pub
+-rw-r--r--   0        0        0     1766 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa_encrypted.privkey
+-rw-r--r--   0        0        0      404 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa_encrypted.pub
+-rw-r--r--   0        0        0       29 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_admin.py
+-rw-r--r--   0        0        0     1224 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_commands.py
+-rw-r--r--   0        0        0     6056 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_keys.py
+-rw-r--r--   0        0        0     8685 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_middleware.py
+-rw-r--r--   0        0        0     4679 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_models.py
+-rw-r--r--   0        0        0      519 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_settings.py
+-rw-r--r--   0        0        0     4316 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_token.py
+-rw-r--r--   0        0        0       71 2024-05-01 23:05:52.547514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_utils.py
+-rw-r--r--   0        0        0     3298 2024-05-01 23:05:52.548514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_views.py
+-rw-r--r--   0        0        0     3809 2024-05-01 23:05:52.548514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tokens.py
+-rw-r--r--   0        0        0      341 2024-05-01 23:05:52.548514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/urls.py
+-rw-r--r--   0        0        0      582 2024-05-01 23:05:52.548514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/utils.py
+-rw-r--r--   0        0        0      691 2024-05-01 23:05:52.548514 asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/views.py
+-rw-r--r--   0        0        0     3781 1970-01-01 00:00:00.000000 asymmetric_jwt_auth-1.0.1b5/PKG-INFO
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/LICENSE.md` & `asymmetric_jwt_auth-1.0.1b5/LICENSE.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,4 +1,15 @@
-Copyright (c) 2021, Craig Weber <crgwbr@gmail.com>
+ISC License
 
-Permission to use, copy, modify, and/or distribute this software for any purpose with or without fee is hereby granted, provided that the above copyright notice and this permission notice appear in all copies.
-THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
+Copyright (c) 2015 - 2024 Craig Weber <crgwbr@gmail.com>
+
+Permission to use, copy, modify, and/or distribute this software for any
+purpose with or without fee is hereby granted, provided that the above
+copyright notice and this permission notice appear in all copies.
+
+THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
+AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,
+INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM
+LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
+OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
+PERFORMANCE OF THIS SOFTWARE.
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/PKG-INFO` & `asymmetric_jwt_auth-1.0.1b5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,94 +1,105 @@
 Metadata-Version: 2.1
 Name: asymmetric_jwt_auth
-Version: 1.0.0b1
+Version: 1.0.1b5
 Summary: Asymmetric key based authentication for HTTP APIs
-Home-page: https://github.com/crgwbr/asymmetric-jwt-auth
+Home-page: https://gitlab.com/crgwbr/asymmetric_jwt_auth
+License: ISC
 Author: Craig Weber
 Author-email: crgwbr@gmail.com
-License: ISC
-Description: Asymmetric JWT Authentication
-        =============================
-        
-        .. image:: https://img.shields.io/pypi/v/asymmetric_jwt_auth.svg
-            :target: https://pypi.python.org/pypi/asymmetric_jwt_auth
-        
-        .. image:: https://travis-ci.org/crgwbr/asymmetric-jwt-auth.svg
-            :target: https://travis-ci.org/crgwbr/asymmetric-jwt-auth
-        
-        
-        What?
-        -----
-        
-        This is an library designed to handle authentication in
-        *server-to-server* API requests. It accomplishes this using RSA public /
-        private key pairs.
-        
-        
-        Why?
-        ----
-        
-        The standard pattern of using username and password works well for
-        user-to-server requests, but is lacking for server-to-server
-        applications. In these scenarios, since the password doesn’t need to be
-        memorable by a user, we can use something far more secure: asymmetric
-        key cryptography. This has the advantage that a password is never
-        actually sent to the server.
-        
-        
-        How?
-        ----
-        
-        A public / private key pair is generated by the client machine. The
-        server machine is then supplied with the public key, which it can store
-        in any method it likes. When this library is used with Django, it
-        provides a model for storing public keys associated with built-in User
-        objects. When a request is made, the client creates a JWT including
-        several claims and signs it using it’s private key. Upon receipt, the
-        server verifies the claim to using the public key to ensure the issuer
-        is legitimately who they claim to be.
-        
-        The claim (issued by the client) includes components: the username of
-        the user who is attempting authentication, the current unix timestamp,
-        and a randomly generated nonce. For example:
-        
-        ::
-        
-            {
-                "username": "guido",
-                "time": 1439216312,
-                "nonce": "1"
-            }
-        
-        The timestamp must be within ±20 seconds of the server time and the
-        nonce must be unique within the given timestamp and user. In other
-        words, if more than one request from a user is made within the same
-        second, the nonce must change. Due to these two factors no token is
-        usable more than once, thereby preventing replay attacks.
-        
-        To make an authenticated request, the client must generate a JWT
-        following the above format and include it as the HTTP Authorization
-        header in the following format:
-        
-        ::
-        
-            Authorization: JWT <my_token>
-        
-        **Important note**: the claim is *not* encrypted, only signed.
-        Additionally, the signature only prevents the claim from being tampered
-        with or re-used. Every other part of the request is still vulnerable to
-        tamper. Therefore, this is not a replacement for using SSL in the
-        transport layer.
-        
-        **Full Documentation**: https://asymmetric-jwt-auth.readthedocs.io
-        
-Platform: UNKNOWN
+Maintainer: Craig Weber
+Maintainer-email: crgwbr@gmail.com
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: ISC License (ISCL)
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Provides-Extra: development
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: Django (>=3.2)
+Requires-Dist: PyJWT (>=2.0.1)
+Requires-Dist: cryptography (>=3.4.6)
+Project-URL: Repository, https://gitlab.com/crgwbr/asymmetric_jwt_auth
+Description-Content-Type: text/x-rst
+
+Asymmetric JWT Authentication
+=============================
+
+.. image:: https://img.shields.io/pypi/v/asymmetric_jwt_auth.svg
+    :target: https://pypi.python.org/pypi/asymmetric_jwt_auth
+
+.. image:: https://gitlab.com/crgwbr/asymmetric_jwt_auth/badges/master/pipeline.svg
+    :target: https://gitlab.com/crgwbr/asymmetric_jwt_auth/-/commits/master
+
+.. image:: https://gitlab.com/crgwbr/asymmetric_jwt_auth/badges/master/coverage.svg
+    :target: https://gitlab.com/crgwbr/asymmetric_jwt_auth/-/commits/master
+
+
+What?
+-----
+
+This is an library designed to handle authentication in
+*server-to-server* API requests. It accomplishes this using RSA public /
+private key pairs.
+
+
+Why?
+----
+
+The standard pattern of using username and password works well for
+user-to-server requests, but is lacking for server-to-server
+applications. In these scenarios, since the password doesn’t need to be
+memorable by a user, we can use something far more secure: asymmetric
+key cryptography. This has the advantage that a password is never
+actually sent to the server.
+
+
+How?
+----
+
+A public / private key pair is generated by the client machine. The
+server machine is then supplied with the public key, which it can store
+in any method it likes. When this library is used with Django, it
+provides a model for storing public keys associated with built-in User
+objects. When a request is made, the client creates a JWT including
+several claims and signs it using it’s private key. Upon receipt, the
+server verifies the claim to using the public key to ensure the issuer
+is legitimately who they claim to be.
+
+The claim (issued by the client) includes components: the username of
+the user who is attempting authentication, the current unix timestamp,
+and a randomly generated nonce. For example:
+
+::
+
+    {
+        "username": "guido",
+        "time": 1439216312,
+        "nonce": "1"
+    }
+
+The timestamp must be within ±20 seconds of the server time and the
+nonce must be unique within the given timestamp and user. In other
+words, if more than one request from a user is made within the same
+second, the nonce must change. Due to these two factors no token is
+usable more than once, thereby preventing replay attacks.
+
+To make an authenticated request, the client must generate a JWT
+following the above format and include it as the HTTP Authorization
+header in the following format:
+
+::
+
+    Authorization: JWT <my_token>
+
+**Important note**: the claim is *not* encrypted, only signed.
+Additionally, the signature only prevents the claim from being tampered
+with or re-used. Every other part of the request is still vulnerable to
+tamper. Therefore, this is not a replacement for using SSL in the
+transport layer.
+
+**Full Documentation**: https://asymmetric-jwt-auth.readthedocs.io
+
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/README.rst` & `asymmetric_jwt_auth-1.0.1b5/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Asymmetric JWT Authentication
 =============================
 
 .. image:: https://img.shields.io/pypi/v/asymmetric_jwt_auth.svg
     :target: https://pypi.python.org/pypi/asymmetric_jwt_auth
 
-.. image:: https://travis-ci.org/crgwbr/asymmetric-jwt-auth.svg
-    :target: https://travis-ci.org/crgwbr/asymmetric-jwt-auth
+.. image:: https://gitlab.com/crgwbr/asymmetric_jwt_auth/badges/master/pipeline.svg
+    :target: https://gitlab.com/crgwbr/asymmetric_jwt_auth/-/commits/master
+
+.. image:: https://gitlab.com/crgwbr/asymmetric_jwt_auth/badges/master/coverage.svg
+    :target: https://gitlab.com/crgwbr/asymmetric_jwt_auth/-/commits/master
 
 
 What?
 -----
 
 This is an library designed to handle authentication in
 *server-to-server* API requests. It accomplishes this using RSA public /
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/__init__.py` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,29 @@
 from django.conf import settings
 import copy
 
-default_app_config = 'asymmetric_jwt_auth.apps.JWTAuthConfig'
-
 #: Default settings. Override using a dictionary named ASYMMETRIC_JWT_AUTH in Django's settings.py.
 default_settings = {
     #: Auth method searched for in the prefix of the Authentication header. Similar to ``Bearer`` or ``Basic``.
-    'AUTH_METHOD': 'JWT',
-
+    "AUTH_METHOD": "JWT",
     #: Number of seconds of clock-drift to tolerate when verifying the authenticity of a JWT.
-    'TIMESTAMP_TOLERANCE': 20,  # Seconds
-
+    "TIMESTAMP_TOLERANCE": 20,  # Seconds
     #: Class used to store and validate nonces
-    'NONCE_BACKEND': 'asymmetric_jwt_auth.nonce.django.DjangoCacheNonceBackend',
-
+    "NONCE_BACKEND": "asymmetric_jwt_auth.nonce.django.DjangoCacheNonceBackend",
     #: Repository class used to fetch users by their username
-    'USER_REPOSITORY': 'asymmetric_jwt_auth.repos.django.DjangoUserRepository',
-
+    "USER_REPOSITORY": "asymmetric_jwt_auth.repos.django.DjangoUserRepository",
     #: List of repository classes used to fetch public keys for a user
-    'PUBLIC_KEY_REPOSITORIES': [
-        'asymmetric_jwt_auth.repos.django.DjangoPublicKeyListRepository',
-        'asymmetric_jwt_auth.repos.django.DjangoJWKSRepository',
+    "PUBLIC_KEY_REPOSITORIES": [
+        "asymmetric_jwt_auth.repos.django.DjangoPublicKeyListRepository",
+        "asymmetric_jwt_auth.repos.django.DjangoJWKSRepository",
     ],
-
     #: List of public keys that should be advertised on our JWKS endpoint.
-    'SIGNING_PUBLIC_KEYS': [],
-
+    "SIGNING_PUBLIC_KEYS": [],
     #: Cache TTL for the JWKS key view
-    'JWKS_VIEW_TTL': (60 * 5),
+    "JWKS_VIEW_TTL": (60 * 5),
 }
 
 
 def get_setting(name: str):
     _settings = copy.deepcopy(default_settings)
-    _settings.update(getattr(settings, 'ASYMMETRIC_JWT_AUTH', {}))
+    _settings.update(getattr(settings, "ASYMMETRIC_JWT_AUTH", {}))
     return _settings[name]
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/keys.py` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/keys.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,109 +8,102 @@
 
 CryptoPrivateKey = Union[rsa.RSAPrivateKey, ed25519.Ed25519PrivateKey]
 CryptoPublicKey = Union[rsa.RSAPublicKey, ed25519.Ed25519PublicKey]
 
 FacadePrivateKey = Union["RSAPrivateKey", "Ed25519PrivateKey"]
 FacadePublicKey = Union["RSAPublicKey", "Ed25519PublicKey"]
 
-PrivateKeyType = TypeVar('PrivateKeyType', rsa.RSAPrivateKey, ed25519.Ed25519PrivateKey)
-PublicKeyType = TypeVar('PublicKeyType', rsa.RSAPublicKey, ed25519.Ed25519PublicKey)
-
+PrivateKeyType = TypeVar("PrivateKeyType", rsa.RSAPrivateKey, ed25519.Ed25519PrivateKey)
+PublicKeyType = TypeVar("PublicKeyType", rsa.RSAPublicKey, ed25519.Ed25519PublicKey)
 
 
 class PublicKey(Generic[PublicKeyType]):
     """Represents a public key"""
 
     _key: PublicKeyType
 
-
     @staticmethod
     def from_cryptography_pubkey(pubkey: CryptoPublicKey) -> FacadePublicKey:
         if isinstance(pubkey, rsa.RSAPublicKey):
             return RSAPublicKey(pubkey)
         if isinstance(pubkey, ed25519.Ed25519PublicKey):
             return Ed25519PublicKey(pubkey)
-        raise TypeError(f'Unknown key type: {pubkey}')
-
+        raise TypeError(f"Unknown key type: {pubkey}")
 
     @classmethod
     def load_pem(cls, pem: bytes) -> FacadePublicKey:
         """
         Load a PEM-format public key
         """
         privkey = serialization.load_pem_public_key(pem)
         return cls.from_cryptography_pubkey(privkey)
 
-
     @classmethod
     def load_openssh(cls, key: bytes) -> FacadePublicKey:
         """
         Load a openssh-format public key
         """
         privkey = serialization.load_ssh_public_key(key)
         return cls.from_cryptography_pubkey(privkey)
 
-
     @classmethod
-    def load_serialized_public_key(cls, key: bytes) -> Tuple[Optional[Exception], Optional[FacadePublicKey]]:
+    def load_serialized_public_key(
+        cls, key: bytes
+    ) -> Tuple[Optional[Exception], Optional[FacadePublicKey]]:
         """
         Load a PEM or openssh format public key
         """
         exc = None
         for loader in (cls.load_pem, cls.load_openssh):
             try:
                 return None, loader(key)
             except Exception as e:
                 exc = e
         return exc, None
 
-
     @property
     def as_pem(self) -> bytes:
         """
         Get the public key as a PEM-formatted byte string
         """
         pem_bytes = self._key.public_bytes(
-            serialization.Encoding.PEM,
-            serialization.PublicFormat.SubjectPublicKeyInfo)
+            serialization.Encoding.PEM, serialization.PublicFormat.SubjectPublicKeyInfo
+        )
         return pem_bytes
 
-
     @property
     def as_jwk(self) -> dict:  # pragma: no cover
         """
         Return the public key in JWK format
         """
         raise NotImplementedError("Subclass does not implement as_jwk method")
 
-
     @property
     def fingerprint(self) -> str:
         """
         Get a sha256 fingerprint of the key.
         """
         return hashlib.sha256(self.as_pem).hexdigest()
 
-
     @property
     def allowed_algorithms(self) -> List[str]:  # pragma: no cover
         """
         Return a list of allowed JWT algorithms for this key, in order of most to least preferred.
         """
-        raise NotImplementedError("Subclass does not implement allowed_algorithms method")
-
+        raise NotImplementedError(
+            "Subclass does not implement allowed_algorithms method"
+        )
 
 
 class RSAPublicKey(PublicKey):
     """Represents an RSA public key"""
 
     def __init__(self, key: rsa.RSAPublicKey):
         self._key = key
 
-
     @property
     def as_jwk(self) -> dict:
         """
         Return the public key in JWK format
         """
         public_numbers = self._key.public_numbers()
         return {
@@ -118,131 +111,121 @@
             "use": "sig",
             "alg": self.allowed_algorithms[0],
             "kid": self.fingerprint,
             "n": long_to_base64(public_numbers.n),
             "e": long_to_base64(public_numbers.e),
         }
 
-
     @property
     def allowed_algorithms(self) -> List[str]:
         return [
-            'RS512',
-            'RS384',
-            'RS256',
+            "RS512",
+            "RS384",
+            "RS256",
         ]
 
 
 class Ed25519PublicKey(PublicKey):
     """Represents an Ed25519 public key"""
 
     def __init__(self, key: ed25519.Ed25519PublicKey):
         self._key = key
 
-
     @property
     def allowed_algorithms(self) -> List[str]:
         return [
-            'EdDSA',
+            "EdDSA",
         ]
 
 
-
 class PrivateKey(Generic[PrivateKeyType]):
     """Represents a private key"""
 
     _key: PrivateKeyType
 
-
     @staticmethod
     def from_cryptography_privkey(privkey: CryptoPrivateKey) -> FacadePrivateKey:
         if isinstance(privkey, rsa.RSAPrivateKey):
             return RSAPrivateKey(privkey)
         if isinstance(privkey, ed25519.Ed25519PrivateKey):
             return Ed25519PrivateKey(privkey)
-        raise TypeError('Unknown key type')
-
+        raise TypeError("Unknown key type")
 
     @classmethod
-    def load_pem_from_file(cls, filepath: os.PathLike, password: Optional[bytes] = None) -> FacadePrivateKey:
+    def load_pem_from_file(
+        cls, filepath: os.PathLike, password: Optional[bytes] = None
+    ) -> FacadePrivateKey:
         """
         Load a PEM-format private key from disk.
         """
-        with open(filepath, 'rb') as fh:
+        with open(filepath, "rb") as fh:
             key_bytes = fh.read()
         return cls.load_pem(key_bytes, password=password)
 
-
     @classmethod
     def load_pem(cls, pem: bytes, password: Optional[bytes] = None) -> FacadePrivateKey:
         """
         Load a PEM-format private key
         """
-        privkey = serialization.load_pem_private_key(pem,
-            password=password)
+        privkey = serialization.load_pem_private_key(pem, password=password)
         return cls.from_cryptography_privkey(privkey)
 
-
     @property
     def as_pem(self):
         pem_bytes = self._key.private_bytes(
             serialization.Encoding.PEM,
             serialization.PrivateFormat.PKCS8,
-            serialization.NoEncryption())
+            serialization.NoEncryption(),
+        )
         return pem_bytes
 
-
     @property
     def public_key(self) -> FacadePublicKey:  # pragma: no cover
         raise NotImplementedError()
 
 
-
 class RSAPrivateKey(PrivateKey[rsa.RSAPrivateKey]):
     """Represents an RSA private key"""
 
     pubkey_cls = RSAPublicKey
 
     @classmethod
-    def generate(cls, size: int = 2048, public_exponent: int = 65537) -> "RSAPrivateKey":
+    def generate(
+        cls, size: int = 2048, public_exponent: int = 65537
+    ) -> "RSAPrivateKey":
         """
         Generate an RSA private key.
         """
         private = rsa.generate_private_key(
-            public_exponent=public_exponent,
-            key_size=size)
+            public_exponent=public_exponent, key_size=size
+        )
         return cls(private)
 
-
     def __init__(self, key: rsa.RSAPrivateKey):
         self._key = key
 
-
     @property
     def public_key(self) -> FacadePublicKey:
         public = self._key.public_key()
         return self.pubkey_cls(public)
 
 
-
 class Ed25519PrivateKey(PrivateKey[ed25519.Ed25519PrivateKey]):
     """Represents an Ed25519 private key"""
 
     pubkey_cls = Ed25519PublicKey
 
     @classmethod
     def generate(cls) -> "Ed25519PrivateKey":
         """
         Generate an Ed25519 private key.
         """
         private = ed25519.Ed25519PrivateKey.generate()
         return cls(private)
 
-
     def __init__(self, key: ed25519.Ed25519PrivateKey):
         self._key = key
 
-
     @property
     def public_key(self) -> FacadePublicKey:
         public = self._key.public_key()
         return self.pubkey_cls(public)
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/management/commands/generate_key_pair.py` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/management/commands/generate_key_pair.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from django.core.management.base import BaseCommand
 from asymmetric_jwt_auth.keys import (
     RSAPrivateKey,
     Ed25519PrivateKey,
 )
 
-TYPE_RSA = 'RSA'
-TYPE_ED25519 = 'Ed25519'
+TYPE_RSA = "RSA"
+TYPE_ED25519 = "Ed25519"
 TYPE_CHOICES = [
     TYPE_RSA,
     TYPE_ED25519,
 ]
 
 
 class Command(BaseCommand):
     help = "Generate a public / private RSA key pair"
 
     def add_arguments(self, parser):
-        parser.add_argument('-t', '--keytype',
-            choices=TYPE_CHOICES,
-            default=TYPE_RSA)
+        parser.add_argument("-t", "--keytype", choices=TYPE_CHOICES, default=TYPE_RSA)
 
     def handle(self, *args, keytype=TYPE_RSA, **options):
         if keytype == TYPE_ED25519:
             privkey = Ed25519PrivateKey.generate()
         else:
             privkey = RSAPrivateKey.generate()
         self.stdout.write(privkey.as_pem.decode())
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/middleware.py` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,43 +14,41 @@
 
     def __init__(self, get_response: Callable[[HttpRequest], HttpResponse]):
         self.get_response = get_response
         self.nonce_backend = get_nonce_backend()
         self.user_repo = get_user_repository()
         self.key_repos = get_public_key_repositories()
 
-
     def __call__(self, request: HttpRequest) -> HttpResponse:
         # Attempt to authorize the request
         self.authorize_request(request)
         # Continue with the request
         return self.get_response(request)
 
-
     def authorize_request(self, request: HttpRequest) -> HttpRequest:
         """
         Process a Django request and authenticate users.
 
         If a JWT authentication header is detected and it is determined to be valid, the user is set as
         ``request.user`` and CSRF protection is disabled (``request._dont_enforce_csrf_checks = True``) on
         the request.
 
         :param request: Django Request instance
         """
         # Check for presence of auth header
-        if 'HTTP_AUTHORIZATION' not in request.META:
+        if "HTTP_AUTHORIZATION" not in request.META:
             return request
 
         # Ensure this auth header was meant for us (it has the JWT auth method).
         try:
-            method, header_data = request.META['HTTP_AUTHORIZATION'].split(' ', 1)
+            method, header_data = request.META["HTTP_AUTHORIZATION"].split(" ", 1)
         except ValueError:
             return request
 
-        auth_method_setting = get_setting('AUTH_METHOD')
+        auth_method_setting = get_setting("AUTH_METHOD")
         if method.upper() != auth_method_setting:
             return request
 
         # Get the (unvalidated!) username that the request is claiming to be
         untrusted_token = UntrustedToken(header_data)
         username = untrusted_token.get_claimed_username()
         if not username:
@@ -69,11 +67,11 @@
                 break
 
         # No keys successfully validated the claim? Abort.
         if not verified_token:
             return request
 
         # Assign the user to the request
-        logger.debug('Successfully authenticated %s using JWT', user.username)
+        logger.debug("Successfully authenticated %s using JWT", user.username)
         request._dont_enforce_csrf_checks = True
         request.user = user
         return request
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/migrations/0001_initial.py` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/migrations/0002_publickey_comment.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
 
-from django.db import models, migrations
-from django.conf import settings
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
+        ("asymmetric_jwt_auth", "0001_initial"),
     ]
 
     operations = [
-        migrations.CreateModel(
-            name='PublicKey',
-            fields=[
-                ('id', models.AutoField(serialize=False, auto_created=True, verbose_name='ID', primary_key=True)),
-                ('key', models.TextField(help_text="The user's RSA public key")),
-                ('user', models.ForeignKey(to=settings.AUTH_USER_MODEL, related_name='public_keys', on_delete=models.CASCADE)),
-            ],
+        migrations.AddField(
+            model_name="publickey",
+            name="comment",
+            field=models.CharField(
+                max_length=100, help_text="Comment describing this key", default=""
+            ),
+            preserve_default=False,
         ),
     ]
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/migrations/0004_auto_20191104_1628.py` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/migrations/0004_auto_20191104_1628.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 # Generated by Django 2.2.5 on 2019-11-04 16:28
 
 import asymmetric_jwt_auth.models
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ('asymmetric_jwt_auth', '0003_auto_20151112_1547'),
+        ("asymmetric_jwt_auth", "0003_auto_20151112_1547"),
     ]
 
     operations = [
         migrations.AddField(
-            model_name='publickey',
-            name='last_used_on',
-            field=models.DateTimeField(blank=True, null=True, verbose_name='Last Used On'),
+            model_name="publickey",
+            name="last_used_on",
+            field=models.DateTimeField(
+                blank=True, null=True, verbose_name="Last Used On"
+            ),
         ),
         migrations.AlterField(
-            model_name='publickey',
-            name='key',
-            field=models.TextField(help_text="The user's RSA public key", validators=[asymmetric_jwt_auth.models.validate_public_key]),
+            model_name="publickey",
+            name="key",
+            field=models.TextField(
+                help_text="The user's RSA public key",
+                validators=[asymmetric_jwt_auth.models.validate_public_key],
+            ),
         ),
     ]
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/migrations/0005_auto_20210304_1116.py` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/migrations/0005_auto_20210304_1116.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,46 +3,84 @@
 import asymmetric_jwt_auth.models
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
-        ('asymmetric_jwt_auth', '0004_auto_20191104_1628'),
+        ("asymmetric_jwt_auth", "0004_auto_20191104_1628"),
     ]
 
     operations = [
         migrations.AlterModelOptions(
-            name='publickey',
-            options={'verbose_name': 'Public Key', 'verbose_name_plural': 'Public Keys'},
+            name="publickey",
+            options={
+                "verbose_name": "Public Key",
+                "verbose_name_plural": "Public Keys",
+            },
         ),
         migrations.AlterField(
-            model_name='publickey',
-            name='comment',
-            field=models.CharField(blank=True, help_text='Comment describing this key', max_length=100, verbose_name='Comment'),
+            model_name="publickey",
+            name="comment",
+            field=models.CharField(
+                blank=True,
+                help_text="Comment describing this key",
+                max_length=100,
+                verbose_name="Comment",
+            ),
         ),
         migrations.AlterField(
-            model_name='publickey',
-            name='key',
-            field=models.TextField(help_text="The user's RSA public key", validators=[asymmetric_jwt_auth.models.validate_public_key], verbose_name='Public Key'),
+            model_name="publickey",
+            name="key",
+            field=models.TextField(
+                help_text="The user's RSA public key",
+                validators=[asymmetric_jwt_auth.models.validate_public_key],
+                verbose_name="Public Key",
+            ),
         ),
         migrations.AlterField(
-            model_name='publickey',
-            name='user',
-            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='public_keys', to=settings.AUTH_USER_MODEL, verbose_name='User'),
+            model_name="publickey",
+            name="user",
+            field=models.ForeignKey(
+                on_delete=django.db.models.deletion.CASCADE,
+                related_name="public_keys",
+                to=settings.AUTH_USER_MODEL,
+                verbose_name="User",
+            ),
         ),
         migrations.CreateModel(
-            name='JWKSEndpointTrust',
+            name="JWKSEndpointTrust",
             fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('jwks_url', models.URLField(help_text='e.g. https://dev-87evx9ru.auth0.com/.well-known/jwks.json', verbose_name='JSON Web Key Set (JWKS) URL')),
-                ('user', models.OneToOneField(on_delete=django.db.models.deletion.CASCADE, related_name='jwks_endpoint', to=settings.AUTH_USER_MODEL, verbose_name='User')),
+                (
+                    "id",
+                    models.AutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                (
+                    "jwks_url",
+                    models.URLField(
+                        help_text="e.g. https://dev-87evx9ru.auth0.com/.well-known/jwks.json",
+                        verbose_name="JSON Web Key Set (JWKS) URL",
+                    ),
+                ),
+                (
+                    "user",
+                    models.OneToOneField(
+                        on_delete=django.db.models.deletion.CASCADE,
+                        related_name="jwks_endpoint",
+                        to=settings.AUTH_USER_MODEL,
+                        verbose_name="User",
+                    ),
+                ),
             ],
             options={
-                'verbose_name': 'JSON Web Key Set',
-                'verbose_name_plural': 'JSON Web Key Sets',
+                "verbose_name": "JSON Web Key Set",
+                "verbose_name_plural": "JSON Web Key Sets",
             },
         ),
     ]
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/models.py` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,110 +4,110 @@
 from django.core.exceptions import ValidationError
 from django.utils.translation import gettext_lazy as _
 from django.utils.encoding import force_str, force_bytes
 from jwt import PyJWKClient
 from . import keys, tokens
 
 
-
 def validate_public_key(keystr: str) -> None:
     """
     Check that the given value is a valid public key in either PEM or OpenSSH format. If it is invalid,
     raises ``django.core.exceptions.ValidationError``.
     """
     key_bytes = keystr.encode()
     exc, key = keys.PublicKey.load_serialized_public_key(key_bytes)
     is_valid = (exc is None) and (key is not None)
     if not is_valid:
-        raise ValidationError('Public key is invalid: %s' % exc)
-
+        raise ValidationError("Public key is invalid: %s" % exc)
 
 
 class PublicKey(models.Model):
     """
     Store a public key and associate it to a particular user.
 
     Implements the same concept as the OpenSSH ``~/.ssh/authorized_keys`` file on a Unix system.
     """
 
     #: Foreign key to the Django User model. Related name: ``public_keys``.
-    user = models.ForeignKey(settings.AUTH_USER_MODEL,
+    user = models.ForeignKey(
+        settings.AUTH_USER_MODEL,
         verbose_name=_("User"),
-        related_name='public_keys',
-        on_delete=models.CASCADE)
+        related_name="public_keys",
+        on_delete=models.CASCADE,
+    )
 
     #: Key text in either PEM or OpenSSH format.
-    key = models.TextField(_("Public Key"),
+    key = models.TextField(
+        _("Public Key"),
         help_text=_("The user's RSA/Ed25519 public key"),
-        validators=[validate_public_key])
+        validators=[validate_public_key],
+    )
 
     #: Comment describing the key. Use this to note what system is authenticating with the key, when it was last rotated, etc.
-    comment = models.CharField(_("Comment"),
+    comment = models.CharField(
+        _("Comment"),
         max_length=100,
         help_text=_("Comment describing this key"),
-        blank=True)
+        blank=True,
+    )
 
     #: Date and time that key was last used for authenticating a request.
-    last_used_on = models.DateTimeField(_("Last Used On"),
-        null=True,
-        blank=True)
+    last_used_on = models.DateTimeField(_("Last Used On"), null=True, blank=True)
 
     class Meta:
         verbose_name = _("Public Key")
         verbose_name_plural = _("Public Keys")
 
-
     def get_key(self) -> keys.FacadePublicKey:
         key_bytes = force_bytes(self.key)
         exc, key = keys.PublicKey.load_serialized_public_key(key_bytes)
         if key is None:
             if exc is None:  # pragma: no cover
                 raise ValueError("Failed to load key")
             raise exc
         return key
 
-
     def update_last_used_datetime(self) -> None:
         self.last_used_on = timezone.now()
         self.save(update_fields=["last_used_on"])
 
-
     def save(self, *args, **kwargs) -> None:
-        key_parts = force_str(self.key).split(' ')
+        key_parts = force_str(self.key).split(" ")
         if len(key_parts) == 3 and not self.comment:
             self.comment = key_parts.pop()
         super(PublicKey, self).save(*args, **kwargs)
 
 
-
 class JWKSEndpointTrust(models.Model):
     """
     Associate a JSON Web Key Set (JWKS) URL with a Django User.
 
     This accomplishes the same purpose of the PublicKey model, in a more automated
     fashion. Instead of manually assigning a public key to a user, the system will
     load a list of public keys from this URL.
     """
 
     #: Foreign key to the Django User model. Related name: ``public_keys``.
-    user = models.OneToOneField(settings.AUTH_USER_MODEL,
+    user = models.OneToOneField(
+        settings.AUTH_USER_MODEL,
         verbose_name=_("User"),
-        related_name='jwks_endpoint',
-        on_delete=models.CASCADE)
+        related_name="jwks_endpoint",
+        on_delete=models.CASCADE,
+    )
 
     #: URL of the JSON Web Key Set (JWKS)
-    jwks_url = models.URLField(_("JSON Web Key Set (JWKS) URL"),
-        help_text=_("e.g. https://dev-87evx9ru.auth0.com/.well-known/jwks.json"))
+    jwks_url = models.URLField(
+        _("JSON Web Key Set (JWKS) URL"),
+        help_text=_("e.g. https://dev-87evx9ru.auth0.com/.well-known/jwks.json"),
+    )
 
     class Meta:
         verbose_name = _("JSON Web Key Set")
         verbose_name_plural = _("JSON Web Key Sets")
 
-
     @property
     def jwks_client(self) -> PyJWKClient:
         return PyJWKClient(self.jwks_url)
 
-
     def get_signing_key(self, untrusted_token: tokens.UntrustedToken) -> keys.PublicKey:
         jwk = self.jwks_client.get_signing_key_from_jwt(untrusted_token.token)
         return keys.PublicKey.from_cryptography_pubkey(jwk.key)
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/nonce/django.py` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/nonce/django.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,28 +15,28 @@
         """
         Confirm that the given nonce hasn't already been used.
         """
         key = self._create_nonce_key(username, timestamp)
         used = cache.get(key, set([]))
         return nonce not in used
 
-
     def log_used_nonce(self, username: str, timestamp: int, nonce: str) -> None:
         """
         Log a nonce as being used, and therefore henceforth invalid.
         """
         key = self._create_nonce_key(username, timestamp)
         used = cache.get(key, set([]))
         used.add(nonce)
-        timestamp_tolerance = getattr(settings, 'ASYMMETRIC_JWT_AUTH', default_settings)['TIMESTAMP_TOLERANCE']
+        timestamp_tolerance = getattr(
+            settings, "ASYMMETRIC_JWT_AUTH", default_settings
+        )["TIMESTAMP_TOLERANCE"]
         cache.set(key, used, timestamp_tolerance * 2)
 
-
     def _create_nonce_key(self, username: str, timestamp: int) -> str:
         """
         Create and return the cache key for storing nonces
         """
-        return '%s-nonces-%s-%s' % (
+        return "%s-nonces-%s-%s" % (
             self.__class__.__name__,
             username,
             timestamp,
         )
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/nonce/null.py` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/nonce/null.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,13 +8,12 @@
 
     def validate_nonce(self, username: str, timestamp: int, nonce: str) -> bool:
         """
         Confirm that the given nonce hasn't already been used.
         """
         return True
 
-
     def log_used_nonce(self, username: str, timestamp: int, nonce: str) -> None:
         """
         Log a nonce as being used, and therefore henceforth invalid.
         """
         pass
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/repos/__init__.py` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/repos/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import List
 from django.utils.module_loading import import_string
 from .. import get_setting
 from .base import BaseUserRepository, BasePublicKeyRepository
 
 
 def get_user_repository() -> BaseUserRepository:
-    Repo = import_string(get_setting('USER_REPOSITORY'))
+    Repo = import_string(get_setting("USER_REPOSITORY"))
     return Repo()
 
 
 def get_public_key_repositories() -> List[BasePublicKeyRepository]:
     repos = []
-    for cls_path in get_setting('PUBLIC_KEY_REPOSITORIES'):
+    for cls_path in get_setting("PUBLIC_KEY_REPOSITORIES"):
         Repo = import_string(cls_path)
         repo = Repo()
         repos.append(repo)
     return repos
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/repos/django.py` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/repos/django.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from django.contrib.auth.models import User
 from jwt.exceptions import PyJWKClientError
 from .base import BaseUserRepository, BasePublicKeyRepository
 from ..tokens import UntrustedToken, Token
 from .. import models
 
 
-
 class DjangoUserRepository(BaseUserRepository):
     def __init__(self):
         self.User = get_user_model()
 
     def get_user(self, username: str) -> Union[None, User]:
         """
         Get a Django user by username
@@ -19,41 +18,41 @@
         try:
             return self.User.objects.get(username=username)
         except self.User.DoesNotExist:
             pass
         return None
 
 
-
 class DjangoPublicKeyListRepository(BasePublicKeyRepository):
-    def attempt_to_verify_token(self, user: User, untrusted_token: UntrustedToken) -> Union[Token, None]:
+    def attempt_to_verify_token(
+        self, user: User, untrusted_token: UntrustedToken
+    ) -> Union[Token, None]:
         """
         Attempt to verify a JWT for the given user using public keys from the PublicKey model.
         """
         for user_key in models.PublicKey.objects.filter(user=user).all():
             public_key = user_key.get_key()
-            token = untrusted_token.verify(
-                public_key=public_key)
+            token = untrusted_token.verify(public_key=public_key)
             if token:
                 user_key.update_last_used_datetime()
                 return token
         return None
 
 
-
 class DjangoJWKSRepository(BasePublicKeyRepository):
-    def attempt_to_verify_token(self, user: User, untrusted_token: UntrustedToken) -> Union[Token, None]:
+    def attempt_to_verify_token(
+        self, user: User, untrusted_token: UntrustedToken
+    ) -> Union[Token, None]:
         """
         Attempt to verify a JWT for the given user using public keys the user's JWKS endpoint.
         """
         jwks_endpoint = models.JWKSEndpointTrust.objects.filter(user=user).first()
         if not jwks_endpoint:
             return None
         try:
             public_key = jwks_endpoint.get_signing_key(untrusted_token)
         except PyJWKClientError:
             return None
-        token = untrusted_token.verify(
-            public_key=public_key)
+        token = untrusted_token.verify(public_key=public_key)
         if token:
             return token
         return None
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/data.py` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/data.py`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa.privkey` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa.privkey`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa_encrypted.privkey` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/fixtures/dummy_rsa_encrypted.privkey`

 * *Files identical despite different names*

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/test_commands.py` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_commands.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,33 +3,29 @@
 from django.core.management import call_command
 
 
 class ManagementCommandTest(TestCase):
     def test_generate_new_rsa_key(self):
         stdout = StringIO()
         stderr = StringIO()
-        call_command('generate_key_pair',
-            stdout=stdout,
-            stderr=stderr)
+        call_command("generate_key_pair", stdout=stdout, stderr=stderr)
         out = stdout.getvalue()
         self.assertIn("-----BEGIN PRIVATE KEY-----\n", out)
         self.assertIn("-----END PRIVATE KEY-----\n", out)
         self.assertIn("-----BEGIN PUBLIC KEY-----\n", out)
         self.assertIn("-----END PUBLIC KEY-----\n", out)
         self.assertTrue(len(out) > 2000)
         self.assertTrue(len(out) < 3000)
 
-
     def test_generate_new_ed25519_key(self):
         stdout = StringIO()
         stderr = StringIO()
-        call_command('generate_key_pair',
-            keytype='Ed25519',
-            stdout=stdout,
-            stderr=stderr)
+        call_command(
+            "generate_key_pair", keytype="Ed25519", stdout=stdout, stderr=stderr
+        )
         out = stdout.getvalue()
         self.assertIn("-----BEGIN PRIVATE KEY-----\n", out)
         self.assertIn("-----END PRIVATE KEY-----\n", out)
         self.assertIn("-----BEGIN PUBLIC KEY-----\n", out)
         self.assertIn("-----END PUBLIC KEY-----\n", out)
         self.assertTrue(len(out) > 200)
         self.assertTrue(len(out) < 300)
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/test_keys.py` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_keys.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,159 +7,153 @@
 
 class PublicKeyTest(TestCase):
     def test_load_pem_rsa(self):
         exc, key = keys.PublicKey.load_serialized_public_key(data.PEM_PUBLIC_RSA)
         self.assertIsNone(exc)
         self.assertIsInstance(key, keys.RSAPublicKey)
 
-
     def test_load_pem_ed25519(self):
         exc, key = keys.PublicKey.load_serialized_public_key(data.PEM_PUBLIC_ED25519)
         self.assertIsNone(exc)
         self.assertIsInstance(key, keys.Ed25519PublicKey)
 
-
     def test_load_openssh_rsa(self):
         exc, key = keys.PublicKey.load_serialized_public_key(data.OPENSSH_RSA)
         self.assertIsNone(exc)
         self.assertIsInstance(key, keys.RSAPublicKey)
 
-
     def test_load_openssh_ed25519(self):
         exc, key = keys.PublicKey.load_serialized_public_key(data.OPENSSH_ED25519)
         self.assertIsNone(exc)
         self.assertIsInstance(key, keys.Ed25519PublicKey)
 
-
     def test_load_invalid_pem_rsa(self):
-        exc, key = keys.PublicKey.load_serialized_public_key(data.PEM_PUBLIC_RSA_INVALID)
+        exc, key = keys.PublicKey.load_serialized_public_key(
+            data.PEM_PUBLIC_RSA_INVALID
+        )
         self.assertIsInstance(exc, Exception)
         self.assertIsNone(key)
 
-
     def test_load_invalid_pem_ed25519(self):
-        exc, key = keys.PublicKey.load_serialized_public_key(data.PEM_PUBLIC_ED25519_INVALID)
+        exc, key = keys.PublicKey.load_serialized_public_key(
+            data.PEM_PUBLIC_ED25519_INVALID
+        )
         self.assertIsInstance(exc, Exception)
         self.assertIsNone(key)
 
-
     def test_load_invalid_openssh_rsa(self):
         exc, key = keys.PublicKey.load_serialized_public_key(data.OPENSSH_RSA_INVALID)
         self.assertIsInstance(exc, Exception)
         self.assertIsNone(key)
 
-
     def test_load_invalid_openssh_ed25519(self):
-        exc, key = keys.PublicKey.load_serialized_public_key(data.OPENSSH_ED25519_INVALID)
+        exc, key = keys.PublicKey.load_serialized_public_key(
+            data.OPENSSH_ED25519_INVALID
+        )
         self.assertIsInstance(exc, Exception)
         self.assertIsNone(key)
 
-
     def test_rsa_as_pem(self):
         exc, key = keys.PublicKey.load_serialized_public_key(data.PEM_PUBLIC_RSA)
         self.assertIsNone(exc)
-        pem = key.as_pem.decode().strip().split('\n')
-        self.assertEqual(pem[0], '-----BEGIN PUBLIC KEY-----')
-        self.assertEqual(pem[-1], '-----END PUBLIC KEY-----')
-
+        pem = key.as_pem.decode().strip().split("\n")
+        self.assertEqual(pem[0], "-----BEGIN PUBLIC KEY-----")
+        self.assertEqual(pem[-1], "-----END PUBLIC KEY-----")
 
     def test_ed25519_as_pem(self):
         exc, key = keys.PublicKey.load_serialized_public_key(data.PEM_PUBLIC_RSA)
         self.assertIsNone(exc)
-        pem = key.as_pem.decode().strip().split('\n')
-        self.assertEqual(pem[0], '-----BEGIN PUBLIC KEY-----')
-        self.assertEqual(pem[-1], '-----END PUBLIC KEY-----')
-
+        pem = key.as_pem.decode().strip().split("\n")
+        self.assertEqual(pem[0], "-----BEGIN PUBLIC KEY-----")
+        self.assertEqual(pem[-1], "-----END PUBLIC KEY-----")
 
     def test_rsa_fingerprint(self):
         exc, key = keys.PublicKey.load_serialized_public_key(data.PEM_PUBLIC_RSA)
         self.assertIsNone(exc)
-        self.assertEqual(key.fingerprint, '53c5b68c5ecba3e25df3f8326de6c0b0befb67e9217651a2f40e388f6567f056')
-
+        self.assertEqual(
+            key.fingerprint,
+            "53c5b68c5ecba3e25df3f8326de6c0b0befb67e9217651a2f40e388f6567f056",
+        )
 
     def test_ed25519_fingerprint(self):
         exc, key = keys.PublicKey.load_serialized_public_key(data.PEM_PUBLIC_ED25519)
         self.assertIsNone(exc)
-        self.assertEqual(key.fingerprint, 'cb10cd75c2eacf7aa2b5195bef9838cccd9d2ae4938601178808cb881b68ec72')
-
+        self.assertEqual(
+            key.fingerprint,
+            "cb10cd75c2eacf7aa2b5195bef9838cccd9d2ae4938601178808cb881b68ec72",
+        )
 
     def test_rsa_allowed_algorithms(self):
         exc, key = keys.PublicKey.load_serialized_public_key(data.PEM_PUBLIC_RSA)
         self.assertIsNone(exc)
-        self.assertEqual(key.allowed_algorithms, [
-            'RS512',
-            'RS384',
-            'RS256',
-        ])
-
+        self.assertEqual(
+            key.allowed_algorithms,
+            [
+                "RS512",
+                "RS384",
+                "RS256",
+            ],
+        )
 
     def test_ed25519_allowed_algorithms(self):
         exc, key = keys.PublicKey.load_serialized_public_key(data.PEM_PUBLIC_ED25519)
         self.assertIsNone(exc)
-        self.assertEqual(key.allowed_algorithms, [
-            'EdDSA',
-        ])
-
+        self.assertEqual(
+            key.allowed_algorithms,
+            [
+                "EdDSA",
+            ],
+        )
 
     def test_unknown_key_type(self):
         with self.assertRaises(TypeError):
             keys.PublicKey.from_cryptography_pubkey(mock.MagicMock())
 
 
-
 class PrivateKeyTest(TestCase):
     def test_generate_rsa(self):
         private = keys.RSAPrivateKey.generate()
         self.assertIsInstance(private, keys.RSAPrivateKey)
         self.assertIsInstance(private.public_key, keys.RSAPublicKey)
 
-
     def test_generate_ed25519(self):
         private = keys.Ed25519PrivateKey.generate()
         self.assertIsInstance(private, keys.Ed25519PrivateKey)
         self.assertIsInstance(private.public_key, keys.Ed25519PublicKey)
 
-
     def test_load_rsa_from_file(self):
         base = os.path.dirname(__file__)
-        filepath = os.path.join(base, 'fixtures/dummy_rsa.privkey')
+        filepath = os.path.join(base, "fixtures/dummy_rsa.privkey")
         private = keys.RSAPrivateKey.load_pem_from_file(filepath)
         self.assertIsInstance(private, keys.RSAPrivateKey)
 
-
     def test_load_rsa_from_file_encrypted(self):
         base = os.path.dirname(__file__)
-        filepath = os.path.join(base, 'fixtures/dummy_rsa_encrypted.privkey')
-        private = keys.RSAPrivateKey.load_pem_from_file(filepath,
-            password=b'password')
+        filepath = os.path.join(base, "fixtures/dummy_rsa_encrypted.privkey")
+        private = keys.RSAPrivateKey.load_pem_from_file(filepath, password=b"password")
         self.assertIsInstance(private, keys.RSAPrivateKey)
 
-
     def test_load_rsa(self):
         priv1 = keys.RSAPrivateKey.generate()
         priv2 = keys.RSAPrivateKey.load_pem(priv1.as_pem)
         self.assertEqual(priv2.as_pem, priv1.as_pem)
 
-
     def test_load_ed25519(self):
         priv1 = keys.Ed25519PrivateKey.generate()
         priv2 = keys.Ed25519PrivateKey.load_pem(priv1.as_pem)
         self.assertEqual(priv2.as_pem, priv1.as_pem)
 
-
     def test_rsa_as_pem(self):
         private = keys.RSAPrivateKey.generate()
-        pem = private.as_pem.decode().strip().split('\n')
-        self.assertEqual(pem[0], '-----BEGIN PRIVATE KEY-----')
-        self.assertEqual(pem[-1], '-----END PRIVATE KEY-----')
-
+        pem = private.as_pem.decode().strip().split("\n")
+        self.assertEqual(pem[0], "-----BEGIN PRIVATE KEY-----")
+        self.assertEqual(pem[-1], "-----END PRIVATE KEY-----")
 
     def test_ed25519_as_pem(self):
         private = keys.Ed25519PrivateKey.generate()
-        pem = private.as_pem.decode().strip().split('\n')
-        self.assertEqual(pem[0], '-----BEGIN PRIVATE KEY-----')
-        self.assertEqual(pem[-1], '-----END PRIVATE KEY-----')
-
+        pem = private.as_pem.decode().strip().split("\n")
+        self.assertEqual(pem[0], "-----BEGIN PRIVATE KEY-----")
+        self.assertEqual(pem[-1], "-----END PRIVATE KEY-----")
 
     def test_unknown_key_type(self):
         with self.assertRaises(TypeError):
             keys.PrivateKey.from_cryptography_privkey(mock.MagicMock())
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/test_middleware.py` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_middleware.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,225 +5,201 @@
 from ..middleware import JWTAuthMiddleware
 from ..tokens import Token
 from ..keys import RSAPrivateKey, Ed25519PrivateKey
 
 
 class BaseMiddlewareTest(TestCase):
     def assertNotLoggedIn(self, request):
-        self.assertEqual(getattr(request, 'user', None), None)
-
+        self.assertEqual(getattr(request, "user", None), None)
 
     def assertLoggedIn(self, request, public_key=None):
         if public_key:
             public_key.refresh_from_db()
             self.assertIsNotNone(public_key.last_used_on)
-        self.assertEqual(getattr(request, 'user', None), self.user)
+        self.assertEqual(getattr(request, "user", None), self.user)
 
 
 class MiddlewareTest(BaseMiddlewareTest):
-
     def setUp(self):
         self.rfactory = RequestFactory()
-        self.user = User.objects.create_user(username='foo')
-        self.user2 = User.objects.create_user(username='bar')
+        self.user = User.objects.create_user(username="foo")
+        self.user2 = User.objects.create_user(username="bar")
 
         self.key_ed25519 = Ed25519PrivateKey.generate()
         self.key_rsa = RSAPrivateKey.generate()
 
         self.user_key_ed25519 = PublicKey.objects.create(
-            user=self.user,
-            key=self.key_ed25519.public_key.as_pem.decode())
+            user=self.user, key=self.key_ed25519.public_key.as_pem.decode()
+        )
         self.user_key_rsa = PublicKey.objects.create(
-            user=self.user,
-            key=self.key_rsa.public_key.as_pem.decode())
+            user=self.user, key=self.key_rsa.public_key.as_pem.decode()
+        )
 
         self.next_middleware = mock.MagicMock()
         self.run_middleware = JWTAuthMiddleware(self.next_middleware)
 
-
     def test_no_auth_header(self):
-        request = self.rfactory.get('/')
+        request = self.rfactory.get("/")
         self.assertNotLoggedIn(request)
         self.run_middleware(request)
         self.assertNotLoggedIn(request)
         self.assertEqual(self.next_middleware.call_count, 1)
 
-
     def test_auth_header_missing_type(self):
-        request = self.rfactory.get('/', HTTP_AUTHORIZATION='Fooopbar')
+        request = self.rfactory.get("/", HTTP_AUTHORIZATION="Fooopbar")
         self.assertNotLoggedIn(request)
         self.run_middleware(request)
         self.assertNotLoggedIn(request)
         self.assertEqual(self.next_middleware.call_count, 1)
 
-
     def test_auth_header_not_jwt_type(self):
-        request = self.rfactory.get('/', HTTP_AUTHORIZATION='Bearer foobar')
+        request = self.rfactory.get("/", HTTP_AUTHORIZATION="Bearer foobar")
         self.assertNotLoggedIn(request)
         self.run_middleware(request)
         self.assertNotLoggedIn(request)
         self.assertEqual(self.next_middleware.call_count, 1)
 
-
     def test_header_jwt_missing_username(self):
-        header = Token('').create_auth_header(self.key_rsa)
-        request = self.rfactory.get('/', HTTP_AUTHORIZATION=header)
+        header = Token("").create_auth_header(self.key_rsa)
+        request = self.rfactory.get("/", HTTP_AUTHORIZATION=header)
         self.assertNotLoggedIn(request)
         self.run_middleware(request)
         self.assertNotLoggedIn(request)
         self.assertEqual(self.next_middleware.call_count, 1)
 
-
     def test_header_jwt_claimed_username_doesnt_exist(self):
-        header = Token('rusty').create_auth_header(self.key_rsa)
-        request = self.rfactory.get('/', HTTP_AUTHORIZATION=header)
+        header = Token("rusty").create_auth_header(self.key_rsa)
+        request = self.rfactory.get("/", HTTP_AUTHORIZATION=header)
         self.assertNotLoggedIn(request)
         self.run_middleware(request)
         self.assertNotLoggedIn(request)
         self.assertEqual(self.next_middleware.call_count, 1)
 
-
     def test_authenticate_request_rsa_valid(self):
         header = Token(self.user.username).create_auth_header(self.key_rsa)
-        request = self.rfactory.get('/', HTTP_AUTHORIZATION=header)
+        request = self.rfactory.get("/", HTTP_AUTHORIZATION=header)
         self.assertNotLoggedIn(request)
         self.run_middleware(request)
         self.assertLoggedIn(request, self.user_key_rsa)
         self.assertEqual(self.next_middleware.call_count, 1)
 
-
     def test_authenticate_request_rsa_unregistered_key(self):
         # Assign the pub keys to user 2
         self.user_key_ed25519.user = self.user2
         self.user_key_ed25519.save()
         self.user_key_rsa.user = self.user2
         self.user_key_rsa.save()
         # Try to use user2's key to login as user1
         header = Token(self.user.username).create_auth_header(self.key_rsa)
-        request = self.rfactory.get('/', HTTP_AUTHORIZATION=header)
+        request = self.rfactory.get("/", HTTP_AUTHORIZATION=header)
         self.assertNotLoggedIn(request)
         self.run_middleware(request)
         self.assertNotLoggedIn(request)
         self.assertEqual(self.next_middleware.call_count, 1)
 
-
     def test_authenticate_request_ed25519_valid(self):
         header = Token(self.user.username).create_auth_header(self.key_ed25519)
-        request = self.rfactory.get('/', HTTP_AUTHORIZATION=header)
+        request = self.rfactory.get("/", HTTP_AUTHORIZATION=header)
         self.assertNotLoggedIn(request)
         self.run_middleware(request)
         self.assertLoggedIn(request, self.user_key_ed25519)
         self.assertEqual(self.next_middleware.call_count, 1)
 
-
     def test_missing_data(self):
-        header = Token(self.user.username, timestamp=0).create_auth_header(self.key_ed25519)
-        request = self.rfactory.get('/', HTTP_AUTHORIZATION=header)
+        header = Token(self.user.username, timestamp=0).create_auth_header(
+            self.key_ed25519
+        )
+        request = self.rfactory.get("/", HTTP_AUTHORIZATION=header)
         self.assertNotLoggedIn(request)
         self.run_middleware(request)
         self.assertNotLoggedIn(request)
         self.assertEqual(self.next_middleware.call_count, 1)
 
-
     def test_cant_reuse_nonce(self):
         header = Token(self.user.username).create_auth_header(self.key_ed25519)
         # First use works
-        request1 = self.rfactory.get('/', HTTP_AUTHORIZATION=header)
+        request1 = self.rfactory.get("/", HTTP_AUTHORIZATION=header)
         self.assertNotLoggedIn(request1)
         self.run_middleware(request1)
         self.assertLoggedIn(request1, self.user_key_ed25519)
         self.assertEqual(self.next_middleware.call_count, 1)
         # Second use doesn't
-        request2 = self.rfactory.get('/', HTTP_AUTHORIZATION=header)
+        request2 = self.rfactory.get("/", HTTP_AUTHORIZATION=header)
         self.assertNotLoggedIn(request2)
         self.run_middleware(request2)
         self.assertNotLoggedIn(request2)
         self.assertEqual(self.next_middleware.call_count, 2)
 
 
-
 class MiddlewareJWKSTest(BaseMiddlewareTest):
-
     def setUp(self):
         self.rfactory = RequestFactory()
-        self.user = User.objects.create_user(username='foo')
+        self.user = User.objects.create_user(username="foo")
 
         self.key_ed25519 = Ed25519PrivateKey.generate()
         self.key_rsa = RSAPrivateKey.generate()
 
         self.next_middleware = mock.MagicMock()
         self.run_middleware = JWTAuthMiddleware(self.next_middleware)
 
-
-    @mock.patch('asymmetric_jwt_auth.models.PyJWKClient.fetch_data')
+    @mock.patch("asymmetric_jwt_auth.models.PyJWKClient.fetch_data")
     def test_authenticate_request_rsa(self, mock_fetch_data):
         mock_fetch_data.return_value = {
             "keys": [
                 self.key_rsa.public_key.as_jwk,
             ],
         }
-        JWKSEndpointTrust.objects.create(
-            user=self.user,
-            jwks_url='')
+        JWKSEndpointTrust.objects.create(user=self.user, jwks_url="")
         header = Token(self.user.username).create_auth_header(self.key_rsa)
-        request = self.rfactory.get('/', HTTP_AUTHORIZATION=header)
+        request = self.rfactory.get("/", HTTP_AUTHORIZATION=header)
         self.assertNotLoggedIn(request)
         self.run_middleware(request)
         self.assertLoggedIn(request)
         self.assertEqual(self.next_middleware.call_count, 1)
 
-
-    @mock.patch('asymmetric_jwt_auth.models.PyJWKClient.fetch_data')
+    @mock.patch("asymmetric_jwt_auth.models.PyJWKClient.fetch_data")
     def test_no_matching_key(self, mock_fetch_data):
         # Change the key ID of the JWKS response so it doesn't match the kid in the header JWT
         jwk = self.key_rsa.public_key.as_jwk
-        jwk['kid'] = 'foobar'
+        jwk["kid"] = "foobar"
         mock_fetch_data.return_value = {
             "keys": [
                 jwk,
             ],
         }
-        JWKSEndpointTrust.objects.create(
-            user=self.user,
-            jwks_url='')
+        JWKSEndpointTrust.objects.create(user=self.user, jwks_url="")
         header = Token(self.user.username).create_auth_header(self.key_rsa)
-        request = self.rfactory.get('/', HTTP_AUTHORIZATION=header)
+        request = self.rfactory.get("/", HTTP_AUTHORIZATION=header)
         self.assertNotLoggedIn(request)
         self.run_middleware(request)
         self.assertNotLoggedIn(request)
         self.assertEqual(self.next_middleware.call_count, 1)
 
-
-    @mock.patch('asymmetric_jwt_auth.models.PyJWKClient.fetch_data')
+    @mock.patch("asymmetric_jwt_auth.models.PyJWKClient.fetch_data")
     def test_header_jwt_claimed_username_doesnt_exist(self, mock_fetch_data):
         mock_fetch_data.return_value = {
             "keys": [
                 self.key_rsa.public_key.as_jwk,
             ],
         }
-        JWKSEndpointTrust.objects.create(
-            user=self.user,
-            jwks_url='')
-        header = Token('rusty').create_auth_header(self.key_rsa)
-        request = self.rfactory.get('/', HTTP_AUTHORIZATION=header)
+        JWKSEndpointTrust.objects.create(user=self.user, jwks_url="")
+        header = Token("rusty").create_auth_header(self.key_rsa)
+        request = self.rfactory.get("/", HTTP_AUTHORIZATION=header)
         self.assertNotLoggedIn(request)
         self.run_middleware(request)
         self.assertNotLoggedIn(request)
         self.assertEqual(self.next_middleware.call_count, 1)
 
-
-    @mock.patch('asymmetric_jwt_auth.models.PyJWKClient.fetch_data')
+    @mock.patch("asymmetric_jwt_auth.models.PyJWKClient.fetch_data")
     def test_missing_data(self, mock_fetch_data):
         mock_fetch_data.return_value = {
             "keys": [
                 self.key_rsa.public_key.as_jwk,
             ],
         }
-        JWKSEndpointTrust.objects.create(
-            user=self.user,
-            jwks_url='')
+        JWKSEndpointTrust.objects.create(user=self.user, jwks_url="")
         header = Token(self.user.username, timestamp=0).create_auth_header(self.key_rsa)
-        request = self.rfactory.get('/', HTTP_AUTHORIZATION=header)
+        request = self.rfactory.get("/", HTTP_AUTHORIZATION=header)
         self.assertNotLoggedIn(request)
         self.run_middleware(request)
         self.assertNotLoggedIn(request)
         self.assertEqual(self.next_middleware.call_count, 1)
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/test_models.py` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_models.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,123 +4,105 @@
 from django.utils import timezone
 from .. import models, keys, tokens
 from . import data
 import jwt
 
 
 class ValidatePublicKeyTest(TestCase):
-
     def test_valid_rsa_pem(self):
         models.validate_public_key(data.PEM_PUBLIC_RSA.decode())
 
-
     def test_valid_ed25519_pem(self):
         models.validate_public_key(data.PEM_PUBLIC_ED25519.decode())
 
-
     def test_valid_rsa_openssh(self):
         models.validate_public_key(data.OPENSSH_RSA.decode())
 
-
     def test_valid_ed25519_openssh(self):
         models.validate_public_key(data.OPENSSH_ED25519.decode())
 
-
     def test_invalid_rsa_pem(self):
         with self.assertRaises(ValidationError):
             models.validate_public_key(data.PEM_PUBLIC_RSA_INVALID.decode())
 
-
     def test_invalid_ed25519_pem(self):
         with self.assertRaises(ValidationError):
             models.validate_public_key(data.PEM_PUBLIC_ED25519_INVALID.decode())
 
-
     def test_invalid_rsa_openssh(self):
         with self.assertRaises(ValidationError):
             models.validate_public_key(data.OPENSSH_RSA_INVALID.decode())
 
-
     def test_invalid_ed25519_openssh(self):
         with self.assertRaises(ValidationError):
             models.validate_public_key(data.OPENSSH_ED25519_INVALID.decode())
 
 
-
 class PublicKeyTest(TestCase):
     def setUp(self):
-        self.user = User.objects.create_user(username='foo')
-
+        self.user = User.objects.create_user(username="foo")
 
     def test_extract_comment(self):
-        pub = models.PublicKey(
-            user=self.user,
-            key=data.OPENSSH_ED25519,
-            comment="")
+        pub = models.PublicKey(user=self.user, key=data.OPENSSH_ED25519, comment="")
         pub.save()
-        self.assertEqual(pub.comment, 'crgwbr@foo')
-
+        self.assertEqual(pub.comment, "crgwbr@foo")
 
     def test_update_last_used_datetime(self):
-        pub = models.PublicKey(
-            user=self.user,
-            key=data.OPENSSH_ED25519)
+        pub = models.PublicKey(user=self.user, key=data.OPENSSH_ED25519)
         pub.save()
         self.assertEqual(pub.last_used_on, None)
         pub.update_last_used_datetime()
         # Check the first 19 digits (year – second precision) of ISO time: 2021-03-03T17:00:24
-        self.assertEqual(pub.last_used_on.isoformat()[:19], timezone.now().isoformat()[:19])
-
+        self.assertEqual(
+            pub.last_used_on.isoformat()[:19], timezone.now().isoformat()[:19]
+        )
 
     def test_get_key_ed25519(self):
-        pub = models.PublicKey(
-            user=self.user,
-            key=data.OPENSSH_ED25519)
+        pub = models.PublicKey(user=self.user, key=data.OPENSSH_ED25519)
         pub.save()
         self.assertIsInstance(pub.get_key(), keys.Ed25519PublicKey)
 
-
     def test_get_loaded_key_rsa(self):
-        pub = models.PublicKey(
-            user=self.user,
-            key=data.OPENSSH_RSA,
-            comment="")
+        pub = models.PublicKey(user=self.user, key=data.OPENSSH_RSA, comment="")
         pub.save()
         self.assertIsInstance(pub.get_key(), keys.RSAPublicKey)
 
-
     def test_get_loaded_key_invalid(self):
-        pub = models.PublicKey(
-            user=self.user,
-            key=data.OPENSSH_ED25519_INVALID)
+        pub = models.PublicKey(user=self.user, key=data.OPENSSH_ED25519_INVALID)
         pub.save()
         with self.assertRaises(ValueError):
             pub.get_key()
 
 
-
 class JWKSEndpointTrustTest(TestCase):
     def setUp(self):
-        self.user = User.objects.create_user(username='foo')
+        self.user = User.objects.create_user(username="foo")
         self.jwks = models.JWKSEndpointTrust.objects.create(
             user=self.user,
-            jwks_url='https://dev-87evx9ru.auth0.com/.well-known/jwks.json')
+            jwks_url="https://dev-87evx9ru.auth0.com/.well-known/jwks.json",
+        )
 
     def test_get_signing_key(self):
-        untrusted_token = tokens.UntrustedToken(b"eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsImtpZCI6Ik5FRTFRVVJCT1RNNE16STVSa0ZETlRZeE9UVTFNRGcyT0Rnd1EwVXpNVGsxUWpZeVJrUkZRdyJ9.eyJpc3MiOiJodHRwczovL2Rldi04N2V2eDlydS5hdXRoMC5jb20vIiwic3ViIjoiYVc0Q2NhNzl4UmVMV1V6MGFFMkg2a0QwTzNjWEJWdENAY2xpZW50cyIsImF1ZCI6Imh0dHBzOi8vZXhwZW5zZXMtYXBpIiwiaWF0IjoxNTcyMDA2OTU0LCJleHAiOjE1NzIwMDY5NjQsImF6cCI6ImFXNENjYTc5eFJlTFdVejBhRTJINmtEME8zY1hCVnRDIiwiZ3R5IjoiY2xpZW50LWNyZWRlbnRpYWxzIn0.PUxE7xn52aTCohGiWoSdMBZGiYAHwE5FYie0Y1qUT68IHSTXwXVd6hn02HTah6epvHHVKA2FqcFZ4GGv5VTHEvYpeggiiZMgbxFrmTEY0csL6VNkX1eaJGcuehwQCRBKRLL3zKmA5IKGy5GeUnIbpPHLHDxr-GXvgFzsdsyWlVQvPX2xjeaQ217r2PtxDeqjlf66UYl6oY6AqNS8DH3iryCvIfCcybRZkc_hdy-6ZMoKT6Piijvk_aXdm7-QQqKJFHLuEqrVSOuBqqiNfVrG27QzAPuPOxvfXTVLXL2jek5meH6n-VWgrBdoMFH93QEszEDowDAEhQPHVs0xj7SIzA")  # NOQA
+        untrusted_token = tokens.UntrustedToken(
+            b"eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsImtpZCI6Ik5FRTFRVVJCT1RNNE16STVSa0ZETlRZeE9UVTFNRGcyT0Rnd1EwVXpNVGsxUWpZeVJrUkZRdyJ9.eyJpc3MiOiJodHRwczovL2Rldi04N2V2eDlydS5hdXRoMC5jb20vIiwic3ViIjoiYVc0Q2NhNzl4UmVMV1V6MGFFMkg2a0QwTzNjWEJWdENAY2xpZW50cyIsImF1ZCI6Imh0dHBzOi8vZXhwZW5zZXMtYXBpIiwiaWF0IjoxNTcyMDA2OTU0LCJleHAiOjE1NzIwMDY5NjQsImF6cCI6ImFXNENjYTc5eFJlTFdVejBhRTJINmtEME8zY1hCVnRDIiwiZ3R5IjoiY2xpZW50LWNyZWRlbnRpYWxzIn0.PUxE7xn52aTCohGiWoSdMBZGiYAHwE5FYie0Y1qUT68IHSTXwXVd6hn02HTah6epvHHVKA2FqcFZ4GGv5VTHEvYpeggiiZMgbxFrmTEY0csL6VNkX1eaJGcuehwQCRBKRLL3zKmA5IKGy5GeUnIbpPHLHDxr-GXvgFzsdsyWlVQvPX2xjeaQ217r2PtxDeqjlf66UYl6oY6AqNS8DH3iryCvIfCcybRZkc_hdy-6ZMoKT6Piijvk_aXdm7-QQqKJFHLuEqrVSOuBqqiNfVrG27QzAPuPOxvfXTVLXL2jek5meH6n-VWgrBdoMFH93QEszEDowDAEhQPHVs0xj7SIzA"  # NOQA
+        )
         signing_key = self.jwks.get_signing_key(untrusted_token)
         self.assertIsInstance(signing_key, keys.RSAPublicKey)
         data = jwt.decode(
             untrusted_token.token,
             signing_key.as_pem,
             algorithms=["RS256"],
             audience="https://expenses-api",
-            options={"verify_exp": False})
-        self.assertEqual(data, {
-            'iss': 'https://dev-87evx9ru.auth0.com/',
-            'sub': 'aW4Cca79xReLWUz0aE2H6kD0O3cXBVtC@clients',
-            'aud': 'https://expenses-api',
-            'iat': 1572006954,
-            'exp': 1572006964,
-            'azp': 'aW4Cca79xReLWUz0aE2H6kD0O3cXBVtC',
-            'gty': 'client-credentials',
-        })
+            options={"verify_exp": False},
+        )
+        self.assertEqual(
+            data,
+            {
+                "iss": "https://dev-87evx9ru.auth0.com/",
+                "sub": "aW4Cca79xReLWUz0aE2H6kD0O3cXBVtC@clients",
+                "aud": "https://expenses-api",
+                "iat": 1572006954,
+                "exp": 1572006964,
+                "azp": "aW4Cca79xReLWUz0aE2H6kD0O3cXBVtC",
+                "gty": "client-credentials",
+            },
+        )
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/test_token.py` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_token.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,113 +4,109 @@
 from freezegun import freeze_time
 from datetime import datetime, timedelta
 from .. import tokens, keys
 from . import data
 import jwt
 
 
-
 class TokenToken(TestCase):
-
     def setUp(self):
-        self.username = 'rusty'
+        self.username = "rusty"
         self.privkey = keys.Ed25519PrivateKey.generate()
 
-
-    @patch('time.time')
-    @patch('secrets.token_urlsafe')
+    @patch("time.time")
+    @patch("secrets.token_urlsafe")
     def test_create_auth_header(self, mock_get_nonce, mock_time):
-        mock_get_nonce.return_value = 'yVJ0MVWhqPQ'
+        mock_get_nonce.return_value = "yVJ0MVWhqPQ"
         mock_time.return_value = 1234000.3
-        token = tokens.Token(
-            username=self.username)
+        token = tokens.Token(username=self.username)
         header = token.create_auth_header(self.privkey)
-        self.assertTrue(header.startswith('JWT '))
+        self.assertTrue(header.startswith("JWT "))
         data = jwt.decode(
-            jwt=header.split(' ')[1],
+            jwt=header.split(" ")[1],
             key=self.privkey.public_key.as_pem,
-            algorithms=self.privkey.public_key.allowed_algorithms)
-        self.assertEqual(data, {
-            'nonce': 'yVJ0MVWhqPQ',
-            'time': 1234000,
-            'username': 'rusty',
-        })
+            algorithms=self.privkey.public_key.allowed_algorithms,
+        )
+        self.assertEqual(
+            data,
+            {
+                "nonce": "yVJ0MVWhqPQ",
+                "time": 1234000,
+                "username": "rusty",
+            },
+        )
 
-
-    @patch('secrets.token_urlsafe')
+    @patch("secrets.token_urlsafe")
     def test_create_auth_header_custom_time(self, mock_get_nonce):
-        mock_get_nonce.return_value = 'yVJ0MVWhqPQ'
-        token = tokens.Token(
-            username=self.username,
-            timestamp=1614974974)
+        mock_get_nonce.return_value = "yVJ0MVWhqPQ"
+        token = tokens.Token(username=self.username, timestamp=1614974974)
         header = token.create_auth_header(self.privkey)
-        self.assertTrue(header.startswith('JWT '))
+        self.assertTrue(header.startswith("JWT "))
         data = jwt.decode(
-            jwt=header.split(' ')[1],
+            jwt=header.split(" ")[1],
             key=self.privkey.public_key.as_pem,
-            algorithms=self.privkey.public_key.allowed_algorithms)
-        self.assertEqual(data, {
-            'nonce': 'yVJ0MVWhqPQ',
-            'time': 1614974974,
-            'username': 'rusty',
-        })
+            algorithms=self.privkey.public_key.allowed_algorithms,
+        )
+        self.assertEqual(
+            data,
+            {
+                "nonce": "yVJ0MVWhqPQ",
+                "time": 1614974974,
+                "username": "rusty",
+            },
+        )
 
 
 class UntrustedTokenTest(TestCase):
     def setUp(self):
-        self.username = 'rusty'
-        self.user = User.objects.create(
-            username=self.username)
+        self.username = "rusty"
+        self.user = User.objects.create(username=self.username)
         self.privkey = keys.Ed25519PrivateKey.generate()
-        self.token = tokens.Token(
-            username=self.username)
+        self.token = tokens.Token(username=self.username)
         self.jwt_value = self.token.sign(self.privkey)
         self.untrusted_token = tokens.UntrustedToken(self.jwt_value)
 
-
     def test_get_claimed_username(self):
         self.assertEqual(self.untrusted_token.get_claimed_username(), self.username)
 
-
     def test_verify_valid(self):
         token = self.untrusted_token.verify(self.privkey.public_key)
         self.assertIsInstance(token, tokens.Token)
         self.assertEqual(token.username, self.username)
 
-
     def test_verify_key_mismatch(self):
         pubkey = keys.PublicKey.load_pem(data.PEM_PUBLIC_RSA)
         token = self.untrusted_token.verify(pubkey)
         self.assertIsNone(token)
 
-
     def test_time_out_of_allowed_range_before(self):
         dt = datetime.now() - timedelta(seconds=30)
         with freeze_time(dt):
             token = self.untrusted_token.verify(self.privkey.public_key)
         self.assertIsNone(token)
 
-
     def test_time_out_of_allowed_range_after(self):
         dt = datetime.now() + timedelta(seconds=30)
         with freeze_time(dt):
             token = self.untrusted_token.verify(self.privkey.public_key)
         self.assertIsNone(token)
 
-
     def test_nonce_already_used(self):
         token1 = self.untrusted_token.verify(self.privkey.public_key)
         self.assertIsInstance(token1, tokens.Token)
         self.assertEqual(token1.username, self.username)
         # Second attempt fails because nonce was already used
         token2 = self.untrusted_token.verify(self.privkey.public_key)
         self.assertIsNone(token2)
 
-
-    @override_settings(ASYMMETRIC_JWT_AUTH=dict(NONCE_BACKEND='asymmetric_jwt_auth.nonce.null.NullNonceBackend'))
+    @override_settings(
+        ASYMMETRIC_JWT_AUTH=dict(
+            NONCE_BACKEND="asymmetric_jwt_auth.nonce.null.NullNonceBackend"
+        )
+    )
     def test_nonce_already_used_null_backend(self):
         token1 = self.untrusted_token.verify(self.privkey.public_key)
         self.assertIsInstance(token1, tokens.Token)
         self.assertEqual(token1.username, self.username)
         # Second attempt works becuase null nonce backend doesn't do anything
         token2 = self.untrusted_token.verify(self.privkey.public_key)
         self.assertIsInstance(token2, tokens.Token)
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tests/test_views.py` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tests/test_views.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,84 +3,93 @@
 from django.urls import reverse
 from . import data
 from ..keys import PublicKey
 import json
 
 
 class JWKSViewTest(TestCase):
-
     def setUp(self):
         cache.clear()
 
-
     def test_no_keys(self):
         client = Client()
-        response = client.get(reverse('asymmetric_jwt_auth:jwks'))
+        response = client.get(reverse("asymmetric_jwt_auth:jwks"))
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(json.loads(response.content), {
-            "keys": [],
-        })
-
-
-    @override_settings(ASYMMETRIC_JWT_AUTH=dict(
-        SIGNING_PUBLIC_KEYS=[
-            data.PEM_PUBLIC_RSA,
-            data.PEM_PUBLIC_RSA
-        ],
-    ))
+        self.assertEqual(
+            json.loads(response.content),
+            {
+                "keys": [],
+            },
+        )
+
+    @override_settings(
+        ASYMMETRIC_JWT_AUTH=dict(
+            SIGNING_PUBLIC_KEYS=[data.PEM_PUBLIC_RSA, data.PEM_PUBLIC_RSA],
+        )
+    )
     def test_pem_keys(self):
         client = Client()
-        response = client.get(reverse('asymmetric_jwt_auth:jwks'))
+        response = client.get(reverse("asymmetric_jwt_auth:jwks"))
         self.assertEqual(response.status_code, 200)
         jwk = {
-            'alg': 'RS512',
-            'e': 'AQAB',
-            'kid': '53c5b68c5ecba3e25df3f8326de6c0b0befb67e9217651a2f40e388f6567f056',
-            'kty': 'RSA',
-            'n': 'odxbRh5LOtoB3Shf6K3mRn7ME7Doo5Qm5h72ITt-E6U0l6qXGdVBTj0XhQVNnGjnZTGzU7IacIw1a_03qVHJfcc0Ki7ig7YSPMMl0WSp0m080YlsCZ-9g-WG6DrgjpGQU7yaBhNsKtR5DP20bm8411S9VLqV2GEOzBKpB10_lwhRZuv_Qj7obwSqdVCzMNb7t5LHqG0MxOF7BeYELXIqTEKFfWkZytXCAnmC9hk9RtzUZ_lryD1UgCHZ16gPtmPdFV7fuN8FBNrbaQCldz6V6HVDjsPVxPmVYswV8qInG8kJUpm48s9PAWfgi4HCGmJgn-Irbed2tlRf73jxyCgX0Q',  # NOQA
-            'use': 'sig',
+            "alg": "RS512",
+            "e": "AQAB",
+            "kid": "53c5b68c5ecba3e25df3f8326de6c0b0befb67e9217651a2f40e388f6567f056",
+            "kty": "RSA",
+            "n": "odxbRh5LOtoB3Shf6K3mRn7ME7Doo5Qm5h72ITt-E6U0l6qXGdVBTj0XhQVNnGjnZTGzU7IacIw1a_03qVHJfcc0Ki7ig7YSPMMl0WSp0m080YlsCZ-9g-WG6DrgjpGQU7yaBhNsKtR5DP20bm8411S9VLqV2GEOzBKpB10_lwhRZuv_Qj7obwSqdVCzMNb7t5LHqG0MxOF7BeYELXIqTEKFfWkZytXCAnmC9hk9RtzUZ_lryD1UgCHZ16gPtmPdFV7fuN8FBNrbaQCldz6V6HVDjsPVxPmVYswV8qInG8kJUpm48s9PAWfgi4HCGmJgn-Irbed2tlRf73jxyCgX0Q",  # NOQA
+            "use": "sig",
         }
-        self.assertEqual(json.loads(response.content), {
-            "keys": [
-                jwk,
-                jwk,
+        self.assertEqual(
+            json.loads(response.content),
+            {
+                "keys": [
+                    jwk,
+                    jwk,
+                ],
+            },
+        )
+
+    @override_settings(
+        ASYMMETRIC_JWT_AUTH=dict(
+            SIGNING_PUBLIC_KEYS=[
+                PublicKey.load_pem(data.PEM_PUBLIC_RSA),
             ],
-        })
-
-
-    @override_settings(ASYMMETRIC_JWT_AUTH=dict(
-        SIGNING_PUBLIC_KEYS=[
-            PublicKey.load_pem(data.PEM_PUBLIC_RSA),
-        ],
-    ))
+        )
+    )
     def test_loaded_keys(self):
         client = Client()
-        response = client.get(reverse('asymmetric_jwt_auth:jwks'))
+        response = client.get(reverse("asymmetric_jwt_auth:jwks"))
         self.assertEqual(response.status_code, 200)
         jwk = {
-            'alg': 'RS512',
-            'e': 'AQAB',
-            'kid': '53c5b68c5ecba3e25df3f8326de6c0b0befb67e9217651a2f40e388f6567f056',
-            'kty': 'RSA',
-            'n': 'odxbRh5LOtoB3Shf6K3mRn7ME7Doo5Qm5h72ITt-E6U0l6qXGdVBTj0XhQVNnGjnZTGzU7IacIw1a_03qVHJfcc0Ki7ig7YSPMMl0WSp0m080YlsCZ-9g-WG6DrgjpGQU7yaBhNsKtR5DP20bm8411S9VLqV2GEOzBKpB10_lwhRZuv_Qj7obwSqdVCzMNb7t5LHqG0MxOF7BeYELXIqTEKFfWkZytXCAnmC9hk9RtzUZ_lryD1UgCHZ16gPtmPdFV7fuN8FBNrbaQCldz6V6HVDjsPVxPmVYswV8qInG8kJUpm48s9PAWfgi4HCGmJgn-Irbed2tlRf73jxyCgX0Q',  # NOQA
-            'use': 'sig',
+            "alg": "RS512",
+            "e": "AQAB",
+            "kid": "53c5b68c5ecba3e25df3f8326de6c0b0befb67e9217651a2f40e388f6567f056",
+            "kty": "RSA",
+            "n": "odxbRh5LOtoB3Shf6K3mRn7ME7Doo5Qm5h72ITt-E6U0l6qXGdVBTj0XhQVNnGjnZTGzU7IacIw1a_03qVHJfcc0Ki7ig7YSPMMl0WSp0m080YlsCZ-9g-WG6DrgjpGQU7yaBhNsKtR5DP20bm8411S9VLqV2GEOzBKpB10_lwhRZuv_Qj7obwSqdVCzMNb7t5LHqG0MxOF7BeYELXIqTEKFfWkZytXCAnmC9hk9RtzUZ_lryD1UgCHZ16gPtmPdFV7fuN8FBNrbaQCldz6V6HVDjsPVxPmVYswV8qInG8kJUpm48s9PAWfgi4HCGmJgn-Irbed2tlRf73jxyCgX0Q",  # NOQA
+            "use": "sig",
         }
-        self.assertEqual(json.loads(response.content), {
-            "keys": [
-                jwk,
+        self.assertEqual(
+            json.loads(response.content),
+            {
+                "keys": [
+                    jwk,
+                ],
+            },
+        )
+
+    @override_settings(
+        ASYMMETRIC_JWT_AUTH=dict(
+            SIGNING_PUBLIC_KEYS=[
+                data.PEM_PUBLIC_RSA_INVALID,
             ],
-        })
-
-
-    @override_settings(ASYMMETRIC_JWT_AUTH=dict(
-        SIGNING_PUBLIC_KEYS=[
-            data.PEM_PUBLIC_RSA_INVALID,
-        ],
-    ))
+        )
+    )
     def test_invalid_pem_keys(self):
         client = Client()
-        response = client.get(reverse('asymmetric_jwt_auth:jwks'))
+        response = client.get(reverse("asymmetric_jwt_auth:jwks"))
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(json.loads(response.content), {
-            "keys": [
-            ],
-        })
+        self.assertEqual(
+            json.loads(response.content),
+            {
+                "keys": [],
+            },
+        )
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/tokens.py` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/tokens.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,118 +4,119 @@
 import jwt
 import time
 import logging
 
 logger = logging.getLogger(__name__)
 
 
-
 class Token:
     """
     Represents a JWT that's either been constructed by our code or has been
     verified to be valid.
     """
+
     username: str
     timestamp: int
 
     def __init__(self, username: str, timestamp: Optional[int] = None):
         self.username = username
         self.timestamp = int(time.time()) if timestamp is None else timestamp
 
-
     def create_auth_header(self, private_key: keys.PrivateKey) -> str:
         """
         Create an HTTP Authorization header
         """
 
-        auth_method = get_setting('AUTH_METHOD')
+        auth_method = get_setting("AUTH_METHOD")
         token = self.sign(private_key)
         return f"{auth_method} {token}"
 
-
     def sign(self, private_key: keys.PrivateKey) -> str:
         """
         Create and return signed authentication JWT
         """
         public_key = private_key.public_key
         algorithm = public_key.allowed_algorithms[0]
         nonce = get_nonce_backend().generate_nonce()
         kid = public_key.fingerprint
         # Build and sign claim data
         token_data = {
-            'username': self.username,
-            'time': self.timestamp,
-            'nonce': nonce,
+            "username": self.username,
+            "time": self.timestamp,
+            "nonce": nonce,
         }
         headers = {
-            'kid': kid,
+            "kid": kid,
         }
         token = jwt.encode(
             payload=token_data,
             key=private_key.as_pem,
             algorithm=algorithm,
-            headers=headers)
+            headers=headers,
+        )
         return token
 
 
-
 class UntrustedToken:
     """
     Represents a JWT received from user input (and not yet trusted)
     """
+
     token: str
 
     def __init__(self, token: str):
         self.token = token
 
-
     def get_claimed_username(self) -> Union[None, str]:
         """
         Given a JWT, get the username that it is claiming to be `without verifying that the signature is valid`.
 
         :param token: JWT claim
         :return: Username
         """
-        unverified_data = jwt.decode(self.token, options={
-            'verify_signature': False
-        })
-        return unverified_data.get('username')
-
+        unverified_data = jwt.decode(self.token, options={"verify_signature": False})
+        return unverified_data.get("username")
 
     def verify(self, public_key: keys.PublicKey) -> Union[None, Token]:
         """
         Verify the validity of the given JWT using the given public key.
         """
         try:
             token_data = jwt.decode(
                 jwt=self.token,
                 key=public_key.as_pem.decode(),
-                algorithms=public_key.allowed_algorithms)
+                algorithms=public_key.allowed_algorithms,
+            )
         except jwt.InvalidTokenError:
-            logger.debug('JWT failed verification')
+            logger.debug("JWT failed verification")
             return None
 
-        claimed_username = token_data.get('username')
-        claimed_time = token_data.get('time', 0)
-        claimed_nonce = token_data.get('nonce')
+        claimed_username = token_data.get("username")
+        claimed_time = token_data.get("time", 0)
+        claimed_nonce = token_data.get("nonce")
 
         # Ensure fields aren't blank
         if not claimed_username or not claimed_time or not claimed_nonce:
             return None
 
         # Ensure time is within acceptable bounds
         current_time = time.time()
-        timestamp_tolerance = get_setting('TIMESTAMP_TOLERANCE')
-        min_time, max_time = (current_time - timestamp_tolerance, current_time + timestamp_tolerance)
+        timestamp_tolerance = get_setting("TIMESTAMP_TOLERANCE")
+        min_time, max_time = (
+            current_time - timestamp_tolerance,
+            current_time + timestamp_tolerance,
+        )
         if claimed_time < min_time or claimed_time > max_time:
-            logger.debug('Claimed time is outside of allowable tolerances')
+            logger.debug("Claimed time is outside of allowable tolerances")
             return None
 
         # Ensure nonce is unique
         nonce_backend = get_nonce_backend()
-        if not nonce_backend.validate_nonce(claimed_username, claimed_time, claimed_nonce):
-            logger.debug('Claimed nonce failed to validate')
+        if not nonce_backend.validate_nonce(
+            claimed_username, claimed_time, claimed_nonce
+        ):
+            logger.debug("Claimed nonce failed to validate")
             return None
 
         # If we've gotten this far, the token is valid
         nonce_backend.log_used_nonce(claimed_username, claimed_time, claimed_nonce)
         return Token(claimed_username, claimed_time)
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/utils.py` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,12 +13,12 @@
 
 def long_to_base64(n: int, mlen: int = 0) -> str:
     bys = long2intarr(n)
     if mlen:
         _len = mlen - len(bys)
         if _len:
             bys = [0] * _len + bys
-    data = struct.pack('%sB' % len(bys), *bys)
+    data = struct.pack("%sB" % len(bys), *bys)
     if not len(data):
-        data = b'\x00'
-    s = base64.urlsafe_b64encode(data).rstrip(b'=')
+        data = b"\x00"
+    s = base64.urlsafe_b64encode(data).rstrip(b"=")
     return s.decode("ascii")
```

### Comparing `asymmetric_jwt_auth-1.0.0b1/src/asymmetric_jwt_auth/views.py` & `asymmetric_jwt_auth-1.0.1b5/src/asymmetric_jwt_auth/views.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from django.views import View
 from django.http import JsonResponse
 from . import get_setting
 from .keys import PublicKey
 
 
 class JWKSEndpointView(View):
-
     def get(self, request):
         keys = self.list_pub_keys()
         data = {
             "keys": [key.as_jwk for key in keys],
         }
         return JsonResponse(data)
 
-
     def list_pub_keys(self):
         keys = []
-        for _key in get_setting('SIGNING_PUBLIC_KEYS'):
+        for _key in get_setting("SIGNING_PUBLIC_KEYS"):
             if isinstance(_key, PublicKey):
                 keys.append(_key)
             else:
                 exc, key = PublicKey.load_serialized_public_key(_key)
                 if key is not None:
                     keys.append(key)
         return keys
```

