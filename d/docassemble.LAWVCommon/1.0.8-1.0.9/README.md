# Comparing `tmp/docassemble.LAWVCommon-1.0.8.tar.gz` & `tmp/docassemble.LAWVCommon-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docassemble.LAWVCommon-1.0.8.tar", last modified: Thu Apr 25 13:26:15 2024, max compression
+gzip compressed data, was "docassemble.LAWVCommon-1.0.9.tar", last modified: Thu May  2 17:50:41 2024, max compression
```

## Comparing `docassemble.LAWVCommon-1.0.8.tar` & `docassemble.LAWVCommon-1.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-04-25 13:26:15.019010 docassemble.LAWVCommon-1.0.8/
--rw-r--r--   0 www-data    (33) www-data    (33)     1087 2024-04-25 13:26:06.000000 docassemble.LAWVCommon-1.0.8/LICENSE
--rw-r--r--   0 www-data    (33) www-data    (33)       18 2024-04-25 13:26:06.000000 docassemble.LAWVCommon-1.0.8/MANIFEST.in
--rw-r--r--   0 www-data    (33) www-data    (33)      464 2024-04-25 13:26:15.019010 docassemble.LAWVCommon-1.0.8/PKG-INFO
--rw-r--r--   0 www-data    (33) www-data    (33)      104 2024-04-25 13:26:06.000000 docassemble.LAWVCommon-1.0.8/README.md
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-04-25 13:26:15.015010 docassemble.LAWVCommon-1.0.8/docassemble/
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-04-25 13:26:15.019010 docassemble.LAWVCommon-1.0.8/docassemble/LAWVCommon/
--rw-r--r--   0 www-data    (33) www-data    (33)       22 2024-04-25 13:26:06.000000 docassemble.LAWVCommon-1.0.8/docassemble/LAWVCommon/__init__.py
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-04-25 13:26:15.015010 docassemble.LAWVCommon-1.0.8/docassemble/LAWVCommon/data/
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-04-25 13:26:15.019010 docassemble.LAWVCommon-1.0.8/docassemble/LAWVCommon/data/questions/
--rw-r--r--   0 www-data    (33) www-data    (33)    62107 2024-04-25 13:25:10.000000 docassemble.LAWVCommon-1.0.8/docassemble/LAWVCommon/data/questions/common_info.yml
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-04-25 13:26:15.019010 docassemble.LAWVCommon-1.0.8/docassemble/LAWVCommon/data/sources/
--rw-r--r--   0 www-data    (33) www-data    (33)      134 2024-04-25 13:26:06.000000 docassemble.LAWVCommon-1.0.8/docassemble/LAWVCommon/data/sources/README.md
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-04-25 13:26:15.019010 docassemble.LAWVCommon-1.0.8/docassemble/LAWVCommon/data/static/
--rw-r--r--   0 www-data    (33) www-data    (33)      105 2024-04-25 13:26:06.000000 docassemble.LAWVCommon-1.0.8/docassemble/LAWVCommon/data/static/README.md
--rw-r--r--   0 www-data    (33) www-data    (33)      105 2023-09-28 20:16:24.000000 docassemble.LAWVCommon-1.0.8/docassemble/LAWVCommon/data/static/force_lightmode.js
--rw-r--r--   0 www-data    (33) www-data    (33)     3907 2023-09-28 20:16:24.000000 docassemble.LAWVCommon-1.0.8/docassemble/LAWVCommon/data/static/lawv.css
--rw-r--r--   0 www-data    (33) www-data    (33)      204 2023-09-28 20:16:24.000000 docassemble.LAWVCommon-1.0.8/docassemble/LAWVCommon/data/static/progressivedisclosure.css
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-04-25 13:26:15.019010 docassemble.LAWVCommon-1.0.8/docassemble/LAWVCommon/data/templates/
--rw-r--r--   0 www-data    (33) www-data    (33)      102 2024-04-25 13:26:06.000000 docassemble.LAWVCommon-1.0.8/docassemble/LAWVCommon/data/templates/README.md
--rw-r--r--   0 www-data    (33) www-data    (33)   455484 2023-10-04 13:26:38.000000 docassemble.LAWVCommon-1.0.8/docassemble/LAWVCommon/data/templates/civil_case_info.pdf
--rw-r--r--   0 www-data    (33) www-data    (33)     1434 2023-09-28 20:15:54.000000 docassemble.LAWVCommon-1.0.8/docassemble/LAWVCommon/progressivedisclosure.py
--rw-r--r--   0 www-data    (33) www-data    (33)       57 2024-04-25 13:26:06.000000 docassemble.LAWVCommon-1.0.8/docassemble/__init__.py
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-04-25 13:26:15.015010 docassemble.LAWVCommon-1.0.8/docassemble.LAWVCommon.egg-info/
--rw-r--r--   0 www-data    (33) www-data    (33)      464 2024-04-25 13:26:14.000000 docassemble.LAWVCommon-1.0.8/docassemble.LAWVCommon.egg-info/PKG-INFO
--rw-r--r--   0 www-data    (33) www-data    (33)      849 2024-04-25 13:26:14.000000 docassemble.LAWVCommon-1.0.8/docassemble.LAWVCommon.egg-info/SOURCES.txt
--rw-r--r--   0 www-data    (33) www-data    (33)        1 2024-04-25 13:26:14.000000 docassemble.LAWVCommon-1.0.8/docassemble.LAWVCommon.egg-info/dependency_links.txt
--rw-r--r--   0 www-data    (33) www-data    (33)       12 2024-04-25 13:26:14.000000 docassemble.LAWVCommon-1.0.8/docassemble.LAWVCommon.egg-info/namespace_packages.txt
--rw-r--r--   0 www-data    (33) www-data    (33)        1 2024-04-25 13:26:14.000000 docassemble.LAWVCommon-1.0.8/docassemble.LAWVCommon.egg-info/not-zip-safe
--rw-r--r--   0 www-data    (33) www-data    (33)       12 2024-04-25 13:26:14.000000 docassemble.LAWVCommon-1.0.8/docassemble.LAWVCommon.egg-info/top_level.txt
--rw-r--r--   0 www-data    (33) www-data    (33)       79 2024-04-25 13:26:15.023010 docassemble.LAWVCommon-1.0.8/setup.cfg
--rw-r--r--   0 www-data    (33) www-data    (33)     2510 2024-04-25 13:26:06.000000 docassemble.LAWVCommon-1.0.8/setup.py
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-02 17:50:41.177280 docassemble.LAWVCommon-1.0.9/
+-rw-r--r--   0 www-data    (33) www-data    (33)     1087 2024-05-02 17:50:33.000000 docassemble.LAWVCommon-1.0.9/LICENSE
+-rw-r--r--   0 www-data    (33) www-data    (33)       18 2024-05-02 17:50:33.000000 docassemble.LAWVCommon-1.0.9/MANIFEST.in
+-rw-r--r--   0 www-data    (33) www-data    (33)      464 2024-05-02 17:50:41.177280 docassemble.LAWVCommon-1.0.9/PKG-INFO
+-rw-r--r--   0 www-data    (33) www-data    (33)      104 2024-05-02 17:50:33.000000 docassemble.LAWVCommon-1.0.9/README.md
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-02 17:50:41.173280 docassemble.LAWVCommon-1.0.9/docassemble/
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-02 17:50:41.173280 docassemble.LAWVCommon-1.0.9/docassemble/LAWVCommon/
+-rw-r--r--   0 www-data    (33) www-data    (33)       22 2024-05-02 17:50:33.000000 docassemble.LAWVCommon-1.0.9/docassemble/LAWVCommon/__init__.py
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-02 17:50:41.173280 docassemble.LAWVCommon-1.0.9/docassemble/LAWVCommon/data/
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-02 17:50:41.173280 docassemble.LAWVCommon-1.0.9/docassemble/LAWVCommon/data/questions/
+-rw-r--r--   0 www-data    (33) www-data    (33)    62107 2024-04-25 13:25:10.000000 docassemble.LAWVCommon-1.0.9/docassemble/LAWVCommon/data/questions/common_info.yml
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-02 17:50:41.177280 docassemble.LAWVCommon-1.0.9/docassemble/LAWVCommon/data/sources/
+-rw-r--r--   0 www-data    (33) www-data    (33)      134 2024-05-02 17:50:33.000000 docassemble.LAWVCommon-1.0.9/docassemble/LAWVCommon/data/sources/README.md
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-02 17:50:41.177280 docassemble.LAWVCommon-1.0.9/docassemble/LAWVCommon/data/static/
+-rw-r--r--   0 www-data    (33) www-data    (33)      105 2024-05-02 17:50:33.000000 docassemble.LAWVCommon-1.0.9/docassemble/LAWVCommon/data/static/README.md
+-rw-r--r--   0 www-data    (33) www-data    (33)      105 2023-09-28 20:16:24.000000 docassemble.LAWVCommon-1.0.9/docassemble/LAWVCommon/data/static/force_lightmode.js
+-rw-r--r--   0 www-data    (33) www-data    (33)     3907 2023-09-28 20:16:24.000000 docassemble.LAWVCommon-1.0.9/docassemble/LAWVCommon/data/static/lawv.css
+-rw-r--r--   0 www-data    (33) www-data    (33)      204 2023-09-28 20:16:24.000000 docassemble.LAWVCommon-1.0.9/docassemble/LAWVCommon/data/static/progressivedisclosure.css
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-02 17:50:41.177280 docassemble.LAWVCommon-1.0.9/docassemble/LAWVCommon/data/templates/
+-rw-r--r--   0 www-data    (33) www-data    (33)      102 2024-05-02 17:50:33.000000 docassemble.LAWVCommon-1.0.9/docassemble/LAWVCommon/data/templates/README.md
+-rw-r--r--   0 www-data    (33) www-data    (33)   331039 2024-05-02 17:49:45.000000 docassemble.LAWVCommon-1.0.9/docassemble/LAWVCommon/data/templates/civil_case_info.pdf
+-rw-r--r--   0 www-data    (33) www-data    (33)     1434 2023-09-28 20:15:54.000000 docassemble.LAWVCommon-1.0.9/docassemble/LAWVCommon/progressivedisclosure.py
+-rw-r--r--   0 www-data    (33) www-data    (33)       57 2024-05-02 17:50:33.000000 docassemble.LAWVCommon-1.0.9/docassemble/__init__.py
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-02 17:50:41.173280 docassemble.LAWVCommon-1.0.9/docassemble.LAWVCommon.egg-info/
+-rw-r--r--   0 www-data    (33) www-data    (33)      464 2024-05-02 17:50:41.000000 docassemble.LAWVCommon-1.0.9/docassemble.LAWVCommon.egg-info/PKG-INFO
+-rw-r--r--   0 www-data    (33) www-data    (33)      849 2024-05-02 17:50:41.000000 docassemble.LAWVCommon-1.0.9/docassemble.LAWVCommon.egg-info/SOURCES.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)        1 2024-05-02 17:50:41.000000 docassemble.LAWVCommon-1.0.9/docassemble.LAWVCommon.egg-info/dependency_links.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)       12 2024-05-02 17:50:41.000000 docassemble.LAWVCommon-1.0.9/docassemble.LAWVCommon.egg-info/namespace_packages.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)        1 2024-05-02 17:50:41.000000 docassemble.LAWVCommon-1.0.9/docassemble.LAWVCommon.egg-info/not-zip-safe
+-rw-r--r--   0 www-data    (33) www-data    (33)       12 2024-05-02 17:50:41.000000 docassemble.LAWVCommon-1.0.9/docassemble.LAWVCommon.egg-info/top_level.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)       79 2024-05-02 17:50:41.177280 docassemble.LAWVCommon-1.0.9/setup.cfg
+-rw-r--r--   0 www-data    (33) www-data    (33)     2510 2024-05-02 17:50:33.000000 docassemble.LAWVCommon-1.0.9/setup.py
```

### Comparing `docassemble.LAWVCommon-1.0.8/LICENSE` & `docassemble.LAWVCommon-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVCommon-1.0.8/docassemble/LAWVCommon/data/questions/common_info.yml` & `docassemble.LAWVCommon-1.0.9/docassemble/LAWVCommon/data/questions/common_info.yml`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVCommon-1.0.8/docassemble/LAWVCommon/data/static/lawv.css` & `docassemble.LAWVCommon-1.0.9/docassemble/LAWVCommon/data/static/lawv.css`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVCommon-1.0.8/docassemble/LAWVCommon/data/templates/civil_case_info.pdf` & `docassemble.LAWVCommon-1.0.9/docassemble/LAWVCommon/data/templates/civil_case_info.pdf`

 * *Files 24% similar despite different names*

#### Comparing `docassemble.LAWVCommon-1.0.8/docassemble/LAWVCommon/data/templates/civil_case_info.pdf` & `docassemble.LAWVCommon-1.0.9/docassemble/LAWVCommon/data/templates/civil_case_info.pdf`

 * *Document info*

```diff
@@ -1,4 +1,4 @@
 CreationDate: "D:20210910092953-04'00'"
 Creator: 'Adobe Acrobat Pro DC 19.21.20061'
-ModDate: "D:20231004092622-04'00'"
+ModDate: "D:20240502134935-04'00'"
 Producer: 'Adobe Acrobat Pro DC 19.21.20061'
```

#### pdftotext {} -

 * *error from `pdftotext {} -`:*

 * *Syntax Error: Expected the optional content group list, but wasn't able to find it, or it isn't an Array*

```diff
@@ -97,73 +97,8 @@
 copies of complaint enclosed/attached.
 Signature:
 
 SCA-C-100: Civil Case Information Statement (Other than Domestic Relations)
 
 Revision Date: 4/2020
 
-Plaintiff:
-vs.
-Defendant:
-
-, et al
-
-Case Number:
-
-, et al
-
-CIVIL CASE INFORMATION STATEMENT
-DEFENDANT(S) CONTINUATION PAGE
-Defendant's Phone:
-Defendant's Name
-Street Address
-City, State, Zip Code
-Defendant's Name
-Street Address
-City, State, Zip Code
-Defendant's Name
-Street Address
-City, State, Zip Code
-
-Days to Answer:
-Type of Service:
-Defendant's Phone:
-Days to Answer:
-Type of Service:
-Defendant's Phone:
-Days to Answer:
-Type of Service:
-Defendant's Phone:
-
-Defendant's Name
-Street Address
-City, State, Zip Code
-Defendant's Name
-Street Address
-City, State, Zip Code
-Defendant's Name
-Street Address
-City, State, Zip Code
-Defendant's Name
-Street Address
-City, State, Zip Code
-
-Days to Answer:
-Type of Service:
-Defendant's Phone:
-
-Days to Answer:
-Type of Service:
-Defendant's Phone:
-
-Days to Answer:
-Type of Service:
-Defendant's Phone:
-
-Days to Answer:
-Type of Service:
-
-SCA-C-100: Civil Case Information Statement-Defendant(s) Continuation Page
-
-Revision Date: 4/2020
-
```

### Comparing `docassemble.LAWVCommon-1.0.8/docassemble/LAWVCommon/progressivedisclosure.py` & `docassemble.LAWVCommon-1.0.9/docassemble/LAWVCommon/progressivedisclosure.py`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVCommon-1.0.8/docassemble.LAWVCommon.egg-info/SOURCES.txt` & `docassemble.LAWVCommon-1.0.9/docassemble.LAWVCommon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVCommon-1.0.8/setup.py` & `docassemble.LAWVCommon-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                         break
                 if bad_name:
                     continue
                 out.setdefault(package, []).append(prefix+name)
     return out
 
 setup(name='docassemble.LAWVCommon',
-      version='1.0.8',
+      version='1.0.9',
       description=('A docassemble extension for LAWV information used across multiple interviews'),
       long_description='Common information, CSS, and classes used across multiple interviews to retain data consistency for LAWV',
       long_description_content_type='text/markdown',
       author='System Administrator',
       author_email='dhenry@lawv.net',
       license='The MIT License (MIT)',
       url='https://docassemble.org',
```

