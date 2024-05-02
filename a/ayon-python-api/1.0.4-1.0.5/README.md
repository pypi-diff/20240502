# Comparing `tmp/ayon-python-api-1.0.4.tar.gz` & `tmp/ayon-python-api-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayon-python-api-1.0.4.tar", last modified: Thu Apr 25 12:55:29 2024, max compression
+gzip compressed data, was "ayon-python-api-1.0.5.tar", last modified: Thu May  2 14:20:29 2024, max compression
```

## Comparing `ayon-python-api-1.0.4.tar` & `ayon-python-api-1.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:55:29.283039 ayon-python-api-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 12:55:23.000000 ayon-python-api-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-04-25 12:55:29.283039 ayon-python-api-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-25 12:55:23.000000 ayon-python-api-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:55:29.279039 ayon-python-api-1.0.4/ayon_api/
--rw-r--r--   0 runner    (1001) docker     (127)    10045 2024-04-25 12:55:23.000000 ayon-python-api-1.0.4/ayon_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   123859 2024-04-25 12:55:23.000000 ayon-python-api-1.0.4/ayon_api/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-25 12:55:23.000000 ayon-python-api-1.0.4/ayon_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    86148 2024-04-25 12:55:23.000000 ayon-python-api-1.0.4/ayon_api/entity_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-25 12:55:23.000000 ayon-python-api-1.0.4/ayon_api/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-25 12:55:23.000000 ayon-python-api-1.0.4/ayon_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25889 2024-04-25 12:55:23.000000 ayon-python-api-1.0.4/ayon_api/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)    21938 2024-04-25 12:55:23.000000 ayon-python-api-1.0.4/ayon_api/graphql_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)    42241 2024-04-25 12:55:23.000000 ayon-python-api-1.0.4/ayon_api/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)   247665 2024-04-25 12:55:23.000000 ayon-python-api-1.0.4/ayon_api/server_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18155 2024-04-25 12:55:23.000000 ayon-python-api-1.0.4/ayon_api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-25 12:55:23.000000 ayon-python-api-1.0.4/ayon_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:55:29.279039 ayon-python-api-1.0.4/ayon_python_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-04-25 12:55:29.000000 ayon-python-api-1.0.4/ayon_python_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-25 12:55:29.000000 ayon-python-api-1.0.4/ayon_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 12:55:29.000000 ayon-python-api-1.0.4/ayon_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-25 12:55:29.000000 ayon-python-api-1.0.4/ayon_python_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 12:55:29.000000 ayon-python-api-1.0.4/ayon_python_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-25 12:55:23.000000 ayon-python-api-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 12:55:29.283039 ayon-python-api-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-25 12:55:23.000000 ayon-python-api-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:20:29.665975 ayon-python-api-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 14:20:25.000000 ayon-python-api-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-05-02 14:20:29.661975 ayon-python-api-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-02 14:20:25.000000 ayon-python-api-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:20:29.661975 ayon-python-api-1.0.5/ayon_api/
+-rw-r--r--   0 runner    (1001) docker     (127)    10091 2024-05-02 14:20:25.000000 ayon-python-api-1.0.5/ayon_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   125425 2024-05-02 14:20:25.000000 ayon-python-api-1.0.5/ayon_api/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-02 14:20:25.000000 ayon-python-api-1.0.5/ayon_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86920 2024-05-02 14:20:25.000000 ayon-python-api-1.0.5/ayon_api/entity_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-02 14:20:25.000000 ayon-python-api-1.0.5/ayon_api/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-02 14:20:25.000000 ayon-python-api-1.0.5/ayon_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25889 2024-05-02 14:20:25.000000 ayon-python-api-1.0.5/ayon_api/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21938 2024-05-02 14:20:25.000000 ayon-python-api-1.0.5/ayon_api/graphql_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42241 2024-05-02 14:20:25.000000 ayon-python-api-1.0.5/ayon_api/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)   249395 2024-05-02 14:20:25.000000 ayon-python-api-1.0.5/ayon_api/server_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18155 2024-05-02 14:20:25.000000 ayon-python-api-1.0.5/ayon_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-02 14:20:25.000000 ayon-python-api-1.0.5/ayon_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:20:29.661975 ayon-python-api-1.0.5/ayon_python_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-05-02 14:20:29.000000 ayon-python-api-1.0.5/ayon_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-02 14:20:29.000000 ayon-python-api-1.0.5/ayon_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:20:29.000000 ayon-python-api-1.0.5/ayon_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-02 14:20:29.000000 ayon-python-api-1.0.5/ayon_python_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 14:20:29.000000 ayon-python-api-1.0.5/ayon_python_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-02 14:20:25.000000 ayon-python-api-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 14:20:29.665975 ayon-python-api-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-02 14:20:25.000000 ayon-python-api-1.0.5/setup.py
```

### Comparing `ayon-python-api-1.0.4/LICENSE` & `ayon-python-api-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.4/PKG-INFO` & `ayon-python-api-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayon-python-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: AYON Python API
 Home-page: https://github.com/ynput/ayon-python-api
 Author: ynput.io
 Author-email: "ynput.io" <info@ynput.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ayon-python-api-1.0.4/README.md` & `ayon-python-api-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.4/ayon_api/__init__.py` & `ayon-python-api-1.0.5/ayon_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,14 +114,15 @@
     get_secret,
     save_secret,
     delete_secret,
     get_rest_project,
     get_rest_projects,
     get_rest_entity_by_id,
     get_rest_folder,
+    get_rest_folders,
     get_rest_task,
     get_rest_product,
     get_rest_version,
     get_rest_representation,
     get_project_names,
     get_projects,
     get_project,
@@ -325,14 +326,15 @@
     "get_secret",
     "save_secret",
     "delete_secret",
     "get_rest_project",
     "get_rest_projects",
     "get_rest_entity_by_id",
     "get_rest_folder",
+    "get_rest_folders",
     "get_rest_task",
     "get_rest_product",
     "get_rest_version",
     "get_rest_representation",
     "get_project_names",
     "get_projects",
     "get_project",
```

### Comparing `ayon-python-api-1.0.4/ayon_api/_api.py` & `ayon-python-api-1.0.5/ayon_api/_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1913,14 +1913,59 @@
 
 
 def get_rest_folder(*args, **kwargs):
     con = get_server_api_connection()
     return con.get_rest_folder(*args, **kwargs)
 
 
+def get_rest_folders(*args, **kwargs):
+    """Get simplified flat list of all project folders.
+
+    Get all project folders in single REST call. This can be faster than
+        using 'get_folders' method which is using GraphQl, but does not
+        allow any filtering, and set of fields is defined
+        by server backend.
+
+    Example::
+
+        [
+            {
+                "id": "112233445566",
+                "parentId": "112233445567",
+                "path": "/root/parent/child",
+                "parents": ["root", "parent"],
+                "name": "child",
+                "label": "Child",
+                "folderType": "Folder",
+                "hasTasks": False,
+                "hasChildren": False,
+                "taskNames": [
+                    "Compositing",
+                ],
+                "status": "In Progress",
+                "attrib": {},
+                "ownAttrib": [],
+                "updatedAt": "2023-06-12T15:37:02.420260",
+            },
+            ...
+        ]
+
+    Args:
+        project_name (str): Project name.
+        include_attrib (Optional[bool]): Include attribute values
+            in output. Slower to query.
+
+    Returns:
+        list[dict[str, Any]]: List of folder entities.
+
+    """
+    con = get_server_api_connection()
+    return con.get_rest_folders(*args, **kwargs)
+
+
 def get_rest_task(*args, **kwargs):
     con = get_server_api_connection()
     return con.get_rest_task(*args, **kwargs)
 
 
 def get_rest_product(*args, **kwargs):
     con = get_server_api_connection()
@@ -2061,14 +2106,20 @@
                 "attrib": {},
                 "ownAttrib": [],
                 "updatedAt": "2023-06-12T15:37:02.420260",
             },
             ...
         ]
 
+    Deprecated:
+        Use 'get_rest_folders' instead. Function was renamed to match
+            other rest functions, like 'get_rest_folder',
+            'get_rest_project' etc. .
+        Will be removed in '1.0.7' or '1.1.0'.
+
     Args:
         project_name (str): Project name.
         include_attrib (Optional[bool]): Include attribute values
             in output. Slower to query.
 
     Returns:
         list[dict[str, Any]]: List of folder entities.
```

### Comparing `ayon-python-api-1.0.4/ayon_api/constants.py` & `ayon-python-api-1.0.5/ayon_api/constants.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.4/ayon_api/entity_hub.py` & `ayon-python-api-1.0.5/ayon_api/entity_hub.py`

 * *Files 0% similar despite different names*

```diff
@@ -2581,14 +2581,15 @@
     def _immutable_for_hierarchy(self):
         if self.has_published_content:
             return True
         return None
 
     def lock(self):
         super(FolderEntity, self).lock()
+        self._orig_label = self._get_label_value()
         self._orig_folder_type = self._folder_type
         self._orig_status = self._status
         self._orig_tags = copy.deepcopy(self._tags)
 
     @property
     def changes(self):
         changes = self._get_default_changes()
@@ -2604,18 +2605,15 @@
 
         if self._orig_status != self._status:
             changes["status"] = self._status
 
         if self._orig_tags != self._tags:
             changes["tags"] = self._tags
 
-        label = self._label
-        if self._name == label:
-            label = None
-
+        label = self._get_label_value()
         if label != self._orig_label:
             changes["label"] = label
 
         return changes
 
     @classmethod
     def from_entity_data(cls, folder, entity_hub):
@@ -2651,14 +2649,18 @@
             raise ValueError("Folder does not have set 'name'")
 
         output = {
             "name": self.name,
             "folderType": self.folder_type,
             "parentId": parent_id,
         }
+        label = self._get_label_value()
+        if label:
+            output["label"] = label
+
         attrib = self.attribs.to_dict()
         if attrib:
             output["attrib"] = attrib
 
         # Add tags only if are available
         if self.tags:
             output["tags"] = list(self.tags)
@@ -2675,14 +2677,26 @@
         if (
             self._entity_hub.allow_data_changes
             and self._data is not UNKNOWN_VALUE
         ):
             output["data"] = self._data
         return output
 
+    def _get_label_value(self):
+        """Get label value that will be used for operations.
+
+        Returns:
+            Union[str, None]: Label value.
+
+        """
+        label = self._label
+        if not label or self._name == label:
+            return None
+        return label
+
 
 class TaskEntity(BaseEntity):
     """Entity representing a task on AYON server.
 
     Args:
         task_type (str): Type of task. Task type must be available in config
             of project task types.
@@ -2730,14 +2744,15 @@
         self._orig_status = status
         self._orig_tags = copy.deepcopy(tags)
 
         self._children_ids = set()
 
     def lock(self):
         super(TaskEntity, self).lock()
+        self._orig_label = self._get_label_value()
         self._orig_task_type = self._task_type
         self._orig_status = self._status
         self._orig_tags = copy.deepcopy(self._tags)
 
     def get_task_type(self):
         return self._task_type
 
@@ -2815,18 +2830,15 @@
 
         if self._orig_status != self._status:
             changes["status"] = self._status
 
         if self._orig_tags != self._tags:
             changes["tags"] = self._tags
 
-        label = self._label
-        if self._name == label:
-            label = None
-
+        label = self._get_label_value()
         if label != self._orig_label:
             changes["label"] = label
 
         return changes
 
     @classmethod
     def from_entity_data(cls, task, entity_hub):
@@ -2851,14 +2863,18 @@
 
         output = {
             "name": self.name,
             "taskType": self.task_type,
             "folderId": self.parent_id,
             "attrib": self.attribs.to_dict(),
         }
+        label = self._get_label_value()
+        if label:
+            output["label"] = label
+
         attrib = self.attribs.to_dict()
         if attrib:
             output["attrib"] = attrib
 
         if self.active is not UNKNOWN_VALUE:
             output["active"] = self.active
 
@@ -2870,7 +2886,19 @@
 
         if (
             self._entity_hub.allow_data_changes
             and self._data is not UNKNOWN_VALUE
         ):
             output["data"] = self._data
         return output
+
+    def _get_label_value(self):
+        """Get label value that will be used for operations.
+
+        Returns:
+            Union[str, None]: Label value.
+
+        """
+        label = self._label
+        if not label or self._name == label:
+            return None
+        return label
```

### Comparing `ayon-python-api-1.0.4/ayon_api/events.py` & `ayon-python-api-1.0.5/ayon_api/events.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.4/ayon_api/exceptions.py` & `ayon-python-api-1.0.5/ayon_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.4/ayon_api/graphql.py` & `ayon-python-api-1.0.5/ayon_api/graphql.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.4/ayon_api/graphql_queries.py` & `ayon-python-api-1.0.5/ayon_api/graphql_queries.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.4/ayon_api/operations.py` & `ayon-python-api-1.0.5/ayon_api/operations.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.4/ayon_api/server_api.py` & `ayon-python-api-1.0.5/ayon_api/server_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -3379,14 +3379,70 @@
         if response.status == 200:
             return response.data
         return None
 
     def get_rest_folder(self, project_name, folder_id):
         return self.get_rest_entity_by_id(project_name, "folder", folder_id)
 
+    def get_rest_folders(self, project_name, include_attrib=False):
+        """Get simplified flat list of all project folders.
+
+        Get all project folders in single REST call. This can be faster than
+            using 'get_folders' method which is using GraphQl, but does not
+            allow any filtering, and set of fields is defined
+            by server backend.
+
+        Example::
+
+            [
+                {
+                    "id": "112233445566",
+                    "parentId": "112233445567",
+                    "path": "/root/parent/child",
+                    "parents": ["root", "parent"],
+                    "name": "child",
+                    "label": "Child",
+                    "folderType": "Folder",
+                    "hasTasks": False,
+                    "hasChildren": False,
+                    "taskNames": [
+                        "Compositing",
+                    ],
+                    "status": "In Progress",
+                    "attrib": {},
+                    "ownAttrib": [],
+                    "updatedAt": "2023-06-12T15:37:02.420260",
+                },
+                ...
+            ]
+
+        Args:
+            project_name (str): Project name.
+            include_attrib (Optional[bool]): Include attribute values
+                in output. Slower to query.
+
+        Returns:
+            list[dict[str, Any]]: List of folder entities.
+
+        """
+        major, minor, patch, _, _ = self.server_version_tuple
+        if (major, minor, patch) < (1, 0, 8):
+            raise UnsupportedServerVersion(
+                "Function 'get_folders_rest' is supported"
+                " for AYON server 1.0.8 and above."
+            )
+        query = "?attrib={}".format(
+            "true" if include_attrib else "false"
+        )
+        response = self.get(
+            "projects/{}/folders{}".format(project_name, query)
+        )
+        response.raise_for_status()
+        return response.data["folders"]
+
     def get_rest_task(self, project_name, task_id):
         return self.get_rest_entity_by_id(project_name, "task", task_id)
 
     def get_rest_product(self, project_name, product_id):
         return self.get_rest_entity_by_id(project_name, "product", product_id)
 
     def get_rest_version(self, project_name, version_id):
@@ -3643,37 +3699,30 @@
                     "attrib": {},
                     "ownAttrib": [],
                     "updatedAt": "2023-06-12T15:37:02.420260",
                 },
                 ...
             ]
 
+        Deprecated:
+            Use 'get_rest_folders' instead. Function was renamed to match
+                other rest functions, like 'get_rest_folder',
+                'get_rest_project' etc. .
+            Will be removed in '1.0.7' or '1.1.0'.
+
         Args:
             project_name (str): Project name.
             include_attrib (Optional[bool]): Include attribute values
                 in output. Slower to query.
 
         Returns:
             list[dict[str, Any]]: List of folder entities.
 
         """
-        major, minor, patch, _, _ = self.server_version_tuple
-        if (major, minor, patch) < (1, 0, 8):
-            raise UnsupportedServerVersion(
-                "Function 'get_folders_rest' is supported"
-                " for AYON server 1.0.8 and above."
-            )
-        query = "?attrib={}".format(
-            "true" if include_attrib else "false"
-        )
-        response = self.get(
-            "projects/{}/folders{}".format(project_name, query)
-        )
-        response.raise_for_status()
-        return response.data["folders"]
+        return self.get_rest_folders(project_name, include_attrib)
 
     def get_folders(
         self,
         project_name,
         folder_ids=None,
         folder_paths=None,
         folder_names=None,
```

### Comparing `ayon-python-api-1.0.4/ayon_api/utils.py` & `ayon-python-api-1.0.5/ayon_api/utils.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.4/ayon_python_api.egg-info/PKG-INFO` & `ayon-python-api-1.0.5/ayon_python_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayon-python-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: AYON Python API
 Home-page: https://github.com/ynput/ayon-python-api
 Author: ynput.io
 Author-email: "ynput.io" <info@ynput.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ayon-python-api-1.0.4/pyproject.toml` & `ayon-python-api-1.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ayon-python-api"
-version = "1.0.4"
+version = "1.0.5"
 description = "AYON Python API"
 license = {file = "LICENSE"}
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [
     {name = "ynput.io", email = "info@ynput.io"}
 ]
 keywords = ["AYON", "ynput", "OpenPype", "vfx"]
@@ -27,15 +27,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ayon-python-api"
-version = "1.0.4"
+version = "1.0.5"
 description = "AYON Python API"
 authors = [
     "ynput.io <info@ynput.io>"
 ]
 
 [tool.poetry.dependencies]
 python = ">=2.7,>=3.6.5"
```

### Comparing `ayon-python-api-1.0.4/setup.py` & `ayon-python-api-1.0.5/setup.py`

 * *Files identical despite different names*

