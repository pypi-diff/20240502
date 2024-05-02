# Comparing `tmp/pylogfile-0.0.1.dev2.tar.gz` & `tmp/pylogfile-0.0.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylogfile-0.0.1.dev2.tar", last modified: Mon Apr  1 17:31:01 2024, max compression
+gzip compressed data, was "pylogfile-0.0.1.dev3.tar", last modified: Thu May  2 20:33:33 2024, max compression
```

## Comparing `pylogfile-0.0.1.dev2.tar` & `pylogfile-0.0.1.dev3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 grantgiesbrecht   (501) staff       (20)        0 2024-04-01 17:31:01.844353 pylogfile-0.0.1.dev2/
--rw-r--r--   0 grantgiesbrecht   (501) staff       (20)     1503 2024-03-28 21:07:52.000000 pylogfile-0.0.1.dev2/LICENSE
--rw-r--r--   0 grantgiesbrecht   (501) staff       (20)      579 2024-04-01 17:31:01.843946 pylogfile-0.0.1.dev2/PKG-INFO
--rw-r--r--   0 grantgiesbrecht   (501) staff       (20)       43 2024-03-28 21:07:52.000000 pylogfile-0.0.1.dev2/README.md
--rw-r--r--   0 grantgiesbrecht   (501) staff       (20)      605 2024-04-01 17:30:40.000000 pylogfile-0.0.1.dev2/pyproject.toml
--rw-r--r--   0 grantgiesbrecht   (501) staff       (20)       38 2024-04-01 17:31:01.844446 pylogfile-0.0.1.dev2/setup.cfg
-drwxr-xr-x   0 grantgiesbrecht   (501) staff       (20)        0 2024-04-01 17:31:01.841484 pylogfile-0.0.1.dev2/src/
--rw-r--r--   0 grantgiesbrecht   (501) staff       (20)        0 2024-04-01 17:13:14.000000 pylogfile-0.0.1.dev2/src/__init__.py
-drwxr-xr-x   0 grantgiesbrecht   (501) staff       (20)        0 2024-04-01 17:31:01.843515 pylogfile-0.0.1.dev2/src/pylogfile.egg-info/
--rw-r--r--   0 grantgiesbrecht   (501) staff       (20)      579 2024-04-01 17:31:01.000000 pylogfile-0.0.1.dev2/src/pylogfile.egg-info/PKG-INFO
--rw-r--r--   0 grantgiesbrecht   (501) staff       (20)      213 2024-04-01 17:31:01.000000 pylogfile-0.0.1.dev2/src/pylogfile.egg-info/SOURCES.txt
--rw-r--r--   0 grantgiesbrecht   (501) staff       (20)        1 2024-04-01 17:31:01.000000 pylogfile-0.0.1.dev2/src/pylogfile.egg-info/dependency_links.txt
--rw-r--r--   0 grantgiesbrecht   (501) staff       (20)       19 2024-04-01 17:31:01.000000 pylogfile-0.0.1.dev2/src/pylogfile.egg-info/top_level.txt
--rw-r--r--   0 grantgiesbrecht   (501) staff       (20)     1788 2024-03-28 21:11:23.000000 pylogfile-0.0.1.dev2/src/pylogfile.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:33:33.023178 pylogfile-0.0.1.dev3/
+-rw-rw-rw-   0        0        0     1531 2024-03-31 18:20:16.000000 pylogfile-0.0.1.dev3/LICENSE
+-rw-rw-rw-   0        0        0      595 2024-05-02 20:33:33.021179 pylogfile-0.0.1.dev3/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2024-03-31 18:20:16.000000 pylogfile-0.0.1.dev3/README.md
+-rw-rw-rw-   0        0        0      626 2024-05-02 20:33:25.000000 pylogfile-0.0.1.dev3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-02 20:33:33.023178 pylogfile-0.0.1.dev3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-02 20:33:33.007023 pylogfile-0.0.1.dev3/src/
+-rw-rw-rw-   0        0        0        0 2024-04-29 19:50:51.000000 pylogfile-0.0.1.dev3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:33:33.020179 pylogfile-0.0.1.dev3/src/pylogfile.egg-info/
+-rw-rw-rw-   0        0        0      595 2024-05-02 20:33:32.000000 pylogfile-0.0.1.dev3/src/pylogfile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2024-05-02 20:33:32.000000 pylogfile-0.0.1.dev3/src/pylogfile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 20:33:32.000000 pylogfile-0.0.1.dev3/src/pylogfile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-02 20:33:32.000000 pylogfile-0.0.1.dev3/src/pylogfile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9713 2024-05-02 20:28:39.000000 pylogfile-0.0.1.dev3/src/pylogfile.py
```

### Comparing `pylogfile-0.0.1.dev2/LICENSE` & `pylogfile-0.0.1.dev3/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-BSD 3-Clause License
-
-Copyright (c) 2024, Grant-Giesbrecht
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2024, Grant-Giesbrecht
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `pylogfile-0.0.1.dev2/pyproject.toml` & `pylogfile-0.0.1.dev3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,16 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "pylogfile"
-version = "0.0.1.dev2"
-authors = [
-  { name="Grant Giesbrecht", email="grant.giesbrecht@colorado.edu" },
-]
-description = "Universal log files for Python"
-readme = "README.md"
-requires-python = ">=3.8"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-Homepage = "https://github.com/Grant-Giesbrecht/pylogfile"
-Issues = "https://github.com/Grant-Giesbrecht/pylogfile/issues"
+Metadata-Version: 2.1
+Name: pylogfile
+Version: 0.0.1.dev3
+Summary: Universal log files for Python
+Author-email: Grant Giesbrecht <grant.giesbrecht@colorado.edu>
+Project-URL: Homepage, https://github.com/Grant-Giesbrecht/pylogfile
+Project-URL: Issues, https://github.com/Grant-Giesbrecht/pylogfile/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pylogfile
+Universal log files for Python
```

