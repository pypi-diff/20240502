# Comparing `tmp/django_gov_notify-0.4.0.tar.gz` & `tmp/django_gov_notify-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_gov_notify-0.4.0.tar", max compression
+gzip compressed data, was "django_gov_notify-0.5.0.tar", max compression
```

## Comparing `django_gov_notify-0.4.0.tar` & `django_gov_notify-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     4303 2023-11-13 11:28:10.756919 django_gov_notify-0.4.0/README.md
--rw-r--r--   0        0        0       22 2020-05-29 11:47:22.143681 django_gov_notify-0.4.0/django_gov_notify/__init__.py
--rw-r--r--   0        0        0     2438 2020-05-28 16:44:09.438661 django_gov_notify-0.4.0/django_gov_notify/backends.py
--rw-r--r--   0        0        0     3997 2023-11-13 11:28:10.756919 django_gov_notify-0.4.0/django_gov_notify/message.py
--rw-r--r--   0        0        0      876 2020-05-28 16:43:25.485950 django_gov_notify-0.4.0/django_gov_notify/utils.py
--rw-r--r--   0        0        0     1296 2023-11-13 11:28:28.637040 django_gov_notify-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5486 1970-01-01 00:00:00.000000 django_gov_notify-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1320 2020-06-18 10:13:39.933804 django_gov_notify-0.5.0/LICENCE
+-rw-r--r--   0        0        0     4303 2024-04-18 13:55:30.373125 django_gov_notify-0.5.0/README.md
+-rw-r--r--   0        0        0       22 2020-05-29 11:47:22.143681 django_gov_notify-0.5.0/django_gov_notify/__init__.py
+-rw-r--r--   0        0        0     2438 2020-05-28 16:44:09.438661 django_gov_notify-0.5.0/django_gov_notify/backends.py
+-rw-r--r--   0        0        0     3997 2023-11-13 11:28:10.756919 django_gov_notify-0.5.0/django_gov_notify/message.py
+-rw-r--r--   0        0        0      876 2020-05-28 16:43:25.485950 django_gov_notify-0.5.0/django_gov_notify/utils.py
+-rw-r--r--   0        0        0     1384 2024-05-02 13:55:59.050182 django_gov_notify-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5671 1970-01-01 00:00:00.000000 django_gov_notify-0.5.0/PKG-INFO
```

### Comparing `django_gov_notify-0.4.0/README.md` & `django_gov_notify-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `django_gov_notify-0.4.0/django_gov_notify/backends.py` & `django_gov_notify-0.5.0/django_gov_notify/backends.py`

 * *Files identical despite different names*

### Comparing `django_gov_notify-0.4.0/django_gov_notify/message.py` & `django_gov_notify-0.5.0/django_gov_notify/message.py`

 * *Files identical despite different names*

### Comparing `django_gov_notify-0.4.0/django_gov_notify/utils.py` & `django_gov_notify-0.5.0/django_gov_notify/utils.py`

 * *Files identical despite different names*

### Comparing `django_gov_notify-0.4.0/pyproject.toml` & `django_gov_notify-0.5.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-gov-notify"
-version = "0.4.0"
+version = "0.5.0"
 description = "A GOV.UK Notify flavoured Django email backend"
 authors = ["Nick Smith <nick.smith@torchbox.com>"]
 readme = "README.md"
 homepage = "https://github.com/nimasmi/django-gov-notify"
 repository = "https://github.com/nimasmi/django-gov-notify"
 keywords = ["email", "Django"]
 classifiers = [
@@ -22,22 +22,25 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 license = "BSD-2-Clause"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
-django = ">=3.2,<5.0"
+python = ">=3.8,<3.13"
+django = [
+    {version = ">=3.2", python = ">=3.8,<3.13"},
+    {version = ">=5.0", python = ">=3.10,<3.13"},
+]
 notifications-python-client = "^8.1.0"
 
 [tool.poetry.dev-dependencies]
 black = "^23.10.1"
 isort = "^5.12.0"
 flake8 = "^5.0.4"
 pre-commit = "^3.5.0"
 detect-secrets = "1.4.0"
 factory-boy = "^3.2.0"
 
 [build-system]
-requires = ["poetry-core>=1.2.0"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `django_gov_notify-0.4.0/PKG-INFO` & `django_gov_notify-0.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: django-gov-notify
-Version: 0.4.0
+Version: 0.5.0
 Summary: A GOV.UK Notify flavoured Django email backend
 Home-page: https://github.com/nimasmi/django-gov-notify
 License: BSD-2-Clause
 Keywords: email,Django
 Author: Nick Smith
 Author-email: nick.smith@torchbox.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8,<3.13
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Communications :: Email
-Requires-Dist: django (>=3.2,<5.0)
+Requires-Dist: django (>=3.2) ; python_version >= "3.8" and python_version < "3.13"
+Requires-Dist: django (>=5.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: notifications-python-client (>=8.1.0,<9.0.0)
 Project-URL: Repository, https://github.com/nimasmi/django-gov-notify
 Description-Content-Type: text/markdown
 
 # django-gov-notify, a GOV.UK Notify flavoured Django email backend
 
 ![GitHub workflow](https://github.com/nimasmi/django-gov-notify/actions/workflows/CI-tests.yml/badge.svg)
```

