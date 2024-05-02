# Comparing `tmp/niquests-3.6.1.tar.gz` & `tmp/niquests-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Apr 22 05:40:24 2024, max compression
+gzip compressed data, last modified: Thu May  2 06:04:54 2024, max compression
```

## Comparing `niquests-3.6.1.tar` & `niquests-3.6.2.tar`

### file list

```diff
@@ -1,69 +1,71 @@
--rw-r--r--   0        0        0      718 2024-04-22 05:40:24.000000 niquests-3.6.1/AUTHORS.rst
--rw-r--r--   0        0        0    85995 2024-04-22 05:40:24.000000 niquests-3.6.1/HISTORY.md
--rw-r--r--   0        0        0      377 2024-04-22 05:40:24.000000 niquests-3.6.1/Makefile
--rw-r--r--   0        0        0       38 2024-04-22 05:40:24.000000 niquests-3.6.1/NOTICE
--rw-r--r--   0        0        0        1 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/.nojekyll
--rw-r--r--   0        0        0     7664 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/Makefile
--rw-r--r--   0        0        0     5355 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/api.rst
--rw-r--r--   0        0        0    12305 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/conf.py
--rw-r--r--   0        0        0     4084 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/index.rst
--rw-r--r--   0        0        0     7253 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/make.bat
--rw-r--r--   0        0        0      185 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/requirements.txt
--rw-r--r--   0        0        0     2990 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/_static/custom.css
--rw-r--r--   0        0        0   306086 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/_static/requests-sidebar.png
--rw-r--r--   0        0        0     7360 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/community/faq.rst
--rw-r--r--   0        0        0     2720 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/community/recommended.rst
--rw-r--r--   0        0        0     1782 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/community/release-process.rst
--rw-r--r--   0        0        0      285 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/community/support.rst
--rw-r--r--   0        0        0      324 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/community/updates.rst
--rw-r--r--   0        0        0      945 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/community/vulnerabilities.rst
--rw-r--r--   0        0        0       48 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/dev/authors.rst
--rw-r--r--   0        0        0     5768 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/dev/contributing.rst
--rw-r--r--   0        0        0     1885 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/dev/migrate.rst
--rw-r--r--   0        0        0    52818 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/user/advanced.rst
--rw-r--r--   0        0        0     6315 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/user/authentication.rst
--rw-r--r--   0        0        0     1046 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/user/install.rst
--rw-r--r--   0        0        0    34594 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/user/quickstart.rst
--rw-r--r--   0        0        0     3071 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/__init__.py
--rw-r--r--   0        0        0      534 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/__version__.py
--rw-r--r--   0        0        0    47149 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/_async.py
--rw-r--r--   0        0        0     2852 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/_compat.py
--rw-r--r--   0        0        0      480 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/_constant.py
--rw-r--r--   0        0        0     5942 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/_typing.py
--rw-r--r--   0        0        0    86853 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/adapters.py
--rw-r--r--   0        0        0    27567 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/api.py
--rw-r--r--   0        0        0     9906 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/auth.py
--rw-r--r--   0        0        0    19797 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/cookies.py
--rw-r--r--   0        0        0     4363 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/exceptions.py
--rw-r--r--   0        0        0     5245 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/help.py
--rw-r--r--   0        0        0     2776 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/hooks.py
--rw-r--r--   0        0        0    62438 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/models.py
--rw-r--r--   0        0        0        0 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/py.typed
--rw-r--r--   0        0        0    69113 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/sessions.py
--rw-r--r--   0        0        0     4284 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/status_codes.py
--rw-r--r--   0        0        0     6973 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/structures.py
--rw-r--r--   0        0        0    37300 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/utils.py
--rw-r--r--   0        0        0      119 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/extensions/__init__.py
--rw-r--r--   0        0        0    22384 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/extensions/_async_ocsp.py
--rw-r--r--   0        0        0    21009 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/extensions/_ocsp.py
--rw-r--r--   0        0        0    16942 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/extensions/_picotls.py
--rw-r--r--   0        0        0       80 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/__init__.py
--rw-r--r--   0        0        0     2193 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/conftest.py
--rw-r--r--   0        0        0     7540 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/test_async.py
--rw-r--r--   0        0        0      875 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/test_help.py
--rw-r--r--   0        0        0      893 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/test_hooks.py
--rw-r--r--   0        0        0     4022 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/test_live.py
--rw-r--r--   0        0        0    15985 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/test_lowlevel.py
--rw-r--r--   0        0        0     3722 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/test_multiplexed.py
--rw-r--r--   0        0        0    99099 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/test_requests.py
--rw-r--r--   0        0        0     2725 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/test_structures.py
--rw-r--r--   0        0        0     6213 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/test_testserver.py
--rw-r--r--   0        0        0    26728 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/test_utils.py
--rw-r--r--   0        0        0      613 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/utils.py
--rw-r--r--   0        0        0        0 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/testserver/__init__.py
--rw-r--r--   0        0        0     3882 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/testserver/server.py
--rw-r--r--   0        0        0      362 2024-04-22 05:40:24.000000 niquests-3.6.1/.gitignore
--rw-r--r--   0        0        0    10142 2024-04-22 05:40:24.000000 niquests-3.6.1/LICENSE
--rw-r--r--   0        0        0    10931 2024-04-22 05:40:24.000000 niquests-3.6.1/README.md
--rw-r--r--   0        0        0     3660 2024-04-22 05:40:24.000000 niquests-3.6.1/pyproject.toml
--rw-r--r--   0        0        0    13292 2024-04-22 05:40:24.000000 niquests-3.6.1/PKG-INFO
+-rw-r--r--   0        0        0      718 2024-05-02 06:04:54.000000 niquests-3.6.2/AUTHORS.rst
+-rw-r--r--   0        0        0    86387 2024-05-02 06:04:54.000000 niquests-3.6.2/HISTORY.md
+-rw-r--r--   0        0        0      377 2024-05-02 06:04:54.000000 niquests-3.6.2/Makefile
+-rw-r--r--   0        0        0       38 2024-05-02 06:04:54.000000 niquests-3.6.2/NOTICE
+-rw-r--r--   0        0        0      201 2024-05-02 06:04:54.000000 niquests-3.6.2/SECURITY.md
+-rw-r--r--   0        0        0      220 2024-05-02 06:04:54.000000 niquests-3.6.2/requirements-dev.txt
+-rw-r--r--   0        0        0        1 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/.nojekyll
+-rw-r--r--   0        0        0     7664 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/Makefile
+-rw-r--r--   0        0        0     5355 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/api.rst
+-rw-r--r--   0        0        0    12305 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/conf.py
+-rw-r--r--   0        0        0     4084 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/index.rst
+-rw-r--r--   0        0        0     7253 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/make.bat
+-rw-r--r--   0        0        0      185 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/requirements.txt
+-rw-r--r--   0        0        0     2990 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/_static/custom.css
+-rw-r--r--   0        0        0   306086 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/_static/requests-sidebar.png
+-rw-r--r--   0        0        0     7360 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/community/faq.rst
+-rw-r--r--   0        0        0     2720 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/community/recommended.rst
+-rw-r--r--   0        0        0     1782 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/community/release-process.rst
+-rw-r--r--   0        0        0      285 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/community/support.rst
+-rw-r--r--   0        0        0      324 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/community/updates.rst
+-rw-r--r--   0        0        0      945 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/community/vulnerabilities.rst
+-rw-r--r--   0        0        0       48 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/dev/authors.rst
+-rw-r--r--   0        0        0     5768 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/dev/contributing.rst
+-rw-r--r--   0        0        0     1885 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/dev/migrate.rst
+-rw-r--r--   0        0        0    52818 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/user/advanced.rst
+-rw-r--r--   0        0        0     6315 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/user/authentication.rst
+-rw-r--r--   0        0        0     1046 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/user/install.rst
+-rw-r--r--   0        0        0    34594 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/user/quickstart.rst
+-rw-r--r--   0        0        0     3071 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/__init__.py
+-rw-r--r--   0        0        0      534 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/__version__.py
+-rw-r--r--   0        0        0    47149 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/_async.py
+-rw-r--r--   0        0        0     2852 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/_compat.py
+-rw-r--r--   0        0        0      480 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/_constant.py
+-rw-r--r--   0        0        0     5942 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/_typing.py
+-rw-r--r--   0        0        0    86853 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/adapters.py
+-rw-r--r--   0        0        0    27567 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/api.py
+-rw-r--r--   0        0        0     9906 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/auth.py
+-rw-r--r--   0        0        0    19797 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/cookies.py
+-rw-r--r--   0        0        0     4363 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/exceptions.py
+-rw-r--r--   0        0        0     5248 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/help.py
+-rw-r--r--   0        0        0     2776 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/hooks.py
+-rw-r--r--   0        0        0    62438 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/models.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/py.typed
+-rw-r--r--   0        0        0    69113 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/sessions.py
+-rw-r--r--   0        0        0     4284 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/status_codes.py
+-rw-r--r--   0        0        0     6973 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/structures.py
+-rw-r--r--   0        0        0    37300 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/utils.py
+-rw-r--r--   0        0        0      119 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/extensions/__init__.py
+-rw-r--r--   0        0        0    22348 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/extensions/_async_ocsp.py
+-rw-r--r--   0        0        0    21009 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/extensions/_ocsp.py
+-rw-r--r--   0        0        0    16942 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/extensions/_picotls.py
+-rw-r--r--   0        0        0       80 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/__init__.py
+-rw-r--r--   0        0        0     2193 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/conftest.py
+-rw-r--r--   0        0        0     7540 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/test_async.py
+-rw-r--r--   0        0        0      875 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/test_help.py
+-rw-r--r--   0        0        0      893 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/test_hooks.py
+-rw-r--r--   0        0        0     4022 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/test_live.py
+-rw-r--r--   0        0        0    15985 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/test_lowlevel.py
+-rw-r--r--   0        0        0     3722 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/test_multiplexed.py
+-rw-r--r--   0        0        0    99099 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/test_requests.py
+-rw-r--r--   0        0        0     2725 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/test_structures.py
+-rw-r--r--   0        0        0     6213 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/test_testserver.py
+-rw-r--r--   0        0        0    26728 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/test_utils.py
+-rw-r--r--   0        0        0      613 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/utils.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/testserver/__init__.py
+-rw-r--r--   0        0        0     3882 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/testserver/server.py
+-rw-r--r--   0        0        0      362 2024-05-02 06:04:54.000000 niquests-3.6.2/.gitignore
+-rw-r--r--   0        0        0    10142 2024-05-02 06:04:54.000000 niquests-3.6.2/LICENSE
+-rw-r--r--   0        0        0    10768 2024-05-02 06:04:54.000000 niquests-3.6.2/README.md
+-rw-r--r--   0        0        0     3662 2024-05-02 06:04:54.000000 niquests-3.6.2/pyproject.toml
+-rw-r--r--   0        0        0    13129 2024-05-02 06:04:54.000000 niquests-3.6.2/PKG-INFO
```

### Comparing `niquests-3.6.1/AUTHORS.rst` & `niquests-3.6.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/HISTORY.md` & `niquests-3.6.2/HISTORY.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Release History
 ===============
 
+3.6.2 (2024-05-02)
+------------------
+
+**Fixed**
+- "Help" program `python -m niquests.help` that depended on h2 while not required anymore.
+- Minor performance regression in async while checking OCSP when certificate isn't eligible (e.g. no OCSP url provided).
+
+**Changed**
+- urllib3.future lower bound constraint has been raised to version 2.7.905 to ensure inclusion of jh2 instead of h2.
+
 3.6.1 (2024-04-22)
 ------------------
 
 **Fixed**
 - Handling broken environments with a graceful exception with a detailed error message.
 
 3.6.0 (2024-04-20)
```

### Comparing `niquests-3.6.1/docs/Makefile` & `niquests-3.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/docs/api.rst` & `niquests-3.6.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/docs/conf.py` & `niquests-3.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/docs/index.rst` & `niquests-3.6.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/docs/make.bat` & `niquests-3.6.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/docs/_static/custom.css` & `niquests-3.6.2/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/docs/_static/requests-sidebar.png` & `niquests-3.6.2/docs/_static/requests-sidebar.png`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/docs/community/faq.rst` & `niquests-3.6.2/docs/community/faq.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/docs/community/recommended.rst` & `niquests-3.6.2/docs/community/recommended.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/docs/community/release-process.rst` & `niquests-3.6.2/docs/community/release-process.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/docs/community/vulnerabilities.rst` & `niquests-3.6.2/docs/community/vulnerabilities.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/docs/dev/contributing.rst` & `niquests-3.6.2/docs/dev/contributing.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/docs/dev/migrate.rst` & `niquests-3.6.2/docs/dev/migrate.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/docs/user/advanced.rst` & `niquests-3.6.2/docs/user/advanced.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/docs/user/authentication.rst` & `niquests-3.6.2/docs/user/authentication.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/docs/user/install.rst` & `niquests-3.6.2/docs/user/install.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/docs/user/quickstart.rst` & `niquests-3.6.2/docs/user/quickstart.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/src/niquests/__init__.py` & `niquests-3.6.2/src/niquests/__init__.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/src/niquests/__version__.py` & `niquests-3.6.2/src/niquests/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 
 __title__: str = "niquests"
 __description__: str = "Python HTTP for Humans."
 __url__: str = "https://niquests.readthedocs.io"
 
 __version__: str
-__version__ = "3.6.1"
+__version__ = "3.6.2"
 
-__build__: int = 0x030601
+__build__: int = 0x030602
 __author__: str = "Kenneth Reitz"
 __author_email__: str = "me@kennethreitz.org"
 __license__: str = "Apache-2.0"
 __copyright__: str = "Copyright Kenneth Reitz"
 __cake__: str = "\u2728 \U0001f370 \u2728"
```

### Comparing `niquests-3.6.1/src/niquests/_async.py` & `niquests-3.6.2/src/niquests/_async.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/src/niquests/_compat.py` & `niquests-3.6.2/src/niquests/_compat.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/src/niquests/_typing.py` & `niquests-3.6.2/src/niquests/_typing.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/src/niquests/adapters.py` & `niquests-3.6.2/src/niquests/adapters.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/src/niquests/api.py` & `niquests-3.6.2/src/niquests/api.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/src/niquests/auth.py` & `niquests-3.6.2/src/niquests/auth.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/src/niquests/cookies.py` & `niquests-3.6.2/src/niquests/cookies.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/src/niquests/exceptions.py` & `niquests-3.6.2/src/niquests/exceptions.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/src/niquests/help.py` & `niquests-3.6.2/src/niquests/help.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import platform
 import ssl
 import sys
 import warnings
 from json import JSONDecodeError
 
 import charset_normalizer
-import h2  # type: ignore
+import jh2  # type: ignore
 import h11
 import idna
 import wassima
 
 from . import RequestException
 from . import __version__ as niquests_version
 from . import get
@@ -124,15 +124,15 @@
             "version": niquests_version,
         },
         "http3": {
             "enabled": qh3 is not None,
             "qh3": qh3.__version__ if qh3 is not None else None,
         },
         "http2": {
-            "h2": h2.__version__,
+            "jh2": jh2.__version__,
         },
         "http1": {
             "h11": h11.__version__,
         },
         "wassima": {
             "enabled": wassima.RUSTLS_LOADED,
             "certifi_fallback": wassima.RUSTLS_LOADED is False and certifi is not None,
```

### Comparing `niquests-3.6.1/src/niquests/hooks.py` & `niquests-3.6.2/src/niquests/hooks.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/src/niquests/models.py` & `niquests-3.6.2/src/niquests/models.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/src/niquests/sessions.py` & `niquests-3.6.2/src/niquests/sessions.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/src/niquests/status_codes.py` & `niquests-3.6.2/src/niquests/status_codes.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/src/niquests/structures.py` & `niquests-3.6.2/src/niquests/structures.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/src/niquests/utils.py` & `niquests-3.6.2/src/niquests/utils.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/src/niquests/extensions/_async_ocsp.py` & `niquests-3.6.2/src/niquests/extensions/_async_ocsp.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,28 +305,28 @@
     if (
         conn_info is None
         or conn_info.certificate_der is None
         or conn_info.certificate_dict is None
     ):
         return
 
-    peer_certificate = Certificate(conn_info.certificate_der)
+    endpoints: list[str] = [  # type: ignore
+        # exclude non-HTTP endpoint. like ldap.
+        ep  # type: ignore
+        for ep in list(conn_info.certificate_dict.get("OCSP", []))  # type: ignore
+        if ep.startswith("http://")  # type: ignore
+    ]
 
-    async with _SharedRevocationStatusCache.lock(peer_certificate):
-        endpoints: list[str] = [  # type: ignore
-            # exclude non-HTTP endpoint. like ldap.
-            ep  # type: ignore
-            for ep in list(conn_info.certificate_dict.get("OCSP", []))  # type: ignore
-            if ep.startswith("http://")  # type: ignore
-        ]
+    # well... not all issued certificate have a OCSP entry. e.g. mkcert.
+    if not endpoints:
+        return
 
-        # well... not all issued certificate have a OCSP entry. e.g. mkcert.
-        if not endpoints:
-            return
+    peer_certificate = Certificate(conn_info.certificate_der)
 
+    async with _SharedRevocationStatusCache.lock(peer_certificate):
         # this feature, by default, is reserved for a reasonable usage.
         if not strict:
             mean_rate_sec = _SharedRevocationStatusCache.rate()
             cache_count = len(_SharedRevocationStatusCache)
 
             if cache_count >= 10 and mean_rate_sec <= 1.0:
                 _SharedRevocationStatusCache.hold = True
```

### Comparing `niquests-3.6.1/src/niquests/extensions/_ocsp.py` & `niquests-3.6.2/src/niquests/extensions/_ocsp.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/src/niquests/extensions/_picotls.py` & `niquests-3.6.2/src/niquests/extensions/_picotls.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/tests/conftest.py` & `niquests-3.6.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/tests/test_async.py` & `niquests-3.6.2/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/tests/test_help.py` & `niquests-3.6.2/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/tests/test_hooks.py` & `niquests-3.6.2/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/tests/test_live.py` & `niquests-3.6.2/tests/test_live.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/tests/test_lowlevel.py` & `niquests-3.6.2/tests/test_lowlevel.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/tests/test_multiplexed.py` & `niquests-3.6.2/tests/test_multiplexed.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/tests/test_requests.py` & `niquests-3.6.2/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/tests/test_structures.py` & `niquests-3.6.2/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/tests/test_testserver.py` & `niquests-3.6.2/tests/test_testserver.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/tests/test_utils.py` & `niquests-3.6.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/tests/utils.py` & `niquests-3.6.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/tests/testserver/server.py` & `niquests-3.6.2/tests/testserver/server.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/LICENSE` & `niquests-3.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `niquests-3.6.1/README.md` & `niquests-3.6.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 </div>
 
 **Niquests** is a simple, yet elegant, HTTP library. It is a drop-in replacement for **Requests**, which is under feature freeze.
 
 Niquests, is the “**Safest**, **Fastest[^10]**, **Easiest**, and **Most advanced**” Python HTTP Client. Production Ready!
 
 ✔️ **Try before you switch:** [See Multiplexed in Action](https://replit.com/@ahmedtahri4/Python#main.py)<br>
-📖 **See why you should switch:** [Read about 10 reasons why](https://medium.com/dev-genius/10-reasons-you-should-quit-your-http-client-98fd4c94bef3), and ["_Revived the promise made six years ago for Requests 3_"](https://medium.com/@ahmed.tahri/revived-the-promise-made-six-years-ago-for-requests-3-37b440e6a064)
+📖 **See why you should switch:** [Read about 10 reasons why](https://medium.com/@ahmed.tahri/10-reasons-you-should-quit-your-http-client-98fd4c94bef3), and ["_Revived the promise made six years ago for Requests 3_"](https://medium.com/@ahmed.tahri/revived-the-promise-made-six-years-ago-for-requests-3-37b440e6a064)
 
 <details>
   <summary>👆 <b>Look at the feature table comparison</b> against <i>requests, httpx and aiohttp</i>!</summary>
 
 | Feature                             | niquests | requests  |     httpx     | aiohttp       |
 |-------------------------------------|:--------:|:---------:|:-------------:|---------------|
 | `HTTP/1.1`                          |    ✅     |     ✅     |       ✅       | ✅             |
@@ -44,28 +44,28 @@
 <details>
   <summary>📈 <b>Look at the performance comparison</b> against <i>them</i>!</summary>
 
 _Scenario:_ Fetch a thousand requests using 10 tasks or threads, each with a hundred requests using a single pool of connection.
 
 **High-Level APIs**
 
-| Client   | Average Delay to Complete                | Notes                        |
-|----------|------------------------------------------|------------------------------|
-| requests | <span style="color:red">987 ms</span>    | ThreadPoolExecutor. HTTP/1.1 |
-| httpx    | <span style="color:orange">735 ms</span> | Asyncio. HTTP/2              |
-| niquests | <span style="color:green">470 ms</span>  | Asyncio. HTTP/2              |
+| Client   | Average Delay to Complete | Notes                        |
+|----------|---------------------------|------------------------------|
+| requests | 987 ms                    | ThreadPoolExecutor. HTTP/1.1 |
+| httpx    | 735 ms                    | Asyncio. HTTP/2              |
+| niquests | 400 ms                    | Asyncio. HTTP/2              |
 
 **Simplified APIs**
 
-| Client        | Average Delay to Complete                | Notes                        |
-|---------------|------------------------------------------|------------------------------|
-| requests core | <span style="color:red">643 ms</span>    | ThreadPoolExecutor. HTTP/1.1 |
-| httpx core    | <span style="color:orange">550 ms</span> | Asyncio. HTTP/2              |
-| aiohttp       | <span style="color:green">220 ms</span>  | Asyncio. HTTP/1.1            |
-| niquests core | <span style="color:green">210 ms</span>  | Asyncio. HTTP/2              |
+| Client        | Average Delay to Complete | Notes                        |
+|---------------|---------------------------|------------------------------|
+| requests core | 643 ms                    | ThreadPoolExecutor. HTTP/1.1 |
+| httpx core    | 550 ms                    | Asyncio. HTTP/2              |
+| aiohttp       | 220 ms                    | Asyncio. HTTP/1.1            |
+| niquests core | 190 ms                    | Asyncio. HTTP/2              |
 
 Did you give up on HTTP/2 due to performance concerns? Think again! Multiplexing and response lazyness open up a wide range
 of possibilities! Want to learn more about the tests? scripts? reasoning?
 
 Take a deeper look at https://github.com/Ousret/niquests-stats
 
 ⚠️ Do the responsible thing with this library and do not attempt DoS remote servers using its abilities.
```

### Comparing `niquests-3.6.1/pyproject.toml` & `niquests-3.6.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     "Topic :: Software Development :: Libraries",
 ]
 requires-python = ">=3.7"
 dynamic = ["version"]
 dependencies = [
     "charset_normalizer>=2,<4",
     "idna>=2.5,<4",
-    "urllib3.future>=2.7.904,<3",
+    "urllib3.future>=2.7.905,<3",
     "wassima>=1.0.1,<2",
     "kiss_headers>=2,<4",
 ]
 
 [project.optional-dependencies]
 socks = [
     "urllib3.future[socks]",
@@ -71,22 +71,22 @@
 path = "src/niquests/__version__.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
     "/docs",
     "/src",
     "/tests",
-    "/dev-requirements.txt",
+    "/requirements-dev.txt",
     "/HISTORY.md",
     "/README.md",
+    "/SECURITY.md",
     "/AUTHORS.rst",
     "/LICENSE",
     "/NOTICE",
     "/Makefile",
-    "/setup.cfg",
 ]
 
 [tool.hatch.build.targets.wheel]
 packages = [
     "src/niquests",
 ]
```

### Comparing `niquests-3.6.1/PKG-INFO` & `niquests-3.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: niquests
-Version: 3.6.1
+Version: 3.6.2
 Summary: Niquests is a simple, yet elegant, HTTP library. It is a drop-in replacement for Requests, which is under feature freeze.
 Project-URL: Changelog, https://github.com/jawah/niquests/blob/main/HISTORY.md
 Project-URL: Documentation, https://niquests.readthedocs.io
 Project-URL: Code, https://github.com/jawah/niquests
 Project-URL: Issue tracker, https://github.com/jawah/niquests/issues
 Author-email: Kenneth Reitz <me@kennethreitz.org>
 Maintainer-email: "Ahmed R. TAHRI" <ahmed.tahri@cloudnursery.dev>
@@ -30,15 +30,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Requires-Dist: charset-normalizer<4,>=2
 Requires-Dist: idna<4,>=2.5
 Requires-Dist: kiss-headers<4,>=2
-Requires-Dist: urllib3-future<3,>=2.7.904
+Requires-Dist: urllib3-future<3,>=2.7.905
 Requires-Dist: wassima<2,>=1.0.1
 Provides-Extra: http3
 Requires-Dist: urllib3-future[qh3]; extra == 'http3'
 Provides-Extra: ocsp
 Requires-Dist: urllib3-future[qh3]; extra == 'ocsp'
 Provides-Extra: socks
 Requires-Dist: urllib3-future[socks]; extra == 'socks'
@@ -52,15 +52,15 @@
 </div>
 
 **Niquests** is a simple, yet elegant, HTTP library. It is a drop-in replacement for **Requests**, which is under feature freeze.
 
 Niquests, is the “**Safest**, **Fastest[^10]**, **Easiest**, and **Most advanced**” Python HTTP Client. Production Ready!
 
 ✔️ **Try before you switch:** [See Multiplexed in Action](https://replit.com/@ahmedtahri4/Python#main.py)<br>
-📖 **See why you should switch:** [Read about 10 reasons why](https://medium.com/dev-genius/10-reasons-you-should-quit-your-http-client-98fd4c94bef3), and ["_Revived the promise made six years ago for Requests 3_"](https://medium.com/@ahmed.tahri/revived-the-promise-made-six-years-ago-for-requests-3-37b440e6a064)
+📖 **See why you should switch:** [Read about 10 reasons why](https://medium.com/@ahmed.tahri/10-reasons-you-should-quit-your-http-client-98fd4c94bef3), and ["_Revived the promise made six years ago for Requests 3_"](https://medium.com/@ahmed.tahri/revived-the-promise-made-six-years-ago-for-requests-3-37b440e6a064)
 
 <details>
   <summary>👆 <b>Look at the feature table comparison</b> against <i>requests, httpx and aiohttp</i>!</summary>
 
 | Feature                             | niquests | requests  |     httpx     | aiohttp       |
 |-------------------------------------|:--------:|:---------:|:-------------:|---------------|
 | `HTTP/1.1`                          |    ✅     |     ✅     |       ✅       | ✅             |
@@ -93,28 +93,28 @@
 <details>
   <summary>📈 <b>Look at the performance comparison</b> against <i>them</i>!</summary>
 
 _Scenario:_ Fetch a thousand requests using 10 tasks or threads, each with a hundred requests using a single pool of connection.
 
 **High-Level APIs**
 
-| Client   | Average Delay to Complete                | Notes                        |
-|----------|------------------------------------------|------------------------------|
-| requests | <span style="color:red">987 ms</span>    | ThreadPoolExecutor. HTTP/1.1 |
-| httpx    | <span style="color:orange">735 ms</span> | Asyncio. HTTP/2              |
-| niquests | <span style="color:green">470 ms</span>  | Asyncio. HTTP/2              |
+| Client   | Average Delay to Complete | Notes                        |
+|----------|---------------------------|------------------------------|
+| requests | 987 ms                    | ThreadPoolExecutor. HTTP/1.1 |
+| httpx    | 735 ms                    | Asyncio. HTTP/2              |
+| niquests | 400 ms                    | Asyncio. HTTP/2              |
 
 **Simplified APIs**
 
-| Client        | Average Delay to Complete                | Notes                        |
-|---------------|------------------------------------------|------------------------------|
-| requests core | <span style="color:red">643 ms</span>    | ThreadPoolExecutor. HTTP/1.1 |
-| httpx core    | <span style="color:orange">550 ms</span> | Asyncio. HTTP/2              |
-| aiohttp       | <span style="color:green">220 ms</span>  | Asyncio. HTTP/1.1            |
-| niquests core | <span style="color:green">210 ms</span>  | Asyncio. HTTP/2              |
+| Client        | Average Delay to Complete | Notes                        |
+|---------------|---------------------------|------------------------------|
+| requests core | 643 ms                    | ThreadPoolExecutor. HTTP/1.1 |
+| httpx core    | 550 ms                    | Asyncio. HTTP/2              |
+| aiohttp       | 220 ms                    | Asyncio. HTTP/1.1            |
+| niquests core | 190 ms                    | Asyncio. HTTP/2              |
 
 Did you give up on HTTP/2 due to performance concerns? Think again! Multiplexing and response lazyness open up a wide range
 of possibilities! Want to learn more about the tests? scripts? reasoning?
 
 Take a deeper look at https://github.com/Ousret/niquests-stats
 
 ⚠️ Do the responsible thing with this library and do not attempt DoS remote servers using its abilities.
```

