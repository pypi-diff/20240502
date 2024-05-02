# Comparing `tmp/ansys_grantami_recordlists-1.2.0a0.tar.gz` & `tmp/ansys_grantami_recordlists-1.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_grantami_recordlists-1.2.0a0.tar", max compression
+gzip compressed data, was "ansys_grantami_recordlists-1.2.0b0.tar", max compression
```

## Comparing `ansys_grantami_recordlists-1.2.0a0.tar` & `ansys_grantami_recordlists-1.2.0b0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      629 2024-04-04 15:47:44.276857 ansys_grantami_recordlists-1.2.0a0/AUTHORS
--rw-r--r--   0        0        0     1089 2024-04-04 15:47:44.276857 ansys_grantami_recordlists-1.2.0a0/LICENSE
--rw-r--r--   0        0        0     3897 2024-04-04 15:47:44.276857 ansys_grantami_recordlists-1.2.0a0/README.rst
--rw-r--r--   0        0        0     2417 2024-04-04 15:47:44.280858 ansys_grantami_recordlists-1.2.0a0/pyproject.toml
--rw-r--r--   0        0        0     1746 2024-04-04 15:47:44.280858 ansys_grantami_recordlists-1.2.0a0/src/ansys/grantami/recordlists/__init__.py
--rw-r--r--   0        0        0    31603 2024-04-04 15:47:44.280858 ansys_grantami_recordlists-1.2.0a0/src/ansys/grantami/recordlists/_connection.py
--rw-r--r--   0        0        0     1268 2024-04-04 15:47:44.280858 ansys_grantami_recordlists-1.2.0a0/src/ansys/grantami/recordlists/_logger.py
--rw-r--r--   0        0        0    28762 2024-04-04 15:47:44.280858 ansys_grantami_recordlists-1.2.0a0/src/ansys/grantami/recordlists/_models.py
--rw-r--r--   0        0        0        0 2024-04-04 15:47:44.280858 ansys_grantami_recordlists-1.2.0a0/src/ansys/grantami/recordlists/py.typed
--rw-r--r--   0        0        0     4977 1970-01-01 00:00:00.000000 ansys_grantami_recordlists-1.2.0a0/PKG-INFO
+-rw-r--r--   0        0        0      629 2024-04-22 16:38:11.243311 ansys_grantami_recordlists-1.2.0b0/AUTHORS
+-rw-r--r--   0        0        0     1089 2024-04-22 16:38:11.243311 ansys_grantami_recordlists-1.2.0b0/LICENSE
+-rw-r--r--   0        0        0     3897 2024-04-22 16:38:11.243311 ansys_grantami_recordlists-1.2.0b0/README.rst
+-rw-r--r--   0        0        0     2416 2024-04-22 16:38:11.247310 ansys_grantami_recordlists-1.2.0b0/pyproject.toml
+-rw-r--r--   0        0        0     1746 2024-04-22 16:38:11.247310 ansys_grantami_recordlists-1.2.0b0/src/ansys/grantami/recordlists/__init__.py
+-rw-r--r--   0        0        0    32212 2024-04-22 16:38:11.247310 ansys_grantami_recordlists-1.2.0b0/src/ansys/grantami/recordlists/_connection.py
+-rw-r--r--   0        0        0     1268 2024-04-22 16:38:11.247310 ansys_grantami_recordlists-1.2.0b0/src/ansys/grantami/recordlists/_logger.py
+-rw-r--r--   0        0        0    28762 2024-04-22 16:38:11.247310 ansys_grantami_recordlists-1.2.0b0/src/ansys/grantami/recordlists/_models.py
+-rw-r--r--   0        0        0        0 2024-04-22 16:38:11.247310 ansys_grantami_recordlists-1.2.0b0/src/ansys/grantami/recordlists/py.typed
+-rw-r--r--   0        0        0     4976 1970-01-01 00:00:00.000000 ansys_grantami_recordlists-1.2.0b0/PKG-INFO
```

### Comparing `ansys_grantami_recordlists-1.2.0a0/AUTHORS` & `ansys_grantami_recordlists-1.2.0b0/AUTHORS`

 * *Files identical despite different names*

### Comparing `ansys_grantami_recordlists-1.2.0a0/LICENSE` & `ansys_grantami_recordlists-1.2.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_grantami_recordlists-1.2.0a0/README.rst` & `ansys_grantami_recordlists-1.2.0b0/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_grantami_recordlists-1.2.0a0/pyproject.toml` & `ansys_grantami_recordlists-1.2.0b0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 # Check https://python-poetry.org/docs/pyproject/ for all available sections
 name = "ansys-grantami-recordlists"
-version = "1.2.0a0"
+version = "1.2.0b0"
 description = "A python wrapper for the Granta MI RecordLists API"
 license = "MIT"
 authors = ["ANSYS, Inc. <pyansys.core@ansys.com>"]
 maintainers = ["ANSYS, Inc. <pyansys.core@ansys.com>"]
 readme = "README.rst"
 repository = "https://github.com/ansys/grantami-recordlists"
 documentation = "https://recordlists.grantami.docs.pyansys.com"
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -26,15 +26,15 @@
 packages = [
     { include = "ansys", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 ansys-openapi-common = "^2.0.0"
-ansys-grantami-serverapi-openapi = "3.0.0a3"
+ansys-grantami-serverapi-openapi = "3.0.0b0"
 requests = "^2.26"
 
 # Optional documentation dependencies
 [tool.poetry.group.doc]
 optional = true
 
 [tool.poetry.group.doc.dependencies]
```

### Comparing `ansys_grantami_recordlists-1.2.0a0/src/ansys/grantami/recordlists/__init__.py` & `ansys_grantami_recordlists-1.2.0b0/src/ansys/grantami/recordlists/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_grantami_recordlists-1.2.0a0/src/ansys/grantami/recordlists/_connection.py` & `ansys_grantami_recordlists-1.2.0b0/src/ansys/grantami/recordlists/_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+from collections import defaultdict
 import concurrent.futures
-from typing import Dict, List, Optional, Tuple, Union
+from typing import List, Optional, Tuple, Union
 
 from ansys.grantami.serverapi_openapi import api, models  # type: ignore[import]
 from ansys.openapi.common import (  # type: ignore[import]
     ApiClient,
     ApiClientFactory,
     ApiException,
     SessionConfiguration,
@@ -201,14 +202,16 @@
     ) -> List[RecordListItem]:
         """
         Get all resolvable items included in a record list.
 
         If an item cannot be resolved, it will not be returned. Performs multiple HTTP requests
         against the Granta MI Server API.
 
+        .. versionadded:: 1.2
+
         Parameters
         ----------
         record_list : RecordList
             Record list for which items will be fetched.
         read_mode : bool
             Whether to enable read-mode for users who ordinarily have write permissions. Has no
             effect for read-only users.
@@ -602,15 +605,14 @@
 class _ItemResolver:
     _max_requests = 5
 
     def __init__(self, client: ApiClient, read_mode: bool) -> None:
         self._record_histories_api = api.RecordsRecordHistoriesApi(client)
         self._record_versions_api = api.RecordsRecordVersionsApi(client)
         self._db_schema_api = api.SchemaDatabasesApi(client)
-        self._db_map: Dict[str, str] = {}
         self._read_mode = read_mode
 
     def get_resolvable_items(self, all_items: List[RecordListItem]) -> List[RecordListItem]:
         """Test all items to see if they can be resolved as the current user.
 
         Uses concurrent.futures to handle threading, since openapi-common is currently based on
         requests which limits asyncio options.
@@ -621,60 +623,79 @@
             The items for which to check resolvability.
 
         Returns
         -------
         resolvable_items
             The items which could be resolved on the server.
         """
-        self._db_map = self._get_db_map()
+        db_map = self._get_db_map()
         with concurrent.futures.ThreadPoolExecutor(max_workers=self._max_requests) as executor:
             resolvable_test_futures = {
-                executor.submit(self._is_item_resolvable, i): i for i in all_items
+                executor.submit(self._is_item_resolvable, i, db_map): i for i in all_items
             }
             resolvable_items = [
                 resolvable_test_futures[f]
                 for f in concurrent.futures.as_completed(resolvable_test_futures)
                 if f.result()
             ]
         return resolvable_items
 
-    def _get_db_map(self) -> Dict[str, str]:
+    def _get_db_map(self) -> defaultdict[str, List[str]]:
         dbs = self._db_schema_api.get_all_databases()
-        return {db.guid: db.key for db in dbs.databases}
-
-    def _is_item_resolvable(self, item: RecordListItem) -> bool:
+        db_map: defaultdict[str, List[str]] = defaultdict(list)
+        for db in dbs.databases:
+            db_map[db.guid].append(db.key)
+        return db_map
+
+    def _is_item_resolvable(
+        self, item: RecordListItem, db_map: defaultdict[str, List[str]]
+    ) -> bool:
         """Test if a specific item is resolvable.
 
+        Returns
+        -------
+        bool
+            True if the item can be resolved in any database with the correct GUID, False otherwise.
+        """
+        if item.database_guid not in db_map:
+            return False
+        for db_key in db_map[item.database_guid]:
+            if self._is_item_resolvable_in_db(item, db_key):
+                return True
+        return False
+
+    def _is_item_resolvable_in_db(self, item: RecordListItem, db_key: str) -> bool:
+        """
+        Test if a specific item is resolvable in a database.
+
         If the item has a record version and record guid, attempt to resolve the record version
         directly.
 
         If the item has a record version number only, check that the version number is available
         to the user running the record.
 
         If there is no version at all, check that the history can be resolved.
 
         Returns
         -------
         bool
             True if the item can be resolved, False otherwise.
         """
-        if item.database_guid not in self._db_map:
-            return False
         try:
             if item.record_version is not None and item.record_guid is not None:
                 self._record_versions_api.get_record_version(
-                    database_key=self._db_map[item.database_guid],
+                    database_key=db_key,
                     table_guid=item.table_guid,
                     record_history_guid=item.record_history_guid,
                     record_version_guid=item.record_guid,
                     mode="read" if self._read_mode else None,
                 )
             else:
                 history_info = self._record_histories_api.get_record_history(
-                    database_key=self._db_map[item.database_guid],
+                    database_key=db_key,
                     record_history_guid=item.record_history_guid,
                     mode="read" if self._read_mode else None,
                 )
                 if item.record_version is not None:
                     for version in history_info.record_versions:
                         if item.record_version == version.version_number:
                             return True
```

### Comparing `ansys_grantami_recordlists-1.2.0a0/src/ansys/grantami/recordlists/_logger.py` & `ansys_grantami_recordlists-1.2.0b0/src/ansys/grantami/recordlists/_logger.py`

 * *Files identical despite different names*

### Comparing `ansys_grantami_recordlists-1.2.0a0/src/ansys/grantami/recordlists/_models.py` & `ansys_grantami_recordlists-1.2.0b0/src/ansys/grantami/recordlists/_models.py`

 * *Files identical despite different names*

### Comparing `ansys_grantami_recordlists-1.2.0a0/PKG-INFO` & `ansys_grantami_recordlists-1.2.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: ansys-grantami-recordlists
-Version: 1.2.0a0
+Version: 1.2.0b0
 Summary: A python wrapper for the Granta MI RecordLists API
 Home-page: https://github.com/ansys/grantami-recordlists
 License: MIT
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: ansys-grantami-serverapi-openapi (==3.0.0a3)
+Requires-Dist: ansys-grantami-serverapi-openapi (==3.0.0b0)
 Requires-Dist: ansys-openapi-common (>=2.0.0,<3.0.0)
 Requires-Dist: requests (>=2.26,<3.0)
 Project-URL: Documentation, https://recordlists.grantami.docs.pyansys.com
 Project-URL: Repository, https://github.com/ansys/grantami-recordlists
 Description-Content-Type: text/x-rst
 
 |pyansys| |python| |pypi| |GH-CI| |codecov| |MIT| |black| |pre-commit-ci|
```

