# Comparing `tmp/ctdfjorder-0.0.5.tar.gz` & `tmp/ctdfjorder-0.0.6.tar.gz`

## Comparing `ctdfjorder-0.0.5.tar` & `ctdfjorder-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ctdfjorder-0.0.5/CTDFjorder.iml
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ctdfjorder-0.0.5/build.bat
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 ctdfjorder-0.0.5/build.sh
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ctdfjorder-0.0.5/environment.yml
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 ctdfjorder-0.0.5/meta.yaml
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ctdfjorder-0.0.5/requirements.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ctdfjorder-0.0.5/setup.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ctdfjorder-0.0.5/.idea/.gitignore
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ctdfjorder-0.0.5/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 ctdfjorder-0.0.5/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 ctdfjorder-0.0.5/.idea/vcs.xml
--rw-r--r--   0        0        0     5464 2020-02-02 00:00:00.000000 ctdfjorder-0.0.5/.idea/workspace.xml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ctdfjorder-0.0.5/src/Makefile
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 ctdfjorder-0.0.5/src/__init__.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ctdfjorder-0.0.5/src/make.bat
--rw-r--r--   0        0        0    54980 2020-02-02 00:00:00.000000 ctdfjorder-0.0.5/src/CTDFjorder/CTDFjorder.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ctdfjorder-0.0.5/src/CTDFjorder/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ctdfjorder-0.0.5/src/CTDFjorder/make.bat
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 ctdfjorder-0.0.5/LICENSE
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ctdfjorder-0.0.5/README.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 ctdfjorder-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 ctdfjorder-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/CTDFjorder.iml
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/build.bat
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/build.sh
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/environment.yml
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/meta.yaml
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/requirements.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/setup.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/.idea/.gitignore
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/.idea/vcs.xml
+-rw-r--r--   0        0        0     5464 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/.idea/workspace.xml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/src/Makefile
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/src/__init__.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/src/make.bat
+-rw-r--r--   0        0        0    54980 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/src/CTDFjorder/CTDFjorder.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/src/CTDFjorder/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/src/CTDFjorder/make.bat
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/LICENSE
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/README.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/PKG-INFO
```

### Comparing `ctdfjorder-0.0.5/.idea/workspace.xml` & `ctdfjorder-0.0.6/.idea/workspace.xml`

 * *Files 0% similar despite different names*

#### Comparing `ctdfjorder-0.0.5/.idea/workspace.xml` & `ctdfjorder-0.0.6/.idea/workspace.xml`

```diff
@@ -86,15 +86,15 @@
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="79559f9c-5462-40fb-9c71-dbede6c21cc8" name="Changes" comment=""/>
       <created>1714542246341</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1714542246341</updated>
-      <workItem from="1714542247510" duration="16942000"/>
+      <workItem from="1714542247510" duration="17082000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="XSLT-Support.FileAssociations.UIState">
```

### Comparing `ctdfjorder-0.0.5/src/Makefile` & `ctdfjorder-0.0.6/src/Makefile`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.5/src/make.bat` & `ctdfjorder-0.0.6/src/make.bat`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.5/src/CTDFjorder/CTDFjorder.py` & `ctdfjorder-0.0.6/src/CTDFjorder/CTDFjorder.py`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.5/src/CTDFjorder/Makefile` & `ctdfjorder-0.0.6/src/CTDFjorder/Makefile`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.5/src/CTDFjorder/make.bat` & `ctdfjorder-0.0.6/src/CTDFjorder/make.bat`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.5/LICENSE` & `ctdfjorder-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.5/pyproject.toml` & `ctdfjorder-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "CTDFjorder"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name="Nikolas Yanek-Chrones", email="nikojb1001@gmail.com" },
 ]
 description = "A package for processing and analyzing CTD data."
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
```

### Comparing `ctdfjorder-0.0.5/PKG-INFO` & `ctdfjorder-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: CTDFjorder
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for processing and analyzing CTD data.
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
 Author-email: Nikolas Yanek-Chrones <nikojb1001@gmail.com>
 License-File: LICENSE
 Keywords: CTD
 Classifier: Development Status :: 3 - Alpha
```

