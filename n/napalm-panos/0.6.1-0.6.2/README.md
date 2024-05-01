# Comparing `tmp/napalm_panos-0.6.1.tar.gz` & `tmp/napalm_panos-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napalm_panos-0.6.1.tar", max compression
+gzip compressed data, was "napalm_panos-0.6.2.tar", max compression
```

## Comparing `napalm_panos-0.6.1.tar` & `napalm_panos-0.6.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       77 2024-04-23 01:52:25.182351 napalm_panos-0.6.1/AUTHORS
--rw-r--r--   0        0        0     1959 2024-04-23 01:52:25.182351 napalm_panos-0.6.1/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2024-04-23 01:52:25.182351 napalm_panos-0.6.1/LICENSE
--rw-r--r--   0        0        0     4012 2024-04-23 01:52:25.182351 napalm_panos-0.6.1/README.md
--rw-r--r--   0        0        0      769 2024-04-23 01:52:25.182351 napalm_panos-0.6.1/napalm_panos/__init__.py
--rw-r--r--   0        0        0    31634 2024-04-23 01:52:25.182351 napalm_panos-0.6.1/napalm_panos/panos.py
--rw-r--r--   0        0        0        0 2024-04-23 01:52:25.182351 napalm_panos-0.6.1/napalm_panos/templates/.placeholder
--rw-r--r--   0        0        0       46 2024-04-23 01:52:25.182351 napalm_panos-0.6.1/napalm_panos/templates/set_hostname.j2
--rw-r--r--   0        0        0       28 2024-04-23 01:52:25.182351 napalm_panos-0.6.1/napalm_panos/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 01:52:25.182351 napalm_panos-0.6.1/napalm_panos/utils/textfsm_templates/.placeholder
--rw-r--r--   0        0        0     2834 2024-04-23 01:52:32.378396 napalm_panos-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     5215 1970-01-01 00:00:00.000000 napalm_panos-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0       77 2024-05-01 22:20:28.929094 napalm_panos-0.6.2/AUTHORS
+-rw-r--r--   0        0        0     2037 2024-05-01 22:20:28.929094 napalm_panos-0.6.2/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2024-05-01 22:20:28.929094 napalm_panos-0.6.2/LICENSE
+-rw-r--r--   0        0        0     4012 2024-05-01 22:20:28.929094 napalm_panos-0.6.2/README.md
+-rw-r--r--   0        0        0      820 2024-05-01 22:20:28.929094 napalm_panos-0.6.2/napalm_panos/__init__.py
+-rw-r--r--   0        0        0    31634 2024-05-01 22:20:28.929094 napalm_panos-0.6.2/napalm_panos/panos.py
+-rw-r--r--   0        0        0        0 2024-05-01 22:20:28.929094 napalm_panos-0.6.2/napalm_panos/templates/.placeholder
+-rw-r--r--   0        0        0       46 2024-05-01 22:20:28.929094 napalm_panos-0.6.2/napalm_panos/templates/set_hostname.j2
+-rw-r--r--   0        0        0       28 2024-05-01 22:20:28.933094 napalm_panos-0.6.2/napalm_panos/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 22:20:28.933094 napalm_panos-0.6.2/napalm_panos/utils/textfsm_templates/.placeholder
+-rw-r--r--   0        0        0     2811 2024-05-01 22:20:41.737198 napalm_panos-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     5177 1970-01-01 00:00:00.000000 napalm_panos-0.6.2/PKG-INFO
```

### Comparing `napalm_panos-0.6.1/CHANGELOG.md` & `napalm_panos-0.6.2/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,36 @@
+# 0.6.2 - 2024-04
+
+### Fixed
+- #118 Remove cryptography pinned dependency.
+
+
 # 0.6.1 - 2024-04
 
 ### Added
 - #108 Added Support for sdwan interfaces
 - #105 Include interface description for get_interfaces method
 
-
 ### Fixed
 - #115 Update package dependencies, fix tests
 
+
 # 0.6.0 - 2022-02
 
 ### Added
 - #102 Added Support for get_arp_table method
 - #99 Added documentation of supported getters
 - #93 Added ability to lock config optionally
 - #104 Added change log document
 
 ## Fixed
 - #101 Handles unable to convert to int for edge case with interfaces
 - #103 Fix Empty List of Interfaces
 
+
 ## 0.5.4 - 2022-02
 
 ### Fixed
 - #94 load_replace_candidate broke
 
 ### Changed
 - #96 Update Readme
```

### Comparing `napalm_panos-0.6.1/LICENSE` & `napalm_panos-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napalm_panos-0.6.1/README.md` & `napalm_panos-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `napalm_panos-0.6.1/napalm_panos/__init__.py` & `napalm_panos-0.6.2/napalm_panos/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,13 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations under
 # the License.
 
 """napalm_panos package."""
 
+from importlib import metadata
+
 # Import local modules
 from napalm_panos.panos import PANOSDriver
 
-__version__ = "0.6.1"
+__version__ = metadata.version(__name__)
 
 __all__ = ("PANOSDriver",)
```

### Comparing `napalm_panos-0.6.1/napalm_panos/panos.py` & `napalm_panos-0.6.2/napalm_panos/panos.py`

 * *Files identical despite different names*

### Comparing `napalm_panos-0.6.1/pyproject.toml` & `napalm_panos-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "napalm_panos"
-version = "v0.6.1"
+version = "v0.6.2"
 description = "Network Automation and Programmability Abstraction Layer with Multivendor support for PANOS."
 authors = ["Gabriele Gerbino <gabriele@networktocode.com>"]
 license = "Apache-2.0"
 homepage = "https://github.com/napalm-automation/napalm-panos"
 repository = "https://github.com/napalm-automation/napalm-panos"
 documentation = "https://github.com/napalm-automation/napalm-panos"
 readme = "README.md"
@@ -23,15 +23,14 @@
     "LICENSE",
     "README.md",
     "napalm_panos/templates/*.j2",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-cryptography = "3.3.2"
 napalm = "^4.0.0"
 lxml = "^5.0.0"
 pan-python = "*"
 netmiko = "^4.0.0"
 requests-toolbelt = "*"
 xmltodict = "*"
```

### Comparing `napalm_panos-0.6.1/PKG-INFO` & `napalm_panos-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napalm_panos
-Version: 0.6.1
+Version: 0.6.2
 Summary: Network Automation and Programmability Abstraction Layer with Multivendor support for PANOS.
 Home-page: https://github.com/napalm-automation/napalm-panos
 License: Apache-2.0
 Keywords: napalm,panos,napalm-panos
 Author: Gabriele Gerbino
 Author-email: gabriele@networktocode.com
 Requires-Python: >=3.8,<3.12
@@ -12,15 +12,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: cryptography (==3.3.2)
 Requires-Dist: lxml (>=5.0.0,<6.0.0)
 Requires-Dist: napalm (>=4.0.0,<5.0.0)
 Requires-Dist: netmiko (>=4.0.0,<5.0.0)
 Requires-Dist: pan-python
 Requires-Dist: requests-toolbelt
 Requires-Dist: xmltodict
 Project-URL: Documentation, https://github.com/napalm-automation/napalm-panos
```

