# Comparing `tmp/mojo_results-1.3.8.tar.gz` & `tmp/mojo_results-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_results-1.3.8.tar", max compression
+gzip compressed data, was "mojo_results-1.3.9.tar", max compression
```

## Comparing `mojo_results-1.3.8.tar` & `mojo_results-1.3.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1083 2024-01-26 02:53:51.913156 mojo_results-1.3.8/LICENSE.txt
--rw-r--r--   0        0        0      993 2024-01-26 02:53:51.913246 mojo_results-1.3.8/README.rst
--rw-r--r--   0        0        0      751 2024-03-01 02:51:13.766001 mojo_results-1.3.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-26 02:53:51.914161 mojo_results-1.3.8/source/packages/mojo/results/concentrators/__init__.py
--rw-r--r--   0        0        0     4650 2024-01-26 02:53:51.914225 mojo_results-1.3.8/source/packages/mojo/results/concentrators/progresscontentratorservice.py
--rw-r--r--   0        0        0        0 2024-01-26 02:53:51.914269 mojo_results-1.3.8/source/packages/mojo/results/model/__init__.py
--rw-r--r--   0        0        0      933 2024-01-26 02:53:51.914339 mojo_results-1.3.8/source/packages/mojo/results/model/buildinfo.py
--rw-r--r--   0        0        0      969 2024-01-26 02:53:51.914390 mojo_results-1.3.8/source/packages/mojo/results/model/forwardinginfo.py
--rw-r--r--   0        0        0     1290 2024-01-26 02:53:51.914491 mojo_results-1.3.8/source/packages/mojo/results/model/jobcontainer.py
--rw-r--r--   0        0        0      952 2024-01-26 02:53:51.914545 mojo_results-1.3.8/source/packages/mojo/results/model/jobinfo.py
--rw-r--r--   0        0        0      824 2024-01-26 02:53:51.914590 mojo_results-1.3.8/source/packages/mojo/results/model/pipelineinfo.py
--rw-r--r--   0        0        0      206 2024-01-26 02:53:51.914634 mojo_results-1.3.8/source/packages/mojo/results/model/progresscode.py
--rw-r--r--   0        0        0      444 2024-02-17 05:34:32.277678 mojo_results-1.3.8/source/packages/mojo/results/model/progressdelivery.py
--rw-r--r--   0        0        0     1952 2024-01-26 02:53:51.914686 mojo_results-1.3.8/source/packages/mojo/results/model/progressinfo.py
--rw-r--r--   0        0        0      146 2024-01-26 02:53:51.914730 mojo_results-1.3.8/source/packages/mojo/results/model/progresstype.py
--rw-r--r--   0        0        0     1157 2024-01-26 02:53:51.914769 mojo_results-1.3.8/source/packages/mojo/results/model/renderinfo.py
--rw-r--r--   0        0        0      764 2024-01-26 02:53:51.914830 mojo_results-1.3.8/source/packages/mojo/results/model/resultcode.py
--rw-r--r--   0        0        0     3044 2024-01-26 02:53:51.914874 mojo_results-1.3.8/source/packages/mojo/results/model/resultcontainer.py
--rw-r--r--   0        0        0     7784 2024-01-26 02:53:51.914926 mojo_results-1.3.8/source/packages/mojo/results/model/resultnode.py
--rw-r--r--   0        0        0      836 2024-01-26 02:53:51.914975 mojo_results-1.3.8/source/packages/mojo/results/model/resulttype.py
--rw-r--r--   0        0        0     2699 2024-01-26 02:53:51.915021 mojo_results-1.3.8/source/packages/mojo/results/model/taskinggroup.py
--rw-r--r--   0        0        0     8272 2024-03-01 02:50:58.690173 mojo_results-1.3.8/source/packages/mojo/results/model/taskingresult.py
--rw-r--r--   0        0        0     1474 2024-01-26 02:53:51.915134 mojo_results-1.3.8/source/packages/mojo/results/model/testcontainer.py
--rw-r--r--   0        0        0     4694 2024-01-26 02:53:51.915184 mojo_results-1.3.8/source/packages/mojo/results/model/testresult.py
--rw-r--r--   0        0        0        0 2024-01-26 02:53:51.915234 mojo_results-1.3.8/source/packages/mojo/results/recorders/__init__.py
--rw-r--r--   0        0        0     4750 2024-02-17 08:12:31.006971 mojo_results-1.3.8/source/packages/mojo/results/recorders/jsonresultrecorder.py
--rw-r--r--   0        0        0    13105 2024-02-17 08:32:31.683795 mojo_results-1.3.8/source/packages/mojo/results/recorders/resultrecorder.py
--rw-r--r--   0        0        0     1921 2024-01-26 02:53:51.915449 mojo_results-1.3.8/source/packages/mojo/results/utilities.py
--rw-r--r--   0        0        0     1842 1970-01-01 00:00:00.000000 mojo_results-1.3.8/setup.py
--rw-r--r--   0        0        0     1749 1970-01-01 00:00:00.000000 mojo_results-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-26 02:53:51.913156 mojo_results-1.3.9/LICENSE.txt
+-rw-r--r--   0        0        0      993 2024-01-26 02:53:51.913246 mojo_results-1.3.9/README.rst
+-rw-r--r--   0        0        0      751 2024-03-01 02:54:49.434329 mojo_results-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-26 02:53:51.914161 mojo_results-1.3.9/source/packages/mojo/results/concentrators/__init__.py
+-rw-r--r--   0        0        0     4650 2024-01-26 02:53:51.914225 mojo_results-1.3.9/source/packages/mojo/results/concentrators/progresscontentratorservice.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:53:51.914269 mojo_results-1.3.9/source/packages/mojo/results/model/__init__.py
+-rw-r--r--   0        0        0      933 2024-01-26 02:53:51.914339 mojo_results-1.3.9/source/packages/mojo/results/model/buildinfo.py
+-rw-r--r--   0        0        0      969 2024-01-26 02:53:51.914390 mojo_results-1.3.9/source/packages/mojo/results/model/forwardinginfo.py
+-rw-r--r--   0        0        0     1290 2024-01-26 02:53:51.914491 mojo_results-1.3.9/source/packages/mojo/results/model/jobcontainer.py
+-rw-r--r--   0        0        0      952 2024-01-26 02:53:51.914545 mojo_results-1.3.9/source/packages/mojo/results/model/jobinfo.py
+-rw-r--r--   0        0        0      824 2024-01-26 02:53:51.914590 mojo_results-1.3.9/source/packages/mojo/results/model/pipelineinfo.py
+-rw-r--r--   0        0        0      206 2024-01-26 02:53:51.914634 mojo_results-1.3.9/source/packages/mojo/results/model/progresscode.py
+-rw-r--r--   0        0        0      444 2024-02-17 05:34:32.277678 mojo_results-1.3.9/source/packages/mojo/results/model/progressdelivery.py
+-rw-r--r--   0        0        0     1952 2024-01-26 02:53:51.914686 mojo_results-1.3.9/source/packages/mojo/results/model/progressinfo.py
+-rw-r--r--   0        0        0      146 2024-01-26 02:53:51.914730 mojo_results-1.3.9/source/packages/mojo/results/model/progresstype.py
+-rw-r--r--   0        0        0     1157 2024-01-26 02:53:51.914769 mojo_results-1.3.9/source/packages/mojo/results/model/renderinfo.py
+-rw-r--r--   0        0        0      764 2024-01-26 02:53:51.914830 mojo_results-1.3.9/source/packages/mojo/results/model/resultcode.py
+-rw-r--r--   0        0        0     3044 2024-01-26 02:53:51.914874 mojo_results-1.3.9/source/packages/mojo/results/model/resultcontainer.py
+-rw-r--r--   0        0        0     7784 2024-01-26 02:53:51.914926 mojo_results-1.3.9/source/packages/mojo/results/model/resultnode.py
+-rw-r--r--   0        0        0      836 2024-01-26 02:53:51.914975 mojo_results-1.3.9/source/packages/mojo/results/model/resulttype.py
+-rw-r--r--   0        0        0     2699 2024-01-26 02:53:51.915021 mojo_results-1.3.9/source/packages/mojo/results/model/taskinggroup.py
+-rw-r--r--   0        0        0     8430 2024-03-01 02:54:42.422751 mojo_results-1.3.9/source/packages/mojo/results/model/taskingresult.py
+-rw-r--r--   0        0        0     1474 2024-01-26 02:53:51.915134 mojo_results-1.3.9/source/packages/mojo/results/model/testcontainer.py
+-rw-r--r--   0        0        0     4694 2024-01-26 02:53:51.915184 mojo_results-1.3.9/source/packages/mojo/results/model/testresult.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:53:51.915234 mojo_results-1.3.9/source/packages/mojo/results/recorders/__init__.py
+-rw-r--r--   0        0        0     4750 2024-02-17 08:12:31.006971 mojo_results-1.3.9/source/packages/mojo/results/recorders/jsonresultrecorder.py
+-rw-r--r--   0        0        0    13105 2024-02-17 08:32:31.683795 mojo_results-1.3.9/source/packages/mojo/results/recorders/resultrecorder.py
+-rw-r--r--   0        0        0     1921 2024-01-26 02:53:51.915449 mojo_results-1.3.9/source/packages/mojo/results/utilities.py
+-rw-r--r--   0        0        0     1842 1970-01-01 00:00:00.000000 mojo_results-1.3.9/setup.py
+-rw-r--r--   0        0        0     1749 1970-01-01 00:00:00.000000 mojo_results-1.3.9/PKG-INFO
```

### Comparing `mojo_results-1.3.8/LICENSE.txt` & `mojo_results-1.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_results-1.3.8/README.rst` & `mojo_results-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `mojo_results-1.3.8/pyproject.toml` & `mojo_results-1.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mojo-results"
 description = "The Automation Mojo Results Package"
-version = "1.3.8"
+version = "1.3.9"
 authors = ["Myron W. Walker"]
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
```

### Comparing `mojo_results-1.3.8/source/packages/mojo/results/concentrators/progresscontentratorservice.py` & `mojo_results-1.3.9/source/packages/mojo/results/concentrators/progresscontentratorservice.py`

 * *Files identical despite different names*

### Comparing `mojo_results-1.3.8/source/packages/mojo/results/model/buildinfo.py` & `mojo_results-1.3.9/source/packages/mojo/results/model/buildinfo.py`

 * *Files identical despite different names*

### Comparing `mojo_results-1.3.8/source/packages/mojo/results/model/forwardinginfo.py` & `mojo_results-1.3.9/source/packages/mojo/results/model/forwardinginfo.py`

 * *Files identical despite different names*

### Comparing `mojo_results-1.3.8/source/packages/mojo/results/model/jobcontainer.py` & `mojo_results-1.3.9/source/packages/mojo/results/model/jobcontainer.py`

 * *Files identical despite different names*

### Comparing `mojo_results-1.3.8/source/packages/mojo/results/model/jobinfo.py` & `mojo_results-1.3.9/source/packages/mojo/results/model/jobinfo.py`

 * *Files identical despite different names*

### Comparing `mojo_results-1.3.8/source/packages/mojo/results/model/pipelineinfo.py` & `mojo_results-1.3.9/source/packages/mojo/results/model/pipelineinfo.py`

 * *Files identical despite different names*

### Comparing `mojo_results-1.3.8/source/packages/mojo/results/model/progressinfo.py` & `mojo_results-1.3.9/source/packages/mojo/results/model/progressinfo.py`

 * *Files identical despite different names*

### Comparing `mojo_results-1.3.8/source/packages/mojo/results/model/renderinfo.py` & `mojo_results-1.3.9/source/packages/mojo/results/model/renderinfo.py`

 * *Files identical despite different names*

### Comparing `mojo_results-1.3.8/source/packages/mojo/results/model/resultcode.py` & `mojo_results-1.3.9/source/packages/mojo/results/model/resultcode.py`

 * *Files identical despite different names*

### Comparing `mojo_results-1.3.8/source/packages/mojo/results/model/resultcontainer.py` & `mojo_results-1.3.9/source/packages/mojo/results/model/resultcontainer.py`

 * *Files identical despite different names*

### Comparing `mojo_results-1.3.8/source/packages/mojo/results/model/resultnode.py` & `mojo_results-1.3.9/source/packages/mojo/results/model/resultnode.py`

 * *Files identical despite different names*

### Comparing `mojo_results-1.3.8/source/packages/mojo/results/model/resulttype.py` & `mojo_results-1.3.9/source/packages/mojo/results/model/resulttype.py`

 * *Files identical despite different names*

### Comparing `mojo_results-1.3.8/source/packages/mojo/results/model/taskinggroup.py` & `mojo_results-1.3.9/source/packages/mojo/results/model/taskinggroup.py`

 * *Files identical despite different names*

### Comparing `mojo_results-1.3.8/source/packages/mojo/results/model/taskingresult.py` & `mojo_results-1.3.9/source/packages/mojo/results/model/taskingresult.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,21 @@
     @property
     def worker(self):
         """
             The worker that will be used to execute the tasking.
         """
         return self._worker
 
+    def add_result(self, result: Any):
+        """
+            Add a result to this tasking result.
+        """
+        self._result = result
+        return
+
     def as_dict(self, is_preview: bool = False) -> collections.OrderedDict:
         """
             Converts the result node instance to an :class:`collections.OrderedDict` object.
         """
 
         start_datetime = format_datetime_with_fractional(self._start)
```

### Comparing `mojo_results-1.3.8/source/packages/mojo/results/model/testcontainer.py` & `mojo_results-1.3.9/source/packages/mojo/results/model/testcontainer.py`

 * *Files identical despite different names*

### Comparing `mojo_results-1.3.8/source/packages/mojo/results/model/testresult.py` & `mojo_results-1.3.9/source/packages/mojo/results/model/testresult.py`

 * *Files identical despite different names*

### Comparing `mojo_results-1.3.8/source/packages/mojo/results/recorders/jsonresultrecorder.py` & `mojo_results-1.3.9/source/packages/mojo/results/recorders/jsonresultrecorder.py`

 * *Files identical despite different names*

### Comparing `mojo_results-1.3.8/source/packages/mojo/results/recorders/resultrecorder.py` & `mojo_results-1.3.9/source/packages/mojo/results/recorders/resultrecorder.py`

 * *Files identical despite different names*

### Comparing `mojo_results-1.3.8/source/packages/mojo/results/utilities.py` & `mojo_results-1.3.9/source/packages/mojo/results/utilities.py`

 * *Files identical despite different names*

### Comparing `mojo_results-1.3.8/setup.py` & `mojo_results-1.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 {'': ['*']}
 
 install_requires = \
 ['mojo-errors>=1.3.0,<1.4.0', 'mojo-xmodules>=1.3.0,<1.4.0']
 
 setup_kwargs = {
     'name': 'mojo-results',
-    'version': '1.3.8',
+    'version': '1.3.9',
     'description': 'The Automation Mojo Results Package',
     'long_description': "=======================\nMojo Results Package\n=======================\nThis package contains code elements for working with automation results.\n\n=========================\nFeatures of this Template\n=========================\n* Machine Setup\n* Virtual Environment Setup (Poetry)\n* PyPi Publishing\n* Sphinx Documentation\n\n=================\nCode Organization\n=================\n* .vscode - Common tasks\n* development - This is where the runtime environment scripts are located\n* repository-setup - Scripts for homing your repository and to your checkout and machine setup\n* userguide - Where you put your user guide\n* source/packages - Put your root folder here 'source/packages/(root-module-folder)'\n* source/sphinx - This is the Sphinx documentation folder\n* workspaces - This is where you add VSCode workspaces templates and where workspaces show up when homed.\n\n==========\nReferences\n==========\n\n- `User Guide <userguide/userguide.rst>`\n- `Coding Standards <userguide/10-00-coding-standards.rst>`\n",
     'author': 'Myron W. Walker',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mojo_results-1.3.8/PKG-INFO` & `mojo_results-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mojo-results
-Version: 1.3.8
+Version: 1.3.9
 Summary: The Automation Mojo Results Package
 License: LICENSE.txt
 Keywords: python
 Author: Myron W. Walker
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
```

