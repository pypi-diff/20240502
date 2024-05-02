# Comparing `tmp/sqlitewithoutsql-1.0.tar.gz` & `tmp/sqlitewithoutsql-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlitewithoutsql-1.0.tar", last modified: Sun Mar 24 10:31:50 2024, max compression
+gzip compressed data, was "sqlitewithoutsql-1.1.0.tar", last modified: Thu May  2 18:11:19 2024, max compression
```

## Comparing `sqlitewithoutsql-1.0.tar` & `sqlitewithoutsql-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-24 10:31:50.869680 sqlitewithoutsql-1.0/
--rw-rw-rw-   0        0        0      221 2024-03-24 10:31:50.868681 sqlitewithoutsql-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1377 2024-03-24 10:23:52.000000 sqlitewithoutsql-1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-03-24 10:31:50.871679 sqlitewithoutsql-1.0/setup.cfg
--rw-rw-rw-   0        0        0      260 2024-03-24 10:30:56.000000 sqlitewithoutsql-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-24 10:31:50.848699 sqlitewithoutsql-1.0/sqlitewithoutsql/
--rw-rw-rw-   0        0        0       92 2024-03-24 09:06:21.000000 sqlitewithoutsql-1.0/sqlitewithoutsql/__init__.py
--rw-rw-rw-   0        0        0     2882 2024-03-24 10:12:34.000000 sqlitewithoutsql-1.0/sqlitewithoutsql/database.py
--rw-rw-rw-   0        0        0      123 2024-03-24 10:10:45.000000 sqlitewithoutsql-1.0/sqlitewithoutsql/sqltype.py
-drwxrwxrwx   0        0        0        0 2024-03-24 10:31:50.867683 sqlitewithoutsql-1.0/sqlitewithoutsql.egg-info/
--rw-rw-rw-   0        0        0      221 2024-03-24 10:31:50.000000 sqlitewithoutsql-1.0/sqlitewithoutsql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-03-24 10:31:50.000000 sqlitewithoutsql-1.0/sqlitewithoutsql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-24 10:31:50.000000 sqlitewithoutsql-1.0/sqlitewithoutsql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-03-24 10:31:50.000000 sqlitewithoutsql-1.0/sqlitewithoutsql.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 18:11:19.211732 sqlitewithoutsql-1.1.0/
+-rw-rw-rw-   0        0        0    35149 2024-03-24 10:34:52.000000 sqlitewithoutsql-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      245 2024-05-02 18:11:19.210662 sqlitewithoutsql-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1408 2024-03-24 10:34:52.000000 sqlitewithoutsql-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-02 18:11:19.214663 sqlitewithoutsql-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      306 2024-05-02 18:09:32.000000 sqlitewithoutsql-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 18:11:19.179661 sqlitewithoutsql-1.1.0/sqlitewithoutsql/
+-rw-rw-rw-   0        0        0       94 2024-05-02 18:06:03.000000 sqlitewithoutsql-1.1.0/sqlitewithoutsql/__init__.py
+-rw-rw-rw-   0        0        0     2883 2024-05-02 18:06:14.000000 sqlitewithoutsql-1.1.0/sqlitewithoutsql/database.py
+-rw-rw-rw-   0        0        0      121 2024-03-24 10:34:52.000000 sqlitewithoutsql-1.1.0/sqlitewithoutsql/sqltype.py
+drwxrwxrwx   0        0        0        0 2024-05-02 18:11:19.209661 sqlitewithoutsql-1.1.0/sqlitewithoutsql.egg-info/
+-rw-rw-rw-   0        0        0      245 2024-05-02 18:11:19.000000 sqlitewithoutsql-1.1.0/sqlitewithoutsql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-05-02 18:11:19.000000 sqlitewithoutsql-1.1.0/sqlitewithoutsql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 18:11:19.000000 sqlitewithoutsql-1.1.0/sqlitewithoutsql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-02 18:11:19.000000 sqlitewithoutsql-1.1.0/sqlitewithoutsql.egg-info/top_level.txt
```

### Comparing `sqlitewithoutsql-1.0/sqlitewithoutsql/database.py` & `sqlitewithoutsql-1.1.0/sqlitewithoutsql/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any
 import sqlite3
-from sqltype import Sqltype
+from .sqltype import Sqltype
 
 class Database:
     def __init__(self, path: str):
         """Connect to the sqlite database
         
         Ps: If you haven't any database, just create a .db file"""
```

