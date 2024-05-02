# Comparing `tmp/flict-1.2.8.tar.gz` & `tmp/flict-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flict-1.2.8.tar", last modified: Tue Feb 13 04:28:22 2024, max compression
+gzip compressed data, was "flict-1.2.9.tar", last modified: Mon Feb 26 14:42:54 2024, max compression
```

## Comparing `flict-1.2.8.tar` & `flict-1.2.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 04:28:22.046248 flict-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-13 04:28:06.000000 flict-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-13 04:28:06.000000 flict-1.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-02-13 04:28:22.046248 flict-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-02-13 04:28:06.000000 flict-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 04:28:22.042248 flict-1.2.8/flict/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-13 04:28:06.000000 flict-1.2.8/flict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11715 2024-02-13 04:28:06.000000 flict-1.2.8/flict/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 04:28:22.042248 flict-1.2.8/flict/flictlib/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-13 04:28:06.000000 flict-1.2.8/flict/flictlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11725 2024-02-13 04:28:06.000000 flict-1.2.8/flict/flictlib/arbiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15806 2024-02-13 04:28:06.000000 flict-1.2.8/flict/flictlib/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-13 04:28:21.000000 flict-1.2.8/flict/flictlib/flict_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 04:28:22.046248 flict-1.2.8/flict/flictlib/format/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 04:28:06.000000 flict-1.2.8/flict/flictlib/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-13 04:28:06.000000 flict-1.2.8/flict/flictlib/format/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-02-13 04:28:06.000000 flict-1.2.8/flict/flictlib/format/dot_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-02-13 04:28:06.000000 flict-1.2.8/flict/flictlib/format/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-02-13 04:28:06.000000 flict-1.2.8/flict/flictlib/format/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-02-13 04:28:06.000000 flict-1.2.8/flict/flictlib/format/json_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-02-13 04:28:06.000000 flict-1.2.8/flict/flictlib/format/markdown_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-02-13 04:28:06.000000 flict-1.2.8/flict/flictlib/format/text_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-02-13 04:28:06.000000 flict-1.2.8/flict/flictlib/lic_comp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-02-13 04:28:06.000000 flict-1.2.8/flict/flictlib/license.py
--rw-r--r--   0 runner    (1001) docker     (127)     8525 2024-02-13 04:28:06.000000 flict-1.2.8/flict/flictlib/license_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-02-13 04:28:06.000000 flict-1.2.8/flict/flictlib/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 04:28:22.046248 flict-1.2.8/flict/flictlib/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 04:28:06.000000 flict-1.2.8/flict/flictlib/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-02-13 04:28:06.000000 flict-1.2.8/flict/flictlib/project/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-02-13 04:28:06.000000 flict-1.2.8/flict/flictlib/return_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-02-13 04:28:06.000000 flict-1.2.8/flict/flictlib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-02-13 04:28:06.000000 flict-1.2.8/flict/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 04:28:22.046248 flict-1.2.8/flict/var/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-02-13 04:28:06.000000 flict-1.2.8/flict/var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17319 2024-02-13 04:28:06.000000 flict-1.2.8/flict/var/alias.json
--rw-r--r--   0 runner    (1001) docker     (127)   457966 2024-02-13 04:28:06.000000 flict-1.2.8/flict/var/scancode-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 04:28:22.042248 flict-1.2.8/flict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-02-13 04:28:22.000000 flict-1.2.8/flict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-02-13 04:28:22.000000 flict-1.2.8/flict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 04:28:22.000000 flict-1.2.8/flict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-13 04:28:22.000000 flict-1.2.8/flict.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-02-13 04:28:22.000000 flict-1.2.8/flict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-13 04:28:22.000000 flict-1.2.8/flict.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-13 04:28:06.000000 flict-1.2.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-13 04:28:06.000000 flict-1.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-02-13 04:28:22.046248 flict-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-02-13 04:28:06.000000 flict-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:42:54.800763 flict-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-26 14:42:35.000000 flict-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-26 14:42:35.000000 flict-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6083 2024-02-26 14:42:54.800763 flict-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-02-26 14:42:35.000000 flict-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:42:54.796763 flict-1.2.9/flict/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-26 14:42:35.000000 flict-1.2.9/flict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-02-26 14:42:35.000000 flict-1.2.9/flict/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:42:54.796763 flict-1.2.9/flict/flictlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-26 14:42:35.000000 flict-1.2.9/flict/flictlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12026 2024-02-26 14:42:35.000000 flict-1.2.9/flict/flictlib/arbiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15806 2024-02-26 14:42:35.000000 flict-1.2.9/flict/flictlib/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-26 14:42:54.000000 flict-1.2.9/flict/flictlib/flict_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:42:54.796763 flict-1.2.9/flict/flictlib/format/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 14:42:35.000000 flict-1.2.9/flict/flictlib/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-26 14:42:35.000000 flict-1.2.9/flict/flictlib/format/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-02-26 14:42:35.000000 flict-1.2.9/flict/flictlib/format/dot_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-02-26 14:42:35.000000 flict-1.2.9/flict/flictlib/format/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-02-26 14:42:35.000000 flict-1.2.9/flict/flictlib/format/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-02-26 14:42:35.000000 flict-1.2.9/flict/flictlib/format/json_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-02-26 14:42:35.000000 flict-1.2.9/flict/flictlib/format/markdown_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-02-26 14:42:35.000000 flict-1.2.9/flict/flictlib/format/text_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-02-26 14:42:35.000000 flict-1.2.9/flict/flictlib/lic_comp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-02-26 14:42:35.000000 flict-1.2.9/flict/flictlib/license.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8525 2024-02-26 14:42:35.000000 flict-1.2.9/flict/flictlib/license_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-02-26 14:42:35.000000 flict-1.2.9/flict/flictlib/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:42:54.800763 flict-1.2.9/flict/flictlib/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 14:42:35.000000 flict-1.2.9/flict/flictlib/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-02-26 14:42:35.000000 flict-1.2.9/flict/flictlib/project/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-02-26 14:42:35.000000 flict-1.2.9/flict/flictlib/return_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-02-26 14:42:35.000000 flict-1.2.9/flict/flictlib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-02-26 14:42:35.000000 flict-1.2.9/flict/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:42:54.800763 flict-1.2.9/flict/var/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-02-26 14:42:35.000000 flict-1.2.9/flict/var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17319 2024-02-26 14:42:35.000000 flict-1.2.9/flict/var/alias.json
+-rw-r--r--   0 runner    (1001) docker     (127)   457966 2024-02-26 14:42:35.000000 flict-1.2.9/flict/var/scancode-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:42:54.796763 flict-1.2.9/flict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6083 2024-02-26 14:42:54.000000 flict-1.2.9/flict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-02-26 14:42:54.000000 flict-1.2.9/flict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 14:42:54.000000 flict-1.2.9/flict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-26 14:42:54.000000 flict-1.2.9/flict.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-02-26 14:42:54.000000 flict-1.2.9/flict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-26 14:42:54.000000 flict-1.2.9/flict.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-26 14:42:35.000000 flict-1.2.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-26 14:42:35.000000 flict-1.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-02-26 14:42:54.800763 flict-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-02-26 14:42:35.000000 flict-1.2.9/setup.py
```

### Comparing `flict-1.2.8/LICENSE` & `flict-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flict-1.2.8/PKG-INFO` & `flict-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: flict
-Version: 1.2.8
+Version: 1.2.9
 Summary: FOSS License Compatibility Tool
 Home-page: https://github.com/vinland-technology/flict
 Author: Henrik Sanklef
 Author-email: hesa@sandklef.com
-License: UNKNOWN
+License: GPL-3.0-or-later
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
```

### Comparing `flict-1.2.8/README.md` & `flict-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `flict-1.2.8/flict/__main__.py` & `flict-1.2.9/flict/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,16 @@
                                         type=str,
                                         dest='license_matrix_file',
                                         help='File with license compatibility matrix, defaults to osadl-matrix database',
                                         default=flict_config.DEFAULT_MATRIX_FILE)
 
     commmon_defaults_group.add_argument('--licenses-denied-file', '-ldf', type=str, dest='licenses_denied_file', help='', default=None)
 
+    commmon_defaults_group.add_argument('--licenses-allowed-file', '-laf', type=str, dest='licenses_allowed_file', help='', default=None)
+
     commmon_defaults_group.add_argument('--licenses-preference-file', '-lpf', type=str, dest='licenses_preference_file', help='', default=None)
 
     commmon_defaults_group.add_argument('--license-info-file', '-lif', type=str, dest='licenses_info_file', help='Short for applying -lmf <file> -ldf <file> -lpf <file>', default=None)
 
     # COMMON
     parser.add_argument('-ip', '--ignore-problems',
                         action='store_true',
```

### Comparing `flict-1.2.8/flict/flictlib/arbiter.py` & `flict-1.2.9/flict/flictlib/arbiter.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,29 +12,34 @@
 from flict.flictlib.license import compatible_license_short
 from flict.flictlib.project.reader import FlictProjectReader
 
 
 class Arbiter:
     """Arbiter is a class to verify compatibility"""
 
-    def __init__(self, license_db=None, licenses_preferences=None, denied_licenses=None, update_dual=True):
+    def __init__(self, license_db=None, licenses_preferences=None, denied_licenses=None, allowed_licenses=None, update_dual=True):
         """Initializes Arbiter objects
              Parameters:
                  license_db: license database to use instead of builtin
                  licenses_preferences: license preferences to use instead of builtin
                  denied_licenses: licenses that cannot be used
+                 allowed_licenses: licenses that are the only ones to be used
         """
         self.update_dual = update_dual
         self.license_compatibility = LicenseCompatibilty(
-            license_db=license_db, licenses_preferences=licenses_preferences, denied_licenses=denied_licenses, update_dual=update_dual)
+            license_db=license_db, licenses_preferences=licenses_preferences, denied_licenses=denied_licenses, allowed_licenses=allowed_licenses, update_dual=update_dual)
 
     def supported_licenses(self):
         """Returns the supported licenses"""
         return self.license_compatibility.supported_licenses()
 
+    def license_allowed(self, lic):
+        """Return whether or not a license is allowed"""
+        return self.license_compatibility.license.license_allowed(lic)
+
     def _verify_package(self, package, licenses):
         """Verifies a package's license to a list of outbounds and returns the
         compatibility between the liceses.
              Parameters:
                  package: the package (with its license) to check for compatibility
                  licenses: the licenses to check the package's license against
         """
```

### Comparing `flict-1.2.8/flict/flictlib/compatibility.py` & `flict-1.2.9/flict/flictlib/compatibility.py`

 * *Files identical despite different names*

### Comparing `flict-1.2.8/flict/flictlib/flict_config.py` & `flict-1.2.9/flict/flictlib/flict_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         except Exception:  # noqa: S110 - it's okay ignore all errors here
             pass
     return {}
 
 
 _userconfig = read_user_config()
 
-flict_version = "1.2.8"
+flict_version = "1.2.9"
 
 SCRIPT_DIR = os.path.realpath(os.path.join(os.path.dirname(os.path.realpath(__file__)), "../"))
 
 VAR_DIR = os.path.join(SCRIPT_DIR, "var")
 
 DEFAULT_MATRIX_FILE = _userconfig.get('matrix-file', OSADL_MATRIX_JSON)
 DEFAULT_OUTPUT_FORMAT = _userconfig.get('output-format', "JSON")
```

### Comparing `flict-1.2.8/flict/flictlib/format/common.py` & `flict-1.2.9/flict/flictlib/format/common.py`

 * *Files identical despite different names*

### Comparing `flict-1.2.8/flict/flictlib/format/dot_format.py` & `flict-1.2.9/flict/flictlib/format/dot_format.py`

 * *Files identical despite different names*

### Comparing `flict-1.2.8/flict/flictlib/format/factory.py` & `flict-1.2.9/flict/flictlib/format/factory.py`

 * *Files identical despite different names*

### Comparing `flict-1.2.8/flict/flictlib/format/format.py` & `flict-1.2.9/flict/flictlib/format/format.py`

 * *Files identical despite different names*

### Comparing `flict-1.2.8/flict/flictlib/format/json_format.py` & `flict-1.2.9/flict/flictlib/format/json_format.py`

 * *Files identical despite different names*

### Comparing `flict-1.2.8/flict/flictlib/format/markdown_format.py` & `flict-1.2.9/flict/flictlib/format/markdown_format.py`

 * *Files identical despite different names*

### Comparing `flict-1.2.8/flict/flictlib/format/text_format.py` & `flict-1.2.9/flict/flictlib/format/text_format.py`

 * *Files identical despite different names*

### Comparing `flict-1.2.8/flict/flictlib/lic_comp.py` & `flict-1.2.9/flict/flictlib/lic_comp.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 from flict.flictlib.return_codes import FlictError, ReturnCodes
 
 COMPATIBILITY_TAG = "compatibility"
 
 
 class LicenseCompatibilty:
 
-    def __init__(self, license_db=None, licenses_preferences=None, denied_licenses=None, update_dual=True):
-        self.license = License(denied_licenses, update_dual)
+    def __init__(self, license_db=None, licenses_preferences=None, denied_licenses=None, allowed_licenses=None, update_dual=True):
+        self.license = License(denied_licenses, allowed_licenses, update_dual)
 
         self.compatibility = CompatibilityFactory.get_compatibility(license_db)
 
         if not licenses_preferences or licenses_preferences == []:
             self.license_chooser = CompatibilityLicenseChooser(self.compatibility.supported_licenses())
         else:
             self.license_chooser = CustomLicenseChooser(licenses_preferences)
```

### Comparing `flict-1.2.8/flict/flictlib/license.py` & `flict-1.2.9/flict/flictlib/license.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,16 +19,22 @@
 class License():
     """Class managing license expressions, e.g.:
     X11
     MIT OR BSD-3-Clause
     GPL-2.0-or-later or (GPL-3.0-only WITH GCC-exception-3.1 AND curl
     """
 
-    def __init__(self, denied_licenses, update_dual=True):
+    def __init__(self, denied_licenses, allowed_licenses, update_dual=True):
         self._denied_licenses = denied_licenses
+        self._allowed_licenses = allowed_licenses
+        # Either denied or allower or none: OK
+        # Both: not OK, raise exception
+        if self._denied_licenses and self._allowed_licenses:
+            raise FlictError(ReturnCodes.RET_CONFLICT_LICENSE_LIST, 'You can only supply either of denied or allowed licenses, not both.')
+
         self.parser = LicenseParserFactory.get_parser()
         self.update_dual = update_dual
 
     def get_license(self, expr):
         return self.parser.parse_license(expr)['license']
 
     def license_name(self, expr):
@@ -42,17 +48,22 @@
 
     def licenses(self, expr):
         return self.parser.licenses(expr)
 
     def denied_licenses(self):
         return self._denied_licenses
 
+    def allowed_licenses(self):
+        return self._allowed_licenses
+
     def license_denied(self, license_):
         if self._denied_licenses:
             return license_ in self._denied_licenses
+        if self._allowed_licenses:
+            return license_ not in self._allowed_licenses
         return False
 
     def license_allowed(self, license_):
         return not self.license_denied(license_)
 
     def simplify_license(self, expr):
         try:
```

### Comparing `flict-1.2.8/flict/flictlib/license_parser.py` & `flict-1.2.9/flict/flictlib/license_parser.py`

 * *Files identical despite different names*

### Comparing `flict-1.2.8/flict/flictlib/logger.py` & `flict-1.2.9/flict/flictlib/logger.py`

 * *Files identical despite different names*

### Comparing `flict-1.2.8/flict/flictlib/project/reader.py` & `flict-1.2.9/flict/flictlib/project/reader.py`

 * *Files identical despite different names*

### Comparing `flict-1.2.8/flict/flictlib/return_codes.py` & `flict-1.2.9/flict/flictlib/return_codes.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     # 9
 
     RET_INVALID_PROJECT = (10, "Invalid project")
     RET_INVALID_EXPRESSSION = (11, "Invalid expression")
     RET_FILE_NOT_FOUND = (12, "File not found")
     RET_INVALID_LICENSE_PREFERENCE = (13, "Invalid license preferences")
     RET_INVALID_MATRIX = (14, "Invalid matrix or matrix extension")
+    RET_CONFLICT_LICENSE_LIST = (15, "Conflicting allowed/denied license lists")
 
     @classmethod
     def get_help(cls, indent="  "):
         """
         Return help string for all defined enum values
         """
         ret = []
```

### Comparing `flict-1.2.8/flict/flictlib/utils.py` & `flict-1.2.9/flict/flictlib/utils.py`

 * *Files identical despite different names*

### Comparing `flict-1.2.8/flict/impl.py` & `flict-1.2.9/flict/impl.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,27 +37,31 @@
         return self._formatter.format_compats(inter_compats)
 
     def simplify(self):
         simplified = self.arbiter.simplify_license(" ".join(self._args.license_expression))
         return self._formatter.format_simplified(simplified)
 
     def suggest_outbound_candidate(self):
+        license_expression = self._args.license_expression
+
         if self._args.extended_licenses:
             licenses = self.arbiter.supported_licenses()
         else:
-            licenses = self.arbiter.licenses(" ".join(self._args.license_expression))
+            license_expression = self.arbiter.simplify_license(" ".join(self._args.license_expression))['simplified']
+            licenses = self.arbiter.licenses(license_expression)
+
+        allowed_licenses = [x for x in licenses if self.arbiter.license_allowed(x)]
+
         outbounds = []
         try:
-            for outbound in licenses:
-                compats = self.arbiter.inbounds_outbound_check(outbound, self._args.license_expression)
-                compat_status = compats['compatibility']
-                if compat_status == "Yes":
+            for outbound in allowed_licenses:
+                compats = self.arbiter.inbounds_outbound_check(outbound, [license_expression])
+                compat = compats['compatibility'] == 'Yes'
+                if compat:
                     outbounds.append(outbound)
-                elif compat_status == "No":
-                    pass
 
             outbounds.sort()
             return self._formatter.format_outbound_license(outbounds)
 
         except Exception as e:
             raise FlictError(ReturnCodes.RET_INVALID_EXPRESSSION,
                              f'Invalid license expression: {self._args.license_expression}. Original cause: {e}')
@@ -77,25 +81,28 @@
             return ret
         else:
             with open(file_name) as fp:
                 return json.load(fp)[object_key]
 
     def _get_arbiter(self):
         licenses_denied_file = self._args.licenses_denied_file
+        licenses_allowed_file = self._args.licenses_allowed_file
         licenses_preference_file = self._args.licenses_preference_file
 
         if self._args.licenses_info_file:
             licenses_denied_file = self._args.licenses_info_file
             licenses_preference_file = self._args.licenses_info_file
 
         licenses_denied = self._read_json_object(licenses_denied_file, "licenses_denied", [])
+        licenses_allowed = self._read_json_object(licenses_allowed_file, "licenses_allowed", [])
         licenses_preferences = self._read_json_object(licenses_preference_file, "license_preferences", [])
         arbiter = Arbiter(license_db=self._args.license_matrix_file,
                           licenses_preferences=licenses_preferences,
                           denied_licenses=licenses_denied,
+                          allowed_licenses=licenses_allowed,
                           update_dual=not self._args.no_relicense)
 
         return arbiter
 
     def _compatibility_report_to_return_code(self, compatibility_report):
         """ Given a compatibility report, this functions returns the return code
         """
```

### Comparing `flict-1.2.8/flict/var/alias.json` & `flict-1.2.9/flict/var/alias.json`

 * *Files identical despite different names*

### Comparing `flict-1.2.8/flict/var/scancode-licenses.json` & `flict-1.2.9/flict/var/scancode-licenses.json`

 * *Files identical despite different names*

### Comparing `flict-1.2.8/flict.egg-info/PKG-INFO` & `flict-1.2.9/flict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: flict
-Version: 1.2.8
+Version: 1.2.9
 Summary: FOSS License Compatibility Tool
 Home-page: https://github.com/vinland-technology/flict
 Author: Henrik Sanklef
 Author-email: hesa@sandklef.com
-License: UNKNOWN
+License: GPL-3.0-or-later
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
```

### Comparing `flict-1.2.8/flict.egg-info/SOURCES.txt` & `flict-1.2.9/flict.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flict-1.2.8/flict.egg-info/requires.txt` & `flict-1.2.9/flict.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 flake8-functions==0.0.8
 flake8-isort==6.1.1
 flake8-logging-format==0.9.0
 flake8-mutable~=1.2
 flake8-pep3101~=2.1
 flake8-print~=5.0
 flake8-quotes~=3.4
-flake8-requirements~=2.0
+flake8-requirements~=2.1
 flake8-string-format~=0.3
 flake8-variables-names==0.0.6
 flake8~=7.0
 jsonschema~=4.21
 pytest-bandit~=0.6
 pytest-cov~=4.1
 pytest-forked~=1.6
```

### Comparing `flict-1.2.8/requirements-dev.txt` & `flict-1.2.9/requirements-dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 flake8-functions == 0.0.8
 flake8-isort == 6.1.1
 flake8-logging-format == 0.9.0
 flake8-mutable ~= 1.2
 flake8-pep3101 ~= 2.1
 flake8-print ~= 5.0
 flake8-quotes ~= 3.4
-flake8-requirements ~= 2.0
+flake8-requirements ~= 2.1
 flake8-string-format ~= 0.3
 flake8-variables-names == 0.0.6
 pytest ~= 8.0
 pytest-bandit ~= 0.6
 pytest-cov ~= 4.1
 pytest-forked ~= 1.6
 pytest-icdiff ~= 0.9
```

### Comparing `flict-1.2.8/setup.py` & `flict-1.2.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,17 @@
     version=flict_version,
     author="Henrik Sanklef",
     author_email="hesa@sandklef.com",
     description="FOSS License Compatibility Tool",
     long_description=_long_description,
     long_description_content_type="text/markdown",
     license_files=('LICENSE',),
+    license='GPL-3.0-or-later',
     url="https://github.com/vinland-technology/flict",
+    bugtrack_url="https://github.com/vinland-technology/flict/issues",
     packages=['flict', 'flict.flictlib', 'flict.flictlib.format', 'flict.flictlib.project'],
     entry_points={
         "console_scripts": [
             "flict = flict.__main__:main",
         ],
     },
     package_data={
```

