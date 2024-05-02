# Comparing `tmp/galaxy-selenium-24.0.0.tar.gz` & `tmp/galaxy_selenium-24.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-selenium-24.0.0.tar", last modified: Wed Apr  3 02:45:22 2024, max compression
+gzip compressed data, was "galaxy_selenium-24.0.1.tar", last modified: Thu May  2 13:48:28 2024, max compression
```

## Comparing `galaxy-selenium-24.0.0.tar` & `galaxy_selenium-24.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:22.959222 galaxy-selenium-24.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-04-03 02:45:22.959222 galaxy-selenium-24.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:22.955222 galaxy-selenium-24.0.0/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:22.959222 galaxy-selenium-24.0.0/galaxy/selenium/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/axe_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/driver_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    12894 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/has_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/jupyter_context.py
--rw-r--r--   0 runner    (1001) docker     (127)   101170 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/navigates_galaxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:22.959222 galaxy-selenium-24.0.0/galaxy/selenium/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1474 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/scripts/dump_tour.py
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/sizzle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/smart_components.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:22.959222 galaxy-selenium-24.0.0/galaxy/selenium/toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/toolbox/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:22.959222 galaxy-selenium-24.0.0/galaxy_selenium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-04-03 02:45:22.000000 galaxy-selenium-24.0.0/galaxy_selenium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-03 02:45:22.000000 galaxy-selenium-24.0.0/galaxy_selenium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:45:22.000000 galaxy-selenium-24.0.0/galaxy_selenium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-03 02:45:22.000000 galaxy-selenium-24.0.0/galaxy_selenium.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 02:45:22.000000 galaxy-selenium-24.0.0/galaxy_selenium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:45:22.000000 galaxy-selenium-24.0.0/galaxy_selenium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-03 02:45:22.959222 galaxy-selenium-24.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:28.005793 galaxy_selenium-24.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-05-02 13:48:28.005793 galaxy_selenium-24.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:28.001793 galaxy_selenium-24.0.1/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:28.005793 galaxy_selenium-24.0.1/galaxy/selenium/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/axe_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/driver_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12894 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/has_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/jupyter_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101236 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/navigates_galaxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:28.005793 galaxy_selenium-24.0.1/galaxy/selenium/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1474 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/scripts/dump_tour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/sizzle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/smart_components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:28.005793 galaxy_selenium-24.0.1/galaxy/selenium/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/toolbox/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:28.005793 galaxy_selenium-24.0.1/galaxy_selenium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-05-02 13:48:27.000000 galaxy_selenium-24.0.1/galaxy_selenium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-02 13:48:27.000000 galaxy_selenium-24.0.1/galaxy_selenium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:48:27.000000 galaxy_selenium-24.0.1/galaxy_selenium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-02 13:48:27.000000 galaxy_selenium-24.0.1/galaxy_selenium.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-02 13:48:27.000000 galaxy_selenium-24.0.1/galaxy_selenium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:48:27.000000 galaxy_selenium-24.0.1/galaxy_selenium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-02 13:48:28.005793 galaxy_selenium-24.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/test-requirements.txt
```

### Comparing `galaxy-selenium-24.0.0/HISTORY.rst` & `galaxy_selenium-24.0.1/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Set from_tool_form: true when saving new workflow by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17972 <https://github.com/galaxyproject/galaxy/pull/17972>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-selenium-24.0.0/LICENSE` & `galaxy_selenium-24.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-24.0.0/PKG-INFO` & `galaxy_selenium-24.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-selenium
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy Selenium interaction framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -49,14 +49,25 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Set from_tool_form: true when saving new workflow by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17972 <https://github.com/galaxyproject/galaxy/pull/17972>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-selenium-24.0.0/galaxy/selenium/axe_results.py` & `galaxy_selenium-24.0.1/galaxy/selenium/axe_results.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-24.0.0/galaxy/selenium/cli.py` & `galaxy_selenium-24.0.1/galaxy/selenium/cli.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-24.0.0/galaxy/selenium/context.py` & `galaxy_selenium-24.0.1/galaxy/selenium/context.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-24.0.0/galaxy/selenium/driver_factory.py` & `galaxy_selenium-24.0.1/galaxy/selenium/driver_factory.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-24.0.0/galaxy/selenium/has_driver.py` & `galaxy_selenium-24.0.1/galaxy/selenium/has_driver.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-24.0.0/galaxy/selenium/navigates_galaxy.py` & `galaxy_selenium-24.0.1/galaxy/selenium/navigates_galaxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1554,31 +1554,32 @@
 
     def workflow_run_ensure_expanded(self):
         workflow_run = self.components.workflow_run
         if workflow_run.expanded_form.is_absent:
             workflow_run.expand_form_link.wait_for_and_click()
             workflow_run.expanded_form.wait_for_visible()
 
-    def workflow_create_new(self, annotation=None, clear_placeholder=False):
+    def workflow_create_new(self, annotation=None, clear_placeholder=False, save_workflow=True):
         self.workflow_index_open()
         self.sleep_for(self.wait_types.UX_RENDER)
         self.click_button_new_workflow()
         self.sleep_for(self.wait_types.UX_RENDER)
         name = self._get_random_name()
         name_component = self.components.workflow_editor.edit_name
         if clear_placeholder:
             name_component.wait_for_visible().clear()
         name_component.wait_for_and_send_keys(name)
         annotation = annotation or self._get_random_name()
         self.components.workflow_editor.edit_annotation.wait_for_and_send_keys(annotation)
-        save_button = self.components.workflow_editor.save_button
-        save_button.wait_for_visible()
-        assert not save_button.has_class("disabled")
-        save_button.wait_for_and_click()
-        self.sleep_for(self.wait_types.UX_RENDER)
+        if save_workflow:
+            save_button = self.components.workflow_editor.save_button
+            save_button.wait_for_visible()
+            assert not save_button.has_class("disabled")
+            save_button.wait_for_and_click()
+            self.sleep_for(self.wait_types.UX_RENDER)
         return name
 
     def invocation_index_table_elements(self):
         invocations = self.components.invocations
         invocations.invocations_table.wait_for_visible()
         return invocations.invocations_table_rows.all()
```

### Comparing `galaxy-selenium-24.0.0/galaxy/selenium/scripts/dump_tour.py` & `galaxy_selenium-24.0.1/galaxy/selenium/scripts/dump_tour.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-24.0.0/galaxy/selenium/sizzle.py` & `galaxy_selenium-24.0.1/galaxy/selenium/sizzle.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-24.0.0/galaxy/selenium/smart_components.py` & `galaxy_selenium-24.0.1/galaxy/selenium/smart_components.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-24.0.0/galaxy_selenium.egg-info/PKG-INFO` & `galaxy_selenium-24.0.1/galaxy_selenium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-selenium
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy Selenium interaction framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -49,14 +49,25 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Set from_tool_form: true when saving new workflow by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17972 <https://github.com/galaxyproject/galaxy/pull/17972>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-selenium-24.0.0/galaxy_selenium.egg-info/SOURCES.txt` & `galaxy_selenium-24.0.1/galaxy_selenium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-24.0.0/setup.cfg` & `galaxy_selenium-24.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-selenium
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.0
+version = 24.0.1
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-navigation
 	galaxy-util
 	axe-selenium-python
```

