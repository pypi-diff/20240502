# Comparing `tmp/contact-email-address-local-0.0.6.tar.gz` & `tmp/contact_email_address_local-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact-email-address-local-0.0.6.tar", last modified: Mon Feb  5 02:09:38 2024, max compression
+gzip compressed data, was "contact_email_address_local-0.0.7.tar", last modified: Thu May  2 03:58:11 2024, max compression
```

## Comparing `contact-email-address-local-0.0.6.tar` & `contact_email_address_local-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:09:38.158589 contact-email-address-local-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-02-05 02:09:38.158589 contact-email-address-local-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-05 02:09:00.000000 contact-email-address-local-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:09:38.150589 contact-email-address-local-0.0.6/contact_email_address_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:09:38.158589 contact-email-address-local-0.0.6/contact_email_address_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 02:09:00.000000 contact-email-address-local-0.0.6/contact_email_address_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-02-05 02:09:00.000000 contact-email-address-local-0.0.6/contact_email_address_local/src/contact_email_addresses_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-02-05 02:09:00.000000 contact-email-address-local-0.0.6/contact_email_address_local/src/contact_email_addresses_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:09:38.158589 contact-email-address-local-0.0.6/contact_email_address_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-02-05 02:09:38.000000 contact-email-address-local-0.0.6/contact_email_address_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-02-05 02:09:38.000000 contact-email-address-local-0.0.6/contact_email_address_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 02:09:38.000000 contact-email-address-local-0.0.6/contact_email_address_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-05 02:09:38.000000 contact-email-address-local-0.0.6/contact_email_address_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-05 02:09:38.000000 contact-email-address-local-0.0.6/contact_email_address_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-02-05 02:09:00.000000 contact-email-address-local-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 02:09:38.158589 contact-email-address-local-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-02-05 02:09:00.000000 contact-email-address-local-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:58:11.047135 contact_email_address_local-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-02 03:58:11.047135 contact_email_address_local-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-02 03:57:46.000000 contact_email_address_local-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:58:11.043135 contact_email_address_local-0.0.7/contact_email_address_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:58:11.047135 contact_email_address_local-0.0.7/contact_email_address_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 03:57:46.000000 contact_email_address_local-0.0.7/contact_email_address_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-02 03:57:46.000000 contact_email_address_local-0.0.7/contact_email_address_local/src/contact_email_addresses_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-02 03:57:46.000000 contact_email_address_local-0.0.7/contact_email_address_local/src/contact_email_addresses_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:58:11.047135 contact_email_address_local-0.0.7/contact_email_address_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-02 03:58:11.000000 contact_email_address_local-0.0.7/contact_email_address_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-02 03:58:11.000000 contact_email_address_local-0.0.7/contact_email_address_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 03:58:11.000000 contact_email_address_local-0.0.7/contact_email_address_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-02 03:58:11.000000 contact_email_address_local-0.0.7/contact_email_address_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-02 03:58:11.000000 contact_email_address_local-0.0.7/contact_email_address_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-02 03:57:46.000000 contact_email_address_local-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 03:58:11.047135 contact_email_address_local-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-02 03:57:46.000000 contact_email_address_local-0.0.7/setup.py
```

### Comparing `contact-email-address-local-0.0.6/contact_email_address_local/src/contact_email_addresses_constants.py` & `contact_email_address_local-0.0.7/contact_email_address_local/src/contact_email_addresses_constants.py`

 * *Files identical despite different names*

### Comparing `contact-email-address-local-0.0.6/contact_email_address_local/src/contact_email_addresses_local.py` & `contact_email_address_local-0.0.7/contact_email_address_local/src/contact_email_addresses_local.py`

 * *Files identical despite different names*

### Comparing `contact-email-address-local-0.0.6/setup.py` & `contact_email_address_local-0.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "contact-email-address-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.6',  # update only the minor version each time # https://pypi.org/project/contact-email-address-local/
+    version='0.0.7',  # update only the minor version each time # https://pypi.org/project/contact-email-address-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles contact-email-address-local Python",
     long_description="PyPI Package for Circles contact-email-address-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/contact-email-address-local-pyhon-package",  # https://pypi.org/project/contact-email-address-local/       # noqa: E501
     packages=[package_dir],
```

