# Comparing `tmp/cim_11_certic-0.6.0.tar.gz` & `tmp/cim_11_certic-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cim_11_certic-0.6.0.tar", max compression
+gzip compressed data, was "cim_11_certic-0.6.1.tar", max compression
```

## Comparing `cim_11_certic-0.6.0.tar` & `cim_11_certic-0.6.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3448 2023-12-18 17:23:25.585872 cim_11_certic-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     1823 2024-03-12 12:11:37.118412 cim_11_certic-0.6.0/README.md
--rw-r--r--   0        0        0     8931 2024-05-01 10:05:28.579052 cim_11_certic-0.6.0/cim_11/__init__.py
--rw-r--r--   0        0        0 11919360 2024-03-12 10:47:06.046802 cim_11_certic-0.6.0/cim_11/cim-11.sqlite3
--rw-r--r--   0        0        0   403379 2024-05-01 09:48:10.188567 cim_11_certic-0.6.0/cim_11/stopwords.py
--rw-r--r--   0        0        0      534 2024-05-01 09:54:19.725552 cim_11_certic-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 cim_11_certic-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     3448 2023-12-18 17:23:25.585872 cim_11_certic-0.6.1/LICENSE.txt
+-rw-r--r--   0        0        0     1823 2024-03-12 12:11:37.118412 cim_11_certic-0.6.1/README.md
+-rw-r--r--   0        0        0     8967 2024-05-01 10:15:14.895597 cim_11_certic-0.6.1/cim_11/__init__.py
+-rw-r--r--   0        0        0 11919360 2024-03-12 10:47:06.046802 cim_11_certic-0.6.1/cim_11/cim-11.sqlite3
+-rw-r--r--   0        0        0   403379 2024-05-01 09:48:10.188567 cim_11_certic-0.6.1/cim_11/stopwords.py
+-rw-r--r--   0        0        0      534 2024-05-01 10:16:42.067241 cim_11_certic-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 cim_11_certic-0.6.1/PKG-INFO
```

### Comparing `cim_11_certic-0.6.0/LICENSE.txt` & `cim_11_certic-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cim_11_certic-0.6.0/README.md` & `cim_11_certic-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `cim_11_certic-0.6.0/cim_11/__init__.py` & `cim_11_certic-0.6.1/cim_11/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,16 @@
                 (self.parent_idc_id,),
             ):
                 return Concept(row[0], row[1], row[2], row[3], row[4])
 
     def __str__(self):
         if self.icode:
             return f"{self.icode} {self.label}"
+        else:
+            return ""
 
 
 def all_concepts() -> Iterator[Concept]:
     with _db_cursor() as cursor:
         for row in cursor.execute(
             "SELECT idc_id, icode, label, parent_idc_id, label_en from cim11"
         ):
```

### Comparing `cim_11_certic-0.6.0/cim_11/cim-11.sqlite3` & `cim_11_certic-0.6.1/cim_11/cim-11.sqlite3`

 * *Files identical despite different names*

### Comparing `cim_11_certic-0.6.0/cim_11/stopwords.py` & `cim_11_certic-0.6.1/cim_11/stopwords.py`

 * *Files identical despite different names*

### Comparing `cim_11_certic-0.6.0/pyproject.toml` & `cim_11_certic-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cim-11-CERTIC"
-version = "0.6.0"
+version = "0.6.1"
 description = "Classification Internationale des Maladies Onzième Révision en français. Données OMS."
 authors = ["Mickaël Desfrênes <mickael.desfrenes@unicaen.fr>", "Arnaud Daret <arnaud.daret@unicaen.fr>"]
 readme = "README.md"
 license = "LICENSE.txt"
 packages = [{include = "cim_11"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cim_11_certic-0.6.0/PKG-INFO` & `cim_11_certic-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cim-11-CERTIC
-Version: 0.6.0
+Version: 0.6.1
 Summary: Classification Internationale des Maladies Onzième Révision en français. Données OMS.
 License: LICENSE.txt
 Author: Mickaël Desfrênes
 Author-email: mickael.desfrenes@unicaen.fr
 Requires-Python: >=3.9
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

