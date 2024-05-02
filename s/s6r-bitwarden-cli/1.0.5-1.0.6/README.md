# Comparing `tmp/s6r-bitwarden-cli-1.0.5.tar.gz` & `tmp/s6r_bitwarden_cli-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s6r-bitwarden-cli-1.0.5.tar", last modified: Tue Jan 23 14:20:07 2024, max compression
+gzip compressed data, was "s6r_bitwarden_cli-1.0.6.tar", last modified: Thu May  2 08:18:52 2024, max compression
```

## Comparing `s6r-bitwarden-cli-1.0.5.tar` & `s6r_bitwarden_cli-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 14:20:07.408573 s6r-bitwarden-cli-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-01-23 14:19:58.000000 s6r-bitwarden-cli-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-01-23 14:20:07.404574 s6r-bitwarden-cli-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-01-23 14:19:58.000000 s6r-bitwarden-cli-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-01-23 14:19:58.000000 s6r-bitwarden-cli-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-23 14:20:07.408573 s6r-bitwarden-cli-1.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 14:20:07.404574 s6r-bitwarden-cli-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 14:20:07.404574 s6r-bitwarden-cli-1.0.5/src/s6r_bitwarden_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-23 14:19:58.000000 s6r-bitwarden-cli-1.0.5/src/s6r_bitwarden_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-01-23 14:19:58.000000 s6r-bitwarden-cli-1.0.5/src/s6r_bitwarden_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-01-23 14:19:58.000000 s6r-bitwarden-cli-1.0.5/src/s6r_bitwarden_cli/bitwarden.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 14:20:07.404574 s6r-bitwarden-cli-1.0.5/src/s6r_bitwarden_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-01-23 14:20:07.000000 s6r-bitwarden-cli-1.0.5/src/s6r_bitwarden_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-01-23 14:20:07.000000 s6r-bitwarden-cli-1.0.5/src/s6r_bitwarden_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 14:20:07.000000 s6r-bitwarden-cli-1.0.5/src/s6r_bitwarden_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-23 14:20:07.000000 s6r-bitwarden-cli-1.0.5/src/s6r_bitwarden_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-23 14:20:07.000000 s6r-bitwarden-cli-1.0.5/src/s6r_bitwarden_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-23 14:20:07.000000 s6r-bitwarden-cli-1.0.5/src/s6r_bitwarden_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:18:52.856915 s6r_bitwarden_cli-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-02 08:18:42.000000 s6r_bitwarden_cli-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14936 2024-05-02 08:18:52.856915 s6r_bitwarden_cli-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-05-02 08:18:42.000000 s6r_bitwarden_cli-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-02 08:18:42.000000 s6r_bitwarden_cli-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 08:18:52.856915 s6r_bitwarden_cli-1.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:18:52.852915 s6r_bitwarden_cli-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:18:52.856915 s6r_bitwarden_cli-1.0.6/src/s6r_bitwarden_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 08:18:42.000000 s6r_bitwarden_cli-1.0.6/src/s6r_bitwarden_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-02 08:18:42.000000 s6r_bitwarden_cli-1.0.6/src/s6r_bitwarden_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-05-02 08:18:42.000000 s6r_bitwarden_cli-1.0.6/src/s6r_bitwarden_cli/bitwarden.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:18:52.856915 s6r_bitwarden_cli-1.0.6/src/s6r_bitwarden_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14936 2024-05-02 08:18:52.000000 s6r_bitwarden_cli-1.0.6/src/s6r_bitwarden_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-02 08:18:52.000000 s6r_bitwarden_cli-1.0.6/src/s6r_bitwarden_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 08:18:52.000000 s6r_bitwarden_cli-1.0.6/src/s6r_bitwarden_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 08:18:52.000000 s6r_bitwarden_cli-1.0.6/src/s6r_bitwarden_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-02 08:18:52.000000 s6r_bitwarden_cli-1.0.6/src/s6r_bitwarden_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 08:18:52.000000 s6r_bitwarden_cli-1.0.6/src/s6r_bitwarden_cli.egg-info/top_level.txt
```

### Comparing `s6r-bitwarden-cli-1.0.5/LICENSE` & `s6r_bitwarden_cli-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `s6r-bitwarden-cli-1.0.5/PKG-INFO` & `s6r_bitwarden_cli-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s6r-bitwarden-cli
-Version: 1.0.5
+Version: 1.0.6
 Summary: Interact easily with Bitwarden client
 Author-email: Michel Perrocheau <michel@scalizer.fr>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -217,14 +217,21 @@
 
 ## Installation
 
 ```bash
     pip install s6r-bitwarden-cli
 ```
 
+Make sure you have already logged for the first time with `bw`:
+
+```bash
+bw login
+```
+
+
 ### Install Bitwarden CLI
 
 Make sure to install the Bitwarden CLI tool on your system. 
 You can download it from the official Bitwarden website or use your package manager.
 
 [Download and install](https://bitwarden.com/help/cli/#download-and-install)
 
@@ -300,14 +307,20 @@
 
 # Search for Bitwarden items
 items = bw.search_objects(objects='items', search='keyword')
 
 # Retrieve details of a Bitwarden item
 item_details = bw.get_item(name='item_name')
 
+# Get username of a Bitwarden item
+username = bw.get_item_username(name='item_name')
+
+# Get value of a custom field of a Bitwarden item
+my_custom_field = bw.get_item_field(name='item_name', field_name='my_custom_field')
+
 # Get a list of Bitwarden organizations
 organizations = bw.get_organizations()
 
 # Get the default organization
 default_organization = bw.get_default_organization()
 
 # Get the ID of the default organization
```

### Comparing `s6r-bitwarden-cli-1.0.5/README.md` & `s6r_bitwarden_cli-1.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,21 @@
 
 ## Installation
 
 ```bash
     pip install s6r-bitwarden-cli
 ```
 
+Make sure you have already logged for the first time with `bw`:
+
+```bash
+bw login
+```
+
+
 ### Install Bitwarden CLI
 
 Make sure to install the Bitwarden CLI tool on your system. 
 You can download it from the official Bitwarden website or use your package manager.
 
 [Download and install](https://bitwarden.com/help/cli/#download-and-install)
 
@@ -113,14 +120,20 @@
 
 # Search for Bitwarden items
 items = bw.search_objects(objects='items', search='keyword')
 
 # Retrieve details of a Bitwarden item
 item_details = bw.get_item(name='item_name')
 
+# Get username of a Bitwarden item
+username = bw.get_item_username(name='item_name')
+
+# Get value of a custom field of a Bitwarden item
+my_custom_field = bw.get_item_field(name='item_name', field_name='my_custom_field')
+
 # Get a list of Bitwarden organizations
 organizations = bw.get_organizations()
 
 # Get the default organization
 default_organization = bw.get_default_organization()
 
 # Get the ID of the default organization
@@ -161,8 +174,8 @@
 This software is maintained by [Scalizer](https://www.scalizer.fr).
 
 
 <div style="text-align: center;">
 
 [![Scaliser](./logo_scalizer.png)](https://www.scalizer.fr)
 
-</div>
+</div>
```

### Comparing `s6r-bitwarden-cli-1.0.5/pyproject.toml` & `s6r_bitwarden_cli-1.0.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "s6r-bitwarden-cli"
-version = "1.0.5"
+version = "1.0.6"
 description = "Interact easily with Bitwarden client"
 readme = "README.md"
 authors = [{ name = "Michel Perrocheau", email = "michel@scalizer.fr" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Programming Language :: Python",
```

### Comparing `s6r-bitwarden-cli-1.0.5/src/s6r_bitwarden_cli/bitwarden.py` & `s6r_bitwarden_cli-1.0.6/src/s6r_bitwarden_cli/bitwarden.py`

 * *Files 8% similar despite different names*

```diff
@@ -150,18 +150,35 @@
 
     def get_item_login(self, name, organization_id='', collection_id='', collection_name=''):
         res = self.get_item(name, organization_id, collection_id, collection_name)
         if res and isinstance(res, dict):
             return res.get('login', {})
         return {}
 
+    def get_item_fields(self, name, organization_id='', collection_id='', collection_name=''):
+        res = self.get_item(name, organization_id, collection_id, collection_name)
+        if res and isinstance(res, dict):
+            return res.get('fields', [])
+        return []
+
+    def get_item_field(self, name, field_name, organization_id='', collection_id='', collection_name=''):
+        fields = self.get_item_fields(name, organization_id, collection_id, collection_name)
+        for field in fields:
+            if field.get('name') == field_name:
+                return field.get('value', '')
+        return ''
+
     def get_item_password(self, name, organization_id='', collection_id='', collection_name=''):
         res = self.get_item_login(name, organization_id, collection_id, collection_name)
         return res.get('password', '')
 
+    def get_item_username(self, name, organization_id='', collection_id='', collection_name=''):
+        res = self.get_item_login(name, organization_id, collection_id, collection_name)
+        return res.get('username', '')
+
     def get_organizations(self):
         return self.search_objects('organizations')
 
     def get_default_organization(self):
         organizations = self.get_organizations()
         return organizations[0] if organizations else False
```

### Comparing `s6r-bitwarden-cli-1.0.5/src/s6r_bitwarden_cli.egg-info/PKG-INFO` & `s6r_bitwarden_cli-1.0.6/src/s6r_bitwarden_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s6r-bitwarden-cli
-Version: 1.0.5
+Version: 1.0.6
 Summary: Interact easily with Bitwarden client
 Author-email: Michel Perrocheau <michel@scalizer.fr>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -217,14 +217,21 @@
 
 ## Installation
 
 ```bash
     pip install s6r-bitwarden-cli
 ```
 
+Make sure you have already logged for the first time with `bw`:
+
+```bash
+bw login
+```
+
+
 ### Install Bitwarden CLI
 
 Make sure to install the Bitwarden CLI tool on your system. 
 You can download it from the official Bitwarden website or use your package manager.
 
 [Download and install](https://bitwarden.com/help/cli/#download-and-install)
 
@@ -300,14 +307,20 @@
 
 # Search for Bitwarden items
 items = bw.search_objects(objects='items', search='keyword')
 
 # Retrieve details of a Bitwarden item
 item_details = bw.get_item(name='item_name')
 
+# Get username of a Bitwarden item
+username = bw.get_item_username(name='item_name')
+
+# Get value of a custom field of a Bitwarden item
+my_custom_field = bw.get_item_field(name='item_name', field_name='my_custom_field')
+
 # Get a list of Bitwarden organizations
 organizations = bw.get_organizations()
 
 # Get the default organization
 default_organization = bw.get_default_organization()
 
 # Get the ID of the default organization
```

