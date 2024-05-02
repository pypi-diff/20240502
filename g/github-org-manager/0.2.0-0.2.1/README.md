# Comparing `tmp/github_org_manager-0.2.0.tar.gz` & `tmp/github_org_manager-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_org_manager-0.2.0.tar", max compression
+gzip compressed data, was "github_org_manager-0.2.1.tar", max compression
```

## Comparing `github_org_manager-0.2.0.tar` & `github_org_manager-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11361 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/LICENSE.txt
-drwxr-xr-x   0        0        0        0 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/LICENSES/
--rw-r--r--   0        0        0    11361 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0        0        0    17023 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0        0        0     7048 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0        0        0     1078 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/LICENSES/MIT.txt
--rw-r--r--   0        0        0     3645 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/README.md
--rw-r--r--   0        0        0      597 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/gh_org_mgr/__init__.py
--rw-r--r--   0        0        0     4022 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/gh_org_mgr/_config.py
--rw-r--r--   0        0        0      794 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/gh_org_mgr/_gh_api.py
--rw-r--r--   0        0        0    17581 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/gh_org_mgr/_gh_org.py
--rw-r--r--   0        0        0     2121 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/gh_org_mgr/manage.py
--rw-r--r--   0        0        0      923 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4199 1970-01-01 00:00:00.000000 github_org_manager-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11361 2024-05-02 07:59:49.270486 github_org_manager-0.2.1/LICENSE.txt
+drwxr-xr-x   0        0        0        0 2024-05-02 07:59:49.270486 github_org_manager-0.2.1/LICENSES/
+-rw-r--r--   0        0        0    11361 2024-05-02 07:59:49.270486 github_org_manager-0.2.1/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0    17023 2024-05-02 07:59:49.270486 github_org_manager-0.2.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0        0        0     7048 2024-05-02 07:59:49.270486 github_org_manager-0.2.1/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0     1078 2024-05-02 07:59:49.270486 github_org_manager-0.2.1/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     3645 2024-05-02 07:59:49.270486 github_org_manager-0.2.1/README.md
+-rw-r--r--   0        0        0      597 2024-05-02 07:59:49.274486 github_org_manager-0.2.1/gh_org_mgr/__init__.py
+-rw-r--r--   0        0        0     4022 2024-05-02 07:59:49.274486 github_org_manager-0.2.1/gh_org_mgr/_config.py
+-rw-r--r--   0        0        0      794 2024-05-02 07:59:49.274486 github_org_manager-0.2.1/gh_org_mgr/_gh_api.py
+-rw-r--r--   0        0        0    17581 2024-05-02 07:59:49.274486 github_org_manager-0.2.1/gh_org_mgr/_gh_org.py
+-rw-r--r--   0        0        0     2121 2024-05-02 07:59:49.274486 github_org_manager-0.2.1/gh_org_mgr/manage.py
+-rw-r--r--   0        0        0     1419 2024-05-02 07:59:49.274486 github_org_manager-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4787 1970-01-01 00:00:00.000000 github_org_manager-0.2.1/PKG-INFO
```

### Comparing `github_org_manager-0.2.0/LICENSE.txt` & `github_org_manager-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `github_org_manager-0.2.0/LICENSES/Apache-2.0.txt` & `github_org_manager-0.2.1/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `github_org_manager-0.2.0/LICENSES/CC-BY-4.0.txt` & `github_org_manager-0.2.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `github_org_manager-0.2.0/LICENSES/CC0-1.0.txt` & `github_org_manager-0.2.1/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `github_org_manager-0.2.0/LICENSES/MIT.txt` & `github_org_manager-0.2.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `github_org_manager-0.2.0/README.md` & `github_org_manager-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `github_org_manager-0.2.0/gh_org_mgr/__init__.py` & `github_org_manager-0.2.1/gh_org_mgr/__init__.py`

 * *Files identical despite different names*

### Comparing `github_org_manager-0.2.0/gh_org_mgr/_config.py` & `github_org_manager-0.2.1/gh_org_mgr/_config.py`

 * *Files identical despite different names*

### Comparing `github_org_manager-0.2.0/gh_org_mgr/_gh_api.py` & `github_org_manager-0.2.1/gh_org_mgr/_gh_api.py`

 * *Files identical despite different names*

### Comparing `github_org_manager-0.2.0/gh_org_mgr/_gh_org.py` & `github_org_manager-0.2.1/gh_org_mgr/_gh_org.py`

 * *Files identical despite different names*

### Comparing `github_org_manager-0.2.0/gh_org_mgr/manage.py` & `github_org_manager-0.2.1/gh_org_mgr/manage.py`

 * *Files identical despite different names*

### Comparing `github_org_manager-0.2.0/PKG-INFO` & `github_org_manager-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 Metadata-Version: 2.1
 Name: github-org-manager
-Version: 0.2.0
+Version: 0.2.1
 Summary: Manage a GitHub Organization, its teams, repository permissions, and more
+Home-page: https://github.com/OpenRailAssociation/openrail-org-config
+License: Apache-2.0
+Keywords: github,github-management,permissions,access-control
 Author: Max Mehl
 Author-email: max.mehl@deutschebahn.com
 Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Version Control :: Git
+Classifier: Topic :: Utilities
 Requires-Dist: pygithub (>=2.3.0,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Project-URL: Repository, https://github.com/OpenRailAssociation/openrail-org-config
 Description-Content-Type: text/markdown
 
 <!--
 SPDX-FileCopyrightText: 2024 DB Systel GmbH
 
 SPDX-License-Identifier: Apache-2.0
 -->
```

