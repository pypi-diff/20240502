# Comparing `tmp/galaxy-files-24.0.0.tar.gz` & `tmp/galaxy_files-24.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-files-24.0.0.tar", last modified: Wed Apr  3 02:44:16 2024, max compression
+gzip compressed data, was "galaxy_files-24.0.1.tar", last modified: Thu May  2 13:47:21 2024, max compression
```

## Comparing `galaxy-files-24.0.0.tar` & `galaxy_files-24.0.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:16.762559 galaxy-files-24.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-04-03 02:44:16.762559 galaxy-files-24.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:16.754559 galaxy-files-24.0.0/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:16.754559 galaxy-files-24.0.0/galaxy/files/
--rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:16.758559 galaxy-files-24.0.0/galaxy/files/sources/
--rw-r--r--   0 runner    (1001) docker     (127)    18971 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/_pyfilesystem2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/_rdm.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/anvil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/base64.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/basespace.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/drs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/galaxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/googlecloudstorage.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/googledrive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/http.py
--rw-r--r--   0 runner    (1001) docker     (127)    15262 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/invenio.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/onedata.py
--rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/posix.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/s3fs.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/sources/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:16.758559 galaxy-files-24.0.0/galaxy/files/unittest_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/unittest_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/files/uris.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:16.762559 galaxy-files-24.0.0/galaxy_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-04-03 02:44:16.000000 galaxy-files-24.0.0/galaxy_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-03 02:44:16.000000 galaxy-files-24.0.0/galaxy_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:44:16.000000 galaxy-files-24.0.0/galaxy_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 02:44:16.000000 galaxy-files-24.0.0/galaxy_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:44:16.000000 galaxy-files-24.0.0/galaxy_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-03 02:44:16.762559 galaxy-files-24.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 02:43:42.000000 galaxy-files-24.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:21.893414 galaxy_files-24.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-05-02 13:47:21.893414 galaxy_files-24.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:21.889414 galaxy_files-24.0.1/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:21.889414 galaxy_files-24.0.1/galaxy/files/
+-rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:21.893414 galaxy_files-24.0.1/galaxy/files/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)    18971 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/_pyfilesystem2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7971 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/_rdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/anvil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/base64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/basespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/drs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/galaxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/googlecloudstorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15242 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/invenio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/onedata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/posix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/s3fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:21.893414 galaxy_files-24.0.1/galaxy/files/unittest_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/unittest_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/uris.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:21.893414 galaxy_files-24.0.1/galaxy_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-05-02 13:47:21.000000 galaxy_files-24.0.1/galaxy_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-02 13:47:21.000000 galaxy_files-24.0.1/galaxy_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:47:21.000000 galaxy_files-24.0.1/galaxy_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 13:47:21.000000 galaxy_files-24.0.1/galaxy_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:47:21.000000 galaxy_files-24.0.1/galaxy_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-02 13:47:21.893414 galaxy_files-24.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/test-requirements.txt
```

### Comparing `galaxy-files-24.0.0/HISTORY.rst` & `galaxy_files-24.0.1/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,30 @@
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
+* Invenio plugin fixes by `@davelopez <https://github.com/davelopez>`_ in `#17997 <https://github.com/galaxyproject/galaxy/pull/17997>`_
+
+============
+Enhancements
+============
+
+* Fix remote files sources error handling by `@davelopez <https://github.com/davelopez>`_ in `#18027 <https://github.com/galaxyproject/galaxy/pull/18027>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-files-24.0.0/LICENSE.txt` & `galaxy_files-24.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `galaxy-files-24.0.0/PKG-INFO` & `galaxy_files-24.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-files
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy file source framework and default plugins
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -46,14 +46,31 @@
 
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
+* Invenio plugin fixes by `@davelopez <https://github.com/davelopez>`_ in `#17997 <https://github.com/galaxyproject/galaxy/pull/17997>`_
+
+============
+Enhancements
+============
+
+* Fix remote files sources error handling by `@davelopez <https://github.com/davelopez>`_ in `#18027 <https://github.com/galaxyproject/galaxy/pull/18027>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-files-24.0.0/galaxy/files/__init__.py` & `galaxy_files-24.0.1/galaxy/files/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-24.0.0/galaxy/files/sources/__init__.py` & `galaxy_files-24.0.1/galaxy/files/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-24.0.0/galaxy/files/sources/_pyfilesystem2.py` & `galaxy_files-24.0.1/galaxy/files/sources/_pyfilesystem2.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,17 +8,22 @@
     Dict,
     List,
     Optional,
     Type,
 )
 
 import fs
+import fs.errors
 from fs.base import FS
 from typing_extensions import Unpack
 
+from galaxy.exceptions import (
+    AuthenticationRequired,
+    MessageException,
+)
 from . import (
     BaseFilesSource,
     FilesSourceOptions,
     FilesSourceProperties,
 )
 
 log = logging.getLogger(__name__)
@@ -38,27 +43,33 @@
 
     @abc.abstractmethod
     def _open_fs(self, user_context=None, opts: Optional[FilesSourceOptions] = None):
         """Subclasses must instantiate a PyFilesystem2 handle for this file system."""
 
     def _list(self, path="/", recursive=False, user_context=None, opts: Optional[FilesSourceOptions] = None):
         """Return dictionary of 'Directory's and 'File's."""
-
-        with self._open_fs(user_context=user_context, opts=opts) as h:
-            if recursive:
-                res: List[Dict[str, Any]] = []
-                for p, dirs, files in h.walk(path):
-                    to_dict = functools.partial(self._resource_info_to_dict, p)
-                    res.extend(map(to_dict, dirs))
-                    res.extend(map(to_dict, files))
-                return res
-            else:
-                res = h.scandir(path, namespaces=["details"])
-                to_dict = functools.partial(self._resource_info_to_dict, path)
-                return list(map(to_dict, res))
+        try:
+            with self._open_fs(user_context=user_context, opts=opts) as h:
+                if recursive:
+                    res: List[Dict[str, Any]] = []
+                    for p, dirs, files in h.walk(path):
+                        to_dict = functools.partial(self._resource_info_to_dict, p)
+                        res.extend(map(to_dict, dirs))
+                        res.extend(map(to_dict, files))
+                    return res
+                else:
+                    res = h.scandir(path, namespaces=["details"])
+                    to_dict = functools.partial(self._resource_info_to_dict, path)
+                    return list(map(to_dict, res))
+        except fs.errors.PermissionDenied as e:
+            raise AuthenticationRequired(
+                f"Permission Denied. Reason: {e}. Please check your credentials in your preferences for {self.label}."
+            )
+        except fs.errors.FSError as e:
+            raise MessageException(f"Problem listing file source path {path}. Reason: {e}") from e
 
     def _realize_to(self, source_path, native_path, user_context=None, opts: Optional[FilesSourceOptions] = None):
         with open(native_path, "wb") as write_file:
             self._open_fs(user_context=user_context, opts=opts).download(source_path, write_file)
 
     def _write_from(self, target_path, native_path, user_context=None, opts: Optional[FilesSourceOptions] = None):
         with open(native_path, "rb") as read_file:
```

### Comparing `galaxy-files-24.0.0/galaxy/files/sources/_rdm.py` & `galaxy_files-24.0.1/galaxy/files/sources/_rdm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 from typing import (
-    cast,
     List,
     NamedTuple,
     Optional,
 )
 
 from typing_extensions import Unpack
 
@@ -22,14 +21,15 @@
 
 OptionalUserContext = Optional[ProvidesUserFileSourcesUserContext]
 
 
 class RDMFilesSourceProperties(FilesSourceProperties):
     url: str
     token: str
+    public_name: str
 
 
 class RecordFilename(NamedTuple):
     record_id: str
     filename: str
 
 
@@ -76,15 +76,17 @@
     ) -> List[RemoteFile]:
         """Returns the list of files contained in the given record.
 
         If writeable is True, we are signaling that the user intends to write to the record.
         """
         raise NotImplementedError()
 
-    def create_draft_record(self, title: str, user_context: OptionalUserContext = None):
+    def create_draft_record(
+        self, title: str, public_name: Optional[str] = None, user_context: OptionalUserContext = None
+    ):
         """Creates a draft record (directory) in the repository with basic metadata.
 
         The metadata is usually just the title of the record and the user that created it.
         Some plugins might also provide additional metadata defaults in the user settings."""
         raise NotImplementedError()
 
     def upload_file_to_draft_record(
@@ -134,30 +136,25 @@
 
     """
 
     plugin_kind = PluginKind.rdm
 
     def __init__(self, **kwd: Unpack[FilesSourceProperties]):
         props = self._parse_common_config_opts(kwd)
-        base_url = props.get("url", None)
+        base_url = props.get("url")
         if not base_url:
             raise Exception("URL for RDM repository must be provided in configuration")
         self._repository_url = base_url
-        self._token = props.get("token", None)
         self._props = props
         self._repository_interactor = self.get_repository_interactor(base_url)
 
     @property
     def repository(self) -> RDMRepositoryInteractor:
         return self._repository_interactor
 
-    @property
-    def token(self) -> Optional[str]:
-        return self._token if self._token and not self._token.startswith("$") else None
-
     def get_repository_interactor(self, repository_url: str) -> RDMRepositoryInteractor:
         """Returns an interactor compatible with the given repository URL.
 
         This must be implemented by subclasses."""
         raise NotImplementedError()
 
     def parse_path(self, source_path: str, record_id_only: bool = False) -> RecordFilename:
@@ -186,29 +183,27 @@
             raise ValueError(get_error_msg("Too many parts. Please provide the record_id and file_name only."))
         record_id, file_name = parts
         return RecordFilename(record_id=record_id, filename=file_name)
 
     def get_record_id_from_path(self, source_path: str) -> str:
         return self.parse_path(source_path, record_id_only=True).record_id
 
-    def _serialization_props(self, user_context: OptionalUserContext = None) -> RDMFilesSourceProperties:
+    def _serialization_props(self, user_context: OptionalUserContext = None):
         effective_props = {}
         for key, val in self._props.items():
             effective_props[key] = self._evaluate_prop(val, user_context=user_context)
-        effective_props["url"] = self._repository_url
-        effective_props["token"] = self.safe_get_authorization_token(user_context)
-        return cast(RDMFilesSourceProperties, effective_props)
+        return effective_props
 
     def get_authorization_token(self, user_context: OptionalUserContext) -> str:
-        token = self.token
-        if not token and user_context:
-            vault = user_context.user_vault if user_context else None
-            token = vault.read_secret(f"preferences/{self.id}/token") if vault else None
-        if token is None:
-            raise AuthenticationRequired(f"No authorization token provided in user's settings for '{self.label}'")
+        token = None
+        if user_context:
+            effective_props = self._serialization_props(user_context)
+            token = effective_props.get("token")
+        if not token:
+            raise AuthenticationRequired(
+                f"Please provide a personal access token in your user's preferences for '{self.label}'"
+            )
         return token
 
-    def safe_get_authorization_token(self, user_context: OptionalUserContext) -> Optional[str]:
-        try:
-            return self.get_authorization_token(user_context)
-        except AuthenticationRequired:
-            return None
+    def get_public_name(self, user_context: OptionalUserContext) -> Optional[str]:
+        effective_props = self._serialization_props(user_context)
+        return effective_props.get("public_name")
```

### Comparing `galaxy-files-24.0.0/galaxy/files/sources/anvil.py` & `galaxy_files-24.0.1/galaxy/files/sources/anvil.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-24.0.0/galaxy/files/sources/base64.py` & `galaxy_files-24.0.1/galaxy/files/sources/base64.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-24.0.0/galaxy/files/sources/basespace.py` & `galaxy_files-24.0.1/galaxy/files/sources/basespace.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-24.0.0/galaxy/files/sources/dropbox.py` & `galaxy_files-24.0.1/galaxy/files/sources/ssh.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 try:
-    from fs.dropboxfs import DropboxFS
+    from fs.sshfs import SSHFS
 except ImportError:
-    DropboxFS = None
+    SSHFS = None
 
 from typing import (
     Optional,
     Union,
 )
 
 from . import (
     FilesSourceOptions,
     FilesSourceProperties,
 )
 from ._pyfilesystem2 import PyFilesystem2FilesSource
 
 
-class DropboxFilesSource(PyFilesystem2FilesSource):
-    plugin_type = "dropbox"
-    required_module = DropboxFS
-    required_package = "fs.dropboxfs"
+class SshFilesSource(PyFilesystem2FilesSource):
+    plugin_type = "ssh"
+    required_module = SSHFS
+    required_package = "fs.sshfs"
 
     def _open_fs(self, user_context=None, opts: Optional[FilesSourceOptions] = None):
         props = self._serialization_props(user_context)
         extra_props: Union[FilesSourceProperties, dict] = opts.extra_props or {} if opts else {}
-        # accessToken has been renamed to access_token in fs.dropboxfs 1.0
-        if "accessToken" in props:
-            props["access_token"] = props.pop("accessToken")
-
-        handle = DropboxFS(**{**props, **extra_props})
+        path = props.pop("path")
+        handle = SSHFS(**{**props, **extra_props})
+        if path:
+            handle = handle.opendir(path)
         return handle
 
 
-__all__ = ("DropboxFilesSource",)
+__all__ = ("SshFilesSource",)
```

### Comparing `galaxy-files-24.0.0/galaxy/files/sources/drs.py` & `galaxy_files-24.0.1/galaxy/files/sources/drs.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-24.0.0/galaxy/files/sources/ftp.py` & `galaxy_files-24.0.1/galaxy/files/sources/ftp.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-24.0.0/galaxy/files/sources/galaxy.py` & `galaxy_files-24.0.1/galaxy/files/sources/galaxy.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-24.0.0/galaxy/files/sources/googlecloudstorage.py` & `galaxy_files-24.0.1/galaxy/files/sources/googlecloudstorage.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-24.0.0/galaxy/files/sources/googledrive.py` & `galaxy_files-24.0.1/galaxy/files/sources/googledrive.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-24.0.0/galaxy/files/sources/http.py` & `galaxy_files-24.0.1/galaxy/files/sources/http.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-24.0.0/galaxy/files/sources/invenio.py` & `galaxy_files-24.0.1/galaxy/files/sources/invenio.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,15 +131,16 @@
 
     def _create_entry(
         self,
         entry_data: EntryData,
         user_context: OptionalUserContext = None,
         opts: Optional[FilesSourceOptions] = None,
     ) -> Entry:
-        record = self.repository.create_draft_record(entry_data["name"], user_context=user_context)
+        public_name = self.get_public_name(user_context)
+        record = self.repository.create_draft_record(entry_data["name"], public_name, user_context=user_context)
         return {
             "uri": self.repository.to_plugin_uri(record["id"]),
             "name": record["metadata"]["title"],
             "external_link": record["links"]["self_html"],
         }
 
     def _realize_to(
@@ -194,17 +195,19 @@
         self, record_id: str, writeable: bool, user_context: OptionalUserContext = None
     ) -> List[RemoteFile]:
         conditionally_draft = "/draft" if writeable else ""
         request_url = f"{self.records_url}/{record_id}{conditionally_draft}/files"
         response_data = self._get_response(user_context, request_url)
         return self._get_record_files_from_response(record_id, response_data)
 
-    def create_draft_record(self, title: str, user_context: OptionalUserContext = None) -> RemoteDirectory:
+    def create_draft_record(
+        self, title: str, public_name: Optional[str] = None, user_context: OptionalUserContext = None
+    ) -> RemoteDirectory:
         today = datetime.date.today().isoformat()
-        creator = self._get_creator_from_user_context(user_context)
+        creator = self._get_creator_from_public_name(public_name)
         create_record_request = {
             "files": {"enabled": True},
             "metadata": {
                 "title": title,
                 "publication_date": today,
                 "resource_type": {"id": "dataset"},
                 "creators": [
@@ -356,31 +359,34 @@
                         "ctime": entry["created"],
                         "uri": uri,
                         "path": path,
                     }
                 )
         return rval
 
-    def _get_creator_from_user_context(self, user_context: OptionalUserContext):
-        public_name = self.get_user_preference_by_key("public_name", user_context)
-        family_name = "Galaxy User"
+    def _get_creator_from_public_name(self, public_name: Optional[str] = None) -> Creator:
         given_name = "Anonymous"
+        family_name = "Galaxy User"
         if public_name:
             tokens = public_name.split(", ")
             if len(tokens) == 2:
                 family_name = tokens[0]
                 given_name = tokens[1]
             else:
                 given_name = public_name
-        return {"person_or_org": {"family_name": family_name, "given_name": given_name, "type": "personal"}}
-
-    def get_user_preference_by_key(self, key: str, user_context: OptionalUserContext):
-        preferences = user_context.preferences if user_context else None
-        value = preferences.get(f"{self.plugin.id}|{key}", None) if preferences else None
-        return value
+        return {
+            "person_or_org": {
+                "name": f"{given_name} {family_name}",
+                "family_name": family_name,
+                "given_name": given_name,
+                "type": "personal",
+                "identifiers": [],
+            },
+            "affiliations": [],
+        }
 
     def _get_response(
         self, user_context: OptionalUserContext, request_url: str, params: Optional[Dict[str, Any]] = None
     ) -> dict:
         headers = self._get_request_headers(user_context)
         response = requests.get(request_url, params=params, headers=headers)
         self._ensure_response_has_expected_status_code(response, 200)
```

### Comparing `galaxy-files-24.0.0/galaxy/files/sources/onedata.py` & `galaxy_files-24.0.1/galaxy/files/sources/onedata.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-24.0.0/galaxy/files/sources/posix.py` & `galaxy_files-24.0.1/galaxy/files/sources/posix.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-24.0.0/galaxy/files/sources/s3fs.py` & `galaxy_files-24.0.1/galaxy/files/sources/s3fs.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-24.0.0/galaxy/files/sources/ssh.py` & `galaxy_files-24.0.1/galaxy/files/sources/webdav.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 try:
-    from fs.sshfs import SSHFS
+    from webdavfs.webdavfs import WebDAVFS
 except ImportError:
-    SSHFS = None
+    WebDAVFS = None
 
+import tempfile
 from typing import (
     Optional,
     Union,
 )
 
 from . import (
     FilesSourceOptions,
     FilesSourceProperties,
 )
 from ._pyfilesystem2 import PyFilesystem2FilesSource
 
 
-class SshFilesSource(PyFilesystem2FilesSource):
-    plugin_type = "ssh"
-    required_module = SSHFS
-    required_package = "fs.sshfs"
+class WebDavFilesSource(PyFilesystem2FilesSource):
+    plugin_type = "webdav"
+    required_module = WebDAVFS
+    required_package = "fs.webdavfs"
 
     def _open_fs(self, user_context=None, opts: Optional[FilesSourceOptions] = None):
         props = self._serialization_props(user_context)
+        use_temp_files = props.pop("use_temp_files", None)
+        if use_temp_files is None:
+            # Default to True to avoid memory issues with large files.
+            props["use_temp_files"] = True
+            props["temp_path"] = props.get("temp_path", tempfile.TemporaryDirectory(prefix="webdav_"))
         extra_props: Union[FilesSourceProperties, dict] = opts.extra_props or {} if opts else {}
-        path = props.pop("path")
-        handle = SSHFS(**{**props, **extra_props})
-        if path:
-            handle = handle.opendir(path)
+        handle = WebDAVFS(**{**props, **extra_props})
         return handle
 
 
-__all__ = ("SshFilesSource",)
+__all__ = ("WebDavFilesSource",)
```

### Comparing `galaxy-files-24.0.0/galaxy/files/unittest_utils/__init__.py` & `galaxy_files-24.0.1/galaxy/files/unittest_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-24.0.0/galaxy/files/uris.py` & `galaxy_files-24.0.1/galaxy/files/uris.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-24.0.0/galaxy_files.egg-info/PKG-INFO` & `galaxy_files-24.0.1/galaxy_files.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-files
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy file source framework and default plugins
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -46,14 +46,31 @@
 
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
+* Invenio plugin fixes by `@davelopez <https://github.com/davelopez>`_ in `#17997 <https://github.com/galaxyproject/galaxy/pull/17997>`_
+
+============
+Enhancements
+============
+
+* Fix remote files sources error handling by `@davelopez <https://github.com/davelopez>`_ in `#18027 <https://github.com/galaxyproject/galaxy/pull/18027>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-files-24.0.0/galaxy_files.egg-info/SOURCES.txt` & `galaxy_files-24.0.1/galaxy_files.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-files-24.0.0/setup.cfg` & `galaxy_files-24.0.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-files
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.0
+version = 24.0.1
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
 	fs
 	isal
```

