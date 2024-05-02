# Comparing `tmp/pyson_data-0.0.2.tar.gz` & `tmp/pyson_data-0.0.3.tar.gz`

## Comparing `pyson_data-0.0.2.tar` & `pyson_data-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pyson_data-0.0.2/setup.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 pyson_data-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 pyson_data-0.0.2/.idea/PYSON.iml
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 pyson_data-0.0.2/.idea/discord.xml
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 pyson_data-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 pyson_data-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pyson_data-0.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 pyson_data-0.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pyson_data-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 pyson_data-0.0.2/src/pyson_data/.pypirc
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pyson_data-0.0.2/src/pyson_data/__init__.py
--rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 pyson_data-0.0.2/src/pyson_data/pyson.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 pyson_data-0.0.2/tests/example.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 pyson_data-0.0.2/tests/example.pyson
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pyson_data-0.0.2/.gitignore
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 pyson_data-0.0.2/LICENSE
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 pyson_data-0.0.2/README.md
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 pyson_data-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 pyson_data-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 pyson_data-0.0.3/setup.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 pyson_data-0.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 pyson_data-0.0.3/.idea/PYSON.iml
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 pyson_data-0.0.3/.idea/discord.xml
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 pyson_data-0.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 pyson_data-0.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pyson_data-0.0.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 pyson_data-0.0.3/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pyson_data-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 pyson_data-0.0.3/src/pyson_data/.pypirc
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pyson_data-0.0.3/src/pyson_data/__init__.py
+-rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 pyson_data-0.0.3/src/pyson_data/pyson.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 pyson_data-0.0.3/tests/example.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 pyson_data-0.0.3/tests/example.pyson
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pyson_data-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 pyson_data-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 pyson_data-0.0.3/README.md
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 pyson_data-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 pyson_data-0.0.3/PKG-INFO
```

### Comparing `pyson_data-0.0.2/setup.py` & `pyson_data-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
      name='pyson_data',
-     version='0.1',
+     version='0.0.3',
      scripts=['pyson_data'],
      author="ComputingSquid",
      description="Provides support for storing data in .pyson format",
      long_description=long_description,
-   long_description_content_type="text/markdown",
+     long_description_content_type="text/markdown",
      url="https://github.com/ProbablyComputingSquid/PYSON",
      packages=setuptools.find_packages(),
      classifiers=[
          "Programming Language :: Python :: 3",
          "License :: OSI Approved :: MIT License",
          "Operating System :: OS Independent",
      ],
```

### Comparing `pyson_data-0.0.2/.idea/workspace.xml` & `pyson_data-0.0.3/.idea/workspace.xml`

 * *Files 0% similar despite different names*

#### Comparing `pyson_data-0.0.2/.idea/workspace.xml` & `pyson_data-0.0.3/.idea/workspace.xml`

```diff
@@ -1,16 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="7702ad28-190f-4fe1-86d3-84aadacb3e86" name="Changes" comment="">
-      <change afterPath="$PROJECT_DIR$/dist/pyson_data-0.0.1-py3-none-any.whl" afterDir="false"/>
-      <change afterPath="$PROJECT_DIR$/dist/pyson_data-0.0.1.tar.gz" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/dist/pyson_data-0.0.2-py3-none-any.whl" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/dist/pyson_data-0.0.2.tar.gz" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/setup.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/pyson_data/.pypirc" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/pyson_data/__init__.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/tests/example.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/example.py" beforeDir="false"/>
       <change beforePath="$PROJECT_DIR$/example.pyson" beforeDir="false" afterPath="$PROJECT_DIR$/tests/example.pyson" afterDir="false"/>
@@ -88,15 +88,15 @@
     <task active="true" id="Default" summary="Default task">
       <changelist id="7702ad28-190f-4fe1-86d3-84aadacb3e86" name="Changes" comment=""/>
       <created>1714600810067</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1714600810067</updated>
       <workItem from="1714600811622" duration="1271000"/>
-      <workItem from="1714604796800" duration="1918000"/>
+      <workItem from="1714604796800" duration="2314000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="VcsManagerConfiguration">
```

### Comparing `pyson_data-0.0.2/src/pyson_data/pyson.py` & `pyson_data-0.0.3/src/pyson_data/pyson.py`

 * *Files identical despite different names*

### Comparing `pyson_data-0.0.2/tests/example.py` & `pyson_data-0.0.3/tests/example.py`

 * *Files identical despite different names*

### Comparing `pyson_data-0.0.2/LICENSE` & `pyson_data-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyson_data-0.0.2/README.md` & `pyson_data-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyson_data-0.0.2/pyproject.toml` & `pyson_data-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyson-data"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="josh-co", email="author@example.com" },
 ]
 description = "Pyson package for .pyson data format"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pyson_data-0.0.2/PKG-INFO` & `pyson_data-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyson-data
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pyson package for .pyson data format
 Project-URL: Homepage, https://github.com/ProbablyComputingSquid/PYSON/
 Project-URL: Issues, https://github.com/ProbablyComputingSquid/PYSON/issues
 Author-email: josh-co <author@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

