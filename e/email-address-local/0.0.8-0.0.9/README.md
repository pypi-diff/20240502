# Comparing `tmp/email-address-local-0.0.8.tar.gz` & `tmp/email-address-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "email-address-local-0.0.8.tar", last modified: Tue Oct 24 12:22:58 2023, max compression
+gzip compressed data, was "email-address-local-0.0.9.tar", last modified: Wed Oct 25 10:00:50 2023, max compression
```

## Comparing `email-address-local-0.0.8.tar` & `email-address-local-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 12:22:58.899444 email-address-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2023-10-24 12:22:58.899444 email-address-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-24 12:22:35.000000 email-address-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 12:22:58.895444 email-address-local-0.0.8/email_address_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 12:22:58.899444 email-address-local-0.0.8/email_address_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2023-10-24 12:22:35.000000 email-address-local-0.0.8/email_address_local/src/email_address.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 12:22:58.899444 email-address-local-0.0.8/email_address_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2023-10-24 12:22:58.000000 email-address-local-0.0.8/email_address_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-10-24 12:22:58.000000 email-address-local-0.0.8/email_address_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-24 12:22:58.000000 email-address-local-0.0.8/email_address_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-10-24 12:22:58.000000 email-address-local-0.0.8/email_address_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-24 12:22:58.000000 email-address-local-0.0.8/email_address_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      463 2023-10-24 12:22:35.000000 email-address-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-24 12:22:58.899444 email-address-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      885 2023-10-24 12:22:35.000000 email-address-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 10:00:50.480523 email-address-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2023-10-25 10:00:50.476523 email-address-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-25 10:00:22.000000 email-address-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 10:00:50.476523 email-address-local-0.0.9/email_address_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 10:00:50.476523 email-address-local-0.0.9/email_address_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2023-10-25 10:00:22.000000 email-address-local-0.0.9/email_address_local/src/email_address.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 10:00:50.476523 email-address-local-0.0.9/email_address_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2023-10-25 10:00:50.000000 email-address-local-0.0.9/email_address_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2023-10-25 10:00:50.000000 email-address-local-0.0.9/email_address_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-25 10:00:50.000000 email-address-local-0.0.9/email_address_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-10-25 10:00:50.000000 email-address-local-0.0.9/email_address_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-25 10:00:50.000000 email-address-local-0.0.9/email_address_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2023-10-25 10:00:22.000000 email-address-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-25 10:00:50.480523 email-address-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2023-10-25 10:00:22.000000 email-address-local-0.0.9/setup.py
```

### Comparing `email-address-local-0.0.8/email_address_local/src/email_address.py` & `email-address-local-0.0.9/email_address_local/src/email_address.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,64 +22,60 @@
 }
 logger = Logger.create_logger(object=object1)
 
 
 class EmailAddress(GenericCRUD):
 
     def __init__(self) -> None:
-        pass
-    @staticmethod
-    def insert(email_address: str, lang_code: lang_code.LangCode, name: str) -> int or None:
+        super().__init__(EMAIL_ADDRESS_SCHEMA_NAME)
+
+    def insert_email_adress(self, email_address: str, lang_code: lang_code.LangCode, name: str) -> int or None:
         logger.start(object={"email_address": email_address,
                      "lang_code": lang_code.value, "name": name})
         data = {
             EMAIL_COLLUMN_NAME: f'{email_address}',
         }
-        email_address_id = GenericCRUD(schema_name=EMAIL_ADDRESS_SCHEMA_NAME).insert(
+        email_address_id = self.insert(
             table_name=EMAIL_ADDRESS_TABLE_NAME, json_data=data)
         data = {
             "email_id": email_address_id,
             "lang_code": f'{lang_code.value}',
             "name": f'{name}'
         }
-        GenericCRUD(schema_name=EMAIL_ADDRESS_SCHEMA_NAME).insert(
+        self.insert(
             table_name=EMAIL_ADRESS_ML_TABLE_NAME, json_data=data)
         logger.end(object={'email_address_id': email_address_id})
         return email_address_id
 
-    @staticmethod
-    def update(email_address_id: int, new_email: str) -> None:
+    def update_email_adress(self, email_address_id: int, new_email: str) -> None:
         logger.start(
             object={"email_address_id": email_address_id, "new_email": new_email})
         data = {"email": new_email}
-        GenericCRUD(schema_name=EMAIL_ADDRESS_SCHEMA_NAME).update(table_name=EMAIL_ADDRESS_TABLE_NAME,
-                                                                  json_data=data, id_column_name="email_address_id", id_column_value=email_address_id, where='')
+        self.update(table_name=EMAIL_ADDRESS_TABLE_NAME,
+                    json_data=data, id_column_name="email_address_id", id_column_value=email_address_id, where='')
         logger.end(object={})
 
-    @staticmethod
-    def delete(email_address_id: int) -> None:
+    def delete(self, email_address_id: int) -> None:
         logger.start(object={"email_id": email_address_id})
-        GenericCRUD(schema_name=EMAIL_ADDRESS_SCHEMA_NAME).delete_by_where(table_name=EMAIL_ADDRESS_TABLE_NAME,
-                                                                           where=f"{EMAIL_ADDRESS_ID_COLLUMN_NAME}={email_address_id}")
+        self.delete_by_where(table_name=EMAIL_ADDRESS_TABLE_NAME,
+                             where=f"{EMAIL_ADDRESS_ID_COLLUMN_NAME}={email_address_id}")
         logger.end(object={})
 
-    @staticmethod
-    def get_email_address_by_email_address_id(email_address_id: int) -> str or None:
+    def get_email_address_by_email_address_id(self, email_address_id: int) -> str or None:
         logger.start(object={"email_address_id":  email_address_id})
         email_address = None
-        result = GenericCRUD(schema_name=EMAIL_ADDRESS_SCHEMA_NAME).select_multi_by_id(view_table_name=EMAIL_ADDRESS_VIEW, select_clause_value=
-            EMAIL_COLLUMN_NAME, id_column_name=EMAIL_ADDRESS_ID_COLLUMN_NAME, id_column_value=email_address_id)
+        result = self.select_multi_by_id(view_table_name=EMAIL_ADDRESS_VIEW, select_clause_value=EMAIL_COLLUMN_NAME,
+                                         id_column_name=EMAIL_ADDRESS_ID_COLLUMN_NAME, id_column_value=email_address_id)
         if result:
             email_address = result[0][0]
         logger.end(object={'email_address': email_address})
         return email_address
 
-    @staticmethod
-    def get_email_address_id_by_email_address(email: str) -> int or None:
+    def get_email_address_id_by_email_address(self, email: str) -> int or None:
         email_address_id = None
         logger.start(object={"email": email})
-        result = GenericCRUD(schema_name=EMAIL_ADDRESS_SCHEMA_NAME).select_multi_by_where(view_table_name=EMAIL_ADDRESS_VIEW, select_clause_value=
-            EMAIL_ADDRESS_ID_COLLUMN_NAME, where=f"{EMAIL_COLLUMN_NAME}='{email}'")
+        result = self.select_multi_by_where(
+            view_table_name=EMAIL_ADDRESS_VIEW, select_clause_value=EMAIL_ADDRESS_ID_COLLUMN_NAME, where=f"{EMAIL_COLLUMN_NAME}='{email}'")
         if result:
             email_address_id = result[0][0]
         logger.end(object={'email_address_id': email_address_id})
         return email_address_id
```

### Comparing `email-address-local-0.0.8/setup.py` & `email-address-local-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 with open('README.md') as f:
     readme = f.read()
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/queue-local
-    version='0.0.8',
+    version='0.0.9',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description=readme,
```

